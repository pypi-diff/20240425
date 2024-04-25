# Comparing `tmp/helios_ml-0.1.2.tar.gz` & `tmp/helios_ml-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helios_ml-0.1.2.tar", last modified: Tue Apr 16 22:36:29 2024, max compression
+gzip compressed data, was "helios_ml-0.1.3.tar", last modified: Thu Apr 25 01:43:45 2024, max compression
```

## Comparing `helios_ml-0.1.2.tar` & `helios_ml-0.1.3.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:29.603686 helios_ml-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:29.587686 helios_ml-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:29.591686 helios_ml-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-16 22:34:50.000000 helios_ml-0.1.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-16 22:34:50.000000 helios_ml-0.1.2/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-16 22:34:50.000000 helios_ml-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-16 22:34:50.000000 helios_ml-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-16 22:34:50.000000 helios_ml-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-04-16 22:36:29.603686 helios_ml-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-04-16 22:34:50.000000 helios_ml-0.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:29.587686 helios_ml-0.1.2/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:29.591686 helios_ml-0.1.2/data/logo/
--rw-r--r--   0 runner    (1001) docker     (127)    20058 2024-04-16 22:34:50.000000 helios_ml-0.1.2/data/logo/logo-background.png
--rw-r--r--   0 runner    (1001) docker     (127)    14627 2024-04-16 22:34:50.000000 helios_ml-0.1.2/data/logo/logo-transparent.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:29.587686 helios_ml-0.1.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:29.591686 helios_ml-0.1.2/examples/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)    11404 2024-04-16 22:34:50.000000 helios_ml-0.1.2/examples/cifar10/cifar10.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-16 22:34:50.000000 helios_ml-0.1.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:29.595686 helios_ml-0.1.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-16 22:34:50.000000 helios_ml-0.1.2/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-16 22:34:50.000000 helios_ml-0.1.2/requirements/default.txt
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-16 22:34:50.000000 helios_ml-0.1.2/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 22:36:29.603686 helios_ml-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:29.591686 helios_ml-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:29.595686 helios_ml-0.1.2/src/helios/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-16 22:34:50.000000 helios_ml-0.1.2/src/helios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-16 22:34:50.000000 helios_ml-0.1.2/src/helios/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:29.595686 helios_ml-0.1.2/src/helios/core/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-16 22:34:50.000000 helios_ml-0.1.2/src/helios/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-16 22:34:50.000000 helios_ml-0.1.2/src/helios/core/cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-04-16 22:34:50.000000 helios_ml-0.1.2/src/helios/core/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)    17255 2024-04-16 22:34:50.000000 helios_ml-0.1.2/src/helios/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-04-16 22:34:50.000000 helios_ml-0.1.2/src/helios/core/rng.py
--rw-r--r--   0 runner    (1001) docker     (127)    13539 2024-04-16 22:34:50.000000 helios_ml-0.1.2/src/helios/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:29.595686 helios_ml-0.1.2/src/helios/data/
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-16 22:34:50.000000 helios_ml-0.1.2/src/helios/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12644 2024-04-16 22:34:50.000000 helios_ml-0.1.2/src/helios/data/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-04-16 22:34:50.000000 helios_ml-0.1.2/src/helios/data/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     7733 2024-04-16 22:34:50.000000 helios_ml-0.1.2/src/helios/data/samplers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-16 22:34:50.000000 helios_ml-0.1.2/src/helios/data/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:29.595686 helios_ml-0.1.2/src/helios/losses/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-16 22:34:50.000000 helios_ml-0.1.2/src/helios/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-16 22:34:50.000000 helios_ml-0.1.2/src/helios/losses/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-16 22:34:50.000000 helios_ml-0.1.2/src/helios/losses/weighted_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:29.595686 helios_ml-0.1.2/src/helios/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-16 22:34:50.000000 helios_ml-0.1.2/src/helios/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13882 2024-04-16 22:34:50.000000 helios_ml-0.1.2/src/helios/metrics/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-04-16 22:34:50.000000 helios_ml-0.1.2/src/helios/metrics/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:29.599686 helios_ml-0.1.2/src/helios/model/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-16 22:34:50.000000 helios_ml-0.1.2/src/helios/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12625 2024-04-16 22:34:50.000000 helios_ml-0.1.2/src/helios/model/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-16 22:34:50.000000 helios_ml-0.1.2/src/helios/model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:29.599686 helios_ml-0.1.2/src/helios/nn/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-16 22:34:50.000000 helios_ml-0.1.2/src/helios/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-16 22:34:50.000000 helios_ml-0.1.2/src/helios/nn/swa_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-16 22:34:50.000000 helios_ml-0.1.2/src/helios/nn/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-16 22:34:50.000000 helios_ml-0.1.2/src/helios/onnx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:29.599686 helios_ml-0.1.2/src/helios/optim/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-16 22:34:50.000000 helios_ml-0.1.2/src/helios/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-16 22:34:50.000000 helios_ml-0.1.2/src/helios/optim/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:34:50.000000 helios_ml-0.1.2/src/helios/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:29.599686 helios_ml-0.1.2/src/helios/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-16 22:34:50.000000 helios_ml-0.1.2/src/helios/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-16 22:34:50.000000 helios_ml-0.1.2/src/helios/scheduler/schedulers.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-16 22:34:50.000000 helios_ml-0.1.2/src/helios/scheduler/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    35406 2024-04-16 22:34:50.000000 helios_ml-0.1.2/src/helios/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:29.603686 helios_ml-0.1.2/src/helios_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-04-16 22:36:29.000000 helios_ml-0.1.2/src/helios_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-16 22:36:29.000000 helios_ml-0.1.2/src/helios_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 22:36:29.000000 helios_ml-0.1.2/src/helios_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-16 22:36:29.000000 helios_ml-0.1.2/src/helios_ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 22:36:29.000000 helios_ml-0.1.2/src/helios_ml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:29.603686 helios_ml-0.1.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:34:50.000000 helios_ml-0.1.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-16 22:34:50.000000 helios_ml-0.1.2/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:29.603686 helios_ml-0.1.2/test/registry_test/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-16 22:34:50.000000 helios_ml-0.1.2/test/registry_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-16 22:34:50.000000 helios_ml-0.1.2/test/registry_test/extra.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-16 22:34:50.000000 helios_ml-0.1.2/test/registry_test/foo.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-16 22:34:50.000000 helios_ml-0.1.2/test/registry_test/func_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:29.603686 helios_ml-0.1.2/test/registry_test/nested/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:34:50.000000 helios_ml-0.1.2/test/registry_test/nested/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-16 22:34:50.000000 helios_ml-0.1.2/test/registry_test/nested/bar.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-16 22:34:50.000000 helios_ml-0.1.2/test/registry_test/nested/extra.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:34:50.000000 helios_ml-0.1.2/test/registry_test/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-04-16 22:34:50.000000 helios_ml-0.1.2/test/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-04-16 22:34:50.000000 helios_ml-0.1.2/test/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-16 22:34:50.000000 helios_ml-0.1.2/test/test_losses.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-16 22:34:50.000000 helios_ml-0.1.2/test/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-16 22:34:50.000000 helios_ml-0.1.2/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-16 22:34:50.000000 helios_ml-0.1.2/test/test_nn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-16 22:34:50.000000 helios_ml-0.1.2/test/test_onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-16 22:34:50.000000 helios_ml-0.1.2/test/test_optim.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-16 22:34:50.000000 helios_ml-0.1.2/test/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-04-16 22:34:50.000000 helios_ml-0.1.2/test/test_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:29.603686 helios_ml-0.1.2/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-16 22:34:50.000000 helios_ml-0.1.2/tools/generate_requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:43:45.142274 helios_ml-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:43:45.126274 helios_ml-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:43:45.130274 helios_ml-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-25 01:43:09.000000 helios_ml-0.1.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-25 01:43:09.000000 helios_ml-0.1.3/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-25 01:43:09.000000 helios_ml-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-25 01:43:09.000000 helios_ml-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-25 01:43:09.000000 helios_ml-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-04-25 01:43:45.142274 helios_ml-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-04-25 01:43:09.000000 helios_ml-0.1.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:43:45.126274 helios_ml-0.1.3/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:43:45.130274 helios_ml-0.1.3/data/logo/
+-rw-r--r--   0 runner    (1001) docker     (127)    20058 2024-04-25 01:43:09.000000 helios_ml-0.1.3/data/logo/logo-background.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14627 2024-04-25 01:43:09.000000 helios_ml-0.1.3/data/logo/logo-transparent.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:43:45.126274 helios_ml-0.1.3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:43:45.130274 helios_ml-0.1.3/examples/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)    11404 2024-04-25 01:43:09.000000 helios_ml-0.1.3/examples/cifar10/cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-25 01:43:09.000000 helios_ml-0.1.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:43:45.130274 helios_ml-0.1.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-25 01:43:09.000000 helios_ml-0.1.3/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-25 01:43:09.000000 helios_ml-0.1.3/requirements/default.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-25 01:43:09.000000 helios_ml-0.1.3/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 01:43:45.142274 helios_ml-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:43:45.126274 helios_ml-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:43:45.130274 helios_ml-0.1.3/src/helios/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-25 01:43:09.000000 helios_ml-0.1.3/src/helios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-25 01:43:09.000000 helios_ml-0.1.3/src/helios/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:43:45.130274 helios_ml-0.1.3/src/helios/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-25 01:43:09.000000 helios_ml-0.1.3/src/helios/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-25 01:43:09.000000 helios_ml-0.1.3/src/helios/core/cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-04-25 01:43:09.000000 helios_ml-0.1.3/src/helios/core/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17255 2024-04-25 01:43:09.000000 helios_ml-0.1.3/src/helios/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-04-25 01:43:09.000000 helios_ml-0.1.3/src/helios/core/rng.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13539 2024-04-25 01:43:09.000000 helios_ml-0.1.3/src/helios/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:43:45.134274 helios_ml-0.1.3/src/helios/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-25 01:43:09.000000 helios_ml-0.1.3/src/helios/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12644 2024-04-25 01:43:09.000000 helios_ml-0.1.3/src/helios/data/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-04-25 01:43:09.000000 helios_ml-0.1.3/src/helios/data/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7733 2024-04-25 01:43:09.000000 helios_ml-0.1.3/src/helios/data/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-25 01:43:09.000000 helios_ml-0.1.3/src/helios/data/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:43:45.134274 helios_ml-0.1.3/src/helios/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-25 01:43:09.000000 helios_ml-0.1.3/src/helios/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-25 01:43:09.000000 helios_ml-0.1.3/src/helios/losses/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-25 01:43:09.000000 helios_ml-0.1.3/src/helios/losses/weighted_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:43:45.134274 helios_ml-0.1.3/src/helios/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-25 01:43:09.000000 helios_ml-0.1.3/src/helios/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13882 2024-04-25 01:43:09.000000 helios_ml-0.1.3/src/helios/metrics/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-04-25 01:43:09.000000 helios_ml-0.1.3/src/helios/metrics/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:43:45.134274 helios_ml-0.1.3/src/helios/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-25 01:43:09.000000 helios_ml-0.1.3/src/helios/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13012 2024-04-25 01:43:09.000000 helios_ml-0.1.3/src/helios/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-25 01:43:09.000000 helios_ml-0.1.3/src/helios/model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:43:45.134274 helios_ml-0.1.3/src/helios/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-25 01:43:09.000000 helios_ml-0.1.3/src/helios/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-25 01:43:09.000000 helios_ml-0.1.3/src/helios/nn/swa_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-25 01:43:09.000000 helios_ml-0.1.3/src/helios/nn/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-25 01:43:09.000000 helios_ml-0.1.3/src/helios/onnx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:43:45.134274 helios_ml-0.1.3/src/helios/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-25 01:43:09.000000 helios_ml-0.1.3/src/helios/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-25 01:43:09.000000 helios_ml-0.1.3/src/helios/optim/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 01:43:09.000000 helios_ml-0.1.3/src/helios/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:43:45.134274 helios_ml-0.1.3/src/helios/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-25 01:43:09.000000 helios_ml-0.1.3/src/helios/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-25 01:43:09.000000 helios_ml-0.1.3/src/helios/scheduler/schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-25 01:43:09.000000 helios_ml-0.1.3/src/helios/scheduler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35667 2024-04-25 01:43:09.000000 helios_ml-0.1.3/src/helios/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:43:45.138274 helios_ml-0.1.3/src/helios_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-04-25 01:43:45.000000 helios_ml-0.1.3/src/helios_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-25 01:43:45.000000 helios_ml-0.1.3/src/helios_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 01:43:45.000000 helios_ml-0.1.3/src/helios_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-25 01:43:45.000000 helios_ml-0.1.3/src/helios_ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 01:43:45.000000 helios_ml-0.1.3/src/helios_ml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:43:45.138274 helios_ml-0.1.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 01:43:09.000000 helios_ml-0.1.3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-25 01:43:09.000000 helios_ml-0.1.3/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:43:45.138274 helios_ml-0.1.3/test/registry_test/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-25 01:43:09.000000 helios_ml-0.1.3/test/registry_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-25 01:43:09.000000 helios_ml-0.1.3/test/registry_test/extra.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-25 01:43:09.000000 helios_ml-0.1.3/test/registry_test/foo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-25 01:43:09.000000 helios_ml-0.1.3/test/registry_test/func_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:43:45.138274 helios_ml-0.1.3/test/registry_test/nested/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 01:43:09.000000 helios_ml-0.1.3/test/registry_test/nested/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-25 01:43:09.000000 helios_ml-0.1.3/test/registry_test/nested/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-25 01:43:09.000000 helios_ml-0.1.3/test/registry_test/nested/extra.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 01:43:09.000000 helios_ml-0.1.3/test/registry_test/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-04-25 01:43:09.000000 helios_ml-0.1.3/test/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-04-25 01:43:09.000000 helios_ml-0.1.3/test/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-25 01:43:09.000000 helios_ml-0.1.3/test/test_losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-25 01:43:09.000000 helios_ml-0.1.3/test/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-25 01:43:09.000000 helios_ml-0.1.3/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-25 01:43:09.000000 helios_ml-0.1.3/test/test_nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-25 01:43:09.000000 helios_ml-0.1.3/test/test_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-25 01:43:09.000000 helios_ml-0.1.3/test/test_optim.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-25 01:43:09.000000 helios_ml-0.1.3/test/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-04-25 01:43:09.000000 helios_ml-0.1.3/test/test_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:43:45.138274 helios_ml-0.1.3/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-25 01:43:09.000000 helios_ml-0.1.3/tools/generate_requirements.py
```

### Comparing `helios_ml-0.1.2/.github/workflows/publish.yml` & `helios_ml-0.1.3/.github/workflows/publish.yml`

 * *Files 8% similar despite different names*

```diff
@@ -13,24 +13,24 @@
     environment:
       name: pypi
       url: https://pypi.org/project/helios-ml
     permissions:
       id-token: write
     steps:
       - name: Checkout
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
 
       - name: Setup Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         id: setup_python
         with:
           python-version: "3.11"
 
       - name: Cache virtualenv
