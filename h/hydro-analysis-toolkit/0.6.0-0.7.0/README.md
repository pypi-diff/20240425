# Comparing `tmp/hydro_analysis_toolkit-0.6.0.tar.gz` & `tmp/hydro_analysis_toolkit-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydro_analysis_toolkit-0.6.0.tar", last modified: Thu Nov 16 10:23:20 2023, max compression
+gzip compressed data, was "hydro_analysis_toolkit-0.7.0.tar", last modified: Thu Apr 25 10:24:18 2024, max compression
```

## Comparing `hydro_analysis_toolkit-0.6.0.tar` & `hydro_analysis_toolkit-0.7.0.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 10:23:20.261999 hydro_analysis_toolkit-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-11-16 10:23:07.000000 hydro_analysis_toolkit-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2023-11-16 10:23:20.261999 hydro_analysis_toolkit-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2023-11-16 10:23:07.000000 hydro_analysis_toolkit-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 10:23:20.258000 hydro_analysis_toolkit-0.6.0/hat/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2023-11-16 10:23:07.000000 hydro_analysis_toolkit-0.6.0/hat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2023-11-16 10:23:07.000000 hydro_analysis_toolkit-0.6.0/hat/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2023-11-16 10:23:07.000000 hydro_analysis_toolkit-0.6.0/hat/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 10:23:20.258000 hydro_analysis_toolkit-0.6.0/hat/config_json/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 10:23:07.000000 hydro_analysis_toolkit-0.6.0/hat/config_json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2023-11-16 10:23:07.000000 hydro_analysis_toolkit-0.6.0/hat/config_json/river_network_coordinate_names.json
--rw-r--r--   0 runner    (1001) docker     (127)      330 2023-11-16 10:23:07.000000 hydro_analysis_toolkit-0.6.0/hat/config_json/timeseries.json
--rw-r--r--   0 runner    (1001) docker     (127)     7917 2023-11-16 10:23:07.000000 hydro_analysis_toolkit-0.6.0/hat/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2023-11-16 10:23:07.000000 hydro_analysis_toolkit-0.6.0/hat/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2023-11-16 10:23:07.000000 hydro_analysis_toolkit-0.6.0/hat/extract_simulation_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)     6007 2023-11-16 10:23:07.000000 hydro_analysis_toolkit-0.6.0/hat/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    11430 2023-11-16 10:23:07.000000 hydro_analysis_toolkit-0.6.0/hat/geo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2023-11-16 10:23:07.000000 hydro_analysis_toolkit-0.6.0/hat/hydrostats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2023-11-16 10:23:07.000000 hydro_analysis_toolkit-0.6.0/hat/hydrostats_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2023-11-16 10:23:07.000000 hydro_analysis_toolkit-0.6.0/hat/hydrostats_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 10:23:20.261999 hydro_analysis_toolkit-0.6.0/hat/interactive/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2023-11-16 10:23:07.000000 hydro_analysis_toolkit-0.6.0/hat/interactive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11968 2023-11-16 10:23:07.000000 hydro_analysis_toolkit-0.6.0/hat/interactive/explorers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7505 2023-11-16 10:23:07.000000 hydro_analysis_toolkit-0.6.0/hat/interactive/leaflet.py
--rw-r--r--   0 runner    (1001) docker     (127)    16125 2023-11-16 10:23:07.000000 hydro_analysis_toolkit-0.6.0/hat/interactive/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2023-11-16 10:23:07.000000 hydro_analysis_toolkit-0.6.0/hat/observations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2023-11-16 10:23:07.000000 hydro_analysis_toolkit-0.6.0/hat/timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 10:23:20.261999 hydro_analysis_toolkit-0.6.0/hat/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 10:23:07.000000 hydro_analysis_toolkit-0.6.0/hat/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2023-11-16 10:23:07.000000 hydro_analysis_toolkit-0.6.0/hat/tools/extract_simulation_timeseries_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2023-11-16 10:23:07.000000 hydro_analysis_toolkit-0.6.0/hat/tools/hydrostats_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-16 10:23:07.000000 hydro_analysis_toolkit-0.6.0/hat/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 10:23:20.261999 hydro_analysis_toolkit-0.6.0/hydro_analysis_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2023-11-16 10:23:20.000000 hydro_analysis_toolkit-0.6.0/hydro_analysis_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2023-11-16 10:23:20.000000 hydro_analysis_toolkit-0.6.0/hydro_analysis_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-16 10:23:20.000000 hydro_analysis_toolkit-0.6.0/hydro_analysis_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      139 2023-11-16 10:23:20.000000 hydro_analysis_toolkit-0.6.0/hydro_analysis_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2023-11-16 10:23:20.000000 hydro_analysis_toolkit-0.6.0/hydro_analysis_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-11-16 10:23:07.000000 hydro_analysis_toolkit-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      767 2023-11-16 10:23:20.261999 hydro_analysis_toolkit-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-16 10:23:07.000000 hydro_analysis_toolkit-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 10:23:20.261999 hydro_analysis_toolkit-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2023-11-16 10:23:07.000000 hydro_analysis_toolkit-0.6.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2023-11-16 10:23:07.000000 hydro_analysis_toolkit-0.6.0/tests/test_hydrostats_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2023-11-16 10:23:07.000000 hydro_analysis_toolkit-0.6.0/tests/test_hydrostats_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2023-11-16 10:23:07.000000 hydro_analysis_toolkit-0.6.0/tests/test_hydrostats_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5991 2023-11-16 10:23:07.000000 hydro_analysis_toolkit-0.6.0/tests/test_interactive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:24:18.668772 hydro_analysis_toolkit-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-25 10:24:07.000000 hydro_analysis_toolkit-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-25 10:24:18.668772 hydro_analysis_toolkit-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-25 10:24:07.000000 hydro_analysis_toolkit-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:24:18.664772 hydro_analysis_toolkit-0.7.0/hat/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-25 10:24:07.000000 hydro_analysis_toolkit-0.7.0/hat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-25 10:24:07.000000 hydro_analysis_toolkit-0.7.0/hat/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-25 10:24:07.000000 hydro_analysis_toolkit-0.7.0/hat/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:24:18.664772 hydro_analysis_toolkit-0.7.0/hat/config_json/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 10:24:07.000000 hydro_analysis_toolkit-0.7.0/hat/config_json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-25 10:24:07.000000 hydro_analysis_toolkit-0.7.0/hat/config_json/river_network_coordinate_names.json
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-25 10:24:07.000000 hydro_analysis_toolkit-0.7.0/hat/config_json/timeseries.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7917 2024-04-25 10:24:07.000000 hydro_analysis_toolkit-0.7.0/hat/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-25 10:24:07.000000 hydro_analysis_toolkit-0.7.0/hat/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-25 10:24:07.000000 hydro_analysis_toolkit-0.7.0/hat/extract_simulation_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-04-25 10:24:07.000000 hydro_analysis_toolkit-0.7.0/hat/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11430 2024-04-25 10:24:07.000000 hydro_analysis_toolkit-0.7.0/hat/geo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-25 10:24:07.000000 hydro_analysis_toolkit-0.7.0/hat/hydrostats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-25 10:24:07.000000 hydro_analysis_toolkit-0.7.0/hat/hydrostats_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-25 10:24:07.000000 hydro_analysis_toolkit-0.7.0/hat/hydrostats_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:24:18.664772 hydro_analysis_toolkit-0.7.0/hat/interactive/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-25 10:24:07.000000 hydro_analysis_toolkit-0.7.0/hat/interactive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11968 2024-04-25 10:24:07.000000 hydro_analysis_toolkit-0.7.0/hat/interactive/explorers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-04-25 10:24:07.000000 hydro_analysis_toolkit-0.7.0/hat/interactive/leaflet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16125 2024-04-25 10:24:07.000000 hydro_analysis_toolkit-0.7.0/hat/interactive/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-25 10:24:07.000000 hydro_analysis_toolkit-0.7.0/hat/observations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-04-25 10:24:07.000000 hydro_analysis_toolkit-0.7.0/hat/timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:24:18.664772 hydro_analysis_toolkit-0.7.0/hat/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 10:24:07.000000 hydro_analysis_toolkit-0.7.0/hat/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-25 10:24:07.000000 hydro_analysis_toolkit-0.7.0/hat/tools/extract_simulation_timeseries_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-25 10:24:07.000000 hydro_analysis_toolkit-0.7.0/hat/tools/hydrostats_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 10:24:07.000000 hydro_analysis_toolkit-0.7.0/hat/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:24:18.668772 hydro_analysis_toolkit-0.7.0/hydro_analysis_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-25 10:24:18.000000 hydro_analysis_toolkit-0.7.0/hydro_analysis_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-25 10:24:18.000000 hydro_analysis_toolkit-0.7.0/hydro_analysis_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 10:24:18.000000 hydro_analysis_toolkit-0.7.0/hydro_analysis_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-25 10:24:18.000000 hydro_analysis_toolkit-0.7.0/hydro_analysis_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-25 10:24:18.000000 hydro_analysis_toolkit-0.7.0/hydro_analysis_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-25 10:24:07.000000 hydro_analysis_toolkit-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-25 10:24:18.668772 hydro_analysis_toolkit-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 10:24:07.000000 hydro_analysis_toolkit-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:24:18.668772 hydro_analysis_toolkit-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-25 10:24:07.000000 hydro_analysis_toolkit-0.7.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-25 10:24:07.000000 hydro_analysis_toolkit-0.7.0/tests/test_hydrostats_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-25 10:24:07.000000 hydro_analysis_toolkit-0.7.0/tests/test_hydrostats_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-25 10:24:07.000000 hydro_analysis_toolkit-0.7.0/tests/test_hydrostats_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5991 2024-04-25 10:24:07.000000 hydro_analysis_toolkit-0.7.0/tests/test_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8172 2024-04-25 10:24:07.000000 hydro_analysis_toolkit-0.7.0/tests/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-25 10:24:07.000000 hydro_analysis_toolkit-0.7.0/tests/test_mapping_evaluation.py
```

### Comparing `hydro_analysis_toolkit-0.6.0/LICENSE` & `hydro_analysis_toolkit-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hydro_analysis_toolkit-0.6.0/PKG-INFO` & `hydro_analysis_toolkit-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydro_analysis_toolkit
-Version: 0.6.0
+Version: 0.7.0
 Summary: ECMWF Hydrological Analysis Tools
 Home-page: https://hydro-analysis-toolkit.readthedocs.io
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hydro_analysis_toolkit-0.6.0/README.md` & `hydro_analysis_toolkit-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `hydro_analysis_toolkit-0.6.0/hat/cli.py` & `hydro_analysis_toolkit-0.7.0/hat/cli.py`

 * *Files identical despite different names*

