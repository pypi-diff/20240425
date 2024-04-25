# Comparing `tmp/tf_ocr-0.1.2.tar.gz` & `tmp/tf_ocr-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tf_ocr-0.1.2.tar", last modified: Mon Apr 22 10:22:06 2024, max compression
+gzip compressed data, was "tf_ocr-0.1.3.tar", last modified: Thu Apr 25 06:57:52 2024, max compression
```

## Comparing `tf_ocr-0.1.2.tar` & `tf_ocr-0.1.3.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:22:06.449471 tf_ocr-0.1.2/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3655 2024-04-22 10:22:06.439471 tf_ocr-0.1.2/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3304 2024-03-15 09:08:54.000000 tf_ocr-0.1.2/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      494 2024-04-22 10:22:03.000000 tf_ocr-0.1.2/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-22 10:22:06.449471 tf_ocr-0.1.2/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:22:06.429471 tf_ocr-0.1.2/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:22:06.429471 tf_ocr-0.1.2/src/tf_ocr/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      325 2024-04-22 09:03:00.000000 tf_ocr-0.1.2/src/tf_ocr/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:22:06.429471 tf_ocr-0.1.2/src/tf_ocr/images/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      101 2024-04-22 09:02:59.000000 tf_ocr-0.1.2/src/tf_ocr/images/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3002 2024-04-22 09:02:46.000000 tf_ocr-0.1.2/src/tf_ocr/images/images.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:22:06.429471 tf_ocr-0.1.2/src/tf_ocr/labels/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       78 2024-03-14 04:50:41.000000 tf_ocr-0.1.2/src/tf_ocr/labels/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2367 2024-03-14 04:56:24.000000 tf_ocr-0.1.2/src/tf_ocr/labels/labels.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:22:06.429471 tf_ocr-0.1.2/src/tf_ocr/serving/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       64 2024-03-15 07:32:33.000000 tf_ocr-0.1.2/src/tf_ocr/serving/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1977 2024-03-15 09:44:36.000000 tf_ocr-0.1.2/src/tf_ocr/serving/pipeline.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:22:06.429471 tf_ocr-0.1.2/src/tf_ocr/tfrecords/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      129 2024-04-22 08:41:03.000000 tf_ocr-0.1.2/src/tf_ocr/tfrecords/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3400 2024-04-22 08:47:47.000000 tf_ocr-0.1.2/src/tf_ocr/tfrecords/datasets.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1606 2024-03-14 16:27:34.000000 tf_ocr-0.1.2/src/tf_ocr/tfrecords/examples.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:22:06.439471 tf_ocr-0.1.2/src/tf_ocr/utils/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       72 2024-03-15 08:59:17.000000 tf_ocr-0.1.2/src/tf_ocr/utils/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      694 2024-03-14 08:35:55.000000 tf_ocr-0.1.2/src/tf_ocr/utils/logits.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      820 2024-03-15 08:59:05.000000 tf_ocr-0.1.2/src/tf_ocr/utils/postprocess.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:22:06.439471 tf_ocr-0.1.2/src/tf_ocr/vocab/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       91 2024-03-13 13:27:25.000000 tf_ocr-0.1.2/src/tf_ocr/vocab/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      416 2024-03-13 13:56:11.000000 tf_ocr-0.1.2/src/tf_ocr/vocab/test_vocab.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2071 2024-04-22 05:20:12.000000 tf_ocr-0.1.2/src/tf_ocr/vocab/vocab.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:22:06.439471 tf_ocr-0.1.2/src/tf_ocr.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3655 2024-04-22 10:22:06.000000 tf_ocr-0.1.2/src/tf_ocr.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      667 2024-04-22 10:22:06.000000 tf_ocr-0.1.2/src/tf_ocr.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-22 10:22:06.000000 tf_ocr-0.1.2/src/tf_ocr.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       46 2024-04-22 10:22:06.000000 tf_ocr-0.1.2/src/tf_ocr.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        7 2024-04-22 10:22:06.000000 tf_ocr-0.1.2/src/tf_ocr.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:57:52.714238 tf_ocr-0.1.3/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3655 2024-04-25 06:57:52.714238 tf_ocr-0.1.3/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3304 2024-03-15 09:08:54.000000 tf_ocr-0.1.3/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      494 2024-04-25 06:57:50.000000 tf_ocr-0.1.3/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-25 06:57:52.714238 tf_ocr-0.1.3/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:57:52.704238 tf_ocr-0.1.3/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:57:52.704238 tf_ocr-0.1.3/src/tf_ocr/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-24 16:58:23.000000 tf_ocr-0.1.3/src/tf_ocr/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      716 2024-04-25 06:34:35.000000 tf_ocr-0.1.3/src/tf_ocr/__init__.pyi
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:57:52.704238 tf_ocr-0.1.3/src/tf_ocr/images/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      101 2024-04-22 09:02:59.000000 tf_ocr-0.1.3/src/tf_ocr/images/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3002 2024-04-22 09:02:46.000000 tf_ocr-0.1.3/src/tf_ocr/images/images.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:57:52.704238 tf_ocr-0.1.3/src/tf_ocr/labels/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       78 2024-03-14 04:50:41.000000 tf_ocr-0.1.3/src/tf_ocr/labels/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2386 2024-04-24 17:29:16.000000 tf_ocr-0.1.3/src/tf_ocr/labels/labels.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:57:52.704238 tf_ocr-0.1.3/src/tf_ocr/serving/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       64 2024-03-15 07:32:33.000000 tf_ocr-0.1.3/src/tf_ocr/serving/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1977 2024-03-15 09:44:36.000000 tf_ocr-0.1.3/src/tf_ocr/serving/pipeline.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:57:52.704238 tf_ocr-0.1.3/src/tf_ocr/tfrecords/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      169 2024-04-25 06:34:15.000000 tf_ocr-0.1.3/src/tf_ocr/tfrecords/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4609 2024-04-25 06:34:10.000000 tf_ocr-0.1.3/src/tf_ocr/tfrecords/datasets.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1606 2024-03-14 16:27:34.000000 tf_ocr-0.1.3/src/tf_ocr/tfrecords/examples.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:57:52.714238 tf_ocr-0.1.3/src/tf_ocr/utils/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       72 2024-03-15 08:59:17.000000 tf_ocr-0.1.3/src/tf_ocr/utils/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      729 2024-04-25 06:57:33.000000 tf_ocr-0.1.3/src/tf_ocr/utils/logits.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      802 2024-04-25 06:57:39.000000 tf_ocr-0.1.3/src/tf_ocr/utils/postprocess.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:57:52.714238 tf_ocr-0.1.3/src/tf_ocr/vocab/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       91 2024-03-13 13:27:25.000000 tf_ocr-0.1.3/src/tf_ocr/vocab/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      416 2024-03-13 13:56:11.000000 tf_ocr-0.1.3/src/tf_ocr/vocab/test_vocab.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2071 2024-04-22 05:20:12.000000 tf_ocr-0.1.3/src/tf_ocr/vocab/vocab.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:57:52.714238 tf_ocr-0.1.3/src/tf_ocr.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3655 2024-04-25 06:57:52.000000 tf_ocr-0.1.3/src/tf_ocr.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      691 2024-04-25 06:57:52.000000 tf_ocr-0.1.3/src/tf_ocr.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-25 06:57:52.000000 tf_ocr-0.1.3/src/tf_ocr.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       46 2024-04-25 06:57:52.000000 tf_ocr-0.1.3/src/tf_ocr.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        7 2024-04-25 06:57:52.000000 tf_ocr-0.1.3/src/tf_ocr.egg-info/top_level.txt
```

### Comparing `tf_ocr-0.1.2/PKG-INFO` & `tf_ocr-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tf-ocr
-Version: 0.1.2
+Version: 0.1.3
 Summary: Tools for OCR in tensorflow. Typed with `jaxtyping`
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: jaxtyping
 Requires-Dist: tf-ctc
 Requires-Dist: tf-tools
