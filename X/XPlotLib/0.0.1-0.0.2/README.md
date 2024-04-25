# Comparing `tmp/xplotlib-0.0.1.tar.gz` & `tmp/xplotlib-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xplotlib-0.0.1.tar", last modified: Tue Apr 23 22:46:44 2024, max compression
+gzip compressed data, was "xplotlib-0.0.2.tar", last modified: Thu Apr 25 04:23:46 2024, max compression
```

## Comparing `xplotlib-0.0.1.tar` & `xplotlib-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:46:44.506619 xplotlib-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-23 22:46:32.000000 xplotlib-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-23 22:46:44.506619 xplotlib-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-23 22:46:32.000000 xplotlib-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-23 22:46:32.000000 xplotlib-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-23 22:46:44.506619 xplotlib-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:46:44.502619 xplotlib-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:46:44.506619 xplotlib-0.0.1/src/XPlotLib/
--rw-r--r--   0 runner    (1001) docker     (127)    17920 2024-04-23 22:46:32.000000 xplotlib-0.0.1/src/XPlotLib/DOSAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:46:32.000000 xplotlib-0.0.1/src/XPlotLib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:46:44.506619 xplotlib-0.0.1/src/XPlotLib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-23 22:46:44.000000 xplotlib-0.0.1/src/XPlotLib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-23 22:46:44.000000 xplotlib-0.0.1/src/XPlotLib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 22:46:44.000000 xplotlib-0.0.1/src/XPlotLib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-23 22:46:44.000000 xplotlib-0.0.1/src/XPlotLib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 22:46:44.000000 xplotlib-0.0.1/src/XPlotLib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:23:46.909131 xplotlib-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-25 04:23:40.000000 xplotlib-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-25 04:23:46.909131 xplotlib-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-25 04:23:40.000000 xplotlib-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-25 04:23:40.000000 xplotlib-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-25 04:23:46.909131 xplotlib-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:23:46.901131 xplotlib-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:23:46.905131 xplotlib-0.0.2/src/XPlotLib/
+-rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-04-25 04:23:40.000000 xplotlib-0.0.2/src/XPlotLib/BandgapAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17920 2024-04-25 04:23:40.000000 xplotlib-0.0.2/src/XPlotLib/DOSAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-25 04:23:40.000000 xplotlib-0.0.2/src/XPlotLib/XPlotLibUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:23:40.000000 xplotlib-0.0.2/src/XPlotLib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:23:46.905131 xplotlib-0.0.2/src/XPlotLib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-25 04:23:46.000000 xplotlib-0.0.2/src/XPlotLib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-25 04:23:46.000000 xplotlib-0.0.2/src/XPlotLib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 04:23:46.000000 xplotlib-0.0.2/src/XPlotLib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-25 04:23:46.000000 xplotlib-0.0.2/src/XPlotLib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 04:23:46.000000 xplotlib-0.0.2/src/XPlotLib.egg-info/top_level.txt
```

### Comparing `xplotlib-0.0.1/LICENSE` & `xplotlib-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xplotlib-0.0.1/PKG-INFO` & `xplotlib-0.0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XPlotLib
-Version: 0.0.1
+Version: 0.0.2
 Summary: Libary to plot experimental and theoretical XRay data.
 Home-page: https://github.com/CMM02/XPlotLib
 Author: Carl Magnus Meier
 Author-email: magnus.meier@outook.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xplotlib-0.0.1/setup.cfg` & `xplotlib-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = XPlotLib
-version = 0.0.1
+version = 0.0.2
 author = Carl Magnus Meier
 author_email = magnus.meier@outook.de
 description = Libary to plot experimental and theoretical XRay data.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CMM02/XPlotLib
 classifiers =
```

### Comparing `xplotlib-0.0.1/src/XPlotLib/DOSAnalyzer.py` & `xplotlib-0.0.2/src/XPlotLib/DOSAnalyzer.py`

 * *Files identical despite different names*

### Comparing `xplotlib-0.0.1/src/XPlotLib.egg-info/PKG-INFO` & `xplotlib-0.0.2/src/XPlotLib.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XPlotLib
-Version: 0.0.1
+Version: 0.0.2
 Summary: Libary to plot experimental and theoretical XRay data.
 Home-page: https://github.com/CMM02/XPlotLib
 Author: Carl Magnus Meier
 Author-email: magnus.meier@outook.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

