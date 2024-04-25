# Comparing `tmp/BioUtensils-0.5.tar.gz` & `tmp/BioUtensils-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BioUtensils-0.5.tar", last modified: Fri Apr 19 14:46:51 2024, max compression
+gzip compressed data, was "BioUtensils-0.6.tar", last modified: Thu Apr 25 07:49:38 2024, max compression
```

## Comparing `BioUtensils-0.5.tar` & `BioUtensils-0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:46:51.736076 BioUtensils-0.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:46:51.732076 BioUtensils-0.5/BioUtensils/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-19 14:46:42.000000 BioUtensils-0.5/BioUtensils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-19 14:46:42.000000 BioUtensils-0.5/BioUtensils/normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-19 14:46:42.000000 BioUtensils-0.5/BioUtensils/rgb_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:46:51.732076 BioUtensils-0.5/BioUtensils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-19 14:46:51.000000 BioUtensils-0.5/BioUtensils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-19 14:46:51.000000 BioUtensils-0.5/BioUtensils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:46:51.000000 BioUtensils-0.5/BioUtensils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-19 14:46:51.000000 BioUtensils-0.5/BioUtensils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 14:46:51.000000 BioUtensils-0.5/BioUtensils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-19 14:46:51.736076 BioUtensils-0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-19 14:46:42.000000 BioUtensils-0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 14:46:51.736076 BioUtensils-0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-19 14:46:49.000000 BioUtensils-0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:49:38.193354 BioUtensils-0.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:49:38.189354 BioUtensils-0.6/BioUtensils/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-25 07:49:32.000000 BioUtensils-0.6/BioUtensils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-25 07:49:32.000000 BioUtensils-0.6/BioUtensils/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-25 07:49:32.000000 BioUtensils-0.6/BioUtensils/rgb_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:49:38.189354 BioUtensils-0.6/BioUtensils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-25 07:49:38.000000 BioUtensils-0.6/BioUtensils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-25 07:49:38.000000 BioUtensils-0.6/BioUtensils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 07:49:38.000000 BioUtensils-0.6/BioUtensils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-25 07:49:38.000000 BioUtensils-0.6/BioUtensils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 07:49:38.000000 BioUtensils-0.6/BioUtensils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-25 07:49:38.189354 BioUtensils-0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-25 07:49:32.000000 BioUtensils-0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 07:49:38.193354 BioUtensils-0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-25 07:49:36.000000 BioUtensils-0.6/setup.py
```

### Comparing `BioUtensils-0.5/BioUtensils/normalize.py` & `BioUtensils-0.6/BioUtensils/normalize.py`

 * *Files identical despite different names*

### Comparing `BioUtensils-0.5/BioUtensils/rgb_utils.py` & `BioUtensils-0.6/BioUtensils/rgb_utils.py`

 * *Files identical despite different names*

### Comparing `BioUtensils-0.5/setup.py` & `BioUtensils-0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def read_requirements():
     with open('requirements.txt', 'r') as file:
         return [line.strip() for line in file.readlines()]
 
 setup(
     name=package_name,
-    version='0.5',
+    version='0.6',
     packages=find_packages(),
     install_requires=read_requirements(),
     author="Simon Gutwein",
     include_package_data=True,
     author_email="simon.gutwein@ccri.at",
     description="",
     long_description=open('README.md').read(),
```

