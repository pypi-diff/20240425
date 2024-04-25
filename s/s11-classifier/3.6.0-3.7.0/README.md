# Comparing `tmp/s11-classifier-3.6.0.tar.gz` & `tmp/s11-classifier-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s11-classifier-3.6.0.tar", last modified: Tue Dec 19 10:53:25 2023, max compression
+gzip compressed data, was "s11-classifier-3.7.0.tar", last modified: Thu Apr 25 07:34:08 2024, max compression
```

## Comparing `s11-classifier-3.6.0.tar` & `s11-classifier-3.7.0.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-19 10:53:25.530349 s11-classifier-3.6.0/
--rw-r--r--   0 root         (0) root         (0)     2102 2023-12-19 10:53:25.530349 s11-classifier-3.6.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1035 2023-12-14 12:09:36.000000 s11-classifier-3.6.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-19 10:53:25.523349 s11-classifier-3.6.0/classifier/
--rw-rw-rw-   0 root         (0) root         (0)      224 2023-12-13 14:48:59.000000 s11-classifier-3.6.0/classifier/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9765 2023-12-13 14:48:59.000000 s11-classifier-3.6.0/classifier/accuracy.py
--rw-rw-rw-   0 root         (0) root         (0)     8410 2023-12-13 14:48:59.000000 s11-classifier-3.6.0/classifier/classify.py
--rw-rw-rw-   0 root         (0) root         (0)     4071 2023-12-13 14:48:59.000000 s11-classifier-3.6.0/classifier/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1711 2023-12-13 14:48:59.000000 s11-classifier-3.6.0/classifier/dataprep.py
--rw-rw-rw-   0 root         (0) root         (0)    14497 2023-12-13 14:48:59.000000 s11-classifier-3.6.0/classifier/models.py
--rw-rw-rw-   0 root         (0) root         (0)    11365 2023-12-13 14:48:59.000000 s11-classifier-3.6.0/classifier/predict.py
--rw-rw-rw-   0 root         (0) root         (0)    27970 2023-12-13 14:48:59.000000 s11-classifier-3.6.0/classifier/samples.py
--rw-rw-rw-   0 root         (0) root         (0)      624 2023-12-13 14:48:59.000000 s11-classifier-3.6.0/classifier/settings.py
--rw-rw-rw-   0 root         (0) root         (0)    11068 2023-12-13 14:48:59.000000 s11-classifier-3.6.0/classifier/timeseries.py
--rw-rw-rw-   0 root         (0) root         (0)    10405 2023-12-13 14:48:59.000000 s11-classifier-3.6.0/classifier/train.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-19 10:53:25.524349 s11-classifier-3.6.0/classifier/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-13 14:48:59.000000 s11-classifier-3.6.0/classifier/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20302 2023-12-13 14:48:59.000000 s11-classifier-3.6.0/classifier/utils/config.py
--rw-rw-rw-   0 root         (0) root         (0)    15585 2023-12-13 14:48:59.000000 s11-classifier-3.6.0/classifier/utils/general.py
--rw-rw-rw-   0 root         (0) root         (0)     8696 2023-12-13 14:48:59.000000 s11-classifier-3.6.0/classifier/utils/raster.py
--rw-rw-rw-   0 root         (0) root         (0)     3274 2023-12-13 14:48:59.000000 s11-classifier-3.6.0/classifier/utils/vector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-19 10:53:25.529349 s11-classifier-3.6.0/s11_classifier.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2102 2023-12-19 10:53:25.000000 s11-classifier-3.6.0/s11_classifier.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1037 2023-12-19 10:53:25.000000 s11-classifier-3.6.0/s11_classifier.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-19 10:53:25.000000 s11-classifier-3.6.0/s11_classifier.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-14 12:11:30.000000 s11-classifier-3.6.0/s11_classifier.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      478 2023-12-19 10:53:25.000000 s11-classifier-3.6.0/s11_classifier.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-12-19 10:53:25.000000 s11-classifier-3.6.0/s11_classifier.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-12-19 10:53:25.530349 s11-classifier-3.6.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1537 2023-12-14 12:09:36.000000 s11-classifier-3.6.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-19 10:53:25.528349 s11-classifier-3.6.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-13 14:48:59.000000 s11-classifier-3.6.0/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      902 2023-12-13 14:48:59.000000 s11-classifier-3.6.0/tests/accuracy_test.py
--rw-rw-rw-   0 root         (0) root         (0)     5898 2023-12-13 14:48:59.000000 s11-classifier-3.6.0/tests/config_test.py
--rw-rw-rw-   0 root         (0) root         (0)     8087 2023-12-13 14:48:59.000000 s11-classifier-3.6.0/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-19 10:53:25.529349 s11-classifier-3.6.0/tests/integration/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-13 14:48:59.000000 s11-classifier-3.6.0/tests/integration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2595 2023-12-13 14:48:59.000000 s11-classifier-3.6.0/tests/integration/integration_different_configs_test.py
--rw-rw-rw-   0 root         (0) root         (0)     3413 2023-12-13 14:48:59.000000 s11-classifier-3.6.0/tests/integration/integration_supervised_singleraster_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2687 2023-12-13 14:48:59.000000 s11-classifier-3.6.0/tests/integration/integration_supervised_timeseries_test.py
--rw-rw-rw-   0 root         (0) root         (0)     1471 2023-12-13 14:48:59.000000 s11-classifier-3.6.0/tests/integration/integration_unsupervised_test.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2023-12-13 14:48:59.000000 s11-classifier-3.6.0/tests/samples_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-19 10:53:25.529349 s11-classifier-3.6.0/tests/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-13 14:48:59.000000 s11-classifier-3.6.0/tests/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      899 2023-12-13 14:48:59.000000 s11-classifier-3.6.0/tests/utils/raster_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:34:08.780160 s11-classifier-3.7.0/
+-rw-r--r--   0 root         (0) root         (0)     2102 2024-04-25 07:34:08.779160 s11-classifier-3.7.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1035 2024-04-08 13:24:27.000000 s11-classifier-3.7.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:34:08.774159 s11-classifier-3.7.0/classifier/
+-rw-rw-rw-   0 root         (0) root         (0)      224 2024-03-28 13:26:07.000000 s11-classifier-3.7.0/classifier/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11505 2024-03-28 13:26:07.000000 s11-classifier-3.7.0/classifier/accuracy.py
+-rw-rw-rw-   0 root         (0) root         (0)     8214 2024-03-28 13:26:07.000000 s11-classifier-3.7.0/classifier/classify.py
+-rw-rw-rw-   0 root         (0) root         (0)     4026 2024-03-28 13:26:07.000000 s11-classifier-3.7.0/classifier/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1545 2024-03-28 13:26:07.000000 s11-classifier-3.7.0/classifier/dataprep.py
+-rw-rw-rw-   0 root         (0) root         (0)    14548 2024-03-28 13:26:07.000000 s11-classifier-3.7.0/classifier/models.py
+-rw-rw-rw-   0 root         (0) root         (0)    11365 2024-03-28 13:26:07.000000 s11-classifier-3.7.0/classifier/predict.py
+-rw-rw-rw-   0 root         (0) root         (0)    29392 2024-03-28 13:26:07.000000 s11-classifier-3.7.0/classifier/samples.py
+-rw-rw-rw-   0 root         (0) root         (0)      624 2024-03-28 13:26:07.000000 s11-classifier-3.7.0/classifier/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)    11068 2024-03-28 13:26:07.000000 s11-classifier-3.7.0/classifier/timeseries.py
+-rw-rw-rw-   0 root         (0) root         (0)    10601 2024-03-28 13:26:07.000000 s11-classifier-3.7.0/classifier/train.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:34:08.775159 s11-classifier-3.7.0/classifier/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:26:07.000000 s11-classifier-3.7.0/classifier/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21736 2024-03-28 13:26:07.000000 s11-classifier-3.7.0/classifier/utils/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    15585 2024-03-28 13:26:07.000000 s11-classifier-3.7.0/classifier/utils/general.py
+-rw-rw-rw-   0 root         (0) root         (0)     8696 2024-03-28 13:26:07.000000 s11-classifier-3.7.0/classifier/utils/raster.py
+-rw-rw-rw-   0 root         (0) root         (0)     4183 2024-03-28 13:26:07.000000 s11-classifier-3.7.0/classifier/utils/vector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:34:08.779160 s11-classifier-3.7.0/s11_classifier.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2102 2024-04-25 07:34:08.000000 s11-classifier-3.7.0/s11_classifier.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1064 2024-04-25 07:34:08.000000 s11-classifier-3.7.0/s11_classifier.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 07:34:08.000000 s11-classifier-3.7.0/s11_classifier.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 13:26:55.000000 s11-classifier-3.7.0/s11_classifier.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      478 2024-04-25 07:34:08.000000 s11-classifier-3.7.0/s11_classifier.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-25 07:34:08.000000 s11-classifier-3.7.0/s11_classifier.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 07:34:08.780160 s11-classifier-3.7.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1537 2024-04-08 13:24:27.000000 s11-classifier-3.7.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:34:08.777160 s11-classifier-3.7.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 13:24:27.000000 s11-classifier-3.7.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5196 2024-04-08 13:24:27.000000 s11-classifier-3.7.0/tests/accuracy_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     6191 2024-04-08 13:24:27.000000 s11-classifier-3.7.0/tests/config_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     9208 2024-04-08 13:24:27.000000 s11-classifier-3.7.0/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:34:08.778160 s11-classifier-3.7.0/tests/integration/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 13:24:27.000000 s11-classifier-3.7.0/tests/integration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2595 2024-04-08 13:24:27.000000 s11-classifier-3.7.0/tests/integration/integration_different_configs_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     3413 2024-04-08 13:24:27.000000 s11-classifier-3.7.0/tests/integration/integration_supervised_singleraster_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2687 2024-04-08 13:24:27.000000 s11-classifier-3.7.0/tests/integration/integration_supervised_timeseries_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     1471 2024-04-08 13:24:27.000000 s11-classifier-3.7.0/tests/integration/integration_unsupervised_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     1423 2024-04-08 13:24:27.000000 s11-classifier-3.7.0/tests/samples_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:34:08.778160 s11-classifier-3.7.0/tests/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 13:24:27.000000 s11-classifier-3.7.0/tests/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      899 2024-04-08 13:24:27.000000 s11-classifier-3.7.0/tests/utils/raster_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2528 2024-04-08 13:24:27.000000 s11-classifier-3.7.0/tests/utils/vector_test.py
```

### Comparing `s11-classifier-3.6.0/PKG-INFO` & `s11-classifier-3.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s11-classifier
-Version: 3.6.0
+Version: 3.7.0
 Summary: Classifier
 Home-page: https://gitlab.com/satelligence/classifier
 Author: Satelligence
 Author-email: team@satelligence.com
 License: Apache-2.0
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `s11-classifier-3.6.0/README.md` & `s11-classifier-3.7.0/README.md`

 * *Files identical despite different names*

