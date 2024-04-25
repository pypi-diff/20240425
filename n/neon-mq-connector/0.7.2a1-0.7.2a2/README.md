# Comparing `tmp/neon_mq_connector-0.7.2a1.tar.gz` & `tmp/neon_mq_connector-0.7.2a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon_mq_connector-0.7.2a1.tar", last modified: Sat Mar 30 20:28:36 2024, max compression
+gzip compressed data, was "neon_mq_connector-0.7.2a2.tar", last modified: Thu Apr 25 16:27:09 2024, max compression
```

## Comparing `neon_mq_connector-0.7.2a1.tar` & `neon_mq_connector-0.7.2a2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:28:36.261575 neon_mq_connector-0.7.2a1/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-03-30 20:28:33.000000 neon_mq_connector-0.7.2a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-03-30 20:28:36.261575 neon_mq_connector-0.7.2a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-03-30 20:28:33.000000 neon_mq_connector-0.7.2a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:28:36.257575 neon_mq_connector-0.7.2a1/neon_mq_connector/
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-03-30 20:28:33.000000 neon_mq_connector-0.7.2a1/neon_mq_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-03-30 20:28:33.000000 neon_mq_connector-0.7.2a1/neon_mq_connector/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    33789 2024-03-30 20:28:33.000000 neon_mq_connector-0.7.2a1/neon_mq_connector/connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:28:36.257575 neon_mq_connector-0.7.2a1/neon_mq_connector/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-03-30 20:28:33.000000 neon_mq_connector-0.7.2a1/neon_mq_connector/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6845 2024-03-30 20:28:33.000000 neon_mq_connector-0.7.2a1/neon_mq_connector/utils/client_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7700 2024-03-30 20:28:33.000000 neon_mq_connector-0.7.2a1/neon_mq_connector/utils/connection_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-03-30 20:28:33.000000 neon_mq_connector-0.7.2a1/neon_mq_connector/utils/network_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-03-30 20:28:33.000000 neon_mq_connector-0.7.2a1/neon_mq_connector/utils/rabbit_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-03-30 20:28:33.000000 neon_mq_connector-0.7.2a1/neon_mq_connector/utils/thread_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:28:36.257575 neon_mq_connector-0.7.2a1/neon_mq_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-03-30 20:28:36.000000 neon_mq_connector-0.7.2a1/neon_mq_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-03-30 20:28:36.000000 neon_mq_connector-0.7.2a1/neon_mq_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 20:28:36.000000 neon_mq_connector-0.7.2a1/neon_mq_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-30 20:28:36.000000 neon_mq_connector-0.7.2a1/neon_mq_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-30 20:28:36.000000 neon_mq_connector-0.7.2a1/neon_mq_connector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 20:28:36.000000 neon_mq_connector-0.7.2a1/neon_mq_connector.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 20:28:36.261575 neon_mq_connector-0.7.2a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-03-30 20:28:33.000000 neon_mq_connector-0.7.2a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:27:09.952226 neon_mq_connector-0.7.2a2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-25 16:27:05.000000 neon_mq_connector-0.7.2a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-25 16:27:09.952226 neon_mq_connector-0.7.2a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-25 16:27:05.000000 neon_mq_connector-0.7.2a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:27:09.948226 neon_mq_connector-0.7.2a2/neon_mq_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-25 16:27:05.000000 neon_mq_connector-0.7.2a2/neon_mq_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-04-25 16:27:05.000000 neon_mq_connector-0.7.2a2/neon_mq_connector/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33789 2024-04-25 16:27:05.000000 neon_mq_connector-0.7.2a2/neon_mq_connector/connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:27:09.952226 neon_mq_connector-0.7.2a2/neon_mq_connector/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-25 16:27:05.000000 neon_mq_connector-0.7.2a2/neon_mq_connector/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6845 2024-04-25 16:27:05.000000 neon_mq_connector-0.7.2a2/neon_mq_connector/utils/client_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7700 2024-04-25 16:27:05.000000 neon_mq_connector-0.7.2a2/neon_mq_connector/utils/connection_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-04-25 16:27:05.000000 neon_mq_connector-0.7.2a2/neon_mq_connector/utils/network_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-25 16:27:05.000000 neon_mq_connector-0.7.2a2/neon_mq_connector/utils/rabbit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-25 16:27:05.000000 neon_mq_connector-0.7.2a2/neon_mq_connector/utils/thread_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:27:09.948226 neon_mq_connector-0.7.2a2/neon_mq_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-25 16:27:09.000000 neon_mq_connector-0.7.2a2/neon_mq_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-25 16:27:09.000000 neon_mq_connector-0.7.2a2/neon_mq_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:27:09.000000 neon_mq_connector-0.7.2a2/neon_mq_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-25 16:27:09.000000 neon_mq_connector-0.7.2a2/neon_mq_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 16:27:09.000000 neon_mq_connector-0.7.2a2/neon_mq_connector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:27:09.000000 neon_mq_connector-0.7.2a2/neon_mq_connector.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 16:27:09.952226 neon_mq_connector-0.7.2a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-04-25 16:27:05.000000 neon_mq_connector-0.7.2a2/setup.py
```

### Comparing `neon_mq_connector-0.7.2a1/LICENSE.md` & `neon_mq_connector-0.7.2a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon_mq_connector-0.7.2a1/PKG-INFO` & `neon_mq_connector-0.7.2a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon_mq_connector
-Version: 0.7.2a1
+Version: 0.7.2a2
 Summary: MQ Connector for Neon Modules
 Home-page: https://github.com/NeonGeckoCom/neon_mq_connector
 Author: NeonGecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `neon_mq_connector-0.7.2a1/README.md` & `neon_mq_connector-0.7.2a2/README.md`

 * *Files identical despite different names*

