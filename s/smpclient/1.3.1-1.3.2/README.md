# Comparing `tmp/smpclient-1.3.1.tar.gz` & `tmp/smpclient-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smpclient-1.3.1.tar", max compression
+gzip compressed data, was "smpclient-1.3.2.tar", max compression
```

## Comparing `smpclient-1.3.1.tar` & `smpclient-1.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11421 2024-03-18 22:57:41.112363 smpclient-1.3.1/LICENSE
--rw-r--r--   0        0        0     2433 2024-03-18 22:57:41.112363 smpclient-1.3.1/README.md
--rw-r--r--   0        0        0     1081 2024-03-18 22:57:41.112363 smpclient-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     6022 2024-03-18 22:57:41.112363 smpclient-1.3.1/smpclient/__init__.py
--rw-r--r--   0        0        0      188 2024-03-18 22:57:41.112363 smpclient-1.3.1/smpclient/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-18 22:57:41.112363 smpclient-1.3.1/smpclient/extensions/__init__.py
--rw-r--r--   0        0        0     2489 2024-03-18 22:57:41.112363 smpclient-1.3.1/smpclient/extensions/intercreate.py
--rw-r--r--   0        0        0     2750 2024-03-18 22:57:41.112363 smpclient-1.3.1/smpclient/generics.py
--rw-r--r--   0        0        0     8285 2024-03-18 22:57:41.112363 smpclient-1.3.1/smpclient/mcuboot.py
--rw-r--r--   0        0        0        0 2024-03-18 22:57:41.112363 smpclient-1.3.1/smpclient/py.typed
--rw-r--r--   0        0        0        0 2024-03-18 22:57:41.112363 smpclient-1.3.1/smpclient/requests/__init__.py
--rw-r--r--   0        0        0      808 2024-03-18 22:57:41.112363 smpclient-1.3.1/smpclient/requests/image_management.py
--rw-r--r--   0        0        0      599 2024-03-18 22:57:41.112363 smpclient-1.3.1/smpclient/requests/os_management.py
--rw-r--r--   0        0        0      529 2024-03-18 22:57:41.112363 smpclient-1.3.1/smpclient/requests/shell_management.py
--rw-r--r--   0        0        0        0 2024-03-18 22:57:41.112363 smpclient-1.3.1/smpclient/requests/user/__init__.py
--rw-r--r--   0        0        0      457 2024-03-18 22:57:41.112363 smpclient-1.3.1/smpclient/requests/user/intercreate.py
--rw-r--r--   0        0        0     1048 2024-03-18 22:57:41.112363 smpclient-1.3.1/smpclient/transport/__init__.py
--rw-r--r--   0        0        0     5537 2024-03-18 22:57:41.112363 smpclient-1.3.1/smpclient/transport/ble.py
--rw-r--r--   0        0        0     9514 2024-03-18 22:57:41.112363 smpclient-1.3.1/smpclient/transport/serial.py
--rw-r--r--   0        0        0     3137 1970-01-01 00:00:00.000000 smpclient-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11421 2024-04-24 23:33:42.875688 smpclient-1.3.2/LICENSE
+-rw-r--r--   0        0        0     2433 2024-04-24 23:33:42.875688 smpclient-1.3.2/README.md
+-rw-r--r--   0        0        0     1081 2024-04-24 23:33:42.875688 smpclient-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     6022 2024-04-24 23:33:42.875688 smpclient-1.3.2/smpclient/__init__.py
+-rw-r--r--   0        0        0      188 2024-04-24 23:33:42.875688 smpclient-1.3.2/smpclient/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-24 23:33:42.879688 smpclient-1.3.2/smpclient/extensions/__init__.py
+-rw-r--r--   0        0        0     2489 2024-04-24 23:33:42.879688 smpclient-1.3.2/smpclient/extensions/intercreate.py
+-rw-r--r--   0        0        0     2750 2024-04-24 23:33:42.879688 smpclient-1.3.2/smpclient/generics.py
+-rw-r--r--   0        0        0     8285 2024-04-24 23:33:42.879688 smpclient-1.3.2/smpclient/mcuboot.py
+-rw-r--r--   0        0        0        0 2024-04-24 23:33:42.879688 smpclient-1.3.2/smpclient/py.typed
+-rw-r--r--   0        0        0        0 2024-04-24 23:33:42.879688 smpclient-1.3.2/smpclient/requests/__init__.py
+-rw-r--r--   0        0        0      808 2024-04-24 23:33:42.879688 smpclient-1.3.2/smpclient/requests/image_management.py
+-rw-r--r--   0        0        0      599 2024-04-24 23:33:42.879688 smpclient-1.3.2/smpclient/requests/os_management.py
+-rw-r--r--   0        0        0      529 2024-04-24 23:33:42.879688 smpclient-1.3.2/smpclient/requests/shell_management.py
+-rw-r--r--   0        0        0        0 2024-04-24 23:33:42.879688 smpclient-1.3.2/smpclient/requests/user/__init__.py
+-rw-r--r--   0        0        0      457 2024-04-24 23:33:42.879688 smpclient-1.3.2/smpclient/requests/user/intercreate.py
+-rw-r--r--   0        0        0     1048 2024-04-24 23:33:42.879688 smpclient-1.3.2/smpclient/transport/__init__.py
+-rw-r--r--   0        0        0     5537 2024-04-24 23:33:42.879688 smpclient-1.3.2/smpclient/transport/ble.py
+-rw-r--r--   0        0        0     9514 2024-04-24 23:33:42.879688 smpclient-1.3.2/smpclient/transport/serial.py
+-rw-r--r--   0        0        0     3137 1970-01-01 00:00:00.000000 smpclient-1.3.2/PKG-INFO
```

### Comparing `smpclient-1.3.1/LICENSE` & `smpclient-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `smpclient-1.3.1/README.md` & `smpclient-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `smpclient-1.3.1/pyproject.toml` & `smpclient-1.3.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 [tool.poetry-version-plugin]
 source = "git-tag"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <3.13"
 pyserial = "^3.5"
