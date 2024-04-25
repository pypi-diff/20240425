# Comparing `tmp/prefect_gcp-0.5.8.tar.gz` & `tmp/prefect_gcp-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_gcp-0.5.8.tar", last modified: Tue Apr 23 19:10:44 2024, max compression
+gzip compressed data, was "prefect_gcp-0.5.9.tar", last modified: Thu Apr 25 19:20:03 2024, max compression
```

## Comparing `prefect_gcp-0.5.8.tar` & `prefect_gcp-0.5.9.tar`

### file list

```diff
@@ -1,51 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:10:44.166912 prefect_gcp-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-04-23 19:10:44.166912 prefect_gcp-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:10:44.166912 prefect_gcp-0.5.8/prefect_gcp/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/prefect_gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-23 19:10:44.166912 prefect_gcp-0.5.8/prefect_gcp/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    21657 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/prefect_gcp/aiplatform.py
--rw-r--r--   0 runner    (1001) docker     (127)    34349 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/prefect_gcp/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (127)    32239 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/prefect_gcp/cloud_run.py
--rw-r--r--   0 runner    (1001) docker     (127)    46400 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/prefect_gcp/cloud_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    17066 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/prefect_gcp/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:10:44.158912 prefect_gcp-0.5.8/prefect_gcp/deployments/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/prefect_gcp/deployments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8913 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/prefect_gcp/deployments/steps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:10:44.158912 prefect_gcp-0.5.8/prefect_gcp/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/prefect_gcp/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11693 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/prefect_gcp/models/cloud_run_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    13577 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/prefect_gcp/secret_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/prefect_gcp/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:10:44.158912 prefect_gcp-0.5.8/prefect_gcp/workers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/prefect_gcp/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31976 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/prefect_gcp/workers/cloud_run.py
--rw-r--r--   0 runner    (1001) docker     (127)    28869 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/prefect_gcp/workers/cloud_run_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    24133 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/prefect_gcp/workers/vertex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:10:44.162912 prefect_gcp-0.5.8/prefect_gcp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-04-23 19:10:44.000000 prefect_gcp-0.5.8/prefect_gcp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-23 19:10:44.000000 prefect_gcp-0.5.8/prefect_gcp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:10:44.000000 prefect_gcp-0.5.8/prefect_gcp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-23 19:10:44.000000 prefect_gcp-0.5.8/prefect_gcp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-23 19:10:44.000000 prefect_gcp-0.5.8/prefect_gcp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 19:10:44.000000 prefect_gcp-0.5.8/prefect_gcp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-23 19:10:44.166912 prefect_gcp-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:10:44.162912 prefect_gcp-0.5.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/tests/test_aiplatform.py
--rw-r--r--   0 runner    (1001) docker     (127)     9885 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/tests/test_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)    34052 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/tests/test_cloud_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/tests/test_cloud_run_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    26236 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/tests/test_cloud_run_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/tests/test_cloud_run_worker_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    20315 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/tests/test_cloud_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/tests/test_deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/tests/test_secret_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10711 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/tests/test_vertex_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    80049 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:03.083167 prefect_gcp-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-04-25 19:20:03.083167 prefect_gcp-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:03.075167 prefect_gcp-0.5.9/prefect_gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/prefect_gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 19:20:02.000000 prefect_gcp-0.5.9/prefect_gcp/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21574 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/prefect_gcp/aiplatform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34350 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/prefect_gcp/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32157 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/prefect_gcp/cloud_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46401 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/prefect_gcp/cloud_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17066 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/prefect_gcp/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:03.075167 prefect_gcp-0.5.9/prefect_gcp/deployments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/prefect_gcp/deployments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8914 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/prefect_gcp/deployments/steps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:03.075167 prefect_gcp-0.5.9/prefect_gcp/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/prefect_gcp/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11694 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/prefect_gcp/models/cloud_run_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13578 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/prefect_gcp/secret_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/prefect_gcp/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:03.079167 prefect_gcp-0.5.9/prefect_gcp/workers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/prefect_gcp/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31977 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/prefect_gcp/workers/cloud_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28870 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/prefect_gcp/workers/cloud_run_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24134 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/prefect_gcp/workers/vertex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:03.079167 prefect_gcp-0.5.9/prefect_gcp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-04-25 19:20:02.000000 prefect_gcp-0.5.9/prefect_gcp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-25 19:20:03.000000 prefect_gcp-0.5.9/prefect_gcp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:20:02.000000 prefect_gcp-0.5.9/prefect_gcp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-25 19:20:02.000000 prefect_gcp-0.5.9/prefect_gcp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-25 19:20:02.000000 prefect_gcp-0.5.9/prefect_gcp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 19:20:02.000000 prefect_gcp-0.5.9/prefect_gcp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:20:03.083167 prefect_gcp-0.5.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:03.079167 prefect_gcp-0.5.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:03.079167 prefect_gcp-0.5.9/tests/projects/
+-rw-r--r--   0 runner    (1001) docker     (127)     7646 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/tests/projects/test_steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/tests/test_aiplatform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9871 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/tests/test_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34051 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/tests/test_cloud_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/tests/test_cloud_run_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26236 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/tests/test_cloud_run_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/tests/test_cloud_run_worker_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20315 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/tests/test_cloud_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/tests/test_deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/tests/test_secret_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10710 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/tests/test_vertex_worker.py
```

### Comparing `prefect_gcp-0.5.8/PKG-INFO` & `prefect_gcp-0.5.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: prefect-gcp
-Version: 0.5.8
-Summary: Prefect tasks and subflows for interacting with Google Cloud Platform.
-Home-page: https://github.com/PrefectHQ/prefect-gcp
-Author: Prefect Technologies, Inc.
-Author-email: help@prefect.io
+Version: 0.5.9
+Summary: Prefect integrations for interacting with Google Cloud Platform.
+Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
+Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-gcp
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
 Requires-Dist: prefect>=2.16.4
 Requires-Dist: google-api-python-client>=2.20.0
 Requires-Dist: google-cloud-storage>=2.0.0
 Requires-Dist: tenacity>=8.0.0
 Requires-Dist: python-slugify>=8.0.0
 Provides-Extra: cloud-storage
 Requires-Dist: google-cloud-storage; extra == "cloud-storage"
@@ -31,61 +30,48 @@
 Requires-Dist: google-cloud-bigquery; extra == "bigquery"
 Requires-Dist: google-cloud-bigquery-storage; extra == "bigquery"
 Provides-Extra: secret-manager
 Requires-Dist: google-cloud-secret-manager; extra == "secret-manager"
 Provides-Extra: aiplatform
 Requires-Dist: google-cloud-aiplatform; extra == "aiplatform"
 Provides-Extra: all-extras
-Requires-Dist: google-cloud-aiplatform; extra == "all-extras"
+Requires-Dist: google-cloud-storage; extra == "all-extras"
 Requires-Dist: google-cloud-bigquery; extra == "all-extras"
 Requires-Dist: google-cloud-bigquery-storage; extra == "all-extras"
 Requires-Dist: google-cloud-secret-manager; extra == "all-extras"
-Requires-Dist: google-cloud-storage; extra == "all-extras"
+Requires-Dist: google-cloud-aiplatform; extra == "all-extras"
 Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
-Requires-Dist: flake8; extra == "dev"
+Requires-Dist: google-cloud-aiplatform; extra == "dev"
+Requires-Dist: google-cloud-bigquery-storage; extra == "dev"
+Requires-Dist: google-cloud-bigquery; extra == "dev"
+Requires-Dist: google-cloud-secret-manager; extra == "dev"
+Requires-Dist: google-cloud-storage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
-Requires-Dist: isort; extra == "dev"
-Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
+Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
 Requires-Dist: mock; python_version < "3.8" and extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pandas; extra == "dev"
 Requires-Dist: pillow; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pyarrow; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
-Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
-Requires-Dist: google-cloud-aiplatform; extra == "dev"
-Requires-Dist: google-cloud-bigquery; extra == "dev"
-Requires-Dist: google-cloud-bigquery-storage; extra == "dev"
-Requires-Dist: google-cloud-secret-manager; extra == "dev"
-Requires-Dist: google-cloud-storage; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
 
 # `prefect-gcp`
 
 <p align="center">
     <a href="https://pypi.python.org/pypi/prefect-gcp/" alt="PyPI version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-gcp?color=0052FF&labelColor=090422"></a>
-    <a href="https://github.com/PrefectHQ/prefect-gcp/" alt="Stars">
-        <img src="https://img.shields.io/github/stars/PrefectHQ/prefect-gcp?color=0052FF&labelColor=090422" /></a>
     <a href="https://pypistats.org/packages/prefect-gcp/" alt="Downloads">
         <img src="https://img.shields.io/pypi/dm/prefect-gcp?color=0052FF&labelColor=090422" /></a>
-    <a href="https://github.com/PrefectHQ/prefect-gcp/pulse" alt="Activity">
-        <img src="https://img.shields.io/github/commit-activity/m/PrefectHQ/prefect-gcp?color=0052FF&labelColor=090422" /></a>
-    <br>
-    <a href="https://prefect-community.slack.com" alt="Slack">
-        <img src="https://img.shields.io/badge/slack-join_community-red.svg?color=0052FF&labelColor=090422&logo=slack" /></a>
-    <a href="https://discourse.prefect.io/" alt="Discourse">
-        <img src="https://img.shields.io/badge/discourse-browse_forum-red.svg?color=0052FF&labelColor=090422&logo=discourse" /></a>
 </p>
 
 `prefect-gcp` makes it easy to leverage the capabilities of Google Cloud Platform (GCP) in your flows, featuring support for Vertex AI, Cloud Run, BigQuery, Cloud Storage, and Secret Manager.
 
 Visit the full docs [here](https://PrefectHQ.github.io/prefect-gcp).
 
 ### Installation
```

#### html2text {}

```diff
@@ -1,54 +1,48 @@
-Metadata-Version: 2.1 Name: prefect-gcp Version: 0.5.8 Summary: Prefect tasks
-and subflows for interacting with Google Cloud Platform. Home-page: https://
-github.com/PrefectHQ/prefect-gcp Author: Prefect Technologies, Inc. Author-
-email: help@prefect.io License: Apache License 2.0 Keywords: prefect
-Classifier: Natural Language :: English Classifier: Intended Audience ::
-Developers Classifier: Intended Audience :: System Administrators Classifier:
-License :: OSI Approved :: Apache Software License Classifier: Programming
-Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
-3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries Requires-Python: >=3.7
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-prefect>=2.16.4 Requires-Dist: google-api-python-client>=2.20.0 Requires-Dist:
-google-cloud-storage>=2.0.0 Requires-Dist: tenacity>=8.0.0 Requires-Dist:
-python-slugify>=8.0.0 Provides-Extra: cloud-storage Requires-Dist: google-
-cloud-storage; extra == "cloud-storage" Provides-Extra: bigquery Requires-Dist:
-google-cloud-bigquery; extra == "bigquery" Requires-Dist: google-cloud-
-bigquery-storage; extra == "bigquery" Provides-Extra: secret-manager Requires-
-Dist: google-cloud-secret-manager; extra == "secret-manager" Provides-Extra:
-aiplatform Requires-Dist: google-cloud-aiplatform; extra == "aiplatform"
-Provides-Extra: all-extras Requires-Dist: google-cloud-aiplatform; extra ==
-"all-extras" Requires-Dist: google-cloud-bigquery; extra == "all-extras"
-Requires-Dist: google-cloud-bigquery-storage; extra == "all-extras" Requires-
-Dist: google-cloud-secret-manager; extra == "all-extras" Requires-Dist: google-
-cloud-storage; extra == "all-extras" Provides-Extra: dev Requires-Dist: black;
-extra == "dev" Requires-Dist: coverage; extra == "dev" Requires-Dist: flake8;
-extra == "dev" Requires-Dist: interrogate; extra == "dev" Requires-Dist: isort;
-extra == "dev" Requires-Dist: mkdocs; extra == "dev" Requires-Dist: mkdocs-gen-
-files; extra == "dev" Requires-Dist: mkdocs-material; extra == "dev" Requires-
-Dist: mkdocstrings[python]; extra == "dev" Requires-Dist: mock; python_version
-< "3.8" and extra == "dev" Requires-Dist: mypy; extra == "dev" Requires-Dist:
+Metadata-Version: 2.1 Name: prefect-gcp Version: 0.5.9 Summary: Prefect
+integrations for interacting with Google Cloud Platform. Author-email: "Prefect
+Technologies, Inc."
+prefect.io> License: Apache License 2.0 Project-URL: Homepage, https://
+github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-gcp Keywords:
+prefect Classifier: Natural Language :: English Classifier: Intended Audience
+:: Developers Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: Apache Software License Classifier:
+Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
+Topic :: Software Development :: Libraries Requires-Python: >=3.8 Description-
+Content-Type: text/markdown Requires-Dist: prefect>=2.16.4 Requires-Dist:
+google-api-python-client>=2.20.0 Requires-Dist: google-cloud-storage>=2.0.0
+Requires-Dist: tenacity>=8.0.0 Requires-Dist: python-slugify>=8.0.0 Provides-
+Extra: cloud-storage Requires-Dist: google-cloud-storage; extra == "cloud-
+storage" Provides-Extra: bigquery Requires-Dist: google-cloud-bigquery; extra
+== "bigquery" Requires-Dist: google-cloud-bigquery-storage; extra == "bigquery"
+Provides-Extra: secret-manager Requires-Dist: google-cloud-secret-manager;
+extra == "secret-manager" Provides-Extra: aiplatform Requires-Dist: google-
+cloud-aiplatform; extra == "aiplatform" Provides-Extra: all-extras Requires-
+Dist: google-cloud-storage; extra == "all-extras" Requires-Dist: google-cloud-
+bigquery; extra == "all-extras" Requires-Dist: google-cloud-bigquery-storage;
+extra == "all-extras" Requires-Dist: google-cloud-secret-manager; extra ==
+"all-extras" Requires-Dist: google-cloud-aiplatform; extra == "all-extras"
+Provides-Extra: dev Requires-Dist: coverage; extra == "dev" Requires-Dist:
+google-cloud-aiplatform; extra == "dev" Requires-Dist: google-cloud-bigquery-
+storage; extra == "dev" Requires-Dist: google-cloud-bigquery; extra == "dev"
+Requires-Dist: google-cloud-secret-manager; extra == "dev" Requires-Dist:
+google-cloud-storage; extra == "dev" Requires-Dist: interrogate; extra == "dev"
+Requires-Dist: mkdocs-gen-files; extra == "dev" Requires-Dist: mkdocs-material;
+extra == "dev" Requires-Dist: mkdocs; extra == "dev" Requires-Dist:
+mkdocstrings[python]; extra == "dev" Requires-Dist: mock; python_version <
+"3.8" and extra == "dev" Requires-Dist: mypy; extra == "dev" Requires-Dist:
 pandas; extra == "dev" Requires-Dist: pillow; extra == "dev" Requires-Dist:
 pre-commit; extra == "dev" Requires-Dist: pyarrow; extra == "dev" Requires-
-Dist: pytest; extra == "dev" Requires-Dist: pytest-asyncio; extra == "dev"
-Requires-Dist: pytest-cov; extra == "dev" Requires-Dist: pytest-xdist; extra ==
-"dev" Requires-Dist: google-cloud-aiplatform; extra == "dev" Requires-Dist:
-google-cloud-bigquery; extra == "dev" Requires-Dist: google-cloud-bigquery-
-storage; extra == "dev" Requires-Dist: google-cloud-secret-manager; extra ==
-"dev" Requires-Dist: google-cloud-storage; extra == "dev" # `prefect-gcp`
-         _[_P_y_P_I_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_P_r_e_f_e_c_t_H_Q_/_p_r_e_f_e_c_t_-
-  _g_c_p_?_c_o_l_o_r_=_0_0_5_2_F_F_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_p_r_e_f_e_c_t_-
-   _g_c_p_?_c_o_l_o_r_=_0_0_5_2_F_F_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_c_o_m_m_i_t_-
-       _a_c_t_i_v_i_t_y_/_m_/_P_r_e_f_e_c_t_H_Q_/_p_r_e_f_e_c_t_-_g_c_p_?_c_o_l_o_r_=_0_0_5_2_F_F_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_]
-              _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_s_l_a_c_k_-_j_o_i_n___c_o_m_m_u_n_i_t_y_-
-  _r_e_d_._s_v_g_?_c_o_l_o_r_=_0_0_5_2_F_F_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_&_l_o_g_o_=_s_l_a_c_k_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-                         _b_a_d_g_e_/_d_i_s_c_o_u_r_s_e_-_b_r_o_w_s_e___f_o_r_u_m_-
-            _r_e_d_._s_v_g_?_c_o_l_o_r_=_0_0_5_2_F_F_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_&_l_o_g_o_=_d_i_s_c_o_u_r_s_e_]
+Dist: pytest-asyncio; extra == "dev" Requires-Dist: pytest-xdist; extra ==
+"dev" Requires-Dist: pytest; extra == "dev" # `prefect-gcp`
+                _[_P_y_P_I_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_p_r_e_f_e_c_t_-
+                      _g_c_p_?_c_o_l_o_r_=_0_0_5_2_F_F_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_]
 `prefect-gcp` makes it easy to leverage the capabilities of Google Cloud
 Platform (GCP) in your flows, featuring support for Vertex AI, Cloud Run,
 BigQuery, Cloud Storage, and Secret Manager. Visit the full docs [here](https:/
 /PrefectHQ.github.io/prefect-gcp). ### Installation To start using `prefect-
 gcp`: ```bash pip install prefect-gcp ``` To install extras, see [here](https:/
 /prefecthq.github.io/prefect-gcp/#installation). ### Contributing Thanks for
 thinking about chipping in! Check out this [step-by-step guide](https://
```

