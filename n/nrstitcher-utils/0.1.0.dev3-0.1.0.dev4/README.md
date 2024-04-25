# Comparing `tmp/nrstitcher_utils-0.1.0.dev3.tar.gz` & `tmp/nrstitcher_utils-0.1.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrstitcher_utils-0.1.0.dev3.tar", last modified: Tue Apr 23 13:42:07 2024, max compression
+gzip compressed data, was "nrstitcher_utils-0.1.0.dev4.tar", last modified: Thu Apr 25 06:37:45 2024, max compression
```

## Comparing `nrstitcher_utils-0.1.0.dev3.tar` & `nrstitcher_utils-0.1.0.dev4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 13:42:07.580072 nrstitcher_utils-0.1.0.dev3/
--rw-r--r--   0 payno     (1000) payno     (1000)     1241 2024-04-23 06:19:33.000000 nrstitcher_utils-0.1.0.dev3/LICENSE
--rw-r--r--   0 payno     (1000) payno     (1000)     3612 2024-04-23 13:42:07.580072 nrstitcher_utils-0.1.0.dev3/PKG-INFO
--rw-r--r--   0 payno     (1000) payno     (1000)      251 2024-04-23 06:19:33.000000 nrstitcher_utils-0.1.0.dev3/README.md
--rw-r--r--   0 payno     (1000) payno     (1000)     2131 2024-04-23 06:24:16.000000 nrstitcher_utils-0.1.0.dev3/pyproject.toml
--rw-r--r--   0 payno     (1000) payno     (1000)       38 2024-04-23 13:42:07.580072 nrstitcher_utils-0.1.0.dev3/setup.cfg
--rw-r--r--   0 payno     (1000) payno     (1000)       38 2024-04-23 06:34:32.000000 nrstitcher_utils-0.1.0.dev3/setup.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 13:42:07.576073 nrstitcher_utils-0.1.0.dev3/src/
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 13:42:07.576073 nrstitcher_utils-0.1.0.dev3/src/nrstitcher_utils/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-23 06:19:33.000000 nrstitcher_utils-0.1.0.dev3/src/nrstitcher_utils/__init__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 13:42:07.580072 nrstitcher_utils-0.1.0.dev3/src/nrstitcher_utils/app/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-23 06:19:33.000000 nrstitcher_utils-0.1.0.dev3/src/nrstitcher_utils/app/__init__.py
--rwxr-xr-x   0 payno     (1000) payno     (1000)     8309 2024-04-23 13:40:29.000000 nrstitcher_utils-0.1.0.dev3/src/nrstitcher_utils/app/nrs_config_id16a_ht.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 13:42:07.580072 nrstitcher_utils-0.1.0.dev3/src/nrstitcher_utils/core/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-23 06:24:31.000000 nrstitcher_utils-0.1.0.dev3/src/nrstitcher_utils/core/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3220 2024-04-23 07:26:52.000000 nrstitcher_utils-0.1.0.dev3/src/nrstitcher_utils/core/h5_settings.py
--rw-r--r--   0 payno     (1000) payno     (1000)     8694 2024-04-23 07:27:28.000000 nrstitcher_utils-0.1.0.dev3/src/nrstitcher_utils/core/ht_vol.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3430 2024-04-23 06:34:32.000000 nrstitcher_utils-0.1.0.dev3/src/nrstitcher_utils/core/utils.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 13:42:07.580072 nrstitcher_utils-0.1.0.dev3/src/nrstitcher_utils/resources/
--rw-r--r--   0 payno     (1000) payno     (1000)      282 2024-04-23 13:31:31.000000 nrstitcher_utils-0.1.0.dev3/src/nrstitcher_utils/resources/__init__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 13:42:07.580072 nrstitcher_utils-0.1.0.dev3/src/nrstitcher_utils/resources/config_files/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-23 13:41:08.000000 nrstitcher_utils-0.1.0.dev3/src/nrstitcher_utils/resources/config_files/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)       45 2024-04-23 13:42:01.000000 nrstitcher_utils-0.1.0.dev3/src/nrstitcher_utils/version.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 13:42:07.580072 nrstitcher_utils-0.1.0.dev3/src/nrstitcher_utils.egg-info/
--rw-r--r--   0 payno     (1000) payno     (1000)     3612 2024-04-23 13:42:07.000000 nrstitcher_utils-0.1.0.dev3/src/nrstitcher_utils.egg-info/PKG-INFO
--rw-r--r--   0 payno     (1000) payno     (1000)      706 2024-04-23 13:42:07.000000 nrstitcher_utils-0.1.0.dev3/src/nrstitcher_utils.egg-info/SOURCES.txt
--rw-r--r--   0 payno     (1000) payno     (1000)        1 2024-04-23 13:42:07.000000 nrstitcher_utils-0.1.0.dev3/src/nrstitcher_utils.egg-info/dependency_links.txt
--rw-r--r--   0 payno     (1000) payno     (1000)       86 2024-04-23 13:42:07.000000 nrstitcher_utils-0.1.0.dev3/src/nrstitcher_utils.egg-info/entry_points.txt
--rw-r--r--   0 payno     (1000) payno     (1000)      138 2024-04-23 13:42:07.000000 nrstitcher_utils-0.1.0.dev3/src/nrstitcher_utils.egg-info/requires.txt
--rw-r--r--   0 payno     (1000) payno     (1000)       17 2024-04-23 13:42:07.000000 nrstitcher_utils-0.1.0.dev3/src/nrstitcher_utils.egg-info/top_level.txt
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-25 06:37:45.276165 nrstitcher_utils-0.1.0.dev4/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1241 2024-04-22 13:12:35.000000 nrstitcher_utils-0.1.0.dev4/LICENSE
+-rw-r--r--   0 payno     (1000) payno     (1000)     3612 2024-04-25 06:37:45.276165 nrstitcher_utils-0.1.0.dev4/PKG-INFO
+-rw-r--r--   0 payno     (1000) payno     (1000)      251 2024-04-25 06:33:30.000000 nrstitcher_utils-0.1.0.dev4/README.md
+-rw-r--r--   0 payno     (1000) payno     (1000)     2131 2024-04-25 06:33:38.000000 nrstitcher_utils-0.1.0.dev4/pyproject.toml
+-rw-r--r--   0 payno     (1000) payno     (1000)       38 2024-04-25 06:37:45.276165 nrstitcher_utils-0.1.0.dev4/setup.cfg
+-rw-r--r--   0 payno     (1000) payno     (1000)       38 2024-04-25 06:33:38.000000 nrstitcher_utils-0.1.0.dev4/setup.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-25 06:37:45.276165 nrstitcher_utils-0.1.0.dev4/src/
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-25 06:37:45.276165 nrstitcher_utils-0.1.0.dev4/src/nrstitcher_utils/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-22 12:54:51.000000 nrstitcher_utils-0.1.0.dev4/src/nrstitcher_utils/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-25 06:37:45.276165 nrstitcher_utils-0.1.0.dev4/src/nrstitcher_utils/app/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-25 06:33:38.000000 nrstitcher_utils-0.1.0.dev4/src/nrstitcher_utils/app/__init__.py
+-rwxr-xr-x   0 payno     (1000) payno     (1000)     8267 2024-04-25 06:37:15.000000 nrstitcher_utils-0.1.0.dev4/src/nrstitcher_utils/app/nrs_config_id16a_ht.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-25 06:37:45.276165 nrstitcher_utils-0.1.0.dev4/src/nrstitcher_utils/core/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-25 06:33:38.000000 nrstitcher_utils-0.1.0.dev4/src/nrstitcher_utils/core/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3220 2024-04-25 06:33:38.000000 nrstitcher_utils-0.1.0.dev4/src/nrstitcher_utils/core/h5_settings.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8694 2024-04-25 06:33:38.000000 nrstitcher_utils-0.1.0.dev4/src/nrstitcher_utils/core/ht_vol.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3430 2024-04-25 06:33:38.000000 nrstitcher_utils-0.1.0.dev4/src/nrstitcher_utils/core/utils.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-25 06:37:45.276165 nrstitcher_utils-0.1.0.dev4/src/nrstitcher_utils/resources/
+-rw-r--r--   0 payno     (1000) payno     (1000)      282 2024-04-25 06:33:38.000000 nrstitcher_utils-0.1.0.dev4/src/nrstitcher_utils/resources/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-25 06:37:45.276165 nrstitcher_utils-0.1.0.dev4/src/nrstitcher_utils/resources/config_files/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-25 06:33:38.000000 nrstitcher_utils-0.1.0.dev4/src/nrstitcher_utils/resources/config_files/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)       45 2024-04-25 06:35:22.000000 nrstitcher_utils-0.1.0.dev4/src/nrstitcher_utils/version.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-25 06:37:45.276165 nrstitcher_utils-0.1.0.dev4/src/nrstitcher_utils.egg-info/
+-rw-r--r--   0 payno     (1000) payno     (1000)     3612 2024-04-25 06:37:45.000000 nrstitcher_utils-0.1.0.dev4/src/nrstitcher_utils.egg-info/PKG-INFO
+-rw-r--r--   0 payno     (1000) payno     (1000)      706 2024-04-25 06:37:45.000000 nrstitcher_utils-0.1.0.dev4/src/nrstitcher_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)        1 2024-04-25 06:37:45.000000 nrstitcher_utils-0.1.0.dev4/src/nrstitcher_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)       86 2024-04-25 06:37:45.000000 nrstitcher_utils-0.1.0.dev4/src/nrstitcher_utils.egg-info/entry_points.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)      138 2024-04-25 06:37:45.000000 nrstitcher_utils-0.1.0.dev4/src/nrstitcher_utils.egg-info/requires.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)       17 2024-04-25 06:37:45.000000 nrstitcher_utils-0.1.0.dev4/src/nrstitcher_utils.egg-info/top_level.txt
```

### Comparing `nrstitcher_utils-0.1.0.dev3/LICENSE` & `nrstitcher_utils-0.1.0.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `nrstitcher_utils-0.1.0.dev3/PKG-INFO` & `nrstitcher_utils-0.1.0.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrstitcher_utils
-Version: 0.1.0.dev3
+Version: 0.1.0.dev4
 Summary: NRStitcher utils for esrf usage
 Author: Arttu Miettenen, Yervand Azatian
 Author-email: Jayde Livingstone <jayde.livingstone@gmail.com>, Henri Payno <henri.payno@esrf.fr>
 License: The nrstitcher_utils library goal is to ease usage of nrstitcher at esrf
         
         nrstitcher_utils is distributed under the MIT license.
```

