# Comparing `tmp/ctrip-app-ui-0.0.3.tar.gz` & `tmp/ctrip-app-ui-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.0.3.tar", last modified: Wed Apr 24 15:32:07 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.0.4.tar", last modified: Wed Apr 24 16:04:28 2024, max compression
```

## Comparing `ctrip-app-ui-0.0.3.tar` & `ctrip-app-ui-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 15:32:07.378896 ctrip-app-ui-0.0.3/
--rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      474 2024-04-24 15:32:07.376898 ctrip-app-ui-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 15:32:07.363960 ctrip-app-ui-0.0.3/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.0.3/capp_ui/__init__.py
--rw-rw-rw-   0        0        0     3028 2024-04-24 09:35:36.000000 ctrip-app-ui-0.0.3/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1191 2024-04-24 09:24:00.000000 ctrip-app-ui-0.0.3/capp_ui/device.py
--rw-rw-rw-   0        0        0     1263 2024-04-24 09:31:47.000000 ctrip-app-ui-0.0.3/capp_ui/dir.py
--rw-rw-rw-   0        0        0    49360 2024-04-24 10:21:33.000000 ctrip-app-ui-0.0.3/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.0.3/capp_ui/fee.py
--rw-rw-rw-   0        0        0     2270 2024-04-24 09:34:43.000000 ctrip-app-ui-0.0.3/capp_ui/libs.py
--rw-rw-rw-   0        0        0    23814 2024-04-24 09:32:32.000000 ctrip-app-ui-0.0.3/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1799 2024-04-24 09:24:12.000000 ctrip-app-ui-0.0.3/capp_ui/platforms.py
--rw-rw-rw-   0        0        0     5563 2024-04-24 09:33:04.000000 ctrip-app-ui-0.0.3/capp_ui/utils.py
--rw-rw-rw-   0        0        0     2676 2024-04-24 15:31:32.000000 ctrip-app-ui-0.0.3/capp_ui/validators.py
-drwxrwxrwx   0        0        0        0 2024-04-24 15:32:07.374905 ctrip-app-ui-0.0.3/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-04-24 15:32:07.000000 ctrip-app-ui-0.0.3/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      426 2024-04-24 15:32:07.000000 ctrip-app-ui-0.0.3/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 15:32:07.000000 ctrip-app-ui-0.0.3/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-24 15:32:07.000000 ctrip-app-ui-0.0.3/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-24 15:32:07.000000 ctrip-app-ui-0.0.3/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 15:32:07.378896 ctrip-app-ui-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-04-24 15:31:59.000000 ctrip-app-ui-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:04:28.910132 ctrip-app-ui-0.0.4/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-04-24 16:04:28.908151 ctrip-app-ui-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 16:04:28.898164 ctrip-app-ui-0.0.4/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.0.4/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0     3028 2024-04-24 09:35:36.000000 ctrip-app-ui-0.0.4/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1191 2024-04-24 09:24:00.000000 ctrip-app-ui-0.0.4/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1263 2024-04-24 09:31:47.000000 ctrip-app-ui-0.0.4/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    50132 2024-04-24 16:03:46.000000 ctrip-app-ui-0.0.4/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.0.4/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     2270 2024-04-24 09:34:43.000000 ctrip-app-ui-0.0.4/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    23814 2024-04-24 09:32:32.000000 ctrip-app-ui-0.0.4/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1799 2024-04-24 09:24:12.000000 ctrip-app-ui-0.0.4/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0     5563 2024-04-24 09:33:04.000000 ctrip-app-ui-0.0.4/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     2676 2024-04-24 15:31:32.000000 ctrip-app-ui-0.0.4/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:04:28.907149 ctrip-app-ui-0.0.4/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-04-24 16:04:28.000000 ctrip-app-ui-0.0.4/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      426 2024-04-24 16:04:28.000000 ctrip-app-ui-0.0.4/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 16:04:28.000000 ctrip-app-ui-0.0.4/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-24 16:04:28.000000 ctrip-app-ui-0.0.4/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-24 16:04:28.000000 ctrip-app-ui-0.0.4/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 16:04:28.910132 ctrip-app-ui-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-04-24 16:04:25.000000 ctrip-app-ui-0.0.4/setup.py
```

### Comparing `ctrip-app-ui-0.0.3/LICENSE` & `ctrip-app-ui-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.3/capp_ui/date_extend.py` & `ctrip-app-ui-0.0.4/capp_ui/date_extend.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.3/capp_ui/device.py` & `ctrip-app-ui-0.0.4/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.3/capp_ui/dir.py` & `ctrip-app-ui-0.0.4/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.3/capp_ui/domain_service.py` & `ctrip-app-ui-0.0.4/capp_ui/domain_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # Description:  TODO
 # Author:       mfkifhss2023
 # CreateDate:   2024/04/24
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 import re
+import time
 import typing as t
 from decimal import Decimal
 from poco.proxy import UIObjectProxy
 from poco.exceptions import PocoNoSuchNodeException
 
 from capp_ui.platforms import PlatformService
 from capp_ui.mobile_terminals import stop_app
@@ -67,14 +68,33 @@
 
     @SleepWait(wait_time=1)
     def touch_my(self) -> None:
         """进入app后，点击【我的】"""
         my_button = self.device.poco(type="android.view.ViewGroup", name="ctrip.android.view:id/a", desc="我的")
         my_button.click()
 
+    @SleepWait(wait_time=1)
+    def touch_settings(self):
+        """我的主页，点击【设置】"""
+        setting_button = self.device.poco(type="android.widget.ImageView", name="ctrip.android.view:id/a", desc="设置")
+        setting_button.click()
+
+    @SleepWait(wait_time=1)
+    def touch_logout_user(self):
+        """在设置界面，点击【退出登录】"""
+        self.device.quick_slide_screen(duration=1)
+        try:
+            logout_user = self.device.poco(
+                type="android.widget.Button", name="ctrip.android.view:id/a", text="退出登录"
+            )
+            if logout_user.exists() is True:
+                logout_user.click()
+        except (PocoNoSuchNodeException,):
+            pass
+
     @SleepWait(wait_time=2)
     def touch_unpaid(self) -> None:
         """进入my主页后，点击【待付款】"""
         unpaid_button = self.device.poco(type="android.widget.TextView", name="ctrip.android.view:id/a", text="待付款")
         unpaid_button.click()
 
     @SleepWait(wait_time=2)
```

### Comparing `ctrip-app-ui-0.0.3/capp_ui/fee.py` & `ctrip-app-ui-0.0.4/capp_ui/fee.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.3/capp_ui/libs.py` & `ctrip-app-ui-0.0.4/capp_ui/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.3/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.0.4/capp_ui/mobile_terminals.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.3/capp_ui/platforms.py` & `ctrip-app-ui-0.0.4/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.3/capp_ui/utils.py` & `ctrip-app-ui-0.0.4/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.3/capp_ui/validators.py` & `ctrip-app-ui-0.0.4/capp_ui/validators.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.3/setup.py` & `ctrip-app-ui-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.0.3',
+    version='0.0.4',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```