-smp = "^0.3.3"
+smp = "^0.3.4"
 intelhex = "^2.3.0"
 bleak = "^0.21.1"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.3"
 pytest-cov = "^4.1.0"
```

### Comparing `smpclient-1.3.1/smpclient/__init__.py` & `smpclient-1.3.2/smpclient/__init__.py`

 * *Files identical despite different names*

### Comparing `smpclient-1.3.1/smpclient/extensions/intercreate.py` & `smpclient-1.3.2/smpclient/extensions/intercreate.py`

 * *Files identical despite different names*

### Comparing `smpclient-1.3.1/smpclient/generics.py` & `smpclient-1.3.2/smpclient/generics.py`

 * *Files identical despite different names*

### Comparing `smpclient-1.3.1/smpclient/mcuboot.py` & `smpclient-1.3.2/smpclient/mcuboot.py`

 * *Files identical despite different names*

### Comparing `smpclient-1.3.1/smpclient/requests/image_management.py` & `smpclient-1.3.2/smpclient/requests/image_management.py`

 * *Files identical despite different names*

### Comparing `smpclient-1.3.1/smpclient/requests/os_management.py` & `smpclient-1.3.2/smpclient/requests/os_management.py`

 * *Files identical despite different names*

### Comparing `smpclient-1.3.1/smpclient/requests/shell_management.py` & `smpclient-1.3.2/smpclient/requests/shell_management.py`

 * *Files identical despite different names*

### Comparing `smpclient-1.3.1/smpclient/transport/__init__.py` & `smpclient-1.3.2/smpclient/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `smpclient-1.3.1/smpclient/transport/ble.py` & `smpclient-1.3.2/smpclient/transport/ble.py`

 * *Files identical despite different names*

### Comparing `smpclient-1.3.1/smpclient/transport/serial.py` & `smpclient-1.3.2/smpclient/transport/serial.py`

 * *Files identical despite different names*

### Comparing `smpclient-1.3.1/PKG-INFO` & `smpclient-1.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: smpclient
-Version: 1.3.1
+Version: 1.3.2
 Summary: Simple Management Protocol (SMP) Client for remotely managing MCU firmware
 License: Apache-2.0
 Author: J.P. Hutchins
 Author-email: jphutchins@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: bleak (>=0.21.1,<0.22.0)
 Requires-Dist: intelhex (>=2.3.0,<3.0.0)
 Requires-Dist: pyserial (>=3.5,<4.0)
-Requires-Dist: smp (>=0.3.3,<0.4.0)
+Requires-Dist: smp (>=0.3.4,<0.4.0)
 Description-Content-Type: text/markdown
 
 # Simple Management Protocol (SMP) Client 
 
 `smpclient` implements the transport layer of the Simple Management Protocol.  This library can be
 used as a dependency in applications that use SMP over **serial (UART or USB)**, **Bluetooth (BLE)**,
 or **UDP** connections.  Some abstractions are provided for common routines like upgrading device
```

