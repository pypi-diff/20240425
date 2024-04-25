# Comparing `tmp/tui_dsg-202404221312.tar.gz` & `tmp/tui_dsg-202404250955.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tui_dsg-202404221312.tar", last modified: Mon Apr 22 13:12:34 2024, max compression
+gzip compressed data, was "tui_dsg-202404250955.tar", last modified: Thu Apr 25 09:55:50 2024, max compression
```

## Comparing `tui_dsg-202404221312.tar` & `tui_dsg-202404250955.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:12:34.770393 tui_dsg-202404221312/
--rw-r--r--   0 root         (0) root         (0)     1188 2024-04-22 13:12:34.770393 tui_dsg-202404221312/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-22 13:12:34.770393 tui_dsg-202404221312/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1472 2024-04-20 12:08:44.000000 tui_dsg-202404221312/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:12:34.766393 tui_dsg-202404221312/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:12:34.766393 tui_dsg-202404221312/src/tui_dsg/
--rw-rw-rw-   0 root         (0) root         (0)        5 2024-03-28 13:23:09.000000 tui_dsg-202404221312/src/tui_dsg/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:12:34.770393 tui_dsg-202404221312/src/tui_dsg.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1188 2024-04-22 13:12:34.000000 tui_dsg-202404221312/src/tui_dsg.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      206 2024-04-22 13:12:34.000000 tui_dsg-202404221312/src/tui_dsg.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 13:12:34.000000 tui_dsg-202404221312/src/tui_dsg.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      348 2024-04-22 13:12:34.000000 tui_dsg-202404221312/src/tui_dsg.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-22 13:12:34.000000 tui_dsg-202404221312/src/tui_dsg.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 09:55:50.073029 tui_dsg-202404250955/
+-rw-r--r--   0 root         (0) root         (0)     1188 2024-04-25 09:55:50.073029 tui_dsg-202404250955/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 09:55:50.073029 tui_dsg-202404250955/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1472 2024-04-25 09:55:42.000000 tui_dsg-202404250955/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 09:55:50.073029 tui_dsg-202404250955/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 09:55:50.073029 tui_dsg-202404250955/src/tui_dsg/
+-rw-rw-rw-   0 root         (0) root         (0)        5 2024-04-25 09:55:42.000000 tui_dsg-202404250955/src/tui_dsg/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 09:55:50.073029 tui_dsg-202404250955/src/tui_dsg.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1188 2024-04-25 09:55:50.000000 tui_dsg-202404250955/src/tui_dsg.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      206 2024-04-25 09:55:50.000000 tui_dsg-202404250955/src/tui_dsg.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 09:55:50.000000 tui_dsg-202404250955/src/tui_dsg.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      348 2024-04-25 09:55:50.000000 tui_dsg-202404250955/src/tui_dsg.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-25 09:55:50.000000 tui_dsg-202404250955/src/tui_dsg.egg-info/top_level.txt
```

### Comparing `tui_dsg-202404221312/PKG-INFO` & `tui_dsg-202404250955/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tui_dsg
-Version: 202404221312
+Version: 202404250955
 Summary: everything you need for our jupyter notebooks
 Home-page: https://dbgit.prakinf.tu-ilmenau.de/lectures/data-science-grundlagen
 Author: Eric Tröbs
 Author-email: eric.troebs@tu-ilmenau.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tui_dsg-202404221312/setup.py` & `tui_dsg-202404250955/setup.py`

 * *Files identical despite different names*

### Comparing `tui_dsg-202404221312/src/tui_dsg.egg-info/PKG-INFO` & `tui_dsg-202404250955/src/tui_dsg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tui_dsg
-Version: 202404221312
+Version: 202404250955
 Summary: everything you need for our jupyter notebooks
 Home-page: https://dbgit.prakinf.tu-ilmenau.de/lectures/data-science-grundlagen
 Author: Eric Tröbs
 Author-email: eric.troebs@tu-ilmenau.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

