# Comparing `tmp/math_ops_131-1.0.tar.gz` & `tmp/math_ops_131-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "math_ops_131-1.0.tar", last modified: Sat Apr 20 12:07:37 2024, max compression
+gzip compressed data, was "math_ops_131-1.1.tar", last modified: Thu Apr 25 11:06:14 2024, max compression
```

## Comparing `math_ops_131-1.0.tar` & `math_ops_131-1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxr-x   0 unnath    (1000) unnath    (1000)        0 2024-04-20 12:07:37.731278 math_ops_131-1.0/
--rw-rw-r--   0 unnath    (1000) unnath    (1000)      448 2024-04-20 12:07:37.731278 math_ops_131-1.0/PKG-INFO
-drwxrwxr-x   0 unnath    (1000) unnath    (1000)        0 2024-04-20 12:07:37.731278 math_ops_131-1.0/math_ops_131.egg-info/
--rw-rw-r--   0 unnath    (1000) unnath    (1000)      448 2024-04-20 12:07:37.000000 math_ops_131-1.0/math_ops_131.egg-info/PKG-INFO
--rw-rw-r--   0 unnath    (1000) unnath    (1000)      152 2024-04-20 12:07:37.000000 math_ops_131-1.0/math_ops_131.egg-info/SOURCES.txt
--rw-rw-r--   0 unnath    (1000) unnath    (1000)        1 2024-04-20 12:07:37.000000 math_ops_131-1.0/math_ops_131.egg-info/dependency_links.txt
--rw-rw-r--   0 unnath    (1000) unnath    (1000)        1 2024-04-20 12:07:37.000000 math_ops_131-1.0/math_ops_131.egg-info/top_level.txt
--rw-rw-r--   0 unnath    (1000) unnath    (1000)       38 2024-04-20 12:07:37.731278 math_ops_131-1.0/setup.cfg
--rw-rw-r--   0 unnath    (1000) unnath    (1000)      521 2024-04-20 12:04:40.000000 math_ops_131-1.0/setup.py
+drwxrwxr-x   0 unnath    (1000) unnath    (1000)        0 2024-04-25 11:06:14.095473 math_ops_131-1.1/
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)      448 2024-04-25 11:06:14.095473 math_ops_131-1.1/PKG-INFO
+drwxrwxr-x   0 unnath    (1000) unnath    (1000)        0 2024-04-25 11:06:14.091473 math_ops_131-1.1/math_ops_131.egg-info/
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)      448 2024-04-25 11:06:13.000000 math_ops_131-1.1/math_ops_131.egg-info/PKG-INFO
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)      152 2024-04-25 11:06:13.000000 math_ops_131-1.1/math_ops_131.egg-info/SOURCES.txt
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)        1 2024-04-25 11:06:13.000000 math_ops_131-1.1/math_ops_131.egg-info/dependency_links.txt
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)        1 2024-04-25 11:06:13.000000 math_ops_131-1.1/math_ops_131.egg-info/top_level.txt
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)       38 2024-04-25 11:06:14.095473 math_ops_131-1.1/setup.cfg
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)      521 2024-04-25 11:03:49.000000 math_ops_131-1.1/setup.py
```

### Comparing `math_ops_131-1.0/setup.py` & `math_ops_131-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='math_ops_131',
-    version='1.0',
+    version='1.1',
     packages=find_packages(),
     description='A Python package for basic mathematical operations.',
     author='Unnath Chittimalla',
     author_email='unnath.chittimalla@iiitb.ac.in',
     url='https://github.com/AspiringPianist/math_operations_package',
     classifiers=[
         'Programming Language :: Python :: 3',
```

