# Comparing `tmp/gmaps_avoid_swiss-0.1.7.tar.gz` & `tmp/gmaps_avoid_swiss-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmaps_avoid_swiss-0.1.7.tar", last modified: Sun Apr 21 04:19:19 2024, max compression
+gzip compressed data, was "gmaps_avoid_swiss-0.1.8.tar", last modified: Thu Apr 25 11:47:51 2024, max compression
```

## Comparing `gmaps_avoid_swiss-0.1.7.tar` & `gmaps_avoid_swiss-0.1.8.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-21 04:19:19.805290 gmaps_avoid_swiss-0.1.7/
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      162 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.7/AUTHORS.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     3851 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.7/CONTRIBUTING.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       89 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.7/HISTORY.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1072 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.7/LICENSE
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      262 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.7/MANIFEST.in
--rw-r--r--   0 gregor    (1000) gregor    (1000)     2896 2024-04-21 04:19:19.805290 gmaps_avoid_swiss-0.1.7/PKG-INFO
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1865 2024-04-21 03:33:06.000000 gmaps_avoid_swiss-0.1.7/README.rst
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-21 04:19:19.801290 gmaps_avoid_swiss-0.1.7/docs/
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      618 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.7/docs/Makefile
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-21 04:19:19.801290 gmaps_avoid_swiss-0.1.7/docs/_build/
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-21 04:19:19.801290 gmaps_avoid_swiss-0.1.7/docs/_build/html/
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-21 04:19:19.801290 gmaps_avoid_swiss-0.1.7/docs/_build/html/_static/
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      286 2024-04-19 14:44:04.000000 gmaps_avoid_swiss-0.1.7/docs/_build/html/_static/file.png
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       90 2024-04-19 14:44:04.000000 gmaps_avoid_swiss-0.1.7/docs/_build/html/_static/minus.png
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       90 2024-04-19 14:44:04.000000 gmaps_avoid_swiss-0.1.7/docs/_build/html/_static/plus.png
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       28 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.7/docs/authors.rst
--rwxrwxr-x   0 gregor    (1000) gregor    (1000)     4934 2024-04-21 02:19:23.000000 gmaps_avoid_swiss-0.1.7/docs/conf.py
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       33 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.7/docs/contributing.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1152 2024-04-20 18:21:23.000000 gmaps_avoid_swiss-0.1.7/docs/geos.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      881 2024-04-21 03:31:07.000000 gmaps_avoid_swiss-0.1.7/docs/gmaps_avoid_swiss.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       28 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.7/docs/history.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      343 2024-04-21 02:19:08.000000 gmaps_avoid_swiss-0.1.7/docs/index.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1211 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.7/docs/installation.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      815 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.7/docs/make.bat
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       88 2024-04-21 03:31:07.000000 gmaps_avoid_swiss-0.1.7/docs/modules.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       27 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.7/docs/readme.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1237 2024-04-21 02:18:54.000000 gmaps_avoid_swiss-0.1.7/docs/usage.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1449 2024-04-21 04:19:08.000000 gmaps_avoid_swiss-0.1.7/pyproject.toml
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       38 2024-04-21 04:19:19.805290 gmaps_avoid_swiss-0.1.7/setup.cfg
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1081 2024-04-21 04:19:08.000000 gmaps_avoid_swiss-0.1.7/setup.py
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-21 04:19:19.801290 gmaps_avoid_swiss-0.1.7/src/
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-21 04:19:19.801290 gmaps_avoid_swiss-0.1.7/src/gmaps_avoid_swiss/
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      307 2024-04-21 04:19:08.000000 gmaps_avoid_swiss-0.1.7/src/gmaps_avoid_swiss/__init__.py
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      674 2024-04-20 16:51:38.000000 gmaps_avoid_swiss-0.1.7/src/gmaps_avoid_swiss/client.py
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-21 04:19:19.801290 gmaps_avoid_swiss-0.1.7/src/gmaps_avoid_swiss/data/
--rw-rw-r--   0 gregor    (1000) gregor    (1000)    17771 2024-04-20 19:48:38.000000 gmaps_avoid_swiss-0.1.7/src/gmaps_avoid_swiss/data/switzerland.geojson
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     4030 2024-04-21 02:11:49.000000 gmaps_avoid_swiss-0.1.7/src/gmaps_avoid_swiss/geo_check.py
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     7470 2024-04-21 02:11:04.000000 gmaps_avoid_swiss-0.1.7/src/gmaps_avoid_swiss/routes.py
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     2540 2024-04-20 16:57:41.000000 gmaps_avoid_swiss-0.1.7/src/gmaps_avoid_swiss/waypoints.py
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-21 04:19:19.801290 gmaps_avoid_swiss-0.1.7/src/gmaps_avoid_swiss.egg-info/
--rw-r--r--   0 gregor    (1000) gregor    (1000)     2896 2024-04-21 04:19:19.000000 gmaps_avoid_swiss-0.1.7/src/gmaps_avoid_swiss.egg-info/PKG-INFO
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      979 2024-04-21 04:19:19.000000 gmaps_avoid_swiss-0.1.7/src/gmaps_avoid_swiss.egg-info/SOURCES.txt
--rw-rw-r--   0 gregor    (1000) gregor    (1000)        1 2024-04-21 04:19:19.000000 gmaps_avoid_swiss-0.1.7/src/gmaps_avoid_swiss.egg-info/dependency_links.txt
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       76 2024-04-21 04:19:19.000000 gmaps_avoid_swiss-0.1.7/src/gmaps_avoid_swiss.egg-info/requires.txt
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       18 2024-04-21 04:19:19.000000 gmaps_avoid_swiss-0.1.7/src/gmaps_avoid_swiss.egg-info/top_level.txt
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-21 04:19:19.805290 gmaps_avoid_swiss-0.1.7/tests/
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       47 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.7/tests/__init__.py
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1383 2024-04-21 03:10:41.000000 gmaps_avoid_swiss-0.1.7/tests/test_geo_check.py
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1460 2024-04-21 03:00:26.000000 gmaps_avoid_swiss-0.1.7/tests/test_gmaps_avoid_swiss.py
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1550 2024-04-21 03:19:07.000000 gmaps_avoid_swiss-0.1.7/tests/test_routes.py
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1202 2024-04-19 19:57:47.000000 gmaps_avoid_swiss-0.1.7/tests/test_waypoints.py
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-25 11:47:51.735776 gmaps_avoid_swiss-0.1.8/
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      162 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.8/AUTHORS.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     3851 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.8/CONTRIBUTING.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       89 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.8/HISTORY.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1072 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.8/LICENSE
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      262 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.8/MANIFEST.in
+-rw-r--r--   0 gregor    (1000) gregor    (1000)     2875 2024-04-25 11:47:51.735776 gmaps_avoid_swiss-0.1.8/PKG-INFO
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1844 2024-04-22 16:54:22.000000 gmaps_avoid_swiss-0.1.8/README.rst
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-25 11:47:51.731775 gmaps_avoid_swiss-0.1.8/docs/
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      618 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.8/docs/Makefile
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-25 11:47:51.731775 gmaps_avoid_swiss-0.1.8/docs/_build/
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-25 11:47:51.731775 gmaps_avoid_swiss-0.1.8/docs/_build/html/
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-25 11:47:51.735776 gmaps_avoid_swiss-0.1.8/docs/_build/html/_static/
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      286 2024-04-19 14:44:04.000000 gmaps_avoid_swiss-0.1.8/docs/_build/html/_static/file.png
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       90 2024-04-19 14:44:04.000000 gmaps_avoid_swiss-0.1.8/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       90 2024-04-19 14:44:04.000000 gmaps_avoid_swiss-0.1.8/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       28 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.8/docs/authors.rst
+-rwxrwxr-x   0 gregor    (1000) gregor    (1000)     4934 2024-04-21 02:19:23.000000 gmaps_avoid_swiss-0.1.8/docs/conf.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       33 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.8/docs/contributing.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1152 2024-04-20 18:21:23.000000 gmaps_avoid_swiss-0.1.8/docs/geos.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      881 2024-04-22 16:34:26.000000 gmaps_avoid_swiss-0.1.8/docs/gmaps_avoid_swiss.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       28 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.8/docs/history.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      343 2024-04-21 02:19:08.000000 gmaps_avoid_swiss-0.1.8/docs/index.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1211 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.8/docs/installation.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      815 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.8/docs/make.bat
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       88 2024-04-22 16:34:26.000000 gmaps_avoid_swiss-0.1.8/docs/modules.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       27 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.8/docs/readme.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     2453 2024-04-22 17:01:53.000000 gmaps_avoid_swiss-0.1.8/docs/usage.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1449 2024-04-25 11:43:00.000000 gmaps_avoid_swiss-0.1.8/pyproject.toml
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       38 2024-04-25 11:47:51.735776 gmaps_avoid_swiss-0.1.8/setup.cfg
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1081 2024-04-25 11:43:00.000000 gmaps_avoid_swiss-0.1.8/setup.py
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-25 11:47:51.731775 gmaps_avoid_swiss-0.1.8/src/
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-25 11:47:51.735776 gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss/
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      307 2024-04-25 11:43:00.000000 gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss/__init__.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      674 2024-04-20 16:51:38.000000 gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss/client.py
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-25 11:47:51.735776 gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss/data/
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)    17771 2024-04-20 19:48:38.000000 gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss/data/switzerland.geojson
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     4506 2024-04-25 11:42:00.000000 gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss/geo_check.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     7588 2024-04-25 11:39:10.000000 gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss/routes.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     2540 2024-04-20 16:57:41.000000 gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss/waypoints.py
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-25 11:47:51.735776 gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss.egg-info/
+-rw-r--r--   0 gregor    (1000) gregor    (1000)     2875 2024-04-25 11:47:51.000000 gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss.egg-info/PKG-INFO
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      979 2024-04-25 11:47:51.000000 gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss.egg-info/SOURCES.txt
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)        1 2024-04-25 11:47:51.000000 gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss.egg-info/dependency_links.txt
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       76 2024-04-25 11:47:51.000000 gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss.egg-info/requires.txt
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       18 2024-04-25 11:47:51.000000 gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss.egg-info/top_level.txt
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-25 11:47:51.735776 gmaps_avoid_swiss-0.1.8/tests/
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       47 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.8/tests/__init__.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1383 2024-04-21 03:10:41.000000 gmaps_avoid_swiss-0.1.8/tests/test_geo_check.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1460 2024-04-21 03:00:26.000000 gmaps_avoid_swiss-0.1.8/tests/test_gmaps_avoid_swiss.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1550 2024-04-21 03:19:07.000000 gmaps_avoid_swiss-0.1.8/tests/test_routes.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1202 2024-04-19 19:57:47.000000 gmaps_avoid_swiss-0.1.8/tests/test_waypoints.py
```

### Comparing `gmaps_avoid_swiss-0.1.7/CONTRIBUTING.rst` & `gmaps_avoid_swiss-0.1.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.7/LICENSE` & `gmaps_avoid_swiss-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.7/PKG-INFO` & `gmaps_avoid_swiss-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmaps_avoid_swiss
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Python package that customizes Google Maps routing to avoid Swiss routes unless the origin, destination, or waypoints include locations within Switzerland.
 Home-page: https://github.com/xbencat/gmaps_avoid_swiss
 Author: Gregor Bencat
 Author-email: Gregor Bencat <bencat.gregor@gmail.com>
 Maintainer-email: Gregor Bencat <bencat.gregor@gmail.com>
 License: MIT license
 Project-URL: bugs, https://github.com/xbencat/gmaps_avoid_swiss/issues
