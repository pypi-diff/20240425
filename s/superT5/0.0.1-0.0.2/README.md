# Comparing `tmp/supert5-0.0.1.tar.gz` & `tmp/supert5-0.0.2.tar.gz`

## Comparing `supert5-0.0.1.tar` & `supert5-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 supert5-0.0.1/README.md
--rw-r--r--   0        0        0    66416 2020-02-02 00:00:00.000000 supert5-0.0.1/images/forwardpass_benchmarking.png
--rw-r--r--   0        0        0    66248 2020-02-02 00:00:00.000000 supert5-0.0.1/images/memory_benchmarking.png
--rw-r--r--   0        0        0    52665 2020-02-02 00:00:00.000000 supert5-0.0.1/images/speedup_benchmarking.png
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 supert5-0.0.1/src/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 supert5-0.0.1/src/heads/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 supert5-0.0.1/src/heads/decoder_heds.py
--rw-r--r--   0        0        0    10997 2020-02-02 00:00:00.000000 supert5-0.0.1/src/heads/encoder_heads.py
--rw-r--r--   0        0        0    34038 2020-02-02 00:00:00.000000 supert5-0.0.1/src/heads/t5_heads.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 supert5-0.0.1/src/model/__init__.py
--rw-r--r--   0        0        0    49182 2020-02-02 00:00:00.000000 supert5-0.0.1/src/model/attentions.py
--rw-r--r--   0        0        0     8159 2020-02-02 00:00:00.000000 supert5-0.0.1/src/model/config.py
--rw-r--r--   0        0        0    40800 2020-02-02 00:00:00.000000 supert5-0.0.1/src/model/modeling.py
--rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 supert5-0.0.1/src/model/modules.py
--rw-r--r--   0        0        0    13016 2020-02-02 00:00:00.000000 supert5-0.0.1/src/model/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 supert5-0.0.1/src/ops/__init__.py
--rw-r--r--   0        0        0     7893 2020-02-02 00:00:00.000000 supert5-0.0.1/src/ops/attention_bias.py
--rw-r--r--   0        0        0    32478 2020-02-02 00:00:00.000000 supert5-0.0.1/src/ops/flash_attention.py
--rw-r--r--   0        0        0    33884 2020-02-02 00:00:00.000000 supert5-0.0.1/src/ops/fused_bias_attention.py
--rw-r--r--   0        0        0    21361 2020-02-02 00:00:00.000000 supert5-0.0.1/src/ops/gated_mlp.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 supert5-0.0.1/src/ops/naive_attention.py
--rw-r--r--   0        0        0     6487 2020-02-02 00:00:00.000000 supert5-0.0.1/src/ops/rms_norm.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 supert5-0.0.1/tests/test_attentions.py
--rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 supert5-0.0.1/tests/test_generation.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 supert5-0.0.1/tests/test_rms_norm.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 supert5-0.0.1/.gitignore
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 supert5-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 supert5-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 supert5-0.0.2/README.md
+-rw-r--r--   0        0        0    66416 2020-02-02 00:00:00.000000 supert5-0.0.2/images/forwardpass_benchmarking.png
+-rw-r--r--   0        0        0    66248 2020-02-02 00:00:00.000000 supert5-0.0.2/images/memory_benchmarking.png
+-rw-r--r--   0        0        0    52665 2020-02-02 00:00:00.000000 supert5-0.0.2/images/speedup_benchmarking.png
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 supert5-0.0.2/src/superT5/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 supert5-0.0.2/src/superT5/heads/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 supert5-0.0.2/src/superT5/heads/decoder_heds.py
+-rw-r--r--   0        0        0    10997 2020-02-02 00:00:00.000000 supert5-0.0.2/src/superT5/heads/encoder_heads.py
+-rw-r--r--   0        0        0    34038 2020-02-02 00:00:00.000000 supert5-0.0.2/src/superT5/heads/t5_heads.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 supert5-0.0.2/src/superT5/model/__init__.py
+-rw-r--r--   0        0        0    49182 2020-02-02 00:00:00.000000 supert5-0.0.2/src/superT5/model/attentions.py
+-rw-r--r--   0        0        0     8159 2020-02-02 00:00:00.000000 supert5-0.0.2/src/superT5/model/config.py
+-rw-r--r--   0        0        0    40800 2020-02-02 00:00:00.000000 supert5-0.0.2/src/superT5/model/modeling.py
+-rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 supert5-0.0.2/src/superT5/model/modules.py
+-rw-r--r--   0        0        0    13016 2020-02-02 00:00:00.000000 supert5-0.0.2/src/superT5/model/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 supert5-0.0.2/src/superT5/ops/__init__.py
+-rw-r--r--   0        0        0     7893 2020-02-02 00:00:00.000000 supert5-0.0.2/src/superT5/ops/attention_bias.py
+-rw-r--r--   0        0        0    32478 2020-02-02 00:00:00.000000 supert5-0.0.2/src/superT5/ops/flash_attention.py
+-rw-r--r--   0        0        0    33884 2020-02-02 00:00:00.000000 supert5-0.0.2/src/superT5/ops/fused_bias_attention.py
+-rw-r--r--   0        0        0    21361 2020-02-02 00:00:00.000000 supert5-0.0.2/src/superT5/ops/gated_mlp.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 supert5-0.0.2/src/superT5/ops/naive_attention.py
+-rw-r--r--   0        0        0     6487 2020-02-02 00:00:00.000000 supert5-0.0.2/src/superT5/ops/rms_norm.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 supert5-0.0.2/tests/test_attentions.py
+-rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 supert5-0.0.2/tests/test_generation.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 supert5-0.0.2/tests/test_rms_norm.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 supert5-0.0.2/.gitignore
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 supert5-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 supert5-0.0.2/PKG-INFO
```

### Comparing `supert5-0.0.1/README.md` & `supert5-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `supert5-0.0.1/images/forwardpass_benchmarking.png` & `supert5-0.0.2/images/forwardpass_benchmarking.png`

 * *Files identical despite different names*