-        uses: actions/cache@v3
+        uses: actions/cache@v4
         with:
           key: venv-${{ runner.os }}-${{ steps.setup_python.outputs.python-version}}-${{ hashFiles('requirements/ci.txt') }}
           path: venv
 
       - name: Install dependencies
         run: |
           python -m venv venv
```

### Comparing `helios_ml-0.1.2/.github/workflows/tests.yml` & `helios_ml-0.1.3/.github/workflows/tests.yml`

 * *Files 8% similar despite different names*

```diff
@@ -19,24 +19,24 @@
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
     steps:
       - name: Checkout
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
 
       - name: Setup Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         id: setup_python
         with:
           python-version: "3.11"
 
       - name: Cache virtualenv
-        uses: actions/cache@v3
+        uses: actions/cache@v4
         with:
           key: venv-${{ runner.os }}-${{ steps.setup_python.outputs.python-version}}-${{ hashFiles('requirements/ci.txt') }}
           path: venv
 
       - name: Install dependencies
         run: |
           python -m venv venv
```

### Comparing `helios_ml-0.1.2/.pre-commit-config.yaml` & `helios_ml-0.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.2/LICENSE` & `helios_ml-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.2/PKG-INFO` & `helios_ml-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helios-ml
-Version: 0.1.2
+Version: 0.1.3
 Summary: A light-weight system for training AI networks using PyTorch
 Author-email: "Mauricio A. Rovira Galvez" <maroviragalvez@outlook.com>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/marovira/helios-ml
 Project-URL: source, https://github.com/marovira/helios-ml
 Project-URL: issues, https://github.com/marovira/helios-ml/issues
 Project-URL: release notes, https://github.com/marovira/helios-ml/releases
