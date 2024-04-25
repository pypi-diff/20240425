# Comparing `tmp/quadax-0.2.0.tar.gz` & `tmp/quadax-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quadax-0.2.0.tar", last modified: Fri Nov  3 21:19:42 2023, max compression
+gzip compressed data, was "quadax-0.2.1.tar", last modified: Thu Apr 25 02:09:16 2024, max compression
```

## Comparing `quadax-0.2.0.tar` & `quadax-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 21:19:42.721958 quadax-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2023-11-03 21:19:05.000000 quadax-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-11-03 21:19:05.000000 quadax-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2023-11-03 21:19:42.721958 quadax-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2023-11-03 21:19:05.000000 quadax-0.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      248 2023-11-03 21:19:05.000000 quadax-0.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 21:19:42.725958 quadax-0.2.0/quadax/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2023-11-03 21:19:05.000000 quadax-0.2.0/quadax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2023-11-03 21:19:42.725958 quadax-0.2.0/quadax/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    22091 2023-11-03 21:19:05.000000 quadax-0.2.0/quadax/adaptive.py
--rw-r--r--   0 runner    (1001) docker     (127)     9358 2023-11-03 21:19:05.000000 quadax-0.2.0/quadax/fixed_order.py
--rw-r--r--   0 runner    (1001) docker     (127)    38362 2023-11-03 21:19:05.000000 quadax-0.2.0/quadax/quad_weights.py
--rw-r--r--   0 runner    (1001) docker     (127)     7820 2023-11-03 21:19:05.000000 quadax-0.2.0/quadax/romberg.py
--rw-r--r--   0 runner    (1001) docker     (127)    11190 2023-11-03 21:19:05.000000 quadax-0.2.0/quadax/sampled.py
--rw-r--r--   0 runner    (1001) docker     (127)     8830 2023-11-03 21:19:05.000000 quadax-0.2.0/quadax/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 21:19:42.721958 quadax-0.2.0/quadax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2023-11-03 21:19:42.000000 quadax-0.2.0/quadax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      476 2023-11-03 21:19:42.000000 quadax-0.2.0/quadax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-03 21:19:42.000000 quadax-0.2.0/quadax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-11-03 21:19:42.000000 quadax-0.2.0/quadax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-03 21:19:42.000000 quadax-0.2.0/quadax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      455 2023-11-03 21:19:05.000000 quadax-0.2.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-11-03 21:19:05.000000 quadax-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2023-11-03 21:19:42.725958 quadax-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2023-11-03 21:19:05.000000 quadax-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 21:19:42.721958 quadax-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    19192 2023-11-03 21:19:05.000000 quadax-0.2.0/tests/test_adaptive.py
--rw-r--r--   0 runner    (1001) docker     (127)     5371 2023-11-03 21:19:05.000000 quadax-0.2.0/tests/test_derivatives.py
--rw-r--r--   0 runner    (1001) docker     (127)     4873 2023-11-03 21:19:05.000000 quadax-0.2.0/tests/test_sampled.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:09:16.711716 quadax-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-25 02:08:50.000000 quadax-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-25 02:08:50.000000 quadax-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-04-25 02:09:16.711716 quadax-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-25 02:08:50.000000 quadax-0.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-25 02:08:50.000000 quadax-0.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:09:16.711716 quadax-0.2.1/quadax/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-25 02:08:50.000000 quadax-0.2.1/quadax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-25 02:09:16.711716 quadax-0.2.1/quadax/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22366 2024-04-25 02:08:50.000000 quadax-0.2.1/quadax/adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9358 2024-04-25 02:08:50.000000 quadax-0.2.1/quadax/fixed_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38362 2024-04-25 02:08:50.000000 quadax-0.2.1/quadax/quad_weights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8082 2024-04-25 02:08:50.000000 quadax-0.2.1/quadax/romberg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-25 02:08:50.000000 quadax-0.2.1/quadax/sampled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9112 2024-04-25 02:08:50.000000 quadax-0.2.1/quadax/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:09:16.711716 quadax-0.2.1/quadax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-04-25 02:09:16.000000 quadax-0.2.1/quadax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-25 02:09:16.000000 quadax-0.2.1/quadax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 02:09:16.000000 quadax-0.2.1/quadax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 02:09:16.000000 quadax-0.2.1/quadax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 02:09:16.000000 quadax-0.2.1/quadax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-25 02:08:50.000000 quadax-0.2.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-25 02:08:50.000000 quadax-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-25 02:09:16.711716 quadax-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-25 02:08:50.000000 quadax-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:09:16.711716 quadax-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    19167 2024-04-25 02:08:50.000000 quadax-0.2.1/tests/test_adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-04-25 02:08:50.000000 quadax-0.2.1/tests/test_derivatives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-04-25 02:08:50.000000 quadax-0.2.1/tests/test_sampled.py
```

### Comparing `quadax-0.2.0/LICENSE` & `quadax-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quadax-0.2.0/PKG-INFO` & `quadax-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quadax
-Version: 0.2.0
+Version: 0.2.1
 Summary: Numerical quadrature with JAX
 Home-page: https://github.com/f0uriest/quadax
 Author: Rory Conlin
 Author-email: wconlin@princeton.edu
 License: MIT
 Project-URL: Issues Tracker, https://github.com/f0uriest/quadax/issues
 Project-URL: Contributing, https://github.com/f0uriest/quadax/blob/master/CONTRIBUTING.rst
