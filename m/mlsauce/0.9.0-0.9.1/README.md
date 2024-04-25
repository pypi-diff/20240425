# Comparing `tmp/mlsauce-0.9.0.tar.gz` & `tmp/mlsauce-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlsauce-0.9.0.tar", last modified: Mon Dec 25 21:00:21 2023, max compression
+gzip compressed data, was "mlsauce-0.9.1.tar", last modified: Tue Dec 26 19:08:12 2023, max compression
```

## Comparing `mlsauce-0.9.0.tar` & `mlsauce-0.9.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-12-25 21:00:21.897077 mlsauce-0.9.0/
--rw-r--r--   0 codespace  (1000) codespace  (1000)      967 2023-12-25 21:00:21.897077 mlsauce-0.9.0/PKG-INFO
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-12-25 21:00:21.889077 mlsauce-0.9.0/mlsauce/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-12-25 21:00:21.893077 mlsauce-0.9.0/mlsauce/__check_build/
--rw-rw-rw-   0 codespace  (1000) root         (0)     1711 2023-11-19 05:42:36.341667 mlsauce-0.9.0/mlsauce/__check_build/__init__.py
--rw-rw-rw-   0 codespace  (1000) root         (0)       29 2023-11-19 05:42:36.349667 mlsauce-0.9.0/mlsauce/__check_build/_check_build.pyx
--rw-rw-rw-   0 codespace  (1000) root         (0)      552 2023-11-19 05:42:36.349667 mlsauce-0.9.0/mlsauce/__check_build/setup.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3158 2023-12-25 20:17:03.729178 mlsauce-0.9.0/mlsauce/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-12-25 21:00:21.893077 mlsauce-0.9.0/mlsauce/_build_utils/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3670 2023-12-25 20:17:03.729178 mlsauce-0.9.0/mlsauce/_build_utils/__init__.py
--rw-rw-rw-   0 codespace  (1000) root         (0)     3957 2023-11-19 05:42:36.349667 mlsauce-0.9.0/mlsauce/_build_utils/openmp_helpers.py
--rw-rw-rw-   0 codespace  (1000) root         (0)     2175 2023-11-19 05:42:36.349667 mlsauce-0.9.0/mlsauce/_build_utils/pre_build_helpers.py
--rw-rw-rw-   0 codespace  (1000) root         (0)     5149 2023-11-19 05:42:36.349667 mlsauce-0.9.0/mlsauce/_config.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-12-25 21:00:21.893077 mlsauce-0.9.0/mlsauce/adaopt/
--rw-rw-rw-   0 codespace  (1000) root         (0)       50 2023-11-19 05:42:36.349667 mlsauce-0.9.0/mlsauce/adaopt/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10782 2023-12-25 20:17:03.729178 mlsauce-0.9.0/mlsauce/adaopt/_adaopt.py
--rw-rw-rw-   0 codespace  (1000) root         (0)    22717 2023-11-19 05:42:36.353667 mlsauce-0.9.0/mlsauce/adaopt/_adaoptc.pyx
--rw-rw-rw-   0 codespace  (1000) root         (0)      578 2023-11-19 05:42:36.353667 mlsauce-0.9.0/mlsauce/adaopt/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-12-25 21:00:21.893077 mlsauce-0.9.0/mlsauce/booster/
--rw-rw-rw-   0 codespace  (1000) root         (0)      153 2023-11-19 05:42:36.353667 mlsauce-0.9.0/mlsauce/booster/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5455 2023-12-25 20:17:03.741178 mlsauce-0.9.0/mlsauce/booster/_booster_classifier.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4940 2023-12-25 20:17:03.741178 mlsauce-0.9.0/mlsauce/booster/_booster_regressor.py
--rw-rw-rw-   0 codespace  (1000) root         (0)    11541 2023-11-19 05:42:36.357667 mlsauce-0.9.0/mlsauce/booster/_boosterc.pyx
--rw-rw-rw-   0 codespace  (1000) root         (0)      581 2023-11-19 05:42:36.357667 mlsauce-0.9.0/mlsauce/booster/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-12-25 21:00:21.893077 mlsauce-0.9.0/mlsauce/datasets/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       53 2023-12-25 20:17:03.749178 mlsauce-0.9.0/mlsauce/datasets/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      285 2023-12-25 20:17:03.749178 mlsauce-0.9.0/mlsauce/datasets/dowload.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-12-25 21:00:21.893077 mlsauce-0.9.0/mlsauce/encoders/
--rw-rw-rw-   0 codespace  (1000) root         (0)       82 2023-11-19 05:42:36.361667 mlsauce-0.9.0/mlsauce/encoders/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2228 2023-12-25 20:17:03.749178 mlsauce-0.9.0/mlsauce/encoders/target_encoders.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-12-25 21:00:21.893077 mlsauce-0.9.0/mlsauce/lasso/
--rw-rw-rw-   0 codespace  (1000) root         (0)       65 2023-11-19 05:42:36.361667 mlsauce-0.9.0/mlsauce/lasso/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5078 2023-12-25 20:17:03.749178 mlsauce-0.9.0/mlsauce/lasso/_lasso.py
--rw-rw-rw-   0 codespace  (1000) root         (0)     9010 2023-11-19 05:42:36.365666 mlsauce-0.9.0/mlsauce/lasso/_lassoc.pyx
--rw-rw-rw-   0 codespace  (1000) root         (0)      575 2023-11-19 05:42:36.365666 mlsauce-0.9.0/mlsauce/lasso/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-12-25 21:00:21.893077 mlsauce-0.9.0/mlsauce/ridge/
--rw-rw-rw-   0 codespace  (1000) root         (0)       65 2023-11-19 05:42:36.365666 mlsauce-0.9.0/mlsauce/ridge/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3517 2023-12-25 20:17:03.757178 mlsauce-0.9.0/mlsauce/ridge/_ridge.py
--rw-rw-rw-   0 codespace  (1000) root         (0)     6470 2023-11-19 05:42:36.369667 mlsauce-0.9.0/mlsauce/ridge/_ridgec.pyx
--rw-rw-rw-   0 codespace  (1000) root         (0)      575 2023-11-19 05:42:36.369667 mlsauce-0.9.0/mlsauce/ridge/setup.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1559 2023-12-25 20:17:03.761178 mlsauce-0.9.0/mlsauce/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-12-25 21:00:21.897077 mlsauce-0.9.0/mlsauce/stump/
--rw-rw-rw-   0 codespace  (1000) root         (0)       78 2023-11-19 05:42:36.369667 mlsauce-0.9.0/mlsauce/stump/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2549 2023-12-25 20:17:03.761178 mlsauce-0.9.0/mlsauce/stump/_stump_classifier.py
--rw-rw-rw-   0 codespace  (1000) root         (0)     6887 2023-11-19 05:42:36.373667 mlsauce-0.9.0/mlsauce/stump/_stumpc.pyx
--rw-rw-rw-   0 codespace  (1000) root         (0)      575 2023-11-19 05:42:36.373667 mlsauce-0.9.0/mlsauce/stump/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-12-25 21:00:21.897077 mlsauce-0.9.0/mlsauce/tests/
--rw-rw-rw-   0 codespace  (1000) root         (0)       37 2023-11-19 05:42:36.373667 mlsauce-0.9.0/mlsauce/tests/__init__.py
--rw-rw-rw-   0 codespace  (1000) root         (0)      387 2023-11-19 05:42:36.373667 mlsauce-0.9.0/mlsauce/tests/test_adaopt.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-12-25 21:00:21.897077 mlsauce-0.9.0/mlsauce/utils/
--rw-rw-rw-   0 codespace  (1000) root         (0)      196 2023-11-19 05:42:36.373667 mlsauce-0.9.0/mlsauce/utils/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-12-25 21:00:21.897077 mlsauce-0.9.0/mlsauce/utils/memoryuse/
--rw-rw-rw-   0 codespace  (1000) root         (0)       72 2023-11-19 05:42:36.373667 mlsauce-0.9.0/mlsauce/utils/memoryuse/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2338 2023-12-25 20:17:03.769178 mlsauce-0.9.0/mlsauce/utils/memoryuse/mem_usage.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-12-25 21:00:21.897077 mlsauce-0.9.0/mlsauce/utils/misc/
--rw-rw-rw-   0 codespace  (1000) root         (0)      132 2023-11-19 05:42:36.373667 mlsauce-0.9.0/mlsauce/utils/misc/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      694 2023-12-25 20:17:03.769178 mlsauce-0.9.0/mlsauce/utils/misc/misc.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-12-25 21:00:21.897077 mlsauce-0.9.0/mlsauce/utils/sampling/
--rw-rw-rw-   0 codespace  (1000) root         (0)       64 2023-11-19 05:42:36.373667 mlsauce-0.9.0/mlsauce/utils/sampling/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3169 2023-12-25 20:17:03.769178 mlsauce-0.9.0/mlsauce/utils/sampling/rowsubsampling.py
--rw-rw-rw-   0 codespace  (1000) root         (0)      352 2023-11-19 05:42:36.373667 mlsauce-0.9.0/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11531 2023-12-25 20:17:03.777178 mlsauce-0.9.0/setup.py
+drwxr-xr-x   0 t          (501) staff       (20)        0 2023-12-26 19:08:12.890536 mlsauce-0.9.1/
+-rw-r--r--   0 t          (501) staff       (20)      975 2023-12-26 19:08:12.890168 mlsauce-0.9.1/PKG-INFO
+drwxr-xr-x   0 t          (501) staff       (20)        0 2023-12-26 19:08:12.867673 mlsauce-0.9.1/mlsauce/
+drwxr-xr-x   0 t          (501) staff       (20)        0 2023-12-26 19:08:12.869148 mlsauce-0.9.1/mlsauce/__check_build/
+-rw-r--r--   0 t          (501) staff       (20)     1711 2023-12-26 00:36:40.701139 mlsauce-0.9.1/mlsauce/__check_build/__init__.py
+-rw-r--r--   0 t          (501) staff       (20)       29 2023-12-26 00:36:40.718343 mlsauce-0.9.1/mlsauce/__check_build/_check_build.pyx
+-rw-r--r--   0 t          (501) staff       (20)      552 2023-12-26 00:36:40.719093 mlsauce-0.9.1/mlsauce/__check_build/setup.py
+-rw-r--r--   0 t          (501) staff       (20)     3158 2023-12-26 00:36:40.720236 mlsauce-0.9.1/mlsauce/__init__.py
+drwxr-xr-x   0 t          (501) staff       (20)        0 2023-12-26 19:08:12.870517 mlsauce-0.9.1/mlsauce/_build_utils/
+-rw-r--r--   0 t          (501) staff       (20)     3670 2023-12-26 00:36:40.721265 mlsauce-0.9.1/mlsauce/_build_utils/__init__.py
+-rw-r--r--   0 t          (501) staff       (20)     3957 2023-12-26 00:36:40.722083 mlsauce-0.9.1/mlsauce/_build_utils/openmp_helpers.py
+-rw-r--r--   0 t          (501) staff       (20)     2175 2023-12-26 00:36:40.723434 mlsauce-0.9.1/mlsauce/_build_utils/pre_build_helpers.py
+-rw-r--r--   0 t          (501) staff       (20)     5149 2023-12-26 00:36:40.724499 mlsauce-0.9.1/mlsauce/_config.py
+drwxr-xr-x   0 t          (501) staff       (20)        0 2023-12-26 19:08:12.872591 mlsauce-0.9.1/mlsauce/adaopt/
+-rw-r--r--   0 t          (501) staff       (20)       50 2023-12-26 00:36:40.725629 mlsauce-0.9.1/mlsauce/adaopt/__init__.py
+-rw-r--r--   0 t          (501) staff       (20)    10782 2023-12-26 00:36:40.726543 mlsauce-0.9.1/mlsauce/adaopt/_adaopt.py
+-rw-r--r--   0 t          (501) staff       (20)    22717 2023-12-26 00:36:40.739306 mlsauce-0.9.1/mlsauce/adaopt/_adaoptc.pyx
+-rw-r--r--   0 t          (501) staff       (20)      578 2023-12-26 00:36:40.739881 mlsauce-0.9.1/mlsauce/adaopt/setup.py
+drwxr-xr-x   0 t          (501) staff       (20)        0 2023-12-26 19:08:12.875078 mlsauce-0.9.1/mlsauce/booster/
+-rw-r--r--   0 t          (501) staff       (20)      153 2023-12-26 00:36:40.740316 mlsauce-0.9.1/mlsauce/booster/__init__.py
+-rw-r--r--   0 t          (501) staff       (20)     5455 2023-12-26 00:36:40.740732 mlsauce-0.9.1/mlsauce/booster/_booster_classifier.py
+-rw-r--r--   0 t          (501) staff       (20)     4940 2023-12-26 00:36:40.741194 mlsauce-0.9.1/mlsauce/booster/_booster_regressor.py
+-rw-r--r--   0 t          (501) staff       (20)    11541 2023-12-26 00:36:40.797129 mlsauce-0.9.1/mlsauce/booster/_boosterc.pyx
+-rw-r--r--   0 t          (501) staff       (20)      581 2023-12-26 00:36:40.804534 mlsauce-0.9.1/mlsauce/booster/setup.py
+drwxr-xr-x   0 t          (501) staff       (20)        0 2023-12-26 19:08:12.876036 mlsauce-0.9.1/mlsauce/datasets/
+-rw-r--r--   0 t          (501) staff       (20)       53 2023-12-26 00:36:40.805612 mlsauce-0.9.1/mlsauce/datasets/__init__.py
+-rw-r--r--   0 t          (501) staff       (20)      285 2023-12-26 00:36:40.806235 mlsauce-0.9.1/mlsauce/datasets/dowload.py
+drwxr-xr-x   0 t          (501) staff       (20)        0 2023-12-26 19:08:12.877069 mlsauce-0.9.1/mlsauce/encoders/
+-rw-r--r--   0 t          (501) staff       (20)       82 2023-12-26 00:36:40.855856 mlsauce-0.9.1/mlsauce/encoders/__init__.py
+-rw-r--r--   0 t          (501) staff       (20)     2228 2023-12-26 00:36:40.858305 mlsauce-0.9.1/mlsauce/encoders/target_encoders.py
+drwxr-xr-x   0 t          (501) staff       (20)        0 2023-12-26 19:08:12.879103 mlsauce-0.9.1/mlsauce/lasso/
+-rw-r--r--   0 t          (501) staff       (20)       65 2023-12-26 00:36:40.859353 mlsauce-0.9.1/mlsauce/lasso/__init__.py
+-rw-r--r--   0 t          (501) staff       (20)     5078 2023-12-26 00:36:40.860283 mlsauce-0.9.1/mlsauce/lasso/_lasso.py
+-rw-r--r--   0 t          (501) staff       (20)     9010 2023-12-26 00:36:40.898787 mlsauce-0.9.1/mlsauce/lasso/_lassoc.pyx
+-rw-r--r--   0 t          (501) staff       (20)      575 2023-12-26 00:36:40.906560 mlsauce-0.9.1/mlsauce/lasso/setup.py
+drwxr-xr-x   0 t          (501) staff       (20)        0 2023-12-26 19:08:12.881209 mlsauce-0.9.1/mlsauce/ridge/
+-rw-r--r--   0 t          (501) staff       (20)       65 2023-12-26 00:36:40.907747 mlsauce-0.9.1/mlsauce/ridge/__init__.py
+-rw-r--r--   0 t          (501) staff       (20)     3517 2023-12-26 00:36:40.914587 mlsauce-0.9.1/mlsauce/ridge/_ridge.py
+-rw-r--r--   0 t          (501) staff       (20)     6470 2023-12-26 00:36:40.941092 mlsauce-0.9.1/mlsauce/ridge/_ridgec.pyx
+-rw-r--r--   0 t          (501) staff       (20)      575 2023-12-26 00:36:40.941711 mlsauce-0.9.1/mlsauce/ridge/setup.py
+-rw-r--r--   0 t          (501) staff       (20)     1559 2023-12-26 00:36:40.943991 mlsauce-0.9.1/mlsauce/setup.py
+drwxr-xr-x   0 t          (501) staff       (20)        0 2023-12-26 19:08:12.883473 mlsauce-0.9.1/mlsauce/stump/
+-rw-r--r--   0 t          (501) staff       (20)       78 2023-12-26 00:36:40.944995 mlsauce-0.9.1/mlsauce/stump/__init__.py
+-rw-r--r--   0 t          (501) staff       (20)     2549 2023-12-26 00:36:40.945688 mlsauce-0.9.1/mlsauce/stump/_stump_classifier.py
+-rw-r--r--   0 t          (501) staff       (20)     6887 2023-12-26 00:36:40.991182 mlsauce-0.9.1/mlsauce/stump/_stumpc.pyx
+-rw-r--r--   0 t          (501) staff       (20)      575 2023-12-26 00:36:40.991738 mlsauce-0.9.1/mlsauce/stump/setup.py
+drwxr-xr-x   0 t          (501) staff       (20)        0 2023-12-26 19:08:12.884504 mlsauce-0.9.1/mlsauce/tests/
+-rw-r--r--   0 t          (501) staff       (20)       37 2023-12-26 00:36:40.992457 mlsauce-0.9.1/mlsauce/tests/__init__.py
+-rw-r--r--   0 t          (501) staff       (20)      387 2023-12-26 00:36:40.992972 mlsauce-0.9.1/mlsauce/tests/test_adaopt.py
+drwxr-xr-x   0 t          (501) staff       (20)        0 2023-12-26 19:08:12.885261 mlsauce-0.9.1/mlsauce/utils/
+-rw-r--r--   0 t          (501) staff       (20)      196 2023-12-26 00:36:40.993986 mlsauce-0.9.1/mlsauce/utils/__init__.py
+drwxr-xr-x   0 t          (501) staff       (20)        0 2023-12-26 19:08:12.886834 mlsauce-0.9.1/mlsauce/utils/memoryuse/
+-rw-r--r--   0 t          (501) staff       (20)       72 2023-12-26 00:36:40.994914 mlsauce-0.9.1/mlsauce/utils/memoryuse/__init__.py
+-rw-r--r--   0 t          (501) staff       (20)     2338 2023-12-26 00:36:40.995327 mlsauce-0.9.1/mlsauce/utils/memoryuse/mem_usage.py
+drwxr-xr-x   0 t          (501) staff       (20)        0 2023-12-26 19:08:12.888010 mlsauce-0.9.1/mlsauce/utils/misc/
+-rw-r--r--   0 t          (501) staff       (20)      132 2023-12-26 00:36:40.996171 mlsauce-0.9.1/mlsauce/utils/misc/__init__.py
+-rw-r--r--   0 t          (501) staff       (20)      694 2023-12-26 00:36:40.996717 mlsauce-0.9.1/mlsauce/utils/misc/misc.py
+drwxr-xr-x   0 t          (501) staff       (20)        0 2023-12-26 19:08:12.889205 mlsauce-0.9.1/mlsauce/utils/sampling/
+-rw-r--r--   0 t          (501) staff       (20)       64 2023-12-26 00:36:40.997545 mlsauce-0.9.1/mlsauce/utils/sampling/__init__.py
+-rw-r--r--   0 t          (501) staff       (20)     3169 2023-12-26 00:36:40.998061 mlsauce-0.9.1/mlsauce/utils/sampling/rowsubsampling.py
+-rw-r--r--   0 t          (501) staff       (20)      352 2023-12-26 00:36:40.999055 mlsauce-0.9.1/setup.cfg
+-rw-r--r--   0 t          (501) staff       (20)    11705 2023-12-26 18:55:16.559469 mlsauce-0.9.1/setup.py
```

### Comparing `mlsauce-0.9.0/PKG-INFO` & `mlsauce-0.9.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlsauce
-Version: 0.9.0
+Version: 0.9.1
 Summary: Miscellaneous Statistical/Machine Learning tools
 Maintainer: T. Moudiki
 Maintainer-email: thierry.moudiki@gmail.com
 License: BSD3 Clause Clear
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -19,11 +19,11 @@
 Requires-Dist: jax
 Requires-Dist: jaxlib
 Requires-Dist: numpy>=1.13.0
 Requires-Dist: scipy>=0.19.0
 Requires-Dist: joblib>=1.2.0
 Requires-Dist: scikit-learn>=0.18.0
 Requires-Dist: pandas>=0.25.3
