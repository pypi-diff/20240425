# Comparing `tmp/antakia_core-0.4.2.tar.gz` & `tmp/antakia_core-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antakia_core-0.4.2.tar", max compression
+gzip compressed data, was "antakia_core-0.4.3.tar", max compression
```

## Comparing `antakia_core-0.4.2.tar` & `antakia_core-0.4.3.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0     1497 2024-03-19 14:18:22.609303 antakia_core-0.4.2/LICENSE
--rw-r--r--   0        0        0       54 2024-03-19 14:18:22.609385 antakia_core-0.4.2/README.md
--rw-r--r--   0        0        0      667 2024-04-23 12:45:18.968154 antakia_core-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      110 2024-03-19 14:18:22.610283 antakia_core-0.4.2/src/antakia_core/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 14:18:22.610377 antakia_core-0.4.2/src/antakia_core/compute/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 14:18:22.610480 antakia_core-0.4.2/src/antakia_core/compute/dim_reduction/__init__.py
--rw-r--r--   0        0        0     5731 2024-04-23 10:15:03.843273 antakia_core-0.4.2/src/antakia_core/compute/dim_reduction/dim_reduc_method.py
--rw-r--r--   0        0        0     7598 2024-04-23 10:17:30.940235 antakia_core-0.4.2/src/antakia_core/compute/dim_reduction/dim_reduction.py
--rw-r--r--   0        0        0       75 2024-03-22 17:21:14.615326 antakia_core-0.4.2/src/antakia_core/compute/dim_reduction/pacmap_progress/__init__.py
--rw-r--r--   0        0        0    40149 2024-03-22 17:21:15.061170 antakia_core-0.4.2/src/antakia_core/compute/dim_reduction/pacmap_progress/pacmap_progress.py
--rw-r--r--   0        0        0        0 2024-03-19 14:18:22.610898 antakia_core-0.4.2/src/antakia_core/compute/model_subtitution/__init__.py
--rw-r--r--   0        0        0      840 2024-03-21 16:04:55.999992 antakia_core-0.4.2/src/antakia_core/compute/model_subtitution/classification_models.py
--rw-r--r--   0        0        0     3733 2024-04-23 09:45:08.540154 antakia_core-0.4.2/src/antakia_core/compute/model_subtitution/model_class.py
--rw-r--r--   0        0        0     7402 2024-04-23 09:45:08.540523 antakia_core-0.4.2/src/antakia_core/compute/model_subtitution/model_interface.py
--rw-r--r--   0        0        0     1842 2024-03-19 14:18:22.611366 antakia_core-0.4.2/src/antakia_core/compute/model_subtitution/regression_models.py
--rw-r--r--   0        0        0     1786 2024-04-23 09:45:08.540983 antakia_core-0.4.2/src/antakia_core/compute/skope_rule/skope_rule.py
--rw-r--r--   0        0        0      192 2024-03-19 14:18:22.611682 antakia_core-0.4.2/src/antakia_core/data_handler/__init__.py
--rw-r--r--   0        0        0     3968 2024-04-23 10:15:03.844379 antakia_core-0.4.2/src/antakia_core/data_handler/projected_values.py
--rw-r--r--   0        0        0       98 2024-03-19 14:18:22.611895 antakia_core-0.4.2/src/antakia_core/data_handler/region.py
--rw-r--r--   0        0        0     8700 2024-04-23 10:23:06.051162 antakia_core-0.4.2/src/antakia_core/data_handler/region_.py
--rw-r--r--   0        0        0    10471 2024-03-19 15:16:36.155976 antakia_core-0.4.2/src/antakia_core/data_handler/region_set.py
--rw-r--r--   0        0        0     9434 2024-04-23 09:45:08.541305 antakia_core-0.4.2/src/antakia_core/data_handler/rule.py
--rw-r--r--   0        0        0     4176 2024-03-22 13:24:54.198488 antakia_core-0.4.2/src/antakia_core/data_handler/rules.py
--rw-r--r--   0        0        0      190 2024-03-19 14:18:22.612650 antakia_core-0.4.2/src/antakia_core/explanation/__init__.py
--rw-r--r--   0        0        0     2129 2024-03-29 12:59:56.497027 antakia_core-0.4.2/src/antakia_core/explanation/explanation_method.py
--rw-r--r--   0        0        0     4778 2024-04-23 09:45:08.541634 antakia_core-0.4.2/src/antakia_core/explanation/explanations.py
--rw-r--r--   0        0        0      307 2024-03-19 14:18:22.612977 antakia_core-0.4.2/src/antakia_core/utils/__init__.py
--rw-r--r--   0        0        0     1302 2024-03-29 13:06:13.987832 antakia_core-0.4.2/src/antakia_core/utils/long_task.py
--rw-r--r--   0        0        0      548 2024-04-23 10:15:03.844754 antakia_core-0.4.2/src/antakia_core/utils/splittable_callback.py
--rw-r--r--   0        0        0     4576 2024-04-23 09:45:08.541955 antakia_core-0.4.2/src/antakia_core/utils/utils.py
--rw-r--r--   0        0        0    12510 2024-04-23 09:45:08.542559 antakia_core-0.4.2/src/antakia_core/utils/variable.py
--rw-r--r--   0        0        0      832 1970-01-01 00:00:00.000000 antakia_core-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1497 2024-03-19 14:18:22.609303 antakia_core-0.4.3/LICENSE
+-rw-r--r--   0        0        0       54 2024-03-19 14:18:22.609385 antakia_core-0.4.3/README.md
+-rw-r--r--   0        0        0      758 2024-04-25 14:13:58.088096 antakia_core-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0      110 2024-03-19 14:18:22.610283 antakia_core-0.4.3/src/antakia_core/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 14:18:22.610377 antakia_core-0.4.3/src/antakia_core/compute/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 14:18:22.610480 antakia_core-0.4.3/src/antakia_core/compute/dim_reduction/__init__.py
+-rw-r--r--   0        0        0     7261 2024-04-23 14:56:02.573651 antakia_core-0.4.3/src/antakia_core/compute/dim_reduction/dim_reduc_method.py
+-rw-r--r--   0        0        0     7926 2024-04-25 14:03:01.843934 antakia_core-0.4.3/src/antakia_core/compute/dim_reduction/dim_reduction.py
+-rw-r--r--   0        0        0       75 2024-03-22 17:21:14.615326 antakia_core-0.4.3/src/antakia_core/compute/dim_reduction/pacmap_progress/__init__.py
+-rw-r--r--   0        0        0    40149 2024-03-22 17:21:15.061170 antakia_core-0.4.3/src/antakia_core/compute/dim_reduction/pacmap_progress/pacmap_progress.py
+-rw-r--r--   0        0        0        0 2024-03-19 14:18:22.610898 antakia_core-0.4.3/src/antakia_core/compute/model_subtitution/__init__.py
+-rw-r--r--   0        0        0      840 2024-03-21 16:04:55.999992 antakia_core-0.4.3/src/antakia_core/compute/model_subtitution/classification_models.py
+-rw-r--r--   0        0        0     3733 2024-04-23 14:51:04.769035 antakia_core-0.4.3/src/antakia_core/compute/model_subtitution/model_class.py
+-rw-r--r--   0        0        0     8139 2024-04-23 14:51:04.885872 antakia_core-0.4.3/src/antakia_core/compute/model_subtitution/model_interface.py
+-rw-r--r--   0        0        0     1842 2024-03-19 14:18:22.611366 antakia_core-0.4.3/src/antakia_core/compute/model_subtitution/regression_models.py
+-rw-r--r--   0        0        0     1785 2024-04-23 14:50:36.703592 antakia_core-0.4.3/src/antakia_core/compute/skope_rule/skope_rule.py
+-rw-r--r--   0        0        0      192 2024-03-19 14:18:22.611682 antakia_core-0.4.3/src/antakia_core/data_handler/__init__.py
+-rw-r--r--   0        0        0     3969 2024-04-23 14:51:04.148770 antakia_core-0.4.3/src/antakia_core/data_handler/projected_values.py
+-rw-r--r--   0        0        0       98 2024-03-19 14:18:22.611895 antakia_core-0.4.3/src/antakia_core/data_handler/region.py
+-rw-r--r--   0        0        0     9794 2024-04-25 14:05:57.905202 antakia_core-0.4.3/src/antakia_core/data_handler/region_.py
+-rw-r--r--   0        0        0    10674 2024-04-23 14:50:36.705105 antakia_core-0.4.3/src/antakia_core/data_handler/region_set.py
+-rw-r--r--   0        0        0    10089 2024-04-23 14:50:36.705350 antakia_core-0.4.3/src/antakia_core/data_handler/rule.py
+-rw-r--r--   0        0        0     4434 2024-04-23 14:50:36.706070 antakia_core-0.4.3/src/antakia_core/data_handler/rules.py
+-rw-r--r--   0        0        0      190 2024-03-19 14:18:22.612650 antakia_core-0.4.3/src/antakia_core/explanation/__init__.py
+-rw-r--r--   0        0        0     2129 2024-03-29 12:59:56.497027 antakia_core-0.4.3/src/antakia_core/explanation/explanation_method.py
+-rw-r--r--   0        0        0     4778 2024-04-23 09:45:08.541634 antakia_core-0.4.3/src/antakia_core/explanation/explanations.py
+-rw-r--r--   0        0        0      307 2024-03-19 14:18:22.612977 antakia_core-0.4.3/src/antakia_core/utils/__init__.py
+-rw-r--r--   0        0        0     2031 2024-04-23 14:51:04.685563 antakia_core-0.4.3/src/antakia_core/utils/correlation_coef.py
+-rw-r--r--   0        0        0     1302 2024-03-29 13:06:13.987832 antakia_core-0.4.3/src/antakia_core/utils/long_task.py
+-rw-r--r--   0        0        0      561 2024-04-23 14:51:04.692721 antakia_core-0.4.3/src/antakia_core/utils/splittable_callback.py
+-rw-r--r--   0        0        0     4576 2024-04-23 09:45:08.541955 antakia_core-0.4.3/src/antakia_core/utils/utils.py
+-rw-r--r--   0        0        0    12510 2024-04-23 09:45:08.542559 antakia_core-0.4.3/src/antakia_core/utils/variable.py
+-rw-r--r--   0        0        0      939 1970-01-01 00:00:00.000000 antakia_core-0.4.3/PKG-INFO
```

### Comparing `antakia_core-0.4.2/LICENSE` & `antakia_core-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `antakia_core-0.4.2/pyproject.toml` & `antakia_core-0.4.3/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 [tool.poetry]
 name = "antakia-core"
-version = "0.4.2"
+version = "0.4.3"
 description = "Core modules for AntakIA"
 authors = ["Pierre Hulot <pierre@ai-vidence.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
 pandas = "^2.2.0"
 scikit-learn = "^1.4.1.post1"
 pacmap = "*"
-openTSNE = "*"
 interpret = "*"
-pygam = "*"
 lime = "^0.2.0.1"
 shap = "^0.43.0"
 umap-learn = "^0.5.5"
-skope-rules-temp = "*"
+skope-rules-temp = ">=0.2.4"
 scipy = "*"
+pygam = [
+    { version = ">=0.9.0", python = ">=3.11,<3.13" },
+    { version = "<0.9.0", python = "<3.11" }
+]
+
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.6.2"
 mkdocs = "^1.5.3"
 mock = "^5.1.0"
 pytest = "^8.0.1"
 pytest-cov = "^4.1.0"
```

