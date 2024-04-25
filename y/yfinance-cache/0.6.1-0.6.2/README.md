# Comparing `tmp/yfinance_cache-0.6.1.tar.gz` & `tmp/yfinance_cache-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yfinance_cache-0.6.1.tar", last modified: Tue Apr 16 20:50:13 2024, max compression
+gzip compressed data, was "yfinance_cache-0.6.2.tar", last modified: Thu Apr 25 17:59:14 2024, max compression
```

## Comparing `yfinance_cache-0.6.1.tar` & `yfinance_cache-0.6.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 gonzo     (1000) gonzo     (1000)        0 2024-04-16 20:50:13.234508 yfinance_cache-0.6.1/
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     1068 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/LICENSE
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     5986 2024-04-16 20:50:13.234508 yfinance_cache-0.6.1/PKG-INFO
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     5294 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/README.md
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)      104 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/pyproject.toml
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)      829 2024-04-16 20:50:13.235509 yfinance_cache-0.6.1/setup.cfg
-drwxr-xr-x   0 gonzo     (1000) gonzo     (1000)        0 2024-04-16 20:50:13.234508 yfinance_cache-0.6.1/tests/
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)       21 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/__init__.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     1675 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/context.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     8469 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_cache.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)      991 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_datetime-assumptions.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    74555 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_market_intervals_asx.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    70793 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_market_intervals_nze.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    74237 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_market_intervals_tlv.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    71006 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_market_intervals_usa.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    24913 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_market_schedules_asx.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    24789 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_market_schedules_nze.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    32509 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_market_schedules_tlv.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    23272 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_market_schedules_usa.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    12038 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_missing_intervals_asx.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    12079 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_missing_intervals_nze.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    13799 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_missing_intervals_tlv.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    13077 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_missing_intervals_usa.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    25165 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_price_data_aging_1d.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    16811 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_price_data_aging_1h.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    17013 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_price_data_aging_1w.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     2447 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_time_utils.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     1698 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_utils.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     2955 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_yf_assumptions.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    32294 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_yfc_adjust.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    12038 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_yfc_backend.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    12467 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_yfc_financials.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    40121 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_yfc_interface.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     4270 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_yfc_ticker.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     5085 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/utils.py
-drwxr-xr-x   0 gonzo     (1000) gonzo     (1000)        0 2024-04-16 20:50:13.228508 yfinance_cache-0.6.1/yfinance_cache/
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)      354 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/yfinance_cache/__init__.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    16324 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/yfinance_cache/yfc_cache_manager.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    52610 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/yfinance_cache/yfc_dat.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    89428 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/yfinance_cache/yfc_financials_manager.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     2197 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/yfinance_cache/yfc_logging.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     6792 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/yfinance_cache/yfc_multi.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     1453 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/yfinance_cache/yfc_options.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)   204038 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/yfinance_cache/yfc_prices_manager.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    39338 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/yfinance_cache/yfc_ticker.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    81302 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/yfinance_cache/yfc_time.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)      653 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/yfinance_cache/yfc_upgrade.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    25372 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/yfinance_cache/yfc_utils.py
-drwxr-xr-x   0 gonzo     (1000) gonzo     (1000)        0 2024-04-16 20:50:13.234508 yfinance_cache-0.6.1/yfinance_cache.egg-info/
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     5986 2024-04-16 20:50:13.000000 yfinance_cache-0.6.1/yfinance_cache.egg-info/PKG-INFO
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     2316 2024-04-16 20:50:13.000000 yfinance_cache-0.6.1/yfinance_cache.egg-info/SOURCES.txt
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)        1 2024-04-16 20:50:13.000000 yfinance_cache-0.6.1/yfinance_cache.egg-info/dependency_links.txt
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)       79 2024-04-16 20:50:13.000000 yfinance_cache-0.6.1/yfinance_cache.egg-info/requires.txt
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)       21 2024-04-16 20:50:13.000000 yfinance_cache-0.6.1/yfinance_cache.egg-info/top_level.txt
+drwxr-xr-x   0 gonzo     (1000) gonzo     (1000)        0 2024-04-25 17:59:14.054618 yfinance_cache-0.6.2/
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     1068 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/LICENSE
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     5939 2024-04-25 17:59:14.054618 yfinance_cache-0.6.2/PKG-INFO
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     5247 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/README.md
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)      104 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/pyproject.toml
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)      829 2024-04-25 17:59:14.054618 yfinance_cache-0.6.2/setup.cfg
+drwxr-xr-x   0 gonzo     (1000) gonzo     (1000)        0 2024-04-25 17:59:14.053618 yfinance_cache-0.6.2/tests/
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)       21 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/tests/__init__.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     1675 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/tests/context.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     8469 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/tests/test_cache.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)      991 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/tests/test_datetime-assumptions.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    74555 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/tests/test_market_intervals_asx.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    70793 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/tests/test_market_intervals_nze.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    74237 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/tests/test_market_intervals_tlv.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    71006 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/tests/test_market_intervals_usa.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    24913 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/tests/test_market_schedules_asx.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    24789 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/tests/test_market_schedules_nze.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    32509 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/tests/test_market_schedules_tlv.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    23272 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/tests/test_market_schedules_usa.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    12038 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/tests/test_missing_intervals_asx.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    12079 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/tests/test_missing_intervals_nze.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    13799 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/tests/test_missing_intervals_tlv.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    13077 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/tests/test_missing_intervals_usa.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    25165 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/tests/test_price_data_aging_1d.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    16811 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/tests/test_price_data_aging_1h.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    17013 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/tests/test_price_data_aging_1w.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     2447 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/tests/test_time_utils.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     1698 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/tests/test_utils.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     2955 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/tests/test_yf_assumptions.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    32294 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/tests/test_yfc_adjust.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    12038 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/tests/test_yfc_backend.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    12467 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/tests/test_yfc_financials.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    40121 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/tests/test_yfc_interface.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     4270 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/tests/test_yfc_ticker.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     5085 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/tests/utils.py
+drwxr-xr-x   0 gonzo     (1000) gonzo     (1000)        0 2024-04-25 17:59:14.047618 yfinance_cache-0.6.2/yfinance_cache/
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)      354 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/yfinance_cache/__init__.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    16324 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/yfinance_cache/yfc_cache_manager.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    52610 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/yfinance_cache/yfc_dat.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    89428 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/yfinance_cache/yfc_financials_manager.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     2197 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/yfinance_cache/yfc_logging.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     6792 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/yfinance_cache/yfc_multi.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     1453 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/yfinance_cache/yfc_options.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)   204038 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/yfinance_cache/yfc_prices_manager.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    39338 2024-04-25 17:58:13.000000 yfinance_cache-0.6.2/yfinance_cache/yfc_ticker.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    81302 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/yfinance_cache/yfc_time.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)      653 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/yfinance_cache/yfc_upgrade.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    25372 2024-04-25 17:55:15.000000 yfinance_cache-0.6.2/yfinance_cache/yfc_utils.py
+drwxr-xr-x   0 gonzo     (1000) gonzo     (1000)        0 2024-04-25 17:59:14.054618 yfinance_cache-0.6.2/yfinance_cache.egg-info/
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     5939 2024-04-25 17:59:14.000000 yfinance_cache-0.6.2/yfinance_cache.egg-info/PKG-INFO
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     2316 2024-04-25 17:59:14.000000 yfinance_cache-0.6.2/yfinance_cache.egg-info/SOURCES.txt
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)        1 2024-04-25 17:59:14.000000 yfinance_cache-0.6.2/yfinance_cache.egg-info/dependency_links.txt
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)       79 2024-04-25 17:59:14.000000 yfinance_cache-0.6.2/yfinance_cache.egg-info/requires.txt
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)       21 2024-04-25 17:59:14.000000 yfinance_cache-0.6.2/yfinance_cache.egg-info/top_level.txt
```

### Comparing `yfinance_cache-0.6.1/LICENSE` & `yfinance_cache-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yfinance_cache-0.6.1/PKG-INFO` & `yfinance_cache-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yfinance-cache
-Version: 0.6.1
+Version: 0.6.2
 Summary: Smart caching wrapper for 'yfinance' module
 Home-page: https://github.com/ValueRaider/yfinance-cache
 Author: ValueRaider
 Author-email: ValueRaider@protonmail.com
 Project-URL: Bug Tracker, https://github.com/ValueRaider/yfinance-cache/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -167,9 +167,8 @@
 
 ## Installation
 
 Available on PIP: `pip install yfinance_cache`
 
 ## Limitations
 
