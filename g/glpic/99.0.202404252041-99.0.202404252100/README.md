# Comparing `tmp/glpic-99.0.202404252041.tar.gz` & `tmp/glpic-99.0.202404252100.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glpic-99.0.202404252041.tar", last modified: Thu Apr 25 20:41:57 2024, max compression
+gzip compressed data, was "glpic-99.0.202404252100.tar", last modified: Thu Apr 25 21:00:50 2024, max compression
```

## Comparing `glpic-99.0.202404252041.tar` & `glpic-99.0.202404252100.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:41:57.146967 glpic-99.0.202404252041/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-25 20:41:57.146967 glpic-99.0.202404252041/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-25 20:41:43.000000 glpic-99.0.202404252041/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:41:57.146967 glpic-99.0.202404252041/glpic/
--rw-r--r--   0 runner    (1001) docker     (127)    10545 2024-04-25 20:41:43.000000 glpic-99.0.202404252041/glpic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10248 2024-04-25 20:41:43.000000 glpic-99.0.202404252041/glpic/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:41:57.146967 glpic-99.0.202404252041/glpic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-25 20:41:57.000000 glpic-99.0.202404252041/glpic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-25 20:41:57.000000 glpic-99.0.202404252041/glpic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 20:41:57.000000 glpic-99.0.202404252041/glpic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-25 20:41:57.000000 glpic-99.0.202404252041/glpic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 20:41:57.000000 glpic-99.0.202404252041/glpic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 20:41:57.000000 glpic-99.0.202404252041/glpic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 20:41:57.000000 glpic-99.0.202404252041/glpic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 20:41:57.146967 glpic-99.0.202404252041/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-25 20:41:56.000000 glpic-99.0.202404252041/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:00:50.136817 glpic-99.0.202404252100/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-25 21:00:50.136817 glpic-99.0.202404252100/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-25 21:00:30.000000 glpic-99.0.202404252100/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:00:50.136817 glpic-99.0.202404252100/glpic/
+-rw-r--r--   0 runner    (1001) docker     (127)    10545 2024-04-25 21:00:30.000000 glpic-99.0.202404252100/glpic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-04-25 21:00:30.000000 glpic-99.0.202404252100/glpic/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:00:50.136817 glpic-99.0.202404252100/glpic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-25 21:00:50.000000 glpic-99.0.202404252100/glpic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-25 21:00:50.000000 glpic-99.0.202404252100/glpic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 21:00:50.000000 glpic-99.0.202404252100/glpic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-25 21:00:50.000000 glpic-99.0.202404252100/glpic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 21:00:50.000000 glpic-99.0.202404252100/glpic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 21:00:50.000000 glpic-99.0.202404252100/glpic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 21:00:50.000000 glpic-99.0.202404252100/glpic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 21:00:50.136817 glpic-99.0.202404252100/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-25 21:00:49.000000 glpic-99.0.202404252100/setup.py
```

### Comparing `glpic-99.0.202404252041/README.md` & `glpic-99.0.202404252100/README.md`

 * *Files identical despite different names*

### Comparing `glpic-99.0.202404252041/glpic/__init__.py` & `glpic-99.0.202404252100/glpic/__init__.py`

 * *Files identical despite different names*

### Comparing `glpic-99.0.202404252041/glpic/cli.py` & `glpic-99.0.202404252100/glpic/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 from argparse import RawDescriptionHelpFormatter as rawhelp
 from prettytable import PrettyTable
 import os
 import sys
 from glpic import Glpic
-from glpic import error, handle_parameters
+from glpic import error, handle_parameters, info
 
 PARAMHELP = "specify parameter or keyword for rendering (multiple can be specified)"
 
 
 def confirm(message):
     message = f"{message} [y/N]: "
     try:
@@ -64,22 +64,23 @@
     for reservation in args.reservations:
         glpic.delete_reservation(reservation)
 
 
 def update_reservation(args):
     glpic = Glpic(args.url, args.user, args.token, args.debug)
     for reservation in args.reservations:
+        info(f"Updating reservation {reservation}")
         glpic.update_reservation(reservation, overrides=handle_parameters(args.param))
 
 
 def info_computer(args):
     glpic = Glpic(args.url, args.user, args.token, args.debug)
-    info = glpic.info_computer(args.computer, args.full)
-    for key in info:
-        print(f"{key}: {info[key]}")
+    data = glpic.info_computer(args.computer, args.full)
+    for key in data:
+        print(f"{key}: {data[key]}")
 
 
 def list_computers(args):
     glpic = Glpic(args.url, args.user, args.token, args.debug)
     computerstable = PrettyTable(["Id", "Name", "Group", "Serial", "Comment"])
     for computer in glpic.list_computers(overrides=handle_parameters(args.param)):
         _id, group, = computer['id'], computer['groups_id_tech']
```

### Comparing `glpic-99.0.202404252041/setup.py` & `glpic-99.0.202404252100/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 description = 'Glpic wrapper'
 long_description = description
 if os.path.exists('README.rst'):
     long_description = open('README.rst').read()
 
 setup(
     name='glpic',
-    version='99.0.202404252041',
+    version='99.0.202404252100',
     include_package_data=True,
     packages=find_packages(),
     zip_safe=False,
     description=description,
     long_description=long_description,
     url='http://github.com/karmab/glpic',
     author='Karim Boumedhel',
```

