# Comparing `tmp/s5-pytorch-0.1.9.tar.gz` & `tmp/s5-pytorch-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s5-pytorch-0.1.9.tar", last modified: Sun Jun 25 10:32:41 2023, max compression
+gzip compressed data, was "s5-pytorch-0.2.0.tar", last modified: Thu Apr 25 11:45:34 2024, max compression
```

## Comparing `s5-pytorch-0.1.9.tar` & `s5-pytorch-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 null      (1000) null      (1000)        0 2023-06-25 10:32:41.277875 s5-pytorch-0.1.9/
--rw-r--r--   0 null      (1000) null      (1000)    16727 2023-05-27 11:40:20.000000 s5-pytorch-0.1.9/LICENSE
--rw-r--r--   0 null      (1000) null      (1000)     2122 2023-06-25 10:32:41.277875 s5-pytorch-0.1.9/PKG-INFO
--rw-r--r--   0 null      (1000) null      (1000)     1444 2023-05-27 11:40:20.000000 s5-pytorch-0.1.9/README.md
-drwxr-xr-x   0 null      (1000) null      (1000)        0 2023-06-25 10:32:41.276875 s5-pytorch-0.1.9/s5/
--rw-r--r--   0 null      (1000) null      (1000)       24 2023-05-27 11:40:20.000000 s5-pytorch-0.1.9/s5/__init__.py
--rw-r--r--   0 null      (1000) null      (1000)     8786 2023-05-27 11:40:20.000000 s5-pytorch-0.1.9/s5/init.py
--rw-r--r--   0 null      (1000) null      (1000)    15899 2023-06-25 09:50:15.000000 s5-pytorch-0.1.9/s5/jax_compat.py
--rw-r--r--   0 null      (1000) null      (1000)    17474 2023-06-25 10:29:18.000000 s5-pytorch-0.1.9/s5/s5_model.py
-drwxr-xr-x   0 null      (1000) null      (1000)        0 2023-06-25 10:32:41.277875 s5-pytorch-0.1.9/s5_pytorch.egg-info/
--rw-r--r--   0 null      (1000) null      (1000)     2122 2023-06-25 10:32:41.000000 s5-pytorch-0.1.9/s5_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 null      (1000) null      (1000)      253 2023-06-25 10:32:41.000000 s5-pytorch-0.1.9/s5_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 null      (1000) null      (1000)        1 2023-06-25 10:32:41.000000 s5-pytorch-0.1.9/s5_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 null      (1000) null      (1000)       34 2023-06-25 10:32:41.000000 s5-pytorch-0.1.9/s5_pytorch.egg-info/requires.txt
--rw-r--r--   0 null      (1000) null      (1000)        3 2023-06-25 10:32:41.000000 s5-pytorch-0.1.9/s5_pytorch.egg-info/top_level.txt
--rw-r--r--   0 null      (1000) null      (1000)       38 2023-06-25 10:32:41.277875 s5-pytorch-0.1.9/setup.cfg
--rw-r--r--   0 null      (1000) null      (1000)     1023 2023-06-25 10:32:18.000000 s5-pytorch-0.1.9/setup.py
+drwxr-xr-x   0 null      (1000) null      (1000)        0 2024-04-25 11:45:34.978487 s5-pytorch-0.2.0/
+-rw-r--r--   0 null      (1000) null      (1000)    16727 2023-03-21 00:02:05.000000 s5-pytorch-0.2.0/LICENSE
+-rw-r--r--   0 null      (1000) null      (1000)     2293 2024-04-25 11:45:34.978487 s5-pytorch-0.2.0/PKG-INFO
+-rw-r--r--   0 null      (1000) null      (1000)     1615 2024-04-25 11:42:15.000000 s5-pytorch-0.2.0/README.md
+drwxr-xr-x   0 null      (1000) null      (1000)        0 2024-04-25 11:45:34.978487 s5-pytorch-0.2.0/s5/
+-rw-r--r--   0 null      (1000) null      (1000)       24 2023-01-16 11:22:05.000000 s5-pytorch-0.2.0/s5/__init__.py
+-rw-r--r--   0 null      (1000) null      (1000)     8786 2023-02-08 11:34:23.000000 s5-pytorch-0.2.0/s5/init.py
+-rw-r--r--   0 null      (1000) null      (1000)     5453 2024-04-25 11:30:10.000000 s5-pytorch-0.2.0/s5/jax_bench.py
+-rw-r--r--   0 null      (1000) null      (1000)    15875 2024-04-25 11:38:15.000000 s5-pytorch-0.2.0/s5/jax_compat.py
+-rw-r--r--   0 null      (1000) null      (1000)    19749 2024-04-25 11:33:29.000000 s5-pytorch-0.2.0/s5/s5_model.py
+drwxr-xr-x   0 null      (1000) null      (1000)        0 2024-04-25 11:45:34.978487 s5-pytorch-0.2.0/s5_pytorch.egg-info/
+-rw-r--r--   0 null      (1000) null      (1000)     2293 2024-04-25 11:45:34.000000 s5-pytorch-0.2.0/s5_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 null      (1000) null      (1000)      269 2024-04-25 11:45:34.000000 s5-pytorch-0.2.0/s5_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 null      (1000) null      (1000)        1 2024-04-25 11:45:34.000000 s5-pytorch-0.2.0/s5_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 null      (1000) null      (1000)       27 2024-04-25 11:45:34.000000 s5-pytorch-0.2.0/s5_pytorch.egg-info/requires.txt
+-rw-r--r--   0 null      (1000) null      (1000)        3 2024-04-25 11:45:34.000000 s5-pytorch-0.2.0/s5_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 null      (1000) null      (1000)       38 2024-04-25 11:45:34.978487 s5-pytorch-0.2.0/setup.cfg
+-rw-r--r--   0 null      (1000) null      (1000)     1057 2024-04-25 11:40:23.000000 s5-pytorch-0.2.0/setup.py
```

### Comparing `s5-pytorch-0.1.9/LICENSE` & `s5-pytorch-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `s5-pytorch-0.1.9/PKG-INFO` & `s5-pytorch-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s5-pytorch
-Version: 0.1.9
+Version: 0.2.0
 Summary: S5 - Simplified State Space Layers for Sequence Modeling - Pytorch
 Home-page: https://github.com/i404788/s5-pytorch
 Author: Ferris Kwaijtaal
 Author-email: ferris+gh@devdroplets.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
@@ -15,16 +15,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # S5: Simplified State Space Layers for Sequence Modeling
 This is a ported version derived from <https://github.com/lindermanlab/S5> and <https://github.com/kavorite/S5>.
 It includes a bunch of functions ported from jax/lax/flax/whatever since they didn't exist yet. 
 
-Jax is required because it relies on the pytree structure but it's not used for any computation. 
-Pytorch 1.13 or later is required because it makes heavy use of `functorch.vamp` to substitute it's jax counterpart.
+~~Jax is required because it relies on the pytree structure but it's not used for any computation.~~
+Since version 0.2.0 jax is not required, it's using the pytorch native `torch.utils._pytree` (this may be incompatible for pytorch future versions).
+Pytorch 2 or later is required because it makes heavy use of `torch.vmap` and `torch.utils._pytree` to substitute it's jax counterpart.
 Python 3.10 or later is required due to usage of the `match` keyword
 
 \--- 
 
 Update:
 
 In my experiments it follows the results found in the [Hyena Hierarchy](https://arxiv.org/abs/2302.10866) (& H3) paper that the state spaces alone lack the recall capabilities required for LLM but seem work well for regular sequence feature extraction and linear complexity.
```

