# Comparing `tmp/bnpm-0.5.1.tar.gz` & `tmp/bnpm-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bnpm-0.5.1.tar", last modified: Sat Apr 13 02:30:19 2024, max compression
+gzip compressed data, was "bnpm-0.5.2.tar", last modified: Thu Apr 25 00:04:02 2024, max compression
```

## Comparing `bnpm-0.5.1.tar` & `bnpm-0.5.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 02:30:19.427810 bnpm-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-13 02:30:14.000000 bnpm-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-13 02:30:14.000000 bnpm-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12116 2024-04-13 02:30:19.427810 bnpm-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-13 02:30:14.000000 bnpm-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 02:30:19.415810 bnpm-0.5.1/bnpm/
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-13 02:30:14.000000 bnpm-0.5.1/bnpm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    57948 2024-04-13 02:30:14.000000 bnpm-0.5.1/bnpm/automatic_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)    37853 2024-04-13 02:30:14.000000 bnpm-0.5.1/bnpm/ca2p_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-04-13 02:30:14.000000 bnpm-0.5.1/bnpm/circular.py
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-04-13 02:30:14.000000 bnpm-0.5.1/bnpm/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)    49222 2024-04-13 02:30:14.000000 bnpm-0.5.1/bnpm/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)    18244 2024-04-13 02:30:14.000000 bnpm-0.5.1/bnpm/container_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-04-13 02:30:14.000000 bnpm-0.5.1/bnpm/cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-13 02:30:14.000000 bnpm-0.5.1/bnpm/cupy_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    29002 2024-04-13 02:30:14.000000 bnpm-0.5.1/bnpm/decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-04-13 02:30:14.000000 bnpm-0.5.1/bnpm/email_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17100 2024-04-13 02:30:14.000000 bnpm-0.5.1/bnpm/featurization.py
--rw-r--r--   0 runner    (1001) docker     (127)    24549 2024-04-13 02:30:14.000000 bnpm-0.5.1/bnpm/file_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11970 2024-04-13 02:30:14.000000 bnpm-0.5.1/bnpm/h5_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)    26452 2024-04-13 02:30:14.000000 bnpm-0.5.1/bnpm/image_augmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    64030 2024-04-13 02:30:14.000000 bnpm-0.5.1/bnpm/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    26653 2024-04-13 02:30:14.000000 bnpm-0.5.1/bnpm/indexing.py
--rw-r--r--   0 runner    (1001) docker     (127)    25013 2024-04-13 02:30:14.000000 bnpm-0.5.1/bnpm/linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)    10013 2024-04-13 02:30:14.000000 bnpm-0.5.1/bnpm/math_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16827 2024-04-13 02:30:14.000000 bnpm-0.5.1/bnpm/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    19083 2024-04-13 02:30:14.000000 bnpm-0.5.1/bnpm/neural_networks.py
--rw-r--r--   0 runner    (1001) docker     (127)    14180 2024-04-13 02:30:14.000000 bnpm-0.5.1/bnpm/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-04-13 02:30:14.000000 bnpm-0.5.1/bnpm/other_peoples_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-04-13 02:30:14.000000 bnpm-0.5.1/bnpm/parallel_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17759 2024-04-13 02:30:14.000000 bnpm-0.5.1/bnpm/path_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    44685 2024-04-13 02:30:14.000000 bnpm-0.5.1/bnpm/plotting_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9811 2024-04-13 02:30:14.000000 bnpm-0.5.1/bnpm/resource_tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)    43636 2024-04-13 02:30:14.000000 bnpm-0.5.1/bnpm/server.py
--rw-r--r--   0 runner    (1001) docker     (127)    33617 2024-04-13 02:30:14.000000 bnpm-0.5.1/bnpm/similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)    17139 2024-04-13 02:30:14.000000 bnpm-0.5.1/bnpm/spectral.py
--rw-r--r--   0 runner    (1001) docker     (127)    13584 2024-04-13 02:30:14.000000 bnpm-0.5.1/bnpm/sql_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-04-13 02:30:14.000000 bnpm-0.5.1/bnpm/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     8385 2024-04-13 02:30:14.000000 bnpm-0.5.1/bnpm/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)    47053 2024-04-13 02:30:14.000000 bnpm-0.5.1/bnpm/timeSeries.py
--rw-r--r--   0 runner    (1001) docker     (127)    32955 2024-04-13 02:30:14.000000 bnpm-0.5.1/bnpm/torch_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    53601 2024-04-13 02:30:14.000000 bnpm-0.5.1/bnpm/video.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-13 02:30:14.000000 bnpm-0.5.1/bnpm/welford_moving.py
--rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-04-13 02:30:14.000000 bnpm-0.5.1/bnpm/welford_moving_2D.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 02:30:19.415810 bnpm-0.5.1/bnpm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12116 2024-04-13 02:30:19.000000 bnpm-0.5.1/bnpm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-13 02:30:19.000000 bnpm-0.5.1/bnpm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 02:30:19.000000 bnpm-0.5.1/bnpm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-13 02:30:19.000000 bnpm-0.5.1/bnpm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-13 02:30:19.000000 bnpm-0.5.1/bnpm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-13 02:30:14.000000 bnpm-0.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-13 02:30:19.427810 bnpm-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-13 02:30:14.000000 bnpm-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:04:02.199751 bnpm-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-25 00:03:53.000000 bnpm-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-25 00:03:53.000000 bnpm-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12627 2024-04-25 00:04:02.195751 bnpm-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-25 00:03:53.000000 bnpm-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:04:02.183750 bnpm-0.5.2/bnpm/
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-25 00:03:53.000000 bnpm-0.5.2/bnpm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57948 2024-04-25 00:03:53.000000 bnpm-0.5.2/bnpm/automatic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37830 2024-04-25 00:03:53.000000 bnpm-0.5.2/bnpm/ca2p_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-04-25 00:03:53.000000 bnpm-0.5.2/bnpm/circular.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-04-25 00:03:53.000000 bnpm-0.5.2/bnpm/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49222 2024-04-25 00:03:53.000000 bnpm-0.5.2/bnpm/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18269 2024-04-25 00:03:53.000000 bnpm-0.5.2/bnpm/container_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-04-25 00:03:53.000000 bnpm-0.5.2/bnpm/cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-25 00:03:53.000000 bnpm-0.5.2/bnpm/cupy_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29002 2024-04-25 00:03:53.000000 bnpm-0.5.2/bnpm/decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-04-25 00:03:53.000000 bnpm-0.5.2/bnpm/email_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17100 2024-04-25 00:03:53.000000 bnpm-0.5.2/bnpm/featurization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24577 2024-04-25 00:03:53.000000 bnpm-0.5.2/bnpm/file_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11970 2024-04-25 00:03:53.000000 bnpm-0.5.2/bnpm/h5_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26452 2024-04-25 00:03:53.000000 bnpm-0.5.2/bnpm/image_augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64030 2024-04-25 00:03:53.000000 bnpm-0.5.2/bnpm/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30238 2024-04-25 00:03:53.000000 bnpm-0.5.2/bnpm/indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36325 2024-04-25 00:03:53.000000 bnpm-0.5.2/bnpm/linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10013 2024-04-25 00:03:53.000000 bnpm-0.5.2/bnpm/math_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17373 2024-04-25 00:03:53.000000 bnpm-0.5.2/bnpm/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19083 2024-04-25 00:03:53.000000 bnpm-0.5.2/bnpm/neural_networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14180 2024-04-25 00:03:53.000000 bnpm-0.5.2/bnpm/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-04-25 00:03:53.000000 bnpm-0.5.2/bnpm/other_peoples_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-04-25 00:03:53.000000 bnpm-0.5.2/bnpm/parallel_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17749 2024-04-25 00:03:53.000000 bnpm-0.5.2/bnpm/path_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44685 2024-04-25 00:03:53.000000 bnpm-0.5.2/bnpm/plotting_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9811 2024-04-25 00:03:53.000000 bnpm-0.5.2/bnpm/resource_tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43636 2024-04-25 00:03:53.000000 bnpm-0.5.2/bnpm/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34372 2024-04-25 00:03:53.000000 bnpm-0.5.2/bnpm/similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28366 2024-04-25 00:03:53.000000 bnpm-0.5.2/bnpm/spectral.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13584 2024-04-25 00:03:53.000000 bnpm-0.5.2/bnpm/sql_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-04-25 00:03:53.000000 bnpm-0.5.2/bnpm/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8385 2024-04-25 00:03:53.000000 bnpm-0.5.2/bnpm/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47053 2024-04-25 00:03:53.000000 bnpm-0.5.2/bnpm/timeSeries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41417 2024-04-25 00:03:53.000000 bnpm-0.5.2/bnpm/torch_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53601 2024-04-25 00:03:53.000000 bnpm-0.5.2/bnpm/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-25 00:03:53.000000 bnpm-0.5.2/bnpm/welford_moving.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-04-25 00:03:53.000000 bnpm-0.5.2/bnpm/welford_moving_2D.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:04:02.183750 bnpm-0.5.2/bnpm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12627 2024-04-25 00:04:02.000000 bnpm-0.5.2/bnpm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-25 00:04:02.000000 bnpm-0.5.2/bnpm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 00:04:02.000000 bnpm-0.5.2/bnpm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-25 00:04:02.000000 bnpm-0.5.2/bnpm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-25 00:04:02.000000 bnpm-0.5.2/bnpm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-25 00:03:53.000000 bnpm-0.5.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-25 00:04:02.199751 bnpm-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-04-25 00:03:53.000000 bnpm-0.5.2/setup.py
```

### Comparing `bnpm-0.5.1/LICENSE` & `bnpm-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bnpm-0.5.1/PKG-INFO` & `bnpm-0.5.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bnpm
-Version: 0.5.1
+Version: 0.5.2
 Summary: A library of useful modules for data analysis.
 Home-page: https://github.com/RichieHakim/basic_neural_processing_modules
 Author: Richard Hakim
 License: LICENSE
 Keywords: data analysis,machine learning,neuroscience
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -14,35 +14,36 @@
 Requires-Dist: ipywidgets; extra == "all"
 Requires-Dist: kornia; extra == "all"
 Requires-Dist: matplotlib; extra == "all"
 Requires-Dist: natsort; extra == "all"
 Requires-Dist: numba; extra == "all"
 Requires-Dist: numpy; extra == "all"
 Requires-Dist: opencv_contrib_python; extra == "all"
+Requires-Dist: opt_einsum; extra == "all"
 Requires-Dist: optuna; extra == "all"
 Requires-Dist: optuna_integration; extra == "all"
 Requires-Dist: pandas; extra == "all"
 Requires-Dist: paramiko; extra == "all"
 Requires-Dist: psutil; extra == "all"
 Requires-Dist: PyYAML; extra == "all"
 Requires-Dist: pytest; extra == "all"
+Requires-Dist: hypothesis; extra == "all"
 Requires-Dist: scikit_learn; extra == "all"
 Requires-Dist: tqdm; extra == "all"
 Requires-Dist: seaborn; extra == "all"
 Requires-Dist: sparse; extra == "all"
 Requires-Dist: scipy; extra == "all"
 Requires-Dist: sqlalchemy; extra == "all"
 Requires-Dist: pymysql; extra == "all"
 Requires-Dist: xxhash; extra == "all"
 Requires-Dist: wandb; extra == "all"
 Requires-Dist: torch; extra == "all"
 Requires-Dist: torchvision; extra == "all"
 Requires-Dist: torchaudio; extra == "all"
 Requires-Dist: tables; extra == "all"
