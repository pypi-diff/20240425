# Comparing `tmp/keras_generators-1.4.4-py3-none-any.whl.zip` & `tmp/keras_generators-1.4.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 30014 bytes, number of entries: 16
+Zip file size: 30013 bytes, number of entries: 16
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-08 16:27 examples/__init__.py
 -rw-rw-rw-  2.0 fat     6233 b- defN 23-Apr-13 14:38 examples/predict_stock_price.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-08 16:27 keras_generators/__init__.py
 -rw-rw-rw-  2.0 fat     6339 b- defN 24-Apr-24 11:12 keras_generators/callbacks.py
 -rw-rw-rw-  2.0 fat     1471 b- defN 24-Apr-24 12:10 keras_generators/common.py
 -rw-rw-rw-  2.0 fat    10842 b- defN 23-Mar-08 16:27 keras_generators/encoders.py
 -rw-rw-rw-  2.0 fat    36073 b- defN 24-Apr-22 16:04 keras_generators/generators.py
 -rw-rw-rw-  2.0 fat     4139 b- defN 23-Mar-08 19:39 keras_generators/splitters.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-08 16:27 keras_generators/model_abstractions/__init__.py
--rw-rw-rw-  2.0 fat     8066 b- defN 24-Apr-24 12:06 keras_generators/model_abstractions/model_object.py
+-rw-rw-rw-  2.0 fat     8073 b- defN 24-Apr-25 20:12 keras_generators/model_abstractions/model_object.py
 -rw-rw-rw-  2.0 fat     3263 b- defN 24-Apr-22 14:58 keras_generators/model_abstractions/model_params.py
--rw-rw-rw-  2.0 fat    11558 b- defN 24-Apr-24 12:12 keras_generators-1.4.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    13884 b- defN 24-Apr-24 12:12 keras_generators-1.4.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-24 12:12 keras_generators-1.4.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       26 b- defN 24-Apr-24 12:12 keras_generators-1.4.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1423 b- defN 24-Apr-24 12:12 keras_generators-1.4.4.dist-info/RECORD
-16 files, 103409 bytes uncompressed, 27628 bytes compressed:  73.3%
+-rw-rw-rw-  2.0 fat    11558 b- defN 24-Apr-25 20:12 keras_generators-1.4.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    13884 b- defN 24-Apr-25 20:12 keras_generators-1.4.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-25 20:12 keras_generators-1.4.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       26 b- defN 24-Apr-25 20:12 keras_generators-1.4.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1423 b- defN 24-Apr-25 20:12 keras_generators-1.4.5.dist-info/RECORD
+16 files, 103416 bytes uncompressed, 27627 bytes compressed:  73.3%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: keras_generators/model_abstractions/model_object.py
 Comment: 
 
 Filename: keras_generators/model_abstractions/model_params.py
 Comment: 
 
-Filename: keras_generators-1.4.4.dist-info/LICENSE
+Filename: keras_generators-1.4.5.dist-info/LICENSE
 Comment: 
 
-Filename: keras_generators-1.4.4.dist-info/METADATA
+Filename: keras_generators-1.4.5.dist-info/METADATA
 Comment: 
 
-Filename: keras_generators-1.4.4.dist-info/WHEEL
+Filename: keras_generators-1.4.5.dist-info/WHEEL
 Comment: 
 
-Filename: keras_generators-1.4.4.dist-info/top_level.txt
+Filename: keras_generators-1.4.5.dist-info/top_level.txt
 Comment: 
 
-Filename: keras_generators-1.4.4.dist-info/RECORD
+Filename: keras_generators-1.4.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## keras_generators/model_abstractions/model_object.py

