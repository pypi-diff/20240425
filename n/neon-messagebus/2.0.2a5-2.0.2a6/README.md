# Comparing `tmp/neon_messagebus-2.0.2a5.tar.gz` & `tmp/neon_messagebus-2.0.2a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon_messagebus-2.0.2a5.tar", last modified: Wed Apr 10 01:03:10 2024, max compression
+gzip compressed data, was "neon_messagebus-2.0.2a6.tar", last modified: Thu Apr 25 16:23:18 2024, max compression
```

## Comparing `neon_messagebus-2.0.2a5.tar` & `neon_messagebus-2.0.2a6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:03:10.459369 neon_messagebus-2.0.2a5/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-10 01:03:07.000000 neon_messagebus-2.0.2a5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-10 01:03:10.459369 neon_messagebus-2.0.2a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-10 01:03:07.000000 neon_messagebus-2.0.2a5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:03:10.455369 neon_messagebus-2.0.2a5/neon_messagebus/
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-10 01:03:07.000000 neon_messagebus-2.0.2a5/neon_messagebus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-10 01:03:07.000000 neon_messagebus-2.0.2a5/neon_messagebus/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:03:10.459369 neon_messagebus-2.0.2a5/neon_messagebus/service/
--rw-r--r--   0 runner    (1001) docker     (127)     8667 2024-04-10 01:03:07.000000 neon_messagebus-2.0.2a5/neon_messagebus/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-10 01:03:07.000000 neon_messagebus-2.0.2a5/neon_messagebus/service/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:03:10.459369 neon_messagebus-2.0.2a5/neon_messagebus/util/
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-10 01:03:07.000000 neon_messagebus-2.0.2a5/neon_messagebus/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-10 01:03:07.000000 neon_messagebus-2.0.2a5/neon_messagebus/util/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-04-10 01:03:07.000000 neon_messagebus-2.0.2a5/neon_messagebus/util/message_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-10 01:03:07.000000 neon_messagebus-2.0.2a5/neon_messagebus/util/mq_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     8651 2024-04-10 01:03:07.000000 neon_messagebus-2.0.2a5/neon_messagebus/util/signal_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:03:10.459369 neon_messagebus-2.0.2a5/neon_messagebus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-10 01:03:10.000000 neon_messagebus-2.0.2a5/neon_messagebus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-10 01:03:10.000000 neon_messagebus-2.0.2a5/neon_messagebus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 01:03:10.000000 neon_messagebus-2.0.2a5/neon_messagebus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-10 01:03:10.000000 neon_messagebus-2.0.2a5/neon_messagebus.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-10 01:03:10.000000 neon_messagebus-2.0.2a5/neon_messagebus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-10 01:03:10.000000 neon_messagebus-2.0.2a5/neon_messagebus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 01:03:10.459369 neon_messagebus-2.0.2a5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-10 01:03:07.000000 neon_messagebus-2.0.2a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:23:18.584571 neon_messagebus-2.0.2a6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-25 16:23:15.000000 neon_messagebus-2.0.2a6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-25 16:23:18.584571 neon_messagebus-2.0.2a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-25 16:23:15.000000 neon_messagebus-2.0.2a6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:23:18.584571 neon_messagebus-2.0.2a6/neon_messagebus/
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-25 16:23:15.000000 neon_messagebus-2.0.2a6/neon_messagebus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-25 16:23:15.000000 neon_messagebus-2.0.2a6/neon_messagebus/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:23:18.584571 neon_messagebus-2.0.2a6/neon_messagebus/service/
+-rw-r--r--   0 runner    (1001) docker     (127)     8667 2024-04-25 16:23:15.000000 neon_messagebus-2.0.2a6/neon_messagebus/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-25 16:23:15.000000 neon_messagebus-2.0.2a6/neon_messagebus/service/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:23:18.584571 neon_messagebus-2.0.2a6/neon_messagebus/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-25 16:23:15.000000 neon_messagebus-2.0.2a6/neon_messagebus/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-25 16:23:15.000000 neon_messagebus-2.0.2a6/neon_messagebus/util/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-04-25 16:23:15.000000 neon_messagebus-2.0.2a6/neon_messagebus/util/message_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-25 16:23:15.000000 neon_messagebus-2.0.2a6/neon_messagebus/util/mq_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8651 2024-04-25 16:23:15.000000 neon_messagebus-2.0.2a6/neon_messagebus/util/signal_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:23:18.584571 neon_messagebus-2.0.2a6/neon_messagebus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-25 16:23:18.000000 neon_messagebus-2.0.2a6/neon_messagebus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-25 16:23:18.000000 neon_messagebus-2.0.2a6/neon_messagebus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:23:18.000000 neon_messagebus-2.0.2a6/neon_messagebus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-25 16:23:18.000000 neon_messagebus-2.0.2a6/neon_messagebus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-25 16:23:18.000000 neon_messagebus-2.0.2a6/neon_messagebus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-25 16:23:18.000000 neon_messagebus-2.0.2a6/neon_messagebus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 16:23:18.584571 neon_messagebus-2.0.2a6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-25 16:23:15.000000 neon_messagebus-2.0.2a6/setup.py
```

### Comparing `neon_messagebus-2.0.2a5/LICENSE.md` & `neon_messagebus-2.0.2a6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon_messagebus-2.0.2a5/PKG-INFO` & `neon_messagebus-2.0.2a6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon_messagebus
-Version: 2.0.2a5
+Version: 2.0.2a6
 Summary: Neon Messagebus Module
 Home-page: https://github.com/NeonGeckoCom/neon_messagebus
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: docker
```

### Comparing `neon_messagebus-2.0.2a5/README.md` & `neon_messagebus-2.0.2a6/README.md`

 * *Files identical despite different names*

### Comparing `neon_messagebus-2.0.2a5/neon_messagebus/__init__.py` & `neon_messagebus-2.0.2a6/neon_messagebus/__init__.py`

 * *Files identical despite different names*

### Comparing `neon_messagebus-2.0.2a5/neon_messagebus/cli.py` & `neon_messagebus-2.0.2a6/neon_messagebus/cli.py`

 * *Files identical despite different names*

### Comparing `neon_messagebus-2.0.2a5/neon_messagebus/service/__init__.py` & `neon_messagebus-2.0.2a6/neon_messagebus/service/__init__.py`

 * *Files identical despite different names*

### Comparing `neon_messagebus-2.0.2a5/neon_messagebus/service/__main__.py` & `neon_messagebus-2.0.2a6/neon_messagebus/service/__main__.py`

 * *Files identical despite different names*

### Comparing `neon_messagebus-2.0.2a5/neon_messagebus/util/__init__.py` & `neon_messagebus-2.0.2a6/neon_messagebus/util/__init__.py`

 * *Files identical despite different names*

### Comparing `neon_messagebus-2.0.2a5/neon_messagebus/util/config.py` & `neon_messagebus-2.0.2a6/neon_messagebus/util/config.py`

 * *Files identical despite different names*

### Comparing `neon_messagebus-2.0.2a5/neon_messagebus/util/message_utils.py` & `neon_messagebus-2.0.2a6/neon_messagebus/util/message_utils.py`

 * *Files identical despite different names*

### Comparing `neon_messagebus-2.0.2a5/neon_messagebus/util/mq_connector.py` & `neon_messagebus-2.0.2a6/neon_messagebus/util/mq_connector.py`

 * *Files identical despite different names*

### Comparing `neon_messagebus-2.0.2a5/neon_messagebus/util/signal_utils.py` & `neon_messagebus-2.0.2a6/neon_messagebus/util/signal_utils.py`

 * *Files identical despite different names*

### Comparing `neon_messagebus-2.0.2a5/neon_messagebus.egg-info/PKG-INFO` & `neon_messagebus-2.0.2a6/neon_messagebus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-messagebus
-Version: 2.0.2a5
+Version: 2.0.2a6
 Summary: Neon Messagebus Module
 Home-page: https://github.com/NeonGeckoCom/neon_messagebus
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: docker
```

### Comparing `neon_messagebus-2.0.2a5/neon_messagebus.egg-info/SOURCES.txt` & `neon_messagebus-2.0.2a6/neon_messagebus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon_messagebus-2.0.2a5/setup.py` & `neon_messagebus-2.0.2a6/setup.py`

 * *Files identical despite different names*

