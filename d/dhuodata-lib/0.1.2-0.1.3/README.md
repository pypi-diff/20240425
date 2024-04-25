# Comparing `tmp/dhuodata_lib-0.1.2.tar.gz` & `tmp/dhuodata-lib-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhuodata_lib-0.1.2.tar", last modified: Wed Apr 24 22:35:47 2024, max compression
+gzip compressed data, was "dhuodata-lib-0.1.3.tar", last modified: Thu Apr 25 13:18:11 2024, max compression
```

## Comparing `dhuodata_lib-0.1.2.tar` & `dhuodata-lib-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-24 22:35:47.436676 dhuodata_lib-0.1.2/
--rw-r--r--   0 diego     (1000) diego     (1000)     2983 2024-04-24 22:35:47.436676 dhuodata_lib-0.1.2/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)     2346 2024-04-16 18:35:41.000000 dhuodata_lib-0.1.2/README.md
--rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-04-24 22:35:47.436676 dhuodata_lib-0.1.2/setup.cfg
--rw-rw-r--   0 diego     (1000) diego     (1000)      863 2024-04-24 22:35:42.000000 dhuodata_lib-0.1.2/setup.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-24 22:35:47.432676 dhuodata_lib-0.1.2/src/
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-24 22:35:47.436676 dhuodata_lib-0.1.2/src/dhuodata_lib.egg-info/
--rw-r--r--   0 diego     (1000) diego     (1000)     2983 2024-04-24 22:35:47.000000 dhuodata_lib-0.1.2/src/dhuodata_lib.egg-info/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)      489 2024-04-24 22:35:47.000000 dhuodata_lib-0.1.2/src/dhuodata_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-04-24 22:35:47.000000 dhuodata_lib-0.1.2/src/dhuodata_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)      128 2024-04-24 22:35:47.000000 dhuodata_lib-0.1.2/src/dhuodata_lib.egg-info/requires.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        8 2024-04-24 22:35:47.000000 dhuodata_lib-0.1.2/src/dhuodata_lib.egg-info/top_level.txt
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-24 22:35:47.436676 dhuodata_lib-0.1.2/src/dhuolib/
--rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:35:41.000000 dhuodata_lib-0.1.2/src/dhuolib/__init__.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      261 2024-04-23 16:50:53.000000 dhuodata_lib-0.1.2/src/dhuolib/auth.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     3863 2024-04-24 19:16:19.000000 dhuodata_lib-0.1.2/src/dhuolib/clients.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      358 2024-04-23 16:51:37.000000 dhuodata_lib-0.1.2/src/dhuolib/config.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-24 22:35:47.436676 dhuodata_lib-0.1.2/src/dhuolib/oci_tools/
--rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:52:32.000000 dhuodata_lib-0.1.2/src/dhuolib/oci_tools/__init__.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      716 2024-04-24 18:22:15.000000 dhuodata_lib-0.1.2/src/dhuolib/oci_tools/utils.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      758 2024-04-24 18:22:52.000000 dhuodata_lib-0.1.2/src/dhuolib/predict.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     1087 2024-04-23 16:51:03.000000 dhuodata_lib-0.1.2/src/dhuolib/services.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      711 2024-04-24 18:14:19.000000 dhuodata_lib-0.1.2/src/dhuolib/validations.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      141 2024-04-23 16:51:15.000000 dhuodata_lib-0.1.2/src/dhuolib/worker.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-24 22:35:47.436676 dhuodata_lib-0.1.2/tests/
--rw-rw-r--   0 diego     (1000) diego     (1000)     3466 2024-04-24 20:10:56.000000 dhuodata_lib-0.1.2/tests/test_dhuolib.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-25 13:18:11.065555 dhuodata-lib-0.1.3/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2528 2024-04-25 13:18:11.065555 dhuodata-lib-0.1.3/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2346 2024-04-16 18:35:41.000000 dhuodata-lib-0.1.3/README.md
+-rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-04-25 13:18:11.065555 dhuodata-lib-0.1.3/setup.cfg
+-rw-rw-r--   0 diego     (1000) diego     (1000)      863 2024-04-25 13:16:05.000000 dhuodata-lib-0.1.3/setup.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-25 13:18:11.065555 dhuodata-lib-0.1.3/src/
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-25 13:18:11.065555 dhuodata-lib-0.1.3/src/dhuodata_lib.egg-info/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2528 2024-04-25 13:18:10.000000 dhuodata-lib-0.1.3/src/dhuodata_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)      489 2024-04-25 13:18:11.000000 dhuodata-lib-0.1.3/src/dhuodata_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-04-25 13:18:10.000000 dhuodata-lib-0.1.3/src/dhuodata_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)      128 2024-04-25 13:18:10.000000 dhuodata-lib-0.1.3/src/dhuodata_lib.egg-info/requires.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        8 2024-04-25 13:18:10.000000 dhuodata-lib-0.1.3/src/dhuodata_lib.egg-info/top_level.txt
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-25 13:18:11.065555 dhuodata-lib-0.1.3/src/dhuolib/
+-rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:35:41.000000 dhuodata-lib-0.1.3/src/dhuolib/__init__.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      261 2024-04-23 16:50:53.000000 dhuodata-lib-0.1.3/src/dhuolib/auth.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     3847 2024-04-24 22:37:49.000000 dhuodata-lib-0.1.3/src/dhuolib/clients.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      358 2024-04-23 16:51:37.000000 dhuodata-lib-0.1.3/src/dhuolib/config.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-25 13:18:11.065555 dhuodata-lib-0.1.3/src/dhuolib/oci_tools/
+-rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:52:32.000000 dhuodata-lib-0.1.3/src/dhuolib/oci_tools/__init__.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      716 2024-04-24 18:22:15.000000 dhuodata-lib-0.1.3/src/dhuolib/oci_tools/utils.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      758 2024-04-24 18:22:52.000000 dhuodata-lib-0.1.3/src/dhuolib/predict.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1087 2024-04-23 16:51:03.000000 dhuodata-lib-0.1.3/src/dhuolib/services.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      711 2024-04-24 18:14:19.000000 dhuodata-lib-0.1.3/src/dhuolib/validations.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      141 2024-04-23 16:51:15.000000 dhuodata-lib-0.1.3/src/dhuolib/worker.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-25 13:18:11.065555 dhuodata-lib-0.1.3/tests/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     3491 2024-04-25 13:16:44.000000 dhuodata-lib-0.1.3/tests/test_dhuolib.py
```

### Comparing `dhuodata_lib-0.1.2/PKG-INFO` & `dhuodata-lib-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,16 @@
 Metadata-Version: 2.1
 Name: dhuodata-lib
