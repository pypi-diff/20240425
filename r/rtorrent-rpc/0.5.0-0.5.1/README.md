# Comparing `tmp/rtorrent_rpc-0.5.0.tar.gz` & `tmp/rtorrent_rpc-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtorrent_rpc-0.5.0.tar", max compression
+gzip compressed data, was "rtorrent_rpc-0.5.1.tar", max compression
```

## Comparing `rtorrent_rpc-0.5.0.tar` & `rtorrent_rpc-0.5.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1084 2024-04-25 13:30:24.611627 rtorrent_rpc-0.5.0/LICENSE
--rw-r--r--   0        0        0     2457 2024-04-25 13:30:24.611627 rtorrent_rpc-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1406 2024-04-25 13:30:24.611627 rtorrent_rpc-0.5.0/readme.md
--rw-r--r--   0        0        0    29423 2024-04-25 13:30:24.611627 rtorrent_rpc-0.5.0/rtorrent_rpc/__init__.py
--rw-r--r--   0        0        0     2327 2024-04-25 13:30:24.611627 rtorrent_rpc-0.5.0/rtorrent_rpc/_jsonrpc/__init__.py
--rw-r--r--   0        0        0     3050 2024-04-25 13:30:24.611627 rtorrent_rpc-0.5.0/rtorrent_rpc/_jsonrpc/transport.py
--rw-r--r--   0        0        0     1235 2024-04-25 13:30:24.611627 rtorrent_rpc-0.5.0/rtorrent_rpc/_scgi.py
--rw-r--r--   0        0        0      803 2024-04-25 13:30:24.611627 rtorrent_rpc-0.5.0/rtorrent_rpc/_transport.py
--rw-r--r--   0        0        0     2943 2024-04-25 13:30:24.611627 rtorrent_rpc-0.5.0/rtorrent_rpc/helper.py
--rw-r--r--   0        0        0        0 2024-04-25 13:30:24.611627 rtorrent_rpc-0.5.0/rtorrent_rpc/py.typed
--rw-r--r--   0        0        0     2373 1970-01-01 00:00:00.000000 rtorrent_rpc-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2024-04-25 13:46:34.322564 rtorrent_rpc-0.5.1/LICENSE
+-rw-r--r--   0        0        0     2456 2024-04-25 13:46:34.322564 rtorrent_rpc-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1406 2024-04-25 13:46:34.322564 rtorrent_rpc-0.5.1/readme.md
+-rw-r--r--   0        0        0    29423 2024-04-25 13:46:34.322564 rtorrent_rpc-0.5.1/rtorrent_rpc/__init__.py
+-rw-r--r--   0        0        0     2327 2024-04-25 13:46:34.322564 rtorrent_rpc-0.5.1/rtorrent_rpc/_jsonrpc/__init__.py
+-rw-r--r--   0        0        0     3050 2024-04-25 13:46:34.322564 rtorrent_rpc-0.5.1/rtorrent_rpc/_jsonrpc/transport.py
+-rw-r--r--   0        0        0     1235 2024-04-25 13:46:34.322564 rtorrent_rpc-0.5.1/rtorrent_rpc/_scgi.py
+-rw-r--r--   0        0        0      803 2024-04-25 13:46:34.326564 rtorrent_rpc-0.5.1/rtorrent_rpc/_transport.py
+-rw-r--r--   0        0        0     2943 2024-04-25 13:46:34.326564 rtorrent_rpc-0.5.1/rtorrent_rpc/helper.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:34.326564 rtorrent_rpc-0.5.1/rtorrent_rpc/py.typed
+-rw-r--r--   0        0        0     2373 1970-01-01 00:00:00.000000 rtorrent_rpc-0.5.1/PKG-INFO
```

### Comparing `rtorrent_rpc-0.5.0/LICENSE` & `rtorrent_rpc-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.5.0/pyproject.toml` & `rtorrent_rpc-0.5.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "rtorrent-rpc"
-version = "0.5.0"
+version = "0.5.1"
 description = "Typed rtorrent rpc client"
 authors = ["Trim21 <i@trim21.me>"]
 readme = 'readme.md'
 repository = 'https://github.com/trim21/rtorrent-rpc'
 license = 'MIT'
 packages = [{ include = 'rtorrent_rpc' }]
 keywords = ['rtorrent', 'rpc']
@@ -37,15 +37,15 @@
 coverage = "==7.5.0"
 
 # linter and formatter
 pre-commit = { version = "==3.7.0", markers = "implementation_name != 'pypy'", python = "^3.9" }
 #mypy = { version = "==1.4.1", markers = "implementation_name != 'pypy'", python = "^3.9" }
 sphinx-autobuild = { version = "2024.4.16", python = "^3.9" }
 mypy = { version = "1.10.0", python = "^3.9" }
-orjson = "^3.10.1"
+orjson = "3.10.1"
 
 [tool.poetry-plugin-bump]
 commit_msg = 'bump: v{version}'
 
 [tool.pytest.ini_options]
 addopts = '-rav -Werror'
```

### Comparing `rtorrent_rpc-0.5.0/readme.md` & `rtorrent_rpc-0.5.1/readme.md`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.5.0/rtorrent_rpc/__init__.py` & `rtorrent_rpc-0.5.1/rtorrent_rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.5.0/rtorrent_rpc/_jsonrpc/__init__.py` & `rtorrent_rpc-0.5.1/rtorrent_rpc/_jsonrpc/__init__.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.5.0/rtorrent_rpc/_jsonrpc/transport.py` & `rtorrent_rpc-0.5.1/rtorrent_rpc/_jsonrpc/transport.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.5.0/rtorrent_rpc/_scgi.py` & `rtorrent_rpc-0.5.1/rtorrent_rpc/_scgi.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.5.0/rtorrent_rpc/_transport.py` & `rtorrent_rpc-0.5.1/rtorrent_rpc/_transport.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.5.0/rtorrent_rpc/helper.py` & `rtorrent_rpc-0.5.1/rtorrent_rpc/helper.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.5.0/PKG-INFO` & `rtorrent_rpc-0.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtorrent-rpc
-Version: 0.5.0
+Version: 0.5.1
 Summary: Typed rtorrent rpc client
 Home-page: https://github.com/trim21/rtorrent-rpc
 License: MIT
 Keywords: rtorrent,rpc
 Author: Trim21
 Author-email: i@trim21.me
 Requires-Python: >=3.8,<4.0
```

