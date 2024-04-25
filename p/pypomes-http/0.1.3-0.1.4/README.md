# Comparing `tmp/pypomes_http-0.1.3.tar.gz` & `tmp/pypomes_http-0.1.4.tar.gz`

## Comparing `pypomes_http-0.1.3.tar` & `pypomes_http-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 pypomes_http-0.1.3/src/pypomes_http/__init__.py
--rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 pypomes_http-0.1.3/src/pypomes_http/http_async.py
--rw-r--r--   0        0        0    15965 2020-02-02 00:00:00.000000 pypomes_http-0.1.3/src/pypomes_http/http_pomes.py
--rw-r--r--   0        0        0    22977 2020-02-02 00:00:00.000000 pypomes_http-0.1.3/src/pypomes_http/http_statuses.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_http-0.1.3/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_http-0.1.3/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_http-0.1.3/README.md
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 pypomes_http-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 pypomes_http-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 pypomes_http-0.1.4/src/pypomes_http/__init__.py
+-rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 pypomes_http-0.1.4/src/pypomes_http/http_async.py
+-rw-r--r--   0        0        0    15861 2020-02-02 00:00:00.000000 pypomes_http-0.1.4/src/pypomes_http/http_pomes.py
+-rw-r--r--   0        0        0    22977 2020-02-02 00:00:00.000000 pypomes_http-0.1.4/src/pypomes_http/http_statuses.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_http-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_http-0.1.4/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_http-0.1.4/README.md
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 pypomes_http-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 pypomes_http-0.1.4/PKG-INFO
```

### Comparing `pypomes_http-0.1.3/src/pypomes_http/__init__.py` & `pypomes_http-0.1.4/src/pypomes_http/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_http-0.1.3/src/pypomes_http/http_async.py` & `pypomes_http-0.1.4/src/pypomes_http/http_async.py`

 * *Files identical despite different names*

### Comparing `pypomes_http-0.1.3/src/pypomes_http/http_pomes.py` & `pypomes_http-0.1.4/src/pypomes_http/http_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import contextlib
 import copy
 import logging
 import requests
 import sys
 from flask import Request
 from pypomes_core import APP_PREFIX, env_get_int, exc_format
 from pypomes_security import access_get_token
@@ -99,42 +100,42 @@
     if result is None:
         # no, look for parameter in the URL query
         # ruff: noqa: PD011
         params = request.values
         if params:
             result = params.get(param)
 
-            # still not found, and the request's content type is JSON ?
-            if result is None and request.mimetype == MIMETYPE_JSON:
-                # yes, look for parameter in the request's body
-                params: dict = request.get_json()
-                if params:
-                    result = params.get(param)
+    # was it found ?
+    if result is None:
+        # no, look for parameter in the JSON data
+        with contextlib.suppress(Exception):
+            params = request.get_json()
+            if params:
+                result = params.get(param)
 
     return result
 
 
 def http_get_parameters(request: Request) -> dict:
     """
     Obtain the *request*'s input parameters.
 
     The following are cumulatively attempted, in sequence:
         - key/value pairs in a *JSON* structure in the request's body
         - parameters in the URL's query part
         - elements in a HTML form
 
     :param request: the Request object
-    :return: dict containing the input parameters (empty, if no input data exist)
+    :return: dict containing the input parameters (empty, if no input data exists)
     """
     # initialize the return variable
     result: dict = {}
 
-    # is JSON the content type of the request ?
-    if request.mimetype == MIMETYPE_JSON:
-        # yes, retrieve the JSON data
+    # attempt to retrieve the JSON data in body
+    with contextlib.suppress(Exception):
         result.update(request.get_json())
 
     # obtain parameters in URL query
     result.update(request.values)
 
     # obtain parameters in form
     result.update(request.form)
```

### Comparing `pypomes_http-0.1.3/src/pypomes_http/http_statuses.py` & `pypomes_http-0.1.4/src/pypomes_http/http_statuses.py`

 * *Files identical despite different names*

### Comparing `pypomes_http-0.1.3/LICENSE` & `pypomes_http-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_http-0.1.3/pyproject.toml` & `pypomes_http-0.1.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_http"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (HTTP modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "Flask>=3.0.2",
     "pip>=24.0",
-    "pypomes_core>=0.8.3",
+    "pypomes_core>=0.8.7",
     "pypomes_security>=0.1.3",
     "requests>=2.31.0",
     "setuptools>=68.0.0",
     "wheel>=0.42.0"
 ]
 
 [project.urls]
```

### Comparing `pypomes_http-0.1.3/PKG-INFO` & `pypomes_http-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.3
 Name: pypomes_http
-Version: 0.1.3
+Version: 0.1.4
 Summary: A collection of Python pomes, pennyeach (HTTP modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-HTTP
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-HTTP/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: flask>=3.0.2
 Requires-Dist: pip>=24.0
-Requires-Dist: pypomes-core>=0.8.3
+Requires-Dist: pypomes-core>=0.8.7
 Requires-Dist: pypomes-security>=0.1.3
 Requires-Dist: requests>=2.31.0
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: wheel>=0.42.0
```

