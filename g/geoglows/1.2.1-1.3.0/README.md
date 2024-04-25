# Comparing `tmp/geoglows-1.2.1.tar.gz` & `tmp/geoglows-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoglows-1.2.1.tar", last modified: Wed Apr 17 19:42:49 2024, max compression
+gzip compressed data, was "geoglows-1.3.0.tar", last modified: Thu Apr 25 14:44:51 2024, max compression
```

## Comparing `geoglows-1.2.1.tar` & `geoglows-1.3.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:42:49.250964 geoglows-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-17 19:42:44.000000 geoglows-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-17 19:42:44.000000 geoglows-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-17 19:42:49.250964 geoglows-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-17 19:42:44.000000 geoglows-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:42:49.246964 geoglows-1.2.1/geoglows/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-17 19:42:44.000000 geoglows-1.2.1/geoglows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-17 19:42:44.000000 geoglows-1.2.1/geoglows/_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:42:49.250964 geoglows-1.2.1/geoglows/_plots/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-17 19:42:44.000000 geoglows-1.2.1/geoglows/_plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-17 19:42:44.000000 geoglows-1.2.1/geoglows/_plots/format_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    16447 2024-04-17 19:42:44.000000 geoglows-1.2.1/geoglows/_plots/plotly_bias_corrected.py
--rw-r--r--   0 runner    (1001) docker     (127)    11334 2024-04-17 19:42:44.000000 geoglows-1.2.1/geoglows/_plots/plotly_forecasts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-17 19:42:44.000000 geoglows-1.2.1/geoglows/_plots/plotly_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9693 2024-04-17 19:42:44.000000 geoglows-1.2.1/geoglows/_plots/plotly_retrospective.py
--rw-r--r--   0 runner    (1001) docker     (127)    11701 2024-04-17 19:42:44.000000 geoglows-1.2.1/geoglows/_plots/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-04-17 19:42:44.000000 geoglows-1.2.1/geoglows/analyze.py
--rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-04-17 19:42:44.000000 geoglows-1.2.1/geoglows/bias.py
--rw-r--r--   0 runner    (1001) docker     (127)    15279 2024-04-17 19:42:44.000000 geoglows-1.2.1/geoglows/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    15652 2024-04-17 19:42:44.000000 geoglows-1.2.1/geoglows/streamflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-17 19:42:44.000000 geoglows-1.2.1/geoglows/streams.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-17 19:42:44.000000 geoglows-1.2.1/geoglows/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:42:49.250964 geoglows-1.2.1/geoglows.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-17 19:42:49.000000 geoglows-1.2.1/geoglows.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-17 19:42:49.000000 geoglows-1.2.1/geoglows.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 19:42:49.000000 geoglows-1.2.1/geoglows.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-17 19:42:49.000000 geoglows-1.2.1/geoglows.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 19:42:49.000000 geoglows-1.2.1/geoglows.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-17 19:42:44.000000 geoglows-1.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 19:42:49.250964 geoglows-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-17 19:42:44.000000 geoglows-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:44:51.527587 geoglows-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-25 14:44:43.000000 geoglows-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-25 14:44:43.000000 geoglows-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-25 14:44:51.527587 geoglows-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-25 14:44:43.000000 geoglows-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:44:51.523587 geoglows-1.3.0/geoglows/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-25 14:44:43.000000 geoglows-1.3.0/geoglows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-25 14:44:43.000000 geoglows-1.3.0/geoglows/_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:44:51.527587 geoglows-1.3.0/geoglows/_plots/
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-25 14:44:43.000000 geoglows-1.3.0/geoglows/_plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-25 14:44:43.000000 geoglows-1.3.0/geoglows/_plots/format_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16447 2024-04-25 14:44:43.000000 geoglows-1.3.0/geoglows/_plots/plotly_bias_corrected.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11330 2024-04-25 14:44:43.000000 geoglows-1.3.0/geoglows/_plots/plotly_forecasts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-25 14:44:43.000000 geoglows-1.3.0/geoglows/_plots/plotly_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9693 2024-04-25 14:44:43.000000 geoglows-1.3.0/geoglows/_plots/plotly_retrospective.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12471 2024-04-25 14:44:43.000000 geoglows-1.3.0/geoglows/_plots/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-04-25 14:44:43.000000 geoglows-1.3.0/geoglows/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-04-25 14:44:43.000000 geoglows-1.3.0/geoglows/bias.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15279 2024-04-25 14:44:43.000000 geoglows-1.3.0/geoglows/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15652 2024-04-25 14:44:43.000000 geoglows-1.3.0/geoglows/streamflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-25 14:44:43.000000 geoglows-1.3.0/geoglows/streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-25 14:44:43.000000 geoglows-1.3.0/geoglows/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:44:51.527587 geoglows-1.3.0/geoglows.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-25 14:44:51.000000 geoglows-1.3.0/geoglows.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-25 14:44:51.000000 geoglows-1.3.0/geoglows.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 14:44:51.000000 geoglows-1.3.0/geoglows.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-25 14:44:51.000000 geoglows-1.3.0/geoglows.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 14:44:51.000000 geoglows-1.3.0/geoglows.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-25 14:44:43.000000 geoglows-1.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 14:44:51.527587 geoglows-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-25 14:44:43.000000 geoglows-1.3.0/setup.py
```

### Comparing `geoglows-1.2.1/LICENSE` & `geoglows-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geoglows-1.2.1/PKG-INFO` & `geoglows-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoglows
-Version: 1.2.1
+Version: 1.3.0
 Summary: Package for accessing data from the GEOGLOWS Hydrological Model
 Home-page: https://data.geoglows.org
 Author: Riley Hales PhD
 License: BSD 3-Clause Clear License
 Project-URL: Homepage, https://data.geoglows.org
 Project-URL: Documentation, https://geoglows.readthedocs.io
 Project-URL: Source, https://github.com/geoglows/pygeoglows
