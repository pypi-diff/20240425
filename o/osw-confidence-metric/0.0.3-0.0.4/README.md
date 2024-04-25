# Comparing `tmp/osw_confidence_metric-0.0.3-py3-none-any.whl.zip` & `tmp/osw_confidence_metric-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 12140 bytes, number of entries: 11
--rw-r--r--  2.0 unx       32 b- defN 24-Jan-30 18:20 osw_confidence_metric/__init__.py
--rw-r--r--  2.0 unx     4627 b- defN 24-Jan-30 18:20 osw_confidence_metric/area_analyzer.py
--rw-r--r--  2.0 unx      964 b- defN 24-Jan-30 18:20 osw_confidence_metric/osm_data_handler.py
--rw-r--r--  2.0 unx     8192 b- defN 24-Jan-30 18:20 osw_confidence_metric/trust_score_calculator.py
--rw-r--r--  2.0 unx    12040 b- defN 24-Jan-30 18:20 osw_confidence_metric/utils.py
--rw-r--r--  2.0 unx       21 b- defN 24-Jan-30 18:20 osw_confidence_metric/version.py
--rw-r--r--  2.0 unx     1073 b- defN 24-Jan-30 18:20 osw_confidence_metric-0.0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx    10561 b- defN 24-Jan-30 18:20 osw_confidence_metric-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jan-30 18:20 osw_confidence_metric-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       22 b- defN 24-Jan-30 18:20 osw_confidence_metric-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1016 b- defN 24-Jan-30 18:20 osw_confidence_metric-0.0.3.dist-info/RECORD
-11 files, 38640 bytes uncompressed, 10382 bytes compressed:  73.1%
+Zip file size: 12184 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       32 b- defN 24-Apr-25 05:05 osw_confidence_metric/__init__.py
+-rw-r--r--  2.0 unx     4705 b- defN 24-Apr-25 05:05 osw_confidence_metric/area_analyzer.py
+-rw-r--r--  2.0 unx      964 b- defN 24-Apr-25 05:05 osw_confidence_metric/osm_data_handler.py
+-rw-r--r--  2.0 unx     8192 b- defN 24-Apr-25 05:05 osw_confidence_metric/trust_score_calculator.py
+-rw-r--r--  2.0 unx    12040 b- defN 24-Apr-25 05:05 osw_confidence_metric/utils.py
+-rw-r--r--  2.0 unx       21 b- defN 24-Apr-25 05:05 osw_confidence_metric/version.py
+-rw-r--r--  2.0 unx     1073 b- defN 24-Apr-25 05:05 osw_confidence_metric-0.0.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx    10561 b- defN 24-Apr-25 05:05 osw_confidence_metric-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-25 05:05 osw_confidence_metric-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       22 b- defN 24-Apr-25 05:05 osw_confidence_metric-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1016 b- defN 24-Apr-25 05:05 osw_confidence_metric-0.0.4.dist-info/RECORD
+11 files, 38718 bytes uncompressed, 10426 bytes compressed:  73.1%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: osw_confidence_metric/utils.py
 Comment: 
 
 Filename: osw_confidence_metric/version.py
 Comment: 
 
-Filename: osw_confidence_metric-0.0.3.dist-info/LICENSE
+Filename: osw_confidence_metric-0.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: osw_confidence_metric-0.0.3.dist-info/METADATA
+Filename: osw_confidence_metric-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: osw_confidence_metric-0.0.3.dist-info/WHEEL
+Filename: osw_confidence_metric-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: osw_confidence_metric-0.0.3.dist-info/top_level.txt
+Filename: osw_confidence_metric-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: osw_confidence_metric-0.0.3.dist-info/RECORD
+Filename: osw_confidence_metric-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## osw_confidence_metric/area_analyzer.py

```diff
@@ -1,9 +1,10 @@
 # area_analyzer.py file
-
+import warnings
+warnings.simplefilter(action='ignore', category=FutureWarning)
 import osmnx as ox
 import pandas as pd
 import dask_geopandas
 import geopandas as gpd
 import geonetworkx as gnx
 from datetime import datetime
 from shapely.ops import voronoi_diagram
```

## osw_confidence_metric/version.py

```diff
@@ -1 +1 @@
-__version__ = '0.0.3'
+__version__ = '0.0.4'
```

