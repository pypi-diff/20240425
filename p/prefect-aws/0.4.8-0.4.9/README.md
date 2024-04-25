# Comparing `tmp/prefect-aws-0.4.8.tar.gz` & `tmp/prefect-aws-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect-aws-0.4.8.tar", last modified: Tue Jan 23 16:15:05 2024, max compression
+gzip compressed data, was "prefect-aws-0.4.9.tar", last modified: Wed Jan 24 18:48:34 2024, max compression
```

## Comparing `prefect-aws-0.4.8.tar` & `prefect-aws-0.4.9.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:15:05.263176 prefect-aws-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-01-23 16:14:08.000000 prefect-aws-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-01-23 16:14:08.000000 prefect-aws-0.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-01-23 16:15:05.263176 prefect-aws-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-01-23 16:14:08.000000 prefect-aws-0.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:15:05.263176 prefect-aws-0.4.8/prefect_aws/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-01-23 16:14:08.000000 prefect-aws-0.4.8/prefect_aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-01-23 16:15:05.263176 prefect-aws-0.4.8/prefect_aws/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-01-23 16:14:08.000000 prefect-aws-0.4.8/prefect_aws/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6335 2024-01-23 16:14:08.000000 prefect-aws-0.4.8/prefect_aws/client_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-01-23 16:14:08.000000 prefect-aws-0.4.8/prefect_aws/client_waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9718 2024-01-23 16:14:08.000000 prefect-aws-0.4.8/prefect_aws/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:15:05.259176 prefect-aws-0.4.8/prefect_aws/deployments/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 16:14:08.000000 prefect-aws-0.4.8/prefect_aws/deployments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8220 2024-01-23 16:14:08.000000 prefect-aws-0.4.8/prefect_aws/deployments/steps.py
--rw-r--r--   0 runner    (1001) docker     (127)    60946 2024-01-23 16:14:08.000000 prefect-aws-0.4.8/prefect_aws/ecs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-01-23 16:14:08.000000 prefect-aws-0.4.8/prefect_aws/lambda_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    46314 2024-01-23 16:14:08.000000 prefect-aws-0.4.8/prefect_aws/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)    17632 2024-01-23 16:14:08.000000 prefect-aws-0.4.8/prefect_aws/secrets_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:15:05.259176 prefect-aws-0.4.8/prefect_aws/workers/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-01-23 16:14:08.000000 prefect-aws-0.4.8/prefect_aws/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    61644 2024-01-23 16:14:08.000000 prefect-aws-0.4.8/prefect_aws/workers/ecs_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:15:05.263176 prefect-aws-0.4.8/prefect_aws.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-01-23 16:15:05.000000 prefect-aws-0.4.8/prefect_aws.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-01-23 16:15:05.000000 prefect-aws-0.4.8/prefect_aws.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 16:15:05.000000 prefect-aws-0.4.8/prefect_aws.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-23 16:15:05.000000 prefect-aws-0.4.8/prefect_aws.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-01-23 16:15:05.000000 prefect-aws-0.4.8/prefect_aws.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-23 16:15:05.000000 prefect-aws-0.4.8/prefect_aws.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-01-23 16:14:08.000000 prefect-aws-0.4.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-01-23 16:14:08.000000 prefect-aws-0.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-01-23 16:15:05.263176 prefect-aws-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-01-23 16:14:08.000000 prefect-aws-0.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:15:05.263176 prefect-aws-0.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-01-23 16:14:08.000000 prefect-aws-0.4.8/tests/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-01-23 16:14:08.000000 prefect-aws-0.4.8/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-01-23 16:14:08.000000 prefect-aws-0.4.8/tests/test_client_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-01-23 16:14:08.000000 prefect-aws-0.4.8/tests/test_client_waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-01-23 16:14:08.000000 prefect-aws-0.4.8/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    74469 2024-01-23 16:14:08.000000 prefect-aws-0.4.8/tests/test_ecs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7090 2024-01-23 16:14:08.000000 prefect-aws-0.4.8/tests/test_lambda_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    35089 2024-01-23 16:14:08.000000 prefect-aws-0.4.8/tests/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7001 2024-01-23 16:14:08.000000 prefect-aws-0.4.8/tests/test_secrets_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    80043 2024-01-23 16:14:08.000000 prefect-aws-0.4.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 18:48:34.378931 prefect-aws-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-01-24 18:47:39.000000 prefect-aws-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-01-24 18:47:39.000000 prefect-aws-0.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-01-24 18:48:34.378931 prefect-aws-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-01-24 18:47:39.000000 prefect-aws-0.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 18:48:34.382931 prefect-aws-0.4.9/prefect_aws/
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-01-24 18:47:39.000000 prefect-aws-0.4.9/prefect_aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-01-24 18:48:34.382931 prefect-aws-0.4.9/prefect_aws/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-01-24 18:47:39.000000 prefect-aws-0.4.9/prefect_aws/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6403 2024-01-24 18:47:39.000000 prefect-aws-0.4.9/prefect_aws/client_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-01-24 18:47:39.000000 prefect-aws-0.4.9/prefect_aws/client_waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9692 2024-01-24 18:47:39.000000 prefect-aws-0.4.9/prefect_aws/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 18:48:34.374931 prefect-aws-0.4.9/prefect_aws/deployments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 18:47:39.000000 prefect-aws-0.4.9/prefect_aws/deployments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8220 2024-01-24 18:47:39.000000 prefect-aws-0.4.9/prefect_aws/deployments/steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60946 2024-01-24 18:47:39.000000 prefect-aws-0.4.9/prefect_aws/ecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-01-24 18:47:39.000000 prefect-aws-0.4.9/prefect_aws/lambda_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46314 2024-01-24 18:47:39.000000 prefect-aws-0.4.9/prefect_aws/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17632 2024-01-24 18:47:39.000000 prefect-aws-0.4.9/prefect_aws/secrets_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-01-24 18:47:39.000000 prefect-aws-0.4.9/prefect_aws/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 18:48:34.374931 prefect-aws-0.4.9/prefect_aws/workers/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-01-24 18:47:39.000000 prefect-aws-0.4.9/prefect_aws/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61644 2024-01-24 18:47:39.000000 prefect-aws-0.4.9/prefect_aws/workers/ecs_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 18:48:34.378931 prefect-aws-0.4.9/prefect_aws.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-01-24 18:48:34.000000 prefect-aws-0.4.9/prefect_aws.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-01-24 18:48:34.000000 prefect-aws-0.4.9/prefect_aws.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-24 18:48:34.000000 prefect-aws-0.4.9/prefect_aws.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-24 18:48:34.000000 prefect-aws-0.4.9/prefect_aws.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-01-24 18:48:34.000000 prefect-aws-0.4.9/prefect_aws.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-24 18:48:34.000000 prefect-aws-0.4.9/prefect_aws.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-01-24 18:47:39.000000 prefect-aws-0.4.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-01-24 18:47:39.000000 prefect-aws-0.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-01-24 18:48:34.378931 prefect-aws-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-01-24 18:47:39.000000 prefect-aws-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 18:48:34.378931 prefect-aws-0.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-01-24 18:47:39.000000 prefect-aws-0.4.9/tests/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-01-24 18:47:39.000000 prefect-aws-0.4.9/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-01-24 18:47:39.000000 prefect-aws-0.4.9/tests/test_client_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-01-24 18:47:39.000000 prefect-aws-0.4.9/tests/test_client_waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-01-24 18:47:39.000000 prefect-aws-0.4.9/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74469 2024-01-24 18:47:39.000000 prefect-aws-0.4.9/tests/test_ecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7090 2024-01-24 18:47:39.000000 prefect-aws-0.4.9/tests/test_lambda_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35089 2024-01-24 18:47:39.000000 prefect-aws-0.4.9/tests/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7001 2024-01-24 18:47:39.000000 prefect-aws-0.4.9/tests/test_secrets_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-01-24 18:47:39.000000 prefect-aws-0.4.9/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80043 2024-01-24 18:47:39.000000 prefect-aws-0.4.9/versioneer.py
```

### Comparing `prefect-aws-0.4.8/LICENSE` & `prefect-aws-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.4.8/PKG-INFO` & `prefect-aws-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-aws
-Version: 0.4.8
+Version: 0.4.9
 Summary: Prefect collection of tasks and subflows to integrate with AWS
 Home-page: https://github.com/PrefectHQ/prefect-aws
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prefect-aws Version: 0.4.8 Summary: Prefect
+Metadata-Version: 2.1 Name: prefect-aws Version: 0.4.9 Summary: Prefect
 collection of tasks and subflows to integrate with AWS Home-page: https://
 github.com/PrefectHQ/prefect-aws Author: Prefect Technologies, Inc. Author-
 email: help@prefect.io License: Apache License 2.0 Keywords: prefect
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: System Administrators Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
```

### Comparing `prefect-aws-0.4.8/README.md` & `prefect-aws-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.4.8/prefect_aws/__init__.py` & `prefect-aws-0.4.9/prefect_aws/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.4.8/prefect_aws/batch.py` & `prefect-aws-0.4.9/prefect_aws/batch.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.4.8/prefect_aws/client_parameters.py` & `prefect-aws-0.4.9/prefect_aws/client_parameters.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import warnings
 from typing import Any, Dict, Optional, Union
 
 from botocore import UNSIGNED
 from botocore.client import Config
 from pydantic import VERSION as PYDANTIC_VERSION
 
