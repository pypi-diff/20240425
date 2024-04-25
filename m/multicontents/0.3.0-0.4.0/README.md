# Comparing `tmp/multicontents-0.3.0.tar.gz` & `tmp/multicontents-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/multicontents-0.3.0.tar", last modified: Tue Feb 16 01:17:47 2021, max compression
+gzip compressed data, was "dist/multicontents-0.4.0.tar", last modified: Thu Apr 25 17:34:26 2024, max compression
```

## Comparing `multicontents-0.3.0.tar` & `multicontents-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-16 01:17:47.000000 multicontents-0.3.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2578 2021-02-16 01:17:47.000000 multicontents-0.3.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1532 2021-02-16 01:16:33.000000 multicontents-0.3.0/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-02-16 01:17:47.000000 multicontents-0.3.0/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-16 01:17:47.000000 multicontents-0.3.0/multicontents/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2924 2021-02-16 01:16:33.000000 multicontents-0.3.0/multicontents/multi_versions_file_checkpoints.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7421 2021-02-16 01:16:33.000000 multicontents-0.3.0/multicontents/multicontents_manager.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      111 2021-02-16 01:16:33.000000 multicontents-0.3.0/multicontents/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-16 01:17:47.000000 multicontents-0.3.0/multicontents.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2578 2021-02-16 01:17:47.000000 multicontents-0.3.0/multicontents.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-02-16 01:17:47.000000 multicontents-0.3.0/multicontents.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       20 2021-02-16 01:17:47.000000 multicontents-0.3.0/multicontents.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      442 2021-02-16 01:17:47.000000 multicontents-0.3.0/multicontents.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       19 2021-02-16 01:17:47.000000 multicontents-0.3.0/multicontents.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1024 2021-02-16 01:16:33.000000 multicontents-0.3.0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-16 01:17:47.000000 multicontents-0.3.0/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11529 2021-02-16 01:16:33.000000 multicontents-0.3.0/tests/multicontents_manager_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1033 2021-02-16 01:16:33.000000 multicontents-0.3.0/tests/integration_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2634 2021-02-16 01:16:33.000000 multicontents-0.3.0/tests/multi_versions_file_checkpoints_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-02-16 01:16:33.000000 multicontents-0.3.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:34:26.000000 multicontents-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-25 17:34:26.000000 multicontents-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-25 17:34:04.000000 multicontents-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:34:26.000000 multicontents-0.4.0/multicontents/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-25 17:34:04.000000 multicontents-0.4.0/multicontents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-25 17:34:04.000000 multicontents-0.4.0/multicontents/multi_versions_file_checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7421 2024-04-25 17:34:04.000000 multicontents-0.4.0/multicontents/multicontents_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:34:26.000000 multicontents-0.4.0/multicontents.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-25 17:34:26.000000 multicontents-0.4.0/multicontents.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-25 17:34:26.000000 multicontents-0.4.0/multicontents.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 17:34:26.000000 multicontents-0.4.0/multicontents.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-25 17:34:26.000000 multicontents-0.4.0/multicontents.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-25 17:34:26.000000 multicontents-0.4.0/multicontents.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 17:34:26.000000 multicontents-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-25 17:34:04.000000 multicontents-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:34:26.000000 multicontents-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:34:04.000000 multicontents-0.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-25 17:34:04.000000 multicontents-0.4.0/tests/integration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-25 17:34:04.000000 multicontents-0.4.0/tests/multi_versions_file_checkpoints_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11529 2024-04-25 17:34:04.000000 multicontents-0.4.0/tests/multicontents_manager_test.py
```

### Comparing `multicontents-0.3.0/PKG-INFO` & `multicontents-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multicontents
-Version: 0.3.0
+Version: 0.4.0
 Summary: providing contents from multiple sources in jupyter notebook
 Home-page: https://github.com/lydian/multicontents
 Author: Lydian Lee
 Author-email: lydianly@gmail.com
 Maintainer: Lydian Lee
 Maintainer-email: lydianly@gmail.com
 License: UNKNOWN
```

### Comparing `multicontents-0.3.0/README.md` & `multicontents-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `multicontents-0.3.0/multicontents/multi_versions_file_checkpoints.py` & `multicontents-0.4.0/multicontents/multi_versions_file_checkpoints.py`

 * *Files identical despite different names*

### Comparing `multicontents-0.3.0/multicontents/multicontents_manager.py` & `multicontents-0.4.0/multicontents/multicontents_manager.py`

 * *Files identical despite different names*

### Comparing `multicontents-0.3.0/multicontents.egg-info/PKG-INFO` & `multicontents-0.4.0/multicontents.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multicontents
-Version: 0.3.0
+Version: 0.4.0
 Summary: providing contents from multiple sources in jupyter notebook
 Home-page: https://github.com/lydian/multicontents
 Author: Lydian Lee
 Author-email: lydianly@gmail.com
 Maintainer: Lydian Lee
 Maintainer-email: lydianly@gmail.com
 License: UNKNOWN
```

### Comparing `multicontents-0.3.0/setup.py` & `multicontents-0.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)), "README.md")) as fp:
     long_description = fp.read()
 
 setup(
     name="multicontents",
-    version="0.3.0",
+    version="0.4.0",
     description="providing contents from multiple sources in jupyter notebook",
     long_description_content_type="text/markdown",
     long_description=long_description,
     url="https://github.com/lydian/multicontents",
     author="Lydian Lee",
     author_email="lydianly@gmail.com",
     maintainer="Lydian Lee",
```

### Comparing `multicontents-0.3.0/tests/multicontents_manager_test.py` & `multicontents-0.4.0/tests/multicontents_manager_test.py`

 * *Files identical despite different names*

### Comparing `multicontents-0.3.0/tests/integration_test.py` & `multicontents-0.4.0/tests/integration_test.py`

 * *Files identical despite different names*

### Comparing `multicontents-0.3.0/tests/multi_versions_file_checkpoints_test.py` & `multicontents-0.4.0/tests/multi_versions_file_checkpoints_test.py`

 * *Files identical despite different names*

