# Comparing `tmp/dropmqttapi-1.0.2.tar.gz` & `tmp/dropmqttapi-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dropmqttapi-1.0.2.tar", last modified: Wed Jan  3 17:56:05 2024, max compression
+gzip compressed data, was "dropmqttapi-1.0.3.tar", last modified: Thu Apr 25 14:14:44 2024, max compression
```

## Comparing `dropmqttapi-1.0.2.tar` & `dropmqttapi-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 pfrazer   (1000) pfrazer   (1000)        0 2024-01-03 17:56:05.800030 dropmqttapi-1.0.2/
--rw-rw-r--   0 pfrazer   (1000) pfrazer   (1000)     1079 2023-12-18 21:24:05.000000 dropmqttapi-1.0.2/LICENSE
--rw-r--r--   0 pfrazer   (1000) pfrazer   (1000)     1815 2024-01-03 17:56:05.800030 dropmqttapi-1.0.2/PKG-INFO
--rw-rw-r--   0 pfrazer   (1000) pfrazer   (1000)       65 2023-12-18 21:24:05.000000 dropmqttapi-1.0.2/README.md
--rw-rw-r--   0 pfrazer   (1000) pfrazer   (1000)      662 2024-01-03 17:51:11.000000 dropmqttapi-1.0.2/pyproject.toml
--rw-rw-r--   0 pfrazer   (1000) pfrazer   (1000)       38 2024-01-03 17:56:05.800030 dropmqttapi-1.0.2/setup.cfg
-drwxrwxr-x   0 pfrazer   (1000) pfrazer   (1000)        0 2024-01-03 17:56:05.800030 dropmqttapi-1.0.2/src/
-drwxrwxr-x   0 pfrazer   (1000) pfrazer   (1000)        0 2024-01-03 17:56:05.800030 dropmqttapi-1.0.2/src/dropmqttapi/
--rw-rw-r--   0 pfrazer   (1000) pfrazer   (1000)       20 2023-12-18 21:27:46.000000 dropmqttapi-1.0.2/src/dropmqttapi/__init__.py
--rw-rw-r--   0 pfrazer   (1000) pfrazer   (1000)     3213 2023-12-19 12:40:02.000000 dropmqttapi-1.0.2/src/dropmqttapi/discovery.py
--rw-rw-r--   0 pfrazer   (1000) pfrazer   (1000)     5397 2024-01-03 17:49:49.000000 dropmqttapi-1.0.2/src/dropmqttapi/mqttapi.py
-drwxrwxr-x   0 pfrazer   (1000) pfrazer   (1000)        0 2024-01-03 17:56:05.800030 dropmqttapi-1.0.2/src/dropmqttapi.egg-info/
--rw-r--r--   0 pfrazer   (1000) pfrazer   (1000)     1815 2024-01-03 17:56:05.000000 dropmqttapi-1.0.2/src/dropmqttapi.egg-info/PKG-INFO
--rw-rw-r--   0 pfrazer   (1000) pfrazer   (1000)      272 2024-01-03 17:56:05.000000 dropmqttapi-1.0.2/src/dropmqttapi.egg-info/SOURCES.txt
--rw-rw-r--   0 pfrazer   (1000) pfrazer   (1000)        1 2024-01-03 17:56:05.000000 dropmqttapi-1.0.2/src/dropmqttapi.egg-info/dependency_links.txt
--rw-rw-r--   0 pfrazer   (1000) pfrazer   (1000)       12 2024-01-03 17:56:05.000000 dropmqttapi-1.0.2/src/dropmqttapi.egg-info/top_level.txt
+drwxrwxr-x   0 pfrazer   (1000) pfrazer   (1000)        0 2024-04-25 14:14:44.273162 dropmqttapi-1.0.3/
+-rw-rw-r--   0 pfrazer   (1000) pfrazer   (1000)     1079 2024-04-25 12:21:51.000000 dropmqttapi-1.0.3/LICENSE
+-rw-r--r--   0 pfrazer   (1000) pfrazer   (1000)     1815 2024-04-25 14:14:44.273162 dropmqttapi-1.0.3/PKG-INFO
+-rw-rw-r--   0 pfrazer   (1000) pfrazer   (1000)       65 2024-04-25 12:21:51.000000 dropmqttapi-1.0.3/README.md
+-rw-rw-r--   0 pfrazer   (1000) pfrazer   (1000)      662 2024-04-25 12:25:53.000000 dropmqttapi-1.0.3/pyproject.toml
+-rw-rw-r--   0 pfrazer   (1000) pfrazer   (1000)       38 2024-04-25 14:14:44.273162 dropmqttapi-1.0.3/setup.cfg
+drwxrwxr-x   0 pfrazer   (1000) pfrazer   (1000)        0 2024-04-25 14:14:44.269162 dropmqttapi-1.0.3/src/
+drwxrwxr-x   0 pfrazer   (1000) pfrazer   (1000)        0 2024-04-25 14:14:44.269162 dropmqttapi-1.0.3/src/dropmqttapi/
+-rw-rw-r--   0 pfrazer   (1000) pfrazer   (1000)       20 2024-04-25 12:21:51.000000 dropmqttapi-1.0.3/src/dropmqttapi/__init__.py
+-rw-rw-r--   0 pfrazer   (1000) pfrazer   (1000)     3213 2024-04-25 12:21:51.000000 dropmqttapi-1.0.3/src/dropmqttapi/discovery.py
+-rw-rw-r--   0 pfrazer   (1000) pfrazer   (1000)     5641 2024-04-25 12:46:33.000000 dropmqttapi-1.0.3/src/dropmqttapi/mqttapi.py
+drwxrwxr-x   0 pfrazer   (1000) pfrazer   (1000)        0 2024-04-25 14:14:44.269162 dropmqttapi-1.0.3/src/dropmqttapi.egg-info/
+-rw-r--r--   0 pfrazer   (1000) pfrazer   (1000)     1815 2024-04-25 14:14:44.000000 dropmqttapi-1.0.3/src/dropmqttapi.egg-info/PKG-INFO
+-rw-rw-r--   0 pfrazer   (1000) pfrazer   (1000)      272 2024-04-25 14:14:44.000000 dropmqttapi-1.0.3/src/dropmqttapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 pfrazer   (1000) pfrazer   (1000)        1 2024-04-25 14:14:44.000000 dropmqttapi-1.0.3/src/dropmqttapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 pfrazer   (1000) pfrazer   (1000)       12 2024-04-25 14:14:44.000000 dropmqttapi-1.0.3/src/dropmqttapi.egg-info/top_level.txt
```

### Comparing `dropmqttapi-1.0.2/LICENSE` & `dropmqttapi-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dropmqttapi-1.0.2/PKG-INFO` & `dropmqttapi-1.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dropmqttapi
-Version: 1.0.2
+Version: 1.0.3
 Summary: MQTT API for DROP water management products
 Author-email: Patrick Frazer <pfrazer@chandlersystemsinc.com>
 License: MIT License
         
         Copyright (c) 2023 Chandler Systems, Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dropmqttapi-1.0.2/pyproject.toml` & `dropmqttapi-1.0.3/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dropmqttapi"