### Comparing `s5-pytorch-0.1.9/README.md` & `s5-pytorch-0.2.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # S5: Simplified State Space Layers for Sequence Modeling
 This is a ported version derived from <https://github.com/lindermanlab/S5> and <https://github.com/kavorite/S5>.
 It includes a bunch of functions ported from jax/lax/flax/whatever since they didn't exist yet. 
 
-Jax is required because it relies on the pytree structure but it's not used for any computation. 
-Pytorch 1.13 or later is required because it makes heavy use of `functorch.vamp` to substitute it's jax counterpart.
+~~Jax is required because it relies on the pytree structure but it's not used for any computation.~~
+Since version 0.2.0 jax is not required, it's using the pytorch native `torch.utils._pytree` (this may be incompatible for pytorch future versions).
+Pytorch 2 or later is required because it makes heavy use of `torch.vmap` and `torch.utils._pytree` to substitute it's jax counterpart.
 Python 3.10 or later is required due to usage of the `match` keyword
 
 \--- 
 
 Update:
 
 In my experiments it follows the results found in the [Hyena Hierarchy](https://arxiv.org/abs/2302.10866) (& H3) paper that the state spaces alone lack the recall capabilities required for LLM but seem work well for regular sequence feature extraction and linear complexity.
```

### Comparing `s5-pytorch-0.1.9/s5/init.py` & `s5-pytorch-0.2.0/s5/init.py`

 * *Files identical despite different names*

### Comparing `s5-pytorch-0.1.9/s5/jax_compat.py` & `s5-pytorch-0.2.0/s5/jax_compat.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import torch
-import functorch
 import numpy as np
-from jax.tree_util import tree_flatten, tree_unflatten
-from typing import overload, Callable, Iterable, List, TypeVar, Any, Literal, Union, Sequence, Tuple, Optional
+from torch.utils._pytree import tree_flatten, tree_unflatten
+from typing import overload, Callable, Iterable, List, TypeVar, Any, Literal, Sequence, Optional
 from functools import partial
-from einops import rearrange
 import math
 
 """
 Jax-Pytorch ported functions, mostly interfaces are kept the same but unsupported features are removed:
 * Jax-Keyed RNGs are sampled from global RNG
 * Canonical/Named shapes/dtypes/etc are now regular shapes,dtypes
 """
@@ -39,162 +37,164 @@
     args = list(map(list, args))
     n = len(args[0])
     for arg in args[1:]:
         assert len(arg) == n, f'length mismatch: {list(map(len, args))}'
     return list(map(f, *args))
 
 
-def slice_along_axis(start, end, stride=None, axis=0):
-    return (slice(None),) * axis + (slice(start, end, stride),)
+def combine(tree, operator, a_flat, b_flat):
+    # Lower `fn` to operate on flattened sequences of elems.
+    a = tree_unflatten(a_flat, tree)
+    b = tree_unflatten(b_flat, tree)
+    c = operator(a, b)
+    c_flat, _ = tree_flatten(c)
+    return c_flat
+
+
+def _scan(tree, operator, elems, axis: int):
+    """Perform scan on `elems`."""
+    num_elems = elems[0].shape[axis]
+
+    if num_elems < 2:
+        return elems
+
+    # Combine adjacent pairs of elements.
+    reduced_elems = combine(tree, operator,
+                            [torch.ops.aten.slice(elem, axis, 0, -1, 2) for elem in elems],
+                            [torch.ops.aten.slice(elem, axis, 1, None, 2) for elem in elems])
+
+    # Recursively compute scan for partially reduced tensors.
+    odd_elems = _scan(tree, operator, reduced_elems, axis)
+
+    if num_elems % 2 == 0:
+        even_elems = combine(tree, operator,
+                             [torch.ops.aten.slice(e, axis, 0, -1) for e in odd_elems],
+                             [torch.ops.aten.slice(e, axis, 2, None, 2) for e in elems])
+    else:
+        even_elems = combine(tree, operator,
+                             odd_elems,
+                             [torch.ops.aten.slice(e, axis, 2, None, 2) for e in elems])
+
+    # The first element of a scan is the same as the first element
+    # of the original `elems`.
+    even_elems = [
+        torch.cat([torch.ops.aten.slice(elem, axis, 0, 1), result], dim=axis)
+        if result.shape.numel() > 0 and elem.shape[axis] > 0 else
+        result if result.shape.numel() > 0 else
+        torch.ops.aten.slice(elem, axis, 0, 1)  # Jax allows/ignores concat with 0-dim, Pytorch does not
+        for (elem, result) in zip(elems, even_elems)]
 
+    return list(safe_map(partial(_interleave, axis=axis), even_elems, odd_elems))
 
 # Pytorch impl. of jax.lax.associative_scan
-def associative_scan(operator, elems, axis=0, reverse=False):
-    if not callable(operator):
-        raise TypeError("lax.associative_scan: fn argument should be callable.")
+
+
+def associative_scan(operator: Callable, elems, axis: int = 0, reverse: bool = False):
+    # if not callable(operator):
+    #     raise TypeError("lax.associative_scan: fn argument should be callable.")
     elems_flat, tree = tree_flatten(elems)
 
     if reverse:
         elems_flat = [torch.flip(elem, [axis]) for elem in elems_flat]
 
-    def combine(a_flat, b_flat):
-        # Lower `fn` to operate on flattened sequences of elems.
-        a = tree_unflatten(tree, a_flat)
-        b = tree_unflatten(tree, b_flat)
-        c = operator(a, b)
-        c_flat, _ = tree_flatten(c)
-        return c_flat
-
     assert axis >= 0 or axis < elems_flat[0].ndim, "Axis should be within bounds of input"
     num_elems = int(elems_flat[0].shape[axis])
     if not all(int(elem.shape[axis]) == num_elems for elem in elems_flat[1:]):
         raise ValueError('Array inputs to associative_scan must have the same '
                          'first dimension. (saw: {})'
                          .format([elem.shape for elem in elems_flat]))
 
-    def _scan(elems):
-        """Perform scan on `elems`."""
-        num_elems = elems[0].shape[axis]
-
-        if num_elems < 2:
-            return elems
-
-        # Combine adjacent pairs of elements.
-        reduced_elems = combine(
-          [elem[slice_along_axis(0, -1, stride=2, axis=axis)] for elem in elems],
-          [elem[slice_along_axis(1, None, stride=2, axis=axis)] for elem in elems])
-
-        # Recursively compute scan for partially reduced tensors.
-        odd_elems = _scan(reduced_elems)
-
-        if num_elems % 2 == 0:
-            even_elems = combine(
-                [e[slice_along_axis(0, -1, axis=axis)] for e in odd_elems],
-                [e[slice_along_axis(2, None, stride=2, axis=axis)] for e in elems])
-        else:
-            even_elems = combine(
-                odd_elems,
-                [e[slice_along_axis(2, None, stride=2, axis=axis)] for e in elems])
-
-        # The first element of a scan is the same as the first element
-        # of the original `elems`.
-        even_elems = [
-          torch.cat([elem[slice_along_axis(0, 1, axis=axis)], result], dim=axis)
-          if result.shape.numel() > 0 and elem.shape[axis] > 0 else
-          result if result.shape.numel() > 0 else
-          elem[slice_along_axis(0, 1, axis=axis)]  # Jax allows/ignores concat with 0-dim, Pytorch does not
-          for (elem, result) in zip(elems, even_elems)]
-
-        return list(safe_map(partial(_interleave, axis=axis), even_elems, odd_elems))
-
-    scans = _scan(elems_flat)
+    scans = _scan(tree, operator, elems_flat, axis)
 
     if reverse:
         scans = [torch.flip(scanned, [axis]) for scanned in scans]
 
-    return tree_unflatten(tree, scans)
+    return tree_unflatten(scans, tree)
+
 
 def test_associative_scan(shape=(1, 24, 24)):
     import jax.lax
     import jax
 
     x = np.random.randn(*shape)
     jx = jax.numpy.array(x)
     tx = torch.tensor(x, dtype=torch.float32)
-    
-    def nested_func(a,b):
-        a_i,b_i = a
-        a_j,b_j = b
+
+    def nested_func(a, b):
+        a_i, b_i = a
+        a_j, b_j = b
         return a_j*a_i, a_j*b_i + b_j
     jy1, jy2 = jax.lax.associative_scan(nested_func, (jx, jx))
-    ty1, ty2 = associative_scan(nested_func, (tx,tx))
+    ty1, ty2 = associative_scan(nested_func, (tx, tx))
     assert np.isclose(ty1.numpy(), np.array(jy1)).all() and np.isclose(ty2.numpy(), np.array(jy2)).all(), "Expected jax & pytorch impl to be close"
 
     jy1, jy2 = jax.lax.associative_scan(nested_func, (jx, jx), reverse=True)
-    ty1, ty2 = associative_scan(nested_func, (tx,tx), reverse=True)
+    ty1, ty2 = associative_scan(nested_func, (tx, tx), reverse=True)
     assert np.isclose(ty1.numpy(), np.array(jy1)).all() and np.isclose(ty2.numpy(), np.array(jy2)).all(), "Expected jax & pytorch reverse impl to be close"
-    
-    
+
 
 # def _interleave(a, b, axis):
 #     assert a.shape[axis] == b.shape[axis] or a.shape[axis] == b.shape[axis] + 1
 #     if b_trunc := (a.shape[axis] == b.shape[axis] + 1):
 #         pad = [0, 0] * b.ndim
 #         pad[(b.ndim-axis-1)*2+1] = 1 # +1=always end of dim, pad-order is reversed so start is at end
 #         b = torch.nn.functional.pad(b, pad)
-        
+
 #     keys = list('ijklmnop')[:a.ndim]  # Get enough keys for each dim
 #     expr = 't ' + ' '.join(keys) + ' -> '
 
 #     keys[axis] = f'({keys[axis]} t)'  # Interleave along desired axis
 #     expr += ' '.join(keys)
 #     # for example 't i j -> (i t) j'
 #     out: torch.Tensor = rearrange([a, b], expr)
 #     if b_trunc:
 #         out = out[slice_along_axis(0, b.shape[axis]+a.shape[axis]-1, axis=axis)]
 #     return out
 
-def _interleave(a, b, axis):
+# @torch.jit.script
+def _interleave(a, b, axis: int):
     # https://stackoverflow.com/questions/60869537/how-can-i-interleave-5-pytorch-tensors
-    if b_trunc := (a.shape[axis] == b.shape[axis] + 1):
+    b_trunc = (a.shape[axis] == b.shape[axis] + 1)
+    if b_trunc:
         pad = [0, 0] * b.ndim
-        pad[(b.ndim-axis-1)*2+1] = 1 # +1=always end of dim, pad-order is reversed so start is at end
+        pad[(b.ndim-axis-1)*2+1] = 1  # +1=always end of dim, pad-order is reversed so start is at end
         b = torch.nn.functional.pad(b, pad)
 
     stacked = torch.stack([a, b], dim=axis+1)
     interleaved = torch.flatten(stacked, start_dim=axis, end_dim=axis+1)
     if b_trunc:
         # TODO: find torch alternative for slice_along axis for torch.jit.script to work
-        interleaved = interleaved[slice_along_axis(0, b.shape[axis]+a.shape[axis]-1, axis=axis)]
+        interleaved = torch.ops.aten.slice(interleaved, axis, 0, b.shape[axis]+a.shape[axis]-1)
     return interleaved
 
+
 def test_interleave():
-    x,y = torch.randn(1, 32, 32), torch.randn(1, 32, 32)
-    v = _interleave(x,y, axis=1)
-    assert v.shape == (1,64,32)
+    x, y = torch.randn(1, 32, 32), torch.randn(1, 32, 32)
+    v = _interleave(x, y, axis=1)
+    assert v.shape == (1, 64, 32)
     assert (v[:, 0] == x[:, 0]).all()
     assert (v[:, 1] == y[:, 0]).all()
     assert (v[:, 2] == x[:, 1]).all()
     assert (v[:, 3] == y[:, 1]).all()
     assert (v[:, 4] == x[:, 2]).all()
 
-    v = _interleave(x,y, axis=2)
-    assert v.shape == (1,32,64)
+    v = _interleave(x, y, axis=2)
+    assert v.shape == (1, 32, 64)
     assert (v[..., 0] == x[..., 0]).all()
     assert (v[..., 1] == y[..., 0]).all()
     assert (v[..., 2] == x[..., 1]).all()
     assert (v[..., 3] == y[..., 1]).all()
     assert (v[..., 4] == x[..., 2]).all()
 
-    x,y = torch.randn(1, 24, 24), torch.randn(1, 24, 24)
-    assert _interleave(x,y, axis=1).shape == (1,48,24)
-    assert _interleave(x,y, axis=2).shape == (1,24,48)
+    x, y = torch.randn(1, 24, 24), torch.randn(1, 24, 24)
+    assert _interleave(x, y, axis=1).shape == (1, 48, 24)
+    assert _interleave(x, y, axis=2).shape == (1, 24, 48)
 
-    x,y = torch.randn(3, 96), torch.randn(2, 96)
-    v = _interleave(x,y,axis=0)
+    x, y = torch.randn(3, 96), torch.randn(2, 96)
+    v = _interleave(x, y, axis=0)
     assert v.shape == (5, 96)
     assert (v[0] == x[0]).all()
     assert (v[1] == y[0]).all()
     assert (v[2] == x[1]).all()
     assert (v[3] == y[1]).all()
     assert (v[4] == x[2]).all()
     print('Interleave working as expected!')
@@ -359,15 +359,14 @@
          [-0.61677957, -0.67402434,  0.09683388]], dtype=float32)
 
     .. _Lecun normal initializer: https://arxiv.org/abs/1706.02515
     """
     return variance_scaling(1.0, "fan_in", "truncated_normal", fan_in_axes=fan_in_axes, dtype=dtype)
 
 
-
 def test_variance_scaling():
     v = variance_scaling(1.0, distribution='normal')
     n_f32 = v((1, 10000), dtype=torch.float)
     assert np.isclose(n_f32.std().item(), 1.0, rtol=0.015, atol=0.015), f'std for f32 normal[0,1.0] is {n_f32.std()} != 1.0'
     del n_f32
     # NOTE: this is used in the original as `complex_normal` (but with stddev=0.5**0.5)
     n_c64 = v((1, 10000), dtype=torch.complex64)
@@ -398,9 +397,9 @@
 #    del tn_c64
 
 
 if __name__ == '__main__':
     test_variance_scaling()
     test_interleave()
     test_associative_scan()
-    test_associative_scan(shape=(2,256,24))
+    test_associative_scan(shape=(2, 256, 24))
     test_associative_scan(shape=(360, 96))
```

### Comparing `s5-pytorch-0.1.9/s5/s5_model.py` & `s5-pytorch-0.2.0/s5/s5_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-import functorch
 import torch
 import torch.nn.functional as F
-import numpy as np
-from typing import overload, Callable, Iterable, List, TypeVar, Any, Literal, Union, Sequence, Tuple, Optional
+from typing import Tuple, Optional, Literal
 from .jax_compat import associative_scan
 from .init import *
 
 # Runtime functions
 
 
 @torch.jit.script
@@ -19,60 +17,71 @@
         new element ( A_out, Bu_out )
     """
     A_i, b_i = q_i
     A_j, b_j = q_j
     # return A_j * A_i, A_j * b_i + b_j
     return A_j * A_i, torch.addcmul(b_j, A_j, b_i)
 
