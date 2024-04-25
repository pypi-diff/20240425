# Comparing `tmp/gbx-lm-0.2.0.tar.gz` & `tmp/gbx-lm-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gbx-lm-0.2.0.tar", last modified: Mon Apr 22 20:10:12 2024, max compression
+gzip compressed data, was "gbx-lm-0.2.1.tar", last modified: Thu Apr 25 15:29:26 2024, max compression
```

## Comparing `gbx-lm-0.2.0.tar` & `gbx-lm-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-04-22 20:10:12.280233 gbx-lm-0.2.0/
--rw-r--r--   0 haojin     (501) staff       (20)    11357 2024-03-18 14:26:20.000000 gbx-lm-0.2.0/LICENSE
--rw-r--r--   0 haojin     (501) staff       (20)     4613 2024-04-22 20:10:12.280020 gbx-lm-0.2.0/PKG-INFO
--rw-r--r--   0 haojin     (501) staff       (20)     4110 2024-04-22 19:59:47.000000 gbx-lm-0.2.0/README.md
-drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-04-22 20:10:12.277203 gbx-lm-0.2.0/gbx_lm/
--rw-r--r--   0 haojin     (501) staff       (20)       81 2024-04-10 08:41:13.000000 gbx-lm-0.2.0/gbx_lm/__init__.py
--rw-r--r--   0 haojin     (501) staff       (20)    12369 2024-04-08 20:13:35.000000 gbx-lm-0.2.0/gbx_lm/gba2mlx.py
--rw-r--r--   0 haojin     (501) staff       (20)     4158 2024-04-09 06:52:36.000000 gbx-lm-0.2.0/gbx_lm/generate.py
-drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-04-22 20:10:12.279228 gbx-lm-0.2.0/gbx_lm/models/
--rw-r--r--   0 haojin     (501) staff       (20)        0 2024-03-05 09:34:30.000000 gbx-lm-0.2.0/gbx_lm/models/__init__.py
--rw-r--r--   0 haojin     (501) staff       (20)      314 2024-01-13 21:15:10.000000 gbx-lm-0.2.0/gbx_lm/models/base.py
--rw-r--r--   0 haojin     (501) staff       (20)     5639 2024-04-08 11:50:53.000000 gbx-lm-0.2.0/gbx_lm/models/qgemma.py
--rw-r--r--   0 haojin     (501) staff       (20)     7114 2024-04-08 15:08:09.000000 gbx-lm-0.2.0/gbx_lm/models/qllama.py
--rw-r--r--   0 haojin     (501) staff       (20)     8289 2024-04-08 12:11:47.000000 gbx-lm-0.2.0/gbx_lm/models/qmixtral.py
--rw-r--r--   0 haojin     (501) staff       (20)     6614 2024-04-08 15:40:16.000000 gbx-lm-0.2.0/gbx_lm/models/qqwen2.py
--rw-r--r--   0 haojin     (501) staff       (20)    10690 2024-04-02 17:49:04.000000 gbx-lm-0.2.0/gbx_lm/models/quantized_linear_gba.py
-drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-04-22 20:10:12.279565 gbx-lm-0.2.0/gbx_lm/serve/
--rw-r--r--   0 haojin     (501) staff       (20)        0 2024-04-11 18:36:08.000000 gbx-lm-0.2.0/gbx_lm/serve/__init__.py
--rw-r--r--   0 haojin     (501) staff       (20)     9383 2024-04-11 14:56:32.000000 gbx-lm-0.2.0/gbx_lm/serve/mlx_fastchat_worker.py
--rw-r--r--   0 haojin     (501) staff       (20)    17365 2024-04-09 06:50:01.000000 gbx-lm-0.2.0/gbx_lm/utils.py
--rw-r--r--   0 haojin     (501) staff       (20)       21 2024-04-22 19:59:47.000000 gbx-lm-0.2.0/gbx_lm/version.py
-drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-04-22 20:10:12.277819 gbx-lm-0.2.0/gbx_lm.egg-info/
--rw-r--r--   0 haojin     (501) staff       (20)     4613 2024-04-22 20:10:12.000000 gbx-lm-0.2.0/gbx_lm.egg-info/PKG-INFO
--rw-r--r--   0 haojin     (501) staff       (20)      510 2024-04-22 20:10:12.000000 gbx-lm-0.2.0/gbx_lm.egg-info/SOURCES.txt
--rw-r--r--   0 haojin     (501) staff       (20)        1 2024-04-22 20:10:12.000000 gbx-lm-0.2.0/gbx_lm.egg-info/dependency_links.txt
--rw-r--r--   0 haojin     (501) staff       (20)       88 2024-04-22 20:10:12.000000 gbx-lm-0.2.0/gbx_lm.egg-info/requires.txt
--rw-r--r--   0 haojin     (501) staff       (20)        7 2024-04-22 20:10:12.000000 gbx-lm-0.2.0/gbx_lm.egg-info/top_level.txt
--rw-r--r--   0 haojin     (501) staff       (20)       38 2024-04-22 20:10:12.280288 gbx-lm-0.2.0/setup.cfg
--rw-r--r--   0 haojin     (501) staff       (20)      816 2024-04-11 19:04:43.000000 gbx-lm-0.2.0/setup.py
+drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-04-25 15:29:26.012401 gbx-lm-0.2.1/
+-rw-r--r--   0 haojin     (501) staff       (20)    11357 2024-03-18 14:26:20.000000 gbx-lm-0.2.1/LICENSE
+-rw-r--r--   0 haojin     (501) staff       (20)     4613 2024-04-25 15:29:26.012185 gbx-lm-0.2.1/PKG-INFO
+-rw-r--r--   0 haojin     (501) staff       (20)     4110 2024-04-22 19:59:47.000000 gbx-lm-0.2.1/README.md
+drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-04-25 15:29:26.009390 gbx-lm-0.2.1/gbx_lm/
+-rw-r--r--   0 haojin     (501) staff       (20)       81 2024-04-10 08:41:13.000000 gbx-lm-0.2.1/gbx_lm/__init__.py
+-rw-r--r--   0 haojin     (501) staff       (20)    12501 2024-04-25 15:28:27.000000 gbx-lm-0.2.1/gbx_lm/gba2mlx.py
+-rw-r--r--   0 haojin     (501) staff       (20)     4158 2024-04-09 06:52:36.000000 gbx-lm-0.2.1/gbx_lm/generate.py
+drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-04-25 15:29:26.011514 gbx-lm-0.2.1/gbx_lm/models/
+-rw-r--r--   0 haojin     (501) staff       (20)        0 2024-03-05 09:34:30.000000 gbx-lm-0.2.1/gbx_lm/models/__init__.py
+-rw-r--r--   0 haojin     (501) staff       (20)      314 2024-01-13 21:15:10.000000 gbx-lm-0.2.1/gbx_lm/models/base.py
+-rw-r--r--   0 haojin     (501) staff       (20)     5639 2024-04-08 11:50:53.000000 gbx-lm-0.2.1/gbx_lm/models/qgemma.py
+-rw-r--r--   0 haojin     (501) staff       (20)     6744 2024-04-25 15:28:27.000000 gbx-lm-0.2.1/gbx_lm/models/qllama.py
+-rw-r--r--   0 haojin     (501) staff       (20)     7897 2024-04-25 15:28:27.000000 gbx-lm-0.2.1/gbx_lm/models/qmixtral.py
+-rw-r--r--   0 haojin     (501) staff       (20)     6211 2024-04-25 15:28:27.000000 gbx-lm-0.2.1/gbx_lm/models/qphi3.py
+-rw-r--r--   0 haojin     (501) staff       (20)     6614 2024-04-08 15:40:16.000000 gbx-lm-0.2.1/gbx_lm/models/qqwen2.py
+-rw-r--r--   0 haojin     (501) staff       (20)    10841 2024-04-25 15:28:27.000000 gbx-lm-0.2.1/gbx_lm/models/quantized_linear_gba.py
+drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-04-25 15:29:26.011749 gbx-lm-0.2.1/gbx_lm/serve/
+-rw-r--r--   0 haojin     (501) staff       (20)        0 2024-04-11 18:36:08.000000 gbx-lm-0.2.1/gbx_lm/serve/__init__.py
+-rw-r--r--   0 haojin     (501) staff       (20)     9383 2024-04-11 14:56:32.000000 gbx-lm-0.2.1/gbx_lm/serve/mlx_fastchat_worker.py
+-rw-r--r--   0 haojin     (501) staff       (20)    17391 2024-04-25 15:28:27.000000 gbx-lm-0.2.1/gbx_lm/utils.py
+-rw-r--r--   0 haojin     (501) staff       (20)       21 2024-04-25 15:28:27.000000 gbx-lm-0.2.1/gbx_lm/version.py
+drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-04-25 15:29:26.009982 gbx-lm-0.2.1/gbx_lm.egg-info/
+-rw-r--r--   0 haojin     (501) staff       (20)     4613 2024-04-25 15:29:25.000000 gbx-lm-0.2.1/gbx_lm.egg-info/PKG-INFO
+-rw-r--r--   0 haojin     (501) staff       (20)      533 2024-04-25 15:29:25.000000 gbx-lm-0.2.1/gbx_lm.egg-info/SOURCES.txt
+-rw-r--r--   0 haojin     (501) staff       (20)        1 2024-04-25 15:29:25.000000 gbx-lm-0.2.1/gbx_lm.egg-info/dependency_links.txt
+-rw-r--r--   0 haojin     (501) staff       (20)       88 2024-04-25 15:29:25.000000 gbx-lm-0.2.1/gbx_lm.egg-info/requires.txt
+-rw-r--r--   0 haojin     (501) staff       (20)        7 2024-04-25 15:29:25.000000 gbx-lm-0.2.1/gbx_lm.egg-info/top_level.txt
+-rw-r--r--   0 haojin     (501) staff       (20)       38 2024-04-25 15:29:26.012457 gbx-lm-0.2.1/setup.cfg
+-rw-r--r--   0 haojin     (501) staff       (20)      816 2024-04-11 19:04:43.000000 gbx-lm-0.2.1/setup.py
```

### Comparing `gbx-lm-0.2.0/LICENSE` & `gbx-lm-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gbx-lm-0.2.0/PKG-INFO` & `gbx-lm-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbx-lm
-Version: 0.2.0
+Version: 0.2.1
 Summary: GBA Model Toolkit for MLX
 Home-page: https://github.com/GreenBitAI/gbx-lm
 Author: GreenBitAI and MLX Contributors
 Author-email: team@greenbit.ai
 License: Apache-2.0
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `gbx-lm-0.2.0/README.md` & `gbx-lm-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `gbx-lm-0.2.0/gbx_lm/gba2mlx.py` & `gbx-lm-0.2.1/gbx_lm/gba2mlx.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,16 +76,20 @@
       - The PreTrainedTokenizer associated with the model.
 
     The function leverages the Transformers library to obtain the configuration and tokenizer, and assumes the
     existence of a `load_model` function tailored for loading and possibly quantizing the model based on the given
     parameters.
     """
     model_path = get_model_path(model_path, token=token)
-    config = transformers.AutoConfig.from_pretrained(model_path, token=token)
-    tokenizer = transformers.AutoTokenizer.from_pretrained(model_path, token=token)
+    config = transformers.AutoConfig.from_pretrained(model_path, token=token, trust_remote_code=True)
+
+    # Building tokenizer_config
+    tokenizer_config = {"token": token, "trust_remote_code": True}
+    tokenizer = transformers.AutoTokenizer.from_pretrained(model_path, **tokenizer_config)
+
     model = load_model(model_path, bits, group_size, is_conversion)
     return model, config.to_dict(), tokenizer, model_path
 
 
 def get_quantized_parameters(
     model: nn.Module, config: dict, q_group_size: int, q_bits: int
 ) -> tuple:
```

### Comparing `gbx-lm-0.2.0/gbx_lm/generate.py` & `gbx-lm-0.2.1/gbx_lm/generate.py`

 * *Files identical despite different names*

### Comparing `gbx-lm-0.2.0/gbx_lm/models/qgemma.py` & `gbx-lm-0.2.1/gbx_lm/models/qgemma.py`

 * *Files identical despite different names*

### Comparing `gbx-lm-0.2.0/gbx_lm/models/qllama.py` & `gbx-lm-0.2.1/gbx_lm/models/qllama.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,28 +30,14 @@
             if not all(key in self.rope_scaling for key in required_keys):
                 raise ValueError(f"rope_scaling must contain keys {required_keys}")
 
             if self.rope_scaling["type"] != "linear":
                 raise ValueError("rope_scaling 'type' currently only supports 'linear'")
 
 
-class RMSNorm(nn.Module):
-    def __init__(self, dims: int, eps: float = 1e-5):
-        super().__init__()
-        self.weight = mx.ones((dims,))
-        self.eps = eps
-
-    def _norm(self, x):
-        return x * mx.rsqrt(x.square().mean(-1, keepdims=True) + self.eps)
-
-    def __call__(self, x):
-        output = self._norm(x.astype(mx.float32)).astype(x.dtype)
-        return self.weight * output
-
-
 class Attention(nn.Module):
     def __init__(self, args: ModelArgs):
         super().__init__()
 
         dim = args.hidden_size
         self.n_heads = n_heads = args.num_attention_heads
         self.n_kv_heads = n_kv_heads = args.num_key_value_heads
@@ -132,16 +118,18 @@
 class TransformerBlock(nn.Module):
     def __init__(self, args: ModelArgs):
         super().__init__()
         self.num_attention_heads = args.num_attention_heads
         self.hidden_size = args.hidden_size
         self.self_attn = Attention(args)
         self.mlp = MLP(args.hidden_size, args.intermediate_size)
-        self.input_layernorm = RMSNorm(args.hidden_size, eps=args.rms_norm_eps)
-        self.post_attention_layernorm = RMSNorm(args.hidden_size, eps=args.rms_norm_eps)
+        self.input_layernorm = nn.RMSNorm(args.hidden_size, eps=args.rms_norm_eps)
+        self.post_attention_layernorm = nn.RMSNorm(
+            args.hidden_size, eps=args.rms_norm_eps
+        )
         self.args = args
 
     def __call__(
         self,
         x: mx.array,
         mask: Optional[mx.array] = None,
         cache: Optional[Tuple[mx.array, mx.array]] = None,
@@ -160,15 +148,15 @@
         self.vocab_size = args.vocab_size
         self.num_hidden_layers = args.num_hidden_layers
         assert self.vocab_size > 0
         self.embed_tokens = nn.Embedding(args.vocab_size, args.hidden_size)
         self.layers = [
             TransformerBlock(args=args) for _ in range(args.num_hidden_layers)
         ]
-        self.norm = RMSNorm(args.hidden_size, eps=args.rms_norm_eps)
+        self.norm = nn.RMSNorm(args.hidden_size, eps=args.rms_norm_eps)
 
     def __call__(
         self,
         inputs: mx.array,
         cache=None,
     ):
         h = self.embed_tokens(inputs)
```

### Comparing `gbx-lm-0.2.0/gbx_lm/models/qmixtral.py` & `gbx-lm-0.2.1/gbx_lm/models/qmixtral.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,28 +26,14 @@
     rope_scaling: Optional[Dict[str, Union[float, str]]] = None
 
     def __post_init__(self):
         if self.num_key_value_heads is None:
             self.num_key_value_heads = self.num_attention_heads
 
 
-class RMSNorm(nn.Module):
-    def __init__(self, dims: int, eps: float = 1e-5):
-        super().__init__()
-        self.weight = mx.ones((dims,))
-        self.eps = eps
-
-    def _norm(self, x):
-        return x * mx.rsqrt(x.square().mean(-1, keepdims=True) + self.eps)
-
-    def __call__(self, x):
-        output = self._norm(x.astype(mx.float32)).astype(x.dtype)
-        return self.weight * output
-
-
 class MixtralAttention(nn.Module):
     def __init__(self, args: ModelArgs):
         super().__init__()
         self.hidden_size = args.hidden_size
         self.num_heads = args.num_attention_heads
         self.head_dim = self.hidden_size // self.num_heads
         self.num_key_value_heads = args.num_key_value_heads
@@ -178,16 +164,16 @@
     def __init__(self, args: ModelArgs):
         super().__init__()
         self.hidden_size = args.hidden_size
 
         self.self_attn = MixtralAttention(args)
 
         self.block_sparse_moe = MixtralSparseMoeBlock(args)
-        self.input_layernorm = RMSNorm(args.hidden_size, eps=args.rms_norm_eps)
-        self.post_attention_layernorm = RMSNorm(args.hidden_size, eps=args.rms_norm_eps)
+        self.input_layernorm = nn.RMSNorm(args.hidden_size, eps=args.rms_norm_eps)
+        self.post_attention_layernorm = nn.RMSNorm(args.hidden_size, eps=args.rms_norm_eps)
 
     def __call__(
         self,
         x: mx.array,
         mask: Optional[mx.array] = None,
         cache: Optional[Tuple[mx.array, mx.array]] = None,
     ) -> mx.array:
@@ -204,15 +190,15 @@
         self.vocab_size = args.vocab_size
         self.num_hidden_layers = args.num_hidden_layers
 
         self.embed_tokens = nn.Embedding(args.vocab_size, args.hidden_size)
         self.layers = [
             MixtralDecoderLayer(args=args) for _ in range(args.num_hidden_layers)
         ]
-        self.norm = RMSNorm(args.hidden_size, eps=args.rms_norm_eps)
+        self.norm = nn.RMSNorm(args.hidden_size, eps=args.rms_norm_eps)
 
     def __call__(
         self,
         inputs: mx.array,
         cache=None,
     ):
         h = self.embed_tokens(inputs)
```

### Comparing `gbx-lm-0.2.0/gbx_lm/models/qqwen2.py` & `gbx-lm-0.2.1/gbx_lm/models/qqwen2.py`

 * *Files identical despite different names*

### Comparing `gbx-lm-0.2.0/gbx_lm/models/quantized_linear_gba.py` & `gbx-lm-0.2.1/gbx_lm/models/quantized_linear_gba.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,18 +224,21 @@
             """
             for name, child in model.named_modules():
                 if isinstance(child, QuantizedLinear):
                     # read bits and group size from strategy
                     layer_number = name.split('.')[2]
                     strategy_per_block = strategy["model.layers.{}".format(layer_number)]
 
