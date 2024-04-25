# Comparing `tmp/finalsa-sqs-client-0.0.5.tar.gz` & `tmp/finalsa_sqs_client-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finalsa-sqs-client-0.0.5.tar", last modified: Fri Mar 29 05:03:17 2024, max compression
+gzip compressed data, was "finalsa_sqs_client-0.1.0.tar", last modified: Thu Apr 25 14:37:06 2024, max compression
```

## Comparing `finalsa-sqs-client-0.0.5.tar` & `finalsa_sqs_client-0.1.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:03:17.216278 finalsa-sqs-client-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-03-29 05:03:09.000000 finalsa-sqs-client-0.0.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-03-29 05:03:17.216278 finalsa-sqs-client-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 05:03:09.000000 finalsa-sqs-client-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:03:17.212278 finalsa-sqs-client-0.0.5/finalsa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:03:17.212278 finalsa-sqs-client-0.0.5/finalsa/sqs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:03:17.216278 finalsa-sqs-client-0.0.5/finalsa/sqs/client/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-29 05:03:09.000000 finalsa-sqs-client-0.0.5/finalsa/sqs/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:03:17.216278 finalsa-sqs-client-0.0.5/finalsa/sqs/client/clients/
--rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-03-29 05:03:09.000000 finalsa-sqs-client-0.0.5/finalsa/sqs/client/clients/Client.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-29 05:03:09.000000 finalsa-sqs-client-0.0.5/finalsa/sqs/client/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:03:17.216278 finalsa-sqs-client-0.0.5/finalsa/sqs/client/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-29 05:03:09.000000 finalsa-sqs-client-0.0.5/finalsa/sqs/client/exceptions/SqsException.py
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-29 05:03:09.000000 finalsa-sqs-client-0.0.5/finalsa/sqs/client/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:03:17.216278 finalsa-sqs-client-0.0.5/finalsa/sqs/client/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-03-29 05:03:09.000000 finalsa-sqs-client-0.0.5/finalsa/sqs/client/interfaces/SqsService.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-29 05:03:09.000000 finalsa-sqs-client-0.0.5/finalsa/sqs/client/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 05:03:09.000000 finalsa-sqs-client-0.0.5/finalsa/sqs/client/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:03:17.216278 finalsa-sqs-client-0.0.5/finalsa/sqs/client/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-03-29 05:03:09.000000 finalsa-sqs-client-0.0.5/finalsa/sqs/client/tests/Client.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-29 05:03:09.000000 finalsa-sqs-client-0.0.5/finalsa/sqs/client/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:03:17.216278 finalsa-sqs-client-0.0.5/finalsa_sqs_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-03-29 05:03:17.000000 finalsa-sqs-client-0.0.5/finalsa_sqs_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-03-29 05:03:17.000000 finalsa-sqs-client-0.0.5/finalsa_sqs_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 05:03:17.000000 finalsa-sqs-client-0.0.5/finalsa_sqs_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-29 05:03:17.000000 finalsa-sqs-client-0.0.5/finalsa_sqs_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-29 05:03:17.000000 finalsa-sqs-client-0.0.5/finalsa_sqs_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 05:03:17.000000 finalsa-sqs-client-0.0.5/finalsa_sqs_client.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-29 05:03:17.220278 finalsa-sqs-client-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-03-29 05:03:09.000000 finalsa-sqs-client-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:03:17.216278 finalsa-sqs-client-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-03-29 05:03:09.000000 finalsa-sqs-client-0.0.5/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:06.301103 finalsa_sqs_client-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-25 14:37:02.000000 finalsa_sqs_client-0.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-25 14:37:06.301103 finalsa_sqs_client-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:02.000000 finalsa_sqs_client-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:06.297104 finalsa_sqs_client-0.1.0/finalsa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:06.297104 finalsa_sqs_client-0.1.0/finalsa/sqs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:06.297104 finalsa_sqs_client-0.1.0/finalsa/sqs/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-25 14:37:02.000000 finalsa_sqs_client-0.1.0/finalsa/sqs/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:06.301103 finalsa_sqs_client-0.1.0/finalsa/sqs/client/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-04-25 14:37:02.000000 finalsa_sqs_client-0.1.0/finalsa/sqs/client/clients/Client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-25 14:37:02.000000 finalsa_sqs_client-0.1.0/finalsa/sqs/client/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:06.301103 finalsa_sqs_client-0.1.0/finalsa/sqs/client/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-25 14:37:02.000000 finalsa_sqs_client-0.1.0/finalsa/sqs/client/exceptions/SqsException.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-25 14:37:02.000000 finalsa_sqs_client-0.1.0/finalsa/sqs/client/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:06.301103 finalsa_sqs_client-0.1.0/finalsa/sqs/client/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-25 14:37:02.000000 finalsa_sqs_client-0.1.0/finalsa/sqs/client/interfaces/SqsService.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-25 14:37:02.000000 finalsa_sqs_client-0.1.0/finalsa/sqs/client/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:02.000000 finalsa_sqs_client-0.1.0/finalsa/sqs/client/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:06.301103 finalsa_sqs_client-0.1.0/finalsa/sqs/client/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-25 14:37:02.000000 finalsa_sqs_client-0.1.0/finalsa/sqs/client/tests/Client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-25 14:37:02.000000 finalsa_sqs_client-0.1.0/finalsa/sqs/client/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:06.301103 finalsa_sqs_client-0.1.0/finalsa_sqs_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-25 14:37:06.000000 finalsa_sqs_client-0.1.0/finalsa_sqs_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-25 14:37:06.000000 finalsa_sqs_client-0.1.0/finalsa_sqs_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 14:37:06.000000 finalsa_sqs_client-0.1.0/finalsa_sqs_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-25 14:37:06.000000 finalsa_sqs_client-0.1.0/finalsa_sqs_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-25 14:37:06.000000 finalsa_sqs_client-0.1.0/finalsa_sqs_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 14:37:06.000000 finalsa_sqs_client-0.1.0/finalsa_sqs_client.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-25 14:37:06.301103 finalsa_sqs_client-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-25 14:37:02.000000 finalsa_sqs_client-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:06.301103 finalsa_sqs_client-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-25 14:37:02.000000 finalsa_sqs_client-0.1.0/tests/test_client.py
```

### Comparing `finalsa-sqs-client-0.0.5/LICENSE.md` & `finalsa_sqs_client-0.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `finalsa-sqs-client-0.0.5/PKG-INFO` & `finalsa_sqs_client-0.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finalsa-sqs-client
-Version: 0.0.5
+Version: 0.1.0
 Summary: An utils package for using sqs.
 Home-page: https://github.com/finalsa/sqs-client
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
 Requires-Dist: finalsa-common-models>=0.0.4
```

