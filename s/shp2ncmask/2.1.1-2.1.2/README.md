# Comparing `tmp/shp2ncmask-2.1.1.tar.gz` & `tmp/shp2ncmask-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shp2ncmask-2.1.1.tar", last modified: Wed May  3 08:18:47 2023, max compression
+gzip compressed data, was "shp2ncmask-2.1.2.tar", last modified: Thu Apr 25 13:47:08 2024, max compression
```

## Comparing `shp2ncmask-2.1.1.tar` & `shp2ncmask-2.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-03 08:18:47.375907 shp2ncmask-2.1.1/
--rw-r--r--   0 yrobin     (501) staff       (20)    35149 2022-03-15 07:47:17.000000 shp2ncmask-2.1.1/LICENSE
--rw-r--r--   0 yrobin     (501) staff       (20)     1134 2023-05-03 08:18:47.375774 shp2ncmask-2.1.1/PKG-INFO
--rw-r--r--   0 yrobin     (501) staff       (20)     3238 2023-03-24 15:56:34.000000 shp2ncmask-2.1.1/README.md
-drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-03 08:18:47.374209 shp2ncmask-2.1.1/Shp2ncmask/
--rw-r--r--   0 yrobin     (501) staff       (20)     3798 2023-03-24 15:56:34.000000 shp2ncmask-2.1.1/Shp2ncmask/__S2NParams.py
--rw-r--r--   0 yrobin     (501) staff       (20)     2706 2022-12-15 07:08:11.000000 shp2ncmask-2.1.1/Shp2ncmask/__curses_doc.py
--rw-r--r--   0 yrobin     (501) staff       (20)     5736 2023-03-24 15:56:34.000000 shp2ncmask-2.1.1/Shp2ncmask/__doc.py
--rw-r--r--   0 yrobin     (501) staff       (20)      940 2023-03-24 15:47:30.000000 shp2ncmask-2.1.1/Shp2ncmask/__exceptions.py
--rw-r--r--   0 yrobin     (501) staff       (20)     6099 2023-04-12 08:26:21.000000 shp2ncmask-2.1.1/Shp2ncmask/__exec.py
--rw-r--r--   0 yrobin     (501) staff       (20)     5244 2023-04-09 07:52:46.000000 shp2ncmask-2.1.1/Shp2ncmask/__grid.py
--rw-r--r--   0 yrobin     (501) staff       (20)      995 2023-03-24 15:47:30.000000 shp2ncmask-2.1.1/Shp2ncmask/__init__.py
--rw-r--r--   0 yrobin     (501) staff       (20)     2510 2023-03-24 15:56:34.000000 shp2ncmask-2.1.1/Shp2ncmask/__inputs.py
--rw-r--r--   0 yrobin     (501) staff       (20)     2525 2023-03-24 15:47:30.000000 shp2ncmask-2.1.1/Shp2ncmask/__logs.py
--rw-r--r--   0 yrobin     (501) staff       (20)     8237 2023-04-09 07:52:46.000000 shp2ncmask-2.1.1/Shp2ncmask/__mask.py
--rw-r--r--   0 yrobin     (501) staff       (20)     4854 2023-03-24 15:47:30.000000 shp2ncmask-2.1.1/Shp2ncmask/__plot.py
--rw-r--r--   0 yrobin     (501) staff       (20)     1504 2023-04-12 08:26:21.000000 shp2ncmask-2.1.1/Shp2ncmask/__release.py
-drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-03 08:18:47.374446 shp2ncmask-2.1.1/scripts/
--rwxr-xr-x   0 yrobin     (501) staff       (20)      948 2023-03-24 15:47:30.000000 shp2ncmask-2.1.1/scripts/shp2ncmask
--rw-r--r--   0 yrobin     (501) staff       (20)       38 2023-05-03 08:18:47.375953 shp2ncmask-2.1.1/setup.cfg
--rw-r--r--   0 yrobin     (501) staff       (20)     2347 2023-03-24 15:47:30.000000 shp2ncmask-2.1.1/setup.py
-drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-03 08:18:47.375575 shp2ncmask-2.1.1/shp2ncmask.egg-info/
--rw-r--r--   0 yrobin     (501) staff       (20)     1134 2023-05-03 08:18:47.000000 shp2ncmask-2.1.1/shp2ncmask.egg-info/PKG-INFO
--rw-r--r--   0 yrobin     (501) staff       (20)      456 2023-05-03 08:18:47.000000 shp2ncmask-2.1.1/shp2ncmask.egg-info/SOURCES.txt
--rw-r--r--   0 yrobin     (501) staff       (20)        1 2023-05-03 08:18:47.000000 shp2ncmask-2.1.1/shp2ncmask.egg-info/dependency_links.txt
--rw-r--r--   0 yrobin     (501) staff       (20)       11 2023-05-03 08:18:47.000000 shp2ncmask-2.1.1/shp2ncmask.egg-info/top_level.txt
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2024-04-25 13:47:08.527148 shp2ncmask-2.1.2/
+-rw-r--r--   0 yrobin     (501) staff       (20)    35149 2022-03-15 07:47:17.000000 shp2ncmask-2.1.2/LICENSE
+-rw-r--r--   0 yrobin     (501) staff       (20)     1134 2024-04-25 13:47:08.526931 shp2ncmask-2.1.2/PKG-INFO
+-rw-r--r--   0 yrobin     (501) staff       (20)     3238 2023-03-24 15:56:34.000000 shp2ncmask-2.1.2/README.md
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2024-04-25 13:47:08.525543 shp2ncmask-2.1.2/Shp2ncmask/
+-rw-r--r--   0 yrobin     (501) staff       (20)     3798 2023-03-24 15:56:34.000000 shp2ncmask-2.1.2/Shp2ncmask/__S2NParams.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     2706 2022-12-15 07:08:11.000000 shp2ncmask-2.1.2/Shp2ncmask/__curses_doc.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     5736 2023-03-24 15:56:34.000000 shp2ncmask-2.1.2/Shp2ncmask/__doc.py
+-rw-r--r--   0 yrobin     (501) staff       (20)      940 2023-03-24 15:47:30.000000 shp2ncmask-2.1.2/Shp2ncmask/__exceptions.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     6099 2023-04-12 08:26:21.000000 shp2ncmask-2.1.2/Shp2ncmask/__exec.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     5244 2023-04-09 07:52:46.000000 shp2ncmask-2.1.2/Shp2ncmask/__grid.py
+-rw-r--r--   0 yrobin     (501) staff       (20)      995 2023-03-24 15:47:30.000000 shp2ncmask-2.1.2/Shp2ncmask/__init__.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     2510 2023-03-24 15:56:34.000000 shp2ncmask-2.1.2/Shp2ncmask/__inputs.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     2525 2023-03-24 15:47:30.000000 shp2ncmask-2.1.2/Shp2ncmask/__logs.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     8222 2023-05-22 14:23:29.000000 shp2ncmask-2.1.2/Shp2ncmask/__mask.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     4854 2023-03-24 15:47:30.000000 shp2ncmask-2.1.2/Shp2ncmask/__plot.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     1504 2023-05-22 14:23:34.000000 shp2ncmask-2.1.2/Shp2ncmask/__release.py
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2024-04-25 13:47:08.525699 shp2ncmask-2.1.2/scripts/
+-rwxr-xr-x   0 yrobin     (501) staff       (20)      948 2023-03-24 15:47:30.000000 shp2ncmask-2.1.2/scripts/shp2ncmask
+-rw-r--r--   0 yrobin     (501) staff       (20)       38 2024-04-25 13:47:08.527193 shp2ncmask-2.1.2/setup.cfg
+-rw-r--r--   0 yrobin     (501) staff       (20)     2347 2023-03-24 15:47:30.000000 shp2ncmask-2.1.2/setup.py
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2024-04-25 13:47:08.526685 shp2ncmask-2.1.2/shp2ncmask.egg-info/
+-rw-r--r--   0 yrobin     (501) staff       (20)     1134 2024-04-25 13:47:08.000000 shp2ncmask-2.1.2/shp2ncmask.egg-info/PKG-INFO
+-rw-r--r--   0 yrobin     (501) staff       (20)      456 2024-04-25 13:47:08.000000 shp2ncmask-2.1.2/shp2ncmask.egg-info/SOURCES.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)        1 2024-04-25 13:47:08.000000 shp2ncmask-2.1.2/shp2ncmask.egg-info/dependency_links.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)       11 2024-04-25 13:47:08.000000 shp2ncmask-2.1.2/shp2ncmask.egg-info/top_level.txt
```

### Comparing `shp2ncmask-2.1.1/LICENSE` & `shp2ncmask-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shp2ncmask-2.1.1/PKG-INFO` & `shp2ncmask-2.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shp2ncmask
-Version: 2.1.1
+Version: 2.1.2
 Summary: shp2ncmask is a tools to transform a shapefile in a netcdf file
 Home-page: https://github.com/yrobink/Shp2ncmask
 Author: Yoann Robin
 Author-email: yoann.robin.k@gmail.com
 License: GNU-GPL3
 Keywords: shapefile,netcdf,mask
 Platform: linux
