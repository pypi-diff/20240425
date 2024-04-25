# Comparing `tmp/the_utils-0.4.0.tar.gz` & `tmp/the_utils-0.5.0.tar.gz`

## Comparing `the_utils-0.4.0.tar` & `the_utils-0.5.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 the_utils-0.4.0/.editorconfig
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 the_utils-0.4.0/.gitmodules
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 the_utils-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    17935 2020-02-02 00:00:00.000000 the_utils-0.4.0/.pylintrc
--rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 the_utils-0.4.0/CHANGELOG.md
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 the_utils-0.4.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 the_utils-0.4.0/requirements-dev.txt
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 the_utils-0.4.0/requirements.txt
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 the_utils-0.4.0/.ci/cuda.sh
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 the_utils-0.4.0/.ci/docs.sh
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 the_utils-0.4.0/.ci/install-cpu.sh
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 the_utils-0.4.0/.ci/install-dev.sh
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 the_utils-0.4.0/.ci/install.sh
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 the_utils-0.4.0/.ci/nb.sh
--rw-r--r--   0        0        0    56106 2020-02-02 00:00:00.000000 the_utils-0.4.0/.ci/configs/nb.py
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 the_utils-0.4.0/.github/workflows/release.yml
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 the_utils-0.4.0/.vscode/extensions.json
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 the_utils-0.4.0/demos/demo.ipynb
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 the_utils-0.4.0/docs/Makefile
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 the_utils-0.4.0/docs/conf.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 the_utils-0.4.0/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 the_utils-0.4.0/docs/make.bat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 the_utils-0.4.0/docs/_static/css/table.css
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 the_utils-0.4.0/docs/rst/the_utils.bot.rst
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 the_utils-0.4.0/docs/rst/the_utils.common.rst
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 the_utils-0.4.0/docs/rst/the_utils.evaluation.rst
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 the_utils-0.4.0/docs/rst/the_utils.file.rst
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 the_utils-0.4.0/docs/rst/the_utils.plt.rst
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 the_utils-0.4.0/docs/rst/the_utils.save_load.rst
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 the_utils-0.4.0/docs/rst/the_utils.setting.rst
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 the_utils-0.4.0/docs/tpls/module.rst_t
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 the_utils-0.4.0/docs/tpls/package.rst_t
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 the_utils-0.4.0/docs/tpls/toc.rst_t
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 the_utils-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 the_utils-0.4.0/the_utils/__init__.py
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 the_utils-0.4.0/the_utils/bot.py
--rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 the_utils-0.4.0/the_utils/common.py
--rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 the_utils-0.4.0/the_utils/file.py
--rw-r--r--   0        0        0    10349 2020-02-02 00:00:00.000000 the_utils-0.4.0/the_utils/plt.py
--rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 the_utils-0.4.0/the_utils/save_load.py
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 the_utils-0.4.0/the_utils/setting.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 the_utils-0.4.0/the_utils/evaluation/__init__.py
--rw-r--r--   0        0        0    18771 2020-02-02 00:00:00.000000 the_utils-0.4.0/the_utils/evaluation/unsupervised_graph_learning.py
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 the_utils-0.4.0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 the_utils-0.4.0/LICENSE
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 the_utils-0.4.0/README.md
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 the_utils-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 the_utils-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 the_utils-0.5.0/.editorconfig
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 the_utils-0.5.0/.gitmodules
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 the_utils-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    17935 2020-02-02 00:00:00.000000 the_utils-0.5.0/.pylintrc
+-rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 the_utils-0.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 the_utils-0.5.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 the_utils-0.5.0/requirements-dev.txt
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 the_utils-0.5.0/requirements.txt
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 the_utils-0.5.0/.ci/cuda.sh
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 the_utils-0.5.0/.ci/docs.sh
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 the_utils-0.5.0/.ci/install-cpu.sh
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 the_utils-0.5.0/.ci/install-dev.sh
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 the_utils-0.5.0/.ci/install.sh
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 the_utils-0.5.0/.ci/nb.sh
+-rw-r--r--   0        0        0    56106 2020-02-02 00:00:00.000000 the_utils-0.5.0/.ci/configs/nb.py
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 the_utils-0.5.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 the_utils-0.5.0/.vscode/extensions.json
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 the_utils-0.5.0/demos/demo.ipynb
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 the_utils-0.5.0/docs/Makefile
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 the_utils-0.5.0/docs/conf.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 the_utils-0.5.0/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 the_utils-0.5.0/docs/make.bat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 the_utils-0.5.0/docs/_static/css/table.css
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 the_utils-0.5.0/docs/rst/the_utils.bot.rst
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 the_utils-0.5.0/docs/rst/the_utils.common.rst
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 the_utils-0.5.0/docs/rst/the_utils.evaluation.rst
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 the_utils-0.5.0/docs/rst/the_utils.file.rst
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 the_utils-0.5.0/docs/rst/the_utils.plt.rst
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 the_utils-0.5.0/docs/rst/the_utils.save_load.rst
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 the_utils-0.5.0/docs/rst/the_utils.setting.rst
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 the_utils-0.5.0/docs/tpls/module.rst_t
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 the_utils-0.5.0/docs/tpls/package.rst_t
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 the_utils-0.5.0/docs/tpls/toc.rst_t
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 the_utils-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 the_utils-0.5.0/the_utils/__init__.py
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 the_utils-0.5.0/the_utils/bot.py
+-rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 the_utils-0.5.0/the_utils/common.py
+-rw-r--r--   0        0        0     5766 2020-02-02 00:00:00.000000 the_utils-0.5.0/the_utils/file.py
+-rw-r--r--   0        0        0    10550 2020-02-02 00:00:00.000000 the_utils-0.5.0/the_utils/plt.py
+-rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 the_utils-0.5.0/the_utils/save_load.py
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 the_utils-0.5.0/the_utils/setting.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 the_utils-0.5.0/the_utils/evaluation/__init__.py
+-rw-r--r--   0        0        0    18771 2020-02-02 00:00:00.000000 the_utils-0.5.0/the_utils/evaluation/unsupervised_graph_learning.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 the_utils-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 the_utils-0.5.0/LICENSE
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 the_utils-0.5.0/README.md
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 the_utils-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 the_utils-0.5.0/PKG-INFO
```

### Comparing `the_utils-0.4.0/.pre-commit-config.yaml` & `the_utils-0.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `the_utils-0.4.0/.pylintrc` & `the_utils-0.5.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `the_utils-0.4.0/CHANGELOG.md` & `the_utils-0.5.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 # CHANGELOG
 
 
 
