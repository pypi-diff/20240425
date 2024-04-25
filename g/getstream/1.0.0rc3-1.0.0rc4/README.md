# Comparing `tmp/getstream-1.0.0rc3.tar.gz` & `tmp/getstream-1.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getstream-1.0.0rc3.tar", max compression
+gzip compressed data, was "getstream-1.0.0rc4.tar", max compression
```

## Comparing `getstream-1.0.0rc3.tar` & `getstream-1.0.0rc4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    14205 2024-04-25 14:47:11.022843 getstream-1.0.0rc3/LICENSE.md
--rw-r--r--   0        0        0     3154 2024-04-25 14:47:11.022843 getstream-1.0.0rc3/README.md
--rw-r--r--   0        0        0       50 2024-04-25 14:47:11.022843 getstream-1.0.0rc3/getstream/__init__.py
--rw-r--r--   0        0        0     6264 2024-04-25 14:47:11.022843 getstream-1.0.0rc3/getstream/base.py
--rw-r--r--   0        0        0        0 2024-04-25 14:47:11.026843 getstream-1.0.0rc3/getstream/chat/__init__.py
--rw-r--r--   0        0        0       24 2024-04-25 14:47:11.026843 getstream-1.0.0rc3/getstream/chat/channel.py
--rw-r--r--   0        0        0      267 2024-04-25 14:47:11.026843 getstream-1.0.0rc3/getstream/chat/client.py
--rw-r--r--   0        0        0    48047 2024-04-25 14:47:11.026843 getstream-1.0.0rc3/getstream/chat/rest_client.py
--rw-r--r--   0        0        0        0 2024-04-25 14:47:11.026843 getstream-1.0.0rc3/getstream/common/__init__.py
--rw-r--r--   0        0        0      275 2024-04-25 14:47:11.026843 getstream-1.0.0rc3/getstream/common/client.py
--rw-r--r--   0        0        0    16612 2024-04-25 14:47:11.026843 getstream-1.0.0rc3/getstream/common/rest_client.py
--rw-r--r--   0        0        0      925 2024-04-25 14:47:11.026843 getstream-1.0.0rc3/getstream/config.py
--rw-r--r--   0        0        0       46 2024-04-25 14:47:11.026843 getstream-1.0.0rc3/getstream/generic.py
--rw-r--r--   0        0        0      497 2024-04-25 14:47:11.026843 getstream-1.0.0rc3/getstream/meta.py
--rw-r--r--   0        0        0   297290 2024-04-25 14:47:11.026843 getstream-1.0.0rc3/getstream/models/__init__.py
--rw-r--r--   0        0        0     1168 2024-04-25 14:47:11.026843 getstream-1.0.0rc3/getstream/rate_limit.py
--rw-r--r--   0        0        0     4061 2024-04-25 14:47:11.026843 getstream-1.0.0rc3/getstream/stream.py
--rw-r--r--   0        0        0     1024 2024-04-25 14:47:11.026843 getstream-1.0.0rc3/getstream/stream_response.py
--rw-r--r--   0        0        0     4057 2024-04-25 14:47:11.026843 getstream-1.0.0rc3/getstream/utils.py
--rw-r--r--   0        0        0       22 2024-04-25 14:47:11.026843 getstream-1.0.0rc3/getstream/version.py
--rw-r--r--   0        0        0        0 2024-04-25 14:47:11.026843 getstream-1.0.0rc3/getstream/video/__init__.py
--rw-r--r--   0        0        0     9640 2024-04-25 14:47:11.026843 getstream-1.0.0rc3/getstream/video/call.py
--rw-r--r--   0        0        0      817 2024-04-25 14:47:11.026843 getstream-1.0.0rc3/getstream/video/client.py
--rw-r--r--   0        0        0    20228 2024-04-25 14:47:11.026843 getstream-1.0.0rc3/getstream/video/rest_client.py
--rw-r--r--   0        0        0      682 2024-04-25 14:47:11.026843 getstream-1.0.0rc3/pyproject.toml
--rw-r--r--   0        0        0     3864 1970-01-01 00:00:00.000000 getstream-1.0.0rc3/PKG-INFO
+-rw-r--r--   0        0        0    14205 2024-04-25 14:31:22.776641 getstream-1.0.0rc4/LICENSE.md
+-rw-r--r--   0        0        0     3154 2024-04-25 14:31:22.776641 getstream-1.0.0rc4/README.md
+-rw-r--r--   0        0        0       50 2024-04-25 14:31:22.776641 getstream-1.0.0rc4/getstream/__init__.py
+-rw-r--r--   0        0        0     6264 2024-04-25 14:31:22.776641 getstream-1.0.0rc4/getstream/base.py
+-rw-r--r--   0        0        0        0 2024-04-25 14:31:22.776641 getstream-1.0.0rc4/getstream/chat/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-25 14:31:22.776641 getstream-1.0.0rc4/getstream/chat/channel.py
+-rw-r--r--   0        0        0      267 2024-04-25 14:31:22.776641 getstream-1.0.0rc4/getstream/chat/client.py
+-rw-r--r--   0        0        0    48047 2024-04-25 14:31:22.776641 getstream-1.0.0rc4/getstream/chat/rest_client.py
+-rw-r--r--   0        0        0        0 2024-04-25 14:31:22.776641 getstream-1.0.0rc4/getstream/common/__init__.py
+-rw-r--r--   0        0        0      275 2024-04-25 14:31:22.776641 getstream-1.0.0rc4/getstream/common/client.py
+-rw-r--r--   0        0        0    16612 2024-04-25 14:31:22.776641 getstream-1.0.0rc4/getstream/common/rest_client.py
+-rw-r--r--   0        0        0      925 2024-04-25 14:31:22.776641 getstream-1.0.0rc4/getstream/config.py
+-rw-r--r--   0        0        0       46 2024-04-25 14:31:22.776641 getstream-1.0.0rc4/getstream/generic.py
+-rw-r--r--   0        0        0      497 2024-04-25 14:31:22.776641 getstream-1.0.0rc4/getstream/meta.py
+-rw-r--r--   0        0        0   297290 2024-04-25 14:31:22.776641 getstream-1.0.0rc4/getstream/models/__init__.py
+-rw-r--r--   0        0        0     1168 2024-04-25 14:31:22.776641 getstream-1.0.0rc4/getstream/rate_limit.py
+-rw-r--r--   0        0        0     4061 2024-04-25 14:31:22.776641 getstream-1.0.0rc4/getstream/stream.py
+-rw-r--r--   0        0        0     1024 2024-04-25 14:31:22.780641 getstream-1.0.0rc4/getstream/stream_response.py
+-rw-r--r--   0        0        0     4057 2024-04-25 14:31:22.780641 getstream-1.0.0rc4/getstream/utils.py
+-rw-r--r--   0        0        0       22 2024-04-25 14:31:22.780641 getstream-1.0.0rc4/getstream/version.py
+-rw-r--r--   0        0        0        0 2024-04-25 14:31:22.780641 getstream-1.0.0rc4/getstream/video/__init__.py
+-rw-r--r--   0        0        0     9640 2024-04-25 14:31:22.780641 getstream-1.0.0rc4/getstream/video/call.py
+-rw-r--r--   0        0        0      817 2024-04-25 14:31:22.780641 getstream-1.0.0rc4/getstream/video/client.py
+-rw-r--r--   0        0        0    20228 2024-04-25 14:31:22.780641 getstream-1.0.0rc4/getstream/video/rest_client.py
+-rw-r--r--   0        0        0      682 2024-04-25 14:31:22.780641 getstream-1.0.0rc4/pyproject.toml
+-rw-r--r--   0        0        0     3864 1970-01-01 00:00:00.000000 getstream-1.0.0rc4/PKG-INFO
```

### Comparing `getstream-1.0.0rc3/LICENSE.md` & `getstream-1.0.0rc4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `getstream-1.0.0rc3/README.md` & `getstream-1.0.0rc4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Official Python SDK for [Stream](https://getstream.io/)
 
-[![build](https://github.com/GetStream/stream-py/actions/workflows/ci.yml/badge.svg)](https://github.com/GetStream/stream-py/actions) [![PyPI version](https://badge.fury.io/py/getstream.svg)](http://badge.fury.io/py/getstream) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/getstream.svg)
+[![build](https://github.com/GetStream/stream-py/workflows/build/badge.svg)](https://github.com/GetStream/stream-chat-python/actions) [![PyPI version](https://badge.fury.io/py/getstream.svg)](http://badge.fury.io/py/getstream) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/getstream.svg)
 
 ## Features
 
 - Video call creation and management
 - Chat session creation and management
 - Token generation for user authentication
```

