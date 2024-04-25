# Comparing `tmp/openlayer-0.1.0a8.tar.gz` & `tmp/openlayer-0.1.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlayer-0.1.0a8.tar", last modified: Mon Sep 25 07:04:55 2023, max compression
+gzip compressed data, was "openlayer-0.1.0a9.tar", last modified: Fri Sep 29 05:25:33 2023, max compression
```

## Comparing `openlayer-0.1.0a8.tar` & `openlayer-0.1.0a9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 07:04:55.435314 openlayer-0.1.0a8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-09-25 07:03:57.000000 openlayer-0.1.0a8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2023-09-25 07:04:55.435314 openlayer-0.1.0a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2023-09-25 07:03:57.000000 openlayer-0.1.0a8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 07:04:55.431314 openlayer-0.1.0a8/openlayer/
--rw-r--r--   0 runner    (1001) docker     (127)    53476 2023-09-25 07:03:57.000000 openlayer-0.1.0a8/openlayer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11117 2023-09-25 07:03:57.000000 openlayer-0.1.0a8/openlayer/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2023-09-25 07:03:57.000000 openlayer-0.1.0a8/openlayer/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2023-09-25 07:03:57.000000 openlayer-0.1.0a8/openlayer/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2023-09-25 07:03:57.000000 openlayer-0.1.0a8/openlayer/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 07:04:55.431314 openlayer-0.1.0a8/openlayer/model_runners/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-25 07:03:57.000000 openlayer-0.1.0a8/openlayer/model_runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2023-09-25 07:03:57.000000 openlayer-0.1.0a8/openlayer/model_runners/base_model_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     8088 2023-09-25 07:03:57.000000 openlayer-0.1.0a8/openlayer/model_runners/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    22788 2023-09-25 07:03:57.000000 openlayer-0.1.0a8/openlayer/model_runners/ll_model_runners.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 07:04:55.431314 openlayer-0.1.0a8/openlayer/model_runners/prediction_jobs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-25 07:03:57.000000 openlayer-0.1.0a8/openlayer/model_runners/prediction_jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2023-09-25 07:03:57.000000 openlayer-0.1.0a8/openlayer/model_runners/prediction_jobs/classification_prediction_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2023-09-25 07:03:57.000000 openlayer-0.1.0a8/openlayer/model_runners/prediction_jobs/regression_prediction_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2023-09-25 07:03:57.000000 openlayer-0.1.0a8/openlayer/model_runners/traditional_ml_model_runners.py
--rw-r--r--   0 runner    (1001) docker     (127)     7015 2023-09-25 07:03:57.000000 openlayer-0.1.0a8/openlayer/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4936 2023-09-25 07:03:57.000000 openlayer-0.1.0a8/openlayer/project_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2023-09-25 07:03:57.000000 openlayer-0.1.0a8/openlayer/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)    14287 2023-09-25 07:03:57.000000 openlayer-0.1.0a8/openlayer/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2023-09-25 07:03:57.000000 openlayer-0.1.0a8/openlayer/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6570 2023-09-25 07:03:57.000000 openlayer-0.1.0a8/openlayer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 07:04:55.435314 openlayer-0.1.0a8/openlayer/validators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-25 07:03:57.000000 openlayer-0.1.0a8/openlayer/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3832 2023-09-25 07:03:57.000000 openlayer-0.1.0a8/openlayer/validators/base_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2023-09-25 07:03:57.000000 openlayer-0.1.0a8/openlayer/validators/baseline_model_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)    28952 2023-09-25 07:03:57.000000 openlayer-0.1.0a8/openlayer/validators/commit_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)    35757 2023-09-25 07:03:57.000000 openlayer-0.1.0a8/openlayer/validators/dataset_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)    26116 2023-09-25 07:03:57.000000 openlayer-0.1.0a8/openlayer/validators/model_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2023-09-25 07:03:57.000000 openlayer-0.1.0a8/openlayer/validators/project_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2023-09-25 07:03:57.000000 openlayer-0.1.0a8/openlayer/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 07:04:55.431314 openlayer-0.1.0a8/openlayer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2023-09-25 07:04:55.000000 openlayer-0.1.0a8/openlayer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2023-09-25 07:04:55.000000 openlayer-0.1.0a8/openlayer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-25 07:04:55.000000 openlayer-0.1.0a8/openlayer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-25 07:04:55.000000 openlayer-0.1.0a8/openlayer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      149 2023-09-25 07:04:55.000000 openlayer-0.1.0a8/openlayer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-09-25 07:04:55.000000 openlayer-0.1.0a8/openlayer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2023-09-25 07:03:57.000000 openlayer-0.1.0a8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2023-09-25 07:04:55.435314 openlayer-0.1.0a8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       93 2023-09-25 07:03:57.000000 openlayer-0.1.0a8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 07:04:55.435314 openlayer-0.1.0a8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2023-09-25 07:03:57.000000 openlayer-0.1.0a8/tests/test_openlayer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 05:25:33.180608 openlayer-0.1.0a9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-09-29 05:24:35.000000 openlayer-0.1.0a9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2023-09-29 05:25:33.180608 openlayer-0.1.0a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2023-09-29 05:24:35.000000 openlayer-0.1.0a9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 05:25:33.180608 openlayer-0.1.0a9/openlayer/
+-rw-r--r--   0 runner    (1001) docker     (127)    53476 2023-09-29 05:24:35.000000 openlayer-0.1.0a9/openlayer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11117 2023-09-29 05:24:35.000000 openlayer-0.1.0a9/openlayer/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2023-09-29 05:24:35.000000 openlayer-0.1.0a9/openlayer/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2023-09-29 05:24:35.000000 openlayer-0.1.0a9/openlayer/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2023-09-29 05:24:35.000000 openlayer-0.1.0a9/openlayer/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 05:25:33.180608 openlayer-0.1.0a9/openlayer/model_runners/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-29 05:24:35.000000 openlayer-0.1.0a9/openlayer/model_runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2023-09-29 05:24:35.000000 openlayer-0.1.0a9/openlayer/model_runners/base_model_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8088 2023-09-29 05:24:35.000000 openlayer-0.1.0a9/openlayer/model_runners/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22788 2023-09-29 05:24:35.000000 openlayer-0.1.0a9/openlayer/model_runners/ll_model_runners.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 05:25:33.180608 openlayer-0.1.0a9/openlayer/model_runners/prediction_jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-29 05:24:35.000000 openlayer-0.1.0a9/openlayer/model_runners/prediction_jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2023-09-29 05:24:35.000000 openlayer-0.1.0a9/openlayer/model_runners/prediction_jobs/classification_prediction_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2023-09-29 05:24:35.000000 openlayer-0.1.0a9/openlayer/model_runners/prediction_jobs/regression_prediction_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2023-09-29 05:24:35.000000 openlayer-0.1.0a9/openlayer/model_runners/traditional_ml_model_runners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7015 2023-09-29 05:24:35.000000 openlayer-0.1.0a9/openlayer/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4936 2023-09-29 05:24:35.000000 openlayer-0.1.0a9/openlayer/project_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2023-09-29 05:24:35.000000 openlayer-0.1.0a9/openlayer/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14287 2023-09-29 05:24:35.000000 openlayer-0.1.0a9/openlayer/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2023-09-29 05:24:35.000000 openlayer-0.1.0a9/openlayer/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6570 2023-09-29 05:24:35.000000 openlayer-0.1.0a9/openlayer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 05:25:33.180608 openlayer-0.1.0a9/openlayer/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-29 05:24:35.000000 openlayer-0.1.0a9/openlayer/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3832 2023-09-29 05:24:35.000000 openlayer-0.1.0a9/openlayer/validators/base_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2023-09-29 05:24:35.000000 openlayer-0.1.0a9/openlayer/validators/baseline_model_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28672 2023-09-29 05:24:35.000000 openlayer-0.1.0a9/openlayer/validators/commit_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35757 2023-09-29 05:24:35.000000 openlayer-0.1.0a9/openlayer/validators/dataset_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26116 2023-09-29 05:24:35.000000 openlayer-0.1.0a9/openlayer/validators/model_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2023-09-29 05:24:35.000000 openlayer-0.1.0a9/openlayer/validators/project_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2023-09-29 05:24:35.000000 openlayer-0.1.0a9/openlayer/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 05:25:33.180608 openlayer-0.1.0a9/openlayer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2023-09-29 05:25:33.000000 openlayer-0.1.0a9/openlayer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2023-09-29 05:25:33.000000 openlayer-0.1.0a9/openlayer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-29 05:25:33.000000 openlayer-0.1.0a9/openlayer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-29 05:25:33.000000 openlayer-0.1.0a9/openlayer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2023-09-29 05:25:33.000000 openlayer-0.1.0a9/openlayer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2023-09-29 05:25:33.000000 openlayer-0.1.0a9/openlayer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2023-09-29 05:24:35.000000 openlayer-0.1.0a9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2023-09-29 05:25:33.184608 openlayer-0.1.0a9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2023-09-29 05:24:35.000000 openlayer-0.1.0a9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 05:25:33.180608 openlayer-0.1.0a9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2023-09-29 05:24:35.000000 openlayer-0.1.0a9/tests/test_openlayer.py
```

### Comparing `openlayer-0.1.0a8/LICENSE` & `openlayer-0.1.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a8/PKG-INFO` & `openlayer-0.1.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlayer
-Version: 0.1.0a8
+Version: 0.1.0a9
 Summary: The official Python API library for Openlayer: the Testing and Debugging Platform for AI
 Home-page: https://github.com/openlayer-ai/openlayer-python
 Author: Unbox Inc.
 Project-URL: Documentation, https://docs.openlayer.com/
 Project-URL: Openlayer User Slack Group, https://l.linklyhq.com/l/1DG73
 Keywords: MLOps,AI,Openlayer
 Classifier: Operating System :: OS Independent
