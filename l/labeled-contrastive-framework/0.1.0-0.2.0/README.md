# Comparing `tmp/labeled_contrastive_framework-0.1.0.tar.gz` & `tmp/labeled_contrastive_framework-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labeled_contrastive_framework-0.1.0.tar", last modified: Thu Apr 25 03:10:38 2024, max compression
+gzip compressed data, was "labeled_contrastive_framework-0.2.0.tar", last modified: Thu Apr 25 18:52:33 2024, max compression
```

## Comparing `labeled_contrastive_framework-0.1.0.tar` & `labeled_contrastive_framework-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 03:10:38.303203 labeled_contrastive_framework-0.1.0/
--rw-r--r--   0 carl      (1000) carl      (1000)     1072 2024-04-20 14:34:35.000000 labeled_contrastive_framework-0.1.0/LICENSE
--rw-r--r--   0 carl      (1000) carl      (1000)      648 2024-04-25 03:10:38.303203 labeled_contrastive_framework-0.1.0/PKG-INFO
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 03:10:38.303203 labeled_contrastive_framework-0.1.0/labeled_contrastive_framework.egg-info/
--rw-r--r--   0 carl      (1000) carl      (1000)      648 2024-04-25 03:10:38.000000 labeled_contrastive_framework-0.1.0/labeled_contrastive_framework.egg-info/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)      286 2024-04-25 03:10:38.000000 labeled_contrastive_framework-0.1.0/labeled_contrastive_framework.egg-info/SOURCES.txt
--rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-25 03:10:38.000000 labeled_contrastive_framework-0.1.0/labeled_contrastive_framework.egg-info/dependency_links.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       33 2024-04-25 03:10:38.000000 labeled_contrastive_framework-0.1.0/labeled_contrastive_framework.egg-info/requires.txt
--rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-25 03:10:38.000000 labeled_contrastive_framework-0.1.0/labeled_contrastive_framework.egg-info/top_level.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      919 2024-04-25 03:10:13.000000 labeled_contrastive_framework-0.1.0/pyproject.toml
--rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-25 03:10:38.303203 labeled_contrastive_framework-0.1.0/setup.cfg
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 18:52:33.616517 labeled_contrastive_framework-0.2.0/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1079 2024-04-25 18:44:05.000000 labeled_contrastive_framework-0.2.0/LICENSE
+-rw-r--r--   0 carl      (1000) carl      (1000)      688 2024-04-25 18:52:33.616517 labeled_contrastive_framework-0.2.0/PKG-INFO
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 18:52:33.613184 labeled_contrastive_framework-0.2.0/labeled_contrastive_framework/
+-rw-r--r--   0 carl      (1000) carl      (1000)     5639 2024-04-25 17:18:30.000000 labeled_contrastive_framework-0.2.0/labeled_contrastive_framework/module.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2786 2024-04-24 00:16:10.000000 labeled_contrastive_framework-0.2.0/labeled_contrastive_framework/transform.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 18:52:33.613184 labeled_contrastive_framework-0.2.0/labeled_contrastive_framework.egg-info/
+-rw-r--r--   0 carl      (1000) carl      (1000)      688 2024-04-25 18:52:33.000000 labeled_contrastive_framework-0.2.0/labeled_contrastive_framework.egg-info/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)      369 2024-04-25 18:52:33.000000 labeled_contrastive_framework-0.2.0/labeled_contrastive_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-25 18:52:33.000000 labeled_contrastive_framework-0.2.0/labeled_contrastive_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       58 2024-04-25 18:52:33.000000 labeled_contrastive_framework-0.2.0/labeled_contrastive_framework.egg-info/requires.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       30 2024-04-25 18:52:33.000000 labeled_contrastive_framework-0.2.0/labeled_contrastive_framework.egg-info/top_level.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      977 2024-04-25 18:52:20.000000 labeled_contrastive_framework-0.2.0/pyproject.toml
+-rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-25 18:52:33.616517 labeled_contrastive_framework-0.2.0/setup.cfg
```

### Comparing `labeled_contrastive_framework-0.1.0/LICENSE` & `labeled_contrastive_framework-0.2.0/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-Copyright (c) 2012-2024 Scott Chacon and others
+The MIT License (MIT)
 
-Permission is hereby granted, free of charge, to any person obtaining
-a copy of this software and associated documentation files (the
-"Software"), to deal in the Software without restriction, including
-without limitation the rights to use, copy, modify, merge, publish,
-distribute, sublicense, and/or sell copies of the Software, and to
-permit persons to whom the Software is furnished to do so, subject to
-the following conditions:
+Copyright (c) 2024 Carl Schader
 
-The above copyright notice and this permission notice shall be
-included in all copies or substantial portions of the Software.
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
-NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
-LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
-WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+THE SOFTWARE.
```

### Comparing `labeled_contrastive_framework-0.1.0/PKG-INFO` & `labeled_contrastive_framework-0.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: labeled_contrastive_framework
-Version: 0.1.0
+Version: 0.2.0
 Summary: Framework for training contrastive models with labeled data using arcface loss.
 Author-email: Carl Schader <carlschader@gmail.com>
 Project-URL: Homepage, https://github.com/carlschader/ssl_framework
 Project-URL: Issues, https://github.com/carlschader/ssl_framework/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch>=2.0.0
 Requires-Dist: torchvision>=0.17.0
+Requires-Dist: pytorch-lightning>=2.2.0
```

### Comparing `labeled_contrastive_framework-0.1.0/labeled_contrastive_framework.egg-info/PKG-INFO` & `labeled_contrastive_framework-0.2.0/labeled_contrastive_framework.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: labeled_contrastive_framework
-Version: 0.1.0
+Version: 0.2.0
 Summary: Framework for training contrastive models with labeled data using arcface loss.
 Author-email: Carl Schader <carlschader@gmail.com>
 Project-URL: Homepage, https://github.com/carlschader/ssl_framework
 Project-URL: Issues, https://github.com/carlschader/ssl_framework/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch>=2.0.0
 Requires-Dist: torchvision>=0.17.0
+Requires-Dist: pytorch-lightning>=2.2.0
```

### Comparing `labeled_contrastive_framework-0.1.0/pyproject.toml` & `labeled_contrastive_framework-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "labeled_contrastive_framework"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
   { name="Carl Schader", email="carlschader@gmail.com" },
 ]
 description = "Framework for training contrastive models with labeled data using arcface loss."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "torch >= 2.0.0",
     "torchvision >= 0.17.0",
+    "pytorch-lightning >= 2.2.0",
 ]
 
 [project.urls]
 Homepage = "https://github.com/carlschader/ssl_framework"
 Issues = "https://github.com/carlschader/ssl_framework/issues"
 
 [tool.setuptools.packages.find]
 # All the following settings are optional:
 where = ["."]  # ["."] by default
-include = ["src/*"]  # ["*"] by default
+include = ["labeled_contrastive_framework"]  # ["*"] by default
 exclude = ["scripts"]  # empty by default
```

