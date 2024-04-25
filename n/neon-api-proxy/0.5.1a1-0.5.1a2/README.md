# Comparing `tmp/neon-api-proxy-0.5.1a1.tar.gz` & `tmp/neon-api-proxy-0.5.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-api-proxy-0.5.1a1.tar", last modified: Tue Apr  9 23:59:53 2024, max compression
+gzip compressed data, was "neon-api-proxy-0.5.1a2.tar", last modified: Thu Apr 25 16:29:17 2024, max compression
```

## Comparing `neon-api-proxy-0.5.1a1.tar` & `neon-api-proxy-0.5.1a2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:59:53.291070 neon-api-proxy-0.5.1a1/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-09 23:59:50.000000 neon-api-proxy-0.5.1a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-09 23:59:53.291070 neon-api-proxy-0.5.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-09 23:59:50.000000 neon-api-proxy-0.5.1a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:59:53.291070 neon-api-proxy-0.5.1a1/neon_api_proxy/
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-09 23:59:50.000000 neon-api-proxy-0.5.1a1/neon_api_proxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-09 23:59:50.000000 neon-api-proxy-0.5.1a1/neon_api_proxy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-09 23:59:50.000000 neon-api-proxy-0.5.1a1/neon_api_proxy/alpha_vantage_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-04-09 23:59:50.000000 neon-api-proxy-0.5.1a1/neon_api_proxy/api_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-04-09 23:59:50.000000 neon-api-proxy-0.5.1a1/neon_api_proxy/cached_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:59:53.291070 neon-api-proxy-0.5.1a1/neon_api_proxy/client/
--rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-04-09 23:59:50.000000 neon-api-proxy-0.5.1a1/neon_api_proxy/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-04-09 23:59:50.000000 neon-api-proxy-0.5.1a1/neon_api_proxy/client/alpha_vantage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-09 23:59:50.000000 neon-api-proxy-0.5.1a1/neon_api_proxy/client/financial_modeling_prep.py
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-09 23:59:50.000000 neon-api-proxy-0.5.1a1/neon_api_proxy/client/map_maker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-04-09 23:59:50.000000 neon-api-proxy-0.5.1a1/neon_api_proxy/client/open_weather_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-04-09 23:59:50.000000 neon-api-proxy-0.5.1a1/neon_api_proxy/client/wolfram_alpha.py
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-09 23:59:50.000000 neon-api-proxy-0.5.1a1/neon_api_proxy/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-04-09 23:59:50.000000 neon-api-proxy-0.5.1a1/neon_api_proxy/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-09 23:59:50.000000 neon-api-proxy-0.5.1a1/neon_api_proxy/owm_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:59:53.291070 neon-api-proxy-0.5.1a1/neon_api_proxy/services/
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-09 23:59:50.000000 neon-api-proxy-0.5.1a1/neon_api_proxy/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-04-09 23:59:50.000000 neon-api-proxy-0.5.1a1/neon_api_proxy/services/alpha_vantage_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-09 23:59:50.000000 neon-api-proxy-0.5.1a1/neon_api_proxy/services/map_maker_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-04-09 23:59:50.000000 neon-api-proxy-0.5.1a1/neon_api_proxy/services/owm_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-09 23:59:50.000000 neon-api-proxy-0.5.1a1/neon_api_proxy/services/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7270 2024-04-09 23:59:50.000000 neon-api-proxy-0.5.1a1/neon_api_proxy/services/wolfram_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-09 23:59:50.000000 neon-api-proxy-0.5.1a1/neon_api_proxy/socket_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-09 23:59:50.000000 neon-api-proxy-0.5.1a1/neon_api_proxy/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-09 23:59:50.000000 neon-api-proxy-0.5.1a1/neon_api_proxy/wolfram_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:59:53.291070 neon-api-proxy-0.5.1a1/neon_api_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-09 23:59:53.000000 neon-api-proxy-0.5.1a1/neon_api_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-09 23:59:53.000000 neon-api-proxy-0.5.1a1/neon_api_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 23:59:53.000000 neon-api-proxy-0.5.1a1/neon_api_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-09 23:59:53.000000 neon-api-proxy-0.5.1a1/neon_api_proxy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-09 23:59:53.000000 neon-api-proxy-0.5.1a1/neon_api_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-09 23:59:53.000000 neon-api-proxy-0.5.1a1/neon_api_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 23:59:53.000000 neon-api-proxy-0.5.1a1/neon_api_proxy.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 23:59:53.291070 neon-api-proxy-0.5.1a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-09 23:59:50.000000 neon-api-proxy-0.5.1a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:17.626588 neon-api-proxy-0.5.1a2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-25 16:29:17.626588 neon-api-proxy-0.5.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:17.622588 neon-api-proxy-0.5.1a2/neon_api_proxy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/alpha_vantage_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/api_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/cached_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:17.622588 neon-api-proxy-0.5.1a2/neon_api_proxy/client/
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/client/alpha_vantage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/client/financial_modeling_prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/client/map_maker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/client/open_weather_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/client/wolfram_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/owm_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:17.626588 neon-api-proxy-0.5.1a2/neon_api_proxy/services/
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/services/alpha_vantage_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/services/map_maker_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/services/owm_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/services/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7270 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/services/wolfram_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/socket_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/wolfram_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:17.622588 neon-api-proxy-0.5.1a2/neon_api_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-25 16:29:17.000000 neon-api-proxy-0.5.1a2/neon_api_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-25 16:29:17.000000 neon-api-proxy-0.5.1a2/neon_api_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:29:17.000000 neon-api-proxy-0.5.1a2/neon_api_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-25 16:29:17.000000 neon-api-proxy-0.5.1a2/neon_api_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-25 16:29:17.000000 neon-api-proxy-0.5.1a2/neon_api_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-25 16:29:17.000000 neon-api-proxy-0.5.1a2/neon_api_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:29:17.000000 neon-api-proxy-0.5.1a2/neon_api_proxy.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 16:29:17.626588 neon-api-proxy-0.5.1a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/setup.py
```

### Comparing `neon-api-proxy-0.5.1a1/LICENSE.md` & `neon-api-proxy-0.5.1a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a1/PKG-INFO` & `neon-api-proxy-0.5.1a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-api-proxy
-Version: 0.5.1a1
+Version: 0.5.1a2
 Summary: Neon Proxy for external API Calls
 Home-page: https://github.com/NeonGeckoCom/neon_api_proxy
 Author: Neongecko
 Author-email: developers@neon.ai
 License: NeonAI License v1.0
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `neon-api-proxy-0.5.1a1/README.md` & `neon-api-proxy-0.5.1a2/README.md`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a1/neon_api_proxy/__init__.py` & `neon-api-proxy-0.5.1a2/neon_api_proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a1/neon_api_proxy/__main__.py` & `neon-api-proxy-0.5.1a2/neon_api_proxy/__main__.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a1/neon_api_proxy/alpha_vantage_api.py` & `neon-api-proxy-0.5.1a2/neon_api_proxy/alpha_vantage_api.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a1/neon_api_proxy/api_connector.py` & `neon-api-proxy-0.5.1a2/neon_api_proxy/api_connector.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a1/neon_api_proxy/cached_api.py` & `neon-api-proxy-0.5.1a2/neon_api_proxy/cached_api.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a1/neon_api_proxy/client/__init__.py` & `neon-api-proxy-0.5.1a2/neon_api_proxy/client/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a1/neon_api_proxy/client/alpha_vantage.py` & `neon-api-proxy-0.5.1a2/neon_api_proxy/client/alpha_vantage.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a1/neon_api_proxy/client/financial_modeling_prep.py` & `neon-api-proxy-0.5.1a2/neon_api_proxy/client/financial_modeling_prep.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a1/neon_api_proxy/client/map_maker.py` & `neon-api-proxy-0.5.1a2/neon_api_proxy/client/map_maker.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a1/neon_api_proxy/client/open_weather_map.py` & `neon-api-proxy-0.5.1a2/neon_api_proxy/client/open_weather_map.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a1/neon_api_proxy/client/wolfram_alpha.py` & `neon-api-proxy-0.5.1a2/neon_api_proxy/client/wolfram_alpha.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a1/neon_api_proxy/config.py` & `neon-api-proxy-0.5.1a2/neon_api_proxy/config.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a1/neon_api_proxy/controller.py` & `neon-api-proxy-0.5.1a2/neon_api_proxy/controller.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a1/neon_api_proxy/owm_api.py` & `neon-api-proxy-0.5.1a2/neon_api_proxy/owm_api.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a1/neon_api_proxy/services/__init__.py` & `neon-api-proxy-0.5.1a2/neon_api_proxy/services/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a1/neon_api_proxy/services/alpha_vantage_api.py` & `neon-api-proxy-0.5.1a2/neon_api_proxy/services/alpha_vantage_api.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a1/neon_api_proxy/services/map_maker_api.py` & `neon-api-proxy-0.5.1a2/neon_api_proxy/services/map_maker_api.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a1/neon_api_proxy/services/owm_api.py` & `neon-api-proxy-0.5.1a2/neon_api_proxy/services/owm_api.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a1/neon_api_proxy/services/test_api.py` & `neon-api-proxy-0.5.1a2/neon_api_proxy/services/test_api.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a1/neon_api_proxy/services/wolfram_api.py` & `neon-api-proxy-0.5.1a2/neon_api_proxy/services/wolfram_api.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a1/neon_api_proxy/socket_handler.py` & `neon-api-proxy-0.5.1a2/neon_api_proxy/socket_handler.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a1/neon_api_proxy/test_api.py` & `neon-api-proxy-0.5.1a2/neon_api_proxy/test_api.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a1/neon_api_proxy/wolfram_api.py` & `neon-api-proxy-0.5.1a2/neon_api_proxy/wolfram_api.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a1/neon_api_proxy.egg-info/PKG-INFO` & `neon-api-proxy-0.5.1a2/neon_api_proxy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-api-proxy
-Version: 0.5.1a1
+Version: 0.5.1a2
 Summary: Neon Proxy for external API Calls
 Home-page: https://github.com/NeonGeckoCom/neon_api_proxy
 Author: Neongecko
 Author-email: developers@neon.ai
 License: NeonAI License v1.0
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `neon-api-proxy-0.5.1a1/neon_api_proxy.egg-info/SOURCES.txt` & `neon-api-proxy-0.5.1a2/neon_api_proxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a1/setup.py` & `neon-api-proxy-0.5.1a2/setup.py`

 * *Files identical despite different names*

