# Comparing `tmp/turu-0.9.8.tar.gz` & `tmp/turu-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turu-0.9.8.tar", max compression
+gzip compressed data, was "turu-0.9.9.tar", max compression
```

## Comparing `turu-0.9.8.tar` & `turu-0.9.9.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     4180 2024-02-08 05:52:59.839725 turu-0.9.8/README.md
--rw-r--r--   0        0        0     3391 2024-02-08 05:53:26.051432 turu-0.9.8/pyproject.toml
--rw-r--r--   0        0        0       72 2024-02-08 05:52:59.839725 turu-0.9.8/src/turu/version.py
--rw-r--r--   0        0        0     5931 1970-01-01 00:00:00.000000 turu-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0     4180 2024-02-10 15:17:56.631607 turu-0.9.9/README.md
+-rw-r--r--   0        0        0     3399 2024-02-10 15:18:20.419602 turu-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0       72 2024-02-10 15:17:56.635607 turu-0.9.9/src/turu/version.py
+-rw-r--r--   0        0        0     5931 1970-01-01 00:00:00.000000 turu-0.9.9/PKG-INFO
```

### Comparing `turu-0.9.8/README.md` & `turu-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `turu-0.9.8/pyproject.toml` & `turu-0.9.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "turu"
-version = "0.9.8"
+version = "0.9.9"
 description = "Simple Typed Python Database Client based PEP 249"
 authors = ["yassun7010 <yassun7010@outlook.com>"]
 readme = "README.md"
 repository = "https://github.com/yassun7010/turu-py"
 documentation = "https://yassun7010.github.io/turu-py/"
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -35,46 +35,46 @@
 bigquery = ["turu-bigquery"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 
 [tool.poetry.dependencies.turu-core]
 # INFO: poetry-dynamic-versioning to replace this.
-version = "0.9.8"
+version = "0.9.9"
 
 [tool.poetry.dependencies.turu-sqlite3]
 # INFO: poetry-dynamic-versioning to replace this.
-version = "0.9.8"
+version = "0.9.9"
 optional = true
 
 [tool.poetry.dependencies.turu-mysql]
 # INFO: poetry-dynamic-versioning to replace this.
-version = "0.9.8"
+version = "0.9.9"
 optional = true
 
 [tool.poetry.dependencies.turu-postgres]
 # INFO: poetry-dynamic-versioning to replace this.
-version = "0.9.8"
+version = "0.9.9"
 optional = true
 
 [tool.poetry.dependencies.turu-snowflake]
 # INFO: poetry-dynamic-versioning to replace this.
-version = "0.9.8"
+version = "0.9.9"
 optional = true
 
 [tool.poetry.dependencies.turu-bigquery]
 # INFO: poetry-dynamic-versioning to replace this.
-version = "0.9.8"
+version = "0.9.9"
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.4"
 taskipy = "^1.12.0"
 pyright = "^1.1.345"
-ruff = "^0.1.11"
+ruff = ">=0.1.11,<0.3.0"
 pydantic = "^2.5.3"
 pytest-cov = "^4.1.0"
 pytest-asyncio = "^0.23.3"
 pytest-xdist = "^3.5.0"
 pandera = "^0.18.0"
 typing-extensions = "^4.9.0"
```

### Comparing `turu-0.9.8/PKG-INFO` & `turu-0.9.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turu
-Version: 0.9.8
+Version: 0.9.9
 Summary: Simple Typed Python Database Client based PEP 249
 Home-page: https://github.com/yassun7010/turu-py
 Author: yassun7010
 Author-email: yassun7010@outlook.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -24,20 +24,20 @@
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: bigquery
 Provides-Extra: mysql
 Provides-Extra: postgres
 Provides-Extra: snowflake
 Provides-Extra: sqlite3
-Requires-Dist: turu-bigquery (==0.9.8) ; extra == "bigquery"
-Requires-Dist: turu-core (==0.9.8)
-Requires-Dist: turu-mysql (==0.9.8) ; extra == "mysql"
-Requires-Dist: turu-postgres (==0.9.8) ; extra == "postgres"
-Requires-Dist: turu-snowflake (==0.9.8) ; extra == "snowflake"
-Requires-Dist: turu-sqlite3 (==0.9.8) ; extra == "sqlite3"
+Requires-Dist: turu-bigquery (==0.9.9) ; extra == "bigquery"
+Requires-Dist: turu-core (==0.9.9)
+Requires-Dist: turu-mysql (==0.9.9) ; extra == "mysql"
+Requires-Dist: turu-postgres (==0.9.9) ; extra == "postgres"
+Requires-Dist: turu-snowflake (==0.9.9) ; extra == "snowflake"
+Requires-Dist: turu-sqlite3 (==0.9.9) ; extra == "sqlite3"
 Project-URL: Documentation, https://yassun7010.github.io/turu-py/
 Project-URL: Repository, https://github.com/yassun7010/turu-py
 Description-Content-Type: text/markdown
 
 # Turu: Simple Database Client for Typed Python
 
 <!-- --8<-- [start:badges] -->
```