@@ -45,15 +45,15 @@
 * Documentation: https://gmaps-avoid-swiss.readthedocs.io.
 
 
 Dependencies
 ____________
 
 This package requires the GEOS library as it utilizes Shapely for geographic operations.
-For installation instructions and more details, please refer to our `Geos <geos.html>`_ page for more details.
+For installation instructions and more details, please refer to `Geos <geos.html>`_ page.
 
 
 Features
 --------
 
 * Calculates duration, transit time, and encoded path from origin to destination
 * Avoids routing through Switzerland by dynamically selecting alternative cities
```

### Comparing `gmaps_avoid_swiss-0.1.7/README.rst` & `gmaps_avoid_swiss-0.1.8/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 * Documentation: https://gmaps-avoid-swiss.readthedocs.io.
 
 
 Dependencies
 ____________
 
 This package requires the GEOS library as it utilizes Shapely for geographic operations.
-For installation instructions and more details, please refer to our `Geos <geos.html>`_ page for more details.
+For installation instructions and more details, please refer to `Geos <geos.html>`_ page.
 
 
 Features
 --------
 
 * Calculates duration, transit time, and encoded path from origin to destination
 * Avoids routing through Switzerland by dynamically selecting alternative cities
```

### Comparing `gmaps_avoid_swiss-0.1.7/docs/Makefile` & `gmaps_avoid_swiss-0.1.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.7/docs/conf.py` & `gmaps_avoid_swiss-0.1.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.7/docs/geos.rst` & `gmaps_avoid_swiss-0.1.8/docs/geos.rst`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.7/docs/gmaps_avoid_swiss.rst` & `gmaps_avoid_swiss-0.1.8/docs/gmaps_avoid_swiss.rst`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.7/docs/installation.rst` & `gmaps_avoid_swiss-0.1.8/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.7/docs/make.bat` & `gmaps_avoid_swiss-0.1.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.7/pyproject.toml` & `gmaps_avoid_swiss-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gmaps_avoid_swiss"
-version = "0.1.7"
+version = "0.1.8"
 description = "A Python package that customizes Google Maps routing to avoid Swiss routes unless the origin, destination, or waypoints include locations within Switzerland."
 readme = "README.rst"
 authors = [
   {name = "Gregor Bencat", email = "bencat.gregor@gmail.com"}
 ]
 maintainers = [
   {name = "Gregor Bencat", email = "bencat.gregor@gmail.com"}
```

### Comparing `gmaps_avoid_swiss-0.1.7/setup.py` & `gmaps_avoid_swiss-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gmaps_avoid_swiss',
-    version='0.1.7',
+    version='0.1.8',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     url='https://github.com/xbencat/gmaps_avoid_swiss',
     license='MIT',
     author='Gregor Bencat',
     author_email='bencat.gregor@gmail.com',
     description='A Python package that customizes Google Maps routing to avoid Swiss routes.',
```

### Comparing `gmaps_avoid_swiss-0.1.7/src/gmaps_avoid_swiss/client.py` & `gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss/client.py`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.7/src/gmaps_avoid_swiss/data/switzerland.geojson` & `gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss/data/switzerland.geojson`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.7/src/gmaps_avoid_swiss/geo_check.py` & `gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss/geo_check.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import json
 from importlib import resources
+from typing import Union
 
 from google.maps.routing_v2 import Polyline
 from polyline import polyline
+from shapely import MultiLineString
 from shapely.geometry import shape, Point, Polygon, LineString
 
 
 class GeographicChecker:
     INNSBRUCK = {"lat": 47.2692, "lng": 11.4041}
     LION = {"lat": 45.7640, "lng": 4.8357}
     BEAUNE = {"lat": 47.0260, "lng": 4.8400}
@@ -51,26 +53,32 @@
         except Exception as e:
             raise ValueError(f"Error decoding polyline: {str(e)}")
 
         route_linestring = LineString(points)
 
         return self.swiss_polygon.intersection(route_linestring)
 
-    def sort_cities_by_distance(self, intersection: LineString):
+    def sort_cities_by_distance(self, intersection: Union[LineString, MultiLineString]):
         """
         Sort the cities based on their total distance to the start and end points of the intersection with Switzerland.
 
         :param intersection: The LineString representing the intersection of the route with Switzerland.
         :type intersection: LineString
         """
 
         self.cities.clear()
 
-        start = Point(intersection.coords[0])  # start of intersection
-        end = Point(intersection.coords[-1])  # end of intersection
+        if isinstance(intersection, LineString):
+            start = Point(intersection.coords[0])  # Start of LineString
+            end = Point(intersection.coords[-1])  # End of LineString
+        elif isinstance(intersection, MultiLineString):
+            start = Point(intersection.geoms[0].coords[0])  # First point of the first LineString
+            end = Point(intersection.geoms[-1].coords[-1])  # Last point of the last LineString
+        else:
+            raise TypeError("Unsupported geometry type for intersection")
 
         for city in [self.INNSBRUCK, self.LION, self.BEAUNE]:
             city_point = Point(city['lng'], city['lat'])
 
             distance_to_start = start.distance(city_point)
             distance_from_end = end.distance(city_point)
             total_distance = distance_to_start + distance_from_end
```

### Comparing `gmaps_avoid_swiss-0.1.7/src/gmaps_avoid_swiss/routes.py` & `gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss/routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         self.default_fields = default_fields
 
     def compute_route(self, origin: dict, destination: dict,
                       extra_fields: list = None) -> routing_v2.ComputeRoutesResponse:
         """
         Compute the route from origin to destination with customizable response fields.
         Extends the default fields with any extra fields specified for this particular call.
+        For detailed information on all available extra fields, refer to the corresponding section in the user guide.
 
         :param origin: A dictionary containing the origin location data.
         :type origin: dict
         :param destination: A dictionary containing the destination location data.
         :type destination: dict
         :param extra_fields: Additional fields to include in the response, in addition to default fields.
         :type extra_fields: list, optional
```

### Comparing `gmaps_avoid_swiss-0.1.7/src/gmaps_avoid_swiss/waypoints.py` & `gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss/waypoints.py`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.7/src/gmaps_avoid_swiss.egg-info/PKG-INFO` & `gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmaps-avoid-swiss
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Python package that customizes Google Maps routing to avoid Swiss routes unless the origin, destination, or waypoints include locations within Switzerland.
 Home-page: https://github.com/xbencat/gmaps_avoid_swiss
 Author: Gregor Bencat
 Author-email: Gregor Bencat <bencat.gregor@gmail.com>
 Maintainer-email: Gregor Bencat <bencat.gregor@gmail.com>
 License: MIT license
 Project-URL: bugs, https://github.com/xbencat/gmaps_avoid_swiss/issues
@@ -45,15 +45,15 @@
 * Documentation: https://gmaps-avoid-swiss.readthedocs.io.
 
 
 Dependencies
 ____________
 
 This package requires the GEOS library as it utilizes Shapely for geographic operations.
-For installation instructions and more details, please refer to our `Geos <geos.html>`_ page for more details.
+For installation instructions and more details, please refer to `Geos <geos.html>`_ page.
 
 
 Features
 --------
 
 * Calculates duration, transit time, and encoded path from origin to destination
 * Avoids routing through Switzerland by dynamically selecting alternative cities
```

### Comparing `gmaps_avoid_swiss-0.1.7/src/gmaps_avoid_swiss.egg-info/SOURCES.txt` & `gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.7/tests/test_geo_check.py` & `gmaps_avoid_swiss-0.1.8/tests/test_geo_check.py`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.7/tests/test_gmaps_avoid_swiss.py` & `gmaps_avoid_swiss-0.1.8/tests/test_gmaps_avoid_swiss.py`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.7/tests/test_routes.py` & `gmaps_avoid_swiss-0.1.8/tests/test_routes.py`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.7/tests/test_waypoints.py` & `gmaps_avoid_swiss-0.1.8/tests/test_waypoints.py`

 * *Files identical despite different names*

