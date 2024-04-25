# Comparing `tmp/moveread_models-0.1.1.tar.gz` & `tmp/moveread_models-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread_models-0.1.1.tar", last modified: Thu Apr 25 09:17:07 2024, max compression
+gzip compressed data, was "moveread_models-0.1.2.tar", last modified: Thu Apr 25 14:34:17 2024, max compression
```

## Comparing `moveread_models-0.1.1.tar` & `moveread_models-0.1.2.tar`

### file list

```diff
@@ -1,34 +1,39 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 09:17:07.014237 moveread_models-0.1.1/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      563 2024-04-25 09:17:07.014237 moveread_models-0.1.1/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       40 2024-04-24 16:25:57.000000 moveread_models-0.1.1/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      583 2024-04-25 09:17:04.000000 moveread_models-0.1.1/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-25 09:17:07.014237 moveread_models-0.1.1/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 09:17:07.004238 moveread_models-0.1.1/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 09:17:07.004238 moveread_models-0.1.1/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 09:17:07.004238 moveread_models-0.1.1/src/moveread/models/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      179 2024-04-24 16:51:19.000000 moveread_models-0.1.1/src/moveread/models/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      323 2024-04-25 07:51:37.000000 moveread_models-0.1.1/src/moveread/models/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      524 2024-04-25 06:24:04.000000 moveread_models-0.1.1/src/moveread/models/eval.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 09:17:07.004238 moveread_models-0.1.1/src/moveread/models/experiments/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-24 18:04:53.000000 moveread_models-0.1.1/src/moveread/models/experiments/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      339 2024-04-25 09:09:50.000000 moveread_models-0.1.1/src/moveread/models/experiments/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      640 2024-04-25 09:14:32.000000 moveread_models-0.1.1/src/moveread/models/experiments/api.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      718 2024-04-25 09:04:57.000000 moveread_models-0.1.1/src/moveread/models/experiments/experiments.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 09:17:07.004238 moveread_models-0.1.1/src/moveread/models/experiments/hparams/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-24 18:59:45.000000 moveread_models-0.1.1/src/moveread/models/experiments/hparams/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      291 2024-04-24 19:08:30.000000 moveread_models-0.1.1/src/moveread/models/experiments/hparams/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      426 2024-04-24 19:07:08.000000 moveread_models-0.1.1/src/moveread/models/experiments/hparams/_hparams.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      469 2024-04-24 19:09:36.000000 moveread_models-0.1.1/src/moveread/models/experiments/hparams/optimizers.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 09:17:07.014237 moveread_models-0.1.1/src/moveread/models/models/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-24 16:50:59.000000 moveread_models-0.1.1/src/moveread/models/models/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      143 2024-04-25 09:11:13.000000 moveread_models-0.1.1/src/moveread/models/models/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      406 2024-04-24 18:08:45.000000 moveread_models-0.1.1/src/moveread/models/models/_create.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      259 2024-04-25 09:11:02.000000 moveread_models-0.1.1/src/moveread/models/models/_load.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2020 2024-04-24 17:01:50.000000 moveread_models-0.1.1/src/moveread/models/models/_original.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       65 2024-04-25 09:16:55.000000 moveread_models-0.1.1/src/moveread/models/models/types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 09:17:07.014237 moveread_models-0.1.1/src/moveread_models.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      563 2024-04-25 09:17:06.000000 moveread_models-0.1.1/src/moveread_models.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      946 2024-04-25 09:17:06.000000 moveread_models-0.1.1/src/moveread_models.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-25 09:17:06.000000 moveread_models-0.1.1/src/moveread_models.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       70 2024-04-25 09:17:06.000000 moveread_models-0.1.1/src/moveread_models.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-04-25 09:17:06.000000 moveread_models-0.1.1/src/moveread_models.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 14:34:17.975633 moveread_models-0.1.2/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      563 2024-04-25 14:34:17.975633 moveread_models-0.1.2/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       40 2024-04-24 16:25:57.000000 moveread_models-0.1.2/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      583 2024-04-25 14:34:14.000000 moveread_models-0.1.2/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-25 14:34:17.975633 moveread_models-0.1.2/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 14:34:17.955630 moveread_models-0.1.2/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 14:34:17.955630 moveread_models-0.1.2/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 14:34:17.965631 moveread_models-0.1.2/src/moveread/models/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-25 09:29:13.000000 moveread_models-0.1.2/src/moveread/models/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       94 2024-04-25 10:07:15.000000 moveread_models-0.1.2/src/moveread/models/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      548 2024-04-25 09:44:16.000000 moveread_models-0.1.2/src/moveread/models/api.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 14:34:17.965631 moveread_models-0.1.2/src/moveread/models/impl/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-25 10:06:39.000000 moveread_models-0.1.2/src/moveread/models/impl/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      195 2024-04-25 10:07:56.000000 moveread_models-0.1.2/src/moveread/models/impl/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      975 2024-04-25 10:32:49.000000 moveread_models-0.1.2/src/moveread/models/impl/_optimizer.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      519 2024-04-25 10:08:01.000000 moveread_models-0.1.2/src/moveread/models/impl/eval.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 14:34:17.965631 moveread_models-0.1.2/src/moveread/models/impl/models/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-25 09:49:31.000000 moveread_models-0.1.2/src/moveread/models/impl/models/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      118 2024-04-25 09:50:32.000000 moveread_models-0.1.2/src/moveread/models/impl/models/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      309 2024-04-25 09:48:11.000000 moveread_models-0.1.2/src/moveread/models/impl/models/_load.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2021 2024-04-25 09:45:56.000000 moveread_models-0.1.2/src/moveread/models/impl/models/_original.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      403 2024-04-25 09:46:26.000000 moveread_models-0.1.2/src/moveread/models/impl/models/create.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 14:34:17.965631 moveread_models-0.1.2/src/moveread/models/types/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-25 09:43:29.000000 moveread_models-0.1.2/src/moveread/models/types/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      245 2024-04-25 09:47:39.000000 moveread_models-0.1.2/src/moveread/models/types/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      734 2024-04-25 09:47:30.000000 moveread_models-0.1.2/src/moveread/models/types/_types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 14:34:17.965631 moveread_models-0.1.2/src/moveread/models/types/hparams/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-25 09:40:18.000000 moveread_models-0.1.2/src/moveread/models/types/hparams/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      360 2024-04-25 10:03:15.000000 moveread_models-0.1.2/src/moveread/models/types/hparams/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      229 2024-04-25 09:34:01.000000 moveread_models-0.1.2/src/moveread/models/types/hparams/_hparams.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      261 2024-04-25 09:31:58.000000 moveread_models-0.1.2/src/moveread/models/types/hparams/models.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      495 2024-04-25 10:34:42.000000 moveread_models-0.1.2/src/moveread/models/types/hparams/optimizers.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      107 2024-04-25 09:33:49.000000 moveread_models-0.1.2/src/moveread/models/types/hparams/run.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 14:34:17.975633 moveread_models-0.1.2/src/moveread_models.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      563 2024-04-25 14:34:17.000000 moveread_models-0.1.2/src/moveread_models.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1079 2024-04-25 14:34:17.000000 moveread_models-0.1.2/src/moveread_models.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-25 14:34:17.000000 moveread_models-0.1.2/src/moveread_models.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       70 2024-04-25 14:34:17.000000 moveread_models-0.1.2/src/moveread_models.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-04-25 14:34:17.000000 moveread_models-0.1.2/src/moveread_models.egg-info/top_level.txt
```

### Comparing `moveread_models-0.1.1/PKG-INFO` & `moveread_models-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-models
-Version: 0.1.1
+Version: 0.1.2
 Summary: Model training, metrics and metadata for Moveread OCR
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-ocr.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: lazy-load
 Requires-Dist: pydantic
