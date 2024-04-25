# Comparing `tmp/finalsa-common-models-0.0.4.tar.gz` & `tmp/finalsa_common_models-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finalsa-common-models-0.0.4.tar", last modified: Wed Mar 27 02:05:53 2024, max compression
+gzip compressed data, was "finalsa_common_models-0.1.0.tar", last modified: Thu Apr 25 14:30:22 2024, max compression
```

## Comparing `finalsa-common-models-0.0.4.tar` & `finalsa_common_models-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 02:05:53.759814 finalsa-common-models-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-03-27 02:05:47.000000 finalsa-common-models-0.0.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-03-27 02:05:53.759814 finalsa-common-models-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 02:05:47.000000 finalsa-common-models-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 02:05:53.755814 finalsa-common-models-0.0.4/finalsa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 02:05:53.755814 finalsa-common-models-0.0.4/finalsa/common/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 02:05:53.755814 finalsa-common-models-0.0.4/finalsa/common/models/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-27 02:05:47.000000 finalsa-common-models-0.0.4/finalsa/common/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 02:05:53.755814 finalsa-common-models-0.0.4/finalsa/common/models/models/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-27 02:05:47.000000 finalsa-common-models-0.0.4/finalsa/common/models/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-03-27 02:05:47.000000 finalsa-common-models-0.0.4/finalsa/common/models/models/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-03-27 02:05:47.000000 finalsa-common-models-0.0.4/finalsa/common/models/models/sqs_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-03-27 02:05:47.000000 finalsa-common-models-0.0.4/finalsa/common/models/models/sqs_response.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 02:05:47.000000 finalsa-common-models-0.0.4/finalsa/common/models/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 02:05:53.755814 finalsa-common-models-0.0.4/finalsa_common_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-03-27 02:05:53.000000 finalsa-common-models-0.0.4/finalsa_common_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-27 02:05:53.000000 finalsa-common-models-0.0.4/finalsa_common_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 02:05:53.000000 finalsa-common-models-0.0.4/finalsa_common_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-27 02:05:53.000000 finalsa-common-models-0.0.4/finalsa_common_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-27 02:05:53.000000 finalsa-common-models-0.0.4/finalsa_common_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 02:05:53.000000 finalsa-common-models-0.0.4/finalsa_common_models.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-27 02:05:53.759814 finalsa-common-models-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-03-27 02:05:47.000000 finalsa-common-models-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 02:05:53.755814 finalsa-common-models-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-03-27 02:05:47.000000 finalsa-common-models-0.0.4/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:30:22.239010 finalsa_common_models-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-25 14:30:14.000000 finalsa_common_models-0.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-25 14:30:22.239010 finalsa_common_models-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:30:14.000000 finalsa_common_models-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:30:22.235010 finalsa_common_models-0.1.0/finalsa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:30:22.235010 finalsa_common_models-0.1.0/finalsa/common/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:30:22.239010 finalsa_common_models-0.1.0/finalsa/common/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-25 14:30:14.000000 finalsa_common_models-0.1.0/finalsa/common/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:30:22.239010 finalsa_common_models-0.1.0/finalsa/common/models/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-25 14:30:14.000000 finalsa_common_models-0.1.0/finalsa/common/models/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-25 14:30:14.000000 finalsa_common_models-0.1.0/finalsa/common/models/models/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-25 14:30:14.000000 finalsa_common_models-0.1.0/finalsa/common/models/models/sqs_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-25 14:30:14.000000 finalsa_common_models-0.1.0/finalsa/common/models/models/sqs_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:30:14.000000 finalsa_common_models-0.1.0/finalsa/common/models/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:30:22.239010 finalsa_common_models-0.1.0/finalsa_common_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-25 14:30:22.000000 finalsa_common_models-0.1.0/finalsa_common_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-25 14:30:22.000000 finalsa_common_models-0.1.0/finalsa_common_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 14:30:22.000000 finalsa_common_models-0.1.0/finalsa_common_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-25 14:30:22.000000 finalsa_common_models-0.1.0/finalsa_common_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-25 14:30:22.000000 finalsa_common_models-0.1.0/finalsa_common_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 14:30:22.000000 finalsa_common_models-0.1.0/finalsa_common_models.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-25 14:30:22.239010 finalsa_common_models-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-25 14:30:14.000000 finalsa_common_models-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:30:22.239010 finalsa_common_models-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6190 2024-04-25 14:30:14.000000 finalsa_common_models-0.1.0/tests/test_client.py
```

### Comparing `finalsa-common-models-0.0.4/LICENSE.md` & `finalsa_common_models-0.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `finalsa-common-models-0.0.4/PKG-INFO` & `finalsa_common_models-0.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finalsa-common-models
-Version: 0.0.4
+Version: 0.1.0
 Summary: An utils package for using finalsa common models.
 Home-page: https://github.com/finalsa/finalsa-common-models
 Author: Luis Jimenez
 Author-email: luis@finalsa.com
 License: MIT
 Keywords: dynamodb
 Classifier: Intended Audience :: Developers
@@ -12,12 +12,12 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: boto3>=1.20.3
 Requires-Dist: pydantic>=2.5.2
```

