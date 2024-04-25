# Comparing `tmp/folx-0.2.5.tar.gz` & `tmp/folx-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "folx-0.2.5.tar", max compression
+gzip compressed data, was "folx-0.2.6.tar", max compression
```

## Comparing `folx-0.2.5.tar` & `folx-0.2.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1141 2023-12-12 15:39:39.316411 folx-0.2.5/LICENSE
--rw-r--r--   0        0        0     9594 2023-12-14 10:04:12.586401 folx-0.2.5/README.md
--rw-r--r--   0        0        0      743 2024-02-08 19:35:20.067248 folx-0.2.5/folx/__init__.py
--rw-r--r--   0        0        0     2812 2024-02-13 22:40:14.551068 folx-0.2.5/folx/ad.py
--rw-r--r--   0        0        0    13966 2024-02-21 19:51:50.908838 folx-0.2.5/folx/api.py
--rw-r--r--   0        0        0     3304 2024-02-20 21:38:29.124052 folx-0.2.5/folx/custom_hessian.py
--rw-r--r--   0        0        0    14242 2024-02-14 16:24:35.308557 folx-0.2.5/folx/hessian.py
--rw-r--r--   0        0        0    11805 2024-02-21 19:51:50.912838 folx-0.2.5/folx/interpreter.py
--rw-r--r--   0        0        0    17570 2024-02-21 14:55:47.827412 folx-0.2.5/folx/jvp.py
--rw-r--r--   0        0        0     1858 2024-02-01 09:34:38.851198 folx-0.2.5/folx/operators.py
--rw-r--r--   0        0        0     2226 2024-02-01 09:34:38.851198 folx-0.2.5/folx/tree_utils.py
--rw-r--r--   0        0        0    18789 2024-02-21 14:55:47.827412 folx-0.2.5/folx/utils.py
--rw-r--r--   0        0        0     2845 2024-02-01 09:34:38.855198 folx-0.2.5/folx/vmap.py
--rw-r--r--   0        0        0    15537 2024-02-20 21:38:29.124052 folx-0.2.5/folx/wrapped_functions.py
--rw-r--r--   0        0        0     5241 2024-02-14 16:24:35.312557 folx-0.2.5/folx/wrapper.py
--rw-r--r--   0        0        0     1388 2024-02-21 19:51:53.792814 folx-0.2.5/pyproject.toml
--rw-r--r--   0        0        0    10844 1970-01-01 00:00:00.000000 folx-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1141 2023-12-12 15:39:39.316411 folx-0.2.6/LICENSE
+-rw-r--r--   0        0        0    11302 2024-03-23 09:07:16.106122 folx-0.2.6/README.md
+-rw-r--r--   0        0        0      743 2024-02-08 19:35:20.067248 folx-0.2.6/folx/__init__.py
+-rw-r--r--   0        0        0     2812 2024-02-13 22:40:14.551068 folx-0.2.6/folx/ad.py
+-rw-r--r--   0        0        0    13900 2024-03-15 13:17:04.011521 folx-0.2.6/folx/api.py
+-rw-r--r--   0        0        0     3304 2024-04-25 12:26:02.179017 folx-0.2.6/folx/custom_hessian.py
+-rw-r--r--   0        0        0    14208 2024-03-15 13:17:04.011521 folx-0.2.6/folx/hessian.py
+-rw-r--r--   0        0        0    12236 2024-04-25 12:26:12.486944 folx-0.2.6/folx/interpreter.py
+-rw-r--r--   0        0        0    17552 2024-04-25 12:25:16.227342 folx-0.2.6/folx/jvp.py
+-rw-r--r--   0        0        0     1943 2024-03-23 09:06:28.458443 folx-0.2.6/folx/operators.py
+-rw-r--r--   0        0        0     2226 2024-02-01 09:34:38.851198 folx-0.2.6/folx/tree_utils.py
+-rw-r--r--   0        0        0    18755 2024-03-15 13:17:04.019521 folx-0.2.6/folx/utils.py
+-rw-r--r--   0        0        0     2845 2024-02-01 09:34:38.855198 folx-0.2.6/folx/vmap.py
+-rw-r--r--   0        0        0    15558 2024-04-25 12:26:12.486944 folx-0.2.6/folx/wrapped_functions.py
+-rw-r--r--   0        0        0     5241 2024-02-14 16:24:35.312557 folx-0.2.6/folx/wrapper.py
+-rw-r--r--   0        0        0     1388 2024-04-25 12:36:13.126698 folx-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0    12552 1970-01-01 00:00:00.000000 folx-0.2.6/PKG-INFO
```

### Comparing `folx-0.2.5/LICENSE` & `folx-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `folx-0.2.5/README.md` & `folx-0.2.6/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,57 +1,96 @@
 # `folx` - Forward Laplacian for JAX
 
 This submodule implements the forward laplacian from https://arxiv.org/abs/2307.08214. It is implemented as a [custom interpreter for Jaxprs](https://jax.readthedocs.io/en/latest/notebooks/Writing_custom_interpreters_in_Jax.html).
 
 ## Install
 
-Either clone repo and install locally via 
+Either clone repo and install locally via
 ```bash
 poetry install
 ```
 or
 ```bash
 pip install .
 ```
 or install via `pip` package manager via
 ```bash
 pip install folx
 ```
 
 ## Example
+### Dense example
 For simple usage, one can decorate any function with `forward_laplacian`.
 ```python
 import numpy as np
 from folx import forward_laplacian
 
 def f(x):
     return (x**2).sum()
 
 fwd_f = forward_laplacian(f)
 result = fwd_f(np.arange(3, dtype=float))
 result.x # f(x) 3
 result.jacobian.dense_array # J_f(x) [0, 2, 4]
 result.laplacian # tr(H_f(x)) 6
 ```
+### Sparsity example
+A big feature of `folx` is to automatically work with sparse jacobians to accelerate computations. Note that the results are still **exact**. To enable this feature simply supply a maximum sparsity threshold. Compile times may increase significantly as tracing the sparsity patterns of the jacobians is a lengthy process. Here is an example with an MLP operating indepdently on individual node features.
+```python
+import folx
+import jax
+import jax.numpy as jnp
+import flax.linen as nn
+
+class MLP(nn.Module):
+    @nn.compact
+    def __call__(self, x):
+        for _ in range(10):
+            x = nn.Dense(100)(x)
+            x = nn.silu(x)
+        return nn.Dense(1)(x).sum()
+
+mlp = MLP()
+x = jnp.ones((20, 100, 4))
+params = mlp.init(jax.random.PRNGKey(0), x)
+def fwd(x):
+    return mlp.apply(params, x)
+
+# Traditional loop implementation
+lapl = jax.jit(jax.vmap(folx.LoopLaplacianOperator()(fwd)))
+%time jax.block_until_ready(lapl(x)) # Wall time: 1.42 s
+%timeit jax.block_until_ready(lapl(x)) # 224 ms ± 54 µs per loop (mean ± std. dev. of 7 runs, 1 loop each)
+
+# Forward laplacian without sparsity
+lapl = jax.jit(jax.vmap(folx.ForwardLaplacianOperator(0)(fwd)))
+%time jax.block_until_ready(lapl(x)) # Wall time: 2.66 s
+%timeit jax.block_until_ready(lapl(x)) # 48.7 ms ± 42.1 µs per loop (mean ± std. dev. of 7 runs, 10 loops each)
+
+# Forward laplacian with sparsity
+lapl = jax.jit(jax.vmap(folx.ForwardLaplacianOperator(4)(fwd)))
+%time jax.block_until_ready(lapl(x)) # Wall time: 5.05 s
+%timeit jax.block_until_ready(lapl(x)) # 2.59 ms ± 15.3 µs per loop (mean ± std. dev. of 7 runs, 100 loops each)
+```
+For electronic wave function like FermiNet or PsiFormer, `sparsity_threshold=6` is a recommended value. But, tuning this hyperparameter may accelerate computations.
 
 ## Introduction
-To avoid custom wrappers for all of JAX's commands, the forward laplacian is implemented as custom interpreter for Jaxpr. 
+To avoid custom wrappers for all of JAX's commands, the forward laplacian is implemented as custom interpreter for Jaxpr.
 This means if you have a function
 ```python
 class Fn(Protocol):
     def __call__(self, *args: PyTree[Array]) -> PyTree[Array]:
         ...
 ```
 the resulting function will have the signature:
 ```python
 class LaplacianFn(Protocol):
     def __call__(self, *args: PyTree[Array]) -> PyTree[FwdLaplArray]:
         ...
 ```
-where `FwdLaplArray` is a triplet of 
+where `FwdLaplArray` is a triplet of
 ```python
 FwdLaplArray.x # jax.Array f(x) f(x).shape
 FwdLaplArray.jacobian # FwdJacobian J_f(x)
 FwdLaplArray.laplacian # jax.Array tr(H_f(x)) f(x).shape
 ```
 The jacobian is implemented by a custom class as the forward laplacian supports automatic sparsity. To get the full jacobian:
 ```python
