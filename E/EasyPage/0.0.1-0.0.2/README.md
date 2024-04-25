# Comparing `tmp/EasyPage-0.0.1.tar.gz` & `tmp/EasyPage-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EasyPage-0.0.1.tar", last modified: Thu Apr 25 07:58:21 2024, max compression
+gzip compressed data, was "EasyPage-0.0.2.tar", last modified: Thu Apr 25 08:07:19 2024, max compression
```

## Comparing `EasyPage-0.0.1.tar` & `EasyPage-0.0.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 07:58:21.520489 EasyPage-0.0.1/
-drwxrwxrwx   0        0        0        0 2024-04-25 07:58:21.187650 EasyPage-0.0.1/EasyPage.egg-info/
--rw-rw-rw-   0        0        0      286 2024-04-25 07:58:21.000000 EasyPage-0.0.1/EasyPage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      918 2024-04-25 07:58:21.000000 EasyPage-0.0.1/EasyPage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 07:58:21.000000 EasyPage-0.0.1/EasyPage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2024-04-25 07:58:21.000000 EasyPage-0.0.1/EasyPage.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-25 07:58:21.000000 EasyPage-0.0.1/EasyPage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      286 2024-04-25 07:58:21.519489 EasyPage-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-25 07:58:21.302474 EasyPage-0.0.1/easypage/
--rw-rw-rw-   0        0        0       81 2024-04-22 09:13:20.000000 EasyPage-0.0.1/easypage/__init__.py
--rw-rw-rw-   0        0        0     3243 2024-04-22 08:15:25.000000 EasyPage-0.0.1/easypage/cdp.py
-drwxrwxrwx   0        0        0        0 2024-04-25 07:58:21.452460 EasyPage-0.0.1/easypage/cdp_method/
--rw-rw-rw-   0        0        0        0 2024-04-17 12:56:48.000000 EasyPage-0.0.1/easypage/cdp_method/__init__.py
--rw-rw-rw-   0        0        0     1536 2024-04-24 09:10:40.000000 EasyPage-0.0.1/easypage/cdp_method/browser.py
--rw-rw-rw-   0        0        0    12414 2024-04-24 09:08:35.000000 EasyPage-0.0.1/easypage/cdp_method/dom.py
--rw-rw-rw-   0        0        0     1049 2024-04-24 08:57:22.000000 EasyPage-0.0.1/easypage/cdp_method/emulation.py
--rw-rw-rw-   0        0        0     9545 2024-04-24 14:05:55.000000 EasyPage-0.0.1/easypage/cdp_method/fetch.py
--rw-rw-rw-   0        0        0     2654 2024-04-24 09:06:00.000000 EasyPage-0.0.1/easypage/cdp_method/input.py
--rw-rw-rw-   0        0        0     3598 2024-04-24 11:46:26.000000 EasyPage-0.0.1/easypage/cdp_method/network.py
--rw-rw-rw-   0        0        0     5659 2024-04-24 09:12:45.000000 EasyPage-0.0.1/easypage/cdp_method/page.py
--rw-rw-rw-   0        0        0     3667 2024-04-24 09:16:01.000000 EasyPage-0.0.1/easypage/cdp_method/runtime.py
--rw-rw-rw-   0        0        0     2354 2024-04-24 09:16:01.000000 EasyPage-0.0.1/easypage/cdp_method/security.py
--rw-rw-rw-   0        0        0     1322 2024-04-24 09:16:01.000000 EasyPage-0.0.1/easypage/cdp_method/storage.py
--rw-rw-rw-   0        0        0     5884 2024-04-24 13:35:04.000000 EasyPage-0.0.1/easypage/cdp_method/target.py
--rw-rw-rw-   0        0        0    15945 2024-04-24 13:42:44.000000 EasyPage-0.0.1/easypage/conn.py
--rw-rw-rw-   0        0        0      391 2024-04-25 02:28:17.000000 EasyPage-0.0.1/easypage/definition.py
-drwxrwxrwx   0        0        0        0 2024-04-25 07:58:21.491412 EasyPage-0.0.1/easypage/driver/
--rw-rw-rw-   0        0        0        0 2024-04-09 06:15:36.000000 EasyPage-0.0.1/easypage/driver/__init__.py
--rw-rw-rw-   0        0        0     6188 2024-04-24 14:23:36.000000 EasyPage-0.0.1/easypage/driver/browser.py
--rw-rw-rw-   0        0        0     1587 2024-04-24 02:49:07.000000 EasyPage-0.0.1/easypage/driver/driver.py
--rw-rw-rw-   0        0        0    21191 2024-04-25 07:47:13.000000 EasyPage-0.0.1/easypage/driver/page.py
--rw-rw-rw-   0        0        0     1462 2024-04-24 08:29:43.000000 EasyPage-0.0.1/easypage/errors.py
--rw-rw-rw-   0        0        0     2074 2024-04-22 08:51:10.000000 EasyPage-0.0.1/easypage/logger.py
--rw-rw-rw-   0        0        0     4086 2024-04-25 02:12:39.000000 EasyPage-0.0.1/easypage/main.py
--rw-rw-rw-   0        0        0     4108 2024-04-25 01:40:28.000000 EasyPage-0.0.1/easypage/operate.py
--rw-rw-rw-   0        0        0    10944 2024-04-24 08:39:28.000000 EasyPage-0.0.1/easypage/options.py
--rw-rw-rw-   0        0        0     2787 2024-04-22 08:05:28.000000 EasyPage-0.0.1/easypage/settings.py
-drwxrwxrwx   0        0        0        0 2024-04-25 07:58:21.508488 EasyPage-0.0.1/easypage/utils/
--rw-rw-rw-   0        0        0        0 2024-04-09 06:15:42.000000 EasyPage-0.0.1/easypage/utils/__init__.py
--rw-rw-rw-   0        0        0     3708 2024-04-10 01:27:44.000000 EasyPage-0.0.1/easypage/utils/browser_utils.py
--rw-rw-rw-   0        0        0     1134 2024-04-24 06:28:10.000000 EasyPage-0.0.1/easypage/utils/other_utils.py
--rw-rw-rw-   0        0        0       42 2024-04-25 07:58:21.520489 EasyPage-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      620 2024-04-25 07:58:20.000000 EasyPage-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 08:07:19.214280 EasyPage-0.0.2/
+drwxrwxrwx   0        0        0        0 2024-04-25 08:07:19.183277 EasyPage-0.0.2/EasyPage.egg-info/
+-rw-rw-rw-   0        0        0      286 2024-04-25 08:07:19.000000 EasyPage-0.0.2/EasyPage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      918 2024-04-25 08:07:19.000000 EasyPage-0.0.2/EasyPage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 08:07:19.000000 EasyPage-0.0.2/EasyPage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2024-04-25 08:07:19.000000 EasyPage-0.0.2/EasyPage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-25 08:07:19.000000 EasyPage-0.0.2/EasyPage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      286 2024-04-25 08:07:19.214280 EasyPage-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-25 08:07:19.193277 EasyPage-0.0.2/easypage/
+-rw-rw-rw-   0        0        0       81 2024-04-22 09:13:20.000000 EasyPage-0.0.2/easypage/__init__.py
+-rw-rw-rw-   0        0        0     3243 2024-04-22 08:15:25.000000 EasyPage-0.0.2/easypage/cdp.py
+drwxrwxrwx   0        0        0        0 2024-04-25 08:07:19.205277 EasyPage-0.0.2/easypage/cdp_method/
+-rw-rw-rw-   0        0        0        0 2024-04-17 12:56:48.000000 EasyPage-0.0.2/easypage/cdp_method/__init__.py
+-rw-rw-rw-   0        0        0     1536 2024-04-24 09:10:40.000000 EasyPage-0.0.2/easypage/cdp_method/browser.py
+-rw-rw-rw-   0        0        0    12414 2024-04-24 09:08:35.000000 EasyPage-0.0.2/easypage/cdp_method/dom.py
+-rw-rw-rw-   0        0        0     1049 2024-04-24 08:57:22.000000 EasyPage-0.0.2/easypage/cdp_method/emulation.py
+-rw-rw-rw-   0        0        0     9545 2024-04-24 14:05:55.000000 EasyPage-0.0.2/easypage/cdp_method/fetch.py
+-rw-rw-rw-   0        0        0     2654 2024-04-24 09:06:00.000000 EasyPage-0.0.2/easypage/cdp_method/input.py
+-rw-rw-rw-   0        0        0     3598 2024-04-24 11:46:26.000000 EasyPage-0.0.2/easypage/cdp_method/network.py
+-rw-rw-rw-   0        0        0     5659 2024-04-24 09:12:45.000000 EasyPage-0.0.2/easypage/cdp_method/page.py
+-rw-rw-rw-   0        0        0     3667 2024-04-24 09:16:01.000000 EasyPage-0.0.2/easypage/cdp_method/runtime.py
+-rw-rw-rw-   0        0        0     2354 2024-04-24 09:16:01.000000 EasyPage-0.0.2/easypage/cdp_method/security.py
+-rw-rw-rw-   0        0        0     1322 2024-04-24 09:16:01.000000 EasyPage-0.0.2/easypage/cdp_method/storage.py
+-rw-rw-rw-   0        0        0     5884 2024-04-24 13:35:04.000000 EasyPage-0.0.2/easypage/cdp_method/target.py
+-rw-rw-rw-   0        0        0    15945 2024-04-24 13:42:44.000000 EasyPage-0.0.2/easypage/conn.py
+-rw-rw-rw-   0        0        0      391 2024-04-25 02:28:17.000000 EasyPage-0.0.2/easypage/definition.py
+drwxrwxrwx   0        0        0        0 2024-04-25 08:07:19.209277 EasyPage-0.0.2/easypage/driver/
+-rw-rw-rw-   0        0        0        0 2024-04-09 06:15:36.000000 EasyPage-0.0.2/easypage/driver/__init__.py
+-rw-rw-rw-   0        0        0     6188 2024-04-24 14:23:36.000000 EasyPage-0.0.2/easypage/driver/browser.py
+-rw-rw-rw-   0        0        0     1587 2024-04-24 02:49:07.000000 EasyPage-0.0.2/easypage/driver/driver.py
+-rw-rw-rw-   0        0        0    21191 2024-04-25 07:47:13.000000 EasyPage-0.0.2/easypage/driver/page.py
+-rw-rw-rw-   0        0        0     1462 2024-04-24 08:29:43.000000 EasyPage-0.0.2/easypage/errors.py
+-rw-rw-rw-   0        0        0     2074 2024-04-22 08:51:10.000000 EasyPage-0.0.2/easypage/logger.py
+-rw-rw-rw-   0        0        0     4086 2024-04-25 02:12:39.000000 EasyPage-0.0.2/easypage/main.py
+-rw-rw-rw-   0        0        0     4108 2024-04-25 01:40:28.000000 EasyPage-0.0.2/easypage/operate.py
+-rw-rw-rw-   0        0        0    10944 2024-04-24 08:39:28.000000 EasyPage-0.0.2/easypage/options.py
+-rw-rw-rw-   0        0        0     2787 2024-04-22 08:05:28.000000 EasyPage-0.0.2/easypage/settings.py
+drwxrwxrwx   0        0        0        0 2024-04-25 08:07:19.212278 EasyPage-0.0.2/easypage/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-09 06:15:42.000000 EasyPage-0.0.2/easypage/utils/__init__.py
+-rw-rw-rw-   0        0        0     3708 2024-04-10 01:27:44.000000 EasyPage-0.0.2/easypage/utils/browser_utils.py
+-rw-rw-rw-   0        0        0     1134 2024-04-24 06:28:10.000000 EasyPage-0.0.2/easypage/utils/other_utils.py
+-rw-rw-rw-   0        0        0       42 2024-04-25 08:07:19.215278 EasyPage-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      599 2024-04-25 08:07:16.000000 EasyPage-0.0.2/setup.py
```

### Comparing `EasyPage-0.0.1/EasyPage.egg-info/SOURCES.txt` & `EasyPage-0.0.2/EasyPage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.1/easypage/cdp.py` & `EasyPage-0.0.2/easypage/cdp.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.1/easypage/cdp_method/browser.py` & `EasyPage-0.0.2/easypage/cdp_method/browser.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.1/easypage/cdp_method/dom.py` & `EasyPage-0.0.2/easypage/cdp_method/dom.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.1/easypage/cdp_method/emulation.py` & `EasyPage-0.0.2/easypage/cdp_method/emulation.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.1/easypage/cdp_method/fetch.py` & `EasyPage-0.0.2/easypage/cdp_method/fetch.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.1/easypage/cdp_method/input.py` & `EasyPage-0.0.2/easypage/cdp_method/input.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.1/easypage/cdp_method/network.py` & `EasyPage-0.0.2/easypage/cdp_method/network.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.1/easypage/cdp_method/page.py` & `EasyPage-0.0.2/easypage/cdp_method/page.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.1/easypage/cdp_method/runtime.py` & `EasyPage-0.0.2/easypage/cdp_method/runtime.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.1/easypage/cdp_method/security.py` & `EasyPage-0.0.2/easypage/cdp_method/security.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.1/easypage/cdp_method/storage.py` & `EasyPage-0.0.2/easypage/cdp_method/storage.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.1/easypage/cdp_method/target.py` & `EasyPage-0.0.2/easypage/cdp_method/target.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.1/easypage/conn.py` & `EasyPage-0.0.2/easypage/conn.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.1/easypage/driver/browser.py` & `EasyPage-0.0.2/easypage/driver/browser.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.1/easypage/driver/driver.py` & `EasyPage-0.0.2/easypage/driver/driver.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.1/easypage/driver/page.py` & `EasyPage-0.0.2/easypage/driver/page.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.1/easypage/errors.py` & `EasyPage-0.0.2/easypage/errors.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.1/easypage/logger.py` & `EasyPage-0.0.2/easypage/logger.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.1/easypage/main.py` & `EasyPage-0.0.2/easypage/main.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.1/easypage/operate.py` & `EasyPage-0.0.2/easypage/operate.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.1/easypage/options.py` & `EasyPage-0.0.2/easypage/options.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.1/easypage/settings.py` & `EasyPage-0.0.2/easypage/settings.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.1/easypage/utils/browser_utils.py` & `EasyPage-0.0.2/easypage/utils/browser_utils.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.1/easypage/utils/other_utils.py` & `EasyPage-0.0.2/easypage/utils/other_utils.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.1/setup.py` & `EasyPage-0.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name='EasyPage',
-    version='0.0.1',
+    version='0.0.2',
     author='leviathangk',
     author_email='1015295213@qq.com',
     description='基于 CDP 协议，简洁快速的浏览器控制 API',
     keywords=['EasyPage', 'page', 'browser'],
     packages=find_packages(),
     install_requires=[
         "lxml",
         "parsel",
         "requests",
         "loguru",
         "beautifulsoup4",
-        "websockets~=10.4",
-        "pyee~=10.0.2",
-        "websocket-client~=1.7.0",
+        "websockets",
+        "pyee",
+        "websocket-client",
     ],
 )
 
 """
     python setup.py sdist
     python -m twine upload dist/*
 """
```

