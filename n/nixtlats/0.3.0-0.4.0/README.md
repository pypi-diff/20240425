# Comparing `tmp/nixtlats-0.3.0.tar.gz` & `tmp/nixtlats-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nixtlats-0.3.0.tar", last modified: Wed Apr  3 02:32:11 2024, max compression
+gzip compressed data, was "nixtlats-0.4.0.tar", last modified: Thu Apr 25 02:01:31 2024, max compression
```

## Comparing `nixtlats-0.3.0.tar` & `nixtlats-0.4.0.tar`

### file list

```diff
@@ -1,59 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:32:11.102105 nixtlats-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11414 2024-04-03 02:32:06.000000 nixtlats-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-04-03 02:32:11.102105 nixtlats-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-04-03 02:32:06.000000 nixtlats-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:32:11.094105 nixtlats-0.3.0/action_files/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:32:06.000000 nixtlats-0.3.0/action_files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:32:11.094105 nixtlats-0.3.0/nixtlats/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20917 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (127)    47299 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:32:11.098105 nixtlats-0.3.0/nixtlats/core/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/core/api_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/core/client_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/core/datetime_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/core/jsonable_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/core/remove_none_from_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/date_features.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:32:11.098105 nixtlats-0.3.0/nixtlats/distributed/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11179 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/distributed/nixtla_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:32:11.098105 nixtlats-0.3.0/nixtlats/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/errors/unprocessable_entity_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    62656 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/nixtla_client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:32:11.102105 nixtlats-0.3.0/nixtlats/types/
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/multi_series_anomaly.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/multi_series_anomaly_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/multi_series_cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/multi_series_cross_validation_fewshot_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/multi_series_cross_validation_finetune_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/multi_series_cross_validation_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/multi_series_forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/multi_series_forecast_fewshot_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/multi_series_forecast_finetune_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/multi_series_forecast_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/multi_series_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/multi_series_insample_forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/multi_series_insample_forecast_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/single_series_forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/single_series_forecast_fewshot_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/single_series_forecast_finetune_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/single_series_forecast_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/single_series_insample_forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/single_series_insample_forecast_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/validation_error_loc_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:32:11.102105 nixtlats-0.3.0/nixtlats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-04-03 02:32:11.000000 nixtlats-0.3.0/nixtlats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-03 02:32:11.000000 nixtlats-0.3.0/nixtlats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:32:11.000000 nixtlats-0.3.0/nixtlats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-03 02:32:11.000000 nixtlats-0.3.0/nixtlats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 02:32:11.000000 nixtlats-0.3.0/nixtlats.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 02:32:11.102105 nixtlats-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-03 02:32:06.000000 nixtlats-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:01:31.048704 nixtlats-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11414 2024-04-25 02:01:13.000000 nixtlats-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-25 02:01:31.048704 nixtlats-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-25 02:01:13.000000 nixtlats-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:01:31.040704 nixtlats-0.4.0/nixtlats/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-25 02:01:29.000000 nixtlats-0.4.0/nixtlats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19978 2024-04-25 02:01:29.000000 nixtlats-0.4.0/nixtlats/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48931 2024-04-25 02:01:29.000000 nixtlats-0.4.0/nixtlats/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:01:31.040704 nixtlats-0.4.0/nixtlats/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-25 02:01:29.000000 nixtlats-0.4.0/nixtlats/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-25 02:01:29.000000 nixtlats-0.4.0/nixtlats/core/api_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-25 02:01:29.000000 nixtlats-0.4.0/nixtlats/core/client_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-25 02:01:29.000000 nixtlats-0.4.0/nixtlats/core/datetime_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-25 02:01:29.000000 nixtlats-0.4.0/nixtlats/core/jsonable_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-25 02:01:29.000000 nixtlats-0.4.0/nixtlats/core/remove_none_from_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-25 02:01:29.000000 nixtlats-0.4.0/nixtlats/date_features.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:01:31.040704 nixtlats-0.4.0/nixtlats/distributed/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 02:01:29.000000 nixtlats-0.4.0/nixtlats/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11179 2024-04-25 02:01:29.000000 nixtlats-0.4.0/nixtlats/distributed/nixtla_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:01:31.040704 nixtlats-0.4.0/nixtlats/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-25 02:01:29.000000 nixtlats-0.4.0/nixtlats/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-25 02:01:29.000000 nixtlats-0.4.0/nixtlats/errors/unprocessable_entity_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64069 2024-04-25 02:01:29.000000 nixtlats-0.4.0/nixtlats/nixtla_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 02:01:13.000000 nixtlats-0.4.0/nixtlats/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:01:31.044704 nixtlats-0.4.0/nixtlats/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-25 02:01:29.000000 nixtlats-0.4.0/nixtlats/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-25 02:01:29.000000 nixtlats-0.4.0/nixtlats/types/http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-25 02:01:29.000000 nixtlats-0.4.0/nixtlats/types/multi_series_anomaly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-25 02:01:29.000000 nixtlats-0.4.0/nixtlats/types/multi_series_anomaly_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-04-25 02:01:29.000000 nixtlats-0.4.0/nixtlats/types/multi_series_cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-25 02:01:29.000000 nixtlats-0.4.0/nixtlats/types/multi_series_cross_validation_fewshot_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-25 02:01:29.000000 nixtlats-0.4.0/nixtlats/types/multi_series_cross_validation_finetune_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-25 02:01:29.000000 nixtlats-0.4.0/nixtlats/types/multi_series_cross_validation_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-04-25 02:01:29.000000 nixtlats-0.4.0/nixtlats/types/multi_series_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-25 02:01:29.000000 nixtlats-0.4.0/nixtlats/types/multi_series_forecast_fewshot_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-25 02:01:29.000000 nixtlats-0.4.0/nixtlats/types/multi_series_forecast_finetune_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-25 02:01:29.000000 nixtlats-0.4.0/nixtlats/types/multi_series_forecast_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-25 02:01:29.000000 nixtlats-0.4.0/nixtlats/types/multi_series_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-25 02:01:29.000000 nixtlats-0.4.0/nixtlats/types/multi_series_insample_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-25 02:01:29.000000 nixtlats-0.4.0/nixtlats/types/multi_series_insample_forecast_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-04-25 02:01:29.000000 nixtlats-0.4.0/nixtlats/types/single_series_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-25 02:01:29.000000 nixtlats-0.4.0/nixtlats/types/single_series_forecast_fewshot_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-25 02:01:29.000000 nixtlats-0.4.0/nixtlats/types/single_series_forecast_finetune_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-25 02:01:29.000000 nixtlats-0.4.0/nixtlats/types/single_series_forecast_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-25 02:01:29.000000 nixtlats-0.4.0/nixtlats/types/single_series_insample_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-25 02:01:29.000000 nixtlats-0.4.0/nixtlats/types/single_series_insample_forecast_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-25 02:01:29.000000 nixtlats-0.4.0/nixtlats/types/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-25 02:01:29.000000 nixtlats-0.4.0/nixtlats/types/validation_error_loc_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-25 02:01:29.000000 nixtlats-0.4.0/nixtlats/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:01:31.044704 nixtlats-0.4.0/nixtlats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-25 02:01:31.000000 nixtlats-0.4.0/nixtlats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-25 02:01:31.000000 nixtlats-0.4.0/nixtlats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 02:01:31.000000 nixtlats-0.4.0/nixtlats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-25 02:01:31.000000 nixtlats-0.4.0/nixtlats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 02:01:31.000000 nixtlats-0.4.0/nixtlats.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 02:01:31.048704 nixtlats-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-25 02:01:29.000000 nixtlats-0.4.0/setup.py
```

### Comparing `nixtlats-0.3.0/LICENSE` & `nixtlats-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nixtlats-0.3.0/PKG-INFO` & `nixtlats-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,95 +1,95 @@
 Metadata-Version: 2.1
 Name: nixtlats
-Version: 0.3.0
+Version: 0.4.0
 Summary: Python SDK for Nixtla API (TimeGPT)
 Home-page: https://github.com/Nixtla/nixtla
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx
 Requires-Dist: pandas
 Requires-Dist: pydantic<2
 Requires-Dist: requests
 Requires-Dist: tenacity
-Requires-Dist: utilsforecast>=0.0.13
+Requires-Dist: utilsforecast>=0.1.7
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: datasetsforecast; extra == "dev"
 Requires-Dist: nbdev; extra == "dev"
 Requires-Dist: plotly; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: python-dotenv; extra == "dev"
 Requires-Dist: statsforecast; extra == "dev"
 Requires-Dist: dask[dataframe]; extra == "dev"
 Requires-Dist: fugue[ray]>=0.8.7; extra == "dev"
 Requires-Dist: pyspark; extra == "dev"
 Requires-Dist: ray[serve-grpc]; extra == "dev"
-Requires-Dist: utilsforecast[plotting]>=0.0.5; extra == "dev"
+Requires-Dist: utilsforecast[plotting]>=0.1.7; extra == "dev"
 Requires-Dist: holidays; extra == "dev"
 Provides-Extra: distributed
 Requires-Dist: dask[dataframe]; extra == "distributed"
 Requires-Dist: fugue[ray]>=0.8.7; extra == "distributed"
 Requires-Dist: pyspark; extra == "distributed"
 Requires-Dist: ray[serve-grpc]; extra == "distributed"
 Provides-Extra: plotting
