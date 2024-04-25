# Comparing `tmp/arrapi-1.4.8.tar.gz` & `tmp/arrapi-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arrapi-1.4.8.tar", last modified: Sun Apr 21 18:03:49 2024, max compression
+gzip compressed data, was "arrapi-1.4.9.tar", last modified: Sun Apr 21 18:10:15 2024, max compression
```

## Comparing `arrapi-1.4.8.tar` & `arrapi-1.4.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:03:49.410606 arrapi-1.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-21 18:03:36.000000 arrapi-1.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13981 2024-04-21 18:03:49.410606 arrapi-1.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12942 2024-04-21 18:03:36.000000 arrapi-1.4.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:03:49.402605 arrapi-1.4.8/arrapi/
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-21 18:03:36.000000 arrapi-1.4.8/arrapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:03:49.406606 arrapi-1.4.8/arrapi/apis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 18:03:36.000000 arrapi-1.4.8/arrapi/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-04-21 18:03:36.000000 arrapi-1.4.8/arrapi/apis/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-21 18:03:36.000000 arrapi-1.4.8/arrapi/apis/lidarr.py
--rw-r--r--   0 runner    (1001) docker     (127)    20751 2024-04-21 18:03:36.000000 arrapi-1.4.8/arrapi/apis/radarr.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-21 18:03:36.000000 arrapi-1.4.8/arrapi/apis/readarr.py
--rw-r--r--   0 runner    (1001) docker     (127)    24653 2024-04-21 18:03:36.000000 arrapi-1.4.8/arrapi/apis/sonarr.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-21 18:03:36.000000 arrapi-1.4.8/arrapi/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:03:49.406606 arrapi-1.4.8/arrapi/objs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 18:03:36.000000 arrapi-1.4.8/arrapi/objs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-04-21 18:03:36.000000 arrapi-1.4.8/arrapi/objs/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    36475 2024-04-21 18:03:36.000000 arrapi-1.4.8/arrapi/objs/reload.py
--rw-r--r--   0 runner    (1001) docker     (127)     8301 2024-04-21 18:03:36.000000 arrapi-1.4.8/arrapi/objs/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:03:49.406606 arrapi-1.4.8/arrapi/raws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 18:03:36.000000 arrapi-1.4.8/arrapi/raws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-04-21 18:03:36.000000 arrapi-1.4.8/arrapi/raws/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-21 18:03:36.000000 arrapi-1.4.8/arrapi/raws/lidarr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-21 18:03:36.000000 arrapi-1.4.8/arrapi/raws/radarr.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-21 18:03:36.000000 arrapi-1.4.8/arrapi/raws/readarr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-21 18:03:36.000000 arrapi-1.4.8/arrapi/raws/sonarr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:03:49.406606 arrapi-1.4.8/arrapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13981 2024-04-21 18:03:49.000000 arrapi-1.4.8/arrapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-21 18:03:49.000000 arrapi-1.4.8/arrapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 18:03:49.000000 arrapi-1.4.8/arrapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-21 18:03:49.000000 arrapi-1.4.8/arrapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-21 18:03:49.000000 arrapi-1.4.8/arrapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 18:03:49.410606 arrapi-1.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-21 18:03:36.000000 arrapi-1.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:03:49.406606 arrapi-1.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-04-21 18:03:36.000000 arrapi-1.4.8/tests/test_radarr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-04-21 18:03:36.000000 arrapi-1.4.8/tests/test_sonarr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:10:15.684672 arrapi-1.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-21 18:10:02.000000 arrapi-1.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13981 2024-04-21 18:10:15.684672 arrapi-1.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12942 2024-04-21 18:10:02.000000 arrapi-1.4.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:10:15.680672 arrapi-1.4.9/arrapi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-21 18:10:02.000000 arrapi-1.4.9/arrapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:10:15.680672 arrapi-1.4.9/arrapi/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 18:10:02.000000 arrapi-1.4.9/arrapi/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-04-21 18:10:02.000000 arrapi-1.4.9/arrapi/apis/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-21 18:10:02.000000 arrapi-1.4.9/arrapi/apis/lidarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20751 2024-04-21 18:10:02.000000 arrapi-1.4.9/arrapi/apis/radarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-21 18:10:02.000000 arrapi-1.4.9/arrapi/apis/readarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24653 2024-04-21 18:10:02.000000 arrapi-1.4.9/arrapi/apis/sonarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-21 18:10:02.000000 arrapi-1.4.9/arrapi/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:10:15.680672 arrapi-1.4.9/arrapi/objs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 18:10:02.000000 arrapi-1.4.9/arrapi/objs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-04-21 18:10:02.000000 arrapi-1.4.9/arrapi/objs/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36475 2024-04-21 18:10:02.000000 arrapi-1.4.9/arrapi/objs/reload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8301 2024-04-21 18:10:02.000000 arrapi-1.4.9/arrapi/objs/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:10:15.684672 arrapi-1.4.9/arrapi/raws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 18:10:02.000000 arrapi-1.4.9/arrapi/raws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-04-21 18:10:02.000000 arrapi-1.4.9/arrapi/raws/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-21 18:10:02.000000 arrapi-1.4.9/arrapi/raws/lidarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-21 18:10:02.000000 arrapi-1.4.9/arrapi/raws/radarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-21 18:10:02.000000 arrapi-1.4.9/arrapi/raws/readarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-21 18:10:02.000000 arrapi-1.4.9/arrapi/raws/sonarr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:10:15.684672 arrapi-1.4.9/arrapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13981 2024-04-21 18:10:15.000000 arrapi-1.4.9/arrapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-21 18:10:15.000000 arrapi-1.4.9/arrapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 18:10:15.000000 arrapi-1.4.9/arrapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-21 18:10:15.000000 arrapi-1.4.9/arrapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-21 18:10:15.000000 arrapi-1.4.9/arrapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 18:10:15.684672 arrapi-1.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-21 18:10:02.000000 arrapi-1.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:10:15.684672 arrapi-1.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-04-21 18:10:02.000000 arrapi-1.4.9/tests/test_radarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-04-21 18:10:02.000000 arrapi-1.4.9/tests/test_sonarr.py
```

### Comparing `arrapi-1.4.8/LICENSE` & `arrapi-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `arrapi-1.4.8/PKG-INFO` & `arrapi-1.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrapi
-Version: 1.4.8
+Version: 1.4.9
 Summary: Python wrapper for Radarr and Sonarr APIs:
 Home-page: https://github.com/Kometa-Team/ArrAPI
 Author: Nathan Taggart
 Author-email: kometateam@proton.me
 License: MIT License
 Project-URL: Documentation, https://arrapi.kometa.wiki
 Project-URL: Funding, https://github.com/sponsors/meisnate12
```