### Comparing `prefect_gcp-0.5.8/README.md` & `prefect_gcp-0.5.9/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,14 @@
 # `prefect-gcp`
 
 <p align="center">
     <a href="https://pypi.python.org/pypi/prefect-gcp/" alt="PyPI version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-gcp?color=0052FF&labelColor=090422"></a>
-    <a href="https://github.com/PrefectHQ/prefect-gcp/" alt="Stars">
-        <img src="https://img.shields.io/github/stars/PrefectHQ/prefect-gcp?color=0052FF&labelColor=090422" /></a>
     <a href="https://pypistats.org/packages/prefect-gcp/" alt="Downloads">
         <img src="https://img.shields.io/pypi/dm/prefect-gcp?color=0052FF&labelColor=090422" /></a>
-    <a href="https://github.com/PrefectHQ/prefect-gcp/pulse" alt="Activity">
-        <img src="https://img.shields.io/github/commit-activity/m/PrefectHQ/prefect-gcp?color=0052FF&labelColor=090422" /></a>
-    <br>
-    <a href="https://prefect-community.slack.com" alt="Slack">
-        <img src="https://img.shields.io/badge/slack-join_community-red.svg?color=0052FF&labelColor=090422&logo=slack" /></a>
-    <a href="https://discourse.prefect.io/" alt="Discourse">
-        <img src="https://img.shields.io/badge/discourse-browse_forum-red.svg?color=0052FF&labelColor=090422&logo=discourse" /></a>
 </p>
 
 `prefect-gcp` makes it easy to leverage the capabilities of Google Cloud Platform (GCP) in your flows, featuring support for Vertex AI, Cloud Run, BigQuery, Cloud Storage, and Secret Manager.
 
 Visit the full docs [here](https://PrefectHQ.github.io/prefect-gcp).
 
 ### Installation
```

#### html2text {}

```diff
@@ -1,16 +1,10 @@
 # `prefect-gcp`
-         _[_P_y_P_I_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_P_r_e_f_e_c_t_H_Q_/_p_r_e_f_e_c_t_-
-  _g_c_p_?_c_o_l_o_r_=_0_0_5_2_F_F_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_p_r_e_f_e_c_t_-
-   _g_c_p_?_c_o_l_o_r_=_0_0_5_2_F_F_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_c_o_m_m_i_t_-
-       _a_c_t_i_v_i_t_y_/_m_/_P_r_e_f_e_c_t_H_Q_/_p_r_e_f_e_c_t_-_g_c_p_?_c_o_l_o_r_=_0_0_5_2_F_F_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_]
-              _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_s_l_a_c_k_-_j_o_i_n___c_o_m_m_u_n_i_t_y_-
-  _r_e_d_._s_v_g_?_c_o_l_o_r_=_0_0_5_2_F_F_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_&_l_o_g_o_=_s_l_a_c_k_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-                         _b_a_d_g_e_/_d_i_s_c_o_u_r_s_e_-_b_r_o_w_s_e___f_o_r_u_m_-
-            _r_e_d_._s_v_g_?_c_o_l_o_r_=_0_0_5_2_F_F_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_&_l_o_g_o_=_d_i_s_c_o_u_r_s_e_]
+                _[_P_y_P_I_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_p_r_e_f_e_c_t_-
+                      _g_c_p_?_c_o_l_o_r_=_0_0_5_2_F_F_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_]
 `prefect-gcp` makes it easy to leverage the capabilities of Google Cloud
 Platform (GCP) in your flows, featuring support for Vertex AI, Cloud Run,
 BigQuery, Cloud Storage, and Secret Manager. Visit the full docs [here](https:/
 /PrefectHQ.github.io/prefect-gcp). ### Installation To start using `prefect-
 gcp`: ```bash pip install prefect-gcp ``` To install extras, see [here](https:/
 /prefecthq.github.io/prefect-gcp/#installation). ### Contributing Thanks for
 thinking about chipping in! Check out this [step-by-step guide](https://
```

### Comparing `prefect_gcp-0.5.8/prefect_gcp/__init__.py` & `prefect_gcp-0.5.9/prefect_gcp/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,8 +17,8 @@
     "prefect_gcp.projects", "prefect_gcp.deployments", start_date="Jun 2023"
 )
 register_renamed_module(
     "prefect_gcp.worker", "prefect_gcp.workers", start_date="Sep 2023"
 )
 
 
-__version__ = _version.get_versions()["version"]
+__version__ = _version.__version__
```

### Comparing `prefect_gcp-0.5.8/prefect_gcp/aiplatform.py` & `prefect_gcp-0.5.9/prefect_gcp/aiplatform.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 This module is deprecated as of March 2024 and will not be available after September 2024.
 It has been replaced by the Vertex AI worker, which offers enhanced functionality and better performance.
 
 For upgrade instructions, see https://docs.prefect.io/latest/guides/upgrade-guide-agents-to-workers/.
 
 Integrations with Google AI Platform.
 
-Note this module is experimental. The intefaces within may change without notice.
-
 Examples:
 
     Run a job using Vertex AI Custom Training:
     ```python
     from prefect_gcp.credentials import GcpCredentials
     from prefect_gcp.aiplatform import VertexAICustomTrainingJob
 
@@ -61,19 +59,20 @@
 import re
 import shlex
 import time
 from typing import Dict, List, Optional, Tuple
 from uuid import uuid4
 
 from anyio.abc import TaskStatus
+from pydantic import VERSION as PYDANTIC_VERSION
+
 from prefect._internal.compatibility.deprecated import deprecated_class
 from prefect.exceptions import InfrastructureNotFound
 from prefect.infrastructure import Infrastructure, InfrastructureResult
 from prefect.utilities.asyncutils import run_sync_in_worker_thread, sync_compatible
-from pydantic import VERSION as PYDANTIC_VERSION
 
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import Field
 else:
     from pydantic import Field
 
 from slugify import slugify
@@ -99,15 +98,14 @@
 except ModuleNotFoundError:
     pass
 
 from prefect.blocks.core import BlockNotSavedError
 from prefect.workers.utilities import (
     get_default_base_job_template_for_infrastructure_type,
 )
-
 from prefect_gcp.credentials import GcpCredentials
 
 _DISALLOWED_GCP_LABEL_CHARACTERS = re.compile(r"[^-a-zA-Z0-9_]+")
 
 
 class VertexAICustomTrainingJobResult(InfrastructureResult):
     """Result from a Vertex AI custom training job."""
```

