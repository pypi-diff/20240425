# Comparing `tmp/kv_sqlite_sync-0.1.7.tar.gz` & `tmp/kv_sqlite_sync-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kv_sqlite_sync-0.1.7.tar", last modified: Wed Apr 24 13:42:39 2024, max compression
+gzip compressed data, was "kv_sqlite_sync-0.1.8.tar", last modified: Thu Apr 25 05:12:27 2024, max compression
```

## Comparing `kv_sqlite_sync-0.1.7.tar` & `kv_sqlite_sync-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-24 13:42:39.953952 kv_sqlite_sync-0.1.7/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      894 2024-04-24 13:42:39.953952 kv_sqlite_sync-0.1.7/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      401 2024-04-24 13:02:36.000000 kv_sqlite_sync-0.1.7/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      695 2024-04-24 13:42:37.000000 kv_sqlite_sync-0.1.7/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-24 13:42:39.953952 kv_sqlite_sync-0.1.7/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-24 13:42:39.953952 kv_sqlite_sync-0.1.7/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-24 13:42:39.953952 kv_sqlite_sync-0.1.7/src/kv/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-24 13:42:39.953952 kv_sqlite_sync-0.1.7/src/kv/sqlite/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-24 13:32:50.000000 kv_sqlite_sync-0.1.7/src/kv/sqlite/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      203 2024-04-24 13:32:38.000000 kv_sqlite_sync-0.1.7/src/kv/sqlite/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3669 2024-04-24 13:41:44.000000 kv_sqlite_sync-0.1.7/src/kv/sqlite/api.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1631 2024-04-24 13:37:20.000000 kv_sqlite_sync-0.1.7/src/kv/sqlite/queries.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-24 13:42:39.953952 kv_sqlite_sync-0.1.7/src/kv_sqlite_sync.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      894 2024-04-24 13:42:39.000000 kv_sqlite_sync-0.1.7/src/kv_sqlite_sync.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      332 2024-04-24 13:42:39.000000 kv_sqlite_sync-0.1.7/src/kv_sqlite_sync.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-24 13:42:39.000000 kv_sqlite_sync-0.1.7/src/kv_sqlite_sync.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       30 2024-04-24 13:42:39.000000 kv_sqlite_sync-0.1.7/src/kv_sqlite_sync.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-24 13:42:39.000000 kv_sqlite_sync-0.1.7/src/kv_sqlite_sync.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 05:12:27.044239 kv_sqlite_sync-0.1.8/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      894 2024-04-25 05:12:27.044239 kv_sqlite_sync-0.1.8/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      401 2024-04-24 13:02:36.000000 kv_sqlite_sync-0.1.8/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      695 2024-04-25 05:12:24.000000 kv_sqlite_sync-0.1.8/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-25 05:12:27.044239 kv_sqlite_sync-0.1.8/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 05:12:27.044239 kv_sqlite_sync-0.1.8/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 05:12:27.044239 kv_sqlite_sync-0.1.8/src/kv/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 05:12:27.044239 kv_sqlite_sync-0.1.8/src/kv/sqlite/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-24 13:32:50.000000 kv_sqlite_sync-0.1.8/src/kv/sqlite/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      203 2024-04-24 13:32:38.000000 kv_sqlite_sync-0.1.8/src/kv/sqlite/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3480 2024-04-25 05:10:08.000000 kv_sqlite_sync-0.1.8/src/kv/sqlite/api.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1631 2024-04-24 13:37:20.000000 kv_sqlite_sync-0.1.8/src/kv/sqlite/queries.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 05:12:27.044239 kv_sqlite_sync-0.1.8/src/kv_sqlite_sync.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      894 2024-04-25 05:12:27.000000 kv_sqlite_sync-0.1.8/src/kv_sqlite_sync.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      332 2024-04-25 05:12:27.000000 kv_sqlite_sync-0.1.8/src/kv_sqlite_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-25 05:12:27.000000 kv_sqlite_sync-0.1.8/src/kv_sqlite_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       30 2024-04-25 05:12:27.000000 kv_sqlite_sync-0.1.8/src/kv_sqlite_sync.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-25 05:12:27.000000 kv_sqlite_sync-0.1.8/src/kv_sqlite_sync.egg-info/top_level.txt
```

### Comparing `kv_sqlite_sync-0.1.7/PKG-INFO` & `kv_sqlite_sync-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kv-sqlite-sync
-Version: 0.1.7
+Version: 0.1.8
 Summary: Key-Value interface over SQLite. Supports any datatype, including JSON and BLOB
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/python-storage
 Project-URL: home, https://github.com/moveread/python-storage/tree/main/kv/kv-sqlite-sync
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: kv-api
```

### Comparing `kv_sqlite_sync-0.1.7/pyproject.toml` & `kv_sqlite_sync-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kv-sqlite-sync"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Key-Value interface over SQLite. Supports any datatype, including JSON and BLOB"
 dependencies = [
   "kv-api", "haskellian", "lazy-loader"
 ]
