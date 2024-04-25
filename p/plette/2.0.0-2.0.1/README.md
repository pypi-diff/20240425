# Comparing `tmp/plette-2.0.0.tar.gz` & `tmp/plette-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plette-2.0.0.tar", last modified: Thu Apr 25 07:34:42 2024, max compression
+gzip compressed data, was "plette-2.0.1.tar", last modified: Thu Apr 25 10:42:00 2024, max compression
```

## Comparing `plette-2.0.0.tar` & `plette-2.0.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:34:42.751733 plette-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-25 07:34:29.000000 plette-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-25 07:34:29.000000 plette-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-25 07:34:42.751733 plette-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-25 07:34:29.000000 plette-2.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-25 07:34:29.000000 plette-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-25 07:34:42.751733 plette-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-25 07:34:29.000000 plette-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:34:42.743733 plette-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:34:42.747733 plette-2.0.0/src/plette/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-25 07:34:29.000000 plette-2.0.0/src/plette/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-25 07:34:29.000000 plette-2.0.0/src/plette/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-04-25 07:34:29.000000 plette-2.0.0/src/plette/lockfiles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:34:42.747733 plette-2.0.0/src/plette/models/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-25 07:34:29.000000 plette-2.0.0/src/plette/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-25 07:34:29.000000 plette-2.0.0/src/plette/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-25 07:34:29.000000 plette-2.0.0/src/plette/models/hashes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-25 07:34:29.000000 plette-2.0.0/src/plette/models/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-25 07:34:29.000000 plette-2.0.0/src/plette/models/scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-04-25 07:34:29.000000 plette-2.0.0/src/plette/models/sections.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-25 07:34:29.000000 plette-2.0.0/src/plette/models/sources.py
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-04-25 07:34:29.000000 plette-2.0.0/src/plette/pipfiles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:34:42.751733 plette-2.0.0/src/plette.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-25 07:34:42.000000 plette-2.0.0/src/plette.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-25 07:34:42.000000 plette-2.0.0/src/plette.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 07:34:42.000000 plette-2.0.0/src/plette.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-25 07:34:42.000000 plette-2.0.0/src/plette.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 07:34:42.000000 plette-2.0.0/src/plette.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 07:34:33.000000 plette-2.0.0/src/plette.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:34:42.747733 plette-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-25 07:34:29.000000 plette-2.0.0/tests/test_lockfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     6501 2024-04-25 07:34:29.000000 plette-2.0.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-25 07:34:29.000000 plette-2.0.0/tests/test_pipfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-25 07:34:29.000000 plette-2.0.0/tests/test_scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:42:00.673123 plette-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-25 10:41:49.000000 plette-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-25 10:41:49.000000 plette-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-25 10:42:00.673123 plette-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-25 10:41:49.000000 plette-2.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-25 10:41:49.000000 plette-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-25 10:42:00.673123 plette-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-25 10:41:49.000000 plette-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:42:00.669123 plette-2.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:42:00.669123 plette-2.0.1/src/plette/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-25 10:41:49.000000 plette-2.0.1/src/plette/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-25 10:41:49.000000 plette-2.0.1/src/plette/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-04-25 10:41:49.000000 plette-2.0.1/src/plette/lockfiles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:42:00.673123 plette-2.0.1/src/plette/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-25 10:41:49.000000 plette-2.0.1/src/plette/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-25 10:41:49.000000 plette-2.0.1/src/plette/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-25 10:41:49.000000 plette-2.0.1/src/plette/models/hashes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-25 10:41:49.000000 plette-2.0.1/src/plette/models/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-25 10:41:49.000000 plette-2.0.1/src/plette/models/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-04-25 10:41:49.000000 plette-2.0.1/src/plette/models/sections.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-25 10:41:49.000000 plette-2.0.1/src/plette/models/sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-04-25 10:41:49.000000 plette-2.0.1/src/plette/pipfiles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:42:00.673123 plette-2.0.1/src/plette.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-25 10:42:00.000000 plette-2.0.1/src/plette.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-25 10:42:00.000000 plette-2.0.1/src/plette.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 10:42:00.000000 plette-2.0.1/src/plette.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-25 10:42:00.000000 plette-2.0.1/src/plette.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 10:42:00.000000 plette-2.0.1/src/plette.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 10:41:52.000000 plette-2.0.1/src/plette.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:42:00.673123 plette-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-25 10:41:49.000000 plette-2.0.1/tests/test_lockfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6501 2024-04-25 10:41:49.000000 plette-2.0.1/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-25 10:41:49.000000 plette-2.0.1/tests/test_pipfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-25 10:41:49.000000 plette-2.0.1/tests/test_scripts.py
```

### Comparing `plette-2.0.0/LICENSE` & `plette-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `plette-2.0.0/PKG-INFO` & `plette-2.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plette
-Version: 2.0.0
+Version: 2.0.1
 Summary: Structured Pipfile and Pipfile.lock models.
 Author-email: Tzu-ping Chung <uranusjr@gmail.com>
 License: ISC License
 Project-URL: Homepage, https://github.com/sarugaku/plette
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
```

