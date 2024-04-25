# Comparing `tmp/ontopint-0.0.3.tar.gz` & `tmp/ontopint-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ontopint-0.0.3.tar", last modified: Wed Apr 24 13:07:54 2024, max compression
+gzip compressed data, was "ontopint-0.0.4.tar", last modified: Thu Apr 25 08:31:16 2024, max compression
```

## Comparing `ontopint-0.0.3.tar` & `ontopint-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:07:54.899689 ontopint-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:07:54.895689 ontopint-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:07:54.895689 ontopint-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-24 13:07:45.000000 ontopint-0.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-04-24 13:07:45.000000 ontopint-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-24 13:07:45.000000 ontopint-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-04-24 13:07:54.899689 ontopint-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-24 13:07:45.000000 ontopint-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-24 13:07:45.000000 ontopint-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 13:07:54.899689 ontopint-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:07:54.895689 ontopint-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:07:54.895689 ontopint-0.0.3/src/ontopint/
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-24 13:07:45.000000 ontopint-0.0.3/src/ontopint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:07:54.899689 ontopint-0.0.3/src/ontopint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-04-24 13:07:54.000000 ontopint-0.0.3/src/ontopint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-24 13:07:54.000000 ontopint-0.0.3/src/ontopint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:07:54.000000 ontopint-0.0.3/src/ontopint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-24 13:07:54.000000 ontopint-0.0.3/src/ontopint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 13:07:54.000000 ontopint-0.0.3/src/ontopint.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:31:16.566547 ontopint-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:31:16.562547 ontopint-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:31:16.566547 ontopint-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-25 08:31:11.000000 ontopint-0.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-04-25 08:31:11.000000 ontopint-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-25 08:31:11.000000 ontopint-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-25 08:31:16.566547 ontopint-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-25 08:31:11.000000 ontopint-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-25 08:31:11.000000 ontopint-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 08:31:16.566547 ontopint-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:31:16.566547 ontopint-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:31:16.566547 ontopint-0.0.4/src/ontopint/
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-25 08:31:11.000000 ontopint-0.0.4/src/ontopint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:31:16.566547 ontopint-0.0.4/src/ontopint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-25 08:31:16.000000 ontopint-0.0.4/src/ontopint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-25 08:31:16.000000 ontopint-0.0.4/src/ontopint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 08:31:16.000000 ontopint-0.0.4/src/ontopint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-25 08:31:16.000000 ontopint-0.0.4/src/ontopint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 08:31:16.000000 ontopint-0.0.4/src/ontopint.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:31:16.566547 ontopint-0.0.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:31:16.566547 ontopint-0.0.4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-25 08:31:11.000000 ontopint-0.0.4/tests/data/test_data.jsonld
```

### Comparing `ontopint-0.0.3/.github/workflows/python-publish.yml` & `ontopint-0.0.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ontopint-0.0.3/.gitignore` & `ontopint-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ontopint-0.0.3/LICENSE` & `ontopint-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ontopint-0.0.3/PKG-INFO` & `ontopint-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ontopint
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python package for reading units from a JSON-LD files and generating pint quantities.
-Author: Fabian Kirchner, Simon Stier
+Author: Fabian Kirchner, Simon Stier, Fabio Lopes, Despoina Adamopoulou, Samantha Pearman-Kanza
 Author-email: Hampus Näsström <hampus.naesstroem@physik.hu-berlin.de>
 Maintainer-email: Hampus Näsström <hampus.naesstroem@physik.hu-berlin.de>
 License: MIT License
         
         Copyright (c) 2024 Hampus Näsström
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,12 +33,13 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: rdflib
 Requires-Dist: pint
+Requires-Dist: pyld
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 
 # ontopint
 A python package for reading units from a JSON-LD files and generating pint quantities.
```

### Comparing `ontopint-0.0.3/pyproject.toml` & `ontopint-0.0.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -10,27 +10,31 @@
 dynamic = ["version"]
 description = "A python package for reading units from a JSON-LD files and generating pint quantities."
 readme = "README.md"
 authors = [
     { name = "Hampus Näsström", email = 'hampus.naesstroem@physik.hu-berlin.de' },
     { name = "Fabian Kirchner" },
     { name = "Simon Stier" },
+    { name = "Fabio Lopes" },
+    { name = "Despoina Adamopoulou" },
+    { name = "Samantha Pearman-Kanza"}
 ]
 maintainers = [
   { name = "Hampus Näsström", email = 'hampus.naesstroem@physik.hu-berlin.de' }
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "License :: OSI Approved :: MIT License",
 ]
 dependencies = [
     "rdflib",
     "pint",
+    "pyld",
 ]
 [project.optional-dependencies]
 dev = [
     "pytest",
 ]
 
 [project.license]
```

### Comparing `ontopint-0.0.3/src/ontopint.egg-info/PKG-INFO` & `ontopint-0.0.4/src/ontopint.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ontopint
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python package for reading units from a JSON-LD files and generating pint quantities.
-Author: Fabian Kirchner, Simon Stier
+Author: Fabian Kirchner, Simon Stier, Fabio Lopes, Despoina Adamopoulou, Samantha Pearman-Kanza
 Author-email: Hampus Näsström <hampus.naesstroem@physik.hu-berlin.de>
 Maintainer-email: Hampus Näsström <hampus.naesstroem@physik.hu-berlin.de>
 License: MIT License
         
         Copyright (c) 2024 Hampus Näsström
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,12 +33,13 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: rdflib
 Requires-Dist: pint
+Requires-Dist: pyld
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 
 # ontopint
 A python package for reading units from a JSON-LD files and generating pint quantities.
```

