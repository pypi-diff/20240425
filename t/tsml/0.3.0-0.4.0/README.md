# Comparing `tmp/tsml-0.3.0.tar.gz` & `tmp/tsml-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsml-0.3.0.tar", last modified: Tue Jan  9 14:33:47 2024, max compression
+gzip compressed data, was "tsml-0.4.0.tar", last modified: Thu Apr 25 10:07:18 2024, max compression
```

## Comparing `tsml-0.3.0.tar` & `tsml-0.4.0.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 14:33:47.627291 tsml-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-01-09 14:33:37.000000 tsml-0.3.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-01-09 14:33:37.000000 tsml-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-01-09 14:33:37.000000 tsml-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-01-09 14:33:47.627291 tsml-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-01-09 14:33:37.000000 tsml-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 14:33:47.607291 tsml-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-01-09 14:33:37.000000 tsml-0.3.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 14:33:47.607291 tsml-0.3.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-01-09 14:33:37.000000 tsml-0.3.0/docs/_templates/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-01-09 14:33:37.000000 tsml-0.3.0/docs/_templates/function.rst
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-01-09 14:33:37.000000 tsml-0.3.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-01-09 14:33:37.000000 tsml-0.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-01-09 14:33:37.000000 tsml-0.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-01-09 14:33:37.000000 tsml-0.3.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-01-09 14:33:37.000000 tsml-0.3.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-01-09 14:33:37.000000 tsml-0.3.0/docs/user_guide.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-01-09 14:33:37.000000 tsml-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-09 14:33:47.627291 tsml-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 14:33:47.607291 tsml-0.3.0/tsml/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11394 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 14:33:47.607291 tsml-0.3.0/tsml/compose/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/compose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20638 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/compose/_channel_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 14:33:47.611292 tsml-0.3.0/tsml/compose/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/compose/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/compose/tests/test_channel_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 14:33:47.611292 tsml-0.3.0/tsml/datasets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 14:33:47.611292 tsml-0.3.0/tsml/datasets/EqualMinimalJapaneseVowels/
--rw-r--r--   0 runner    (1001) docker     (127)   120661 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TEST.ts
--rw-r--r--   0 runner    (1001) docker     (127)   120799 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TRAIN.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 14:33:47.611292 tsml-0.3.0/tsml/datasets/MinimalChinatown/
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/datasets/MinimalChinatown/MinimalChinatown_TEST.ts
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/datasets/MinimalChinatown/MinimalChinatown_TRAIN.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 14:33:47.611292 tsml-0.3.0/tsml/datasets/MinimalGasPrices/
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TEST.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TRAIN.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 14:33:47.611292 tsml-0.3.0/tsml/datasets/MinimalJapaneseVowels/
--rw-r--r--   0 runner    (1001) docker     (127)    36247 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TEST.ts
--rw-r--r--   0 runner    (1001) docker     (127)    38758 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TRAIN.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 14:33:47.611292 tsml-0.3.0/tsml/datasets/UnequalMinimalChinatown/
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TEST.ts
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TRAIN.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 14:33:47.611292 tsml-0.3.0/tsml/datasets/UnequalMinimalGasPrices/
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TEST.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TRAIN.ts
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24932 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/datasets/_data_io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 14:33:47.615291 tsml-0.3.0/tsml/datasets/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/datasets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   286342 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/datasets/tests/_expected_data_io_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/datasets/tests/test_data_io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 14:33:47.615291 tsml-0.3.0/tsml/distance_based/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/distance_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7896 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/distance_based/_grail.py
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/distance_based/_mpdist.py
--rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/distance_based/_pf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 14:33:47.615291 tsml-0.3.0/tsml/distances/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/distances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/distances/_manhattan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 14:33:47.615291 tsml-0.3.0/tsml/dummy/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18023 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/dummy/_dummy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 14:33:47.615291 tsml-0.3.0/tsml/feature_based/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/feature_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20217 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/feature_based/_catch22.py
--rw-r--r--   0 runner    (1001) docker     (127)    13708 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/feature_based/_fpca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 14:33:47.615291 tsml-0.3.0/tsml/hybrid/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/hybrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22124 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/hybrid/_rist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 14:33:47.619291 tsml-0.3.0/tsml/interval_based/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/interval_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48835 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/interval_based/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    41948 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/interval_based/_cif.py
--rw-r--r--   0 runner    (1001) docker     (127)    21846 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/interval_based/_interval_forest.py
--rw-r--r--   0 runner    (1001) docker     (127)    30448 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/interval_based/_interval_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)    16744 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/interval_based/_rise.py
--rw-r--r--   0 runner    (1001) docker     (127)    17244 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/interval_based/_stsf.py
--rw-r--r--   0 runner    (1001) docker     (127)    16955 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/interval_based/_tsf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 14:33:47.619291 tsml-0.3.0/tsml/interval_based/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/interval_based/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/interval_based/tests/test_interval_forest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/interval_based/tests/test_interval_pipelines.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 14:33:47.619291 tsml-0.3.0/tsml/shapelet_based/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/shapelet_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/shapelet_based/_mrsqm.py
--rw-r--r--   0 runner    (1001) docker     (127)    20841 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/shapelet_based/_rdst.py
--rw-r--r--   0 runner    (1001) docker     (127)    11162 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/shapelet_based/_rsf.py
--rw-r--r--   0 runner    (1001) docker     (127)    12293 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/shapelet_based/_stc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 14:33:47.619291 tsml-0.3.0/tsml/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/tests/test_all_estimators.py
--rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/tests/test_estimator_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    47622 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/tests/test_estimators_sklearn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/tests/test_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 14:33:47.623291 tsml-0.3.0/tsml/transformations/
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/transformations/_acf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/transformations/_ar_coefficient.py
--rw-r--r--   0 runner    (1001) docker     (127)    43348 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/transformations/_catch22.py
--rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/transformations/_fpca.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/transformations/_function_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    56888 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/transformations/_interval_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/transformations/_periodogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/transformations/_quantile.py
--rw-r--r--   0 runner    (1001) docker     (127)    41527 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/transformations/_sfa.py
--rw-r--r--   0 runner    (1001) docker     (127)    56382 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/transformations/_shapelet_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/transformations/_summary_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/transformations/_transform_concatenator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 14:33:47.623291 tsml-0.3.0/tsml/transformations/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/transformations/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/transformations/tests/test_function_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/transformations/tests/test_interval_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/transformations/tests/test_periodogram.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/transformations/tests/test_transform_concatenator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 14:33:47.623291 tsml-0.3.0/tsml/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/utils/_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/utils/discovery.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 14:33:47.623291 tsml-0.3.0/tsml/utils/numba_functions/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/utils/numba_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15812 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/utils/numba_functions/general.py
--rw-r--r--   0 runner    (1001) docker     (127)    22906 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/utils/numba_functions/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    10603 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)    22625 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/utils/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 14:33:47.623291 tsml-0.3.0/tsml/vector/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15847 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/vector/_cit.py
--rw-r--r--   0 runner    (1001) docker     (127)    29766 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/vector/_rotation_forest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 14:33:47.623291 tsml-0.3.0/tsml/vector/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/vector/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-01-09 14:33:37.000000 tsml-0.3.0/tsml/vector/tests/test_rotation_forest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 14:33:47.623291 tsml-0.3.0/tsml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-01-09 14:33:47.000000 tsml-0.3.0/tsml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-01-09 14:33:47.000000 tsml-0.3.0/tsml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-09 14:33:47.000000 tsml-0.3.0/tsml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-01-09 14:33:47.000000 tsml-0.3.0/tsml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-09 14:33:47.000000 tsml-0.3.0/tsml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:07:18.342908 tsml-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-25 10:07:13.000000 tsml-0.4.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-25 10:07:13.000000 tsml-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-25 10:07:13.000000 tsml-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7105 2024-04-25 10:07:18.342908 tsml-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-25 10:07:13.000000 tsml-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:07:18.322908 tsml-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-25 10:07:13.000000 tsml-0.4.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:07:18.322908 tsml-0.4.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-25 10:07:13.000000 tsml-0.4.0/docs/_templates/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-25 10:07:13.000000 tsml-0.4.0/docs/_templates/function.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-25 10:07:13.000000 tsml-0.4.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-25 10:07:13.000000 tsml-0.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-25 10:07:13.000000 tsml-0.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-25 10:07:13.000000 tsml-0.4.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-25 10:07:13.000000 tsml-0.4.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 10:07:13.000000 tsml-0.4.0/docs/user_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-25 10:07:13.000000 tsml-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 10:07:18.342908 tsml-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:07:18.322908 tsml-0.4.0/tsml/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11394 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:07:18.322908 tsml-0.4.0/tsml/compose/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/compose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20638 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/compose/_channel_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:07:18.322908 tsml-0.4.0/tsml/compose/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/compose/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/compose/tests/test_channel_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:07:18.326908 tsml-0.4.0/tsml/datasets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:07:18.326908 tsml-0.4.0/tsml/datasets/EqualMinimalJapaneseVowels/
+-rw-r--r--   0 runner    (1001) docker     (127)   120661 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TEST.ts
+-rw-r--r--   0 runner    (1001) docker     (127)   120799 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TRAIN.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:07:18.326908 tsml-0.4.0/tsml/datasets/MinimalChinatown/
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/datasets/MinimalChinatown/MinimalChinatown_TEST.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/datasets/MinimalChinatown/MinimalChinatown_TRAIN.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:07:18.326908 tsml-0.4.0/tsml/datasets/MinimalGasPrices/
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TEST.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TRAIN.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:07:18.326908 tsml-0.4.0/tsml/datasets/MinimalJapaneseVowels/
+-rw-r--r--   0 runner    (1001) docker     (127)    36247 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TEST.ts
+-rw-r--r--   0 runner    (1001) docker     (127)    38758 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TRAIN.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:07:18.326908 tsml-0.4.0/tsml/datasets/UnequalMinimalChinatown/
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TEST.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TRAIN.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:07:18.326908 tsml-0.4.0/tsml/datasets/UnequalMinimalGasPrices/
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TEST.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TRAIN.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24932 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/datasets/_data_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:07:18.326908 tsml-0.4.0/tsml/datasets/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/datasets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   286342 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/datasets/tests/_expected_data_io_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/datasets/tests/test_data_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:07:18.330908 tsml-0.4.0/tsml/distance_based/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/distance_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8228 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/distance_based/_grail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/distance_based/_mpdist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/distance_based/_pf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:07:18.330908 tsml-0.4.0/tsml/distances/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/distances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/distances/_manhattan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:07:18.330908 tsml-0.4.0/tsml/dummy/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18023 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/dummy/_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:07:18.330908 tsml-0.4.0/tsml/feature_based/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/feature_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20217 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/feature_based/_catch22.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13708 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/feature_based/_fpca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:07:18.330908 tsml-0.4.0/tsml/hybrid/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/hybrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22193 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/hybrid/_rist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:07:18.330908 tsml-0.4.0/tsml/interval_based/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/interval_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48783 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/interval_based/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41866 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/interval_based/_cif.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21731 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/interval_based/_interval_forest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30448 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/interval_based/_interval_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16757 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/interval_based/_rise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17283 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/interval_based/_stsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16862 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/interval_based/_tsf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:07:18.330908 tsml-0.4.0/tsml/interval_based/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/interval_based/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/interval_based/tests/test_interval_forest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/interval_based/tests/test_interval_pipelines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:07:18.334908 tsml-0.4.0/tsml/shapelet_based/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/shapelet_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/shapelet_based/_mrsqm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20841 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/shapelet_based/_rdst.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11162 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/shapelet_based/_rsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12220 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/shapelet_based/_stc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:07:18.334908 tsml-0.4.0/tsml/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/tests/test_all_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/tests/test_estimator_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47622 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/tests/test_estimators_sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/tests/test_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:07:18.334908 tsml-0.4.0/tsml/transformations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/transformations/_acf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/transformations/_ar_coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43348 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/transformations/_catch22.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/transformations/_fpca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/transformations/_function_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56888 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/transformations/_interval_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/transformations/_periodogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/transformations/_quantile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41527 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/transformations/_sfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56382 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/transformations/_shapelet_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/transformations/_summary_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/transformations/_transform_concatenator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:07:18.338908 tsml-0.4.0/tsml/transformations/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/transformations/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/transformations/tests/test_function_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/transformations/tests/test_interval_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/transformations/tests/test_periodogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/transformations/tests/test_transform_concatenator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:07:18.338908 tsml-0.4.0/tsml/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/utils/_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/utils/discovery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:07:18.338908 tsml-0.4.0/tsml/utils/numba_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/utils/numba_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15812 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/utils/numba_functions/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22906 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/utils/numba_functions/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10603 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23075 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/utils/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:07:18.338908 tsml-0.4.0/tsml/vector/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15847 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/vector/_cit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28108 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/vector/_rotation_forest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:07:18.338908 tsml-0.4.0/tsml/vector/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/vector/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-25 10:07:13.000000 tsml-0.4.0/tsml/vector/tests/test_rotation_forest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:07:18.338908 tsml-0.4.0/tsml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7105 2024-04-25 10:07:18.000000 tsml-0.4.0/tsml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-04-25 10:07:18.000000 tsml-0.4.0/tsml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 10:07:18.000000 tsml-0.4.0/tsml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-25 10:07:18.000000 tsml-0.4.0/tsml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-25 10:07:18.000000 tsml-0.4.0/tsml.egg-info/top_level.txt
```

### Comparing `tsml-0.3.0/LICENSE` & `tsml-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/PKG-INFO` & `tsml-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsml
-Version: 0.3.0
+Version: 0.4.0
 Summary: A toolkit for time series machine learning algorithms.
 Author-email: Matthew Middlehurst <m.b.middlehurst@soton.ac.uk>
 Maintainer-email: Matthew Middlehurst <m.b.middlehurst@soton.ac.uk>
 License: BSD 3-Clause License
         
         Copyright (c) The Time Series Machine Learning (tsml) developers.
         All rights reserved.
