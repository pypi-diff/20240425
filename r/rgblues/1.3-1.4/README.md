# Comparing `tmp/rgblues-1.3.tar.gz` & `tmp/rgblues-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rgblues-1.3.tar", last modified: Sat Feb  3 10:10:50 2024, max compression
+gzip compressed data, was "rgblues-1.4.tar", last modified: Thu Apr 25 14:48:31 2024, max compression
```

## Comparing `rgblues-1.3.tar` & `rgblues-1.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-02-03 10:10:50.076547 rgblues-1.3/
--rw-r--r--   0 cardiel    (501) staff       (20)    35149 2022-11-05 19:26:58.000000 rgblues-1.3/LICENSE
--rw-r--r--   0 cardiel    (501) staff       (20)    11041 2024-02-03 10:10:50.076459 rgblues-1.3/PKG-INFO
--rw-r--r--   0 cardiel    (501) staff       (20)    10111 2024-02-03 10:01:12.000000 rgblues-1.3/README.md
--rw-r--r--   0 cardiel    (501) staff       (20)      100 2022-11-05 19:26:58.000000 rgblues-1.3/pyproject.toml
-drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-02-03 10:10:50.073948 rgblues-1.3/rgblues/
--rw-r--r--   0 cardiel    (501) staff       (20)       51 2022-11-05 19:26:58.000000 rgblues-1.3/rgblues/__init__.py
--rw-r--r--   0 cardiel    (501) staff       (20)     7020 2022-11-05 19:26:58.000000 rgblues-1.3/rgblues/__main__.py
-drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-02-03 10:10:50.075695 rgblues-1.3/rgblues/core/
--rw-r--r--   0 cardiel    (501) staff       (20)        0 2022-11-05 19:26:58.000000 rgblues-1.3/rgblues/core/__init__.py
--rw-r--r--   0 cardiel    (501) staff       (20)     2468 2022-11-05 19:26:58.000000 rgblues-1.3/rgblues/core/step1.py
--rw-r--r--   0 cardiel    (501) staff       (20)     3469 2022-11-05 19:26:58.000000 rgblues-1.3/rgblues/core/step2.py
--rw-r--r--   0 cardiel    (501) staff       (20)     1253 2022-11-05 19:26:58.000000 rgblues-1.3/rgblues/core/step3.py
--rw-r--r--   0 cardiel    (501) staff       (20)     2245 2022-11-05 19:26:58.000000 rgblues-1.3/rgblues/core/step4.py
--rw-r--r--   0 cardiel    (501) staff       (20)     2080 2022-11-05 19:26:58.000000 rgblues-1.3/rgblues/core/step5.py
--rw-r--r--   0 cardiel    (501) staff       (20)     2115 2022-11-05 19:26:58.000000 rgblues-1.3/rgblues/core/step6.py
--rw-r--r--   0 cardiel    (501) staff       (20)     5591 2022-11-05 19:26:58.000000 rgblues-1.3/rgblues/core/step7.py
-drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-02-03 10:10:50.076091 rgblues-1.3/rgblues/gui/
--rw-r--r--   0 cardiel    (501) staff       (20)        0 2022-11-05 19:26:58.000000 rgblues-1.3/rgblues/gui/__init__.py
--rw-r--r--   0 cardiel    (501) staff       (20)     8492 2022-11-06 08:27:37.000000 rgblues-1.3/rgblues/gui/step8.py
--rw-r--r--   0 cardiel    (501) staff       (20)      496 2022-11-05 19:26:58.000000 rgblues-1.3/rgblues/gui/style.py
--rw-r--r--   0 cardiel    (501) staff       (20)       16 2024-02-03 10:09:02.000000 rgblues-1.3/rgblues/version.py
-drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-02-03 10:10:50.076260 rgblues-1.3/rgblues.egg-info/
--rw-r--r--   0 cardiel    (501) staff       (20)    11041 2024-02-03 10:10:50.000000 rgblues-1.3/rgblues.egg-info/PKG-INFO
--rw-r--r--   0 cardiel    (501) staff       (20)      543 2024-02-03 10:10:50.000000 rgblues-1.3/rgblues.egg-info/SOURCES.txt
--rw-r--r--   0 cardiel    (501) staff       (20)        1 2024-02-03 10:10:50.000000 rgblues-1.3/rgblues.egg-info/dependency_links.txt
--rw-r--r--   0 cardiel    (501) staff       (20)       50 2024-02-03 10:10:50.000000 rgblues-1.3/rgblues.egg-info/entry_points.txt
--rw-r--r--   0 cardiel    (501) staff       (20)       56 2024-02-03 10:10:50.000000 rgblues-1.3/rgblues.egg-info/requires.txt
--rw-r--r--   0 cardiel    (501) staff       (20)        8 2024-02-03 10:10:50.000000 rgblues-1.3/rgblues.egg-info/top_level.txt
--rw-r--r--   0 cardiel    (501) staff       (20)      988 2024-02-03 10:10:50.076843 rgblues-1.3/setup.cfg
--rw-r--r--   0 cardiel    (501) staff       (20)       68 2022-11-05 19:26:58.000000 rgblues-1.3/setup.py
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-25 14:48:31.901517 rgblues-1.4/
+-rw-r--r--   0 cardiel    (501) staff       (20)    35149 2022-11-05 19:26:58.000000 rgblues-1.4/LICENSE
+-rw-r--r--   0 cardiel    (501) staff       (20)    11041 2024-04-25 14:48:31.901243 rgblues-1.4/PKG-INFO
+-rw-r--r--   0 cardiel    (501) staff       (20)    10111 2024-02-03 10:01:12.000000 rgblues-1.4/README.md
+-rw-r--r--   0 cardiel    (501) staff       (20)      100 2022-11-05 19:26:58.000000 rgblues-1.4/pyproject.toml
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-25 14:48:31.893053 rgblues-1.4/rgblues/
+-rw-r--r--   0 cardiel    (501) staff       (20)       51 2022-11-05 19:26:58.000000 rgblues-1.4/rgblues/__init__.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     7020 2022-11-05 19:26:58.000000 rgblues-1.4/rgblues/__main__.py
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-25 14:48:31.898750 rgblues-1.4/rgblues/core/
+-rw-r--r--   0 cardiel    (501) staff       (20)        0 2022-11-05 19:26:58.000000 rgblues-1.4/rgblues/core/__init__.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     2719 2024-04-25 14:47:39.000000 rgblues-1.4/rgblues/core/step1.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     3469 2022-11-05 19:26:58.000000 rgblues-1.4/rgblues/core/step2.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     1253 2022-11-05 19:26:58.000000 rgblues-1.4/rgblues/core/step3.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     2493 2024-04-25 14:47:39.000000 rgblues-1.4/rgblues/core/step4.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     2080 2022-11-05 19:26:58.000000 rgblues-1.4/rgblues/core/step5.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     2115 2022-11-05 19:26:58.000000 rgblues-1.4/rgblues/core/step6.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     5591 2022-11-05 19:26:58.000000 rgblues-1.4/rgblues/core/step7.py
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-25 14:48:31.900094 rgblues-1.4/rgblues/gui/
+-rw-r--r--   0 cardiel    (501) staff       (20)        0 2022-11-05 19:26:58.000000 rgblues-1.4/rgblues/gui/__init__.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     8492 2022-11-06 08:27:37.000000 rgblues-1.4/rgblues/gui/step8.py
+-rw-r--r--   0 cardiel    (501) staff       (20)      496 2022-11-05 19:26:58.000000 rgblues-1.4/rgblues/gui/style.py
+-rw-r--r--   0 cardiel    (501) staff       (20)      171 2024-04-25 14:47:39.000000 rgblues-1.4/rgblues/version.py
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-25 14:48:31.900623 rgblues-1.4/rgblues.egg-info/
+-rw-r--r--   0 cardiel    (501) staff       (20)    11041 2024-04-25 14:48:31.000000 rgblues-1.4/rgblues.egg-info/PKG-INFO
+-rw-r--r--   0 cardiel    (501) staff       (20)      543 2024-04-25 14:48:31.000000 rgblues-1.4/rgblues.egg-info/SOURCES.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)        1 2024-04-25 14:48:31.000000 rgblues-1.4/rgblues.egg-info/dependency_links.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)       50 2024-04-25 14:48:31.000000 rgblues-1.4/rgblues.egg-info/entry_points.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)       56 2024-04-25 14:48:31.000000 rgblues-1.4/rgblues.egg-info/requires.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)        8 2024-04-25 14:48:31.000000 rgblues-1.4/rgblues.egg-info/top_level.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)      988 2024-04-25 14:48:31.902330 rgblues-1.4/setup.cfg
+-rw-r--r--   0 cardiel    (501) staff       (20)       68 2022-11-05 19:26:58.000000 rgblues-1.4/setup.py
```

### Comparing `rgblues-1.3/LICENSE` & `rgblues-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rgblues-1.3/PKG-INFO` & `rgblues-1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgblues
-Version: 1.3
+Version: 1.4
 Summary: RGB from Gaia EDR3
 Home-page: https://github.com/guaix-ucm/rgblues
 Author: Nicolás Cardiel
 Author-email: cardiel@ucm.es
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `rgblues-1.3/README.md` & `rgblues-1.4/README.md`

 * *Files identical despite different names*

