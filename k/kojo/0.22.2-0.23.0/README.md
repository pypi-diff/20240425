# Comparing `tmp/kojo-0.22.2.tar.gz` & `tmp/kojo-0.23.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kojo-0.22.2.tar", last modified: Thu Apr 25 07:42:48 2024, max compression
+gzip compressed data, was "kojo-0.23.0.tar", last modified: Thu Apr 25 09:00:39 2024, max compression
```

## Comparing `kojo-0.22.2.tar` & `kojo-0.23.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-04-25 07:42:48.911746 kojo-0.22.2/
--rw-rw-r--   0 olaf      (1000) olaf      (1000)    35148 2023-04-27 08:31:58.000000 kojo-0.22.2/LICENSE.txt
--rw-r--r--   0 olaf      (1000) olaf      (1000)     4494 2024-04-25 07:42:48.911746 kojo-0.22.2/PKG-INFO
--rw-rw-r--   0 olaf      (1000) olaf      (1000)     3752 2023-04-27 09:07:15.000000 kojo-0.22.2/README.md
-drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-04-25 07:42:48.911746 kojo-0.22.2/kojo/
--rw-rw-r--   0 olaf      (1000) olaf      (1000)      142 2023-04-27 08:51:59.000000 kojo-0.22.2/kojo/__init__.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)     1115 2024-04-24 05:46:05.000000 kojo-0.22.2/kojo/extra.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)     5238 2024-04-24 07:18:15.000000 kojo-0.22.2/kojo/item.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)     2367 2024-04-24 12:28:53.000000 kojo-0.22.2/kojo/process.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)        0 2024-04-25 07:40:38.000000 kojo-0.22.2/kojo/py.typed
-drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-04-25 07:42:48.911746 kojo-0.22.2/kojo.egg-info/
--rw-r--r--   0 olaf      (1000) olaf      (1000)     4494 2024-04-25 07:42:48.000000 kojo-0.22.2/kojo.egg-info/PKG-INFO
--rw-rw-r--   0 olaf      (1000) olaf      (1000)      222 2024-04-25 07:42:48.000000 kojo-0.22.2/kojo.egg-info/SOURCES.txt
--rw-rw-r--   0 olaf      (1000) olaf      (1000)        1 2024-04-25 07:42:48.000000 kojo-0.22.2/kojo.egg-info/dependency_links.txt
--rw-rw-r--   0 olaf      (1000) olaf      (1000)        5 2024-04-25 07:42:48.000000 kojo-0.22.2/kojo.egg-info/top_level.txt
--rw-rw-r--   0 olaf      (1000) olaf      (1000)      801 2024-04-25 07:42:15.000000 kojo-0.22.2/pyproject.toml
--rw-rw-r--   0 olaf      (1000) olaf      (1000)       38 2024-04-25 07:42:48.911746 kojo-0.22.2/setup.cfg
+drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-04-25 09:00:39.290722 kojo-0.23.0/
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)    35148 2023-04-27 08:31:58.000000 kojo-0.23.0/LICENSE.txt
+-rw-r--r--   0 olaf      (1000) olaf      (1000)     4494 2024-04-25 09:00:39.290722 kojo-0.23.0/PKG-INFO
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)     3752 2023-04-27 09:07:15.000000 kojo-0.23.0/README.md
+drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-04-25 09:00:39.290722 kojo-0.23.0/kojo/
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)      142 2023-04-27 08:51:59.000000 kojo-0.23.0/kojo/__init__.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)     1115 2024-04-24 05:46:05.000000 kojo-0.23.0/kojo/extra.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)     4696 2024-04-25 08:56:19.000000 kojo-0.23.0/kojo/item.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)     2367 2024-04-24 12:28:53.000000 kojo-0.23.0/kojo/process.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)        0 2024-04-25 07:40:38.000000 kojo-0.23.0/kojo/py.typed
+drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-04-25 09:00:39.290722 kojo-0.23.0/kojo.egg-info/
+-rw-r--r--   0 olaf      (1000) olaf      (1000)     4494 2024-04-25 09:00:39.000000 kojo-0.23.0/kojo.egg-info/PKG-INFO
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)      222 2024-04-25 09:00:39.000000 kojo-0.23.0/kojo.egg-info/SOURCES.txt
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)        1 2024-04-25 09:00:39.000000 kojo-0.23.0/kojo.egg-info/dependency_links.txt
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)        5 2024-04-25 09:00:39.000000 kojo-0.23.0/kojo.egg-info/top_level.txt
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)      801 2024-04-25 08:59:54.000000 kojo-0.23.0/pyproject.toml
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)       38 2024-04-25 09:00:39.290722 kojo-0.23.0/setup.cfg
```

### Comparing `kojo-0.22.2/LICENSE.txt` & `kojo-0.23.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kojo-0.22.2/PKG-INFO` & `kojo-0.23.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kojo
-Version: 0.22.2
+Version: 0.23.0
 Summary: A library to transform data through a pipeline
 Author-email: Olaf Schneider <mail@olafschneider.com>
 License: GNU GPLv3
 Project-URL: Repository, https://gitlab.com/filchos/kojo
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `kojo-0.22.2/README.md` & `kojo-0.23.0/README.md`

 * *Files identical despite different names*