-- only price data is checked if refresh needed
 - intraday pre/post price data not available
```

### Comparing `yfinance_cache-0.6.1/README.md` & `yfinance_cache-0.6.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -147,9 +147,8 @@
 
 ## Installation
 
 Available on PIP: `pip install yfinance_cache`
 
 ## Limitations
 
-- only price data is checked if refresh needed
 - intraday pre/post price data not available
```

### Comparing `yfinance_cache-0.6.1/setup.cfg` & `yfinance_cache-0.6.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = yfinance-cache
-version = 0.6.1
+version = 0.6.2
 author = ValueRaider
 author_email = ValueRaider@protonmail.com
 description = Smart caching wrapper for 'yfinance' module
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ValueRaider/yfinance-cache
 project_urls =
```

### Comparing `yfinance_cache-0.6.1/tests/context.py` & `yfinance_cache-0.6.2/tests/context.py`

 * *Files identical despite different names*

### Comparing `yfinance_cache-0.6.1/tests/test_cache.py` & `yfinance_cache-0.6.2/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `yfinance_cache-0.6.1/tests/test_datetime-assumptions.py` & `yfinance_cache-0.6.2/tests/test_datetime-assumptions.py`

 * *Files identical despite different names*

### Comparing `yfinance_cache-0.6.1/tests/test_market_intervals_asx.py` & `yfinance_cache-0.6.2/tests/test_market_intervals_asx.py`

 * *Files identical despite different names*

