# Comparing `tmp/quant1x-base-0.3.9.tar.gz` & `tmp/quant1x_base-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quant1x-base-0.3.9.tar", last modified: Sun Feb 18 08:55:39 2024, max compression
+gzip compressed data, was "quant1x_base-0.4.1.tar", last modified: Wed Apr 24 22:59:23 2024, max compression
```

## Comparing `quant1x-base-0.3.9.tar` & `quant1x_base-0.4.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 wangfeng   (501) staff       (20)        0 2024-02-18 08:55:39.322058 quant1x-base-0.3.9/
--rw-r--r--   0 wangfeng   (501) staff       (20)     1087 2023-11-19 21:55:22.000000 quant1x-base-0.3.9/LICENSE
--rw-r--r--   0 wangfeng   (501) staff       (20)      926 2024-02-18 08:55:39.321148 quant1x-base-0.3.9/PKG-INFO
--rw-r--r--   0 wangfeng   (501) staff       (20)       49 2023-11-19 23:24:11.000000 quant1x-base-0.3.9/README.md
-drwxr-xr-x   0 wangfeng   (501) staff       (20)        0 2024-02-18 08:55:39.315106 quant1x-base-0.3.9/base1x/
--rw-r--r--   0 wangfeng   (501) staff       (20)      478 2024-01-20 23:42:40.000000 quant1x-base-0.3.9/base1x/__init__.py
--rw-r--r--   0 wangfeng   (501) staff       (20)      730 2024-01-21 06:59:21.000000 quant1x-base-0.3.9/base1x/app.py
--rw-r--r--   0 wangfeng   (501) staff       (20)     1314 2023-12-11 22:41:35.000000 quant1x-base-0.3.9/base1x/config.py
--rw-r--r--   0 wangfeng   (501) staff       (20)      394 2023-11-27 22:38:37.000000 quant1x-base-0.3.9/base1x/device.py
--rw-r--r--   0 wangfeng   (501) staff       (20)      653 2023-11-29 21:25:24.000000 quant1x-base-0.3.9/base1x/devp.py
--rw-r--r--   0 wangfeng   (501) staff       (20)      750 2024-01-21 06:59:21.000000 quant1x-base-0.3.9/base1x/file.py
--rw-r--r--   0 wangfeng   (501) staff       (20)      538 2024-01-21 10:12:23.000000 quant1x-base-0.3.9/base1x/logger.py
--rw-r--r--   0 wangfeng   (501) staff       (20)     1496 2023-11-30 20:02:54.000000 quant1x-base-0.3.9/base1x/market.py
--rw-r--r--   0 wangfeng   (501) staff       (20)     1261 2023-11-29 06:37:40.000000 quant1x-base-0.3.9/base1x/network.py
--rw-r--r--   0 wangfeng   (501) staff       (20)      725 2023-11-30 00:06:43.000000 quant1x-base-0.3.9/base1x/num.py
--rw-r--r--   0 wangfeng   (501) staff       (20)      448 2023-11-29 21:25:24.000000 quant1x-base-0.3.9/base1x/pattern.py
--rw-r--r--   0 wangfeng   (501) staff       (20)     3589 2023-11-29 21:25:24.000000 quant1x-base-0.3.9/base1x/timestamp.py
--rw-r--r--   0 wangfeng   (501) staff       (20)     1531 2023-11-29 21:25:24.000000 quant1x-base-0.3.9/base1x/version.py
-drwxr-xr-x   0 wangfeng   (501) staff       (20)        0 2024-02-18 08:55:39.320309 quant1x-base-0.3.9/quant1x_base.egg-info/
--rw-r--r--   0 wangfeng   (501) staff       (20)      926 2024-02-18 08:55:39.000000 quant1x-base-0.3.9/quant1x_base.egg-info/PKG-INFO
--rw-r--r--   0 wangfeng   (501) staff       (20)      459 2024-02-18 08:55:39.000000 quant1x-base-0.3.9/quant1x_base.egg-info/SOURCES.txt
--rw-r--r--   0 wangfeng   (501) staff       (20)        1 2024-02-18 08:55:39.000000 quant1x-base-0.3.9/quant1x_base.egg-info/dependency_links.txt
--rw-r--r--   0 wangfeng   (501) staff       (20)        1 2024-02-18 08:55:39.000000 quant1x-base-0.3.9/quant1x_base.egg-info/not-zip-safe
--rw-r--r--   0 wangfeng   (501) staff       (20)       95 2024-02-18 08:55:39.000000 quant1x-base-0.3.9/quant1x_base.egg-info/requires.txt
--rw-r--r--   0 wangfeng   (501) staff       (20)        7 2024-02-18 08:55:39.000000 quant1x-base-0.3.9/quant1x_base.egg-info/top_level.txt
--rw-r--r--   0 wangfeng   (501) staff       (20)       38 2024-02-18 08:55:39.322568 quant1x-base-0.3.9/setup.cfg
--rw-r--r--   0 wangfeng   (501) staff       (20)     2240 2023-12-08 01:54:13.000000 quant1x-base-0.3.9/setup.py
+drwxr-xr-x   0 wangfeng   (501) staff       (20)        0 2024-04-24 22:59:23.195519 quant1x_base-0.4.1/
+-rw-r--r--   0 wangfeng   (501) staff       (20)     1087 2023-11-19 21:55:22.000000 quant1x_base-0.4.1/LICENSE
+-rw-r--r--   0 wangfeng   (501) staff       (20)      990 2024-04-24 22:59:23.194799 quant1x_base-0.4.1/PKG-INFO
+-rw-r--r--   0 wangfeng   (501) staff       (20)       49 2023-11-19 23:24:11.000000 quant1x_base-0.4.1/README.md
+drwxr-xr-x   0 wangfeng   (501) staff       (20)        0 2024-04-24 22:59:23.189505 quant1x_base-0.4.1/base1x/
+-rw-r--r--   0 wangfeng   (501) staff       (20)      478 2024-01-20 23:42:40.000000 quant1x_base-0.4.1/base1x/__init__.py
+-rw-r--r--   0 wangfeng   (501) staff       (20)      730 2024-01-21 06:59:21.000000 quant1x_base-0.4.1/base1x/app.py
+-rw-r--r--   0 wangfeng   (501) staff       (20)     1314 2023-12-11 22:41:35.000000 quant1x_base-0.4.1/base1x/config.py
+-rw-r--r--   0 wangfeng   (501) staff       (20)      394 2023-11-27 22:38:37.000000 quant1x_base-0.4.1/base1x/device.py
+-rw-r--r--   0 wangfeng   (501) staff       (20)      653 2023-11-29 21:25:24.000000 quant1x_base-0.4.1/base1x/devp.py
+-rw-r--r--   0 wangfeng   (501) staff       (20)      750 2024-01-21 06:59:21.000000 quant1x_base-0.4.1/base1x/file.py
+-rw-r--r--   0 wangfeng   (501) staff       (20)      538 2024-01-21 10:12:23.000000 quant1x_base-0.4.1/base1x/logger.py
+-rw-r--r--   0 wangfeng   (501) staff       (20)     1496 2023-11-30 20:02:54.000000 quant1x_base-0.4.1/base1x/market.py
+-rw-r--r--   0 wangfeng   (501) staff       (20)     1261 2023-11-29 06:37:40.000000 quant1x_base-0.4.1/base1x/network.py
+-rw-r--r--   0 wangfeng   (501) staff       (20)      725 2023-11-30 00:06:43.000000 quant1x_base-0.4.1/base1x/num.py
+-rw-r--r--   0 wangfeng   (501) staff       (20)      448 2023-11-29 21:25:24.000000 quant1x_base-0.4.1/base1x/pattern.py
+-rw-r--r--   0 wangfeng   (501) staff       (20)     3589 2023-11-29 21:25:24.000000 quant1x_base-0.4.1/base1x/timestamp.py
+-rw-r--r--   0 wangfeng   (501) staff       (20)     1531 2023-11-29 21:25:24.000000 quant1x_base-0.4.1/base1x/version.py
+drwxr-xr-x   0 wangfeng   (501) staff       (20)        0 2024-04-24 22:59:23.194054 quant1x_base-0.4.1/quant1x_base.egg-info/
+-rw-r--r--   0 wangfeng   (501) staff       (20)      990 2024-04-24 22:59:23.000000 quant1x_base-0.4.1/quant1x_base.egg-info/PKG-INFO
+-rw-r--r--   0 wangfeng   (501) staff       (20)      459 2024-04-24 22:59:23.000000 quant1x_base-0.4.1/quant1x_base.egg-info/SOURCES.txt
+-rw-r--r--   0 wangfeng   (501) staff       (20)        1 2024-04-24 22:59:23.000000 quant1x_base-0.4.1/quant1x_base.egg-info/dependency_links.txt
+-rw-r--r--   0 wangfeng   (501) staff       (20)        1 2024-04-24 22:59:23.000000 quant1x_base-0.4.1/quant1x_base.egg-info/not-zip-safe
+-rw-r--r--   0 wangfeng   (501) staff       (20)      129 2024-04-24 22:59:23.000000 quant1x_base-0.4.1/quant1x_base.egg-info/requires.txt
+-rw-r--r--   0 wangfeng   (501) staff       (20)        7 2024-04-24 22:59:23.000000 quant1x_base-0.4.1/quant1x_base.egg-info/top_level.txt
+-rw-r--r--   0 wangfeng   (501) staff       (20)       38 2024-04-24 22:59:23.195772 quant1x_base-0.4.1/setup.cfg
+-rw-r--r--   0 wangfeng   (501) staff       (20)     2240 2023-12-08 01:54:13.000000 quant1x_base-0.4.1/setup.py
```

### Comparing `quant1x-base-0.3.9/LICENSE` & `quant1x_base-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quant1x-base-0.3.9/PKG-INFO` & `quant1x_base-0.4.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quant1x-base
-Version: 0.3.9
+Version: 0.4.1
 Summary: Quant1X量化系统python基础库
 Home-page: https://gitee.com/quant1x/base
 Author: WangFeng
 Author-email: wangfengxy@sina.cn
 License: MIT license
 Keywords: quant1x base
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -13,18 +13,20 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
-Requires-Dist: setuptools~=69.1.0
-Requires-Dist: GitPython~=3.1.42
+Requires-Dist: setuptools~=69.5.1
+Requires-Dist: twine==5.0.0
+Requires-Dist: wheel==0.43.0
+Requires-Dist: requests-toolbelt==1.0.0
 Requires-Dist: loguru~=0.7.2
 Requires-Dist: icecream~=2.1.3
