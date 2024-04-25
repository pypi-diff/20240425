# Comparing `tmp/sandal-0.1.0a1.tar.gz` & `tmp/sandal-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sandal-0.1.0a1.tar", last modified: Tue Mar 19 20:51:56 2024, max compression
+gzip compressed data, was "sandal-0.1.0a2.tar", last modified: Thu Apr 25 01:02:33 2024, max compression
```

## Comparing `sandal-0.1.0a1.tar` & `sandal-0.1.0a2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:51:56.577277 sandal-0.1.0a1/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-19 20:51:44.000000 sandal-0.1.0a1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-19 20:51:44.000000 sandal-0.1.0a1/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-19 20:51:44.000000 sandal-0.1.0a1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-19 20:51:44.000000 sandal-0.1.0a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-19 20:51:44.000000 sandal-0.1.0a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-03-19 20:51:56.577277 sandal-0.1.0a1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:51:56.573277 sandal-0.1.0a1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-19 20:51:44.000000 sandal-0.1.0a1/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-03-19 20:51:44.000000 sandal-0.1.0a1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-19 20:51:44.000000 sandal-0.1.0a1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-19 20:51:44.000000 sandal-0.1.0a1/docs/notebook.rst
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-03-19 20:51:44.000000 sandal-0.1.0a1/justfile
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-03-19 20:51:44.000000 sandal-0.1.0a1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:51:56.573277 sandal-0.1.0a1/sandal/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-19 20:51:44.000000 sandal-0.1.0a1/sandal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-03-19 20:51:44.000000 sandal-0.1.0a1/sandal/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-03-19 20:51:44.000000 sandal-0.1.0a1/sandal/loghelper.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-19 20:51:44.000000 sandal-0.1.0a1/sandal/notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-19 20:51:44.000000 sandal-0.1.0a1/sandal/root.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:51:56.573277 sandal-0.1.0a1/sandal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-03-19 20:51:56.000000 sandal-0.1.0a1/sandal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-03-19 20:51:56.000000 sandal-0.1.0a1/sandal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 20:51:56.000000 sandal-0.1.0a1/sandal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-19 20:51:56.000000 sandal-0.1.0a1/sandal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-19 20:51:56.000000 sandal-0.1.0a1/sandal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 20:51:56.577277 sandal-0.1.0a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:02:33.427831 sandal-0.1.0a2/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-25 01:02:28.000000 sandal-0.1.0a2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-25 01:02:28.000000 sandal-0.1.0a2/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-25 01:02:28.000000 sandal-0.1.0a2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-25 01:02:28.000000 sandal-0.1.0a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-25 01:02:28.000000 sandal-0.1.0a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-25 01:02:33.423831 sandal-0.1.0a2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:02:33.419831 sandal-0.1.0a2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-25 01:02:28.000000 sandal-0.1.0a2/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-25 01:02:28.000000 sandal-0.1.0a2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-25 01:02:28.000000 sandal-0.1.0a2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-25 01:02:28.000000 sandal-0.1.0a2/docs/notebook.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-25 01:02:28.000000 sandal-0.1.0a2/justfile
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-25 01:02:28.000000 sandal-0.1.0a2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:02:33.423831 sandal-0.1.0a2/sandal/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-25 01:02:28.000000 sandal-0.1.0a2/sandal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-25 01:02:28.000000 sandal-0.1.0a2/sandal/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-25 01:02:28.000000 sandal-0.1.0a2/sandal/loghelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-25 01:02:28.000000 sandal-0.1.0a2/sandal/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-25 01:02:28.000000 sandal-0.1.0a2/sandal/root.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:02:33.423831 sandal-0.1.0a2/sandal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-25 01:02:33.000000 sandal-0.1.0a2/sandal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-25 01:02:33.000000 sandal-0.1.0a2/sandal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 01:02:33.000000 sandal-0.1.0a2/sandal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-25 01:02:33.000000 sandal-0.1.0a2/sandal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 01:02:33.000000 sandal-0.1.0a2/sandal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 01:02:33.427831 sandal-0.1.0a2/setup.cfg
```

### Comparing `sandal-0.1.0a1/.gitignore` & `sandal-0.1.0a2/.gitignore`

 * *Files identical despite different names*

### Comparing `sandal-0.1.0a1/LICENSE.md` & `sandal-0.1.0a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sandal-0.1.0a1/PKG-INFO` & `sandal-0.1.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sandal
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: Lightweight bootstrapping for project scripts
 Author-email: Michael Ekstrand <mdekstrand@drexel.edu>
 License: Copyright (c) 2023 Michael D. Ekstrand
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `sandal-0.1.0a1/docs/conf.py` & `sandal-0.1.0a2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sandal-0.1.0a1/justfile` & `sandal-0.1.0a2/justfile`

 * *Files identical despite different names*

### Comparing `sandal-0.1.0a1/pyproject.toml` & `sandal-0.1.0a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sandal-0.1.0a1/sandal/cli.py` & `sandal-0.1.0a2/sandal/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import logging
 import sys
 from pathlib import Path
 
 import progress_api
 from colorlog import ColoredFormatter
 from enlighten import Manager
+from progress_api.backends.enlighten import EnlightenProgressBackend
 
 from .loghelper import Verbosity, vrb_to_level
 
 term_fmt = ColoredFormatter(
     "[%(blue)s%(asctime)s%(reset)s] %(log_color)s%(levelname)-8s%(reset)s %(cyan)s%(logger)s %(blue)s%(message)s",  # noqa: E501
     datefmt="%H:%M:%S",
     reset=True,
@@ -64,8 +65,8 @@
         fh.setLevel(file_level)
         fh.setFormatter(file_fmt)
         root.addHandler(fh)
     else:
         root.setLevel(term_level)
 
     emgr = Manager(stream=sys.stderr)
-    progress_api.set_backend("enlighten", emgr)
+    progress_api.set_backend(EnlightenProgressBackend, emgr)
```

### Comparing `sandal-0.1.0a1/sandal/notebook.py` & `sandal-0.1.0a2/sandal/notebook.py`

 * *Files identical despite different names*

### Comparing `sandal-0.1.0a1/sandal.egg-info/PKG-INFO` & `sandal-0.1.0a2/sandal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sandal
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: Lightweight bootstrapping for project scripts
 Author-email: Michael Ekstrand <mdekstrand@drexel.edu>
 License: Copyright (c) 2023 Michael D. Ekstrand
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