### Comparing `yfinance_cache-0.6.1/tests/test_market_intervals_nze.py` & `yfinance_cache-0.6.2/tests/test_market_intervals_nze.py`

 * *Files identical despite different names*

### Comparing `yfinance_cache-0.6.1/tests/test_market_intervals_tlv.py` & `yfinance_cache-0.6.2/tests/test_market_intervals_tlv.py`

 * *Files identical despite different names*

### Comparing `yfinance_cache-0.6.1/tests/test_market_intervals_usa.py` & `yfinance_cache-0.6.2/tests/test_market_intervals_usa.py`

 * *Files identical despite different names*

### Comparing `yfinance_cache-0.6.1/tests/test_market_schedules_asx.py` & `yfinance_cache-0.6.2/tests/test_market_schedules_asx.py`

 * *Files identical despite different names*

### Comparing `yfinance_cache-0.6.1/tests/test_market_schedules_nze.py` & `yfinance_cache-0.6.2/tests/test_market_schedules_nze.py`

 * *Files identical despite different names*

### Comparing `yfinance_cache-0.6.1/tests/test_market_schedules_tlv.py` & `yfinance_cache-0.6.2/tests/test_market_schedules_tlv.py`

 * *Files identical despite different names*

### Comparing `yfinance_cache-0.6.1/tests/test_market_schedules_usa.py` & `yfinance_cache-0.6.2/tests/test_market_schedules_usa.py`

 * *Files identical despite different names*

### Comparing `yfinance_cache-0.6.1/tests/test_missing_intervals_asx.py` & `yfinance_cache-0.6.2/tests/test_missing_intervals_asx.py`

 * *Files identical despite different names*

### Comparing `yfinance_cache-0.6.1/tests/test_missing_intervals_nze.py` & `yfinance_cache-0.6.2/tests/test_missing_intervals_nze.py`

 * *Files identical despite different names*

### Comparing `yfinance_cache-0.6.1/tests/test_missing_intervals_tlv.py` & `yfinance_cache-0.6.2/tests/test_missing_intervals_tlv.py`

 * *Files identical despite different names*

### Comparing `yfinance_cache-0.6.1/tests/test_missing_intervals_usa.py` & `yfinance_cache-0.6.2/tests/test_missing_intervals_usa.py`

 * *Files identical despite different names*

### Comparing `yfinance_cache-0.6.1/tests/test_price_data_aging_1d.py` & `yfinance_cache-0.6.2/tests/test_price_data_aging_1d.py`

 * *Files identical despite different names*

### Comparing `yfinance_cache-0.6.1/tests/test_price_data_aging_1h.py` & `yfinance_cache-0.6.2/tests/test_price_data_aging_1h.py`

 * *Files identical despite different names*

### Comparing `yfinance_cache-0.6.1/tests/test_price_data_aging_1w.py` & `yfinance_cache-0.6.2/tests/test_price_data_aging_1w.py`

 * *Files identical despite different names*

### Comparing `yfinance_cache-0.6.1/tests/test_time_utils.py` & `yfinance_cache-0.6.2/tests/test_time_utils.py`

 * *Files identical despite different names*

### Comparing `yfinance_cache-0.6.1/tests/test_utils.py` & `yfinance_cache-0.6.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `yfinance_cache-0.6.1/tests/test_yf_assumptions.py` & `yfinance_cache-0.6.2/tests/test_yf_assumptions.py`

 * *Files identical despite different names*

### Comparing `yfinance_cache-0.6.1/tests/test_yfc_adjust.py` & `yfinance_cache-0.6.2/tests/test_yfc_adjust.py`

 * *Files identical despite different names*

### Comparing `yfinance_cache-0.6.1/tests/test_yfc_backend.py` & `yfinance_cache-0.6.2/tests/test_yfc_backend.py`

 * *Files identical despite different names*

