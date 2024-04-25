# Comparing `tmp/pyriemann-qiskit-0.1.0.tar.gz` & `tmp/pyriemann_qiskit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyriemann-qiskit-0.1.0.tar", last modified: Thu Oct  5 08:33:37 2023, max compression
+gzip compressed data, was "pyriemann_qiskit-0.2.0.tar", last modified: Thu Apr 25 07:52:26 2024, max compression
```

## Comparing `pyriemann-qiskit-0.1.0.tar` & `pyriemann_qiskit-0.2.0.tar`

### file list

```diff
@@ -1,46 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 08:33:37.156247 pyriemann-qiskit-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2023-10-05 08:33:13.000000 pyriemann-qiskit-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-10-05 08:33:13.000000 pyriemann-qiskit-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13005 2023-10-05 08:33:37.156247 pyriemann-qiskit-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11499 2023-10-05 08:33:13.000000 pyriemann-qiskit-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 08:33:37.148247 pyriemann-qiskit-0.1.0/pyriemann_qiskit/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2023-10-05 08:33:13.000000 pyriemann-qiskit-0.1.0/pyriemann_qiskit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-10-05 08:33:13.000000 pyriemann-qiskit-0.1.0/pyriemann_qiskit/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    23992 2023-10-05 08:33:13.000000 pyriemann-qiskit-0.1.0/pyriemann_qiskit/classification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 08:33:37.152247 pyriemann-qiskit-0.1.0/pyriemann_qiskit/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2023-10-05 08:33:13.000000 pyriemann-qiskit-0.1.0/pyriemann_qiskit/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7674 2023-10-05 08:33:13.000000 pyriemann-qiskit-0.1.0/pyriemann_qiskit/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15020 2023-10-05 08:33:13.000000 pyriemann-qiskit-0.1.0/pyriemann_qiskit/pipelines.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 08:33:37.152247 pyriemann-qiskit-0.1.0/pyriemann_qiskit/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2023-10-05 08:33:13.000000 pyriemann-qiskit-0.1.0/pyriemann_qiskit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2023-10-05 08:33:13.000000 pyriemann-qiskit-0.1.0/pyriemann_qiskit/utils/distance.py
--rw-r--r--   0 runner    (1001) docker     (127)    14088 2023-10-05 08:33:13.000000 pyriemann-qiskit-0.1.0/pyriemann_qiskit/utils/docplex.py
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2023-10-05 08:33:13.000000 pyriemann-qiskit-0.1.0/pyriemann_qiskit/utils/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-10-05 08:33:13.000000 pyriemann-qiskit-0.1.0/pyriemann_qiskit/utils/firebase_cert.py
--rw-r--r--   0 runner    (1001) docker     (127)    12350 2023-10-05 08:33:13.000000 pyriemann-qiskit-0.1.0/pyriemann_qiskit/utils/firebase_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7031 2023-10-05 08:33:13.000000 pyriemann-qiskit-0.1.0/pyriemann_qiskit/utils/hyper_params_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2023-10-05 08:33:13.000000 pyriemann-qiskit-0.1.0/pyriemann_qiskit/utils/math.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2023-10-05 08:33:13.000000 pyriemann-qiskit-0.1.0/pyriemann_qiskit/utils/mean.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2023-10-05 08:33:13.000000 pyriemann-qiskit-0.1.0/pyriemann_qiskit/utils/quantum_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 08:33:37.152247 pyriemann-qiskit-0.1.0/pyriemann_qiskit/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2023-10-05 08:33:13.000000 pyriemann-qiskit-0.1.0/pyriemann_qiskit/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2023-10-05 08:33:13.000000 pyriemann-qiskit-0.1.0/pyriemann_qiskit/visualization/art.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 08:33:37.148247 pyriemann-qiskit-0.1.0/pyriemann_qiskit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13005 2023-10-05 08:33:37.000000 pyriemann-qiskit-0.1.0/pyriemann_qiskit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2023-10-05 08:33:37.000000 pyriemann-qiskit-0.1.0/pyriemann_qiskit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-05 08:33:37.000000 pyriemann-qiskit-0.1.0/pyriemann_qiskit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-05 08:33:36.000000 pyriemann-qiskit-0.1.0/pyriemann_qiskit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      362 2023-10-05 08:33:37.000000 pyriemann-qiskit-0.1.0/pyriemann_qiskit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-10-05 08:33:37.000000 pyriemann-qiskit-0.1.0/pyriemann_qiskit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      234 2023-10-05 08:33:37.156247 pyriemann-qiskit-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2023-10-05 08:33:13.000000 pyriemann-qiskit-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 08:33:37.156247 pyriemann-qiskit-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6709 2023-10-05 08:33:13.000000 pyriemann-qiskit-0.1.0/tests/test_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2023-10-05 08:33:13.000000 pyriemann-qiskit-0.1.0/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2023-10-05 08:33:13.000000 pyriemann-qiskit-0.1.0/tests/test_docplex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2023-10-05 08:33:13.000000 pyriemann-qiskit-0.1.0/tests/test_filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2023-10-05 08:33:13.000000 pyriemann-qiskit-0.1.0/tests/test_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-10-05 08:33:13.000000 pyriemann-qiskit-0.1.0/tests/test_utils_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2023-10-05 08:33:13.000000 pyriemann-qiskit-0.1.0/tests/test_utils_firebase.py
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2023-10-05 08:33:13.000000 pyriemann-qiskit-0.1.0/tests/test_utils_hyper_params_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2023-10-05 08:33:13.000000 pyriemann-qiskit-0.1.0/tests/test_utils_mean.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:52:26.623057 pyriemann_qiskit-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-25 07:52:20.000000 pyriemann_qiskit-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 07:52:20.000000 pyriemann_qiskit-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11576 2024-04-25 07:52:26.623057 pyriemann_qiskit-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-04-25 07:52:20.000000 pyriemann_qiskit-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:52:26.615057 pyriemann_qiskit-0.2.0/pyriemann_qiskit/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-25 07:52:20.000000 pyriemann_qiskit-0.2.0/pyriemann_qiskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 07:52:20.000000 pyriemann_qiskit-0.2.0/pyriemann_qiskit/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37851 2024-04-25 07:52:20.000000 pyriemann_qiskit-0.2.0/pyriemann_qiskit/classification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:52:26.615057 pyriemann_qiskit-0.2.0/pyriemann_qiskit/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-25 07:52:20.000000 pyriemann_qiskit-0.2.0/pyriemann_qiskit/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7574 2024-04-25 07:52:20.000000 pyriemann_qiskit-0.2.0/pyriemann_qiskit/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-04-25 07:52:20.000000 pyriemann_qiskit-0.2.0/pyriemann_qiskit/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17132 2024-04-25 07:52:20.000000 pyriemann_qiskit-0.2.0/pyriemann_qiskit/pipelines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:52:26.619057 pyriemann_qiskit-0.2.0/pyriemann_qiskit/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-25 07:52:20.000000 pyriemann_qiskit-0.2.0/pyriemann_qiskit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-04-25 07:52:20.000000 pyriemann_qiskit-0.2.0/pyriemann_qiskit/utils/distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14634 2024-04-25 07:52:20.000000 pyriemann_qiskit-0.2.0/pyriemann_qiskit/utils/docplex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-25 07:52:20.000000 pyriemann_qiskit-0.2.0/pyriemann_qiskit/utils/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-25 07:52:20.000000 pyriemann_qiskit-0.2.0/pyriemann_qiskit/utils/firebase_cert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12297 2024-04-25 07:52:20.000000 pyriemann_qiskit-0.2.0/pyriemann_qiskit/utils/firebase_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9190 2024-04-25 07:52:20.000000 pyriemann_qiskit-0.2.0/pyriemann_qiskit/utils/hyper_params_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-25 07:52:20.000000 pyriemann_qiskit-0.2.0/pyriemann_qiskit/utils/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-25 07:52:20.000000 pyriemann_qiskit-0.2.0/pyriemann_qiskit/utils/mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-25 07:52:20.000000 pyriemann_qiskit-0.2.0/pyriemann_qiskit/utils/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-25 07:52:20.000000 pyriemann_qiskit-0.2.0/pyriemann_qiskit/utils/quantum_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-25 07:52:20.000000 pyriemann_qiskit-0.2.0/pyriemann_qiskit/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:52:26.619057 pyriemann_qiskit-0.2.0/pyriemann_qiskit/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-25 07:52:20.000000 pyriemann_qiskit-0.2.0/pyriemann_qiskit/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-25 07:52:20.000000 pyriemann_qiskit-0.2.0/pyriemann_qiskit/visualization/art.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-25 07:52:20.000000 pyriemann_qiskit-0.2.0/pyriemann_qiskit/visualization/manifold.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:52:26.619057 pyriemann_qiskit-0.2.0/pyriemann_qiskit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11576 2024-04-25 07:52:26.000000 pyriemann_qiskit-0.2.0/pyriemann_qiskit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-25 07:52:26.000000 pyriemann_qiskit-0.2.0/pyriemann_qiskit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 07:52:26.000000 pyriemann_qiskit-0.2.0/pyriemann_qiskit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 07:52:26.000000 pyriemann_qiskit-0.2.0/pyriemann_qiskit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-25 07:52:26.000000 pyriemann_qiskit-0.2.0/pyriemann_qiskit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-25 07:52:26.000000 pyriemann_qiskit-0.2.0/pyriemann_qiskit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-25 07:52:26.623057 pyriemann_qiskit-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-25 07:52:20.000000 pyriemann_qiskit-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:52:26.619057 pyriemann_qiskit-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-04-25 07:52:20.000000 pyriemann_qiskit-0.2.0/tests/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-25 07:52:20.000000 pyriemann_qiskit-0.2.0/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-25 07:52:20.000000 pyriemann_qiskit-0.2.0/tests/test_docplex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-25 07:52:20.000000 pyriemann_qiskit-0.2.0/tests/test_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-25 07:52:20.000000 pyriemann_qiskit-0.2.0/tests/test_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-25 07:52:20.000000 pyriemann_qiskit-0.2.0/tests/test_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-25 07:52:20.000000 pyriemann_qiskit-0.2.0/tests/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-25 07:52:20.000000 pyriemann_qiskit-0.2.0/tests/test_utils_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-25 07:52:20.000000 pyriemann_qiskit-0.2.0/tests/test_utils_firebase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-04-25 07:52:20.000000 pyriemann_qiskit-0.2.0/tests/test_utils_hyper_params_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-25 07:52:20.000000 pyriemann_qiskit-0.2.0/tests/test_utils_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-04-25 07:52:20.000000 pyriemann_qiskit-0.2.0/tests/test_utils_mean.py
```

### Comparing `pyriemann-qiskit-0.1.0/LICENSE` & `pyriemann_qiskit-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyriemann-qiskit-0.1.0/PKG-INFO` & `pyriemann_qiskit-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,106 +1,118 @@
 Metadata-Version: 2.1
 Name: pyriemann-qiskit