### Comparing `nrstitcher_utils-0.1.0.dev3/pyproject.toml` & `nrstitcher_utils-0.1.0.dev4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nrstitcher_utils-0.1.0.dev3/src/nrstitcher_utils/app/nrs_config_id16a_ht.py` & `nrstitcher_utils-0.1.0.dev4/src/nrstitcher_utils/app/nrs_config_id16a_ht.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/data/id16a/inhouse1/sware/NRstitcher/pyenv/bin/python3
+# coding: utf-8
 
 """
 stitch_settings_from_ID16a_ht.py:
 
 This script is dedicated to holotomographic data acquired on the beamline ID16A at the ESRF, and is used to generate a stitch settings file to be used as input to nr_stitcher.py. 
 The stitch settings file is generated based on the template default_stitch_settings.py provided with nr_stitcher, with parameters mofdified based on user-selected options.
 After adding the NRStitcher directory to the path, this script should be run from the directory where the generated stitch settings file is to be saved.
```

### Comparing `nrstitcher_utils-0.1.0.dev3/src/nrstitcher_utils/core/h5_settings.py` & `nrstitcher_utils-0.1.0.dev4/src/nrstitcher_utils/core/h5_settings.py`

 * *Files identical despite different names*

### Comparing `nrstitcher_utils-0.1.0.dev3/src/nrstitcher_utils/core/ht_vol.py` & `nrstitcher_utils-0.1.0.dev4/src/nrstitcher_utils/core/ht_vol.py`

 * *Files identical despite different names*

### Comparing `nrstitcher_utils-0.1.0.dev3/src/nrstitcher_utils/core/utils.py` & `nrstitcher_utils-0.1.0.dev4/src/nrstitcher_utils/core/utils.py`

 * *Files identical despite different names*

### Comparing `nrstitcher_utils-0.1.0.dev3/src/nrstitcher_utils.egg-info/PKG-INFO` & `nrstitcher_utils-0.1.0.dev4/src/nrstitcher_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrstitcher_utils
-Version: 0.1.0.dev3
+Version: 0.1.0.dev4
 Summary: NRStitcher utils for esrf usage
 Author: Arttu Miettenen, Yervand Azatian
 Author-email: Jayde Livingstone <jayde.livingstone@gmail.com>, Henri Payno <henri.payno@esrf.fr>
 License: The nrstitcher_utils library goal is to ease usage of nrstitcher at esrf
         
         nrstitcher_utils is distributed under the MIT license.
```

### Comparing `nrstitcher_utils-0.1.0.dev3/src/nrstitcher_utils.egg-info/SOURCES.txt` & `nrstitcher_utils-0.1.0.dev4/src/nrstitcher_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

