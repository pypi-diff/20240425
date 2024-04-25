# Comparing `tmp/math_ops_131-1.3.2.tar.gz` & `tmp/math_ops_131-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "math_ops_131-1.3.2.tar", last modified: Thu Apr 25 11:41:38 2024, max compression
+gzip compressed data, was "math_ops_131-1.3.3.tar", last modified: Thu Apr 25 11:49:54 2024, max compression
```

## Comparing `math_ops_131-1.3.2.tar` & `math_ops_131-1.3.3.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxrwxr-x   0 unnath    (1000) unnath    (1000)        0 2024-04-25 11:41:38.160118 math_ops_131-1.3.2/
--rw-rw-r--   0 unnath    (1000) unnath    (1000)     1253 2024-04-25 11:41:38.160118 math_ops_131-1.3.2/PKG-INFO
--rw-rw-r--   0 unnath    (1000) unnath    (1000)      777 2024-04-25 11:20:34.000000 math_ops_131-1.3.2/README.md
-drwxrwxr-x   0 unnath    (1000) unnath    (1000)        0 2024-04-25 11:41:38.160118 math_ops_131-1.3.2/math_ops_131.egg-info/
--rw-rw-r--   0 unnath    (1000) unnath    (1000)     1253 2024-04-25 11:41:37.000000 math_ops_131-1.3.2/math_ops_131.egg-info/PKG-INFO
--rw-rw-r--   0 unnath    (1000) unnath    (1000)      162 2024-04-25 11:41:37.000000 math_ops_131-1.3.2/math_ops_131.egg-info/SOURCES.txt
--rw-rw-r--   0 unnath    (1000) unnath    (1000)        1 2024-04-25 11:41:37.000000 math_ops_131-1.3.2/math_ops_131.egg-info/dependency_links.txt
--rw-rw-r--   0 unnath    (1000) unnath    (1000)        1 2024-04-25 11:41:37.000000 math_ops_131-1.3.2/math_ops_131.egg-info/top_level.txt
--rw-rw-r--   0 unnath    (1000) unnath    (1000)       38 2024-04-25 11:41:38.160118 math_ops_131-1.3.2/setup.cfg
--rw-rw-r--   0 unnath    (1000) unnath    (1000)      699 2024-04-25 11:41:27.000000 math_ops_131-1.3.2/setup.py
+drwxrwxr-x   0 unnath    (1000) unnath    (1000)        0 2024-04-25 11:49:54.809813 math_ops_131-1.3.3/
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)     1253 2024-04-25 11:49:54.809813 math_ops_131-1.3.3/PKG-INFO
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)      777 2024-04-25 11:20:34.000000 math_ops_131-1.3.3/README.md
+drwxrwxr-x   0 unnath    (1000) unnath    (1000)        0 2024-04-25 11:49:54.805813 math_ops_131-1.3.3/calculator/
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)        0 2024-04-25 11:48:10.000000 math_ops_131-1.3.3/calculator/__init__.py
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)      696 2024-04-25 11:03:26.000000 math_ops_131-1.3.3/calculator/calculator.py
+drwxrwxr-x   0 unnath    (1000) unnath    (1000)        0 2024-04-25 11:49:54.805813 math_ops_131-1.3.3/math_ops_131.egg-info/
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)     1253 2024-04-25 11:49:54.000000 math_ops_131-1.3.3/math_ops_131.egg-info/PKG-INFO
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)      210 2024-04-25 11:49:54.000000 math_ops_131-1.3.3/math_ops_131.egg-info/SOURCES.txt
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)        1 2024-04-25 11:49:54.000000 math_ops_131-1.3.3/math_ops_131.egg-info/dependency_links.txt
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)       11 2024-04-25 11:49:54.000000 math_ops_131-1.3.3/math_ops_131.egg-info/top_level.txt
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)       38 2024-04-25 11:49:54.809813 math_ops_131-1.3.3/setup.cfg
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)      699 2024-04-25 11:49:49.000000 math_ops_131-1.3.3/setup.py
```

### Comparing `math_ops_131-1.3.2/PKG-INFO` & `math_ops_131-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: math_ops_131
-Version: 1.3.2
+Version: 1.3.3
 Summary: A Python package for basic mathematical operations.
 Home-page: https://github.com/AspiringPianist/math_ops_131
 Author: Unnath Chittimalla
 Author-email: unnath.chittimalla@iiitb.ac.in
 License: MIT License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `math_ops_131-1.3.2/README.md` & `math_ops_131-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `math_ops_131-1.3.2/math_ops_131.egg-info/PKG-INFO` & `math_ops_131-1.3.3/math_ops_131.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: math-ops-131
-Version: 1.3.2
+Version: 1.3.3
 Summary: A Python package for basic mathematical operations.
 Home-page: https://github.com/AspiringPianist/math_ops_131
 Author: Unnath Chittimalla
 Author-email: unnath.chittimalla@iiitb.ac.in
 License: MIT License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `math_ops_131-1.3.2/setup.py` & `math_ops_131-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='math_ops_131',
-    version='1.3.2',
+    version='1.3.3',
     packages=find_packages(),
     description='A Python package for basic mathematical operations.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Unnath Chittimalla',
     license = 'MIT License',
     author_email='unnath.chittimalla@iiitb.ac.in',
```