```

### Comparing `helios_ml-0.1.2/README.rst` & `helios_ml-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.2/data/logo/logo-background.png` & `helios_ml-0.1.3/data/logo/logo-background.png`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.2/data/logo/logo-transparent.png` & `helios_ml-0.1.3/data/logo/logo-transparent.png`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.2/examples/cifar10/cifar10.py` & `helios_ml-0.1.3/examples/cifar10/cifar10.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.2/pyproject.toml` & `helios_ml-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.2/src/helios/core/distributed.py` & `helios_ml-0.1.3/src/helios/core/distributed.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.2/src/helios/core/logging.py` & `helios_ml-0.1.3/src/helios/core/logging.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.2/src/helios/core/rng.py` & `helios_ml-0.1.3/src/helios/core/rng.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.2/src/helios/core/utils.py` & `helios_ml-0.1.3/src/helios/core/utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.2/src/helios/data/__init__.py` & `helios_ml-0.1.3/src/helios/data/__init__.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.2/src/helios/data/datamodule.py` & `helios_ml-0.1.3/src/helios/data/datamodule.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.2/src/helios/data/functional.py` & `helios_ml-0.1.3/src/helios/data/functional.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.2/src/helios/data/samplers.py` & `helios_ml-0.1.3/src/helios/data/samplers.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.2/src/helios/data/transforms.py` & `helios_ml-0.1.3/src/helios/data/transforms.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.2/src/helios/losses/utils.py` & `helios_ml-0.1.3/src/helios/losses/utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.2/src/helios/losses/weighted_loss.py` & `helios_ml-0.1.3/src/helios/losses/weighted_loss.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             *args: arguments to the loss function.
             **kwargs: keyword arguments.
 
         Returns:
             Any: the result of the loss function.
         """
 
-    def forward(self, *args, **kwargs) -> typing.Any:
+    def forward(self, *args: typing.Any, **kwargs: typing.Any) -> typing.Any:
         """
         Forward wrapper function.
 
         The final loss value will be computed as described above.
 
         Args:
             *args: arguments to the loss function.
