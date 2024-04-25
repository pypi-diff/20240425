# Comparing `tmp/village-data-analysis-1.0.tar.gz` & `tmp/village-data-analysis-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "village-data-analysis-1.0.tar", last modified: Wed Apr 24 12:18:23 2024, max compression
+gzip compressed data, was "village-data-analysis-1.1.tar", last modified: Wed Apr 24 12:50:00 2024, max compression
```

## Comparing `village-data-analysis-1.0.tar` & `village-data-analysis-1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 istvan    (1000) istvan    (1000)        0 2024-04-24 12:18:23.767054 village-data-analysis-1.0/
--rw-r--r--   0 istvan    (1000) istvan    (1000)      184 2024-04-24 12:18:23.767054 village-data-analysis-1.0/PKG-INFO
--rw-r--r--   0 istvan    (1000) istvan    (1000)      645 2024-04-24 12:15:57.000000 village-data-analysis-1.0/README.md
--rw-r--r--   0 istvan    (1000) istvan    (1000)       38 2024-04-24 12:18:23.767054 village-data-analysis-1.0/setup.cfg
--rw-r--r--   0 istvan    (1000) istvan    (1000)      438 2024-04-24 12:11:32.000000 village-data-analysis-1.0/setup.py
-drwxr-xr-x   0 istvan    (1000) istvan    (1000)        0 2024-04-24 12:18:23.763720 village-data-analysis-1.0/village_data_analysis/
--rw-r--r--   0 istvan    (1000) istvan    (1000)        0 2024-04-22 12:22:55.000000 village-data-analysis-1.0/village_data_analysis/__init__.py
--rw-r--r--   0 istvan    (1000) istvan    (1000)    14800 2024-04-22 12:22:55.000000 village-data-analysis-1.0/village_data_analysis/analyzer.py
--rw-r--r--   0 istvan    (1000) istvan    (1000)     1107 2024-04-22 12:22:55.000000 village-data-analysis-1.0/village_data_analysis/coord_converter.py
--rw-r--r--   0 istvan    (1000) istvan    (1000)     4294 2024-04-22 12:22:55.000000 village-data-analysis-1.0/village_data_analysis/data_create.py
--rw-r--r--   0 istvan    (1000) istvan    (1000)      708 2024-04-22 12:22:55.000000 village-data-analysis-1.0/village_data_analysis/helpers.py
-drwxr-xr-x   0 istvan    (1000) istvan    (1000)        0 2024-04-24 12:18:23.767054 village-data-analysis-1.0/village_data_analysis.egg-info/
--rw-r--r--   0 istvan    (1000) istvan    (1000)      184 2024-04-24 12:18:23.000000 village-data-analysis-1.0/village_data_analysis.egg-info/PKG-INFO
--rw-r--r--   0 istvan    (1000) istvan    (1000)      421 2024-04-24 12:18:23.000000 village-data-analysis-1.0/village_data_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 istvan    (1000) istvan    (1000)        1 2024-04-24 12:18:23.000000 village-data-analysis-1.0/village_data_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 istvan    (1000) istvan    (1000)       52 2024-04-24 12:18:23.000000 village-data-analysis-1.0/village_data_analysis.egg-info/requires.txt
--rw-r--r--   0 istvan    (1000) istvan    (1000)       22 2024-04-24 12:18:23.000000 village-data-analysis-1.0/village_data_analysis.egg-info/top_level.txt
+drwxr-xr-x   0 istvan    (1000) istvan    (1000)        0 2024-04-24 12:50:00.140427 village-data-analysis-1.1/
+-rw-r--r--   0 istvan    (1000) istvan    (1000)      242 2024-04-24 12:50:00.140427 village-data-analysis-1.1/PKG-INFO
+-rw-r--r--   0 istvan    (1000) istvan    (1000)      753 2024-04-24 12:43:39.000000 village-data-analysis-1.1/README.md
+-rw-r--r--   0 istvan    (1000) istvan    (1000)       38 2024-04-24 12:50:00.140427 village-data-analysis-1.1/setup.cfg
+-rw-r--r--   0 istvan    (1000) istvan    (1000)      497 2024-04-24 12:49:37.000000 village-data-analysis-1.1/setup.py
+drwxr-xr-x   0 istvan    (1000) istvan    (1000)        0 2024-04-24 12:50:00.140427 village-data-analysis-1.1/village_data_analysis/
+-rw-r--r--   0 istvan    (1000) istvan    (1000)        0 2024-04-22 12:22:55.000000 village-data-analysis-1.1/village_data_analysis/__init__.py
+-rw-r--r--   0 istvan    (1000) istvan    (1000)    14800 2024-04-22 12:22:55.000000 village-data-analysis-1.1/village_data_analysis/analyzer.py
+-rw-r--r--   0 istvan    (1000) istvan    (1000)     1107 2024-04-22 12:22:55.000000 village-data-analysis-1.1/village_data_analysis/coord_converter.py
+-rw-r--r--   0 istvan    (1000) istvan    (1000)     4294 2024-04-22 12:22:55.000000 village-data-analysis-1.1/village_data_analysis/data_create.py
+-rw-r--r--   0 istvan    (1000) istvan    (1000)      708 2024-04-22 12:22:55.000000 village-data-analysis-1.1/village_data_analysis/helpers.py
+drwxr-xr-x   0 istvan    (1000) istvan    (1000)        0 2024-04-24 12:50:00.140427 village-data-analysis-1.1/village_data_analysis.egg-info/
+-rw-r--r--   0 istvan    (1000) istvan    (1000)      242 2024-04-24 12:50:00.000000 village-data-analysis-1.1/village_data_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 istvan    (1000) istvan    (1000)      421 2024-04-24 12:50:00.000000 village-data-analysis-1.1/village_data_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 istvan    (1000) istvan    (1000)        1 2024-04-24 12:50:00.000000 village-data-analysis-1.1/village_data_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 istvan    (1000) istvan    (1000)       52 2024-04-24 12:50:00.000000 village-data-analysis-1.1/village_data_analysis.egg-info/requires.txt
+-rw-r--r--   0 istvan    (1000) istvan    (1000)       22 2024-04-24 12:50:00.000000 village-data-analysis-1.1/village_data_analysis.egg-info/top_level.txt
```

### Comparing `village-data-analysis-1.0/village_data_analysis/analyzer.py` & `village-data-analysis-1.1/village_data_analysis/analyzer.py`

 * *Files identical despite different names*

### Comparing `village-data-analysis-1.0/village_data_analysis/coord_converter.py` & `village-data-analysis-1.1/village_data_analysis/coord_converter.py`

 * *Files identical despite different names*

### Comparing `village-data-analysis-1.0/village_data_analysis/data_create.py` & `village-data-analysis-1.1/village_data_analysis/data_create.py`

 * *Files identical despite different names*

### Comparing `village-data-analysis-1.0/village_data_analysis/helpers.py` & `village-data-analysis-1.1/village_data_analysis/helpers.py`

 * *Files identical despite different names*

