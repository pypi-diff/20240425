# Comparing `tmp/mure-1.0.0b1.tar.gz` & `tmp/mure-1.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mure-1.0.0b1.tar", max compression
+gzip compressed data, was "mure-1.0.0b3.tar", max compression
```

## Comparing `mure-1.0.0b1.tar` & `mure-1.0.0b3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11345 2024-04-25 12:32:55.563618 mure-1.0.0b1/LICENSE
--rw-r--r--   0        0        0     5557 2024-04-25 12:32:55.563618 mure-1.0.0b1/README.md
--rw-r--r--   0        0        0      212 2024-04-25 12:32:55.563618 mure-1.0.0b1/mure/__init__.py
--rw-r--r--   0        0        0     3097 2024-04-25 12:32:55.563618 mure-1.0.0b1/mure/cache.py
--rw-r--r--   0        0        0     4419 2024-04-25 12:32:55.563618 mure-1.0.0b1/mure/core.py
--rw-r--r--   0        0        0     9076 2024-04-25 12:32:55.563618 mure-1.0.0b1/mure/iterator.py
--rw-r--r--   0        0        0     4272 2024-04-25 12:32:55.563618 mure-1.0.0b1/mure/logging.py
--rw-r--r--   0        0        0     3874 2024-04-25 12:32:55.563618 mure-1.0.0b1/mure/models.py
--rw-r--r--   0        0        0     2794 2024-04-25 12:32:55.563618 mure-1.0.0b1/pyproject.toml
--rw-r--r--   0        0        0     6072 1970-01-01 00:00:00.000000 mure-1.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0    11345 2024-04-25 12:57:01.777310 mure-1.0.0b3/LICENSE
+-rw-r--r--   0        0        0     5557 2024-04-25 12:57:01.777310 mure-1.0.0b3/README.md
+-rw-r--r--   0        0        0      212 2024-04-25 12:57:01.777310 mure-1.0.0b3/mure/__init__.py
+-rw-r--r--   0        0        0     4264 2024-04-25 12:57:01.777310 mure-1.0.0b3/mure/cache.py
+-rw-r--r--   0        0        0     4419 2024-04-25 12:57:01.777310 mure-1.0.0b3/mure/core.py
+-rw-r--r--   0        0        0     9076 2024-04-25 12:57:01.777310 mure-1.0.0b3/mure/iterator.py
+-rw-r--r--   0        0        0     4272 2024-04-25 12:57:01.777310 mure-1.0.0b3/mure/logging.py
+-rw-r--r--   0        0        0     3463 2024-04-25 12:57:01.777310 mure-1.0.0b3/mure/models.py
+-rw-r--r--   0        0        0     2794 2024-04-25 12:57:01.777310 mure-1.0.0b3/pyproject.toml
+-rw-r--r--   0        0        0     6072 1970-01-01 00:00:00.000000 mure-1.0.0b3/PKG-INFO
```

### Comparing `mure-1.0.0b1/LICENSE` & `mure-1.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `mure-1.0.0b1/README.md` & `mure-1.0.0b3/README.md`

 * *Files identical despite different names*

### Comparing `mure-1.0.0b1/mure/cache.py` & `mure-1.0.0b3/mure/cache.py`

 * *Files 15% similar despite different names*

```diff
@@ -69,52 +69,92 @@
             Request to check if it's in the cache.
 
         Returns
         -------
         bool
             True if the request is in the cache; otherwise, False.
         """
-        return request in self._cache
+        return request.id in self._cache
 
     def get(self, request: Request) -> Response | None:
         """Get the response for the specified request from the cache.
 
         Parameters
         ----------
         request : Request
             Request to get response from the cache.
 
         Returns
         -------
         Response | None
             Response from the cache or None if the request is not in the cache.
         """
-        return self._cache.get(request)
+        return self._cache.get(request.id)
 
     def set(self, request: Request, response: Response):
         """Save a request and its response to the cache.
 
         Parameters
         ----------
         request : Request
             Request to save to the cache.
         response : Response
             Response to save to the cache.
         """
-        self._cache[request] = response
+        self._cache[request.id] = response
 
 
-class DiskCache(MemoryCache):
+class DiskCache(Cache):
     """Simple on-disk cache."""
 
     def __init__(self, path: Path = Path("mure-cache.shelve")):
-        super().__init__()
-
         self.path = path.resolve()
         self._cache = shelve.open(str(self.path))
 
         if self.path.exists():
             LOGGER.warning(f"Cache ({self.path}) already exists")
 
     def __del__(self):
         """Close the cache."""
         self._cache.close()
+
+    def has(self, request: Request) -> bool:
+        """Check if a request (and its corresponding response) is in the cache.
+
+        Parameters
+        ----------
+        request : Request
+            Request to check if it's in the cache.
+
+        Returns
+        -------
+        bool
+            True if the request is in the cache; otherwise, False.
+        """
+        return request.id in self._cache
+
+    def get(self, request: Request) -> Response | None:
+        """Get the response for the specified request from the cache.
+
+        Parameters
+        ----------
+        request : Request
+            Request to get response from the cache.
+
+        Returns
+        -------
+        Response | None
+            Response from the cache or None if the request is not in the cache.
+        """
+        return self._cache.get(request.id)
+
+    def set(self, request: Request, response: Response):
+        """Save a request and its response to the cache.
+
+        Parameters
+        ----------
+        request : Request
+            Request to save to the cache.
+        response : Response
+            Response to save to the cache.
+        """
+        self._cache[request.id] = response
```

