# Comparing `tmp/supert5-0.0.2.tar.gz` & `tmp/supert5-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "supert5-0.0.3.tar", max compression
```

## Comparing `supert5-0.0.2.tar` & `supert5-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,21 @@
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 supert5-0.0.2/README.md
--rw-r--r--   0        0        0    66416 2020-02-02 00:00:00.000000 supert5-0.0.2/images/forwardpass_benchmarking.png
--rw-r--r--   0        0        0    66248 2020-02-02 00:00:00.000000 supert5-0.0.2/images/memory_benchmarking.png
--rw-r--r--   0        0        0    52665 2020-02-02 00:00:00.000000 supert5-0.0.2/images/speedup_benchmarking.png
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 supert5-0.0.2/src/superT5/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 supert5-0.0.2/src/superT5/heads/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 supert5-0.0.2/src/superT5/heads/decoder_heds.py
--rw-r--r--   0        0        0    10997 2020-02-02 00:00:00.000000 supert5-0.0.2/src/superT5/heads/encoder_heads.py
--rw-r--r--   0        0        0    34038 2020-02-02 00:00:00.000000 supert5-0.0.2/src/superT5/heads/t5_heads.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 supert5-0.0.2/src/superT5/model/__init__.py
--rw-r--r--   0        0        0    49182 2020-02-02 00:00:00.000000 supert5-0.0.2/src/superT5/model/attentions.py
--rw-r--r--   0        0        0     8159 2020-02-02 00:00:00.000000 supert5-0.0.2/src/superT5/model/config.py
--rw-r--r--   0        0        0    40800 2020-02-02 00:00:00.000000 supert5-0.0.2/src/superT5/model/modeling.py
--rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 supert5-0.0.2/src/superT5/model/modules.py
--rw-r--r--   0        0        0    13016 2020-02-02 00:00:00.000000 supert5-0.0.2/src/superT5/model/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 supert5-0.0.2/src/superT5/ops/__init__.py
--rw-r--r--   0        0        0     7893 2020-02-02 00:00:00.000000 supert5-0.0.2/src/superT5/ops/attention_bias.py
--rw-r--r--   0        0        0    32478 2020-02-02 00:00:00.000000 supert5-0.0.2/src/superT5/ops/flash_attention.py
--rw-r--r--   0        0        0    33884 2020-02-02 00:00:00.000000 supert5-0.0.2/src/superT5/ops/fused_bias_attention.py
--rw-r--r--   0        0        0    21361 2020-02-02 00:00:00.000000 supert5-0.0.2/src/superT5/ops/gated_mlp.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 supert5-0.0.2/src/superT5/ops/naive_attention.py
--rw-r--r--   0        0        0     6487 2020-02-02 00:00:00.000000 supert5-0.0.2/src/superT5/ops/rms_norm.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 supert5-0.0.2/tests/test_attentions.py
--rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 supert5-0.0.2/tests/test_generation.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 supert5-0.0.2/tests/test_rms_norm.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 supert5-0.0.2/.gitignore
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 supert5-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 supert5-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     5326 2024-04-25 09:12:53.444969 supert5-0.0.3/README.md
+-rw-r--r--   0        0        0      372 2024-04-25 09:30:56.519950 supert5-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      341 2024-04-25 08:27:50.294134 supert5-0.0.3/src/supert5/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 08:27:50.294134 supert5-0.0.3/src/supert5/heads/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 08:27:50.294134 supert5-0.0.3/src/supert5/heads/decoder_heds.py
+-rw-r--r--   0        0        0    10997 2024-04-25 08:27:50.294134 supert5-0.0.3/src/supert5/heads/encoder_heads.py
+-rw-r--r--   0        0        0    34038 2024-04-25 08:27:50.294134 supert5-0.0.3/src/supert5/heads/t5_heads.py
+-rw-r--r--   0        0        0        0 2024-04-25 08:27:50.298134 supert5-0.0.3/src/supert5/model/__init__.py
+-rw-r--r--   0        0        0    49182 2024-04-25 09:12:18.881487 supert5-0.0.3/src/supert5/model/attentions.py
+-rw-r--r--   0        0        0     8159 2024-04-25 08:27:50.298134 supert5-0.0.3/src/supert5/model/config.py
+-rw-r--r--   0        0        0    40800 2024-04-25 09:12:14.929547 supert5-0.0.3/src/supert5/model/modeling.py
+-rw-r--r--   0        0        0     3938 2024-04-25 08:27:50.298134 supert5-0.0.3/src/supert5/model/modules.py
+-rw-r--r--   0        0        0    13016 2024-04-25 08:27:50.298134 supert5-0.0.3/src/supert5/model/utils.py
+-rw-r--r--   0        0        0        0 2024-04-25 08:27:50.298134 supert5-0.0.3/src/supert5/ops/__init__.py
+-rw-r--r--   0        0        0     7893 2024-04-25 08:27:50.298134 supert5-0.0.3/src/supert5/ops/attention_bias.py
+-rw-r--r--   0        0        0    32478 2024-04-25 08:29:35.982790 supert5-0.0.3/src/supert5/ops/flash_attention.py
+-rw-r--r--   0        0        0    33884 2024-04-25 08:28:40.454478 supert5-0.0.3/src/supert5/ops/fused_bias_attention.py
+-rw-r--r--   0        0        0    21361 2024-04-25 08:27:50.302134 supert5-0.0.3/src/supert5/ops/gated_mlp.py
+-rw-r--r--   0        0        0      790 2024-04-25 08:27:50.302134 supert5-0.0.3/src/supert5/ops/naive_attention.py
+-rw-r--r--   0        0        0     6487 2024-04-25 08:27:50.302134 supert5-0.0.3/src/supert5/ops/rms_norm.py
+-rw-r--r--   0        0        0     5908 1970-01-01 00:00:00.000000 supert5-0.0.3/PKG-INFO
```

### Comparing `supert5-0.0.2/README.md` & `supert5-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `supert5-0.0.2/src/superT5/heads/encoder_heads.py` & `supert5-0.0.3/src/supert5/heads/encoder_heads.py`

 * *Files identical despite different names*

