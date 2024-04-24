# Comparing `tmp/einfunc-0.0.3.tar.gz` & `tmp/einfunc-0.0.4.tar.gz`

## Comparing `einfunc-0.0.3.tar` & `einfunc-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 einfunc-0.0.3/src/einfunc/__about__.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 einfunc-0.0.3/src/einfunc/__init__.py
--rw-r--r--   0        0        0     4509 2020-02-02 00:00:00.000000 einfunc-0.0.3/src/einfunc/einfunc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 einfunc-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 einfunc-0.0.3/tests/test_einfunc_function.py
--rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 einfunc-0.0.3/tests/test_einfunc_reduction.py
--rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 einfunc-0.0.3/tests/test_einfunc_shape.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 einfunc-0.0.3/.gitignore
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 einfunc-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 einfunc-0.0.3/README.md
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 einfunc-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     5283 2020-02-02 00:00:00.000000 einfunc-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 einfunc-0.0.4/src/einfunc/__about__.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 einfunc-0.0.4/src/einfunc/__init__.py
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 einfunc-0.0.4/src/einfunc/einfunc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 einfunc-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 einfunc-0.0.4/tests/test_einfunc_function.py
+-rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 einfunc-0.0.4/tests/test_einfunc_reduction.py
+-rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 einfunc-0.0.4/tests/test_einfunc_shape.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 einfunc-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 einfunc-0.0.4/LICENSE.txt
+-rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 einfunc-0.0.4/README.md
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 einfunc-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5167 2020-02-02 00:00:00.000000 einfunc-0.0.4/PKG-INFO
```

### Comparing `einfunc-0.0.3/src/einfunc/einfunc.py` & `einfunc-0.0.4/src/einfunc/einfunc.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,56 +2,44 @@
 from typing import Union
 from functools import lru_cache
 
 import torch
 from functorch.dim import dims
 
 
-@lru_cache(maxsize=126)
+#@lru_cache(maxsize=126)
 def _parse_pattern(pattern: str, pass_axis: bool):
     """Parses the pattern of the einstein notation for a tensor operation"""
-
     if "->" not in pattern:
         raise ValueError("einstein pattern must contain ->")
-
-    left_str, right_str = pattern.split("->")
+    input_str, output_str = pattern.split("->")
 
     # Determine total number of axis and tensor dim map
-    total_axis = set()
-    tensor_dim = []
-    for tensor_axis in left_str.split(","):
-        tensor_axis = tensor_axis.split()
-        total_axis = total_axis | set(tensor_axis)
-        tensor_dim.append(tensor_axis)
-
-    # Create axis and then map dim to axis
-    axis = dims(len(total_axis))
-
-    # Ensure axis is a list
+    inputs = [input.split() for input in input_str.split(",")]
+    dim = set.union(*map(set, inputs))
+    axis = dims(len(dim))
     if not isinstance(axis, tuple):
         axis = (axis,)
+    dim2axis = dict(zip(dim, axis))
 
-    dim2axis = dict(zip(total_axis, axis))
-
-    # Create tensor_axis
-    tensor_axis = list(map(lambda x: [dim2axis[dim] for dim in x], tensor_dim))
-
-    # Determine axis to collapse and final shape of tensor
-    right_axises = right_str.split()
-    collapse_axis = total_axis - set(right_axises)
-    collapse_axis = [dim2axis[x] for x in collapse_axis]
-    final_shape = [dim2axis[dim] for dim in right_axises]
+    tensor_axis = [[dim2axis[d] for d in exp] for exp in inputs]
+    output_axis = [output.split() for output in output_str.split(",")]
+    collapse_axis = [list(dim - set(output)) for output in output_axis]
+    collapse_axis = [[dim2axis[x] for x in exp] for exp in collapse_axis]
+    final_shape = [[dim2axis[x] for x in exp] for exp in output_axis]
 
     if pass_axis:
         return tensor_axis, collapse_axis, final_shape, axis
     return tensor_axis, collapse_axis, final_shape
 
 
 def _collapse_function(tensor: torch.Tensor, collapse: str, axis):
     """#Collapses the tensor along the given axis"""
+    if len(axis) == 0:
+        return tensor
     if collapse == "min":
         return tensor.amin(axis)
     if collapse == "max":
         return tensor.amax(axis)
     if collapse == "sum":
         return tensor.sum(axis)
     if collapse == "prod":
@@ -127,15 +115,24 @@
 
     # Pass to function (just pass, it should work lol)
     if pass_axis and axis is not None:
         final_tensor = function(*tensors, *axis)
     else:
         final_tensor = function(*tensors)
 
-    # apply the mode of collapse
-    if len(collapse_axis):
-        final_tensor = _collapse_function(final_tensor, collapse, collapse_axis)
+    if isinstance(final_tensor, tuple):
+        final_tensor = list(final_tensor)
+    else:
+        final_tensor = [final_tensor]
 