@@ -21,17 +21,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: jax[cpu]<=0.4.14,>=0.3.2
-Requires-Dist: numpy<1.25.0,>=1.20.0
-Requires-Dist: scipy<1.11.0,>=1.5.0
+Requires-Dist: jax<=0.5.0,>=0.3.2
+Requires-Dist: numpy<2.0,>=1.20.0
 
 
 ########
 quadax
 ########
 |License| |DOI| |Issues| |Pypi|
 
@@ -70,21 +69,21 @@
 
 .. code-block:: python
 
     import jax.numpy as jnp
     import numpy as np
     from quadax import quadgk
 
-    f = lambda t: t * jnp.log(1 + t)
+    fun = lambda t: t * jnp.log(1 + t)
 
-    epsabs = epsrel = 1e-14
+    epsabs = epsrel = 1e-5 # by default jax uses 32 bit, higher accuracy requires going to 64 bit
     a, b = 0, 1
     y, info = quadgk(fun, [a, b], epsabs=epsabs, epsrel=epsrel)
     assert info.err < max(epsabs, epsrel*abs(y))
-    np.testing.assert_allclose(y, 1/4, rtol=1e-14, atol=1e-14)
+    np.testing.assert_allclose(y, 1/4, rtol=epsrel, atol=epsabs)
 
 
 For full details of various options see the `API documentation <https://quadax.readthedocs.io/en/latest/api.html>`__
 
 
 .. |License| image:: https://img.shields.io/github/license/f0uriest/quadax?color=blue&logo=open-source-initiative&logoColor=white
     :target: https://github.com/f0uriest/quadax/blob/master/LICENSE
```

### Comparing `quadax-0.2.0/README.rst` & `quadax-0.2.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -39,21 +39,21 @@
 
 .. code-block:: python
 
     import jax.numpy as jnp
     import numpy as np
     from quadax import quadgk
 
-    f = lambda t: t * jnp.log(1 + t)
+    fun = lambda t: t * jnp.log(1 + t)
 
-    epsabs = epsrel = 1e-14
+    epsabs = epsrel = 1e-5 # by default jax uses 32 bit, higher accuracy requires going to 64 bit
     a, b = 0, 1
     y, info = quadgk(fun, [a, b], epsabs=epsabs, epsrel=epsrel)
     assert info.err < max(epsabs, epsrel*abs(y))
-    np.testing.assert_allclose(y, 1/4, rtol=1e-14, atol=1e-14)
+    np.testing.assert_allclose(y, 1/4, rtol=epsrel, atol=epsabs)
 
 
 For full details of various options see the `API documentation <https://quadax.readthedocs.io/en/latest/api.html>`__
 
 
 .. |License| image:: https://img.shields.io/github/license/f0uriest/quadax?color=blue&logo=open-source-initiative&logoColor=white
     :target: https://github.com/f0uriest/quadax/blob/master/LICENSE
```

### Comparing `quadax-0.2.0/quadax/adaptive.py` & `quadax-0.2.1/quadax/adaptive.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 """Functions for globally h-adaptive quadrature."""
 
 import jax
 import jax.numpy as jnp
 
 from .fixed_order import fixed_quadcc, fixed_quadgk, fixed_quadts