@@ -73,30 +112,30 @@
 ## Implementation
 
 When you call the function returned by `forward_laplacian(fn)`, we first use `jax.make_jaxpr` to obtain the jaxpr for `fn`.
 But instead of using the [standard evaluation pipeline](https://github.com/google/jax/blob/776baba0a3fca15a909cb7d108eea830cbe3fc1d/jax/_src/core.py#L436), we use a custom interpreter that replaces all operations to propate `FwdLaplArray` forward instead of regular `jax.Array`.
 
 ### Package structure
 The general structure of the package is
-* `interpreter.py` contains the evaluation of jaxpr and exported function decorator. 
+* `interpreter.py` contains the evaluation of jaxpr and exported function decorator.
 * `wrapper.py` contains subfunction decorator that maps a function that takes `jax.Array`s to a function that accepts `FwdLaplArray`s instead.
 * `wrapped_functions.py` contains a registry of predefined functions as well as utility functions to add new functions to the registry.
 * `jvp.py` contains logic for jacobian vector products.
 * `hessian.py` contains logic for tr(JHJ^T).
 * `custom_hessian.py` contains special treatment logic for tr(JHJ^T).
 * `api.py` contains general interfaces shared in the package.
 * `operators.py` contains a forward laplacian operator as well as alternatives.
 * `utils.py` contains several small utility functions.
-* `tree_utils.py` contains several utility functions for PyTrees. 
+* `tree_utils.py` contains several utility functions for PyTrees.
 * `vmap.py` contains a batched vmap implementation to reduce memory usage by going through a batch sequentially in chunks.
 
 
 ### Function Annotations
 There is a default interpreter that will simply apply the rules outlined above but if additional information about a function is available, e.g., that it applies elementwise like `jnp.tanh`, we can do better.
-These additional annotations are available in `wrapped_functions.py`'s `_LAPLACE_FN_REGISTRY`. 
+These additional annotations are available in `wrapped_functions.py`'s `_LAPLACE_FN_REGISTRY`.
 Specifically, to augment a function `fn` to accept `FwdLaplArray` instead of regular `jax.Array`, we wrap it with `wrap_forward_laplacian` from `fwd_laplacian.py`:
 ```python
 wrap_forward_laplacian(jnp.tanh, in_axes=())
 ```
 In this case, we annotate the function to be applied elementwise, i.e., `()` indicates that none of the axes are relevant for the function.
 
 If we know nothing about which axes might be essential, one must pass `None` (the default value) to mark all axes as imporatnt, e.g.,
@@ -138,38 +177,41 @@
 ```
 
 
 ### Sparsity
 Sparsity is detected at compile time, this has the advantage of avoiding expensive index computations at runtime and enables efficient reductions. However, it completely prohibits dynamic indexing, i.e., if indices are data-dependent we will simply default to full jacobians.
 
 As we know a lot about the sparsity structure apriori, e.g., that we are only sparse in one dimension, we use a custom sparsity operations that are more efficient than relying on JAX's default `BCOO` (further, at the time of writing, the support for `jax.experimental.sparse` is quite bad).
-So, the sparsity data format is implemented in `FwdJacobian` in `api.py`. Instead of storing a dense array `(m, n)` for a function `f:R^n -> R^m`, we store only the non-zero data in a `(m,d)` array where `d<n` is the maximum number of non-zero inputs any output depends on. 
+So, the sparsity data format is implemented in `FwdJacobian` in `api.py`. Instead of storing a dense array `(m, n)` for a function `f:R^n -> R^m`, we store only the non-zero data in a `(m,d)` array where `d<n` is the maximum number of non-zero inputs any output depends on.
 To be able to recreate the larger `(m,n)` array from the `(m,d)` array, we additional keep track of the indices in the last dimension in a mask `(m,d)` dimensional array of integers `0<mask_ij<n`.
 
 Masks are treated as compile time static and will be traced automatically. If the tracing is not possible, e.g., due to data dependent indexing, we will fall back to a dense implementation. These propagation rules are implemented in `jvp.py`.
 
-##### Omnistaging
-If arrays do not depend on the initial input, they are typically still traced to better optimize the final program. This is called [omnistaging](https://github.com/google/jax/pull/3370). While this generally is beneficial, it does not allow us to perform indexing as tracer hide the actual data. 
-So, if we use sparsity we want to compute all arrays that do not explicitly depend on the input such that we could use them for index operations.
-While this is not documented, it can be accomplished by overwriting the global trace via:
+
+### Memory efficiency
+The forward laplacian uses more GPU memory due to the full materialization of the Jacobian matrix.
+To compensate for this, it is recommended to loop over the batch size (while other implementations typically loop over the Hessian).
+We provide an easy to use utility for this via `folx.batched_vmap` which functions like `jax.vmap` but chunks the input into batches and operates on these sequentially.
 ```python
-from jax import core
+from folx import batched_vmap
+
+def f(x):
+    return x**2
 
-with core.new_main(core.EvalTrace, dynamic=True):
-    ...
+batched_f = batched_vmap(f, max_batch_size=64)
 ```
 
 ## Citation
 If you find work helpful, please consider citing it as
 ```
-@software{folx2023gao,
-  author = {Nichoals Gao and Jonas Köhler and Adam Foster},
+@software{gao2023folx,
+  author = {Nicholas Gao and Jonas Köhler and Adam Foster},
   title = {folx - Forward Laplacian for JAX},
   url = {http://github.com/microsoft/folx},
-  version = {0.2.0},
+  version = {0.2.5},
   year = {2023},
 }
 ```
 as well as the original forward laplacian:
 ```
 @article{li2023forward,
   title={Forward Laplacian: A New Computational Framework for Neural Network-based Variational Monte Carlo},
@@ -191,12 +233,12 @@
 
 This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
 For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
 contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
 
 ## Trademarks
 
-This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft 
-trademarks or logos is subject to and must follow 
+This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft
+trademarks or logos is subject to and must follow
 [Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general).
 Use of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship.
 Any use of third-party trademarks or logos are subject to those third-party's policies.
```

### Comparing `folx-0.2.5/folx/__init__.py` & `folx-0.2.6/folx/__init__.py`

 * *Files identical despite different names*

### Comparing `folx-0.2.5/folx/ad.py` & `folx-0.2.6/folx/ad.py`

 * *Files identical despite different names*

### Comparing `folx-0.2.5/folx/api.py` & `folx-0.2.6/folx/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from enum import IntFlag
 from typing import Any, Callable, NamedTuple, Protocol, TypeAlias, TypeVar
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 import numpy.typing as npt
-from jax import core
 from jaxtyping import Array, PyTree
 
 T = TypeVar('T', bound=PyTree[Array])
 R = TypeVar('R', bound=PyTree[Array])
 
 ExtraArgs = tuple[Array, ...]
 Arrays = tuple[Array, ...]
@@ -127,15 +126,15 @@
         def get_indices(mask, out_mask):
             matching = mask[..., None] == out_mask
             indices = jnp.argmax(matching, axis=-1)
             indices = jnp.where(jnp.any(matching, axis=-1), indices, -1)
             return indices
 
         if isinstance(outputs, np.ndarray):
-            with core.new_main(core.EvalTrace, dynamic=True):
+            with jax.ensure_compile_time_eval():
                 result = np.asarray(get_indices(flat_mask, flat_outputs), dtype=int).T
         else:
             result = get_indices(flat_mask, flat_outputs).T
         return result.reshape(mask.shape)
 
     @property
     def data_shape(self):
@@ -386,50 +385,46 @@
 Axes = Any
 
 ArrayOrArrays: TypeAlias = Array | tuple[Array, ...] | list[Array]
 ForwardFn = Callable[..., ArrayOrArrays]
 
 
 class MergeFn(Protocol):
-    def __call__(self, args: Arrays, extra: ExtraArgs) -> Arrays:
-        ...
+    def __call__(self, args: Arrays, extra: ExtraArgs) -> Arrays: ...
 
 
 class ForwardLaplacianFns(NamedTuple):
     forward: ForwardFn
     jvp: Callable[
         [FwdLaplArgs, dict[str, Any]], tuple[ArrayOrArrays, FwdJacobian, ArrayOrArrays]
     ]
     jac_hessian_jac_trace: Callable[[FwdLaplArgs, int], ArrayOrArrays]
 
 
 class JvpFn(Protocol):
-    def __call__(self, primals: Arrays, tangents: Arrays) -> tuple[Array, Array]:
-        ...
+    def __call__(self, primals: Arrays, tangents: Arrays) -> tuple[Array, Array]: ...
 
 
 class CustomTraceJacHessianJac(Protocol):
     def __call__(
         self,
         args: FwdLaplArgs,
         extra_args: ExtraArgs,
         merge: MergeFn,
         materialize_idx: Array,
-    ) -> PyTree[Array]:
-        ...
+    ) -> PyTree[Array]: ...
 
 
 class ForwardLaplacian(Protocol):
     def __call__(
         self,
         args: tuple[ArrayOrFwdLaplArray],
         kwargs: dict[str, Any],
         sparsity_threshold: int,
-    ) -> PyTree[ArrayOrFwdLaplArray]:
-        ...
+    ) -> PyTree[ArrayOrFwdLaplArray]: ...
 
 
 class FunctionFlags(IntFlag):
     GENERAL = 0
     LINEAR_IN_FIRST = 1
     LINEAR_IN_ONE = 2 | LINEAR_IN_FIRST
     LINEAR = 4 | LINEAR_IN_ONE
```

### Comparing `folx-0.2.5/folx/custom_hessian.py` & `folx-0.2.6/folx/custom_hessian.py`

 * *Files identical despite different names*

### Comparing `folx-0.2.5/folx/hessian.py` & `folx-0.2.6/folx/hessian.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 import jax
 import jax.flatten_util as jfu
 import jax.numpy as jnp
 import jax.tree_util as jtu
 import jaxlib.xla_extension
 import numpy as np
-from jax import core
 
 from .api import (
     JAC_DIM,
     Array,
     Axes,
     CustomTraceJacHessianJac,
     ExtraArgs,
@@ -202,15 +201,15 @@
 def find_materialization_idx(
     lapl_args: FwdLaplArgs, in_axes, flags: FunctionFlags, threshold: int
 ):
     if not lapl_args.any_jacobian_weak:
         return None
     # TODO: Rewrite this!! This is quity messy and inefficient.
     # it assumes that we're only interested in the last dimension.
-    with core.new_main(core.EvalTrace, dynamic=True):
+    with jax.ensure_compile_time_eval():
         vmap_seq, (inp,) = vmap_sequences_and_squeeze(
             ([j.mask for j in lapl_args.jacobian],),
             (
                 [
                     j
                     for j in add_vmap_jacobian_dim(
                         lapl_args, FwdLaplArgs(in_axes)
```

### Comparing `folx-0.2.5/folx/interpreter.py` & `folx-0.2.6/folx/interpreter.py`

 * *Files 6% similar despite different names*

```diff
@@ -167,43 +167,53 @@
             return fn(
                 (*subfuns, *invals), params, sparsity_threshold=sparsity_threshold
             )
 
     for eqn in jaxpr.eqns:
         invals = env.read_many(eqn.invars)
         # Eval expression
-        if all(not isinstance(x, FwdLaplArray) for x in invals):
-            subfuns, bind_params = eqn.primitive.get_bind_params(eqn.params)
-            # If non of the inputs were dependent on an FwdLaplArray,
-            # we can just use the regular primitive. This will avoid
-            # omnistaging. While this could cost us some memory and speed,
-            # it gives us access to more variables during tracing.
-            # https://github.com/google/jax/pull/3370
-            if all(not isinstance(x, core.Tracer) for x in invals) and enable_sparsity:
-                try:
-                    with core.new_main(core.EvalTrace, dynamic=True):
+        try:
+            if all(not isinstance(x, FwdLaplArray) for x in invals):
+                subfuns, bind_params = eqn.primitive.get_bind_params(eqn.params)
+                # If non of the inputs were dependent on an FwdLaplArray,
+                # we can just use the regular primitive. This will avoid
+                # omnistaging. While this could cost us some memory and speed,
+                # it gives us access to more variables during tracing.
+                # https://github.com/google/jax/pull/3370
+                if (
+                    all(not isinstance(x, core.Tracer) for x in invals)
+                    and enable_sparsity
+                ):
+                    try:
+                        with jax.ensure_compile_time_eval():
+                            outvals = eqn.primitive.bind(
+                                *subfuns, *invals, **bind_params
+                            )
+                    except Exception as e:
+                        with LoggingPrefix(f'({summarize(eqn.source_info)})'):
+                            logging.warning(
+                                f'Could not perform operation {eqn.primitive.name} in eager execution despite it only depending on non-input dependent values. '
+                                'We switch to tracing rather than eager execution. This may impact sparsity propagation.\n'
+                                f'{e}'
+                            )
                         outvals = eqn.primitive.bind(*subfuns, *invals, **bind_params)
-                except Exception as e:
-                    with LoggingPrefix(f'({summarize(eqn.source_info)})'):
-                        logging.warning(
-                            f'Could not perform operation {eqn.primitive.name} in eager execution despite it only depending on non-input dependent values. '
-                            'We switch to tracing rather than eager execution. This may impact sparsity propagation.\n'
-                            f'{e}'
-                        )
+                else:
                     outvals = eqn.primitive.bind(*subfuns, *invals, **bind_params)
+            elif eqn.primitive.name == 'scan':
+                outvals = eval_scan(eqn, invals)
+            elif eqn.primitive.name == 'pjit':
+                outvals = eval_pjit(eqn, invals)
+            elif eqn.primitive.name == 'custom_jvp_call':
+                outvals = eval_custom_jvp(eqn, invals)
             else:
-                outvals = eqn.primitive.bind(*subfuns, *invals, **bind_params)
-        elif eqn.primitive.name == 'scan':
-            outvals = eval_scan(eqn, invals)
-        elif eqn.primitive.name == 'pjit':
-            outvals = eval_pjit(eqn, invals)
-        elif eqn.primitive.name == 'custom_jvp_call':
-            outvals = eval_custom_jvp(eqn, invals)
-        else:
-            outvals = eval_laplacian(eqn, invals)
+                outvals = eval_laplacian(eqn, invals)
+        except Exception as e:
+            with LoggingPrefix(f'({summarize(eqn.source_info)})'):
+                logging.error(f'Error in operation {eqn.primitive.name}.')
+            raise e
 
         # unify output
         if not eqn.primitive.multiple_results:
             outvals = [outvals]
         # save output
         env.write_many(eqn.outvars, outvals)  # type: ignore
     return env.read_many(jaxpr.outvars)
```

### Comparing `folx-0.2.5/folx/jvp.py` & `folx-0.2.6/folx/jvp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import functools
 import logging
 from typing import TypeVar
 
 import jax
-import jax.core as core
 import jax.numpy as jnp
 import jax.tree_util as jtu
 import numpy as np
 
 from .api import (
     JAC_DIM,
     Array,
@@ -188,15 +187,15 @@
     # Compute output mask
     try:
         # We must disable any jit tracer and evaluate the index operation
         # explictly here. This allows us to perform the index operation on our mask.
         # An index operation is expected to be static. If it is not, we will default to
         # materializing everything.
         # https://github.com/google/jax/pull/3370
-        with core.new_main(core.EvalTrace, dynamic=True):
+        with jax.ensure_compile_time_eval():
             extra_filled = jtu.tree_map(
                 lambda x: jnp.full(x.shape, -1, dtype=jnp.int32), extra_args
             )
 
             def _merged_fwd(*args):
                 # For index operations some operands may be static, i.e., they are not
                 # part of the output. We need to make sure that we do not fill these.
@@ -283,15 +282,15 @@
         logging.info(
             'Scatter: dimension numbers not supported. At the moment only segment sums are supported.'
         )
         return dense_jvp(fwd, laplace_args, flags=flags, in_axes=in_axes)
 
     updates: FwdLaplArray = updates
     n = updates.jacobian.max_n + 1
-    with core.new_main(core.EvalTrace, dynamic=True):
+    with jax.ensure_compile_time_eval():
         one_hot_mask = jax.nn.one_hot(
             updates.jacobian.x0_idx, n, axis=-1, dtype=jnp.int32
         ).sum(0)
         out_mask = np.array(jax.ops.segment_sum(one_hot_mask, scatter_indices[:, 0]))
         max_out = np.sum(out_mask.astype(bool), axis=-1).max()
         out_mask = np.where(
             out_mask > 0, out_mask * jnp.arange(n), np.iinfo(np.int32).max
@@ -482,13 +481,14 @@
         return y, grad, lapl  # type: ignore
 
     def jvp(args: FwdLaplArgs, kwargs) -> tuple[Array, FwdJacobian, Array]:
         if (
             (not args.any_jacobian_weak)
             or (FunctionFlags.INDEXING in flags)
             or (in_axes == ())
+            or (len(args) == 1)
         ):
             return parallel_jvp(args, kwargs)
         else:
             return one_by_one_jvp(args, kwargs)
 
     return jvp
```

### Comparing `folx-0.2.5/folx/operators.py` & `folx-0.2.6/folx/operators.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,21 +14,19 @@
     'ForwardLaplacianOperator',
     'LoopLaplacianOperator',
     'ParallelLaplacianOperator',
 ]
 
 
 class Laplacian(Protocol):
-    def __call__(self, x: Array) -> tuple[Array, Array]:
-        ...
+    def __call__(self, x: Array) -> tuple[Array, Array]: ...
 
 
 class LaplacianOperator(Protocol):
-    def __call__(self, f: Callable[[Array], Array]) -> Laplacian:
-        ...
+    def __call__(self, f: Callable[[Array], Array]) -> Laplacian: ...
 
 
 @dataclass(frozen=True)
 class ForwardLaplacianOperator(LaplacianOperator):
     sparsity_threshold: float | int
 
     def __call__(self, f):
@@ -42,18 +40,23 @@
 
 
 class LoopLaplacianOperator(LaplacianOperator):
     @staticmethod
     def __call__(f):
         @jax.jit
         def laplacian(x: jax.Array):
+            x_shape = x.shape
             x = x.reshape(-1)
             n = x.shape[0]
             eye = jnp.eye(n)
-            grad_f = jax.grad(f)
+
+            def f_(x):
+                return f(x.reshape(x_shape))
+
+            grad_f = jax.grad(f_)
             jacobian, dgrad_f = jax.linearize(grad_f, x)
 
             _, laplacian = jax.lax.scan(
                 lambda i, _: (i + 1, dgrad_f(eye[i])[i]), 0, None, length=n
             )
             return laplacian, jacobian
```

### Comparing `folx-0.2.5/folx/tree_utils.py` & `folx-0.2.6/folx/tree_utils.py`

 * *Files identical despite different names*

### Comparing `folx-0.2.5/folx/utils.py` & `folx-0.2.6/folx/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from typing import Sequence, Type, TypeVar
 
 import jax
 import jax.flatten_util as jfu
 import jax.numpy as jnp
 import jax.tree_util as jtu
 import numpy as np
-from jax import core
 
 from .api import (
     JAC_DIM,
     Array,
     IS_LEAF,
     ArrayOrFwdLaplArray,
     Arrays,
@@ -559,15 +558,15 @@
         del target_shape[JAC_DIM]
         target_shape = tuple(target_shape)
 
         @functools.partial(jax.vmap, in_axes=JAC_DIM, out_axes=JAC_DIM)
         def brdcast(x):
             return jnp.broadcast_to(x, target_shape)
 
-        with core.new_main(core.EvalTrace, dynamic=True):
+        with jax.ensure_compile_time_eval():
             return np.asarray(brdcast(m), dtype=m.dtype)
 
     return jtu.tree_map(broadcast, mask, jacobian)
 
 
 class LoggingPrefix(logging.Formatter):
     prefix: str
```

### Comparing `folx-0.2.5/folx/vmap.py` & `folx-0.2.6/folx/vmap.py`

 * *Files identical despite different names*

### Comparing `folx-0.2.5/folx/wrapped_functions.py` & `folx-0.2.6/folx/wrapped_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
     def custom_jvp(jacobian, tangent, sign):
         jac_dot_tangent = jnp.vdot(jacobian.T.conj(), tangent)
         if jac_dot_tangent.dtype in (jnp.complex64, jnp.complex128):
             # this is not the real jvp but a cached value to ease the Tr(JHJ^T) computation
             sign_jvp = jac_dot_tangent
             log_det_jvp = jac_dot_tangent.real
         else:
-            sign_jvp = jnp.zeros(())
+            sign_jvp = jnp.zeros((), dtype=jac_dot_tangent.dtype)
             log_det_jvp = jac_dot_tangent
         return (sign_jvp, log_det_jvp)
 
     y_tangent = jax.vmap(custom_jvp)(jacobians, tangents, sign)
 
     y, y_tangent = jtu.tree_map(lambda x: x.reshape(*batch_shape), (y, y_tangent))
     return y, y_tangent
@@ -379,23 +379,21 @@
     """
     return primitive_or_name in _LAPLACE_FN_REGISTRY
 
 
 @overload
 def get_laplacian(
     primitive_or_name: Primitive, wrap_if_missing: Literal[True]
-) -> ForwardLaplacian:
-    ...
+) -> ForwardLaplacian: ...
 
 
 @overload
 def get_laplacian(
     primitive_or_name: Primitive | str, wrap_if_missing: Literal[False] = False
-) -> ForwardLaplacian | None:
-    ...
+) -> ForwardLaplacian | None: ...
 
 
 def get_laplacian(
     primitive_or_name: Primitive | str, wrap_if_missing: bool = False
 ) -> ForwardLaplacian | None:
     """
     Get the forward laplacian of a primitive or a function name.
```

### Comparing `folx-0.2.5/folx/wrapper.py` & `folx-0.2.6/folx/wrapper.py`

 * *Files identical despite different names*

### Comparing `folx-0.2.5/pyproject.toml` & `folx-0.2.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'folx'
-version = '0.2.5'
+version = '0.2.6'
 description = 'Forward Laplacian for JAX'
 authors = [
     "Nicholas Gao <n.gao@tum.de>",
     "Jonas Koehler <jonas.koehler@microsoft.com>",
     "Adam Foster <adam.e.foster@microsoft.com>"
 ]
 maintainers = [
```

### Comparing `folx-0.2.5/PKG-INFO` & `folx-0.2.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: folx
-Version: 0.2.5
+Version: 0.2.6
 Summary: Forward Laplacian for JAX
 Home-page: https://github.com/microsoft/folx
 License: MIT
 Keywords: jax,laplacian,numeric
 Author: Nicholas Gao
 Author-email: n.gao@tum.de
 Maintainer: Nicholas Gao
@@ -35,58 +35,97 @@
 
 # `folx` - Forward Laplacian for JAX
 
 This submodule implements the forward laplacian from https://arxiv.org/abs/2307.08214. It is implemented as a [custom interpreter for Jaxprs](https://jax.readthedocs.io/en/latest/notebooks/Writing_custom_interpreters_in_Jax.html).
 
 ## Install
 
-Either clone repo and install locally via 
+Either clone repo and install locally via
 ```bash
 poetry install
 ```
 or
 ```bash
 pip install .
 ```
 or install via `pip` package manager via
 ```bash
 pip install folx
 ```
 
 ## Example
+### Dense example
 For simple usage, one can decorate any function with `forward_laplacian`.
 ```python
 import numpy as np
 from folx import forward_laplacian
 
 def f(x):
     return (x**2).sum()
 
 fwd_f = forward_laplacian(f)
 result = fwd_f(np.arange(3, dtype=float))
 result.x # f(x) 3
 result.jacobian.dense_array # J_f(x) [0, 2, 4]
 result.laplacian # tr(H_f(x)) 6
 ```
+### Sparsity example
+A big feature of `folx` is to automatically work with sparse jacobians to accelerate computations. Note that the results are still **exact**. To enable this feature simply supply a maximum sparsity threshold. Compile times may increase significantly as tracing the sparsity patterns of the jacobians is a lengthy process. Here is an example with an MLP operating indepdently on individual node features.
+```python
+import folx
+import jax
+import jax.numpy as jnp
+import flax.linen as nn
+
+class MLP(nn.Module):
+    @nn.compact
+    def __call__(self, x):
+        for _ in range(10):
+            x = nn.Dense(100)(x)
+            x = nn.silu(x)
+        return nn.Dense(1)(x).sum()
+
+mlp = MLP()
+x = jnp.ones((20, 100, 4))
+params = mlp.init(jax.random.PRNGKey(0), x)
+def fwd(x):
+    return mlp.apply(params, x)
+
+# Traditional loop implementation
+lapl = jax.jit(jax.vmap(folx.LoopLaplacianOperator()(fwd)))
+%time jax.block_until_ready(lapl(x)) # Wall time: 1.42 s
+%timeit jax.block_until_ready(lapl(x)) # 224 ms ± 54 µs per loop (mean ± std. dev. of 7 runs, 1 loop each)
+
+# Forward laplacian without sparsity
+lapl = jax.jit(jax.vmap(folx.ForwardLaplacianOperator(0)(fwd)))
+%time jax.block_until_ready(lapl(x)) # Wall time: 2.66 s
+%timeit jax.block_until_ready(lapl(x)) # 48.7 ms ± 42.1 µs per loop (mean ± std. dev. of 7 runs, 10 loops each)
+
+# Forward laplacian with sparsity
+lapl = jax.jit(jax.vmap(folx.ForwardLaplacianOperator(4)(fwd)))
+%time jax.block_until_ready(lapl(x)) # Wall time: 5.05 s
+%timeit jax.block_until_ready(lapl(x)) # 2.59 ms ± 15.3 µs per loop (mean ± std. dev. of 7 runs, 100 loops each)
+```
+For electronic wave function like FermiNet or PsiFormer, `sparsity_threshold=6` is a recommended value. But, tuning this hyperparameter may accelerate computations.
 
 ## Introduction
-To avoid custom wrappers for all of JAX's commands, the forward laplacian is implemented as custom interpreter for Jaxpr. 
+To avoid custom wrappers for all of JAX's commands, the forward laplacian is implemented as custom interpreter for Jaxpr.
 This means if you have a function
 ```python
 class Fn(Protocol):
     def __call__(self, *args: PyTree[Array]) -> PyTree[Array]:
         ...
 ```
 the resulting function will have the signature:
 ```python
 class LaplacianFn(Protocol):
     def __call__(self, *args: PyTree[Array]) -> PyTree[FwdLaplArray]:
         ...
 ```
-where `FwdLaplArray` is a triplet of 
+where `FwdLaplArray` is a triplet of
 ```python
 FwdLaplArray.x # jax.Array f(x) f(x).shape
 FwdLaplArray.jacobian # FwdJacobian J_f(x)
 FwdLaplArray.laplacian # jax.Array tr(H_f(x)) f(x).shape
 ```
 The jacobian is implemented by a custom class as the forward laplacian supports automatic sparsity. To get the full jacobian:
 ```python
@@ -108,30 +147,30 @@
 ## Implementation
 
 When you call the function returned by `forward_laplacian(fn)`, we first use `jax.make_jaxpr` to obtain the jaxpr for `fn`.
 But instead of using the [standard evaluation pipeline](https://github.com/google/jax/blob/776baba0a3fca15a909cb7d108eea830cbe3fc1d/jax/_src/core.py#L436), we use a custom interpreter that replaces all operations to propate `FwdLaplArray` forward instead of regular `jax.Array`.
 
 ### Package structure
 The general structure of the package is
-* `interpreter.py` contains the evaluation of jaxpr and exported function decorator. 
+* `interpreter.py` contains the evaluation of jaxpr and exported function decorator.
 * `wrapper.py` contains subfunction decorator that maps a function that takes `jax.Array`s to a function that accepts `FwdLaplArray`s instead.
 * `wrapped_functions.py` contains a registry of predefined functions as well as utility functions to add new functions to the registry.
 * `jvp.py` contains logic for jacobian vector products.
 * `hessian.py` contains logic for tr(JHJ^T).
 * `custom_hessian.py` contains special treatment logic for tr(JHJ^T).
 * `api.py` contains general interfaces shared in the package.
 * `operators.py` contains a forward laplacian operator as well as alternatives.
 * `utils.py` contains several small utility functions.
-* `tree_utils.py` contains several utility functions for PyTrees. 
+* `tree_utils.py` contains several utility functions for PyTrees.
 * `vmap.py` contains a batched vmap implementation to reduce memory usage by going through a batch sequentially in chunks.
 
 
 ### Function Annotations
 There is a default interpreter that will simply apply the rules outlined above but if additional information about a function is available, e.g., that it applies elementwise like `jnp.tanh`, we can do better.
-These additional annotations are available in `wrapped_functions.py`'s `_LAPLACE_FN_REGISTRY`. 
+These additional annotations are available in `wrapped_functions.py`'s `_LAPLACE_FN_REGISTRY`.
 Specifically, to augment a function `fn` to accept `FwdLaplArray` instead of regular `jax.Array`, we wrap it with `wrap_forward_laplacian` from `fwd_laplacian.py`:
 ```python
 wrap_forward_laplacian(jnp.tanh, in_axes=())
 ```
 In this case, we annotate the function to be applied elementwise, i.e., `()` indicates that none of the axes are relevant for the function.
 
 If we know nothing about which axes might be essential, one must pass `None` (the default value) to mark all axes as imporatnt, e.g.,
@@ -173,38 +212,41 @@
 ```
 
 
 ### Sparsity
 Sparsity is detected at compile time, this has the advantage of avoiding expensive index computations at runtime and enables efficient reductions. However, it completely prohibits dynamic indexing, i.e., if indices are data-dependent we will simply default to full jacobians.
 
 As we know a lot about the sparsity structure apriori, e.g., that we are only sparse in one dimension, we use a custom sparsity operations that are more efficient than relying on JAX's default `BCOO` (further, at the time of writing, the support for `jax.experimental.sparse` is quite bad).
-So, the sparsity data format is implemented in `FwdJacobian` in `api.py`. Instead of storing a dense array `(m, n)` for a function `f:R^n -> R^m`, we store only the non-zero data in a `(m,d)` array where `d<n` is the maximum number of non-zero inputs any output depends on. 
+So, the sparsity data format is implemented in `FwdJacobian` in `api.py`. Instead of storing a dense array `(m, n)` for a function `f:R^n -> R^m`, we store only the non-zero data in a `(m,d)` array where `d<n` is the maximum number of non-zero inputs any output depends on.
 To be able to recreate the larger `(m,n)` array from the `(m,d)` array, we additional keep track of the indices in the last dimension in a mask `(m,d)` dimensional array of integers `0<mask_ij<n`.
 
 Masks are treated as compile time static and will be traced automatically. If the tracing is not possible, e.g., due to data dependent indexing, we will fall back to a dense implementation. These propagation rules are implemented in `jvp.py`.
 
-##### Omnistaging
-If arrays do not depend on the initial input, they are typically still traced to better optimize the final program. This is called [omnistaging](https://github.com/google/jax/pull/3370). While this generally is beneficial, it does not allow us to perform indexing as tracer hide the actual data. 
-So, if we use sparsity we want to compute all arrays that do not explicitly depend on the input such that we could use them for index operations.
-While this is not documented, it can be accomplished by overwriting the global trace via:
+
+### Memory efficiency
+The forward laplacian uses more GPU memory due to the full materialization of the Jacobian matrix.
+To compensate for this, it is recommended to loop over the batch size (while other implementations typically loop over the Hessian).
+We provide an easy to use utility for this via `folx.batched_vmap` which functions like `jax.vmap` but chunks the input into batches and operates on these sequentially.
 ```python
-from jax import core
+from folx import batched_vmap
+
+def f(x):
+    return x**2
 
-with core.new_main(core.EvalTrace, dynamic=True):
-    ...
+batched_f = batched_vmap(f, max_batch_size=64)
 ```
 
 ## Citation
 If you find work helpful, please consider citing it as
 ```
-@software{folx2023gao,
-  author = {Nichoals Gao and Jonas Köhler and Adam Foster},
+@software{gao2023folx,
+  author = {Nicholas Gao and Jonas Köhler and Adam Foster},
   title = {folx - Forward Laplacian for JAX},
   url = {http://github.com/microsoft/folx},
-  version = {0.2.0},
+  version = {0.2.5},
   year = {2023},
 }
 ```
 as well as the original forward laplacian:
 ```
 @article{li2023forward,
   title={Forward Laplacian: A New Computational Framework for Neural Network-based Variational Monte Carlo},
@@ -226,13 +268,13 @@
 
 This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
 For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
 contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
 
 ## Trademarks
 
-This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft 
-trademarks or logos is subject to and must follow 
+This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft
+trademarks or logos is subject to and must follow
 [Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general).
 Use of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship.
 Any use of third-party trademarks or logos are subject to those third-party's policies.
```

