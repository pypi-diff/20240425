# Comparing `tmp/spikeinterface_pipelines-0.0.8.tar.gz` & `tmp/spikeinterface_pipelines-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spikeinterface_pipelines-0.0.8.tar", last modified: Tue Feb  6 16:24:59 2024, max compression
+gzip compressed data, was "spikeinterface_pipelines-0.0.9.tar", last modified: Tue Feb  6 17:30:03 2024, max compression
```

## Comparing `spikeinterface_pipelines-0.0.8.tar` & `spikeinterface_pipelines-0.0.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:24:59.674221 spikeinterface_pipelines-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-06 16:24:46.000000 spikeinterface_pipelines-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-02-06 16:24:59.674221 spikeinterface_pipelines-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-02-06 16:24:46.000000 spikeinterface_pipelines-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-02-06 16:24:46.000000 spikeinterface_pipelines-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 16:24:59.674221 spikeinterface_pipelines-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:24:59.666221 spikeinterface_pipelines-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:24:59.666221 spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-06 16:24:46.000000 spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:24:59.670221 spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines/curation/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-06 16:24:46.000000 spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines/curation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-02-06 16:24:46.000000 spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines/curation/curation.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-02-06 16:24:46.000000 spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines/curation/params.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-02-06 16:24:46.000000 spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines/global_params.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-06 16:24:46.000000 spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-02-06 16:24:46.000000 spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:24:59.670221 spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines/postprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-06 16:24:46.000000 spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines/postprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9065 2024-02-06 16:24:46.000000 spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines/postprocessing/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-02-06 16:24:46.000000 spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines/postprocessing/postprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:24:59.670221 spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-06 16:24:46.000000 spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11225 2024-02-06 16:24:46.000000 spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines/preprocessing/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     5769 2024-02-06 16:24:46.000000 spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines/preprocessing/preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:24:59.670221 spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines/spikesorting/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-06 16:24:46.000000 spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines/spikesorting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-02-06 16:24:46.000000 spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines/spikesorting/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-02-06 16:24:46.000000 spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines/spikesorting/spikesorting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:24:59.670221 spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-06 16:24:46.000000 spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-02-06 16:24:46.000000 spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines/visualization/params.py
--rw-r--r--   0 runner    (1001) docker     (127)    10030 2024-02-06 16:24:46.000000 spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines/visualization/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:24:59.674221 spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-02-06 16:24:59.000000 spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-02-06 16:24:59.000000 spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 16:24:59.000000 spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-06 16:24:59.000000 spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-06 16:24:59.000000 spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:24:59.670221 spikeinterface_pipelines-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7486 2024-02-06 16:24:46.000000 spikeinterface_pipelines-0.0.8/tests/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 17:30:03.494244 spikeinterface_pipelines-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-06 17:29:50.000000 spikeinterface_pipelines-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-02-06 17:30:03.494244 spikeinterface_pipelines-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-02-06 17:29:50.000000 spikeinterface_pipelines-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-02-06 17:29:50.000000 spikeinterface_pipelines-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 17:30:03.494244 spikeinterface_pipelines-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 17:30:03.486244 spikeinterface_pipelines-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 17:30:03.490244 spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-06 17:29:50.000000 spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 17:30:03.490244 spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines/curation/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-06 17:29:50.000000 spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines/curation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-02-06 17:29:50.000000 spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines/curation/curation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-02-06 17:29:50.000000 spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines/curation/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-02-06 17:29:50.000000 spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines/global_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-06 17:29:50.000000 spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-02-06 17:29:50.000000 spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 17:30:03.494244 spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines/postprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-06 17:29:50.000000 spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines/postprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9065 2024-02-06 17:29:50.000000 spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines/postprocessing/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-02-06 17:29:50.000000 spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines/postprocessing/postprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 17:30:03.494244 spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-06 17:29:50.000000 spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11225 2024-02-06 17:29:50.000000 spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines/preprocessing/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5769 2024-02-06 17:29:50.000000 spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines/preprocessing/preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 17:30:03.494244 spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines/spikesorting/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-06 17:29:50.000000 spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines/spikesorting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-02-06 17:29:50.000000 spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines/spikesorting/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-02-06 17:29:50.000000 spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines/spikesorting/spikesorting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 17:30:03.494244 spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-06 17:29:50.000000 spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-02-06 17:29:50.000000 spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines/visualization/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10030 2024-02-06 17:29:50.000000 spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines/visualization/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 17:30:03.494244 spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-02-06 17:30:03.000000 spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-02-06 17:30:03.000000 spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 17:30:03.000000 spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-06 17:30:03.000000 spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-06 17:30:03.000000 spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 17:30:03.494244 spikeinterface_pipelines-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7486 2024-02-06 17:29:50.000000 spikeinterface_pipelines-0.0.9/tests/test_pipeline.py
```

### Comparing `spikeinterface_pipelines-0.0.8/LICENSE` & `spikeinterface_pipelines-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spikeinterface_pipelines-0.0.8/PKG-INFO` & `spikeinterface_pipelines-0.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: spikeinterface_pipelines
-Version: 0.0.8
+Version: 0.0.9
 Summary: Collection of standardized analysis pipelines based on SpikeInterfacee.
 Author-email: Alessio Buccino <alessiop.buccino@gmail.com>, Jeremy Magland <jmagland@flatironinstitute.org>, Luiz Tauffer <luiz.tauffer@catalystneuro.com>
 Project-URL: homepage, https://github.com/SpikeInterface/spikeinterface_pipelines
 Project-URL: documentation, https://github.com/SpikeInterface/spikeinterface_pipelines
 Project-URL: repository, https://github.com/SpikeInterface/spikeinterface_pipelines
 Keywords: spikeinterface,spike sorting,electrophysiology,neuroscience
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: spikeinterface[full,widgets]>=0.100.0
 Requires-Dist: neo>=0.12.0
 Requires-Dist: pydantic>=2.4.2