-Version: 0.1.0
+Version: 0.2.0
 Summary: Qiskit wrapper for pyRiemann
 Home-page: https://pyriemann-qiskit.readthedocs.io
 Author: Gregoire Cattan
 Author-email: gcattan@hotmail.com
 License: BSD (3-clause)
 Project-URL: Documentation, https://pyriemann.readthedocs.io
 Project-URL: Source, https://github.com/pyRiemann/pyRiemann-qiskit
 Project-URL: Tracker, https://github.com/pyRiemann/pyRiemann-qiskit/issues/
 Platform: any
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy<1.24
+Requires-Dist: numpy<1.27
 Requires-Dist: cython
 Requires-Dist: pyriemann==0.5
+Requires-Dist: qiskit==0.45.0
 Requires-Dist: qiskit_machine_learning==0.6.1
-Requires-Dist: qiskit-ibm-provider==0.7.0
+Requires-Dist: qiskit-ibm-provider==0.7.3
 Requires-Dist: qiskit-optimization==0.5.0
 Requires-Dist: qiskit-aer==0.12.2
-Requires-Dist: cvxpy==1.3.2
-Requires-Dist: scipy==1.10.1
-Requires-Dist: docplex>=2.21.207
-Requires-Dist: firebase_admin==6.2.0
+Requires-Dist: cvxpy==1.4.2
+Requires-Dist: scipy==1.11.4
+Requires-Dist: docplex==2.25.236
+Requires-Dist: grpcio-status==1.62.1
+Requires-Dist: protobuf==4.25.3
+Requires-Dist: firebase_admin==6.4.0
+Requires-Dist: scikit-learn==1.3.2
 Requires-Dist: tqdm
+Requires-Dist: pandas
 Provides-Extra: docs
 Requires-Dist: sphinx-gallery; extra == "docs"
 Requires-Dist: sphinx-bootstrap_theme; extra == "docs"
 Requires-Dist: numpydoc; extra == "docs"
-Requires-Dist: mne; extra == "docs"
-Requires-Dist: seaborn; extra == "docs"
-Requires-Dist: moabb>=0.4.6; extra == "docs"
+Requires-Dist: mne==1.6.1; extra == "docs"
+Requires-Dist: seaborn>=0.12.1; extra == "docs"
+Requires-Dist: moabb>=1.0.0; extra == "docs"
+Requires-Dist: imbalanced-learn==0.12.0; extra == "docs"
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: seaborn; extra == "tests"
 Requires-Dist: flake8; extra == "tests"
 Requires-Dist: mne; extra == "tests"
 Requires-Dist: pooch; extra == "tests"
 Provides-Extra: optim
 Requires-Dist: qiskit-aer-gpu==0.12.2; extra == "optim"
 
