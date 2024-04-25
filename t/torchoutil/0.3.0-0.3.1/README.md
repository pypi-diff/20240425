# Comparing `tmp/torchoutil-0.3.0.tar.gz` & `tmp/torchoutil-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchoutil-0.3.0.tar", last modified: Wed Apr 17 14:13:33 2024, max compression
+gzip compressed data, was "torchoutil-0.3.1.tar", last modified: Thu Apr 25 15:01:15 2024, max compression
```

## Comparing `torchoutil-0.3.0.tar` & `torchoutil-0.3.1.tar`

### file list

```diff
@@ -1,89 +1,103 @@
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-17 14:13:33.942098 torchoutil-0.3.0/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1064 2024-03-01 09:46:35.000000 torchoutil-0.3.0/LICENSE
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6273 2024-04-17 14:13:33.942098 torchoutil-0.3.0/PKG-INFO
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3697 2024-04-17 14:04:29.000000 torchoutil-0.3.0/README.md
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1959 2024-03-07 15:01:16.000000 torchoutil-0.3.0/pyproject.toml
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      108 2024-03-07 15:01:16.000000 torchoutil-0.3.0/requirements-dev.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       53 2024-03-04 17:33:08.000000 torchoutil-0.3.0/requirements-extras.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       57 2024-03-04 17:33:08.000000 torchoutil-0.3.0/requirements.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       38 2024-04-17 14:13:33.942098 torchoutil-0.3.0/setup.cfg
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      117 2024-03-04 17:33:08.000000 torchoutil-0.3.0/setup.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-17 14:13:33.934098 torchoutil-0.3.0/src/
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-17 14:13:33.938099 torchoutil-0.3.0/src/torchoutil/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      376 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      137 2024-03-04 17:33:08.000000 torchoutil-0.3.0/src/torchoutil/__main__.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-17 14:13:33.938099 torchoutil-0.3.0/src/torchoutil/hub/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       96 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/hub/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      996 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/hub/download.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6856 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/hub/registry.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1032 2024-03-04 17:33:08.000000 torchoutil-0.3.0/src/torchoutil/info.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-17 14:13:33.938099 torchoutil-0.3.0/src/torchoutil/nn/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       70 2024-04-17 12:32:36.000000 torchoutil-0.3.0/src/torchoutil/nn/__init__.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-17 14:13:33.938099 torchoutil-0.3.0/src/torchoutil/nn/functional/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      292 2024-03-04 17:33:08.000000 torchoutil-0.3.0/src/torchoutil/nn/functional/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      404 2024-03-04 17:33:08.000000 torchoutil-0.3.0/src/torchoutil/nn/functional/activation.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2566 2024-03-04 17:33:08.000000 torchoutil-0.3.0/src/torchoutil/nn/functional/crop.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      460 2024-03-04 17:33:08.000000 torchoutil-0.3.0/src/torchoutil/nn/functional/get.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4475 2024-03-08 10:17:47.000000 torchoutil-0.3.0/src/torchoutil/nn/functional/indices.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    12723 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/nn/functional/mask.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4311 2024-03-08 10:17:47.000000 torchoutil-0.3.0/src/torchoutil/nn/functional/multiclass.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6945 2024-03-08 10:17:47.000000 torchoutil-0.3.0/src/torchoutil/nn/functional/multilabel.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      992 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/nn/functional/numpy.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4196 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/nn/functional/others.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     8421 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/nn/functional/pad.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1108 2024-03-04 17:33:08.000000 torchoutil-0.3.0/src/torchoutil/nn/functional/repeat.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-17 14:13:33.938099 torchoutil-0.3.0/src/torchoutil/nn/modules/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      270 2024-03-04 17:33:08.000000 torchoutil-0.3.0/src/torchoutil/nn/modules/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      700 2024-03-04 17:33:08.000000 torchoutil-0.3.0/src/torchoutil/nn/modules/activation.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1871 2024-03-04 17:33:08.000000 torchoutil-0.3.0/src/torchoutil/nn/modules/crop.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1643 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/nn/modules/layer.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1184 2024-03-08 10:17:47.000000 torchoutil-0.3.0/src/torchoutil/nn/modules/mask.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4703 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/nn/modules/multiclass.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5188 2024-03-08 10:17:47.000000 torchoutil-0.3.0/src/torchoutil/nn/modules/multilabel.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1005 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/nn/modules/numpy.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3311 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/nn/modules/pad.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1259 2024-03-01 09:46:35.000000 torchoutil-0.3.0/src/torchoutil/nn/modules/repeat.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9618 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/nn/modules/tensor.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5825 2024-03-08 10:17:47.000000 torchoutil-0.3.0/src/torchoutil/nn/modules/typed.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-17 14:13:33.938099 torchoutil-0.3.0/src/torchoutil/optim/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       46 2024-03-04 17:33:08.000000 torchoutil-0.3.0/src/torchoutil/optim/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1761 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/optim/utils.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-17 14:13:33.938099 torchoutil-0.3.0/src/torchoutil/utils/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       46 2024-03-01 09:46:35.000000 torchoutil-0.3.0/src/torchoutil/utils/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6934 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/utils/collections.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-17 14:13:33.942098 torchoutil-0.3.0/src/torchoutil/utils/data/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      141 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/utils/data/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2370 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/utils/data/collate.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      523 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/utils/data/dataloader.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1497 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/utils/data/dataset.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4099 2024-03-04 17:33:08.000000 torchoutil-0.3.0/src/torchoutil/utils/data/split.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-17 14:13:33.942098 torchoutil-0.3.0/src/torchoutil/utils/hdf/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      394 2024-03-04 17:33:08.000000 torchoutil-0.3.0/src/torchoutil/utils/hdf/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      593 2024-03-07 14:09:27.000000 torchoutil-0.3.0/src/torchoutil/utils/hdf/common.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    16579 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/utils/hdf/dataset.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    16689 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/utils/hdf/pack.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      624 2024-03-04 17:33:08.000000 torchoutil-0.3.0/src/torchoutil/utils/packaging.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      528 2024-03-04 17:33:08.000000 torchoutil-0.3.0/src/torchoutil/utils/return_types.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5299 2024-03-04 17:33:08.000000 torchoutil-0.3.0/src/torchoutil/utils/tensorboard.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1157 2024-03-07 15:01:16.000000 torchoutil-0.3.0/src/torchoutil/utils/type_checks.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-17 14:13:33.938099 torchoutil-0.3.0/src/torchoutil.egg-info/
--rw-r--r--   0 labbeti   (1000) labbeti   (1000)     6273 2024-04-17 14:13:33.000000 torchoutil-0.3.0/src/torchoutil.egg-info/PKG-INFO
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2443 2024-04-17 14:13:33.000000 torchoutil-0.3.0/src/torchoutil.egg-info/SOURCES.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        1 2024-04-17 14:13:33.000000 torchoutil-0.3.0/src/torchoutil.egg-info/dependency_links.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       71 2024-04-17 14:13:33.000000 torchoutil-0.3.0/src/torchoutil.egg-info/entry_points.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      160 2024-04-17 14:13:33.000000 torchoutil-0.3.0/src/torchoutil.egg-info/requires.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       11 2024-04-17 14:13:33.000000 torchoutil-0.3.0/src/torchoutil.egg-info/top_level.txt
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-17 14:13:33.942098 torchoutil-0.3.0/tests/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1172 2024-04-17 14:04:29.000000 torchoutil-0.3.0/tests/test_hub.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      472 2024-03-04 17:33:08.000000 torchoutil-0.3.0/tests/test_nn_functional_crop.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      620 2024-03-07 15:01:16.000000 torchoutil-0.3.0/tests/test_nn_functional_indices.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    10920 2024-03-07 12:43:25.000000 torchoutil-0.3.0/tests/test_nn_functional_mask.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3836 2024-03-07 15:01:16.000000 torchoutil-0.3.0/tests/test_nn_functional_multilabel.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1463 2024-04-17 14:04:29.000000 torchoutil-0.3.0/tests/test_nn_functional_others.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7010 2024-03-07 12:42:21.000000 torchoutil-0.3.0/tests/test_nn_functional_pad.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      577 2024-03-01 09:46:35.000000 torchoutil-0.3.0/tests/test_nn_functional_repeat.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1238 2024-03-01 09:46:35.000000 torchoutil-0.3.0/tests/test_nn_modules_multilabel.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2239 2024-03-01 09:46:35.000000 torchoutil-0.3.0/tests/test_readme.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1131 2024-04-17 14:04:20.000000 torchoutil-0.3.0/tests/test_utils_ckpt.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2335 2024-04-17 14:04:29.000000 torchoutil-0.3.0/tests/test_utils_collections.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1967 2024-03-07 15:01:16.000000 torchoutil-0.3.0/tests/test_utils_hdf.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-25 15:01:15.452894 torchoutil-0.3.1/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1064 2024-03-01 09:46:35.000000 torchoutil-0.3.1/LICENSE
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7441 2024-04-25 15:01:15.448894 torchoutil-0.3.1/PKG-INFO
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4865 2024-04-25 14:46:40.000000 torchoutil-0.3.1/README.md
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1959 2024-03-07 15:01:16.000000 torchoutil-0.3.1/pyproject.toml
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      137 2024-04-25 14:46:40.000000 torchoutil-0.3.1/requirements-dev.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       71 2024-04-25 14:46:40.000000 torchoutil-0.3.1/requirements-extras.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       57 2024-03-04 17:33:08.000000 torchoutil-0.3.1/requirements.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       38 2024-04-25 15:01:15.452894 torchoutil-0.3.1/setup.cfg
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      117 2024-03-04 17:33:08.000000 torchoutil-0.3.1/setup.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-25 15:01:15.440894 torchoutil-0.3.1/src/
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-25 15:01:15.440894 torchoutil-0.3.1/src/torchoutil/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      376 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      137 2024-03-04 17:33:08.000000 torchoutil-0.3.1/src/torchoutil/__main__.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-25 15:01:15.440894 torchoutil-0.3.1/src/torchoutil/hub/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       96 2024-04-17 14:04:29.000000 torchoutil-0.3.1/src/torchoutil/hub/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      996 2024-04-17 14:04:29.000000 torchoutil-0.3.1/src/torchoutil/hub/download.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6856 2024-04-17 14:04:29.000000 torchoutil-0.3.1/src/torchoutil/hub/registry.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1032 2024-03-04 17:33:08.000000 torchoutil-0.3.1/src/torchoutil/info.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-25 15:01:15.440894 torchoutil-0.3.1/src/torchoutil/nn/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       70 2024-04-17 12:32:36.000000 torchoutil-0.3.1/src/torchoutil/nn/__init__.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-25 15:01:15.444894 torchoutil-0.3.1/src/torchoutil/nn/functional/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      329 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/nn/functional/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      404 2024-03-04 17:33:08.000000 torchoutil-0.3.1/src/torchoutil/nn/functional/activation.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2566 2024-03-04 17:33:08.000000 torchoutil-0.3.1/src/torchoutil/nn/functional/crop.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      460 2024-03-04 17:33:08.000000 torchoutil-0.3.1/src/torchoutil/nn/functional/get.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4475 2024-03-08 10:17:47.000000 torchoutil-0.3.1/src/torchoutil/nn/functional/indices.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    12723 2024-04-17 14:04:29.000000 torchoutil-0.3.1/src/torchoutil/nn/functional/mask.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4805 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/nn/functional/multiclass.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6945 2024-03-08 10:17:47.000000 torchoutil-0.3.1/src/torchoutil/nn/functional/multilabel.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1231 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/nn/functional/numpy.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4534 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/nn/functional/others.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     8564 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/nn/functional/pad.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2877 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/nn/functional/transform.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-25 15:01:15.444894 torchoutil-0.3.1/src/torchoutil/nn/modules/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      297 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/nn/modules/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      810 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/nn/modules/activation.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2064 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/nn/modules/crop.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1643 2024-04-17 14:04:29.000000 torchoutil-0.3.1/src/torchoutil/nn/modules/layer.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1381 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/nn/modules/mask.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5870 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/nn/modules/multiclass.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6125 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/nn/modules/multilabel.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1244 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/nn/modules/numpy.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3740 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/nn/modules/pad.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9618 2024-04-25 12:28:31.000000 torchoutil-0.3.1/src/torchoutil/nn/modules/tensor.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2833 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/nn/modules/transform.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6170 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/nn/modules/typed.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-25 15:01:15.444894 torchoutil-0.3.1/src/torchoutil/optim/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       68 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/optim/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1805 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/optim/utils.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-25 15:01:15.444894 torchoutil-0.3.1/src/torchoutil/utils/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       46 2024-04-25 13:24:09.000000 torchoutil-0.3.1/src/torchoutil/utils/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    10196 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/utils/collections.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-25 15:01:15.444894 torchoutil-0.3.1/src/torchoutil/utils/data/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      141 2024-04-17 14:04:29.000000 torchoutil-0.3.1/src/torchoutil/utils/data/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2370 2024-04-17 14:04:29.000000 torchoutil-0.3.1/src/torchoutil/utils/data/collate.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      523 2024-04-17 14:04:29.000000 torchoutil-0.3.1/src/torchoutil/utils/data/dataloader.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1508 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/utils/data/dataset.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4099 2024-03-04 17:33:08.000000 torchoutil-0.3.1/src/torchoutil/utils/data/split.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-25 15:01:15.448894 torchoutil-0.3.1/src/torchoutil/utils/hdf/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      394 2024-03-04 17:33:08.000000 torchoutil-0.3.1/src/torchoutil/utils/hdf/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      875 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/utils/hdf/common.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    16619 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/utils/hdf/dataset.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    16706 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/utils/hdf/pack.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2797 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/utils/log_utils.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      730 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/utils/packaging.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-25 15:01:15.448894 torchoutil-0.3.1/src/torchoutil/utils/pickle_dataset/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      177 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/utils/pickle_dataset/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      473 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/utils/pickle_dataset/common.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3842 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/utils/pickle_dataset/dataset.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6055 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/utils/pickle_dataset/pack.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      528 2024-03-04 17:33:08.000000 torchoutil-0.3.1/src/torchoutil/utils/return_types.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-25 15:01:15.448894 torchoutil-0.3.1/src/torchoutil/utils/saving/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      195 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/utils/saving/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      945 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/utils/saving/common.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1598 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/utils/saving/csv_io.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2389 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/utils/saving/yaml_io.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5297 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/utils/tensorboard.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2658 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/utils/type_checks.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-25 15:01:15.440894 torchoutil-0.3.1/src/torchoutil.egg-info/
+-rw-r--r--   0 labbeti   (1000) labbeti   (1000)     7441 2024-04-25 15:01:15.000000 torchoutil-0.3.1/src/torchoutil.egg-info/PKG-INFO
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2924 2024-04-25 15:01:15.000000 torchoutil-0.3.1/src/torchoutil.egg-info/SOURCES.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        1 2024-04-25 15:01:15.000000 torchoutil-0.3.1/src/torchoutil.egg-info/dependency_links.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       71 2024-04-25 15:01:15.000000 torchoutil-0.3.1/src/torchoutil.egg-info/entry_points.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      206 2024-04-25 15:01:15.000000 torchoutil-0.3.1/src/torchoutil.egg-info/requires.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       11 2024-04-25 15:01:15.000000 torchoutil-0.3.1/src/torchoutil.egg-info/top_level.txt
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-25 15:01:15.448894 torchoutil-0.3.1/tests/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1176 2024-04-25 14:46:40.000000 torchoutil-0.3.1/tests/test_hub.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      472 2024-03-04 17:33:08.000000 torchoutil-0.3.1/tests/test_nn_functional_crop.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      620 2024-03-07 15:01:16.000000 torchoutil-0.3.1/tests/test_nn_functional_indices.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    10920 2024-03-07 12:43:25.000000 torchoutil-0.3.1/tests/test_nn_functional_mask.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1659 2024-04-25 14:46:40.000000 torchoutil-0.3.1/tests/test_nn_functional_multiclass.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3836 2024-03-07 15:01:16.000000 torchoutil-0.3.1/tests/test_nn_functional_multilabel.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2478 2024-04-25 14:46:40.000000 torchoutil-0.3.1/tests/test_nn_functional_others.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7010 2024-03-07 12:42:21.000000 torchoutil-0.3.1/tests/test_nn_functional_pad.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1750 2024-04-25 14:46:40.000000 torchoutil-0.3.1/tests/test_nn_functional_transform.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      674 2024-04-25 14:46:40.000000 torchoutil-0.3.1/tests/test_nn_modules.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1240 2024-04-25 14:46:40.000000 torchoutil-0.3.1/tests/test_nn_modules_multilabel.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2239 2024-03-01 09:46:35.000000 torchoutil-0.3.1/tests/test_readme.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3484 2024-04-25 14:46:40.000000 torchoutil-0.3.1/tests/test_utils_collections.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1967 2024-03-07 15:01:16.000000 torchoutil-0.3.1/tests/test_utils_hdf.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5279 2024-04-25 14:46:40.000000 torchoutil-0.3.1/tests/test_utils_pickle.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      755 2024-04-25 14:46:40.000000 torchoutil-0.3.1/tests/test_utils_type_checks.py
```

### Comparing `torchoutil-0.3.0/LICENSE` & `torchoutil-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `torchoutil-0.3.0/PKG-INFO` & `torchoutil-0.3.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 746f 7263  : 2.1.Name: torc
 00000020: 686f 7574 696c 0a56 6572 7369 6f6e 3a20  houtil.Version: 
-00000030: 302e 332e 300a 5375 6d6d 6172 793a 2043  0.3.0.Summary: C
+00000030: 302e 332e 310a 5375 6d6d 6172 793a 2043  0.3.1.Summary: C
 00000040: 6f6c 6c65 6374 696f 6e20 6f66 2066 756e  ollection of fun
 00000050: 6374 696f 6e73 2061 6e64 206d 6f64 756c  ctions and modul
 00000060: 6573 2074 6f20 6865 6c70 2064 6576 656c  es to help devel
 00000070: 6f70 6d65 6e74 2069 6e20 5079 546f 7263  opment in PyTorc
 00000080: 682e 0a41 7574 686f 722d 656d 6169 6c3a  h..Author-email:
 00000090: 2022 c389 7469 656e 6e65 204c 6162 62c3   "..tienne Labb.
 000000a0: a920 284c 6162 6265 7469 2922 203c 6c61  . (Labbeti)" <la
@@ -301,93 +301,166 @@
 000012c0: 203d 2074 6f72 6368 2e61 735f 7465 6e73   = torch.as_tens
 000012d0: 6f72 285b 5b31 2c20 302c 2030 5d2c 205b  or([[1, 0, 0], [
 000012e0: 302c 2031 2c20 315d 2c20 5b30 2c20 302c  0, 1, 1], [0, 0,
 000012f0: 2030 5d5d 290a 696e 6469 6365 7320 3d20   0]]).indices = 
 00001300: 6d75 6c74 6968 6f74 5f74 6f5f 696e 6469  multihot_to_indi
 00001310: 6365 7328 6d75 6c74 6968 6f74 290a 2320  ces(multihot).# 
 00001320: 5b5b 305d 2c20 5b31 2c20 325d 2c20 5b5d  [[0], [1, 2], []
-00001330: 5d0a 6060 600a 0a23 2323 202e 2e2e 616e  ].```..### ...an
-00001340: 6420 6d6f 7265 2074 656e 736f 7220 6d61  d more tensor ma
-00001350: 6e69 7075 6c61 7469 6f6e 7321 0a0a 6060  nipulations!..``
-00001360: 6070 7974 686f 6e0a 696d 706f 7274 2074  `python.import t
-00001370: 6f72 6368 0a66 726f 6d20 746f 7263 686f  orch.from torcho
-00001380: 7574 696c 2069 6d70 6f72 7420 696e 7365  util import inse
-00001390: 7274 5f61 745f 696e 6469 6365 730a 0a78  rt_at_indices..x
-000013a0: 203d 2074 6f72 6368 2e61 735f 7465 6e73   = torch.as_tens
-000013b0: 6f72 285b 312c 2032 2c20 332c 2034 5d29  or([1, 2, 3, 4])
-000013c0: 0a72 6573 756c 7420 3d20 696e 7365 7274  .result = insert
-000013d0: 5f61 745f 696e 6469 6365 7328 782c 2069  _at_indices(x, i
-000013e0: 6e64 6963 6573 3d5b 302c 2032 5d2c 2076  ndices=[0, 2], v
-000013f0: 616c 7565 733d 3529 0a23 2072 6573 756c  alues=5).# resul
-00001400: 7420 636f 6e74 6169 6e73 2074 656e 736f  t contains tenso
-00001410: 7220 7769 7468 2069 6e73 6572 7465 6420  r with inserted 
-00001420: 7661 6c75 6573 3a20 7465 6e73 6f72 285b  values: tensor([
-00001430: 352c 2031 2c20 322c 2035 2c20 332c 2034  5, 1, 2, 5, 3, 4
-00001440: 5d29 0a60 6060 0a0a 6060 6070 7974 686f  ]).```..```pytho
-00001450: 6e0a 696d 706f 7274 2074 6f72 6368 0a66  n.import torch.f
-00001460: 726f 6d20 746f 7263 686f 7574 696c 2069  rom torchoutil i
-00001470: 6d70 6f72 7420 6765 745f 696e 7665 7273  mport get_invers
-00001480: 655f 7065 726d 0a0a 7065 726d 203d 2074  e_perm..perm = t
-00001490: 6f72 6368 2e72 616e 6470 6572 6d28 3130  orch.randperm(10
-000014a0: 290a 696e 765f 7065 726d 203d 2067 6574  ).inv_perm = get
-000014b0: 5f69 6e76 6572 7365 5f70 6572 6d28 7065  _inverse_perm(pe
-000014c0: 726d 290a 0a78 3120 3d20 746f 7263 682e  rm)..x1 = torch.
-000014d0: 7261 6e64 2831 3029 0a78 3220 3d20 7831  rand(10).x2 = x1
-000014e0: 5b70 6572 6d5d 0a78 3320 3d20 7832 5b69  [perm].x3 = x2[i
-000014f0: 6e76 5f70 6572 6d5d 0a23 2069 6e76 5f70  nv_perm].# inv_p
-00001500: 6572 6d20 6172 6520 696e 6469 6365 7320  erm are indices 
-00001510: 7468 6174 2061 6c6c 6f77 2075 7320 746f  that allow us to
-00001520: 2067 6574 2078 3320 6672 6f6d 2078 322c   get x3 from x2,
-00001530: 2069 2e65 2e20 7831 203d 3d20 7833 2068   i.e. x1 == x3 h
-00001540: 6572 650a 6060 600a 0a23 2320 4578 7472  ere.```..## Extr
-00001550: 6173 0a60 746f 7263 686f 7574 696c 6020  as.`torchoutil` 
-00001560: 616c 736f 2070 726f 7669 6465 7320 6164  also provides ad
-00001570: 6469 7469 6f6e 616c 206d 6f64 756c 6573  ditional modules
-00001580: 2077 6865 6e20 736f 6d65 2073 7065 6369   when some speci
-00001590: 6669 6320 7061 636b 6167 6520 6172 6520  fic package are 
-000015a0: 616c 7265 6164 7920 696e 7374 616c 6c65  already installe
-000015b0: 6420 696e 2079 6f75 7220 656e 7669 726f  d in your enviro
-000015c0: 6e6d 656e 742e 0a41 6c6c 2065 7874 7261  nment..All extra
-000015d0: 7320 6361 6e20 6265 2069 6e73 7461 6c6c  s can be install
-000015e0: 6564 2077 6974 6820 6070 6970 2069 6e73  ed with `pip ins
-000015f0: 7461 6c6c 2074 6f72 6368 6f75 7469 6c5b  tall torchoutil[
-00001600: 6578 7472 6173 5d60 0a0a 2d20 4966 2060  extras]`..- If `
-00001610: 7465 6e73 6f72 626f 6172 6460 2069 7320  tensorboard` is 
-00001620: 696e 7374 616c 6c65 642c 2074 6865 2066  installed, the f
-00001630: 756e 6374 696f 6e20 606c 6f61 645f 6576  unction `load_ev
-00001640: 656e 745f 6669 6c65 6020 6361 6e20 6265  ent_file` can be
-00001650: 2075 7365 642e 2049 7420 6973 2075 7365   used. It is use
-00001660: 6675 6c20 746f 206c 6f61 6420 6d61 6e75  ful to load manu
-00001670: 616c 6c79 2061 6c6c 2064 6174 6120 636f  ally all data co
-00001680: 6e74 6169 6e65 6420 696e 2061 6e20 7465  ntained in an te
-00001690: 6e73 6f72 626f 6172 6420 6576 656e 7420  nsorboard event 
-000016a0: 6669 6c65 2e0a 2d20 4966 2060 6e75 6d70  file..- If `nump
-000016b0: 7960 2069 7320 696e 7374 616c 6c65 642c  y` is installed,
-000016c0: 2074 6865 2063 6c61 7373 6573 2060 4672   the classes `Fr
-000016d0: 6f6d 4e75 6d70 7960 2061 6e64 2020 6054  omNumpy` and  `T
-000016e0: 6f4e 756d 7079 6020 6361 6e20 6265 2075  oNumpy` can be u
-000016f0: 7365 6420 616e 6420 7468 6569 7220 7265  sed and their re
-00001700: 6c61 7465 6420 6675 6e63 7469 6f6e 2e20  lated function. 
-00001710: 4974 2069 7320 6d65 616e 7420 746f 2062  It is meant to b
-00001720: 6520 7573 6564 2074 6f20 636f 6d70 6f73  e used to compos
-00001730: 6520 6479 6e61 6d69 6320 7472 616e 7366  e dynamic transf
-00001740: 6f72 6d73 2069 6e74 6f20 6053 6571 7565  orms into `Seque
-00001750: 6e74 6961 6c60 206d 6f64 756c 652e 0a2d  ntial` module..-
-00001760: 2049 6620 6068 3570 7960 2069 7320 696e   If `h5py` is in
-00001770: 7374 616c 6c65 642c 2074 6865 2066 756e  stalled, the fun
-00001780: 6374 696f 6e20 6070 6163 6b5f 746f 5f68  ction `pack_to_h
-00001790: 6466 6020 616e 6420 636c 6173 7320 6048  df` and class `H
-000017a0: 4446 4461 7461 7365 7460 2063 616e 2062  DFDataset` can b
-000017b0: 6520 7573 6564 2e20 4361 6e20 6265 2075  e used. Can be u
-000017c0: 7365 6420 746f 2070 6163 6b2f 7265 6164  sed to pack/read
-000017d0: 2064 6174 6173 6574 2074 6f20 4844 4620   dataset to HDF 
-000017e0: 6669 6c65 732c 2061 6e64 2073 7570 706f  files, and suppo
-000017f0: 7274 7320 7661 7269 6162 6c65 2d6c 656e  rts variable-len
-00001800: 6774 6820 7365 7175 656e 6365 7320 6f66  gth sequences of
-00001810: 2064 6174 612e 0a0a 0a23 2320 436f 6e74   data....## Cont
-00001820: 6163 740a 4d61 696e 7461 696e 6572 3a0a  act.Maintainer:.
-00001830: 2d20 5bc3 8974 6965 6e6e 6520 4c61 6262  - [..tienne Labb
-00001840: c3a9 5d28 6874 7470 733a 2f2f 6c61 6262  ..](https://labb
-00001850: 6574 692e 6769 7468 7562 2e69 6f2f 2920  eti.github.io/) 
-00001860: 224c 6162 6265 7469 223a 206c 6162 6265  "Labbeti": labbe
-00001870: 7469 2e70 7562 4067 6d61 696c 2e63 6f6d  ti.pub@gmail.com
-00001880: 0a                                       .
+00001330: 5d0a 6060 600a 0a23 2323 2045 6173 656c  ].```..### Easel
+00001340: 7920 7072 652d 636f 6d70 7574 6520 7472  y pre-compute tr
+00001350: 616e 7366 6f72 6d73 0a0a 4865 7265 2069  ansforms..Here i
+00001360: 7320 616e 2065 7861 6d70 6c65 206f 6620  s an example of 
+00001370: 7072 652d 636f 6d70 7574 696e 6720 7370  pre-computing sp
+00001380: 6563 7472 6f67 7261 6d73 206f 6620 746f  ectrograms of to
+00001390: 7263 6861 7564 696f 2060 5350 4545 4348  rchaudio `SPEECH
+000013a0: 434f 4d4d 414e 4453 6020 6461 7461 7365  COMMANDS` datase
+000013b0: 742c 2075 7369 6e67 2060 7061 636b 5f74  t, using `pack_t
+000013c0: 6f5f 7069 636b 6c65 6020 6675 6e63 7469  o_pickle` functi
+000013d0: 6f6e 3a0a 0a60 6060 7079 7468 6f6e 0a66  on:..```python.f
+000013e0: 726f 6d20 746f 7263 6820 696d 706f 7274  rom torch import
+000013f0: 206e 6e0a 6672 6f6d 2074 6f72 6368 6175   nn.from torchau
+00001400: 6469 6f2e 6461 7461 7365 7473 2069 6d70  dio.datasets imp
+00001410: 6f72 7420 5350 4545 4348 434f 4d4d 414e  ort SPEECHCOMMAN
+00001420: 4453 0a66 726f 6d20 746f 7263 6861 7564  DS.from torchaud
+00001430: 696f 2e74 7261 6e73 666f 726d 7320 696d  io.transforms im
+00001440: 706f 7274 2053 7065 6374 726f 6772 616d  port Spectrogram
+00001450: 0a66 726f 6d20 746f 7263 686f 7574 696c  .from torchoutil
+00001460: 2e75 7469 6c73 2e70 6963 6b6c 655f 6461  .utils.pickle_da
+00001470: 7461 7365 7420 696d 706f 7274 2070 6163  taset import pac
+00001480: 6b5f 746f 5f70 6963 6b6c 650a 0a73 7065  k_to_pickle..spe
+00001490: 6563 685f 636f 6d6d 616e 6473 5f72 6f6f  ech_commands_roo
+000014a0: 7420 3d20 2270 6174 682f 746f 2f73 7065  t = "path/to/spe
+000014b0: 6563 685f 636f 6d6d 616e 6473 220a 7069  ech_commands".pi
+000014c0: 636b 6c65 5f72 6f6f 7420 3d20 2270 6174  ckle_root = "pat
+000014d0: 682f 746f 2f70 6963 6b6c 655f 6461 7461  h/to/pickle_data
+000014e0: 7365 7422 0a0a 6461 7461 7365 7420 3d20  set"..dataset = 
+000014f0: 5350 4545 4348 434f 4d4d 414e 4453 2873  SPEECHCOMMANDS(s
+00001500: 7065 6563 685f 636f 6d6d 616e 6473 5f72  peech_commands_r
+00001510: 6f6f 742c 2064 6f77 6e6c 6f61 643d 5472  oot, download=Tr
+00001520: 7565 2c20 7375 6273 6574 3d22 7661 6c69  ue, subset="vali
+00001530: 6461 7469 6f6e 2229 0a0a 636c 6173 7320  dation")..class 
+00001540: 4d79 5472 616e 7366 6f72 6d28 6e6e 2e4d  MyTransform(nn.M
+00001550: 6f64 756c 6529 3a0a 2020 2020 6465 6620  odule):.    def 
+00001560: 5f5f 696e 6974 5f5f 2873 656c 6629 202d  __init__(self) -
+00001570: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00001580: 7375 7065 7228 292e 5f5f 696e 6974 5f5f  super().__init__
+00001590: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+000015a0: 7370 6563 7472 6f67 7261 6d5f 6578 7472  spectrogram_extr
+000015b0: 6163 746f 7220 3d20 5370 6563 7472 6f67  actor = Spectrog
+000015c0: 7261 6d28 290a 0a20 2020 2064 6566 2066  ram()..    def f
+000015d0: 6f72 7761 7264 2873 656c 662c 2069 7465  orward(self, ite
+000015e0: 6d29 3a0a 2020 2020 2020 2020 7761 7665  m):.        wave
+000015f0: 666f 726d 203d 2069 7465 6d5b 305d 0a20  form = item[0]. 
+00001600: 2020 2020 2020 2073 7065 6374 726f 6772         spectrogr
+00001610: 616d 203d 2073 656c 662e 7370 6563 7472  am = self.spectr
+00001620: 6f67 7261 6d5f 6578 7472 6163 746f 7228  ogram_extractor(
+00001630: 7761 7665 666f 726d 290a 2020 2020 2020  waveform).      
+00001640: 2020 7265 7475 726e 2028 7370 6563 7472    return (spectr
+00001650: 6f67 7261 6d2c 2920 2b20 6974 656d 5b31  ogram,) + item[1
+00001660: 3a5d 0a0a 7061 636b 5f74 6f5f 7069 636b  :]..pack_to_pick
+00001670: 6c65 2864 6174 6173 6574 2c20 7069 636b  le(dataset, pick
+00001680: 6c65 5f72 6f6f 742c 204d 7954 7261 6e73  le_root, MyTrans
+00001690: 666f 726d 2829 290a 6060 600a 0a54 6865  form()).```..The
+000016a0: 6e20 796f 7520 6361 6e20 6c6f 6164 2074  n you can load t
+000016b0: 6865 2070 7265 2d63 6f6d 7075 7465 6420  he pre-computed 
+000016c0: 6461 7461 7365 7420 7573 696e 6720 6050  dataset using `P
+000016d0: 6963 6b6c 6544 6174 6173 6574 603a 0a60  ickleDataset`:.`
+000016e0: 6060 7079 7468 6f6e 0a66 726f 6d20 746f  ``python.from to
+000016f0: 7263 686f 7574 696c 2e75 7469 6c73 2e70  rchoutil.utils.p
+00001700: 6963 6b6c 655f 6461 7461 7365 7420 696d  ickle_dataset im
+00001710: 706f 7274 2050 6963 6b6c 6544 6174 6173  port PickleDatas
+00001720: 6574 0a0a 7069 636b 6c65 5f72 6f6f 7420  et..pickle_root 
+00001730: 3d20 2270 6174 682f 746f 2f70 6963 6b6c  = "path/to/pickl
+00001740: 655f 6461 7461 7365 7422 0a70 6963 6b6c  e_dataset".pickl
+00001750: 655f 6461 7461 7365 7420 3d20 5069 636b  e_dataset = Pick
+00001760: 6c65 4461 7461 7365 7428 7069 636b 6c65  leDataset(pickle
+00001770: 5f72 6f6f 7429 0a70 6963 6b6c 655f 6461  _root).pickle_da
+00001780: 7461 7365 745b 305d 2020 2320 3d3d 2066  taset[0]  # == f
+00001790: 6972 7374 2074 7261 6e73 666f 726d 6564  irst transformed
+000017a0: 2069 7465 6d2c 2069 2e65 2e20 7472 616e   item, i.e. tran
+000017b0: 7366 6f72 6d28 6461 7461 7365 745b 305d  sform(dataset[0]
+000017c0: 290a 6060 600a 0a23 2323 202e 2e2e 616e  ).```..### ...an
+000017d0: 6420 6d6f 7265 2074 656e 736f 7220 6d61  d more tensor ma
+000017e0: 6e69 7075 6c61 7469 6f6e 7321 0a0a 6060  nipulations!..``
+000017f0: 6070 7974 686f 6e0a 696d 706f 7274 2074  `python.import t
+00001800: 6f72 6368 0a66 726f 6d20 746f 7263 686f  orch.from torcho
+00001810: 7574 696c 2069 6d70 6f72 7420 696e 7365  util import inse
+00001820: 7274 5f61 745f 696e 6469 6365 730a 0a78  rt_at_indices..x
+00001830: 203d 2074 6f72 6368 2e61 735f 7465 6e73   = torch.as_tens
+00001840: 6f72 285b 312c 2032 2c20 332c 2034 5d29  or([1, 2, 3, 4])
+00001850: 0a72 6573 756c 7420 3d20 696e 7365 7274  .result = insert
+00001860: 5f61 745f 696e 6469 6365 7328 782c 2069  _at_indices(x, i
+00001870: 6e64 6963 6573 3d5b 302c 2032 5d2c 2076  ndices=[0, 2], v
+00001880: 616c 7565 733d 3529 0a23 2072 6573 756c  alues=5).# resul
+00001890: 7420 636f 6e74 6169 6e73 2074 656e 736f  t contains tenso
+000018a0: 7220 7769 7468 2069 6e73 6572 7465 6420  r with inserted 
+000018b0: 7661 6c75 6573 3a20 7465 6e73 6f72 285b  values: tensor([
+000018c0: 352c 2031 2c20 322c 2035 2c20 332c 2034  5, 1, 2, 5, 3, 4
+000018d0: 5d29 0a60 6060 0a0a 6060 6070 7974 686f  ]).```..```pytho
+000018e0: 6e0a 696d 706f 7274 2074 6f72 6368 0a66  n.import torch.f
+000018f0: 726f 6d20 746f 7263 686f 7574 696c 2069  rom torchoutil i
+00001900: 6d70 6f72 7420 6765 745f 696e 7665 7273  mport get_invers
+00001910: 655f 7065 726d 0a0a 7065 726d 203d 2074  e_perm..perm = t
+00001920: 6f72 6368 2e72 616e 6470 6572 6d28 3130  orch.randperm(10
+00001930: 290a 696e 765f 7065 726d 203d 2067 6574  ).inv_perm = get
+00001940: 5f69 6e76 6572 7365 5f70 6572 6d28 7065  _inverse_perm(pe
+00001950: 726d 290a 0a78 3120 3d20 746f 7263 682e  rm)..x1 = torch.
+00001960: 7261 6e64 2831 3029 0a78 3220 3d20 7831  rand(10).x2 = x1
+00001970: 5b70 6572 6d5d 0a78 3320 3d20 7832 5b69  [perm].x3 = x2[i
+00001980: 6e76 5f70 6572 6d5d 0a23 2069 6e76 5f70  nv_perm].# inv_p
+00001990: 6572 6d20 6172 6520 696e 6469 6365 7320  erm are indices 
+000019a0: 7468 6174 2061 6c6c 6f77 2075 7320 746f  that allow us to
+000019b0: 2067 6574 2078 3320 6672 6f6d 2078 322c   get x3 from x2,
+000019c0: 2069 2e65 2e20 7831 203d 3d20 7833 2068   i.e. x1 == x3 h
+000019d0: 6572 650a 6060 600a 0a23 2320 4578 7472  ere.```..## Extr
+000019e0: 6173 0a60 746f 7263 686f 7574 696c 6020  as.`torchoutil` 
+000019f0: 616c 736f 2070 726f 7669 6465 7320 6164  also provides ad
+00001a00: 6469 7469 6f6e 616c 206d 6f64 756c 6573  ditional modules
+00001a10: 2077 6865 6e20 736f 6d65 2073 7065 6369   when some speci
+00001a20: 6669 6320 7061 636b 6167 6520 6172 6520  fic package are 
+00001a30: 616c 7265 6164 7920 696e 7374 616c 6c65  already installe
+00001a40: 6420 696e 2079 6f75 7220 656e 7669 726f  d in your enviro
+00001a50: 6e6d 656e 742e 0a41 6c6c 2065 7874 7261  nment..All extra
+00001a60: 7320 6361 6e20 6265 2069 6e73 7461 6c6c  s can be install
+00001a70: 6564 2077 6974 6820 6070 6970 2069 6e73  ed with `pip ins
+00001a80: 7461 6c6c 2074 6f72 6368 6f75 7469 6c5b  tall torchoutil[
+00001a90: 6578 7472 6173 5d60 0a0a 2d20 4966 2060  extras]`..- If `
+00001aa0: 7465 6e73 6f72 626f 6172 6460 2069 7320  tensorboard` is 
+00001ab0: 696e 7374 616c 6c65 642c 2074 6865 2066  installed, the f
+00001ac0: 756e 6374 696f 6e20 606c 6f61 645f 6576  unction `load_ev
+00001ad0: 656e 745f 6669 6c65 6020 6361 6e20 6265  ent_file` can be
+00001ae0: 2075 7365 642e 2049 7420 6973 2075 7365   used. It is use
+00001af0: 6675 6c20 746f 206c 6f61 6420 6d61 6e75  ful to load manu
+00001b00: 616c 6c79 2061 6c6c 2064 6174 6120 636f  ally all data co
+00001b10: 6e74 6169 6e65 6420 696e 2061 6e20 7465  ntained in an te
+00001b20: 6e73 6f72 626f 6172 6420 6576 656e 7420  nsorboard event 
+00001b30: 6669 6c65 2e0a 2d20 4966 2060 6e75 6d70  file..- If `nump
+00001b40: 7960 2069 7320 696e 7374 616c 6c65 642c  y` is installed,
+00001b50: 2074 6865 2063 6c61 7373 6573 2060 4672   the classes `Fr
+00001b60: 6f6d 4e75 6d70 7960 2061 6e64 2020 6054  omNumpy` and  `T
+00001b70: 6f4e 756d 7079 6020 6361 6e20 6265 2075  oNumpy` can be u
+00001b80: 7365 6420 616e 6420 7468 6569 7220 7265  sed and their re
+00001b90: 6c61 7465 6420 6675 6e63 7469 6f6e 2e20  lated function. 
+00001ba0: 4974 2069 7320 6d65 616e 7420 746f 2062  It is meant to b
+00001bb0: 6520 7573 6564 2074 6f20 636f 6d70 6f73  e used to compos
+00001bc0: 6520 6479 6e61 6d69 6320 7472 616e 7366  e dynamic transf
+00001bd0: 6f72 6d73 2069 6e74 6f20 6053 6571 7565  orms into `Seque
+00001be0: 6e74 6961 6c60 206d 6f64 756c 652e 0a2d  ntial` module..-
+00001bf0: 2049 6620 6068 3570 7960 2069 7320 696e   If `h5py` is in
+00001c00: 7374 616c 6c65 642c 2074 6865 2066 756e  stalled, the fun
+00001c10: 6374 696f 6e20 6070 6163 6b5f 746f 5f68  ction `pack_to_h
+00001c20: 6466 6020 616e 6420 636c 6173 7320 6048  df` and class `H
+00001c30: 4446 4461 7461 7365 7460 2063 616e 2062  DFDataset` can b
+00001c40: 6520 7573 6564 2e20 4361 6e20 6265 2075  e used. Can be u
+00001c50: 7365 6420 746f 2070 6163 6b2f 7265 6164  sed to pack/read
+00001c60: 2064 6174 6173 6574 2074 6f20 4844 4620   dataset to HDF 
+00001c70: 6669 6c65 732c 2061 6e64 2073 7570 706f  files, and suppo
+00001c80: 7274 7320 7661 7269 6162 6c65 2d6c 656e  rts variable-len
+00001c90: 6774 6820 7365 7175 656e 6365 7320 6f66  gth sequences of
+00001ca0: 2064 6174 612e 0a0a 0a23 2320 436f 6e74   data....## Cont
+00001cb0: 6163 740a 4d61 696e 7461 696e 6572 3a0a  act.Maintainer:.
+00001cc0: 2d20 5bc3 8974 6965 6e6e 6520 4c61 6262  - [..tienne Labb
+00001cd0: c3a9 5d28 6874 7470 733a 2f2f 6c61 6262  ..](https://labb
+00001ce0: 6574 692e 6769 7468 7562 2e69 6f2f 2920  eti.github.io/) 
+00001cf0: 224c 6162 6265 7469 223a 206c 6162 6265  "Labbeti": labbe
+00001d00: 7469 2e70 7562 4067 6d61 696c 2e63 6f6d  ti.pub@gmail.com
+00001d10: 0a                                       .
```

### Comparing `torchoutil-0.3.0/README.md` & `torchoutil-0.3.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -140,93 +140,166 @@
 000008b0: 203d 2074 6f72 6368 2e61 735f 7465 6e73   = torch.as_tens
 000008c0: 6f72 285b 5b31 2c20 302c 2030 5d2c 205b  or([[1, 0, 0], [
 000008d0: 302c 2031 2c20 315d 2c20 5b30 2c20 302c  0, 1, 1], [0, 0,
 000008e0: 2030 5d5d 290a 696e 6469 6365 7320 3d20   0]]).indices = 
 000008f0: 6d75 6c74 6968 6f74 5f74 6f5f 696e 6469  multihot_to_indi
 00000900: 6365 7328 6d75 6c74 6968 6f74 290a 2320  ces(multihot).# 
 00000910: 5b5b 305d 2c20 5b31 2c20 325d 2c20 5b5d  [[0], [1, 2], []
-00000920: 5d0a 6060 600a 0a23 2323 202e 2e2e 616e  ].```..### ...an
-00000930: 6420 6d6f 7265 2074 656e 736f 7220 6d61  d more tensor ma
-00000940: 6e69 7075 6c61 7469 6f6e 7321 0a0a 6060  nipulations!..``
-00000950: 6070 7974 686f 6e0a 696d 706f 7274 2074  `python.import t
-00000960: 6f72 6368 0a66 726f 6d20 746f 7263 686f  orch.from torcho
-00000970: 7574 696c 2069 6d70 6f72 7420 696e 7365  util import inse
-00000980: 7274 5f61 745f 696e 6469 6365 730a 0a78  rt_at_indices..x
-00000990: 203d 2074 6f72 6368 2e61 735f 7465 6e73   = torch.as_tens
-000009a0: 6f72 285b 312c 2032 2c20 332c 2034 5d29  or([1, 2, 3, 4])
-000009b0: 0a72 6573 756c 7420 3d20 696e 7365 7274  .result = insert
-000009c0: 5f61 745f 696e 6469 6365 7328 782c 2069  _at_indices(x, i
-000009d0: 6e64 6963 6573 3d5b 302c 2032 5d2c 2076  ndices=[0, 2], v
-000009e0: 616c 7565 733d 3529 0a23 2072 6573 756c  alues=5).# resul
-000009f0: 7420 636f 6e74 6169 6e73 2074 656e 736f  t contains tenso
-00000a00: 7220 7769 7468 2069 6e73 6572 7465 6420  r with inserted 
-00000a10: 7661 6c75 6573 3a20 7465 6e73 6f72 285b  values: tensor([
-00000a20: 352c 2031 2c20 322c 2035 2c20 332c 2034  5, 1, 2, 5, 3, 4
-00000a30: 5d29 0a60 6060 0a0a 6060 6070 7974 686f  ]).```..```pytho
-00000a40: 6e0a 696d 706f 7274 2074 6f72 6368 0a66  n.import torch.f
-00000a50: 726f 6d20 746f 7263 686f 7574 696c 2069  rom torchoutil i
-00000a60: 6d70 6f72 7420 6765 745f 696e 7665 7273  mport get_invers
-00000a70: 655f 7065 726d 0a0a 7065 726d 203d 2074  e_perm..perm = t
-00000a80: 6f72 6368 2e72 616e 6470 6572 6d28 3130  orch.randperm(10
-00000a90: 290a 696e 765f 7065 726d 203d 2067 6574  ).inv_perm = get
-00000aa0: 5f69 6e76 6572 7365 5f70 6572 6d28 7065  _inverse_perm(pe
-00000ab0: 726d 290a 0a78 3120 3d20 746f 7263 682e  rm)..x1 = torch.
-00000ac0: 7261 6e64 2831 3029 0a78 3220 3d20 7831  rand(10).x2 = x1
-00000ad0: 5b70 6572 6d5d 0a78 3320 3d20 7832 5b69  [perm].x3 = x2[i
-00000ae0: 6e76 5f70 6572 6d5d 0a23 2069 6e76 5f70  nv_perm].# inv_p
-00000af0: 6572 6d20 6172 6520 696e 6469 6365 7320  erm are indices 
-00000b00: 7468 6174 2061 6c6c 6f77 2075 7320 746f  that allow us to
-00000b10: 2067 6574 2078 3320 6672 6f6d 2078 322c   get x3 from x2,
-00000b20: 2069 2e65 2e20 7831 203d 3d20 7833 2068   i.e. x1 == x3 h
-00000b30: 6572 650a 6060 600a 0a23 2320 4578 7472  ere.```..## Extr
-00000b40: 6173 0a60 746f 7263 686f 7574 696c 6020  as.`torchoutil` 
-00000b50: 616c 736f 2070 726f 7669 6465 7320 6164  also provides ad
-00000b60: 6469 7469 6f6e 616c 206d 6f64 756c 6573  ditional modules
-00000b70: 2077 6865 6e20 736f 6d65 2073 7065 6369   when some speci
-00000b80: 6669 6320 7061 636b 6167 6520 6172 6520  fic package are 
-00000b90: 616c 7265 6164 7920 696e 7374 616c 6c65  already installe
-00000ba0: 6420 696e 2079 6f75 7220 656e 7669 726f  d in your enviro
-00000bb0: 6e6d 656e 742e 0a41 6c6c 2065 7874 7261  nment..All extra
-00000bc0: 7320 6361 6e20 6265 2069 6e73 7461 6c6c  s can be install
-00000bd0: 6564 2077 6974 6820 6070 6970 2069 6e73  ed with `pip ins
-00000be0: 7461 6c6c 2074 6f72 6368 6f75 7469 6c5b  tall torchoutil[
-00000bf0: 6578 7472 6173 5d60 0a0a 2d20 4966 2060  extras]`..- If `
-00000c00: 7465 6e73 6f72 626f 6172 6460 2069 7320  tensorboard` is 
-00000c10: 696e 7374 616c 6c65 642c 2074 6865 2066  installed, the f
-00000c20: 756e 6374 696f 6e20 606c 6f61 645f 6576  unction `load_ev
-00000c30: 656e 745f 6669 6c65 6020 6361 6e20 6265  ent_file` can be
-00000c40: 2075 7365 642e 2049 7420 6973 2075 7365   used. It is use
-00000c50: 6675 6c20 746f 206c 6f61 6420 6d61 6e75  ful to load manu
-00000c60: 616c 6c79 2061 6c6c 2064 6174 6120 636f  ally all data co
-00000c70: 6e74 6169 6e65 6420 696e 2061 6e20 7465  ntained in an te
-00000c80: 6e73 6f72 626f 6172 6420 6576 656e 7420  nsorboard event 
-00000c90: 6669 6c65 2e0a 2d20 4966 2060 6e75 6d70  file..- If `nump
-00000ca0: 7960 2069 7320 696e 7374 616c 6c65 642c  y` is installed,
-00000cb0: 2074 6865 2063 6c61 7373 6573 2060 4672   the classes `Fr
-00000cc0: 6f6d 4e75 6d70 7960 2061 6e64 2020 6054  omNumpy` and  `T
-00000cd0: 6f4e 756d 7079 6020 6361 6e20 6265 2075  oNumpy` can be u
-00000ce0: 7365 6420 616e 6420 7468 6569 7220 7265  sed and their re
-00000cf0: 6c61 7465 6420 6675 6e63 7469 6f6e 2e20  lated function. 
-00000d00: 4974 2069 7320 6d65 616e 7420 746f 2062  It is meant to b
-00000d10: 6520 7573 6564 2074 6f20 636f 6d70 6f73  e used to compos
-00000d20: 6520 6479 6e61 6d69 6320 7472 616e 7366  e dynamic transf
-00000d30: 6f72 6d73 2069 6e74 6f20 6053 6571 7565  orms into `Seque
-00000d40: 6e74 6961 6c60 206d 6f64 756c 652e 0a2d  ntial` module..-
-00000d50: 2049 6620 6068 3570 7960 2069 7320 696e   If `h5py` is in
-00000d60: 7374 616c 6c65 642c 2074 6865 2066 756e  stalled, the fun
-00000d70: 6374 696f 6e20 6070 6163 6b5f 746f 5f68  ction `pack_to_h
-00000d80: 6466 6020 616e 6420 636c 6173 7320 6048  df` and class `H
-00000d90: 4446 4461 7461 7365 7460 2063 616e 2062  DFDataset` can b
-00000da0: 6520 7573 6564 2e20 4361 6e20 6265 2075  e used. Can be u
-00000db0: 7365 6420 746f 2070 6163 6b2f 7265 6164  sed to pack/read
-00000dc0: 2064 6174 6173 6574 2074 6f20 4844 4620   dataset to HDF 
-00000dd0: 6669 6c65 732c 2061 6e64 2073 7570 706f  files, and suppo
-00000de0: 7274 7320 7661 7269 6162 6c65 2d6c 656e  rts variable-len
-00000df0: 6774 6820 7365 7175 656e 6365 7320 6f66  gth sequences of
-00000e00: 2064 6174 612e 0a0a 0a23 2320 436f 6e74   data....## Cont
-00000e10: 6163 740a 4d61 696e 7461 696e 6572 3a0a  act.Maintainer:.
-00000e20: 2d20 5bc3 8974 6965 6e6e 6520 4c61 6262  - [..tienne Labb
-00000e30: c3a9 5d28 6874 7470 733a 2f2f 6c61 6262  ..](https://labb
-00000e40: 6574 692e 6769 7468 7562 2e69 6f2f 2920  eti.github.io/) 
-00000e50: 224c 6162 6265 7469 223a 206c 6162 6265  "Labbeti": labbe
-00000e60: 7469 2e70 7562 4067 6d61 696c 2e63 6f6d  ti.pub@gmail.com
-00000e70: 0a                                       .
+00000920: 5d0a 6060 600a 0a23 2323 2045 6173 656c  ].```..### Easel
+00000930: 7920 7072 652d 636f 6d70 7574 6520 7472  y pre-compute tr
+00000940: 616e 7366 6f72 6d73 0a0a 4865 7265 2069  ansforms..Here i
+00000950: 7320 616e 2065 7861 6d70 6c65 206f 6620  s an example of 
+00000960: 7072 652d 636f 6d70 7574 696e 6720 7370  pre-computing sp
+00000970: 6563 7472 6f67 7261 6d73 206f 6620 746f  ectrograms of to
+00000980: 7263 6861 7564 696f 2060 5350 4545 4348  rchaudio `SPEECH
+00000990: 434f 4d4d 414e 4453 6020 6461 7461 7365  COMMANDS` datase
+000009a0: 742c 2075 7369 6e67 2060 7061 636b 5f74  t, using `pack_t
+000009b0: 6f5f 7069 636b 6c65 6020 6675 6e63 7469  o_pickle` functi
+000009c0: 6f6e 3a0a 0a60 6060 7079 7468 6f6e 0a66  on:..```python.f
+000009d0: 726f 6d20 746f 7263 6820 696d 706f 7274  rom torch import
+000009e0: 206e 6e0a 6672 6f6d 2074 6f72 6368 6175   nn.from torchau
+000009f0: 6469 6f2e 6461 7461 7365 7473 2069 6d70  dio.datasets imp
+00000a00: 6f72 7420 5350 4545 4348 434f 4d4d 414e  ort SPEECHCOMMAN
+00000a10: 4453 0a66 726f 6d20 746f 7263 6861 7564  DS.from torchaud
+00000a20: 696f 2e74 7261 6e73 666f 726d 7320 696d  io.transforms im
+00000a30: 706f 7274 2053 7065 6374 726f 6772 616d  port Spectrogram
+00000a40: 0a66 726f 6d20 746f 7263 686f 7574 696c  .from torchoutil
+00000a50: 2e75 7469 6c73 2e70 6963 6b6c 655f 6461  .utils.pickle_da
+00000a60: 7461 7365 7420 696d 706f 7274 2070 6163  taset import pac
+00000a70: 6b5f 746f 5f70 6963 6b6c 650a 0a73 7065  k_to_pickle..spe
+00000a80: 6563 685f 636f 6d6d 616e 6473 5f72 6f6f  ech_commands_roo
+00000a90: 7420 3d20 2270 6174 682f 746f 2f73 7065  t = "path/to/spe
+00000aa0: 6563 685f 636f 6d6d 616e 6473 220a 7069  ech_commands".pi
+00000ab0: 636b 6c65 5f72 6f6f 7420 3d20 2270 6174  ckle_root = "pat
+00000ac0: 682f 746f 2f70 6963 6b6c 655f 6461 7461  h/to/pickle_data
+00000ad0: 7365 7422 0a0a 6461 7461 7365 7420 3d20  set"..dataset = 
+00000ae0: 5350 4545 4348 434f 4d4d 414e 4453 2873  SPEECHCOMMANDS(s
+00000af0: 7065 6563 685f 636f 6d6d 616e 6473 5f72  peech_commands_r
+00000b00: 6f6f 742c 2064 6f77 6e6c 6f61 643d 5472  oot, download=Tr
+00000b10: 7565 2c20 7375 6273 6574 3d22 7661 6c69  ue, subset="vali
+00000b20: 6461 7469 6f6e 2229 0a0a 636c 6173 7320  dation")..class 
+00000b30: 4d79 5472 616e 7366 6f72 6d28 6e6e 2e4d  MyTransform(nn.M
+00000b40: 6f64 756c 6529 3a0a 2020 2020 6465 6620  odule):.    def 
+00000b50: 5f5f 696e 6974 5f5f 2873 656c 6629 202d  __init__(self) -
+00000b60: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00000b70: 7375 7065 7228 292e 5f5f 696e 6974 5f5f  super().__init__
+00000b80: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+00000b90: 7370 6563 7472 6f67 7261 6d5f 6578 7472  spectrogram_extr
+00000ba0: 6163 746f 7220 3d20 5370 6563 7472 6f67  actor = Spectrog
+00000bb0: 7261 6d28 290a 0a20 2020 2064 6566 2066  ram()..    def f
+00000bc0: 6f72 7761 7264 2873 656c 662c 2069 7465  orward(self, ite
+00000bd0: 6d29 3a0a 2020 2020 2020 2020 7761 7665  m):.        wave
+00000be0: 666f 726d 203d 2069 7465 6d5b 305d 0a20  form = item[0]. 
+00000bf0: 2020 2020 2020 2073 7065 6374 726f 6772         spectrogr
+00000c00: 616d 203d 2073 656c 662e 7370 6563 7472  am = self.spectr
+00000c10: 6f67 7261 6d5f 6578 7472 6163 746f 7228  ogram_extractor(
+00000c20: 7761 7665 666f 726d 290a 2020 2020 2020  waveform).      
+00000c30: 2020 7265 7475 726e 2028 7370 6563 7472    return (spectr
+00000c40: 6f67 7261 6d2c 2920 2b20 6974 656d 5b31  ogram,) + item[1
+00000c50: 3a5d 0a0a 7061 636b 5f74 6f5f 7069 636b  :]..pack_to_pick
+00000c60: 6c65 2864 6174 6173 6574 2c20 7069 636b  le(dataset, pick
+00000c70: 6c65 5f72 6f6f 742c 204d 7954 7261 6e73  le_root, MyTrans
+00000c80: 666f 726d 2829 290a 6060 600a 0a54 6865  form()).```..The
+00000c90: 6e20 796f 7520 6361 6e20 6c6f 6164 2074  n you can load t
+00000ca0: 6865 2070 7265 2d63 6f6d 7075 7465 6420  he pre-computed 
+00000cb0: 6461 7461 7365 7420 7573 696e 6720 6050  dataset using `P
+00000cc0: 6963 6b6c 6544 6174 6173 6574 603a 0a60  ickleDataset`:.`
+00000cd0: 6060 7079 7468 6f6e 0a66 726f 6d20 746f  ``python.from to
+00000ce0: 7263 686f 7574 696c 2e75 7469 6c73 2e70  rchoutil.utils.p
+00000cf0: 6963 6b6c 655f 6461 7461 7365 7420 696d  ickle_dataset im
+00000d00: 706f 7274 2050 6963 6b6c 6544 6174 6173  port PickleDatas
+00000d10: 6574 0a0a 7069 636b 6c65 5f72 6f6f 7420  et..pickle_root 
+00000d20: 3d20 2270 6174 682f 746f 2f70 6963 6b6c  = "path/to/pickl
+00000d30: 655f 6461 7461 7365 7422 0a70 6963 6b6c  e_dataset".pickl
+00000d40: 655f 6461 7461 7365 7420 3d20 5069 636b  e_dataset = Pick
+00000d50: 6c65 4461 7461 7365 7428 7069 636b 6c65  leDataset(pickle
+00000d60: 5f72 6f6f 7429 0a70 6963 6b6c 655f 6461  _root).pickle_da
+00000d70: 7461 7365 745b 305d 2020 2320 3d3d 2066  taset[0]  # == f
+00000d80: 6972 7374 2074 7261 6e73 666f 726d 6564  irst transformed
+00000d90: 2069 7465 6d2c 2069 2e65 2e20 7472 616e   item, i.e. tran
+00000da0: 7366 6f72 6d28 6461 7461 7365 745b 305d  sform(dataset[0]
+00000db0: 290a 6060 600a 0a23 2323 202e 2e2e 616e  ).```..### ...an
+00000dc0: 6420 6d6f 7265 2074 656e 736f 7220 6d61  d more tensor ma
+00000dd0: 6e69 7075 6c61 7469 6f6e 7321 0a0a 6060  nipulations!..``
+00000de0: 6070 7974 686f 6e0a 696d 706f 7274 2074  `python.import t
+00000df0: 6f72 6368 0a66 726f 6d20 746f 7263 686f  orch.from torcho
+00000e00: 7574 696c 2069 6d70 6f72 7420 696e 7365  util import inse
+00000e10: 7274 5f61 745f 696e 6469 6365 730a 0a78  rt_at_indices..x
+00000e20: 203d 2074 6f72 6368 2e61 735f 7465 6e73   = torch.as_tens
+00000e30: 6f72 285b 312c 2032 2c20 332c 2034 5d29  or([1, 2, 3, 4])
+00000e40: 0a72 6573 756c 7420 3d20 696e 7365 7274  .result = insert
+00000e50: 5f61 745f 696e 6469 6365 7328 782c 2069  _at_indices(x, i
+00000e60: 6e64 6963 6573 3d5b 302c 2032 5d2c 2076  ndices=[0, 2], v
+00000e70: 616c 7565 733d 3529 0a23 2072 6573 756c  alues=5).# resul
+00000e80: 7420 636f 6e74 6169 6e73 2074 656e 736f  t contains tenso
+00000e90: 7220 7769 7468 2069 6e73 6572 7465 6420  r with inserted 
+00000ea0: 7661 6c75 6573 3a20 7465 6e73 6f72 285b  values: tensor([
+00000eb0: 352c 2031 2c20 322c 2035 2c20 332c 2034  5, 1, 2, 5, 3, 4
+00000ec0: 5d29 0a60 6060 0a0a 6060 6070 7974 686f  ]).```..```pytho
+00000ed0: 6e0a 696d 706f 7274 2074 6f72 6368 0a66  n.import torch.f
+00000ee0: 726f 6d20 746f 7263 686f 7574 696c 2069  rom torchoutil i
+00000ef0: 6d70 6f72 7420 6765 745f 696e 7665 7273  mport get_invers
+00000f00: 655f 7065 726d 0a0a 7065 726d 203d 2074  e_perm..perm = t
+00000f10: 6f72 6368 2e72 616e 6470 6572 6d28 3130  orch.randperm(10
+00000f20: 290a 696e 765f 7065 726d 203d 2067 6574  ).inv_perm = get
+00000f30: 5f69 6e76 6572 7365 5f70 6572 6d28 7065  _inverse_perm(pe
+00000f40: 726d 290a 0a78 3120 3d20 746f 7263 682e  rm)..x1 = torch.
+00000f50: 7261 6e64 2831 3029 0a78 3220 3d20 7831  rand(10).x2 = x1
+00000f60: 5b70 6572 6d5d 0a78 3320 3d20 7832 5b69  [perm].x3 = x2[i
+00000f70: 6e76 5f70 6572 6d5d 0a23 2069 6e76 5f70  nv_perm].# inv_p
+00000f80: 6572 6d20 6172 6520 696e 6469 6365 7320  erm are indices 
+00000f90: 7468 6174 2061 6c6c 6f77 2075 7320 746f  that allow us to
+00000fa0: 2067 6574 2078 3320 6672 6f6d 2078 322c   get x3 from x2,
+00000fb0: 2069 2e65 2e20 7831 203d 3d20 7833 2068   i.e. x1 == x3 h
+00000fc0: 6572 650a 6060 600a 0a23 2320 4578 7472  ere.```..## Extr
+00000fd0: 6173 0a60 746f 7263 686f 7574 696c 6020  as.`torchoutil` 
+00000fe0: 616c 736f 2070 726f 7669 6465 7320 6164  also provides ad
+00000ff0: 6469 7469 6f6e 616c 206d 6f64 756c 6573  ditional modules
+00001000: 2077 6865 6e20 736f 6d65 2073 7065 6369   when some speci
+00001010: 6669 6320 7061 636b 6167 6520 6172 6520  fic package are 
+00001020: 616c 7265 6164 7920 696e 7374 616c 6c65  already installe
+00001030: 6420 696e 2079 6f75 7220 656e 7669 726f  d in your enviro
+00001040: 6e6d 656e 742e 0a41 6c6c 2065 7874 7261  nment..All extra
+00001050: 7320 6361 6e20 6265 2069 6e73 7461 6c6c  s can be install
+00001060: 6564 2077 6974 6820 6070 6970 2069 6e73  ed with `pip ins
+00001070: 7461 6c6c 2074 6f72 6368 6f75 7469 6c5b  tall torchoutil[
+00001080: 6578 7472 6173 5d60 0a0a 2d20 4966 2060  extras]`..- If `
+00001090: 7465 6e73 6f72 626f 6172 6460 2069 7320  tensorboard` is 
+000010a0: 696e 7374 616c 6c65 642c 2074 6865 2066  installed, the f
+000010b0: 756e 6374 696f 6e20 606c 6f61 645f 6576  unction `load_ev
+000010c0: 656e 745f 6669 6c65 6020 6361 6e20 6265  ent_file` can be
+000010d0: 2075 7365 642e 2049 7420 6973 2075 7365   used. It is use
+000010e0: 6675 6c20 746f 206c 6f61 6420 6d61 6e75  ful to load manu
+000010f0: 616c 6c79 2061 6c6c 2064 6174 6120 636f  ally all data co
+00001100: 6e74 6169 6e65 6420 696e 2061 6e20 7465  ntained in an te
+00001110: 6e73 6f72 626f 6172 6420 6576 656e 7420  nsorboard event 
+00001120: 6669 6c65 2e0a 2d20 4966 2060 6e75 6d70  file..- If `nump
+00001130: 7960 2069 7320 696e 7374 616c 6c65 642c  y` is installed,
+00001140: 2074 6865 2063 6c61 7373 6573 2060 4672   the classes `Fr
+00001150: 6f6d 4e75 6d70 7960 2061 6e64 2020 6054  omNumpy` and  `T
+00001160: 6f4e 756d 7079 6020 6361 6e20 6265 2075  oNumpy` can be u
+00001170: 7365 6420 616e 6420 7468 6569 7220 7265  sed and their re
+00001180: 6c61 7465 6420 6675 6e63 7469 6f6e 2e20  lated function. 
+00001190: 4974 2069 7320 6d65 616e 7420 746f 2062  It is meant to b
+000011a0: 6520 7573 6564 2074 6f20 636f 6d70 6f73  e used to compos
+000011b0: 6520 6479 6e61 6d69 6320 7472 616e 7366  e dynamic transf
+000011c0: 6f72 6d73 2069 6e74 6f20 6053 6571 7565  orms into `Seque
+000011d0: 6e74 6961 6c60 206d 6f64 756c 652e 0a2d  ntial` module..-
+000011e0: 2049 6620 6068 3570 7960 2069 7320 696e   If `h5py` is in
+000011f0: 7374 616c 6c65 642c 2074 6865 2066 756e  stalled, the fun
+00001200: 6374 696f 6e20 6070 6163 6b5f 746f 5f68  ction `pack_to_h
+00001210: 6466 6020 616e 6420 636c 6173 7320 6048  df` and class `H
+00001220: 4446 4461 7461 7365 7460 2063 616e 2062  DFDataset` can b
+00001230: 6520 7573 6564 2e20 4361 6e20 6265 2075  e used. Can be u
+00001240: 7365 6420 746f 2070 6163 6b2f 7265 6164  sed to pack/read
+00001250: 2064 6174 6173 6574 2074 6f20 4844 4620   dataset to HDF 
+00001260: 6669 6c65 732c 2061 6e64 2073 7570 706f  files, and suppo
+00001270: 7274 7320 7661 7269 6162 6c65 2d6c 656e  rts variable-len
+00001280: 6774 6820 7365 7175 656e 6365 7320 6f66  gth sequences of
+00001290: 2064 6174 612e 0a0a 0a23 2320 436f 6e74   data....## Cont
+000012a0: 6163 740a 4d61 696e 7461 696e 6572 3a0a  act.Maintainer:.
+000012b0: 2d20 5bc3 8974 6965 6e6e 6520 4c61 6262  - [..tienne Labb
+000012c0: c3a9 5d28 6874 7470 733a 2f2f 6c61 6262  ..](https://labb
+000012d0: 6574 692e 6769 7468 7562 2e69 6f2f 2920  eti.github.io/) 
+000012e0: 224c 6162 6265 7469 223a 206c 6162 6265  "Labbeti": labbe
+000012f0: 7469 2e70 7562 4067 6d61 696c 2e63 6f6d  ti.pub@gmail.com
+00001300: 0a                                       .
```

### Comparing `torchoutil-0.3.0/pyproject.toml` & `torchoutil-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `torchoutil-0.3.0/src/torchoutil/hub/download.py` & `torchoutil-0.3.1/src/torchoutil/hub/download.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.3.0/src/torchoutil/hub/registry.py` & `torchoutil-0.3.1/src/torchoutil/hub/registry.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.3.0/src/torchoutil/info.py` & `torchoutil-0.3.1/src/torchoutil/info.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.3.0/src/torchoutil/nn/functional/crop.py` & `torchoutil-0.3.1/src/torchoutil/nn/functional/crop.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.3.0/src/torchoutil/nn/functional/indices.py` & `torchoutil-0.3.1/src/torchoutil/nn/functional/indices.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.3.0/src/torchoutil/nn/functional/mask.py` & `torchoutil-0.3.1/src/torchoutil/nn/functional/mask.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.3.0/src/torchoutil/nn/functional/multiclass.py` & `torchoutil-0.3.1/src/torchoutil/nn/functional/multiclass.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,56 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 """Helper functions for conversion between classes indices, onehot, names and probabilities for multiclass classification.
 """
 
-from typing import List, Mapping, Sequence, TypeVar, Union
+from typing import List, Mapping, Optional, Sequence, TypeVar, Union
 
 import torch
 from torch import Tensor
 from torch.nn import functional as F
 
 from torchoutil.nn.functional.get import get_device
 
 T = TypeVar("T")
 
 
 def indices_to_onehot(
-    indices: Union[Sequence[int], Tensor],
+    indices: Union[Sequence[int], Tensor, Sequence],
     num_classes: int,
     *,
+    padding_idx: Optional[int] = None,
     device: Union[str, torch.device, None] = None,
     dtype: Union[torch.dtype, None] = torch.bool,
 ) -> Tensor:
     """Convert indices of labels to onehot boolean encoding.
 
     Args:
-        indices: List of list of label indices.
+        indices: List label indices.
+            Can be a nested list of indices, but it should be convertible to Tensor.
         num_classes: Number maximal of unique classes.
+        padding_idx: Class index to ignore. Output will contains only zeroes for this value. defaults to None.
         device: PyTorch device of the output tensor.
         dtype: PyTorch DType of the output tensor.
     """
     device = get_device(device)
     indices = torch.as_tensor(indices, device=device, dtype=torch.long)
-    onehot = F.one_hot(indices, num_classes)
+
+    if padding_idx is not None:
+        mask = indices == padding_idx
+        indices = torch.where(mask, num_classes, indices)
+        num_classes += 1
+
+    onehot: Tensor = F.one_hot(indices, num_classes)
     onehot = onehot.to(dtype=dtype)
+
+    if padding_idx is not None:
+        onehot = onehot[..., :-1].contiguous()
+
     return onehot
 
 
 def indices_to_names(
     indices: Union[Sequence[int], Tensor],
     idx_to_name: Mapping[int, T],
 ) -> List[T]:
@@ -54,15 +67,15 @@
     onehot: Tensor,
 ) -> List[int]:
     """Convert onehot boolean encoding to indices of labels.
 
     Args:
         onehot: OneHot labels encoded as 2D matrix.
     """
-    return onehot.argmax(dim=-1).tolist()
+    return onehot.int().argmax(dim=-1).tolist()
 
 
 def onehot_to_names(
     onehot: Tensor,
     idx_to_name: Mapping[int, T],
 ) -> List[T]:
     """Convert onehot boolean encoding to names using a mapping.
```

### Comparing `torchoutil-0.3.0/src/torchoutil/nn/functional/multilabel.py` & `torchoutil-0.3.1/src/torchoutil/nn/functional/multilabel.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.3.0/src/torchoutil/nn/functional/numpy.py` & `torchoutil-0.3.1/src/torchoutil/nn/functional/numpy.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-from typing import Any, Union
+from typing import Any, Literal, Union
 
 import torch
 from torch import Tensor
 from typing_extensions import TypeGuard
 
 from torchoutil.nn.functional.get import get_device
 from torchoutil.utils.packaging import _NUMPY_AVAILABLE
 
-if _NUMPY_AVAILABLE:
+if not _NUMPY_AVAILABLE:
+
+    def is_numpy_scalar(x: Any) -> Literal[False]:
+        return False
+
+else:
     import numpy as np
 
     def to_numpy(
         x: Union[Tensor, np.ndarray, list],
+        *,
         dtype: Union[str, np.dtype, None] = None,
     ) -> np.ndarray:
         if isinstance(x, Tensor):
             return x.cpu().numpy().astype(dtype=dtype)
         else:
             return np.asarray(x, dtype=dtype)
 
     def from_numpy(
         x: np.ndarray,
-        dtype: Union[torch.dtype, None] = None,
+        *,
         device: Union[str, torch.device, None] = None,
+        dtype: Union[torch.dtype, None] = None,
     ) -> Tensor:
         device = get_device(device)
         return torch.from_numpy(x).to(dtype=dtype, device=device)
 
-    def is_numpy_scalar(x: Any) -> TypeGuard[np.generic]:
-        return np.isscalar(x) and x.__class__.__module__ != "__builtin__"
+    def is_numpy_scalar(x: Any) -> TypeGuard[Union[np.generic, np.ndarray]]:
+        """Returns True if x is a numpy generic type or a zero-dimensional numpy array."""
+        return isinstance(x, np.generic) or (isinstance(x, np.ndarray) and x.ndim == 0)
```

### Comparing `torchoutil-0.3.0/src/torchoutil/nn/functional/others.py` & `torchoutil-0.3.1/src/torchoutil/nn/functional/others.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,23 +18,33 @@
 )
 
 import torch
 from torch import Tensor, nn
 from typing_extensions import TypeGuard
 
 from torchoutil.nn.functional.get import get_device
