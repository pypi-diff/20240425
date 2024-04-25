# Comparing `tmp/ellar_cli-0.4.0.tar.gz` & `tmp/ellar_cli-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ellar_cli-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ellar_cli-0.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ellar_cli-0.4.0.tar` & `ellar_cli-0.4.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     2113 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/README.md
--rw-r--r--   0        0        0      116 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/__init__.py
--rw-r--r--   0        0        0       94 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/__main__.py
--rw-r--r--   0        0        0      367 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/cli.py
--rw-r--r--   0        0        0     4302 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/click/__init__.py
--rw-r--r--   0        0        0     2459 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/click/argument.py
--rw-r--r--   0        0        0     1367 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/click/command.py
--rw-r--r--   0        0        0     3932 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/click/group.py
--rw-r--r--   0        0        0      821 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/click/util.py
--rw-r--r--   0        0        0       89 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/constants.py
--rw-r--r--   0        0        0     4750 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/file_scaffolding.py
--rw-r--r--   0        0        0     2159 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/main.py
--rw-r--r--   0        0        0      221 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/manage_commands/__init__.py
--rw-r--r--   0        0        0     3280 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/manage_commands/create_module.py
--rw-r--r--   0        0        0     5213 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/manage_commands/create_project.py
--rw-r--r--   0        0        0     6257 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/manage_commands/new.py
--rw-r--r--   0        0        0    12498 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/manage_commands/runserver.py
--rw-r--r--   0        0        0        0 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/py.typed
--rw-r--r--   0        0        0        0 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/scaffolding/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/scaffolding/module_template/module_name/__init__.ellar
--rw-r--r--   0        0        0      474 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/scaffolding/module_template/module_name/controllers.ellar
--rw-r--r--   0        0        0     1049 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/scaffolding/module_template/module_name/module.ellar
--rw-r--r--   0        0        0      255 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/scaffolding/module_template/module_name/routers.ellar
--rw-r--r--   0        0        0      155 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/scaffolding/module_template/module_name/schemas.ellar
--rw-r--r--   0        0        0      180 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/scaffolding/module_template/module_name/services.ellar
--rw-r--r--   0        0        0        0 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/scaffolding/module_template/module_name/tests/__init__.ellar
--rw-r--r--   0        0        0        0 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/scaffolding/module_template/module_name/tests/test_controllers.ellar
--rw-r--r--   0        0        0        0 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/scaffolding/module_template/module_name/tests/test_routers.ellar
--rw-r--r--   0        0        0        0 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/scaffolding/module_template/module_name/tests/test_services.ellar
--rw-r--r--   0        0        0      663 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/scaffolding/module_template/setup.json
--rw-r--r--   0        0        0      202 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/scaffolding/new_manage_template/folder_name/README.md
--rw-r--r--   0        0        0      412 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/scaffolding/new_manage_template/folder_name/manage.ellar
--rw-r--r--   0        0        0       43 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/scaffolding/new_manage_template/folder_name/tests/conftest.ellar
--rw-r--r--   0        0        0      449 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/scaffolding/new_manage_template/setup.json
--rw-r--r--   0        0        0      204 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/scaffolding/new_template/folder_name/README.md
--rw-r--r--   0        0        0        0 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/scaffolding/new_template/folder_name/pyproject.toml
--rw-r--r--   0        0        0       43 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/scaffolding/new_template/folder_name/tests/conftest.ellar
--rw-r--r--   0        0        0      451 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/scaffolding/new_template/setup.json
--rw-r--r--   0        0        0        0 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/scaffolding/project_template/project_name/__init__.ellar
--rw-r--r--   0        0        0     2580 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/scaffolding/project_template/project_name/config.ellar
--rw-r--r--   0        0        0        0 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/scaffolding/project_template/project_name/core/__init__.ellar
--rw-r--r--   0        0        0        0 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/scaffolding/project_template/project_name/domain/__init__.ellar
--rw-r--r--   0        0        0      438 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/scaffolding/project_template/project_name/root_module.ellar
--rw-r--r--   0        0        0     1268 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/scaffolding/project_template/project_name/server.ellar
--rw-r--r--   0        0        0      766 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/scaffolding/project_template/setup.json
--rw-r--r--   0        0        0     2028 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/scaffolding/scaffolding_json_validator.py
--rw-r--r--   0        0        0     1450 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/schema.py
--rw-r--r--   0        0        0      264 2024-03-27 19:16:47.986008 ellar_cli-0.4.0/ellar_cli/service/__init__.py
--rw-r--r--   0        0        0    10945 2024-03-27 19:16:47.990008 ellar_cli-0.4.0/ellar_cli/service/cli.py
--rw-r--r--   0        0        0       71 2024-03-27 19:16:47.990008 ellar_cli-0.4.0/ellar_cli/service/exceptions.py
--rw-r--r--   0        0        0     1837 2024-03-27 19:16:47.990008 ellar_cli-0.4.0/ellar_cli/service/pyproject.py
--rw-r--r--   0        0        0      707 2024-03-27 19:16:47.990008 ellar_cli-0.4.0/ellar_cli/testing.py
--rw-r--r--   0        0        0     3202 2024-03-27 19:16:47.990008 ellar_cli-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3789 1970-01-01 00:00:00.000000 ellar_cli-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2113 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/README.md
+-rw-r--r--   0        0        0      116 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/__init__.py
+-rw-r--r--   0        0        0       94 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/__main__.py
+-rw-r--r--   0        0        0      367 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/cli.py
+-rw-r--r--   0        0        0     4302 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/click/__init__.py
+-rw-r--r--   0        0        0     2459 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/click/argument.py
+-rw-r--r--   0        0        0     1367 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/click/command.py
+-rw-r--r--   0        0        0     3932 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/click/group.py
+-rw-r--r--   0        0        0      821 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/click/util.py
+-rw-r--r--   0        0        0       89 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/constants.py
+-rw-r--r--   0        0        0     4750 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/file_scaffolding.py
+-rw-r--r--   0        0        0     2159 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/main.py
+-rw-r--r--   0        0        0      221 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/manage_commands/__init__.py
+-rw-r--r--   0        0        0     3280 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/manage_commands/create_module.py
+-rw-r--r--   0        0        0     5213 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/manage_commands/create_project.py
+-rw-r--r--   0        0        0     6257 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/manage_commands/new.py
+-rw-r--r--   0        0        0    12498 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/manage_commands/runserver.py
+-rw-r--r--   0        0        0        0 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/py.typed
+-rw-r--r--   0        0        0        0 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/scaffolding/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/scaffolding/module_template/module_name/__init__.ellar
+-rw-r--r--   0        0        0      474 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/scaffolding/module_template/module_name/controllers.ellar
+-rw-r--r--   0        0        0     1049 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/scaffolding/module_template/module_name/module.ellar
+-rw-r--r--   0        0        0      255 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/scaffolding/module_template/module_name/routers.ellar
+-rw-r--r--   0        0        0      155 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/scaffolding/module_template/module_name/schemas.ellar
+-rw-r--r--   0        0        0      180 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/scaffolding/module_template/module_name/services.ellar
+-rw-r--r--   0        0        0        0 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/scaffolding/module_template/module_name/tests/__init__.ellar
+-rw-r--r--   0        0        0        0 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/scaffolding/module_template/module_name/tests/test_controllers.ellar
+-rw-r--r--   0        0        0        0 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/scaffolding/module_template/module_name/tests/test_routers.ellar
+-rw-r--r--   0        0        0        0 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/scaffolding/module_template/module_name/tests/test_services.ellar
+-rw-r--r--   0        0        0      663 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/scaffolding/module_template/setup.json
+-rw-r--r--   0        0        0      202 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/scaffolding/new_manage_template/folder_name/README.md
+-rw-r--r--   0        0        0      412 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/scaffolding/new_manage_template/folder_name/manage.ellar
+-rw-r--r--   0        0        0       43 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/scaffolding/new_manage_template/folder_name/tests/conftest.ellar
+-rw-r--r--   0        0        0      449 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/scaffolding/new_manage_template/setup.json
+-rw-r--r--   0        0        0      204 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/scaffolding/new_template/folder_name/README.md
+-rw-r--r--   0        0        0        0 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/scaffolding/new_template/folder_name/pyproject.toml
+-rw-r--r--   0        0        0       43 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/scaffolding/new_template/folder_name/tests/conftest.ellar
+-rw-r--r--   0        0        0      451 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/scaffolding/new_template/setup.json
+-rw-r--r--   0        0        0        0 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/scaffolding/project_template/project_name/__init__.ellar
+-rw-r--r--   0        0        0     2580 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/scaffolding/project_template/project_name/config.ellar
+-rw-r--r--   0        0        0        0 2024-04-25 08:42:00.905336 ellar_cli-0.4.1/ellar_cli/scaffolding/project_template/project_name/core/__init__.ellar
+-rw-r--r--   0        0        0        0 2024-04-25 08:42:00.909336 ellar_cli-0.4.1/ellar_cli/scaffolding/project_template/project_name/domain/__init__.ellar
+-rw-r--r--   0        0        0      438 2024-04-25 08:42:00.909336 ellar_cli-0.4.1/ellar_cli/scaffolding/project_template/project_name/root_module.ellar
+-rw-r--r--   0        0        0     1268 2024-04-25 08:42:00.909336 ellar_cli-0.4.1/ellar_cli/scaffolding/project_template/project_name/server.ellar
+-rw-r--r--   0        0        0      766 2024-04-25 08:42:00.909336 ellar_cli-0.4.1/ellar_cli/scaffolding/project_template/setup.json
+-rw-r--r--   0        0        0     2028 2024-04-25 08:42:00.909336 ellar_cli-0.4.1/ellar_cli/scaffolding/scaffolding_json_validator.py
+-rw-r--r--   0        0        0     1450 2024-04-25 08:42:00.909336 ellar_cli-0.4.1/ellar_cli/schema.py
+-rw-r--r--   0        0        0      264 2024-04-25 08:42:00.909336 ellar_cli-0.4.1/ellar_cli/service/__init__.py
+-rw-r--r--   0        0        0    10945 2024-04-25 08:42:00.909336 ellar_cli-0.4.1/ellar_cli/service/cli.py
+-rw-r--r--   0        0        0       71 2024-04-25 08:42:00.909336 ellar_cli-0.4.1/ellar_cli/service/exceptions.py
+-rw-r--r--   0        0        0     1837 2024-04-25 08:42:00.909336 ellar_cli-0.4.1/ellar_cli/service/pyproject.py
+-rw-r--r--   0        0        0      707 2024-04-25 08:42:00.909336 ellar_cli-0.4.1/ellar_cli/testing.py
+-rw-r--r--   0        0        0     3202 2024-04-25 08:42:00.909336 ellar_cli-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3789 1970-01-01 00:00:00.000000 ellar_cli-0.4.1/PKG-INFO
```

### Comparing `ellar_cli-0.4.0/README.md` & `ellar_cli-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `ellar_cli-0.4.0/ellar_cli/click/__init__.py` & `ellar_cli-0.4.1/ellar_cli/click/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar_cli-0.4.0/ellar_cli/click/argument.py` & `ellar_cli-0.4.1/ellar_cli/click/argument.py`

 * *Files identical despite different names*