-Requires-Dist: opt_einsum; extra == "all"
 Requires-Dist: pulp; extra == "all"
 Requires-Dist: spconv; extra == "all"
 Requires-Dist: torch_sparse; extra == "all"
 Requires-Dist: av; extra == "all"
 Requires-Dist: pynwb; extra == "all"
 Requires-Dist: sendgrid; extra == "all"
 Requires-Dist: pycuda; extra == "all"
@@ -60,35 +61,36 @@
 Requires-Dist: ipywidgets; extra == "all-latest"
 Requires-Dist: kornia; extra == "all-latest"
 Requires-Dist: matplotlib; extra == "all-latest"
 Requires-Dist: natsort; extra == "all-latest"
 Requires-Dist: numba; extra == "all-latest"
 Requires-Dist: numpy; extra == "all-latest"
 Requires-Dist: opencv_contrib_python; extra == "all-latest"
+Requires-Dist: opt_einsum; extra == "all-latest"
 Requires-Dist: optuna; extra == "all-latest"
 Requires-Dist: optuna_integration; extra == "all-latest"
 Requires-Dist: pandas; extra == "all-latest"
 Requires-Dist: paramiko; extra == "all-latest"
 Requires-Dist: psutil; extra == "all-latest"
 Requires-Dist: PyYAML; extra == "all-latest"
 Requires-Dist: pytest; extra == "all-latest"
+Requires-Dist: hypothesis; extra == "all-latest"
 Requires-Dist: scikit_learn; extra == "all-latest"
 Requires-Dist: tqdm; extra == "all-latest"
 Requires-Dist: seaborn; extra == "all-latest"
 Requires-Dist: sparse; extra == "all-latest"
 Requires-Dist: scipy; extra == "all-latest"
 Requires-Dist: sqlalchemy; extra == "all-latest"
 Requires-Dist: pymysql; extra == "all-latest"
 Requires-Dist: xxhash; extra == "all-latest"
 Requires-Dist: wandb; extra == "all-latest"
 Requires-Dist: torch; extra == "all-latest"
 Requires-Dist: torchvision; extra == "all-latest"
 Requires-Dist: torchaudio; extra == "all-latest"
 Requires-Dist: tables; extra == "all-latest"
-Requires-Dist: opt_einsum; extra == "all-latest"
 Requires-Dist: pulp; extra == "all-latest"
 Requires-Dist: spconv; extra == "all-latest"
 Requires-Dist: torch_sparse; extra == "all-latest"
 Requires-Dist: av; extra == "all-latest"
 Requires-Dist: pynwb; extra == "all-latest"
 Requires-Dist: sendgrid; extra == "all-latest"
 Requires-Dist: pycuda; extra == "all-latest"
@@ -106,22 +108,24 @@
 Requires-Dist: kornia; extra == "core"
 Requires-Dist: matplotlib; extra == "core"
 Requires-Dist: numba; extra == "core"
 Requires-Dist: scikit_learn; extra == "core"
 Requires-Dist: tqdm; extra == "core"
 Requires-Dist: h5py; extra == "core"
 Requires-Dist: opencv_contrib_python; extra == "core"
+Requires-Dist: opt_einsum; extra == "core"
 Requires-Dist: optuna; extra == "core"
 Requires-Dist: optuna_integration; extra == "core"
 Requires-Dist: sparse; extra == "core"
 Requires-Dist: natsort; extra == "core"
 Requires-Dist: paramiko; extra == "core"
 Requires-Dist: pandas; extra == "core"
 Requires-Dist: psutil; extra == "core"
 Requires-Dist: pytest; extra == "core"
+Requires-Dist: hypothesis; extra == "core"
 Requires-Dist: PyYAML; extra == "core"
 Requires-Dist: torch; extra == "core"
 Requires-Dist: torchvision; extra == "core"
 Requires-Dist: torchaudio; extra == "core"
 Requires-Dist: ipywidgets; extra == "core"
 Requires-Dist: eva_decord; extra == "core"
 Requires-Dist: wandb; extra == "core"
@@ -133,22 +137,24 @@
 Requires-Dist: kornia; extra == "core-latest"
 Requires-Dist: matplotlib; extra == "core-latest"
 Requires-Dist: numba; extra == "core-latest"
 Requires-Dist: scikit_learn; extra == "core-latest"
 Requires-Dist: tqdm; extra == "core-latest"
 Requires-Dist: h5py; extra == "core-latest"
 Requires-Dist: opencv_contrib_python; extra == "core-latest"
+Requires-Dist: opt_einsum; extra == "core-latest"
 Requires-Dist: optuna; extra == "core-latest"
 Requires-Dist: optuna_integration; extra == "core-latest"
 Requires-Dist: sparse; extra == "core-latest"
 Requires-Dist: natsort; extra == "core-latest"
 Requires-Dist: paramiko; extra == "core-latest"
 Requires-Dist: pandas; extra == "core-latest"
 Requires-Dist: psutil; extra == "core-latest"
 Requires-Dist: pytest; extra == "core-latest"
+Requires-Dist: hypothesis; extra == "core-latest"
 Requires-Dist: PyYAML; extra == "core-latest"
 Requires-Dist: torch; extra == "core-latest"
 Requires-Dist: torchvision; extra == "core-latest"
 Requires-Dist: torchaudio; extra == "core-latest"
 Requires-Dist: ipywidgets; extra == "core-latest"
 Requires-Dist: eva_decord; extra == "core-latest"
 Requires-Dist: wandb; extra == "core-latest"
@@ -160,22 +166,24 @@
 Requires-Dist: kornia; extra == "core-cv2headless"
 Requires-Dist: matplotlib; extra == "core-cv2headless"
 Requires-Dist: numba; extra == "core-cv2headless"
 Requires-Dist: scikit_learn; extra == "core-cv2headless"
 Requires-Dist: tqdm; extra == "core-cv2headless"
 Requires-Dist: h5py; extra == "core-cv2headless"
 Requires-Dist: opencv_contrib_python_headless; extra == "core-cv2headless"
+Requires-Dist: opt_einsum; extra == "core-cv2headless"
 Requires-Dist: optuna; extra == "core-cv2headless"
 Requires-Dist: optuna_integration; extra == "core-cv2headless"
 Requires-Dist: sparse; extra == "core-cv2headless"
 Requires-Dist: natsort; extra == "core-cv2headless"
 Requires-Dist: paramiko; extra == "core-cv2headless"
 Requires-Dist: pandas; extra == "core-cv2headless"
 Requires-Dist: psutil; extra == "core-cv2headless"
 Requires-Dist: pytest; extra == "core-cv2headless"
+Requires-Dist: hypothesis; extra == "core-cv2headless"
 Requires-Dist: PyYAML; extra == "core-cv2headless"
 Requires-Dist: torch; extra == "core-cv2headless"
 Requires-Dist: torchvision; extra == "core-cv2headless"
 Requires-Dist: torchaudio; extra == "core-cv2headless"
 Requires-Dist: ipywidgets; extra == "core-cv2headless"
 Requires-Dist: eva_decord; extra == "core-cv2headless"
 Requires-Dist: wandb; extra == "core-cv2headless"
@@ -187,22 +195,24 @@
 Requires-Dist: kornia; extra == "core-latest-cv2headless"
 Requires-Dist: matplotlib; extra == "core-latest-cv2headless"
 Requires-Dist: numba; extra == "core-latest-cv2headless"
 Requires-Dist: scikit_learn; extra == "core-latest-cv2headless"
 Requires-Dist: tqdm; extra == "core-latest-cv2headless"
 Requires-Dist: h5py; extra == "core-latest-cv2headless"
 Requires-Dist: opencv_contrib_python_headless; extra == "core-latest-cv2headless"
+Requires-Dist: opt_einsum; extra == "core-latest-cv2headless"
 Requires-Dist: optuna; extra == "core-latest-cv2headless"
 Requires-Dist: optuna_integration; extra == "core-latest-cv2headless"
 Requires-Dist: sparse; extra == "core-latest-cv2headless"
 Requires-Dist: natsort; extra == "core-latest-cv2headless"
 Requires-Dist: paramiko; extra == "core-latest-cv2headless"
 Requires-Dist: pandas; extra == "core-latest-cv2headless"
 Requires-Dist: psutil; extra == "core-latest-cv2headless"
 Requires-Dist: pytest; extra == "core-latest-cv2headless"
+Requires-Dist: hypothesis; extra == "core-latest-cv2headless"
 Requires-Dist: PyYAML; extra == "core-latest-cv2headless"
 Requires-Dist: torch; extra == "core-latest-cv2headless"
 Requires-Dist: torchvision; extra == "core-latest-cv2headless"
 Requires-Dist: torchaudio; extra == "core-latest-cv2headless"
 Requires-Dist: ipywidgets; extra == "core-latest-cv2headless"
 Requires-Dist: eva_decord; extra == "core-latest-cv2headless"
 Requires-Dist: wandb; extra == "core-latest-cv2headless"
```

### Comparing `bnpm-0.5.1/README.md` & `bnpm-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `bnpm-0.5.1/bnpm/__init__.py` & `bnpm-0.5.2/bnpm/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -33,16 +33,16 @@
     'timeSeries',
     'torch_helpers',
     'video',
 ]
 
 
 ## Prepare cv2.imshow
-import pkg_resources
-installed_packages = {pkg.key for pkg in pkg_resources.working_set}
+import importlib.metadata
+installed_packages = {dist.metadata['Name'] for dist in importlib.metadata.distributions()}
 has_cv2_headless = 'opencv-contrib-python-headless' in installed_packages
 has_cv2_normal = 'opencv-contrib-python' in installed_packages
 if has_cv2_normal and not has_cv2_headless:
     run_cv2_imshow = True
 elif has_cv2_headless and not has_cv2_normal:
     run_cv2_imshow = False
 elif has_cv2_headless and has_cv2_normal:
@@ -62,22 +62,22 @@
         av and decord.
         RH 2022
         """
         import numpy as np
         import cv2
         test = np.zeros((1,300,400,3))
         for frame in test:
-            cv2.putText(frame, "WELCOME TO FACE BNPM!", (10,50), cv2.FONT_HERSHEY_SIMPLEX, 0.7, (255,255,255), 2)
+            cv2.putText(frame, "WELCOME TO BNPM!", (10,50), cv2.FONT_HERSHEY_SIMPLEX, 0.7, (255,255,255), 2)
             cv2.putText(frame, "Prepping CV2", (10,100), cv2.FONT_HERSHEY_SIMPLEX, 0.7, (255,255,255), 2)
             cv2.putText(frame, "Calling this figure allows cv2.imshow ", (10,150), cv2.FONT_HERSHEY_SIMPLEX, 0.5, (255,255,255), 1)
             cv2.putText(frame, "to work without crashing if this function", (10,170), cv2.FONT_HERSHEY_SIMPLEX, 0.5, (255,255,255), 1)
             cv2.putText(frame, "is called before importing av and decord", (10,190), cv2.FONT_HERSHEY_SIMPLEX, 0.5, (255,255,255), 1)
             cv2.imshow('startup', frame)
             cv2.waitKey(1000)
         cv2.destroyWindow('startup')
     prepare_cv2_imshow()
 
 
 for pkg in __all__:
     exec('from . import ' + pkg)
 
-__version__ = '0.5.1'
+__version__ = '0.5.2'
```

