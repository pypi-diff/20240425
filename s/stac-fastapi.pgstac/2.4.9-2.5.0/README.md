# Comparing `tmp/stac-fastapi.pgstac-2.4.9.tar.gz` & `tmp/stac_fastapi_pgstac-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac-fastapi.pgstac-2.4.9.tar", last modified: Wed Jun 21 21:25:28 2023, max compression
+gzip compressed data, was "stac_fastapi_pgstac-2.5.0.tar", last modified: Thu Apr 25 15:42:48 2024, max compression
```

## Comparing `stac-fastapi.pgstac-2.4.9.tar` & `stac_fastapi_pgstac-2.5.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:25:28.619498 stac-fastapi.pgstac-2.4.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-06-21 21:25:28.619498 stac-fastapi.pgstac-2.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-21 21:25:28.619498 stac-fastapi.pgstac-2.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:25:28.615498 stac-fastapi.pgstac-2.4.9/stac_fastapi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:25:28.615498 stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14657 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:25:28.615498 stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/extensions/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/extensions/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:25:28.615498 stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/models/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/models/links.py
--rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/transactions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:25:28.615498 stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/types/base_item_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/types/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:25:28.615498 stac-fastapi.pgstac-2.4.9/stac_fastapi.pgstac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-06-21 21:25:28.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi.pgstac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-21 21:25:28.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi.pgstac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 21:25:28.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi.pgstac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-21 21:25:28.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi.pgstac.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 21:25:28.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi.pgstac.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-21 21:25:28.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi.pgstac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-21 21:25:28.000000 stac-fastapi.pgstac-2.4.9/stac_fastapi.pgstac.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:25:28.615498 stac-fastapi.pgstac-2.4.9/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:25:28.615498 stac-fastapi.pgstac-2.4.9/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24577 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/tests/api/test_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:25:28.619498 stac-fastapi.pgstac-2.4.9/tests/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/tests/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/tests/clients/test_postgres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:25:28.619498 stac-fastapi.pgstac-2.4.9/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/tests/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/tests/resources/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/tests/resources/test_conformance.py
--rw-r--r--   0 runner    (1001) docker     (123)    50432 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/tests/resources/test_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-21 21:25:17.000000 stac-fastapi.pgstac-2.4.9/tests/resources/test_mgmt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:42:48.866034 stac_fastapi_pgstac-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-04-25 15:42:48.866034 stac_fastapi_pgstac-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-25 15:42:48.866034 stac_fastapi_pgstac-2.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:42:48.858034 stac_fastapi_pgstac-2.5.0/stac_fastapi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:42:48.862034 stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14888 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:42:48.862034 stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/extensions/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/extensions/query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:42:48.862034 stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/models/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7519 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:42:48.862034 stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/types/base_item_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/types/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6024 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:42:48.866034 stac_fastapi_pgstac-2.5.0/stac_fastapi.pgstac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-04-25 15:42:48.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi.pgstac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-25 15:42:48.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi.pgstac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:42:48.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi.pgstac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-25 15:42:48.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi.pgstac.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:42:48.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi.pgstac.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-25 15:42:48.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi.pgstac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-25 15:42:48.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi.pgstac.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:42:48.858034 stac_fastapi_pgstac-2.5.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:42:48.862034 stac_fastapi_pgstac-2.5.0/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24752 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/tests/api/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:42:48.862034 stac_fastapi_pgstac-2.5.0/tests/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/tests/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14131 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/tests/clients/test_postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:42:48.866034 stac_fastapi_pgstac-2.5.0/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/tests/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7864 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/tests/resources/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/tests/resources/test_conformance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50351 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/tests/resources/test_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/tests/resources/test_mgmt.py
```

### Comparing `stac-fastapi.pgstac-2.4.9/LICENSE` & `stac_fastapi_pgstac-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.9/PKG-INFO` & `stac_fastapi_pgstac-2.5.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: stac-fastapi.pgstac
-Version: 2.4.9
-Summary: An implementation of STAC API based on the FastAPI framework and using the pgstac backend.
-Home-page: https://github.com/stac-utils/stac-fastapi
-Author: David Bitner
-Author-email: david@developmentseed.org
-License: MIT
-Keywords: STAC FastAPI COG
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: docs
-Provides-Extra: server
-Provides-Extra: awslambda
-License-File: LICENSE
-
 # stac-fastapi-pgstac
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/stac-utils/stac-fastapi-pgstac/cicd.yaml?style=for-the-badge)](https://github.com/stac-utils/stac-fastapi-pgstac/actions/workflows/cicd.yaml)
 [![PyPI](https://img.shields.io/pypi/v/stac-fastapi.pgstac?style=for-the-badge)](https://pypi.org/project/stac-fastapi.pgstac)
 [![Documentation](https://img.shields.io/github/actions/workflow/status/stac-utils/stac-fastapi-pgstac/pages.yml?label=Docs&style=for-the-badge)](https://stac-utils.github.io/stac-fastapi-pgstac/)
 [![License](https://img.shields.io/github/license/stac-utils/stac-fastapi-pgstac?style=for-the-badge)](https://github.com/stac-utils/stac-fastapi-pgstac/blob/main/LICENSE)
 
@@ -99,14 +77,14 @@
 ```shell
 mkdocs serve
 ```
 
 ## History
 
 **stac-fastapi-pgstac** was initially added to **stac-fastapi** by [developmentseed](https://github.com/developmentseed).
-In April of 2023, it was removed from the core **stac-fastapi** repository and moved to its current location (<http://github.com/stac-util/stac-fastapi-pgstac>).
+In April of 2023, it was removed from the core **stac-fastapi** repository and moved to its current location (<http://github.com/stac-utils/stac-fastapi-pgstac>).
 
 ## License
 
 [MIT](https://github.com/stac-utils/stac-fastapi-pgstac/blob/main/LICENSE)
 
 <!-- markdownlint-disable-file MD033 -->
```

### Comparing `stac-fastapi.pgstac-2.4.9/setup.py` & `stac_fastapi_pgstac-2.5.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,31 +6,32 @@
     desc = f.read()
 
 install_requires = [
     "attrs",
     "orjson",
     "pydantic[dotenv]>=1.10.8",  # https://github.com/pydantic/pydantic/issues/5821
     "stac_pydantic==2.0.*",
-    "stac-fastapi.types~=2.4.8",
-    "stac-fastapi.api~=2.4.8",
-    "stac-fastapi.extensions~=2.4.8",
+    "stac-fastapi.types~=2.5.5.post1",
+    "stac-fastapi.api~=2.5.5.post1",
+    "stac-fastapi.extensions~=2.5.5.post1",
     "asyncpg",
     "buildpg",
     "brotli_asgi",
     "pygeofilter>=0.2",
     "pypgstac==0.7.*",
 ]
 
 extra_reqs = {
     "dev": [
         "pystac[validation]",
         "pypgstac[psycopg]==0.7.*",
+        "pytest-postgresql",
         "pytest",
         "pytest-cov",
-        "pytest-asyncio>=0.17",
+        "pytest-asyncio>=0.17,<0.23.0",
         "pre-commit",
         "requests",
         "shapely",
         "httpx",
         "twine",
         "wheel",
     ],
@@ -59,11 +60,9 @@
     url="https://github.com/stac-utils/stac-fastapi",
     license="MIT",
     packages=find_namespace_packages(exclude=["tests", "scripts"]),
     zip_safe=False,
     install_requires=install_requires,
     tests_require=extra_reqs["dev"],
     extras_require=extra_reqs,
-    entry_points={
-        "console_scripts": ["stac-fastapi-pgstac=stac_fastapi.pgstac.app:run"]
-    },
+    entry_points={"console_scripts": ["stac-fastapi-pgstac=stac_fastapi.pgstac.app:run"]},
 )
```

### Comparing `stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/app.py` & `stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,26 +42,25 @@
     "context": ContextExtension(),
     "filter": FilterExtension(client=FiltersClient()),
     "bulk_transactions": BulkTransactionExtension(client=BulkTransactionsClient()),
 }
 
 if enabled_extensions := os.getenv("ENABLED_EXTENSIONS"):
     extensions = [
-        extensions_map[extension_name]
-        for extension_name in enabled_extensions.split(",")
+        extensions_map[extension_name] for extension_name in enabled_extensions.split(",")
     ]
 else:
     extensions = list(extensions_map.values())
 
 post_request_model = create_post_request_model(extensions, base_model=PgstacSearch)
 
 api = StacApi(
     settings=settings,
     extensions=extensions,
-    client=CoreCrudClient(post_request_model=post_request_model),
+    client=CoreCrudClient(post_request_model=post_request_model),  # type: ignore
     response_class=ORJSONResponse,
     search_get_request_model=create_get_request_model(extensions),
     search_post_request_model=post_request_model,
 )
 app = api.app
 
 
@@ -86,16 +85,16 @@
             "stac_fastapi.pgstac.app:app",
             host=settings.app_host,
             port=settings.app_port,
             log_level="info",
             reload=settings.reload,
             root_path=os.getenv("UVICORN_ROOT_PATH", ""),
         )
-    except ImportError:
-        raise RuntimeError("Uvicorn must be installed in order to use command")
+    except ImportError as e:
+        raise RuntimeError("Uvicorn must be installed in order to use command") from e
 
 
 if __name__ == "__main__":
     run()
 
 
 def create_handler(app):
```

### Comparing `stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/config.py` & `stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Postgres API configuration."""
 
 from typing import List, Type
 from urllib.parse import quote
 
+from pydantic import BaseModel, Extra
 from stac_fastapi.types.config import ApiSettings
 
 from stac_fastapi.pgstac.types.base_item_cache import (
     BaseItemCache,
     DefaultBaseItemCache,
 )
 
@@ -28,14 +29,21 @@
     "+",
     ",",
     ";",
     "=",
 ]
 
 
+class ServerSettings(BaseModel, extra=Extra.allow):
+    """Server runtime parameters."""
+
+    search_path: str = "pgstac,public"
+    application_name: str = "pgstac"
+
+
 class Settings(ApiSettings):
     """Postgres-specific API settings.
 
     Attributes:
         postgres_user: postgres username.
         postgres_pass: postgres password.
         postgres_host_reader: hostname for the reader connection.
@@ -54,14 +62,16 @@
     postgres_dbname: str
 
     db_min_conn_size: int = 10
     db_max_conn_size: int = 10
     db_max_queries: int = 50000
     db_max_inactive_conn_lifetime: float = 300
 
+    server_settings: ServerSettings = ServerSettings()
+
     use_api_hydrate: bool = False
     base_item_cache: Type[BaseItemCache] = DefaultBaseItemCache
     invalid_id_chars: List[str] = DEFAULT_INVALID_ID_CHARS
 
     testing: bool = False
 
     @property
@@ -74,7 +84,12 @@
         """Create writer psql connection string."""
         return f"postgresql://{self.postgres_user}:{quote(self.postgres_pass)}@{self.postgres_host_writer}:{self.postgres_port}/{self.postgres_dbname}"
 
     @property
     def testing_connection_string(self):
         """Create testing psql connection string."""
         return f"postgresql://{self.postgres_user}:{quote(self.postgres_pass)}@{self.postgres_host_writer}:{self.postgres_port}/pgstactestdb"
+
+    class Config(ApiSettings.Config):
+        """Model config."""
+
+        env_nested_delimiter = "__"
```

### Comparing `stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/core.py` & `stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Item crud client."""
+
 import re
-from datetime import datetime
 from typing import Any, Dict, List, Optional, Union
 from urllib.parse import unquote_plus, urljoin
 
 import attr
 import orjson
 from asyncpg.exceptions import InvalidDatetimeFormatError
 from buildpg import render
@@ -12,27 +12,28 @@
 from pydantic import ValidationError
 from pygeofilter.backends.cql2_json import to_cql2
 from pygeofilter.parsers.cql2_text import parse as parse_cql2_text
 from pypgstac.hydration import hydrate
 from stac_fastapi.types.core import AsyncBaseCoreClient
 from stac_fastapi.types.errors import InvalidQueryParameter, NotFoundError
 from stac_fastapi.types.requests import get_base_url
+from stac_fastapi.types.rfc3339 import DateTimeType
 from stac_fastapi.types.stac import Collection, Collections, Item, ItemCollection
 from stac_pydantic.links import Relations
-from stac_pydantic.shared import MimeTypes
+from stac_pydantic.shared import BBox, MimeTypes
 
 from stac_fastapi.pgstac.config import Settings
 from stac_fastapi.pgstac.models.links import (
     CollectionLinks,
     ItemCollectionLinks,
     ItemLinks,
     PagingLinks,
 )
 from stac_fastapi.pgstac.types.search import PgstacSearch
-from stac_fastapi.pgstac.utils import filter_fields
+from stac_fastapi.pgstac.utils import filter_fields, format_datetime_range
 
 NumType = Union[float, int]
 
 
 @attr.s
 class CoreCrudClient(AsyncBaseCoreClient):
     """Client for core endpoints defined by stac."""
@@ -132,15 +133,15 @@
             item = await conn.fetchval(q, *p)
 
         if item is None:
             raise NotFoundError(f"A base item for {collection_id} does not exist.")
 
         return item
 
-    async def _search_base(
+    async def _search_base(  # noqa: C901
         self,
         search_request: PgstacSearch,
         request: Request,
     ) -> ItemCollection:
         """Cross catalog search (POST).
 
         Called with `POST /search`.
@@ -151,31 +152,35 @@
         Returns:
             ItemCollection containing items which match the search criteria.
         """
         items: Dict[str, Any]
 
         settings: Settings = request.app.state.settings
 
+        if search_request.datetime:
+            search_request.datetime = format_datetime_range(search_request.datetime)
+
         search_request.conf = search_request.conf or {}
         search_request.conf["nohydrate"] = settings.use_api_hydrate
+
         search_request_json = search_request.json(exclude_none=True, by_alias=True)
 
         try:
             async with request.app.state.get_connection(request, "r") as conn:
                 q, p = render(
                     """
                     SELECT * FROM search(:req::text::jsonb);
                     """,
                     req=search_request_json,
                 )
                 items = await conn.fetchval(q, *p)
-        except InvalidDatetimeFormatError:
+        except InvalidDatetimeFormatError as e:
             raise InvalidQueryParameter(
                 f"Datetime parameter {search_request.datetime} is invalid."
-            )
+            ) from e
 
         next: Optional[str] = items.pop("next", None)
         prev: Optional[str] = items.pop("prev", None)
         collection = ItemCollection(**items)
 
         exclude = search_request.fields.exclude
         if exclude and len(exclude) == 0:
@@ -199,16 +204,16 @@
 
             if (
                 search_request.fields.exclude is None
                 or "links" not in search_request.fields.exclude
                 and all([collection_id, item_id])
             ):
                 feature["links"] = await ItemLinks(
-                    collection_id=collection_id,
-                    item_id=item_id,
+                    collection_id=collection_id,  # type: ignore
+                    item_id=item_id,  # type: ignore
                     request=request,
                 ).get_links(extra_links=feature.get("links"))
 
         cleaned_features: List[Item] = []
 
         if settings.use_api_hydrate:
 
@@ -244,18 +249,18 @@
         ).get_links()
         return collection
 
     async def item_collection(
         self,
         collection_id: str,
         request: Request,
-        bbox: Optional[List[NumType]] = None,
-        datetime: Optional[Union[str, datetime]] = None,
+        bbox: Optional[BBox] = None,
+        datetime: Optional[DateTimeType] = None,
         limit: Optional[int] = None,
-        token: str = None,
+        token: Optional[str] = None,
         **kwargs,
     ) -> ItemCollection:
         """Get all items from a specific collection.
 
         Called with `GET /collections/{collection_id}/items`
 
         Args:
@@ -332,21 +337,21 @@
 
         Returns:
             ItemCollection containing items which match the search criteria.
         """
         item_collection = await self._search_base(search_request, request=request)
         return ItemCollection(**item_collection)
 
-    async def get_search(
+    async def get_search(  # noqa: C901
         self,
         request: Request,
         collections: Optional[List[str]] = None,
         ids: Optional[List[str]] = None,
-        bbox: Optional[List[NumType]] = None,
-        datetime: Optional[Union[str, datetime]] = None,
+        bbox: Optional[BBox] = None,
+        datetime: Optional[DateTimeType] = None,
         limit: Optional[int] = None,
         query: Optional[str] = None,
         token: Optional[str] = None,
         fields: Optional[List[str]] = None,
         sortby: Optional[str] = None,
         filter: Optional[str] = None,
         filter_lang: Optional[str] = None,
@@ -424,9 +429,10 @@
 
         # Do the request
         try:
             search_request = self.post_request_model(**clean)
         except ValidationError as e:
             raise HTTPException(
                 status_code=400, detail=f"Invalid parameters provided {e}"
-            )
+            ) from e
+
         return await self.post_search(search_request, request=request)
```

### Comparing `stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/db.py` & `stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/db.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 """Database connection handling."""
 
 import json
 from contextlib import asynccontextmanager, contextmanager
-from typing import AsyncIterator, Callable, Dict, Generator, Literal, Union
+from typing import (
+    AsyncIterator,
+    Callable,
+    Dict,
+    Generator,
+    List,
+    Literal,
+    Optional,
+    Union,
+)
 
 import attr
 import orjson
 from asyncpg import Connection, exceptions
 from buildpg import V, asyncpg, render
 from fastapi import FastAPI, Request
 from stac_fastapi.types.errors import (
@@ -32,22 +41,25 @@
         schema="pg_catalog",
     )
 
 
 ConnectionGetter = Callable[[Request, Literal["r", "w"]], AsyncIterator[Connection]]
 
 
-async def connect_to_db(app: FastAPI, get_conn: ConnectionGetter = None) -> None:
+async def connect_to_db(
+    app: FastAPI, get_conn: Optional[ConnectionGetter] = None
+) -> None:
     """Create connection pools & connection retriever on application."""
     settings = app.state.settings
     if app.state.settings.testing:
         readpool = writepool = settings.testing_connection_string
     else:
         readpool = settings.reader_connection_string
         writepool = settings.writer_connection_string
+
     db = DB()
     app.state.readpool = await db.create_pool(readpool, settings)
     app.state.writepool = await db.create_pool(writepool, settings)
     app.state.get_connection = get_conn if get_conn else get_connection
 
 
 async def close_db_connection(app: FastAPI) -> None:
@@ -58,23 +70,21 @@
 
 @asynccontextmanager
 async def get_connection(
     request: Request,
     readwrite: Literal["r", "w"] = "r",
 ) -> AsyncIterator[Connection]:
     """Retrieve connection from database conection pool."""
-    pool = (
-        request.app.state.writepool if readwrite == "w" else request.app.state.readpool
-    )
+    pool = request.app.state.writepool if readwrite == "w" else request.app.state.readpool
     with translate_pgstac_errors():
         async with pool.acquire() as conn:
             yield conn
 
 
-async def dbfunc(conn: Connection, func: str, arg: Union[str, Dict]):
+async def dbfunc(conn: Connection, func: str, arg: Union[str, Dict, List]):
     """Wrap PLPGSQL Functions.
 
     Keyword arguments:
     pool -- the asyncpg pool to use to connect to the database
     func -- the name of the PostgreSQL function to call
     arg -- the argument to the PostgreSQL function as either a string
     or a dict that will be converted into jsonb
@@ -128,13 +138,10 @@
         pool = await asyncpg.create_pool(
             connection_string,
             min_size=settings.db_min_conn_size,
             max_size=settings.db_max_conn_size,
             max_queries=settings.db_max_queries,
             max_inactive_connection_lifetime=settings.db_max_inactive_conn_lifetime,
             init=con_init,
-            server_settings={
-                "search_path": "pgstac,public",
-                "application_name": "pgstac",
-            },
+            server_settings=settings.server_settings.dict(),
         )
         return pool
```

### Comparing `stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/extensions/filter.py` & `stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/extensions/filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Get Queryables."""
+
 from typing import Any, Optional
 
 from buildpg import render
 from fastapi import Request
 from fastapi.responses import JSONResponse
 from stac_fastapi.types.core import AsyncBaseFiltersClient
 from stac_fastapi.types.errors import NotFoundError
```

### Comparing `stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/extensions/query.py` & `stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/extensions/query.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/models/links.py` & `stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/models/links.py`

 * *Files 22% similar despite different names*

```diff
@@ -55,21 +55,27 @@
 
     def resolve(self, url):
         """Resolve url to the current request url."""
         return urljoin(str(self.base_url), str(url))
 
     def link_self(self) -> Dict:
         """Return the self link."""
-        return dict(rel=Relations.self.value, type=MimeTypes.json.value, href=self.url)
+        return {
+            "rel": Relations.self.value,
+            "type": MimeTypes.json.value,
+            "href": self.url,
+        }
 
     def link_root(self) -> Dict:
         """Return the catalog root."""
-        return dict(
-            rel=Relations.root.value, type=MimeTypes.json.value, href=self.base_url
-        )
+        return {
+            "rel": Relations.root.value,
+            "type": MimeTypes.json.value,
+            "href": self.base_url,
+        }
 
     def create_links(self) -> List[Dict[str, Any]]:
         """Return all inferred links."""
         links = []
         for name in dir(self):
             if name.startswith("link_") and callable(getattr(self, name)):
                 link = getattr(self, name)()
@@ -120,21 +126,22 @@
 
     def link_next(self) -> Optional[Dict[str, Any]]:
         """Create link for next page."""
         if self.next is not None:
             method = self.request.method
             if method == "GET":
                 href = merge_params(self.url, {"token": f"next:{self.next}"})
-                link = dict(
-                    rel=Relations.next.value,
-                    type=MimeTypes.geojson.value,
-                    method=method,
-                    href=href,
-                )
+                link = {
+                    "rel": Relations.next.value,
+                    "type": MimeTypes.geojson.value,
+                    "method": method,
+                    "href": href,
+                }
                 return link
+
             if method == "POST":
                 return {
                     "rel": Relations.next,
                     "type": MimeTypes.geojson,
                     "method": method,
                     "href": f"{self.request.url}",
                     "body": {**self.request.postbody, "token": f"next:{self.next}"},
@@ -144,20 +151,21 @@
 
     def link_prev(self) -> Optional[Dict[str, Any]]:
         """Create link for previous page."""
         if self.prev is not None:
             method = self.request.method
             if method == "GET":
                 href = merge_params(self.url, {"token": f"prev:{self.prev}"})
-                return dict(
-                    rel=Relations.previous.value,
-                    type=MimeTypes.geojson.value,
-                    method=method,
-                    href=href,
-                )
+                return {
+                    "rel": Relations.previous.value,
+                    "type": MimeTypes.geojson.value,
+                    "method": method,
+                    "href": href,
+                }
+
             if method == "POST":
                 return {
                     "rel": Relations.previous,
                     "type": MimeTypes.geojson,
                     "method": method,
                     "href": f"{self.request.url}",
                     "body": {**self.request.postbody, "token": f"prev:{self.prev}"},
@@ -169,57 +177,57 @@
 class CollectionLinksBase(BaseLinks):
     """Create inferred links specific to collections."""
 
     collection_id: str = attr.ib()
 
     def collection_link(self, rel: str = Relations.collection.value) -> Dict:
         """Create a link to a collection."""
-        return dict(
-            rel=rel,
-            type=MimeTypes.json.value,
-            href=self.resolve(f"collections/{self.collection_id}"),
-        )
+        return {
+            "rel": rel,
+            "type": MimeTypes.json.value,
+            "href": self.resolve(f"collections/{self.collection_id}"),
+        }
 
 
 @attr.s
 class CollectionLinks(CollectionLinksBase):
     """Create inferred links specific to collections."""
 
     def link_self(self) -> Dict:
         """Return the self link."""
         return self.collection_link(rel=Relations.self.value)
 
     def link_parent(self) -> Dict:
         """Create the `parent` link."""
-        return dict(
-            rel=Relations.parent.value,
-            type=MimeTypes.json.value,
-            href=self.base_url,
-        )
+        return {
+            "rel": Relations.parent.value,
+            "type": MimeTypes.json.value,
+            "href": self.base_url,
+        }
 
     def link_items(self) -> Dict:
         """Create the `item` link."""
-        return dict(
-            rel="items",
-            type=MimeTypes.geojson.value,
-            href=self.resolve(f"collections/{self.collection_id}/items"),
-        )
+        return {
+            "rel": "items",
+            "type": MimeTypes.geojson.value,
+            "href": self.resolve(f"collections/{self.collection_id}/items"),
+        }
 
 
 @attr.s
 class ItemCollectionLinks(CollectionLinksBase):
     """Create inferred links specific to collections."""
 
     def link_self(self) -> Dict:
         """Return the self link."""
-        return dict(
-            rel=Relations.self.value,
-            type=MimeTypes.geojson.value,
-            href=self.resolve(f"collections/{self.collection_id}/items"),
-        )
+        return {
+            "rel": Relations.self.value,
+            "type": MimeTypes.geojson.value,
+            "href": self.resolve(f"collections/{self.collection_id}/items"),
+        }
 
     def link_parent(self) -> Dict:
         """Create the `parent` link."""
         return self.collection_link(rel=Relations.parent.value)
 
     def link_collection(self) -> Dict:
         """Create the `collection` link."""
@@ -230,19 +238,21 @@
 class ItemLinks(CollectionLinksBase):
     """Create inferred links specific to items."""
 
     item_id: str = attr.ib()
 
     def link_self(self) -> Dict:
         """Create the self link."""
-        return dict(
-            rel=Relations.self.value,
-            type=MimeTypes.geojson.value,
-            href=self.resolve(f"collections/{self.collection_id}/items/{self.item_id}"),
-        )
+        return {
+            "rel": Relations.self.value,
+            "type": MimeTypes.geojson.value,
+            "href": self.resolve(
+                f"collections/{self.collection_id}/items/{self.item_id}"
+            ),
+        }
 
     def link_parent(self) -> Dict:
         """Create the `parent` link."""
         return self.collection_link(rel=Relations.parent.value)
 
     def link_collection(self) -> Dict:
         """Create the `collection` link."""
```

### Comparing `stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/transactions.py` & `stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/transactions.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import Optional, Union
 
 import attr
 from buildpg import render
 from fastapi import HTTPException, Request
 from stac_fastapi.extensions.third_party.bulk_transactions import (
     AsyncBaseBulkTransactionsClient,
+    BulkTransactionMethod,
     Items,
 )
 from stac_fastapi.types import stac as stac_types
 from stac_fastapi.types.core import AsyncBaseTransactionsClient
 from starlette.responses import JSONResponse, Response
 
 from stac_fastapi.pgstac.config import Settings
@@ -23,15 +24,15 @@
 logger.setLevel(logging.INFO)
 
 
 @attr.s
 class TransactionsClient(AsyncBaseTransactionsClient):
     """Transactions extension specific CRUD operations."""
 
-    def _validate_id(self, id: str, settings: Settings) -> bool:
+    def _validate_id(self, id: str, settings: Settings):
         invalid_chars = settings.invalid_id_chars
         id_regex = "[" + "".join(re.escape(char) for char in invalid_chars) + "]"
 
         if bool(re.search(id_regex, id)):
             raise HTTPException(
                 status_code=400,
                 detail=f"ID ({id}) cannot contain the following characters: {' '.join(invalid_chars)}",
@@ -71,15 +72,15 @@
         item: Union[stac_types.Item, stac_types.ItemCollection],
         request: Request,
         **kwargs,
     ) -> Optional[Union[stac_types.Item, Response]]:
         """Create item."""
         if item["type"] == "FeatureCollection":
             valid_items = []
-            for item in item["features"]:
+            for item in item["features"]:  # noqa: B020
                 self._validate_item(request, item, collection_id)
                 item["collection"] = collection_id
                 valid_items.append(item)
 
             async with request.app.state.get_connection(request, "w") as conn:
                 await dbfunc(conn, "create_items", valid_items)
 
@@ -176,13 +177,19 @@
 
 @attr.s
 class BulkTransactionsClient(AsyncBaseBulkTransactionsClient):
     """Postgres bulk transactions."""
 
     async def bulk_item_insert(self, items: Items, request: Request, **kwargs) -> str:
         """Bulk item insertion using pgstac."""
-        items = list(items.items.values())
+        items_to_insert = list(items.items.values())
+
         async with request.app.state.get_connection(request, "w") as conn:
-            await dbfunc(conn, "create_items", items)
+            if items.method == BulkTransactionMethod.INSERT:
+                method_verb = "added"
+                await dbfunc(conn, "create_items", items_to_insert)
+            elif items.method == BulkTransactionMethod.UPSERT:
+                method_verb = "upserted"
+                await dbfunc(conn, "upsert_items", items_to_insert)
 
-        return_msg = f"Successfully added {len(items)} items."
+        return_msg = f"Successfully {method_verb} {len(items_to_insert)} items."
         return return_msg
```

### Comparing `stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/types/base_item_cache.py` & `stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/types/base_item_cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """base_item_cache classes for pgstac fastapi."""
+
 import abc
 from typing import Any, Callable, Coroutine, Dict
 
 from starlette.requests import Request
 
 
 class BaseItemCache(abc.ABC):
@@ -39,15 +40,15 @@
 
     def __init__(
         self,
         fetch_base_item: Callable[[str], Coroutine[Any, Any, Dict[str, Any]]],
         request: Request,
     ):
         """Initialize the base item cache."""
-        self._base_items = {}
+        self._base_items: Dict = {}
         super().__init__(fetch_base_item, request)
 
     async def get(self, collection_id: str):
         """Return the base item for the collection and cache by collection id."""
         if collection_id not in self._base_items:
             self._base_items[collection_id] = await self._fetch_base_item(
                 collection_id,
```

### Comparing `stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/types/search.py` & `stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/types/search.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.9/stac_fastapi/pgstac/utils.py` & `stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """stac-fastapi utility methods."""
+
+from datetime import datetime
 from typing import Any, Dict, Optional, Set, Union
 
+from stac_fastapi.types.rfc3339 import DateTimeType
 from stac_fastapi.types.stac import Item
 
 
-def filter_fields(
+def filter_fields(  # noqa: C901
     item: Union[Item, Dict[str, Any]],
     include: Optional[Set[str]] = None,
     exclude: Optional[Set[str]] = None,
 ) -> Item:
     """Preserve and remove fields as indicated by the fields extension include/exclude sets.
 
     Returns a shallow copy of the Item with the fields filtered.
@@ -32,15 +35,15 @@
             key_root = key_path_parts[0]
             if key_root in source:
                 if isinstance(source[key_root], dict) and len(key_path_parts) > 1:
                     # The root of this key path on the item is a dict, and the
                     # key path indicates a sub-key to be included. Walk the dict
                     # from the root key and get the full nested value to include.
                     value = include_fields(
-                        source[key_root], fields=set([".".join(key_path_parts[1:])])
+                        source[key_root], fields={".".join(key_path_parts[1:])}
                     )
 
                     if isinstance(clean_item.get(key_root), dict):
                         # A previously specified key and sub-keys may have been included
                         # already, so do a deep merge update if the root key already exists.
                         dict_deep_update(clean_item[key_root], value)
                     else:
@@ -64,17 +67,15 @@
     def exclude_fields(source: Dict[str, Any], fields: Optional[Set[str]]) -> None:
         for key_path in fields or []:
             key_path_part = key_path.split(".")
             key_root = key_path_part[0]
             if key_root in source:
                 if isinstance(source[key_root], dict) and len(key_path_part) > 1:
                     # Walk the nested path of this key to remove the leaf-key
-                    exclude_fields(
-                        source[key_root], fields=set([".".join(key_path_part[1:])])
-                    )
+                    exclude_fields(source[key_root], fields={".".join(key_path_part[1:])})
                     # If, after removing the leaf-key, the root is now an empty
                     # dict, remove it entirely
                     if not source[key_root]:
                         del source[key_root]
                 else:
                     # The key's value is not a dict, or there is no sub-key to remove. The
                     # entire key can be removed from the source.
@@ -87,15 +88,15 @@
     item = dict(item)
 
     clean_item = include_fields(item, include)
 
     # If, after including all the specified fields, there are no included properties,
     # return just id and collection.
     if not clean_item:
-        return Item({"id": item.get(id), "collection": item.get("collection")})
+        return Item({"id": item["id"], "collection": item["collection"]})
 
     exclude_fields(clean_item, exclude)
 
     return Item(**clean_item)
 
 
 def dict_deep_update(merge_to: Dict[str, Any], merge_from: Dict[str, Any]) -> None:
@@ -109,7 +110,38 @@
             k in merge_to
             and isinstance(merge_to[k], dict)
             and isinstance(merge_from[k], dict)
         ):
             dict_deep_update(merge_to[k], merge_from[k])
         else:
             merge_to[k] = v
+
+
+def format_datetime_range(dt_range: DateTimeType) -> Union[str, Any]:
+    """
+    Convert a datetime object or a tuple of datetime objects to a formatted string for datetime ranges.
+
+    Args:
+        dt_range (DateTimeType): The date interval,
+            which might be a single datetime or a tuple with one or two datetimes.
+
+    Returns:
+        str: A formatted string like 'YYYY-MM-DDTHH:MM:SSZ/..', 'YYYY-MM-DDTHH:MM:SSZ', or the original string input.
+    """
+    # Handle a single datetime object
+    if isinstance(dt_range, datetime):
+        return dt_range.isoformat().replace("+00:00", "Z")
+
+    # Handle a tuple containing datetime objects or None
+    if isinstance(dt_range, tuple):
+        start, end = dt_range
+
+        # Convert start datetime to string if not None, otherwise use ".."
+        start_str = start.isoformat().replace("+00:00", "Z") if start else ".."
+
+        # Convert end datetime to string if not None, otherwise use ".."
+        end_str = end.isoformat().replace("+00:00", "Z") if end else ".."
+
+        return f"{start_str}/{end_str}"
+
+    # Return input as-is if it's not any expected type (fallback)
+    return dt_range
```

### Comparing `stac-fastapi.pgstac-2.4.9/stac_fastapi.pgstac.egg-info/PKG-INFO` & `stac_fastapi_pgstac-2.5.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,57 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.pgstac
-Version: 2.4.9
+Version: 2.5.0
 Summary: An implementation of STAC API based on the FastAPI framework and using the pgstac backend.
 Home-page: https://github.com/stac-utils/stac-fastapi
 Author: David Bitner
 Author-email: david@developmentseed.org
 License: MIT
 Keywords: STAC FastAPI COG
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: attrs
+Requires-Dist: orjson
+Requires-Dist: pydantic[dotenv]>=1.10.8
+Requires-Dist: stac_pydantic==2.0.*
+Requires-Dist: stac-fastapi.types~=2.5.5.post1
+Requires-Dist: stac-fastapi.api~=2.5.5.post1
+Requires-Dist: stac-fastapi.extensions~=2.5.5.post1
+Requires-Dist: asyncpg
+Requires-Dist: buildpg
+Requires-Dist: brotli_asgi
+Requires-Dist: pygeofilter>=0.2
+Requires-Dist: pypgstac==0.7.*
 Provides-Extra: dev
+Requires-Dist: pystac[validation]; extra == "dev"
+Requires-Dist: pypgstac[psycopg]==0.7.*; extra == "dev"
+Requires-Dist: pytest-postgresql; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: pytest-asyncio<0.23.0,>=0.17; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: requests; extra == "dev"
+Requires-Dist: shapely; extra == "dev"
+Requires-Dist: httpx; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+Requires-Dist: wheel; extra == "dev"
 Provides-Extra: docs
+Requires-Dist: mkdocs; extra == "docs"
+Requires-Dist: mkdocs-material; extra == "docs"
+Requires-Dist: pdocs; extra == "docs"
 Provides-Extra: server
+Requires-Dist: uvicorn[standard]==0.19.0; extra == "server"
 Provides-Extra: awslambda
-License-File: LICENSE
+Requires-Dist: mangum; extra == "awslambda"
 
 # stac-fastapi-pgstac
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/stac-utils/stac-fastapi-pgstac/cicd.yaml?style=for-the-badge)](https://github.com/stac-utils/stac-fastapi-pgstac/actions/workflows/cicd.yaml)
 [![PyPI](https://img.shields.io/pypi/v/stac-fastapi.pgstac?style=for-the-badge)](https://pypi.org/project/stac-fastapi.pgstac)
 [![Documentation](https://img.shields.io/github/actions/workflow/status/stac-utils/stac-fastapi-pgstac/pages.yml?label=Docs&style=for-the-badge)](https://stac-utils.github.io/stac-fastapi-pgstac/)
 [![License](https://img.shields.io/github/license/stac-utils/stac-fastapi-pgstac?style=for-the-badge)](https://github.com/stac-utils/stac-fastapi-pgstac/blob/main/LICENSE)
@@ -99,14 +128,14 @@
 ```shell
 mkdocs serve
 ```
 
 ## History
 
 **stac-fastapi-pgstac** was initially added to **stac-fastapi** by [developmentseed](https://github.com/developmentseed).
-In April of 2023, it was removed from the core **stac-fastapi** repository and moved to its current location (<http://github.com/stac-util/stac-fastapi-pgstac>).
+In April of 2023, it was removed from the core **stac-fastapi** repository and moved to its current location (<http://github.com/stac-utils/stac-fastapi-pgstac>).
 
 ## License
 
 [MIT](https://github.com/stac-utils/stac-fastapi-pgstac/blob/main/LICENSE)
 
 <!-- markdownlint-disable-file MD033 -->
```

### Comparing `stac-fastapi.pgstac-2.4.9/stac_fastapi.pgstac.egg-info/SOURCES.txt` & `stac_fastapi_pgstac-2.5.0/stac_fastapi.pgstac.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.9/tests/api/test_api.py` & `stac_fastapi_pgstac-2.5.0/tests/api/test_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 ]
 
 STAC_TRANSACTION_ROUTES = [
     "DELETE /collections/{collection_id}",
     "DELETE /collections/{collection_id}/items/{item_id}",
     "POST /collections",
     "POST /collections/{collection_id}/items",
-    "PUT /collections",
+    "PUT /collections/{collection_id}",
     "PUT /collections/{collection_id}/items/{item_id}",
 ]
 
 GLOBAL_BBOX = [-180.0, -90.0, 180.0, 90.0]
 GLOBAL_GEOMETRY = {
     "type": "Polygon",
     "coordinates": (
@@ -83,47 +83,41 @@
 
 
 async def test_get_features_self_link(app_client, load_test_collection):
     # https://github.com/stac-utils/stac-fastapi/issues/483
     resp = await app_client.get(f"collections/{load_test_collection.id}/items")
     assert resp.status_code == 200
     resp_json = resp.json()
-    self_link = next(
-        (link for link in resp_json["links"] if link["rel"] == "self"), None
-    )
+    self_link = next((link for link in resp_json["links"] if link["rel"] == "self"), None)
     assert self_link is not None
     assert self_link["href"].endswith("/items")
 
 
-async def test_get_feature_content_type(
-    app_client, load_test_collection, load_test_item
-):
+async def test_get_feature_content_type(app_client, load_test_collection, load_test_item):
     resp = await app_client.get(
         f"collections/{load_test_collection.id}/items/{load_test_item.id}"
     )
     assert resp.headers["content-type"] == "application/geo+json"
 
 
 async def test_api_headers(app_client):
     resp = await app_client.get("/api")
-    assert (
-        resp.headers["content-type"] == "application/vnd.oai.openapi+json;version=3.0"
-    )
+    assert resp.headers["content-type"] == "application/vnd.oai.openapi+json;version=3.0"
     assert resp.status_code == 200
 
 
 async def test_core_router(api_client, app):
     core_routes = set()
     for core_route in STAC_CORE_ROUTES:
         method, path = core_route.split(" ")
         core_routes.add("{} {}".format(method, app.state.router_prefix + path))
 
-    api_routes = set(
-        [f"{list(route.methods)[0]} {route.path}" for route in api_client.app.routes]
-    )
+    api_routes = {
+        f"{list(route.methods)[0]} {route.path}" for route in api_client.app.routes
+    }
     assert not core_routes - api_routes
 
 
 async def test_landing_page_stac_extensions(app_client):
     resp = await app_client.get("/")
     assert resp.status_code == 200
     resp_json = resp.json()
@@ -132,17 +126,17 @@
 
 async def test_transactions_router(api_client, app):
     transaction_routes = set()
     for transaction_route in STAC_TRANSACTION_ROUTES:
         method, path = transaction_route.split(" ")
         transaction_routes.add("{} {}".format(method, app.state.router_prefix + path))
 
-    api_routes = set(
-        [f"{list(route.methods)[0]} {route.path}" for route in api_client.app.routes]
-    )
+    api_routes = {
+        f"{list(route.methods)[0]} {route.path}" for route in api_client.app.routes
+    }
     assert not transaction_routes - api_routes
 
 
 async def test_app_transaction_extension(
     app_client, load_test_data, load_test_collection
 ):
     coll = load_test_collection
@@ -226,17 +220,15 @@
     params = {"query": {"proj:epsg": {"gt": item["properties"]["proj:epsg"]}}}
     resp = await app_client.post("/search", json=params)
     assert resp.status_code == 200
     resp_json = resp.json()
     assert len(resp_json["features"]) == 0
 
 
-async def test_app_query_extension_gte(
-    load_test_data, app_client, load_test_collection
-):
+async def test_app_query_extension_gte(load_test_data, app_client, load_test_collection):
     coll = load_test_collection
     item = load_test_data("test_item.json")
     resp = await app_client.post(f"/collections/{coll.id}/items", json=item)
     assert resp.status_code == 200
 
     params = {"query": {"proj:epsg": {"gte": item["properties"]["proj:epsg"]}}}
     resp = await app_client.post("/search", json=params)
@@ -329,28 +321,26 @@
 
     assert resp_json.get("type") == "FeatureCollection"
     # stac_version and stac_extensions were removed in v1.0.0-beta.3
     assert resp_json.get("stac_version") is None
     assert resp_json.get("stac_extensions") is None
 
 
-async def test_search_point_intersects(
-    load_test_data, app_client, load_test_collection
-):
+async def test_search_point_intersects(load_test_data, app_client, load_test_collection):
     coll = load_test_collection
     item = load_test_data("test_item.json")
     resp = await app_client.post(f"/collections/{coll.id}/items", json=item)
     assert resp.status_code == 200
 
-    new_coordinates = list()
+    new_coordinates = []
     for coordinate in item["geometry"]["coordinates"][0]:
         new_coordinates.append([coordinate[0] * -1, coordinate[1] * -1])
     item["id"] = "test-item-other-hemispheres"
     item["geometry"]["coordinates"] = [new_coordinates]
-    item["bbox"] = list(value * -1 for value in item["bbox"])
+    item["bbox"] = [value * -1 for value in item["bbox"]]
     resp = await app_client.post(f"/collections/{coll.id}/items", json=item)
     assert resp.status_code == 200
 
     point = [150.04, -33.14]
     intersects = {"type": "Point", "coordinates": point}
 
     params = {
@@ -387,17 +377,15 @@
     resp = await app_client.post("/search", json=params)
     assert resp.status_code == 200
     resp_json = resp.json()
     assert len(resp_json["features"]) == 1
 
 
 @pytest.mark.asyncio
-async def test_landing_forwarded_header(
-    load_test_data, app_client, load_test_collection
-):
+async def test_landing_forwarded_header(load_test_data, app_client, load_test_collection):
     coll = load_test_collection
     item = load_test_data("test_item.json")
     await app_client.post(f"/collections/{coll.id}/items", json=item)
     response = (
         await app_client.get(
             "/",
             headers={
@@ -408,17 +396,15 @@
         )
     ).json()
     for link in response["links"]:
         assert link["href"].startswith("https://test:1234/")
 
 
 @pytest.mark.asyncio
-async def test_search_forwarded_header(
-    load_test_data, app_client, load_test_collection
-):
+async def test_search_forwarded_header(load_test_data, app_client, load_test_collection):
     coll = load_test_collection
     item = load_test_data("test_item.json")
     await app_client.post(f"/collections/{coll.id}/items", json=item)
     resp = await app_client.post(
         "/search",
         json={
             "collections": [item["collection"]],
@@ -608,15 +594,15 @@
         response = await app_client.post(
             f"/collections/{collection_id}/items",
             json=item.to_dict(include_self_link=False, transform_hrefs=False),
         )
         assert response.status_code == 200
 
     async def search(query: Dict[str, Any]) -> List[Item]:
-        items: List[Item] = list()
+        items: List[Item] = []
         while True:
             response = await app_client.post("/search", json=query)
             json = response.json()
             assert response.status_code == 200, json
             items.extend((Item.from_dict(d) for d in json["features"]))
             next_link = next(
                 (link for link in json["links"] if link["rel"] == "next"), None
@@ -632,28 +618,28 @@
         "limit": 5,
     }
     items = await search(query)
     assert len(items) == 10, items
 
 
 @pytest.mark.asyncio
-async def test_wrapped_function(load_test_data) -> None:
+async def test_wrapped_function(load_test_data, database) -> None:
     # Ensure wrappers, e.g. Planetary Computer's rate limiting, work.
     # https://github.com/gadomski/planetary-computer-apis/blob/2719ccf6ead3e06de0784c39a2918d4d1811368b/pccommon/pccommon/redis.py#L205-L238
 
     T = TypeVar("T")
 
     def wrap() -> (
         Callable[
             [Callable[..., Coroutine[Any, Any, T]]],
             Callable[..., Coroutine[Any, Any, T]],
         ]
     ):
         def decorator(
-            fn: Callable[..., Coroutine[Any, Any, T]]
+            fn: Callable[..., Coroutine[Any, Any, T]],
         ) -> Callable[..., Coroutine[Any, Any, T]]:
             async def _wrapper(*args: Any, **kwargs: Any) -> T:
                 request: Optional[Request] = kwargs.get("request")
                 if request:
                     pass  # This is where rate limiting would be applied
                 else:
                     raise ValueError(f"Missing request in {fn.__name__}")
@@ -664,19 +650,26 @@
         return decorator
 
     class Client(CoreCrudClient):
         @wrap()
         async def get_collection(
             self, collection_id: str, request: Request, **kwargs
         ) -> stac_types.Item:
-            return await super().get_collection(
-                collection_id, request=request, **kwargs
-            )
+            return await super().get_collection(collection_id, request=request, **kwargs)
+
+    settings = Settings(
+        postgres_user=database.user,
+        postgres_pass=database.password,
+        postgres_host_reader=database.host,
+        postgres_host_writer=database.host,
+        postgres_port=database.port,
+        postgres_dbname=database.dbname,
+        testing=True,
+    )
 
-    settings = Settings(testing=True)
     extensions = [
         TransactionExtension(client=TransactionsClient(), settings=settings),
         FieldsExtension(),
     ]
     post_request_model = create_post_request_model(extensions, base_model=PgstacSearch)
     api = StacApi(
         client=Client(post_request_model=post_request_model),
```

### Comparing `stac-fastapi.pgstac-2.4.9/tests/clients/test_postgres.py` & `stac_fastapi_pgstac-2.5.0/tests/clients/test_postgres.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     assert post_coll.dict(exclude={"links"}) == get_coll.dict(exclude={"links"})
 
 
 async def test_update_collection(app_client, load_test_collection):
     in_coll = load_test_collection
     in_coll.keywords.append("newkeyword")
 
-    resp = await app_client.put("/collections", json=in_coll.dict())
+    resp = await app_client.put(f"/collections/{in_coll.id}", json=in_coll.dict())
     assert resp.status_code == 200
 
     resp = await app_client.get(f"/collections/{in_coll.id}")
     assert resp.status_code == 200
 
     get_coll = Collection.parse_obj(resp.json())
     assert in_coll.dict(exclude={"links"}) == get_coll.dict(exclude={"links"})
@@ -322,14 +322,84 @@
     assert resp.text == '"Successfully added 2 items."'
 
     for item_id in items.keys():
         resp = await app_client.get(f"/collections/{coll.id}/items/{item_id}")
         assert resp.status_code == 200
 
 
+async def test_create_bulk_items_already_exist_insert(
+    app_client, load_test_data: Callable, load_test_collection
+):
+    coll = load_test_collection
+    item = load_test_data("test_item.json")
+
+    items = {}
+    for _ in range(2):
+        _item = deepcopy(item)
+        _item["id"] = str(uuid.uuid4())
+        items[_item["id"]] = _item
+
+    payload = {"items": items, "method": "insert"}
+
+    resp = await app_client.post(
+        f"/collections/{coll.id}/bulk_items",
+        json=payload,
+    )
+    assert resp.status_code == 200
+    assert resp.text == '"Successfully added 2 items."'
+
+    for item_id in items.keys():
+        resp = await app_client.get(f"/collections/{coll.id}/items/{item_id}")
+        assert resp.status_code == 200
+
+    # Try creating the same items again.
+    # This should fail with the default insert behavior.
+    resp = await app_client.post(
+        f"/collections/{coll.id}/bulk_items",
+        json=payload,
+    )
+    assert resp.status_code == 409
+
+
+async def test_create_bulk_items_already_exist_upsert(
+    app_client, load_test_data: Callable, load_test_collection
+):
+    coll = load_test_collection
+    item = load_test_data("test_item.json")
+
+    items = {}
+    for _ in range(2):
+        _item = deepcopy(item)
+        _item["id"] = str(uuid.uuid4())
+        items[_item["id"]] = _item
+
+    payload = {"items": items, "method": "insert"}
+
+    resp = await app_client.post(
+        f"/collections/{coll.id}/bulk_items",
+        json=payload,
+    )
+    assert resp.status_code == 200
+    assert resp.text == '"Successfully added 2 items."'
+
+    for item_id in items.keys():
+        resp = await app_client.get(f"/collections/{coll.id}/items/{item_id}")
+        assert resp.status_code == 200
+
+    # Try creating the same items again, but using upsert.
+    # This should succeed.
+    payload["method"] = "upsert"
+    resp = await app_client.post(
+        f"/collections/{coll.id}/bulk_items",
+        json=payload,
+    )
+    assert resp.status_code == 200
+    assert resp.text == '"Successfully upserted 2 items."'
+
+
 # TODO since right now puts implement upsert
 # test_create_collection_already_exists
 # test create_item_already_exists
 
 
 # def test_get_collection_items(
 #     postgres_core: CoreCrudClient,
```

### Comparing `stac-fastapi.pgstac-2.4.9/tests/resources/test_collection.py` & `stac_fastapi_pgstac-2.5.0/tests/resources/test_collection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Callable
+from typing import Callable, Optional
 
 import pystac
 import pytest
 from stac_pydantic import Collection
 
 
 async def test_create_collection(app_client, load_test_data: Callable):
@@ -16,27 +16,25 @@
     post_coll = Collection.parse_obj(resp.json())
     assert in_coll.dict(exclude={"links"}) == post_coll.dict(exclude={"links"})
     resp = await app_client.get(f"/collections/{post_coll.id}")
     assert resp.status_code == 200
     get_coll = Collection.parse_obj(resp.json())
     assert post_coll.dict(exclude={"links"}) == get_coll.dict(exclude={"links"})
 
-    post_self_link = next(
-        (link for link in post_coll.links if link.rel == "self"), None
-    )
+    post_self_link = next((link for link in post_coll.links if link.rel == "self"), None)
     get_self_link = next((link for link in get_coll.links if link.rel == "self"), None)
     assert post_self_link is not None and get_self_link is not None
     assert post_self_link.href == get_self_link.href
 
 
 async def test_update_collection(app_client, load_test_data, load_test_collection):
     in_coll = load_test_collection
     in_coll.keywords.append("newkeyword")
 
-    resp = await app_client.put("/collections", json=in_coll.dict())
+    resp = await app_client.put(f"/collections/{in_coll.id}", json=in_coll.dict())
     assert resp.status_code == 200
     put_coll = Collection.parse_obj(resp.json())
 
     resp = await app_client.get(f"/collections/{in_coll.id}")
     assert resp.status_code == 200
 
     get_coll = Collection.parse_obj(resp.json())
@@ -84,15 +82,15 @@
     assert resp.status_code == 405
 
 
 async def test_update_new_collection(app_client, load_test_collection):
     in_coll = load_test_collection
     in_coll.id = "test-updatenew"
 
-    resp = await app_client.put("/collections", json=in_coll.dict())
+    resp = await app_client.put(f"/collections/{in_coll.id}", json=in_coll.dict())
     assert resp.status_code == 404
 
 
 async def test_nocollections(
     app_client,
 ):
     resp = await app_client.get("/collections")
@@ -149,15 +147,16 @@
     resp = await app_client.get("/collections")
     assert resp.status_code == 200
     resp_json = resp.json()
     collections = resp_json["collections"]
     # Find collection in list by ID
     single_coll = next(coll for coll in collections if coll["id"] == in_json["id"])
     is_coll_from_list_valid = False
-    single_coll_mocked_link = dict()
+
+    single_coll_mocked_link: Optional[pystac.Collection] = None
     if single_coll is not None:
         single_coll_mocked_link = pystac.Collection.from_dict(
             single_coll, root=mock_root, preserve_dict=False
         )
         is_coll_from_list_valid = single_coll_mocked_link.validate()
 
     assert is_coll_from_list_valid
```

### Comparing `stac-fastapi.pgstac-2.4.9/tests/resources/test_conformance.py` & `stac_fastapi_pgstac-2.5.0/tests/resources/test_conformance.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.9/tests/resources/test_item.py` & `stac_fastapi_pgstac-2.5.0/tests/resources/test_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     assert post_coll.dict(exclude={"links"}) == get_coll.dict(exclude={"links"})
 
 
 async def test_update_collection(app_client, load_test_data, load_test_collection):
     in_coll = load_test_collection
     in_coll.keywords.append("newkeyword")
 
-    resp = await app_client.put("/collections", json=in_coll.dict())
+    resp = await app_client.put(f"/collections/{in_coll.id}", json=in_coll.dict())
     assert resp.status_code == 200
 
     resp = await app_client.get(f"/collections/{in_coll.id}")
     assert resp.status_code == 200
 
     get_coll = Collection.parse_obj(resp.json())
     assert in_coll.dict(exclude={"links"}) == get_coll.dict(exclude={"links"})
@@ -78,17 +78,15 @@
 
     resp = await app_client.get(f"/collections/{coll.id}/items/{post_item.id}")
 
     assert resp.status_code == 200
     get_item = Item.parse_obj(resp.json())
     assert in_item.dict(exclude={"links"}) == get_item.dict(exclude={"links"})
 
-    post_self_link = next(
-        (link for link in post_item.links if link.rel == "self"), None
-    )
+    post_self_link = next((link for link in post_item.links if link.rel == "self"), None)
     get_self_link = next((link for link in get_item.links if link.rel == "self"), None)
     assert post_self_link is not None and get_self_link is not None
     assert post_self_link.href == get_self_link.href
 
 
 async def test_create_item_mismatched_collection_id(
     app_client, load_test_data: Callable, load_test_collection
@@ -367,15 +365,15 @@
         assert resp.status_code == 200
 
     params = {"collections": [test_item["collection"]], "ids": ids}
     resp = await app_client.post("/search", json=params)
     assert resp.status_code == 200
     resp_json = resp.json()
     assert len(resp_json["features"]) == len(ids)
-    assert set([feat["id"] for feat in resp_json["features"]]) == set(ids)
+    assert {feat["id"] for feat in resp_json["features"]} == set(ids)
 
 
 async def test_item_search_by_id_no_results_post(
     app_client, load_test_data, load_test_collection
 ):
     """Test POST search by item id (core) when there are no results"""
     test_item = load_test_data("test_item.json")
@@ -529,15 +527,15 @@
         assert resp.status_code == 200
 
     params = {"collections": test_item["collection"], "ids": ",".join(ids)}
     resp = await app_client.get("/search", params=params)
     assert resp.status_code == 200
     resp_json = resp.json()
     assert len(resp_json["features"]) == len(ids)
-    assert set([feat["id"] for feat in resp_json["features"]]) == set(ids)
+    assert {feat["id"] for feat in resp_json["features"]} == set(ids)
 
 
 async def test_item_search_bbox_get(app_client, load_test_data, load_test_collection):
     """Test GET search with spatial query (core)"""
     test_item = load_test_data("test_item.json")
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=test_item
@@ -754,18 +752,18 @@
     assert len(resp.json()["features"]) == 1
     assert (
         resp_json["features"][0]["properties"]["proj:epsg"]
         == test_item["properties"]["proj:epsg"]
     )
 
 
-async def test_item_search_get_filter_extension_cql(
+async def test_item_search_post_filter_extension_cql(
     app_client, load_test_data, load_test_collection
 ):
-    """Test GET search with JSONB query (cql json filter extension)"""
+    """Test POST search with JSONB query (cql json filter extension)"""
     test_item = load_test_data("test_item.json")
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=test_item
     )
     assert resp.status_code == 200
 
     second_test_item = load_test_data("test_item2.json")
@@ -804,18 +802,18 @@
     assert len(resp.json()["features"]) == 1
     assert (
         resp_json["features"][0]["properties"]["proj:epsg"]
         == test_item["properties"]["proj:epsg"]
     )
 
 
-async def test_item_search_get_filter_extension_cql2(
+async def test_item_search_post_filter_extension_cql2(
     app_client, load_test_data, load_test_collection
 ):
-    """Test GET search with JSONB query (cql2 json filter extension)"""
+    """Test POST search with JSONB query (cql2 json filter extension)"""
     test_item = load_test_data("test_item.json")
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=test_item
     )
     assert resp.status_code == 200
 
     second_test_item = load_test_data("test_item2.json")
@@ -858,18 +856,18 @@
     assert len(resp.json()["features"]) == 1
     assert (
         resp_json["features"][0]["properties"]["proj:epsg"]
         == test_item["properties"]["proj:epsg"]
     )
 
 
-async def test_item_search_get_filter_extension_cql2_with_query_fails(
+async def test_item_search_post_filter_extension_cql2_with_query_fails(
     app_client, load_test_data, load_test_collection
 ):
-    """Test GET search with JSONB query (cql2 json filter extension)"""
+    """Test POST search with JSONB query (cql2 json filter extension)"""
     test_item = load_test_data("test_item.json")
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=test_item
     )
     assert resp.status_code == 200
 
     second_test_item = load_test_data("test_item2.json")
@@ -911,15 +909,15 @@
     app_client, load_test_data, load_test_collection
 ):
     """Test item collection pagination links (paging extension)"""
     test_item = load_test_data("test_item.json")
     ids = []
 
     # Ingest 5 items
-    for idx in range(5):
+    for _ in range(5):
         uid = str(uuid.uuid4())
         test_item["id"] = uid
         resp = await app_client.post(
             f"/collections/{test_item['collection']}/items", json=test_item
         )
         assert resp.status_code == 200
         ids.append(uid)
@@ -930,37 +928,36 @@
     )
     idx = 0
     item_ids = []
     while True:
         idx += 1
         page_data = page.json()
         item_ids.append(page_data["features"][0]["id"])
-        nextlink = [
-            link["href"] for link in page_data["links"] if link["rel"] == "next"
-        ]
+        nextlink = [link["href"] for link in page_data["links"] if link["rel"] == "next"]
         if len(nextlink) < 1:
             break
+
         page = await app_client.get(nextlink.pop())
-        if idx >= 10:
-            assert False
+
+        assert idx < 10
 
     # Our limit is 1 so we expect len(ids) number of requests before we run out of pages
     assert idx == len(ids)
 
     # Confirm we have paginated through all items
     assert not set(item_ids) - set(ids)
 
 
 async def test_pagination_post(app_client, load_test_data, load_test_collection):
     """Test POST pagination (paging extension)"""
     test_item = load_test_data("test_item.json")
     ids = []
 
     # Ingest 5 items
-    for idx in range(5):
+    for _ in range(5):
         uid = str(uuid.uuid4())
         test_item["id"] = uid
         resp = await app_client.post(
             f"/collections/{test_item['collection']}/items", json=test_item
         )
         assert resp.status_code == 200
         ids.append(uid)
@@ -977,20 +974,20 @@
     while True:
         idx += 1
         page_data = page.json()
         item_ids.append(page_data["features"][0]["id"])
         next_link = list(filter(lambda link: link["rel"] == "next", page_data["links"]))
         if not next_link:
             break
+
         # Merge request bodies
         request_body.update(next_link[0]["body"])
         page = await app_client.post("/search", json=request_body)
 
-        if idx > 10:
-            assert False
+        assert idx < 10
 
     # Our limit is 1 so we expect len(ids) number of requests before we run out of pages
     assert idx == len(ids)
 
     # Confirm we have paginated through all items
     assert not set(item_ids) - set(ids)
 
@@ -999,15 +996,15 @@
     app_client, load_test_data, load_test_collection
 ):
     """Test that pagination tokens are idempotent (paging extension)"""
     test_item = load_test_data("test_item.json")
     ids = []
 
     # Ingest 5 items
-    for idx in range(5):
+    for _ in range(5):
         uid = str(uuid.uuid4())
         test_item["id"] = uid
         resp = await app_client.post(
             f"/collections/{test_item['collection']}/items", json=test_item
         )
         assert resp.status_code == 200
         ids.append(uid)
@@ -1129,30 +1126,30 @@
     body = {"fields": {"include": ["properties.width", "properties.height"]}}
 
     resp = await app_client.post("/search", json=body)
     assert resp.status_code == 200
     resp_json = resp.json()
 
     resp_prop_keys = resp_json["features"][0]["properties"].keys()
-    assert set(resp_prop_keys) == set(["width", "height"])
+    assert set(resp_prop_keys) == {"width", "height"}
 
 
 async def test_field_extension_include_multiple_deeply_nested_subkeys(
     app_client, load_test_item, load_test_collection
 ):
     """Test that multiple deeply nested subkeys of an object field are included"""
     body = {"fields": {"include": ["assets.ANG.type", "assets.ANG.href"]}}
 
     resp = await app_client.post("/search", json=body)
     assert resp.status_code == 200
     resp_json = resp.json()
 
     resp_assets = resp_json["features"][0]["assets"]
-    assert set(resp_assets.keys()) == set(["ANG"])
-    assert set(resp_assets["ANG"].keys()) == set(["type", "href"])
+    assert set(resp_assets.keys()) == {"ANG"}
+    assert set(resp_assets["ANG"].keys()) == {"type", "href"}
 
 
 async def test_field_extension_exclude_multiple_deeply_nested_subkeys(
     app_client, load_test_item, load_test_collection
 ):
     """Test that multiple deeply nested subkeys of an object field are excluded"""
     body = {"fields": {"exclude": ["assets.ANG.type", "assets.ANG.href"]}}
@@ -1281,18 +1278,18 @@
     assert response_item.status_code == 200
     item = response_item.json()
     extra_link = [link for link in item["links"] if link["rel"] == "preview"]
     assert extra_link
     assert extra_link[0]["href"] == expected_href
 
 
-async def test_item_search_get_filter_extension_cql_explicitlang(
+async def test_item_search_post_filter_extension_cql_explicitlang(
     app_client, load_test_data, load_test_collection
 ):
-    """Test GET search with JSONB query (cql json filter extension)"""
+    """Test POST search with JSONB query (cql json filter extension)"""
     test_item = load_test_data("test_item.json")
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=test_item
     )
     assert resp.status_code == 200
 
     # EPSG is a JSONB key
@@ -1327,18 +1324,18 @@
     assert len(resp.json()["features"]) == 1
     assert (
         resp_json["features"][0]["properties"]["proj:epsg"]
         == test_item["properties"]["proj:epsg"]
     )
 
 
-async def test_item_search_get_filter_extension_cql2_2(
+async def test_item_search_post_filter_extension_cql2_2(
     app_client, load_test_data, load_test_collection
 ):
-    """Test GET search with JSONB query (cql json filter extension)"""
+    """Test POST search with JSONB query (cql json filter extension)"""
     test_item = load_test_data("test_item.json")
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=test_item
     )
     assert resp.status_code == 200
 
     # EPSG is a JSONB key
@@ -1417,15 +1414,15 @@
         resp = await app_client.post("/search", json=body)
         assert resp.status_code == 400
 
         resp = await app_client.get("/search?datetime={}".format(dt))
         assert resp.status_code == 400
 
 
-async def test_filter_cql2text(app_client, load_test_data, load_test_collection):
+async def test_get_filter_cql2text(app_client, load_test_data, load_test_collection):
     """Test GET search with cql2-text"""
     test_item = load_test_data("test_item.json")
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=test_item
     )
     assert resp.status_code == 200
```

