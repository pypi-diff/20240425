# Comparing `tmp/autocortext_py-0.1.0.tar.gz` & `tmp/autocortext_py-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autocortext_py-0.1.0.tar", last modified: Wed Apr 24 23:53:47 2024, max compression
+gzip compressed data, was "autocortext_py-0.1.1.tar", last modified: Thu Apr 25 00:13:12 2024, max compression
```

## Comparing `autocortext_py-0.1.0.tar` & `autocortext_py-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mark       (502) staff       (20)        0 2024-04-24 23:53:47.503057 autocortext_py-0.1.0/
--rw-r--r--   0 mark       (502) staff       (20)     1072 2024-04-24 23:42:07.000000 autocortext_py-0.1.0/LICENSE
--rw-r--r--   0 mark       (502) staff       (20)     1199 2024-04-24 23:53:47.502825 autocortext_py-0.1.0/PKG-INFO
--rw-r--r--   0 mark       (502) staff       (20)      657 2024-04-24 23:38:31.000000 autocortext_py-0.1.0/README.md
-drwxr-xr-x   0 mark       (502) staff       (20)        0 2024-04-24 23:53:47.500963 autocortext_py-0.1.0/autocortext_py/
--rw-r--r--   0 mark       (502) staff       (20)       32 2024-04-24 23:10:13.000000 autocortext_py-0.1.0/autocortext_py/__init__.py
--rw-r--r--   0 mark       (502) staff       (20)      506 2024-04-24 23:34:02.000000 autocortext_py-0.1.0/autocortext_py/client.py
-drwxr-xr-x   0 mark       (502) staff       (20)        0 2024-04-24 23:53:47.502347 autocortext_py-0.1.0/autocortext_py.egg-info/
--rw-r--r--   0 mark       (502) staff       (20)     1199 2024-04-24 23:53:47.000000 autocortext_py-0.1.0/autocortext_py.egg-info/PKG-INFO
--rw-r--r--   0 mark       (502) staff       (20)      267 2024-04-24 23:53:47.000000 autocortext_py-0.1.0/autocortext_py.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (502) staff       (20)        1 2024-04-24 23:53:47.000000 autocortext_py-0.1.0/autocortext_py.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (502) staff       (20)       12 2024-04-24 23:53:47.000000 autocortext_py-0.1.0/autocortext_py.egg-info/requires.txt
--rw-r--r--   0 mark       (502) staff       (20)       15 2024-04-24 23:53:47.000000 autocortext_py-0.1.0/autocortext_py.egg-info/top_level.txt
--rw-r--r--   0 mark       (502) staff       (20)       38 2024-04-24 23:53:47.503291 autocortext_py-0.1.0/setup.cfg
--rw-r--r--   0 mark       (502) staff       (20)      735 2024-04-24 23:47:53.000000 autocortext_py-0.1.0/setup.py
+drwxr-xr-x   0 mark       (502) staff       (20)        0 2024-04-25 00:13:12.620073 autocortext_py-0.1.1/
+-rw-r--r--   0 mark       (502) staff       (20)     1072 2024-04-24 23:42:07.000000 autocortext_py-0.1.1/LICENSE
+-rw-r--r--   0 mark       (502) staff       (20)     1144 2024-04-25 00:13:12.619903 autocortext_py-0.1.1/PKG-INFO
+-rw-r--r--   0 mark       (502) staff       (20)      657 2024-04-25 00:08:52.000000 autocortext_py-0.1.1/README.md
+drwxr-xr-x   0 mark       (502) staff       (20)        0 2024-04-25 00:13:12.618669 autocortext_py-0.1.1/autocortext_py/
+-rw-r--r--   0 mark       (502) staff       (20)       32 2024-04-24 23:10:13.000000 autocortext_py-0.1.1/autocortext_py/__init__.py
+-rw-r--r--   0 mark       (502) staff       (20)      506 2024-04-24 23:34:02.000000 autocortext_py-0.1.1/autocortext_py/client.py
+drwxr-xr-x   0 mark       (502) staff       (20)        0 2024-04-25 00:13:12.619702 autocortext_py-0.1.1/autocortext_py.egg-info/
+-rw-r--r--   0 mark       (502) staff       (20)     1144 2024-04-25 00:13:12.000000 autocortext_py-0.1.1/autocortext_py.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (502) staff       (20)      267 2024-04-25 00:13:12.000000 autocortext_py-0.1.1/autocortext_py.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (502) staff       (20)        1 2024-04-25 00:13:12.000000 autocortext_py-0.1.1/autocortext_py.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (502) staff       (20)       12 2024-04-25 00:13:12.000000 autocortext_py-0.1.1/autocortext_py.egg-info/requires.txt
+-rw-r--r--   0 mark       (502) staff       (20)       15 2024-04-25 00:13:12.000000 autocortext_py-0.1.1/autocortext_py.egg-info/top_level.txt
+-rw-r--r--   0 mark       (502) staff       (20)       38 2024-04-25 00:13:12.620141 autocortext_py-0.1.1/setup.cfg
+-rw-r--r--   0 mark       (502) staff       (20)      681 2024-04-25 00:12:35.000000 autocortext_py-0.1.1/setup.py
```

### Comparing `autocortext_py-0.1.0/LICENSE` & `autocortext_py-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autocortext_py-0.1.0/PKG-INFO` & `autocortext_py-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 Metadata-Version: 2.1
 Name: autocortext_py
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple client for AutoCortext API
 Home-page: https://autocortext.com
 Author: Mark Watson
 Author-email: markus.c.watson@gmail.com
 License: UNKNOWN
 Keywords: autocortext
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## AutoCortext API CLient
 
