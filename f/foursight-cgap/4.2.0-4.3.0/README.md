# Comparing `tmp/foursight_cgap-4.2.0.tar.gz` & `tmp/foursight_cgap-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight_cgap-4.2.0.tar", max compression
+gzip compressed data, was "foursight_cgap-4.3.0.tar", max compression
```

## Comparing `foursight_cgap-4.2.0.tar` & `foursight_cgap-4.3.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1083 2024-02-27 12:58:23.006075 foursight_cgap-4.2.0/LICENSE.txt
--rw-r--r--   0        0        0        0 2024-02-27 12:58:23.006075 foursight_cgap-4.2.0/chalicelib_cgap/__init__.py
--rw-r--r--   0        0        0     1071 2024-02-27 12:58:23.006075 foursight_cgap-4.2.0/chalicelib_cgap/app_utils.py
--rw-r--r--   0        0        0      952 2024-02-27 12:58:23.006075 foursight_cgap-4.2.0/chalicelib_cgap/buckets.py
--rw-r--r--   0        0        0     4805 2024-02-27 12:58:23.006075 foursight_cgap-4.2.0/chalicelib_cgap/check_schedules.py
--rw-r--r--   0        0        0    17006 2024-02-27 12:58:23.006075 foursight_cgap-4.2.0/chalicelib_cgap/check_setup.json
--rw-r--r--   0        0        0     9278 2024-02-27 12:58:23.006075 foursight_cgap-4.2.0/chalicelib_cgap/check_setup.json-local
--rw-r--r--   0        0        0      249 2024-02-27 12:58:23.006075 foursight_cgap-4.2.0/chalicelib_cgap/checks/__init__.py
--rw-r--r--   0        0        0     9636 2024-02-27 12:58:23.006075 foursight_cgap-4.2.0/chalicelib_cgap/checks/audit_checks.py
--rw-r--r--   0        0        0    11502 2024-02-27 12:58:23.006075 foursight_cgap-4.2.0/chalicelib_cgap/checks/deployment_checks.py
--rw-r--r--   0        0        0     2874 2024-02-27 12:58:23.006075 foursight_cgap-4.2.0/chalicelib_cgap/checks/ecs_checks.py
--rw-r--r--   0        0        0     3919 2024-02-27 12:58:23.006075 foursight_cgap-4.2.0/chalicelib_cgap/checks/es_checks.py
--rw-r--r--   0        0        0    11577 2024-02-27 12:58:23.006075 foursight_cgap-4.2.0/chalicelib_cgap/checks/helpers/clone_utils.py
--rw-r--r--   0        0        0      262 2024-02-27 12:58:23.006075 foursight_cgap-4.2.0/chalicelib_cgap/checks/helpers/confchecks.py
--rw-r--r--   0        0        0      333 2024-02-27 12:58:23.006075 foursight_cgap-4.2.0/chalicelib_cgap/checks/helpers/constants.py
--rw-r--r--   0        0        0    13110 2024-02-27 12:58:23.006075 foursight_cgap-4.2.0/chalicelib_cgap/checks/helpers/lifecycle_utils.py
--rw-r--r--   0        0        0     8518 2024-02-27 12:58:23.010075 foursight_cgap-4.2.0/chalicelib_cgap/checks/helpers/linecount_dicts.py
--rw-r--r--   0        0        0     4014 2024-02-27 12:58:23.010075 foursight_cgap-4.2.0/chalicelib_cgap/checks/helpers/utils.py
--rw-r--r--   0        0        0    39030 2024-02-27 12:58:23.010075 foursight_cgap-4.2.0/chalicelib_cgap/checks/helpers/wfr_utils.py
--rw-r--r--   0        0        0     2571 2024-02-27 12:58:23.010075 foursight_cgap-4.2.0/chalicelib_cgap/checks/helpers/wfrset_utils.py
--rw-r--r--   0        0        0     7577 2024-02-27 12:58:23.010075 foursight_cgap-4.2.0/chalicelib_cgap/checks/lifecycle_checks.py
--rw-r--r--   0        0        0    26338 2024-02-27 12:58:23.010075 foursight_cgap-4.2.0/chalicelib_cgap/checks/system_checks.py
--rw-r--r--   0        0        0    58850 2024-02-27 12:58:23.010075 foursight_cgap-4.2.0/chalicelib_cgap/checks/wfr_checks.py
--rw-r--r--   0        0        0    58234 2024-02-27 12:58:23.010075 foursight_cgap-4.2.0/chalicelib_cgap/checks/wrangler_checks.py
--rw-r--r--   0        0        0      772 2024-02-27 12:58:23.010075 foursight_cgap-4.2.0/chalicelib_cgap/deploy.py
--rw-r--r--   0        0        0      129 2024-02-27 12:58:34.906197 foursight_cgap-4.2.0/chalicelib_cgap/gitinfo.json
--rw-r--r--   0        0        0      616 2024-02-27 12:58:23.010075 foursight_cgap-4.2.0/chalicelib_cgap/package.py
--rw-r--r--   0        0        0      322 2024-02-27 12:58:23.010075 foursight_cgap-4.2.0/chalicelib_cgap/scripts/local_check_execution.py
--rw-r--r--   0        0        0      315 2024-02-27 12:58:23.010075 foursight_cgap-4.2.0/chalicelib_cgap/vars.py
--rw-r--r--   0        0        0     1543 2024-02-27 12:58:23.010075 foursight_cgap-4.2.0/pyproject.toml
--rw-r--r--   0        0        0     1281 1970-01-01 00:00:00.000000 foursight_cgap-4.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-04-25 15:16:10.210029 foursight_cgap-4.3.0/LICENSE.txt
+-rw-r--r--   0        0        0        0 2024-04-25 15:16:10.210029 foursight_cgap-4.3.0/chalicelib_cgap/__init__.py
+-rw-r--r--   0        0        0     1071 2024-04-25 15:16:10.210029 foursight_cgap-4.3.0/chalicelib_cgap/app_utils.py
+-rw-r--r--   0        0        0      952 2024-04-25 15:16:10.210029 foursight_cgap-4.3.0/chalicelib_cgap/buckets.py
+-rw-r--r--   0        0        0     4805 2024-04-25 15:16:10.210029 foursight_cgap-4.3.0/chalicelib_cgap/check_schedules.py
+-rw-r--r--   0        0        0    17006 2024-04-25 15:16:10.210029 foursight_cgap-4.3.0/chalicelib_cgap/check_setup.json
+-rw-r--r--   0        0        0     9278 2024-04-25 15:16:10.210029 foursight_cgap-4.3.0/chalicelib_cgap/check_setup.json-local
+-rw-r--r--   0        0        0      249 2024-04-25 15:16:10.210029 foursight_cgap-4.3.0/chalicelib_cgap/checks/__init__.py
+-rw-r--r--   0        0        0     9636 2024-04-25 15:16:10.210029 foursight_cgap-4.3.0/chalicelib_cgap/checks/audit_checks.py
+-rw-r--r--   0        0        0    11502 2024-04-25 15:16:10.210029 foursight_cgap-4.3.0/chalicelib_cgap/checks/deployment_checks.py
+-rw-r--r--   0        0        0     2874 2024-04-25 15:16:10.210029 foursight_cgap-4.3.0/chalicelib_cgap/checks/ecs_checks.py
+-rw-r--r--   0        0        0     3919 2024-04-25 15:16:10.210029 foursight_cgap-4.3.0/chalicelib_cgap/checks/es_checks.py
+-rw-r--r--   0        0        0    11577 2024-04-25 15:16:10.210029 foursight_cgap-4.3.0/chalicelib_cgap/checks/helpers/clone_utils.py
+-rw-r--r--   0        0        0      262 2024-04-25 15:16:10.210029 foursight_cgap-4.3.0/chalicelib_cgap/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0      333 2024-04-25 15:16:10.210029 foursight_cgap-4.3.0/chalicelib_cgap/checks/helpers/constants.py
+-rw-r--r--   0        0        0    13110 2024-04-25 15:16:10.210029 foursight_cgap-4.3.0/chalicelib_cgap/checks/helpers/lifecycle_utils.py
+-rw-r--r--   0        0        0     8518 2024-04-25 15:16:10.210029 foursight_cgap-4.3.0/chalicelib_cgap/checks/helpers/linecount_dicts.py
+-rw-r--r--   0        0        0     4014 2024-04-25 15:16:10.210029 foursight_cgap-4.3.0/chalicelib_cgap/checks/helpers/utils.py
+-rw-r--r--   0        0        0    39030 2024-04-25 15:16:10.214029 foursight_cgap-4.3.0/chalicelib_cgap/checks/helpers/wfr_utils.py
+-rw-r--r--   0        0        0     2571 2024-04-25 15:16:10.214029 foursight_cgap-4.3.0/chalicelib_cgap/checks/helpers/wfrset_utils.py
+-rw-r--r--   0        0        0     7577 2024-04-25 15:16:10.214029 foursight_cgap-4.3.0/chalicelib_cgap/checks/lifecycle_checks.py
+-rw-r--r--   0        0        0    26338 2024-04-25 15:16:10.214029 foursight_cgap-4.3.0/chalicelib_cgap/checks/system_checks.py
+-rw-r--r--   0        0        0    58850 2024-04-25 15:16:10.214029 foursight_cgap-4.3.0/chalicelib_cgap/checks/wfr_checks.py
+-rw-r--r--   0        0        0    58234 2024-04-25 15:16:10.214029 foursight_cgap-4.3.0/chalicelib_cgap/checks/wrangler_checks.py
+-rw-r--r--   0        0        0      772 2024-04-25 15:16:10.214029 foursight_cgap-4.3.0/chalicelib_cgap/deploy.py
+-rw-r--r--   0        0        0      129 2024-04-25 15:16:23.474042 foursight_cgap-4.3.0/chalicelib_cgap/gitinfo.json
+-rw-r--r--   0        0        0      616 2024-04-25 15:16:10.214029 foursight_cgap-4.3.0/chalicelib_cgap/package.py
+-rw-r--r--   0        0        0      322 2024-04-25 15:16:10.214029 foursight_cgap-4.3.0/chalicelib_cgap/scripts/local_check_execution.py
+-rw-r--r--   0        0        0      315 2024-04-25 15:16:10.214029 foursight_cgap-4.3.0/chalicelib_cgap/vars.py
+-rw-r--r--   0        0        0     1543 2024-04-25 15:16:10.214029 foursight_cgap-4.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1281 1970-01-01 00:00:00.000000 foursight_cgap-4.3.0/PKG-INFO
```

### Comparing `foursight_cgap-4.2.0/LICENSE.txt` & `foursight_cgap-4.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight_cgap-4.2.0/chalicelib_cgap/app_utils.py` & `foursight_cgap-4.3.0/chalicelib_cgap/app_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-4.2.0/chalicelib_cgap/buckets.py` & `foursight_cgap-4.3.0/chalicelib_cgap/buckets.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-4.2.0/chalicelib_cgap/check_schedules.py` & `foursight_cgap-4.3.0/chalicelib_cgap/check_schedules.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-4.2.0/chalicelib_cgap/check_setup.json` & `foursight_cgap-4.3.0/chalicelib_cgap/check_setup.json`

 * *Files identical despite different names*

### Comparing `foursight_cgap-4.2.0/chalicelib_cgap/check_setup.json-local` & `foursight_cgap-4.3.0/chalicelib_cgap/check_setup.json-local`

 * *Files identical despite different names*

### Comparing `foursight_cgap-4.2.0/chalicelib_cgap/checks/audit_checks.py` & `foursight_cgap-4.3.0/chalicelib_cgap/checks/audit_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-4.2.0/chalicelib_cgap/checks/deployment_checks.py` & `foursight_cgap-4.3.0/chalicelib_cgap/checks/deployment_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-4.2.0/chalicelib_cgap/checks/ecs_checks.py` & `foursight_cgap-4.3.0/chalicelib_cgap/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-4.2.0/chalicelib_cgap/checks/es_checks.py` & `foursight_cgap-4.3.0/chalicelib_cgap/checks/es_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-4.2.0/chalicelib_cgap/checks/helpers/clone_utils.py` & `foursight_cgap-4.3.0/chalicelib_cgap/checks/helpers/clone_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-4.2.0/chalicelib_cgap/checks/helpers/lifecycle_utils.py` & `foursight_cgap-4.3.0/chalicelib_cgap/checks/helpers/lifecycle_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-4.2.0/chalicelib_cgap/checks/helpers/linecount_dicts.py` & `foursight_cgap-4.3.0/chalicelib_cgap/checks/helpers/linecount_dicts.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-4.2.0/chalicelib_cgap/checks/helpers/utils.py` & `foursight_cgap-4.3.0/chalicelib_cgap/checks/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-4.2.0/chalicelib_cgap/checks/helpers/wfr_utils.py` & `foursight_cgap-4.3.0/chalicelib_cgap/checks/helpers/wfr_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-4.2.0/chalicelib_cgap/checks/helpers/wfrset_utils.py` & `foursight_cgap-4.3.0/chalicelib_cgap/checks/helpers/wfrset_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-4.2.0/chalicelib_cgap/checks/lifecycle_checks.py` & `foursight_cgap-4.3.0/chalicelib_cgap/checks/lifecycle_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-4.2.0/chalicelib_cgap/checks/system_checks.py` & `foursight_cgap-4.3.0/chalicelib_cgap/checks/system_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-4.2.0/chalicelib_cgap/checks/wfr_checks.py` & `foursight_cgap-4.3.0/chalicelib_cgap/checks/wfr_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-4.2.0/chalicelib_cgap/checks/wrangler_checks.py` & `foursight_cgap-4.3.0/chalicelib_cgap/checks/wrangler_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-4.2.0/chalicelib_cgap/deploy.py` & `foursight_cgap-4.3.0/chalicelib_cgap/deploy.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-4.2.0/chalicelib_cgap/package.py` & `foursight_cgap-4.3.0/chalicelib_cgap/package.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-4.2.0/pyproject.toml` & `foursight_cgap-4.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "foursight-cgap"
-version = "4.2.0"
+version = "4.3.0"
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "chalicelib_cgap" }
 ]
 