### Comparing `rgblues-1.3/rgblues/__main__.py` & `rgblues-1.4/rgblues/__main__.py`

 * *Files identical despite different names*

### Comparing `rgblues-1.3/rgblues/core/step1.py` & `rgblues-1.4/rgblues/core/step1.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright 2021 Universidad Complutense de Madrid
+# Copyright 2021-2024 Universidad Complutense de Madrid
 #
 # SPDX-License-Identifier: GPL-3.0+
 # License-Filename: LICENSE.txt
 #
 
 """
 Perform EDR3 query
@@ -79,8 +79,13 @@
     nstars_colorcut = len(r_edr3_colorcut)
     print(f'        --> {nstars_colorcut} stars outside -0.5 < G_BP-G_RP < 2.0')
     if nstars == 0:
         raise SystemExit('ERROR: no stars found. Change search parameters!')
     if verbose:
         r_edr3.pprint(max_width=1000)
 
+    # change the column labels to lowercase
+    # (important: the Gaia database has changed 'source_id' by 'SOURCE_ID')
+    new_colnames = [colname.lower() for colname in r_edr3.colnames]
+    r_edr3.rename_columns(r_edr3.colnames, new_colnames)
+
     return r_edr3, nstars, nstars_colorcut
```

### Comparing `rgblues-1.3/rgblues/core/step2.py` & `rgblues-1.4/rgblues/core/step2.py`

 * *Files identical despite different names*

### Comparing `rgblues-1.3/rgblues/core/step3.py` & `rgblues-1.4/rgblues/core/step3.py`

 * *Files identical despite different names*

### Comparing `rgblues-1.3/rgblues/core/step4.py` & `rgblues-1.4/rgblues/core/step4.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright 2021 Universidad Complutense de Madrid
+# Copyright 2021-2024 Universidad Complutense de Madrid
 #
 # SPDX-License-Identifier: GPL-3.0+
 # License-Filename: LICENSE.txt
 #
 
 """
 DR2 query to identify variable stars
