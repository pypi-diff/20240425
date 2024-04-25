# Comparing `tmp/cmaqsatproc-0.2.4.tar.gz` & `tmp/cmaqsatproc-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cmaqsatproc-0.2.4.tar", last modified: Fri Oct 13 14:39:53 2023, max compression
+gzip compressed data, was "cmaqsatproc-0.3.1.tar", last modified: Thu Apr 25 14:42:04 2024, max compression
```

## Comparing `cmaqsatproc-0.2.4.tar` & `cmaqsatproc-0.3.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-10-13 14:39:53.000000 cmaqsatproc-0.2.4/
--rw-r--r--   0 bhenders (83225) romo       (131)     1136 2023-10-13 14:39:48.000000 cmaqsatproc-0.2.4/setup.py
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-10-13 14:39:53.000000 cmaqsatproc-0.2.4/cmaqsatproc.egg-info/
--rw-r--r--   0 bhenders (83225) romo       (131)     1011 2023-10-13 14:39:52.000000 cmaqsatproc-0.2.4/cmaqsatproc.egg-info/SOURCES.txt
--rw-r--r--   0 bhenders (83225) romo       (131)     7078 2023-10-13 14:39:52.000000 cmaqsatproc-0.2.4/cmaqsatproc.egg-info/PKG-INFO
--rw-r--r--   0 bhenders (83225) romo       (131)        1 2023-10-13 14:39:52.000000 cmaqsatproc-0.2.4/cmaqsatproc.egg-info/dependency_links.txt
--rw-r--r--   0 bhenders (83225) romo       (131)       12 2023-10-13 14:39:52.000000 cmaqsatproc-0.2.4/cmaqsatproc.egg-info/top_level.txt
--rw-r--r--   0 bhenders (83225) romo       (131)       82 2023-10-13 14:39:52.000000 cmaqsatproc-0.2.4/cmaqsatproc.egg-info/requires.txt
--rw-r--r--   0 bhenders (83225) romo       (131)     7078 2023-10-13 14:39:53.000000 cmaqsatproc-0.2.4/PKG-INFO
--rw-r--r--   0 bhenders (83225) romo       (131)    35149 2019-06-14 15:58:09.000000 cmaqsatproc-0.2.4/LICENSE
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-10-13 14:39:53.000000 cmaqsatproc-0.2.4/cmaqsatproc/
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-10-13 14:39:53.000000 cmaqsatproc-0.2.4/cmaqsatproc/tests/
--rw-r--r--   0 bhenders (83225) romo       (131)     4684 2022-10-13 17:44:09.000000 cmaqsatproc-0.2.4/cmaqsatproc/tests/test_omihcho.py
--rw-r--r--   0 bhenders (83225) romo       (131)     3608 2022-10-13 17:44:09.000000 cmaqsatproc-0.2.4/cmaqsatproc/tests/test_omino2.py
--rw-r--r--   0 bhenders (83225) romo       (131)        0 2022-10-13 17:44:09.000000 cmaqsatproc-0.2.4/cmaqsatproc/tests/__init__.py
--rw-r--r--   0 bhenders (83225) romo       (131)     2344 2022-10-13 17:44:09.000000 cmaqsatproc-0.2.4/cmaqsatproc/tests/test_utils.py
--rw-r--r--   0 bhenders (83225) romo       (131)      687 2022-10-13 17:44:09.000000 cmaqsatproc-0.2.4/cmaqsatproc/tests/test_cmaq.py
--rw-r--r--   0 bhenders (83225) romo       (131)     4333 2022-10-13 17:44:09.000000 cmaqsatproc-0.2.4/cmaqsatproc/tests/test_mod04.py
--rw-r--r--   0 bhenders (83225) romo       (131)     2914 2022-10-13 17:44:09.000000 cmaqsatproc-0.2.4/cmaqsatproc/tests/test_satellite.py
--rw-r--r--   0 bhenders (83225) romo       (131)    25139 2023-10-13 14:38:24.000000 cmaqsatproc-0.2.4/cmaqsatproc/cmaq.py
--rw-r--r--   0 bhenders (83225) romo       (131)      379 2023-02-07 21:21:07.000000 cmaqsatproc-0.2.4/cmaqsatproc/__init__.py
--rw-r--r--   0 bhenders (83225) romo       (131)     9554 2022-12-05 21:28:43.000000 cmaqsatproc-0.2.4/cmaqsatproc/utils.py
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-10-13 14:39:53.000000 cmaqsatproc-0.2.4/cmaqsatproc/drivers/
--rw-r--r--   0 bhenders (83225) romo       (131)     1377 2022-10-13 17:44:09.000000 cmaqsatproc-0.2.4/cmaqsatproc/drivers/__init__.py
--rw-r--r--   0 bhenders (83225) romo       (131)     5573 2022-10-13 17:44:09.000000 cmaqsatproc-0.2.4/cmaqsatproc/drivers/localdisk.py
--rw-r--r--   0 bhenders (83225) romo       (131)        0 2022-10-13 17:44:09.000000 cmaqsatproc-0.2.4/cmaqsatproc/drivers/optutils.py
--rw-r--r--   0 bhenders (83225) romo       (131)     6266 2022-10-13 17:44:09.000000 cmaqsatproc-0.2.4/cmaqsatproc/drivers/opendap.py
--rw-r--r--   0 bhenders (83225) romo       (131)      153 2022-10-13 17:44:09.000000 cmaqsatproc-0.2.4/cmaqsatproc/__main__.py
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-10-13 14:39:53.000000 cmaqsatproc-0.2.4/cmaqsatproc/readers/
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-10-13 14:39:53.000000 cmaqsatproc-0.2.4/cmaqsatproc/readers/goes/
--rw-r--r--   0 bhenders (83225) romo       (131)     8859 2022-10-14 10:59:05.000000 cmaqsatproc-0.2.4/cmaqsatproc/readers/goes/__init__.py
--rw-r--r--   0 bhenders (83225) romo       (131)     1453 2022-10-13 17:44:09.000000 cmaqsatproc-0.2.4/cmaqsatproc/readers/__init__.py
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-10-13 14:39:53.000000 cmaqsatproc-0.2.4/cmaqsatproc/readers/omi/
--rw-r--r--   0 bhenders (83225) romo       (131)    31120 2022-10-13 17:44:09.000000 cmaqsatproc-0.2.4/cmaqsatproc/readers/omi/__init__.py
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-10-13 14:39:53.000000 cmaqsatproc-0.2.4/cmaqsatproc/readers/omps/
--rw-r--r--   0 bhenders (83225) romo       (131)    10373 2022-10-13 17:44:09.000000 cmaqsatproc-0.2.4/cmaqsatproc/readers/omps/__init__.py
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-10-13 14:39:53.000000 cmaqsatproc-0.2.4/cmaqsatproc/readers/iasi/
--rw-r--r--   0 bhenders (83225) romo       (131)     4066 2022-10-13 17:44:09.000000 cmaqsatproc-0.2.4/cmaqsatproc/readers/iasi/__init__.py
--rw-r--r--   0 bhenders (83225) romo       (131)    20144 2022-10-22 13:57:20.000000 cmaqsatproc-0.2.4/cmaqsatproc/readers/core.py
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-10-13 14:39:53.000000 cmaqsatproc-0.2.4/cmaqsatproc/readers/tropomi/
--rw-r--r--   0 bhenders (83225) romo       (131)    34123 2022-11-21 15:39:16.000000 cmaqsatproc-0.2.4/cmaqsatproc/readers/tropomi/__init__.py
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-10-13 14:39:53.000000 cmaqsatproc-0.2.4/cmaqsatproc/readers/viirs/
--rw-r--r--   0 bhenders (83225) romo       (131)    14053 2022-10-13 17:44:09.000000 cmaqsatproc-0.2.4/cmaqsatproc/readers/viirs/__init__.py
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-10-13 14:39:53.000000 cmaqsatproc-0.2.4/cmaqsatproc/readers/modis/
--rw-r--r--   0 bhenders (83225) romo       (131)    11325 2022-11-21 15:57:28.000000 cmaqsatproc-0.2.4/cmaqsatproc/readers/modis/__init__.py
--rw-r--r--   0 bhenders (83225) romo       (131)     3959 2022-10-13 17:44:09.000000 cmaqsatproc-0.2.4/cmaqsatproc/readers/modis/modis_readers.py
--rw-r--r--   0 bhenders (83225) romo       (131)       38 2023-10-13 14:39:53.000000 cmaqsatproc-0.2.4/setup.cfg
--rw-r--r--   0 bhenders (83225) romo       (131)     6483 2023-06-02 18:25:28.000000 cmaqsatproc-0.2.4/README.md
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2024-04-25 14:42:04.333778 cmaqsatproc-0.3.1/
+-rw-r--r--   0 bhenders (83225) romo       (131)    35149 2019-06-14 15:58:09.000000 cmaqsatproc-0.3.1/LICENSE
+-rw-r--r--   0 bhenders (83225) romo       (131)     7041 2024-04-25 14:42:04.333487 cmaqsatproc-0.3.1/PKG-INFO
+-rw-r--r--   0 bhenders (83225) romo       (131)     6483 2023-06-02 18:25:28.000000 cmaqsatproc-0.3.1/README.md
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2024-04-25 14:42:04.316780 cmaqsatproc-0.3.1/cmaqsatproc/
+-rw-r--r--   0 bhenders (83225) romo       (131)     2418 2024-04-25 14:39:31.000000 cmaqsatproc-0.3.1/cmaqsatproc/__init__.py
+-rw-r--r--   0 bhenders (83225) romo       (131)      153 2022-10-13 17:44:09.000000 cmaqsatproc-0.3.1/cmaqsatproc/__main__.py
+-rw-r--r--   0 bhenders (83225) romo       (131)    25663 2024-04-24 20:05:04.000000 cmaqsatproc-0.3.1/cmaqsatproc/cmaq.py
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2024-04-25 14:42:04.322130 cmaqsatproc-0.3.1/cmaqsatproc/drivers/
+-rw-r--r--   0 bhenders (83225) romo       (131)     1377 2022-10-13 17:44:09.000000 cmaqsatproc-0.3.1/cmaqsatproc/drivers/__init__.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     5573 2022-10-13 17:44:09.000000 cmaqsatproc-0.3.1/cmaqsatproc/drivers/localdisk.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     6333 2023-10-13 15:24:00.000000 cmaqsatproc-0.3.1/cmaqsatproc/drivers/opendap.py
+-rw-r--r--   0 bhenders (83225) romo       (131)        0 2022-10-13 17:44:09.000000 cmaqsatproc-0.3.1/cmaqsatproc/drivers/optutils.py
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2024-04-25 14:42:04.323213 cmaqsatproc-0.3.1/cmaqsatproc/readers/
+-rw-r--r--   0 bhenders (83225) romo       (131)     1453 2022-10-13 17:44:09.000000 cmaqsatproc-0.3.1/cmaqsatproc/readers/__init__.py
+-rw-r--r--   0 bhenders (83225) romo       (131)    20254 2024-01-26 18:59:06.000000 cmaqsatproc-0.3.1/cmaqsatproc/readers/core.py
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2024-04-25 14:42:04.323928 cmaqsatproc-0.3.1/cmaqsatproc/readers/goes/
+-rw-r--r--   0 bhenders (83225) romo       (131)     8859 2022-10-14 10:59:05.000000 cmaqsatproc-0.3.1/cmaqsatproc/readers/goes/__init__.py
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2024-04-25 14:42:04.325099 cmaqsatproc-0.3.1/cmaqsatproc/readers/iasi/
+-rw-r--r--   0 bhenders (83225) romo       (131)     4066 2022-10-13 17:44:09.000000 cmaqsatproc-0.3.1/cmaqsatproc/readers/iasi/__init__.py
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2024-04-25 14:42:04.326677 cmaqsatproc-0.3.1/cmaqsatproc/readers/modis/
+-rw-r--r--   0 bhenders (83225) romo       (131)    11361 2024-03-06 16:30:54.000000 cmaqsatproc-0.3.1/cmaqsatproc/readers/modis/__init__.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     3959 2022-10-13 17:44:09.000000 cmaqsatproc-0.3.1/cmaqsatproc/readers/modis/modis_readers.py
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2024-04-25 14:42:04.327220 cmaqsatproc-0.3.1/cmaqsatproc/readers/omi/
+-rw-r--r--   0 bhenders (83225) romo       (131)    31899 2024-03-06 16:42:50.000000 cmaqsatproc-0.3.1/cmaqsatproc/readers/omi/__init__.py
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2024-04-25 14:42:04.327863 cmaqsatproc-0.3.1/cmaqsatproc/readers/omps/
+-rw-r--r--   0 bhenders (83225) romo       (131)    10385 2024-03-06 16:39:26.000000 cmaqsatproc-0.3.1/cmaqsatproc/readers/omps/__init__.py
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2024-04-25 14:42:04.328434 cmaqsatproc-0.3.1/cmaqsatproc/readers/tropomi/
+-rw-r--r--   0 bhenders (83225) romo       (131)    33246 2024-03-07 18:03:51.000000 cmaqsatproc-0.3.1/cmaqsatproc/readers/tropomi/__init__.py
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2024-04-25 14:42:04.329072 cmaqsatproc-0.3.1/cmaqsatproc/readers/viirs/
+-rw-r--r--   0 bhenders (83225) romo       (131)    14045 2024-03-06 16:32:07.000000 cmaqsatproc-0.3.1/cmaqsatproc/readers/viirs/__init__.py
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2024-04-25 14:42:04.333086 cmaqsatproc-0.3.1/cmaqsatproc/tests/
+-rw-r--r--   0 bhenders (83225) romo       (131)        0 2022-10-13 17:44:09.000000 cmaqsatproc-0.3.1/cmaqsatproc/tests/__init__.py
+-rw-r--r--   0 bhenders (83225) romo       (131)      687 2022-10-13 17:44:09.000000 cmaqsatproc-0.3.1/cmaqsatproc/tests/test_cmaq.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     4333 2022-10-13 17:44:09.000000 cmaqsatproc-0.3.1/cmaqsatproc/tests/test_mod04.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     4684 2022-10-13 17:44:09.000000 cmaqsatproc-0.3.1/cmaqsatproc/tests/test_omihcho.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     3608 2022-10-13 17:44:09.000000 cmaqsatproc-0.3.1/cmaqsatproc/tests/test_omino2.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     2914 2022-10-13 17:44:09.000000 cmaqsatproc-0.3.1/cmaqsatproc/tests/test_satellite.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     2344 2022-10-13 17:44:09.000000 cmaqsatproc-0.3.1/cmaqsatproc/tests/test_utils.py
+-rw-r--r--   0 bhenders (83225) romo       (131)    10731 2024-03-07 18:18:11.000000 cmaqsatproc-0.3.1/cmaqsatproc/utils.py
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2024-04-25 14:42:04.319554 cmaqsatproc-0.3.1/cmaqsatproc.egg-info/
+-rw-r--r--   0 bhenders (83225) romo       (131)     7041 2024-04-25 14:42:03.000000 cmaqsatproc-0.3.1/cmaqsatproc.egg-info/PKG-INFO
+-rw-r--r--   0 bhenders (83225) romo       (131)     1011 2024-04-25 14:42:03.000000 cmaqsatproc-0.3.1/cmaqsatproc.egg-info/SOURCES.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)        1 2024-04-25 14:42:03.000000 cmaqsatproc-0.3.1/cmaqsatproc.egg-info/dependency_links.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)       75 2024-04-25 14:42:03.000000 cmaqsatproc-0.3.1/cmaqsatproc.egg-info/requires.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)       12 2024-04-25 14:42:03.000000 cmaqsatproc-0.3.1/cmaqsatproc.egg-info/top_level.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)       38 2024-04-25 14:42:04.334044 cmaqsatproc-0.3.1/setup.cfg
+-rw-r--r--   0 bhenders (83225) romo       (131)     1126 2024-04-25 14:36:30.000000 cmaqsatproc-0.3.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cmaqsatproc-0.2.4/setup.py` & `cmaqsatproc-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,13 +26,13 @@
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Development Status :: 2 - Pre-Alpha",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     install_requires=[
         "numpy", "matplotlib", "pandas", "geopandas", "xarray", "pyproj",
