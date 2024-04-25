# Comparing `tmp/centerline-width-1.5.0.tar.gz` & `tmp/centerline-width-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "centerline-width-1.5.0.tar", last modified: Sat Feb 24 21:46:08 2024, max compression
+gzip compressed data, was "centerline-width-1.6.0.tar", last modified: Thu Apr 25 03:20:00 2024, max compression
```

## Comparing `centerline-width-1.5.0.tar` & `centerline-width-1.6.0.tar`

### file list

```diff
@@ -1,30 +1,38 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-24 21:46:08.266257 centerline-width-1.5.0/
--rw-rw-r--   0 user      (1000) user      (1000)     1072 2024-01-24 02:23:54.000000 centerline-width-1.5.0/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)    54400 2024-02-24 21:46:08.266257 centerline-width-1.5.0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    52656 2024-02-24 07:57:22.000000 centerline-width-1.5.0/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-24 21:46:08.262257 centerline-width-1.5.0/centerline_width/
--rw-rw-r--   0 user      (1000) user      (1000)     1981 2024-02-20 22:14:45.000000 centerline-width-1.5.0/centerline_width/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    27826 2024-01-24 02:23:54.000000 centerline-width-1.5.0/centerline_width/centerline.py
--rw-rw-r--   0 user      (1000) user      (1000)    18755 2024-02-24 07:49:17.000000 centerline-width-1.5.0/centerline_width/error_handling.py
--rw-rw-r--   0 user      (1000) user      (1000)     1854 2024-01-24 02:23:54.000000 centerline-width-1.5.0/centerline_width/getCoordinatesKML.py
--rw-rw-r--   0 user      (1000) user      (1000)    13895 2024-02-24 07:48:47.000000 centerline-width-1.5.0/centerline_width/plotDiagrams.py
--rw-rw-r--   0 user      (1000) user      (1000)     7153 2024-02-24 07:20:05.000000 centerline-width-1.5.0/centerline_width/preprocessing.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-24 21:46:08.266257 centerline-width-1.5.0/centerline_width/pytests/
--rw-rw-r--   0 user      (1000) user      (1000)     5352 2024-01-24 02:23:54.000000 centerline-width-1.5.0/centerline_width/pytests/test_centerline.py
--rw-rw-r--   0 user      (1000) user      (1000)     3237 2024-01-24 02:23:54.000000 centerline-width-1.5.0/centerline_width/pytests/test_getCoordinatesKML.py
--rw-rw-r--   0 user      (1000) user      (1000)    13706 2024-02-24 07:51:58.000000 centerline-width-1.5.0/centerline_width/pytests/test_plotDiagrams.py
--rw-rw-r--   0 user      (1000) user      (1000)     1838 2024-01-24 02:23:54.000000 centerline-width-1.5.0/centerline_width/pytests/test_preprocessing.py
--rw-rw-r--   0 user      (1000) user      (1000)     3736 2024-01-24 02:23:54.000000 centerline-width-1.5.0/centerline_width/pytests/test_riverCenterlineClass.py
--rw-rw-r--   0 user      (1000) user      (1000)     8412 2024-01-24 02:23:54.000000 centerline-width-1.5.0/centerline_width/pytests/test_saveOutput.py
--rw-rw-r--   0 user      (1000) user      (1000)     4720 2024-01-24 02:23:54.000000 centerline-width-1.5.0/centerline_width/pytests/test_verifyOutput.py
--rw-rw-r--   0 user      (1000) user      (1000)     3516 2024-01-24 02:23:54.000000 centerline-width-1.5.0/centerline_width/relativeDistance.py
--rw-rw-r--   0 user      (1000) user      (1000)    10046 2024-02-24 07:48:33.000000 centerline-width-1.5.0/centerline_width/riverCenterlineClass.py
--rw-rw-r--   0 user      (1000) user      (1000)     5928 2024-01-24 02:23:54.000000 centerline-width-1.5.0/centerline_width/saveOutput.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-24 21:46:08.266257 centerline-width-1.5.0/centerline_width.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)    54400 2024-02-24 21:46:08.000000 centerline-width-1.5.0/centerline_width.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      866 2024-02-24 21:46:08.000000 centerline-width-1.5.0/centerline_width.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-02-24 21:46:08.000000 centerline-width-1.5.0/centerline_width.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      160 2024-02-24 21:46:08.000000 centerline-width-1.5.0/centerline_width.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       17 2024-02-24 21:46:08.000000 centerline-width-1.5.0/centerline_width.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2024-02-24 21:46:08.266257 centerline-width-1.5.0/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2005 2024-02-24 20:47:56.000000 centerline-width-1.5.0/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-25 03:20:00.310359 centerline-width-1.6.0/
+-rw-rw-r--   0 user      (1000) user      (1000)     1072 2024-01-24 02:23:54.000000 centerline-width-1.6.0/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)    60635 2024-04-25 03:20:00.306359 centerline-width-1.6.0/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    58970 2024-04-16 22:25:45.000000 centerline-width-1.6.0/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-25 03:20:00.298359 centerline-width-1.6.0/centerline_width/
+-rw-rw-r--   0 user      (1000) user      (1000)     2122 2024-04-12 04:18:48.000000 centerline-width-1.6.0/centerline_width/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12498 2024-04-12 05:34:16.000000 centerline-width-1.6.0/centerline_width/centerline.py
+-rw-rw-r--   0 user      (1000) user      (1000)    23402 2024-04-13 17:54:41.000000 centerline-width-1.6.0/centerline_width/error_handling.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2108 2024-04-06 01:57:11.000000 centerline-width-1.6.0/centerline_width/getCoordinatesKML.py
+-rw-rw-r--   0 user      (1000) user      (1000)    17981 2024-04-16 05:39:51.000000 centerline-width-1.6.0/centerline_width/plotDiagrams.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8504 2024-04-13 17:52:28.000000 centerline-width-1.6.0/centerline_width/preprocessing.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-25 03:20:00.306359 centerline-width-1.6.0/centerline_width/pytests/
+-rw-rw-r--   0 user      (1000) user      (1000)     4253 2024-03-23 07:29:19.000000 centerline-width-1.6.0/centerline_width/pytests/test_errorGetCoordinatesKML.py
+-rw-rw-r--   0 user      (1000) user      (1000)    18479 2024-03-30 07:09:41.000000 centerline-width-1.6.0/centerline_width/pytests/test_errorPlotDiagrams.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2299 2024-04-13 18:14:24.000000 centerline-width-1.6.0/centerline_width/pytests/test_errorPreprocessing.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6390 2024-03-24 01:47:45.000000 centerline-width-1.6.0/centerline_width/pytests/test_errorRiverCenterlineClass.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12625 2024-03-26 06:29:01.000000 centerline-width-1.6.0/centerline_width/pytests/test_errorSaveOutput.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8300 2024-03-26 06:47:33.000000 centerline-width-1.6.0/centerline_width/pytests/test_errorWidth.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8895 2024-04-05 08:11:25.000000 centerline-width-1.6.0/centerline_width/pytests/test_verifyGetCoordinatesKML.py
+-rw-rw-r--   0 user      (1000) user      (1000)    48370 2024-04-06 02:13:03.000000 centerline-width-1.6.0/centerline_width/pytests/test_verifyPlotDiagrams.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3506 2024-04-13 17:58:42.000000 centerline-width-1.6.0/centerline_width/pytests/test_verifyPreprocessing.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4467 2024-03-25 00:40:26.000000 centerline-width-1.6.0/centerline_width/pytests/test_verifyRiverFeatures.py
+-rw-rw-r--   0 user      (1000) user      (1000)    40957 2024-03-26 06:22:51.000000 centerline-width-1.6.0/centerline_width/pytests/test_verifySaveOutput.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3439 2024-04-19 02:23:09.000000 centerline-width-1.6.0/centerline_width/pytests/test_verifyWidth.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4611 2024-04-06 02:40:53.000000 centerline-width-1.6.0/centerline_width/relativeDistance.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6163 2024-04-16 22:25:51.000000 centerline-width-1.6.0/centerline_width/riverAsymmetry.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12455 2024-04-06 03:19:55.000000 centerline-width-1.6.0/centerline_width/riverCenterlineClass.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1125 2024-04-07 21:27:25.000000 centerline-width-1.6.0/centerline_width/riverFeatures.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7033 2024-04-06 02:40:51.000000 centerline-width-1.6.0/centerline_width/saveOutput.py
+-rw-rw-r--   0 user      (1000) user      (1000)    23405 2024-04-12 02:56:27.000000 centerline-width-1.6.0/centerline_width/width.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-25 03:20:00.306359 centerline-width-1.6.0/centerline_width.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)    60635 2024-04-25 03:20:00.000000 centerline-width-1.6.0/centerline_width.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1250 2024-04-25 03:20:00.000000 centerline-width-1.6.0/centerline_width.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-25 03:20:00.000000 centerline-width-1.6.0/centerline_width.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       83 2024-04-25 03:20:00.000000 centerline-width-1.6.0/centerline_width.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       17 2024-04-25 03:20:00.000000 centerline-width-1.6.0/centerline_width.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2024-04-25 03:20:00.310359 centerline-width-1.6.0/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2091 2024-04-19 02:24:53.000000 centerline-width-1.6.0/setup.py
```

### Comparing `centerline-width-1.5.0/LICENSE` & `centerline-width-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `centerline-width-1.5.0/PKG-INFO` & `centerline-width-1.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,56 +1,59 @@
 Metadata-Version: 2.1
 Name: centerline-width
-Version: 1.5.0
+Version: 1.6.0
 Summary: A Python package to find the centerline and width of rivers based on the latitude and longitude of the right and left bank
 Home-page: https://github.com/cyschneck/centerline-width
-Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v1.5.0.tar.gz
+Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v1.6.0.tar.gz
 Author: Una Schneck (unaschneck), Cora Schneck (cyschneck)
 License: MIT
 Keywords: geophysics,python,voronoi,networkx,centerline,centerline-extraction,centerline-detection,rivers,river-bank-length,river-bank,limnology,hydrology,fluvial,geomorphology
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: geopy>=2.3.0
-Requires-Dist: haversine>=2.8.0
-Requires-Dist: matplotlib>=3.1.0
-Requires-Dist: networkx>=3.0
-Requires-Dist: numpy>=1.24.1
-Requires-Dist: pandas>=1.3.5
-Requires-Dist: pykml>=0.2.0
-Requires-Dist: pyproj>=3.4.1
-Requires-Dist: pytest>=7.2.2
-Requires-Dist: scipy>=1.10.1
-Requires-Dist: shapely>=2.0.1
+Requires-Dist: geopy
+Requires-Dist: haversine
+Requires-Dist: matplotlib
+Requires-Dist: networkx
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: pykml
+Requires-Dist: pyproj
+Requires-Dist: pytest
+Requires-Dist: scipy
+Requires-Dist: shapely
 
 # Centerline-Width
  <p align="center">
   <img src="https://raw.githubusercontent.com/cyschneck/centerline-width/main/assets/centerline_logo.jpg" />
 </p>
 
 ![PyPi](https://img.shields.io/pypi/v/centerline-width)
 ![license](https://img.shields.io/github/license/cyschneck/centerline-width)
+[![repo-status](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 [![NSF-2141064](https://img.shields.io/badge/NSF-2141064-blue)](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2141064&HistoricalAwards=false)
 ![PyPi-Versions](https://img.shields.io/pypi/pyversions/centerline-width)
 [![pytests](https://github.com/cyschneck/centerline-width/actions/workflows/pytests.yml/badge.svg)](https://github.com/cyschneck/centerline-width/actions/workflows/pytests.yml)
+[![pre-commit](https://github.com/cyschneck/centerline-width/actions/workflows/pre-commit.yml/badge.svg)](https://github.com/cyschneck/centerline-width/actions/workflows/pre-commit.yml)
+[![codecov](https://codecov.io/gh/cyschneck/centerline-width/graph/badge.svg?token=V6Z2DC37MT)](https://codecov.io/gh/cyschneck/centerline-width)
 
 Find the centerline and width of rivers based on the latitude and longitude positions from the right and left bank 
 
 * **Convert raw data from Google Earth Pro to CSV**
 	* extractPointsToTextFile()
 	* convertColumnsToCSV()
 * **Find centerline and width of river**
@@ -58,16 +61,18 @@
 	* plotCenterlineWidth()
 	* riverWidthFromCenterline()
 	* centerlineVoronoi
 	* centerlineEqualDistance 
 	* centerlineEvenlySpaced
 	* centerlineSmoothed
 	* centerlineLength
+* **Return river features**
 	* rightBankLength
 	* leftBankLength
+	* riverArea
 * **Export centerline to .CSV and .MAT files**
 	* saveCenterlineCSV()
 	* saveCenterlineMAT()
 
 | River Outlined in Google Earth Pro | Generated Centerline for the Riverbank |
 | ------------- | ------------- |
 | ![river_google_earth+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_example_google_earth.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_example.png) |
@@ -172,26 +177,26 @@
 ```
 
 ### Converted Text File to CSV
 
 Convert a text file with coordinates for a left and right bank's latitude and longitude to a csv file with columns for the left bank latitude (llat), left bank longitude (llon), right bank latitude (rlat), right bank longitude (rlon)
 
 ```
-convertColumnsToCSV(text_file=None, flipBankDirection=False)
+convertColumnsToCSV(text_file=None, flip_direction=False)
 ```
 * **[REQUIRED]** text_file (string): File location of the text file to convert
-* [OPTIONAL] flipBankDirection (boolean): If the latitude/longitude of the banks are generated in reverse order, flip the final values so left/right bank are in order
+* [OPTIONAL] flip_direction (boolean): If the latitude/longitude of the banks are generated in reverse order, flip the final values so left/right bank are in order
 
 Scripts expects data as a list of point for left and right banks:
 - Header: llat, llon, rlat, rlon
 
 ```python
 import centerline_width
 centerline_width.convertColumnsToCSV(text_file="data/river_coords.txt",
-				flipBankDirection=True)
+				flip_direction=True)
 ```
 Converts text file:
 ```
      llat       llon      rlat       rlon
 30.037581 -92.868569 30.037441 -92.867476
 30.037613 -92.868549 30.037448 -92.867474
 30.037648 -92.868546 30.037482 -92.867449
@@ -223,15 +228,15 @@
 ```
 * **[REQUIRED]** csv_data (string): File location of the text file to convert
 * [OPTIONAL] optional_cutoff (int): Include only the first x number of the data to chart (useful for debugging)
 * [OPTIONAL] interpolate_data (boolean): Interpolate between existing data by adding additional points
 * [OPTIONAL] interpolate_n (int): Number of additional points to add between existing data, defaults to 5 (note: larger numbers will take exponentially longer to run, recommends less than 15)
 * [OPTIONAL] interpolate_n_centerpoints (int): Number of points used to interpolate the Voronoi centerline, defaults to the the length of the data frame (df_len)
 * [OPTIONAL] equal_distance (int): Equal distance between points (in meters) used to interpolate the Voronoi centerline, defaults 10 meters
