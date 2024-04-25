# Comparing `tmp/prefect-dbt-0.4.1.tar.gz` & `tmp/prefect_dbt-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect-dbt-0.4.1.tar", last modified: Mon Nov 13 22:54:14 2023, max compression
+gzip compressed data, was "prefect_dbt-0.4.2.tar", last modified: Thu Apr 25 19:20:12 2024, max compression
```

## Comparing `prefect-dbt-0.4.1.tar` & `prefect_dbt-0.4.2.tar`

### file list

```diff
@@ -1,41 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 22:54:14.006147 prefect-dbt-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2023-11-13 22:52:47.000000 prefect-dbt-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      318 2023-11-13 22:52:47.000000 prefect-dbt-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14192 2023-11-13 22:54:14.006147 prefect-dbt-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11402 2023-11-13 22:52:47.000000 prefect-dbt-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 22:54:14.006147 prefect-dbt-0.4.1/prefect_dbt/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2023-11-13 22:52:47.000000 prefect-dbt-0.4.1/prefect_dbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2023-11-13 22:54:14.006147 prefect-dbt-0.4.1/prefect_dbt/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 22:54:13.998147 prefect-dbt-0.4.1/prefect_dbt/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      543 2023-11-13 22:52:47.000000 prefect-dbt-0.4.1/prefect_dbt/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15254 2023-11-13 22:52:47.000000 prefect-dbt-0.4.1/prefect_dbt/cli/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 22:54:13.998147 prefect-dbt-0.4.1/prefect_dbt/cli/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2023-11-13 22:52:47.000000 prefect-dbt-0.4.1/prefect_dbt/cli/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10507 2023-11-13 22:52:47.000000 prefect-dbt-0.4.1/prefect_dbt/cli/configs/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5768 2023-11-13 22:52:47.000000 prefect-dbt-0.4.1/prefect_dbt/cli/configs/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2023-11-13 22:52:47.000000 prefect-dbt-0.4.1/prefect_dbt/cli/configs/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2023-11-13 22:52:47.000000 prefect-dbt-0.4.1/prefect_dbt/cli/configs/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2023-11-13 22:52:47.000000 prefect-dbt-0.4.1/prefect_dbt/cli/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 22:54:14.002147 prefect-dbt-0.4.1/prefect_dbt/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2023-11-13 22:52:47.000000 prefect-dbt-0.4.1/prefect_dbt/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8538 2023-11-13 22:52:47.000000 prefect-dbt-0.4.1/prefect_dbt/cloud/clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     6518 2023-11-13 22:52:47.000000 prefect-dbt-0.4.1/prefect_dbt/cloud/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2023-11-13 22:52:47.000000 prefect-dbt-0.4.1/prefect_dbt/cloud/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    43411 2023-11-13 22:52:47.000000 prefect-dbt-0.4.1/prefect_dbt/cloud/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2023-11-13 22:52:47.000000 prefect-dbt-0.4.1/prefect_dbt/cloud/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     9943 2023-11-13 22:52:47.000000 prefect-dbt-0.4.1/prefect_dbt/cloud/runs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2023-11-13 22:52:47.000000 prefect-dbt-0.4.1/prefect_dbt/cloud/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 22:54:13.998147 prefect-dbt-0.4.1/prefect_dbt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14192 2023-11-13 22:54:13.000000 prefect-dbt-0.4.1/prefect_dbt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      885 2023-11-13 22:54:13.000000 prefect-dbt-0.4.1/prefect_dbt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-13 22:54:13.000000 prefect-dbt-0.4.1/prefect_dbt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-11-13 22:54:13.000000 prefect-dbt-0.4.1/prefect_dbt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      672 2023-11-13 22:54:13.000000 prefect-dbt-0.4.1/prefect_dbt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-11-13 22:54:13.000000 prefect-dbt-0.4.1/prefect_dbt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      180 2023-11-13 22:52:47.000000 prefect-dbt-0.4.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-11-13 22:52:47.000000 prefect-dbt-0.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      833 2023-11-13 22:54:14.006147 prefect-dbt-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2023-11-13 22:52:47.000000 prefect-dbt-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 22:54:14.002147 prefect-dbt-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2023-11-13 22:52:47.000000 prefect-dbt-0.4.1/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)    80049 2023-11-13 22:52:47.000000 prefect-dbt-0.4.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:12.740582 prefect_dbt-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    12649 2024-04-25 19:20:12.740582 prefect_dbt-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9853 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:12.728582 prefect_dbt-0.4.2/prefect_dbt/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/prefect_dbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 19:20:12.000000 prefect_dbt-0.4.2/prefect_dbt/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:12.732582 prefect_dbt-0.4.2/prefect_dbt/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/prefect_dbt/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15255 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/prefect_dbt/cli/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:12.732582 prefect_dbt-0.4.2/prefect_dbt/cli/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/prefect_dbt/cli/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10508 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/prefect_dbt/cli/configs/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/prefect_dbt/cli/configs/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/prefect_dbt/cli/configs/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/prefect_dbt/cli/configs/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/prefect_dbt/cli/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/prefect_dbt/cli/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:12.732582 prefect_dbt-0.4.2/prefect_dbt/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/prefect_dbt/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/prefect_dbt/cloud/clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/prefect_dbt/cloud/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/prefect_dbt/cloud/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43316 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/prefect_dbt/cloud/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/prefect_dbt/cloud/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9943 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/prefect_dbt/cloud/runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/prefect_dbt/cloud/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:12.736582 prefect_dbt-0.4.2/prefect_dbt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12649 2024-04-25 19:20:12.000000 prefect_dbt-0.4.2/prefect_dbt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-25 19:20:12.000000 prefect_dbt-0.4.2/prefect_dbt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:20:12.000000 prefect_dbt-0.4.2/prefect_dbt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-25 19:20:12.000000 prefect_dbt-0.4.2/prefect_dbt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-25 19:20:12.000000 prefect_dbt-0.4.2/prefect_dbt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 19:20:12.000000 prefect_dbt-0.4.2/prefect_dbt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:20:12.740582 prefect_dbt-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:12.732582 prefect_dbt-0.4.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:12.732582 prefect_dbt-0.4.2/tests/cli/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:12.736582 prefect_dbt-0.4.2/tests/cli/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/tests/cli/configs/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/tests/cli/configs/test_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/tests/cli/configs/test_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/tests/cli/configs/test_snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/tests/cli/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/tests/cli/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/tests/cli/test_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:12.736582 prefect_dbt-0.4.2/tests/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/tests/cloud/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/tests/cloud/test_cloud_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31500 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/tests/cloud/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/tests/cloud/test_runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/tests/cloud/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/tests/test_version.py
```

### Comparing `prefect-dbt-0.4.1/PKG-INFO` & `prefect_dbt-0.4.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: prefect-dbt
-Version: 0.4.1
-Summary: Prefect integration for working with dbt
-Home-page: https://github.com/PrefectHQ/prefect-dbt
-Author: Prefect Technologies, Inc.
-Author-email: help@prefect.io
+Version: 0.4.2
+Summary: Prefect integrations for working with dbt
+Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
+Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-dbt
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
-Requires-Dist: prefect>=2.13.5
+Requires-Dist: prefect>=2.16.6
 Requires-Dist: dbt_core>=1.1.1