@@ -69,8 +69,13 @@
             raise SystemExit('Unexpected type of data in column phot_variable_flag')
         nvariables = sum(mask_var)
         print(f'        --> {nstars_dr2} stars in DR2, ({nvariables} initial variables)')
     if nvariables > 0:
         if verbose:
             r_dr2[mask_var].pprint(max_width=1000)
 
+    # change the column labels to lowercase
+    # (important: the Gaia database has changed 'source_id' by 'SOURCE_ID')
+    new_colnames = [colname.lower() for colname in r_dr2.colnames]
+    r_dr2.rename_columns(r_dr2.colnames, new_colnames)
+
     return r_dr2, nvariables, mask_var
```

### Comparing `rgblues-1.3/rgblues/core/step5.py` & `rgblues-1.4/rgblues/core/step5.py`

 * *Files identical despite different names*

### Comparing `rgblues-1.3/rgblues/core/step6.py` & `rgblues-1.4/rgblues/core/step6.py`

 * *Files identical despite different names*

### Comparing `rgblues-1.3/rgblues/core/step7.py` & `rgblues-1.4/rgblues/core/step7.py`

 * *Files identical despite different names*

### Comparing `rgblues-1.3/rgblues/gui/step8.py` & `rgblues-1.4/rgblues/gui/step8.py`

 * *Files identical despite different names*

### Comparing `rgblues-1.3/rgblues.egg-info/PKG-INFO` & `rgblues-1.4/rgblues.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgblues
-Version: 1.3
+Version: 1.4
 Summary: RGB from Gaia EDR3
 Home-page: https://github.com/guaix-ucm/rgblues
 Author: Nicolás Cardiel
 Author-email: cardiel@ucm.es
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `rgblues-1.3/rgblues.egg-info/SOURCES.txt` & `rgblues-1.4/rgblues.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rgblues-1.3/setup.cfg` & `rgblues-1.4/setup.cfg`

 * *Files identical despite different names*

