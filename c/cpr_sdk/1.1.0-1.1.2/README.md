# Comparing `tmp/cpr_sdk-1.1.0.tar.gz` & `tmp/cpr_sdk-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpr_sdk-1.1.0.tar", max compression
+gzip compressed data, was "cpr_sdk-1.1.2.tar", max compression
```

## Comparing `cpr_sdk-1.1.0.tar` & `cpr_sdk-1.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1507 2024-04-11 09:15:11.625016 cpr_sdk-1.1.0/LICENSE
--rw-r--r--   0        0        0     6615 2024-04-11 09:15:11.625016 cpr_sdk-1.1.0/README.md
--rw-r--r--   0        0        0     2885 2024-04-11 09:15:35.217292 cpr_sdk-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       52 2024-04-11 09:15:11.625016 cpr_sdk-1.1.0/src/cpr_sdk/__init__.py
--rw-r--r--   0        0        0     5693 2024-04-11 09:15:11.625016 cpr_sdk-1.1.0/src/cpr_sdk/data_adaptors.py
--rw-r--r--   0        0        0     1118 2024-04-11 09:15:11.625016 cpr_sdk-1.1.0/src/cpr_sdk/embedding.py
--rw-r--r--   0        0        0      797 2024-04-11 09:15:11.625016 cpr_sdk-1.1.0/src/cpr_sdk/exceptions.py
--rw-r--r--   0        0        0    50630 2024-04-11 09:15:11.629016 cpr_sdk-1.1.0/src/cpr_sdk/models/__init__.py
--rw-r--r--   0        0        0    11979 2024-04-11 09:15:11.629016 cpr_sdk-1.1.0/src/cpr_sdk/models/search.py
--rw-r--r--   0        0        0    14816 2024-04-11 09:15:11.629016 cpr_sdk-1.1.0/src/cpr_sdk/parser_models.py
--rw-r--r--   0        0        0     2679 2024-04-11 09:15:11.629016 cpr_sdk-1.1.0/src/cpr_sdk/pipeline_general_models.py
--rw-r--r--   0        0        0    71013 2024-04-11 09:15:11.629016 cpr_sdk-1.1.0/src/cpr_sdk/resources/sensitive_query_terms.tsv
--rw-r--r--   0        0        0     2791 2024-04-11 09:15:11.629016 cpr_sdk-1.1.0/src/cpr_sdk/s3.py
--rw-r--r--   0        0        0     4584 2024-04-11 09:15:11.629016 cpr_sdk-1.1.0/src/cpr_sdk/search_adaptors.py
--rw-r--r--   0        0        0     4143 2024-04-11 09:15:11.629016 cpr_sdk-1.1.0/src/cpr_sdk/utils.py
--rw-r--r--   0        0        0      169 2024-04-11 09:15:11.629016 cpr_sdk-1.1.0/src/cpr_sdk/version.py
--rw-r--r--   0        0        0     6979 2024-04-11 09:15:11.629016 cpr_sdk-1.1.0/src/cpr_sdk/vespa.py
--rw-r--r--   0        0        0     7015 2024-04-11 09:15:11.629016 cpr_sdk-1.1.0/src/cpr_sdk/yql_builder.py
--rw-r--r--   0        0        0     7960 1970-01-01 00:00:00.000000 cpr_sdk-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1507 2024-04-25 10:37:27.273597 cpr_sdk-1.1.2/LICENSE
+-rw-r--r--   0        0        0     6615 2024-04-25 10:37:27.273597 cpr_sdk-1.1.2/README.md
+-rw-r--r--   0        0        0     2926 2024-04-25 10:38:35.301835 cpr_sdk-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0       52 2024-04-25 10:37:27.277597 cpr_sdk-1.1.2/src/cpr_sdk/__init__.py
+-rw-r--r--   0        0        0     5693 2024-04-25 10:37:27.277597 cpr_sdk-1.1.2/src/cpr_sdk/data_adaptors.py
+-rw-r--r--   0        0        0     1118 2024-04-25 10:37:27.277597 cpr_sdk-1.1.2/src/cpr_sdk/embedding.py
+-rw-r--r--   0        0        0      797 2024-04-25 10:37:27.277597 cpr_sdk-1.1.2/src/cpr_sdk/exceptions.py
+-rw-r--r--   0        0        0    50630 2024-04-25 10:37:27.277597 cpr_sdk-1.1.2/src/cpr_sdk/models/__init__.py
+-rw-r--r--   0        0        0    11979 2024-04-25 10:37:27.277597 cpr_sdk-1.1.2/src/cpr_sdk/models/search.py
+-rw-r--r--   0        0        0    14816 2024-04-25 10:37:27.277597 cpr_sdk-1.1.2/src/cpr_sdk/parser_models.py
+-rw-r--r--   0        0        0     2679 2024-04-25 10:37:27.277597 cpr_sdk-1.1.2/src/cpr_sdk/pipeline_general_models.py
+-rw-r--r--   0        0        0    71013 2024-04-25 10:37:27.277597 cpr_sdk-1.1.2/src/cpr_sdk/resources/sensitive_query_terms.tsv
+-rw-r--r--   0        0        0     2791 2024-04-25 10:37:27.277597 cpr_sdk-1.1.2/src/cpr_sdk/s3.py
+-rw-r--r--   0        0        0     4584 2024-04-25 10:37:27.277597 cpr_sdk-1.1.2/src/cpr_sdk/search_adaptors.py
+-rw-r--r--   0        0        0     4143 2024-04-25 10:37:27.277597 cpr_sdk-1.1.2/src/cpr_sdk/utils.py
+-rw-r--r--   0        0        0      169 2024-04-25 10:37:27.277597 cpr_sdk-1.1.2/src/cpr_sdk/version.py
+-rw-r--r--   0        0        0     6979 2024-04-25 10:37:27.277597 cpr_sdk-1.1.2/src/cpr_sdk/vespa.py
+-rw-r--r--   0        0        0     7015 2024-04-25 10:37:27.277597 cpr_sdk-1.1.2/src/cpr_sdk/yql_builder.py
+-rw-r--r--   0        0        0     7999 1970-01-01 00:00:00.000000 cpr_sdk-1.1.2/PKG-INFO
```

### Comparing `cpr_sdk-1.1.0/LICENSE` & `cpr_sdk-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.1.0/README.md` & `cpr_sdk-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.1.0/pyproject.toml` & `cpr_sdk-1.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cpr_sdk"
-# This version in a placeholder and should not be updated. 
-# During the release flow the version from the cpr_sdk/__init__.py is used. 
-version = "1.1.0"
+# This version is a placeholder that is overwritten during release.
+# The placeholder is replaced by the value from the cpr_sdk package itself.
+version = "1.1.2"
 description = ""
 authors = ["CPR Tech <tech@climatepolicyradar.org>"]
 readme = "README.md"
