# Comparing `tmp/tf_ctc-0.1.4.tar.gz` & `tmp/tf_ctc-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tf_ctc-0.1.4.tar", last modified: Mon Apr 22 10:21:55 2024, max compression
+gzip compressed data, was "tf_ctc-0.1.5.tar", last modified: Thu Apr 25 07:41:21 2024, max compression
```

## Comparing `tf_ctc-0.1.4.tar` & `tf_ctc-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:21:55.669556 tf_ctc-0.1.4/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3776 2024-04-22 10:21:55.669556 tf_ctc-0.1.4/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3388 2024-03-14 10:50:47.000000 tf_ctc-0.1.4/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      519 2024-04-22 10:21:52.000000 tf_ctc-0.1.4/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-22 10:21:55.669556 tf_ctc-0.1.4/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:21:55.659556 tf_ctc-0.1.4/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:21:55.669556 tf_ctc-0.1.4/src/tf_ctc/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      187 2024-04-22 05:26:08.000000 tf_ctc-0.1.4/src/tf_ctc/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3824 2024-04-22 05:28:09.000000 tf_ctc-0.1.4/src/tf_ctc/decoding.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2780 2024-04-22 05:25:31.000000 tf_ctc-0.1.4/src/tf_ctc/logits.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      575 2024-03-14 04:43:40.000000 tf_ctc-0.1.4/src/tf_ctc/loss_.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1647 2024-04-22 05:39:27.000000 tf_ctc-0.1.4/src/tf_ctc/metrics.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      163 2024-04-22 05:25:42.000000 tf_ctc-0.1.4/src/tf_ctc/test.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:21:55.669556 tf_ctc-0.1.4/src/tf_ctc/tests/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      935 2024-03-14 06:02:21.000000 tf_ctc-0.1.4/src/tf_ctc/tests/test_decoding.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      539 2024-03-14 05:40:16.000000 tf_ctc-0.1.4/src/tf_ctc/tests/test_loss.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      897 2024-03-14 09:49:15.000000 tf_ctc-0.1.4/src/tf_ctc/tests/test_metrics.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:21:55.669556 tf_ctc-0.1.4/src/tf_ctc.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3776 2024-04-22 10:21:55.000000 tf_ctc-0.1.4/src/tf_ctc.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      418 2024-04-22 10:21:55.000000 tf_ctc-0.1.4/src/tf_ctc.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-22 10:21:55.000000 tf_ctc-0.1.4/src/tf_ctc.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       56 2024-04-22 10:21:55.000000 tf_ctc-0.1.4/src/tf_ctc.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        7 2024-04-22 10:21:55.000000 tf_ctc-0.1.4/src/tf_ctc.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:41:21.364241 tf_ctc-0.1.5/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3776 2024-04-25 07:41:21.364241 tf_ctc-0.1.5/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3388 2024-03-14 10:50:47.000000 tf_ctc-0.1.5/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      519 2024-04-25 07:41:19.000000 tf_ctc-0.1.5/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-25 07:41:21.364241 tf_ctc-0.1.5/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:41:21.354241 tf_ctc-0.1.5/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:41:21.354241 tf_ctc-0.1.5/src/tf_ctc/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      187 2024-04-22 05:26:08.000000 tf_ctc-0.1.5/src/tf_ctc/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3824 2024-04-22 05:28:09.000000 tf_ctc-0.1.5/src/tf_ctc/decoding.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2780 2024-04-22 05:25:31.000000 tf_ctc-0.1.5/src/tf_ctc/logits.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      594 2024-04-24 17:12:39.000000 tf_ctc-0.1.5/src/tf_ctc/loss_.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1647 2024-04-22 05:39:27.000000 tf_ctc-0.1.5/src/tf_ctc/metrics.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      163 2024-04-22 05:25:42.000000 tf_ctc-0.1.5/src/tf_ctc/test.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:41:21.364241 tf_ctc-0.1.5/src/tf_ctc/tests/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      935 2024-03-14 06:02:21.000000 tf_ctc-0.1.5/src/tf_ctc/tests/test_decoding.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      539 2024-03-14 05:40:16.000000 tf_ctc-0.1.5/src/tf_ctc/tests/test_loss.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      897 2024-03-14 09:49:15.000000 tf_ctc-0.1.5/src/tf_ctc/tests/test_metrics.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:41:21.364241 tf_ctc-0.1.5/src/tf_ctc.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3776 2024-04-25 07:41:21.000000 tf_ctc-0.1.5/src/tf_ctc.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      418 2024-04-25 07:41:21.000000 tf_ctc-0.1.5/src/tf_ctc.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-25 07:41:21.000000 tf_ctc-0.1.5/src/tf_ctc.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       56 2024-04-25 07:41:21.000000 tf_ctc-0.1.5/src/tf_ctc.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        7 2024-04-25 07:41:21.000000 tf_ctc-0.1.5/src/tf_ctc.egg-info/top_level.txt
```

### Comparing `tf_ctc-0.1.4/PKG-INFO` & `tf_ctc-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tf-ctc
-Version: 0.1.4
+Version: 0.1.5
 Summary: CTC with tensorflow, simplified
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: jaxtyping
 Requires-Dist: tf-tools
 Requires-Dist: tensorflow
