# Comparing `tmp/rov_collector-1.1.4.tar.gz` & `tmp/rov_collector-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rov_collector-1.1.4.tar", last modified: Sun Apr  7 07:23:28 2024, max compression
+gzip compressed data, was "rov_collector-1.1.5.tar", last modified: Thu Apr 25 04:20:37 2024, max compression
```

## Comparing `rov_collector-1.1.4.tar` & `rov_collector-1.1.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-07 07:23:28.129138 rov_collector-1.1.4/
--rw-rw-r--   0 anon      (1000) anon      (1000)     1460 2023-11-28 04:14:44.000000 rov_collector-1.1.4/LICENSE.txt
--rw-rw-r--   0 anon      (1000) anon      (1000)      124 2024-04-07 07:21:39.000000 rov_collector-1.1.4/MANIFEST.in
--rw-r--r--   0 anon      (1000) anon      (1000)    14317 2024-04-07 07:23:28.129138 rov_collector-1.1.4/PKG-INFO
--rw-rw-r--   0 anon      (1000) anon      (1000)    11665 2024-04-07 07:22:54.000000 rov_collector-1.1.4/README.md
--rw-rw-r--   0 anon      (1000) anon      (1000)     1788 2024-04-07 07:21:44.000000 rov_collector-1.1.4/pyproject.toml
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-07 07:23:28.125138 rov_collector-1.1.4/rov_collector/
--rwxrwxr-x   0 anon      (1000) anon      (1000)      690 2023-12-06 20:43:29.000000 rov_collector-1.1.4/rov_collector/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      811 2023-12-06 20:56:04.000000 rov_collector-1.1.4/rov_collector/__main__.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-07 07:23:28.125138 rov_collector-1.1.4/rov_collector/collectors/
--rw-rw-r--   0 anon      (1000) anon      (1000)      651 2023-11-30 02:52:38.000000 rov_collector-1.1.4/rov_collector/collectors/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     4049 2023-12-06 20:35:44.000000 rov_collector-1.1.4/rov_collector/collectors/apnic_collector.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1605 2023-11-30 04:11:39.000000 rov_collector-1.1.4/rov_collector/collectors/friends_collector.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     2231 2023-11-28 19:47:29.000000 rov_collector-1.1.4/rov_collector/collectors/is_bgp_safe_yet_collector.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1559 2023-12-06 20:37:44.000000 rov_collector-1.1.4/rov_collector/collectors/rov_rpki_net_collector.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1984 2023-12-06 20:48:03.000000 rov_collector-1.1.4/rov_collector/collectors/rovista_collector.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1356 2023-12-06 20:37:56.000000 rov_collector-1.1.4/rov_collector/collectors/tma_collector.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-07 07:23:28.125138 rov_collector-1.1.4/rov_collector/data/
--rw-rw-r--   0 anon      (1000) anon      (1000)    35977 2023-11-30 02:46:24.000000 rov_collector-1.1.4/rov_collector/data/friends.json
--rw-rw-r--   0 anon      (1000) anon      (1000)    94633 2023-11-28 08:07:02.000000 rov_collector-1.1.4/rov_collector/data/rov.rpki.net.json
--rw-rw-r--   0 anon      (1000) anon      (1000)     1153 2023-11-28 06:33:42.000000 rov_collector-1.1.4/rov_collector/data/tma.csv
--rw-rw-r--   0 anon      (1000) anon      (1000)      948 2023-12-06 20:47:51.000000 rov_collector-1.1.4/rov_collector/enums_dataclasses.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-07 07:23:28.129138 rov_collector-1.1.4/rov_collector/graphs/
--rw-rw-r--   0 anon      (1000) anon      (1000)      187 2023-12-06 20:40:19.000000 rov_collector-1.1.4/rov_collector/graphs/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     2844 2023-12-06 20:56:04.000000 rov_collector-1.1.4/rov_collector/graphs/rov_confidence_distribution_graph.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     3393 2024-02-23 03:27:13.000000 rov_collector-1.1.4/rov_collector/graphs/rov_source_graph.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1912 2023-12-01 08:19:32.000000 rov_collector-1.1.4/rov_collector/rov_collector.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-07 07:23:28.129138 rov_collector-1.1.4/rov_collector/test/
--rwxrwxr-x   0 anon      (1000) anon      (1000)        0 2023-11-28 04:14:44.000000 rov_collector-1.1.4/rov_collector/test/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     2404 2023-11-28 07:37:59.000000 rov_collector-1.1.4/rov_collector/test/test_rov_collectors.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-07 07:23:28.129138 rov_collector-1.1.4/rov_collector.egg-info/
--rw-r--r--   0 anon      (1000) anon      (1000)    14317 2024-04-07 07:23:28.000000 rov_collector-1.1.4/rov_collector.egg-info/PKG-INFO
--rw-rw-r--   0 anon      (1000) anon      (1000)     1029 2024-04-07 07:23:28.000000 rov_collector-1.1.4/rov_collector.egg-info/SOURCES.txt
--rw-rw-r--   0 anon      (1000) anon      (1000)        1 2024-04-07 07:23:28.000000 rov_collector-1.1.4/rov_collector.egg-info/dependency_links.txt
--rw-rw-r--   0 anon      (1000) anon      (1000)       62 2024-04-07 07:23:28.000000 rov_collector-1.1.4/rov_collector.egg-info/entry_points.txt
--rw-rw-r--   0 anon      (1000) anon      (1000)      195 2024-04-07 07:23:28.000000 rov_collector-1.1.4/rov_collector.egg-info/requires.txt
--rw-rw-r--   0 anon      (1000) anon      (1000)       14 2024-04-07 07:23:28.000000 rov_collector-1.1.4/rov_collector.egg-info/top_level.txt
--rw-rw-r--   0 anon      (1000) anon      (1000)       69 2024-04-07 07:23:28.129138 rov_collector-1.1.4/setup.cfg
--rw-rw-r--   0 anon      (1000) anon      (1000)     1051 2024-02-23 03:56:08.000000 rov_collector-1.1.4/tox.ini
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-25 04:20:37.695921 rov_collector-1.1.5/
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1460 2023-11-28 04:14:44.000000 rov_collector-1.1.5/LICENSE.txt
+-rw-rw-r--   0 anon      (1000) anon      (1000)      124 2024-04-07 07:21:39.000000 rov_collector-1.1.5/MANIFEST.in
+-rw-r--r--   0 anon      (1000) anon      (1000)    14362 2024-04-25 04:20:37.695921 rov_collector-1.1.5/PKG-INFO
+-rw-rw-r--   0 anon      (1000) anon      (1000)    11710 2024-04-25 04:19:05.000000 rov_collector-1.1.5/README.md
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1788 2024-04-25 04:20:13.000000 rov_collector-1.1.5/pyproject.toml
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-25 04:20:37.691921 rov_collector-1.1.5/rov_collector/
+-rwxrwxr-x   0 anon      (1000) anon      (1000)      797 2024-04-25 04:20:04.000000 rov_collector-1.1.5/rov_collector/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      811 2023-12-06 20:56:04.000000 rov_collector-1.1.5/rov_collector/__main__.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-25 04:20:37.695921 rov_collector-1.1.5/rov_collector/collectors/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      651 2023-11-30 02:52:38.000000 rov_collector-1.1.5/rov_collector/collectors/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     4049 2023-12-06 20:35:44.000000 rov_collector-1.1.5/rov_collector/collectors/apnic_collector.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1605 2023-11-30 04:11:39.000000 rov_collector-1.1.5/rov_collector/collectors/friends_collector.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     2231 2023-11-28 19:47:29.000000 rov_collector-1.1.5/rov_collector/collectors/is_bgp_safe_yet_collector.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1559 2023-12-06 20:37:44.000000 rov_collector-1.1.5/rov_collector/collectors/rov_rpki_net_collector.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1984 2023-12-06 20:48:03.000000 rov_collector-1.1.5/rov_collector/collectors/rovista_collector.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1356 2023-12-06 20:37:56.000000 rov_collector-1.1.5/rov_collector/collectors/tma_collector.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-25 04:20:37.695921 rov_collector-1.1.5/rov_collector/data/
+-rw-rw-r--   0 anon      (1000) anon      (1000)    35977 2023-11-30 02:46:24.000000 rov_collector-1.1.5/rov_collector/data/friends.json
+-rw-rw-r--   0 anon      (1000) anon      (1000)    94633 2023-11-28 08:07:02.000000 rov_collector-1.1.5/rov_collector/data/rov.rpki.net.json
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1153 2023-11-28 06:33:42.000000 rov_collector-1.1.5/rov_collector/data/tma.csv
+-rw-rw-r--   0 anon      (1000) anon      (1000)      948 2023-12-06 20:47:51.000000 rov_collector-1.1.5/rov_collector/enums_dataclasses.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-25 04:20:37.695921 rov_collector-1.1.5/rov_collector/graphs/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      187 2023-12-06 20:40:19.000000 rov_collector-1.1.5/rov_collector/graphs/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     2844 2023-12-06 20:56:04.000000 rov_collector-1.1.5/rov_collector/graphs/rov_confidence_distribution_graph.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     3393 2024-02-23 03:27:13.000000 rov_collector-1.1.5/rov_collector/graphs/rov_source_graph.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1912 2023-12-01 08:19:32.000000 rov_collector-1.1.5/rov_collector/rov_collector.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-25 04:20:37.695921 rov_collector-1.1.5/rov_collector/test/
+-rwxrwxr-x   0 anon      (1000) anon      (1000)        0 2023-11-28 04:14:44.000000 rov_collector-1.1.5/rov_collector/test/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     2404 2023-11-28 07:37:59.000000 rov_collector-1.1.5/rov_collector/test/test_rov_collectors.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-25 04:20:37.695921 rov_collector-1.1.5/rov_collector.egg-info/
+-rw-r--r--   0 anon      (1000) anon      (1000)    14362 2024-04-25 04:20:37.000000 rov_collector-1.1.5/rov_collector.egg-info/PKG-INFO
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1029 2024-04-25 04:20:37.000000 rov_collector-1.1.5/rov_collector.egg-info/SOURCES.txt
+-rw-rw-r--   0 anon      (1000) anon      (1000)        1 2024-04-25 04:20:37.000000 rov_collector-1.1.5/rov_collector.egg-info/dependency_links.txt
+-rw-rw-r--   0 anon      (1000) anon      (1000)       62 2024-04-25 04:20:37.000000 rov_collector-1.1.5/rov_collector.egg-info/entry_points.txt
+-rw-rw-r--   0 anon      (1000) anon      (1000)      195 2024-04-25 04:20:37.000000 rov_collector-1.1.5/rov_collector.egg-info/requires.txt
+-rw-rw-r--   0 anon      (1000) anon      (1000)       14 2024-04-25 04:20:37.000000 rov_collector-1.1.5/rov_collector.egg-info/top_level.txt
+-rw-rw-r--   0 anon      (1000) anon      (1000)       69 2024-04-25 04:20:37.699921 rov_collector-1.1.5/setup.cfg
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1051 2024-02-23 03:56:08.000000 rov_collector-1.1.5/tox.ini
```

### Comparing `rov_collector-1.1.4/LICENSE.txt` & `rov_collector-1.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rov_collector-1.1.4/PKG-INFO` & `rov_collector-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rov_collector
-Version: 1.1.4
+Version: 1.1.5
 Summary: Downloads ROV info from various sources
 Author-email: Justin Furuness <jfuruness@gmail.com>
 License: Copyright 2020 Justin Furuness
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
@@ -368,14 +368,15 @@
 * [Collector](https://github.com/jfuruness/rov_collector/blob/master/rov_collector/apnic_collector.py)
 
 
 
 ## History
 * [rov\_collector](#rov\_collector)
 
+1.1.5 Added a top level import for the enums
 1.1.4 Fixed a typo in the MANIFEST.IN file that resulted in the data directly not being included in source distributions
 1.1.3 Updated versions and dependencies
 
 ## Development/Contributing
 * [rov\_collector](#rov\_collector)
 
 1. Fork it!
```

### Comparing `rov_collector-1.1.4/README.md` & `rov_collector-1.1.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -328,14 +328,15 @@
 * [Collector](https://github.com/jfuruness/rov_collector/blob/master/rov_collector/apnic_collector.py)
 
 
 
 ## History
 * [rov\_collector](#rov\_collector)
 
+1.1.5 Added a top level import for the enums
 1.1.4 Fixed a typo in the MANIFEST.IN file that resulted in the data directly not being included in source distributions
 1.1.3 Updated versions and dependencies
 
 ## Development/Contributing
 * [rov\_collector](#rov\_collector)
 
 1. Fork it!
```

### Comparing `rov_collector-1.1.4/pyproject.toml` & `rov_collector-1.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "rov_collector"
-version = "1.1.4"
+version = "1.1.5"
 description = "Downloads ROV info from various sources"
 readme = "README.md"
 authors = [
     {name = "Justin Furuness", email = "jfuruness@gmail.com"},
 ]
 license = {file = "LICENSE.txt"}
 keywords = [
```

### Comparing `rov_collector-1.1.4/rov_collector/__init__.py` & `rov_collector-1.1.5/rov_collector/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,20 +4,25 @@
 from .collectors import FriendsCollector
 from .collectors import ROVISTACollector
 from .collectors import ROVRPKINetCollector
 from .collectors import TMACollector
 from .collectors import rov_collector_classes
 from .graphs import ROVSourceGraph
 from .graphs import ROVConfidenceDistributionGraph
+from .enums_dataclasses import FilterType, Source, ROVInfo
+
 
 __all__ = [
     "ROVCollector",
     "APNICCollector",
     "IsBGPSafeYetCollector",
     "FriendsCollector",
     "ROVISTACollector",
     "ROVRPKINetCollector",
     "TMACollector",
     "rov_collector_classes",
     "ROVConfidenceDistributionGraph",
     "ROVSourceGraph",
+    "FilterType",
+    "Source",
+    "ROVInfo",
 ]
```

### Comparing `rov_collector-1.1.4/rov_collector/__main__.py` & `rov_collector-1.1.5/rov_collector/__main__.py`

 * *Files identical despite different names*

### Comparing `rov_collector-1.1.4/rov_collector/collectors/__init__.py` & `rov_collector-1.1.5/rov_collector/collectors/__init__.py`

 * *Files identical despite different names*

### Comparing `rov_collector-1.1.4/rov_collector/collectors/apnic_collector.py` & `rov_collector-1.1.5/rov_collector/collectors/apnic_collector.py`

 * *Files identical despite different names*

### Comparing `rov_collector-1.1.4/rov_collector/collectors/friends_collector.py` & `rov_collector-1.1.5/rov_collector/collectors/friends_collector.py`

 * *Files identical despite different names*

### Comparing `rov_collector-1.1.4/rov_collector/collectors/is_bgp_safe_yet_collector.py` & `rov_collector-1.1.5/rov_collector/collectors/is_bgp_safe_yet_collector.py`

 * *Files identical despite different names*

### Comparing `rov_collector-1.1.4/rov_collector/collectors/rov_rpki_net_collector.py` & `rov_collector-1.1.5/rov_collector/collectors/rov_rpki_net_collector.py`

 * *Files identical despite different names*

### Comparing `rov_collector-1.1.4/rov_collector/collectors/rovista_collector.py` & `rov_collector-1.1.5/rov_collector/collectors/rovista_collector.py`

 * *Files identical despite different names*

### Comparing `rov_collector-1.1.4/rov_collector/collectors/tma_collector.py` & `rov_collector-1.1.5/rov_collector/collectors/tma_collector.py`

 * *Files identical despite different names*

### Comparing `rov_collector-1.1.4/rov_collector/data/friends.json` & `rov_collector-1.1.5/rov_collector/data/friends.json`

 * *Files identical despite different names*

### Comparing `rov_collector-1.1.4/rov_collector/data/rov.rpki.net.json` & `rov_collector-1.1.5/rov_collector/data/rov.rpki.net.json`

 * *Files identical despite different names*

### Comparing `rov_collector-1.1.4/rov_collector/data/tma.csv` & `rov_collector-1.1.5/rov_collector/data/tma.csv`

 * *Files identical despite different names*

### Comparing `rov_collector-1.1.4/rov_collector/enums_dataclasses.py` & `rov_collector-1.1.5/rov_collector/enums_dataclasses.py`

 * *Files identical despite different names*

### Comparing `rov_collector-1.1.4/rov_collector/graphs/rov_confidence_distribution_graph.py` & `rov_collector-1.1.5/rov_collector/graphs/rov_confidence_distribution_graph.py`

 * *Files identical despite different names*

### Comparing `rov_collector-1.1.4/rov_collector/graphs/rov_source_graph.py` & `rov_collector-1.1.5/rov_collector/graphs/rov_source_graph.py`

 * *Files identical despite different names*

### Comparing `rov_collector-1.1.4/rov_collector/rov_collector.py` & `rov_collector-1.1.5/rov_collector/rov_collector.py`

 * *Files identical despite different names*

### Comparing `rov_collector-1.1.4/rov_collector/test/test_rov_collectors.py` & `rov_collector-1.1.5/rov_collector/test/test_rov_collectors.py`

 * *Files identical despite different names*

### Comparing `rov_collector-1.1.4/rov_collector.egg-info/PKG-INFO` & `rov_collector-1.1.5/rov_collector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rov_collector
-Version: 1.1.4
+Version: 1.1.5
 Summary: Downloads ROV info from various sources
 Author-email: Justin Furuness <jfuruness@gmail.com>
 License: Copyright 2020 Justin Furuness
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
@@ -368,14 +368,15 @@
 * [Collector](https://github.com/jfuruness/rov_collector/blob/master/rov_collector/apnic_collector.py)
 
 
 
 ## History
 * [rov\_collector](#rov\_collector)
 
+1.1.5 Added a top level import for the enums
 1.1.4 Fixed a typo in the MANIFEST.IN file that resulted in the data directly not being included in source distributions
 1.1.3 Updated versions and dependencies
 
 ## Development/Contributing
 * [rov\_collector](#rov\_collector)
 
 1. Fork it!
```

### Comparing `rov_collector-1.1.4/rov_collector.egg-info/SOURCES.txt` & `rov_collector-1.1.5/rov_collector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rov_collector-1.1.4/tox.ini` & `rov_collector-1.1.5/tox.ini`

 * *Files identical despite different names*

