# Comparing `tmp/finalsa_s3_client-0.0.2.tar.gz` & `tmp/finalsa_s3_client-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finalsa_s3_client-0.0.2.tar", last modified: Wed Apr 24 12:57:25 2024, max compression
+gzip compressed data, was "finalsa_s3_client-0.1.0.tar", last modified: Thu Apr 25 14:40:08 2024, max compression
```

## Comparing `finalsa_s3_client-0.0.2.tar` & `finalsa_s3_client-0.1.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:25.235166 finalsa_s3_client-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-24 12:57:15.000000 finalsa_s3_client-0.0.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-24 12:57:25.235166 finalsa_s3_client-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:15.000000 finalsa_s3_client-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:25.227166 finalsa_s3_client-0.0.2/finalsa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:25.227166 finalsa_s3_client-0.0.2/finalsa/s3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:25.231166 finalsa_s3_client-0.0.2/finalsa/s3/client/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-24 12:57:15.000000 finalsa_s3_client-0.0.2/finalsa/s3/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:25.231166 finalsa_s3_client-0.0.2/finalsa/s3/client/client/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-24 12:57:15.000000 finalsa_s3_client-0.0.2/finalsa/s3/client/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-24 12:57:15.000000 finalsa_s3_client-0.0.2/finalsa/s3/client/client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:25.231166 finalsa_s3_client-0.0.2/finalsa/s3/client/interface/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-24 12:57:15.000000 finalsa_s3_client-0.0.2/finalsa/s3/client/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-24 12:57:15.000000 finalsa_s3_client-0.0.2/finalsa/s3/client/interface/client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:15.000000 finalsa_s3_client-0.0.2/finalsa/s3/client/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:25.231166 finalsa_s3_client-0.0.2/finalsa/s3/client/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-24 12:57:15.000000 finalsa_s3_client-0.0.2/finalsa/s3/client/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-24 12:57:15.000000 finalsa_s3_client-0.0.2/finalsa/s3/client/tests/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:25.231166 finalsa_s3_client-0.0.2/finalsa_s3_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-24 12:57:25.000000 finalsa_s3_client-0.0.2/finalsa_s3_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-24 12:57:25.000000 finalsa_s3_client-0.0.2/finalsa_s3_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 12:57:25.000000 finalsa_s3_client-0.0.2/finalsa_s3_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-24 12:57:25.000000 finalsa_s3_client-0.0.2/finalsa_s3_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-24 12:57:25.000000 finalsa_s3_client-0.0.2/finalsa_s3_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 12:57:25.000000 finalsa_s3_client-0.0.2/finalsa_s3_client.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-24 12:57:25.235166 finalsa_s3_client-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-24 12:57:15.000000 finalsa_s3_client-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:25.231166 finalsa_s3_client-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-24 12:57:15.000000 finalsa_s3_client-0.0.2/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:40:08.820468 finalsa_s3_client-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-25 14:40:02.000000 finalsa_s3_client-0.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-25 14:40:08.820468 finalsa_s3_client-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:40:02.000000 finalsa_s3_client-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:40:08.816467 finalsa_s3_client-0.1.0/finalsa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:40:08.816467 finalsa_s3_client-0.1.0/finalsa/s3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:40:08.816467 finalsa_s3_client-0.1.0/finalsa/s3/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-25 14:40:02.000000 finalsa_s3_client-0.1.0/finalsa/s3/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:40:08.816467 finalsa_s3_client-0.1.0/finalsa/s3/client/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-25 14:40:02.000000 finalsa_s3_client-0.1.0/finalsa/s3/client/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-25 14:40:02.000000 finalsa_s3_client-0.1.0/finalsa/s3/client/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:40:08.816467 finalsa_s3_client-0.1.0/finalsa/s3/client/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-25 14:40:02.000000 finalsa_s3_client-0.1.0/finalsa/s3/client/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-25 14:40:02.000000 finalsa_s3_client-0.1.0/finalsa/s3/client/interface/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:40:02.000000 finalsa_s3_client-0.1.0/finalsa/s3/client/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:40:08.816467 finalsa_s3_client-0.1.0/finalsa/s3/client/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-25 14:40:02.000000 finalsa_s3_client-0.1.0/finalsa/s3/client/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-25 14:40:02.000000 finalsa_s3_client-0.1.0/finalsa/s3/client/tests/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:40:08.820468 finalsa_s3_client-0.1.0/finalsa_s3_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-25 14:40:08.000000 finalsa_s3_client-0.1.0/finalsa_s3_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-25 14:40:08.000000 finalsa_s3_client-0.1.0/finalsa_s3_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 14:40:08.000000 finalsa_s3_client-0.1.0/finalsa_s3_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-25 14:40:08.000000 finalsa_s3_client-0.1.0/finalsa_s3_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-25 14:40:08.000000 finalsa_s3_client-0.1.0/finalsa_s3_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 14:40:08.000000 finalsa_s3_client-0.1.0/finalsa_s3_client.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-25 14:40:08.820468 finalsa_s3_client-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-25 14:40:02.000000 finalsa_s3_client-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:40:08.820468 finalsa_s3_client-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-25 14:40:02.000000 finalsa_s3_client-0.1.0/tests/test_client.py
```

### Comparing `finalsa_s3_client-0.0.2/LICENSE.md` & `finalsa_s3_client-0.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `finalsa_s3_client-0.0.2/PKG-INFO` & `finalsa_s3_client-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finalsa-s3-client
-Version: 0.0.2
+Version: 0.1.0
 Summary: An utils package for using s3
 Home-page: https://github.com/finalsa/finalsa-s3-client
 Author: Luis Jimenez
 Author-email: luis@finalsa.com
 License: MIT
 Keywords: s3
 Classifier: Intended Audience :: Developers
@@ -12,11 +12,11 @@
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
```

### Comparing `finalsa_s3_client-0.0.2/finalsa/s3/client/client/client.py` & `finalsa_s3_client-0.1.0/finalsa/s3/client/client/client.py`

 * *Files identical despite different names*

### Comparing `finalsa_s3_client-0.0.2/finalsa/s3/client/interface/client.py` & `finalsa_s3_client-0.1.0/finalsa/s3/client/interface/client.py`

 * *Files identical despite different names*

### Comparing `finalsa_s3_client-0.0.2/finalsa/s3/client/tests/client.py` & `finalsa_s3_client-0.1.0/finalsa/s3/client/tests/client.py`

 * *Files identical despite different names*

### Comparing `finalsa_s3_client-0.0.2/finalsa_s3_client.egg-info/PKG-INFO` & `finalsa_s3_client-0.1.0/finalsa_s3_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finalsa-s3-client
-Version: 0.0.2
+Version: 0.1.0
 Summary: An utils package for using s3
 Home-page: https://github.com/finalsa/finalsa-s3-client
 Author: Luis Jimenez
 Author-email: luis@finalsa.com
 License: MIT
 Keywords: s3
 Classifier: Intended Audience :: Developers
@@ -12,11 +12,11 @@
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
```

### Comparing `finalsa_s3_client-0.0.2/finalsa_s3_client.egg-info/SOURCES.txt` & `finalsa_s3_client-0.1.0/finalsa_s3_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finalsa_s3_client-0.0.2/setup.py` & `finalsa_s3_client-0.1.0/setup.py`

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

### Comparing `finalsa_s3_client-0.0.2/tests/test_client.py` & `finalsa_s3_client-0.1.0/tests/test_client.py`

 * *Files identical despite different names*