### Comparing `plette-2.0.0/README.rst` & `plette-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `plette-2.0.0/pyproject.toml` & `plette-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plette-2.0.0/src/plette/__main__.py` & `plette-2.0.1/src/plette/__main__.py`

 * *Files identical despite different names*

### Comparing `plette-2.0.0/src/plette/lockfiles.py` & `plette-2.0.1/src/plette/lockfiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
                 return Meta(value)
             else:
                 return PackageCollection(value)
         except KeyError:
             return value
 
     def __setitem__(self, key, value):
-        if isinstance(value, DataView):
+        if isinstance(value, DataModel):
             self._data[key] = value._data
         else:
             self._data[key] = value
 
     def is_up_to_date(self, pipfile):
         return self.meta.hash == pipfile.get_hash()
```

### Comparing `plette-2.0.0/src/plette/models/__init__.py` & `plette-2.0.1/src/plette/models/__init__.py`

 * *Files identical despite different names*

### Comparing `plette-2.0.0/src/plette/models/base.py` & `plette-2.0.1/src/plette/models/base.py`

 * *Files identical despite different names*

### Comparing `plette-2.0.0/src/plette/models/hashes.py` & `plette-2.0.1/src/plette/models/hashes.py`

 * *Files identical despite different names*

### Comparing `plette-2.0.0/src/plette/models/packages.py` & `plette-2.0.1/src/plette/models/packages.py`

 * *Files identical despite different names*

### Comparing `plette-2.0.0/src/plette/models/scripts.py` & `plette-2.0.1/src/plette/models/scripts.py`

 * *Files identical despite different names*

### Comparing `plette-2.0.0/src/plette/models/sections.py` & `plette-2.0.1/src/plette/models/sections.py`

 * *Files identical despite different names*

### Comparing `plette-2.0.0/src/plette/models/sources.py` & `plette-2.0.1/src/plette/models/sources.py`

 * *Files identical despite different names*

### Comparing `plette-2.0.0/src/plette/pipfiles.py` & `plette-2.0.1/src/plette/pipfiles.py`

 * *Files identical despite different names*

### Comparing `plette-2.0.0/src/plette.egg-info/PKG-INFO` & `plette-2.0.1/src/plette.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plette
-Version: 2.0.0
+Version: 2.0.1
 Summary: Structured Pipfile and Pipfile.lock models.
 Author-email: Tzu-ping Chung <uranusjr@gmail.com>
 License: ISC License
 Project-URL: Homepage, https://github.com/sarugaku/plette
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
```

### Comparing `plette-2.0.0/src/plette.egg-info/SOURCES.txt` & `plette-2.0.1/src/plette.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plette-2.0.0/tests/test_lockfiles.py` & `plette-2.0.1/tests/test_lockfiles.py`

 * *Files identical despite different names*

### Comparing `plette-2.0.0/tests/test_models.py` & `plette-2.0.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `plette-2.0.0/tests/test_pipfiles.py` & `plette-2.0.1/tests/test_pipfiles.py`

 * *Files identical despite different names*

### Comparing `plette-2.0.0/tests/test_scripts.py` & `plette-2.0.1/tests/test_scripts.py`

 * *Files identical despite different names*