### Comparing `ellar_cli-0.4.0/ellar_cli/click/command.py` & `ellar_cli-0.4.1/ellar_cli/click/command.py`

 * *Files identical despite different names*

### Comparing `ellar_cli-0.4.0/ellar_cli/click/group.py` & `ellar_cli-0.4.1/ellar_cli/click/group.py`

 * *Files identical despite different names*

### Comparing `ellar_cli-0.4.0/ellar_cli/click/util.py` & `ellar_cli-0.4.1/ellar_cli/click/util.py`

 * *Files identical despite different names*

### Comparing `ellar_cli-0.4.0/ellar_cli/file_scaffolding.py` & `ellar_cli-0.4.1/ellar_cli/file_scaffolding.py`

 * *Files identical despite different names*

### Comparing `ellar_cli-0.4.0/ellar_cli/main.py` & `ellar_cli-0.4.1/ellar_cli/main.py`

 * *Files identical despite different names*

### Comparing `ellar_cli-0.4.0/ellar_cli/manage_commands/create_module.py` & `ellar_cli-0.4.1/ellar_cli/manage_commands/create_module.py`

 * *Files identical despite different names*

### Comparing `ellar_cli-0.4.0/ellar_cli/manage_commands/create_project.py` & `ellar_cli-0.4.1/ellar_cli/manage_commands/create_project.py`

 * *Files identical despite different names*