+from torchoutil.nn.functional.numpy import is_numpy_scalar
 
 T = TypeVar("T")
 U = TypeVar("U")
 
 
-def count_parameters(model: nn.Module, only_trainable: bool = False) -> int:
-    params = (p for p in model.parameters() if not only_trainable or p.requires_grad)
-    count = sum(p.numel() for p in params)
-    return count
+def count_parameters(
+    model: nn.Module,
+    *,
+    recurse: bool = True,
+    only_trainable: bool = False,
+) -> int:
+    params = (
+        param
+        for param in model.parameters(recurse)
+        if not only_trainable or param.requires_grad
+    )
+    num_params = sum(param.numel() for param in params)
+    return num_params
 
 
 def find(
     x: Tensor,
     value: Any,
     default: Union[None, Tensor, int, float] = None,
     dim: int = -1,
@@ -102,23 +112,25 @@
         else:
             return list(generator)
     else:
         return x
 
 
 def is_python_scalar(x: Any) -> TypeGuard[Union[int, float, bool, complex]]:
+    """Returns True if x is a builtin scalar type (int, float, bool, complex)."""
     return isinstance(x, (int, float, bool, complex))
 
 
 def is_torch_scalar(x: Any) -> TypeGuard[Tensor]:
+    """Returns True if x is a zero-dimensional torch Tensor."""
     return isinstance(x, Tensor) and x.ndim == 0
 
 
 def is_scalar(x: Any) -> TypeGuard[Union[int, float, bool, complex, Tensor]]:
-    return is_python_scalar(x) or is_torch_scalar(x)
+    return is_python_scalar(x) or is_torch_scalar(x) or is_numpy_scalar(x)
 
 
 def can_be_stacked(
     tensors: Union[List[Any], Tuple[Any, ...]],
 ) -> TypeGuard[Union[List[Tensor], Tuple[Tensor, ...]]]:
     if len(tensors) == 0:
         return True
```

### Comparing `torchoutil-0.3.0/src/torchoutil/nn/functional/pad.py` & `torchoutil-0.3.1/src/torchoutil/nn/functional/pad.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-from typing import Any, Dict, Iterable, List, Literal, Sized, Tuple, Union
+from typing import Any, Callable, Dict, Iterable, List, Literal, Sized, Tuple, Union
 
 import torch
 from torch import Generator, Size, Tensor
 from torch.nn import functional as F
 from torch.types import Number
 
 from torchoutil.nn.functional.get import get_device
 from torchoutil.nn.functional.others import can_be_stacked, is_scalar
 
 PAD_ALIGNS = ("left", "right", "center", "random")
 PadAlign = Literal["left", "right", "center", "random"]
+PadValue = Union[Number, Callable[[Tensor], Number]]
 
 
 def pad_dim(
     x: Tensor,
     target_length: int,
     align: PadAlign = "left",
-    pad_value: float = 0.0,
+    pad_value: PadValue = 0.0,
     dim: int = -1,
     mode: str = "constant",
     generator: Union[int, Generator, None] = None,
 ) -> Tensor:
     """Generic function for pad a single dimension."""
     return pad_dims(x, [target_length], [align], pad_value, [dim], mode, generator)
 
 
 def pad_dims(
     x: Tensor,
     target_lengths: Iterable[int],
     aligns: Iterable[PadAlign] = ("left",),
-    pad_value: float = 0.0,
+    pad_value: PadValue = 0.0,
     dims: Iterable[int] = (-1,),
     mode: str = "constant",
     generator: Union[int, Generator, None] = None,
 ) -> Tensor:
     """Generic function to pad multiple dimensions."""
     if isinstance(generator, int):
         generator = Generator().manual_seed(generator)
@@ -56,14 +57,17 @@
         )
 
     if len(aligns) != len(dims):
         raise ValueError(
             f"Invalid number of aligns ({len(aligns)}) with the number of dimensions ({len(dims)})."
         )
 