-Requires-Dist: requests
+Requires-Dist: requests>=2.31.0
 Requires-Dist: tqdm
 
 Miscellaneous Statistical/Machine Learning tools
```

### Comparing `mlsauce-0.9.0/mlsauce/__check_build/__init__.py` & `mlsauce-0.9.1/mlsauce/__check_build/__init__.py`

 * *Files identical despite different names*

### Comparing `mlsauce-0.9.0/mlsauce/__check_build/setup.py` & `mlsauce-0.9.1/mlsauce/__check_build/setup.py`

 * *Files identical despite different names*

### Comparing `mlsauce-0.9.0/mlsauce/__init__.py` & `mlsauce-0.9.1/mlsauce/__init__.py`

 * *Files identical despite different names*

### Comparing `mlsauce-0.9.0/mlsauce/_build_utils/__init__.py` & `mlsauce-0.9.1/mlsauce/_build_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mlsauce-0.9.0/mlsauce/_build_utils/openmp_helpers.py` & `mlsauce-0.9.1/mlsauce/_build_utils/openmp_helpers.py`

 * *Files identical despite different names*

### Comparing `mlsauce-0.9.0/mlsauce/_build_utils/pre_build_helpers.py` & `mlsauce-0.9.1/mlsauce/_build_utils/pre_build_helpers.py`

 * *Files identical despite different names*

### Comparing `mlsauce-0.9.0/mlsauce/_config.py` & `mlsauce-0.9.1/mlsauce/_config.py`

 * *Files identical despite different names*

### Comparing `mlsauce-0.9.0/mlsauce/adaopt/_adaopt.py` & `mlsauce-0.9.1/mlsauce/adaopt/_adaopt.py`

 * *Files identical despite different names*

### Comparing `mlsauce-0.9.0/mlsauce/adaopt/_adaoptc.pyx` & `mlsauce-0.9.1/mlsauce/adaopt/_adaoptc.pyx`

 * *Files identical despite different names*

### Comparing `mlsauce-0.9.0/mlsauce/adaopt/setup.py` & `mlsauce-0.9.1/mlsauce/adaopt/setup.py`

 * *Files identical despite different names*

### Comparing `mlsauce-0.9.0/mlsauce/booster/_booster_classifier.py` & `mlsauce-0.9.1/mlsauce/booster/_booster_classifier.py`

 * *Files identical despite different names*

### Comparing `mlsauce-0.9.0/mlsauce/booster/_booster_regressor.py` & `mlsauce-0.9.1/mlsauce/booster/_booster_regressor.py`

 * *Files identical despite different names*

### Comparing `mlsauce-0.9.0/mlsauce/booster/_boosterc.pyx` & `mlsauce-0.9.1/mlsauce/booster/_boosterc.pyx`

 * *Files identical despite different names*

### Comparing `mlsauce-0.9.0/mlsauce/booster/setup.py` & `mlsauce-0.9.1/mlsauce/booster/setup.py`

 * *Files identical despite different names*

### Comparing `mlsauce-0.9.0/mlsauce/encoders/target_encoders.py` & `mlsauce-0.9.1/mlsauce/encoders/target_encoders.py`

 * *Files identical despite different names*

### Comparing `mlsauce-0.9.0/mlsauce/lasso/_lasso.py` & `mlsauce-0.9.1/mlsauce/lasso/_lasso.py`

 * *Files identical despite different names*

### Comparing `mlsauce-0.9.0/mlsauce/lasso/_lassoc.pyx` & `mlsauce-0.9.1/mlsauce/lasso/_lassoc.pyx`

 * *Files identical despite different names*

### Comparing `mlsauce-0.9.0/mlsauce/lasso/setup.py` & `mlsauce-0.9.1/mlsauce/lasso/setup.py`

 * *Files identical despite different names*

### Comparing `mlsauce-0.9.0/mlsauce/ridge/_ridge.py` & `mlsauce-0.9.1/mlsauce/ridge/_ridge.py`

 * *Files identical despite different names*

### Comparing `mlsauce-0.9.0/mlsauce/ridge/_ridgec.pyx` & `mlsauce-0.9.1/mlsauce/ridge/_ridgec.pyx`

 * *Files identical despite different names*

### Comparing `mlsauce-0.9.0/mlsauce/ridge/setup.py` & `mlsauce-0.9.1/mlsauce/ridge/setup.py`

 * *Files identical despite different names*

### Comparing `mlsauce-0.9.0/mlsauce/setup.py` & `mlsauce-0.9.1/mlsauce/setup.py`

 * *Files identical despite different names*

### Comparing `mlsauce-0.9.0/mlsauce/stump/_stump_classifier.py` & `mlsauce-0.9.1/mlsauce/stump/_stump_classifier.py`

 * *Files identical despite different names*

### Comparing `mlsauce-0.9.0/mlsauce/stump/_stumpc.pyx` & `mlsauce-0.9.1/mlsauce/stump/_stumpc.pyx`

 * *Files identical despite different names*

### Comparing `mlsauce-0.9.0/mlsauce/stump/setup.py` & `mlsauce-0.9.1/mlsauce/stump/setup.py`

 * *Files identical despite different names*

### Comparing `mlsauce-0.9.0/mlsauce/utils/memoryuse/mem_usage.py` & `mlsauce-0.9.1/mlsauce/utils/memoryuse/mem_usage.py`

 * *Files identical despite different names*

### Comparing `mlsauce-0.9.0/mlsauce/utils/misc/misc.py` & `mlsauce-0.9.1/mlsauce/utils/misc/misc.py`

 * *Files identical despite different names*

### Comparing `mlsauce-0.9.0/mlsauce/utils/sampling/rowsubsampling.py` & `mlsauce-0.9.1/mlsauce/utils/sampling/rowsubsampling.py`

 * *Files identical despite different names*

### Comparing `mlsauce-0.9.0/setup.py` & `mlsauce-0.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,18 @@
 try:
     import builtins
 except ImportError:
     # Python 2 compat: just to be able to declare that Python >=3.5 is needed.
     import __builtin__ as builtins
 
 try: 