## Comparing `osw_confidence_metric-0.0.3.dist-info/LICENSE` & `osw_confidence_metric-0.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `osw_confidence_metric-0.0.3.dist-info/METADATA` & `osw_confidence_metric-0.0.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: osw-confidence-metric
-Version: 0.0.3
+Version: 0.0.4
 Summary: Calculates the confidence score of a given geojson area
 Home-page: https://github.com/TaskarCenterAtUW/TDEI-python-lib-confidence-metric
 Author: Sujata Misra
 Author-email: sujatam@gaussiansolutions.com
 Project-URL: Documentation, https://github.com/TaskarCenterAtUW/TDEI-python-lib-confidence-metric/blob/main/README.md
 Project-URL: GitHub, https://github.com/TaskarCenterAtUW/TDEI-python-lib-confidence-metric
 Project-URL: Changelog, https://github.com/TaskarCenterAtUW/TDEI-python-lib-confidence-metric/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: osmapi ==4.0.0
-Requires-Dist: geopandas ==0.14.1
+Requires-Dist: geopandas ==0.14.3
 Requires-Dist: osmnx ==1.8.0
 Requires-Dist: dask-geopandas ==0.3.1
 Requires-Dist: geonetworkx ==0.5.3
 Requires-Dist: shapely ==2.0.2
 Requires-Dist: coverage ==7.2.7
 
 # TDEI-python-confidence-metric-lib
```

## Comparing `osw_confidence_metric-0.0.3.dist-info/RECORD` & `osw_confidence_metric-0.0.4.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 osw_confidence_metric/__init__.py,sha256=8zLGg-DfQhnDl2Ky0n-zXpN-8e-g7iR0AcaI4l4Vvpk,32
-osw_confidence_metric/area_analyzer.py,sha256=gK7g_oXu3VRLytBFDu1RxViCqCg80tbUrs_o42ieNnA,4627
+osw_confidence_metric/area_analyzer.py,sha256=6JfWbhmyAwQfy9tFHG7QpLsd7cX1qr-jjWqLSvIw8Dw,4705
 osw_confidence_metric/osm_data_handler.py,sha256=4m09avQHBPZpwmrQjd9DKp9Lj-N0QcQ62SnykCB-Qhg,964
 osw_confidence_metric/trust_score_calculator.py,sha256=mAlJUie9TBxdPY_kEtPTOoFTvCUHEC1Kg-ZQVlKn-e0,8192
 osw_confidence_metric/utils.py,sha256=hnnBNAGZCK7bv6rAEntFj3eP6HnRjqY3MavVQyhl1NQ,12040
-osw_confidence_metric/version.py,sha256=kQOJvtmpbHGE0oVJv6oubUfigE6lAOQFBGPyh3SkWZI,21
-osw_confidence_metric-0.0.3.dist-info/LICENSE,sha256=KXSpN2qzyPU7LuuGtJrQH4JsLkKmn077inwH99InLGw,1073
-osw_confidence_metric-0.0.3.dist-info/METADATA,sha256=puP9fJXYyNSm8tDDorfTex9GbKHKgYasYNUraREpx9o,10561
-osw_confidence_metric-0.0.3.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-osw_confidence_metric-0.0.3.dist-info/top_level.txt,sha256=Wd15KBVKmX49xc5WCCnrqkVodEBX9sn5zFPfglyc8mE,22
-osw_confidence_metric-0.0.3.dist-info/RECORD,,
+osw_confidence_metric/version.py,sha256=Qkdiz6Ybn1PE1SlWhKAQBmETf7pQ0yr5HmkqLVDxsqE,21
+osw_confidence_metric-0.0.4.dist-info/LICENSE,sha256=KXSpN2qzyPU7LuuGtJrQH4JsLkKmn077inwH99InLGw,1073
+osw_confidence_metric-0.0.4.dist-info/METADATA,sha256=3-_QdvNRXpk0uoqUfQuEzyAb16l3kub42bU7ylFfQ_k,10561
+osw_confidence_metric-0.0.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+osw_confidence_metric-0.0.4.dist-info/top_level.txt,sha256=Wd15KBVKmX49xc5WCCnrqkVodEBX9sn5zFPfglyc8mE,22
+osw_confidence_metric-0.0.4.dist-info/RECORD,,
```

