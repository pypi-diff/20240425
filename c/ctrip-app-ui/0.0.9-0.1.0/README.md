# Comparing `tmp/ctrip-app-ui-0.0.9.tar.gz` & `tmp/ctrip-app-ui-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.0.9.tar", last modified: Thu Apr 25 08:44:39 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.1.0.tar", last modified: Thu Apr 25 08:55:28 2024, max compression
```

## Comparing `ctrip-app-ui-0.0.9.tar` & `ctrip-app-ui-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 08:44:39.123354 ctrip-app-ui-0.0.9/
--rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.0.9/LICENSE
--rw-rw-rw-   0        0        0      474 2024-04-25 08:44:39.122383 ctrip-app-ui-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 08:44:39.110388 ctrip-app-ui-0.0.9/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.0.9/capp_ui/__init__.py
--rw-rw-rw-   0        0        0     3028 2024-04-24 09:35:36.000000 ctrip-app-ui-0.0.9/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1191 2024-04-24 09:24:00.000000 ctrip-app-ui-0.0.9/capp_ui/device.py
--rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.0.9/capp_ui/dir.py
--rw-rw-rw-   0        0        0    51320 2024-04-25 08:44:24.000000 ctrip-app-ui-0.0.9/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.0.9/capp_ui/fee.py
--rw-rw-rw-   0        0        0     2270 2024-04-24 09:34:43.000000 ctrip-app-ui-0.0.9/capp_ui/libs.py
--rw-rw-rw-   0        0        0    23814 2024-04-25 08:28:03.000000 ctrip-app-ui-0.0.9/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1799 2024-04-24 09:24:12.000000 ctrip-app-ui-0.0.9/capp_ui/platforms.py
--rw-rw-rw-   0        0        0      689 2024-04-25 07:52:15.000000 ctrip-app-ui-0.0.9/capp_ui/test.py
--rw-rw-rw-   0        0        0     5563 2024-04-24 09:33:04.000000 ctrip-app-ui-0.0.9/capp_ui/utils.py
--rw-rw-rw-   0        0        0     2676 2024-04-24 15:31:32.000000 ctrip-app-ui-0.0.9/capp_ui/validators.py
-drwxrwxrwx   0        0        0        0 2024-04-25 08:44:39.121371 ctrip-app-ui-0.0.9/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-04-25 08:44:39.000000 ctrip-app-ui-0.0.9/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2024-04-25 08:44:39.000000 ctrip-app-ui-0.0.9/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 08:44:39.000000 ctrip-app-ui-0.0.9/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-25 08:44:39.000000 ctrip-app-ui-0.0.9/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-25 08:44:39.000000 ctrip-app-ui-0.0.9/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 08:44:39.124351 ctrip-app-ui-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-04-25 08:44:34.000000 ctrip-app-ui-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 08:55:28.797535 ctrip-app-ui-0.1.0/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-04-25 08:55:28.793575 ctrip-app-ui-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 08:55:28.619173 ctrip-app-ui-0.1.0/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.1.0/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0     3028 2024-04-24 09:35:36.000000 ctrip-app-ui-0.1.0/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1191 2024-04-24 09:24:00.000000 ctrip-app-ui-0.1.0/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.1.0/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    51378 2024-04-25 08:55:00.000000 ctrip-app-ui-0.1.0/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.1.0/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     2270 2024-04-24 09:34:43.000000 ctrip-app-ui-0.1.0/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    23814 2024-04-25 08:28:03.000000 ctrip-app-ui-0.1.0/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1799 2024-04-24 09:24:12.000000 ctrip-app-ui-0.1.0/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0      689 2024-04-25 07:52:15.000000 ctrip-app-ui-0.1.0/capp_ui/test.py
+-rw-rw-rw-   0        0        0     5563 2024-04-24 09:33:04.000000 ctrip-app-ui-0.1.0/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     2676 2024-04-24 15:31:32.000000 ctrip-app-ui-0.1.0/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-04-25 08:55:28.789555 ctrip-app-ui-0.1.0/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-04-25 08:55:28.000000 ctrip-app-ui-0.1.0/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2024-04-25 08:55:28.000000 ctrip-app-ui-0.1.0/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 08:55:28.000000 ctrip-app-ui-0.1.0/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-25 08:55:28.000000 ctrip-app-ui-0.1.0/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-25 08:55:28.000000 ctrip-app-ui-0.1.0/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 08:55:28.797535 ctrip-app-ui-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-04-25 08:55:20.000000 ctrip-app-ui-0.1.0/setup.py
```

### Comparing `ctrip-app-ui-0.0.9/LICENSE` & `ctrip-app-ui-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.9/capp_ui/date_extend.py` & `ctrip-app-ui-0.1.0/capp_ui/date_extend.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.9/capp_ui/device.py` & `ctrip-app-ui-0.1.0/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.9/capp_ui/dir.py` & `ctrip-app-ui-0.1.0/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.9/capp_ui/domain_service.py` & `ctrip-app-ui-0.1.0/capp_ui/domain_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -582,16 +582,17 @@
     def enter_password(self, password: str) -> None:
         """输入登录密码"""
         password_poco = self.device.get_po(
             type="android.widget.EditText", name="android.widget.EditText", text="登录密码"
         )
         # password_poco.click()
         password_poco.set_text(password)
-        file_name = join_path([get_images_dir(), "键盘隐藏.png"])
-        self.device.hide_keyword(file_name=file_name)
+        # file_name = join_path([get_images_dir(), "键盘隐藏.png"])
+        # self.device.hide_keyword(file_name=file_name)
+        self.device.quick_slide_screen(duration=0.5)
 
     def touch_login(self) -> None:
         """点击【登录】"""
         login_poco = self.device.get_po(type="android.widget.TextView", name="ctrip.android.view:id/a",
                                         text="登录")
         login_poco.click()
```

### Comparing `ctrip-app-ui-0.0.9/capp_ui/fee.py` & `ctrip-app-ui-0.1.0/capp_ui/fee.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.9/capp_ui/libs.py` & `ctrip-app-ui-0.1.0/capp_ui/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.9/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.1.0/capp_ui/mobile_terminals.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.9/capp_ui/platforms.py` & `ctrip-app-ui-0.1.0/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.9/capp_ui/test.py` & `ctrip-app-ui-0.1.0/capp_ui/test.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.9/capp_ui/utils.py` & `ctrip-app-ui-0.1.0/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.9/capp_ui/validators.py` & `ctrip-app-ui-0.1.0/capp_ui/validators.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.9/setup.py` & `ctrip-app-ui-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.0.9',
+    version='0.1.0',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```