### Comparing `finalsa-common-models-0.0.4/finalsa/common/models/models/functions.py` & `finalsa_common_models-0.1.0/finalsa/common/models/models/functions.py`

 * *Files identical despite different names*

### Comparing `finalsa-common-models-0.0.4/finalsa/common/models/models/sqs_message.py` & `finalsa_common_models-0.1.0/finalsa/common/models/models/sqs_message.py`

 * *Files identical despite different names*

### Comparing `finalsa-common-models-0.0.4/finalsa/common/models/models/sqs_response.py` & `finalsa_common_models-0.1.0/finalsa/common/models/models/sqs_response.py`

 * *Files identical despite different names*

### Comparing `finalsa-common-models-0.0.4/finalsa_common_models.egg-info/PKG-INFO` & `finalsa_common_models-0.1.0/finalsa_common_models.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finalsa-common-models
-Version: 0.0.4
+Version: 0.1.0
 Summary: An utils package for using finalsa common models.
 Home-page: https://github.com/finalsa/finalsa-common-models
 Author: Luis Jimenez
 Author-email: luis@finalsa.com
 License: MIT
 Keywords: dynamodb
 Classifier: Intended Audience :: Developers
@@ -12,12 +12,12 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: boto3>=1.20.3
 Requires-Dist: pydantic>=2.5.2
```

### Comparing `finalsa-common-models-0.0.4/finalsa_common_models.egg-info/SOURCES.txt` & `finalsa_common_models-0.1.0/finalsa_common_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finalsa-common-models-0.0.4/setup.py` & `finalsa_common_models-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     ],
     author="Luis Jimenez",
     author_email="luis@finalsa.com",
     packages=get_packages(PACKAGE_FOLDER),
     package_data={PACKAGE: ["py.typed"]},
     include_package_data=True,
     zip_safe=True,
-    python_requires=">=3.8",
+    python_requires=">=3.10",
     data_files=[("", ["LICENSE.md"])],
     install_requires=[
         "boto3>=1.20.3",
         "pydantic>=2.5.2",
     ],
     extras_require={
```

### Comparing `finalsa-common-models-0.0.4/tests/test_client.py` & `finalsa_common_models-0.1.0/tests/test_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,15 @@
     to_message_attributes, __version__)
 import os
 import sys
 import uuid
 import datetime
 import decimal
 
+from json import dumps
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '../../')))
 
 
 def test_version():
     assert __version__ is not None
 
 
@@ -135,7 +136,42 @@
     assert result['binary']['BinaryValue'] == b'test'
     assert result['uuid']['DataType'] == 'String'
     assert result['uuid']['StringValue'] == str(attributes['uuid'])
     assert result['datetime']['DataType'] == 'String'
     assert result['datetime']['StringValue'] == attributes['datetime'].isoformat()
     assert result['decimal']['DataType'] == 'Number'
     assert result['decimal']['StringValue'] == '1.0'
+
+
+def test_parse_from_sns_response():
+    real_message_body = {
+        "test": "test"
+    }
+    body = dumps({
+        'Type': 'Notification',
+        'TopicArn': 'mytopic',
+        'Message': dumps(real_message_body),
+        'MessageAttributes': {'correlation_id': {
+            'Type': 'String', 'Value': '123e4567-e89b-12d3-a456-426614174000'
+        }}
+    })
+
+    boto_response = {
+        'MessageId': 'test',
+        'ReceiptHandle': 'test',
+        'MD5OfBody': 'test',
+        'Body': body,
+        'Attributes': {'test': 'test', 'correlation_id': '123e4567-e89b-12d3-a456-426614174000'},
+        'MessageAttributes': {'correlation_id': {'Type': 'String', 'Value': '123e4567-e89b-12d3-a456-426614174000'}}
+
+    }
+
+    response = SqsReponse.from_boto_response(boto_response)
+    assert response.body == body
+    assert response.get_correlation_id() == '123e4567-e89b-12d3-a456-426614174000'
+    assert response.topic == ''
+    assert response.message_attributes == {
+        'correlation_id': "123e4567-e89b-12d3-a456-426614174000"}
+    assert response.attributes == {
+        'test': 'test', 'correlation_id': '123e4567-e89b-12d3-a456-426614174000'}
+    assert response.parse_from_sns() == real_message_body
+    assert response.parse() == real_message_body
```

