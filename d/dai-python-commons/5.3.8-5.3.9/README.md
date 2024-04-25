# Comparing `tmp/dai_python_commons-5.3.8.tar.gz` & `tmp/dai_python_commons-5.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dai_python_commons-5.3.8.tar", max compression
+gzip compressed data, was "dai_python_commons-5.3.9.tar", max compression
```

## Comparing `dai_python_commons-5.3.8.tar` & `dai_python_commons-5.3.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      108 2023-09-01 08:20:54.663194 dai_python_commons-5.3.8/dai_python_commons/__init__.py
--rw-r--r--   0        0        0     1522 2023-09-01 08:20:54.663194 dai_python_commons-5.3.8/dai_python_commons/cdk_utils.py
--rw-r--r--   0        0        0     1386 2023-09-01 08:20:54.663194 dai_python_commons-5.3.8/dai_python_commons/cloudwatch_utils.py
--rw-r--r--   0        0        0     4466 2023-09-01 08:20:54.663194 dai_python_commons-5.3.8/dai_python_commons/dai_error.py
--rw-r--r--   0        0        0     2524 2023-09-01 08:20:54.663194 dai_python_commons-5.3.8/dai_python_commons/event_bridge.py
--rw-r--r--   0        0        0     5328 2023-09-01 08:20:54.663194 dai_python_commons-5.3.8/dai_python_commons/glue_utils.py
--rw-r--r--   0        0        0     1834 2023-09-01 08:20:54.663194 dai_python_commons-5.3.8/dai_python_commons/logging_utils.py
--rw-r--r--   0        0        0    14069 2023-09-01 08:20:54.667194 dai_python_commons-5.3.8/dai_python_commons/parquet_utils.py
--rw-r--r--   0        0        0    24467 2023-09-01 08:20:54.667194 dai_python_commons-5.3.8/dai_python_commons/s3_event_object_copy.py
--rw-r--r--   0        0        0     8170 2023-09-01 08:20:54.667194 dai_python_commons-5.3.8/dai_python_commons/s3_utils.py
--rw-r--r--   0        0        0     2441 2023-09-01 08:20:54.667194 dai_python_commons-5.3.8/dai_python_commons/time_utils.py
--rw-r--r--   0        0        0      889 2023-09-01 08:20:54.667194 dai_python_commons-5.3.8/pyproject.toml
--rw-r--r--   0        0        0      943 1970-01-01 00:00:00.000000 dai_python_commons-5.3.8/setup.py
--rw-r--r--   0        0        0      691 1970-01-01 00:00:00.000000 dai_python_commons-5.3.8/PKG-INFO
+-rw-r--r--   0        0        0      108 2023-09-01 09:05:51.957382 dai_python_commons-5.3.9/dai_python_commons/__init__.py
+-rw-r--r--   0        0        0     1522 2023-09-01 09:05:51.957382 dai_python_commons-5.3.9/dai_python_commons/cdk_utils.py
+-rw-r--r--   0        0        0     1386 2023-09-01 09:05:51.957382 dai_python_commons-5.3.9/dai_python_commons/cloudwatch_utils.py
+-rw-r--r--   0        0        0     4466 2023-09-01 09:05:51.961382 dai_python_commons-5.3.9/dai_python_commons/dai_error.py
+-rw-r--r--   0        0        0     2524 2023-09-01 09:05:51.961382 dai_python_commons-5.3.9/dai_python_commons/event_bridge.py
+-rw-r--r--   0        0        0     5328 2023-09-01 09:05:51.961382 dai_python_commons-5.3.9/dai_python_commons/glue_utils.py
+-rw-r--r--   0        0        0     1834 2023-09-01 09:05:51.961382 dai_python_commons-5.3.9/dai_python_commons/logging_utils.py
+-rw-r--r--   0        0        0    14069 2023-09-01 09:05:51.961382 dai_python_commons-5.3.9/dai_python_commons/parquet_utils.py
+-rw-r--r--   0        0        0    24467 2023-09-01 09:05:51.961382 dai_python_commons-5.3.9/dai_python_commons/s3_event_object_copy.py
+-rw-r--r--   0        0        0     8170 2023-09-01 09:05:51.961382 dai_python_commons-5.3.9/dai_python_commons/s3_utils.py
+-rw-r--r--   0        0        0     2441 2023-09-01 09:05:51.961382 dai_python_commons-5.3.9/dai_python_commons/time_utils.py
+-rw-r--r--   0        0        0      889 2023-09-01 09:05:51.961382 dai_python_commons-5.3.9/pyproject.toml
+-rw-r--r--   0        0        0      943 1970-01-01 00:00:00.000000 dai_python_commons-5.3.9/setup.py
+-rw-r--r--   0        0        0      691 1970-01-01 00:00:00.000000 dai_python_commons-5.3.9/PKG-INFO
```

### Comparing `dai_python_commons-5.3.8/dai_python_commons/cdk_utils.py` & `dai_python_commons-5.3.9/dai_python_commons/cdk_utils.py`

 * *Files identical despite different names*

### Comparing `dai_python_commons-5.3.8/dai_python_commons/cloudwatch_utils.py` & `dai_python_commons-5.3.9/dai_python_commons/cloudwatch_utils.py`

 * *Files identical despite different names*

### Comparing `dai_python_commons-5.3.8/dai_python_commons/dai_error.py` & `dai_python_commons-5.3.9/dai_python_commons/dai_error.py`

 * *Files identical despite different names*

### Comparing `dai_python_commons-5.3.8/dai_python_commons/event_bridge.py` & `dai_python_commons-5.3.9/dai_python_commons/event_bridge.py`

 * *Files identical despite different names*

### Comparing `dai_python_commons-5.3.8/dai_python_commons/glue_utils.py` & `dai_python_commons-5.3.9/dai_python_commons/glue_utils.py`

 * *Files identical despite different names*

### Comparing `dai_python_commons-5.3.8/dai_python_commons/logging_utils.py` & `dai_python_commons-5.3.9/dai_python_commons/logging_utils.py`

 * *Files identical despite different names*

### Comparing `dai_python_commons-5.3.8/dai_python_commons/parquet_utils.py` & `dai_python_commons-5.3.9/dai_python_commons/parquet_utils.py`

 * *Files identical despite different names*

### Comparing `dai_python_commons-5.3.8/dai_python_commons/s3_event_object_copy.py` & `dai_python_commons-5.3.9/dai_python_commons/s3_event_object_copy.py`

 * *Files identical despite different names*

### Comparing `dai_python_commons-5.3.8/dai_python_commons/s3_utils.py` & `dai_python_commons-5.3.9/dai_python_commons/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dai_python_commons-5.3.8/dai_python_commons/time_utils.py` & `dai_python_commons-5.3.9/dai_python_commons/time_utils.py`

 * *Files identical despite different names*

### Comparing `dai_python_commons-5.3.8/pyproject.toml` & `dai_python_commons-5.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dai-python-commons"
-version = "5.3.8"
+version = "5.3.9"
 description = "Collection of small python utilities useful for lambda functions or glue jobs. By the Stockholm Public Transport Administration."
 authors = []
 
 [tool.poetry.dependencies]
 python = "~3.10"
 loguru = "^0.7.0"
 boto3 = "^1.26.0"
```

### Comparing `dai_python_commons-5.3.8/setup.py` & `dai_python_commons-5.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 extras_require = \
 {'data-consolidation': ['polars==0.18.8'],
  'glue': ['awswrangler==3.2.1', 'cryptography==41.0.2']}
 
 setup_kwargs = {
     'name': 'dai-python-commons',
-    'version': '5.3.8',
+    'version': '5.3.9',
     'description': 'Collection of small python utilities useful for lambda functions or glue jobs. By the Stockholm Public Transport Administration.',
     'long_description': 'None',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `dai_python_commons-5.3.8/PKG-INFO` & `dai_python_commons-5.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dai-python-commons
-Version: 5.3.8
+Version: 5.3.9
 Summary: Collection of small python utilities useful for lambda functions or glue jobs. By the Stockholm Public Transport Administration.
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: data-consolidation
 Provides-Extra: glue
 Requires-Dist: awswrangler (==3.2.1); extra == "glue"
```

