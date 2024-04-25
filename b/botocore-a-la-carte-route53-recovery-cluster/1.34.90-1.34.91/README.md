# Comparing `tmp/botocore-a-la-carte-route53-recovery-cluster-1.34.90.tar.gz` & `tmp/botocore-a-la-carte-route53-recovery-cluster-1.34.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-route53-recovery-cluster-1.34.90.tar", last modified: Wed Apr 24 01:02:27 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-route53-recovery-cluster-1.34.91.tar", last modified: Thu Apr 25 01:03:52 2024, max compression
```

## Comparing `botocore-a-la-carte-route53-recovery-cluster-1.34.90.tar` & `botocore-a-la-carte-route53-recovery-cluster-1.34.91.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:02:27.210587 botocore-a-la-carte-route53-recovery-cluster-1.34.90/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-24 01:02:26.000000 botocore-a-la-carte-route53-recovery-cluster-1.34.90/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-24 01:02:27.210587 botocore-a-la-carte-route53-recovery-cluster-1.34.90/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:02:27.206587 botocore-a-la-carte-route53-recovery-cluster-1.34.90/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:02:27.206587 botocore-a-la-carte-route53-recovery-cluster-1.34.90/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:02:27.206587 botocore-a-la-carte-route53-recovery-cluster-1.34.90/botocore/data/route53-recovery-cluster/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:02:27.206587 botocore-a-la-carte-route53-recovery-cluster-1.34.90/botocore/data/route53-recovery-cluster/2019-12-02/
--rw-r--r--   0 runner    (1001) docker     (127)    13798 2024-04-24 01:01:50.000000 botocore-a-la-carte-route53-recovery-cluster-1.34.90/botocore/data/route53-recovery-cluster/2019-12-02/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-24 01:01:50.000000 botocore-a-la-carte-route53-recovery-cluster-1.34.90/botocore/data/route53-recovery-cluster/2019-12-02/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-24 01:01:50.000000 botocore-a-la-carte-route53-recovery-cluster-1.34.90/botocore/data/route53-recovery-cluster/2019-12-02/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    26304 2024-04-24 01:01:50.000000 botocore-a-la-carte-route53-recovery-cluster-1.34.90/botocore/data/route53-recovery-cluster/2019-12-02/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:02:27.210587 botocore-a-la-carte-route53-recovery-cluster-1.34.90/botocore_a_la_carte_route53_recovery_cluster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-24 01:02:27.000000 botocore-a-la-carte-route53-recovery-cluster-1.34.90/botocore_a_la_carte_route53_recovery_cluster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-24 01:02:27.000000 botocore-a-la-carte-route53-recovery-cluster-1.34.90/botocore_a_la_carte_route53_recovery_cluster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 01:02:27.000000 botocore-a-la-carte-route53-recovery-cluster-1.34.90/botocore_a_la_carte_route53_recovery_cluster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 01:02:27.000000 botocore-a-la-carte-route53-recovery-cluster-1.34.90/botocore_a_la_carte_route53_recovery_cluster.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 01:02:27.210587 botocore-a-la-carte-route53-recovery-cluster-1.34.90/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-24 01:02:26.000000 botocore-a-la-carte-route53-recovery-cluster-1.34.90/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:03:52.851641 botocore-a-la-carte-route53-recovery-cluster-1.34.91/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-25 01:03:52.000000 botocore-a-la-carte-route53-recovery-cluster-1.34.91/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-25 01:03:52.847641 botocore-a-la-carte-route53-recovery-cluster-1.34.91/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:03:52.847641 botocore-a-la-carte-route53-recovery-cluster-1.34.91/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:03:52.847641 botocore-a-la-carte-route53-recovery-cluster-1.34.91/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:03:52.847641 botocore-a-la-carte-route53-recovery-cluster-1.34.91/botocore/data/route53-recovery-cluster/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:03:52.847641 botocore-a-la-carte-route53-recovery-cluster-1.34.91/botocore/data/route53-recovery-cluster/2019-12-02/
+-rw-r--r--   0 runner    (1001) docker     (127)    13798 2024-04-25 01:03:19.000000 botocore-a-la-carte-route53-recovery-cluster-1.34.91/botocore/data/route53-recovery-cluster/2019-12-02/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-25 01:03:19.000000 botocore-a-la-carte-route53-recovery-cluster-1.34.91/botocore/data/route53-recovery-cluster/2019-12-02/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-25 01:03:19.000000 botocore-a-la-carte-route53-recovery-cluster-1.34.91/botocore/data/route53-recovery-cluster/2019-12-02/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    26304 2024-04-25 01:03:19.000000 botocore-a-la-carte-route53-recovery-cluster-1.34.91/botocore/data/route53-recovery-cluster/2019-12-02/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:03:52.847641 botocore-a-la-carte-route53-recovery-cluster-1.34.91/botocore_a_la_carte_route53_recovery_cluster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-25 01:03:52.000000 botocore-a-la-carte-route53-recovery-cluster-1.34.91/botocore_a_la_carte_route53_recovery_cluster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-25 01:03:52.000000 botocore-a-la-carte-route53-recovery-cluster-1.34.91/botocore_a_la_carte_route53_recovery_cluster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 01:03:52.000000 botocore-a-la-carte-route53-recovery-cluster-1.34.91/botocore_a_la_carte_route53_recovery_cluster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 01:03:52.000000 botocore-a-la-carte-route53-recovery-cluster-1.34.91/botocore_a_la_carte_route53_recovery_cluster.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 01:03:52.851641 botocore-a-la-carte-route53-recovery-cluster-1.34.91/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-25 01:03:52.000000 botocore-a-la-carte-route53-recovery-cluster-1.34.91/setup.py
```

### Comparing `botocore-a-la-carte-route53-recovery-cluster-1.34.90/LICENSE.txt` & `botocore-a-la-carte-route53-recovery-cluster-1.34.91/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-route53-recovery-cluster-1.34.90/PKG-INFO` & `botocore-a-la-carte-route53-recovery-cluster-1.34.91/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-route53-recovery-cluster
-Version: 1.34.90
+Version: 1.34.91
 Summary: route53-recovery-cluster data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-route53-recovery-cluster-1.34.90/botocore/data/route53-recovery-cluster/2019-12-02/endpoint-rule-set-1.json` & `botocore-a-la-carte-route53-recovery-cluster-1.34.91/botocore/data/route53-recovery-cluster/2019-12-02/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-route53-recovery-cluster-1.34.90/botocore/data/route53-recovery-cluster/2019-12-02/service-2.json` & `botocore-a-la-carte-route53-recovery-cluster-1.34.91/botocore/data/route53-recovery-cluster/2019-12-02/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-route53-recovery-cluster-1.34.90/botocore_a_la_carte_route53_recovery_cluster.egg-info/PKG-INFO` & `botocore-a-la-carte-route53-recovery-cluster-1.34.91/botocore_a_la_carte_route53_recovery_cluster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-route53-recovery-cluster
-Version: 1.34.90
+Version: 1.34.91
 Summary: route53-recovery-cluster data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-route53-recovery-cluster-1.34.90/botocore_a_la_carte_route53_recovery_cluster.egg-info/SOURCES.txt` & `botocore-a-la-carte-route53-recovery-cluster-1.34.91/botocore_a_la_carte_route53_recovery_cluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-route53-recovery-cluster-1.34.90/setup.py` & `botocore-a-la-carte-route53-recovery-cluster-1.34.91/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-route53-recovery-cluster',
-    version="1.34.90",
+    version="1.34.91",
     description='route53-recovery-cluster data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/route53-recovery-cluster/*/*.json'],
```

