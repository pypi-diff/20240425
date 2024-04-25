# Comparing `tmp/math_ops_131-1.3.tar.gz` & `tmp/math_ops_131-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "math_ops_131-1.3.tar", last modified: Thu Apr 25 11:17:28 2024, max compression
+gzip compressed data, was "math_ops_131-1.3.1.tar", last modified: Thu Apr 25 11:20:47 2024, max compression
```

## Comparing `math_ops_131-1.3.tar` & `math_ops_131-1.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 unnath    (1000) unnath    (1000)        0 2024-04-25 11:17:28.088575 math_ops_131-1.3/
--rw-rw-r--   0 unnath    (1000) unnath    (1000)     1261 2024-04-25 11:17:28.088575 math_ops_131-1.3/PKG-INFO
--rw-rw-r--   0 unnath    (1000) unnath    (1000)      780 2024-04-25 11:14:01.000000 math_ops_131-1.3/README.md
-drwxrwxr-x   0 unnath    (1000) unnath    (1000)        0 2024-04-25 11:17:28.084575 math_ops_131-1.3/math_ops_131.egg-info/
--rw-rw-r--   0 unnath    (1000) unnath    (1000)     1261 2024-04-25 11:17:27.000000 math_ops_131-1.3/math_ops_131.egg-info/PKG-INFO
--rw-rw-r--   0 unnath    (1000) unnath    (1000)      162 2024-04-25 11:17:27.000000 math_ops_131-1.3/math_ops_131.egg-info/SOURCES.txt
--rw-rw-r--   0 unnath    (1000) unnath    (1000)        1 2024-04-25 11:17:27.000000 math_ops_131-1.3/math_ops_131.egg-info/dependency_links.txt
--rw-rw-r--   0 unnath    (1000) unnath    (1000)        1 2024-04-25 11:17:27.000000 math_ops_131-1.3/math_ops_131.egg-info/top_level.txt
--rw-rw-r--   0 unnath    (1000) unnath    (1000)       38 2024-04-25 11:17:28.088575 math_ops_131-1.3/setup.cfg
--rw-rw-r--   0 unnath    (1000) unnath    (1000)      710 2024-04-25 11:17:16.000000 math_ops_131-1.3/setup.py
+drwxrwxr-x   0 unnath    (1000) unnath    (1000)        0 2024-04-25 11:20:47.851141 math_ops_131-1.3.1/
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)     1260 2024-04-25 11:20:47.847141 math_ops_131-1.3.1/PKG-INFO
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)      777 2024-04-25 11:20:34.000000 math_ops_131-1.3.1/README.md
+drwxrwxr-x   0 unnath    (1000) unnath    (1000)        0 2024-04-25 11:20:47.847141 math_ops_131-1.3.1/math_ops_131.egg-info/
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)     1260 2024-04-25 11:20:47.000000 math_ops_131-1.3.1/math_ops_131.egg-info/PKG-INFO
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)      162 2024-04-25 11:20:47.000000 math_ops_131-1.3.1/math_ops_131.egg-info/SOURCES.txt
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)        1 2024-04-25 11:20:47.000000 math_ops_131-1.3.1/math_ops_131.egg-info/dependency_links.txt
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)        1 2024-04-25 11:20:47.000000 math_ops_131-1.3.1/math_ops_131.egg-info/top_level.txt
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)       38 2024-04-25 11:20:47.851141 math_ops_131-1.3.1/setup.cfg
+-rw-rw-r--   0 unnath    (1000) unnath    (1000)      712 2024-04-25 11:20:43.000000 math_ops_131-1.3.1/setup.py
```

### Comparing `math_ops_131-1.3/PKG-INFO` & `math_ops_131-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: math_ops_131
-Version: 1.3
+Version: 1.3.1
 Summary: A Python package for basic mathematical operations.
 Home-page: https://github.com/AspiringPianist/math_operations_package
 Author: Unnath Chittimalla
 Author-email: unnath.chittimalla@iiitb.ac.in
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -26,15 +26,15 @@
 pip install math_ops_131 
 ```
 
 ## Usage 
 
 Import the `math_ops_131.calculator` module to use the provided functions: 
 ```python 
-import math_operations.calculator as calc 
+import math_ops_131.calculator as calc 
 
 # Example usage 
 result_add = calc.add(5, 3)  # Result: 8 
 result_sub = calc.subtract(10, 4)  # Result: 6  
 result_mul = calc.multiply(2, 7)  # Result: 14 
 ```
 For detailed documentation of each function, refer to the docstrings in `calculator.py`.
```

### Comparing `math_ops_131-1.3/README.md` & `math_ops_131-1.3.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 pip install math_ops_131 
 ```
 
 ## Usage 
 
 Import the `math_ops_131.calculator` module to use the provided functions: 
 ```python 
-import math_operations.calculator as calc 
+import math_ops_131.calculator as calc 
 
 # Example usage 
 result_add = calc.add(5, 3)  # Result: 8 
 result_sub = calc.subtract(10, 4)  # Result: 6  
 result_mul = calc.multiply(2, 7)  # Result: 14 
 ```
 For detailed documentation of each function, refer to the docstrings in `calculator.py`.
```

### Comparing `math_ops_131-1.3/math_ops_131.egg-info/PKG-INFO` & `math_ops_131-1.3.1/math_ops_131.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: math-ops-131
-Version: 1.3
+Version: 1.3.1
 Summary: A Python package for basic mathematical operations.
 Home-page: https://github.com/AspiringPianist/math_operations_package
 Author: Unnath Chittimalla
 Author-email: unnath.chittimalla@iiitb.ac.in
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -26,15 +26,15 @@
 pip install math_ops_131 
 ```
 
 ## Usage 
 
 Import the `math_ops_131.calculator` module to use the provided functions: 
 ```python 
-import math_operations.calculator as calc 
+import math_ops_131.calculator as calc 
 
 # Example usage 
 result_add = calc.add(5, 3)  # Result: 8 
 result_sub = calc.subtract(10, 4)  # Result: 6  
 result_mul = calc.multiply(2, 7)  # Result: 14 
 ```
 For detailed documentation of each function, refer to the docstrings in `calculator.py`.
```

### Comparing `math_ops_131-1.3/setup.py` & `math_ops_131-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='math_ops_131',
-    version='1.3',
+    version='1.3.1',
     packages=find_packages(),
     description='A Python package for basic mathematical operations.',
     long_description=long_description,
     long_description_content_type='text/markdown',  # Ensure this line is present
     author='Unnath Chittimalla',
     author_email='unnath.chittimalla@iiitb.ac.in',
     url='https://github.com/AspiringPianist/math_operations_package',
```