+[<img src=https://github.com/Qiskit/ecosystem/blob/main/badges/pyRiemann-qiskit.svg>](https://qiskit.org/ecosystem)
+
 # pyRiemann-qiskit
 
-Litterature on quantum computing suggests it may offer an advantage as compared with
-classical computing in terms of computational time and outcomes, such as for pattern
-recognition or when using limited training sets [1, 2].
+Literature on quantum computing suggests it may offer an advantage compared with classical
+computing in terms of computational time and outcomes, such as for pattern recognition or
+when using limited training sets [1, 2].
 
 A ubiquitous library on quantum computing is Qiskit [3]. Qiskit is an IBM library
 distributed under Apache 2.0 which provides both quantum algorithms and backends. A
-backend can be either your local machine or a remote machine, which one can emulates or be
-a quantum machine. Qiskit abstraction over the type of machine you want to use, make
-designing quantum algorithm seamless.
-
-Qiskit implements a quantum version of support vector -like classifiers, known as
-quantum-enhanced support vector classifier (QSVC) and varitional quantum classifier (VQC)
-[4]. These classifiers likely offer an advantage over classical SVM in situations where
-the classification task is complex. Task complexity is raised by the encoding of the data
-into a quantum state, the number of available data and the quality of the data. An initial
-study is available in [5], and it can be downloaded from
+backend can be either your local machine or a remote machine, which one can emulate or be
+a quantum machine. Qiskit abstraction over the type of machine you want to use, makes
+designing quantum algorithms seamless.
+
+Qiskit implements a quantum version of support vector-like classifiers, known as
+quantum-enhanced support vector classifiers (QSVCs) and variational quantum classifiers
+(VQCs) [4]. These classifiers likely offer an advantage over classical SVM in situations
+where the classification task is complex. Task complexity is raised by the encoding of the
+data into a quantum state, the number of available data, and the quality of the data. An
+initial study is available in [5], and it can be downloaded from
 [here](doc/Presentations/QuantumERPClassification.pdf). Although there is no study on this
-topic at the time of writting, this could be an interesting research direction to
+topic at the time of writing, this could be an interesting research direction to
 investigate BCI illiteracy.
 
-pyRiemann-qiskit implements a wrapper around QSVC and VQC, to use quantum classification
+`pyRiemann-qiskit` implements a wrapper around QSVC and VQC, to use quantum classification
 with Riemannian geometry. A use case would be to use vectorized covariance matrices in the
 tangent space as an input for these classifiers, enabling a possible sandbox for
 researchers and engineers in the field.
 
-The remaining details some of the quantum drawbacks and will guide you through
-installation. Full documentation, including API description, is available at
+`pyRiemann-qiskit` also introduces a quantum version of the famous MDM algorithm. There is
+a dedicated example on quantum-MDM
+[here](https://github.com/pyRiemann/pyRiemann-qiskit/blob/main/examples/ERP/classify_P300_bi_quantum_mdm.py).
+
+The remaining of this readme details some of the quantum drawbacks and will guide you
+through installation. Full documentation, including API description, is available at
 <https://pyriemann-qiskit.readthedocs.io/>. The repository also includes a
 [wiki](https://github.com/pyRiemann/pyRiemann-qiskit/wiki) where you can find additional
 information.
 
 ## Quantum drawbacks
 
 - Limitation of the feature dimension
 
   The number of qubits (and therefore the feature dimension) is limited to:
 
-  - 24 on a local quantum simulator, and up to:
+  - ~36 (depends on system memory size) on a local quantum simulator, and up to:
   - 5000 on a remote quantum simulator;
-  - 5 on free real quantum computers, and up to:
-  - 65 on exploratory quantum computers (not available for public use).
+  - 7 on free real quantum computers, and up to:
+  - 127 on exploratory quantum computers (not available for public use).
 
 - Time complexity
 
-  A higher number of trials or dimension increases time to completion of the quantum
+  A higher number of trials or dimensions increases the time to completion of the quantum
   algorithm, especially when running on a local machine. This is why the number of trials
   is limited in the examples we provided. However, you should avoid such practices in your
   own analysis.
 
   Although these aspects are less important in a remote backend, it may happen that the
   quantum algorithm is queued depending on the number of concurrent users.
 
-  For all these aspects, the use of pyRiemann-qiskit should be limited to offline analysis
-  only.
+  For all these aspects, the use of `pyRiemann-qiskit` should be limited to offline
+  analysis only.
 
 ## References
 
 [1] A. Blance and M. Spannowsky, ‘Quantum machine learning for particle physics using a
 variational quantum classifier’, J. High Energ. Phys., vol. 2021, no. 2, p. 212, Feb.
 2021, https://doi.org/10.1007/JHEP02(2021)212
 
@@ -118,39 +130,37 @@
 [5] G. Cattan, A. Andreev, First steps to the classification of ERPs using quantum
 computation, NTB Berlin 2022 - International Forum on Neural Engineering & Brain
 Technologies, May 2022, Berlin, Germany, https://hal.archives-ouvertes.fr/hal-03672246/
 
 ### How to cite?
 
 Anton Andreev, Grégoire Cattan, Sylvain Chevallier, and Quentin Barthélemy.
-‘PyRiemann-Qiskit: A Sandbox for Quantum Classification Experiments with Riemannian
+‘pyRiemann-qiskit: A Sandbox for Quantum Classification Experiments with Riemannian
 Geometry’. Research Ideas and Outcomes 9 (20 March 2023).
 https://doi.org/10.3897/rio.9.e101006.
 
+This library is part of the [Qiskit Ecosystem](https://qiskit.org/ecosystem)
+
 ## Installation
 
 _We recommend the use of [Anaconda](https://www.anaconda.com/) to manage python
 environements._
 
-`pyRiemann-qiskit` currently supports Windows, Mac and Linux OS with Python 3.8 and 3.9.
+`pyRiemann-qiskit` currently supports Windows, Mac and Linux OS with **Python 3.9 -
+3.11**.
 
 You can install `pyRiemann-qiskit` release from PyPI:
 
 ```
 pip install pyriemann-qiskit
 ```
 
 The development version can be installed by cloning this repository and installing the
-package on your local machine using the `setup.py` script:
-
-```
-python setup.py develop
-```
-
-Or directly pip:
+package on your local machine using the `setup.py` script. We recommand to do it using
+`pip`:
 
 ```
 pip install .
 ```
 
 Note that the steps above need to be re-executed in your local environment after any
 changes inside your local copy of the `pyriemann_qiskit` folder, including pulling from
@@ -196,22 +206,22 @@
 Wait for the container to build, and open a python shell within the container. Then ensure
 everything went smoothly by typing:
 
 ```
 import pyriemann_qiskit
 ```
 
-Alternatively you can from the console (Windows or Linux) build the docker image from our
-Dockerfile. Go to the root folder of pyRiemann-qiskit and type:
+Alternatively, you can from the console (Windows or Linux) build the docker image from our
+Dockerfile. Go to the root folder of `pyRiemann-qiskit` and type:
 
 ```
 docker build -t pyrq .
 ```
 
-Next use `docker run --detach pyrq` to enter the pyRiemann-qiskit image.
+Next use `docker run --detach pyrq` to enter the `pyRiemann-qiskit` image.
 
 If you wish, you can also download docker images directly from github docker registry:
 https://github.com/pyRiemann/pyRiemann-qiskit/pkgs/container/pyriemann-qiskit
 
 They are pushed to the docker registry on each release.
 
 ## Contributor Guidelines
@@ -268,42 +278,9 @@
   [Github Actions](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/enabling-features-for-your-repository/managing-github-actions-settings-for-a-repository)
   in your fork to see the result of the CI pipeline. Results are also indicated at the end
   of your pull request when raised. However note, that workflows in the pull request need
   approval from the maintainers before being executed.
 
 # Troubleshooting
 
-## Version of pyRiemann not updated
-
-There is a known issue when you install `pyRiemann-qiskit` in an environement where there
-is already `pyRiemann` installed. In such case, the `pyRiemann` version is not updated.
-Therefore before installing or updating `pyRiemann-qiskit`, we recommend to install
-`pyRiemann` as it follows:
-
-```
-pip uninstall pyriemann
-pip install pyriemann@git+https://github.com/pyRiemann/pyRiemann#egg=pyriemann
-```
-
-## Firebase admin not loading
-
-In some environment, the firebase admin module is not loaded. There is two reasons:
-
-1. The protobuf package is missing an `__init__.py` file. You can fix this issue by adding
-   it manually as it is done in the DockerFile:
-
-```
-touch /usr/local/lib/python3.8/site-packages/protobuf-4.22.1-py3.8-linux-x86_64.egg/google/__init__.py
-```
-
-2. The Firestore service contains unused dependency to `google.cloud.location`. You can
-   fix this issue by removing the dependencies manually, as it is done in the DockerFile
-   too:
-
-```
-sed -i 's/from google.cloud.location import locations_pb2//g' '/usr/local/lib/python3.8/site-packages/google_cloud_firestore-2.10.1-py3.8.egg/google/cloud/firestore_v1/services/firestore/client.py'
-sed -i 's/from google.cloud.location import locations_pb2//g' '/usr/local/lib/python3.8/site-packages/google_cloud_firestore-2.10.1-py3.8.egg/google/cloud/firestore_v1/services/firestore/transports/base.py'
-sed -i 's/from google.cloud.location import locations_pb2//g' '/usr/local/lib/python3.8/site-packages/google_cloud_firestore-2.10.1-py3.8.egg/google/cloud/firestore_v1/services/firestore/transports/grpc.py'
-sed -i 's/from google.cloud.location import locations_pb2//g' '/usr/local/lib/python3.8/site-packages/google_cloud_firestore-2.10.1-py3.8.egg/google/cloud/firestore_v1/services/firestore/transports/grpc_asyncio.py'
-sed -i 's/from google.cloud.location import locations_pb2//g' '/usr/local/lib/python3.8/site-packages/google_cloud_firestore-2.10.1-py3.8.egg/google/cloud/firestore_v1/services/firestore/transports/rest.py'
-sed -i 's/from google.cloud.location import locations_pb2//g' '/usr/local/lib/python3.8/site-packages/google_cloud_firestore-2.10.1-py3.8.egg/google/cloud/firestore_v1/services/firestore/async_client.py'
-```
+See our [dedicated](https://github.com/pyRiemann/pyRiemann-qiskit/wiki/Troubleshooting)
+wiki page.
```

### Comparing `pyriemann-qiskit-0.1.0/README.md` & `pyriemann_qiskit-0.2.0/pyriemann_qiskit.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,63 +1,118 @@
+Metadata-Version: 2.1
+Name: pyriemann-qiskit
+Version: 0.2.0
+Summary: Qiskit wrapper for pyRiemann
+Home-page: https://pyriemann-qiskit.readthedocs.io
+Author: Gregoire Cattan
+Author-email: gcattan@hotmail.com
+License: BSD (3-clause)
+Project-URL: Documentation, https://pyriemann.readthedocs.io
+Project-URL: Source, https://github.com/pyRiemann/pyRiemann-qiskit
+Project-URL: Tracker, https://github.com/pyRiemann/pyRiemann-qiskit/issues/
+Platform: any
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy<1.27
+Requires-Dist: cython
+Requires-Dist: pyriemann==0.5
+Requires-Dist: qiskit==0.45.0
+Requires-Dist: qiskit_machine_learning==0.6.1
+Requires-Dist: qiskit-ibm-provider==0.7.3
+Requires-Dist: qiskit-optimization==0.5.0
+Requires-Dist: qiskit-aer==0.12.2
+Requires-Dist: cvxpy==1.4.2
+Requires-Dist: scipy==1.11.4
+Requires-Dist: docplex==2.25.236
+Requires-Dist: grpcio-status==1.62.1
+Requires-Dist: protobuf==4.25.3
+Requires-Dist: firebase_admin==6.4.0
+Requires-Dist: scikit-learn==1.3.2
+Requires-Dist: tqdm
+Requires-Dist: pandas
+Provides-Extra: docs
+Requires-Dist: sphinx-gallery; extra == "docs"
+Requires-Dist: sphinx-bootstrap_theme; extra == "docs"
+Requires-Dist: numpydoc; extra == "docs"
+Requires-Dist: mne==1.6.1; extra == "docs"
+Requires-Dist: seaborn>=0.12.1; extra == "docs"
+Requires-Dist: moabb>=1.0.0; extra == "docs"
+Requires-Dist: imbalanced-learn==0.12.0; extra == "docs"
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: seaborn; extra == "tests"
+Requires-Dist: flake8; extra == "tests"
+Requires-Dist: mne; extra == "tests"
+Requires-Dist: pooch; extra == "tests"
+Provides-Extra: optim
+Requires-Dist: qiskit-aer-gpu==0.12.2; extra == "optim"
+
+[<img src=https://github.com/Qiskit/ecosystem/blob/main/badges/pyRiemann-qiskit.svg>](https://qiskit.org/ecosystem)
+
 # pyRiemann-qiskit
 
-Litterature on quantum computing suggests it may offer an advantage as compared with
-classical computing in terms of computational time and outcomes, such as for pattern
-recognition or when using limited training sets [1, 2].
+Literature on quantum computing suggests it may offer an advantage compared with classical
+computing in terms of computational time and outcomes, such as for pattern recognition or
+when using limited training sets [1, 2].
 
 A ubiquitous library on quantum computing is Qiskit [3]. Qiskit is an IBM library
 distributed under Apache 2.0 which provides both quantum algorithms and backends. A
-backend can be either your local machine or a remote machine, which one can emulates or be
-a quantum machine. Qiskit abstraction over the type of machine you want to use, make
-designing quantum algorithm seamless.
-
-Qiskit implements a quantum version of support vector -like classifiers, known as
-quantum-enhanced support vector classifier (QSVC) and varitional quantum classifier (VQC)
-[4]. These classifiers likely offer an advantage over classical SVM in situations where
-the classification task is complex. Task complexity is raised by the encoding of the data
-into a quantum state, the number of available data and the quality of the data. An initial
-study is available in [5], and it can be downloaded from
+backend can be either your local machine or a remote machine, which one can emulate or be
+a quantum machine. Qiskit abstraction over the type of machine you want to use, makes
+designing quantum algorithms seamless.
+
+Qiskit implements a quantum version of support vector-like classifiers, known as
+quantum-enhanced support vector classifiers (QSVCs) and variational quantum classifiers
+(VQCs) [4]. These classifiers likely offer an advantage over classical SVM in situations
+where the classification task is complex. Task complexity is raised by the encoding of the
+data into a quantum state, the number of available data, and the quality of the data. An
+initial study is available in [5], and it can be downloaded from
 [here](doc/Presentations/QuantumERPClassification.pdf). Although there is no study on this
-topic at the time of writting, this could be an interesting research direction to
+topic at the time of writing, this could be an interesting research direction to
 investigate BCI illiteracy.
 
-pyRiemann-qiskit implements a wrapper around QSVC and VQC, to use quantum classification
+`pyRiemann-qiskit` implements a wrapper around QSVC and VQC, to use quantum classification
 with Riemannian geometry. A use case would be to use vectorized covariance matrices in the
 tangent space as an input for these classifiers, enabling a possible sandbox for
 researchers and engineers in the field.
 
-The remaining details some of the quantum drawbacks and will guide you through
-installation. Full documentation, including API description, is available at
+`pyRiemann-qiskit` also introduces a quantum version of the famous MDM algorithm. There is
+a dedicated example on quantum-MDM
+[here](https://github.com/pyRiemann/pyRiemann-qiskit/blob/main/examples/ERP/classify_P300_bi_quantum_mdm.py).
+
+The remaining of this readme details some of the quantum drawbacks and will guide you
+through installation. Full documentation, including API description, is available at
 <https://pyriemann-qiskit.readthedocs.io/>. The repository also includes a
 [wiki](https://github.com/pyRiemann/pyRiemann-qiskit/wiki) where you can find additional
 information.
 
 ## Quantum drawbacks
 
 - Limitation of the feature dimension
 
   The number of qubits (and therefore the feature dimension) is limited to:
 
-  - 24 on a local quantum simulator, and up to:
+  - ~36 (depends on system memory size) on a local quantum simulator, and up to:
   - 5000 on a remote quantum simulator;
-  - 5 on free real quantum computers, and up to:
-  - 65 on exploratory quantum computers (not available for public use).
+  - 7 on free real quantum computers, and up to:
+  - 127 on exploratory quantum computers (not available for public use).
 
 - Time complexity
 
-  A higher number of trials or dimension increases time to completion of the quantum
+  A higher number of trials or dimensions increases the time to completion of the quantum
   algorithm, especially when running on a local machine. This is why the number of trials
   is limited in the examples we provided. However, you should avoid such practices in your
   own analysis.
 
   Although these aspects are less important in a remote backend, it may happen that the
   quantum algorithm is queued depending on the number of concurrent users.
 
-  For all these aspects, the use of pyRiemann-qiskit should be limited to offline analysis
-  only.
+  For all these aspects, the use of `pyRiemann-qiskit` should be limited to offline
+  analysis only.
 
 ## References
 
 [1] A. Blance and M. Spannowsky, ‘Quantum machine learning for particle physics using a
 variational quantum classifier’, J. High Energ. Phys., vol. 2021, no. 2, p. 212, Feb.
 2021, https://doi.org/10.1007/JHEP02(2021)212
 
@@ -75,39 +130,37 @@
 [5] G. Cattan, A. Andreev, First steps to the classification of ERPs using quantum
 computation, NTB Berlin 2022 - International Forum on Neural Engineering & Brain
 Technologies, May 2022, Berlin, Germany, https://hal.archives-ouvertes.fr/hal-03672246/
 
 ### How to cite?
 
 Anton Andreev, Grégoire Cattan, Sylvain Chevallier, and Quentin Barthélemy.
-‘PyRiemann-Qiskit: A Sandbox for Quantum Classification Experiments with Riemannian
+‘pyRiemann-qiskit: A Sandbox for Quantum Classification Experiments with Riemannian
 Geometry’. Research Ideas and Outcomes 9 (20 March 2023).
 https://doi.org/10.3897/rio.9.e101006.
 
+This library is part of the [Qiskit Ecosystem](https://qiskit.org/ecosystem)
+
 ## Installation
 
 _We recommend the use of [Anaconda](https://www.anaconda.com/) to manage python
 environements._
 
-`pyRiemann-qiskit` currently supports Windows, Mac and Linux OS with Python 3.8 and 3.9.
+`pyRiemann-qiskit` currently supports Windows, Mac and Linux OS with **Python 3.9 -
+3.11**.
 
 You can install `pyRiemann-qiskit` release from PyPI:
 
 ```
 pip install pyriemann-qiskit
 ```
 
 The development version can be installed by cloning this repository and installing the
-package on your local machine using the `setup.py` script:
-
-```
-python setup.py develop
-```
-
-Or directly pip:
+package on your local machine using the `setup.py` script. We recommand to do it using
+`pip`:
 
 ```
 pip install .
 ```
 
 Note that the steps above need to be re-executed in your local environment after any
 changes inside your local copy of the `pyriemann_qiskit` folder, including pulling from
@@ -153,22 +206,22 @@
 Wait for the container to build, and open a python shell within the container. Then ensure
 everything went smoothly by typing:
 
 ```
 import pyriemann_qiskit
 ```
 
-Alternatively you can from the console (Windows or Linux) build the docker image from our
-Dockerfile. Go to the root folder of pyRiemann-qiskit and type:
+Alternatively, you can from the console (Windows or Linux) build the docker image from our
+Dockerfile. Go to the root folder of `pyRiemann-qiskit` and type:
 
 ```
 docker build -t pyrq .
 ```
 
-Next use `docker run --detach pyrq` to enter the pyRiemann-qiskit image.
+Next use `docker run --detach pyrq` to enter the `pyRiemann-qiskit` image.
 
 If you wish, you can also download docker images directly from github docker registry:
 https://github.com/pyRiemann/pyRiemann-qiskit/pkgs/container/pyriemann-qiskit
 
 They are pushed to the docker registry on each release.
 
 ## Contributor Guidelines
@@ -225,42 +278,9 @@
   [Github Actions](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/enabling-features-for-your-repository/managing-github-actions-settings-for-a-repository)
   in your fork to see the result of the CI pipeline. Results are also indicated at the end
   of your pull request when raised. However note, that workflows in the pull request need
   approval from the maintainers before being executed.
 
 # Troubleshooting
 
-## Version of pyRiemann not updated
-
-There is a known issue when you install `pyRiemann-qiskit` in an environement where there
-is already `pyRiemann` installed. In such case, the `pyRiemann` version is not updated.
-Therefore before installing or updating `pyRiemann-qiskit`, we recommend to install
-`pyRiemann` as it follows:
-
-```
-pip uninstall pyriemann
-pip install pyriemann@git+https://github.com/pyRiemann/pyRiemann#egg=pyriemann
-```
-
-## Firebase admin not loading
-
-In some environment, the firebase admin module is not loaded. There is two reasons:
-
-1. The protobuf package is missing an `__init__.py` file. You can fix this issue by adding
-   it manually as it is done in the DockerFile:
-
-```
-touch /usr/local/lib/python3.8/site-packages/protobuf-4.22.1-py3.8-linux-x86_64.egg/google/__init__.py
-```
-
-2. The Firestore service contains unused dependency to `google.cloud.location`. You can
-   fix this issue by removing the dependencies manually, as it is done in the DockerFile
-   too:
-
-```
-sed -i 's/from google.cloud.location import locations_pb2//g' '/usr/local/lib/python3.8/site-packages/google_cloud_firestore-2.10.1-py3.8.egg/google/cloud/firestore_v1/services/firestore/client.py'
-sed -i 's/from google.cloud.location import locations_pb2//g' '/usr/local/lib/python3.8/site-packages/google_cloud_firestore-2.10.1-py3.8.egg/google/cloud/firestore_v1/services/firestore/transports/base.py'
-sed -i 's/from google.cloud.location import locations_pb2//g' '/usr/local/lib/python3.8/site-packages/google_cloud_firestore-2.10.1-py3.8.egg/google/cloud/firestore_v1/services/firestore/transports/grpc.py'
-sed -i 's/from google.cloud.location import locations_pb2//g' '/usr/local/lib/python3.8/site-packages/google_cloud_firestore-2.10.1-py3.8.egg/google/cloud/firestore_v1/services/firestore/transports/grpc_asyncio.py'
-sed -i 's/from google.cloud.location import locations_pb2//g' '/usr/local/lib/python3.8/site-packages/google_cloud_firestore-2.10.1-py3.8.egg/google/cloud/firestore_v1/services/firestore/transports/rest.py'
-sed -i 's/from google.cloud.location import locations_pb2//g' '/usr/local/lib/python3.8/site-packages/google_cloud_firestore-2.10.1-py3.8.egg/google/cloud/firestore_v1/services/firestore/async_client.py'
-```
+See our [dedicated](https://github.com/pyRiemann/pyRiemann-qiskit/wiki/Troubleshooting)
+wiki page.
```

### Comparing `pyriemann-qiskit-0.1.0/pyriemann_qiskit/datasets/utils.py` & `pyriemann_qiskit-0.2.0/pyriemann_qiskit/datasets/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,37 +10,36 @@
 except Exception:
     warn("mne not available. get_mne_sample will fail.")
 from qiskit_machine_learning.datasets import ad_hoc_data
 from sklearn.datasets import make_classification
 
 
 def get_mne_sample(n_trials=10, include_auditory=False):
-    """Return sample data from the mne dataset.
+    """Return sample data from the MNE dataset.
 
-    ```
+    ``
     In this experiment, checkerboard patterns were presented to the subject
     into the left and right visual field, interspersed by tones to the
     left or right ear. The interval between the stimuli was 750 ms.
     Occasionally a smiley face was presented at the center of the visual field.
     The subject was asked to press a key with the right index finger
     as soon as possible after the appearance of the face.
-    ``` [1]_
+    `` [1]_
 
     The samples returned by this method are epochs of duration 1s.
     Only visual left and right trials are selected.
     Data are returned filtered.
 
     Parameters
     ----------
     n_trials : int (default:10)
         Number of trials to return.
         If -1, then all trials are returned.
     include_auditory : boolean (default:False)
-        If True, it returns also the auditory stimulation
-        in the MNE dataset.
+        If True, it returns also the auditory stimulation in the MNE dataset.
 
     Returns
     -------
     X : ndarray, shape (n_trials, n_channels, n_times)
         ndarray of trials.
     y : ndarray, shape (n_trials,)
         Predicted target vector relative to X.
@@ -232,27 +231,20 @@
         The number of subjects in the dataset.
         A dataset will be generated for all subjects using the handler
         `dataset_gen`.
 
     Attributes
     ----------
     code_ : str
-        The code of the dataset.
-        The code of the dataset is also the string representation
+        The code of the dataset, which is also the string representation
         of the dataset.
-    data_ : Dict
-        A dictionnary representing the dataset. Ex:
-        ```
-        {
-            subject1: (samples1, labels1),
-            subject2: (samples2, labels2),
-            ...
-        }
-        ```
-    subjects_ : List[int]
+    data_ : dict
+        A dictionnary representing the dataset, e.g.:
+        ``{subject1: (samples1, labels1), subject2: (samples2, labels2), ...}``
+    subjects_ : list[int]
         The subjects of the dataset.
 
     Notes
     -----
     .. versionadded:: 0.0.3
 
     """
```

### Comparing `pyriemann-qiskit-0.1.0/pyriemann_qiskit/pipelines.py` & `pyriemann_qiskit-0.2.0/pyriemann_qiskit/pipelines.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 """Module for pipelines."""
 import numpy as np
 from sklearn.base import BaseEstimator, ClassifierMixin, TransformerMixin
 from sklearn.decomposition import PCA
-from sklearn.pipeline import make_pipeline
+from sklearn.discriminant_analysis import LinearDiscriminantAnalysis as LDA
+from sklearn.pipeline import make_pipeline, FeatureUnion
 from sklearn.ensemble import VotingClassifier
+from qiskit_optimization.algorithms import CobylaOptimizer
 from pyriemann.estimation import XdawnCovariances, ERPCovariances
 from pyriemann.tangentspace import TangentSpace
 from pyriemann.preprocessing import Whitening
+from pyriemann.classification import MDM
+from pyriemann_qiskit.utils.utils import is_qfunction
 from pyriemann_qiskit.utils.filtering import NoDimRed
 from pyriemann_qiskit.utils.hyper_params_factory import (
-    gen_zz_feature_map,
+    # gen_zz_feature_map,
+    gen_x_feature_map,
     gen_two_local,
     get_spsa,
 )
-from pyriemann_qiskit.classification import QuanticVQC, QuanticSVM, QuanticMDM
+from pyriemann_qiskit.classification import (
+    QuanticNCH,
+    QuanticVQC,
+    QuanticSVM,
+    QuanticMDM,
+)
 
 
 class BasePipeline(BaseEstimator, ClassifierMixin, TransformerMixin):
 
-    """Base class for quantum classifiers with riemannian pipeline.
+    """Base class for quantum classifiers with Riemannian pipeline.
 
     Parameters
     ----------
     code: string
         Identifier of the pipeline (for log purposes).
 
     Attributes
@@ -45,15 +55,15 @@
         raise NotImplementedError()
 
     def _log(self, trace):
         if self.verbose:
             print("[" + self.code + "] ", trace)
 
     def fit(self, X, y):
-        """Train the riemann quantum classifier.
+        """Train the Riemannian quantum classifier.
 
         Parameters
         ----------
         X : ndarray, shape (n_trials, n_channels, n_times)
             ndarray of trials.
         y : ndarray, shape (n_samples,)
             Target vector relative to X.
@@ -66,14 +76,15 @@
 
         self.classes_ = np.unique(y)
         self._pipe.fit(X, y)
         return self
 
     def score(self, X, y):
         """Return the accuracy.
+
         You might want to use a different metric by using sklearn
         cross_val_score
 
         Parameters
         ----------
         X : ndarray, shape (n_trials, n_channels, n_times)
             ndarray of trials.
@@ -135,32 +146,32 @@
             `n_filter` and `dim_red`.
         """
         return self._pipe.transform(X)
 
 
 class QuantumClassifierWithDefaultRiemannianPipeline(BasePipeline):
 
-    """Default pipeline with Riemann Geometry and a quantum classifier.
+    """Default pipeline with Riemannian geometry and a quantum classifier.
 
     Projects the data into the tangent space of the Riemannian manifold
     and applies quantum classification.
 
     The type of quantum classification (quantum SVM or VQC) depends on
     the value of the parameters.
 
     Data are entangled using a ZZFeatureMap. A SPSA optimizer and a two-local
     circuits are used in addition when the VQC is selected.
 
-
-
     Parameters
     ----------
     nfilter : int (default: 1)
         The number of filter for the xDawnFilter.
         The number of components selected is 2 x nfilter.
+    classes: list[int] (default: None)
+        Classes for the XdawnCovariances.
     dim_red : TransformerMixin (default: PCA())
         A transformer that will reduce the dimension of the feature,
         after the data are projected into the tangent space.
     gamma : float | None (default:None)
         Used as input for sklearn rbf_kernel which is used internally.
         See [1]_ for more information about gamma.
     C : float (default: 1.0)
@@ -172,51 +183,48 @@
         number of steps in Pegasos or SVC.
         If None, respective default values for Pegasos and (Q)SVC
         are used. The default value for Pegasos is 1000.
         For (Q)SVC it is -1 (that is no limit).
     shots : int | None (default: 1024)
         Number of repetitions of each circuit, for sampling.
         If None, classical computation will be performed.
-    feature_entanglement : str | list[list[list[int]]] | \
-                   Callable[int, list[list[list[int]]]]
-        Specifies the entanglement structure for the ZZFeatureMap.
-        Entanglement structure can be provided with indices or string.
-        Possible string values are: 'full', 'linear', 'circular' and 'sca'.
-        Consult [2]_ for more details on entanglement structure.
     feature_reps : int (default: 2)
-        The number of repeated circuits for the ZZFeatureMap,
+        The number of repeated circuits for the FeatureMap,
         greater or equal to 1.
     spsa_trials : int (default: None)
         Maximum number of iterations to perform using SPSA optimizer.
         For VQC, you can use 40 as a default.
         VQC is only enabled if spsa_trials and two_local_reps are not None.
     two_local_reps : int (default: None)
         The number of repetition for the two-local cricuit.
         VQC is only enabled if spsa_trials and two_local_reps are not None.
         For VQC, you can use 3 as a default.
-    params: Dict (default: {})
+    params: dict (default: {})
         Additional parameters to pass to the nested instance
         of the quantum classifier.
         See QuanticClassifierBase, QuanticVQC and QuanticSVM for
         a complete list of the parameters.
 
     Attributes
     ----------
     classes_ : list
         list of classes.
 
     Notes
     -----
     .. versionadded:: 0.0.1
+    .. versionchanged:: 0.2.0
+        Changed feature map from ZZFeatureMap to XFeatureMap.
+        Therefore remove unused parameter `feature_entanglement`.
 
     See Also
     --------
     XdawnCovariances
     TangentSpace
-    gen_zz_feature_map
+    gen_x_feature_map
     gen_two_local
     get_spsa
     QuanticVQC
     QuanticSVM
     QuanticClassifierBase
 
     References
@@ -228,45 +236,49 @@
         https://qiskit.org/documentation/stable/0.36/stubs/qiskit.circuit.library.NLocal.html
 
     """
 
     def __init__(
         self,
         nfilter=1,
+        classes=None,
         dim_red=PCA(),
         gamma="scale",
         C=1.0,
         max_iter=None,
         shots=1024,
-        feature_entanglement="full",
         feature_reps=2,
         spsa_trials=None,
         two_local_reps=None,
         params={},
     ):
         self.nfilter = nfilter
+        self.classes = classes
         self.dim_red = dim_red
         self.gamma = gamma
         self.C = C
         self.max_iter = max_iter
         self.shots = shots
-        self.feature_entanglement = feature_entanglement
         self.feature_reps = feature_reps
         self.spsa_trials = spsa_trials
         self.two_local_reps = two_local_reps
         self.params = params
         # verbose is passed as an additional parameter to quantum classifiers.
         self.verbose = "verbose" in self.params and self.params["verbose"]
         BasePipeline.__init__(self, "QuantumClassifierWithDefaultRiemannianPipeline")
 
     def _create_pipe(self):
         is_vqc = self.spsa_trials and self.two_local_reps
         is_quantum = self.shots is not None
 
-        feature_map = gen_zz_feature_map(self.feature_reps, self.feature_entanglement)
+        # Different feature maps can be used.
+        # Currently the best results are produced by the x_feature_map.
+        # This can change in the future as the code for the different feature maps
+        # is updated in the new versions of Qiskit.
+        feature_map = gen_x_feature_map(self.feature_reps)
 
         if is_vqc:
             self._log("QuanticVQC chosen.")
             clf = QuanticVQC(
                 optimizer=get_spsa(self.spsa_trials),
                 gen_var_form=gen_two_local(self.two_local_reps),
                 gen_feature_map=feature_map,
@@ -283,138 +295,158 @@
                 max_iter=self.max_iter,
                 gen_feature_map=feature_map,
                 shots=self.shots,
                 **self.params
             )
 
         return make_pipeline(
-            XdawnCovariances(nfilter=self.nfilter), TangentSpace(), self.dim_red, clf
+            XdawnCovariances(
+                nfilter=self.nfilter,
+                classes=self.classes,
+                estimator="scm",
+                xdawn_estimator="lwf",
+            ),
+            TangentSpace(),
+            self.dim_red,
+            clf,
         )
 
 
 class QuantumMDMWithRiemannianPipeline(BasePipeline):
 
-    """MDM with riemannian pipeline adapted for convex metrics.
-    It can run on classical or quantum optimizer.
+    """MDM with Riemannian pipeline adapted for cpm metrics.
 
+    It can run on classical or quantum optimizer.
 
     Parameters
     ----------
-    convex_metric : string (default: "distance")
-        `metric` passed to the inner QuanticMDM depends on the
-        `convex_metric` as follows (convex_metric => metric):
-        - "distance" => {mean=logeuclid, distance=convex}
-        - "mean" => {mean=convex, distance=euclid}
-        - "both" => {mean=convex, distance=convex}
-        - other => same as "distance"
+    metric : string | dict, default={"mean": 'logeuclid', "distance": 'qlogeuclid'}
+        The type of metric used for centroid and distance estimation.
     quantum : bool (default: True)
         - If true will run on local or remote backend
-        (depending on q_account_token value).
-        - If false, will perform classical computing instead
+          (depending on q_account_token value),
+        - If false, will perform classical computing instead.
     q_account_token : string (default:None)
-        If quantum==True and q_account_token provided,
+        If `quantum` is True and `q_account_token` provided,
         the classification task will be running on a IBM quantum backend.
         If `load_account` is provided, the classifier will use the previous
         token saved with `IBMProvider.save_account()`.
     verbose : bool (default:True)
-        If true will output all intermediate results and logs
+        If true, will output all intermediate results and logs.
     shots : int (default:1024)
-        Number of repetitions of each circuit, for sampling
-    gen_feature_map : Callable[int, QuantumCircuit | FeatureMap] \
-                      (default : Callable[int, ZZFeatureMap])
-        Function generating a feature map to encode data into a quantum state.
+        Number of repetitions of each circuit, for sampling.
+    upper_bound : int (default: 7)
+        The maximum integer value for matrix normalization.
+    regularization: MixinTransformer (defulat: None)
+        Additional post-processing to regularize means.
+    classical_optimizer : OptimizationAlgorithm
+        An instance of OptimizationAlgorithm [1]_
 
     Attributes
     ----------
     classes_ : list
         list of classes.
 
     Notes
     -----
     .. versionadded:: 0.1.0
+    .. versionchanged:: 0.2.0
+        Add regularization parameter.
+        Add classical_optimizer parameter.
+        Change metric, so you can pass the kernel of your choice\
+            as when using MDM.
 
     See Also
     --------
     QuanticMDM
 
+    References
+    ----------
+    .. [1] \
+        https://qiskit-community.github.io/qiskit-optimization/stubs/qiskit_optimization.algorithms.OptimizationAlgorithm.html#optimizationalgorithm
+
     """
 
     def __init__(
         self,
-        convex_metric="distance",
+        metric={"mean": "logeuclid", "distance": "qlogeuclid_hull"},
         quantum=True,
         q_account_token=None,
         verbose=True,
         shots=1024,
-        gen_feature_map=gen_zz_feature_map(),
+        upper_bound=7,
+        regularization=None,
+        classical_optimizer=CobylaOptimizer(rhobeg=2.1, rhoend=0.000001),
     ):
-        self.convex_metric = convex_metric
+        self.metric = metric
         self.quantum = quantum
         self.q_account_token = q_account_token
         self.verbose = verbose
         self.shots = shots
-        self.gen_feature_map = gen_feature_map
+        self.upper_bound = upper_bound
+        self.regularization = regularization
+        self.classical_optimizer = classical_optimizer
 
         BasePipeline.__init__(self, "QuantumMDMWithRiemannianPipeline")
 
     def _create_pipe(self):
-        if self.convex_metric == "both":
-            metric = {"mean": "convex", "distance": "convex"}
-        elif self.convex_metric == "mean":
-            metric = {"mean": "convex", "distance": "euclid"}
-        else:
-            metric = {"mean": "logeuclid", "distance": "convex"}
-
-        if metric["mean"] == "convex":
+        print(self.metric)
+        print(self.metric["mean"])
+        if is_qfunction(self.metric["mean"]):
             if self.quantum:
                 covariances = XdawnCovariances(
                     nfilter=1, estimator="scm", xdawn_estimator="lwf"
                 )
                 filtering = Whitening(dim_red={"n_components": 2})
             else:
                 covariances = ERPCovariances(estimator="lwf")
                 filtering = NoDimRed()
         else:
             covariances = ERPCovariances(estimator="lwf")
             filtering = NoDimRed()
 
         clf = QuanticMDM(
-            metric,
-            self.quantum,
-            self.q_account_token,
-            self.verbose,
-            self.shots,
-            self.gen_feature_map,
+            metric=self.metric,
+            quantum=self.quantum,
+            q_account_token=self.q_account_token,
+            verbose=self.verbose,
+            shots=self.shots,
+            upper_bound=self.upper_bound,
+            regularization=self.regularization,
+            classical_optimizer=self.classical_optimizer,
         )
 
         return make_pipeline(covariances, filtering, clf)
 
 
 class QuantumMDMVotingClassifier(BasePipeline):
 
-    """Voting classifier with two configuration of
-    QuantumMDMWithRiemannianPipeline :
-    - with mean = convex and distance = euclid
-    - with mean = logeuclid and distance = convex
+    """Voting classifier with two QuantumMDMWithRiemannianPipeline
+
+    Voting classifier with two configurations of
+    QuantumMDMWithRiemannianPipeline:
+
+    - with mean = qeuclid and distance = euclid,
+    - with mean = logeuclid and distance = qlogeuclid.
 
     Parameters
     ----------
     quantum : bool (default: True)
         - If true will run on local or remote backend
-        (depending on q_account_token value).
-        - If false, will perform classical computing instead
+          (depending on q_account_token value),
+        - If false, will perform classical computing instead.
     q_account_token : string (default:None)
-        If quantum==True and q_account_token provided,
+        If `quantum` is True and `q_account_token` provided,
         the classification task will be running on a IBM quantum backend.
         If `load_account` is provided, the classifier will use the previous
         token saved with `IBMProvider.save_account()`.
     verbose : bool (default:True)
-        If true will output all intermediate results and logs
+        If true, will output all intermediate results and logs.
     shots : int (default:1024)
-        Number of repetitions of each circuit, for sampling
+        Number of repetitions of each circuit, for sampling.
     gen_feature_map : Callable[int, QuantumCircuit | FeatureMap] \
                       (default : Callable[int, ZZFeatureMap])
         Function generating a feature map to encode data into a quantum state.
 
     Attributes
     ----------
     classes_ : list
@@ -432,43 +464,87 @@
 
     def __init__(
         self,
         quantum=True,
         q_account_token=None,
         verbose=True,
         shots=1024,
-        gen_feature_map=gen_zz_feature_map(),
+        upper_bound=7,
     ):
         self.quantum = quantum
         self.q_account_token = q_account_token
         self.verbose = verbose
         self.shots = shots
-        self.gen_feature_map = gen_feature_map
+        self.upper_bound = upper_bound
         BasePipeline.__init__(self, "QuantumMDMVotingClassifier")
 
     def _create_pipe(self):
-        clf_mean_logeuclid_dist_convex = QuantumMDMWithRiemannianPipeline(
-            "distance",
+        clf_mean_logeuclid_dist_cpm = QuantumMDMWithRiemannianPipeline(
+            {"mean": "logeuclid", "distance": "qlogeuclid_hull"},
             self.quantum,
             self.q_account_token,
             self.verbose,
             self.shots,
-            self.gen_feature_map,
+            self.upper_bound,
         )
-        clf_mean_convex_dist_euclid = QuantumMDMWithRiemannianPipeline(
-            "mean",
+        clf_mean_cpm_dist_euclid = QuantumMDMWithRiemannianPipeline(
+            {"mean": "qeuclid", "distance": "euclid"},
             self.quantum,
             self.q_account_token,
             self.verbose,
             self.shots,
-            self.gen_feature_map,
+            self.upper_bound,
         )
 
         return make_pipeline(
             VotingClassifier(
                 [
-                    ("mean_logeuclid_dist_convex", clf_mean_logeuclid_dist_convex),
-                    ("mean_convex_dist_euclid ", clf_mean_convex_dist_euclid),
+                    ("mean_logeuclid_dist_cpm", clf_mean_logeuclid_dist_cpm),
+                    ("mean_cpm_dist_euclid ", clf_mean_cpm_dist_euclid),
                 ],
                 voting="soft",
             )
         )
+
+
+class FeaturesUnionClassifier(BasePipeline):
+
+    """An alias for FeatureUnion + Classifier
+
+    Aggregate features generated by different transformers, and
+    use a classifier (e.g. LDA) in top of it.
+
+    Parameters
+    ----------
+    transformers : List[TransformerMixin], default=[QuanticNCH, MDM]
+        A list of sklearn transformers.
+    classifier : ClassifierMixin, default=LDA()
+        A classifier
+
+    Attributes
+    ----------
+    classes_ : list
+        list of classes.
+
+    Notes
+    -----
+    .. versionadded:: 0.2.0
+
+    """
+
+    def __init__(
+        self,
+        transformers=[
+            QuanticNCH(quantum=True, subsampling="random", n_jobs=-1),
+            MDM(metric="logeuclid"),
+        ],
+        classifier=LDA(),
+    ):
+        self.transformers = transformers
+        self.classifier = classifier
+        BasePipeline.__init__(self, "FeatureUnionClassifier")
+
+    def _create_pipe(self):
+        return make_pipeline(
+            FeatureUnion([(type(t).__name__, t) for t in self.transformers]),
+            self.classifier,
+        )
```

### Comparing `pyriemann-qiskit-0.1.0/pyriemann_qiskit/utils/__init__.py` & `pyriemann_qiskit-0.2.0/pyriemann_qiskit/utils/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from . import hyper_params_factory, filtering
+from . import hyper_params_factory, filtering, preprocessing
 from .quantum_provider import get_provider, get_devices, get_simulator
-from .math import cov_to_corr_matrix
+from .math import cov_to_corr_matrix, union_of_diff
 from .docplex import (
     square_cont_mat_var,
     square_int_mat_var,
     square_bin_mat_var,
     ClassicalOptimizer,
     NaiveQAOAOptimizer,
     set_global_optimizer,
@@ -14,31 +14,37 @@
     FirebaseConnector,
     Cache,
     generate_caches,
     filter_subjects_by_incomplete_results,
     add_moabb_dataframe_results_to_caches,
     convert_caches_to_dataframes,
 )
-from .distance import logeucl_dist_convex
+from . import distance
+from . import mean
+from . import utils
 
 __all__ = [
     "hyper_params_factory",
     "filtering",
+    "preprocessing",
     "get_provider",
     "get_devices",
     "get_simulator",
     "cov_to_corr_matrix",
+    "union_of_diff",
     "square_cont_mat_var",
     "square_int_mat_var",
     "square_bin_mat_var",
     "ClassicalOptimizer",
     "NaiveQAOAOptimizer",
     "set_global_optimizer",
     "get_global_optimizer",
-    "logeucl_dist_convex",
+    "distance",
+    "mean",
     "FirebaseConnector",
     "Cache",
     "generate_caches",
     "filter_subjects_by_incomplete_results",
     "add_moabb_dataframe_results_to_caches",
     "convert_caches_to_dataframes",
+    "utils",
 ]
```

### Comparing `pyriemann-qiskit-0.1.0/pyriemann_qiskit/utils/docplex.py` & `pyriemann_qiskit-0.2.0/pyriemann_qiskit/utils/docplex.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,42 +9,43 @@
 import numpy as np
 from docplex.mp.vartype import ContinuousVarType, IntegerVarType, BinaryVarType
 from qiskit.utils import QuantumInstance
 from qiskit.algorithms import QAOA
 from qiskit_optimization.algorithms import CobylaOptimizer, MinimumEigenOptimizer
 from qiskit_optimization.converters import IntegerToBinary
 from qiskit_optimization.translators import from_docplex_mp
-from pyriemann_qiskit.utils import cov_to_corr_matrix, get_simulator
+from pyriemann.utils.covariance import normalize
+from pyriemann_qiskit.utils import get_simulator
 
 
 _global_optimizer = [None]
 
 
 def set_global_optimizer(optimizer):
     """Set the value of the global optimizer
 
     Parameters
     ----------
     optimizer: pyQiskitOptimizer
-      An instance of pyQiskitOptimizer.
+      An instance of :class:`pyriemann_qiskit.utils.docplex.pyQiskitOptimizer`.
 
     Notes
     -----
     .. versionadded:: 0.0.4
     """
     _global_optimizer[0] = optimizer
 
 
 def get_global_optimizer(default):
     """Get the value of the global optimizer
 
     Parameters
     ----------
     default: pyQiskitOptimizer
-      An instance of pyQiskitOptimizer.
+      An instance of :class:`pyriemann_qiskit.utils.docplex.pyQiskitOptimizer`.
       It will be returned by default if the global optimizer is None.
 
     Returns
     -------
     optimizer : pyQiskitOptimizer
         The global optimizer.
 
@@ -303,27 +304,40 @@
         raise NotImplementedError()
 
 
 class ClassicalOptimizer(pyQiskitOptimizer):
 
     """Wrapper for the classical Cobyla optimizer.
 
+    Attributes
+    ----------
+    optimizer : OptimizationAlgorithm
+        An instance of OptimizationAlgorithm [1]_
+
     Notes
     -----
     .. versionadded:: 0.0.2
     .. versionchanged:: 0.0.4
+    .. versionchanged:: 0.2.0
+        Add attribute `optimizer`.
 
     See Also
     --------
     pyQiskitOptimizer
 
+    References
+    ----------
+    .. [1] \
+        https://qiskit-community.github.io/qiskit-optimization/stubs/qiskit_optimization.algorithms.OptimizationAlgorithm.html#optimizationalgorithm
+
     """
 
-    def __init__(self):
+    def __init__(self, optimizer=CobylaOptimizer(rhobeg=2.1, rhoend=0.000001)):
         pyQiskitOptimizer.__init__(self)
+        self.optimizer = optimizer
 
     """Helper to create a docplex representation of a
     covariance matrix variable.
 
     Parameters
     ----------
     prob : Model
@@ -356,15 +370,15 @@
 
     """
 
     def covmat_var(self, prob, channels, name):
         return square_cont_mat_var(prob, channels, name)
 
     def _solve_qp(self, qp, reshape=True):
-        result = CobylaOptimizer(rhobeg=2.1, rhoend=0.000001).solve(qp).x
+        result = self.optimizer.solve(qp).x
         if reshape:
             n_channels = int(math.sqrt(result.shape[0]))
             return np.reshape(result, (n_channels, n_channels))
         return result
 
     """Helper to create a docplex representation of a
     weight vector.
@@ -443,15 +457,15 @@
     Notes
     -----
     .. versionadded:: 0.0.2
 
     """
 
     def convert_covmat(self, covmat):
-        corr = cov_to_corr_matrix(covmat)
+        corr = normalize(covmat, "corr")
         return np.round(corr * self.upper_bound, 0)
 
     """Helper to create a docplex representation of a
     covariance matrix variable.
 
     Parameters
     ----------
```

### Comparing `pyriemann-qiskit-0.1.0/pyriemann_qiskit/utils/filtering.py` & `pyriemann_qiskit-0.2.0/pyriemann_qiskit/utils/filtering.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from sklearn.base import BaseEstimator, TransformerMixin
 import numpy as np
 
 
 class NoDimRed(TransformerMixin):
     """No dimensional reduction.
 
-    A Ghost transformer that just returns the data without
-    transformation.
+    A Ghost transformer that just returns the data without transformation.
 
     Notes
     -----
     .. versionadded:: 0.0.1
 
     """
 
@@ -55,15 +54,15 @@
         X : object
             The same data passed through the parameter X.
         """
         return X
 
 
 class NaiveDimRed(TransformerMixin):
-    """Naive dimensional reduction
+    """Naive dimensional reduction.
 
     Reduce the dimension of the feature by two,
 
     Parameters
     ----------
     is_even : bool (default: True)
         - If true keep only even indices of feature vectors.
@@ -112,15 +111,17 @@
             The filtered feature vectors.
         """
         offset = 0 if self.is_even else 1
         return X[:, offset::2]
 
 
 class Vectorizer(BaseEstimator, TransformerMixin):
-    """This is an auxiliary transformer that allows one to vectorize data
+    """Vectorization.
+
+    This is an auxiliary transformer that allows one to vectorize data
     structures in a pipeline. For instance, in the case of an X with
     dimensions (n_samples, n_features, n_channels),
     one might be interested in a new data structure with dimensions
     (n_samples, n_features x n_channels)
 
     Notes
     -----
```

### Comparing `pyriemann-qiskit-0.1.0/pyriemann_qiskit/utils/firebase_connector.py` & `pyriemann_qiskit-0.2.0/pyriemann_qiskit/utils/firebase_connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,33 +10,33 @@
         """No firebase_admin found. Firebase connector \
          can only run with mock data."""
     )
 from .firebase_cert import certificate
 
 
 class FirebaseConnector:
-    """
-    A connector to Firebase.
+    """A connector to Firebase.
+
     It gets/adds data to Firestore.
     (noSql database).
 
     Format of the data is as follows:
 
-    ```
+    ``
     datasets: {
-        bi2012: {
-            subject_01: {
-                pipeline1: {
-                    true_labels: [...],
-                    predicted_labels: [...]
-                }
-            }
-        }
+    bi2012: {
+    subject_01: {
+    pipeline1: {
+    true_labels: [...],
+    predicted_labels: [...]
+    }
+    }
+    }
     }
-    ```
+    ``
 
     Parameters
     ----------
     mock_data : Dict (default: None)
         If provided, it will skip the connection to firestore
         and use these data instead.
         It is useful for testing or
@@ -134,17 +134,17 @@
         pipeline_dict["true_labels"] = true_labels
         pipeline_dict["predicted_labels"] = predicted_labels
         if not self.mock_data:
             self._collection.document(dataset).set(dataset_dict)
 
     @property
     def datasets(self):
-        """
-        Get the data from Firestore
-        (or the mock data if provided).
+        """Get the data from Firestore.
+
+        Get the data from Firestore (or the mock data if provided).
         Data are readonly.
 
         Format of the data is as follows:
 
         Returns
         -------
         self : A representation of the database
@@ -155,18 +155,17 @@
         return str(self.datasets)
 
     def __str__(self) -> str:
         return repr(self)
 
 
 class Cache:
-    """
-    Layer of abstraction over FirebaseConnector.
-    It facilitates adding/removing data
-    for a particular dataset and pipeline.
+    """Layer of abstraction over FirebaseConnector.
+
+    It facilitates adding/removing data for a particular dataset and pipeline.
 
     Parameters
     ----------
     dataset_name: str
         The name of the dataset.
     pipeline: Pipeline
         The sklearn pipeline use for the analysis of the dataset.
@@ -188,24 +187,24 @@
         self._connector = FirebaseConnector(mock_data=mock_data)
 
     def _get_pipeline_dict(self, subject):
         key = str(self._pipeline)
         return self._connector.datasets[self._dataset_name][subject][key]
 
     def add(self, subject, true_labels, predicted_labels):
-        """
-        Add the prediction of the pipeline to the dataset.
+        """Add the prediction of the pipeline to the dataset.
 
         Parameters
         ----------
         subject: int|str
             The subject whom data were used for prediction.
-        true_labels: List
+        true_labels: list
             The true labels
-        predicted_labels: The predicted labels
+        predicted_labels: list
+            The predicted labels
 
         See Also
         --------
         FirebaseConnector
 
         Notes
         -----
@@ -225,16 +224,16 @@
         with the pipeline pass as a parameter in the constructor.
 
         Parameters
         ----------
         subject: int|str
             A subject in the dataset.
 
-        Return
-        --------
+        Returns
+        -------
         true_labels: List
             The true labels.
         predicted_labels: List
             The predicted labels obtained for this subject
             with the pipeline passed a a parameter in the constructor.
 
         Notes
@@ -267,20 +266,20 @@
     mock_data: Dict (default: None)
         Mock data that can be passed to the FirebaseConnector.
 
     See Also
     --------
     FirebaseConnector
 
-    Return
-    --------
+    Returns
+    -------
     caches: Dict
         A dictionnary containing all the generated caches, e.g.:
-        caches[datasetA][pipeline1]
-        contains the cache for the datasetA and the pipeline1.
+        ``caches[datasetA][pipeline1]``
+        contains the cache for the ``datasetA`` and the ``pipeline1``.
 
     Notes
     -----
     .. versionadded:: 0.0.4
     """
     caches = {}
     for dataset in datasets:
@@ -309,16 +308,16 @@
         caches[datasetA][pipeline1]
         contains the cache for the datasetA and the pipeline1.
     datasets: List
         The datasets.
     pipelines: List
         The sklearn Pipelines.
 
-    Return
-    --------
+    Returns
+    -------
     results: Dict
         A dictionnary of existing results, e.g.:
         results[datasetA][subjectA]
 
     Notes
     -----
     .. versionadded:: 0.0.4
@@ -401,16 +400,16 @@
         caches[datasetA][pipeline1]
         contains the cache for the datasetA and the pipeline1.
     datasets: List
         The datasets.
     pipelines: List
         The sklearn Pipelines.
 
-    Return
-    --------
+    Returns
+    -------
     results: pandas.DataFrame
         Results extracted from the caches.
         Headers of the DataFrame are:
         `pipeline`, `dataset`, `subject`, `score` and `time`.
         All columns contain string values except for `score` and `time`.
 
     Notes
```

### Comparing `pyriemann-qiskit-0.1.0/pyriemann_qiskit/utils/hyper_params_factory.py` & `pyriemann_qiskit-0.2.0/pyriemann_qiskit/utils/hyper_params_factory.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,137 @@
-from qiskit.circuit.library import ZZFeatureMap
+from qiskit.circuit.library import ZZFeatureMap, ZFeatureMap, PauliFeatureMap
 from qiskit.algorithms.optimizers import SPSA
 from qiskit.circuit.library import TwoLocal
 import inspect
 
 
+def gen_x_feature_map(reps=2):
+    """Return a callable that generates a XFeatureMap.
+
+    A feature map encodes data into a quantum state.
+    A XFeatureMap is a first-order Pauli-X evolution circuit (no entanglement).
+    See [1]_ for more details.
+
+    Parameters
+    ----------
+    reps : int (default 2)
+        The number of repeated circuits, greater or equal to 1.
+
+    Returns
+    -------
+    ret : XFeatureMap
+        An instance of XFeatureMap.
+
+    Raises
+    ------
+    ValueError
+        Raised if ``reps`` is lower than 1.
+
+    References
+    ----------
+    .. [1] \
+        https://docs.quantum.ibm.com/api/qiskit/0.44/qiskit.circuit.library.PauliFeatureMap
+
+    Notes
+    -----
+    .. versionadded:: 0.2.0
+    """
+    if reps < 1:
+        raise ValueError(f"Parameter reps must be superior or equal to 1 (Got {reps})")
+
+    return lambda n_features: PauliFeatureMap(
+        feature_dimension=n_features,
+        paulis=["X"],
+        reps=reps,
+        data_map_func=None,
+        parameter_prefix="x",
+        insert_barriers=False,
+        name="XFeatureMap",
+    )
+
+
+def gen_z_feature_map(reps=2):
+    """Return a callable that generates a ZFeatureMap.
+
+    A feature map encodes data into a quantum state.
+    A ZFeatureMap is a first-order Pauli-Z evolution circuit (no entanglement).
+    See [1]_ for more details.
+
+    Parameters
+    ----------
+    reps : int (default 2)
+        The number of repeated circuits, greater or equal to 1.
+
+    Returns
+    -------
+    ret : ZFeatureMap
+        An instance of ZFeatureMap.
+
+    Raises
+    ------
+    ValueError
+        Raised if ``reps`` is lower than 1.
+
+    References
+    ----------
+    .. [1] \
+        https://docs.quantum.ibm.com/api/qiskit/0.44/qiskit.circuit.library.ZFeatureMap
+
+    Notes
+    -----
+    .. versionadded:: 0.2.0
+    """
+    if reps < 1:
+        raise ValueError(f"Parameter reps must be superior or equal to 1 (Got {reps})")
+
+    return lambda n_features: ZFeatureMap(feature_dimension=n_features, reps=reps)
+
+
 def gen_zz_feature_map(reps=2, entanglement="linear"):
-    """Return a callable that generate a ZZFeatureMap.
+    """Return a callable that generates a ZZFeatureMap.
+
     A feature map encodes data into a quantum state.
     A ZZFeatureMap is a second-order Pauli-Z evolution circuit.
+    See [1]_ for more details.
+
 
     Parameters
     ----------
     reps : int (default 2)
         The number of repeated circuits, greater or equal to 1.
     entanglement : str | list[list[list[int]]] | \
                    Callable[int, list[list[list[int]]]]
         Specifies the entanglement structure.
         Entanglement structure can be provided with indices or string.
         Possible string values are: 'full', 'linear', 'circular' and 'sca'.
-        Consult [1]_ for more details on entanglement structure.
+        See [2]_ for more details on entanglement structure.
 
     Returns
     -------
     ret : ZZFeatureMap
-        An instance of ZZFeatureMap
+        An instance of ZZFeatureMap.
 
     Raises
     ------
     ValueError
         Raised if ``reps`` is lower than 1.
 
     References
     ----------
     .. [1] \
+        https://docs.quantum.ibm.com/api/qiskit/0.44/qiskit.circuit.library.ZZFeatureMap
+    .. [2] \
         https://qiskit.org/documentation/stable/0.19/stubs/qiskit.circuit.library.NLocal.html
+
+    Notes
+    -----
+    .. versionadded:: 0.0.1
     """
     if reps < 1:
-        raise ValueError(
-            "Parameter reps must be superior \
-                          or equal to 1 (Got %d)"
-            % reps
-        )
+        raise ValueError(f"Parameter reps must be superior or equal to 1 (Got {reps})")
 
     return lambda n_features: ZZFeatureMap(
         feature_dimension=n_features, reps=reps, entanglement=entanglement
     )
 
 
 # Valid gates for two local circuits
@@ -86,14 +173,15 @@
     else:
         if blocks not in gates:
             raise ValueError("Gate %s is not a valid gate" % blocks)
 
 
 def gen_two_local(reps=3, rotation_blocks=["ry", "rz"], entanglement_blocks="cz"):
     """Return a callable that generate a TwoLocal circuit.
+
     The two-local circuit is a parameterized circuit consisting
     of alternating rotation layers and entanglement layers [1]_.
 
     Parameters
     ----------
     reps : int (default 3)
         Specifies how often a block consisting of a rotation layer
@@ -104,21 +192,21 @@
     entanglement_blocks : str | list[str]
         The gates used in the entanglement layer.
         Valid string values are defined in `gates`.
 
     Returns
     -------
     ret : TwoLocal
-        An instance of a TwoLocal circuit
+        An instance of a TwoLocal circuit.
 
     Raises
     ------
     ValueError
         Raised if ``rotation_blocks`` or ``entanglement_blocks`` contain
-        a non valid gate
+        a non valid gate.
 
     References
     ----------
     .. [1] \
         https://qiskit.org/documentation/stable/0.19/stubs/qiskit.circuit.library.TwoLocal.html
     """
     if reps < 1:
@@ -135,14 +223,15 @@
     return lambda n_features: TwoLocal(
         n_features, rotation_blocks, entanglement_blocks, reps=reps
     )
 
 
 def get_spsa(max_trials=40, c=(None, None, None, None, 4.0)):
     """Return an instance of SPSA.
+
     SPSA [1]_, [2]_ is an algorithmic method for optimizing systems
     with multiple unknown parameters.
     For more details, see [3]_ and [4]_.
 
     Parameters
     ----------
     max_trials : int (default:40)
@@ -151,19 +240,18 @@
         The 5 control parameters for SPSA algorithms, namely:
         the initial point, the intial perturbation, alpha, gamma
         and the stability constant.
         See [3]_ for implementation details. This function set the
         default value of the control parameters for the `calibrate` method of
         the implementation.
 
-
     Returns
     -------
     ret : SPSA
-        An instance of SPSA
+        An instance of SPSA.
 
     References
     ----------
     .. [1] Spall, J. C. (2012), “Stochastic Optimization,”
            in Handbook of Computational Statistics:
            Concepts and Methods (2nd ed.)
            (J. Gentle, W. Härdle, and Y. Mori, eds.),
@@ -212,16 +300,17 @@
         )
 
     spsa.calibrate = calibrate
     return spsa
 
 
 def get_spsa_parameters(spsa):
-    """Return the default values of the `calibrate` method of
-    an SPSA instance. See [1]_ for implementation details.
+    """Return the default values of the `calibrate` method of an SPSA instance.
+
+    See [1]_ for implementation details.
 
     Parameters
     ----------
     spsa : SPSA
         The SPSA instance.
 
     Returns
```

### Comparing `pyriemann-qiskit-0.1.0/pyriemann_qiskit/utils/quantum_provider.py` & `pyriemann_qiskit-0.2.0/pyriemann_qiskit/utils/quantum_provider.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,17 @@
     .. versionchanged:: 0.1.0
         IBMProvider is not a static API anymore but need to be instanciated.
     """
     return IBMProvider()
 
 
 def get_simulator():
-    """Return a quantum simulator,
+    """Return a quantum simulator.
+
+    Return a quantum simulator,
     supporting GPU and NVIDIA's cuQuantum optimization
     (if enabled).
 
     Returns
     -------
     simulator : AerSimulator
         A quantum simulator.
@@ -41,17 +43,19 @@
         backend.set_options(device="GPU")
     else:
         print("GPU optimization disabled. No device found.")
     return backend
 
 
 def get_devices(provider, min_qubits):
-    """Returns all real remote quantum backends,
+    """Returns all real remote quantum backends.
+
+    Returns all real remote quantum backends,
     available with the account token and having at least
-    `min_qubits`
+    `min_qubits`.
 
     Parameters
     ----------
     provider: IBMProvider
         An instance of IBMProvider.
     min_qubits: int
         The minimun of qubits.
```

### Comparing `pyriemann-qiskit-0.1.0/pyriemann_qiskit/visualization/art.py` & `pyriemann_qiskit-0.2.0/pyriemann_qiskit/visualization/art.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+Artistic visualization for quantum.
+"""
+
 import pandas as pd
 import numpy as np
 
 
 def weights_spiral(axe, vqc, X, y, n_trainings=5):
     """Artistic representation of vqc training.
```

### Comparing `pyriemann-qiskit-0.1.0/pyriemann_qiskit.egg-info/SOURCES.txt` & `pyriemann_qiskit-0.2.0/pyriemann_qiskit.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 pyriemann_qiskit/__init__.py
 pyriemann_qiskit/_version.py
 pyriemann_qiskit/classification.py
+pyriemann_qiskit/ensemble.py
 pyriemann_qiskit/pipelines.py
 pyriemann_qiskit.egg-info/PKG-INFO
 pyriemann_qiskit.egg-info/SOURCES.txt
 pyriemann_qiskit.egg-info/dependency_links.txt
 pyriemann_qiskit.egg-info/not-zip-safe
 pyriemann_qiskit.egg-info/requires.txt
 pyriemann_qiskit.egg-info/top_level.txt
@@ -20,19 +21,25 @@
 pyriemann_qiskit/utils/docplex.py
 pyriemann_qiskit/utils/filtering.py
 pyriemann_qiskit/utils/firebase_cert.py
 pyriemann_qiskit/utils/firebase_connector.py
 pyriemann_qiskit/utils/hyper_params_factory.py
 pyriemann_qiskit/utils/math.py
 pyriemann_qiskit/utils/mean.py
+pyriemann_qiskit/utils/preprocessing.py
 pyriemann_qiskit/utils/quantum_provider.py
+pyriemann_qiskit/utils/utils.py
 pyriemann_qiskit/visualization/__init__.py
 pyriemann_qiskit/visualization/art.py
+pyriemann_qiskit/visualization/manifold.py
 tests/test_classification.py
 tests/test_datasets.py
 tests/test_docplex.py
+tests/test_ensemble.py
 tests/test_filtering.py
 tests/test_pipelines.py
+tests/test_preprocessing.py
 tests/test_utils_distance.py
 tests/test_utils_firebase.py
 tests/test_utils_hyper_params_factory.py
+tests/test_utils_math.py
 tests/test_utils_mean.py
```

### Comparing `pyriemann-qiskit-0.1.0/setup.py` & `pyriemann_qiskit-0.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,29 +28,42 @@
       long_description_content_type='text/markdown',
       project_urls={
           'Documentation': 'https://pyriemann.readthedocs.io',
           'Source': 'https://github.com/pyRiemann/pyRiemann-qiskit',
           'Tracker': 'https://github.com/pyRiemann/pyRiemann-qiskit/issues/',
       },
       platforms='any',
-      python_requires=">=3.8",
+      python_requires=">=3.9",
       install_requires=[
-                        'numpy<1.24',
+                        'numpy<1.27',
                         'cython',
                         'pyriemann==0.5',
+                        'qiskit==0.45.0',
                         'qiskit_machine_learning==0.6.1',
-                        'qiskit-ibm-provider==0.7.0',
+                        'qiskit-ibm-provider==0.7.3',
                         'qiskit-optimization==0.5.0',
                         'qiskit-aer==0.12.2',
-                        'cvxpy==1.3.2',
-                        'scipy==1.10.1',
-                        'docplex>=2.21.207',
-                        'firebase_admin==6.2.0',
-                        'tqdm'
+                        'cvxpy==1.4.2',
+                        'scipy==1.11.4',
+                        'docplex==2.25.236',
+                        'grpcio-status==1.62.1',
+                        'protobuf==4.25.3',
+                        'firebase_admin==6.4.0',
+                        'scikit-learn==1.3.2',
+                        'tqdm',
+                        'pandas'
                         ],
-      extras_require={'docs': ['sphinx-gallery', 'sphinx-bootstrap_theme', 'numpydoc', 'mne', 'seaborn', 'moabb>=0.4.6'],
+      extras_require={'docs': [
+                                'sphinx-gallery',
+                                'sphinx-bootstrap_theme',
+                                'numpydoc',
+                                'mne==1.6.1',
+                                'seaborn>=0.12.1',
+                                'moabb>=1.0.0',
+                                'imbalanced-learn==0.12.0'
+                            ],
                       'tests': ['pytest', 'seaborn', 'flake8', 'mne', 'pooch'],
                       # GPU optimization not available on all platform.
                       # See https://github.com/Qiskit/qiskit-aer/issues/929#issuecomment-691716936
                       'optim': ['qiskit-aer-gpu==0.12.2']},
       zip_safe=False,
 )
```

### Comparing `pyriemann-qiskit-0.1.0/tests/test_classification.py` & `pyriemann_qiskit-0.2.0/tests/test_classification.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import numpy as np
 from pyriemann.classification import TangentSpace
 from pyriemann.estimation import XdawnCovariances
 from pyriemann_qiskit.classification import (
     QuanticSVM,
     QuanticVQC,
     QuanticMDM,
+    QuanticNCH,
 )
 from pyriemann_qiskit.datasets import get_mne_sample
 from pyriemann_qiskit.utils.filtering import NaiveDimRed
 from sklearn.pipeline import make_pipeline
 from sklearn.model_selection import StratifiedKFold, cross_val_score
 
 
@@ -110,20 +111,18 @@
             "n_samples": 100,
             "n_features": 9,
             "quantum_instance": quantum_instance,
             "type": "bin",
         }
 
     def check(self):
-        assert (
-            self.prediction[: self.class_len].all() == self.quantum_instance.classes_[0]
-        )
-        assert (
-            self.prediction[self.class_len :].all() == self.quantum_instance.classes_[1]
-        )
+        # Check that all classes are predicted
+        assert len(self.prediction) == len(self.labels)
+        # Check if the proba for each classes are returned
+        assert self.predict_proab.shape[1] == len(np.unique(self.labels))
 
 
 class TestQuanticSVM(TestClassicalSVM):
     """Tests the Quantum version of Quantic SVM.
     It is executed on a simulated quantum computer.
     This test can also be run on a real computer by providing a qAccountToken.
     To do so, you need to use your own token, by registering on:
@@ -137,14 +136,25 @@
             "n_samples": 10,
             "n_features": 4,
             "quantum_instance": quantum_instance,
             "type": "bin",
         }
 
 
+class TestQuanticSVM_MultiClass(MultiClassFVT):
+    """Perform SVM on a simulated quantum computer
+    (multi-label classification)"""
+
+    def get_params(self):
+        return TestQuanticSVM.get_params(self)
+
+    def check(self):
+        TestQuanticSVM.check(self)
+
+
 class TestQuanticPegasosSVM(TestClassicalSVM):
     """Same as TestQuanticSVM, except it uses
     PegasosQSVC instead of QSVC implementation.
     """
 
     def get_params(self):
         quantum_instance = QuanticSVM(quantum=True, verbose=False, pegasos=True)
@@ -170,16 +180,18 @@
             "type": "rand",
         }
 
     def check(self):
         # Considering the inputs, this probably make no sense to test accuracy.
         # Instead, we could consider this test as a canary test
         assert len(self.prediction) == len(self.labels)
-        # Check the number of classes is consistent
+        # Check if the number of classes is consistent
         assert len(np.unique(self.prediction)) == len(np.unique(self.labels))
+        # Check if the proba for each classes are returned
+        assert self.predict_proab.shape[1] == len(np.unique(self.labels))
 
 
 class TestQuanticVQC_MultiClass(MultiClassFVT):
     """Perform VQC on a simulated quantum computer
     (multi-label classification)"""
 
     def get_params(self):
@@ -196,20 +208,55 @@
     def get_params(self):
         quantum_instance = QuanticMDM(
             quantum=False,
             verbose=False,
             metric={"mean": "logdet", "distance": "logdet"},
         )
         return {
-            "n_samples": 100,
+            "n_samples": 50,
             "n_features": 9,
             "quantum_instance": quantum_instance,
             "type": "bin_cov",
         }
 
     def check(self):
-        assert (
-            self.prediction[: self.class_len].all() == self.quantum_instance.classes_[0]
-        )
-        assert (
-            self.prediction[self.class_len :].all() == self.quantum_instance.classes_[1]
+        assert len(self.prediction) == len(self.labels)
+        # Check if the number of classes is consistent
+        assert len(np.unique(self.prediction)) == len(np.unique(self.labels))
+        # Check if the proba for each classes are returned
+        assert self.predict_proab.shape[1] == len(np.unique(self.labels))
+
+
+class TestQuanticMDM_MultiClass(MultiClassFVT):
+    """Perform MDM on a simulated quantum computer
+    (multi-label classification)"""
+
+    def get_params(self):
+        return TestClassicalMDM.get_params(self)
+
+    def check(self):
+        TestClassicalMDM.check(self)
+
+
+class TestClassicalNCH(BinaryFVT):
+    """Test the classical version of NCH using the QuanticNCH wrapper."""
+
+    def get_params(self):
+        quantum_instance = QuanticNCH(
+            n_hulls_per_class=1,
+            n_samples_per_hull=3,
+            subsampling="random",
+            quantum=False,
         )
+        return {
+            "n_samples": 50,
+            "n_features": 7,
+            "quantum_instance": quantum_instance,
+            "type": "bin_cov",
+        }
+
+    def check(self):
+        assert len(self.prediction) == len(self.labels)
+        # Check if the number of classes is consistent
+        assert len(np.unique(self.prediction)) == len(np.unique(self.labels))
+        # Check if the proba for each classes are returned
+        assert self.predict_proab.shape[1] == len(np.unique(self.labels))
```

### Comparing `pyriemann-qiskit-0.1.0/tests/test_datasets.py` & `pyriemann_qiskit-0.2.0/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `pyriemann-qiskit-0.1.0/tests/test_docplex.py` & `pyriemann_qiskit-0.2.0/tests/test_docplex.py`

 * *Files identical despite different names*

### Comparing `pyriemann-qiskit-0.1.0/tests/test_filtering.py` & `pyriemann_qiskit-0.2.0/tests/test_filtering.py`

 * *Files identical despite different names*

### Comparing `pyriemann-qiskit-0.1.0/tests/test_pipelines.py` & `pyriemann_qiskit-0.2.0/tests/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `pyriemann-qiskit-0.1.0/tests/test_utils_firebase.py` & `pyriemann_qiskit-0.2.0/tests/test_utils_firebase.py`

 * *Files identical despite different names*

### Comparing `pyriemann-qiskit-0.1.0/tests/test_utils_hyper_params_factory.py` & `pyriemann_qiskit-0.2.0/tests/test_utils_hyper_params_factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,38 @@
 import pytest
 from qiskit.circuit.parametertable import ParameterView
 from pyriemann_qiskit.utils.hyper_params_factory import (
+    gen_x_feature_map,
+    gen_z_feature_map,
     gen_zz_feature_map,
     gen_two_local,
     gates,
     get_spsa,
     get_spsa_parameters,
 )
 
 
+class TestGenXFeatureMapParams:
+    @pytest.mark.parametrize("reps", [2, 3])
+    def test_reps(self, reps):
+        """Test gen_z_feature_map with different number of repetitions"""
+        n_features = 2
+        feature_map = gen_x_feature_map(reps=reps)(n_features)
+        assert isinstance(feature_map.parameters, ParameterView)
+
+
+class TestGenZFeatureMapParams:
+    @pytest.mark.parametrize("reps", [2, 3])
+    def test_reps(self, reps):
+        """Test gen_z_feature_map with different number of repetitions"""
+        n_features = 2
+        feature_map = gen_z_feature_map(reps=reps)(n_features)
+        assert isinstance(feature_map.parameters, ParameterView)
+
+
 class TestGenZZFeatureMapParams:
     @pytest.mark.parametrize("entanglement", ["full", "linear", "circular", "sca"])
     def test_entangl_strings(self, entanglement):
         """Test gen_zz_feature_map with different
         string options of entanglement
         """
         n_features = 2
```