@@ -21,15 +21,15 @@
 # Error: "The client noticed that the server is not Elasticsearch and we do not support this unknown product"
 # https://stackoverflow.com/questions/68802324/elasticsearch-in-go-err-the-client-noticed-that-the-server-is-not-elasticsear
 elasticsearch = "7.13.4"
 elasticsearch-dsl = "^7.0.0"
 gitpython = "^3.1.2"
 pytz = "^2020.1"
 magma-suite = "^3.0.0"
-tibanna-ff = "^3.2.0"
+tibanna-ff = "^3.4.0"
 MarkupSafe = "^2.1.3"
 foursight-core = "^5.3.0"
 # use below for tests but not for deployment
 #foursight-core = { git = "https://github.com/4dn-dcic/foursight-core.git", branch="core2" }
 #portal-pipeline-utils = "2.1.0.1b1"
 # Need pytest-redis 3.0.2 or higher for pytest 7.4.2 (or higher).
 pytest = "^7.4.2"
```

### Comparing `foursight_cgap-4.2.0/PKG-INFO` & `foursight_cgap-4.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursight-cgap
-Version: 4.2.0
+Version: 4.3.0
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -24,9 +24,9 @@
 Requires-Dist: geocoder (==1.38.1)
 Requires-Dist: gitpython (>=3.1.2,<4.0.0)
 Requires-Dist: google-api-python-client (>=1.12.5,<2.0.0)
 Requires-Dist: magma-suite (>=3.0.0,<4.0.0)
 Requires-Dist: pytest (>=7.4.2,<8.0.0)
 Requires-Dist: pytest-redis (>=3.0.2,<4.0.0)
 Requires-Dist: pytz (>=2020.1,<2021.0)
-Requires-Dist: tibanna-ff (>=3.2.0,<4.0.0)
+Requires-Dist: tibanna-ff (>=3.4.0,<4.0.0)
 Requires-Dist: tzlocal (>=5.1,<6.0)
```

