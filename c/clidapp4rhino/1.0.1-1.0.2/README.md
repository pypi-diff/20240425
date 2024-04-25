# Comparing `tmp/clidapp4rhino-1.0.1.tar.gz` & `tmp/clidapp4rhino-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clidapp4rhino-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "clidapp4rhino-1.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `clidapp4rhino-1.0.1.tar` & `clidapp4rhino-1.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      228 2024-04-23 13:25:03.249344 clidapp4rhino-1.0.1/README.md
--rw-r--r--   0        0        0      766 2024-04-25 15:31:30.507296 clidapp4rhino-1.0.1/pyproject.toml
--rwxr-xr-x   0        0        0  7665296 2024-04-23 14:11:02.795583 clidapp4rhino-1.0.1/src/clidapp4rhino/CliDApp4Rhino
--rw-r--r--   0        0        0        0 2024-04-23 12:55:45.768956 clidapp4rhino-1.0.1/src/clidapp4rhino/__init__.py
--rw-r--r--   0        0        0      195 2024-04-25 15:13:03.802479 clidapp4rhino-1.0.1/src/clidapp4rhino/run_executable.py
--rw-r--r--   0        0        0      839 1970-01-01 00:00:00.000000 clidapp4rhino-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      228 2024-04-23 13:25:03.249344 clidapp4rhino-1.0.2/README.md
+-rw-r--r--   0        0        0      812 2024-04-25 15:44:10.618033 clidapp4rhino-1.0.2/pyproject.toml
+-rwxr-xr-x   0        0        0  7665296 2024-04-23 14:11:02.795583 clidapp4rhino-1.0.2/src/clidapp4rhino/CliDApp4Rhino
+-rw-r--r--   0        0        0        0 2024-04-23 12:55:45.768956 clidapp4rhino-1.0.2/src/clidapp4rhino/__init__.py
+-rw-r--r--   0        0        0      195 2024-04-25 15:13:03.802479 clidapp4rhino-1.0.2/src/clidapp4rhino/run_executable.py
+-rw-r--r--   0        0        0      839 1970-01-01 00:00:00.000000 clidapp4rhino-1.0.2/PKG-INFO
```

### Comparing `clidapp4rhino-1.0.1/pyproject.toml` & `clidapp4rhino-1.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [project]
 name = "clidapp4rhino"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Elizabeth Consulting International Inc.", email="info@ec-intl.com" },
 ]
 description = "The CliDApp4Rhino package is a Python package that provides a command to install the CliDApp4Rhino plugin for MacOS in Rhino."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+include = ["src/clidapp4rhino/CliDApp4Rhino"]
 
 [project.urls]
 Homepage = "https://github.com/ec-intl/clidapp4rhino"
 Issues = "https://github.com/ec-intl/clidapp4rhino/issues"
 
 [build-system]
 requires = ["flit_core>=3.4"]
```

### Comparing `clidapp4rhino-1.0.1/src/clidapp4rhino/CliDApp4Rhino` & `clidapp4rhino-1.0.2/src/clidapp4rhino/CliDApp4Rhino`

 * *Files identical despite different names*

### Comparing `clidapp4rhino-1.0.1/PKG-INFO` & `clidapp4rhino-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clidapp4rhino
-Version: 1.0.1
+Version: 1.0.2
 Summary: The CliDApp4Rhino package is a Python package that provides a command to install the CliDApp4Rhino plugin for MacOS in Rhino.
 Author-email: "Elizabeth Consulting International Inc." <info@ec-intl.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

