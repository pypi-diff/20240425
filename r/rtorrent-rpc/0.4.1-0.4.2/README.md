# Comparing `tmp/rtorrent_rpc-0.4.1.tar.gz` & `tmp/rtorrent_rpc-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtorrent_rpc-0.4.1.tar", max compression
+gzip compressed data, was "rtorrent_rpc-0.4.2.tar", max compression
```

## Comparing `rtorrent_rpc-0.4.1.tar` & `rtorrent_rpc-0.4.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1084 2024-04-24 19:23:35.074561 rtorrent_rpc-0.4.1/LICENSE
--rw-r--r--   0        0        0     2433 2024-04-24 19:23:35.074561 rtorrent_rpc-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1077 2024-04-24 19:23:35.074561 rtorrent_rpc-0.4.1/readme.md
--rw-r--r--   0        0        0    28294 2024-04-24 19:23:35.074561 rtorrent_rpc-0.4.1/rtorrent_rpc/__init__.py
--rw-r--r--   0        0        0     2943 2024-04-24 19:23:35.074561 rtorrent_rpc-0.4.1/rtorrent_rpc/helper.py
--rw-r--r--   0        0        0        0 2024-04-24 19:23:35.074561 rtorrent_rpc-0.4.1/rtorrent_rpc/py.typed
--rw-r--r--   0        0        0     3925 2024-04-24 19:23:35.074561 rtorrent_rpc-0.4.1/rtorrent_rpc/scgi.py
--rw-r--r--   0        0        0     2004 1970-01-01 00:00:00.000000 rtorrent_rpc-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2024-04-25 08:36:18.387944 rtorrent_rpc-0.4.2/LICENSE
+-rw-r--r--   0        0        0     2419 2024-04-25 08:36:18.387944 rtorrent_rpc-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1077 2024-04-25 08:36:18.387944 rtorrent_rpc-0.4.2/readme.md
+-rw-r--r--   0        0        0    28294 2024-04-25 08:36:18.387944 rtorrent_rpc-0.4.2/rtorrent_rpc/__init__.py
+-rw-r--r--   0        0        0     2943 2024-04-25 08:36:18.387944 rtorrent_rpc-0.4.2/rtorrent_rpc/helper.py
+-rw-r--r--   0        0        0        0 2024-04-25 08:36:18.387944 rtorrent_rpc-0.4.2/rtorrent_rpc/py.typed
+-rw-r--r--   0        0        0     4554 2024-04-25 08:36:18.387944 rtorrent_rpc-0.4.2/rtorrent_rpc/scgi.py
+-rw-r--r--   0        0        0     2004 1970-01-01 00:00:00.000000 rtorrent_rpc-0.4.2/PKG-INFO
```

### Comparing `rtorrent_rpc-0.4.1/LICENSE` & `rtorrent_rpc-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.4.1/pyproject.toml` & `rtorrent_rpc-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "rtorrent-rpc"
-version = "0.4.1"
+version = "0.4.2"
 description = "Typed rtorrent rpc client"
 authors = ["Trim21 <i@trim21.me>"]
 readme = 'readme.md'
 repository = 'https://github.com/trim21/rtorrent-rpc'
 license = 'MIT'
 packages = [{ include = 'rtorrent_rpc' }]
 keywords = ['rtorrent', 'rpc']
@@ -29,22 +29,21 @@
 sphinx = { version = "^7.0.0", python = "^3.9" }
 furo = { version = "^2024.0.0", python = "^3.9" }
 
 [tool.poetry.group.dev.dependencies]
 # tests
 pytest = "==8.1.1"
 pytest-github-actions-annotate-failures = "==0.2.0"
-coverage = "==7.4.4"
+coverage = "==7.5.0"
 
 # linter and formatter
 pre-commit = { version = "==3.7.0", markers = "implementation_name != 'pypy'", python = "^3.9" }
 #mypy = { version = "==1.4.1", markers = "implementation_name != 'pypy'", python = "^3.9" }
-ruff = "0.3.7"
 sphinx-autobuild = { version = "2024.4.16", python = "^3.9" }
-mypy = { version = "1.9.0", python = "^3.9" }
+mypy = { version = "1.10.0", python = "^3.9" }
 
 [tool.poetry-plugin-bump]
 commit_msg = 'bump: v{version}'
 
 [tool.pytest.ini_options]
 addopts = '-rav -Werror'
