# Comparing `tmp/quant1x-trader-0.7.6.tar.gz` & `tmp/quant1x_trader-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quant1x-trader-0.7.6.tar", last modified: Tue Apr 23 04:54:07 2024, max compression
+gzip compressed data, was "quant1x_trader-0.7.7.tar", last modified: Wed Apr 24 23:25:33 2024, max compression
```

## Comparing `quant1x-trader-0.7.6.tar` & `quant1x_trader-0.7.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 04:54:07.249725 quant1x-trader-0.7.6/
--rw-rw-rw-   0        0        0     1087 2023-11-13 03:59:57.000000 quant1x-trader-0.7.6/LICENSE
--rw-rw-rw-   0        0        0     1340 2024-04-23 04:54:07.248725 quant1x-trader-0.7.6/PKG-INFO
--rw-rw-rw-   0        0        0       60 2023-12-07 15:33:00.000000 quant1x-trader-0.7.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 04:54:07.247720 quant1x-trader-0.7.6/quant1x_trader.egg-info/
--rw-rw-rw-   0        0        0     1340 2024-04-23 04:54:07.000000 quant1x-trader-0.7.6/quant1x_trader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      515 2024-04-23 04:54:07.000000 quant1x-trader-0.7.6/quant1x_trader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 04:54:07.000000 quant1x-trader-0.7.6/quant1x_trader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      138 2024-04-23 04:54:07.000000 quant1x-trader-0.7.6/quant1x_trader.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-23 04:54:07.000000 quant1x-trader-0.7.6/quant1x_trader.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      288 2024-04-23 04:54:07.000000 quant1x-trader-0.7.6/quant1x_trader.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-23 04:54:07.000000 quant1x-trader-0.7.6/quant1x_trader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 04:54:07.249725 quant1x-trader-0.7.6/setup.cfg
--rw-rw-rw-   0        0        0     2284 2024-04-22 05:07:51.000000 quant1x-trader-0.7.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 04:54:07.246210 quant1x-trader-0.7.6/trader1x/
--rw-rw-rw-   0        0        0      103 2024-02-19 01:20:42.000000 quant1x-trader-0.7.6/trader1x/__init__.py
--rw-rw-rw-   0        0        0      197 2023-12-11 07:07:15.000000 quant1x-trader-0.7.6/trader1x/__main__.py
--rw-rw-rw-   0        0        0    16143 2024-02-19 01:20:42.000000 quant1x-trader-0.7.6/trader1x/auto.py
--rw-rw-rw-   0        0        0     8648 2024-02-19 01:20:42.000000 quant1x-trader-0.7.6/trader1x/config.py
--rw-rw-rw-   0        0        0     7922 2024-02-19 01:20:42.000000 quant1x-trader-0.7.6/trader1x/context.py
--rw-rw-rw-   0        0        0     1193 2024-02-19 01:20:42.000000 quant1x-trader-0.7.6/trader1x/log4py.py
--rw-rw-rw-   0        0        0    18556 2024-04-23 04:54:02.000000 quant1x-trader-0.7.6/trader1x/proxy.py
--rw-rw-rw-   0        0        0     1266 2024-04-22 04:56:33.000000 quant1x-trader-0.7.6/trader1x/qmt.py
--rw-rw-rw-   0        0        0    19739 2024-04-22 05:07:58.000000 quant1x-trader-0.7.6/trader1x/thinktrader.py
--rw-rw-rw-   0        0        0     1368 2024-02-19 01:20:42.000000 quant1x-trader-0.7.6/trader1x/utils.py
--rw-rw-rw-   0        0        0    38933 2024-01-21 09:52:15.000000 quant1x-trader-0.7.6/trader1x/win32serviceutil.py
+drwxrwxrwx   0        0        0        0 2024-04-24 23:25:33.380204 quant1x_trader-0.7.7/
+-rw-rw-rw-   0        0        0     1087 2023-11-13 03:59:57.000000 quant1x_trader-0.7.7/LICENSE
+-rw-rw-rw-   0        0        0     1339 2024-04-24 23:25:33.378723 quant1x_trader-0.7.7/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2023-12-07 15:33:00.000000 quant1x_trader-0.7.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 23:25:33.377725 quant1x_trader-0.7.7/quant1x_trader.egg-info/
+-rw-rw-rw-   0        0        0     1339 2024-04-24 23:25:33.000000 quant1x_trader-0.7.7/quant1x_trader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      515 2024-04-24 23:25:33.000000 quant1x_trader-0.7.7/quant1x_trader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 23:25:33.000000 quant1x_trader-0.7.7/quant1x_trader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      138 2024-04-24 23:25:33.000000 quant1x_trader-0.7.7/quant1x_trader.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-24 23:25:33.000000 quant1x_trader-0.7.7/quant1x_trader.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      287 2024-04-24 23:25:33.000000 quant1x_trader-0.7.7/quant1x_trader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-24 23:25:33.000000 quant1x_trader-0.7.7/quant1x_trader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 23:25:33.380204 quant1x_trader-0.7.7/setup.cfg
+-rw-rw-rw-   0        0        0     2284 2024-04-22 05:07:51.000000 quant1x_trader-0.7.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 23:25:33.376718 quant1x_trader-0.7.7/trader1x/
+-rw-rw-rw-   0        0        0      103 2024-02-19 01:20:42.000000 quant1x_trader-0.7.7/trader1x/__init__.py
+-rw-rw-rw-   0        0        0      197 2023-12-11 07:07:15.000000 quant1x_trader-0.7.7/trader1x/__main__.py
+-rw-rw-rw-   0        0        0    16143 2024-02-19 01:20:42.000000 quant1x_trader-0.7.7/trader1x/auto.py
+-rw-rw-rw-   0        0        0     8648 2024-02-19 01:20:42.000000 quant1x_trader-0.7.7/trader1x/config.py
+-rw-rw-rw-   0        0        0     7922 2024-02-19 01:20:42.000000 quant1x_trader-0.7.7/trader1x/context.py
+-rw-rw-rw-   0        0        0     1193 2024-02-19 01:20:42.000000 quant1x_trader-0.7.7/trader1x/log4py.py
+-rw-rw-rw-   0        0        0    18556 2024-04-23 04:54:02.000000 quant1x_trader-0.7.7/trader1x/proxy.py
+-rw-rw-rw-   0        0        0     1266 2024-04-22 04:56:33.000000 quant1x_trader-0.7.7/trader1x/qmt.py
+-rw-rw-rw-   0        0        0    19739 2024-04-22 05:07:58.000000 quant1x_trader-0.7.7/trader1x/thinktrader.py
+-rw-rw-rw-   0        0        0     1368 2024-02-19 01:20:42.000000 quant1x_trader-0.7.7/trader1x/utils.py
+-rw-rw-rw-   0        0        0    38933 2024-01-21 09:52:15.000000 quant1x_trader-0.7.7/trader1x/win32serviceutil.py
```

### Comparing `quant1x-trader-0.7.6/LICENSE` & `quant1x_trader-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `quant1x-trader-0.7.6/PKG-INFO` & `quant1x_trader-0.7.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quant1x-trader
-Version: 0.7.6
+Version: 0.7.7
 Summary: Quant1X程序化自动化交易
 Home-page: https://gitee.com/quant1x/trader
 Author: WangFeng
 Author-email: wangfengxy@sina.cn
 License: MIT license
 Keywords: quant1x auto trader
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -13,27 +13,27 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
-Requires-Dist: setuptools~=69.1.0
-Requires-Dist: future~=0.18.3
+Requires-Dist: setuptools~=69.5.1
+Requires-Dist: future~=1.0.0
 Requires-Dist: numpy~=1.26.4
 Requires-Dist: pandas~=2.2.0
 Requires-Dist: PyYAML~=6.0.1
 Requires-Dist: pywin32==306
-Requires-Dist: uvicorn==0.27.1
+Requires-Dist: uvicorn==0.29.0
 Requires-Dist: fastapi~=0.110.2
-Requires-Dist: path==16.10.0
+Requires-Dist: path==16.14.0
 Requires-Dist: requests==2.31.0
 Requires-Dist: loguru~=0.7.2
-Requires-Dist: quant1x-xtquant==2024.3.29
-Requires-Dist: quant1x-base~=0.3.9
+Requires-Dist: quant1x-xtquant==2024.3.31
+Requires-Dist: quant1x-base~=0.4.2
 Requires-Dist: aiohttp~=3.9.5
 Requires-Dist: sanic==23.12.1
 Requires-Dist: python-multipart~=0.0.9
 Requires-Dist: APScheduler~=3.10.4
 
 # trader
```

