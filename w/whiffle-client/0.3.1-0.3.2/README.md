# Comparing `tmp/whiffle_client-0.3.1.tar.gz` & `tmp/whiffle_client-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whiffle_client-0.3.1.tar", last modified: Mon Apr  8 08:35:39 2024, max compression
+gzip compressed data, was "whiffle_client-0.3.2.tar", last modified: Thu Apr 25 06:57:57 2024, max compression
```

## Comparing `whiffle_client-0.3.1.tar` & `whiffle_client-0.3.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:35:39.320943 whiffle_client-0.3.1/
--rw-rw-rw-   0 root         (0) root         (0)     1069 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/LICENCE.txt
--rw-r--r--   0 root         (0) root         (0)     3326 2024-04-08 08:35:39.320943 whiffle_client-0.3.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      980 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2413 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/USER_README.md
--rw-rw-rw-   0 root         (0) root         (0)     1226 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 08:35:39.320943 whiffle_client-0.3.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:35:39.312943 whiffle_client-0.3.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     4791 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/tests/test_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:35:39.313943 whiffle_client-0.3.1/whiffle_client/
--rw-rw-rw-   0 root         (0) root         (0)      197 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:35:39.315943 whiffle_client-0.3.1/whiffle_client/analysis/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/analysis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6719 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/analysis/io.py
--rw-rw-rw-   0 root         (0) root         (0)    16419 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/analysis/plot.py
--rw-rw-rw-   0 root         (0) root         (0)     4854 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/analysis/scatter.py
--rw-rw-rw-   0 root         (0) root         (0)     4957 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/analysis/skill.py
--rw-rw-rw-   0 root         (0) root         (0)     3231 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/analysis/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     8323 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/client.py
--rw-rw-rw-   0 root         (0) root         (0)     3218 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/entrypoints.py
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/io.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:35:39.316943 whiffle_client-0.3.1/whiffle_client/resources/
--rw-rw-rw-   0 root         (0) root         (0)     2624 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/resources/example_generic_params.json
--rw-rw-rw-   0 root         (0) root         (0)     1015 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/resources/example_yaml_include.yaml
--rw-rw-rw-   0 root         (0) root         (0)      154 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/resources/example_yaml_include_metmasts.yaml
--rw-rw-rw-   0 root         (0) root         (0)       60 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/resources/whiffle_config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:35:39.317943 whiffle_client-0.3.1/whiffle_client/wind/
--rw-rw-rw-   0 root         (0) root         (0)       96 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/wind/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10808 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/wind/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:35:39.318943 whiffle_client-0.3.1/whiffle_client/wind/components/
--rw-rw-rw-   0 root         (0) root         (0)      298 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/wind/components/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      248 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/wind/components/domain.py
--rw-rw-rw-   0 root         (0) root         (0)      253 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/wind/components/geometries.py
--rw-rw-rw-   0 root         (0) root         (0)      111 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/wind/components/metmast.py
--rw-rw-rw-   0 root         (0) root         (0)      366 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/wind/components/turbine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:35:39.318943 whiffle_client-0.3.1/whiffle_client/wind/loaders/
--rw-rw-rw-   0 root         (0) root         (0)       67 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/wind/loaders/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1072 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/wind/loaders/csv.py
--rw-rw-rw-   0 root         (0) root         (0)     4513 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/wind/wind_simulation_task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:35:39.319943 whiffle_client-0.3.1/whiffle_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3326 2024-04-08 08:35:39.000000 whiffle_client-0.3.1/whiffle_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1207 2024-04-08 08:35:39.000000 whiffle_client-0.3.1/whiffle_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 08:35:39.000000 whiffle_client-0.3.1/whiffle_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2024-04-08 08:35:39.000000 whiffle_client-0.3.1/whiffle_client.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      161 2024-04-08 08:35:39.000000 whiffle_client-0.3.1/whiffle_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-04-08 08:35:39.000000 whiffle_client-0.3.1/whiffle_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 06:57:57.059095 whiffle_client-0.3.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/LICENCE.txt
+-rw-r--r--   0 root         (0) root         (0)     3390 2024-04-25 06:57:57.059095 whiffle_client-0.3.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      980 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2413 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/USER_README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 06:57:57.059095 whiffle_client-0.3.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 06:57:57.049095 whiffle_client-0.3.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     4791 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/tests/test_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 06:57:57.050095 whiffle_client-0.3.2/whiffle_client/
+-rw-rw-rw-   0 root         (0) root         (0)      197 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 06:57:57.054095 whiffle_client-0.3.2/whiffle_client/analysis/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/analysis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7628 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/analysis/io.py
+-rw-rw-rw-   0 root         (0) root         (0)    16433 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/analysis/plot.py
+-rw-rw-rw-   0 root         (0) root         (0)     4854 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/analysis/scatter.py
+-rw-rw-rw-   0 root         (0) root         (0)     4957 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/analysis/skill.py
+-rw-rw-rw-   0 root         (0) root         (0)     3231 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/analysis/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     8323 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     3218 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/entrypoints.py
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/io.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 06:57:57.055095 whiffle_client-0.3.2/whiffle_client/resources/
+-rw-rw-rw-   0 root         (0) root         (0)     2624 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/resources/example_generic_params.json
+-rw-rw-rw-   0 root         (0) root         (0)     1015 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/resources/example_yaml_include.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      154 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/resources/example_yaml_include_metmasts.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/resources/whiffle_config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 06:57:57.055095 whiffle_client-0.3.2/whiffle_client/wind/
+-rw-rw-rw-   0 root         (0) root         (0)       96 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/wind/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10808 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/wind/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 06:57:57.057095 whiffle_client-0.3.2/whiffle_client/wind/components/
+-rw-rw-rw-   0 root         (0) root         (0)      298 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/wind/components/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      248 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/wind/components/domain.py
+-rw-rw-rw-   0 root         (0) root         (0)      253 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/wind/components/geometries.py
+-rw-rw-rw-   0 root         (0) root         (0)      111 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/wind/components/metmast.py
+-rw-rw-rw-   0 root         (0) root         (0)      366 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/wind/components/turbine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 06:57:57.058095 whiffle_client-0.3.2/whiffle_client/wind/loaders/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/wind/loaders/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/wind/loaders/csv.py
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/wind/wind_simulation_task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 06:57:57.058095 whiffle_client-0.3.2/whiffle_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3390 2024-04-25 06:57:57.000000 whiffle_client-0.3.2/whiffle_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1207 2024-04-25 06:57:57.000000 whiffle_client-0.3.2/whiffle_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 06:57:57.000000 whiffle_client-0.3.2/whiffle_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2024-04-25 06:57:57.000000 whiffle_client-0.3.2/whiffle_client.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      189 2024-04-25 06:57:57.000000 whiffle_client-0.3.2/whiffle_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-25 06:57:57.000000 whiffle_client-0.3.2/whiffle_client.egg-info/top_level.txt
```

### Comparing `whiffle_client-0.3.1/LICENCE.txt` & `whiffle_client-0.3.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.1/PKG-INFO` & `whiffle_client-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whiffle_client
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python based web client to interact with Whiffle services
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
@@ -12,21 +12,22 @@
 Requires-Dist: PyYAML~=6.0
 Requires-Dist: pyyaml-include~=1.3.1
 Requires-Dist: platformdirs~=4.0.0
 Requires-Dist: requests
 Requires-Dist: jupyter
 Provides-Extra: analysis
 Requires-Dist: numpy; extra == "analysis"
