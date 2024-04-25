# Comparing `tmp/highlevel_python-0.1.2.tar.gz` & `tmp/highlevel_python-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "highlevel_python-0.1.2.tar", max compression
+gzip compressed data, was "highlevel_python-0.1.3.tar", max compression
```

## Comparing `highlevel_python-0.1.2.tar` & `highlevel_python-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-01-04 14:02:02.002143 highlevel_python-0.1.2/highlevel/__init__.py
--rw-r--r--   0        0        0     8503 2024-01-04 14:02:02.003146 highlevel_python-0.1.2/highlevel/client.py
--rw-r--r--   0        0        0      143 2024-01-04 14:02:02.003146 highlevel_python-0.1.2/highlevel/exceptions.py
--rw-r--r--   0        0        0      435 2024-01-04 14:02:02.004145 highlevel_python-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1596 2024-01-04 14:02:02.002143 highlevel_python-0.1.2/README.md
--rw-r--r--   0        0        0     2297 1970-01-01 00:00:00.000000 highlevel_python-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-25 14:16:23.563971 highlevel_python-0.1.3/highlevel/__init__.py
+-rw-r--r--   0        0        0     4706 2024-04-25 14:16:23.563971 highlevel_python-0.1.3/highlevel/client.py
+-rw-r--r--   0        0        0      143 2024-04-25 14:16:23.564970 highlevel_python-0.1.3/highlevel/exceptions.py
+-rw-r--r--   0        0        0      437 2024-04-25 14:16:23.565970 highlevel_python-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1596 2024-04-25 14:16:23.562971 highlevel_python-0.1.3/README.md
+-rw-r--r--   0        0        0     2299 1970-01-01 00:00:00.000000 highlevel_python-0.1.3/PKG-INFO
```

### Comparing `highlevel_python-0.1.2/README.md` & `highlevel_python-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 # highlevel-python
-![](https://img.shields.io/badge/version-0.1.4-success) ![](https://img.shields.io/badge/Python-3.8%20|%203.9%20|%203.10%20|%203.11-4B8BBE?logo=python&logoColor=white)  
+![](https://img.shields.io/badge/version-0.1.3-success) ![](https://img.shields.io/badge/Python-3.8%20|%203.9%20|%203.10%20|%203.11-4B8BBE?logo=python&logoColor=white)  
 
 *highlevel-python* is an API wrapper for highlevel, written in Python.  
 This library uses Oauth2 for authentication.
 ## Installing
 ```
 pip install highlevel-python
 ```
```

### Comparing `highlevel_python-0.1.2/PKG-INFO` & `highlevel_python-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: highlevel-python
-Version: 0.1.2
+Version: 0.1.3
 Summary: API wrapper for Highlevel written in Python
 License: MIT
-Author: Diego C
-Author-email: dcastano@gearplug.io
+Author: Gearplug Team
+Author-email: apps@gearplug.io
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: requests (>=2.26.0,<3.0.0)
 Requires-Dist: requests_oauthlib (>=1.3.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 
 # highlevel-python
-![](https://img.shields.io/badge/version-0.1.4-success) ![](https://img.shields.io/badge/Python-3.8%20|%203.9%20|%203.10%20|%203.11-4B8BBE?logo=python&logoColor=white)  
+![](https://img.shields.io/badge/version-0.1.3-success) ![](https://img.shields.io/badge/Python-3.8%20|%203.9%20|%203.10%20|%203.11-4B8BBE?logo=python&logoColor=white)  
 
 *highlevel-python* is an API wrapper for highlevel, written in Python.  
 This library uses Oauth2 for authentication.
 ## Installing
 ```
 pip install highlevel-python
 ```
```

