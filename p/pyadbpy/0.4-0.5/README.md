# Comparing `tmp/pyadbpy-0.4.tar.gz` & `tmp/pyadbpy-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyadbpy-0.4.tar", last modified: Thu Apr 25 16:01:08 2024, max compression
+gzip compressed data, was "pyadbpy-0.5.tar", last modified: Thu Apr 25 16:10:39 2024, max compression
```

## Comparing `pyadbpy-0.4.tar` & `pyadbpy-0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:01:08.031681 pyadbpy-0.4/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-25 16:01:08.031681 pyadbpy-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-25 16:01:03.000000 pyadbpy-0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:01:08.031681 pyadbpy-0.4/pyadbpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-25 16:01:08.000000 pyadbpy-0.4/pyadbpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-25 16:01:08.000000 pyadbpy-0.4/pyadbpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:01:08.000000 pyadbpy-0.4/pyadbpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:01:08.000000 pyadbpy-0.4/pyadbpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 16:01:08.031681 pyadbpy-0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-25 16:01:03.000000 pyadbpy-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:10:39.316490 pyadbpy-0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-25 16:10:39.316490 pyadbpy-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-25 16:10:34.000000 pyadbpy-0.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:10:39.316490 pyadbpy-0.5/pyadbpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-25 16:10:39.000000 pyadbpy-0.5/pyadbpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-25 16:10:39.000000 pyadbpy-0.5/pyadbpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:10:39.000000 pyadbpy-0.5/pyadbpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:10:39.000000 pyadbpy-0.5/pyadbpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 16:10:39.316490 pyadbpy-0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-25 16:10:34.000000 pyadbpy-0.5/setup.py
```

### Comparing `pyadbpy-0.4/setup.py` & `pyadbpy-0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.rst", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='pyadbpy',
-    version='0.4',
+    version='0.5',
     packages=find_packages(),
     author='termuxdev314',
     author_email='termuxdev314@gmail.com',
     description='Ein Modul für ADB Operationen.',
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url='https://github.com/termuxdev314/adbpy',
```