-Requires-Dist: prefect_shell>=0.1.0
+Requires-Dist: prefect_shell>=0.1.4
 Requires-Dist: sgqlc>=16.0.0
 Provides-Extra: snowflake
 Requires-Dist: prefect-snowflake>=0.2.4; extra == "snowflake"
 Requires-Dist: dbt-snowflake; extra == "snowflake"
 Provides-Extra: bigquery
 Requires-Dist: prefect-gcp[bigquery]>=0.1.8; extra == "bigquery"
 Requires-Dist: dbt-bigquery; extra == "bigquery"
@@ -37,59 +36,44 @@
 Requires-Dist: dbt-bigquery; extra == "all-extras"
 Requires-Dist: dbt-postgres; extra == "all-extras"
 Requires-Dist: dbt-snowflake; extra == "all-extras"
 Requires-Dist: prefect-gcp[bigquery]>=0.1.8; extra == "all-extras"
 Requires-Dist: prefect-snowflake>=0.2.4; extra == "all-extras"
 Requires-Dist: prefect-sqlalchemy>=0.2.1; extra == "all-extras"
 Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: black; extra == "dev"
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: mypy; extra == "dev"
-Requires-Dist: mkdocs; extra == "dev"
-Requires-Dist: mkdocs-material; extra == "dev"
-Requires-Dist: mkdocstrings[python]; extra == "dev"
-Requires-Dist: isort; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: pytest-asyncio; extra == "dev"
-Requires-Dist: mock; python_version < "3.8" and extra == "dev"
-Requires-Dist: mkdocs-gen-files; extra == "dev"
-Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
-Requires-Dist: respx; extra == "dev"
-Requires-Dist: pillow; extra == "dev"
 Requires-Dist: dbt-bigquery; extra == "dev"
 Requires-Dist: dbt-postgres; extra == "dev"
 Requires-Dist: dbt-snowflake; extra == "dev"
+Requires-Dist: interrogate; extra == "dev"
+Requires-Dist: mkdocs-gen-files; extra == "dev"
+Requires-Dist: mkdocs-material; extra == "dev"
+Requires-Dist: mkdocs; extra == "dev"
+Requires-Dist: mkdocstrings[python]; extra == "dev"
+Requires-Dist: mock; python_version < "3.8" and extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: pillow; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: prefect-gcp[bigquery]>=0.1.8; extra == "dev"
 Requires-Dist: prefect-snowflake>=0.2.4; extra == "dev"
 Requires-Dist: prefect-sqlalchemy>=0.2.1; extra == "dev"
+Requires-Dist: pytest-asyncio; extra == "dev"
+Requires-Dist: pytest-xdist; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: respx; extra == "dev"
 
-# Coordinate and use dbt in your dataflow with prefect-dbt
+# prefect-dbt
 
 <p align="center">
-    <img src="https://user-images.githubusercontent.com/15331990/215649781-be317381-9ff0-4f45-85d4-a30e80514554.png" width=40% height=40%>
-    <br>
     <a href="https://pypi.python.org/pypi/prefect-dbt/" alt="PyPI version">
-        <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-dbt?color=0052FF&labelColor=090422"></a>
-    <a href="https://github.com/prefecthq/prefect-dbt/" alt="Stars">
-        <img src="https://img.shields.io/github/stars/prefecthq/prefect-dbt?color=0052FF&labelColor=090422" /></a>
+        <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-dbt?color=26272B&labelColor=090422"></a>0
     <a href="https://pepy.tech/badge/prefect-dbt/" alt="Downloads">
