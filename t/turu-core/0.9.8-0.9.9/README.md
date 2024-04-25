# Comparing `tmp/turu_core-0.9.8.tar.gz` & `tmp/turu_core-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turu_core-0.9.8.tar", max compression
+gzip compressed data, was "turu_core-0.9.9.tar", max compression
```

## Comparing `turu_core-0.9.8.tar` & `turu_core-0.9.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      150 2024-02-08 05:51:41.505591 turu_core-0.9.8/README.md
--rw-r--r--   0        0        0     1860 2024-02-08 05:52:06.021876 turu_core-0.9.8/pyproject.toml
--rw-r--r--   0        0        0       81 2024-02-08 05:51:41.505591 turu_core-0.9.8/src/turu/core/__init__.py
--rw-r--r--   0        0        0     4724 2024-02-08 05:51:41.505591 turu_core-0.9.8/src/turu/core/async_connection.py
--rw-r--r--   0        0        0     3271 2024-02-08 05:51:41.505591 turu_core-0.9.8/src/turu/core/async_cursor.py
--rw-r--r--   0        0        0     4512 2024-02-08 05:51:41.505591 turu_core-0.9.8/src/turu/core/connection.py
--rw-r--r--   0        0        0     4212 2024-02-08 05:51:41.505591 turu_core-0.9.8/src/turu/core/cursor.py
--rw-r--r--   0        0        0     1398 2024-02-08 05:51:41.505591 turu_core-0.9.8/src/turu/core/exception.py
--rw-r--r--   0        0        0      332 2024-02-08 05:51:41.505591 turu_core-0.9.8/src/turu/core/features.py
--rw-r--r--   0        0        0      267 2024-02-08 05:51:41.505591 turu_core-0.9.8/src/turu/core/mock/__init__.py
--rw-r--r--   0        0        0     2614 2024-02-08 05:51:41.505591 turu_core-0.9.8/src/turu/core/mock/async_connection.py
--rw-r--r--   0        0        0     4023 2024-02-08 05:51:41.505591 turu_core-0.9.8/src/turu/core/mock/async_cursor.py
--rw-r--r--   0        0        0     2580 2024-02-08 05:51:41.505591 turu_core-0.9.8/src/turu/core/mock/connection.py
--rw-r--r--   0        0        0     3757 2024-02-08 05:51:41.505591 turu_core-0.9.8/src/turu/core/mock/cursor.py
--rw-r--r--   0        0        0     1369 2024-02-08 05:51:41.505591 turu_core-0.9.8/src/turu/core/mock/exception.py
--rw-r--r--   0        0        0     1613 2024-02-08 05:51:41.505591 turu_core-0.9.8/src/turu/core/mock/store.py
--rw-r--r--   0        0        0        0 2024-02-08 05:51:41.505591 turu_core-0.9.8/src/turu/core/protocols/__init__.py
--rw-r--r--   0        0        0      769 2024-02-08 05:51:41.509590 turu_core-0.9.8/src/turu/core/protocols/async_connection.py
--rw-r--r--   0        0        0     3373 2024-02-08 05:51:41.509590 turu_core-0.9.8/src/turu/core/protocols/async_cursor.py
--rw-r--r--   0        0        0      666 2024-02-08 05:51:41.509590 turu_core-0.9.8/src/turu/core/protocols/connection.py
--rw-r--r--   0        0        0     2973 2024-02-08 05:51:41.509590 turu_core-0.9.8/src/turu/core/protocols/cursor.py
--rw-r--r--   0        0        0      114 2024-02-08 05:51:41.509590 turu_core-0.9.8/src/turu/core/protocols/dataclass.py
--rw-r--r--   0        0        0        0 2024-02-08 05:51:41.509590 turu_core-0.9.8/src/turu/core/py.typed
--rw-r--r--   0        0        0     4733 2024-02-08 05:51:41.509590 turu_core-0.9.8/src/turu/core/record/__init__.py
--rw-r--r--   0        0        0     3470 2024-02-08 05:51:41.509590 turu_core-0.9.8/src/turu/core/record/async_record_cursor.py
--rw-r--r--   0        0        0     3414 2024-02-08 05:51:41.509590 turu_core-0.9.8/src/turu/core/record/csv_recorder.py
--rw-r--r--   0        0        0     3215 2024-02-08 05:51:41.509590 turu_core-0.9.8/src/turu/core/record/record_cursor.py
--rw-r--r--   0        0        0      228 2024-02-08 05:51:41.509590 turu_core-0.9.8/src/turu/core/record/recorder_protcol.py
--rw-r--r--   0        0        0     1465 1970-01-01 00:00:00.000000 turu_core-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0      150 2024-02-10 15:16:33.988391 turu_core-0.9.9/README.md
+-rw-r--r--   0        0        0     1860 2024-02-10 15:16:59.180575 turu_core-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0       81 2024-02-10 15:16:33.988391 turu_core-0.9.9/src/turu/core/__init__.py
+-rw-r--r--   0        0        0     4724 2024-02-10 15:16:33.988391 turu_core-0.9.9/src/turu/core/async_connection.py
+-rw-r--r--   0        0        0     3271 2024-02-10 15:16:33.988391 turu_core-0.9.9/src/turu/core/async_cursor.py
+-rw-r--r--   0        0        0     4512 2024-02-10 15:16:33.988391 turu_core-0.9.9/src/turu/core/connection.py
+-rw-r--r--   0        0        0     4212 2024-02-10 15:16:33.988391 turu_core-0.9.9/src/turu/core/cursor.py
+-rw-r--r--   0        0        0     1398 2024-02-10 15:16:33.988391 turu_core-0.9.9/src/turu/core/exception.py
+-rw-r--r--   0        0        0      332 2024-02-10 15:16:33.988391 turu_core-0.9.9/src/turu/core/features.py
+-rw-r--r--   0        0        0      267 2024-02-10 15:16:33.988391 turu_core-0.9.9/src/turu/core/mock/__init__.py
+-rw-r--r--   0        0        0     2614 2024-02-10 15:16:33.988391 turu_core-0.9.9/src/turu/core/mock/async_connection.py
+-rw-r--r--   0        0        0     4023 2024-02-10 15:16:33.988391 turu_core-0.9.9/src/turu/core/mock/async_cursor.py
+-rw-r--r--   0        0        0     2580 2024-02-10 15:16:33.988391 turu_core-0.9.9/src/turu/core/mock/connection.py
+-rw-r--r--   0        0        0     3757 2024-02-10 15:16:33.988391 turu_core-0.9.9/src/turu/core/mock/cursor.py
+-rw-r--r--   0        0        0     1369 2024-02-10 15:16:33.988391 turu_core-0.9.9/src/turu/core/mock/exception.py
+-rw-r--r--   0        0        0     1621 2024-02-10 15:16:33.988391 turu_core-0.9.9/src/turu/core/mock/store.py
+-rw-r--r--   0        0        0        0 2024-02-10 15:16:33.988391 turu_core-0.9.9/src/turu/core/protocols/__init__.py
+-rw-r--r--   0        0        0      769 2024-02-10 15:16:33.988391 turu_core-0.9.9/src/turu/core/protocols/async_connection.py
+-rw-r--r--   0        0        0     3373 2024-02-10 15:16:33.988391 turu_core-0.9.9/src/turu/core/protocols/async_cursor.py
+-rw-r--r--   0        0        0      666 2024-02-10 15:16:33.988391 turu_core-0.9.9/src/turu/core/protocols/connection.py
+-rw-r--r--   0        0        0     2973 2024-02-10 15:16:33.988391 turu_core-0.9.9/src/turu/core/protocols/cursor.py
+-rw-r--r--   0        0        0      114 2024-02-10 15:16:33.988391 turu_core-0.9.9/src/turu/core/protocols/dataclass.py
+-rw-r--r--   0        0        0        0 2024-02-10 15:16:33.988391 turu_core-0.9.9/src/turu/core/py.typed
+-rw-r--r--   0        0        0     4733 2024-02-10 15:16:33.988391 turu_core-0.9.9/src/turu/core/record/__init__.py
+-rw-r--r--   0        0        0     3470 2024-02-10 15:16:33.988391 turu_core-0.9.9/src/turu/core/record/async_record_cursor.py
+-rw-r--r--   0        0        0     3414 2024-02-10 15:16:33.988391 turu_core-0.9.9/src/turu/core/record/csv_recorder.py
+-rw-r--r--   0        0        0     3215 2024-02-10 15:16:33.988391 turu_core-0.9.9/src/turu/core/record/record_cursor.py
+-rw-r--r--   0        0        0      228 2024-02-10 15:16:33.988391 turu_core-0.9.9/src/turu/core/record/recorder_protcol.py
+-rw-r--r--   0        0        0     1465 1970-01-01 00:00:00.000000 turu_core-0.9.9/PKG-INFO
```

### Comparing `turu_core-0.9.8/pyproject.toml` & `turu_core-0.9.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "turu-core"
-version = "0.9.8"
+version = "0.9.9"
 description = ""
 authors = ["yassun7010 <yassun7010@outlook.com>"]
 readme = "README.md"
 packages = [{ include = "turu", from = "src" }]
 repository = "https://github.com/yassun7010/turu-py"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `turu_core-0.9.8/src/turu/core/async_connection.py` & `turu_core-0.9.9/src/turu/core/async_connection.py`

 * *Files identical despite different names*

