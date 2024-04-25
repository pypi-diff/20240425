# Comparing `tmp/finalsa_common_lambdas-0.1.1.tar.gz` & `tmp/finalsa_common_lambdas-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finalsa_common_lambdas-0.1.1.tar", last modified: Tue Apr 23 04:02:42 2024, max compression
+gzip compressed data, was "finalsa_common_lambdas-0.2.0.tar", last modified: Thu Apr 25 14:37:57 2024, max compression
```

## Comparing `finalsa_common_lambdas-0.1.1.tar` & `finalsa_common_lambdas-0.2.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:02:42.509569 finalsa_common_lambdas-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-23 04:02:33.000000 finalsa_common_lambdas-0.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-23 04:02:42.509569 finalsa_common_lambdas-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 04:02:33.000000 finalsa_common_lambdas-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:02:42.501569 finalsa_common_lambdas-0.1.1/finalsa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:02:42.501569 finalsa_common_lambdas-0.1.1/finalsa/common/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:02:42.505569 finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-23 04:02:33.000000 finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:02:42.505569 finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/app/
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-23 04:02:33.000000 finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/app/App.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-23 04:02:33.000000 finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/app/AppEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-23 04:02:33.000000 finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:02:42.505569 finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/http/
--rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-04-23 04:02:33.000000 finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/http/HttpHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-23 04:02:33.000000 finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/http/HttpHeaders.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-23 04:02:33.000000 finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 04:02:33.000000 finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:02:42.505569 finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/sqs/
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-23 04:02:33.000000 finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/sqs/SqsEvent.py
--rw-r--r--   0 runner    (1001) docker     (127)     7168 2024-04-23 04:02:33.000000 finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/sqs/SqsHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-23 04:02:33.000000 finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/sqs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:02:42.509569 finalsa_common_lambdas-0.1.1/finalsa_common_lambdas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-23 04:02:42.000000 finalsa_common_lambdas-0.1.1/finalsa_common_lambdas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-23 04:02:42.000000 finalsa_common_lambdas-0.1.1/finalsa_common_lambdas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 04:02:42.000000 finalsa_common_lambdas-0.1.1/finalsa_common_lambdas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-23 04:02:42.000000 finalsa_common_lambdas-0.1.1/finalsa_common_lambdas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-23 04:02:42.000000 finalsa_common_lambdas-0.1.1/finalsa_common_lambdas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 04:02:42.000000 finalsa_common_lambdas-0.1.1/finalsa_common_lambdas.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-23 04:02:42.509569 finalsa_common_lambdas-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-23 04:02:33.000000 finalsa_common_lambdas-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:02:42.509569 finalsa_common_lambdas-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-23 04:02:33.000000 finalsa_common_lambdas-0.1.1/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-23 04:02:33.000000 finalsa_common_lambdas-0.1.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13351 2024-04-23 04:02:33.000000 finalsa_common_lambdas-0.1.1/tests/test_http_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-04-23 04:02:33.000000 finalsa_common_lambdas-0.1.1/tests/test_sqs_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:57.116454 finalsa_common_lambdas-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-25 14:37:52.000000 finalsa_common_lambdas-0.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-25 14:37:57.116454 finalsa_common_lambdas-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:52.000000 finalsa_common_lambdas-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:57.108454 finalsa_common_lambdas-0.2.0/finalsa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:57.108454 finalsa_common_lambdas-0.2.0/finalsa/common/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:57.112454 finalsa_common_lambdas-0.2.0/finalsa/common/lambdas/
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-25 14:37:52.000000 finalsa_common_lambdas-0.2.0/finalsa/common/lambdas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:57.112454 finalsa_common_lambdas-0.2.0/finalsa/common/lambdas/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-25 14:37:52.000000 finalsa_common_lambdas-0.2.0/finalsa/common/lambdas/app/App.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-25 14:37:52.000000 finalsa_common_lambdas-0.2.0/finalsa/common/lambdas/app/AppEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 14:37:52.000000 finalsa_common_lambdas-0.2.0/finalsa/common/lambdas/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:57.112454 finalsa_common_lambdas-0.2.0/finalsa/common/lambdas/http/
+-rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-04-25 14:37:52.000000 finalsa_common_lambdas-0.2.0/finalsa/common/lambdas/http/HttpHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-25 14:37:52.000000 finalsa_common_lambdas-0.2.0/finalsa/common/lambdas/http/HttpHeaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-25 14:37:52.000000 finalsa_common_lambdas-0.2.0/finalsa/common/lambdas/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:52.000000 finalsa_common_lambdas-0.2.0/finalsa/common/lambdas/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:57.116454 finalsa_common_lambdas-0.2.0/finalsa/common/lambdas/sqs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-25 14:37:52.000000 finalsa_common_lambdas-0.2.0/finalsa/common/lambdas/sqs/SqsEvent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7168 2024-04-25 14:37:52.000000 finalsa_common_lambdas-0.2.0/finalsa/common/lambdas/sqs/SqsHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-25 14:37:52.000000 finalsa_common_lambdas-0.2.0/finalsa/common/lambdas/sqs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:57.116454 finalsa_common_lambdas-0.2.0/finalsa_common_lambdas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-25 14:37:57.000000 finalsa_common_lambdas-0.2.0/finalsa_common_lambdas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-25 14:37:57.000000 finalsa_common_lambdas-0.2.0/finalsa_common_lambdas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 14:37:57.000000 finalsa_common_lambdas-0.2.0/finalsa_common_lambdas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-25 14:37:57.000000 finalsa_common_lambdas-0.2.0/finalsa_common_lambdas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-25 14:37:57.000000 finalsa_common_lambdas-0.2.0/finalsa_common_lambdas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 14:37:56.000000 finalsa_common_lambdas-0.2.0/finalsa_common_lambdas.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-25 14:37:57.116454 finalsa_common_lambdas-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-25 14:37:52.000000 finalsa_common_lambdas-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:57.116454 finalsa_common_lambdas-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-25 14:37:52.000000 finalsa_common_lambdas-0.2.0/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-25 14:37:52.000000 finalsa_common_lambdas-0.2.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13351 2024-04-25 14:37:52.000000 finalsa_common_lambdas-0.2.0/tests/test_http_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-04-25 14:37:52.000000 finalsa_common_lambdas-0.2.0/tests/test_sqs_service.py
```

### Comparing `finalsa_common_lambdas-0.1.1/LICENSE.md` & `finalsa_common_lambdas-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `finalsa_common_lambdas-0.1.1/PKG-INFO` & `finalsa_common_lambdas-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finalsa-common-lambdas
-Version: 0.1.1
+Version: 0.2.0
 Summary: An utils package for using finalsa common lambas.
 Home-page: https://github.com/finalsa/finalsa-common-lambda
 Author: Luis Jimenez
 Author-email: luis@finalsa.com
 License: MIT
 Keywords: dynamodb
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,14 @@
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
 Requires-Dist: finalsa-common-models>=0.0.4
 Requires-Dist: finalsa-sqs-client>=0.0.3
```

