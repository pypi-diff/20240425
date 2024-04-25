# Comparing `tmp/joker-mongodb-0.1.5.tar.gz` & `tmp/joker-mongodb-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joker-mongodb-0.1.5.tar", last modified: Fri Nov 25 02:16:38 2022, max compression
+gzip compressed data, was "joker-mongodb-0.2.0.tar", last modified: Thu Apr 25 06:00:07 2024, max compression
```

## Comparing `joker-mongodb-0.1.5.tar` & `joker-mongodb-0.2.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2022-11-25 02:16:38.949159 joker-mongodb-0.1.5/
--rw-r--r--   0 Hailong    (502) staff       (20)    35149 2021-07-11 03:40:54.000000 joker-mongodb-0.1.5/LICENSE
--rw-r--r--   0 Hailong    (502) staff       (20)       41 2021-07-11 03:42:23.000000 joker-mongodb-0.1.5/MANIFEST.in
--rw-r--r--   0 Hailong    (502) staff       (20)     2315 2022-11-25 02:16:38.948829 joker-mongodb-0.1.5/PKG-INFO
--rw-r--r--   0 Hailong    (502) staff       (20)     1574 2022-05-25 12:06:36.000000 joker-mongodb-0.1.5/README.md
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2022-11-25 02:16:38.935072 joker-mongodb-0.1.5/joker/
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2022-11-25 02:16:38.939064 joker-mongodb-0.1.5/joker/mongodb/
--rw-r--r--   0 Hailong    (502) staff       (20)      159 2022-10-28 15:27:23.000000 joker-mongodb-0.1.5/joker/mongodb/__init__.py
--rw-r--r--   0 Hailong    (502) staff       (20)     6408 2022-03-14 03:26:26.000000 joker-mongodb-0.1.5/joker/mongodb/interfaces.py
--rw-r--r--   0 Hailong    (502) staff       (20)     1873 2021-10-24 02:15:04.000000 joker-mongodb-0.1.5/joker/mongodb/legacy.py
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2022-11-25 02:16:38.944862 joker-mongodb-0.1.5/joker/mongodb/tools/
--rw-r--r--   0 Hailong    (502) staff       (20)       39 2021-07-11 03:25:17.000000 joker-mongodb-0.1.5/joker/mongodb/tools/__init__.py
--rw-r--r--   0 Hailong    (502) staff       (20)     1294 2022-01-26 16:25:20.000000 joker-mongodb-0.1.5/joker/mongodb/tools/cmdline.py
--rw-r--r--   0 Hailong    (502) staff       (20)     1081 2022-01-26 15:39:10.000000 joker-mongodb-0.1.5/joker/mongodb/tools/dumping.py
--rw-r--r--   0 Hailong    (502) staff       (20)      208 2022-03-23 11:39:14.000000 joker-mongodb-0.1.5/joker/mongodb/tools/experimental.py
--rw-r--r--   0 Hailong    (502) staff       (20)      739 2021-07-11 10:35:01.000000 joker-mongodb-0.1.5/joker/mongodb/tools/filters.py
--rw-r--r--   0 Hailong    (502) staff       (20)     1454 2021-07-15 15:19:30.000000 joker-mongodb-0.1.5/joker/mongodb/tools/integrity.py
--rw-r--r--   0 Hailong    (502) staff       (20)      639 2021-10-22 13:21:36.000000 joker-mongodb-0.1.5/joker/mongodb/tools/kvstore.py
--rw-r--r--   0 Hailong    (502) staff       (20)     9769 2021-11-24 13:07:47.000000 joker-mongodb-0.1.5/joker/mongodb/tools/misc.py
--rw-r--r--   0 Hailong    (502) staff       (20)     1053 2022-02-24 13:25:47.000000 joker-mongodb-0.1.5/joker/mongodb/tools/mongoshell.py
--rw-r--r--   0 Hailong    (502) staff       (20)     5368 2022-10-27 13:41:44.000000 joker-mongodb-0.1.5/joker/mongodb/tools/oplog.py
--rw-r--r--   0 Hailong    (502) staff       (20)     1173 2022-06-02 08:07:27.000000 joker-mongodb-0.1.5/joker/mongodb/tools/querying.py
--rw-r--r--   0 Hailong    (502) staff       (20)     3917 2022-05-25 11:59:41.000000 joker-mongodb-0.1.5/joker/mongodb/tools/schema.py
--rw-r--r--   0 Hailong    (502) staff       (20)     1160 2022-04-08 10:50:53.000000 joker-mongodb-0.1.5/joker/mongodb/tools/transactional.py
--rw-r--r--   0 Hailong    (502) staff       (20)     3695 2022-01-26 15:43:57.000000 joker-mongodb-0.1.5/joker/mongodb/utils.py
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2022-11-25 02:16:38.948309 joker-mongodb-0.1.5/joker_mongodb.egg-info/
--rw-r--r--   0 Hailong    (502) staff       (20)     2315 2022-11-25 02:16:38.000000 joker-mongodb-0.1.5/joker_mongodb.egg-info/PKG-INFO
--rw-r--r--   0 Hailong    (502) staff       (20)      837 2022-11-25 02:16:38.000000 joker-mongodb-0.1.5/joker_mongodb.egg-info/SOURCES.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        1 2022-11-25 02:16:38.000000 joker-mongodb-0.1.5/joker_mongodb.egg-info/dependency_links.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        6 2022-11-25 02:16:38.000000 joker-mongodb-0.1.5/joker_mongodb.egg-info/namespace_packages.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        1 2022-05-25 12:01:12.000000 joker-mongodb-0.1.5/joker_mongodb.egg-info/not-zip-safe
--rw-r--r--   0 Hailong    (502) staff       (20)       73 2022-11-25 02:16:38.000000 joker-mongodb-0.1.5/joker_mongodb.egg-info/requires.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        6 2022-11-25 02:16:38.000000 joker-mongodb-0.1.5/joker_mongodb.egg-info/top_level.txt
--rw-r--r--   0 Hailong    (502) staff       (20)       73 2022-04-11 13:54:28.000000 joker-mongodb-0.1.5/requirements.txt
--rw-r--r--   0 Hailong    (502) staff       (20)       38 2022-11-25 02:16:38.949262 joker-mongodb-0.1.5/setup.cfg
--rw-r--r--   0 Hailong    (502) staff       (20)     2106 2022-05-25 11:55:13.000000 joker-mongodb-0.1.5/setup.py
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-04-25 06:00:07.960088 joker-mongodb-0.2.0/
+-rw-r--r--   0 Hailong    (502) staff       (20)    35149 2021-07-11 03:40:54.000000 joker-mongodb-0.2.0/LICENSE
+-rw-r--r--   0 Hailong    (502) staff       (20)       41 2021-07-11 03:42:23.000000 joker-mongodb-0.2.0/MANIFEST.in
+-rw-r--r--   0 Hailong    (502) staff       (20)     2578 2024-04-25 06:00:07.959333 joker-mongodb-0.2.0/PKG-INFO
+-rw-r--r--   0 Hailong    (502) staff       (20)     1574 2022-05-25 12:06:36.000000 joker-mongodb-0.2.0/README.md
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-04-25 06:00:07.946801 joker-mongodb-0.2.0/joker/
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-04-25 06:00:07.949415 joker-mongodb-0.2.0/joker/mongodb/
+-rw-r--r--   0 Hailong    (502) staff       (20)      159 2024-04-25 05:56:42.000000 joker-mongodb-0.2.0/joker/mongodb/__init__.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     6408 2022-03-14 03:26:26.000000 joker-mongodb-0.2.0/joker/mongodb/interfaces.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1873 2021-10-24 02:15:04.000000 joker-mongodb-0.2.0/joker/mongodb/legacy.py
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-04-25 06:00:07.955064 joker-mongodb-0.2.0/joker/mongodb/tools/
+-rw-r--r--   0 Hailong    (502) staff       (20)       39 2021-07-11 03:25:17.000000 joker-mongodb-0.2.0/joker/mongodb/tools/__init__.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1294 2022-01-26 16:25:20.000000 joker-mongodb-0.2.0/joker/mongodb/tools/cmdline.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1081 2022-01-26 15:39:10.000000 joker-mongodb-0.2.0/joker/mongodb/tools/dumping.py
+-rw-r--r--   0 Hailong    (502) staff       (20)      208 2022-03-23 11:39:14.000000 joker-mongodb-0.2.0/joker/mongodb/tools/experimental.py
+-rw-r--r--   0 Hailong    (502) staff       (20)      739 2021-07-11 10:35:01.000000 joker-mongodb-0.2.0/joker/mongodb/tools/filters.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1454 2021-07-15 15:19:30.000000 joker-mongodb-0.2.0/joker/mongodb/tools/integrity.py
+-rw-r--r--   0 Hailong    (502) staff       (20)      639 2021-10-22 13:21:36.000000 joker-mongodb-0.2.0/joker/mongodb/tools/kvstore.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     9769 2021-11-24 13:07:47.000000 joker-mongodb-0.2.0/joker/mongodb/tools/misc.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1053 2022-02-24 13:25:47.000000 joker-mongodb-0.2.0/joker/mongodb/tools/mongoshell.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     5473 2022-12-02 03:57:24.000000 joker-mongodb-0.2.0/joker/mongodb/tools/oplog.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1173 2022-06-02 08:07:27.000000 joker-mongodb-0.2.0/joker/mongodb/tools/querying.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     3917 2022-05-25 11:59:41.000000 joker-mongodb-0.2.0/joker/mongodb/tools/schema.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1160 2022-04-08 10:50:53.000000 joker-mongodb-0.2.0/joker/mongodb/tools/transactional.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     3695 2022-01-26 15:43:57.000000 joker-mongodb-0.2.0/joker/mongodb/utils.py
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-04-25 06:00:07.958551 joker-mongodb-0.2.0/joker_mongodb.egg-info/
+-rw-r--r--   0 Hailong    (502) staff       (20)     2578 2024-04-25 06:00:07.000000 joker-mongodb-0.2.0/joker_mongodb.egg-info/PKG-INFO
+-rw-r--r--   0 Hailong    (502) staff       (20)      837 2024-04-25 06:00:07.000000 joker-mongodb-0.2.0/joker_mongodb.egg-info/SOURCES.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        1 2024-04-25 06:00:07.000000 joker-mongodb-0.2.0/joker_mongodb.egg-info/dependency_links.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        6 2024-04-25 06:00:07.000000 joker-mongodb-0.2.0/joker_mongodb.egg-info/namespace_packages.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        1 2022-05-25 12:01:12.000000 joker-mongodb-0.2.0/joker_mongodb.egg-info/not-zip-safe
+-rw-r--r--   0 Hailong    (502) staff       (20)       86 2024-04-25 06:00:07.000000 joker-mongodb-0.2.0/joker_mongodb.egg-info/requires.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        6 2024-04-25 06:00:07.000000 joker-mongodb-0.2.0/joker_mongodb.egg-info/top_level.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)       86 2024-04-25 05:57:29.000000 joker-mongodb-0.2.0/requirements.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)       38 2024-04-25 06:00:07.960228 joker-mongodb-0.2.0/setup.cfg
+-rw-r--r--   0 Hailong    (502) staff       (20)     2205 2024-04-25 05:58:45.000000 joker-mongodb-0.2.0/setup.py
```

### Comparing `joker-mongodb-0.1.5/LICENSE` & `joker-mongodb-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `joker-mongodb-0.1.5/PKG-INFO` & `joker-mongodb-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 Metadata-Version: 2.1
 Name: joker-mongodb
-Version: 0.1.5
+Version: 0.2.0
 Summary: access mongodb with handy utilities and fun
 Home-page: https://github.com/frozflame/joker-mongodb
 Author: frozflame
 Author-email: frozflame@outlook.com
 License: GNU General Public License (GPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: joker-cast>=0.5.0
+Requires-Dist: joker-textmanip>=0.3.1
+Requires-Dist: joker>=0.3.3
+Requires-Dist: pymongo>=3.11.0
+Requires-Dist: volkanic>=0.5.1
 
 joker-mongodb
 =============
 
 Access mongodb with handy utilities and fun.
 
 ## Connnect to multiple mongo servers with MongoInterface
```

