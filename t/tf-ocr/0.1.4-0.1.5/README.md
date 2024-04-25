# Comparing `tmp/tf_ocr-0.1.4.tar.gz` & `tmp/tf_ocr-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tf_ocr-0.1.4.tar", last modified: Thu Apr 25 07:20:17 2024, max compression
+gzip compressed data, was "tf_ocr-0.1.5.tar", last modified: Thu Apr 25 14:34:18 2024, max compression
```

## Comparing `tf_ocr-0.1.4.tar` & `tf_ocr-0.1.5.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:20:17.954235 tf_ocr-0.1.4/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3688 2024-04-25 07:20:17.954235 tf_ocr-0.1.4/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3304 2024-03-15 09:08:54.000000 tf_ocr-0.1.4/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      515 2024-04-25 07:20:14.000000 tf_ocr-0.1.4/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-25 07:20:17.954235 tf_ocr-0.1.4/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:20:17.944235 tf_ocr-0.1.4/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:20:17.954235 tf_ocr-0.1.4/src/tf_ocr/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-24 16:58:23.000000 tf_ocr-0.1.4/src/tf_ocr/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      716 2024-04-25 06:34:35.000000 tf_ocr-0.1.4/src/tf_ocr/__init__.pyi
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:20:17.954235 tf_ocr-0.1.4/src/tf_ocr/images/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      101 2024-04-22 09:02:59.000000 tf_ocr-0.1.4/src/tf_ocr/images/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3002 2024-04-22 09:02:46.000000 tf_ocr-0.1.4/src/tf_ocr/images/images.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:20:17.954235 tf_ocr-0.1.4/src/tf_ocr/labels/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       78 2024-03-14 04:50:41.000000 tf_ocr-0.1.4/src/tf_ocr/labels/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2386 2024-04-24 17:29:16.000000 tf_ocr-0.1.4/src/tf_ocr/labels/labels.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:20:17.954235 tf_ocr-0.1.4/src/tf_ocr/serving/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       64 2024-03-15 07:32:33.000000 tf_ocr-0.1.4/src/tf_ocr/serving/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1977 2024-03-15 09:44:36.000000 tf_ocr-0.1.4/src/tf_ocr/serving/pipeline.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:20:17.954235 tf_ocr-0.1.4/src/tf_ocr/tfrecords/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      169 2024-04-25 06:34:15.000000 tf_ocr-0.1.4/src/tf_ocr/tfrecords/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4620 2024-04-25 07:03:46.000000 tf_ocr-0.1.4/src/tf_ocr/tfrecords/datasets.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1606 2024-03-14 16:27:34.000000 tf_ocr-0.1.4/src/tf_ocr/tfrecords/examples.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:20:17.954235 tf_ocr-0.1.4/src/tf_ocr/utils/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       72 2024-03-15 08:59:17.000000 tf_ocr-0.1.4/src/tf_ocr/utils/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      729 2024-04-25 06:57:33.000000 tf_ocr-0.1.4/src/tf_ocr/utils/logits.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      802 2024-04-25 06:57:39.000000 tf_ocr-0.1.4/src/tf_ocr/utils/postprocess.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:20:17.954235 tf_ocr-0.1.4/src/tf_ocr/vocab/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       91 2024-03-13 13:27:25.000000 tf_ocr-0.1.4/src/tf_ocr/vocab/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      416 2024-03-13 13:56:11.000000 tf_ocr-0.1.4/src/tf_ocr/vocab/test_vocab.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2071 2024-04-22 05:20:12.000000 tf_ocr-0.1.4/src/tf_ocr/vocab/vocab.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:20:17.954235 tf_ocr-0.1.4/src/tf_ocr.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3688 2024-04-25 07:20:17.000000 tf_ocr-0.1.4/src/tf_ocr.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      691 2024-04-25 07:20:17.000000 tf_ocr-0.1.4/src/tf_ocr.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-25 07:20:17.000000 tf_ocr-0.1.4/src/tf_ocr.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       64 2024-04-25 07:20:17.000000 tf_ocr-0.1.4/src/tf_ocr.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        7 2024-04-25 07:20:17.000000 tf_ocr-0.1.4/src/tf_ocr.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 14:34:18.085647 tf_ocr-0.1.5/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3688 2024-04-25 14:34:18.085647 tf_ocr-0.1.5/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3304 2024-03-15 09:08:54.000000 tf_ocr-0.1.5/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      515 2024-04-25 14:34:14.000000 tf_ocr-0.1.5/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-25 14:34:18.085647 tf_ocr-0.1.5/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 14:34:18.075646 tf_ocr-0.1.5/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 14:34:18.085647 tf_ocr-0.1.5/src/tf_ocr/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-24 16:58:23.000000 tf_ocr-0.1.5/src/tf_ocr/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      716 2024-04-25 06:34:35.000000 tf_ocr-0.1.5/src/tf_ocr/__init__.pyi
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 14:34:18.085647 tf_ocr-0.1.5/src/tf_ocr/images/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      101 2024-04-22 09:02:59.000000 tf_ocr-0.1.5/src/tf_ocr/images/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3002 2024-04-22 09:02:46.000000 tf_ocr-0.1.5/src/tf_ocr/images/images.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 14:34:18.085647 tf_ocr-0.1.5/src/tf_ocr/labels/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       78 2024-03-14 04:50:41.000000 tf_ocr-0.1.5/src/tf_ocr/labels/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2386 2024-04-24 17:29:16.000000 tf_ocr-0.1.5/src/tf_ocr/labels/labels.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 14:34:18.085647 tf_ocr-0.1.5/src/tf_ocr/serving/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       64 2024-03-15 07:32:33.000000 tf_ocr-0.1.5/src/tf_ocr/serving/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1977 2024-03-15 09:44:36.000000 tf_ocr-0.1.5/src/tf_ocr/serving/pipeline.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 14:34:18.085647 tf_ocr-0.1.5/src/tf_ocr/tfrecords/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-25 10:21:09.000000 tf_ocr-0.1.5/src/tf_ocr/tfrecords/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      355 2024-04-25 10:21:03.000000 tf_ocr-0.1.5/src/tf_ocr/tfrecords/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4405 2024-04-25 14:26:59.000000 tf_ocr-0.1.5/src/tf_ocr/tfrecords/datasets.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1606 2024-04-25 10:17:45.000000 tf_ocr-0.1.5/src/tf_ocr/tfrecords/examples.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      601 2024-04-25 10:15:00.000000 tf_ocr-0.1.5/src/tf_ocr/tfrecords/params.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      636 2024-04-25 10:15:18.000000 tf_ocr-0.1.5/src/tf_ocr/tfrecords/params.pyi
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 14:34:18.085647 tf_ocr-0.1.5/src/tf_ocr/utils/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       72 2024-03-15 08:59:17.000000 tf_ocr-0.1.5/src/tf_ocr/utils/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      729 2024-04-25 06:57:33.000000 tf_ocr-0.1.5/src/tf_ocr/utils/logits.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      802 2024-04-25 06:57:39.000000 tf_ocr-0.1.5/src/tf_ocr/utils/postprocess.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 14:34:18.085647 tf_ocr-0.1.5/src/tf_ocr/vocab/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       91 2024-03-13 13:27:25.000000 tf_ocr-0.1.5/src/tf_ocr/vocab/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      416 2024-03-13 13:56:11.000000 tf_ocr-0.1.5/src/tf_ocr/vocab/test_vocab.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2071 2024-04-22 05:20:12.000000 tf_ocr-0.1.5/src/tf_ocr/vocab/vocab.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 14:34:18.085647 tf_ocr-0.1.5/src/tf_ocr.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3688 2024-04-25 14:34:18.000000 tf_ocr-0.1.5/src/tf_ocr.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      788 2024-04-25 14:34:18.000000 tf_ocr-0.1.5/src/tf_ocr.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-25 14:34:18.000000 tf_ocr-0.1.5/src/tf_ocr.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       64 2024-04-25 14:34:18.000000 tf_ocr-0.1.5/src/tf_ocr.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        7 2024-04-25 14:34:18.000000 tf_ocr-0.1.5/src/tf_ocr.egg-info/top_level.txt
```

### Comparing `tf_ocr-0.1.4/PKG-INFO` & `tf_ocr-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tf-ocr
-Version: 0.1.4
+Version: 0.1.5
 Summary: Tools for OCR in tensorflow. Typed with `jaxtyping`
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: jaxtyping
 Requires-Dist: tf-ctc
 Requires-Dist: tf-tools
