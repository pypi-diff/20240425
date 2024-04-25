# Comparing `tmp/multidefusion-0.0.16.tar.gz` & `tmp/multidefusion-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multidefusion-0.0.16.tar", last modified: Thu Apr 25 11:48:26 2024, max compression
+gzip compressed data, was "multidefusion-0.0.6.tar", last modified: Wed Apr 10 15:01:04 2024, max compression
```

## Comparing `multidefusion-0.0.16.tar` & `multidefusion-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 11:48:26.752404 multidefusion-0.0.16/
--rw-rw-rw-   0        0        0      175 2024-04-25 10:36:12.000000 multidefusion-0.0.16/AUTHORS.rst
--rw-rw-rw-   0        0        0      129 2024-04-25 10:36:12.000000 multidefusion-0.0.16/MANIFEST.in
--rw-rw-rw-   0        0        0     1422 2024-04-25 11:48:26.752404 multidefusion-0.0.16/PKG-INFO
--rw-rw-rw-   0        0        0      614 2024-04-25 10:36:12.000000 multidefusion-0.0.16/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 11:48:26.736780 multidefusion-0.0.16/multidefusion/
--rw-rw-rw-   0        0        0      142 2024-04-25 10:36:12.000000 multidefusion-0.0.16/multidefusion/__init__.py
--rw-rw-rw-   0        0        0    19080 2024-04-20 15:07:40.000000 multidefusion-0.0.16/multidefusion/datainterface.py
--rw-rw-rw-   0        0        0     2898 2024-04-24 18:40:07.000000 multidefusion-0.0.16/multidefusion/fusion.py
--rw-rw-rw-   0        0        0    26310 2024-04-22 12:20:09.000000 multidefusion-0.0.16/multidefusion/integration.py
--rw-rw-rw-   0        0        0    52030 2024-04-24 18:42:36.000000 multidefusion-0.0.16/multidefusion/results.py
-drwxrwxrwx   0        0        0        0 2024-04-25 11:48:26.752404 multidefusion-0.0.16/multidefusion.egg-info/
--rw-rw-rw-   0        0        0     1422 2024-04-25 11:48:26.000000 multidefusion-0.0.16/multidefusion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      416 2024-04-25 11:48:26.000000 multidefusion-0.0.16/multidefusion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 11:48:26.000000 multidefusion-0.0.16/multidefusion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-25 11:46:42.000000 multidefusion-0.0.16/multidefusion.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       14 2024-04-25 11:48:26.000000 multidefusion-0.0.16/multidefusion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-04-25 10:36:12.000000 multidefusion-0.0.16/requirements.txt
--rw-rw-rw-   0        0        0      421 2024-04-25 11:48:26.752404 multidefusion-0.0.16/setup.cfg
--rw-rw-rw-   0        0        0     1831 2024-04-25 11:47:56.000000 multidefusion-0.0.16/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 11:48:26.752404 multidefusion-0.0.16/tests/
--rw-rw-rw-   0        0        0      438 2024-04-25 10:36:12.000000 multidefusion-0.0.16/tests/test_multidefusion.py
+drwxrwxrwx   0        0        0        0 2024-04-10 15:01:04.511137 multidefusion-0.0.6/
+-rw-rw-rw-   0        0        0      175 2024-04-10 14:26:29.000000 multidefusion-0.0.6/AUTHORS.rst
+-rw-rw-rw-   0        0        0     1094 2024-04-10 14:26:29.000000 multidefusion-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      129 2024-04-10 14:26:29.000000 multidefusion-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1594 2024-04-10 15:01:04.509632 multidefusion-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      614 2024-04-10 14:26:29.000000 multidefusion-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 15:01:04.490536 multidefusion-0.0.6/multidefusion/
+-rw-rw-rw-   0        0        0      142 2024-04-10 14:26:29.000000 multidefusion-0.0.6/multidefusion/__init__.py
+-rw-rw-rw-   0        0        0      194 2024-04-10 14:26:29.000000 multidefusion-0.0.6/multidefusion/common.py
+-rw-rw-rw-   0        0        0    19053 2024-04-10 14:43:27.000000 multidefusion-0.0.6/multidefusion/datainterface.py
+-rw-rw-rw-   0        0        0     1705 2024-04-10 14:42:56.000000 multidefusion-0.0.6/multidefusion/fusion.py
+-rw-rw-rw-   0        0        0    26603 2024-04-10 14:43:21.000000 multidefusion-0.0.6/multidefusion/integration.py
+-rw-rw-rw-   0        0        0       20 2024-04-10 14:26:29.000000 multidefusion-0.0.6/multidefusion/multidefusion.py
+-rw-rw-rw-   0        0        0    45552 2024-04-10 14:43:34.000000 multidefusion-0.0.6/multidefusion/results.py
+drwxrwxrwx   0        0        0        0 2024-04-10 15:01:04.508643 multidefusion-0.0.6/multidefusion.egg-info/
+-rw-rw-rw-   0        0        0     1594 2024-04-10 15:01:04.000000 multidefusion-0.0.6/multidefusion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      515 2024-04-10 15:01:04.000000 multidefusion-0.0.6/multidefusion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       70 2024-04-10 15:01:04.000000 multidefusion-0.0.6/multidefusion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-10 14:55:46.000000 multidefusion-0.0.6/multidefusion.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       70 2024-04-10 15:01:04.000000 multidefusion-0.0.6/multidefusion.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-10 15:01:04.000000 multidefusion-0.0.6/multidefusion.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       73 2024-04-10 14:50:44.000000 multidefusion-0.0.6/requirements.txt
+-rw-rw-rw-   0        0        0      421 2024-04-10 15:01:04.512144 multidefusion-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1830 2024-04-10 15:00:13.000000 multidefusion-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 15:01:04.505637 multidefusion-0.0.6/tests/
+-rw-rw-rw-   0        0        0      438 2024-04-10 14:26:29.000000 multidefusion-0.0.6/tests/test_multidefusion.py
```

### Comparing `multidefusion-0.0.16/PKG-INFO` & `multidefusion-0.0.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multidefusion
-Version: 0.0.16
+Version: 0.0.6
 Summary: Perform data fusion and analysis of the ground deformations for multiple stations.
 Home-page: https://github.com/damiantondas/multidefusion
 Author: Damian Tondas
 Author-email: damian.tondas@gmail.com
 License: MIT license
 Keywords: multidefusion
 Classifier: Intended Audience :: Developers
