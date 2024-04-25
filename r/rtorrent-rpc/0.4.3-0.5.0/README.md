# Comparing `tmp/rtorrent_rpc-0.4.3.tar.gz` & `tmp/rtorrent_rpc-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtorrent_rpc-0.4.3.tar", max compression
+gzip compressed data, was "rtorrent_rpc-0.5.0.tar", max compression
```

## Comparing `rtorrent_rpc-0.4.3.tar` & `rtorrent_rpc-0.5.0.tar`

### file list

```diff
@@ -1,8 +1,11 @@
--rw-r--r--   0        0        0     1084 2024-04-25 08:48:33.445154 rtorrent_rpc-0.4.3/LICENSE
--rw-r--r--   0        0        0     2419 2024-04-25 08:48:33.445154 rtorrent_rpc-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     1077 2024-04-25 08:48:33.445154 rtorrent_rpc-0.4.3/readme.md
--rw-r--r--   0        0        0    28295 2024-04-25 08:48:33.445154 rtorrent_rpc-0.4.3/rtorrent_rpc/__init__.py
--rw-r--r--   0        0        0     2943 2024-04-25 08:48:33.445154 rtorrent_rpc-0.4.3/rtorrent_rpc/helper.py
--rw-r--r--   0        0        0        0 2024-04-25 08:48:33.445154 rtorrent_rpc-0.4.3/rtorrent_rpc/py.typed
--rw-r--r--   0        0        0     4554 2024-04-25 08:48:33.445154 rtorrent_rpc-0.4.3/rtorrent_rpc/scgi.py
--rw-r--r--   0        0        0     2004 1970-01-01 00:00:00.000000 rtorrent_rpc-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1084 2024-04-25 13:30:24.611627 rtorrent_rpc-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2457 2024-04-25 13:30:24.611627 rtorrent_rpc-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1406 2024-04-25 13:30:24.611627 rtorrent_rpc-0.5.0/readme.md
+-rw-r--r--   0        0        0    29423 2024-04-25 13:30:24.611627 rtorrent_rpc-0.5.0/rtorrent_rpc/__init__.py
+-rw-r--r--   0        0        0     2327 2024-04-25 13:30:24.611627 rtorrent_rpc-0.5.0/rtorrent_rpc/_jsonrpc/__init__.py
+-rw-r--r--   0        0        0     3050 2024-04-25 13:30:24.611627 rtorrent_rpc-0.5.0/rtorrent_rpc/_jsonrpc/transport.py
+-rw-r--r--   0        0        0     1235 2024-04-25 13:30:24.611627 rtorrent_rpc-0.5.0/rtorrent_rpc/_scgi.py
+-rw-r--r--   0        0        0      803 2024-04-25 13:30:24.611627 rtorrent_rpc-0.5.0/rtorrent_rpc/_transport.py
+-rw-r--r--   0        0        0     2943 2024-04-25 13:30:24.611627 rtorrent_rpc-0.5.0/rtorrent_rpc/helper.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:30:24.611627 rtorrent_rpc-0.5.0/rtorrent_rpc/py.typed
+-rw-r--r--   0        0        0     2373 1970-01-01 00:00:00.000000 rtorrent_rpc-0.5.0/PKG-INFO
```

### Comparing `rtorrent_rpc-0.4.3/LICENSE` & `rtorrent_rpc-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.4.3/pyproject.toml` & `rtorrent_rpc-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "rtorrent-rpc"
-version = "0.4.3"
+version = "0.5.0"
 description = "Typed rtorrent rpc client"
 authors = ["Trim21 <i@trim21.me>"]
 readme = 'readme.md'
 repository = 'https://github.com/trim21/rtorrent-rpc'
 license = 'MIT'
 packages = [{ include = 'rtorrent_rpc' }]
 keywords = ['rtorrent', 'rpc']