-Requires-Dist: pandas; extra == "analysis"
+Requires-Dist: pandas>=2; extra == "analysis"
 Requires-Dist: scipy; extra == "analysis"
 Requires-Dist: scikit-learn; extra == "analysis"
-Requires-Dist: xarray; extra == "analysis"
+Requires-Dist: xarray>=2022.12.0; extra == "analysis"
 Requires-Dist: netcdf4; extra == "analysis"
 Requires-Dist: matplotlib; extra == "analysis"
 Requires-Dist: hvplot; extra == "analysis"
+Requires-Dist: jupyter_bokeh; extra == "analysis"
 
 # Whiffle client
 
 ## Quickstart
 
 `whiffle-client` can be installed with `pip` as follows:
```

### Comparing `whiffle_client-0.3.1/README.md` & `whiffle_client-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.1/USER_README.md` & `whiffle_client-0.3.2/USER_README.md`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.1/pyproject.toml` & `whiffle_client-0.3.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -23,21 +23,22 @@
 ]
 
 dynamic = ["version"]
 
 [project.optional-dependencies]
 analysis = [
     "numpy",
-    "pandas",
+    "pandas>=2",
     "scipy",
     "scikit-learn",
-    "xarray",
+    "xarray>=2022.12.0",
     "netcdf4",
     "matplotlib",
-    "hvplot"
+    "hvplot",
+    "jupyter_bokeh",
 ]
 
 [project.scripts]
 whiffle = "whiffle_client.entrypoints:whiffle"
 
 [tool.setuptools]
 package-dir = {"whiffle_client" = "whiffle_client"}
```