-Version: 0.1.2
+Version: 0.1.3
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
-Requires-Dist: mlflow
-Requires-Dist: oci==2.125.3
 Provides-Extra: interactive
-Requires-Dist: mypy==1.5.1; extra == "interactive"
-Requires-Dist: flake8==6.1.0; extra == "interactive"
-Requires-Dist: black==22.3.0; extra == "interactive"
-Requires-Dist: pytest-cov~=4.0; extra == "interactive"
-Requires-Dist: pytest~=7.0; extra == "interactive"
-Requires-Dist: twine; extra == "interactive"
-Requires-Dist: wheel; extra == "interactive"
-Requires-Dist: oci==2.125.3; extra == "interactive"
 
 # DHuO LIb
 
 ## Board
 
 ![](assets/imgs/board.png)
```

### Comparing `dhuodata_lib-0.1.2/README.md` & `dhuodata-lib-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `dhuodata_lib-0.1.2/setup.py` & `dhuodata-lib-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 README = ""
 if os.path.exists("README.md"):
     README = open("README.md").read()
 
 setup(
     name="dhuodata-lib",
-    version="0.1.2",
+    version="0.1.3",
     long_description=README,
     long_description_content_type="text/markdown",
     author="DHuO Data Team",
     author_email="diego.salles@engdb.com.br",
     url="https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib",
     install_requires=REQUIRED_PACKAGES,
     extras_require={"interactive": DEV_PACKAGES},
```