```

### Comparing `helios_ml-0.1.2/src/helios/metrics/functional.py` & `helios_ml-0.1.3/src/helios/metrics/functional.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.2/src/helios/metrics/metrics.py` & `helios_ml-0.1.3/src/helios/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.2/src/helios/model/model.py` & `helios_ml-0.1.3/src/helios/model/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 
         self._is_distributed: bool = False
         self._map_loc: str | dict[str, str] = ""
         self._device: torch.device | None = None
         self._rank: int = 0
 
         self._loss_items: dict[str, torch.Tensor] = {}
+        self._running_losses: dict[str, float] = {}
         self._val_scores: dict[str, float] = {}
         self._test_scores: dict[str, float] = {}
 
     @property
     def save_name(self) -> str:
         """The name of the model used for saving checkpoints and final networks."""
         return self._save_name
@@ -136,14 +137,33 @@
         Use this function to save any state that you require for checkpoints.
 
         Returns:
             dict[str, Any]: the state dictionary of the model.
         """
         return {}
 
+    def trained_state_dict(
+        self, *args: typing.Any, **kwargs: typing.Any
+    ) -> dict[str, typing.Any]:
+        """
+        Get the state dictionary for the trained model.
+
+        Use this function to save the state required for the final trained model. The
+        returned dictionary should contain only the necessary information to re-create the
+        network(s) along with any additional data you require.
+
+        Args:
+            args: positional arguments.
+            kwargs: keyword arguments.
+
+        Returns:
+            dict[str, Any]: the state dictionary without any training data.
+        """
+        return {}
+
     def append_metadata_to_chkpt_name(self, chkpt_name: str) -> str:
         """
         Append additional data to the checkpoint filename.
 
         Use this function to append the value of the loss function(s), validation
         metric(s), or any extra metadata you wish to add to the name of the checkpoint.
         Note that the epoch and iteration numbers are added automatically. The extension
