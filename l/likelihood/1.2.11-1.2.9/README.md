# Comparing `tmp/likelihood-1.2.11.tar.gz` & `tmp/likelihood-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "likelihood-1.2.11.tar", last modified: Thu Apr 25 01:20:21 2024, max compression
+gzip compressed data, was "likelihood-1.2.9.tar", last modified: Wed Apr  3 19:41:38 2024, max compression
```

## Comparing `likelihood-1.2.11.tar` & `likelihood-1.2.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:20:21.975709 likelihood-1.2.11/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-25 01:20:14.000000 likelihood-1.2.11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-25 01:20:21.975709 likelihood-1.2.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-25 01:20:14.000000 likelihood-1.2.11/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:20:21.971709 likelihood-1.2.11/likelihood/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-25 01:20:14.000000 likelihood-1.2.11/likelihood/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:20:21.971709 likelihood-1.2.11/likelihood/graph/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-25 01:20:14.000000 likelihood-1.2.11/likelihood/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-25 01:20:14.000000 likelihood-1.2.11/likelihood/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     8591 2024-04-25 01:20:14.000000 likelihood-1.2.11/likelihood/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:20:21.971709 likelihood-1.2.11/likelihood/models/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 01:20:14.000000 likelihood-1.2.11/likelihood/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-04-25 01:20:14.000000 likelihood-1.2.11/likelihood/models/regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-25 01:20:14.000000 likelihood-1.2.11/likelihood/models/simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-25 01:20:14.000000 likelihood-1.2.11/likelihood/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:20:21.975709 likelihood-1.2.11/likelihood/tools/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-25 01:20:14.000000 likelihood-1.2.11/likelihood/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-25 01:20:14.000000 likelihood-1.2.11/likelihood/tools/numeric_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    38594 2024-04-25 01:20:14.000000 likelihood-1.2.11/likelihood/tools/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:20:21.975709 likelihood-1.2.11/likelihood.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-25 01:20:21.000000 likelihood-1.2.11/likelihood.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-25 01:20:21.000000 likelihood-1.2.11/likelihood.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 01:20:21.000000 likelihood-1.2.11/likelihood.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-25 01:20:21.000000 likelihood-1.2.11/likelihood.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-25 01:20:21.000000 likelihood-1.2.11/likelihood.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 01:20:21.975709 likelihood-1.2.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-25 01:20:14.000000 likelihood-1.2.11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:38.250659 likelihood-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-03 19:41:34.000000 likelihood-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-03 19:41:38.250659 likelihood-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-03 19:41:34.000000 likelihood-1.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:38.246659 likelihood-1.2.9/likelihood/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-03 19:41:35.000000 likelihood-1.2.9/likelihood/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:38.246659 likelihood-1.2.9/likelihood/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 19:41:35.000000 likelihood-1.2.9/likelihood/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-03 19:41:35.000000 likelihood-1.2.9/likelihood/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8591 2024-04-03 19:41:35.000000 likelihood-1.2.9/likelihood/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:38.250659 likelihood-1.2.9/likelihood/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-03 19:41:35.000000 likelihood-1.2.9/likelihood/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-04-03 19:41:35.000000 likelihood-1.2.9/likelihood/models/regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-03 19:41:35.000000 likelihood-1.2.9/likelihood/models/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-03 19:41:35.000000 likelihood-1.2.9/likelihood/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:38.250659 likelihood-1.2.9/likelihood/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-03 19:41:35.000000 likelihood-1.2.9/likelihood/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-03 19:41:35.000000 likelihood-1.2.9/likelihood/tools/numeric_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36497 2024-04-03 19:41:35.000000 likelihood-1.2.9/likelihood/tools/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:38.250659 likelihood-1.2.9/likelihood.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-03 19:41:38.000000 likelihood-1.2.9/likelihood.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-03 19:41:38.000000 likelihood-1.2.9/likelihood.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:41:38.000000 likelihood-1.2.9/likelihood.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-03 19:41:38.000000 likelihood-1.2.9/likelihood.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 19:41:38.000000 likelihood-1.2.9/likelihood.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:41:38.250659 likelihood-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-03 19:41:35.000000 likelihood-1.2.9/setup.py
```

### Comparing `likelihood-1.2.11/LICENSE` & `likelihood-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `likelihood-1.2.11/PKG-INFO` & `likelihood-1.2.9/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,22 @@
 Metadata-Version: 2.1
 Name: likelihood
-Version: 1.2.11
+Version: 1.2.9
 Summary: A package that performs the maximum likelihood algorithm.
 Home-page: https://github.com/jzsmoreno/likelihood/
 Author: J. A. Moreno-Guerra
 Author-email: jzs.gm27@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: black[jupyter]==24.1.1
-Requires-Dist: mypy-extensions==1.0.0
-Requires-Dist: types-openpyxl==3.1.0.15
-Requires-Dist: pydocstyle==6.3.0
-Requires-Dist: flake8==6.0.0
-Requires-Dist: isort==5.12.0
-Requires-Dist: mypy==1.4.1
 Requires-Dist: numpy<2.0.0
 Requires-Dist: matplotlib
-Requires-Dist: networkx
-Requires-Dist: pyyaml
-Requires-Dist: pandas
 Requires-Dist: corner
 Requires-Dist: pyvis
 
 ![likelihood](https://raw.githubusercontent.com/RodolfoFerro/likelihood/main/likelihood.png)
 
 ![GitHub last commit](https://img.shields.io/github/last-commit/jzsmoreno/likelihood?style=for-the-badge)
 ![GitHub repo size](https://img.shields.io/github/repo-size/jzsmoreno/likelihood?style=for-the-badge)
```

