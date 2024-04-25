# Comparing `tmp/ctrip-app-ui-0.1.2.tar.gz` & `tmp/ctrip-app-ui-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.1.2.tar", last modified: Thu Apr 25 09:42:23 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.1.3.tar", last modified: Thu Apr 25 09:49:04 2024, max compression
```

## Comparing `ctrip-app-ui-0.1.2.tar` & `ctrip-app-ui-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 09:42:23.050298 ctrip-app-ui-0.1.2/
--rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      474 2024-04-25 09:42:23.048326 ctrip-app-ui-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 09:42:23.035363 ctrip-app-ui-0.1.2/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.1.2/capp_ui/__init__.py
--rw-rw-rw-   0        0        0     3028 2024-04-24 09:35:36.000000 ctrip-app-ui-0.1.2/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1191 2024-04-24 09:24:00.000000 ctrip-app-ui-0.1.2/capp_ui/device.py
--rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.1.2/capp_ui/dir.py
--rw-rw-rw-   0        0        0    52028 2024-04-25 09:42:10.000000 ctrip-app-ui-0.1.2/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.1.2/capp_ui/fee.py
--rw-rw-rw-   0        0        0     2270 2024-04-24 09:34:43.000000 ctrip-app-ui-0.1.2/capp_ui/libs.py
--rw-rw-rw-   0        0        0    23814 2024-04-25 08:28:03.000000 ctrip-app-ui-0.1.2/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1799 2024-04-24 09:24:12.000000 ctrip-app-ui-0.1.2/capp_ui/platforms.py
--rw-rw-rw-   0        0        0      689 2024-04-25 07:52:15.000000 ctrip-app-ui-0.1.2/capp_ui/test.py
--rw-rw-rw-   0        0        0     5563 2024-04-24 09:33:04.000000 ctrip-app-ui-0.1.2/capp_ui/utils.py
--rw-rw-rw-   0        0        0     2676 2024-04-24 15:31:32.000000 ctrip-app-ui-0.1.2/capp_ui/validators.py
-drwxrwxrwx   0        0        0        0 2024-04-25 09:42:23.047306 ctrip-app-ui-0.1.2/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-04-25 09:42:22.000000 ctrip-app-ui-0.1.2/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2024-04-25 09:42:22.000000 ctrip-app-ui-0.1.2/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 09:42:22.000000 ctrip-app-ui-0.1.2/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-25 09:42:22.000000 ctrip-app-ui-0.1.2/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-25 09:42:22.000000 ctrip-app-ui-0.1.2/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 09:42:23.050298 ctrip-app-ui-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-04-25 09:42:18.000000 ctrip-app-ui-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 09:49:04.373562 ctrip-app-ui-0.1.3/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-04-25 09:49:04.371574 ctrip-app-ui-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 09:49:04.360597 ctrip-app-ui-0.1.3/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.1.3/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0     3028 2024-04-24 09:35:36.000000 ctrip-app-ui-0.1.3/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1191 2024-04-24 09:24:00.000000 ctrip-app-ui-0.1.3/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.1.3/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    52549 2024-04-25 09:48:31.000000 ctrip-app-ui-0.1.3/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.1.3/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     2270 2024-04-24 09:34:43.000000 ctrip-app-ui-0.1.3/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    23814 2024-04-25 08:28:03.000000 ctrip-app-ui-0.1.3/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1799 2024-04-24 09:24:12.000000 ctrip-app-ui-0.1.3/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0      689 2024-04-25 07:52:15.000000 ctrip-app-ui-0.1.3/capp_ui/test.py
+-rw-rw-rw-   0        0        0     5563 2024-04-24 09:33:04.000000 ctrip-app-ui-0.1.3/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     2676 2024-04-24 15:31:32.000000 ctrip-app-ui-0.1.3/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-04-25 09:49:04.370570 ctrip-app-ui-0.1.3/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-04-25 09:49:04.000000 ctrip-app-ui-0.1.3/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2024-04-25 09:49:04.000000 ctrip-app-ui-0.1.3/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 09:49:04.000000 ctrip-app-ui-0.1.3/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-25 09:49:04.000000 ctrip-app-ui-0.1.3/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-25 09:49:04.000000 ctrip-app-ui-0.1.3/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 09:49:04.373562 ctrip-app-ui-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-04-25 09:49:00.000000 ctrip-app-ui-0.1.3/setup.py
```

### Comparing `ctrip-app-ui-0.1.2/LICENSE` & `ctrip-app-ui-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.2/capp_ui/date_extend.py` & `ctrip-app-ui-0.1.3/capp_ui/date_extend.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.2/capp_ui/device.py` & `ctrip-app-ui-0.1.3/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.2/capp_ui/dir.py` & `ctrip-app-ui-0.1.3/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.2/capp_ui/domain_service.py` & `ctrip-app-ui-0.1.3/capp_ui/domain_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,22 +122,35 @@
             else:
                 logger.warning("没有找到待付款按钮")
         except (PocoNoSuchNodeException, PocoTargetTimeout):
             pass
         except Exception as e:
             logger.error(e)
 
-    @SleepWait(wait_time=2)
-    def select_search_box(self, ctrip_order_id: str) -> None:
+    @SleepWait(wait_time=1)
+    def touch_list_page_search_box(self) -> None:
         """进入待付款列表页，点击【搜索框】"""
         try:
             search_box = self.device.poco(
                 type="android.widget.TextView", name="android.widget.TextView", text="搜索订单"
             )
             search_box.click()
+        except (PocoNoSuchNodeException, PocoTargetTimeout):
+            pass
+        except Exception as e:
+            logger.error(e)
+
+    @SleepWait(wait_time=1)
+    def touch_search_page_search_box(self, ctrip_order_id: str) -> None:
+        """进入搜索页，点击【搜索框】"""
+        try:
+            search_box = self.device.poco(
+                type="android.widget.TextView", name="android.widget.TextView", text="输入城市名/订单号 搜索订单"
+            )
+            search_box.click()
             search_box.set_text(ctrip_order_id)
             # 模拟键盘按下回车键（keyCode为66表示回车键）
             self.device.poco.device.input(keyevent="66")
         except (PocoNoSuchNodeException, PocoTargetTimeout):
             pass
         except Exception as e:
             logger.error(e)
```

### Comparing `ctrip-app-ui-0.1.2/capp_ui/fee.py` & `ctrip-app-ui-0.1.3/capp_ui/fee.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.2/capp_ui/libs.py` & `ctrip-app-ui-0.1.3/capp_ui/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.2/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.1.3/capp_ui/mobile_terminals.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.2/capp_ui/platforms.py` & `ctrip-app-ui-0.1.3/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.2/capp_ui/test.py` & `ctrip-app-ui-0.1.3/capp_ui/test.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.2/capp_ui/utils.py` & `ctrip-app-ui-0.1.3/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.2/capp_ui/validators.py` & `ctrip-app-ui-0.1.3/capp_ui/validators.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.2/setup.py` & `ctrip-app-ui-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.1.2',
+    version='0.1.3',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```

