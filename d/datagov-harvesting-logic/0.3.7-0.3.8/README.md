# Comparing `tmp/datagov_harvesting_logic-0.3.7.tar.gz` & `tmp/datagov_harvesting_logic-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datagov_harvesting_logic-0.3.7.tar", max compression
+gzip compressed data, was "datagov_harvesting_logic-0.3.8.tar", max compression
```

## Comparing `datagov_harvesting_logic-0.3.7.tar` & `datagov_harvesting_logic-0.3.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1878 2024-04-24 14:59:01.131058 datagov_harvesting_logic-0.3.7/LICENSE.md
--rw-r--r--   0        0        0     5265 2024-04-24 14:59:01.131058 datagov_harvesting_logic-0.3.7/README.md
--rw-r--r--   0        0        0      162 2024-04-24 14:59:01.135058 datagov_harvesting_logic-0.3.7/harvester/__init__.py
--rw-r--r--   0        0        0     4489 2024-04-24 14:59:01.135058 datagov_harvesting_logic-0.3.7/harvester/ckan_utils.py
--rw-r--r--   0        0        0     4464 2024-04-24 14:59:01.135058 datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/arm.data.json
--rw-r--r--   0        0        0     7830 2024-04-24 14:59:01.135058 datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/collection-1-parent-2-children.data.json
--rw-r--r--   0        0        0    14027 2024-04-24 14:59:01.135058 datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/collection-2-parent-4-children.data.json
--rw-r--r--   0        0        0     7454 2024-04-24 14:59:01.135058 datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/geospatial.data.json
--rw-r--r--   0        0        0   310979 2024-04-24 14:59:01.139058 datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/large-spatial.data.json
--rw-r--r--   0        0        0      918 2024-04-24 14:59:01.139058 datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/missing-catalog.data.json
--rw-r--r--   0        0        0     1059 2024-04-24 14:59:01.139058 datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/missing-dataset-fields.data.json
--rw-r--r--   0        0        0     3259 2024-04-24 14:59:01.139058 datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/missing-identifier-title.data.json
--rw-r--r--   0        0        0     1292 2024-04-24 14:59:01.139058 datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/numerical-title.data.json
--rw-r--r--   0        0        0     2520 2024-04-24 14:59:01.139058 datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/ny.data.json
--rw-r--r--   0        0        0     1314 2024-04-24 14:59:01.139058 datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/reserved-title.data.json
--rw-r--r--   0        0        0     9562 2024-04-24 14:59:01.139058 datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/usda.gov.data.json
--rw-r--r--   0        0        0     1604 2024-04-24 14:59:01.139058 datagov_harvesting_logic-0.3.7/harvester/data/dcatus/schemas/catalog.json
--rw-r--r--   0        0        0    23811 2024-04-24 14:59:01.139058 datagov_harvesting_logic-0.3.7/harvester/data/dcatus/schemas/dataset.json
--rw-r--r--   0        0        0     2158 2024-04-24 14:59:01.139058 datagov_harvesting_logic-0.3.7/harvester/exceptions.py
--rw-r--r--   0        0        0    25444 2024-04-24 14:59:01.139058 datagov_harvesting_logic-0.3.7/harvester/harvest.py
--rw-r--r--   0        0        0      589 2024-04-24 14:59:01.139058 datagov_harvesting_logic-0.3.7/harvester/logger_config.py
--rw-r--r--   0        0        0     3632 2024-04-24 14:59:01.139058 datagov_harvesting_logic-0.3.7/harvester/utils.py
--rw-r--r--   0        0        0     2241 2024-04-24 14:59:01.139058 datagov_harvesting_logic-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     6582 1970-01-01 00:00:00.000000 datagov_harvesting_logic-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1878 2024-04-24 21:07:10.203062 datagov_harvesting_logic-0.3.8/LICENSE.md
+-rw-r--r--   0        0        0     5265 2024-04-24 21:07:10.203062 datagov_harvesting_logic-0.3.8/README.md
+-rw-r--r--   0        0        0      162 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/__init__.py
+-rw-r--r--   0        0        0     4489 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/ckan_utils.py
+-rw-r--r--   0        0        0     4464 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/arm.data.json
+-rw-r--r--   0        0        0     7830 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/collection-1-parent-2-children.data.json
+-rw-r--r--   0        0        0    14027 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/collection-2-parent-4-children.data.json
+-rw-r--r--   0        0        0     7454 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/geospatial.data.json
+-rw-r--r--   0        0        0   310979 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/large-spatial.data.json
+-rw-r--r--   0        0        0      918 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/missing-catalog.data.json
+-rw-r--r--   0        0        0     1059 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/missing-dataset-fields.data.json
+-rw-r--r--   0        0        0     3259 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/missing-identifier-title.data.json
+-rw-r--r--   0        0        0     1292 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/numerical-title.data.json
+-rw-r--r--   0        0        0     2520 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/ny.data.json
+-rw-r--r--   0        0        0     1314 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/reserved-title.data.json
+-rw-r--r--   0        0        0     9562 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/usda.gov.data.json
+-rw-r--r--   0        0        0     1604 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/data/dcatus/schemas/catalog.json
+-rw-r--r--   0        0        0    23811 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/data/dcatus/schemas/dataset.json
+-rw-r--r--   0        0        0     2158 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/exceptions.py
+-rw-r--r--   0        0        0    25444 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/harvest.py
+-rw-r--r--   0        0        0      589 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/logger_config.py
+-rw-r--r--   0        0        0     3859 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/utils.py
+-rw-r--r--   0        0        0     2241 2024-04-24 21:07:10.215062 datagov_harvesting_logic-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     6582 1970-01-01 00:00:00.000000 datagov_harvesting_logic-0.3.8/PKG-INFO
```

### Comparing `datagov_harvesting_logic-0.3.7/LICENSE.md` & `datagov_harvesting_logic-0.3.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.7/README.md` & `datagov_harvesting_logic-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.7/harvester/ckan_utils.py` & `datagov_harvesting_logic-0.3.8/harvester/ckan_utils.py`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/arm.data.json` & `datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/arm.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/collection-1-parent-2-children.data.json` & `datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/collection-1-parent-2-children.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/collection-2-parent-4-children.data.json` & `datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/collection-2-parent-4-children.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/geospatial.data.json` & `datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/geospatial.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/large-spatial.data.json` & `datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/large-spatial.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/missing-catalog.data.json` & `datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/missing-catalog.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/missing-dataset-fields.data.json` & `datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/missing-dataset-fields.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/missing-identifier-title.data.json` & `datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/missing-identifier-title.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/numerical-title.data.json` & `datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/numerical-title.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/ny.data.json` & `datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/ny.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/reserved-title.data.json` & `datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/reserved-title.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/usda.gov.data.json` & `datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/usda.gov.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.7/harvester/data/dcatus/schemas/catalog.json` & `datagov_harvesting_logic-0.3.8/harvester/data/dcatus/schemas/catalog.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.7/harvester/data/dcatus/schemas/dataset.json` & `datagov_harvesting_logic-0.3.8/harvester/data/dcatus/schemas/dataset.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.7/harvester/exceptions.py` & `datagov_harvesting_logic-0.3.8/harvester/exceptions.py`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.7/harvester/harvest.py` & `datagov_harvesting_logic-0.3.8/harvester/harvest.py`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.7/harvester/logger_config.py` & `datagov_harvesting_logic-0.3.8/harvester/logger_config.py`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.7/harvester/utils.py` & `datagov_harvesting_logic-0.3.8/harvester/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,31 @@
 import hashlib
 import json
 import os
