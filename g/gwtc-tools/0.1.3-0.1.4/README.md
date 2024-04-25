# Comparing `tmp/gwtc_tools-0.1.3.tar.gz` & `tmp/gwtc_tools-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwtc_tools-0.1.3.tar", last modified: Fri Apr 19 09:49:02 2024, max compression
+gzip compressed data, was "gwtc_tools-0.1.4.tar", last modified: Thu Apr 25 14:00:47 2024, max compression
```

## Comparing `gwtc_tools-0.1.3.tar` & `gwtc_tools-0.1.4.tar`

### file list

```diff
@@ -1,50 +1,47 @@
-drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-04-19 09:49:02.452489 gwtc_tools-0.1.3/
--rw-r--r--   0 channa     (502) staff       (20)       97 2023-11-02 15:10:15.000000 gwtc_tools-0.1.3/.gitignore
--rw-r--r--   0 channa     (502) staff       (20)      865 2024-04-17 16:37:35.000000 gwtc_tools-0.1.3/.gitlab-ci.yml
--rw-r--r--   0 channa     (502) staff       (20)      677 2023-11-02 15:10:15.000000 gwtc_tools-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0 channa     (502) staff       (20)     1078 2023-11-02 15:10:15.000000 gwtc_tools-0.1.3/LICENSE.md
--rw-r--r--   0 channa     (502) staff       (20)     7305 2024-04-19 09:49:02.452294 gwtc_tools-0.1.3/PKG-INFO
--rw-r--r--   0 channa     (502) staff       (20)     6339 2024-04-17 16:37:35.000000 gwtc_tools-0.1.3/README.md
-drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-04-19 09:49:02.433540 gwtc_tools-0.1.3/docs/
--rw-r--r--   0 channa     (502) staff       (20)      638 2023-11-02 15:10:15.000000 gwtc_tools-0.1.3/docs/Makefile
--rw-r--r--   0 channa     (502) staff       (20)      804 2023-11-02 15:10:15.000000 gwtc_tools-0.1.3/docs/make.bat
--rw-r--r--   0 channa     (502) staff       (20)       59 2024-04-17 16:37:35.000000 gwtc_tools-0.1.3/docs/requirements.txt
-drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-04-19 09:49:02.434905 gwtc_tools-0.1.3/docs/source/
-drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-04-19 09:49:02.436158 gwtc_tools-0.1.3/docs/source/_templates/
--rw-r--r--   0 channa     (502) staff       (20)      662 2023-11-02 15:10:15.000000 gwtc_tools-0.1.3/docs/source/_templates/custom-class-template.rst
--rw-r--r--   0 channa     (502) staff       (20)     1408 2023-11-02 15:10:15.000000 gwtc_tools-0.1.3/docs/source/_templates/custom-module-template.rst
--rw-r--r--   0 channa     (502) staff       (20)     2507 2023-11-02 15:10:15.000000 gwtc_tools-0.1.3/docs/source/conf.py
--rw-r--r--   0 channa     (502) staff       (20)      484 2023-11-02 15:10:15.000000 gwtc_tools-0.1.3/docs/source/index.rst
-drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-04-19 09:49:02.442933 gwtc_tools-0.1.3/examples/
--rw-r--r--   0 channa     (502) staff       (20)     1415 2023-11-02 15:10:15.000000 gwtc_tools-0.1.3/examples/H1-GSTLAL_AllSky-1368009034-0.xml.gz
--rw-r--r--   0 channa     (502) staff       (20)     1440 2024-04-17 16:37:35.000000 gwtc_tools-0.1.3/examples/H1L1-GSTLAL_AllSky-1376883065-0.xml.gz
--rw-r--r--   0 channa     (502) staff       (20)   115407 2024-04-17 16:37:35.000000 gwtc_tools-0.1.3/examples/H1L1-SPIIR_AllSky-1376883065-0.xml.gz
--rw-r--r--   0 channa     (502) staff       (20)       91 2024-04-17 16:37:35.000000 gwtc_tools-0.1.3/examples/H1L1-SPIIR_AllSky_PASTRO-1376883065-0.json
--rw-r--r--   0 channa     (502) staff       (20)     1416 2023-11-02 15:10:15.000000 gwtc_tools-0.1.3/examples/L1-GSTLAL_AllSky-1368783503-0.xml.gz
--rw-r--r--   0 channa     (502) staff       (20)       58 2024-04-17 16:37:35.000000 gwtc_tools-0.1.3/examples/L1-GSTLAL_AllSky_PASTRO-1368783503-0.json
--rw-r--r--   0 channa     (502) staff       (20)     3460 2024-04-17 16:37:35.000000 gwtc_tools-0.1.3/examples/README.md
--rw-r--r--   0 channa     (502) staff       (20)      114 2024-04-17 16:37:35.000000 gwtc_tools-0.1.3/examples/gstlalv1.yaml
--rw-r--r--   0 channa     (502) staff       (20)      212 2024-04-17 16:37:35.000000 gwtc_tools-0.1.3/examples/gstlalv2.yaml
--rw-r--r--   0 channa     (502) staff       (20)     1653 2024-04-19 09:48:23.000000 gwtc_tools-0.1.3/pyproject.toml
--rw-r--r--   0 channa     (502) staff       (20)      855 2024-04-19 09:49:02.453609 gwtc_tools-0.1.3/setup.cfg
--rw-r--r--   0 channa     (502) staff       (20)       92 2023-11-02 15:10:15.000000 gwtc_tools-0.1.3/setup.py
-drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-04-19 09:49:02.428260 gwtc_tools-0.1.3/src/
-drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-04-19 09:49:02.444329 gwtc_tools-0.1.3/src/catalog_pipeline/
--rw-r--r--   0 channa     (502) staff       (20)       51 2024-04-17 16:37:35.000000 gwtc_tools-0.1.3/src/catalog_pipeline/__init__.py
--rw-r--r--   0 channa     (502) staff       (20)     5835 2024-04-17 16:37:35.000000 gwtc_tools-0.1.3/src/catalog_pipeline/aggregate_data.py
-drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-04-19 09:49:02.448018 gwtc_tools-0.1.3/src/gwtc/
--rw-r--r--   0 channa     (502) staff       (20)      324 2024-04-17 16:37:35.000000 gwtc_tools-0.1.3/src/gwtc/__init__.py
--rw-r--r--   0 channa     (502) staff       (20)      444 2024-04-19 09:49:02.000000 gwtc_tools-0.1.3/src/gwtc/_version.py
--rw-r--r--   0 channa     (502) staff       (20)    10091 2024-04-17 16:37:35.000000 gwtc_tools-0.1.3/src/gwtc/gwtc.py
--rwxr-xr-x   0 channa     (502) staff       (20)     1301 2024-04-17 16:37:35.000000 gwtc_tools-0.1.3/src/gwtc/gwtc_create_from_query.py
--rwxr-xr-x   0 channa     (502) staff       (20)     1480 2024-04-17 16:37:35.000000 gwtc_tools-0.1.3/src/gwtc/gwtc_diff.py
--rwxr-xr-x   0 channa     (502) staff       (20)     2516 2024-04-17 16:37:35.000000 gwtc_tools-0.1.3/src/gwtc/gwtc_get_gevent_coinc_files.py
--rw-r--r--   0 channa     (502) staff       (20)     8723 2024-04-17 16:37:35.000000 gwtc_tools-0.1.3/src/gwtc/gwtc_gracedb.py
--rwxr-xr-x   0 channa     (502) staff       (20)     4337 2024-04-17 16:37:35.000000 gwtc_tools-0.1.3/src/gwtc/gwtc_update_pipeline_gevents.py
-drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-04-19 09:49:02.451404 gwtc_tools-0.1.3/src/gwtc_tools.egg-info/
--rw-r--r--   0 channa     (502) staff       (20)     7305 2024-04-19 09:49:02.000000 gwtc_tools-0.1.3/src/gwtc_tools.egg-info/PKG-INFO
--rw-r--r--   0 channa     (502) staff       (20)     1174 2024-04-19 09:49:02.000000 gwtc_tools-0.1.3/src/gwtc_tools.egg-info/SOURCES.txt
--rw-r--r--   0 channa     (502) staff       (20)        1 2024-04-19 09:49:02.000000 gwtc_tools-0.1.3/src/gwtc_tools.egg-info/dependency_links.txt
--rw-r--r--   0 channa     (502) staff       (20)      315 2024-04-19 09:49:02.000000 gwtc_tools-0.1.3/src/gwtc_tools.egg-info/entry_points.txt
--rw-r--r--   0 channa     (502) staff       (20)       28 2024-04-19 09:49:02.000000 gwtc_tools-0.1.3/src/gwtc_tools.egg-info/requires.txt
--rw-r--r--   0 channa     (502) staff       (20)       22 2024-04-19 09:49:02.000000 gwtc_tools-0.1.3/src/gwtc_tools.egg-info/top_level.txt
+drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-04-25 14:00:47.647720 gwtc_tools-0.1.4/
+-rw-r--r--   0 channa     (502) staff       (20)       97 2023-11-02 15:10:15.000000 gwtc_tools-0.1.4/.gitignore
+-rw-r--r--   0 channa     (502) staff       (20)      865 2024-04-17 16:37:35.000000 gwtc_tools-0.1.4/.gitlab-ci.yml
+-rw-r--r--   0 channa     (502) staff       (20)      677 2023-11-02 15:10:15.000000 gwtc_tools-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0 channa     (502) staff       (20)     1078 2023-11-02 15:10:15.000000 gwtc_tools-0.1.4/LICENSE.md
+-rw-r--r--   0 channa     (502) staff       (20)     1861 2024-04-25 14:00:47.647525 gwtc_tools-0.1.4/PKG-INFO
+-rw-r--r--   0 channa     (502) staff       (20)      918 2024-04-25 13:54:01.000000 gwtc_tools-0.1.4/README.md
+drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-04-25 14:00:47.627680 gwtc_tools-0.1.4/docs/
+-rw-r--r--   0 channa     (502) staff       (20)      638 2023-11-02 15:10:15.000000 gwtc_tools-0.1.4/docs/Makefile
+-rw-r--r--   0 channa     (502) staff       (20)      804 2023-11-02 15:10:15.000000 gwtc_tools-0.1.4/docs/make.bat
+-rw-r--r--   0 channa     (502) staff       (20)       59 2024-04-17 16:37:35.000000 gwtc_tools-0.1.4/docs/requirements.txt
+drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-04-25 14:00:47.628979 gwtc_tools-0.1.4/docs/source/
+drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-04-25 14:00:47.630451 gwtc_tools-0.1.4/docs/source/_templates/
+-rw-r--r--   0 channa     (502) staff       (20)      662 2023-11-02 15:10:15.000000 gwtc_tools-0.1.4/docs/source/_templates/custom-class-template.rst
+-rw-r--r--   0 channa     (502) staff       (20)     1408 2023-11-02 15:10:15.000000 gwtc_tools-0.1.4/docs/source/_templates/custom-module-template.rst
+-rw-r--r--   0 channa     (502) staff       (20)     2507 2023-11-02 15:10:15.000000 gwtc_tools-0.1.4/docs/source/conf.py
+-rw-r--r--   0 channa     (502) staff       (20)      484 2023-11-02 15:10:15.000000 gwtc_tools-0.1.4/docs/source/index.rst
+drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-04-25 14:00:47.636656 gwtc_tools-0.1.4/examples/
+-rw-r--r--   0 channa     (502) staff       (20)     1415 2023-11-02 15:10:15.000000 gwtc_tools-0.1.4/examples/H1-GSTLAL_AllSky-1368009034-0.xml.gz
+-rw-r--r--   0 channa     (502) staff       (20)     1440 2024-04-17 16:37:35.000000 gwtc_tools-0.1.4/examples/H1L1-GSTLAL_AllSky-1376883065-0.xml.gz
+-rw-r--r--   0 channa     (502) staff       (20)   115407 2024-04-17 16:37:35.000000 gwtc_tools-0.1.4/examples/H1L1-SPIIR_AllSky-1376883065-0.xml.gz
+-rw-r--r--   0 channa     (502) staff       (20)       91 2024-04-17 16:37:35.000000 gwtc_tools-0.1.4/examples/H1L1-SPIIR_AllSky_PASTRO-1376883065-0.json
+-rw-r--r--   0 channa     (502) staff       (20)     1416 2023-11-02 15:10:15.000000 gwtc_tools-0.1.4/examples/L1-GSTLAL_AllSky-1368783503-0.xml.gz
+-rw-r--r--   0 channa     (502) staff       (20)       58 2024-04-17 16:37:35.000000 gwtc_tools-0.1.4/examples/L1-GSTLAL_AllSky_PASTRO-1368783503-0.json
+-rw-r--r--   0 channa     (502) staff       (20)     5286 2024-04-25 13:54:01.000000 gwtc_tools-0.1.4/examples/README.md
+-rw-r--r--   0 channa     (502) staff       (20)      114 2024-04-17 16:37:35.000000 gwtc_tools-0.1.4/examples/gstlalv1.yaml
+-rw-r--r--   0 channa     (502) staff       (20)      212 2024-04-17 16:37:35.000000 gwtc_tools-0.1.4/examples/gstlalv2.yaml
+-rw-r--r--   0 channa     (502) staff       (20)     1571 2024-04-25 13:55:59.000000 gwtc_tools-0.1.4/pyproject.toml
+-rw-r--r--   0 channa     (502) staff       (20)      855 2024-04-25 14:00:47.648797 gwtc_tools-0.1.4/setup.cfg
+-rw-r--r--   0 channa     (502) staff       (20)       92 2023-11-02 15:10:15.000000 gwtc_tools-0.1.4/setup.py
+drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-04-25 14:00:47.621195 gwtc_tools-0.1.4/src/
+drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-04-25 14:00:47.642619 gwtc_tools-0.1.4/src/gwtc/
+-rw-r--r--   0 channa     (502) staff       (20)      324 2024-04-17 16:37:35.000000 gwtc_tools-0.1.4/src/gwtc/__init__.py
+-rw-r--r--   0 channa     (502) staff       (20)      464 2024-04-25 14:00:47.000000 gwtc_tools-0.1.4/src/gwtc/_version.py
+-rw-r--r--   0 channa     (502) staff       (20)    10091 2024-04-17 16:37:35.000000 gwtc_tools-0.1.4/src/gwtc/gwtc.py
+-rwxr-xr-x   0 channa     (502) staff       (20)     1301 2024-04-17 16:37:35.000000 gwtc_tools-0.1.4/src/gwtc/gwtc_create_from_query.py
+-rwxr-xr-x   0 channa     (502) staff       (20)     1480 2024-04-17 16:37:35.000000 gwtc_tools-0.1.4/src/gwtc/gwtc_diff.py
+-rwxr-xr-x   0 channa     (502) staff       (20)     2516 2024-04-17 16:37:35.000000 gwtc_tools-0.1.4/src/gwtc/gwtc_get_gevent_coinc_files.py
+-rw-r--r--   0 channa     (502) staff       (20)     8723 2024-04-17 16:37:35.000000 gwtc_tools-0.1.4/src/gwtc/gwtc_gracedb.py
+-rwxr-xr-x   0 channa     (502) staff       (20)     4337 2024-04-17 16:37:35.000000 gwtc_tools-0.1.4/src/gwtc/gwtc_update_pipeline_gevents.py
+drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-04-25 14:00:47.646669 gwtc_tools-0.1.4/src/gwtc_tools.egg-info/
+-rw-r--r--   0 channa     (502) staff       (20)     1861 2024-04-25 14:00:47.000000 gwtc_tools-0.1.4/src/gwtc_tools.egg-info/PKG-INFO
+-rw-r--r--   0 channa     (502) staff       (20)     1102 2024-04-25 14:00:47.000000 gwtc_tools-0.1.4/src/gwtc_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 channa     (502) staff       (20)        1 2024-04-25 14:00:47.000000 gwtc_tools-0.1.4/src/gwtc_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 channa     (502) staff       (20)      253 2024-04-25 14:00:47.000000 gwtc_tools-0.1.4/src/gwtc_tools.egg-info/entry_points.txt
+-rw-r--r--   0 channa     (502) staff       (20)       20 2024-04-25 14:00:47.000000 gwtc_tools-0.1.4/src/gwtc_tools.egg-info/requires.txt
+-rw-r--r--   0 channa     (502) staff       (20)        5 2024-04-25 14:00:47.000000 gwtc_tools-0.1.4/src/gwtc_tools.egg-info/top_level.txt
```

### Comparing `gwtc_tools-0.1.3/.gitlab-ci.yml` & `gwtc_tools-0.1.4/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.3/.pre-commit-config.yaml` & `gwtc_tools-0.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.3/LICENSE.md` & `gwtc_tools-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.3/docs/Makefile` & `gwtc_tools-0.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.3/docs/make.bat` & `gwtc_tools-0.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.3/docs/source/_templates/custom-class-template.rst` & `gwtc_tools-0.1.4/docs/source/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.3/docs/source/_templates/custom-module-template.rst` & `gwtc_tools-0.1.4/docs/source/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.3/docs/source/conf.py` & `gwtc_tools-0.1.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.3/examples/H1-GSTLAL_AllSky-1368009034-0.xml.gz` & `gwtc_tools-0.1.4/examples/H1-GSTLAL_AllSky-1368009034-0.xml.gz`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.3/examples/H1L1-GSTLAL_AllSky-1376883065-0.xml.gz` & `gwtc_tools-0.1.4/examples/H1L1-GSTLAL_AllSky-1376883065-0.xml.gz`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.3/examples/H1L1-SPIIR_AllSky-1376883065-0.xml.gz` & `gwtc_tools-0.1.4/examples/H1L1-SPIIR_AllSky-1376883065-0.xml.gz`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.3/examples/L1-GSTLAL_AllSky-1368783503-0.xml.gz` & `gwtc_tools-0.1.4/examples/L1-GSTLAL_AllSky-1368783503-0.xml.gz`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.3/pyproject.toml` & `gwtc_tools-0.1.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 [tool.setuptools_scm]
 write_to = "src/gwtc/_version.py"
 
 
 [project]
 name = "gwtc-tools"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Chad Hanna", email="chad.hanna@ligo.org" },
   { name="Alexander Pace", email="alexander.pace@ligo.org" },
   { name="Divya Singh", email="divya.singh@ligo.org" },
   { name="Leo Tsukada", email="leo.tsukada@ligo.org" },
   { name="Patrick Godwin", email="patrick.godwin@ligo.org" },
   { name="Prathamesh Joshi", email="prathamesh.joshi@ligo.org" },