```

### Comparing `geoglows-1.2.1/README.md` & `geoglows-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `geoglows-1.2.1/geoglows/_plots/__init__.py` & `geoglows-1.3.0/geoglows/_plots/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .plots import (
     forecast,
     forecast_stats,
     forecast_ensembles,
+    forecast_records,
     retrospective,
     daily_averages,
     monthly_averages,
     annual_averages,
     flow_duration_curve,
     corrected_retrospective,
     corrected_month_average,
@@ -13,14 +14,15 @@
     corrected_scatterplots,
 )
 
 __all__ = [
     'forecast',
     'forecast_stats',
     'forecast_ensembles',
+    'forecast_records',
     'retrospective',
     'daily_averages',
     'monthly_averages',
     'annual_averages',
     'flow_duration_curve',
     'corrected_retrospective',
     'corrected_month_average',
```

### Comparing `geoglows-1.2.1/geoglows/_plots/format_tools.py` & `geoglows-1.3.0/geoglows/_plots/format_tools.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.2.1/geoglows/_plots/plotly_bias_corrected.py` & `geoglows-1.3.0/geoglows/_plots/plotly_bias_corrected.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.2.1/geoglows/_plots/plotly_forecasts.py` & `geoglows-1.3.0/geoglows/_plots/plotly_forecasts.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,35 +255,35 @@
             'hoverformat': '%b %d %Y',
             'tickformat': '%b %d %Y'
         },
     )
     return go.Figure(scatter_plots, layout=layout)
 
 
-def forecast_records(recs: pd.DataFrame, *, rp_df: pd.DataFrame = None, plot_titles: list = False, ) -> go.Figure:
+def forecast_records(df: pd.DataFrame, *, rp_df: pd.DataFrame = None, plot_titles: list = False, ) -> go.Figure:
     """
     Makes the streamflow saved forecast data and metadata into a plotly plot
 
     Args:
-        recs: the csv response from forecast_records
+        df: the csv response from forecast_records
         rp_df: the csv response from return_periods
         plot_titles: a list of strings to place in the figure title. each list item will be on a new line.
 
     Return:
          plotly.GraphObject: plotly object, especially for use with python notebooks and the .show() method
     """
     # Start processing the inputs
-    dates = recs.index.tolist()
+    dates = df.index.tolist()
     startdate = dates[0]
     enddate = dates[-1]
 
     plot_data = {
         'x_records': dates,
-        'recorded_flows': recs.dropna(axis=0).values.flatten(),
-        'y_max': max(recs.values),
+        'recorded_flows': df.dropna(axis=0).values.flatten(),
+        'y_max': np.nanmax(df.values),
     }
     if rp_df is not None:
         plot_data.update(rp_df.to_dict(orient='index').items())
         rperiod_scatters = _rperiod_scatters(startdate, enddate, rp_df, plot_data['y_max'], plot_data['y_max'])
     else:
         rperiod_scatters = []