@@ -20,14 +20,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 # dependencies
 typing-extensions = ">=4.7.1"
 bencode2 = ">=0.0.6,<1"
+urllib3 = "^2.2.1"
 
 [tool.poetry.group.docs.dependencies]
 sphinx = { version = "^7.0.0", python = "^3.9" }
 furo = { version = "^2024.0.0", python = "^3.9" }
 
 [tool.poetry.group.dev.dependencies]
 # tests
@@ -36,14 +37,15 @@
 coverage = "==7.5.0"
 
 # linter and formatter
 pre-commit = { version = "==3.7.0", markers = "implementation_name != 'pypy'", python = "^3.9" }
 #mypy = { version = "==1.4.1", markers = "implementation_name != 'pypy'", python = "^3.9" }
 sphinx-autobuild = { version = "2024.4.16", python = "^3.9" }
 mypy = { version = "1.10.0", python = "^3.9" }
+orjson = "^3.10.1"
 
 [tool.poetry-plugin-bump]
 commit_msg = 'bump: v{version}'
 
 [tool.pytest.ini_options]
 addopts = '-rav -Werror'
```

### Comparing `rtorrent_rpc-0.4.3/readme.md` & `rtorrent_rpc-0.5.0/readme.md`

 * *Files 8% similar despite different names*

```diff
@@ -25,13 +25,21 @@
 
 client = RTorrent(address='scgi://127.0.0.1:5000')
 unix_client = RTorrent(address='scgi:///home/ubuntu/.local/share/rtorrent.sock')
 ```
 
 ## Known problem:
 
-rTorrent's xmlrpc doesn't support emoji. If torrent name of file name contains any emoji,
+rTorrent's [xmlrpc do not support all utf8 characters](https://github.com/rakshasa/rtorrent/issues/1250), for example, emoji.
+
+If torrent name of file name contains any emoji,
 you can't retrieve correct torrent name of file name through xmlrpc.
 
+Please consider use a rtorrent distro with json-rpc support,
+for example: [jesec/rtorrent](https://github.com/jesec/rtorrent)
+
+If your rtorrent distro support jsonrpc,
+you can use send json-rpc request with `RTorrent(...).jsonrpc.call(...)`.
+
 ## License
 
 `rtorrent-rpc` is licensed under the MIT license.
```

### Comparing `rtorrent_rpc-0.4.3/rtorrent_rpc/__init__.py` & `rtorrent_rpc-0.5.0/rtorrent_rpc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 from __future__ import annotations
 
 import time
+import urllib
 import urllib.parse
 import xmlrpc.client
 from collections.abc import Iterable
 from typing import Any, Literal, Protocol
 from urllib.parse import quote
 
 import bencode2
 from typing_extensions import NotRequired, TypeAlias, TypedDict
 
-from .scgi import SCGIServerProxy
-
-__all__ = ["RTorrent", "MultiCall", "RutorrentCompatibilityDisabledError"]
+from rtorrent_rpc._jsonrpc import JSONRpc, JSONRpcError
+from rtorrent_rpc._jsonrpc.transport import BadStatusError
+from rtorrent_rpc._transport import SsciXmlTransport
+
+__all__ = [
+    "RTorrent",
+    "MultiCall",
+    "RutorrentCompatibilityDisabledError",
+    "BadStatusError",
+    "JSONRpcError",
+]
 
 Unknown: TypeAlias = Any
 
 
 class RutorrentCompatibilityDisabledError(Exception):
     def __init__(self) -> None:
         super().__init__("you need enable ruTorrent compatibility to use this feature")
