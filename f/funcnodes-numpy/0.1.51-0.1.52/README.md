# Comparing `tmp/funcnodes_numpy-0.1.51.tar.gz` & `tmp/funcnodes_numpy-0.1.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcnodes_numpy-0.1.51.tar", max compression
+gzip compressed data, was "funcnodes_numpy-0.1.52.tar", max compression
```

## Comparing `funcnodes_numpy-0.1.51.tar` & `funcnodes_numpy-0.1.52.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    13387 2024-04-11 20:27:32.034210 funcnodes_numpy-0.1.51/funcnodes_numpy/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 09:55:21.532750 funcnodes_numpy-0.1.51/funcnodes_numpy/_array_creation.py
--rw-r--r--   0        0        0    82702 2024-03-22 12:33:05.106319 funcnodes_numpy-0.1.51/funcnodes_numpy/_core/__init__.py
--rw-r--r--   0        0        0      481 2024-03-19 16:23:50.188790 funcnodes_numpy-0.1.51/funcnodes_numpy/_core/_datetime.py
--rw-r--r--   0        0        0     1182 2024-03-22 12:20:39.200788 funcnodes_numpy-0.1.51/funcnodes_numpy/_core/_defchararray.py
--rw-r--r--   0        0        0        0 2024-03-19 09:12:23.563823 funcnodes_numpy-0.1.51/funcnodes_numpy/_core/_fromnumeric.py
--rw-r--r--   0        0        0        0 2024-03-19 09:13:00.460173 funcnodes_numpy-0.1.51/funcnodes_numpy/_core/_multiarray.py
--rw-r--r--   0        0        0    75951 2024-03-22 06:01:33.436725 funcnodes_numpy-0.1.51/funcnodes_numpy/_core/ufuncs.py
--rw-r--r--   0        0        0     3927 2024-03-22 12:32:44.058278 funcnodes_numpy-0.1.51/funcnodes_numpy/_dtypes.py
--rw-r--r--   0        0        0       91 2024-03-22 12:20:39.204892 funcnodes_numpy-0.1.51/funcnodes_numpy/_lib/__init__.py
--rw-r--r--   0        0        0     3015 2024-03-22 12:20:39.202680 funcnodes_numpy-0.1.51/funcnodes_numpy/_lib/scimath.py
--rw-r--r--   0        0        0       23 2024-03-19 12:34:04.505018 funcnodes_numpy-0.1.51/funcnodes_numpy/_linalg/__init__.py
--rw-r--r--   0        0        0     9828 2024-03-22 12:20:39.200788 funcnodes_numpy-0.1.51/funcnodes_numpy/_linalg/_linalg.py
--rw-r--r--   0        0        0    16374 2024-03-22 12:20:39.199729 funcnodes_numpy-0.1.51/funcnodes_numpy/_ndarray.py
--rw-r--r--   0        0        0     3582 2024-04-11 20:12:41.922477 funcnodes_numpy-0.1.51/funcnodes_numpy/_types.py
--rw-r--r--   0        0        0      423 2024-03-22 12:20:39.199729 funcnodes_numpy-0.1.51/funcnodes_numpy/constants.py
--rw-r--r--   0        0        0      489 2024-04-11 20:27:25.563128 funcnodes_numpy-0.1.51/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-12 14:46:02.900426 funcnodes_numpy-0.1.51/README.md
--rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 funcnodes_numpy-0.1.51/PKG-INFO
+-rw-r--r--   0        0        0    13387 2024-04-25 10:55:47.708690 funcnodes_numpy-0.1.52/funcnodes_numpy/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-18 09:55:21.532750 funcnodes_numpy-0.1.52/funcnodes_numpy/_array_creation.py
+-rw-r--r--   0        0        0    82702 2024-03-22 12:33:05.106319 funcnodes_numpy-0.1.52/funcnodes_numpy/_core/__init__.py
+-rw-r--r--   0        0        0      481 2024-03-19 16:23:50.188790 funcnodes_numpy-0.1.52/funcnodes_numpy/_core/_datetime.py
+-rw-r--r--   0        0        0     1182 2024-03-22 12:20:39.200788 funcnodes_numpy-0.1.52/funcnodes_numpy/_core/_defchararray.py
+-rw-r--r--   0        0        0        0 2024-03-19 09:12:23.563823 funcnodes_numpy-0.1.52/funcnodes_numpy/_core/_fromnumeric.py
+-rw-r--r--   0        0        0        0 2024-03-19 09:13:00.460173 funcnodes_numpy-0.1.52/funcnodes_numpy/_core/_multiarray.py
+-rw-r--r--   0        0        0    75951 2024-03-22 06:01:33.436725 funcnodes_numpy-0.1.52/funcnodes_numpy/_core/ufuncs.py
+-rw-r--r--   0        0        0     3927 2024-03-22 12:32:44.058278 funcnodes_numpy-0.1.52/funcnodes_numpy/_dtypes.py
+-rw-r--r--   0        0        0       91 2024-03-22 12:20:39.204892 funcnodes_numpy-0.1.52/funcnodes_numpy/_lib/__init__.py
+-rw-r--r--   0        0        0     3015 2024-03-22 12:20:39.202680 funcnodes_numpy-0.1.52/funcnodes_numpy/_lib/scimath.py
+-rw-r--r--   0        0        0       23 2024-03-19 12:34:04.505018 funcnodes_numpy-0.1.52/funcnodes_numpy/_linalg/__init__.py
+-rw-r--r--   0        0        0     9828 2024-03-22 12:20:39.200788 funcnodes_numpy-0.1.52/funcnodes_numpy/_linalg/_linalg.py
+-rw-r--r--   0        0        0    16374 2024-03-22 12:20:39.199729 funcnodes_numpy-0.1.52/funcnodes_numpy/_ndarray.py
+-rw-r--r--   0        0        0     3582 2024-04-11 20:12:41.922477 funcnodes_numpy-0.1.52/funcnodes_numpy/_types.py
+-rw-r--r--   0        0        0      423 2024-03-22 12:20:39.199729 funcnodes_numpy-0.1.52/funcnodes_numpy/constants.py
+-rw-r--r--   0        0        0      497 2024-04-25 10:55:36.542578 funcnodes_numpy-0.1.52/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-12 14:46:02.900426 funcnodes_numpy-0.1.52/README.md
+-rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 funcnodes_numpy-0.1.52/PKG-INFO
```

### Comparing `funcnodes_numpy-0.1.51/funcnodes_numpy/__init__.py` & `funcnodes_numpy-0.1.52/funcnodes_numpy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 from ._dtypes import DTYPE_ENUM
 
 from exposedfunctionality.function_parser.types import type_to_string
 
 import numpy as np
 
