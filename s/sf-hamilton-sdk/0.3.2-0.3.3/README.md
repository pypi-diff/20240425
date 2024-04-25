# Comparing `tmp/sf_hamilton_sdk-0.3.2.tar.gz` & `tmp/sf_hamilton_sdk-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sf_hamilton_sdk-0.3.2.tar", last modified: Mon Apr 22 05:04:11 2024, max compression
+gzip compressed data, was "sf_hamilton_sdk-0.3.3.tar", last modified: Thu Apr 25 06:34:58 2024, max compression
```

## Comparing `sf_hamilton_sdk-0.3.2.tar` & `sf_hamilton_sdk-0.3.3.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-22 05:04:11.580302 sf_hamilton_sdk-0.3.2/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3529 2024-04-22 05:04:11.579871 sf_hamilton_sdk-0.3.2/PKG-INFO
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2130 2024-04-22 04:48:39.000000 sf_hamilton_sdk-0.3.2/README.md
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1916 2024-04-22 05:03:58.000000 sf_hamilton_sdk-0.3.2/pyproject.toml
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       18 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/requirements-test.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      140 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/requirements.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       38 2024-04-22 05:04:11.580387 sf_hamilton_sdk-0.3.2/setup.cfg
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      115 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/setup.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-22 05:04:11.542256 sf_hamilton_sdk-0.3.2/src/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-22 05:04:11.546865 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       25 2024-04-18 21:22:37.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)    24694 2024-04-18 19:22:29.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/adapters.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-22 05:04:11.549979 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/api/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-18 18:40:32.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/api/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)    30591 2024-04-18 19:22:29.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/api/clients.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       86 2024-04-18 18:40:32.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/api/constants.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      244 2024-04-18 18:40:32.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/api/projecttypes.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-22 05:04:11.551611 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-18 18:40:32.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      962 2024-04-18 18:40:32.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/cli.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5454 2024-04-18 18:40:32.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/initialize.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-22 05:04:11.552156 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/__init__.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-22 05:04:11.554375 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/common/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      123 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/common/.env.jinja2
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      307 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/common/README.md.jinja2
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       51 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/common/requirements.txt.jinja2
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2702 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/common/run.py.jinja2
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      697 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/common/run.sh.jinja2
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-22 05:04:11.554794 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/data_processing/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-22 05:04:11.556280 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/data_processing/components/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/data_processing/components/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      351 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/data_processing/components/_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      520 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/data_processing/components/common.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2528 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/data_processing/components/data_loader.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-22 05:04:11.556668 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/data_processing/config/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       26 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/data_processing/config/config.json
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-22 05:04:11.557896 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/data_processing/data/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      232 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/data_processing/data/order_details.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      480 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/data_processing/data/orders_new.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      309 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/data_processing/data/orders_old.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      678 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/data_processing/template_data.json
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-22 05:04:11.558324 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/hello_world/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-22 05:04:11.559118 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/hello_world/components/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/hello_world/components/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1577 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/hello_world/components/transforms.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-22 05:04:11.559901 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/hello_world/data/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      157 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/hello_world/data/signups.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      149 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/hello_world/data/spend.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      674 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/hello_world/template_data.json
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-22 05:04:11.560361 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/machine_learning/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-22 05:04:11.562446 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/machine_learning/components/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/machine_learning/components/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      488 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/machine_learning/components/_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3736 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/machine_learning/components/feature_transforms.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      598 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/machine_learning/components/iris_loader.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2531 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/machine_learning/components/model_fitting.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1402 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/machine_learning/components/models.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      477 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/machine_learning/template_data.json
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-22 05:04:11.562887 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/time_series_feature_engineering/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-22 05:04:11.565174 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1451 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      369 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/data_loader.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      710 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      931 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      744 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-22 05:04:11.565538 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/time_series_feature_engineering/data/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)   991302 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/time_series_feature_engineering/data/train_sample.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      679 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/time_series_feature_engineering/template_data.json
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)    31118 2024-04-18 19:22:29.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/driver.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-22 05:04:11.574951 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/tracking/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-18 18:40:32.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/tracking/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2401 2024-04-18 18:40:32.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/tracking/dataframe_stats.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4910 2024-04-18 18:40:32.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/tracking/example_tracking.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1072 2024-04-18 18:40:32.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/tracking/numpy_stats.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5442 2024-04-18 18:40:32.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/tracking/pandas_col_stats.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4833 2024-04-18 18:40:32.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/tracking/pandas_stats.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6279 2024-04-18 18:40:32.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/tracking/polars_col_stats.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4682 2024-04-18 18:40:32.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/tracking/polars_stats.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     8472 2024-04-18 18:40:32.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/tracking/runs.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      638 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/tracking/sql_utils.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6237 2024-04-18 18:40:32.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/tracking/stats.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1429 2024-04-18 18:40:32.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/tracking/trackingtypes.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1980 2024-04-18 19:22:29.000000 sf_hamilton_sdk-0.3.2/src/hamilton_sdk/tracking/utils.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-22 05:04:11.578904 sf_hamilton_sdk-0.3.2/src/sf_hamilton_sdk.egg-info/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3529 2024-04-22 05:04:11.000000 sf_hamilton_sdk-0.3.2/src/sf_hamilton_sdk.egg-info/PKG-INFO
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3700 2024-04-22 05:04:11.000000 sf_hamilton_sdk-0.3.2/src/sf_hamilton_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        1 2024-04-22 05:04:11.000000 sf_hamilton_sdk-0.3.2/src/sf_hamilton_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       58 2024-04-22 05:04:11.000000 sf_hamilton_sdk-0.3.2/src/sf_hamilton_sdk.egg-info/entry_points.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      109 2024-04-22 05:04:11.000000 sf_hamilton_sdk-0.3.2/src/sf_hamilton_sdk.egg-info/requires.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       13 2024-04-22 05:04:11.000000 sf_hamilton_sdk-0.3.2/src/sf_hamilton_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-22 05:04:11.578278 sf_hamilton_sdk-0.3.2/tests/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5383 2024-04-18 20:25:32.000000 sf_hamilton_sdk-0.3.2/tests/test_adapters.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3535 2024-04-18 18:30:22.000000 sf_hamilton_sdk-0.3.2/tests/test_driver.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     9604 2024-04-18 19:22:29.000000 sf_hamilton_sdk-0.3.2/tests/test_tracking.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.134060 sf_hamilton_sdk-0.3.3/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3529 2024-04-25 06:34:58.133170 sf_hamilton_sdk-0.3.3/PKG-INFO
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2130 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/README.md
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1916 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/pyproject.toml
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       18 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/requirements-test.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      140 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/requirements.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       38 2024-04-25 06:34:58.134242 sf_hamilton_sdk-0.3.3/setup.cfg
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      115 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/setup.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.069525 sf_hamilton_sdk-0.3.3/src/
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.075127 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       24 2024-04-25 06:33:40.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)    24683 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/adapters.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.077949 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/api/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/api/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)    30765 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/api/clients.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       85 2024-04-24 23:04:38.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/api/constants.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      243 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/api/projecttypes.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.080062 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      960 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/cli.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5453 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/initialize.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.080964 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/__init__.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.085893 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/common/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      123 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/common/.env.jinja2
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      307 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/common/README.md.jinja2
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       51 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/common/requirements.txt.jinja2
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2702 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/common/run.py.jinja2
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      697 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/common/run.sh.jinja2
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.086801 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/data_processing/
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.089658 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/data_processing/components/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/data_processing/components/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      352 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/data_processing/components/_run.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      520 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/data_processing/components/common.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2529 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/data_processing/components/data_loader.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.090345 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/data_processing/config/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       26 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/data_processing/config/config.json
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.092819 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/data_processing/data/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      232 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/data_processing/data/order_details.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      480 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/data_processing/data/orders_new.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      309 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/data_processing/data/orders_old.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      678 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/data_processing/template_data.json
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.093677 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/hello_world/
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.095066 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/hello_world/components/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/hello_world/components/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1577 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/hello_world/components/transforms.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.096552 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/hello_world/data/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      157 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/hello_world/data/signups.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      149 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/hello_world/data/spend.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      674 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/hello_world/template_data.json
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.097563 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/machine_learning/
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.101936 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/machine_learning/components/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/machine_learning/components/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      469 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/machine_learning/components/_run.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3738 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/machine_learning/components/feature_transforms.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      600 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/machine_learning/components/iris_loader.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2532 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/machine_learning/components/model_fitting.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1403 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/machine_learning/components/models.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      477 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/machine_learning/template_data.json
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.102751 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/time_series_feature_engineering/
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.108416 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1450 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/_run.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      370 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/data_loader.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      711 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      932 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      745 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.109160 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/time_series_feature_engineering/data/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)   991302 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/time_series_feature_engineering/data/train_sample.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      679 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/time_series_feature_engineering/template_data.json
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)    31210 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/driver.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.124149 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2401 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/dataframe_stats.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4908 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/example_tracking.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1037 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/numpy_stats.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5440 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/pandas_col_stats.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4833 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/pandas_stats.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6277 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/polars_col_stats.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4683 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/polars_stats.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     8470 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/runs.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      638 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/sql_utils.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6235 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/stats.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1428 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/trackingtypes.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1980 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/utils.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.131130 sf_hamilton_sdk-0.3.3/src/sf_hamilton_sdk.egg-info/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3529 2024-04-25 06:34:58.000000 sf_hamilton_sdk-0.3.3/src/sf_hamilton_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3700 2024-04-25 06:34:58.000000 sf_hamilton_sdk-0.3.3/src/sf_hamilton_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        1 2024-04-25 06:34:58.000000 sf_hamilton_sdk-0.3.3/src/sf_hamilton_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       58 2024-04-25 06:34:58.000000 sf_hamilton_sdk-0.3.3/src/sf_hamilton_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      109 2024-04-25 06:34:58.000000 sf_hamilton_sdk-0.3.3/src/sf_hamilton_sdk.egg-info/requires.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       13 2024-04-25 06:34:58.000000 sf_hamilton_sdk-0.3.3/src/sf_hamilton_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-25 06:34:58.130377 sf_hamilton_sdk-0.3.3/tests/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5387 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/tests/test_adapters.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3535 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/tests/test_driver.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     9605 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.3/tests/test_tracking.py
```

### Comparing `sf_hamilton_sdk-0.3.2/PKG-INFO` & `sf_hamilton_sdk-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sf-hamilton-sdk
-Version: 0.3.2
+Version: 0.3.3
 Summary: Hamilton SDK for reading and writing to the Hamilton backend APIs that support the UI.
 Author-email: Stefan Krawczyk <stefan@dagworks.io>, Elijah ben Izzy <elijah@dagworks.io>
 Project-URL: Homepage, https://github.com/dagworks-inc/hamilton/
 Project-URL: Bug Reports, https://github.com/dagworks-inc/hamilton/issues
 Project-URL: Source, https://github.com/dagworks-inc/hamilton/ui/sdk
 Project-URL: Documenation, https://hamilton.dagworks.io/
 Keywords: hamilton,dagworks,observability
