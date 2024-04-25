# Comparing `tmp/dir2prompt-1.0.5.tar.gz` & `tmp/dir2prompt-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dir2prompt-1.0.5.tar", last modified: Thu Apr 25 16:44:53 2024, max compression
+gzip compressed data, was "dir2prompt-1.0.6.tar", last modified: Thu Apr 25 17:04:12 2024, max compression
```

## Comparing `dir2prompt-1.0.5.tar` & `dir2prompt-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mkieffer   (501) staff       (20)        0 2024-04-25 16:44:53.260195 dir2prompt-1.0.5/
--rw-r--r--   0 mkieffer   (501) staff       (20)     1069 2024-04-02 23:08:45.000000 dir2prompt-1.0.5/LICENSE
--rw-r--r--   0 mkieffer   (501) staff       (20)     6624 2024-04-25 16:44:53.259993 dir2prompt-1.0.5/PKG-INFO
--rw-r--r--   0 mkieffer   (501) staff       (20)     4322 2024-04-25 15:53:20.000000 dir2prompt-1.0.5/README.md
-drwxr-xr-x   0 mkieffer   (501) staff       (20)        0 2024-04-25 16:44:53.259743 dir2prompt-1.0.5/dir2prompt.egg-info/
--rw-r--r--   0 mkieffer   (501) staff       (20)     6624 2024-04-25 16:44:53.000000 dir2prompt-1.0.5/dir2prompt.egg-info/PKG-INFO
--rw-r--r--   0 mkieffer   (501) staff       (20)      257 2024-04-25 16:44:53.000000 dir2prompt-1.0.5/dir2prompt.egg-info/SOURCES.txt
--rw-r--r--   0 mkieffer   (501) staff       (20)        1 2024-04-25 16:44:53.000000 dir2prompt-1.0.5/dir2prompt.egg-info/dependency_links.txt
--rw-r--r--   0 mkieffer   (501) staff       (20)       37 2024-04-25 16:44:53.000000 dir2prompt-1.0.5/dir2prompt.egg-info/entry_points.txt
--rw-r--r--   0 mkieffer   (501) staff       (20)        4 2024-04-25 16:44:53.000000 dir2prompt-1.0.5/dir2prompt.egg-info/top_level.txt
--rw-r--r--   0 mkieffer   (501) staff       (20)     1241 2024-04-25 16:44:48.000000 dir2prompt-1.0.5/pyproject.toml
--rw-r--r--   0 mkieffer   (501) staff       (20)       38 2024-04-25 16:44:53.260249 dir2prompt-1.0.5/setup.cfg
--rw-r--r--   0 mkieffer   (501) staff       (20)     1370 2024-04-03 04:12:15.000000 dir2prompt-1.0.5/setup.py
-drwxr-xr-x   0 mkieffer   (501) staff       (20)        0 2024-04-25 16:44:53.259542 dir2prompt-1.0.5/src/
--rw-r--r--   0 mkieffer   (501) staff       (20)        0 2024-04-25 16:44:25.000000 dir2prompt-1.0.5/src/__init__.py
--rw-r--r--   0 mkieffer   (501) staff       (20)      978 2024-04-02 23:57:47.000000 dir2prompt-1.0.5/src/config.json
--rw-r--r--   0 mkieffer   (501) staff       (20)     7916 2024-04-25 16:39:29.000000 dir2prompt-1.0.5/src/d2p.py
+drwxr-xr-x   0 mkieffer   (501) staff       (20)        0 2024-04-25 17:04:12.008733 dir2prompt-1.0.6/
+-rw-r--r--   0 mkieffer   (501) staff       (20)     1069 2024-04-02 23:08:45.000000 dir2prompt-1.0.6/LICENSE
+-rw-r--r--   0 mkieffer   (501) staff       (20)     6624 2024-04-25 17:04:12.008490 dir2prompt-1.0.6/PKG-INFO
+-rw-r--r--   0 mkieffer   (501) staff       (20)     4322 2024-04-25 15:53:20.000000 dir2prompt-1.0.6/README.md
+drwxr-xr-x   0 mkieffer   (501) staff       (20)        0 2024-04-25 17:04:12.008174 dir2prompt-1.0.6/dir2prompt.egg-info/
+-rw-r--r--   0 mkieffer   (501) staff       (20)     6624 2024-04-25 17:04:12.000000 dir2prompt-1.0.6/dir2prompt.egg-info/PKG-INFO
+-rw-r--r--   0 mkieffer   (501) staff       (20)      257 2024-04-25 17:04:12.000000 dir2prompt-1.0.6/dir2prompt.egg-info/SOURCES.txt
+-rw-r--r--   0 mkieffer   (501) staff       (20)        1 2024-04-25 17:04:12.000000 dir2prompt-1.0.6/dir2prompt.egg-info/dependency_links.txt
+-rw-r--r--   0 mkieffer   (501) staff       (20)       37 2024-04-25 17:04:12.000000 dir2prompt-1.0.6/dir2prompt.egg-info/entry_points.txt
+-rw-r--r--   0 mkieffer   (501) staff       (20)        4 2024-04-25 17:04:12.000000 dir2prompt-1.0.6/dir2prompt.egg-info/top_level.txt
+-rw-r--r--   0 mkieffer   (501) staff       (20)     1241 2024-04-25 17:02:06.000000 dir2prompt-1.0.6/pyproject.toml
+-rw-r--r--   0 mkieffer   (501) staff       (20)       38 2024-04-25 17:04:12.008792 dir2prompt-1.0.6/setup.cfg
+-rw-r--r--   0 mkieffer   (501) staff       (20)     1470 2024-04-25 17:02:57.000000 dir2prompt-1.0.6/setup.py
+drwxr-xr-x   0 mkieffer   (501) staff       (20)        0 2024-04-25 17:04:12.007721 dir2prompt-1.0.6/src/
+-rw-r--r--   0 mkieffer   (501) staff       (20)        0 2024-04-25 16:44:25.000000 dir2prompt-1.0.6/src/__init__.py
+-rw-r--r--   0 mkieffer   (501) staff       (20)      978 2024-04-02 23:57:47.000000 dir2prompt-1.0.6/src/config.json
+-rw-r--r--   0 mkieffer   (501) staff       (20)     7916 2024-04-25 16:39:29.000000 dir2prompt-1.0.6/src/d2p.py
```

### Comparing `dir2prompt-1.0.5/LICENSE` & `dir2prompt-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dir2prompt-1.0.5/PKG-INFO` & `dir2prompt-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dir2prompt
-Version: 1.0.5
+Version: 1.0.6
 Summary: Generate prompts for long-context LLMs using the content in your directory
 Home-page: https://github.com/mkieffer1107/dir2prompt
 Author: Max Kieffer
 Author-email: Max Kieffer <wkieffer@ufl.edu>
 License: MIT License
         
         Copyright (c) 2024 mkieffer1107
