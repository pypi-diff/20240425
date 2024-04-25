# Comparing `tmp/aioxmlrpc-0.8.0.tar.gz` & `tmp/aioxmlrpc-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioxmlrpc-0.8.0.tar", max compression
+gzip compressed data, was "aioxmlrpc-0.8.1.tar", max compression
```

## Comparing `aioxmlrpc-0.8.0.tar` & `aioxmlrpc-0.8.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1525 2022-06-02 06:43:48.349040 aioxmlrpc-0.8.0/LICENSE
--rw-r--r--   0        0        0     1464 2023-05-08 09:36:16.556811 aioxmlrpc-0.8.0/README.rst
--rw-r--r--   0        0        0      579 2024-04-09 20:57:38.065005 aioxmlrpc-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      129 2022-06-02 06:43:48.352373 aioxmlrpc-0.8.0/src/aioxmlrpc/__init__.py
--rw-r--r--   0        0        0     4844 2023-05-08 09:47:19.208644 aioxmlrpc-0.8.0/src/aioxmlrpc/client.py
--rw-r--r--   0        0        0     2283 1970-01-01 00:00:00.000000 aioxmlrpc-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1525 2022-06-02 06:43:48.349040 aioxmlrpc-0.8.1/LICENSE
+-rw-r--r--   0        0        0     1464 2023-05-08 09:36:16.556811 aioxmlrpc-0.8.1/README.rst
+-rw-r--r--   0        0        0      671 2024-04-25 15:40:40.925074 aioxmlrpc-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0      129 2022-06-02 06:43:48.352373 aioxmlrpc-0.8.1/src/aioxmlrpc/__init__.py
+-rw-r--r--   0        0        0     4844 2023-05-08 09:47:19.208644 aioxmlrpc-0.8.1/src/aioxmlrpc/client.py
+-rw-r--r--   0        0        0     2283 1970-01-01 00:00:00.000000 aioxmlrpc-0.8.1/PKG-INFO
```

### Comparing `aioxmlrpc-0.8.0/LICENSE` & `aioxmlrpc-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aioxmlrpc-0.8.0/README.rst` & `aioxmlrpc-0.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `aioxmlrpc-0.8.0/src/aioxmlrpc/client.py` & `aioxmlrpc-0.8.1/src/aioxmlrpc/client.py`

 * *Files identical despite different names*

### Comparing `aioxmlrpc-0.8.0/PKG-INFO` & `aioxmlrpc-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioxmlrpc
-Version: 0.8.0
+Version: 0.8.1
 Summary: XML-RPC client for asyncio
 Home-page: https://github.com/mardiros/aioxmlrpc
 License: BSD-3-Clause License
 Author: Guillaume Gauvrit
 Author-email: guillaume@gauvr.it
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
```