### Comparing `likelihood-1.2.11/README.md` & `likelihood-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `likelihood-1.2.11/likelihood/graph/graph.py` & `likelihood-1.2.9/likelihood/graph/graph.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-from typing import List
-
-import networkx as nx
 from IPython.display import HTML, display
 from pandas.core.frame import DataFrame
 from pyvis.network import Network
 
 from likelihood.tools import FeatureSelection
 
 
@@ -14,63 +11,40 @@
     def __init__(self, df: DataFrame, n_importances: int, **kwargs):
         self.G = Network(
             notebook=True, cdn_resources="remote", directed=True
         )  # enable interactive visualization in Jupyter Notebooks
         self.df = df
         self.n_importances = n_importances
         super().__init__(**kwargs)
-        self.labels: List[str] = []
 
     def fit(self, **kwargs) -> None:
         """Fit the model according to the given data and parameters."""
         self.get_digraph(self.df, self.n_importances)
         # create a dictionary with the indexes and names of the dataframe
-        self.get_index = dict(zip(self.X.columns, range(len(self.X.columns))))
+        self.get_index = dict(zip(self.df.columns, range(len(self.df.columns))))
         self._make_network()
 
     def _make_network(self) -> None:
         """Create nodes and edges of the network based on feature importance scores"""
         self._add_nodes()
         for i in range(len(self.all_features_imp_graph)):
             node = self.all_features_imp_graph[i][0]
             edges = self.all_features_imp_graph[i][1]
 
             for label, weight in edges:
-                self.G.add_edge(self.get_index[node], self.get_index[label], weight=weight)
+                self.G.add_edge(i, self.get_index[label], weight=weight)
 
     def _add_nodes(self) -> None:
         for i in range(len(self.all_features_imp_graph)):
             node = self.all_features_imp_graph[i][0]
-            self.labels.append(node)
             self.G.add_node(n_id=i, label=node)
 
     def draw(self, name="graph.html", **kwargs) -> None:
         """Display the network using HTML format"""
         spring_length = kwargs["spring_length"] if "spring_length" in kwargs else 500
         node_distance = kwargs["node_distance"] if "node_distance" in kwargs else 100
         self.G.repulsion(node_distance=node_distance, spring_length=spring_length)
         self.G.show_buttons(filter_=["physics"])
         self.G.show(name)
 
         html_file_content = open(name, "r").read()
         display(HTML(html_file_content))
