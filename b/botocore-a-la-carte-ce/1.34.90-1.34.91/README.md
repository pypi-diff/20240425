# Comparing `tmp/botocore-a-la-carte-ce-1.34.90.tar.gz` & `tmp/botocore-a-la-carte-ce-1.34.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-ce-1.34.90.tar", last modified: Wed Apr 24 01:02:03 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-ce-1.34.91.tar", last modified: Thu Apr 25 01:03:29 2024, max compression
```

## Comparing `botocore-a-la-carte-ce-1.34.90.tar` & `botocore-a-la-carte-ce-1.34.91.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:02:03.542605 botocore-a-la-carte-ce-1.34.90/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-24 01:02:03.000000 botocore-a-la-carte-ce-1.34.90/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-24 01:02:03.542605 botocore-a-la-carte-ce-1.34.90/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:02:03.542605 botocore-a-la-carte-ce-1.34.90/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:02:03.542605 botocore-a-la-carte-ce-1.34.90/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:02:03.542605 botocore-a-la-carte-ce-1.34.90/botocore/data/ce/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:02:03.542605 botocore-a-la-carte-ce-1.34.90/botocore/data/ce/2017-10-25/
--rw-r--r--   0 runner    (1001) docker     (127)    18478 2024-04-24 01:01:50.000000 botocore-a-la-carte-ce-1.34.90/botocore/data/ce/2017-10-25/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-24 01:01:50.000000 botocore-a-la-carte-ce-1.34.90/botocore/data/ce/2017-10-25/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-24 01:01:50.000000 botocore-a-la-carte-ce-1.34.90/botocore/data/ce/2017-10-25/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   271813 2024-04-24 01:01:50.000000 botocore-a-la-carte-ce-1.34.90/botocore/data/ce/2017-10-25/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:02:03.542605 botocore-a-la-carte-ce-1.34.90/botocore_a_la_carte_ce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-24 01:02:03.000000 botocore-a-la-carte-ce-1.34.90/botocore_a_la_carte_ce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-24 01:02:03.000000 botocore-a-la-carte-ce-1.34.90/botocore_a_la_carte_ce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 01:02:03.000000 botocore-a-la-carte-ce-1.34.90/botocore_a_la_carte_ce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 01:02:03.000000 botocore-a-la-carte-ce-1.34.90/botocore_a_la_carte_ce.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 01:02:03.542605 botocore-a-la-carte-ce-1.34.90/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-24 01:02:03.000000 botocore-a-la-carte-ce-1.34.90/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:03:29.751457 botocore-a-la-carte-ce-1.34.91/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-25 01:03:29.000000 botocore-a-la-carte-ce-1.34.91/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-25 01:03:29.751457 botocore-a-la-carte-ce-1.34.91/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:03:29.751457 botocore-a-la-carte-ce-1.34.91/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:03:29.751457 botocore-a-la-carte-ce-1.34.91/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:03:29.751457 botocore-a-la-carte-ce-1.34.91/botocore/data/ce/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:03:29.751457 botocore-a-la-carte-ce-1.34.91/botocore/data/ce/2017-10-25/
+-rw-r--r--   0 runner    (1001) docker     (127)    18478 2024-04-25 01:03:19.000000 botocore-a-la-carte-ce-1.34.91/botocore/data/ce/2017-10-25/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-25 01:03:19.000000 botocore-a-la-carte-ce-1.34.91/botocore/data/ce/2017-10-25/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-25 01:03:19.000000 botocore-a-la-carte-ce-1.34.91/botocore/data/ce/2017-10-25/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   271813 2024-04-25 01:03:19.000000 botocore-a-la-carte-ce-1.34.91/botocore/data/ce/2017-10-25/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:03:29.751457 botocore-a-la-carte-ce-1.34.91/botocore_a_la_carte_ce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-25 01:03:29.000000 botocore-a-la-carte-ce-1.34.91/botocore_a_la_carte_ce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-25 01:03:29.000000 botocore-a-la-carte-ce-1.34.91/botocore_a_la_carte_ce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 01:03:29.000000 botocore-a-la-carte-ce-1.34.91/botocore_a_la_carte_ce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 01:03:29.000000 botocore-a-la-carte-ce-1.34.91/botocore_a_la_carte_ce.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 01:03:29.751457 botocore-a-la-carte-ce-1.34.91/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-25 01:03:29.000000 botocore-a-la-carte-ce-1.34.91/setup.py
```

### Comparing `botocore-a-la-carte-ce-1.34.90/LICENSE.txt` & `botocore-a-la-carte-ce-1.34.91/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ce-1.34.90/PKG-INFO` & `botocore-a-la-carte-ce-1.34.91/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-ce
-Version: 1.34.90
+Version: 1.34.91
 Summary: ce data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-ce-1.34.90/botocore/data/ce/2017-10-25/endpoint-rule-set-1.json` & `botocore-a-la-carte-ce-1.34.91/botocore/data/ce/2017-10-25/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ce-1.34.90/botocore/data/ce/2017-10-25/service-2.json` & `botocore-a-la-carte-ce-1.34.91/botocore/data/ce/2017-10-25/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ce-1.34.90/botocore_a_la_carte_ce.egg-info/PKG-INFO` & `botocore-a-la-carte-ce-1.34.91/botocore_a_la_carte_ce.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-ce
-Version: 1.34.90
+Version: 1.34.91
 Summary: ce data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-ce-1.34.90/setup.py` & `botocore-a-la-carte-ce-1.34.91/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-ce',
-    version="1.34.90",
+    version="1.34.91",
     description='ce data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/ce/*/*.json'],
```