@@ -153,34 +173,14 @@
             chkpt_name (str): the name of the checkpoint filename (without extension).
 
         Returns:
             str: the name with any additional metadata.
         """
         return chkpt_name
 
-    def strip_training_data(
-        self, state_dict: dict[str, typing.Any]
-    ) -> dict[str, typing.Any]:
-        """
-        Remove any training data from the state dictionary.
-
-        Use this function to convert a checkpoint into a pre-trained network. Note that
-        the auxiliary training state (log information, training settings, etc.) will be
-        removed automatically before this function is called. The returned dictionary
-        should contain only the necessary information to re-create the network(s) along
-        with any additional data you require.
-
-        Args:
-            state_dict (dict[str, Any]): the state dictionary.
-
-        Returns:
-            dict[str, Any]: the state dictionary without any training data.
-        """
-        return state_dict
-
     def train(self) -> None:
         """Switch the model to training mode."""
 
     def on_training_start(self) -> None:
         """
         Perform any necessary actions when training starts.
 
@@ -220,25 +220,33 @@
     def on_training_batch_end(
         self, state: TrainingState, should_log: bool = False
     ) -> None:
         """
         Perform any actions when a training batch ends.
 
         This function is called after train_step is called. By default, it will gather all
-        the losses (if using distributed training), but you may also use it to log your
-        losses or perform any additional tasks after the training step.
+        the losses stored in self._loss_items (if using distributed training) and will
+        update the running losses using those values. You may also use this function to
+        log your losses or perform any additional tasks after the training step.
 
         Args:
             state (TrainingState): the current training state.
             should_log (bool): if true, then logging should be performed.
         """
         if self._is_distributed:
             for _, loss in self._loss_items.items():
                 dist.all_reduce_tensors(loss)
 