-                    for key in ['q_proj', 'k_proj', 'v_proj', 'o_proj', 'gate_proj', 'up_proj', 'down_proj']:
+                    for key in ['q_proj', 'k_proj', 'v_proj', 'o_proj', 'gate_proj', 'up_proj', 'down_proj', 'qkv_proj', 'gate_up_proj']:
                         if key in name:
-                            strg = strategy_per_block[key]
-                            break
+                            try:
+                                strg = strategy_per_block[key]
+                                break
+                            except KeyError:
+                                pass
                     child.bits = strg["bits"][0]
                     child.group_size = strg["group_size"][str(child.bits)]
                     assert child.group_size in [32, 64, 128], f"The group size value ({child.group_size}) must be 32, 64 or 128."
                     # print(f'[DEBUG]: {name}: Updated QuantizedLinear bits to {child.bits}, group_size to {child.group_size}')
 
                     # re-init params
                     child.init_params(use_double_quantization, use_q_perm)
```

### Comparing `gbx-lm-0.2.0/gbx_lm/serve/mlx_fastchat_worker.py` & `gbx-lm-0.2.1/gbx_lm/serve/mlx_fastchat_worker.py`

 * *Files identical despite different names*

### Comparing `gbx-lm-0.2.0/gbx_lm/utils.py` & `gbx-lm-0.2.1/gbx_lm/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,25 +7,26 @@
 
 import mlx.core as mx
 import mlx.nn as nn
 from huggingface_hub import snapshot_download
 from transformers import AutoTokenizer, PreTrainedTokenizer, AutoConfig
 
 # Local imports
