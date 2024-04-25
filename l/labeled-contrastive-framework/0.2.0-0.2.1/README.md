# Comparing `tmp/labeled_contrastive_framework-0.2.0.tar.gz` & `tmp/labeled_contrastive_framework-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labeled_contrastive_framework-0.2.0.tar", last modified: Thu Apr 25 18:52:33 2024, max compression
+gzip compressed data, was "labeled_contrastive_framework-0.2.1.tar", last modified: Thu Apr 25 18:58:42 2024, max compression
```

## Comparing `labeled_contrastive_framework-0.2.0.tar` & `labeled_contrastive_framework-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 18:52:33.616517 labeled_contrastive_framework-0.2.0/
--rw-r--r--   0 carl      (1000) carl      (1000)     1079 2024-04-25 18:44:05.000000 labeled_contrastive_framework-0.2.0/LICENSE
--rw-r--r--   0 carl      (1000) carl      (1000)      688 2024-04-25 18:52:33.616517 labeled_contrastive_framework-0.2.0/PKG-INFO
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 18:52:33.613184 labeled_contrastive_framework-0.2.0/labeled_contrastive_framework/
--rw-r--r--   0 carl      (1000) carl      (1000)     5639 2024-04-25 17:18:30.000000 labeled_contrastive_framework-0.2.0/labeled_contrastive_framework/module.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2786 2024-04-24 00:16:10.000000 labeled_contrastive_framework-0.2.0/labeled_contrastive_framework/transform.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 18:52:33.613184 labeled_contrastive_framework-0.2.0/labeled_contrastive_framework.egg-info/
--rw-r--r--   0 carl      (1000) carl      (1000)      688 2024-04-25 18:52:33.000000 labeled_contrastive_framework-0.2.0/labeled_contrastive_framework.egg-info/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)      369 2024-04-25 18:52:33.000000 labeled_contrastive_framework-0.2.0/labeled_contrastive_framework.egg-info/SOURCES.txt
--rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-25 18:52:33.000000 labeled_contrastive_framework-0.2.0/labeled_contrastive_framework.egg-info/dependency_links.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       58 2024-04-25 18:52:33.000000 labeled_contrastive_framework-0.2.0/labeled_contrastive_framework.egg-info/requires.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       30 2024-04-25 18:52:33.000000 labeled_contrastive_framework-0.2.0/labeled_contrastive_framework.egg-info/top_level.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      977 2024-04-25 18:52:20.000000 labeled_contrastive_framework-0.2.0/pyproject.toml
--rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-25 18:52:33.616517 labeled_contrastive_framework-0.2.0/setup.cfg
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 18:58:42.208358 labeled_contrastive_framework-0.2.1/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1079 2024-04-25 18:44:05.000000 labeled_contrastive_framework-0.2.1/LICENSE
+-rw-r--r--   0 carl      (1000) carl      (1000)      688 2024-04-25 18:58:42.208358 labeled_contrastive_framework-0.2.1/PKG-INFO
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 18:58:42.205025 labeled_contrastive_framework-0.2.1/labeled_contrastive_framework/
+-rw-r--r--   0 carl      (1000) carl      (1000)     5639 2024-04-25 17:18:30.000000 labeled_contrastive_framework-0.2.1/labeled_contrastive_framework/module.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2786 2024-04-24 00:16:10.000000 labeled_contrastive_framework-0.2.1/labeled_contrastive_framework/transform.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 18:58:42.208358 labeled_contrastive_framework-0.2.1/labeled_contrastive_framework.egg-info/
+-rw-r--r--   0 carl      (1000) carl      (1000)      688 2024-04-25 18:58:42.000000 labeled_contrastive_framework-0.2.1/labeled_contrastive_framework.egg-info/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)      369 2024-04-25 18:58:42.000000 labeled_contrastive_framework-0.2.1/labeled_contrastive_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-25 18:58:42.000000 labeled_contrastive_framework-0.2.1/labeled_contrastive_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       58 2024-04-25 18:58:42.000000 labeled_contrastive_framework-0.2.1/labeled_contrastive_framework.egg-info/requires.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       30 2024-04-25 18:58:42.000000 labeled_contrastive_framework-0.2.1/labeled_contrastive_framework.egg-info/top_level.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      977 2024-04-25 18:58:27.000000 labeled_contrastive_framework-0.2.1/pyproject.toml
+-rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-25 18:58:42.208358 labeled_contrastive_framework-0.2.1/setup.cfg
```

### Comparing `labeled_contrastive_framework-0.2.0/LICENSE` & `labeled_contrastive_framework-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `labeled_contrastive_framework-0.2.0/PKG-INFO` & `labeled_contrastive_framework-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labeled_contrastive_framework
-Version: 0.2.0
+Version: 0.2.1
 Summary: Framework for training contrastive models with labeled data using arcface loss.
 Author-email: Carl Schader <carlschader@gmail.com>
 Project-URL: Homepage, https://github.com/carlschader/ssl_framework
 Project-URL: Issues, https://github.com/carlschader/ssl_framework/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `labeled_contrastive_framework-0.2.0/labeled_contrastive_framework/module.py` & `labeled_contrastive_framework-0.2.1/labeled_contrastive_framework/module.py`

 * *Files identical despite different names*

### Comparing `labeled_contrastive_framework-0.2.0/labeled_contrastive_framework/transform.py` & `labeled_contrastive_framework-0.2.1/labeled_contrastive_framework/transform.py`

 * *Files identical despite different names*

### Comparing `labeled_contrastive_framework-0.2.0/labeled_contrastive_framework.egg-info/PKG-INFO` & `labeled_contrastive_framework-0.2.1/labeled_contrastive_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labeled_contrastive_framework
-Version: 0.2.0
+Version: 0.2.1
 Summary: Framework for training contrastive models with labeled data using arcface loss.
 Author-email: Carl Schader <carlschader@gmail.com>
 Project-URL: Homepage, https://github.com/carlschader/ssl_framework
 Project-URL: Issues, https://github.com/carlschader/ssl_framework/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `labeled_contrastive_framework-0.2.0/pyproject.toml` & `labeled_contrastive_framework-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "labeled_contrastive_framework"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Carl Schader", email="carlschader@gmail.com" },
 ]
 description = "Framework for training contrastive models with labeled data using arcface loss."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