### Comparing `finalsa-sqs-client-0.0.5/finalsa/sqs/client/clients/Client.py` & `finalsa_sqs_client-0.1.0/finalsa/sqs/client/clients/Client.py`

 * *Files identical despite different names*

### Comparing `finalsa-sqs-client-0.0.5/finalsa/sqs/client/interfaces/SqsService.py` & `finalsa_sqs_client-0.1.0/finalsa/sqs/client/interfaces/SqsService.py`

 * *Files identical despite different names*

### Comparing `finalsa-sqs-client-0.0.5/finalsa/sqs/client/tests/Client.py` & `finalsa_sqs_client-0.1.0/finalsa/sqs/client/tests/Client.py`

 * *Files identical despite different names*

### Comparing `finalsa-sqs-client-0.0.5/finalsa_sqs_client.egg-info/PKG-INFO` & `finalsa_sqs_client-0.1.0/finalsa_sqs_client.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finalsa-sqs-client
-Version: 0.0.5
+Version: 0.1.0
 Summary: An utils package for using sqs.
 Home-page: https://github.com/finalsa/sqs-client
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
 Requires-Dist: finalsa-common-models>=0.0.4
```

### Comparing `finalsa-sqs-client-0.0.5/finalsa_sqs_client.egg-info/SOURCES.txt` & `finalsa_sqs_client-0.1.0/finalsa_sqs_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finalsa-sqs-client-0.0.5/setup.py` & `finalsa_sqs_client-0.1.0/setup.py`

 * *Files 0% similar despite different names*

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
         "finalsa-common-models>=0.0.4"
     ],
     extras_require={
```

### Comparing `finalsa-sqs-client-0.0.5/tests/test_client.py` & `finalsa_sqs_client-0.1.0/tests/test_client.py`

 * *Files identical despite different names*