-packages = [{include = "cpr_sdk", from = "src"}]
+packages = [{ include = "cpr_sdk", from = "src" }]
 classifiers = [
-    "Intended Audience :: Science/Research",
-    "Programming Language :: Python :: 3",
-    "Topic :: Scientific/Engineering :: Artificial Intelligence",
+  "Intended Audience :: Science/Research",
+  "Programming Language :: Python :: 3",
+  "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 
 license = "LICENSE"
 
 [project.urls]
 Homepage = "https://github.com/climatepolicyradar/cpr-sdk"
 Repository = "https://github.com/climatepolicyradar/cpr-sdk"
@@ -33,45 +33,44 @@
 aws-error-utils = "^2.7.0"
 pandas = "^1.5.3"
 datasets = "^2.14.0"
 langdetect = "^1.0.9"
 deprecation = "^2.1.0"
 numpy = ">=1.23.5"
 
-pyvespa = { version = "^0.37.1", optional = true } 
-pyyaml = { version = "^6.0.1", optional = true } 
-sentence-transformers = { version = "^2.2.2", optional = true } 
-torch = { version = "^2.0.0", optional = true } 
-spacy = { version = "^3.5.1", optional = true } 
+pyvespa = { version = "^0.37.1", optional = true }
+pyyaml = { version = "^6.0.1", optional = true }
+sentence-transformers = { version = "^2.2.2", optional = true }
+torch = { version = "^2.0.0", optional = true }
+spacy = { version = "^3.5.1", optional = true }
+poetry = "^1.8.2"
 
 [tool.poetry.extras]
 vespa = ["pyvespa", "pyyaml", "sentence-transformers", "torch"]
 spacy = ["spacy"]
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.6.2"
 pyright = "^1.1.352"
 pytest = "^8.0.2"
 black = "^24.2.0"
-moto = {extras = ["s3"], version = "^5.0.2"}
+moto = { extras = ["s3"], version = "^5.0.2" }
 pytest-dotenv = "^0.5.2"
 
 
 [tool.pytest.ini_options]
 addopts = "-p no:cacheprovider"
 env_files = """
     .env.test
     .env
 """
-markers = [
-    "vespa",
-]
+markers = ["vespa"]
 
 [tool.black-jupyter]
 line-length = 88
 target-version = ["py39"]
 
 [tool.ruff]
 select = ["E", "F", "D"]
@@ -85,15 +84,29 @@
 # D213 - Multi-line docstring summary should start at the first line
 # D400 - First line should end with a period
 # D401 - First line should be in imperative mood
 # D406 - Section name should end with a newline
 # D407 - Missing dashed underline after section
 # D413 - Missing blank line after last section
 # D415 - First line should end with a period, question mark, or exclamation point
-ignore = ["D100", "D103", "D104", "D107", "D202", "D203", "D212", "D400", "D401", "D406", "D407", "D413", "D415", "E501"]
+ignore = [
+  "D100",
+  "D103",
+  "D104",
+  "D107",
+  "D202",
+  "D203",
+  "D212",
+  "D400",
+  "D401",
+  "D406",
+  "D407",
+  "D413",
+  "D415",
+  "E501",
+]
 line-length = 88
 
 # Ignore `E402` (import violations) in all `__init__.py` files, and in `path/to/file.py`.
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]
 "tests/*" = ["E501"]