@@ -45,46 +45,47 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: <3.12,>=3.8
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: <3.13,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numba>=0.55.0
 Requires-Dist: numpy>=1.21.0
 Requires-Dist: pandas>=1.5.3
 Requires-Dist: scikit-learn>=1.0.0
 Requires-Dist: packaging>=20.0
 Provides-Extra: all-extras
-Requires-Dist: pyfftw>=0.12.0; extra == "all-extras"
-Requires-Dist: statsmodels>=0.12.1; extra == "all-extras"
-Requires-Dist: wildboar>=1.1.0; extra == "all-extras"
+Requires-Dist: grailts; extra == "all-extras"
 Requires-Dist: scikit-fda>=0.7.0; extra == "all-extras"
+Requires-Dist: statsmodels>=0.12.1; extra == "all-extras"
 Requires-Dist: stumpy>=1.6.0; extra == "all-extras"
-Requires-Dist: grailts; extra == "all-extras"
+Requires-Dist: wildboar>=1.1.0; extra == "all-extras"
 Requires-Dist: fdasrsf<=2.5.2; extra == "all-extras"
 Provides-Extra: unstable-extras
-Requires-Dist: mrsqm>=0.0.1; platform_system == "Darwin" and extra == "unstable-extras"
+Requires-Dist: mrsqm>=0.0.1; (platform_system == "Darwin" and python_version < "3.12") and extra == "unstable-extras"
 Requires-Dist: pycatch22<=0.4.3; extra == "unstable-extras"
+Requires-Dist: pyfftw>=0.12.0; python_version < "3.12" and extra == "unstable-extras"
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-randomly; extra == "dev"
 Requires-Dist: pytest-timeout; extra == "dev"
-Requires-Dist: pytest-xdist; extra == "dev"
+Requires-Dist: pytest-xdist[psutil]; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-rerunfailures; extra == "dev"
 Provides-Extra: binder
 Requires-Dist: notebook; extra == "binder"
 Requires-Dist: jupyterlab; extra == "binder"
 Provides-Extra: docs
-Requires-Dist: sphinx<8.0.0; extra == "docs"
+Requires-Dist: sphinx<7.3.0; extra == "docs"
 Requires-Dist: sphinx-design; extra == "docs"
 Requires-Dist: sphinx-version-warning; extra == "docs"
 Requires-Dist: sphinx_issues; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Requires-Dist: sphinx-remove-toctrees; extra == "docs"
 Requires-Dist: sphinxext-opengraph; extra == "docs"
 Requires-Dist: nbsphinx; extra == "docs"