```diff
@@ -4,17 +4,17 @@
 import gzip
 import logging
 import pickle
 from abc import ABC
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Type, Union
 
-import keras.backend as K
 import tensorflow as tf
-from keras import Model
+import tf_keras as keras
+import tf_keras.backend as K
 from tf_keras.callbacks import (
     Callback,
     CSVLogger,
     EarlyStopping,
     History,
     ModelCheckpoint,
     ReduceLROnPlateau,
@@ -27,15 +27,15 @@
 from ..model_abstractions.model_params import ModelParams
 
 
 class ModelObject(ABC):
     def __init__(
         self,
         mp: ModelParams,
-        model: Model,
+        model: keras.Model,
         encoders: Dict[str, List[DataEncoder]],
         state_autoclear: int = 128,
     ) -> None:
         """
         :param mp: the model parameters
         :param model: the keras model
         :param encoders: the encoders used to encode/decode the data
@@ -200,9 +200,9 @@
         encoders_dir = model_dir / "encoders"
         with gzip.open(encoders_dir / "encoders.pk.gz", "rb") as f:
             encoders = pickle.load(f)
 
         with tf.device(device):
             custom_object_classes = [model_params_cls] + (custom_classes or [])
             custom_objects = {cls.__name__: cls for cls in custom_object_classes}
-            model = tf.keras.models.load_model(hdf5_path, custom_objects=custom_objects)
+            model = keras.models.load_model(hdf5_path, custom_objects=custom_objects)
         return cls(mp=mp, model=model, encoders=encoders)
```

## Comparing `keras_generators-1.4.4.dist-info/LICENSE` & `keras_generators-1.4.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `keras_generators-1.4.4.dist-info/METADATA` & `keras_generators-1.4.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-generators
-Version: 1.4.4
+Version: 1.4.5
 Summary: Multi-dimensional/Multi-input/Multi-output Data preprocessing and Batch Generators for Keras models
 Home-page: https://github.com/asuiu/keras-generators
 Author: Andrei Suiu
 Author-email: andrei.suiu@gmail.com
 License: Apache License 2.0
 Keywords: ML,DataGenerators,Keras,tensorflow
 Classifier: Intended Audience :: Developers
```

## Comparing `keras_generators-1.4.4.dist-info/RECORD` & `keras_generators-1.4.5.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -3,14 +3,14 @@
 keras_generators/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 keras_generators/callbacks.py,sha256=vZzvDM2vvxV0VbfSoIpvbaEZa_D9DG6_q-dffU7JJjQ,6339
 keras_generators/common.py,sha256=727hoCVFO0bs5QHHgv0R7BbGsujtTvgHNikGoKwxuM4,1471
 keras_generators/encoders.py,sha256=WwviJAdT_mYwjSIn9wqzt3-DEjLNl7jbliKC2jjlYik,10842
 keras_generators/generators.py,sha256=ZZXh0c4RPzKui0n-VVvvJQesmhc4ZRu3KIo_MqK0NMU,36073
 keras_generators/splitters.py,sha256=O7AKehcoPiQNjv1kuZWOoax-yvnjTFPuOkwLjox-qMw,4139
 keras_generators/model_abstractions/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-keras_generators/model_abstractions/model_object.py,sha256=V7wbnHfnoY6vrTyeDFGaDIbOH2SihMQTQEaybhkOjlY,8066
+keras_generators/model_abstractions/model_object.py,sha256=w6YFRQkxad9MpZfsReU7PUp3PYUdSLFulWzgr1qaLWU,8073
 keras_generators/model_abstractions/model_params.py,sha256=114iJ1gi15XEUhhU5vZnBgvfL1GY2ozhEsIiXf7rwTE,3263
-keras_generators-1.4.4.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-keras_generators-1.4.4.dist-info/METADATA,sha256=8r7VN0GxNIxhi97wUKs26IJfWQYBSxdEBekY4WUbjLE,13884
-keras_generators-1.4.4.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-keras_generators-1.4.4.dist-info/top_level.txt,sha256=6h3qtPKTpHlh7dFVHfOuDDRxVzXpjgb3hL-O3LMXK2w,26
-keras_generators-1.4.4.dist-info/RECORD,,
+keras_generators-1.4.5.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+keras_generators-1.4.5.dist-info/METADATA,sha256=d8YWObjpAi1A10lSMncryzuZlwjigpghCIG0aMGWCdM,13884
+keras_generators-1.4.5.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+keras_generators-1.4.5.dist-info/top_level.txt,sha256=6h3qtPKTpHlh7dFVHfOuDDRxVzXpjgb3hL-O3LMXK2w,26
+keras_generators-1.4.5.dist-info/RECORD,,
```

