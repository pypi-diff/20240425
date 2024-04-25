# Comparing `tmp/lsrestclient-1.5.2.tar.gz` & `tmp/lsrestclient-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsrestclient-1.5.2.tar", max compression
+gzip compressed data, was "lsrestclient-2.0.0.tar", max compression
```

## Comparing `lsrestclient-1.5.2.tar` & `lsrestclient-2.0.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     6181 2023-07-26 06:33:28.812862 lsrestclient-1.5.2/README.md
--rw-r--r--   0        0        0       72 2023-08-23 12:32:03.526743 lsrestclient-1.5.2/lsrestclient/__init__.py
--rw-r--r--   0        0        0      468 2023-10-12 07:47:24.090818 lsrestclient-1.5.2/lsrestclient/auth.py
--rw-r--r--   0        0        0    11094 2023-11-14 11:03:19.738747 lsrestclient-1.5.2/lsrestclient/client.py
--rw-r--r--   0        0        0        0 2023-08-23 13:30:32.939048 lsrestclient-1.5.2/lsrestclient/contexts/__init__.py
--rw-r--r--   0        0        0      753 2023-08-23 13:30:32.939048 lsrestclient-1.5.2/lsrestclient/contexts/bearer_token.py
--rw-r--r--   0        0        0     2105 2023-10-11 14:06:13.142464 lsrestclient-1.5.2/lsrestclient/exceptions.py
--rw-r--r--   0        0        0      239 2023-10-11 13:08:57.366081 lsrestclient-1.5.2/lsrestclient/fixtures.py
--rw-r--r--   0        0        0     1213 2023-10-11 13:56:48.875942 lsrestclient-1.5.2/lsrestclient/mock.py
--rw-r--r--   0        0        0     1923 2023-11-21 15:24:01.294987 lsrestclient-1.5.2/lsrestclient/response.py
--rw-r--r--   0        0        0      872 2023-11-21 15:39:51.721769 lsrestclient-1.5.2/pyproject.toml
--rw-r--r--   0        0        0     6656 1970-01-01 00:00:00.000000 lsrestclient-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0     6181 2023-07-25 09:41:02.649481 lsrestclient-2.0.0/README.md
+-rw-r--r--   0        0        0       72 2023-07-27 14:36:50.038756 lsrestclient-2.0.0/lsrestclient/__init__.py
+-rw-r--r--   0        0        0      468 2023-10-13 13:20:34.663834 lsrestclient-2.0.0/lsrestclient/auth.py
+-rw-r--r--   0        0        0    11159 2024-04-08 13:43:39.869341 lsrestclient-2.0.0/lsrestclient/client.py
+-rw-r--r--   0        0        0        0 2023-08-23 13:22:18.238446 lsrestclient-2.0.0/lsrestclient/contexts/__init__.py
+-rw-r--r--   0        0        0      753 2023-08-23 13:22:18.238446 lsrestclient-2.0.0/lsrestclient/contexts/bearer_token.py
+-rw-r--r--   0        0        0     2197 2024-04-25 08:10:43.168133 lsrestclient-2.0.0/lsrestclient/exceptions.py
+-rw-r--r--   0        0        0      239 2023-10-11 08:49:21.282413 lsrestclient-2.0.0/lsrestclient/fixtures.py
+-rw-r--r--   0        0        0     1376 2024-04-25 08:10:43.176133 lsrestclient-2.0.0/lsrestclient/mock.py
+-rw-r--r--   0        0        0     1923 2024-04-08 14:47:34.966071 lsrestclient-2.0.0/lsrestclient/response.py
+-rw-r--r--   0        0        0      871 2024-04-25 08:11:39.083721 lsrestclient-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6748 1970-01-01 00:00:00.000000 lsrestclient-2.0.0/PKG-INFO
```

### Comparing `lsrestclient-1.5.2/README.md` & `lsrestclient-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `lsrestclient-1.5.2/lsrestclient/client.py` & `lsrestclient-2.0.0/lsrestclient/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
         name: str = "default",
     ) -> None:
         """Class representing a REST client for JSON API."""
 
         self._mocks = {}
         self.base_url = base_url
         self.base_headers = {"content-type": "application/json"}
+        self.base_kwargs = {}
         self.name = name
         super().__init__()
         self._clients[name] = self
 
     @staticmethod
     def mock_name(client_name: str, method: str, url: str) -> str:
         return f"{client_name}_{method.upper()}_{url}"
@@ -160,14 +161,15 @@
         # apply base_headers
 
         with bearer_token_context() as bearer_token:
             bearer_headers = {"Authorization": f"Bearer {bearer_token}"} if bearer_token is not None else {}
 
         headers = self.base_headers | bearer_headers | kwargs.get("headers", {})
 
+        kwargs |= self.base_kwargs
         kwargs |= dict(headers=headers)
 
         # params
         if params is None:
             params = {}
         if body is not None:
             kwargs["data"] = lsjsonclasses.LSoftJSONEncoder.dumps(body).encode("utf8")
```