### Comparing `bnpm-0.5.1/bnpm/automatic_regression.py` & `bnpm-0.5.2/bnpm/automatic_regression.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.5.1/bnpm/ca2p_preprocessing.py` & `bnpm-0.5.2/bnpm/ca2p_preprocessing.py`

 * *Files 0% similar despite different names*

```diff
@@ -438,15 +438,14 @@
 
     # var_FneuSub = torch.var(F_neuSub, dim=1)
     # EV__F_by_Fneu = 1 - (var_FneuSub / var_F)
     _, EV__F_by_Fneu, _, _ = pairwise_orthogonalization_torch(
         v1=F.T,
         v2=Fneu.T,
         center=True,
-        device=device,
     )
 
     # F_baseline = torch.quantile(F, percentile_baseline/100, dim=1, keepdim=True)
     # FneuSub_baseline = torch.quantile(F_neuSub, percentile_baseline/100, dim=1, keepdim=True)
     ## For some reason, torch.quantile is absurdly slow. So we'll use kthvalue instead
     k = int(np.round((F.shape[1]-1) * percentile_baseline / 100)) + 1  ## kthvalue is 1-indexed
     F_baseline = torch.kthvalue(F, k, dim=1, keepdim=True).values
```

### Comparing `bnpm-0.5.1/bnpm/circular.py` & `bnpm-0.5.2/bnpm/circular.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.5.1/bnpm/classification.py` & `bnpm-0.5.2/bnpm/classification.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.5.1/bnpm/clustering.py` & `bnpm-0.5.2/bnpm/clustering.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.5.1/bnpm/container_helpers.py` & `bnpm-0.5.2/bnpm/container_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import re
 import copy
 from collections.abc import MutableMapping
 from typing import Dict, Any, Optional, Union, List, Tuple, Callable, Iterable, Iterator, Type
 
-import numpy as np
-
 """
 This module is intended to have minimal dependencies.
 It is called by server.py which is intended to run
  outside of a specialized environment, so no weird
  libraries should be required.
 RH 2022
 """
@@ -243,14 +241,16 @@
         params_unchanging (list of dicts):
             List of dictionary items that are the 
              same across all dictionaries.
         params_changing (list of dicts):
             List of dictionary items that are 
              different in at least one dictionary.
     """
+    import numpy as np
+
     def get_binary_search_combos(n):
         combos = list(np.arange(n))
         if len(combos)%2 == 1:
             combos.append(combos[-1])
         combos = np.array(combos).reshape(len(combos)//2, 2)
         return combos
 
@@ -563,10 +563,11 @@
 
     Returns:
         ss_comb_dicts (list):
             List of dictionaries, where each dictionary is a combination of
             parameter values from the search space.\n
             Example: [{'lr': 0.1, 'batch_size': 32}, {'lr': 0.1, 'batch_size': 64}, ...]
     """
+    import itertools
     vals_comb = list(itertools.product(*search_space.values()))
     ss_comb_dicts = [{k: val for k, val in zip(search_space.keys(), vals)} for vals in vals_comb]
     return ss_comb_dicts
```

### Comparing `bnpm-0.5.1/bnpm/cross_validation.py` & `bnpm-0.5.2/bnpm/cross_validation.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.5.1/bnpm/cupy_helpers.py` & `bnpm-0.5.2/bnpm/cupy_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.5.1/bnpm/decomposition.py` & `bnpm-0.5.2/bnpm/decomposition.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.5.1/bnpm/email_helpers.py` & `bnpm-0.5.2/bnpm/email_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.5.1/bnpm/featurization.py` & `bnpm-0.5.2/bnpm/featurization.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.5.1/bnpm/file_helpers.py` & `bnpm-0.5.2/bnpm/file_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import json
 import yaml
 from pathlib import Path
 import zipfile
 
 from tqdm import tqdm
 
+from . import path_helpers
+
 
 def prepare_path(path, mkdir=False, exist_ok=True):
     """
     Checks if a directory or filepath for validity for different
      purposes: saving, loading, etc.
     If exists:
         If exist_ok=True: all good
```

### Comparing `bnpm-0.5.1/bnpm/h5_handling.py` & `bnpm-0.5.2/bnpm/h5_handling.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.5.1/bnpm/image_augmentation.py` & `bnpm-0.5.2/bnpm/image_augmentation.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.5.1/bnpm/image_processing.py` & `bnpm-0.5.2/bnpm/image_processing.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.5.1/bnpm/indexing.py` & `bnpm-0.5.2/bnpm/indexing.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Optional, Union, Iterator
 import math
 
 import numpy as np
 from numba import jit, njit, prange
 import copy
 import scipy.signal
 import matplotlib.pyplot as plt
@@ -248,15 +249,19 @@
 
     assert batch_size > 0, 'batch_size must be greater than 0'
     assert min_batch_size <= batch_size, 'min_batch_size must be less than or equal to batch_size'
     assert num_batches > 0, 'num_batches must be greater than 0'    
 
     ## Make slices
     offset = np.random.randint(0, batch_size) if randomize_batch_indices else 0
-    idx_slices = [slice(s, min(e, l), None) for s, e in (zip(np.arange(idx_start + offset, l, batch_size), np.arange(idx_start + batch_size + offset, l + batch_size + offset, batch_size)))]
+    idx_slices = [
+        slice(s, min(e, l), None) for s, e in (zip(
+            np.arange(idx_start + offset, l, batch_size), 
+            np.arange(idx_start + batch_size + offset, l + batch_size + offset, batch_size)
+        ))]
     if offset > 0:
         idx_slices = [slice(0, offset, None)] + idx_slices
 
     ## Remove small batches
     if min_batch_size > 0:
         idx_slices = [idx for idx in idx_slices if (idx.stop - idx.start) >= min_batch_size]
 
@@ -460,14 +465,106 @@
             off-diagonal elements of x.
     """
     n, m = x.shape
     assert n == m
     return x.reshape(-1)[:-1].reshape(n - 1, n + 1)[:, 1:].reshape(-1)
 
 
+def batched_unfold(
+    tensor: torch.Tensor, 
+    dimension: int,
+    size: int,
+    step: int, 
+    batch_size: int = 10, 
+    pad_value: Optional[Union[int, float]] = None,
+) -> Iterator[torch.Tensor]:
+    """
+    Generates batches of overlapping windows from a tensor in a batched manner.
+    This function mimics the behavior of `torch.Tensor.unfold` but allows for
+    processing in smaller, more manageable batches. Using
+    `torch.cat(list(batched_unfold(...)), dim=dimension)` should reproduce the
+    result of `tensor.unfold(dimension, size, step)`. Note: The last batch may
+    be smaller than the specified batch size due to the remainder of the
+    division.
+
+    RH 2024
+
+    Args:
+        tensor (torch.Tensor): 
+            The input tensor from which to generate unfolded windows.
+        dimension (int): 
+            The dimension along which to unfold the tensor.
+        size (int): 
+            The size of each window to unfold.
+        step (int): 
+            The step size between the starts of each window.
+        batch_size (int): 
+            The number of windows to include in each batch. (Default is 10)
+        pad_value (Optional[Union[int, float]]):
+            The value to use for padding the last batch if it is smaller than
+            the specified batch size. If None, the last batch will not be
+            padded. (Default is None)
+
+
+    Yields:
+        torch.Tensor: 
+            A batch of unfolded windows from the tensor.
+    """
+    n_samples = tensor.shape[dimension]
+    if step >= n_samples:
+        raise ValueError("Step size must be less than the tensor size along the specified dimension.")
+    if size > n_samples:
+        raise ValueError("Window size must be less than or equal to the tensor size along the specified dimension.")
+
+    # Calculate end points
+    idx_start_last = ((n_samples - size) // step) * step
+    # idx_last_start = max(idx_last_start, 0)
+    # idx_last_end = idx_last_start + size - 1  ## Inclusive
+
+    idx_starts_all = range(0, idx_start_last + 1, step)
+    # idx_ends_all = list((idx + size for idx in idx_starts_all))  ## Exclusive
+
+    ## Generate batches
+    for i_batch, idx_start in enumerate(idx_starts_all[::batch_size]):
+        idx_end = idx_start + (step * (batch_size - 1)) + size
+        n_samples_pad = 0
+        if idx_end > n_samples:
+            if pad_value is None:
+                idx_end = n_samples
+            else:
+                n_samples_batch = n_samples - idx_start
+                idx_start_last_batch = int((math.ceil((n_samples_batch - size) / step)) * step)
+                idx_end = idx_start + idx_start_last_batch + size
+                idx_end = min(idx_end, n_samples + size)
+                n_samples_pad = idx_end - n_samples
+            
+        len_batch = idx_end - idx_start
+
+        if n_samples_pad > 0:
+            shape_pad = list(tensor.shape)
+            shape_pad[dimension] = n_samples_pad
+            x_batch = torch.cat((
+                tensor.narrow(
+                    dim=dimension, 
+                    start=idx_start, 
+                    length=n_samples - idx_start,
+                ), 
+                torch.full(
+                    size=shape_pad,
+                    fill_value=pad_value,
+                    dtype=tensor.dtype,
+                    device=tensor.device,
+                )
+            ))
+        else:
+            x_batch = tensor.narrow(dimension, idx_start, len_batch)
+
+        yield x_batch.unfold(dimension, size, step)
+
+
 #######################################
 ############ SPARSE STUFF #############
 #######################################
 
 def sparse_mask(x, mask_sparse, do_safety_steps=True):
     """
     Masks a sparse matrix with the non-zero elements of another
```

### Comparing `bnpm-0.5.1/bnpm/math_functions.py` & `bnpm-0.5.2/bnpm/math_functions.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.5.1/bnpm/misc.py` & `bnpm-0.5.2/bnpm/misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-import numpy as np
+from typing import Callable, List, Any, Dict, Union
 import sys
 import re
 import hashlib
 from pathlib import Path
 import warnings
-from typing import Callable, List, Any, Dict
 from contextlib import contextmanager, ExitStack
 
+import numpy as np
+
 
 def estimate_array_size(
     array=None, 
     numel=None, 
     input_shape=None, 
     bitsize=64, 
     units='GB',
@@ -335,32 +336,39 @@
         gcc_version = subprocess.check_output(['gcc', '--version']).decode('utf-8').split('\n')[0].split(' ')[-1]
     except Exception as e:
         warnings.warn(f'RH WARNING: unable to get gcc version. Got error: {e}')
         gcc_version = 'Faled to get'
     print(f'== GCC Version ==: {gcc_version}') if verbose else None
     
     ## PyTorch
-    import torch
-    torch_version = str(torch.__version__)
-    print(f'== PyTorch Version ==: {torch_version}') if verbose else None
-    ## CUDA
-    if torch.cuda.is_available():
-        cuda_version = torch.version.cuda
-        cudnn_version = torch.backends.cudnn.version()
-        torch_devices = [f'device {i}: Name={torch.cuda.get_device_name(i)}, Memory={torch.cuda.get_device_properties(i).total_memory / 1e9} GB' for i in range(torch.cuda.device_count())]
-        print(f"== CUDA Version ==: {cuda_version}, CUDNN Version: {cudnn_version}, Number of Devices: {torch.cuda.device_count()}, Devices: {torch_devices}, ") if verbose else None
-    else:
-        cuda_version = None
-        cudnn_version = None
-        torch_devices = None
-        print('== CUDA is not available ==') if verbose else None
+    try:
+        import torch
+        torch_version = str(torch.__version__)
+        print(f'== PyTorch Version ==: {torch_version}') if verbose else None
+        ## CUDA
+        if torch.cuda.is_available():
+            cuda_version = torch.version.cuda
+            cudnn_version = torch.backends.cudnn.version()
+            torch_devices = [f'device {i}: Name={torch.cuda.get_device_name(i)}, Memory={torch.cuda.get_device_properties(i).total_memory / 1e9} GB' for i in range(torch.cuda.device_count())]
+            print(f"== CUDA Version ==: {cuda_version}, CUDNN Version: {cudnn_version}, Number of Devices: {torch.cuda.device_count()}, Devices: {torch_devices}, ") if verbose else None
+        else:
+            cuda_version = 'cuda not available'
+            cudnn_version = 'cuda not available'
+            torch_devices = 'cuda not available'
+            print('== CUDA is not available ==') if verbose else None
+    except Exception as e:
+        warnings.warn(f'RH WARNING: unable to get torch info. Got error: {e}')
+        torch_version = 'torch not found'
+        cuda_version = 'torch not found'
+        cudnn_version = 'torch not found'
+        torch_devices = 'torch not found'
 
     ## all packages in environment
-    import pkg_resources
-    pkgs_dict = {i.key: i.version for i in pkg_resources.working_set}
+    import importlib.metadata
+    pkgs_dict = {dist.metadata['Name']: dist.metadata['Version'] for dist in importlib.metadata.distributions()}
 
     ## get datetime
     from datetime import datetime
     dt = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
 
     versions = {
         'datetime': dt,
@@ -530,14 +538,22 @@
     signal.alarm(seconds)
     try:
         yield
     finally:
         signal.alarm(0)
 
 
+@contextmanager
+def nullcontext():
+    """
+    A context manager that does nothing.
+    """
+    yield
+
+
 #########################################################
 ############ INTRA-MODULE HELPER FUNCTIONS ##############
 #########################################################
 
 
 def convert_size(size, return_size='GB'):
     """
```

### Comparing `bnpm-0.5.1/bnpm/neural_networks.py` & `bnpm-0.5.2/bnpm/neural_networks.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.5.1/bnpm/optimization.py` & `bnpm-0.5.2/bnpm/optimization.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.5.1/bnpm/other_peoples_code.py` & `bnpm-0.5.2/bnpm/other_peoples_code.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.5.1/bnpm/parallel_helpers.py` & `bnpm-0.5.2/bnpm/parallel_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,16 @@
     func: Callable, 
     args: List[Any], 
     method: str = 'multithreading', 
     n_workers: int = -1, 
     prog_bar: bool = True
 ) -> List[Any]:
     """
-    Maps a function to a list of arguments in parallel.
+    Maps a function to a list of arguments in parallel. Includes a progress bar
+    and error handling that points to the job that failed.
     RH 2022
 
     Args:
         func (Callable): 
             The function to be mapped.
         args (List[Any]): 
             List of arguments to which the function should be mapped.
```

### Comparing `bnpm-0.5.1/bnpm/path_helpers.py` & `bnpm-0.5.2/bnpm/path_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import os
 import numpy as np
 from pathlib import Path
 import re
 import warnings
 import datetime
 
-from . import misc
 
 def mkdir(directory, parents=True, exist_ok=True):
     '''
     Create a directory if it doesn't exist.
     RH 2021
 
     Args:
@@ -414,15 +413,15 @@
     file_openable = {file: check_with_timeout(file, time_limit=time_limit_per_file) for file in files}
     return file_openable
 
 
 def touch_path(
     path: Union[str, Path],
     recursive: bool = False,
-    dt: Optional[datetime] = None,
+    dt: Optional[datetime.datetime] = None,
     files: bool = True,
     directories: bool = True,
     verbose: Union[bool, int] = False,
 ) -> None:
     """
     Update the last modified datetime of specified files and/or directories
     without creating new ones. Symbolic links are skipped. \n
