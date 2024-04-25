# Comparing `tmp/ikpls-1.2.0.post2.tar.gz` & `tmp/ikpls-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ikpls-1.2.0.post2.tar", max compression
+gzip compressed data, was "ikpls-1.2.1.tar", max compression
```

## Comparing `ikpls-1.2.0.post2.tar` & `ikpls-1.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11433 2024-04-24 00:21:01.861739 ikpls-1.2.0.post2/LICENSE
--rw-r--r--   0        0        0     7674 2024-04-24 00:21:01.861739 ikpls-1.2.0.post2/README.md
--rw-r--r--   0        0        0       28 2024-04-24 00:21:01.865739 ikpls-1.2.0.post2/ikpls/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 00:21:01.865739 ikpls-1.2.0.post2/ikpls/fast_cross_validation/__init__.py
--rw-r--r--   0        0        0    23705 2024-04-24 00:21:01.865739 ikpls-1.2.0.post2/ikpls/fast_cross_validation/numpy_ikpls.py
--rw-r--r--   0        0        0    15583 2024-04-24 00:21:01.865739 ikpls-1.2.0.post2/ikpls/jax_ikpls_alg_1.py
--rw-r--r--   0        0        0    13495 2024-04-24 00:21:01.865739 ikpls-1.2.0.post2/ikpls/jax_ikpls_alg_2.py
--rw-r--r--   0        0        0    41664 2024-04-24 00:21:01.865739 ikpls-1.2.0.post2/ikpls/jax_ikpls_base.py
--rw-r--r--   0        0        0    10170 2024-04-24 00:21:01.865739 ikpls-1.2.0.post2/ikpls/numpy_ikpls.py
--rw-r--r--   0        0        0      558 2024-04-24 00:21:01.869739 ikpls-1.2.0.post2/pyproject.toml
--rw-r--r--   0        0        0     8602 1970-01-01 00:00:00.000000 ikpls-1.2.0.post2/PKG-INFO
+-rw-r--r--   0        0        0    11433 2024-04-24 17:27:10.449547 ikpls-1.2.1/LICENSE
+-rw-r--r--   0        0        0     7664 2024-04-24 17:27:10.449547 ikpls-1.2.1/README.md
+-rw-r--r--   0        0        0       22 2024-04-24 17:27:10.449547 ikpls-1.2.1/ikpls/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 17:27:10.449547 ikpls-1.2.1/ikpls/fast_cross_validation/__init__.py
+-rw-r--r--   0        0        0    24042 2024-04-24 17:27:10.449547 ikpls-1.2.1/ikpls/fast_cross_validation/numpy_ikpls.py
+-rw-r--r--   0        0        0    15583 2024-04-24 17:27:10.449547 ikpls-1.2.1/ikpls/jax_ikpls_alg_1.py
+-rw-r--r--   0        0        0    13495 2024-04-24 17:27:10.453547 ikpls-1.2.1/ikpls/jax_ikpls_alg_2.py
+-rw-r--r--   0        0        0    41664 2024-04-24 17:27:10.453547 ikpls-1.2.1/ikpls/jax_ikpls_base.py
+-rw-r--r--   0        0        0    10170 2024-04-24 17:27:10.453547 ikpls-1.2.1/ikpls/numpy_ikpls.py
+-rw-r--r--   0        0        0      552 2024-04-24 17:27:10.453547 ikpls-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     8586 1970-01-01 00:00:00.000000 ikpls-1.2.1/PKG-INFO
```

### Comparing `ikpls-1.2.0.post2/LICENSE` & `ikpls-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ikpls-1.2.0.post2/README.md` & `ikpls-1.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -151,20 +151,21 @@
     JAX.](https://github.com/Sm00thix/IKPLS/tree/main/examples/gradient_jax.py)
 
 ## Contribute
 
 To contribute, please read the [Contribution
 Guidelines](https://github.com/Sm00thix/IKPLS/blob/main/CONTRIBUTING.md).
 
+(references)=
 ## References
 
 1. [Dayal, B. S., & MacGregor, J. F. (1997). Improved PLS algorithms. *Journal of Chemometrics*, 11(1), 73-85.](https://doi.org/10.1002/(SICI)1099-128X(199701)11:1%3C73::AID-CEM435%3E3.0.CO;2-%23?)
 2. [Alin, A. (2009). Comparison of PLS algorithms when the number of objects is much larger than the number of variables. *Statistical Papers*, 50, 711-720.](https://doi.org/10.1007/s00362-009-0251-7)
 3. [Andersson, M. (2009). A comparison of nine PLS1 algorithms. *Journal of Chemometrics*, 23(10), 518-529.](https://doi.org/10.1002/cem.1248)
 4. [NumPy](https://numpy.org/)
 5. [scikit-learn](https://scikit-learn.org/stable/)
 6. [JAX](https://jax.readthedocs.io/en/latest/)
 7. [Engstrøm, O.-C. G. (2024). Shortcutting Cross-Validation:
     Efficiently Deriving Column-Wise Centered and Scaled Training Set
-    \$\\\\mathbf{X}\^\\\\mathbf{T}\\\\mathbf{X}\$ and
-    \$\\\\mathbf{X}\^\\\\mathbf{T}\\\\mathbf{Y}\$ Without Full
+    $\mathbf{X}^\mathbf{T}\mathbf{X}$ and
+    $\mathbf{X}^\mathbf{T}\mathbf{Y}$ Without Full
     Recomputation of Matrix Products or Statistical Moments](https://arxiv.org/abs/2401.13185)
```

### Comparing `ikpls-1.2.0.post2/ikpls/fast_cross_validation/numpy_ikpls.py` & `ikpls-1.2.1/ikpls/fast_cross_validation/numpy_ikpls.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 cross-validation process using joblib.
 
 Author: Ole-Christian Galbo Engstrøm
 E-mail: ole.e@di.ku.dk
 """
 
 import warnings
-from collections import defaultdict
 from typing import Any, Callable, Hashable, Iterable, Union
 
 import joblib
 import numpy as np
 import numpy.linalg as la
 import numpy.typing as npt
 from joblib import Parallel, delayed
@@ -484,47 +483,52 @@
             training_X_mean,
             training_Y_mean,
             training_X_std,
             training_Y_std,
         )
         return metric_function(self.Y[validation_indices], Y_pred)
 
-    def _generate_validation_indices_list(
+    def _generate_validation_indices_dict(
         self, cv_splits: Iterable[Hashable]
-    ) -> list[npt.NDArray[np.int_]]:
+    ) -> dict[Hashable, npt.NDArray[np.int_]]:
         """
         Generates a list of validation indices for each fold in `cv_splits`.
 
         Parameters
         ----------
         cv_splits : Iterable of Hashable with N elements
             An iterable defining cross-validation splits. Each unique value in
             `cv_splits` corresponds to a different fold.
 
         Returns
         -------
-        validation_indices_list : list of array of int
-            A list of validation indices for each fold.
+        index_dict : dict of Hashable to Array
+            A dictionary mapping each unique value in `cv_splits` to an array of
+            validation indices.
         """
-        index_dict = defaultdict(list)
+        index_dict = {}
         for i, num in enumerate(cv_splits):
-            index_dict[num].append(i)
-        validation_indices_list = list(index_dict.values())
-        return [np.asarray(indices) for indices in validation_indices_list]
+            try:
+                index_dict[num].append(i)
+            except:
+                index_dict[num] = [i]
+        for key in index_dict:
+            index_dict[key] = np.asarray(index_dict[key], dtype=int)
+        return index_dict
 
     def cross_validate(
         self,
         X: npt.ArrayLike,
         Y: npt.ArrayLike,
         A: int,
         cv_splits: Iterable[Hashable],
         metric_function: Callable[[npt.ArrayLike, npt.ArrayLike], Any],
         n_jobs=-1,
         verbose=10,
-    ) -> list[Any]:
+    ) -> dict[Hashable, Any]:
         """
         Cross-validates the PLS model using `cv_splits` splits on `X` and `Y` with
         `n_components` components evaluating results with `metric_function`.
 
         Parameters
         ----------
         X : Array of shape (N, K)
@@ -556,32 +560,35 @@
             available cores and the number of unique values in `cv_splits`.
 
         verbose : int, optional default=10
             Controls verbosity of parallel jobs.
 
         Returns
         -------
-        metrics : list of Any
-            A list of the results of evaluating `metric_function` on each fold.
+        metrics : dict of Hashable to Any
+            A dictionary mapping each unique value in `cv_splits` to the result of
+            evaluating `metric_function` on the validation set corresponding to that
+            value.
 
         Notes:
         ------
         The order of cross-validation folds is determined by the order of the unique
-        values in `cv_splits`. `metrics` will be sorted in the same order.
+        values in `cv_splits`. The keys and values of `metrics` will be sorted in the
+        same order.
         """
 
         self.X = np.asarray(X, dtype=self.dtype)
         self.Y = np.asarray(Y, dtype=self.dtype)
         if self.Y.ndim == 1:
             self.Y = self.Y.reshape(-1, 1)
         self.A = A
         self.N, self.K = X.shape
         self.M = self.Y.shape[1]
-        validation_indices_list = self._generate_validation_indices_list(cv_splits)
-        num_splits = len(validation_indices_list)
+        validation_indices_dict = self._generate_validation_indices_dict(cv_splits)
+        num_splits = len(validation_indices_dict)
 
         if self.algorithm == 1:
             self.all_indices = np.arange(self.N, dtype=int)
 
         if n_jobs == -1:
             n_jobs = min(joblib.cpu_count(), num_splits)
 
@@ -622,13 +629,15 @@
                    metric_function: Callable[[npt.ArrayLike, npt.ArrayLike], Any]
                    ) -> Any:
             return self._stateless_fit_predict_eval(
                     validation_indices,
                     metric_function
                    )
 
-        metrics = Parallel(n_jobs=n_jobs, verbose=verbose)(
+        metrics_list = Parallel(n_jobs=n_jobs, verbose=verbose)(
             delayed(worker)(validation_indices, metric_function)
-            for validation_indices in validation_indices_list
+            for validation_indices in validation_indices_dict.values()
         )
 
-        return metrics
+        metrics_dict = dict(zip(validation_indices_dict.keys(), metrics_list))
+ 
+        return metrics_dict
```

### Comparing `ikpls-1.2.0.post2/ikpls/jax_ikpls_alg_1.py` & `ikpls-1.2.1/ikpls/jax_ikpls_alg_1.py`

 * *Files identical despite different names*

### Comparing `ikpls-1.2.0.post2/ikpls/jax_ikpls_alg_2.py` & `ikpls-1.2.1/ikpls/jax_ikpls_alg_2.py`

 * *Files identical despite different names*

### Comparing `ikpls-1.2.0.post2/ikpls/jax_ikpls_base.py` & `ikpls-1.2.1/ikpls/jax_ikpls_base.py`

 * *Files identical despite different names*

### Comparing `ikpls-1.2.0.post2/ikpls/numpy_ikpls.py` & `ikpls-1.2.1/ikpls/numpy_ikpls.py`

 * *Files identical despite different names*

### Comparing `ikpls-1.2.0.post2/pyproject.toml` & `ikpls-1.2.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ikpls"
-version = "1.2.0.post2"
+version = "1.2.1"
 description = ""
 authors = ["Sm00thix <oleemail@icloud.com>"]
 maintainers = ["Sm00thix <oleemail@icloud.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://ikpls.readthedocs.io/en/latest/"
 repository = "https://github.com/Sm00thix/IKPLS"
```

### Comparing `ikpls-1.2.0.post2/PKG-INFO` & `ikpls-1.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ikpls
-Version: 1.2.0.post2
+Version: 1.2.1
 Summary: 
 Home-page: https://ikpls.readthedocs.io/en/latest/
 License: Apache-2.0
 Author: Sm00thix
 Author-email: oleemail@icloud.com
 Maintainer: Sm00thix
 Maintainer-email: oleemail@icloud.com
@@ -177,20 +177,21 @@
     JAX.](https://github.com/Sm00thix/IKPLS/tree/main/examples/gradient_jax.py)
 
 ## Contribute
 
 To contribute, please read the [Contribution
 Guidelines](https://github.com/Sm00thix/IKPLS/blob/main/CONTRIBUTING.md).
 
+(references)=
 ## References
 
 1. [Dayal, B. S., & MacGregor, J. F. (1997). Improved PLS algorithms. *Journal of Chemometrics*, 11(1), 73-85.](https://doi.org/10.1002/(SICI)1099-128X(199701)11:1%3C73::AID-CEM435%3E3.0.CO;2-%23?)
 2. [Alin, A. (2009). Comparison of PLS algorithms when the number of objects is much larger than the number of variables. *Statistical Papers*, 50, 711-720.](https://doi.org/10.1007/s00362-009-0251-7)
 3. [Andersson, M. (2009). A comparison of nine PLS1 algorithms. *Journal of Chemometrics*, 23(10), 518-529.](https://doi.org/10.1002/cem.1248)
 4. [NumPy](https://numpy.org/)
 5. [scikit-learn](https://scikit-learn.org/stable/)
 6. [JAX](https://jax.readthedocs.io/en/latest/)
 7. [Engstrøm, O.-C. G. (2024). Shortcutting Cross-Validation:
     Efficiently Deriving Column-Wise Centered and Scaled Training Set
-    \$\\\\mathbf{X}\^\\\\mathbf{T}\\\\mathbf{X}\$ and
-    \$\\\\mathbf{X}\^\\\\mathbf{T}\\\\mathbf{Y}\$ Without Full
+    $\mathbf{X}^\mathbf{T}\mathbf{X}$ and
+    $\mathbf{X}^\mathbf{T}\mathbf{Y}$ Without Full
     Recomputation of Matrix Products or Statistical Moments](https://arxiv.org/abs/2401.13185)
```