### Comparing `arrapi-1.4.8/README.rst` & `arrapi-1.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `arrapi-1.4.8/arrapi/__init__.py` & `arrapi-1.4.9/arrapi/__init__.py`

 * *Files identical despite different names*

### Comparing `arrapi-1.4.8/arrapi/apis/base.py` & `arrapi-1.4.9/arrapi/apis/base.py`

 * *Files identical despite different names*

### Comparing `arrapi-1.4.8/arrapi/apis/radarr.py` & `arrapi-1.4.9/arrapi/apis/radarr.py`

 * *Files identical despite different names*

### Comparing `arrapi-1.4.8/arrapi/apis/sonarr.py` & `arrapi-1.4.9/arrapi/apis/sonarr.py`

 * *Files identical despite different names*

### Comparing `arrapi-1.4.8/arrapi/exceptions.py` & `arrapi-1.4.9/arrapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `arrapi-1.4.8/arrapi/objs/base.py` & `arrapi-1.4.9/arrapi/objs/base.py`

 * *Files identical despite different names*

### Comparing `arrapi-1.4.8/arrapi/objs/reload.py` & `arrapi-1.4.9/arrapi/objs/reload.py`

 * *Files identical despite different names*

### Comparing `arrapi-1.4.8/arrapi/objs/simple.py` & `arrapi-1.4.9/arrapi/objs/simple.py`

 * *Files identical despite different names*

### Comparing `arrapi-1.4.8/arrapi/raws/base.py` & `arrapi-1.4.9/arrapi/raws/base.py`

 * *Files identical despite different names*

### Comparing `arrapi-1.4.8/arrapi/raws/radarr.py` & `arrapi-1.4.9/arrapi/raws/radarr.py`

 * *Files identical despite different names*

### Comparing `arrapi-1.4.8/arrapi/raws/sonarr.py` & `arrapi-1.4.9/arrapi/raws/sonarr.py`

 * *Files identical despite different names*

### Comparing `arrapi-1.4.8/arrapi.egg-info/PKG-INFO` & `arrapi-1.4.9/arrapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrapi
-Version: 1.4.8
+Version: 1.4.9
 Summary: Python wrapper for Radarr and Sonarr APIs:
 Home-page: https://github.com/Kometa-Team/ArrAPI
 Author: Nathan Taggart
 Author-email: kometateam@proton.me
 License: MIT License
 Project-URL: Documentation, https://arrapi.kometa.wiki
 Project-URL: Funding, https://github.com/sponsors/meisnate12
```

### Comparing `arrapi-1.4.8/arrapi.egg-info/SOURCES.txt` & `arrapi-1.4.9/arrapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arrapi-1.4.8/setup.py` & `arrapi-1.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `arrapi-1.4.8/tests/test_radarr.py` & `arrapi-1.4.9/tests/test_radarr.py`

 * *Files identical despite different names*

### Comparing `arrapi-1.4.8/tests/test_sonarr.py` & `arrapi-1.4.9/tests/test_sonarr.py`

 * *Files identical despite different names*

