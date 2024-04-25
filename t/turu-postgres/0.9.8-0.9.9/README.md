# Comparing `tmp/turu_postgres-0.9.8.tar.gz` & `tmp/turu_postgres-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turu_postgres-0.9.8.tar", max compression
+gzip compressed data, was "turu_postgres-0.9.9.tar", max compression
```

## Comparing `turu_postgres-0.9.8.tar` & `turu_postgres-0.9.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       95 2024-02-08 05:52:19.054453 turu_postgres-0.9.8/README.md
--rw-r--r--   0        0        0     2138 2024-02-08 05:52:40.250306 turu_postgres-0.9.8/pyproject.toml
--rw-r--r--   0        0        0      876 2024-02-08 05:52:19.054453 turu_postgres-0.9.8/src/turu/postgres/__init__.py
--rw-r--r--   0        0        0     3237 2024-02-08 05:52:19.054453 turu_postgres-0.9.8/src/turu/postgres/async_connection.py
--rw-r--r--   0        0        0     4019 2024-02-08 05:52:19.054453 turu_postgres-0.9.8/src/turu/postgres/async_cursor.py
--rw-r--r--   0        0        0     3063 2024-02-08 05:52:19.054453 turu_postgres-0.9.8/src/turu/postgres/connection.py
--rw-r--r--   0        0        0     3947 2024-02-08 05:52:19.054453 turu_postgres-0.9.8/src/turu/postgres/cursor.py
--rw-r--r--   0        0        0      586 2024-02-08 05:52:19.054453 turu_postgres-0.9.8/src/turu/postgres/mock_async_connection.py
--rw-r--r--   0        0        0      318 2024-02-08 05:52:19.054453 turu_postgres-0.9.8/src/turu/postgres/mock_async_cursor.py
--rw-r--r--   0        0        0      462 2024-02-08 05:52:19.054453 turu_postgres-0.9.8/src/turu/postgres/mock_connection.py
--rw-r--r--   0        0        0      255 2024-02-08 05:52:19.054453 turu_postgres-0.9.8/src/turu/postgres/mock_cursor.py
--rw-r--r--   0        0        0        0 2024-02-08 05:52:19.054453 turu_postgres-0.9.8/src/turu/postgres/py.typed
--rw-r--r--   0        0        0     1437 1970-01-01 00:00:00.000000 turu_postgres-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0       95 2024-02-10 15:17:13.686678 turu_postgres-0.9.9/README.md
+-rw-r--r--   0        0        0     2138 2024-02-10 15:17:37.606854 turu_postgres-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0      876 2024-02-10 15:17:13.686678 turu_postgres-0.9.9/src/turu/postgres/__init__.py
+-rw-r--r--   0        0        0     3237 2024-02-10 15:17:13.686678 turu_postgres-0.9.9/src/turu/postgres/async_connection.py
+-rw-r--r--   0        0        0     4019 2024-02-10 15:17:13.686678 turu_postgres-0.9.9/src/turu/postgres/async_cursor.py
+-rw-r--r--   0        0        0     3063 2024-02-10 15:17:13.686678 turu_postgres-0.9.9/src/turu/postgres/connection.py
+-rw-r--r--   0        0        0     3947 2024-02-10 15:17:13.686678 turu_postgres-0.9.9/src/turu/postgres/cursor.py
+-rw-r--r--   0        0        0      586 2024-02-10 15:17:13.686678 turu_postgres-0.9.9/src/turu/postgres/mock_async_connection.py
+-rw-r--r--   0        0        0      318 2024-02-10 15:17:13.686678 turu_postgres-0.9.9/src/turu/postgres/mock_async_cursor.py
+-rw-r--r--   0        0        0      462 2024-02-10 15:17:13.686678 turu_postgres-0.9.9/src/turu/postgres/mock_connection.py
+-rw-r--r--   0        0        0      255 2024-02-10 15:17:13.686678 turu_postgres-0.9.9/src/turu/postgres/mock_cursor.py
+-rw-r--r--   0        0        0        0 2024-02-10 15:17:13.686678 turu_postgres-0.9.9/src/turu/postgres/py.typed
+-rw-r--r--   0        0        0     1437 1970-01-01 00:00:00.000000 turu_postgres-0.9.9/PKG-INFO
```

### Comparing `turu_postgres-0.9.8/pyproject.toml` & `turu_postgres-0.9.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "turu-postgres"
-version = "0.9.8"
+version = "0.9.9"
 description = "PostgreSQL adapter for turu"
 authors = ["yassun7010 <yassun7010@outlook.com>"]
 readme = "README.md"
 packages = [{ include = "turu", from = "src" }]
 repository = "https://github.com/yassun7010/turu-py"
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -39,15 +39,15 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 typing-extensions = "^4.8.0"
 psycopg = "^3.1.16"
 
 [tool.poetry.dependencies.turu-core]
 # INFO: poetry-dynamic-versioning to replace this.
-version = "0.9.8"
+version = "0.9.9"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 
 [[tool.poetry-dynamic-versioning.substitution.folders]]
 path = "."
 files = ["pyproject.toml"]
```

### Comparing `turu_postgres-0.9.8/src/turu/postgres/__init__.py` & `turu_postgres-0.9.9/src/turu/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `turu_postgres-0.9.8/src/turu/postgres/async_connection.py` & `turu_postgres-0.9.9/src/turu/postgres/async_connection.py`

 * *Files identical despite different names*

### Comparing `turu_postgres-0.9.8/src/turu/postgres/async_cursor.py` & `turu_postgres-0.9.9/src/turu/postgres/async_cursor.py`

 * *Files identical despite different names*

### Comparing `turu_postgres-0.9.8/src/turu/postgres/connection.py` & `turu_postgres-0.9.9/src/turu/postgres/connection.py`

 * *Files identical despite different names*

### Comparing `turu_postgres-0.9.8/src/turu/postgres/cursor.py` & `turu_postgres-0.9.9/src/turu/postgres/cursor.py`

 * *Files identical despite different names*

### Comparing `turu_postgres-0.9.8/src/turu/postgres/mock_async_connection.py` & `turu_postgres-0.9.9/src/turu/postgres/mock_async_connection.py`

 * *Files identical despite different names*

### Comparing `turu_postgres-0.9.8/PKG-INFO` & `turu_postgres-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turu-postgres
-Version: 0.9.8
+Version: 0.9.9
 Summary: PostgreSQL adapter for turu
 Home-page: https://github.com/yassun7010/turu-py
 Author: yassun7010
 Author-email: yassun7010@outlook.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -20,15 +20,15 @@
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: psycopg (>=3.1.16,<4.0.0)
-Requires-Dist: turu-core (==0.9.8)
+Requires-Dist: turu-core (==0.9.9)
 Requires-Dist: typing-extensions (>=4.8.0,<5.0.0)
 Project-URL: Repository, https://github.com/yassun7010/turu-py
 Description-Content-Type: text/markdown
 
 # turu-postgres
 
 This is a postgres adapter for [turu](https://github.com/yassun7010/turu-py).
```

