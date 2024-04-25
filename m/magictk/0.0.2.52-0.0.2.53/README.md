# Comparing `tmp/magictk-0.0.2.52.tar.gz` & `tmp/magictk-0.0.2.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magictk-0.0.2.52.tar", last modified: Thu Apr 25 14:52:07 2024, max compression
+gzip compressed data, was "magictk-0.0.2.53.tar", last modified: Thu Apr 25 14:57:36 2024, max compression
```

## Comparing `magictk-0.0.2.52.tar` & `magictk-0.0.2.53.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:52:07.503738 magictk-0.0.2.52/
--rw-r--r--   0 root         (0) root         (0)       47 2024-04-25 14:52:07.000000 magictk-0.0.2.52/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      595 2024-04-25 14:52:07.503738 magictk-0.0.2.52/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1376 2024-04-25 14:52:07.000000 magictk-0.0.2.52/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:52:07.503738 magictk-0.0.2.52/magictk/
--rw-r--r--   0 root         (0) root         (0)      411 2024-04-25 14:52:07.000000 magictk-0.0.2.52/magictk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9695 2024-04-25 14:52:07.000000 magictk-0.0.2.52/magictk/_window_ctl.py
--rw-r--r--   0 root         (0) root         (0)    13250 2024-04-25 14:52:07.000000 magictk-0.0.2.52/magictk/_window_size.py
--rw-r--r--   0 root         (0) root         (0)     3285 2024-04-25 14:52:07.000000 magictk-0.0.2.52/magictk/basicwindow.py
--rw-r--r--   0 root         (0) root         (0)    13554 2024-04-25 14:52:07.000000 magictk-0.0.2.52/magictk/button.py
--rw-r--r--   0 root         (0) root         (0)    11247 2024-04-25 14:52:07.000000 magictk-0.0.2.52/magictk/checkbox.py
--rw-r--r--   0 root         (0) root         (0)     1919 2024-04-25 14:52:07.000000 magictk-0.0.2.52/magictk/color_tmpl.py
--rw-r--r--   0 root         (0) root         (0)    12242 2024-04-25 14:52:07.000000 magictk-0.0.2.52/magictk/entry.py
--rw-r--r--   0 root         (0) root         (0)      578 2024-04-25 14:52:07.000000 magictk-0.0.2.52/magictk/fontconfig.py
--rw-r--r--   0 root         (0) root         (0)     3725 2024-04-25 14:52:07.000000 magictk-0.0.2.52/magictk/frame.py
--rw-r--r--   0 root         (0) root         (0)    15906 2024-04-25 14:52:07.000000 magictk-0.0.2.52/magictk/icon.ico
--rw-r--r--   0 root         (0) root         (0)       70 2024-04-25 14:52:07.000000 magictk-0.0.2.52/magictk/mtk.py
--rw-r--r--   0 root         (0) root         (0)      720 2024-04-25 14:52:07.000000 magictk-0.0.2.52/magictk/photoload.py
--rw-r--r--   0 root         (0) root         (0)     5995 2024-04-25 14:52:07.000000 magictk-0.0.2.52/magictk/progressbar.py
--rw-r--r--   0 root         (0) root         (0) 11073665 2024-04-25 14:52:07.000000 magictk-0.0.2.52/magictk/res.pickle
--rw-r--r--   0 root         (0) root         (0)     8106 2024-04-25 14:52:07.000000 magictk-0.0.2.52/magictk/scrollbar.py
--rw-r--r--   0 root         (0) root         (0)     6178 2024-04-25 14:52:07.000000 magictk-0.0.2.52/magictk/select.py
--rw-r--r--   0 root         (0) root         (0)    11076 2024-04-25 14:52:07.000000 magictk-0.0.2.52/magictk/submenu.py
--rw-r--r--   0 root         (0) root         (0)    10245 2024-04-25 14:52:07.000000 magictk-0.0.2.52/magictk/window.py
--rw-r--r--   0 root         (0) root         (0)     2647 2024-04-25 14:52:07.000000 magictk-0.0.2.52/magictk/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:52:07.503738 magictk-0.0.2.52/magictk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      595 2024-04-25 14:52:07.000000 magictk-0.0.2.52/magictk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      592 2024-04-25 14:52:07.000000 magictk-0.0.2.52/magictk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 14:52:07.000000 magictk-0.0.2.52/magictk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-25 14:52:07.000000 magictk-0.0.2.52/magictk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 14:52:07.503738 magictk-0.0.2.52/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1127 2024-04-25 14:52:07.000000 magictk-0.0.2.52/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:57:36.375087 magictk-0.0.2.53/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-04-25 14:57:35.000000 magictk-0.0.2.53/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      595 2024-04-25 14:57:36.371087 magictk-0.0.2.53/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1376 2024-04-25 14:57:35.000000 magictk-0.0.2.53/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:57:36.371087 magictk-0.0.2.53/magictk/
+-rw-r--r--   0 root         (0) root         (0)      411 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9695 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/_window_ctl.py
+-rw-r--r--   0 root         (0) root         (0)    13250 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/_window_size.py
+-rw-r--r--   0 root         (0) root         (0)     3285 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/basicwindow.py
+-rw-r--r--   0 root         (0) root         (0)    13554 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/button.py
+-rw-r--r--   0 root         (0) root         (0)    11247 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/checkbox.py
+-rw-r--r--   0 root         (0) root         (0)     1919 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/color_tmpl.py
+-rw-r--r--   0 root         (0) root         (0)    12242 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/entry.py
+-rw-r--r--   0 root         (0) root         (0)      578 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/fontconfig.py
+-rw-r--r--   0 root         (0) root         (0)     3725 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/frame.py
+-rw-r--r--   0 root         (0) root         (0)    15906 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/icon.ico
+-rw-r--r--   0 root         (0) root         (0)       70 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/mtk.py
+-rw-r--r--   0 root         (0) root         (0)      720 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/photoload.py
+-rw-r--r--   0 root         (0) root         (0)     5995 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/progressbar.py
+-rw-r--r--   0 root         (0) root         (0) 11073665 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/res.pickle
+-rw-r--r--   0 root         (0) root         (0)     8106 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/scrollbar.py
+-rw-r--r--   0 root         (0) root         (0)     6178 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/select.py
+-rw-r--r--   0 root         (0) root         (0)    11076 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/submenu.py
+-rw-r--r--   0 root         (0) root         (0)    10245 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/window.py
+-rw-r--r--   0 root         (0) root         (0)     2647 2024-04-25 14:57:35.000000 magictk-0.0.2.53/magictk/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:57:36.371087 magictk-0.0.2.53/magictk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      595 2024-04-25 14:57:36.000000 magictk-0.0.2.53/magictk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      592 2024-04-25 14:57:36.000000 magictk-0.0.2.53/magictk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 14:57:36.000000 magictk-0.0.2.53/magictk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-25 14:57:36.000000 magictk-0.0.2.53/magictk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 14:57:36.375087 magictk-0.0.2.53/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1127 2024-04-25 14:57:35.000000 magictk-0.0.2.53/setup.py
```

### Comparing `magictk-0.0.2.52/PKG-INFO` & `magictk-0.0.2.53/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: magictk
-Version: 0.0.2.52
+Version: 0.0.2.53
 Summary: A tkinter weights looks like element-plus
 Home-page: http://git.hmtsai.cn/cxykevin/magictk.git
 Author: cxykevin|git.hmtsai.cn
 Author-email: cxykevin@yeah.net
 License: GPLv2
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `magictk-0.0.2.52/README.md` & `magictk-0.0.2.53/README.md`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.52/magictk/_window_ctl.py` & `magictk-0.0.2.53/magictk/_window_ctl.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.52/magictk/_window_size.py` & `magictk-0.0.2.53/magictk/_window_size.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.52/magictk/basicwindow.py` & `magictk-0.0.2.53/magictk/basicwindow.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.52/magictk/button.py` & `magictk-0.0.2.53/magictk/button.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.52/magictk/checkbox.py` & `magictk-0.0.2.53/magictk/checkbox.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.52/magictk/color_tmpl.py` & `magictk-0.0.2.53/magictk/color_tmpl.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.52/magictk/entry.py` & `magictk-0.0.2.53/magictk/entry.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.52/magictk/fontconfig.py` & `magictk-0.0.2.53/magictk/fontconfig.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.52/magictk/frame.py` & `magictk-0.0.2.53/magictk/frame.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.52/magictk/icon.ico` & `magictk-0.0.2.53/magictk/icon.ico`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.52/magictk/photoload.py` & `magictk-0.0.2.53/magictk/photoload.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.52/magictk/progressbar.py` & `magictk-0.0.2.53/magictk/progressbar.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.52/magictk/res.pickle` & `magictk-0.0.2.53/magictk/res.pickle`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.52/magictk/scrollbar.py` & `magictk-0.0.2.53/magictk/scrollbar.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.52/magictk/select.py` & `magictk-0.0.2.53/magictk/select.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.52/magictk/submenu.py` & `magictk-0.0.2.53/magictk/submenu.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.52/magictk/window.py` & `magictk-0.0.2.53/magictk/window.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.52/magictk/workspace.py` & `magictk-0.0.2.53/magictk/workspace.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.52/magictk.egg-info/PKG-INFO` & `magictk-0.0.2.53/magictk.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: magictk
-Version: 0.0.2.52
+Version: 0.0.2.53
 Summary: A tkinter weights looks like element-plus
 Home-page: http://git.hmtsai.cn/cxykevin/magictk.git
 Author: cxykevin|git.hmtsai.cn
 Author-email: cxykevin@yeah.net
 License: GPLv2
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `magictk-0.0.2.52/magictk.egg-info/SOURCES.txt` & `magictk-0.0.2.53/magictk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.52/setup.py` & `magictk-0.0.2.53/setup.py`

 * *Files identical despite different names*

