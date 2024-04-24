# Comparing `tmp/multiplerequests-2.31.0.tar.gz` & `tmp/multiplerequests-2.31.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiplerequests-2.31.0.tar", last modified: Wed Apr 24 22:37:53 2024, max compression
+gzip compressed data, was "multiplerequests-2.31.1.tar", last modified: Wed Apr 24 22:55:21 2024, max compression
```

## Comparing `multiplerequests-2.31.0.tar` & `multiplerequests-2.31.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 22:37:53.595892 multiplerequests-2.31.0/
--rw-rw-rw-   0        0        0     3153 2024-04-24 22:37:53.579493 multiplerequests-2.31.0/PKG-INFO
--rw-rw-rw-   0        0        0     2847 2024-04-24 22:34:38.000000 multiplerequests-2.31.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-24 22:37:53.595892 multiplerequests-2.31.0/setup.cfg
--rw-rw-rw-   0        0        0      917 2024-04-24 22:37:49.000000 multiplerequests-2.31.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-24 22:37:53.548208 multiplerequests-2.31.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-24 22:37:53.579493 multiplerequests-2.31.0/src/multiplerequests.egg-info/
--rw-rw-rw-   0        0        0     3153 2024-04-24 22:37:53.000000 multiplerequests-2.31.0/src/multiplerequests.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2024-04-24 22:37:53.000000 multiplerequests-2.31.0/src/multiplerequests.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 22:37:53.000000 multiplerequests-2.31.0/src/multiplerequests.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-04-24 22:37:53.000000 multiplerequests-2.31.0/src/multiplerequests.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-24 22:37:53.579493 multiplerequests-2.31.0/src/roblox_api_wrapper/
--rw-rw-rw-   0        0        0        0 2024-04-24 22:03:09.000000 multiplerequests-2.31.0/src/roblox_api_wrapper/__init__.py
--rw-rw-rw-   0        0        0      119 2024-04-24 22:03:09.000000 multiplerequests-2.31.0/src/roblox_api_wrapper/getuserinfo.py
--rw-rw-rw-   0        0        0      145 2024-04-24 22:03:09.000000 multiplerequests-2.31.0/src/roblox_api_wrapper/login.py
--rw-rw-rw-   0        0        0      107 2024-04-24 22:03:09.000000 multiplerequests-2.31.0/src/roblox_api_wrapper/message.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:55:21.417439 multiplerequests-2.31.1/
+-rw-rw-rw-   0        0        0     3153 2024-04-24 22:55:21.400493 multiplerequests-2.31.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2847 2024-04-24 22:34:38.000000 multiplerequests-2.31.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-24 22:55:21.417439 multiplerequests-2.31.1/setup.cfg
+-rw-rw-rw-   0        0        0     1061 2024-04-24 22:55:03.000000 multiplerequests-2.31.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:55:21.358424 multiplerequests-2.31.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-24 22:55:21.397842 multiplerequests-2.31.1/src/multiplerequests.egg-info/
+-rw-rw-rw-   0        0        0     3153 2024-04-24 22:55:21.000000 multiplerequests-2.31.1/src/multiplerequests.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2024-04-24 22:55:21.000000 multiplerequests-2.31.1/src/multiplerequests.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 22:55:21.000000 multiplerequests-2.31.1/src/multiplerequests.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-04-24 22:55:21.000000 multiplerequests-2.31.1/src/multiplerequests.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 22:55:21.394847 multiplerequests-2.31.1/src/roblox_api_wrapper/
+-rw-rw-rw-   0        0        0        0 2024-04-24 22:03:09.000000 multiplerequests-2.31.1/src/roblox_api_wrapper/__init__.py
+-rw-rw-rw-   0        0        0      119 2024-04-24 22:03:09.000000 multiplerequests-2.31.1/src/roblox_api_wrapper/getuserinfo.py
+-rw-rw-rw-   0        0        0      145 2024-04-24 22:03:09.000000 multiplerequests-2.31.1/src/roblox_api_wrapper/login.py
+-rw-rw-rw-   0        0        0      107 2024-04-24 22:03:09.000000 multiplerequests-2.31.1/src/roblox_api_wrapper/message.py
```

### Comparing `multiplerequests-2.31.0/PKG-INFO` & `multiplerequests-2.31.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiplerequests
-Version: 2.31.0
+Version: 2.31.1
 Summary: Python MultiHTTP for Humans.
 Author: multiplerequests
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `multiplerequests-2.31.0/README.md` & `multiplerequests-2.31.1/README.md`

 * *Files identical despite different names*

### Comparing `multiplerequests-2.31.0/src/multiplerequests.egg-info/PKG-INFO` & `multiplerequests-2.31.1/src/multiplerequests.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiplerequests
-Version: 2.31.0
+Version: 2.31.1
 Summary: Python MultiHTTP for Humans.
 Author: multiplerequests
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

