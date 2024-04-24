# Comparing `tmp/milkcow-0.0.10.tar.gz` & `tmp/milkcow-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "milkcow-0.0.10.tar", last modified: Sun Apr 21 03:30:37 2024, max compression
+gzip compressed data, was "milkcow-0.0.11.tar", last modified: Wed Apr 24 23:11:53 2024, max compression
```

## Comparing `milkcow-0.0.10.tar` & `milkcow-0.0.11.tar`

### file list

```diff
@@ -1,30 +1,36 @@
-drwxr-xr-x   0 gabby     (1000) gabby     (1000)        0 2024-04-21 03:30:37.548737 milkcow-0.0.10/
--rw-r--r--   0 gabby     (1000) gabby     (1000)     1074 2024-04-18 22:17:11.000000 milkcow-0.0.10/LICENSE.txt
--rw-r--r--   0 gabby     (1000) gabby     (1000)     8327 2024-04-21 03:30:37.548737 milkcow-0.0.10/PKG-INFO
-drwxr-xr-x   0 gabby     (1000) gabby     (1000)        0 2024-04-21 03:30:37.545404 milkcow-0.0.10/milkcow/
--rw-r--r--   0 gabby     (1000) gabby     (1000)      117 2024-04-21 01:21:23.000000 milkcow-0.0.10/milkcow/__init__.py
-drwxr-xr-x   0 gabby     (1000) gabby     (1000)        0 2024-04-21 03:30:37.548737 milkcow-0.0.10/milkcow/common/
--rw-r--r--   0 gabby     (1000) gabby     (1000)        0 2024-04-21 01:21:23.000000 milkcow-0.0.10/milkcow/common/__init__.py
--rw-r--r--   0 gabby     (1000) gabby     (1000)     2731 2024-04-21 01:21:23.000000 milkcow-0.0.10/milkcow/common/basecacheddb.py
--rw-r--r--   0 gabby     (1000) gabby     (1000)     2410 2024-04-21 01:21:23.000000 milkcow-0.0.10/milkcow/common/basestore.py
--rw-r--r--   0 gabby     (1000) gabby     (1000)      966 2024-04-21 01:21:23.000000 milkcow-0.0.10/milkcow/common/transcode.py
-drwxr-xr-x   0 gabby     (1000) gabby     (1000)        0 2024-04-21 03:30:37.548737 milkcow-0.0.10/milkcow/core/
--rw-r--r--   0 gabby     (1000) gabby     (1000)        1 2024-04-21 01:21:23.000000 milkcow-0.0.10/milkcow/core/__init__.py
--rw-r--r--   0 gabby     (1000) gabby     (1000)     3329 2024-04-21 02:24:00.000000 milkcow-0.0.10/milkcow/core/basebufferedsocket.py
--rw-r--r--   0 gabby     (1000) gabby     (1000)     1863 2024-04-21 01:57:48.000000 milkcow-0.0.10/milkcow/core/classes.py
--rw-r--r--   0 gabby     (1000) gabby     (1000)     4069 2024-04-21 01:21:23.000000 milkcow-0.0.10/milkcow/core/connections.py
--rw-r--r--   0 gabby     (1000) gabby     (1000)      125 2024-04-21 01:21:23.000000 milkcow-0.0.10/milkcow/main.py
-drwxr-xr-x   0 gabby     (1000) gabby     (1000)        0 2024-04-21 03:30:37.548737 milkcow-0.0.10/milkcow/test/
--rw-r--r--   0 gabby     (1000) gabby     (1000)       68 2024-04-21 01:21:23.000000 milkcow-0.0.10/milkcow/test/__init__.py
-drwxr-xr-x   0 gabby     (1000) gabby     (1000)        0 2024-04-21 03:30:37.548737 milkcow-0.0.10/milkcow/test/example/
--rw-r--r--   0 gabby     (1000) gabby     (1000)        0 2024-04-21 01:21:23.000000 milkcow-0.0.10/milkcow/test/example/__init__.py
--rw-r--r--   0 gabby     (1000) gabby     (1000)      327 2024-04-21 01:21:23.000000 milkcow-0.0.10/milkcow/test/example/ex1.py
--rw-r--r--   0 gabby     (1000) gabby     (1000)      429 2024-04-21 01:21:23.000000 milkcow-0.0.10/milkcow/test/example/ex2.py
--rw-r--r--   0 gabby     (1000) gabby     (1000)      362 2024-04-21 01:21:23.000000 milkcow-0.0.10/milkcow/test/example/my_model_class.py
-drwxr-xr-x   0 gabby     (1000) gabby     (1000)        0 2024-04-21 03:30:37.548737 milkcow-0.0.10/milkcow.egg-info/
--rw-r--r--   0 gabby     (1000) gabby     (1000)     8327 2024-04-21 03:30:37.000000 milkcow-0.0.10/milkcow.egg-info/PKG-INFO
--rw-r--r--   0 gabby     (1000) gabby     (1000)      559 2024-04-21 03:30:37.000000 milkcow-0.0.10/milkcow.egg-info/SOURCES.txt
--rw-r--r--   0 gabby     (1000) gabby     (1000)        1 2024-04-21 03:30:37.000000 milkcow-0.0.10/milkcow.egg-info/dependency_links.txt
--rw-r--r--   0 gabby     (1000) gabby     (1000)        8 2024-04-21 03:30:37.000000 milkcow-0.0.10/milkcow.egg-info/top_level.txt
--rw-r--r--   0 gabby     (1000) gabby     (1000)       38 2024-04-21 03:30:37.548737 milkcow-0.0.10/setup.cfg
--rw-r--r--   0 gabby     (1000) gabby     (1000)      803 2024-04-21 03:30:33.000000 milkcow-0.0.10/setup.py
+drwxr-xr-x   0 gabby     (1000) gabby     (1000)        0 2024-04-24 23:11:53.176182 milkcow-0.0.11/
+-rw-r--r--   0 gabby     (1000) gabby     (1000)     1074 2024-04-18 22:17:11.000000 milkcow-0.0.11/LICENSE.txt
+-rw-r--r--   0 gabby     (1000) gabby     (1000)     5321 2024-04-24 23:11:53.176182 milkcow-0.0.11/PKG-INFO
+drwxr-xr-x   0 gabby     (1000) gabby     (1000)        0 2024-04-24 23:11:53.172849 milkcow-0.0.11/milkcow/
+-rw-r--r--   0 gabby     (1000) gabby     (1000)      168 2024-04-24 22:37:08.000000 milkcow-0.0.11/milkcow/__init__.py
+drwxr-xr-x   0 gabby     (1000) gabby     (1000)        0 2024-04-24 23:11:53.172849 milkcow-0.0.11/milkcow/common/
+-rw-r--r--   0 gabby     (1000) gabby     (1000)        0 2024-04-21 21:20:50.000000 milkcow-0.0.11/milkcow/common/__init__.py
+-rw-r--r--   0 gabby     (1000) gabby     (1000)     3240 2024-04-24 22:37:26.000000 milkcow-0.0.11/milkcow/common/basebufferedsocket.py
+-rw-r--r--   0 gabby     (1000) gabby     (1000)     3901 2024-04-24 22:37:26.000000 milkcow-0.0.11/milkcow/common/basedb.py
+-rw-r--r--   0 gabby     (1000) gabby     (1000)     3174 2024-04-24 22:37:26.000000 milkcow-0.0.11/milkcow/common/basestore.py
+drwxr-xr-x   0 gabby     (1000) gabby     (1000)        0 2024-04-24 23:11:53.172849 milkcow-0.0.11/milkcow/core/
+-rw-r--r--   0 gabby     (1000) gabby     (1000)      230 2024-04-24 22:34:05.000000 milkcow-0.0.11/milkcow/core/__init__.py
+-rw-r--r--   0 gabby     (1000) gabby     (1000)     3764 2024-04-24 22:37:08.000000 milkcow-0.0.11/milkcow/core/connections.py
+drwxr-xr-x   0 gabby     (1000) gabby     (1000)        0 2024-04-24 23:11:53.176182 milkcow-0.0.11/milkcow/core/milkcat/
+-rw-r--r--   0 gabby     (1000) gabby     (1000)       60 2024-04-24 22:34:05.000000 milkcow-0.0.11/milkcow/core/milkcat/__init__.py
+-rw-r--r--   0 gabby     (1000) gabby     (1000)     1943 2024-04-24 22:37:08.000000 milkcow-0.0.11/milkcow/core/milkcat/milkcat.py
+-rw-r--r--   0 gabby     (1000) gabby     (1000)     3973 2024-04-24 22:37:26.000000 milkcow-0.0.11/milkcow/core/senders.py
+drwxr-xr-x   0 gabby     (1000) gabby     (1000)        0 2024-04-24 23:11:53.176182 milkcow-0.0.11/milkcow/test/
+-rw-r--r--   0 gabby     (1000) gabby     (1000)        0 2024-04-21 21:20:50.000000 milkcow-0.0.11/milkcow/test/__init__.py
+drwxr-xr-x   0 gabby     (1000) gabby     (1000)        0 2024-04-24 23:11:53.176182 milkcow-0.0.11/milkcow/test/example/
+-rw-r--r--   0 gabby     (1000) gabby     (1000)      108 2024-04-24 22:34:05.000000 milkcow-0.0.11/milkcow/test/example/__init__.py
+-rw-r--r--   0 gabby     (1000) gabby     (1000)      383 2024-04-24 22:37:08.000000 milkcow-0.0.11/milkcow/test/example/jc_ex.py
+-rw-r--r--   0 gabby     (1000) gabby     (1000)      919 2024-04-24 22:37:08.000000 milkcow-0.0.11/milkcow/test/example/mc_ex.py
+-rw-r--r--   0 gabby     (1000) gabby     (1000)      362 2024-04-24 20:13:04.000000 milkcow-0.0.11/milkcow/test/example/my_model_class.py
+-rw-r--r--   0 gabby     (1000) gabby     (1000)      312 2024-04-24 22:34:05.000000 milkcow-0.0.11/milkcow/test/example/oc_ex.py
+drwxr-xr-x   0 gabby     (1000) gabby     (1000)        0 2024-04-24 23:11:53.176182 milkcow-0.0.11/milkcow/util/
+-rw-r--r--   0 gabby     (1000) gabby     (1000)        0 2024-04-24 23:05:44.000000 milkcow-0.0.11/milkcow/util/__init__.py
+-rw-r--r--   0 gabby     (1000) gabby     (1000)     1998 2024-04-24 22:37:08.000000 milkcow-0.0.11/milkcow/util/cli.py
+drwxr-xr-x   0 gabby     (1000) gabby     (1000)        0 2024-04-24 23:11:53.176182 milkcow-0.0.11/milkcow.egg-info/
+-rw-r--r--   0 gabby     (1000) gabby     (1000)     5321 2024-04-24 23:11:53.000000 milkcow-0.0.11/milkcow.egg-info/PKG-INFO
+-rw-r--r--   0 gabby     (1000) gabby     (1000)      689 2024-04-24 23:11:53.000000 milkcow-0.0.11/milkcow.egg-info/SOURCES.txt
+-rw-r--r--   0 gabby     (1000) gabby     (1000)        1 2024-04-24 23:11:53.000000 milkcow-0.0.11/milkcow.egg-info/dependency_links.txt
+-rw-r--r--   0 gabby     (1000) gabby     (1000)       53 2024-04-24 23:11:53.000000 milkcow-0.0.11/milkcow.egg-info/entry_points.txt
+-rw-r--r--   0 gabby     (1000) gabby     (1000)        8 2024-04-24 23:11:53.000000 milkcow-0.0.11/milkcow.egg-info/top_level.txt
+-rw-r--r--   0 gabby     (1000) gabby     (1000)       38 2024-04-24 23:11:53.176182 milkcow-0.0.11/setup.cfg
+-rw-r--r--   0 gabby     (1000) gabby     (1000)      891 2024-04-24 23:06:52.000000 milkcow-0.0.11/setup.py
```

### Comparing `milkcow-0.0.10/LICENSE.txt` & `milkcow-0.0.11/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `milkcow-0.0.10/milkcow/core/connections.py` & `milkcow-0.0.11/milkcow/common/basedb.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,133 +1,124 @@
+from collections.abc import KeysView
+from typing import ItemsView, Optional
 import sqlite3
-from typing import Optional
 
-from milkcow.common.basecacheddb import BaseCachedDB
 from milkcow.common.basestore import BaseStore
-from milkcow.common.transcode import BlobStore, ObjectStore
 
 
-class BaseDB(BaseCachedDB):
-    def _connect(self):
-        '''Create database connection'''
-        self._conn = sqlite3.connect('mc.db')
-
-    def _prep_values_for_db(self, values: list) -> None:
-        '''In-place operation on values list. Returns None'''
-        del values
-        raise NotImplementedError
-
-    def _create_table(self, key: str):
-        '''Create a database with key'''
-        if key not in self._store.keys():
-            sql = f'''CREATE TABLE IF NOT EXISTS {key} (data TEXT NOT NULL)'''
-            self._conn.execute(sql)
+class BaseDB:
+    '''Interact with database and bytes datastore'''
 
     def _push_by_key(self, cur, key, value) -> None:
         '''Create sql statement and executes on passed cursor'''
         assert type(value) is str, value
         sql = f'''INSERT INTO {key} VALUES (?)'''
         cur.execute(sql, [value])
 
-    def _pull_by_key(self, key: str):
+    def _pull_by_key(self, key: str) -> list:
         '''Pull from database and return iterable'''
         assert type(key) is str
         sql = f'''SELECT * FROM {key}'''
         try:
             cur = self._conn.execute(sql)
             items = [value[0] for value in cur.fetchall()]
             return items
         except sqlite3.OperationalError as e:
             print(e)
         return []
 
+    def _create_table(self, key: str) -> None:
+        '''Create a database with key'''
+        sql = f'''CREATE TABLE IF NOT EXISTS {key} (data TEXT NOT NULL)'''
+        try:
+            self._conn.execute(sql)
+        except AttributeError as e:
+            raise e
+
     def _drop_by_key(self, key: str) -> None:
         '''Drop table by key'''
         sql = f'''DROP TABLE {key};'''
         self._conn.execute(sql)
 
+    def _push_values(self, key, values) -> None:
+        '''Call _push_by_key over iterable. Does not call _prep_values'''
+        assert self._conn is not None
+        cur = self._conn.cursor()
+        for value in values:
+            self._push_by_key(cur, key, value)
+        self._conn.commit()
+
     def connect(self, path: Optional[str] = None):
         '''Create database connection'''
         if path is None:
-            self._connect()
+            self._conn = sqlite3.connect('mc.db')
         else:
             self._conn = sqlite3.connect(path)
 
 
-class Db0(BaseDB):
-    ''' object -> str -> db
-                      -> byes -> store'''
-
-    def __init__(self, classmodel) -> None:
-        _store = BlobStore(classmodel)  # BlobStore string -> bytes'''
-        super().__init__(_store)
-
-    def _prep_values_for_db(self, values: list) -> None:
-        '''Take list of objects and return list of string'''
-        for i, obj in enumerate(values):
-            try:
-                values[i] = obj.model_dump_json()
-            except Exception as e:
-                try:
-                    values[i] = obj.dump()
-                except Exception:
-                    raise e
-
-
-class Db1(BaseDB):
-    ''' object -> str -> db
-               -> store'''
-
-    def __init__(self, classmodel) -> None:
-        self.classmodel = classmodel
-        _store = BaseStore()  # BaseStore does not transcode'''
-        super().__init__(_store)
-
-    def _prep_values_for_db(self, values: list) -> None:
-        '''Take list of objects and return list of string'''
-        for i, obj in enumerate(values):
-            assert isinstance(obj, self.classmodel)
-            values[i] = obj.model_dump_json()
-
-
-class Db2(BaseDB):
-    ''' str -> db
-            -> byes -> store'''
-
-    def __init__(self, classmodel) -> None:
-        _store = BlobStore(classmodel)  # BlobStore string -> bytes'''
-        super().__init__(_store)
-
-    def _prep_values_for_db(self, values: list) -> None:
-        '''bypass'''
-        x = len(values)
-        del x
-
-
-class Db3(BaseDB):
-    ''' str -> db
-            -> obj -> store'''
-
-    def __init__(self, classmodel) -> None:
-        _store = ObjectStore(classmodel)  # ObjectStore string -> objects
-        super().__init__(_store)
-
-    def _prep_values_for_db(self, values: list) -> None:
-        '''bypass do nothing'''
-        x = len(values)
-        del x
-
-
-class Db4(BaseDB):
-    ''' byets -> str -> db
-                     -> obj -> store'''
-    pass
-
-    def __init__(self, classmodel) -> None:
-        _store = ObjectStore(classmodel)  # ObjectStore string -> objects
-        super().__init__(_store)
-
-    def _prep_values_for_db(self, values: list) -> None:
-        '''Take list of bytes and do in place decode to string'''
-        for i, value in enumerate(values):
-            assert type(value) is bytes
-            values[i] = value.decode()
+class CachedDb(BaseDB):
+    def __init__(self) -> None:
+        super().__init__()
+        self._new_map: dict = {}
+        self._cache: BaseStore = BaseStore()
+
+    def _add_to_cache(self, key: str, values: list) -> None:
+        '''Add to cache'''
+        self._cache.extend(key, values)
+
+    def _push_values_and_cache(self, key: str, values: list) -> None:
+        '''Push values and add to cache'''
+        self._push_values(key, values)
+        self._add_to_cache(key, values)
+
+    def _pull_values_and_cache(self, key: str) -> list:
+        '''Pull values and cache if there are any'''
+        return self._pull_by_key(key)
+
+    def new(self, key: str) -> list:
+        '''Return a list of new values added since the last call'''
+        return self._cache.new(key)
+
+    def new_values(self) -> dict:
+        '''Return dict of new values for all items'''
+        return self._cache.new_values()
+
+    def push(self, key: str, values: list) -> None:
+        '''Push list of values to the database'''
+        if key not in self._cache.keys():
+            self._new_map[key] = 0
+            self._create_table(key)
+            self._pull_by_key(key)
+        self._push_values_and_cache(key, values)
+
+    def pull(self, key: str) -> list:
+        '''Pull key from database'''
+        return self._pull_values_and_cache(key)
+
+    def drop(self, key: str) -> None:
+        '''Drop form database'''
+        self._drop_by_key(key)
+        self._cache.drop(key)
+
+    def keys(self) -> KeysView:
+        '''Return keys for items pulled or pushed'''
+        return self._cache.keys()
+
+    def items(self) -> ItemsView:
+        '''Return items pulled or pushed'''
+        return self._cache.items()
+
+
+class TranscodedDb(CachedDb):
+    def _add_to_cache(self, key: str, values: list) -> None:
+        del key
+        del values
+        raise NotImplementedError
+
+    def _push_values_and_cache(self, key: str, values: list) -> None:
+        del key
+        del values
+        raise NotImplementedError
+
+    def _pull_values_and_cache(self, key: str) -> list:
+        del key
+        raise NotImplementedError
```

