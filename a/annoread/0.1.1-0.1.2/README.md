# Comparing `tmp/annoread-0.1.1.tar.gz` & `tmp/annoread-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "annoread-0.1.1.tar", last modified: Thu Apr 25 09:33:22 2024, max compression
+gzip compressed data, was "annoread-0.1.2.tar", last modified: Thu Apr 25 10:36:29 2024, max compression
```

## Comparing `annoread-0.1.1.tar` & `annoread-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 fanghl    (1000) fanghl    (1000)        0 2024-04-25 09:33:22.792027 annoread-0.1.1/
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)      746 2024-04-25 09:33:22.791027 annoread-0.1.1/PKG-INFO
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)      286 2024-04-18 00:57:03.000000 annoread-0.1.1/README.md
-drwxr-xr-x   0 fanghl    (1000) fanghl    (1000)        0 2024-04-25 09:33:22.791027 annoread-0.1.1/annoread/
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)       94 2024-04-25 09:28:04.000000 annoread-0.1.1/annoread/__init__.py
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)    16786 2024-04-19 07:17:59.000000 annoread-0.1.1/annoread/annodata.py
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)    13908 2024-04-25 09:10:19.000000 annoread-0.1.1/annoread/annoread.py
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)     4931 2024-04-18 00:57:03.000000 annoread-0.1.1/annoread/assignread.py
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)     3722 2024-04-18 00:57:03.000000 annoread-0.1.1/annoread/countmtx.py
-drwxr-xr-x   0 fanghl    (1000) fanghl    (1000)        0 2024-04-25 09:33:22.791027 annoread-0.1.1/annoread.egg-info/
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)      746 2024-04-25 09:33:22.000000 annoread-0.1.1/annoread.egg-info/PKG-INFO
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)      334 2024-04-25 09:33:22.000000 annoread-0.1.1/annoread.egg-info/SOURCES.txt
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)        1 2024-04-25 09:33:22.000000 annoread-0.1.1/annoread.egg-info/dependency_links.txt
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)       42 2024-04-25 09:33:22.000000 annoread-0.1.1/annoread.egg-info/entry_points.txt
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)       16 2024-04-25 09:33:22.000000 annoread-0.1.1/annoread.egg-info/requires.txt
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)        9 2024-04-25 09:33:22.000000 annoread-0.1.1/annoread.egg-info/top_level.txt
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)      633 2024-04-25 09:33:11.000000 annoread-0.1.1/pyproject.toml
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)       38 2024-04-25 09:33:22.792027 annoread-0.1.1/setup.cfg
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)       69 2024-04-25 08:59:46.000000 annoread-0.1.1/setup.py
+drwxr-xr-x   0 fanghl    (1000) fanghl    (1000)        0 2024-04-25 10:36:29.071227 annoread-0.1.2/
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)      746 2024-04-25 10:36:29.071227 annoread-0.1.2/PKG-INFO
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)      286 2024-04-18 00:57:03.000000 annoread-0.1.2/README.md
+drwxr-xr-x   0 fanghl    (1000) fanghl    (1000)        0 2024-04-25 10:36:29.070227 annoread-0.1.2/annoread/
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)       94 2024-04-25 09:28:04.000000 annoread-0.1.2/annoread/__init__.py
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)    16786 2024-04-19 07:17:59.000000 annoread-0.1.2/annoread/annodata.py
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)    13908 2024-04-25 09:10:19.000000 annoread-0.1.2/annoread/annoread.py
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)     4932 2024-04-25 10:26:41.000000 annoread-0.1.2/annoread/assignread.py
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)     3723 2024-04-25 10:25:47.000000 annoread-0.1.2/annoread/countmtx.py
+drwxr-xr-x   0 fanghl    (1000) fanghl    (1000)        0 2024-04-25 10:36:29.070227 annoread-0.1.2/annoread.egg-info/
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)      746 2024-04-25 10:36:29.000000 annoread-0.1.2/annoread.egg-info/PKG-INFO
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)      334 2024-04-25 10:36:29.000000 annoread-0.1.2/annoread.egg-info/SOURCES.txt
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)        1 2024-04-25 10:36:29.000000 annoread-0.1.2/annoread.egg-info/dependency_links.txt
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)       51 2024-04-25 10:36:29.000000 annoread-0.1.2/annoread.egg-info/entry_points.txt
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)       16 2024-04-25 10:36:29.000000 annoread-0.1.2/annoread.egg-info/requires.txt
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)        9 2024-04-25 10:36:29.000000 annoread-0.1.2/annoread.egg-info/top_level.txt
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)      642 2024-04-25 10:36:15.000000 annoread-0.1.2/pyproject.toml
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)       38 2024-04-25 10:36:29.071227 annoread-0.1.2/setup.cfg
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)       69 2024-04-25 08:59:46.000000 annoread-0.1.2/setup.py
```

### Comparing `annoread-0.1.1/PKG-INFO` & `annoread-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annoread
-Version: 0.1.1
+Version: 0.1.2
 Summary: annotate read from mapping data, and assign the multiple mapped reads, and count
 Author-email: Hailing Fang <benjaminfang.ol@outlook.com>
 Project-URL: Homepage, https://github.com/benjaminfang/annoread
 Keywords: read annotation,read assignment,read count
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `annoread-0.1.1/annoread/annodata.py` & `annoread-0.1.2/annoread/annodata.py`

 * *Files identical despite different names*