### Comparing `antakia_core-0.4.2/src/antakia_core/compute/dim_reduction/dim_reduction.py` & `antakia_core-0.4.3/src/antakia_core/compute/dim_reduction/dim_reduction.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from .pacmap_progress import PaCMAP
 import pandas as pd
 from sklearn.decomposition import PCA
-from openTSNE import TSNE
+#from openTSNE import TSNE
 
 from antakia_core.compute.dim_reduction.dim_reduc_method import DimReducMethod
 from ...utils.splittable_callback import ProgressCallback
 
 # ===========================================================
 #         Projections / Dim Reductions implementations
 # ===========================================================
 
 
 class PCADimReduc(DimReducMethod):
     """
     PCA computation class.
     """
-    dimreduc_method = DimReducMethod.dimreduc_method_as_int('PCA')
+    dimreduc_method: int = DimReducMethod.dimreduc_method_as_int(
+        'PCA')  # type: ignore
     allowed_kwargs = [
         'copy', 'whiten', 'svd_solver', 'tol', 'iterated_power',
         'n_oversamples', 'power_iteration_normalizer', 'random_state'
     ]
 
     def __init__(self,
                  X: pd.DataFrame,
@@ -31,68 +32,68 @@
                          X,
                          progress_callback=progress_callback,
                          default_parameters={
                              'n_components': dimension,
                          })
 
 
