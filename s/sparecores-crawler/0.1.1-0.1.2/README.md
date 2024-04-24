# Comparing `tmp/sparecores_crawler-0.1.1.tar.gz` & `tmp/sparecores_crawler-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparecores_crawler-0.1.1.tar", last modified: Fri Apr 12 17:16:58 2024, max compression
+gzip compressed data, was "sparecores_crawler-0.1.2.tar", last modified: Wed Apr 24 22:22:20 2024, max compression
```

## Comparing `sparecores_crawler-0.1.1.tar` & `sparecores_crawler-0.1.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-04-12 17:16:58.198246 sparecores_crawler-0.1.1/
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)    16726 2023-12-08 22:12:52.000000 sparecores_crawler-0.1.1/LICENSE
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)       53 2024-04-12 16:09:18.000000 sparecores_crawler-0.1.1/MANIFEST.in
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     7384 2024-04-12 17:16:58.198246 sparecores_crawler-0.1.1/PKG-INFO
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     5326 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.1/README.md
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     3515 2024-04-12 15:19:56.000000 sparecores_crawler-0.1.1/pyproject.toml
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)       38 2024-04-12 17:16:58.198246 sparecores_crawler-0.1.1/setup.cfg
-drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-04-12 17:16:58.184913 sparecores_crawler-0.1.1/src/
-drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-04-12 17:16:58.191579 sparecores_crawler-0.1.1/src/sc_crawler/
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)        0 2024-02-14 13:12:38.000000 sparecores_crawler-0.1.1/src/sc_crawler/__init__.py
-drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-04-12 17:16:58.191579 sparecores_crawler-0.1.1/src/sc_crawler/alembic/
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     2977 2024-04-12 16:51:35.000000 sparecores_crawler-0.1.1/src/sc_crawler/alembic/env.py
-drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-04-12 17:16:58.191579 sparecores_crawler-0.1.1/src/sc_crawler/alembic/versions/
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     5929 2024-04-12 16:51:35.000000 sparecores_crawler-0.1.1/src/sc_crawler/alembic/versions/4691089690c2_v0_1_1.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)    68592 2024-04-12 16:51:35.000000 sparecores_crawler-0.1.1/src/sc_crawler/alembic/versions/98894dffd37c_v0_1_0.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     3618 2024-04-12 15:45:00.000000 sparecores_crawler-0.1.1/src/sc_crawler/alembic.ini
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1185 2024-04-12 16:10:05.000000 sparecores_crawler-0.1.1/src/sc_crawler/alembic_helpers.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)    22486 2024-04-12 16:49:26.000000 sparecores_crawler-0.1.1/src/sc_crawler/cli.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     6780 2024-04-10 22:14:16.000000 sparecores_crawler-0.1.1/src/sc_crawler/insert.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     8517 2024-04-04 14:01:05.000000 sparecores_crawler-0.1.1/src/sc_crawler/logger.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     3503 2024-04-12 15:19:56.000000 sparecores_crawler-0.1.1/src/sc_crawler/lookup.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     2201 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.1/src/sc_crawler/str_utils.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)    19543 2024-04-12 15:19:56.000000 sparecores_crawler-0.1.1/src/sc_crawler/table_bases.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     4705 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.1/src/sc_crawler/table_fields.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)    17021 2024-04-12 15:16:24.000000 sparecores_crawler-0.1.1/src/sc_crawler/tables.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     2730 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.1/src/sc_crawler/tables_scd.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     4836 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.1/src/sc_crawler/utils.py
-drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-04-12 17:16:58.191579 sparecores_crawler-0.1.1/src/sc_crawler/vendors/
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)      116 2024-04-12 15:19:56.000000 sparecores_crawler-0.1.1/src/sc_crawler/vendors/__init__.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)    38933 2024-04-12 15:19:56.000000 sparecores_crawler-0.1.1/src/sc_crawler/vendors/aws.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)      520 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.1/src/sc_crawler/vendors/gcp.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     9834 2024-04-12 15:19:56.000000 sparecores_crawler-0.1.1/src/sc_crawler/vendors/hcloud.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1298 2024-04-12 15:19:56.000000 sparecores_crawler-0.1.1/src/sc_crawler/vendors/vendors.py
-drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-04-12 17:16:58.194913 sparecores_crawler-0.1.1/src/sparecores_crawler.egg-info/
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     7384 2024-04-12 17:16:58.000000 sparecores_crawler-0.1.1/src/sparecores_crawler.egg-info/PKG-INFO
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1042 2024-04-12 17:16:58.000000 sparecores_crawler-0.1.1/src/sparecores_crawler.egg-info/SOURCES.txt
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)        1 2024-04-12 17:16:58.000000 sparecores_crawler-0.1.1/src/sparecores_crawler.egg-info/dependency_links.txt
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)       50 2024-04-12 17:16:58.000000 sparecores_crawler-0.1.1/src/sparecores_crawler.egg-info/entry_points.txt
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)      495 2024-04-12 17:16:58.000000 sparecores_crawler-0.1.1/src/sparecores_crawler.egg-info/requires.txt
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)       11 2024-04-12 17:16:58.000000 sparecores_crawler-0.1.1/src/sparecores_crawler.egg-info/top_level.txt
-drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-04-12 17:16:58.194913 sparecores_crawler-0.1.1/tests/
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1391 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.1/tests/test_schemas.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1316 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.1/tests/test_str_utils.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1216 2024-03-25 14:01:48.000000 sparecores_crawler-0.1.1/tests/test_utils.py
+drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-04-24 22:22:20.498400 sparecores_crawler-0.1.2/
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)    16726 2023-12-08 22:12:52.000000 sparecores_crawler-0.1.2/LICENSE
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)       53 2024-04-12 16:09:18.000000 sparecores_crawler-0.1.2/MANIFEST.in
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     7725 2024-04-24 22:22:20.498400 sparecores_crawler-0.1.2/PKG-INFO
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     5326 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.2/README.md
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     3737 2024-04-24 22:21:44.000000 sparecores_crawler-0.1.2/pyproject.toml
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)       38 2024-04-24 22:22:20.498400 sparecores_crawler-0.1.2/setup.cfg
+drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-04-24 22:22:20.485067 sparecores_crawler-0.1.2/src/
+drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-04-24 22:22:20.491734 sparecores_crawler-0.1.2/src/sc_crawler/
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)        0 2024-02-14 13:12:38.000000 sparecores_crawler-0.1.2/src/sc_crawler/__init__.py
+drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-04-24 22:22:20.491734 sparecores_crawler-0.1.2/src/sc_crawler/alembic/
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     2977 2024-04-24 21:32:55.000000 sparecores_crawler-0.1.2/src/sc_crawler/alembic/env.py
+drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-04-24 22:22:20.491734 sparecores_crawler-0.1.2/src/sc_crawler/alembic/versions/
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     5929 2024-04-24 21:32:55.000000 sparecores_crawler-0.1.2/src/sc_crawler/alembic/versions/4691089690c2_v0_1_1.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)    68592 2024-04-24 21:32:55.000000 sparecores_crawler-0.1.2/src/sc_crawler/alembic/versions/98894dffd37c_v0_1_0.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     3618 2024-04-12 15:45:00.000000 sparecores_crawler-0.1.2/src/sc_crawler/alembic.ini
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1185 2024-04-12 16:10:05.000000 sparecores_crawler-0.1.2/src/sc_crawler/alembic_helpers.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)    22486 2024-04-12 16:49:26.000000 sparecores_crawler-0.1.2/src/sc_crawler/cli.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     6780 2024-04-10 22:14:16.000000 sparecores_crawler-0.1.2/src/sc_crawler/insert.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     8517 2024-04-04 14:01:05.000000 sparecores_crawler-0.1.2/src/sc_crawler/logger.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     3624 2024-04-24 22:21:44.000000 sparecores_crawler-0.1.2/src/sc_crawler/lookup.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     2201 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.2/src/sc_crawler/str_utils.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)    19543 2024-04-23 20:55:29.000000 sparecores_crawler-0.1.2/src/sc_crawler/table_bases.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     4705 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.2/src/sc_crawler/table_fields.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)    17017 2024-04-24 22:21:44.000000 sparecores_crawler-0.1.2/src/sc_crawler/tables.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     2730 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.2/src/sc_crawler/tables_scd.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     5156 2024-04-24 22:21:44.000000 sparecores_crawler-0.1.2/src/sc_crawler/utils.py
+drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-04-24 22:22:20.491734 sparecores_crawler-0.1.2/src/sc_crawler/vendors/
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)      116 2024-04-12 15:19:56.000000 sparecores_crawler-0.1.2/src/sc_crawler/vendors/__init__.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)    38992 2024-04-24 22:21:44.000000 sparecores_crawler-0.1.2/src/sc_crawler/vendors/aws.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)    31391 2024-04-24 22:21:44.000000 sparecores_crawler-0.1.2/src/sc_crawler/vendors/gcp.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)    10143 2024-04-24 22:21:44.000000 sparecores_crawler-0.1.2/src/sc_crawler/vendors/hcloud.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1520 2024-04-24 22:21:44.000000 sparecores_crawler-0.1.2/src/sc_crawler/vendors/vendors.py
+drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-04-24 22:22:20.495067 sparecores_crawler-0.1.2/src/sparecores_crawler.egg-info/
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     7725 2024-04-24 22:22:20.000000 sparecores_crawler-0.1.2/src/sparecores_crawler.egg-info/PKG-INFO
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1042 2024-04-24 22:22:20.000000 sparecores_crawler-0.1.2/src/sparecores_crawler.egg-info/SOURCES.txt
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)        1 2024-04-24 22:22:20.000000 sparecores_crawler-0.1.2/src/sparecores_crawler.egg-info/dependency_links.txt
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)       50 2024-04-24 22:22:20.000000 sparecores_crawler-0.1.2/src/sparecores_crawler.egg-info/entry_points.txt
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)      581 2024-04-24 22:22:20.000000 sparecores_crawler-0.1.2/src/sparecores_crawler.egg-info/requires.txt
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)       11 2024-04-24 22:22:20.000000 sparecores_crawler-0.1.2/src/sparecores_crawler.egg-info/top_level.txt
+drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-04-24 22:22:20.495067 sparecores_crawler-0.1.2/tests/
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1391 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.2/tests/test_schemas.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1316 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.2/tests/test_str_utils.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1216 2024-03-25 14:01:48.000000 sparecores_crawler-0.1.2/tests/test_utils.py
```

### Comparing `sparecores_crawler-0.1.1/LICENSE` & `sparecores_crawler-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.1/PKG-INFO` & `sparecores_crawler-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: sparecores-crawler
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pull and standardize data on cloud compute resources.
 Author: Attila Nagy, Gergely Daroczi, Balazs Hodobay
 Maintainer-email: Spare Cores team <pkg@sparecores.com>
 Project-URL: repository, https://github.com/SpareCores/sc-crawler
 Project-URL: issues, https://github.com/SpareCores/sc-crawler/issues
 Project-URL: documentation, https://sparecores.github.io/sc-crawler/