```

### Comparing `shp2ncmask-2.1.1/README.md` & `shp2ncmask-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `shp2ncmask-2.1.1/Shp2ncmask/__S2NParams.py` & `shp2ncmask-2.1.2/Shp2ncmask/__S2NParams.py`

 * *Files identical despite different names*

### Comparing `shp2ncmask-2.1.1/Shp2ncmask/__curses_doc.py` & `shp2ncmask-2.1.2/Shp2ncmask/__curses_doc.py`

 * *Files identical despite different names*

### Comparing `shp2ncmask-2.1.1/Shp2ncmask/__doc.py` & `shp2ncmask-2.1.2/Shp2ncmask/__doc.py`

 * *Files identical despite different names*

### Comparing `shp2ncmask-2.1.1/Shp2ncmask/__exceptions.py` & `shp2ncmask-2.1.2/Shp2ncmask/__exceptions.py`

 * *Files identical despite different names*

### Comparing `shp2ncmask-2.1.1/Shp2ncmask/__exec.py` & `shp2ncmask-2.1.2/Shp2ncmask/__exec.py`

 * *Files identical despite different names*

### Comparing `shp2ncmask-2.1.1/Shp2ncmask/__grid.py` & `shp2ncmask-2.1.2/Shp2ncmask/__grid.py`

 * *Files identical despite different names*

