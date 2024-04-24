# Comparing `tmp/ziptimezone-1.0.2.tar.gz` & `tmp/ziptimezone-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ziptimezone-1.0.2.tar", max compression
+gzip compressed data, was "ziptimezone-1.0.3.tar", max compression
```

## Comparing `ziptimezone-1.0.2.tar` & `ziptimezone-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        2 2024-04-20 11:29:25.216037 ziptimezone-1.0.2/LICENSE
--rw-r--r--   0        0        0      846 2024-04-23 11:23:29.690490 ziptimezone-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1810 2024-04-23 11:23:18.002282 ziptimezone-1.0.2/README.rst
--rw-r--r--   0        0        0     1183 2024-04-23 11:02:12.525191 ziptimezone-1.0.2/ziptimezone/__init__.py
--rw-r--r--   0        0        0     1968 2024-04-21 13:54:36.748759 ziptimezone-1.0.2/ziptimezone/batch_processor.py
--rw-r--r--   0        0        0     1801 2024-04-21 13:54:36.748759 ziptimezone-1.0.2/ziptimezone/core.py
--rw-r--r--   0        0        0     2780 2024-04-21 13:54:36.749759 ziptimezone-1.0.2/ziptimezone/data_manager.py
--rw-r--r--   0        0        0     1101 2024-04-21 13:54:36.749759 ziptimezone-1.0.2/ziptimezone/geocode.py
--rw-r--r--   0        0        0     1645 2024-04-21 13:54:36.749759 ziptimezone-1.0.2/ziptimezone/globals.py
--rw-r--r--   0        0        0     1874 2024-04-21 13:54:36.749759 ziptimezone-1.0.2/ziptimezone/mappings.py
--rw-r--r--   0        0        0     2483 1970-01-01 00:00:00.000000 ziptimezone-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0        2 2024-04-20 11:29:25.216037 ziptimezone-1.0.3/LICENSE
+-rw-r--r--   0        0        0      846 2024-04-24 22:13:20.879302 ziptimezone-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1818 2024-04-24 12:24:15.572521 ziptimezone-1.0.3/README.rst
+-rw-r--r--   0        0        0     1334 2024-04-24 12:20:02.715620 ziptimezone-1.0.3/ziptimezone/__init__.py
+-rw-r--r--   0        0        0     3598 2024-04-24 12:28:21.581939 ziptimezone-1.0.3/ziptimezone/batch_processor.py
+-rw-r--r--   0        0        0     1801 2024-04-21 13:54:36.748759 ziptimezone-1.0.3/ziptimezone/core.py
+-rw-r--r--   0        0        0     2780 2024-04-21 13:54:36.749759 ziptimezone-1.0.3/ziptimezone/data_manager.py
+-rw-r--r--   0        0        0     1101 2024-04-21 13:54:36.749759 ziptimezone-1.0.3/ziptimezone/geocode.py
+-rw-r--r--   0        0        0     1645 2024-04-21 13:54:36.749759 ziptimezone-1.0.3/ziptimezone/globals.py
+-rw-r--r--   0        0        0     1874 2024-04-21 13:54:36.749759 ziptimezone-1.0.3/ziptimezone/mappings.py
+-rw-r--r--   0        0        0     2490 1970-01-01 00:00:00.000000 ziptimezone-1.0.3/PKG-INFO
```

### Comparing `ziptimezone-1.0.2/pyproject.toml` & `ziptimezone-1.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ziptimezone"
-version = "1.0.2"
+version = "1.0.3"
 description = "A package to convert ZIP codes to time zones and get geographic coordinates."
 readme = "README.rst"
 authors = ["Manjunath Bettadapura <manjunathbettadapura412@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.9, <4.0"
```

### Comparing `ziptimezone-1.0.2/README.rst` & `ziptimezone-1.0.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,16 @@
 .. code-block:: python
 
     import ziptimezone as zpt
 
     # returns a tuple (42.377, -71.1256)
     zpt.get_lat_long_for_zip('02138')
 
-    # returns 'Eastern' the timezone has been reduced to the more popular zones for United States Regions
+    # returns 'Eastern' the timezone has been reduced to the more popular zones 
+    # for United States Regions
     zpt.get_timezone_by_zip('02138') 
 
     # returns a dictionary, {'02138': 'Eastern', '85260': 'Mountain'}
     zpt.get_timezone_for_many_zips(['02138', '85260']) 
 
 
 For more refer to the `Documentation <https://ziptimezone.readthedocs.io/en/latest/>`__.
```

### Comparing `ziptimezone-1.0.2/ziptimezone/__init__.py` & `ziptimezone-1.0.3/ziptimezone/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,31 +3,33 @@
 and retrieving geographic coordinates (latitude and longitude) based on ZIP codes.
 
 This package includes:
 - `get_timezone_by_zip`: Function to convert a ZIP code into a timezone name.
 - `map_timezone_to_region`: Function to map detailed timezone names to broader, 
   more general region names (e.g., 'Eastern', 'Central').
 - `get_lat_long`: Function to retrieve the latitude and longitude for a given ZIP code.
+- 'get_timezone_for_many_zips' and 'get_lat_long_for_many_zips' for multiple zip codes
 
 Example usage:
 from ziptimezone import get_timezone_by_zip, get_lat_long_for_zip
 
 # Get the timezone of a ZIP code
 timezone = get_timezone_by_zip('85260')
 
 # Get the latitude and longitude of a ZIP code
 latitude, longitude = get_lat_long_for_zip('02138')
 """
 
 from .core import get_timezone_by_zip, get_lat_long_for_zip
 from .data_manager import refresh_data_if_needed
-from .batch_processor import get_timezone_for_many_zips
+from .batch_processor import get_timezone_for_many_zips, get_lat_long_for_many_zips
 
 ##from .mappings import map_timezone_to_region
 # from .geocode import get_lat_long_for_zip
 
 __all__ = [
     "get_timezone_by_zip",
     "refresh_data_if_needed",
     "get_lat_long_for_zip",
     "get_timezone_for_many_zips",
+    "get_lat_long_for_many_zips",
 ]
```

### Comparing `ziptimezone-1.0.2/ziptimezone/batch_processor.py` & `ziptimezone-1.0.3/ziptimezone/batch_processor.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import concurrent.futures
-from .core import get_timezone_by_zip
+from .core import get_timezone_by_zip, get_lat_long_for_zip
 import logging
 
+##
 # Setup basic logging
 logging.basicConfig(
     level=logging.INFO, format="%(asctime)s - %(levelname)s - %(message)s"
 )
 
 
 def process_zip_code(zip_code):
@@ -14,14 +15,23 @@
     try:
         return zip_code, get_timezone_by_zip(zip_code)
     except Exception as e:
         logging.error(f"Error processing ZIP code {zip_code}: {str(e)}")
         return zip_code, None
 
 
+def process_zip_code_lat_long(zip_code):
+    """Helper function to process a single ZIP code for latitude and longitude."""
+    try:
+        return zip_code, get_lat_long_for_zip(zip_code)
+    except Exception as e:
+        logging.error(f"Error processing ZIP code {zip_code}: {str(e)}")
+        return zip_code, (None, None)
+
+
 def get_timezone_for_many_zips(zip_codes, max_workers=None):
     """
     Processes a list of ZIP codes in parallel using ThreadPoolExecutor,
     retrieving time zones for each. The number of workers can be customized based on the machine.
 
     Args:
         zip_codes (list of str): A list of ZIP codes.
@@ -45,7 +55,39 @@
             try:
                 _, timezone = future.result()
                 results[zip_code] = timezone
             except Exception as exc:
                 logging.error(f"Exception for ZIP code {zip_code}: {exc}")
                 results[zip_code] = None
     return results
+
+
+def get_lat_long_for_many_zips(zip_codes, max_workers=None):
+    """
+    Processes a list of ZIP codes in parallel using ThreadPoolExecutor,
+    retrieving latitudes and longitudes for each. The number of workers can be customized.
+
+    Args:
+        zip_codes (list of str): A list of ZIP codes.
+        max_workers (int, optional): Maximum number of threads to use for parallel processing.
+
+    Returns:
+        dict: A dictionary mapping ZIP codes to their corresponding latitudes and longitudes.
+    """
+    if max_workers is None:
+        max_workers = os.cpu_count() * 2
+
+    results = {}
+    with concurrent.futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
+        future_to_zip = {
+            executor.submit(process_zip_code_lat_long, zip_code): zip_code
+            for zip_code in zip_codes
+        }
+        for future in concurrent.futures.as_completed(future_to_zip):
+            zip_code = future_to_zip[future]
+            try:
+                _, lat_long = future.result()
+                results[zip_code] = lat_long
+            except Exception as exc:
+                logging.error(f"Exception for ZIP code {zip_code}: {exc}")
+                results[zip_code] = (None, None)
+    return results
```

### Comparing `ziptimezone-1.0.2/ziptimezone/core.py` & `ziptimezone-1.0.3/ziptimezone/core.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-1.0.2/ziptimezone/data_manager.py` & `ziptimezone-1.0.3/ziptimezone/data_manager.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-1.0.2/ziptimezone/geocode.py` & `ziptimezone-1.0.3/ziptimezone/geocode.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-1.0.2/ziptimezone/globals.py` & `ziptimezone-1.0.3/ziptimezone/globals.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-1.0.2/ziptimezone/mappings.py` & `ziptimezone-1.0.3/ziptimezone/mappings.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-1.0.2/PKG-INFO` & `ziptimezone-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ziptimezone
-Version: 1.0.2
+Version: 1.0.3
 Summary: A package to convert ZIP codes to time zones and get geographic coordinates.
 License: MIT
 Author: Manjunath Bettadapura
 Author-email: manjunathbettadapura412@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -59,15 +59,16 @@
 .. code-block:: python
 
     import ziptimezone as zpt
 
     # returns a tuple (42.377, -71.1256)
     zpt.get_lat_long_for_zip('02138')
 
-    # returns 'Eastern' the timezone has been reduced to the more popular zones for United States Regions
+    # returns 'Eastern' the timezone has been reduced to the more popular zones 
+    # for United States Regions
     zpt.get_timezone_by_zip('02138') 
 
     # returns a dictionary, {'02138': 'Eastern', '85260': 'Mountain'}
     zpt.get_timezone_for_many_zips(['02138', '85260']) 
 
 
 For more refer to the `Documentation <https://ziptimezone.readthedocs.io/en/latest/>`__.
```

