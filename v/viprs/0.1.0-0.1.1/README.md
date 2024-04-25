# Comparing `tmp/viprs-0.1.0.tar.gz` & `tmp/viprs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viprs-0.1.0.tar", last modified: Mon Apr  8 01:00:25 2024, max compression
+gzip compressed data, was "viprs-0.1.1.tar", last modified: Thu Apr 25 18:33:17 2024, max compression
```

## Comparing `viprs-0.1.0.tar` & `viprs-0.1.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:00:25.413947 viprs-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-08 01:00:05.000000 viprs-0.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-08 01:00:05.000000 viprs-0.1.0/CITATION.md
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-08 01:00:05.000000 viprs-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-08 01:00:05.000000 viprs-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-08 01:00:25.413947 viprs-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-08 01:00:05.000000 viprs-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:00:25.409947 viprs-0.1.0/bin/
--rw-r--r--   0 runner    (1001) docker     (127)     6796 2024-04-08 01:00:05.000000 viprs-0.1.0/bin/viprs_evaluate
--rw-r--r--   0 runner    (1001) docker     (127)    30136 2024-04-08 01:00:05.000000 viprs-0.1.0/bin/viprs_fit
--rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-04-08 01:00:05.000000 viprs-0.1.0/bin/viprs_score
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-08 01:00:05.000000 viprs-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-08 01:00:05.000000 viprs-0.1.0/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-08 01:00:05.000000 viprs-0.1.0/requirements-optional.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-08 01:00:05.000000 viprs-0.1.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-08 01:00:05.000000 viprs-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 01:00:25.413947 viprs-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     7540 2024-04-08 01:00:05.000000 viprs-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:00:25.409947 viprs-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-04-08 01:00:05.000000 viprs-0.1.0/tests/test_basic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:00:25.409947 viprs-0.1.0/viprs/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:00:25.409947 viprs-0.1.0/viprs/eval/
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9711 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/eval/binary_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/eval/continuous_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/eval/pseudo_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:00:25.409947 viprs-0.1.0/viprs/model/
--rw-r--r--   0 runner    (1001) docker     (127)    13932 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/model/BayesPRSModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/model/LDPredInf.py
--rw-r--r--   0 runner    (1001) docker     (127)    34542 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/model/VIPRS.py
--rw-r--r--   0 runner    (1001) docker     (127)    13713 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/model/VIPRSMix.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:00:25.413947 viprs-0.1.0/viprs/model/gridsearch/
--rw-r--r--   0 runner    (1001) docker     (127)     9090 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/model/gridsearch/HyperparameterGrid.py
--rw-r--r--   0 runner    (1001) docker     (127)    18510 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/model/gridsearch/HyperparameterSearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/model/gridsearch/VIPRSBMA.py
--rw-r--r--   0 runner    (1001) docker     (127)    16599 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/model/gridsearch/VIPRSGrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/model/gridsearch/VIPRSGridSearch.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/model/gridsearch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:00:25.413947 viprs-0.1.0/viprs/model/vi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/model/vi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23486 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/model/vi/e_step.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/model/vi/e_step.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    16795 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/model/vi/e_step.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/model/vi/e_step_cpp.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     7236 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/model/vi/e_step_cpp.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:00:25.413947 viprs-0.1.0/viprs/plot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/plot/diagnostics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:00:25.413947 viprs-0.1.0/viprs/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/utils/OptimizeResult.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/utils/compute_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/utils/math_utils.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-04-08 01:00:05.000000 viprs-0.1.0/viprs/utils/math_utils.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:00:25.413947 viprs-0.1.0/viprs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-08 01:00:25.000000 viprs-0.1.0/viprs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-08 01:00:25.000000 viprs-0.1.0/viprs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 01:00:25.000000 viprs-0.1.0/viprs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 01:00:24.000000 viprs-0.1.0/viprs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-08 01:00:25.000000 viprs-0.1.0/viprs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-08 01:00:25.000000 viprs-0.1.0/viprs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:33:17.912455 viprs-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-04-25 18:32:57.000000 viprs-0.1.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-25 18:32:57.000000 viprs-0.1.1/CITATION.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-25 18:32:57.000000 viprs-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-25 18:32:57.000000 viprs-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-25 18:33:17.912455 viprs-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-25 18:32:57.000000 viprs-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:33:17.904456 viprs-0.1.1/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-04-25 18:32:57.000000 viprs-0.1.1/bin/viprs_evaluate
+-rw-r--r--   0 runner    (1001) docker     (127)    30137 2024-04-25 18:32:57.000000 viprs-0.1.1/bin/viprs_fit
+-rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-04-25 18:32:57.000000 viprs-0.1.1/bin/viprs_score
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-25 18:32:57.000000 viprs-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-25 18:32:57.000000 viprs-0.1.1/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-25 18:32:57.000000 viprs-0.1.1/requirements-optional.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 18:32:57.000000 viprs-0.1.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-25 18:32:57.000000 viprs-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 18:33:17.912455 viprs-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-25 18:32:57.000000 viprs-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:33:17.904456 viprs-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-04-25 18:32:57.000000 viprs-0.1.1/tests/test_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:33:17.904456 viprs-0.1.1/viprs/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-25 18:32:57.000000 viprs-0.1.1/viprs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:33:17.908455 viprs-0.1.1/viprs/eval/
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-25 18:32:57.000000 viprs-0.1.1/viprs/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9711 2024-04-25 18:32:57.000000 viprs-0.1.1/viprs/eval/binary_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-04-25 18:32:57.000000 viprs-0.1.1/viprs/eval/continuous_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-04-25 18:32:57.000000 viprs-0.1.1/viprs/eval/pseudo_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:33:17.908455 viprs-0.1.1/viprs/model/
+-rw-r--r--   0 runner    (1001) docker     (127)    13934 2024-04-25 18:32:57.000000 viprs-0.1.1/viprs/model/BayesPRSModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-25 18:32:57.000000 viprs-0.1.1/viprs/model/LDPredInf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34542 2024-04-25 18:32:57.000000 viprs-0.1.1/viprs/model/VIPRS.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13713 2024-04-25 18:32:57.000000 viprs-0.1.1/viprs/model/VIPRSMix.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:32:57.000000 viprs-0.1.1/viprs/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:33:17.908455 viprs-0.1.1/viprs/model/gridsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)     9090 2024-04-25 18:32:57.000000 viprs-0.1.1/viprs/model/gridsearch/HyperparameterGrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18510 2024-04-25 18:32:57.000000 viprs-0.1.1/viprs/model/gridsearch/HyperparameterSearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-25 18:32:57.000000 viprs-0.1.1/viprs/model/gridsearch/VIPRSBMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16599 2024-04-25 18:32:57.000000 viprs-0.1.1/viprs/model/gridsearch/VIPRSGrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-25 18:32:57.000000 viprs-0.1.1/viprs/model/gridsearch/VIPRSGridSearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:32:57.000000 viprs-0.1.1/viprs/model/gridsearch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:33:17.908455 viprs-0.1.1/viprs/model/vi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:32:57.000000 viprs-0.1.1/viprs/model/vi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23486 2024-04-25 18:32:57.000000 viprs-0.1.1/viprs/model/vi/e_step.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-25 18:32:57.000000 viprs-0.1.1/viprs/model/vi/e_step.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    16795 2024-04-25 18:32:57.000000 viprs-0.1.1/viprs/model/vi/e_step.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-25 18:32:57.000000 viprs-0.1.1/viprs/model/vi/e_step_cpp.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-04-25 18:32:57.000000 viprs-0.1.1/viprs/model/vi/e_step_cpp.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:33:17.908455 viprs-0.1.1/viprs/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:32:57.000000 viprs-0.1.1/viprs/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-25 18:32:57.000000 viprs-0.1.1/viprs/plot/diagnostics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:33:17.912455 viprs-0.1.1/viprs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-25 18:32:57.000000 viprs-0.1.1/viprs/utils/OptimizeResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:32:57.000000 viprs-0.1.1/viprs/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-25 18:32:57.000000 viprs-0.1.1/viprs/utils/compute_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-25 18:32:57.000000 viprs-0.1.1/viprs/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-25 18:32:57.000000 viprs-0.1.1/viprs/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-25 18:32:57.000000 viprs-0.1.1/viprs/utils/math_utils.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-04-25 18:32:57.000000 viprs-0.1.1/viprs/utils/math_utils.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:33:17.912455 viprs-0.1.1/viprs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-25 18:33:17.000000 viprs-0.1.1/viprs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-25 18:33:17.000000 viprs-0.1.1/viprs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 18:33:17.000000 viprs-0.1.1/viprs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 18:33:16.000000 viprs-0.1.1/viprs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-25 18:33:17.000000 viprs-0.1.1/viprs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 18:33:17.000000 viprs-0.1.1/viprs.egg-info/top_level.txt
```

### Comparing `viprs-0.1.0/CHANGELOG.md` & `viprs-0.1.1/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.1.1] - 2024-04-24
+
+### Changed
+
+- Fixed bugs in the E-Step benchmarking script.
+- Re-wrote the logic for finding BLAS libraries in the `setup.py` script. :crossed_fingers:
+- Fixed bugs in CI / GitHub Actions scripts.
+
+### Added
+
+- `Dockerfile`s for both `cli` and `jupyter` modes.
+
 ## [0.1.0] - 2024-04-05
 
 A large scale restructuring of the code base to improve efficiency and usability.
 
 ### Changed
 
 - Moved plotting script to its own separate module.