-def apply_ssm(Lambda_bars: torch.Tensor, B_bars, C_tilde, D, input_sequence, bidir: bool = False):
+
+def apply_ssm(Lambda_bars: torch.Tensor, B_bars, C_tilde, D, input_sequence, state=None, bidir: bool = False):
     cinput_sequence = input_sequence.type(Lambda_bars.dtype)  # Cast to correct complex type
 
     if B_bars.ndim == 3:
         # Dynamic timesteps (significantly more expensive)
-        Bu_elements = functorch.vmap(lambda B_bar, u: B_bar @ u)(B_bars, cinput_sequence)
+        Bu_elements = torch.vmap(lambda B_bar, u: B_bar @ u)(B_bars, cinput_sequence)
     else:
         # Static timesteps
-        Bu_elements = functorch.vmap(lambda u: B_bars @ u)(cinput_sequence)
+        Bu_elements = torch.vmap(lambda u: B_bars @ u)(cinput_sequence)
 
-    if Lambda_bars.ndim == 1: # Repeat for associative_scan
-        Lambda_bars = Lambda_bars.tile(input_sequence.shape[0], 1)
+    if Lambda_bars.ndim == 1:  # Zero-pad for associative_scan
+        # Lambda_bars = Lambda_bars.tile(input_sequence.shape[0], 1)
+        Lambda_bars = F.pad(Lambda_bars.unsqueeze(0), (0, 0, 0, input_sequence.shape[0]-1), 'constant', value=0)
+
+    if state is not None:
+        # Replace initial x_k with state if provided
+        Lambda_bars[:] = state
 
     _, xs = associative_scan(binary_operator, (Lambda_bars, Bu_elements))
 
     if bidir:
         _, xs2 = associative_scan(binary_operator, (Lambda_bars, Bu_elements), reverse=True)
         xs = torch.cat((xs, xs2), axis=-1)
 