+    subprocess.run(['pip', 'install', 'Cython>=0.29.21'], check=False)
     subprocess.run(['pip', 'install', 'numpy>= 1.13.0'], check=False)
     subprocess.run(['pip', 'install', 'scipy>= 0.19.0'], check=False)
-    subprocess.run(['pip', 'install', 'Cython>=0.29.21'], check=False)
+    subprocess.run(['pip', 'install', 'requests>=2.31.0'], check=False)
 except Exception:
     pass 
 
 builtins.__MLSAUCE_SETUP__ = True
 
 
 DISTNAME = 'mlsauce'
@@ -37,15 +38,15 @@
 MAINTAINER_EMAIL = 'thierry.moudiki@gmail.com'
 LICENSE = 'BSD3 Clause Clear'
 
 # We can actually import a restricted version of mlsauce that
 # does not need the compiled code
 import mlsauce
 
-__version__ = '0.9.0'
+__version__ = '0.9.1'
 
 VERSION = __version__
 
 if platform.python_implementation() == 'PyPy':
     SCIPY_MIN_VERSION = '1.1.0'
     NUMPY_MIN_VERSION = '1.14.0'
 else:
@@ -53,14 +54,15 @@
     NUMPY_MIN_VERSION = '1.13.0'
 
 JOBLIB_MIN_VERSION = '1.2.0'
 SKLEARN_MIN_VERSION = '0.18.0'
 THREADPOOLCTL_MIN_VERSION = '2.0.0'
 PANDAS_MIN_VERSION = '0.25.3'
 QUERIER_MIN_VERSION = '0.4.0'