+    if isinstance(pad_value, Callable):
+        pad_value = pad_value(x)
+
     pad_seq = __generate_pad_seq(x.shape, target_lengths, dims, aligns, generator)
     x = F.pad(x, pad_seq, mode=mode, value=pad_value)
     return x
 
 
 def pad_and_stack_rec(
     sequence: Union[Tensor, int, float, tuple, list],
```

### Comparing `torchoutil-0.3.0/src/torchoutil/nn/modules/activation.py` & `torchoutil-0.3.1/src/torchoutil/nn/modules/activation.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 from torch import Tensor, nn
 
 from torchoutil.nn.functional.activation import softmax_multidim
 from torchoutil.utils.collections import dump_dict
 
 
 class SoftmaxMultidim(nn.Module):
+    """
+    For more information, see :func:`~torchoutil.nn.functional.activation.softmax_multidim`.
+    """
+
     def __init__(
         self,
         dims: Union[Iterable[int], None] = (-1,),
     ) -> None:
         if dims is not None:
             dims = tuple(dims)
```

### Comparing `torchoutil-0.3.0/src/torchoutil/nn/modules/crop.py` & `torchoutil-0.3.1/src/torchoutil/nn/modules/crop.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from typing import Iterable, Union
 
 from torch import Generator, Tensor, nn
 
-from torchoutil.nn.functional.crop import crop_dim, crop_dims, CropAlign
+from torchoutil.nn.functional.crop import CropAlign, crop_dim, crop_dims
 from torchoutil.utils.collections import dump_dict
 
 
 class CropDim(nn.Module):
+    """
+    For more information, see :func:`~torchoutil.nn.functional.crop.crop_dim`.
+    """
+
     def __init__(
         self,
         target_length: int,
         align: CropAlign = "left",
         dim: int = -1,
         generator: Union[int, Generator, None] = None,
     ) -> None:
@@ -42,14 +46,18 @@
                 align=self.align,
                 dim=self.dim,
             )
         )
 
 
 class CropDims(nn.Module):