```

### Comparing `tf_ocr-0.1.2/README.md` & `tf_ocr-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `tf_ocr-0.1.2/src/tf_ocr/images/images.py` & `tf_ocr-0.1.3/src/tf_ocr/images/images.py`

 * *Files identical despite different names*

### Comparing `tf_ocr-0.1.2/src/tf_ocr/labels/labels.py` & `tf_ocr-0.1.3/src/tf_ocr/labels/labels.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from ..vocab import vectorize, stringify
 
 @tf_function 
 def encode(label: str | list[str], maxlen: int | None = None, char2num: StringLookup = None) -> Shaped[tf.SparseTensor, "maxlen"]:
   """Convert a label (or labels) into a valid OCR input (a batch of `SparseTensor`s)"""
   labels = [label] if isinstance(label, str) else label
   chars: tf.RaggedTensor = tf.strings.unicode_split(labels, 'UTF-8')
-  inds = vectorize(chars, char2num)
+  inds = tf.cast(vectorize(chars, char2num), tf.int32)
   if maxlen is None:
     return inds.to_sparse()
   else:
     padded = inds.to_tensor(shape=(len(labels), maxlen))
     return tf.sparse.from_dense(padded)
   
 @tf_function
```

### Comparing `tf_ocr-0.1.2/src/tf_ocr/serving/pipeline.py` & `tf_ocr-0.1.3/src/tf_ocr/serving/pipeline.py`

 * *Files identical despite different names*

### Comparing `tf_ocr-0.1.2/src/tf_ocr/tfrecords/examples.py` & `tf_ocr-0.1.3/src/tf_ocr/tfrecords/examples.py`

 * *Files identical despite different names*

### Comparing `tf_ocr-0.1.2/src/tf_ocr/utils/logits.py` & `tf_ocr-0.1.3/src/tf_ocr/utils/logits.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import tensorflow as tf
+from haskellian import iter as I
 from jaxtyping import Float