-Requires-Dist: numpy~=1.26.2
+Requires-Dist: numpy~=1.26.4
 Requires-Dist: PyYAML~=6.0.1
 
 # base
 
 #### 介绍
 quant1x系统python基础库
```

### Comparing `quant1x-base-0.3.9/base1x/app.py` & `quant1x_base-0.4.1/base1x/app.py`

 * *Files identical despite different names*

### Comparing `quant1x-base-0.3.9/base1x/config.py` & `quant1x_base-0.4.1/base1x/config.py`

 * *Files identical despite different names*

### Comparing `quant1x-base-0.3.9/base1x/devp.py` & `quant1x_base-0.4.1/base1x/devp.py`

 * *Files identical despite different names*

### Comparing `quant1x-base-0.3.9/base1x/file.py` & `quant1x_base-0.4.1/base1x/file.py`

 * *Files identical despite different names*

### Comparing `quant1x-base-0.3.9/base1x/logger.py` & `quant1x_base-0.4.1/base1x/logger.py`

 * *Files identical despite different names*

### Comparing `quant1x-base-0.3.9/base1x/market.py` & `quant1x_base-0.4.1/base1x/market.py`

 * *Files identical despite different names*

### Comparing `quant1x-base-0.3.9/base1x/network.py` & `quant1x_base-0.4.1/base1x/network.py`

 * *Files identical despite different names*

### Comparing `quant1x-base-0.3.9/base1x/num.py` & `quant1x_base-0.4.1/base1x/num.py`

 * *Files identical despite different names*

### Comparing `quant1x-base-0.3.9/base1x/timestamp.py` & `quant1x_base-0.4.1/base1x/timestamp.py`

 * *Files identical despite different names*

### Comparing `quant1x-base-0.3.9/base1x/version.py` & `quant1x_base-0.4.1/base1x/version.py`

 * *Files identical despite different names*

### Comparing `quant1x-base-0.3.9/quant1x_base.egg-info/PKG-INFO` & `quant1x_base-0.4.1/quant1x_base.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quant1x-base
-Version: 0.3.9
+Version: 0.4.1
 Summary: Quant1X量化系统python基础库
 Home-page: https://gitee.com/quant1x/base
 Author: WangFeng
 Author-email: wangfengxy@sina.cn
 License: MIT license
 Keywords: quant1x base
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -13,18 +13,20 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
-Requires-Dist: setuptools~=69.1.0
-Requires-Dist: GitPython~=3.1.42
+Requires-Dist: setuptools~=69.5.1
+Requires-Dist: twine==5.0.0
+Requires-Dist: wheel==0.43.0
+Requires-Dist: requests-toolbelt==1.0.0
 Requires-Dist: loguru~=0.7.2
 Requires-Dist: icecream~=2.1.3
-Requires-Dist: numpy~=1.26.2
+Requires-Dist: numpy~=1.26.4
 Requires-Dist: PyYAML~=6.0.1
 
 # base
 
 #### 介绍
 quant1x系统python基础库
```

### Comparing `quant1x-base-0.3.9/setup.py` & `quant1x_base-0.4.1/setup.py`

 * *Files identical despite different names*

