# Comparing `tmp/data-place-0.1.6.tar.gz` & `tmp/data-place-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-place-0.1.6.tar", last modified: Sun Feb 11 17:10:41 2024, max compression
+gzip compressed data, was "data-place-0.2.0.tar", last modified: Thu Apr 25 06:17:15 2024, max compression
```

## Comparing `data-place-0.1.6.tar` & `data-place-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-02-11 17:10:41.276826 data-place-0.1.6/
--rw-rw-rw-   0        0        0       74 2024-02-11 17:10:41.000000 data-place-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     6188 2024-02-11 17:10:41.275825 data-place-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     5156 2024-01-27 16:23:24.000000 data-place-0.1.6/README.md
--rw-rw-rw-   0        0        0    12832 2024-01-20 13:15:44.000000 data-place-0.1.6/build.py
-drwxrwxrwx   0        0        0        0 2024-02-11 17:10:41.273826 data-place-0.1.6/data_place.egg-info/
--rw-rw-rw-   0        0        0     6188 2024-02-11 17:10:41.000000 data-place-0.1.6/data_place.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2024-02-11 17:10:41.000000 data-place-0.1.6/data_place.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-11 17:10:41.000000 data-place-0.1.6/data_place.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-02-11 17:10:41.000000 data-place-0.1.6/data_place.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-02-11 17:10:41.000000 data-place-0.1.6/data_place.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-02-11 17:10:41.271827 data-place-0.1.6/dataplace/
--rw-rw-rw-   0        0        0      269 2024-01-20 13:15:44.000000 data-place-0.1.6/dataplace/__init__.py
--rw-rw-rw-   0        0        0     1611 2024-01-24 19:26:19.000000 data-place-0.1.6/dataplace/base.py
--rw-rw-rw-   0        0        0     2304 2024-01-27 08:30:20.000000 data-place-0.1.6/dataplace/callback.py
--rw-rw-rw-   0        0        0     2251 2024-01-27 16:19:43.000000 data-place-0.1.6/dataplace/control.py
--rw-rw-rw-   0        0        0     3556 2024-02-11 17:10:37.000000 data-place-0.1.6/dataplace/handler.py
--rw-rw-rw-   0        0        0     2771 2024-01-25 20:35:44.000000 data-place-0.1.6/dataplace/io.py
--rw-rw-rw-   0        0        0     8302 2024-01-26 07:10:39.000000 data-place-0.1.6/dataplace/receive.py
--rw-rw-rw-   0        0        0    10585 2024-01-26 07:23:18.000000 data-place-0.1.6/dataplace/send.py
--rw-rw-rw-   0        0        0     7833 2024-01-27 16:23:24.000000 data-place-0.1.6/dataplace/store.py
--rw-rw-rw-   0        0        0       34 2024-01-20 13:15:44.000000 data-place-0.1.6/requirements-dev.txt
--rw-rw-rw-   0        0        0       10 2024-01-20 13:15:44.000000 data-place-0.1.6/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-02-11 17:10:41.276826 data-place-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1615 2024-02-11 17:10:37.000000 data-place-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 06:17:15.660901 data-place-0.2.0/
+-rw-rw-rw-   0        0        0       44 2024-04-25 06:17:15.000000 data-place-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6073 2024-04-25 06:17:15.660901 data-place-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5156 2024-01-27 16:23:24.000000 data-place-0.2.0/README.md
+-rw-rw-rw-   0        0        0     9793 2024-04-19 12:34:18.000000 data-place-0.2.0/build.py
+drwxrwxrwx   0        0        0        0 2024-04-25 06:17:15.659900 data-place-0.2.0/data_place.egg-info/
+-rw-rw-rw-   0        0        0     6073 2024-04-25 06:17:15.000000 data-place-0.2.0/data_place.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2024-04-25 06:17:15.000000 data-place-0.2.0/data_place.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 06:17:15.000000 data-place-0.2.0/data_place.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-25 06:17:15.000000 data-place-0.2.0/data_place.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-25 06:17:15.000000 data-place-0.2.0/data_place.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 06:17:15.658901 data-place-0.2.0/dataplace/
+-rw-rw-rw-   0        0        0      269 2024-01-20 13:15:44.000000 data-place-0.2.0/dataplace/__init__.py
+-rw-rw-rw-   0        0        0     1611 2024-01-24 19:26:19.000000 data-place-0.2.0/dataplace/base.py
+-rw-rw-rw-   0        0        0     2304 2024-01-27 08:30:20.000000 data-place-0.2.0/dataplace/callback.py
+-rw-rw-rw-   0        0        0     2251 2024-01-27 16:19:43.000000 data-place-0.2.0/dataplace/control.py
+-rw-rw-rw-   0        0        0     3556 2024-02-11 17:10:37.000000 data-place-0.2.0/dataplace/handler.py
+-rw-rw-rw-   0        0        0     2771 2024-01-25 20:35:44.000000 data-place-0.2.0/dataplace/io.py
+-rw-rw-rw-   0        0        0     8302 2024-01-26 07:10:39.000000 data-place-0.2.0/dataplace/receive.py
+-rw-rw-rw-   0        0        0    10585 2024-01-26 07:23:18.000000 data-place-0.2.0/dataplace/send.py
+-rw-rw-rw-   0        0        0     7533 2024-04-25 06:14:46.000000 data-place-0.2.0/dataplace/store.py
+-rw-rw-rw-   0        0        0       10 2024-01-20 13:15:44.000000 data-place-0.2.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 06:17:15.660901 data-place-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1615 2024-04-25 06:17:12.000000 data-place-0.2.0/setup.py
```

### Comparing `data-place-0.1.6/PKG-INFO` & `data-place-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-place
-Version: 0.1.6
+Version: 0.2.0
 Summary: A powerfull and flexible framework for designing async socket based data streaming and distribution systems, with automated parsing, dynamic data store and high-level control hooks.
 Home-page: https://github.com/Shahaf-F-S/data-place
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,17 +14,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: websockets
 Provides-Extra: dev