### Comparing `shp2ncmask-2.1.1/Shp2ncmask/__init__.py` & `shp2ncmask-2.1.2/Shp2ncmask/__init__.py`

 * *Files identical despite different names*

### Comparing `shp2ncmask-2.1.1/Shp2ncmask/__inputs.py` & `shp2ncmask-2.1.2/Shp2ncmask/__inputs.py`

 * *Files identical despite different names*

### Comparing `shp2ncmask-2.1.1/Shp2ncmask/__logs.py` & `shp2ncmask-2.1.2/Shp2ncmask/__logs.py`

 * *Files identical despite different names*

### Comparing `shp2ncmask-2.1.1/Shp2ncmask/__mask.py` & `shp2ncmask-2.1.2/Shp2ncmask/__mask.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 	
 	cf_params = crs.to_cf()
 	
 	name = cf_params["grid_mapping_name"]
 	if "lambert" in name and "conformal" in name:
 		name = "Lambert_Conformal"
 		attrs = {}
-		for key in ["grid_mapping_name","standard_parallel","longitude_of_central_meridian","latitude_of_projection_origin","false_easting","false_northing","scale_factor"]:
+		for key in ["grid_mapping_name","standard_parallel","longitude_of_central_meridian","latitude_of_projection_origin","false_easting","false_northing"]:
 			attrs[key] = str(cf_params.get(key))
 	
 	return name,attrs
 ##}}}
 
 @log_start_end(logger)
 def save_netcdf( mask , grid ):##{{{
```

### Comparing `shp2ncmask-2.1.1/Shp2ncmask/__plot.py` & `shp2ncmask-2.1.2/Shp2ncmask/__plot.py`

 * *Files identical despite different names*

### Comparing `shp2ncmask-2.1.1/Shp2ncmask/__release.py` & `shp2ncmask-2.1.2/Shp2ncmask/__release.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 ##############
 ## Packages ##
 ##############
 
 
 version_major = 2
 version_minor = 1
-version_patch = 1
+version_patch = 2
 version_extra = ""
 version       = "{}.{}.{}{}".format(version_major,version_minor,version_patch,version_extra)
 
 
 ##
 
 name = "shp2ncmask"
```

### Comparing `shp2ncmask-2.1.1/scripts/shp2ncmask` & `shp2ncmask-2.1.2/scripts/shp2ncmask`

 * *Files identical despite different names*

### Comparing `shp2ncmask-2.1.1/setup.py` & `shp2ncmask-2.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `shp2ncmask-2.1.1/shp2ncmask.egg-info/PKG-INFO` & `shp2ncmask-2.1.2/shp2ncmask.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shp2ncmask
-Version: 2.1.1
+Version: 2.1.2
 Summary: shp2ncmask is a tools to transform a shapefile in a netcdf file
 Home-page: https://github.com/yrobink/Shp2ncmask
 Author: Yoann Robin
 Author-email: yoann.robin.k@gmail.com
 License: GNU-GPL3
 Keywords: shapefile,netcdf,mask
 Platform: linux
```