### Comparing `s11-classifier-3.6.0/classifier/accuracy.py` & `s11-classifier-3.7.0/classifier/accuracy.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,71 @@
 "Accuracy assessment and plotting for classifier"
 import itertools
 import logging
 import time
 from pathlib import Path
-from typing import List, Optional
+from typing import List, Optional, Tuple
 
 import fiona
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from shapely.geometry import shape
-from shapely.ops import cascaded_union
 from sklearn.ensemble import RandomForestRegressor
 from sklearn.metrics import cohen_kappa_score, confusion_matrix
+from sklearn.metrics import classification_report
+from tqdm import tqdm
 
 from classifier.utils.raster import clip_raster_on_geometry, ndarray_to_df
 from classifier.utils.config import Configuration
+from classifier.utils.vector import create_spatial_index, true_intersect
 
 ACCURACY_LOGGER = logging.getLogger(__name__)
 
 
 def write_confusion_matrix(
-        model_dict: dict, test_set: pd.DataFrame, cm_fn: Path,
+        model_dict: dict, test_set: pd.DataFrame, out_dir: Path,
         plot: bool = True, csv: bool = True) -> None:
     """ Uses a sklearn confusion matrix (np 2d array) to write to a csv file
     that also contains overall metrics. Also plots the confusion matrix for
     easier viewing.
 
         Args:
             model_dict (dict):dictionary with the name, model and label encoder
             test_set (pd.DataFrame): test dataset not used during training
-            cm_fn (Path): Path of the output csv file
+            out_dir (Path): output folder
             plot (bool): Whether or not to plot the figure
             csv (bool): Whether or not to write csv file
 
         returns:
             nothing
     """
     # Convert dict and dataframe to arrays
     x_test = test_set[[x for x in test_set.columns
                        if 'class' not in x and 'roi_fid' not in x]].values
     y_test = np.ravel(
         test_set[[x for x in test_set.columns if 'class' in x]].values)
     preds = model_dict['model'].predict(x_test)
