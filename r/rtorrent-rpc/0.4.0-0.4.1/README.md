# Comparing `tmp/rtorrent_rpc-0.4.0.tar.gz` & `tmp/rtorrent_rpc-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtorrent_rpc-0.4.0.tar", max compression
+gzip compressed data, was "rtorrent_rpc-0.4.1.tar", max compression
```

## Comparing `rtorrent_rpc-0.4.0.tar` & `rtorrent_rpc-0.4.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1084 2024-04-24 16:59:40.890687 rtorrent_rpc-0.4.0/LICENSE
--rw-r--r--   0        0        0     2433 2024-04-24 16:59:40.890687 rtorrent_rpc-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1077 2024-04-24 16:59:40.890687 rtorrent_rpc-0.4.0/readme.md
--rw-r--r--   0        0        0    28294 2024-04-24 16:59:40.890687 rtorrent_rpc-0.4.0/rtorrent_rpc/__init__.py
--rw-r--r--   0        0        0     2934 2024-04-24 16:59:40.890687 rtorrent_rpc-0.4.0/rtorrent_rpc/helper.py
--rw-r--r--   0        0        0        0 2024-04-24 16:59:40.890687 rtorrent_rpc-0.4.0/rtorrent_rpc/py.typed
--rw-r--r--   0        0        0     3925 2024-04-24 16:59:40.890687 rtorrent_rpc-0.4.0/rtorrent_rpc/scgi.py
--rw-r--r--   0        0        0     2004 1970-01-01 00:00:00.000000 rtorrent_rpc-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2024-04-24 19:23:35.074561 rtorrent_rpc-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2433 2024-04-24 19:23:35.074561 rtorrent_rpc-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1077 2024-04-24 19:23:35.074561 rtorrent_rpc-0.4.1/readme.md
+-rw-r--r--   0        0        0    28294 2024-04-24 19:23:35.074561 rtorrent_rpc-0.4.1/rtorrent_rpc/__init__.py
+-rw-r--r--   0        0        0     2943 2024-04-24 19:23:35.074561 rtorrent_rpc-0.4.1/rtorrent_rpc/helper.py
+-rw-r--r--   0        0        0        0 2024-04-24 19:23:35.074561 rtorrent_rpc-0.4.1/rtorrent_rpc/py.typed
+-rw-r--r--   0        0        0     3925 2024-04-24 19:23:35.074561 rtorrent_rpc-0.4.1/rtorrent_rpc/scgi.py
+-rw-r--r--   0        0        0     2004 1970-01-01 00:00:00.000000 rtorrent_rpc-0.4.1/PKG-INFO
```

### Comparing `rtorrent_rpc-0.4.0/LICENSE` & `rtorrent_rpc-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.4.0/pyproject.toml` & `rtorrent_rpc-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "rtorrent-rpc"
-version = "0.4.0"
+version = "0.4.1"
 description = "Typed rtorrent rpc client"
 authors = ["Trim21 <i@trim21.me>"]
 readme = 'readme.md'
 repository = 'https://github.com/trim21/rtorrent-rpc'
 license = 'MIT'
 packages = [{ include = 'rtorrent_rpc' }]
 keywords = ['rtorrent', 'rpc']
```

### Comparing `rtorrent_rpc-0.4.0/readme.md` & `rtorrent_rpc-0.4.1/readme.md`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.4.0/rtorrent_rpc/__init__.py` & `rtorrent_rpc-0.4.1/rtorrent_rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.4.0/rtorrent_rpc/helper.py` & `rtorrent_rpc-0.4.1/rtorrent_rpc/helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 def parse_tags(s: str) -> set[str]:
     """ruTorrent compatibility method to parse ``d.custom1`` as tags"""
     tags = set()
     for t in s.split(","):
         tt = t.strip()
         if tt:
-            tags.add(tt)
+            tags.add(unquote(tt))
     return tags
 
 
 if sys.version_info >= (3, 9):
 
     def __remove_prefix(s: str, prefix: str) -> str:
         return s.removeprefix(prefix)
```

### Comparing `rtorrent_rpc-0.4.0/rtorrent_rpc/scgi.py` & `rtorrent_rpc-0.4.1/rtorrent_rpc/scgi.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.4.0/PKG-INFO` & `rtorrent_rpc-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtorrent-rpc
-Version: 0.4.0
+Version: 0.4.1
 Summary: Typed rtorrent rpc client
 Home-page: https://github.com/trim21/rtorrent-rpc
 License: MIT
 Keywords: rtorrent,rpc
 Author: Trim21
 Author-email: i@trim21.me
 Requires-Python: >=3.8,<4.0
```