+from prefect_aws.utilities import hash_collection
+
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import BaseModel, Field, FilePath, root_validator, validator
 else:
     from pydantic import BaseModel, Field, FilePath, root_validator, validator
 
 
 class AwsClientParameters(BaseModel):
@@ -74,15 +76,15 @@
         return hash(
             (
                 self.api_version,
                 self.use_ssl,
                 self.verify,
                 self.verify_cert_path,
                 self.endpoint_url,
-                self.config,
+                hash_collection(self.config),
             )
         )
 
     @validator("config", pre=True)
     def instantiate_config(cls, value: Union[Config, Dict[str, Any]]) -> Dict[str, Any]:
         """
         Casts lists to Config instances.
```

### Comparing `prefect-aws-0.4.8/prefect_aws/client_waiter.py` & `prefect-aws-0.4.9/prefect_aws/client_waiter.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.4.8/prefect_aws/credentials.py` & `prefect-aws-0.4.9/prefect_aws/credentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,15 @@
     def __hash__(self):
         field_hashes = (
             hash(self.aws_access_key_id),
             hash(self.aws_secret_access_key),
             hash(self.aws_session_token),
             hash(self.profile_name),
             hash(self.region_name),
-            hash(frozenset(self.aws_client_parameters.dict().items())),
+            hash(self.aws_client_parameters),
         )
         return hash(field_hashes)
 
     def get_boto3_session(self) -> boto3.Session:
         """
         Returns an authenticated boto3 session that can be used to create clients
         for AWS services