-    compute_confusion_matrix(y_test, preds, cm_fn, plot, csv)
+    labels = {int(k): int(v) for k, v in model_dict['labels'].items()}
+    preds_decoded = np.vectorize(lambda x: labels[x])(preds)
+    compute_confusion_matrix(y_test, preds_decoded, out_dir, plot, csv)
 
 
 def compute_confusion_matrix(
-        y_test: np.ndarray, preds: np.ndarray, cm_fn: Path, plot: bool = True,
+        y_test: np.ndarray, preds: np.ndarray, out_dir: Path, plot: bool = True,
         csv: bool = True) -> None:
     """ Uses a sklearn confusion matrix (np 2d array) to write to a csv file
     that also contains overall metrics. Also plots the confusion matrix for
     easier viewing.
 
         Args:
             y_test (np.array): Ground truth (correct) target values
             preds (np.array): Estimated targets as returned by a classifier
-            cm_fn (Path): Path of output file
+            out_dir (Path): output folder
             plot (bool): Whether or not to plot the figure
             csv (bool):  Whether or not to write the csv
     """
 
     # Write and plot confusion Matrix
     cm_labels = sorted(list(set(np.unique(y_test)) | set(np.unique(
         preds))))
@@ -91,26 +95,27 @@
             np.diag(conf_matrix) / np.sum(conf_matrix, axis=0),
             index=cm_labels).rename('Reliability')
         df_cm_all = pd.concat(
             [df_cm, pd.DataFrame(total_row).T,
              pd.DataFrame(reliability).T],
             axis=0)
         df_cm_all.to_csv(
-            cm_fn.with_suffix('.csv'), sep=';', float_format='%.4f')
+            out_dir / 'confusion_matrix.csv', sep=';', float_format='%.4f')
 
     if plot:
         # Plotting if necessary
         try:
             # Plot normalized confusion matrix
             plt.figure()
             plot_confusion_matrix(conf_matrix,
                                   classes=cm_labels,
                                   normalize=True
                                   )
-            plt.savefig(cm_fn.parent / (cm_fn.stem + '_plot.png'), dpi=150)
+            plt.tight_layout()
+            plt.savefig(out_dir / 'confusion_matrix_plot.png', dpi=150)
         except AttributeError:  # Not all models have FIs, so skip
             pass
 
 
 def plot_confusion_matrix(conf_matrix: np.ndarray, classes: List[str],
                           normalize: bool = False,
                           cmap: matplotlib.colors.Colormap = plt.cm.Blues) \
@@ -144,29 +149,29 @@
                  fontsize=4)
 
     plt.tight_layout()
     plt.ylabel('True label')
     plt.xlabel('Predicted label')
 
 
-def plot_feature_importances(model_dict: dict, outfile: Path) -> None:
+def plot_feature_importances(model_dict: dict, out_dir: Path) -> None:
     """Plot the feature importances of the forest
 
     Args:
         model_dict (dict): dict containing the model, metadata and feature names
-        outfile (Path): path to output file
+        out_dir (Path): output folder
     """
     importances = model_dict['model'].feature_importances_
     feat_importances = pd.Series(importances, index=model_dict['names'])
 
     # only features which have higher importance than 0.01 are plotted
     feat_importances_big = feat_importances[feat_importances > 0.01]
 
     fig, axis = plt.subplots()