```

### Comparing `bnpm-0.5.1/bnpm/plotting_helpers.py` & `bnpm-0.5.2/bnpm/plotting_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.5.1/bnpm/resource_tracking.py` & `bnpm-0.5.2/bnpm/resource_tracking.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.5.1/bnpm/server.py` & `bnpm-0.5.2/bnpm/server.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.5.1/bnpm/similarity.py` & `bnpm-0.5.2/bnpm/similarity.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,44 +233,52 @@
                     pca_dict[key] = pca_dict[key].cpu().numpy()
 
     return v1_orth, EVR, EVR_total, pca_dict
 
 
 def orthogonalize_matrix_nearest(X: Union[np.ndarray, torch.Tensor], center=True):
     """
-    Orthogonalizes a matrix by finding the nearest orthogonal matrix. Nearest is
-    defined as solving the Procrustes problem via minimizing the Frobenius norm
-    of the difference between the original input matrix and the orthogonal
-    matrix. \n
-    X_orth = argmin ||X - X_orth||_F
+    Orthogonalizes a matrix by finding the nearest orthonormal matrix to an
+    input ``X``. 'Nearest' is defined as solving the orthogonal Procrustes
+    problem via minimizing the Frobenius norm of the difference between the
+    original input matrix and a orthonormal matrix that spans the same
+    dimensions as ``X``. For the initial orthonormal matrix, we use a centered
+    ``Q`` from a QR decomposition of ``X``. \n
+    ``X_orth = argmin: X_orth for ||X - X_orth||_F`` , where ``X_orth = Q @ R`` , where
+    ``R`` is a rotation matrix derived from solving the orthogonal Procrustes
+    problem for ``R = argmin: R for ||X - Q @ R||_F``. \n
 
-    Note: The solution to this problem is generally equivalent to the ZCA
-    whitening of PCA(X).
+    RH 2024
+
+    Note: The solution to this problem is generally very similar or equivalent
+    to the ZCA whitening of PCA(X).
 
     Args:
         X (ndarray):
             Matrix to orthogonalize. shape: (n_samples, n_features)
         center (bool):
             Whether to center the matrix. Default is True.
 
     Returns:
         (ndarray):
-            X_orth: orthogonalized matrix. shape: (n_samples, n_features)
+            X_orth: 
+                Orthogonalized matrix. shape: (n_samples, n_features)
     """
     if isinstance(X, np.ndarray):
-        op, qr = scipy.linalg.orthogonal_procrustes, np.linalg.qr
+        op, qr, svd = scipy.linalg.orthogonal_procrustes, np.linalg.qr, np.linalg.svd
     elif isinstance(X, torch.Tensor):
-        op, qr = torch_helpers.orthogonal_procrustes, torch.linalg.qr
+        op, qr, svd = torch_helpers.orthogonal_procrustes, torch.linalg.qr, torch.linalg.svd
 
     if center:
         X = X - X.mean(axis=0, keepdims=True)
 
     Q = qr(X)[0]
-    w, scale = op(Q, X)
-    return Q @ w
+    Q -= Q.mean(axis=0, keepdims=True)
+    R, scale = op(Q, X)
+    return Q @ R
 
 
 @njit
 def pair_orth_helper(v1, v2):
     """
     Helper function for main pairwise_orthogonalization
      function. Performs the pairwise orthogonalization
@@ -327,14 +335,15 @@
              weighted by the variance of each column of v1.
         EVR_total_unweighted (scalar):
             Average amount of variance explained in v1 by v2
     """
     assert v1.ndim == v2.ndim
     if v1.ndim==1:
         v1 = v1[:,None]
+    if v2.ndim==1:
         v2 = v2[:,None]
     assert v1.shape[1] == v2.shape[1]
     assert v1.shape[0] == v2.shape[0]
     
     if center:
         v1 = v1 - np.mean(v1, axis=0)
         v2 = v2 - np.mean(v2, axis=0)
@@ -368,15 +377,15 @@
 
     v1_var = torch.var(v1, dim=0)
     EVR = 1 - (torch.var(v1_orth, dim=0) / v1_var)
 
     EVR_total_weighted = torch.nansum(v1_var * EVR) / torch.sum(v1_var)
     EVR_total_unweighted = torch.nanmean(EVR)
     return v1_orth, EVR, EVR_total_weighted, EVR_total_unweighted
-def pairwise_orthogonalization_torch(v1, v2, center:bool=True, device='cpu'):
+def pairwise_orthogonalization_torch(v1, v2, center:bool=True):
     """
     Orthogonalizes columns of v2 off of the columns of v1
      and returns the orthogonalized v1 and the explained
      variance ratio of v2 off of v1.
     Use center=True to get guarantee zero correlation between
      columns of v1_orth and v2.
     v1: y_true, v2: y_pred
@@ -412,21 +421,22 @@
             Average amount of variance explained in v1 by v2
              weighted by the variance of each column of v1.
         EVR_total_unweighted (scalar):
             Average amount of variance explained in v1 by v2
     """
     if isinstance(v1, np.ndarray):
         v1 = torch.from_numpy(v1)
+        if isinstance(v2, np.ndarray):
+            v2 = torch.from_numpy(v2)
+        else:
+            raise ValueError("v2 must be a numpy array if v1 is a numpy array")
         return_numpy = True
-    else:
+    elif isinstance(v1, torch.Tensor):
         return_numpy = False
-    if isinstance(v2, np.ndarray):
-        v2 = torch.from_numpy(v2)
-    v1 = v1.to(device)
-    v2 = v2.to(device)
+        
     v1_orth, EVR, EVR_total_weighted, EVR_total_unweighted = pairwise_orthogonalization_torch_helper(v1, v2, center=center)
     if return_numpy:
         v1_orth = v1_orth.cpu().numpy()
         EVR = EVR.cpu().numpy()
         EVR_total_weighted = EVR_total_weighted.cpu().numpy()
         EVR_total_unweighted = EVR_total_unweighted.cpu().numpy()
     return v1_orth, EVR, EVR_total_weighted, EVR_total_unweighted