+        for key, loss in self._loss_items.items():
+            if loss is not None:
+                if key not in self._running_losses:
+                    self._running_losses[key] = loss.item()
+                else:
+                    self._running_losses[key] += loss.item()
+
     def on_training_end(self) -> None:
         """
         Perform any necessary actions when training ends.
 
         You may use this function to update any weight averaging networks, or any other
         tasks that should only happen at the end of training.
         """
@@ -293,20 +301,21 @@
             step (int): the current validation batch.
         """
 
     def on_validation_end(self, validation_cycle: int) -> None:
         """
         Perform any necessary actions when validation ends.
 
-        You may use this function to compute any final validation metrics as well as log
-        them.
+        By default, this function will clear out the running loss table, but you may use
+        this function to compute any final validation metrics as well as log them.
 
         Args:
             validation_cycle (int): the validation cycle number.
         """
+        self._running_losses.clear()
 
     def have_metrics_improved(self) -> bool:
         """
         Determine whether the current validation results are an improvement or not.
 
         This is used when early stopping is enabled in the trainer to determine whether
         the stop cycle count should increase or not.
```

### Comparing `helios_ml-0.1.2/src/helios/model/utils.py` & `helios_ml-0.1.3/src/helios/model/utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.2/src/helios/nn/swa_utils.py` & `helios_ml-0.1.3/src/helios/nn/swa_utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.2/src/helios/nn/utils.py` & `helios_ml-0.1.3/src/helios/nn/utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.2/src/helios/onnx.py` & `helios_ml-0.1.3/src/helios/onnx.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.2/src/helios/optim/utils.py` & `helios_ml-0.1.3/src/helios/optim/utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.2/src/helios/scheduler/schedulers.py` & `helios_ml-0.1.3/src/helios/scheduler/schedulers.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.2/src/helios/scheduler/utils.py` & `helios_ml-0.1.3/src/helios/scheduler/utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.2/src/helios/trainer.py` & `helios_ml-0.1.3/src/helios/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -420,17 +420,22 @@
         self.model.on_training_start()
         if self._train_unit == TrainingUnit.ITERATION:
             self._train_on_iteration(training_state, resume_training)
         else:
             self._train_on_epoch(training_state)
 
         self.model.on_training_end()
