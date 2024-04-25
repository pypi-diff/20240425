# Comparing `tmp/nixtla-0.0.2.tar.gz` & `tmp/nixtla-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nixtla-0.0.2.tar", last modified: Sat Oct  7 03:09:42 2023, max compression
+gzip compressed data, was "nixtla-0.4.0.tar", last modified: Thu Apr 25 02:01:19 2024, max compression
```

## Comparing `nixtla-0.0.2.tar` & `nixtla-0.4.0.tar`

### file list

```diff
@@ -1,11 +1,57 @@
-drwxr-xr-x   0 fedex      (501) staff       (20)        0 2023-10-07 03:09:42.129847 nixtla-0.0.2/
--rw-r--r--   0 fedex      (501) staff       (20)    11357 2023-07-25 17:03:20.000000 nixtla-0.0.2/LICENSE
--rw-r--r--   0 fedex      (501) staff       (20)      415 2023-10-07 03:09:42.129380 nixtla-0.0.2/PKG-INFO
--rw-r--r--   0 fedex      (501) staff       (20)       33 2023-07-25 17:03:20.000000 nixtla-0.0.2/README.md
-drwxr-xr-x   0 fedex      (501) staff       (20)        0 2023-10-07 03:09:42.129198 nixtla-0.0.2/nixtla.egg-info/
--rw-r--r--   0 fedex      (501) staff       (20)      415 2023-10-07 03:09:41.000000 nixtla-0.0.2/nixtla.egg-info/PKG-INFO
--rw-r--r--   0 fedex      (501) staff       (20)      146 2023-10-07 03:09:42.000000 nixtla-0.0.2/nixtla.egg-info/SOURCES.txt
--rw-r--r--   0 fedex      (501) staff       (20)        1 2023-10-07 03:09:41.000000 nixtla-0.0.2/nixtla.egg-info/dependency_links.txt
--rw-r--r--   0 fedex      (501) staff       (20)        1 2023-10-07 03:09:42.000000 nixtla-0.0.2/nixtla.egg-info/top_level.txt
--rw-r--r--   0 fedex      (501) staff       (20)       38 2023-10-07 03:09:42.129904 nixtla-0.0.2/setup.cfg
--rw-r--r--   0 fedex      (501) staff       (20)      549 2023-10-07 03:09:35.000000 nixtla-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:01:19.340592 nixtla-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11414 2024-04-25 02:01:13.000000 nixtla-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-04-25 02:01:19.340592 nixtla-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-25 02:01:13.000000 nixtla-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:01:19.332591 nixtla-0.4.0/nixtla/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19978 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48931 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:01:19.332591 nixtla-0.4.0/nixtla/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/core/api_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/core/client_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/core/datetime_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/core/jsonable_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/core/remove_none_from_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/date_features.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:01:19.332591 nixtla-0.4.0/nixtla/distributed/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11177 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/distributed/nixtla_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:01:19.332591 nixtla-0.4.0/nixtla/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/errors/unprocessable_entity_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64067 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/nixtla_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:01:19.336591 nixtla-0.4.0/nixtla/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/multi_series_anomaly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/multi_series_anomaly_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/multi_series_cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/multi_series_cross_validation_fewshot_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/multi_series_cross_validation_finetune_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/multi_series_cross_validation_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/multi_series_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/multi_series_forecast_fewshot_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/multi_series_forecast_finetune_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/multi_series_forecast_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/multi_series_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/multi_series_insample_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/multi_series_insample_forecast_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/single_series_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/single_series_forecast_fewshot_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/single_series_forecast_finetune_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/single_series_forecast_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/single_series_insample_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/single_series_insample_forecast_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/validation_error_loc_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:01:19.336591 nixtla-0.4.0/nixtla.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-04-25 02:01:19.000000 nixtla-0.4.0/nixtla.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-25 02:01:19.000000 nixtla-0.4.0/nixtla.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 02:01:19.000000 nixtla-0.4.0/nixtla.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-25 02:01:19.000000 nixtla-0.4.0/nixtla.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 02:01:19.000000 nixtla-0.4.0/nixtla.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 02:01:19.340592 nixtla-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-25 02:01:13.000000 nixtla-0.4.0/setup.py
```

### Comparing `nixtla-0.0.2/LICENSE` & `nixtla-0.4.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-                                 Apache License
+Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION FOR THE PYTHON SDK 
+(FOR TERMS AND CONDITIONS OF TIME GPT VISIT https://docs.nixtla.io/docs/terms-and-conditions)
 
    1. Definitions.
 
       "License" shall mean the terms and conditions for use, reproduction,
       and distribution as defined by Sections 1 through 9 of this document.
 
       "Licensor" shall mean the copyright owner or entity authorized by
@@ -182,15 +183,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [yyyy] [name of copyright owner]
+   Copyright 2022 Nixtla
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