-version = "1.0.2"
+version = "1.0.3"
 description = "MQTT API for DROP water management products"
 readme = "README.md"
 authors = [{ name = "Patrick Frazer", email = "pfrazer@chandlersystemsinc.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `dropmqttapi-1.0.2/src/dropmqttapi/discovery.py` & `dropmqttapi-1.0.3/src/dropmqttapi/discovery.py`

 * *Files identical despite different names*

### Comparing `dropmqttapi-1.0.2/src/dropmqttapi/mqttapi.py` & `dropmqttapi-1.0.3/src/dropmqttapi/mqttapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,22 @@
         """Return cartridge 3 life remaining."""
         return self.get_int_val("cart3")
 
     def leak_detected(self) -> int | None:
         """Return leak detected value."""
         return self.get_int_val("leak")
 
+    def sensor_high(self) -> int | None:
+        """Return sensor high indication."""
+        return self.get_int_val("sens")
+
+    def power(self) -> int | None:
+        """Return power state."""
+        return self.get_int_val("pwrOff") == 0
+
     def notification_pending(self) -> int | None:
         """Return notification pending value."""
         return self.get_int_val("notif")
 
     def salt_low(self) -> int | None:
         """Return salt low value."""
         return self.get_int_val("salt")
```

### Comparing `dropmqttapi-1.0.2/src/dropmqttapi.egg-info/PKG-INFO` & `dropmqttapi-1.0.3/src/dropmqttapi.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dropmqttapi
-Version: 1.0.2
+Version: 1.0.3
 Summary: MQTT API for DROP water management products
 Author-email: Patrick Frazer <pfrazer@chandlersystemsinc.com>
 License: MIT License
         
         Copyright (c) 2023 Chandler Systems, Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

