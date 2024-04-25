# Comparing `tmp/gloe-0.5.7.tar.gz` & `tmp/gloe-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gloe-0.5.7.tar", last modified: Mon Apr 22 15:15:00 2024, max compression
+gzip compressed data, was "gloe-0.5.8.tar", last modified: Thu Apr 25 20:56:00 2024, max compression
```

## Comparing `gloe-0.5.7.tar` & `gloe-0.5.8.tar`

### file list

```diff
@@ -1,93 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:15:00.996467 gloe-0.5.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11334 2024-04-22 15:14:55.000000 gloe-0.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-22 15:14:55.000000 gloe-0.5.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-04-22 15:15:00.996467 gloe-0.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-04-22 15:14:55.000000 gloe-0.5.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:15:00.980467 gloe-0.5.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:15:00.984467 gloe-0.5.7/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:15:00.984467 gloe-0.5.7/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:15:00.984467 gloe-0.5.7/docs/source/_static/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-22 15:14:55.000000 gloe-0.5.7/docs/source/_static/assets/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-04-22 15:14:55.000000 gloe-0.5.7/docs/source/_static/assets/gloe-logo-small.png
--rw-r--r--   0 runner    (1001) docker     (127)     7184 2024-04-22 15:14:55.000000 gloe-0.5.7/docs/source/_static/assets/gloe-logo-small.webp
--rw-r--r--   0 runner    (1001) docker     (127)    22309 2024-04-22 15:14:55.000000 gloe-0.5.7/docs/source/_static/assets/gloe-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    55575 2024-04-22 15:14:55.000000 gloe-0.5.7/docs/source/_static/assets/graph_example.jpeg
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-22 15:14:55.000000 gloe-0.5.7/docs/source/_static/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:15:00.984467 gloe-0.5.7/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-22 15:14:55.000000 gloe-0.5.7/docs/source/_templates/page.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:15:00.984467 gloe-0.5.7/docs/source/api-reference/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-22 15:14:55.000000 gloe-0.5.7/docs/source/api-reference/gloe.collection.md
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-22 15:14:55.000000 gloe-0.5.7/docs/source/api-reference/gloe.experimental.md
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-22 15:14:55.000000 gloe-0.5.7/docs/source/api-reference/gloe.utils.md
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-22 15:14:55.000000 gloe-0.5.7/docs/source/api-reference/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-04-22 15:14:55.000000 gloe-0.5.7/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-22 15:14:55.000000 gloe-0.5.7/docs/source/docutils.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:15:00.988467 gloe-0.5.7/docs/source/getting-started/
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-22 15:14:55.000000 gloe-0.5.7/docs/source/getting-started/async-transformers.md
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-22 15:14:55.000000 gloe-0.5.7/docs/source/getting-started/conditional-flows.md
--rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-04-22 15:14:55.000000 gloe-0.5.7/docs/source/getting-started/ensurers.md
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-22 15:14:55.000000 gloe-0.5.7/docs/source/getting-started/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-22 15:14:55.000000 gloe-0.5.7/docs/source/getting-started/partial-transformers.md
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-22 15:14:55.000000 gloe-0.5.7/docs/source/getting-started/plotting.md
--rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-04-22 15:14:55.000000 gloe-0.5.7/docs/source/getting-started/transformers.md
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-22 15:14:55.000000 gloe-0.5.7/docs/source/getting-started/utilities.md
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-22 15:14:55.000000 gloe-0.5.7/docs/source/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-22 15:14:55.000000 gloe-0.5.7/docs/source/limitations.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:15:00.988467 gloe-0.5.7/docs/source/pygments/
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-22 15:14:55.000000 gloe-0.5.7/docs/source/pygments/styles.py
--rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-04-22 15:14:55.000000 gloe-0.5.7/docs/source/theory.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:15:00.988467 gloe-0.5.7/gloe/
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-22 15:14:55.000000 gloe-0.5.7/gloe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9899 2024-04-22 15:14:55.000000 gloe-0.5.7/gloe/_composition_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-22 15:14:55.000000 gloe-0.5.7/gloe/_generic_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-22 15:14:55.000000 gloe-0.5.7/gloe/_plotting_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-22 15:14:55.000000 gloe-0.5.7/gloe/_transformer_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-04-22 15:14:55.000000 gloe-0.5.7/gloe/_typing_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-04-22 15:14:55.000000 gloe-0.5.7/gloe/async_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14647 2024-04-22 15:14:55.000000 gloe-0.5.7/gloe/base_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:15:00.992467 gloe-0.5.7/gloe/collection/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-22 15:14:55.000000 gloe-0.5.7/gloe/collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-22 15:14:55.000000 gloe-0.5.7/gloe/collection/_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-22 15:14:55.000000 gloe-0.5.7/gloe/collection/_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-22 15:14:55.000000 gloe-0.5.7/gloe/collection/_mapover.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:15:00.992467 gloe-0.5.7/gloe/conditional/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-22 15:14:55.000000 gloe-0.5.7/gloe/conditional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7383 2024-04-22 15:14:55.000000 gloe-0.5.7/gloe/conditional/_conditioner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:15:00.992467 gloe-0.5.7/gloe/ensurer/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-22 15:14:55.000000 gloe-0.5.7/gloe/ensurer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-22 15:14:55.000000 gloe-0.5.7/gloe/ensurer/_ensure.py
--rw-r--r--   0 runner    (1001) docker     (127)     8725 2024-04-22 15:14:55.000000 gloe-0.5.7/gloe/ensurer/_transformer_ensurer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:15:00.992467 gloe-0.5.7/gloe/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-22 15:14:55.000000 gloe-0.5.7/gloe/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:15:00.992467 gloe-0.5.7/gloe/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-22 15:14:55.000000 gloe-0.5.7/gloe/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-22 15:14:55.000000 gloe-0.5.7/gloe/experimental/_bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-04-22 15:14:55.000000 gloe-0.5.7/gloe/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 15:14:55.000000 gloe-0.5.7/gloe/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-22 15:14:55.000000 gloe-0.5.7/gloe/transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-22 15:14:55.000000 gloe-0.5.7/gloe/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:15:00.996467 gloe-0.5.7/gloe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-04-22 15:15:00.000000 gloe-0.5.7/gloe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-22 15:15:00.000000 gloe-0.5.7/gloe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 15:15:00.000000 gloe-0.5.7/gloe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-22 15:15:00.000000 gloe-0.5.7/gloe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-22 15:15:00.000000 gloe-0.5.7/gloe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-22 15:14:55.000000 gloe-0.5.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 15:15:00.996467 gloe-0.5.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:15:00.992467 gloe-0.5.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 15:14:55.000000 gloe-0.5.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:15:00.996467 gloe-0.5.7/tests/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 15:14:55.000000 gloe-0.5.7/tests/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-22 15:14:55.000000 gloe-0.5.7/tests/lib/conditioners.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-22 15:14:55.000000 gloe-0.5.7/tests/lib/ensurers.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-22 15:14:55.000000 gloe-0.5.7/tests/lib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-22 15:14:55.000000 gloe-0.5.7/tests/lib/transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7563 2024-04-22 15:14:55.000000 gloe-0.5.7/tests/test_async_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-22 15:14:55.000000 gloe-0.5.7/tests/test_conditioner_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8390 2024-04-22 15:14:55.000000 gloe-0.5.7/tests/test_function_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-22 15:14:55.000000 gloe-0.5.7/tests/test_transformer_bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-22 15:14:55.000000 gloe-0.5.7/tests/test_transformer_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)    10220 2024-04-22 15:14:55.000000 gloe-0.5.7/tests/test_transformer_ensurer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10757 2024-04-22 15:14:55.000000 gloe-0.5.7/tests/test_transformer_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     8543 2024-04-22 15:14:55.000000 gloe-0.5.7/tests/test_transformer_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-22 15:14:55.000000 gloe-0.5.7/tests/test_transformer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:56:00.292173 gloe-0.5.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11334 2024-04-25 20:55:54.000000 gloe-0.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-25 20:55:54.000000 gloe-0.5.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-04-25 20:56:00.292173 gloe-0.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-04-25 20:55:54.000000 gloe-0.5.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:56:00.276173 gloe-0.5.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:56:00.280173 gloe-0.5.8/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:56:00.280173 gloe-0.5.8/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:56:00.280173 gloe-0.5.8/docs/source/_static/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/_static/assets/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/_static/assets/gloe-logo-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7184 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/_static/assets/gloe-logo-small.webp
+-rw-r--r--   0 runner    (1001) docker     (127)    22309 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/_static/assets/gloe-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    55575 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/_static/assets/graph_example.jpeg
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/_static/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:56:00.280173 gloe-0.5.8/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/_templates/page.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:56:00.284173 gloe-0.5.8/docs/source/api-reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/api-reference/gloe.collection.md
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/api-reference/gloe.experimental.md
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/api-reference/gloe.utils.md
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/api-reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/docutils.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:56:00.284173 gloe-0.5.8/docs/source/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/getting-started/async-transformers.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/getting-started/conditional-flows.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/getting-started/ensurers.md
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/getting-started/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/getting-started/partial-transformers.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/getting-started/plotting.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/getting-started/transformers.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/getting-started/utilities.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/limitations.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:56:00.284173 gloe-0.5.8/docs/source/pygments/
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/pygments/styles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-04-25 20:55:54.000000 gloe-0.5.8/docs/source/theory.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:56:00.288173 gloe-0.5.8/gloe/
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9899 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/_composition_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/_generic_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/_plotting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/_transformer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/_typing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/async_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15206 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/base_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:56:00.288173 gloe-0.5.8/gloe/collection/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/collection/_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/collection/_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/collection/_mapover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:56:00.288173 gloe-0.5.8/gloe/conditional/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/conditional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7383 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/conditional/_conditioner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:56:00.288173 gloe-0.5.8/gloe/ensurer/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/ensurer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/ensurer/_ensure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8725 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/ensurer/_transformer_ensurer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:56:00.288173 gloe-0.5.8/gloe/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:56:00.288173 gloe-0.5.8/gloe/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/experimental/_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-25 20:55:54.000000 gloe-0.5.8/gloe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:56:00.292173 gloe-0.5.8/gloe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-04-25 20:56:00.000000 gloe-0.5.8/gloe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-25 20:56:00.000000 gloe-0.5.8/gloe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 20:56:00.000000 gloe-0.5.8/gloe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-25 20:56:00.000000 gloe-0.5.8/gloe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-25 20:56:00.000000 gloe-0.5.8/gloe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-25 20:55:54.000000 gloe-0.5.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 20:56:00.292173 gloe-0.5.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:56:00.292173 gloe-0.5.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 20:55:54.000000 gloe-0.5.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:56:00.292173 gloe-0.5.8/tests/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 20:55:54.000000 gloe-0.5.8/tests/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-25 20:55:54.000000 gloe-0.5.8/tests/lib/conditioners.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-25 20:55:54.000000 gloe-0.5.8/tests/lib/ensurers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-25 20:55:54.000000 gloe-0.5.8/tests/lib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-25 20:55:54.000000 gloe-0.5.8/tests/lib/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7563 2024-04-25 20:55:54.000000 gloe-0.5.8/tests/test_async_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-25 20:55:54.000000 gloe-0.5.8/tests/test_conditioner_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8390 2024-04-25 20:55:54.000000 gloe-0.5.8/tests/test_function_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-25 20:55:54.000000 gloe-0.5.8/tests/test_transformer_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-25 20:55:54.000000 gloe-0.5.8/tests/test_transformer_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10220 2024-04-25 20:55:54.000000 gloe-0.5.8/tests/test_transformer_ensurer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-25 20:55:54.000000 gloe-0.5.8/tests/test_transformer_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10757 2024-04-25 20:55:54.000000 gloe-0.5.8/tests/test_transformer_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8543 2024-04-25 20:55:54.000000 gloe-0.5.8/tests/test_transformer_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-25 20:55:54.000000 gloe-0.5.8/tests/test_transformer_utils.py
```

### Comparing `gloe-0.5.7/LICENSE` & `gloe-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/PKG-INFO` & `gloe-0.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gloe
-Version: 0.5.7
+Version: 0.5.8
 Summary: Gloe (pronounced /ɡloʊ/, like "glow") is a general-purpose library made to help developers create, maintain, document, and test both operational and flow-oriented code.
 Author-email: Samir Braga <samirchavess@gmail.com>
 Project-URL: Homepage, https://gloe.ideos.com.br
 Project-URL: Documentation, https://gloe.ideos.com.br
 Project-URL: Issues, https://github.com/ideos/gloe/issues
 Project-URL: Repository, https://github.com/ideos/gloe
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: typing_extensions~=4.7.1
+Requires-Dist: typing_extensions~=4.7
 Requires-Dist: networkx~=3.1
 Provides-Extra: plot
 Requires-Dist: pygraphviz>=1.11; extra == "plot"
 Provides-Extra: types
 Requires-Dist: mypy~=1.7.0; extra == "types"