```

### Comparing `viprs-0.1.0/CITATION.md` & `viprs-0.1.1/CITATION.md`

 * *Files identical despite different names*

### Comparing `viprs-0.1.0/LICENSE` & `viprs-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `viprs-0.1.0/PKG-INFO` & `viprs-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viprs
-Version: 0.1.0
+Version: 0.1.1
 Summary: Variational Inference of Polygenic Risk Scores (VIPRS)
 Home-page: https://github.com/shz9/viprs
 Author: Shadi Zabad
 Author-email: shadi.zabad@mail.mcgill.ca
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `viprs-0.1.0/README.md` & `viprs-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `viprs-0.1.0/bin/viprs_evaluate` & `viprs-0.1.1/bin/viprs_evaluate`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 # Read the covariates file:
 if args.covariates_file is not None:
     sample_table.read_covariates_file(args.covariates_file)
 
 # Make sure that samples remain after reading both:
 assert sample_table.n > 0, "No samples found after merging the covariates and phenotype files."
 
-prs_df = pd.read_csv(args.prs_file, sep='\t')
+prs_df = pd.read_csv(args.prs_file, sep=r'\s+')
 
 # Merge the PRS data with the phenotype data:
 prs_df = prs_df.merge(sample_table.get_individual_table(), on=['FID', 'IID'])
 
 assert len(prs_df) > 0, "No common samples found in the PRS and phenotype files."
 
 sample_table.filter_samples(keep_samples=prs_df.IID.values)
