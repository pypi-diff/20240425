# Comparing `tmp/kuflow_temporal_activity_kuflow-1.5.0.tar.gz` & `tmp/kuflow_temporal_activity_kuflow-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuflow_temporal_activity_kuflow-1.5.0.tar", max compression
+gzip compressed data, was "kuflow_temporal_activity_kuflow-1.5.1.tar", max compression
```

## Comparing `kuflow_temporal_activity_kuflow-1.5.0.tar` & `kuflow_temporal_activity_kuflow-1.5.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      878 2024-04-09 11:44:28.833042 kuflow_temporal_activity_kuflow-1.5.0/README.md
--rw-r--r--   0        0        0        6 2024-04-09 11:44:28.833042 kuflow_temporal_activity_kuflow-1.5.0/VERSION
--rw-r--r--   0        0        0     1325 2024-04-09 11:44:28.833042 kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/__init__.py
--rw-r--r--   0        0        0     9152 2024-04-09 11:44:28.833042 kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/_validation.py
--rw-r--r--   0        0        0     4932 2024-04-09 11:44:28.833042 kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/converter.py
--rw-r--r--   0        0        0    16373 2024-04-09 11:44:28.833042 kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/kuflow_activities.py
--rw-r--r--   0        0        0     3803 2024-04-09 11:44:28.833042 kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/models/__init__.py
--rw-r--r--   0        0        0     2133 2024-04-09 11:50:16.973127 kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/models/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    23527 2024-04-09 11:50:16.973127 kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/models/__pycache__/_models.cpython-38.pyc
--rw-r--r--   0        0        0    23017 2024-04-09 11:44:28.833042 kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/models/_models.py
--rw-r--r--   0        0        0     1463 2024-04-09 11:44:28.833042 kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/utils/__init__.py
--rw-r--r--   0        0        0      499 2024-04-09 11:50:17.025128 kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/utils/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    10493 2024-04-09 11:50:17.025128 kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/utils/__pycache__/_save_process_element_utils.cpython-38.pyc
--rw-r--r--   0        0        0    13245 2024-04-09 11:50:17.029128 kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/utils/__pycache__/_save_task_element_utils.cpython-38.pyc
--rw-r--r--   0        0        0    14343 2024-04-09 11:50:17.029128 kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/utils/__pycache__/_save_task_json_forms_value_data_request_utils.cpython-38.pyc
--rw-r--r--   0        0        0    11189 2024-04-09 11:44:28.833042 kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/utils/_save_process_element_utils.py
--rw-r--r--   0        0        0    14055 2024-04-09 11:44:28.833042 kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/utils/_save_task_element_utils.py
--rw-r--r--   0        0        0    15409 2024-04-09 11:44:28.833042 kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/utils/_save_task_json_forms_value_data_request_utils.py
--rw-r--r--   0        0        0      939 2024-04-09 11:50:39.177383 kuflow_temporal_activity_kuflow-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     1705 1970-01-01 00:00:00.000000 kuflow_temporal_activity_kuflow-1.5.0/setup.py
--rw-r--r--   0        0        0     1667 1970-01-01 00:00:00.000000 kuflow_temporal_activity_kuflow-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0      878 2024-04-25 11:49:37.325017 kuflow_temporal_activity_kuflow-1.5.1/README.md
+-rw-r--r--   0        0        0        6 2024-04-25 11:49:37.325017 kuflow_temporal_activity_kuflow-1.5.1/VERSION
+-rw-r--r--   0        0        0     1325 2024-04-25 11:49:37.325017 kuflow_temporal_activity_kuflow-1.5.1/kuflow_temporal_activity_kuflow/__init__.py
+-rw-r--r--   0        0        0     9152 2024-04-25 11:49:37.325017 kuflow_temporal_activity_kuflow-1.5.1/kuflow_temporal_activity_kuflow/_validation.py
+-rw-r--r--   0        0        0     4932 2024-04-25 11:49:37.325017 kuflow_temporal_activity_kuflow-1.5.1/kuflow_temporal_activity_kuflow/converter.py
+-rw-r--r--   0        0        0    16373 2024-04-25 11:49:37.325017 kuflow_temporal_activity_kuflow-1.5.1/kuflow_temporal_activity_kuflow/kuflow_activities.py
+-rw-r--r--   0        0        0     3803 2024-04-25 11:49:37.325017 kuflow_temporal_activity_kuflow-1.5.1/kuflow_temporal_activity_kuflow/models/__init__.py
+-rw-r--r--   0        0        0     2133 2024-04-25 11:56:39.000056 kuflow_temporal_activity_kuflow-1.5.1/kuflow_temporal_activity_kuflow/models/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    23527 2024-04-25 11:56:39.004056 kuflow_temporal_activity_kuflow-1.5.1/kuflow_temporal_activity_kuflow/models/__pycache__/_models.cpython-38.pyc
+-rw-r--r--   0        0        0    23017 2024-04-25 11:49:37.325017 kuflow_temporal_activity_kuflow-1.5.1/kuflow_temporal_activity_kuflow/models/_models.py
+-rw-r--r--   0        0        0     1463 2024-04-25 11:49:37.325017 kuflow_temporal_activity_kuflow-1.5.1/kuflow_temporal_activity_kuflow/utils/__init__.py
+-rw-r--r--   0        0        0      499 2024-04-25 11:56:39.036056 kuflow_temporal_activity_kuflow-1.5.1/kuflow_temporal_activity_kuflow/utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    10493 2024-04-25 11:56:39.036056 kuflow_temporal_activity_kuflow-1.5.1/kuflow_temporal_activity_kuflow/utils/__pycache__/_save_process_element_utils.cpython-38.pyc
+-rw-r--r--   0        0        0    13245 2024-04-25 11:56:39.044056 kuflow_temporal_activity_kuflow-1.5.1/kuflow_temporal_activity_kuflow/utils/__pycache__/_save_task_element_utils.cpython-38.pyc
+-rw-r--r--   0        0        0    14343 2024-04-25 11:56:39.044056 kuflow_temporal_activity_kuflow-1.5.1/kuflow_temporal_activity_kuflow/utils/__pycache__/_save_task_json_forms_value_data_request_utils.cpython-38.pyc
+-rw-r--r--   0        0        0    11189 2024-04-25 11:49:37.325017 kuflow_temporal_activity_kuflow-1.5.1/kuflow_temporal_activity_kuflow/utils/_save_process_element_utils.py
+-rw-r--r--   0        0        0    14055 2024-04-25 11:49:37.325017 kuflow_temporal_activity_kuflow-1.5.1/kuflow_temporal_activity_kuflow/utils/_save_task_element_utils.py
+-rw-r--r--   0        0        0    15409 2024-04-25 11:49:37.325017 kuflow_temporal_activity_kuflow-1.5.1/kuflow_temporal_activity_kuflow/utils/_save_task_json_forms_value_data_request_utils.py
+-rw-r--r--   0        0        0      939 2024-04-25 11:56:59.392199 kuflow_temporal_activity_kuflow-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1705 1970-01-01 00:00:00.000000 kuflow_temporal_activity_kuflow-1.5.1/setup.py
+-rw-r--r--   0        0        0     1667 1970-01-01 00:00:00.000000 kuflow_temporal_activity_kuflow-1.5.1/PKG-INFO
```

### Comparing `kuflow_temporal_activity_kuflow-1.5.0/README.md` & `kuflow_temporal_activity_kuflow-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/__init__.py` & `kuflow_temporal_activity_kuflow-1.5.1/kuflow_temporal_activity_kuflow/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,8 +24,8 @@
 
 from .kuflow_activities import KuFlowActivities
 
 
 KUFLOW_ENGINE_SIGNAL_COMPLETED_TASK = "KuFlow_Engine_Signal_Completed_Task"
 
 __all__ = ["KuFlowActivities", "KUFLOW_ENGINE_SIGNAL_COMPLETED_TASK"]