+Requires-Dist: sortingview>=0.13.1
+Requires-Dist: kachery_cloud>=0.4.7
 
 [![PyPI version](https://badge.fury.io/py/spikeinterface-pipelines.svg)](https://badge.fury.io/py/spikeinterface-pipelines)
 
 # spikeinterface_pipelines
 Collection of standardized analysis pipelines based on SpikeInterface
```

### Comparing `spikeinterface_pipelines-0.0.8/pyproject.toml` & `spikeinterface_pipelines-0.0.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [project]
 name = "spikeinterface_pipelines"
-version = "0.0.8"
+version = "0.0.9"
 description = "Collection of standardized analysis pipelines based on SpikeInterfacee."
 readme = "README.md"
 authors = [
     { name = "Alessio Buccino", email = "alessiop.buccino@gmail.com" },
     { name = "Jeremy Magland", email = "jmagland@flatironinstitute.org" },
     { name = "Luiz Tauffer", email = "luiz.tauffer@catalystneuro.com" },
 ]
 requires-python = ">=3.8"
 dependencies = [
     "spikeinterface[full,widgets]>=0.100.0",
     "neo>=0.12.0",
     "pydantic>=2.4.2",
+    "sortingview>=0.13.1",
+    "kachery_cloud>=0.4.7",
 ]
 keywords = [
     "spikeinterface",
     "spike sorting",
     "electrophysiology",
     "neuroscience",
 ]
```

### Comparing `spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines/curation/curation.py` & `spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines/curation/curation.py`

 * *Files identical despite different names*

### Comparing `spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines/pipeline.py` & `spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines/postprocessing/params.py` & `spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines/postprocessing/params.py`

 * *Files identical despite different names*

### Comparing `spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines/postprocessing/postprocessing.py` & `spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines/postprocessing/postprocessing.py`

 * *Files identical despite different names*

### Comparing `spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines/preprocessing/params.py` & `spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines/preprocessing/params.py`

 * *Files identical despite different names*

### Comparing `spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines/preprocessing/preprocessing.py` & `spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines/preprocessing/preprocessing.py`

 * *Files identical despite different names*

### Comparing `spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines/spikesorting/params.py` & `spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines/spikesorting/params.py`

 * *Files identical despite different names*

### Comparing `spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines/spikesorting/spikesorting.py` & `spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines/spikesorting/spikesorting.py`

 * *Files identical despite different names*

### Comparing `spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines/visualization/params.py` & `spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines/visualization/params.py`

 * *Files identical despite different names*

### Comparing `spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines/visualization/visualization.py` & `spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines/visualization/visualization.py`

 * *Files identical despite different names*

### Comparing `spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines.egg-info/PKG-INFO` & `spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: spikeinterface_pipelines
-Version: 0.0.8
+Version: 0.0.9
 Summary: Collection of standardized analysis pipelines based on SpikeInterfacee.
 Author-email: Alessio Buccino <alessiop.buccino@gmail.com>, Jeremy Magland <jmagland@flatironinstitute.org>, Luiz Tauffer <luiz.tauffer@catalystneuro.com>
 Project-URL: homepage, https://github.com/SpikeInterface/spikeinterface_pipelines
 Project-URL: documentation, https://github.com/SpikeInterface/spikeinterface_pipelines
 Project-URL: repository, https://github.com/SpikeInterface/spikeinterface_pipelines
 Keywords: spikeinterface,spike sorting,electrophysiology,neuroscience
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: spikeinterface[full,widgets]>=0.100.0
 Requires-Dist: neo>=0.12.0
 Requires-Dist: pydantic>=2.4.2
+Requires-Dist: sortingview>=0.13.1
+Requires-Dist: kachery_cloud>=0.4.7
 
 [![PyPI version](https://badge.fury.io/py/spikeinterface-pipelines.svg)](https://badge.fury.io/py/spikeinterface-pipelines)
 
 # spikeinterface_pipelines
 Collection of standardized analysis pipelines based on SpikeInterface
```

### Comparing `spikeinterface_pipelines-0.0.8/src/spikeinterface_pipelines.egg-info/SOURCES.txt` & `spikeinterface_pipelines-0.0.9/src/spikeinterface_pipelines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spikeinterface_pipelines-0.0.8/tests/test_pipeline.py` & `spikeinterface_pipelines-0.0.9/tests/test_pipeline.py`

 * *Files identical despite different names*

