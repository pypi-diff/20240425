# Comparing `tmp/magictk-0.0.2.50.tar.gz` & `tmp/magictk-0.0.2.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magictk-0.0.2.50.tar", last modified: Wed Apr 24 14:19:16 2024, max compression
+gzip compressed data, was "magictk-0.0.2.51.tar", last modified: Thu Apr 25 14:25:44 2024, max compression
```

## Comparing `magictk-0.0.2.50.tar` & `magictk-0.0.2.51.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:19:16.865636 magictk-0.0.2.50/
--rw-r--r--   0 root         (0) root         (0)       47 2024-04-24 14:19:16.000000 magictk-0.0.2.50/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      595 2024-04-24 14:19:16.865636 magictk-0.0.2.50/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1376 2024-04-24 14:19:16.000000 magictk-0.0.2.50/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:19:16.865636 magictk-0.0.2.50/magictk/
--rw-r--r--   0 root         (0) root         (0)      411 2024-04-24 14:19:16.000000 magictk-0.0.2.50/magictk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9695 2024-04-24 14:19:16.000000 magictk-0.0.2.50/magictk/_window_ctl.py
--rw-r--r--   0 root         (0) root         (0)    13250 2024-04-24 14:19:16.000000 magictk-0.0.2.50/magictk/_window_size.py
--rw-r--r--   0 root         (0) root         (0)     3285 2024-04-24 14:19:16.000000 magictk-0.0.2.50/magictk/basicwindow.py
--rw-r--r--   0 root         (0) root         (0)    13554 2024-04-24 14:19:16.000000 magictk-0.0.2.50/magictk/button.py
--rw-r--r--   0 root         (0) root         (0)    11247 2024-04-24 14:19:16.000000 magictk-0.0.2.50/magictk/checkbox.py
--rw-r--r--   0 root         (0) root         (0)     1919 2024-04-24 14:19:16.000000 magictk-0.0.2.50/magictk/color_tmpl.py
--rw-r--r--   0 root         (0) root         (0)    12242 2024-04-24 14:19:16.000000 magictk-0.0.2.50/magictk/entry.py
--rw-r--r--   0 root         (0) root         (0)      578 2024-04-24 14:19:16.000000 magictk-0.0.2.50/magictk/fontconfig.py
--rw-r--r--   0 root         (0) root         (0)     3725 2024-04-24 14:19:16.000000 magictk-0.0.2.50/magictk/frame.py
--rw-r--r--   0 root         (0) root         (0)    15906 2024-04-24 14:19:16.000000 magictk-0.0.2.50/magictk/icon.ico
--rw-r--r--   0 root         (0) root         (0)       70 2024-04-24 14:19:16.000000 magictk-0.0.2.50/magictk/mtk.py
--rw-r--r--   0 root         (0) root         (0)      720 2024-04-24 14:19:16.000000 magictk-0.0.2.50/magictk/photoload.py
--rw-r--r--   0 root         (0) root         (0)     5995 2024-04-24 14:19:16.000000 magictk-0.0.2.50/magictk/progressbar.py
--rw-r--r--   0 root         (0) root         (0)    22329 2024-04-24 14:19:16.000000 magictk-0.0.2.50/magictk/res.pickle
--rw-r--r--   0 root         (0) root         (0)     8106 2024-04-24 14:19:16.000000 magictk-0.0.2.50/magictk/scrollbar.py
--rw-r--r--   0 root         (0) root         (0)     6178 2024-04-24 14:19:16.000000 magictk-0.0.2.50/magictk/select.py
--rw-r--r--   0 root         (0) root         (0)    11076 2024-04-24 14:19:16.000000 magictk-0.0.2.50/magictk/submenu.py
--rw-r--r--   0 root         (0) root         (0)    10245 2024-04-24 14:19:16.000000 magictk-0.0.2.50/magictk/window.py
--rw-r--r--   0 root         (0) root         (0)     2647 2024-04-24 14:19:16.000000 magictk-0.0.2.50/magictk/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:19:16.865636 magictk-0.0.2.50/magictk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      595 2024-04-24 14:19:16.000000 magictk-0.0.2.50/magictk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      592 2024-04-24 14:19:16.000000 magictk-0.0.2.50/magictk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 14:19:16.000000 magictk-0.0.2.50/magictk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-24 14:19:16.000000 magictk-0.0.2.50/magictk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 14:19:16.865636 magictk-0.0.2.50/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1127 2024-04-24 14:19:16.000000 magictk-0.0.2.50/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:25:44.113128 magictk-0.0.2.51/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-04-25 14:25:43.000000 magictk-0.0.2.51/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      595 2024-04-25 14:25:44.113128 magictk-0.0.2.51/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1376 2024-04-25 14:25:43.000000 magictk-0.0.2.51/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:25:44.113128 magictk-0.0.2.51/magictk/
+-rw-r--r--   0 root         (0) root         (0)      411 2024-04-25 14:25:43.000000 magictk-0.0.2.51/magictk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9695 2024-04-25 14:25:43.000000 magictk-0.0.2.51/magictk/_window_ctl.py
+-rw-r--r--   0 root         (0) root         (0)    13250 2024-04-25 14:25:43.000000 magictk-0.0.2.51/magictk/_window_size.py
+-rw-r--r--   0 root         (0) root         (0)     3285 2024-04-25 14:25:43.000000 magictk-0.0.2.51/magictk/basicwindow.py
+-rw-r--r--   0 root         (0) root         (0)    13554 2024-04-25 14:25:43.000000 magictk-0.0.2.51/magictk/button.py
+-rw-r--r--   0 root         (0) root         (0)    11247 2024-04-25 14:25:43.000000 magictk-0.0.2.51/magictk/checkbox.py
+-rw-r--r--   0 root         (0) root         (0)     1919 2024-04-25 14:25:43.000000 magictk-0.0.2.51/magictk/color_tmpl.py
+-rw-r--r--   0 root         (0) root         (0)    12242 2024-04-25 14:25:43.000000 magictk-0.0.2.51/magictk/entry.py
+-rw-r--r--   0 root         (0) root         (0)      578 2024-04-25 14:25:43.000000 magictk-0.0.2.51/magictk/fontconfig.py
+-rw-r--r--   0 root         (0) root         (0)     3725 2024-04-25 14:25:43.000000 magictk-0.0.2.51/magictk/frame.py
+-rw-r--r--   0 root         (0) root         (0)    15906 2024-04-25 14:25:43.000000 magictk-0.0.2.51/magictk/icon.ico
+-rw-r--r--   0 root         (0) root         (0)       70 2024-04-25 14:25:43.000000 magictk-0.0.2.51/magictk/mtk.py
+-rw-r--r--   0 root         (0) root         (0)      720 2024-04-25 14:25:43.000000 magictk-0.0.2.51/magictk/photoload.py
+-rw-r--r--   0 root         (0) root         (0)     5995 2024-04-25 14:25:43.000000 magictk-0.0.2.51/magictk/progressbar.py
+-rw-r--r--   0 root         (0) root         (0) 11073665 2024-04-25 14:25:43.000000 magictk-0.0.2.51/magictk/res.pickle
+-rw-r--r--   0 root         (0) root         (0)     8106 2024-04-25 14:25:43.000000 magictk-0.0.2.51/magictk/scrollbar.py
+-rw-r--r--   0 root         (0) root         (0)     6178 2024-04-25 14:25:43.000000 magictk-0.0.2.51/magictk/select.py
+-rw-r--r--   0 root         (0) root         (0)    11076 2024-04-25 14:25:43.000000 magictk-0.0.2.51/magictk/submenu.py
+-rw-r--r--   0 root         (0) root         (0)    10245 2024-04-25 14:25:43.000000 magictk-0.0.2.51/magictk/window.py
+-rw-r--r--   0 root         (0) root         (0)     2647 2024-04-25 14:25:43.000000 magictk-0.0.2.51/magictk/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:25:44.113128 magictk-0.0.2.51/magictk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      595 2024-04-25 14:25:44.000000 magictk-0.0.2.51/magictk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      592 2024-04-25 14:25:44.000000 magictk-0.0.2.51/magictk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 14:25:44.000000 magictk-0.0.2.51/magictk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-25 14:25:44.000000 magictk-0.0.2.51/magictk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 14:25:44.113128 magictk-0.0.2.51/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1127 2024-04-25 14:25:43.000000 magictk-0.0.2.51/setup.py
```

### Comparing `magictk-0.0.2.50/PKG-INFO` & `magictk-0.0.2.51/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: magictk
-Version: 0.0.2.50
+Version: 0.0.2.51
 Summary: A tkinter weights looks like element-plus
 Home-page: http://git.hmtsai.cn/cxykevin/magictk.git
 Author: cxykevin|git.hmtsai.cn
 Author-email: cxykevin@yeah.net
 License: GPLv2
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `magictk-0.0.2.50/README.md` & `magictk-0.0.2.51/README.md`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.50/magictk/_window_ctl.py` & `magictk-0.0.2.51/magictk/_window_ctl.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.50/magictk/_window_size.py` & `magictk-0.0.2.51/magictk/_window_size.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.50/magictk/basicwindow.py` & `magictk-0.0.2.51/magictk/basicwindow.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.50/magictk/button.py` & `magictk-0.0.2.51/magictk/button.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.50/magictk/checkbox.py` & `magictk-0.0.2.51/magictk/checkbox.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.50/magictk/color_tmpl.py` & `magictk-0.0.2.51/magictk/color_tmpl.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.50/magictk/entry.py` & `magictk-0.0.2.51/magictk/entry.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.50/magictk/fontconfig.py` & `magictk-0.0.2.51/magictk/fontconfig.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.50/magictk/frame.py` & `magictk-0.0.2.51/magictk/frame.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.50/magictk/icon.ico` & `magictk-0.0.2.51/magictk/icon.ico`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.50/magictk/photoload.py` & `magictk-0.0.2.51/magictk/photoload.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.50/magictk/progressbar.py` & `magictk-0.0.2.51/magictk/progressbar.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.50/magictk/scrollbar.py` & `magictk-0.0.2.51/magictk/scrollbar.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.50/magictk/select.py` & `magictk-0.0.2.51/magictk/select.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.50/magictk/submenu.py` & `magictk-0.0.2.51/magictk/submenu.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.50/magictk/window.py` & `magictk-0.0.2.51/magictk/window.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.50/magictk/workspace.py` & `magictk-0.0.2.51/magictk/workspace.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.50/magictk.egg-info/PKG-INFO` & `magictk-0.0.2.51/magictk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: magictk
-Version: 0.0.2.50
+Version: 0.0.2.51
 Summary: A tkinter weights looks like element-plus
 Home-page: http://git.hmtsai.cn/cxykevin/magictk.git
 Author: cxykevin|git.hmtsai.cn
 Author-email: cxykevin@yeah.net
 License: GPLv2
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `magictk-0.0.2.50/magictk.egg-info/SOURCES.txt` & `magictk-0.0.2.51/magictk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.50/setup.py` & `magictk-0.0.2.51/setup.py`

 * *Files identical despite different names*