```

### Comparing `tf_ocr-0.1.4/README.md` & `tf_ocr-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `tf_ocr-0.1.4/pyproject.toml` & `tf_ocr-0.1.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tf-ocr"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
     { name="Marcel Claramunt", email="marcel@moveread.com" }
 ]
 description = "Tools for OCR in tensorflow. Typed with `jaxtyping`"
 dependencies = [
     "jaxtyping", "tf-ctc", "tf-tools",
     "tensorflow", "tf-keras", "typing-extensions"
```

### Comparing `tf_ocr-0.1.4/src/tf_ocr/__init__.pyi` & `tf_ocr-0.1.5/src/tf_ocr/__init__.pyi`

 * *Files identical despite different names*

### Comparing `tf_ocr-0.1.4/src/tf_ocr/images/images.py` & `tf_ocr-0.1.5/src/tf_ocr/images/images.py`

 * *Files identical despite different names*

### Comparing `tf_ocr-0.1.4/src/tf_ocr/labels/labels.py` & `tf_ocr-0.1.5/src/tf_ocr/labels/labels.py`

 * *Files identical despite different names*

### Comparing `tf_ocr-0.1.4/src/tf_ocr/serving/pipeline.py` & `tf_ocr-0.1.5/src/tf_ocr/serving/pipeline.py`

 * *Files identical despite different names*