@@ -456,19 +466,23 @@
         EV_total_weighted (scalar):
             total weighted explained variance. Same as
             sklearn.metrics.explained_variance_score(y_true, y_pred, multioutput='variance_weighted')
         EV_total_unweighted (scalar):
             average of all EV values. Same as
             sklearn.metrics.explained_variance_score(y_true, y_pred, multioutput='uniform_average')
     '''
-
-    EV = 1 - np.sum((y_true - y_pred)**2, axis=0) / np.sum((y_true - np.mean(y_true, axis=0))**2, axis=0)
-    y_true_var = np.var(y_true, axis=0)
-    EV_total_weighted = np.sum( y_true_var* EV ) / np.sum(y_true_var)
-    EV_total_unweighted = np.mean(EV)
+    if isinstance(y_true, np.ndarray):
+        sum, mean, var = np.sum, np.mean, np.var
+    elif isinstance(y_true, torch.Tensor):
+        sum, mean, var = torch.sum, torch.mean, torch.var
+
+    EV = 1 - sum((y_true - y_pred)**2, axis=0) / sum((y_true - mean(y_true, axis=0))**2, axis=0)
+    y_true_var = var(y_true, axis=0)
+    EV_total_weighted = sum( y_true_var* EV ) / sum(y_true_var)
+    EV_total_unweighted = mean(EV)
 
     return EV , EV_total_weighted , EV_total_unweighted
 
 
 def pairwise_similarity(v1 , v2=None , method='pearson' , ddof=1):
     '''
     Computes similarity matrices between two sets of vectors (columns within
```

### Comparing `bnpm-0.5.1/bnpm/spectral.py` & `bnpm-0.5.2/bnpm/spectral.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from typing import Union, Tuple, List, Dict, Any, Optional
 import functools
+import math
 
 import scipy.signal
 import scipy.stats
 import numpy as np
 import matplotlib.pyplot as plt
 import torch
+import opt_einsum
 
 from . import circular
 from . import misc
 from . import torch_helpers
 from . import timeSeries
+from . import indexing
 
 
 def design_butter_bandpass(lowcut, highcut, fs, order=5, plot_pref=True):
     '''
     designs a butterworth bandpass filter.
     Makes a lowpass filter if lowcut is 0.
     Makes a highpass filter if highcut is fs/2.
@@ -366,14 +369,58 @@
         ind = [np.newaxis] * x.ndim
         ind[dim] = slice(None)
         m = m[tuple(ind)]
 
     return torch.fft.ifft(xf * m, dim=dim)
 
 
+def hilbert_fourier_domain(xf, axis=-1):
+    """
+    Computes the Fourier-transform of the analytic signal using the
+    Fourier-transformed signal. Input is ``xf`` and output is ``xhf``. Uses the
+    approach used in scipy.signal.hilbert.\n
+    RH 2024
+    
+    Args:
+        xf (torch.Tensor or np.ndarray):
+            Fourier-transformed signal data. Should be complex and have negative
+            frequencies. Generally, the output of torch.fft.fft or np.fft.fft.
+        axis (int):
+            Dimension along which to do the transformation.
+
+    Returns:
+        (nd tensor):
+            Fourier-transformed analytic signal along axis.
+    """
+    if isinstance(xf, torch.Tensor):
+        is_complex = torch.is_complex
+        zeros = functools.partial(torch.zeros, device=xf.device)
+    if isinstance(xf, np.ndarray):
+        zeros, is_complex = np.zeros, np.iscomplexobj
+    
+    assert is_complex(xf), "xf should be complex"
+
+    n = xf.shape[axis]
+
+    m = zeros(n, dtype=xf.dtype)
+    if n % 2 == 0: ## then even
+        m[0] = m[n//2] = 1
+        m[1:n//2] = 2
+    else:
+        m[0] = 1 ## then odd
+        m[1:(n+1)//2] = 2
+
+    if xf.ndim > 1:
+        ind = [np.newaxis] * xf.ndim
+        ind[axis] = slice(None)
+        m = m[tuple(ind)]
+
+    return xf * m        
+        
+
 def signal_angle_difference(x, y, center=True, window=None, axis=-1):
     """
     Computes the average angle difference between two signals.\n
     Calculated as the mean of the angle difference between the Hilbert
     transforms of the signals.\n
     Bound to the range [-pi, pi] (i.e. -180 to 180 degrees). Negative values
     indicate that x leads y.\n
@@ -509,8 +556,237 @@
     out = ifft(out, n=n)  ## xk
     out = torch_helpers.slice_along_dim(
         X=out,
         dim=-1,
         idx=slice(0, x.shape[-1]),
     )
     out = out.real if use_real else out
-    return out
+    return out
+
+
+def torch_coherence(
+    x: torch.Tensor,
+    y: torch.Tensor,
+    fs: float = 1.0,
+    window: str = 'hann',
+    nperseg: Optional[int] = None,
+    noverlap: Optional[int] = None,
+    nfft: Optional[int] = None,
+    detrend: str = 'constant',
+    axis: int = -1,
+    batch_size: Optional[int] = None,
+    pad_last_segment: Optional[float] = None,
+) -> Tuple[torch.Tensor, torch.Tensor]:
+    """
+    Computes the magnitude-squared coherence between two signals using a PyTorch
+    implementation. This function gives identical results to the
+    scipy.signal.coherence, but its much faster. A ``batch_size`` option allows
+    for large arrays to be processed on GPU.\n    
+    RH 2024
+    
+    Args:
+        x (torch.Tensor): 
+            First input signal.
+        y (torch.Tensor): 
+            Second input signal.
+        fs (float): 
+            Sampling frequency of the input signal. (Default is 1.0)
+        window (str): 
+            Type of window to apply. Supported window types are the same as
+            `scipy.signal.get_window`. (Default is 'hann')
+        nperseg (Optional[int]): 
+            Length of each segment. (Default is ``None``, which uses ``len(x) //
+            8``)
+        noverlap (Optional[int]): 
+            Number of points to overlap between segments. (Default is ``None``,
+            which uses ``nperseg // 2``)
+        nfft (Optional[int]): 
+            Number of points in the FFT used for each segment. (Default is
+            ``None``, which sets it equal to `nperseg`)
+        detrend (str): 
+            Specifies how to detrend each segment. Supported values are
+            'constant' or 'linear'. (Default is 'constant')
+        axis (int): 
+            Axis along which the coherence is calculated. (Default is -1)
+        batch_size (Optional[int]):
+            Number of segments to process at once. Used to reduce memory usage.
+            If None, then all segments are processed at once. Note that
+            ``num_segments = (x.shape[axis] - nperseg) // (nperseg - noverlap) +
+            1``. (Default is None)
+        pad_last_segment (bool):
+            Whether to pad the last segment with a value defined by this
+            argument. If None, then no padding is done. (Default is None)
+
+    Returns:
+        Tuple[torch.Tensor, torch.Tensor]: 
+            freqs (torch.Tensor): 
+                Frequencies for which the coherence is computed. Shape is
+                ``nfft // 2 + 1``.
+            coherence (torch.Tensor): 
+                Magnitude-squared coherence values. Shape is x broadcasted with
+                y and the specified axis set to ``nfft // 2 + 1``.
+
+    Example:
+        .. highlight:: python
+        .. code-block:: python
+
+            x = torch.randn(1024)
+            y = torch.randn(1024)
+            freqs, coherence = torch_coherence(x, y, fs=256)
+    """
+    ## Convert axis to positive
+    axis = axis % len(x.shape)
+
+    ## Checks
+    ### Tensor checks
+    assert isinstance(x, torch.Tensor), "x should be a torch tensor"
+    assert isinstance(y, torch.Tensor), "y should be a torch tensor"
+    ### Dims should either be the same or one of them should be 1
+    if not (x.shape == y.shape):
+        assert all([(x.shape[ii] == y.shape[ii]) or (1 in [x.shape[ii], y.shape[ii]]) for ii in range(len(x.shape))]), f"x and y should have the same shape or one of them should have shape 1 at each dimension. Found x.shape={x.shape} and y.shape={y.shape}"
+
+    if nperseg is None:
+        nperseg = len(x) // 8
+
+    if noverlap is None:
+        noverlap = nperseg // 2
+
+    if nfft is None:
+        nfft = nperseg
+
+    if window is not None:
+        window = scipy.signal.get_window(window, nperseg)
+        window = torch.tensor(window, dtype=x.dtype, device=x.device)
+
+    ## args should be greater than nfft
+    assert all([arg.shape[axis] >= nfft for arg in (x, y)]), f"Signal length along axis should be greater than nfft. Found x.shape={x.shape} and y.shape={y.shape} and nfft={nfft}"
+
+    ## Detrend the signals
+    def detrend_constant(y, axis):
+        y = y - torch.mean(y, axis=axis, keepdim=True)
+        return y
+
+    if detrend == 'linear':
+        X_linearDetrendPrep = torch.ones(nperseg, 2, dtype=y.dtype, device=y.device)
+        X_linearDetrendPrep[:, 1] = torch.arange(nperseg, dtype=y.dtype, device=y.device)
+    def detrend_linear(y, axis):
+        """
+        Uses least squares approach to remove linear trend.
+        """
+        ## Move axis to end
+        y = y.moveaxis(axis, -1)[..., None]
+        ## Prepare the design matrix
+        X = X_linearDetrendPrep[*([None] * (len(y.shape) - 2))]
+        ## Compute the coefficients
+        # beta = torch.linalg.lstsq(X, y)[0] 
+        ### Use closed form solution for least squares
+        beta = torch.linalg.inv(X.transpose(-1, -2) @ X) @ X.transpose(-1, -2) @ y
+        ## Remove the trend
+        y = y - opt_einsum.contract('...ij, ...jk -> ...ik', X, beta)
+        y = y[..., 0]
+        ## Move axis back to original position (argsort y_dims_to)
+        y = y.moveaxis(-1, axis)
+        return y
+
+    if detrend == 'constant':
+        fn_detrend = detrend_constant
+    elif detrend == 'linear':
+        fn_detrend = detrend_linear
+    else:
+        raise ValueError(f"detrend must be 'constant' or 'linear'. Found {detrend}")
+    
+    ## Initialize the coherence arrays
+    ### Get broadcasted dimensions: max(x, y) at each dimension, and nfft at axis
+    x_shape = list(x.shape)
+    y_shape = list(y.shape)
+    out_shape = [max(x_shape[i], y_shape[i]) for i in range(len(x_shape))]
+    out_shape[axis] = nfft // 2 + 1  ## rfft returns only non-negative frequencies (0 to fs/2 inclusive)
+    
+    ## Initialize sums for Welch's method
+    ### Prepare complex dtype
+    dtype_complex = torch_helpers.dtype_to_complex(x.dtype)
+    f_cross = torch.zeros(out_shape, dtype=dtype_complex, device=x.device)
+    psd1 = torch.zeros(out_shape, dtype=x.dtype, device=x.device)
+    psd2 = torch.zeros(out_shape, dtype=x.dtype, device=x.device)
+
+    ## Prepare batch generator
+    num_segments = (x.shape[axis] - nperseg) // (nperseg - noverlap) + 1
+    batch_size = max(num_segments, 1) if batch_size is None else batch_size
+    x_batches, y_batches = (indexing.batched_unfold(
+        var, 
+        dimension=axis, 
+        size=nperseg, 
+        step=nperseg - noverlap, 
+        batch_size=batch_size,
+        pad_value=pad_last_segment,
+    ) for var in (x, y))
+    
+    ## Perform Welch's averaging of FFT segments
+    for segs_x, segs_y in zip(x_batches, y_batches):
+        process_segment = lambda x: torch.fft.rfft(fn_detrend(x, axis=-1) * window, n=nfft, dim=-1)  ## Note the broadcasting of 1-D window with last dimension of x
+        segs_x = process_segment(segs_x)
+        segs_y = process_segment(segs_y)
+        f_cross += (torch.sum(torch.conj(segs_x) * segs_y, dim=axis).moveaxis(-1, axis)) / num_segments
+        psd1 += (torch.sum((torch.conj(segs_x) * segs_x).real, dim=axis).moveaxis(-1, axis)) / num_segments
+        psd2 += (torch.sum((torch.conj(segs_y) * segs_y).real, dim=axis).moveaxis(-1, axis)) / num_segments
+
+    ## Compute coherence
+    coherence = torch.abs(f_cross) ** 2 / (psd1 * psd2)
+
+    ## Generate frequency axis
+    freqs = torch.fft.rfftfreq(nfft, d=1 / fs)
+
+    ## Take the positive part of the frequency spectrum
+    ### NOTE: This is not necessary as the coherence is symmetric (always odd and real)
+    # pos_mask = freqs >= 0
+    # ### slice along axis
+    # freqs = freqs[pos_mask]
+    # coherence = torch_helpers.slice_along_dim(coherence, axis=axis, idx=pos_mask)
+    
+    return freqs, coherence
+
+
+def spectrogram_magnitude_normalization(S: torch.Tensor, k: float = 0.05):
+    """
+    Normalize spectrogram by dividing by the total power across all frequencies
+    at each time point. ``mag = mag / ((k * mean_mag_at_each_time) + (1-k))``.
+    This formula differs slightly from the forumla often used in audio
+    engineering in that it is a linear scaling, and does not apply only to data
+    above a certain threshold.
+
+    Args:
+        spectrogram (torch.Tensor):
+            A single spectrogram
+            Spectrogram should be of shape: (n_points, n_freq_bins, n_samples)  
+        k (float):
+            Weighting factor for the normalization. 0 means no normalization. 1
+            means every time point has the same power when summed across all
+            frequencies.
+
+    Returns:
+        spectrogram (tuple or torch.Tensor):
+            A single normalized spectrogram of same shape as input.
+    """
+    if k == 0:
+        return S
+    
+    ## Check inputs
+    if isinstance(S, torch.Tensor):
+        mean, sum, polar, is_complex, abs, angle  = torch.mean, torch.sum, torch.polar, torch.is_complex, torch.abs, torch.angle
+    elif isinstance(S, np.ndarray):
+        mean, sum, is_complex, abs, angle = np.mean, np.sum, np.iscomplexobj, np.abs, np.angle
+        polar = lambda mag, phase: mag * np.exp(1j * phase)
+
+    assert S.ndim == 3, "Spectrogram should be of shape: (n_points, n_freq_bins, n_samples)"
+
+    if is_complex(S) == False:
+        s_mean = mean(sum(S, dim=1, keepdims=True) , dim=0, keepdims=True)  ## Mean of the summed power across all frequencies and points. Shape (n_samples,)
+        s_norm =  S / ((k * s_mean) + (1-k))  ## Normalize the spectrogram by the mean power across all frequencies and points. Shape (n_points, n_freq_bins, n_samples)
+    
+    elif is_complex(S) == True:
+        s_mag = abs(S)
+        s_phase = angle(S)
+        s_mean = mean(sum(s_mag, dim=1, keepdims=True), dim=0, keepdims=True)  ## Mean of the summed power across all frequencies and points. Shape (n_samples,)
+        s_mag = s_mag / ((k * s_mean) + (1-k))  ## Normalize the spectrogram by the mean power across all frequencies and points. Shape (n_points, n_freq_bins, n_samples)
+        s_norm = polar(s_mag, s_phase)
+    
+    return s_norm
```

### Comparing `bnpm-0.5.1/bnpm/sql_helpers.py` & `bnpm-0.5.2/bnpm/sql_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.5.1/bnpm/stats.py` & `bnpm-0.5.2/bnpm/stats.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.5.1/bnpm/testing.py` & `bnpm-0.5.2/bnpm/testing.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.5.1/bnpm/timeSeries.py` & `bnpm-0.5.2/bnpm/timeSeries.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.5.1/bnpm/torch_helpers.py` & `bnpm-0.5.2/bnpm/torch_helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import sys
 import gc
 import copy
-from typing import Union, List, Tuple, Dict, Callable, Optional, Any
+from typing import Union, List, Tuple, Dict, Callable, Optional, Any, Iterable, Iterator, Generator
 from contextlib import contextmanager
+import warnings
 
 import torch
 from torch.utils.data import Dataset
 import numpy as np
+from tqdm import tqdm
 
 from . import indexing
 from . import misc
 
 
 ############################################
 ############ VARIABLE HELPERS ##############
@@ -24,15 +26,15 @@
     """
     # prints currently alive Tensors and Variables
     import torch
     import gc
     for obj in gc.get_objects():
         try:
             if torch.is_tensor(obj) or (hasattr(obj, 'data') and torch.is_tensor(obj.data)):
-                print(type(obj), obj.size())
+                print(type(obj), obj.size(), misc.estimate_array_size(obj))
         except:
             pass
 
 
 
 @contextmanager
 def temp_eval(module):
@@ -151,14 +153,52 @@
     torch.cuda.empty_cache()
     gc.collect()
     torch.cuda.empty_cache()
     gc.collect()
     torch.cuda.empty_cache()
 
 
+def wrap_clear_cuda_cache(func: Callable, before=True, after=True) -> Callable:
+    """
+    Wraps a function with a call to clear the CUDA cache before and/or after the
+    function call.
+
+    Args:
+        func (Callable):
+            The function to wrap.
+        before (bool):
+            If ``True``, clears the CUDA cache before calling the function.
+            (Default is ``True``)
+        after (bool):
+            If ``True``, clears the CUDA cache after calling the function.
+            (Default is ``True``)
+
+    Returns:
+        (Callable):
+            The wrapped function.
+
+    Demo:
+        .. code-block:: python
+            
+                @wrap_clear_cuda_cache
+                def my_function():
+                    pass
+    """
+    import functools
+    @functools.wraps(func)
+    def wrapper(*args, **kwargs):
+        if before:
+            clear_cuda_cache()
+        result = func(*args, **kwargs)
+        if after:
+            clear_cuda_cache()
+        return result
+    return wrapper
+
+
 def set_device(
     use_GPU: bool = True, 
     device_num: int = 0, 
     verbose: bool = True
 ) -> str:
     """
     Sets the device for PyTorch. If a GPU is available and **use_GPU** is
@@ -255,32 +295,77 @@
             init_linalg_device = torch.device(init_linalg_device)
         torch.inverse(torch.ones((1, 1), device=init_linalg_device))
         torch.linalg.qr(torch.as_tensor([[1.0, 2.0], [3.0, 4.0]], device=init_linalg_device))
 
 
 def profiler_simple(
     path_save: str = 'trace.json',
+    activities: List[str] = ['CPU', 'CUDA'],
+    with_stack: bool = False,
+    record_shapes: bool = True,
+    profile_memory: bool = True,
+    with_flops: bool = False,
+    with_modules: bool = False,
 ):
     """
     Simple profiler for PyTorch. \n
     Makes a context manager that can be used to profile code. \n
     Upon exit, will save the trace to the specified path. \n
+    Use Chrome's chrome://tracing/ to view the trace. \n
+    RH 2024
+
+    Args:
+        path_save (str):
+            The path to save the trace.
+        activities (List[str]):
+            The activities to profile. Options are ``'CPU'`` and ``'CUDA'``.
+        with_stack (bool):
+            If ``True``, records the stack, which are all the functions that
+            were called. 
+        record_shapes (bool):
+            If ``True``, records shapes of the tensors.
+        profile_memory (bool):
+            If ``True``, profiles memory usage of the tensors.
+        with_flops (bool):
+            If ``True``, records flops (floating point operations).
+        with_modules (bool):
+            If ``True``, records modules that were called.
+
+    Returns:
+        (contextmanager):
+            A context manager that can be used to profile code.
+
+    Demo:
+        .. highlight:: python
+        .. code-block:: python
+
+            with profiler_simple():
+                y = model(x)
+
+            >> Then open google chrome and go to the url chrome://tracing/ and
+            load the trace file.
     """
     from torch.profiler import profile, record_function, ProfilerActivity
     from contextlib import contextmanager
     
+    activities_dict = {
+        'CPU': ProfilerActivity.CPU,
+        'CUDA': ProfilerActivity.CUDA,
+    }
+    activities = [activities_dict[act.upper()] for act in activities]
+
     @contextmanager
     def simple_profiler(path_save: str = 'trace.json'):
         with profile(
-            activities=[ProfilerActivity.CPU, ProfilerActivity.CUDA], 
-            record_shapes=True,
-            profile_memory=True,
-            with_stack=True,
-            # with_flops=True,
-            # with_modules=True,
+            activities=activities,
+            record_shapes=record_shapes,
+            profile_memory=profile_memory,
+            with_stack=with_stack,
+            with_flops=with_flops,
+            with_modules=with_modules,
         ) as p:
             with record_function("model_inference"):
                 yield
         p.export_chrome_trace(path_save)
 
     return simple_profiler(path_save=path_save)
 
@@ -434,14 +519,147 @@
     def __len__(self):
         """
         Returns the number of samples in the dataset.
         """
         return self.len_dataset
 
 
+def map_batches_cuda(
+    batches: Union[Iterable, Iterator, Generator],
+    func: Callable,
+    device_func: str = 'cuda:0',
+    device_return: str = 'cpu',
+    pin_memory: bool = True,
+    non_blocking: bool = True,
+    progress_bar: bool = False,
+    len_batches: Optional[int] = None,
+    verbose: bool = False,
+):
+    """
+    Run batches through a user specified function on a cuda device using CUDA
+    streams. This function is useful for running batches through a model in
+    serial, but with asynchronous data transfers. This is similar to
+    torch.utils.data.DataLoader, but is simpler and doesn't implement
+    multiprocessing.
+    RH 2024
+
+    Args:
+        batches (Union[Iterable, Iterator, Generator]):
+            The batches to process. Each batch can either be a single tensor, a
+            tuple containing tensors, or other.
+        func (Callable):
+            The function to run on the batches. The function must accept the
+            items in the batches as arguments.
+        device_func (str):
+            The device to run the function on. Should typically be a CUDA device
+            (e.g., 'cuda:0'). Can also be 'cpu' or other, but this will not
+            utilize CUDA streams, memory pinning, or non-blocking transfers.
+            (Default is 'cuda:0')
+        device_return (str):
+            The device to return the results on. For this function, it will
+            typically be 'cpu'. (Default is 'cpu')
+        pin_memory (bool):
+            If ``True``, the function will pin the memory for the input tensors.
+            Ideally, the original, non-batched, tensors should be pinned.
+            However, this option will pin the memory for each batch. Warning,
+            pinning memory can cause excess and persistent memory usage.
+            (Default is ``True``)
+        non_blocking (bool):
+            If ``True``, the function will use non-blocking transfers to and
+            from the device. Warning, pinning memory can cause excess and
+            persistent memory usage. (Default is ``True``)
+        progress_bar (bool):
+            If ``True``, displays a progress bar. (Default is ``False``)
+        len_batches Optional[int]:
+            The length of the batches to be used as the total length of the
+            progress bar. If not provided, will attempt to find len(batches).
+            (Default is ``None``)
+        verbose (bool):
+            If ``True``, displays warnings. (Default is ``False``)
+
+    Returns:
+        (List):
+            results (List):
+                The results of the function run on the batches.
+
+    Example:
+        .. highlight:: python
+        .. code-block:: python
+
+            def func(x, y):
+                a, b = model.forward(x, y)
+                return a, b
+            
+            batches = ((x_i, y_i) for x_i, y_i in zip(X.pin_memory(), Y.pin_memory()))
+        
+            results = process_batches_cuda(
+                batches,
+                func,
+                device_func='cuda:0',
+                device_return='cpu',
+                pin_memory=False,
+                non_blocking=True,
+                progress_bar=True,
+                len_batches=int(math.ceil(len(X)/batch_size),
+                verbose=False,
+            )
+    """
+    results = []
+    device_func = torch.device(device_func)
+
+    assert device_func.type in ['cuda', 'cpu'], 'device must be either "cuda" or "cpu" type.'
+
+    if len_batches is None:
+        len_batches = len(batches) if hasattr(batches, '__len__') else None
+    
+    def send_to_device(batch, device, non_blocking, pin_memory):
+        """
+        Send a batch (either a single tensor, tuple containing tensors, or
+        other) to a device.
+        """
+        if isinstance(batch, torch.Tensor):
+            if pin_memory and batch.device.type != 'cuda':
+                batch = batch.pin_memory()
+
+            if batch.device != device:
+                if non_blocking:
+                    batch = batch.to(device, non_blocking=non_blocking)
+                else:
+                    batch = batch.to(device)
+
+        elif isinstance(batch, tuple):
+            batch = tuple([send_to_device(b, device, non_blocking, pin_memory) for b in batch])
+        
+        return batch
+
+    if device_func.type == 'cuda':
+        stream = torch.cuda.Stream(device=device_func)  ## create a stream
+        for ii, batch in tqdm(enumerate(batches), total=len_batches, disable=not progress_bar):
+            if not isinstance(batch, tuple):  ## Make batch a tuple
+                batch = (batch,)
+            with torch.cuda.stream(stream):  ## run on new stream
+                batch = send_to_device(batch=batch, device=device_func, non_blocking=non_blocking, pin_memory=pin_memory)
+                outs = func(*batch)  ## run func on batch
+                outs = send_to_device(batch=outs, device=device_return, non_blocking=non_blocking, pin_memory=False)
+                results.append(outs)  ## append to results
+        torch.cuda.synchronize()  ## wait for all streams to finish
+    else:
+        warnings.warn('device_func is not cuda. No streams will be used.') if verbose else None
+        for ii, batch in tqdm(enumerate(batches), total=len_batches, disable=not progress_bar):
+            ## Make batch a tuple
+            if not isinstance(batch, tuple):
+                batch = (batch,)
+            batch = send_to_device(batch=batch, device=device_func, non_blocking=non_blocking, pin_memory=pin_memory)
+            outs = func(*batch)
+            outs = send_to_device(batch=outs, device=device_return, non_blocking=non_blocking, pin_memory=False)
+            results.append(outs)
+
+    return results
+
+
 ##################################################################
 ############# STUFF PYTORCH SHOULD ALREADY HAVE ##################
 ##################################################################
 
 
 @misc.wrapper_flexible_args(['dim', 'axis'])
 @misc.wrapper_flexible_args(['keepdim', 'keepdims'])
@@ -867,27 +1085,27 @@
     return (X - mean) / std
 
 
 @misc.wrapper_flexible_args(['dim', 'axis'])
 def slice_along_dim(
     X: torch.Tensor, 
     dim: int, 
-    idx: int
+    idx: Union[int, slice, List[int], torch.Tensor]
 ) -> torch.Tensor:
     """
     Slices a tensor along a specified dimension.
     RH 2022
 
     Args:
         X (torch.Tensor): 
             Tensor to slice.
         dim (int): 
             Dimension to slice along.
-        idx (int): 
-            Index to slice at.
+        idx Union[int, slice, List[int], torch.Tensor]:
+            Index / slice / list of indices / tensor of indices to slice with.
 
     Returns:
         (torch.Tensor): 
             sliced_tensor (torch.Tensor):
                 Sliced tensor.
     """
     slices = [slice(None)] * X.ndim
@@ -942,56 +1160,54 @@
 
     U, S, V = torch.linalg.svd((B.T @ A).T, full_matrices=False)
     R = U @ V
     scale = S.sum()
     return R, scale
 
 
-#########################################################
-############ INTRA-MODULE HELPER FUNCTIONS ##############
-#########################################################
-
-def _convert_size(
-    size: Union[int, float], 
-    return_size: str = 'GB'
-) -> float:
+def dtype_to_complex(dtype: torch.dtype) -> torch.dtype:
     """
-    Converts the size in bytes to another unit (TB, GB, MB, KB, or B).
-    RH 2021
+    Converts a real torch dtype to a complex dtype. \n
+    Pytorch 2.2 has this, but it crashes after calling it ~100 times. \n
+    RH 2024
 
     Args:
-        size (Union[int, float]): 
-            Size in bytes.
-        return_size (str): 
-            Unit to which the size should be converted. Either \n
-            * ``'TB'``: Terabytes
-            * ``'GB'``: Gigabytes
-            * ``'MB'``: Megabytes
-            * ``'KB'``: Kilobytes
-            * ``'B'``: Bytes \n
-            (Default is ``'GB'``)
+        dtype (torch.dtype): 
+            Real dtype to convert to complex dtype.
 
     Returns:
-        (float): 
-            out_size (float):
-                Size converted to the specified unit.
-
-    Example:
-        .. highlight:: python
-        .. code-block:: python
-
-            size_in_gb = _convert_size(1000000000, 'GB')
+        (torch.dtype): 
+            complex_dtype (torch.dtype):
+                Complex dtype.
+    """
+    map = {
+        torch.float16: torch.complex32,
+        torch.bfloat16: torch.complex64,
+        torch.float32: torch.complex64,
+        torch.float64: torch.complex128,
+    }
+    if dtype not in map:
+        raise ValueError(f'{dtype} does not have a complex equivalent in map.')
+    return map[dtype]
+def dtype_to_real(dtype: torch.dtype) -> torch.dtype:
     """
+    Converts a complex torch dtype to a real dtype. \n
+    Pytorch 2.2 has this, but it crashes after calling it ~100 times. \n
+    RH 2024
 
-    if return_size == 'TB':
-        out_size = size / 1000000000000
-    elif return_size == 'GB':
-        out_size = size / 1000000000
-    elif return_size == 'MB':
-        out_size = size / 1000000
-    elif return_size == 'KB':
-        out_size = size / 1000
-    elif return_size == 'B':
-        out_size = size / 1
-
-    return out_size
+    Args:
+        dtype (torch.dtype): 
+            Complex dtype to convert to real dtype.
 
+    Returns:
+        (torch.dtype): 
+            real_dtype (torch.dtype):
+                Real dtype.
+    """
+    map = {
+        torch.complex32: torch.float16,
+        torch.complex64: torch.float32,
+        torch.complex128: torch.float64,
+    }
+    if dtype not in map:
+        raise ValueError(f'{dtype} does not have a real equivalent in map.')
+    return map[dtype]
```

### Comparing `bnpm-0.5.1/bnpm/video.py` & `bnpm-0.5.2/bnpm/video.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.5.1/bnpm/welford_moving.py` & `bnpm-0.5.2/bnpm/welford_moving.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.5.1/bnpm/welford_moving_2D.py` & `bnpm-0.5.2/bnpm/welford_moving_2D.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.5.1/bnpm.egg-info/PKG-INFO` & `bnpm-0.5.2/bnpm.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bnpm
-Version: 0.5.1
+Version: 0.5.2
 Summary: A library of useful modules for data analysis.
 Home-page: https://github.com/RichieHakim/basic_neural_processing_modules
 Author: Richard Hakim
 License: LICENSE
 Keywords: data analysis,machine learning,neuroscience
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -14,35 +14,36 @@
 Requires-Dist: ipywidgets; extra == "all"
 Requires-Dist: kornia; extra == "all"
 Requires-Dist: matplotlib; extra == "all"
 Requires-Dist: natsort; extra == "all"
 Requires-Dist: numba; extra == "all"
 Requires-Dist: numpy; extra == "all"
 Requires-Dist: opencv_contrib_python; extra == "all"
+Requires-Dist: opt_einsum; extra == "all"
 Requires-Dist: optuna; extra == "all"
 Requires-Dist: optuna_integration; extra == "all"
 Requires-Dist: pandas; extra == "all"
 Requires-Dist: paramiko; extra == "all"
 Requires-Dist: psutil; extra == "all"
 Requires-Dist: PyYAML; extra == "all"
 Requires-Dist: pytest; extra == "all"
+Requires-Dist: hypothesis; extra == "all"
 Requires-Dist: scikit_learn; extra == "all"
 Requires-Dist: tqdm; extra == "all"
 Requires-Dist: seaborn; extra == "all"
 Requires-Dist: sparse; extra == "all"
 Requires-Dist: scipy; extra == "all"
 Requires-Dist: sqlalchemy; extra == "all"
 Requires-Dist: pymysql; extra == "all"
 Requires-Dist: xxhash; extra == "all"
 Requires-Dist: wandb; extra == "all"
 Requires-Dist: torch; extra == "all"
 Requires-Dist: torchvision; extra == "all"
 Requires-Dist: torchaudio; extra == "all"
 Requires-Dist: tables; extra == "all"
-Requires-Dist: opt_einsum; extra == "all"
 Requires-Dist: pulp; extra == "all"
 Requires-Dist: spconv; extra == "all"
 Requires-Dist: torch_sparse; extra == "all"
 Requires-Dist: av; extra == "all"
 Requires-Dist: pynwb; extra == "all"
 Requires-Dist: sendgrid; extra == "all"
 Requires-Dist: pycuda; extra == "all"
@@ -60,35 +61,36 @@
 Requires-Dist: ipywidgets; extra == "all-latest"
 Requires-Dist: kornia; extra == "all-latest"
 Requires-Dist: matplotlib; extra == "all-latest"
 Requires-Dist: natsort; extra == "all-latest"
 Requires-Dist: numba; extra == "all-latest"
 Requires-Dist: numpy; extra == "all-latest"
 Requires-Dist: opencv_contrib_python; extra == "all-latest"
+Requires-Dist: opt_einsum; extra == "all-latest"
 Requires-Dist: optuna; extra == "all-latest"
 Requires-Dist: optuna_integration; extra == "all-latest"
 Requires-Dist: pandas; extra == "all-latest"
 Requires-Dist: paramiko; extra == "all-latest"
 Requires-Dist: psutil; extra == "all-latest"
 Requires-Dist: PyYAML; extra == "all-latest"
 Requires-Dist: pytest; extra == "all-latest"
+Requires-Dist: hypothesis; extra == "all-latest"
 Requires-Dist: scikit_learn; extra == "all-latest"
 Requires-Dist: tqdm; extra == "all-latest"
 Requires-Dist: seaborn; extra == "all-latest"
 Requires-Dist: sparse; extra == "all-latest"
 Requires-Dist: scipy; extra == "all-latest"
 Requires-Dist: sqlalchemy; extra == "all-latest"
 Requires-Dist: pymysql; extra == "all-latest"
 Requires-Dist: xxhash; extra == "all-latest"
 Requires-Dist: wandb; extra == "all-latest"
 Requires-Dist: torch; extra == "all-latest"
 Requires-Dist: torchvision; extra == "all-latest"
 Requires-Dist: torchaudio; extra == "all-latest"
 Requires-Dist: tables; extra == "all-latest"
-Requires-Dist: opt_einsum; extra == "all-latest"
 Requires-Dist: pulp; extra == "all-latest"
 Requires-Dist: spconv; extra == "all-latest"
 Requires-Dist: torch_sparse; extra == "all-latest"
 Requires-Dist: av; extra == "all-latest"
 Requires-Dist: pynwb; extra == "all-latest"
 Requires-Dist: sendgrid; extra == "all-latest"
 Requires-Dist: pycuda; extra == "all-latest"
@@ -106,22 +108,24 @@
 Requires-Dist: kornia; extra == "core"
 Requires-Dist: matplotlib; extra == "core"
 Requires-Dist: numba; extra == "core"
 Requires-Dist: scikit_learn; extra == "core"
 Requires-Dist: tqdm; extra == "core"
 Requires-Dist: h5py; extra == "core"
 Requires-Dist: opencv_contrib_python; extra == "core"
+Requires-Dist: opt_einsum; extra == "core"
 Requires-Dist: optuna; extra == "core"
 Requires-Dist: optuna_integration; extra == "core"
 Requires-Dist: sparse; extra == "core"
 Requires-Dist: natsort; extra == "core"
 Requires-Dist: paramiko; extra == "core"
 Requires-Dist: pandas; extra == "core"
 Requires-Dist: psutil; extra == "core"
 Requires-Dist: pytest; extra == "core"
+Requires-Dist: hypothesis; extra == "core"
 Requires-Dist: PyYAML; extra == "core"
 Requires-Dist: torch; extra == "core"
 Requires-Dist: torchvision; extra == "core"
 Requires-Dist: torchaudio; extra == "core"
 Requires-Dist: ipywidgets; extra == "core"
 Requires-Dist: eva_decord; extra == "core"
 Requires-Dist: wandb; extra == "core"
@@ -133,22 +137,24 @@
 Requires-Dist: kornia; extra == "core-latest"
 Requires-Dist: matplotlib; extra == "core-latest"
 Requires-Dist: numba; extra == "core-latest"
 Requires-Dist: scikit_learn; extra == "core-latest"
 Requires-Dist: tqdm; extra == "core-latest"
 Requires-Dist: h5py; extra == "core-latest"
 Requires-Dist: opencv_contrib_python; extra == "core-latest"
+Requires-Dist: opt_einsum; extra == "core-latest"
 Requires-Dist: optuna; extra == "core-latest"
 Requires-Dist: optuna_integration; extra == "core-latest"
 Requires-Dist: sparse; extra == "core-latest"
 Requires-Dist: natsort; extra == "core-latest"
 Requires-Dist: paramiko; extra == "core-latest"
 Requires-Dist: pandas; extra == "core-latest"
 Requires-Dist: psutil; extra == "core-latest"
 Requires-Dist: pytest; extra == "core-latest"
+Requires-Dist: hypothesis; extra == "core-latest"
 Requires-Dist: PyYAML; extra == "core-latest"
 Requires-Dist: torch; extra == "core-latest"
 Requires-Dist: torchvision; extra == "core-latest"
 Requires-Dist: torchaudio; extra == "core-latest"
 Requires-Dist: ipywidgets; extra == "core-latest"
 Requires-Dist: eva_decord; extra == "core-latest"
 Requires-Dist: wandb; extra == "core-latest"
@@ -160,22 +166,24 @@
 Requires-Dist: kornia; extra == "core-cv2headless"
 Requires-Dist: matplotlib; extra == "core-cv2headless"
 Requires-Dist: numba; extra == "core-cv2headless"
 Requires-Dist: scikit_learn; extra == "core-cv2headless"
 Requires-Dist: tqdm; extra == "core-cv2headless"
 Requires-Dist: h5py; extra == "core-cv2headless"
 Requires-Dist: opencv_contrib_python_headless; extra == "core-cv2headless"
+Requires-Dist: opt_einsum; extra == "core-cv2headless"
 Requires-Dist: optuna; extra == "core-cv2headless"
 Requires-Dist: optuna_integration; extra == "core-cv2headless"
 Requires-Dist: sparse; extra == "core-cv2headless"
 Requires-Dist: natsort; extra == "core-cv2headless"
 Requires-Dist: paramiko; extra == "core-cv2headless"
 Requires-Dist: pandas; extra == "core-cv2headless"
 Requires-Dist: psutil; extra == "core-cv2headless"
 Requires-Dist: pytest; extra == "core-cv2headless"
+Requires-Dist: hypothesis; extra == "core-cv2headless"
 Requires-Dist: PyYAML; extra == "core-cv2headless"
 Requires-Dist: torch; extra == "core-cv2headless"
 Requires-Dist: torchvision; extra == "core-cv2headless"
 Requires-Dist: torchaudio; extra == "core-cv2headless"
 Requires-Dist: ipywidgets; extra == "core-cv2headless"
 Requires-Dist: eva_decord; extra == "core-cv2headless"
 Requires-Dist: wandb; extra == "core-cv2headless"
@@ -187,22 +195,24 @@
 Requires-Dist: kornia; extra == "core-latest-cv2headless"
 Requires-Dist: matplotlib; extra == "core-latest-cv2headless"
 Requires-Dist: numba; extra == "core-latest-cv2headless"
 Requires-Dist: scikit_learn; extra == "core-latest-cv2headless"
 Requires-Dist: tqdm; extra == "core-latest-cv2headless"
 Requires-Dist: h5py; extra == "core-latest-cv2headless"
 Requires-Dist: opencv_contrib_python_headless; extra == "core-latest-cv2headless"
+Requires-Dist: opt_einsum; extra == "core-latest-cv2headless"
 Requires-Dist: optuna; extra == "core-latest-cv2headless"
 Requires-Dist: optuna_integration; extra == "core-latest-cv2headless"
 Requires-Dist: sparse; extra == "core-latest-cv2headless"
 Requires-Dist: natsort; extra == "core-latest-cv2headless"
 Requires-Dist: paramiko; extra == "core-latest-cv2headless"
 Requires-Dist: pandas; extra == "core-latest-cv2headless"
 Requires-Dist: psutil; extra == "core-latest-cv2headless"
 Requires-Dist: pytest; extra == "core-latest-cv2headless"
+Requires-Dist: hypothesis; extra == "core-latest-cv2headless"
 Requires-Dist: PyYAML; extra == "core-latest-cv2headless"
 Requires-Dist: torch; extra == "core-latest-cv2headless"
 Requires-Dist: torchvision; extra == "core-latest-cv2headless"
 Requires-Dist: torchaudio; extra == "core-latest-cv2headless"
 Requires-Dist: ipywidgets; extra == "core-latest-cv2headless"
 Requires-Dist: eva_decord; extra == "core-latest-cv2headless"
 Requires-Dist: wandb; extra == "core-latest-cv2headless"
```

### Comparing `bnpm-0.5.1/bnpm.egg-info/SOURCES.txt` & `bnpm-0.5.2/bnpm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bnpm-0.5.1/bnpm.egg-info/requires.txt` & `bnpm-0.5.2/bnpm.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -5,35 +5,36 @@
 ipywidgets
 kornia
 matplotlib
 natsort
 numba
 numpy
 opencv_contrib_python
+opt_einsum
 optuna
 optuna_integration
 pandas
 paramiko
 psutil
 PyYAML
 pytest
+hypothesis
 scikit_learn
 tqdm
 seaborn
 sparse
 scipy
 sqlalchemy
 pymysql
 xxhash
 wandb
 torch
 torchvision
 torchaudio
 tables
-opt_einsum
 pulp
 spconv
 torch_sparse
 av
 pynwb
 sendgrid
 pycuda
@@ -52,35 +53,36 @@
 ipywidgets
 kornia
 matplotlib
 natsort
 numba
 numpy
 opencv_contrib_python
+opt_einsum
 optuna
 optuna_integration
 pandas
 paramiko
 psutil
 PyYAML
 pytest
+hypothesis
 scikit_learn
 tqdm
 seaborn
 sparse
 scipy
 sqlalchemy
 pymysql
 xxhash
 wandb
 torch
 torchvision
 torchaudio
 tables
-opt_einsum
 pulp
 spconv
 torch_sparse
 av
 pynwb
 sendgrid
 pycuda
@@ -99,22 +101,24 @@
 kornia
 matplotlib
 numba
 scikit_learn
 tqdm
 h5py
 opencv_contrib_python
+opt_einsum
 optuna
 optuna_integration
 sparse
 natsort
 paramiko
 pandas
 psutil
 pytest
+hypothesis
 PyYAML
 torch
 torchvision
 torchaudio
 ipywidgets
 eva_decord
 wandb
@@ -127,22 +131,24 @@
 kornia
 matplotlib
 numba
 scikit_learn
 tqdm
 h5py
 opencv_contrib_python_headless
+opt_einsum
 optuna
 optuna_integration
 sparse
 natsort
 paramiko
 pandas
 psutil
 pytest
+hypothesis
 PyYAML
 torch
 torchvision
 torchaudio
 ipywidgets
 eva_decord
 wandb
@@ -155,22 +161,24 @@
 kornia
 matplotlib
 numba
 scikit_learn
 tqdm
 h5py
 opencv_contrib_python
+opt_einsum
 optuna
 optuna_integration
 sparse
 natsort
 paramiko
 pandas
 psutil
 pytest
+hypothesis
 PyYAML
 torch
 torchvision
 torchaudio
 ipywidgets
 eva_decord
 wandb
@@ -183,22 +191,24 @@
 kornia
 matplotlib
 numba
 scikit_learn
 tqdm
 h5py
 opencv_contrib_python_headless
+opt_einsum
 optuna
 optuna_integration
 sparse
 natsort
 paramiko
 pandas
 psutil
 pytest
+hypothesis
 PyYAML
 torch
 torchvision
 torchaudio
 ipywidgets
 eva_decord
 wandb
```

### Comparing `bnpm-0.5.1/setup.py` & `bnpm-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,36 +61,37 @@
     'kornia',
     'matplotlib',
     'numba',
     'scikit_learn',
     'tqdm',
     'h5py',
     'opencv_contrib_python',
+    'opt_einsum',
     'optuna',
     'optuna_integration',
     'sparse',
     'natsort',
     'paramiko',
     'pandas',
     'psutil',
     'pytest',
+    'hypothesis',
     'PyYAML',
     'torch',
     'torchvision',
     'torchaudio',
     'ipywidgets',
     'eva_decord',
     'wandb',
     'sqlalchemy',
     'pymysql',
 ]}
 
 deps_advanced = {dep: deps_all_dict[dep] for dep in [
     'tables',
-    'opt_einsum',
     # 'rolling_quantiles',
     'pulp',
     'spconv',
     'torch_sparse',
     'av',
     'pynwb',
     'sendgrid',
```

