# Comparing `tmp/pymindcore-0.2.0.tar.gz` & `tmp/pymindcore-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymindcore-0.2.0.tar", last modified: Thu Apr 25 02:53:04 2024, max compression
+gzip compressed data, was "pymindcore-0.2.1.tar", last modified: Thu Apr 25 03:57:57 2024, max compression
```

## Comparing `pymindcore-0.2.0.tar` & `pymindcore-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 02:53:04.345626 pymindcore-0.2.0/
--rw-rw-rw-   0        0        0      520 2023-11-17 04:55:51.000000 pymindcore-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     3187 2024-04-25 02:53:04.344125 pymindcore-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2598 2024-04-25 02:48:39.000000 pymindcore-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 02:53:04.335618 pymindcore-0.2.0/pymindcore/
--rw-rw-rw-   0        0        0    44585 2024-04-25 02:43:15.000000 pymindcore-0.2.0/pymindcore/core.py
-drwxrwxrwx   0        0        0        0 2024-04-25 02:53:04.342124 pymindcore-0.2.0/pymindcore.egg-info/
--rw-rw-rw-   0        0        0     3187 2024-04-25 02:53:04.000000 pymindcore-0.2.0/pymindcore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2024-04-25 02:53:04.000000 pymindcore-0.2.0/pymindcore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 02:53:04.000000 pymindcore-0.2.0/pymindcore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-04-25 02:53:04.000000 pymindcore-0.2.0/pymindcore.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 02:53:04.000000 pymindcore-0.2.0/pymindcore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 02:53:04.345626 pymindcore-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      766 2024-04-25 02:39:26.000000 pymindcore-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 03:57:57.802024 pymindcore-0.2.1/
+-rw-rw-rw-   0        0        0      520 2023-11-17 04:55:51.000000 pymindcore-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     3187 2024-04-25 03:57:57.800523 pymindcore-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2598 2024-04-25 02:48:39.000000 pymindcore-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 03:57:57.792016 pymindcore-0.2.1/pymindcore/
+-rw-rw-rw-   0        0        0    44585 2024-04-25 02:43:15.000000 pymindcore-0.2.1/pymindcore/core.py
+drwxrwxrwx   0        0        0        0 2024-04-25 03:57:57.799522 pymindcore-0.2.1/pymindcore.egg-info/
+-rw-rw-rw-   0        0        0     3187 2024-04-25 03:57:57.000000 pymindcore-0.2.1/pymindcore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2024-04-25 03:57:57.000000 pymindcore-0.2.1/pymindcore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 03:57:57.000000 pymindcore-0.2.1/pymindcore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-04-25 03:57:57.000000 pymindcore-0.2.1/pymindcore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 03:57:57.000000 pymindcore-0.2.1/pymindcore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 03:57:57.802524 pymindcore-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      766 2024-04-25 03:57:29.000000 pymindcore-0.2.1/setup.py
```

### Comparing `pymindcore-0.2.0/LICENSE` & `pymindcore-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymindcore-0.2.0/PKG-INFO` & `pymindcore-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymindcore
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python library for AI, easy to use, freely available for any use
 Home-page: https://github.com/Dogz-R-Godz/Pymind
 Author: Dogz R Godz
 Author-email: doggocam01@gmail.com
 License: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
```

### Comparing `pymindcore-0.2.0/README.md` & `pymindcore-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pymindcore-0.2.0/pymindcore/core.py` & `pymindcore-0.2.1/pymindcore/core.py`

 * *Files identical despite different names*

### Comparing `pymindcore-0.2.0/pymindcore.egg-info/PKG-INFO` & `pymindcore-0.2.1/pymindcore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymindcore
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python library for AI, easy to use, freely available for any use
 Home-page: https://github.com/Dogz-R-Godz/Pymind
 Author: Dogz R Godz
 Author-email: doggocam01@gmail.com
 License: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
```

### Comparing `pymindcore-0.2.0/setup.py` & `pymindcore-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pymindcore',
-    version='0.2.0',
+    version='0.2.1',
     packages=find_packages(),
     description='A Python library for AI, easy to use, freely available for any use',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Dogz-R-Godz/Pymind',
     author='Dogz R Godz',
     author_email='doggocam01@gmail.com',
```

