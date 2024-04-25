# Comparing `tmp/tf_ocr-0.1.3.tar.gz` & `tmp/tf_ocr-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tf_ocr-0.1.3.tar", last modified: Thu Apr 25 06:57:52 2024, max compression
+gzip compressed data, was "tf_ocr-0.1.4.tar", last modified: Thu Apr 25 07:20:17 2024, max compression
```

## Comparing `tf_ocr-0.1.3.tar` & `tf_ocr-0.1.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:57:52.714238 tf_ocr-0.1.3/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3655 2024-04-25 06:57:52.714238 tf_ocr-0.1.3/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3304 2024-03-15 09:08:54.000000 tf_ocr-0.1.3/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      494 2024-04-25 06:57:50.000000 tf_ocr-0.1.3/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-25 06:57:52.714238 tf_ocr-0.1.3/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:57:52.704238 tf_ocr-0.1.3/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:57:52.704238 tf_ocr-0.1.3/src/tf_ocr/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-24 16:58:23.000000 tf_ocr-0.1.3/src/tf_ocr/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      716 2024-04-25 06:34:35.000000 tf_ocr-0.1.3/src/tf_ocr/__init__.pyi
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:57:52.704238 tf_ocr-0.1.3/src/tf_ocr/images/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      101 2024-04-22 09:02:59.000000 tf_ocr-0.1.3/src/tf_ocr/images/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3002 2024-04-22 09:02:46.000000 tf_ocr-0.1.3/src/tf_ocr/images/images.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:57:52.704238 tf_ocr-0.1.3/src/tf_ocr/labels/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       78 2024-03-14 04:50:41.000000 tf_ocr-0.1.3/src/tf_ocr/labels/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2386 2024-04-24 17:29:16.000000 tf_ocr-0.1.3/src/tf_ocr/labels/labels.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:57:52.704238 tf_ocr-0.1.3/src/tf_ocr/serving/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       64 2024-03-15 07:32:33.000000 tf_ocr-0.1.3/src/tf_ocr/serving/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1977 2024-03-15 09:44:36.000000 tf_ocr-0.1.3/src/tf_ocr/serving/pipeline.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:57:52.704238 tf_ocr-0.1.3/src/tf_ocr/tfrecords/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      169 2024-04-25 06:34:15.000000 tf_ocr-0.1.3/src/tf_ocr/tfrecords/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4609 2024-04-25 06:34:10.000000 tf_ocr-0.1.3/src/tf_ocr/tfrecords/datasets.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1606 2024-03-14 16:27:34.000000 tf_ocr-0.1.3/src/tf_ocr/tfrecords/examples.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:57:52.714238 tf_ocr-0.1.3/src/tf_ocr/utils/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       72 2024-03-15 08:59:17.000000 tf_ocr-0.1.3/src/tf_ocr/utils/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      729 2024-04-25 06:57:33.000000 tf_ocr-0.1.3/src/tf_ocr/utils/logits.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      802 2024-04-25 06:57:39.000000 tf_ocr-0.1.3/src/tf_ocr/utils/postprocess.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:57:52.714238 tf_ocr-0.1.3/src/tf_ocr/vocab/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       91 2024-03-13 13:27:25.000000 tf_ocr-0.1.3/src/tf_ocr/vocab/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      416 2024-03-13 13:56:11.000000 tf_ocr-0.1.3/src/tf_ocr/vocab/test_vocab.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2071 2024-04-22 05:20:12.000000 tf_ocr-0.1.3/src/tf_ocr/vocab/vocab.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:57:52.714238 tf_ocr-0.1.3/src/tf_ocr.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3655 2024-04-25 06:57:52.000000 tf_ocr-0.1.3/src/tf_ocr.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      691 2024-04-25 06:57:52.000000 tf_ocr-0.1.3/src/tf_ocr.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-25 06:57:52.000000 tf_ocr-0.1.3/src/tf_ocr.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       46 2024-04-25 06:57:52.000000 tf_ocr-0.1.3/src/tf_ocr.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        7 2024-04-25 06:57:52.000000 tf_ocr-0.1.3/src/tf_ocr.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:20:17.954235 tf_ocr-0.1.4/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3688 2024-04-25 07:20:17.954235 tf_ocr-0.1.4/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3304 2024-03-15 09:08:54.000000 tf_ocr-0.1.4/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      515 2024-04-25 07:20:14.000000 tf_ocr-0.1.4/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-25 07:20:17.954235 tf_ocr-0.1.4/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:20:17.944235 tf_ocr-0.1.4/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:20:17.954235 tf_ocr-0.1.4/src/tf_ocr/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-24 16:58:23.000000 tf_ocr-0.1.4/src/tf_ocr/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      716 2024-04-25 06:34:35.000000 tf_ocr-0.1.4/src/tf_ocr/__init__.pyi
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:20:17.954235 tf_ocr-0.1.4/src/tf_ocr/images/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      101 2024-04-22 09:02:59.000000 tf_ocr-0.1.4/src/tf_ocr/images/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3002 2024-04-22 09:02:46.000000 tf_ocr-0.1.4/src/tf_ocr/images/images.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:20:17.954235 tf_ocr-0.1.4/src/tf_ocr/labels/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       78 2024-03-14 04:50:41.000000 tf_ocr-0.1.4/src/tf_ocr/labels/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2386 2024-04-24 17:29:16.000000 tf_ocr-0.1.4/src/tf_ocr/labels/labels.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:20:17.954235 tf_ocr-0.1.4/src/tf_ocr/serving/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       64 2024-03-15 07:32:33.000000 tf_ocr-0.1.4/src/tf_ocr/serving/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1977 2024-03-15 09:44:36.000000 tf_ocr-0.1.4/src/tf_ocr/serving/pipeline.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:20:17.954235 tf_ocr-0.1.4/src/tf_ocr/tfrecords/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      169 2024-04-25 06:34:15.000000 tf_ocr-0.1.4/src/tf_ocr/tfrecords/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4620 2024-04-25 07:03:46.000000 tf_ocr-0.1.4/src/tf_ocr/tfrecords/datasets.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1606 2024-03-14 16:27:34.000000 tf_ocr-0.1.4/src/tf_ocr/tfrecords/examples.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:20:17.954235 tf_ocr-0.1.4/src/tf_ocr/utils/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       72 2024-03-15 08:59:17.000000 tf_ocr-0.1.4/src/tf_ocr/utils/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      729 2024-04-25 06:57:33.000000 tf_ocr-0.1.4/src/tf_ocr/utils/logits.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      802 2024-04-25 06:57:39.000000 tf_ocr-0.1.4/src/tf_ocr/utils/postprocess.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:20:17.954235 tf_ocr-0.1.4/src/tf_ocr/vocab/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       91 2024-03-13 13:27:25.000000 tf_ocr-0.1.4/src/tf_ocr/vocab/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      416 2024-03-13 13:56:11.000000 tf_ocr-0.1.4/src/tf_ocr/vocab/test_vocab.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2071 2024-04-22 05:20:12.000000 tf_ocr-0.1.4/src/tf_ocr/vocab/vocab.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:20:17.954235 tf_ocr-0.1.4/src/tf_ocr.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3688 2024-04-25 07:20:17.000000 tf_ocr-0.1.4/src/tf_ocr.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      691 2024-04-25 07:20:17.000000 tf_ocr-0.1.4/src/tf_ocr.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-25 07:20:17.000000 tf_ocr-0.1.4/src/tf_ocr.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       64 2024-04-25 07:20:17.000000 tf_ocr-0.1.4/src/tf_ocr.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        7 2024-04-25 07:20:17.000000 tf_ocr-0.1.4/src/tf_ocr.egg-info/top_level.txt
```

### Comparing `tf_ocr-0.1.3/PKG-INFO` & `tf_ocr-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: tf-ocr
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tools for OCR in tensorflow. Typed with `jaxtyping`
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: jaxtyping
 Requires-Dist: tf-ctc
 Requires-Dist: tf-tools
 Requires-Dist: tensorflow
 Requires-Dist: tf-keras
