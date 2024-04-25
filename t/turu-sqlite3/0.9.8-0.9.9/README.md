# Comparing `tmp/turu_sqlite3-0.9.8.tar.gz` & `tmp/turu_sqlite3-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turu_sqlite3-0.9.8.tar", max compression
+gzip compressed data, was "turu_sqlite3-0.9.9.tar", max compression
```

## Comparing `turu_sqlite3-0.9.8.tar` & `turu_sqlite3-0.9.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       93 2024-02-08 05:52:18.960444 turu_sqlite3-0.9.8/README.md
--rw-r--r--   0        0        0     2136 2024-02-08 05:52:38.988433 turu_sqlite3-0.9.8/pyproject.toml
--rw-r--r--   0        0        0      698 2024-02-08 05:52:18.960444 turu_sqlite3-0.9.8/src/turu/sqlite3/__init__.py
--rw-r--r--   0        0        0     1471 2024-02-08 05:52:18.960444 turu_sqlite3-0.9.8/src/turu/sqlite3/async_connection.py
--rw-r--r--   0        0        0     4090 2024-02-08 05:52:18.960444 turu_sqlite3-0.9.8/src/turu/sqlite3/async_cursor.py
--rw-r--r--   0        0        0     1460 2024-02-08 05:52:18.960444 turu_sqlite3-0.9.8/src/turu/sqlite3/connection.py
--rw-r--r--   0        0        0     3547 2024-02-08 05:52:18.960444 turu_sqlite3-0.9.8/src/turu/sqlite3/cursor.py
--rw-r--r--   0        0        0      582 2024-02-08 05:52:18.960444 turu_sqlite3-0.9.8/src/turu/sqlite3/mock_async_connection.py
--rw-r--r--   0        0        0      338 2024-02-08 05:52:18.960444 turu_sqlite3-0.9.8/src/turu/sqlite3/mock_async_cursor.py
--rw-r--r--   0        0        0      476 2024-02-08 05:52:18.960444 turu_sqlite3-0.9.8/src/turu/sqlite3/mock_connection.py
--rw-r--r--   0        0        0      349 2024-02-08 05:52:18.960444 turu_sqlite3-0.9.8/src/turu/sqlite3/mock_cursor.py
--rw-r--r--   0        0        0        0 2024-02-08 05:52:18.960444 turu_sqlite3-0.9.8/src/turu/sqlite3/py.typed
--rw-r--r--   0        0        0     1434 1970-01-01 00:00:00.000000 turu_sqlite3-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0       93 2024-02-10 15:17:12.896201 turu_sqlite3-0.9.9/README.md
+-rw-r--r--   0        0        0     2136 2024-02-10 15:17:33.804486 turu_sqlite3-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0      698 2024-02-10 15:17:12.896201 turu_sqlite3-0.9.9/src/turu/sqlite3/__init__.py
+-rw-r--r--   0        0        0     1471 2024-02-10 15:17:12.896201 turu_sqlite3-0.9.9/src/turu/sqlite3/async_connection.py
+-rw-r--r--   0        0        0     4090 2024-02-10 15:17:12.896201 turu_sqlite3-0.9.9/src/turu/sqlite3/async_cursor.py
+-rw-r--r--   0        0        0     1460 2024-02-10 15:17:12.896201 turu_sqlite3-0.9.9/src/turu/sqlite3/connection.py
+-rw-r--r--   0        0        0     3547 2024-02-10 15:17:12.896201 turu_sqlite3-0.9.9/src/turu/sqlite3/cursor.py
+-rw-r--r--   0        0        0      582 2024-02-10 15:17:12.896201 turu_sqlite3-0.9.9/src/turu/sqlite3/mock_async_connection.py
+-rw-r--r--   0        0        0      338 2024-02-10 15:17:12.896201 turu_sqlite3-0.9.9/src/turu/sqlite3/mock_async_cursor.py
+-rw-r--r--   0        0        0      476 2024-02-10 15:17:12.896201 turu_sqlite3-0.9.9/src/turu/sqlite3/mock_connection.py
+-rw-r--r--   0        0        0      349 2024-02-10 15:17:12.896201 turu_sqlite3-0.9.9/src/turu/sqlite3/mock_cursor.py
+-rw-r--r--   0        0        0        0 2024-02-10 15:17:12.896201 turu_sqlite3-0.9.9/src/turu/sqlite3/py.typed
+-rw-r--r--   0        0        0     1434 1970-01-01 00:00:00.000000 turu_sqlite3-0.9.9/PKG-INFO
```

### Comparing `turu_sqlite3-0.9.8/pyproject.toml` & `turu_sqlite3-0.9.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "turu-sqlite3"
-version = "0.9.8"
+version = "0.9.9"
 description = "sqlite3 adapter for turu"
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
 aiosqlite = "^0.19.0"
 
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

### Comparing `turu_sqlite3-0.9.8/src/turu/sqlite3/__init__.py` & `turu_sqlite3-0.9.9/src/turu/sqlite3/__init__.py`

 * *Files identical despite different names*

### Comparing `turu_sqlite3-0.9.8/src/turu/sqlite3/async_connection.py` & `turu_sqlite3-0.9.9/src/turu/sqlite3/async_connection.py`

 * *Files identical despite different names*

### Comparing `turu_sqlite3-0.9.8/src/turu/sqlite3/async_cursor.py` & `turu_sqlite3-0.9.9/src/turu/sqlite3/async_cursor.py`

 * *Files identical despite different names*

### Comparing `turu_sqlite3-0.9.8/src/turu/sqlite3/connection.py` & `turu_sqlite3-0.9.9/src/turu/sqlite3/connection.py`

 * *Files identical despite different names*

### Comparing `turu_sqlite3-0.9.8/src/turu/sqlite3/cursor.py` & `turu_sqlite3-0.9.9/src/turu/sqlite3/cursor.py`

 * *Files identical despite different names*

### Comparing `turu_sqlite3-0.9.8/src/turu/sqlite3/mock_async_connection.py` & `turu_sqlite3-0.9.9/src/turu/sqlite3/mock_async_connection.py`

 * *Files identical despite different names*

### Comparing `turu_sqlite3-0.9.8/PKG-INFO` & `turu_sqlite3-0.9.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turu-sqlite3
-Version: 0.9.8
+Version: 0.9.9
 Summary: sqlite3 adapter for turu
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
 Requires-Dist: aiosqlite (>=0.19.0,<0.20.0)
-Requires-Dist: turu-core (==0.9.8)
+Requires-Dist: turu-core (==0.9.9)
 Requires-Dist: typing-extensions (>=4.8.0,<5.0.0)
 Project-URL: Repository, https://github.com/yassun7010/turu-py
 Description-Content-Type: text/markdown
 
 # turu-sqlite3
 
 This is a sqlite3 adapter for [turu](https://github.com/yassun7010/turu-py).
```

