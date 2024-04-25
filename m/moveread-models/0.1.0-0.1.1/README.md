# Comparing `tmp/moveread_models-0.1.0.tar.gz` & `tmp/moveread_models-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread_models-0.1.0.tar", last modified: Thu Apr 25 06:55:13 2024, max compression
+gzip compressed data, was "moveread_models-0.1.1.tar", last modified: Thu Apr 25 09:17:07 2024, max compression
```

## Comparing `moveread_models-0.1.0.tar` & `moveread_models-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:55:13.624241 moveread_models-0.1.0/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      563 2024-04-25 06:55:13.624241 moveread_models-0.1.0/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       40 2024-04-24 16:25:57.000000 moveread_models-0.1.0/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      583 2024-04-25 06:54:37.000000 moveread_models-0.1.0/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-25 06:55:13.624241 moveread_models-0.1.0/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:55:13.614241 moveread_models-0.1.0/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:55:13.614241 moveread_models-0.1.0/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:55:13.614241 moveread_models-0.1.0/src/moveread/models/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      179 2024-04-24 16:51:19.000000 moveread_models-0.1.0/src/moveread/models/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      293 2024-04-25 06:24:33.000000 moveread_models-0.1.0/src/moveread/models/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      524 2024-04-25 06:24:04.000000 moveread_models-0.1.0/src/moveread/models/eval.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:55:13.624241 moveread_models-0.1.0/src/moveread/models/experiments/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-24 18:04:53.000000 moveread_models-0.1.0/src/moveread/models/experiments/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      269 2024-04-24 19:07:09.000000 moveread_models-0.1.0/src/moveread/models/experiments/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      554 2024-04-25 06:00:27.000000 moveread_models-0.1.0/src/moveread/models/experiments/api.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      607 2024-04-25 06:19:03.000000 moveread_models-0.1.0/src/moveread/models/experiments/experiments.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:55:13.624241 moveread_models-0.1.0/src/moveread/models/experiments/hparams/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-24 18:59:45.000000 moveread_models-0.1.0/src/moveread/models/experiments/hparams/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      291 2024-04-24 19:08:30.000000 moveread_models-0.1.0/src/moveread/models/experiments/hparams/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      426 2024-04-24 19:07:08.000000 moveread_models-0.1.0/src/moveread/models/experiments/hparams/_hparams.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      469 2024-04-24 19:09:36.000000 moveread_models-0.1.0/src/moveread/models/experiments/hparams/optimizers.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:55:13.624241 moveread_models-0.1.0/src/moveread/models/models/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-24 16:50:59.000000 moveread_models-0.1.0/src/moveread/models/models/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       93 2024-04-24 18:09:01.000000 moveread_models-0.1.0/src/moveread/models/models/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      406 2024-04-24 18:08:45.000000 moveread_models-0.1.0/src/moveread/models/models/_create.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2020 2024-04-24 17:01:50.000000 moveread_models-0.1.0/src/moveread/models/models/_original.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:55:13.624241 moveread_models-0.1.0/src/moveread_models.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      563 2024-04-25 06:55:13.000000 moveread_models-0.1.0/src/moveread_models.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      874 2024-04-25 06:55:13.000000 moveread_models-0.1.0/src/moveread_models.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-25 06:55:13.000000 moveread_models-0.1.0/src/moveread_models.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       70 2024-04-25 06:55:13.000000 moveread_models-0.1.0/src/moveread_models.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-04-25 06:55:13.000000 moveread_models-0.1.0/src/moveread_models.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 09:17:07.014237 moveread_models-0.1.1/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      563 2024-04-25 09:17:07.014237 moveread_models-0.1.1/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       40 2024-04-24 16:25:57.000000 moveread_models-0.1.1/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      583 2024-04-25 09:17:04.000000 moveread_models-0.1.1/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-25 09:17:07.014237 moveread_models-0.1.1/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 09:17:07.004238 moveread_models-0.1.1/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 09:17:07.004238 moveread_models-0.1.1/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 09:17:07.004238 moveread_models-0.1.1/src/moveread/models/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      179 2024-04-24 16:51:19.000000 moveread_models-0.1.1/src/moveread/models/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      323 2024-04-25 07:51:37.000000 moveread_models-0.1.1/src/moveread/models/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      524 2024-04-25 06:24:04.000000 moveread_models-0.1.1/src/moveread/models/eval.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 09:17:07.004238 moveread_models-0.1.1/src/moveread/models/experiments/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-24 18:04:53.000000 moveread_models-0.1.1/src/moveread/models/experiments/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      339 2024-04-25 09:09:50.000000 moveread_models-0.1.1/src/moveread/models/experiments/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      640 2024-04-25 09:14:32.000000 moveread_models-0.1.1/src/moveread/models/experiments/api.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      718 2024-04-25 09:04:57.000000 moveread_models-0.1.1/src/moveread/models/experiments/experiments.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 09:17:07.004238 moveread_models-0.1.1/src/moveread/models/experiments/hparams/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-24 18:59:45.000000 moveread_models-0.1.1/src/moveread/models/experiments/hparams/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      291 2024-04-24 19:08:30.000000 moveread_models-0.1.1/src/moveread/models/experiments/hparams/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      426 2024-04-24 19:07:08.000000 moveread_models-0.1.1/src/moveread/models/experiments/hparams/_hparams.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      469 2024-04-24 19:09:36.000000 moveread_models-0.1.1/src/moveread/models/experiments/hparams/optimizers.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 09:17:07.014237 moveread_models-0.1.1/src/moveread/models/models/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-24 16:50:59.000000 moveread_models-0.1.1/src/moveread/models/models/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      143 2024-04-25 09:11:13.000000 moveread_models-0.1.1/src/moveread/models/models/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      406 2024-04-24 18:08:45.000000 moveread_models-0.1.1/src/moveread/models/models/_create.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      259 2024-04-25 09:11:02.000000 moveread_models-0.1.1/src/moveread/models/models/_load.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2020 2024-04-24 17:01:50.000000 moveread_models-0.1.1/src/moveread/models/models/_original.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       65 2024-04-25 09:16:55.000000 moveread_models-0.1.1/src/moveread/models/models/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 09:17:07.014237 moveread_models-0.1.1/src/moveread_models.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      563 2024-04-25 09:17:06.000000 moveread_models-0.1.1/src/moveread_models.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      946 2024-04-25 09:17:06.000000 moveread_models-0.1.1/src/moveread_models.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-25 09:17:06.000000 moveread_models-0.1.1/src/moveread_models.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       70 2024-04-25 09:17:06.000000 moveread_models-0.1.1/src/moveread_models.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-04-25 09:17:06.000000 moveread_models-0.1.1/src/moveread_models.egg-info/top_level.txt
```

### Comparing `moveread_models-0.1.0/PKG-INFO` & `moveread_models-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-models
-Version: 0.1.0
+Version: 0.1.1
 Summary: Model training, metrics and metadata for Moveread OCR
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-ocr.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: lazy-load
 Requires-Dist: pydantic
