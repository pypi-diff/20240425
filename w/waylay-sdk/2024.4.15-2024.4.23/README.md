# Comparing `tmp/waylay_sdk-2024.4.15.tar.gz` & `tmp/waylay_sdk-2024.4.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylay_sdk-2024.4.15.tar", last modified: Mon Apr 15 12:57:09 2024, max compression
+gzip compressed data, was "waylay_sdk-2024.4.23.tar", last modified: Thu Apr 25 12:52:44 2024, max compression
```

## Comparing `waylay_sdk-2024.4.15.tar` & `waylay_sdk-2024.4.23.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 12:57:09.446366 waylay_sdk-2024.4.15/
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     8303 2024-04-15 12:57:09.446013 waylay_sdk-2024.4.15/PKG-INFO
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     6769 2024-04-09 09:16:22.000000 waylay_sdk-2024.4.15/README.md
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     1190 2024-04-15 12:56:18.000000 waylay_sdk-2024.4.15/pyproject.toml
--rw-r--r--   0 simonschoonjans   (501) staff       (20)       38 2024-04-15 12:57:09.446411 waylay_sdk-2024.4.15/setup.cfg
-drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 12:57:09.445173 waylay_sdk-2024.4.15/waylay_sdk.egg-info/
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     8303 2024-04-15 12:57:09.000000 waylay_sdk-2024.4.15/waylay_sdk.egg-info/PKG-INFO
--rw-r--r--   0 simonschoonjans   (501) staff       (20)      193 2024-04-15 12:57:09.000000 waylay_sdk-2024.4.15/waylay_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 simonschoonjans   (501) staff       (20)        1 2024-04-15 12:57:09.000000 waylay_sdk-2024.4.15/waylay_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 simonschoonjans   (501) staff       (20)      513 2024-04-15 12:57:09.000000 waylay_sdk-2024.4.15/waylay_sdk.egg-info/requires.txt
--rw-r--r--   0 simonschoonjans   (501) staff       (20)        1 2024-04-15 12:57:09.000000 waylay_sdk-2024.4.15/waylay_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-25 12:52:44.069711 waylay_sdk-2024.4.23/
+-rw-r--r--   0 thomas     (502) staff       (20)      746 2024-04-25 12:51:46.000000 waylay_sdk-2024.4.23/LICENCE.txt
+-rw-r--r--   0 thomas     (502) staff       (20)     8664 2024-04-25 12:52:44.069224 waylay_sdk-2024.4.23/PKG-INFO
+-rw-r--r--   0 thomas     (502) staff       (20)     6769 2024-04-09 11:13:26.000000 waylay_sdk-2024.4.23/README.md
+-rw-r--r--   0 thomas     (502) staff       (20)     1606 2024-04-25 12:49:55.000000 waylay_sdk-2024.4.23/pyproject.toml
+-rw-r--r--   0 thomas     (502) staff       (20)       38 2024-04-25 12:52:44.069757 waylay_sdk-2024.4.23/setup.cfg
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-25 12:52:44.068390 waylay_sdk-2024.4.23/waylay_sdk.egg-info/
+-rw-r--r--   0 thomas     (502) staff       (20)     8664 2024-04-25 12:52:44.000000 waylay_sdk-2024.4.23/waylay_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 thomas     (502) staff       (20)      205 2024-04-25 12:52:44.000000 waylay_sdk-2024.4.23/waylay_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas     (502) staff       (20)        1 2024-04-25 12:52:44.000000 waylay_sdk-2024.4.23/waylay_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas     (502) staff       (20)      833 2024-04-25 12:52:44.000000 waylay_sdk-2024.4.23/waylay_sdk.egg-info/requires.txt
+-rw-r--r--   0 thomas     (502) staff       (20)        1 2024-04-25 12:52:44.000000 waylay_sdk-2024.4.23/waylay_sdk.egg-info/top_level.txt
```

### Comparing `waylay_sdk-2024.4.15/PKG-INFO` & `waylay_sdk-2024.4.23/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 Metadata-Version: 2.1
 Name: waylay-sdk