### Comparing `hydro_analysis_toolkit-0.6.0/hat/config.py` & `hydro_analysis_toolkit-0.7.0/hat/config.py`

 * *Files identical despite different names*

### Comparing `hydro_analysis_toolkit-0.6.0/hat/data.py` & `hydro_analysis_toolkit-0.7.0/hat/data.py`

 * *Files identical despite different names*

### Comparing `hydro_analysis_toolkit-0.6.0/hat/extract_simulation_timeseries.py` & `hydro_analysis_toolkit-0.7.0/hat/extract_simulation_timeseries.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Python module for extracting simulation timeseries from grids (i.e. rasters)
 """
+
 import geopandas as gpd
 import xarray as xr
 
 from hat.config import load_package_config, valid_custom_config
 
 # hat modules
 from hat.geo import geopoints_to_array, latlon_coords
```

### Comparing `hydro_analysis_toolkit-0.6.0/hat/filters.py` & `hydro_analysis_toolkit-0.7.0/hat/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,14 +126,16 @@
     if "," in filters:
         filters = filters.split(",")
     else:
         filters = [filters]
 
     # apply each filter in turn
     for filter_str in filters:
+        if filter_str == "":
+            continue
         parts = filter_str.split()
         if len(parts) != 3:
             raise ValueError("Invalid filter format. Expected 'key operator value'.")
 
         key, operator, value = parts
 
         df = apply_filter(df, key, operator, value)
```

### Comparing `hydro_analysis_toolkit-0.6.0/hat/geo.py` & `hydro_analysis_toolkit-0.7.0/hat/geo.py`

 * *Files identical despite different names*

### Comparing `hydro_analysis_toolkit-0.6.0/hat/hydrostats.py` & `hydro_analysis_toolkit-0.7.0/hat/hydrostats.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """high level python api for hydrological statistics"""
+
 from typing import List
 
 import numpy as np
 import xarray as xr
 
 from hat import hydrostats_functions
```

### Comparing `hydro_analysis_toolkit-0.6.0/hat/hydrostats_decorators.py` & `hydro_analysis_toolkit-0.7.0/hat/hydrostats_decorators.py`

 * *Files identical despite different names*

### Comparing `hydro_analysis_toolkit-0.6.0/hat/hydrostats_functions.py` & `hydro_analysis_toolkit-0.7.0/hat/hydrostats_functions.py`

 * *Files identical despite different names*

### Comparing `hydro_analysis_toolkit-0.6.0/hat/interactive/explorers.py` & `hydro_analysis_toolkit-0.7.0/hat/interactive/explorers.py`

 * *Files identical despite different names*

### Comparing `hydro_analysis_toolkit-0.6.0/hat/interactive/leaflet.py` & `hydro_analysis_toolkit-0.7.0/hat/interactive/leaflet.py`

 * *Files identical despite different names*

### Comparing `hydro_analysis_toolkit-0.6.0/hat/interactive/widgets.py` & `hydro_analysis_toolkit-0.7.0/hat/interactive/widgets.py`

 * *Files identical despite different names*

### Comparing `hydro_analysis_toolkit-0.6.0/hat/observations.py` & `hydro_analysis_toolkit-0.7.0/hat/observations.py`

 * *Files identical despite different names*

### Comparing `hydro_analysis_toolkit-0.6.0/hat/timeseries.py` & `hydro_analysis_toolkit-0.7.0/hat/timeseries.py`

 * *Files identical despite different names*

### Comparing `hydro_analysis_toolkit-0.6.0/hat/tools/extract_simulation_timeseries_cli.py` & `hydro_analysis_toolkit-0.7.0/hat/tools/extract_simulation_timeseries_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 
     # read simulated data
     simulation = read_simulation_as_xarray(cfg["simulation"])
 
     print_overview(cfg, stations, simulation)
 
     # Extract time series
-    timeseries = extract_timeseries(stations, simulation)
+    timeseries = extract_timeseries(stations, simulation, cfg)
     title("Timeseries extracted")
     print(timeseries)
 
     save_dataset_to_netcdf(timeseries, cfg["simulation_output_filepath"])
 
     title("TIMESERIES EXTRACTION COMPLETE", background="cyan", bold=True)
```

### Comparing `hydro_analysis_toolkit-0.6.0/hat/tools/hydrostats_cli.py` & `hydro_analysis_toolkit-0.7.0/hat/tools/hydrostats_cli.py`

 * *Files identical despite different names*

### Comparing `hydro_analysis_toolkit-0.6.0/hydro_analysis_toolkit.egg-info/PKG-INFO` & `hydro_analysis_toolkit-0.7.0/hydro_analysis_toolkit.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hydro-analysis-toolkit
-Version: 0.6.0
+Name: hydro_analysis_toolkit
+Version: 0.7.0
 Summary: ECMWF Hydrological Analysis Tools
 Home-page: https://hydro-analysis-toolkit.readthedocs.io
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hydro_analysis_toolkit-0.6.0/hydro_analysis_toolkit.egg-info/SOURCES.txt` & `hydro_analysis_toolkit-0.7.0/hydro_analysis_toolkit.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -32,8 +32,10 @@
 hydro_analysis_toolkit.egg-info/dependency_links.txt
 hydro_analysis_toolkit.egg-info/entry_points.txt
 hydro_analysis_toolkit.egg-info/top_level.txt
 tests/test_config.py
 tests/test_hydrostats_cli.py
 tests/test_hydrostats_decorators.py
 tests/test_hydrostats_functions.py
-tests/test_interactive.py
+tests/test_interactive.py
+tests/test_mapping.py
+tests/test_mapping_evaluation.py
```

### Comparing `hydro_analysis_toolkit-0.6.0/setup.cfg` & `hydro_analysis_toolkit-0.7.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -20,12 +20,13 @@
 [options.packages.find]
 include = hat*
 
 [options.entry_points]
 console_scripts = 
 	hat-extract-timeseries = hat.tools.extract_simulation_timeseries_cli:main
 	hat-hydrostats = hat.tools.hydrostats_cli:main
+	hat-stations-mapping = hat.mapping.station_mapping:main
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `hydro_analysis_toolkit-0.6.0/tests/test_config.py` & `hydro_analysis_toolkit-0.7.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `hydro_analysis_toolkit-0.6.0/tests/test_hydrostats_cli.py` & `hydro_analysis_toolkit-0.7.0/tests/test_hydrostats_cli.py`

 * *Files identical despite different names*

### Comparing `hydro_analysis_toolkit-0.6.0/tests/test_hydrostats_decorators.py` & `hydro_analysis_toolkit-0.7.0/tests/test_hydrostats_decorators.py`

 * *Files identical despite different names*

### Comparing `hydro_analysis_toolkit-0.6.0/tests/test_hydrostats_functions.py` & `hydro_analysis_toolkit-0.7.0/tests/test_hydrostats_functions.py`

 * *Files identical despite different names*

### Comparing `hydro_analysis_toolkit-0.6.0/tests/test_interactive.py` & `hydro_analysis_toolkit-0.7.0/tests/test_interactive.py`

 * *Files identical despite different names*