-        "shapely", "pygeos", "pycno"
+        "shapely", "pycno"
     ],
     extras_require={
         "gdal":  ["gdal"],
     }
 )
```

### Comparing `cmaqsatproc-0.2.4/cmaqsatproc.egg-info/SOURCES.txt` & `cmaqsatproc-0.3.1/cmaqsatproc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cmaqsatproc-0.2.4/cmaqsatproc.egg-info/PKG-INFO` & `cmaqsatproc-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: cmaqsatproc
-Version: 0.2.4
+Version: 0.3.1
 Summary: Processor to grid satellite data for comparison to CMAQ.
 Home-page: https://github.com/barronh/cmaqsatproc
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
 Provides-Extra: gdal
@@ -218,9 +216,7 @@
     style cmaqsatproc fill:#cefad0,stroke:#cefad0,stroke-width:4px
     style csplabel fill:#cefad0,stroke:#cefad0,stroke-width:4px
 ```
 
 ## References
 
 Henderson, B. H. (2022, October 17). cmaqsatproc v2: Satellite data processing for CMAQ [Poster]. 21st Annual Community Modeling and Analysis System Conference, Chapel Hill, NC. https://www.cmascenter.org/conference/2022/agenda.cfm; [direct link](https://www.cmascenter.org/conference/2022/slides/Henderson_satellite-data-CMAS2022.pdf)
-
-
```

