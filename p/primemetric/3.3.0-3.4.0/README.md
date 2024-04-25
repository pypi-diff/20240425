# Comparing `tmp/primemetric-3.3.0.tar.gz` & `tmp/primemetric-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "primemetric-3.3.0.tar", last modified: Thu Apr 25 00:54:04 2024, max compression
+gzip compressed data, was "primemetric-3.4.0.tar", last modified: Thu Apr 25 01:00:59 2024, max compression
```

## Comparing `primemetric-3.3.0.tar` & `primemetric-3.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 andrewlevin   (501) staff       (20)        0 2024-04-25 00:54:04.647751 primemetric-3.3.0/
--rw-r--r--   0 andrewlevin   (501) staff       (20)     1081 2024-04-23 01:04:50.000000 primemetric-3.3.0/LICENSE.txt
--rw-r--r--   0 andrewlevin   (501) staff       (20)     4410 2024-04-25 00:54:04.647458 primemetric-3.3.0/PKG-INFO
--rw-r--r--   0 andrewlevin   (501) staff       (20)     1811 2024-04-23 21:38:16.000000 primemetric-3.3.0/README.md
--rw-r--r--   0 andrewlevin   (501) staff       (20)     6716 2024-04-25 00:50:32.000000 primemetric-3.3.0/pyproject.toml
--rw-r--r--   0 andrewlevin   (501) staff       (20)       38 2024-04-25 00:54:04.647822 primemetric-3.3.0/setup.cfg
-drwxr-xr-x   0 andrewlevin   (501) staff       (20)        0 2024-04-25 00:54:04.643515 primemetric-3.3.0/src/
-drwxr-xr-x   0 andrewlevin   (501) staff       (20)        0 2024-04-25 00:54:04.644794 primemetric-3.3.0/src/metric/
--rw-r--r--   0 andrewlevin   (501) staff       (20)      113 2024-04-25 00:47:23.000000 primemetric-3.3.0/src/metric/__init__.py
--rw-r--r--   0 andrewlevin   (501) staff       (20)      485 2024-04-25 00:48:09.000000 primemetric-3.3.0/src/metric/metric.py
-drwxr-xr-x   0 andrewlevin   (501) staff       (20)        0 2024-04-25 00:54:04.646938 primemetric-3.3.0/src/primemetric.egg-info/
--rw-r--r--   0 andrewlevin   (501) staff       (20)     4410 2024-04-25 00:54:04.000000 primemetric-3.3.0/src/primemetric.egg-info/PKG-INFO
--rw-r--r--   0 andrewlevin   (501) staff       (20)      337 2024-04-25 00:54:04.000000 primemetric-3.3.0/src/primemetric.egg-info/SOURCES.txt
--rw-r--r--   0 andrewlevin   (501) staff       (20)        1 2024-04-25 00:54:04.000000 primemetric-3.3.0/src/primemetric.egg-info/dependency_links.txt
--rw-r--r--   0 andrewlevin   (501) staff       (20)       39 2024-04-25 00:54:04.000000 primemetric-3.3.0/src/primemetric.egg-info/entry_points.txt
--rw-r--r--   0 andrewlevin   (501) staff       (20)       39 2024-04-25 00:54:04.000000 primemetric-3.3.0/src/primemetric.egg-info/requires.txt
--rw-r--r--   0 andrewlevin   (501) staff       (20)        7 2024-04-25 00:54:04.000000 primemetric-3.3.0/src/primemetric.egg-info/top_level.txt
-drwxr-xr-x   0 andrewlevin   (501) staff       (20)        0 2024-04-25 00:54:04.646546 primemetric-3.3.0/tests/
--rw-r--r--   0 andrewlevin   (501) staff       (20)      428 2024-04-24 23:05:13.000000 primemetric-3.3.0/tests/test_metric.py
+drwxr-xr-x   0 andrewlevin   (501) staff       (20)        0 2024-04-25 01:00:59.498890 primemetric-3.4.0/
+-rw-r--r--   0 andrewlevin   (501) staff       (20)     1081 2024-04-23 01:04:50.000000 primemetric-3.4.0/LICENSE.txt
+-rw-r--r--   0 andrewlevin   (501) staff       (20)     4410 2024-04-25 01:00:59.498676 primemetric-3.4.0/PKG-INFO
+-rw-r--r--   0 andrewlevin   (501) staff       (20)     1811 2024-04-23 21:38:16.000000 primemetric-3.4.0/README.md
+-rw-r--r--   0 andrewlevin   (501) staff       (20)     6716 2024-04-25 01:00:45.000000 primemetric-3.4.0/pyproject.toml
+-rw-r--r--   0 andrewlevin   (501) staff       (20)       38 2024-04-25 01:00:59.498947 primemetric-3.4.0/setup.cfg
+drwxr-xr-x   0 andrewlevin   (501) staff       (20)        0 2024-04-25 01:00:59.496118 primemetric-3.4.0/src/
+drwxr-xr-x   0 andrewlevin   (501) staff       (20)        0 2024-04-25 01:00:59.496928 primemetric-3.4.0/src/metric/
+-rw-r--r--   0 andrewlevin   (501) staff       (20)        0 2024-04-25 01:00:31.000000 primemetric-3.4.0/src/metric/__init__.py
+-rw-r--r--   0 andrewlevin   (501) staff       (20)      485 2024-04-25 00:48:09.000000 primemetric-3.4.0/src/metric/metric.py
+drwxr-xr-x   0 andrewlevin   (501) staff       (20)        0 2024-04-25 01:00:59.498279 primemetric-3.4.0/src/primemetric.egg-info/
+-rw-r--r--   0 andrewlevin   (501) staff       (20)     4410 2024-04-25 01:00:59.000000 primemetric-3.4.0/src/primemetric.egg-info/PKG-INFO
+-rw-r--r--   0 andrewlevin   (501) staff       (20)      337 2024-04-25 01:00:59.000000 primemetric-3.4.0/src/primemetric.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewlevin   (501) staff       (20)        1 2024-04-25 01:00:59.000000 primemetric-3.4.0/src/primemetric.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewlevin   (501) staff       (20)       39 2024-04-25 01:00:59.000000 primemetric-3.4.0/src/primemetric.egg-info/entry_points.txt
+-rw-r--r--   0 andrewlevin   (501) staff       (20)       39 2024-04-25 01:00:59.000000 primemetric-3.4.0/src/primemetric.egg-info/requires.txt
+-rw-r--r--   0 andrewlevin   (501) staff       (20)        7 2024-04-25 01:00:59.000000 primemetric-3.4.0/src/primemetric.egg-info/top_level.txt
+drwxr-xr-x   0 andrewlevin   (501) staff       (20)        0 2024-04-25 01:00:59.498047 primemetric-3.4.0/tests/
+-rw-r--r--   0 andrewlevin   (501) staff       (20)      428 2024-04-24 23:05:13.000000 primemetric-3.4.0/tests/test_metric.py
```

### Comparing `primemetric-3.3.0/LICENSE.txt` & `primemetric-3.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `primemetric-3.3.0/PKG-INFO` & `primemetric-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: primemetric
-Version: 3.3.0
+Version: 3.4.0
 Summary: 📐 Prime Metric Demo CLI app
 Author-email: Andrew Levin <author@example.com>
 Maintainer-email: "A. Great Maintainer" <maintainer@example.com>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

### Comparing `primemetric-3.3.0/README.md` & `primemetric-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `primemetric-3.3.0/pyproject.toml` & `primemetric-3.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 name = "primemetric"  # REQUIRED, is the only field that cannot be marked as dynamic.
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "3.3.0"  # REQUIRED, although can be dynamic
+version = "3.4.0"  # REQUIRED, although can be dynamic
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "📐 Prime Metric Demo CLI app"
 
 # This is an optional longer description of your project that represents
```

### Comparing `primemetric-3.3.0/src/primemetric.egg-info/PKG-INFO` & `primemetric-3.4.0/src/primemetric.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: primemetric
-Version: 3.3.0
+Version: 3.4.0
 Summary: 📐 Prime Metric Demo CLI app
 Author-email: Andrew Levin <author@example.com>
 Maintainer-email: "A. Great Maintainer" <maintainer@example.com>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

