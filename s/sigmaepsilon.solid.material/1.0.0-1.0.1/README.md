# Comparing `tmp/sigmaepsilon_solid_material-1.0.0.tar.gz` & `tmp/sigmaepsilon_solid_material-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigmaepsilon_solid_material-1.0.0.tar", max compression
+gzip compressed data, was "sigmaepsilon_solid_material-1.0.1.tar", max compression
```

## Comparing `sigmaepsilon_solid_material-1.0.0.tar` & `sigmaepsilon_solid_material-1.0.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1069 2024-02-20 18:24:43.749042 sigmaepsilon_solid_material-1.0.0/LICENSE
--rw-r--r--   0        0        0     6525 2024-02-20 18:24:43.749042 sigmaepsilon_solid_material-1.0.0/README.md
--rw-r--r--   0        0        0     2058 2024-02-20 18:24:43.789043 sigmaepsilon_solid_material-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1654 2024-02-20 18:24:43.789043 sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/__init__.py
--rw-r--r--   0        0        0      482 2024-02-20 18:24:43.789043 sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/config.py
--rw-r--r--   0        0        0     6204 2024-02-20 18:24:43.789043 sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/elasticitytensor.py
--rw-r--r--   0        0        0     2291 2024-02-20 18:24:43.789043 sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/enums.py
--rw-r--r--   0        0        0     1185 2024-02-20 18:24:43.793043 sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/evaluator.py
--rw-r--r--   0        0        0       36 2024-02-20 18:24:43.793043 sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/exceptions.py
--rw-r--r--   0        0        0      495 2024-02-20 18:24:43.793043 sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/failure/__init__.py
--rw-r--r--   0        0        0     5297 2024-02-20 18:24:43.793043 sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/failure/abstract.py
--rw-r--r--   0        0        0    10253 2024-02-20 18:24:43.793043 sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/failure/hmh.py
--rw-r--r--   0        0        0     7199 2024-02-20 18:24:43.793043 sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/failure/hoffman.py
--rw-r--r--   0        0        0       87 2024-02-20 18:24:43.793043 sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/frame/__init__.py
--rw-r--r--   0        0        0     7595 2024-02-20 18:24:43.793043 sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/frame/bernoulliframe.py
--rw-r--r--   0        0        0     6102 2024-02-20 18:24:43.793043 sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/linearelasticmaterial.py
--rw-r--r--   0        0        0     2930 2024-02-20 18:24:43.793043 sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/proto.py
--rw-r--r--   0        0        0     1572 2024-02-20 18:24:43.793043 sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/straintensor.py
--rw-r--r--   0        0        0      414 2024-02-20 18:24:43.793043 sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/stresstensor.py
--rw-r--r--   0        0        0      380 2024-02-20 18:24:43.793043 sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/surface/__init__.py
--rw-r--r--   0        0        0     4314 2024-02-20 18:24:43.793043 sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/surface/kirchhoffplate.py
--rw-r--r--   0        0        0     3461 2024-02-20 18:24:43.793043 sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/surface/kirchhoffshell.py
--rw-r--r--   0        0        0     9673 2024-02-20 18:24:43.793043 sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/surface/membrane.py
--rw-r--r--   0        0        0     3854 2024-02-20 18:24:43.793043 sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/surface/mindlinplate.py
--rw-r--r--   0        0        0    23971 2024-02-20 18:24:43.793043 sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/surface/mindlinshell.py
--rw-r--r--   0        0        0    11095 2024-02-20 18:24:43.793043 sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/surface/surface.py
--rw-r--r--   0        0        0     3322 2024-02-20 18:24:43.793043 sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/tensor2x3.py
--rw-r--r--   0        0        0      441 2024-02-20 18:24:43.793043 sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/testing.py
--rw-r--r--   0        0        0       89 2024-02-20 18:24:43.793043 sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/utils/__init__.py
--rw-r--r--   0        0        0     2400 2024-02-20 18:24:43.793043 sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/utils/bernoulli.py
--rw-r--r--   0        0        0    11438 2024-02-20 18:24:43.793043 sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/utils/hmh.py
--rw-r--r--   0        0        0     2772 2024-02-20 18:24:43.793043 sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/utils/hoffman.py
--rw-r--r--   0        0        0     2082 2024-02-20 18:24:43.793043 sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/utils/imap.py
--rw-r--r--   0        0        0     2272 2024-02-20 18:24:43.793043 sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/utils/material.py
--rw-r--r--   0        0        0     9528 2024-02-20 18:24:43.793043 sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/utils/mindlin.py
--rw-r--r--   0        0        0    10976 2024-02-20 18:24:43.793043 sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/utils/postproc.py
--rw-r--r--   0        0        0     4107 2024-02-20 18:24:43.793043 sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/utils/principal.py
--rw-r--r--   0        0        0     4463 2024-02-20 18:24:43.793043 sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/utils/surface.py
--rw-r--r--   0        0        0     4406 2024-02-20 18:24:43.793043 sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/utils/symbolic.py
--rw-r--r--   0        0        0      515 2024-02-20 18:24:43.793043 sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/utils/tr.py
--rw-r--r--   0        0        0    15544 2024-02-20 18:24:43.793043 sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/utils/utils.py
--rw-r--r--   0        0        0      283 2024-02-20 18:24:43.793043 sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/warnings.py
--rw-r--r--   0        0        0     7750 1970-01-01 00:00:00.000000 sigmaepsilon_solid_material-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-25 17:18:17.292954 sigmaepsilon_solid_material-1.0.1/LICENSE
+-rw-r--r--   0        0        0     6525 2024-04-25 17:18:17.292954 sigmaepsilon_solid_material-1.0.1/README.md
+-rw-r--r--   0        0        0     2058 2024-04-25 17:18:17.336955 sigmaepsilon_solid_material-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1738 2024-04-25 17:18:17.336955 sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/__init__.py
+-rw-r--r--   0        0        0      482 2024-04-25 17:18:17.336955 sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/config.py
+-rw-r--r--   0        0        0     6528 2024-04-25 17:18:17.336955 sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/elasticitytensor.py
+-rw-r--r--   0        0        0     2291 2024-04-25 17:18:17.336955 sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/enums.py
+-rw-r--r--   0        0        0     1185 2024-04-25 17:18:17.336955 sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/evaluator.py
+-rw-r--r--   0        0        0       36 2024-04-25 17:18:17.336955 sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/exceptions.py
+-rw-r--r--   0        0        0      495 2024-04-25 17:18:17.336955 sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/failure/__init__.py
+-rw-r--r--   0        0        0     5297 2024-04-25 17:18:17.336955 sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/failure/abstract.py
+-rw-r--r--   0        0        0    10253 2024-04-25 17:18:17.336955 sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/failure/hmh.py
+-rw-r--r--   0        0        0     7199 2024-04-25 17:18:17.340955 sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/failure/hoffman.py
+-rw-r--r--   0        0        0       87 2024-04-25 17:18:17.340955 sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/frame/__init__.py
+-rw-r--r--   0        0        0     7595 2024-04-25 17:18:17.340955 sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/frame/bernoulliframe.py
+-rw-r--r--   0        0        0     6102 2024-04-25 17:18:17.340955 sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/linearelasticmaterial.py
+-rw-r--r--   0        0        0     2930 2024-04-25 17:18:17.340955 sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/proto.py
+-rw-r--r--   0        0        0     1572 2024-04-25 17:18:17.340955 sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/straintensor.py
+-rw-r--r--   0        0        0      414 2024-04-25 17:18:17.340955 sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/stresstensor.py
+-rw-r--r--   0        0        0      380 2024-04-25 17:18:17.340955 sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/surface/__init__.py
+-rw-r--r--   0        0        0     4314 2024-04-25 17:18:17.340955 sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/surface/kirchhoffplate.py
+-rw-r--r--   0        0        0     3461 2024-04-25 17:18:17.340955 sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/surface/kirchhoffshell.py
+-rw-r--r--   0        0        0     9673 2024-04-25 17:18:17.340955 sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/surface/membrane.py
+-rw-r--r--   0        0        0     3854 2024-04-25 17:18:17.340955 sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/surface/mindlinplate.py
+-rw-r--r--   0        0        0    23971 2024-04-25 17:18:17.340955 sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/surface/mindlinshell.py
+-rw-r--r--   0        0        0    11095 2024-04-25 17:18:17.340955 sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/surface/surface.py
+-rw-r--r--   0        0        0     3322 2024-04-25 17:18:17.340955 sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/tensor2x3.py
+-rw-r--r--   0        0        0      441 2024-04-25 17:18:17.340955 sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/testing.py
+-rw-r--r--   0        0        0       89 2024-04-25 17:18:17.340955 sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/utils/__init__.py
+-rw-r--r--   0        0        0     2400 2024-04-25 17:18:17.340955 sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/utils/bernoulli.py
+-rw-r--r--   0        0        0    11439 2024-04-25 17:18:17.340955 sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/utils/hmh.py
+-rw-r--r--   0        0        0     2772 2024-04-25 17:18:17.340955 sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/utils/hoffman.py
+-rw-r--r--   0        0        0     2082 2024-04-25 17:18:17.340955 sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/utils/imap.py
+-rw-r--r--   0        0        0     2272 2024-04-25 17:18:17.340955 sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/utils/material.py
+-rw-r--r--   0        0        0     9528 2024-04-25 17:18:17.340955 sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/utils/mindlin.py
+-rw-r--r--   0        0        0    10976 2024-04-25 17:18:17.340955 sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/utils/postproc.py
+-rw-r--r--   0        0        0     4107 2024-04-25 17:18:17.340955 sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/utils/principal.py
+-rw-r--r--   0        0        0     4463 2024-04-25 17:18:17.340955 sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/utils/surface.py
+-rw-r--r--   0        0        0     4406 2024-04-25 17:18:17.340955 sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/utils/symbolic.py
+-rw-r--r--   0        0        0      515 2024-04-25 17:18:17.340955 sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/utils/tr.py
+-rw-r--r--   0        0        0    15544 2024-04-25 17:18:17.340955 sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/utils/utils.py
+-rw-r--r--   0        0        0      283 2024-04-25 17:18:17.340955 sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/warnings.py
+-rw-r--r--   0        0        0     7750 1970-01-01 00:00:00.000000 sigmaepsilon_solid_material-1.0.1/PKG-INFO
```

### Comparing `sigmaepsilon_solid_material-1.0.0/LICENSE` & `sigmaepsilon_solid_material-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sigmaepsilon_solid_material-1.0.0/README.md` & `sigmaepsilon_solid_material-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `sigmaepsilon_solid_material-1.0.0/pyproject.toml` & `sigmaepsilon_solid_material-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "sigmaepsilon.solid.material"
-version = "1.0.0"
+version = "1.0.1"
 description = "Material models for solid structures in Python."
 classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
```