### Comparing `cmaqsatproc-0.2.4/PKG-INFO` & `cmaqsatproc-0.3.1/cmaqsatproc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: cmaqsatproc
-Version: 0.2.4
+Version: 0.3.1
 Summary: Processor to grid satellite data for comparison to CMAQ.
 Home-page: https://github.com/barronh/cmaqsatproc
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
 Provides-Extra: gdal
@@ -218,9 +216,7 @@
     style cmaqsatproc fill:#cefad0,stroke:#cefad0,stroke-width:4px
     style csplabel fill:#cefad0,stroke:#cefad0,stroke-width:4px
 ```
 
 ## References
 
 Henderson, B. H. (2022, October 17). cmaqsatproc v2: Satellite data processing for CMAQ [Poster]. 21st Annual Community Modeling and Analysis System Conference, Chapel Hill, NC. https://www.cmascenter.org/conference/2022/agenda.cfm; [direct link](https://www.cmascenter.org/conference/2022/slides/Henderson_satellite-data-CMAS2022.pdf)
-
-
```

### Comparing `cmaqsatproc-0.2.4/LICENSE` & `cmaqsatproc-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cmaqsatproc-0.2.4/cmaqsatproc/tests/test_omihcho.py` & `cmaqsatproc-0.3.1/cmaqsatproc/tests/test_omihcho.py`

 * *Files identical despite different names*

### Comparing `cmaqsatproc-0.2.4/cmaqsatproc/tests/test_omino2.py` & `cmaqsatproc-0.3.1/cmaqsatproc/tests/test_omino2.py`

 * *Files identical despite different names*

### Comparing `cmaqsatproc-0.2.4/cmaqsatproc/tests/test_utils.py` & `cmaqsatproc-0.3.1/cmaqsatproc/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cmaqsatproc-0.2.4/cmaqsatproc/tests/test_cmaq.py` & `cmaqsatproc-0.3.1/cmaqsatproc/tests/test_cmaq.py`

 * *Files identical despite different names*

### Comparing `cmaqsatproc-0.2.4/cmaqsatproc/tests/test_mod04.py` & `cmaqsatproc-0.3.1/cmaqsatproc/tests/test_mod04.py`

 * *Files identical despite different names*

### Comparing `cmaqsatproc-0.2.4/cmaqsatproc/tests/test_satellite.py` & `cmaqsatproc-0.3.1/cmaqsatproc/tests/test_satellite.py`

 * *Files identical despite different names*

