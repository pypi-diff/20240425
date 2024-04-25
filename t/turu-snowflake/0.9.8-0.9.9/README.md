# Comparing `tmp/turu_snowflake-0.9.8.tar.gz` & `tmp/turu_snowflake-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turu_snowflake-0.9.8.tar", max compression
+gzip compressed data, was "turu_snowflake-0.9.9.tar", max compression
```

## Comparing `turu_snowflake-0.9.8.tar` & `turu_snowflake-0.9.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       97 2024-02-08 05:52:20.254832 turu_snowflake-0.9.8/README.md
--rw-r--r--   0        0        0     2590 2024-02-08 05:52:43.922933 turu_snowflake-0.9.8/pyproject.toml
--rw-r--r--   0        0        0      860 2024-02-08 05:52:20.254832 turu_snowflake-0.9.8/src/turu/snowflake/__init__.py
--rw-r--r--   0        0        0    10626 2024-02-08 05:52:20.254832 turu_snowflake-0.9.8/src/turu/snowflake/async_connection.py
--rw-r--r--   0        0        0    11875 2024-02-08 05:52:20.254832 turu_snowflake-0.9.8/src/turu/snowflake/async_cursor.py
--rw-r--r--   0        0        0    10351 2024-02-08 05:52:20.254832 turu_snowflake-0.9.8/src/turu/snowflake/connection.py
--rw-r--r--   0        0        0    11259 2024-02-08 05:52:20.254832 turu_snowflake-0.9.8/src/turu/snowflake/cursor.py
--rw-r--r--   0        0        0     1644 2024-02-08 05:52:20.254832 turu_snowflake-0.9.8/src/turu/snowflake/features.py
--rw-r--r--   0        0        0     4261 2024-02-08 05:52:20.254832 turu_snowflake-0.9.8/src/turu/snowflake/mock_async_connection.py
--rw-r--r--   0        0        0     6501 2024-02-08 05:52:20.254832 turu_snowflake-0.9.8/src/turu/snowflake/mock_async_cursor.py
--rw-r--r--   0        0        0     4322 2024-02-08 05:52:20.254832 turu_snowflake-0.9.8/src/turu/snowflake/mock_connection.py
--rw-r--r--   0        0        0     6209 2024-02-08 05:52:20.254832 turu_snowflake-0.9.8/src/turu/snowflake/mock_cursor.py
--rw-r--r--   0        0        0        0 2024-02-08 05:52:20.254832 turu_snowflake-0.9.8/src/turu/snowflake/py.typed
--rw-r--r--   0        0        0      339 2024-02-08 05:52:20.254832 turu_snowflake-0.9.8/src/turu/snowflake/record/__init__.py
--rw-r--r--   0        0        0      600 2024-02-08 05:52:20.254832 turu_snowflake-0.9.8/src/turu/snowflake/record/async_record_cursor.py
--rw-r--r--   0        0        0      584 2024-02-08 05:52:20.254832 turu_snowflake-0.9.8/src/turu/snowflake/record/record_cursor.py
--rw-r--r--   0        0        0     1677 1970-01-01 00:00:00.000000 turu_snowflake-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0       97 2024-02-10 15:17:12.866681 turu_snowflake-0.9.9/README.md
+-rw-r--r--   0        0        0     2590 2024-02-10 15:17:34.294700 turu_snowflake-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0      860 2024-02-10 15:17:12.866681 turu_snowflake-0.9.9/src/turu/snowflake/__init__.py
+-rw-r--r--   0        0        0    10626 2024-02-10 15:17:12.866681 turu_snowflake-0.9.9/src/turu/snowflake/async_connection.py
+-rw-r--r--   0        0        0    11875 2024-02-10 15:17:12.866681 turu_snowflake-0.9.9/src/turu/snowflake/async_cursor.py
+-rw-r--r--   0        0        0    10351 2024-02-10 15:17:12.866681 turu_snowflake-0.9.9/src/turu/snowflake/connection.py
+-rw-r--r--   0        0        0    11259 2024-02-10 15:17:12.866681 turu_snowflake-0.9.9/src/turu/snowflake/cursor.py
+-rw-r--r--   0        0        0     1644 2024-02-10 15:17:12.866681 turu_snowflake-0.9.9/src/turu/snowflake/features.py
+-rw-r--r--   0        0        0     4261 2024-02-10 15:17:12.866681 turu_snowflake-0.9.9/src/turu/snowflake/mock_async_connection.py
+-rw-r--r--   0        0        0     6501 2024-02-10 15:17:12.866681 turu_snowflake-0.9.9/src/turu/snowflake/mock_async_cursor.py
+-rw-r--r--   0        0        0     4322 2024-02-10 15:17:12.866681 turu_snowflake-0.9.9/src/turu/snowflake/mock_connection.py
+-rw-r--r--   0        0        0     6209 2024-02-10 15:17:12.866681 turu_snowflake-0.9.9/src/turu/snowflake/mock_cursor.py
+-rw-r--r--   0        0        0        0 2024-02-10 15:17:12.866681 turu_snowflake-0.9.9/src/turu/snowflake/py.typed
+-rw-r--r--   0        0        0      339 2024-02-10 15:17:12.866681 turu_snowflake-0.9.9/src/turu/snowflake/record/__init__.py
+-rw-r--r--   0        0        0      721 2024-02-10 15:17:12.866681 turu_snowflake-0.9.9/src/turu/snowflake/record/async_record_cursor.py
+-rw-r--r--   0        0        0      705 2024-02-10 15:17:12.866681 turu_snowflake-0.9.9/src/turu/snowflake/record/record_cursor.py
+-rw-r--r--   0        0        0     1677 1970-01-01 00:00:00.000000 turu_snowflake-0.9.9/PKG-INFO
```

### Comparing `turu_snowflake-0.9.8/pyproject.toml` & `turu_snowflake-0.9.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "turu-snowflake"
-version = "0.9.8"
+version = "0.9.9"
 description = "snowflake adapter for turu"
 authors = ["yassun7010 <yassun7010@outlook.com>"]
 readme = "README.md"
 packages = [{ include = "turu", from = "src" }]
 repository = "https://github.com/yassun7010/turu-py"
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -38,15 +38,15 @@
 snowflake-connector-python = "^3.6.0"
 pandas = { version = "*", optional = true }
 pyarrow = { version = "*", optional = true }
 pandera = { version = "^0.18.0", optional = true }
 
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