```

### Comparing `dir2prompt-1.0.5/README.md` & `dir2prompt-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `dir2prompt-1.0.5/dir2prompt.egg-info/PKG-INFO` & `dir2prompt-1.0.6/dir2prompt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dir2prompt
-Version: 1.0.5
+Version: 1.0.6
 Summary: Generate prompts for long-context LLMs using the content in your directory
 Home-page: https://github.com/mkieffer1107/dir2prompt
 Author: Max Kieffer
 Author-email: Max Kieffer <wkieffer@ufl.edu>
 License: MIT License
         
         Copyright (c) 2024 mkieffer1107
```

### Comparing `dir2prompt-1.0.5/pyproject.toml` & `dir2prompt-1.0.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dir2prompt"
-version = "1.0.5"
+version = "1.0.6"
 license = {file = "LICENSE"}
 authors = [
   { name="Max Kieffer", email="wkieffer@ufl.edu" },
 ]
 description = "Generate prompts for long-context LLMs using the content in your directory"
 readme = "README.md"
 requires-python = ">=3.6"
```

### Comparing `dir2prompt-1.0.5/setup.py` & `dir2prompt-1.0.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dir2prompt",
-    version="1.0.3",
+    version="1.0.6",
     packages=find_packages(),
     package_data={
         "src": ["config.json"],   
     },
     entry_points={
         "console_scripts": [
             "d2p=src.d2p:main"
@@ -37,9 +37,11 @@
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

### Comparing `dir2prompt-1.0.5/src/config.json` & `dir2prompt-1.0.6/src/config.json`

 * *Files identical despite different names*

### Comparing `dir2prompt-1.0.5/src/d2p.py` & `dir2prompt-1.0.6/src/d2p.py`

 * *Files identical despite different names*