-* [OPTIONAL] ellipsoid (string): Ellipsoid definition of Earth to provide size and shape for built-in functions to convert degrees to meters, options include (is sensitive to case): ["GRS80", "airy", "bessel", "clrk66", "intl", "WGS60", "WGS66", "WGS72", "WGS84", "sphere"] for more details: ["Built-in ellipsoid defintions"](https://proj.org/en/9.2/usage/ellipsoids.html#built-in-ellipsoid-definitions), defaults to "WGS84"
+* [OPTIONAL] ellipsoid (string): Ellipsoid definition of Earth to provide size and shape for built-in functions to convert degrees to meters, options include (is sensitive to case): ["GRS80", "airy", "bessel", "clrk66", "intl", "WGS60", "WGS66", "WGS72", "WGS84", "sphere"] for more details: ["Built-in ellipsoid definitions"](https://proj.org/en/9.2/usage/ellipsoids.html#built-in-ellipsoid-definitions), defaults to "WGS84"
 
 **Equal Distance - Equal linear distance between points**
 
 `equal_distance` will generate points along the centerline that are an equal linear distance from one another in meters. When `equal_distance=5` each point will be 5 meters apart
 
 | equal_distance=5 | equal_distance=20 |
 | ------------- | ------------- |
@@ -254,14 +259,15 @@
 * centerlineVoronoi (list of tuples): List of the latitude and longitude coordinates of the centerline generated by Voronoi diagrams
 * centerlineEqualDistance (list of tuples): List of the latitude and longitude coordinates of the centerline generated by equal distances between coordinates from the Voronoi diagrams
 * centerlineEvenlySpaced (list of tuples): List of the latitude and longitude coordinates of the centerline generated by evenly spacing out points generated by the Voronoi diagrams
 * centerlineSmoothed (list of tuples): List of the latitude and longitude coordinates of the centerline generated by smoothing out the evenly spaced-out points generated by the Voronoi diagrams
 * centerlineLength (float): Length of the centerline of the river (in km)
 * rightBankLength (float): Length of the right bank of the river (in km)
 * leftBankLength (float): Length of the left bank of the river (in km)
+* riverArea (float): Area contained within river bank polygon (in km^2)
 * centerlineVoronoiRelative (list of tuples): List of the relative distance coordinates of the centerline generated by Voronoi diagrams
 * centerlineEqualDistanceRelative (list of tuples): List of the relative distance coordinates of the centerline generated by equal distances between coordinates from the Voronoi diagrams
 * centerlineEvenlySpacedRelative (list of tuples): List of the relative distance coordinates of the centerline generated by evenly spacing out points generated by the Voronoi diagrams
 * centerlineSmoothedRelative (list of tuples): List of the relative distance coordinates of the centerline generated by smoothing out the evenly spaced out points generated by the Voronoi diagrams
 
 **Object (class) additional attributes:**
 
@@ -407,14 +413,27 @@
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
 river_centerline_length = river_object.centerlineLength
 ```
 The length of the river centerline returns `215.34700589636674` km
 
+### Area of River
+Return the area contained within the polygon generated the left and right bank latitude/longitudes
+```
+river_object.riverArea
+```
+Area returned in kilometers^2
+```python
+import centerline_width
+river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
+river_area = river_object.riverArea
+```
+The area of the river returns `334.0398585246558` km^2
+
 ## Plot Centerline in Matplotlib
 Plot the centerline created from a list of right and left banks
 
 ```
 plotCenterline(centerline_type="Voronoi",
 		marker_type="line",
 		centerline_color="black",
@@ -429,28 +448,93 @@
 ```
 * [OPTIONAL] centerline_type (string): Centerline type graph within river (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
 * [OPTIONAL] marker_type (string): Graph type (not case-sensitive), options: ["Line", "Scatter"], defaults to "Line"
 * [OPTIONAL] centerline_color (string): Color of centerline coordinates on graph (not case-sensitive), options: [matplotlib named colors](https://matplotlib.org/stable/gallery/color/named_colors.html), defaults to "black"
 * [OPTIONAL] dark_mode (bool): Change plot to a black ground (and override if `centerline_color="black"` to `centerline_color="white"`), defaults to False
 * [OPTIONAL] equal_axis (bool): Set x/y axes in plot to be equal, defaults to False
 * [OPTIONAL] display_all_possible_paths (boolean): Display all possible paths, not just the centerline (useful for debugging), defaults to False
-* [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False"
+* [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False, Interpolated = True/False"
 * [OPTIONAL] save_plot_name (string): Save the plot with a given name and location
 * [OPTIONAL] display_voronoi (boolean): Overlay Voronoi diagram used to generate centerline, defaults to False
 * [OPTIONAL] show_plot (boolean): display and open plots (plt.show() in Matplotlib), defaults to True
 * [OPTIONAL] coordinate_unit (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longitude) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degrees"
 
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
 river_object.plotCenterline()
 ```
-Output:
 ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_centerline.png)
 
+**centerline_type**
+
+Display different centerline types in plot ("Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"), but defaults to "Voronoi"
+
+| centerline_type="Voronoi" | centerline_type="Smoothed" |
+| ------------- | ------------- |
+| ![centerline_type_voronoi+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_centerline.png) | ![centerline_type_equal_distance+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_centerline_type_smoothed.png) |
+
+**marker_type**
+
+Display centerline plot as either line or scatter
+
+| marker_type="Line" | marker_type="Scatter" |
+| ------------- | ------------- |
+| ![marker_type_line+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_centerline.png)  | ![marker_type_scatter+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_marker_type_scatter.png) |
+
+**centerline_color**
+
+Change the color of the centerline, defaults to black
+
+| centerline_color="black" | centerline_color="palegreen" |
+| ------------- | ------------- |
+| ![centerline_color_black+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_centerline.png) | ![centerline_color_purple+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_centerline_color.png) |
+
+**dark_mode**
+
+dark_mode will change the default Matplotlib background black and swap `centerline_color` from default black to white
+
+| dark_mode=False | dark_mode=True |
+| ------------- | ------------- |
+| ![dark_mode_false+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_centerline.png) | ![dark_mode_true+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_dark_mode.png) |
+
+**equal_axis**
+
+equal_axis will set the x and y axis of the plot to be equal
+
+| equal_axis=False | equal_axis=True |
+| ------------- | ------------- |
+| ![river_not_equal+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_equal_axis_false.png) | ![river_equal+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_equal_axis_true.png)|
+
+**display_all_possible_paths**
+
+Display all possible paths generated by Voronoi edge ridges, defaults to False
+
+| display_all_possible_paths=False | display_all_possible_paths=True |
+| ------------- | ------------- |
+| ![display_all_possible_paths_false+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_centerline.png) | ![display_all_possible_paths_true+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_display_all_possible_paths_true.png) |
+
+**display_voronoi**
+
+Overlay Voronoi diagram used to generate centerline, defaults to False
+
+| display_voronoi=False | display_voronoi=True |
+| ------------- | ------------- |
+| ![display_voronoi_default+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_display_voronoi_false.png) | ![display_voronoi_true+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_display_voronoi_true.png) |
+
+
+**coordinate_unit**
+
+Plot as either "Decimal Degrees" and "Relative Distance". defaults to "Decimal Degrees" 
+
+| coordinate_unit="Decimal Degrees" | coordinate_unit="Relative Distance" |
+| ------------- | ------------- |
+| ![coordinate_unit_dd+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_centerline.png) | ![coordinate_unit_rd+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coordinate_unit_rd.png) |
+
+
 ## Plot Centerline Width Lines in Matplotlib
 ### Plot the Centerline Width Lines
 Plot the width of the river based on the centerline
 
 ```
 plotCenterlineWidth(plot_title=None, 
 		save_plot_name=None, 
@@ -461,27 +545,35 @@
 		flag_intersections=True,
 		remove_intersections=False,
 		dark_mode=False,
 		equal_axis=False,
 		show_plot=True,
 		coordinate_unit="Decimal Degrees")
 ```
-* [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False"
+* [OPTIONAL] plot_title (string): Change plot title, defaults to "River Width Coordinates: Valid Centerline = True/False, Valid Polygon = True/False, Centerline made of <interpolate_n_centerpoints> Fixed Points, width lines generated every <transect_span_distance> points, Interpolated = True/False"
 * [OPTIONAL] save_plot_name (string): Save the plot with a given name and location
 * [OPTIONAL] display_true_centerline (boolean): Display generated true centerline based on Voronoi diagrams, defaults to True
 * [OPTIONAL] transect_span_distance (int): Number n points around a center point to determine the slope (increase to decrease the impact of sudden changes), defaults to 3, must be greater than 1 (since the slope is found from the difference in position between two points)
 * [OPTIONAL] transect_slope (str): Determine how the width lines are generated, either by averaging all slopes "Average" or directly from the first to last point in the span distance as "Direct", defaults to "Average"
 * [OPTIONAL] apply_smoothing (boolean): Apply a B-spline smoothing to centerline
 * [OPTIONAL] flag_intersections (boolean): Display intersecting width lines as red in graph, defaults to True
 * [OPTIONAL] remove_intersections (boolean): Remove intersecting lines (but maintain the most width lines as possible) and only return non-intersecting width lines, defaults to False
 * [OPTIONAL] dark_mode (bool): Change plot to a black ground (and override if `centerline_color="black"` to `centerline_color="white"`), defaults to False
 * [OPTIONAL] equal_axis (bool): Set x/y axes in plot to be equal, defaults to False
 * [OPTIONAL] show_plot (boolean): display and open plots (plt.show() in Matplotlib), defaults to True
 * [OPTIONAL] coordinate_unit (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longitude) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degrees"
 
+
+```python
+import centerline_width
+river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
+river_object.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
+```
+![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width.png)
+
 **display_true_centerline**
 
 The width lines are generated from the evenly spaced coordinate (by default) or with the smoothed coordinates (when `apply_smoothing=True`), but display_true_centerline will overlay the Voronoi centerline on top of the plot
 
 | display_true_centerline=True | display_true_centerline=False |
 | ------------- | ------------- |
 | ![river_with_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_with_centerline.png) | ![river_no_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_without_centerline.png) |
@@ -527,15 +619,15 @@
 
 | remove_intersections=False | remove_intersections=True |
 | ------------- | ------------- |
 | ![river_keep+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_keep_intersections.png) | ![river_remove+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_remove_intersections.png)|
 
 **dark_mode**
 
-dark_mode will change the default Matplotlib background black and swap `centerline_color` from black to white
+dark_mode will change the default Matplotlib background black and swap `centerline_color` from default black to white
 
 | dark_mode=False | dark_mode=True |
 | ------------- | ------------- |
 | ![river_white+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_dark_mode_false.png) | ![river_black+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_dark_mode_true.png)|
 
 **equal_axis**
 
@@ -545,25 +637,18 @@
 | ------------- | ------------- |
 | ![river_not_equal+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_not_equal_default_ax.png) | ![river_equal+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_equal_ax.png)|
 
 **coordinate_unit**
 
 Two options for measuring and displaying coordinates. The two options are "Decimal Degrees" and "Relative Distance". "Decimal Degrees" is the default option that uses the original data coordinate system with latitude/longitude. "Relative Distance" changes the coordinates of each point to be the distance (in meters) from the first point on the left bank
 
-| coordinate_unit="Decimal Degrees" | remove_intersections="Relative Distance" |
+| coordinate_unit="Decimal Degrees" | coordinate_unit="Relative Distance" |
 | ------------- | ------------- |
 | ![dd_coords+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_decimal_degrees.png) | ![rd_coords+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_relative_distance.png)|
 
-```python
-import centerline_width
-river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
-river_object.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
-```
-![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width.png)
-
 ### Return Width of River
 Return the width of the river at each (evenly spaced or smoothed) with coordinates where width line intersects either the centerline, `(Centerline Longitude, Centerline Latitude) : width`, or riverbanks, `((Right Bank Longitude, Right Bank Latitude), (Left Bank Longitude, Left Bank Latitude)) : width` in kilometers
 
 ```
 riverWidthFromCenterline(transect_span_distance=3,
 			transect_slope="Average",
 			apply_smoothing=True,
@@ -595,137 +680,162 @@
 Note: it is best practice to plot the centerline and width with same arguments in `plotCenterlineWidth()` to ensure that the results when `save_to_csv=True` are as expected
 
 ## Documentation and Algorithm to Determine Centerline
 
 The centerline is defined by the greatest distance from the right and left bank, created from a Voronoi Diagram. The remaining paths within the river are filtered through Dijkstra's algorithm to find the shortest path that is the centerline
 
 ### Right and Left bank points are plotted (X-Axis for Latitude, Y-Axis for Longitude)
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example1.png)
+![algorithm_step1+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/algorithm_step1.png)
 
 ### Generate a polygon to encapsulate the river between the right and left banks to define in and outside of river
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example2.png)
+![algorithm_step2+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/algorithm_step2.png)
 
 ### Generate a Voronoi diagram based on the points along the riverbanks
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example3.png)
+![algorithm_step3+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/algorithm_step3.png)
 
 ### Display Voronoi ridge vertices that lie within the polygon (within the riverbanks)
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example4.png)
+Filter out any point pairs that only have one connection to filter out the short dead end paths
 
-### Filter out any point pairs that only have one connection to filter out the short dead end paths
 With the vertices removed, it is possible to form multiple unconnected graphs within the polygon. The largest subgraph is assumed to contain the centerline and the other subgraphs are filtered out
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example6.png)
+![algorithm_step4+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/algorithm_step4.png)
+
+### Define Top and Bottom of Polygon
+The top of the river is defined as the last plotted points in the data, while the bottom of the river is the first plotted points
+![algorithm_step5+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/algorithm_step5.png)
 
 ### Find the starting and ending node based on distance from the top and bottom of polygon
 The starting/ending node is defined by the vertex closest to the top/bottom of the polygon along the longest path
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example7.png)
+![algorithm_step6+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/algorithm_step6.png)
 
 ### Find the shortest path from the starting node to the ending node ([Dijkstra's Algorithm](https://networkx.org/documentation/stable/reference/algorithms/generated/networkx.algorithms.shortest_paths.generic.shortest_path.html#networkx.algorithms.shortest_paths.generic.shortest_path))
 | Points on Riverbank | NetworkX Graph of Points on Riverbank |
 | ------------- | ------------- |
-| ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example10.png) | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example9.png) |
+| ![algorithm_step7+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/algorithm_step7.png) | ![algorithm_step8+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/algorithm_step8.png) |
 
 ### Display the centerline found by connecting the starting/ending node with the shortest path
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example8.png)
+![algorithm_step9+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/algorithm_step9.png)
 
 This is an attempt at a more robust algorithm working from raw data to ensure that all dead ends are removed, and no gaps exist in the centerline
 
 Points that only have one connection are removed, but limiting the number of connections for a point to just two will create gaps. The Voronoi vertices connect to other vertex values, but some connect to more and some only connect to one other point. Removing additional values will create gaps, so this is avoided in this code by not applying additional filters.
 
 **All vertices:**
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example4.png)
+![algorithm_step4+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/algorithm_step4.png)
 
 **Vertices that have at least two connections (that would create gaps):**
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example5.png)
+![algorithm_step10+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/algorithm_step10.png)
 
 ## Debugging, Error Handling, and Edge Cases
 ### Wide Start/End of River
 If the data starts or ends with a large width, it is possible for the starting/ending nodes to end up in the wrong position
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_example3.png)
+![invalid_too_wide+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_too_wide.png)
 Currently, the starting node is determined by the closest node on the path to the top of the bank (in green) and the ending node is determined by the closest node on the path to the bottom of the bank (in red) that sits along the longest path
 
 ### Invalid Polygon
 A polygon is formed to encapsulate the river with the given data (to determine the inside and outside of the river). The top and bottom are connected by a straight line from the start/end of the available data. As a result, it is possible for this straight line to overlap and create an invalid polygon.
 
 A polygon is invalid if it overlaps within itself:
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_example1.png)
+![invalid_minor_polygon+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_minor_polygon.png)
 In this example, the polygon is invalid, but with such a small overlap it is still able to find a valid path
 
 With limited data, the polygon will overlap more dramatically and will struggle to find a valid centerline:
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_example4.png)
+![invalid_major_polygon+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_major_polygon.png)
 
 ### Invalid Centerline
-If the data is too small, a centerline and its coordinates cannot not be found (since only a single Voronoi vertex exists within the polygon and after dead ends are filtered)
+If the data is too small, a centerline and its coordinates cannot be found (since only a single Voronoi vertex exists within the polygon and after dead ends are filtered)
 
-`CRITICAL ERROR, Polygon too short for the Voronoi diagram generated (no starting node found), unable to plot centerline. Set displayVoronoi=True to view vertices. Can typically be fixed by adding more data to expand range.`
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_example2.png)
+`CRITICAL ERROR, Polygon too short for the Voronoi diagram generated (no starting node found), unable to plot centerline. Set display_voronoi=True to view vertices. Can typically be fixed by adding more data to expand range`
+![invalid_too_small+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_too_small.png)
 Can be fixed by expanding the data until the polygon is large enough to contain at least two different vertex points
 
-### Invalid Top and Bottom Bank Positions (flipBankDirection = True)
-Error: `WARNING: Invalid Polygon Due to Flipped Banks, fix recommendation: rerun convertColumnsToCSV() and set flipBankDirection=True (or reset to default 'False' if currently set to flipBankDirection=True)`
+### Invalid Top and Bottom Bank Positions (flip_direction = True)
+Error: `WARNING: Invalid Polygon Due to Flipped Banks, fix recommendation: rerun convertColumnsToCSV() and set flip_direction=True (or reset to default 'False' if currently set to flip_direction=True)`
 
 If the data for the left and right riverbanks are generated in reverse order, they will be read in the incorrect order and the graph will find the invalid top and bottom of the bank
 
 If the latitude/longitude of the banks are generated in reverse order, flip the final values so left/right bank are in order
 
-This can be fixed by using the flipBankDirection optional argument `centerline_width.convertColumnsToCSV(text_file="data_example.txt", flipBankDirection=True)`
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/flipDirection_example.png)
+This can be fixed by using the flip_direction optional argument `centerline_width.convertColumnsToCSV(text_file="data_example.txt", flip_direction=True)`
+![invalid_flipped_banks+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_flipped_banks.png)
 
 ### Invalid Smoothed Centerline
 The smoothed centerline (`river_object.centerlineSmoothed`) can end up lying outside the river if the centerline data points are sparse in a narrow river. If more than two points in the smoothed centerline lie outside the river, a warning will be thrown
 
 Example Error: `WARNING: Partially invalid smoothed centerline due to sparse centerline data (6 points lie outside the polygon), fix recommendation: rerun riverCenterline to create river object with interpolate_n_centerpoints set to 62+`
 
-By default, `interpolate_n_centerpoints` is set to None and not additional points will be added between the existing points along the centerline. By adding additional points between the existing centerline, the smoothed centerline can be fixed to stay within the polygon. This fix is set by creating a river object, `centerline_width.riverCenterline`, with `interpolate_n_centerpoints=65` (with the recommended 62+) to fix for centerline coordinates that lie outside the polygon
+By default, `interpolate_n_centerpoints` is set to None and no additional points will be added between the existing points along the centerline. By adding additional points between the existing centerline, the smoothed centerline can be fixed to stay within the polygon. This fix is set by creating a river object, `centerline_width.riverCenterline`, with `interpolate_n_centerpoints=65` (with the recommended 62+) to fix for centerline coordinates that lie outside the polygon
 
 `interpolate_n_centerpoints = None` does not interpolate data points, so the size will be set to the number of fixed points when creating the evenly spaced coordinates (equal to the size of the data frame)
 
 | interpolate_n_centerpoints = None | interpolate_n_centerpoints = 65 |
 | ------------- | ------------- |
 | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_smoothed_centerline.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_smoothed_centerline_fixed.png) |
 
 For very narrow rivers, this problem can become extreme and pronounced
 ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_smoothed_centerline_extreme.png)
 
 By increasing the interpolation between the centerline points, the smoothed centerlines will be forced within the polygon and reduce the number of points outside of the polygon. By default, this warning will be thrown if more than 2 points are outside of polygon, so as long as more than 2 points lie outside the polygon, the warning will recommend doubling the amount of centerline points
 
-### Fix Gaps and Jagged Centerlines
+### Fixing Gaps and Jagged Centerlines
 Gaps formed can cause part of the centerline to be skipped due to sparse data. As a result, the start and end of the centerline can skip parts at the beginning or end of a river
 ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps_short_path.png)
 Set river object created by `centerline_width.riverCenterline` to `interpolate_data=True` to fix for jagged edges or gaps formed by the interaction of sparse data and narrow banks
 ```python
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", interpolate_data=True)
 ```
 | interpolate_data = False | interpolate_data = True |
 | ------------- | ------------- |
 | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_true_no_gaps.png) |
 | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps_2.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_true_no_gaps_2.png) |
 
 The number of additional points added by interpolating can be adjusted with `interpolate_n`, but defaults to add 5 additional points between values
 
-## Development Environment
+## Development Environment	
 To run or test against `centerline-width` github repo/fork, a development environment can be created via conda/miniconda
 
 First, [install Miniconda](https://docs.conda.io/projects/miniconda/en/latest/miniconda-install.html)
 
 Then, using the existing `environment.yml`, a new conda environment can be create to run/test scripts against
 
 ```
 conda env create --file environment.yml
 ```
 Once the environment has been built, activate the environment:
 ```
 conda activate centerline_width
 ```
+Set up pre-commit hooks to ensure standard code formatting and spelling:
+```
+pre-commit install
+```
+Pre-commit hooks can be manually run before commits:
+```
+pre-commit run --all-files
+```
 To run existing and new tests from the root directory:
 ```
 python -m pytest
 ```
+## Beta :test_tube: Features
+These features are not included in pip install because they are still experimental and being tested/debugged. For more information and getting them up and running, contact cyschneck@gmail.com or ugschneck@gmail.com or post a question as a [Github Issue](https://github.com/cyschneck/centerline-width/issues)
+
+- Calculate sinuosity of river, in total and in equal parts
+
+- Calculate the dominant meander wavelength amd its variance
+
+- Calculate the asymmetry of the meanders 
+
+- Calculate the dominant submeander and supermeander scales
+
+- Extract elevation/slope from river profiles (.kml files)
+
+- Overlay plots with images via geopandas
 
 ## Citations
-Originally a Python implementation of [R-Code CMGO](https://github.com/AntoniusGolly/cmgo) (Golly et al. 2017) but has been extensively expanded:
+Originally a Python implementation of [R-Code CMGO](https://github.com/AntoniusGolly/cmgo) (Golly et al. 2017) but has since been extensively expanded:
 
 >Golly, A. and Turowski, J. M.: Deriving principal channel metrics from bank and long-profile geometry with the R package cmgo, Earth Surf. Dynam., 5, 557-570, https://doi.org/10.5194/esurf-5-557-2017, 2017.
 
  <p align="center">
   <img src="https://user-images.githubusercontent.com/22159116/222872092-e0b579cc-4f84-4f49-aa53-397785fb9bf2.png" />
   <img src="https://user-images.githubusercontent.com/22159116/222872119-7c485ee2-4ffd-413a-9e4f-b043b122d2bb.png" />
   <img src="https://user-images.githubusercontent.com/22159116/222872019-12931138-9e10-4e51-aa1e-552e72d09af0.png" />
@@ -733,15 +843,15 @@
 
 ## Acknowledging Software 
 Please acknowledge the use of this software in any publications:
 
 ```
 "River centerline/width extraction software was provided by C. Y. Schneck and U. G. Schneck, and is available at URL: https://github.com/cyschneck/centerline-width."
 ```
-Please send a copy of such publications to: cyschneck@gmail.com and ugschneck@gmail.com
+We are interested in expanding this software based on river needs, so please send a copy of such publications to: cyschneck@gmail.com and ugschneck@gmail.com
 
 
 This material is based upon work supported by the National Science Foundation Graduate Fellowship under Grant No. 2141064. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the authors and do not necessarily reflect the views of the National Science Foundation.
 
-## Bug and Feature Request
+## Bug :bug: and Feature Requests
 
 Submit a bug fix, question, or feature request as a [Github Issue](https://github.com/cyschneck/centerline-width/issues) or to ugschneck@gmail.com/cyschneck@gmail.com
```

### Comparing `centerline-width-1.5.0/README.md` & `centerline-width-1.6.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 # Centerline-Width
  <p align="center">
   <img src="https://raw.githubusercontent.com/cyschneck/centerline-width/main/assets/centerline_logo.jpg" />
 </p>
 
 ![PyPi](https://img.shields.io/pypi/v/centerline-width)
 ![license](https://img.shields.io/github/license/cyschneck/centerline-width)
+[![repo-status](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 [![NSF-2141064](https://img.shields.io/badge/NSF-2141064-blue)](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2141064&HistoricalAwards=false)
 ![PyPi-Versions](https://img.shields.io/pypi/pyversions/centerline-width)
 [![pytests](https://github.com/cyschneck/centerline-width/actions/workflows/pytests.yml/badge.svg)](https://github.com/cyschneck/centerline-width/actions/workflows/pytests.yml)
+[![pre-commit](https://github.com/cyschneck/centerline-width/actions/workflows/pre-commit.yml/badge.svg)](https://github.com/cyschneck/centerline-width/actions/workflows/pre-commit.yml)
+[![codecov](https://codecov.io/gh/cyschneck/centerline-width/graph/badge.svg?token=V6Z2DC37MT)](https://codecov.io/gh/cyschneck/centerline-width)
 
 Find the centerline and width of rivers based on the latitude and longitude positions from the right and left bank 
 
 * **Convert raw data from Google Earth Pro to CSV**
 	* extractPointsToTextFile()
 	* convertColumnsToCSV()
 * **Find centerline and width of river**
@@ -19,16 +22,18 @@
 	* plotCenterlineWidth()
 	* riverWidthFromCenterline()
 	* centerlineVoronoi
 	* centerlineEqualDistance 
 	* centerlineEvenlySpaced
 	* centerlineSmoothed
 	* centerlineLength
+* **Return river features**
 	* rightBankLength
 	* leftBankLength
+	* riverArea
 * **Export centerline to .CSV and .MAT files**
 	* saveCenterlineCSV()
 	* saveCenterlineMAT()
 
 | River Outlined in Google Earth Pro | Generated Centerline for the Riverbank |
 | ------------- | ------------- |
 | ![river_google_earth+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_example_google_earth.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_example.png) |
@@ -133,26 +138,26 @@
 ```
 
 ### Converted Text File to CSV
 
 Convert a text file with coordinates for a left and right bank's latitude and longitude to a csv file with columns for the left bank latitude (llat), left bank longitude (llon), right bank latitude (rlat), right bank longitude (rlon)
 
 ```
-convertColumnsToCSV(text_file=None, flipBankDirection=False)
+convertColumnsToCSV(text_file=None, flip_direction=False)
 ```
 * **[REQUIRED]** text_file (string): File location of the text file to convert
-* [OPTIONAL] flipBankDirection (boolean): If the latitude/longitude of the banks are generated in reverse order, flip the final values so left/right bank are in order
+* [OPTIONAL] flip_direction (boolean): If the latitude/longitude of the banks are generated in reverse order, flip the final values so left/right bank are in order
 
 Scripts expects data as a list of point for left and right banks:
 - Header: llat, llon, rlat, rlon
 
 ```python
 import centerline_width
 centerline_width.convertColumnsToCSV(text_file="data/river_coords.txt",
-				flipBankDirection=True)
+				flip_direction=True)
 ```
 Converts text file:
 ```
      llat       llon      rlat       rlon
 30.037581 -92.868569 30.037441 -92.867476
 30.037613 -92.868549 30.037448 -92.867474
 30.037648 -92.868546 30.037482 -92.867449
@@ -184,15 +189,15 @@
 ```
 * **[REQUIRED]** csv_data (string): File location of the text file to convert
 * [OPTIONAL] optional_cutoff (int): Include only the first x number of the data to chart (useful for debugging)
 * [OPTIONAL] interpolate_data (boolean): Interpolate between existing data by adding additional points
 * [OPTIONAL] interpolate_n (int): Number of additional points to add between existing data, defaults to 5 (note: larger numbers will take exponentially longer to run, recommends less than 15)
 * [OPTIONAL] interpolate_n_centerpoints (int): Number of points used to interpolate the Voronoi centerline, defaults to the the length of the data frame (df_len)
 * [OPTIONAL] equal_distance (int): Equal distance between points (in meters) used to interpolate the Voronoi centerline, defaults 10 meters
-* [OPTIONAL] ellipsoid (string): Ellipsoid definition of Earth to provide size and shape for built-in functions to convert degrees to meters, options include (is sensitive to case): ["GRS80", "airy", "bessel", "clrk66", "intl", "WGS60", "WGS66", "WGS72", "WGS84", "sphere"] for more details: ["Built-in ellipsoid defintions"](https://proj.org/en/9.2/usage/ellipsoids.html#built-in-ellipsoid-definitions), defaults to "WGS84"
+* [OPTIONAL] ellipsoid (string): Ellipsoid definition of Earth to provide size and shape for built-in functions to convert degrees to meters, options include (is sensitive to case): ["GRS80", "airy", "bessel", "clrk66", "intl", "WGS60", "WGS66", "WGS72", "WGS84", "sphere"] for more details: ["Built-in ellipsoid definitions"](https://proj.org/en/9.2/usage/ellipsoids.html#built-in-ellipsoid-definitions), defaults to "WGS84"
 
 **Equal Distance - Equal linear distance between points**
 
 `equal_distance` will generate points along the centerline that are an equal linear distance from one another in meters. When `equal_distance=5` each point will be 5 meters apart
 
 | equal_distance=5 | equal_distance=20 |
 | ------------- | ------------- |
@@ -215,14 +220,15 @@
 * centerlineVoronoi (list of tuples): List of the latitude and longitude coordinates of the centerline generated by Voronoi diagrams
 * centerlineEqualDistance (list of tuples): List of the latitude and longitude coordinates of the centerline generated by equal distances between coordinates from the Voronoi diagrams
 * centerlineEvenlySpaced (list of tuples): List of the latitude and longitude coordinates of the centerline generated by evenly spacing out points generated by the Voronoi diagrams
 * centerlineSmoothed (list of tuples): List of the latitude and longitude coordinates of the centerline generated by smoothing out the evenly spaced-out points generated by the Voronoi diagrams
 * centerlineLength (float): Length of the centerline of the river (in km)
 * rightBankLength (float): Length of the right bank of the river (in km)
 * leftBankLength (float): Length of the left bank of the river (in km)
+* riverArea (float): Area contained within river bank polygon (in km^2)
 * centerlineVoronoiRelative (list of tuples): List of the relative distance coordinates of the centerline generated by Voronoi diagrams
 * centerlineEqualDistanceRelative (list of tuples): List of the relative distance coordinates of the centerline generated by equal distances between coordinates from the Voronoi diagrams
 * centerlineEvenlySpacedRelative (list of tuples): List of the relative distance coordinates of the centerline generated by evenly spacing out points generated by the Voronoi diagrams
 * centerlineSmoothedRelative (list of tuples): List of the relative distance coordinates of the centerline generated by smoothing out the evenly spaced out points generated by the Voronoi diagrams
 
 **Object (class) additional attributes:**
 
@@ -368,14 +374,27 @@
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
 river_centerline_length = river_object.centerlineLength
 ```
 The length of the river centerline returns `215.34700589636674` km
 
+### Area of River
+Return the area contained within the polygon generated the left and right bank latitude/longitudes
+```
+river_object.riverArea
+```
+Area returned in kilometers^2
+```python
+import centerline_width
+river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
+river_area = river_object.riverArea
+```
+The area of the river returns `334.0398585246558` km^2
+
 ## Plot Centerline in Matplotlib
 Plot the centerline created from a list of right and left banks
 
 ```
 plotCenterline(centerline_type="Voronoi",
 		marker_type="line",
 		centerline_color="black",
@@ -390,28 +409,93 @@
 ```
 * [OPTIONAL] centerline_type (string): Centerline type graph within river (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
 * [OPTIONAL] marker_type (string): Graph type (not case-sensitive), options: ["Line", "Scatter"], defaults to "Line"
 * [OPTIONAL] centerline_color (string): Color of centerline coordinates on graph (not case-sensitive), options: [matplotlib named colors](https://matplotlib.org/stable/gallery/color/named_colors.html), defaults to "black"
 * [OPTIONAL] dark_mode (bool): Change plot to a black ground (and override if `centerline_color="black"` to `centerline_color="white"`), defaults to False
 * [OPTIONAL] equal_axis (bool): Set x/y axes in plot to be equal, defaults to False
 * [OPTIONAL] display_all_possible_paths (boolean): Display all possible paths, not just the centerline (useful for debugging), defaults to False
-* [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False"
+* [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False, Interpolated = True/False"
 * [OPTIONAL] save_plot_name (string): Save the plot with a given name and location
 * [OPTIONAL] display_voronoi (boolean): Overlay Voronoi diagram used to generate centerline, defaults to False
 * [OPTIONAL] show_plot (boolean): display and open plots (plt.show() in Matplotlib), defaults to True
 * [OPTIONAL] coordinate_unit (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longitude) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degrees"
 
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
 river_object.plotCenterline()
 ```
-Output:
 ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_centerline.png)
 
+**centerline_type**
+
+Display different centerline types in plot ("Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"), but defaults to "Voronoi"
+
+| centerline_type="Voronoi" | centerline_type="Smoothed" |
+| ------------- | ------------- |
+| ![centerline_type_voronoi+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_centerline.png) | ![centerline_type_equal_distance+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_centerline_type_smoothed.png) |
+
+**marker_type**
+
+Display centerline plot as either line or scatter
+
+| marker_type="Line" | marker_type="Scatter" |
+| ------------- | ------------- |
+| ![marker_type_line+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_centerline.png)  | ![marker_type_scatter+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_marker_type_scatter.png) |
+
+**centerline_color**
+
+Change the color of the centerline, defaults to black
+
+| centerline_color="black" | centerline_color="palegreen" |
+| ------------- | ------------- |
+| ![centerline_color_black+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_centerline.png) | ![centerline_color_purple+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_centerline_color.png) |
+
+**dark_mode**
+
+dark_mode will change the default Matplotlib background black and swap `centerline_color` from default black to white
+
+| dark_mode=False | dark_mode=True |
+| ------------- | ------------- |
+| ![dark_mode_false+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_centerline.png) | ![dark_mode_true+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_dark_mode.png) |
+
+**equal_axis**
+
+equal_axis will set the x and y axis of the plot to be equal
+
+| equal_axis=False | equal_axis=True |
+| ------------- | ------------- |
+| ![river_not_equal+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_equal_axis_false.png) | ![river_equal+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_equal_axis_true.png)|
+
+**display_all_possible_paths**
+
+Display all possible paths generated by Voronoi edge ridges, defaults to False
+
+| display_all_possible_paths=False | display_all_possible_paths=True |
+| ------------- | ------------- |
+| ![display_all_possible_paths_false+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_centerline.png) | ![display_all_possible_paths_true+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_display_all_possible_paths_true.png) |
+
+**display_voronoi**
+
+Overlay Voronoi diagram used to generate centerline, defaults to False
+
+| display_voronoi=False | display_voronoi=True |
+| ------------- | ------------- |
+| ![display_voronoi_default+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_display_voronoi_false.png) | ![display_voronoi_true+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_display_voronoi_true.png) |
+
+
+**coordinate_unit**
+
+Plot as either "Decimal Degrees" and "Relative Distance". defaults to "Decimal Degrees" 
+
+| coordinate_unit="Decimal Degrees" | coordinate_unit="Relative Distance" |
+| ------------- | ------------- |
+| ![coordinate_unit_dd+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_centerline.png) | ![coordinate_unit_rd+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coordinate_unit_rd.png) |
+
+
 ## Plot Centerline Width Lines in Matplotlib
 ### Plot the Centerline Width Lines
 Plot the width of the river based on the centerline
 
 ```
 plotCenterlineWidth(plot_title=None, 
 		save_plot_name=None, 
@@ -422,27 +506,35 @@
 		flag_intersections=True,
 		remove_intersections=False,
 		dark_mode=False,
 		equal_axis=False,
 		show_plot=True,
 		coordinate_unit="Decimal Degrees")
 ```
-* [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False"
+* [OPTIONAL] plot_title (string): Change plot title, defaults to "River Width Coordinates: Valid Centerline = True/False, Valid Polygon = True/False, Centerline made of <interpolate_n_centerpoints> Fixed Points, width lines generated every <transect_span_distance> points, Interpolated = True/False"
 * [OPTIONAL] save_plot_name (string): Save the plot with a given name and location
 * [OPTIONAL] display_true_centerline (boolean): Display generated true centerline based on Voronoi diagrams, defaults to True
 * [OPTIONAL] transect_span_distance (int): Number n points around a center point to determine the slope (increase to decrease the impact of sudden changes), defaults to 3, must be greater than 1 (since the slope is found from the difference in position between two points)
 * [OPTIONAL] transect_slope (str): Determine how the width lines are generated, either by averaging all slopes "Average" or directly from the first to last point in the span distance as "Direct", defaults to "Average"
 * [OPTIONAL] apply_smoothing (boolean): Apply a B-spline smoothing to centerline
 * [OPTIONAL] flag_intersections (boolean): Display intersecting width lines as red in graph, defaults to True
 * [OPTIONAL] remove_intersections (boolean): Remove intersecting lines (but maintain the most width lines as possible) and only return non-intersecting width lines, defaults to False
 * [OPTIONAL] dark_mode (bool): Change plot to a black ground (and override if `centerline_color="black"` to `centerline_color="white"`), defaults to False
 * [OPTIONAL] equal_axis (bool): Set x/y axes in plot to be equal, defaults to False
 * [OPTIONAL] show_plot (boolean): display and open plots (plt.show() in Matplotlib), defaults to True
 * [OPTIONAL] coordinate_unit (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longitude) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degrees"
 
+
+```python
+import centerline_width
+river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
+river_object.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
+```
+![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width.png)
+
 **display_true_centerline**
 
 The width lines are generated from the evenly spaced coordinate (by default) or with the smoothed coordinates (when `apply_smoothing=True`), but display_true_centerline will overlay the Voronoi centerline on top of the plot
 
 | display_true_centerline=True | display_true_centerline=False |
 | ------------- | ------------- |
 | ![river_with_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_with_centerline.png) | ![river_no_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_without_centerline.png) |
@@ -488,15 +580,15 @@
 
 | remove_intersections=False | remove_intersections=True |
 | ------------- | ------------- |
 | ![river_keep+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_keep_intersections.png) | ![river_remove+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_remove_intersections.png)|
 
 **dark_mode**
 
-dark_mode will change the default Matplotlib background black and swap `centerline_color` from black to white
+dark_mode will change the default Matplotlib background black and swap `centerline_color` from default black to white
 
 | dark_mode=False | dark_mode=True |
 | ------------- | ------------- |
 | ![river_white+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_dark_mode_false.png) | ![river_black+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_dark_mode_true.png)|
 
 **equal_axis**
 
@@ -506,25 +598,18 @@
 | ------------- | ------------- |
 | ![river_not_equal+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_not_equal_default_ax.png) | ![river_equal+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_equal_ax.png)|
 
 **coordinate_unit**
 
 Two options for measuring and displaying coordinates. The two options are "Decimal Degrees" and "Relative Distance". "Decimal Degrees" is the default option that uses the original data coordinate system with latitude/longitude. "Relative Distance" changes the coordinates of each point to be the distance (in meters) from the first point on the left bank
 
-| coordinate_unit="Decimal Degrees" | remove_intersections="Relative Distance" |
+| coordinate_unit="Decimal Degrees" | coordinate_unit="Relative Distance" |
 | ------------- | ------------- |
 | ![dd_coords+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_decimal_degrees.png) | ![rd_coords+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_relative_distance.png)|
 
-```python
-import centerline_width
-river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
-river_object.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
-```
-![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width.png)
-
 ### Return Width of River
 Return the width of the river at each (evenly spaced or smoothed) with coordinates where width line intersects either the centerline, `(Centerline Longitude, Centerline Latitude) : width`, or riverbanks, `((Right Bank Longitude, Right Bank Latitude), (Left Bank Longitude, Left Bank Latitude)) : width` in kilometers
 
 ```
 riverWidthFromCenterline(transect_span_distance=3,
 			transect_slope="Average",
 			apply_smoothing=True,
@@ -556,137 +641,162 @@
 Note: it is best practice to plot the centerline and width with same arguments in `plotCenterlineWidth()` to ensure that the results when `save_to_csv=True` are as expected
 
 ## Documentation and Algorithm to Determine Centerline
 
 The centerline is defined by the greatest distance from the right and left bank, created from a Voronoi Diagram. The remaining paths within the river are filtered through Dijkstra's algorithm to find the shortest path that is the centerline
 
 ### Right and Left bank points are plotted (X-Axis for Latitude, Y-Axis for Longitude)
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example1.png)
+![algorithm_step1+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/algorithm_step1.png)
 
 ### Generate a polygon to encapsulate the river between the right and left banks to define in and outside of river
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example2.png)
+![algorithm_step2+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/algorithm_step2.png)
 
 ### Generate a Voronoi diagram based on the points along the riverbanks
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example3.png)
+![algorithm_step3+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/algorithm_step3.png)
 
 ### Display Voronoi ridge vertices that lie within the polygon (within the riverbanks)
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example4.png)
+Filter out any point pairs that only have one connection to filter out the short dead end paths
 
-### Filter out any point pairs that only have one connection to filter out the short dead end paths
 With the vertices removed, it is possible to form multiple unconnected graphs within the polygon. The largest subgraph is assumed to contain the centerline and the other subgraphs are filtered out
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example6.png)
+![algorithm_step4+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/algorithm_step4.png)
+
+### Define Top and Bottom of Polygon
+The top of the river is defined as the last plotted points in the data, while the bottom of the river is the first plotted points
+![algorithm_step5+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/algorithm_step5.png)
 
 ### Find the starting and ending node based on distance from the top and bottom of polygon
 The starting/ending node is defined by the vertex closest to the top/bottom of the polygon along the longest path
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example7.png)
+![algorithm_step6+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/algorithm_step6.png)
 
 ### Find the shortest path from the starting node to the ending node ([Dijkstra's Algorithm](https://networkx.org/documentation/stable/reference/algorithms/generated/networkx.algorithms.shortest_paths.generic.shortest_path.html#networkx.algorithms.shortest_paths.generic.shortest_path))
 | Points on Riverbank | NetworkX Graph of Points on Riverbank |
 | ------------- | ------------- |
-| ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example10.png) | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example9.png) |
+| ![algorithm_step7+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/algorithm_step7.png) | ![algorithm_step8+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/algorithm_step8.png) |
 
 ### Display the centerline found by connecting the starting/ending node with the shortest path
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example8.png)
+![algorithm_step9+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/algorithm_step9.png)
 
 This is an attempt at a more robust algorithm working from raw data to ensure that all dead ends are removed, and no gaps exist in the centerline
 
 Points that only have one connection are removed, but limiting the number of connections for a point to just two will create gaps. The Voronoi vertices connect to other vertex values, but some connect to more and some only connect to one other point. Removing additional values will create gaps, so this is avoided in this code by not applying additional filters.
 
 **All vertices:**
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example4.png)
+![algorithm_step4+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/algorithm_step4.png)
 
 **Vertices that have at least two connections (that would create gaps):**
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example5.png)
+![algorithm_step10+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/algorithm_step10.png)
 
 ## Debugging, Error Handling, and Edge Cases
 ### Wide Start/End of River
 If the data starts or ends with a large width, it is possible for the starting/ending nodes to end up in the wrong position
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_example3.png)
+![invalid_too_wide+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_too_wide.png)
 Currently, the starting node is determined by the closest node on the path to the top of the bank (in green) and the ending node is determined by the closest node on the path to the bottom of the bank (in red) that sits along the longest path
 
 ### Invalid Polygon
 A polygon is formed to encapsulate the river with the given data (to determine the inside and outside of the river). The top and bottom are connected by a straight line from the start/end of the available data. As a result, it is possible for this straight line to overlap and create an invalid polygon.
 
 A polygon is invalid if it overlaps within itself:
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_example1.png)
+![invalid_minor_polygon+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_minor_polygon.png)
 In this example, the polygon is invalid, but with such a small overlap it is still able to find a valid path
 
 With limited data, the polygon will overlap more dramatically and will struggle to find a valid centerline:
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_example4.png)
+![invalid_major_polygon+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_major_polygon.png)
 
 ### Invalid Centerline
-If the data is too small, a centerline and its coordinates cannot not be found (since only a single Voronoi vertex exists within the polygon and after dead ends are filtered)
+If the data is too small, a centerline and its coordinates cannot be found (since only a single Voronoi vertex exists within the polygon and after dead ends are filtered)
 
-`CRITICAL ERROR, Polygon too short for the Voronoi diagram generated (no starting node found), unable to plot centerline. Set displayVoronoi=True to view vertices. Can typically be fixed by adding more data to expand range.`
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_example2.png)
+`CRITICAL ERROR, Polygon too short for the Voronoi diagram generated (no starting node found), unable to plot centerline. Set display_voronoi=True to view vertices. Can typically be fixed by adding more data to expand range`
+![invalid_too_small+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_too_small.png)
 Can be fixed by expanding the data until the polygon is large enough to contain at least two different vertex points
 
-### Invalid Top and Bottom Bank Positions (flipBankDirection = True)
-Error: `WARNING: Invalid Polygon Due to Flipped Banks, fix recommendation: rerun convertColumnsToCSV() and set flipBankDirection=True (or reset to default 'False' if currently set to flipBankDirection=True)`
+### Invalid Top and Bottom Bank Positions (flip_direction = True)
+Error: `WARNING: Invalid Polygon Due to Flipped Banks, fix recommendation: rerun convertColumnsToCSV() and set flip_direction=True (or reset to default 'False' if currently set to flip_direction=True)`
 
 If the data for the left and right riverbanks are generated in reverse order, they will be read in the incorrect order and the graph will find the invalid top and bottom of the bank
 
 If the latitude/longitude of the banks are generated in reverse order, flip the final values so left/right bank are in order
 
-This can be fixed by using the flipBankDirection optional argument `centerline_width.convertColumnsToCSV(text_file="data_example.txt", flipBankDirection=True)`
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/flipDirection_example.png)
+This can be fixed by using the flip_direction optional argument `centerline_width.convertColumnsToCSV(text_file="data_example.txt", flip_direction=True)`
+![invalid_flipped_banks+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_flipped_banks.png)
 
 ### Invalid Smoothed Centerline
 The smoothed centerline (`river_object.centerlineSmoothed`) can end up lying outside the river if the centerline data points are sparse in a narrow river. If more than two points in the smoothed centerline lie outside the river, a warning will be thrown
 
 Example Error: `WARNING: Partially invalid smoothed centerline due to sparse centerline data (6 points lie outside the polygon), fix recommendation: rerun riverCenterline to create river object with interpolate_n_centerpoints set to 62+`
 
-By default, `interpolate_n_centerpoints` is set to None and not additional points will be added between the existing points along the centerline. By adding additional points between the existing centerline, the smoothed centerline can be fixed to stay within the polygon. This fix is set by creating a river object, `centerline_width.riverCenterline`, with `interpolate_n_centerpoints=65` (with the recommended 62+) to fix for centerline coordinates that lie outside the polygon
+By default, `interpolate_n_centerpoints` is set to None and no additional points will be added between the existing points along the centerline. By adding additional points between the existing centerline, the smoothed centerline can be fixed to stay within the polygon. This fix is set by creating a river object, `centerline_width.riverCenterline`, with `interpolate_n_centerpoints=65` (with the recommended 62+) to fix for centerline coordinates that lie outside the polygon
 
 `interpolate_n_centerpoints = None` does not interpolate data points, so the size will be set to the number of fixed points when creating the evenly spaced coordinates (equal to the size of the data frame)
 
 | interpolate_n_centerpoints = None | interpolate_n_centerpoints = 65 |
 | ------------- | ------------- |
 | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_smoothed_centerline.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_smoothed_centerline_fixed.png) |
 
 For very narrow rivers, this problem can become extreme and pronounced
 ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_smoothed_centerline_extreme.png)
 
 By increasing the interpolation between the centerline points, the smoothed centerlines will be forced within the polygon and reduce the number of points outside of the polygon. By default, this warning will be thrown if more than 2 points are outside of polygon, so as long as more than 2 points lie outside the polygon, the warning will recommend doubling the amount of centerline points
 
-### Fix Gaps and Jagged Centerlines
+### Fixing Gaps and Jagged Centerlines
 Gaps formed can cause part of the centerline to be skipped due to sparse data. As a result, the start and end of the centerline can skip parts at the beginning or end of a river
 ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps_short_path.png)
 Set river object created by `centerline_width.riverCenterline` to `interpolate_data=True` to fix for jagged edges or gaps formed by the interaction of sparse data and narrow banks
 ```python
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", interpolate_data=True)
 ```
 | interpolate_data = False | interpolate_data = True |
 | ------------- | ------------- |
 | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_true_no_gaps.png) |
 | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps_2.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_true_no_gaps_2.png) |
 
 The number of additional points added by interpolating can be adjusted with `interpolate_n`, but defaults to add 5 additional points between values
 