### Comparing `quant1x-trader-0.7.6/quant1x_trader.egg-info/PKG-INFO` & `quant1x_trader-0.7.7/quant1x_trader.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quant1x-trader
-Version: 0.7.6
+Version: 0.7.7
 Summary: Quant1X程序化自动化交易
 Home-page: https://gitee.com/quant1x/trader
 Author: WangFeng
 Author-email: wangfengxy@sina.cn
 License: MIT license
 Keywords: quant1x auto trader
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -13,27 +13,27 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
-Requires-Dist: setuptools~=69.1.0
-Requires-Dist: future~=0.18.3
+Requires-Dist: setuptools~=69.5.1
+Requires-Dist: future~=1.0.0
 Requires-Dist: numpy~=1.26.4
 Requires-Dist: pandas~=2.2.0
 Requires-Dist: PyYAML~=6.0.1
 Requires-Dist: pywin32==306
-Requires-Dist: uvicorn==0.27.1
+Requires-Dist: uvicorn==0.29.0
 Requires-Dist: fastapi~=0.110.2
-Requires-Dist: path==16.10.0
+Requires-Dist: path==16.14.0
 Requires-Dist: requests==2.31.0
 Requires-Dist: loguru~=0.7.2
-Requires-Dist: quant1x-xtquant==2024.3.29
-Requires-Dist: quant1x-base~=0.3.9
+Requires-Dist: quant1x-xtquant==2024.3.31
+Requires-Dist: quant1x-base~=0.4.2
 Requires-Dist: aiohttp~=3.9.5
 Requires-Dist: sanic==23.12.1
 Requires-Dist: python-multipart~=0.0.9
 Requires-Dist: APScheduler~=3.10.4
 
 # trader