### Comparing `cmaqsatproc-0.2.4/cmaqsatproc/cmaq.py` & `cmaqsatproc-0.3.1/cmaqsatproc/cmaq.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,19 +71,31 @@
 'NAQFC_CONUS'
 'LamCon_25N_95W' -4226153.11044303 -834746.472325356 5079.0 5079.0  1473 1025 1
 ' '"""
 
 
 def griddesc(griddesc_txt):
     from collections import OrderedDict
+    import re
     gddefns = OrderedDict()
     prjdefns = OrderedDict()
-    # lines with ' ' are separators
+    # Clean up GRIDDESC
+    # Replace commas with spaces
+    griddesc_txt = griddesc_txt.replace(',', ' ')
+    # Remove comments prefixed by !
+    griddesc_txt = '\n'.join([
+        gdl.split('!')[0].strip()
+        for gdl in griddesc_txt.split('\n')
+    ])
+    dble = re.compile('([\d.])[Dd]([\d])')
+    griddesc_txt = dble.sub(r'\1e\2', griddesc_txt)
+    # lines with ' ' are separators and blank shouldn't happen
     reallines = [
-        l for l in griddesc_txt.split('\n') if l.strip() not in ("''", "' '")
+        l for l in griddesc_txt.split('\n')
+        if l.strip() not in ("''", "' '", "")
     ]
     # All definitions come in pairs of lines. The first is the name and the
     # second is either all numeric for projections or, for grids, a string
     #  projection name followed by numeric grid definitions
     prjattrkeys = ['GDTYP', 'P_ALP', 'P_BET', 'P_GAM', 'XCENT', 'YCENT']
     gdattrkeys = [
         'PRJNAME', 'XORIG', 'YORIG', 'XCELL', 'YCELL', 'NCOLS',
@@ -281,15 +293,18 @@
             qf = self._obj
         else:
             qf = self._obj.copy()
 
         if 'TFLAG' in qf.data_vars:
             tflag = qf.data_vars['TFLAG'][:, 0].values.copy()
             if (tflag[:, 0] < 1).all():
-                tflag[:, 0] = 1970001
+                sdate = qf.attrs.get('SDATE', 0)
+                if sdate < 1:
+                    sdate = 1970001
+                tflag[:, 0] = sdate
             times = pd.to_datetime([
                 datetime.strptime(f'{JDATE}T{TIME:06d}', '%Y%jT%H%M%S')
                 for JDATE, TIME in tflag
             ])
         elif 'TSTEP' in qf.coords:
             tstep = qf.coords['TSTEP']
             if tstep.size == 1:
@@ -301,36 +316,36 @@
                 ) for t in tstep
             ]
         else:
             SDATE = qf.SDATE
             if SDATE < 1:
                 SDATE = 1970001
             date = datetime.strptime(f'{SDATE}T{qf.STIME:06d}', '%Y%jT%H%M%S')
-            nt = qf.dims['TSTEP']
+            nt = qf.sizes['TSTEP']
             dm = (qf.attrs['TSTEP'] % 10000) // 100
             ds = (qf.attrs['TSTEP'] % 100)
             dh = qf.attrs['TSTEP'] // 10000 + dm / 60 + ds / 3600.
             if nt == 1 and dh == 0:
                 dh = 1
-            times = pd.date_range(date, periods=nt, freq=f'{dh}H')
+            times = pd.date_range(date, periods=nt, freq=f'{dh}h')
 
         qf.coords['TSTEP'] = times
         if 'VGLVLS' in qf.attrs:
             qf.coords['LAY'] = (qf.VGLVLS[1:] + qf.VGLVLS[:-1]) / 2
 
         crs = get_proj4string(qf.attrs)
         if crs is None:
             warnings.warn((
                 'Unknown project ({GDTYP}); currently support lonlat (1),'
                 + ' lcc (2), polar stereograpic (6), equatorial mercator (7)'
             ).format(GDTYP=qf.attrs['GDTYP']))
         else:
             qf.attrs['crs'] = crs
-            row = np.arange(qf.dims['ROW']) + 0.5
-            col = np.arange(qf.dims['COL']) + 0.5
+            row = np.arange(qf.sizes['ROW']) + 0.5
+            col = np.arange(qf.sizes['COL']) + 0.5
             if qf.GDTYP == 1:
                 row = row * qf.attrs['YCELL'] + qf.attrs['YORIG']
                 col = col * qf.attrs['XCELL'] + qf.attrs['XORIG']
             qf.coords['ROW'] = row
             qf.coords['COL'] = col
 
         return qf
@@ -363,15 +378,15 @@
             )
             defattrs.update(outf[k].attrs)
             outf[k].attrs.update(defattrs)
 
         outkeys = [k for k in outf.data_vars if k != 'TFLAG']
         nv = np.int32(len(outkeys))
 
-        nl = np.int32(outf.dims.get('LAY', 1))
+        nl = np.int32(outf.sizes.get('LAY', 1))
         vglvls = np.linspace(0, 1, nl + 1, dtype='f')[::-1]
         vgtyp = np.int32(-9999)
         vgtop = np.float32(5000)
         sdate = np.int32(-635)
 
         defattrs = {
             'EXEC_ID': 'NA'.ljust(80), 'IOAPI_VERSION': 'NA'.ljust(80),
```

### Comparing `cmaqsatproc-0.2.4/cmaqsatproc/utils.py` & `cmaqsatproc-0.3.1/cmaqsatproc/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,56 +24,82 @@
     return outputs
 
 
 def grouped_weighted_avg(values, weights, by):
     numerator = values.multiply(
         weights, axis=0
     ).groupby(by).sum()
-    denominator = weights.groupby(by).sum()
+    wgb = weights.groupby(by)
+    denominator = wgb.sum()
+    simplemean = wgb.mean()
+    count = wgb.count()
     outdf = numerator.divide(denominator, axis=0)
     outdf['weight_sum'] = denominator
+    outdf['weight_mean'] = simplemean
+    outdf['count'] = count
     return outdf
 
 
 def getcmrgranules(
-    short_name, temporal, bbox=None, poly=None, verbose=0, **kwds
+    temporal, bbox=None, poly=None, verbose=0, **kwds
 ):
     """
     Return all links from the Common Metadata Repository for the product
     granules with short_name, date_range, and optionally a bounding box.
 
     Arguments
     ---------
-    short_name : str
-        NASA short_name that is recognized by NASA Common Metadata Repository
     temporal : str
         NASA temporal that is recognized by NASA Common Metadata Repository
         i.e, YYYY-MM-DDTHH:MM:SSZ or YYYY-MM-DDTHH:MM:SSZ/YYYY-MM-DDTHH:MM:SSZ
         or YYYY-MM-DDTHH:MM:SSZ/P01D (or P01M or P01Y) etc.
     bbox : list
         Longitude/latitude bounding edges as floats (wlon,slat,elon,nlat)
     poly : shapely.geometry.Polygon
         The exterior will be converted to floats and ordered x1,y1,...,xN,yN
     filterfunc : function
         Takes a link dictionary from CMR and returns True if it should be
         retained