### Comparing `joker-mongodb-0.1.5/README.md` & `joker-mongodb-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `joker-mongodb-0.1.5/joker/mongodb/interfaces.py` & `joker-mongodb-0.2.0/joker/mongodb/interfaces.py`

 * *Files identical despite different names*

### Comparing `joker-mongodb-0.1.5/joker/mongodb/legacy.py` & `joker-mongodb-0.2.0/joker/mongodb/legacy.py`

 * *Files identical despite different names*

### Comparing `joker-mongodb-0.1.5/joker/mongodb/tools/cmdline.py` & `joker-mongodb-0.2.0/joker/mongodb/tools/cmdline.py`

 * *Files identical despite different names*

### Comparing `joker-mongodb-0.1.5/joker/mongodb/tools/dumping.py` & `joker-mongodb-0.2.0/joker/mongodb/tools/dumping.py`

 * *Files identical despite different names*

### Comparing `joker-mongodb-0.1.5/joker/mongodb/tools/filters.py` & `joker-mongodb-0.2.0/joker/mongodb/tools/filters.py`

 * *Files identical despite different names*

### Comparing `joker-mongodb-0.1.5/joker/mongodb/tools/integrity.py` & `joker-mongodb-0.2.0/joker/mongodb/tools/integrity.py`

 * *Files identical despite different names*

