# Comparing `tmp/helmet-0.1.2.tar.gz` & `tmp/helmet-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helmet-0.1.2.tar", max compression
+gzip compressed data, was "helmet-1.0.1.tar", max compression
```

## Comparing `helmet-0.1.2.tar` & `helmet-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1205 2024-04-23 09:39:41.032230 helmet-0.1.2/README.md
--rw-r--r--   0        0        0      497 2024-04-23 11:25:34.267289 helmet-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2173 2024-04-23 11:48:07.925589 helmet-0.1.2/src/helmet/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 15:03:40.081201 helmet-0.1.2/src/helmet/explainers/__init__.py
--rw-r--r--   0        0        0     5236 2024-04-23 09:39:41.040600 helmet-0.1.2/src/helmet/explainers/gradients.py
--rw-r--r--   0        0        0      630 2024-04-22 15:03:40.082765 helmet-0.1.2/src/helmet/explainers/perturbation.py
--rw-r--r--   0        0        0       49 2024-04-22 15:03:40.083280 helmet-0.1.2/src/helmet/model/__init__.py
--rw-r--r--   0        0        0     3402 2024-04-23 08:24:42.095619 helmet-0.1.2/src/helmet/model/base_lm.py
--rw-r--r--   0        0        0     6942 2024-04-23 13:34:24.625940 helmet-0.1.2/src/helmet/model/dec_lm.py
--rw-r--r--   0        0        0     3888 2024-04-23 09:54:26.292511 helmet-0.1.2/src/helmet/updater.py
--rw-r--r--   0        0        0       79 2024-04-22 15:03:40.087155 helmet-0.1.2/src/helmet/utils/constants.py
--rw-r--r--   0        0        0     3277 2024-04-23 13:34:24.627631 helmet-0.1.2/src/helmet/utils/types.py
--rw-r--r--   0        0        0      130 2024-04-22 15:03:40.089028 helmet-0.1.2/src/helmet/utils/utils.py
--rw-r--r--   0        0        0     1965 1970-01-01 00:00:00.000000 helmet-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1279 2024-04-24 07:27:14.185772 helmet-1.0.1/README.md
+-rw-r--r--   0        0        0      497 2024-04-24 07:27:14.185772 helmet-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2173 2024-04-24 07:27:14.185772 helmet-1.0.1/src/helmet/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 07:27:14.185772 helmet-1.0.1/src/helmet/explainers/__init__.py
+-rw-r--r--   0        0        0     5236 2024-04-24 07:27:14.185772 helmet-1.0.1/src/helmet/explainers/gradients.py
+-rw-r--r--   0        0        0      630 2024-04-24 07:27:14.185772 helmet-1.0.1/src/helmet/explainers/perturbation.py
+-rw-r--r--   0        0        0       49 2024-04-24 07:27:14.185772 helmet-1.0.1/src/helmet/model/__init__.py
+-rw-r--r--   0        0        0     3402 2024-04-24 07:27:14.185772 helmet-1.0.1/src/helmet/model/base_lm.py
+-rw-r--r--   0        0        0     6942 2024-04-24 07:27:14.185772 helmet-1.0.1/src/helmet/model/dec_lm.py
+-rw-r--r--   0        0        0     3888 2024-04-24 07:27:14.185772 helmet-1.0.1/src/helmet/updater.py
+-rw-r--r--   0        0        0       79 2024-04-24 07:27:14.185772 helmet-1.0.1/src/helmet/utils/constants.py
+-rw-r--r--   0        0        0     3277 2024-04-24 07:27:14.185772 helmet-1.0.1/src/helmet/utils/types.py
+-rw-r--r--   0        0        0      130 2024-04-24 07:27:14.185772 helmet-1.0.1/src/helmet/utils/utils.py
+-rw-r--r--   0        0        0     2039 1970-01-01 00:00:00.000000 helmet-1.0.1/PKG-INFO
```

### Comparing `helmet-0.1.2/README.md` & `helmet-1.0.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -29,15 +29,22 @@
 
 1. `deactivate`
 2. `jupyter-kernelspec uninstall venv`
 3. `rm -r venv`
 
 ## Configuration files
 
-- Project configuration
+### Project configuration
+
+```python
+project_config = {
+    platform_url: "localhost:4000"
+}
+```
+
 - Model configuration
 - Run configuration
 
 ## Features
 
 - Load any causal model from Huggingface.
 - Create a project for your experiment
```

### Comparing `helmet-0.1.2/src/helmet/__init__.py` & `helmet-1.0.1/src/helmet/__init__.py`

 * *Files identical despite different names*

### Comparing `helmet-0.1.2/src/helmet/explainers/gradients.py` & `helmet-1.0.1/src/helmet/explainers/gradients.py`

 * *Files identical despite different names*

### Comparing `helmet-0.1.2/src/helmet/explainers/perturbation.py` & `helmet-1.0.1/src/helmet/explainers/perturbation.py`

 * *Files identical despite different names*

### Comparing `helmet-0.1.2/src/helmet/model/base_lm.py` & `helmet-1.0.1/src/helmet/model/base_lm.py`

 * *Files identical despite different names*

### Comparing `helmet-0.1.2/src/helmet/model/dec_lm.py` & `helmet-1.0.1/src/helmet/model/dec_lm.py`

 * *Files identical despite different names*

### Comparing `helmet-0.1.2/src/helmet/updater.py` & `helmet-1.0.1/src/helmet/updater.py`

 * *Files identical despite different names*

### Comparing `helmet-0.1.2/src/helmet/utils/types.py` & `helmet-1.0.1/src/helmet/utils/types.py`

 * *Files identical despite different names*

### Comparing `helmet-0.1.2/PKG-INFO` & `helmet-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helmet
-Version: 0.1.2
+Version: 1.0.1
 Summary: 
 Author: Jeroen
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -51,15 +51,22 @@
 
 1. `deactivate`
 2. `jupyter-kernelspec uninstall venv`
 3. `rm -r venv`
 
 ## Configuration files
 
-- Project configuration
+### Project configuration
+
+```python
+project_config = {
+    platform_url: "localhost:4000"
+}
+```
+
 - Model configuration
 - Run configuration
 
 ## Features
 
 - Load any causal model from Huggingface.
 - Create a project for your experiment
```

