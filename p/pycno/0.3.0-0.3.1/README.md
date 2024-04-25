# Comparing `tmp/pycno-0.3.0.tar.gz` & `tmp/pycno-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pycno-0.3.0.tar", last modified: Thu Sep 21 18:16:45 2023, max compression
+gzip compressed data, was "pycno-0.3.1.tar", last modified: Thu Apr 25 15:51:44 2024, max compression
```

## Comparing `pycno-0.3.0.tar` & `pycno-0.3.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-09-21 18:16:45.000000 pycno-0.3.0/
--rw-r--r--   0 bhenders (83225) romo       (131)     1055 2022-04-27 16:01:50.000000 pycno-0.3.0/setup.py
--rw-r--r--   0 bhenders (83225) romo       (131)     3588 2023-09-21 18:16:45.000000 pycno-0.3.0/PKG-INFO
--rw-r--r--   0 bhenders (83225) romo       (131)    35149 2020-08-17 14:41:39.000000 pycno-0.3.0/LICENSE
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-09-21 18:16:45.000000 pycno-0.3.0/pycno/
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-09-21 18:16:45.000000 pycno-0.3.0/pycno/util/
--rw-r--r--   0 bhenders (83225) romo       (131)       45 2021-11-03 21:34:22.000000 pycno-0.3.0/pycno/util/__init__.py
--rw-r--r--   0 bhenders (83225) romo       (131)     3145 2021-11-03 21:34:14.000000 pycno-0.3.0/pycno/util/shp2cno.py
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-09-21 18:16:45.000000 pycno-0.3.0/pycno/tests/
--rw-r--r--   0 bhenders (83225) romo       (131)        0 2020-08-17 18:47:57.000000 pycno-0.3.0/pycno/tests/__init__.py
--rw-r--r--   0 bhenders (83225) romo       (131)     4038 2023-09-21 17:50:07.000000 pycno-0.3.0/pycno/tests/test_cno.py
--rw-r--r--   0 bhenders (83225) romo       (131)    16212 2023-09-21 18:14:06.000000 pycno-0.3.0/pycno/__init__.py
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-09-21 18:16:45.000000 pycno-0.3.0/pycno/data/
--rw-r--r--   0 bhenders (83225) romo       (131)      325 2021-01-19 16:32:14.000000 pycno-0.3.0/pycno/data/README.md
--rw-r--r--   0 bhenders (83225) romo       (131)   217536 2014-04-08 02:14:09.000000 pycno-0.3.0/pycno/data/MWDB_Coasts_Countries_3.cnob
--rw-r--r--   0 bhenders (83225) romo       (131)      100 2021-01-19 16:46:46.000000 pycno-0.3.0/pycno/data/test.cnob
--rw-r--r--   0 bhenders (83225) romo       (131)       96 2021-01-19 16:48:08.000000 pycno-0.3.0/pycno/data/test.cno
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-09-21 18:16:45.000000 pycno-0.3.0/pycno.egg-info/
--rw-r--r--   0 bhenders (83225) romo       (131)      395 2023-09-21 18:16:45.000000 pycno-0.3.0/pycno.egg-info/SOURCES.txt
--rw-r--r--   0 bhenders (83225) romo       (131)     3588 2023-09-21 18:16:45.000000 pycno-0.3.0/pycno.egg-info/PKG-INFO
--rw-r--r--   0 bhenders (83225) romo       (131)        1 2023-09-21 18:16:45.000000 pycno-0.3.0/pycno.egg-info/dependency_links.txt
--rw-r--r--   0 bhenders (83225) romo       (131)        6 2023-09-21 18:16:45.000000 pycno-0.3.0/pycno.egg-info/top_level.txt
--rw-r--r--   0 bhenders (83225) romo       (131)       32 2023-09-21 18:16:45.000000 pycno-0.3.0/pycno.egg-info/requires.txt
--rw-r--r--   0 bhenders (83225) romo       (131)       38 2023-09-21 18:16:45.000000 pycno-0.3.0/setup.cfg
--rw-r--r--   0 bhenders (83225) romo       (131)     3006 2021-11-12 21:28:43.000000 pycno-0.3.0/README.md
--rw-r--r--   0 bhenders (83225) romo       (131)       21 2021-01-19 16:50:48.000000 pycno-0.3.0/MANIFEST.in
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2024-04-25 15:51:44.374070 pycno-0.3.1/
+-rw-r--r--   0 bhenders (83225) romo       (131)    35149 2020-08-17 14:41:39.000000 pycno-0.3.1/LICENSE
+-rw-r--r--   0 bhenders (83225) romo       (131)       21 2021-01-19 16:50:48.000000 pycno-0.3.1/MANIFEST.in
+-rw-r--r--   0 bhenders (83225) romo       (131)     3551 2024-04-25 15:51:44.373524 pycno-0.3.1/PKG-INFO
+-rw-r--r--   0 bhenders (83225) romo       (131)     3006 2021-11-12 21:28:43.000000 pycno-0.3.1/README.md
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2024-04-25 15:51:44.364540 pycno-0.3.1/pycno/
+-rw-r--r--   0 bhenders (83225) romo       (131)    16212 2024-04-25 15:48:24.000000 pycno-0.3.1/pycno/__init__.py
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2024-04-25 15:51:44.370820 pycno-0.3.1/pycno/data/
+-rw-r--r--   0 bhenders (83225) romo       (131)   217536 2014-04-08 02:14:09.000000 pycno-0.3.1/pycno/data/MWDB_Coasts_Countries_3.cnob
+-rw-r--r--   0 bhenders (83225) romo       (131)      325 2021-01-19 16:32:14.000000 pycno-0.3.1/pycno/data/README.md
+-rw-r--r--   0 bhenders (83225) romo       (131)       96 2021-01-19 16:48:08.000000 pycno-0.3.1/pycno/data/test.cno
+-rw-r--r--   0 bhenders (83225) romo       (131)      100 2021-01-19 16:46:46.000000 pycno-0.3.1/pycno/data/test.cnob
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2024-04-25 15:51:44.371933 pycno-0.3.1/pycno/tests/
+-rw-r--r--   0 bhenders (83225) romo       (131)        0 2020-08-17 18:47:57.000000 pycno-0.3.1/pycno/tests/__init__.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     4038 2023-09-21 17:50:07.000000 pycno-0.3.1/pycno/tests/test_cno.py
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2024-04-25 15:51:44.373126 pycno-0.3.1/pycno/util/
+-rw-r--r--   0 bhenders (83225) romo       (131)       45 2021-11-03 21:34:22.000000 pycno-0.3.1/pycno/util/__init__.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     3145 2021-11-03 21:34:14.000000 pycno-0.3.1/pycno/util/shp2cno.py
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2024-04-25 15:51:44.367163 pycno-0.3.1/pycno.egg-info/
+-rw-r--r--   0 bhenders (83225) romo       (131)     3551 2024-04-25 15:51:44.365193 pycno-0.3.1/pycno.egg-info/PKG-INFO
+-rw-r--r--   0 bhenders (83225) romo       (131)      395 2024-04-25 15:51:44.365693 pycno-0.3.1/pycno.egg-info/SOURCES.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)        1 2024-04-25 15:51:44.366177 pycno-0.3.1/pycno.egg-info/dependency_links.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)       32 2024-04-25 15:51:44.366715 pycno-0.3.1/pycno.egg-info/requires.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)        6 2024-04-25 15:51:44.367235 pycno-0.3.1/pycno.egg-info/top_level.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)       38 2024-04-25 15:51:44.374163 pycno-0.3.1/setup.cfg
+-rw-r--r--   0 bhenders (83225) romo       (131)     1219 2024-04-25 15:48:03.000000 pycno-0.3.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pycno-0.3.0/setup.py` & `pycno-0.3.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 import setuptools
+import os
+
+cachedir = os.path.expanduser('~/.pycno')
+try:
+    os.makedirs(cachedir, exist_ok=True)
+except Exception:
+    # could not install user cache
+    pass
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 with open("pycno/__init__.py", "r") as fh:
-    for l in fh:
-        if l.startswith('__version__'):
-            exec(l)
+    for _l in fh:
+        if _l.startswith('__version__'):
+            exec(_l)
             break
     else:
         __version__ = 'x.y.z'
 
 setuptools.setup(
     name="pycno",
     version=__version__,
```

### Comparing `pycno-0.3.0/PKG-INFO` & `pycno-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: pycno
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python map overlay software to read CNO and CNOB files.
 Home-page: https://github.com/barronh/pycno
 Author: Barron H. Henderson
 Author-email: barronh@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: proj
@@ -104,9 +102,7 @@
   preserve_units=True
 )
 plt.axis('image')
 cno = pycno.cno(proj=proj, xlim=(0, 187), ylim=(0, 187))
 cno.draw()
 plt.savefig('coasts_countries_ps.png')
 ```
-
-
```

