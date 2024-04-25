# Comparing `tmp/quilt3-6.0.0a2.tar.gz` & `tmp/quilt3-6.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/quilt/quilt/api/python/dist/.tmp-nunz_r4w/quilt3-6.0.0a2.tar", last modified: Mon Apr 15 15:46:14 2024, max compression
+gzip compressed data, was "/home/runner/work/quilt/quilt/api/python/dist/.tmp-zolhn1fj/quilt3-6.0.0a3.tar", last modified: Thu Apr 25 15:24:56 2024, max compression
```

## Comparing `quilt3-6.0.0a2.tar` & `quilt3-6.0.0a3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:14.000000 quilt3-6.0.0a2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-15 15:46:14.000000 quilt3-6.0.0a2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:14.000000 quilt3-6.0.0a2/quilt3/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:14.000000 quilt3-6.0.0a2/quilt3/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9832 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/backends/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/backends/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6287 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)    54270 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    42519 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)    16592 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    66000 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/search_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     8138 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)    18987 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:14.000000 quilt3-6.0.0a2/quilt3/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)    11102 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/workflows/config-1.schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:14.000000 quilt3-6.0.0a2/quilt3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-15 15:46:14.000000 quilt3-6.0.0a2/quilt3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-15 15:46:14.000000 quilt3-6.0.0a2/quilt3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 15:46:14.000000 quilt3-6.0.0a2/quilt3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-15 15:46:14.000000 quilt3-6.0.0a2/quilt3.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-15 15:46:14.000000 quilt3-6.0.0a2/quilt3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 15:46:14.000000 quilt3-6.0.0a2/quilt3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 15:46:14.000000 quilt3-6.0.0a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:14.000000 quilt3-6.0.0a2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     8676 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/tests/test_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     8222 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    29428 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/tests/test_data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7600 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/tests/test_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/tests/test_s3clientprovider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/tests/test_telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     8526 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/tests/test_workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:56.000000 quilt3-6.0.0a3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-25 15:24:35.000000 quilt3-6.0.0a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-25 15:24:35.000000 quilt3-6.0.0a3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-25 15:24:56.000000 quilt3-6.0.0a3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:56.000000 quilt3-6.0.0a3/quilt3/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 15:24:35.000000 quilt3-6.0.0a3/quilt3/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-25 15:24:35.000000 quilt3-6.0.0a3/quilt3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-25 15:24:35.000000 quilt3-6.0.0a3/quilt3/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-04-25 15:24:35.000000 quilt3-6.0.0a3/quilt3/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:56.000000 quilt3-6.0.0a3/quilt3/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-25 15:24:35.000000 quilt3-6.0.0a3/quilt3/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9832 2024-04-25 15:24:35.000000 quilt3-6.0.0a3/quilt3/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-25 15:24:35.000000 quilt3-6.0.0a3/quilt3/backends/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-25 15:24:35.000000 quilt3-6.0.0a3/quilt3/backends/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-04-25 15:24:35.000000 quilt3-6.0.0a3/quilt3/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54270 2024-04-25 15:24:35.000000 quilt3-6.0.0a3/quilt3/data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-25 15:24:35.000000 quilt3-6.0.0a3/quilt3/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42519 2024-04-25 15:24:35.000000 quilt3-6.0.0a3/quilt3/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-25 15:24:35.000000 quilt3-6.0.0a3/quilt3/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16592 2024-04-25 15:24:35.000000 quilt3-6.0.0a3/quilt3/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66000 2024-04-25 15:24:35.000000 quilt3-6.0.0a3/quilt3/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-25 15:24:35.000000 quilt3-6.0.0a3/quilt3/search_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8138 2024-04-25 15:24:35.000000 quilt3-6.0.0a3/quilt3/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-04-25 15:24:35.000000 quilt3-6.0.0a3/quilt3/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18987 2024-04-25 15:24:35.000000 quilt3-6.0.0a3/quilt3/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:56.000000 quilt3-6.0.0a3/quilt3/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)    11102 2024-04-25 15:24:35.000000 quilt3-6.0.0a3/quilt3/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-04-25 15:24:35.000000 quilt3-6.0.0a3/quilt3/workflows/config-1.schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:56.000000 quilt3-6.0.0a3/quilt3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-25 15:24:56.000000 quilt3-6.0.0a3/quilt3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-25 15:24:56.000000 quilt3-6.0.0a3/quilt3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:24:56.000000 quilt3-6.0.0a3/quilt3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-25 15:24:56.000000 quilt3-6.0.0a3/quilt3.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-25 15:24:56.000000 quilt3-6.0.0a3/quilt3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 15:24:56.000000 quilt3-6.0.0a3/quilt3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:24:56.000000 quilt3-6.0.0a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-25 15:24:35.000000 quilt3-6.0.0a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:56.000000 quilt3-6.0.0a3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-25 15:24:35.000000 quilt3-6.0.0a3/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8676 2024-04-25 15:24:35.000000 quilt3-6.0.0a3/tests/test_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8222 2024-04-25 15:24:35.000000 quilt3-6.0.0a3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29428 2024-04-25 15:24:35.000000 quilt3-6.0.0a3/tests/test_data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7600 2024-04-25 15:24:35.000000 quilt3-6.0.0a3/tests/test_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-25 15:24:35.000000 quilt3-6.0.0a3/tests/test_s3clientprovider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-25 15:24:35.000000 quilt3-6.0.0a3/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-25 15:24:35.000000 quilt3-6.0.0a3/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-25 15:24:35.000000 quilt3-6.0.0a3/tests/test_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-25 15:24:35.000000 quilt3-6.0.0a3/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8526 2024-04-25 15:24:35.000000 quilt3-6.0.0a3/tests/test_workflows.py
```

### Comparing `quilt3-6.0.0a2/LICENSE` & `quilt3-6.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a2/PKG-INFO` & `quilt3-6.0.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quilt3
-Version: 6.0.0a2
+Version: 6.0.0a3
 Summary: Quilt: where data comes together
 Home-page: https://github.com/quiltdata/quilt
 Author: quiltdata
 Author-email: contact@quiltdata.io
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `quilt3-6.0.0a2/quilt3/__init__.py` & `quilt3-6.0.0a3/quilt3/__init__.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a2/quilt3/admin.py` & `quilt3-6.0.0a3/quilt3/admin.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a2/quilt3/api.py` & `quilt3-6.0.0a3/quilt3/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import typing as T
+
 from .backends import get_package_registry
 from .data_transfer import copy_file
 from .search_util import search_api
 from .telemetry import ApiTelemetry
 from .util import (
     CONFIG_PATH,
     CONFIG_TEMPLATE,
@@ -160,42 +162,27 @@
 
 
 def _disable_telemetry():
     _config(telemetry_disabled=True)
 
 
 @ApiTelemetry("api.search")
-def search(query, limit=10):
+def search(query: T.Union[str, dict], limit: int = 10) -> T.List[dict]:
     """
     Execute a search against the configured search endpoint.
 
     Args:
-        query (str): query string to search
-        limit (number): maximum number of results to return. Defaults to 10
+        query: query string to query if passed as `str`, DSL query body if passed as `dict`
+        limit: maximum number of results to return. Defaults to 10
 
     Query Syntax:
-        [simple query string query](
-            https://www.elastic.co/guide/en/elasticsearch/reference/6.8/query-dsl-simple-query-string-query.html)
-
+        [Query String Query](
+            https://www.elastic.co/guide/en/elasticsearch/reference/6.8/query-dsl-query-string-query.html)
+        [Query DSL](https://www.elastic.co/guide/en/elasticsearch/reference/6.8/query-dsl.html)
 
     Returns:
-        a list of objects with the following structure:
-        ```
-        [{
-            "_id": <document unique id>
-            "_index": <source index>,
-            "_score": <relevance score>
-            "_source":
-                "key": <key of the object>,
-                "size": <size of object in bytes>,
-                "user_meta": <user metadata from meta= via quilt3>,
-                "last_modified": <timestamp from ElasticSearch>,
-                "updated": <object timestamp from S3>,
-                "version_id": <version_id of object version>
-            "_type": <document type>
-        }, ...]
-        ```
+        search results
     """
     # force a call to configure_from_default if no config exists
     _config()
-    raw_results = search_api(query, '*', limit)
+    raw_results = search_api(query, '_all', limit)
     return raw_results['hits']['hits']
```