@@ -30,24 +30,22 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "ligo-gracedb",
     "pyyaml", 
-    "cbcflow"
 ]
 
 [project.scripts]
     gwtc_test = "gwtc:gwtc_test"
     gwtc_update_pipeline_gevents = "gwtc:gwtc_update_pipeline_gevents"
     gwtc_diff = "gwtc:gwtc_diff"
     gwtc_get_gevent_coinc_files = "gwtc:gwtc_get_gevent_coinc_files"
     gwtc_create_from_query = "gwtc:gwtc_create_from_query"
-    catalog_pipe_aggregate_data = "catalog_pipeline:aggregate_data"
 
 #[tool.setuptools.dynamic]
 #version = "0.1.0"# {attr = "gwtc._version.__version__"}
 
 [project.urls]
 "Homepage" = "https://git.ligo.org/chad-hanna/gwtc"
 "Bug Tracker" = "https://git.ligo.org/chad-hanna/gwtc/-/issues"
```

### Comparing `gwtc_tools-0.1.3/setup.cfg` & `gwtc_tools-0.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.3/src/gwtc/gwtc.py` & `gwtc_tools-0.1.4/src/gwtc/gwtc.py`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.3/src/gwtc/gwtc_create_from_query.py` & `gwtc_tools-0.1.4/src/gwtc/gwtc_create_from_query.py`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.3/src/gwtc/gwtc_diff.py` & `gwtc_tools-0.1.4/src/gwtc/gwtc_diff.py`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.3/src/gwtc/gwtc_get_gevent_coinc_files.py` & `gwtc_tools-0.1.4/src/gwtc/gwtc_get_gevent_coinc_files.py`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.3/src/gwtc/gwtc_gracedb.py` & `gwtc_tools-0.1.4/src/gwtc/gwtc_gracedb.py`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.3/src/gwtc/gwtc_update_pipeline_gevents.py` & `gwtc_tools-0.1.4/src/gwtc/gwtc_update_pipeline_gevents.py`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.3/src/gwtc_tools.egg-info/SOURCES.txt` & `gwtc_tools-0.1.4/src/gwtc_tools.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -18,16 +18,14 @@
 examples/H1L1-SPIIR_AllSky-1376883065-0.xml.gz
 examples/H1L1-SPIIR_AllSky_PASTRO-1376883065-0.json
 examples/L1-GSTLAL_AllSky-1368783503-0.xml.gz
 examples/L1-GSTLAL_AllSky_PASTRO-1368783503-0.json
 examples/README.md
 examples/gstlalv1.yaml
 examples/gstlalv2.yaml
-src/catalog_pipeline/__init__.py
-src/catalog_pipeline/aggregate_data.py
 src/gwtc/__init__.py
 src/gwtc/_version.py
 src/gwtc/gwtc.py
 src/gwtc/gwtc_create_from_query.py
 src/gwtc/gwtc_diff.py
 src/gwtc/gwtc_get_gevent_coinc_files.py
 src/gwtc/gwtc_gracedb.py
```

