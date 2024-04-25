# Comparing `tmp/ecodev_front-0.0.8.tar.gz` & `tmp/ecodev_front-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecodev_front-0.0.8.tar", max compression
+gzip compressed data, was "ecodev_front-0.0.9.tar", max compression
```

## Comparing `ecodev_front-0.0.8.tar` & `ecodev_front-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rwxr-xr-x   0        0        0      247 2024-02-07 12:48:51.946855 ecodev_front-0.0.8/README.md
--rwxr-xr-x   0        0        0     1518 2024-02-07 13:05:14.677408 ecodev_front-0.0.8/ecodev_front/__init__.py
--rwxr-xr-x   0        0        0     1470 2024-02-07 12:48:51.946855 ecodev_front-0.0.8/ecodev_front/card.py
--rwxr-xr-x   0        0        0       46 2024-02-07 12:48:51.946855 ecodev_front-0.0.8/ecodev_front/component_ids.py
--rwxr-xr-x   0        0        0     2486 2024-02-07 12:48:51.946855 ecodev_front-0.0.8/ecodev_front/data_table.py
--rw-r--r--   0        0        0      409 2024-02-07 12:48:51.946855 ecodev_front-0.0.8/ecodev_front/display_utils.py
--rw-r--r--   0        0        0      570 2024-02-07 12:48:51.946855 ecodev_front-0.0.8/ecodev_front/footer.py
--rw-r--r--   0        0        0      428 2024-02-07 12:48:51.946855 ecodev_front-0.0.8/ecodev_front/graph.py
--rw-r--r--   0        0        0     3375 2024-02-07 12:48:51.950855 ecodev_front-0.0.8/ecodev_front/nav_items.py
--rw-r--r--   0        0        0     1302 2024-02-07 12:48:51.950855 ecodev_front-0.0.8/ecodev_front/navbar_header.py
--rw-r--r--   0        0        0     1417 2024-02-07 12:48:51.950855 ecodev_front-0.0.8/ecodev_front/navbar_login.py
--rw-r--r--   0        0        0      703 2024-02-07 12:48:51.950855 ecodev_front-0.0.8/ecodev_front/report_value.py
--rw-r--r--   0        0        0     1258 2024-02-07 12:48:51.950855 ecodev_front-0.0.8/ecodev_front/search_bar.py
--rw-r--r--   0        0        0     1077 2024-02-07 12:48:51.950855 ecodev_front-0.0.8/ecodev_front/upload_box.py
--rw-r--r--   0        0        0     1652 2024-02-07 13:05:27.573388 ecodev_front-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1743 1970-01-01 00:00:00.000000 ecodev_front-0.0.8/PKG-INFO
+-rwxr-xr-x   0        0        0      247 2024-02-07 12:48:51.946855 ecodev_front-0.0.9/README.md
+-rwxr-xr-x   0        0        0     1584 2024-02-07 13:09:57.016976 ecodev_front-0.0.9/ecodev_front/__init__.py
+-rwxr-xr-x   0        0        0     1470 2024-02-07 12:48:51.946855 ecodev_front-0.0.9/ecodev_front/card.py
+-rwxr-xr-x   0        0        0       46 2024-02-07 12:48:51.946855 ecodev_front-0.0.9/ecodev_front/component_ids.py
+-rwxr-xr-x   0        0        0     2486 2024-02-07 12:48:51.946855 ecodev_front-0.0.9/ecodev_front/data_table.py
+-rw-r--r--   0        0        0      409 2024-02-07 12:48:51.946855 ecodev_front-0.0.9/ecodev_front/display_utils.py
+-rw-r--r--   0        0        0      570 2024-02-07 12:48:51.946855 ecodev_front-0.0.9/ecodev_front/footer.py
+-rw-r--r--   0        0        0      428 2024-02-07 12:48:51.946855 ecodev_front-0.0.9/ecodev_front/graph.py
+-rw-r--r--   0        0        0     3375 2024-02-07 12:48:51.950855 ecodev_front-0.0.9/ecodev_front/nav_items.py
+-rw-r--r--   0        0        0     1302 2024-02-07 12:48:51.950855 ecodev_front-0.0.9/ecodev_front/navbar_header.py
+-rw-r--r--   0        0        0     1417 2024-02-07 12:48:51.950855 ecodev_front-0.0.9/ecodev_front/navbar_login.py
+-rw-r--r--   0        0        0      703 2024-02-07 12:48:51.950855 ecodev_front-0.0.9/ecodev_front/report_value.py
+-rw-r--r--   0        0        0     1258 2024-02-07 12:48:51.950855 ecodev_front-0.0.9/ecodev_front/search_bar.py
+-rw-r--r--   0        0        0     1077 2024-02-07 12:48:51.950855 ecodev_front-0.0.9/ecodev_front/upload_box.py
+-rw-r--r--   0        0        0     1652 2024-02-07 13:11:38.524820 ecodev_front-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1743 1970-01-01 00:00:00.000000 ecodev_front-0.0.9/PKG-INFO
```

### Comparing `ecodev_front-0.0.8/ecodev_front/__init__.py` & `ecodev_front-0.0.9/ecodev_front/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,14 @@
 from ecodev_front.navbar_header import navbar_header
 from ecodev_front.navbar_login import LOGIN_BTN_ID
 from ecodev_front.navbar_login import LOGIN_PASSWORD_INPUT_ID
 from ecodev_front.navbar_login import LOGIN_USERNAME_INPUT_ID
 from ecodev_front.navbar_login import navbar_login
 from ecodev_front.search_bar import search_bar
 from ecodev_front.upload_box import upload_box
