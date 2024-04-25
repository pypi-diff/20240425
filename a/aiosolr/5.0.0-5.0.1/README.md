# Comparing `tmp/aiosolr-5.0.0.tar.gz` & `tmp/aiosolr-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiosolr-5.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiosolr-5.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiosolr-5.0.0.tar` & `aiosolr-5.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      865 2020-07-02 02:10:06.000000 aiosolr-5.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1217 2019-08-23 19:48:55.000000 aiosolr-5.0.0/.gitignore
--rw-r--r--   0        0        0    12471 2024-03-05 16:14:27.227899 aiosolr-5.0.0/.pylintrc
--rw-r--r--   0        0        0      447 2021-06-10 19:49:05.087000 aiosolr-5.0.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1073 2021-06-10 19:49:05.087359 aiosolr-5.0.0/LICENSE.md
--rw-r--r--   0        0        0     1529 2024-04-04 15:56:49.098443 aiosolr-5.0.0/Makefile
--rw-r--r--   0        0        0     3923 2024-04-04 15:47:10.871940 aiosolr-5.0.0/README.md
--rw-r--r--   0        0        0    22806 2024-04-04 15:54:26.819827 aiosolr-5.0.0/aiosolr.py
--rwxr-xr-x   0        0        0       48 2021-06-10 19:49:07.028510 aiosolr-5.0.0/githooks/pre-commit
--rw-r--r--   0        0        0      787 2024-04-04 16:05:32.241358 aiosolr-5.0.0/pyproject.toml
--rw-r--r--   0        0        0       92 2024-04-04 15:57:58.073707 aiosolr-5.0.0/requirements.in
--rw-r--r--   0        0        0     3271 2024-04-04 15:59:01.350044 aiosolr-5.0.0/requirements.txt
--rw-r--r--   0        0        0      227 2021-06-10 19:49:05.089652 aiosolr-5.0.0/setup.cfg
--rw-r--r--   0        0        0     1222 2024-04-04 16:04:55.947358 aiosolr-5.0.0/setup.py
--rw-r--r--   0        0        0      517 2024-03-05 16:14:27.230893 aiosolr-5.0.0/tests/test_clean.py
--rw-r--r--   0        0        0      222 1970-01-01 00:00:00.000000 aiosolr-5.0.0/PKG-INFO
+-rw-r--r--   0        0        0      865 2020-07-02 02:10:06.000000 aiosolr-5.0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1217 2019-08-23 19:48:55.000000 aiosolr-5.0.1/.gitignore
+-rw-r--r--   0        0        0    12471 2024-03-05 16:14:27.227899 aiosolr-5.0.1/.pylintrc
+-rw-r--r--   0        0        0      447 2021-06-10 19:49:05.087000 aiosolr-5.0.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1073 2021-06-10 19:49:05.087359 aiosolr-5.0.1/LICENSE.md
+-rw-r--r--   0        0        0     1539 2024-04-25 02:45:04.496385 aiosolr-5.0.1/Makefile
+-rw-r--r--   0        0        0     3923 2024-04-04 15:47:10.871940 aiosolr-5.0.1/README.md
+-rw-r--r--   0        0        0    22806 2024-04-25 02:54:33.015882 aiosolr-5.0.1/aiosolr.py
+-rwxr-xr-x   0        0        0       48 2021-06-10 19:49:07.028510 aiosolr-5.0.1/githooks/pre-commit
+-rw-r--r--   0        0        0     1227 2024-04-25 02:51:44.879002 aiosolr-5.0.1/pyproject.toml
+-rw-r--r--   0        0        0       92 2024-04-25 02:45:04.498006 aiosolr-5.0.1/requirements.in
+-rw-r--r--   0        0        0     3271 2024-04-25 02:45:04.498438 aiosolr-5.0.1/requirements.txt
+-rw-r--r--   0        0        0      227 2021-06-10 19:49:05.089652 aiosolr-5.0.1/setup.cfg
+-rw-r--r--   0        0        0     1222 2024-04-25 02:45:04.498855 aiosolr-5.0.1/setup.py
+-rw-r--r--   0        0        0      517 2024-03-05 16:14:27.230893 aiosolr-5.0.1/tests/test_clean.py
+-rw-r--r--   0        0        0     4600 1970-01-01 00:00:00.000000 aiosolr-5.0.1/PKG-INFO
```

### Comparing `aiosolr-5.0.0/.github/workflows/python-publish.yml` & `aiosolr-5.0.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `aiosolr-5.0.0/.gitignore` & `aiosolr-5.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `aiosolr-5.0.0/.pylintrc` & `aiosolr-5.0.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `aiosolr-5.0.0/LICENSE.md` & `aiosolr-5.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aiosolr-5.0.0/Makefile` & `aiosolr-5.0.1/Makefile`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 	@isort aiosolr.py --check --diff
 	@echo "isort looks good!"
 	@echo
 
 lint: black isort pylint
 
 publish:
-	@flit publish
+	@python -m flit publish
 
 pylint:
 	@pylint --help > /dev/null || (echo "Error: pylint not found"; exit 1)
 	@echo "> running pylint..."
 	@pylint --rcfile=.pylintrc aiosolr.py
 	@echo "pylint looks good!"
```

### Comparing `aiosolr-5.0.0/README.md` & `aiosolr-5.0.1/README.md`

 * *Files identical despite different names*

### Comparing `aiosolr-5.0.0/aiosolr.py` & `aiosolr-5.0.1/aiosolr.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import re
 import urllib.parse
 from typing import TYPE_CHECKING
 
 import aiohttp
 import bleach
 
-__version__ = "5.0.0"
+__version__ = "5.0.1"
 
 LOGGER = logging.getLogger("aiosolr")
 
 
 class SolrError(Exception):
     """Base class for exceptions in this module."""
```

### Comparing `aiosolr-5.0.0/pyproject.toml` & `aiosolr-5.0.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,30 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "aiosolr"
 authors = [{name = "Brad Belyeu", email = "bradley.belyeu@youversion.com"}]
+classifiers=[
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python",
+    "Topic :: Internet :: WWW/HTTP :: Indexing/Search",
+    "Programming Language :: Python :: 3",
+]
+dependencies = [
+    "aiohttp >= 3.8",
+    "bleach >= 6",
+]
 dynamic = ["version", "description"]
+keywords = ["solr", "asyncio", "aiohttp", "search"]
+readme = "README.md"
+requires-python = ">=3.10"
 
 [project.urls]
 Home = "https://github.com/bbelyeu/aiosolr"
 
 [tool.black]
 line-length = 100
 exclude = '''
```

### Comparing `aiosolr-5.0.0/requirements.txt` & `aiosolr-5.0.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `aiosolr-5.0.0/setup.py` & `aiosolr-5.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `aiosolr-5.0.0/tests/test_clean.py` & `aiosolr-5.0.1/tests/test_clean.py`

 * *Files identical despite different names*