### Comparing `sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/__init__.py` & `sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 from os.path import dirname, abspath
 from importlib.metadata import metadata
 
+from numba import config as nbconfig
+
+nbconfig.CUDA_LOW_OCCUPANCY_WARNINGS = False
+
 from sigmaepsilon.core.config import namespace_package_name
 
 from .frame import BernoulliFrameSection
 from .surface import (
     MindlinShellSection,
     MembraneSection,
     MindlinPlateSection,
```

### Comparing `sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/elasticitytensor.py` & `sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/elasticitytensor.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,29 +16,39 @@
 class ElasticityTensor(Tensor4):
     """
     A class to represent the 4th order stiffness tensor.
 
     Parameters
     ----------
     yield_strength: Number, Optional
-        The maximum stress the material can sustain without experiencing
-        relevant losses in performance. Default is `np.Infinity`.
+        The maximum eqivalent stress the material can sustain without experiencing
+        significant losses in performance. Default is `np.Infinity`.
+    material_params: dict, Optional
+        A dictionary of material parameters that can be used to instantiate the
+        stiffness matrix. Default is `None`.
     """
 
     number_of_stress_components = 6
 
-    def __init__(self, *args, yield_strength: Optional[Number] = np.Infinity, **kwargs):
-        self._input_params = None
-        if len(args) > 0 and isinstance(args[0], dict):
-            if _has_elastic_params(args[0]):
-                self._input_params = args[0]
-                args = (elastic_stiffness_matrix(args[0]),)
-        elif _has_elastic_params(**kwargs):
-            self._input_params = kwargs
-            args = (elastic_stiffness_matrix(**kwargs),)
+    def __init__(
+        self,
+        *args,
+        yield_strength: Optional[Number] = np.Infinity,
+        material_params: dict = None,
+        **kwargs
+    ):
+        self._input_params = material_params
+        if not self._input_params:
+            if len(args) > 0 and isinstance(args[0], dict):
+                if _has_elastic_params(args[0]):
+                    self._input_params = args[0]
+                    args = (elastic_stiffness_matrix(args[0]),)
+            elif _has_elastic_params(**kwargs):
+                self._input_params = kwargs
+                args = (elastic_stiffness_matrix(**kwargs),)
 
         self._yield_strength = yield_strength
 
         if len(args) > 0 and isinstance(args[0], ndarray):
             arr = args[0]
             shape = arr.shape
```

### Comparing `sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/enums.py` & `sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/enums.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/evaluator.py` & `sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/evaluator.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/failure/abstract.py` & `sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/failure/abstract.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/failure/hmh.py` & `sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/failure/hmh.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/failure/hoffman.py` & `sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/failure/hoffman.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/frame/bernoulliframe.py` & `sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/frame/bernoulliframe.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/linearelasticmaterial.py` & `sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/linearelasticmaterial.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/proto.py` & `sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/proto.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/straintensor.py` & `sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/straintensor.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/surface/kirchhoffplate.py` & `sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/surface/kirchhoffplate.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/surface/kirchhoffshell.py` & `sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/surface/kirchhoffshell.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/surface/membrane.py` & `sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/surface/membrane.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/surface/mindlinplate.py` & `sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/surface/mindlinplate.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/surface/mindlinshell.py` & `sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/surface/mindlinshell.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/surface/surface.py` & `sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/surface/surface.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/tensor2x3.py` & `sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/tensor2x3.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/utils/bernoulli.py` & `sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/utils/bernoulli.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/utils/hmh.py` & `sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/utils/hmh.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from numba import njit, vectorize, guvectorize, prange, float64
 
 from ..config import __has_cupy__, __has_numba_cuda__
 
 __cache = True
 
 
+
 @njit(nogil=True, cache=__cache)
 def HMH_M(strs: ndarray) -> float:
     """
     Evaluates the Huber-Mises-Hencky formula for membranes at a single point.
 
     Example
     -------
```

### Comparing `sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/utils/hoffman.py` & `sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/utils/hoffman.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/utils/imap.py` & `sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/utils/imap.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/utils/material.py` & `sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/utils/material.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/utils/mindlin.py` & `sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/utils/mindlin.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/utils/postproc.py` & `sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/utils/postproc.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/utils/principal.py` & `sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/utils/principal.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/utils/surface.py` & `sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/utils/surface.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/utils/symbolic.py` & `sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/utils/symbolic.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/utils/tr.py` & `sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/utils/tr.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon_solid_material-1.0.0/src/sigmaepsilon/solid/material/utils/utils.py` & `sigmaepsilon_solid_material-1.0.1/src/sigmaepsilon/solid/material/utils/utils.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon_solid_material-1.0.0/PKG-INFO` & `sigmaepsilon_solid_material-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigmaepsilon.solid.material
-Version: 1.0.0
+Version: 1.0.1
 Summary: Material models for solid structures in Python.
 Home-page: https://github.com/sigma-epsilon/sigmaepsilon.solid.material
 License: MIT
 Keywords: engineering,mechanics,solid mechanics,Python,numerical methods,material models,material properties,material testing,material characterization,material science
 Author: Bence Balogh
 Author-email: bencebalogh@sigmaepsilon.com
 Maintainer: Bence Balogh
```

