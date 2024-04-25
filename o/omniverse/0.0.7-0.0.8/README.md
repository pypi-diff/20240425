# Comparing `tmp/omniverse-0.0.7.tar.gz` & `tmp/omniverse-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omniverse-0.0.7.tar", last modified: Fri Dec 29 03:11:21 2023, max compression
+gzip compressed data, was "omniverse-0.0.8.tar", last modified: Fri Dec 29 03:29:41 2023, max compression
```

## Comparing `omniverse-0.0.7.tar` & `omniverse-0.0.8.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:21.190936 omniverse-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)    10827 2023-12-29 03:11:11.000000 omniverse-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10474 2023-12-29 03:11:21.190936 omniverse-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8776 2023-12-29 03:11:11.000000 omniverse-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:21.174936 omniverse-0.0.7/omnivault/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:21.178936 omniverse-0.0.7/omnivault/_types/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/_types/_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/_types/_generic.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/_types/_newtype.py
--rw-r--r--   0 runner    (1001) docker     (127)     7341 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/_types/_sentinel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/_types/sentinel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:21.178936 omniverse-0.0.7/omnivault/dsa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/dsa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:21.178936 omniverse-0.0.7/omnivault/dsa/heap/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/dsa/heap/priority_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:21.178936 omniverse-0.0.7/omnivault/dsa/queue/
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/dsa/queue/deque.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:21.178936 omniverse-0.0.7/omnivault/dsa/searching_algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)      611 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/dsa/searching_algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/dsa/searching_algorithms/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/dsa/searching_algorithms/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     6709 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/dsa/searching_algorithms/strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:21.178936 omniverse-0.0.7/omnivault/dsa/stack/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/dsa/stack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/dsa/stack/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/dsa/stack/concrete.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:21.178936 omniverse-0.0.7/omnivault/linear_algebra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/linear_algebra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/linear_algebra/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7953 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/linear_algebra/plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/linear_algebra/vector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:21.178936 omniverse-0.0.7/omnivault/transformer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/transformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:21.182936 omniverse-0.0.7/omnivault/transformer/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/transformer/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/transformer/config/composer.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/transformer/config/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/transformer/config/criterion.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/transformer/config/decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/transformer/config/global_.py
--rw-r--r--   0 runner    (1001) docker     (127)     9812 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/transformer/config/ground_truth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4419 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/transformer/config/optim.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:21.182936 omniverse-0.0.7/omnivault/transformer/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/transformer/core/criterion.py
--rw-r--r--   0 runner    (1001) docker     (127)    12425 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/transformer/core/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/transformer/core/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/transformer/core/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/transformer/core/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/transformer/core/state.py
--rw-r--r--   0 runner    (1001) docker     (127)    10087 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/transformer/core/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5015 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/transformer/core/vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:21.182936 omniverse-0.0.7/omnivault/transformer/decoder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/transformer/decoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4792 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/transformer/decoder/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12168 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/transformer/decoder/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/transformer/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:21.182936 omniverse-0.0.7/omnivault/transformer/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/transformer/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:21.182936 omniverse-0.0.7/omnivault/transformer/modules/attention/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/transformer/modules/attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5511 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/transformer/modules/attention/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11246 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/transformer/modules/attention/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:21.186936 omniverse-0.0.7/omnivault/transformer/modules/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/transformer/modules/layers/addnorm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/transformer/modules/layers/mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/transformer/modules/layers/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/transformer/modules/layers/residual.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:21.186936 omniverse-0.0.7/omnivault/transformer/modules/positional/
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/transformer/modules/positional/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:21.186936 omniverse-0.0.7/omnivault/transformer/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/transformer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/transformer/utils/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/transformer/utils/reproducibility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:21.186936 omniverse-0.0.7/omnivault/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:21.186936 omniverse-0.0.7/omnivault/utils/config_management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/utils/config_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5053 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/utils/config_management/dynamic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:21.186936 omniverse-0.0.7/omnivault/utils/format/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/utils/format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/utils/format/replace_inline_latex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:21.186936 omniverse-0.0.7/omnivault/utils/reproducibility/
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/utils/reproducibility/seed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:21.186936 omniverse-0.0.7/omnivault/utils/testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/utils/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/utils/testing/test_framework.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:21.186936 omniverse-0.0.7/omnivault/utils/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/utils/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/utils/visualization/figure_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/utils/visualization/matplotlib_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/utils/visualization/style.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2023-12-29 03:11:11.000000 omniverse-0.0.7/omnivault/utils/visualization/tabbed_svg_viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:11:21.190936 omniverse-0.0.7/omniverse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10474 2023-12-29 03:11:21.000000 omniverse-0.0.7/omniverse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2023-12-29 03:11:21.000000 omniverse-0.0.7/omniverse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-29 03:11:21.000000 omniverse-0.0.7/omniverse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      469 2023-12-29 03:11:21.000000 omniverse-0.0.7/omniverse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-12-29 03:11:21.000000 omniverse-0.0.7/omniverse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2023-12-29 03:11:11.000000 omniverse-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-29 03:11:21.190936 omniverse-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:41.456288 omniverse-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    10827 2023-12-29 03:29:32.000000 omniverse-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10860 2023-12-29 03:29:41.456288 omniverse-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9162 2023-12-29 03:29:32.000000 omniverse-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:41.440288 omniverse-0.0.8/omnivault/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:41.440288 omniverse-0.0.8/omnivault/_types/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/_types/_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/_types/_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/_types/_newtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7341 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/_types/_sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4820 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/_types/sentinel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:41.440288 omniverse-0.0.8/omnivault/dsa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/dsa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:41.440288 omniverse-0.0.8/omnivault/dsa/heap/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/dsa/heap/priority_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:41.440288 omniverse-0.0.8/omnivault/dsa/queue/
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/dsa/queue/deque.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:41.440288 omniverse-0.0.8/omnivault/dsa/searching_algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/dsa/searching_algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/dsa/searching_algorithms/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/dsa/searching_algorithms/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6709 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/dsa/searching_algorithms/strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:41.440288 omniverse-0.0.8/omnivault/dsa/stack/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/dsa/stack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/dsa/stack/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/dsa/stack/concrete.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:41.444288 omniverse-0.0.8/omnivault/linear_algebra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/linear_algebra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/linear_algebra/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7953 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/linear_algebra/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/linear_algebra/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:41.444288 omniverse-0.0.8/omnivault/transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/transformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:41.444288 omniverse-0.0.8/omnivault/transformer/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/transformer/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/transformer/config/composer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/transformer/config/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/transformer/config/criterion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/transformer/config/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/transformer/config/global_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9812 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/transformer/config/ground_truth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4419 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/transformer/config/optim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:41.444288 omniverse-0.0.8/omnivault/transformer/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/transformer/core/criterion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12425 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/transformer/core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/transformer/core/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/transformer/core/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/transformer/core/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/transformer/core/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10087 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/transformer/core/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/transformer/core/vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:41.448288 omniverse-0.0.8/omnivault/transformer/decoder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/transformer/decoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4792 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/transformer/decoder/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12168 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/transformer/decoder/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/transformer/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:41.448288 omniverse-0.0.8/omnivault/transformer/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/transformer/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:41.448288 omniverse-0.0.8/omnivault/transformer/modules/attention/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/transformer/modules/attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5511 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/transformer/modules/attention/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11246 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/transformer/modules/attention/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:41.448288 omniverse-0.0.8/omnivault/transformer/modules/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/transformer/modules/layers/addnorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/transformer/modules/layers/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/transformer/modules/layers/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/transformer/modules/layers/residual.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:41.448288 omniverse-0.0.8/omnivault/transformer/modules/positional/
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/transformer/modules/positional/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:41.448288 omniverse-0.0.8/omnivault/transformer/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/transformer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/transformer/utils/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/transformer/utils/reproducibility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:41.448288 omniverse-0.0.8/omnivault/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:41.448288 omniverse-0.0.8/omnivault/utils/config_management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/utils/config_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5053 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/utils/config_management/dynamic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:41.448288 omniverse-0.0.8/omnivault/utils/format/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/utils/format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/utils/format/replace_inline_latex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:41.448288 omniverse-0.0.8/omnivault/utils/reproducibility/
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/utils/reproducibility/seed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:41.452288 omniverse-0.0.8/omnivault/utils/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/utils/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/utils/testing/test_framework.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:41.452288 omniverse-0.0.8/omnivault/utils/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/utils/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/utils/visualization/figure_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/utils/visualization/matplotlib_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/utils/visualization/style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2023-12-29 03:29:32.000000 omniverse-0.0.8/omnivault/utils/visualization/tabbed_svg_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 03:29:41.452288 omniverse-0.0.8/omniverse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10860 2023-12-29 03:29:41.000000 omniverse-0.0.8/omniverse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2023-12-29 03:29:41.000000 omniverse-0.0.8/omniverse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-29 03:29:41.000000 omniverse-0.0.8/omniverse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2023-12-29 03:29:41.000000 omniverse-0.0.8/omniverse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2023-12-29 03:29:41.000000 omniverse-0.0.8/omniverse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2023-12-29 03:29:32.000000 omniverse-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-29 03:29:41.456288 omniverse-0.0.8/setup.cfg
```

### Comparing `omniverse-0.0.7/LICENSE` & `omniverse-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/PKG-INFO` & `omniverse-0.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniverse
-Version: 0.0.7
+Version: 0.0.8
 Summary: A collection of code for Omniverse.
 Author-email: GAO Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/omniverse
 Project-URL: Issues, https://github.com/gao-hongnan/omniverse/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -216,25 +216,32 @@
 
 One thing that is not mentioned in the guide, but is a good practice, is to do
 all the necessary pre-release checks before releasing your package, that
 includes all the pre-merge checks, and additional checks such as running tests,
 linting, and building the documentation. This ensures that the release is of
 high quality and is ready to be used by others.
 