-    # Unbind dimension and return
-    if len(final_shape):
-        return final_tensor.order(*final_shape)
-    return final_tensor
+    # apply the mode of collapse
+    print(final_tensor, collapse_axis, final_shape)
+    ret = [
+        (
+            _collapse_function(tensor, collapse, caxis).order(*final)
+            if len(final)
+            else _collapse_function(tensor, collapse, caxis)
+        )
+        for tensor, caxis, final in zip(final_tensor, collapse_axis, final_shape)
+    ]
+    print(pattern, final_tensor, collapse_axis, final_shape)
+    return ret if len(ret) != 1 else ret[0]
```

### Comparing `einfunc-0.0.3/tests/test_einfunc_reduction.py` & `einfunc-0.0.4/tests/test_einfunc_reduction.py`

 * *Files identical despite different names*

### Comparing `einfunc-0.0.3/tests/test_einfunc_shape.py` & `einfunc-0.0.4/tests/test_einfunc_shape.py`

 * *Files identical despite different names*

### Comparing `einfunc-0.0.3/LICENSE.txt` & `einfunc-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `einfunc-0.0.3/README.md` & `einfunc-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 `einfunc` is a simple interface, which utilizes Pytorch's [torchdim](https://github.com/facebookresearch/torchdim). I highly recommend checking out torchdim as it is by far the best way to do readable tensor operations in pytorch. `einfunc` is just a convenient way of tapping into torchdim with a function similar to `einsum`.
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [API](#api)
 - [Why you shouldn't use einfunc](#why-not-use)
-- [Why you should use einfund](#why-yes-use)
+- [Why you should use einfunc](#why-yes-use)
 - [Additional Examples](#additional-examples)
 - [Planned Work](#planned-work)
 - [Acknowledgements](#acknowledgements)
 
 
 ## Installation
 
@@ -49,64 +49,62 @@
 ### Reducing
 Currently, einfunc supports 5 different types of reduction. 
 - Mean
 
 $$ \frac{1}{I} \sum_i^I x_{i,j} - y_{k, i} $$
 
 ```python
-result = einfunc(x, y, 'i j, k i -> j k', lambda a b : a - b, reduce='mean')
+result = einfunc(x, y, 'i j, k i -> j k', lambda a, b : a - b, reduce='mean')
 ```
   
 - Sum
   
 $$ \sum_i^I x_{i,j} - y_{k, i} $$
 
 ```python
-result = einfunc(x, y, 'i j, k i -> j k', lambda a b : a - b, reduce='sum')
+result = einfunc(x, y, 'i j, k i -> j k', lambda a, b : a - b, reduce='sum')
 ```
   
 - Prod
   
 $$ \prod_i^I x_{i,j} - y_{k, i} $$
 
 ```python
-result = einfunc(x, y, 'i j, k i -> j k', lambda a b : a - b, reduce='prod')
+result = einfunc(x, y, 'i j, k i -> j k', lambda a, b : a - b, reduce='prod')
 ```
 
 - Max
 
 $$ Max(x_{i,j} - y_{k, i}, \quad dim=i) $$
 
 ```python
-result = einfunc(x, y, 'i j, k i -> j k', lambda a b : a - b, reduce='max')
+result = einfunc(x, y, 'i j, k i -> j k', lambda a, b : a - b, reduce='max')
 ```
 - Min
 
 $$ Min(x_{i,j} - y_{k, i}, \quad dim=i) $$
 
 ```python
-result = einfunc(x, y, 'i j, k i -> j k', lambda a b : a - b, reduce='min')
+result = einfunc(x, y, 'i j, k i -> j k', lambda a, b : a - b, reduce='min')
 ```
 
 One thing to note is that if `reduce` is not passed then 'sum' is assumed by einfunc.
 
 ## Why you shouldn't use einfunc <a name="why-not-use"></a>
 
 Einfunc is just a convenient way of interfacing with PyTorch and Torchdim. This creates some overhead when operating on tensors, compared to vanilla operations and torchdim operations. This means that it will be much faster to use vanilla pytorch operations if doing a simple operation, or just use torchdim if trying to do something more complex.
 
 ## Why you should use einfunc <a name="why-yes-use"></a>
 
 It's convenient and slightly more readable than torchdim IMO. Understanding exactly what is happening in an operation can be hard, and einfunc makes it a lot simpler by boiling operations down to a single expression, while using einstein notation to indicate indexing.
 
 ## Additional Examples <a name="additional-examples"></a>
 
-Comming Soon :)
+Coming Soon :)
 
 ## Planned Work <a name="planned-work"></a>
 
 Currently, einfunc does support parenthesis and ellipses. I will be working on implementing this as soon as I can.
 
-Also, I have only tested einfunc on python >= 3.11 and I need to work on implementation to previous version of python.
-
 ## Acknowledgements
 
 Check out [einops](https://github.com/arogozhnikov/einops) and [torchdim](https://github.com/facebookresearch/torchdim).
```

