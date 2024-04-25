# Comparing `tmp/self_stats-0.1.0.tar.gz` & `tmp/self_stats-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "self_stats-0.1.0.tar", last modified: Tue Apr 23 20:17:38 2024, max compression
+gzip compressed data, was "self_stats-0.1.1.tar", last modified: Thu Apr 25 16:29:35 2024, max compression
```

## Comparing `self_stats-0.1.0.tar` & `self_stats-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2024-04-23 20:17:38.468108 self_stats-0.1.0/
--rw-r--r--   0 bio       (1000) bio       (1000)     7464 2024-04-23 20:17:38.468108 self_stats-0.1.0/PKG-INFO
--rw-r--r--   0 bio       (1000) bio       (1000)     5430 2024-04-23 19:17:32.000000 self_stats-0.1.0/README.md
-drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2024-04-23 20:17:38.468108 self_stats-0.1.0/app/
--rw-r--r--   0 bio       (1000) bio       (1000)        0 2024-04-15 18:42:24.000000 self_stats-0.1.0/app/__init__.py
--rw-r--r--   0 bio       (1000) bio       (1000)     1613 2024-04-23 19:26:57.000000 self_stats-0.1.0/app/__main__.py
-drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2024-04-23 20:17:38.468108 self_stats-0.1.0/app/dash_app/
--rw-r--r--   0 bio       (1000) bio       (1000)        0 2024-04-17 22:51:48.000000 self_stats-0.1.0/app/dash_app/__init__.py
--rw-r--r--   0 bio       (1000) bio       (1000)      650 2024-04-23 19:17:32.000000 self_stats-0.1.0/app/dash_app/dash_app_caller.py
--rw-r--r--   0 bio       (1000) bio       (1000)     7909 2024-04-23 19:17:32.000000 self_stats-0.1.0/app/dash_app/dash_callbacks.py
--rw-r--r--   0 bio       (1000) bio       (1000)      779 2024-04-17 19:05:11.000000 self_stats-0.1.0/app/dash_app/dash_layout.py
--rw-r--r--   0 bio       (1000) bio       (1000)      883 2024-04-18 17:52:10.000000 self_stats-0.1.0/app/dash_app/tz_offset.py
-drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2024-04-23 20:17:38.468108 self_stats-0.1.0/app/munger/
--rw-r--r--   0 bio       (1000) bio       (1000)        0 2024-04-17 22:51:36.000000 self_stats-0.1.0/app/munger/__init__.py
--rw-r--r--   0 bio       (1000) bio       (1000)     3018 2024-04-18 16:47:55.000000 self_stats-0.1.0/app/munger/changepoint_analysis.py
--rw-r--r--   0 bio       (1000) bio       (1000)     4456 2024-04-18 17:25:20.000000 self_stats-0.1.0/app/munger/clean_dates.py
--rw-r--r--   0 bio       (1000) bio       (1000)     1244 2024-04-18 16:47:13.000000 self_stats-0.1.0/app/munger/input_output.py
--rw-r--r--   0 bio       (1000) bio       (1000)     1181 2024-04-23 19:17:32.000000 self_stats-0.1.0/app/munger/munger_main.py
--rw-r--r--   0 bio       (1000) bio       (1000)     3559 2024-04-23 19:17:32.000000 self_stats-0.1.0/app/munger/parse_and_process.py
--rw-r--r--   0 bio       (1000) bio       (1000)     1054 2024-04-18 09:25:58.000000 self_stats-0.1.0/app/munger/selector.py
-drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2024-04-23 20:17:38.468108 self_stats-0.1.0/self_stats.egg-info/
--rw-r--r--   0 bio       (1000) bio       (1000)     7464 2024-04-23 20:17:38.000000 self_stats-0.1.0/self_stats.egg-info/PKG-INFO
--rw-r--r--   0 bio       (1000) bio       (1000)      709 2024-04-23 20:17:38.000000 self_stats-0.1.0/self_stats.egg-info/SOURCES.txt
--rw-r--r--   0 bio       (1000) bio       (1000)        1 2024-04-23 20:17:38.000000 self_stats-0.1.0/self_stats.egg-info/dependency_links.txt
--rw-r--r--   0 bio       (1000) bio       (1000)     1015 2024-04-23 20:17:38.000000 self_stats-0.1.0/self_stats.egg-info/requires.txt
--rw-r--r--   0 bio       (1000) bio       (1000)        4 2024-04-23 20:17:38.000000 self_stats-0.1.0/self_stats.egg-info/top_level.txt
--rw-r--r--   0 bio       (1000) bio       (1000)       38 2024-04-23 20:17:38.468108 self_stats-0.1.0/setup.cfg
--rw-r--r--   0 bio       (1000) bio       (1000)     2054 2024-04-23 20:13:38.000000 self_stats-0.1.0/setup.py
-drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2024-04-23 20:17:38.468108 self_stats-0.1.0/tests/
--rw-r--r--   0 bio       (1000) bio       (1000)     1207 2024-04-23 19:17:32.000000 self_stats-0.1.0/tests/test_clean_output_data.py
--rw-r--r--   0 bio       (1000) bio       (1000)     2153 2024-04-15 22:21:44.000000 self_stats-0.1.0/tests/test_extract.py
--rw-r--r--   0 bio       (1000) bio       (1000)     1824 2024-04-23 19:17:32.000000 self_stats-0.1.0/tests/test_process_search_history.py
--rw-r--r--   0 bio       (1000) bio       (1000)     1763 2024-04-23 19:17:32.000000 self_stats-0.1.0/tests/test_process_video_watch_history.py
--rw-r--r--   0 bio       (1000) bio       (1000)     1815 2024-04-23 19:17:32.000000 self_stats-0.1.0/tests/test_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:35.523725 self_stats-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-04-25 16:29:35.523725 self_stats-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5745 2024-04-25 16:29:26.000000 self_stats-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:35.519725 self_stats-0.1.1/self_stats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:26.000000 self_stats-0.1.1/self_stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-25 16:29:26.000000 self_stats-0.1.1/self_stats/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:35.523725 self_stats-0.1.1/self_stats/dash_app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:26.000000 self_stats-0.1.1/self_stats/dash_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-25 16:29:26.000000 self_stats-0.1.1/self_stats/dash_app/dash_app_caller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7916 2024-04-25 16:29:26.000000 self_stats-0.1.1/self_stats/dash_app/dash_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-25 16:29:26.000000 self_stats-0.1.1/self_stats/dash_app/dash_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-25 16:29:26.000000 self_stats-0.1.1/self_stats/dash_app/tz_offset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:35.523725 self_stats-0.1.1/self_stats/munger/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:26.000000 self_stats-0.1.1/self_stats/munger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-04-25 16:29:26.000000 self_stats-0.1.1/self_stats/munger/changepoint_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-04-25 16:29:26.000000 self_stats-0.1.1/self_stats/munger/clean_dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-25 16:29:26.000000 self_stats-0.1.1/self_stats/munger/input_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-25 16:29:26.000000 self_stats-0.1.1/self_stats/munger/munger_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-25 16:29:26.000000 self_stats-0.1.1/self_stats/munger/parse_and_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-25 16:29:26.000000 self_stats-0.1.1/self_stats/munger/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:35.523725 self_stats-0.1.1/self_stats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-04-25 16:29:35.000000 self_stats-0.1.1/self_stats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-25 16:29:35.000000 self_stats-0.1.1/self_stats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:29:35.000000 self_stats-0.1.1/self_stats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-25 16:29:35.000000 self_stats-0.1.1/self_stats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-25 16:29:35.000000 self_stats-0.1.1/self_stats.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 16:29:35.523725 self_stats-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-25 16:29:26.000000 self_stats-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:35.523725 self_stats-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-25 16:29:26.000000 self_stats-0.1.1/tests/test_clean_output_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-25 16:29:26.000000 self_stats-0.1.1/tests/test_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-25 16:29:26.000000 self_stats-0.1.1/tests/test_process_search_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-25 16:29:26.000000 self_stats-0.1.1/tests/test_process_video_watch_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-25 16:29:26.000000 self_stats-0.1.1/tests/test_selector.py
```

### Comparing `self_stats-0.1.0/PKG-INFO` & `self_stats-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: self_stats
-Version: 0.1.0
+Version: 0.1.1
 Summary: Process Google Takeout data and visualize it using Dash.
 Author: Colton Robbins
 Author-email: coltonrobbins73@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: alabaster==0.7.16
 Requires-Dist: Babel==2.14.0
 Requires-Dist: blinker==1.7.0