### Comparing `getstream-1.0.0rc3/getstream/base.py` & `getstream-1.0.0rc4/getstream/base.py`

 * *Files identical despite different names*

### Comparing `getstream-1.0.0rc3/getstream/chat/rest_client.py` & `getstream-1.0.0rc4/getstream/chat/rest_client.py`

 * *Files identical despite different names*

### Comparing `getstream-1.0.0rc3/getstream/common/rest_client.py` & `getstream-1.0.0rc4/getstream/common/rest_client.py`

 * *Files identical despite different names*

### Comparing `getstream-1.0.0rc3/getstream/config.py` & `getstream-1.0.0rc4/getstream/config.py`

 * *Files identical despite different names*

### Comparing `getstream-1.0.0rc3/getstream/models/__init__.py` & `getstream-1.0.0rc4/getstream/models/__init__.py`

 * *Files identical despite different names*

### Comparing `getstream-1.0.0rc3/getstream/rate_limit.py` & `getstream-1.0.0rc4/getstream/rate_limit.py`

 * *Files identical despite different names*

### Comparing `getstream-1.0.0rc3/getstream/stream.py` & `getstream-1.0.0rc4/getstream/stream.py`

 * *Files identical despite different names*

### Comparing `getstream-1.0.0rc3/getstream/stream_response.py` & `getstream-1.0.0rc4/getstream/stream_response.py`

 * *Files identical despite different names*

