# Comparing `tmp/fdk-0.1.71.tar.gz` & `tmp/fdk-0.1.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fdk-0.1.71.tar", last modified: Wed Mar 27 10:43:51 2024, max compression
+gzip compressed data, was "fdk-0.1.72.tar", last modified: Thu Apr 25 09:37:14 2024, max compression
```

## Comparing `fdk-0.1.71.tar` & `fdk-0.1.72.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 10:43:51.923651 fdk-0.1.71/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 10:43:51.909651 fdk-0.1.71/.eggs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 10:43:51.909651 fdk-0.1.71/.eggs/pbr-6.0.0-py3.11.egg/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 10:43:51.909651 fdk-0.1.71/.eggs/pbr-6.0.0-py3.11.egg/pbr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 10:43:51.909651 fdk-0.1.71/.eggs/pbr-6.0.0-py3.11.egg/pbr/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 10:43:51.913651 fdk-0.1.71/.eggs/pbr-6.0.0-py3.11.egg/pbr/tests/testpackage/
--rw-rw-r--   0 root         (0) root         (0)       48 2024-03-27 10:43:51.000000 fdk-0.1.71/.eggs/pbr-6.0.0-py3.11.egg/pbr/tests/testpackage/test-requirements.txt
--rw-r--r--   0 root         (0) root         (0)    11357 2024-03-27 10:41:08.000000 fdk-0.1.71/LICENSE
--rw-r--r--   0 root         (0) root         (0)      140 2024-03-27 10:41:08.000000 fdk-0.1.71/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      985 2024-03-27 10:41:08.000000 fdk-0.1.71/NOTICE.txt
--rw-r--r--   0 root         (0) root         (0)      748 2024-03-27 10:43:51.923651 fdk-0.1.71/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14588 2024-03-27 10:41:08.000000 fdk-0.1.71/README.md
--rw-r--r--   0 root         (0) root         (0)   105344 2024-03-27 10:41:08.000000 fdk-0.1.71/THIRD_PARTY_LICENSES.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 10:43:51.916651 fdk-0.1.71/fdk/
--rw-r--r--   0 root         (0) root         (0)     4154 2024-03-27 10:41:08.000000 fdk-0.1.71/fdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 10:43:51.920651 fdk-0.1.71/fdk/async_http/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-27 10:41:08.000000 fdk-0.1.71/fdk/async_http/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4034 2024-03-27 10:41:08.000000 fdk-0.1.71/fdk/async_http/app.py
--rw-r--r--   0 root         (0) root         (0)     4686 2024-03-27 10:41:08.000000 fdk-0.1.71/fdk/async_http/error_handler.py
--rw-r--r--   0 root         (0) root         (0)    11798 2024-03-27 10:41:08.000000 fdk-0.1.71/fdk/async_http/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    20459 2024-03-27 10:41:08.000000 fdk-0.1.71/fdk/async_http/protocol.py
--rw-r--r--   0 root         (0) root         (0)     4381 2024-03-27 10:41:08.000000 fdk-0.1.71/fdk/async_http/request.py
--rw-r--r--   0 root         (0) root         (0)    11148 2024-03-27 10:41:08.000000 fdk-0.1.71/fdk/async_http/response.py
--rw-r--r--   0 root         (0) root         (0)     1756 2024-03-27 10:41:08.000000 fdk-0.1.71/fdk/async_http/router.py
--rw-r--r--   0 root         (0) root         (0)     6771 2024-03-27 10:41:08.000000 fdk-0.1.71/fdk/async_http/server.py
--rw-r--r--   0 root         (0) root         (0)     2117 2024-03-27 10:41:08.000000 fdk-0.1.71/fdk/constants.py
--rw-r--r--   0 root         (0) root         (0)    11375 2024-03-27 10:41:08.000000 fdk-0.1.71/fdk/context.py
--rw-r--r--   0 root         (0) root         (0)     2810 2024-03-27 10:41:08.000000 fdk-0.1.71/fdk/customer_code.py
--rw-r--r--   0 root         (0) root         (0)     1290 2024-03-27 10:41:08.000000 fdk-0.1.71/fdk/errors.py
--rw-r--r--   0 root         (0) root         (0)     2316 2024-03-27 10:41:08.000000 fdk-0.1.71/fdk/event_handler.py
--rw-r--r--   0 root         (0) root         (0)     2807 2024-03-27 10:41:08.000000 fdk-0.1.71/fdk/fixtures.py
--rw-r--r--   0 root         (0) root         (0)     2773 2024-03-27 10:41:08.000000 fdk-0.1.71/fdk/headers.py
--rw-r--r--   0 root         (0) root         (0)     1880 2024-03-27 10:41:08.000000 fdk-0.1.71/fdk/log.py
--rw-r--r--   0 root         (0) root         (0)     2415 2024-03-27 10:41:08.000000 fdk-0.1.71/fdk/response.py
--rw-r--r--   0 root         (0) root         (0)     3349 2024-03-27 10:41:08.000000 fdk-0.1.71/fdk/runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 10:43:51.921651 fdk-0.1.71/fdk/scripts/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-27 10:41:08.000000 fdk-0.1.71/fdk/scripts/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1160 2024-03-27 10:41:08.000000 fdk-0.1.71/fdk/scripts/fdk.py
--rw-r--r--   0 root         (0) root         (0)     1228 2024-03-27 10:41:08.000000 fdk-0.1.71/fdk/scripts/fdk_tcp_debug.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 10:43:51.923651 fdk-0.1.71/fdk/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-27 10:41:08.000000 fdk-0.1.71/fdk/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3537 2024-03-27 10:41:08.000000 fdk-0.1.71/fdk/tests/funcs.py
--rw-r--r--   0 root         (0) root         (0)     1657 2024-03-27 10:41:08.000000 fdk-0.1.71/fdk/tests/tcp_debug.py
--rw-r--r--   0 root         (0) root         (0)     1638 2024-03-27 10:41:08.000000 fdk-0.1.71/fdk/tests/test_delayed_loader.py
--rw-r--r--   0 root         (0) root         (0)     4224 2024-03-27 10:41:08.000000 fdk-0.1.71/fdk/tests/test_headers.py
--rw-r--r--   0 root         (0) root         (0)     7037 2024-03-27 10:41:08.000000 fdk-0.1.71/fdk/tests/test_http_stream.py
--rw-r--r--   0 root         (0) root         (0)     1256 2024-03-27 10:41:08.000000 fdk-0.1.71/fdk/tests/test_protocol.py
--rw-r--r--   0 root         (0) root         (0)     5992 2024-03-27 10:41:08.000000 fdk-0.1.71/fdk/tests/test_tracing.py
--rw-r--r--   0 root         (0) root         (0)       19 2024-03-27 10:41:08.000000 fdk-0.1.71/fdk/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 10:43:51.918651 fdk-0.1.71/fdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      748 2024-03-27 10:43:51.000000 fdk-0.1.71/fdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1093 2024-03-27 10:43:51.000000 fdk-0.1.71/fdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-27 10:43:51.000000 fdk-0.1.71/fdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       92 2024-03-27 10:43:51.000000 fdk-0.1.71/fdk.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-27 10:43:51.000000 fdk-0.1.71/fdk.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      141 2024-03-27 10:43:51.000000 fdk-0.1.71/fdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2024-03-27 10:43:51.000000 fdk-0.1.71/fdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      137 2024-03-27 10:41:08.000000 fdk-0.1.71/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      889 2024-03-27 10:43:51.923651 fdk-0.1.71/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      851 2024-03-27 10:41:08.000000 fdk-0.1.71/setup.py
--rw-r--r--   0 root         (0) root         (0)      106 2024-03-27 10:41:08.000000 fdk-0.1.71/test-requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 09:37:14.933568 fdk-0.1.72/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 09:37:14.919568 fdk-0.1.72/.eggs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 09:37:14.919568 fdk-0.1.72/.eggs/pbr-6.0.0-py3.11.egg/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 09:37:14.919568 fdk-0.1.72/.eggs/pbr-6.0.0-py3.11.egg/pbr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 09:37:14.920568 fdk-0.1.72/.eggs/pbr-6.0.0-py3.11.egg/pbr/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 09:37:14.923568 fdk-0.1.72/.eggs/pbr-6.0.0-py3.11.egg/pbr/tests/testpackage/
+-rw-rw-r--   0 root         (0) root         (0)       48 2024-04-25 09:37:14.000000 fdk-0.1.72/.eggs/pbr-6.0.0-py3.11.egg/pbr/tests/testpackage/test-requirements.txt
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-04-25 09:33:15.000000 fdk-0.1.72/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      140 2024-04-25 09:33:15.000000 fdk-0.1.72/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      985 2024-04-25 09:33:15.000000 fdk-0.1.72/NOTICE.txt
+-rw-r--r--   0 root         (0) root         (0)      748 2024-04-25 09:37:14.933568 fdk-0.1.72/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14588 2024-04-25 09:33:15.000000 fdk-0.1.72/README.md
+-rw-r--r--   0 root         (0) root         (0)   105344 2024-04-25 09:33:15.000000 fdk-0.1.72/THIRD_PARTY_LICENSES.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 09:37:14.926568 fdk-0.1.72/fdk/
+-rw-r--r--   0 root         (0) root         (0)     4154 2024-04-25 09:33:15.000000 fdk-0.1.72/fdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 09:37:14.930568 fdk-0.1.72/fdk/async_http/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 09:33:15.000000 fdk-0.1.72/fdk/async_http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4034 2024-04-25 09:33:15.000000 fdk-0.1.72/fdk/async_http/app.py
+-rw-r--r--   0 root         (0) root         (0)     4686 2024-04-25 09:33:15.000000 fdk-0.1.72/fdk/async_http/error_handler.py
+-rw-r--r--   0 root         (0) root         (0)    11798 2024-04-25 09:33:15.000000 fdk-0.1.72/fdk/async_http/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    20459 2024-04-25 09:33:15.000000 fdk-0.1.72/fdk/async_http/protocol.py
+-rw-r--r--   0 root         (0) root         (0)     4381 2024-04-25 09:33:15.000000 fdk-0.1.72/fdk/async_http/request.py
+-rw-r--r--   0 root         (0) root         (0)    11148 2024-04-25 09:33:15.000000 fdk-0.1.72/fdk/async_http/response.py
+-rw-r--r--   0 root         (0) root         (0)     1756 2024-04-25 09:33:15.000000 fdk-0.1.72/fdk/async_http/router.py
+-rw-r--r--   0 root         (0) root         (0)     6771 2024-04-25 09:33:15.000000 fdk-0.1.72/fdk/async_http/server.py
+-rw-r--r--   0 root         (0) root         (0)     2117 2024-04-25 09:33:15.000000 fdk-0.1.72/fdk/constants.py
+-rw-r--r--   0 root         (0) root         (0)    11375 2024-04-25 09:33:15.000000 fdk-0.1.72/fdk/context.py
+-rw-r--r--   0 root         (0) root         (0)     2810 2024-04-25 09:33:15.000000 fdk-0.1.72/fdk/customer_code.py
+-rw-r--r--   0 root         (0) root         (0)     1290 2024-04-25 09:33:15.000000 fdk-0.1.72/fdk/errors.py
+-rw-r--r--   0 root         (0) root         (0)     2316 2024-04-25 09:33:15.000000 fdk-0.1.72/fdk/event_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2807 2024-04-25 09:33:15.000000 fdk-0.1.72/fdk/fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     2773 2024-04-25 09:33:15.000000 fdk-0.1.72/fdk/headers.py
+-rw-r--r--   0 root         (0) root         (0)     1880 2024-04-25 09:33:15.000000 fdk-0.1.72/fdk/log.py
+-rw-r--r--   0 root         (0) root         (0)     2415 2024-04-25 09:33:15.000000 fdk-0.1.72/fdk/response.py
+-rw-r--r--   0 root         (0) root         (0)     3349 2024-04-25 09:33:15.000000 fdk-0.1.72/fdk/runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 09:37:14.931568 fdk-0.1.72/fdk/scripts/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 09:33:15.000000 fdk-0.1.72/fdk/scripts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2024-04-25 09:33:15.000000 fdk-0.1.72/fdk/scripts/fdk.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2024-04-25 09:33:15.000000 fdk-0.1.72/fdk/scripts/fdk_tcp_debug.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 09:37:14.933568 fdk-0.1.72/fdk/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 09:33:15.000000 fdk-0.1.72/fdk/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3537 2024-04-25 09:33:15.000000 fdk-0.1.72/fdk/tests/funcs.py
+-rw-r--r--   0 root         (0) root         (0)     1657 2024-04-25 09:33:15.000000 fdk-0.1.72/fdk/tests/tcp_debug.py
+-rw-r--r--   0 root         (0) root         (0)     1638 2024-04-25 09:33:15.000000 fdk-0.1.72/fdk/tests/test_delayed_loader.py
+-rw-r--r--   0 root         (0) root         (0)     4224 2024-04-25 09:33:15.000000 fdk-0.1.72/fdk/tests/test_headers.py
+-rw-r--r--   0 root         (0) root         (0)     7037 2024-04-25 09:33:15.000000 fdk-0.1.72/fdk/tests/test_http_stream.py
+-rw-r--r--   0 root         (0) root         (0)     1256 2024-04-25 09:33:15.000000 fdk-0.1.72/fdk/tests/test_protocol.py
+-rw-r--r--   0 root         (0) root         (0)     5992 2024-04-25 09:33:15.000000 fdk-0.1.72/fdk/tests/test_tracing.py
+-rw-r--r--   0 root         (0) root         (0)       19 2024-04-25 09:33:15.000000 fdk-0.1.72/fdk/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 09:37:14.927568 fdk-0.1.72/fdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      748 2024-04-25 09:37:14.000000 fdk-0.1.72/fdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1093 2024-04-25 09:37:14.000000 fdk-0.1.72/fdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 09:37:14.000000 fdk-0.1.72/fdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2024-04-25 09:37:14.000000 fdk-0.1.72/fdk.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 09:37:14.000000 fdk-0.1.72/fdk.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      141 2024-04-25 09:37:14.000000 fdk-0.1.72/fdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2024-04-25 09:37:14.000000 fdk-0.1.72/fdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      137 2024-04-25 09:33:15.000000 fdk-0.1.72/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      889 2024-04-25 09:37:14.933568 fdk-0.1.72/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      851 2024-04-25 09:33:15.000000 fdk-0.1.72/setup.py
+-rw-r--r--   0 root         (0) root         (0)      106 2024-04-25 09:33:15.000000 fdk-0.1.72/test-requirements.txt
```

### Comparing `fdk-0.1.71/LICENSE` & `fdk-0.1.72/LICENSE`

 * *Files identical despite different names*

### Comparing `fdk-0.1.71/NOTICE.txt` & `fdk-0.1.72/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `fdk-0.1.71/PKG-INFO` & `fdk-0.1.72/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdk
-Version: 0.1.71
+Version: 0.1.72
 Summary: Function Developer Kit for Python
 Home-page: https://fnproject.github.io
 Author: Denis Makogon
 Author-email: denys.makogon@oracle.com
 License: Apache License 2.0
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
```

