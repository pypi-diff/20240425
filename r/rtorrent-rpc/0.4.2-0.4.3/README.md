# Comparing `tmp/rtorrent_rpc-0.4.2.tar.gz` & `tmp/rtorrent_rpc-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtorrent_rpc-0.4.2.tar", max compression
+gzip compressed data, was "rtorrent_rpc-0.4.3.tar", max compression
```

## Comparing `rtorrent_rpc-0.4.2.tar` & `rtorrent_rpc-0.4.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1084 2024-04-25 08:36:18.387944 rtorrent_rpc-0.4.2/LICENSE
--rw-r--r--   0        0        0     2419 2024-04-25 08:36:18.387944 rtorrent_rpc-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     1077 2024-04-25 08:36:18.387944 rtorrent_rpc-0.4.2/readme.md
--rw-r--r--   0        0        0    28294 2024-04-25 08:36:18.387944 rtorrent_rpc-0.4.2/rtorrent_rpc/__init__.py
--rw-r--r--   0        0        0     2943 2024-04-25 08:36:18.387944 rtorrent_rpc-0.4.2/rtorrent_rpc/helper.py
--rw-r--r--   0        0        0        0 2024-04-25 08:36:18.387944 rtorrent_rpc-0.4.2/rtorrent_rpc/py.typed
--rw-r--r--   0        0        0     4554 2024-04-25 08:36:18.387944 rtorrent_rpc-0.4.2/rtorrent_rpc/scgi.py
--rw-r--r--   0        0        0     2004 1970-01-01 00:00:00.000000 rtorrent_rpc-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1084 2024-04-25 08:48:33.445154 rtorrent_rpc-0.4.3/LICENSE
+-rw-r--r--   0        0        0     2419 2024-04-25 08:48:33.445154 rtorrent_rpc-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     1077 2024-04-25 08:48:33.445154 rtorrent_rpc-0.4.3/readme.md
+-rw-r--r--   0        0        0    28295 2024-04-25 08:48:33.445154 rtorrent_rpc-0.4.3/rtorrent_rpc/__init__.py
+-rw-r--r--   0        0        0     2943 2024-04-25 08:48:33.445154 rtorrent_rpc-0.4.3/rtorrent_rpc/helper.py
+-rw-r--r--   0        0        0        0 2024-04-25 08:48:33.445154 rtorrent_rpc-0.4.3/rtorrent_rpc/py.typed
+-rw-r--r--   0        0        0     4554 2024-04-25 08:48:33.445154 rtorrent_rpc-0.4.3/rtorrent_rpc/scgi.py
+-rw-r--r--   0        0        0     2004 1970-01-01 00:00:00.000000 rtorrent_rpc-0.4.3/PKG-INFO
```

### Comparing `rtorrent_rpc-0.4.2/LICENSE` & `rtorrent_rpc-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.4.2/pyproject.toml` & `rtorrent_rpc-0.4.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "rtorrent-rpc"
-version = "0.4.2"
+version = "0.4.3"
 description = "Typed rtorrent rpc client"
 authors = ["Trim21 <i@trim21.me>"]
 readme = 'readme.md'
 repository = 'https://github.com/trim21/rtorrent-rpc'
 license = 'MIT'
 packages = [{ include = 'rtorrent_rpc' }]
 keywords = ['rtorrent', 'rpc']
```

### Comparing `rtorrent_rpc-0.4.2/readme.md` & `rtorrent_rpc-0.4.3/readme.md`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.4.2/rtorrent_rpc/__init__.py` & `rtorrent_rpc-0.4.3/rtorrent_rpc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
         if tags:
             if not self.rutorrent_compatibility:
                 raise RutorrentCompatibilityDisabledError
             params.append(f'd.custom1.set="{_encode_tags(tags)}"')
 
         if self.rutorrent_compatibility:
             t = bencode2.bdecode(content)
-            if "comment" in t:
+            if b"comment" in t:
                 params.append(
                     f'd.custom2.set="VRS24mrker{quote(t[b"comment"].decode().strip())}"'
                 )
 
         self.rpc.load.raw_start_verbose(*params)  # type: ignore
 
     def stop_torrent(self, info_hash: str) -> None:
```

### Comparing `rtorrent_rpc-0.4.2/rtorrent_rpc/helper.py` & `rtorrent_rpc-0.4.3/rtorrent_rpc/helper.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.4.2/rtorrent_rpc/scgi.py` & `rtorrent_rpc-0.4.3/rtorrent_rpc/scgi.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.4.2/PKG-INFO` & `rtorrent_rpc-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtorrent-rpc
-Version: 0.4.2
+Version: 0.4.3
 Summary: Typed rtorrent rpc client
 Home-page: https://github.com/trim21/rtorrent-rpc
 License: MIT
 Keywords: rtorrent,rpc
 Author: Trim21
 Author-email: i@trim21.me
 Requires-Python: >=3.8,<4.0
```