```

### Comparing `rtorrent_rpc-0.4.1/readme.md` & `rtorrent_rpc-0.4.2/readme.md`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.4.1/rtorrent_rpc/__init__.py` & `rtorrent_rpc-0.4.2/rtorrent_rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.4.1/rtorrent_rpc/helper.py` & `rtorrent_rpc-0.4.2/rtorrent_rpc/helper.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.4.1/rtorrent_rpc/scgi.py` & `rtorrent_rpc-0.4.2/rtorrent_rpc/scgi.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,55 +7,82 @@
 # Inspired by Glenn Washburn's xmlrpc2scgi.py [1], but subclasses the
 # built-in xmlrpclib classes so that it is compatible with features
 # such as MultiCall objects.
 #
 # [1] <http://libtorrent.rakshasa.no/wiki/UtilsXmlrpc2scgi>
 from __future__ import annotations
 
+import functools
 import socket
 import urllib
 import urllib.parse
 import xmlrpc.client
-from typing import Any
+from typing import Any, Iterator
 
-__all__ = ["SCGITransport", "SCGIServerProxy"]
+__all__ = ["SCGITransport", "SCGIServerProxy", "encode_request", "parse_response"]
 
 NULL = b"\x00"
 
 
+def encode_request(body: bytes, content_type: str | None = None) -> Iterator[bytes]:
+    length = len(body)
+
+    header_items: list[bytes] = [
+        *(b"CONTENT_LENGTH", NULL, str(length).encode(), NULL),
+        *(b"SCGI", NULL, b"1", NULL),
+    ]
+
+    if content_type:
+        header_items.extend((b"CONTENT_TYPE", NULL, content_type.encode(), NULL))
+
+    header_len = sum(len(c) for c in header_items)
+
+    yield str(header_len).encode()
+    yield b":"
+    yield from header_items
+    yield b","
+    yield body
+
+
+def parse_response(res: bytes) -> tuple[dict[str, str], bytes]:
+    """
+    Args:
+        res: should be full response bytes, including headers and body
+    """
+    raw_header, _, body = res.partition(b"\r\n\r\n")
+    h = __parse_raw_headers(raw_header)
+    assert int(h["content-length"].encode()) == len(body)
+    return h, body
+
+
+def __parse_raw_headers(raw: bytes) -> dict[str, str]:
+    lines = raw.split(b"\r\n")
+    d = {}
+    for line in lines:
+        key, value = line.split(b":")
+        key = key.strip()
+        d[key.decode().lower()] = value.strip().decode()
+    return d
+
+
 class SCGITransport(xmlrpc.client.Transport):
     def __init__(self, *args: Any, **kwargs: Any):
         super().__init__(*args, **kwargs)
 
-    def encode_scgi_headers(self, content_length: int) -> bytes:
-        # Need to use an ordered dict because content length MUST be the first
-        #  key present in the encoded headers.
-        headers = {
-            b"CONTENT_LENGTH": str(content_length).encode("utf-8"),
-            b"SCGI": b"1",
-        }
-
-        encoded = NULL.join(k + NULL + v for k, v in headers.items()) + NULL
-        length = str(len(encoded)).encode("utf-8")
-        return length + b":" + encoded
-
     def single_request(
         self,
         host: str | tuple[str, dict[str, str]],
         handler: str,
         request_body: Any,
         verbose: bool = False,
     ) -> Any:
         # Add SCGI headers to the request.
-        header = self.encode_scgi_headers(len(request_body))
-
         with self.__connect(host, handler) as sock:
-            sock.send(header)
-            sock.send(b",")
-            sock.send(request_body)
+            for chunk in encode_request(request_body):
+                sock.send(chunk)
             with sock.makefile(mode="rb", errors="strict") as res:
                 return self._parse_response(res.read(), verbose)
 
     def __connect(
         self,
         host: str | tuple[str, dict[str, str]],
         handler: str,
@@ -69,21 +96,22 @@
             return socket.create_connection((host, port))
         # unix domain socket
         sock = socket.socket(socket.AF_UNIX, socket.SOCK_STREAM)
         sock.connect(handler)
         return sock
 
     def _parse_response(self, response_data: bytes, verbose: bool) -> Any:
-        p, u = self.getparser()
 
-        header, s, body = response_data.partition(b"\r\n\r\n")
+        header, body = parse_response(response_data)
 
         if verbose:
             print("body:", repr(body))
 
+        p, u = self.getparser()
+
         p.feed(body)
         p.close()
 
         return u.close()
 
 
 class SCGIServerProxy(xmlrpc.client.ServerProxy):
@@ -109,14 +137,15 @@
         super().__init__(
             urllib.parse.urlunparse(u._replace(scheme="http")),
             transport=transport,
             **kwargs,
         )
 
 
+@functools.lru_cache
 def splitport(hostport: str) -> tuple[str, int]:
     """
     splitport('host:port') --> 'host', 'port'.
 
     This functionality use to (sort of) be provided by urllib as
      `urllib.splithost` in python2, but has since been removed.
     """
```

### Comparing `rtorrent_rpc-0.4.1/PKG-INFO` & `rtorrent_rpc-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtorrent-rpc
-Version: 0.4.1
+Version: 0.4.2
 Summary: Typed rtorrent rpc client
 Home-page: https://github.com/trim21/rtorrent-rpc
 License: MIT
 Keywords: rtorrent,rpc
 Author: Trim21
 Author-email: i@trim21.me
 Requires-Python: >=3.8,<4.0
```

