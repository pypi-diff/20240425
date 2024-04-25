# Comparing `tmp/icecube-skyreader-1.2.8.tar.gz` & `tmp/icecube-skyreader-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icecube-skyreader-1.2.8.tar", last modified: Tue Nov 14 17:20:40 2023, max compression
+gzip compressed data, was "icecube-skyreader-1.2.9.tar", last modified: Thu Apr 25 12:48:30 2024, max compression
```

## Comparing `icecube-skyreader-1.2.8.tar` & `icecube-skyreader-1.2.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 17:20:40.939898 icecube-skyreader-1.2.8/
--rw-r--r--   0 root         (0) root         (0)     1085 2023-11-14 17:20:37.000000 icecube-skyreader-1.2.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2059 2023-11-14 17:20:40.939898 icecube-skyreader-1.2.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1025 2023-11-14 17:20:37.000000 icecube-skyreader-1.2.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 17:20:40.939898 icecube-skyreader-1.2.8/icecube_skyreader.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2059 2023-11-14 17:20:40.000000 icecube-skyreader-1.2.8/icecube_skyreader.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      412 2023-11-14 17:20:40.000000 icecube-skyreader-1.2.8/icecube_skyreader.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-14 17:20:40.000000 icecube-skyreader-1.2.8/icecube_skyreader.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      164 2023-11-14 17:20:40.000000 icecube-skyreader-1.2.8/icecube_skyreader.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-11-14 17:20:40.000000 icecube-skyreader-1.2.8/icecube_skyreader.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1835 2023-11-14 17:20:40.943898 icecube-skyreader-1.2.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       76 2023-11-14 17:20:37.000000 icecube-skyreader-1.2.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 17:20:40.939898 icecube-skyreader-1.2.8/skyreader/
--rw-r--r--   0 root         (0) root         (0)      740 2023-11-14 17:20:38.000000 icecube-skyreader-1.2.8/skyreader/__init__.py
--rw-r--r--   0 root         (0) root         (0)      915 2023-11-14 17:20:37.000000 icecube-skyreader-1.2.8/skyreader/event_metadata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 17:20:40.939898 icecube-skyreader-1.2.8/skyreader/plot/
--rw-r--r--   0 root         (0) root         (0)       63 2023-11-14 17:20:37.000000 icecube-skyreader-1.2.8/skyreader/plot/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29228 2023-11-14 17:20:37.000000 icecube-skyreader-1.2.8/skyreader/plot/plot.py
--rw-r--r--   0 root         (0) root         (0)     9821 2023-11-14 17:20:37.000000 icecube-skyreader-1.2.8/skyreader/plot/plotting_tools.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-14 17:20:37.000000 icecube-skyreader-1.2.8/skyreader/py.typed
--rw-r--r--   0 root         (0) root         (0)    20253 2023-11-14 17:20:37.000000 icecube-skyreader-1.2.8/skyreader/result.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 12:48:30.757730 icecube-skyreader-1.2.9/
+-rw-r--r--   0 root         (0) root         (0)     1085 2024-04-25 12:48:27.000000 icecube-skyreader-1.2.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2059 2024-04-25 12:48:30.757730 icecube-skyreader-1.2.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-04-25 12:48:27.000000 icecube-skyreader-1.2.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 12:48:30.757730 icecube-skyreader-1.2.9/icecube_skyreader.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2059 2024-04-25 12:48:30.000000 icecube-skyreader-1.2.9/icecube_skyreader.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      412 2024-04-25 12:48:30.000000 icecube-skyreader-1.2.9/icecube_skyreader.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 12:48:30.000000 icecube-skyreader-1.2.9/icecube_skyreader.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      164 2024-04-25 12:48:30.000000 icecube-skyreader-1.2.9/icecube_skyreader.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-25 12:48:30.000000 icecube-skyreader-1.2.9/icecube_skyreader.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1835 2024-04-25 12:48:30.757730 icecube-skyreader-1.2.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       76 2024-04-25 12:48:27.000000 icecube-skyreader-1.2.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 12:48:30.757730 icecube-skyreader-1.2.9/skyreader/
+-rw-r--r--   0 root         (0) root         (0)      740 2024-04-25 12:48:28.000000 icecube-skyreader-1.2.9/skyreader/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      915 2024-04-25 12:48:27.000000 icecube-skyreader-1.2.9/skyreader/event_metadata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 12:48:30.757730 icecube-skyreader-1.2.9/skyreader/plot/
+-rw-r--r--   0 root         (0) root         (0)       63 2024-04-25 12:48:27.000000 icecube-skyreader-1.2.9/skyreader/plot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29228 2024-04-25 12:48:27.000000 icecube-skyreader-1.2.9/skyreader/plot/plot.py
+-rw-r--r--   0 root         (0) root         (0)     9937 2024-04-25 12:48:27.000000 icecube-skyreader-1.2.9/skyreader/plot/plotting_tools.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 12:48:27.000000 icecube-skyreader-1.2.9/skyreader/py.typed
+-rw-r--r--   0 root         (0) root         (0)    20253 2024-04-25 12:48:27.000000 icecube-skyreader-1.2.9/skyreader/result.py
```

### Comparing `icecube-skyreader-1.2.8/LICENSE` & `icecube-skyreader-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-1.2.8/PKG-INFO` & `icecube-skyreader-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icecube-skyreader
-Version: 1.2.8
+Version: 1.2.9
 Summary: An API for Results Produced by SkyDriver & the Skymap Scanner
 Home-page: https://github.com/icecube/skyreader
 Download-URL: https://pypi.org/project/icecube-skyreader/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/icecube/skyreader/issues