-## Development Environment
+## Development Environment	
 To run or test against `centerline-width` github repo/fork, a development environment can be created via conda/miniconda
 
 First, [install Miniconda](https://docs.conda.io/projects/miniconda/en/latest/miniconda-install.html)
 
 Then, using the existing `environment.yml`, a new conda environment can be create to run/test scripts against
 
 ```
 conda env create --file environment.yml
 ```
 Once the environment has been built, activate the environment:
 ```
 conda activate centerline_width
 ```
+Set up pre-commit hooks to ensure standard code formatting and spelling:
+```
+pre-commit install
+```
+Pre-commit hooks can be manually run before commits:
+```
+pre-commit run --all-files
+```
 To run existing and new tests from the root directory:
 ```
 python -m pytest
 ```
+## Beta :test_tube: Features
+These features are not included in pip install because they are still experimental and being tested/debugged. For more information and getting them up and running, contact cyschneck@gmail.com or ugschneck@gmail.com or post a question as a [Github Issue](https://github.com/cyschneck/centerline-width/issues)
+
+- Calculate sinuosity of river, in total and in equal parts
+
+- Calculate the dominant meander wavelength amd its variance
+
+- Calculate the asymmetry of the meanders 
+
+- Calculate the dominant submeander and supermeander scales
+
+- Extract elevation/slope from river profiles (.kml files)
+
+- Overlay plots with images via geopandas
 
 ## Citations
-Originally a Python implementation of [R-Code CMGO](https://github.com/AntoniusGolly/cmgo) (Golly et al. 2017) but has been extensively expanded:
+Originally a Python implementation of [R-Code CMGO](https://github.com/AntoniusGolly/cmgo) (Golly et al. 2017) but has since been extensively expanded:
 
 >Golly, A. and Turowski, J. M.: Deriving principal channel metrics from bank and long-profile geometry with the R package cmgo, Earth Surf. Dynam., 5, 557-570, https://doi.org/10.5194/esurf-5-557-2017, 2017.
 
  <p align="center">
   <img src="https://user-images.githubusercontent.com/22159116/222872092-e0b579cc-4f84-4f49-aa53-397785fb9bf2.png" />
   <img src="https://user-images.githubusercontent.com/22159116/222872119-7c485ee2-4ffd-413a-9e4f-b043b122d2bb.png" />
   <img src="https://user-images.githubusercontent.com/22159116/222872019-12931138-9e10-4e51-aa1e-552e72d09af0.png" />
@@ -694,15 +804,15 @@
 
 ## Acknowledging Software 
 Please acknowledge the use of this software in any publications:
 
 ```
 "River centerline/width extraction software was provided by C. Y. Schneck and U. G. Schneck, and is available at URL: https://github.com/cyschneck/centerline-width."
 ```
-Please send a copy of such publications to: cyschneck@gmail.com and ugschneck@gmail.com
+We are interested in expanding this software based on river needs, so please send a copy of such publications to: cyschneck@gmail.com and ugschneck@gmail.com
 
 
 This material is based upon work supported by the National Science Foundation Graduate Fellowship under Grant No. 2141064. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the authors and do not necessarily reflect the views of the National Science Foundation.
 
-## Bug and Feature Request
+## Bug :bug: and Feature Requests
 
 Submit a bug fix, question, or feature request as a [Github Issue](https://github.com/cyschneck/centerline-width/issues) or to ugschneck@gmail.com/cyschneck@gmail.com
```

### Comparing `centerline-width-1.5.0/centerline_width/__init__.py` & `centerline-width-1.6.0/centerline_width/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,21 +17,27 @@
 from .relativeDistance import relativeBankCoordinates
 from .relativeDistance import relativeCenterlineCoordinates
 from .relativeDistance import relativeRidgeCoordinates
 from .relativeDistance import relativeWidthCoordinates
 
 # centerline.py function calls
 from .centerline import centerlinePath
+from .centerline import generateNXGraph
 from .centerline import networkXGraphShortestPath
-from .centerline import centerlineLength
 from .centerline import equalDistanceCenterline
 from .centerline import evenlySpacedCenterline
 from .centerline import smoothedCoordinates
-from .centerline import riverWidthFromCenterlineCoordinates
-from .centerline import riverWidthFromCenterline
+
+# riverFeatures.py function calls
+from .riverFeatures import centerlineLength
+from .riverFeatures import calculateRiverArea
+
+# width.py function calls
+from .width import riverWidthFromCenterlineCoordinates
+from .width import riverWidthFromCenterline
 
 # saveOutput.py function calls
 from .saveOutput import saveCenterlineCSV
 from .saveOutput import saveCenterlineMAT
 
 # plotDiagrams.py function calls
 from .plotDiagrams import plotCenterline
```

### Comparing `centerline-width-1.5.0/centerline_width/preprocessing.py` & `centerline-width-1.6.0/centerline_width/preprocessing.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,160 +1,198 @@
-# Built in Python functions
+# Built-in Python functions
 import csv
 import logging
 import math
 import os
-
-# External Python libraries (installed via pip install)
 from collections import Counter
+
+# External Python libraries
 import numpy as np
 from shapely.geometry import Point, Polygon, LineString
 from scipy.spatial import Voronoi
 
 # Internal centerline_width reference to access functions, global variables, and error handling
 import centerline_width
 
 ## Logging set up for .INFO
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 stream_handler = logging.StreamHandler()
 logger.addHandler(stream_handler)
 
-def convertColumnsToCSV(text_file=None, flipBankDirection=False):
-	# Convert txt file to a comma seperated version of the file to use in pandas
-	centerline_width.errrorHandlingConvertColumnsToCSV(text_file=text_file, flipBankDirection=flipBankDirection)
-
-	left_rows = []
-	right_rows = []
-	with open(text_file) as input_file:
-		lines = input_file.readlines()
-		for i, line in enumerate(lines):
-			line = line.strip().split(" ")
-			line = [x for x in line if x != '']
-			if i == 0:
-				header_fields = line
-			else:
-				left_rows.append(line[:2])
-				right_rows.append(line[2:])
-
-	# reverse the direction for the right bank
-	if flipBankDirection:
-		right_rows = right_rows[::-1]
-
-	total_rows = []
-	for i, row in enumerate(left_rows):
-		total_rows.append(row + right_rows[i])
-
-	# account for relative and absolute paths to use text_file name and location for .csv
-	full_path, filename = os.path.split(os.path.abspath(text_file))
-	csv_file_name = filename.split(".")[0] + ".csv"
-	write_file_name = os.path.join(full_path, csv_file_name)
-
-	with open(write_file_name, "w") as f:
-		write = csv.writer(f)
-		write.writerow(header_fields)
-		write.writerows(total_rows)
-
-def leftRightCoordinates(dataframe):
-	right_bank_coordinates = [] # without nan
-	left_bank_coordinates = [] # wtihout nan
-	for index, row in dataframe.iterrows():
-		if not math.isnan(row.rlat) and not math.isnan(row.rlon):
-			right_bank_coordinates.append([row.rlon, row.rlat])
-		if not math.isnan(row.llat) and not math.isnan(row.llon):
-			left_bank_coordinates.append([row.llon, row.llat])
-	return left_bank_coordinates, right_bank_coordinates
-
-def generatePolygon(left_bank_lst, right_bank_lst, coord_type=None, recursion_check=False):
-	# Return a shapely polygon based on the position of the river bank points
-	if len(right_bank_lst) == 0:
-		logger.critical("\nCRITICAL ERROR, right bank data is empty (or NaN)")
-		exit()
-	if len(left_bank_lst) == 0:
-		logger.critical("\nCRITICAL ERROR, left bank data is empty (or NaN)")
-		exit()
-	circular_list_of_banks = left_bank_lst + right_bank_lst[::-1] + [left_bank_lst[0]]
-
-	river_polygon = Polygon(circular_list_of_banks)
-	top_river = LineString([Point(left_bank_lst[::-1][0][0],left_bank_lst[::-1][0][1]), Point(right_bank_lst[::-1][0][0], right_bank_lst[::-1][0][1])])
-	bottom_river = LineString([Point(right_bank_lst[0][0], right_bank_lst[0][1]), Point(left_bank_lst[0][0], left_bank_lst[0][1])])
-
-	if not river_polygon.is_valid and not recursion_check:
-		logger.critical(f"[FAILED]  Invalid Polygon may need to be corrected - {coord_type}")
-		# only run once with recursion_check set (just to check if reverse banks fixes issue)
-		polygon_check, _, _ = generatePolygon(left_bank_lst=left_bank_lst,
-											  right_bank_lst=right_bank_lst[::-1],
-											  coord_type=coord_type,
-											  recursion_check=True) 
-		if polygon_check.is_valid:
-			logger.critical("\nWARNING: Invalid Polygon Due to Flipped Banks, fix recommendation: rerun convertColumnsToCSV() and set flipBankDirection=True (or reset to default 'False' if currently set to flipBankDirection=True)\n")
-	if river_polygon.is_valid and not recursion_check:
-		logger.info(f"[SUCCESS] Valid polygon generated - {coord_type}")
-
-	return river_polygon, top_river, bottom_river
-
-def generateVoronoi(left_bank_lst, right_bank_lst, coord_type=None):
-	# Generate a Voronoi shape based on the left/right bank points
-	all_banks_points = left_bank_lst + right_bank_lst
-	all_banks_points = np.array(all_banks_points)
-
-	river_voronoi = Voronoi(all_banks_points)
-	logger.info(f"[SUCCESS] Voronoi diagram generated - {coord_type}")
-	return river_voronoi
-
-def pointsFromVoronoi(river_voronoi, river_polygon):
-	# Returns a dictionary list of all the voronoi points: {start point : [list of end points]}
-	points_dict = {}
-	all_connections_start_to_end = []
-	logger.info("[PROCESSING] Attempting to determine a valid centerline from Voronoi points, may take a few minutes...") # longest step, O(n^n)
-	for ridge_vertex_point in river_voronoi.ridge_vertices:
-		if ridge_vertex_point[0] >= 0 and ridge_vertex_point[1] >= 0: # Only include non-infinity vertex edges
-			v0 = river_voronoi.vertices[ridge_vertex_point[0]]
-			v1 = river_voronoi.vertices[ridge_vertex_point[1]]
-			# Check if start and end points are within the polygon, otherwise remove the connection pair
-			if river_polygon.contains(Point([v0[0], v0[1]])) and river_polygon.contains(Point([v1[0], v1[1]])):
-				start_point = tuple([v0[0], v0[1]])
-				end_point = tuple([v1[0], v1[1]])
-				start_to_end = [start_point, end_point]
-				if start_to_end not in all_connections_start_to_end: 
-					all_connections_start_to_end.append(start_to_end)
-
-	# Dictionary with connections that have at least one connection
-	connections_counter_start_to_end = Counter(x for xs in all_connections_start_to_end for x in set(xs)) # counter the amount of connections for each point
-	for connection in all_connections_start_to_end:
-		start_point = connection[0]
-		end_point = connection[1]
-		# Only plot points with at least two connections (removes any edges that are not connected to additional points)
-		if connections_counter_start_to_end[start_point] > 1:
-			if connections_counter_start_to_end[end_point] > 1: 
-				if start_point not in points_dict.keys():
-					points_dict[start_point] = []
-				points_dict[start_point].append(end_point)
-
-	return points_dict
-
-def interpolateBetweenPoints(left_bank_coordinates, right_bank_coordinates, interpolate_n):
-	# Interpolated between points at an even distance along the river banks to attempt to even out Voronoi diagrams
-	interpolate_n += 2 # adds two exta points, to ensure that interpolating is adding the points between the existing points
-	def interpolateList(lst):
-		# Add points to existing list to increase resolution
-		#haversine_distance_between = haversine((lat1, lon1), (lat2, lon2), unit=units)
-		bank_expanded = []
-		for i in range(len(lst)):
-			if i+1 < len(lst):
-				lon1, lat1 = lst[i][0], lst[i][1]
-				lon2, lat2 = lst[i+1][0], lst[i+1][1]
-
-				x_expand = np.linspace(lon1, lon2, interpolate_n)
-				y_expand = np.linspace(lat1, lat2, interpolate_n)
-
-				for j in range(len(x_expand)):
-					bank_expanded.append([x_expand[j],y_expand[j]])
-				bank_expanded.append(lst[i+1]) # add end position (np.linspace excludes ending position)
-			else: 
-				bank_expanded.append(lst[i])
-		return bank_expanded
 
-	right_interpolated_coordinates = interpolateList(right_bank_coordinates)
-	left_interpolated_coordinates = interpolateList(left_bank_coordinates)
+def convertColumnsToCSV(text_file: str = None,
+                        flip_direction: bool = False) -> None:
+    # Convert txt file to a comma-separated version of the file to use in pandas
+    centerline_width.errrorHandlingConvertColumnsToCSV(
+        text_file=text_file, flip_direction=flip_direction)
+
+    left_rows = []
+    right_rows = []
+    with open(text_file) as input_file:
+        lines = input_file.readlines()
+        for i, line in enumerate(lines):
+            line = line.strip().split(" ")
+            line = [x for x in line if x != '']
+            if i == 0:
+                header_fields = line
+            else:
+                left_rows.append(line[:2])
+                right_rows.append(line[2:])
+
+    # reverse the direction for the right bank
+    if flip_direction:
+        right_rows = right_rows[::-1]
+
+    total_rows = []
+    for i, row in enumerate(left_rows):
+        total_rows.append(row + right_rows[i])
+
+    # account for relative and absolute paths to use text_file name and location for .csv
+    full_path, filename = os.path.split(os.path.abspath(text_file))
+    csv_file_name = filename.split(".")[0] + ".csv"
+    write_file_name = os.path.join(full_path, csv_file_name)
+
+    with open(write_file_name, "w") as f:
+        write = csv.writer(f)
+        write.writerow(header_fields)
+        write.writerows(total_rows)
+
+
+def leftRightCoordinates(dataframe=None):
+    right_bank_coordinates = []  # without nan
+    left_bank_coordinates = []  # without nan
+    for index, row in dataframe.iterrows():
+        if not math.isnan(row.rlat) and not math.isnan(row.rlon):
+            right_bank_coordinates.append([row.rlon, row.rlat])
+        if not math.isnan(row.llat) and not math.isnan(row.llon):
+            left_bank_coordinates.append([row.llon, row.llat])
+    return left_bank_coordinates, right_bank_coordinates
+
+
+def generatePolygon(
+        left_bank_lst: list = None,
+        right_bank_lst: list = None,
+        coord_type: str = None,
+        recursion_check: bool = False) -> [Polygon, LineString, LineString]:
+    # Return a shapely polygon based on the position of the river bank points
+    if len(right_bank_lst) == 0:
+        raise ValueError("CRITICAL ERROR, right bank data is empty (or NaN)")
+    if len(left_bank_lst) == 0:
+        raise ValueError("\nCRITICAL ERROR, left bank data is empty (or NaN)")
+    circular_list_of_banks = left_bank_lst + right_bank_lst[::-1] + [
+        left_bank_lst[0]
+    ]
+
+    river_polygon = Polygon(circular_list_of_banks)
+    top_river = LineString([
+        Point(left_bank_lst[::-1][0][0], left_bank_lst[::-1][0][1]),
+        Point(right_bank_lst[::-1][0][0], right_bank_lst[::-1][0][1])
+    ])
+    bottom_river = LineString([
+        Point(right_bank_lst[0][0], right_bank_lst[0][1]),
+        Point(left_bank_lst[0][0], left_bank_lst[0][1])
+    ])
+
+    if not river_polygon.is_valid and not recursion_check:
+        logger.critical(
+            f"[FAILED]  Invalid Polygon may need to be corrected - {coord_type}"
+        )
+        # only run once with recursion_check set (just to check if reverse banks fixes issue)
+        polygon_check, _, _ = generatePolygon(
+            left_bank_lst=left_bank_lst,
+            right_bank_lst=right_bank_lst[::-1],
+            coord_type=coord_type,
+            recursion_check=True)
+        if polygon_check.is_valid:
+            logger.critical(
+                "\nWARNING: Invalid Polygon Due to Flipped Banks, fix recommendation: rerun convertColumnsToCSV() and set flip_direction=True (or reset to default 'False' if currently set to flip_direction=True)\n"
+            )
+    if river_polygon.is_valid and not recursion_check:
+        logger.info(f"[SUCCESS] Valid polygon generated - {coord_type}")
+
+    return river_polygon, top_river, bottom_river
+
+
+def generateVoronoi(left_bank_lst: list = None,
+                    right_bank_lst: list = None,
+                    coord_type: str = None) -> Voronoi:
+    # Generate a Voronoi shape based on the left/right bank points
+    all_banks_points = left_bank_lst + right_bank_lst
+    all_banks_points = np.array(all_banks_points)
+
+    river_voronoi = Voronoi(all_banks_points)
+    logger.info(f"[SUCCESS] Voronoi diagram generated - {coord_type}")
+    return river_voronoi
+
+
+def pointsFromVoronoi(river_voronoi: Voronoi = None,
+                      river_polygon: Polygon = None) -> dict:
+    # Returns a dictionary list of all the voronoi points: {start point : [list of end points]}
+    points_dict = {}
+    all_connections_start_to_end = []
+    logger.info(
+        "[PROCESSING] Attempting to determine a valid centerline from Voronoi points, may take a few minutes..."
+    )  # longest step, O(n^n)
+    for ridge_vertex_point in river_voronoi.ridge_vertices:
+        if ridge_vertex_point[0] >= 0 and ridge_vertex_point[
+                1] >= 0:  # Only include non-infinity vertex edges
+            v0 = river_voronoi.vertices[ridge_vertex_point[0]]
+            v1 = river_voronoi.vertices[ridge_vertex_point[1]]
+            # Check if start and end points are within the polygon, otherwise remove the connection pair
+            if river_polygon.contains(Point([v0[0], v0[1]
+                                             ])) and river_polygon.contains(
+                                                 Point([v1[0], v1[1]])):
+                start_point = tuple([v0[0], v0[1]])
+                end_point = tuple([v1[0], v1[1]])
+                start_to_end = [start_point, end_point]
+                if start_to_end not in all_connections_start_to_end:
+                    all_connections_start_to_end.append(start_to_end)
+
+    # Dictionary with connections that have at least one connection
+    connections_counter_start_to_end = Counter(
+        x for xs in all_connections_start_to_end
+        for x in set(xs))  # counter the amount of connections for each point
+    for connection in all_connections_start_to_end:
+        start_point = connection[0]
+        end_point = connection[1]
+        # Only plot points with at least two connections (removes any edges that are not connected to additional points)
+        if connections_counter_start_to_end[start_point] > 1:
+            if connections_counter_start_to_end[end_point] > 1:
+                if start_point not in points_dict.keys():
+                    points_dict[start_point] = []
+                points_dict[start_point].append(end_point)
+
+    return points_dict
+
+
+def interpolateBetweenPoints(left_bank_coordinates: list = None,
+                             right_bank_coordinates: list = None,
+                             interpolate_n: int = 5) -> [list, list]:
+    # Interpolated between points at an even distance along the river banks to attempt to even out Voronoi diagrams
+    interpolate_n += 2  # adds two exta points, to ensure that interpolating is adding the points between the existing points
+
+    def interpolateList(lst):
+        # Add points to existing list to increase resolution
+        #haversine_distance_between = haversine((lat1, lon1), (lat2, lon2), unit=units)
+        bank_expanded = []
+        for i in range(len(lst)):
+            if i + 1 < len(lst):
+                lon1, lat1 = lst[i][0], lst[i][1]
+                lon2, lat2 = lst[i + 1][0], lst[i + 1][1]
+
+                x_expand = np.linspace(lon1, lon2, interpolate_n)
+                y_expand = np.linspace(lat1, lat2, interpolate_n)
+
+                for j in range(len(x_expand)):
+                    bank_expanded.append([x_expand[j], y_expand[j]])
+                bank_expanded.append(
+                    lst[i + 1]
+                )  # add end position (np.linspace excludes ending position)
+            else:
+                bank_expanded.append(lst[i])
+        return bank_expanded
+
+    right_interpolated_coordinates = interpolateList(right_bank_coordinates)
+    left_interpolated_coordinates = interpolateList(left_bank_coordinates)
 
-	return right_interpolated_coordinates, left_interpolated_coordinates
+    return right_interpolated_coordinates, left_interpolated_coordinates
```

### Comparing `centerline-width-1.5.0/centerline_width/pytests/test_centerline.py` & `centerline-width-1.6.0/centerline_width/pytests/test_errorRiverCenterlineClass.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,98 +1,154 @@
-# Pytest for preprocessing.py
-# centerline-width/: python3 -m pytest -v
+# Pytest for riverCenterlineClass.py
+# centerline-width/: python -m pytest -v
 from io import StringIO
 import re
 
 # External Python libraries (installed via pip install)
 import pytest
 
 # Internal centerline-width reference to access functions, global variables, and error handling
 import centerline_width
 
 invalid_non_bool_options = [(1961, "<class 'int'>"),
-						(3.1415, "<class 'float'>"),
-						([], "<class 'list'>"),
-						("testing_string", "<class 'str'>")]
-
-invalid_non_class_options = [(1961, "<class 'int'>"),
-						(3.1415, "<class 'float'>"),
-						([], "<class 'list'>"),
-						("testing_string", "<class 'str'>"),
-						(False, "<class 'bool'>")]
+                            (3.1415, "<class 'float'>"),
+                            ([], "<class 'list'>"),
+                            ("testing_string", "<class 'str'>")]
 
 invalid_non_int_options = [("testing_string", "<class 'str'>"),
-						(3.1415, "<class 'float'>"),
-						([], "<class 'list'>"),
-						(False, "<class 'bool'>")]
+                           (3.1415, "<class 'float'>"), ([], "<class 'list'>"),
+                           (False, "<class 'bool'>")]
+
+invalid_non_num_options = [("testing_string", "<class 'str'>"),
+                           ([], "<class 'list'>"), (False, "<class 'bool'>")]
 
 invalid_non_str_options = [(1961, "<class 'int'>"),
-						(3.1415, "<class 'float'>"),
-						([], "<class 'list'>"),
-						(False, "<class 'bool'>")]
-
-def river_class_object():
-	csv_example = StringIO()
-	csv_example.write("llat,llon,rlat,rlon\n")
-	csv_example.write("30.037581,-92.868569,30.037441,-92.867476\n")
-	csv_example.write("30.137581,-92.868569,30.037441,-92.867476\n")
-	csv_example.write("30.237581,-92.868569,30.037441,-92.867476\n")
-	csv_example.seek(0)
-	return centerline_width.riverCenterline(csv_data=csv_example)
-
-river_class_example = river_class_object()
-
-## riverWidthFromCenterlineCoordinates() #####################################################
-def test_riverWidthFromCenterline_riverObjectRequired():
-	with pytest.raises(ValueError, match=re.escape("[river_object]: Requires a river object (see: centerline_width.riverCenterline)")):
-		centerline_width.riverWidthFromCenterline(river_object=None)
-
-@pytest.mark.parametrize("invalid_input, error_output", invalid_non_class_options)
-def test_riverWidthFromCenterline_riverObjectInvalidTypes(invalid_input, error_output):
-	with pytest.raises(ValueError, match=re.escape("[river_object]: Must be a river object (see: centerline_width.riverCenterline), current type = '{0}'".format(error_output))):
-		centerline_width.riverWidthFromCenterline(river_object=invalid_input)
-
-@pytest.mark.parametrize("invalid_input, error_output", invalid_non_int_options)
-def test_riverWidthFromCenterline_transectSpanDistanceInvalidTypes(invalid_input, error_output):
-	with pytest.raises(ValueError, match=re.escape(f"[transect_span_distance]: Must be a int, current type = '{error_output}'")):
-		centerline_width.riverWidthFromCenterline(river_object=river_class_example,
-											transect_span_distance=invalid_input)
-
-@pytest.mark.parametrize("invalid_input, error_output", invalid_non_bool_options)
-def test_riverWidthFromCenterline_applySmoothingInvalidTypes(invalid_input, error_output):
-	with pytest.raises(ValueError, match=re.escape(f"[apply_smoothing]: Must be a bool, current type = '{error_output}'")):
-		centerline_width.riverWidthFromCenterline(river_object=river_class_example,
-											apply_smoothing=invalid_input)
-
-@pytest.mark.parametrize("invalid_input, error_output", invalid_non_bool_options)
-def test_riverWidthFromCenterline_removeIntersectionsInvalidTypes(invalid_input, error_output):
-	with pytest.raises(ValueError, match=re.escape(f"[remove_intersections]: Must be a bool, current type = '{error_output}'")):
-		centerline_width.riverWidthFromCenterline(river_object=river_class_example,
-											remove_intersections=invalid_input)
-
-@pytest.mark.parametrize("invalid_input, error_output", invalid_non_str_options)
-def test_riverWidthFromCenterline_saveToCSVInvalidTypes(invalid_input, error_output):
-	with pytest.raises(ValueError, match=re.escape(f"[save_to_csv]: Must be a str, current type = '{error_output}'")):
-		centerline_width.riverWidthFromCenterline(river_object=river_class_example,
-											save_to_csv=invalid_input)
-
-def test_riverWidthFromCenterline_csvInvalidExtension():
-	with pytest.raises(ValueError, match=re.escape("[save_to_csv]: Extension must be a .csv file, current extension = 'txt'")):
-		centerline_width.riverWidthFromCenterline(river_object=river_class_example,
-												save_to_csv="filename.txt")
-
-def test_riverWidthFromCenterline_coordinateUnitInvalidOption():
-	with pytest.raises(ValueError, match=re.escape("[coordinate_unit]: Must be an available option in ['Decimal Degrees', 'Relative Distance'], current option = 'Invalid Option'")):
-		centerline_width.riverWidthFromCenterline(river_object=river_class_example,
-												coordinate_unit="Invalid Option")
-
-@pytest.mark.parametrize("invalid_input, error_output", invalid_non_str_options)
-def test_riverWidthFromCenterline_coordinateUnitInvalidTypes(invalid_input, error_output):
-	with pytest.raises(ValueError, match=re.escape(f"[coordinate_unit]: Must be a str, current type = '{error_output}'")):
-		centerline_width.riverWidthFromCenterline(river_object=river_class_example,
-												coordinate_unit=invalid_input)
-
-@pytest.mark.parametrize("invalid_input, error_output", invalid_non_str_options)
-def test_riverWidthFromCenterline_coordinateReferenceInvalidTypes(invalid_input, error_output):
-	with pytest.raises(ValueError, match=re.escape(f"[coordinate_reference]: Must be a str, current type = '{error_output}'")):
-		centerline_width.riverWidthFromCenterline(river_object=river_class_example,
-												coordinate_reference=invalid_input)
+                           (3.1415, "<class 'float'>"), ([], "<class 'list'>"),
+                           (False, "<class 'bool'>")]
+
+
+## class riverCenterline #####################################################
+def test_riverCenterline_csvDataRequired():
+    with pytest.raises(
+            ValueError,
+            match=re.escape("[csv_data]: Requires csv_data location")):
+        centerline_width.riverCenterline(csv_data=None)
+
+
+@pytest.mark.parametrize("invalid_input, error_output",
+                         invalid_non_str_options)
+def test_riverCenterline_csvDataInvalidTypes(invalid_input, error_output):
+    with pytest.raises(
+            ValueError,
+            match=re.escape(
+                f"[csv_data]: Must be a str, current type = '{error_output}'")
+    ):
+        centerline_width.riverCenterline(csv_data=invalid_input)
+
+
+@pytest.mark.parametrize("invalid_input, error_output",
+                         invalid_non_int_options)
+def test_riverCenterline_optionalCutoffInvalidTypes(invalid_input,
+                                                    error_output):
+    with pytest.raises(
+            ValueError,
+            match=re.escape(
+                f"[optional_cutoff]: Must be a int, current type = '{error_output}'"
+            )):
+        centerline_width.riverCenterline(csv_data="csv_example.csv",
+                                         optional_cutoff=invalid_input)
+
+
+@pytest.mark.parametrize("invalid_input, error_output",
+                         invalid_non_bool_options)
+def test_riverCenterline_interpolateDataInvalidTypes(invalid_input,
+                                                     error_output):
+    with pytest.raises(
+            ValueError,
+            match=re.escape(
+                f"[interpolate_data]: Must be a bool, current type = '{error_output}'"
+            )):
+        centerline_width.riverCenterline(csv_data="csv_example.csv",
+                                         interpolate_data=invalid_input)
+
+
+@pytest.mark.parametrize("invalid_input, error_output",
+                         invalid_non_int_options)
+def test_riverCenterline_interpolateNInvalidTypes(invalid_input, error_output):
+    with pytest.raises(
+            ValueError,
+            match=re.escape(
+                f"[interpolate_n]: Must be a int, current type = '{error_output}'"
+            )):
+        centerline_width.riverCenterline(csv_data="csv_example.csv",
+                                         interpolate_n=invalid_input)
+
+
+@pytest.mark.parametrize("invalid_input, error_output",
+                         invalid_non_int_options)
+def test_riverCenterline_interpolateNCenterpointsInvalidTypes(
+        invalid_input, error_output):
+    with pytest.raises(
+            ValueError,
+            match=re.escape(
+                f"[interpolate_n_centerpoints]: Must be a int, current type = '{error_output}'"
+            )):
+        centerline_width.riverCenterline(
+            csv_data="csv_example.csv",
+            interpolate_n_centerpoints=invalid_input)
+
+
+def test_riverCenterline_interpolateNCenterpointsInvalidRange():
+    with pytest.raises(
+            ValueError,
+            match=re.escape(
+                f"[interpolate_n_centerpoints]: Must be a greater than 1, currently = '1'"
+            )):
+        centerline_width.riverCenterline(csv_data="csv_example.csv",
+                                         interpolate_n_centerpoints=1)
+
+
+@pytest.mark.parametrize("invalid_input, error_output",
+                         invalid_non_num_options)
+def test_riverCenterline_equalDistanceInvalidTypes(invalid_input,
+                                                   error_output):
+    with pytest.raises(
+            ValueError,
+            match=re.escape(
+                f"[equal_distance]: Must be a int or float, current type = '{error_output}'"
+            )):
+        centerline_width.riverCenterline(csv_data="csv_example.csv",
+                                         equal_distance=invalid_input)
+
+
+@pytest.mark.parametrize("invalid_input, error_output", [(-1, -1), (0, 0)])
+def test_riverCenterline_equalDistanceInvalidRange(invalid_input,
+                                                   error_output):
+    with pytest.raises(
+            ValueError,
+            match=re.escape(
+                f"[equal_distance]: Must be a positive value, greater than 0, currently = '{error_output}'"
+            )):
+        centerline_width.riverCenterline(csv_data="csv_example.csv",
+                                         equal_distance=invalid_input)
+
+
+@pytest.mark.parametrize("invalid_input, error_output",
+                         invalid_non_str_options)
+def test_riverCenterline_ellipsoidInvalidTypes(invalid_input, error_output):
+    with pytest.raises(
+            ValueError,
+            match=re.escape(
+                f"[ellipsoid]: Must be a str, current type = '{error_output}'")
+    ):
+        centerline_width.riverCenterline(csv_data="csv_example.csv",
+                                         ellipsoid=invalid_input)
+
+
+def test_riverCenterline_ellipsoidInvalidOptions():
+    with pytest.raises(
+            ValueError,
+            match=re.escape(
+                "[ellipsoid]: Must be an available option in ['GRS80', 'airy', 'bessel', 'clrk66', 'intl', 'WGS60', 'WGS66', 'WGS72', 'WGS84', 'sphere'], current option = 'invalid'"
+            )):
+        centerline_width.riverCenterline(csv_data="csv_example.csv",
+                                         ellipsoid="invalid")
```

### Comparing `centerline-width-1.5.0/centerline_width/pytests/test_getCoordinatesKML.py` & `centerline-width-1.6.0/centerline_width/pytests/test_errorGetCoordinatesKML.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,50 +5,101 @@
 # External Python libraries (installed via pip install)
 import pytest
 
 # Internal centerline-width reference to access functions, global variables, and error handling
 import centerline_width
 
 invalid_non_str_options = [(1961, "<class 'int'>"),
-						(3.1415, "<class 'float'>"),
-						([], "<class 'list'>"),
-						(False, "<class 'bool'>")]
+                           (3.1415, "<class 'float'>"), ([], "<class 'list'>"),
+                           (False, "<class 'bool'>")]
+
 
 ## extractPointsToTextFile() #####################################################
 def test_extractPointsToTextFile_leftKMLRequired():
-	with pytest.raises(ValueError, match=re.escape("[left_kml]: Requires left_kml file")):
-		centerline_width.extractPointsToTextFile(left_kml=None)
+    with pytest.raises(ValueError,
+                       match=re.escape("[left_kml]: Requires left_kml file")):
+        centerline_width.extractPointsToTextFile(left_kml=None)
+
 
-@pytest.mark.parametrize("invalid_input, error_output", invalid_non_str_options)
+@pytest.mark.parametrize("invalid_input, error_output",
+                         invalid_non_str_options)
 def test_plotCenterline_leftKMLInvalidTypes(invalid_input, error_output):
-	with pytest.raises(ValueError, match=re.escape(f"[left_kml]: Must be a str, current type = '{error_output}'")):
-			centerline_width.extractPointsToTextFile(left_kml=invalid_input)
+    with pytest.raises(
+            ValueError,
+            match=re.escape(
+                f"[left_kml]: Must be a str, current type = '{error_output}'")
+    ):
+        centerline_width.extractPointsToTextFile(left_kml=invalid_input)
+
 
 def test_extractPointsToTextFile_leftKMLInvalidExtension():
-	with pytest.raises(ValueError, match=re.escape("[left_kml]: Extension must be a .kml file, current extension = 'txt'")):
-		centerline_width.extractPointsToTextFile(left_kml="left_kml.txt")
+    with pytest.raises(
+            ValueError,
+            match=re.escape(
+                "[left_kml]: Extension must be a .kml file, current extension = 'txt'"
+            )):
+        centerline_width.extractPointsToTextFile(left_kml="left_kml.txt")
+
 
 def test_extractPointsToTextFile_rightKMLRequired():
-	with pytest.raises(ValueError, match=re.escape("[right_kml]: Requires right_kml file")):
-		centerline_width.extractPointsToTextFile(left_kml="left_kml.kml", right_kml=None)
+    with pytest.raises(
+            ValueError,
+            match=re.escape("[right_kml]: Requires right_kml file")):
+        centerline_width.extractPointsToTextFile(left_kml="left_kml.kml",
+                                                 right_kml=None)
 
-@pytest.mark.parametrize("invalid_input, error_output", invalid_non_str_options)
+
+@pytest.mark.parametrize("invalid_input, error_output",
+                         invalid_non_str_options)
 def test_plotCenterline_rightKMLInvalidTypes(invalid_input, error_output):
-	with pytest.raises(ValueError, match=re.escape(f"[right_kml]: Must be a str, current type = '{error_output}'")):
-			centerline_width.extractPointsToTextFile(left_kml="left_kml.kml", right_kml=invalid_input)
+    with pytest.raises(
+            ValueError,
+            match=re.escape(
+                f"[right_kml]: Must be a str, current type = '{error_output}'")
+    ):
+        centerline_width.extractPointsToTextFile(left_kml="left_kml.kml",
+                                                 right_kml=invalid_input)
+
 
 def test_extractPointsToTextFile_rightKMLInvalidExtension():
-	with pytest.raises(ValueError, match=re.escape("[right_kml]: Extension must be a .kml file, current extension = 'txt'")):
-		centerline_width.extractPointsToTextFile(left_kml="left_kml.kml", right_kml="right_kml.txt")
+    with pytest.raises(
+            ValueError,
+            match=re.escape(
+                "[right_kml]: Extension must be a .kml file, current extension = 'txt'"
+            )):
+        centerline_width.extractPointsToTextFile(left_kml="left_kml.kml",
+                                                 right_kml="right_kml.txt")
+
 
 def test_extractPointsToTextFile_textOutputNameRequired():
-	with pytest.raises(ValueError, match=re.escape("[text_output_name]: Requires output file name")):
-		centerline_width.extractPointsToTextFile(left_kml="left_kml.kml", right_kml="right_kml.kml", text_output_name=None)
+    with pytest.raises(
+            ValueError,
+            match=re.escape("[text_output_name]: Requires output file name")):
+        centerline_width.extractPointsToTextFile(left_kml="left_kml.kml",
+                                                 right_kml="right_kml.kml",
+                                                 text_output_name=None)
+
+
+@pytest.mark.parametrize("invalid_input, error_output",
+                         invalid_non_str_options)
+def test_plotCenterline_textOutputNameInvalidTypes(invalid_input,
+                                                   error_output):
+    with pytest.raises(
+            ValueError,
+            match=re.escape(
+                f"[text_output_name]: Must be a str, current type = '{error_output}'"
+            )):
+        centerline_width.extractPointsToTextFile(
+            left_kml="left_kml.kml",
+            right_kml="right_kml.kml",
+            text_output_name=invalid_input)
 
-@pytest.mark.parametrize("invalid_input, error_output", invalid_non_str_options)
-def test_plotCenterline_textOutputNameInvalidTypes(invalid_input, error_output):
-	with pytest.raises(ValueError, match=re.escape(f"[text_output_name]: Must be a str, current type = '{error_output}'")):
-			centerline_width.extractPointsToTextFile(left_kml="left_kml.kml", right_kml="right_kml.kml", text_output_name=invalid_input)
 
 def test_extractPointsToTextFile_rightAndLeftKMLMatchInvalid():
-	with pytest.raises(ValueError, match=re.escape("right_kml and left_kml are set to the same file (needs a seperate left and right bank): right_kml='same_kml.kml' and left_kml='same_kml.kml'")):
-		centerline_width.extractPointsToTextFile(left_kml="same_kml.kml", right_kml="same_kml.kml", text_output_name=None)
+    with pytest.raises(
+            ValueError,
+            match=re.escape(
+                "right_kml and left_kml are set to the same file (needs a separate left and right bank): right_kml='same_kml.kml' and left_kml='same_kml.kml'"
+            )):
+        centerline_width.extractPointsToTextFile(left_kml="same_kml.kml",
+                                                 right_kml="same_kml.kml",
+                                                 text_output_name=None)
```

### Comparing `centerline-width-1.5.0/centerline_width/pytests/test_saveOutput.py` & `centerline-width-1.6.0/centerline_width/pytests/test_errorSaveOutput.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,144 +1,298 @@
 # Pytest for preprocessing.py
-# centerline-width/: python3 -m pytest -v
+# centerline-width/: python -m pytest -v
 from io import StringIO
 import re
 
 # External Python libraries (installed via pip install)
 import pytest
 
 # Internal centerline-width reference to access functions, global variables, and error handling
 import centerline_width
 
 invalid_non_str_options = [(1961, "<class 'int'>"),
-						(3.1415, "<class 'float'>"),
-						([], "<class 'list'>"),
-						(False, "<class 'bool'>")]
+                           (3.1415, "<class 'float'>"), ([], "<class 'list'>"),
+                           (False, "<class 'bool'>")]
+
 
 def river_class_object():