@@ -13,15 +13,21 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: numpy==1.24.4
+Requires-Dist: pandas==2.0.3
+Requires-Dist: scipy==1.10.1
+Requires-Dist: plotly==5.20.0
+Requires-Dist: dash==2.16.1
 
 # multidefusion
 
 
 [![image](https://img.shields.io/pypi/v/multidefusion.svg)](https://pypi.python.org/pypi/multidefusion)
 [![image](https://img.shields.io/conda/vn/conda-forge/multidefusion.svg)](https://anaconda.org/conda-forge/multidefusion)
```

### Comparing `multidefusion-0.0.16/README.md` & `multidefusion-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `multidefusion-0.0.16/multidefusion/datainterface.py` & `multidefusion-0.0.6/multidefusion/datainterface.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,25 +115,25 @@
                     return data_by_date
         return None
 
     def process_timestamp_columns(self) -> None:
         """
         Process timestamp columns in the data.
 
-        Converts GNSS, SBAS, and PSI "YYYY", "MM", "DD" columns into a single "timestamp" column,
+        Converts "YYYY", "MM", "DD" columns into a single "timestamp" column,
         sets it as the index, and resamples the data based on the time interval.
         """
         self.data["timestamp"] = pd.to_datetime(self.data[["YYYY", "MM", "DD"]].astype(int).astype(str).apply(" ".join, 1), format="%Y %m %d")
         self.data = self.data.drop(["YYYY", "MM", "DD"], axis=1)
         self.data.set_index(["timestamp"], inplace=True)
         self.data = self.data.resample(self.TIME_INTERVAL).asfreq()
 
     def convert_range_into_two_timestamps(self) -> None:
         """
-        Convert DInSAR range columns into two timestamp columns.
+        Convert range columns into two timestamp columns.
 
         Converts "YYYY1", "MM1", "DD1", "YYYY2", "MM2", "DD2" columns into
         "timestamp1" and "timestamp2" columns, and sets them as the index.
         """
         self.data["timestamp1"] = pd.to_datetime(self.data[["YYYY1", "MM1", "DD1"]].astype(int).astype(str).apply(" ".join, 1), format="%Y %m %d")
         self.data["timestamp2"] = pd.to_datetime(self.data[["YYYY2", "MM2", "DD2"]].astype(int).astype(str).apply(" ".join, 1), format="%Y %m %d")
         self.data = self.data.drop(["YYYY1", "MM1", "DD1", "YYYY2", "MM2", "DD2"], axis=1)
```

### Comparing `multidefusion-0.0.16/multidefusion/integration.py` & `multidefusion-0.0.6/multidefusion/integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 class DataIntegration:
     """
     Class for integrating and processing different types of data using the Kalman filter.
 
     Args:
         station_name (str): The name of the station.
         path (str): The base path where data files are located.
-        noise (float): The noise parameter for the Kalman filter.
         port (int): The port is necessary for parallel displaying of subsequent integration results on localhost.
 
     Attributes:
         station (str): The name of the station.
         path (str): The base path where data files are located.
         data_dict (Dict[str, Dict[str, Any]]): A dictionary containing data objects organized by data type and label.
         mean_data_dict (Dict[str, Dict[str, Any]]): Dictionary to store averaged data after integration is performed.
@@ -34,14 +33,23 @@
     """
 
     N = 6
     TIME_INTERVAL_NUM = 1
     TIME_INTERVAL = 'D'
 
     def __init__(self, station_name: str, path: str, noise: float, port: int) -> None:
+        """
+        Initializes DataIntegration object.
+
+        Args:
+            station_name (str): The name of the station.
+            path (str): The base path where data files are located.
+            noise (float): The noise parameter for the Kalman filter.
+            port (int): The definition of subsequent port on localhost.
+        """
         self.station = station_name
         self.path = path
         self.port = port
         self.data_dict = {}
         self.mean_data_dict = {}
         self.predicted_state_and_variance = {}
         self.filtered_state_and_variance = {}
@@ -278,15 +286,15 @@
             number=parts[1]
         
         if len(parts)<=2:
             suffix = False
         else:
             suffix = parts[2][0].isdigit()
             
-            if suffix is True:
+            if suffix is False:
                 suffix2 = parts[2][0]
 
         return (prefix, number, suffix, suffix2)
 
     def sar_data_validation(self):
         """
         Validates SAR data and applies bias reduction if necessary.
```

### Comparing `multidefusion-0.0.16/multidefusion/results.py` & `multidefusion-0.0.6/multidefusion/results.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,47 +1,17 @@
 import plotly.graph_objects as go
 import plotly.subplots as sp
 from dateutil.relativedelta import relativedelta
 import pandas as pd
 from statistics import mean
-from dash import dash, dcc, html, Input, Output, ctx
+from dash import dash, dcc, html, Input, Output
 import webbrowser
 
 class Figures:
-    """Class for creating displacement plots.
-    
-    The final plot is created involving the Plotly library and Dash framework. The graphic representation of the results is automatically launched on the localhost server on port 8050.
-
-    The most important plot features:
-
-    1. Visualisation: The default port for displaying results on localhost is 8050. For more than one station, the outputs will be displayed simultaneously on consecutive ports.
-    2. Legend: Work for all of the traces and provide a general overview of the results by activating or deactivating groups of data using the legend entities.
-    3. Hover: Working within a single trace and providing a detailed overview of the results using the cursor.
-    4. Table: To provide the most relevant information about the integration procedure.
-    5. Customisation: To provide individual ranges for dates or values:
-        - Dates range: adjustable by providing initial and last date or by using the calendar.
-        - Horizontal range: adjustable by providing minimum and maximum values.
-        - Vertical & LOS range: adjustable by providing minimum and maximum values.
-        - Rate range: adjustable by providing minimum and maximum values.
-    6. Buttons: To facilitate manipulation between the traces:
-        - Restore default: Restore the original ranges of dates or values after user manipulations.
-        - Sync ranges: To synchronise the ranges to the same values (by default, the horizontal and vertical ranges of displacement are disjoint).
-    7. Mode bar: A default toolbar of the plotly library located in the top right corner:
-        - Download plot: To save the plot in svg format after user's manipulations.
-        - Edit in Chart Studio: To provide more advanced modifications in the plotly Chart Studio.
-        - Zoom: Work for a selected part of the trace. Double click on the trace to zoom back out.
-        - Pan: Working within a single trace by moving the current view of the trace.
-        - Draw line: Working within a single trace.
-        - Draw circle: Working within a single trace.
-        - Draw rectangle: Working within a single trace.
-        - Erase the active shape: A single-click to activate the shape.
-        - Zoom in: Work simultaneously for all of the traces.
-        - Zoom out: Work simultaneously for all of the traces.
-        - Reset axes: Work simultaneously for all of the traces.
-    """
+    """Class for creating displacement plots."""
     def __init__(self, data_integration):
         """
         Initialize Figures object.
 
         Args:
             data_integration (object): Object containing integrated data.
         """
@@ -90,40 +60,20 @@
         if not lists:
             return None
         flattened_list = [item for sublist in lists for item in sublist]
         return max(flattened_list)
     
     @staticmethod
     def find_max_total(df):
-        """
-        Find the maximum value (positive or negative) from each column from a set of dataframe.
-
-        Args:
-            df: dataframe
-
-        Returns:
-            Maximum value from from each column from a set of dataframe.
-        """
         return df.apply(lambda col: col.max() if col.max() >= -col.min() else col.min(), axis=0)
     
     @staticmethod
     def add_vline(fig, timestamp_min_value, timestamp_max_value, row, col):    
-        """
-        Add Thicker line for each subplot to indicate the beginning of a year
-
-        Args:
-            fig: Figure
-            timestamp_min_value: Earliest date
-            timestamp_max_value: Lastest date
-            row: figure's row
-            col: figure's column
-
-        Returns:
-            None
-        """
+        # THICKER LINE TO INDICATE THE BEGINNING OF THE YEAR
+        
         [fig.add_shape(x0=date, x1=date, y0=-10, y1=10, type="line", line=dict(color='lightgray', width=2), layer="below", row=row, col=col) for date in
         pd.date_range(start=timestamp_min_value - relativedelta(years=2),
         end=timestamp_max_value + relativedelta(years=2), freq='YS')]
 
     def create_displacement_plot(self):
         """
         Create displacement plot using Plotly and Dash.
@@ -705,92 +655,61 @@
                 figure = fig,
                 config = {
                     'toImageButtonOptions': {'format': 'svg', 'filename': 'MultiDEFusion_'+self.data_integration.station},
                     'displaylogo': False,
                     'showEditInChartStudio': True,
                     'plotlyServerURL': "https://chart-studio.plotly.com",
                     'modeBarButtonsToRemove': ['select', 'lasso2d', 'autoScale'],
-                    'modeBarButtonsToAdd': ['drawline', 'drawcircle', 'drawrect', 'eraseshape', 'sendDataToCloud']
+                    'modeBarButtonsToAdd': ['zoomIn2d', 'zoomOut2d', 'drawline', 'drawcircle', 'drawrect', 'eraseshape', 'sendDataToCloud']
                     }
-                ),
-            ])
+            ),])
         
         container2 = html.Div([
             html.H2('Customise dates range',
                     style={'fontsize': '25px',
-                           'margin-bottom': '5px',
-                           'margin-left': '65px',}),
+                           'margin-bottom': '5px'}),
             
 		    dcc.DatePickerRange(
 				id='date_range',
+				#initial_visible_month=dates_range[0],
 				display_format='DD/MM/YYYY',
 				show_outside_days = True,
 				start_date=dates_range[0],
 				end_date=dates_range[1],
                 number_of_months_shown=2,
                 style={'border': '2px solid black',
-                       'margin-bottom': '10px',
-                       'vertical-align': 'middle',
-                       'display': 'inline-block'},
+                       'margin-bottom': '10px'},
 			),
             