### Comparing `pycno-0.3.0/LICENSE` & `pycno-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycno-0.3.0/pycno/util/shp2cno.py` & `pycno-0.3.1/pycno/util/shp2cno.py`

 * *Files identical despite different names*

### Comparing `pycno-0.3.0/pycno/tests/test_cno.py` & `pycno-0.3.1/pycno/tests/test_cno.py`

 * *Files identical despite different names*

### Comparing `pycno-0.3.0/pycno/__init__.py` & `pycno-0.3.1/pycno/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
 
 import os
 from pathlib import Path
 import warnings
 import numpy as np
 from . import util
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 
 _panoplyurl = 'https://www.giss.nasa.gov/tools/panoply/overlays/'
 _panoplycnobs = [
     'MWDB_Coasts_1.cnob',
     'MWDB_Coasts_3.cnob',
     'MWDB_Coasts_Countries_1.cnob',
     'MWDB_Coasts_Countries_3.cnob',
```

### Comparing `pycno-0.3.0/pycno/data/MWDB_Coasts_Countries_3.cnob` & `pycno-0.3.1/pycno/data/MWDB_Coasts_Countries_3.cnob`

 * *Files identical despite different names*

### Comparing `pycno-0.3.0/pycno.egg-info/PKG-INFO` & `pycno-0.3.1/pycno.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: pycno
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python map overlay software to read CNO and CNOB files.
 Home-page: https://github.com/barronh/pycno
 Author: Barron H. Henderson
 Author-email: barronh@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: proj
@@ -104,9 +102,7 @@
   preserve_units=True
 )
 plt.axis('image')
 cno = pycno.cno(proj=proj, xlim=(0, 187), ylim=(0, 187))
 cno.draw()
 plt.savefig('coasts_countries_ps.png')
 ```
-
-
```

### Comparing `pycno-0.3.0/README.md` & `pycno-0.3.1/README.md`

 * *Files identical despite different names*

