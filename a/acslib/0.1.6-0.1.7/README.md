# Comparing `tmp/acslib-0.1.6.tar.gz` & `tmp/acslib-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acslib-0.1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "acslib-0.1.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `acslib-0.1.6.tar` & `acslib-0.1.7.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0      163 2024-04-16 13:04:12.660568 acslib-0.1.6/.coveragerc
--rw-r--r--   0        0        0      104 2024-04-16 13:04:12.660568 acslib-0.1.6/.dockerignore
--rw-r--r--   0        0        0      292 2024-04-16 13:04:12.660568 acslib-0.1.6/.editorconfig
--rw-r--r--   0        0        0      296 2024-04-16 13:04:12.660568 acslib-0.1.6/.github/pr_template.md
--rw-r--r--   0        0        0     9382 2024-04-16 13:04:12.660568 acslib-0.1.6/.github/workflows/test_publish_release..yml
--rw-r--r--   0        0        0     1388 2024-04-16 13:04:12.660568 acslib-0.1.6/.gitignore
--rw-r--r--   0        0        0       81 2024-04-16 13:04:12.660568 acslib-0.1.6/.isort.cfg
--rw-r--r--   0        0        0      875 2024-04-16 13:04:12.660568 acslib-0.1.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      118 2024-04-16 13:04:12.660568 acslib-0.1.6/AUTHORS.md
--rw-r--r--   0        0        0      212 2024-04-16 13:04:12.660568 acslib-0.1.6/CONTRIBUTING.md
--rw-r--r--   0        0        0      473 2024-04-16 13:04:12.660568 acslib-0.1.6/Dockerfile
--rw-r--r--   0        0        0       59 2024-04-16 13:04:12.660568 acslib-0.1.6/HISTORY.md
--rw-r--r--   0        0        0     1089 2024-04-16 13:04:12.660568 acslib-0.1.6/LICENSE
--rw-r--r--   0        0        0      589 2024-04-16 13:04:12.660568 acslib-0.1.6/Makefile
--rw-r--r--   0        0        0     5171 2024-04-16 13:04:12.660568 acslib-0.1.6/README.md
--rw-r--r--   0        0        0      188 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/__init__.py
--rw-r--r--   0        0        0      218 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/base/__init__.py
--rw-r--r--   0        0        0      259 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/base/acs.py
--rw-r--r--   0        0        0      172 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/base/config.py
--rw-r--r--   0        0        0     6294 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/base/connection.py
--rw-r--r--   0        0        0      272 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/base/search.py
--rw-r--r--   0        0        0     6113 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/base/status.py
--rw-r--r--   0        0        0      322 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/ccure/__init__.py
--rw-r--r--   0        0        0      595 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/ccure/base.py
--rw-r--r--   0        0        0     2923 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/ccure/config.py
--rw-r--r--   0        0        0     7444 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/ccure/connection.py
--rw-r--r--   0        0        0    17177 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/ccure/crud.py
--rw-r--r--   0        0        0     1070 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/ccure/data_models.py
--rw-r--r--   0        0        0     1141 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/ccure/endpoints.py
--rw-r--r--   0        0        0     7674 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/ccure/filters.py
--rw-r--r--   0        0        0       36 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/ccure/tests/__init__.py
--rw-r--r--   0        0        0     1839 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/ccure/tests/conftest.py
--rw-r--r--   0        0        0     2037 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/ccure/tests/test_base.py
--rw-r--r--   0        0        0     2801 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/ccure/tests/test_config.py
--rw-r--r--   0        0        0     2111 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/ccure/tests/test_connection.py
--rw-r--r--   0        0        0     2588 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/ccure/tests/test_search.py
--rw-r--r--   0        0        0      348 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/ccure/types.py
--rw-r--r--   0        0        0       11 2024-04-16 13:04:12.660568 acslib-0.1.6/docs/api.md
--rw-r--r--   0        0        0       41 2024-04-16 13:04:12.660568 acslib-0.1.6/docs/authors.md
--rw-r--r--   0        0        0       46 2024-04-16 13:04:12.660568 acslib-0.1.6/docs/contributing.md
--rw-r--r--   0        0        0       41 2024-04-16 13:04:12.660568 acslib-0.1.6/docs/history.md
--rw-r--r--   0        0        0       42 2024-04-16 13:04:12.660568 acslib-0.1.6/docs/index.md
--rw-r--r--   0        0        0     1188 2024-04-16 13:04:12.660568 acslib-0.1.6/docs/installation.md
--rw-r--r--   0        0        0       87 2024-04-16 13:04:12.664568 acslib-0.1.6/docs/usage.md
--rw-r--r--   0        0        0       20 2024-04-16 13:04:12.664568 acslib-0.1.6/envrc_sample
--rw-r--r--   0        0        0     1949 2024-04-16 13:04:12.664568 acslib-0.1.6/mkdocs.yml
--rw-r--r--   0        0        0     1918 2024-04-16 13:04:12.664568 acslib-0.1.6/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint
--rw-r--r--   0        0        0     2314 2024-04-16 13:04:12.664568 acslib-0.1.6/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint.ipynb
--rw-r--r--   0        0        0    12624 2024-04-16 13:04:12.664568 acslib-0.1.6/notebooks/encode_investigation.ipynb
--rw-r--r--   0        0        0     2699 2024-04-16 13:04:12.664568 acslib-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      219 2024-04-16 13:04:12.664568 acslib-0.1.6/pytest.ini
--rw-r--r--   0        0        0      926 2024-04-16 13:04:12.664568 acslib-0.1.6/requirements/base/base.txt
--rw-r--r--   0        0        0     4618 2024-04-16 13:04:12.664568 acslib-0.1.6/requirements/dev/dev.txt
--rw-r--r--   0        0        0     6756 1970-01-01 00:00:00.000000 acslib-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      163 2024-04-25 17:42:34.491990 acslib-0.1.7/.coveragerc
+-rw-r--r--   0        0        0      104 2024-04-25 17:42:34.491990 acslib-0.1.7/.dockerignore
+-rw-r--r--   0        0        0      292 2024-04-25 17:42:34.491990 acslib-0.1.7/.editorconfig
+-rw-r--r--   0        0        0      296 2024-04-25 17:42:34.491990 acslib-0.1.7/.github/pr_template.md
+-rw-r--r--   0        0        0     9382 2024-04-25 17:42:34.491990 acslib-0.1.7/.github/workflows/test_publish_release..yml
+-rw-r--r--   0        0        0     1388 2024-04-25 17:42:34.491990 acslib-0.1.7/.gitignore
+-rw-r--r--   0        0        0       81 2024-04-25 17:42:34.491990 acslib-0.1.7/.isort.cfg
+-rw-r--r--   0        0        0      875 2024-04-25 17:42:34.491990 acslib-0.1.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      118 2024-04-25 17:42:34.491990 acslib-0.1.7/AUTHORS.md
+-rw-r--r--   0        0        0      212 2024-04-25 17:42:34.491990 acslib-0.1.7/CONTRIBUTING.md
+-rw-r--r--   0        0        0      473 2024-04-25 17:42:34.491990 acslib-0.1.7/Dockerfile
+-rw-r--r--   0        0        0       59 2024-04-25 17:42:34.491990 acslib-0.1.7/HISTORY.md
+-rw-r--r--   0        0        0     1089 2024-04-25 17:42:34.491990 acslib-0.1.7/LICENSE
+-rw-r--r--   0        0        0      589 2024-04-25 17:42:34.491990 acslib-0.1.7/Makefile
+-rw-r--r--   0        0        0     5171 2024-04-25 17:42:34.491990 acslib-0.1.7/README.md
+-rw-r--r--   0        0        0      188 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/__init__.py
+-rw-r--r--   0        0        0      218 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/base/__init__.py
+-rw-r--r--   0        0        0      259 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/base/acs.py
+-rw-r--r--   0        0        0      172 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/base/config.py
+-rw-r--r--   0        0        0     6294 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/base/connection.py
+-rw-r--r--   0        0        0      272 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/base/search.py
+-rw-r--r--   0        0        0     6113 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/base/status.py
+-rw-r--r--   0        0        0      322 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/ccure/__init__.py
+-rw-r--r--   0        0        0      595 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/ccure/base.py
+-rw-r--r--   0        0        0     2923 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/ccure/config.py
+-rw-r--r--   0        0        0     7444 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/ccure/connection.py
+-rw-r--r--   0        0        0    17568 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/ccure/crud.py
+-rw-r--r--   0        0        0     1070 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/ccure/data_models.py
+-rw-r--r--   0        0        0     1141 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/ccure/endpoints.py
+-rw-r--r--   0        0        0     7674 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/ccure/filters.py
+-rw-r--r--   0        0        0       36 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/ccure/tests/__init__.py
+-rw-r--r--   0        0        0     1839 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/ccure/tests/conftest.py
+-rw-r--r--   0        0        0     2037 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/ccure/tests/test_base.py
+-rw-r--r--   0        0        0     2801 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/ccure/tests/test_config.py
+-rw-r--r--   0        0        0     2111 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/ccure/tests/test_connection.py
+-rw-r--r--   0        0        0     2588 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/ccure/tests/test_search.py
+-rw-r--r--   0        0        0      348 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/ccure/types.py
+-rw-r--r--   0        0        0       11 2024-04-25 17:42:34.491990 acslib-0.1.7/docs/api.md
+-rw-r--r--   0        0        0       41 2024-04-25 17:42:34.491990 acslib-0.1.7/docs/authors.md
+-rw-r--r--   0        0        0       46 2024-04-25 17:42:34.491990 acslib-0.1.7/docs/contributing.md
+-rw-r--r--   0        0        0       41 2024-04-25 17:42:34.491990 acslib-0.1.7/docs/history.md
+-rw-r--r--   0        0        0       42 2024-04-25 17:42:34.491990 acslib-0.1.7/docs/index.md
+-rw-r--r--   0        0        0     1188 2024-04-25 17:42:34.491990 acslib-0.1.7/docs/installation.md
+-rw-r--r--   0        0        0       87 2024-04-25 17:42:34.491990 acslib-0.1.7/docs/usage.md
+-rw-r--r--   0        0        0       20 2024-04-25 17:42:34.491990 acslib-0.1.7/envrc_sample
+-rw-r--r--   0        0        0     1949 2024-04-25 17:42:34.491990 acslib-0.1.7/mkdocs.yml
+-rw-r--r--   0        0        0     1918 2024-04-25 17:42:34.491990 acslib-0.1.7/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint
+-rw-r--r--   0        0        0     2314 2024-04-25 17:42:34.491990 acslib-0.1.7/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint.ipynb
+-rw-r--r--   0        0        0    12624 2024-04-25 17:42:34.491990 acslib-0.1.7/notebooks/encode_investigation.ipynb
+-rw-r--r--   0        0        0     2699 2024-04-25 17:42:34.491990 acslib-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      219 2024-04-25 17:42:34.491990 acslib-0.1.7/pytest.ini
+-rw-r--r--   0        0        0      926 2024-04-25 17:42:34.491990 acslib-0.1.7/requirements/base/base.txt
+-rw-r--r--   0        0        0     4618 2024-04-25 17:42:34.491990 acslib-0.1.7/requirements/dev/dev.txt
+-rw-r--r--   0        0        0     6756 1970-01-01 00:00:00.000000 acslib-0.1.7/PKG-INFO
```

### Comparing `acslib-0.1.6/.github/workflows/test_publish_release..yml` & `acslib-0.1.7/.github/workflows/test_publish_release..yml`

 * *Files identical despite different names*

### Comparing `acslib-0.1.6/.gitignore` & `acslib-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `acslib-0.1.6/.pre-commit-config.yaml` & `acslib-0.1.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `acslib-0.1.6/LICENSE` & `acslib-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `acslib-0.1.6/Makefile` & `acslib-0.1.7/Makefile`

 * *Files identical despite different names*

