# Comparing `tmp/neon_gui-1.3.0.tar.gz` & `tmp/neon_gui-1.3.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon_gui-1.3.0.tar", last modified: Tue Apr 23 17:16:53 2024, max compression
+gzip compressed data, was "neon_gui-1.3.1a1.tar", last modified: Thu Apr 25 19:49:56 2024, max compression
```

## Comparing `neon_gui-1.3.0.tar` & `neon_gui-1.3.1a1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:53.391005 neon_gui-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-23 17:16:44.000000 neon_gui-1.3.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-23 17:16:53.391005 neon_gui-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-23 17:16:44.000000 neon_gui-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:53.387005 neon_gui-1.3.0/neon_gui/
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-23 17:16:44.000000 neon_gui-1.3.0/neon_gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-23 17:16:44.000000 neon_gui-1.3.0/neon_gui/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-23 17:16:44.000000 neon_gui-1.3.0/neon_gui/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-23 17:16:44.000000 neon_gui-1.3.0/neon_gui/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-04-23 17:16:44.000000 neon_gui-1.3.0/neon_gui/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:53.391005 neon_gui-1.3.0/neon_gui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-23 17:16:53.000000 neon_gui-1.3.0/neon_gui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-23 17:16:53.000000 neon_gui-1.3.0/neon_gui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 17:16:53.000000 neon_gui-1.3.0/neon_gui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-23 17:16:53.000000 neon_gui-1.3.0/neon_gui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-23 17:16:53.000000 neon_gui-1.3.0/neon_gui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 17:16:53.000000 neon_gui-1.3.0/neon_gui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 17:16:53.391005 neon_gui-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-04-23 17:16:44.000000 neon_gui-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:49:56.607891 neon_gui-1.3.1a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-25 19:49:53.000000 neon_gui-1.3.1a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-25 19:49:56.607891 neon_gui-1.3.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-25 19:49:53.000000 neon_gui-1.3.1a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:49:56.603891 neon_gui-1.3.1a1/neon_gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-25 19:49:53.000000 neon_gui-1.3.1a1/neon_gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-25 19:49:53.000000 neon_gui-1.3.1a1/neon_gui/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-25 19:49:53.000000 neon_gui-1.3.1a1/neon_gui/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-25 19:49:53.000000 neon_gui-1.3.1a1/neon_gui/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-04-25 19:49:53.000000 neon_gui-1.3.1a1/neon_gui/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:49:56.607891 neon_gui-1.3.1a1/neon_gui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-25 19:49:56.000000 neon_gui-1.3.1a1/neon_gui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-25 19:49:56.000000 neon_gui-1.3.1a1/neon_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:49:56.000000 neon_gui-1.3.1a1/neon_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-25 19:49:56.000000 neon_gui-1.3.1a1/neon_gui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-25 19:49:56.000000 neon_gui-1.3.1a1/neon_gui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 19:49:56.000000 neon_gui-1.3.1a1/neon_gui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:49:56.607891 neon_gui-1.3.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-04-25 19:49:53.000000 neon_gui-1.3.1a1/setup.py
```

### Comparing `neon_gui-1.3.0/LICENSE.md` & `neon_gui-1.3.1a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon_gui-1.3.0/PKG-INFO` & `neon_gui-1.3.1a1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon_gui
-Version: 1.3.0
+Version: 1.3.1a1
 Summary: Neon GUI Module
 Home-page: https://github.com/NeonGeckoCom/neon_gui
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: docker
```

### Comparing `neon_gui-1.3.0/README.md` & `neon_gui-1.3.1a1/README.md`

 * *Files identical despite different names*

### Comparing `neon_gui-1.3.0/neon_gui/__init__.py` & `neon_gui-1.3.1a1/neon_gui/__init__.py`

 * *Files identical despite different names*

### Comparing `neon_gui-1.3.0/neon_gui/__main__.py` & `neon_gui-1.3.1a1/neon_gui/__main__.py`

 * *Files identical despite different names*

### Comparing `neon_gui-1.3.0/neon_gui/cli.py` & `neon_gui-1.3.1a1/neon_gui/cli.py`

 * *Files identical despite different names*

### Comparing `neon_gui-1.3.0/neon_gui/service.py` & `neon_gui-1.3.1a1/neon_gui/service.py`

 * *Files identical despite different names*

### Comparing `neon_gui-1.3.0/neon_gui/utils.py` & `neon_gui-1.3.1a1/neon_gui/utils.py`

 * *Files identical despite different names*

### Comparing `neon_gui-1.3.0/neon_gui.egg-info/PKG-INFO` & `neon_gui-1.3.1a1/neon_gui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-gui
-Version: 1.3.0
+Version: 1.3.1a1
 Summary: Neon GUI Module
 Home-page: https://github.com/NeonGeckoCom/neon_gui
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: docker
```

### Comparing `neon_gui-1.3.0/setup.py` & `neon_gui-1.3.1a1/setup.py`

 * *Files identical despite different names*

