# Comparing `tmp/ecs_session-24.4.8.tar.gz` & `tmp/ecs_session-24.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecs_session-24.4.8.tar", max compression
+gzip compressed data, was "ecs_session-24.4.9.tar", max compression
```

## Comparing `ecs_session-24.4.8.tar` & `ecs_session-24.4.9.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1428 2024-04-23 08:14:37.442380 ecs_session-24.4.8/README.md
--rw-r--r--   0        0        0     3859 2024-04-23 12:01:42.084232 ecs_session-24.4.8/ecs_session/__init__.py
--rw-r--r--   0        0        0     7116 2024-04-25 13:14:21.010256 ecs_session-24.4.8/ecs_session/cli.py
--rw-r--r--   0        0        0      640 2024-04-25 13:14:32.910891 ecs_session-24.4.8/pyproject.toml
--rw-r--r--   0        0        0     2255 1970-01-01 00:00:00.000000 ecs_session-24.4.8/setup.py
--rw-r--r--   0        0        0     2448 1970-01-01 00:00:00.000000 ecs_session-24.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1428 2024-04-25 16:11:25.530756 ecs_session-24.4.9/README.md
+-rw-r--r--   0        0        0     3859 2024-04-25 16:11:25.530756 ecs_session-24.4.9/ecs_session/__init__.py
+-rw-r--r--   0        0        0     7115 2024-04-25 16:13:56.803693 ecs_session-24.4.9/ecs_session/cli.py
+-rw-r--r--   0        0        0      640 2024-04-25 16:14:03.460814 ecs_session-24.4.9/pyproject.toml
+-rw-r--r--   0        0        0     2499 1970-01-01 00:00:00.000000 ecs_session-24.4.9/PKG-INFO
```

### Comparing `ecs_session-24.4.8/README.md` & `ecs_session-24.4.9/README.md`

 * *Files identical despite different names*

### Comparing `ecs_session-24.4.8/ecs_session/__init__.py` & `ecs_session-24.4.9/ecs_session/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_session-24.4.8/ecs_session/cli.py` & `ecs_session-24.4.9/ecs_session/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         items = items + ["Back"]
     menu = TerminalMenu(
         items,
         title=f'? {title} (Press "q"/"ESC" to quit):\n',
         show_search_hint=True,
     )
     index = menu.show()
-    if index == len(items) - 1:
+    if items[index] == "Back":
         return None, index
     if index is None:
         exit(0)
     return source[index], index
 
 
 def ecs_paginator(ecs: session.Session.client, paginator: str, leaf: str, **kwargs):
```

### Comparing `ecs_session-24.4.8/pyproject.toml` & `ecs_session-24.4.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ecs-session"
-version = "24.4.8"
+version = "24.4.9"
 description = "ECS SSM tool"
 authors = ["Stefan Heitmüller <stefan.heitmueller@gmx.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/morph027/ecs-session"
 
 [tool.poetry.dependencies]
```

### Comparing `ecs_session-24.4.8/PKG-INFO` & `ecs_session-24.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecs-session
-Version: 24.4.8
+Version: 24.4.9
 Summary: ECS SSM tool
 Home-page: https://github.com/morph027/ecs-session
 License: MIT
 Author: Stefan Heitmüller
 Author-email: stefan.heitmueller@gmx.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: boto3
 Requires-Dist: configargparse
 Requires-Dist: shtab
 Requires-Dist: simple_term_menu
 Project-URL: Repository, https://github.com/morph027/ecs-session
 Description-Content-Type: text/markdown
```