-            html.Button('Restore default',
-                        id='reset_dates',
-                        n_clicks=0,
-                        style={'fontsize': '20px',
-                               'font-weight': 'bold',
-                               'height': '45px', 
-                               'width': '100px', 
-                               'margin-left': '10px',
-                               'margin-bottom': '10px',
-                               'vertical-align': 'middle',
-                               'display': 'inline-block'}),
-            
             html.Div(id='output_x_range',
                      style={'fontsize': '15px',
                             'color': 'red'}),
             
             html.H2('Customise values range',
                     style={'fontsize': '25px',
-                           'margin-bottom': '5px',
-                           'margin-left': '60px'}),
-                                     
-            html.Div([
+                           'margin-bottom': '5px'}),
+                           
             dcc.Dropdown(
                 id = 'show_or_hide',
                 options=[
                     {'label': 'Horizontal range [m]', 'value': 'hor'},
                     {'label': 'Vertical & LOS range [m]', 'value': 'ver'},
-                    {'label': 'Rate range [mm/day]', 'value': 'rate'}],
+                    {'label': 'Rate range [mm/day]', 'value': 'rate'}
+                ],
                 value = 'hor',
                 clearable = False,
                 style={'width': '286px',
                        'font-size': '20px', 
                        'border': '0.2px solid black',
                        'border-radius': '0',
                        'height': '40px', 
-                       'vertical-align': 'middle',
-                       'display': 'inline-block'},
-            ),
-            
-            html.Button('Sync ranges',
-                        id='fit_ranges',
-                        n_clicks=0,
-                        style={'fontsize': '20px',
-                               'font-weight': 'bold',
-                               'height': '38px', 
-                               'width': '100px',
-                               'margin-left': '10px',
-                               'vertical-align': 'middle',
-                               'display': 'inline-block'}
+                       'margin-bottom': '5px'},
             ),