+    """
+    For more information, see :func:`~torchoutil.nn.functional.crop.crop_dims`.
+    """
+
     def __init__(
         self,
         target_lengths: Iterable[int],
         aligns: Iterable[CropAlign] = ("left",),
         dims: Iterable[int] = (-1,),
         generator: Union[int, Generator, None] = None,
     ) -> None:
```

### Comparing `torchoutil-0.3.0/src/torchoutil/nn/modules/layer.py` & `torchoutil-0.3.1/src/torchoutil/nn/modules/layer.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.3.0/src/torchoutil/nn/modules/mask.py` & `torchoutil-0.3.1/src/torchoutil/nn/modules/mask.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 from torch import Tensor, nn
 
 from torchoutil.nn.functional.mask import masked_mean, masked_sum
 from torchoutil.utils.collections import dump_dict
 
 
 class MaskedMean(nn.Module):
+    """
+    For more information, see :func:`~torchoutil.nn.functional.mask.masked_mean`.
+    """
+
     def __init__(self, dim: Union[None, int, Iterable[int]] = None) -> None:
         super().__init__()
         self.dim = dim
 
     def forward(self, tensor: Tensor, non_pad_mask: Tensor) -> Tensor:
         reduced = masked_mean(tensor, non_pad_mask, self.dim)
         return reduced
