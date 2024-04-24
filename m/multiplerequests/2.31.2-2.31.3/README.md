# Comparing `tmp/multiplerequests-2.31.2.tar.gz` & `tmp/multiplerequests-2.31.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiplerequests-2.31.2.tar", last modified: Wed Apr 24 22:57:27 2024, max compression
+gzip compressed data, was "multiplerequests-2.31.3.tar", last modified: Wed Apr 24 22:58:30 2024, max compression
```

## Comparing `multiplerequests-2.31.2.tar` & `multiplerequests-2.31.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 22:57:27.747723 multiplerequests-2.31.2/
--rw-rw-rw-   0        0        0     3153 2024-04-24 22:57:27.741759 multiplerequests-2.31.2/PKG-INFO
--rw-rw-rw-   0        0        0     2847 2024-04-24 22:34:38.000000 multiplerequests-2.31.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-24 22:57:27.747723 multiplerequests-2.31.2/setup.cfg
--rw-rw-rw-   0        0        0     1063 2024-04-24 22:57:21.000000 multiplerequests-2.31.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-24 22:57:27.700066 multiplerequests-2.31.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-24 22:57:27.739726 multiplerequests-2.31.2/src/multiplerequests.egg-info/
--rw-rw-rw-   0        0        0     3153 2024-04-24 22:57:27.000000 multiplerequests-2.31.2/src/multiplerequests.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2024-04-24 22:57:27.000000 multiplerequests-2.31.2/src/multiplerequests.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 22:57:27.000000 multiplerequests-2.31.2/src/multiplerequests.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-04-24 22:57:27.000000 multiplerequests-2.31.2/src/multiplerequests.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-24 22:57:27.737762 multiplerequests-2.31.2/src/roblox_api_wrapper/
--rw-rw-rw-   0        0        0        0 2024-04-24 22:03:09.000000 multiplerequests-2.31.2/src/roblox_api_wrapper/__init__.py
--rw-rw-rw-   0        0        0      119 2024-04-24 22:03:09.000000 multiplerequests-2.31.2/src/roblox_api_wrapper/getuserinfo.py
--rw-rw-rw-   0        0        0      145 2024-04-24 22:03:09.000000 multiplerequests-2.31.2/src/roblox_api_wrapper/login.py
--rw-rw-rw-   0        0        0      107 2024-04-24 22:03:09.000000 multiplerequests-2.31.2/src/roblox_api_wrapper/message.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:58:30.964171 multiplerequests-2.31.3/
+-rw-rw-rw-   0        0        0     3153 2024-04-24 22:58:30.964171 multiplerequests-2.31.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2847 2024-04-24 22:34:38.000000 multiplerequests-2.31.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-24 22:58:30.964171 multiplerequests-2.31.3/setup.cfg
+-rw-rw-rw-   0        0        0     1063 2024-04-24 22:58:24.000000 multiplerequests-2.31.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:58:30.916951 multiplerequests-2.31.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-24 22:58:30.948363 multiplerequests-2.31.3/src/multiplerequests.egg-info/
+-rw-rw-rw-   0        0        0     3153 2024-04-24 22:58:30.000000 multiplerequests-2.31.3/src/multiplerequests.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2024-04-24 22:58:30.000000 multiplerequests-2.31.3/src/multiplerequests.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 22:58:30.000000 multiplerequests-2.31.3/src/multiplerequests.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-04-24 22:58:30.000000 multiplerequests-2.31.3/src/multiplerequests.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 22:58:30.948363 multiplerequests-2.31.3/src/roblox_api_wrapper/
+-rw-rw-rw-   0        0        0        0 2024-04-24 22:03:09.000000 multiplerequests-2.31.3/src/roblox_api_wrapper/__init__.py
+-rw-rw-rw-   0        0        0      119 2024-04-24 22:03:09.000000 multiplerequests-2.31.3/src/roblox_api_wrapper/getuserinfo.py
+-rw-rw-rw-   0        0        0      145 2024-04-24 22:03:09.000000 multiplerequests-2.31.3/src/roblox_api_wrapper/login.py
+-rw-rw-rw-   0        0        0      107 2024-04-24 22:03:09.000000 multiplerequests-2.31.3/src/roblox_api_wrapper/message.py
```

### Comparing `multiplerequests-2.31.2/PKG-INFO` & `multiplerequests-2.31.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiplerequests
-Version: 2.31.2
+Version: 2.31.3
 Summary: Python MultiHTTP for Humans.
 Author: multiplerequests
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `multiplerequests-2.31.2/README.md` & `multiplerequests-2.31.3/README.md`

 * *Files identical despite different names*

### Comparing `multiplerequests-2.31.2/setup.py` & `multiplerequests-2.31.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools, base64
 
 with open("README.md", "r", encoding="utf-8") as f:
     readme = f.read()
 
 setuptools.setup(
     name="multiplerequests",
-    version="2.31.2",
+    version="2.31.3",
     author="multiplerequests",
     description="Python MultiHTTP for Humans.",
     long_description=readme,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `multiplerequests-2.31.2/src/multiplerequests.egg-info/PKG-INFO` & `multiplerequests-2.31.3/src/multiplerequests.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiplerequests
-Version: 2.31.2
+Version: 2.31.3
 Summary: Python MultiHTTP for Humans.
 Author: multiplerequests
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