@@ -92,15 +92,15 @@
 ### Data Preparation
 
 #### Downloading Your Data from Google Takeout
 
 - Open your web browser and go to [Google Takeout](https://takeout.google.com/).
 - Google Takeout allows you to export data from your Google account products.
 - Choose the Google products you want data from. Ensure you have selected **"MyActivity"** and **"YouTube and YouTube Music"**
-- Change the file format to **JSON**.
+- Change the file format to **JSON**. The default is HTML and will be incompatible with this pipeline.
 - Once your archive is ready, Google will notify you via email.
 - Download the archive and extract it.
 
 ![Google Takeout Demo](gifs/Google_Takeout_instructions.gif)
 
 #### Setting Up the Visualizer
 
@@ -159,16 +159,19 @@
 ## Why Choose Google Takeout Data Insights Visualizer?
 
 Our tool not only visualizes your data from Google Takeout but also provides a powerful platform to uncover and understand personal trends and usage statistics, empowering you with the knowledge to make informed decisions about your digital privacy and online habits.
 
 # TODO
 
 - Make a blank data folder to submit to github for user access
-- Be more explicit about JSON settings for download
+  - The package version does not need this
 - Change package name to something different
+  - Better to change the repo name and keep the package the same
 - Add plot titles
 - Label axis better
 - Add modules to the init files
 - Document directory names
 - Make module docstrings
 - Leave some more comments throughout the script
--
+- Add logic to retain asset images in installed package
+  - Add assets to package directory and explicitly call for them with a MANIFEST.in file
+  - setup.py should include "package_data" element
```

### Comparing `self_stats-0.1.0/README.md` & `self_stats-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 ### Data Preparation
 
 #### Downloading Your Data from Google Takeout
 
 - Open your web browser and go to [Google Takeout](https://takeout.google.com/).
 - Google Takeout allows you to export data from your Google account products.
 - Choose the Google products you want data from. Ensure you have selected **"MyActivity"** and **"YouTube and YouTube Music"**
-- Change the file format to **JSON**.
+- Change the file format to **JSON**. The default is HTML and will be incompatible with this pipeline.
 - Once your archive is ready, Google will notify you via email.
 - Download the archive and extract it.
 
 ![Google Takeout Demo](gifs/Google_Takeout_instructions.gif)
 
 #### Setting Up the Visualizer
 
@@ -98,16 +98,19 @@
 ## Why Choose Google Takeout Data Insights Visualizer?
 
 Our tool not only visualizes your data from Google Takeout but also provides a powerful platform to uncover and understand personal trends and usage statistics, empowering you with the knowledge to make informed decisions about your digital privacy and online habits.
 
 # TODO
 
 - Make a blank data folder to submit to github for user access
-- Be more explicit about JSON settings for download
+  - The package version does not need this
 - Change package name to something different
+  - Better to change the repo name and keep the package the same
 - Add plot titles
 - Label axis better
 - Add modules to the init files
 - Document directory names
 - Make module docstrings
 - Leave some more comments throughout the script
--
+- Add logic to retain asset images in installed package
+  - Add assets to package directory and explicitly call for them with a MANIFEST.in file
+  - setup.py should include "package_data" element
```

### Comparing `self_stats-0.1.0/app/__main__.py` & `self_stats-0.1.1/self_stats/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from app.munger.selector import get_file_presence_flags
-from app.munger.munger_main import main as munger_main
-from app.dash_app.dash_app_caller import main as dash_main
+from self_stats.munger.selector import get_file_presence_flags
+from self_stats.munger.munger_main import main as munger_main
+from self_stats.dash_app.dash_app_caller import main as dash_main
 
 def main() -> None:
     """
     Main function that orchestr
     ates the processing of watch history and search history based on file presence.
     """
     skip_preprocess = False # This line will be used if the user just wants data viz functionality
@@ -37,11 +37,11 @@
     
     #TODO Implement dash visualization sub-module here
 
     viz_flag = 'watch'
 
     if viz_flag == 'watch':
         print("Visualizing watch history...\n")
-        dash_main('data/output/dash_ready_watch_data.csv')
+        dash_main(f'{directory}/output/dash_ready_watch_data.csv')
 
 if __name__ == "__main__":
     main()
```

### Comparing `self_stats-0.1.0/app/dash_app/dash_app_caller.py` & `self_stats-0.1.1/self_stats/dash_app/dash_app_caller.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dash import Dash
 from pathlib import Path
 
-import app.dash_app.dash_callbacks as dash_callbacks 
-from app.dash_app.dash_layout import create_layout
+import self_stats.dash_app.dash_callbacks as dash_callbacks 
+from self_stats.dash_app.dash_layout import create_layout
 
 def main(path: str | Path) -> None:
     """
     Main function that visualizes processed data using Dash.
     """
     app = Dash(__name__)
     app.layout = create_layout()
```

### Comparing `self_stats-0.1.0/app/dash_app/dash_callbacks.py` & `self_stats-0.1.1/self_stats/dash_app/dash_callbacks.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import pandas as pd
 import plotly.express as px
 from plotly.graph_objs import Figure
 from dash import Dash
 from dash.dependencies import Input, Output, State
 
-from app.dash_app.tz_offset import get_utc_offset, adjust_time_by_utc_offset
+from self_stats.dash_app.tz_offset import get_utc_offset, adjust_time_by_utc_offset
 
 def load_data(n: int, path: Union[str, Path]) -> str:
     """
     Loads and preprocesses data at regular intervals, specified by `n_intervals`.
     This function reads data from a CSV file specified by `path`, preprocesses it,
     and returns a JSON string containing the preprocessed data.
```

### Comparing `self_stats-0.1.0/app/dash_app/dash_layout.py` & `self_stats-0.1.1/self_stats/dash_app/dash_layout.py`

 * *Files identical despite different names*

### Comparing `self_stats-0.1.0/app/dash_app/tz_offset.py` & `self_stats-0.1.1/self_stats/dash_app/tz_offset.py`

 * *Files identical despite different names*

### Comparing `self_stats-0.1.0/app/munger/changepoint_analysis.py` & `self_stats-0.1.1/self_stats/munger/changepoint_analysis.py`

 * *Files identical despite different names*

### Comparing `self_stats-0.1.0/app/munger/clean_dates.py` & `self_stats-0.1.1/self_stats/munger/clean_dates.py`

 * *Files identical despite different names*

### Comparing `self_stats-0.1.0/app/munger/input_output.py` & `self_stats-0.1.1/self_stats/munger/input_output.py`

 * *Files identical despite different names*

### Comparing `self_stats-0.1.0/app/munger/munger_main.py` & `self_stats-0.1.1/self_stats/munger/munger_main.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from typing import List
 
-from app.munger.input_output import save_to_csv
-from app.munger.changepoint_analysis import trim_date
-from app.munger.parse_and_process import main as parse_and_process
+from self_stats.munger.input_output import save_to_csv
+from self_stats.munger.changepoint_analysis import trim_date
+from self_stats.munger.parse_and_process import main as parse_and_process
 
 def main(directory: str, input_file_name: str, mappings: List[str]) -> None:
 
     if mappings[0] == 'Text Title':
         data_source = 'search'
     elif mappings[0] == 'Video URL':
         data_source = 'watch'
```

### Comparing `self_stats-0.1.0/app/munger/parse_and_process.py` & `self_stats-0.1.1/self_stats/munger/parse_and_process.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple
 from urllib.parse import parse_qs, urlparse
 
-from app.munger.clean_dates import convert_to_arrays, main as cleaner_main
-from app.munger.input_output import read_json_file
+from self_stats.munger.clean_dates import convert_to_arrays, main as cleaner_main
+from self_stats.munger.input_output import read_json_file
 
 def extract_coordinates(location_url: str) -> Tuple[Optional[float], Optional[float]]:
     """
     Extracts latitude and longitude from a location URL.
 
     Args:
         location_url (str): The URL containing the geolocation coordinates.
```

### Comparing `self_stats-0.1.0/app/munger/selector.py` & `self_stats-0.1.1/self_stats/munger/selector.py`

 * *Files identical despite different names*

### Comparing `self_stats-0.1.0/self_stats.egg-info/PKG-INFO` & `self_stats-0.1.1/self_stats.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: self_stats
-Version: 0.1.0
+Version: 0.1.1
 Summary: Process Google Takeout data and visualize it using Dash.
 Author: Colton Robbins
 Author-email: coltonrobbins73@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: alabaster==0.7.16
 Requires-Dist: Babel==2.14.0
 Requires-Dist: blinker==1.7.0
@@ -92,15 +92,15 @@
 ### Data Preparation
 
 #### Downloading Your Data from Google Takeout
 
 - Open your web browser and go to [Google Takeout](https://takeout.google.com/).
 - Google Takeout allows you to export data from your Google account products.
 - Choose the Google products you want data from. Ensure you have selected **"MyActivity"** and **"YouTube and YouTube Music"**
-- Change the file format to **JSON**.
+- Change the file format to **JSON**. The default is HTML and will be incompatible with this pipeline.
 - Once your archive is ready, Google will notify you via email.
 - Download the archive and extract it.
 
 ![Google Takeout Demo](gifs/Google_Takeout_instructions.gif)
 
 #### Setting Up the Visualizer
 
@@ -159,16 +159,19 @@
 ## Why Choose Google Takeout Data Insights Visualizer?
 
 Our tool not only visualizes your data from Google Takeout but also provides a powerful platform to uncover and understand personal trends and usage statistics, empowering you with the knowledge to make informed decisions about your digital privacy and online habits.
 
 # TODO
 
 - Make a blank data folder to submit to github for user access
-- Be more explicit about JSON settings for download
+  - The package version does not need this
 - Change package name to something different
+  - Better to change the repo name and keep the package the same
 - Add plot titles
 - Label axis better
 - Add modules to the init files
 - Document directory names
 - Make module docstrings
 - Leave some more comments throughout the script
--
+- Add logic to retain asset images in installed package
+  - Add assets to package directory and explicitly call for them with a MANIFEST.in file
+  - setup.py should include "package_data" element
```

### Comparing `self_stats-0.1.0/self_stats.egg-info/requires.txt` & `self_stats-0.1.1/self_stats.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `self_stats-0.1.0/setup.py` & `self_stats-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='self_stats',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
     install_requires=[
         'alabaster==0.7.16',
         'Babel==2.14.0',
         'blinker==1.7.0',
         'certifi==2024.2.2',
         'charset-normalizer==3.3.2',
```

### Comparing `self_stats-0.1.0/tests/test_clean_output_data.py` & `self_stats-0.1.1/tests/test_clean_output_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 import regex as re
 from datetime import datetime
-from app.munger.search_cleaner import remove_invisible_characters, remove_timezone, parse_date, process_row, clean_and_convert_data
+from self_stats.munger.search_cleaner import remove_invisible_characters, remove_timezone, parse_date, process_row, clean_and_convert_data
 
 class TestYourModule(unittest.TestCase):
     def setUp(self):
         # This is the regex pattern compiled once for all tests.
         self.pattern = re.compile(r'\p{C}+|\p{Z}+|[\u200B-\u200F\u2028-\u202F]+')
 
     def test_remove_invisible_characters(self):
```

### Comparing `self_stats-0.1.0/tests/test_extract.py` & `self_stats-0.1.1/tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `self_stats-0.1.0/tests/test_process_search_history.py` & `self_stats-0.1.1/tests/test_process_search_history.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 from unittest.mock import patch, Mock
 from bs4 import BeautifulSoup
 
 # Assuming the script's functions are in a module named 'script'
-from app.process_search_history import extract_search_data, extract_search_text, extract_date, extract_coordinates
+from self_stats.process_search_history import extract_search_data, extract_search_text, extract_date, extract_coordinates
 
 class TestScript(unittest.TestCase):
     def setUp(self):
         self.html_content = "<html><body><a href='http://maps.example.com/?center=40.7128,-74.0060' text='this general area'>Location</a></body></html>"
         self.soup = BeautifulSoup(self.html_content, 'html.parser')
         self.entry = self.soup.new_tag('div')
         self.entry.append(self.soup.new_tag('a', href="http://example.com"))
```

### Comparing `self_stats-0.1.0/tests/test_process_video_watch_history.py` & `self_stats-0.1.1/tests/test_process_video_watch_history.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 from unittest.mock import patch, Mock
 from bs4 import BeautifulSoup
 
 # Assuming the script's functions are in a module named 'video_script'
-from app.process_watch_history import extract_video_data, extract_video_field, extract_date
+from self_stats.process_watch_history import extract_video_data, extract_video_field, extract_date
 d
 class TestVideoScript(unittest.TestCase):
     def setUp(self):
         self.html_content = "<html><body><div><a href='http://youtube.com/watch?v=example'>Video Title</a><a href='http://youtube.com/channel'>Channel Title</a></div></body></html>"
         self.soup = BeautifulSoup(self.html_content, 'html.parser')
         self.entry = self.soup.find('div')
```

### Comparing `self_stats-0.1.0/tests/test_selector.py` & `self_stats-0.1.1/tests/test_selector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 from unittest.mock import patch, MagicMock
-from app.munger.selector import ensure_directory_exists, get_file_presence_flags
+from self_stats.munger.selector import ensure_directory_exists, get_file_presence_flags
 
 class TestSelector(unittest.TestCase):
     def test_ensure_directory_exists(self):
         with patch('selector.Path') as mock_path:
             mock_path.return_value.is_dir.return_value = True
             # Test that no exception is raised for existing directory
             try:
```