@@ -18,20 +18,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 Requires-Dist: click
 Requires-Dist: gitpython
+Requires-Dist: jinja2
+Requires-Dist: loguru
 Requires-Dist: posthog
 Requires-Dist: requests
 Requires-Dist: sf-hamilton>=1.43.0
 Requires-Dist: sqlglot
-Requires-Dist: jinja2
-Requires-Dist: loguru
 Provides-Extra: test
 Requires-Dist: polars; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: ray; extra == "test"
 
 # Hamilton UI SDK: Client Code &amp; Related
```

### Comparing `sf_hamilton_sdk-0.3.2/README.md` & `sf_hamilton_sdk-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.2/pyproject.toml` & `sf_hamilton_sdk-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.2/src/hamilton_sdk/adapters.py` & `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/adapters.py`

 * *Files identical despite different names*

```diff
@@ -1,31 +1,29 @@
 import asyncio
+import datetime
 import hashlib
 import logging
-import datetime
+import os
+import random
 import traceback
 from datetime import timezone
-import random
 from types import ModuleType
-from typing import Callable, Optional, Dict, Any, List
-
-from hamilton import node
-from hamilton.lifecycle import base
-from hamilton import graph as h_graph
-from hamilton.data_quality import base as dq_base
+from typing import Any, Callable, Dict, List, Optional
 
 from hamilton_sdk import driver
 from hamilton_sdk.api import clients, constants
 from hamilton_sdk.tracking import runs
 from hamilton_sdk.tracking.runs import Status, TrackingState