```

### Comparing `prefect-aws-0.4.8/prefect_aws/deployments/steps.py` & `prefect-aws-0.4.9/prefect_aws/deployments/steps.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.4.8/prefect_aws/ecs.py` & `prefect-aws-0.4.9/prefect_aws/ecs.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.4.8/prefect_aws/lambda_function.py` & `prefect-aws-0.4.9/prefect_aws/lambda_function.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.4.8/prefect_aws/s3.py` & `prefect-aws-0.4.9/prefect_aws/s3.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.4.8/prefect_aws/secrets_manager.py` & `prefect-aws-0.4.9/prefect_aws/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.4.8/prefect_aws/workers/ecs_worker.py` & `prefect-aws-0.4.9/prefect_aws/workers/ecs_worker.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.4.8/prefect_aws.egg-info/PKG-INFO` & `prefect-aws-0.4.9/prefect_aws.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-aws
-Version: 0.4.8
+Version: 0.4.9
 Summary: Prefect collection of tasks and subflows to integrate with AWS
 Home-page: https://github.com/PrefectHQ/prefect-aws
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prefect-aws Version: 0.4.8 Summary: Prefect
+Metadata-Version: 2.1 Name: prefect-aws Version: 0.4.9 Summary: Prefect
 collection of tasks and subflows to integrate with AWS Home-page: https://
 github.com/PrefectHQ/prefect-aws Author: Prefect Technologies, Inc. Author-
 email: help@prefect.io License: Apache License 2.0 Keywords: prefect
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: System Administrators Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
```

### Comparing `prefect-aws-0.4.8/prefect_aws.egg-info/SOURCES.txt` & `prefect-aws-0.4.9/prefect_aws.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 prefect_aws/client_parameters.py
 prefect_aws/client_waiter.py
 prefect_aws/credentials.py
 prefect_aws/ecs.py
 prefect_aws/lambda_function.py
 prefect_aws/s3.py
 prefect_aws/secrets_manager.py