+import argparse
 
 import boto3
 import sansjson
 
 from cloudfoundry_client.client import CloudFoundryClient
 from cloudfoundry_client.v3.tasks import TaskManager
 
 # ruff: noqa: F841
 
 
+def parse_args(args):
+
+    parser = argparse.ArgumentParser(
+        prog="Harvest Runner", description="etl harvest sources"
+    )
+    parser.add_argument("-j", "--jobid")
+
+    return parser.parse_args(args)
+
+
 def convert_set_to_list(obj):
     if isinstance(obj, set):
         return list(obj)
     raise TypeError
 
 
 def sort_dataset(d):
```

### Comparing `datagov_harvesting_logic-0.3.7/pyproject.toml` & `datagov_harvesting_logic-0.3.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datagov-harvesting-logic"
-version = "0.3.7"
+version = "0.3.8"
 description = ""
 # authors = [
 #     {name = "Jin Sun", email = "jin.sun@gsa.gov"},
 #     {name = "Tyler Burton", email = "tyler.burton@gsa.gov"},
 # ]
 authors = [
     "Datagov Team <datagov@gsa.gov>",
```

### Comparing `datagov_harvesting_logic-0.3.7/PKG-INFO` & `datagov_harvesting_logic-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datagov-harvesting-logic
-Version: 0.3.7
+Version: 0.3.8
 Summary: 
 Home-page: https://github.com/GSA/datagov-harvesting-logic
 License: LICENSE.md
 Author: Datagov Team
 Author-email: datagov@gsa.gov
 Maintainer: Datagov Team
 Maintainer-email: datagov@gsa.gov
```

