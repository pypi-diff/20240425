# Comparing `tmp/transkribus_rest_api-0.2.0.tar.gz` & `tmp/transkribus_rest_api-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transkribus_rest_api-0.2.0.tar", last modified: Wed Mar 13 12:29:39 2024, max compression
+gzip compressed data, was "transkribus_rest_api-0.3.0.tar", last modified: Thu Apr 25 14:52:43 2024, max compression
```

## Comparing `transkribus_rest_api-0.2.0.tar` & `transkribus_rest_api-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:29:39.121487 transkribus_rest_api-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-13 12:29:17.000000 transkribus_rest_api-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-03-13 12:29:39.121487 transkribus_rest_api-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-13 12:29:17.000000 transkribus_rest_api-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-03-13 12:29:17.000000 transkribus_rest_api-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-13 12:29:17.000000 transkribus_rest_api-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 12:29:39.121487 transkribus_rest_api-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:29:39.121487 transkribus_rest_api-0.2.0/transkribus_rest_api/
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-03-13 12:29:17.000000 transkribus_rest_api-0.2.0/transkribus_rest_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-03-13 12:29:17.000000 transkribus_rest_api-0.2.0/transkribus_rest_api/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-03-13 12:29:17.000000 transkribus_rest_api-0.2.0/transkribus_rest_api/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-13 12:29:17.000000 transkribus_rest_api-0.2.0/transkribus_rest_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:29:39.121487 transkribus_rest_api-0.2.0/transkribus_rest_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-03-13 12:29:39.000000 transkribus_rest_api-0.2.0/transkribus_rest_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-03-13 12:29:39.000000 transkribus_rest_api-0.2.0/transkribus_rest_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 12:29:39.000000 transkribus_rest_api-0.2.0/transkribus_rest_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-13 12:29:39.000000 transkribus_rest_api-0.2.0/transkribus_rest_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-13 12:29:39.000000 transkribus_rest_api-0.2.0/transkribus_rest_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:52:43.769941 transkribus_rest_api-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-25 14:52:32.000000 transkribus_rest_api-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-25 14:52:43.769941 transkribus_rest_api-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-25 14:52:32.000000 transkribus_rest_api-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-25 14:52:32.000000 transkribus_rest_api-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-25 14:52:32.000000 transkribus_rest_api-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 14:52:43.769941 transkribus_rest_api-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:52:43.769941 transkribus_rest_api-0.3.0/transkribus_rest_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-25 14:52:32.000000 transkribus_rest_api-0.3.0/transkribus_rest_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-04-25 14:52:32.000000 transkribus_rest_api-0.3.0/transkribus_rest_api/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-25 14:52:32.000000 transkribus_rest_api-0.3.0/transkribus_rest_api/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-25 14:52:32.000000 transkribus_rest_api-0.3.0/transkribus_rest_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:52:43.769941 transkribus_rest_api-0.3.0/transkribus_rest_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-25 14:52:43.000000 transkribus_rest_api-0.3.0/transkribus_rest_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-25 14:52:43.000000 transkribus_rest_api-0.3.0/transkribus_rest_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 14:52:43.000000 transkribus_rest_api-0.3.0/transkribus_rest_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-25 14:52:43.000000 transkribus_rest_api-0.3.0/transkribus_rest_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-25 14:52:43.000000 transkribus_rest_api-0.3.0/transkribus_rest_api.egg-info/top_level.txt
```

### Comparing `transkribus_rest_api-0.2.0/LICENSE` & `transkribus_rest_api-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `transkribus_rest_api-0.2.0/PKG-INFO` & `transkribus_rest_api-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transkribus_rest_api
-Version: 0.2.0
+Version: 0.3.0
 Summary: Transkribus Metagrapho API Client.
 Author-email: "J. Nathanael Philipp" <nathanael@philipp.land>
 License: GPLv3+
 Project-URL: Homepage, https://github.com/jnphilipp/transkribus_rest_api
 Project-URL: Bug Tracker, http://github.com/jnphilipp/transkribus_rest_api/issues
 Keywords: transkribus,api
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `transkribus_rest_api-0.2.0/pyproject.toml` & `transkribus_rest_api-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "transkribus_rest_api"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
     {name = "J. Nathanael Philipp", email = "nathanael@philipp.land"}
 ]
 description="Transkribus Metagrapho API Client."
 readme = "README.md"
 license = {text = "GPLv3+"}
 requires-python = ">=3.10"
@@ -32,7 +32,10 @@
 [project.urls]
 "Homepage" = "https://github.com/jnphilipp/transkribus_rest_api"
 "Bug Tracker" = "http://github.com/jnphilipp/transkribus_rest_api/issues"
 
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
+
+[tool.setuptools.package-data]
+transkribus_rest_api = ["py.typed"]
```

### Comparing `transkribus_rest_api-0.2.0/transkribus_rest_api/__init__.py` & `transkribus_rest_api-0.3.0/transkribus_rest_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 __all__ = ["TranskribusRestApi", "transkribus_rest_api"]
 
 __app_name__ = "transkribus-rest-api"
 __author__ = "J. Nathanael Philipp"
 __email__ = "nathanael@philipp.land"
 __copyright__ = "Copyright 2024 J. Nathanael Philipp (jnphilipp)"
 __license__ = "GPLv3"
-__version_info__ = (0, 2, 0)
+__version_info__ = (0, 3, 0)
 __version__ = ".".join(str(e) for e in __version_info__)
 __github__ = "https://github.com/jnphilipp/transkribus-rest-api"
 VERSION = (
     f"%(prog)s v{__version__}\n{__copyright__}\n"
     + "License GPLv3+: GNU GPL version 3 or later <https://gnu.org/licenses/gpl.html>."
     + "\nThis is free software: you are free to change and redistribute it.\n"
     + "There is NO WARRANTY, to the extent permitted by law.\n\n"
```

### Comparing `transkribus_rest_api-0.2.0/transkribus_rest_api/types.py` & `transkribus_rest_api-0.3.0/transkribus_rest_api/types.py`

 * *Files identical despite different names*

### Comparing `transkribus_rest_api-0.2.0/transkribus_rest_api/utils.py` & `transkribus_rest_api-0.3.0/transkribus_rest_api/utils.py`

 * *Files identical despite different names*

### Comparing `transkribus_rest_api-0.2.0/transkribus_rest_api.egg-info/PKG-INFO` & `transkribus_rest_api-0.3.0/transkribus_rest_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transkribus_rest_api
-Version: 0.2.0
+Version: 0.3.0
 Summary: Transkribus Metagrapho API Client.
 Author-email: "J. Nathanael Philipp" <nathanael@philipp.land>
 License: GPLv3+
 Project-URL: Homepage, https://github.com/jnphilipp/transkribus_rest_api
 Project-URL: Bug Tracker, http://github.com/jnphilipp/transkribus_rest_api/issues
 Keywords: transkribus,api
 Classifier: Development Status :: 5 - Production/Stable
```