### Comparing `turu_snowflake-0.9.8/src/turu/snowflake/__init__.py` & `turu_snowflake-0.9.9/src/turu/snowflake/__init__.py`

 * *Files identical despite different names*

### Comparing `turu_snowflake-0.9.8/src/turu/snowflake/async_connection.py` & `turu_snowflake-0.9.9/src/turu/snowflake/async_connection.py`

 * *Files identical despite different names*

### Comparing `turu_snowflake-0.9.8/src/turu/snowflake/async_cursor.py` & `turu_snowflake-0.9.9/src/turu/snowflake/async_cursor.py`

 * *Files identical despite different names*

### Comparing `turu_snowflake-0.9.8/src/turu/snowflake/connection.py` & `turu_snowflake-0.9.9/src/turu/snowflake/connection.py`

 * *Files identical despite different names*

### Comparing `turu_snowflake-0.9.8/src/turu/snowflake/cursor.py` & `turu_snowflake-0.9.9/src/turu/snowflake/cursor.py`

 * *Files identical despite different names*

### Comparing `turu_snowflake-0.9.8/src/turu/snowflake/features.py` & `turu_snowflake-0.9.9/src/turu/snowflake/features.py`

 * *Files identical despite different names*

### Comparing `turu_snowflake-0.9.8/src/turu/snowflake/mock_async_connection.py` & `turu_snowflake-0.9.9/src/turu/snowflake/mock_async_connection.py`

 * *Files identical despite different names*