+prefect_aws/utilities.py
 prefect_aws.egg-info/PKG-INFO
 prefect_aws.egg-info/SOURCES.txt
 prefect_aws.egg-info/dependency_links.txt
 prefect_aws.egg-info/entry_points.txt
 prefect_aws.egg-info/requires.txt
 prefect_aws.egg-info/top_level.txt
 prefect_aws/deployments/__init__.py
@@ -30,8 +31,9 @@
 tests/test_block_standards.py
 tests/test_client_parameters.py
 tests/test_client_waiter.py
 tests/test_credentials.py
 tests/test_ecs.py
 tests/test_lambda_function.py
 tests/test_s3.py
-tests/test_secrets_manager.py
+tests/test_secrets_manager.py
+tests/test_utilities.py
```

### Comparing `prefect-aws-0.4.8/setup.cfg` & `prefect-aws-0.4.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.4.8/setup.py` & `prefect-aws-0.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.4.8/tests/test_batch.py` & `prefect-aws-0.4.9/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.4.8/tests/test_block_standards.py` & `prefect-aws-0.4.9/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.4.8/tests/test_client_parameters.py` & `prefect-aws-0.4.9/tests/test_client_parameters.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.4.8/tests/test_client_waiter.py` & `prefect-aws-0.4.9/tests/test_client_waiter.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.4.8/tests/test_credentials.py` & `prefect-aws-0.4.9/tests/test_credentials.py`

 * *Files 8% similar despite different names*

```diff
@@ -160,7 +160,32 @@
     credentials = credentials_type(**initial_field)
     initial_hash = hash(credentials)
 
     setattr(credentials, list(new_field.keys())[0], list(new_field.values())[0])
     new_hash = hash(credentials)
 
     assert initial_hash != new_hash, "Hash should change when region_name changes"
+
+
+def test_aws_credentials_nested_client_parameters_are_hashable():
+    """
+    Test to ensure that nested client parameters are hashable.
+    """
+
+    creds = AwsCredentials(
+        region_name="us-east-1",
+        aws_client_parameters=dict(
+            config=dict(
+                connect_timeout=5,
+                read_timeout=5,
+                retries=dict(max_attempts=10, mode="standard"),
+            )
+        ),
+    )
+
+    assert hash(creds) is not None
+
+    client = creds.get_client("s3")
+
+    _client = creds.get_client("s3")
+
+    assert client is _client
```

### Comparing `prefect-aws-0.4.8/tests/test_ecs.py` & `prefect-aws-0.4.9/tests/test_ecs.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.4.8/tests/test_lambda_function.py` & `prefect-aws-0.4.9/tests/test_lambda_function.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.4.8/tests/test_s3.py` & `prefect-aws-0.4.9/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.4.8/tests/test_secrets_manager.py` & `prefect-aws-0.4.9/tests/test_secrets_manager.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.4.8/versioneer.py` & `prefect-aws-0.4.9/versioneer.py`

 * *Files identical despite different names*