### Comparing `whiffle_client-0.3.1/tests/test_client.py` & `whiffle_client-0.3.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.1/whiffle_client/analysis/io.py` & `whiffle_client-0.3.2/whiffle_client/analysis/io.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,23 @@
 from whiffle_client.analysis.utils import mean_angle
 
 WINDOGRAPHER_COLUMN_MAP = {
     "AvgWs": "wind-speed [m/s]",
     "AvgWd": "wind-direction [deg]",
 }
 
+CABAUW_DATA_VARS_MAP = {
+    "F": ("wind-speed", "m/s"),
+    "D": ("wind-direction", "deg"),
+}
+CABAUW_DIMS_MAP = {
+    "z": ("height", "m"),
+}
+CABAUW_HEIGHTS_TO_KEEP = [10.0, 20.0, 40.0, 80.0, 140.0, 200.0]
+
 
 def _parse_turbine_column_name(col_name: str) -> tuple[str, str, str]:
     turbine_name = "_".join(col_name.split("_")[:-1])
     variable = col_name.split("_")[-1].split("[")[0]
     units = col_name.split("[")[-1].split("]")[0]
     units = f"[{units}]"
     return turbine_name, variable, units
@@ -214,7 +223,23 @@
     )
     df = df.rename(columns=WINDOGRAPHER_COLUMN_MAP)
     df.index = (df.index - pd.Timedelta(utc_time_diff, unit="hour")).tz_localize("utc")
     df = df.stack(future_stack=True)
     df = pd.concat({metmast_name: df}, names=["metmast", "time [UTC]", "height [m]"])
     df = df.reorder_levels([1, 0, 2]).sort_index()
     return df
+
+
+def cabauw_metmast_nc_to_dataset(netcdf_path: str):
+    ds = xr.load_dataset(netcdf_path)
+    ds = ds[list(CABAUW_DATA_VARS_MAP)]
+    for var, (new_var, unit) in CABAUW_DATA_VARS_MAP.items():
+        ds = ds.rename_vars({var: new_var})
+        ds[new_var].attrs["units"] = unit
+    for var, (new_var, unit) in CABAUW_DIMS_MAP.items():
+        ds = ds.rename_dims({var: new_var}).rename_vars({var: new_var})
+        ds[new_var].attrs["units"] = unit
+    ds["time"] = ds["time"].dt.round("10min").to_index().tz_localize("utc")
+    ds["time"].attrs["units"] = "UTC"
+    ds = ds.assign_coords(metmast="cabauw_metmast").expand_dims("metmast")
+    ds = ds.sel(height=CABAUW_HEIGHTS_TO_KEEP)
+    return ds
```

### Comparing `whiffle_client-0.3.1/whiffle_client/analysis/plot.py` & `whiffle_client-0.3.2/whiffle_client/analysis/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
         f'{c}:\nk={weibull_params_df[c]["k"]:.2f}\nA={weibull_params_df[c]["A"]:.2f} m/s'
         for c in weibull_pdf_df.columns
     ]
     weibull_pdf_df.plot(ax=ax)
     ax.legend(loc="center left", bbox_to_anchor=(1, 0.5))
     ax.set_xlabel("Wind speed [m/s]")
     ax.set_ylabel("Weibull pdf [-]")