-__version__ = "1.5.0"
+__version__ = "1.5.1"
```

### Comparing `kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/_validation.py` & `kuflow_temporal_activity_kuflow-1.5.1/kuflow_temporal_activity_kuflow/_validation.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/converter.py` & `kuflow_temporal_activity_kuflow-1.5.1/kuflow_temporal_activity_kuflow/converter.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/kuflow_activities.py` & `kuflow_temporal_activity_kuflow-1.5.1/kuflow_temporal_activity_kuflow/kuflow_activities.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/models/__init__.py` & `kuflow_temporal_activity_kuflow-1.5.1/kuflow_temporal_activity_kuflow/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/models/__pycache__/__init__.cpython-38.pyc` & `kuflow_temporal_activity_kuflow-1.5.1/kuflow_temporal_activity_kuflow/models/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 3803 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 db0e 0000  U........*.f....
+00000000: 550d 0d0a 0000 0000 5143 2a66 db0e 0000  U.......QC*f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 002c 0000 0040 0000 0073 1801 0000 6400  .,...@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 6d07 5a07  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d10 5a10 6d11 5a11 6d12 5a12 6d13 5a13  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/models/__pycache__/_models.cpython-38.pyc` & `kuflow_temporal_activity_kuflow-1.5.1/kuflow_temporal_activity_kuflow/models/__pycache__/_models.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 23017 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 e959 0000  U........*.f.Y..
+00000000: 550d 0d0a 0000 0000 5143 2a66 e959 0000  U.......QC*f.Y..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4c03 0000 6400  .....@...sL...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6400 6402 6c05 6d06 5a07  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6403 6c08 6d09 5a09 0100 4700  ..d.d.l.m.Z...G.
 00000060: 6404 6405 8400 6405 6509 6a0a 8303 5a0b  d.d...d.e.j...Z.
 00000070: 4700 6406 6407 8400 6407 6509 6a0a 8303  G.d.d...d.e.j...
