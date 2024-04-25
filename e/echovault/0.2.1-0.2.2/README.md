# Comparing `tmp/echovault-0.2.1.tar.gz` & `tmp/echovault-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echovault-0.2.1.tar", max compression
+gzip compressed data, was "echovault-0.2.2.tar", max compression
```

## Comparing `echovault-0.2.1.tar` & `echovault-0.2.2.tar`

### file list

```diff
@@ -1,10 +1,15 @@
--rw-r--r--   0        0        0     1075 2024-04-19 19:04:53.372948 echovault-0.2.1/README.md
--rw-r--r--   0        0        0        0 2024-04-14 05:54:15.655547 echovault-0.2.1/echovault/__init__.py
--rw-r--r--   0        0        0      472 2024-04-11 19:33:04.149986 echovault-0.2.1/echovault/db.py
--rw-r--r--   0        0        0        0 2024-04-11 19:04:01.114880 echovault-0.2.1/echovault/db.py~
--rw-r--r--   0        0        0     3884 2024-04-19 19:14:39.971313 echovault-0.2.1/echovault/table.py
--rw-r--r--   0        0        0     2903 2024-04-14 19:48:17.176500 echovault-0.2.1/echovault/table.py~
--rw-r--r--   0        0        0     3519 2024-04-20 19:07:08.353727 echovault-0.2.1/echovault/vault.py
--rw-r--r--   0        0        0     1289 2024-04-14 19:18:41.190124 echovault-0.2.1/echovault/vault.py~
--rw-r--r--   0        0        0      380 2024-04-21 19:41:43.512483 echovault-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1492 1970-01-01 00:00:00.000000 echovault-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-04-19 19:04:53.372948 echovault-0.2.2/README.md
+-rw-r--r--   0        0        0       34 2024-04-25 18:14:25.800920 echovault-0.2.2/echovault/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-14 05:54:15.655547 echovault-0.2.2/echovault/__init__.py~
+-rw-r--r--   0        0        0     1028 2024-04-25 04:59:27.197132 echovault-0.2.2/echovault/_container.py
+-rw-r--r--   0        0        0     1030 2024-04-24 19:49:03.244111 echovault-0.2.2/echovault/_container.py~
+-rw-r--r--   0        0        0        0 2024-04-11 19:04:01.114880 echovault-0.2.2/echovault/db.py~
+-rw-r--r--   0        0        0     1782 2024-04-24 19:17:52.808075 echovault-0.2.2/echovault/dict.py
+-rw-r--r--   0        0        0     2283 2024-04-23 18:43:20.644733 echovault-0.2.2/echovault/dict.py~
+-rw-r--r--   0        0        0     1217 2024-04-25 05:01:58.009942 echovault-0.2.2/echovault/list.py
+-rw-r--r--   0        0        0     1176 2024-04-24 19:49:34.034385 echovault-0.2.2/echovault/list.py~
+-rw-r--r--   0        0        0     2903 2024-04-14 19:48:17.176500 echovault-0.2.2/echovault/table.py~
+-rw-r--r--   0        0        0     3621 2024-04-25 18:06:26.997077 echovault-0.2.2/echovault/vault.py
+-rw-r--r--   0        0        0     1289 2024-04-14 19:18:41.190124 echovault-0.2.2/echovault/vault.py~
+-rw-r--r--   0        0        0      380 2024-04-25 18:13:49.510631 echovault-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1492 1970-01-01 00:00:00.000000 echovault-0.2.2/PKG-INFO
```

### Comparing `echovault-0.2.1/README.md` & `echovault-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `echovault-0.2.1/echovault/table.py` & `echovault-0.2.2/echovault/vault.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,146 +1,127 @@
-from dulwich.objects import Tree, Blob
-from pickle import dumps, loads
+from dulwich.objects import Tree, Commit
+from echovault.list import List
 from base64 import b64decode, b64encode
-from stat import S_IFREG, S_IFDIR
-from uuid import uuid4
+from socket import getfqdn, gethostname
+from os import getpid, getlogin, name as operating_system_name
+from sys import argv
+from typing import Optional
+from time import time
+from stat import S_IFDIR
+from echovault._container import Container
+
+try:
+    from os import getuid, getgid
+except:
+    def getuid():
+        return None
 
-class Entry:
-    @staticmethod
-    def encode(value):
-        return b64encode(dumps(value))
+    def getgid():
+        return None
+    
 
+class Vault(Container):
+    @staticmethod
+    def encode(string):
+        return string.encode('utf-8')
 
     @staticmethod
     def decode(value):
-        return loads(b64decode(value))
+        return value.decode('utf-8')
     
-    def __init__(self, object_store, table, identifier, items=(), *, tree=None):
-        self.object_store = object_store
-        self.table = table
-        self.identifier = identifier
-        
-        if tree is None:
-            tree = Tree()
-
-        self.tree = tree
-        
-        for key, value in (items.items()
-                           if isinstance(items, dict)
-                           else items):
-            self[key] = value
+    def __init__(self, object_store, refs, *, tree:Tree=None, ref=None):
+        self.refs = refs
 
-        if not b'_' in self.tree:
-            blob = Blob()
-            
-            if not blob.id in self.object_store:
-                self.object_store.add_object(blob)
+        if ref is not None:
+            ref = b'refs/heads/' + ref.encode('utf-8')
             
-            self.tree[b'_'] = S_IFREG | 0o755, blob.id
-
-        self._update()
-
-    def _update(self):
-        if not self.tree.id in self.object_store:
-            self.object_store.add_object(self.tree)
+            if ref in self.refs and tree is None:
+                tree = self.object_store[self.object_store[self.refs[ref]].tree]
+        
+        self.ref = ref
 
-        self.table.tree[self.identifier] = S_IFDIR, self.tree.id
-            
-        self.table._update()
+        super().__init__(object_store, None, None, tree)
 
-    def __getitem__(self, key):
-        _, id_ = self.tree[self.encode(key)]
-        return loads(self.object_store[id_].data)
-
-    def __setitem__(self, key, value):
-        blob = Blob()
-        blob.data = dumps(value)
-        
-        if not blob.id in self.object_store:
-            self.object_store.add_object(blob)
-            
-        self.tree[self.encode(key)] = S_IFREG | 0o755, blob.id
+    def __getitem__(self, name:str):
+        identifier = self.encode(name)
+        _, oid = self.tree[identifier]
+        tree = self.object_store[oid]
+        return List(self.object_store,
+                     self,
+                     identifier,
+                     tree=tree)
 
+    def __setitem__(self, name:str, iterable):
+        identifier = self.encode(name)
+        self.tree[identifier] = S_IFDIR, None
+        table = List(self.object_store, self, identifier, iterable)
         self._update()
 
-    def __delitem__(self, key):
-        del self.tree[self.encode(key)]
-        
+    def __delitem__(self, name:str):
+        del self.tree[self.encode(name)]
         self._update()
-            
+
     def __iter__(self):
         return (self.decode(raw_key)
                 for raw_key
-                in iter(self.tree)
-                if raw_key != b'_')
-
-    def keys(self):
-        yield from iter(self)
+                in iter(self.tree))
 
-    def items(self):
-        for key in self.keys():
-            yield (key, self[key])
-
-    def values(self):
-        for _, value in self.items():
-            yield value
-
-    def __repr__(self):
-        return repr(dict(self.items()))
+    def rollback(self):
+        if self.ref is None:
+            self.tree = Tree()
+        else:
+            self.tree = self.object_store[self.object_store[self.refs[ref]].tree]
+    
+    def commit(self,
+               ref:Optional[str]=None,
+               message:Optional[str]='',
+               author:Optional[str]=None,
+               committer:Optional[str]=None,
+               time_:Optional[int]=None,
+               timezone:Optional[int]=None,
+               ):
+        if ref is None:
+            ref = self.ref
+        else:
+            ref = b'refs/heads/' + ref.encode('utf-8')
+            
+        commit = Commit()
+        
+        commit.message = message.encode('utf-8')
+        commit.tree = self.tree
+
+        if committer is None:
+            committer = ('_'.join((getfqdn(), gethostname(),
+                                   operating_system_name,
+                                   repr(getgid()),
+                                   repr(getuid()), repr(getpid())))
+                         + ': '
+                         + ' '.join(argv))
+            
+        if author is None:
+            author = getlogin()
+
+        commit.committer = committer.encode('utf-8')
+        commit.author = author.encode('utf-8')
+
+        if time_ is None:
+            time_ = int(time())
+
+        if timezone is None:
+            timezone = 0
+
+        commit.commit_time = time_
+        commit.commit_timezone = timezone
+        commit.author_time = time_
+        commit.author_timezone = timezone
+
+        try:
+            parents = (self.refs[ref],)
+        except:
+            parents = ()
             
-class Table:
-    def __init__(self, object_store, vault, identifier, values=(), *, tree=None):
-        self.object_store = object_store
-        self.vault = vault
-        self.identifier = identifier
+        commit.parents = parents
         
-        if tree is None:
-            tree = Tree()
+        if not commit.id in self.object_store:
+            self.object_store.add_object(commit)
 
-        self.tree = tree
-        self.extend(values)
-
-
-        if not b'_' in self.tree:
-            blob = Blob()
-            
-            if not blob.id in self.object_store:
-                self.object_store.add_object(blob)
-            
-            self.tree[b'_'] = S_IFREG | 0o755, blob.id
-
-        self._update()
-
-    def _update(self):
-        if not self.tree.id in self.object_store:
-            self.object_store.add_object(self.tree)
-
-        self.vault._tree[self.identifier] = S_IFDIR, self.tree.id
-            
-        self.vault._update()
-            
-    def __iter__(self):
-        for key in self.tree:
-            if key == b'_':
-                continue
-            
-            _, id_ = self.tree[key]
-            yield Entry(self.object_store,
-                        self,
-                        key,
-                        tree=self.object_store[id_])
-            
-
-    def extend(self, iterable):
-        for item in iterable:
-            entry = Entry(self.object_store,
-                          self,
-                          str(uuid4()).encode('utf-8'),
-                          item)
-            self.tree[entry.identifier] = S_IFDIR, entry.tree.id
-
-        self._update()
-            
-    def remove(self, entry):
-        del self.tree[entry.identifier]
-        
-        self._update()
+        self.refs[ref] = commit.id
```

### Comparing `echovault-0.2.1/echovault/table.py~` & `echovault-0.2.2/echovault/table.py~`

 * *Files identical despite different names*

### Comparing `echovault-0.2.1/echovault/vault.py~` & `echovault-0.2.2/echovault/vault.py~`

 * *Files identical despite different names*

### Comparing `echovault-0.2.1/PKG-INFO` & `echovault-0.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echovault
-Version: 0.2.1
+Version: 0.2.2
 Summary: echovault is git data storage
 Author: Charles Bajeux
 Author-email: charles.bajeux@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