### Comparing `fdk-0.1.71/README.md` & `fdk-0.1.72/README.md`

 * *Files identical despite different names*

### Comparing `fdk-0.1.71/THIRD_PARTY_LICENSES.txt` & `fdk-0.1.72/THIRD_PARTY_LICENSES.txt`

 * *Files identical despite different names*

### Comparing `fdk-0.1.71/fdk/__init__.py` & `fdk-0.1.72/fdk/__init__.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.71/fdk/async_http/app.py` & `fdk-0.1.72/fdk/async_http/app.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.71/fdk/async_http/error_handler.py` & `fdk-0.1.72/fdk/async_http/error_handler.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.71/fdk/async_http/exceptions.py` & `fdk-0.1.72/fdk/async_http/exceptions.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.71/fdk/async_http/protocol.py` & `fdk-0.1.72/fdk/async_http/protocol.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.71/fdk/async_http/request.py` & `fdk-0.1.72/fdk/async_http/request.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.71/fdk/async_http/response.py` & `fdk-0.1.72/fdk/async_http/response.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.71/fdk/async_http/router.py` & `fdk-0.1.72/fdk/async_http/router.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.71/fdk/async_http/server.py` & `fdk-0.1.72/fdk/async_http/server.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.71/fdk/constants.py` & `fdk-0.1.72/fdk/constants.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.71/fdk/context.py` & `fdk-0.1.72/fdk/context.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.71/fdk/customer_code.py` & `fdk-0.1.72/fdk/customer_code.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.71/fdk/errors.py` & `fdk-0.1.72/fdk/errors.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.71/fdk/event_handler.py` & `fdk-0.1.72/fdk/event_handler.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.71/fdk/fixtures.py` & `fdk-0.1.72/fdk/fixtures.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.71/fdk/headers.py` & `fdk-0.1.72/fdk/headers.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.71/fdk/log.py` & `fdk-0.1.72/fdk/log.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.71/fdk/response.py` & `fdk-0.1.72/fdk/response.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.71/fdk/runner.py` & `fdk-0.1.72/fdk/runner.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.71/fdk/scripts/fdk.py` & `fdk-0.1.72/fdk/scripts/fdk.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.71/fdk/scripts/fdk_tcp_debug.py` & `fdk-0.1.72/fdk/scripts/fdk_tcp_debug.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.71/fdk/tests/funcs.py` & `fdk-0.1.72/fdk/tests/funcs.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.71/fdk/tests/tcp_debug.py` & `fdk-0.1.72/fdk/tests/tcp_debug.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.71/fdk/tests/test_delayed_loader.py` & `fdk-0.1.72/fdk/tests/test_delayed_loader.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.71/fdk/tests/test_headers.py` & `fdk-0.1.72/fdk/tests/test_headers.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.71/fdk/tests/test_http_stream.py` & `fdk-0.1.72/fdk/tests/test_http_stream.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.71/fdk/tests/test_protocol.py` & `fdk-0.1.72/fdk/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.71/fdk/tests/test_tracing.py` & `fdk-0.1.72/fdk/tests/test_tracing.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.71/fdk.egg-info/PKG-INFO` & `fdk-0.1.72/fdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdk
-Version: 0.1.71
+Version: 0.1.72
 Summary: Function Developer Kit for Python
 Home-page: https://fnproject.github.io
 Author: Denis Makogon
 Author-email: denys.makogon@oracle.com
 License: Apache License 2.0
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
```

### Comparing `fdk-0.1.71/fdk.egg-info/SOURCES.txt` & `fdk-0.1.72/fdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fdk-0.1.71/setup.cfg` & `fdk-0.1.72/setup.cfg`

 * *Files identical despite different names*

### Comparing `fdk-0.1.71/setup.py` & `fdk-0.1.72/setup.py`

 * *Files identical despite different names*