-from .utils import QuadratureInfo, bounded_while_loop, errorif, map_interval, wrap_func
+from .utils import (
+    QuadratureInfo,
+    bounded_while_loop,
+    errorif,
+    map_interval,
+    setdefault,
+    wrap_func,
+)
 
 NORMAL_EXIT = 0
 MAX_NINTER = 1
 ROUNDOFF = 2
 BAD_INTEGRAND = 3
 NO_CONVERGE = 4
 DIVERGENT = 5
 
 
 def quadgk(
     fun,
     interval,
     args=(),
     full_output=False,
-    epsabs=1.4e-8,
-    epsrel=1.4e-8,
+    epsabs=None,
+    epsrel=None,
     max_ninter=50,
     order=21,
     norm=jnp.inf,
 ):
     """Global adaptive quadrature using Gauss-Konrod rule.
 
     Integrate fun from `interval[0]` to `interval[-1]` using a h-adaptive scheme with
@@ -45,18 +52,18 @@
         denote infinite intervals.
     args : tuple, optional
         Extra arguments passed to fun.
     full_output : bool, optional
         If True, return the full state of the integrator. See below for more
         information.
     epsabs, epsrel : float, optional
-        Absolute and relative error tolerance. Default is 1.4e-8. Algorithm tries to
-        obtain an accuracy of ``abs(i-result) <= max(epsabs, epsrel*abs(i))``
-        where ``i`` = integral of `fun` over `interval`, and ``result`` is the
-        numerical approximation.
+        Absolute and relative error tolerance. Default is square root of
+        machine precision. Algorithm tries to obtain an accuracy of
+        ``abs(i-result) <= max(epsabs, epsrel*abs(i))`` where ``i`` = integral of
+        `fun` over `interval`, and ``result`` is the numerical approximation.
     max_ninter : int, optional
         An upper bound on the number of sub-intervals used in the adaptive
         algorithm.
     order : {15, 21, 31, 41, 51, 61}
         Order of local integration rule.
     norm : int, callable
         Norm to use for measuring error for vector valued integrands. No effect if the
@@ -116,16 +123,16 @@
 
 
 def quadcc(
     fun,
     interval,
     args=(),
     full_output=False,
-    epsabs=1.4e-8,
-    epsrel=1.4e-8,
+    epsabs=None,
+    epsrel=None,
     max_ninter=50,
     order=32,
     norm=jnp.inf,
 ):
     """Global adaptive quadrature using Clenshaw-Curtis rule.
 
     Integrate fun from `interval[0]` to `interval[-1]` using a h-adaptive scheme with
@@ -145,18 +152,18 @@
         denote infinite intervals.
     args : tuple, optional
         Extra arguments passed to fun.
     full_output : bool, optional
         If True, return the full state of the integrator. See below for more
         information.
     epsabs, epsrel : float, optional
-        Absolute and relative error tolerance. Default is 1.4e-8. Algorithm tries to
-        obtain an accuracy of ``abs(i-result) <= max(epsabs, epsrel*abs(i))``
-        where ``i`` = integral of `fun` over `interval`, and ``result`` is the
-        numerical approximation.
+        Absolute and relative error tolerance. Default is square root of
+        machine precision. Algorithm tries to obtain an accuracy of
+        ``abs(i-result) <= max(epsabs, epsrel*abs(i))`` where ``i`` = integral of
+        `fun` over `interval`, and ``result`` is the numerical approximation.
     max_ninter : int, optional
         An upper bound on the number of sub-intervals used in the adaptive
         algorithm.
     order : {8, 16, 32, 64, 128, 256}
         Order of local integration rule.
     norm : int, callable
         Norm to use for measuring error for vector valued integrands. No effect if the
@@ -216,16 +223,16 @@
 
 
 def quadts(
     fun,
     interval,
     args=(),
     full_output=False,
-    epsabs=1.4e-8,
-    epsrel=1.4e-8,
+    epsabs=None,
+    epsrel=None,
     max_ninter=50,
     order=61,
     norm=jnp.inf,
 ):
     """Global adaptive quadrature using trapezoidal tanh-sinh rule.
 
     Integrate fun from `interval[0]` to `interval[-1]` using a h-adaptive scheme with
@@ -244,18 +251,18 @@
         denote infinite intervals.
     args : tuple, optional
         Extra arguments passed to fun.
     full_output : bool, optional
         If True, return the full state of the integrator. See below for more
         information.
     epsabs, epsrel : float, optional
-        Absolute and relative error tolerance. Default is 1.4e-8. Algorithm tries to
-        obtain an accuracy of ``abs(i-result) <= max(epsabs, epsrel*abs(i))``
-        where ``i`` = integral of `fun` over `interval`, and ``result`` is the
-        numerical approximation.
+        Absolute and relative error tolerance. Default is square root of
+        machine precision. Algorithm tries to obtain an accuracy of
+        ``abs(i-result) <= max(epsabs, epsrel*abs(i))`` where ``i`` = integral of
+        `fun` over `interval`, and ``result`` is the numerical approximation.
     max_ninter : int, optional
         An upper bound on the number of sub-intervals used in the adaptive
         algorithm.
     order : {41, 61, 81, 101}
         Order of local integration rule.
     norm : int, callable
         Norm to use for measuring error for vector valued integrands. No effect if the
@@ -316,16 +323,16 @@
 
 def adaptive_quadrature(
     rule,
     fun,
     interval,
     args=(),
     full_output=False,
-    epsabs=1.4e-8,
-    epsrel=1.4e-8,
+    epsabs=None,
+    epsrel=None,
     max_ninter=50,
     norm=jnp.inf,
     **kwargs,
 ):
     """Global adaptive quadrature.
 
     This is a lower level routine allowing for custom local quadrature rules. For most