+REQUESTS_MIN_VERSION = '2.31.0'
 if platform.system() in ('Linux', 'Darwin'):
     JAX_MIN_VERSION = '0.1.72'
     JAXLIB_MIN_VERSION = '0.1.51'
 
 # Optional setuptools features
 # We need to import setuptools early, if we want setuptools features,
 # as it monkey-patches the 'setup' function
@@ -234,22 +236,23 @@
                         'numpy>={}'.format(NUMPY_MIN_VERSION),
                         'scipy>={}'.format(SCIPY_MIN_VERSION),
                         'joblib>={}'.format(JOBLIB_MIN_VERSION),
                         'scikit-learn>={}'.format(SKLEARN_MIN_VERSION),
                         #'threadpoolctl>={}'.format(THREADPOOLCTL_MIN_VERSION),
                         'pandas>={}'.format(PANDAS_MIN_VERSION),
                         #'querier>={}'.format(QUERIER_MIN_VERSION)
+                        'requests>={}'.format(REQUESTS_MIN_VERSION),
                     ]
 
     install_jax_requires = [
                             'jax',
                             'jaxlib'
                             ] if platform.system() in ('Linux', 'Darwin') else []
 
-    other_requirements = ["requests",
+    other_requirements = [#"requests",
                           "tqdm", 
                           #"pymongo >= 3.10.1", 
                           #"SQLAlchemy >= 1.3.18"
                           ]
 
     install_requires = [item for sublist in [install_jax_requires, install_all_requires, other_requirements] for item in sublist]
```