### Comparing `prefect_gcp-0.5.8/prefect_gcp/bigquery.py` & `prefect_gcp-0.5.9/prefect_gcp/bigquery.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 
 import os
 from functools import partial
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 from anyio import to_thread
+from pydantic import VERSION as PYDANTIC_VERSION
+
 from prefect import get_run_logger, task
 from prefect.blocks.abstract import DatabaseBlock
 from prefect.utilities.asyncutils import run_sync_in_worker_thread, sync_compatible
 from prefect.utilities.hashing import hash_objects
-from pydantic import VERSION as PYDANTIC_VERSION
 
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import Field
 else:
     from pydantic import Field
 
 from prefect_gcp.credentials import GcpCredentials
```

### Comparing `prefect_gcp-0.5.8/prefect_gcp/cloud_run.py` & `prefect_gcp-0.5.9/prefect_gcp/cloud_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 This module is deprecated as of March 2024 and will not be available after September 2024.
 It has been replaced by the Cloud Run and Cloud Run V2 workers, which offer enhanced functionality and better performance.
 
 For upgrade instructions, see https://docs.prefect.io/latest/guides/upgrade-guide-agents-to-workers/.
 
 Integrations with Google Cloud Run Job.
 
-Note this module is experimental. The intefaces within may change without notice.
-
 Examples:
 
     Run a job using Google Cloud Run Jobs:
     ```python
     CloudRunJob(
         image="gcr.io/my-project/my-image",
         region="us-east1",
@@ -43,31 +41,32 @@
 from uuid import uuid4
 
 import googleapiclient
 from anyio.abc import TaskStatus
 from google.api_core.client_options import ClientOptions
 from googleapiclient import discovery
 from googleapiclient.discovery import Resource
+from pydantic import VERSION as PYDANTIC_VERSION
+
 from prefect._internal.compatibility.deprecated import deprecated_class
 from prefect.exceptions import InfrastructureNotFound
 from prefect.infrastructure.base import Infrastructure, InfrastructureResult
 from prefect.utilities.asyncutils import run_sync_in_worker_thread, sync_compatible
-from pydantic import VERSION as PYDANTIC_VERSION
 
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import BaseModel, Field, root_validator, validator
 else:
     from pydantic import BaseModel, Field, root_validator, validator
 
+from typing_extensions import Literal
+
 from prefect.blocks.core import BlockNotSavedError
 from prefect.workers.utilities import (
     get_default_base_job_template_for_infrastructure_type,
 )
-from typing_extensions import Literal
-
 from prefect_gcp.credentials import GcpCredentials
 
 
 class Job(BaseModel):
     """
     Utility class to call GCP `jobs` API and
     interact with the returned objects.
```

### Comparing `prefect_gcp-0.5.8/prefect_gcp/cloud_storage.py` & `prefect_gcp-0.5.9/prefect_gcp/cloud_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 import asyncio
 import os
 from enum import Enum
 from io import BytesIO
 from pathlib import Path, PurePosixPath
 from typing import Any, BinaryIO, Dict, List, Optional, Tuple, Union
 
+from pydantic import VERSION as PYDANTIC_VERSION
+
 from prefect import get_run_logger, task
 from prefect.blocks.abstract import ObjectStorageBlock
 from prefect.filesystems import WritableDeploymentStorage, WritableFileSystem
 from prefect.logging import disable_run_logger
 from prefect.utilities.asyncutils import run_sync_in_worker_thread, sync_compatible
 from prefect.utilities.filesystem import filter_files
-from pydantic import VERSION as PYDANTIC_VERSION
 
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import Field, validator
 else:
     from pydantic import Field, validator
 
 # cannot be type_checking only or else `fields = cls.schema()` raises
```

### Comparing `prefect_gcp-0.5.8/prefect_gcp/credentials.py` & `prefect_gcp-0.5.9/prefect_gcp/credentials.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 from enum import Enum
 from pathlib import Path
 from typing import Any, Dict, Optional, Union
 
 import google.auth
 import google.auth.transport.requests
 from google.oauth2.service_account import Credentials
+from pydantic import VERSION as PYDANTIC_VERSION
+
 from prefect.blocks.abstract import CredentialsBlock
 from prefect.blocks.fields import SecretDict
 from prefect.utilities.asyncutils import run_sync_in_worker_thread, sync_compatible
-from pydantic import VERSION as PYDANTIC_VERSION
 
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import Field, root_validator, validator
 else:
     from pydantic import Field, root_validator, validator
 
 try:
@@ -68,15 +69,14 @@
 
         return inner
 
     return outer
 
 
 class ClientType(Enum):
-
     CLOUD_STORAGE = "cloud_storage"
     BIGQUERY = "bigquery"
     SECRET_MANAGER = "secret_manager"
     AIPLATFORM = "job_service"  # vertex ai
 
 
 class GcpCredentials(CredentialsBlock):
