# Comparing `tmp/robotframework-xlibrary-11.0.4.tar.gz` & `tmp/robotframework-xlibrary-11.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\robotframework-xlibrary-11.0.4.tar", last modified: Tue Apr 23 10:13:28 2024, max compression
+gzip compressed data, was "dist\robotframework-xlibrary-11.0.5.tar", last modified: Wed Apr 24 03:29:40 2024, max compression
```

## Comparing `robotframework-xlibrary-11.0.4.tar` & `robotframework-xlibrary-11.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 10:13:28.000000 robotframework-xlibrary-11.0.4/
--rw-rw-rw-   0        0        0        0 2024-03-13 03:39:44.000000 robotframework-xlibrary-11.0.4/LICENSE
--rw-rw-rw-   0        0        0     2269 2024-04-23 10:13:28.000000 robotframework-xlibrary-11.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1777 2024-04-22 17:31:21.000000 robotframework-xlibrary-11.0.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-23 10:13:28.000000 robotframework-xlibrary-11.0.4/setup.cfg
--rw-rw-rw-   0        0        0      779 2024-04-23 10:08:25.000000 robotframework-xlibrary-11.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 10:13:28.000000 robotframework-xlibrary-11.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-23 10:13:28.000000 robotframework-xlibrary-11.0.4/src/XLibrary/
--rw-rw-rw-   0        0        0     1114 2024-04-17 07:26:57.000000 robotframework-xlibrary-11.0.4/src/XLibrary/__init__.py
--rw-rw-rw-   0        0        0      235 2024-03-18 09:34:26.000000 robotframework-xlibrary-11.0.4/src/XLibrary/main.py
-drwxrwxrwx   0        0        0        0 2024-04-23 10:13:28.000000 robotframework-xlibrary-11.0.4/src/XLibrary/submodule1/
--rw-rw-rw-   0        0        0      108 2024-03-18 09:34:30.000000 robotframework-xlibrary-11.0.4/src/XLibrary/submodule1/__init__.py
--rw-rw-rw-   0        0        0     1421 2024-04-18 05:25:30.000000 robotframework-xlibrary-11.0.4/src/XLibrary/submodule1/module1.py
--rw-rw-rw-   0        0        0     7948 2024-04-23 09:32:37.000000 robotframework-xlibrary-11.0.4/src/XLibrary/submodule1/module2.py
-drwxrwxrwx   0        0        0        0 2024-04-23 10:13:28.000000 robotframework-xlibrary-11.0.4/src/XLibrary/submodule2/
--rw-rw-rw-   0        0        0      114 2024-03-18 09:34:30.000000 robotframework-xlibrary-11.0.4/src/XLibrary/submodule2/__init__.py
--rw-rw-rw-   0        0        0     1774 2024-04-13 12:59:03.000000 robotframework-xlibrary-11.0.4/src/XLibrary/submodule2/module1.py
--rw-rw-rw-   0        0        0      261 2024-04-22 17:28:01.000000 robotframework-xlibrary-11.0.4/src/XLibrary/submodule2/module2.py
-drwxrwxrwx   0        0        0        0 2024-04-23 10:13:28.000000 robotframework-xlibrary-11.0.4/src/robotframework_xlibrary.egg-info/
--rw-rw-rw-   0        0        0     2269 2024-04-23 10:13:28.000000 robotframework-xlibrary-11.0.4/src/robotframework_xlibrary.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      538 2024-04-23 10:13:28.000000 robotframework-xlibrary-11.0.4/src/robotframework_xlibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 10:13:28.000000 robotframework-xlibrary-11.0.4/src/robotframework_xlibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-23 10:13:28.000000 robotframework-xlibrary-11.0.4/src/robotframework_xlibrary.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-23 10:13:28.000000 robotframework-xlibrary-11.0.4/src/robotframework_xlibrary.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 03:29:40.000000 robotframework-xlibrary-11.0.5/
+-rw-rw-rw-   0        0        0        0 2024-03-13 03:39:44.000000 robotframework-xlibrary-11.0.5/LICENSE
+-rw-rw-rw-   0        0        0     2269 2024-04-24 03:29:40.000000 robotframework-xlibrary-11.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1777 2024-04-22 17:31:21.000000 robotframework-xlibrary-11.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-24 03:29:40.000000 robotframework-xlibrary-11.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      779 2024-04-24 03:27:40.000000 robotframework-xlibrary-11.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:29:40.000000 robotframework-xlibrary-11.0.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-24 03:29:40.000000 robotframework-xlibrary-11.0.5/src/XLibrary/
+-rw-rw-rw-   0        0        0     1114 2024-04-17 07:26:57.000000 robotframework-xlibrary-11.0.5/src/XLibrary/__init__.py
+-rw-rw-rw-   0        0        0      235 2024-03-18 09:34:26.000000 robotframework-xlibrary-11.0.5/src/XLibrary/main.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:29:40.000000 robotframework-xlibrary-11.0.5/src/XLibrary/submodule1/
+-rw-rw-rw-   0        0        0      108 2024-03-18 09:34:30.000000 robotframework-xlibrary-11.0.5/src/XLibrary/submodule1/__init__.py
+-rw-rw-rw-   0        0        0     4870 2024-04-24 03:28:43.000000 robotframework-xlibrary-11.0.5/src/XLibrary/submodule1/module1.py
+-rw-rw-rw-   0        0        0     7948 2024-04-23 09:32:37.000000 robotframework-xlibrary-11.0.5/src/XLibrary/submodule1/module2.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:29:40.000000 robotframework-xlibrary-11.0.5/src/XLibrary/submodule2/
+-rw-rw-rw-   0        0        0      114 2024-03-18 09:34:30.000000 robotframework-xlibrary-11.0.5/src/XLibrary/submodule2/__init__.py
+-rw-rw-rw-   0        0        0     1774 2024-04-13 12:59:03.000000 robotframework-xlibrary-11.0.5/src/XLibrary/submodule2/module1.py
+-rw-rw-rw-   0        0        0      261 2024-04-22 17:28:01.000000 robotframework-xlibrary-11.0.5/src/XLibrary/submodule2/module2.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:29:40.000000 robotframework-xlibrary-11.0.5/src/robotframework_xlibrary.egg-info/
+-rw-rw-rw-   0        0        0     2269 2024-04-24 03:29:40.000000 robotframework-xlibrary-11.0.5/src/robotframework_xlibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      538 2024-04-24 03:29:40.000000 robotframework-xlibrary-11.0.5/src/robotframework_xlibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 03:29:40.000000 robotframework-xlibrary-11.0.5/src/robotframework_xlibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-24 03:29:40.000000 robotframework-xlibrary-11.0.5/src/robotframework_xlibrary.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-24 03:29:40.000000 robotframework-xlibrary-11.0.5/src/robotframework_xlibrary.egg-info/top_level.txt
```

### Comparing `robotframework-xlibrary-11.0.4/PKG-INFO` & `robotframework-xlibrary-11.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-xlibrary
-Version: 11.0.4
+Version: 11.0.5
 Summary: Custom Library for MyAIS 2.0 Automation
 Home-page: https://github.com/Khrx1999/robotframework-xlibrary.git
 Author: Tassana Khrueawan
 Author-email: tassana.khr@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `robotframework-xlibrary-11.0.4/README.md` & `robotframework-xlibrary-11.0.5/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-xlibrary-11.0.4/setup.py` & `robotframework-xlibrary-11.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="robotframework-xlibrary",
-    version="11.0.4",
+    version="11.0.5",
     author="Tassana Khrueawan",
     author_email="tassana.khr@gmail.com",
     description="Custom Library for MyAIS 2.0 Automation",
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Khrx1999/robotframework-xlibrary.git",
     package_dir={'': 'src'},
```

### Comparing `robotframework-xlibrary-11.0.4/src/XLibrary/__init__.py` & `robotframework-xlibrary-11.0.5/src/XLibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-xlibrary-11.0.4/src/XLibrary/submodule1/module2.py` & `robotframework-xlibrary-11.0.5/src/XLibrary/submodule1/module2.py`

 * *Files identical despite different names*

### Comparing `robotframework-xlibrary-11.0.4/src/XLibrary/submodule2/module1.py` & `robotframework-xlibrary-11.0.5/src/XLibrary/submodule2/module1.py`

 * *Files identical despite different names*

### Comparing `robotframework-xlibrary-11.0.4/src/robotframework_xlibrary.egg-info/PKG-INFO` & `robotframework-xlibrary-11.0.5/src/robotframework_xlibrary.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-xlibrary
-Version: 11.0.4
+Version: 11.0.5
 Summary: Custom Library for MyAIS 2.0 Automation
 Home-page: https://github.com/Khrx1999/robotframework-xlibrary.git
 Author: Tassana Khrueawan
 Author-email: tassana.khr@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `robotframework-xlibrary-11.0.4/src/robotframework_xlibrary.egg-info/SOURCES.txt` & `robotframework-xlibrary-11.0.5/src/robotframework_xlibrary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