### Comparing `einfunc-0.0.3/pyproject.toml` & `einfunc-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `einfunc-0.0.3/PKG-INFO` & `einfunc-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: einfunc
-Version: 0.0.3
+Version: 0.0.4
 Summary: Einstein notation function which allows for simple, readible, and highly flexible tensor operations.
 Project-URL: Documentation, https://github.com/Hprairie/einfunc#readme
 Project-URL: Issues, https://github.com/Hprairie/einfunc/issues
 Project-URL: Source, https://github.com/Hprairie/einfunc
 Author-email: Hayden Prairie <haydenprairie@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -32,15 +32,15 @@
 `einfunc` is a simple interface, which utilizes Pytorch's [torchdim](https://github.com/facebookresearch/torchdim). I highly recommend checking out torchdim as it is by far the best way to do readable tensor operations in pytorch. `einfunc` is just a convenient way of tapping into torchdim with a function similar to `einsum`.
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [API](#api)
 - [Why you shouldn't use einfunc](#why-not-use)
-- [Why you should use einfund](#why-yes-use)
+- [Why you should use einfunc](#why-yes-use)
 - [Additional Examples](#additional-examples)
 - [Planned Work](#planned-work)
 - [Acknowledgements](#acknowledgements)
 
 
 ## Installation
 
@@ -71,64 +71,62 @@
 ### Reducing
 Currently, einfunc supports 5 different types of reduction. 
 - Mean
 
 $$ \frac{1}{I} \sum_i^I x_{i,j} - y_{k, i} $$
 
 ```python
-result = einfunc(x, y, 'i j, k i -> j k', lambda a b : a - b, reduce='mean')
+result = einfunc(x, y, 'i j, k i -> j k', lambda a, b : a - b, reduce='mean')
 ```
   
 - Sum
   
 $$ \sum_i^I x_{i,j} - y_{k, i} $$
 
 ```python
-result = einfunc(x, y, 'i j, k i -> j k', lambda a b : a - b, reduce='sum')
+result = einfunc(x, y, 'i j, k i -> j k', lambda a, b : a - b, reduce='sum')
 ```
   
 - Prod
   
 $$ \prod_i^I x_{i,j} - y_{k, i} $$
 
 ```python
-result = einfunc(x, y, 'i j, k i -> j k', lambda a b : a - b, reduce='prod')
+result = einfunc(x, y, 'i j, k i -> j k', lambda a, b : a - b, reduce='prod')
 ```
 
 - Max
 
 $$ Max(x_{i,j} - y_{k, i}, \quad dim=i) $$
 
 ```python
-result = einfunc(x, y, 'i j, k i -> j k', lambda a b : a - b, reduce='max')
+result = einfunc(x, y, 'i j, k i -> j k', lambda a, b : a - b, reduce='max')
 ```
 - Min
 
 $$ Min(x_{i,j} - y_{k, i}, \quad dim=i) $$
 
 ```python
-result = einfunc(x, y, 'i j, k i -> j k', lambda a b : a - b, reduce='min')
+result = einfunc(x, y, 'i j, k i -> j k', lambda a, b : a - b, reduce='min')
 ```
 
 One thing to note is that if `reduce` is not passed then 'sum' is assumed by einfunc.
 
 ## Why you shouldn't use einfunc <a name="why-not-use"></a>
 
 Einfunc is just a convenient way of interfacing with PyTorch and Torchdim. This creates some overhead when operating on tensors, compared to vanilla operations and torchdim operations. This means that it will be much faster to use vanilla pytorch operations if doing a simple operation, or just use torchdim if trying to do something more complex.
 
 ## Why you should use einfunc <a name="why-yes-use"></a>
 
 It's convenient and slightly more readable than torchdim IMO. Understanding exactly what is happening in an operation can be hard, and einfunc makes it a lot simpler by boiling operations down to a single expression, while using einstein notation to indicate indexing.
 
 ## Additional Examples <a name="additional-examples"></a>
 
-Comming Soon :)
+Coming Soon :)
 
 ## Planned Work <a name="planned-work"></a>
 
 Currently, einfunc does support parenthesis and ellipses. I will be working on implementing this as soon as I can.
 
-Also, I have only tested einfunc on python >= 3.11 and I need to work on implementation to previous version of python.
-
 ## Acknowledgements
 
 Check out [einops](https://github.com/arogozhnikov/einops) and [torchdim](https://github.com/facebookresearch/torchdim).
```