-
-    def pyvis_to_networkx(self):
-        nx_graph = nx.Graph()
-
-        # Adding nodes
-        nodes = [d["id"] for d in self.G.nodes]
-        for node_dic in self.G.nodes:
-            id = node_dic["label"]
-            del node_dic["label"]
-            nx_graph.add_nodes_from([(id, node_dic)])
-        self.node_edge_dict = dict(zip(nodes, self.labels))
-        del nodes
-
-        # Adding edges
-        for edge in self.G.edges:
-            source, target = self.node_edge_dict[edge["from"]], self.node_edge_dict[edge["to"]]
-            del edge["from"]
-            del edge["to"]
-            nx_graph.add_edges_from([(source, target, edge)])
-
-        return nx_graph
```

### Comparing `likelihood-1.2.11/likelihood/main.py` & `likelihood-1.2.9/likelihood/main.py`

 * *Files identical despite different names*

### Comparing `likelihood-1.2.11/likelihood/models/regression.py` & `likelihood-1.2.9/likelihood/models/regression.py`

 * *Files identical despite different names*

### Comparing `likelihood-1.2.11/likelihood/models/simulation.py` & `likelihood-1.2.9/likelihood/models/simulation.py`

 * *Files identical despite different names*

### Comparing `likelihood-1.2.11/likelihood/models/utils.py` & `likelihood-1.2.9/likelihood/models/utils.py`

 * *Files identical despite different names*

### Comparing `likelihood-1.2.11/likelihood/tools/numeric_tools.py` & `likelihood-1.2.9/likelihood/tools/numeric_tools.py`

 * *Files identical despite different names*

### Comparing `likelihood-1.2.11/likelihood/tools/tools.py` & `likelihood-1.2.9/likelihood/tools/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import math
 import os
 import pickle
-from typing import Callable, Dict, List, Tuple
+from typing import Callable, List, Tuple
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-import yaml
 from numpy import ndarray
 from pandas.core.frame import DataFrame
 
 # -------------------------------------------------------------------------
 
 """
 Data Science from Scratch, Second Edition, by Joel Grus (O'Reilly).Copyright 2019 Joel Grus, 978-1-492-04113-9
@@ -90,61 +89,14 @@
     """
     return [partial_difference_quotient(f, v, i, h) for i in range(len(v))]
 
 
 # -------------------------------------------------------------------------
 
 