-Version: 2024.4.15
+Version: 2024.4.23
 Summary: Waylay Python SDK.
 Author-email: Waylay <info@waylay.io>
 Project-URL: Homepage, https://www.waylay.io/
 Project-URL: Documentation, https://docs.waylay.io/#/api/sdk/python
 Project-URL: Repository, https://github.com/waylayio/waylay-py-services.git
 Keywords: waylay,sdk
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: waylay-sdk-alarms
-Requires-Dist: waylay-sdk-data
-Requires-Dist: waylay-sdk-registry
-Requires-Dist: waylay-sdk-resources
-Requires-Dist: waylay-sdk-rules
-Requires-Dist: waylay-sdk-storage
+License-File: LICENCE.txt
+Requires-Dist: waylay-sdk-core~=0.2.1
+Requires-Dist: waylay-sdk-alarms>=1.11.0.20240423
+Requires-Dist: waylay-sdk-data>=2.14.0.20240423
+Requires-Dist: waylay-sdk-registry>=2.12.4.20240423
+Requires-Dist: waylay-sdk-resources>=8.1.0.20240423
+Requires-Dist: waylay-sdk-rules>=6.5.0.20240423
+Requires-Dist: waylay-sdk-storage>=0.4.1.20240423
 Provides-Extra: types-alarms
-Requires-Dist: waylay-sdk-alarms-types; extra == "types-alarms"
+Requires-Dist: waylay-sdk-alarms-types>=1.11.0.20240423; extra == "types-alarms"
 Provides-Extra: types-data
-Requires-Dist: waylay-sdk-data-types; extra == "types-data"
+Requires-Dist: waylay-sdk-data-types>=2.14.0.20240423; extra == "types-data"
 Provides-Extra: types-registry
-Requires-Dist: waylay-sdk-registry-types; extra == "types-registry"
+Requires-Dist: waylay-sdk-registry-types>=2.12.4.20240423; extra == "types-registry"
 Provides-Extra: types-resources
-Requires-Dist: waylay-sdk-resources-types; extra == "types-resources"
+Requires-Dist: waylay-sdk-resources-types>=8.1.0.20240423; extra == "types-resources"
 Provides-Extra: types-rules
-Requires-Dist: waylay-sdk-rules-types; extra == "types-rules"
+Requires-Dist: waylay-sdk-rules-types>=6.5.0.20240423; extra == "types-rules"
 Provides-Extra: types-storage
-Requires-Dist: waylay-sdk-storage-types; extra == "types-storage"
+Requires-Dist: waylay-sdk-storage-types>=0.4.1.20240423; extra == "types-storage"
 Provides-Extra: types