-__version__ = "0.1.51"
+__version__ = "0.1.52"
 
 
 # set the print options to display a smaller number of elements for node previews
 np.set_printoptions(threshold=100)
 
 
 def from_np(obj, preview=False):
```

### Comparing `funcnodes_numpy-0.1.51/funcnodes_numpy/_core/__init__.py` & `funcnodes_numpy-0.1.52/funcnodes_numpy/_core/__init__.py`

 * *Files identical despite different names*

### Comparing `funcnodes_numpy-0.1.51/funcnodes_numpy/_core/_defchararray.py` & `funcnodes_numpy-0.1.52/funcnodes_numpy/_core/_defchararray.py`

 * *Files identical despite different names*

### Comparing `funcnodes_numpy-0.1.51/funcnodes_numpy/_core/ufuncs.py` & `funcnodes_numpy-0.1.52/funcnodes_numpy/_core/ufuncs.py`

 * *Files identical despite different names*

### Comparing `funcnodes_numpy-0.1.51/funcnodes_numpy/_dtypes.py` & `funcnodes_numpy-0.1.52/funcnodes_numpy/_dtypes.py`

 * *Files identical despite different names*

### Comparing `funcnodes_numpy-0.1.51/funcnodes_numpy/_lib/scimath.py` & `funcnodes_numpy-0.1.52/funcnodes_numpy/_lib/scimath.py`

 * *Files identical despite different names*

### Comparing `funcnodes_numpy-0.1.51/funcnodes_numpy/_linalg/_linalg.py` & `funcnodes_numpy-0.1.52/funcnodes_numpy/_linalg/_linalg.py`

 * *Files identical despite different names*

### Comparing `funcnodes_numpy-0.1.51/funcnodes_numpy/_ndarray.py` & `funcnodes_numpy-0.1.52/funcnodes_numpy/_ndarray.py`

 * *Files identical despite different names*

### Comparing `funcnodes_numpy-0.1.51/funcnodes_numpy/_types.py` & `funcnodes_numpy-0.1.52/funcnodes_numpy/_types.py`

 * *Files identical despite different names*

### Comparing `funcnodes_numpy-0.1.51/PKG-INFO` & `funcnodes_numpy-0.1.52/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: funcnodes-numpy
-Version: 0.1.51
+Version: 0.1.52
 Summary: 
 Author: Julian Kimmig
 Author-email: julian.kimmig@gmx.net
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: funcnodes (>=0.1.11,<0.2.0)
+Requires-Dist: funcnodes (>=0.1.42,<1.0.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Description-Content-Type: text/markdown
```
