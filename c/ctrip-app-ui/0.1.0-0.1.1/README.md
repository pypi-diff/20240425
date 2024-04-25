# Comparing `tmp/ctrip-app-ui-0.1.0.tar.gz` & `tmp/ctrip-app-ui-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.1.0.tar", last modified: Thu Apr 25 08:55:28 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.1.1.tar", last modified: Thu Apr 25 09:10:37 2024, max compression
```

## Comparing `ctrip-app-ui-0.1.0.tar` & `ctrip-app-ui-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 08:55:28.797535 ctrip-app-ui-0.1.0/
--rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      474 2024-04-25 08:55:28.793575 ctrip-app-ui-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 08:55:28.619173 ctrip-app-ui-0.1.0/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.1.0/capp_ui/__init__.py
--rw-rw-rw-   0        0        0     3028 2024-04-24 09:35:36.000000 ctrip-app-ui-0.1.0/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1191 2024-04-24 09:24:00.000000 ctrip-app-ui-0.1.0/capp_ui/device.py
--rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.1.0/capp_ui/dir.py
--rw-rw-rw-   0        0        0    51378 2024-04-25 08:55:00.000000 ctrip-app-ui-0.1.0/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.1.0/capp_ui/fee.py
--rw-rw-rw-   0        0        0     2270 2024-04-24 09:34:43.000000 ctrip-app-ui-0.1.0/capp_ui/libs.py
--rw-rw-rw-   0        0        0    23814 2024-04-25 08:28:03.000000 ctrip-app-ui-0.1.0/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1799 2024-04-24 09:24:12.000000 ctrip-app-ui-0.1.0/capp_ui/platforms.py
--rw-rw-rw-   0        0        0      689 2024-04-25 07:52:15.000000 ctrip-app-ui-0.1.0/capp_ui/test.py
--rw-rw-rw-   0        0        0     5563 2024-04-24 09:33:04.000000 ctrip-app-ui-0.1.0/capp_ui/utils.py
--rw-rw-rw-   0        0        0     2676 2024-04-24 15:31:32.000000 ctrip-app-ui-0.1.0/capp_ui/validators.py
-drwxrwxrwx   0        0        0        0 2024-04-25 08:55:28.789555 ctrip-app-ui-0.1.0/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-04-25 08:55:28.000000 ctrip-app-ui-0.1.0/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2024-04-25 08:55:28.000000 ctrip-app-ui-0.1.0/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 08:55:28.000000 ctrip-app-ui-0.1.0/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-25 08:55:28.000000 ctrip-app-ui-0.1.0/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-25 08:55:28.000000 ctrip-app-ui-0.1.0/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 08:55:28.797535 ctrip-app-ui-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-04-25 08:55:20.000000 ctrip-app-ui-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 09:10:37.665890 ctrip-app-ui-0.1.1/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-04-25 09:10:37.663891 ctrip-app-ui-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 09:10:37.651922 ctrip-app-ui-0.1.1/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.1.1/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0     3028 2024-04-24 09:35:36.000000 ctrip-app-ui-0.1.1/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1191 2024-04-24 09:24:00.000000 ctrip-app-ui-0.1.1/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.1.1/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    51821 2024-04-25 09:10:07.000000 ctrip-app-ui-0.1.1/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.1.1/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     2270 2024-04-24 09:34:43.000000 ctrip-app-ui-0.1.1/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    23814 2024-04-25 08:28:03.000000 ctrip-app-ui-0.1.1/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1799 2024-04-24 09:24:12.000000 ctrip-app-ui-0.1.1/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0      689 2024-04-25 07:52:15.000000 ctrip-app-ui-0.1.1/capp_ui/test.py
+-rw-rw-rw-   0        0        0     5563 2024-04-24 09:33:04.000000 ctrip-app-ui-0.1.1/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     2676 2024-04-24 15:31:32.000000 ctrip-app-ui-0.1.1/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-04-25 09:10:37.662924 ctrip-app-ui-0.1.1/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-04-25 09:10:37.000000 ctrip-app-ui-0.1.1/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2024-04-25 09:10:37.000000 ctrip-app-ui-0.1.1/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 09:10:37.000000 ctrip-app-ui-0.1.1/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-25 09:10:37.000000 ctrip-app-ui-0.1.1/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-25 09:10:37.000000 ctrip-app-ui-0.1.1/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 09:10:37.665890 ctrip-app-ui-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-04-25 09:10:33.000000 ctrip-app-ui-0.1.1/setup.py
```

### Comparing `ctrip-app-ui-0.1.0/LICENSE` & `ctrip-app-ui-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.0/capp_ui/date_extend.py` & `ctrip-app-ui-0.1.1/capp_ui/date_extend.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.0/capp_ui/device.py` & `ctrip-app-ui-0.1.1/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.0/capp_ui/dir.py` & `ctrip-app-ui-0.1.1/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.0/capp_ui/domain_service.py` & `ctrip-app-ui-0.1.1/capp_ui/domain_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -542,22 +542,31 @@
             touchable=False,
         )[0]
         ordinary_booking_button.click()
 
     def is_need_login(self) -> bool:
         flag = False
         try:
-            login = self.device.get_po(
+            login_page = self.device.get_po(
                 type="android.widget.TextView", name="ctrip.android.view:id/a", text="手机验证码登录"
             )
-            if login.exists() is True:
+            my_login = self.device.get_po(
+                type="android.widget.Button", name="ctrip.android.view:id/a", text="登录/注册"
+            )
+            if login_page.exists() is True:
+                logger.warning("手机app已经跳转至登录界面，需要做登录操作.")
+                flag = True
+            elif my_login.exists() is True:
+                my_login.click()
                 logger.warning("手机app已经跳转至登录界面，需要做登录操作.")
                 flag = True
-        except (PocoNoSuchNodeException, Exception):
+        except (PocoNoSuchNodeException, PocoTargetTimeout):
             pass
+        except Exception as e:
+            logger.error(e)
         return flag
 
     def select_agree_service_agreement(self) -> None:
         """选择【同意服务协议】"""
         service_agreement = self.device.get_po(
             type="android.widget.ImageView", name="ctrip.android.view:id/a", desc="勾选服务协议和个人信息保护指引"
         )
```

### Comparing `ctrip-app-ui-0.1.0/capp_ui/fee.py` & `ctrip-app-ui-0.1.1/capp_ui/fee.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.0/capp_ui/libs.py` & `ctrip-app-ui-0.1.1/capp_ui/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.0/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.1.1/capp_ui/mobile_terminals.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.0/capp_ui/platforms.py` & `ctrip-app-ui-0.1.1/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.0/capp_ui/test.py` & `ctrip-app-ui-0.1.1/capp_ui/test.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.0/capp_ui/utils.py` & `ctrip-app-ui-0.1.1/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.0/capp_ui/validators.py` & `ctrip-app-ui-0.1.1/capp_ui/validators.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.0/setup.py` & `ctrip-app-ui-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.1.0',
+    version='0.1.1',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```