-    Du = functorch.vmap(lambda u: D * u)(input_sequence)
+    Du = torch.vmap(lambda u: D * u)(input_sequence)
     # TODO: the last element of xs (non-bidir) is the hidden state, allow returning it
-    return functorch.vmap(lambda x: (C_tilde @ x).real)(xs) + Du
+    return torch.vmap(lambda x: (C_tilde @ x).real)(xs) + Du, xs[-1]
+
 
-def apply_ssm_liquid(Lambda_bars, B_bars, C_tilde, D, input_sequence, bidir: bool = False):
+def apply_ssm_liquid(Lambda_bars, B_bars, C_tilde, D, input_sequence, state=None, bidir: bool = False):
     """Liquid time constant SSM \u00e1 la dynamical systems given in Eq. 8 of
     https://arxiv.org/abs/2209.12951"""
     cinput_sequence = input_sequence.type(Lambda_bars.dtype)  # Cast to correct complex type
 
     if B_bars.ndim == 3:
         # Dynamic timesteps (significantly more expensive)
-        Bu_elements = functorch.vmap(lambda B_bar, u: B_bar @ u)(B_bars, cinput_sequence)
+        Bu_elements = torch.vmap(lambda B_bar, u: B_bar @ u)(B_bars, cinput_sequence)
     else:
         # Static timesteps