```

### Comparing `geoglows-1.2.1/geoglows/_plots/plotly_helpers.py` & `geoglows-1.3.0/geoglows/_plots/plotly_helpers.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.2.1/geoglows/_plots/plotly_retrospective.py` & `geoglows-1.3.0/geoglows/_plots/plotly_retrospective.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.2.1/geoglows/_plots/plots.py` & `geoglows-1.3.0/geoglows/_plots/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 import pandas as pd
 import plotly.graph_objects as go
 
 from .format_tools import plotly_figure_to_html_plot
+from .plotly_bias_corrected import (
+    corrected_retrospective as plotly_corrected_retrospective,
+    corrected_month_average as plotly_corrected_month_average,
+    corrected_day_average as plotly_corrected_day_average,
+    corrected_scatterplots as plotly_corrected_scatterplots,
+)
 from .plotly_forecasts import (
     forecast as plotly_forecast,
     forecast_stats as plotly_forecast_stats,
-    forecast_ensembles as plotly_forecast_ensembles
+    forecast_ensembles as plotly_forecast_ensembles,
+    forecast_records as plotly_forecast_records,
 )
 from .plotly_retrospective import (
     retrospective as plotly_retrospective,
     daily_averages as plotly_daily_averages,
     monthly_averages as plotly_monthly_averages,
     annual_averages as plotly_annual_averages,
     flow_duration_curve as plotly_flow_duration_curve,
 )
-from .plotly_bias_corrected import (
-    corrected_retrospective as plotly_corrected_retrospective,
-    corrected_month_average as plotly_corrected_month_average,
-    corrected_day_average as plotly_corrected_day_average,
-    corrected_scatterplots as plotly_corrected_scatterplots,
-)
 
 __all__ = [
     'forecast',
     'forecast_stats',
     'forecast_ensembles',
+    'forecast_records',
 
     'retrospective',
     'daily_averages',
     'monthly_averages',
     'annual_averages',
     'flow_duration_curve',
 
@@ -101,14 +103,37 @@
         figure = plotly_forecast_ensembles(df, rp_df=rp_df, plot_titles=plot_titles)
         if plot_type == 'html':
             return plotly_figure_to_html_plot(figure)
         return figure
     raise NotImplementedError(f'Plot type "{plot_type}" is not supported.')
 
 
+def forecast_records(df: pd.DataFrame, *,
+                     plot_type: str = 'plotly',
+                     rp_df: pd.DataFrame = None,
+                     plot_titles: list = None, ) -> go.Figure:
+    """
+    Plots forecasted streamflow and optional return periods
+    Args:
+        df:
+        plot_type:
+        rp_df:
+        plot_titles:
+
+    Returns:
+        go.Figure
+    """
+    if plot_type in ('plotly', 'html'):
+        figure = plotly_forecast_records(df, rp_df=rp_df, plot_titles=plot_titles)
+        if plot_type == 'html':
+            return plotly_figure_to_html_plot(figure)
+        return figure
+    raise NotImplementedError(f'Plot type "{plot_type}" is not supported.')
+
+
 def retrospective(df: pd.DataFrame, *,
                   plot_type: str = 'plotly',
                   rp_df: pd.DataFrame = None,
                   plot_titles: list = None, ) -> go.Figure:
     """
     Plots the retrospective simulation data
```

### Comparing `geoglows-1.2.1/geoglows/analyze.py` & `geoglows-1.3.0/geoglows/analyze.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.2.1/geoglows/bias.py` & `geoglows-1.3.0/geoglows/bias.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.2.1/geoglows/data.py` & `geoglows-1.3.0/geoglows/data.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.2.1/geoglows/streamflow.py` & `geoglows-1.3.0/geoglows/streamflow.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.2.1/geoglows/streams.py` & `geoglows-1.3.0/geoglows/streams.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.2.1/geoglows/tables.py` & `geoglows-1.3.0/geoglows/tables.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.2.1/geoglows.egg-info/PKG-INFO` & `geoglows-1.3.0/geoglows.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoglows
-Version: 1.2.1
+Version: 1.3.0
 Summary: Package for accessing data from the GEOGLOWS Hydrological Model
 Home-page: https://data.geoglows.org
 Author: Riley Hales PhD
 License: BSD 3-Clause Clear License
 Project-URL: Homepage, https://data.geoglows.org
 Project-URL: Documentation, https://geoglows.readthedocs.io
 Project-URL: Source, https://github.com/geoglows/pygeoglows
```

### Comparing `geoglows-1.2.1/geoglows.egg-info/SOURCES.txt` & `geoglows-1.3.0/geoglows.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geoglows-1.2.1/setup.py` & `geoglows-1.3.0/setup.py`

 * *Files identical despite different names*