```

### Comparing `moveread_models-0.1.0/pyproject.toml` & `moveread_models-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-models"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Model training, metrics and metadata for Moveread OCR"
 dependencies = [
   "lazy-load", "pydantic", "kv-api", "kv-fs", "kv-sqlite-sync"
 ]
```

### Comparing `moveread_models-0.1.0/src/moveread/models/eval.py` & `moveread_models-0.1.1/src/moveread/models/eval.py`

 * *Files identical despite different names*

### Comparing `moveread_models-0.1.0/src/moveread/models/experiments/api.py` & `moveread_models-0.1.1/src/moveread/models/experiments/api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from dataclasses import dataclass
 from kv.api import KV
 from kv.fs import FilesystemKV
 from .experiments import Experiment
+from ..models import load_artifact
 
 @dataclass
 class ModelsAPI:
   """API to store models and experiments: artifacts, metrics, etc."""
   meta: KV[Experiment]
   artifacts: FilesystemKV[bytes]
 
@@ -13,8 +14,11 @@
   def at(cls, path: str) -> 'ModelsAPI':
     import os
     from kv.sqlite import SQLiteKV
     return ModelsAPI(
       meta=SQLiteKV.validated(Experiment, os.path.join(path, 'meta.sqlite')),
       artifacts=FilesystemKV(os.path.join(path, 'artifacts'))
     )
+  
+  async def load(self, experimentId: str):
+
```

### Comparing `moveread_models-0.1.0/src/moveread/models/models/_original.py` & `moveread_models-0.1.1/src/moveread/models/models/_original.py`

 * *Files identical despite different names*

### Comparing `moveread_models-0.1.0/src/moveread_models.egg-info/PKG-INFO` & `moveread_models-0.1.1/src/moveread_models.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-models
-Version: 0.1.0
+Version: 0.1.1
 Summary: Model training, metrics and metadata for Moveread OCR
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-ocr.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: lazy-load
 Requires-Dist: pydantic
```

### Comparing `moveread_models-0.1.0/src/moveread_models.egg-info/SOURCES.txt` & `moveread_models-0.1.1/src/moveread_models.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,13 +10,15 @@
 src/moveread/models/experiments/hparams/__init__.py
 src/moveread/models/experiments/hparams/__init__.pyi
 src/moveread/models/experiments/hparams/_hparams.py
 src/moveread/models/experiments/hparams/optimizers.py
 src/moveread/models/models/__init__.py
 src/moveread/models/models/__init__.pyi
 src/moveread/models/models/_create.py
+src/moveread/models/models/_load.py
 src/moveread/models/models/_original.py
+src/moveread/models/models/types.py
 src/moveread_models.egg-info/PKG-INFO
 src/moveread_models.egg-info/SOURCES.txt
 src/moveread_models.egg-info/dependency_links.txt
 src/moveread_models.egg-info/requires.txt
 src/moveread_models.egg-info/top_level.txt
```

