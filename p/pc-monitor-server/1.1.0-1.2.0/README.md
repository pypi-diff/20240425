# Comparing `tmp/pc-monitor-server-1.1.0.tar.gz` & `tmp/pc-monitor-server-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pc-monitor-server-1.1.0.tar", last modified: Thu Jan 11 10:06:12 2024, max compression
+gzip compressed data, was "pc-monitor-server-1.2.0.tar", last modified: Thu Apr 25 06:41:47 2024, max compression
```

## Comparing `pc-monitor-server-1.1.0.tar` & `pc-monitor-server-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 neucrack  (1000) neucrack  (1000)        0 2024-01-11 10:06:12.651271 pc-monitor-server-1.1.0/
--rw-rw-r--   0 neucrack  (1000) neucrack  (1000)     1065 2024-01-08 02:02:21.000000 pc-monitor-server-1.1.0/LICENSE
--rw-rw-r--   0 neucrack  (1000) neucrack  (1000)      207 2024-01-11 10:06:12.651271 pc-monitor-server-1.1.0/PKG-INFO
--rw-rw-r--   0 neucrack  (1000) neucrack  (1000)      606 2024-01-11 10:02:47.000000 pc-monitor-server-1.1.0/README.md
-drwxrwxr-x   0 neucrack  (1000) neucrack  (1000)        0 2024-01-11 10:06:12.651271 pc-monitor-server-1.1.0/pc_monitor_server/
--rw-rw-r--   0 neucrack  (1000) neucrack  (1000)       61 2024-01-10 13:12:32.000000 pc-monitor-server-1.1.0/pc_monitor_server/__init__.py
--rw-rw-r--   0 neucrack  (1000) neucrack  (1000)     1751 2024-01-11 09:48:46.000000 pc-monitor-server-1.1.0/pc_monitor_server/main.py
--rw-rw-r--   0 neucrack  (1000) neucrack  (1000)     6830 2024-01-09 10:51:19.000000 pc-monitor-server-1.1.0/pc_monitor_server/util.py
--rw-rw-r--   0 neucrack  (1000) neucrack  (1000)       22 2024-01-11 10:06:06.000000 pc-monitor-server-1.1.0/pc_monitor_server/version.py
-drwxrwxr-x   0 neucrack  (1000) neucrack  (1000)        0 2024-01-11 10:06:12.651271 pc-monitor-server-1.1.0/pc_monitor_server.egg-info/
--rw-rw-r--   0 neucrack  (1000) neucrack  (1000)      207 2024-01-11 10:06:12.000000 pc-monitor-server-1.1.0/pc_monitor_server.egg-info/PKG-INFO
--rw-rw-r--   0 neucrack  (1000) neucrack  (1000)      385 2024-01-11 10:06:12.000000 pc-monitor-server-1.1.0/pc_monitor_server.egg-info/SOURCES.txt
--rw-rw-r--   0 neucrack  (1000) neucrack  (1000)        1 2024-01-11 10:06:12.000000 pc-monitor-server-1.1.0/pc_monitor_server.egg-info/dependency_links.txt
--rw-rw-r--   0 neucrack  (1000) neucrack  (1000)       71 2024-01-11 10:06:12.000000 pc-monitor-server-1.1.0/pc_monitor_server.egg-info/entry_points.txt
--rw-rw-r--   0 neucrack  (1000) neucrack  (1000)      110 2024-01-11 10:06:12.000000 pc-monitor-server-1.1.0/pc_monitor_server.egg-info/requires.txt
--rw-rw-r--   0 neucrack  (1000) neucrack  (1000)       18 2024-01-11 10:06:12.000000 pc-monitor-server-1.1.0/pc_monitor_server.egg-info/top_level.txt
--rw-rw-r--   0 neucrack  (1000) neucrack  (1000)       38 2024-01-11 10:06:12.651271 pc-monitor-server-1.1.0/setup.cfg
--rw-rw-r--   0 neucrack  (1000) neucrack  (1000)      938 2024-01-10 14:03:48.000000 pc-monitor-server-1.1.0/setup.py
+drwxrwxr-x   0 neucrack  (1000) neucrack  (1000)        0 2024-04-25 06:41:47.516436 pc-monitor-server-1.2.0/
+-rw-rw-r--   0 neucrack  (1000) neucrack  (1000)     1065 2024-01-08 02:02:21.000000 pc-monitor-server-1.2.0/LICENSE
+-rw-rw-r--   0 neucrack  (1000) neucrack  (1000)      207 2024-04-25 06:41:47.516436 pc-monitor-server-1.2.0/PKG-INFO
+-rw-rw-r--   0 neucrack  (1000) neucrack  (1000)      606 2024-01-11 10:02:47.000000 pc-monitor-server-1.2.0/README.md
+drwxrwxr-x   0 neucrack  (1000) neucrack  (1000)        0 2024-04-25 06:41:47.516436 pc-monitor-server-1.2.0/pc_monitor_server/
+-rw-rw-r--   0 neucrack  (1000) neucrack  (1000)       61 2024-01-10 13:12:32.000000 pc-monitor-server-1.2.0/pc_monitor_server/__init__.py
+-rw-rw-r--   0 neucrack  (1000) neucrack  (1000)       70 2024-04-25 06:41:35.000000 pc-monitor-server-1.2.0/pc_monitor_server/__main__.py
+-rw-rw-r--   0 neucrack  (1000) neucrack  (1000)     4097 2024-04-25 06:41:35.000000 pc-monitor-server-1.2.0/pc_monitor_server/main.py
+-rw-rw-r--   0 neucrack  (1000) neucrack  (1000)     6830 2024-01-09 10:51:19.000000 pc-monitor-server-1.2.0/pc_monitor_server/util.py
+-rw-rw-r--   0 neucrack  (1000) neucrack  (1000)       22 2024-04-25 06:41:35.000000 pc-monitor-server-1.2.0/pc_monitor_server/version.py
+drwxrwxr-x   0 neucrack  (1000) neucrack  (1000)        0 2024-04-25 06:41:47.516436 pc-monitor-server-1.2.0/pc_monitor_server.egg-info/
+-rw-rw-r--   0 neucrack  (1000) neucrack  (1000)      207 2024-04-25 06:41:47.000000 pc-monitor-server-1.2.0/pc_monitor_server.egg-info/PKG-INFO
+-rw-rw-r--   0 neucrack  (1000) neucrack  (1000)      415 2024-04-25 06:41:47.000000 pc-monitor-server-1.2.0/pc_monitor_server.egg-info/SOURCES.txt
+-rw-rw-r--   0 neucrack  (1000) neucrack  (1000)        1 2024-04-25 06:41:47.000000 pc-monitor-server-1.2.0/pc_monitor_server.egg-info/dependency_links.txt
+-rw-rw-r--   0 neucrack  (1000) neucrack  (1000)       71 2024-04-25 06:41:47.000000 pc-monitor-server-1.2.0/pc_monitor_server.egg-info/entry_points.txt
+-rw-rw-r--   0 neucrack  (1000) neucrack  (1000)      130 2024-04-25 06:41:47.000000 pc-monitor-server-1.2.0/pc_monitor_server.egg-info/requires.txt
+-rw-rw-r--   0 neucrack  (1000) neucrack  (1000)       18 2024-04-25 06:41:47.000000 pc-monitor-server-1.2.0/pc_monitor_server.egg-info/top_level.txt
+-rw-rw-r--   0 neucrack  (1000) neucrack  (1000)       38 2024-04-25 06:41:47.516436 pc-monitor-server-1.2.0/setup.cfg
+-rw-rw-r--   0 neucrack  (1000) neucrack  (1000)      955 2024-04-25 06:41:35.000000 pc-monitor-server-1.2.0/setup.py
```

### Comparing `pc-monitor-server-1.1.0/LICENSE` & `pc-monitor-server-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pc-monitor-server-1.1.0/README.md` & `pc-monitor-server-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pc-monitor-server-1.1.0/pc_monitor_server/util.py` & `pc-monitor-server-1.2.0/pc_monitor_server/util.py`

 * *Files identical despite different names*

### Comparing `pc-monitor-server-1.1.0/setup.py` & `pc-monitor-server-1.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from setuptools import setup, find_packages
 
 requirements = [
     "Flask",
     "pynvml",
-    "qrcode"
+    "qrcode",
+    "netifaces"
 ]
 requirements_win = [
     "wmi",
     "pythonnet"
 ]
 requirements_unix = requirements
```