### Comparing `tf_ocr-0.1.4/src/tf_ocr/tfrecords/datasets.py` & `tf_ocr-0.1.5/src/tf_ocr/tfrecords/datasets.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,45 @@
 from typing_extensions import Callable, Literal, AsyncIterable, Sequence, TypedDict, Unpack, NotRequired
 from functools import partial
 import os
 import time
 from haskellian import kwargs as kw
 import tensorflow as tf
-import keras
+import fs
 from .examples import deserialize, serialize
 from ..labels import encode
+from .params import EncodeParams, _ReadParams, DeserializeParams, ProcessParams
 
 Dataset = tf.data.Dataset
 
-class DeserializeParams(TypedDict):
-  keep_order: NotRequired[bool]
-  compression: NotRequired[Literal['ZLIB', 'GZIP'] | None]
-
 def deserialize_dataset(
   filenames: Sequence[str], *,
   keep_order: bool = False,
-  compression: Literal['ZLIB', 'GZIP'] | None = None
-) -> tf.data.TFRecordDataset:
+  compression: Literal['ZLIB', 'GZIP'] | None = 'GZIP'
+) -> tf.data.Dataset:
   """Parse a series of TFRecord files into a `tf.data.TFRecordDataset`
   - Each element is of type `ocr.tfrecords.Example`
   - Note: use `read_dataset` for a ready-to-train dataset
   """
   ignore_order = tf.data.Options()
   ignore_order.experimental_deterministic = keep_order
   return (
     tf.data.TFRecordDataset(filenames, compression_type=compression, num_parallel_reads=tf.data.AUTOTUNE)
     .with_options(ignore_order)
     .map(deserialize, num_parallel_calls=tf.data.AUTOTUNE)
   )
 
-class EncodeParams(TypedDict):
-  maxlen: NotRequired[int | None]
-  char2num: NotRequired[keras.layers.StringLookup | None]
-
-class ProcessParams(EncodeParams):
-  remove_checks: NotRequired[bool]
-
 def process_batch(batch: dict[str, tf.Tensor], remove_checks: bool = True, **p: Unpack[EncodeParams]) -> tuple[tf.Tensor, tf.SparseTensor]:
   lab = tf.strings.regex_replace(batch["label"], "[\+#]", "") if remove_checks else batch["label"]