### Comparing `lsrestclient-1.5.2/lsrestclient/contexts/bearer_token.py` & `lsrestclient-2.0.0/lsrestclient/contexts/bearer_token.py`

 * *Files identical despite different names*

### Comparing `lsrestclient-1.5.2/lsrestclient/exceptions.py` & `lsrestclient-2.0.0/lsrestclient/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import contextlib
+import logging
 from typing import Optional, List, Type
 
 import pydash
 from webexception.webexception import WebException
-import logging
 
 log = logging.getLogger(__name__)
 
 
 # noinspection PyShadowingBuiltins
 class ConnectionError(Exception):
     """Exception class for connection errors.
@@ -39,16 +39,20 @@
         self.url = url
         self.status_code = status_code
         self.content = content
         super().__init__(f"Downstream error calling {self.url}. {self.status_code} {self.content}")
 
 
 @contextlib.contextmanager
-def raise_errors(r, exceptions: List[Type[Exception]]):
-    exceptions_by_class = {e.__name__: e for e in exceptions}
+def raise_errors(r, exceptions: Optional[List[Type[Exception]]] = None):
+    if exceptions is None:
+        exceptions_by_class = {}
+    else:
+        exceptions_by_class = {e.__name__: e for e in exceptions}
+
     if r.status_code < 399:
         yield r
     else:
         try:
             json = r.json()
             detail = pydash.get(json, "detail", json)
             error_class = pydash.get(detail, "error_class", None)
```

### Comparing `lsrestclient-1.5.2/lsrestclient/response.py` & `lsrestclient-2.0.0/lsrestclient/response.py`

 * *Files identical despite different names*

### Comparing `lsrestclient-1.5.2/pyproject.toml` & `lsrestclient-2.0.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "lsrestclient"
-version = "1.5.2"
+version = "2.0.0"
 description = "REST Api Client"
 authors = ["mba <bartel@electronic-shop.lu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.9"
 requests = "^2.31.0"
-lsjsonclasses = "^2.0.0"
-pydash = "^7.0.6"
-webexception = "^1.0.4"
+lsjsonclasses = "^2.0.1"
+pydash = ">4.0.0"
+webexception = "^1.0.5"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 black = "^23.7.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `lsrestclient-1.5.2/PKG-INFO` & `lsrestclient-2.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: lsrestclient
-Version: 1.5.2
+Version: 2.0.0
 Summary: REST Api Client
 Author: mba
 Author-email: bartel@electronic-shop.lu
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: lsjsonclasses (>=2.0.0,<3.0.0)
-Requires-Dist: pydash (>=7.0.6,<8.0.0)
+Requires-Dist: lsjsonclasses (>=2.0.1,<3.0.0)
+Requires-Dist: pydash (>4.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: webexception (>=1.0.4,<2.0.0)
+Requires-Dist: webexception (>=1.0.5,<2.0.0)
 Description-Content-Type: text/markdown
 
 # lsrestclient
 
 
 
 ## Getting started
```

