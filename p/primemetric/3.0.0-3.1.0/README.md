# Comparing `tmp/primemetric-3.0.0.tar.gz` & `tmp/primemetric-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "primemetric-3.0.0.tar", last modified: Wed Apr 24 23:10:26 2024, max compression
+gzip compressed data, was "primemetric-3.1.0.tar", last modified: Wed Apr 24 23:17:38 2024, max compression
```

## Comparing `primemetric-3.0.0.tar` & `primemetric-3.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 andrewlevin   (501) staff       (20)        0 2024-04-24 23:10:26.150689 primemetric-3.0.0/
--rw-r--r--   0 andrewlevin   (501) staff       (20)     1081 2024-04-23 01:04:50.000000 primemetric-3.0.0/LICENSE.txt
--rw-r--r--   0 andrewlevin   (501) staff       (20)     4436 2024-04-24 23:10:26.150502 primemetric-3.0.0/PKG-INFO
--rw-r--r--   0 andrewlevin   (501) staff       (20)     1811 2024-04-23 21:38:16.000000 primemetric-3.0.0/README.md
--rw-r--r--   0 andrewlevin   (501) staff       (20)     6732 2024-04-24 21:59:20.000000 primemetric-3.0.0/pyproject.toml
--rw-r--r--   0 andrewlevin   (501) staff       (20)       38 2024-04-24 23:10:26.150740 primemetric-3.0.0/setup.cfg
-drwxr-xr-x   0 andrewlevin   (501) staff       (20)        0 2024-04-24 23:10:26.147946 primemetric-3.0.0/src/
-drwxr-xr-x   0 andrewlevin   (501) staff       (20)        0 2024-04-24 23:10:26.149021 primemetric-3.0.0/src/metric/
--rw-r--r--   0 andrewlevin   (501) staff       (20)      110 2024-04-23 23:06:10.000000 primemetric-3.0.0/src/metric/__init__.py
--rw-r--r--   0 andrewlevin   (501) staff       (20)      405 2024-04-24 23:07:52.000000 primemetric-3.0.0/src/metric/metric.py
-drwxr-xr-x   0 andrewlevin   (501) staff       (20)        0 2024-04-24 23:10:26.150165 primemetric-3.0.0/src/primemetric.egg-info/
--rw-r--r--   0 andrewlevin   (501) staff       (20)     4436 2024-04-24 23:10:26.000000 primemetric-3.0.0/src/primemetric.egg-info/PKG-INFO
--rw-r--r--   0 andrewlevin   (501) staff       (20)      337 2024-04-24 23:10:26.000000 primemetric-3.0.0/src/primemetric.egg-info/SOURCES.txt
--rw-r--r--   0 andrewlevin   (501) staff       (20)        1 2024-04-24 23:10:26.000000 primemetric-3.0.0/src/primemetric.egg-info/dependency_links.txt
--rw-r--r--   0 andrewlevin   (501) staff       (20)       39 2024-04-24 23:10:26.000000 primemetric-3.0.0/src/primemetric.egg-info/entry_points.txt
--rw-r--r--   0 andrewlevin   (501) staff       (20)       50 2024-04-24 23:10:26.000000 primemetric-3.0.0/src/primemetric.egg-info/requires.txt
--rw-r--r--   0 andrewlevin   (501) staff       (20)        7 2024-04-24 23:10:26.000000 primemetric-3.0.0/src/primemetric.egg-info/top_level.txt
-drwxr-xr-x   0 andrewlevin   (501) staff       (20)        0 2024-04-24 23:10:26.149986 primemetric-3.0.0/tests/
--rw-r--r--   0 andrewlevin   (501) staff       (20)      428 2024-04-24 23:05:13.000000 primemetric-3.0.0/tests/test_metric.py
+drwxr-xr-x   0 andrewlevin   (501) staff       (20)        0 2024-04-24 23:17:38.057025 primemetric-3.1.0/
+-rw-r--r--   0 andrewlevin   (501) staff       (20)     1081 2024-04-23 01:04:50.000000 primemetric-3.1.0/LICENSE.txt
+-rw-r--r--   0 andrewlevin   (501) staff       (20)     4436 2024-04-24 23:17:38.056842 primemetric-3.1.0/PKG-INFO
+-rw-r--r--   0 andrewlevin   (501) staff       (20)     1811 2024-04-23 21:38:16.000000 primemetric-3.1.0/README.md
+-rw-r--r--   0 andrewlevin   (501) staff       (20)     6732 2024-04-24 23:17:06.000000 primemetric-3.1.0/pyproject.toml
+-rw-r--r--   0 andrewlevin   (501) staff       (20)       38 2024-04-24 23:17:38.057078 primemetric-3.1.0/setup.cfg
+drwxr-xr-x   0 andrewlevin   (501) staff       (20)        0 2024-04-24 23:17:38.054787 primemetric-3.1.0/src/
+drwxr-xr-x   0 andrewlevin   (501) staff       (20)        0 2024-04-24 23:17:38.055469 primemetric-3.1.0/src/metric/
+-rw-r--r--   0 andrewlevin   (501) staff       (20)      110 2024-04-23 23:06:10.000000 primemetric-3.1.0/src/metric/__init__.py
+-rw-r--r--   0 andrewlevin   (501) staff       (20)      405 2024-04-24 23:07:52.000000 primemetric-3.1.0/src/metric/metric.py
+drwxr-xr-x   0 andrewlevin   (501) staff       (20)        0 2024-04-24 23:17:38.056497 primemetric-3.1.0/src/primemetric.egg-info/
+-rw-r--r--   0 andrewlevin   (501) staff       (20)     4436 2024-04-24 23:17:38.000000 primemetric-3.1.0/src/primemetric.egg-info/PKG-INFO
+-rw-r--r--   0 andrewlevin   (501) staff       (20)      337 2024-04-24 23:17:38.000000 primemetric-3.1.0/src/primemetric.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewlevin   (501) staff       (20)        1 2024-04-24 23:17:38.000000 primemetric-3.1.0/src/primemetric.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewlevin   (501) staff       (20)       39 2024-04-24 23:17:38.000000 primemetric-3.1.0/src/primemetric.egg-info/entry_points.txt
+-rw-r--r--   0 andrewlevin   (501) staff       (20)       50 2024-04-24 23:17:38.000000 primemetric-3.1.0/src/primemetric.egg-info/requires.txt
+-rw-r--r--   0 andrewlevin   (501) staff       (20)        7 2024-04-24 23:17:38.000000 primemetric-3.1.0/src/primemetric.egg-info/top_level.txt
+drwxr-xr-x   0 andrewlevin   (501) staff       (20)        0 2024-04-24 23:17:38.056328 primemetric-3.1.0/tests/
+-rw-r--r--   0 andrewlevin   (501) staff       (20)      428 2024-04-24 23:05:13.000000 primemetric-3.1.0/tests/test_metric.py
```

### Comparing `primemetric-3.0.0/LICENSE.txt` & `primemetric-3.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `primemetric-3.0.0/PKG-INFO` & `primemetric-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: primemetric
-Version: 3.0.0
+Version: 3.1.0
 Summary: 📐 Prime Metric Demo CLI app
 Author-email: Andrew Levin <author@example.com>
 Maintainer-email: "A. Great Maintainer" <maintainer@example.com>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

### Comparing `primemetric-3.0.0/README.md` & `primemetric-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `primemetric-3.0.0/pyproject.toml` & `primemetric-3.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 name = "primemetric"  # REQUIRED, is the only field that cannot be marked as dynamic.
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "3.0.0"  # REQUIRED, although can be dynamic
+version = "3.1.0"  # REQUIRED, although can be dynamic
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "📐 Prime Metric Demo CLI app"
 
 # This is an optional longer description of your project that represents
@@ -151,15 +151,15 @@
 "Funding" = "https://donate.pypi.org"
 "Say Thanks!" = "https://github.com/andrewalevin/primemetric"
 "Source" = "https://github.com/andrewalevin/primemetric"
 
 # The following would provide a command line executable called `metric`
 # which executes the function `main` from this package when invoked.
 [project.scripts]
-sample = "sample:main"
+metric = "metric:main"
 
 
 # This is configuration specific to the `setuptools` build backend.
 # If you are using a different build backend, you will need to change this.
 [tool.setuptools]
 # If there are data files included in your packages that need to be
 # installed, specify them here.
```

### Comparing `primemetric-3.0.0/src/primemetric.egg-info/PKG-INFO` & `primemetric-3.1.0/src/primemetric.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: primemetric
-Version: 3.0.0
+Version: 3.1.0
 Summary: 📐 Prime Metric Demo CLI app
 Author-email: Andrew Levin <author@example.com>
 Maintainer-email: "A. Great Maintainer" <maintainer@example.com>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