```

### Comparing `tf_ctc-0.1.4/README.md` & `tf_ctc-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `tf_ctc-0.1.4/pyproject.toml` & `tf_ctc-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tf-ctc"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
     { name="Marcel Claramunt", email="marcel@moveread.com" }
 ]
 description = "CTC with tensorflow, simplified"
 dependencies = [
     "jaxtyping", "tf-tools", "tensorflow"
 ]
```

### Comparing `tf_ctc-0.1.4/src/tf_ctc/decoding.py` & `tf_ctc-0.1.5/src/tf_ctc/decoding.py`

 * *Files identical despite different names*

### Comparing `tf_ctc-0.1.4/src/tf_ctc/logits.py` & `tf_ctc-0.1.5/src/tf_ctc/logits.py`

 * *Files identical despite different names*

### Comparing `tf_ctc-0.1.4/src/tf_ctc/loss_.py` & `tf_ctc-0.1.5/src/tf_ctc/loss_.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,8 +8,8 @@
   logits: Float[tf.Tensor, "batch maxlen vocab"],
   blank_index: int = 0
 ) -> Float[tf.Tensor, "batch"]:
   """CTC loss. `blank_index` is the index in the vocabulary corresponding to the blank character"""
   batch = tf.shape(logits)[0]
   maxlen = tf.shape(logits)[1]
   logit_lens = tf.repeat(maxlen, batch)
-  return tf.nn.ctc_loss(labels, logits, None, logit_lens, logits_time_major=False, blank_index=blank_index)
+  return tf.nn.ctc_loss(tf.cast(labels, tf.int32), logits, None, logit_lens, logits_time_major=False, blank_index=blank_index)
```

### Comparing `tf_ctc-0.1.4/src/tf_ctc/metrics.py` & `tf_ctc-0.1.5/src/tf_ctc/metrics.py`

 * *Files identical despite different names*

### Comparing `tf_ctc-0.1.4/src/tf_ctc/tests/test_decoding.py` & `tf_ctc-0.1.5/src/tf_ctc/tests/test_decoding.py`

 * *Files identical despite different names*

### Comparing `tf_ctc-0.1.4/src/tf_ctc/tests/test_loss.py` & `tf_ctc-0.1.5/src/tf_ctc/tests/test_loss.py`

 * *Files identical despite different names*

### Comparing `tf_ctc-0.1.4/src/tf_ctc/tests/test_metrics.py` & `tf_ctc-0.1.5/src/tf_ctc/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `tf_ctc-0.1.4/src/tf_ctc.egg-info/PKG-INFO` & `tf_ctc-0.1.5/src/tf_ctc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tf-ctc
-Version: 0.1.4
+Version: 0.1.5
 Summary: CTC with tensorflow, simplified
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: jaxtyping
 Requires-Dist: tf-tools
 Requires-Dist: tensorflow
```