-
-import os
-
 from hamilton_sdk.tracking.trackingtypes import TaskRun
 
+from hamilton import graph as h_graph
+from hamilton import node
+from hamilton.data_quality import base as dq_base
+from hamilton.lifecycle import base
+
 logger = logging.getLogger(__name__)
 
 
 def get_node_name(node_: node.Node, task_id: Optional[str]) -> str:
     if task_id is not None:
         return f"{task_id}-{node_.name}"
     return node_.name
@@ -387,15 +385,15 @@
         driver.validate_tags(self.base_tags)
         self.dag_name = dag_name
         self.hamilton_ui_url = hamilton_ui_url
         logger.debug("Validating authentication against Hamilton BE API...")
         asyncio.run(self.client.validate_auth())
         logger.debug(f"Ensuring project {self.project_id} exists...")
         try:
-            exists = asyncio.run(self.client.project_exists(self.project_id))
+            asyncio.run(self.client.project_exists(self.project_id))
         except clients.UnauthorizedException:
             logger.exception(
                 f"Authentication failed. Please check your username and try again. "
                 f"Username: {self.username}"
             )
             raise
         except clients.ResourceDoesNotExistException:
```

### Comparing `sf_hamilton_sdk-0.3.2/src/hamilton_sdk/api/clients.py` & `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/api/clients.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-
 import abc
-from collections import defaultdict
-from functools import reduce
-import threading
-import queue
-import time
-import aiohttp
 import datetime
 import logging
-from typing import Dict, Any, List, Callable
+import queue
+import threading
+import time
+from collections import defaultdict
+from functools import reduce
+from typing import Any, Callable, Dict, List
 from urllib.parse import urlencode
 