-	csv_example = StringIO()
-	csv_example.write("llat,llon,rlat,rlon\n")
-	csv_example.write("30.037581,-92.868569,30.037441,-92.867476\n")
-	csv_example.write("30.137581,-92.868569,30.037441,-92.867476\n")
-	csv_example.write("30.237581,-92.868569,30.037441,-92.867476\n")
-	csv_example.seek(0)
-	return centerline_width.riverCenterline(csv_data=csv_example)
+    csv_example = StringIO()
+    csv_example.write("llat,llon,rlat,rlon\n")
+    csv_example.write("30.037581,-92.868569,30.037441,-92.867476\n")
+    csv_example.write("30.137581,-92.868569,30.037441,-92.867476\n")
+    csv_example.write("30.237581,-92.868569,30.037441,-92.867476\n")
+    csv_example.seek(0)
+    return centerline_width.riverCenterline(csv_data=csv_example)
+
 
 river_class_example = river_class_object()
 
+
 ## saveCenterlineCSV() #####################################################
 def test_saveCenterlineCSV_riverObjectRequired():
-	with pytest.raises(ValueError, match=re.escape("[river_object]: Requires a river object (see: centerline_width.riverCenterline)")):
-		centerline_width.saveCenterlineCSV(river_object=None)
+    with pytest.raises(
+            ValueError,
+            match=re.escape(
+                "[river_object]: Requires a river object (see: centerline_width.riverCenterline)"
+            )):
+        centerline_width.saveCenterlineCSV(river_object=None)
+
+
+@pytest.mark.parametrize("invalid_input, error_output",
+                         invalid_non_str_options)
+def test_saveCenterlineCSV_riverObjectInvalidType(invalid_input, error_output):
+    with pytest.raises(
+            ValueError,
+            match=re.escape(
+                f"[river_object]: Must be a river object (see: centerline_width.riverCenterline), current type = '{error_output}'"
+            )):
+        centerline_width.saveCenterlineCSV(river_object=invalid_input)
+
 
 def test_saveCenterlineCSV_csvInvalidExtension():