-    ax.set_title("Fitted Weibull pdf comparison")
+    ax.set_title("Fitted Weibull PDF comparison on wind speed")
     ax.grid()
     return ax
 
 
 def plot_wind_speed_distribution_comparison(
     measured_wind_speed_series: pd.Series,
     aspire_wind_speed_series: pd.Series,
```

### Comparing `whiffle_client-0.3.1/whiffle_client/analysis/scatter.py` & `whiffle_client-0.3.2/whiffle_client/analysis/scatter.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.1/whiffle_client/analysis/skill.py` & `whiffle_client-0.3.2/whiffle_client/analysis/skill.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.1/whiffle_client/analysis/utils.py` & `whiffle_client-0.3.2/whiffle_client/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.1/whiffle_client/client.py` & `whiffle_client-0.3.2/whiffle_client/client.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.1/whiffle_client/entrypoints.py` & `whiffle_client-0.3.2/whiffle_client/entrypoints.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.1/whiffle_client/io.py` & `whiffle_client-0.3.2/whiffle_client/io.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.1/whiffle_client/resources/example_generic_params.json` & `whiffle_client-0.3.2/whiffle_client/resources/example_generic_params.json`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.1/whiffle_client/resources/example_yaml_include.yaml` & `whiffle_client-0.3.2/whiffle_client/resources/example_yaml_include.yaml`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.1/whiffle_client/wind/client.py` & `whiffle_client-0.3.2/whiffle_client/wind/client.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.1/whiffle_client/wind/loaders/csv.py` & `whiffle_client-0.3.2/whiffle_client/wind/loaders/csv.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.1/whiffle_client/wind/wind_simulation_task.py` & `whiffle_client-0.3.2/whiffle_client/wind/wind_simulation_task.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.1/whiffle_client.egg-info/PKG-INFO` & `whiffle_client-0.3.2/whiffle_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whiffle_client
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python based web client to interact with Whiffle services
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
@@ -12,21 +12,22 @@
 Requires-Dist: PyYAML~=6.0
 Requires-Dist: pyyaml-include~=1.3.1
 Requires-Dist: platformdirs~=4.0.0
 Requires-Dist: requests
 Requires-Dist: jupyter
 Provides-Extra: analysis
 Requires-Dist: numpy; extra == "analysis"
-Requires-Dist: pandas; extra == "analysis"
+Requires-Dist: pandas>=2; extra == "analysis"
 Requires-Dist: scipy; extra == "analysis"
 Requires-Dist: scikit-learn; extra == "analysis"
-Requires-Dist: xarray; extra == "analysis"
+Requires-Dist: xarray>=2022.12.0; extra == "analysis"
 Requires-Dist: netcdf4; extra == "analysis"
 Requires-Dist: matplotlib; extra == "analysis"
 Requires-Dist: hvplot; extra == "analysis"
+Requires-Dist: jupyter_bokeh; extra == "analysis"
 
 # Whiffle client
 
 ## Quickstart
 
 `whiffle-client` can be installed with `pip` as follows:
```

### Comparing `whiffle_client-0.3.1/whiffle_client.egg-info/SOURCES.txt` & `whiffle_client-0.3.2/whiffle_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

