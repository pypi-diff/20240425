# Comparing `tmp/xplainable-1.2.2.post1.tar.gz` & `tmp/xplainable-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xplainable-1.2.2.post1.tar", last modified: Thu Mar 14 03:04:00 2024, max compression
+gzip compressed data, was "xplainable-1.2.3.tar", last modified: Thu Apr 25 07:23:31 2024, max compression
```

## Comparing `xplainable-1.2.2.post1.tar` & `xplainable-1.2.3.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-03-14 03:04:00.273985 xplainable-1.2.2.post1/
--rw-r--r--   0 jtuppack   (501) staff       (20)    34523 2024-03-14 02:10:23.000000 xplainable-1.2.2.post1/LICENSE
--rw-r--r--   0 jtuppack   (501) staff       (20)    51063 2024-03-14 03:04:00.273572 xplainable-1.2.2.post1/PKG-INFO
--rw-r--r--   0 jtuppack   (501) staff       (20)     9633 2024-01-25 02:25:40.000000 xplainable-1.2.2.post1/README.md
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-03-14 03:04:00.254478 xplainable-1.2.2.post1/docs/
--rw-r--r--   0 jtuppack   (501) staff       (20)     1291 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/docs/conf.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     1296 2024-03-14 03:03:37.000000 xplainable-1.2.2.post1/pyproject.toml
--rw-r--r--   0 jtuppack   (501) staff       (20)       38 2024-03-14 03:04:00.274053 xplainable-1.2.2.post1/setup.cfg
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-03-14 03:04:00.254938 xplainable-1.2.2.post1/tests/
--rw-r--r--   0 jtuppack   (501) staff       (20)        0 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/tests/__init__.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-03-14 03:04:00.255064 xplainable-1.2.2.post1/tests/core/
--rw-r--r--   0 jtuppack   (501) staff       (20)        0 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/tests/core/__init__.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-03-14 03:04:00.255266 xplainable-1.2.2.post1/tests/core/ml/
--rw-r--r--   0 jtuppack   (501) staff       (20)        0 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/tests/core/ml/__init__.py
--rw-r--r--   0 jtuppack   (501) staff       (20)      334 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/tests/core/ml/test_constructor.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-03-14 03:04:00.255672 xplainable-1.2.2.post1/tests/feature_selection/
--rw-r--r--   0 jtuppack   (501) staff       (20)        0 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/tests/feature_selection/__init__.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-03-14 03:04:00.255810 xplainable-1.2.2.post1/tests/metrics/
--rw-r--r--   0 jtuppack   (501) staff       (20)        0 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/tests/metrics/__init__.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-03-14 03:04:00.255918 xplainable-1.2.2.post1/tests/preprocessing/
--rw-r--r--   0 jtuppack   (501) staff       (20)        0 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/tests/preprocessing/__init__.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-03-14 03:04:00.256011 xplainable-1.2.2.post1/tests/quality/
--rw-r--r--   0 jtuppack   (501) staff       (20)        0 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/tests/quality/__init__.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-03-14 03:04:00.256097 xplainable-1.2.2.post1/tests/utils/
--rw-r--r--   0 jtuppack   (501) staff       (20)        0 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/tests/utils/__init__.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-03-14 03:04:00.256822 xplainable-1.2.2.post1/xplainable/
--rw-r--r--   0 jtuppack   (501) staff       (20)      834 2024-01-25 02:25:40.000000 xplainable-1.2.2.post1/xplainable/__init__.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     1575 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/_dependencies.py
--rw-r--r--   0 jtuppack   (501) staff       (20)       22 2024-03-14 02:15:51.000000 xplainable-1.2.2.post1/xplainable/_version.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-03-14 03:04:00.258013 xplainable-1.2.2.post1/xplainable/callbacks/
--rw-r--r--   0 jtuppack   (501) staff       (20)       27 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/callbacks/__init__.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     3705 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/callbacks/optimisation.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-03-14 03:04:00.258934 xplainable-1.2.2.post1/xplainable/client/
--rw-r--r--   0 jtuppack   (501) staff       (20)        0 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/client/__init__.py
--rw-r--r--   0 jtuppack   (501) staff       (20)    27284 2024-03-14 02:11:57.000000 xplainable-1.2.2.post1/xplainable/client/client.py
--rw-r--r--   0 jtuppack   (501) staff       (20)      885 2024-01-25 02:25:40.000000 xplainable-1.2.2.post1/xplainable/client/datasets.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     2295 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/client/init.py
--rw-r--r--   0 jtuppack   (501) staff       (20)      113 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/config.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-03-14 03:04:00.259217 xplainable-1.2.2.post1/xplainable/core/
--rw-r--r--   0 jtuppack   (501) staff       (20)       21 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/core/__init__.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-03-14 03:04:00.260654 xplainable-1.2.2.post1/xplainable/core/ml/
--rw-r--r--   0 jtuppack   (501) staff       (20)        0 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/core/ml/__init__.py
--rw-r--r--   0 jtuppack   (501) staff       (20)    19869 2024-03-14 02:11:57.000000 xplainable-1.2.2.post1/xplainable/core/ml/_base_model.py
--rw-r--r--   0 jtuppack   (501) staff       (20)    15808 2024-03-14 02:11:57.000000 xplainable-1.2.2.post1/xplainable/core/ml/_constructor.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     3591 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/core/ml/_constructor_parameters.py
--rw-r--r--   0 jtuppack   (501) staff       (20)    21097 2024-03-14 02:11:57.000000 xplainable-1.2.2.post1/xplainable/core/ml/classification.py
--rw-r--r--   0 jtuppack   (501) staff       (20)    15752 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/core/ml/regression.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     4311 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/core/ml/surrogate.py
--rw-r--r--   0 jtuppack   (501) staff       (20)      119 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/core/models.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-03-14 03:04:00.260890 xplainable-1.2.2.post1/xplainable/core/nlp/
--rw-r--r--   0 jtuppack   (501) staff       (20)        0 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/core/nlp/__init__.py
--rw-r--r--   0 jtuppack   (501) staff       (20)    22430 2024-01-25 02:25:40.000000 xplainable-1.2.2.post1/xplainable/core/nlp/feature_extraction.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-03-14 03:04:00.262248 xplainable-1.2.2.post1/xplainable/core/optimisation/
--rw-r--r--   0 jtuppack   (501) staff       (20)        0 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/core/optimisation/__init__.py
--rw-r--r--   0 jtuppack   (501) staff       (20)    14994 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/core/optimisation/bayesian.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     6036 2024-01-25 02:25:40.000000 xplainable-1.2.2.post1/xplainable/core/optimisation/genetic.py
--rw-r--r--   0 jtuppack   (501) staff       (20)    22379 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/core/optimisation/layers.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     6612 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/core/optimisation/nlp.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     6890 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/core/optimisation/targeting.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-03-14 03:04:00.262758 xplainable-1.2.2.post1/xplainable/feature_selection/
--rw-r--r--   0 jtuppack   (501) staff       (20)        0 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/feature_selection/__init__.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     5894 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/feature_selection/classification.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     7511 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/feature_selection/graph.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-03-14 03:04:00.263062 xplainable-1.2.2.post1/xplainable/gpt/
--rw-r--r--   0 jtuppack   (501) staff       (20)       21 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/gpt/__init__.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     1128 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/gpt/report.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-03-14 03:04:00.263225 xplainable-1.2.2.post1/xplainable/gui/
--rw-r--r--   0 jtuppack   (501) staff       (20)     1722 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/gui/__init__.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-03-14 03:04:00.264265 xplainable-1.2.2.post1/xplainable/gui/components/
--rw-r--r--   0 jtuppack   (501) staff       (20)      112 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/gui/components/__init__.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     6351 2024-03-14 02:11:57.000000 xplainable-1.2.2.post1/xplainable/gui/components/bars.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     4588 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/gui/components/cards.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     1093 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/gui/components/connectivity.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     3018 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/gui/components/header.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     8784 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/gui/components/pipelines.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     2848 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/gui/components/tables.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-03-14 03:04:00.264620 xplainable-1.2.2.post1/xplainable/gui/gradio/
--rw-r--r--   0 jtuppack   (501) staff       (20)        0 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/gui/gradio/__init__.py
--rw-r--r--   0 jtuppack   (501) staff       (20)    19766 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/gui/gradio/fine_tuning.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-03-14 03:04:00.266770 xplainable-1.2.2.post1/xplainable/gui/screens/
--rw-r--r--   0 jtuppack   (501) staff       (20)        0 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/gui/screens/__init__.py
--rw-r--r--   0 jtuppack   (501) staff       (20)    24170 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/gui/screens/classifier.py
--rw-r--r--   0 jtuppack   (501) staff       (20)    36231 2024-01-25 02:25:40.000000 xplainable-1.2.2.post1/xplainable/gui/screens/evaluate.py
--rw-r--r--   0 jtuppack   (501) staff       (20)    15870 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/gui/screens/loader.py
--rw-r--r--   0 jtuppack   (501) staff       (20)    38820 2024-01-25 02:25:40.000000 xplainable-1.2.2.post1/xplainable/gui/screens/preprocessor.py
--rw-r--r--   0 jtuppack   (501) staff       (20)    21007 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/gui/screens/regressor.py
--rw-r--r--   0 jtuppack   (501) staff       (20)    19960 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/gui/screens/save.py
--rw-r--r--   0 jtuppack   (501) staff       (20)    22051 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/gui/screens/scenario.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-03-14 03:04:00.267118 xplainable-1.2.2.post1/xplainable/metrics/
--rw-r--r--   0 jtuppack   (501) staff       (20)       22 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/metrics/__init__.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     6410 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/metrics/metrics.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-03-14 03:04:00.267430 xplainable-1.2.2.post1/xplainable/preprocessing/
--rw-r--r--   0 jtuppack   (501) staff       (20)       27 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/preprocessing/__init__.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     7554 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/preprocessing/pipeline.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-03-14 03:04:00.269119 xplainable-1.2.2.post1/xplainable/preprocessing/transformers/
--rw-r--r--   0 jtuppack   (501) staff       (20)       94 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/preprocessing/transformers/__init__.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     3518 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/preprocessing/transformers/base.py
--rw-r--r--   0 jtuppack   (501) staff       (20)    19977 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/preprocessing/transformers/categorical.py
--rw-r--r--   0 jtuppack   (501) staff       (20)    33790 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/preprocessing/transformers/dataset.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     3295 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/preprocessing/transformers/mixed.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     5002 2024-01-25 02:25:40.000000 xplainable-1.2.2.post1/xplainable/preprocessing/transformers/numeric.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-03-14 03:04:00.269414 xplainable-1.2.2.post1/xplainable/quality/
--rw-r--r--   0 jtuppack   (501) staff       (20)       26 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/quality/__init__.py
--rw-r--r--   0 jtuppack   (501) staff       (20)    10250 2024-03-14 03:02:52.000000 xplainable-1.2.2.post1/xplainable/quality/scanner.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-03-14 03:04:00.271657 xplainable-1.2.2.post1/xplainable/utils/
--rw-r--r--   0 jtuppack   (501) staff       (20)      170 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/utils/__init__.py
--rw-r--r--   0 jtuppack   (501) staff       (20)      391 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/utils/activation.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     1132 2024-03-14 02:10:23.000000 xplainable-1.2.2.post1/xplainable/utils/api.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     2209 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/utils/collections.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     6250 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/utils/dualdict.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     1293 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/utils/encoders.py
--rw-r--r--   0 jtuppack   (501) staff       (20)      226 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/utils/exceptions.py
--rw-r--r--   0 jtuppack   (501) staff       (20)      627 2024-01-25 02:25:40.000000 xplainable-1.2.2.post1/xplainable/utils/handlers.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     1048 2024-03-14 02:10:23.000000 xplainable-1.2.2.post1/xplainable/utils/helpers.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     2111 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/utils/loaders.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     2989 2024-01-25 02:25:40.000000 xplainable-1.2.2.post1/xplainable/utils/model_parsers.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     1158 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/utils/numba_funcs.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     4906 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/utils/svgs.py
--rw-r--r--   0 jtuppack   (501) staff       (20)    10052 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/utils/xwidgets.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-03-14 03:04:00.272131 xplainable-1.2.2.post1/xplainable/visualisation/
--rw-r--r--   0 jtuppack   (501) staff       (20)        0 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/visualisation/__init__.py
--rw-r--r--   0 jtuppack   (501) staff       (20)    11042 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/visualisation/explain.py
--rw-r--r--   0 jtuppack   (501) staff       (20)     2822 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/visualisation/network.py
--rw-r--r--   0 jtuppack   (501) staff       (20)      387 2024-01-22 05:09:46.000000 xplainable-1.2.2.post1/xplainable/visualisation/regression.py
-drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-03-14 03:04:00.272323 xplainable-1.2.2.post1/xplainable.egg-info/
--rw-r--r--   0 jtuppack   (501) staff       (20)    51063 2024-03-14 03:04:00.000000 xplainable-1.2.2.post1/xplainable.egg-info/PKG-INFO
--rw-r--r--   0 jtuppack   (501) staff       (20)     3218 2024-03-14 03:04:00.000000 xplainable-1.2.2.post1/xplainable.egg-info/SOURCES.txt
--rw-r--r--   0 jtuppack   (501) staff       (20)        1 2024-03-14 03:04:00.000000 xplainable-1.2.2.post1/xplainable.egg-info/dependency_links.txt
--rw-r--r--   0 jtuppack   (501) staff       (20)      440 2024-03-14 03:04:00.000000 xplainable-1.2.2.post1/xplainable.egg-info/requires.txt
--rw-r--r--   0 jtuppack   (501) staff       (20)       44 2024-03-14 03:04:00.000000 xplainable-1.2.2.post1/xplainable.egg-info/top_level.txt
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-04-25 07:23:31.644093 xplainable-1.2.3/
+-rw-r--r--   0 jtuppack   (501) staff       (20)    34523 2024-03-14 02:10:23.000000 xplainable-1.2.3/LICENSE
+-rw-r--r--   0 jtuppack   (501) staff       (20)    50918 2024-04-25 07:23:31.642892 xplainable-1.2.3/PKG-INFO
+-rw-r--r--   0 jtuppack   (501) staff       (20)     9494 2024-04-24 01:55:36.000000 xplainable-1.2.3/README.md
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-04-25 07:23:31.613380 xplainable-1.2.3/docs/
+-rw-r--r--   0 jtuppack   (501) staff       (20)     1291 2024-01-22 05:09:46.000000 xplainable-1.2.3/docs/conf.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     1294 2024-04-25 07:03:29.000000 xplainable-1.2.3/pyproject.toml
+-rw-r--r--   0 jtuppack   (501) staff       (20)       38 2024-04-25 07:23:31.644166 xplainable-1.2.3/setup.cfg
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-04-25 07:23:31.613677 xplainable-1.2.3/tests/
+-rw-r--r--   0 jtuppack   (501) staff       (20)        0 2024-01-22 05:09:46.000000 xplainable-1.2.3/tests/__init__.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-04-25 07:23:31.613779 xplainable-1.2.3/tests/core/
+-rw-r--r--   0 jtuppack   (501) staff       (20)        0 2024-01-22 05:09:46.000000 xplainable-1.2.3/tests/core/__init__.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-04-25 07:23:31.613970 xplainable-1.2.3/tests/core/ml/
+-rw-r--r--   0 jtuppack   (501) staff       (20)        0 2024-01-22 05:09:46.000000 xplainable-1.2.3/tests/core/ml/__init__.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)      334 2024-01-22 05:09:46.000000 xplainable-1.2.3/tests/core/ml/test_constructor.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-04-25 07:23:31.614253 xplainable-1.2.3/tests/feature_selection/
+-rw-r--r--   0 jtuppack   (501) staff       (20)        0 2024-01-22 05:09:46.000000 xplainable-1.2.3/tests/feature_selection/__init__.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-04-25 07:23:31.614351 xplainable-1.2.3/tests/metrics/
+-rw-r--r--   0 jtuppack   (501) staff       (20)        0 2024-01-22 05:09:46.000000 xplainable-1.2.3/tests/metrics/__init__.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-04-25 07:23:31.614438 xplainable-1.2.3/tests/preprocessing/
+-rw-r--r--   0 jtuppack   (501) staff       (20)        0 2024-01-22 05:09:46.000000 xplainable-1.2.3/tests/preprocessing/__init__.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-04-25 07:23:31.614533 xplainable-1.2.3/tests/quality/
+-rw-r--r--   0 jtuppack   (501) staff       (20)        0 2024-01-22 05:09:46.000000 xplainable-1.2.3/tests/quality/__init__.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-04-25 07:23:31.614622 xplainable-1.2.3/tests/utils/
+-rw-r--r--   0 jtuppack   (501) staff       (20)        0 2024-01-22 05:09:46.000000 xplainable-1.2.3/tests/utils/__init__.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-04-25 07:23:31.615725 xplainable-1.2.3/xplainable/
+-rw-r--r--   0 jtuppack   (501) staff       (20)      834 2024-01-25 02:25:40.000000 xplainable-1.2.3/xplainable/__init__.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     1575 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/_dependencies.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)       22 2024-04-25 07:03:29.000000 xplainable-1.2.3/xplainable/_version.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-04-25 07:23:31.617184 xplainable-1.2.3/xplainable/callbacks/
+-rw-r--r--   0 jtuppack   (501) staff       (20)       27 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/callbacks/__init__.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     3705 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/callbacks/optimisation.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-04-25 07:23:31.618058 xplainable-1.2.3/xplainable/client/
+-rw-r--r--   0 jtuppack   (501) staff       (20)        0 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/client/__init__.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)    27293 2024-04-25 07:03:29.000000 xplainable-1.2.3/xplainable/client/client.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)      885 2024-01-25 02:25:40.000000 xplainable-1.2.3/xplainable/client/datasets.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     2295 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/client/init.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)      113 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/config.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-04-25 07:23:31.618509 xplainable-1.2.3/xplainable/core/
+-rw-r--r--   0 jtuppack   (501) staff       (20)       21 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/core/__init__.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-04-25 07:23:31.620708 xplainable-1.2.3/xplainable/core/ml/
+-rw-r--r--   0 jtuppack   (501) staff       (20)        0 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/core/ml/__init__.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)    20689 2024-04-25 07:03:29.000000 xplainable-1.2.3/xplainable/core/ml/_base_model.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)    15808 2024-03-14 02:11:57.000000 xplainable-1.2.3/xplainable/core/ml/_constructor.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     3591 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/core/ml/_constructor_parameters.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)    21097 2024-03-14 02:11:57.000000 xplainable-1.2.3/xplainable/core/ml/classification.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)    16236 2024-04-25 07:03:29.000000 xplainable-1.2.3/xplainable/core/ml/regression.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     4311 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/core/ml/surrogate.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)      119 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/core/models.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-04-25 07:23:31.621120 xplainable-1.2.3/xplainable/core/nlp/
+-rw-r--r--   0 jtuppack   (501) staff       (20)        0 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/core/nlp/__init__.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)    22430 2024-01-25 02:25:40.000000 xplainable-1.2.3/xplainable/core/nlp/feature_extraction.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-04-25 07:23:31.622598 xplainable-1.2.3/xplainable/core/optimisation/
+-rw-r--r--   0 jtuppack   (501) staff       (20)        0 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/core/optimisation/__init__.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)    14994 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/core/optimisation/bayesian.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     6036 2024-01-25 02:25:40.000000 xplainable-1.2.3/xplainable/core/optimisation/genetic.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)    22379 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/core/optimisation/layers.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     6612 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/core/optimisation/nlp.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     6890 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/core/optimisation/targeting.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-04-25 07:23:31.623033 xplainable-1.2.3/xplainable/feature_selection/
+-rw-r--r--   0 jtuppack   (501) staff       (20)        0 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/feature_selection/__init__.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     5894 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/feature_selection/classification.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     7511 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/feature_selection/graph.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-04-25 07:23:31.623356 xplainable-1.2.3/xplainable/gpt/
+-rw-r--r--   0 jtuppack   (501) staff       (20)       21 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/gpt/__init__.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     1128 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/gpt/report.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-04-25 07:23:31.623587 xplainable-1.2.3/xplainable/gui/
+-rw-r--r--   0 jtuppack   (501) staff       (20)     1722 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/gui/__init__.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-04-25 07:23:31.624811 xplainable-1.2.3/xplainable/gui/components/
+-rw-r--r--   0 jtuppack   (501) staff       (20)      112 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/gui/components/__init__.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     6351 2024-03-14 02:11:57.000000 xplainable-1.2.3/xplainable/gui/components/bars.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     4588 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/gui/components/cards.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     1093 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/gui/components/connectivity.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     3018 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/gui/components/header.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     8784 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/gui/components/pipelines.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     2848 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/gui/components/tables.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-04-25 07:23:31.625045 xplainable-1.2.3/xplainable/gui/gradio/
+-rw-r--r--   0 jtuppack   (501) staff       (20)        0 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/gui/gradio/__init__.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)    19766 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/gui/gradio/fine_tuning.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-04-25 07:23:31.627118 xplainable-1.2.3/xplainable/gui/screens/
+-rw-r--r--   0 jtuppack   (501) staff       (20)        0 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/gui/screens/__init__.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)    24170 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/gui/screens/classifier.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)    36231 2024-01-25 02:25:40.000000 xplainable-1.2.3/xplainable/gui/screens/evaluate.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)    15870 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/gui/screens/loader.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)    38820 2024-01-25 02:25:40.000000 xplainable-1.2.3/xplainable/gui/screens/preprocessor.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)    21007 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/gui/screens/regressor.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)    19960 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/gui/screens/save.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)    22051 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/gui/screens/scenario.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-04-25 07:23:31.627484 xplainable-1.2.3/xplainable/metrics/
+-rw-r--r--   0 jtuppack   (501) staff       (20)       22 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/metrics/__init__.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     6410 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/metrics/metrics.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-04-25 07:23:31.627779 xplainable-1.2.3/xplainable/preprocessing/
+-rw-r--r--   0 jtuppack   (501) staff       (20)       27 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/preprocessing/__init__.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     7554 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/preprocessing/pipeline.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-04-25 07:23:31.629383 xplainable-1.2.3/xplainable/preprocessing/transformers/
+-rw-r--r--   0 jtuppack   (501) staff       (20)       94 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/preprocessing/transformers/__init__.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     3518 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/preprocessing/transformers/base.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)    19977 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/preprocessing/transformers/categorical.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)    33790 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/preprocessing/transformers/dataset.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     3295 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/preprocessing/transformers/mixed.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     5002 2024-01-25 02:25:40.000000 xplainable-1.2.3/xplainable/preprocessing/transformers/numeric.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-04-25 07:23:31.629688 xplainable-1.2.3/xplainable/quality/
+-rw-r--r--   0 jtuppack   (501) staff       (20)       26 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/quality/__init__.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)    10432 2024-04-24 01:55:29.000000 xplainable-1.2.3/xplainable/quality/scanner.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-04-25 07:23:31.637139 xplainable-1.2.3/xplainable/utils/
+-rw-r--r--   0 jtuppack   (501) staff       (20)      170 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/utils/__init__.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)      391 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/utils/activation.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     1132 2024-03-14 02:10:23.000000 xplainable-1.2.3/xplainable/utils/api.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     2209 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/utils/collections.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     6250 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/utils/dualdict.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     1293 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/utils/encoders.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)      226 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/utils/exceptions.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)      627 2024-01-25 02:25:40.000000 xplainable-1.2.3/xplainable/utils/handlers.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     1048 2024-03-14 02:10:23.000000 xplainable-1.2.3/xplainable/utils/helpers.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     2111 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/utils/loaders.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     2989 2024-01-25 02:25:40.000000 xplainable-1.2.3/xplainable/utils/model_parsers.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     1158 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/utils/numba_funcs.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     4906 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/utils/svgs.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)    10052 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/utils/xwidgets.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-04-25 07:23:31.639130 xplainable-1.2.3/xplainable/visualisation/
+-rw-r--r--   0 jtuppack   (501) staff       (20)        0 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/visualisation/__init__.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)    11042 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/visualisation/explain.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     2822 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/visualisation/network.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)      387 2024-01-22 05:09:46.000000 xplainable-1.2.3/xplainable/visualisation/regression.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-04-25 07:23:31.640577 xplainable-1.2.3/xplainable.egg-info/
+-rw-r--r--   0 jtuppack   (501) staff       (20)    50918 2024-04-25 07:23:31.000000 xplainable-1.2.3/xplainable.egg-info/PKG-INFO
+-rw-r--r--   0 jtuppack   (501) staff       (20)     3218 2024-04-25 07:23:31.000000 xplainable-1.2.3/xplainable.egg-info/SOURCES.txt
+-rw-r--r--   0 jtuppack   (501) staff       (20)        1 2024-04-25 07:23:31.000000 xplainable-1.2.3/xplainable.egg-info/dependency_links.txt
+-rw-r--r--   0 jtuppack   (501) staff       (20)      440 2024-04-25 07:23:31.000000 xplainable-1.2.3/xplainable.egg-info/requires.txt
+-rw-r--r--   0 jtuppack   (501) staff       (20)       44 2024-04-25 07:23:31.000000 xplainable-1.2.3/xplainable.egg-info/top_level.txt
```

### Comparing `xplainable-1.2.2.post1/LICENSE` & `xplainable-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/PKG-INFO` & `xplainable-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xplainable
-Version: 1.2.2.post1
+Version: 1.2.3
 Summary: Real-time explainable machine learning for business optimisation
 Author-email: xplainable pty ltd <contact@xplainable.io>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -711,15 +711,14 @@
 <div align="center">
 <img src="https://raw.githubusercontent.com/xplainable/xplainable/main/docs/assets/logo/xplainable-logo.png">
 <h1 align="center">xplainable</h1>
 <h3 align="center">Real-time explainable machine learning for business optimisation</h3>
     
 [![Python](https://img.shields.io/pypi/pyversions/xplainable)](https://pypi.org/project/xplainable/)
 [![PyPi](https://img.shields.io/pypi/v/xplainable?color=blue)](https://pypi.org/project/xplainable/)
-[![License: Apache-2.0](https://img.shields.io/github/license/saltstack/salt)](https://github.com/xplainable/xplainable/blob/main/LICENSE)
 [![Downloads](https://static.pepy.tech/badge/xplainable)](https://pepy.tech/project/xplainable)
     
 **Xplainable** makes tabular machine learning transparent, fair, and actionable.
 </div>
 
 ## Why Was Xplainable Created?
 In machine learning, there has long been a trade-off between accuracy and
```

### Comparing `xplainable-1.2.2.post1/README.md` & `xplainable-1.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 <div align="center">
 <img src="https://raw.githubusercontent.com/xplainable/xplainable/main/docs/assets/logo/xplainable-logo.png">
 <h1 align="center">xplainable</h1>
 <h3 align="center">Real-time explainable machine learning for business optimisation</h3>
     
 [![Python](https://img.shields.io/pypi/pyversions/xplainable)](https://pypi.org/project/xplainable/)
 [![PyPi](https://img.shields.io/pypi/v/xplainable?color=blue)](https://pypi.org/project/xplainable/)
-[![License: Apache-2.0](https://img.shields.io/github/license/saltstack/salt)](https://github.com/xplainable/xplainable/blob/main/LICENSE)
 [![Downloads](https://static.pepy.tech/badge/xplainable)](https://pepy.tech/project/xplainable)
     
 **Xplainable** makes tabular machine learning transparent, fair, and actionable.
 </div>
 
 ## Why Was Xplainable Created?
 In machine learning, there has long been a trade-off between accuracy and
```

### Comparing `xplainable-1.2.2.post1/docs/conf.py` & `xplainable-1.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/pyproject.toml` & `xplainable-1.2.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages]
 find = {} 
 
 [project]
 name = "xplainable"
-version = "1.2.2-1"
+version = "1.2.3"
 authors = [
   { name="xplainable pty ltd", email="contact@xplainable.io" },
 ]
 description = "Real-time explainable machine learning for business optimisation"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `xplainable-1.2.2.post1/xplainable/__init__.py` & `xplainable-1.2.3/xplainable/__init__.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/_dependencies.py` & `xplainable-1.2.3/xplainable/_dependencies.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/callbacks/optimisation.py` & `xplainable-1.2.3/xplainable/callbacks/optimisation.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/client/client.py` & `xplainable-1.2.3/xplainable/client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -486,15 +486,16 @@
         elif model.__class__.__name__ in independent_models:
             pdata = self._get_partition_data(model, '__dataset__', x, y)
             payload['partitions'].append(pdata)
         
         # Create a new version and fetch id
         url = f'{self.hostname}/v1/{self.__ext}/models/{model_id}/add-version'
         response = self.__session.post(
-            url=url, json=force_json_compliant(payload))
+            url=url, json=force_json_compliant(payload)
+        )
 
         version_id = get_response_content(response)
 
         return version_id
 
     def _get_partition_data(
             self, model, partition_name: str, x: pd.DataFrame,
```

### Comparing `xplainable-1.2.2.post1/xplainable/client/datasets.py` & `xplainable-1.2.3/xplainable/client/datasets.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/client/init.py` & `xplainable-1.2.3/xplainable/client/init.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/core/ml/_base_model.py` & `xplainable-1.2.3/xplainable/core/ml/_base_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,15 +189,16 @@
                 *[
                     (const.min_raw_score, const.max_raw_score) for const in self._constructs
                 ]
             )
         ]
 
         for xconst in self._constructs:
-            xconst.normalise_scores(_sum_min, _sum_max, self.base_value, self.min_seen, self.max_seen)
+            if not xconst.regressor:
+                xconst.normalise_scores(_sum_min, _sum_max, self.base_value, self.min_seen, self.max_seen)
             self._profile.append(np.array([list(x) for x in xconst._nodes]))
 
         return self
 
     def _encode_feature(self, x, y):
         """ Encodes features in order of their relationship with the target.
 
@@ -332,14 +333,35 @@
         if y is not None:
             if len(self.target_map) > 0:
                 y = y.map(self.target_map)
             y = y.astype(float)
             return x, y
         return x
 
+    def _normalise_transform(self, x):
+        x = x.copy()
+        x = self._cast_to_pandas(x, column_names=self.columns)
+        x = self._coerce_dtypes(x)
+        x = self._encode(x)
+        x = self._preprocess(x).to_numpy()
+
+        b = []
+        for i in range(x.shape[1]):
+            a = []
+            nodes = np.array(self._profile[i])
+            for _ in range(len(nodes)):
+                a.append(np.zeros((x.shape[0], 1)))
+            feature_matrix = np.concatenate(a, axis=1)
+            idx = np.searchsorted(nodes[:, -5], x[:, i])
+            feature_matrix[np.arange(feature_matrix.shape[0]), idx] = nodes[idx, -4]
+            b.append(feature_matrix)
+        full = np.concatenate(b, axis=1)
+
+        return full
+
     def _transform(self, x):
         x = x.copy()
         x = self._cast_to_pandas(x, column_names=self.columns)
         x = self._coerce_dtypes(x)
         x = self._encode(x)
         x = self._preprocess(x).to_numpy()
 
@@ -348,14 +370,15 @@
             idx = np.searchsorted(nodes[:, -5], x[:, i])
 
             known = np.where(idx < len(nodes))
             unknown = np.where(idx >= len(nodes))  # flag unknown categories, the addition of nan might change this
             
             x[unknown, i] = 0  # Set new categories to 0 contribution
             x[known, i] = nodes[idx[known], -4]  # get score
+            # print(nodes[idx[known], -4])
 
         return x
 
     def predict_explain(self, x):
         """ Predictions with explanations.
 
         Args:
```

### Comparing `xplainable-1.2.2.post1/xplainable/core/ml/_constructor.py` & `xplainable-1.2.3/xplainable/core/ml/_constructor.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/core/ml/_constructor_parameters.py` & `xplainable-1.2.3/xplainable/core/ml/_constructor_parameters.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/core/ml/classification.py` & `xplainable-1.2.3/xplainable/core/ml/classification.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/core/ml/regression.py` & `xplainable-1.2.3/xplainable/core/ml/regression.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 warnings.simplefilter(action='ignore', category=FutureWarning)
 
 import numpy as np
 import pandas as pd
 from ._base_model import BaseModel, BasePartition
 from ._constructor import XCatConstructor, XNumConstructor, ConstructorParams
 from sklearn.metrics import *
+from sklearn.linear_model import Ridge
 from time import time
 from typing import Union
 
 
 class XRegressor(BaseModel):
     """ Xplainable Regression model for transparent machine learning.
 
@@ -104,14 +105,24 @@
 
         self.feature_params = {}
         self.samples = None
 
         self.min_seen = 0
         self.max_seen = 0
 
+    def normalise(self, x, y):
+        trans = self._normalise_transform(x)
+        lr = Ridge().fit(trans, y)
+        idx = 0
+        for c_n, construct in enumerate(self._constructs):
+            for i, node in enumerate(construct._nodes):
+                self._constructs[c_n]._nodes[i][-4] = node[-1]*lr.coef_[idx]
+                idx += 1
+        self.base_value = lr.intercept_
+
     def fit(
         self, x: Union[pd.DataFrame, np.ndarray],
         y: Union[pd.Series, np.ndarray], id_columns: list = [],
         column_names: list = None, target_name: str = 'target', alpha=0.1
     ) -> 'XRegressor':
         """ Fits the model to the data.
 
@@ -151,14 +162,17 @@
 
             xconst.fit(f, y, alpha)
             xconst.construct()
             self._constructs.append(xconst)
 
         self._build_profile()
 
+        self.normalise(x, y)
+        self._build_profile()
+
         # record metadata
         self.metadata['fit_time'] = time() - start
         self.metadata['observations'] = x.shape[0]
         self.metadata['features'] = x.shape[1]
 
         return self
```

### Comparing `xplainable-1.2.2.post1/xplainable/core/ml/surrogate.py` & `xplainable-1.2.3/xplainable/core/ml/surrogate.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/core/nlp/feature_extraction.py` & `xplainable-1.2.3/xplainable/core/nlp/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/core/optimisation/bayesian.py` & `xplainable-1.2.3/xplainable/core/optimisation/bayesian.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/core/optimisation/genetic.py` & `xplainable-1.2.3/xplainable/core/optimisation/genetic.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/core/optimisation/layers.py` & `xplainable-1.2.3/xplainable/core/optimisation/layers.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/core/optimisation/nlp.py` & `xplainable-1.2.3/xplainable/core/optimisation/nlp.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/core/optimisation/targeting.py` & `xplainable-1.2.3/xplainable/core/optimisation/targeting.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/feature_selection/classification.py` & `xplainable-1.2.3/xplainable/feature_selection/classification.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/feature_selection/graph.py` & `xplainable-1.2.3/xplainable/feature_selection/graph.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/gpt/report.py` & `xplainable-1.2.3/xplainable/gpt/report.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/gui/__init__.py` & `xplainable-1.2.3/xplainable/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/gui/components/bars.py` & `xplainable-1.2.3/xplainable/gui/components/bars.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/gui/components/cards.py` & `xplainable-1.2.3/xplainable/gui/components/cards.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/gui/components/connectivity.py` & `xplainable-1.2.3/xplainable/gui/components/connectivity.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/gui/components/header.py` & `xplainable-1.2.3/xplainable/gui/components/header.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/gui/components/pipelines.py` & `xplainable-1.2.3/xplainable/gui/components/pipelines.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/gui/components/tables.py` & `xplainable-1.2.3/xplainable/gui/components/tables.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/gui/gradio/fine_tuning.py` & `xplainable-1.2.3/xplainable/gui/gradio/fine_tuning.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/gui/screens/classifier.py` & `xplainable-1.2.3/xplainable/gui/screens/classifier.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/gui/screens/evaluate.py` & `xplainable-1.2.3/xplainable/gui/screens/evaluate.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/gui/screens/loader.py` & `xplainable-1.2.3/xplainable/gui/screens/loader.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/gui/screens/preprocessor.py` & `xplainable-1.2.3/xplainable/gui/screens/preprocessor.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/gui/screens/regressor.py` & `xplainable-1.2.3/xplainable/gui/screens/regressor.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/gui/screens/save.py` & `xplainable-1.2.3/xplainable/gui/screens/save.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/gui/screens/scenario.py` & `xplainable-1.2.3/xplainable/gui/screens/scenario.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/metrics/metrics.py` & `xplainable-1.2.3/xplainable/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/preprocessing/pipeline.py` & `xplainable-1.2.3/xplainable/preprocessing/pipeline.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/preprocessing/transformers/base.py` & `xplainable-1.2.3/xplainable/preprocessing/transformers/base.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/preprocessing/transformers/categorical.py` & `xplainable-1.2.3/xplainable/preprocessing/transformers/categorical.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/preprocessing/transformers/dataset.py` & `xplainable-1.2.3/xplainable/preprocessing/transformers/dataset.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/preprocessing/transformers/mixed.py` & `xplainable-1.2.3/xplainable/preprocessing/transformers/mixed.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/preprocessing/transformers/numeric.py` & `xplainable-1.2.3/xplainable/preprocessing/transformers/numeric.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/quality/scanner.py` & `xplainable-1.2.3/xplainable/quality/scanner.py`

 * *Files 4% similar despite different names*

```diff
@@ -374,9 +374,13 @@
         if target:
             if target not in df.columns:
                 raise ValueError(f"{target} not in df")
             df = df.drop(columns=[target])
 
         # Iterate over each column and check for non-NaN existence before scanning
         for col in tqdm(list(df.columns)):
+            if df[col].isna().all():
+                print(f"Skipping column {col} because it is completely NaN.")
+                continue  # Skip this column as it's entirely NaN
+
             # Proceed with scanning non-NaN columns
             self.profile[col] = self._scan_feature(df[col])
```

### Comparing `xplainable-1.2.2.post1/xplainable/utils/api.py` & `xplainable-1.2.3/xplainable/utils/api.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/utils/collections.py` & `xplainable-1.2.3/xplainable/utils/collections.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/utils/dualdict.py` & `xplainable-1.2.3/xplainable/utils/dualdict.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/utils/encoders.py` & `xplainable-1.2.3/xplainable/utils/encoders.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/utils/handlers.py` & `xplainable-1.2.3/xplainable/utils/handlers.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/utils/helpers.py` & `xplainable-1.2.3/xplainable/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/utils/loaders.py` & `xplainable-1.2.3/xplainable/utils/loaders.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/utils/model_parsers.py` & `xplainable-1.2.3/xplainable/utils/model_parsers.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/utils/numba_funcs.py` & `xplainable-1.2.3/xplainable/utils/numba_funcs.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/utils/svgs.py` & `xplainable-1.2.3/xplainable/utils/svgs.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/utils/xwidgets.py` & `xplainable-1.2.3/xplainable/utils/xwidgets.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/visualisation/explain.py` & `xplainable-1.2.3/xplainable/visualisation/explain.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable/visualisation/network.py` & `xplainable-1.2.3/xplainable/visualisation/network.py`

 * *Files identical despite different names*

### Comparing `xplainable-1.2.2.post1/xplainable.egg-info/PKG-INFO` & `xplainable-1.2.3/xplainable.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xplainable
-Version: 1.2.2.post1
+Version: 1.2.3
 Summary: Real-time explainable machine learning for business optimisation
 Author-email: xplainable pty ltd <contact@xplainable.io>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -711,15 +711,14 @@
 <div align="center">
 <img src="https://raw.githubusercontent.com/xplainable/xplainable/main/docs/assets/logo/xplainable-logo.png">
 <h1 align="center">xplainable</h1>
 <h3 align="center">Real-time explainable machine learning for business optimisation</h3>
     
 [![Python](https://img.shields.io/pypi/pyversions/xplainable)](https://pypi.org/project/xplainable/)
 [![PyPi](https://img.shields.io/pypi/v/xplainable?color=blue)](https://pypi.org/project/xplainable/)
-[![License: Apache-2.0](https://img.shields.io/github/license/saltstack/salt)](https://github.com/xplainable/xplainable/blob/main/LICENSE)
 [![Downloads](https://static.pepy.tech/badge/xplainable)](https://pepy.tech/project/xplainable)
     
 **Xplainable** makes tabular machine learning transparent, fair, and actionable.
 </div>
 
 ## Why Was Xplainable Created?
 In machine learning, there has long been a trade-off between accuracy and
```

### Comparing `xplainable-1.2.2.post1/xplainable.egg-info/SOURCES.txt` & `xplainable-1.2.3/xplainable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