### Comparing `milkcow-0.0.10/milkcow.egg-info/SOURCES.txt` & `milkcow-0.0.11/milkcow.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 LICENSE.txt
 setup.py
 milkcow/__init__.py
-milkcow/main.py
 milkcow.egg-info/PKG-INFO
 milkcow.egg-info/SOURCES.txt
 milkcow.egg-info/dependency_links.txt
+milkcow.egg-info/entry_points.txt
 milkcow.egg-info/top_level.txt
 milkcow/common/__init__.py
-milkcow/common/basecacheddb.py
+milkcow/common/basebufferedsocket.py
+milkcow/common/basedb.py
 milkcow/common/basestore.py
-milkcow/common/transcode.py
 milkcow/core/__init__.py
-milkcow/core/basebufferedsocket.py
-milkcow/core/classes.py
 milkcow/core/connections.py
+milkcow/core/senders.py
+milkcow/core/milkcat/__init__.py
+milkcow/core/milkcat/milkcat.py
 milkcow/test/__init__.py
 milkcow/test/example/__init__.py
-milkcow/test/example/ex1.py
-milkcow/test/example/ex2.py
-milkcow/test/example/my_model_class.py
+milkcow/test/example/jc_ex.py
+milkcow/test/example/mc_ex.py
+milkcow/test/example/my_model_class.py
+milkcow/test/example/oc_ex.py
+milkcow/util/__init__.py
+milkcow/util/cli.py
```

### Comparing `milkcow-0.0.10/setup.py` & `milkcow-0.0.11/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,17 +2,20 @@
 
 
 with open('milkcow/README.md', 'r') as f:
     long_description = f.read()
 
 
 setup(
+        entry_points={
+            'console_scripts': ['milkcow=milkcow.util.cli:run_cli']
+            },
         name='milkcow',
-        version='0.0.10',
-        description='A tool to building middleware for the multiprocessing of data',
+        version='0.0.11',
+        description='A library pulling json into python projects',
         packages=find_packages(),
         long_description=long_description,
         long_description_content_type='text/markdown',
         url='https://github.com/SamReynoso/milkcow',
         author='SamReynoso',
         license='MIT',
         classifiers=[
```