+Project-URL: homepage, https://sparecores.com
+Keywords: cloud,compute,etl,sqlite,spot-instances,cost-optimization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -36,17 +38,22 @@
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: sparecores-crawler[mkdocs]; extra == "testing"
 Provides-Extra: aws
 Requires-Dist: boto3; extra == "aws"
 Provides-Extra: hcloud
 Requires-Dist: hcloud; extra == "hcloud"
+Provides-Extra: gcp
+Requires-Dist: google-cloud; extra == "gcp"
+Requires-Dist: google-cloud-compute; extra == "gcp"
+Requires-Dist: google-cloud-billing; extra == "gcp"
 Provides-Extra: vendors
 Requires-Dist: sparecores-crawler[aws]; extra == "vendors"
 Requires-Dist: sparecores-crawler[hcloud]; extra == "vendors"
+Requires-Dist: sparecores-crawler[gcp]; extra == "vendors"
 Provides-Extra: all
 Requires-Dist: sparecores-crawler[testing]; extra == "all"
 Requires-Dist: sparecores-crawler[vendors]; extra == "all"
 
 ## Spare Cores Crawler
 
 [![Build](https://img.shields.io/github/actions/workflow/status/SpareCores/sc-crawler/tests.yaml)](https://github.com/SpareCores/sc-crawler/actions/workflows/tests.yaml)
```

### Comparing `sparecores_crawler-0.1.1/README.md` & `sparecores_crawler-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.1/pyproject.toml` & `sparecores_crawler-0.1.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sparecores-crawler"
-version = "0.1.1"
+version = "0.1.2"
 requires-python = ">= 3.7"
 dependencies = [
   "alembic",
   "cachier",
   "pydantic",
   "pydantic_extra_types",
   "rich",
@@ -21,39 +21,42 @@
   { name="Balazs Hodobay" },
 ]
 maintainers = [
   { name="Spare Cores team", email="pkg@sparecores.com" }
 ]
 description = "Pull and standardize data on cloud compute resources."
 readme = "README.md"
+keywords = ["cloud", "compute", "etl", "sqlite", "spot-instances", "cost-optimization"]
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
   "Operating System :: OS Independent",
   "Development Status :: 3 - Alpha",
 ]
 
 [project.urls]
 repository = "https://github.com/SpareCores/sc-crawler"
 issues = "https://github.com/SpareCores/sc-crawler/issues"
 documentation = "https://sparecores.github.io/sc-crawler/"
+homepage = "https://sparecores.com"
 
 [project.optional-dependencies]
 mkdocs = [
   "markdown==3.5.2", # https://github.com/mkdocstrings/mkdocstrings/issues/662
   "mkdocs",
   "mkdocs-material[imaging]==9.5.13", "mkdocs-material-extensions",
   "mkdocs-autorefs", "mkdocs-gen-files", "mkdocs-literate-nav", "mkdocs-section-index",
   "mkdocstrings[python]>=0.18",
   "griffe", "griffe-inherited-docstrings",
 ]
 testing = ["pytest", "sparecores-crawler[mkdocs]"]
 aws = ["boto3"]
 hcloud = ["hcloud"]
-vendors = ["sparecores-crawler[aws]", "sparecores-crawler[hcloud]"]
+gcp = ["google-cloud", "google-cloud-compute", "google-cloud-billing"]
+vendors = ["sparecores-crawler[aws]", "sparecores-crawler[hcloud]", "sparecores-crawler[gcp]"]
 all = ["sparecores-crawler[testing]", "sparecores-crawler[vendors]"]
 
 [project.scripts]
 sc-crawler = "sc_crawler.cli:cli"
 
 [tool.setuptools]
 include-package-data = true  # see MANIFEST.in
```

### Comparing `sparecores_crawler-0.1.1/src/sc_crawler/alembic/env.py` & `sparecores_crawler-0.1.2/src/sc_crawler/alembic/env.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.1/src/sc_crawler/alembic/versions/4691089690c2_v0_1_1.py` & `sparecores_crawler-0.1.2/src/sc_crawler/alembic/versions/4691089690c2_v0_1_1.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.1/src/sc_crawler/alembic/versions/98894dffd37c_v0_1_0.py` & `sparecores_crawler-0.1.2/src/sc_crawler/alembic/versions/98894dffd37c_v0_1_0.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.1/src/sc_crawler/alembic.ini` & `sparecores_crawler-0.1.2/src/sc_crawler/alembic.ini`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.1/src/sc_crawler/alembic_helpers.py` & `sparecores_crawler-0.1.2/src/sc_crawler/alembic_helpers.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.1/src/sc_crawler/cli.py` & `sparecores_crawler-0.1.2/src/sc_crawler/cli.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.1/src/sc_crawler/insert.py` & `sparecores_crawler-0.1.2/src/sc_crawler/insert.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.1/src/sc_crawler/logger.py` & `sparecores_crawler-0.1.2/src/sc_crawler/logger.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.1/src/sc_crawler/lookup.py` & `sparecores_crawler-0.1.2/src/sc_crawler/lookup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 from .tables import ComplianceFramework, Country
 
 # country codes: https://en.wikipedia.org/wiki/ISO_3166-1#Codes
 # mapping: https://github.com/manumanoj0010/countrydetails/blob/master/Countrydetails/data/continents.json  # noqa: E501
 country_continent_mapping = {
     "AE": "Asia",
     "AU": "Oceania",
+    "BE": "Europe",
     "BH": "Asia",
     "BR": "South America",
     "CA": "North America",
     "CH": "Europe",
+    "CL": "South America",
     "CN": "Asia",
     "DE": "Europe",
     "ES": "Europe",
     "FI": "Europe",
     "FR": "Europe",
     "GB": "Europe",
     "HK": "Asia",
@@ -22,16 +24,20 @@
     "IE": "Europe",
     "IL": "Asia",
     "IT": "Europe",
     "IN": "Asia",
     "JP": "Asia",
     "KR": "Asia",
     "NL": "Europe",
+    "PL": "Europe",
+    "QA": "Asia",
+    "SA": "Asia",
     "SE": "Europe",
     "SG": "Asia",
+    "TW": "Asia",
     "US": "North America",
     "ZA": "Africa",
 }
 
 
 countries: dict = {
     k: Country(country_id=k, continent=v) for k, v in country_continent_mapping.items()
```

### Comparing `sparecores_crawler-0.1.1/src/sc_crawler/str_utils.py` & `sparecores_crawler-0.1.2/src/sc_crawler/str_utils.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.1/src/sc_crawler/table_bases.py` & `sparecores_crawler-0.1.2/src/sc_crawler/table_bases.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.1/src/sc_crawler/table_fields.py` & `sparecores_crawler-0.1.2/src/sc_crawler/table_fields.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.1/src/sc_crawler/tables.py` & `sparecores_crawler-0.1.2/src/sc_crawler/tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,15 +249,15 @@
         self.set_table_rows_inactive(
             ServerPrice, ServerPrice.allocation == Allocation.SPOT
         )
         insert_items(
             ServerPrice,
             self._get_methods().inventory_server_prices_spot(self),
             self,
-            prefix="ondemand",
+            prefix="spot",
         )
 
     @log_start_end
     def inventory_storages(self):
         self._inventory(Storage, self._get_methods().inventory_storages)
 
     @log_start_end
```

### Comparing `sparecores_crawler-0.1.1/src/sc_crawler/tables_scd.py` & `sparecores_crawler-0.1.2/src/sc_crawler/tables_scd.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.1/src/sc_crawler/utils.py` & `sparecores_crawler-0.1.2/src/sc_crawler/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from collections import defaultdict
 from enum import Enum
 from hashlib import sha1
 from json import dumps
 from math import isinf
 from typing import Any, Dict, Iterable, List, Optional, Union
 
 from rich.progress import Progress
@@ -147,7 +148,20 @@
     Returns:
         ScModel object read from the database.
     """
     q = select(model)
     for k, v in pks.items():
         q = q.where(getattr(model, k) == v)
     return session.exec(statement=q).one()
+
+
+def nesteddefaultdict():
+    """Recursive defaultdict.
+
+    Examples:
+        >>> foo = nesteddefaultdict()
+        >>> foo["bar"]["baz"] = 43
+        >>> from json import dumps
+        >>> dumps(foo)
+        '{"bar": {"baz": 43}}'
+    """
+    return defaultdict(nesteddefaultdict)
```

### Comparing `sparecores_crawler-0.1.1/src/sc_crawler/vendors/aws.py` & `sparecores_crawler-0.1.2/src/sc_crawler/vendors/aws.py`

 * *Files 1% similar despite different names*

```diff
@@ -364,15 +364,18 @@
 
 
 # ##############################################################################
 # Public methods to fetch data
 
 
 def inventory_compliance_frameworks(vendor):
-    """Manual list of compliance frameworks known for AWS."""
+    """Manual list of compliance frameworks known for AWS.
+
+    Resources: <https://aws.amazon.com/compliance/programs/>
+    """
     return map_compliance_frameworks_to_vendor(
         vendor.vendor_id, ["hipaa", "soc2t2", "iso27001"]
     )
 
 
 def inventory_datacenters(vendor):
     """List all available AWS datacenters via `boto3` calls.
@@ -1040,14 +1043,15 @@
     vendor.progress_tracker.hide_task()
     return prices
 
 
 def inventory_traffic_prices(vendor):
     """List all inbound and outbound traffic prices in all regions via `boto3` calls."""
     datacenters = scmodels_to_dict(vendor.datacenters, keys=["name", "aliases"])
+    items = []
     for direction in list(TrafficDirection):
         loc_dir = "toLocation" if direction == TrafficDirection.IN else "fromLocation"
         vendor.progress_tracker.start_task(
             name=f"Searching for {direction.value} traffic_price(s)", total=None
         )
         products = _boto_get_products(
             service_code="AWSDataTransfer",
@@ -1056,15 +1060,14 @@
             },
         )
         vendor.log(f"Found {len(products)} {direction.value} traffic_price(s).")
         vendor.progress_tracker.update_task(
             description=f"Syncing {direction.value} traffic_price(s)",
             total=len(products),
         )