### Comparing `kojo-0.22.2/kojo/extra.py` & `kojo-0.23.0/kojo/extra.py`

 * *Files identical despite different names*

### Comparing `kojo-0.22.2/kojo/item.py` & `kojo-0.23.0/kojo/item.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
-from collections import UserDict
+from collections import UserDict, UserList
 import copy
 import json
 import logging
-from typing import Any, Union
+from typing import Any, Iterable, Union
 
 DictType = Union[dict[str, Any], UserDict[str, Any]]
 
 
 def _flatten(item: DictType, prefix: str = "") -> DictType:
     flat_dict = {}
     for k, v in item.items():
@@ -42,27 +42,24 @@
     def __contains__(self, key: str) -> bool:
         return key in self.details
 
     def __getitem__(self, key: str) -> Any:
         return self.details[key]
 
 
-class ItemLog:
-    level: int  # logging.NOTSET .. logging.CRITICAL
-    entries: list[ItemLogEntry]
-
-    def __init__(self) -> None:
-        self.level = logging.NOTSET
-        self.entries = []
+class ItemLog(UserList[ItemLogEntry]):
+    @property
+    def level(self) -> int:
+        if len(self) == 0:
+            return logging.NOTSET
+        return max([entry.level for entry in self])
 
     def log(self, _level: int, _message: str, **details: Any) -> None:
         entry = ItemLogEntry(_level, _message, **details)
-        self.entries.append(entry)
-        if _level > self.level:
-            self.level = _level
+        self.append(entry)
 
     def debug(self, _message: str, **details: Any) -> None:
         self.log(logging.DEBUG, _message, **details)
 
     def info(self, _message: str, **details: Any) -> None:
         self.log(logging.INFO, _message, **details)
 
@@ -72,41 +69,25 @@
     def error(self, _message: str, **details: Any) -> None:
         self.log(logging.ERROR, _message, **details)
 
     def critical(self, _message: str, **details: Any) -> None:
         self.log(logging.CRITICAL, _message, **details)
 
     def clone(self) -> ItemLog:
-        log = ItemLog()
-        log.level = self.level
-        log.entries = copy.copy(self.entries)
-        return log
+        return copy.deepcopy(self)
 
     def __repr__(self) -> str:
-        return "ItemLog(" + ", ".join([repr(entry) for entry in self.entries]) + ")"
-
-    def __len__(self) -> int:
-        return len(self.entries)
+        return "ItemLog(" + ", ".join([repr(entry) for entry in self]) + ")"
 
-    def __add__(self, other: ItemLog) -> ItemLog:
+    def __add__(self, other: Iterable[ItemLogEntry]) -> ItemLog:
         if type(other) is not ItemLog:
-            raise TypeError(
-                "TypeError: unsupported operand type(s) for +: 'ItemLog' and '{}'".format(
-                    type(other).__name__
-                )
-            )
-        log = ItemLog()
-        for entry in self.entries:
-            log.log(entry.level, entry.message, **entry.details)
-        for entry in other.entries:
-            log.log(entry.level, entry.message, **entry.details)
-        return log
+            msg = f"TypeError: unsupported operand type(s) for +: 'ItemLog' and '{type(other).__name__}'"
+            raise TypeError(msg)
 
-    def __getitem__(self, index: int) -> ItemLogEntry:
-        return self.entries[index]
+        return ItemLog(list(self) + list(other))
 
 
 class Item(UserDict[str, Any]):
     """
     Item extends the dictionary class.
 
     Item behaves like a dict but provides additional functionality
@@ -148,15 +129,15 @@
             "details": entry.details,
         }
 
 
 class ItemLogEncoder(json.JSONEncoder):
     def default(self, item_log: ItemLog) -> list[dict[str, Any]]:
         encoder = ItemLogEntryEncoder()
-        return [encoder.default(entry) for entry in item_log.entries]
+        return [encoder.default(entry) for entry in item_log]
 
 
 class ItemEncoder(json.JSONEncoder):
     def default(self, item: Item) -> dict[str, Any]:
         return {
             "data": dict(item),
             "log": ItemLogEncoder().default(item.log),
```

### Comparing `kojo-0.22.2/kojo/process.py` & `kojo-0.23.0/kojo/process.py`

 * *Files identical despite different names*

### Comparing `kojo-0.22.2/kojo.egg-info/PKG-INFO` & `kojo-0.23.0/kojo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kojo
-Version: 0.22.2
+Version: 0.23.0
 Summary: A library to transform data through a pipeline
 Author-email: Olaf Schneider <mail@olafschneider.com>
 License: GNU GPLv3
 Project-URL: Repository, https://gitlab.com/filchos/kojo
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `kojo-0.22.2/pyproject.toml` & `kojo-0.23.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kojo"
-version = "0.22.2"
+version = "0.23.0"
 requires-python = ">= 3.10"
 authors = [{ name = "Olaf Schneider", email = "mail@olafschneider.com" }]
 description = "A library to transform data through a pipeline"
 readme = "README.md"
 license = { text = "GNU GPLv3" }
 classifiers = [
     "Development Status :: 4 - Beta",
```