### Comparing `joker-mongodb-0.1.5/joker/mongodb/tools/kvstore.py` & `joker-mongodb-0.2.0/joker/mongodb/tools/kvstore.py`

 * *Files identical despite different names*

### Comparing `joker-mongodb-0.1.5/joker/mongodb/tools/misc.py` & `joker-mongodb-0.2.0/joker/mongodb/tools/misc.py`

 * *Files identical despite different names*

### Comparing `joker-mongodb-0.1.5/joker/mongodb/tools/mongoshell.py` & `joker-mongodb-0.2.0/joker/mongodb/tools/mongoshell.py`

 * *Files identical despite different names*

### Comparing `joker-mongodb-0.1.5/joker/mongodb/tools/oplog.py` & `joker-mongodb-0.2.0/joker/mongodb/tools/oplog.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 # coding: utf-8
 from __future__ import annotations
 
 import logging
 import threading
 import time
+import traceback
 from collections import UserDict
 from collections import defaultdict
 from typing import Callable
 
 import pymongo
 from bson import Timestamp, json_util, ObjectId
 from pymongo import MongoClient
@@ -147,32 +148,36 @@
 
 class ChangeStreamRegistry:
     def __init__(self, db: Database):
         self.db = db
         self.handlers = defaultdict(list)
 
     @staticmethod