-	with pytest.raises(ValueError, match=re.escape("[save_to_csv]: Requires csv filename")):
-		centerline_width.saveCenterlineCSV(river_object=river_class_example, save_to_csv=None)
+    with pytest.raises(
+            ValueError,
+            match=re.escape("[save_to_csv]: Requires csv filename")):
+        centerline_width.saveCenterlineCSV(river_object=river_class_example,
+                                           save_to_csv=None)
+
+
+@pytest.mark.parametrize("invalid_input, error_output",
+                         invalid_non_str_options)
+def test_saveCenterlineCSV_csvInvalidType(invalid_input, error_output):
+    with pytest.raises(
+            ValueError,
+            match=re.escape(
+                f"[save_to_csv]: Must be a str, current type = '{error_output}'"
+            )):
+        centerline_width.saveCenterlineCSV(river_object=river_class_example,
+                                           save_to_csv=invalid_input)
+
 
 def test_saveCenterlineCSV_csvRequired():
-	with pytest.raises(ValueError, match=re.escape("[save_to_csv]: Extension must be a .csv file, current extension = 'txt'")):
-		centerline_width.saveCenterlineCSV(river_object=river_class_example, save_to_csv="filename.txt")
+    with pytest.raises(
+            ValueError,
+            match=re.escape(
+                "[save_to_csv]: Extension must be a .csv file, current extension = 'txt'"
+            )):
+        centerline_width.saveCenterlineCSV(river_object=river_class_example,
+                                           save_to_csv="filename.txt")
+
+
+@pytest.mark.parametrize("invalid_input, error_output",
+                         invalid_non_str_options)
+def test_saveCenterlineCSV_latitudeHeaderTypeInvalidTypes(
+        invalid_input, error_output):
+    with pytest.raises(
+            ValueError,
+            match=re.escape(
+                f"[latitude_header]: Must be a str, current type = '{error_output}'"
+            )):
+        centerline_width.saveCenterlineCSV(river_object=river_class_example,
+                                           save_to_csv="testing.csv",
+                                           latitude_header=invalid_input)
+
+
+@pytest.mark.parametrize("invalid_input, error_output",
+                         invalid_non_str_options)
+def test_saveCenterlineCSV_longitudeHeaderTypeInvalidTypes(
+        invalid_input, error_output):
+    with pytest.raises(
+            ValueError,
+            match=re.escape(
+                f"[longitude_header]: Must be a str, current type = '{error_output}'"
+            )):
+        centerline_width.saveCenterlineCSV(river_object=river_class_example,
+                                           save_to_csv="testing.csv",
+                                           longitude_header=invalid_input)
+
+
+@pytest.mark.parametrize("invalid_input, error_output",
+                         invalid_non_str_options)
+def test_saveCenterlineCSV_centerlineTypeInvalidTypes(invalid_input,
+                                                      error_output):
+    with pytest.raises(
+            ValueError,
+            match=re.escape(
+                f"[centerline_type]: Must be a str, current type = '{error_output}'"
+            )):
+        centerline_width.saveCenterlineCSV(river_object=river_class_example,
+                                           save_to_csv="testing.csv",
+                                           centerline_type=invalid_input)
 