```

### Comparing `icecube-skyreader-1.2.8/README.md` & `icecube-skyreader-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-1.2.8/icecube_skyreader.egg-info/PKG-INFO` & `icecube-skyreader-1.2.9/icecube_skyreader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icecube-skyreader
-Version: 1.2.8
+Version: 1.2.9
 Summary: An API for Results Produced by SkyDriver & the Skymap Scanner
 Home-page: https://github.com/icecube/skyreader
 Download-URL: https://pypi.org/project/icecube-skyreader/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/icecube/skyreader/issues
```

### Comparing `icecube-skyreader-1.2.8/setup.cfg` & `icecube-skyreader-1.2.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-1.2.8/skyreader/__init__.py` & `icecube-skyreader-1.2.9/skyreader/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "1.2.8"
+__version__ = "1.2.9"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `icecube-skyreader-1.2.8/skyreader/event_metadata.py` & `icecube-skyreader-1.2.9/skyreader/event_metadata.py`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-1.2.8/skyreader/plot/plot.py` & `icecube-skyreader-1.2.9/skyreader/plot/plot.py`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-1.2.8/skyreader/plot/plotting_tools.py` & `icecube-skyreader-1.2.9/skyreader/plot/plotting_tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -107,15 +107,15 @@
                 size="medium", xycoords="axes fraction")
 
 
 def plot_catalog(master_map, cmap, lower_ra, upper_ra, lower_dec, upper_dec,
         cmap_min=0., cmap_max=250.):
     """"Plots the 4FGL catalog in a color that contrasts with the background
     healpix map."""
-    hdu = pyfits.open('/cvmfs/icecube.opensciencegrid.org/users/steinrob/reference_catalogues/Fermi_4FGL_v18.fit')
+    hdu = pyfits.open('/cvmfs/icecube.opensciencegrid.org/users/azegarelli/realtime/catalogs/gll_psc_v34.fit') ## LAT 14-year Source Catalog (4FGL-DR4 in FITS format) ; https://fermi.gsfc.nasa.gov/ssc/data/access/lat/14yr_catalog/
     fgl = hdu[1]
     pe = [path_effects.Stroke(linewidth=0.5, foreground=cmap(0.0)),
         path_effects.Normal()]
 
     fname_i = np.array(fgl.data['Source_Name'])
     fra_i = np.array(fgl.data['RAJ2000'])*np.pi/180.
     fdec_i = np.array(fgl.data['DEJ2000'])*np.pi/180.
```

### Comparing `icecube-skyreader-1.2.8/skyreader/result.py` & `icecube-skyreader-1.2.9/skyreader/result.py`

 * *Files identical despite different names*