-        Bu_elements = functorch.vmap(lambda u: B_bars @ u)(cinput_sequence)
+        Bu_elements = torch.vmap(lambda u: B_bars @ u)(cinput_sequence)
+
+    if Lambda_bars.ndim == 1:  # Zero-pad for associative_scan
+        Lambda_bars = F.pad(Lambda_bars.unsqueeze(0), (0, 0, 0, input_sequence.shape[0]-1), 'constant', value=0)
 
-    if Lambda_bars.ndim == 1: # Repeat for associative_scan
-        Lambda_bars = Lambda_bars.tile(input_sequence.shape[0], 1)
+    if state is not None:
+        # Replace initial x_k with state if provided
+        Lambda_bars[:] = state
 
     _, xs = associative_scan(binary_operator, (Lambda_bars + Bu_elements, Bu_elements))
 
     if bidir:
         _, xs2 = associative_scan(binary_operator, (Lambda_bars, Bu_elements), reverse=True)
         xs = torch.cat((xs, xs2), axis=-1)
 
-    Du = functorch.vmap(lambda u: D * u)(input_sequence)
-    return functorch.vmap(lambda x: (C_tilde @ x).real)(xs) + Du
+    Du = torch.vmap(lambda u: D * u)(input_sequence)
+    return torch.vmap(lambda x: (C_tilde @ x).real)(xs) + Du, xs[-1]
 
 
 # Discretization functions
 def discretize_bilinear(Lambda, B_tilde, Delta):
     """Discretize a diagonalized, continuous-time linear SSM
     using bilinear transform method.
     Args:
@@ -84,27 +93,28 @@
     """
     Identity = torch.ones(Lambda.shape[0], device=Lambda.device)
     BL = 1 / (Identity - (Delta / 2.0) * Lambda)
     Lambda_bar = BL * (Identity + (Delta / 2.0) * Lambda)
     B_bar = (BL * Delta)[..., None] * B_tilde
     return Lambda_bar, B_bar
 