+
         logging.flush_default_loggers()
         logging.close_default_loggers()
 
+        # If we're distributed, ensure that all processes are caught up before we exit.
+        if self._is_distributed:
+            td.barrier()
+
     def _test(self) -> None:
         """
         Test the model.
 
         This will ensure everything gets correctly initialised and run the testing loop on
         the dataset.
         It will automatically try to load the last saved checkpoint for testing provided
@@ -484,14 +489,17 @@
                 self.model.on_testing_batch_start(idx)
                 self.model.test_step(batch, idx)
                 self.model.on_testing_batch_end(idx)
                 pbar.update()
 
         self.model.on_testing_end()
 
+        if self._is_distributed:
+            td.barrier()
+
     def _configure_env(self) -> None:
         """
         Configure the training environment.
 
         This will seed the RNGs as well as setup any CUDA state (if using).
         """
         rng.seed_rngs(self._random_seed)
@@ -673,16 +681,16 @@
         state.
 
         Args:
             state (TrainingState): the current training state.
         """
         chkpt_root = core.get_from_optional(self._chkpt_root)
 
-        epoch = state.global_epoch
-        ite = state.global_iteration
+        epoch = state.global_epoch + 1
+        ite = state.current_iteration
         filename = f"{self.model.save_name}_epoch_{epoch}_iter_{ite}"
         filename = self.model.append_metadata_to_chkpt_name(filename)
         filename += ".pth"
 
         state_dict: dict[str, typing.Any] = {}
         state_dict["training_state"] = state.dict()
         state_dict["model"] = self.model.state_dict()
@@ -754,14 +762,15 @@
             self._is_distributed and self.rank != 0
         ) or not enable_progress_bar
         pbar = tqdm.tqdm(
             total=total_steps if total_steps != float("inf") else None,
             desc="Training iterations",
             unit="it",
             disable=pbar_disabled,
+            initial=state.current_iteration,
         )
 
         dataloader: tud.DataLoader
         sampler: ResumableSamplerType
         dataloader, sampler = core.get_from_optional(self.datamodule.train_dataloader())
 
         sampler.start_iter = state.dataset_iter