### Comparing `acslib-0.1.6/README.md` & `acslib-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `acslib-0.1.6/acslib/base/connection.py` & `acslib-0.1.7/acslib/base/connection.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.6/acslib/base/status.py` & `acslib-0.1.7/acslib/base/status.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.6/acslib/ccure/base.py` & `acslib-0.1.7/acslib/ccure/base.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.6/acslib/ccure/config.py` & `acslib-0.1.7/acslib/ccure/config.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.6/acslib/ccure/connection.py` & `acslib-0.1.7/acslib/ccure/connection.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.6/acslib/ccure/crud.py` & `acslib-0.1.7/acslib/ccure/crud.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 from typing import Optional
 
-from acslib.base import ACSRequestData, ACSRequestResponse
+from acslib.base import ACSRequestData, ACSRequestResponse, status, ACSRequestException
 from acslib.base.connection import ACSRequestMethod
 from acslib.ccure.base import CcureACS
 from acslib.ccure.connection import CcureConnection
 from acslib.ccure.filters import (
     ClearanceFilter,
     ClearanceItemFilter,
     CredentialFilter,
@@ -179,22 +179,28 @@
             request_data=ACSRequestData(
                 url=self.config.base_url + self.config.endpoints.FIND_OBJS_W_CRITERIA,
                 request_json=request_options,
                 headers=self.connection.base_headers,
             ),
         ).json
 