### Comparing `ellar_cli-0.4.0/ellar_cli/manage_commands/new.py` & `ellar_cli-0.4.1/ellar_cli/manage_commands/new.py`

 * *Files identical despite different names*

### Comparing `ellar_cli-0.4.0/ellar_cli/manage_commands/runserver.py` & `ellar_cli-0.4.1/ellar_cli/manage_commands/runserver.py`

 * *Files identical despite different names*

### Comparing `ellar_cli-0.4.0/ellar_cli/scaffolding/module_template/module_name/module.ellar` & `ellar_cli-0.4.1/ellar_cli/scaffolding/module_template/module_name/module.ellar`

 * *Files identical despite different names*

### Comparing `ellar_cli-0.4.0/ellar_cli/scaffolding/module_template/setup.json` & `ellar_cli-0.4.1/ellar_cli/scaffolding/module_template/setup.json`

 * *Files identical despite different names*

### Comparing `ellar_cli-0.4.0/ellar_cli/scaffolding/project_template/project_name/config.ellar` & `ellar_cli-0.4.1/ellar_cli/scaffolding/project_template/project_name/config.ellar`

 * *Files identical despite different names*

### Comparing `ellar_cli-0.4.0/ellar_cli/scaffolding/project_template/project_name/server.ellar` & `ellar_cli-0.4.1/ellar_cli/scaffolding/project_template/project_name/server.ellar`

 * *Files identical despite different names*

