# Comparing `tmp/nue-0.0.1.tar.gz` & `tmp/nue-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nue-0.0.1.tar", last modified: Thu Apr 25 06:11:54 2024, max compression
+gzip compressed data, was "nue-0.0.2.tar", last modified: Thu Apr 25 06:25:57 2024, max compression
```

## Comparing `nue-0.0.1.tar` & `nue-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 juanvera   (501) staff       (20)        0 2024-04-25 06:11:54.459020 nue-0.0.1/
--rw-r--r--   0 juanvera   (501) staff       (20)     1062 2024-04-22 16:56:55.000000 nue-0.0.1/LICENSE
--rw-r--r--   0 juanvera   (501) staff       (20)     1776 2024-04-25 06:11:54.458815 nue-0.0.1/PKG-INFO
--rw-r--r--   0 juanvera   (501) staff       (20)     1212 2024-04-25 01:49:56.000000 nue-0.0.1/README.md
-drwxr-xr-x   0 juanvera   (501) staff       (20)        0 2024-04-25 06:11:54.457983 nue-0.0.1/nue/
--rw-r--r--   0 juanvera   (501) staff       (20)        0 2024-04-22 17:43:10.000000 nue-0.0.1/nue/__init__.py
-drwxr-xr-x   0 juanvera   (501) staff       (20)        0 2024-04-25 06:11:54.458567 nue-0.0.1/nue.egg-info/
--rw-r--r--   0 juanvera   (501) staff       (20)     1776 2024-04-25 06:11:54.000000 nue-0.0.1/nue.egg-info/PKG-INFO
--rw-r--r--   0 juanvera   (501) staff       (20)      176 2024-04-25 06:11:54.000000 nue-0.0.1/nue.egg-info/SOURCES.txt
--rw-r--r--   0 juanvera   (501) staff       (20)        1 2024-04-25 06:11:54.000000 nue-0.0.1/nue.egg-info/dependency_links.txt
--rw-r--r--   0 juanvera   (501) staff       (20)       24 2024-04-25 06:11:54.000000 nue-0.0.1/nue.egg-info/requires.txt
--rw-r--r--   0 juanvera   (501) staff       (20)        4 2024-04-25 06:11:54.000000 nue-0.0.1/nue.egg-info/top_level.txt
--rw-r--r--   0 juanvera   (501) staff       (20)       38 2024-04-25 06:11:54.459062 nue-0.0.1/setup.cfg
--rw-r--r--   0 juanvera   (501) staff       (20)      862 2024-04-25 06:11:28.000000 nue-0.0.1/setup.py
+drwxr-xr-x   0 juanvera   (501) staff       (20)        0 2024-04-25 06:25:57.665049 nue-0.0.2/
+-rw-r--r--   0 juanvera   (501) staff       (20)     1062 2024-04-22 16:56:55.000000 nue-0.0.2/LICENSE
+-rw-r--r--   0 juanvera   (501) staff       (20)     1776 2024-04-25 06:25:57.664834 nue-0.0.2/PKG-INFO
+-rw-r--r--   0 juanvera   (501) staff       (20)     1212 2024-04-25 01:49:56.000000 nue-0.0.2/README.md
+drwxr-xr-x   0 juanvera   (501) staff       (20)        0 2024-04-25 06:25:57.663809 nue-0.0.2/nue/
+-rw-r--r--   0 juanvera   (501) staff       (20)       73 2024-04-25 06:23:13.000000 nue-0.0.2/nue/__init__.py
+drwxr-xr-x   0 juanvera   (501) staff       (20)        0 2024-04-25 06:25:57.664552 nue-0.0.2/nue.egg-info/
+-rw-r--r--   0 juanvera   (501) staff       (20)     1776 2024-04-25 06:25:57.000000 nue-0.0.2/nue.egg-info/PKG-INFO
+-rw-r--r--   0 juanvera   (501) staff       (20)      176 2024-04-25 06:25:57.000000 nue-0.0.2/nue.egg-info/SOURCES.txt
+-rw-r--r--   0 juanvera   (501) staff       (20)        1 2024-04-25 06:25:57.000000 nue-0.0.2/nue.egg-info/dependency_links.txt
+-rw-r--r--   0 juanvera   (501) staff       (20)       24 2024-04-25 06:25:57.000000 nue-0.0.2/nue.egg-info/requires.txt
+-rw-r--r--   0 juanvera   (501) staff       (20)        4 2024-04-25 06:25:57.000000 nue-0.0.2/nue.egg-info/top_level.txt
+-rw-r--r--   0 juanvera   (501) staff       (20)       38 2024-04-25 06:25:57.665094 nue-0.0.2/setup.cfg
+-rw-r--r--   0 juanvera   (501) staff       (20)      862 2024-04-25 06:24:35.000000 nue-0.0.2/setup.py
```

### Comparing `nue-0.0.1/LICENSE` & `nue-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nue-0.0.1/PKG-INFO` & `nue-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nue
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Deep Learning Package for Entry Level Tinkerers
 Home-page: https://github.com/vxnuaj/neuo
 Author: vxnuaj
 Author-email: jv.100420@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nue-0.0.1/README.md` & `nue-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nue-0.0.1/nue.egg-info/PKG-INFO` & `nue-0.0.2/nue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nue
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Deep Learning Package for Entry Level Tinkerers
 Home-page: https://github.com/vxnuaj/neuo
 Author: vxnuaj
 Author-email: jv.100420@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nue-0.0.1/setup.py` & `nue-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # setup.py
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
-DEFAULTV = '0.0.1'
+VERSION = '0.0.2'
+DEFAULTV = '0.0.2'
 DESCRIPTION = 'A Deep Learning Package for Entry Level Tinkerers'
 
 setup(
     name='nue',
     version= VERSION,
     default_version= DEFAULTV,
     packages=find_packages(exclude = ['examples']),
```