-@pytest.mark.parametrize("invalid_input, error_output", invalid_non_str_options)
-def test_saveCenterlineCSV_latitudeHeaderTypeInvalidTypes(invalid_input, error_output):
-	with pytest.raises(ValueError, match=re.escape(f"[latitude_header]: Must be a str, current type = '{error_output}'")):
-		centerline_width.saveCenterlineCSV(river_object=river_class_example,
-											save_to_csv="testing.csv",
-											latitude_header=invalid_input)
-
-@pytest.mark.parametrize("invalid_input, error_output", invalid_non_str_options)
-def test_saveCenterlineCSV_longitudeHeaderTypeInvalidTypes(invalid_input, error_output):
-	with pytest.raises(ValueError, match=re.escape(f"[longitude_header]: Must be a str, current type = '{error_output}'")):
-		centerline_width.saveCenterlineCSV(river_object=river_class_example,
-											save_to_csv="testing.csv",
-											longitude_header=invalid_input)
-
-@pytest.mark.parametrize("invalid_input, error_output", invalid_non_str_options)
-def test_saveCenterlineCSV_centerlineTypeInvalidTypes(invalid_input, error_output):
-	with pytest.raises(ValueError, match=re.escape(f"[centerline_type]: Must be a str, current type = '{error_output}'")):
-		centerline_width.saveCenterlineCSV(river_object=river_class_example,
-											save_to_csv="testing.csv",
-											centerline_type=invalid_input)
 
 def test_saveCenterlineCSV_centerlineTypeInvalidOptions():
-	with pytest.raises(ValueError, match=re.escape("[centerline_type]: Must be an available option in ['Voronoi', 'Evenly Spaced', 'Smoothed', 'Equal Distance'], current option = 'not valid'")):
-		centerline_width.saveCenterlineCSV(river_object=river_class_example,
-											save_to_csv="testing.csv",
-											centerline_type="not valid")
+    with pytest.raises(
+            ValueError,
+            match=re.escape(
+                "[centerline_type]: Must be an available option in ['Voronoi', 'Evenly Spaced', 'Smoothed', 'Equal Distance'], current option = 'not valid'"
+            )):
+        centerline_width.saveCenterlineCSV(river_object=river_class_example,
+                                           save_to_csv="testing.csv",
+                                           centerline_type="not valid")
+
 
 def test_saveCenterlineCSV_coordinateUnitInvalidOption():
-	with pytest.raises(ValueError, match=re.escape("[coordinate_unit]: Must be an available option in ['Decimal Degrees', 'Relative Distance'], current option = 'Invalid Option'")):
-		centerline_width.saveCenterlineCSV(river_object=river_class_example,
-										save_to_csv="testing.csv",
-										coordinate_unit="Invalid Option")
-
-@pytest.mark.parametrize("invalid_input, error_output", invalid_non_str_options)
-def test_saveCenterlineCSV_coordinateTypeInvalidTypes(invalid_input, error_output):
-	with pytest.raises(ValueError, match=re.escape(f"coordinate_unit]: Must be a str, current type = '{error_output}'")):
-		centerline_width.saveCenterlineCSV(river_object=river_class_example,
-										save_to_csv="testing.csv",
-										coordinate_unit=invalid_input)
+    with pytest.raises(
+            ValueError,
+            match=re.escape(
+                "[coordinate_unit]: Must be an available option in ['Decimal Degrees', 'Relative Distance'], current option = 'Invalid Option'"
+            )):
+        centerline_width.saveCenterlineCSV(river_object=river_class_example,
+                                           save_to_csv="testing.csv",
+                                           coordinate_unit="Invalid Option")
+
+
+@pytest.mark.parametrize("invalid_input, error_output",
+                         invalid_non_str_options)
+def test_saveCenterlineCSV_coordinateTypeInvalidTypes(invalid_input,
+                                                      error_output):
+    with pytest.raises(
+            ValueError,
+            match=re.escape(
+                f"coordinate_unit]: Must be a str, current type = '{error_output}'"
+            )):
+        centerline_width.saveCenterlineCSV(river_object=river_class_example,
+                                           save_to_csv="testing.csv",
+                                           coordinate_unit=invalid_input)
+
 
 ## saveCenterlineMAT() #####################################################
 def test_saveCenterlineMAT_riverObjectRequired():
-	with pytest.raises(ValueError, match=re.escape("[river_object]: Requires a river object (see: centerline_width.riverCenterline)")):
-		centerline_width.saveCenterlineMAT(river_object=None)
+    with pytest.raises(
+            ValueError,
+            match=re.escape(
+                "[river_object]: Requires a river object (see: centerline_width.riverCenterline)"
+            )):
+        centerline_width.saveCenterlineMAT(river_object=None)
+
 
 def test_saveCenterlineMAT_matInvalidExtension():
-	with pytest.raises(ValueError, match=re.escape("[save_to_mat]: Requires mat filename")):
-		centerline_width.saveCenterlineMAT(river_object=river_class_example, save_to_mat=None)
+    with pytest.raises(
+            ValueError,
+            match=re.escape("[save_to_mat]: Requires mat filename")):
+        centerline_width.saveCenterlineMAT(river_object=river_class_example,
+                                           save_to_mat=None)
+
+
+@pytest.mark.parametrize("invalid_input, error_output",
+                         invalid_non_str_options)
+def test_saveCenterlineMAT_matInvalidType(invalid_input, error_output):
+    with pytest.raises(
+            ValueError,
+            match=re.escape(
+                f"[save_to_mat]: Must be a str, current type = '{error_output}'"
+            )):
+        centerline_width.saveCenterlineMAT(river_object=river_class_example,
+                                           save_to_mat=invalid_input)
+
 
 def test_saveCenterlineMAT_matRequired():
-	with pytest.raises(ValueError, match=re.escape("[save_to_mat]: Extension must be a .mat file, current extension = 'txt'")):
-		centerline_width.saveCenterlineMAT(river_object=river_class_example, save_to_mat="filename.txt")
+    with pytest.raises(
+            ValueError,
+            match=re.escape(
+                "[save_to_mat]: Extension must be a .mat file, current extension = 'txt'"
+            )):
+        centerline_width.saveCenterlineMAT(river_object=river_class_example,
+                                           save_to_mat="filename.txt")
+
+
+@pytest.mark.parametrize("invalid_input, error_output",
+                         invalid_non_str_options)
+def test_saveCenterlineMAT_latitudeHeaderTypeInvalidTypes(
+        invalid_input, error_output):
+    with pytest.raises(
+            ValueError,
+            match=re.escape(
+                f"[latitude_header]: Must be a str, current type = '{error_output}'"
+            )):
+        centerline_width.saveCenterlineMAT(river_object=river_class_example,
+                                           save_to_mat="testing.mat",
+                                           latitude_header=invalid_input)
 
-@pytest.mark.parametrize("invalid_input, error_output", invalid_non_str_options)
-def test_saveCenterlineMAT_latitudeHeaderTypeInvalidTypes(invalid_input, error_output):
-	with pytest.raises(ValueError, match=re.escape(f"[latitude_header]: Must be a str, current type = '{error_output}'")):
-		centerline_width.saveCenterlineMAT(river_object=river_class_example,
-											save_to_mat="testing.mat",
-											latitude_header=invalid_input)
 
 def test_saveCenterlineMAT_latitudeHeaderTypeInvalidAlphanumeric():
-	with pytest.raises(ValueError, match=re.escape("[latitude_header]: Column names cannot contain any whitespace or non-alphanumeric characters, currently = 'invalid whitespace'")):
-		centerline_width.saveCenterlineMAT(river_object=river_class_example,
-											save_to_mat="testing.mat",
-											latitude_header="invalid whitespace")
-
-@pytest.mark.parametrize("invalid_input, error_output", invalid_non_str_options)
-def test_saveCenterlineMAT_longitudeHeaderTypeInvalidTypes(invalid_input, error_output):
-	with pytest.raises(ValueError, match=re.escape(f"[longitude_header]: Must be a str, current type = '{error_output}'")):
-		centerline_width.saveCenterlineMAT(river_object=river_class_example,
-											save_to_mat="testing.mat",
-											longitude_header=invalid_input)
+    with pytest.raises(
+            ValueError,
+            match=re.escape(
+                "[latitude_header]: Column names cannot contain any whitespace or non-alphanumeric characters, currently = 'invalid whitespace'"
+            )):
+        centerline_width.saveCenterlineMAT(
+            river_object=river_class_example,
+            save_to_mat="testing.mat",
+            latitude_header="invalid whitespace")
+
+
+@pytest.mark.parametrize("invalid_input, error_output",
+                         invalid_non_str_options)
+def test_saveCenterlineMAT_longitudeHeaderTypeInvalidTypes(
+        invalid_input, error_output):
+    with pytest.raises(
+            ValueError,
+            match=re.escape(
+                f"[longitude_header]: Must be a str, current type = '{error_output}'"
+            )):
+        centerline_width.saveCenterlineMAT(river_object=river_class_example,
+                                           save_to_mat="testing.mat",
+                                           longitude_header=invalid_input)
+
 
 def test_saveCenterlineMAT_longitudeHeaderTypeInvalidAlphanumeric():
-	with pytest.raises(ValueError, match=re.escape("[longitude_header]: Column names cannot contain any whitespace or non-alphanumeric characters, currently = 'invalid whitespace'")):
-		centerline_width.saveCenterlineMAT(river_object=river_class_example,
-											save_to_mat="testing.mat",
-											longitude_header="invalid whitespace")
-
-@pytest.mark.parametrize("invalid_input, error_output", invalid_non_str_options)
-def test_saveCenterlineMAT_centerlineTypeInvalidTypes(invalid_input, error_output):
-	with pytest.raises(ValueError, match=re.escape(f"[centerline_type]: Must be a str, current type = '{error_output}'")):
-		centerline_width.saveCenterlineMAT(river_object=river_class_example,
-											save_to_mat="testing.mat",
-											centerline_type=invalid_input)
+    with pytest.raises(
+            ValueError,
+            match=re.escape(
+                "[longitude_header]: Column names cannot contain any whitespace or non-alphanumeric characters, currently = 'invalid whitespace'"
+            )):
+        centerline_width.saveCenterlineMAT(
+            river_object=river_class_example,
+            save_to_mat="testing.mat",
+            longitude_header="invalid whitespace")
+
+
+@pytest.mark.parametrize("invalid_input, error_output",
+                         invalid_non_str_options)
+def test_saveCenterlineMAT_centerlineTypeInvalidTypes(invalid_input,
+                                                      error_output):
+    with pytest.raises(
+            ValueError,
+            match=re.escape(
+                f"[centerline_type]: Must be a str, current type = '{error_output}'"
+            )):
+        centerline_width.saveCenterlineMAT(river_object=river_class_example,
+                                           save_to_mat="testing.mat",
+                                           centerline_type=invalid_input)
+
 
 def test_saveCenterlineMAT_centerlineTypeInvalidOptions():
-	with pytest.raises(ValueError, match=re.escape("[centerline_type]: Must be an available option in ['Voronoi', 'Evenly Spaced', 'Smoothed', 'Equal Distance'], current option = 'not valid'")):
-		centerline_width.saveCenterlineMAT(river_object=river_class_example,
-											save_to_mat="testing.mat",
-											centerline_type="not valid")
+    with pytest.raises(
+            ValueError,
+            match=re.escape(
+                "[centerline_type]: Must be an available option in ['Voronoi', 'Evenly Spaced', 'Smoothed', 'Equal Distance'], current option = 'not valid'"
+            )):
+        centerline_width.saveCenterlineMAT(river_object=river_class_example,
+                                           save_to_mat="testing.mat",
+                                           centerline_type="not valid")
+
 
 def test_saveCenterlineMAT_coordinateUnitInvalidOption():
-	with pytest.raises(ValueError, match=re.escape("[coordinate_unit]: Must be an available option in ['Decimal Degrees', 'Relative Distance'], current option = 'Invalid Option'")):
-		centerline_width.saveCenterlineMAT(river_object=river_class_example,
-										save_to_mat="testing.mat",
-										coordinate_unit="Invalid Option")
-
-@pytest.mark.parametrize("invalid_input, error_output", invalid_non_str_options)
-def test_saveCenterlineMAT_coordinateUnitInvalidTypes(invalid_input, error_output):
-	with pytest.raises(ValueError, match=re.escape(f"[coordinate_unit]: Must be a str, current type = '{error_output}'")):
-		centerline_width.saveCenterlineMAT(river_object=river_class_example,
-										save_to_mat="testing.mat",
-										coordinate_unit=invalid_input)
+    with pytest.raises(
+            ValueError,
+            match=re.escape(
+                "[coordinate_unit]: Must be an available option in ['Decimal Degrees', 'Relative Distance'], current option = 'Invalid Option'"
+            )):
+        centerline_width.saveCenterlineMAT(river_object=river_class_example,
+                                           save_to_mat="testing.mat",
+                                           coordinate_unit="Invalid Option")
+
+
+@pytest.mark.parametrize("invalid_input, error_output",
+                         invalid_non_str_options)
+def test_saveCenterlineMAT_coordinateUnitInvalidTypes(invalid_input,
+                                                      error_output):
+    with pytest.raises(
+            ValueError,
+            match=re.escape(
+                f"[coordinate_unit]: Must be a str, current type = '{error_output}'"
+            )):
+        centerline_width.saveCenterlineMAT(river_object=river_class_example,
+                                           save_to_mat="testing.mat",
+                                           coordinate_unit=invalid_input)
```

### Comparing `centerline-width-1.5.0/centerline_width/saveOutput.py` & `centerline-width-1.6.0/centerline_width/saveOutput.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,118 +1,152 @@
-# Built in Python functions
+# Built-in Python functions
 import csv
 import logging
 
-# External Python libraries (installed via pip install)
+# External Python libraries
 import numpy as np
 from scipy.io import savemat
 
 # Internal centerline_width reference to access functions, global variables, and error handling
 import centerline_width
 
 ## Logging set up for .CRITICAL
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.WARNING)
 stream_handler = logging.StreamHandler()
 logger.addHandler(stream_handler)
 