+Furthermore, we add a `release-docker` workflow to build and publish a Docker
+image to Docker Hub. The workflow is triggered when a new release is published
+to PyPI. I followed
+[langchain's workflow](https://github.com/langchain-ai/langchain/blob/master/.github/workflows/langchain_release.yml)
+on how to publish a Docker image to Docker Hub via GitHub Actions. The rationale
+is ..?
+
 ### Example Workflow
 
 Update the `version` field in `pyproject.toml` to the new version, and commit
-the changes to the `dev` branch (or any other branch that satisfies the
+the changes to the `main` branch (or any other branch that satisfies the
 `on.push.branches` condition in the workflow).
 
 ```bash
-git commit -m "Bump version to 0.0.3"
-git tag -a v0.0.3 -m "Release version 0.0.3"
-git push origin dev
-git push origin v0.0.3
+git commit -m "bump version to 0.0.8"
+git tag -a v0.0.8 -m "Release version 0.0.8"
+git push origin main
+git push origin v0.0.8
 ```
 
 Then the workflow will be triggered, and the package will be published to PyPI.
 It is worth noting that we will do a pre-release check before publishing the
 package.
 
 ### References and Further Readings
```

### Comparing `omniverse-0.0.7/README.md` & `omniverse-0.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -173,25 +173,32 @@
 
 One thing that is not mentioned in the guide, but is a good practice, is to do
 all the necessary pre-release checks before releasing your package, that
 includes all the pre-merge checks, and additional checks such as running tests,
 linting, and building the documentation. This ensures that the release is of
 high quality and is ready to be used by others.
 
+Furthermore, we add a `release-docker` workflow to build and publish a Docker
+image to Docker Hub. The workflow is triggered when a new release is published
+to PyPI. I followed
+[langchain's workflow](https://github.com/langchain-ai/langchain/blob/master/.github/workflows/langchain_release.yml)
+on how to publish a Docker image to Docker Hub via GitHub Actions. The rationale
+is ..?
+
 ### Example Workflow
 
 Update the `version` field in `pyproject.toml` to the new version, and commit
-the changes to the `dev` branch (or any other branch that satisfies the
+the changes to the `main` branch (or any other branch that satisfies the
 `on.push.branches` condition in the workflow).
 
 ```bash
-git commit -m "Bump version to 0.0.3"
-git tag -a v0.0.3 -m "Release version 0.0.3"
-git push origin dev
-git push origin v0.0.3
+git commit -m "bump version to 0.0.8"
+git tag -a v0.0.8 -m "Release version 0.0.8"
+git push origin main
+git push origin v0.0.8
 ```
 
 Then the workflow will be triggered, and the package will be published to PyPI.
 It is worth noting that we will do a pre-release check before publishing the
 package.
 
 ### References and Further Readings
```

### Comparing `omniverse-0.0.7/omnivault/_types/_generic.py` & `omniverse-0.0.8/omnivault/_types/_generic.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/_types/_newtype.py` & `omniverse-0.0.8/omnivault/_types/_newtype.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/_types/_sentinel.py` & `omniverse-0.0.8/omnivault/_types/_sentinel.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/_types/sentinel.py` & `omniverse-0.0.8/omnivault/_types/sentinel.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/dsa/queue/deque.py` & `omniverse-0.0.8/omnivault/dsa/queue/deque.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/dsa/searching_algorithms/__init__.py` & `omniverse-0.0.8/omnivault/dsa/searching_algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/dsa/searching_algorithms/base.py` & `omniverse-0.0.8/omnivault/dsa/searching_algorithms/base.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/dsa/searching_algorithms/context.py` & `omniverse-0.0.8/omnivault/dsa/searching_algorithms/context.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/dsa/searching_algorithms/strategies.py` & `omniverse-0.0.8/omnivault/dsa/searching_algorithms/strategies.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/dsa/stack/base.py` & `omniverse-0.0.8/omnivault/dsa/stack/base.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/dsa/stack/concrete.py` & `omniverse-0.0.8/omnivault/dsa/stack/concrete.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/linear_algebra/base.py` & `omniverse-0.0.8/omnivault/linear_algebra/base.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/linear_algebra/plotter.py` & `omniverse-0.0.8/omnivault/linear_algebra/plotter.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/linear_algebra/vector.py` & `omniverse-0.0.8/omnivault/linear_algebra/vector.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/transformer/config/composer.py` & `omniverse-0.0.8/omnivault/transformer/config/composer.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/transformer/config/constants.py` & `omniverse-0.0.8/omnivault/transformer/config/constants.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/transformer/config/decoder.py` & `omniverse-0.0.8/omnivault/transformer/config/decoder.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/transformer/config/global_.py` & `omniverse-0.0.8/omnivault/transformer/config/global_.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/transformer/config/ground_truth.py` & `omniverse-0.0.8/omnivault/transformer/config/ground_truth.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/transformer/config/optim.py` & `omniverse-0.0.8/omnivault/transformer/config/optim.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/transformer/core/dataset.py` & `omniverse-0.0.8/omnivault/transformer/core/dataset.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/transformer/core/optimizer.py` & `omniverse-0.0.8/omnivault/transformer/core/optimizer.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/transformer/core/trainer.py` & `omniverse-0.0.8/omnivault/transformer/core/trainer.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/transformer/core/vocabulary.py` & `omniverse-0.0.8/omnivault/transformer/core/vocabulary.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/transformer/decoder/base.py` & `omniverse-0.0.8/omnivault/transformer/decoder/base.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/transformer/decoder/core.py` & `omniverse-0.0.8/omnivault/transformer/decoder/core.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/transformer/main.py` & `omniverse-0.0.8/omnivault/transformer/main.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/transformer/modules/attention/base.py` & `omniverse-0.0.8/omnivault/transformer/modules/attention/base.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/transformer/modules/attention/core.py` & `omniverse-0.0.8/omnivault/transformer/modules/attention/core.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/transformer/modules/layers/addnorm.py` & `omniverse-0.0.8/omnivault/transformer/modules/layers/addnorm.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/transformer/modules/layers/mlp.py` & `omniverse-0.0.8/omnivault/transformer/modules/layers/mlp.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/transformer/modules/layers/normalization.py` & `omniverse-0.0.8/omnivault/transformer/modules/layers/normalization.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/transformer/modules/positional/core.py` & `omniverse-0.0.8/omnivault/transformer/modules/positional/core.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/transformer/utils/reproducibility.py` & `omniverse-0.0.8/omnivault/transformer/utils/reproducibility.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/utils/config_management/dynamic.py` & `omniverse-0.0.8/omnivault/utils/config_management/dynamic.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/utils/format/replace_inline_latex.py` & `omniverse-0.0.8/omnivault/utils/format/replace_inline_latex.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/utils/reproducibility/seed.py` & `omniverse-0.0.8/omnivault/utils/reproducibility/seed.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/utils/testing/test_framework.py` & `omniverse-0.0.8/omnivault/utils/testing/test_framework.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/utils/visualization/figure_manager.py` & `omniverse-0.0.8/omnivault/utils/visualization/figure_manager.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/utils/visualization/matplotlib_wrapper.py` & `omniverse-0.0.8/omnivault/utils/visualization/matplotlib_wrapper.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omnivault/utils/visualization/tabbed_svg_viewer.py` & `omniverse-0.0.8/omnivault/utils/visualization/tabbed_svg_viewer.py`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/omniverse.egg-info/PKG-INFO` & `omniverse-0.0.8/omniverse.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniverse
-Version: 0.0.7
+Version: 0.0.8
 Summary: A collection of code for Omniverse.
 Author-email: GAO Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/omniverse
 Project-URL: Issues, https://github.com/gao-hongnan/omniverse/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -216,25 +216,32 @@
 
 One thing that is not mentioned in the guide, but is a good practice, is to do
 all the necessary pre-release checks before releasing your package, that
 includes all the pre-merge checks, and additional checks such as running tests,
 linting, and building the documentation. This ensures that the release is of
 high quality and is ready to be used by others.
 
+Furthermore, we add a `release-docker` workflow to build and publish a Docker
+image to Docker Hub. The workflow is triggered when a new release is published
+to PyPI. I followed
+[langchain's workflow](https://github.com/langchain-ai/langchain/blob/master/.github/workflows/langchain_release.yml)
+on how to publish a Docker image to Docker Hub via GitHub Actions. The rationale
+is ..?
+
 ### Example Workflow
 
 Update the `version` field in `pyproject.toml` to the new version, and commit
-the changes to the `dev` branch (or any other branch that satisfies the
+the changes to the `main` branch (or any other branch that satisfies the
 `on.push.branches` condition in the workflow).
 
 ```bash
-git commit -m "Bump version to 0.0.3"
-git tag -a v0.0.3 -m "Release version 0.0.3"
-git push origin dev
-git push origin v0.0.3
+git commit -m "bump version to 0.0.8"
+git tag -a v0.0.8 -m "Release version 0.0.8"
+git push origin main
+git push origin v0.0.8
 ```
 
 Then the workflow will be triggered, and the package will be published to PyPI.
 It is worth noting that we will do a pre-release check before publishing the
 package.
 
 ### References and Further Readings
```

### Comparing `omniverse-0.0.7/omniverse.egg-info/SOURCES.txt` & `omniverse-0.0.8/omniverse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omniverse-0.0.7/pyproject.toml` & `omniverse-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "omniverse"
-version = "0.0.7"
+version = "0.0.8"
 description = "A collection of code for Omniverse."
 authors = [{name="GAO Hongnan", email="hongnangao@gmail.com"}]
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
```