### Comparing `finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/app/App.py` & `finalsa_common_lambdas-0.2.0/finalsa/common/lambdas/app/App.py`

 * *Files identical despite different names*

### Comparing `finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/app/AppEntry.py` & `finalsa_common_lambdas-0.2.0/finalsa/common/lambdas/app/AppEntry.py`

 * *Files identical despite different names*

### Comparing `finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/http/HttpHandler.py` & `finalsa_common_lambdas-0.2.0/finalsa/common/lambdas/http/HttpHandler.py`

 * *Files identical despite different names*

### Comparing `finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/http/HttpHeaders.py` & `finalsa_common_lambdas-0.2.0/finalsa/common/lambdas/http/HttpHeaders.py`

 * *Files identical despite different names*

### Comparing `finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/sqs/SqsEvent.py` & `finalsa_common_lambdas-0.2.0/finalsa/common/lambdas/sqs/SqsEvent.py`

 * *Files identical despite different names*

### Comparing `finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/sqs/SqsHandler.py` & `finalsa_common_lambdas-0.2.0/finalsa/common/lambdas/sqs/SqsHandler.py`

 * *Files identical despite different names*

### Comparing `finalsa_common_lambdas-0.1.1/finalsa_common_lambdas.egg-info/PKG-INFO` & `finalsa_common_lambdas-0.2.0/finalsa_common_lambdas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finalsa-common-lambdas
-Version: 0.1.1
+Version: 0.2.0
 Summary: An utils package for using finalsa common lambas.
 Home-page: https://github.com/finalsa/finalsa-common-lambda
 Author: Luis Jimenez
 Author-email: luis@finalsa.com
 License: MIT
 Keywords: dynamodb
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,14 @@
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
 Requires-Dist: finalsa-common-models>=0.0.4
 Requires-Dist: finalsa-sqs-client>=0.0.3
```

### Comparing `finalsa_common_lambdas-0.1.1/finalsa_common_lambdas.egg-info/SOURCES.txt` & `finalsa_common_lambdas-0.2.0/finalsa_common_lambdas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finalsa_common_lambdas-0.1.1/setup.py` & `finalsa_common_lambdas-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
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
         "finalsa-common-models>=0.0.4",
         "finalsa-sqs-client>=0.0.3",
     ],
```

### Comparing `finalsa_common_lambdas-0.1.1/tests/test_app.py` & `finalsa_common_lambdas-0.2.0/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `finalsa_common_lambdas-0.1.1/tests/test_http_service.py` & `finalsa_common_lambdas-0.2.0/tests/test_http_service.py`

 * *Files identical despite different names*

### Comparing `finalsa_common_lambdas-0.1.1/tests/test_sqs_service.py` & `finalsa_common_lambdas-0.2.0/tests/test_sqs_service.py`

 * *Files identical despite different names*