+
 def discretize_zoh(Lambda, B_tilde, Delta):
     """Discretize a diagonalized, continuous-time linear SSM
     using zero-order hold method.
     Args:
         Lambda (complex64): diagonal state matrix              (P,)
         B_tilde (complex64): input matrix                      (P, H)
         Delta (float32): discretization step sizes             (P,)
     Returns:
         discretized Lambda_bar (complex64), B_bar (complex64)  (P,), (P,H)
     """
-    # Identity = torch.ones(Lambda.shape[0], device=Lambda.device) # (replaced by -1)
+    Identity = torch.ones(Lambda.shape[0], device=Lambda.device) # (replaced by -1)
     Lambda_bar = torch.exp(Lambda * Delta)
-    B_bar = (1 / Lambda * (Lambda_bar - 1))[..., None] * B_tilde
+    B_bar = (1 / Lambda * (Lambda_bar - Identity))[..., None] * B_tilde
     return Lambda_bar, B_bar
 
 
 def as_complex(t: torch.Tensor, dtype=torch.complex64):
     assert t.shape[-1] == 2, "as_complex can only be done on tensors with shape=(...,2)"
     nt = torch.complex(t[..., 0], t[..., 1])
     if nt.dtype != dtype:
@@ -243,31 +253,43 @@
             Lambda_bar += Bu
         # https://arxiv.org/abs/2208.04933v2, Eq. 2
         x = Lambda_bar * prev_state + Bu
         y = (C_tilde @ x + self.D * signal).real
         return y, x
 
     # NOTE: can only be used as RNN OR S5(MIMO) (no mixing)
-    def forward(self, signal, step_scale: float | torch.Tensor = 1.0):
+    def forward(self, signal, step_scale: float | torch.Tensor = 1.0, state=None, return_state=False):
         B_tilde, C_tilde = self.get_BC_tilde()
-        if self.degree != 1:
-            assert (B_bar.shape[-2] == B_bar.shape[-1]), "higher-order input operators must be full-rank"
-            B_bar **= self.degree
 
         if not torch.is_tensor(step_scale) or step_scale.ndim == 0:
-            #step_scale = torch.ones(signal.shape[-2], device=signal.device) * step_scale
             step = step_scale * torch.exp(self.log_step)
         else:
             # TODO: This is very expensive due to individual steps being multiplied by B_tilde in self.discretize
             step = step_scale[:, None] * torch.exp(self.log_step)
 