```

### Comparing `quant1x-trader-0.7.6/quant1x_trader.egg-info/SOURCES.txt` & `quant1x_trader-0.7.7/quant1x_trader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quant1x-trader-0.7.6/setup.py` & `quant1x_trader-0.7.7/setup.py`

 * *Files identical despite different names*

### Comparing `quant1x-trader-0.7.6/trader1x/auto.py` & `quant1x_trader-0.7.7/trader1x/auto.py`

 * *Files identical despite different names*

### Comparing `quant1x-trader-0.7.6/trader1x/config.py` & `quant1x_trader-0.7.7/trader1x/config.py`

 * *Files identical despite different names*

### Comparing `quant1x-trader-0.7.6/trader1x/context.py` & `quant1x_trader-0.7.7/trader1x/context.py`

 * *Files identical despite different names*

### Comparing `quant1x-trader-0.7.6/trader1x/log4py.py` & `quant1x_trader-0.7.7/trader1x/log4py.py`

 * *Files identical despite different names*

### Comparing `quant1x-trader-0.7.6/trader1x/proxy.py` & `quant1x_trader-0.7.7/trader1x/proxy.py`

 * *Files identical despite different names*

### Comparing `quant1x-trader-0.7.6/trader1x/qmt.py` & `quant1x_trader-0.7.7/trader1x/qmt.py`

 * *Files identical despite different names*

### Comparing `quant1x-trader-0.7.6/trader1x/thinktrader.py` & `quant1x_trader-0.7.7/trader1x/thinktrader.py`

 * *Files identical despite different names*

### Comparing `quant1x-trader-0.7.6/trader1x/utils.py` & `quant1x_trader-0.7.7/trader1x/utils.py`

 * *Files identical despite different names*

### Comparing `quant1x-trader-0.7.6/trader1x/win32serviceutil.py` & `quant1x_trader-0.7.7/trader1x/win32serviceutil.py`

 * *Files identical despite different names*

