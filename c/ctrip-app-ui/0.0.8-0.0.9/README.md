# Comparing `tmp/ctrip-app-ui-0.0.8.tar.gz` & `tmp/ctrip-app-ui-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.0.8.tar", last modified: Thu Apr 25 08:28:42 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.0.9.tar", last modified: Thu Apr 25 08:44:39 2024, max compression
```

## Comparing `ctrip-app-ui-0.0.8.tar` & `ctrip-app-ui-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 08:28:42.733171 ctrip-app-ui-0.0.8/
--rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      474 2024-04-25 08:28:42.731176 ctrip-app-ui-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 08:28:42.718211 ctrip-app-ui-0.0.8/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.0.8/capp_ui/__init__.py
--rw-rw-rw-   0        0        0     3028 2024-04-24 09:35:36.000000 ctrip-app-ui-0.0.8/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1191 2024-04-24 09:24:00.000000 ctrip-app-ui-0.0.8/capp_ui/device.py
--rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.0.8/capp_ui/dir.py
--rw-rw-rw-   0        0        0    50586 2024-04-25 08:02:54.000000 ctrip-app-ui-0.0.8/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.0.8/capp_ui/fee.py
--rw-rw-rw-   0        0        0     2270 2024-04-24 09:34:43.000000 ctrip-app-ui-0.0.8/capp_ui/libs.py
--rw-rw-rw-   0        0        0    23814 2024-04-25 08:28:03.000000 ctrip-app-ui-0.0.8/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1799 2024-04-24 09:24:12.000000 ctrip-app-ui-0.0.8/capp_ui/platforms.py
--rw-rw-rw-   0        0        0      689 2024-04-25 07:52:15.000000 ctrip-app-ui-0.0.8/capp_ui/test.py
--rw-rw-rw-   0        0        0     5563 2024-04-24 09:33:04.000000 ctrip-app-ui-0.0.8/capp_ui/utils.py
--rw-rw-rw-   0        0        0     2676 2024-04-24 15:31:32.000000 ctrip-app-ui-0.0.8/capp_ui/validators.py
-drwxrwxrwx   0        0        0        0 2024-04-25 08:28:42.729182 ctrip-app-ui-0.0.8/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-04-25 08:28:42.000000 ctrip-app-ui-0.0.8/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2024-04-25 08:28:42.000000 ctrip-app-ui-0.0.8/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 08:28:42.000000 ctrip-app-ui-0.0.8/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-25 08:28:42.000000 ctrip-app-ui-0.0.8/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-25 08:28:42.000000 ctrip-app-ui-0.0.8/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 08:28:42.733171 ctrip-app-ui-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-04-25 08:28:38.000000 ctrip-app-ui-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 08:44:39.123354 ctrip-app-ui-0.0.9/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-04-25 08:44:39.122383 ctrip-app-ui-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 08:44:39.110388 ctrip-app-ui-0.0.9/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.0.9/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0     3028 2024-04-24 09:35:36.000000 ctrip-app-ui-0.0.9/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1191 2024-04-24 09:24:00.000000 ctrip-app-ui-0.0.9/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.0.9/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    51320 2024-04-25 08:44:24.000000 ctrip-app-ui-0.0.9/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.0.9/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     2270 2024-04-24 09:34:43.000000 ctrip-app-ui-0.0.9/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    23814 2024-04-25 08:28:03.000000 ctrip-app-ui-0.0.9/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1799 2024-04-24 09:24:12.000000 ctrip-app-ui-0.0.9/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0      689 2024-04-25 07:52:15.000000 ctrip-app-ui-0.0.9/capp_ui/test.py
+-rw-rw-rw-   0        0        0     5563 2024-04-24 09:33:04.000000 ctrip-app-ui-0.0.9/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     2676 2024-04-24 15:31:32.000000 ctrip-app-ui-0.0.9/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-04-25 08:44:39.121371 ctrip-app-ui-0.0.9/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-04-25 08:44:39.000000 ctrip-app-ui-0.0.9/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2024-04-25 08:44:39.000000 ctrip-app-ui-0.0.9/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 08:44:39.000000 ctrip-app-ui-0.0.9/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-25 08:44:39.000000 ctrip-app-ui-0.0.9/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-25 08:44:39.000000 ctrip-app-ui-0.0.9/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 08:44:39.124351 ctrip-app-ui-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-04-25 08:44:34.000000 ctrip-app-ui-0.0.9/setup.py
```

### Comparing `ctrip-app-ui-0.0.8/LICENSE` & `ctrip-app-ui-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.8/capp_ui/date_extend.py` & `ctrip-app-ui-0.0.9/capp_ui/date_extend.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.8/capp_ui/device.py` & `ctrip-app-ui-0.0.9/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.8/capp_ui/dir.py` & `ctrip-app-ui-0.0.9/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.8/capp_ui/domain_service.py` & `ctrip-app-ui-0.0.9/capp_ui/domain_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # ---------------------------------------------------------------------------------------------------------
 """
 import re
 import time
 import typing as t
 from decimal import Decimal
 from poco.proxy import UIObjectProxy
-from poco.exceptions import PocoNoSuchNodeException
+from poco.exceptions import PocoNoSuchNodeException, PocoTargetTimeout
 
 from capp_ui.platforms import PlatformService
 from capp_ui.mobile_terminals import stop_app
 from capp_ui.libs import SleepWait, LoopFindElement
 from capp_ui.utils import logger, get_ui_object_proxy_attr
 from capp_ui.dir import get_images_dir, is_exists, join_path
 from capp_ui.date_extend import get_trip_year_month_day, get_datetime_area, is_public_holiday
@@ -102,16 +102,33 @@
                 logout_user.click()
         except (PocoNoSuchNodeException,):
             pass
 
     @SleepWait(wait_time=2)
     def touch_unpaid(self) -> None:
         """进入my主页后，点击【待付款】"""
-        unpaid_button = self.device.poco(type="android.widget.TextView", name="ctrip.android.view:id/a", text="待付款")
-        unpaid_button.click()
+        try:
+            # 登录后的待付款元素定位
+            login_unpaid_button = self.device.poco(
+                type="android.widget.TextView", name="ctrip.android.view:id/a", text="待付款"
+            )
+            # 未登录的待付款元素定位
+            logout_unpaid_button = self.device.poco(
+                type="android.widget.TextView", name="android.widget.TextView", text="待付款"
+            )
+            if login_unpaid_button.exists() is True:
+                login_unpaid_button.click()
+            elif logout_unpaid_button.exists() is True:
+                logout_unpaid_button.click()
+            else:
+                logger.warning("没有找到待付款按钮")
+        except (PocoNoSuchNodeException, PocoTargetTimeout):
+            pass
+        except Exception as e:
+            logger.error(e)
 
     @SleepWait(wait_time=2)
     def select_search_box(self, ctrip_order_id: str) -> None:
         """进入待付款列表页，点击【搜索框】"""
         search_box = self.device.poco(type="android.widget.TextView", name="ctrip.android.view:id/a", text="搜索订单")
         search_box.click()
         search_box.set_text(ctrip_order_id)
```

### Comparing `ctrip-app-ui-0.0.8/capp_ui/fee.py` & `ctrip-app-ui-0.0.9/capp_ui/fee.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.8/capp_ui/libs.py` & `ctrip-app-ui-0.0.9/capp_ui/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.8/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.0.9/capp_ui/mobile_terminals.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.8/capp_ui/platforms.py` & `ctrip-app-ui-0.0.9/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.8/capp_ui/test.py` & `ctrip-app-ui-0.0.9/capp_ui/test.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.8/capp_ui/utils.py` & `ctrip-app-ui-0.0.9/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.8/capp_ui/validators.py` & `ctrip-app-ui-0.0.9/capp_ui/validators.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.8/setup.py` & `ctrip-app-ui-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.0.8',
+    version='0.0.9',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```