-class TSNEwrapper(TSNE):
-
-    def fit_transform(self, X):
-        return pd.DataFrame(self.fit(X.values), index=X.index)
-
-
-class TSNEDimReduc(DimReducMethod):
-    """
-    T-SNE computation class.
-    """
-    dimreduc_method = -1  # DimReducMethod.dimreduc_method_as_int('TSNE')
-    allowed_kwargs = [
-        'perplexity', 'early_exaggeration', 'learning_rate', 'n_iter',
-        'n_iter_without_progress', 'min_grad_norm', 'metric', 'metric_params',
-        'init', 'verbose', 'random_state', 'method', 'angle', 'n_jobs'
-    ]
-
-    def __init__(self,
-                 X: pd.DataFrame,
-                 dimension: int = 2,
-                 progress_callback: ProgressCallback | None = None):
-        super().__init__(self.dimreduc_method,
-                         TSNEwrapper,
-                         dimension,
-                         X,
-                         progress_callback=progress_callback,
-                         default_parameters={
-                             'n_components': dimension,
-                             'n_jobs': -1
-                         })
-
-    @classmethod
-    def parameters(cls) -> dict:
-        return {
-            'perplexity': {
-                'type': float,
-                'min': 5,
-                'max': 50,
-                'default': 12
-            },
-            'learning_rate': {
-                'type': [float, str],
-                'min': 10,
-                'max': 1000,
-                'default': 'auto'
-            }
-        }
+# class TSNEwrapper(TSNE):
+#
+#     def fit_transform(self, X):
+#         return pd.DataFrame(self.fit(X.values), index=X.index)
+
+# class TSNEDimReduc(DimReducMethod):
+#     """
+#     T-SNE computation class.
+#     """
+#     dimreduc_method = -1  # DimReducMethod.dimreduc_method_as_int('TSNE')
+#     allowed_kwargs = [
+#         'perplexity', 'early_exaggeration', 'learning_rate', 'n_iter',
+#         'n_iter_without_progress', 'min_grad_norm', 'metric', 'metric_params',
+#         'init', 'verbose', 'random_state', 'method', 'angle', 'n_jobs'
+#     ]
+#
+#     def __init__(self,
+#                  X: pd.DataFrame,
+#                  dimension: int = 2,
+#                  progress_callback: ProgressCallback | None = None):
+#         super().__init__(self.dimreduc_method,
+#                          TSNEwrapper,
+#                          dimension,
+#                          X,
+#                          progress_callback=progress_callback,
+#                          default_parameters={
+#                              'n_components': dimension,
+#                              'n_jobs': -1
+#                          })
+#
+#     @classmethod
+#     def parameters(cls) -> dict:
+#         return {
+#             'perplexity': {
+#                 'type': float,
+#                 'min': 5,
+#                 'max': 50,
+#                 'default': 12
+#             },
+#             'learning_rate': {
+#                 'type': [float, str],
+#                 'min': 10,
+#                 'max': 1000,
+#                 'default': 'auto'
+#             }
+#         }
 
 
 class UMAPDimReduc(DimReducMethod):
     """
     UMAP computation class.
     """