```

### Comparing `prefect_gcp-0.5.8/prefect_gcp/deployments/steps.py` & `prefect_gcp-0.5.9/prefect_gcp/deployments/steps.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 """
 from pathlib import Path, PurePosixPath
 from typing import Dict, Optional
 
 import google.auth
 from google.cloud.storage import Client as StorageClient
 from google.oauth2.service_account import Credentials
+from typing_extensions import TypedDict
+
 from prefect._internal.compatibility.deprecated import deprecated_callable
 from prefect.utilities.filesystem import filter_files, relative_path_to_current_platform
-from typing_extensions import TypedDict
 
 
 class PushToGcsOutput(TypedDict):
     """
     The output of the `push_to_gcs` step.
     """
```

### Comparing `prefect_gcp-0.5.8/prefect_gcp/models/cloud_run_v2.py` & `prefect_gcp-0.5.9/prefect_gcp/models/cloud_run_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import time
 from typing import Dict, List, Literal, Optional
 
 # noinspection PyProtectedMember
 from googleapiclient.discovery import Resource
-from prefect.infrastructure.base import InfrastructureResult
 from pydantic import VERSION as PYDANTIC_VERSION
 
+from prefect.infrastructure.base import InfrastructureResult
+
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import BaseModel
 else:
     from pydantic import BaseModel
 
 
 class JobV2(BaseModel):
```

### Comparing `prefect_gcp-0.5.8/prefect_gcp/secret_manager.py` & `prefect_gcp-0.5.9/prefect_gcp/secret_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from functools import partial
 from typing import Optional, Union
 
 from anyio import to_thread
 from google.api_core.exceptions import NotFound
+from pydantic import VERSION as PYDANTIC_VERSION
+
 from prefect import get_run_logger, task
 from prefect.blocks.abstract import SecretBlock
 from prefect.utilities.asyncutils import run_sync_in_worker_thread, sync_compatible
-from pydantic import VERSION as PYDANTIC_VERSION
 
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import Field
 else:
     from pydantic import Field
 
 from prefect_gcp.credentials import GcpCredentials
```

### Comparing `prefect_gcp-0.5.8/prefect_gcp/utilities.py` & `prefect_gcp-0.5.9/prefect_gcp/utilities.py`

 * *Files identical despite different names*

### Comparing `prefect_gcp-0.5.8/prefect_gcp/workers/cloud_run.py` & `prefect_gcp-0.5.9/prefect_gcp/workers/cloud_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,26 +159,27 @@
 
 import anyio
 import googleapiclient
 from anyio.abc import TaskStatus  # noqa
 from google.api_core.client_options import ClientOptions
 from googleapiclient import discovery
 from googleapiclient.discovery import Resource
+from pydantic import VERSION as PYDANTIC_VERSION
+
 from prefect.exceptions import InfrastructureNotFound
 from prefect.logging.loggers import PrefectLogAdapter
 from prefect.utilities.asyncutils import run_sync_in_worker_thread
 from prefect.utilities.dockerutils import get_prefect_image_name
 from prefect.utilities.pydantic import JsonPatch
 from prefect.workers.base import (
     BaseJobConfiguration,
     BaseVariables,
     BaseWorker,
     BaseWorkerResult,
 )
-from pydantic import VERSION as PYDANTIC_VERSION
 
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import Field, validator
 else:
     from pydantic import Field, validator
 
 from prefect_gcp.cloud_run import Execution, Job
```

### Comparing `prefect_gcp-0.5.8/prefect_gcp/workers/cloud_run_v2.py` & `prefect_gcp-0.5.9/prefect_gcp/workers/cloud_run_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,31 +7,32 @@
 from anyio.abc import TaskStatus
 from google.api_core.client_options import ClientOptions
 from googleapiclient import discovery
 
 # noinspection PyProtectedMember
 from googleapiclient.discovery import Resource
 from googleapiclient.errors import HttpError
+from pydantic import VERSION as PYDANTIC_VERSION
+
 from prefect.exceptions import InfrastructureNotFound
 from prefect.logging.loggers import PrefectLogAdapter
 from prefect.utilities.asyncutils import run_sync_in_worker_thread
 from prefect.utilities.dockerutils import get_prefect_image_name
 from prefect.utilities.pydantic import JsonPatch
 from prefect.workers.base import (
     BaseJobConfiguration,
     BaseVariables,
     BaseWorker,
     BaseWorkerResult,
 )
-from pydantic import VERSION as PYDANTIC_VERSION
 
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import Field, PrivateAttr, validator
 else:
-    from pydantic import Field, validator, PrivateAttr
+    from pydantic import Field, PrivateAttr, validator
 
 from prefect_gcp.credentials import GcpCredentials
 from prefect_gcp.models.cloud_run_v2 import CloudRunJobV2Result, ExecutionV2, JobV2
 from prefect_gcp.utilities import slugify_name
 
 if TYPE_CHECKING:
     from prefect.client.schemas import FlowRun
```

### Comparing `prefect_gcp-0.5.8/prefect_gcp/workers/vertex.py` & `prefect_gcp-0.5.9/prefect_gcp/workers/vertex.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,25 +22,26 @@
 import re
 import shlex
 import time
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple
 from uuid import uuid4
 
 import anyio
+from pydantic import VERSION as PYDANTIC_VERSION
+
 from prefect.exceptions import InfrastructureNotFound
 from prefect.logging.loggers import PrefectLogAdapter
 from prefect.utilities.asyncutils import run_sync_in_worker_thread
 from prefect.utilities.pydantic import JsonPatch
 from prefect.workers.base import (
     BaseJobConfiguration,
     BaseVariables,
     BaseWorker,
     BaseWorkerResult,
 )
-from pydantic import VERSION as PYDANTIC_VERSION
 
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import Field, validator
 else:
     from pydantic import Field, validator
 
 from slugify import slugify
```

### Comparing `prefect_gcp-0.5.8/prefect_gcp.egg-info/PKG-INFO` & `prefect_gcp-0.5.9/prefect_gcp.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: prefect-gcp
-Version: 0.5.8
-Summary: Prefect tasks and subflows for interacting with Google Cloud Platform.
-Home-page: https://github.com/PrefectHQ/prefect-gcp
-Author: Prefect Technologies, Inc.
-Author-email: help@prefect.io
+Version: 0.5.9
+Summary: Prefect integrations for interacting with Google Cloud Platform.
+Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
+Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-gcp
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
 Requires-Dist: prefect>=2.16.4
 Requires-Dist: google-api-python-client>=2.20.0
 Requires-Dist: google-cloud-storage>=2.0.0
 Requires-Dist: tenacity>=8.0.0
 Requires-Dist: python-slugify>=8.0.0
 Provides-Extra: cloud-storage
 Requires-Dist: google-cloud-storage; extra == "cloud-storage"
@@ -31,61 +30,48 @@
 Requires-Dist: google-cloud-bigquery; extra == "bigquery"
 Requires-Dist: google-cloud-bigquery-storage; extra == "bigquery"
 Provides-Extra: secret-manager
 Requires-Dist: google-cloud-secret-manager; extra == "secret-manager"
 Provides-Extra: aiplatform
 Requires-Dist: google-cloud-aiplatform; extra == "aiplatform"
 Provides-Extra: all-extras
-Requires-Dist: google-cloud-aiplatform; extra == "all-extras"
+Requires-Dist: google-cloud-storage; extra == "all-extras"
 Requires-Dist: google-cloud-bigquery; extra == "all-extras"
 Requires-Dist: google-cloud-bigquery-storage; extra == "all-extras"
 Requires-Dist: google-cloud-secret-manager; extra == "all-extras"
-Requires-Dist: google-cloud-storage; extra == "all-extras"
+Requires-Dist: google-cloud-aiplatform; extra == "all-extras"
 Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
-Requires-Dist: flake8; extra == "dev"
+Requires-Dist: google-cloud-aiplatform; extra == "dev"
+Requires-Dist: google-cloud-bigquery-storage; extra == "dev"
+Requires-Dist: google-cloud-bigquery; extra == "dev"
+Requires-Dist: google-cloud-secret-manager; extra == "dev"
+Requires-Dist: google-cloud-storage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
-Requires-Dist: isort; extra == "dev"
-Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
+Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
 Requires-Dist: mock; python_version < "3.8" and extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pandas; extra == "dev"
 Requires-Dist: pillow; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pyarrow; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
-Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
-Requires-Dist: google-cloud-aiplatform; extra == "dev"
-Requires-Dist: google-cloud-bigquery; extra == "dev"
-Requires-Dist: google-cloud-bigquery-storage; extra == "dev"
-Requires-Dist: google-cloud-secret-manager; extra == "dev"
-Requires-Dist: google-cloud-storage; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
 
 # `prefect-gcp`
 
 <p align="center">
     <a href="https://pypi.python.org/pypi/prefect-gcp/" alt="PyPI version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-gcp?color=0052FF&labelColor=090422"></a>
-    <a href="https://github.com/PrefectHQ/prefect-gcp/" alt="Stars">
-        <img src="https://img.shields.io/github/stars/PrefectHQ/prefect-gcp?color=0052FF&labelColor=090422" /></a>
     <a href="https://pypistats.org/packages/prefect-gcp/" alt="Downloads">
         <img src="https://img.shields.io/pypi/dm/prefect-gcp?color=0052FF&labelColor=090422" /></a>
-    <a href="https://github.com/PrefectHQ/prefect-gcp/pulse" alt="Activity">
-        <img src="https://img.shields.io/github/commit-activity/m/PrefectHQ/prefect-gcp?color=0052FF&labelColor=090422" /></a>
-    <br>
-    <a href="https://prefect-community.slack.com" alt="Slack">
-        <img src="https://img.shields.io/badge/slack-join_community-red.svg?color=0052FF&labelColor=090422&logo=slack" /></a>
-    <a href="https://discourse.prefect.io/" alt="Discourse">
-        <img src="https://img.shields.io/badge/discourse-browse_forum-red.svg?color=0052FF&labelColor=090422&logo=discourse" /></a>
 </p>
 
 `prefect-gcp` makes it easy to leverage the capabilities of Google Cloud Platform (GCP) in your flows, featuring support for Vertex AI, Cloud Run, BigQuery, Cloud Storage, and Secret Manager.
 
 Visit the full docs [here](https://PrefectHQ.github.io/prefect-gcp).
 
 ### Installation
```

#### html2text {}

```diff
@@ -1,54 +1,48 @@
-Metadata-Version: 2.1 Name: prefect-gcp Version: 0.5.8 Summary: Prefect tasks
-and subflows for interacting with Google Cloud Platform. Home-page: https://
-github.com/PrefectHQ/prefect-gcp Author: Prefect Technologies, Inc. Author-
-email: help@prefect.io License: Apache License 2.0 Keywords: prefect
-Classifier: Natural Language :: English Classifier: Intended Audience ::
-Developers Classifier: Intended Audience :: System Administrators Classifier:
-License :: OSI Approved :: Apache Software License Classifier: Programming
-Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
-3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries Requires-Python: >=3.7
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-prefect>=2.16.4 Requires-Dist: google-api-python-client>=2.20.0 Requires-Dist:
-google-cloud-storage>=2.0.0 Requires-Dist: tenacity>=8.0.0 Requires-Dist:
-python-slugify>=8.0.0 Provides-Extra: cloud-storage Requires-Dist: google-
-cloud-storage; extra == "cloud-storage" Provides-Extra: bigquery Requires-Dist:
-google-cloud-bigquery; extra == "bigquery" Requires-Dist: google-cloud-
-bigquery-storage; extra == "bigquery" Provides-Extra: secret-manager Requires-
-Dist: google-cloud-secret-manager; extra == "secret-manager" Provides-Extra:
-aiplatform Requires-Dist: google-cloud-aiplatform; extra == "aiplatform"
-Provides-Extra: all-extras Requires-Dist: google-cloud-aiplatform; extra ==
-"all-extras" Requires-Dist: google-cloud-bigquery; extra == "all-extras"
-Requires-Dist: google-cloud-bigquery-storage; extra == "all-extras" Requires-
-Dist: google-cloud-secret-manager; extra == "all-extras" Requires-Dist: google-
-cloud-storage; extra == "all-extras" Provides-Extra: dev Requires-Dist: black;
-extra == "dev" Requires-Dist: coverage; extra == "dev" Requires-Dist: flake8;
-extra == "dev" Requires-Dist: interrogate; extra == "dev" Requires-Dist: isort;
-extra == "dev" Requires-Dist: mkdocs; extra == "dev" Requires-Dist: mkdocs-gen-
-files; extra == "dev" Requires-Dist: mkdocs-material; extra == "dev" Requires-
-Dist: mkdocstrings[python]; extra == "dev" Requires-Dist: mock; python_version
-< "3.8" and extra == "dev" Requires-Dist: mypy; extra == "dev" Requires-Dist:
+Metadata-Version: 2.1 Name: prefect-gcp Version: 0.5.9 Summary: Prefect
+integrations for interacting with Google Cloud Platform. Author-email: "Prefect
+Technologies, Inc."
+prefect.io> License: Apache License 2.0 Project-URL: Homepage, https://
+github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-gcp Keywords:
+prefect Classifier: Natural Language :: English Classifier: Intended Audience
+:: Developers Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: Apache Software License Classifier:
+Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
+Topic :: Software Development :: Libraries Requires-Python: >=3.8 Description-
+Content-Type: text/markdown Requires-Dist: prefect>=2.16.4 Requires-Dist:
+google-api-python-client>=2.20.0 Requires-Dist: google-cloud-storage>=2.0.0
+Requires-Dist: tenacity>=8.0.0 Requires-Dist: python-slugify>=8.0.0 Provides-
+Extra: cloud-storage Requires-Dist: google-cloud-storage; extra == "cloud-
+storage" Provides-Extra: bigquery Requires-Dist: google-cloud-bigquery; extra
+== "bigquery" Requires-Dist: google-cloud-bigquery-storage; extra == "bigquery"
+Provides-Extra: secret-manager Requires-Dist: google-cloud-secret-manager;
+extra == "secret-manager" Provides-Extra: aiplatform Requires-Dist: google-
+cloud-aiplatform; extra == "aiplatform" Provides-Extra: all-extras Requires-
+Dist: google-cloud-storage; extra == "all-extras" Requires-Dist: google-cloud-
+bigquery; extra == "all-extras" Requires-Dist: google-cloud-bigquery-storage;
+extra == "all-extras" Requires-Dist: google-cloud-secret-manager; extra ==
+"all-extras" Requires-Dist: google-cloud-aiplatform; extra == "all-extras"
+Provides-Extra: dev Requires-Dist: coverage; extra == "dev" Requires-Dist:
+google-cloud-aiplatform; extra == "dev" Requires-Dist: google-cloud-bigquery-
+storage; extra == "dev" Requires-Dist: google-cloud-bigquery; extra == "dev"
+Requires-Dist: google-cloud-secret-manager; extra == "dev" Requires-Dist:
+google-cloud-storage; extra == "dev" Requires-Dist: interrogate; extra == "dev"
+Requires-Dist: mkdocs-gen-files; extra == "dev" Requires-Dist: mkdocs-material;
+extra == "dev" Requires-Dist: mkdocs; extra == "dev" Requires-Dist:
+mkdocstrings[python]; extra == "dev" Requires-Dist: mock; python_version <
+"3.8" and extra == "dev" Requires-Dist: mypy; extra == "dev" Requires-Dist:
 pandas; extra == "dev" Requires-Dist: pillow; extra == "dev" Requires-Dist:
 pre-commit; extra == "dev" Requires-Dist: pyarrow; extra == "dev" Requires-
-Dist: pytest; extra == "dev" Requires-Dist: pytest-asyncio; extra == "dev"
-Requires-Dist: pytest-cov; extra == "dev" Requires-Dist: pytest-xdist; extra ==
-"dev" Requires-Dist: google-cloud-aiplatform; extra == "dev" Requires-Dist:
-google-cloud-bigquery; extra == "dev" Requires-Dist: google-cloud-bigquery-
-storage; extra == "dev" Requires-Dist: google-cloud-secret-manager; extra ==
-"dev" Requires-Dist: google-cloud-storage; extra == "dev" # `prefect-gcp`
-         _[_P_y_P_I_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_P_r_e_f_e_c_t_H_Q_/_p_r_e_f_e_c_t_-
-  _g_c_p_?_c_o_l_o_r_=_0_0_5_2_F_F_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_p_r_e_f_e_c_t_-
-   _g_c_p_?_c_o_l_o_r_=_0_0_5_2_F_F_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_c_o_m_m_i_t_-
-       _a_c_t_i_v_i_t_y_/_m_/_P_r_e_f_e_c_t_H_Q_/_p_r_e_f_e_c_t_-_g_c_p_?_c_o_l_o_r_=_0_0_5_2_F_F_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_]
-              _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_s_l_a_c_k_-_j_o_i_n___c_o_m_m_u_n_i_t_y_-
-  _r_e_d_._s_v_g_?_c_o_l_o_r_=_0_0_5_2_F_F_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_&_l_o_g_o_=_s_l_a_c_k_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-                         _b_a_d_g_e_/_d_i_s_c_o_u_r_s_e_-_b_r_o_w_s_e___f_o_r_u_m_-
-            _r_e_d_._s_v_g_?_c_o_l_o_r_=_0_0_5_2_F_F_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_&_l_o_g_o_=_d_i_s_c_o_u_r_s_e_]
+Dist: pytest-asyncio; extra == "dev" Requires-Dist: pytest-xdist; extra ==
+"dev" Requires-Dist: pytest; extra == "dev" # `prefect-gcp`
+                _[_P_y_P_I_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_p_r_e_f_e_c_t_-
+                      _g_c_p_?_c_o_l_o_r_=_0_0_5_2_F_F_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_]
 `prefect-gcp` makes it easy to leverage the capabilities of Google Cloud
 Platform (GCP) in your flows, featuring support for Vertex AI, Cloud Run,
 BigQuery, Cloud Storage, and Secret Manager. Visit the full docs [here](https:/
 /PrefectHQ.github.io/prefect-gcp). ### Installation To start using `prefect-
 gcp`: ```bash pip install prefect-gcp ``` To install extras, see [here](https:/
 /prefecthq.github.io/prefect-gcp/#installation). ### Contributing Thanks for
 thinking about chipping in! Check out this [step-by-step guide](https://
```

### Comparing `prefect_gcp-0.5.8/prefect_gcp.egg-info/SOURCES.txt` & `prefect_gcp-0.5.9/prefect_gcp.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,9 @@
-LICENSE
-MANIFEST.in
 README.md
-requirements-dev.txt
-requirements.txt
-setup.cfg
-setup.py
-versioneer.py
+pyproject.toml
 prefect_gcp/__init__.py
 prefect_gcp/_version.py
 prefect_gcp/aiplatform.py
 prefect_gcp/bigquery.py
 prefect_gcp/cloud_run.py
 prefect_gcp/cloud_storage.py
 prefect_gcp/credentials.py
@@ -25,19 +19,22 @@
 prefect_gcp/deployments/steps.py
 prefect_gcp/models/__init__.py
 prefect_gcp/models/cloud_run_v2.py
 prefect_gcp/workers/__init__.py
 prefect_gcp/workers/cloud_run.py
 prefect_gcp/workers/cloud_run_v2.py
 prefect_gcp/workers/vertex.py
+tests/conftest.py
 tests/test_aiplatform.py
 tests/test_bigquery.py
 tests/test_block_standards.py
 tests/test_cloud_run.py
 tests/test_cloud_run_v2.py
 tests/test_cloud_run_worker.py
 tests/test_cloud_run_worker_v2.py
 tests/test_cloud_storage.py
 tests/test_credentials.py
 tests/test_deprecation.py
 tests/test_secret_manager.py
-tests/test_vertex_worker.py
+tests/test_version.py
+tests/test_vertex_worker.py
+tests/projects/test_steps.py
```

### Comparing `prefect_gcp-0.5.8/prefect_gcp.egg-info/requires.txt` & `prefect_gcp-0.5.9/prefect_gcp.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,50 +4,46 @@
 tenacity>=8.0.0
 python-slugify>=8.0.0
 
 [aiplatform]
 google-cloud-aiplatform
 
 [all_extras]
-google-cloud-aiplatform
+google-cloud-storage
 google-cloud-bigquery
 google-cloud-bigquery-storage
 google-cloud-secret-manager
-google-cloud-storage
+google-cloud-aiplatform
 
 [bigquery]
 google-cloud-bigquery
 google-cloud-bigquery-storage
 
 [cloud_storage]
 google-cloud-storage
 
 [dev]
-black
 coverage
-flake8
+google-cloud-aiplatform
+google-cloud-bigquery-storage
+google-cloud-bigquery
+google-cloud-secret-manager
+google-cloud-storage
 interrogate
-isort
-mkdocs
 mkdocs-gen-files
 mkdocs-material
+mkdocs
 mkdocstrings[python]
 mypy
 pandas
 pillow
 pre-commit
 pyarrow
-pytest
 pytest-asyncio
-pytest-cov
 pytest-xdist
-google-cloud-aiplatform
-google-cloud-bigquery
-google-cloud-bigquery-storage
-google-cloud-secret-manager
-google-cloud-storage
+pytest
 
 [dev:python_version < "3.8"]
 mock
 
 [secret_manager]
 google-cloud-secret-manager
```

### Comparing `prefect_gcp-0.5.8/tests/test_aiplatform.py` & `prefect_gcp-0.5.9/tests/test_aiplatform.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from copy import deepcopy
 from unittest.mock import MagicMock, patch
 
 import pytest
 from google.cloud.aiplatform_v1.types.accelerator_type import AcceleratorType
 from google.cloud.aiplatform_v1.types.job_state import JobState
-from prefect.exceptions import InfrastructureNotFound
-from tenacity import RetryError
-
 from prefect_gcp.aiplatform import (
     VertexAICustomTrainingJob,
     VertexAICustomTrainingJobResult,
 )
 from prefect_gcp.credentials import GcpCredentials
 from prefect_gcp.workers.vertex import VertexAIWorker
+from tenacity import RetryError
+
+from prefect.exceptions import InfrastructureNotFound
 
 
 class TestVertexAICustomTrainingJob:
     @pytest.fixture
     def vertex_ai_custom_training_job(self, gcp_credentials):
         return VertexAICustomTrainingJob(
             command=["echo", "hello!!"],
```

### Comparing `prefect_gcp-0.5.8/tests/test_bigquery.py` & `prefect_gcp-0.5.9/tests/test_bigquery.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import os
 from unittest.mock import MagicMock
 
 import pytest
 from google.cloud.bigquery import ExternalConfig, SchemaField
 from google.cloud.bigquery.dbapi.connection import Connection
-from prefect import flow
-
 from prefect_gcp.bigquery import (
     BigQueryWarehouse,
     bigquery_create_table,
     bigquery_insert_stream,
     bigquery_load_cloud_storage,
     bigquery_load_file,
     bigquery_query,
 )
 
+from prefect import flow
+
 
 @pytest.mark.parametrize("to_dataframe", [False, True])
 @pytest.mark.parametrize("result_transformer", [None, lambda _: ("test_transformer",)])
 @pytest.mark.parametrize("dry_run_max_bytes", [None, 5, 15])
 def test_bigquery_query(
     to_dataframe, result_transformer, dry_run_max_bytes, gcp_credentials
 ):
@@ -91,15 +91,14 @@
         with pytest.raises(ValueError, match="Either a schema or an external"):
             test_flow()
     else:
         assert test_flow() == "table"
 
 
 def test_bigquery_insert_stream(gcp_credentials):
-
     records = [
         {"number": 1, "text": "abc", "bool": True},
         {"number": 2, "text": "def", "bool": False},
     ]
 
     @flow
     def test_flow():
@@ -130,15 +129,14 @@
     result = test_flow()
     assert result.output == "uri"
     assert result._client is None
     assert result._completion_lock is None
 
 
 def test_bigquery_load_file(gcp_credentials):
-
     path = os.path.abspath(__file__)
 
     @flow
     def test_flow():
         schema = [
             SchemaField("number", field_type="INTEGER", mode="REQUIRED"),
             SchemaField("text", field_type="STRING", mode="REQUIRED"),
@@ -180,15 +178,15 @@
         assert bigquery_warehouse.fetch_size == 2
 
     def test_close(self, bigquery_warehouse, mock_connection):
         bigquery_warehouse._connection = mock_connection
         assert bigquery_warehouse._connection is not None
         bigquery_warehouse.close()
         assert bigquery_warehouse._unique_cursors == {}
-        assert mock_connection._connection.close.called_once()
+        mock_connection.close.assert_called_once()
         assert bigquery_warehouse._connection is None
 
     def test_context_management(self, gcp_credentials):
         with BigQueryWarehouse(
             gcp_credentials=gcp_credentials, fetch_size=2
         ) as warehouse:
             assert isinstance(warehouse._connection, Connection)
```

### Comparing `prefect_gcp-0.5.8/tests/test_block_standards.py` & `prefect_gcp-0.5.9/tests/test_block_standards.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytest
+
 from prefect.blocks.core import Block
 from prefect.testing.standard_test_suites import BlockStandardTestSuite
 from prefect.utilities.dispatch import get_registry_for_type
 from prefect.utilities.importtools import to_qualified_name
 
 
 def find_module_blocks():
```

### Comparing `prefect_gcp-0.5.8/tests/test_cloud_run.py` & `prefect_gcp-0.5.9/tests/test_cloud_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 from copy import deepcopy
 from unittest.mock import Mock
 
 import anyio
-from pydantic import VERSION as PYDANTIC_VERSION
-
 from prefect_gcp.workers.cloud_run import CloudRunWorker
+from pydantic import VERSION as PYDANTIC_VERSION
 
 if PYDANTIC_VERSION.startswith("2."):
     import pydantic.v1 as pydantic
 else:
     import pydantic
 
 import pytest
 from googleapiclient.errors import HttpError
+from prefect_gcp.cloud_run import CloudRunJob, CloudRunJobResult, Execution, Job
+from prefect_gcp.credentials import GcpCredentials
+
 from prefect.exceptions import InfrastructureNotFound
 from prefect.settings import (
     PREFECT_API_KEY,
     PREFECT_API_URL,
     PREFECT_LOGGING_TO_API_ENABLED,
     PREFECT_PROFILES_PATH,
     temporary_settings,
 )
 
-from prefect_gcp.cloud_run import CloudRunJob, CloudRunJobResult, Execution, Job
-from prefect_gcp.credentials import GcpCredentials
-
 executions_return_value = {
     "metadata": {"name": "test-name", "namespace": "test-namespace"},
     "spec": {"MySpec": "spec"},
     "status": {"logUri": "test-log-uri"},
 }
 
 jobs_return_value = {
```

### Comparing `prefect_gcp-0.5.8/tests/test_cloud_run_v2.py` & `prefect_gcp-0.5.9/tests/test_cloud_run_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from prefect_gcp.models.cloud_run_v2 import JobV2
 
 jobs_return_value = {
     "name": "test-job-name",
     "uid": "uid-123",
     "generation": "1",
     "labels": {},
```

### Comparing `prefect_gcp-0.5.8/tests/test_cloud_run_worker.py` & `prefect_gcp-0.5.9/tests/test_cloud_run_worker.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -8,26 +8,26 @@
     import pydantic.v1 as pydantic
 else:
     import pydantic
 
 import pytest
 from googleapiclient.errors import HttpError
 from jsonschema.exceptions import ValidationError
-from prefect.client.schemas import FlowRun
-from prefect.exceptions import InfrastructureNotFound
-from prefect.server.schemas.actions import DeploymentCreate
-
 from prefect_gcp.credentials import GcpCredentials
 from prefect_gcp.utilities import slugify_name
 from prefect_gcp.workers.cloud_run import (
     CloudRunWorker,
     CloudRunWorkerJobConfiguration,
     CloudRunWorkerResult,
 )
 
+from prefect.client.schemas import FlowRun
+from prefect.exceptions import InfrastructureNotFound
+from prefect.server.schemas.actions import DeploymentCreate
+
 
 @pytest.fixture(autouse=True)
 def mock_credentials(gcp_credentials):
     yield
 
 
 @pytest.fixture
```

### Comparing `prefect_gcp-0.5.8/tests/test_cloud_run_worker_v2.py` & `prefect_gcp-0.5.9/tests/test_cloud_run_worker_v2.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest
-from prefect.utilities.dockerutils import get_prefect_image_name
-
 from prefect_gcp.credentials import GcpCredentials
 from prefect_gcp.utilities import slugify_name
 from prefect_gcp.workers.cloud_run_v2 import CloudRunWorkerJobV2Configuration
 
+from prefect.utilities.dockerutils import get_prefect_image_name
+
 
 @pytest.fixture
 def job_body():
     return {
         "client": "prefect",
         "launchStage": None,
         "template": {
```

### Comparing `prefect_gcp-0.5.8/tests/test_cloud_storage.py` & `prefect_gcp-0.5.9/tests/test_cloud_storage.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import os
 from io import BytesIO
 from pathlib import Path, PurePosixPath
 
 import pandas as pd
 import pytest
-from prefect import flow
-from prefect.deployments import Deployment
-
 from prefect_gcp.cloud_storage import (
     GcsBucket,
     cloud_storage_copy_blob,
     cloud_storage_create_bucket,
     cloud_storage_download_blob_as_bytes,
     cloud_storage_download_blob_to_file,
     cloud_storage_upload_blob_from_file,
     cloud_storage_upload_blob_from_string,
 )
 
+from prefect import flow
+from prefect.deployments import Deployment
+
 
 def test_cloud_storage_create_bucket(gcp_credentials):
     bucket = "expected"
     location = "US"
 
     @flow
     def test_flow():
```

### Comparing `prefect_gcp-0.5.8/tests/test_credentials.py` & `prefect_gcp-0.5.9/tests/test_credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import json
 import os
 from pathlib import Path
 
 import pytest
 from google.cloud.aiplatform.gapic import JobServiceClient
-from prefect import flow, task
-from prefect.blocks.core import Block
-
 from prefect_gcp import GcpCredentials
 from prefect_gcp.credentials import ClientType
 
+from prefect import flow, task
+from prefect.blocks.core import Block
+
 
 def _get_first_file_in_root():
     for path in os.listdir(os.path.expanduser("~")):
         if os.path.isfile(os.path.join(os.path.expanduser("~"), path)):
             return os.path.join("~", path)
 
 
@@ -56,15 +56,15 @@
     for key, value in service_account_info.items():
         assert getattr(credentials, key) == value
 
 
 def test_get_credentials_from_service_account_file_error(oauth2_credentials):
     with pytest.raises(ValueError):
         GcpCredentials(
-            service_account_file="~/doesnt/exist"
+            service_account_file="~/does_not/exist"
         ).get_credentials_from_service_account()
 
 
 def test_able_to_load_credentials_from_json_string(service_account_info_json):
     gcp_credentials = GcpCredentials(service_account_info=service_account_info_json)
     assert gcp_credentials.service_account_info.get_secret_value() == {
         "project_id": "my_project",
```

### Comparing `prefect_gcp-0.5.8/tests/test_deprecation.py` & `prefect_gcp-0.5.9/tests/test_deprecation.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
-from prefect._internal.compatibility.deprecated import PrefectDeprecationWarning
-
 from prefect_gcp.aiplatform import VertexAICustomTrainingJob
 from prefect_gcp.cloud_run import CloudRunJob
 
+from prefect._internal.compatibility.deprecated import PrefectDeprecationWarning
+
 
 @pytest.mark.parametrize(
     "InfraBlock, kwargs, expected_message",
     [
         (
             CloudRunJob,
             {"image": "foo", "region": "us-central1"},
```

### Comparing `prefect_gcp-0.5.8/tests/test_secret_manager.py` & `prefect_gcp-0.5.9/tests/test_secret_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import pytest
-from prefect import flow
-
 from prefect_gcp.secret_manager import (
     GcpSecret,
     create_secret,
     delete_secret,
     delete_secret_version,
     read_secret,
     update_secret,
 )
 
+from prefect import flow
+
 
 def test_create_secret(gcp_credentials):
     @flow
     def test_flow():
         return create_secret("secret_name", gcp_credentials)
 
     assert test_flow() == "projects/gcp_credentials_project/secrets/secret_name"
@@ -39,30 +39,28 @@
 
     expected = "secret_data"
     assert test_flow() == expected
 
 
 @pytest.mark.parametrize("project", [None, "override_project"])
 def test_delete_secret(project, gcp_credentials):
-
     secret_name = "secret_name"
 
     @flow
     def test_flow():
         return delete_secret(secret_name, gcp_credentials, project=project)
 
     project = project or gcp_credentials.project
     path = f"projects/{project}/secrets/{secret_name}/"
     assert test_flow() == path
 
 
 @pytest.mark.parametrize("project", [None, "override_project"])
 @pytest.mark.parametrize("version_id", ["latest", 1])
 def test_delete_secret_version_id(project, version_id, gcp_credentials):
-
     secret_name = "secret_name"
 
     @flow
     def test_flow():
         return delete_secret_version(
             secret_name, version_id, gcp_credentials, project=project
         )
```

### Comparing `prefect_gcp-0.5.8/tests/test_vertex_worker.py` & `prefect_gcp-0.5.9/tests/test_vertex_worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,23 +9,23 @@
     import pydantic.v1 as pydantic
 else:
     import pydantic
 
 import pytest
 from google.cloud.aiplatform_v1.types.job_service import CancelCustomJobRequest
 from google.cloud.aiplatform_v1.types.job_state import JobState
-from prefect.client.schemas import FlowRun
-from prefect.exceptions import InfrastructureNotFound
-
 from prefect_gcp.workers.vertex import (
     VertexAIWorker,
     VertexAIWorkerJobConfiguration,
     VertexAIWorkerResult,
 )
 
+from prefect.client.schemas import FlowRun
+from prefect.exceptions import InfrastructureNotFound
+
 
 @pytest.fixture
 def job_config(service_account_info, gcp_credentials):
     return VertexAIWorkerJobConfiguration(
         name="my-custom-ai-job",
         region="ashenvale",
         credentials=gcp_credentials,
@@ -237,15 +237,14 @@
         self, flow_run, job_config, caplog
     ):
         mock = job_config.credentials.job_service_client.create_custom_job
         mock.return_value = SimpleNamespace(
             name="bazzbar", state=JobState.JOB_STATE_PENDING
         )
         async with VertexAIWorker("test-pool") as worker:
-
             input_grace_period = 32
 
             with anyio.fail_after(10):
                 async with anyio.create_task_group() as tg:
                     identifier = await tg.start(worker.run, flow_run, job_config)
                 await worker.kill_infrastructure(
                     identifier, job_config, input_grace_period
```