-
+from ecodev_front.report_value import report_value
 
 __all__ = ['app_logo', 'app_title', 'navbar_header', 'navbar_menu', 'data_table', 'navbar_divider',
            'navbar_action_item', 'navbar_login', 'navbar_menu_item', 'upload_box', 'card_section',
            'card_title', 'macro_info', 'number_formatting', 'background_card', 'search_bar',
            'graph_box', 'LOGIN_USERNAME_INPUT_ID', 'LOGIN_PASSWORD_INPUT_ID', 'LOGIN_BTN_ID',
-           'footer_style']
+           'footer_style', 'report_value']
```

### Comparing `ecodev_front-0.0.8/ecodev_front/card.py` & `ecodev_front-0.0.9/ecodev_front/card.py`

 * *Files identical despite different names*

### Comparing `ecodev_front-0.0.8/ecodev_front/data_table.py` & `ecodev_front-0.0.9/ecodev_front/data_table.py`

 * *Files identical despite different names*

### Comparing `ecodev_front-0.0.8/ecodev_front/footer.py` & `ecodev_front-0.0.9/ecodev_front/footer.py`

 * *Files identical despite different names*

### Comparing `ecodev_front-0.0.8/ecodev_front/nav_items.py` & `ecodev_front-0.0.9/ecodev_front/nav_items.py`

 * *Files identical despite different names*

### Comparing `ecodev_front-0.0.8/ecodev_front/navbar_header.py` & `ecodev_front-0.0.9/ecodev_front/navbar_header.py`

 * *Files identical despite different names*

### Comparing `ecodev_front-0.0.8/ecodev_front/navbar_login.py` & `ecodev_front-0.0.9/ecodev_front/navbar_login.py`

 * *Files identical despite different names*

### Comparing `ecodev_front-0.0.8/ecodev_front/report_value.py` & `ecodev_front-0.0.9/ecodev_front/report_value.py`

 * *Files identical despite different names*

### Comparing `ecodev_front-0.0.8/ecodev_front/search_bar.py` & `ecodev_front-0.0.9/ecodev_front/search_bar.py`

 * *Files identical despite different names*

### Comparing `ecodev_front-0.0.8/ecodev_front/upload_box.py` & `ecodev_front-0.0.9/ecodev_front/upload_box.py`

 * *Files identical despite different names*

### Comparing `ecodev_front-0.0.8/pyproject.toml` & `ecodev_front-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ecodev-front"
-version = "0.0.8"
+version = "0.0.9"
 description = "Dash component helpers"
 authors = ["Amaury Salles <amaury.salles@gmail.com>",
 					 "Yoann Diep <yoann.diep@hotmail.fr>",
                         "Thomas Epelbaum <tomepel@gmail.com>",
 					 "Olivier Gabriel <olivier.gabriel.geom@gmail.com>",
 					 "Dorian Kodelja <dorian.kodelja@gmail.com>",
 ]
```

### Comparing `ecodev_front-0.0.8/PKG-INFO` & `ecodev_front-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecodev-front
-Version: 0.0.8
+Version: 0.0.9
 Summary: Dash component helpers
 License: MIT
 Author: Amaury Salles
 Author-email: amaury.salles@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Web Environment
```