```

### Comparing `moveread_models-0.1.1/pyproject.toml` & `moveread_models-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-models"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Model training, metrics and metadata for Moveread OCR"
 dependencies = [
   "lazy-load", "pydantic", "kv-api", "kv-fs", "kv-sqlite-sync"
 ]
```

### Comparing `moveread_models-0.1.1/src/moveread/models/eval.py` & `moveread_models-0.1.2/src/moveread/models/impl/eval.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import tensorflow as tf
 import keras
 import tf_ctc as ctc
-from .experiments import Metrics
+from ..types import Metrics
 
 def top5_accuracy(labs, logits):
   return ctc.accuracy(labs, logits, k=5)
 
 def evaluate(model: keras.Model, ds: tf.data.Dataset) -> Metrics:
   metrics = dict(
     ctc_loss=ctc.loss, accuracy=ctc.accuracy,
```

### Comparing `moveread_models-0.1.1/src/moveread/models/experiments/api.py` & `moveread_models-0.1.2/src/moveread/models/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from dataclasses import dataclass
 from kv.api import KV
 from kv.fs import FilesystemKV
-from .experiments import Experiment
-from ..models import load_artifact
+from .types import Experiment
 
 @dataclass
 class ModelsAPI:
   """API to store models and experiments: artifacts, metrics, etc."""
   meta: KV[Experiment]
   artifacts: FilesystemKV[bytes]
 
@@ -14,11 +13,8 @@
   def at(cls, path: str) -> 'ModelsAPI':
     import os
     from kv.sqlite import SQLiteKV
     return ModelsAPI(
       meta=SQLiteKV.validated(Experiment, os.path.join(path, 'meta.sqlite')),
       artifacts=FilesystemKV(os.path.join(path, 'artifacts'))
     )
-  
-  async def load(self, experimentId: str):
-
```

### Comparing `moveread_models-0.1.1/src/moveread/models/experiments/experiments.py` & `moveread_models-0.1.2/src/moveread/models/types/_types.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import TypeAlias, Literal
 from pydantic import BaseModel, ConfigDict
 from .hparams import HParams
 
 DatasetID: TypeAlias = str
 
-Format = Literal['tf2', 'keras']
+ArtifactFormat = Literal['tf2', 'keras']
 
 class Artifact(BaseModel):
-  format: Format
+  format: ArtifactFormat
   file: str
 
 class Metrics(BaseModel):
   model_config = ConfigDict(extra='forbid')
   ctc_loss: float | None = None
   accuracy: float | None = None
   top5_accuracy: float | None = None
```

### Comparing `moveread_models-0.1.1/src/moveread/models/models/_original.py` & `moveread_models-0.1.2/src/moveread/models/impl/models/_original.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -20,8 +20,8 @@
     kl.Conv2D(512, kernel_size=(3, 3), strides=(1, 1), padding='same', activation='relu', use_bias=False, name="conv6", kernel_initializer=conv_kernel_initializer),
     kl.MaxPooling2D(pool_size=(2, 1), strides=(2, 1), padding='valid'),
     kl.MaxPooling2D(pool_size=(2, 2), strides=(3, 2), padding='valid'),
     kl.Reshape((11, -1)),
     kl.Bidirectional(kl.LSTM(256, return_sequences=True, dropout=lstm_dropout), name="BiLSTM1"),
     kl.Bidirectional(kl.LSTM(256, return_sequences=True, dropout=lstm_dropout), name="BiLSTM2"),
     kl.Dense(num_classes, activation=None, name="dense")
-  ], name="original")
+  ], name="original")
```

### Comparing `moveread_models-0.1.1/src/moveread_models.egg-info/PKG-INFO` & `moveread_models-0.1.2/src/moveread_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-models
-Version: 0.1.1
+Version: 0.1.2
 Summary: Model training, metrics and metadata for Moveread OCR
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-ocr.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: lazy-load
 Requires-Dist: pydantic
```