### Comparing `quilt3-6.0.0a2/quilt3/backends/__init__.py` & `quilt3-6.0.0a3/quilt3/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a2/quilt3/backends/base.py` & `quilt3-6.0.0a3/quilt3/backends/base.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a2/quilt3/backends/local.py` & `quilt3-6.0.0a3/quilt3/backends/local.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a2/quilt3/backends/s3.py` & `quilt3-6.0.0a3/quilt3/backends/s3.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a2/quilt3/bucket.py` & `quilt3-6.0.0a3/quilt3/bucket.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 bucket.py
 
 Contains the Bucket class, which provides several useful functions
     over an s3 bucket.
 """
 import pathlib
+import typing as T
 
 from .data_transfer import (
     copy_file,
     delete_object,
     list_object_versions,
     list_objects,
     select,
@@ -32,44 +33,31 @@
         """
         self._pk = PhysicalKey.from_url(bucket_uri)
         if self._pk.is_local():
             raise QuiltException("Bucket URI must be an S3 URI")
         if self._pk.path or self._pk.version_id is not None:
             raise QuiltException("Bucket URI shouldn't contain a path or a version ID")
 
-    def search(self, query, limit=10):
+    def search(self, query: T.Union[str, dict], limit: int = 10) -> T.List[dict]:
         """
         Execute a search against the configured search endpoint.
 
         Args:
-            query (str): query string to search
-            limit (number): maximum number of results to return. Defaults to 10
+            query: query string to query if passed as `str`, DSL query body if passed as `dict`
+            limit: maximum number of results to return. Defaults to 10
 
         Query Syntax:
-            By default, a normal plaintext search will be executed over the query string.
-            You can use field-match syntax to filter on exact matches for fields in
-                your metadata.
-            The syntax for field match is `user_meta.$field_name:"exact_match"`.
+            [Query String Query](
+                https://www.elastic.co/guide/en/elasticsearch/reference/6.8/query-dsl-query-string-query.html)
+            [Query DSL](https://www.elastic.co/guide/en/elasticsearch/reference/6.8/query-dsl.html)
 
         Returns:
-            a list of objects with the following structure:
-            ```
-            [{
-                "key": <key of the object>,
-                "version_id": <version_id of object version>,
-                "operation": <"Create" or "Delete">,
-                "meta": <metadata attached to object>,
-                "size": <size of object in bytes>,
-                "text": <indexed text of object>,
-                "source": <source document for object (what is actually stored in ElasticSeach)>,
-                "time": <timestamp for operation>,
-            }...]
-            ```
+            search results
         """