@@ -352,18 +359,18 @@
         denote infinite intervals.
     args : tuple, optional
         Extra arguments passed to fun.
     full_output : bool, optional
         If True, return the full state of the integrator. See below for more
         information.
     epsabs, epsrel : float, optional
-        Absolute and relative error tolerance. Default is 1.4e-8. Algorithm tries to
-        obtain an accuracy of ``abs(i-result) <= max(epsabs, epsrel*abs(i))``
-        where ``i`` = integral of `fun` over `interval`, and ``result`` is the
-        numerical approximation.
+        Absolute and relative error tolerance. Default is square root of
+        machine precision. Algorithm tries to obtain an accuracy of
+        ``abs(i-result) <= max(epsabs, epsrel*abs(i))`` where ``i`` = integral of
+        `fun` over `interval`, and ``result`` is the numerical approximation.
     max_ninter : int, optional
         An upper bound on the number of sub-intervals used in the adaptive
         algorithm.
     norm : int, callable
         Norm to use for measuring error for vector valued integrands. No effect if the
         integrand is scalar valued. If an int, uses p-norm of the given order, otherwise
         should be callable.
@@ -400,14 +407,16 @@
 
     """
     errorif(
         max_ninter < len(interval) - 1,
         ValueError,
         f"max_ninter={max_ninter} is not enough for {len(interval)-1} breakpoints",
     )
+    epsabs = setdefault(epsabs, jnp.sqrt(jnp.finfo(jnp.array(1.0)).eps))
+    epsrel = setdefault(epsrel, jnp.sqrt(jnp.finfo(jnp.array(1.0)).eps))
     _norm = norm if callable(norm) else lambda x: jnp.linalg.norm(x.flatten(), ord=norm)
     fun, interval = map_interval(fun, interval)
     vfunc = wrap_func(fun, args)
     f = jax.eval_shape(vfunc, (interval[0] + interval[-1] / 2))
     epmach = jnp.finfo(f.dtype).eps
     shape = f.shape
```

### Comparing `quadax-0.2.0/quadax/fixed_order.py` & `quadax-0.2.1/quadax/fixed_order.py`

 * *Files identical despite different names*

### Comparing `quadax-0.2.0/quadax/quad_weights.py` & `quadax-0.2.1/quadax/quad_weights.py`

 * *Files identical despite different names*

### Comparing `quadax-0.2.0/quadax/romberg.py` & `quadax-0.2.1/quadax/romberg.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 import jax.numpy as jnp
 
 from .utils import (
     QuadratureInfo,
     bounded_while_loop,
     errorif,
     map_interval,
+    setdefault,
     tanhsinh_transform,
     wrap_func,
 )
 
 
 def romberg(
     fun,
     interval,
     args=(),
     full_output=False,
-    epsabs=1.4e-8,
-    epsrel=1.4e-8,
+    epsabs=None,
+    epsrel=None,
     divmax=20,
     norm=jnp.inf,
 ):
     """Romberg integration of a callable function or method.
 
     Returns the integral of `fun` (a function of one variable) over `interval`.
 
@@ -42,15 +43,16 @@
         additional arguments passed to fun
     full_output : bool, optional
         If True, return the full state of the integrator. See below for more
         information.
     epsabs, epsrel : float
         Absolute and relative tolerances. If I1 and I2 are two
         successive approximations to the integral, algorithm terminates