@@ -911,15 +920,15 @@
                         should_log=(
                             False
                             if print_freq is None
                             else state.current_iteration % print_freq == 0
                         ),
                     )
                     state.dataset_iter += 1
-                    if ite_pbar.update():
+                    if not ite_pbar.update():
                         ite_pbar.refresh()
 
             state.dataset_iter = 0
             state.global_epoch += 1
 
             if val_freq is not None and state.global_epoch % val_freq == 0:
                 self._validate(state.validation_cycles)
```

### Comparing `helios_ml-0.1.2/src/helios_ml.egg-info/PKG-INFO` & `helios_ml-0.1.3/src/helios_ml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helios-ml
-Version: 0.1.2
+Version: 0.1.3
 Summary: A light-weight system for training AI networks using PyTorch
 Author-email: "Mauricio A. Rovira Galvez" <maroviragalvez@outlook.com>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/marovira/helios-ml
 Project-URL: source, https://github.com/marovira/helios-ml
 Project-URL: issues, https://github.com/marovira/helios-ml/issues
 Project-URL: release notes, https://github.com/marovira/helios-ml/releases
```

### Comparing `helios_ml-0.1.2/src/helios_ml.egg-info/SOURCES.txt` & `helios_ml-0.1.3/src/helios_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.2/test/conftest.py` & `helios_ml-0.1.3/test/conftest.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.2/test/test_core.py` & `helios_ml-0.1.3/test/test_core.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.2/test/test_data.py` & `helios_ml-0.1.3/test/test_data.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.2/test/test_losses.py` & `helios_ml-0.1.3/test/test_losses.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.2/test/test_metrics.py` & `helios_ml-0.1.3/test/test_metrics.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.2/test/test_model.py` & `helios_ml-0.1.3/test/test_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,18 @@
         super().__init__("mock-model")
 
     @property
     def loss_items(self) -> dict[str, torch.Tensor]:
         return self._loss_items
 
     @property
+    def running_loss(self) -> dict[str, float]:
+        return self._running_losses
+
+    @property
     def val_scores(self) -> dict[str, float]:
         return self._val_scores
 
     @property
     def test_scores(self) -> dict[str, float]:
         return self._test_scores
 
@@ -45,30 +49,34 @@
 class TestModel:
     def test_defaults(self) -> None:
         model = MockModel()
         state = hlt.TrainingState()
 
         assert model.save_name == "mock-model"
         assert model.state_dict() == {}
+        assert model.trained_state_dict() == {}
 
         chkpt_name = "chkpt"
         assert model.append_metadata_to_chkpt_name(chkpt_name) == chkpt_name
 
-        state_dict = {"a": 1, "b": 2}
-        assert model.strip_training_data(state_dict) == state_dict
-
+        model.on_training_batch_start(state)
+        assert len(model.loss_items) == 0
         model.populate_loss()
         assert len(model.loss_items) != 0
+        model.on_training_batch_end(state)
+        assert len(model.running_loss) != 0
         model.on_training_batch_start(state)
         assert len(model.loss_items) == 0
 
         model.populate_val_scores()
         assert len(model.val_scores) != 0
         model.on_validation_start(0)
         assert len(model.loss_items) == 0
+        model.on_validation_end(0)
+        assert len(model.running_loss) == 0
 
         assert model.have_metrics_improved()
 
         model.populate_test_scores()
         assert len(model.test_scores) != 0
         model.on_testing_start()
         assert len(model.test_scores) == 0
```

### Comparing `helios_ml-0.1.2/test/test_nn.py` & `helios_ml-0.1.3/test/test_nn.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.2/test/test_onnx.py` & `helios_ml-0.1.3/test/test_onnx.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.2/test/test_trainer.py` & `helios_ml-0.1.3/test/test_trainer.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.2/tools/generate_requirements.py` & `helios_ml-0.1.3/tools/generate_requirements.py`

 * *Files identical despite different names*