-        items = []
         for product in products:
             try:
                 datacenter = datacenters[product["product"]["attributes"][loc_dir]]
                 prices = _extract_ondemand_prices(product["terms"])
                 price = [PriceTier.model_validate(p).model_dump() for p in prices[0]]
                 items.append(
                     {
@@ -1078,15 +1081,15 @@
                     }
                 )
             except KeyError:
                 continue
             finally:
                 vendor.progress_tracker.advance_task()
         vendor.progress_tracker.hide_task()
-        return items
+    return items
 
 
 def inventory_ipv4_prices(vendor):
     """List IPV4 prices in all regions via `boto3` calls."""
     vendor.progress_tracker.start_task(name="Searching for ipv4_price(s)", total=None)
     products = _boto_get_products(
         service_code="AmazonVPC",
```

### Comparing `sparecores_crawler-0.1.1/src/sc_crawler/vendors/hcloud.py` & `sparecores_crawler-0.1.2/src/sc_crawler/vendors/hcloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     CpuAllocation,
     CpuArchitecture,
     PriceUnit,
     Status,
     StorageType,
     TrafficDirection,
 )
+from ..utils import scmodels_to_dict
 
 # ##############################################################################
 # Cached client wrappers
 
 
 @cache
 def _client() -> Client:
@@ -83,15 +84,15 @@
     for datacenter in _client().datacenters.get_all():
         items.append(
             {
                 "vendor_id": vendor.vendor_id,
                 "datacenter_id": str(datacenter.id),
                 "name": datacenter.name,
                 # TODO add datacenter.description
-                "aliases": [],
+                "aliases": [datacenter.location.name],
                 "country_id": datacenter.location.country,
                 "state": None,
                 "city": datacenter.location.city,
                 "address_line": None,
                 "zip_code": None,
                 "founding_year": None,
                 "green_energy": True,
@@ -175,22 +176,25 @@
                 "status": Status.ACTIVE if not server.deprecation else Status.INACTIVE,
             }
         )
     return items
 
 
 def inventory_server_prices(vendor):