-    dimreduc_method = DimReducMethod.dimreduc_method_as_int('UMAP')
+    dimreduc_method: int = DimReducMethod.dimreduc_method_as_int(
+        'UMAP')  # type: ignore
     allowed_kwargs = [
         'n_neighbors',
         'metric',
         'metric_kwds',
         'output_metric',
         'output_metric_kwds',
         'n_epochs',
@@ -164,15 +165,16 @@
 
 
 class PaCMAPDimReduc(DimReducMethod):
     """
     PaCMAP computation class.
 
     """
-    dimreduc_method = DimReducMethod.dimreduc_method_as_int('PaCMAP')
+    dimreduc_method: int = DimReducMethod.dimreduc_method_as_int(
+        'PaCMAP')  # type: ignore
     allowed_kwargs = [
         'n_neighbors', 'MN_ratio', 'FP_ratio', 'pair_neighbors', 'pair_MN',
         'pair_FP', 'distance', 'lr', 'num_iters', 'apply_pca', 'intermediate',
         'intermediate_snapshots', 'random_state'
     ]
     has_progress_callback = True
 
@@ -214,35 +216,42 @@
                 'scale': 'log'
             }
         }
 
 
 dim_reduc_factory: dict[int, type[DimReducMethod]] = {
     dm.dimreduc_method: dm
-    for dm in [PCADimReduc, TSNEDimReduc, UMAPDimReduc, PaCMAPDimReduc]
+    for dm in [
+        PCADimReduc,
+        # TSNEDimReduc,
+        UMAPDimReduc,
+        PaCMAPDimReduc
+    ]
 }
 
 
 def compute_projection(X: pd.DataFrame,
                        y: pd.Series,
                        dimreduc_method: int,
                        dimension: int,
                        progress_callback: ProgressCallback | None = None,
+                       fit_sample_num=None,
                        **kwargs) -> pd.DataFrame:
     dim_reduc = dim_reduc_factory.get(dimreduc_method)
 
     if dim_reduc is None or not DimReducMethod.is_valid_dim_number(dimension):
         raise ValueError("Cannot compute proj method #", dimreduc_method,
                          " in ", dimension, " dimensions")
 
-    default_kwargs = {'random_state': 9}
+    default_kwargs = {'random_state': 9, 'fit_sample_num': fit_sample_num}
     default_kwargs.update(kwargs)
     dim_reduc_kwargs = {
         k: v
-        for k, v in default_kwargs.items() if k in dim_reduc.allowed_kwargs
+        for k, v in default_kwargs.items()
+        if k in dim_reduc.allowed_kwargs or k == 'fit_sample_num'
     }
     proj_values = pd.DataFrame(
         dim_reduc(  # type:ignore
             X,  # type:ignore
             dimension,  # type:ignore
             progress_callback).compute(  # type:ignore
                 **dim_reduc_kwargs).values,  # type:ignore
```

### Comparing `antakia_core-0.4.2/src/antakia_core/compute/dim_reduction/pacmap_progress/pacmap_progress.py` & `antakia_core-0.4.3/src/antakia_core/compute/dim_reduction/pacmap_progress/pacmap_progress.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.4.2/src/antakia_core/compute/model_subtitution/classification_models.py` & `antakia_core-0.4.3/src/antakia_core/compute/model_subtitution/classification_models.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.4.2/src/antakia_core/compute/model_subtitution/model_class.py` & `antakia_core-0.4.3/src/antakia_core/compute/model_subtitution/model_class.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.4.2/src/antakia_core/compute/model_subtitution/model_interface.py` & `antakia_core-0.4.3/src/antakia_core/compute/model_subtitution/model_interface.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 from antakia_core.compute.model_subtitution.classification_models import *
 from antakia_core.compute.model_subtitution.regression_models import *
 import re
 
 from antakia_core.utils.utils import ProblemCategory
 
 
-def pretty_model_name(model_name):
+def pretty_model_name(model_name: str) -> str:
     return model_name.replace('_', ' ').title()
 
 
-def reduce_name(model_name):
+def reduce_name(model_name: str) -> str:
     parts = re.split(r'\W+', model_name)
     name = ''
     for part in parts:
         name += part[0].upper()
         for char in part[1:]:
             if char.isupper():
                 name += char
@@ -67,20 +67,45 @@
             ]
         return [
             AvgClassificationBaselineModel, DecisionTreeClassifier,
             LogisticRegression
         ]
 
     def _init_models(self, task_type):
+        """
+        fills the empty dict with all available models
+        Parameters
+        ----------
+        task_type
+
+        Returns
+        -------
+
+        """
         for model_class in self._get_available_models(task_type):
             model = model_class()
             if model.name not in self.models:
                 self.models[pretty_model_name(model.name)] = model
 
     def _init_scores(self, customer_model, task_type, X_test, y_test):
+        """
+        fills the empty dict with score names as key, and tuple
+        (scoring function, score type) as value
+
+        Parameters
+        ----------
+        customer_model
+        task_type
+        X_test
+        y_test
+
+        Returns
+        -------
+
+        """
         if self.score_type == 'compute':
             self._compute_score_type(customer_model, X_test, y_test)
         if task_type == ProblemCategory.regression:
             scores_list = ['MSE', 'MAE', 'R2']
         else:
             scores_list = [
                 'ACC', 'F1', 'precision'.upper(), 'recall'.upper(), 'R2'
@@ -89,36 +114,52 @@
             score: self.available_scores[score]
             for score in scores_list
         }
         self.scores[self.custom_score_str] = (self.custom_score,
                                               self.score_type)
 
     def _train_models(self, X_train, y_train, X_test, y_test):