```

### Comparing `kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/models/_models.py` & `kuflow_temporal_activity_kuflow-1.5.1/kuflow_temporal_activity_kuflow/models/_models.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/utils/__init__.py` & `kuflow_temporal_activity_kuflow-1.5.1/kuflow_temporal_activity_kuflow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/utils/__pycache__/_save_process_element_utils.cpython-38.pyc` & `kuflow_temporal_activity_kuflow-1.5.1/kuflow_temporal_activity_kuflow/utils/__pycache__/_save_process_element_utils.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 11189 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 b52b 0000  U........*.f.+..
+00000000: 550d 0d0a 0000 0000 5143 2a66 b52b 0000  U.......QC*f.+..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 c200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6400 6405 6c0b  m.Z.m.Z...d.d.l.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/utils/__pycache__/_save_task_element_utils.cpython-38.pyc` & `kuflow_temporal_activity_kuflow-1.5.1/kuflow_temporal_activity_kuflow/utils/__pycache__/_save_task_element_utils.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 14055 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 e736 0000  U........*.f.6..
+00000000: 550d 0d0a 0000 0000 5143 2a66 e736 0000  U.......QC*f.6..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 e200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 6400  m.Z.m.Z.m.Z...d.
 00000060: 6404 6c09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  d.l.m.Z.m.Z.m.Z.
 00000070: 0100 6400 6405 6c0d 6d0e 5a0e 6d0f 5a0f  ..d.d.l.m.Z.m.Z.