```

### Comparing `gloe-0.5.7/README.md` & `gloe-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/docs/source/_static/assets/favicon.ico` & `gloe-0.5.8/docs/source/_static/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/docs/source/_static/assets/gloe-logo-small.png` & `gloe-0.5.8/docs/source/_static/assets/gloe-logo-small.png`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/docs/source/_static/assets/gloe-logo-small.webp` & `gloe-0.5.8/docs/source/_static/assets/gloe-logo-small.webp`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/docs/source/_static/assets/gloe-logo.png` & `gloe-0.5.8/docs/source/_static/assets/gloe-logo.png`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/docs/source/_static/assets/graph_example.jpeg` & `gloe-0.5.8/docs/source/_static/assets/graph_example.jpeg`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/docs/source/_templates/page.html` & `gloe-0.5.8/docs/source/_templates/page.html`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/docs/source/api-reference/index.md` & `gloe-0.5.8/docs/source/api-reference/index.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/docs/source/conf.py` & `gloe-0.5.8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/docs/source/getting-started/async-transformers.md` & `gloe-0.5.8/docs/source/getting-started/async-transformers.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/docs/source/getting-started/conditional-flows.md` & `gloe-0.5.8/docs/source/getting-started/conditional-flows.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/docs/source/getting-started/ensurers.md` & `gloe-0.5.8/docs/source/getting-started/ensurers.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/docs/source/getting-started/partial-transformers.md` & `gloe-0.5.8/docs/source/getting-started/partial-transformers.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/docs/source/getting-started/plotting.md` & `gloe-0.5.8/docs/source/getting-started/plotting.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/docs/source/getting-started/transformers.md` & `gloe-0.5.8/docs/source/getting-started/transformers.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/docs/source/getting-started/utilities.md` & `gloe-0.5.8/docs/source/getting-started/utilities.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/docs/source/index.md` & `gloe-0.5.8/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/docs/source/limitations.md` & `gloe-0.5.8/docs/source/limitations.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/docs/source/pygments/styles.py` & `gloe-0.5.8/docs/source/pygments/styles.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/docs/source/theory.md` & `gloe-0.5.8/docs/source/theory.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/gloe/__init__.py` & `gloe-0.5.8/gloe/__init__.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/gloe/_composition_utils.py` & `gloe-0.5.8/gloe/_composition_utils.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/gloe/_generic_types.py` & `gloe-0.5.8/gloe/_generic_types.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/gloe/_plotting_utils.py` & `gloe-0.5.8/gloe/_plotting_utils.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/gloe/_transformer_utils.py` & `gloe-0.5.8/gloe/_transformer_utils.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/gloe/_typing_utils.py` & `gloe-0.5.8/gloe/_typing_utils.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/gloe/async_transformer.py` & `gloe-0.5.8/gloe/async_transformer.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/gloe/base_transformer.py` & `gloe-0.5.8/gloe/base_transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -405,14 +405,28 @@
     def graph(self) -> DiGraph:
         net = nx.DiGraph()
         net.graph["splines"] = "ortho"
         self._dag(net)
         return net
 
     def export(self, path: str, with_edge_labels: bool = True):  # pragma: no cover
+        """Export Transformer object in dot format"""
+
+        try:
+            import pygraphviz  # noqa: F401
+
+        except ImportError as err:
+            raise ImportError(
+                "Please, the module pygraphviz is required for this method,"
+                + " install with "
+                + """"conda install --channel conda-forge pygraphviz" or """
+                + """"pip install pygraphviz". More information is available in """
+                + "https://pygraphviz.github.io/documentation/stable/install.html"
+            ) from err
+
         net = self.graph()
         boxed_nodes = [
             node
             for node in net.nodes.data()
             if "parent_id" in node[1] and "bounding_box" in node[1]
         ]
         if not with_edge_labels:
```

