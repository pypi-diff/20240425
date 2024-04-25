# Comparing `tmp/ecs_session-24.4.7.tar.gz` & `tmp/ecs_session-24.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecs_session-24.4.7.tar", max compression
+gzip compressed data, was "ecs_session-24.4.8.tar", max compression
```

## Comparing `ecs_session-24.4.7.tar` & `ecs_session-24.4.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1428 2024-04-23 08:14:37.442380 ecs_session-24.4.7/README.md
--rw-r--r--   0        0        0     3859 2024-04-23 12:01:42.084232 ecs_session-24.4.7/ecs_session/__init__.py
--rw-r--r--   0        0        0     7038 2024-04-25 13:00:17.901007 ecs_session-24.4.7/ecs_session/cli.py
--rw-r--r--   0        0        0      640 2024-04-25 13:00:05.940577 ecs_session-24.4.7/pyproject.toml
--rw-r--r--   0        0        0     2255 1970-01-01 00:00:00.000000 ecs_session-24.4.7/setup.py
--rw-r--r--   0        0        0     2448 1970-01-01 00:00:00.000000 ecs_session-24.4.7/PKG-INFO
+-rw-r--r--   0        0        0     1428 2024-04-23 08:14:37.442380 ecs_session-24.4.8/README.md
+-rw-r--r--   0        0        0     3859 2024-04-23 12:01:42.084232 ecs_session-24.4.8/ecs_session/__init__.py
+-rw-r--r--   0        0        0     7116 2024-04-25 13:14:21.010256 ecs_session-24.4.8/ecs_session/cli.py
+-rw-r--r--   0        0        0      640 2024-04-25 13:14:32.910891 ecs_session-24.4.8/pyproject.toml
+-rw-r--r--   0        0        0     2255 1970-01-01 00:00:00.000000 ecs_session-24.4.8/setup.py
+-rw-r--r--   0        0        0     2448 1970-01-01 00:00:00.000000 ecs_session-24.4.8/PKG-INFO
```

### Comparing `ecs_session-24.4.7/README.md` & `ecs_session-24.4.8/README.md`

 * *Files identical despite different names*

### Comparing `ecs_session-24.4.7/ecs_session/__init__.py` & `ecs_session-24.4.8/ecs_session/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_session-24.4.7/ecs_session/cli.py` & `ecs_session-24.4.8/ecs_session/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,27 +66,29 @@
     )
     subparsers.required = True
     subparsers.add_parser("forward", help="Portforwarding")
     subparsers.add_parser("command", help="Execute command")
     return parser
 
 
-def show_menu(items: list, title: str, source: list = None):
+def show_menu(items: list, title: str, source: list = None, back: bool = True):
     """
     menu function
     """
     index = None
     source = source or items
+    if back:
+        items = items + ["Back"]
     menu = TerminalMenu(
-        items + ["Back"],
+        items,
         title=f'? {title} (Press "q"/"ESC" to quit):\n',
         show_search_hint=True,
     )
     index = menu.show()
-    if index == len(items):
+    if index == len(items) - 1:
         return None, index
     if index is None:
         exit(0)
     return source[index], index
 
 
 def ecs_paginator(ecs: session.Session.client, paginator: str, leaf: str, **kwargs):
@@ -112,14 +114,15 @@
         paginator="list_clusters",
         leaf="clusterArns",
     )
     clusters = [cluster.split("/")[-1] for cluster in arns]
     return show_menu(
         items=clusters,
         title="Select cluster",
+        back=False,
     )
 
 
 def get_service(ecs: session.Session.client, service: str, cluster: str):
     """
     get service
     """
```

### Comparing `ecs_session-24.4.7/pyproject.toml` & `ecs_session-24.4.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ecs-session"
-version = "24.4.7"
+version = "24.4.8"
 description = "ECS SSM tool"
 authors = ["Stefan Heitmüller <stefan.heitmueller@gmx.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/morph027/ecs-session"
 
 [tool.poetry.dependencies]
```

### Comparing `ecs_session-24.4.7/setup.py` & `ecs_session-24.4.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['boto3', 'configargparse', 'shtab', 'simple_term_menu']
 
 entry_points = \
 {'console_scripts': ['ecs-session = ecs_session.cli:run']}
 
 setup_kwargs = {
     'name': 'ecs-session',
-    'version': '24.4.7',
+    'version': '24.4.8',
     'description': 'ECS SSM tool',
     'long_description': '# ecs-session\n\nInspired by [ecsgo](https://github.com/tedsmitt/ecsgo) (`ecspy` is in use already).\n\nProvides a tool to interact with AWS ECS tasks.\n\nCurrently provides:\n\n* interactive execute-command (e.g. shell)\n* port-forwarding\n\nYou can supply command-line arguments to specify which cluster/service/task/... to use or will be prompted with a nice menu.\n\n## Installation\n\n```\npip install ecs-session\n```\n\n## Pre-requisites\n\n### [session-manager-plugin](https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager-working-with-install-plugin.html)\n\n#### Linux\n\n```bash\ncurl https://s3.amazonaws.com/session-manager-downloads/plugin/latest/ubuntu_64bit/session-manager-plugin.deb -o "/tmp/session-manager-plugin.deb"\nmkdir -p ~/bin\ndpkg-deb --fsys-tarfile /tmp/session-manager-plugin.deb | tar --strip-components=4 -C ~/bin/ -xvf - usr/local/sessionmanagerplugin/bin/session-manager-plugin\n```\n\n#### MacOS\n\n`brew install --cask session-manager-plugin`\n\n### Infrastructure\n\nUse [ecs-exec-checker](https://github.com/aws-containers/amazon-ecs-exec-checker) to check for the pre-requisites to use ECS exec.\n\n\n## Usage\n\nSee `ecs-session --help` for all features.\n\n### Execute command\n\nSelect all from menu:\n\n```bash\necs-session command\n```\n\n### Port forwarding\n\nSelect all from menu:\n\n```bash\necs-session forward\n```\n\nSpecify port and select the rest from menu:\n\n```bash\necs-session --remote-port 8080 forward\n```\n',
     'author': 'Stefan Heitmüller',
     'author_email': 'stefan.heitmueller@gmx.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/morph027/ecs-session',
```

### Comparing `ecs_session-24.4.7/PKG-INFO` & `ecs_session-24.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecs-session
-Version: 24.4.7
+Version: 24.4.8
 Summary: ECS SSM tool
 Home-page: https://github.com/morph027/ecs-session
 License: MIT
 Author: Stefan Heitmüller
 Author-email: stefan.heitmueller@gmx.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
```

