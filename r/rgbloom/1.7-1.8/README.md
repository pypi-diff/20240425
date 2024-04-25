# Comparing `tmp/rgbloom-1.7.tar.gz` & `tmp/rgbloom-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rgbloom-1.7.tar", last modified: Wed Sep 27 17:15:30 2023, max compression
+gzip compressed data, was "rgbloom-1.8.tar", last modified: Thu Apr 25 14:27:12 2024, max compression
```

## Comparing `rgbloom-1.7.tar` & `rgbloom-1.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2023-09-27 17:15:30.270266 rgbloom-1.7/
--rw-r--r--   0 cardiel    (501) staff       (20)    35149 2022-11-06 08:36:25.000000 rgbloom-1.7/LICENSE
--rw-r--r--   0 cardiel    (501) staff       (20)    14558 2023-09-27 17:15:30.270046 rgbloom-1.7/PKG-INFO
--rw-r--r--   0 cardiel    (501) staff       (20)    13559 2023-09-27 17:14:08.000000 rgbloom-1.7/README.md
--rw-r--r--   0 cardiel    (501) staff       (20)      100 2022-11-06 08:38:35.000000 rgbloom-1.7/pyproject.toml
-drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2023-09-27 17:15:30.264794 rgbloom-1.7/rgbloom/
--rw-r--r--   0 cardiel    (501) staff       (20)       51 2022-11-06 08:39:16.000000 rgbloom-1.7/rgbloom/__init__.py
--rw-r--r--   0 cardiel    (501) staff       (20)     6597 2023-05-24 13:46:56.000000 rgbloom-1.7/rgbloom/__main__.py
--rw-r--r--   0 cardiel    (501) staff       (20)      439 2023-05-25 06:38:09.000000 rgbloom-1.7/rgbloom/choices_mag_plot.py
-drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2023-09-27 17:15:30.268608 rgbloom-1.7/rgbloom/core/
--rw-r--r--   0 cardiel    (501) staff       (20)        0 2022-11-06 08:39:16.000000 rgbloom-1.7/rgbloom/core/__init__.py
--rw-r--r--   0 cardiel    (501) staff       (20)     2487 2022-11-06 08:39:16.000000 rgbloom-1.7/rgbloom/core/step1.py
--rw-r--r--   0 cardiel    (501) staff       (20)     1844 2022-11-06 08:39:16.000000 rgbloom-1.7/rgbloom/core/step2.py
--rw-r--r--   0 cardiel    (501) staff       (20)     3128 2023-03-21 17:40:50.000000 rgbloom-1.7/rgbloom/core/step3.py
--rw-r--r--   0 cardiel    (501) staff       (20)     2560 2022-11-06 08:39:16.000000 rgbloom-1.7/rgbloom/core/step4.py
--rw-r--r--   0 cardiel    (501) staff       (20)     3007 2023-03-21 17:42:15.000000 rgbloom-1.7/rgbloom/core/step5.py
-drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2023-09-27 17:15:30.269425 rgbloom-1.7/rgbloom/gui/
--rw-r--r--   0 cardiel    (501) staff       (20)        0 2022-11-06 08:39:16.000000 rgbloom-1.7/rgbloom/gui/__init__.py
--rw-r--r--   0 cardiel    (501) staff       (20)    13610 2023-05-25 08:32:56.000000 rgbloom-1.7/rgbloom/gui/step6.py
--rw-r--r--   0 cardiel    (501) staff       (20)      497 2022-11-06 08:39:16.000000 rgbloom-1.7/rgbloom/gui/style.py
--rw-r--r--   0 cardiel    (501) staff       (20)       16 2023-09-27 17:09:33.000000 rgbloom-1.7/rgbloom/version.py
-drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2023-09-27 17:15:30.266898 rgbloom-1.7/rgbloom.egg-info/
--rw-r--r--   0 cardiel    (501) staff       (20)    14558 2023-09-27 17:15:30.000000 rgbloom-1.7/rgbloom.egg-info/PKG-INFO
--rw-r--r--   0 cardiel    (501) staff       (20)      527 2023-09-27 17:15:30.000000 rgbloom-1.7/rgbloom.egg-info/SOURCES.txt
--rw-r--r--   0 cardiel    (501) staff       (20)        1 2023-09-27 17:15:30.000000 rgbloom-1.7/rgbloom.egg-info/dependency_links.txt
--rw-r--r--   0 cardiel    (501) staff       (20)       50 2023-09-27 17:15:30.000000 rgbloom-1.7/rgbloom.egg-info/entry_points.txt
--rw-r--r--   0 cardiel    (501) staff       (20)       80 2023-09-27 17:15:30.000000 rgbloom-1.7/rgbloom.egg-info/requires.txt
--rw-r--r--   0 cardiel    (501) staff       (20)        8 2023-09-27 17:15:30.000000 rgbloom-1.7/rgbloom.egg-info/top_level.txt
--rw-r--r--   0 cardiel    (501) staff       (20)     1040 2023-09-27 17:15:30.270810 rgbloom-1.7/setup.cfg
--rw-r--r--   0 cardiel    (501) staff       (20)       68 2022-11-06 08:39:44.000000 rgbloom-1.7/setup.py
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-25 14:27:12.110639 rgbloom-1.8/
+-rw-r--r--   0 cardiel    (501) staff       (20)    35149 2022-11-06 08:36:25.000000 rgbloom-1.8/LICENSE
+-rw-r--r--   0 cardiel    (501) staff       (20)    14558 2024-04-25 14:27:12.110436 rgbloom-1.8/PKG-INFO
+-rw-r--r--   0 cardiel    (501) staff       (20)    13559 2023-09-27 17:14:08.000000 rgbloom-1.8/README.md
+-rw-r--r--   0 cardiel    (501) staff       (20)      100 2022-11-06 08:38:35.000000 rgbloom-1.8/pyproject.toml
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-25 14:27:12.103166 rgbloom-1.8/rgbloom/
+-rw-r--r--   0 cardiel    (501) staff       (20)       51 2022-11-06 08:39:16.000000 rgbloom-1.8/rgbloom/__init__.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     6597 2023-05-24 13:46:56.000000 rgbloom-1.8/rgbloom/__main__.py
+-rw-r--r--   0 cardiel    (501) staff       (20)      439 2023-05-25 06:38:09.000000 rgbloom-1.8/rgbloom/choices_mag_plot.py
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-25 14:27:12.108018 rgbloom-1.8/rgbloom/core/
+-rw-r--r--   0 cardiel    (501) staff       (20)        0 2022-11-06 08:39:16.000000 rgbloom-1.8/rgbloom/core/__init__.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     2735 2024-04-25 14:25:02.000000 rgbloom-1.8/rgbloom/core/step1.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     1844 2022-11-06 08:39:16.000000 rgbloom-1.8/rgbloom/core/step2.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     3128 2023-03-21 17:40:50.000000 rgbloom-1.8/rgbloom/core/step3.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     2560 2022-11-06 08:39:16.000000 rgbloom-1.8/rgbloom/core/step4.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     3007 2023-03-21 17:42:15.000000 rgbloom-1.8/rgbloom/core/step5.py
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-25 14:27:12.109166 rgbloom-1.8/rgbloom/gui/
+-rw-r--r--   0 cardiel    (501) staff       (20)        0 2022-11-06 08:39:16.000000 rgbloom-1.8/rgbloom/gui/__init__.py
+-rw-r--r--   0 cardiel    (501) staff       (20)    13610 2023-05-25 08:32:56.000000 rgbloom-1.8/rgbloom/gui/step6.py
+-rw-r--r--   0 cardiel    (501) staff       (20)      497 2022-11-06 08:39:16.000000 rgbloom-1.8/rgbloom/gui/style.py
+-rw-r--r--   0 cardiel    (501) staff       (20)      171 2024-04-25 14:25:02.000000 rgbloom-1.8/rgbloom/version.py
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-25 14:27:12.109742 rgbloom-1.8/rgbloom.egg-info/
+-rw-r--r--   0 cardiel    (501) staff       (20)    14558 2024-04-25 14:27:12.000000 rgbloom-1.8/rgbloom.egg-info/PKG-INFO
+-rw-r--r--   0 cardiel    (501) staff       (20)      527 2024-04-25 14:27:12.000000 rgbloom-1.8/rgbloom.egg-info/SOURCES.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)        1 2024-04-25 14:27:12.000000 rgbloom-1.8/rgbloom.egg-info/dependency_links.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)       50 2024-04-25 14:27:12.000000 rgbloom-1.8/rgbloom.egg-info/entry_points.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)       80 2024-04-25 14:27:12.000000 rgbloom-1.8/rgbloom.egg-info/requires.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)        8 2024-04-25 14:27:12.000000 rgbloom-1.8/rgbloom.egg-info/top_level.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)     1040 2024-04-25 14:27:12.111186 rgbloom-1.8/setup.cfg
+-rw-r--r--   0 cardiel    (501) staff       (20)       68 2022-11-06 08:39:44.000000 rgbloom-1.8/setup.py
```

### Comparing `rgbloom-1.7/LICENSE` & `rgbloom-1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rgbloom-1.7/PKG-INFO` & `rgbloom-1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgbloom
-Version: 1.7
+Version: 1.8
 Summary: RGB from Gaia EDR3
 Home-page: https://github.com/guaix-ucm/rgbloom
 Author: Nicolás Cardiel
 Author-email: cardiel@ucm.es
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `rgbloom-1.7/README.md` & `rgbloom-1.8/README.md`

 * *Files identical despite different names*

