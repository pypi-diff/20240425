# Comparing `tmp/ctrip-app-ui-0.0.5.tar.gz` & `tmp/ctrip-app-ui-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.0.5.tar", last modified: Thu Apr 25 07:31:18 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.0.6.tar", last modified: Thu Apr 25 07:53:38 2024, max compression
```

## Comparing `ctrip-app-ui-0.0.5.tar` & `ctrip-app-ui-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 07:31:18.364153 ctrip-app-ui-0.0.5/
--rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      474 2024-04-25 07:31:18.362158 ctrip-app-ui-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 07:31:18.342211 ctrip-app-ui-0.0.5/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.0.5/capp_ui/__init__.py
--rw-rw-rw-   0        0        0     3028 2024-04-24 09:35:36.000000 ctrip-app-ui-0.0.5/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1191 2024-04-24 09:24:00.000000 ctrip-app-ui-0.0.5/capp_ui/device.py
--rw-rw-rw-   0        0        0     1263 2024-04-24 09:31:47.000000 ctrip-app-ui-0.0.5/capp_ui/dir.py
--rw-rw-rw-   0        0        0    50150 2024-04-25 07:31:00.000000 ctrip-app-ui-0.0.5/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.0.5/capp_ui/fee.py
--rw-rw-rw-   0        0        0     2270 2024-04-24 09:34:43.000000 ctrip-app-ui-0.0.5/capp_ui/libs.py
--rw-rw-rw-   0        0        0    23814 2024-04-24 09:32:32.000000 ctrip-app-ui-0.0.5/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1799 2024-04-24 09:24:12.000000 ctrip-app-ui-0.0.5/capp_ui/platforms.py
--rw-rw-rw-   0        0        0     5563 2024-04-24 09:33:04.000000 ctrip-app-ui-0.0.5/capp_ui/utils.py
--rw-rw-rw-   0        0        0     2676 2024-04-24 15:31:32.000000 ctrip-app-ui-0.0.5/capp_ui/validators.py
-drwxrwxrwx   0        0        0        0 2024-04-25 07:31:18.360172 ctrip-app-ui-0.0.5/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-04-25 07:31:18.000000 ctrip-app-ui-0.0.5/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      426 2024-04-25 07:31:18.000000 ctrip-app-ui-0.0.5/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 07:31:18.000000 ctrip-app-ui-0.0.5/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-25 07:31:18.000000 ctrip-app-ui-0.0.5/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-25 07:31:18.000000 ctrip-app-ui-0.0.5/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 07:31:18.365150 ctrip-app-ui-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-04-25 07:31:11.000000 ctrip-app-ui-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 07:53:38.318488 ctrip-app-ui-0.0.6/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-04-25 07:53:38.317519 ctrip-app-ui-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 07:53:38.303529 ctrip-app-ui-0.0.6/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.0.6/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0     3028 2024-04-24 09:35:36.000000 ctrip-app-ui-0.0.6/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1191 2024-04-24 09:24:00.000000 ctrip-app-ui-0.0.6/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1263 2024-04-24 09:31:47.000000 ctrip-app-ui-0.0.6/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    50150 2024-04-25 07:31:00.000000 ctrip-app-ui-0.0.6/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.0.6/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     2270 2024-04-24 09:34:43.000000 ctrip-app-ui-0.0.6/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    23814 2024-04-24 09:32:32.000000 ctrip-app-ui-0.0.6/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1799 2024-04-24 09:24:12.000000 ctrip-app-ui-0.0.6/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0      689 2024-04-25 07:52:15.000000 ctrip-app-ui-0.0.6/capp_ui/test.py
+-rw-rw-rw-   0        0        0     5563 2024-04-24 09:33:04.000000 ctrip-app-ui-0.0.6/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     2676 2024-04-24 15:31:32.000000 ctrip-app-ui-0.0.6/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-04-25 07:53:38.315496 ctrip-app-ui-0.0.6/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-04-25 07:53:38.000000 ctrip-app-ui-0.0.6/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2024-04-25 07:53:38.000000 ctrip-app-ui-0.0.6/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 07:53:38.000000 ctrip-app-ui-0.0.6/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-25 07:53:38.000000 ctrip-app-ui-0.0.6/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-25 07:53:38.000000 ctrip-app-ui-0.0.6/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 07:53:38.319485 ctrip-app-ui-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-04-25 07:53:30.000000 ctrip-app-ui-0.0.6/setup.py
```

### Comparing `ctrip-app-ui-0.0.5/LICENSE` & `ctrip-app-ui-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.5/capp_ui/date_extend.py` & `ctrip-app-ui-0.0.6/capp_ui/date_extend.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.5/capp_ui/device.py` & `ctrip-app-ui-0.0.6/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.5/capp_ui/dir.py` & `ctrip-app-ui-0.0.6/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.5/capp_ui/domain_service.py` & `ctrip-app-ui-0.0.6/capp_ui/domain_service.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.5/capp_ui/fee.py` & `ctrip-app-ui-0.0.6/capp_ui/fee.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.5/capp_ui/libs.py` & `ctrip-app-ui-0.0.6/capp_ui/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.5/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.0.6/capp_ui/mobile_terminals.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.5/capp_ui/platforms.py` & `ctrip-app-ui-0.0.6/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.5/capp_ui/utils.py` & `ctrip-app-ui-0.0.6/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.5/capp_ui/validators.py` & `ctrip-app-ui-0.0.6/capp_ui/validators.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.5/setup.py` & `ctrip-app-ui-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.0.5',
+    version='0.0.6',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```