### Comparing `gloe-0.5.7/gloe/collection/_filter.py` & `gloe-0.5.8/gloe/collection/_filter.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/gloe/collection/_map.py` & `gloe-0.5.8/gloe/collection/_map.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/gloe/collection/_mapover.py` & `gloe-0.5.8/gloe/collection/_mapover.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/gloe/conditional/_conditioner.py` & `gloe-0.5.8/gloe/conditional/_conditioner.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/gloe/ensurer/_ensure.py` & `gloe-0.5.8/gloe/ensurer/_ensure.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/gloe/ensurer/_transformer_ensurer.py` & `gloe-0.5.8/gloe/ensurer/_transformer_ensurer.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/gloe/experimental/_bridge.py` & `gloe-0.5.8/gloe/experimental/_bridge.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/gloe/functional.py` & `gloe-0.5.8/gloe/functional.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/gloe/transformers.py` & `gloe-0.5.8/gloe/transformers.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/gloe/utils.py` & `gloe-0.5.8/gloe/utils.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/gloe.egg-info/PKG-INFO` & `gloe-0.5.8/gloe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gloe
-Version: 0.5.7
+Version: 0.5.8
 Summary: Gloe (pronounced /ɡloʊ/, like "glow") is a general-purpose library made to help developers create, maintain, document, and test both operational and flow-oriented code.
 Author-email: Samir Braga <samirchavess@gmail.com>
 Project-URL: Homepage, https://gloe.ideos.com.br
 Project-URL: Documentation, https://gloe.ideos.com.br
 Project-URL: Issues, https://github.com/ideos/gloe/issues
 Project-URL: Repository, https://github.com/ideos/gloe
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: typing_extensions~=4.7.1
+Requires-Dist: typing_extensions~=4.7
 Requires-Dist: networkx~=3.1
 Provides-Extra: plot
 Requires-Dist: pygraphviz>=1.11; extra == "plot"
 Provides-Extra: types
 Requires-Dist: mypy~=1.7.0; extra == "types"