-    axis.set_title("Feature importances >0.01 (band numbers)")
+    axis.set_title("Feature importances >0.01 \n(band numbers)")
     axis.set_xlabel("Mean decrease in impurity")
 
     # Get STD whenever possible
     if model_dict['app_algorithm'] in [
             'randomforest', 'randomforest_ts_metrics']:
         std = pd.Series(
             np.std([tree.feature_importances_ for tree in model_dict[
@@ -174,65 +179,112 @@
         std = std[feat_importances > 0.01]
         feat_importances_big.sort_values(ascending=False).plot(
             ax=axis, color=['red'], kind='barh', xerr=std)
     else:
         feat_importances_big.sort_values(ascending=False).plot(
             ax=axis, color=['red'], kind='barh')
     fig.tight_layout()
+    outfile = out_dir / 'feature_importance.png'
     plt.savefig(outfile, dpi=300)
 
 
-def assess_accuracy(
-        raster: Path, rois: Path, cm_fn: Path, config: Configuration,
-        subset: Optional[Path] = None) -> None:
-    """"Accuracy assessment
+def collect_classification_and_reference(
+        raster: Path,
+        rois: Path,
+        subset: Path | None = None,
+    ) -> Tuple[np.ndarray, np.ndarray]:
+    """Collect the classification result and reference class for given rois.
+    Ignore rois if it intersects with rois in subset (used for classification). 
 
     Args:
-        raster (Path): Path of classication raster
-        rois (Path): Path of rois
-        cm_fn (Path): Path of output
-        config (Configuration): Configuration
-        subset (Path, optional): Path of subset used for classication
-    """
-
-    start = time.time()
+        raster (Path): raster path
+        rois (Path): all rois
+        subset (Path | None, optional): rois used for classification. Defaults to None.
 
+    Returns:
+        Tuple[np.ndarray, np.ndarray]: class prediction, class reference
+    """
+    ACCURACY_LOGGER.info("Collect predicted and reference class")
     # Is subset is given, exclude its polygons from accuracy assessment
     if subset:
-        polygons = [
-            shape(feature['geometry']) for feature in fiona.open(subset)]
-        union_subset = cascaded_union(polygons)
-    sample_labels = []
-    all_samples = []
+        rtree_index = create_spatial_index(subset)
+    all_y_pred = []
+    all_y_true = []
     counter = 0
     with fiona.open(rois, "r") as shapefile:
-        for roi in shapefile:
-            if subset and shape(roi['geometry']).intersects(union_subset):
-                counter += 1
-                continue
-            roi_samples = clip_raster_on_geometry(
-                raster,
-                roi['geometry']
-            ).flatten()
-            if roi_samples is not None:
-                all_samples += list(roi_samples.astype(float))
-                roi_id = int(roi['properties']['id'])
-                sample_labels += len(roi_samples) * [roi_id]
-        all_samples = np.array(all_samples)
-        sample_labels = np.array(sample_labels)
+        for roi in tqdm(shapefile):
+            roi_geom = shape(roi['geometry'])
+            if subset:
+                with fiona.open(subset) as subset_polygons:
+                    fids = list(rtree_index.intersection(roi_geom.bounds))
+                    # only skip when theres a true intersection
+                    if any(
+                        true_intersect(
+                            roi_geom, shape(subset_polygons[int(fid)]['geometry']))
+                        for fid in fids
+                    ):
+                        counter += 1
+                        continue
+            roi_samples = clip_raster_on_geometry(raster, roi_geom).flatten()
+            if roi_samples is not None and roi_samples.size != 0:
+                y_pred = roi_samples.astype(int)
+                y_true = int(roi['properties']['id'])
+
+                all_y_pred += list(y_pred)
+                all_y_true += len(y_pred) * [y_true]
+
+        all_y_pred = np.array(all_y_pred)
+        all_y_true = np.array(all_y_true)
 
         ACCURACY_LOGGER.info(
-            "Using %i groundtruth polygons, \
-                excluding %i already used in classifier",
+            "Using %i groundtruth polygons, excluding %i already used in classifier",
             len(shapefile),
             counter)
+    return all_y_pred, all_y_true
+
+
+def assess_accuracy(
+        raster: Path,
+        rois: Path,
+        out_dir: Path,
+        config: Configuration,
+        subset: Optional[Path] = None,
+    ) -> None:
+    """"Accuracy assessment
+
+    Args:
+        raster (Path): Path of classication raster
+        rois (Path): Path of rois
+        out_dir (Path): Path of output
+        config (Configuration): Configuration
+        subset (Path, optional): Path of subset used for classication
+    """
+    start = time.time()
+    y_pred, y_true = collect_classification_and_reference(
+        raster,
+        rois,
+        subset,
+    )
+
+    report = pd.DataFrame(
+        classification_report(
+            y_true=y_true,
+            y_pred=y_pred,
+            output_dict=True
+            )
+    ).T
+    report.to_csv(
+        out_dir / 'classification_report.csv',
+        sep=';',
+        float_format='%.4f',
+    )
 
     # write confusion matrix
     compute_confusion_matrix(
-        sample_labels, all_samples, cm_fn, plot=True, csv=False)
+        y_test=y_true, preds=y_pred, out_dir=out_dir, plot=True, csv=True)
     config.tmp_dir.cleanup()
     ACCURACY_LOGGER.info(
         "Total run time was %i seconds", (int(time.time() - start)))
 
 
 def get_confidence_map_from_random_forest_model(
         model: RandomForestRegressor,
```

### Comparing `s11-classifier-3.6.0/classifier/classify.py` & `s11-classifier-3.7.0/classifier/classify.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,21 +49,17 @@
         model_dict, test = train_dataset(
             samples,
             out_dir,
             config
         )
         if config.app.algorithm in ['randomforest', 'xgboost'] \
                 and config.accuracy.perform_assesment:
-            CLASSIFIER_LOGGER.info(
-                "\n####----Accuracy Assessment----#####\n")
             # Do the accuracy analysis
-            cm_fn = out_dir / 'confusion_matrix'
-            fi_fn = out_dir / 'feature_importance.png'
-            write_confusion_matrix(model_dict, test, cm_fn)
-            plot_feature_importances(model_dict, fi_fn)
+            write_confusion_matrix(model_dict, test, out_dir)
+            plot_feature_importances(model_dict, out_dir)
     # save the model as a python pickle
     if not rois_extent is None:
         model_dict['rois_bounds'] = rois_extent
     if config.app.model_save:
         save_model(model_dict, out_dir, config)
     CLASSIFIER_LOGGER.info("\nFinished Training\n")
     return model_dict
```

### Comparing `s11-classifier-3.6.0/classifier/cli.py` & `s11-classifier-3.7.0/classifier/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -111,16 +111,15 @@
         [str(raster)],
         overwrite,
         config_location,
         rois
     )
     if subset is not None:
         subset = WORKSPACE / subset
-    cm_fn = out_dir / 'confusion_matrix_total'
-    assess_accuracy(rasters[0], rois_path, cm_fn, config, subset)
+    assess_accuracy(rasters[0], rois_path, out_dir, config, subset)
 
 
 @ cli.command()
 def make_config() -> None:
     """Make a config file with default values in your workspace directory
     and exit"""
     save_config_as_json()
```

### Comparing `s11-classifier-3.6.0/classifier/models.py` & `s11-classifier-3.7.0/classifier/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,19 @@
         self.ccp_alpha = ccp_alpha
         self.max_samples = max_samples
 
 
 class XGBoost(XGBClassifier, BaseMixin):
     """XGBoost class, child of XGBoostclassifier model from sk-learn"""
 
-    def __init__(self, objective: str ="binary:logistic", **kwargs) -> None:
+    def __init__(
+            self,
+            objective: str ="binary:logistic",
+            **kwargs: Any
+        ) -> None:
         super().__init__(objective=objective, **kwargs)
         self.optimization_parameters = {
             "learning_rate": [0.1, 0.2, 0.3],
             "n_estimators": [10, 20, 50, 100, 200],
             "max_depth": [1, 3, 5, 10]
         }
```

### Comparing `s11-classifier-3.6.0/classifier/predict.py` & `s11-classifier-3.7.0/classifier/predict.py`

 * *Files identical despite different names*

### Comparing `s11-classifier-3.6.0/classifier/samples.py` & `s11-classifier-3.7.0/classifier/samples.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 import rasterio
 from rasterio.windows import Window
 from sklearn.ensemble import IsolationForest
 from sklearn.impute import SimpleImputer
 
 from classifier.dataprep import class_counts
 from classifier.settings import US_ALGORITHMS
-from classifier.utils.config import Configuration
+from classifier.utils.config import (Configuration,
+                                     SubsampleSupervisedConfiguration)
 from classifier.utils.general import parallel_function, rois_in_raster_extent
 from classifier.utils.raster import (count_bands, get_bandnames, get_meta,
                                      get_raster_date, clip_raster_on_geometry,
                                      verify_and_count_bands)
 
 SAMPLES_LOGGER = logging.getLogger(__name__)
 
@@ -347,16 +348,22 @@
                 "Check your rois or rasters."
             )
             sys.exit(1)
 
         # make class column instead of index
         samples_df.reset_index(level='class', inplace=True)
 
-        # Remove outliers (right now only for non timeseries)
         if not for_prediction:
+            # Subsample the data
+            if config.supervised.subsample.active:
+                samples_df = Samples.subsample(
+                    samples_df, config.supervised.subsample
+                )
+
+            # Remove outliers (right now only for non timeseries)
             if config.supervised.remove_outliers \
                     and not config.app.rasters_are_timeseries:
                 samples_df = self.outlier_removal(
                     samples_df, config)
 
         # make roi_fid a column instead of index
         samples_df.reset_index(level='roi_fid', inplace=True)
@@ -627,14 +634,46 @@
         # prediction sometimes lie partially outside
         if rois is not None and len(rois) > 1:
             rois_lie_inside_rasters = rois_in_raster_extent(
                 rasters, rois)
             return rois_lie_inside_rasters
         return True
 
+    @staticmethod
+    def subsample(
+        samples: pd.DataFrame,
+        config_subsampling: SubsampleSupervisedConfiguration,
+        ) -> pd.DataFrame:
+        """Subsampling
+
+        Args:
+            samples (pd.DataFrame): samples
+            config (SubsampleSupervisedConfiguration): 
+                Parameters to use for subsampling
+
+        Returns:
+            samples (pd.DataFrame): subsampled samples 
+        """
+        group_by = config_subsampling.group_by
+        sample_type = config_subsampling.sample_type
+        amount = config_subsampling.amount
+        replace = config_subsampling.replace
+
+        SAMPLES_LOGGER.info(
+            "Do subsampling based on %s with %s: %s, replace: %s",
+            group_by, sample_type, amount, replace)
+
+        SAMPLES_LOGGER.info("Total size before subsampling: %s",
+                            len(samples))
+        samples = samples.groupby(by=group_by).sample(
+            **{sample_type: amount, 'replace': replace}, random_state=0)
+        SAMPLES_LOGGER.info("Total size after subsampling: %s",
+                            len(samples))
+        return samples
+
 
 class TimeSeries(Samples):
     """Class for Timeseries samples, subclass of Sample
 
     Overwrites some methods of Sample which need to be
     adjusted for time series
     """
```

### Comparing `s11-classifier-3.6.0/classifier/settings.py` & `s11-classifier-3.7.0/classifier/settings.py`

 * *Files identical despite different names*

### Comparing `s11-classifier-3.6.0/classifier/timeseries.py` & `s11-classifier-3.7.0/classifier/timeseries.py`

 * *Files identical despite different names*

### Comparing `s11-classifier-3.6.0/classifier/train.py` & `s11-classifier-3.7.0/classifier/train.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 "Training module for classifier"
 import logging
 import dataclasses
 from pathlib import Path
-from typing import Any, List, Tuple
+from typing import Any, List, Tuple, Dict
 
 import numpy as np
 import pandas as pd
 from sklearn.model_selection import train_test_split
+from sklearn.preprocessing import LabelEncoder
 
 from classifier import __version__ as classifier_version
 from classifier.utils.general import dict_product
 from classifier.settings import ALGORITHM_DICT
 from classifier.samples import Samples
 from classifier.utils.config import Configuration
 from classifier.utils.general import get_available_model_args
@@ -57,21 +58,20 @@
         config (Configuration): contains config
 
     Returns:
         model_dict (dict): A dictionary containing the name, model and label
                         encoder.
         test (np.ndarray): A test dataset which was not used during training
     """
-    # Encode the labels
-    labels = np.unique(samples.get_labels().values).tolist()
-    labels = dict(zip(range(len(labels)), labels))
     # Split the dataset,
-    model, xcols, test = init_model_and_train(samples.get_samples(),
-                                              out_dir,
-                                              config)
+    model, xcols, test, labels = init_model_and_train(
+        samples.get_samples(),
+        out_dir,
+        config,
+    )
 
     model_dict = {'app_algorithm': config.app.algorithm,
                   'model': model,
                   'labels': labels,
                   'names': xcols,
                   'version': classifier_version}
     return model_dict, test
@@ -232,30 +232,31 @@
 
     optimized_model = set_model_parameters(
         config.app.algorithm, algorithm_args)
 
     return optimized_model
 
 
-def init_model_and_train(dataset: pd.DataFrame,
-                         out_dir: Path,
-                         config: Configuration) -> Tuple[
-                             Any, List[str], pd.DataFrame]:
+def init_model_and_train(
+        dataset: pd.DataFrame,
+        out_dir: Path,
+        config: Configuration
+    ) -> Tuple[Any, List[str], pd.DataFrame, Dict[str, str]]:
     """Set the model parameters and train it
 
     Args:
         dataset (Array) : The dataset for input in the model (array)
         out_dir (Path): The output directory
         config (Configuration): Contains config
 
     Returns:
         model (Any): Trained sklearn model
         xcols (List[str]): Names of bands
         test (pd.DataFrame): Test dataset
-
+        labels (Dict[str, str]): labels mapped to ascending integers
     """
     optimize = config.supervised.optimization.optimize
     test_size = config.accuracy.testfraction
     algorithm_args = {}
 
     train, test = train_test_split(dataset, test_size=test_size)
     xcols = [x for x in train.columns
@@ -263,27 +264,33 @@
     if config.app.algorithm == 'knn_dtw':
         # keep class and roi_fid column for knn_dtw training
         x_train = train
     else:
         x_train = train[xcols]
     y_train = train['class']
 
+    # encode the labels
+    label_encoder = LabelEncoder()
+    y_train_encoded = label_encoder.fit_transform(y_train)
+    labels_encoded = zip(label_encoder.transform(label_encoder.classes_), label_encoder.classes_)
+    labels = {str(k): str(v) for k, v in labels_encoded}
+
     # Get the model/algorithm arguments
     algorithm_args = get_algorithm_args(config, dataset, out_dir)
 
     # Create the model with the given params
     model = set_model_parameters(config.app.algorithm, algorithm_args)
     # Optimize model
     if optimize:
         model = optimize_model(
-            model, x_train, y_train, out_dir, config)
+            model, x_train, y_train_encoded, out_dir, config)
 
     # y_train_encoded = sample_labels_encoder.transform(y_train)
     TRAIN_LOGGER.info("Train model ...")
     # Use array repr (x_train.values) to make sure feature names are not used.
     # Except when we use KNN DTW, because that needs the band names.
     if not config.app.algorithm == 'knn_dtw':
         x_train = x_train.values
 
-    model.fit(x_train, y_train)
+    model.fit(x_train, y_train_encoded)
     TRAIN_LOGGER.info("Model trained.")
-    return model, xcols, test
+    return model, xcols, test, labels
```

### Comparing `s11-classifier-3.6.0/classifier/utils/config.py` & `s11-classifier-3.7.0/classifier/utils/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,22 @@
     "supervised": {
         "probability": True,
         "all_probabilities": False,
         "remove_outliers": True,  # Remove outliers from the training data
         "optimization": {
             "optimize": False,  # Optimize the model parameters
             "optimize_number": 10,  # Number of iterations for optimization
-        }
+        },
+        "subsample": {
+            "active": False,
+            "group_by": "class",
+            "sample_type": "n",
+            "amount": 100,
+            "replace": False,
+        },
     },
     "unsupervised": {
         "nclasses": 2,  # Number of classes for unsupervised
         "trainfraction": 1.0  # Fraction of raster used for training
     },
     "accuracy": {
         "perform_assesment": True,  # Perform accuracy assessment
@@ -231,33 +238,68 @@
     optimize = fields.Bool()
     optimize_number = fields.Int(
         validate=validate.Range(
             min=1,
             error="Value must be greater than 0. Better value is > 5.")
     )
 
+@ dataclass
+class SubsampleSupervisedConfiguration():
+    """Dataclass which stores the subsample parameters for
+    the supervised classification"""
+
+    active: bool  # Do sampling
+    group_by: str  # Groupby class or roi_fid
+    sample_type: str # n or frac
+    amount: Union[int, float] # int for n and float for frac
+    replace: bool # reuse values when sampling
+
+
+class SubsampleSupervisedConfigurationSchema(Schema):
+    """Schema for the subsample part of the supervised classification
+    configuration dataclass.
+    Will raise ValidationErrors when invalid data are passed in"""
+    active = fields.Bool()
+    group_by = fields.Str(validate=validate.OneOf(['class', 'roi_fid']))
+    sample_type = fields.Str(validate=validate.OneOf(['n', 'frac']))
+    amount = IntFloatField(
+        {'Int':
+            fields.Int(
+                validate=validate.Range(
+                    min=1,
+                    error="Value must be >= 1."),
+            ),
+         'Float':
+            fields.Float(
+                validate=validate.Range(
+                    min=0.01, max=1))
+         }
+    )
+    replace = fields.Bool()
 
 @ dataclass
 class SupervisedConfiguration:
     """Dataclass which stores supervised classification config"""
 
     probability: bool  # output probability map
     all_probabilities: bool
     remove_outliers: bool  # Remove outliers from the training data
     optimization: OptimizeSupervisedConfiguration
+    subsample: SubsampleSupervisedConfiguration
 
 
 class SupervisedConfigurationSchema(Schema):
     """Schema for the supervised classification configuration dataclass.
     Will raise ValidationErrors when invalid data are passed in"""
 
     probability = fields.Bool()
     all_probabilities = fields.Bool()
     remove_outliers = fields.Bool()  # Remove outliers from the training data
     optimization = fields.Nested(OptimizeSupervisedConfigurationSchema)
+    subsample = fields.Nested(SubsampleSupervisedConfigurationSchema)
 
 
 @ dataclass
 class UnsupervisedConfiguration:
     """Dataclass which stores unsupervised classification config"""
 
     nclasses: int  # Number of classes for unsupervised
```

### Comparing `s11-classifier-3.6.0/classifier/utils/general.py` & `s11-classifier-3.7.0/classifier/utils/general.py`

 * *Files identical despite different names*

### Comparing `s11-classifier-3.6.0/classifier/utils/raster.py` & `s11-classifier-3.7.0/classifier/utils/raster.py`

 * *Files identical despite different names*

### Comparing `s11-classifier-3.6.0/classifier/utils/vector.py` & `s11-classifier-3.7.0/classifier/utils/vector.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 import numpy as np
 import fiona
 import rasterio
 from geopandas import GeoDataFrame
 from rasterio import Affine
 from rasterio.features import shapes
 from rasterio.windows import Window
-from shapely.geometry import MultiPolygon, Polygon
+from rtree.index import Index
+from shapely.geometry.base import BaseGeometry
+from shapely.geometry import MultiPolygon, Polygon, shape
 
 UTILS_VECTOR_LOGGER = logging.getLogger(__name__)
 
 
 def vectorize_array(
         array_to_vectorize: np.ndarray,
         transform: Optional[Affine] = None) -> GeoDataFrame:
@@ -101,7 +103,39 @@
 
     Returns:
         bounds of rois (list): ulx, uly, llx, lly coordinates
 
     """
     with fiona.open(rois, "r") as shapefile:
         return shapefile.bounds
+
+
+def create_spatial_index(rois: Path) -> Index:
+    """Create an RTree spatial index filled with the bboxes of the polygons
+
+    Args:
+        rois (Path): rois path
+
+    Returns:
+        Index: rtree index
+    """
+    rtree_index = Index()
+    with fiona.open(rois) as polygons:
+        for fid, feature in polygons.items():
+            geometry = shape(feature['geometry'])
+            rtree_index.insert(fid, geometry.bounds)
+    return rtree_index
+
+
+def true_intersect(geom_1: BaseGeometry, geom_2: BaseGeometry) -> bool:
+    """Check for a true intersection (not only touch, but overlap)
+
+    Args:
+        geom_1 (BaseGeometry): geometry 1
+        geom_2 (BaseGeometry): geometry 2
+
+    Returns:
+        bool: true if true intersection
+    """
+    return bool(geom_1.relate_pattern(
+        geom_2, 'T********'
+    ))
```

### Comparing `s11-classifier-3.6.0/s11_classifier.egg-info/PKG-INFO` & `s11-classifier-3.7.0/s11_classifier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s11-classifier
-Version: 3.6.0
+Version: 3.7.0
 Summary: Classifier
 Home-page: https://gitlab.com/satelligence/classifier
 Author: Satelligence
 Author-email: team@satelligence.com
 License: Apache-2.0
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `s11-classifier-3.6.0/s11_classifier.egg-info/SOURCES.txt` & `s11-classifier-3.7.0/s11_classifier.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,8 +29,9 @@
 tests/samples_test.py
 tests/integration/__init__.py
 tests/integration/integration_different_configs_test.py
 tests/integration/integration_supervised_singleraster_test.py
 tests/integration/integration_supervised_timeseries_test.py
 tests/integration/integration_unsupervised_test.py
 tests/utils/__init__.py
-tests/utils/raster_test.py
+tests/utils/raster_test.py
+tests/utils/vector_test.py
```

### Comparing `s11-classifier-3.6.0/setup.py` & `s11-classifier-3.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # (c) Satelligence, see LICENSE.
 # pylint: skip-file
 from setuptools import setup
 import setuptools
 
-version = '3.6.0'
+version = '3.7.0'
 
 long_description = open('README.md').read()
 
 test_requirements = [
     'pytest'
 ]
```

### Comparing `s11-classifier-3.6.0/tests/config_test.py` & `s11-classifier-3.7.0/tests/config_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """ Unittests for config file"""
 from classifier.utils.config import (
     AccuracyConfiguration, AppConfiguration, Configuration,
     OptimizeSupervisedConfiguration, RandomForestConfiguration,
-    SupervisedConfiguration, UnsupervisedConfiguration, json_to_config)
+    SupervisedConfiguration, UnsupervisedConfiguration, SubsampleSupervisedConfiguration, 
+    json_to_config)
 from classifier.utils.config import DtwConfiguration, json_to_config
 import copy
 import json
 import os
 import unittest
 
 from classifier.utils.config import PARAMETERS
@@ -55,14 +56,21 @@
             SupervisedConfiguration(
                 probability=probability,
                 all_probabilities=all_probabilities,
                 remove_outliers=remove_outliers,
                 optimization=OptimizeSupervisedConfiguration(
                     optimize=optimize,
                     optimize_number=optimize_number),
+                subsample=SubsampleSupervisedConfiguration(
+                    active=False,
+                    group_by='class',
+                    sample_type='n',
+                    amount=100,
+                    replace=False,
+                )
             ),
             UnsupervisedConfiguration(nclasses, trainfraction),
             AccuracyConfiguration(perform_assesment, testfraction),
             DtwConfiguration(
                 patterns=None,
                 patterns_save=False,
                 number_of_patterns_per_class=1,
```

### Comparing `s11-classifier-3.6.0/tests/conftest.py` & `s11-classifier-3.7.0/tests/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -250,7 +250,47 @@
     )
     columns = pd.MultiIndex.from_product(
         [dates, bands],
         names=['Date', 'Band']
     )
     samples_test = pd.DataFrame(data, index=index, columns=columns)
     return samples_test
+
+@pytest.fixture
+def setup_samples_df_with_rois_fid():
+    data = np.array([[1., 4.],
+                    [2., 3.],
+                    [1., 7.],
+                    [1., 8.],
+                    ])
+        
+    roi_classes = [0, 0, 1, 1]
+    roi_fids = [1, 1, 2, 2]
+    pixel_ids = [0, 1, 0, 1]
+    bands = ['B01', 'B02']
+
+    index = pd.MultiIndex.from_tuples(
+        list(zip(roi_classes, roi_fids, pixel_ids)),
+        names=['class', 'roi_fid', 'pixel_id']
+    )
+    columns = ['band0', 'band1']
+    samples_test = pd.DataFrame(data, index=index, columns=columns)
+    return samples_test
+
+@pytest.fixture
+def setup_samples_df_with_rois_fid_subsampled():
+    data = np.array([[2., 3.],
+                    [1., 7.],
+                    ])
+        
+    roi_classes = [0, 1]
+    roi_fids = [1, 2]
+    pixel_ids = [1, 0]
+    bands = ['B01', 'B02']
+
+    index = pd.MultiIndex.from_tuples(
+        list(zip(roi_classes, roi_fids, pixel_ids)),
+        names=['class', 'roi_fid', 'pixel_id']
+    )
+    columns = ['band0', 'band1']
+    samples_test = pd.DataFrame(data, index=index, columns=columns)
+    return samples_test
```

### Comparing `s11-classifier-3.6.0/tests/integration/integration_different_configs_test.py` & `s11-classifier-3.7.0/tests/integration/integration_different_configs_test.py`

 * *Files identical despite different names*

### Comparing `s11-classifier-3.6.0/tests/integration/integration_supervised_singleraster_test.py` & `s11-classifier-3.7.0/tests/integration/integration_supervised_singleraster_test.py`

 * *Files identical despite different names*

### Comparing `s11-classifier-3.6.0/tests/integration/integration_supervised_timeseries_test.py` & `s11-classifier-3.7.0/tests/integration/integration_supervised_timeseries_test.py`

 * *Files identical despite different names*

### Comparing `s11-classifier-3.6.0/tests/integration/integration_unsupervised_test.py` & `s11-classifier-3.7.0/tests/integration/integration_unsupervised_test.py`

 * *Files identical despite different names*

### Comparing `s11-classifier-3.6.0/tests/samples_test.py` & `s11-classifier-3.7.0/tests/samples_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 "Test for samples module"
 import numpy as np
+import pandas as pd
 from classifier.samples import Samples, TimeSeries
-from classifier.utils.config import setup_config
+from classifier.utils.config import setup_config, SubsampleSupervisedConfiguration
 
 
 def test_impute_timeseries_AsExpected(
         setup_samples_df_with_nans_ref, setup_samples_df_with_nans):
     ref_samples = setup_samples_df_with_nans_ref
     timeseries = TimeSeries(None, None, None)
 
@@ -19,7 +20,23 @@
         setup_samples_df, setup_samples_df_with_outliers):
     config = setup_config()
     
     ref_samples = setup_samples_df
     samples_outlier_removed = Samples.outlier_removal(
         setup_samples_df_with_outliers, config)
     np.array_equal(ref_samples.values, samples_outlier_removed.values)
+    
+    
+def test_subsample_AsExpected(
+        setup_samples_df_with_rois_fid, setup_samples_df_with_rois_fid_subsampled):
+    samples = setup_samples_df_with_rois_fid
+    
+    config = SubsampleSupervisedConfiguration(
+        active=True,
+        group_by='roi_fid',
+        sample_type='n',
+        amount=1,
+        replace=False
+    )
+
+    samples_subsampled = Samples.subsample(samples, config)
+    pd.testing.assert_frame_equal(samples_subsampled, setup_samples_df_with_rois_fid_subsampled)
```

### Comparing `s11-classifier-3.6.0/tests/utils/raster_test.py` & `s11-classifier-3.7.0/tests/utils/raster_test.py`

 * *Files identical despite different names*