@@ -24,14 +28,18 @@
                 dim=self.dim,
             ),
             ignore_none=True,
         )
 
 
 class MaskedSum(nn.Module):
+    """
+    For more information, see :func:`~torchoutil.nn.functional.mask.masked_sum`.
+    """
+
     def __init__(self, dim: Union[None, int, Iterable[int]] = None) -> None:
         super().__init__()
         self.dim = dim
 
     def forward(self, tensor: Tensor, non_pad_mask: Tensor) -> Tensor:
         reduced = masked_sum(tensor, non_pad_mask, self.dim)
         return reduced
```

### Comparing `torchoutil-0.3.0/src/torchoutil/nn/modules/multiclass.py` & `torchoutil-0.3.1/src/torchoutil/nn/modules/multiclass.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-from typing import Generic, List, Mapping, TypeVar, Union
+from typing import Generic, List, Mapping, Optional, TypeVar, Union
 
 import torch
 from torch import Tensor, nn
 
 from torchoutil.nn.functional.multiclass import (
     indices_to_names,
     indices_to_onehot,
@@ -19,50 +19,62 @@
 )
 from torchoutil.utils.collections import dump_dict
 
 T = TypeVar("T")
 
 
 class IndicesToOneHot(nn.Module):
+    """
+    For more information, see :func:`~torchoutil.nn.functional.multiclass.indices_to_onehot`.
+    """
+
     def __init__(
         self,
         num_classes: int,
         *,
+        padding_idx: Optional[int] = None,
         device: Union[str, torch.device, None] = None,
         dtype: Union[torch.dtype, None] = torch.bool,
     ) -> None:
         super().__init__()
         self.num_classes = num_classes
+        self.padding_idx = padding_idx
         self.device = device
         self.dtype = dtype
 
     def forward(
         self,
         indices: Union[List[int], Tensor],
     ) -> Tensor:
         onehot = indices_to_onehot(
             indices,
             self.num_classes,
+            padding_idx=self.padding_idx,
             device=self.device,
             dtype=self.dtype,
         )
         return onehot
 
     def extra_repr(self) -> str:
         return dump_dict(
             dict(
                 num_classes=self.num_classes,
+                padding_idx=self.padding_idx,
                 device=self.device,
                 dtype=self.dtype,
             ),
             ignore_none=True,
         )
 
 
 class IndicesToNames(nn.Module, Generic[T]):
+    """
+    For more information, see :func:`~torchoutil.nn.functional.multiclass.indices_to_names`.
+    """
+
     def __init__(
         self,
         idx_to_name: Mapping[int, T],
     ) -> None:
         super().__init__()
         self.idx_to_name = idx_to_name
 
@@ -71,26 +83,34 @@
         indices: Union[List[int], Tensor],
     ) -> List[T]:
         names = indices_to_names(indices, self.idx_to_name)
         return names
 
 
 class OneHotToIndices(nn.Module):
+    """
+    For more information, see :func:`~torchoutil.nn.functional.multiclass.onehot_to_indices`.
+    """
+
     def __init__(self) -> None:
         super().__init__()
 
     def forward(
         self,
         onehot: Tensor,
     ) -> List[int]:
         names = onehot_to_indices(onehot)
         return names
 
 
 class OneHotToNames(nn.Module, Generic[T]):
+    """
+    For more information, see :func:`~torchoutil.nn.functional.multiclass.onehot_to_names`.
+    """
+
     def __init__(
         self,
         idx_to_name: Mapping[int, T],
     ) -> None:
         super().__init__()
         self.idx_to_name = idx_to_name
 
@@ -99,14 +119,18 @@
         onehot: Tensor,
     ) -> List[T]:
         names = onehot_to_names(onehot, self.idx_to_name)
         return names
 
 
 class NamesToIndices(nn.Module, Generic[T]):
+    """
+    For more information, see :func:`~torchoutil.nn.functional.multiclass.names_to_indices`.
+    """
+
     def __init__(
         self,
         idx_to_name: Mapping[int, T],
     ) -> None:
         super().__init__()
         self.idx_to_name = idx_to_name
 
@@ -115,14 +139,18 @@
         names: List[T],
     ) -> List[int]:
         indices = names_to_indices(names, self.idx_to_name)
         return indices
 
 
 class NamesToOneHot(nn.Module, Generic[T]):
+    """
+    For more information, see :func:`~torchoutil.nn.functional.multiclass.names_to_onehot`.
+    """
+
     def __init__(
         self,
         idx_to_name: Mapping[int, T],
         *,
         device: Union[str, torch.device, None] = None,
         dtype: Union[torch.dtype, None] = torch.bool,
     ) -> None:
@@ -150,23 +178,31 @@
                 dtype=self.dtype,
             ),
             ignore_none=True,
         )
 
 
 class ProbsToIndices(nn.Module):
+    """
+    For more information, see :func:`~torchoutil.nn.functional.multiclass.probs_to_indices`.
+    """
+
     def forward(
         self,
         probs: Tensor,
     ) -> List[int]:
         indices = probs_to_indices(probs)
         return indices
 
 
 class ProbsToOneHot(nn.Module):
+    """
+    For more information, see :func:`~torchoutil.nn.functional.multiclass.probs_to_onehot`.
+    """
+
     def __init__(
         self,
         *,
         device: Union[str, torch.device, None] = None,
         dtype: Union[torch.dtype, None] = torch.bool,
     ) -> None:
         super().__init__()
@@ -191,14 +227,18 @@
                 dtype=self.dtype,
             ),
             ignore_none=True,
         )
 
 
 class ProbsToNames(nn.Module, Generic[T]):
+    """
+    For more information, see :func:`~torchoutil.nn.functional.multiclass.probs_to_names`.
+    """
+
     def __init__(
         self,
         idx_to_name: Mapping[int, T],
     ) -> None:
         super().__init__()
         self.idx_to_name = idx_to_name
```

### Comparing `torchoutil-0.3.0/src/torchoutil/nn/modules/multilabel.py` & `torchoutil-0.3.1/src/torchoutil/nn/modules/multilabel.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,14 +19,18 @@
 )
 from torchoutil.utils.collections import dump_dict
 
 T = TypeVar("T")
 
 
 class IndicesToMultihot(nn.Module):
+    """
+    For more information, see :func:`~torchoutil.nn.functional.multilabel.indices_to_multihot`.
+    """
+
     def __init__(
         self,
         num_classes: int,
         *,
         device: Union[str, torch.device, None] = None,
         dtype: Union[torch.dtype, None] = torch.bool,
     ) -> None:
@@ -55,14 +59,18 @@
                 dtype=self.dtype,
             ),
             ignore_none=True,
         )
 
 
 class IndicesToNames(nn.Module, Generic[T]):
+    """
+    For more information, see :func:`~torchoutil.nn.functional.multilabel.indices_to_names`.
+    """
+
     def __init__(
         self,
         idx_to_name: Mapping[int, T],
     ) -> None:
         super().__init__()
         self.idx_to_name = idx_to_name
 
@@ -71,26 +79,31 @@
         indices: Union[List[List[int]], List[Tensor]],
     ) -> List[List[T]]:
         names = indices_to_names(indices, self.idx_to_name)
         return names
 
 
 class MultihotToIndices(nn.Module):
-    def __init__(self) -> None:
-        super().__init__()
+    """
+    For more information, see :func:`~torchoutil.nn.functional.multilabel.multihot_to_indices`.
+    """
 
     def forward(
         self,
         multihot: Tensor,
     ) -> List[List[int]]:
         names = multihot_to_indices(multihot)
         return names
 
 
 class MultihotToNames(nn.Module, Generic[T]):
+    """
+    For more information, see :func:`~torchoutil.nn.functional.multilabel.multihot_to_names`.
+    """
+
     def __init__(
         self,
         idx_to_name: Mapping[int, T],
     ) -> None:
         super().__init__()
         self.idx_to_name = idx_to_name
 
@@ -99,14 +112,18 @@
         multihot: Tensor,
     ) -> List[List[T]]:
         names = multihot_to_names(multihot, self.idx_to_name)
         return names
 
 
 class NamesToIndices(nn.Module, Generic[T]):
+    """
+    For more information, see :func:`~torchoutil.nn.functional.multilabel.names_to_indices`.
+    """
+
     def __init__(
         self,
         idx_to_name: Mapping[int, T],
     ) -> None:
         super().__init__()
         self.idx_to_name = idx_to_name
 
@@ -115,14 +132,18 @@
         names: List[List[T]],
     ) -> List[List[int]]:
         indices = names_to_indices(names, self.idx_to_name)
         return indices
 
 
 class NamesToMultihot(nn.Module, Generic[T]):
+    """
+    For more information, see :func:`~torchoutil.nn.functional.multilabel.names_to_multihot`.
+    """
+
     def __init__(
         self,
         idx_to_name: Mapping[int, T],
         *,
         device: Union[str, torch.device, None] = None,
         dtype: Union[torch.dtype, None] = torch.bool,
     ) -> None:
@@ -150,14 +171,18 @@
                 dtype=self.dtype,
             ),
             ignore_none=True,
         )
 
 
 class ProbsToIndices(nn.Module):
+    """
+    For more information, see :func:`~torchoutil.nn.functional.multilabel.probs_to_indices`.
+    """
+
     def __init__(
         self,
         threshold: Union[float, Tensor],
     ) -> None:
         super().__init__()
         self.threshold = threshold
 
@@ -166,14 +191,18 @@
         probs: Tensor,
     ) -> List[List[int]]:
         indices = probs_to_indices(probs, self.threshold)
         return indices
 
 
 class ProbsToMultihot(nn.Module):
+    """
+    For more information, see :func:`~torchoutil.nn.functional.multilabel.probs_to_multihot`.
+    """
+
     def __init__(
         self,
         threshold: Union[float, Tensor],
         *,
         device: Union[str, torch.device, None] = None,
         dtype: Union[torch.dtype, None] = torch.bool,
     ) -> None:
@@ -201,14 +230,18 @@
                 dtype=self.dtype,
             ),
             ignore_none=True,
         )
 
 
 class ProbsToNames(nn.Module, Generic[T]):
+    """
+    For more information, see :func:`~torchoutil.nn.functional.multilabel.probs_to_names`.
+    """
+
     def __init__(
         self,
         threshold: Union[float, Tensor],
         idx_to_name: Mapping[int, T],
     ) -> None:
         super().__init__()
         self.threshold = threshold
```

### Comparing `torchoutil-0.3.0/src/torchoutil/nn/modules/numpy.py` & `torchoutil-0.3.1/src/torchoutil/nn/modules/numpy.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,27 +10,35 @@
 
 if _NUMPY_AVAILABLE:
     import numpy as np
 
     from torchoutil.nn.functional.numpy import from_numpy, to_numpy
 
     class ToNumpy(nn.Module):
+        """
+        For more information, see :func:`~torchoutil.nn.functional.numpy.to_numpy`.
+        """
+
         def __init__(self, *, dtype: Union[str, np.dtype, None] = None) -> None:
             super().__init__()
             self.dtype = dtype
 
         def forward(self, x: Union[Tensor, np.ndarray, list]) -> np.ndarray:
-            return to_numpy(x, self.dtype)
+            return to_numpy(x, dtype=self.dtype)
 
     class FromNumpy(nn.Module):
+        """
+        For more information, see :func:`~torchoutil.nn.functional.numpy.from_numpy`.
+        """
+
         def __init__(
             self,
             *,
             device: Union[str, torch.device, None] = None,
             dtype: Union[torch.dtype, None] = None,
         ) -> None:
             super().__init__()
             self.device = device
             self.dtype = dtype
 
         def forward(self, x: np.ndarray) -> Tensor:
-            return from_numpy(x, self.dtype, self.device)
+            return from_numpy(x, dtype=self.dtype, device=self.device)
```

### Comparing `torchoutil-0.3.0/src/torchoutil/nn/modules/pad.py` & `torchoutil-0.3.1/src/torchoutil/nn/modules/pad.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,48 +3,58 @@
 
 from typing import Iterable, Union
 
 import torch
 from torch import Generator, Tensor, nn
 from torch.types import Number
 
-from torchoutil.nn.functional.pad import PadAlign, pad_and_stack_rec, pad_dim, pad_dims
+from torchoutil.nn.functional.pad import (
+    PadAlign,
+    PadValue,
+    pad_and_stack_rec,
+    pad_dim,
+    pad_dims,
+)
 from torchoutil.utils.collections import dump_dict
 
 
 class PadDim(nn.Module):
+    """
+    For more information, see :func:`~torchoutil.nn.functional.pad.pad_dim`.
+    """
+
     def __init__(
         self,
         target_length: int,
         align: PadAlign = "left",
-        pad_value: float = 0.0,
+        pad_value: PadValue = 0.0,
         dim: int = -1,
         mode: str = "constant",
         generator: Union[int, Generator, None] = None,
     ) -> None:
         super().__init__()
         self.target_length = target_length
-        self.align = align
+        self.align: PadAlign = align
         self.pad_value = pad_value
         self.dim = dim
         self.mode = mode
         self.generator = generator
 
     def forward(
         self,
         x: Tensor,
     ) -> Tensor:
         return pad_dim(
             x,
-            self.target_length,
-            self.align,  # type: ignore
-            self.pad_value,
-            self.dim,
-            self.mode,
-            self.generator,
+            target_length=self.target_length,
+            align=self.align,
+            pad_value=self.pad_value,
+            dim=self.dim,
+            mode=self.mode,
+            generator=self.generator,
         )
 
     def extra_repr(self) -> str:
         return dump_dict(
             dict(
                 target_length=self.target_length,
                 align=self.align,
@@ -52,19 +62,23 @@
                 dim=self.dim,
                 mode=self.mode,
             )
         )
 
 
 class PadDims(nn.Module):
+    """
+    For more information, see :func:`~torchoutil.nn.functional.pad.pad_dims`.
+    """
+
     def __init__(
         self,
         target_lengths: Iterable[int],
         aligns: Iterable[PadAlign] = ("left",),
-        pad_value: float = 0.0,
+        pad_value: PadValue = 0.0,
         dims: Iterable[int] = (-1,),
         mode: str = "constant",
         generator: Union[int, Generator, None] = None,
     ) -> None:
         super().__init__()
         self.target_lengths = target_lengths
         self.aligns = aligns