+import aiohttp
 import requests
-from requests import HTTPError
-
 from hamilton_sdk.api.projecttypes import GitInfo
 from hamilton_sdk.tracking.utils import make_json_safe
+from requests import HTTPError
 
 logger = logging.getLogger(__name__)
 
 
 class ResourceDoesNotExistException(Exception):
     def __init__(self, resource_type: str, resource_id: str, username: str):
         message = f"Resource {resource_type} with id {resource_id} does not exist/is accesible for user {username}."
@@ -356,17 +354,21 @@
             f"{self.base_url}/projects/{project_id}", headers=self._common_headers()
         )
         try:
             response.raise_for_status()
             logger.debug(f"Project {project_id} exists")
             return True
         except HTTPError as e:
-            logger.debug(f"Project {project_id} does not exist/is accessible for user {self.username}")
+            logger.debug(
+                f"Project {project_id} does not exist/is accessible for user {self.username}"
+            )
             if response.status_code // 100 == 4:
-                raise ResourceDoesNotExistException("project", str(project_id), self.username) from e
+                raise ResourceDoesNotExistException(
+                    "project", str(project_id), self.username
+                ) from e
             raise
 
     def register_dag_template_if_not_exists(
         self,
         project_id: int,
         dag_hash: str,
         code_hash: str,
@@ -552,15 +554,17 @@
                     data = await response.json()
                     exists = data is not None
                 except aiohttp.ClientResponseError as e:
                     logger.debug(
                         f"Failed to access project version {project_id} when looking for code hash: {code_hash}"
                     )
                     if response.status // 100 == 4:
-                        raise ResourceDoesNotExistException("code_version", code_hash, self.username) from e
+                        raise ResourceDoesNotExistException(
+                            "code_version", code_hash, self.username
+                        ) from e
                     raise
 
         if exists:
             return data["id"]
         code_slurped = slurp_code()
         async with aiohttp.ClientSession() as session:
             async with session.post(
@@ -599,15 +603,17 @@
                 try:
                     response.raise_for_status()
                     logger.debug(f"Project {project_id} exists")
                     return True
                 except aiohttp.ClientResponseError as e:
                     logger.debug(f"Project {project_id} does not exist")
                     if response.status // 100 == 4:
-                        raise ResourceDoesNotExistException("project", str(project_id), self.username) from e
+                        raise ResourceDoesNotExistException(
+                            "project", str(project_id), self.username
+                        ) from e
                     raise
 
     async def register_dag_template_if_not_exists(
         self,
         project_id: int,
         dag_hash: str,
         code_hash: str,
```

### Comparing `sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/cli.py` & `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-
 import os
 
 import click
-
 from hamilton_sdk.cli import initialize
 
 
 @click.group()
 def cli():
     pass
```

### Comparing `sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/initialize.py` & `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/initialize.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import importlib.resources
 import json
 import os
 import shutil
 from typing import Any, Dict
 
 import jinja2
```

### Comparing `sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/common/run.py.jinja2` & `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/common/run.py.jinja2`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/common/run.sh.jinja2` & `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/common/run.sh.jinja2`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/data_processing/components/common.py` & `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/data_processing/components/common.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/data_processing/components/data_loader.py` & `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/data_processing/components/data_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pandas as pd
 import pandera as pa
+
 from hamilton.function_modifiers import check_output, config, source
 from hamilton.function_modifiers.adapters import load_from
 
 PRODUCT_SET = frozenset(["Apple", "Orange", "Banana", "Grape", "Pineapple", "Watermelon"])
 order_details_schema = pa.DataFrameSchema(
     {
         "order_id": pa.Column(int, checks=[pa.Check.ge(0)], nullable=False),
```

### Comparing `sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/data_processing/template_data.json` & `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/data_processing/template_data.json`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/hello_world/components/transforms.py` & `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/hello_world/components/transforms.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/hello_world/template_data.json` & `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/hello_world/template_data.json`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/machine_learning/components/feature_transforms.py` & `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/machine_learning/components/feature_transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """
 Module to transform iris data into features.
 """
+
 import numpy as np
 import pandas as pd
+
 from hamilton.function_modifiers import parameterize_sources
 
 RAW_FEATURES = ["sepal_length_cm", "sepal_width_cm", "petal_length_cm", "petal_width_cm"]
 
 # Here is more terse code that does the same thing as the below *_log functions.
 # Any `@parameterize*` decorator is just a less verbose way of defining functions that differ
 # slightly. We don't see anything wrong with verbose code - so we recommend err'ing on the side of
```

### Comparing `sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/machine_learning/components/iris_loader.py` & `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/machine_learning/components/iris_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 Module to load iris data.
 """
+
 import pandas as pd
-from hamilton.function_modifiers import extract_columns
 from sklearn import datasets, utils
 
+from hamilton.function_modifiers import extract_columns
+
 RAW_COLUMN_NAMES = [
     "sepal_length_cm",
     "sepal_width_cm",
     "petal_length_cm",
     "petal_width_cm",
 ]
```

### Comparing `sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/machine_learning/components/model_fitting.py` & `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/machine_learning/components/model_fitting.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """This module contains basic code for model fitting."""
 
 from typing import Dict
 
 import numpy as np
 import pandas as pd
-from hamilton import function_modifiers
 from sklearn import base, linear_model, metrics, svm
 from sklearn.model_selection import train_test_split
 
+from hamilton import function_modifiers
+
 
 @function_modifiers.config.when(clf="svm")
 def prefit_clf__svm(gamma: float = 0.001) -> base.ClassifierMixin:
     """Returns an unfitted SVM classifier object.
 
     :param gamma: ...
     :return:
```

### Comparing `sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/machine_learning/components/models.py` & `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/machine_learning/components/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """This module contains specific incarnations of models."""
 
-from hamilton.function_modifiers import source, subdag
 from sklearn import base
 
+from hamilton.function_modifiers import source, subdag
+
 try:
     import model_fitting
 except ImportError:
     from . import model_fitting
 
 
 @subdag(
```

### Comparing `sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/_run.py` & `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/_run.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import Tuple
 
-import pandas as pd
-
 import data_loader
 import ftrs_autoregression
 import ftrs_calendar
 import ftrs_common_prep
+import pandas as pd
 
 
 def create_training_features(data_path: str) -> Tuple[pd.DataFrame, pd.DataFrame]:
     config = {
         "data_path": data_path,
     }
     import os
```

### Comparing `sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py` & `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pandas as pd
-from hamilton.function_modifiers import parameterize_values, tag
 from pandas.core.groupby import DataFrameGroupBy
 
+from hamilton.function_modifiers import parameterize_values, tag
+
 
 @tag(stage="production")
 @parameterize_values(
     parameter="n",
     assigned_output={
         ("lag_sales_1", ""): 1,
         ("lag_sales_2", ""): 2,
```

### Comparing `sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py` & `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pandas as pd
+
 from hamilton.function_modifiers import extract_columns, tag
 
 
 @extract_columns("date")
 def sales_data_set_output_idx(sales_data_set: pd.DataFrame, output_idx: pd.Index) -> pd.DataFrame:
     return sales_data_set.loc[output_idx]
```

### Comparing `sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py` & `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pandas as pd
-from hamilton.function_modifiers import extract_columns, tag
 from pandas import DataFrame
 from pandas.core.groupby import DataFrameGroupBy
 
+from hamilton.function_modifiers import extract_columns, tag
+
 
 def output_idx(lag_sales_31: pd.Series) -> pd.Index:
     return lag_sales_31.index
 
 
 def grp_date_store_item(sales_data_set: DataFrame) -> DataFrameGroupBy:
     return sales_data_set.groupby(by=["store", "item"])
```

### Comparing `sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/time_series_feature_engineering/data/train_sample.csv` & `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/time_series_feature_engineering/data/train_sample.csv`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.2/src/hamilton_sdk/cli/templates/time_series_feature_engineering/template_data.json` & `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/cli/templates/time_series_feature_engineering/template_data.json`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.2/src/hamilton_sdk/driver.py` & `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 import hashlib
 import inspect
 import json
 import logging
 import operator
 import os
 from types import ModuleType
-from typing import Any, Callable, Dict, List, Set, Tuple, Union, Optional
+from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
 
-from hamilton import base, driver, node, graph
+from hamilton_sdk.api.clients import UnauthorizedException
+
+from hamilton import base, driver, graph, node
 from hamilton.driver import Variable
 from hamilton.io import materialization
 from hamilton.lifecycle.base import BaseDoNodeExecute
 from hamilton.node import Node
-from hamilton_sdk.api.clients import UnauthorizedException
 
 try:
     import git
 except ImportError:
     git = None
 
 from hamilton_sdk.api import clients, constants
 from hamilton_sdk.api.projecttypes import GitInfo
 from hamilton_sdk.tracking.runs import Status, TrackingState, monkey_patch_adapter
 
-
 logger = logging.getLogger(__name__)
 
 
 def _hash_module(
     module: ModuleType, hash_object: hashlib.sha256, seen_modules: Set[ModuleType]
 ) -> hashlib.sha256:
     """Generate a hash of the specified module and its imports.
@@ -263,15 +263,14 @@
         :param dagworks_api_url: Optional. URL to use for the DAGWorks API.
         :param dagworks_ui_url: Optional. URL to use for the DAGWorks UI.
         """
         if adapter is None:
             adapter = base.SimplePythonGraphAdapter(result_builder=base.DictResult())
         super(Driver, self).__init__(config, *modules, adapter=adapter)
 
-
         self.config = config
         self.project = project_id
         self.api_key = api_key
         self.username = username
         # TODO -- figure out how to pass any additional configuration to the client if needed
         self.client = client_factory(api_key, username, dagworks_api_url)
         self.module_hash = _get_modules_hash(modules)
@@ -358,15 +357,14 @@
         inputs: Dict[str, Any] = None,
         _fn_graph: graph.FunctionGraph = None,
     ) -> Dict[str, Any]:
         return super(Driver, self).raw_execute(
             final_vars, overrides, display_graph, inputs, _fn_graph
         )
 
-
     def materialize(
         self,
         *materializers: materialization.MaterializerFactory,
         additional_vars: List[Union[str, Callable, Variable]] = None,
         overrides: Dict[str, Any] = None,
         inputs: Dict[str, Any] = None,
     ) -> Tuple[Any, Dict[str, Any]]:
@@ -486,17 +484,21 @@
                 name=node_.name,
                 output={"type_name": str(node_.type)},
                 output_type="python_type",
                 output_schema_version=1,  # TODO -- merge this with _convert_node_dependencies
                 documentation=node_.documentation,
                 tags=node_.tags,  # TODO -- ensure serializable
                 classifications=_convert_classifications(node_),  # TODO -- manage classifications
-                code_artifact_pointers=code_artifact_pointers
-                if node_.originating_functions is None or len(node_.originating_functions) == 0
-                else [_get_fully_qualified_function_path(fn) for fn in node_.originating_functions],
+                code_artifact_pointers=(
+                    code_artifact_pointers
+                    if node_.originating_functions is None or len(node_.originating_functions) == 0
+                    else [
+                        _get_fully_qualified_function_path(fn) for fn in node_.originating_functions
+                    ]
+                ),
                 **_convert_node_dependencies(node_),
             )
         )
     return node_templates
 
 
 def _derive_url(vcs_info: GitInfo, path: str, line: int) -> str:
```

### Comparing `sf_hamilton_sdk-0.3.2/src/hamilton_sdk/tracking/dataframe_stats.py` & `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/dataframe_stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-
-from typing import Union, Dict, Any
 from dataclasses import dataclass
+from typing import Any, Dict, Union
+
 import numpy as np
 import pandas as pd
 
 
 def type_converter(obj: Any) -> Any:
     # obj = getattr(self, key)
     if isinstance(obj, np.ndarray):
```

### Comparing `sf_hamilton_sdk-0.3.2/src/hamilton_sdk/tracking/example_tracking.py` & `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/example_tracking.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-
 import logging
 import os
 import sys
 from types import ModuleType
 from typing import Any, Dict, List
 
 import click
-import pandas as pd
-
 import dagworks.driver
+import pandas as pd
 
 logging.basicConfig(level=logging.DEBUG, stream=sys.stdout)
 
 """
 Some basic examples
 These are meant to be run from within the hamilton repo --
 they use the examples there.
```

### Comparing `sf_hamilton_sdk-0.3.2/src/hamilton_sdk/tracking/numpy_stats.py` & `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/numpy_stats.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-
-from typing import Dict, Any
+from typing import Any, Dict
 
 import numpy as np
 import pandas as pd
-
-from hamilton_sdk.tracking import pandas_stats
-from hamilton_sdk.tracking import stats
+from hamilton_sdk.tracking import pandas_stats, stats
 
 """Module that houses functions to compute statistics on numpy objects
 Notes:
  - we should assume numpy v1.0+ so that we have a string type
 """
```

### Comparing `sf_hamilton_sdk-0.3.2/src/hamilton_sdk/tracking/pandas_col_stats.py` & `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/pandas_col_stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-
 from typing import Dict, List, Union
 
 import pandas as pd
-
 from hamilton_sdk.tracking import dataframe_stats as dfs
 
 
 def data_type(col: pd.Series) -> str:
     return str(col.dtype)
```

### Comparing `sf_hamilton_sdk-0.3.2/src/hamilton_sdk/tracking/pandas_stats.py` & `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/pandas_stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
+from typing import Any, Dict, Union
 
-from typing import Dict, Any, Union
 import pandas as pd
-from hamilton import driver
-
 from hamilton_sdk.tracking import pandas_col_stats as pcs
 from hamilton_sdk.tracking import stats
 
+from hamilton import driver
+
 """Module that houses functions to compute statistics on pandas series/dataframes.
 Notes:
  - we should assume pandas v1.0+ so that we have a string type
  - for object types we should :shrug:
 """
 
 dr = driver.Builder().with_modules(pcs).with_config({"config_key": "config_value"}).build()
```

### Comparing `sf_hamilton_sdk-0.3.2/src/hamilton_sdk/tracking/polars_col_stats.py` & `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/polars_col_stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-
 import datetime
 from typing import Dict, List, Union
 
 import polars as pl
-
 from hamilton_sdk.tracking import dataframe_stats as dfs
 
 
 def data_type(col: pl.Series) -> str:
     return str(col.dtype)
```

### Comparing `sf_hamilton_sdk-0.3.2/src/hamilton_sdk/tracking/polars_stats.py` & `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/polars_stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+from typing import Any, Dict
 
-from typing import Dict, Any
 import polars as pl
 
 if not hasattr(pl, "Series"):
     raise ImportError("Polars is not installed")
-from hamilton import driver
 from hamilton_sdk.tracking import polars_col_stats as pls
 from hamilton_sdk.tracking import stats
 
+from hamilton import driver
+
 """Module that houses functions to compute statistics on polars series/dataframes.
 Notes:
  - we should assume a minimum polars version
  - for object types we should :shrug:
  - TBD how close the schemas
 
 """
```

### Comparing `sf_hamilton_sdk-0.3.2/src/hamilton_sdk/tracking/runs.py` & `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/runs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-
 import functools
 import logging
 import sys
 import time as py_time
 import traceback
 from contextlib import contextmanager
 from datetime import datetime, timezone
 from typing import Any, Callable, Dict, List, Optional
 
+from hamilton_sdk.tracking import stats
+from hamilton_sdk.tracking.trackingtypes import DAGRun, Status, TaskRun
+
 from hamilton import node as h_node
 from hamilton.data_quality import base as dq_base
-
 from hamilton.lifecycle import base as lifecycle_base
 
-from hamilton_sdk.tracking import stats
-from hamilton_sdk.tracking.trackingtypes import DAGRun, Status, TaskRun
-
 try:
-    from hamilton_sdk.tracking import pandas_stats  # noqa: F401
     from hamilton_sdk.tracking import numpy_stats  # noqa: F401
+    from hamilton_sdk.tracking import pandas_stats  # noqa: F401
 
 except ImportError:
     pass
 
 try:
     from hamilton_sdk.tracking import polars_stats  # noqa: F401
```

### Comparing `sf_hamilton_sdk-0.3.2/src/hamilton_sdk/tracking/sql_utils.py` & `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/sql_utils.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.2/src/hamilton_sdk/tracking/stats.py` & `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-
-from functools import singledispatch
 import json
-from typing import Dict, Any
+from functools import singledispatch
+from typing import Any, Dict
 
 import pandas as pd
-
 from hamilton_sdk.tracking import sql_utils
 
 
 @singledispatch
 def compute_stats(result, node_name: str, node_tags: dict) -> Dict[str, Any]:
     """This is the default implementation for computing stats on a result.
```

### Comparing `sf_hamilton_sdk-0.3.2/src/hamilton_sdk/tracking/trackingtypes.py` & `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/trackingtypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import dataclasses
 import enum
 from datetime import datetime
 from typing import List, Optional, Type
 
 
 class Status(enum.Enum):
```

### Comparing `sf_hamilton_sdk-0.3.2/src/hamilton_sdk/tracking/utils.py` & `sf_hamilton_sdk-0.3.3/src/hamilton_sdk/tracking/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import dataclasses
 import datetime
-from enum import Enum
 import json
 import logging
-from typing import Union, Any
+from enum import Enum
+from typing import Any, Union
 
 import numpy as np
 
 logger = logging.getLogger(__name__)
 
 
 class CustomEncoder(json.JSONEncoder):
```

### Comparing `sf_hamilton_sdk-0.3.2/src/sf_hamilton_sdk.egg-info/PKG-INFO` & `sf_hamilton_sdk-0.3.3/src/sf_hamilton_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sf-hamilton-sdk
-Version: 0.3.2
+Version: 0.3.3
 Summary: Hamilton SDK for reading and writing to the Hamilton backend APIs that support the UI.
 Author-email: Stefan Krawczyk <stefan@dagworks.io>, Elijah ben Izzy <elijah@dagworks.io>
 Project-URL: Homepage, https://github.com/dagworks-inc/hamilton/
 Project-URL: Bug Reports, https://github.com/dagworks-inc/hamilton/issues
 Project-URL: Source, https://github.com/dagworks-inc/hamilton/ui/sdk
 Project-URL: Documenation, https://hamilton.dagworks.io/
 Keywords: hamilton,dagworks,observability
@@ -18,20 +18,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 Requires-Dist: click
 Requires-Dist: gitpython
+Requires-Dist: jinja2
+Requires-Dist: loguru
 Requires-Dist: posthog
 Requires-Dist: requests
 Requires-Dist: sf-hamilton>=1.43.0
 Requires-Dist: sqlglot
-Requires-Dist: jinja2
-Requires-Dist: loguru
 Provides-Extra: test
 Requires-Dist: polars; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: ray; extra == "test"
 
 # Hamilton UI SDK: Client Code &amp; Related
```

### Comparing `sf_hamilton_sdk-0.3.2/src/sf_hamilton_sdk.egg-info/SOURCES.txt` & `sf_hamilton_sdk-0.3.3/src/sf_hamilton_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.2/tests/test_adapters.py` & `sf_hamilton_sdk-0.3.3/tests/test_adapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import os.path
 
 import pytest
+from hamilton_sdk import adapters
+
 from hamilton import driver
 
 import tests.resources.basic_dag_with_config
 import tests.resources.parallel_dag
 import tests.resources.parallel_dag_error
-from hamilton_sdk import adapters
 from tests import test_tracking
 
 adapter_kwargs = dict(
     project_id=19319,
     api_key="l-PlUq02JLQR6rAvO4x7VTttNTtprj1Tz5zBZ0ARpQ4olb8TK4hlgY2pennFhvsR1DxpYMQ-TLm0JknXVn7y9A",
     username="stefan@dagworks.io",
     tags={"env": "dev", "status": "development"},
@@ -41,17 +42,18 @@
 #     )
 #     [adapters.AsyncHamiltonAdapter(**kwargs)]
 
 
 def test_parallel_ray():
     """Tests ray works without sampling.
     Doesn't actually check the client - go do that in the UI."""
-    from hamilton.plugins import h_ray
     import ray
 
+    from hamilton.plugins import h_ray
+
     kwargs = adapter_kwargs | dict(dag_name="parallel_test_dag", tags={"sampling_rate": "None"})
     lifecycle_adapters = [adapters.HamiltonTracker(**kwargs)]
     remote_executor = h_ray.RayTaskExecutor(None)
     # remote_executor = executors.SynchronousLocalTaskExecutor()
     shutdown = ray.shutdown
     dr = (
         driver.Builder()
@@ -73,17 +75,18 @@
     for val in result.index.values:
         assert val in expected_cities
 
 
 def test_parallel_ray_sample():
     """Tests ray works with sampling.
     Doesn't actually check the client - go do that in the UI."""
-    from hamilton.plugins import h_ray
     import ray
 
+    from hamilton.plugins import h_ray
+
     special_parallel_sample_strategy = 0.33
     kwargs = adapter_kwargs | dict(
         dag_name="parallel_test_dag", tags={"sampling_rate": str(special_parallel_sample_strategy)}
     )
     lifecycle_adapters = [adapters.HamiltonTracker(**kwargs)]
     lifecycle_adapters[0].special_parallel_sample_strategy = special_parallel_sample_strategy
     remote_executor = h_ray.RayTaskExecutor(None)
@@ -109,17 +112,18 @@
     for val in result.index.values:
         assert val in expected_cities
 
 
 def test_parallel_ray_sample_error():
     """Tests error returning a sample.
     Doesn't actually check the client - go do that in the UI."""
-    from hamilton.plugins import h_ray
     import ray
 
+    from hamilton.plugins import h_ray
+
     special_parallel_sample_strategy = 0.0
     kwargs = adapter_kwargs | dict(
         dag_name="parallel_test_dag", tags={"sampling_rate": str(special_parallel_sample_strategy)}
     )
     lifecycle_adapters = [adapters.HamiltonTracker(**kwargs)]
     lifecycle_adapters[0].special_parallel_sample_strategy = special_parallel_sample_strategy
     remote_executor = h_ray.RayTaskExecutor(None)
```

### Comparing `sf_hamilton_sdk-0.3.2/tests/test_driver.py` & `sf_hamilton_sdk-0.3.3/tests/test_driver.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.2/tests/test_tracking.py` & `sf_hamilton_sdk-0.3.3/tests/test_tracking.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import functools
 from datetime import datetime, timezone
 from typing import Any, Callable, Dict, List
 
 import pytest
-from hamilton import base
-from hamilton.io.materialization import to
-
-import tests.resources.basic_dag_with_config
 from hamilton_sdk import driver
 from hamilton_sdk.api.clients import HamiltonClient
 from hamilton_sdk.api.projecttypes import GitInfo
 from hamilton_sdk.tracking.runs import TrackingState
 from hamilton_sdk.tracking.trackingtypes import Status, TaskRun
 
+from hamilton import base
+from hamilton.io.materialization import to
+
+import tests.resources.basic_dag_with_config
+
 
 # Yeah, I should probably use a mock library but this is simple and does what I want
 def track_calls(fn: Callable):
     @functools.wraps(fn)
     def wrapper(self, *args, **kwargs):
         setattr(self, f"{fn.__name__}_latest_kwargs", kwargs)
         setattr(self, f"{fn.__name__}_latest_args", args)
```