-
+    concept_id : str
+        Optional, NASA concept_id that is the unique identifier for a
+        collection in NASA's Common Metadata Repository
+    short_name : str
+        Optional, short_name identifier for a collection that is often, but
+        not always unique in the NASA Common Metadata Repository. If you have
+        the short_name and want the concept_id put the url below in your
+        browser where you replace OMNO2 (the example) with your short_name
+        https://cmr.earthdata.nasa.gov/search/collections?short_name=OMNO2
     Returns
     -------
     jr : dictionary
         json result as a dictionary
     """
     from copy import deepcopy
     import requests
+    import warnings
 
     opts = deepcopy(kwds)
     opts.setdefault('page_size', '1000')
     opts.setdefault('pretty', 'false')
-    opts['short_name'] = short_name
     opts['temporal'] = temporal
+    if opts.get('concept_id', None) is None:
+        if 'short_name' in opts:
+            short_name = opts['short_name']
+            msg = (
+                'short_name not guaranteed unique. Try the concept_id keyword'
+                + ' instead of short_name. Potential values for concept_id can'
+                + '  be found at: https://cmr.earthdata.nasa.gov/search/'
+                + f'collections?short_name={short_name}'
+            )
+        else:
+            msg = (
+                'Queries are best with at least short_name and preferrably'
+                + ' concept_id'
+            )
+        warnings.warn(msg)
 
     if bbox is not None:
         opts['bounding_box'] = '{:f},{:f},{:f},{:f}'.format(*bbox)
 
     if poly is not None:
         import numpy as np
         from shapely.geometry import polygon
```

### Comparing `cmaqsatproc-0.2.4/cmaqsatproc/drivers/__init__.py` & `cmaqsatproc-0.3.1/cmaqsatproc/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `cmaqsatproc-0.2.4/cmaqsatproc/drivers/localdisk.py` & `cmaqsatproc-0.3.1/cmaqsatproc/drivers/localdisk.py`

 * *Files identical despite different names*

### Comparing `cmaqsatproc-0.2.4/cmaqsatproc/drivers/opendap.py` & `cmaqsatproc-0.3.1/cmaqsatproc/drivers/opendap.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,16 @@
     gdpath : str or None
         if str, a path to a GRIDDESC file.
     SDATE : str
         Any date-like starting date for CMR query
     EDATE : str
         Any date-like starting date for CMR query
     outpath : str
-        path to write out result; If None, default {reader}_{gdnam}.csv
+        path to write out result; If None, the default path is
+        {reader}_{SDATE}_{EDATE}_{gdnam}.nc
     overwrite : bool
         Overwrite existing files?
 
     Results
     -------
     None :
         Outputs are written to disk.
@@ -93,15 +94,16 @@
     EDATE : str
         Any date-like starting date for CMR query
     variables : list
         Variables to write out.
     geo : bool
         Write geometry as a WKT polygon
     outpath : str
-        path to write out result; If None, default {reader}_{gdnam}.csv
+        path to write out result; If None, default path is
+        {reader}_{SDATE}_{EDATE}_{gdnam}.csv
     overwrite : bool
         Overwrite existing files?
 
     Results
     -------
     None :
         Outputs are written to disk.
```

### Comparing `cmaqsatproc-0.2.4/cmaqsatproc/readers/goes/__init__.py` & `cmaqsatproc-0.3.1/cmaqsatproc/readers/goes/__init__.py`

 * *Files identical despite different names*

### Comparing `cmaqsatproc-0.2.4/cmaqsatproc/readers/__init__.py` & `cmaqsatproc-0.3.1/cmaqsatproc/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `cmaqsatproc-0.2.4/cmaqsatproc/readers/omi/__init__.py` & `cmaqsatproc-0.3.1/cmaqsatproc/readers/omi/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,32 @@
 __all__ = ['OMIL2', 'OMNO2', 'OMHCHO', 'OMPROFOZ', 'OMO3PR']
 
 from ..core import satellite
 from ...utils import walk_groups
 
 
+def cloudleq(cldf, thresh):
+    """
+    Check if cloud is less than or equal to thresh.
+
+    This is a convenience function to deal with he5 files having a different
+    metadata than their OpenDAP counterparts.
+    """
+    cldval = cldf.load()
+    scale = cldf.attrs.get('ScaleFactor', 1)
+    offset = cldf.attrs.get('Offset', 0)
+    if scale != 1 or offset != 0:
+        cldval = cldval * scale + offset
+    elif cldval.mean() > 100 and thresh < 1:
+        import warnings
+        warnings.warn('Cloud scaled by 0.001 because avg > 100 and limit < 1')
+        cldval = cldval * 0.001
+    return cldval <= thresh
+
+
 class OMIL2(satellite):
     __doc__ = """
     Default OMI satellite processor.
     * bbox subsets the nTimes and nTimes_1  dimensions
     """
 
     @classmethod
@@ -231,29 +250,29 @@
         'ScatteringWeight', 'ScatteringWtPressure', 'TropopausePressure',
         'TerrainPressure',
     )
 
     @classmethod
     def cmr_links(cls, method='opendap', **kwds):
         """
-        Thin wrapper around satellite.cmr_links where short_name is set to
-        "OMNO2".
+        Thin wrapper around satellite.cmr_links where concept_id is set to
+        "C1239966842-GES_DISC".
 
         Arguments
         ---------
         method : str
             'opendap', 'download', or 's3'. 's3' is not supported for OMI at
             this time.
 
         Returns
         -------
         links : list
             List of links for download or OpenDAP
         """
-        kwds.setdefault('short_name', 'OMNO2')
+        kwds.setdefault('concept_id', 'C1239966842-GES_DISC')
         return OMIL2.cmr_links(method=method, **kwds)
 
     @classmethod
     def open_dataset(cls, path, bbox=None, **kwargs):
         """
         Arguments
         ---------
@@ -280,15 +299,15 @@
         for key, corner in corners.items():
             ds[f'{key}_x'] = ds['FoV75CornerLongitude'].sel(nCorners=corner)
             ds[f'{key}_y'] = ds['FoV75CornerLatitude'].sel(nCorners=corner)
 
         ds['valid'] = (
             ((ds['VcdQualityFlags'].astype('i') & 1) == 0)
             & (ds['XTrackQualityFlags'] == 0)
-            & (ds['CloudFraction'] <= 0.3)
+            & cloudleq(ds['CloudFraction'], 0.3)
         )
         if bbox is not None:
             swlon, swlat, nelon, nelat = bbox
             ds['valid'] = (
                 ds['valid']
                 & (ds['Latitude'] >= swlat) & (ds['Latitude'] <= nelat)
                 & (ds['Longitude'] >= swlon) & (ds['Longitude'] <= nelon)
@@ -459,29 +478,29 @@
         'ColumnAmount', 'ReferenceSectorCorrectedVerticalColumn',
         'AirMassFactor', 'ScatteringWeights', 'ClimatologyLevels'
     )
 
     @classmethod
     def cmr_links(cls, method='opendap', **kwds):
         """
-        Thin wrapper around satellite.cmr_links where short_name is set to
-        "OMHCHO".
+        Thin wrapper around satellite.cmr_links where concept_id is set to
+        "C1239966779-GES_DISC".
 
         Arguments
         ---------
         method : str
             'opendap', 'download', or 's3'. 's3' is not supported for OMI at
             this time.
 
         Returns
         -------
         links : list
             List of links for download or OpenDAP
         """