-
```

### Comparing `cpr_sdk-1.1.0/src/cpr_sdk/data_adaptors.py` & `cpr_sdk-1.1.2/src/cpr_sdk/data_adaptors.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.1.0/src/cpr_sdk/embedding.py` & `cpr_sdk-1.1.2/src/cpr_sdk/embedding.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.1.0/src/cpr_sdk/exceptions.py` & `cpr_sdk-1.1.2/src/cpr_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.1.0/src/cpr_sdk/models/__init__.py` & `cpr_sdk-1.1.2/src/cpr_sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.1.0/src/cpr_sdk/models/search.py` & `cpr_sdk-1.1.2/src/cpr_sdk/models/search.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.1.0/src/cpr_sdk/parser_models.py` & `cpr_sdk-1.1.2/src/cpr_sdk/parser_models.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.1.0/src/cpr_sdk/pipeline_general_models.py` & `cpr_sdk-1.1.2/src/cpr_sdk/pipeline_general_models.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.1.0/src/cpr_sdk/resources/sensitive_query_terms.tsv` & `cpr_sdk-1.1.2/src/cpr_sdk/resources/sensitive_query_terms.tsv`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.1.0/src/cpr_sdk/s3.py` & `cpr_sdk-1.1.2/src/cpr_sdk/s3.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.1.0/src/cpr_sdk/search_adaptors.py` & `cpr_sdk-1.1.2/src/cpr_sdk/search_adaptors.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.1.0/src/cpr_sdk/utils.py` & `cpr_sdk-1.1.2/src/cpr_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.1.0/src/cpr_sdk/vespa.py` & `cpr_sdk-1.1.2/src/cpr_sdk/vespa.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.1.0/src/cpr_sdk/yql_builder.py` & `cpr_sdk-1.1.2/src/cpr_sdk/yql_builder.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-1.1.0/PKG-INFO` & `cpr_sdk-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpr_sdk
-Version: 1.1.0
+Version: 1.1.2
 Summary: 
 License: LICENSE
 Author: CPR Tech
 Author-email: tech@climatepolicyradar.org
 Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
@@ -19,14 +19,15 @@
 Requires-Dist: aws-error-utils (>=2.7.0,<3.0.0)
 Requires-Dist: boto3 (>=1.26.16,<2.0.0)
 Requires-Dist: datasets (>=2.14.0,<3.0.0)
 Requires-Dist: deprecation (>=2.1.0,<3.0.0)
 Requires-Dist: langdetect (>=1.0.9,<2.0.0)
 Requires-Dist: numpy (>=1.23.5)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: poetry (>=1.8.2,<2.0.0)
 Requires-Dist: pydantic (>=2.4.0,<3.0.0)
 Requires-Dist: pyvespa (>=0.37.1,<0.38.0) ; extra == "vespa"
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0) ; extra == "vespa"
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0) ; extra == "vespa"
 Requires-Dist: spacy (>=3.5.1,<4.0.0) ; extra == "spacy"
 Requires-Dist: torch (>=2.0.0,<3.0.0) ; extra == "vespa"
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
```

