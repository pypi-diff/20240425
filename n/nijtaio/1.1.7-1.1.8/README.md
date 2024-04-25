# Comparing `tmp/nijtaio-1.1.7.tar.gz` & `tmp/nijtaio-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nijtaio-1.1.7.tar", last modified: Mon Jan 22 14:54:09 2024, max compression
+gzip compressed data, was "nijtaio-1.1.8.tar", last modified: Thu Apr 25 09:29:56 2024, max compression
```

## Comparing `nijtaio-1.1.7.tar` & `nijtaio-1.1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-22 14:54:09.727985 nijtaio-1.1.7/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2235 2024-01-22 14:54:09.727985 nijtaio-1.1.7/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1722 2023-10-27 13:17:30.000000 nijtaio-1.1.7/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-22 14:54:09.727985 nijtaio-1.1.7/nijtaio/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6712 2024-01-22 14:52:20.000000 nijtaio-1.1.7/nijtaio/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2024-01-22 14:52:20.000000 nijtaio-1.1.7/nijtaio/_version.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3388 2024-01-22 14:46:02.000000 nijtaio-1.1.7/nijtaio/cli.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-22 14:54:09.727985 nijtaio-1.1.7/nijtaio.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2235 2024-01-22 14:54:09.000000 nijtaio-1.1.7/nijtaio.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      337 2024-01-22 14:54:09.000000 nijtaio-1.1.7/nijtaio.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-01-22 14:54:09.000000 nijtaio-1.1.7/nijtaio.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       49 2024-01-22 14:54:09.000000 nijtaio-1.1.7/nijtaio.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       41 2024-01-22 14:54:09.000000 nijtaio-1.1.7/nijtaio.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2024-01-22 14:54:09.000000 nijtaio-1.1.7/nijtaio.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      596 2024-01-22 14:53:31.000000 nijtaio-1.1.7/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-01-22 14:54:09.727985 nijtaio-1.1.7/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      471 2023-11-28 13:18:36.000000 nijtaio-1.1.7/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-22 14:54:09.727985 nijtaio-1.1.7/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      891 2023-12-01 13:56:45.000000 nijtaio-1.1.7/tests/test_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      628 2023-11-28 13:18:36.000000 nijtaio-1.1.7/tests/test_nijtaio.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1427 2023-11-08 17:25:26.000000 nijtaio-1.1.7/tests/test_s3.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-25 09:29:56.620210 nijtaio-1.1.8/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2206 2024-04-25 09:29:56.620210 nijtaio-1.1.8/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1722 2023-10-27 13:17:30.000000 nijtaio-1.1.8/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-25 09:29:56.620210 nijtaio-1.1.8/nijtaio/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6873 2024-04-25 08:45:28.000000 nijtaio-1.1.8/nijtaio/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2024-04-11 17:18:02.000000 nijtaio-1.1.8/nijtaio/_version.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3388 2024-01-22 14:46:02.000000 nijtaio-1.1.8/nijtaio/cli.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-25 09:29:56.620210 nijtaio-1.1.8/nijtaio.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2206 2024-04-25 09:29:56.000000 nijtaio-1.1.8/nijtaio.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      337 2024-04-25 09:29:56.000000 nijtaio-1.1.8/nijtaio.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-25 09:29:56.000000 nijtaio-1.1.8/nijtaio.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       49 2024-04-25 09:29:56.000000 nijtaio-1.1.8/nijtaio.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       41 2024-04-25 09:29:56.000000 nijtaio-1.1.8/nijtaio.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2024-04-25 09:29:56.000000 nijtaio-1.1.8/nijtaio.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      567 2024-04-25 08:56:32.000000 nijtaio-1.1.8/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-25 09:29:56.620210 nijtaio-1.1.8/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      471 2023-11-28 13:18:36.000000 nijtaio-1.1.8/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-25 09:29:56.620210 nijtaio-1.1.8/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      891 2023-12-01 13:56:45.000000 nijtaio-1.1.8/tests/test_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      628 2023-11-28 13:18:36.000000 nijtaio-1.1.8/tests/test_nijtaio.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1427 2023-11-08 17:25:26.000000 nijtaio-1.1.8/tests/test_s3.py
```

### Comparing `nijtaio-1.1.7/PKG-INFO` & `nijtaio-1.1.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: nijtaio
-Version: 1.1.7
+Version: 1.1.8
 Summary: Helper module to streamline access to Nijta's API
