# Comparing `tmp/step_in_line-0.5.0.tar.gz` & `tmp/step_in_line-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "step_in_line-0.5.0.tar", max compression
+gzip compressed data, was "step_in_line-0.5.1.tar", max compression
```

## Comparing `step_in_line-0.5.0.tar` & `step_in_line-0.5.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2024-04-25 00:43:45.400320 step_in_line-0.5.0/LICENSE
--rw-r--r--   0        0        0     5879 2024-04-25 00:43:45.400320 step_in_line-0.5.0/README.md
--rw-r--r--   0        0        0      505 2024-04-25 00:44:00.884309 step_in_line-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-25 00:43:45.400320 step_in_line-0.5.0/step_in_line/__init__.py
--rw-r--r--   0        0        0     5160 2024-04-25 00:43:45.404320 step_in_line-0.5.0/step_in_line/pipeline.py
--rw-r--r--   0        0        0     4818 2024-04-25 00:43:45.404320 step_in_line-0.5.0/step_in_line/step.py
--rw-r--r--   0        0        0     1729 2024-04-25 00:43:45.404320 step_in_line-0.5.0/step_in_line/template_lambda.py
--rw-r--r--   0        0        0    14445 2024-04-25 00:43:45.404320 step_in_line-0.5.0/step_in_line/tf.py
--rw-r--r--   0        0        0     6544 1970-01-01 00:00:00.000000 step_in_line-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-25 00:54:58.430348 step_in_line-0.5.1/LICENSE
+-rw-r--r--   0        0        0     5904 2024-04-25 00:54:58.430348 step_in_line-0.5.1/README.md
+-rw-r--r--   0        0        0      505 2024-04-25 00:55:12.262416 step_in_line-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-25 00:54:58.430348 step_in_line-0.5.1/step_in_line/__init__.py
+-rw-r--r--   0        0        0     5160 2024-04-25 00:54:58.430348 step_in_line-0.5.1/step_in_line/pipeline.py
+-rw-r--r--   0        0        0     4818 2024-04-25 00:54:58.430348 step_in_line-0.5.1/step_in_line/step.py
+-rw-r--r--   0        0        0     1729 2024-04-25 00:54:58.430348 step_in_line-0.5.1/step_in_line/template_lambda.py
+-rw-r--r--   0        0        0    14445 2024-04-25 00:54:58.430348 step_in_line-0.5.1/step_in_line/tf.py
+-rw-r--r--   0        0        0     6569 1970-01-01 00:00:00.000000 step_in_line-0.5.1/PKG-INFO
```

### Comparing `step_in_line-0.5.0/LICENSE` & `step_in_line-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `step_in_line-0.5.0/README.md` & `step_in_line-0.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 ### Example Pipeline
 ```python
 from cdktf import App
 from step_in_line.step import step
 from step_in_line.pipeline import Pipeline
 from step_in_line.tf import StepInLine, rename_tf_output
+from pathlib import Path
 
 app = App(hcl_output=True)
 
 # function names must be unique, or you can pass a name to the step to 
 # ensure uniqueness
 @step(
     name = "preprocess_unique",
```

### Comparing `step_in_line-0.5.0/step_in_line/pipeline.py` & `step_in_line-0.5.1/step_in_line/pipeline.py`

 * *Files identical despite different names*

### Comparing `step_in_line-0.5.0/step_in_line/step.py` & `step_in_line-0.5.1/step_in_line/step.py`

 * *Files identical despite different names*

### Comparing `step_in_line-0.5.0/step_in_line/template_lambda.py` & `step_in_line-0.5.1/step_in_line/template_lambda.py`

 * *Files identical despite different names*

### Comparing `step_in_line-0.5.0/step_in_line/tf.py` & `step_in_line-0.5.1/step_in_line/tf.py`

 * *Files identical despite different names*

### Comparing `step_in_line-0.5.0/PKG-INFO` & `step_in_line-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: step-in-line
-Version: 0.5.0
+Version: 0.5.1
 Summary: 
 Author: Daniel Stahl
 Author-email: danstahl1138@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -30,14 +30,15 @@
 
 ### Example Pipeline
 ```python
 from cdktf import App
 from step_in_line.step import step
 from step_in_line.pipeline import Pipeline
 from step_in_line.tf import StepInLine, rename_tf_output
+from pathlib import Path
 
 app = App(hcl_output=True)
 
 # function names must be unique, or you can pass a name to the step to 
 # ensure uniqueness
 @step(
     name = "preprocess_unique",
```