### Comparing `yfinance_cache-0.6.1/tests/test_yfc_financials.py` & `yfinance_cache-0.6.2/tests/test_yfc_financials.py`

 * *Files identical despite different names*

### Comparing `yfinance_cache-0.6.1/tests/test_yfc_interface.py` & `yfinance_cache-0.6.2/tests/test_yfc_interface.py`

 * *Files identical despite different names*

### Comparing `yfinance_cache-0.6.1/tests/test_yfc_ticker.py` & `yfinance_cache-0.6.2/tests/test_yfc_ticker.py`

 * *Files identical despite different names*

### Comparing `yfinance_cache-0.6.1/tests/utils.py` & `yfinance_cache-0.6.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `yfinance_cache-0.6.1/yfinance_cache/yfc_cache_manager.py` & `yfinance_cache-0.6.2/yfinance_cache/yfc_cache_manager.py`

 * *Files identical despite different names*

### Comparing `yfinance_cache-0.6.1/yfinance_cache/yfc_dat.py` & `yfinance_cache-0.6.2/yfinance_cache/yfc_dat.py`

 * *Files identical despite different names*

### Comparing `yfinance_cache-0.6.1/yfinance_cache/yfc_financials_manager.py` & `yfinance_cache-0.6.2/yfinance_cache/yfc_financials_manager.py`

 * *Files identical despite different names*

### Comparing `yfinance_cache-0.6.1/yfinance_cache/yfc_logging.py` & `yfinance_cache-0.6.2/yfinance_cache/yfc_logging.py`

 * *Files identical despite different names*

### Comparing `yfinance_cache-0.6.1/yfinance_cache/yfc_multi.py` & `yfinance_cache-0.6.2/yfinance_cache/yfc_multi.py`

 * *Files identical despite different names*

### Comparing `yfinance_cache-0.6.1/yfinance_cache/yfc_options.py` & `yfinance_cache-0.6.2/yfinance_cache/yfc_options.py`

 * *Files identical despite different names*

### Comparing `yfinance_cache-0.6.1/yfinance_cache/yfc_prices_manager.py` & `yfinance_cache-0.6.2/yfinance_cache/yfc_prices_manager.py`

 * *Files identical despite different names*

### Comparing `yfinance_cache-0.6.1/yfinance_cache/yfc_ticker.py` & `yfinance_cache-0.6.2/yfinance_cache/yfc_ticker.py`

 * *Files 0% similar despite different names*

```diff
@@ -534,15 +534,15 @@
                 print(f'{self.ticker}: {msg}')
                 yfcm.WriteCacheMetadata(self.ticker, "info", 'LastCheck', i['FetchDate'])
                 return self._info
 
         self._info = i
         if md is None:
             md = {}
-        mf['LastCheck'] = i['FetchDate']
+        md['LastCheck'] = i['FetchDate']
         yfcm.StoreCacheDatum(self.ticker, "info", self._info, metadata=md)
 
         exchange, tz_name = self._getExchangeAndTz()
         yfct.SetExchangeTzName(exchange, tz_name)
 
         return self._info
```

### Comparing `yfinance_cache-0.6.1/yfinance_cache/yfc_time.py` & `yfinance_cache-0.6.2/yfinance_cache/yfc_time.py`

 * *Files identical despite different names*

### Comparing `yfinance_cache-0.6.1/yfinance_cache/yfc_upgrade.py` & `yfinance_cache-0.6.2/yfinance_cache/yfc_upgrade.py`

 * *Files identical despite different names*

### Comparing `yfinance_cache-0.6.1/yfinance_cache/yfc_utils.py` & `yfinance_cache-0.6.2/yfinance_cache/yfc_utils.py`

 * *Files identical despite different names*

### Comparing `yfinance_cache-0.6.1/yfinance_cache.egg-info/PKG-INFO` & `yfinance_cache-0.6.2/yfinance_cache.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yfinance-cache
-Version: 0.6.1
+Version: 0.6.2
 Summary: Smart caching wrapper for 'yfinance' module
 Home-page: https://github.com/ValueRaider/yfinance-cache
 Author: ValueRaider
 Author-email: ValueRaider@protonmail.com
 Project-URL: Bug Tracker, https://github.com/ValueRaider/yfinance-cache/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -167,9 +167,8 @@
 
 ## Installation
 
 Available on PIP: `pip install yfinance_cache`
 
 ## Limitations
 
-- only price data is checked if refresh needed
 - intraday pre/post price data not available
```

### Comparing `yfinance_cache-0.6.1/yfinance_cache.egg-info/SOURCES.txt` & `yfinance_cache-0.6.2/yfinance_cache.egg-info/SOURCES.txt`

 * *Files identical despite different names*