### Comparing `supert5-0.0.2/src/superT5/heads/t5_heads.py` & `supert5-0.0.3/src/supert5/heads/t5_heads.py`

 * *Files identical despite different names*

### Comparing `supert5-0.0.2/src/superT5/model/attentions.py` & `supert5-0.0.3/src/supert5/model/attentions.py`

 * *Files identical despite different names*

### Comparing `supert5-0.0.2/src/superT5/model/config.py` & `supert5-0.0.3/src/supert5/model/config.py`

 * *Files identical despite different names*

### Comparing `supert5-0.0.2/src/superT5/model/modeling.py` & `supert5-0.0.3/src/supert5/model/modeling.py`

 * *Files identical despite different names*

### Comparing `supert5-0.0.2/src/superT5/model/modules.py` & `supert5-0.0.3/src/supert5/model/modules.py`

 * *Files identical despite different names*

### Comparing `supert5-0.0.2/src/superT5/model/utils.py` & `supert5-0.0.3/src/supert5/model/utils.py`

 * *Files identical despite different names*

### Comparing `supert5-0.0.2/src/superT5/ops/attention_bias.py` & `supert5-0.0.3/src/supert5/ops/attention_bias.py`

 * *Files identical despite different names*

### Comparing `supert5-0.0.2/src/superT5/ops/flash_attention.py` & `supert5-0.0.3/src/supert5/ops/flash_attention.py`

 * *Files identical despite different names*

### Comparing `supert5-0.0.2/src/superT5/ops/fused_bias_attention.py` & `supert5-0.0.3/src/supert5/ops/fused_bias_attention.py`

 * *Files identical despite different names*

### Comparing `supert5-0.0.2/src/superT5/ops/gated_mlp.py` & `supert5-0.0.3/src/supert5/ops/gated_mlp.py`

 * *Files identical despite different names*

### Comparing `supert5-0.0.2/src/superT5/ops/naive_attention.py` & `supert5-0.0.3/src/supert5/ops/naive_attention.py`

 * *Files identical despite different names*

### Comparing `supert5-0.0.2/src/superT5/ops/rms_norm.py` & `supert5-0.0.3/src/supert5/ops/rms_norm.py`

 * *Files identical despite different names*