-            ]),
 
-            html.Div([
-                html.Div(id = 'hor_options', children=[
+            html.Div(id = 'hor_options', children=[
                 dcc.Input(
                 id = 'hor_min',
                 placeholder = 'Minimum value',
                 type='number',
                 step = 0.001,
                 value = float("{:.3f}".format(range_hor[0])),
                 style = {'font-size': '17px',
@@ -808,15 +727,14 @@
                 style = {'font-size': '17px',
                          'border': '1px solid black',
                          'height': '30px', 
                          'width': '138px'}
                 )
             ],
             style={'display': 'block',
-                   'margin-top': '5px',
                    'margin-bottom': '10px'},
             ),
             
             html.Div(id = 'ver_options', children=[
                 dcc.Input(
                 id = 'ver_min',
                 placeholder = 'Minimum value',
@@ -864,58 +782,41 @@
                 type='number',
                 step = 0.1,
                 value = float("{:.1f}".format(range_rate[1])),
                 style = {'font-size': '17px', 
                          'border': '1px solid black',
                          'height': '30px', 
                          'width': '138px'}
-                ),
-                
+                )
             ],
             style={'display': 'block',
                    'margin-bottom': '10px'},
-            )
-            ], style={'display': 'inline-block',
-                      'vertical-align': 'middle'}),
-
-            
-            html.Button('Restore default',
-                        id='reset_values',
-                        n_clicks=0,
-                        style={'fontsize': '20px',
-                               'font-weight': 'bold',
-                               'height': '38px', 
-                               'width': '100px',
-                               'margin-left': '10px',
-                               'display': 'inline-block',
-                               'vertical-align': 'middle',}
             ),
             
-            
             html.Div(id='output_y_range',
                      style={'fontsize': '15px',
                             'color': 'red'}
-                     ),
+                     )
         ], 
         style={'position': 'absolute', 
                'top': f'{picker_position}px', 
-               'left': '145px', 
+               'left': '155px', 
                'width': 'fit-content',
                'fontFamily': 'Helvetica',
                'color': 'black', 
                }
         )
         
         app.layout = html.Div([container1, container2])
 		
         @app.callback(
-            Output('hor_options', 'style'),
-            Output('ver_options', 'style'),
-            Output('rate_options', 'style'),
-            Input('show_or_hide', 'value'))
+           Output('hor_options', 'style'),
+           Output('ver_options', 'style'),
+           Output('rate_options', 'style'),
+           Input('show_or_hide', 'value'))
 
         def show_hide_element(visibility_state):
             if visibility_state == 'hor':
                 return {'display': 'block'}, {'display': 'none'}, {'display': 'none'}
             elif visibility_state == 'ver':
                 return {'display': 'none'}, {'display': 'block'}, {'display': 'none'}
             else:
@@ -966,41 +867,11 @@
                     fig.update_yaxes(range=[ver_min, ver_max], row=3)
                 
                 # UPDATE X AND Y RANGE FOR DInSAR WITH PSI& SBAS
                 fig.update_yaxes(range=[rate_min, rate_max], row=4)
         
             return fig, warning_dates, warning_values
         
-
-        @app.callback(
-            Output('date_range', 'start_date'),
-            Output('date_range', 'end_date'),
-            Input('reset_dates', 'n_clicks')
-        )
-        
-        def reset_date_range(n_clicks):
-            return dates_range[0], dates_range[1]
-        
-        @app.callback(
-          [Output('hor_min', 'value'), 
-            Output('hor_max', 'value'),
-            Output('ver_min', 'value'), 
-            Output('ver_max', 'value'),
-            Output('rate_min', 'value'), 
-            Output('rate_max', 'value')],
-            Input('reset_values', 'n_clicks'),
-            Input('fit_ranges', 'n_clicks'),
-            prevent_initial_call=True
-          )
-        
-        def reset_fit_range(btn1, btn2):
-            min_range = float("{:.3f}".format(min(range_ver[0], range_hor[0])))
-            max_range = float("{:.3f}".format(max(range_ver[1], range_hor[1])))
-            if 'reset_values' == ctx.triggered_id:
-                return float("{:.3f}".format(range_hor[0])), float("{:.3f}".format(range_hor[1])), float("{:.3f}".format(range_ver[0])), float("{:.3f}".format(range_ver[1])),  float("{:.1f}".format(range_rate[0])), float("{:.1f}".format(range_rate[1]))
-            if 'fit_ranges' == ctx.triggered_id:
-                return min_range, max_range, min_range, max_range, float("{:.1f}".format(range_rate[0])), float("{:.1f}".format(range_rate[1]))
-       
         
         print("MultiDEFusion procedure accomplished.\n")
         app.run_server(debug=True, host="localhost", port=self.data_integration.port);
         webbrowser.open(f'http://localhost:{self.data_integration.port}')