+    datacenters = scmodels_to_dict(vendor.datacenters, keys=["name", "aliases"])
     items = []
     for server in _client().server_types.get_all():
         for location in server.prices:
+            datacenter_id = datacenters[location["location"]].datacenter_id
             items.append(
                 {
                     "vendor_id": vendor.vendor_id,
-                    "datacenter_id": location["location"],
-                    "zone_id": location["location"],
+                    "datacenter_id": datacenter_id,
+                    # zone_id is a dummy datacenter_id as there are no zones at Hetzner
+                    "zone_id": datacenter_id,
                     "server_id": str(server.id),
                     "operating_system": "Linux",
                     "allocation": Allocation.ONDEMAND,
                     "unit": PriceUnit.HOUR,
                     "price": float(location["price_hourly"]["net"]),
                     "price_upfront": 0,
                     "price_tiered": [],
@@ -268,15 +272,15 @@
                 "direction": TrafficDirection.IN,
             }
         )
         items.append(
             {
                 "vendor_id": vendor.vendor_id,
                 "datacenter_id": datacenter.datacenter_id,
-                "price": 1,
+                "price": round(1 / 1024, 8),
                 "price_tiered": [],
                 "currency": "EUR",
                 "unit": PriceUnit.GB_MONTH,
                 "direction": TrafficDirection.OUT,
             }
         )
     return items