```

### Comparing `openlayer-0.1.0a8/README.md` & `openlayer-0.1.0a9/README.md`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a8/openlayer/__init__.py` & `openlayer-0.1.0a9/openlayer/__init__.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a8/openlayer/api.py` & `openlayer-0.1.0a9/openlayer/api.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a8/openlayer/constants.py` & `openlayer-0.1.0a9/openlayer/constants.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a8/openlayer/datasets.py` & `openlayer-0.1.0a9/openlayer/datasets.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a8/openlayer/exceptions.py` & `openlayer-0.1.0a9/openlayer/exceptions.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a8/openlayer/model_runners/base_model_runner.py` & `openlayer-0.1.0a9/openlayer/model_runners/base_model_runner.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a8/openlayer/model_runners/environment.py` & `openlayer-0.1.0a9/openlayer/model_runners/environment.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a8/openlayer/model_runners/ll_model_runners.py` & `openlayer-0.1.0a9/openlayer/model_runners/ll_model_runners.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a8/openlayer/model_runners/prediction_jobs/classification_prediction_job.py` & `openlayer-0.1.0a9/openlayer/model_runners/prediction_jobs/classification_prediction_job.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a8/openlayer/model_runners/prediction_jobs/regression_prediction_job.py` & `openlayer-0.1.0a9/openlayer/model_runners/prediction_jobs/regression_prediction_job.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a8/openlayer/model_runners/traditional_ml_model_runners.py` & `openlayer-0.1.0a9/openlayer/model_runners/traditional_ml_model_runners.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a8/openlayer/models.py` & `openlayer-0.1.0a9/openlayer/models.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a8/openlayer/project_versions.py` & `openlayer-0.1.0a9/openlayer/project_versions.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a8/openlayer/projects.py` & `openlayer-0.1.0a9/openlayer/projects.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a8/openlayer/schemas.py` & `openlayer-0.1.0a9/openlayer/schemas.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a8/openlayer/tasks.py` & `openlayer-0.1.0a9/openlayer/tasks.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a8/openlayer/utils.py` & `openlayer-0.1.0a9/openlayer/utils.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a8/openlayer/validators/base_validator.py` & `openlayer-0.1.0a9/openlayer/validators/base_validator.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a8/openlayer/validators/baseline_model_validators.py` & `openlayer-0.1.0a9/openlayer/validators/baseline_model_validators.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a8/openlayer/validators/commit_validators.py` & `openlayer-0.1.0a9/openlayer/validators/commit_validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,31 +204,25 @@
                             "predictions. Please provide predictions for both datasets."
                         )
 
         else:
             if (
                 "training" in self._bundle_resources
                 or "fine-tuning" in self._bundle_resources
-            ) and "validation" not in self._bundle_resources:
+            ) and ("validation" not in self._bundle_resources):
                 if outputs_in_training_set:
                     self.failed_validations.append(
                         "The training/fine-tuning dataset contains predictions, but no model was"
                         " provided. To push a training/fine-tuning set with predictions, please provide"
                         " a model and a validation set with predictions as well."
                     )
             elif (
-                "training" not in self._bundle_resources
-                or "fine-tuning" not in self._bundle_resources
-            ) and "validation" in self._bundle_resources:
-                # This is allowed -- listed just for completeness
-                pass
-            elif (
                 "training" in self._bundle_resources
                 or "fine-tuning" in self._bundle_resources
-            ) and "validation" in self._bundle_resources:
+            ) and ("validation" in self._bundle_resources):
                 if outputs_in_training_set or outputs_in_validation_set:
                     self.failed_validations.append(
                         "You are trying to push a training/fine-tuning set and a validation set to the platform. "
                         "However, the training/fine-tuning or the validation set contain predictions. "
                         "To push datasets with predictions, please provide a model as well."
                     )
```