@@ -75,20 +89,20 @@
 
     def forward(
         self,
         x: Tensor,
     ) -> Tensor:
         return pad_dims(
             x,
-            self.target_lengths,
-            self.aligns,
-            self.pad_value,
-            self.dims,
-            self.mode,
-            self.generator,
+            target_lengths=self.target_lengths,
+            aligns=self.aligns,
+            pad_value=self.pad_value,
+            dims=self.dims,
+            mode=self.mode,
+            generator=self.generator,
         )
 
     def extra_repr(self) -> str:
         return dump_dict(
             dict(
                 target_lengths=self.target_lengths,
                 aligns=self.aligns,
@@ -96,14 +110,18 @@
                 dims=self.dims,
                 mode=self.mode,
             )
         )
 
 
 class PadAndStackRec(nn.Module):
+    """
+    For more information, see :func:`~torchoutil.nn.functional.pad.pad_and_stack_rec`.
+    """
+
     def __init__(
         self,
         pad_value: Number,
         *,
         device: Union[str, torch.device, None] = None,
         dtype: Union[None, torch.dtype] = None,
     ) -> None:
```

### Comparing `torchoutil-0.3.0/src/torchoutil/nn/modules/tensor.py` & `torchoutil-0.3.1/src/torchoutil/nn/modules/tensor.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.3.0/src/torchoutil/nn/modules/typed.py` & `torchoutil-0.3.1/src/torchoutil/nn/modules/typed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from typing import Any, Generic, OrderedDict, TypeVar, overload
 
 from torch import nn
 
+from torchoutil.nn.functional.others import count_parameters
+
 InType = TypeVar("InType", covariant=False, contravariant=True)
 OutType = TypeVar("OutType", covariant=True, contravariant=False)
 T1 = TypeVar("T1")
 T2 = TypeVar("T2")
 T3 = TypeVar("T3")
 T4 = TypeVar("T4")
 T5 = TypeVar("T5")
@@ -35,14 +37,23 @@
     def compose(self, other) -> "TSequential[InType, Any]":
         return TSequential(self, other)
 
     def duplicate(self, num: int) -> "TSequential[InType, OutType]":
         duplicated = [self] * num
         return TSequential(*duplicated)
 
+    def count_parameters(
+        self,
+        *,
+        recurse: bool = True,
+        only_trainable: bool = False,
+    ) -> int:
+        """Returns the number of parameters in this module."""
+        return count_parameters(self, recurse=recurse, only_trainable=only_trainable)
+
 
 class TSequential(Generic[InType, OutType], TModule[InType, OutType], nn.Sequential):
     """Typed version of torch.nn.Sequential, designed to work with torchoutil.nn.TModules."""
 
     @overload
     def __init__(
         self,
```

### Comparing `torchoutil-0.3.0/src/torchoutil/optim/utils.py` & `torchoutil-0.3.1/src/torchoutil/optim/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import logging
-from typing import Any, Iterable, List, Optional, Tuple, Union
+from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
 
 from torch import nn
 from torch.nn.parameter import Parameter
 from torch.optim.optimizer import Optimizer
 
 pylog = logging.getLogger(__name__)
 
 
-def get_lr(optim: Optimizer, idx: int = 0) -> float:
+def get_lr(optim: Optimizer, idx: int = 0, key: str = "lr") -> float:
     """
     Get the learning rate of the first group of an optimizer.
 
     Args:
         optim: The optimizer to get.
         idx: The group index of the learning rate in the optimizer. defaults to 0.
     """
-    return get_lrs(optim)[idx]
+    return get_lrs(optim, key)[idx]
 
 
-def get_lrs(optim: Optimizer) -> List[float]:
+def get_lrs(optim: Optimizer, key: str = "lr") -> List[float]:
     """
     Get the learning rates in all groups of an optimizer.
 
     Args:
         optim: The optimizer to get.
     """
-    return [group["lr"] for group in optim.param_groups]
+    return [group[key] for group in optim.param_groups]
 
 
 def create_params_groups_bias(
     model: Union[nn.Module, Iterable[Tuple[str, Parameter]]],
     weight_decay: float,
     skip_list: Optional[Iterable[str]] = (),
     verbose: int = 2,
-) -> list[dict[str, Any]]:
+) -> List[Dict[str, Any]]:
     if isinstance(model, nn.Module):
         params = model.named_parameters()
     else:
         params = model
     del model
 
-    decay: list[Parameter] = []
-    no_decay: list[Parameter] = []
+    decay: List[Parameter] = []
+    no_decay: List[Parameter] = []
 
     if skip_list is None:
         skip_list = {}
     else:
         skip_list = dict.fromkeys(skip_list)
 
     for name, param in params:
```

### Comparing `torchoutil-0.3.0/src/torchoutil/utils/collections.py` & `torchoutil-0.3.1/src/torchoutil/utils/collections.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     Sequence,
     Tuple,
     TypeVar,
     Union,
     overload,
 )
 
-from torchoutil.utils.type_checks import is_mapping_str_any
+from torchoutil.utils.type_checks import is_mapping_str
 
 K = TypeVar("K")
 T = TypeVar("T")
 U = TypeVar("U")
 V = TypeVar("V")
 W = TypeVar("W")
 
@@ -64,27 +64,84 @@
     """
     if len(lst) <= 0:
         return {}
 
     keys = set(lst[0].keys())
     if key_mode == "same":
         if not all(keys == set(item.keys()) for item in lst[1:]):
-            raise ValueError("Invalid keys for batch.")
+            raise ValueError(f"Invalid keys with {key_mode=}.")
     elif key_mode == "intersect":
         keys = intersect_lists([item.keys() for item in lst])
     elif key_mode == "union":
         keys = union_lists([item.keys() for item in lst])
     else:
         raise ValueError(
             f"Invalid argument key_mode={key_mode}. (expected one of {KEY_MODES})"
         )
 
     return {key: [item.get(key, default_val) for item in lst] for key in keys}
 
 
+@overload
+def dict_list_to_list_dict(
+    dic: Mapping[T, Sequence[U]],
+    key_mode: Literal["same", "intersect"],
+    default_val: Any = None,
+) -> List[Dict[T, U]]:
+    ...
+
+
+@overload
+def dict_list_to_list_dict(
+    dic: Mapping[T, Sequence[U]],
+    key_mode: Literal["union"] = "union",
+    default_val: W = None,
+) -> List[Dict[T, Union[U, W]]]:
+    ...
+
+
+def dict_list_to_list_dict(
+    dic: Mapping[T, Sequence[U]],
+    key_mode: KeyMode = "union",
+    default_val: W = None,
+) -> List[Dict[T, Union[U, W]]]:
+    """Convert dict of lists with same sizes to list of dicts.
+
+    Example 1
+    ----------
+    ```
+    >>> dic = {"a": [1, 2], "b": [3, 4]}
+    >>> dict_list_to_list_dict(dic)
+    ... [{"a": 1, "b": 3}, {"a": 2, "b": 4}]
+    ```
+    """
+    if len(dic) == 0:
+        return []
+
+    lengths = [len(seq) for seq in dic.values()]
+    if key_mode == "same":
+        if not all_eq(lengths):
+            raise ValueError("Invalid sequences for batch.")
+        length = lengths[0]
+    elif key_mode == "intersect":
+        length = min(lengths)
+    elif key_mode == "union":
+        length = max(lengths)
+    else:
+        raise ValueError(
+            f"Invalid argument key_mode={key_mode}. (expected one of {KEY_MODES})"
+        )
+
+    result = [
+        {k: (v[i] if i < len(v) else default_val) for k, v in dic.items()}
+        for i in range(length)
+    ]
+    return result
+
+
 def intersect_lists(lst_of_lst: Sequence[Iterable[T]]) -> List[T]:
     """Performs intersection of elements in lists (like set intersection), but keep their original order."""
     if len(lst_of_lst) <= 0:
         return []
     out = list(dict.fromkeys(lst_of_lst[0]))
     for lst_i in lst_of_lst[1:]:
         out = [name for name in out if name in lst_i]
@@ -148,16 +205,30 @@
     first = it[0]
     if eq_fn is None:
         return all(first == elt for elt in it)
     else:
         return all(eq_fn(first, elt) for elt in it)
 
 
+def all_ne(it: Iterable[T], ne_fn: Optional[Callable[[T, T], bool]] = None) -> bool:
+    """Returns true if all elements in inputs are differents."""
+    it = list(it)
+    if ne_fn is None:
+        return all(
+            it[i] != it[j] for i in range(len(it)) for j in range(i + 1, len(it))
+        )
+    else:
+        return all(
+            ne_fn(it[i], it[j]) for i in range(len(it)) for j in range(i + 1, len(it))
+        )
+
+
 def flat_dict_of_dict(
     nested_dic: Mapping[str, Any],
+    *,
     sep: str = ".",
     flat_iterables: bool = False,
     overwrite: bool = True,
 ) -> Dict[str, Any]:
     """Flat a nested dictionary.
 
     Example 1
