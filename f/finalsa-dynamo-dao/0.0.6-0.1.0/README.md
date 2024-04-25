# Comparing `tmp/finalsa-dynamo-dao-0.0.6.tar.gz` & `tmp/finalsa_dynamo_dao-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finalsa-dynamo-dao-0.0.6.tar", last modified: Thu Apr 11 01:01:11 2024, max compression
+gzip compressed data, was "finalsa_dynamo_dao-0.1.0.tar", last modified: Thu Apr 25 14:42:11 2024, max compression
```

## Comparing `finalsa-dynamo-dao-0.0.6.tar` & `finalsa_dynamo_dao-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:11.923224 finalsa-dynamo-dao-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-11 01:01:01.000000 finalsa-dynamo-dao-0.0.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-11 01:01:11.923224 finalsa-dynamo-dao-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-11 01:01:01.000000 finalsa-dynamo-dao-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:11.919224 finalsa-dynamo-dao-0.0.6/finalsa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:11.919224 finalsa-dynamo-dao-0.0.6/finalsa/dynamo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:11.923224 finalsa-dynamo-dao-0.0.6/finalsa/dynamo/dao/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-11 01:01:01.000000 finalsa-dynamo-dao-0.0.6/finalsa/dynamo/dao/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:11.923224 finalsa-dynamo-dao-0.0.6/finalsa/dynamo/dao/content/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-11 01:01:01.000000 finalsa-dynamo-dao-0.0.6/finalsa/dynamo/dao/content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-11 01:01:01.000000 finalsa-dynamo-dao-0.0.6/finalsa/dynamo/dao/content/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-11 01:01:01.000000 finalsa-dynamo-dao-0.0.6/finalsa/dynamo/dao/content/base_dao.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:01.000000 finalsa-dynamo-dao-0.0.6/finalsa/dynamo/dao/content/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:01.000000 finalsa-dynamo-dao-0.0.6/finalsa/dynamo/dao/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:11.923224 finalsa-dynamo-dao-0.0.6/finalsa_dynamo_dao.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-11 01:01:11.000000 finalsa-dynamo-dao-0.0.6/finalsa_dynamo_dao.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-11 01:01:11.000000 finalsa-dynamo-dao-0.0.6/finalsa_dynamo_dao.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 01:01:11.000000 finalsa-dynamo-dao-0.0.6/finalsa_dynamo_dao.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-11 01:01:11.000000 finalsa-dynamo-dao-0.0.6/finalsa_dynamo_dao.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-11 01:01:11.000000 finalsa-dynamo-dao-0.0.6/finalsa_dynamo_dao.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 01:01:11.000000 finalsa-dynamo-dao-0.0.6/finalsa_dynamo_dao.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-11 01:01:11.927224 finalsa-dynamo-dao-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-11 01:01:01.000000 finalsa-dynamo-dao-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:11.923224 finalsa-dynamo-dao-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-11 01:01:01.000000 finalsa-dynamo-dao-0.0.6/tests/test_dao.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:42:11.203795 finalsa_dynamo_dao-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-25 14:42:02.000000 finalsa_dynamo_dao-0.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-25 14:42:11.203795 finalsa_dynamo_dao-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-25 14:42:02.000000 finalsa_dynamo_dao-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:42:11.199795 finalsa_dynamo_dao-0.1.0/finalsa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:42:11.199795 finalsa_dynamo_dao-0.1.0/finalsa/dynamo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:42:11.203795 finalsa_dynamo_dao-0.1.0/finalsa/dynamo/dao/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-25 14:42:02.000000 finalsa_dynamo_dao-0.1.0/finalsa/dynamo/dao/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:42:11.203795 finalsa_dynamo_dao-0.1.0/finalsa/dynamo/dao/content/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-25 14:42:02.000000 finalsa_dynamo_dao-0.1.0/finalsa/dynamo/dao/content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-25 14:42:02.000000 finalsa_dynamo_dao-0.1.0/finalsa/dynamo/dao/content/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-25 14:42:02.000000 finalsa_dynamo_dao-0.1.0/finalsa/dynamo/dao/content/base_dao.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:42:02.000000 finalsa_dynamo_dao-0.1.0/finalsa/dynamo/dao/content/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:42:02.000000 finalsa_dynamo_dao-0.1.0/finalsa/dynamo/dao/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:42:11.203795 finalsa_dynamo_dao-0.1.0/finalsa_dynamo_dao.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-25 14:42:11.000000 finalsa_dynamo_dao-0.1.0/finalsa_dynamo_dao.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-25 14:42:11.000000 finalsa_dynamo_dao-0.1.0/finalsa_dynamo_dao.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 14:42:11.000000 finalsa_dynamo_dao-0.1.0/finalsa_dynamo_dao.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-25 14:42:11.000000 finalsa_dynamo_dao-0.1.0/finalsa_dynamo_dao.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-25 14:42:11.000000 finalsa_dynamo_dao-0.1.0/finalsa_dynamo_dao.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 14:42:11.000000 finalsa_dynamo_dao-0.1.0/finalsa_dynamo_dao.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-25 14:42:11.203795 finalsa_dynamo_dao-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-25 14:42:02.000000 finalsa_dynamo_dao-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:42:11.203795 finalsa_dynamo_dao-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-25 14:42:02.000000 finalsa_dynamo_dao-0.1.0/tests/test_dao.py
```

### Comparing `finalsa-dynamo-dao-0.0.6/LICENSE.md` & `finalsa_dynamo_dao-0.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `finalsa-dynamo-dao-0.0.6/PKG-INFO` & `finalsa_dynamo_dao-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finalsa-dynamo-dao
-Version: 0.0.6
+Version: 0.1.0
 Summary: An utils package for using dynamodb
 Home-page: https://github.com/finalsa/finalsa-dynamo-dao
 Author: Luis Jimenez
 Author-email: luis@finalsa.com
 License: MIT
 Keywords: dynamodb
 Classifier: Intended Audience :: Developers
@@ -12,15 +12,15 @@
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
 
 Dynamo Dao
 
 ## Description
```