### Comparing `supert5-0.0.1/images/memory_benchmarking.png` & `supert5-0.0.2/images/memory_benchmarking.png`

 * *Files identical despite different names*

### Comparing `supert5-0.0.1/images/speedup_benchmarking.png` & `supert5-0.0.2/images/speedup_benchmarking.png`

 * *Files identical despite different names*

### Comparing `supert5-0.0.1/src/heads/encoder_heads.py` & `supert5-0.0.2/src/superT5/heads/encoder_heads.py`

 * *Files identical despite different names*

### Comparing `supert5-0.0.1/src/heads/t5_heads.py` & `supert5-0.0.2/src/superT5/heads/t5_heads.py`

 * *Files identical despite different names*

### Comparing `supert5-0.0.1/src/model/attentions.py` & `supert5-0.0.2/src/superT5/model/attentions.py`

 * *Files identical despite different names*

### Comparing `supert5-0.0.1/src/model/config.py` & `supert5-0.0.2/src/superT5/model/config.py`

 * *Files identical despite different names*

### Comparing `supert5-0.0.1/src/model/modeling.py` & `supert5-0.0.2/src/superT5/model/modeling.py`

 * *Files identical despite different names*

### Comparing `supert5-0.0.1/src/model/modules.py` & `supert5-0.0.2/src/superT5/model/modules.py`

 * *Files identical despite different names*

### Comparing `supert5-0.0.1/src/model/utils.py` & `supert5-0.0.2/src/superT5/model/utils.py`

 * *Files identical despite different names*

### Comparing `supert5-0.0.1/src/ops/attention_bias.py` & `supert5-0.0.2/src/superT5/ops/attention_bias.py`

 * *Files identical despite different names*

### Comparing `supert5-0.0.1/src/ops/flash_attention.py` & `supert5-0.0.2/src/superT5/ops/flash_attention.py`

 * *Files identical despite different names*

### Comparing `supert5-0.0.1/src/ops/fused_bias_attention.py` & `supert5-0.0.2/src/superT5/ops/fused_bias_attention.py`

 * *Files identical despite different names*

### Comparing `supert5-0.0.1/src/ops/gated_mlp.py` & `supert5-0.0.2/src/superT5/ops/gated_mlp.py`

 * *Files identical despite different names*

### Comparing `supert5-0.0.1/src/ops/naive_attention.py` & `supert5-0.0.2/src/superT5/ops/naive_attention.py`

 * *Files identical despite different names*

### Comparing `supert5-0.0.1/src/ops/rms_norm.py` & `supert5-0.0.2/src/superT5/ops/rms_norm.py`

 * *Files identical despite different names*

### Comparing `supert5-0.0.1/tests/test_attentions.py` & `supert5-0.0.2/tests/test_attentions.py`

 * *Files identical despite different names*

### Comparing `supert5-0.0.1/tests/test_generation.py` & `supert5-0.0.2/tests/test_generation.py`

 * *Files identical despite different names*

### Comparing `supert5-0.0.1/tests/test_rms_norm.py` & `supert5-0.0.2/tests/test_rms_norm.py`

 * *Files identical despite different names*

### Comparing `supert5-0.0.1/.gitignore` & `supert5-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `supert5-0.0.1/pyproject.toml` & `supert5-0.0.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["hatchling<=1.18.0"]
 build-backend = "hatchling.build"
 
 [project]
 name = "superT5"
-version = "0.0.1"
+version = "0.0.2"
 
 requires-python = ">=3.7"
 
-description = "Efficient T5 models."
+description = "Memory and compute efficient T5 models."
 license = "MIT"
 long_description = "file: README.md"
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
@@ -22,14 +22,14 @@
     "triton>=2.2.0",
     "transformers",
     "torch>=2.3.0"
 ]
 
 
 [options]
-packages = "./src"
+packages = "./src/superT5"
 zip_safe = "True"
 
 
 [tool.black]
 line-length = 80
 target-version = ['py37']
```