-Requires-Dist: utilsforecast[plotting]>=0.0.5; extra == "plotting"
+Requires-Dist: utilsforecast[plotting]>=0.1.7; extra == "plotting"
 Provides-Extra: date-extras
 Requires-Dist: holidays; extra == "date-extras"
 
 # Nixtla &nbsp; [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Statistical%20Forecasting%20Algorithms%20by%20Nixtla%20&url=https://github.com/Nixtla/statsforecast&via=nixtlainc&hashtags=StatisticalModels,TimeSeries,Forecasting) &nbsp;[![Slack](https://img.shields.io/badge/Slack-4A154B?&logo=slack&logoColor=white)](https://join.slack.com/t/nixtlacommunity/shared_invite/zt-1pmhan9j5-F54XR20edHk0UtYAPcW4KQ)
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/Nixtla/neuralforecast/main/nbs/imgs_indx/logo_mid.png">
-<h1 align="center">NixtlaTS</h1>
+<h1 align="center">Nixtla</h1>
 <h3 align="center">Forecast using TimeGPT</h3>
     
 [![CI](https://github.com/Nixtla/nixtla/actions/workflows/ci.yaml/badge.svg?branch=main)](https://github.com/Nixtla/nixtla/actions/workflows/ci.yaml)
-[![Python](https://img.shields.io/pypi/pyversions/nixtlats)](https://pypi.org/project/nixtlats/)
-[![PyPi](https://img.shields.io/pypi/v/nixtlats?color=blue)](https://pypi.org/project/nixtlats/)
-[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://github.com/Nixtla/nixtlats/blob/main/LICENSE)
+[![Python](https://img.shields.io/pypi/pyversions/nixtla)](https://pypi.org/project/nixtla/)
+[![PyPi](https://img.shields.io/pypi/v/nixtla?color=blue)](https://pypi.org/project/nixtla/)
+[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://github.com/Nixtla/nixtla/blob/main/LICENSE)
 [![docs](https://img.shields.io/website-up-down-green-red/http/nixtla.github.io/nixtla.svg?label=docs)](https://nixtla.github.io/nixtla/)
-[![Downloads](https://pepy.tech/badge/nixtlats)](https://pepy.tech/project/nixtlats)
+[![Downloads](https://pepy.tech/badge/nixtla)](https://pepy.tech/project/nixtla)
     
-**NixtlaTS** offers a collection of classes and methods to interact with the API of TimeGPT.
+**Nixtla** offers a collection of classes and methods to interact with the API of TimeGPT.
 </div>
 
 # 🕰️ TimeGPT: Revolutionizing Time-Series Analysis
 
 Developed by Nixtla, TimeGPT is a cutting-edge generative pre-trained transformer model dedicated to prediction tasks. 🚀 By leveraging the most extensive dataset ever – financial, weather, energy, and sales data – TimeGPT brings unparalleled time-series analysis right to your terminal! 👩‍💻👨‍💻
 
 In seconds, TimeGPT can discern complex patterns and predict future data points, transforming the landscape of data science and predictive analytics.
 
 ## ⚙️ Fine-Tuning: For Precision Prediction
 
 In addition to its core capabilities, TimeGPT supports fine-tuning, enhancing its specialization for specific prediction tasks. 🎯 This feature is like training a machine learning model on a targeted data subset to improve its task-specific performance, making TimeGPT an even more versatile tool for your predictive needs.
 
-## 🔄 `NixtlaTS`: Your Gateway to TimeGPT
+## 🔄 `Nixtla`: Your Gateway to TimeGPT
 
-With `NixtlaTS`, you can easily interact with TimeGPT through simple API calls, making the power of TimeGPT readily accessible in your projects.
+With `Nixtla`, you can easily interact with TimeGPT through simple API calls, making the power of TimeGPT readily accessible in your projects.
 
 ## 💻 Installation
 
-Get `NixtlaTS` up and running with a simple pip command:
+Get `Nixtla` up and running with a simple pip command:
 
 ```python
-pip install nixtlats>=0.1.0
+pip install nixtla>=0.1.0
 ```
 
 ## 🎈 Quick Start
 
 Get started with TimeGPT now:
 
 ```python
 df = pd.read_csv('https://raw.githubusercontent.com/Nixtla/transfer-learning-time-series/main/datasets/electricity-short.csv')
 
-from nixtlats import NixtlaClient
+from nixtla import NixtlaClient
 nixtla = NixtlaClient(
     # defaults to os.environ.get("NIXTLA_API_KEY")
     api_key = 'my_api_key_provided_by_nixtla'
 )
 fcst_df = nixtla.forecast(df, h=24, level=[80, 90])
 ```
```

### Comparing `nixtlats-0.3.0/README.md` & `nixtlats-0.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 # Nixtla &nbsp; [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Statistical%20Forecasting%20Algorithms%20by%20Nixtla%20&url=https://github.com/Nixtla/statsforecast&via=nixtlainc&hashtags=StatisticalModels,TimeSeries,Forecasting) &nbsp;[![Slack](https://img.shields.io/badge/Slack-4A154B?&logo=slack&logoColor=white)](https://join.slack.com/t/nixtlacommunity/shared_invite/zt-1pmhan9j5-F54XR20edHk0UtYAPcW4KQ)
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/Nixtla/neuralforecast/main/nbs/imgs_indx/logo_mid.png">
-<h1 align="center">NixtlaTS</h1>
+<h1 align="center">Nixtla</h1>
 <h3 align="center">Forecast using TimeGPT</h3>
     
 [![CI](https://github.com/Nixtla/nixtla/actions/workflows/ci.yaml/badge.svg?branch=main)](https://github.com/Nixtla/nixtla/actions/workflows/ci.yaml)
-[![Python](https://img.shields.io/pypi/pyversions/nixtlats)](https://pypi.org/project/nixtlats/)
-[![PyPi](https://img.shields.io/pypi/v/nixtlats?color=blue)](https://pypi.org/project/nixtlats/)
-[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://github.com/Nixtla/nixtlats/blob/main/LICENSE)
+[![Python](https://img.shields.io/pypi/pyversions/nixtla)](https://pypi.org/project/nixtla/)
+[![PyPi](https://img.shields.io/pypi/v/nixtla?color=blue)](https://pypi.org/project/nixtla/)
+[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://github.com/Nixtla/nixtla/blob/main/LICENSE)
 [![docs](https://img.shields.io/website-up-down-green-red/http/nixtla.github.io/nixtla.svg?label=docs)](https://nixtla.github.io/nixtla/)
-[![Downloads](https://pepy.tech/badge/nixtlats)](https://pepy.tech/project/nixtlats)
+[![Downloads](https://pepy.tech/badge/nixtla)](https://pepy.tech/project/nixtla)
     
-**NixtlaTS** offers a collection of classes and methods to interact with the API of TimeGPT.
+**Nixtla** offers a collection of classes and methods to interact with the API of TimeGPT.
 </div>
 
 # 🕰️ TimeGPT: Revolutionizing Time-Series Analysis
 
 Developed by Nixtla, TimeGPT is a cutting-edge generative pre-trained transformer model dedicated to prediction tasks. 🚀 By leveraging the most extensive dataset ever – financial, weather, energy, and sales data – TimeGPT brings unparalleled time-series analysis right to your terminal! 👩‍💻👨‍💻
 
 In seconds, TimeGPT can discern complex patterns and predict future data points, transforming the landscape of data science and predictive analytics.
 
 ## ⚙️ Fine-Tuning: For Precision Prediction
 
 In addition to its core capabilities, TimeGPT supports fine-tuning, enhancing its specialization for specific prediction tasks. 🎯 This feature is like training a machine learning model on a targeted data subset to improve its task-specific performance, making TimeGPT an even more versatile tool for your predictive needs.
 
-## 🔄 `NixtlaTS`: Your Gateway to TimeGPT
+## 🔄 `Nixtla`: Your Gateway to TimeGPT
 
-With `NixtlaTS`, you can easily interact with TimeGPT through simple API calls, making the power of TimeGPT readily accessible in your projects.
+With `Nixtla`, you can easily interact with TimeGPT through simple API calls, making the power of TimeGPT readily accessible in your projects.
 
 ## 💻 Installation
 
-Get `NixtlaTS` up and running with a simple pip command:
+Get `Nixtla` up and running with a simple pip command:
 
 ```python
-pip install nixtlats>=0.1.0
+pip install nixtla>=0.1.0
 ```
 
 ## 🎈 Quick Start
 
 Get started with TimeGPT now:
 
 ```python
 df = pd.read_csv('https://raw.githubusercontent.com/Nixtla/transfer-learning-time-series/main/datasets/electricity-short.csv')
 
-from nixtlats import NixtlaClient
+from nixtla import NixtlaClient
 nixtla = NixtlaClient(
     # defaults to os.environ.get("NIXTLA_API_KEY")
     api_key = 'my_api_key_provided_by_nixtla'
 )
 fcst_df = nixtla.forecast(df, h=24, level=[80, 90])
 ```
```

### Comparing `nixtlats-0.3.0/nixtlats/_modidx.py` & `nixtlats-0.4.0/nixtlats/_modidx.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,164 +1,161 @@
 # Autogenerated by nbdev
 
 d = { 'settings': { 'branch': 'main',
-                'doc_baseurl': '/nixtlats/',
+                'doc_baseurl': '/nixtla/',
                 'doc_host': 'https://Nixtla.github.io',
                 'git_url': 'https://github.com/Nixtla/nixtla/',
-                'lib_path': 'nixtlats'},
-  'syms': { 'nixtlats.client': {},
-            'nixtlats.core.api_error': {},
-            'nixtlats.core.client_wrapper': {},
-            'nixtlats.core.datetime_utils': {},
-            'nixtlats.core.jsonable_encoder': {},
-            'nixtlats.core.remove_none_from_dict': {},
-            'nixtlats.date_features': { 'nixtlats.date_features.CountryHolidays': ( 'date_features.html#countryholidays',
-                                                                                    'nixtlats/date_features.py'),
-                                        'nixtlats.date_features.CountryHolidays.__call__': ( 'date_features.html#countryholidays.__call__',
-                                                                                             'nixtlats/date_features.py'),
-                                        'nixtlats.date_features.CountryHolidays.__init__': ( 'date_features.html#countryholidays.__init__',
-                                                                                             'nixtlats/date_features.py'),
-                                        'nixtlats.date_features.CountryHolidays.__name__': ( 'date_features.html#countryholidays.__name__',
-                                                                                             'nixtlats/date_features.py'),
-                                        'nixtlats.date_features.SpecialDates': ( 'date_features.html#specialdates',
-                                                                                 'nixtlats/date_features.py'),
-                                        'nixtlats.date_features.SpecialDates.__call__': ( 'date_features.html#specialdates.__call__',
-                                                                                          'nixtlats/date_features.py'),
-                                        'nixtlats.date_features.SpecialDates.__init__': ( 'date_features.html#specialdates.__init__',
-                                                                                          'nixtlats/date_features.py'),
-                                        'nixtlats.date_features.SpecialDates.__name__': ( 'date_features.html#specialdates.__name__',
-                                                                                          'nixtlats/date_features.py'),
-                                        'nixtlats.date_features._get_holidays_df': ( 'date_features.html#_get_holidays_df',
-                                                                                     'nixtlats/date_features.py'),
-                                        'nixtlats.date_features._transform_dict_holidays': ( 'date_features.html#_transform_dict_holidays',
-                                                                                             'nixtlats/date_features.py')},
-            'nixtlats.distributed.nixtla_client': { 'nixtlats.distributed.nixtla_client._DistributedNixtlaClient': ( 'distributed.nixtla_client.html#_distributednixtlaclient',
-                                                                                                                     'nixtlats/distributed/nixtla_client.py'),
-                                                    'nixtlats.distributed.nixtla_client._DistributedNixtlaClient.__init__': ( 'distributed.nixtla_client.html#_distributednixtlaclient.__init__',
-                                                                                                                              'nixtlats/distributed/nixtla_client.py'),
-                                                    'nixtlats.distributed.nixtla_client._DistributedNixtlaClient._cross_validation': ( 'distributed.nixtla_client.html#_distributednixtlaclient._cross_validation',
-                                                                                                                                       'nixtlats/distributed/nixtla_client.py'),
-                                                    'nixtlats.distributed.nixtla_client._DistributedNixtlaClient._detect_anomalies': ( 'distributed.nixtla_client.html#_distributednixtlaclient._detect_anomalies',
-                                                                                                                                       'nixtlats/distributed/nixtla_client.py'),
-                                                    'nixtlats.distributed.nixtla_client._DistributedNixtlaClient._distribute_method': ( 'distributed.nixtla_client.html#_distributednixtlaclient._distribute_method',
-                                                                                                                                        'nixtlats/distributed/nixtla_client.py'),
-                                                    'nixtlats.distributed.nixtla_client._DistributedNixtlaClient._forecast': ( 'distributed.nixtla_client.html#_distributednixtlaclient._forecast',
-                                                                                                                               'nixtlats/distributed/nixtla_client.py'),
-                                                    'nixtlats.distributed.nixtla_client._DistributedNixtlaClient._forecast_x': ( 'distributed.nixtla_client.html#_distributednixtlaclient._forecast_x',
-                                                                                                                                 'nixtlats/distributed/nixtla_client.py'),
-                                                    'nixtlats.distributed.nixtla_client._DistributedNixtlaClient._get_anomalies_schema': ( 'distributed.nixtla_client.html#_distributednixtlaclient._get_anomalies_schema',
-                                                                                                                                           'nixtlats/distributed/nixtla_client.py'),
-                                                    'nixtlats.distributed.nixtla_client._DistributedNixtlaClient._get_forecast_schema': ( 'distributed.nixtla_client.html#_distributednixtlaclient._get_forecast_schema',
-                                                                                                                                          'nixtlats/distributed/nixtla_client.py'),
-                                                    'nixtlats.distributed.nixtla_client._DistributedNixtlaClient._instantiate_nixtla_client': ( 'distributed.nixtla_client.html#_distributednixtlaclient._instantiate_nixtla_client',
-                                                                                                                                                'nixtlats/distributed/nixtla_client.py'),
-                                                    'nixtlats.distributed.nixtla_client._DistributedNixtlaClient.cross_validation': ( 'distributed.nixtla_client.html#_distributednixtlaclient.cross_validation',
-                                                                                                                                      'nixtlats/distributed/nixtla_client.py'),
-                                                    'nixtlats.distributed.nixtla_client._DistributedNixtlaClient.detect_anomalies': ( 'distributed.nixtla_client.html#_distributednixtlaclient.detect_anomalies',
-                                                                                                                                      'nixtlats/distributed/nixtla_client.py'),
-                                                    'nixtlats.distributed.nixtla_client._DistributedNixtlaClient.forecast': ( 'distributed.nixtla_client.html#_distributednixtlaclient.forecast',
-                                                                                                                              'nixtlats/distributed/nixtla_client.py'),
-                                                    'nixtlats.distributed.nixtla_client._cotransform': ( 'distributed.nixtla_client.html#_cotransform',
-                                                                                                         'nixtlats/distributed/nixtla_client.py')},
-            'nixtlats.errors.unprocessable_entity_error': {},
-            'nixtlats.nixtla_client': { 'nixtlats.nixtla_client.NixtlaClient': ( 'nixtla_client.html#nixtlaclient',
-                                                                                 'nixtlats/nixtla_client.py'),
-                                        'nixtlats.nixtla_client.NixtlaClient._instantiate_distributed_nixtla_client': ( 'nixtla_client.html#nixtlaclient._instantiate_distributed_nixtla_client',
-                                                                                                                        'nixtlats/nixtla_client.py'),
-                                        'nixtlats.nixtla_client.NixtlaClient.cross_validation': ( 'nixtla_client.html#nixtlaclient.cross_validation',
-                                                                                                  'nixtlats/nixtla_client.py'),
-                                        'nixtlats.nixtla_client.NixtlaClient.detect_anomalies': ( 'nixtla_client.html#nixtlaclient.detect_anomalies',
-                                                                                                  'nixtlats/nixtla_client.py'),
-                                        'nixtlats.nixtla_client.NixtlaClient.forecast': ( 'nixtla_client.html#nixtlaclient.forecast',
-                                                                                          'nixtlats/nixtla_client.py'),
-                                        'nixtlats.nixtla_client.TimeGPT': ('nixtla_client.html#timegpt', 'nixtlats/nixtla_client.py'),
-                                        'nixtlats.nixtla_client.TimeGPT.__init__': ( 'nixtla_client.html#timegpt.__init__',
-                                                                                     'nixtlats/nixtla_client.py'),
-                                        'nixtlats.nixtla_client._NixtlaClient': ( 'nixtla_client.html#_nixtlaclient',
-                                                                                  'nixtlats/nixtla_client.py'),
-                                        'nixtlats.nixtla_client._NixtlaClient.__init__': ( 'nixtla_client.html#_nixtlaclient.__init__',
-                                                                                           'nixtlats/nixtla_client.py'),
-                                        'nixtlats.nixtla_client._NixtlaClient._cross_validation': ( 'nixtla_client.html#_nixtlaclient._cross_validation',
-                                                                                                    'nixtlats/nixtla_client.py'),
-                                        'nixtlats.nixtla_client._NixtlaClient._detect_anomalies': ( 'nixtla_client.html#_nixtlaclient._detect_anomalies',
-                                                                                                    'nixtlats/nixtla_client.py'),
-                                        'nixtlats.nixtla_client._NixtlaClient._forecast': ( 'nixtla_client.html#_nixtlaclient._forecast',
-                                                                                            'nixtlats/nixtla_client.py'),
-                                        'nixtlats.nixtla_client._NixtlaClient.plot': ( 'nixtla_client.html#_nixtlaclient.plot',
-                                                                                       'nixtlats/nixtla_client.py'),
-                                        'nixtlats.nixtla_client._NixtlaClient.validate_api_key': ( 'nixtla_client.html#_nixtlaclient.validate_api_key',
-                                                                                                   'nixtlats/nixtla_client.py'),
-                                        'nixtlats.nixtla_client._NixtlaClient.validate_token': ( 'nixtla_client.html#_nixtlaclient.validate_token',
-                                                                                                 'nixtlats/nixtla_client.py'),
-                                        'nixtlats.nixtla_client._NixtlaClientModel': ( 'nixtla_client.html#_nixtlaclientmodel',
-                                                                                       'nixtlats/nixtla_client.py'),
-                                        'nixtlats.nixtla_client._NixtlaClientModel.__init__': ( 'nixtla_client.html#_nixtlaclientmodel.__init__',
-                                                                                                'nixtlats/nixtla_client.py'),
-                                        'nixtlats.nixtla_client._NixtlaClientModel._call_api': ( 'nixtla_client.html#_nixtlaclientmodel._call_api',
-                                                                                                 'nixtlats/nixtla_client.py'),
-                                        'nixtlats.nixtla_client._NixtlaClientModel._prepare_level_and_quantiles': ( 'nixtla_client.html#_nixtlaclientmodel._prepare_level_and_quantiles',
-                                                                                                                    'nixtlats/nixtla_client.py'),
-                                        'nixtlats.nixtla_client._NixtlaClientModel._retry_strategy': ( 'nixtla_client.html#_nixtlaclientmodel._retry_strategy',
-                                                                                                       'nixtlats/nixtla_client.py'),
-                                        'nixtlats.nixtla_client._NixtlaClientModel.add_date_features': ( 'nixtla_client.html#_nixtlaclientmodel.add_date_features',
-                                                                                                         'nixtlats/nixtla_client.py'),
-                                        'nixtlats.nixtla_client._NixtlaClientModel.compute_date_feature': ( 'nixtla_client.html#_nixtlaclientmodel.compute_date_feature',
-                                                                                                            'nixtlats/nixtla_client.py'),
-                                        'nixtlats.nixtla_client._NixtlaClientModel.cross_validation': ( 'nixtla_client.html#_nixtlaclientmodel.cross_validation',
-                                                                                                        'nixtlats/nixtla_client.py'),
-                                        'nixtlats.nixtla_client._NixtlaClientModel.dataframes_to_dict': ( 'nixtla_client.html#_nixtlaclientmodel.dataframes_to_dict',
-                                                                                                          'nixtlats/nixtla_client.py'),
-                                        'nixtlats.nixtla_client._NixtlaClientModel.detect_anomalies': ( 'nixtla_client.html#_nixtlaclientmodel.detect_anomalies',
-                                                                                                        'nixtlats/nixtla_client.py'),
-                                        'nixtlats.nixtla_client._NixtlaClientModel.forecast': ( 'nixtla_client.html#_nixtlaclientmodel.forecast',
-                                                                                                'nixtlats/nixtla_client.py'),
-                                        'nixtlats.nixtla_client._NixtlaClientModel.infer_freq': ( 'nixtla_client.html#_nixtlaclientmodel.infer_freq',
-                                                                                                  'nixtlats/nixtla_client.py'),
-                                        'nixtlats.nixtla_client._NixtlaClientModel.make_future_dataframe': ( 'nixtla_client.html#_nixtlaclientmodel.make_future_dataframe',
-                                                                                                             'nixtlats/nixtla_client.py'),
-                                        'nixtlats.nixtla_client._NixtlaClientModel.preprocess_X_df': ( 'nixtla_client.html#_nixtlaclientmodel.preprocess_x_df',
-                                                                                                       'nixtlats/nixtla_client.py'),
-                                        'nixtlats.nixtla_client._NixtlaClientModel.preprocess_dataframes': ( 'nixtla_client.html#_nixtlaclientmodel.preprocess_dataframes',
-                                                                                                             'nixtlats/nixtla_client.py'),
-                                        'nixtlats.nixtla_client._NixtlaClientModel.resample_dataframe': ( 'nixtla_client.html#_nixtlaclientmodel.resample_dataframe',
-                                                                                                          'nixtlats/nixtla_client.py'),
-                                        'nixtlats.nixtla_client._NixtlaClientModel.set_model_params': ( 'nixtla_client.html#_nixtlaclientmodel.set_model_params',
-                                                                                                        'nixtlats/nixtla_client.py'),
-                                        'nixtlats.nixtla_client._NixtlaClientModel.transform_inputs': ( 'nixtla_client.html#_nixtlaclientmodel.transform_inputs',
-                                                                                                        'nixtlats/nixtla_client.py'),
-                                        'nixtlats.nixtla_client._NixtlaClientModel.transform_outputs': ( 'nixtla_client.html#_nixtlaclientmodel.transform_outputs',
-                                                                                                         'nixtlats/nixtla_client.py'),
-                                        'nixtlats.nixtla_client._NixtlaClientModel.validate_input_size': ( 'nixtla_client.html#_nixtlaclientmodel.validate_input_size',
-                                                                                                           'nixtlats/nixtla_client.py'),
-                                        'nixtlats.nixtla_client.deprecated_argument': ( 'nixtla_client.html#deprecated_argument',
-                                                                                        'nixtlats/nixtla_client.py'),
-                                        'nixtlats.nixtla_client.deprecated_method': ( 'nixtla_client.html#deprecated_method',
-                                                                                      'nixtlats/nixtla_client.py'),
-                                        'nixtlats.nixtla_client.partition_by_uid': ( 'nixtla_client.html#partition_by_uid',
-                                                                                     'nixtlats/nixtla_client.py'),
-                                        'nixtlats.nixtla_client.remove_unused_categories': ( 'nixtla_client.html#remove_unused_categories',
-                                                                                             'nixtlats/nixtla_client.py'),
-                                        'nixtlats.nixtla_client.validate_model_parameter': ( 'nixtla_client.html#validate_model_parameter',
-                                                                                             'nixtlats/nixtla_client.py')},
-            'nixtlats.types.http_validation_error': {},
-            'nixtlats.types.multi_series_anomaly': {},
-            'nixtlats.types.multi_series_anomaly_model': {},
-            'nixtlats.types.multi_series_cross_validation': {},
-            'nixtlats.types.multi_series_cross_validation_fewshot_loss': {},
-            'nixtlats.types.multi_series_cross_validation_finetune_loss': {},
-            'nixtlats.types.multi_series_cross_validation_model': {},
-            'nixtlats.types.multi_series_forecast': {},
-            'nixtlats.types.multi_series_forecast_fewshot_loss': {},
-            'nixtlats.types.multi_series_forecast_finetune_loss': {},
-            'nixtlats.types.multi_series_forecast_model': {},
-            'nixtlats.types.multi_series_input': {},
-            'nixtlats.types.multi_series_insample_forecast': {},
-            'nixtlats.types.multi_series_insample_forecast_model': {},
-            'nixtlats.types.single_series_forecast': {},
-            'nixtlats.types.single_series_forecast_fewshot_loss': {},
-            'nixtlats.types.single_series_forecast_finetune_loss': {},
-            'nixtlats.types.single_series_forecast_model': {},
-            'nixtlats.types.single_series_insample_forecast': {},
-            'nixtlats.types.single_series_insample_forecast_model': {},
-            'nixtlats.types.validation_error': {},
-            'nixtlats.types.validation_error_loc_item': {},
-            'nixtlats.utils': {'nixtlats.utils.colab_badge': ('utils.html#colab_badge', 'nixtlats/utils.py')}}}
+                'lib_path': 'nixtla'},
+  'syms': { 'nixtla.client': {},
+            'nixtla.core.api_error': {},
+            'nixtla.core.client_wrapper': {},
+            'nixtla.core.datetime_utils': {},
+            'nixtla.core.jsonable_encoder': {},
+            'nixtla.core.remove_none_from_dict': {},
+            'nixtla.date_features': { 'nixtla.date_features.CountryHolidays': ( 'date_features.html#countryholidays',
+                                                                                'nixtla/date_features.py'),
+                                      'nixtla.date_features.CountryHolidays.__call__': ( 'date_features.html#countryholidays.__call__',
+                                                                                         'nixtla/date_features.py'),
+                                      'nixtla.date_features.CountryHolidays.__init__': ( 'date_features.html#countryholidays.__init__',
+                                                                                         'nixtla/date_features.py'),
+                                      'nixtla.date_features.CountryHolidays.__name__': ( 'date_features.html#countryholidays.__name__',
+                                                                                         'nixtla/date_features.py'),
+                                      'nixtla.date_features.SpecialDates': ('date_features.html#specialdates', 'nixtla/date_features.py'),
+                                      'nixtla.date_features.SpecialDates.__call__': ( 'date_features.html#specialdates.__call__',
+                                                                                      'nixtla/date_features.py'),
+                                      'nixtla.date_features.SpecialDates.__init__': ( 'date_features.html#specialdates.__init__',
+                                                                                      'nixtla/date_features.py'),
+                                      'nixtla.date_features.SpecialDates.__name__': ( 'date_features.html#specialdates.__name__',
+                                                                                      'nixtla/date_features.py'),
+                                      'nixtla.date_features._get_holidays_df': ( 'date_features.html#_get_holidays_df',
+                                                                                 'nixtla/date_features.py'),
+                                      'nixtla.date_features._transform_dict_holidays': ( 'date_features.html#_transform_dict_holidays',
+                                                                                         'nixtla/date_features.py')},
+            'nixtla.distributed.nixtla_client': { 'nixtla.distributed.nixtla_client._DistributedNixtlaClient': ( 'distributed.nixtla_client.html#_distributednixtlaclient',
+                                                                                                                 'nixtla/distributed/nixtla_client.py'),
+                                                  'nixtla.distributed.nixtla_client._DistributedNixtlaClient.__init__': ( 'distributed.nixtla_client.html#_distributednixtlaclient.__init__',
+                                                                                                                          'nixtla/distributed/nixtla_client.py'),
+                                                  'nixtla.distributed.nixtla_client._DistributedNixtlaClient._cross_validation': ( 'distributed.nixtla_client.html#_distributednixtlaclient._cross_validation',
+                                                                                                                                   'nixtla/distributed/nixtla_client.py'),
+                                                  'nixtla.distributed.nixtla_client._DistributedNixtlaClient._detect_anomalies': ( 'distributed.nixtla_client.html#_distributednixtlaclient._detect_anomalies',
+                                                                                                                                   'nixtla/distributed/nixtla_client.py'),
+                                                  'nixtla.distributed.nixtla_client._DistributedNixtlaClient._distribute_method': ( 'distributed.nixtla_client.html#_distributednixtlaclient._distribute_method',
+                                                                                                                                    'nixtla/distributed/nixtla_client.py'),
+                                                  'nixtla.distributed.nixtla_client._DistributedNixtlaClient._forecast': ( 'distributed.nixtla_client.html#_distributednixtlaclient._forecast',
+                                                                                                                           'nixtla/distributed/nixtla_client.py'),
+                                                  'nixtla.distributed.nixtla_client._DistributedNixtlaClient._forecast_x': ( 'distributed.nixtla_client.html#_distributednixtlaclient._forecast_x',
+                                                                                                                             'nixtla/distributed/nixtla_client.py'),
+                                                  'nixtla.distributed.nixtla_client._DistributedNixtlaClient._get_anomalies_schema': ( 'distributed.nixtla_client.html#_distributednixtlaclient._get_anomalies_schema',
+                                                                                                                                       'nixtla/distributed/nixtla_client.py'),
+                                                  'nixtla.distributed.nixtla_client._DistributedNixtlaClient._get_forecast_schema': ( 'distributed.nixtla_client.html#_distributednixtlaclient._get_forecast_schema',
+                                                                                                                                      'nixtla/distributed/nixtla_client.py'),
+                                                  'nixtla.distributed.nixtla_client._DistributedNixtlaClient._instantiate_nixtla_client': ( 'distributed.nixtla_client.html#_distributednixtlaclient._instantiate_nixtla_client',
+                                                                                                                                            'nixtla/distributed/nixtla_client.py'),
+                                                  'nixtla.distributed.nixtla_client._DistributedNixtlaClient.cross_validation': ( 'distributed.nixtla_client.html#_distributednixtlaclient.cross_validation',
+                                                                                                                                  'nixtla/distributed/nixtla_client.py'),
+                                                  'nixtla.distributed.nixtla_client._DistributedNixtlaClient.detect_anomalies': ( 'distributed.nixtla_client.html#_distributednixtlaclient.detect_anomalies',
+                                                                                                                                  'nixtla/distributed/nixtla_client.py'),
+                                                  'nixtla.distributed.nixtla_client._DistributedNixtlaClient.forecast': ( 'distributed.nixtla_client.html#_distributednixtlaclient.forecast',
+                                                                                                                          'nixtla/distributed/nixtla_client.py'),
+                                                  'nixtla.distributed.nixtla_client._cotransform': ( 'distributed.nixtla_client.html#_cotransform',
+                                                                                                     'nixtla/distributed/nixtla_client.py')},
+            'nixtla.errors.unprocessable_entity_error': {},
+            'nixtla.nixtla_client': { 'nixtla.nixtla_client.NixtlaClient': ('nixtla_client.html#nixtlaclient', 'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client.NixtlaClient._instantiate_distributed_nixtla_client': ( 'nixtla_client.html#nixtlaclient._instantiate_distributed_nixtla_client',
+                                                                                                                    'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client.NixtlaClient.cross_validation': ( 'nixtla_client.html#nixtlaclient.cross_validation',
+                                                                                              'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client.NixtlaClient.detect_anomalies': ( 'nixtla_client.html#nixtlaclient.detect_anomalies',
+                                                                                              'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client.NixtlaClient.forecast': ( 'nixtla_client.html#nixtlaclient.forecast',
+                                                                                      'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client.TimeGPT': ('nixtla_client.html#timegpt', 'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client.TimeGPT.__init__': ( 'nixtla_client.html#timegpt.__init__',
+                                                                                 'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client._NixtlaClient': ('nixtla_client.html#_nixtlaclient', 'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client._NixtlaClient.__init__': ( 'nixtla_client.html#_nixtlaclient.__init__',
+                                                                                       'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client._NixtlaClient._cross_validation': ( 'nixtla_client.html#_nixtlaclient._cross_validation',
+                                                                                                'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client._NixtlaClient._detect_anomalies': ( 'nixtla_client.html#_nixtlaclient._detect_anomalies',
+                                                                                                'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client._NixtlaClient._forecast': ( 'nixtla_client.html#_nixtlaclient._forecast',
+                                                                                        'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client._NixtlaClient.plot': ( 'nixtla_client.html#_nixtlaclient.plot',
+                                                                                   'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client._NixtlaClient.validate_api_key': ( 'nixtla_client.html#_nixtlaclient.validate_api_key',
+                                                                                               'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client._NixtlaClient.validate_token': ( 'nixtla_client.html#_nixtlaclient.validate_token',
+                                                                                             'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client._NixtlaClientModel': ( 'nixtla_client.html#_nixtlaclientmodel',
+                                                                                   'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client._NixtlaClientModel.__init__': ( 'nixtla_client.html#_nixtlaclientmodel.__init__',
+                                                                                            'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client._NixtlaClientModel._call_api': ( 'nixtla_client.html#_nixtlaclientmodel._call_api',
+                                                                                             'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client._NixtlaClientModel._prepare_level_and_quantiles': ( 'nixtla_client.html#_nixtlaclientmodel._prepare_level_and_quantiles',
+                                                                                                                'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client._NixtlaClientModel._retry_strategy': ( 'nixtla_client.html#_nixtlaclientmodel._retry_strategy',
+                                                                                                   'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client._NixtlaClientModel.add_date_features': ( 'nixtla_client.html#_nixtlaclientmodel.add_date_features',
+                                                                                                     'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client._NixtlaClientModel.compute_date_feature': ( 'nixtla_client.html#_nixtlaclientmodel.compute_date_feature',
+                                                                                                        'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client._NixtlaClientModel.cross_validation': ( 'nixtla_client.html#_nixtlaclientmodel.cross_validation',
+                                                                                                    'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client._NixtlaClientModel.dataframes_to_dict': ( 'nixtla_client.html#_nixtlaclientmodel.dataframes_to_dict',
+                                                                                                      'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client._NixtlaClientModel.detect_anomalies': ( 'nixtla_client.html#_nixtlaclientmodel.detect_anomalies',
+                                                                                                    'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client._NixtlaClientModel.forecast': ( 'nixtla_client.html#_nixtlaclientmodel.forecast',
+                                                                                            'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client._NixtlaClientModel.infer_freq': ( 'nixtla_client.html#_nixtlaclientmodel.infer_freq',
+                                                                                              'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client._NixtlaClientModel.make_future_dataframe': ( 'nixtla_client.html#_nixtlaclientmodel.make_future_dataframe',
+                                                                                                         'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client._NixtlaClientModel.preprocess_X_df': ( 'nixtla_client.html#_nixtlaclientmodel.preprocess_x_df',
+                                                                                                   'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client._NixtlaClientModel.preprocess_dataframes': ( 'nixtla_client.html#_nixtlaclientmodel.preprocess_dataframes',
+                                                                                                         'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client._NixtlaClientModel.resample_dataframe': ( 'nixtla_client.html#_nixtlaclientmodel.resample_dataframe',
+                                                                                                      'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client._NixtlaClientModel.set_model_params': ( 'nixtla_client.html#_nixtlaclientmodel.set_model_params',
+                                                                                                    'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client._NixtlaClientModel.transform_inputs': ( 'nixtla_client.html#_nixtlaclientmodel.transform_inputs',
+                                                                                                    'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client._NixtlaClientModel.transform_outputs': ( 'nixtla_client.html#_nixtlaclientmodel.transform_outputs',
+                                                                                                     'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client._NixtlaClientModel.validate_input_size': ( 'nixtla_client.html#_nixtlaclientmodel.validate_input_size',
+                                                                                                       'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client.deprecated_argument': ( 'nixtla_client.html#deprecated_argument',
+                                                                                    'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client.deprecated_method': ( 'nixtla_client.html#deprecated_method',
+                                                                                  'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client.partition_by_uid': ( 'nixtla_client.html#partition_by_uid',
+                                                                                 'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client.remove_unused_categories': ( 'nixtla_client.html#remove_unused_categories',
+                                                                                         'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client.validate_model_parameter': ( 'nixtla_client.html#validate_model_parameter',
+                                                                                         'nixtla/nixtla_client.py')},
+            'nixtla.types.http_validation_error': {},
+            'nixtla.types.multi_series_anomaly': {},
+            'nixtla.types.multi_series_anomaly_model': {},
+            'nixtla.types.multi_series_cross_validation': {},
+            'nixtla.types.multi_series_cross_validation_fewshot_loss': {},
+            'nixtla.types.multi_series_cross_validation_finetune_loss': {},
+            'nixtla.types.multi_series_cross_validation_model': {},
+            'nixtla.types.multi_series_forecast': {},
+            'nixtla.types.multi_series_forecast_fewshot_loss': {},
+            'nixtla.types.multi_series_forecast_finetune_loss': {},
+            'nixtla.types.multi_series_forecast_model': {},
+            'nixtla.types.multi_series_input': {},
+            'nixtla.types.multi_series_insample_forecast': {},
+            'nixtla.types.multi_series_insample_forecast_model': {},
+            'nixtla.types.single_series_forecast': {},
+            'nixtla.types.single_series_forecast_fewshot_loss': {},
+            'nixtla.types.single_series_forecast_finetune_loss': {},
+            'nixtla.types.single_series_forecast_model': {},
+            'nixtla.types.single_series_insample_forecast': {},
+            'nixtla.types.single_series_insample_forecast_model': {},
+            'nixtla.types.validation_error': {},
+            'nixtla.types.validation_error_loc_item': {},
+            'nixtla.utils': {'nixtla.utils.colab_badge': ('utils.html#colab_badge', 'nixtla/utils.py')}}}
```

### Comparing `nixtlats-0.3.0/nixtlats/client.py` & `nixtlats-0.4.0/nixtlats/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,32 @@
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+    def health_health_get(self) -> typing.Any:
+        """
+        Check if server is healthy. Used by the readiness probe to check server is healthy.
+        """
+        _response = self._client_wrapper.httpx_client.request(
+            "GET",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "health"),
+            headers=self._client_wrapper.get_headers(),
+            timeout=60,
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
     def forecast(self, *, request: SingleSeriesForecast) -> typing.Any:
         """
         This endpoint predicts the future values of a single time series based on the provided data. It takes a JSON as an input containing information like the series frequency and historical data. (See below for a full description of the parameters.) The response contains the predicted values based on the input arguments. Get your token for private beta at https://dashboard.nixtla.io
 
         Parameters:
             - request: SingleSeriesForecast.
         """
@@ -468,14 +486,32 @@
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def health_health_get(self) -> typing.Any:
+        """
+        Check if server is healthy. Used by the readiness probe to check server is healthy.
+        """
+        _response = await self._client_wrapper.httpx_client.request(
+            "GET",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "health"),
+            headers=self._client_wrapper.get_headers(),
+            timeout=60,
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+        try:
+            _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def forecast(self, *, request: SingleSeriesForecast) -> typing.Any:
         """
         This endpoint predicts the future values of a single time series based on the provided data. It takes a JSON as an input containing information like the series frequency and historical data. (See below for a full description of the parameters.) The response contains the predicted values based on the input arguments. Get your token for private beta at https://dashboard.nixtla.io
```

### Comparing `nixtlats-0.3.0/nixtlats/core/__init__.py` & `nixtlats-0.4.0/nixtlats/core/__init__.py`

 * *Files identical despite different names*

### Comparing `nixtlats-0.3.0/nixtlats/core/client_wrapper.py` & `nixtlats-0.4.0/nixtlats/core/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `nixtlats-0.3.0/nixtlats/core/datetime_utils.py` & `nixtlats-0.4.0/nixtlats/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `nixtlats-0.3.0/nixtlats/core/jsonable_encoder.py` & `nixtlats-0.4.0/nixtlats/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `nixtlats-0.3.0/nixtlats/date_features.py` & `nixtlats-0.4.0/nixtlats/date_features.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     def __call__(self, dates: pd.DatetimeIndex):
         try:
             from holidays.utils import country_holidays
             from holidays.utils import list_supported_countries
         except ModuleNotFoundError:
             raise Exception(
                 "You have to install additional libraries to use holidays, "
-                'please install them using `pip install "nixtlats[date_extras]"`'
+                'please install them using `pip install "nixtla[date_extras]"`'
             )
         return _get_holidays_df(
             dates, self.countries, country_holidays, list_supported_countries()
         )
 
     def __name__(self):
         return "CountryHolidays"
```

### Comparing `nixtlats-0.3.0/nixtlats/distributed/nixtla_client.py` & `nixtlats-0.4.0/nixtlats/distributed/nixtla_client.py`

 * *Files identical despite different names*

### Comparing `nixtlats-0.3.0/nixtlats/nixtla_client.py` & `nixtlats-0.4.0/nixtlats/nixtla_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,42 +9,46 @@
 import json
 import logging
 import os
 import requests
 import warnings
 from typing import Dict, List, Optional, Union
 
+from functools import partial, wraps
+from multiprocessing import cpu_count
+from concurrent.futures import ThreadPoolExecutor
+from threading import Lock
+
 import numpy as np
 import pandas as pd
 from tenacity import (
     retry,
     stop_after_attempt,
     wait_fixed,
     stop_after_delay,
     RetryCallState,
     retry_if_exception,
     retry_if_not_exception_type,
 )
+from utilsforecast.preprocessing import fill_gaps
 from utilsforecast.processing import (
     backtest_splits,
     drop_index_if_pandas,
     join,
     maybe_compute_sort_indices,
     take_rows,
     vertical_concat,
 )
 
-from nixtlats.client import (
-    ApiError,
-    Nixtla,
-    SingleSeriesForecast,
-    MultiSeriesForecast,
-    MultiSeriesAnomaly,
-    MultiSeriesInsampleForecast,
-)
+from .client import Nixtla
+from .core import ApiError
+from .types.multi_series_anomaly import MultiSeriesAnomaly
+from .types.multi_series_forecast import MultiSeriesForecast
+from .types.multi_series_insample_forecast import MultiSeriesInsampleForecast
+from .types.single_series_forecast import SingleSeriesForecast
 
 logging.basicConfig(level=logging.INFO)
 main_logger = logging.getLogger(__name__)
 httpx_logger = logging.getLogger("httpx")
 httpx_logger.setLevel(logging.ERROR)
 
 # %% ../nbs/nixtla_client.ipynb 5
@@ -326,20 +330,29 @@
                     raise Exception(
                         f"Failed to infer special date, inferred freq {inferred_freq}"
                     )
             main_logger.info(f"Inferred freq: {inferred_freq}")
             self.freq = inferred_freq
 
     def resample_dataframe(self, df: pd.DataFrame):
-        df = df.copy()
-        df["ds"] = pd.to_datetime(df["ds"])
-        resampled_df = (
-            df.set_index("ds").groupby("unique_id").resample(self.freq).bfill()
+        if not pd.api.types.is_datetime64_any_dtype(df["ds"].dtype):
+            df = df.copy(deep=False)
+            df["ds"] = pd.to_datetime(df["ds"])
+        resampled_df = fill_gaps(
+            df,
+            freq=self.freq,
+            start="per_serie",
+            end="per_serie",
+            id_col="unique_id",
+            time_col="ds",
         )
-        resampled_df = resampled_df.drop(columns="unique_id").reset_index()
+        numeric_cols = resampled_df.columns.drop(["unique_id", "ds"])
+        resampled_df[numeric_cols] = resampled_df.groupby("unique_id", observed=True)[
+            numeric_cols
+        ].bfill()
         resampled_df["ds"] = resampled_df["ds"].astype(str)
         return resampled_df
 
     def make_future_dataframe(self, df: pd.DataFrame, reconvert: bool = True):
         last_dates = df.groupby("unique_id")["ds"].max()
 
         def _future_date_range(last_date):
@@ -460,15 +473,15 @@
         if Y_df["y"].isna().any():
             raise Exception("Your target variable contains NA, please check")
         # Azul: efficient this code
         # and think about returning dates that are not in the training set
         Y_df = self.resample_dataframe(Y_df)
         x_cols = []
         if X_df is not None:
-            x_cols = X_df.drop(columns=["unique_id", "ds"]).columns.to_list()
+            x_cols = X_df.columns.drop(["unique_id", "ds"]).to_list()
             if not all(col in df.columns for col in x_cols):
                 raise Exception(
                     "You must include the exogenous variables in the `df` object, "
                     f'exogenous variables {",".join(x_cols)}'
                 )
             if (self.h is not None) and (
                 len(X_df) != df["unique_id"].nunique() * self.h
@@ -747,31 +760,60 @@
 # %% ../nbs/nixtla_client.ipynb 13
 def partition_by_uid(func):
     def wrapper(self, num_partitions, **kwargs):
         if num_partitions is None or num_partitions == 1:
             return func(self, **kwargs, num_partitions=1)
         df = kwargs.pop("df")
         X_df = kwargs.pop("X_df", None)
-        id_col = kwargs["id_col"]
+        id_col = kwargs.pop("id_col")
         uids = df["unique_id"].unique()
-        results_df = []
-        for uids_split in np.array_split(uids, num_partitions):
-            df_uids = df.query("unique_id in @uids_split")
+        df_lock = Lock()
+        X_df_lock = Lock()
+
+        def partition_by_uid_single(uids_split, func, df, X_df, id_col, **kwargs):
+            with df_lock:
+                df_uids = df.query("unique_id in @uids_split")
             if X_df is not None:
-                X_df_uids = X_df.query("unique_id in @uids_split")
+                with X_df_lock:
+                    X_df_uids = X_df.query("unique_id in @uids_split")
             else:
                 X_df_uids = None
             df_uids = remove_unused_categories(df_uids, col=id_col)
             X_df_uids = remove_unused_categories(X_df_uids, col=id_col)
             kwargs_uids = {"df": df_uids, **kwargs}
             if X_df_uids is not None:
                 kwargs_uids["X_df"] = X_df_uids
+
+            kwargs_uids["id_col"] = id_col
             results_uids = func(self, **kwargs_uids, num_partitions=1)
-            results_df.append(results_uids)
-        results_df = pd.concat(results_df).reset_index(drop=True)
+
+            return results_uids
+
+        fpartition_by_uid_single = partial(
+            partition_by_uid_single,
+            func=func,
+            df=df,
+            X_df=X_df,
+            id_col=id_col,
+            **kwargs
+        )
+
+        num_processes = min(num_partitions, cpu_count())
+        uids_splits = np.array_split(uids, num_processes)
+
+        with ThreadPoolExecutor(max_workers=num_processes) as executor:
+            results_uids = [
+                executor.submit(fpartition_by_uid_single, uids_split)
+                for uids_split in uids_splits
+            ]
+
+        results_df = pd.concat(
+            [result_df.result() for result_df in results_uids]
+        ).reset_index(drop=True)
+
         return results_df
 
     return wrapper
 
 # %% ../nbs/nixtla_client.ipynb 14
 class _NixtlaClient:
     """
@@ -1065,15 +1107,15 @@
             its `show_dash` method.
         """
         try:
             from utilsforecast.plotting import plot_series
         except ModuleNotFoundError:
             raise Exception(
                 "You have to install additional dependencies to use this method, "
-                'please install them using `pip install "nixtlats[plotting]"`'
+                'please install them using `pip install "nixtla[plotting]"`'
             )
         df = df.copy()
         if id_col not in df:
             df[id_col] = "ts_0"
         df[time_col] = pd.to_datetime(df[time_col])
         if forecasts_df is not None:
             forecasts_df = forecasts_df.copy()
```

### Comparing `nixtlats-0.3.0/nixtlats/types/__init__.py` & `nixtlats-0.4.0/nixtlats/types/__init__.py`

 * *Files identical despite different names*

### Comparing `nixtlats-0.3.0/nixtlats/types/http_validation_error.py` & `nixtlats-0.4.0/nixtlats/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `nixtlats-0.3.0/nixtlats/types/multi_series_anomaly.py` & `nixtlats-0.4.0/nixtlats/types/multi_series_anomaly.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from ..core.datetime_utils import serialize_datetime
 from .multi_series_anomaly_model import MultiSeriesAnomalyModel
 from .multi_series_input import MultiSeriesInput
 
 
 class MultiSeriesAnomaly(pydantic.BaseModel):
     model: typing.Optional[MultiSeriesAnomalyModel] = pydantic.Field(
-        description="Model to use as a string. Options are: `short-horizon`, and `long-horizon.` We recommend using `long-horizon` for forecasting if you want to predict more than one seasonal period given the frequency of your data."
+        description="Model to use as a string. Options are: `timegpt-1`, and `timegpt-1-long-horizon.` We recommend using `timegpt-1-long-horizon` for forecasting if you want to predict more than one seasonal period given the frequency of your data."
     )
     freq: typing.Optional[str] = pydantic.Field(
         description="The frequency of the data represented as a string. 'D' for daily, 'M' for monthly, 'H' for hourly, and 'W' for weekly frequencies are available."
     )
     level: typing.Optional[typing.List[typing.Any]] = pydantic.Field(
         description="Specifies the confidence level for the prediction interval used in anomaly detection. It is represented as a percentage between 0 and 100. For instance, a level of 95 indicates that the generated prediction interval captures the true future observation 95% of the time. Any observed values outside of this interval would be considered anomalies. A higher level leads to wider prediction intervals and potentially fewer detected anomalies, whereas a lower level results in narrower intervals and potentially more detected anomalies. Default: 99."
     )
```

### Comparing `nixtlats-0.3.0/nixtlats/types/multi_series_anomaly_model.py` & `nixtlats-0.4.0/nixtlats/types/multi_series_anomaly_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,30 +4,34 @@
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
 class MultiSeriesAnomalyModel(str, enum.Enum):
     """
-    Model to use as a string. Options are: `short-horizon`, and `long-horizon.` We recommend using `long-horizon` for forecasting if you want to predict more than one seasonal period given the frequency of your data.
+    Model to use as a string. Options are: `timegpt-1`, and `timegpt-1-long-horizon.` We recommend using `timegpt-1-long-horizon` for forecasting if you want to predict more than one seasonal period given the frequency of your data.
     """
 
-    SHORT_HORIZON = "short-horizon"
-    LONG_HORIZON = "long-horizon"
     TIMEGPT_1 = "timegpt-1"
     TIMEGPT_1_LONG_HORIZON = "timegpt-1-long-horizon"
+    SHORT_HORIZON = "short-horizon"
+    LONG_HORIZON = "long-horizon"
+    AZUREAI = "azureai"
 
     def visit(
         self,
-        short_horizon: typing.Callable[[], T_Result],
-        long_horizon: typing.Callable[[], T_Result],
         timegpt_1: typing.Callable[[], T_Result],
         timegpt_1_long_horizon: typing.Callable[[], T_Result],
+        short_horizon: typing.Callable[[], T_Result],
+        long_horizon: typing.Callable[[], T_Result],
+        azureai: typing.Callable[[], T_Result],
     ) -> T_Result:
-        if self is MultiSeriesAnomalyModel.SHORT_HORIZON:
-            return short_horizon()
-        if self is MultiSeriesAnomalyModel.LONG_HORIZON:
-            return long_horizon()
         if self is MultiSeriesAnomalyModel.TIMEGPT_1:
             return timegpt_1()
         if self is MultiSeriesAnomalyModel.TIMEGPT_1_LONG_HORIZON:
             return timegpt_1_long_horizon()
+        if self is MultiSeriesAnomalyModel.SHORT_HORIZON:
+            return short_horizon()
+        if self is MultiSeriesAnomalyModel.LONG_HORIZON:
+            return long_horizon()
+        if self is MultiSeriesAnomalyModel.AZUREAI:
+            return azureai()
```

### Comparing `nixtlats-0.3.0/nixtlats/types/multi_series_cross_validation.py` & `nixtlats-0.4.0/nixtlats/types/multi_series_cross_validation.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,16 +9,20 @@
 from .multi_series_cross_validation_fewshot_loss import MultiSeriesCrossValidationFewshotLoss
 from .multi_series_cross_validation_finetune_loss import MultiSeriesCrossValidationFinetuneLoss
 from .multi_series_cross_validation_model import MultiSeriesCrossValidationModel
 from .multi_series_input import MultiSeriesInput
 
 
 class MultiSeriesCrossValidation(pydantic.BaseModel):
+    fewshot_steps: typing.Optional[int] = pydantic.Field(description="Deprecated. Please use finetune_steps instead.")
+    fewshot_loss: typing.Optional[MultiSeriesCrossValidationFewshotLoss] = pydantic.Field(
+        description="Deprecated. Please use finetune_loss instead."
+    )
     model: typing.Optional[MultiSeriesCrossValidationModel] = pydantic.Field(
-        description="Model to use as a string. Options are: `short-horizon`, and `long-horizon.` We recommend using `long-horizon` for forecasting if you want to predict more than one seasonal period given the frequency of your data."
+        description="Model to use as a string. Options are: `timegpt-1`, and `timegpt-1-long-horizon.` We recommend using `timegpt-1-long-horizon` for forecasting if you want to predict more than one seasonal period given the frequency of your data."
     )
     freq: typing.Optional[str] = pydantic.Field(
         description="The frequency of the data represented as a string. 'D' for daily, 'M' for monthly, 'H' for hourly, and 'W' for weekly frequencies are available."
     )
     level: typing.Optional[typing.List[typing.Any]] = pydantic.Field(
         description="A list of values representing the prediction intervals. Each value is a percentage that indicates the level of certainty for the corresponding prediction interval. For example, [80, 90] defines 80% and 90% prediction intervals."
     )
@@ -32,23 +36,19 @@
     n_windows: typing.Optional[int] = pydantic.Field(description="Number of windows to evaluate.")
     step_size: typing.Optional[int] = pydantic.Field(
         description="Step size between each cross validation window. If None it will be equal to the forecasting horizon."
     )
     clean_ex_first: typing.Optional[bool] = pydantic.Field(
         description="A boolean flag that indicates whether the API should preprocess (clean) the exogenous signal before applying the large time model. If True, the exogenous signal is cleaned; if False, the exogenous variables are applied after the large time model."
     )
-    fewshot_steps: typing.Optional[int] = pydantic.Field(
+    finetune_steps: typing.Optional[int] = pydantic.Field(
         description="The number of tuning steps used to train the large time model on the data. Set this value to 0 for zero-shot inference, i.e., to make predictions without any further model tuning."
     )
-    fewshot_loss: typing.Optional[MultiSeriesCrossValidationFewshotLoss] = pydantic.Field(
-        description="The loss used to train the large time model on the data. Select from ['default', 'mae', 'mse', 'rmse', 'mape', 'smape']. It will only be used if finetune_steps larger than 0. Default is a robust loss function that is less sensitive to outliers."
-    )
-    finetune_steps: typing.Optional[int] = pydantic.Field(description="Deprecated. Please use fewshot_steps instead.")
     finetune_loss: typing.Optional[MultiSeriesCrossValidationFinetuneLoss] = pydantic.Field(
-        description="Deprecated. Please use fewshot_loss instead."
+        description="The loss used to train the large time model on the data. Select from ['default', 'mae', 'mse', 'rmse', 'mape', 'smape']. It will only be used if finetune_steps larger than 0. Default is a robust loss function that is less sensitive to outliers."
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `nixtlats-0.3.0/nixtlats/types/multi_series_cross_validation_fewshot_loss.py` & `nixtlats-0.4.0/nixtlats/types/multi_series_cross_validation_finetune_loss.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
-class MultiSeriesCrossValidationFewshotLoss(str, enum.Enum):
+class MultiSeriesCrossValidationFinetuneLoss(str, enum.Enum):
     """
     The loss used to train the large time model on the data. Select from ['default', 'mae', 'mse', 'rmse', 'mape', 'smape']. It will only be used if finetune_steps larger than 0. Default is a robust loss function that is less sensitive to outliers.
     """
 
     DEFAULT = "default"
     MAE = "mae"
     MSE = "mse"
@@ -23,19 +23,19 @@
         default: typing.Callable[[], T_Result],
         mae: typing.Callable[[], T_Result],
         mse: typing.Callable[[], T_Result],
         rmse: typing.Callable[[], T_Result],
         mape: typing.Callable[[], T_Result],
         smape: typing.Callable[[], T_Result],
     ) -> T_Result:
-        if self is MultiSeriesCrossValidationFewshotLoss.DEFAULT:
+        if self is MultiSeriesCrossValidationFinetuneLoss.DEFAULT:
             return default()
-        if self is MultiSeriesCrossValidationFewshotLoss.MAE:
+        if self is MultiSeriesCrossValidationFinetuneLoss.MAE:
             return mae()
-        if self is MultiSeriesCrossValidationFewshotLoss.MSE:
+        if self is MultiSeriesCrossValidationFinetuneLoss.MSE:
             return mse()
-        if self is MultiSeriesCrossValidationFewshotLoss.RMSE:
+        if self is MultiSeriesCrossValidationFinetuneLoss.RMSE:
             return rmse()
-        if self is MultiSeriesCrossValidationFewshotLoss.MAPE:
+        if self is MultiSeriesCrossValidationFinetuneLoss.MAPE:
             return mape()
-        if self is MultiSeriesCrossValidationFewshotLoss.SMAPE:
+        if self is MultiSeriesCrossValidationFinetuneLoss.SMAPE:
             return smape()
```

### Comparing `nixtlats-0.3.0/nixtlats/types/multi_series_cross_validation_finetune_loss.py` & `nixtlats-0.4.0/nixtlats/types/multi_series_cross_validation_fewshot_loss.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
-class MultiSeriesCrossValidationFinetuneLoss(str, enum.Enum):
+class MultiSeriesCrossValidationFewshotLoss(str, enum.Enum):
     """
-    Deprecated. Please use fewshot_loss instead.
+    Deprecated. Please use finetune_loss instead.
     """
 
     DEFAULT = "default"
     MAE = "mae"
     MSE = "mse"
     RMSE = "rmse"
     MAPE = "mape"
@@ -23,19 +23,19 @@
         default: typing.Callable[[], T_Result],
         mae: typing.Callable[[], T_Result],
         mse: typing.Callable[[], T_Result],
         rmse: typing.Callable[[], T_Result],
         mape: typing.Callable[[], T_Result],
         smape: typing.Callable[[], T_Result],
     ) -> T_Result:
-        if self is MultiSeriesCrossValidationFinetuneLoss.DEFAULT:
+        if self is MultiSeriesCrossValidationFewshotLoss.DEFAULT:
             return default()
-        if self is MultiSeriesCrossValidationFinetuneLoss.MAE:
+        if self is MultiSeriesCrossValidationFewshotLoss.MAE:
             return mae()
-        if self is MultiSeriesCrossValidationFinetuneLoss.MSE:
+        if self is MultiSeriesCrossValidationFewshotLoss.MSE:
             return mse()
-        if self is MultiSeriesCrossValidationFinetuneLoss.RMSE:
+        if self is MultiSeriesCrossValidationFewshotLoss.RMSE:
             return rmse()
-        if self is MultiSeriesCrossValidationFinetuneLoss.MAPE:
+        if self is MultiSeriesCrossValidationFewshotLoss.MAPE:
             return mape()
-        if self is MultiSeriesCrossValidationFinetuneLoss.SMAPE:
+        if self is MultiSeriesCrossValidationFewshotLoss.SMAPE:
             return smape()
```

### Comparing `nixtlats-0.3.0/nixtlats/types/multi_series_cross_validation_model.py` & `nixtlats-0.4.0/nixtlats/types/multi_series_forecast_model.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,32 +2,36 @@
 
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
-class MultiSeriesCrossValidationModel(str, enum.Enum):
+class MultiSeriesForecastModel(str, enum.Enum):
     """
-    Model to use as a string. Options are: `short-horizon`, and `long-horizon.` We recommend using `long-horizon` for forecasting if you want to predict more than one seasonal period given the frequency of your data.
+    Model to use as a string. Options are: `timegpt-1`, and `timegpt-1-long-horizon.` We recommend using `timegpt-1-long-horizon` for forecasting if you want to predict more than one seasonal period given the frequency of your data.
     """
 
-    SHORT_HORIZON = "short-horizon"
-    LONG_HORIZON = "long-horizon"
     TIMEGPT_1 = "timegpt-1"
     TIMEGPT_1_LONG_HORIZON = "timegpt-1-long-horizon"
+    SHORT_HORIZON = "short-horizon"
+    LONG_HORIZON = "long-horizon"
+    AZUREAI = "azureai"
 
     def visit(
         self,
-        short_horizon: typing.Callable[[], T_Result],
-        long_horizon: typing.Callable[[], T_Result],
         timegpt_1: typing.Callable[[], T_Result],
         timegpt_1_long_horizon: typing.Callable[[], T_Result],
+        short_horizon: typing.Callable[[], T_Result],
+        long_horizon: typing.Callable[[], T_Result],
+        azureai: typing.Callable[[], T_Result],
     ) -> T_Result:
-        if self is MultiSeriesCrossValidationModel.SHORT_HORIZON:
-            return short_horizon()
-        if self is MultiSeriesCrossValidationModel.LONG_HORIZON:
-            return long_horizon()
-        if self is MultiSeriesCrossValidationModel.TIMEGPT_1:
+        if self is MultiSeriesForecastModel.TIMEGPT_1:
             return timegpt_1()
-        if self is MultiSeriesCrossValidationModel.TIMEGPT_1_LONG_HORIZON:
+        if self is MultiSeriesForecastModel.TIMEGPT_1_LONG_HORIZON:
             return timegpt_1_long_horizon()
+        if self is MultiSeriesForecastModel.SHORT_HORIZON:
+            return short_horizon()
+        if self is MultiSeriesForecastModel.LONG_HORIZON:
+            return long_horizon()
+        if self is MultiSeriesForecastModel.AZUREAI:
+            return azureai()
```

### Comparing `nixtlats-0.3.0/nixtlats/types/multi_series_forecast.py` & `nixtlats-0.4.0/nixtlats/types/multi_series_forecast.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,16 +9,20 @@
 from .multi_series_forecast_fewshot_loss import MultiSeriesForecastFewshotLoss
 from .multi_series_forecast_finetune_loss import MultiSeriesForecastFinetuneLoss
 from .multi_series_forecast_model import MultiSeriesForecastModel
 from .multi_series_input import MultiSeriesInput
 
 
 class MultiSeriesForecast(pydantic.BaseModel):
+    fewshot_steps: typing.Optional[int] = pydantic.Field(description="Deprecated. Please use finetune_steps instead.")
+    fewshot_loss: typing.Optional[MultiSeriesForecastFewshotLoss] = pydantic.Field(
+        description="Deprecated. Please use finetune_loss instead."
+    )
     model: typing.Optional[MultiSeriesForecastModel] = pydantic.Field(
-        description="Model to use as a string. Options are: `short-horizon`, and `long-horizon.` We recommend using `long-horizon` for forecasting if you want to predict more than one seasonal period given the frequency of your data."
+        description="Model to use as a string. Options are: `timegpt-1`, and `timegpt-1-long-horizon.` We recommend using `timegpt-1-long-horizon` for forecasting if you want to predict more than one seasonal period given the frequency of your data."
     )
     freq: typing.Optional[str] = pydantic.Field(
         description="The frequency of the data represented as a string. 'D' for daily, 'M' for monthly, 'H' for hourly, and 'W' for weekly frequencies are available."
     )
     level: typing.Optional[typing.List[typing.Any]] = pydantic.Field(
         description="A list of values representing the prediction intervals. Each value is a percentage that indicates the level of certainty for the corresponding prediction interval. For example, [80, 90] defines 80% and 90% prediction intervals."
     )
@@ -28,23 +32,19 @@
     y: typing.Optional[typing.Any]
     x: typing.Optional[MultiSeriesInput] = pydantic.Field(
         description='The exogenous  variables provided as a dictionary of two colums: columns and data. The columns contains the columns of the dataframe and data contains eaach data point. For example: {"columns": ["unique_id", "ds", "ex_1", "ex_2"], "data": [["ts_0", "2021-01-01", 0.2, 0.67], ["ts_0", "2021-01-02", 0.4, 0.7]}. This should also include forecasting horizon (fh) additional timestamps for each unique_id to calculate the future values.'
     )
     clean_ex_first: typing.Optional[bool] = pydantic.Field(
         description="A boolean flag that indicates whether the API should preprocess (clean) the exogenous signal before applying the large time model. If True, the exogenous signal is cleaned; if False, the exogenous variables are applied after the large time model."
     )
-    fewshot_steps: typing.Optional[int] = pydantic.Field(
+    finetune_steps: typing.Optional[int] = pydantic.Field(
         description="The number of tuning steps used to train the large time model on the data. Set this value to 0 for zero-shot inference, i.e., to make predictions without any further model tuning."
     )
-    fewshot_loss: typing.Optional[MultiSeriesForecastFewshotLoss] = pydantic.Field(
-        description="The loss used to train the large time model on the data. Select from ['default', 'mae', 'mse', 'rmse', 'mape', 'smape']. It will only be used if finetune_steps larger than 0. Default is a robust loss function that is less sensitive to outliers."
-    )
-    finetune_steps: typing.Optional[int] = pydantic.Field(description="Deprecated. Please use fewshot_steps instead.")
     finetune_loss: typing.Optional[MultiSeriesForecastFinetuneLoss] = pydantic.Field(
-        description="Deprecated. Please use fewshot_loss instead."
+        description="The loss used to train the large time model on the data. Select from ['default', 'mae', 'mse', 'rmse', 'mape', 'smape']. It will only be used if finetune_steps larger than 0. Default is a robust loss function that is less sensitive to outliers."
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `nixtlats-0.3.0/nixtlats/types/multi_series_forecast_fewshot_loss.py` & `nixtlats-0.4.0/nixtlats/types/multi_series_forecast_finetune_loss.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
-class MultiSeriesForecastFewshotLoss(str, enum.Enum):
+class MultiSeriesForecastFinetuneLoss(str, enum.Enum):
     """
     The loss used to train the large time model on the data. Select from ['default', 'mae', 'mse', 'rmse', 'mape', 'smape']. It will only be used if finetune_steps larger than 0. Default is a robust loss function that is less sensitive to outliers.
     """
 
     DEFAULT = "default"
     MAE = "mae"
     MSE = "mse"
@@ -23,19 +23,19 @@
         default: typing.Callable[[], T_Result],
         mae: typing.Callable[[], T_Result],
         mse: typing.Callable[[], T_Result],
         rmse: typing.Callable[[], T_Result],
         mape: typing.Callable[[], T_Result],
         smape: typing.Callable[[], T_Result],
     ) -> T_Result:
-        if self is MultiSeriesForecastFewshotLoss.DEFAULT:
+        if self is MultiSeriesForecastFinetuneLoss.DEFAULT:
             return default()
-        if self is MultiSeriesForecastFewshotLoss.MAE:
+        if self is MultiSeriesForecastFinetuneLoss.MAE:
             return mae()
-        if self is MultiSeriesForecastFewshotLoss.MSE:
+        if self is MultiSeriesForecastFinetuneLoss.MSE:
             return mse()
-        if self is MultiSeriesForecastFewshotLoss.RMSE:
+        if self is MultiSeriesForecastFinetuneLoss.RMSE:
             return rmse()
-        if self is MultiSeriesForecastFewshotLoss.MAPE:
+        if self is MultiSeriesForecastFinetuneLoss.MAPE:
             return mape()
-        if self is MultiSeriesForecastFewshotLoss.SMAPE:
+        if self is MultiSeriesForecastFinetuneLoss.SMAPE:
             return smape()
```

### Comparing `nixtlats-0.3.0/nixtlats/types/multi_series_forecast_finetune_loss.py` & `nixtlats-0.4.0/nixtlats/types/multi_series_forecast_fewshot_loss.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
-class MultiSeriesForecastFinetuneLoss(str, enum.Enum):
+class MultiSeriesForecastFewshotLoss(str, enum.Enum):
     """
-    Deprecated. Please use fewshot_loss instead.
+    Deprecated. Please use finetune_loss instead.
     """
 
     DEFAULT = "default"
     MAE = "mae"
     MSE = "mse"
     RMSE = "rmse"
     MAPE = "mape"
@@ -23,19 +23,19 @@
         default: typing.Callable[[], T_Result],
         mae: typing.Callable[[], T_Result],
         mse: typing.Callable[[], T_Result],
         rmse: typing.Callable[[], T_Result],
         mape: typing.Callable[[], T_Result],
         smape: typing.Callable[[], T_Result],
     ) -> T_Result:
-        if self is MultiSeriesForecastFinetuneLoss.DEFAULT:
+        if self is MultiSeriesForecastFewshotLoss.DEFAULT:
             return default()
-        if self is MultiSeriesForecastFinetuneLoss.MAE:
+        if self is MultiSeriesForecastFewshotLoss.MAE:
             return mae()
-        if self is MultiSeriesForecastFinetuneLoss.MSE:
+        if self is MultiSeriesForecastFewshotLoss.MSE:
             return mse()
-        if self is MultiSeriesForecastFinetuneLoss.RMSE:
+        if self is MultiSeriesForecastFewshotLoss.RMSE:
             return rmse()
-        if self is MultiSeriesForecastFinetuneLoss.MAPE:
+        if self is MultiSeriesForecastFewshotLoss.MAPE:
             return mape()
-        if self is MultiSeriesForecastFinetuneLoss.SMAPE:
+        if self is MultiSeriesForecastFewshotLoss.SMAPE:
             return smape()
```

### Comparing `nixtlats-0.3.0/nixtlats/types/multi_series_forecast_model.py` & `nixtlats-0.4.0/nixtlats/types/multi_series_insample_forecast_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,32 +2,36 @@
 
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
-class MultiSeriesForecastModel(str, enum.Enum):
+class MultiSeriesInsampleForecastModel(str, enum.Enum):
     """
-    Model to use as a string. Options are: `short-horizon`, and `long-horizon.` We recommend using `long-horizon` for forecasting if you want to predict more than one seasonal period given the frequency of your data.
+    Model to use as a string. Options are: `timegpt-1`, and `timegpt-1-long-horizon.` We recommend using `timegpt-1-long-horizon` for forecasting if you want to predict more than one seasonal period given the frequency of your data.
     """
 
-    SHORT_HORIZON = "short-horizon"
-    LONG_HORIZON = "long-horizon"
     TIMEGPT_1 = "timegpt-1"
     TIMEGPT_1_LONG_HORIZON = "timegpt-1-long-horizon"
+    SHORT_HORIZON = "short-horizon"
+    LONG_HORIZON = "long-horizon"
+    AZUREAI = "azureai"
 
     def visit(
         self,
-        short_horizon: typing.Callable[[], T_Result],
-        long_horizon: typing.Callable[[], T_Result],
         timegpt_1: typing.Callable[[], T_Result],
         timegpt_1_long_horizon: typing.Callable[[], T_Result],
+        short_horizon: typing.Callable[[], T_Result],
+        long_horizon: typing.Callable[[], T_Result],
+        azureai: typing.Callable[[], T_Result],
     ) -> T_Result:
-        if self is MultiSeriesForecastModel.SHORT_HORIZON:
-            return short_horizon()
-        if self is MultiSeriesForecastModel.LONG_HORIZON:
-            return long_horizon()
-        if self is MultiSeriesForecastModel.TIMEGPT_1:
+        if self is MultiSeriesInsampleForecastModel.TIMEGPT_1:
             return timegpt_1()
-        if self is MultiSeriesForecastModel.TIMEGPT_1_LONG_HORIZON:
+        if self is MultiSeriesInsampleForecastModel.TIMEGPT_1_LONG_HORIZON:
             return timegpt_1_long_horizon()
+        if self is MultiSeriesInsampleForecastModel.SHORT_HORIZON:
+            return short_horizon()
+        if self is MultiSeriesInsampleForecastModel.LONG_HORIZON:
+            return long_horizon()
+        if self is MultiSeriesInsampleForecastModel.AZUREAI:
+            return azureai()
```

### Comparing `nixtlats-0.3.0/nixtlats/types/multi_series_input.py` & `nixtlats-0.4.0/nixtlats/types/multi_series_input.py`

 * *Files identical despite different names*

### Comparing `nixtlats-0.3.0/nixtlats/types/multi_series_insample_forecast.py` & `nixtlats-0.4.0/nixtlats/types/multi_series_insample_forecast.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from ..core.datetime_utils import serialize_datetime
 from .multi_series_input import MultiSeriesInput
 from .multi_series_insample_forecast_model import MultiSeriesInsampleForecastModel
 
 
 class MultiSeriesInsampleForecast(pydantic.BaseModel):
     model: typing.Optional[MultiSeriesInsampleForecastModel] = pydantic.Field(
-        description="Model to use as a string. Options are: `short-horizon`, and `long-horizon.` We recommend using `long-horizon` for forecasting if you want to predict more than one seasonal period given the frequency of your data."
+        description="Model to use as a string. Options are: `timegpt-1`, and `timegpt-1-long-horizon.` We recommend using `timegpt-1-long-horizon` for forecasting if you want to predict more than one seasonal period given the frequency of your data."
     )
     freq: typing.Optional[str] = pydantic.Field(
         description="The frequency of the data represented as a string. 'D' for daily, 'M' for monthly, 'H' for hourly, and 'W' for weekly frequencies are available."
     )
     level: typing.Optional[typing.List[typing.Any]] = pydantic.Field(
         description="A list of values representing the prediction intervals. Each value is a percentage that indicates the level of certainty for the corresponding prediction interval. For example, [80, 90] defines 80% and 90% prediction intervals."
     )
```

### Comparing `nixtlats-0.3.0/nixtlats/types/multi_series_insample_forecast_model.py` & `nixtlats-0.4.0/nixtlats/types/multi_series_cross_validation_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,32 +2,36 @@
 
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
-class MultiSeriesInsampleForecastModel(str, enum.Enum):
+class MultiSeriesCrossValidationModel(str, enum.Enum):
     """
-    Model to use as a string. Options are: `short-horizon`, and `long-horizon.` We recommend using `long-horizon` for forecasting if you want to predict more than one seasonal period given the frequency of your data.
+    Model to use as a string. Options are: `timegpt-1`, and `timegpt-1-long-horizon.` We recommend using `timegpt-1-long-horizon` for forecasting if you want to predict more than one seasonal period given the frequency of your data.
     """
 
-    SHORT_HORIZON = "short-horizon"
-    LONG_HORIZON = "long-horizon"
     TIMEGPT_1 = "timegpt-1"
     TIMEGPT_1_LONG_HORIZON = "timegpt-1-long-horizon"
+    SHORT_HORIZON = "short-horizon"
+    LONG_HORIZON = "long-horizon"
+    AZUREAI = "azureai"
 
     def visit(
         self,
-        short_horizon: typing.Callable[[], T_Result],
-        long_horizon: typing.Callable[[], T_Result],
         timegpt_1: typing.Callable[[], T_Result],
         timegpt_1_long_horizon: typing.Callable[[], T_Result],
+        short_horizon: typing.Callable[[], T_Result],
+        long_horizon: typing.Callable[[], T_Result],
+        azureai: typing.Callable[[], T_Result],
     ) -> T_Result:
-        if self is MultiSeriesInsampleForecastModel.SHORT_HORIZON:
-            return short_horizon()
-        if self is MultiSeriesInsampleForecastModel.LONG_HORIZON:
-            return long_horizon()
-        if self is MultiSeriesInsampleForecastModel.TIMEGPT_1:
+        if self is MultiSeriesCrossValidationModel.TIMEGPT_1:
             return timegpt_1()
-        if self is MultiSeriesInsampleForecastModel.TIMEGPT_1_LONG_HORIZON:
+        if self is MultiSeriesCrossValidationModel.TIMEGPT_1_LONG_HORIZON:
             return timegpt_1_long_horizon()
+        if self is MultiSeriesCrossValidationModel.SHORT_HORIZON:
+            return short_horizon()
+        if self is MultiSeriesCrossValidationModel.LONG_HORIZON:
+            return long_horizon()
+        if self is MultiSeriesCrossValidationModel.AZUREAI:
+            return azureai()
```

### Comparing `nixtlats-0.3.0/nixtlats/types/single_series_forecast.py` & `nixtlats-0.4.0/nixtlats/types/single_series_forecast.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,16 +8,20 @@
 from ..core.datetime_utils import serialize_datetime
 from .single_series_forecast_fewshot_loss import SingleSeriesForecastFewshotLoss
 from .single_series_forecast_finetune_loss import SingleSeriesForecastFinetuneLoss
 from .single_series_forecast_model import SingleSeriesForecastModel
 
 
 class SingleSeriesForecast(pydantic.BaseModel):
+    fewshot_steps: typing.Optional[int] = pydantic.Field(description="Deprecated. Please use finetune_steps instead.")
+    fewshot_loss: typing.Optional[SingleSeriesForecastFewshotLoss] = pydantic.Field(
+        description="Deprecated. Please use finetune_loss instead."
+    )
     model: typing.Optional[SingleSeriesForecastModel] = pydantic.Field(
-        description="Model to use as a string. Options are: `short-horizon`, and `long-horizon.` We recommend using `long-horizon` for forecasting if you want to predict more than one seasonal period given the frequency of your data."
+        description="Model to use as a string. Options are: `timegpt-1`, and `timegpt-1-long-horizon.` We recommend using `timegpt-1-long-horizon` for forecasting if you want to predict more than one seasonal period given the frequency of your data."
     )
     freq: typing.Optional[str] = pydantic.Field(
         description="The frequency of the data represented as a string. 'D' for daily, 'M' for monthly, 'H' for hourly, and 'W' for weekly frequencies are available."
     )
     level: typing.Optional[typing.List[typing.Any]] = pydantic.Field(
         description="A list of values representing the prediction intervals. Each value is a percentage that indicates the level of certainty for the corresponding prediction interval. For example, [80, 90] defines 80% and 90% prediction intervals."
     )
@@ -27,23 +31,19 @@
     y: typing.Optional[typing.Any]
     x: typing.Optional[typing.Dict[str, typing.List[float]]] = pydantic.Field(
         description='The exogenous variables provided as a dictionary. Each key is a timestamp (string format: YYYY-MM-DD) and the corresponding value is a list of exogenous variable values at that time point. For example: {"2021-01-01": [0.1], "2021-01-02": [0.4]}. This should also include forecasting horizon (fh) additional timestamps to calculate the future values.'
     )
     clean_ex_first: typing.Optional[bool] = pydantic.Field(
         description="A boolean flag that indicates whether the API should preprocess (clean) the exogenous signal before applying the large time model. If True, the exogenous signal is cleaned; if False, the exogenous variables are applied after the large time model."
     )
-    fewshot_steps: typing.Optional[int] = pydantic.Field(
+    finetune_steps: typing.Optional[int] = pydantic.Field(
         description="The number of tuning steps used to train the large time model on the data. Set this value to 0 for zero-shot inference, i.e., to make predictions without any further model tuning."
     )
-    fewshot_loss: typing.Optional[SingleSeriesForecastFewshotLoss] = pydantic.Field(
-        description="The loss used to train the large time model on the data. Select from ['default', 'mae', 'mse', 'rmse', 'mape', 'smape']. It will only be used if finetune_steps larger than 0. Default is a robust loss function that is less sensitive to outliers."
-    )
-    finetune_steps: typing.Optional[int] = pydantic.Field(description="Deprecated. Please use fewshot_steps instead.")
     finetune_loss: typing.Optional[SingleSeriesForecastFinetuneLoss] = pydantic.Field(
-        description="Deprecated. Please use fewshot_loss instead."
+        description="The loss used to train the large time model on the data. Select from ['default', 'mae', 'mse', 'rmse', 'mape', 'smape']. It will only be used if finetune_steps larger than 0. Default is a robust loss function that is less sensitive to outliers."
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `nixtlats-0.3.0/nixtlats/types/single_series_forecast_fewshot_loss.py` & `nixtlats-0.4.0/nixtlats/types/single_series_forecast_finetune_loss.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
-class SingleSeriesForecastFewshotLoss(str, enum.Enum):
+class SingleSeriesForecastFinetuneLoss(str, enum.Enum):
     """
     The loss used to train the large time model on the data. Select from ['default', 'mae', 'mse', 'rmse', 'mape', 'smape']. It will only be used if finetune_steps larger than 0. Default is a robust loss function that is less sensitive to outliers.
     """
 
     DEFAULT = "default"
     MAE = "mae"
     MSE = "mse"
@@ -23,19 +23,19 @@
         default: typing.Callable[[], T_Result],
         mae: typing.Callable[[], T_Result],
         mse: typing.Callable[[], T_Result],
         rmse: typing.Callable[[], T_Result],
         mape: typing.Callable[[], T_Result],
         smape: typing.Callable[[], T_Result],
     ) -> T_Result:
-        if self is SingleSeriesForecastFewshotLoss.DEFAULT:
+        if self is SingleSeriesForecastFinetuneLoss.DEFAULT:
             return default()
-        if self is SingleSeriesForecastFewshotLoss.MAE:
+        if self is SingleSeriesForecastFinetuneLoss.MAE:
             return mae()
-        if self is SingleSeriesForecastFewshotLoss.MSE:
+        if self is SingleSeriesForecastFinetuneLoss.MSE:
             return mse()
-        if self is SingleSeriesForecastFewshotLoss.RMSE:
+        if self is SingleSeriesForecastFinetuneLoss.RMSE:
             return rmse()
-        if self is SingleSeriesForecastFewshotLoss.MAPE:
+        if self is SingleSeriesForecastFinetuneLoss.MAPE:
             return mape()
-        if self is SingleSeriesForecastFewshotLoss.SMAPE:
+        if self is SingleSeriesForecastFinetuneLoss.SMAPE:
             return smape()
```

### Comparing `nixtlats-0.3.0/nixtlats/types/single_series_forecast_finetune_loss.py` & `nixtlats-0.4.0/nixtlats/types/single_series_forecast_fewshot_loss.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
-class SingleSeriesForecastFinetuneLoss(str, enum.Enum):
+class SingleSeriesForecastFewshotLoss(str, enum.Enum):
     """
-    Deprecated. Please use fewshot_loss instead.
+    Deprecated. Please use finetune_loss instead.
     """
 
     DEFAULT = "default"
     MAE = "mae"
     MSE = "mse"
     RMSE = "rmse"
     MAPE = "mape"
@@ -23,19 +23,19 @@
         default: typing.Callable[[], T_Result],
         mae: typing.Callable[[], T_Result],
         mse: typing.Callable[[], T_Result],
         rmse: typing.Callable[[], T_Result],
         mape: typing.Callable[[], T_Result],
         smape: typing.Callable[[], T_Result],
     ) -> T_Result:
-        if self is SingleSeriesForecastFinetuneLoss.DEFAULT:
+        if self is SingleSeriesForecastFewshotLoss.DEFAULT:
             return default()
-        if self is SingleSeriesForecastFinetuneLoss.MAE:
+        if self is SingleSeriesForecastFewshotLoss.MAE:
             return mae()
-        if self is SingleSeriesForecastFinetuneLoss.MSE:
+        if self is SingleSeriesForecastFewshotLoss.MSE:
             return mse()
-        if self is SingleSeriesForecastFinetuneLoss.RMSE:
+        if self is SingleSeriesForecastFewshotLoss.RMSE:
             return rmse()
-        if self is SingleSeriesForecastFinetuneLoss.MAPE:
+        if self is SingleSeriesForecastFewshotLoss.MAPE:
             return mape()
-        if self is SingleSeriesForecastFinetuneLoss.SMAPE:
+        if self is SingleSeriesForecastFewshotLoss.SMAPE:
             return smape()
```

### Comparing `nixtlats-0.3.0/nixtlats/types/single_series_forecast_model.py` & `nixtlats-0.4.0/nixtlats/types/single_series_forecast_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,30 +4,34 @@
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
 class SingleSeriesForecastModel(str, enum.Enum):
     """
-    Model to use as a string. Options are: `short-horizon`, and `long-horizon.` We recommend using `long-horizon` for forecasting if you want to predict more than one seasonal period given the frequency of your data.
+    Model to use as a string. Options are: `timegpt-1`, and `timegpt-1-long-horizon.` We recommend using `timegpt-1-long-horizon` for forecasting if you want to predict more than one seasonal period given the frequency of your data.
     """
 
-    SHORT_HORIZON = "short-horizon"
-    LONG_HORIZON = "long-horizon"
     TIMEGPT_1 = "timegpt-1"
     TIMEGPT_1_LONG_HORIZON = "timegpt-1-long-horizon"
+    SHORT_HORIZON = "short-horizon"
+    LONG_HORIZON = "long-horizon"
+    AZUREAI = "azureai"
 
     def visit(
         self,
-        short_horizon: typing.Callable[[], T_Result],
-        long_horizon: typing.Callable[[], T_Result],
         timegpt_1: typing.Callable[[], T_Result],
         timegpt_1_long_horizon: typing.Callable[[], T_Result],
+        short_horizon: typing.Callable[[], T_Result],
+        long_horizon: typing.Callable[[], T_Result],
+        azureai: typing.Callable[[], T_Result],
     ) -> T_Result:
-        if self is SingleSeriesForecastModel.SHORT_HORIZON:
-            return short_horizon()
-        if self is SingleSeriesForecastModel.LONG_HORIZON:
-            return long_horizon()
         if self is SingleSeriesForecastModel.TIMEGPT_1:
             return timegpt_1()
         if self is SingleSeriesForecastModel.TIMEGPT_1_LONG_HORIZON:
             return timegpt_1_long_horizon()
+        if self is SingleSeriesForecastModel.SHORT_HORIZON:
+            return short_horizon()
+        if self is SingleSeriesForecastModel.LONG_HORIZON:
+            return long_horizon()
+        if self is SingleSeriesForecastModel.AZUREAI:
+            return azureai()
```

### Comparing `nixtlats-0.3.0/nixtlats/types/single_series_insample_forecast.py` & `nixtlats-0.4.0/nixtlats/types/single_series_insample_forecast.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from ..core.datetime_utils import serialize_datetime
 from .single_series_insample_forecast_model import SingleSeriesInsampleForecastModel
 
 
 class SingleSeriesInsampleForecast(pydantic.BaseModel):
     model: typing.Optional[SingleSeriesInsampleForecastModel] = pydantic.Field(
-        description="Model to use as a string. Options are: `short-horizon`, and `long-horizon.` We recommend using `long-horizon` for forecasting if you want to predict more than one seasonal period given the frequency of your data."
+        description="Model to use as a string. Options are: `timegpt-1`, and `timegpt-1-long-horizon.` We recommend using `timegpt-1-long-horizon` for forecasting if you want to predict more than one seasonal period given the frequency of your data."
     )
     freq: typing.Optional[str] = pydantic.Field(
         description="The frequency of the data represented as a string. 'D' for daily, 'M' for monthly, 'H' for hourly, and 'W' for weekly frequencies are available."
     )
     level: typing.Optional[typing.List[typing.Any]] = pydantic.Field(
         description="A list of values representing the prediction intervals. Each value is a percentage that indicates the level of certainty for the corresponding prediction interval. For example, [80, 90] defines 80% and 90% prediction intervals."
     )
```

### Comparing `nixtlats-0.3.0/nixtlats/types/single_series_insample_forecast_model.py` & `nixtlats-0.4.0/nixtlats/types/single_series_insample_forecast_model.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,30 +4,34 @@
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
 class SingleSeriesInsampleForecastModel(str, enum.Enum):
     """
-    Model to use as a string. Options are: `short-horizon`, and `long-horizon.` We recommend using `long-horizon` for forecasting if you want to predict more than one seasonal period given the frequency of your data.
+    Model to use as a string. Options are: `timegpt-1`, and `timegpt-1-long-horizon.` We recommend using `timegpt-1-long-horizon` for forecasting if you want to predict more than one seasonal period given the frequency of your data.
     """
 
-    SHORT_HORIZON = "short-horizon"
-    LONG_HORIZON = "long-horizon"
     TIMEGPT_1 = "timegpt-1"
     TIMEGPT_1_LONG_HORIZON = "timegpt-1-long-horizon"
+    SHORT_HORIZON = "short-horizon"
+    LONG_HORIZON = "long-horizon"
+    AZUREAI = "azureai"
 
     def visit(
         self,
-        short_horizon: typing.Callable[[], T_Result],
-        long_horizon: typing.Callable[[], T_Result],
         timegpt_1: typing.Callable[[], T_Result],
         timegpt_1_long_horizon: typing.Callable[[], T_Result],
+        short_horizon: typing.Callable[[], T_Result],
+        long_horizon: typing.Callable[[], T_Result],
+        azureai: typing.Callable[[], T_Result],
     ) -> T_Result:
-        if self is SingleSeriesInsampleForecastModel.SHORT_HORIZON:
-            return short_horizon()
-        if self is SingleSeriesInsampleForecastModel.LONG_HORIZON:
-            return long_horizon()
         if self is SingleSeriesInsampleForecastModel.TIMEGPT_1:
             return timegpt_1()
         if self is SingleSeriesInsampleForecastModel.TIMEGPT_1_LONG_HORIZON:
             return timegpt_1_long_horizon()
+        if self is SingleSeriesInsampleForecastModel.SHORT_HORIZON:
+            return short_horizon()
+        if self is SingleSeriesInsampleForecastModel.LONG_HORIZON:
+            return long_horizon()
+        if self is SingleSeriesInsampleForecastModel.AZUREAI:
+            return azureai()
```

### Comparing `nixtlats-0.3.0/nixtlats/types/validation_error.py` & `nixtlats-0.4.0/nixtlats/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `nixtlats-0.3.0/nixtlats.egg-info/PKG-INFO` & `nixtlats-0.4.0/nixtlats.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,95 +1,95 @@
 Metadata-Version: 2.1
 Name: nixtlats
-Version: 0.3.0
+Version: 0.4.0
 Summary: Python SDK for Nixtla API (TimeGPT)
 Home-page: https://github.com/Nixtla/nixtla
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx
 Requires-Dist: pandas
 Requires-Dist: pydantic<2
 Requires-Dist: requests
 Requires-Dist: tenacity
-Requires-Dist: utilsforecast>=0.0.13
+Requires-Dist: utilsforecast>=0.1.7
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: datasetsforecast; extra == "dev"
 Requires-Dist: nbdev; extra == "dev"
 Requires-Dist: plotly; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: python-dotenv; extra == "dev"
 Requires-Dist: statsforecast; extra == "dev"
 Requires-Dist: dask[dataframe]; extra == "dev"
 Requires-Dist: fugue[ray]>=0.8.7; extra == "dev"
 Requires-Dist: pyspark; extra == "dev"
 Requires-Dist: ray[serve-grpc]; extra == "dev"
-Requires-Dist: utilsforecast[plotting]>=0.0.5; extra == "dev"
+Requires-Dist: utilsforecast[plotting]>=0.1.7; extra == "dev"
 Requires-Dist: holidays; extra == "dev"
 Provides-Extra: distributed
 Requires-Dist: dask[dataframe]; extra == "distributed"
 Requires-Dist: fugue[ray]>=0.8.7; extra == "distributed"
 Requires-Dist: pyspark; extra == "distributed"
 Requires-Dist: ray[serve-grpc]; extra == "distributed"
 Provides-Extra: plotting
-Requires-Dist: utilsforecast[plotting]>=0.0.5; extra == "plotting"
+Requires-Dist: utilsforecast[plotting]>=0.1.7; extra == "plotting"
 Provides-Extra: date-extras
 Requires-Dist: holidays; extra == "date-extras"
 
 # Nixtla &nbsp; [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Statistical%20Forecasting%20Algorithms%20by%20Nixtla%20&url=https://github.com/Nixtla/statsforecast&via=nixtlainc&hashtags=StatisticalModels,TimeSeries,Forecasting) &nbsp;[![Slack](https://img.shields.io/badge/Slack-4A154B?&logo=slack&logoColor=white)](https://join.slack.com/t/nixtlacommunity/shared_invite/zt-1pmhan9j5-F54XR20edHk0UtYAPcW4KQ)
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/Nixtla/neuralforecast/main/nbs/imgs_indx/logo_mid.png">
-<h1 align="center">NixtlaTS</h1>
+<h1 align="center">Nixtla</h1>
 <h3 align="center">Forecast using TimeGPT</h3>
     
 [![CI](https://github.com/Nixtla/nixtla/actions/workflows/ci.yaml/badge.svg?branch=main)](https://github.com/Nixtla/nixtla/actions/workflows/ci.yaml)
-[![Python](https://img.shields.io/pypi/pyversions/nixtlats)](https://pypi.org/project/nixtlats/)
-[![PyPi](https://img.shields.io/pypi/v/nixtlats?color=blue)](https://pypi.org/project/nixtlats/)
-[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://github.com/Nixtla/nixtlats/blob/main/LICENSE)
+[![Python](https://img.shields.io/pypi/pyversions/nixtla)](https://pypi.org/project/nixtla/)
+[![PyPi](https://img.shields.io/pypi/v/nixtla?color=blue)](https://pypi.org/project/nixtla/)
+[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://github.com/Nixtla/nixtla/blob/main/LICENSE)
 [![docs](https://img.shields.io/website-up-down-green-red/http/nixtla.github.io/nixtla.svg?label=docs)](https://nixtla.github.io/nixtla/)
-[![Downloads](https://pepy.tech/badge/nixtlats)](https://pepy.tech/project/nixtlats)
+[![Downloads](https://pepy.tech/badge/nixtla)](https://pepy.tech/project/nixtla)
     
-**NixtlaTS** offers a collection of classes and methods to interact with the API of TimeGPT.
+**Nixtla** offers a collection of classes and methods to interact with the API of TimeGPT.
 </div>
 
 # 🕰️ TimeGPT: Revolutionizing Time-Series Analysis
 
 Developed by Nixtla, TimeGPT is a cutting-edge generative pre-trained transformer model dedicated to prediction tasks. 🚀 By leveraging the most extensive dataset ever – financial, weather, energy, and sales data – TimeGPT brings unparalleled time-series analysis right to your terminal! 👩‍💻👨‍💻
 
 In seconds, TimeGPT can discern complex patterns and predict future data points, transforming the landscape of data science and predictive analytics.
 
 ## ⚙️ Fine-Tuning: For Precision Prediction
 
 In addition to its core capabilities, TimeGPT supports fine-tuning, enhancing its specialization for specific prediction tasks. 🎯 This feature is like training a machine learning model on a targeted data subset to improve its task-specific performance, making TimeGPT an even more versatile tool for your predictive needs.
 
-## 🔄 `NixtlaTS`: Your Gateway to TimeGPT
+## 🔄 `Nixtla`: Your Gateway to TimeGPT
 
-With `NixtlaTS`, you can easily interact with TimeGPT through simple API calls, making the power of TimeGPT readily accessible in your projects.
+With `Nixtla`, you can easily interact with TimeGPT through simple API calls, making the power of TimeGPT readily accessible in your projects.
 
 ## 💻 Installation
 
-Get `NixtlaTS` up and running with a simple pip command:
+Get `Nixtla` up and running with a simple pip command:
 
 ```python
-pip install nixtlats>=0.1.0
+pip install nixtla>=0.1.0
 ```
 
 ## 🎈 Quick Start
 
 Get started with TimeGPT now:
 
 ```python
 df = pd.read_csv('https://raw.githubusercontent.com/Nixtla/transfer-learning-time-series/main/datasets/electricity-short.csv')
 
-from nixtlats import NixtlaClient
+from nixtla import NixtlaClient
 nixtla = NixtlaClient(
     # defaults to os.environ.get("NIXTLA_API_KEY")
     api_key = 'my_api_key_provided_by_nixtla'
 )
 fcst_df = nixtla.forecast(df, h=24, level=[80, 90])
 ```
```

### Comparing `nixtlats-0.3.0/nixtlats.egg-info/SOURCES.txt` & `nixtlats-0.4.0/nixtlats.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 README.md
 setup.py
-action_files/__init__.py
 nixtlats/__init__.py
 nixtlats/_modidx.py
 nixtlats/client.py
 nixtlats/date_features.py
 nixtlats/nixtla_client.py
 nixtlats/py.typed
 nixtlats/utils.py
```

### Comparing `nixtlats-0.3.0/setup.py` & `nixtlats-0.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,38 +9,38 @@
     "nbdev",
     "plotly",
     "pre-commit",
     "python-dotenv",
     "statsforecast",
 ]
 distributed = ["dask[dataframe]", "fugue[ray]>=0.8.7", "pyspark", "ray[serve-grpc]"]
-plotting = ["utilsforecast[plotting]>=0.0.5"]
+plotting = ["utilsforecast[plotting]>=0.1.7"]
 date_extras = ["holidays"]
 
 setuptools.setup(
     name="nixtlats",
-    version="0.3.0",
+    version="0.4.0",
     description="Python SDK for Nixtla API (TimeGPT)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Nixtla/nixtla",
-    packages=setuptools.find_packages(),
+    packages=setuptools.find_packages(exclude=["action_files"]),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=[
         "httpx",
         "pandas",
         "pydantic<2",
         "requests",
         "tenacity",
-        "utilsforecast>=0.0.13",
+        "utilsforecast>=0.1.7",
     ],
     extras_require={
         "dev": dev + distributed + plotting + date_extras,
         "distributed": distributed,
         "plotting": plotting,
         "date_extras": date_extras,
     },
```

