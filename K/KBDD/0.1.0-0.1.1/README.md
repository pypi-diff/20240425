# Comparing `tmp/KBDD-0.1.0.tar.gz` & `tmp/KBDD-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KBDD-0.1.0.tar", last modified: Thu Apr 25 09:31:14 2024, max compression
+gzip compressed data, was "KBDD-0.1.1.tar", last modified: Thu Apr 25 10:16:14 2024, max compression
```

## Comparing `KBDD-0.1.0.tar` & `KBDD-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,11 @@
-drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 09:31:14.853022 KBDD-0.1.0/
-drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 09:31:14.852291 KBDD-0.1.0/KBDD.egg-info/
--rw-r--r--   0 liaochenpo   (501) staff       (20)     1133 2024-04-25 09:31:14.000000 KBDD-0.1.0/KBDD.egg-info/PKG-INFO
--rw-r--r--   0 liaochenpo   (501) staff       (20)      169 2024-04-25 09:31:14.000000 KBDD-0.1.0/KBDD.egg-info/SOURCES.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)        1 2024-04-25 09:31:14.000000 KBDD-0.1.0/KBDD.egg-info/dependency_links.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)       62 2024-04-25 09:31:14.000000 KBDD-0.1.0/KBDD.egg-info/requires.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)        1 2024-04-25 09:31:14.000000 KBDD-0.1.0/KBDD.egg-info/top_level.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)     1068 2024-04-25 09:12:48.000000 KBDD-0.1.0/LICENSE.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)     1133 2024-04-25 09:31:14.852733 KBDD-0.1.0/PKG-INFO
--rw-r--r--   0 liaochenpo   (501) staff       (20)      342 2024-04-25 09:04:43.000000 KBDD-0.1.0/README.md
--rw-r--r--   0 liaochenpo   (501) staff       (20)       38 2024-04-25 09:31:14.853080 KBDD-0.1.0/setup.cfg
--rw-r--r--   0 liaochenpo   (501) staff       (20)      943 2024-04-25 09:31:08.000000 KBDD-0.1.0/setup.py
+drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 10:16:14.342362 KBDD-0.1.1/
+drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 10:16:14.341900 KBDD-0.1.1/KBDD.egg-info/
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      966 2024-04-25 10:16:14.000000 KBDD-0.1.1/KBDD.egg-info/PKG-INFO
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      142 2024-04-25 10:16:14.000000 KBDD-0.1.1/KBDD.egg-info/SOURCES.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)        1 2024-04-25 10:16:14.000000 KBDD-0.1.1/KBDD.egg-info/dependency_links.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)        1 2024-04-25 10:16:14.000000 KBDD-0.1.1/KBDD.egg-info/top_level.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     1068 2024-04-25 09:12:48.000000 KBDD-0.1.1/LICENSE.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      966 2024-04-25 10:16:14.342118 KBDD-0.1.1/PKG-INFO
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      342 2024-04-25 09:04:43.000000 KBDD-0.1.1/README.md
+-rw-r--r--   0 liaochenpo   (501) staff       (20)       38 2024-04-25 10:16:14.342414 KBDD-0.1.1/setup.cfg
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      775 2024-04-25 10:16:09.000000 KBDD-0.1.1/setup.py
```

### Comparing `KBDD-0.1.0/KBDD.egg-info/PKG-INFO` & `KBDD-0.1.1/KBDD.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,23 @@
 Metadata-Version: 2.1
 Name: KBDD
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for KBDD: a knowledge-based and data-driven method for genetic network construction
 Author: Chen-Po Liao
 Author-email: liaochenpo@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: numpy
-Requires-Dist: scipy
-Requires-Dist: networkx
-Requires-Dist: itertools
-Requires-Dist: random
-Requires-Dist: matplotlib.pyplot
-Requires-Dist: scipy
 
 # KBDD: a knowledge-based and data-driven method for genetic network construction
 
 Updated: February 14 2024
 
 This repository contains code to reproduce the results of simulation and applications in
```

### Comparing `KBDD-0.1.0/LICENSE.txt` & `KBDD-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `KBDD-0.1.0/PKG-INFO` & `KBDD-0.1.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,23 @@
 Metadata-Version: 2.1
 Name: KBDD
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for KBDD: a knowledge-based and data-driven method for genetic network construction
 Author: Chen-Po Liao
 Author-email: liaochenpo@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: numpy
-Requires-Dist: scipy
-Requires-Dist: networkx
-Requires-Dist: itertools
-Requires-Dist: random
-Requires-Dist: matplotlib.pyplot
-Requires-Dist: scipy
 
 # KBDD: a knowledge-based and data-driven method for genetic network construction
 
 Updated: February 14 2024
 
 This repository contains code to reproduce the results of simulation and applications in
```