-        <img src="https://img.shields.io/pypi/dm/prefect-dbt?color=0052FF&labelColor=090422" /></a>
-    <a href="https://github.com/prefecthq/prefect-dbt/pulse" alt="Activity">
-        <img src="https://img.shields.io/github/commit-activity/m/prefecthq/prefect-dbt?color=0052FF&labelColor=090422" /></a>
-    <br>
-    <a href="https://prefect-community.slack.com" alt="Slack">
-        <img src="https://img.shields.io/badge/slack-join_community-red.svg?color=0052FF&labelColor=090422&logo=slack" /></a>
-    <a href="https://discourse.prefect.io/" alt="Discourse">
-        <img src="https://img.shields.io/badge/discourse-browse_forum-red.svg?color=0052FF&labelColor=090422&logo=discourse" /></a>
+        <img src="https://img.shields.io/pypi/dm/prefect-dbt?color=26272B&labelColor=090422" /></a>
 </p>
 
-Visit the full docs [here](https://PrefectHQ.github.io/prefect-dbt) to see additional examples and the API reference.
-
 With prefect-dbt, you can easily trigger and monitor dbt Cloud jobs, execute dbt Core CLI commands, and incorporate other services, like Snowflake, into your dbt runs!
 
 Check out the examples below to get started!
 
 ## Getting Started
 
 Be sure to install [prefect-dbt](#installation) and [save a block](#saving-credentials-to-block) to run the examples below!
@@ -221,36 +205,34 @@
 
     ```bash
     pip install dbt-databricks
     ```
 
     Check out the [desired profile setup page](https://docs.getdbt.com/reference/profiles.yml) on the sidebar for others.
 
-Requires an installation of Python 3.7+.
+Requires an installation of Python 3.8+.
 
 We recommend using a Python virtual environment manager such as pipenv, conda or virtualenv.
 
-These tasks are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://orion-docs.prefect.io/).
+These tasks are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Saving credentials to block
 
-Note, to use the `load` method on Blocks, you must already have a block document [saved through code](https://orion-docs.prefect.io/concepts/blocks/#saving-blocks) or [saved through the UI](https://orion-docs.prefect.io/ui/blocks/).
+Note, to use the `load` method on Blocks, you must already have a block document [saved through code](https://docs.prefect.io/concepts/blocks/#saving-blocks) or [saved through the UI](https://docs.prefect.io/ui/blocks/).
 
 !!! info "Registering blocks"
 
     Register blocks in this module to
-    [view and edit them](https://orion-docs.prefect.io/ui/blocks/)
+    [view and edit them](https://docs.prefect.io/ui/blocks/)
     on Prefect Cloud:
 
     ```bash
     prefect block register -m prefect_dbt
     ```
 
-A list of available blocks in `prefect-dbt` and their setup instructions can be found [here](https://PrefectHQ.github.io/prefect-dbt/blocks_catalog).
-
 #### dbt Cloud
 
 To create a dbt Cloud credentials block:
 
 1. Head over to your [dbt Cloud profile](https://cloud.getdbt.com/settings/profile).
 2. Login to your dbt Cloud account.
 3. Scroll down to "API" or click "API Access" on the sidebar.
@@ -354,19 +336,17 @@
 from prefect_dbt.cloud import DbtCoreOperation
 
 DbtCoreOperation.load("DBT-CORE-OPERATION-BLOCK-NAME-PLACEHOLDER")
 ```
 
 ### Feedback
 
-If you encounter any bugs while using `prefect-dbt`, feel free to open an issue in the [prefect-dbt](https://github.com/PrefectHQ/prefect-dbt) repository.
-
-If you have any questions or issues while using `prefect-dbt`, you can find help in either the [Prefect Discourse forum](https://discourse.prefect.io/) or the [Prefect Slack community](https://prefect.io/slack).
+If you encounter any bugs while using `prefect-dbt`, feel free to open an issue in the [prefect](https://github.com/PrefectHQ/prefect) repository.
 
-Feel free to star or watch [`prefect-dbt`](https://github.com/PrefectHQ/prefect-dbt) for updates too!
+If you have any questions or issues while using `prefect-dbt`, you can find help in the [Prefect Slack community](https://prefect.io/slack).
 
 ### Contributing
 
 If you'd like to help contribute to fix an issue or add a feature to `prefect-dbt`, please [propose changes through a pull request from a fork of the repository](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork).
 
 Here are the steps:
 
@@ -374,13 +354,12 @@
 2. [Clone the forked repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo#cloning-your-forked-repository)
 3. Install the repository and its dependencies:
 ```
 pip install -e ".[dev]"
 ```
 4. Make desired changes
 5. Add tests
-6. Insert an entry to [CHANGELOG.md](https://github.com/PrefectHQ/prefect-dbt/blob/main/CHANGELOG.md)
-7. Install `pre-commit` to perform quality checks prior to commit:
+6. Install `pre-commit` to perform quality checks prior to commit:
 ```
 pre-commit install
 ```
-8. `git commit`, `git push`, and create a pull request
+7. `git commit`, `git push`, and create a pull request
```

### Comparing `prefect-dbt-0.4.1/README.md` & `prefect_dbt-0.4.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,16 @@
-# Coordinate and use dbt in your dataflow with prefect-dbt
+# prefect-dbt
 
 <p align="center">
-    <img src="https://user-images.githubusercontent.com/15331990/215649781-be317381-9ff0-4f45-85d4-a30e80514554.png" width=40% height=40%>
-    <br>
     <a href="https://pypi.python.org/pypi/prefect-dbt/" alt="PyPI version">
-        <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-dbt?color=0052FF&labelColor=090422"></a>
-    <a href="https://github.com/prefecthq/prefect-dbt/" alt="Stars">
-        <img src="https://img.shields.io/github/stars/prefecthq/prefect-dbt?color=0052FF&labelColor=090422" /></a>
+        <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-dbt?color=26272B&labelColor=090422"></a>0
     <a href="https://pepy.tech/badge/prefect-dbt/" alt="Downloads">
-        <img src="https://img.shields.io/pypi/dm/prefect-dbt?color=0052FF&labelColor=090422" /></a>
-    <a href="https://github.com/prefecthq/prefect-dbt/pulse" alt="Activity">
-        <img src="https://img.shields.io/github/commit-activity/m/prefecthq/prefect-dbt?color=0052FF&labelColor=090422" /></a>
-    <br>
-    <a href="https://prefect-community.slack.com" alt="Slack">
-        <img src="https://img.shields.io/badge/slack-join_community-red.svg?color=0052FF&labelColor=090422&logo=slack" /></a>
-    <a href="https://discourse.prefect.io/" alt="Discourse">
-        <img src="https://img.shields.io/badge/discourse-browse_forum-red.svg?color=0052FF&labelColor=090422&logo=discourse" /></a>
+        <img src="https://img.shields.io/pypi/dm/prefect-dbt?color=26272B&labelColor=090422" /></a>
 </p>
 
-Visit the full docs [here](https://PrefectHQ.github.io/prefect-dbt) to see additional examples and the API reference.
-
 With prefect-dbt, you can easily trigger and monitor dbt Cloud jobs, execute dbt Core CLI commands, and incorporate other services, like Snowflake, into your dbt runs!
 
 Check out the examples below to get started!
 
 ## Getting Started
 
 Be sure to install [prefect-dbt](#installation) and [save a block](#saving-credentials-to-block) to run the examples below!
@@ -155,36 +142,34 @@
 
     ```bash
     pip install dbt-databricks
     ```
 
     Check out the [desired profile setup page](https://docs.getdbt.com/reference/profiles.yml) on the sidebar for others.
 
-Requires an installation of Python 3.7+.
+Requires an installation of Python 3.8+.
 
 We recommend using a Python virtual environment manager such as pipenv, conda or virtualenv.
 
-These tasks are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://orion-docs.prefect.io/).
+These tasks are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Saving credentials to block
 
-Note, to use the `load` method on Blocks, you must already have a block document [saved through code](https://orion-docs.prefect.io/concepts/blocks/#saving-blocks) or [saved through the UI](https://orion-docs.prefect.io/ui/blocks/).
+Note, to use the `load` method on Blocks, you must already have a block document [saved through code](https://docs.prefect.io/concepts/blocks/#saving-blocks) or [saved through the UI](https://docs.prefect.io/ui/blocks/).
 
 !!! info "Registering blocks"
 
     Register blocks in this module to
-    [view and edit them](https://orion-docs.prefect.io/ui/blocks/)
+    [view and edit them](https://docs.prefect.io/ui/blocks/)
     on Prefect Cloud:
 
     ```bash
     prefect block register -m prefect_dbt
     ```
 
-A list of available blocks in `prefect-dbt` and their setup instructions can be found [here](https://PrefectHQ.github.io/prefect-dbt/blocks_catalog).
-
 #### dbt Cloud
 
 To create a dbt Cloud credentials block:
 
 1. Head over to your [dbt Cloud profile](https://cloud.getdbt.com/settings/profile).
 2. Login to your dbt Cloud account.
 3. Scroll down to "API" or click "API Access" on the sidebar.
@@ -288,19 +273,17 @@
 from prefect_dbt.cloud import DbtCoreOperation
 
 DbtCoreOperation.load("DBT-CORE-OPERATION-BLOCK-NAME-PLACEHOLDER")
 ```
 
 ### Feedback
 
-If you encounter any bugs while using `prefect-dbt`, feel free to open an issue in the [prefect-dbt](https://github.com/PrefectHQ/prefect-dbt) repository.
-
-If you have any questions or issues while using `prefect-dbt`, you can find help in either the [Prefect Discourse forum](https://discourse.prefect.io/) or the [Prefect Slack community](https://prefect.io/slack).
+If you encounter any bugs while using `prefect-dbt`, feel free to open an issue in the [prefect](https://github.com/PrefectHQ/prefect) repository.
 
-Feel free to star or watch [`prefect-dbt`](https://github.com/PrefectHQ/prefect-dbt) for updates too!
+If you have any questions or issues while using `prefect-dbt`, you can find help in the [Prefect Slack community](https://prefect.io/slack).
 
 ### Contributing
 
 If you'd like to help contribute to fix an issue or add a feature to `prefect-dbt`, please [propose changes through a pull request from a fork of the repository](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork).
 
 Here are the steps:
 
@@ -308,13 +291,12 @@
 2. [Clone the forked repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo#cloning-your-forked-repository)
 3. Install the repository and its dependencies:
 ```
 pip install -e ".[dev]"
 ```
 4. Make desired changes
 5. Add tests
-6. Insert an entry to [CHANGELOG.md](https://github.com/PrefectHQ/prefect-dbt/blob/main/CHANGELOG.md)
-7. Install `pre-commit` to perform quality checks prior to commit:
+6. Install `pre-commit` to perform quality checks prior to commit:
 ```
 pre-commit install
 ```
-8. `git commit`, `git push`, and create a pull request
+7. `git commit`, `git push`, and create a pull request
```

### Comparing `prefect-dbt-0.4.1/prefect_dbt/__init__.py` & `prefect_dbt-0.4.2/prefect_dbt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,8 +20,8 @@
     pass
 
 try:
     from .cli.configs.postgres import PostgresTargetConfigs  # noqa
 except MissingExtrasRequireError:
     pass
 
-__version__ = _version.get_versions()["version"]
+__version__ = _version.__version__
```

### Comparing `prefect-dbt-0.4.1/prefect_dbt/cli/__init__.py` & `prefect_dbt-0.4.2/prefect_dbt/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-dbt-0.4.1/prefect_dbt/cli/commands.py` & `prefect_dbt-0.4.2/prefect_dbt/cli/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Module containing tasks and flows for interacting with dbt CLI"""
 import os
 from pathlib import Path, PosixPath
 from typing import Any, Dict, List, Optional, Union
 
 import yaml
-from prefect import get_run_logger, task
-from prefect.utilities.filesystem import relative_path_to_current_platform
 from prefect_shell.commands import ShellOperation, shell_run_command
 from pydantic import VERSION as PYDANTIC_VERSION
 
+from prefect import get_run_logger, task
+from prefect.utilities.filesystem import relative_path_to_current_platform
+
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import Field, validator
 else:
     from pydantic import Field, validator
 
 from prefect_dbt.cli.credentials import DbtCliProfile
```

### Comparing `prefect-dbt-0.4.1/prefect_dbt/cli/configs/base.py` & `prefect_dbt-0.4.2/prefect_dbt/cli/configs/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Module containing models for base configs"""
 
 import abc
 from pathlib import Path
 from typing import Any, Dict, Optional
 
-from prefect.blocks.core import Block
 from pydantic import VERSION as PYDANTIC_VERSION
 
+from prefect.blocks.core import Block
+
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import BaseModel, Field, SecretField
 else:
     from pydantic import BaseModel, Field, SecretField
 
 
 class DbtConfigs(Block, abc.ABC):
```

### Comparing `prefect-dbt-0.4.1/prefect_dbt/cli/configs/bigquery.py` & `prefect_dbt-0.4.2/prefect_dbt/cli/configs/bigquery.py`

 * *Files identical despite different names*

### Comparing `prefect-dbt-0.4.1/prefect_dbt/cli/configs/postgres.py` & `prefect_dbt-0.4.2/prefect_dbt/cli/configs/postgres.py`

 * *Files identical despite different names*

### Comparing `prefect-dbt-0.4.1/prefect_dbt/cli/configs/snowflake.py` & `prefect_dbt-0.4.2/prefect_dbt/cli/configs/snowflake.py`

 * *Files identical despite different names*

### Comparing `prefect-dbt-0.4.1/prefect_dbt/cli/credentials.py` & `prefect_dbt-0.4.2/prefect_dbt/cli/credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Module containing credentials for interacting with dbt CLI"""
+
 from typing import Any, Dict, Optional, Union
 
-from prefect.blocks.core import Block
 from pydantic import VERSION as PYDANTIC_VERSION
 
+from prefect.blocks.core import Block
+
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import Field
 else:
     from pydantic import Field
 
 from prefect_dbt.cli.configs import GlobalConfigs, TargetConfigs
```

### Comparing `prefect-dbt-0.4.1/prefect_dbt/cloud/clients.py` & `prefect_dbt-0.4.2/prefect_dbt/cloud/clients.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Module containing clients for interacting with the dbt Cloud API"""
 from typing import Any, Dict, List, Optional
 
-import prefect
 from httpx import AsyncClient, Response
 from sgqlc.endpoint.http import HTTPEndpoint
 from typing_extensions import Literal
 
+import prefect
 from prefect_dbt.cloud.models import TriggerJobRunOptions
 
 
 class DbtCloudAdministrativeClient:
     """
     Client for interacting with the dbt cloud Administrative API.
```

### Comparing `prefect-dbt-0.4.1/prefect_dbt/cloud/credentials.py` & `prefect_dbt-0.4.2/prefect_dbt/cloud/credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Module containing credentials for interacting with dbt Cloud"""
 from typing import Union
 
-from prefect.blocks.abstract import CredentialsBlock
 from pydantic import VERSION as PYDANTIC_VERSION
 
+from prefect.blocks.abstract import CredentialsBlock
+
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import Field, SecretStr
 else:
     from pydantic import Field, SecretStr
 
 from typing_extensions import Literal
```

### Comparing `prefect-dbt-0.4.1/prefect_dbt/cloud/exceptions.py` & `prefect_dbt-0.4.2/prefect_dbt/cloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `prefect-dbt-0.4.1/prefect_dbt/cloud/jobs.py` & `prefect_dbt-0.4.2/prefect_dbt/cloud/jobs.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 import asyncio
 import shlex
 import time
 from json import JSONDecodeError
 from typing import Any, Awaitable, Callable, Dict, List, Optional, Union
 
 from httpx import HTTPStatusError
+from pydantic import VERSION as PYDANTIC_VERSION
+
 from prefect import flow, get_run_logger, task
 from prefect.blocks.abstract import JobBlock, JobRun
 from prefect.context import FlowRunContext
 from prefect.utilities.asyncutils import sync_compatible
-from pydantic import VERSION as PYDANTIC_VERSION
 
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import Field
 else:
     from pydantic import Field
 
 from typing_extensions import Literal
@@ -394,22 +395,20 @@
         while retry_filtered_models_attempts > 0:
             logger.info(
                 f"Retrying job run with ID: {run_id} "
                 f"{retry_filtered_models_attempts} more times"
             )
             try:
                 retry_filtered_models_attempts -= 1
-                run_data = await (
-                    retry_dbt_cloud_job_run_subset_and_wait_for_completion(
-                        dbt_cloud_credentials=dbt_cloud_credentials,
-                        run_id=run_id,
-                        trigger_job_run_options=trigger_job_run_options,
-                        max_wait_seconds=max_wait_seconds,
-                        poll_frequency_seconds=poll_frequency_seconds,
-                    )
+                run_data = await retry_dbt_cloud_job_run_subset_and_wait_for_completion(
+                    dbt_cloud_credentials=dbt_cloud_credentials,
+                    run_id=run_id,
+                    trigger_job_run_options=trigger_job_run_options,
+                    max_wait_seconds=max_wait_seconds,
+                    poll_frequency_seconds=poll_frequency_seconds,
                 )
                 return run_data
             except Exception:
                 pass
         else:
             raise DbtCloudJobRunFailed(f"Triggered job run with ID: {run_id} failed.")
     else:
@@ -837,17 +836,15 @@
             select_arg = "--select"
 
         # prevent duplicate --select/-s statements
         if select_arg is not None:
             # dbt --fail-fast run, -s, bad_mod --vars '{"env": "prod"}' to:
             # dbt --fail-fast run -s other_mod bad_mod --vars '{"env": "prod"}'
             command_start, select_arg, command_end = command.partition(select_arg)
-            modified_command = (
-                f"{command_start} {select_arg} {run_nodes} {command_end}"  # noqa
-            )
+            modified_command = f"{command_start} {select_arg} {run_nodes} {command_end}"  # noqa
         else:
             # dbt --fail-fast, build, --vars '{"env": "prod"}' to:
             # dbt --fail-fast build --select bad_model --vars '{"env": "prod"}'
             dbt_global_args, exe_command, exe_args = command.partition(exe_command)
             modified_command = (
                 f"{dbt_global_args} {exe_command} -s {run_nodes} {exe_args}"
             )
```

### Comparing `prefect-dbt-0.4.1/prefect_dbt/cloud/models.py` & `prefect_dbt-0.4.2/prefect_dbt/cloud/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Module containing models used for passing data to dbt Cloud"""
 from typing import List, Optional
 
-from prefect.context import FlowRunContext, TaskRunContext, get_run_context
 from pydantic import VERSION as PYDANTIC_VERSION
 
+from prefect.context import FlowRunContext, TaskRunContext, get_run_context
+
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import BaseModel, Field
 else:
     from pydantic import BaseModel, Field
 
 
 def default_cause_factory():
```

### Comparing `prefect-dbt-0.4.1/prefect_dbt/cloud/runs.py` & `prefect_dbt-0.4.2/prefect_dbt/cloud/runs.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Module containing tasks and flows for interacting with dbt Cloud job runs"""
 import asyncio
 from enum import Enum
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from httpx import HTTPStatusError
-from prefect import flow, get_run_logger, task
 from typing_extensions import Literal
 
+from prefect import flow, get_run_logger, task
 from prefect_dbt.cloud.credentials import DbtCloudCredentials
 from prefect_dbt.cloud.exceptions import (
     DbtCloudGetRunArtifactFailed,
     DbtCloudGetRunFailed,
     DbtCloudJobRunTimedOut,
     DbtCloudListRunArtifactsFailed,
 )
```

### Comparing `prefect-dbt-0.4.1/prefect_dbt/cloud/utils.py` & `prefect_dbt-0.4.2/prefect_dbt/cloud/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Utilities for common interactions with the dbt Cloud API"""
 from json import JSONDecodeError
 from typing import Any, Dict, Optional
 
 from httpx import HTTPStatusError
-from prefect import task
 
+from prefect import task
 from prefect_dbt.cloud.credentials import DbtCloudCredentials
 
 
 def extract_user_message(ex: HTTPStatusError) -> Optional[str]:
     """
     Extracts user message from a error response from the dbt Cloud administrative API.
 
@@ -132,15 +132,14 @@
             )
             return result["data"]
 
         create_job_flow()
         ```
     """  # noqa
     try:
-
         async with dbt_cloud_credentials.get_administrative_client() as client:
             response = await client.call_endpoint(
                 http_method=http_method, path=path, params=params, json=json
             )
     except HTTPStatusError as ex:
         raise DbtCloudAdministrativeApiCallFailed(extract_developer_message(ex)) from ex
     try:
```

### Comparing `prefect-dbt-0.4.1/prefect_dbt.egg-info/PKG-INFO` & `prefect_dbt-0.4.2/prefect_dbt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: prefect-dbt
-Version: 0.4.1
-Summary: Prefect integration for working with dbt
-Home-page: https://github.com/PrefectHQ/prefect-dbt
-Author: Prefect Technologies, Inc.
-Author-email: help@prefect.io
+Version: 0.4.2
+Summary: Prefect integrations for working with dbt
+Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
+Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-dbt
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
-Requires-Dist: prefect>=2.13.5
+Requires-Dist: prefect>=2.16.6
 Requires-Dist: dbt_core>=1.1.1
-Requires-Dist: prefect_shell>=0.1.0
+Requires-Dist: prefect_shell>=0.1.4
 Requires-Dist: sgqlc>=16.0.0
 Provides-Extra: snowflake
 Requires-Dist: prefect-snowflake>=0.2.4; extra == "snowflake"
 Requires-Dist: dbt-snowflake; extra == "snowflake"
 Provides-Extra: bigquery
 Requires-Dist: prefect-gcp[bigquery]>=0.1.8; extra == "bigquery"
 Requires-Dist: dbt-bigquery; extra == "bigquery"
@@ -37,59 +36,44 @@
 Requires-Dist: dbt-bigquery; extra == "all-extras"
 Requires-Dist: dbt-postgres; extra == "all-extras"
 Requires-Dist: dbt-snowflake; extra == "all-extras"
 Requires-Dist: prefect-gcp[bigquery]>=0.1.8; extra == "all-extras"
 Requires-Dist: prefect-snowflake>=0.2.4; extra == "all-extras"
 Requires-Dist: prefect-sqlalchemy>=0.2.1; extra == "all-extras"
 Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: black; extra == "dev"
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: mypy; extra == "dev"
-Requires-Dist: mkdocs; extra == "dev"
-Requires-Dist: mkdocs-material; extra == "dev"
-Requires-Dist: mkdocstrings[python]; extra == "dev"
-Requires-Dist: isort; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: pytest-asyncio; extra == "dev"
-Requires-Dist: mock; python_version < "3.8" and extra == "dev"
-Requires-Dist: mkdocs-gen-files; extra == "dev"
-Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
-Requires-Dist: respx; extra == "dev"
-Requires-Dist: pillow; extra == "dev"
 Requires-Dist: dbt-bigquery; extra == "dev"
 Requires-Dist: dbt-postgres; extra == "dev"
 Requires-Dist: dbt-snowflake; extra == "dev"
+Requires-Dist: interrogate; extra == "dev"
+Requires-Dist: mkdocs-gen-files; extra == "dev"
+Requires-Dist: mkdocs-material; extra == "dev"
+Requires-Dist: mkdocs; extra == "dev"
+Requires-Dist: mkdocstrings[python]; extra == "dev"
+Requires-Dist: mock; python_version < "3.8" and extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: pillow; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: prefect-gcp[bigquery]>=0.1.8; extra == "dev"
 Requires-Dist: prefect-snowflake>=0.2.4; extra == "dev"
 Requires-Dist: prefect-sqlalchemy>=0.2.1; extra == "dev"
+Requires-Dist: pytest-asyncio; extra == "dev"
+Requires-Dist: pytest-xdist; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: respx; extra == "dev"
 
-# Coordinate and use dbt in your dataflow with prefect-dbt
+# prefect-dbt
 
 <p align="center">
-    <img src="https://user-images.githubusercontent.com/15331990/215649781-be317381-9ff0-4f45-85d4-a30e80514554.png" width=40% height=40%>
-    <br>
     <a href="https://pypi.python.org/pypi/prefect-dbt/" alt="PyPI version">
-        <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-dbt?color=0052FF&labelColor=090422"></a>
-    <a href="https://github.com/prefecthq/prefect-dbt/" alt="Stars">
-        <img src="https://img.shields.io/github/stars/prefecthq/prefect-dbt?color=0052FF&labelColor=090422" /></a>
+        <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-dbt?color=26272B&labelColor=090422"></a>0
     <a href="https://pepy.tech/badge/prefect-dbt/" alt="Downloads">
-        <img src="https://img.shields.io/pypi/dm/prefect-dbt?color=0052FF&labelColor=090422" /></a>
-    <a href="https://github.com/prefecthq/prefect-dbt/pulse" alt="Activity">
-        <img src="https://img.shields.io/github/commit-activity/m/prefecthq/prefect-dbt?color=0052FF&labelColor=090422" /></a>
-    <br>
-    <a href="https://prefect-community.slack.com" alt="Slack">
-        <img src="https://img.shields.io/badge/slack-join_community-red.svg?color=0052FF&labelColor=090422&logo=slack" /></a>
-    <a href="https://discourse.prefect.io/" alt="Discourse">
-        <img src="https://img.shields.io/badge/discourse-browse_forum-red.svg?color=0052FF&labelColor=090422&logo=discourse" /></a>
+        <img src="https://img.shields.io/pypi/dm/prefect-dbt?color=26272B&labelColor=090422" /></a>
 </p>
 
-Visit the full docs [here](https://PrefectHQ.github.io/prefect-dbt) to see additional examples and the API reference.
-
 With prefect-dbt, you can easily trigger and monitor dbt Cloud jobs, execute dbt Core CLI commands, and incorporate other services, like Snowflake, into your dbt runs!
 
 Check out the examples below to get started!
 
 ## Getting Started
 
 Be sure to install [prefect-dbt](#installation) and [save a block](#saving-credentials-to-block) to run the examples below!
@@ -221,36 +205,34 @@
 
     ```bash
     pip install dbt-databricks
     ```
 
     Check out the [desired profile setup page](https://docs.getdbt.com/reference/profiles.yml) on the sidebar for others.
 
-Requires an installation of Python 3.7+.
+Requires an installation of Python 3.8+.
 
 We recommend using a Python virtual environment manager such as pipenv, conda or virtualenv.
 
-These tasks are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://orion-docs.prefect.io/).
+These tasks are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Saving credentials to block
 
-Note, to use the `load` method on Blocks, you must already have a block document [saved through code](https://orion-docs.prefect.io/concepts/blocks/#saving-blocks) or [saved through the UI](https://orion-docs.prefect.io/ui/blocks/).
+Note, to use the `load` method on Blocks, you must already have a block document [saved through code](https://docs.prefect.io/concepts/blocks/#saving-blocks) or [saved through the UI](https://docs.prefect.io/ui/blocks/).
 
 !!! info "Registering blocks"
 
     Register blocks in this module to
-    [view and edit them](https://orion-docs.prefect.io/ui/blocks/)
+    [view and edit them](https://docs.prefect.io/ui/blocks/)
     on Prefect Cloud:
 
     ```bash
     prefect block register -m prefect_dbt
     ```
 
-A list of available blocks in `prefect-dbt` and their setup instructions can be found [here](https://PrefectHQ.github.io/prefect-dbt/blocks_catalog).
-
 #### dbt Cloud
 
 To create a dbt Cloud credentials block:
 
 1. Head over to your [dbt Cloud profile](https://cloud.getdbt.com/settings/profile).
 2. Login to your dbt Cloud account.
 3. Scroll down to "API" or click "API Access" on the sidebar.
@@ -354,19 +336,17 @@
 from prefect_dbt.cloud import DbtCoreOperation
 
 DbtCoreOperation.load("DBT-CORE-OPERATION-BLOCK-NAME-PLACEHOLDER")
 ```
 
 ### Feedback
 
-If you encounter any bugs while using `prefect-dbt`, feel free to open an issue in the [prefect-dbt](https://github.com/PrefectHQ/prefect-dbt) repository.
-
-If you have any questions or issues while using `prefect-dbt`, you can find help in either the [Prefect Discourse forum](https://discourse.prefect.io/) or the [Prefect Slack community](https://prefect.io/slack).
+If you encounter any bugs while using `prefect-dbt`, feel free to open an issue in the [prefect](https://github.com/PrefectHQ/prefect) repository.
 
-Feel free to star or watch [`prefect-dbt`](https://github.com/PrefectHQ/prefect-dbt) for updates too!
+If you have any questions or issues while using `prefect-dbt`, you can find help in the [Prefect Slack community](https://prefect.io/slack).
 
 ### Contributing
 
 If you'd like to help contribute to fix an issue or add a feature to `prefect-dbt`, please [propose changes through a pull request from a fork of the repository](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork).
 
 Here are the steps:
 
@@ -374,13 +354,12 @@
 2. [Clone the forked repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo#cloning-your-forked-repository)
 3. Install the repository and its dependencies:
 ```
 pip install -e ".[dev]"
 ```
 4. Make desired changes
 5. Add tests
-6. Insert an entry to [CHANGELOG.md](https://github.com/PrefectHQ/prefect-dbt/blob/main/CHANGELOG.md)
-7. Install `pre-commit` to perform quality checks prior to commit:
+6. Install `pre-commit` to perform quality checks prior to commit:
 ```
 pre-commit install
 ```
-8. `git commit`, `git push`, and create a pull request
+7. `git commit`, `git push`, and create a pull request
```

### Comparing `prefect-dbt-0.4.1/prefect_dbt.egg-info/requires.txt` & `prefect_dbt-0.4.2/prefect_dbt.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-prefect>=2.13.5
+prefect>=2.16.6
 dbt_core>=1.1.1
-prefect_shell>=0.1.0
+prefect_shell>=0.1.4
 sgqlc>=16.0.0
 
 [all_extras]
 dbt-bigquery
 dbt-postgres
 dbt-snowflake
 prefect-gcp[bigquery]>=0.1.8
@@ -12,35 +12,33 @@
 prefect-sqlalchemy>=0.2.1
 
 [bigquery]
 prefect-gcp[bigquery]>=0.1.8
 dbt-bigquery
 
 [dev]
-pytest
-black
-flake8
-mypy
-mkdocs
-mkdocs-material
-mkdocstrings[python]
-isort
-pre-commit
-pytest-asyncio
-mkdocs-gen-files
-interrogate
 coverage
-respx
-pillow
 dbt-bigquery
 dbt-postgres
 dbt-snowflake
+interrogate
+mkdocs-gen-files
+mkdocs-material
+mkdocs
+mkdocstrings[python]
+mypy
+pillow
+pre-commit
 prefect-gcp[bigquery]>=0.1.8
 prefect-snowflake>=0.2.4
 prefect-sqlalchemy>=0.2.1
+pytest-asyncio
+pytest-xdist
+pytest
+respx
 
 [dev:python_version < "3.8"]
 mock
 
 [postgres]
 prefect-sqlalchemy>=0.2.1
 dbt-postgres
```

### Comparing `prefect-dbt-0.4.1/tests/test_block_standards.py` & `prefect_dbt-0.4.2/tests/test_block_standards.py`

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

