# Comparing `tmp/turu_mysql-0.9.8.tar.gz` & `tmp/turu_mysql-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turu_mysql-0.9.8.tar", max compression
+gzip compressed data, was "turu_mysql-0.9.9.tar", max compression
```

## Comparing `turu_mysql-0.9.8.tar` & `turu_mysql-0.9.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       89 2024-02-08 05:52:19.134042 turu_mysql-0.9.8/README.md
--rw-r--r--   0        0        0     2155 2024-02-08 05:52:42.134088 turu_mysql-0.9.8/pyproject.toml
--rw-r--r--   0        0        0      873 2024-02-08 05:52:19.134042 turu_mysql-0.9.8/src/turu/mysql/__init__.py
--rw-r--r--   0        0        0     3011 2024-02-08 05:52:19.134042 turu_mysql-0.9.8/src/turu/mysql/async_connection.py
--rw-r--r--   0        0        0     4016 2024-02-08 05:52:19.134042 turu_mysql-0.9.8/src/turu/mysql/async_cursor.py
--rw-r--r--   0        0        0     3015 2024-02-08 05:52:19.134042 turu_mysql-0.9.8/src/turu/mysql/connection.py
--rw-r--r--   0        0        0     3975 2024-02-08 05:52:19.134042 turu_mysql-0.9.8/src/turu/mysql/cursor.py
--rw-r--r--   0        0        0      574 2024-02-08 05:52:19.134042 turu_mysql-0.9.8/src/turu/mysql/mock_async_connection.py
--rw-r--r--   0        0        0      318 2024-02-08 05:52:19.134042 turu_mysql-0.9.8/src/turu/mysql/mock_async_cursor.py
--rw-r--r--   0        0        0      462 2024-02-08 05:52:19.134042 turu_mysql-0.9.8/src/turu/mysql/mock_connection.py
--rw-r--r--   0        0        0      255 2024-02-08 05:52:19.134042 turu_mysql-0.9.8/src/turu/mysql/mock_cursor.py
--rw-r--r--   0        0        0        0 2024-02-08 05:52:19.134042 turu_mysql-0.9.8/src/turu/mysql/py.typed
--rw-r--r--   0        0        0     1470 1970-01-01 00:00:00.000000 turu_mysql-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0       89 2024-02-10 15:17:13.820242 turu_mysql-0.9.9/README.md
+-rw-r--r--   0        0        0     2155 2024-02-10 15:17:39.408164 turu_mysql-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0      873 2024-02-10 15:17:13.820242 turu_mysql-0.9.9/src/turu/mysql/__init__.py
+-rw-r--r--   0        0        0     3011 2024-02-10 15:17:13.820242 turu_mysql-0.9.9/src/turu/mysql/async_connection.py
+-rw-r--r--   0        0        0     4016 2024-02-10 15:17:13.820242 turu_mysql-0.9.9/src/turu/mysql/async_cursor.py
+-rw-r--r--   0        0        0     3015 2024-02-10 15:17:13.820242 turu_mysql-0.9.9/src/turu/mysql/connection.py
+-rw-r--r--   0        0        0     3975 2024-02-10 15:17:13.820242 turu_mysql-0.9.9/src/turu/mysql/cursor.py
+-rw-r--r--   0        0        0      574 2024-02-10 15:17:13.820242 turu_mysql-0.9.9/src/turu/mysql/mock_async_connection.py
+-rw-r--r--   0        0        0      318 2024-02-10 15:17:13.820242 turu_mysql-0.9.9/src/turu/mysql/mock_async_cursor.py
+-rw-r--r--   0        0        0      462 2024-02-10 15:17:13.820242 turu_mysql-0.9.9/src/turu/mysql/mock_connection.py
+-rw-r--r--   0        0        0      255 2024-02-10 15:17:13.820242 turu_mysql-0.9.9/src/turu/mysql/mock_cursor.py
+-rw-r--r--   0        0        0        0 2024-02-10 15:17:13.820242 turu_mysql-0.9.9/src/turu/mysql/py.typed
+-rw-r--r--   0        0        0     1470 1970-01-01 00:00:00.000000 turu_mysql-0.9.9/PKG-INFO
```

### Comparing `turu_mysql-0.9.8/pyproject.toml` & `turu_mysql-0.9.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "turu-mysql"
-version = "0.9.8"
+version = "0.9.9"
 description = "MySQL adapter for turu"
 authors = ["yassun7010 <yassun7010@outlook.com>"]
 readme = "README.md"
 packages = [{ include = "turu", from = "src" }]
 repository = "https://github.com/yassun7010/turu-py"
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -40,15 +40,15 @@
 python = "^3.8"
 typing-extensions = "^4.8.0"
 aiomysql = "^0.2.0"
 cryptography = "^41.0.7"
 
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

### Comparing `turu_mysql-0.9.8/src/turu/mysql/__init__.py` & `turu_mysql-0.9.9/src/turu/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `turu_mysql-0.9.8/src/turu/mysql/async_connection.py` & `turu_mysql-0.9.9/src/turu/mysql/async_connection.py`

 * *Files identical despite different names*

### Comparing `turu_mysql-0.9.8/src/turu/mysql/async_cursor.py` & `turu_mysql-0.9.9/src/turu/mysql/async_cursor.py`

 * *Files identical despite different names*

### Comparing `turu_mysql-0.9.8/src/turu/mysql/connection.py` & `turu_mysql-0.9.9/src/turu/mysql/connection.py`

 * *Files identical despite different names*

### Comparing `turu_mysql-0.9.8/src/turu/mysql/cursor.py` & `turu_mysql-0.9.9/src/turu/mysql/cursor.py`

 * *Files identical despite different names*

### Comparing `turu_mysql-0.9.8/src/turu/mysql/mock_async_connection.py` & `turu_mysql-0.9.9/src/turu/mysql/mock_async_connection.py`

 * *Files identical despite different names*

### Comparing `turu_mysql-0.9.8/PKG-INFO` & `turu_mysql-0.9.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turu-mysql
-Version: 0.9.8
+Version: 0.9.9
 Summary: MySQL adapter for turu
 Home-page: https://github.com/yassun7010/turu-py
 Author: yassun7010
 Author-email: yassun7010@outlook.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -21,15 +21,15 @@
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: aiomysql (>=0.2.0,<0.3.0)
 Requires-Dist: cryptography (>=41.0.7,<42.0.0)
-Requires-Dist: turu-core (==0.9.8)
+Requires-Dist: turu-core (==0.9.9)
 Requires-Dist: typing-extensions (>=4.8.0,<5.0.0)
 Project-URL: Repository, https://github.com/yassun7010/turu-py
 Description-Content-Type: text/markdown
 
 # turu-mysql
 
 This is a mysql adapter for [turu](https://github.com/yassun7010/turu-py).
```