-        return search_api(query, index=self._pk.bucket, limit=limit)
+        return search_api(query, index=f"{self._pk.bucket},{self._pk.bucket}_packages", limit=limit)["hits"]["hits"]
 
     def put_file(self, key, path):
         """
         Stores file at path to key in bucket.
 
         Args:
             key(str): key in bucket to store file at
```

### Comparing `quilt3-6.0.0a2/quilt3/data_transfer.py` & `quilt3-6.0.0a3/quilt3/data_transfer.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a2/quilt3/formats.py` & `quilt3-6.0.0a3/quilt3/formats.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a2/quilt3/imports.py` & `quilt3-6.0.0a3/quilt3/imports.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a2/quilt3/main.py` & `quilt3-6.0.0a3/quilt3/main.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a2/quilt3/packages.py` & `quilt3-6.0.0a3/quilt3/packages.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a2/quilt3/session.py` & `quilt3-6.0.0a3/quilt3/session.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a2/quilt3/telemetry.py` & `quilt3-6.0.0a3/quilt3/telemetry.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a2/quilt3/util.py` & `quilt3-6.0.0a3/quilt3/util.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a2/quilt3/workflows/__init__.py` & `quilt3-6.0.0a3/quilt3/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a2/quilt3/workflows/config-1.schema.json` & `quilt3-6.0.0a3/quilt3/workflows/config-1.schema.json`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a2/quilt3.egg-info/PKG-INFO` & `quilt3-6.0.0a3/quilt3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quilt3
-Version: 6.0.0a2
+Version: 6.0.0a3
 Summary: Quilt: where data comes together
 Home-page: https://github.com/quiltdata/quilt
 Author: quiltdata
 Author-email: contact@quiltdata.io
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `quilt3-6.0.0a2/quilt3.egg-info/SOURCES.txt` & `quilt3-6.0.0a3/quilt3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a2/setup.py` & `quilt3-6.0.0a3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,14 @@
     author='quiltdata',
     author_email='contact@quiltdata.io',
     license='Apache-2.0',
     url='https://github.com/quiltdata/quilt',
     keywords='',
     install_requires=[
         'platformdirs>=2',
-        'aws-requests-auth>=0.4.2',
         'boto3>=1.21.7',
         'jsonlines==1.2.0',
         'PyYAML>=5.1',
         'requests>=2.12.4',
         'tenacity>=5.1.1',
         'tqdm>=4.32',
         'requests_futures==1.0.0',
```

### Comparing `quilt3-6.0.0a2/tests/test_api.py` & `quilt3-6.0.0a3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a2/tests/test_bucket.py` & `quilt3-6.0.0a3/tests/test_bucket.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a2/tests/test_cli.py` & `quilt3-6.0.0a3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a2/tests/test_data_transfer.py` & `quilt3-6.0.0a3/tests/test_data_transfer.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a2/tests/test_formats.py` & `quilt3-6.0.0a3/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a2/tests/test_s3clientprovider.py` & `quilt3-6.0.0a3/tests/test_s3clientprovider.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from unittest import mock
 
 import botocore
 import pytest
 
 from quilt3.data_transfer import S3ClientProvider
 
-PATCH_UNSET_CREDENTIALS = mock.patch.dict(os.environ, clear=True)
+PATCH_UNSET_CREDENTIALS = mock.patch.dict(os.environ, {"AWS_SHARED_CREDENTIALS_FILE": "/not-exist"}, clear=True)
 PATCH_SET_CREDENTIALS = mock.patch.dict(
     os.environ,
     dict.fromkeys(
         (
             "AWS_ACCESS_KEY_ID",
             "AWS_SECRET_ACCESS_KEY",
         ),
```

### Comparing `quilt3-6.0.0a2/tests/test_session.py` & `quilt3-6.0.0a3/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a2/tests/test_telemetry.py` & `quilt3-6.0.0a3/tests/test_telemetry.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a2/tests/test_util.py` & `quilt3-6.0.0a3/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a2/tests/test_workflows.py` & `quilt3-6.0.0a3/tests/test_workflows.py`

 * *Files identical despite different names*

