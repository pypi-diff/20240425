# Comparing `tmp/labeled_contrastive_framework-0.2.3.tar.gz` & `tmp/labeled_contrastive_framework-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labeled_contrastive_framework-0.2.3.tar", last modified: Thu Apr 25 19:07:07 2024, max compression
+gzip compressed data, was "labeled_contrastive_framework-0.2.4.tar", last modified: Thu Apr 25 19:09:48 2024, max compression
```

## Comparing `labeled_contrastive_framework-0.2.3.tar` & `labeled_contrastive_framework-0.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:07:07.218436 labeled_contrastive_framework-0.2.3/
--rw-r--r--   0 carl      (1000) carl      (1000)     1079 2024-04-25 18:44:05.000000 labeled_contrastive_framework-0.2.3/LICENSE
--rw-r--r--   0 carl      (1000) carl      (1000)      720 2024-04-25 19:07:07.218436 labeled_contrastive_framework-0.2.3/PKG-INFO
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:07:07.218436 labeled_contrastive_framework-0.2.3/labeled_contrastive_framework/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 19:06:11.000000 labeled_contrastive_framework-0.2.3/labeled_contrastive_framework/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5639 2024-04-25 17:18:30.000000 labeled_contrastive_framework-0.2.3/labeled_contrastive_framework/module.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2786 2024-04-24 00:16:10.000000 labeled_contrastive_framework-0.2.3/labeled_contrastive_framework/transform.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:07:07.218436 labeled_contrastive_framework-0.2.3/labeled_contrastive_framework.egg-info/
--rw-r--r--   0 carl      (1000) carl      (1000)      720 2024-04-25 19:07:07.000000 labeled_contrastive_framework-0.2.3/labeled_contrastive_framework.egg-info/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)      411 2024-04-25 19:07:07.000000 labeled_contrastive_framework-0.2.3/labeled_contrastive_framework.egg-info/SOURCES.txt
--rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-25 19:07:07.000000 labeled_contrastive_framework-0.2.3/labeled_contrastive_framework.egg-info/dependency_links.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       58 2024-04-25 19:07:07.000000 labeled_contrastive_framework-0.2.3/labeled_contrastive_framework.egg-info/requires.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       30 2024-04-25 19:07:07.000000 labeled_contrastive_framework-0.2.3/labeled_contrastive_framework.egg-info/top_level.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     1009 2024-04-25 19:06:53.000000 labeled_contrastive_framework-0.2.3/pyproject.toml
--rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-25 19:07:07.218436 labeled_contrastive_framework-0.2.3/setup.cfg
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:09:48.043011 labeled_contrastive_framework-0.2.4/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1079 2024-04-25 18:44:05.000000 labeled_contrastive_framework-0.2.4/LICENSE
+-rw-r--r--   0 carl      (1000) carl      (1000)      720 2024-04-25 19:09:48.043011 labeled_contrastive_framework-0.2.4/PKG-INFO
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:09:48.043011 labeled_contrastive_framework-0.2.4/labeled_contrastive_framework/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 19:06:11.000000 labeled_contrastive_framework-0.2.4/labeled_contrastive_framework/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5639 2024-04-25 17:18:30.000000 labeled_contrastive_framework-0.2.4/labeled_contrastive_framework/module.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2786 2024-04-24 00:16:10.000000 labeled_contrastive_framework-0.2.4/labeled_contrastive_framework/transform.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:09:48.043011 labeled_contrastive_framework-0.2.4/labeled_contrastive_framework.egg-info/
+-rw-r--r--   0 carl      (1000) carl      (1000)      720 2024-04-25 19:09:33.000000 labeled_contrastive_framework-0.2.4/labeled_contrastive_framework.egg-info/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)      411 2024-04-25 19:09:48.000000 labeled_contrastive_framework-0.2.4/labeled_contrastive_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-25 19:09:33.000000 labeled_contrastive_framework-0.2.4/labeled_contrastive_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       58 2024-04-25 19:09:33.000000 labeled_contrastive_framework-0.2.4/labeled_contrastive_framework.egg-info/requires.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       80 2024-04-25 19:09:33.000000 labeled_contrastive_framework-0.2.4/labeled_contrastive_framework.egg-info/top_level.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      981 2024-04-25 19:08:05.000000 labeled_contrastive_framework-0.2.4/pyproject.toml
+-rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-25 19:09:48.043011 labeled_contrastive_framework-0.2.4/setup.cfg
```

### Comparing `labeled_contrastive_framework-0.2.3/LICENSE` & `labeled_contrastive_framework-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `labeled_contrastive_framework-0.2.3/PKG-INFO` & `labeled_contrastive_framework-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labeled_contrastive_framework
-Version: 0.2.3
+Version: 0.2.4
 Summary: Framework for training contrastive models with labeled data using arcface loss.
 Author-email: Carl Schader <carlschader@gmail.com>
 Project-URL: Homepage, https://github.com/carlschader/labeled-contrastive-framework
 Project-URL: Issues, https://github.com/carlschader/labeled-contrastive-framework/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `labeled_contrastive_framework-0.2.3/labeled_contrastive_framework/module.py` & `labeled_contrastive_framework-0.2.4/labeled_contrastive_framework/module.py`

 * *Files identical despite different names*

### Comparing `labeled_contrastive_framework-0.2.3/labeled_contrastive_framework/transform.py` & `labeled_contrastive_framework-0.2.4/labeled_contrastive_framework/transform.py`

 * *Files identical despite different names*

### Comparing `labeled_contrastive_framework-0.2.3/labeled_contrastive_framework.egg-info/PKG-INFO` & `labeled_contrastive_framework-0.2.4/labeled_contrastive_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labeled_contrastive_framework
-Version: 0.2.3
+Version: 0.2.4
 Summary: Framework for training contrastive models with labeled data using arcface loss.
 Author-email: Carl Schader <carlschader@gmail.com>
 Project-URL: Homepage, https://github.com/carlschader/labeled-contrastive-framework
 Project-URL: Issues, https://github.com/carlschader/labeled-contrastive-framework/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `labeled_contrastive_framework-0.2.3/pyproject.toml` & `labeled_contrastive_framework-0.2.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "labeled_contrastive_framework"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
   { name="Carl Schader", email="carlschader@gmail.com" },
 ]
 description = "Framework for training contrastive models with labeled data using arcface loss."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -25,10 +25,10 @@
 [project.urls]
 Homepage = "https://github.com/carlschader/labeled-contrastive-framework"
 Issues = "https://github.com/carlschader/labeled-contrastive-framework/issues"
 
 [tool.setuptools.packages.find]
 # All the following settings are optional:
 where = ["."]  # ["."] by default
-include = ["labeled_contrastive_framework"]  # ["*"] by default
+include = ["*"]  # ["*"] by default
 exclude = ["scripts"]  # empty by default
```