```

### Comparing `kv_sqlite_sync-0.1.7/src/kv/sqlite/api.py` & `kv_sqlite_sync-0.1.8/src/kv/sqlite/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from typing import AsyncIterable, TypeVar, Generic, Callable, cast
+from typing import AsyncIterable, TypeVar, Generic, Callable, cast, Sequence
 from dataclasses import dataclass
 from haskellian import either as E, promise as P, asyn_iter as AI
 from pydantic import RootModel
-from kv.api import KV
-from kv.api.errors import InexistentItem, DBError, InvalidData
+from kv.api import KV, InexistentItem, DBError, InvalidData
 import sqlite3
 import os
 from . import queries
 
 T = TypeVar('T')
 M = TypeVar('M')
 
@@ -79,23 +78,19 @@
 
   @P.lift
   async def delete(self, key: str) -> E.Either[DBError | InexistentItem, None]:
     return self.execute(queries.delete(key, table=self.table)).bind(
       lambda cur: E.Left(InexistentItem(key)) if cur.rowcount == 0 else E.Right(None)
     )
   
-  @AI.lift
-  async def keys(self, batch_size: int | None = None) -> AsyncIterable[E.Either[DBError, str]]:
-    match self.execute(queries.keys(self.table)):
-      case E.Right(cur):
-        while (batch := cur.fetchmany(batch_size or 256)) != []:
-          for [key] in batch:
-            yield E.Right(key)
-      case E.Left(err):
-        yield E.Left(err)
+  @P.lift
+  async def keys(self) -> E.Either[DBError, Sequence[str]]:
+    return self.execute(queries.keys(self.table)).fmap(
+      lambda cur: [key for [key] in cur.fetchall()]
+    )
 
   @AI.lift
   async def items(self, batch_size: int | None = None) -> AsyncIterable[E.Either[DBError | InvalidData, tuple[str, T]]]:
     match self.execute(queries.items(self.table)):
       case E.Right(cur):
         while (batch := cur.fetchmany(batch_size or 256)) != []:
           for k, v in batch:
```

### Comparing `kv_sqlite_sync-0.1.7/src/kv/sqlite/queries.py` & `kv_sqlite_sync-0.1.8/src/kv/sqlite/queries.py`

 * *Files identical despite different names*

### Comparing `kv_sqlite_sync-0.1.7/src/kv_sqlite_sync.egg-info/PKG-INFO` & `kv_sqlite_sync-0.1.8/src/kv_sqlite_sync.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kv-sqlite-sync
-Version: 0.1.7
+Version: 0.1.8
 Summary: Key-Value interface over SQLite. Supports any datatype, including JSON and BLOB
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/python-storage
 Project-URL: home, https://github.com/moveread/python-storage/tree/main/kv/kv-sqlite-sync
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: kv-api
```

