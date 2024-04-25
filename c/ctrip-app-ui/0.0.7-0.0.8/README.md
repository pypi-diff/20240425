# Comparing `tmp/ctrip-app-ui-0.0.7.tar.gz` & `tmp/ctrip-app-ui-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.0.7.tar", last modified: Thu Apr 25 08:03:11 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.0.8.tar", last modified: Thu Apr 25 08:28:42 2024, max compression
```

## Comparing `ctrip-app-ui-0.0.7.tar` & `ctrip-app-ui-0.0.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 08:03:11.390630 ctrip-app-ui-0.0.7/
--rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      474 2024-04-25 08:03:11.389633 ctrip-app-ui-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 08:03:11.375697 ctrip-app-ui-0.0.7/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.0.7/capp_ui/__init__.py
--rw-rw-rw-   0        0        0     3028 2024-04-24 09:35:36.000000 ctrip-app-ui-0.0.7/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1191 2024-04-24 09:24:00.000000 ctrip-app-ui-0.0.7/capp_ui/device.py
--rw-rw-rw-   0        0        0     1263 2024-04-24 09:31:47.000000 ctrip-app-ui-0.0.7/capp_ui/dir.py
--rw-rw-rw-   0        0        0    50586 2024-04-25 08:02:54.000000 ctrip-app-ui-0.0.7/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.0.7/capp_ui/fee.py
--rw-rw-rw-   0        0        0     2270 2024-04-24 09:34:43.000000 ctrip-app-ui-0.0.7/capp_ui/libs.py
--rw-rw-rw-   0        0        0    23814 2024-04-24 09:32:32.000000 ctrip-app-ui-0.0.7/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1799 2024-04-24 09:24:12.000000 ctrip-app-ui-0.0.7/capp_ui/platforms.py
--rw-rw-rw-   0        0        0      689 2024-04-25 07:52:15.000000 ctrip-app-ui-0.0.7/capp_ui/test.py
--rw-rw-rw-   0        0        0     5563 2024-04-24 09:33:04.000000 ctrip-app-ui-0.0.7/capp_ui/utils.py
--rw-rw-rw-   0        0        0     2676 2024-04-24 15:31:32.000000 ctrip-app-ui-0.0.7/capp_ui/validators.py
-drwxrwxrwx   0        0        0        0 2024-04-25 08:03:11.387640 ctrip-app-ui-0.0.7/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-04-25 08:03:11.000000 ctrip-app-ui-0.0.7/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2024-04-25 08:03:11.000000 ctrip-app-ui-0.0.7/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 08:03:11.000000 ctrip-app-ui-0.0.7/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-25 08:03:11.000000 ctrip-app-ui-0.0.7/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-25 08:03:11.000000 ctrip-app-ui-0.0.7/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 08:03:11.391627 ctrip-app-ui-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-04-25 08:03:06.000000 ctrip-app-ui-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 08:28:42.733171 ctrip-app-ui-0.0.8/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-04-25 08:28:42.731176 ctrip-app-ui-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 08:28:42.718211 ctrip-app-ui-0.0.8/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.0.8/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0     3028 2024-04-24 09:35:36.000000 ctrip-app-ui-0.0.8/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1191 2024-04-24 09:24:00.000000 ctrip-app-ui-0.0.8/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.0.8/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    50586 2024-04-25 08:02:54.000000 ctrip-app-ui-0.0.8/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.0.8/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     2270 2024-04-24 09:34:43.000000 ctrip-app-ui-0.0.8/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    23814 2024-04-25 08:28:03.000000 ctrip-app-ui-0.0.8/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1799 2024-04-24 09:24:12.000000 ctrip-app-ui-0.0.8/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0      689 2024-04-25 07:52:15.000000 ctrip-app-ui-0.0.8/capp_ui/test.py
+-rw-rw-rw-   0        0        0     5563 2024-04-24 09:33:04.000000 ctrip-app-ui-0.0.8/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     2676 2024-04-24 15:31:32.000000 ctrip-app-ui-0.0.8/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-04-25 08:28:42.729182 ctrip-app-ui-0.0.8/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-04-25 08:28:42.000000 ctrip-app-ui-0.0.8/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2024-04-25 08:28:42.000000 ctrip-app-ui-0.0.8/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 08:28:42.000000 ctrip-app-ui-0.0.8/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-25 08:28:42.000000 ctrip-app-ui-0.0.8/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-25 08:28:42.000000 ctrip-app-ui-0.0.8/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 08:28:42.733171 ctrip-app-ui-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-04-25 08:28:38.000000 ctrip-app-ui-0.0.8/setup.py
```

### Comparing `ctrip-app-ui-0.0.7/LICENSE` & `ctrip-app-ui-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.7/capp_ui/date_extend.py` & `ctrip-app-ui-0.0.8/capp_ui/date_extend.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.7/capp_ui/device.py` & `ctrip-app-ui-0.0.8/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.7/capp_ui/dir.py` & `ctrip-app-ui-0.0.8/capp_ui/dir.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 import os
 import sys
 import typing as t
 
 
 def get_project_path():
     # 获取当前执行文件的绝对路径（兼容 Python 2 和 Python 3）
-    return os.path.abspath(sys.argv[0])
+    exec_file_path = os.path.abspath(sys.argv[0])
+    exec_file_path_slice = exec_file_path.split(os.path.sep)
+    return os.path.sep.join(exec_file_path_slice[:-1])
 
 
 def get_images_dir():
     return os.path.join(get_project_path(), "static", "images")
 
 
 def is_exists(file_name: t.LiteralString | str | bytes) -> bool:
```

### Comparing `ctrip-app-ui-0.0.7/capp_ui/domain_service.py` & `ctrip-app-ui-0.0.8/capp_ui/domain_service.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.7/capp_ui/fee.py` & `ctrip-app-ui-0.0.8/capp_ui/fee.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.7/capp_ui/libs.py` & `ctrip-app-ui-0.0.8/capp_ui/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.7/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.0.8/capp_ui/mobile_terminals.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.7/capp_ui/platforms.py` & `ctrip-app-ui-0.0.8/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.7/capp_ui/test.py` & `ctrip-app-ui-0.0.8/capp_ui/test.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.7/capp_ui/utils.py` & `ctrip-app-ui-0.0.8/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.7/capp_ui/validators.py` & `ctrip-app-ui-0.0.8/capp_ui/validators.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.7/setup.py` & `ctrip-app-ui-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.0.7',
+    version='0.0.8',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```

