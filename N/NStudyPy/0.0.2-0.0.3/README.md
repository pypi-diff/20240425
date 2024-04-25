# Comparing `tmp/nstudypy-0.0.2.tar.gz` & `tmp/nstudypy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nstudypy-0.0.2.tar", last modified: Thu Apr 25 02:55:57 2024, max compression
+gzip compressed data, was "nstudypy-0.0.3.tar", last modified: Thu Apr 25 03:22:08 2024, max compression
```

## Comparing `nstudypy-0.0.2.tar` & `nstudypy-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:55:57.672266 nstudypy-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-25 02:55:48.000000 nstudypy-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-25 02:55:57.672266 nstudypy-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-25 02:55:48.000000 nstudypy-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-25 02:55:48.000000 nstudypy-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 02:55:48.000000 nstudypy-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 02:55:57.672266 nstudypy-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:55:57.668266 nstudypy-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:55:57.672266 nstudypy-0.0.2/src/NstudyPy/
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-25 02:55:48.000000 nstudypy-0.0.2/src/NstudyPy/PyTools.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-25 02:55:48.000000 nstudypy-0.0.2/src/NstudyPy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:55:57.672266 nstudypy-0.0.2/src/NstudyPy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-25 02:55:57.000000 nstudypy-0.0.2/src/NstudyPy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-25 02:55:57.000000 nstudypy-0.0.2/src/NstudyPy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 02:55:57.000000 nstudypy-0.0.2/src/NstudyPy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 02:55:57.000000 nstudypy-0.0.2/src/NstudyPy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:22:08.392665 nstudypy-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-25 03:21:57.000000 nstudypy-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-25 03:22:08.392665 nstudypy-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-25 03:21:57.000000 nstudypy-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-25 03:21:57.000000 nstudypy-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:57.000000 nstudypy-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 03:22:08.392665 nstudypy-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:22:08.392665 nstudypy-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:22:08.392665 nstudypy-0.0.3/src/NStudyPy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-25 03:21:57.000000 nstudypy-0.0.3/src/NStudyPy/PyTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-25 03:21:57.000000 nstudypy-0.0.3/src/NStudyPy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:22:08.392665 nstudypy-0.0.3/src/NStudyPy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-25 03:22:08.000000 nstudypy-0.0.3/src/NStudyPy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-25 03:22:08.000000 nstudypy-0.0.3/src/NStudyPy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 03:22:08.000000 nstudypy-0.0.3/src/NStudyPy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 03:22:08.000000 nstudypy-0.0.3/src/NStudyPy.egg-info/top_level.txt
```

### Comparing `nstudypy-0.0.2/LICENSE` & `nstudypy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nstudypy-0.0.2/pyproject.toml` & `nstudypy-0.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [project]
-name = "NstudyPy"
+name = "NStudyPy"
 dynamic = ["version", "dependencies"]
 authors = [
   { name="Jack Li", email="lizhq08@gmail.com" },
 ]
-description = "A NstudyPy useful tools"
+description = "A NStudyPy useful tools"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.setuptools.dynamic]
-version = {attr = "src.NstudyPy.__version__"}
+version = {attr = "src.NStudyPy.__version__"}
 dependencies = {file = ["requirements.txt"]}
 
 [project.urls]
 "Homepage" = "https://nstudy.org"
-"Bug Tracker" = "https://github.com/lizhq/NstudyPy/issues"
+"Bug Tracker" = "https://github.com/lizhq/NStudyPy/issues"
```

### Comparing `nstudypy-0.0.2/src/NstudyPy/PyTools.py` & `nstudypy-0.0.3/src/NStudyPy/PyTools.py`

 * *Files identical despite different names*