-    def _log_handling(coll_name: str, handler: Callable, record: dict):
+    def apply(handler: Callable, coll_name: str, event: dict):
         try:
-            id_ = record['documentKey']['_id']
+            id_ = event['documentKey']['_id']
         except KeyError:
             id_ = None
         _logger.info(
             'applying %s() to change event of collection %r, %s',
             getattr(handler, '__name__', None) or str(handler),
             coll_name, id_
         )
+        # noinspection PyBroadException
+        try:
+            handler(event)
+        except Exception:
+            traceback.print_exc()
 
     def watch(self, coll_name: str):
         coll = self.db[coll_name]
         cursor = coll.watch()
-        for record in cursor:
+        for event in cursor:
             for handler in self.handlers.get(coll_name):
-                self._log_handling(coll_name, handler, record)
-                handler(record)
+                self.apply(handler, coll_name, event)
 
     def register(self, coll_name: str, handler: Callable):
         self.handlers[coll_name].append(handler)
 
     def execute(self):
         threads = []
         for coll_name, handlers in self.handlers.items():
```

### Comparing `joker-mongodb-0.1.5/joker/mongodb/tools/querying.py` & `joker-mongodb-0.2.0/joker/mongodb/tools/querying.py`

 * *Files identical despite different names*

### Comparing `joker-mongodb-0.1.5/joker/mongodb/tools/schema.py` & `joker-mongodb-0.2.0/joker/mongodb/tools/schema.py`

 * *Files identical despite different names*

### Comparing `joker-mongodb-0.1.5/joker/mongodb/tools/transactional.py` & `joker-mongodb-0.2.0/joker/mongodb/tools/transactional.py`

 * *Files identical despite different names*

### Comparing `joker-mongodb-0.1.5/joker/mongodb/utils.py` & `joker-mongodb-0.2.0/joker/mongodb/utils.py`

 * *Files identical despite different names*

### Comparing `joker-mongodb-0.1.5/joker_mongodb.egg-info/PKG-INFO` & `joker-mongodb-0.2.0/joker_mongodb.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 Metadata-Version: 2.1
 Name: joker-mongodb
-Version: 0.1.5
+Version: 0.2.0
 Summary: access mongodb with handy utilities and fun
 Home-page: https://github.com/frozflame/joker-mongodb
 Author: frozflame
 Author-email: frozflame@outlook.com
 License: GNU General Public License (GPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: joker-cast>=0.5.0
+Requires-Dist: joker-textmanip>=0.3.1
+Requires-Dist: joker>=0.3.3
+Requires-Dist: pymongo>=3.11.0
+Requires-Dist: volkanic>=0.5.1
 
 joker-mongodb
 =============
 
 Access mongodb with handy utilities and fun.
 
 ## Connnect to multiple mongo servers with MongoInterface
```

### Comparing `joker-mongodb-0.1.5/joker_mongodb.egg-info/SOURCES.txt` & `joker-mongodb-0.2.0/joker_mongodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `joker-mongodb-0.1.5/setup.py` & `joker-mongodb-0.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 #!/usr/bin/env python3
 # coding: utf-8
-
 import os
 import re
 
 import setuptools
 from setuptools import find_namespace_packages
 
 # CAUTION:
@@ -57,14 +56,16 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
+        "Programming Language :: Python :: 3.13",
     ],
     # ensure copy static file to runtime directory
     "include_package_data": True,
     "long_description": read("README.md"),
     "long_description_content_type": "text/markdown",
 }
```

