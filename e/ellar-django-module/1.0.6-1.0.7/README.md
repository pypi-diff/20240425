# Comparing `tmp/ellar_django_module-1.0.6.tar.gz` & `tmp/ellar_django_module-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ellar_django_module-1.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ellar_django_module-1.0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ellar_django_module-1.0.6.tar` & `ellar_django_module-1.0.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     7330 2024-04-23 18:48:39.706184 ellar_django_module-1.0.6/README.md
--rw-r--r--   0        0        0      158 2024-04-23 18:48:39.706184 ellar_django_module-1.0.6/ellar_django/__init__.py
--rw-r--r--   0        0        0     2228 2024-04-23 18:48:39.706184 ellar_django_module-1.0.6/ellar_django/commands.py
--rw-r--r--   0        0        0     1424 2024-04-23 18:48:39.706184 ellar_django_module-1.0.6/ellar_django/middleware.py
--rw-r--r--   0        0        0     1391 2024-04-23 18:48:39.706184 ellar_django_module-1.0.6/ellar_django/module.py
--rw-r--r--   0        0        0     2329 2024-04-23 18:48:39.706184 ellar_django_module-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     9188 1970-01-01 00:00:00.000000 ellar_django_module-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     7330 2024-04-25 13:46:19.967184 ellar_django_module-1.0.7/README.md
+-rw-r--r--   0        0        0      158 2024-04-25 13:46:19.967184 ellar_django_module-1.0.7/ellar_django/__init__.py
+-rw-r--r--   0        0        0     2762 2024-04-25 13:46:19.967184 ellar_django_module-1.0.7/ellar_django/commands.py
+-rw-r--r--   0        0        0     1424 2024-04-25 13:46:19.967184 ellar_django_module-1.0.7/ellar_django/middleware.py
+-rw-r--r--   0        0        0     1798 2024-04-25 13:46:19.967184 ellar_django_module-1.0.7/ellar_django/module.py
+-rw-r--r--   0        0        0     2329 2024-04-25 13:46:19.967184 ellar_django_module-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     9188 1970-01-01 00:00:00.000000 ellar_django_module-1.0.7/PKG-INFO
```

### Comparing `ellar_django_module-1.0.6/README.md` & `ellar_django_module-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ellar_django_module-1.0.6/ellar_django/commands.py` & `ellar_django_module-1.0.7/ellar_django/commands.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,86 +1,93 @@
 import typing as t
 
 import django
 import ellar_cli.click as click
 from django.core.management import get_commands, load_command_class
 
-BLACKLISTED_COMMANDS: t.Final[t.Set[str]] = {
-    "runserver",
-    "startapp",
-    "startproject",
-}
-
 
 class _CommandItem(t.NamedTuple):
     name: str
     description: str
 
 
 def get_command_description(command_name: str) -> str:
     module = get_commands()[command_name]
     CommandClass = load_command_class(module, command_name)
-    return CommandClass.help or ""
+    CommandClass.help = f"[{module.split('.')[0]}] {CommandClass.help}"
+    return CommandClass.help
 
 
-def generate_command_list() -> t.List[_CommandItem]:
+def _generate_command_list(
+    blacklist_commands: t.Set[str],
+) -> t.Generator[_CommandItem, None, None]:
     commands = get_commands()
-    command_list: t.List[_CommandItem] = []
     for command in commands:
-        if command in BLACKLISTED_COMMANDS:
+        if command in blacklist_commands:
             continue
         description = get_command_description(command)
-        command_list.append(_CommandItem(name=command, description=description))
-    return command_list
-
+        yield _CommandItem(name=command, description=description)
 
-_django_support_commands = generate_command_list()
 
-
-def version_callback(ctx: click.Context, _: t.Any, value: bool) -> None:
+def version_callback(ctx: click.Context, _: click.Parameter, value: bool) -> None:
     if value:
         click.echo(f"Django Version: {django.__version__}")
         ctx.exit()
 
 