### Comparing `getstream-1.0.0rc3/getstream/utils.py` & `getstream-1.0.0rc4/getstream/utils.py`

 * *Files identical despite different names*

### Comparing `getstream-1.0.0rc3/getstream/video/call.py` & `getstream-1.0.0rc4/getstream/video/call.py`

 * *Files identical despite different names*

### Comparing `getstream-1.0.0rc3/getstream/video/client.py` & `getstream-1.0.0rc4/getstream/video/client.py`

 * *Files identical despite different names*

### Comparing `getstream-1.0.0rc3/getstream/video/rest_client.py` & `getstream-1.0.0rc4/getstream/video/rest_client.py`

 * *Files identical despite different names*

### Comparing `getstream-1.0.0rc3/PKG-INFO` & `getstream-1.0.0rc4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getstream
-Version: 1.0.0rc3
+Version: 1.0.0rc4
 Summary: 
 Author: sachaarbonel
 Author-email: sacha.arbonel@hotmail.fr
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -16,15 +16,15 @@
 Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
 Requires-Dist: urllib3 (>=1.26.17,<2.0.0)
 Requires-Dist: validators (>=0.28.1,<0.29.0)
 Description-Content-Type: text/markdown
 
 # Official Python SDK for [Stream](https://getstream.io/)
 
-[![build](https://github.com/GetStream/stream-py/actions/workflows/ci.yml/badge.svg)](https://github.com/GetStream/stream-py/actions) [![PyPI version](https://badge.fury.io/py/getstream.svg)](http://badge.fury.io/py/getstream) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/getstream.svg)
+[![build](https://github.com/GetStream/stream-py/workflows/build/badge.svg)](https://github.com/GetStream/stream-chat-python/actions) [![PyPI version](https://badge.fury.io/py/getstream.svg)](http://badge.fury.io/py/getstream) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/getstream.svg)
 
 ## Features
 
 - Video call creation and management
 - Chat session creation and management
 - Token generation for user authentication
```