### Comparing `rgbloom-1.7/rgbloom/__main__.py` & `rgbloom-1.8/rgbloom/__main__.py`

 * *Files identical despite different names*

### Comparing `rgbloom-1.7/rgbloom/core/step1.py` & `rgbloom-1.8/rgbloom/core/step1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright 2022 Universidad Complutense de Madrid
+# Copyright 2022-2024 Universidad Complutense de Madrid
 #
 # SPDX-License-Identifier: GPL-3.0+
 # License-Filename: LICENSE.txt
 #
 
 """
 Perform DR3 query
@@ -80,8 +80,13 @@
     mask_variable = r_dr3['phot_variable_flag'] == 'VARIABLE'
     r_dr3_variable = r_dr3[mask_variable]
     nstars_variable = len(r_dr3_variable)
     print(f'        --> {nstars_variable} objects classified as VARIABLE')
     if verbose:
         r_dr3.pprint(max_width=1000)
 
+    # change the column labels to lowercase
+    # (important: the Gaia database has changed 'source_id' by 'SOURCE_ID')
+    new_colnames = [colname.lower() for colname in r_dr3.colnames]
+    r_dr3.rename_columns(r_dr3.colnames, new_colnames)
+
     return r_dr3, nstars
```

### Comparing `rgbloom-1.7/rgbloom/core/step2.py` & `rgbloom-1.8/rgbloom/core/step2.py`

 * *Files identical despite different names*

### Comparing `rgbloom-1.7/rgbloom/core/step3.py` & `rgbloom-1.8/rgbloom/core/step3.py`

 * *Files identical despite different names*

### Comparing `rgbloom-1.7/rgbloom/core/step4.py` & `rgbloom-1.8/rgbloom/core/step4.py`

 * *Files identical despite different names*

### Comparing `rgbloom-1.7/rgbloom/core/step5.py` & `rgbloom-1.8/rgbloom/core/step5.py`

 * *Files identical despite different names*

### Comparing `rgbloom-1.7/rgbloom/gui/step6.py` & `rgbloom-1.8/rgbloom/gui/step6.py`

 * *Files identical despite different names*

### Comparing `rgbloom-1.7/rgbloom.egg-info/PKG-INFO` & `rgbloom-1.8/rgbloom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgbloom
-Version: 1.7
+Version: 1.8
 Summary: RGB from Gaia EDR3
 Home-page: https://github.com/guaix-ucm/rgbloom
 Author: Nicolás Cardiel
 Author-email: cardiel@ucm.es
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `rgbloom-1.7/rgbloom.egg-info/SOURCES.txt` & `rgbloom-1.8/rgbloom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rgbloom-1.7/setup.cfg` & `rgbloom-1.8/setup.cfg`

 * *Files identical despite different names*