### Comparing `ellar_cli-0.4.0/ellar_cli/scaffolding/project_template/setup.json` & `ellar_cli-0.4.1/ellar_cli/scaffolding/project_template/setup.json`

 * *Files identical despite different names*

### Comparing `ellar_cli-0.4.0/ellar_cli/scaffolding/scaffolding_json_validator.py` & `ellar_cli-0.4.1/ellar_cli/scaffolding/scaffolding_json_validator.py`

 * *Files identical despite different names*

### Comparing `ellar_cli-0.4.0/ellar_cli/schema.py` & `ellar_cli-0.4.1/ellar_cli/schema.py`

 * *Files identical despite different names*

### Comparing `ellar_cli-0.4.0/ellar_cli/service/cli.py` & `ellar_cli-0.4.1/ellar_cli/service/cli.py`

 * *Files identical despite different names*

### Comparing `ellar_cli-0.4.0/ellar_cli/service/pyproject.py` & `ellar_cli-0.4.1/ellar_cli/service/pyproject.py`

 * *Files identical despite different names*

### Comparing `ellar_cli-0.4.0/ellar_cli/testing.py` & `ellar_cli-0.4.1/ellar_cli/testing.py`

 * *Files identical despite different names*

### Comparing `ellar_cli-0.4.0/pyproject.toml` & `ellar_cli-0.4.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -38,16 +38,16 @@
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
 
 dependencies = [
     # exclude 0.11.2 and 0.11.3 due to https://github.com/sdispater/tomlkit/issues/225
     "tomlkit >=0.11.1,<1.0.0,!=0.11.2,!=0.11.3",
-    "uvicorn[standard] == 0.27.1",
-    "ellar >= 0.7.1",
+    "uvicorn[standard] == 0.29.0",
+    "ellar >= 0.7.4",
     "click >= 8.1.7",
 ]
 
 [project.scripts]
 ellar = "ellar_cli.cli:main"
 
 [project.urls]
```

### Comparing `ellar_cli-0.4.0/PKG-INFO` & `ellar_cli-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ellar-cli
-Version: 0.4.0
+Version: 0.4.1
 Summary: Ellar CLI Tool for Scaffolding Ellar Projects, Modules and also running Ellar Commands
 Author-email: Ezeudoh Tochukwu <tochukwu.ezeudoh@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
@@ -23,16 +23,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Framework :: AsyncIO
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Dist: tomlkit >=0.11.1,<1.0.0,!=0.11.2,!=0.11.3
-Requires-Dist: uvicorn[standard] == 0.27.1
-Requires-Dist: ellar >= 0.7.1
+Requires-Dist: uvicorn[standard] == 0.29.0
+Requires-Dist: ellar >= 0.7.4
 Requires-Dist: click >= 8.1.7
 Project-URL: Documentation, https://github.com/python-ellar/ellar-cli
 Project-URL: Homepage, https://python-ellar.github.io/ellar-cli/
 Project-URL: Source, https://github.com/python-ellar/ellar-cli
 
 <p align="center">
   <a href="#" target="blank"><img src="https://python-ellar.github.io/ellar/img/EllarLogoB.png" width="200" alt="Ellar Logo" /></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ellar-cli Version: 0.4.0 Summary: Ellar CLI Tool
+Metadata-Version: 2.1 Name: ellar-cli Version: 0.4.1 Summary: Ellar CLI Tool
 for Scaffolding Ellar Projects, Modules and also running Ellar Commands Author-
 email: Ezeudoh Tochukwu
 gmail.com> Requires-Python: >=3.8 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology Classifier: Intended
 Audience :: System Administrators Classifier: Operating System :: OS
 Independent Classifier: Topic :: Internet Classifier: Topic :: Software
 Development :: Libraries :: Application Frameworks Classifier: Topic ::
@@ -13,15 +13,15 @@
 :: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3 :: Only Classifier: Framework :: AsyncIO Classifier: Topic ::
 Internet :: WWW/HTTP :: HTTP Servers Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Dist: tomlkit >=0.11.1,<1.0.0,!=0.11.2,!=0.11.3 Requires-Dist: uvicorn
-[standard] == 0.27.1 Requires-Dist: ellar >= 0.7.1 Requires-Dist: click >=
+[standard] == 0.29.0 Requires-Dist: ellar >= 0.7.4 Requires-Dist: click >=
 8.1.7 Project-URL: Documentation, https://github.com/python-ellar/ellar-cli
 Project-URL: Homepage, https://python-ellar.github.io/ellar-cli/ Project-URL:
 Source, https://github.com/python-ellar/ellar-cli
                                  _[_E_l_l_a_r_ _L_o_g_o_]
   Ellar CLI Tool for Scaffolding Ellar Projects and Modules and also running
                                 Ellar Commands
 ![Test](https://github.com/python-ellar/ellar-cli/actions/workflows/
```