### Comparing `annoread-0.1.1/annoread/annoread.py` & `annoread-0.1.2/annoread/annoread.py`

 * *Files identical despite different names*

### Comparing `annoread-0.1.1/annoread/assignread.py` & `annoread-0.1.2/annoread/assignread.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     equal: the read is assign to a feautre randomly in equal probability.
     proportion: the read is assign to a feature randomly in probability proportional
         to unique read of each features.
     largest: The read is assign to the feature which have the largest amount unique
         read.
 """
 import argparse
-from annodata import ANNOREAD_DATA
+from .annodata import ANNOREAD_DATA
 
 
 def getargs():
     parser = argparse.ArgumentParser()
     parser.add_argument("anno_file", help="annoread file")
     parser.add_argument("--out", "-O", help="output file name", default="out")
     parser.add_argument("--gene_name",
```

### Comparing `annoread-0.1.1/annoread/countmtx.py` & `annoread-0.1.2/annoread/countmtx.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 .
 .
 """
 
 import numpy as np
 import os
 import argparse
-from annodata import ANNOREAD_DATA
+from .annodata import ANNOREAD_DATA
 
 
 def getargs():
     parser = argparse.ArgumentParser()
     parser.add_argument("anno_files", help="annoread output file", nargs="+")
     parser.add_argument("--out", "-O", help="output file name", default="out")
     parser.add_argument("--count_level", choices={"gene_name", "gene_id", "transcript_id"},
```

### Comparing `annoread-0.1.1/annoread.egg-info/PKG-INFO` & `annoread-0.1.2/annoread.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annoread
-Version: 0.1.1
+Version: 0.1.2
 Summary: annotate read from mapping data, and assign the multiple mapped reads, and count
 Author-email: Hailing Fang <benjaminfang.ol@outlook.com>
 Project-URL: Homepage, https://github.com/benjaminfang/annoread
 Keywords: read annotation,read assignment,read count
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `annoread-0.1.1/pyproject.toml` & `annoread-0.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "annoread"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
   "biobrary==0.1.4",
 ]
 requires-python = ">=3.11"
 authors = [
   {name = "Hailing Fang", email = "benjaminfang.ol@outlook.com"},
 ]
@@ -19,9 +19,9 @@
   "Programming Language :: Python :: 3"
 ]
 
 [project.urls]
 Homepage = "https://github.com/benjaminfang/annoread"
 
 [project.scripts]
-annread = "annoread:main"
+annread = "annoread.annoread:main"
```

