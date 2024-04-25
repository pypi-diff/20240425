# Comparing `tmp/queue_kv-0.1.1.tar.gz` & `tmp/queue_kv-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "queue_kv-0.1.1.tar", last modified: Sun Apr 21 18:04:21 2024, max compression
+gzip compressed data, was "queue_kv-0.1.2.tar", last modified: Thu Apr 25 16:54:40 2024, max compression
```

## Comparing `queue_kv-0.1.1.tar` & `queue_kv-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 18:04:21.239884 queue_kv-0.1.1/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      591 2024-04-21 18:04:21.229884 queue_kv-0.1.1/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       69 2024-04-15 16:36:13.000000 queue_kv-0.1.1/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      637 2024-04-21 18:04:18.000000 queue_kv-0.1.1/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-21 18:04:21.239884 queue_kv-0.1.1/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 18:04:21.229884 queue_kv-0.1.1/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 18:04:21.229884 queue_kv-0.1.1/src/q/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 18:04:21.229884 queue_kv-0.1.1/src/q/kv/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      174 2024-04-21 18:02:59.000000 queue_kv-0.1.1/src/q/kv/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       98 2024-04-21 18:02:54.000000 queue_kv-0.1.1/src/q/kv/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2220 2024-04-21 17:49:03.000000 queue_kv-0.1.1/src/q/kv/api.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      898 2024-04-21 18:02:31.000000 queue_kv-0.1.1/src/q/kv/append.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 18:04:21.229884 queue_kv-0.1.1/src/queue_kv.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      591 2024-04-21 18:04:21.000000 queue_kv-0.1.1/src/queue_kv.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      281 2024-04-21 18:04:21.000000 queue_kv-0.1.1/src/queue_kv.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-21 18:04:21.000000 queue_kv-0.1.1/src/queue_kv.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       75 2024-04-21 18:04:21.000000 queue_kv-0.1.1/src/queue_kv.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        2 2024-04-21 18:04:21.000000 queue_kv-0.1.1/src/queue_kv.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 16:54:40.263055 queue_kv-0.1.2/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      596 2024-04-25 16:54:40.263055 queue_kv-0.1.2/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       69 2024-04-24 13:02:36.000000 queue_kv-0.1.2/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      642 2024-04-25 16:54:37.000000 queue_kv-0.1.2/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-25 16:54:40.263055 queue_kv-0.1.2/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 16:54:40.253055 queue_kv-0.1.2/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 16:54:40.253055 queue_kv-0.1.2/src/q/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 16:54:40.253055 queue_kv-0.1.2/src/q/kv/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      174 2024-04-24 13:02:36.000000 queue_kv-0.1.2/src/q/kv/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       98 2024-04-24 13:02:36.000000 queue_kv-0.1.2/src/q/kv/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2198 2024-04-25 16:50:10.000000 queue_kv-0.1.2/src/q/kv/api.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      877 2024-04-25 07:26:10.000000 queue_kv-0.1.2/src/q/kv/append.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 16:54:40.263055 queue_kv-0.1.2/src/queue_kv.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      596 2024-04-25 16:54:40.000000 queue_kv-0.1.2/src/queue_kv.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      281 2024-04-25 16:54:40.000000 queue_kv-0.1.2/src/queue_kv.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-25 16:54:40.000000 queue_kv-0.1.2/src/queue_kv.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       75 2024-04-25 16:54:40.000000 queue_kv-0.1.2/src/queue_kv.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        2 2024-04-25 16:54:40.000000 queue_kv-0.1.2/src/queue_kv.egg-info/top_level.txt
```

### Comparing `queue_kv-0.1.1/PKG-INFO` & `queue_kv-0.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: queue-kv
-Version: 0.1.1
+Version: 0.1.2
 Summary: Async Queue API implementation based on a Key-Value api
 Author-email: Marcel Claramunt <marcel@moveread.com>
-Project-URL: repo, https://github.com/moveread/python-kv.git
+Project-URL: repo, https://github.com/moveread/python-storage.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: queue-api
 Requires-Dist: kv-api
 Requires-Dist: pydantic
 Requires-Dist: lazy-loader
 Provides-Extra: fs
```

### Comparing `queue_kv-0.1.1/pyproject.toml` & `queue_kv-0.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "queue-kv"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Async Queue API implementation based on a Key-Value api"
 dependencies = [
   "queue-api", "kv-api", "pydantic", "lazy-loader"
 ]
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
 
 [project.urls]
-repo = "https://github.com/moveread/python-kv.git"
+repo = "https://github.com/moveread/python-storage.git"
 
 [project.optional-dependencies]
 fs = ["kv-fs"]
 sqlite = ["kv-sqlite-sync"]
 
 # test = [
 #   "pytest < 5.0.0",
```

### Comparing `queue_kv-0.1.1/src/q/kv/api.py` & `queue_kv-0.1.2/src/q/kv/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from typing import Generic, Literal, TypeVar, overload
+from typing_extensions import Generic, Literal, TypeVar, overload
 import asyncio
 from datetime import timedelta
-from haskellian import either as E, AsyncIter
+from haskellian import either as E, AsyncIter, iter as I
 from kv.api import KV
 from q.api import Queue
 
 A = TypeVar('A')
 B = TypeVar('B')
 
 class QueueKV(Queue[A], Generic[A]):
@@ -44,24 +44,22 @@
   
   @classmethod
   def at(cls, Type: type[B], path: str, protocol: Literal['fs', 'sqlite'], table: str = 'queue') -> 'QueueKV[B]':
     return QueueKV.fs(Type, path) if protocol == 'fs' else QueueKV.sqlite(Type, path, table)
 
 
   async def push(self, key: str, value: A):
-    return (await self._kv.insert(key, value, replace=True)).unsafe()
+    return (await self._kv.insert(key, value)).unsafe()
   
   async def _read(self, id: str | None = None, remove: bool = False) -> None | tuple[str, A]:
     if id is None:
-      head = await self._kv.keys().head()
-      if head is None:
+      key = I.head((await self._kv.keys()).unsafe())
+      if key is None:
         await asyncio.sleep(self.poll_interval.total_seconds())
         return await self._read(id, remove)
-      else:
-        key = head.unsafe()
     else:
       key = id
 
     value = (await self._kv.read(key)).unsafe()
     if remove:
       (await self._kv.delete(key)).unsafe()
     return key, value
```

### Comparing `queue_kv-0.1.1/src/q/kv/append.py` & `queue_kv-0.1.2/src/q/kv/append.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from typing import Generic, TypeVar
+from typing_extensions import Generic, TypeVar
 import haskellian.either as E
-from kv.api.append import AppendableKV
-from kv.api.errors import InexistentItem
+from kv.api import AppendableKV, InexistentItem
 from q.api import AppendableQueue
 from .api import QueueKV
 
 A = TypeVar('A')
 T = TypeVar('T')
 
 class AppendQueueKV(QueueKV[list[T]], AppendableQueue[T], Generic[T]):
```

### Comparing `queue_kv-0.1.1/src/queue_kv.egg-info/PKG-INFO` & `queue_kv-0.1.2/src/queue_kv.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: queue-kv
-Version: 0.1.1
+Version: 0.1.2
 Summary: Async Queue API implementation based on a Key-Value api
 Author-email: Marcel Claramunt <marcel@moveread.com>
-Project-URL: repo, https://github.com/moveread/python-kv.git
+Project-URL: repo, https://github.com/moveread/python-storage.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: queue-api
 Requires-Dist: kv-api
 Requires-Dist: pydantic
 Requires-Dist: lazy-loader
 Provides-Extra: fs
```