```

### Comparing `gloe-0.5.7/gloe.egg-info/SOURCES.txt` & `gloe-0.5.8/gloe.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 tests/__init__.py
 tests/test_async_transformer.py
 tests/test_conditioner_transformer.py
 tests/test_function_transformer.py
 tests/test_transformer_bridge.py
 tests/test_transformer_collections.py
 tests/test_transformer_ensurer.py
+tests/test_transformer_export.py
 tests/test_transformer_graph.py
 tests/test_transformer_types.py
 tests/test_transformer_utils.py
 tests/lib/__init__.py
 tests/lib/conditioners.py
 tests/lib/ensurers.py
 tests/lib/exceptions.py
```

### Comparing `gloe-0.5.7/pyproject.toml` & `gloe-0.5.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gloe"
-version = "0.5.7"
+version = "0.5.8"
 authors = [
   { name="Samir Braga", email="samirchavess@gmail.com" },
 ]
 description = "Gloe (pronounced /ɡloʊ/, like \"glow\") is a general-purpose library made to help developers create, maintain, document, and test both operational and flow-oriented code."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -16,15 +16,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    'typing_extensions~=4.7.1',
+    'typing_extensions~=4.7',
     'networkx~=3.1'
 ]
 
 [project.urls]
 Homepage = "https://gloe.ideos.com.br"
 Documentation = "https://gloe.ideos.com.br"
 Issues = "https://github.com/ideos/gloe/issues"
```

### Comparing `gloe-0.5.7/tests/lib/ensurers.py` & `gloe-0.5.8/tests/lib/ensurers.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/tests/lib/transformers.py` & `gloe-0.5.8/tests/lib/transformers.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/tests/test_async_transformer.py` & `gloe-0.5.8/tests/test_async_transformer.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/tests/test_conditioner_transformer.py` & `gloe-0.5.8/tests/test_conditioner_transformer.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/tests/test_function_transformer.py` & `gloe-0.5.8/tests/test_function_transformer.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/tests/test_transformer_bridge.py` & `gloe-0.5.8/tests/test_transformer_bridge.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/tests/test_transformer_collections.py` & `gloe-0.5.8/tests/test_transformer_collections.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/tests/test_transformer_ensurer.py` & `gloe-0.5.8/tests/test_transformer_ensurer.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/tests/test_transformer_graph.py` & `gloe-0.5.8/tests/test_transformer_graph.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/tests/test_transformer_types.py` & `gloe-0.5.8/tests/test_transformer_types.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.7/tests/test_transformer_utils.py` & `gloe-0.5.8/tests/test_transformer_utils.py`

 * *Files identical despite different names*