-Requires-Dist: pdoc3; extra == "dev"
-Requires-Dist: twine; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
 
 # data-place
 
 > A powerful and flexible framework for designing async socket based data streaming and distribution systems, with automated parsing, dynamic data store and high-level control hooks.
 
 Installation
 -----------
```

### Comparing `data-place-0.1.6/README.md` & `data-place-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `data-place-0.1.6/data_place.egg-info/PKG-INFO` & `data-place-0.2.0/data_place.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-place
-Version: 0.1.6
+Version: 0.2.0
 Summary: A powerfull and flexible framework for designing async socket based data streaming and distribution systems, with automated parsing, dynamic data store and high-level control hooks.
 Home-page: https://github.com/Shahaf-F-S/data-place
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,17 +14,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: websockets
 Provides-Extra: dev
-Requires-Dist: pdoc3; extra == "dev"
-Requires-Dist: twine; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
 
 # data-place
 
 > A powerful and flexible framework for designing async socket based data streaming and distribution systems, with automated parsing, dynamic data store and high-level control hooks.
 
 Installation
 -----------
```

### Comparing `data-place-0.1.6/dataplace/base.py` & `data-place-0.2.0/dataplace/base.py`

 * *Files identical despite different names*

### Comparing `data-place-0.1.6/dataplace/callback.py` & `data-place-0.2.0/dataplace/callback.py`

 * *Files identical despite different names*

### Comparing `data-place-0.1.6/dataplace/control.py` & `data-place-0.2.0/dataplace/control.py`

 * *Files identical despite different names*

### Comparing `data-place-0.1.6/dataplace/handler.py` & `data-place-0.2.0/dataplace/handler.py`

 * *Files identical despite different names*

### Comparing `data-place-0.1.6/dataplace/io.py` & `data-place-0.2.0/dataplace/io.py`

 * *Files identical despite different names*

### Comparing `data-place-0.1.6/dataplace/receive.py` & `data-place-0.2.0/dataplace/receive.py`

 * *Files identical despite different names*

### Comparing `data-place-0.1.6/dataplace/send.py` & `data-place-0.2.0/dataplace/send.py`

 * *Files identical despite different names*

### Comparing `data-place-0.1.6/dataplace/store.py` & `data-place-0.2.0/dataplace/store.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,47 +44,41 @@
 class SpaceStore[S: Hashable | Iterable[Hashable], D]:
 
     def __init__(self, signature: Callable[[D], S], item: type[D]) -> None:
 
         self.item = item
         self.signature = signature
 
-        self.store: dict[S, list[D]] = {}
+        self.store: dict[tuple[S, ...], list[D]] = {}
 
     def __len__(self) -> int:
 
         return len(self.store)
 
     def __iter__(self) -> Generator[S, ..., ...]:
 
         yield from self.keys()
 
     def __contains__(self, item: S | D) -> bool:
 
-        saved = None
-
-        if isinstance(item, self.item):
-            saved = item
-
-            item = item.signature
-
-        if not (
+        if (
             isinstance(item, Hashable) and
-            isinstance(item, collections.abc.Iterable)
+            not isinstance(item, collections.abc.Iterable)
         ):
-            return False
+            item = (item,)
 
-        item = tuple(item)
-
-        if len(item) != 2:
-            return False
+        if (
+            not isinstance(item, Hashable) and
+            isinstance(item, collections.abc.Iterable)
+        ):
+            item = tuple(item)
 
         return (
             (item in self.store) and
-            (saved is None or saved in self.store[item])
+            (item is None or item in self.store[item])
         )
 
     def __add__(self, other: ...) -> Self:
 
         if not isinstance(other, type(self)):
             raise TypeError(
                 f"both objects must be {type(self)} "
@@ -127,26 +121,14 @@
 
             yield keys, values
 
     def signatures(self) -> set[S]:
 
         return set(self.keys())
 
-    def records(self) -> list[D]:
-
-        records = []
-
-        for (exchange, symbol), values in self.store.items():
-            if None in (exchange, symbol):
-                continue
-
-            records.extend(values)
-
-        return records
-
     @staticmethod
     def validate_signature(signature: ...) -> tuple:
 
         if not isinstance(signature, collections.abc.Iterable):
             signature = (signature,)
 
         if not (
```

### Comparing `data-place-0.1.6/setup.py` & `data-place-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             "__pycache__",
             "*.pyc"
         ],
         include=[],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='data-place',
-        version='0.1.6',
+        version='0.2.0',
         description=(
             "A powerfull and flexible framework for designing async "
             "socket based data streaming and distribution systems, "
             "with automated parsing, dynamic data store and "
             "high-level control hooks."
         ),
         license='MIT',
```