@@ -104,15 +105,20 @@
 [![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![license](https://img.shields.io/badge/license-BSD%203--Clause-green?logo=style)](https://github.com/time-series-machine-learning/tsml-py/blob/main/LICENSE)
 
 # tsml-py
 
 A toolkit for time series machine learning algorithms.
 
-The current release of `tsml` is v0.3.0.
+Please see [`tsml_eval`](https://github.com/time-series-machine-learning/tsml-eval) and
+[`aeon`](https://github.com/aeon-toolkit/aeon) for more developed packages. This package
+is more of a sandbox for testing out new ideas and algorithms. It may contain some
+algorithms and implementations that are not available in the other toolkits.
+
+The current release of `tsml` is v0.4.0.
 
 ## Installation
 
 `tsml` is available on PyPI and can be installed via pip:
 
 ```console
 pip install tsml
```

### Comparing `tsml-0.3.0/README.md` & `tsml-0.4.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,20 @@
 [![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![license](https://img.shields.io/badge/license-BSD%203--Clause-green?logo=style)](https://github.com/time-series-machine-learning/tsml-py/blob/main/LICENSE)
 
 # tsml-py
 
 A toolkit for time series machine learning algorithms.
 
-The current release of `tsml` is v0.3.0.
+Please see [`tsml_eval`](https://github.com/time-series-machine-learning/tsml-eval) and
+[`aeon`](https://github.com/aeon-toolkit/aeon) for more developed packages. This package
+is more of a sandbox for testing out new ideas and algorithms. It may contain some
+algorithms and implementations that are not available in the other toolkits.
+
+The current release of `tsml` is v0.4.0.
 
 ## Installation
 
 `tsml` is available on PyPI and can be installed via pip:
 
 ```console
 pip install tsml
```

### Comparing `tsml-0.3.0/docs/Makefile` & `tsml-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/docs/conf.py` & `tsml-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/docs/index.rst` & `tsml-0.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/docs/make.bat` & `tsml-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/pyproject.toml` & `tsml-0.4.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools>=61", "wheel", "toml", "build"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tsml"
-version = "0.3.0"
+version = "0.4.0"
 description = "A toolkit for time series machine learning algorithms."
 authors = [
     {name = "Matthew Middlehurst", email = "m.b.middlehurst@soton.ac.uk"},
 ]
 maintainers = [
     {name = "Matthew Middlehurst", email = "m.b.middlehurst@soton.ac.uk"},
 ]
 readme = "README.md"
-requires-python = ">=3.8,<3.12"
+requires-python = ">=3.8,<3.13"
 keywords = [
     "data-science",
     "machine-learning",
     "scikit-learn",
     "time-series",
     "time-series-classification",
     "time-series-regression",
@@ -32,53 +32,55 @@
     "Operating System :: Unix",
     "Operating System :: MacOS",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "numba>=0.55.0",
     "numpy>=1.21.0",
     "pandas>=1.5.3",
     "scikit-learn>=1.0.0",
     "packaging>=20.0",
 ]
 
 [project.optional-dependencies]
 all_extras = [
-    "pyfftw>=0.12.0",
-    "statsmodels>=0.12.1",
-    "wildboar>=1.1.0",
+    "grailts",
     "scikit-fda>=0.7.0",
+    "statsmodels>=0.12.1",
     "stumpy>=1.6.0",
-    "grailts",
+    "wildboar>=1.1.0",
+
     # temp
-    "fdasrsf<=2.5.2",  # currently above this breaks on some OS
+    "fdasrsf<=2.5.2",  # temporary, currently above this breaks on some OS
 ]
 unstable_extras = [
-    "mrsqm>=0.0.1 ; platform_system == 'Darwin'",  # requires gcc and fftw to be installed for Windows and some other OS (see http://www.fftw.org/index.html)
+    "mrsqm>=0.0.1 ; platform_system == 'Darwin' and python_version < '3.12'",  # requires gcc and fftw to be installed for Windows and some other OS (see http://www.fftw.org/index.html)
     "pycatch22<=0.4.3",  # Known to fail installation on some setups
+    "pyfftw>=0.12.0; python_version < '3.12'", # requires fftw to be installed for Windows and some other OS (see http://www.fftw.org/index.html)
 ]
 dev = [
     "pre-commit",
     "pytest",
     "pytest-randomly",
     "pytest-timeout",
-    "pytest-xdist",
+    "pytest-xdist[psutil]",
     "pytest-cov",
     "pytest-rerunfailures",
 ]
 binder = [
     "notebook",
     "jupyterlab",
 ]
 docs = [
-    "sphinx<8.0.0",
+    "sphinx<7.3.0",
     "sphinx-design",
     "sphinx-version-warning",
     "sphinx_issues",
     "sphinx-copybutton",
     "sphinx-remove-toctrees",
     "sphinxext-opengraph",
     "nbsphinx",
@@ -102,17 +104,25 @@
 ignore = [
     # Ignore virtual environments in local builds
     "venv/**",
     # Ignore local files
     "local/**",
 ]
 
+[tool.ruff.lint]
+select = ["D"]
+
+[tool.ruff.lint.pydocstyle]
+convention = "numpy"
+
 [tool.pytest.ini_options]
 testpaths = "tsml"
 addopts = '''
+    --doctest-modules
     --durations 20
     --timeout 600
     --showlocals
-    --doctest-modules
-    --numprocesses auto
+    --numprocesses logical
+    --dist worksteal
     --reruns 2
+    --only-rerun "crashed while running"
 '''
```

### Comparing `tsml-0.3.0/tsml/base.py` & `tsml-0.4.0/tsml/base.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/compose/_channel_ensemble.py` & `tsml-0.4.0/tsml/compose/_channel_ensemble.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/compose/tests/test_channel_ensemble.py` & `tsml-0.4.0/tsml/compose/tests/test_channel_ensemble.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TEST.ts` & `tsml-0.4.0/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TEST.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TRAIN.ts` & `tsml-0.4.0/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TRAIN.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/datasets/MinimalChinatown/MinimalChinatown_TEST.ts` & `tsml-0.4.0/tsml/datasets/MinimalChinatown/MinimalChinatown_TEST.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/datasets/MinimalChinatown/MinimalChinatown_TRAIN.ts` & `tsml-0.4.0/tsml/datasets/MinimalChinatown/MinimalChinatown_TRAIN.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TEST.ts` & `tsml-0.4.0/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TEST.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TRAIN.ts` & `tsml-0.4.0/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TRAIN.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TEST.ts` & `tsml-0.4.0/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TEST.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TRAIN.ts` & `tsml-0.4.0/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TRAIN.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TEST.ts` & `tsml-0.4.0/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TEST.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TRAIN.ts` & `tsml-0.4.0/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TRAIN.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TEST.ts` & `tsml-0.4.0/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TEST.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TRAIN.ts` & `tsml-0.4.0/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TRAIN.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/datasets/__init__.py` & `tsml-0.4.0/tsml/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/datasets/_data_io.py` & `tsml-0.4.0/tsml/datasets/_data_io.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/datasets/tests/_expected_data_io_output.py` & `tsml-0.4.0/tsml/datasets/tests/_expected_data_io_output.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/datasets/tests/test_data_io.py` & `tsml-0.4.0/tsml/datasets/tests/test_data_io.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/distance_based/_grail.py` & `tsml-0.4.0/tsml/distance_based/_grail.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 See the original implementation here:
 https://github.com/TheDatumOrg/grail-python
 """
 
 import os
 import sys
+import warnings
 
 import numpy as np
 from sklearn.base import ClassifierMixin
 from sklearn.model_selection import GridSearchCV
 from sklearn.svm import SVC
 from sklearn.utils.multiclass import check_classification_targets
 from sklearn.utils.validation import check_is_fitted
@@ -34,15 +35,15 @@
     """
 
     def __init__(self, classifier="svm"):
         self.classifier = classifier
 
         _check_optional_dependency("grailts", "GRAIL", self)
 
-        super(GRAILClassifier, self).__init__()
+        super().__init__()
 
     def fit(self, X, y):
         """Fit the estimator to training data.
 
         Parameters
         ----------
         X : 2D np.ndarray of shape (n_instances, n_timepoints)
@@ -81,19 +82,27 @@
             self._Dictionary,
             self._gamma,
             self._eigenvecMatrix,
             self._inVa,
         ) = self._modified_GRAIL_rep_fit(X, self._d)
 
         if self.classifier == "svm":
-            self._clf = GridSearchCV(
-                SVC(kernel="linear", probability=True),
-                param_grid={"C": [i**2 for i in np.arange(-10, 20, 0.11)]},
-                cv=min(min(class_count), 5),
-            )
+            cv = min(min(class_count), 5)
+            if cv == 1:
+                warnings.warn(
+                    "Only one class was found in y, so no cross-validation.",
+                    stacklevel=2,
+                )
+                self._clf = SVC(kernel="linear", probability=True, C=1)
+            else:
+                self._clf = GridSearchCV(
+                    SVC(kernel="linear", probability=True),
+                    param_grid={"C": [i**2 for i in np.arange(-10, 20, 0.11)]},
+                    cv=min(min(class_count), 5),
+                )
             self._clf.fit(Xt, y)
         elif self.classifier == "knn":
             self._train_Xt = Xt
             self._train_y = y
         else:
             raise ValueError("classifier must be 'svm' or 'knn'")
```

### Comparing `tsml-0.3.0/tsml/distance_based/_mpdist.py` & `tsml-0.4.0/tsml/distance_based/_mpdist.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/distance_based/_pf.py` & `tsml-0.4.0/tsml/distance_based/_pf.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/distances/_manhattan.py` & `tsml-0.4.0/tsml/distances/_manhattan.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/dummy/_dummy.py` & `tsml-0.4.0/tsml/dummy/_dummy.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/feature_based/_catch22.py` & `tsml-0.4.0/tsml/feature_based/_catch22.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/feature_based/_fpca.py` & `tsml-0.4.0/tsml/feature_based/_fpca.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/hybrid/_rist.py` & `tsml-0.4.0/tsml/hybrid/_rist.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,18 +108,18 @@
     RISTRegressor
 
     Examples
     --------
     >>> from tsml.hybrid import RISTClassifier
     >>> from tsml.utils.testing import generate_3d_test_data
     >>> X, y = generate_3d_test_data(n_samples=8, series_length=10, random_state=0)
-    >>> clf = RISTClassifier(random_state=0)
-    >>> clf.fit(X, y)
+    >>> clf = RISTClassifier(random_state=0)  # doctest: +SKIP
+    >>> clf.fit(X, y)  # doctest: +SKIP
     RISTClassifier(...)
-    >>> clf.predict(X)
+    >>> clf.predict(X)  # doctest: +SKIP
     array([0, 1, 1, 0, 0, 1, 0, 1])
     """
 
     def __init__(
         self,
         n_intervals=None,
         n_shapelets=None,
@@ -140,15 +140,15 @@
         self.n_jobs = n_jobs
 
         if use_pycatch22:
             _check_optional_dependency("pycatch22", "pycatch22", self)
         if use_pyfftw:
             _check_optional_dependency("pyfftw", "pyfftw", self)
 
-        super(RISTClassifier, self).__init__()
+        super().__init__()
 
     def fit(self, X: Union[np.ndarray, List[np.ndarray]], y: np.ndarray) -> object:
         """Fit the estimator to training data.
 
         Parameters
         ----------
         X : 3D np.ndarray of shape (n_instances, n_channels, n_timepoints)
@@ -359,18 +359,18 @@
 
     Examples
     --------
     >>> from tsml.hybrid import RISTRegressor
     >>> from tsml.utils.testing import generate_3d_test_data
     >>> X, y = generate_3d_test_data(n_samples=8, series_length=10,
     ...                              regression_target=True, random_state=0)
-    >>> reg = RISTRegressor(random_state=0)
-    >>> reg.fit(X, y)
+    >>> reg = RISTRegressor(random_state=0)  # doctest: +SKIP
+    >>> reg.fit(X, y)  # doctest: +SKIP
     RISTRegressor(...)
-    >>> reg.predict(X)
+    >>> reg.predict(X)  # doctest: +SKIP
     array([0.31798318, 1.41426301, 1.06414747, 0.6924721 , 0.56660146,
            1.26538944, 0.52324808, 1.0939405 ])
     """
 
     def __init__(
         self,
         n_intervals=None,
@@ -392,15 +392,15 @@
         self.n_jobs = n_jobs
 
         if use_pycatch22:
             _check_optional_dependency("pycatch22", "pycatch22", self)
         if use_pyfftw:
             _check_optional_dependency("pyfftw", "pyfftw", self)
 
-        super(RISTRegressor, self).__init__()
+        super().__init__()
 
     def fit(self, X: Union[np.ndarray, List[np.ndarray]], y: np.ndarray) -> object:
         """Fit the estimator to training data.
 
         Parameters
         ----------
         X : 3D np.ndarray of shape (n_instances, n_channels, n_timepoints)
```

### Comparing `tsml-0.3.0/tsml/interval_based/__init__.py` & `tsml-0.4.0/tsml/interval_based/__init__.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/interval_based/_base.py` & `tsml-0.4.0/tsml/interval_based/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         "nan" will replace infinite values with NaNs. If None, do not replace NaNs.
     time_limit_in_minutes : int, default=0
         Time contract to limit build time in minutes, overriding n_estimators.
         Default of 0 means n_estimators are used.
     contract_max_n_estimators : int, default=500
         Max number of estimators when time_limit_in_minutes is set.
     save_transformed_data : bool, default=False
-        Save the data transformed in fit for use in _get_train_probs.
+        Save the data transformed in fit.
     random_state : int, RandomState instance or None, default=None
         If `int`, random_state is the seed used by the random number generator;
         If `RandomState` instance, random_state is the random number generator;
         If `None`, the random number generator is the `RandomState` instance used
         by `np.random`.
     n_jobs : int, default=1
         The number of jobs to run in parallel for both `fit` and `predict`.
@@ -207,15 +207,15 @@
         self.time_limit_in_minutes = time_limit_in_minutes
         self.contract_max_n_estimators = contract_max_n_estimators
         self.save_transformed_data = save_transformed_data
         self.random_state = random_state
         self.n_jobs = n_jobs
         self.parallel_backend = parallel_backend
 
-        super(BaseIntervalForest, self).__init__()
+        super().__init__()
 
     # if subsampling attributes, an interval_features transformer must contain a
     # parameter name from transformer_feature_selection and an attribute name
     # (or property) from transformer_feature_names to allow features to be subsampled
     transformer_feature_selection = ["features"]
     transformer_feature_names = [
         "features_arguments_",
```

### Comparing `tsml-0.3.0/tsml/interval_based/_cif.py` & `tsml-0.4.0/tsml/interval_based/_cif.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     contract_max_n_estimators : int, default=500
         Max number of estimators when time_limit_in_minutes is set.
     use_pycatch22 : bool, optional, default=True
         Wraps the C based pycatch22 implementation for aeon.
         (https://github.com/DynamicsAndNeuralSystems/pycatch22). This requires the
         ``pycatch22`` package to be installed if True.
     save_transformed_data : bool, default=False
-        Save the data transformed in fit for use in _get_train_probs.
+        Save the data transformed in fit.
     random_state : int, RandomState instance or None, default=None
         If `int`, random_state is the seed used by the random number generator;
         If `RandomState` instance, random_state is the random number generator;
         If `None`, the random number generator is the `RandomState` instance used
         by `np.random`.
     n_jobs : int, default=1
         The number of jobs to run in parallel for both `fit` and `predict`.
@@ -203,15 +203,15 @@
         interval_features = [
             Catch22Transformer(outlier_norm=True, use_pycatch22=use_pycatch22),
             row_mean,
             row_std,
             row_slope,
         ]
 
-        super(CIFClassifier, self).__init__(
+        super().__init__(
             base_estimator=base_estimator,
             n_estimators=n_estimators,
             interval_selection_method="random",
             n_intervals=n_intervals,
             min_interval_length=min_interval_length,
             max_interval_length=max_interval_length,
             interval_features=interval_features,
@@ -341,15 +341,15 @@
     contract_max_n_estimators : int, default=500
         Max number of estimators when time_limit_in_minutes is set.
     use_pycatch22 : bool, optional, default=True
         Wraps the C based pycatch22 implementation for aeon.
         (https://github.com/DynamicsAndNeuralSystems/pycatch22). This requires the
         ``pycatch22`` package to be installed if True.
     save_transformed_data : bool, default=False
-        Save the data transformed in fit for use in _get_train_probs.
+        Save the data transformed in fit.
     random_state : int, RandomState instance or None, default=None
         If `int`, random_state is the seed used by the random number generator;
         If `RandomState` instance, random_state is the random number generator;
         If `None`, the random number generator is the `RandomState` instance used
         by `np.random`.
     n_jobs : int, default=1
         The number of jobs to run in parallel for both `fit` and `predict`.
@@ -427,15 +427,15 @@
         interval_features = [
             Catch22Transformer(outlier_norm=True, use_pycatch22=use_pycatch22),
             row_mean,
             row_std,
             row_slope,
         ]
 
-        super(CIFRegressor, self).__init__(
+        super().__init__(
             base_estimator=base_estimator,
             n_estimators=n_estimators,
             interval_selection_method="random",
             n_intervals=n_intervals,
             min_interval_length=min_interval_length,
             max_interval_length=max_interval_length,
             interval_features=interval_features,
@@ -561,15 +561,15 @@
         Wraps the C based pycatch22 implementation for aeon.
         (https://github.com/DynamicsAndNeuralSystems/pycatch22). This requires the
         ``pycatch22`` package to be installed if True.
     use_pyfftw : bool, default=True
         Whether to use the pyfftw library for FFT calculations. Requires the pyfftw
         package to be installed.
     save_transformed_data : bool, default=False
-        Save the data transformed in fit for use in _get_train_probs.
+        Save the data transformed in fit.
     random_state : int, RandomState instance or None, default=None
         If `int`, random_state is the seed used by the random number generator;
         If `RandomState` instance, random_state is the random number generator;
         If `None`, the random number generator is the `RandomState` instance used
         by `np.random`.
     n_jobs : int, default=1
         The number of jobs to run in parallel for both `fit` and `predict`.
@@ -623,18 +623,18 @@
        classification." arXiv preprint arXiv:2104.07551 (2021).
 
     Examples
     --------
     >>> from tsml.interval_based import DrCIFClassifier
     >>> from tsml.utils.testing import generate_3d_test_data
     >>> X, y = generate_3d_test_data(n_samples=10, series_length=12, random_state=0)
-    >>> clf = DrCIFClassifier(n_estimators=10, random_state=0)
-    >>> clf.fit(X, y)
+    >>> clf = DrCIFClassifier(n_estimators=10, random_state=0)  # doctest: +SKIP
+    >>> clf.fit(X, y)  # doctest: +SKIP
     DrCIFClassifier(...)
-    >>> clf.predict(X)
+    >>> clf.predict(X)  # doctest: +SKIP
     array([0, 1, 0, 1, 0, 0, 1, 1, 1, 0])
     """
 
     def __init__(
         self,
         base_estimator=None,
         n_estimators=200,
@@ -677,15 +677,15 @@
             row_slope,
             row_median,
             row_iqr,
             row_numba_min,
             row_numba_max,
         ]
 
-        super(DrCIFClassifier, self).__init__(
+        super().__init__(
             base_estimator=base_estimator,
             n_estimators=n_estimators,
             interval_selection_method="random",
             n_intervals=n_intervals,
             min_interval_length=min_interval_length,
             max_interval_length=max_interval_length,
             interval_features=interval_features,
@@ -820,15 +820,15 @@
         Wraps the C based pycatch22 implementation for aeon.
         (https://github.com/DynamicsAndNeuralSystems/pycatch22). This requires the
         ``pycatch22`` package to be installed if True.
     use_pyfftw : bool, default=True
         Whether to use the pyfftw library for FFT calculations. Requires the pyfftw
         package to be installed.
     save_transformed_data : bool, default=False
-        Save the data transformed in fit for use in _get_train_probs.
+        Save the data transformed in fit.
     random_state : int, RandomState instance or None, default=None
         If `int`, random_state is the seed used by the random number generator;
         If `RandomState` instance, random_state is the random number generator;
         If `None`, the random number generator is the `RandomState` instance used
         by `np.random`.
     n_jobs : int, default=1
         The number of jobs to run in parallel for both `fit` and `predict`.
@@ -877,18 +877,18 @@
 
     Examples
     --------
     >>> from tsml.interval_based import DrCIFRegressor
     >>> from tsml.utils.testing import generate_3d_test_data
     >>> X, y = generate_3d_test_data(n_samples=10, series_length=12,
     ...                              regression_target=True, random_state=0)
-    >>> reg = DrCIFRegressor(n_estimators=10, random_state=0)
-    >>> reg.fit(X, y)
+    >>> reg = DrCIFRegressor(n_estimators=10, random_state=0)  # doctest: +SKIP
+    >>> reg.fit(X, y)  # doctest: +SKIP
     DrCIFRegressor(...)
-    >>> reg.predict(X)
+    >>> reg.predict(X)  # doctest: +SKIP
     array([0.7252543 , 1.50132442, 0.95608366, 1.64399016, 0.42385504,
            0.60639322, 1.01919317, 1.30157483, 1.66017354, 0.2900776 ])
     """
 
     def __init__(
         self,
         base_estimator=None,
@@ -927,15 +927,15 @@
             row_slope,
             row_median,
             row_iqr,
             row_numba_min,
             row_numba_max,
         ]
 
-        super(DrCIFRegressor, self).__init__(
+        super().__init__(
             base_estimator=base_estimator,
             n_estimators=n_estimators,
             interval_selection_method="random",
             n_intervals=n_intervals,
             min_interval_length=min_interval_length,
             max_interval_length=max_interval_length,
             interval_features=interval_features,
```

### Comparing `tsml-0.3.0/tsml/interval_based/_interval_forest.py` & `tsml-0.4.0/tsml/interval_based/_interval_forest.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         "nan" will replace infinite values with NaNs. If None, do not replace NaNs.
     time_limit_in_minutes : int, default=0
         Time contract to limit build time in minutes, overriding n_estimators.
         Default of 0 means n_estimators are used.
     contract_max_n_estimators : int, default=500
         Max number of estimators when time_limit_in_minutes is set.
     save_transformed_data : bool, default=False
-        Save the data transformed in fit for use in _get_train_probs.
+        Save the data transformed in fit.
     random_state : int, RandomState instance or None, default=None
         If `int`, random_state is the seed used by the random number generator;
         If `RandomState` instance, random_state is the random number generator;
         If `None`, the random number generator is the `RandomState` instance used
         by `np.random`.
     n_jobs : int, default=1
         The number of jobs to run in parallel for both `fit` and `predict`.
@@ -192,15 +192,15 @@
         time_limit_in_minutes=None,
         contract_max_n_estimators=500,
         save_transformed_data=False,
         random_state=None,
         n_jobs=1,
         parallel_backend=None,
     ):
-        super(IntervalForestClassifier, self).__init__(
+        super().__init__(
             base_estimator=base_estimator,
             n_estimators=n_estimators,
             interval_selection_method=interval_selection_method,
             n_intervals=n_intervals,
             min_interval_length=min_interval_length,
             max_interval_length=max_interval_length,
             interval_features=interval_features,
@@ -331,15 +331,15 @@
         "nan" will replace infinite values with NaNs. If None, do not replace NaNs.
     time_limit_in_minutes : int, default=0
         Time contract to limit build time in minutes, overriding n_estimators.
         Default of 0 means n_estimators are used.
     contract_max_n_estimators : int, default=500
         Max number of estimators when time_limit_in_minutes is set.
     save_transformed_data : bool, default=False
-        Save the data transformed in fit for use in _get_train_probs.
+        Save the data transformed in fit.
     random_state : int, RandomState instance or None, default=None
         If `int`, random_state is the seed used by the random number generator;
         If `RandomState` instance, random_state is the random number generator;
         If `None`, the random number generator is the `RandomState` instance used
         by `np.random`.
     n_jobs : int, default=1
         The number of jobs to run in parallel for both `fit` and `predict`.
@@ -408,15 +408,15 @@
         time_limit_in_minutes=None,
         contract_max_n_estimators=500,
         save_transformed_data=False,
         random_state=None,
         n_jobs=1,
         parallel_backend=None,
     ):
-        super(IntervalForestRegressor, self).__init__(
+        super().__init__(
             base_estimator=base_estimator,
             n_estimators=n_estimators,
             interval_selection_method=interval_selection_method,
             n_intervals=n_intervals,
             min_interval_length=min_interval_length,
             max_interval_length=max_interval_length,
             interval_features=interval_features,
```

### Comparing `tsml-0.3.0/tsml/interval_based/_interval_pipelines.py` & `tsml-0.4.0/tsml/interval_based/_interval_pipelines.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/interval_based/_rise.py` & `tsml-0.4.0/tsml/interval_based/_rise.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         Default of 0 means n_estimators are used.
     contract_max_n_estimators : int, default=500
         Max number of estimators when time_limit_in_minutes is set.
     use_pyfftw : bool, default=True
         Whether to use the pyfftw library for FFT calculations. Requires the pyfftw
         package to be installed.
     save_transformed_data : bool, default=False
-        Save the data transformed in fit for use in _get_train_probs.
+        Save the data transformed in fit.
     random_state : int, RandomState instance or None, default=None
         If `int`, random_state is the seed used by the random number generator;
         If `RandomState` instance, random_state is the random number generator;
         If `None`, the random number generator is the `RandomState` instance used
         by `np.random`.
     n_jobs : int, default=1
         The number of jobs to run in parallel for both `fit` and `predict`.
@@ -123,18 +123,18 @@
        Ensembles", ACM Transactions on Knowledge and Data Engineering, 12(5): 2018
 
     Examples
     --------
     >>> from tsml.interval_based import RISEClassifier
     >>> from tsml.utils.testing import generate_3d_test_data
     >>> X, y = generate_3d_test_data(n_samples=10, series_length=12, random_state=0)
-    >>> clf = RISEClassifier(n_estimators=10, random_state=0)
-    >>> clf.fit(X, y)
+    >>> clf = RISEClassifier(n_estimators=10, random_state=0)  # doctest: +SKIP
+    >>> clf.fit(X, y)  # doctest: +SKIP
     RISEClassifier(...)
-    >>> clf.predict(X)
+    >>> clf.predict(X)  # doctest: +SKIP
     array([0, 1, 0, 1, 0, 0, 1, 1, 1, 0])
     """
 
     def __init__(
         self,
         base_estimator=None,
         n_estimators=200,
@@ -165,15 +165,15 @@
         interval_features = [
             PeriodogramTransformer(use_pyfftw=use_pyfftw, pad_with="mean"),
             AutocorrelationFunctionTransformer(
                 n_lags=acf_lag, min_values=acf_min_values
             ),
         ]
 
-        super(RISEClassifier, self).__init__(
+        super().__init__(
             base_estimator=base_estimator,
             n_estimators=n_estimators,
             interval_selection_method="random",
             n_intervals=1,
             min_interval_length=min_interval_length,
             max_interval_length=max_interval_length,
             interval_features=interval_features,
@@ -275,15 +275,15 @@
         Default of 0 means n_estimators are used.
     contract_max_n_estimators : int, default=500
         Max number of estimators when time_limit_in_minutes is set.
     use_pyfftw : bool, default=True
         Whether to use the pyfftw library for FFT calculations. Requires the pyfftw
         package to be installed.
     save_transformed_data : bool, default=False
-        Save the data transformed in fit for use in _get_train_probs.
+        Save the data transformed in fit.
     random_state : int, RandomState instance or None, default=None
         If `int`, random_state is the seed used by the random number generator;
         If `RandomState` instance, random_state is the random number generator;
         If `None`, the random number generator is the `RandomState` instance used
         by `np.random`.
     n_jobs : int, default=1
         The number of jobs to run in parallel for both `fit` and `predict`.
@@ -325,18 +325,18 @@
 
     Examples
     --------
     >>> from tsml.interval_based import RISERegressor
     >>> from tsml.utils.testing import generate_3d_test_data
     >>> X, y = generate_3d_test_data(n_samples=10, series_length=12,
     ...                              regression_target=True, random_state=0)
-    >>> reg = RISERegressor(n_estimators=10, random_state=0)
-    >>> reg.fit(X, y)
+    >>> reg = RISERegressor(n_estimators=10, random_state=0)  # doctest: +SKIP
+    >>> reg.fit(X, y)  # doctest: +SKIP
     RISERegressor(...)
-    >>> reg.predict(X)
+    >>> reg.predict(X)  # doctest: +SKIP
     array([0.7252543 , 1.50132442, 0.95608366, 1.64399016, 0.42385504,
            0.60639322, 1.01919317, 1.30157483, 1.66017354, 0.2900776 ])
     """
 
     def __init__(
         self,
         base_estimator=None,
@@ -363,15 +363,15 @@
         interval_features = [
             PeriodogramTransformer(use_pyfftw=use_pyfftw, pad_with="mean"),
             AutocorrelationFunctionTransformer(
                 n_lags=acf_lag, min_values=acf_min_values
             ),
         ]
 
-        super(RISERegressor, self).__init__(
+        super().__init__(
             base_estimator=base_estimator,
             n_estimators=n_estimators,
             interval_selection_method="random",
             n_intervals=1,
             min_interval_length=min_interval_length,
             max_interval_length=max_interval_length,
             interval_features=interval_features,
```

### Comparing `tsml-0.3.0/tsml/interval_based/_stsf.py` & `tsml-0.4.0/tsml/interval_based/_stsf.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         Default of 0 means n_estimators are used.
     contract_max_n_estimators : int, default=500
         Max number of estimators when time_limit_in_minutes is set.
     use_pyfftw : bool, default=True
         Whether to use the pyfftw library for FFT calculations. Requires the pyfftw
         package to be installed.
     save_transformed_data : bool, default=False
-        Save the data transformed in fit for use in _get_train_probs.
+        Save the data transformed in fit.
     random_state : int, RandomState instance or None, default=None
         If `int`, random_state is the seed used by the random number generator;
         If `RandomState` instance, random_state is the random number generator;
         If `None`, the random number generator is the `RandomState` instance used
         by `np.random`.
     n_jobs : int, default=1
         The number of jobs to run in parallel for both `fit` and `predict`.
@@ -122,18 +122,18 @@
        Through Supervised Interval Search." IEEE ICDM 2020
 
     Examples
     --------
     >>> from tsml.interval_based import STSFClassifier
     >>> from tsml.utils.testing import generate_3d_test_data
     >>> X, y = generate_3d_test_data(n_samples=10, series_length=12, random_state=0)
-    >>> clf = STSFClassifier(n_estimators=10, random_state=0)
-    >>> clf.fit(X, y)
+    >>> clf = STSFClassifier(n_estimators=10, random_state=0)  # doctest: +SKIP
+    >>> clf.fit(X, y)  # doctest: +SKIP
     STSFClassifier(...)
-    >>> clf.predict(X)
+    >>> clf.predict(X)  # doctest: +SKIP
     array([0, 1, 0, 1, 0, 0, 1, 1, 1, 0])
     """
 
     def __init__(
         self,
         base_estimator=None,
         n_estimators=200,
@@ -162,15 +162,15 @@
             row_slope,
             row_median,
             row_iqr,
             row_numba_min,
             row_numba_max,
         ]
 
-        super(STSFClassifier, self).__init__(
+        super().__init__(
             base_estimator=base_estimator,
             n_estimators=n_estimators,
             interval_selection_method="supervised",
             n_intervals=1,
             min_interval_length=min_interval_length,
             max_interval_length=np.inf,
             interval_features=interval_features,
@@ -269,18 +269,18 @@
         arXiv:2105.14876.
 
     Examples
     --------
     >>> from tsml.interval_based import RSTSFClassifier
     >>> from tsml.utils.testing import generate_3d_test_data
     >>> X, y = generate_3d_test_data(n_samples=10, series_length=12, random_state=0)
-    >>> clf = RSTSFClassifier(n_estimators=10, n_intervals=5, random_state=0)
-    >>> clf.fit(X, y)
+    >>> clf = RSTSFClassifier(n_estimators=10, n_intervals=5, random_state=0)  # doctest: +SKIP
+    >>> clf.fit(X, y)  # doctest: +SKIP
     RSTSFClassifier(...)
-    >>> clf.predict(X)
+    >>> clf.predict(X)  # doctest: +SKIP
     array([0, 1, 0, 1, 0, 0, 1, 1, 1, 0])
     """
 
     def __init__(
         self,
         n_estimators=200,
         n_intervals=50,
@@ -296,15 +296,15 @@
         self.random_state = random_state
         self.n_jobs = n_jobs
 
         if use_pyfftw:
             _check_optional_dependency("pyfftw", "pyfftw", self)
         _check_optional_dependency("statsmodels", "statsmodels", self)
 
-        super(RSTSFClassifier, self).__init__()
+        super().__init__()
 
     def fit(self, X: Union[np.ndarray, List[np.ndarray]], y: np.ndarray) -> object:
         """Fit the estimator to training data.
 
         Parameters
         ----------
         X : 3D np.ndarray of shape (n_instances, n_channels, n_timepoints)
```

### Comparing `tsml-0.3.0/tsml/interval_based/_tsf.py` & `tsml-0.4.0/tsml/interval_based/_tsf.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         Ignored for supervised interval_selection_method inputs.
     time_limit_in_minutes : int, default=0
         Time contract to limit build time in minutes, overriding n_estimators.
         Default of 0 means n_estimators are used.
     contract_max_n_estimators : int, default=500
         Max number of estimators when time_limit_in_minutes is set.
     save_transformed_data : bool, default=False
-        Save the data transformed in fit for use in _get_train_probs.
+        Save the data transformed in fit.
     random_state : int, RandomState instance or None, default=None
         If `int`, random_state is the seed used by the random number generator;
         If `RandomState` instance, random_state is the random number generator;
         If `None`, the random number generator is the `RandomState` instance used
         by `np.random`.
     n_jobs : int, default=1
         The number of jobs to run in parallel for both `fit` and `predict`.
@@ -162,15 +162,15 @@
         parallel_backend=None,
     ):
         if isinstance(base_estimator, CITClassifier):
             replace_nan = "nan"
         else:
             replace_nan = 0
 
-        super(TSFClassifier, self).__init__(
+        super().__init__(
             base_estimator=base_estimator,
             n_estimators=n_estimators,
             interval_selection_method="random",
             n_intervals=n_intervals,
             min_interval_length=min_interval_length,
             max_interval_length=max_interval_length,
             interval_features=None,
@@ -281,15 +281,15 @@
         as the number of series_transformers.
     time_limit_in_minutes : int, default=0
         Time contract to limit build time in minutes, overriding n_estimators.
         Default of 0 means n_estimators are used.
     contract_max_n_estimators : int, default=500
         Max number of estimators when time_limit_in_minutes is set.
     save_transformed_data : bool, default=False
-        Save the data transformed in fit for use in _get_train_probs.
+        Save the data transformed in fit.
     random_state : int, RandomState instance or None, default=None
         If `int`, random_state is the seed used by the random number generator;
         If `RandomState` instance, random_state is the random number generator;
         If `None`, the random number generator is the `RandomState` instance used
         by `np.random`.
     n_jobs : int, default=1
         The number of jobs to run in parallel for both `fit` and `predict`.
@@ -348,15 +348,15 @@
         time_limit_in_minutes=None,
         contract_max_n_estimators=500,
         save_transformed_data=False,
         random_state=None,
         n_jobs=1,
         parallel_backend=None,
     ):
-        super(TSFRegressor, self).__init__(
+        super().__init__(
             base_estimator=base_estimator,
             n_estimators=n_estimators,
             interval_selection_method="random",
             n_intervals=n_intervals,
             min_interval_length=min_interval_length,
             max_interval_length=max_interval_length,
             interval_features=None,
```

### Comparing `tsml-0.3.0/tsml/interval_based/tests/test_interval_forest.py` & `tsml-0.4.0/tsml/interval_based/tests/test_interval_forest.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/interval_based/tests/test_interval_pipelines.py` & `tsml-0.4.0/tsml/interval_based/tests/test_interval_pipelines.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/shapelet_based/__init__.py` & `tsml-0.4.0/tsml/shapelet_based/__init__.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/shapelet_based/_mrsqm.py` & `tsml-0.4.0/tsml/shapelet_based/_mrsqm.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/shapelet_based/_rdst.py` & `tsml-0.4.0/tsml/shapelet_based/_rdst.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/shapelet_based/_rsf.py` & `tsml-0.4.0/tsml/shapelet_based/_rsf.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/shapelet_based/_stc.py` & `tsml-0.4.0/tsml/shapelet_based/_stc.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,16 +56,15 @@
         and ``transform_limit_in_minutes``. The ``estimator`` will only be contracted if
         a ``time_limit_in_minutes parameter`` is present. Default of `0` means
         ``n_shapelet_samples`` or ``transform_limit_in_minutes`` is used.
     contract_max_n_shapelet_samples : int, default=np.inf
         Max number of shapelets to extract when contracting the transform with
         ``transform_limit_in_minutes`` or ``time_limit_in_minutes``.
     save_transformed_data : bool, default=False
-        Save the data transformed in fit in ``transformed_data_`` for use in
-        ``_get_train_probs``.
+        Save the data transformed in fit in ``transformed_data_``.
     n_jobs : int, default=1
         The number of jobs to run in parallel for both ``fit`` and ``predict``.
         `-1` means using all processors.
     batch_size : int or None, default=100
         Number of shapelet candidates processed before being merged into the set of best
         shapelets in the transform.
     random_state : int, RandomState instance or None, default=None
@@ -147,15 +146,15 @@
         self.contract_max_n_shapelet_samples = contract_max_n_shapelet_samples
         self.save_transformed_data = save_transformed_data
 
         self.random_state = random_state
         self.batch_size = batch_size
         self.n_jobs = n_jobs
 
-        super(ShapeletTransformClassifier, self).__init__()
+        super().__init__()
 
     def fit(self, X: Union[np.ndarray, List[np.ndarray]], y: np.ndarray) -> object:
         """Fit the estimator to training data.
 
         Parameters
         ----------
         X : 3D np.ndarray of shape (n_instances, n_channels, n_timepoints)
```

### Comparing `tsml-0.3.0/tsml/tests/test_estimator_checks.py` & `tsml-0.4.0/tsml/tests/test_estimator_checks.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/tests/test_estimators_sklearn.py` & `tsml-0.4.0/tsml/tests/test_estimators_sklearn.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/tests/test_interface.py` & `tsml-0.4.0/tsml/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/transformations/__init__.py` & `tsml-0.4.0/tsml/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/transformations/_acf.py` & `tsml-0.4.0/tsml/transformations/_acf.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/transformations/_ar_coefficient.py` & `tsml-0.4.0/tsml/transformations/_ar_coefficient.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/transformations/_catch22.py` & `tsml-0.4.0/tsml/transformations/_catch22.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/transformations/_fpca.py` & `tsml-0.4.0/tsml/transformations/_fpca.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/transformations/_function_transformer.py` & `tsml-0.4.0/tsml/transformations/_function_transformer.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/transformations/_interval_extraction.py` & `tsml-0.4.0/tsml/transformations/_interval_extraction.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/transformations/_periodogram.py` & `tsml-0.4.0/tsml/transformations/_periodogram.py`

 * *Files 11% similar despite different names*

```diff
@@ -36,18 +36,18 @@
 
     Examples
     --------
     >>> from tsml.transformations import PeriodogramTransformer
     >>> from tsml.utils.testing import generate_3d_test_data
     >>> X, _ = generate_3d_test_data(n_samples=4, n_channels=2, series_length=20,
     ...                              random_state=0)
-    >>> tnf = PeriodogramTransformer()
-    >>> tnf.fit(X)
+    >>> tnf = PeriodogramTransformer()  # doctest: +SKIP
+    >>> tnf.fit(X)  # doctest: +SKIP
     PeriodogramTransformer(...)
-    >>> print(tnf.transform(X)[0])
+    >>> print(tnf.transform(X)[0])  # doctest: +SKIP
     [[22.16456597 11.08122685  3.69018936  2.17665255  5.27387039  3.10598557
        6.311107    1.70468284  1.8269671   0.88838033  1.56747869  3.42037058
        1.67988661  1.71142437  3.49821716  1.25120108]
      [22.71382067  8.64933688  6.36412194  0.9298486   5.70358068  2.70669743
        4.33906385  0.36544821  2.28769936  3.67702091  1.45018642  1.26838712
        3.36395549  2.69146494  2.27041859  3.9023142 ]]
     """
@@ -65,15 +65,15 @@
         self.pad_with = pad_with
         self.constant_value = constant_value
         self.n_jobs = n_jobs
 
         if use_pyfftw:
             _check_optional_dependency("pyfftw", "pyfftw", self)
 
-        super(PeriodogramTransformer, self).__init__()
+        super().__init__()
 
     def fit(self, X, y=None):
         self._validate_data(X=X)
         return self
 
     def transform(self, X, y=None):
         X = self._validate_data(X=X, reset=False)
```

### Comparing `tsml-0.3.0/tsml/transformations/_quantile.py` & `tsml-0.4.0/tsml/transformations/_quantile.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/transformations/_sfa.py` & `tsml-0.4.0/tsml/transformations/_sfa.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/transformations/_shapelet_transform.py` & `tsml-0.4.0/tsml/transformations/_shapelet_transform.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/transformations/_summary_features.py` & `tsml-0.4.0/tsml/transformations/_summary_features.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/transformations/_transform_concatenator.py` & `tsml-0.4.0/tsml/transformations/_transform_concatenator.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/transformations/tests/test_function_transformer.py` & `tsml-0.4.0/tsml/transformations/tests/test_function_transformer.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/transformations/tests/test_interval_extraction.py` & `tsml-0.4.0/tsml/transformations/tests/test_interval_extraction.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/transformations/tests/test_transform_concatenator.py` & `tsml-0.4.0/tsml/transformations/tests/test_transform_concatenator.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/utils/_tags.py` & `tsml-0.4.0/tsml/utils/_tags.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/utils/discovery.py` & `tsml-0.4.0/tsml/utils/discovery.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/utils/numba_functions/general.py` & `tsml-0.4.0/tsml/utils/numba_functions/general.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/utils/numba_functions/stats.py` & `tsml-0.4.0/tsml/utils/numba_functions/stats.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/utils/testing.py` & `tsml-0.4.0/tsml/utils/testing.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/utils/validation.py` & `tsml-0.4.0/tsml/utils/validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -541,14 +541,15 @@
     return X
 
 
 def _check_optional_dependency(
     package_name: str,
     package_import_name: str,
     source_name: Union[str, BaseEstimator],
+    raise_error: bool = True,
 ):
     """Check if an optional dependency is installed and raise error if not.
 
     If the dependency is installed but the version is outdated, a warning is raised.
 
     Parameters
     ----------
@@ -558,28 +559,38 @@
     package_import_name : str
         The import name of the package. i.e. for the package `scikit-learn` the import
         name is `sklearn`, while for the package `tsfresh` the import name is the same
         as the package name `tsfresh`.
     source_name : str or BaseEstimator
         Source of the check i.e. an estimator or function. If a BaseEstimator is passed
         the class name of the estimator is used.
+    raise_error : bool, default=True
+        Whether to raise an error if the dependency is not installed.
+
+    Returns
+    -------
+    is_installed : bool
+        True if the dependency is installed and matches the specified version and
+        False otherwise.
 
     Raises
     ------
     ModuleNotFoundError
-        Error with informative message, asking to install required the dependency.
+        Error with informative message, asking to install required the dependency
+        if raise_error.
 
     Examples
     --------
     >>> from tsml.utils.validation import _check_optional_dependency
     >>> _check_optional_dependency(
     ...     "scikit-learn",
     ...     "sklearn",
     ...     "_check_optional_dependency",
     ... )
+    True
     """
     if isinstance(source_name, BaseEstimator):
         source_name = source_name.__class__.__name__
 
     try:
         req = Requirement(package_name)
     except InvalidRequirement:
@@ -592,23 +603,29 @@
     package_version_req = req.specifier
 
     try:
         # attempt to import package
         pkg_ref = import_module(package_import_name)
     except ModuleNotFoundError as e:
         # package cannot be imported
-        raise ModuleNotFoundError(
-            f'{source_name} has an optional dependency and requires "{package_name}" '
-            f'to be installed. Run: "pip install {package_name}" or "pip install '
-            f'tsml[extras]" to install all optional dependencies.'
-        ) from e
+        if raise_error:
+            raise ModuleNotFoundError(
+                f'{source_name} has an optional dependency and requires "{package_name}" '
+                f'to be installed. Run: "pip install {package_name}" or "pip install '
+                f'tsml[extras]" to install all optional dependencies.'
+            ) from e
+        else:
+            return False
 
     # check installed version is compatible
     if package_version_req != SpecifierSet(""):
         pkg_env_version = pkg_ref.__version__
 
         if pkg_env_version not in package_version_req:
             warnings.warn(
                 f'{source_name} requires "{package_name}", but found version '
                 f"{pkg_env_version}.",
                 stacklevel=2,
             )
+            return False
+
+    return True
```

### Comparing `tsml-0.3.0/tsml/vector/_cit.py` & `tsml-0.4.0/tsml/vector/_cit.py`

 * *Files identical despite different names*

### Comparing `tsml-0.3.0/tsml/vector/_rotation_forest.py` & `tsml-0.4.0/tsml/vector/_rotation_forest.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,16 +51,15 @@
         `DecisionTreeClassifier` using entropy as a splitting measure.
     time_limit_in_minutes : int, default=0
         Time contract to limit build time in minutes, overriding ``n_estimators``.
         Default of `0` means ``n_estimators`` is used.
     contract_max_n_estimators : int, default=500
         Max number of estimators to build when ``time_limit_in_minutes`` is set.
     save_transformed_data : bool, default=False
-        Save the data transformed in fit in ``transformed_data_`` for use in
-        ``_get_train_probs``.
+        Save the data transformed in fit in ``transformed_data_``.
     n_jobs : int, default=1
         The number of jobs to run in parallel for both ``fit`` and ``predict``.
         `-1` means using all processors.
     random_state : int, RandomState instance or None, default=None
         If `int`, random_state is the seed used by the random number generator;
         If `RandomState` instance, random_state is the random number generator;
         If `None`, the random number generator is the `RandomState` instance used
@@ -131,15 +130,15 @@
         self.base_estimator = base_estimator
         self.time_limit_in_minutes = time_limit_in_minutes
         self.contract_max_n_estimators = contract_max_n_estimators
         self.save_transformed_data = save_transformed_data
         self.n_jobs = n_jobs
         self.random_state = random_state
 
-        super(RotationForestClassifier, self).__init__()
+        super().__init__()
 
     def fit(self, X: Union[np.ndarray, pd.DataFrame], y: np.ndarray) -> object:
         """Fit the estimator to training data.
 
         Parameters
         ----------
         X : 2d ndarray or DataFrame of shape (n_instances, n_atts)
@@ -300,61 +299,14 @@
         )
 
         output = np.sum(y_probas, axis=0) / (
             np.ones(self.n_classes_) * self._n_estimators
         )
         return output
 
-    def _get_train_probs(self, X, y):
-        check_is_fitted(self)
-
-        # treat case of single class seen in fit
-        if self.n_classes_ == 1:
-            np.repeat([[1]], len(X), axis=0)
-
-        if isinstance(X, np.ndarray) and len(X.shape) == 3 and X.shape[1] == 1:
-            X = np.reshape(X, (X.shape[0], -1))
-
-        X = self._validate_data(X=X, reset=False)
-
-        n_instances, n_atts = X.shape
-
-        if n_instances != self.n_instances_ or n_atts != self.n_atts_:
-            raise ValueError(
-                "n_instances, n_atts mismatch. X should be the same as the training "
-                "data used in fit for generating train probabilities."
-            )
-
-        if not self.save_transformed_data:
-            raise ValueError("Currently only works with saved transform data from fit.")
-
-        p = Parallel(n_jobs=self._n_jobs)(
-            delayed(self._train_probas_for_estimator)(
-                y,
-                i,
-            )
-            for i in range(self._n_estimators)
-        )
-        y_probas, oobs = zip(*p)
-
-        results = np.sum(y_probas, axis=0)
-        divisors = np.zeros(n_instances)
-        for oob in oobs:
-            for inst in oob:
-                divisors[inst] += 1
-
-        for i in range(n_instances):
-            results[i] = (
-                np.ones(self.n_classes_) * (1 / self.n_classes_)
-                if divisors[i] == 0
-                else results[i] / (np.ones(self.n_classes_) * divisors[i])
-            )
-
-        return results
-
     def _fit_estimator(self, X, X_cls_split, y, idx):
         rs = 255 if self.random_state == 0 else self.random_state
         rs = (
             None
             if self.random_state is None
             else (rs * 37 * (idx + 1)) % np.iinfo(np.int32).max
         )
@@ -516,16 +468,15 @@
         `DecisionTreeRegressor` using squared error as a splitting measure.
     time_limit_in_minutes : int, default=0
         Time contract to limit build time in minutes, overriding ``n_estimators``.
         Default of `0` means ``n_estimators`` is used.
     contract_max_n_estimators : int, default=500
         Max number of estimators to build when ``time_limit_in_minutes`` is set.
     save_transformed_data : bool, default=False
-        Save the data transformed in fit in ``transformed_data_`` for use in
-        ``_get_train_probs``.
+        Save the data transformed in fit in ``transformed_data_``.
     n_jobs : int, default=1
         The number of jobs to run in parallel for both ``fit`` and ``predict``.
         `-1` means using all processors.
     random_state : int, RandomState instance or None, default=None
         If `int`, random_state is the seed used by the random number generator;
         If `RandomState` instance, random_state is the random number generator;
         If `None`, the random number generator is the `RandomState` instance used
@@ -586,15 +537,15 @@
         self.base_estimator = base_estimator
         self.time_limit_in_minutes = time_limit_in_minutes
         self.contract_max_n_estimators = contract_max_n_estimators
         self.save_transformed_data = save_transformed_data
         self.n_jobs = n_jobs
         self.random_state = random_state
 
-        super(RotationForestRegressor, self).__init__()
+        super().__init__()
 
     def fit(self, X: Union[np.ndarray, pd.DataFrame], y: np.ndarray) -> object:
         """Fit the estimator to training data.
 
         Parameters
         ----------
         X : 2d ndarray or DataFrame of shape (n_instances, n_atts)
@@ -805,15 +756,15 @@
         params : dict or list of dict
             Parameters to create testing instances of the class.
         """
         return {"n_estimators": 2}
 
 
 def _generate_groups(rng, n_atts, min_group, max_group):
-    permutation = rng.permutation((np.arange(0, n_atts)))
+    permutation = rng.permutation(np.arange(0, n_atts))
 
     # select the size of each group.
     group_size_count = np.zeros(max_group - min_group + 1)
     n_attributes = 0
     n_groups = 0
     while n_attributes < n_atts:
         n = rng.randint(group_size_count.shape[0])
```

### Comparing `tsml-0.3.0/tsml.egg-info/PKG-INFO` & `tsml-0.4.0/tsml.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsml
-Version: 0.3.0
+Version: 0.4.0
 Summary: A toolkit for time series machine learning algorithms.
 Author-email: Matthew Middlehurst <m.b.middlehurst@soton.ac.uk>
 Maintainer-email: Matthew Middlehurst <m.b.middlehurst@soton.ac.uk>
 License: BSD 3-Clause License
         
         Copyright (c) The Time Series Machine Learning (tsml) developers.
         All rights reserved.
@@ -45,46 +45,47 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: <3.12,>=3.8
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: <3.13,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numba>=0.55.0
 Requires-Dist: numpy>=1.21.0
 Requires-Dist: pandas>=1.5.3
 Requires-Dist: scikit-learn>=1.0.0
 Requires-Dist: packaging>=20.0
 Provides-Extra: all-extras
-Requires-Dist: pyfftw>=0.12.0; extra == "all-extras"
-Requires-Dist: statsmodels>=0.12.1; extra == "all-extras"
-Requires-Dist: wildboar>=1.1.0; extra == "all-extras"
+Requires-Dist: grailts; extra == "all-extras"
 Requires-Dist: scikit-fda>=0.7.0; extra == "all-extras"
+Requires-Dist: statsmodels>=0.12.1; extra == "all-extras"
 Requires-Dist: stumpy>=1.6.0; extra == "all-extras"
-Requires-Dist: grailts; extra == "all-extras"
+Requires-Dist: wildboar>=1.1.0; extra == "all-extras"
 Requires-Dist: fdasrsf<=2.5.2; extra == "all-extras"
 Provides-Extra: unstable-extras
-Requires-Dist: mrsqm>=0.0.1; platform_system == "Darwin" and extra == "unstable-extras"
+Requires-Dist: mrsqm>=0.0.1; (platform_system == "Darwin" and python_version < "3.12") and extra == "unstable-extras"
 Requires-Dist: pycatch22<=0.4.3; extra == "unstable-extras"
+Requires-Dist: pyfftw>=0.12.0; python_version < "3.12" and extra == "unstable-extras"
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-randomly; extra == "dev"
 Requires-Dist: pytest-timeout; extra == "dev"
-Requires-Dist: pytest-xdist; extra == "dev"
+Requires-Dist: pytest-xdist[psutil]; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-rerunfailures; extra == "dev"
 Provides-Extra: binder
 Requires-Dist: notebook; extra == "binder"
 Requires-Dist: jupyterlab; extra == "binder"
 Provides-Extra: docs
-Requires-Dist: sphinx<8.0.0; extra == "docs"
+Requires-Dist: sphinx<7.3.0; extra == "docs"
 Requires-Dist: sphinx-design; extra == "docs"
 Requires-Dist: sphinx-version-warning; extra == "docs"
 Requires-Dist: sphinx_issues; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Requires-Dist: sphinx-remove-toctrees; extra == "docs"
 Requires-Dist: sphinxext-opengraph; extra == "docs"
 Requires-Dist: nbsphinx; extra == "docs"
@@ -104,15 +105,20 @@
 [![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![license](https://img.shields.io/badge/license-BSD%203--Clause-green?logo=style)](https://github.com/time-series-machine-learning/tsml-py/blob/main/LICENSE)
 
 # tsml-py
 
 A toolkit for time series machine learning algorithms.
 
-The current release of `tsml` is v0.3.0.
+Please see [`tsml_eval`](https://github.com/time-series-machine-learning/tsml-eval) and
+[`aeon`](https://github.com/aeon-toolkit/aeon) for more developed packages. This package
+is more of a sandbox for testing out new ideas and algorithms. It may contain some
+algorithms and implementations that are not available in the other toolkits.
+
+The current release of `tsml` is v0.4.0.
 
 ## Installation
 
 `tsml` is available on PyPI and can be installed via pip:
 
 ```console
 pip install tsml
```

### Comparing `tsml-0.3.0/tsml.egg-info/SOURCES.txt` & `tsml-0.4.0/tsml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