```

### Comparing `viprs-0.1.0/bin/viprs_fit` & `viprs-0.1.1/bin/viprs_fit`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     python -m viprs_fit -l /path/to/ld_matrices/ -s /path/to/sumstats/ -o /path/to/output/ --sumstats-format custom
                        --custom-sumstats-mapper rsid=SNP,eff_allele=A1,beta=BETA
 
 """
 
 import os.path as osp
 
+
 def check_args(args):
     """
     Check the validity, consistency, and completeness of the commandline arguments.
     """
 
     from magenpy.utils.system_utils import get_filenames, is_path_writable
```

### Comparing `viprs-0.1.0/bin/viprs_score` & `viprs-0.1.1/bin/viprs_score`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import os.path as osp
 import argparse
 import viprs as vp
 from magenpy.utils.system_utils import makedir, get_filenames
 from magenpy.GWADataLoader import GWADataLoader
 from viprs.model.BayesPRSModel import BayesPRSModel
 
+
 print(fr"""
         **********************************************
                     _____
             ___   _____(_)________ ________________
             __ | / /__  / ___  __ \__  ___/__  ___/
             __ |/ / _  /  __  /_/ /_  /    _(__  )
             _____/  /_/   _  .___/ /_/     /____/
```

### Comparing `viprs-0.1.0/tests/test_basic.py` & `viprs-0.1.1/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `viprs-0.1.0/viprs/eval/__init__.py` & `viprs-0.1.1/viprs/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `viprs-0.1.0/viprs/eval/binary_metrics.py` & `viprs-0.1.1/viprs/eval/binary_metrics.py`

 * *Files identical despite different names*

### Comparing `viprs-0.1.0/viprs/eval/continuous_metrics.py` & `viprs-0.1.1/viprs/eval/continuous_metrics.py`

 * *Files identical despite different names*

### Comparing `viprs-0.1.0/viprs/eval/pseudo_metrics.py` & `viprs-0.1.1/viprs/eval/pseudo_metrics.py`

 * *Files identical despite different names*

### Comparing `viprs-0.1.0/viprs/model/BayesPRSModel.py` & `viprs-0.1.1/viprs/model/BayesPRSModel.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,15 +301,15 @@
             * Columns with `VAR_BETA`, will be assigned to `self.post_var_beta`.
         
         :param parameter_table: A pandas table or dataframe.
         """
 
         self.pip, self.post_mean_beta, self.post_var_beta = self.harmonize_data(parameter_table=parameter_table)
 
-    def read_inferred_parameters(self, f_names, sep="\t"):
+    def read_inferred_parameters(self, f_names, sep=r"\s+"):
         """
         Read a file with the inferred parameters.
         :param f_names: A path (or list of paths) to the file with the effect sizes.
         :param sep: The delimiter for the file(s).
         """
 
         if isinstance(f_names, str):
```

### Comparing `viprs-0.1.0/viprs/model/LDPredInf.py` & `viprs-0.1.1/viprs/model/LDPredInf.py`

 * *Files identical despite different names*

### Comparing `viprs-0.1.0/viprs/model/VIPRS.py` & `viprs-0.1.1/viprs/model/VIPRS.py`

 * *Files identical despite different names*

### Comparing `viprs-0.1.0/viprs/model/VIPRSMix.py` & `viprs-0.1.1/viprs/model/VIPRSMix.py`

 * *Files identical despite different names*

### Comparing `viprs-0.1.0/viprs/model/gridsearch/HyperparameterGrid.py` & `viprs-0.1.1/viprs/model/gridsearch/HyperparameterGrid.py`

 * *Files identical despite different names*

### Comparing `viprs-0.1.0/viprs/model/gridsearch/HyperparameterSearch.py` & `viprs-0.1.1/viprs/model/gridsearch/HyperparameterSearch.py`

 * *Files identical despite different names*

### Comparing `viprs-0.1.0/viprs/model/gridsearch/VIPRSBMA.py` & `viprs-0.1.1/viprs/model/gridsearch/VIPRSBMA.py`

 * *Files identical despite different names*

### Comparing `viprs-0.1.0/viprs/model/gridsearch/VIPRSGrid.py` & `viprs-0.1.1/viprs/model/gridsearch/VIPRSGrid.py`

 * *Files identical despite different names*

### Comparing `viprs-0.1.0/viprs/model/gridsearch/VIPRSGridSearch.py` & `viprs-0.1.1/viprs/model/gridsearch/VIPRSGridSearch.py`

 * *Files identical despite different names*

### Comparing `viprs-0.1.0/viprs/model/vi/e_step.hpp` & `viprs-0.1.1/viprs/model/vi/e_step.hpp`

 * *Files identical despite different names*

### Comparing `viprs-0.1.0/viprs/model/vi/e_step.pxd` & `viprs-0.1.1/viprs/model/vi/e_step.pxd`

 * *Files identical despite different names*

### Comparing `viprs-0.1.0/viprs/model/vi/e_step.pyx` & `viprs-0.1.1/viprs/model/vi/e_step.pyx`

 * *Files identical despite different names*

### Comparing `viprs-0.1.0/viprs/model/vi/e_step_cpp.pxd` & `viprs-0.1.1/viprs/model/vi/e_step_cpp.pxd`

 * *Files identical despite different names*

### Comparing `viprs-0.1.0/viprs/model/vi/e_step_cpp.pyx` & `viprs-0.1.1/viprs/model/vi/e_step_cpp.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
                            T* var_mu,
                            T* eta,
                            T* q,
                            T* eta_diff,
                            T* u_logs,
                            T* half_var_tau,
                            T* mu_mult,
-                              T dq_scale,
+                           T dq_scale,
                            int threads,
                            bint use_blas,
                            bint low_memory) noexcept nogil
 
 
 cpdef check_blas_support():
     return blas_supported()