### Comparing `mure-1.0.0b1/mure/core.py` & `mure-1.0.0b3/mure/core.py`

 * *Files identical despite different names*

### Comparing `mure-1.0.0b1/mure/iterator.py` & `mure-1.0.0b3/mure/iterator.py`

 * *Files identical despite different names*

### Comparing `mure-1.0.0b1/mure/logging.py` & `mure-1.0.0b3/mure/logging.py`

 * *Files identical despite different names*

### Comparing `mure-1.0.0b1/mure/models.py` & `mure-1.0.0b3/mure/models.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import json
+from functools import cached_property
+from hashlib import blake2b
 from typing import Any, Literal, Mapping, NotRequired, TypedDict
 
 Method = Literal["DELETE", "GET", "HEAD", "PATCH", "POST", "PUT"]
 
 
 class Resource(TypedDict):
     """Resource to request."""
@@ -55,57 +57,36 @@
         self.json = json
         self.timeout = timeout
 
     def __repr__(self) -> str:
         """Return the string representation of the request."""
         return f"<Request({self.method}, {self.url})>"
 
-    def __hash__(self) -> int:
-        """Hash the request."""
-        return hash(
-            (
-                self.method,
-                self.url,
-                json.dumps(self.params, sort_keys=True, ensure_ascii=False).lower(),
-                json.dumps(self.json, sort_keys=True, ensure_ascii=False).lower(),
-                self.data
-                if isinstance(self.data, (str, bytes))
-                else json.dumps(self.data, sort_keys=True, ensure_ascii=False),
-            )
-        )
-
-    def __eq__(self, other: "Request") -> bool:
-        """Check if two requests are equal.
-
-        Parameters
-        ----------
-        other : Request
-            Other request to compare.
+    @cached_property
+    def id(self) -> str:
+        """Return the unique identifier of the request.
 
         Returns
         -------
-        bool
-            True if the requests are equal; otherwise, False.
+        str
+            Unique identifier of the request.
         """
-        return self.__hash__() == other.__hash__()
-
-    def encode(self, encoding: str = "utf-8") -> bytes:
-        """Encode the request.
-
-        Parameters
-        ----------
-        encoding : str, optional
-            Encoding to use, by default "utf-8".
-
-        Returns
-        -------
-        bytes
-            Encoded request.
-        """
-        return str(self.__hash__()).encode(encoding)
+        # TODO this could/should be improved somehow
+        components: list[str] = [
+            self.method,
+            self.url,
+            json.dumps(self.params, sort_keys=True, ensure_ascii=False).lower(),
+            json.dumps(self.json, sort_keys=True, ensure_ascii=False).lower(),
+            json.dumps(self.data, sort_keys=True, ensure_ascii=False).lower(),
+        ]
+
+        key = blake2b(digest_size=8)
+        for component in components:
+            key.update(component.encode("utf-8"))
+        return key.hexdigest()
 
 
 class Response:
     """HTTP response.
 
     Parameters
     ----------
```

### Comparing `mure-1.0.0b1/pyproject.toml` & `mure-1.0.0b3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mure"
-version = "1.0.0b1"
+version = "1.0.0b3"
 description = "Perform multiple HTTP requests concurrently – without worrying about async/await."
 authors = ["Severin Simmler <s.simmler@snapaddy.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 aiohttp = { extras = ["speedups"], version = "^3.8.5" }
```

### Comparing `mure-1.0.0b1/PKG-INFO` & `mure-1.0.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mure
-Version: 1.0.0b1
+Version: 1.0.0b3
 Summary: Perform multiple HTTP requests concurrently – without worrying about async/await.
 Author: Severin Simmler
 Author-email: s.simmler@snapaddy.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

