# Comparing `tmp/hnn_utils-0.2.4.tar.gz` & `tmp/hnn_utils-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnn_utils-0.2.4.tar", max compression
+gzip compressed data, was "hnn_utils-0.3.0.tar", max compression
```

## Comparing `hnn_utils-0.2.4.tar` & `hnn_utils-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0     1068 2024-03-04 17:55:27.897529 hnn_utils-0.2.4/LICENSE
--rw-r--r--   0        0        0      137 2024-03-04 17:55:27.897529 hnn_utils-0.2.4/README.md
--rw-r--r--   0        0        0        0 2024-03-04 17:55:27.897529 hnn_utils-0.2.4/hnn_utils/__init__.py
--rw-r--r--   0        0        0       48 2024-03-04 17:55:27.901528 hnn_utils-0.2.4/hnn_utils/callbacks/__init__.py
--rw-r--r--   0        0        0     6438 2024-03-04 17:55:27.901528 hnn_utils-0.2.4/hnn_utils/callbacks/ema.py
--rw-r--r--   0        0        0     1370 2024-03-04 17:55:27.901528 hnn_utils-0.2.4/hnn_utils/nn/ALiBi.py
--rw-r--r--   0        0        0     1655 2024-03-04 17:55:27.901528 hnn_utils-0.2.4/hnn_utils/nn/RotaryEmbedding.py
--rw-r--r--   0        0        0    13256 2024-03-04 17:55:27.901528 hnn_utils-0.2.4/hnn_utils/nn/Transformer.py
--rw-r--r--   0        0        0      122 2024-03-04 17:55:27.901528 hnn_utils-0.2.4/hnn_utils/nn/__init__.py
--rw-r--r--   0        0        0     1961 2024-03-04 17:55:27.901528 hnn_utils-0.2.4/hnn_utils/nn/functional.py
--rw-r--r--   0        0        0      448 2024-03-04 17:55:27.901528 hnn_utils-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      761 1970-01-01 00:00:00.000000 hnn_utils-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-25 03:42:44.890258 hnn_utils-0.3.0/LICENSE
+-rw-r--r--   0        0        0      137 2024-04-25 03:42:44.890258 hnn_utils-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-25 03:42:44.890258 hnn_utils-0.3.0/hnn_utils/__init__.py
+-rw-r--r--   0        0        0       48 2024-04-25 03:42:44.890258 hnn_utils-0.3.0/hnn_utils/callbacks/__init__.py
+-rw-r--r--   0        0        0     6438 2024-04-25 03:42:44.890258 hnn_utils-0.3.0/hnn_utils/callbacks/ema.py
+-rw-r--r--   0        0        0     1370 2024-04-25 03:42:44.890258 hnn_utils-0.3.0/hnn_utils/nn/ALiBi.py
+-rw-r--r--   0        0        0     1655 2024-04-25 03:42:44.890258 hnn_utils-0.3.0/hnn_utils/nn/RotaryEmbedding.py
+-rw-r--r--   0        0        0    14366 2024-04-25 03:42:44.890258 hnn_utils-0.3.0/hnn_utils/nn/Transformer.py
+-rw-r--r--   0        0        0      164 2024-04-25 03:42:44.890258 hnn_utils-0.3.0/hnn_utils/nn/__init__.py
+-rw-r--r--   0        0        0     1247 2024-04-25 03:42:44.890258 hnn_utils-0.3.0/hnn_utils/nn/ffn.py
+-rw-r--r--   0        0        0     1961 2024-04-25 03:42:44.890258 hnn_utils-0.3.0/hnn_utils/nn/functional.py
+-rw-r--r--   0        0        0      800 2024-04-25 03:42:44.890258 hnn_utils-0.3.0/hnn_utils/nn/normalization.py
+-rw-r--r--   0        0        0      448 2024-04-25 03:42:44.890258 hnn_utils-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      761 1970-01-01 00:00:00.000000 hnn_utils-0.3.0/PKG-INFO
```

### Comparing `hnn_utils-0.2.4/LICENSE` & `hnn_utils-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.2.4/hnn_utils/callbacks/ema.py` & `hnn_utils-0.3.0/hnn_utils/callbacks/ema.py`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.2.4/hnn_utils/nn/ALiBi.py` & `hnn_utils-0.3.0/hnn_utils/nn/ALiBi.py`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.2.4/hnn_utils/nn/RotaryEmbedding.py` & `hnn_utils-0.3.0/hnn_utils/nn/RotaryEmbedding.py`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.2.4/hnn_utils/nn/Transformer.py` & `hnn_utils-0.3.0/hnn_utils/nn/Transformer.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,123 +3,131 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from einops import rearrange
 from torch import Tensor
 
 from hnn_utils.nn.ALiBi import ALiBi
+from hnn_utils.nn.normalization import LayerNorm
+from hnn_utils.nn.ffn import FFNSwiGLU
+
+try:
+    from flash_attn import flash_attn_kvpacked_func, flash_attn_qkvpacked_func
+
+    FLASH_AVAILABLE = True
+except ImportError as e:
+    print("Flash not available, using PyTorch implementation: ", e)
+    FLASH_AVAILABLE = False
 
 
 class TransformerEncoder(nn.Module):
     """
-    PyTorch API compatible (more or less) encoder for Transformers, with support for ALiBi.
+    Initializes a TransformerEncoder instance.
 
     Args:
-        encoder_layers: encoder layers to use
+        *encoder_layers (nn.Module): Variable number of encoder layers.
+
     """
 
     def __init__(self, *encoder_layers: nn.Module) -> None:
         super().__init__()
 
         self.layers = nn.ModuleList(list(*encoder_layers))
 
     def forward(
         self,
         src: Tensor,
         mask: Optional[Tensor] = None,
-        src_padding_mask: Optional[Tensor] = None,
+        src_pad_mask: Optional[Tensor] = None,
         is_causal: bool = False,
     ) -> Tensor:
         output = src
 
         for layer in self.layers:
-            output = layer(output, mask, src_padding_mask, is_causal=is_causal)
+            output = layer(output, mask, src_pad_mask, is_causal=is_causal)
 
         return output
 
 
 class TransformerDecoder(nn.Module):
     """
-    PyTorch API compatible (more or less) decoder for Transformers, with support for ALiBi.
+    Transformer Decoder module.
 
     Args:
-        decoder_layers: decoder layers to use
+        *decoder_layers: Variable number of decoder layers.
+
     """
 
     def __init__(
         self,
         *decoder_layers: nn.Module,
     ) -> None:
         super().__init__()
 
         self.layers = nn.ModuleList(list(*decoder_layers))
 
     def forward(
         self,
         tgt: Tensor,
-        memory: Tensor,
+        mem: Tensor,
         tgt_mask: Optional[Tensor] = None,
-        memory_mask: Optional[Tensor] = None,
-        tgt_padding_mask: Optional[Tensor] = None,
-        memory_padding_mask: Optional[Tensor] = None,
+        mem_mask: Optional[Tensor] = None,
+        tgt_pad_mask: Optional[Tensor] = None,
+        mem_pad_mask: Optional[Tensor] = None,
         tgt_is_causal: bool = False,
-        memory_is_causal: bool = False,
+        mem_is_causal: bool = False,
     ) -> Tensor:
         output = tgt
 
         for layer in self.layers:
             output = layer(
                 output,
-                memory,
+                mem,
                 tgt_mask,
-                memory_mask,
-                tgt_padding_mask,
-                memory_padding_mask,
+                mem_mask,
+                tgt_pad_mask,
+                mem_pad_mask,
                 tgt_is_causal,
-                memory_is_causal,
+                mem_is_causal,
             )
 
         return output
 
 
 class TransformerEncoderLayer(nn.Module):
     """
-    PyTorch API compatible (more or less) encoder layer for Transformers, with support for ALiBi.
-
-    Note: Some of the defaults do not match the PyTorch implementation as they are used in my own experiments.
-    Note: RMSNorm is supposed to increase throughput, but it doesn't seem to be the case for small models?
+    Transformer Encoder Layer.
 
     Args:
-        d_model: dimension of the embeddings
-        nhead: number of attention heads
-        dim_feedforward: dimension of the feedforward network
-        dropout: dropout value
-        activation: activation function in feedforward (nn.Module)
-        norm_first: whether to apply layer norm before or after blocks
-        self_alibi: use ALiBi in self-attention
-        norm_first: whether to apply layer norm before or after blocks
+        d_model (int): The number of expected features in the input.
+        nhead (int): The number of heads in the multiheadattention models.
+        dim_feedforward (int, optional): The dimension of the feedforward network model. Default is 2048.
+        dropout (float, optional): The dropout value. Default is 0.1.
+        self_alibi (bool, optional): Whether to use self-alibi attention. Default is True.
+        norm_cls (nn.Module, optional): The normalization layer class. Default is LayerNorm.
+        ffn_cls (nn.Module, optional): The feedforward network class. Default is FFNSwiGLU.
+        norm_first (bool, optional): Whether to apply normalization before the self-attention block. Default is True.
     """
 
     def __init__(
         self,
         d_model: int,
         nhead: int,
         dim_feedforward: int = 2048,
         dropout: float = 0.1,
         self_alibi: bool = True,
-        use_rms_norm: bool = True,
-        use_swiglu: bool = True,
+        norm_cls: nn.Module = LayerNorm,
+        ffn_cls: nn.Module = FFNSwiGLU,
         norm_first: bool = True,
     ) -> None:
         super().__init__()
 
-        norm_cls = {True: RMSNorm, False: LayerNormWrapper}[use_rms_norm]
-        ffn_cls = {True: FFNSwiGLU, False: FFNN}[use_swiglu]
-
-        self.self_attn = MultiheadAttention(d_model, nhead, dropout=dropout, use_alibi=self_alibi)  # fmt: skip
+        self.self_attn = SelfAttention(
+            d_model, nhead, dropout=dropout, use_alibi=self_alibi
+        )
 
         self.ff_block = ffn_cls(d_model, dim_feedforward)
 
         self.norm1 = norm_cls(d_model)
         self.norm2 = norm_cls(d_model)
 
         self.dropout = nn.Dropout(dropout)
@@ -128,76 +136,76 @@
 
         self.apply(_reset_parameters)
 
     def forward(
         self,
         src: Tensor,
         src_mask: Optional[Tensor] = None,
-        src_padding_mask: Optional[Tensor] = None,
+        src_pad_mask: Optional[Tensor] = None,
         is_causal: bool = False,
     ) -> Tensor:
         x = src
         if self.norm_first:
-            x = x + self._sa_block(self.norm1(x), src_mask, src_padding_mask, is_causal=is_causal)  # fmt: skip
+            x = x + self._sa_block(self.norm1(x), src_mask, src_pad_mask, is_causal=is_causal)  # fmt: skip
             x = x + self.ff_block(self.norm2(x))
         else:
-            x = self.norm1(x + self._sa_block(x, src_mask, src_padding_mask, is_causal=is_causal))  # fmt: skip
+            x = self.norm1(x + self._sa_block(x, src_mask, src_pad_mask, is_causal=is_causal))  # fmt: skip
             x = self.norm2(x + self.ff_block(x))
 
         return x
 
     def _sa_block(
         self,
         x: Tensor,
         attn_mask: Optional[Tensor],
-        padding_mask: Optional[Tensor],
+        pad_mask: Optional[Tensor],
         is_causal: bool = False,
     ) -> Tensor:
-        x = self.self_attn(x, x, x, attn_mask=attn_mask, padding_mask=padding_mask, is_causal=is_causal)  # fmt: skip
+        x = self.self_attn(
+            x, attn_mask=attn_mask, pad_mask=pad_mask, is_causal=is_causal
+        )
         return self.dropout(x)
 
 
 class TransformerDecoderLayer(nn.Module):
     """
-    PyTorch API compatible (more or less) decoder layer for Transformers, with support for ALiBi.
-
-    Note: Some of the defaults do not match the PyTorch implementation.
-    Note: RMSNorm is supposed to increase throughput, but it doesn't seem to be the case for small models?
+    Transformer Decoder Layer.
 
     Args:
-        d_model: dimension of the embeddings
-        nhead: number of attention heads
-        dim_feedforward: dimension of the feedforward network
-        dropout: dropout value
-        activation: activation function in feedforward (nn.Module)
-        norm_first: whether to apply layer norm before or after blocks
-        self_alibi: use ALiBi in self-attention
-        cross_alibi: use ALiBi in cross-attention
-        norm_first: whether to apply layer norm before or after blocks
+        d_model (int): The number of expected features in the input.
+        nhead (int): The number of heads in the multiheadattention models.
+        dim_feedforward (int, optional): The dimension of the feedforward network model. Default is 2048.
+        dropout (float, optional): The dropout value. Default is 0.1.
+        self_alibi (bool, optional): Whether to use self-alibi attention. Default is True.
+        cross_alibi (bool, optional): Whether to use cross-alibi attention. Default is False.
+        ffn_cls (nn.Module, optional): The feedforward network class. Default is FFNSwiGLU.
+        norm_cls (nn.Module, optional): The normalization class. Default is LayerNorm.
+        norm_first (bool, optional): Whether to apply normalization before each sub-layer. Default is False.
     """
 
     def __init__(
         self,
         d_model: int,
         nhead: int,
         dim_feedforward: int = 2048,
         dropout: float = 0.1,
-        self_alibi: bool = False,
+        self_alibi: bool = True,
         cross_alibi: bool = False,
-        use_rms_norm: bool = True,
-        use_swiglu: bool = True,
-        norm_first: bool = True,
+        ffn_cls: nn.Module = FFNSwiGLU,
+        norm_cls: nn.Module = LayerNorm,
+        norm_first: bool = False,
     ):
         super().__init__()
 
-        norm_cls = {True: RMSNorm, False: LayerNormWrapper}[use_rms_norm]
-        ffn_cls = {True: FFNSwiGLU, False: FFNN}[use_swiglu]
-
-        self.self_attn = MultiheadAttention(d_model, nhead, dropout=dropout, use_alibi=self_alibi)  # fmt: skip
-        self.cross_attn = MultiheadAttention(d_model, nhead, dropout=dropout, use_alibi=cross_alibi)  # fmt: skip
+        self.self_attn = SelfAttention(
+            d_model, nhead, dropout=dropout, use_alibi=self_alibi
+        )
+        self.cross_attn = CrossAttention(
+            d_model, nhead, dropout=dropout, use_alibi=cross_alibi
+        )
 
         self.ff_block = ffn_cls(d_model, dim_feedforward)
 
         self.norm1 = norm_cls(d_model)
         self.norm2 = norm_cls(d_model)
         self.norm3 = norm_cls(d_model)
 
@@ -207,193 +215,208 @@
         self.norm_first = norm_first
 
         self.apply(_reset_parameters)
 
     def forward(
         self,
         tgt: Tensor,
-        memory: Tensor,
+        mem: Tensor,
         tgt_mask: Optional[Tensor] = None,
-        memory_mask: Optional[Tensor] = None,
-        tgt_padding_mask: Optional[Tensor] = None,
-        memory_padding_mask: Optional[Tensor] = None,
+        mem_mask: Optional[Tensor] = None,
+        tgt_pad_mask: Optional[Tensor] = None,
+        mem_pad_mask: Optional[Tensor] = None,
         tgt_is_causal: bool = False,
-        memory_is_causal: bool = False,
+        mem_is_causal: bool = False,
     ) -> Tensor:
         x = tgt
         if self.norm_first:
-            x = x + self._sa_block(self.norm1(x), tgt_mask, tgt_padding_mask, is_causal=tgt_is_causal)  # fmt: skip
-            x = x + self._mha_block(self.norm2(x),memory,memory_mask,memory_padding_mask,memory_is_causal)  # fmt: skip
+            x = x + self._sa_block(self.norm1(x), tgt_mask, tgt_pad_mask, is_causal=tgt_is_causal)  # fmt: skip
+            x = x + self._mha_block(self.norm2(x), mem, mem_mask, mem_pad_mask, mem_is_causal)  # fmt: skip
             x = x + self.ff_block(self.norm3(x))
         else:
-            x = self.norm1(x + self._sa_block(x, tgt_mask, tgt_padding_mask, is_causal=tgt_is_causal))  # fmt: skip
-            x = self.norm2(x + self._mha_block(x, memory, memory_mask, memory_padding_mask, memory_is_causal))  # fmt: skip
+            x = self.norm1(x + self._sa_block(x, tgt_mask, tgt_pad_mask, is_causal=tgt_is_causal))  # fmt: skip
+            x = self.norm2(x + self._mha_block(x, mem, mem_mask, mem_pad_mask, mem_is_causal))  # fmt: skip
             x = self.norm3(x + self.ff_block(x))
         return x
 
     def _sa_block(
         self,
         x: Tensor,
         attn_mask: Optional[Tensor],
-        padding_mask: Optional[Tensor],
+        pad_mask: Optional[Tensor],
         is_causal: bool = False,
     ) -> Tensor:
-        x = self.self_attn(x, x, x, attn_mask=attn_mask, padding_mask=padding_mask, is_causal=is_causal)  # fmt: skip
+        x = self.self_attn(x, attn_mask=attn_mask, pad_mask=pad_mask, is_causal=is_causal)  # fmt: skip
         return self.dropout1(x)
 
-    # multihead attention block
     def _mha_block(
         self,
         x: Tensor,
         mem: Tensor,
         attn_mask: Optional[Tensor],
-        padding_mask: Optional[Tensor],
+        pad_mask: Optional[Tensor],
         is_causal: bool = False,
     ) -> Tensor:
-        x = self.cross_attn(x, mem, mem, attn_mask=attn_mask, padding_mask=padding_mask, is_causal=is_causal)  # fmt: skip
+        x = self.cross_attn(x, mem, attn_mask=attn_mask, pad_mask=pad_mask, is_causal=is_causal)  # fmt: skip
         return self.dropout2(x)
 
 
-class MultiheadAttention(nn.Module):
+class CrossAttention(nn.Module):
     def __init__(
         self,
         embed_dim: int,
         heads: int,
         dropout: float = 0.0,
-        use_alibi: bool = False,
+        use_alibi: bool = True,
     ):
         super().__init__()
 
         self.embed_size = embed_dim
         self.num_heads = heads
         self.head_dim = embed_dim // heads
         self.dropout = dropout
 
         assert (
             self.head_dim * heads == embed_dim
         ), "Embedding size needs to be divisible by heads"
 
         self.q_proj = nn.Linear(self.embed_size, self.embed_size)
-        self.k_proj = nn.Linear(self.embed_size, self.embed_size)
-        self.v_proj = nn.Linear(self.embed_size, self.embed_size)
+        self.kv_proj = nn.Linear(self.embed_size, self.embed_size * 2)
 
         self.out_proj = nn.Linear(heads * self.head_dim, embed_dim)
 
         if use_alibi:
             self.alibi = ALiBi(heads)
 
     def forward(
         self,
         query: Tensor,
-        key: Tensor,
-        value: Tensor,
-        padding_mask: Optional[Tensor] = None,
+        kv: Tensor,
+        pad_mask: Optional[Tensor] = None,
         attn_mask: Optional[Tensor] = None,
         is_causal: bool = False,
     ) -> Tensor:
+        if can_flash(query, pad_mask, attn_mask):
+            return self.flash_forward(query, kv, is_causal)
+
         q = self.q_proj(query)
-        k = self.k_proj(key)
-        v = self.v_proj(value)
+        k, v = self.kv_proj(kv).chunk(2, dim=-1)
 
         q = rearrange(q, "... n (h d) -> ... h n d", h=self.num_heads)
         k = rearrange(k, "... n (h d) -> ... h n d", h=self.num_heads)
         v = rearrange(v, "... n (h d) -> ... h n d", h=self.num_heads)
 
-        mask = combine_masks(attn_mask, padding_mask, self.num_heads, query.dtype)
+        mask = combine_masks(attn_mask, pad_mask, self.num_heads, query.dtype)
 
         if hasattr(self, "alibi"):
             bias = self.alibi(q, k)
             mask = mask + bias if mask is not None else bias
 
         dropout = self.dropout if self.training else 0.0
         attn = F.scaled_dot_product_attention(
             q, k, v, mask, is_causal=is_causal, dropout_p=dropout
         )
 
         attn = rearrange(attn, "... h n d -> ... n (h d)")
         return self.out_proj(attn)
 
+    def flash_forward(self, query: Tensor, kv: Tensor, is_causal: bool) -> Tensor:
+        q = self.q_proj(query)
+        kv = self.kv_proj(kv)
 
-class RMSNorm(nn.Module):
-    """
-    Root Mean Square Layer Normalization
-    https://arxiv.org/abs/1910.07467
-    """
+        q = rearrange(q, "... (h d) -> ... h d", h=self.num_heads)
+        kv = rearrange(kv, "... (n h d) -> ... n h d", h=self.num_heads, n=2)
 
-    def __init__(self, dim: int, eps: float = 1e-6):
-        super().__init__()
+        slopes = self.alibi.slopes.float().squeeze() if hasattr(self, "alibi") else None
 
-        self.eps = eps
-        self.register_parameter("weight", nn.Parameter(torch.ones(dim)))
+        dtype = query.dtype
 
-    def forward(self, x: Tensor) -> Tensor:
-        rms = torch.rsqrt(x.square().mean(dim=-1, keepdim=True) + self.eps)
-        return x * self.weight.type_as(x) * rms.type_as(x)
+        attn = flash_attn_kvpacked_func(
+            q=q.bfloat16(),
+            kv=kv.bfloat16(),
+            causal=is_causal,
+            alibi_slopes=slopes,
+        )
 
+        attn = rearrange(attn, "... h d -> ... (h d)")
+        return self.out_proj(attn).type(dtype)
 
-class LayerNormWrapper(nn.Module):
-    """
-    Wraps nn.LayerNorm as it doesn't really support mixed precision.
-    """
 
-    def __init__(self, dim: int, eps: float = 1e-6):
+class SelfAttention(nn.Module):
+    def __init__(
+        self,
+        embed_dim: int,
+        heads: int,
+        dropout: float = 0.0,
+        use_alibi: bool = True,
+    ):
         super().__init__()
 
-        self.ln = nn.LayerNorm(dim, eps=eps)
+        self.embed_size = embed_dim
+        self.num_heads = heads
+        self.head_dim = embed_dim // heads
+        self.dropout = dropout
 
-    def forward(self, x: Tensor) -> Tensor:
-        return self.ln(x).type_as(x)
+        assert (
+            self.head_dim * heads == embed_dim
+        ), "Embedding size needs to be divisible by heads"
 
+        self.qkv_proj = nn.Linear(self.embed_size, self.embed_size * 3)
 
-class FFNSwiGLU(nn.Module):
-    """
-    GLU Variants Improve Transformer
-    https://arxiv.org/abs/2002.05202
-    """
+        self.out_proj = nn.Linear(heads * self.head_dim, embed_dim)
 
-    def __init__(
+        if use_alibi:
+            self.alibi = ALiBi(heads)
+
+    def forward(
         self,
-        dim: int,
-        dim_feedforward: int,
-        out_dim: Optional[int] = None,
-        use_bias: bool = False,
-    ):
-        super().__init__()
+        x: Tensor,
+        pad_mask: Optional[Tensor] = None,
+        attn_mask: Optional[Tensor] = None,
+        is_causal: bool = False,
+    ) -> Tensor:
+        if can_flash(x, pad_mask, attn_mask):
+            return self.flash_forward(x, is_causal)
+
+        q, k, v = self.qkv_proj(x).chunk(3, dim=-1)
+
+        q = rearrange(q, "... n (h d) -> ... h n d", h=self.num_heads)
+        k = rearrange(k, "... n (h d) -> ... h n d", h=self.num_heads)
+        v = rearrange(v, "... n (h d) -> ... h n d", h=self.num_heads)
+
+        mask = combine_masks(attn_mask, pad_mask, self.num_heads, q.dtype)
 
-        out_dim = out_dim or dim
+        if hasattr(self, "alibi"):
+            bias = self.alibi(q, k)
+            mask = mask + bias if mask is not None else bias
 
-        self.w = nn.Linear(dim, dim_feedforward, bias=use_bias)
-        self.v = nn.Linear(dim, dim_feedforward, bias=use_bias)
-        self.w2 = nn.Linear(dim_feedforward, out_dim, bias=use_bias)
+        dropout = self.dropout if self.training else 0.0
+        attn = F.scaled_dot_product_attention(
+            q, k, v, mask, is_causal=is_causal, dropout_p=dropout
+        )
 
-    def forward(self, x: Tensor) -> Tensor:
-        x = F.silu(self.w(x)) * self.v(x)
-        return self.w2(x)
+        attn = rearrange(attn, "... h n d -> ... n (h d)")
+        return self.out_proj(attn)
 
+    def flash_forward(self, x: Tensor, is_causal: bool) -> Tensor:
+        qkv = self.qkv_proj(x)
+        qkv = rearrange(qkv, "... (n h d) -> ... n h d", h=self.num_heads, n=3)
 
-class FFNN(nn.Module):
-    def __init__(
-        self,
-        dim: int,
-        dim_feedforward: int,
-        out_dim: Optional[int] = None,
-        use_bias: bool = True,
-    ):
-        super().__init__()
+        slopes = None
+        if hasattr(self, "alibi"):
+            slopes = self.alibi.slopes.float().squeeze()
 
-        out_dim = out_dim or dim
+        dtype = x.dtype
 
-        self.block = nn.Sequential(
-            nn.Linear(dim, dim_feedforward, bias=use_bias),
-            nn.SiLU(),
-            nn.Linear(dim_feedforward, out_dim, bias=use_bias),
+        attn = flash_attn_qkvpacked_func(
+            qkv=qkv.bfloat16(), causal=is_causal, alibi_slopes=slopes
         )
 
-    def forward(self, x: Tensor) -> Tensor:
-        return self.block(x)
+        attn = rearrange(attn, "... h d -> ... (h d)")
+        return self.out_proj(attn).type(dtype)
 
 
 def combine_masks(
     attn_mask: Optional[Tensor],
     pad_mask: Optional[Tensor],
     heads: int = 1,
     dtype: Optional[torch.dtype] = None,
@@ -431,7 +454,20 @@
 def causal_mask(embed: Tensor) -> Tensor:
     """
     Creates a causal mask for self-attention.
     """
     mask = torch.full((embed.shape[1], embed.shape[1]), -torch.inf, device=embed.device, dtype=embed.dtype)  # fmt: skip
     mask = torch.triu(mask, diagonal=1)
     return mask
+
+
+def can_flash(
+    x: Tensor,
+    pad_mask: Optional[Tensor] = None,
+    attn_mask: Optional[Tensor] = None,
+):
+    return (
+        pad_mask is None
+        and attn_mask is None
+        and FLASH_AVAILABLE
+        and x.device.type != "cpu"
+    )
```

### Comparing `hnn_utils-0.2.4/hnn_utils/nn/functional.py` & `hnn_utils-0.3.0/hnn_utils/nn/functional.py`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.2.4/PKG-INFO` & `hnn_utils-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hnn_utils
-Version: 0.2.4
+Version: 0.3.0
 Summary: Various utilities used throughout my research
 Author: Haydn Jones
 Author-email: haydnjonest@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

