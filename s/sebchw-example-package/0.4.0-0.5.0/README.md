# Comparing `tmp/sebchw_example_package-0.4.0.tar.gz` & `tmp/sebchw_example_package-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sebchw_example_package-0.4.0.tar", last modified: Thu Apr 18 08:02:24 2024, max compression
+gzip compressed data, was "sebchw_example_package-0.5.0.tar", last modified: Thu Apr 25 11:18:41 2024, max compression
```

## Comparing `sebchw_example_package-0.4.0.tar` & `sebchw_example_package-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 08:02:24.064122 sebchw_example_package-0.4.0/
--rw-r--r--   0 root         (0) root         (0)     1081 2024-04-18 08:02:19.000000 sebchw_example_package-0.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      535 2024-04-18 08:02:24.064122 sebchw_example_package-0.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       26 2024-04-18 08:02:19.000000 sebchw_example_package-0.4.0/README.md
--rw-r--r--   0 root         (0) root         (0)     2107 2024-04-18 08:02:21.000000 sebchw_example_package-0.4.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-18 08:02:24.064122 sebchw_example_package-0.4.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 08:02:24.060122 sebchw_example_package-0.4.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 08:02:24.060122 sebchw_example_package-0.4.0/src/sebchw_example_package/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 08:02:19.000000 sebchw_example_package-0.4.0/src/sebchw_example_package/__init__.py
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-18 08:02:21.000000 sebchw_example_package-0.4.0/src/sebchw_example_package/__version__.py
--rw-r--r--   0 root         (0) root         (0)       64 2024-04-18 08:02:19.000000 sebchw_example_package-0.4.0/src/sebchw_example_package/example.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 08:02:24.064122 sebchw_example_package-0.4.0/src/sebchw_example_package.egg-info/
--rw-r--r--   0 root         (0) root         (0)      535 2024-04-18 08:02:24.000000 sebchw_example_package-0.4.0/src/sebchw_example_package.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      351 2024-04-18 08:02:24.000000 sebchw_example_package-0.4.0/src/sebchw_example_package.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 08:02:24.000000 sebchw_example_package-0.4.0/src/sebchw_example_package.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-18 08:02:24.000000 sebchw_example_package-0.4.0/src/sebchw_example_package.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 11:18:40.999154 sebchw_example_package-0.5.0/
+-rw-r--r--   0 root         (0) root         (0)     1081 2024-04-25 11:18:37.000000 sebchw_example_package-0.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      535 2024-04-25 11:18:40.999154 sebchw_example_package-0.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       26 2024-04-25 11:18:37.000000 sebchw_example_package-0.5.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     2131 2024-04-25 11:18:38.000000 sebchw_example_package-0.5.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       80 2024-04-25 11:18:40.999154 sebchw_example_package-0.5.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 11:18:40.999154 sebchw_example_package-0.5.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 11:18:40.999154 sebchw_example_package-0.5.0/src/sebchw_example_package/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 11:18:37.000000 sebchw_example_package-0.5.0/src/sebchw_example_package/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-25 11:18:38.000000 sebchw_example_package-0.5.0/src/sebchw_example_package/__version__.py
+-rw-r--r--   0 root         (0) root         (0)       64 2024-04-25 11:18:37.000000 sebchw_example_package-0.5.0/src/sebchw_example_package/example.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 11:18:40.999154 sebchw_example_package-0.5.0/src/sebchw_example_package.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      535 2024-04-25 11:18:40.000000 sebchw_example_package-0.5.0/src/sebchw_example_package.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      361 2024-04-25 11:18:40.000000 sebchw_example_package-0.5.0/src/sebchw_example_package.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 11:18:40.000000 sebchw_example_package-0.5.0/src/sebchw_example_package.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-25 11:18:40.000000 sebchw_example_package-0.5.0/src/sebchw_example_package.egg-info/top_level.txt
```

### Comparing `sebchw_example_package-0.4.0/LICENSE` & `sebchw_example_package-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sebchw_example_package-0.4.0/PKG-INFO` & `sebchw_example_package-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sebchw_example_package
-Version: 0.4.0
+Version: 0.5.0
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sebchw_example_package-0.4.0/pyproject.toml` & `sebchw_example_package-0.5.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "sebchw_example_package"
-version = "0.4.0"
+version = "0.5.0"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -30,14 +30,15 @@
 logging_use_named_masks = false
 major_on_zero = false
 allow_zero_version = true
 tag_format = "v{version}"
 version_variables = [
     "pyproject.toml:version",
     "src/sebchw_example_package/__version__.py:__version__",
+    "setup.cfg:version"
 ]
 build_command = "pip install build && python -m build"
 
 [tool.semantic_release.branches.main]
 match = "(main|master)"
 prerelease_token = "rc"
 prerelease = false
```

### Comparing `sebchw_example_package-0.4.0/src/sebchw_example_package.egg-info/PKG-INFO` & `sebchw_example_package-0.5.0/src/sebchw_example_package.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sebchw_example_package
-Version: 0.4.0
+Version: 0.5.0
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

