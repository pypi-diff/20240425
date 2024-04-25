# Comparing `tmp/reka_api-1.0.6.tar.gz` & `tmp/reka_api-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reka_api-1.0.6.tar", max compression
+gzip compressed data, was "reka_api-2.0.0.tar", max compression
```

## Comparing `reka_api-1.0.6.tar` & `reka_api-2.0.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0    25738 2024-04-16 10:47:55.120851 reka_api-1.0.6/LICENSE
--rw-r--r--   0        0        0      149 2024-04-16 10:47:55.120851 reka_api-1.0.6/README.md
--rw-r--r--   0        0        0     1125 2024-04-16 10:47:55.124851 reka_api-1.0.6/pyproject.toml
--rw-r--r--   0        0        0      825 2024-04-16 10:47:55.124851 reka_api-1.0.6/src/reka/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 10:47:55.124851 reka_api-1.0.6/src/reka/api/__init__.py
--rw-r--r--   0        0        0     7483 2024-04-16 10:47:55.124851 reka_api-1.0.6/src/reka/api/chat.py
--rw-r--r--   0        0        0     2481 2024-04-16 10:47:55.124851 reka_api-1.0.6/src/reka/api/completion.py
--rw-r--r--   0        0        0     2077 2024-04-16 10:47:55.124851 reka_api-1.0.6/src/reka/api/dataset.py
--rw-r--r--   0        0        0     2223 2024-04-16 10:47:55.124851 reka_api-1.0.6/src/reka/api/driver.py
--rw-r--r--   0        0        0      694 2024-04-16 10:47:55.124851 reka_api-1.0.6/src/reka/api/job.py
--rw-r--r--   0        0        0      373 2024-04-16 10:47:55.124851 reka_api-1.0.6/src/reka/api/models.py
--rw-r--r--   0        0        0     3563 2024-04-16 10:47:55.124851 reka_api-1.0.6/src/reka/api/retrieval.py
--rw-r--r--   0        0        0     1136 2024-04-16 10:47:55.124851 reka_api-1.0.6/src/reka/errors.py
--rw-r--r--   0        0        0        0 2024-04-16 10:47:55.124851 reka_api-1.0.6/src/reka/py.typed
--rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 reka_api-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0    25738 2024-04-25 14:11:13.751171 reka_api-2.0.0/LICENSE
+-rw-r--r--   0        0        0      149 2024-04-25 14:11:13.751171 reka_api-2.0.0/README.md
+-rw-r--r--   0        0        0     1125 2024-04-25 14:11:13.751171 reka_api-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      764 2024-04-25 14:11:13.751171 reka_api-2.0.0/src/reka/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 14:11:13.751171 reka_api-2.0.0/src/reka/api/__init__.py
+-rw-r--r--   0        0        0     7483 2024-04-25 14:11:13.751171 reka_api-2.0.0/src/reka/api/chat.py
+-rw-r--r--   0        0        0     2077 2024-04-25 14:11:13.751171 reka_api-2.0.0/src/reka/api/dataset.py
+-rw-r--r--   0        0        0     2223 2024-04-25 14:11:13.751171 reka_api-2.0.0/src/reka/api/driver.py
+-rw-r--r--   0        0        0      694 2024-04-25 14:11:13.751171 reka_api-2.0.0/src/reka/api/job.py
+-rw-r--r--   0        0        0      373 2024-04-25 14:11:13.751171 reka_api-2.0.0/src/reka/api/models.py
+-rw-r--r--   0        0        0     3563 2024-04-25 14:11:13.751171 reka_api-2.0.0/src/reka/api/retrieval.py
+-rw-r--r--   0        0        0     1136 2024-04-25 14:11:13.751171 reka_api-2.0.0/src/reka/errors.py
+-rw-r--r--   0        0        0        0 2024-04-25 14:11:13.751171 reka_api-2.0.0/src/reka/py.typed
+-rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 reka_api-2.0.0/PKG-INFO
```

### Comparing `reka_api-1.0.6/LICENSE` & `reka_api-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reka_api-1.0.6/pyproject.toml` & `reka_api-2.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reka-api"
-version = "1.0.6"
+version = "2.0.0"
 authors = [
     "Reka Team <contact@reka.ai>",
 ]
 description = "Reka API"
 readme = "README.md"
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `reka_api-1.0.6/src/reka/__init__.py` & `reka_api-2.0.0/src/reka/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,26 +6,24 @@
 # Grab it from an environment variable by default, but can be overriden
 API_KEY = os.getenv("REKA_API_KEY")
 # Default production server
 _SERVER = os.getenv("REKA_SERVER", "https://api.reka.ai")
 
 __version__ = importlib.metadata.version("reka-api")
 from reka.api.chat import chat
-from reka.api.completion import completion
 from reka.api.dataset import add_dataset, delete_dataset, list_datasets
 from reka.api.models import list_models
 from reka.api.retrieval import (
     PrepareRetrievalStatusResponse,
     prepare_retrieval,
     retrieval_job_status,
 )
 
 __all__ = [
     "chat",
-    "completion",
     "delete_dataset",
     "add_dataset",
     "list_models",
     "list_datasets",
     "PrepareRetrievalStatusResponse",
     "prepare_retrieval",
     "retrieval_job_status",
```

### Comparing `reka_api-1.0.6/src/reka/api/chat.py` & `reka_api-2.0.0/src/reka/api/chat.py`

 * *Files identical despite different names*

### Comparing `reka_api-1.0.6/src/reka/api/dataset.py` & `reka_api-2.0.0/src/reka/api/dataset.py`

 * *Files identical despite different names*

### Comparing `reka_api-1.0.6/src/reka/api/driver.py` & `reka_api-2.0.0/src/reka/api/driver.py`

 * *Files identical despite different names*

### Comparing `reka_api-1.0.6/src/reka/api/job.py` & `reka_api-2.0.0/src/reka/api/job.py`

 * *Files identical despite different names*

### Comparing `reka_api-1.0.6/src/reka/api/retrieval.py` & `reka_api-2.0.0/src/reka/api/retrieval.py`

 * *Files identical despite different names*

### Comparing `reka_api-1.0.6/src/reka/errors.py` & `reka_api-2.0.0/src/reka/errors.py`

 * *Files identical despite different names*

### Comparing `reka_api-1.0.6/PKG-INFO` & `reka_api-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reka-api
-Version: 1.0.6
+Version: 2.0.0
 Summary: Reka API
 Home-page: https://reka.ai/
 Author: Reka Team
 Author-email: contact@reka.ai
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