-        when abs(I1-I2) < max(epsabs, epsrel*|I2|)
+        when abs(I1-I2) < max(epsabs, epsrel*|I2|). Default is square root of
+        machine precision.
     divmax : int, optional
         Maximum order of extrapolation. Default is 20.
         Total number of function evaluations will be at
         most 2**divmax + 1
     norm : int, callable
         Norm to use for measuring error for vector valued integrands. No effect if the
         integrand is scalar valued. If an int, uses p-norm of the given order, otherwise
@@ -84,14 +86,16 @@
 
     """
     errorif(
         len(interval) != 2,
         NotImplementedError,
         "Romberg integration with breakpoints not supported",
     )
+    epsabs = setdefault(epsabs, jnp.sqrt(jnp.finfo(jnp.array(1.0)).eps))
+    epsrel = setdefault(epsrel, jnp.sqrt(jnp.finfo(jnp.array(1.0)).eps))
     _norm = norm if callable(norm) else lambda x: jnp.linalg.norm(x.flatten(), ord=norm)
     # map a, b -> [-1, 1]
     fun, interval = map_interval(fun, interval)
     vfunc = wrap_func(fun, args)
     a, b = interval
     f = jax.eval_shape(vfunc, (a + b / 2))
 
@@ -145,16 +149,16 @@
 
 
 def rombergts(
     fun,
     interval,
     args=(),
     full_output=False,
-    epsabs=1.4e-8,
-    epsrel=1.4e-8,
+    epsabs=None,
+    epsrel=None,
     divmax=20,
     norm=jnp.inf,
 ):
     """Romberg integration with tanh-sinh (aka double exponential) transformation.
 
     Returns the integral of `fun` (a function of one variable) over `interval`.
 
@@ -173,15 +177,16 @@
         additional arguments passed to fun
     full_output : bool, optional
         If True, return the full state of the integrator. See below for more
         information.
     epsabs, epsrel : float
         Absolute and relative tolerances. If I1 and I2 are two
         successive approximations to the integral, algorithm terminates
-        when abs(I1-I2) < max(epsabs, epsrel*|I2|)
+        when abs(I1-I2) < max(epsabs, epsrel*|I2|). Default is square root of
+        machine precision.
     divmax : int, optional
         Maximum order of extrapolation. Default is 20.
         Total number of function evaluations will be at
         most 2**divmax + 1
     norm : int, callable
         Norm to use for measuring error for vector valued integrands. No effect if the
         integrand is scalar valued. If an int, uses p-norm of the given order, otherwise
```

### Comparing `quadax-0.2.0/quadax/sampled.py` & `quadax-0.2.1/quadax/sampled.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,20 +88,24 @@
     array([[0, 1, 2],
            [3, 4, 5]])
     >>> trapezoid(a, axis=0)
     array([1.5, 2.5, 3.5])
     >>> trapezoid(a, axis=1)
     array([2.,  8.])
     """
-    # Future-proofing, in case JAX moves from trapz to trapezoid for the same
-    # reasons as SciPy
-    if hasattr(jnp, "trapezoid"):
-        return jnp.trapezoid(y, x=x, dx=dx, axis=axis)
+    if x is None:
+        y_arr, dx_array = jnp.asarray(y), jnp.asarray(dx)
     else:
-        return jnp.trapz(y, x=x, dx=dx, axis=axis)
+        y_arr, x_arr = jnp.asarray(y), jnp.asarray(x)
+        if x_arr.ndim == 1:
+            dx_array = jnp.diff(x_arr)
+        else:
+            dx_array = jnp.moveaxis(jnp.diff(x_arr, axis=axis), axis, -1)
+    y_arr = jnp.moveaxis(y_arr, axis, -1)
+    return 0.5 * (dx_array * (y_arr[..., 1:] + y_arr[..., :-1])).sum(-1)
 
 
 def cumulative_trapezoid(y, x=None, dx=1.0, axis=-1, initial=None):
     """Cumulatively integrate y(x) using the composite trapezoidal rule.
 
     Parameters
     ----------
```

### Comparing `quadax-0.2.0/quadax/utils.py` & `quadax-0.2.1/quadax/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -264,7 +264,16 @@
     # could do some fancy stuff with checkpointing here like in equinox but the loops
     # in quadax usually only do ~100 iterations max so probably not worth it.
 
     def scanfun(state, *args):
         return jax.lax.cond(condfun(state), bodyfun, lambda x: x, state), None
 
     return jax.lax.scan(scanfun, init_val, None, bound)[0]
