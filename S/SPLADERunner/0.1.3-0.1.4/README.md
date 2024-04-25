# Comparing `tmp/SPLADERunner-0.1.3.tar.gz` & `tmp/SPLADERunner-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SPLADERunner-0.1.3.tar", last modified: Sun Mar 17 03:54:01 2024, max compression
+gzip compressed data, was "SPLADERunner-0.1.4.tar", last modified: Thu Apr 25 04:50:57 2024, max compression
```

## Comparing `SPLADERunner-0.1.3.tar` & `SPLADERunner-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 prithivida   (501) staff       (20)        0 2024-03-17 03:54:01.108856 SPLADERunner-0.1.3/
--rw-r--r--   0 prithivida   (501) staff       (20)     4684 2024-03-17 03:54:01.108735 SPLADERunner-0.1.3/PKG-INFO
--rw-r--r--   0 prithivida   (501) staff       (20)     4127 2024-02-17 05:49:13.000000 SPLADERunner-0.1.3/README.md
-drwxr-xr-x   0 prithivida   (501) staff       (20)        0 2024-03-17 03:54:01.108045 SPLADERunner-0.1.3/SPLADERunner.egg-info/
--rw-r--r--   0 prithivida   (501) staff       (20)     4684 2024-03-17 03:54:01.000000 SPLADERunner-0.1.3/SPLADERunner.egg-info/PKG-INFO
--rw-r--r--   0 prithivida   (501) staff       (20)      270 2024-03-17 03:54:01.000000 SPLADERunner-0.1.3/SPLADERunner.egg-info/SOURCES.txt
--rw-r--r--   0 prithivida   (501) staff       (20)        1 2024-03-17 03:54:01.000000 SPLADERunner-0.1.3/SPLADERunner.egg-info/dependency_links.txt
--rw-r--r--   0 prithivida   (501) staff       (20)       47 2024-03-17 03:54:01.000000 SPLADERunner-0.1.3/SPLADERunner.egg-info/requires.txt
--rw-r--r--   0 prithivida   (501) staff       (20)       13 2024-03-17 03:54:01.000000 SPLADERunner-0.1.3/SPLADERunner.egg-info/top_level.txt
--rw-r--r--   0 prithivida   (501) staff       (20)       38 2024-03-17 03:54:01.108899 SPLADERunner-0.1.3/setup.cfg
--rw-r--r--   0 prithivida   (501) staff       (20)      882 2024-03-17 03:52:58.000000 SPLADERunner-0.1.3/setup.py
-drwxr-xr-x   0 prithivida   (501) staff       (20)        0 2024-03-17 03:54:01.108554 SPLADERunner-0.1.3/spladerunner/
--rw-r--r--   0 prithivida   (501) staff       (20)      181 2024-03-17 03:52:44.000000 SPLADERunner-0.1.3/spladerunner/Config.py
--rw-r--r--   0 prithivida   (501) staff       (20)     6765 2024-02-21 10:54:20.000000 SPLADERunner-0.1.3/spladerunner/Expander.py
--rw-r--r--   0 prithivida   (501) staff       (20)       30 2024-02-16 16:58:15.000000 SPLADERunner-0.1.3/spladerunner/__init__.py
+drwxr-xr-x   0 prithivida   (501) staff       (20)        0 2024-04-25 04:50:57.901768 SPLADERunner-0.1.4/
+-rw-r--r--   0 prithivida   (501) staff       (20)     4684 2024-04-25 04:50:57.901654 SPLADERunner-0.1.4/PKG-INFO
+-rw-r--r--   0 prithivida   (501) staff       (20)     4127 2024-02-17 05:49:13.000000 SPLADERunner-0.1.4/README.md
+drwxr-xr-x   0 prithivida   (501) staff       (20)        0 2024-04-25 04:50:57.900923 SPLADERunner-0.1.4/SPLADERunner.egg-info/
+-rw-r--r--   0 prithivida   (501) staff       (20)     4684 2024-04-25 04:50:57.000000 SPLADERunner-0.1.4/SPLADERunner.egg-info/PKG-INFO
+-rw-r--r--   0 prithivida   (501) staff       (20)      270 2024-04-25 04:50:57.000000 SPLADERunner-0.1.4/SPLADERunner.egg-info/SOURCES.txt
+-rw-r--r--   0 prithivida   (501) staff       (20)        1 2024-04-25 04:50:57.000000 SPLADERunner-0.1.4/SPLADERunner.egg-info/dependency_links.txt
+-rw-r--r--   0 prithivida   (501) staff       (20)       47 2024-04-25 04:50:57.000000 SPLADERunner-0.1.4/SPLADERunner.egg-info/requires.txt
+-rw-r--r--   0 prithivida   (501) staff       (20)       13 2024-04-25 04:50:57.000000 SPLADERunner-0.1.4/SPLADERunner.egg-info/top_level.txt
+-rw-r--r--   0 prithivida   (501) staff       (20)       38 2024-04-25 04:50:57.901806 SPLADERunner-0.1.4/setup.cfg
+-rw-r--r--   0 prithivida   (501) staff       (20)      882 2024-04-25 04:50:03.000000 SPLADERunner-0.1.4/setup.py
+drwxr-xr-x   0 prithivida   (501) staff       (20)        0 2024-04-25 04:50:57.901381 SPLADERunner-0.1.4/spladerunner/
+-rw-r--r--   0 prithivida   (501) staff       (20)      196 2024-04-25 04:49:03.000000 SPLADERunner-0.1.4/spladerunner/Config.py
+-rw-r--r--   0 prithivida   (501) staff       (20)     6765 2024-02-21 10:54:20.000000 SPLADERunner-0.1.4/spladerunner/Expander.py
+-rw-r--r--   0 prithivida   (501) staff       (20)       30 2024-02-16 16:58:15.000000 SPLADERunner-0.1.4/spladerunner/__init__.py
```

### Comparing `SPLADERunner-0.1.3/PKG-INFO` & `SPLADERunner-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SPLADERunner
-Version: 0.1.3
+Version: 0.1.4
 Summary: Ultralight and Fast wrapper for the independent implementation of SPLADE++ models for your search & retrieval pipelines. Models and Library created by Prithivi Da, For PRs and Collaboration to checkout the readme.
 Home-page: https://github.com/PrithivirajDamodaran/SPLADERunner
 Author: Prithivi Da
 Author-email: 
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `SPLADERunner-0.1.3/README.md` & `SPLADERunner-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `SPLADERunner-0.1.3/SPLADERunner.egg-info/PKG-INFO` & `SPLADERunner-0.1.4/SPLADERunner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SPLADERunner
-Version: 0.1.3
+Version: 0.1.4
 Summary: Ultralight and Fast wrapper for the independent implementation of SPLADE++ models for your search & retrieval pipelines. Models and Library created by Prithivi Da, For PRs and Collaboration to checkout the readme.
 Home-page: https://github.com/PrithivirajDamodaran/SPLADERunner
 Author: Prithivi Da
 Author-email: 
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `SPLADERunner-0.1.3/setup.py` & `SPLADERunner-0.1.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='SPLADERunner', 
-    version='0.1.3', 
+    version='0.1.4', 
     packages=find_packages(),
     install_requires=[
         'tokenizers',
         'onnxruntime-gpu',
         'numpy',
         'requests',
         'tqdm'
```

### Comparing `SPLADERunner-0.1.3/spladerunner/Expander.py` & `SPLADERunner-0.1.4/spladerunner/Expander.py`

 * *Files identical despite different names*