+        # print(f'{self.Lambda.shape=} {B_tilde.shape=} {step.shape=}')
+        # Lambda_bars, B_bars = torch.vmap(lambda s: self.discretize(self.Lambda, B_tilde, s))(step)
+        # print(Lambda_bars.shape, B_bars.shape)
         Lambda_bars, B_bars = self.discretize(self.Lambda, B_tilde, step)
-        # Lambda_bars, B_bars = functorch.vmap(self.discretize, (None, None, 0))(self.Lambda, B_tilde, step)
+        if self.degree != 1:
+            assert (B_bars.shape[-2] == B_bars.shape[-1]), "higher-order input operators must be full-rank"
+            B_bars **= self.degree
+
+        assert not (self.bidir and (state is not None)), "injecting state is not compatible with bidirectional S5"
+
         forward = apply_ssm_liquid if self.liquid else apply_ssm
-        return forward(Lambda_bars, B_bars, C_tilde, self.D, signal, bidir=self.bidir)
+        out, state = forward(Lambda_bars, B_bars, C_tilde, self.D, signal, state=state, bidir=self.bidir)
+        # NOTE: technically it could work in a limited sense; taking the first and last element
+        #   but that wouldn't be equivalent to running bidir on full sequences.
+        #  It would be more like a circular S5 where you keep splicing the new signal into it;
+        #   we leave implementing/testing this as an exercise to the reader
+        assert not (self.bidir and return_state), "return_state does not work with bidirectional S5"
+        if return_state:
+            return out, state
+        return out
 
 
 class S5(torch.nn.Module):
     def __init__(self,
                  width: int,
                  state_width: Optional[int] = None,
                  factor_rank: Optional[int] = None,
@@ -310,70 +332,99 @@
             degree=degree,
             bidir=bidir
         )
 
     def initial_state(self, batch_size: Optional[int] = None):
         return self.seq.initial_state(batch_size)
 
-    def forward(self, signal, step_scale: float | torch.Tensor = 1.0):
+    def forward(self, signal, step_scale: float | torch.Tensor = 1.0, state=None, return_state=False):
         # NOTE: step_scale can be float | Tensor[batch] | Tensor[batch, seq]
         if not torch.is_tensor(step_scale):
             # Duplicate across batchdim
             step_scale = torch.ones(signal.shape[0], device=signal.device) * step_scale
 
-        return functorch.vmap(lambda s, ss: self.seq(s, step_scale=ss))(signal, step_scale)
-        #return self.seq(signal, prev_state=prev_state, step_scale=step_scale)
+        if state is None:
+            return torch.vmap(lambda s, ss: self.seq(s, step_scale=ss, return_state=return_state))(signal, step_scale)
+        else:
+            return torch.vmap(lambda s, ss, _state: self.seq(s, step_scale=ss, state=_state, return_state=return_state))(signal, step_scale, state)
+
 
 class GEGLU(torch.nn.Module):
     def forward(self, x):
-        x, gates = x.chunk(2, dim = -1)
+        x, gates = x.chunk(2, dim=-1)
         return x * F.gelu(gates)
 
+
 class S5Block(torch.nn.Module):