@@ -184,43 +255,97 @@
 
     Args:
         nested_dict: Nested mapping containing sub-mappings or iterables.
         sep: Separators between keys.
         flat_iterables: If True, flat iterable and use index as key.
         overwrite: If True, overwrite duplicated keys in output. Otherwise duplicated keys will raises a ValueError.
     """
-    output = {}
-    for k, v in nested_dic.items():
-        if is_mapping_str_any(v):
-            v = flat_dict_of_dict(v, sep, flat_iterables)
-            v = {f"{k}{sep}{kv}": vv for kv, vv in v.items()}
-            output.update(v)
-
-        elif flat_iterables and isinstance(v, Iterable) and not isinstance(v, str):
-            v = {f"{i}": vi for i, vi in enumerate(v)}
-            v = flat_dict_of_dict(v, sep, flat_iterables)
-            v = {f"{k}{sep}{kv}": vv for kv, vv in v.items()}
-            output.update(v)
 
-        elif overwrite or k not in output:
-            output[k] = v
+    def _flat_dict_of_dict_impl(nested_dic: Mapping[str, Any]) -> Dict[str, Any]:
+        output = {}
+        for k, v in nested_dic.items():
+            if is_mapping_str(v):
+                v = _flat_dict_of_dict_impl(v)
+                v = {f"{k}{sep}{kv}": vv for kv, vv in v.items()}
+                output.update(v)
+
+            elif flat_iterables and isinstance(v, Iterable) and not isinstance(v, str):
+                v = {f"{i}": vi for i, vi in enumerate(v)}
+                v = _flat_dict_of_dict_impl(v)
+                v = {f"{k}{sep}{kv}": vv for kv, vv in v.items()}
+                output.update(v)
+
+            elif overwrite or k not in output:
+                output[k] = v
+
+            else:
+                raise ValueError(f"Ambiguous flatten dict with key '{k}'.")
+        return output
+
+    return _flat_dict_of_dict_impl(nested_dic)
 
-        else:
-            raise ValueError(f"Ambiguous flatten dict with key '{k}'.")
 
+def unflat_dict_of_dict(dic: Mapping[str, Any], sep: str = ".") -> Dict[str, Any]:
+    """Unflat a dictionary.
+
+    Example 1
+    ----------
+    ```
+    >>> dic = {
+        "a.a": 1,
+        "b.a": 2,
+        "b.b": 3,
+        "c": 4,
+    }
+    >>> unflat_dict_of_dict(dic)
+    ... {"a": {"a": 1}, "b": {"a": 2, "b": 3}, "c": 4}
+    ```
+    """
+    output = {}
+    for k, v in dic.items():
+        if sep not in k:
+            output[k] = v
+        else:
+            idx = k.index(sep)
+            k, kk = k[:idx], k[idx + 1 :]
+            if k not in output:
+                output[k] = {}
+            elif not isinstance(output[k], Mapping):
+                raise ValueError(
+                    f"Invalid dict argument. (found keys {k} and {k}{sep}{kk})"
+                )
+
+            output[k][kk] = v
+
+    output = {
+        k: (unflat_dict_of_dict(v) if isinstance(v, Mapping) else v)
+        for k, v in output.items()
+    }
     return output
 
 
 def flat_list(lst: Iterable[Sequence[T]]) -> Tuple[List[T], List[int]]:
     """Return a flat version of the input list of sublists with each sublist size."""
     flatten_lst = [element for sublst in lst for element in sublst]
     sizes = [len(sents) for sents in lst]
     return flatten_lst, sizes
 
 
+def unflat_list(flatten_lst: Sequence[T], sizes: Iterable[int]) -> List[List[T]]:
+    """Unflat a list to a list of sublists of given sizes."""
+    lst = []
+    start = 0
+    stop = 0
+    for count in sizes:
+        stop += count
+        lst.append(flatten_lst[start:stop])
+        start = stop
+    return lst
+
+
 @overload
 def unzip(lst: Iterable[Tuple[T]]) -> Tuple[List[T]]:
     ...
 
 
 @overload
 def unzip(lst: Iterable[Tuple[T, U]]) -> Tuple[List[T], List[U]]:
```

### Comparing `torchoutil-0.3.0/src/torchoutil/utils/data/collate.py` & `torchoutil-0.3.1/src/torchoutil/utils/data/collate.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.3.0/src/torchoutil/utils/data/dataloader.py` & `torchoutil-0.3.1/src/torchoutil/utils/data/dataloader.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.3.0/src/torchoutil/utils/data/dataset.py` & `torchoutil-0.3.1/src/torchoutil/utils/data/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
     TypeVar,
     Union,
     runtime_checkable,
 )
 
 from torch.utils.data.dataset import Dataset
 
-T = TypeVar("T", covariant=True)
-U = TypeVar("U", covariant=True)
+T = TypeVar("T", covariant=False)
+U = TypeVar("U", covariant=False)
 
 
 class EmptyDataset(Dataset[None]):
     """Dataset placeholder. Raises StopIteration if __getitem__ is called."""
 
     def __getitem__(self, index) -> None:
         raise StopIteration
@@ -54,13 +54,13 @@
 
     def __len__(self) -> int:
         if isinstance(self._dataset, Sized):
             return len(self._dataset)
         else:
             raise TypeError("Wrapped dataset is not Sized.")
 
-    def unwrap(self) -> Dataset[T]:
+    def unwrap(self) -> SizedDatasetLike[T]:
         return self._dataset
 
     @property
     def transform(self) -> Optional[Callable[[T], U]]:
         return self._transform
```

### Comparing `torchoutil-0.3.0/src/torchoutil/utils/data/split.py` & `torchoutil-0.3.1/src/torchoutil/utils/data/split.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.3.0/src/torchoutil/utils/hdf/dataset.py` & `torchoutil-0.3.1/src/torchoutil/utils/hdf/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,23 +32,24 @@
 from torchoutil.nn.functional.indices import get_inverse_perm
 from torchoutil.utils.collections import all_eq
 from torchoutil.utils.hdf.common import (
     HDF_ENCODING,
     HDF_STRING_DTYPE,
     HDF_VOID_DTYPE,
     SHAPE_SUFFIX,
+    HDFAttributes,
     _dict_to_tuple,
 )
 from torchoutil.utils.type_checks import (
     is_iterable_bytes_list,
     is_iterable_int,
     is_iterable_str,
 )
 
-logger = logging.getLogger(__name__)
+pylog = logging.getLogger(__name__)
 
 
 T = TypeVar("T")
 U = TypeVar("U")
 
 
 IndexType = Union[int, Iterable[int], Tensor, slice, None]
@@ -62,15 +63,15 @@
         or isinstance(index, slice)
         or index is None
         or (isinstance(index, Tensor) and not index.is_floating_point())
     )
 
 
 def _is_column(column: Any) -> TypeGuard[ColumnType]:
-    return isinstance(column, str) or is_iterable_str(column) or column is None
+    return is_iterable_str(column, accept_str=True) or column is None
 
 
 class HDFDataset(Generic[T, U], Dataset[U]):
     def __init__(
         self,
         hdf_fpath: Union[str, Path],
         transform: Optional[Callable[[T], U]] = None,
@@ -131,16 +132,16 @@
 
     @property
     def all_columns(self) -> List[str]:
         """The name of all columns of the dataset."""
         return list(self.get_hdf_keys())
 
     @property
-    def attrs(self) -> Dict[str, Any]:
-        return dict(self._hdf_file.attrs)
+    def attrs(self) -> HDFAttributes:
+        return dict(self._hdf_file.attrs)  # type: ignore
 
     @property
     def metadata(self) -> str:
         return self.attrs.get("metadata", "")
 
     @property
     def column_names(self) -> List[str]:
@@ -227,15 +228,15 @@
         if index is None:
             index = slice(None)
         elif isinstance(index, Tensor):
             index = index.tolist()
         if column is None:
             column = self.column_names
 
-        if is_iterable_str(column):
+        if is_iterable_str(column, accept_str=False):
             return {column_i: self.at(index, column_i) for column_i in column}
 
         if column not in self.all_columns:
             raise ValueError(
                 f"Invalid argument {column=}. (expected one of {tuple(self.all_columns)})"
             )
 
@@ -471,15 +472,15 @@
         if not is_init or (files_are_different and is_open):
             self.open()
 
     # Private methods
     def _sanity_check(self) -> None:
         lens = [dset.shape[0] for dset in self._hdf_file.values()]
         if not all_eq(lens) or lens[0] != len(self):
-            logger.error(
+            pylog.error(
                 f"Incorrect length stored in HDF file. (found {lens=} and {len(self)=})"
             )
 
         if not hasattr(self, "__orig_class__"):
             return None
 
         t_type = self.__orig_class__.__args__[0]  # type: ignore
```

### Comparing `torchoutil-0.3.0/src/torchoutil/utils/hdf/pack.py` & `torchoutil-0.3.1/src/torchoutil/utils/hdf/pack.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from h5py import Dataset as HDFRawDataset
 from torch import Tensor, nn
 from torch.utils.data.dataloader import DataLoader
 
 from torchoutil.nn.functional.numpy import is_numpy_scalar
 from torchoutil.utils.collections import all_eq, unzip
 from torchoutil.utils.data.dataloader import get_auto_num_cpus
-from torchoutil.utils.data.dataset import SizedDatasetLike
+from torchoutil.utils.data.dataset import SizedDatasetLike, TransformWrapper
 from torchoutil.utils.hdf.common import (
     HDF_ENCODING,
     HDF_STRING_DTYPE,
     HDF_VOID_DTYPE,
     SHAPE_SUFFIX,
     _tuple_to_dict,
 )
@@ -93,26 +93,27 @@
     # Check inputs
     if not isinstance(dataset, SizedDatasetLike):
         raise TypeError(
             f"Cannot pack to hdf a non-sized-dataset '{dataset.__class__.__name__}'."
         )
     if len(dataset) == 0:
         raise ValueError("Cannot pack to hdf an empty dataset.")
-    if file_kwargs is None:
-        file_kwargs = {}
 
     hdf_fpath = Path(hdf_fpath).resolve()
     if hdf_fpath.exists() and not hdf_fpath.is_file():
         raise RuntimeError(f"Item {hdf_fpath=} exists but it is not a file.")
 
     if hdf_fpath.is_file() and not overwrite:
         raise ValueError(
             f"Cannot overwrite file {hdf_fpath}. Please remove it or use overwrite=True option."
         )
 
+    if file_kwargs is None:
+        file_kwargs = {}
+
     if num_workers == "auto":
         num_workers = get_auto_num_cpus()
         if verbose >= 2:
             pylog.debug(f"Found num_workers=='auto', set to {num_workers}.")
 
     if pre_transform is None:
         pre_transform = nn.Identity()
@@ -149,31 +150,30 @@
 
     max_shapes: Dict[str, Tuple[int, ...]] = shapes_0
     hdf_dtypes: Dict[str, str] = hdf_dtypes_0
     all_eq_shapes: Dict[str, bool] = {
         attr_name: True for attr_name in item_0_dict.keys()
     }
 
+    wrapped = TransformWrapper(dataset, dict_pre_transform)
     loader = DataLoader(
-        dataset,  # type: ignore
+        wrapped,  # type: ignore
         batch_size=batch_size,
         shuffle=False,
         num_workers=num_workers,
         collate_fn=nn.Identity(),
         drop_last=False,
         pin_memory=False,
     )
 
     for batch in tqdm.tqdm(
         loader,
         desc="Pre compute shapes...",
         disable=verbose <= 0,
     ):
-        batch = [dict_pre_transform(item) for item in batch]
-
         for item in batch:
             for attr_name, value in item.items():
                 shape, hdf_dtype, _src_dtype = _get_shape_and_dtype(value)
                 all_eq_shapes[attr_name] &= max_shapes[attr_name] == shape
                 max_shapes[attr_name] = tuple(
                     map(max, zip(max_shapes[attr_name], shape))
                 )
```

### Comparing `torchoutil-0.3.0/src/torchoutil/utils/packaging.py` & `torchoutil-0.3.1/src/torchoutil/utils/packaging.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,7 +15,9 @@
         # Python >= 3.7
         return False
 
 
 _NUMPY_AVAILABLE = _package_is_available("numpy")
 _TENSORBOARD_AVAILABLE = _package_is_available("tensorboard")
 _H5PY_AVAILABLE = _package_is_available("h5py")
+_OMEGACONF_AVAILABLE = _package_is_available("omegaconf")
+_YAML_AVAILABLE = _package_is_available("yaml")
```

### Comparing `torchoutil-0.3.0/src/torchoutil/utils/return_types.py` & `torchoutil-0.3.1/src/torchoutil/utils/return_types.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.3.0/src/torchoutil/utils/tensorboard.py` & `torchoutil-0.3.1/src/torchoutil/utils/tensorboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         "Optional dependancy 'tensorboard' is not installed. Please install it using 'pip install torchoutil[extras]'"
     )
 
 from tensorboard.backend.event_processing.event_file_loader import (  # type: ignore
     EventFileLoader,
 )
 
-logger = logging.getLogger(__name__)
+pylog = logging.getLogger(__name__)
 
 
 _EVENT_FILE_PREFIX = "events.out.tfevents."
 _DT_FLOAT = 1
 _DT_STRING = 7
 _DTYPES = (_DT_FLOAT, _DT_STRING)
 
@@ -82,15 +82,15 @@
     data = []
     for data_i in raw_data:
         tag: str = data_i["tag"]
         dtype: Any = data_i["dtype"]
 
         if ignore_underscore_tags and tag.startswith("_"):
             if verbose >= 2:
-                logger.debug(
+                pylog.debug(
                     f'Skip value with tag "{tag}" which begins by an underscore.'
                 )
             continue
 
         if dtype == _DT_FLOAT:
             float_val: List[float] = data_i["float_val"]
             dtype = "float"
```

### Comparing `torchoutil-0.3.0/src/torchoutil.egg-info/PKG-INFO` & `torchoutil-0.3.1/src/torchoutil.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 746f 7263  : 2.1.Name: torc
 00000020: 686f 7574 696c 0a56 6572 7369 6f6e 3a20  houtil.Version: 
-00000030: 302e 332e 300a 5375 6d6d 6172 793a 2043  0.3.0.Summary: C
+00000030: 302e 332e 310a 5375 6d6d 6172 793a 2043  0.3.1.Summary: C
 00000040: 6f6c 6c65 6374 696f 6e20 6f66 2066 756e  ollection of fun
 00000050: 6374 696f 6e73 2061 6e64 206d 6f64 756c  ctions and modul
 00000060: 6573 2074 6f20 6865 6c70 2064 6576 656c  es to help devel
 00000070: 6f70 6d65 6e74 2069 6e20 5079 546f 7263  opment in PyTorc
 00000080: 682e 0a41 7574 686f 722d 656d 6169 6c3a  h..Author-email:
 00000090: 2022 c389 7469 656e 6e65 204c 6162 62c3   "..tienne Labb.
 000000a0: a920 284c 6162 6265 7469 2922 203c 6c61  . (Labbeti)" <la
@@ -301,93 +301,166 @@
 000012c0: 203d 2074 6f72 6368 2e61 735f 7465 6e73   = torch.as_tens
 000012d0: 6f72 285b 5b31 2c20 302c 2030 5d2c 205b  or([[1, 0, 0], [
 000012e0: 302c 2031 2c20 315d 2c20 5b30 2c20 302c  0, 1, 1], [0, 0,
 000012f0: 2030 5d5d 290a 696e 6469 6365 7320 3d20   0]]).indices = 
 00001300: 6d75 6c74 6968 6f74 5f74 6f5f 696e 6469  multihot_to_indi
 00001310: 6365 7328 6d75 6c74 6968 6f74 290a 2320  ces(multihot).# 
 00001320: 5b5b 305d 2c20 5b31 2c20 325d 2c20 5b5d  [[0], [1, 2], []
-00001330: 5d0a 6060 600a 0a23 2323 202e 2e2e 616e  ].```..### ...an
-00001340: 6420 6d6f 7265 2074 656e 736f 7220 6d61  d more tensor ma
-00001350: 6e69 7075 6c61 7469 6f6e 7321 0a0a 6060  nipulations!..``
-00001360: 6070 7974 686f 6e0a 696d 706f 7274 2074  `python.import t
-00001370: 6f72 6368 0a66 726f 6d20 746f 7263 686f  orch.from torcho
-00001380: 7574 696c 2069 6d70 6f72 7420 696e 7365  util import inse
-00001390: 7274 5f61 745f 696e 6469 6365 730a 0a78  rt_at_indices..x
-000013a0: 203d 2074 6f72 6368 2e61 735f 7465 6e73   = torch.as_tens
-000013b0: 6f72 285b 312c 2032 2c20 332c 2034 5d29  or([1, 2, 3, 4])
-000013c0: 0a72 6573 756c 7420 3d20 696e 7365 7274  .result = insert
-000013d0: 5f61 745f 696e 6469 6365 7328 782c 2069  _at_indices(x, i
-000013e0: 6e64 6963 6573 3d5b 302c 2032 5d2c 2076  ndices=[0, 2], v
-000013f0: 616c 7565 733d 3529 0a23 2072 6573 756c  alues=5).# resul
-00001400: 7420 636f 6e74 6169 6e73 2074 656e 736f  t contains tenso
-00001410: 7220 7769 7468 2069 6e73 6572 7465 6420  r with inserted 
-00001420: 7661 6c75 6573 3a20 7465 6e73 6f72 285b  values: tensor([
-00001430: 352c 2031 2c20 322c 2035 2c20 332c 2034  5, 1, 2, 5, 3, 4
-00001440: 5d29 0a60 6060 0a0a 6060 6070 7974 686f  ]).```..```pytho
-00001450: 6e0a 696d 706f 7274 2074 6f72 6368 0a66  n.import torch.f
-00001460: 726f 6d20 746f 7263 686f 7574 696c 2069  rom torchoutil i
-00001470: 6d70 6f72 7420 6765 745f 696e 7665 7273  mport get_invers
-00001480: 655f 7065 726d 0a0a 7065 726d 203d 2074  e_perm..perm = t
-00001490: 6f72 6368 2e72 616e 6470 6572 6d28 3130  orch.randperm(10
-000014a0: 290a 696e 765f 7065 726d 203d 2067 6574  ).inv_perm = get
-000014b0: 5f69 6e76 6572 7365 5f70 6572 6d28 7065  _inverse_perm(pe
-000014c0: 726d 290a 0a78 3120 3d20 746f 7263 682e  rm)..x1 = torch.
-000014d0: 7261 6e64 2831 3029 0a78 3220 3d20 7831  rand(10).x2 = x1
-000014e0: 5b70 6572 6d5d 0a78 3320 3d20 7832 5b69  [perm].x3 = x2[i
-000014f0: 6e76 5f70 6572 6d5d 0a23 2069 6e76 5f70  nv_perm].# inv_p
-00001500: 6572 6d20 6172 6520 696e 6469 6365 7320  erm are indices 
-00001510: 7468 6174 2061 6c6c 6f77 2075 7320 746f  that allow us to
-00001520: 2067 6574 2078 3320 6672 6f6d 2078 322c   get x3 from x2,
-00001530: 2069 2e65 2e20 7831 203d 3d20 7833 2068   i.e. x1 == x3 h
-00001540: 6572 650a 6060 600a 0a23 2320 4578 7472  ere.```..## Extr
-00001550: 6173 0a60 746f 7263 686f 7574 696c 6020  as.`torchoutil` 
-00001560: 616c 736f 2070 726f 7669 6465 7320 6164  also provides ad
-00001570: 6469 7469 6f6e 616c 206d 6f64 756c 6573  ditional modules
-00001580: 2077 6865 6e20 736f 6d65 2073 7065 6369   when some speci
-00001590: 6669 6320 7061 636b 6167 6520 6172 6520  fic package are 
-000015a0: 616c 7265 6164 7920 696e 7374 616c 6c65  already installe
-000015b0: 6420 696e 2079 6f75 7220 656e 7669 726f  d in your enviro
-000015c0: 6e6d 656e 742e 0a41 6c6c 2065 7874 7261  nment..All extra
-000015d0: 7320 6361 6e20 6265 2069 6e73 7461 6c6c  s can be install
-000015e0: 6564 2077 6974 6820 6070 6970 2069 6e73  ed with `pip ins
-000015f0: 7461 6c6c 2074 6f72 6368 6f75 7469 6c5b  tall torchoutil[
-00001600: 6578 7472 6173 5d60 0a0a 2d20 4966 2060  extras]`..- If `
-00001610: 7465 6e73 6f72 626f 6172 6460 2069 7320  tensorboard` is 
-00001620: 696e 7374 616c 6c65 642c 2074 6865 2066  installed, the f
-00001630: 756e 6374 696f 6e20 606c 6f61 645f 6576  unction `load_ev
-00001640: 656e 745f 6669 6c65 6020 6361 6e20 6265  ent_file` can be
-00001650: 2075 7365 642e 2049 7420 6973 2075 7365   used. It is use
-00001660: 6675 6c20 746f 206c 6f61 6420 6d61 6e75  ful to load manu
-00001670: 616c 6c79 2061 6c6c 2064 6174 6120 636f  ally all data co
-00001680: 6e74 6169 6e65 6420 696e 2061 6e20 7465  ntained in an te
-00001690: 6e73 6f72 626f 6172 6420 6576 656e 7420  nsorboard event 
-000016a0: 6669 6c65 2e0a 2d20 4966 2060 6e75 6d70  file..- If `nump
-000016b0: 7960 2069 7320 696e 7374 616c 6c65 642c  y` is installed,
-000016c0: 2074 6865 2063 6c61 7373 6573 2060 4672   the classes `Fr
-000016d0: 6f6d 4e75 6d70 7960 2061 6e64 2020 6054  omNumpy` and  `T
-000016e0: 6f4e 756d 7079 6020 6361 6e20 6265 2075  oNumpy` can be u
-000016f0: 7365 6420 616e 6420 7468 6569 7220 7265  sed and their re
-00001700: 6c61 7465 6420 6675 6e63 7469 6f6e 2e20  lated function. 
-00001710: 4974 2069 7320 6d65 616e 7420 746f 2062  It is meant to b
-00001720: 6520 7573 6564 2074 6f20 636f 6d70 6f73  e used to compos
-00001730: 6520 6479 6e61 6d69 6320 7472 616e 7366  e dynamic transf
-00001740: 6f72 6d73 2069 6e74 6f20 6053 6571 7565  orms into `Seque
-00001750: 6e74 6961 6c60 206d 6f64 756c 652e 0a2d  ntial` module..-
-00001760: 2049 6620 6068 3570 7960 2069 7320 696e   If `h5py` is in
-00001770: 7374 616c 6c65 642c 2074 6865 2066 756e  stalled, the fun
-00001780: 6374 696f 6e20 6070 6163 6b5f 746f 5f68  ction `pack_to_h
-00001790: 6466 6020 616e 6420 636c 6173 7320 6048  df` and class `H
-000017a0: 4446 4461 7461 7365 7460 2063 616e 2062  DFDataset` can b
-000017b0: 6520 7573 6564 2e20 4361 6e20 6265 2075  e used. Can be u
-000017c0: 7365 6420 746f 2070 6163 6b2f 7265 6164  sed to pack/read
-000017d0: 2064 6174 6173 6574 2074 6f20 4844 4620   dataset to HDF 
-000017e0: 6669 6c65 732c 2061 6e64 2073 7570 706f  files, and suppo
-000017f0: 7274 7320 7661 7269 6162 6c65 2d6c 656e  rts variable-len
-00001800: 6774 6820 7365 7175 656e 6365 7320 6f66  gth sequences of
-00001810: 2064 6174 612e 0a0a 0a23 2320 436f 6e74   data....## Cont
-00001820: 6163 740a 4d61 696e 7461 696e 6572 3a0a  act.Maintainer:.
-00001830: 2d20 5bc3 8974 6965 6e6e 6520 4c61 6262  - [..tienne Labb
-00001840: c3a9 5d28 6874 7470 733a 2f2f 6c61 6262  ..](https://labb
-00001850: 6574 692e 6769 7468 7562 2e69 6f2f 2920  eti.github.io/) 
-00001860: 224c 6162 6265 7469 223a 206c 6162 6265  "Labbeti": labbe
-00001870: 7469 2e70 7562 4067 6d61 696c 2e63 6f6d  ti.pub@gmail.com
-00001880: 0a                                       .
+00001330: 5d0a 6060 600a 0a23 2323 2045 6173 656c  ].```..### Easel
+00001340: 7920 7072 652d 636f 6d70 7574 6520 7472  y pre-compute tr
+00001350: 616e 7366 6f72 6d73 0a0a 4865 7265 2069  ansforms..Here i
+00001360: 7320 616e 2065 7861 6d70 6c65 206f 6620  s an example of 
+00001370: 7072 652d 636f 6d70 7574 696e 6720 7370  pre-computing sp
+00001380: 6563 7472 6f67 7261 6d73 206f 6620 746f  ectrograms of to
+00001390: 7263 6861 7564 696f 2060 5350 4545 4348  rchaudio `SPEECH
+000013a0: 434f 4d4d 414e 4453 6020 6461 7461 7365  COMMANDS` datase
+000013b0: 742c 2075 7369 6e67 2060 7061 636b 5f74  t, using `pack_t
+000013c0: 6f5f 7069 636b 6c65 6020 6675 6e63 7469  o_pickle` functi
+000013d0: 6f6e 3a0a 0a60 6060 7079 7468 6f6e 0a66  on:..```python.f
+000013e0: 726f 6d20 746f 7263 6820 696d 706f 7274  rom torch import
+000013f0: 206e 6e0a 6672 6f6d 2074 6f72 6368 6175   nn.from torchau
+00001400: 6469 6f2e 6461 7461 7365 7473 2069 6d70  dio.datasets imp
+00001410: 6f72 7420 5350 4545 4348 434f 4d4d 414e  ort SPEECHCOMMAN
+00001420: 4453 0a66 726f 6d20 746f 7263 6861 7564  DS.from torchaud
+00001430: 696f 2e74 7261 6e73 666f 726d 7320 696d  io.transforms im
+00001440: 706f 7274 2053 7065 6374 726f 6772 616d  port Spectrogram
+00001450: 0a66 726f 6d20 746f 7263 686f 7574 696c  .from torchoutil
+00001460: 2e75 7469 6c73 2e70 6963 6b6c 655f 6461  .utils.pickle_da
+00001470: 7461 7365 7420 696d 706f 7274 2070 6163  taset import pac
+00001480: 6b5f 746f 5f70 6963 6b6c 650a 0a73 7065  k_to_pickle..spe
+00001490: 6563 685f 636f 6d6d 616e 6473 5f72 6f6f  ech_commands_roo
+000014a0: 7420 3d20 2270 6174 682f 746f 2f73 7065  t = "path/to/spe
+000014b0: 6563 685f 636f 6d6d 616e 6473 220a 7069  ech_commands".pi
+000014c0: 636b 6c65 5f72 6f6f 7420 3d20 2270 6174  ckle_root = "pat
+000014d0: 682f 746f 2f70 6963 6b6c 655f 6461 7461  h/to/pickle_data
+000014e0: 7365 7422 0a0a 6461 7461 7365 7420 3d20  set"..dataset = 
+000014f0: 5350 4545 4348 434f 4d4d 414e 4453 2873  SPEECHCOMMANDS(s
+00001500: 7065 6563 685f 636f 6d6d 616e 6473 5f72  peech_commands_r
+00001510: 6f6f 742c 2064 6f77 6e6c 6f61 643d 5472  oot, download=Tr
+00001520: 7565 2c20 7375 6273 6574 3d22 7661 6c69  ue, subset="vali
+00001530: 6461 7469 6f6e 2229 0a0a 636c 6173 7320  dation")..class 
+00001540: 4d79 5472 616e 7366 6f72 6d28 6e6e 2e4d  MyTransform(nn.M
+00001550: 6f64 756c 6529 3a0a 2020 2020 6465 6620  odule):.    def 
+00001560: 5f5f 696e 6974 5f5f 2873 656c 6629 202d  __init__(self) -
+00001570: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00001580: 7375 7065 7228 292e 5f5f 696e 6974 5f5f  super().__init__
+00001590: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+000015a0: 7370 6563 7472 6f67 7261 6d5f 6578 7472  spectrogram_extr
+000015b0: 6163 746f 7220 3d20 5370 6563 7472 6f67  actor = Spectrog
+000015c0: 7261 6d28 290a 0a20 2020 2064 6566 2066  ram()..    def f
+000015d0: 6f72 7761 7264 2873 656c 662c 2069 7465  orward(self, ite
+000015e0: 6d29 3a0a 2020 2020 2020 2020 7761 7665  m):.        wave
+000015f0: 666f 726d 203d 2069 7465 6d5b 305d 0a20  form = item[0]. 
+00001600: 2020 2020 2020 2073 7065 6374 726f 6772         spectrogr
+00001610: 616d 203d 2073 656c 662e 7370 6563 7472  am = self.spectr
+00001620: 6f67 7261 6d5f 6578 7472 6163 746f 7228  ogram_extractor(
+00001630: 7761 7665 666f 726d 290a 2020 2020 2020  waveform).      
+00001640: 2020 7265 7475 726e 2028 7370 6563 7472    return (spectr
+00001650: 6f67 7261 6d2c 2920 2b20 6974 656d 5b31  ogram,) + item[1
+00001660: 3a5d 0a0a 7061 636b 5f74 6f5f 7069 636b  :]..pack_to_pick
+00001670: 6c65 2864 6174 6173 6574 2c20 7069 636b  le(dataset, pick
+00001680: 6c65 5f72 6f6f 742c 204d 7954 7261 6e73  le_root, MyTrans
+00001690: 666f 726d 2829 290a 6060 600a 0a54 6865  form()).```..The
+000016a0: 6e20 796f 7520 6361 6e20 6c6f 6164 2074  n you can load t
+000016b0: 6865 2070 7265 2d63 6f6d 7075 7465 6420  he pre-computed 
+000016c0: 6461 7461 7365 7420 7573 696e 6720 6050  dataset using `P
+000016d0: 6963 6b6c 6544 6174 6173 6574 603a 0a60  ickleDataset`:.`
+000016e0: 6060 7079 7468 6f6e 0a66 726f 6d20 746f  ``python.from to
+000016f0: 7263 686f 7574 696c 2e75 7469 6c73 2e70  rchoutil.utils.p
+00001700: 6963 6b6c 655f 6461 7461 7365 7420 696d  ickle_dataset im
+00001710: 706f 7274 2050 6963 6b6c 6544 6174 6173  port PickleDatas
+00001720: 6574 0a0a 7069 636b 6c65 5f72 6f6f 7420  et..pickle_root 
+00001730: 3d20 2270 6174 682f 746f 2f70 6963 6b6c  = "path/to/pickl
+00001740: 655f 6461 7461 7365 7422 0a70 6963 6b6c  e_dataset".pickl
+00001750: 655f 6461 7461 7365 7420 3d20 5069 636b  e_dataset = Pick
+00001760: 6c65 4461 7461 7365 7428 7069 636b 6c65  leDataset(pickle
+00001770: 5f72 6f6f 7429 0a70 6963 6b6c 655f 6461  _root).pickle_da
+00001780: 7461 7365 745b 305d 2020 2320 3d3d 2066  taset[0]  # == f
+00001790: 6972 7374 2074 7261 6e73 666f 726d 6564  irst transformed
+000017a0: 2069 7465 6d2c 2069 2e65 2e20 7472 616e   item, i.e. tran
+000017b0: 7366 6f72 6d28 6461 7461 7365 745b 305d  sform(dataset[0]
+000017c0: 290a 6060 600a 0a23 2323 202e 2e2e 616e  ).```..### ...an
+000017d0: 6420 6d6f 7265 2074 656e 736f 7220 6d61  d more tensor ma
+000017e0: 6e69 7075 6c61 7469 6f6e 7321 0a0a 6060  nipulations!..``
+000017f0: 6070 7974 686f 6e0a 696d 706f 7274 2074  `python.import t
+00001800: 6f72 6368 0a66 726f 6d20 746f 7263 686f  orch.from torcho
+00001810: 7574 696c 2069 6d70 6f72 7420 696e 7365  util import inse
+00001820: 7274 5f61 745f 696e 6469 6365 730a 0a78  rt_at_indices..x
+00001830: 203d 2074 6f72 6368 2e61 735f 7465 6e73   = torch.as_tens
+00001840: 6f72 285b 312c 2032 2c20 332c 2034 5d29  or([1, 2, 3, 4])
+00001850: 0a72 6573 756c 7420 3d20 696e 7365 7274  .result = insert
+00001860: 5f61 745f 696e 6469 6365 7328 782c 2069  _at_indices(x, i
+00001870: 6e64 6963 6573 3d5b 302c 2032 5d2c 2076  ndices=[0, 2], v
+00001880: 616c 7565 733d 3529 0a23 2072 6573 756c  alues=5).# resul
+00001890: 7420 636f 6e74 6169 6e73 2074 656e 736f  t contains tenso
+000018a0: 7220 7769 7468 2069 6e73 6572 7465 6420  r with inserted 
+000018b0: 7661 6c75 6573 3a20 7465 6e73 6f72 285b  values: tensor([
+000018c0: 352c 2031 2c20 322c 2035 2c20 332c 2034  5, 1, 2, 5, 3, 4
+000018d0: 5d29 0a60 6060 0a0a 6060 6070 7974 686f  ]).```..```pytho
+000018e0: 6e0a 696d 706f 7274 2074 6f72 6368 0a66  n.import torch.f
+000018f0: 726f 6d20 746f 7263 686f 7574 696c 2069  rom torchoutil i
+00001900: 6d70 6f72 7420 6765 745f 696e 7665 7273  mport get_invers
+00001910: 655f 7065 726d 0a0a 7065 726d 203d 2074  e_perm..perm = t
+00001920: 6f72 6368 2e72 616e 6470 6572 6d28 3130  orch.randperm(10
+00001930: 290a 696e 765f 7065 726d 203d 2067 6574  ).inv_perm = get
+00001940: 5f69 6e76 6572 7365 5f70 6572 6d28 7065  _inverse_perm(pe
+00001950: 726d 290a 0a78 3120 3d20 746f 7263 682e  rm)..x1 = torch.
+00001960: 7261 6e64 2831 3029 0a78 3220 3d20 7831  rand(10).x2 = x1
+00001970: 5b70 6572 6d5d 0a78 3320 3d20 7832 5b69  [perm].x3 = x2[i
+00001980: 6e76 5f70 6572 6d5d 0a23 2069 6e76 5f70  nv_perm].# inv_p
+00001990: 6572 6d20 6172 6520 696e 6469 6365 7320  erm are indices 
+000019a0: 7468 6174 2061 6c6c 6f77 2075 7320 746f  that allow us to
+000019b0: 2067 6574 2078 3320 6672 6f6d 2078 322c   get x3 from x2,
+000019c0: 2069 2e65 2e20 7831 203d 3d20 7833 2068   i.e. x1 == x3 h
+000019d0: 6572 650a 6060 600a 0a23 2320 4578 7472  ere.```..## Extr
+000019e0: 6173 0a60 746f 7263 686f 7574 696c 6020  as.`torchoutil` 
+000019f0: 616c 736f 2070 726f 7669 6465 7320 6164  also provides ad
+00001a00: 6469 7469 6f6e 616c 206d 6f64 756c 6573  ditional modules
+00001a10: 2077 6865 6e20 736f 6d65 2073 7065 6369   when some speci
+00001a20: 6669 6320 7061 636b 6167 6520 6172 6520  fic package are 
+00001a30: 616c 7265 6164 7920 696e 7374 616c 6c65  already installe
+00001a40: 6420 696e 2079 6f75 7220 656e 7669 726f  d in your enviro
+00001a50: 6e6d 656e 742e 0a41 6c6c 2065 7874 7261  nment..All extra
+00001a60: 7320 6361 6e20 6265 2069 6e73 7461 6c6c  s can be install
+00001a70: 6564 2077 6974 6820 6070 6970 2069 6e73  ed with `pip ins
+00001a80: 7461 6c6c 2074 6f72 6368 6f75 7469 6c5b  tall torchoutil[
+00001a90: 6578 7472 6173 5d60 0a0a 2d20 4966 2060  extras]`..- If `
+00001aa0: 7465 6e73 6f72 626f 6172 6460 2069 7320  tensorboard` is 
+00001ab0: 696e 7374 616c 6c65 642c 2074 6865 2066  installed, the f
+00001ac0: 756e 6374 696f 6e20 606c 6f61 645f 6576  unction `load_ev
+00001ad0: 656e 745f 6669 6c65 6020 6361 6e20 6265  ent_file` can be
+00001ae0: 2075 7365 642e 2049 7420 6973 2075 7365   used. It is use
+00001af0: 6675 6c20 746f 206c 6f61 6420 6d61 6e75  ful to load manu
+00001b00: 616c 6c79 2061 6c6c 2064 6174 6120 636f  ally all data co
+00001b10: 6e74 6169 6e65 6420 696e 2061 6e20 7465  ntained in an te
+00001b20: 6e73 6f72 626f 6172 6420 6576 656e 7420  nsorboard event 
+00001b30: 6669 6c65 2e0a 2d20 4966 2060 6e75 6d70  file..- If `nump
+00001b40: 7960 2069 7320 696e 7374 616c 6c65 642c  y` is installed,
+00001b50: 2074 6865 2063 6c61 7373 6573 2060 4672   the classes `Fr
+00001b60: 6f6d 4e75 6d70 7960 2061 6e64 2020 6054  omNumpy` and  `T
+00001b70: 6f4e 756d 7079 6020 6361 6e20 6265 2075  oNumpy` can be u
+00001b80: 7365 6420 616e 6420 7468 6569 7220 7265  sed and their re
+00001b90: 6c61 7465 6420 6675 6e63 7469 6f6e 2e20  lated function. 
+00001ba0: 4974 2069 7320 6d65 616e 7420 746f 2062  It is meant to b
+00001bb0: 6520 7573 6564 2074 6f20 636f 6d70 6f73  e used to compos
+00001bc0: 6520 6479 6e61 6d69 6320 7472 616e 7366  e dynamic transf
+00001bd0: 6f72 6d73 2069 6e74 6f20 6053 6571 7565  orms into `Seque
+00001be0: 6e74 6961 6c60 206d 6f64 756c 652e 0a2d  ntial` module..-
+00001bf0: 2049 6620 6068 3570 7960 2069 7320 696e   If `h5py` is in
+00001c00: 7374 616c 6c65 642c 2074 6865 2066 756e  stalled, the fun
+00001c10: 6374 696f 6e20 6070 6163 6b5f 746f 5f68  ction `pack_to_h
+00001c20: 6466 6020 616e 6420 636c 6173 7320 6048  df` and class `H
+00001c30: 4446 4461 7461 7365 7460 2063 616e 2062  DFDataset` can b
+00001c40: 6520 7573 6564 2e20 4361 6e20 6265 2075  e used. Can be u
+00001c50: 7365 6420 746f 2070 6163 6b2f 7265 6164  sed to pack/read
+00001c60: 2064 6174 6173 6574 2074 6f20 4844 4620   dataset to HDF 
+00001c70: 6669 6c65 732c 2061 6e64 2073 7570 706f  files, and suppo
+00001c80: 7274 7320 7661 7269 6162 6c65 2d6c 656e  rts variable-len
+00001c90: 6774 6820 7365 7175 656e 6365 7320 6f66  gth sequences of
+00001ca0: 2064 6174 612e 0a0a 0a23 2320 436f 6e74   data....## Cont
+00001cb0: 6163 740a 4d61 696e 7461 696e 6572 3a0a  act.Maintainer:.
+00001cc0: 2d20 5bc3 8974 6965 6e6e 6520 4c61 6262  - [..tienne Labb
+00001cd0: c3a9 5d28 6874 7470 733a 2f2f 6c61 6262  ..](https://labb
+00001ce0: 6574 692e 6769 7468 7562 2e69 6f2f 2920  eti.github.io/) 
+00001cf0: 224c 6162 6265 7469 223a 206c 6162 6265  "Labbeti": labbe
+00001d00: 7469 2e70 7562 4067 6d61 696c 2e63 6f6d  ti.pub@gmail.com
+00001d10: 0a                                       .
```

### Comparing `torchoutil-0.3.0/src/torchoutil.egg-info/SOURCES.txt` & `torchoutil-0.3.1/src/torchoutil.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -25,50 +25,62 @@
 src/torchoutil/nn/functional/indices.py
 src/torchoutil/nn/functional/mask.py
 src/torchoutil/nn/functional/multiclass.py
 src/torchoutil/nn/functional/multilabel.py
 src/torchoutil/nn/functional/numpy.py
 src/torchoutil/nn/functional/others.py
 src/torchoutil/nn/functional/pad.py
-src/torchoutil/nn/functional/repeat.py
+src/torchoutil/nn/functional/transform.py
 src/torchoutil/nn/modules/__init__.py
 src/torchoutil/nn/modules/activation.py
 src/torchoutil/nn/modules/crop.py
 src/torchoutil/nn/modules/layer.py
 src/torchoutil/nn/modules/mask.py
 src/torchoutil/nn/modules/multiclass.py
 src/torchoutil/nn/modules/multilabel.py
 src/torchoutil/nn/modules/numpy.py
 src/torchoutil/nn/modules/pad.py
-src/torchoutil/nn/modules/repeat.py
 src/torchoutil/nn/modules/tensor.py
+src/torchoutil/nn/modules/transform.py
 src/torchoutil/nn/modules/typed.py
 src/torchoutil/optim/__init__.py
 src/torchoutil/optim/utils.py
 src/torchoutil/utils/__init__.py
 src/torchoutil/utils/collections.py
+src/torchoutil/utils/log_utils.py
 src/torchoutil/utils/packaging.py
 src/torchoutil/utils/return_types.py
 src/torchoutil/utils/tensorboard.py
 src/torchoutil/utils/type_checks.py
 src/torchoutil/utils/data/__init__.py
 src/torchoutil/utils/data/collate.py
 src/torchoutil/utils/data/dataloader.py
 src/torchoutil/utils/data/dataset.py
 src/torchoutil/utils/data/split.py
 src/torchoutil/utils/hdf/__init__.py
 src/torchoutil/utils/hdf/common.py
 src/torchoutil/utils/hdf/dataset.py
 src/torchoutil/utils/hdf/pack.py
+src/torchoutil/utils/pickle_dataset/__init__.py
+src/torchoutil/utils/pickle_dataset/common.py
+src/torchoutil/utils/pickle_dataset/dataset.py
+src/torchoutil/utils/pickle_dataset/pack.py
+src/torchoutil/utils/saving/__init__.py
+src/torchoutil/utils/saving/common.py
+src/torchoutil/utils/saving/csv_io.py
+src/torchoutil/utils/saving/yaml_io.py
 tests/test_hub.py
 tests/test_nn_functional_crop.py
 tests/test_nn_functional_indices.py
 tests/test_nn_functional_mask.py
+tests/test_nn_functional_multiclass.py
 tests/test_nn_functional_multilabel.py
 tests/test_nn_functional_others.py
 tests/test_nn_functional_pad.py
-tests/test_nn_functional_repeat.py
+tests/test_nn_functional_transform.py
+tests/test_nn_modules.py
 tests/test_nn_modules_multilabel.py
 tests/test_readme.py
-tests/test_utils_ckpt.py
 tests/test_utils_collections.py
-tests/test_utils_hdf.py
+tests/test_utils_hdf.py
+tests/test_utils_pickle.py
+tests/test_utils_type_checks.py
```

### Comparing `torchoutil-0.3.0/tests/test_hub.py` & `torchoutil-0.3.1/tests/test_hub.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from unittest import TestCase
 
 from torch import Tensor
 
 from torchoutil.hub.registry import RegistryHub
 
 
-class TestRegister(TestCase):
+class TestRegistryHub(TestCase):
     def test_cnext_register(self) -> None:
         register = RegistryHub(
             infos={
                 "cnext_bl_70": {
                     "architecture": "ConvNeXt",
                     "url": "https://zenodo.org/record/8020843/files/convnext_tiny_465mAP_BL_AC_70kit.pth?download=1",
                     "hash_value": "0688ae503f5893be0b6b71cb92f8b428",
@@ -21,15 +21,15 @@
                     "fname": "convnext_tiny_465mAP_BL_AC_70kit.pth",
                     "state_dict_key": "model",
                 },
             },
         )
 
         model_name = "cnext_bl_70"
-        register.download_file(model_name, force=True)
+        register.download_file(model_name, force=False)
         state_dict = register.load_state_dict(model_name, offline=True, device="cpu")
 
         assert isinstance(state_dict, dict)
         assert all(isinstance(k, str) for k in state_dict.keys())
         assert all(isinstance(v, Tensor) for v in state_dict.values())
```

### Comparing `torchoutil-0.3.0/tests/test_nn_functional_indices.py` & `torchoutil-0.3.1/tests/test_nn_functional_indices.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.3.0/tests/test_nn_functional_mask.py` & `torchoutil-0.3.1/tests/test_nn_functional_mask.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.3.0/tests/test_nn_functional_multilabel.py` & `torchoutil-0.3.1/tests/test_nn_functional_multilabel.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.3.0/tests/test_nn_functional_pad.py` & `torchoutil-0.3.1/tests/test_nn_functional_pad.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.3.0/tests/test_nn_modules_multilabel.py` & `torchoutil-0.3.1/tests/test_nn_modules_multilabel.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     NamesToIndices,
     NamesToMultihot,
 )
 from torchoutil.nn.modules.typed import TSequential
 
 
 class TestMultilabel(TestCase):
-    def test_modules(self) -> None:
+    def test_example_1(self) -> None:
         num_samples = int(torch.randint(0, 20, ()).item())
         num_classes = int(torch.randint(1, 20, ()).item())
         threshold = torch.rand(())
         idx_to_name = dict(zip(range(num_classes), map(str, range(num_classes))))
 
         multihot = torch.rand(num_samples, num_classes).ge(threshold)
```

### Comparing `torchoutil-0.3.0/tests/test_readme.py` & `torchoutil-0.3.1/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.3.0/tests/test_utils_collections.py` & `torchoutil-0.3.1/tests/test_utils_collections.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
+import random
 import unittest
 from unittest import TestCase
 
 from torchoutil.utils.collections import (
     flat_dict_of_dict,
+    flat_list,
     intersect_lists,
     list_dict_to_dict_list,
+    unflat_dict_of_dict,
+    unflat_list,
 )
+from torchoutil.utils.type_checks import is_list_list_str, is_list_str
 
 
-class TestCollections(TestCase):
+class TestFlatDict(TestCase):
     def test_example_1(self) -> None:
         x = {
             "a": 1,
             "b": {
                 "a": 2,
                 "b": 10,
             },
@@ -39,14 +44,26 @@
         output = flat_dict_of_dict(x)
         assert output == expected
 
     def test_example_4(self) -> None:
         x = {"a": {"b": 1}, "a.b": 2}
         self.assertRaises(ValueError, flat_dict_of_dict, x, overwrite=False)
 
+    def test_unflat_dict_example_1(self) -> None:
+        x = {
+            "a.a": 1,
+            "b.a": 2,
+            "b.b": 3,
+            "c": 4,
+        }
+        y = {"a": {"a": 1}, "b": {"a": 2, "b": 3}, "c": 4}
+
+        y_hat = unflat_dict_of_dict(x)
+        self.assertEqual(y_hat, y)
+
 
 class TestListDictToDictList(TestCase):
     def test_example_1(self) -> None:
         lst = [{"a": 1, "b": 2}, {"a": 4, "b": 3, "c": 5}]
         output = list_dict_to_dict_list(lst, default_val=0)
         self.assertDictEqual(output, {"a": [1, 4], "b": [2, 3], "c": [0, 5]})
 
@@ -75,9 +92,34 @@
         input_ = [["a", "b", "b", "c"], ["c", "d", "b", "a"], ["b", "a", "a", "e"]]
         expected = ["a", "b"]
 
         output = intersect_lists(input_)
         self.assertListEqual(output, expected)
 
 
+class TestFlatList(TestCase):
+    def test_example_1(self) -> None:
+        lst = [
+            list(map(str, range(random.randint(0, 100))))
+            for _ in range(random.randint(0, 10))
+        ]
+        for sublst in lst:
+            random.shuffle(sublst)
+        random.shuffle(lst)
+
+        self.assertTrue(is_list_list_str(lst))
+
+        flatten, sizes = flat_list(lst)
+
+        self.assertTrue(is_list_str(flatten))
+        self.assertEqual(len(lst), len(sizes))
+        self.assertEqual(len(flatten), sum(sizes))
+
+        unflat = unflat_list(flatten, sizes)
+
+        self.assertTrue(is_list_list_str(unflat))
+        self.assertEqual(len(lst), len(unflat))
+        self.assertListEqual(lst, unflat)
+
+
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `torchoutil-0.3.0/tests/test_utils_hdf.py` & `torchoutil-0.3.1/tests/test_utils_hdf.py`

 * *Files identical despite different names*