-    def update(self, record_id: int, update_data: dict) -> ACSRequestResponse:
-        pass
+    def update(self, *args, **kwargs) -> ACSRequestResponse:
+        raise ACSRequestException(
+            status.HTTP_501_NOT_IMPLEMENTED, "Updating clearances is not currently supported."
+        )
 
-    def create(self, create_data: dict) -> ACSRequestResponse:
-        pass
+    def create(self, *args, **kwargs) -> ACSRequestResponse:
+        raise ACSRequestException(
+            status.HTTP_501_NOT_IMPLEMENTED, "Creating clearances is not currently supported."
+        )
 
-    def delete(self, record_id: int) -> ACSRequestResponse:
-        pass
+    def delete(self, *args, **kwargs) -> ACSRequestResponse:
+        raise ACSRequestException(
+            status.HTTP_501_NOT_IMPLEMENTED, "Deleting clearances is not currently supported."
+        )
 
 
 class CcureCredential(CcureACS):
     def __init__(self, connection: Optional[CcureConnection] = None):
         super().__init__(connection)
         self.search_filter = CredentialFilter()
```

### Comparing `acslib-0.1.6/acslib/ccure/data_models.py` & `acslib-0.1.7/acslib/ccure/data_models.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.6/acslib/ccure/endpoints.py` & `acslib-0.1.7/acslib/ccure/endpoints.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.6/acslib/ccure/filters.py` & `acslib-0.1.7/acslib/ccure/filters.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.6/acslib/ccure/tests/conftest.py` & `acslib-0.1.7/acslib/ccure/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.6/acslib/ccure/tests/test_base.py` & `acslib-0.1.7/acslib/ccure/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.6/acslib/ccure/tests/test_config.py` & `acslib-0.1.7/acslib/ccure/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.6/acslib/ccure/tests/test_connection.py` & `acslib-0.1.7/acslib/ccure/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.6/acslib/ccure/tests/test_search.py` & `acslib-0.1.7/acslib/ccure/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.6/docs/installation.md` & `acslib-0.1.7/docs/installation.md`

 * *Files identical despite different names*

### Comparing `acslib-0.1.6/mkdocs.yml` & `acslib-0.1.7/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `acslib-0.1.6/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint` & `acslib-0.1.7/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint`

 * *Files identical despite different names*

