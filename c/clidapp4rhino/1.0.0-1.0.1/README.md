# Comparing `tmp/clidapp4rhino-1.0.0.tar.gz` & `tmp/clidapp4rhino-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clidapp4rhino-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "clidapp4rhino-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `clidapp4rhino-1.0.0.tar` & `clidapp4rhino-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      228 2024-04-23 13:25:03.249344 clidapp4rhino-1.0.0/README.md
--rw-r--r--   0        0        0      766 2024-04-25 15:14:28.449754 clidapp4rhino-1.0.0/pyproject.toml
--rwxr-xr-x   0        0        0  7665296 2024-04-23 14:11:02.795583 clidapp4rhino-1.0.0/src/CliDApp4Rhino/CliDApp4Rhino
--rw-r--r--   0        0        0        0 2024-04-23 12:55:45.768956 clidapp4rhino-1.0.0/src/CliDApp4Rhino/__init__.py
--rw-r--r--   0        0        0      195 2024-04-25 15:13:03.802479 clidapp4rhino-1.0.0/src/CliDApp4Rhino/run_executable.py
--rw-r--r--   0        0        0      839 1970-01-01 00:00:00.000000 clidapp4rhino-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      228 2024-04-23 13:25:03.249344 clidapp4rhino-1.0.1/README.md
+-rw-r--r--   0        0        0      766 2024-04-25 15:31:30.507296 clidapp4rhino-1.0.1/pyproject.toml
+-rwxr-xr-x   0        0        0  7665296 2024-04-23 14:11:02.795583 clidapp4rhino-1.0.1/src/clidapp4rhino/CliDApp4Rhino
+-rw-r--r--   0        0        0        0 2024-04-23 12:55:45.768956 clidapp4rhino-1.0.1/src/clidapp4rhino/__init__.py
+-rw-r--r--   0        0        0      195 2024-04-25 15:13:03.802479 clidapp4rhino-1.0.1/src/clidapp4rhino/run_executable.py
+-rw-r--r--   0        0        0      839 1970-01-01 00:00:00.000000 clidapp4rhino-1.0.1/PKG-INFO
```

### Comparing `clidapp4rhino-1.0.0/pyproject.toml` & `clidapp4rhino-1.0.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
-name = "CliDApp4Rhino"
-version = "1.0.0"
+name = "clidapp4rhino"
+version = "1.0.1"
 authors = [
   { name="Elizabeth Consulting International Inc.", email="info@ec-intl.com" },
 ]
 description = "The CliDApp4Rhino package is a Python package that provides a command to install the CliDApp4Rhino plugin for MacOS in Rhino."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `clidapp4rhino-1.0.0/src/CliDApp4Rhino/CliDApp4Rhino` & `clidapp4rhino-1.0.1/src/clidapp4rhino/CliDApp4Rhino`

 * *Files identical despite different names*

### Comparing `clidapp4rhino-1.0.0/PKG-INFO` & `clidapp4rhino-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: CliDApp4Rhino
-Version: 1.0.0
+Name: clidapp4rhino
+Version: 1.0.1
 Summary: The CliDApp4Rhino package is a Python package that provides a command to install the CliDApp4Rhino plugin for MacOS in Rhino.
 Author-email: "Elizabeth Consulting International Inc." <info@ec-intl.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