### Comparing `turu_core-0.9.8/src/turu/core/async_cursor.py` & `turu_core-0.9.9/src/turu/core/async_cursor.py`

 * *Files identical despite different names*

### Comparing `turu_core-0.9.8/src/turu/core/connection.py` & `turu_core-0.9.9/src/turu/core/connection.py`

 * *Files identical despite different names*

### Comparing `turu_core-0.9.8/src/turu/core/cursor.py` & `turu_core-0.9.9/src/turu/core/cursor.py`

 * *Files identical despite different names*

### Comparing `turu_core-0.9.8/src/turu/core/exception.py` & `turu_core-0.9.9/src/turu/core/exception.py`

 * *Files identical despite different names*

### Comparing `turu_core-0.9.8/src/turu/core/mock/async_connection.py` & `turu_core-0.9.9/src/turu/core/mock/async_connection.py`

 * *Files identical despite different names*

### Comparing `turu_core-0.9.8/src/turu/core/mock/async_cursor.py` & `turu_core-0.9.9/src/turu/core/mock/async_cursor.py`

 * *Files identical despite different names*

### Comparing `turu_core-0.9.8/src/turu/core/mock/connection.py` & `turu_core-0.9.9/src/turu/core/mock/connection.py`

 * *Files identical despite different names*