-This is a cimple client for the AutoCortext API.
+This is a simple client for the AutoCortext API.
 
 ### Setup
 
 1. An `.env` file with the variable `AUTOCORTEXT_API_KEY` set to a valid key.
 1. An `.env` file with the variable `AUTOCORTEXT_ORG_ID` set to a valid organization ID.
 
 ### Example
 
 Install the AutoCortext clinet using `pip`.
 
 ```shell
-pip istall autocortext_py
+pip istall autocortext-py
 ```
 
 Use the client in your source code.
 
 ```python
 from autocortext_py import AutoCortext
 import os
```

### Comparing `autocortext_py-0.1.0/README.md` & `autocortext_py-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ## AutoCortext API CLient
 
-This is a cimple client for the AutoCortext API.
+This is a simple client for the AutoCortext API.
 
 ### Setup
 
 1. An `.env` file with the variable `AUTOCORTEXT_API_KEY` set to a valid key.
 1. An `.env` file with the variable `AUTOCORTEXT_ORG_ID` set to a valid organization ID.
 
 ### Example
 
 Install the AutoCortext clinet using `pip`.
 
 ```shell
-pip istall autocortext_py
+pip istall autocortext-py
 ```
 
 Use the client in your source code.
 
 ```python
 from autocortext_py import AutoCortext
 import os
```

### Comparing `autocortext_py-0.1.0/autocortext_py.egg-info/PKG-INFO` & `autocortext_py-0.1.1/autocortext_py.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 Metadata-Version: 2.1
 Name: autocortext-py
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple client for AutoCortext API
 Home-page: https://autocortext.com
 Author: Mark Watson
 Author-email: markus.c.watson@gmail.com
 License: UNKNOWN
 Keywords: autocortext
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## AutoCortext API CLient
 
-This is a cimple client for the AutoCortext API.
+This is a simple client for the AutoCortext API.
 
 ### Setup
 
 1. An `.env` file with the variable `AUTOCORTEXT_API_KEY` set to a valid key.
 1. An `.env` file with the variable `AUTOCORTEXT_ORG_ID` set to a valid organization ID.
 
 ### Example
 
 Install the AutoCortext clinet using `pip`.
 
 ```shell
-pip istall autocortext_py
+pip istall autocortext-py
 ```
 
 Use the client in your source code.
 
 ```python
 from autocortext_py import AutoCortext
 import os
```

### Comparing `autocortext_py-0.1.0/setup.py` & `autocortext_py-0.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="autocortext_py",
-    version="0.1.0",
+    version="0.1.1",
     description="Simple client for AutoCortext API",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Mark Watson",
     author_email="markus.c.watson@gmail.com",
     url="https://autocortext.com",
     keywords=["autocortext"],
@@ -14,12 +14,11 @@
     install_requires=[
         "requests",
         "os",
     ],
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
-        "Operating System :: MacOS :: MacOS X",
-        "Operating System :: Microsoft :: Windows",
+        "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
 )
```