-        models = Parallel(n_jobs=-1)(delayed(model.fit_and_compute_fi)(
+        models = Parallel(n_jobs=1)(delayed(model.fit_and_compute_fi)(
             X_train, y_train, X_test, y_test, self.custom_score,
             self.score_type) for model_name, model in self.models.items()
-                                     if not model.fitted)
+                                    if not model.fitted)
 
         for model in models:
             self.models[pretty_model_name(model.name)] = model
 
     def _compute_score_type(self, customer_model, X: pd.DataFrame,
                             y: pd.Series):
         y_pred = customer_model.predict(X)
         s1 = self.custom_score(y_pred, y)
         s2 = self.custom_score(y.sample(len(y)).values, y.values)
         self.score_type = 'maximize' if s1 > s2 else 'minimize'
 
-    def get_models_performance(self,
-                               customer_model,
-                               X_train: pd.DataFrame,
-                               y_train: pd.Series,
-                               X_test: pd.DataFrame | None,
-                               y_test: pd.Series | None,
-                               task_type='regression') -> pd.DataFrame:
+    def get_models_performance(
+            self,
+            customer_model,  #fitted model
+            X_train: pd.DataFrame,
+            y_train: pd.Series,
+            X_test: pd.DataFrame | None,
+            y_test: pd.Series | None,
+            task_type='regression') -> pd.DataFrame:
+        """
+
+        Parameters
+        ----------
+        customer_model
+        X_train
+        y_train
+        X_test
+        y_test
+        task_type
+
+        Returns sorted perf dataframe
+        -------
+
+        """
         if isinstance(task_type, str):
             task_type = ProblemCategory[task_type]
         if len(X_train) <= 50 or len(X_train.T) >= len(X_train):
             return pd.DataFrame()
         if X_test is None or len(X_test) == 0:
             print('no test set provided, splitting train set')
             X_train, X_test, y_train, y_test = train_test_split(X_train,
@@ -145,18 +186,24 @@
 
         def get_delta_color(delta):
             return 'red' if delta > 0.01 else 'green' if delta < -0.01 else 'orange'
 
         self.perfs['delta_color'] = self.perfs['delta'].apply(get_delta_color)
         return self.perfs.sort_values('delta', ascending=True)
 
-    def select_model(self, model_name):
+    def select_model(self, model_name: str):
         self.selected_model = model_name
 
     def selected_model_str(self) -> str:
+        """
+
+        Returns a string representation of the selected model's name and his score
+        -------
+
+        """
         perf = self.perfs.loc[self.selected_model]
         reduced_name = reduce_name(self.selected_model)
         display_str = f'{reduced_name} - {self.custom_score_str}:{perf[self.custom_score_str]:.2f} ({perf["delta"]:.2f})'
         return display_str
 
     def reset(self):
         self.models = {}
```

### Comparing `antakia_core-0.4.2/src/antakia_core/compute/model_subtitution/regression_models.py` & `antakia_core-0.4.3/src/antakia_core/compute/model_subtitution/regression_models.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.4.2/src/antakia_core/compute/skope_rule/skope_rule.py` & `antakia_core-0.4.3/src/antakia_core/compute/skope_rule/skope_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,10 +42,9 @@
 
         sk_classifier.fit(base_space_df, y_train)
 
     if sk_classifier.rules_ != []:
         rules_list, score_dict = RuleSet.sk_rules_to_rule_set(
             sk_classifier.rules_, variables)
         return rules_list, score_dict
-
     else:
         return RuleSet(), {}
```

### Comparing `antakia_core-0.4.2/src/antakia_core/data_handler/projected_values.py` & `antakia_core-0.4.3/src/antakia_core/data_handler/projected_values.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         """
         if not self.is_present(projection):
             self.compute(projection, progress_callback)
         return self._projected_values[projection]
 
     def is_present(self, projection: Proj) -> bool:
         """
-        tests if the projection is already computed
+        checks if the projection is already computed
         Parameters
         ----------
         projection_method
         dimension
 
         Returns
         -------
```

### Comparing `antakia_core-0.4.2/src/antakia_core/data_handler/region_.py` & `antakia_core-0.4.3/src/antakia_core/data_handler/region_.py`

 * *Files 5% similar despite different names*

```diff
@@ -133,23 +133,47 @@
         Returns
         -------
 
         """
         self.validated = True
 
     def update_rule_set(self, rule_set: RuleSet):
+        """
+        overwrite the previous rule set and mask with the rule set given in parameter
+        and his matching mask
+        Parameters
+        ----------
+        rule_set
+
+        Returns
+        -------
+
+        """
         self.rules = rule_set
         self.mask = self.rules.get_matching_mask(self.X)
         self.validated = False
 
     def update_mask(self, mask: pd.Series):
+        """
+        Parameters : the replacement mask
+        ----------
+        replaces the mask of the region by the mask given in parameters
+        set the region's rule set to the empty rule set
+        """
         self.mask = mask
         self.rules = RuleSet()
 
-    def get_color_serie(self):
+    def get_color_serie(self) -> pd.Series:
+        """
+
+        Returns a pd Series containing the color of each data point in the
+        region
+        -------
+
+        """
         color = pd.Series([BASE_COLOR] * len(self.X), index=self.X.index)
         if self.color == BASE_COLOR:
             region_color = 'blue'
         else:
             region_color = self.color
         color[self.mask] = region_color
         return color
@@ -157,18 +181,18 @@
 
 class ModelRegion(Region):
     """
     supercharged Region with an explainable predictive model
     """
 
     def __init__(self,
-                 X,
-                 y,
-                 X_test,
-                 y_test,
+                 X: pd.DataFrame,
+                 y: pd.DataFrame,
+                 X_test: pd.DataFrame | None,
+                 y_test: pd.DataFrame | None,
                  customer_model,
                  rules: RuleSet | None = None,
                  mask: pd.Series | None = None,
                  color=None,
                  score=None,
                  num=-1):
         """
@@ -189,15 +213,15 @@
         self.y = y
         self.X_test = X_test
         self._test_mask = None
         self.y_test = y_test
         self.customer_model = customer_model
         self.interpretable_models = InterpretableModels(score)
 
-    def to_dict(self):
+    def to_dict(self) -> dict:
         """
         transform region to dict
         Returns
         -------
 
         """
         dict_form = super().to_dict()
@@ -290,23 +314,44 @@
                     return boolean_mask(self.X_test,
                                         self.mask.mean()).astype(bool)
                 knn = KNeighborsClassifier().fit(self.X, self.mask)
                 self._test_mask = pd.Series(knn.predict(self.X_test),
                                             index=self.X_test.index)
         return self._test_mask
 
-    def get_model(self, model_name):
+    def get_model(self, model_name: str):
+        """
+
+        Parameters
+        ----------
+        model_name
+
+        Returns the model object corresponding to the model_name parameter
+        -------
+
+        """
         return self.interpretable_models.models[model_name]
 
     def get_selected_model(self):
         if self.interpretable_models.selected_model is None:
             return None
         return self.get_model(self.interpretable_models.selected_model)
 
-    def predict(self, X):
+    def predict(self, X: pd.DataFrame) -> pd.Series:
+        """
+
+        Parameters X_train dataframe
+        ----------
+        X
+
+        Returns a pandas Series of NaN if no model is selected. Or a pandas Series of
+        predicted y values
+        -------
+
+        """
         mask = self.rules.get_matching_mask(X)
         model = self.get_selected_model()
         if model is not None:
             return model.predict(X[mask]).reindex(X.index)
         return pd.Series(index=X.index)
 
     def update_rule_set(self, rule_set: RuleSet):
```

### Comparing `antakia_core-0.4.2/src/antakia_core/data_handler/region_set.py` & `antakia_core-0.4.3/src/antakia_core/data_handler/region_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,16 @@
                                       boolean_mask(self.X, True),
                                       BASE_COLOR,
                                       num=Region.LEFT_OUT_NUM)
 
     def get_new_num(self) -> int:
         """
         get a new Region id
-        Returns
+        Returns 1 if region set empty
+        Returns the smallest integer not already taken as a Region id
         -------
 
         """
         if len(self.regions) == 0:
             return 1
         else:
             for i in range(1, len(self.regions) + 1):
@@ -224,28 +225,28 @@
         """
         for i in list(self.regions.keys()):
             if not self.regions[i].validated:
                 self.remove(i)
 
     def pop_last(self) -> Region | None:
         """
-        removes and return the last region
-        Returns
+        removes and return the last region if not validates.
+        Only returns the region if validates
         -------
 
         """
         if len(self.insert_order) > 0:
             num = self.insert_order[-1]
             region = self.get(num)
             if not self.regions[num].validated:
                 self.remove(num)
             return region
         return None
 
-    def sort(self, by, ascending=True):
+    def sort(self, by: str, ascending=True):
         """
         sort the region set by id, size, insert order
         Parameters
         ----------
         by : 'region_num'|'size'|'insert'
         ascending
 
@@ -254,15 +255,15 @@
 
         """
         if by == 'region_num':
             key = lambda x: x.num
         elif by == 'size':
             key = lambda x: x.num_points()
         elif by == 'insert':
-            key = lambda x: self.insert_order.index(x)
+            key = lambda x: self.insert_order.index(x.num)
         self.display_order.sort(key=key, reverse=not ascending)
 
     def stats(self) -> dict:
         """ Computes the number of distinct points in the regions and the coverage in %
         """
         union_mask = self.mask
         stats = {
@@ -271,15 +272,15 @@
             'coverage': round(100 * union_mask.mean()),
         }
         return stats
 
     def _compute_left_out_region(self):
         """
         compute the left out region
-        Returns
+        Returns the computed region
         -------
 
         """
         left_out_mask = ~self.mask
         self.left_out_region.update_mask(left_out_mask)
         return self.left_out_region
 
@@ -306,24 +307,24 @@
         self.X_test = X_test
         self.y_test = y_test
         self.model = model
         self.score = score
         self.left_out_region = self.upgrade_region_to_model_region(
             self.left_out_region)
 
-    def upgrade_region_to_model_region(self, region: Region):
+    def upgrade_region_to_model_region(self, region: Region) -> ModelRegion:
         """
         Upgrade the provided region to a model region
         Parameters
         ----------
         region
 
         Returns
         -------
-
+        model_region
         """
         model_region = ModelRegion(X=self.X,
                                    y=self.y,
                                    X_test=self.X_test,
                                    y_test=self.y_test,
                                    customer_model=self.model,
                                    score=self.score,
```

### Comparing `antakia_core-0.4.2/src/antakia_core/data_handler/rule.py` & `antakia_core-0.4.3/src/antakia_core/data_handler/rule.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,21 @@
 from antakia_core.utils.variable import Variable
 
 
 class Rule:
     """
     class to represent logical rule over a variable
     """
+    TRUTHY_RULE = -1
+    CATEGORICAL_RULE = 0
+    MAX_RULE = 1
+    MIN_RULE = 2
+    INTERVAL_RULE = 3
+    VALUE_RULE = 4
+    FALSY_RULE = 5
 
     def __init__(self,
                  variable: Variable,
                  min: float | None = None,
                  includes_min: bool | None = None,
                  max: float | None = None,
                  includes_max: bool | None = None,
@@ -43,51 +50,51 @@
             else:
                 self.max = max
                 self.includes_max = includes_max if includes_max else False
 
     def __eq__(self, other):
         if self.rule_type != other.rule_type or self.variable != other.variable:
             return False
-        if self.rule_type in (-1, 5):
+        if self.rule_type in (self.TRUTHY_RULE, self.FALSY_RULE):
             return True
-        if self.rule_type == 0:
+        if self.rule_type == self.CATEGORICAL_RULE:
             return len(self.cat_values.symmetric_difference(
                 other.cat_values)) == 0
-        if self.rule_type == 4:
+        if self.rule_type == self.VALUE_RULE:
             return self.min == other.min
-        if self.rule_type == 1:
+        if self.rule_type == self.MAX_RULE:
             return self.max == other.max and self.includes_max == other.includes_max
-        if self.rule_type == 2:
+        if self.rule_type == self.MIN_RULE:
             return self.min == other.min and self.includes_min == other.includes_min
         return (self.max == other.max
                 and self.includes_max == other.includes_max) and (
                     self.min == other.min
                     and self.includes_min == other.includes_min)
 
     def __repr__(self):
         if self.is_categorical_rule:
             txt = f"{self.variable.display_name} \u2208  \u27E6"
             txt += ', '.join(self.cat_values)
             txt += "\u27E7"
             return txt
-        if self.rule_type == -1:
+        if self.rule_type == self.TRUTHY_RULE:
             return f'{self.variable.display_name} - True'
-        if self.rule_type == 5:
+        if self.rule_type == self.FALSY_RULE:
             return f'{self.variable.display_name} - False'
-        if self.rule_type == 1:
-            # Rule type 1
+        if self.rule_type == self.MAX_RULE:
+            # Rule type 1 : max rule
             op = '\u2264' if self.includes_max else '<'
             txt = f"{self.variable.display_name} {op} {format_number(self.max)}"
             return txt
-        if self.rule_type == 2:
-            # Rule type 2
+        if self.rule_type == self.MIN_RULE:
+            # Rule type 2 : min rule
             op = '\u2265' if self.includes_min else '>'
             txt = f"{self.variable.display_name} {op} {format_number(self.min)}"
             return txt
-        if self.rule_type == 3:
+        if self.rule_type == self.INTERVAL_RULE:
             # Rule type 3 : the rule is of the form : variable included in [min, max] interval, or min < variable < max
             if os.environ.get("USE_INTERVALS_FOR_RULES"):
                 open_bracket = '\u27E6' if self.includes_min else '['
                 close_bracket = '\u27E7' if self.includes_min else ']'
                 txt = f"{self.variable.display_name} \u2208 {open_bracket} {format_number(self.min)},"
                 txt += f" {format_number(self.max)} {close_bracket}"  # element of
                 return txt
@@ -110,77 +117,72 @@
             2: x >(=) min
             3: min <(=) x <(=) max
             4: x = value
             5: Falsy rule
         """
         if self.is_categorical_rule:
             if self.cat_values:
-                return 0
+                return self.CATEGORICAL_RULE
             else:
-                return 5
+                return self.FALSY_RULE
         if self.min == -np.inf and self.max == np.inf:
-            return -1
+            return self.TRUTHY_RULE
         if self.min == -np.inf:
-            return 1
+            return self.MAX_RULE
         if self.max == np.inf:
-            return 2
+            return self.MIN_RULE
         if self.max > self.min:
-            return 3
+            return self.INTERVAL_RULE
         if self.max == self.min and self.includes_max and self.includes_min:
-            return 4
-        return 5
+            return self.VALUE_RULE
+        return self.FALSY_RULE
 
     @property
     def operator_max(self):
-        if self.rule_type == 4:
+        if self.rule_type == self.VALUE_RULE:
             return '__eq__'
         if self.includes_max:
             return '__le__'
         return '__lt__'
 
     @property
     def operator_min(self):
-        if self.rule_type == 4:
+        if self.rule_type == self.VALUE_RULE:
             return '__eq__'
         if self.includes_min:
             return '__ge__'
         return '__gt__'
 
     @property
     def is_categorical_rule(self):
         return self.categorical_rule
 
     def get_matching_mask(self, X: pd.DataFrame) -> pd.Series:
         col = X.loc[:, self.variable.column_name]
-        return self.get_series_matching_mask(col)
-
-    def get_series_matching_mask(self, x: pd.Series) -> pd.Series:
-        if self.rule_type == -1:
-            return boolean_mask(x, True)
-        if self.rule_type == 0:
-            return x.isin(self.cat_values)  # type:ignore
-        if self.rule_type == 4:
-            return x == self.min
-        if self.rule_type == 5:
-            return boolean_mask(x, False)
-        return getattr(x, self.operator_max)(self.max) & getattr(
-            x, self.operator_min)(self.min)
+        if self.rule_type == self.TRUTHY_RULE:
+            return boolean_mask(X, True)
+        if self.rule_type == self.CATEGORICAL_RULE:
+            return col.isin(self.cat_values)  # type:ignore
+        if self.rule_type == self.VALUE_RULE:
+            return col == self.min
+        if self.rule_type == self.FALSY_RULE:
+            return boolean_mask(X, False)
+        return getattr(col, self.operator_max)(self.max) & getattr(
+            col, self.operator_min)(self.min)
 
     def __call__(self, value: float | pd.DataFrame) -> bool | pd.Series:
         if isinstance(value, pd.DataFrame):
             return self.get_matching_mask(value)
-        if isinstance(value, pd.Series):
-            return self.get_series_matching_mask(value)
-        if self.rule_type == -1:
+        if self.rule_type == self.TRUTHY_RULE:
             return True
-        if self.rule_type == 0:
+        if self.rule_type == self.CATEGORICAL_RULE:
             return value in self.cat_values  # type:ignore
-        if self.rule_type == 4:
+        if self.rule_type == self.VALUE_RULE:
             return value == self.min
-        if self.rule_type == 5:
+        if self.rule_type == self.FALSY_RULE:
             return False
         return getattr(value, self.operator_max)(self.max) & getattr(
             value, self.operator_min)(self.min)
 
     def combine(self, rule: Rule):
         """
         builds a new combining current rule and argument rules (logical and)
@@ -236,30 +238,42 @@
                               rule.includes_max)  # type:ignore
         return Rule(self.variable, min_val, include_min, max_val, include_max)
 
     def __and__(self, other):
         return self.combine(other)
 
     def to_dict(self):
+        """
+
+        Returns a dictionnary of the rule's parameters
+        -------
+
+        """
         return {
             'Variable': self.variable.display_name,
-            'Unit': self.variable.unit,
+            # 'Unit': self.variable.unit,
             'Desc': self.variable.descr,
             'Critical': self.variable.critical,
             'Rule': self.__repr__()
         }
 
     def copy(self):
         return Rule(self.variable, self.min, self.includes_min, self.max,
                     self.includes_max, self.cat_values)
 
 
 class TruthyRule(Rule):
+    """
+    class to represent logical rule that is always True over a variable
+    """
 
     def __init__(self, var: Variable):
         super().__init__(var)
 
 
 class FalsyRule(Rule):
+    """
+    class to represent logical rule that is always False over a variable
+    """
 
     def __init__(self, var: Variable):
         super().__init__(var, min=5, max=4)
```

### Comparing `antakia_core-0.4.2/src/antakia_core/data_handler/rules.py` & `antakia_core-0.4.3/src/antakia_core/data_handler/rules.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         if rules:
             for rule in rules:
                 self.add(rule)
 
     def add(self, value: Rule):
         """
         add a new rule
-        combines it with the existing rule is variable already used
+        combines it with the existing rule if variable already used
         Parameters
         ----------
         value
 
         Returns
         -------
 
@@ -54,14 +54,20 @@
 
     def __repr__(self):
         if not self.rules:
             return ""
         return " and ".join([rule.__repr__() for rule in self.rules.values()])
 
     def to_dict(self):
+        """
+        return a list of dictionaries containing the parameters of each rule
+        Returns
+        -------
+
+        """
         if not self.rules:
             return []
         return [rule.to_dict() for rule in self.rules.values()]
 
     def copy(self):
         return RuleSet(self.rules.values())
 
@@ -95,15 +101,15 @@
         """
         masks = []
         if self.rules is not None:
             for rule in self.rules.values():
                 masks.append(rule.get_matching_mask(X))
         return masks
 
-    def get_matching_indexes(self, X):
+    def get_matching_indexes(self, X: pd.DataFrame) -> list:
         """
         get the list indexes of X validating the rule
         Parameters
         ----------
         X
 
         Returns
@@ -123,21 +129,25 @@
         variables
 
         Returns
         -------
 
         """
         rules_info = skrules[0]
+        ###### deprecated
         precision, recall, __ = rules_info[1]
         f1 = precision * recall * 2 / (precision + recall)
+        #precision = TP/(TP+FP)
+        #recall = TP/(TP+FN)
         score_dict = {
             "precision": round(precision, 3),
             "recall": round(recall, 3),
             "f1": round(f1, 3),
         }
+        ######
         rule_strings = rules_info[0].split(" and ")
 
         rule_list = RuleSet()
         for rule in rule_strings:
             rule_parts = rule.split(' ')
 
             variable = variables.get_var(rule_parts[0])
```

### Comparing `antakia_core-0.4.2/src/antakia_core/explanation/explanation_method.py` & `antakia_core-0.4.3/src/antakia_core/explanation/explanation_method.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.4.2/src/antakia_core/explanation/explanations.py` & `antakia_core-0.4.3/src/antakia_core/explanation/explanations.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.4.2/src/antakia_core/utils/long_task.py` & `antakia_core-0.4.3/src/antakia_core/utils/long_task.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.4.2/src/antakia_core/utils/splittable_callback.py` & `antakia_core-0.4.3/src/antakia_core/utils/splittable_callback.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,13 +10,13 @@
               value: float | list[float]) -> Sequence['ProgressCallback']:
         raise NotImplemented
 
 
 class DummyProgressCallback(ProgressCallback):
 
     def __call__(self, *args, **kwargs):
-        pass
+        self.progress = 0
 
     def split(self, value: float | list[float]) -> Sequence[ProgressCallback]:
         if isinstance(value, list):
             return [self for _ in value] + [self]
         return [self, self]
```

### Comparing `antakia_core-0.4.2/src/antakia_core/utils/utils.py` & `antakia_core-0.4.3/src/antakia_core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.4.2/src/antakia_core/utils/variable.py` & `antakia_core-0.4.3/src/antakia_core/utils/variable.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.4.2/PKG-INFO` & `antakia_core-0.4.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: antakia-core
-Version: 0.4.2
+Version: 0.4.3
 Summary: Core modules for AntakIA
 Author: Pierre Hulot
 Author-email: pierre@ai-vidence.com
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: interpret
 Requires-Dist: lime (>=0.2.0.1,<0.3.0.0)
-Requires-Dist: openTSNE
 Requires-Dist: pacmap
 Requires-Dist: pandas (>=2.2.0,<3.0.0)
-Requires-Dist: pygam
+Requires-Dist: pygam (<0.9.0) ; python_version < "3.11"
+Requires-Dist: pygam (>=0.9.0) ; python_version >= "3.11" and python_version < "3.13"
 Requires-Dist: scikit-learn (>=1.4.1.post1,<2.0.0)
 Requires-Dist: scipy
 Requires-Dist: shap (>=0.43.0,<0.44.0)
-Requires-Dist: skope-rules-temp
+Requires-Dist: skope-rules-temp (>=0.2.4)
 Requires-Dist: umap-learn (>=0.5.5,<0.6.0)
 Description-Content-Type: text/markdown
 
 This modules provides various key classes for AntakIA.
```

