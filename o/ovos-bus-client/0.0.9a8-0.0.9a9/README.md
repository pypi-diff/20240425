# Comparing `tmp/ovos-bus-client-0.0.9a8.tar.gz` & `tmp/ovos-bus-client-0.0.9a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-bus-client-0.0.9a8.tar", last modified: Sat Jan 13 22:50:37 2024, max compression
+gzip compressed data, was "ovos-bus-client-0.0.9a9.tar", last modified: Tue Jan 23 16:18:52 2024, max compression
```

## Comparing `ovos-bus-client-0.0.9a8.tar` & `ovos-bus-client-0.0.9a9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 22:50:37.923669 ovos-bus-client-0.0.9a8/
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-01-13 22:50:37.000000 ovos-bus-client-0.0.9a8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-01-13 22:50:37.000000 ovos-bus-client-0.0.9a8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-01-13 22:50:37.923669 ovos-bus-client-0.0.9a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-01-13 22:50:37.000000 ovos-bus-client-0.0.9a8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 22:50:37.923669 ovos-bus-client-0.0.9a8/ovos_bus_client/
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-01-13 22:50:37.000000 ovos-bus-client-0.0.9a8/ovos_bus_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 22:50:37.923669 ovos-bus-client-0.0.9a8/ovos_bus_client/apis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 22:50:37.000000 ovos-bus-client-0.0.9a8/ovos_bus_client/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14309 2024-01-13 22:50:37.000000 ovos-bus-client-0.0.9a8/ovos_bus_client/apis/enclosure.py
--rw-r--r--   0 runner    (1001) docker     (127)    30103 2024-01-13 22:50:37.000000 ovos-bus-client-0.0.9a8/ovos_bus_client/apis/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)    34473 2024-01-13 22:50:37.000000 ovos-bus-client-0.0.9a8/ovos_bus_client/apis/ocp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 22:50:37.923669 ovos-bus-client-0.0.9a8/ovos_bus_client/client/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-01-13 22:50:37.000000 ovos-bus-client-0.0.9a8/ovos_bus_client/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17236 2024-01-13 22:50:37.000000 ovos-bus-client-0.0.9a8/ovos_bus_client/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-01-13 22:50:37.000000 ovos-bus-client-0.0.9a8/ovos_bus_client/client/collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-01-13 22:50:37.000000 ovos-bus-client-0.0.9a8/ovos_bus_client/client/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-01-13 22:50:37.000000 ovos-bus-client-0.0.9a8/ovos_bus_client/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    16260 2024-01-13 22:50:37.000000 ovos-bus-client-0.0.9a8/ovos_bus_client/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-01-13 22:50:37.000000 ovos-bus-client-0.0.9a8/ovos_bus_client/scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-01-13 22:50:37.000000 ovos-bus-client-0.0.9a8/ovos_bus_client/send_func.py
--rw-r--r--   0 runner    (1001) docker     (127)    21045 2024-01-13 22:50:37.000000 ovos-bus-client-0.0.9a8/ovos_bus_client/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 22:50:37.923669 ovos-bus-client-0.0.9a8/ovos_bus_client/util/
--rw-r--r--   0 runner    (1001) docker     (127)     6387 2024-01-13 22:50:37.000000 ovos-bus-client-0.0.9a8/ovos_bus_client/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12919 2024-01-13 22:50:37.000000 ovos-bus-client-0.0.9a8/ovos_bus_client/util/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-01-13 22:50:37.000000 ovos-bus-client-0.0.9a8/ovos_bus_client/util/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-01-13 22:50:37.000000 ovos-bus-client-0.0.9a8/ovos_bus_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 22:50:37.923669 ovos-bus-client-0.0.9a8/ovos_bus_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-01-13 22:50:37.000000 ovos-bus-client-0.0.9a8/ovos_bus_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-01-13 22:50:37.000000 ovos-bus-client-0.0.9a8/ovos_bus_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-13 22:50:37.000000 ovos-bus-client-0.0.9a8/ovos_bus_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-01-13 22:50:37.000000 ovos-bus-client-0.0.9a8/ovos_bus_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-01-13 22:50:37.000000 ovos-bus-client-0.0.9a8/ovos_bus_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-13 22:50:37.000000 ovos-bus-client-0.0.9a8/ovos_bus_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-01-13 22:50:37.000000 ovos-bus-client-0.0.9a8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-13 22:50:37.923669 ovos-bus-client-0.0.9a8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-01-13 22:50:37.000000 ovos-bus-client-0.0.9a8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:18:52.798973 ovos-bus-client-0.0.9a9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-01-23 16:18:52.000000 ovos-bus-client-0.0.9a9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-01-23 16:18:52.000000 ovos-bus-client-0.0.9a9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-01-23 16:18:52.798973 ovos-bus-client-0.0.9a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-01-23 16:18:52.000000 ovos-bus-client-0.0.9a9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:18:52.798973 ovos-bus-client-0.0.9a9/ovos_bus_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-01-23 16:18:52.000000 ovos-bus-client-0.0.9a9/ovos_bus_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:18:52.798973 ovos-bus-client-0.0.9a9/ovos_bus_client/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 16:18:52.000000 ovos-bus-client-0.0.9a9/ovos_bus_client/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14309 2024-01-23 16:18:52.000000 ovos-bus-client-0.0.9a9/ovos_bus_client/apis/enclosure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30103 2024-01-23 16:18:52.000000 ovos-bus-client-0.0.9a9/ovos_bus_client/apis/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34473 2024-01-23 16:18:52.000000 ovos-bus-client-0.0.9a9/ovos_bus_client/apis/ocp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:18:52.798973 ovos-bus-client-0.0.9a9/ovos_bus_client/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-01-23 16:18:52.000000 ovos-bus-client-0.0.9a9/ovos_bus_client/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17236 2024-01-23 16:18:52.000000 ovos-bus-client-0.0.9a9/ovos_bus_client/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-01-23 16:18:52.000000 ovos-bus-client-0.0.9a9/ovos_bus_client/client/collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-01-23 16:18:52.000000 ovos-bus-client-0.0.9a9/ovos_bus_client/client/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-01-23 16:18:52.000000 ovos-bus-client-0.0.9a9/ovos_bus_client/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16260 2024-01-23 16:18:52.000000 ovos-bus-client-0.0.9a9/ovos_bus_client/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-01-23 16:18:52.000000 ovos-bus-client-0.0.9a9/ovos_bus_client/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-01-23 16:18:52.000000 ovos-bus-client-0.0.9a9/ovos_bus_client/send_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21248 2024-01-23 16:18:52.000000 ovos-bus-client-0.0.9a9/ovos_bus_client/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:18:52.798973 ovos-bus-client-0.0.9a9/ovos_bus_client/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     6387 2024-01-23 16:18:52.000000 ovos-bus-client-0.0.9a9/ovos_bus_client/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12919 2024-01-23 16:18:52.000000 ovos-bus-client-0.0.9a9/ovos_bus_client/util/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-01-23 16:18:52.000000 ovos-bus-client-0.0.9a9/ovos_bus_client/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-01-23 16:18:52.000000 ovos-bus-client-0.0.9a9/ovos_bus_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:18:52.798973 ovos-bus-client-0.0.9a9/ovos_bus_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-01-23 16:18:52.000000 ovos-bus-client-0.0.9a9/ovos_bus_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-01-23 16:18:52.000000 ovos-bus-client-0.0.9a9/ovos_bus_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 16:18:52.000000 ovos-bus-client-0.0.9a9/ovos_bus_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-01-23 16:18:52.000000 ovos-bus-client-0.0.9a9/ovos_bus_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-01-23 16:18:52.000000 ovos-bus-client-0.0.9a9/ovos_bus_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-23 16:18:52.000000 ovos-bus-client-0.0.9a9/ovos_bus_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-01-23 16:18:52.000000 ovos-bus-client-0.0.9a9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-23 16:18:52.798973 ovos-bus-client-0.0.9a9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-01-23 16:18:52.000000 ovos-bus-client-0.0.9a9/setup.py
```

### Comparing `ovos-bus-client-0.0.9a8/LICENSE` & `ovos-bus-client-0.0.9a9/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.9a8/PKG-INFO` & `ovos-bus-client-0.0.9a9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-bus-client
-Version: 0.0.9a8
+Version: 0.0.9a9
 Summary: OVOS Messagebus Client
 Home-page: https://github.com/OpenVoiceOS/ovos-bus-client
 Author: JarbasAI
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ovos-bus-client-0.0.9a8/ovos_bus_client/__init__.py` & `ovos-bus-client-0.0.9a9/ovos_bus_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.9a8/ovos_bus_client/apis/enclosure.py` & `ovos-bus-client-0.0.9a9/ovos_bus_client/apis/enclosure.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.9a8/ovos_bus_client/apis/gui.py` & `ovos-bus-client-0.0.9a9/ovos_bus_client/apis/gui.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.9a8/ovos_bus_client/apis/ocp.py` & `ovos-bus-client-0.0.9a9/ovos_bus_client/apis/ocp.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.9a8/ovos_bus_client/client/__init__.py` & `ovos-bus-client-0.0.9a9/ovos_bus_client/client/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.9a8/ovos_bus_client/client/client.py` & `ovos-bus-client-0.0.9a9/ovos_bus_client/client/client.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.9a8/ovos_bus_client/client/collector.py` & `ovos-bus-client-0.0.9a9/ovos_bus_client/client/collector.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.9a8/ovos_bus_client/client/waiter.py` & `ovos-bus-client-0.0.9a9/ovos_bus_client/client/waiter.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.9a8/ovos_bus_client/conf.py` & `ovos-bus-client-0.0.9a9/ovos_bus_client/conf.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.9a8/ovos_bus_client/message.py` & `ovos-bus-client-0.0.9a9/ovos_bus_client/message.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.9a8/ovos_bus_client/scripts.py` & `ovos-bus-client-0.0.9a9/ovos_bus_client/scripts.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.9a8/ovos_bus_client/send_func.py` & `ovos-bus-client-0.0.9a9/ovos_bus_client/send_func.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.9a8/ovos_bus_client/session.py` & `ovos-bus-client-0.0.9a9/ovos_bus_client/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -539,15 +539,17 @@
         @param make_default: if true, set default_session to sess
         """
         if not sess:
             raise ValueError(f"Expected Session and got None")
 
         if make_default:
             sess.session_id = "default"
-            LOG.debug(f"replacing default session with: {sess.serialize()}")
+            # this log is dangerous, session may contain things like passwords and access keys
+            # this comment is here to avoid reintroducing it by accident
+            # LOG.debug(f"replacing default session with: {sess.serialize()}") # DO NOT re-enable in production
 
         if sess.session_id == "default":
             SessionManager.default_session = sess
         SessionManager.sessions[sess.session_id] = sess
 
     @staticmethod
     def get(message: Optional[Message] = None) -> Session:
```

### Comparing `ovos-bus-client-0.0.9a8/ovos_bus_client/util/__init__.py` & `ovos-bus-client-0.0.9a9/ovos_bus_client/util/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.9a8/ovos_bus_client/util/scheduler.py` & `ovos-bus-client-0.0.9a9/ovos_bus_client/util/scheduler.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.9a8/ovos_bus_client/util/utils.py` & `ovos-bus-client-0.0.9a9/ovos_bus_client/util/utils.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.9a8/ovos_bus_client.egg-info/PKG-INFO` & `ovos-bus-client-0.0.9a9/ovos_bus_client.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-bus-client
-Version: 0.0.9a8
+Version: 0.0.9a9
 Summary: OVOS Messagebus Client
 Home-page: https://github.com/OpenVoiceOS/ovos-bus-client
 Author: JarbasAI
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ovos-bus-client-0.0.9a8/ovos_bus_client.egg-info/SOURCES.txt` & `ovos-bus-client-0.0.9a9/ovos_bus_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.9a8/setup.py` & `ovos-bus-client-0.0.9a9/setup.py`

 * *Files identical despite different names*