-import ramda as R
 import tf_ctc as ctc
 from ..labels import encode
 
-def mock_logits(top_preds: list[list[str]], vocabsize: int = None) -> Float[tf.Tensor, "batch 2*maxlen vocabsize"]:
+def mock_logits(top_preds: list[list[str]], vocabsize: int | None = None) -> Float[tf.Tensor, "batch 2*maxlen vocabsize"]:
   """Logits that, when CTC-decoded, will roughly follow `top_preds`
   - `len(top_preds)`: batch_size
   - `top_preds[i]`: top paths considered for each sample
   
   E.g:
   ```
   z = ocr.mock_logits([['e4', 'e5'], ['Nf6', 'Nd6']])
   paths, _ = ctc.beam_decode(logits, top_paths=2)
   [ocr.decode(p) for p in paths] # [[b'e4', b'Nf6'], [b'e5', b'Nd6']]
   ```
   """
-  labs = R.map(encode, R.transpose(top_preds))
+  labs = [encode(p) for p in I.transpose_ragged(top_preds)]
   return ctc.mock_logits(labs, vocabsize=vocabsize)
```

### Comparing `tf_ocr-0.1.2/src/tf_ocr/utils/postprocess.py` & `tf_ocr-0.1.3/src/tf_ocr/utils/postprocess.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import TypedDict
 import tensorflow as tf
 from tf_keras.layers import StringLookup
 from jaxtyping import Float
-import ramda as R
 import tf_ctc as ctc
 from tf_tools import Bytes
 from ..labels import decode_sparse
 
 class PredsProbs(TypedDict):
   preds: Bytes[tf.Tensor, "batch top_paths"]
   logprobs: Float[tf.Tensor, "batch top_paths"]
```

### Comparing `tf_ocr-0.1.2/src/tf_ocr/vocab/vocab.py` & `tf_ocr-0.1.3/src/tf_ocr/vocab/vocab.py`

 * *Files identical despite different names*

### Comparing `tf_ocr-0.1.2/src/tf_ocr.egg-info/PKG-INFO` & `tf_ocr-0.1.3/src/tf_ocr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tf-ocr
-Version: 0.1.2
+Version: 0.1.3
 Summary: Tools for OCR in tensorflow. Typed with `jaxtyping`
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: jaxtyping
 Requires-Dist: tf-ctc
 Requires-Dist: tf-tools
```

### Comparing `tf_ocr-0.1.2/src/tf_ocr.egg-info/SOURCES.txt` & `tf_ocr-0.1.3/src/tf_ocr.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 README.md
 pyproject.toml
 src/tf_ocr/__init__.py
+src/tf_ocr/__init__.pyi
 src/tf_ocr.egg-info/PKG-INFO
 src/tf_ocr.egg-info/SOURCES.txt
 src/tf_ocr.egg-info/dependency_links.txt
 src/tf_ocr.egg-info/requires.txt
 src/tf_ocr.egg-info/top_level.txt
 src/tf_ocr/images/__init__.py
 src/tf_ocr/images/images.py
```

