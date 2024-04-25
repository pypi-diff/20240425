# Comparing `tmp/ontopint-0.0.2.tar.gz` & `tmp/ontopint-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ontopint-0.0.2.tar", last modified: Wed Apr 24 12:56:02 2024, max compression
+gzip compressed data, was "ontopint-0.0.3.tar", last modified: Wed Apr 24 13:07:54 2024, max compression
```

## Comparing `ontopint-0.0.2.tar` & `ontopint-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 hampusnasstrom  (1000) hampusnasstrom  (1000)        0 2024-04-24 12:56:02.056816 ontopint-0.0.2/
--rw-r--r--   0 hampusnasstrom  (1000) hampusnasstrom  (1000)     3089 2024-04-24 12:34:58.000000 ontopint-0.0.2/.gitignore
--rw-r--r--   0 hampusnasstrom  (1000) hampusnasstrom  (1000)     1074 2024-04-24 12:04:04.000000 ontopint-0.0.2/LICENSE
--rw-r--r--   0 hampusnasstrom  (1000) hampusnasstrom  (1000)     2188 2024-04-24 12:56:02.056816 ontopint-0.0.2/PKG-INFO
--rw-r--r--   0 hampusnasstrom  (1000) hampusnasstrom  (1000)       99 2024-04-24 12:04:04.000000 ontopint-0.0.2/README.md
--rw-r--r--   0 hampusnasstrom  (1000) hampusnasstrom  (1000)     2260 2024-04-24 12:17:19.000000 ontopint-0.0.2/pyproject.toml
--rw-r--r--   0 hampusnasstrom  (1000) hampusnasstrom  (1000)       38 2024-04-24 12:56:02.056816 ontopint-0.0.2/setup.cfg
-drwxr-xr-x   0 hampusnasstrom  (1000) hampusnasstrom  (1000)        0 2024-04-24 12:56:02.055816 ontopint-0.0.2/src/
-drwxr-xr-x   0 hampusnasstrom  (1000) hampusnasstrom  (1000)        0 2024-04-24 12:56:02.055816 ontopint-0.0.2/src/ontopint/
--rw-r--r--   0 hampusnasstrom  (1000) hampusnasstrom  (1000)     1116 2024-04-24 12:35:05.000000 ontopint-0.0.2/src/ontopint/__init__.py
-drwxr-xr-x   0 hampusnasstrom  (1000) hampusnasstrom  (1000)        0 2024-04-24 12:56:02.055816 ontopint-0.0.2/src/ontopint.egg-info/
--rw-r--r--   0 hampusnasstrom  (1000) hampusnasstrom  (1000)     2188 2024-04-24 12:56:02.000000 ontopint-0.0.2/src/ontopint.egg-info/PKG-INFO
--rw-r--r--   0 hampusnasstrom  (1000) hampusnasstrom  (1000)      247 2024-04-24 12:56:02.000000 ontopint-0.0.2/src/ontopint.egg-info/SOURCES.txt
--rw-r--r--   0 hampusnasstrom  (1000) hampusnasstrom  (1000)        1 2024-04-24 12:56:02.000000 ontopint-0.0.2/src/ontopint.egg-info/dependency_links.txt
--rw-r--r--   0 hampusnasstrom  (1000) hampusnasstrom  (1000)       26 2024-04-24 12:56:02.000000 ontopint-0.0.2/src/ontopint.egg-info/requires.txt
--rw-r--r--   0 hampusnasstrom  (1000) hampusnasstrom  (1000)        9 2024-04-24 12:56:02.000000 ontopint-0.0.2/src/ontopint.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:07:54.899689 ontopint-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:07:54.895689 ontopint-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:07:54.895689 ontopint-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-24 13:07:45.000000 ontopint-0.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-04-24 13:07:45.000000 ontopint-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-24 13:07:45.000000 ontopint-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-04-24 13:07:54.899689 ontopint-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-24 13:07:45.000000 ontopint-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-24 13:07:45.000000 ontopint-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 13:07:54.899689 ontopint-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:07:54.895689 ontopint-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:07:54.895689 ontopint-0.0.3/src/ontopint/
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-24 13:07:45.000000 ontopint-0.0.3/src/ontopint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:07:54.899689 ontopint-0.0.3/src/ontopint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-04-24 13:07:54.000000 ontopint-0.0.3/src/ontopint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-24 13:07:54.000000 ontopint-0.0.3/src/ontopint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:07:54.000000 ontopint-0.0.3/src/ontopint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-24 13:07:54.000000 ontopint-0.0.3/src/ontopint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 13:07:54.000000 ontopint-0.0.3/src/ontopint.egg-info/top_level.txt
```

### Comparing `ontopint-0.0.2/.gitignore` & `ontopint-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ontopint-0.0.2/LICENSE` & `ontopint-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ontopint-0.0.2/PKG-INFO` & `ontopint-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ontopint
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python package for reading units from a JSON-LD files and generating pint quantities.
 Author: Fabian Kirchner, Simon Stier
 Author-email: Hampus Näsström <hampus.naesstroem@physik.hu-berlin.de>
 Maintainer-email: Hampus Näsström <hampus.naesstroem@physik.hu-berlin.de>
 License: MIT License
         
         Copyright (c) 2024 Hampus Näsström
```

### Comparing `ontopint-0.0.2/pyproject.toml` & `ontopint-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ontopint-0.0.2/src/ontopint/__init__.py` & `ontopint-0.0.3/src/ontopint/__init__.py`

 * *Files identical despite different names*

### Comparing `ontopint-0.0.2/src/ontopint.egg-info/PKG-INFO` & `ontopint-0.0.3/src/ontopint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ontopint
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python package for reading units from a JSON-LD files and generating pint quantities.
 Author: Fabian Kirchner, Simon Stier
 Author-email: Hampus Näsström <hampus.naesstroem@physik.hu-berlin.de>
 Maintainer-email: Hampus Näsström <hampus.naesstroem@physik.hu-berlin.de>
 License: MIT License
         
         Copyright (c) 2024 Hampus Näsström
```