-def generate_feature_yaml(
-    df: DataFrame, ignore_features: List[str] = None, yaml_string: bool = False
-) -> Dict | str:
-    """
-    Generate a YAML string containing information about ordinal, numeric, and categorical features
-    based on the given DataFrame.
-
-    Args:
-        df (`pd.DataFrame`): The DataFrame containing the data.
-        ignore_features (List[`str`]): A list of features to ignore.
-        yaml_string (`bool`): If `True`, return the result as a YAML formatted string. Otherwise, return it as a dictionary. Default is `False`.
-
-    Returns:
-        `Dict` | `str`: A dictionary with four keys ('ordinal_features', 'numeric_features', 'categorical_features', 'ignore_features')
-        mapping to lists of feature names. Or a YAML formatted string if `yaml_string` is `True`.
-    """
-    feature_info = {
-        "ordinal_features": [],
-        "numeric_features": [],
-        "categorical_features": [],
-        "ignore_features": [],
-    }
-
-    for col in df.columns:
-        if ignore_features and col in ignore_features:
-            continue
-
-        if pd.api.types.is_numeric_dtype(df[col]):
-            feature_info["numeric_features"].append(col)
-        elif pd.api.types.is_object_dtype(df[col]) or pd.api.types.is_categorical_dtype(df[col]):
-            feature_info["categorical_features"].append(col)
-        elif pd.api.types.is_integer_dtype(df[col]):
-            feature_info["ordinal_features"].append(col)
-        elif pd.api.types.is_float_dtype(df[col]):
-            feature_info["ordinal_features"].append(col)
-        elif pd.api.types.is_bool_dtype(df[col]):
-            feature_info["ordinal_features"].append(col)
-        else:
-            print(f"Unknown type for feature {col}")
-        feature_info["ignore_features"] = ignore_features
-
-    if yaml_string:
-        return yaml.dump(feature_info, default_flow_style=False)
-    else:
-        return feature_info
-
-
 # a function that calculates the percentage of missing values per column is defined
 def cal_missing_values(df: DataFrame) -> None:
     col = df.columns
     print("Total size : ", "{:,}".format(len(df)))
     for i in col:
         print(
             str(i) + " : " f"{(df.isnull().sum()[i]/(df.isnull().sum()[i]+df[i].count()))*100:.2f}%"
@@ -927,18 +879,14 @@
                         x = np.where(labels == y_true[j])
                         count_mat[i, x[0]] += 1
 
         return count_mat
 
 
 class OneHotEncoder:
-    """
-    Class used to encode categorical variables.
-    It receives an array of integers and returns a binary array using the one-hot encoding method.
-    """
 
     __slots__ = ["x"]
 
     def __init__(self) -> None:
         pass
 
     def encode(self, x: ndarray | list):
```

### Comparing `likelihood-1.2.11/likelihood.egg-info/PKG-INFO` & `likelihood-1.2.9/likelihood.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,22 @@
 Metadata-Version: 2.1
 Name: likelihood
-Version: 1.2.11
+Version: 1.2.9
 Summary: A package that performs the maximum likelihood algorithm.
 Home-page: https://github.com/jzsmoreno/likelihood/
 Author: J. A. Moreno-Guerra
 Author-email: jzs.gm27@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: black[jupyter]==24.1.1
-Requires-Dist: mypy-extensions==1.0.0
-Requires-Dist: types-openpyxl==3.1.0.15
-Requires-Dist: pydocstyle==6.3.0
-Requires-Dist: flake8==6.0.0
-Requires-Dist: isort==5.12.0
-Requires-Dist: mypy==1.4.1
 Requires-Dist: numpy<2.0.0
 Requires-Dist: matplotlib
-Requires-Dist: networkx
-Requires-Dist: pyyaml
-Requires-Dist: pandas
 Requires-Dist: corner
 Requires-Dist: pyvis
 
 ![likelihood](https://raw.githubusercontent.com/RodolfoFerro/likelihood/main/likelihood.png)
 
 ![GitHub last commit](https://img.shields.io/github/last-commit/jzsmoreno/likelihood?style=for-the-badge)
 ![GitHub repo size](https://img.shields.io/github/repo-size/jzsmoreno/likelihood?style=for-the-badge)
```

### Comparing `likelihood-1.2.11/setup.py` & `likelihood-1.2.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 from pathlib import Path
 
 import setuptools
 
-# Parse the requirements.txt file
-with open("requirements.txt", "r") as f:
-    install_requires = f.read().splitlines()
-
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 about = {}
 ROOT_DIR = Path(__file__).resolve().parent
 PACKAGE_DIR = ROOT_DIR / "likelihood"
 with open(PACKAGE_DIR / "VERSION") as f:
@@ -23,15 +19,20 @@
     author_email="jzs.gm27@gmail.com",
     description="A package that performs the maximum likelihood algorithm.",
     py_modules=["likelihood"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jzsmoreno/likelihood/",
     packages=setuptools.find_packages(),
-    install_requires=install_requires,
+    install_requires=[
+        "numpy<2.0.0",
+        "matplotlib",
+        "corner",
+        "pyvis",
+    ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.10",
 )
```

