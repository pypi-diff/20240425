# Comparing `tmp/ecopipeline-0.2.6.tar.gz` & `tmp/ecopipeline-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecopipeline-0.2.6.tar", last modified: Tue Apr 16 19:11:14 2024, max compression
+gzip compressed data, was "ecopipeline-0.2.7.tar", last modified: Wed Apr 24 22:27:53 2024, max compression
```

## Comparing `ecopipeline-0.2.6.tar` & `ecopipeline-0.2.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:11:14.155156 ecopipeline-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 19:10:43.000000 ecopipeline-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-16 19:11:14.155156 ecopipeline-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-16 19:10:43.000000 ecopipeline-0.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-16 19:10:43.000000 ecopipeline-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-16 19:11:14.155156 ecopipeline-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-16 19:10:43.000000 ecopipeline-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:11:14.151156 ecopipeline-0.2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:11:14.151156 ecopipeline-0.2.6/src/ecopipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-16 19:10:43.000000 ecopipeline-0.2.6/src/ecopipeline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:11:14.151156 ecopipeline-0.2.6/src/ecopipeline/extract/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-16 19:10:43.000000 ecopipeline-0.2.6/src/ecopipeline/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27209 2024-04-16 19:10:43.000000 ecopipeline-0.2.6/src/ecopipeline/extract/extract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:11:14.151156 ecopipeline-0.2.6/src/ecopipeline/load/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-16 19:10:43.000000 ecopipeline-0.2.6/src/ecopipeline/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13181 2024-04-16 19:10:43.000000 ecopipeline-0.2.6/src/ecopipeline/load/load.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:11:14.155156 ecopipeline-0.2.6/src/ecopipeline/transform/
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-16 19:10:43.000000 ecopipeline-0.2.6/src/ecopipeline/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17150 2024-04-16 19:10:43.000000 ecopipeline-0.2.6/src/ecopipeline/transform/bayview.py
--rw-r--r--   0 runner    (1001) docker     (127)    33400 2024-04-16 19:10:43.000000 ecopipeline-0.2.6/src/ecopipeline/transform/lbnl.py
--rw-r--r--   0 runner    (1001) docker     (127)    30169 2024-04-16 19:10:43.000000 ecopipeline-0.2.6/src/ecopipeline/transform/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:11:14.155156 ecopipeline-0.2.6/src/ecopipeline/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-04-16 19:10:43.000000 ecopipeline-0.2.6/src/ecopipeline/utils/ConfigManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-16 19:10:43.000000 ecopipeline-0.2.6/src/ecopipeline/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-16 19:10:43.000000 ecopipeline-0.2.6/src/ecopipeline/utils/unit_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:11:14.155156 ecopipeline-0.2.6/src/ecopipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-16 19:11:14.000000 ecopipeline-0.2.6/src/ecopipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-16 19:11:14.000000 ecopipeline-0.2.6/src/ecopipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:11:14.000000 ecopipeline-0.2.6/src/ecopipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-16 19:11:14.000000 ecopipeline-0.2.6/src/ecopipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 19:11:14.000000 ecopipeline-0.2.6/src/ecopipeline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:27:53.378985 ecopipeline-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:27:22.000000 ecopipeline-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-24 22:27:53.378985 ecopipeline-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-24 22:27:22.000000 ecopipeline-0.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-24 22:27:22.000000 ecopipeline-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-24 22:27:53.378985 ecopipeline-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-24 22:27:22.000000 ecopipeline-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:27:53.374985 ecopipeline-0.2.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:27:53.374985 ecopipeline-0.2.7/src/ecopipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-24 22:27:22.000000 ecopipeline-0.2.7/src/ecopipeline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:27:53.374985 ecopipeline-0.2.7/src/ecopipeline/extract/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-24 22:27:22.000000 ecopipeline-0.2.7/src/ecopipeline/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27209 2024-04-24 22:27:22.000000 ecopipeline-0.2.7/src/ecopipeline/extract/extract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:27:53.374985 ecopipeline-0.2.7/src/ecopipeline/load/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-24 22:27:22.000000 ecopipeline-0.2.7/src/ecopipeline/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13181 2024-04-24 22:27:22.000000 ecopipeline-0.2.7/src/ecopipeline/load/load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:27:53.378985 ecopipeline-0.2.7/src/ecopipeline/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-24 22:27:22.000000 ecopipeline-0.2.7/src/ecopipeline/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17150 2024-04-24 22:27:22.000000 ecopipeline-0.2.7/src/ecopipeline/transform/bayview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33400 2024-04-24 22:27:22.000000 ecopipeline-0.2.7/src/ecopipeline/transform/lbnl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30169 2024-04-24 22:27:22.000000 ecopipeline-0.2.7/src/ecopipeline/transform/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:27:53.378985 ecopipeline-0.2.7/src/ecopipeline/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-04-24 22:27:22.000000 ecopipeline-0.2.7/src/ecopipeline/utils/ConfigManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-24 22:27:22.000000 ecopipeline-0.2.7/src/ecopipeline/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-24 22:27:22.000000 ecopipeline-0.2.7/src/ecopipeline/utils/unit_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:27:53.378985 ecopipeline-0.2.7/src/ecopipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-24 22:27:53.000000 ecopipeline-0.2.7/src/ecopipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-24 22:27:53.000000 ecopipeline-0.2.7/src/ecopipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 22:27:53.000000 ecopipeline-0.2.7/src/ecopipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-24 22:27:53.000000 ecopipeline-0.2.7/src/ecopipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 22:27:53.000000 ecopipeline-0.2.7/src/ecopipeline.egg-info/top_level.txt
```

### Comparing `ecopipeline-0.2.6/PKG-INFO` & `ecopipeline-0.2.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecopipeline
-Version: 0.2.6
+Version: 0.2.7
 Summary: Contains functions for use in Ecotope Datapipelines
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ecopipeline-0.2.6/README.md` & `ecopipeline-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.6/setup.cfg` & `ecopipeline-0.2.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ecopipeline
-version = 0.2.6
+version = 0.2.7
 authors = ["Carlos Bello, <bellocarlos@seattleu.edu>, Emil Fahrig <fahrigemil@seattleu.edu>, Casey Mang <cmang@seattleu.edu>, Julian Harris <harrisjulian@seattleu.edu>, Roger Tram <rtram@seattleu.edu>, Nolan Price <nolan@ecotope.com>"]
 description = Contains functions for use in Ecotope Datapipelines
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `ecopipeline-0.2.6/src/ecopipeline/extract/extract.py` & `ecopipeline-0.2.7/src/ecopipeline/extract/extract.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.6/src/ecopipeline/load/load.py` & `ecopipeline-0.2.7/src/ecopipeline/load/load.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.6/src/ecopipeline/transform/__init__.py` & `ecopipeline-0.2.7/src/ecopipeline/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.6/src/ecopipeline/transform/bayview.py` & `ecopipeline-0.2.7/src/ecopipeline/transform/bayview.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.6/src/ecopipeline/transform/lbnl.py` & `ecopipeline-0.2.7/src/ecopipeline/transform/lbnl.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.6/src/ecopipeline/transform/transform.py` & `ecopipeline-0.2.7/src/ecopipeline/transform/transform.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.6/src/ecopipeline/utils/ConfigManager.py` & `ecopipeline-0.2.7/src/ecopipeline/utils/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.6/src/ecopipeline/utils/unit_convert.py` & `ecopipeline-0.2.7/src/ecopipeline/utils/unit_convert.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.6/src/ecopipeline.egg-info/PKG-INFO` & `ecopipeline-0.2.7/src/ecopipeline.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecopipeline
-Version: 0.2.6
+Version: 0.2.7
 Summary: Contains functions for use in Ecotope Datapipelines
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ecopipeline-0.2.6/src/ecopipeline.egg-info/SOURCES.txt` & `ecopipeline-0.2.7/src/ecopipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

