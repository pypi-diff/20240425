# Comparing `tmp/finalsa-sns-client-0.0.4.tar.gz` & `tmp/finalsa_sns_client-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finalsa-sns-client-0.0.4.tar", last modified: Fri Mar 29 06:12:04 2024, max compression
+gzip compressed data, was "finalsa_sns_client-0.1.0.tar", last modified: Thu Apr 25 14:33:14 2024, max compression
```

## Comparing `finalsa-sns-client-0.0.4.tar` & `finalsa_sns_client-0.1.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 06:12:04.656728 finalsa-sns-client-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-03-29 06:11:56.000000 finalsa-sns-client-0.0.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-03-29 06:12:04.656728 finalsa-sns-client-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 06:11:56.000000 finalsa-sns-client-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 06:12:04.648728 finalsa-sns-client-0.0.4/finalsa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 06:12:04.648728 finalsa-sns-client-0.0.4/finalsa/sns/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 06:12:04.652728 finalsa-sns-client-0.0.4/finalsa/sns/client/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-29 06:11:56.000000 finalsa-sns-client-0.0.4/finalsa/sns/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 06:12:04.652728 finalsa-sns-client-0.0.4/finalsa/sns/client/client/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-29 06:11:56.000000 finalsa-sns-client-0.0.4/finalsa/sns/client/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5745 2024-03-29 06:11:56.000000 finalsa-sns-client-0.0.4/finalsa/sns/client/client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 06:12:04.652728 finalsa-sns-client-0.0.4/finalsa/sns/client/interface/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-29 06:11:56.000000 finalsa-sns-client-0.0.4/finalsa/sns/client/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-03-29 06:11:56.000000 finalsa-sns-client-0.0.4/finalsa/sns/client/interface/client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 06:11:56.000000 finalsa-sns-client-0.0.4/finalsa/sns/client/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 06:12:04.652728 finalsa-sns-client-0.0.4/finalsa/sns/client/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-29 06:11:56.000000 finalsa-sns-client-0.0.4/finalsa/sns/client/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-03-29 06:11:56.000000 finalsa-sns-client-0.0.4/finalsa/sns/client/tests/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 06:12:04.656728 finalsa-sns-client-0.0.4/finalsa_sns_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-03-29 06:12:04.000000 finalsa-sns-client-0.0.4/finalsa_sns_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-03-29 06:12:04.000000 finalsa-sns-client-0.0.4/finalsa_sns_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 06:12:04.000000 finalsa-sns-client-0.0.4/finalsa_sns_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-29 06:12:04.000000 finalsa-sns-client-0.0.4/finalsa_sns_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-29 06:12:04.000000 finalsa-sns-client-0.0.4/finalsa_sns_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 06:12:04.000000 finalsa-sns-client-0.0.4/finalsa_sns_client.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-29 06:12:04.656728 finalsa-sns-client-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-03-29 06:11:56.000000 finalsa-sns-client-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 06:12:04.656728 finalsa-sns-client-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-03-29 06:11:56.000000 finalsa-sns-client-0.0.4/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:33:14.664919 finalsa_sns_client-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-25 14:33:05.000000 finalsa_sns_client-0.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-25 14:33:14.664919 finalsa_sns_client-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:33:05.000000 finalsa_sns_client-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:33:14.660918 finalsa_sns_client-0.1.0/finalsa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:33:14.660918 finalsa_sns_client-0.1.0/finalsa/sns/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:33:14.664919 finalsa_sns_client-0.1.0/finalsa/sns/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-25 14:33:05.000000 finalsa_sns_client-0.1.0/finalsa/sns/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:33:14.664919 finalsa_sns_client-0.1.0/finalsa/sns/client/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-25 14:33:05.000000 finalsa_sns_client-0.1.0/finalsa/sns/client/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5745 2024-04-25 14:33:05.000000 finalsa_sns_client-0.1.0/finalsa/sns/client/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:33:14.664919 finalsa_sns_client-0.1.0/finalsa/sns/client/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-25 14:33:05.000000 finalsa_sns_client-0.1.0/finalsa/sns/client/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-25 14:33:05.000000 finalsa_sns_client-0.1.0/finalsa/sns/client/interface/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:33:05.000000 finalsa_sns_client-0.1.0/finalsa/sns/client/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:33:14.664919 finalsa_sns_client-0.1.0/finalsa/sns/client/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-25 14:33:05.000000 finalsa_sns_client-0.1.0/finalsa/sns/client/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-25 14:33:05.000000 finalsa_sns_client-0.1.0/finalsa/sns/client/tests/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:33:14.664919 finalsa_sns_client-0.1.0/finalsa_sns_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-25 14:33:14.000000 finalsa_sns_client-0.1.0/finalsa_sns_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-25 14:33:14.000000 finalsa_sns_client-0.1.0/finalsa_sns_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 14:33:14.000000 finalsa_sns_client-0.1.0/finalsa_sns_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-25 14:33:14.000000 finalsa_sns_client-0.1.0/finalsa_sns_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-25 14:33:14.000000 finalsa_sns_client-0.1.0/finalsa_sns_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 14:33:14.000000 finalsa_sns_client-0.1.0/finalsa_sns_client.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-25 14:33:14.664919 finalsa_sns_client-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-25 14:33:05.000000 finalsa_sns_client-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:33:14.664919 finalsa_sns_client-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-04-25 14:33:05.000000 finalsa_sns_client-0.1.0/tests/test_client.py
```

### Comparing `finalsa-sns-client-0.0.4/LICENSE.md` & `finalsa_sns_client-0.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `finalsa-sns-client-0.0.4/PKG-INFO` & `finalsa_sns_client-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finalsa-sns-client
-Version: 0.0.4
+Version: 0.1.0
 Summary: An utils package for using dynamodb
 Home-page: https://github.com/finalsa/sns-client
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
 Requires-Dist: finalsa-common-models>=0.0.2
```

### Comparing `finalsa-sns-client-0.0.4/finalsa/sns/client/client/client.py` & `finalsa_sns_client-0.1.0/finalsa/sns/client/client/client.py`

 * *Files identical despite different names*

### Comparing `finalsa-sns-client-0.0.4/finalsa/sns/client/interface/client.py` & `finalsa_sns_client-0.1.0/finalsa/sns/client/interface/client.py`

 * *Files identical despite different names*

### Comparing `finalsa-sns-client-0.0.4/finalsa/sns/client/tests/client.py` & `finalsa_sns_client-0.1.0/finalsa/sns/client/tests/client.py`

 * *Files identical despite different names*

### Comparing `finalsa-sns-client-0.0.4/finalsa_sns_client.egg-info/PKG-INFO` & `finalsa_sns_client-0.1.0/finalsa_sns_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finalsa-sns-client
-Version: 0.0.4
+Version: 0.1.0
 Summary: An utils package for using dynamodb
 Home-page: https://github.com/finalsa/sns-client
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
 Requires-Dist: finalsa-common-models>=0.0.2
```

### Comparing `finalsa-sns-client-0.0.4/finalsa_sns_client.egg-info/SOURCES.txt` & `finalsa_sns_client-0.1.0/finalsa_sns_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finalsa-sns-client-0.0.4/setup.py` & `finalsa_sns_client-0.1.0/setup.py`

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
         "finalsa-common-models>=0.0.2",
     ],
     extras_require={
```

### Comparing `finalsa-sns-client-0.0.4/tests/test_client.py` & `finalsa_sns_client-0.1.0/tests/test_client.py`

 * *Files identical despite different names*

