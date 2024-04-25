# Comparing `tmp/nullscream-0.1.1.tar.gz` & `tmp/nullscream-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nullscream-0.1.1.tar", last modified: Thu Apr 25 17:38:51 2024, max compression
+gzip compressed data, was "nullscream-0.1.3.tar", last modified: Thu Apr 25 17:45:18 2024, max compression
```

## Comparing `nullscream-0.1.1.tar` & `nullscream-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:51.891032 nullscream-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-25 17:38:47.000000 nullscream-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-25 17:38:51.891032 nullscream-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-25 17:38:47.000000 nullscream-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 17:38:51.891032 nullscream-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-25 17:38:47.000000 nullscream-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:51.891032 nullscream-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:51.891032 nullscream-0.1.1/src/nullscream/
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-25 17:38:47.000000 nullscream-0.1.1/src/nullscream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-25 17:38:47.000000 nullscream-0.1.1/src/nullscream/noop_class.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-25 17:38:47.000000 nullscream-0.1.1/src/nullscream/noop_function.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:51.891032 nullscream-0.1.1/src/nullscream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-25 17:38:51.000000 nullscream-0.1.1/src/nullscream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-25 17:38:51.000000 nullscream-0.1.1/src/nullscream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 17:38:51.000000 nullscream-0.1.1/src/nullscream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-25 17:38:51.000000 nullscream-0.1.1/src/nullscream.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:51.891032 nullscream-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-25 17:38:47.000000 nullscream-0.1.1/tests/test_blacklist.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-25 17:38:47.000000 nullscream-0.1.1/tests/test_whitelist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:45:18.420873 nullscream-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-25 17:45:14.000000 nullscream-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-25 17:45:18.420873 nullscream-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-25 17:45:14.000000 nullscream-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 17:45:18.420873 nullscream-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-25 17:45:14.000000 nullscream-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:45:18.416874 nullscream-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:45:18.420873 nullscream-0.1.3/src/nullscream/
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-25 17:45:14.000000 nullscream-0.1.3/src/nullscream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-25 17:45:14.000000 nullscream-0.1.3/src/nullscream/noop_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-25 17:45:14.000000 nullscream-0.1.3/src/nullscream/noop_function.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:45:18.420873 nullscream-0.1.3/src/nullscream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-25 17:45:18.000000 nullscream-0.1.3/src/nullscream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-25 17:45:18.000000 nullscream-0.1.3/src/nullscream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 17:45:18.000000 nullscream-0.1.3/src/nullscream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-25 17:45:18.000000 nullscream-0.1.3/src/nullscream.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:45:18.420873 nullscream-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-25 17:45:14.000000 nullscream-0.1.3/tests/test_blacklist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-25 17:45:14.000000 nullscream-0.1.3/tests/test_whitelist.py
```

### Comparing `nullscream-0.1.1/LICENSE` & `nullscream-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nullscream-0.1.1/PKG-INFO` & `nullscream-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nullscream
-Version: 0.1.1
+Version: 0.1.3
 Home-page: https://github.com/Capsize-Games/nullscream
 Author: Capsize LLC
 Author-email: contact@capsizegames.com
 License: GPL-3.0
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `nullscream-0.1.1/README.md` & `nullscream-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nullscream-0.1.1/setup.py` & `nullscream-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="nullscream",
-    version="0.1.1",
+    version="0.1.3",
     author="Capsize LLC",
     description="",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="",
     license="GPL-3.0",
     author_email="contact@capsizegames.com",
```

### Comparing `nullscream-0.1.1/src/nullscream/__init__.py` & `nullscream-0.1.3/src/nullscream/__init__.py`

 * *Files identical despite different names*

### Comparing `nullscream-0.1.1/src/nullscream/noop_class.py` & `nullscream-0.1.3/src/nullscream/noop_class.py`

 * *Files identical despite different names*

### Comparing `nullscream-0.1.1/src/nullscream.egg-info/PKG-INFO` & `nullscream-0.1.3/src/nullscream.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nullscream
-Version: 0.1.1
+Version: 0.1.3
 Home-page: https://github.com/Capsize-Games/nullscream
 Author: Capsize LLC
 Author-email: contact@capsizegames.com
 License: GPL-3.0
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `nullscream-0.1.1/tests/test_whitelist.py` & `nullscream-0.1.3/tests/test_whitelist.py`

 * *Files identical despite different names*