```

### Comparing `kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/utils/__pycache__/_save_task_json_forms_value_data_request_utils.cpython-38.pyc` & `kuflow_temporal_activity_kuflow-1.5.1/kuflow_temporal_activity_kuflow/utils/__pycache__/_save_task_json_forms_value_data_request_utils.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 15409 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 313c 0000  U........*.f1<..
+00000000: 550d 0d0a 0000 0000 5143 2a66 313c 0000  U.......QC*f1<..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 be00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d00 5a00 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 6d05 5a05  d.l.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6403 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6400 6404 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/utils/_save_process_element_utils.py` & `kuflow_temporal_activity_kuflow-1.5.1/kuflow_temporal_activity_kuflow/utils/_save_process_element_utils.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/utils/_save_task_element_utils.py` & `kuflow_temporal_activity_kuflow-1.5.1/kuflow_temporal_activity_kuflow/utils/_save_task_element_utils.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/utils/_save_task_json_forms_value_data_request_utils.py` & `kuflow_temporal_activity_kuflow-1.5.1/kuflow_temporal_activity_kuflow/utils/_save_task_json_forms_value_data_request_utils.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-1.5.0/pyproject.toml` & `kuflow_temporal_activity_kuflow-1.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kuflow-temporal-activity-kuflow"
-version = "1.5.0"
+version = "1.5.1"
 description = "KuFlow SDK :: Temporal.io activities to interact with KuFlow"
 license = "MIT"
 authors = ["KuFlow S.L. <kuflow@kuflow.com>"]
 homepage = "https://kuflow.com/"
 documentation = "https://docs.kuflow.com/"
 repository = "https://github.com/kuflow/kuflow-sdk-python"
 readme = "README.md"
@@ -13,15 +13,15 @@
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-kuflow-temporal-common = "^1.5.0"
+kuflow-temporal-common = "^1.5.1"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.3.0"
 ruff = ">=0.1.8,<1.0.0"
 pytest = "^7.3.1"
 pyyaml = "^6.0"
```

### Comparing `kuflow_temporal_activity_kuflow-1.5.0/setup.py` & `kuflow_temporal_activity_kuflow-1.5.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,19 +6,19 @@
  'kuflow_temporal_activity_kuflow.models',
  'kuflow_temporal_activity_kuflow.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['kuflow-temporal-common>=1.5.0,<2.0.0']
+['kuflow-temporal-common>=1.5.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'kuflow-temporal-activity-kuflow',
-    'version': '1.5.0',
+    'version': '1.5.1',
     'description': 'KuFlow SDK :: Temporal.io activities to interact with KuFlow',
     'long_description': '[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n[![Python](https://img.shields.io/pypi/pyversions/kuflow-temporal-activity-kuflow.svg)](https://pypi.org/project/kuflow-temporal-activity-kuflow)\n[![PyPI](https://img.shields.io/pypi/v/kuflow-temporal-activity-kuflow.svg)](https://pypi.org/project/kuflow-temporal-activity-kuflow)\n\n# KuFlow Temporal Activities KuFlow\n\nTemporal.io activities to interact with KuFlow\n\n## Documentation\n\nMore detailed docs are available in the [documentation pages](https://docs.kuflow.com/developers/).\n\n## Contributing\n\nWe are happy to receive your help and comments, together we will dance a wonderful KuFlow. Please review our [contribution guide](CONTRIBUTING.md).\n\n## License\n\n[MIT License](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n',
     'author': 'KuFlow S.L.',
     'author_email': 'kuflow@kuflow.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kuflow.com/',
```

### Comparing `kuflow_temporal_activity_kuflow-1.5.0/PKG-INFO` & `kuflow_temporal_activity_kuflow-1.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: kuflow-temporal-activity-kuflow
-Version: 1.5.0
+Version: 1.5.1
 Summary: KuFlow SDK :: Temporal.io activities to interact with KuFlow
 Home-page: https://kuflow.com/
 License: MIT
 Author: KuFlow S.L.
 Author-email: kuflow@kuflow.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: kuflow-temporal-common (>=1.5.0,<2.0.0)
+Requires-Dist: kuflow-temporal-common (>=1.5.1,<2.0.0)
 Project-URL: Documentation, https://docs.kuflow.com/
 Project-URL: Repository, https://github.com/kuflow/kuflow-sdk-python
 Description-Content-Type: text/markdown
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)
 [![Python](https://img.shields.io/pypi/pyversions/kuflow-temporal-activity-kuflow.svg)](https://pypi.org/project/kuflow-temporal-activity-kuflow)
 [![PyPI](https://img.shields.io/pypi/v/kuflow-temporal-activity-kuflow.svg)](https://pypi.org/project/kuflow-temporal-activity-kuflow)
```