+Requires-Dist: typing-extensions
 
 # TensorFlow OCR
 
 > Tools to simplify dealing with OCR labels, predictions, models
 
 ## Pre/post processing
```

### Comparing `tf_ocr-0.1.3/README.md` & `tf_ocr-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `tf_ocr-0.1.3/src/tf_ocr/__init__.pyi` & `tf_ocr-0.1.4/src/tf_ocr/__init__.pyi`

 * *Files identical despite different names*

### Comparing `tf_ocr-0.1.3/src/tf_ocr/images/images.py` & `tf_ocr-0.1.4/src/tf_ocr/images/images.py`

 * *Files identical despite different names*

### Comparing `tf_ocr-0.1.3/src/tf_ocr/labels/labels.py` & `tf_ocr-0.1.4/src/tf_ocr/labels/labels.py`

 * *Files identical despite different names*

### Comparing `tf_ocr-0.1.3/src/tf_ocr/serving/pipeline.py` & `tf_ocr-0.1.4/src/tf_ocr/serving/pipeline.py`

 * *Files identical despite different names*

### Comparing `tf_ocr-0.1.3/src/tf_ocr/tfrecords/datasets.py` & `tf_ocr-0.1.4/src/tf_ocr/tfrecords/datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Callable, Literal, AsyncIterable, Sequence, TypedDict, Unpack, NotRequired
+from typing_extensions import Callable, Literal, AsyncIterable, Sequence, TypedDict, Unpack, NotRequired
 from functools import partial
 import os
 import time
 from haskellian import kwargs as kw
 import tensorflow as tf
 import keras
 from .examples import deserialize, serialize
```

### Comparing `tf_ocr-0.1.3/src/tf_ocr/tfrecords/examples.py` & `tf_ocr-0.1.4/src/tf_ocr/tfrecords/examples.py`

 * *Files identical despite different names*

### Comparing `tf_ocr-0.1.3/src/tf_ocr/utils/logits.py` & `tf_ocr-0.1.4/src/tf_ocr/utils/logits.py`

 * *Files identical despite different names*

### Comparing `tf_ocr-0.1.3/src/tf_ocr/utils/postprocess.py` & `tf_ocr-0.1.4/src/tf_ocr/utils/postprocess.py`

 * *Files identical despite different names*

### Comparing `tf_ocr-0.1.3/src/tf_ocr/vocab/vocab.py` & `tf_ocr-0.1.4/src/tf_ocr/vocab/vocab.py`

 * *Files identical despite different names*

### Comparing `tf_ocr-0.1.3/src/tf_ocr.egg-info/PKG-INFO` & `tf_ocr-0.1.4/src/tf_ocr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: tf-ocr
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tools for OCR in tensorflow. Typed with `jaxtyping`
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: jaxtyping
 Requires-Dist: tf-ctc
 Requires-Dist: tf-tools
 Requires-Dist: tensorflow
 Requires-Dist: tf-keras
+Requires-Dist: typing-extensions
 
 # TensorFlow OCR
 
 > Tools to simplify dealing with OCR labels, predictions, models
 
 ## Pre/post processing
```

### Comparing `tf_ocr-0.1.3/src/tf_ocr.egg-info/SOURCES.txt` & `tf_ocr-0.1.4/src/tf_ocr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