+
+
+def setdefault(val, default, cond=None):
+    """Return val if condition is met, otherwise default.
+
+    If cond is None, then it checks if val is not None, returning val
+    or default accordingly.
+    """
+    return val if cond or (cond is None and val is not None) else default
```

### Comparing `quadax-0.2.0/quadax.egg-info/PKG-INFO` & `quadax-0.2.1/quadax.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quadax
-Version: 0.2.0
+Version: 0.2.1
 Summary: Numerical quadrature with JAX
 Home-page: https://github.com/f0uriest/quadax
 Author: Rory Conlin
 Author-email: wconlin@princeton.edu
 License: MIT
 Project-URL: Issues Tracker, https://github.com/f0uriest/quadax/issues
 Project-URL: Contributing, https://github.com/f0uriest/quadax/blob/master/CONTRIBUTING.rst
@@ -21,17 +21,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: jax[cpu]<=0.4.14,>=0.3.2
-Requires-Dist: numpy<1.25.0,>=1.20.0
-Requires-Dist: scipy<1.11.0,>=1.5.0
+Requires-Dist: jax<=0.5.0,>=0.3.2
+Requires-Dist: numpy<2.0,>=1.20.0
 
 
 ########
 quadax
 ########
 |License| |DOI| |Issues| |Pypi|
 
@@ -70,21 +69,21 @@
 
 .. code-block:: python
 
     import jax.numpy as jnp
     import numpy as np
     from quadax import quadgk
 
-    f = lambda t: t * jnp.log(1 + t)
+    fun = lambda t: t * jnp.log(1 + t)
 
-    epsabs = epsrel = 1e-14
+    epsabs = epsrel = 1e-5 # by default jax uses 32 bit, higher accuracy requires going to 64 bit
     a, b = 0, 1
     y, info = quadgk(fun, [a, b], epsabs=epsabs, epsrel=epsrel)
     assert info.err < max(epsabs, epsrel*abs(y))
-    np.testing.assert_allclose(y, 1/4, rtol=1e-14, atol=1e-14)
+    np.testing.assert_allclose(y, 1/4, rtol=epsrel, atol=epsabs)
 
 
 For full details of various options see the `API documentation <https://quadax.readthedocs.io/en/latest/api.html>`__
 
 
 .. |License| image:: https://img.shields.io/github/license/f0uriest/quadax?color=blue&logo=open-source-initiative&logoColor=white
     :target: https://github.com/f0uriest/quadax/blob/master/LICENSE
```

### Comparing `quadax-0.2.0/setup.cfg` & `quadax-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `quadax-0.2.0/setup.py` & `quadax-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `quadax-0.2.0/tests/test_adaptive.py` & `quadax-0.2.1/tests/test_adaptive.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Tests for adaptive quadrature routines."""
 
 import jax.numpy as jnp
 import numpy as np
 import pytest
 import scipy
-from jax.config import config as jax_config
+from jax import config
 
 from quadax import quadcc, quadgk, quadts, romberg, rombergts
 
-jax_config.update("jax_enable_x64", True)
+config.update("jax_enable_x64", True)
 
 example_problems = [
     # problem 0
     {"fun": lambda t: t * jnp.log(1 + t), "interval": [0, 1], "val": 1 / 4},
     # problem 1
     {
         "fun": lambda t: t**2 * jnp.arctan(t),
```

### Comparing `quadax-0.2.0/tests/test_derivatives.py` & `quadax-0.2.1/tests/test_derivatives.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Tests for custom jvp for adaptive quadrature routines."""
 
 import jax
 import jax.numpy as jnp
 import numpy as np
-from jax.config import config as jax_config
+from jax import config
 
 from quadax import quadcc, quadgk, quadts, romberg, rombergts
 
-jax_config.update("jax_enable_x64", True)
+config.update("jax_enable_x64", True)
+
 
 rng = np.random.default_rng(0)
 A0 = 0.5 - rng.random(3)
 
 
 example_problems = [
     # problem 0
```

### Comparing `quadax-0.2.0/tests/test_sampled.py` & `quadax-0.2.1/tests/test_sampled.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Tests for sampled quadrature routines."""
 
 import jax
 import jax.numpy as jnp
 import numpy as np
-from jax.config import config as jax_config
+from jax import config
 
 from quadax import cumulative_trapezoid, simpson, trapezoid
 
-jax_config.update("jax_enable_x64", True)
+config.update("jax_enable_x64", True)
 
 rng = np.random.default_rng(0)
 A0 = 0.5 - rng.random(10)
 
 example_problems = [
     # problem 0
     {
```