### Comparing `openlayer-0.1.0a8/openlayer/validators/dataset_validators.py` & `openlayer-0.1.0a9/openlayer/validators/dataset_validators.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a8/openlayer/validators/model_validators.py` & `openlayer-0.1.0a9/openlayer/validators/model_validators.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a8/openlayer/validators/project_validators.py` & `openlayer-0.1.0a9/openlayer/validators/project_validators.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a8/openlayer/version.py` & `openlayer-0.1.0a9/openlayer/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,8 +18,8 @@
          headers=headers,
          params=params,
          json=body,
          files=files,
          data=data,
       )
 """
-__version__ = "0.1.0a8"
+__version__ = "0.1.0a9"
```

### Comparing `openlayer-0.1.0a8/openlayer.egg-info/PKG-INFO` & `openlayer-0.1.0a9/openlayer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlayer
-Version: 0.1.0a8
+Version: 0.1.0a9
 Summary: The official Python API library for Openlayer: the Testing and Debugging Platform for AI
 Home-page: https://github.com/openlayer-ai/openlayer-python
 Author: Unbox Inc.
 Project-URL: Documentation, https://docs.openlayer.com/
 Project-URL: Openlayer User Slack Group, https://l.linklyhq.com/l/1DG73
 Keywords: MLOps,AI,Openlayer
 Classifier: Operating System :: OS Independent
```

### Comparing `openlayer-0.1.0a8/openlayer.egg-info/SOURCES.txt` & `openlayer-0.1.0a9/openlayer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a8/setup.cfg` & `openlayer-0.1.0a9/setup.cfg`

 * *Files identical despite different names*

