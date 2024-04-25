# Comparing `tmp/math_ops_131-1.3.1.tar.gz` & `tmp/math_ops_131-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "math_ops_131-1.3.1.tar", last modified: Thu Apr 25 11:20:47 2024, max compression
+gzip compressed data, was "math_ops_131-1.3.2.tar", last modified: Thu Apr 25 11:41:38 2024, max compression
```

## Comparing `math_ops_131-1.3.1.tar` & `math_ops_131-1.3.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 unnath    (1000) unnath    (1000)        0 2024-04-25 11:20:47.851141 math_ops_131-1.3.1/
--rw-rw-r--   0 unnath    (1000) unnath    (1000)     1260 2024-04-25 11:20:47.847141 math_ops_131-1.3.1/PKG-INFO
--rw-rw-r--   0 unnath    (1000) unnath    (1000)      777 2024-04-25 11:20:34.000000 math_ops_131-1.3.1/README.md
-drwxrwxr-x   0 unnath    (1000) unnath    (1000)        0 2024-04-25 11:20:47.847141 math_ops_131-1.3.1/math_ops_131.egg-info/
--rw-rw-r--   0 unnath    (1000) unnath    (1000)     1260 2024-04-25 11:20:47.000000 math_ops_131-1.3.1/math_ops_131.egg-info/PKG-INFO
--rw-rw-r--   0 unnath    (1000) unnath    (1000)      162 2024-04-25 11:20:47.000000 math_ops_131-1.3.1/math_ops_131.egg-info/SOURCES.txt
--rw-rw-r--   0 unnath    (1000) unnath    (1000)        1 2024-04-25 11:20:47.000000 math_ops_131-1.3.1/math_ops_131.egg-info/dependency_links.txt
--rw-rw-r--   0 unnath    (1000) unnath    (1000)        1 2024-04-25 11:20:47.000000 math_ops_131-1.3.1/math_ops_131.egg-info/top_level.txt
--rw-rw-r--   0 unnath    (1000) unnath    (1000)       38 2024-04-25 11:20:47.851141 math_ops_131-1.3.1/setup.cfg
--rw-rw-r--   0 unnath    (1000) unnath    (1000)      712 2024-04-25 11:20:43.000000 math_ops_131-1.3.1/setup.py
+drwxrwxr-x   0 unnath    (1000) unnath    (1000)        0 2024-04-25 11:41:38.160118 math_ops_131-1.3.2/
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)     1253 2024-04-25 11:41:38.160118 math_ops_131-1.3.2/PKG-INFO
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)      777 2024-04-25 11:20:34.000000 math_ops_131-1.3.2/README.md
+drwxrwxr-x   0 unnath    (1000) unnath    (1000)        0 2024-04-25 11:41:38.160118 math_ops_131-1.3.2/math_ops_131.egg-info/
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)     1253 2024-04-25 11:41:37.000000 math_ops_131-1.3.2/math_ops_131.egg-info/PKG-INFO
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)      162 2024-04-25 11:41:37.000000 math_ops_131-1.3.2/math_ops_131.egg-info/SOURCES.txt
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)        1 2024-04-25 11:41:37.000000 math_ops_131-1.3.2/math_ops_131.egg-info/dependency_links.txt
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)        1 2024-04-25 11:41:37.000000 math_ops_131-1.3.2/math_ops_131.egg-info/top_level.txt
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)       38 2024-04-25 11:41:38.160118 math_ops_131-1.3.2/setup.cfg
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)      699 2024-04-25 11:41:27.000000 math_ops_131-1.3.2/setup.py
```

### Comparing `math_ops_131-1.3.1/PKG-INFO` & `math_ops_131-1.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: math_ops_131
-Version: 1.3.1
+Version: 1.3.2
 Summary: A Python package for basic mathematical operations.
-Home-page: https://github.com/AspiringPianist/math_operations_package
+Home-page: https://github.com/AspiringPianist/math_ops_131
 Author: Unnath Chittimalla
 Author-email: unnath.chittimalla@iiitb.ac.in
-License: UNKNOWN
+License: MIT License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # math_ops_131 Package
```

### Comparing `math_ops_131-1.3.1/README.md` & `math_ops_131-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `math_ops_131-1.3.1/math_ops_131.egg-info/PKG-INFO` & `math_ops_131-1.3.2/math_ops_131.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: math-ops-131
-Version: 1.3.1
+Version: 1.3.2
 Summary: A Python package for basic mathematical operations.
-Home-page: https://github.com/AspiringPianist/math_operations_package
+Home-page: https://github.com/AspiringPianist/math_ops_131
 Author: Unnath Chittimalla
 Author-email: unnath.chittimalla@iiitb.ac.in
-License: UNKNOWN
+License: MIT License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # math_ops_131 Package
```

### Comparing `math_ops_131-1.3.1/setup.py` & `math_ops_131-1.3.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='math_ops_131',
-    version='1.3.1',
+    version='1.3.2',
     packages=find_packages(),
     description='A Python package for basic mathematical operations.',
     long_description=long_description,
-    long_description_content_type='text/markdown',  # Ensure this line is present
+    long_description_content_type='text/markdown',
     author='Unnath Chittimalla',
+    license = 'MIT License',
     author_email='unnath.chittimalla@iiitb.ac.in',
-    url='https://github.com/AspiringPianist/math_operations_package',
+    url='https://github.com/AspiringPianist/math_ops_131',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
 )
```