-Project-URL: Documentation, https://nijta.readme.io/reference/getting-started-1
+Project-URL: Documentation, https://docs.nijta.com
 Project-URL: Bug Tracker, https://github.com/Nijta/nijta-samples/issues
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: soundfile
 Requires-Dist: librosa
```

### Comparing `nijtaio-1.1.7/README.md` & `nijtaio-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `nijtaio-1.1.7/nijtaio/__init__.py` & `nijtaio-1.1.8/nijtaio/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import ast
 import json
 import requests
 import datasets
 import io
 import os
 import soundfile as sf
+import urllib
 
 
 def _nijta_serializer(obj):
     """Serialize audio dataset.
 
     Serialize audio data from a datasets.DatasetDict or datasets.arrow_dataset.Dataset
     into a dictionary of hex-encoded audio data.
@@ -84,15 +85,15 @@
                                             datasets.Audio(decode=True, mono=False))['train']
         try:
             response = requests.post(f"{api_url}/tasks/{session_id}",
                                      json=json.dumps(
                                          dataset,
                                          default=_nijta_serializer),
                                      headers=headers,
-                                     params=params)
+                                     params=urllib.parse.urlencode(params))
             return response
         except requests.exceptions.RequestException as e:
             return f"Error sending request: {e}"
     else:
         return "Invalid input_data format."
 
 
@@ -167,9 +168,11 @@
         result[filename] = {}
         if 'audio' in anon_batch[filename]:
             result[filename]['audio'] = bytes.fromhex(anon_batch[filename]['audio'])
         if 'transcription' in anon_batch[filename]:
             result[filename]['transcription'] = anon_batch[filename]['transcription']
         if 'words' in anon_batch[filename]:
             result[filename]['words'] = anon_batch[filename]['words']
+        if 'sequence' in anon_batch[filename]:
+            result[filename]['sequence'] = anon_batch[filename]['sequence']
 
     return content['data']['task_status'], result
```

### Comparing `nijtaio-1.1.7/nijtaio/cli.py` & `nijtaio-1.1.8/nijtaio/cli.py`

 * *Files identical despite different names*

### Comparing `nijtaio-1.1.7/nijtaio.egg-info/PKG-INFO` & `nijtaio-1.1.8/nijtaio.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: nijtaio
-Version: 1.1.7
+Version: 1.1.8
 Summary: Helper module to streamline access to Nijta's API
-Project-URL: Documentation, https://nijta.readme.io/reference/getting-started-1
+Project-URL: Documentation, https://docs.nijta.com
 Project-URL: Bug Tracker, https://github.com/Nijta/nijta-samples/issues
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: soundfile
 Requires-Dist: librosa
```

### Comparing `nijtaio-1.1.7/pyproject.toml` & `nijtaio-1.1.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nijtaio"
-version = "1.1.7"
+version = "1.1.8"
 description = "Helper module to streamline access to Nijta's API"
 readme = "README.md"
 classifiers = [
     "Intended Audience :: Developers",
     "License :: Other/Proprietary License"
 ]
 dependencies = ['requests', 'soundfile', 'librosa', 'datasets', 'fire']
 
 [project.scripts]
 voiceharbor = "nijtaio.cli:main"
 
 [project.urls]
-"Documentation" = "https://nijta.readme.io/reference/getting-started-1"
+"Documentation" = "https://docs.nijta.com"
 "Bug Tracker" = "https://github.com/Nijta/nijta-samples/issues"
```

### Comparing `nijtaio-1.1.7/tests/test_dataset.py` & `nijtaio-1.1.8/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `nijtaio-1.1.7/tests/test_nijtaio.py` & `nijtaio-1.1.8/tests/test_nijtaio.py`

 * *Files identical despite different names*

### Comparing `nijtaio-1.1.7/tests/test_s3.py` & `nijtaio-1.1.8/tests/test_s3.py`

 * *Files identical despite different names*