-Requires-Dist: waylay-sdk-alarms-types; extra == "types"
-Requires-Dist: waylay-sdk-data-types; extra == "types"
-Requires-Dist: waylay-sdk-registry-types; extra == "types"
-Requires-Dist: waylay-sdk-resources-types; extra == "types"
-Requires-Dist: waylay-sdk-rules-types; extra == "types"
-Requires-Dist: waylay-sdk-storage-types; extra == "types"
+Requires-Dist: waylay-sdk-alarms-types>=1.11.0.20240423; extra == "types"
+Requires-Dist: waylay-sdk-data-types>=2.14.0.20240423; extra == "types"
+Requires-Dist: waylay-sdk-registry-types>=2.12.4.20240423; extra == "types"
+Requires-Dist: waylay-sdk-resources-types>=8.1.0.20240423; extra == "types"
+Requires-Dist: waylay-sdk-rules-types>=6.5.0.20240423; extra == "types"
+Requires-Dist: waylay-sdk-storage-types>=0.4.1.20240423; extra == "types"
 
 # Waylay Python SDK
 
 Python SDK for the Waylay Platform.
 
 This `waylay-sdk` package is the main entrypoint to install the python SDK client for the [Waylay REST apis](https://docs.waylay.io/#/api/?id=openapi-docs).
```

### Comparing `waylay_sdk-2024.4.15/README.md` & `waylay_sdk-2024.4.23/README.md`

 * *Files identical despite different names*

### Comparing `waylay_sdk-2024.4.15/waylay_sdk.egg-info/PKG-INFO` & `waylay_sdk-2024.4.23/waylay_sdk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 Metadata-Version: 2.1
 Name: waylay-sdk
-Version: 2024.4.15
+Version: 2024.4.23
 Summary: Waylay Python SDK.
 Author-email: Waylay <info@waylay.io>
 Project-URL: Homepage, https://www.waylay.io/
 Project-URL: Documentation, https://docs.waylay.io/#/api/sdk/python
 Project-URL: Repository, https://github.com/waylayio/waylay-py-services.git
 Keywords: waylay,sdk
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: waylay-sdk-alarms
-Requires-Dist: waylay-sdk-data
-Requires-Dist: waylay-sdk-registry
-Requires-Dist: waylay-sdk-resources
-Requires-Dist: waylay-sdk-rules
-Requires-Dist: waylay-sdk-storage
+License-File: LICENCE.txt
+Requires-Dist: waylay-sdk-core~=0.2.1
+Requires-Dist: waylay-sdk-alarms>=1.11.0.20240423
+Requires-Dist: waylay-sdk-data>=2.14.0.20240423
+Requires-Dist: waylay-sdk-registry>=2.12.4.20240423
+Requires-Dist: waylay-sdk-resources>=8.1.0.20240423
+Requires-Dist: waylay-sdk-rules>=6.5.0.20240423
+Requires-Dist: waylay-sdk-storage>=0.4.1.20240423
 Provides-Extra: types-alarms
-Requires-Dist: waylay-sdk-alarms-types; extra == "types-alarms"
+Requires-Dist: waylay-sdk-alarms-types>=1.11.0.20240423; extra == "types-alarms"
 Provides-Extra: types-data
-Requires-Dist: waylay-sdk-data-types; extra == "types-data"
+Requires-Dist: waylay-sdk-data-types>=2.14.0.20240423; extra == "types-data"
 Provides-Extra: types-registry
-Requires-Dist: waylay-sdk-registry-types; extra == "types-registry"
+Requires-Dist: waylay-sdk-registry-types>=2.12.4.20240423; extra == "types-registry"
 Provides-Extra: types-resources
-Requires-Dist: waylay-sdk-resources-types; extra == "types-resources"
+Requires-Dist: waylay-sdk-resources-types>=8.1.0.20240423; extra == "types-resources"
 Provides-Extra: types-rules
-Requires-Dist: waylay-sdk-rules-types; extra == "types-rules"
+Requires-Dist: waylay-sdk-rules-types>=6.5.0.20240423; extra == "types-rules"
 Provides-Extra: types-storage
-Requires-Dist: waylay-sdk-storage-types; extra == "types-storage"
+Requires-Dist: waylay-sdk-storage-types>=0.4.1.20240423; extra == "types-storage"
 Provides-Extra: types
-Requires-Dist: waylay-sdk-alarms-types; extra == "types"
-Requires-Dist: waylay-sdk-data-types; extra == "types"
-Requires-Dist: waylay-sdk-registry-types; extra == "types"
-Requires-Dist: waylay-sdk-resources-types; extra == "types"
-Requires-Dist: waylay-sdk-rules-types; extra == "types"
-Requires-Dist: waylay-sdk-storage-types; extra == "types"
+Requires-Dist: waylay-sdk-alarms-types>=1.11.0.20240423; extra == "types"
+Requires-Dist: waylay-sdk-data-types>=2.14.0.20240423; extra == "types"
+Requires-Dist: waylay-sdk-registry-types>=2.12.4.20240423; extra == "types"
+Requires-Dist: waylay-sdk-resources-types>=8.1.0.20240423; extra == "types"
+Requires-Dist: waylay-sdk-rules-types>=6.5.0.20240423; extra == "types"
+Requires-Dist: waylay-sdk-storage-types>=0.4.1.20240423; extra == "types"
 
 # Waylay Python SDK
 
 Python SDK for the Waylay Platform.
 
 This `waylay-sdk` package is the main entrypoint to install the python SDK client for the [Waylay REST apis](https://docs.waylay.io/#/api/?id=openapi-docs).
```