-    def __init__(self, dim: int, state_dim: int, bidir: bool, block_count: int = 1, liquid: bool = False, degree: int = 1, factor_rank: int | None = None, bcInit: Optional[Initialization] = None, ff_mult: float = 1., glu: bool = True, 
+    def __init__(self, dim: int, state_dim: int, bidir: bool, block_count: int = 1, liquid: bool = False, degree: int = 1, factor_rank: int | None = None, bcInit: Optional[Initialization] = None, ff_mult: float = 1., glu: bool = True,
                  ff_dropout: float = 0.0, attn_dropout: float = 0.0):
         super().__init__()
         self.s5 = S5(dim, state_width=state_dim, bidir=bidir, block_count=block_count, liquid=liquid, degree=degree, factor_rank=factor_rank, bcInit=bcInit)
         self.attn_norm = torch.nn.LayerNorm(dim)
         self.attn_dropout = torch.nn.Dropout(p=attn_dropout)
         self.geglu = GEGLU() if glu else None
         self.ff_enc = torch.nn.Linear(dim, int(dim * ff_mult) * (1 + glu), bias=False)
         self.ff_dec = torch.nn.Linear(int(dim * ff_mult), dim, bias=False)
         self.ff_norm = torch.nn.LayerNorm(dim)
         self.ff_dropout = torch.nn.Dropout(p=ff_dropout)
-    
-    def forward(self, x):
+
+    def forward(self, x, state=None, return_state=False):
         # Standard transfomer-style block with GEGLU/Pre-LayerNorm
         fx = self.attn_norm(x)
         res = fx.clone()
-        x = F.gelu(self.s5(fx)) + res
+        x = self.s5(fx, state=state, return_state=return_state)
+        if return_state:
+            x, next_state = x
+
+        x = F.gelu(x) + res
         x = self.attn_dropout(x)
 
         fx = self.ff_norm(x)
         res = fx.clone()
         x = self.ff_enc(fx)
         if self.geglu is not None:
             x = self.geglu(x)
         x = self.ff_dec(x) + res
-        x = self.ff_dropout(x) # TODO: test if should be placed inbetween ff or after ff
+        x = self.ff_dropout(x)  # TODO: test if should be placed inbetween ff or after ff
+
+        if return_state:
+            return x, next_state
         return x
 
 
 if __name__ == '__main__':
-    import lovely_tensors as lt
-    lt.monkey_patch()
+    # import lovely_tensors as lt
+    # lt.monkey_patch()
 
     def tensor_stats(t: torch.Tensor):  # Clone of lovely_tensors for complex support
         return f'tensor[{t.shape}] n={t.shape.numel()}, u={t.mean()}, s={round(t.std().item(), 3)} var={round(t.var().item(), 3)}\n'
 
-    x = torch.rand([2, 256, 32]).cuda()
-    model = S5(32, 32, factor_rank=None).cuda()
+    x = torch.rand([2, 768, 32])
+    model = S5(32, 128)
     print('B', tensor_stats(model.seq.B.data))
     print('C', tensor_stats(model.seq.C.data))
-    #print('B', tensor_stats(model.seq.BH.data), tensor_stats(model.seq.BP.data))
-    #print('C', tensor_stats(model.seq.CH.data), tensor_stats(model.seq.CP.data))
+    # print('B', tensor_stats(model.seq.BH.data), tensor_stats(model.seq.BP.data))
+    # print('C', tensor_stats(model.seq.CH.data), tensor_stats(model.seq.CP.data))
     # FIXME: unstable initialization
     # state = model.initial_state(256)
     # res = model(x, prev_state=state)
     # print(res.shape, res.dtype, res)
-    res = model(x) # warm-up
-    print(res.shape, res.dtype, res)
+    res, state = model(x, return_state=True)
+    print(state.shape, state.dtype, tensor_stats(state), f'{state[:, :10]=}')
+    print(res.shape, res.dtype, res[:, -255])
+
+    print("Now with 100% more state:")
+    res, state = model(x[:, :256], return_state=True)
+    # print(state.shape, state.dtype, tensor_stats(state))
+    # print(res.shape, res.dtype, res)
+    res, state = model(x[:, 256:512], state=state, return_state=True)
+    # print(state.shape, state.dtype, tensor_stats(state))
+    # print(res.shape, res.dtype, res)
+    res, state = model(x[:, 512:768], state=state, return_state=True)
+    print(state.shape, state.dtype, tensor_stats(state), f'{state[:, :10]=}')
+    print(res.shape, res.dtype, res[:, -255])
+
+    print("Corrupted state (negative test):")
+    res, state = model(x[:, 512:768], state=torch.randn_like(state), return_state=True)
+    print(state.shape, state.dtype, tensor_stats(state), f'{state[:, :10]=}')
+    print(res.shape, res.dtype, res[:, -255])
+
```

### Comparing `s5-pytorch-0.1.9/s5_pytorch.egg-info/PKG-INFO` & `s5-pytorch-0.2.0/s5_pytorch.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s5-pytorch
-Version: 0.1.9
+Version: 0.2.0
 Summary: S5 - Simplified State Space Layers for Sequence Modeling - Pytorch
 Home-page: https://github.com/i404788/s5-pytorch
 Author: Ferris Kwaijtaal
 Author-email: ferris+gh@devdroplets.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
@@ -15,16 +15,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # S5: Simplified State Space Layers for Sequence Modeling
 This is a ported version derived from <https://github.com/lindermanlab/S5> and <https://github.com/kavorite/S5>.
 It includes a bunch of functions ported from jax/lax/flax/whatever since they didn't exist yet. 
 
-Jax is required because it relies on the pytree structure but it's not used for any computation. 
-Pytorch 1.13 or later is required because it makes heavy use of `functorch.vamp` to substitute it's jax counterpart.
+~~Jax is required because it relies on the pytree structure but it's not used for any computation.~~
+Since version 0.2.0 jax is not required, it's using the pytorch native `torch.utils._pytree` (this may be incompatible for pytorch future versions).
+Pytorch 2 or later is required because it makes heavy use of `torch.vmap` and `torch.utils._pytree` to substitute it's jax counterpart.
 Python 3.10 or later is required due to usage of the `match` keyword
 
 \--- 
 
 Update:
 
 In my experiments it follows the results found in the [Hyena Hierarchy](https://arxiv.org/abs/2302.10866) (& H3) paper that the state spaces alone lack the recall capabilities required for LLM but seem work well for regular sequence feature extraction and linear complexity.
```

### Comparing `s5-pytorch-0.1.9/setup.py` & `s5-pytorch-0.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='s5-pytorch',
     packages=find_packages(exclude=[]),
-    version='0.1.9',
+    version='0.2.0',
     license='MIT',
     description='S5 - Simplified State Space Layers for Sequence Modeling - Pytorch',
     author='Ferris Kwaijtaal',
     author_email='ferris+gh@devdroplets.com',
     long_description_content_type='text/markdown',
     long_description=open('README.md', 'r').read(),
     url='https://github.com/i404788/s5-pytorch',
@@ -17,17 +17,19 @@
         'transformers',
         'attention mechanism',
         'audio generation'
     ],
     install_requires=[
         'einops>=0.6',
         'scipy',
-        'torch>=1.13',
-        'jax'
+        'torch>=2',
     ],
+    extra_requires={
+      "dev": ["jax"], 
+    },
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.10',
     ],
```

