# Comparing `tmp/math_ops_131-1.2.tar.gz` & `tmp/math_ops_131-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "math_ops_131-1.2.tar", last modified: Thu Apr 25 11:14:24 2024, max compression
+gzip compressed data, was "math_ops_131-1.3.tar", last modified: Thu Apr 25 11:17:28 2024, max compression
```

## Comparing `math_ops_131-1.2.tar` & `math_ops_131-1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 unnath    (1000) unnath    (1000)        0 2024-04-25 11:14:24.187168 math_ops_131-1.2/
--rw-rw-r--   0 unnath    (1000) unnath    (1000)      448 2024-04-25 11:14:24.187168 math_ops_131-1.2/PKG-INFO
--rw-rw-r--   0 unnath    (1000) unnath    (1000)      780 2024-04-25 11:14:01.000000 math_ops_131-1.2/README.md
-drwxrwxr-x   0 unnath    (1000) unnath    (1000)        0 2024-04-25 11:14:24.187168 math_ops_131-1.2/math_ops_131.egg-info/
--rw-rw-r--   0 unnath    (1000) unnath    (1000)      448 2024-04-25 11:14:24.000000 math_ops_131-1.2/math_ops_131.egg-info/PKG-INFO
--rw-rw-r--   0 unnath    (1000) unnath    (1000)      162 2024-04-25 11:14:24.000000 math_ops_131-1.2/math_ops_131.egg-info/SOURCES.txt
--rw-rw-r--   0 unnath    (1000) unnath    (1000)        1 2024-04-25 11:14:24.000000 math_ops_131-1.2/math_ops_131.egg-info/dependency_links.txt
--rw-rw-r--   0 unnath    (1000) unnath    (1000)        1 2024-04-25 11:14:24.000000 math_ops_131-1.2/math_ops_131.egg-info/top_level.txt
--rw-rw-r--   0 unnath    (1000) unnath    (1000)       38 2024-04-25 11:14:24.187168 math_ops_131-1.2/setup.cfg
--rw-rw-r--   0 unnath    (1000) unnath    (1000)      521 2024-04-25 11:14:13.000000 math_ops_131-1.2/setup.py
+drwxrwxr-x   0 unnath    (1000) unnath    (1000)        0 2024-04-25 11:17:28.088575 math_ops_131-1.3/
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)     1261 2024-04-25 11:17:28.088575 math_ops_131-1.3/PKG-INFO
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)      780 2024-04-25 11:14:01.000000 math_ops_131-1.3/README.md
+drwxrwxr-x   0 unnath    (1000) unnath    (1000)        0 2024-04-25 11:17:28.084575 math_ops_131-1.3/math_ops_131.egg-info/
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)     1261 2024-04-25 11:17:27.000000 math_ops_131-1.3/math_ops_131.egg-info/PKG-INFO
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)      162 2024-04-25 11:17:27.000000 math_ops_131-1.3/math_ops_131.egg-info/SOURCES.txt
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)        1 2024-04-25 11:17:27.000000 math_ops_131-1.3/math_ops_131.egg-info/dependency_links.txt
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)        1 2024-04-25 11:17:27.000000 math_ops_131-1.3/math_ops_131.egg-info/top_level.txt
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)       38 2024-04-25 11:17:28.088575 math_ops_131-1.3/setup.cfg
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)      710 2024-04-25 11:17:16.000000 math_ops_131-1.3/setup.py
```

### Comparing `math_ops_131-1.2/README.md` & `math_ops_131-1.3/README.md`

 * *Files identical despite different names*

### Comparing `math_ops_131-1.2/setup.py` & `math_ops_131-1.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 from setuptools import setup, find_packages
 
+with open('README.md', 'r') as f:
+    long_description = f.read()
+
 setup(
     name='math_ops_131',
-    version='1.2',
+    version='1.3',
     packages=find_packages(),
     description='A Python package for basic mathematical operations.',
+    long_description=long_description,
+    long_description_content_type='text/markdown',  # Ensure this line is present
     author='Unnath Chittimalla',
     author_email='unnath.chittimalla@iiitb.ac.in',
     url='https://github.com/AspiringPianist/math_operations_package',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
 )
+
```