### Comparing `turu_core-0.9.8/src/turu/core/mock/cursor.py` & `turu_core-0.9.9/src/turu/core/mock/cursor.py`

 * *Files identical despite different names*

### Comparing `turu_core-0.9.8/src/turu/core/mock/exception.py` & `turu_core-0.9.9/src/turu/core/mock/exception.py`

 * *Files identical despite different names*

### Comparing `turu_core-0.9.8/src/turu/core/mock/store.py` & `turu_core-0.9.9/src/turu/core/mock/store.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     TuruMockResponseTypeMismatchError,
     TuruMockStoreDataNotFoundError,
 )
 
 
 class TuruMockStore:
     def __init__(self):
-        self._data: List[Tuple[Optional[Type], Sequence | None | Exception]] = []
+        self._data: List[Tuple[Optional[Type], Union[Sequence, None, Exception]]] = []
         self._counter = 0
 
     @overload
     def inject_response(
         self,
         row_type: None,
         response: Union[GenericRowType, Sequence[GenericRowType], None, Exception],
@@ -33,15 +33,15 @@
             response = (response,)
 
         self._data.append((row_type, response))
 
     def provide_response(
         self,
         row_type: Optional[Type],
-    ) -> "Sequence[Any] | None":
+    ) -> "Optional[Sequence[Any]]":
         self._counter += 1
 
         if len(self._data) == 0:
             raise TuruMockStoreDataNotFoundError(self._counter)
 
         _row_type, _response = self._data.pop(0)
```

### Comparing `turu_core-0.9.8/src/turu/core/protocols/async_connection.py` & `turu_core-0.9.9/src/turu/core/protocols/async_connection.py`

 * *Files identical despite different names*

### Comparing `turu_core-0.9.8/src/turu/core/protocols/async_cursor.py` & `turu_core-0.9.9/src/turu/core/protocols/async_cursor.py`

 * *Files identical despite different names*

### Comparing `turu_core-0.9.8/src/turu/core/protocols/connection.py` & `turu_core-0.9.9/src/turu/core/protocols/connection.py`

 * *Files identical despite different names*

### Comparing `turu_core-0.9.8/src/turu/core/protocols/cursor.py` & `turu_core-0.9.9/src/turu/core/protocols/cursor.py`

 * *Files identical despite different names*

### Comparing `turu_core-0.9.8/src/turu/core/record/__init__.py` & `turu_core-0.9.9/src/turu/core/record/__init__.py`

 * *Files identical despite different names*

### Comparing `turu_core-0.9.8/src/turu/core/record/async_record_cursor.py` & `turu_core-0.9.9/src/turu/core/record/async_record_cursor.py`

 * *Files identical despite different names*

### Comparing `turu_core-0.9.8/src/turu/core/record/csv_recorder.py` & `turu_core-0.9.9/src/turu/core/record/csv_recorder.py`

 * *Files identical despite different names*

### Comparing `turu_core-0.9.8/src/turu/core/record/record_cursor.py` & `turu_core-0.9.9/src/turu/core/record/record_cursor.py`

 * *Files identical despite different names*

### Comparing `turu_core-0.9.8/PKG-INFO` & `turu_core-0.9.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turu-core
-Version: 0.9.8
+Version: 0.9.9
 Summary: 
 Home-page: https://github.com/yassun7010/turu-py
 Author: yassun7010
 Author-email: yassun7010@outlook.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