### Comparing `finalsa-dynamo-dao-0.0.6/README.md` & `finalsa_dynamo_dao-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `finalsa-dynamo-dao-0.0.6/finalsa/dynamo/dao/content/base.py` & `finalsa_dynamo_dao-0.1.0/finalsa/dynamo/dao/content/base.py`

 * *Files identical despite different names*

### Comparing `finalsa-dynamo-dao-0.0.6/finalsa/dynamo/dao/content/base_dao.py` & `finalsa_dynamo_dao-0.1.0/finalsa/dynamo/dao/content/base_dao.py`

 * *Files identical despite different names*

### Comparing `finalsa-dynamo-dao-0.0.6/finalsa_dynamo_dao.egg-info/PKG-INFO` & `finalsa_dynamo_dao-0.1.0/finalsa_dynamo_dao.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finalsa-dynamo-dao
-Version: 0.0.6
+Version: 0.1.0
 Summary: An utils package for using dynamodb
 Home-page: https://github.com/finalsa/finalsa-dynamo-dao
 Author: Luis Jimenez
 Author-email: luis@finalsa.com
 License: MIT
 Keywords: dynamodb
 Classifier: Intended Audience :: Developers
@@ -12,15 +12,15 @@
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
 
 Dynamo Dao
 
 ## Description
```

### Comparing `finalsa-dynamo-dao-0.0.6/setup.py` & `finalsa_dynamo_dao-0.1.0/setup.py`

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
         "boto3>=1.20.3"
     ],
     extras_require={
     
     },
```

### Comparing `finalsa-dynamo-dao-0.0.6/tests/test_dao.py` & `finalsa_dynamo_dao-0.1.0/tests/test_dao.py`

 * *Files identical despite different names*