```

### Comparing `sparecores_crawler-0.1.1/src/sc_crawler/vendors/vendors.py` & `sparecores_crawler-0.1.2/src/sc_crawler/vendors/vendors.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,50 @@
-"""Supported cloud and VPS provider vendors."""
+"""Supported cloud and VPS provider vendors.
+
+For logos, see e.g. <https://iconduck.com/sets/svg-logos>,
+and edit to square e.g. via <https://boxy-svg.com>.
+"""
 
 from ..lookup import countries
 from ..tables import Vendor
 
 aws = Vendor(
     vendor_id="aws",
     name="Amazon Web Services",
-    # TODO host on cdn.sparecores.com
-    logo="https://upload.wikimedia.org/wikipedia/commons/9/93/Amazon_Web_Services_Logo.svg",
+    logo="https://sc-data-public-40e9d310.s3.amazonaws.com/cdn/logos/aws.svg",
     homepage="https://aws.amazon.com",
     country=countries["US"],
     state="Washington",
     city="Seattle",
     address_line="410 Terry Ave N",
     zip_code="98109",
     founding_year=2002,
     status_page="https://health.aws.amazon.com/health/status",
 )
 """Amazon Web Services."""
 
 gcp = Vendor(
     vendor_id="gcp",
     name="Google Cloud Platform",
+    logo="https://sc-data-public-40e9d310.s3.amazonaws.com/cdn/logos/gcp.svg",
     homepage="https://cloud.google.com",
     country=countries["US"],
     state="California",
     city="Mountain View",
     address_line="1600 Amphitheatre Pkwy",
     zip_code="94043",
     founding_year=2008,
     status_page="https://status.cloud.google.com/",
 )
 """Google Cloud Platform."""
 
 hcloud = Vendor(
     vendor_id="hcloud",
     name="Hetzner Cloud",
+    logo="https://sc-data-public-40e9d310.s3.amazonaws.com/cdn/logos/hcloud.svg",
     homepage="https://www.hetzner.com/cloud/",
     country=countries["DE"],
     state="Bavaria",
     city="Gunzenhausen",
     address_line="Industriestr. 25",
     zip_code="91710",
     founding_year=1997,
```

### Comparing `sparecores_crawler-0.1.1/src/sparecores_crawler.egg-info/PKG-INFO` & `sparecores_crawler-0.1.2/src/sparecores_crawler.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: sparecores-crawler
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pull and standardize data on cloud compute resources.
 Author: Attila Nagy, Gergely Daroczi, Balazs Hodobay
 Maintainer-email: Spare Cores team <pkg@sparecores.com>
 Project-URL: repository, https://github.com/SpareCores/sc-crawler
 Project-URL: issues, https://github.com/SpareCores/sc-crawler/issues
 Project-URL: documentation, https://sparecores.github.io/sc-crawler/
+Project-URL: homepage, https://sparecores.com
+Keywords: cloud,compute,etl,sqlite,spot-instances,cost-optimization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -36,17 +38,22 @@
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: sparecores-crawler[mkdocs]; extra == "testing"
 Provides-Extra: aws
 Requires-Dist: boto3; extra == "aws"
 Provides-Extra: hcloud
 Requires-Dist: hcloud; extra == "hcloud"
+Provides-Extra: gcp
+Requires-Dist: google-cloud; extra == "gcp"
+Requires-Dist: google-cloud-compute; extra == "gcp"
+Requires-Dist: google-cloud-billing; extra == "gcp"
 Provides-Extra: vendors
 Requires-Dist: sparecores-crawler[aws]; extra == "vendors"
 Requires-Dist: sparecores-crawler[hcloud]; extra == "vendors"
+Requires-Dist: sparecores-crawler[gcp]; extra == "vendors"
 Provides-Extra: all
 Requires-Dist: sparecores-crawler[testing]; extra == "all"
 Requires-Dist: sparecores-crawler[vendors]; extra == "all"
 
 ## Spare Cores Crawler
 
 [![Build](https://img.shields.io/github/actions/workflow/status/SpareCores/sc-crawler/tests.yaml)](https://github.com/SpareCores/sc-crawler/actions/workflows/tests.yaml)
```

### Comparing `sparecores_crawler-0.1.1/src/sparecores_crawler.egg-info/SOURCES.txt` & `sparecores_crawler-0.1.2/src/sparecores_crawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.1/tests/test_schemas.py` & `sparecores_crawler-0.1.2/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.1/tests/test_str_utils.py` & `sparecores_crawler-0.1.2/tests/test_str_utils.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.1/tests/test_utils.py` & `sparecores_crawler-0.1.2/tests/test_utils.py`

 * *Files identical despite different names*