+## v0.5.0 (2024-04-25)
+
+### Feature
+
+* feat: add insert_info and append_info ([`4976798`](https://github.com/galogm/the_utils/commit/497679833f21ac94d26de1b08a8f07e39bdd8ec5))
+
+### Unknown
+
+* Merge branch &#39;master&#39; of github.com:galogm/graph_utils ([`e97d3fe`](https://github.com/galogm/the_utils/commit/e97d3fe4c9a4026fedbf4cb1886b9814a19d3bd1))
+
+
 ## v0.4.0 (2024-04-23)
 
 ### Feature
 
 * feat: add x_label and y_label ([`920bbc4`](https://github.com/galogm/the_utils/commit/920bbc474b2e8eaebd1b372ee5f5609eae75a54e))
 
 ### Unknown
```

### Comparing `the_utils-0.4.0/.ci/cuda.sh` & `the_utils-0.5.0/.ci/cuda.sh`

 * *Files identical despite different names*

### Comparing `the_utils-0.4.0/.ci/install-cpu.sh` & `the_utils-0.5.0/.ci/install-cpu.sh`

 * *Files identical despite different names*

### Comparing `the_utils-0.4.0/.ci/install-dev.sh` & `the_utils-0.5.0/.ci/install-dev.sh`

 * *Files identical despite different names*

### Comparing `the_utils-0.4.0/.ci/install.sh` & `the_utils-0.5.0/.ci/install.sh`

 * *Files identical despite different names*

### Comparing `the_utils-0.4.0/.ci/configs/nb.py` & `the_utils-0.5.0/.ci/configs/nb.py`

 * *Files identical despite different names*

### Comparing `the_utils-0.4.0/.github/workflows/release.yml` & `the_utils-0.5.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `the_utils-0.4.0/demos/demo.ipynb` & `the_utils-0.5.0/demos/demo.ipynb`

 * *Files identical despite different names*

### Comparing `the_utils-0.4.0/docs/Makefile` & `the_utils-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `the_utils-0.4.0/docs/conf.py` & `the_utils-0.5.0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'the_utils'
 copyright = '2023, galo.gm'
 author = 'galo.gm'
 
 # The full version, including alpha/beta/rc tags
-release = '0.4.0'
+release = '0.5.0'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `the_utils-0.4.0/docs/index.rst` & `the_utils-0.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `the_utils-0.4.0/docs/make.bat` & `the_utils-0.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `the_utils-0.4.0/docs/tpls/package.rst_t` & `the_utils-0.5.0/docs/tpls/package.rst_t`

 * *Files identical despite different names*

### Comparing `the_utils-0.4.0/the_utils/bot.py` & `the_utils-0.5.0/the_utils/bot.py`

 * *Files identical despite different names*

### Comparing `the_utils-0.4.0/the_utils/common.py` & `the_utils-0.5.0/the_utils/common.py`

 * *Files identical despite different names*

### Comparing `the_utils-0.4.0/the_utils/file.py` & `the_utils-0.5.0/the_utils/file.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """File Management.
 """
+
 import csv
 import os
 from pathlib import Path
 from pathlib import PurePath
 from typing import Any
 from typing import List
 
@@ -124,25 +125,27 @@
                     if os.stat(target_path).st_size == 0:
                         csv_write.writerow(thead)
                 csv_write.writerow(tbody)
 
 
 def save_to_csv_files(
     results: dict,
-    add_info: dict,
     csv_name: str,
+    insert_info: dict = None,
+    append_info: dict = None,
     save_path="./results",
     sort_head: bool = False,
 ) -> None:
     """Save the evaluation results to a local csv file.
 
     Args:
         results (dict): Evaluation results document.
-        add_info (dict): Additional information, such as data set name, method name.
         csv_name (str): csv file name to store.
+        insert_info (dict): Insert information in front of the results. Defaults to None.
+        append_info (dict): Append information after the results. Defaults to None.
         save_path (str, optional): Folder path to store. Defaults to './results'.
         sort_head (bool, optional): whether to sort the head before writing. Defaults to False.
 
     Example:
         .. code-block:: python
 
             from the_utils import evaluate_from_embed_file
@@ -153,20 +156,24 @@
 
             clustering_res, classification_res = evaluate_from_embed_file(
                 f'{data_name}_{method_name}_embeds.pth',
                 f'{data_name}_data.pth',
                 save_path='./save/',
             )
 
-            add_info = {'data': data_name, 'method': method_name,}
-            save_to_csv_files(clustering_res, add_info, 'clutering.csv')
-            save_to_csv_files(classification_res, add_info, 'classification.csv')
+            insert_info = {'data': data_name, 'method': method_name,}
+            save_to_csv_files(clustering_res, insert_info, 'clutering.csv')
+            save_to_csv_files(classification_res, insert_info, 'classification.csv')
     """
     # save to csv file
-    results.update(add_info)
+    results = {
+        **(insert_info or {}),
+        **results,
+        **(append_info or {}),
+    }
 
     # list of values
     csv2file(
         target_path=os.path.join(save_path, csv_name),
         thead=list(results.keys()),
         tbody=list(results.values()),
         refresh=False,
```

### Comparing `the_utils-0.4.0/the_utils/plt.py` & `the_utils-0.5.0/the_utils/plt.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     fill_colors: List[str] = None,
     fill_alpha: List[float] or float = 0.5,
     figsize: Tuple = (24, 3),
     xmode: str = "s",
     # pylint: disable=unused-argument
     ymode: str = "s",
     title: str = None,
+    suptitle: str = None,
     set_xticks: bool = False,
     xticks: List[Any] = None,
     tick_labels: List[Any] = None,
     x_rotation: float = 45,
     boxes: List[List[int]] = None,
     box_colors: List[str] = None,
     box_alphas: List[float] = None,
@@ -43,16 +44,16 @@
     linewidth: List[int] = None,
     types: List[str] or str = "line",
     markersize: float = 1.25,
     save_path: str = None,
     bar_width: float = 0.25,
     legend_loc: str = "center left",
     legend_bbox_to_anchor: Tuple[float] = (1, 0.5),
-    x_label=None,
-    y_label=None,
+    x_label: str = None,
+    y_label: str = None,
 ) -> None:
     """Draw charts.
 
     Args:
         ys (List[List]): value lists of the y axis.
         lbls (List[str]): legend labels of the value lists.
         y_colors (List[str], optional): colors of the the ys. Defaults to None.
@@ -65,15 +66,16 @@
         fill_alpha (List[float] or float, optional): color alphas of the fill range. \
             Defaults to 0.5.
         figsize (Tuple, optional): size of the output figure. Defaults to (24, 3).
         xmode (str, optional): all ys with the same x ('s') or with different xs ('d'). \
             Defaults to "s".
         ymode (str, optional): all ys with the same tick ('s') or with different ticks ('d'). \
             Defaults to "s".
-        title (str, optional): figure title. Defaults to None.
+        title (str, optional): add a centered title to the figure. Defaults to None.
+        suptitle (str, optional): add a centered suptitle to the figure. Defaults to None.
         set_xticks (bool, optional): set the x ticks. Defaults to True.
         xticks (List[Any], optional): ticks for the x axis. Defaults to None.
         tick_labels (List[Any], optional): tick labels for the x axis. Defaults to None.
         x_rotation (float, optional): rotation of the x ticks. Defaults to 45.
         boxes (List[List[int]], optional): draw boxes. Defaults to None.
         box_colors (List[str], optional): colors of the boxes to draw. Defaults to None.
         box_alpha (List[float], optional): color alphas of the boxes to draw. Defaults to 0.5.
@@ -251,14 +253,16 @@
                     alpha=box_alphas[idx] if box_alphas is not None else 0.5,
                 )
             )
 
     ax.legend(loc=legend_loc, bbox_to_anchor=legend_bbox_to_anchor)
     if title:
         plt.title(title)
+    if suptitle:
+        plt.suptitle(suptitle)
     if xlim is not None:
         plt.xlim(xlim)
     if ylim is not None:
         plt.ylim(ylim)
     if x_label is not None:
         plt.xlabel(x_label)
     if y_label is not None:
```

### Comparing `the_utils-0.4.0/the_utils/save_load.py` & `the_utils-0.5.0/the_utils/save_load.py`

 * *Files identical despite different names*

### Comparing `the_utils-0.4.0/the_utils/setting.py` & `the_utils-0.5.0/the_utils/setting.py`

 * *Files identical despite different names*

### Comparing `the_utils-0.4.0/the_utils/evaluation/unsupervised_graph_learning.py` & `the_utils-0.5.0/the_utils/evaluation/unsupervised_graph_learning.py`

 * *Files identical despite different names*

### Comparing `the_utils-0.4.0/.gitignore` & `the_utils-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `the_utils-0.4.0/LICENSE` & `the_utils-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `the_utils-0.4.0/README.md` & `the_utils-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `the_utils-0.4.0/pyproject.toml` & `the_utils-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "the_utils"
-version = "0.4.0"
+version = "0.5.0"
 authors = [{ name = "galo.gm", email = "galo.gm.work@gmail.com" }]
 keywords = [""]
 description = ""
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `the_utils-0.4.0/PKG-INFO` & `the_utils-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: the_utils
-Version: 0.4.0
+Version: 0.5.0
 Project-URL: Homepage, https://github.com/galogm/the_utils
 Project-URL: Bug Tracker, https://github.com/galogm/the_utils/issues
 Author-email: "galo.gm" <galo.gm.work@gmail.com>
 License: MIT License
         
         Copyright (c) 2023-present Author
```