### Comparing `dhuodata_lib-0.1.2/src/dhuodata_lib.egg-info/PKG-INFO` & `dhuodata-lib-0.1.3/src/dhuodata_lib.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,16 @@
 Metadata-Version: 2.1
 Name: dhuodata-lib
-Version: 0.1.2
+Version: 0.1.3
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
-Requires-Dist: mlflow
-Requires-Dist: oci==2.125.3
 Provides-Extra: interactive
-Requires-Dist: mypy==1.5.1; extra == "interactive"
-Requires-Dist: flake8==6.1.0; extra == "interactive"
-Requires-Dist: black==22.3.0; extra == "interactive"
-Requires-Dist: pytest-cov~=4.0; extra == "interactive"
-Requires-Dist: pytest~=7.0; extra == "interactive"
-Requires-Dist: twine; extra == "interactive"
-Requires-Dist: wheel; extra == "interactive"
-Requires-Dist: oci==2.125.3; extra == "interactive"
 
 # DHuO LIb
 
 ## Board
 
 ![](assets/imgs/board.png)
```

### Comparing `dhuodata_lib-0.1.2/src/dhuolib/clients.py` & `dhuodata-lib-0.1.3/src/dhuolib/clients.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pydantic import ValidationError
 
-from src.dhuolib.config import logger
-from src.dhuolib.oci_tools.utils import OCIUtils
-from src.dhuolib.services import ServiceAPIML
-from src.dhuolib.validations import ExperimentBody, RunExperimentBody
+from dhuolib.config import logger
+from dhuolib.oci_tools.utils import OCIUtils
+from dhuolib.services import ServiceAPIML
+from dhuolib.validations import ExperimentBody, RunExperimentBody
 
 
 class DhuolibClient:
     def __init__(self, service_endpoint=None, config_file_path='~/.oci/config'):
         if not service_endpoint:
             raise ValueError("service_endpoint is required")
```

### Comparing `dhuodata_lib-0.1.2/src/dhuolib/oci_tools/utils.py` & `dhuodata-lib-0.1.3/src/dhuolib/oci_tools/utils.py`

 * *Files identical despite different names*

### Comparing `dhuodata_lib-0.1.2/src/dhuolib/predict.py` & `dhuodata-lib-0.1.3/src/dhuolib/predict.py`

 * *Files identical despite different names*

### Comparing `dhuodata_lib-0.1.2/src/dhuolib/services.py` & `dhuodata-lib-0.1.3/src/dhuolib/services.py`

 * *Files identical despite different names*

### Comparing `dhuodata_lib-0.1.2/src/dhuolib/validations.py` & `dhuodata-lib-0.1.3/src/dhuolib/validations.py`

 * *Files identical despite different names*

### Comparing `dhuodata_lib-0.1.2/tests/test_dhuolib.py` & `dhuodata-lib-0.1.3/tests/test_dhuolib.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import json
 import unittest
 from unittest.mock import MagicMock, patch
-
+import sys
 import pytest
 from pydantic import ValidationError
 
-from src.dhuolib.clients import DhuolibClient
+sys.path.append("src")
+from dhuolib.clients import DhuolibClient
 
 
 class TestDhuolibUtils(unittest.TestCase):
     def setUp(self):
         self.end_point = "http://fake-endpoint"
         self.dhuolib = DhuolibClient(service_endpoint=self.end_point)
         self.namespace = "engdb"
@@ -25,15 +26,15 @@
             },
         }
 
         with pytest.raises(ValidationError):
             self.dhuolib.create_experiment(experiments_params)
 
     @patch("requests.post")
-    @patch('src.dhuolib.clients.OCIUtils')
+    @patch('dhuolib.clients.OCIUtils')
     def test_deve_criar_o_experimento_com_run_params_corretos(self, mock_oci_utils, mock_post):
         client = DhuolibClient(service_endpoint="http://fake-endpoint")
 
         mock_response = mock_post.return_value
         mock_response.status_code = 201
         mock_response.json.return_value = {"experiment_id": "1"}
```