-        kwds.setdefault('short_name', 'OMHCHO')
+        kwds.setdefault('concept_id', 'C1239966779-GES_DISC')
         return OMIL2.cmr_links(method=method, **kwds)
 
     @classmethod
     def open_dataset(cls, path, bbox=None, **kwargs):
         """
         Arguments
         ---------
@@ -500,15 +519,15 @@
         """
         import xarray as xr
         omtmp = OMIL2.open_dataset(path, bbox=bbox, **kwargs)
         ds = omtmp.ds
         ds['valid'] = (
             (ds['MainDataQualityFlag'] == 0)
             & ((ds['XtrackQualityFlagsExpanded'].astype('i') & 1) == 0)
-            & (ds['AMFCloudFraction'] <= 0.3)
+            & cloudleq(ds['AMFCloudFraction'], 0.3)
         )
         ds['cn_x'] = ds['Longitude']
         ds['cn_y'] = ds['Latitude']
 
         if bbox is not None:
             swlon, swlat, nelon, nelat = bbox
             ds['valid'] = (
@@ -695,29 +714,29 @@
     _defaultkeys = (
         'O3', 'AveragingKernel', 'O3APriori', 'Pressure'
     )
 
     @classmethod
     def cmr_links(cls, method='opendap', **kwds):
         """
-        Thin wrapper around satellite.cmr_links where short_name is set to
-        "OMO3PR".
+        Thin wrapper around satellite.cmr_links where concept_id is set to
+        "C1239966827-GES_DISC".
 
         Arguments
         ---------
         method : str
             'opendap', 'download', or 's3'. 's3' is not supported for OMI at
             this time.
 
         Returns
         -------
         links : list
             List of links for download or OpenDAP
         """
-        kwds.setdefault('short_name', 'OMO3PR')
+        kwds.setdefault('concept_id', 'C1239966827-GES_DISC')
         return OMIL2.cmr_links(method=method, **kwds)
 
     @classmethod
     def open_dataset(cls, path, bbox=None, **kwargs):
         """
         Arguments
         ---------
@@ -822,27 +841,28 @@
         'AirMassFactor', 'ScatteringWeights', 'ClimatologyLevels'
     )
 
     @classmethod
     def cmr_links(cls, method='opendap', **kwds):
         """
         Thin wrapper around satellite.cmr_links where short_name is set to
-        "OMO3PR".
+        "OMPROFOZ".
 
         Arguments
         ---------
         method : str
             'opendap', 'download', or 's3'. 's3' is not supported for OMI at
             this time.
 
         Returns
         -------
         links : list
             List of links for download or OpenDAP
         """
+        # BHH : not sure this product exists in the CMR
         kwds.setdefault('short_name', 'OMPROFOZ')
         return OMIL2.cmr_links(method=method, **kwds)
 
     @classmethod
     def open_dataset(cls, path, bbox=None, **kwargs):
         """
         Arguments
@@ -863,15 +883,15 @@
         import xarray as xr
         omtmp = OMIL2.open_dataset(path, bbox=bbox, **kwargs)
         ds = omtmp.ds
         ds['valid'] = ~(
             (ds['ExitStatus'] <= 0) | (ds['ExitStatus'] >= 10)
             | (ds['RMS'].max('nChannel') > 3)
             | (ds['AverageResiduals'].max('nChannel') >= 3)
-            | (ds['EffectiveCloudFraction'] >= 0.3)
+            | ~cloudleq(ds['EffectiveCloudFraction'], 0.3)
         )
         ds['cn_x'] = ds['Longitude']
         ds['cn_y'] = ds['Latitude']
 
         if bbox is not None:
             swlon, swlat, nelon, nelat = bbox
             ds['valid'] = (
```

### Comparing `cmaqsatproc-0.2.4/cmaqsatproc/readers/omps/__init__.py` & `cmaqsatproc-0.3.1/cmaqsatproc/readers/omps/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,30 +212,30 @@
       * GroundPixelQualityFlags == 0
       * PixelQualityFlags == 0
     """
 
     @classmethod
     def cmr_links(cls, method='opendap', **kwargs):
         """
-        Thin wrapper around satellite.cmr_links where short_name is set to
-        "OMPS_NPP_NMNO2_L2".
+        Thin wrapper around satellite.cmr_links where concept_id is set to
+        "C1386443916-GES_DISC".
 
         Arguments
         ---------
         method : str
             'opendap', 'download', or 's3'.
 
         Returns
         -------
         links : list
             List of links for download or OpenDAP
         """
         from copy import copy
         kwargs = copy(kwargs)
-        kwargs.setdefault('short_name', 'OMPS_NPP_NMNO2_L2')
+        kwargs.setdefault('concept_id', 'C1386443916-GES_DISC')
         return OMPS_NPP_L2.cmr_links(method=method, **kwargs)
 
     @classmethod
     def prep_dataset(cls, ds, bbox=None, path=None):
         """
         Defines valid based on Latitude/Longitude and bbox, and inteprolates
         pixel centers to corners. Then further subsets valid pixels where
@@ -307,24 +307,24 @@
             warnings.warn('No valid pixels')
 
         return ds
 
     @classmethod
     def cmr_links(cls, method='opendap', **kwargs):
         """
-        Thin wrapper around satellite.cmr_links where short_name is set to
-        "OMPS_NPP_NMTO3_L2".
+        Thin wrapper around satellite.cmr_links where concept_id is set to
+        "C1386443916-GES_DISC".
 
         Arguments
         ---------
         method : str
             'opendap', 'download', or 's3'.
 
         Returns
         -------
         links : list
             List of links for download or OpenDAP
         """
         from copy import copy
         kwargs = copy(kwargs)
-        kwargs.setdefault('short_name', 'OMPS_NPP_NMTO3_L2')
+        kwargs.setdefault('concept_id', 'C1386443916-GES_DISC')
         return OMPS_NPP_L2.cmr_links(method=method, **kwargs)
```

### Comparing `cmaqsatproc-0.2.4/cmaqsatproc/readers/iasi/__init__.py` & `cmaqsatproc-0.3.1/cmaqsatproc/readers/iasi/__init__.py`

 * *Files identical despite different names*

### Comparing `cmaqsatproc-0.2.4/cmaqsatproc/readers/core.py` & `cmaqsatproc-0.3.1/cmaqsatproc/readers/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -372,14 +372,15 @@
                 if verbose > 1:
                     print(' - Adding intx geometry', flush=True)
                     t0 = time.time()
                 if len(notgeodims) > 0:
                     if verbose > 1:
                         print(f'   - Unstacking {notgeodims}', flush=True)
                     mjustweight = justweight.copy()
+                    ckey = ('count',) + ('',) * len(notgeodims)
                     wkey = ('weight',) + ('',) * len(notgeodims)
                     wskey = ('weight_sum',) + ('',) * len(notgeodims)
                     mjustweight.columns = pd.MultiIndex.from_tuples(
                         [wkey], names=[None] + notgeodims
                     )
                     df = mjustweight.join(df.unstack(notgeodims))
                 else:
@@ -406,14 +407,15 @@
                 gdf = grouped_weighted_avg(
                     df, df[wkey], outdims
                 )
                 if len(notgeodims) > 0:
                     ngdf = gdf.drop([wkey, wskey], axis=1).stack(notgeodims)
                     ngdf['weight'] = gdf[wkey]
                     ngdf['weight_sum'] = gdf[wskey]
+                    ngdf['count'] = gdf[ckey]
                     gdf = ngdf
             else:
                 gdf = self.to_dataframe(*keys, geo=False, valid=False)
                 # tmpgrid = grid.drop('geometry', axis=1).copy()
                 # tmpgrid['none'] = 1
                 # gdf = tmpgrid.set_index('none', append=True).join(
                 #     df.set_index('none', append=True)
```

### Comparing `cmaqsatproc-0.2.4/cmaqsatproc/readers/tropomi/__init__.py` & `cmaqsatproc-0.3.1/cmaqsatproc/readers/tropomi/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -390,38 +390,31 @@
     * bbox subsets the scanline dimensions
     * valid = qa_value >= threshold (default 0.75)
     """
 
     @classmethod
     def cmr_links(cls, method='opendap', **kwargs):
         """
-        Thin wrapper around satellite.cmr_links where short_name is set to
-        "S5P_L2__CO____" or "S5P_L2__CO_____HiR".
-
-        The HiR product started 2019-08-06T02:41:41.000Z
+        Thin wrapper around satellite.cmr_links where concept_id is set to
+        "C2087132178-GES_DISC", which is the HiR product v2. The HiR v2
+        product starts 2018-04-30.
 
         Arguments
         ---------
         method : str
             'opendap', 'download', or 's3'.
 
         Returns
         -------
         links : list
             List of links for download or OpenDAP
         """
         from copy import copy
         kwargs = copy(kwargs)
-        hirstartdate = '2019-08-06'
-        querydate = kwargs.get('temporal', hirstartdate)[:10]
-        if querydate >= hirstartdate:
-            defshortname = 'S5P_L2__CO_____HiR'
-        else:
-            defshortname = 'S5P_L2__CO____'
-        kwargs.setdefault('short_name', defshortname)
+        kwargs.setdefault('concept_id', 'C2087132178-GES_DISC')
         return TropOMI.cmr_links(method=method, **kwargs)
 
     @classmethod
     def cmaq_process(cls, qf, l3, key='CO'):
         """
         Process CMAQ as though it were observed by TropOMI, which is simply
         based on the overpass time.
@@ -517,38 +510,31 @@
     * bbox subsets the scanline dimensions
     * valid = qa_value >= threshold (default 0.75)
     """
 
     @classmethod
     def cmr_links(cls, method='opendap', **kwargs):
         """
-        Thin wrapper around satellite.cmr_links where short_name is set to
-        "S5P_L2__NO2___" or "S5P_L2__NO2____HiR".
-
-        "S5P_L2__NO2____HiR" starts 2019-08-06T02:41:41.000Z
+        Thin wrapper around satellite.cmr_links where concept_id is set to
+        "C2089270961-GES_DISC", which is the HiR v2 product. The HiR v2
+        product starts 2018-05-01.
 
         Arguments
         ---------
         method : str
             'opendap', 'download', or 's3'.
 
         Returns
         -------
         links : list
             List of links for download or OpenDAP
         """
         from copy import copy
         kwargs = copy(kwargs)
-        hirstartdate = '2019-08-06'
-        querydate = kwargs.get('temporal', hirstartdate)[:10]
-        if querydate >= hirstartdate:
-            defshortname = 'S5P_L2__NO2____HiR'
-        else:
-            defshortname = 'S5P_L2__NO2___'
-        kwargs.setdefault('short_name', defshortname)
+        kwargs.setdefault('concept_id', 'C2089270961-GES_DISC')
         return TropOMI.cmr_links(method=method, **kwargs)
 
     @classmethod
     def cmaq_sw(
         cls, overf, satl3f, amfkey='air_mass_factor_total',
         tropopausekey='tm5_tropopause_layer_index'
     ):
@@ -697,48 +683,44 @@
             'TropOMI_NO2 x TropOMI_AMF / CMAQ_AMF'
         ).ljust(80)
 
         return overf
 
 
 class S5P_L2__CH4___(TropOMI):
-    _defaultkeys = ('methane_mixing_ratio', 'averaging_kernel')
+    _defaultkeys = (
+        'methane_mixing_ratio', 'methane_mixing_ratio_bias_corrected',
+        'averaging_kernel'
+    )
     __doc__ = """
     TropOMICH4 satellite processor.
     * bbox subsets the scanline dimensions
     * valid = qa_value >= threshold (default 0.75)
     """
 
     @classmethod
     def cmr_links(cls, method='opendap', **kwargs):
         """
-        Thin wrapper around satellite.cmr_links where short_name is set to
-        "S5P_L2__CH4___" or "S5P_L2__CH4____HiR".
-
-        The HiR product started 2019-08-06T02:41:41.000Z
+        Thin wrapper around satellite.cmr_links where concept_id is set to
+        "C2087216530-GES_DISC", which is the HiR v2 product. The HiR product
+        started 2018-04-30.
 
         Arguments
         ---------
         method : str
             'opendap', 'download', or 's3'.
 
         Returns
         -------
         links : list
             List of links for download or OpenDAP
         """
         from copy import copy
         kwargs = copy(kwargs)
-        hirstartdate = '2019-08-06'
-        querydate = kwargs.get('temporal', hirstartdate)[:10]
-        if querydate >= hirstartdate:
-            defshortname = 'S5P_L2__CH4____HiR'
-        else:
-            defshortname = 'S5P_L2__CH4___'
-        kwargs.setdefault('short_name', defshortname)
+        kwargs.setdefault('concept_id', 'C2087216530-GES_DISC')
         return TropOMI.cmr_links(method=method, **kwargs)
 
     @classmethod
     def cmaq_process(cls, qf, l3, key='CH4'):
         """
         Process CMAQ as though it were observed by TropOMI, which is simply
         based on the overpass time.
@@ -775,38 +757,31 @@
         'formaldehyde_tropospheric_vertical_column',
         'surface_pressure'
     )
 
     @classmethod
     def cmr_links(cls, method='opendap', **kwargs):
         """
-        Thin wrapper around satellite.cmr_links where short_name is set to
-        "S5P_L2__HCHO__" or "S5P_L2__HCHO___HiR".
-
-        "S5P_L2_HCHO___HiR" starts 2019-08-06T02:41:41.000Z
+        Thin wrapper around satellite.cmr_links where concept_id is set to
+        "C1918210023-GES_DISC", which is the HiR v2 product. The HiR v2 product
+        starts in 2018-05-07.
 
         Arguments
         ---------
         method : str
             'opendap', 'download', or 's3'.
 
         Returns
         -------
         links : list
             List of links for download or OpenDAP
         """
         from copy import copy
         kwargs = copy(kwargs)
-        hirstartdate = '2019-08-06'
-        querydate = kwargs.get('temporal', hirstartdate)[:10]
-        if querydate >= hirstartdate:
-            defshortname = 'S5P_L2__HCHO___HiR'
-        else:
-            defshortname = 'S5P_L2__HCHO__'
-        kwargs.setdefault('short_name', defshortname)
+        kwargs.setdefault('concept_id', 'C1918210023-GES_DISC')
         return TropOMI.cmr_links(method=method, **kwargs)
 
     @classmethod
     def cmaq_sw(
         cls, overf, satl3f, amfkey='formaldehyde_tropospheric_air_mass_factor'
     ):
         """
```

### Comparing `cmaqsatproc-0.2.4/cmaqsatproc/readers/viirs/__init__.py` & `cmaqsatproc-0.3.1/cmaqsatproc/readers/viirs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,30 +146,30 @@
     * valid = Land_Ocean_Quality_Flag > isvalid (default 2)
     * pixel corners are based on interpolated lat/lon
     """
 
     @classmethod
     def cmr_links(cls, method='opendap', **kwargs):
         """
-        Thin wrapper around L2_VIIRS_SNPP.cmr_links with short_name set to
-        AERDT_L2_VIIRS_SNPP.
+        Thin wrapper around L2_VIIRS_SNPP.cmr_links with concept_id set to
+        C1688453112-LAADS.
 
         Arguments
         ---------
         method : str
             'opendap', 'download', or 's3'.
 
         Returns
         -------
         links : list
             List of links for download or OpenDAP or s3
         """
         from copy import copy
         kwargs = copy(kwargs)
-        kwargs.setdefault('short_name', 'AERDT_L2_VIIRS_SNPP')
+        kwargs.setdefault('concept_id', 'C1688453112-LAADS')
         return L2_VIIRS_SNPP.cmr_links(method=method, **kwargs)
 
     @classmethod
     def prep_dataset(cls, ds, bbox=None, isvalid=2, path=None):
         """
         Applies spatial subset based on Latitude and Longitude, also
         interpolates pixel centers to corners and applies valid flags:
@@ -290,30 +290,30 @@
         'Aerosol_Optical_Thickness_QA_Flag_Ocean',
         'Aerosol_Optical_Thickness_QA_Flag_Land'
     )
 
     @classmethod
     def cmr_links(cls, method='opendap', **kwargs):
         """
-        Thin wrapper around L2_VIIRS_SNPP.cmr_links with short_name set to
-        AERDT_L2_VIIRS_SNPP.
+        Thin wrapper around L2_VIIRS_SNPP.cmr_links with concept_id set to
+        C2600303218-LAADS.
 
         Arguments
         ---------
         method : str
             'opendap', 'download', or 's3'.
 
         Returns
         -------
         links : list
             List of links for download or OpenDAP or s3
         """
         from copy import copy
         kwargs = copy(kwargs)
-        kwargs.setdefault('short_name', 'AERDB_L2_VIIRS_SNPP')
+        kwargs.setdefault('concept_id', 'C2600303218-LAADS')
         return L2_VIIRS_SNPP.cmr_links(method=method, **kwargs)
 
     @classmethod
     def prep_dataset(cls, ds, bbox=None, isvalid=2, path=None):
         """
         Applies spatial subset based on Latitude and Longitude, also
         interpolates pixel centers to corners and applies valid flags:
```

### Comparing `cmaqsatproc-0.2.4/cmaqsatproc/readers/modis/__init__.py` & `cmaqsatproc-0.3.1/cmaqsatproc/readers/modis/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -130,69 +130,69 @@
         sat.ds = ds
         sat.bbox = bbox
         return sat
 
 
 class MOD04_L2(MOD04):
     __doc__ = """
-    MOD04_L3 filters valid pixels and provides weights for destination polygon:
+    MOD04_L2 filters valid pixels and provides weights for destination polygon:
     * valid = Land_Ocean_Quality_Flag > 1 and value == value
     * pixel_area = corners from centroids +- delta
     * weight = intx_fracarea
     """
 
     @classmethod
     def cmr_links(cls, method='opendap', **kwargs):
         """
-        Thin wrapper around satellite.cmr_links where short_name is set to
-        "MOD04_L2".
+        Thin wrapper around satellite.cmr_links where concept_id is set to
+        "C1443533440-LAADS".
 
         Arguments
         ---------
         method : str
             'opendap', 'download', or 's3'.
 
         Returns
         -------
         links : list
             List of links for download or OpenDAP
         """
         from copy import copy
         kwargs = copy(kwargs)
-        kwargs.setdefault('short_name', 'MOD04_L2')
+        kwargs.setdefault('concept_id', 'C1443533440-LAADS')
         return MOD04.cmr_links(method=method, **kwargs)
 
 
 class MOD04_3K(MOD04):
     __doc__ = """
     MOD04_3K filters valid pixels and provides weights for destination polygon:
     * valid = Land_Ocean_Quality_Flag > 1 and value == value
     * pixel_area = corners from centroids +- delta
     * weight = intx_fracarea
     """
 
     @classmethod
     def cmr_links(cls, method='opendap', **kwargs):
         """
-        Thin wrapper around satellite.cmr_links where short_name is set to
-        "MOD04_3K".
+        Thin wrapper around satellite.cmr_links where concept_id is set to
+        "C1443420430-LAADS".
 
         Arguments
         ---------
         method : str
             'opendap', 'download', or 's3'.
 
         Returns
         -------
         links : list
             List of links for download or OpenDAP
         """
         from copy import copy
         kwargs = copy(kwargs)
-        kwargs.setdefault('short_name', 'MOD04_3K')
+        kwargs.setdefault('concept_id', 'C1443420430-LAADS')
         return MOD04.cmr_links(method=method, **kwargs)
 
 
 class MODISL3(satellite):
     __doc__ = """
     MODISL3 filters valid pixels and provides weights for
     destination polygon:
```

### Comparing `cmaqsatproc-0.2.4/cmaqsatproc/readers/modis/modis_readers.py` & `cmaqsatproc-0.3.1/cmaqsatproc/readers/modis/modis_readers.py`

 * *Files identical despite different names*

### Comparing `cmaqsatproc-0.2.4/README.md` & `cmaqsatproc-0.3.1/README.md`

 * *Files identical despite different names*