### Comparing `turu_snowflake-0.9.8/src/turu/snowflake/mock_async_cursor.py` & `turu_snowflake-0.9.9/src/turu/snowflake/mock_async_cursor.py`

 * *Files identical despite different names*

### Comparing `turu_snowflake-0.9.8/src/turu/snowflake/mock_connection.py` & `turu_snowflake-0.9.9/src/turu/snowflake/mock_connection.py`

 * *Files identical despite different names*

### Comparing `turu_snowflake-0.9.8/src/turu/snowflake/mock_cursor.py` & `turu_snowflake-0.9.9/src/turu/snowflake/mock_cursor.py`

 * *Files identical despite different names*

### Comparing `turu_snowflake-0.9.8/src/turu/snowflake/record/async_record_cursor.py` & `turu_snowflake-0.9.9/src/turu/snowflake/record/async_record_cursor.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,13 +4,19 @@
 
 class AsyncRecordCursor(turu.core.record.AsyncRecordCursor):
     async def fetch_pandas_all(self, **kwargs) -> "PandasDataFrame":
         df: PandasDataFrame = self._raw_cursor.fetch_pandas_all(**kwargs)  # type: ignore
 
         if isinstance(self._recorder, turu.core.record.CsvRecorder):
             if limit := self._recorder._options.get("limit"):
-                df.head(limit).to_csv(self._recorder.file, index=False)
+                record_df = df.head(limit)
 
             else:
-                df.to_csv(self._recorder.file, index=False)
+                record_df = df
+
+            record_df.to_csv(
+                self._recorder.file,
+                index=False,
+                header=self._recorder._options.get("header", True),
+            )
 
         return df
```

### Comparing `turu_snowflake-0.9.8/src/turu/snowflake/record/record_cursor.py` & `turu_snowflake-0.9.9/src/turu/snowflake/record/record_cursor.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,13 +4,19 @@
 
 class RecordCursor(turu.core.record.RecordCursor):
     def fetch_pandas_all(self, **kwargs) -> "PandasDataFrame":
         df: PandasDataFrame = self._raw_cursor.fetch_pandas_all(**kwargs)  # type: ignore
 
         if isinstance(self._recorder, turu.core.record.CsvRecorder):
             if limit := self._recorder._options.get("limit"):
-                df.head(limit).to_csv(self._recorder.file, index=False)
+                record_df = df.head(limit)
 
             else:
-                df.to_csv(self._recorder.file, index=False)
+                record_df = df
+
+            record_df.to_csv(
+                self._recorder.file,
+                index=False,
+                header=self._recorder._options.get("header", True),
+            )
 
         return df
```

### Comparing `turu_snowflake-0.9.8/PKG-INFO` & `turu_snowflake-0.9.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turu-snowflake
-Version: 0.9.8
+Version: 0.9.9
 Summary: snowflake adapter for turu
 Home-page: https://github.com/yassun7010/turu-py
 Author: yassun7010
 Author-email: yassun7010@outlook.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -26,15 +26,15 @@
 Provides-Extra: pandas
 Provides-Extra: pandera
 Provides-Extra: pyarrow
 Requires-Dist: pandas ; extra == "pandas"
 Requires-Dist: pandera (>=0.18.0,<0.19.0) ; extra == "pandera"
 Requires-Dist: pyarrow ; extra == "pyarrow"
 Requires-Dist: snowflake-connector-python (>=3.6.0,<4.0.0)
-Requires-Dist: turu-core (==0.9.8)
+Requires-Dist: turu-core (==0.9.9)
 Requires-Dist: typing-extensions (>=4.9.0,<5.0.0)
 Project-URL: Repository, https://github.com/yassun7010/turu-py
 Description-Content-Type: text/markdown
 
 # turu-snowflake
 
 This is a snowflake adapter for [turu](https://github.com/yassun7010/turu-py).
```