-  return batch["image"], tf.cast(encode(lab, **p), tf.int32)
-
-class _ReadParams(ProcessParams, DeserializeParams):
-  ...
-
-class ReadParams(_ReadParams):
-  batch_size: NotRequired[int]
-  shuffle_size: NotRequired[float | None]
-  cache_files: NotRequired[str | None]
-  prefetch: NotRequired[bool]
+  return batch["image"], tf.cast(encode(lab, **p), tf.int32) # type: ignore
 
 def read_dataset(
   filenames: list[str], *, batch_size: int = 32, shuffle_size: float | None = 1e3,
   cache_file: str | None = '', prefetch: bool = True, **p: Unpack[_ReadParams]
-) -> tf.data.TFRecordDataset:
+) -> tf.data.Dataset:
   """Parse and preprocess a series of TFRecord files. Returns `(img, sparse_label)` batches
   - `shuffle_size`: if set to `None`, disables shuffling
   - `cache_file`: the default `''` caches in memory; `None` disables caching
   - `remove_checks`: whether to remove `'#'` and `'+'` symbols from the labels. Defaults to `True`
   """
   deserialize_params, process_params = kw.split(DeserializeParams, ProcessParams, p)
   ds = (
@@ -75,21 +56,22 @@
   
   return ds
 
 
 async def serialize_datasets(
   output_dir: str,
   datasets: AsyncIterable[tf.data.Dataset],
-  serialize: Callable[[dict|tuple], bytes] = serialize,
+  serialize: Callable[[dict|tuple], str] = serialize, # type: ignore
   num_batches: int | None = None, max_file_size: int = 1024*1024*100,
   filename: Callable[[int], str] = lambda i: f'data_{i}.tfrecord',
-  exist_ok: bool = False
+  exist_ok: bool = False, compress: bool = True
 ):
   """Serialize a `dataset` into a series of TFRecord files
   - `dataset`: sequence of samples of type `T`
+  - `num_batches`: number of batches of the dataset (for ETA estimation)
   - `serialize :: T -> bytes`: serializes a sample into TFRecord format, e.g. using `tf.train.Example.SerializeToString`
   - `max_file_size`: in bytes. Defaults to `100MB`
   """
   os.makedirs(output_dir, exist_ok=exist_ok)
   current_file_size = 0
   file_index = 0
   tfrecord_filename = os.path.join(output_dir, f'data_{file_index}.tfrecord')
@@ -106,21 +88,25 @@
         n_left = n - i - 1
         eta = t_mean*n_left
         msg = f"\r{i+1} / {n} [{(i+1)/n*100:.2f}%] - elapsed {t1-t0:.1f} secs - eta {eta:.1f} secs = {eta/3600:.2f} hours"
       else:
         msg = f"\r{i+1} / unknown - elapsed {t1-t0:.1f} secs"
       
       print(msg, end="", flush=True)
-      serialized_example = serialize(x)
+      serialized_example = serialize(x) # type: ignore
       example_size = len(serialized_example)
       
       if current_file_size + example_size > max_file_size:
         writer.close()
+        if compress:
+          fs.gzcompress(tfrecord_filename, keep=False)
         file_index += 1
         tfrecord_filename = os.path.join(output_dir, filename(file_index))
         current_file_size = 0
         writer = tf.io.TFRecordWriter(tfrecord_filename)
 
       writer.write(serialized_example)
       current_file_size += example_size
       i += 1
-  writer.close()
+  writer.close()
+  if compress:
+    fs.gzcompress(tfrecord_filename, keep=False)
```

### Comparing `tf_ocr-0.1.4/src/tf_ocr/tfrecords/examples.py` & `tf_ocr-0.1.5/src/tf_ocr/tfrecords/examples.py`

 * *Files identical despite different names*

### Comparing `tf_ocr-0.1.4/src/tf_ocr/utils/logits.py` & `tf_ocr-0.1.5/src/tf_ocr/utils/logits.py`

 * *Files identical despite different names*

### Comparing `tf_ocr-0.1.4/src/tf_ocr/utils/postprocess.py` & `tf_ocr-0.1.5/src/tf_ocr/utils/postprocess.py`

 * *Files identical despite different names*

### Comparing `tf_ocr-0.1.4/src/tf_ocr/vocab/vocab.py` & `tf_ocr-0.1.5/src/tf_ocr/vocab/vocab.py`

 * *Files identical despite different names*

### Comparing `tf_ocr-0.1.4/src/tf_ocr.egg-info/PKG-INFO` & `tf_ocr-0.1.5/src/tf_ocr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tf-ocr
-Version: 0.1.4
+Version: 0.1.5
 Summary: Tools for OCR in tensorflow. Typed with `jaxtyping`
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: jaxtyping
 Requires-Dist: tf-ctc
 Requires-Dist: tf-tools
```

### Comparing `tf_ocr-0.1.4/src/tf_ocr.egg-info/SOURCES.txt` & `tf_ocr-0.1.5/src/tf_ocr.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -10,15 +10,18 @@
 src/tf_ocr/images/__init__.py
 src/tf_ocr/images/images.py
 src/tf_ocr/labels/__init__.py
 src/tf_ocr/labels/labels.py
 src/tf_ocr/serving/__init__.py
 src/tf_ocr/serving/pipeline.py
 src/tf_ocr/tfrecords/__init__.py
+src/tf_ocr/tfrecords/__init__.pyi
 src/tf_ocr/tfrecords/datasets.py
 src/tf_ocr/tfrecords/examples.py
+src/tf_ocr/tfrecords/params.py
+src/tf_ocr/tfrecords/params.pyi
 src/tf_ocr/utils/__init__.py
 src/tf_ocr/utils/logits.py
 src/tf_ocr/utils/postprocess.py
 src/tf_ocr/vocab/__init__.py
 src/tf_ocr/vocab/test_vocab.py
 src/tf_ocr/vocab/vocab.py
```