```

### Comparing `viprs-0.1.0/viprs/plot/diagnostics.py` & `viprs-0.1.1/viprs/plot/diagnostics.py`

 * *Files identical despite different names*

### Comparing `viprs-0.1.0/viprs/utils/OptimizeResult.py` & `viprs-0.1.1/viprs/utils/OptimizeResult.py`

 * *Files identical despite different names*

### Comparing `viprs-0.1.0/viprs/utils/compute_utils.py` & `viprs-0.1.1/viprs/utils/compute_utils.py`

 * *Files identical despite different names*

### Comparing `viprs-0.1.0/viprs/utils/data_utils.py` & `viprs-0.1.1/viprs/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `viprs-0.1.0/viprs/utils/math_utils.pxd` & `viprs-0.1.1/viprs/utils/math_utils.pxd`

 * *Files identical despite different names*

### Comparing `viprs-0.1.0/viprs/utils/math_utils.pyx` & `viprs-0.1.1/viprs/utils/math_utils.pyx`

 * *Files identical despite different names*

### Comparing `viprs-0.1.0/viprs.egg-info/PKG-INFO` & `viprs-0.1.1/viprs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viprs
-Version: 0.1.0
+Version: 0.1.1
 Summary: Variational Inference of Polygenic Risk Scores (VIPRS)
 Home-page: https://github.com/shz9/viprs
 Author: Shadi Zabad
 Author-email: shadi.zabad@mail.mcgill.ca
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `viprs-0.1.0/viprs.egg-info/SOURCES.txt` & `viprs-0.1.1/viprs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