-def saveCenterlineCSV(river_object=None,
-					save_to_csv=None,
-					latitude_header=None,
-					longitude_header=None,
-					centerline_type="Voronoi",
-					coordinate_unit="Decimal Degrees"):
-	# Save Centerline Coordinates generated by Voronoi Diagram to .CSV
-	centerline_width.errorHandlingSaveCenterlineCSV(river_object=river_object,
-													save_to_csv=save_to_csv, 
-													latitude_header=latitude_header,
-													longitude_header=longitude_header,
-													centerline_type=centerline_type,
-													coordinate_unit=coordinate_unit)
-	centerline_type = centerline_type.title()
-	coordinate_unit = coordinate_unit.title()
-
-	if coordinate_unit == "Decimal Degrees":
-		if centerline_type == "Voronoi": centerline_coordinates_by_type = river_object.centerlineVoronoi
-		if centerline_type == "Equal Distance": centerline_coordinates_by_type = river_object.centerlineEqualDistance
-		if centerline_type == "Evenly Spaced": centerline_coordinates_by_type = river_object.centerlineEvenlySpaced
-		if centerline_type == "Smoothed": centerline_coordinates_by_type = river_object.centerlineSmoothed
-	if coordinate_unit == "Relative Distance":
-		if centerline_type == "Voronoi": centerline_coordinates_by_type = river_object.centerlineVoronoiRelative
-		if centerline_type == "Equal Distance": centerline_coordinates_by_type = river_object.centerlineEqualDistanceRelative
-		if centerline_type == "Evenly Spaced": centerline_coordinates_by_type = river_object.centerlineEvenlySpacedRelative
-		if centerline_type == "Smoothed": centerline_coordinates_by_type = river_object.centerlineSmoothedRelative
-
-	if coordinate_unit == "Decimal Degrees":
-		if latitude_header is None:
-			latitude_header = f"{centerline_type} Centerline Latitude (Deg)"
-		if longitude_header is None:
-			longitude_header = f"{centerline_type} Centerline Longitude (Deg)"
-	if coordinate_unit == "Relative Distance":
-		if latitude_header is None:
-			latitude_header = f"{centerline_type} Relative Distance Y (from Latitude) (m)"
-		if longitude_header is None:
-			longitude_header = f"{centerline_type} Relative Distance X (from Longitude) (m)"
-
-	with open(save_to_csv, "w") as csv_file_output:
-		writer = csv.writer(csv_file_output)
-		writer.writerow([latitude_header, longitude_header])
-		if centerline_coordinates_by_type is not None:
-			for latitude_longitude in centerline_coordinates_by_type:
-				writer.writerow([latitude_longitude[1], latitude_longitude[0]])
-		else:
-			logger.warn(f"\nWARNING, no {centerline_type} centerline coordinates found, {save_to_csv} file generated will be empty")
-
-def saveCenterlineMAT(river_object=None,
-					save_to_mat=None,
-					latitude_header=None,
-					longitude_header=None,
-					centerline_type="Voronoi",
-					coordinate_unit="Decimal Degrees"):
-	# Save Centerline Coordinates generated by Voronoi Diagram to .MAT
-	centerline_width.errorHandlingSaveCenterlineMAT(river_object=river_object,
-													save_to_mat=save_to_mat, 
-													latitude_header=latitude_header,
-													longitude_header=longitude_header,
-													centerline_type=centerline_type,
-													coordinate_unit=coordinate_unit)
-	centerline_type = centerline_type.title()
-	coordinate_unit = coordinate_unit.title()
-
-	if coordinate_unit == "Decimal Degrees":
-		if centerline_type == "Voronoi": centerline_coordinates_by_type = river_object.centerlineVoronoi
-		if centerline_type == "Equal Distance": centerline_coordinates_by_type = river_object.centerlineEqualDistance
-		if centerline_type == "Evenly Spaced": centerline_coordinates_by_type = river_object.centerlineEvenlySpaced
-		if centerline_type == "Smoothed": centerline_coordinates_by_type = river_object.centerlineSmoothed
-	if coordinate_unit == "Relative Distance":
-		if centerline_type == "Voronoi": centerline_coordinates_by_type = river_object.centerlineVoronoiRelative
-		if centerline_type == "Equal Distance": centerline_coordinates_by_type = river_object.centerlineEqualDistanceRelative
-		if centerline_type == "Evenly Spaced": centerline_coordinates_by_type = river_object.centerlineEvenlySpacedRelative
-		if centerline_type == "Smoothed": centerline_coordinates_by_type = river_object.centerlineSmoothedRelative
-
-	# .mat files do not allow for spaces or special characters in the header
-	if coordinate_unit == "Decimal Degrees":
-		if latitude_header is None:
-			latitude_header = f"{centerline_type.replace(' ', '_')}_Centerline_Latitude_Deg"
-		if longitude_header is None:
-			longitude_header = f"{centerline_type.replace(' ', '_')}_Centerline_Longitude_Deg"
-	if coordinate_unit == "Relative Distance":
-		if latitude_header is None:
-			latitude_header = f"{centerline_type.replace(' ', '_')}_Relative_Distance_Y_From_Latitude_m"
-		if longitude_header is None:
-			longitude_header = f"{centerline_type.replace(' ', '_')}_Relative_Distance_X_From_Longitude_m"
-
-	latitude_lst = []
-	longtiude_lst = []
-
-	if centerline_coordinates_by_type is not None:
-		for latitude_longitude in centerline_coordinates_by_type:
-			longtiude_lst.append(latitude_longitude[0])
-			latitude_lst.append(latitude_longitude[1])
-	else:
-		logger.warn(f"\nWARNING, no {centerline_type} centerline coordinates found, {save_to_mat} file generated will be empty")
-	
-	# Centerline dictionary of latitude and longtiude centerline coordinates
-	centerline_dict = {latitude_header: np.asarray(latitude_lst), longitude_header: np.asarray(longtiude_lst)}
 
-	# Save to matlab format (.mat)
-	savemat(save_to_mat, mdict=centerline_dict)
+def saveCenterlineCSV(river_object: centerline_width.riverCenterline = None,
+                      save_to_csv: str = None,
+                      latitude_header: str = None,
+                      longitude_header: str = None,
+                      centerline_type: str = "Voronoi",
+                      coordinate_unit: str = "Decimal Degrees") -> None:
+    # Save Centerline Coordinates generated by Voronoi Diagram to .CSV
+
+    centerline_width.errorHandlingSaveCenterlineCSV(
+        river_object=river_object,
+        save_to_csv=save_to_csv,
+        latitude_header=latitude_header,
+        longitude_header=longitude_header,
+        centerline_type=centerline_type,
+        coordinate_unit=coordinate_unit)
+    centerline_type = centerline_type.title()
+    coordinate_unit = coordinate_unit.title()
+
+    # set coordinate type and unit
+    if coordinate_unit == "Decimal Degrees":
+        if centerline_type == "Voronoi":
+            centerline_coordinates_by_type = river_object.centerlineVoronoi
+        if centerline_type == "Equal Distance":
+            centerline_coordinates_by_type = river_object.centerlineEqualDistance
+        if centerline_type == "Evenly Spaced":
+            centerline_coordinates_by_type = river_object.centerlineEvenlySpaced
+        if centerline_type == "Smoothed":
+            centerline_coordinates_by_type = river_object.centerlineSmoothed
+    if coordinate_unit == "Relative Distance":
+        if centerline_type == "Voronoi":
+            centerline_coordinates_by_type = river_object.centerlineVoronoiRelative
+        if centerline_type == "Equal Distance":
+            centerline_coordinates_by_type = river_object.centerlineEqualDistanceRelative
+        if centerline_type == "Evenly Spaced":
+            centerline_coordinates_by_type = river_object.centerlineEvenlySpacedRelative
+        if centerline_type == "Smoothed":
+            centerline_coordinates_by_type = river_object.centerlineSmoothedRelative
+
+    # set default latitude/longitude headers
+    if coordinate_unit == "Decimal Degrees":
+        if latitude_header is None:
+            latitude_header = f"{centerline_type} Centerline Latitude (Deg)"
+        if longitude_header is None:
+            longitude_header = f"{centerline_type} Centerline Longitude (Deg)"
+    if coordinate_unit == "Relative Distance":
+        if latitude_header is None:
+            latitude_header = f"{centerline_type} Relative Distance Y (from Latitude) (m)"
+        if longitude_header is None:
+            longitude_header = f"{centerline_type} Relative Distance X (from Longitude) (m)"
+
+    # save csv output
+    with open(save_to_csv, "w") as csv_file_output:
+        writer = csv.writer(csv_file_output)
+        writer.writerow([latitude_header, longitude_header])
+        if centerline_coordinates_by_type is not None:
+            for latitude_longitude in centerline_coordinates_by_type:
+                writer.writerow([latitude_longitude[1], latitude_longitude[0]])
+        else:
+            logger.warn(
+                f"\nWARNING, no {centerline_type} centerline coordinates found, {save_to_csv} file generated will be empty"
+            )
+
+
+def saveCenterlineMAT(river_object: centerline_width.riverCenterline = None,
+                      save_to_mat: str = None,
+                      latitude_header: str = None,
+                      longitude_header: str = None,
+                      centerline_type: str = "Voronoi",
+                      coordinate_unit: str = "Decimal Degrees") -> None:
+    # Save Centerline Coordinates generated by Voronoi Diagram to .MAT
+
+    centerline_width.errorHandlingSaveCenterlineMAT(
+        river_object=river_object,
+        save_to_mat=save_to_mat,
+        latitude_header=latitude_header,
+        longitude_header=longitude_header,
+        centerline_type=centerline_type,
+        coordinate_unit=coordinate_unit)
+    centerline_type = centerline_type.title()
+    coordinate_unit = coordinate_unit.title()
+
+    # set coordinate type and unit
+    if coordinate_unit == "Decimal Degrees":
+        if centerline_type == "Voronoi":
+            centerline_coordinates_by_type = river_object.centerlineVoronoi
+        if centerline_type == "Equal Distance":
+            centerline_coordinates_by_type = river_object.centerlineEqualDistance
+        if centerline_type == "Evenly Spaced":
+            centerline_coordinates_by_type = river_object.centerlineEvenlySpaced
+        if centerline_type == "Smoothed":
+            centerline_coordinates_by_type = river_object.centerlineSmoothed
+    if coordinate_unit == "Relative Distance":
+        if centerline_type == "Voronoi":
+            centerline_coordinates_by_type = river_object.centerlineVoronoiRelative
+        if centerline_type == "Equal Distance":
+            centerline_coordinates_by_type = river_object.centerlineEqualDistanceRelative
+        if centerline_type == "Evenly Spaced":
+            centerline_coordinates_by_type = river_object.centerlineEvenlySpacedRelative
+        if centerline_type == "Smoothed":
+            centerline_coordinates_by_type = river_object.centerlineSmoothedRelative
+
+    # .mat files do not allow for spaces or special characters in the header
+    # convert spaces/special characters to underscores
+    if coordinate_unit == "Decimal Degrees":
+        if latitude_header is None:
+            latitude_header = f"{centerline_type.replace(' ', '_')}_Centerline_Latitude_Deg"
+        if longitude_header is None:
+            longitude_header = f"{centerline_type.replace(' ', '_')}_Centerline_Longitude_Deg"
+    if coordinate_unit == "Relative Distance":
+        if latitude_header is None:
+            latitude_header = f"{centerline_type.replace(' ', '_')}_Relative_Distance_Y_From_Latitude_m"
+        if longitude_header is None:
+            longitude_header = f"{centerline_type.replace(' ', '_')}_Relative_Distance_X_From_Longitude_m"
+
+    latitude_lst = []
+    longtiude_lst = []
+
+    if centerline_coordinates_by_type is not None:
+        for latitude_longitude in centerline_coordinates_by_type:
+            longtiude_lst.append(latitude_longitude[0])
+            latitude_lst.append(latitude_longitude[1])
+    else:
+        logger.warn(
+            f"\nWARNING, no {centerline_type} centerline coordinates found, {save_to_mat} file generated will be empty"
+        )
+
+    # Centerline dictionary of latitude and longtiude centerline coordinates
+    centerline_dict = {
+        latitude_header: np.asarray(latitude_lst),
+        longitude_header: np.asarray(longtiude_lst)
+    }
+
+    # Save to matlab format (.mat)
+    savemat(save_to_mat, mdict=centerline_dict)
```

### Comparing `centerline-width-1.5.0/centerline_width.egg-info/PKG-INFO` & `centerline-width-1.6.0/centerline_width.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,56 +1,59 @@
 Metadata-Version: 2.1
 Name: centerline-width
-Version: 1.5.0
+Version: 1.6.0
 Summary: A Python package to find the centerline and width of rivers based on the latitude and longitude of the right and left bank
 Home-page: https://github.com/cyschneck/centerline-width
-Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v1.5.0.tar.gz
+Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v1.6.0.tar.gz
 Author: Una Schneck (unaschneck), Cora Schneck (cyschneck)
 License: MIT
 Keywords: geophysics,python,voronoi,networkx,centerline,centerline-extraction,centerline-detection,rivers,river-bank-length,river-bank,limnology,hydrology,fluvial,geomorphology
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: geopy>=2.3.0
-Requires-Dist: haversine>=2.8.0
-Requires-Dist: matplotlib>=3.1.0
-Requires-Dist: networkx>=3.0
-Requires-Dist: numpy>=1.24.1
-Requires-Dist: pandas>=1.3.5
-Requires-Dist: pykml>=0.2.0
-Requires-Dist: pyproj>=3.4.1
-Requires-Dist: pytest>=7.2.2
-Requires-Dist: scipy>=1.10.1
-Requires-Dist: shapely>=2.0.1
+Requires-Dist: geopy
+Requires-Dist: haversine
+Requires-Dist: matplotlib
+Requires-Dist: networkx
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: pykml
+Requires-Dist: pyproj
+Requires-Dist: pytest
+Requires-Dist: scipy
+Requires-Dist: shapely
 
 # Centerline-Width
  <p align="center">
   <img src="https://raw.githubusercontent.com/cyschneck/centerline-width/main/assets/centerline_logo.jpg" />
 </p>
 
 ![PyPi](https://img.shields.io/pypi/v/centerline-width)
 ![license](https://img.shields.io/github/license/cyschneck/centerline-width)
+[![repo-status](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 [![NSF-2141064](https://img.shields.io/badge/NSF-2141064-blue)](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2141064&HistoricalAwards=false)
 ![PyPi-Versions](https://img.shields.io/pypi/pyversions/centerline-width)
 [![pytests](https://github.com/cyschneck/centerline-width/actions/workflows/pytests.yml/badge.svg)](https://github.com/cyschneck/centerline-width/actions/workflows/pytests.yml)
+[![pre-commit](https://github.com/cyschneck/centerline-width/actions/workflows/pre-commit.yml/badge.svg)](https://github.com/cyschneck/centerline-width/actions/workflows/pre-commit.yml)
+[![codecov](https://codecov.io/gh/cyschneck/centerline-width/graph/badge.svg?token=V6Z2DC37MT)](https://codecov.io/gh/cyschneck/centerline-width)
 
 Find the centerline and width of rivers based on the latitude and longitude positions from the right and left bank 
 
 * **Convert raw data from Google Earth Pro to CSV**
 	* extractPointsToTextFile()
 	* convertColumnsToCSV()
 * **Find centerline and width of river**
@@ -58,16 +61,18 @@
 	* plotCenterlineWidth()
 	* riverWidthFromCenterline()
 	* centerlineVoronoi
 	* centerlineEqualDistance 
 	* centerlineEvenlySpaced
 	* centerlineSmoothed
 	* centerlineLength
+* **Return river features**
 	* rightBankLength
 	* leftBankLength
+	* riverArea
 * **Export centerline to .CSV and .MAT files**
 	* saveCenterlineCSV()
 	* saveCenterlineMAT()
 
 | River Outlined in Google Earth Pro | Generated Centerline for the Riverbank |
 | ------------- | ------------- |
 | ![river_google_earth+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_example_google_earth.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_example.png) |
@@ -172,26 +177,26 @@
 ```
 
 ### Converted Text File to CSV
 
 Convert a text file with coordinates for a left and right bank's latitude and longitude to a csv file with columns for the left bank latitude (llat), left bank longitude (llon), right bank latitude (rlat), right bank longitude (rlon)
 
 ```
-convertColumnsToCSV(text_file=None, flipBankDirection=False)
+convertColumnsToCSV(text_file=None, flip_direction=False)
 ```
 * **[REQUIRED]** text_file (string): File location of the text file to convert
-* [OPTIONAL] flipBankDirection (boolean): If the latitude/longitude of the banks are generated in reverse order, flip the final values so left/right bank are in order
+* [OPTIONAL] flip_direction (boolean): If the latitude/longitude of the banks are generated in reverse order, flip the final values so left/right bank are in order
 
 Scripts expects data as a list of point for left and right banks:
 - Header: llat, llon, rlat, rlon
 
 ```python
 import centerline_width
 centerline_width.convertColumnsToCSV(text_file="data/river_coords.txt",
-				flipBankDirection=True)
+				flip_direction=True)
 ```
 Converts text file:
 ```
      llat       llon      rlat       rlon
 30.037581 -92.868569 30.037441 -92.867476
 30.037613 -92.868549 30.037448 -92.867474
 30.037648 -92.868546 30.037482 -92.867449
@@ -223,15 +228,15 @@
 ```
 * **[REQUIRED]** csv_data (string): File location of the text file to convert
 * [OPTIONAL] optional_cutoff (int): Include only the first x number of the data to chart (useful for debugging)
 * [OPTIONAL] interpolate_data (boolean): Interpolate between existing data by adding additional points
 * [OPTIONAL] interpolate_n (int): Number of additional points to add between existing data, defaults to 5 (note: larger numbers will take exponentially longer to run, recommends less than 15)
 * [OPTIONAL] interpolate_n_centerpoints (int): Number of points used to interpolate the Voronoi centerline, defaults to the the length of the data frame (df_len)
 * [OPTIONAL] equal_distance (int): Equal distance between points (in meters) used to interpolate the Voronoi centerline, defaults 10 meters
-* [OPTIONAL] ellipsoid (string): Ellipsoid definition of Earth to provide size and shape for built-in functions to convert degrees to meters, options include (is sensitive to case): ["GRS80", "airy", "bessel", "clrk66", "intl", "WGS60", "WGS66", "WGS72", "WGS84", "sphere"] for more details: ["Built-in ellipsoid defintions"](https://proj.org/en/9.2/usage/ellipsoids.html#built-in-ellipsoid-definitions), defaults to "WGS84"
+* [OPTIONAL] ellipsoid (string): Ellipsoid definition of Earth to provide size and shape for built-in functions to convert degrees to meters, options include (is sensitive to case): ["GRS80", "airy", "bessel", "clrk66", "intl", "WGS60", "WGS66", "WGS72", "WGS84", "sphere"] for more details: ["Built-in ellipsoid definitions"](https://proj.org/en/9.2/usage/ellipsoids.html#built-in-ellipsoid-definitions), defaults to "WGS84"
 
 **Equal Distance - Equal linear distance between points**
 
 `equal_distance` will generate points along the centerline that are an equal linear distance from one another in meters. When `equal_distance=5` each point will be 5 meters apart
 
 | equal_distance=5 | equal_distance=20 |
 | ------------- | ------------- |
@@ -254,14 +259,15 @@
 * centerlineVoronoi (list of tuples): List of the latitude and longitude coordinates of the centerline generated by Voronoi diagrams
 * centerlineEqualDistance (list of tuples): List of the latitude and longitude coordinates of the centerline generated by equal distances between coordinates from the Voronoi diagrams
 * centerlineEvenlySpaced (list of tuples): List of the latitude and longitude coordinates of the centerline generated by evenly spacing out points generated by the Voronoi diagrams
 * centerlineSmoothed (list of tuples): List of the latitude and longitude coordinates of the centerline generated by smoothing out the evenly spaced-out points generated by the Voronoi diagrams
 * centerlineLength (float): Length of the centerline of the river (in km)
 * rightBankLength (float): Length of the right bank of the river (in km)
 * leftBankLength (float): Length of the left bank of the river (in km)
+* riverArea (float): Area contained within river bank polygon (in km^2)
 * centerlineVoronoiRelative (list of tuples): List of the relative distance coordinates of the centerline generated by Voronoi diagrams
 * centerlineEqualDistanceRelative (list of tuples): List of the relative distance coordinates of the centerline generated by equal distances between coordinates from the Voronoi diagrams
 * centerlineEvenlySpacedRelative (list of tuples): List of the relative distance coordinates of the centerline generated by evenly spacing out points generated by the Voronoi diagrams
 * centerlineSmoothedRelative (list of tuples): List of the relative distance coordinates of the centerline generated by smoothing out the evenly spaced out points generated by the Voronoi diagrams
 
 **Object (class) additional attributes:**
 
@@ -407,14 +413,27 @@
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
 river_centerline_length = river_object.centerlineLength
 ```
 The length of the river centerline returns `215.34700589636674` km
 
+### Area of River
+Return the area contained within the polygon generated the left and right bank latitude/longitudes
+```
+river_object.riverArea
+```
+Area returned in kilometers^2
+```python
+import centerline_width
+river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
+river_area = river_object.riverArea
+```
+The area of the river returns `334.0398585246558` km^2
+
 ## Plot Centerline in Matplotlib
 Plot the centerline created from a list of right and left banks
 
 ```
 plotCenterline(centerline_type="Voronoi",
 		marker_type="line",
 		centerline_color="black",
@@ -429,28 +448,93 @@
 ```
 * [OPTIONAL] centerline_type (string): Centerline type graph within river (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
 * [OPTIONAL] marker_type (string): Graph type (not case-sensitive), options: ["Line", "Scatter"], defaults to "Line"
 * [OPTIONAL] centerline_color (string): Color of centerline coordinates on graph (not case-sensitive), options: [matplotlib named colors](https://matplotlib.org/stable/gallery/color/named_colors.html), defaults to "black"
 * [OPTIONAL] dark_mode (bool): Change plot to a black ground (and override if `centerline_color="black"` to `centerline_color="white"`), defaults to False
 * [OPTIONAL] equal_axis (bool): Set x/y axes in plot to be equal, defaults to False
 * [OPTIONAL] display_all_possible_paths (boolean): Display all possible paths, not just the centerline (useful for debugging), defaults to False
-* [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False"
+* [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False, Interpolated = True/False"
 * [OPTIONAL] save_plot_name (string): Save the plot with a given name and location
 * [OPTIONAL] display_voronoi (boolean): Overlay Voronoi diagram used to generate centerline, defaults to False
 * [OPTIONAL] show_plot (boolean): display and open plots (plt.show() in Matplotlib), defaults to True
 * [OPTIONAL] coordinate_unit (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longitude) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degrees"
 
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
 river_object.plotCenterline()
 ```
-Output:
 ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_centerline.png)
 
+**centerline_type**
+
+Display different centerline types in plot ("Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"), but defaults to "Voronoi"
+
+| centerline_type="Voronoi" | centerline_type="Smoothed" |
+| ------------- | ------------- |
+| ![centerline_type_voronoi+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_centerline.png) | ![centerline_type_equal_distance+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_centerline_type_smoothed.png) |
+
+**marker_type**
+
+Display centerline plot as either line or scatter
+
+| marker_type="Line" | marker_type="Scatter" |
+| ------------- | ------------- |
+| ![marker_type_line+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_centerline.png)  | ![marker_type_scatter+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_marker_type_scatter.png) |
+
+**centerline_color**
+
+Change the color of the centerline, defaults to black
+
+| centerline_color="black" | centerline_color="palegreen" |
+| ------------- | ------------- |
+| ![centerline_color_black+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_centerline.png) | ![centerline_color_purple+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_centerline_color.png) |
+
+**dark_mode**
+
+dark_mode will change the default Matplotlib background black and swap `centerline_color` from default black to white
+
+| dark_mode=False | dark_mode=True |
+| ------------- | ------------- |
+| ![dark_mode_false+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_centerline.png) | ![dark_mode_true+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_dark_mode.png) |
+
+**equal_axis**
+
+equal_axis will set the x and y axis of the plot to be equal
+
+| equal_axis=False | equal_axis=True |
+| ------------- | ------------- |
+| ![river_not_equal+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_equal_axis_false.png) | ![river_equal+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_equal_axis_true.png)|
+
+**display_all_possible_paths**
+
+Display all possible paths generated by Voronoi edge ridges, defaults to False
+
+| display_all_possible_paths=False | display_all_possible_paths=True |
+| ------------- | ------------- |
+| ![display_all_possible_paths_false+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_centerline.png) | ![display_all_possible_paths_true+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_display_all_possible_paths_true.png) |
+
+**display_voronoi**
+
+Overlay Voronoi diagram used to generate centerline, defaults to False
+
+| display_voronoi=False | display_voronoi=True |
+| ------------- | ------------- |
+| ![display_voronoi_default+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_display_voronoi_false.png) | ![display_voronoi_true+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_display_voronoi_true.png) |
+
+
+**coordinate_unit**
+
+Plot as either "Decimal Degrees" and "Relative Distance". defaults to "Decimal Degrees" 
+
+| coordinate_unit="Decimal Degrees" | coordinate_unit="Relative Distance" |
+| ------------- | ------------- |
+| ![coordinate_unit_dd+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_centerline.png) | ![coordinate_unit_rd+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coordinate_unit_rd.png) |
+
+
 ## Plot Centerline Width Lines in Matplotlib
 ### Plot the Centerline Width Lines
 Plot the width of the river based on the centerline
 
 ```
 plotCenterlineWidth(plot_title=None, 
 		save_plot_name=None, 
@@ -461,27 +545,35 @@
 		flag_intersections=True,
 		remove_intersections=False,
 		dark_mode=False,
 		equal_axis=False,
 		show_plot=True,
 		coordinate_unit="Decimal Degrees")
 ```
-* [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False"
+* [OPTIONAL] plot_title (string): Change plot title, defaults to "River Width Coordinates: Valid Centerline = True/False, Valid Polygon = True/False, Centerline made of <interpolate_n_centerpoints> Fixed Points, width lines generated every <transect_span_distance> points, Interpolated = True/False"
 * [OPTIONAL] save_plot_name (string): Save the plot with a given name and location
 * [OPTIONAL] display_true_centerline (boolean): Display generated true centerline based on Voronoi diagrams, defaults to True
 * [OPTIONAL] transect_span_distance (int): Number n points around a center point to determine the slope (increase to decrease the impact of sudden changes), defaults to 3, must be greater than 1 (since the slope is found from the difference in position between two points)
 * [OPTIONAL] transect_slope (str): Determine how the width lines are generated, either by averaging all slopes "Average" or directly from the first to last point in the span distance as "Direct", defaults to "Average"
 * [OPTIONAL] apply_smoothing (boolean): Apply a B-spline smoothing to centerline
 * [OPTIONAL] flag_intersections (boolean): Display intersecting width lines as red in graph, defaults to True
 * [OPTIONAL] remove_intersections (boolean): Remove intersecting lines (but maintain the most width lines as possible) and only return non-intersecting width lines, defaults to False
 * [OPTIONAL] dark_mode (bool): Change plot to a black ground (and override if `centerline_color="black"` to `centerline_color="white"`), defaults to False
 * [OPTIONAL] equal_axis (bool): Set x/y axes in plot to be equal, defaults to False
 * [OPTIONAL] show_plot (boolean): display and open plots (plt.show() in Matplotlib), defaults to True
 * [OPTIONAL] coordinate_unit (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longitude) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degrees"
 
+
+```python
+import centerline_width
+river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
+river_object.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
+```
+![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width.png)
+
 **display_true_centerline**
 
 The width lines are generated from the evenly spaced coordinate (by default) or with the smoothed coordinates (when `apply_smoothing=True`), but display_true_centerline will overlay the Voronoi centerline on top of the plot
 
 | display_true_centerline=True | display_true_centerline=False |
 | ------------- | ------------- |
 | ![river_with_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_with_centerline.png) | ![river_no_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_without_centerline.png) |
@@ -527,15 +619,15 @@
 
 | remove_intersections=False | remove_intersections=True |
 | ------------- | ------------- |
 | ![river_keep+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_keep_intersections.png) | ![river_remove+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_remove_intersections.png)|
 
 **dark_mode**
 
-dark_mode will change the default Matplotlib background black and swap `centerline_color` from black to white
+dark_mode will change the default Matplotlib background black and swap `centerline_color` from default black to white
 
 | dark_mode=False | dark_mode=True |
 | ------------- | ------------- |
 | ![river_white+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_dark_mode_false.png) | ![river_black+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_dark_mode_true.png)|
 
 **equal_axis**
 
@@ -545,25 +637,18 @@
 | ------------- | ------------- |
 | ![river_not_equal+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_not_equal_default_ax.png) | ![river_equal+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_equal_ax.png)|
 
 **coordinate_unit**
 
 Two options for measuring and displaying coordinates. The two options are "Decimal Degrees" and "Relative Distance". "Decimal Degrees" is the default option that uses the original data coordinate system with latitude/longitude. "Relative Distance" changes the coordinates of each point to be the distance (in meters) from the first point on the left bank
 
-| coordinate_unit="Decimal Degrees" | remove_intersections="Relative Distance" |
+| coordinate_unit="Decimal Degrees" | coordinate_unit="Relative Distance" |
 | ------------- | ------------- |
 | ![dd_coords+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_decimal_degrees.png) | ![rd_coords+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_relative_distance.png)|
 
-```python
-import centerline_width
-river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
-river_object.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
-```
-![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width.png)
-
 ### Return Width of River
 Return the width of the river at each (evenly spaced or smoothed) with coordinates where width line intersects either the centerline, `(Centerline Longitude, Centerline Latitude) : width`, or riverbanks, `((Right Bank Longitude, Right Bank Latitude), (Left Bank Longitude, Left Bank Latitude)) : width` in kilometers
 
 ```
 riverWidthFromCenterline(transect_span_distance=3,
 			transect_slope="Average",
 			apply_smoothing=True,
@@ -595,137 +680,162 @@
 Note: it is best practice to plot the centerline and width with same arguments in `plotCenterlineWidth()` to ensure that the results when `save_to_csv=True` are as expected
 
 ## Documentation and Algorithm to Determine Centerline
 
 The centerline is defined by the greatest distance from the right and left bank, created from a Voronoi Diagram. The remaining paths within the river are filtered through Dijkstra's algorithm to find the shortest path that is the centerline
 
 ### Right and Left bank points are plotted (X-Axis for Latitude, Y-Axis for Longitude)
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example1.png)
+![algorithm_step1+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/algorithm_step1.png)
 
 ### Generate a polygon to encapsulate the river between the right and left banks to define in and outside of river
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example2.png)
+![algorithm_step2+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/algorithm_step2.png)
 
 ### Generate a Voronoi diagram based on the points along the riverbanks
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example3.png)
+![algorithm_step3+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/algorithm_step3.png)
 
 ### Display Voronoi ridge vertices that lie within the polygon (within the riverbanks)
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example4.png)
+Filter out any point pairs that only have one connection to filter out the short dead end paths
 
-### Filter out any point pairs that only have one connection to filter out the short dead end paths
 With the vertices removed, it is possible to form multiple unconnected graphs within the polygon. The largest subgraph is assumed to contain the centerline and the other subgraphs are filtered out
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example6.png)
+![algorithm_step4+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/algorithm_step4.png)
+
+### Define Top and Bottom of Polygon
+The top of the river is defined as the last plotted points in the data, while the bottom of the river is the first plotted points
+![algorithm_step5+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/algorithm_step5.png)
 
 ### Find the starting and ending node based on distance from the top and bottom of polygon
 The starting/ending node is defined by the vertex closest to the top/bottom of the polygon along the longest path
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example7.png)
+![algorithm_step6+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/algorithm_step6.png)
 
 ### Find the shortest path from the starting node to the ending node ([Dijkstra's Algorithm](https://networkx.org/documentation/stable/reference/algorithms/generated/networkx.algorithms.shortest_paths.generic.shortest_path.html#networkx.algorithms.shortest_paths.generic.shortest_path))
 | Points on Riverbank | NetworkX Graph of Points on Riverbank |
 | ------------- | ------------- |
-| ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example10.png) | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example9.png) |
+| ![algorithm_step7+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/algorithm_step7.png) | ![algorithm_step8+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/algorithm_step8.png) |
 
 ### Display the centerline found by connecting the starting/ending node with the shortest path
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example8.png)
+![algorithm_step9+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/algorithm_step9.png)
 
 This is an attempt at a more robust algorithm working from raw data to ensure that all dead ends are removed, and no gaps exist in the centerline
 
 Points that only have one connection are removed, but limiting the number of connections for a point to just two will create gaps. The Voronoi vertices connect to other vertex values, but some connect to more and some only connect to one other point. Removing additional values will create gaps, so this is avoided in this code by not applying additional filters.
 
 **All vertices:**
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example4.png)
+![algorithm_step4+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/algorithm_step4.png)
 
 **Vertices that have at least two connections (that would create gaps):**
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example5.png)
+![algorithm_step10+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/algorithm_step10.png)
 
 ## Debugging, Error Handling, and Edge Cases
 ### Wide Start/End of River
 If the data starts or ends with a large width, it is possible for the starting/ending nodes to end up in the wrong position
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_example3.png)
+![invalid_too_wide+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_too_wide.png)
 Currently, the starting node is determined by the closest node on the path to the top of the bank (in green) and the ending node is determined by the closest node on the path to the bottom of the bank (in red) that sits along the longest path
 
 ### Invalid Polygon
 A polygon is formed to encapsulate the river with the given data (to determine the inside and outside of the river). The top and bottom are connected by a straight line from the start/end of the available data. As a result, it is possible for this straight line to overlap and create an invalid polygon.
 
 A polygon is invalid if it overlaps within itself:
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_example1.png)
+![invalid_minor_polygon+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_minor_polygon.png)
 In this example, the polygon is invalid, but with such a small overlap it is still able to find a valid path
 
 With limited data, the polygon will overlap more dramatically and will struggle to find a valid centerline:
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_example4.png)
+![invalid_major_polygon+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_major_polygon.png)
 
 ### Invalid Centerline
-If the data is too small, a centerline and its coordinates cannot not be found (since only a single Voronoi vertex exists within the polygon and after dead ends are filtered)
+If the data is too small, a centerline and its coordinates cannot be found (since only a single Voronoi vertex exists within the polygon and after dead ends are filtered)
 
-`CRITICAL ERROR, Polygon too short for the Voronoi diagram generated (no starting node found), unable to plot centerline. Set displayVoronoi=True to view vertices. Can typically be fixed by adding more data to expand range.`
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_example2.png)
+`CRITICAL ERROR, Polygon too short for the Voronoi diagram generated (no starting node found), unable to plot centerline. Set display_voronoi=True to view vertices. Can typically be fixed by adding more data to expand range`
+![invalid_too_small+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_too_small.png)
 Can be fixed by expanding the data until the polygon is large enough to contain at least two different vertex points
 
-### Invalid Top and Bottom Bank Positions (flipBankDirection = True)
-Error: `WARNING: Invalid Polygon Due to Flipped Banks, fix recommendation: rerun convertColumnsToCSV() and set flipBankDirection=True (or reset to default 'False' if currently set to flipBankDirection=True)`
+### Invalid Top and Bottom Bank Positions (flip_direction = True)
+Error: `WARNING: Invalid Polygon Due to Flipped Banks, fix recommendation: rerun convertColumnsToCSV() and set flip_direction=True (or reset to default 'False' if currently set to flip_direction=True)`
 
 If the data for the left and right riverbanks are generated in reverse order, they will be read in the incorrect order and the graph will find the invalid top and bottom of the bank
 
 If the latitude/longitude of the banks are generated in reverse order, flip the final values so left/right bank are in order
 
-This can be fixed by using the flipBankDirection optional argument `centerline_width.convertColumnsToCSV(text_file="data_example.txt", flipBankDirection=True)`
-![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/flipDirection_example.png)
+This can be fixed by using the flip_direction optional argument `centerline_width.convertColumnsToCSV(text_file="data_example.txt", flip_direction=True)`
+![invalid_flipped_banks+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_flipped_banks.png)
 
 ### Invalid Smoothed Centerline
 The smoothed centerline (`river_object.centerlineSmoothed`) can end up lying outside the river if the centerline data points are sparse in a narrow river. If more than two points in the smoothed centerline lie outside the river, a warning will be thrown
 
 Example Error: `WARNING: Partially invalid smoothed centerline due to sparse centerline data (6 points lie outside the polygon), fix recommendation: rerun riverCenterline to create river object with interpolate_n_centerpoints set to 62+`
 
-By default, `interpolate_n_centerpoints` is set to None and not additional points will be added between the existing points along the centerline. By adding additional points between the existing centerline, the smoothed centerline can be fixed to stay within the polygon. This fix is set by creating a river object, `centerline_width.riverCenterline`, with `interpolate_n_centerpoints=65` (with the recommended 62+) to fix for centerline coordinates that lie outside the polygon
+By default, `interpolate_n_centerpoints` is set to None and no additional points will be added between the existing points along the centerline. By adding additional points between the existing centerline, the smoothed centerline can be fixed to stay within the polygon. This fix is set by creating a river object, `centerline_width.riverCenterline`, with `interpolate_n_centerpoints=65` (with the recommended 62+) to fix for centerline coordinates that lie outside the polygon
 
 `interpolate_n_centerpoints = None` does not interpolate data points, so the size will be set to the number of fixed points when creating the evenly spaced coordinates (equal to the size of the data frame)
 
 | interpolate_n_centerpoints = None | interpolate_n_centerpoints = 65 |
 | ------------- | ------------- |
 | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_smoothed_centerline.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_smoothed_centerline_fixed.png) |
 
 For very narrow rivers, this problem can become extreme and pronounced
 ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_smoothed_centerline_extreme.png)
 
 By increasing the interpolation between the centerline points, the smoothed centerlines will be forced within the polygon and reduce the number of points outside of the polygon. By default, this warning will be thrown if more than 2 points are outside of polygon, so as long as more than 2 points lie outside the polygon, the warning will recommend doubling the amount of centerline points
 
-### Fix Gaps and Jagged Centerlines
+### Fixing Gaps and Jagged Centerlines
 Gaps formed can cause part of the centerline to be skipped due to sparse data. As a result, the start and end of the centerline can skip parts at the beginning or end of a river
 ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps_short_path.png)
 Set river object created by `centerline_width.riverCenterline` to `interpolate_data=True` to fix for jagged edges or gaps formed by the interaction of sparse data and narrow banks
 ```python
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", interpolate_data=True)
 ```
 | interpolate_data = False | interpolate_data = True |
 | ------------- | ------------- |
 | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_true_no_gaps.png) |
 | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps_2.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_true_no_gaps_2.png) |
 
 The number of additional points added by interpolating can be adjusted with `interpolate_n`, but defaults to add 5 additional points between values
 
-## Development Environment
+## Development Environment	
 To run or test against `centerline-width` github repo/fork, a development environment can be created via conda/miniconda
 
 First, [install Miniconda](https://docs.conda.io/projects/miniconda/en/latest/miniconda-install.html)
 
 Then, using the existing `environment.yml`, a new conda environment can be create to run/test scripts against
 
 ```
 conda env create --file environment.yml
 ```
 Once the environment has been built, activate the environment:
 ```
 conda activate centerline_width
 ```
+Set up pre-commit hooks to ensure standard code formatting and spelling:
+```
+pre-commit install
+```
+Pre-commit hooks can be manually run before commits:
+```
+pre-commit run --all-files
+```
 To run existing and new tests from the root directory:
 ```
 python -m pytest
 ```
+## Beta :test_tube: Features
+These features are not included in pip install because they are still experimental and being tested/debugged. For more information and getting them up and running, contact cyschneck@gmail.com or ugschneck@gmail.com or post a question as a [Github Issue](https://github.com/cyschneck/centerline-width/issues)
+
+- Calculate sinuosity of river, in total and in equal parts
+
+- Calculate the dominant meander wavelength amd its variance
+
+- Calculate the asymmetry of the meanders 
+
+- Calculate the dominant submeander and supermeander scales
+
+- Extract elevation/slope from river profiles (.kml files)
+
+- Overlay plots with images via geopandas
 
 ## Citations
-Originally a Python implementation of [R-Code CMGO](https://github.com/AntoniusGolly/cmgo) (Golly et al. 2017) but has been extensively expanded:
+Originally a Python implementation of [R-Code CMGO](https://github.com/AntoniusGolly/cmgo) (Golly et al. 2017) but has since been extensively expanded:
 
 >Golly, A. and Turowski, J. M.: Deriving principal channel metrics from bank and long-profile geometry with the R package cmgo, Earth Surf. Dynam., 5, 557-570, https://doi.org/10.5194/esurf-5-557-2017, 2017.
 
  <p align="center">
   <img src="https://user-images.githubusercontent.com/22159116/222872092-e0b579cc-4f84-4f49-aa53-397785fb9bf2.png" />
   <img src="https://user-images.githubusercontent.com/22159116/222872119-7c485ee2-4ffd-413a-9e4f-b043b122d2bb.png" />
   <img src="https://user-images.githubusercontent.com/22159116/222872019-12931138-9e10-4e51-aa1e-552e72d09af0.png" />
@@ -733,15 +843,15 @@
 
 ## Acknowledging Software 
 Please acknowledge the use of this software in any publications:
 
 ```
 "River centerline/width extraction software was provided by C. Y. Schneck and U. G. Schneck, and is available at URL: https://github.com/cyschneck/centerline-width."
 ```
-Please send a copy of such publications to: cyschneck@gmail.com and ugschneck@gmail.com
+We are interested in expanding this software based on river needs, so please send a copy of such publications to: cyschneck@gmail.com and ugschneck@gmail.com
 
 
 This material is based upon work supported by the National Science Foundation Graduate Fellowship under Grant No. 2141064. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the authors and do not necessarily reflect the views of the National Science Foundation.
 
-## Bug and Feature Request
+## Bug :bug: and Feature Requests
 
 Submit a bug fix, question, or feature request as a [Github Issue](https://github.com/cyschneck/centerline-width/issues) or to ugschneck@gmail.com/cyschneck@gmail.com
```

### Comparing `centerline-width-1.5.0/centerline_width.egg-info/SOURCES.txt` & `centerline-width-1.6.0/centerline_width.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -4,21 +4,29 @@
 centerline_width/__init__.py
 centerline_width/centerline.py
 centerline_width/error_handling.py
 centerline_width/getCoordinatesKML.py
 centerline_width/plotDiagrams.py
 centerline_width/preprocessing.py
 centerline_width/relativeDistance.py
+centerline_width/riverAsymmetry.py
 centerline_width/riverCenterlineClass.py
+centerline_width/riverFeatures.py
 centerline_width/saveOutput.py
+centerline_width/width.py
 centerline_width.egg-info/PKG-INFO
 centerline_width.egg-info/SOURCES.txt
 centerline_width.egg-info/dependency_links.txt
 centerline_width.egg-info/requires.txt
 centerline_width.egg-info/top_level.txt
-centerline_width/pytests/test_centerline.py
-centerline_width/pytests/test_getCoordinatesKML.py
-centerline_width/pytests/test_plotDiagrams.py
-centerline_width/pytests/test_preprocessing.py
-centerline_width/pytests/test_riverCenterlineClass.py
-centerline_width/pytests/test_saveOutput.py
-centerline_width/pytests/test_verifyOutput.py
+centerline_width/pytests/test_errorGetCoordinatesKML.py
+centerline_width/pytests/test_errorPlotDiagrams.py
+centerline_width/pytests/test_errorPreprocessing.py
+centerline_width/pytests/test_errorRiverCenterlineClass.py
+centerline_width/pytests/test_errorSaveOutput.py
+centerline_width/pytests/test_errorWidth.py
+centerline_width/pytests/test_verifyGetCoordinatesKML.py
+centerline_width/pytests/test_verifyPlotDiagrams.py
+centerline_width/pytests/test_verifyPreprocessing.py
+centerline_width/pytests/test_verifyRiverFeatures.py
+centerline_width/pytests/test_verifySaveOutput.py
+centerline_width/pytests/test_verifyWidth.py
```