@@ -117,22 +126,25 @@
     you can use ``rt.rpc`` for direct rpc call.
 
     :param address: rtorrent rpc address
     :param rutorrent_compatibility: compatibility for ruTorrent or flood.
     """
 
     rpc: xmlrpc.client.ServerProxy
+    jsonrpc: JSONRpc
 
     def __init__(self, address: str, rutorrent_compatibility: bool = True):
         u = urllib.parse.urlparse(address)
         if u.scheme == "scgi":
             self.rpc = SCGIServerProxy(address)
         else:
             self.rpc = xmlrpc.client.ServerProxy(address)
 
+        self.jsonrpc = JSONRpc(address=address)
+
         self.rutorrent_compatibility: bool = rutorrent_compatibility
 
     def get_session_path(self) -> str:
         """get current rtorrent session path"""
         return self.rpc.session.path()  # type: ignore
 
     def add_torrent_by_file(
@@ -1046,7 +1058,36 @@
     "d.session_file",
     "cfg.scrape_interval.active",
     "cfg.scrape_interval.active.set",
     "cfg.scrape_interval.idle",
     "cfg.scrape_interval.idle.set",
     "d.last_scrape.send_set",
 ]
+
+
+class SCGIServerProxy(xmlrpc.client.ServerProxy):
+    def __init__(
+        self,
+        uri: str,
+        transport: xmlrpc.client.Transport | None = None,
+        use_datetime: bool = False,
+        use_builtin_types: bool = False,
+        **kwargs: Any,
+    ):
+        u = urllib.parse.urlparse(uri)
+
+        if u.scheme != "scgi":
+            raise OSError("SCGIServerProxy Only Support XML-RPC over SCGI protocol")
+
+        if transport is None:
+            transport = SsciXmlTransport(
+                use_datetime=use_datetime,
+                address=uri,
+                use_builtin_types=use_builtin_types,
+            )
+
+        # Feed some junk in here, but we'll fix it afterwards
+        super().__init__(
+            urllib.parse.urlunparse(u._replace(scheme="http")),
+            transport=transport,
+            **kwargs,
+        )
```

### Comparing `rtorrent_rpc-0.4.3/rtorrent_rpc/helper.py` & `rtorrent_rpc-0.5.0/rtorrent_rpc/helper.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.4.3/PKG-INFO` & `rtorrent_rpc-0.5.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtorrent-rpc
-Version: 0.4.3
+Version: 0.5.0
 Summary: Typed rtorrent rpc client
 Home-page: https://github.com/trim21/rtorrent-rpc
 License: MIT
 Keywords: rtorrent,rpc
 Author: Trim21
 Author-email: i@trim21.me
 Requires-Python: >=3.8,<4.0
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: bencode2 (>=0.0.6,<1)
 Requires-Dist: typing-extensions (>=4.7.1)
+Requires-Dist: urllib3 (>=2.2.1,<3.0.0)
 Project-URL: Repository, https://github.com/trim21/rtorrent-rpc
 Description-Content-Type: text/markdown
 
 # Typed rtorrent rpc client
 
 [![PyPI](https://img.shields.io/pypi/v/rtorrent-rpc)](https://pypi.org/project/rtorrent-rpc/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rtorrent-rpc)](https://pypi.org/project/rtorrent-rpc/)
@@ -50,14 +51,22 @@
 
 client = RTorrent(address='scgi://127.0.0.1:5000')
 unix_client = RTorrent(address='scgi:///home/ubuntu/.local/share/rtorrent.sock')
 ```
 
 ## Known problem:
 
-rTorrent's xmlrpc doesn't support emoji. If torrent name of file name contains any emoji,
+rTorrent's [xmlrpc do not support all utf8 characters](https://github.com/rakshasa/rtorrent/issues/1250), for example, emoji.
+
+If torrent name of file name contains any emoji,
 you can't retrieve correct torrent name of file name through xmlrpc.
 
+Please consider use a rtorrent distro with json-rpc support,
+for example: [jesec/rtorrent](https://github.com/jesec/rtorrent)
+
+If your rtorrent distro support jsonrpc,
+you can use send json-rpc request with `RTorrent(...).jsonrpc.call(...)`.
+
 ## License
 
 `rtorrent-rpc` is licensed under the MIT license.
```