### Comparing `acslib-0.1.6/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint.ipynb` & `acslib-0.1.7/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `acslib-0.1.6/notebooks/encode_investigation.ipynb` & `acslib-0.1.7/notebooks/encode_investigation.ipynb`

 * *Files identical despite different names*

### Comparing `acslib-0.1.6/pyproject.toml` & `acslib-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.2, <4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "acslib"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
     { name="Jeremy Gibson", email="jmgibso3@ncsu.edu" },
     { name="Luc Sanchez", email="lgsanche@ncsu.edu" },
     { name="Ryan Semmler", email="rsemmle@ncsu.edu" },
 ]
 description = "A library for interacting with Access Control Systems like Genetec or Ccure9k"
 readme = "README.md"
```

### Comparing `acslib-0.1.6/requirements/base/base.txt` & `acslib-0.1.7/requirements/base/base.txt`

 * *Files identical despite different names*

### Comparing `acslib-0.1.6/requirements/dev/dev.txt` & `acslib-0.1.7/requirements/dev/dev.txt`

 * *Files identical despite different names*

### Comparing `acslib-0.1.6/PKG-INFO` & `acslib-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acslib
-Version: 0.1.6
+Version: 0.1.7
 Summary: A library for interacting with Access Control Systems like Genetec or Ccure9k
 Author-email: Jeremy Gibson <jmgibso3@ncsu.edu>, Luc Sanchez <lgsanche@ncsu.edu>, Ryan Semmler <rsemmle@ncsu.edu>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic>=2.5.3, <3.0.0
 Requires-Dist: sat-utils>=1.1.12, <2.0.0
 Requires-Dist: pytest>=6.2.5, <7.0.0 ; extra == "dev"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: acslib Version: 0.1.6 Summary: A library for
+Metadata-Version: 2.1 Name: acslib Version: 0.1.7 Summary: A library for
 interacting with Access Control Systems like Genetec or Ccure9k Author-email:
 Jeremy Gibson
 ncsu.edu>, Luc Sanchez
 ncsu.edu>, Ryan Semmler
 ncsu.edu> Requires-Python: >=3.10 Description-Content-Type: text/markdown
 Requires-Dist: pydantic>=2.5.3, <3.0.0 Requires-Dist: sat-utils>=1.1.12, <2.0.0
 Requires-Dist: pytest>=6.2.5, <7.0.0 ; extra == "dev" Requires-Dist: pytest-
```