### Comparing `neon_mq_connector-0.7.2a1/neon_mq_connector/__init__.py` & `neon_mq_connector-0.7.2a2/neon_mq_connector/__init__.py`

 * *Files identical despite different names*

### Comparing `neon_mq_connector-0.7.2a1/neon_mq_connector/config.py` & `neon_mq_connector-0.7.2a2/neon_mq_connector/config.py`

 * *Files identical despite different names*

### Comparing `neon_mq_connector-0.7.2a1/neon_mq_connector/connector.py` & `neon_mq_connector-0.7.2a2/neon_mq_connector/connector.py`

 * *Files identical despite different names*

### Comparing `neon_mq_connector-0.7.2a1/neon_mq_connector/utils/__init__.py` & `neon_mq_connector-0.7.2a2/neon_mq_connector/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neon_mq_connector-0.7.2a1/neon_mq_connector/utils/client_utils.py` & `neon_mq_connector-0.7.2a2/neon_mq_connector/utils/client_utils.py`

 * *Files identical despite different names*

### Comparing `neon_mq_connector-0.7.2a1/neon_mq_connector/utils/connection_utils.py` & `neon_mq_connector-0.7.2a2/neon_mq_connector/utils/connection_utils.py`

 * *Files identical despite different names*

### Comparing `neon_mq_connector-0.7.2a1/neon_mq_connector/utils/network_utils.py` & `neon_mq_connector-0.7.2a2/neon_mq_connector/utils/network_utils.py`

 * *Files identical despite different names*

### Comparing `neon_mq_connector-0.7.2a1/neon_mq_connector/utils/rabbit_utils.py` & `neon_mq_connector-0.7.2a2/neon_mq_connector/utils/rabbit_utils.py`

 * *Files identical despite different names*

### Comparing `neon_mq_connector-0.7.2a1/neon_mq_connector/utils/thread_utils.py` & `neon_mq_connector-0.7.2a2/neon_mq_connector/utils/thread_utils.py`

 * *Files identical despite different names*

### Comparing `neon_mq_connector-0.7.2a1/neon_mq_connector.egg-info/PKG-INFO` & `neon_mq_connector-0.7.2a2/neon_mq_connector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-mq-connector
-Version: 0.7.2a1
+Version: 0.7.2a2
 Summary: MQ Connector for Neon Modules
 Home-page: https://github.com/NeonGeckoCom/neon_mq_connector
 Author: NeonGecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `neon_mq_connector-0.7.2a1/neon_mq_connector.egg-info/SOURCES.txt` & `neon_mq_connector-0.7.2a2/neon_mq_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon_mq_connector-0.7.2a1/setup.py` & `neon_mq_connector-0.7.2a2/setup.py`

 * *Files identical despite different names*

