# Comparing `tmp/pldag-0.7.2.tar.gz` & `tmp/pldag-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pldag-0.7.2.tar", max compression
+gzip compressed data, was "pldag-0.7.3.tar", max compression
```

## Comparing `pldag-0.7.2.tar` & `pldag-0.7.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.7.2/LICENSE
--rw-r--r--   0        0        0     2812 2024-04-22 11:08:59.388067 pldag-0.7.2/README.md
--rw-r--r--   0        0        0    31535 2024-04-23 20:41:43.576978 pldag-0.7.2/pldag/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 11:08:54.241329 pldag-0.7.2/pldag/solver/__init__.py
--rw-r--r--   0        0        0      973 2024-04-22 15:04:47.780408 pldag-0.7.2/pldag/solver/glpk_solver.py
--rw-r--r--   0        0        0      399 2024-04-23 20:41:57.428526 pldag-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     3303 1970-01-01 00:00:00.000000 pldag-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.7.3/LICENSE
+-rw-r--r--   0        0        0     2812 2024-04-22 11:08:59.388067 pldag-0.7.3/README.md
+-rw-r--r--   0        0        0    31545 2024-04-25 07:31:01.760869 pldag-0.7.3/pldag/__init__.py
+-rw-r--r--   0        0        0       47 2024-04-25 07:41:38.175676 pldag-0.7.3/pldag/solver/__init__.py
+-rw-r--r--   0        0        0     1020 2024-04-25 07:41:53.592443 pldag-0.7.3/pldag/solver/glpk_solver.py
+-rw-r--r--   0        0        0      399 2024-04-25 07:40:31.690286 pldag-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     3303 1970-01-01 00:00:00.000000 pldag-0.7.3/PKG-INFO
```

### Comparing `pldag-0.7.2/LICENSE` & `pldag-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pldag-0.7.2/README.md` & `pldag-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `pldag-0.7.2/pldag/__init__.py` & `pldag-0.7.3/pldag/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -893,15 +893,15 @@
         for i, obj in enumerate(objectives):
             obj_mat[i, [self._col(k) for k in obj]] = list(obj.values())
 
         if solver == Solver.GLPK:
             from pldag.solver.glpk_solver import solve_lp
             solutions = solve_lp(A, b, obj_mat, set(np.argwhere((self._dvec.real != 0) | (self._dvec.imag != 1)).T[0].tolist()))
         else:
-            raise ValueError("Solver not implemented.")
+            raise ValueError(f"Solver `{solver}` not installed.")
         
         return list(
             map(
                 lambda solution: dict(
                     zip(
                         variables.T[0], 
                         map(
```

### Comparing `pldag-0.7.2/pldag/solver/glpk_solver.py` & `pldag-0.7.3/pldag/solver/glpk_solver.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import numpy as np
 import functools
 
+from . import NoSolutionsException
+
 try:
     import npycvx
 except ImportError:
     raise ImportError("Please install the npycvx package to use GLPK solver module.")
 
 def solve_lp(A: np.ndarray, b: np.ndarray, objectives: np.ndarray, int_vrs: set=set()):
     """
@@ -28,10 +30,10 @@
         map(
             solve_part_fn, 
             objectives
         )
     )
 
     if any(map(lambda x: x[0] != 'optimal', solutions)):
-        raise Exception("Could not find solutions. Please check constraints.")
+        raise NoSolutionsException("Could not find solutions. Please check constraints.")
     
     return list(map(lambda x: x[1], solutions))
```

### Comparing `pldag-0.7.2/PKG-INFO` & `pldag-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pldag
-Version: 0.7.2
+Version: 0.7.3
 Summary: 
 Author: znittzel
 Author-email: rikard@ourstudio.se
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