-from .models import qllama, qmixtral, qgemma, qqwen2
+from .models import qllama, qmixtral, qgemma, qqwen2, qphi3
 from .models.quantized_linear_gba import QuantizedLinear
 import re
 
 # Constants
 MODEL_MAPPING = {
     "llama": qllama,
     "mistral": qllama,  # mistral is compatible with llama
     "mixtral": qmixtral,
     "gemma": qgemma,
-    "qwen2": qqwen2
+    "qwen2": qqwen2,
+    "phi3": qphi3
 }
 
 linear_class_predicate = (
     lambda m: isinstance(m, nn.Linear)
     and m.weight.shape[0]
     != 8  # avoid quantizing gate layers, otherwise we have to re-quant and upload all the mixtral models
 )
```

### Comparing `gbx-lm-0.2.0/gbx_lm.egg-info/PKG-INFO` & `gbx-lm-0.2.1/gbx_lm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbx-lm
-Version: 0.2.0
+Version: 0.2.1
 Summary: GBA Model Toolkit for MLX
 Home-page: https://github.com/GreenBitAI/gbx-lm
 Author: GreenBitAI and MLX Contributors
 Author-email: team@greenbit.ai
 License: Apache-2.0
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `gbx-lm-0.2.0/setup.py` & `gbx-lm-0.2.1/setup.py`

 * *Files identical despite different names*