-@click.group(
-    name="django",
-    help="- Ellar Django Commands",
-)
-@click.option(
-    "-v",
-    "--version",
-    callback=version_callback,
-    help="Show the version and exit.",
-    is_flag=True,
-    expose_value=False,
-    is_eager=True,
-)
-@click.pass_context
-def django_command(ctx: click.Context) -> None:
-    pass
+def show_help_callback(ctx: click.Context, _: click.Parameter, value: bool) -> None:
+    if value:
+        command_args = ["manage.py", ctx.info_name, "--help"]
+        django.core.management.execute_from_command_line(command_args)
 
 
-def _add_django_command(command_item: _CommandItem) -> None:
+def _add_django_command(
+    django_command: click.Group, command_item: _CommandItem
+) -> None:
     @django_command.command(
         name=command_item.name,
         help=command_item.description,
         context_settings={"ignore_unknown_options": True, "allow_extra_args": True},
         add_help_option=False,
     )
     @click.option(
         "-h",
         "--help",
+        callback=show_help_callback,
         help="Show the command help.",
         is_flag=True,
         expose_value=False,
         is_eager=True,
     )
     @click.pass_context
     def command(
         ctx: click.Context, *args: t.Tuple[t.Any, ...], **kwargs: t.Dict[str, t.Any]
     ) -> None:
         command_args = ["manage.py", command_item.name] + list(ctx.args)
         django.core.management.execute_from_command_line(command_args)
 
 
-list(map(_add_django_command, _django_support_commands))
+def get_django_command(blacklisted_commands: t.Set[str]) -> click.Group:
+    @click.group(
+        name="django",
+        help="Ellar Django Commands",
+    )
+    @click.option(
+        "-v",
+        "--version",
+        callback=version_callback,
+        help="Show the version and exit.",
+        is_flag=True,
+        expose_value=False,
+        is_eager=True,
+    )
+    @click.pass_context
+    def django_command(ctx: click.Context) -> None:
+        pass
+
+    for command_item in _generate_command_list(blacklisted_commands):
+        _add_django_command(
+            django_command=t.cast(click.Group, django_command),
+            command_item=command_item,
+        )
+
+    return t.cast(click.Group, django_command)
```

### Comparing `ellar_django_module-1.0.6/ellar_django/middleware.py` & `ellar_django_module-1.0.7/ellar_django/middleware.py`

 * *Files identical despite different names*

### Comparing `ellar_django_module-1.0.6/pyproject.toml` & `ellar_django_module-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     "Framework :: Django :: 4.2",
     "Framework :: AsyncIO",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
 
 dependencies = [
-    "ellar-cli >= 0.3.7",
+    "ellar-cli >= 0.4.1",
     "Django >= 3.1",
 ]
 
 
 [project.urls]
 Documentation = "https://github.com/python-ellar/ellar-django-module"
 Source = "https://github.com/python-ellar/ellar-django-module"
```

### Comparing `ellar_django_module-1.0.6/PKG-INFO` & `ellar_django_module-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ellar-django-module
-Version: 1.0.6
+Version: 1.0.7
 Summary: Enables Django ORM and Admin feature in Ellar's application
 Author-email: Ezeudoh Tochukwu <tochukwu.ezeudoh@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
@@ -29,15 +29,15 @@
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: AsyncIO
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP
-Requires-Dist: ellar-cli >= 0.3.7
+Requires-Dist: ellar-cli >= 0.4.1
 Requires-Dist: Django >= 3.1
 Project-URL: Documentation, https://github.com/python-ellar/ellar-django-module
 Project-URL: Homepage, https://python-ellar.github.io/ellar-django-module/
 Project-URL: Source, https://github.com/python-ellar/ellar-django-module
 
 <p align="center">
   <a href="#" target="blank"><img src="https://python-ellar.github.io/ellar/img/EllarLogoB.png" width="200" alt="Ellar Logo" /></a>
```