```

### Comparing `multidefusion-0.0.16/multidefusion.egg-info/PKG-INFO` & `multidefusion-0.0.6/multidefusion.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multidefusion
-Version: 0.0.16
+Version: 0.0.6
 Summary: Perform data fusion and analysis of the ground deformations for multiple stations.
 Home-page: https://github.com/damiantondas/multidefusion
 Author: Damian Tondas
 Author-email: damian.tondas@gmail.com
 License: MIT license
 Keywords: multidefusion
 Classifier: Intended Audience :: Developers
@@ -13,15 +13,21 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: numpy==1.24.4
+Requires-Dist: pandas==2.0.3
+Requires-Dist: scipy==1.10.1
+Requires-Dist: plotly==5.20.0
+Requires-Dist: dash==2.16.1
 
 # multidefusion
 
 
 [![image](https://img.shields.io/pypi/v/multidefusion.svg)](https://pypi.python.org/pypi/multidefusion)
 [![image](https://img.shields.io/conda/vn/conda-forge/multidefusion.svg)](https://anaconda.org/conda-forge/multidefusion)
```

### Comparing `multidefusion-0.0.16/setup.py` & `multidefusion-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,10 +48,10 @@
     keywords='multidefusion',
     name='multidefusion',
     packages=find_packages(include=['multidefusion', 'multidefusion.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/damiantondas/multidefusion',
-    version='0.0.16',
+    version='0.0.6',
     zip_safe=False,
 )
```

