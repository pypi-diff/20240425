# Comparing `tmp/finalsa-dependency-injector-0.0.1.tar.gz` & `tmp/finalsa_dependency_injector-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finalsa-dependency-injector-0.0.1.tar", last modified: Mon Mar 18 01:02:24 2024, max compression
+gzip compressed data, was "finalsa_dependency_injector-0.1.0.tar", last modified: Thu Apr 25 14:44:16 2024, max compression
```

## Comparing `finalsa-dependency-injector-0.0.1.tar` & `finalsa_dependency_injector-0.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 01:02:24.420296 finalsa-dependency-injector-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-03-18 01:02:15.000000 finalsa-dependency-injector-0.0.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-03-18 01:02:24.420296 finalsa-dependency-injector-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 01:02:15.000000 finalsa-dependency-injector-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 01:02:24.416296 finalsa-dependency-injector-0.0.1/finalsa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 01:02:24.416296 finalsa-dependency-injector-0.0.1/finalsa/dependency/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 01:02:24.416296 finalsa-dependency-injector-0.0.1/finalsa/dependency/injector/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-03-18 01:02:15.000000 finalsa-dependency-injector-0.0.1/finalsa/dependency/injector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 01:02:24.416296 finalsa-dependency-injector-0.0.1/finalsa/dependency/injector/container/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-18 01:02:15.000000 finalsa-dependency-injector-0.0.1/finalsa/dependency/injector/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-03-18 01:02:15.000000 finalsa-dependency-injector-0.0.1/finalsa/dependency/injector/container/container.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-18 01:02:15.000000 finalsa-dependency-injector-0.0.1/finalsa/dependency/injector/container/life_cycle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 01:02:24.420296 finalsa-dependency-injector-0.0.1/finalsa/dependency/injector/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-18 01:02:15.000000 finalsa-dependency-injector-0.0.1/finalsa/dependency/injector/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-18 01:02:15.000000 finalsa-dependency-injector-0.0.1/finalsa/dependency/injector/exceptions/dependency_not_found.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-18 01:02:15.000000 finalsa-dependency-injector-0.0.1/finalsa/dependency/injector/exceptions/invalid_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 01:02:15.000000 finalsa-dependency-injector-0.0.1/finalsa/dependency/injector/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 01:02:24.420296 finalsa-dependency-injector-0.0.1/finalsa_dependency_injector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-03-18 01:02:24.000000 finalsa-dependency-injector-0.0.1/finalsa_dependency_injector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-18 01:02:24.000000 finalsa-dependency-injector-0.0.1/finalsa_dependency_injector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 01:02:24.000000 finalsa-dependency-injector-0.0.1/finalsa_dependency_injector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-18 01:02:24.000000 finalsa-dependency-injector-0.0.1/finalsa_dependency_injector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 01:02:24.000000 finalsa-dependency-injector-0.0.1/finalsa_dependency_injector.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-18 01:02:24.420296 finalsa-dependency-injector-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-03-18 01:02:15.000000 finalsa-dependency-injector-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 01:02:24.420296 finalsa-dependency-injector-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-03-18 01:02:15.000000 finalsa-dependency-injector-0.0.1/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:44:16.673295 finalsa_dependency_injector-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-25 14:44:11.000000 finalsa_dependency_injector-0.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-25 14:44:16.673295 finalsa_dependency_injector-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:44:11.000000 finalsa_dependency_injector-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:44:16.669295 finalsa_dependency_injector-0.1.0/finalsa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:44:16.669295 finalsa_dependency_injector-0.1.0/finalsa/dependency/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:44:16.669295 finalsa_dependency_injector-0.1.0/finalsa/dependency/injector/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-25 14:44:11.000000 finalsa_dependency_injector-0.1.0/finalsa/dependency/injector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:44:16.669295 finalsa_dependency_injector-0.1.0/finalsa/dependency/injector/container/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-25 14:44:11.000000 finalsa_dependency_injector-0.1.0/finalsa/dependency/injector/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-04-25 14:44:11.000000 finalsa_dependency_injector-0.1.0/finalsa/dependency/injector/container/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-25 14:44:11.000000 finalsa_dependency_injector-0.1.0/finalsa/dependency/injector/container/life_cycle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:44:16.669295 finalsa_dependency_injector-0.1.0/finalsa/dependency/injector/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-25 14:44:11.000000 finalsa_dependency_injector-0.1.0/finalsa/dependency/injector/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-25 14:44:11.000000 finalsa_dependency_injector-0.1.0/finalsa/dependency/injector/exceptions/dependency_not_found.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-25 14:44:11.000000 finalsa_dependency_injector-0.1.0/finalsa/dependency/injector/exceptions/invalid_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:44:11.000000 finalsa_dependency_injector-0.1.0/finalsa/dependency/injector/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:44:16.673295 finalsa_dependency_injector-0.1.0/finalsa_dependency_injector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-25 14:44:16.000000 finalsa_dependency_injector-0.1.0/finalsa_dependency_injector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-25 14:44:16.000000 finalsa_dependency_injector-0.1.0/finalsa_dependency_injector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 14:44:16.000000 finalsa_dependency_injector-0.1.0/finalsa_dependency_injector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-25 14:44:16.000000 finalsa_dependency_injector-0.1.0/finalsa_dependency_injector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 14:44:16.000000 finalsa_dependency_injector-0.1.0/finalsa_dependency_injector.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-25 14:44:16.673295 finalsa_dependency_injector-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-25 14:44:11.000000 finalsa_dependency_injector-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:44:16.673295 finalsa_dependency_injector-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-25 14:44:11.000000 finalsa_dependency_injector-0.1.0/tests/test_client.py
```

### Comparing `finalsa-dependency-injector-0.0.1/LICENSE.md` & `finalsa_dependency_injector-0.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `finalsa-dependency-injector-0.0.1/PKG-INFO` & `finalsa_dependency_injector-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finalsa-dependency-injector
-Version: 0.0.1
+Version: 0.1.0
 Summary: An utils package for dependency injection .
 Home-page: https://github.com/finalsa/finalsa-dependency-inyector
 Author: Luis Jimenez
 Author-email: luis@finalsa.com
 License: MIT
 Keywords: Injection,Dependency,Python,Finalsa
 Classifier: Intended Audience :: Developers
@@ -12,10 +12,10 @@
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
```

### Comparing `finalsa-dependency-injector-0.0.1/finalsa/dependency/injector/container/container.py` & `finalsa_dependency_injector-0.1.0/finalsa/dependency/injector/container/container.py`

 * *Files identical despite different names*

### Comparing `finalsa-dependency-injector-0.0.1/finalsa_dependency_injector.egg-info/PKG-INFO` & `finalsa_dependency_injector-0.1.0/finalsa_dependency_injector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finalsa-dependency-injector
-Version: 0.0.1
+Version: 0.1.0
 Summary: An utils package for dependency injection .
 Home-page: https://github.com/finalsa/finalsa-dependency-inyector
 Author: Luis Jimenez
 Author-email: luis@finalsa.com
 License: MIT
 Keywords: Injection,Dependency,Python,Finalsa
 Classifier: Intended Audience :: Developers
@@ -12,10 +12,10 @@
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
```

### Comparing `finalsa-dependency-injector-0.0.1/finalsa_dependency_injector.egg-info/SOURCES.txt` & `finalsa_dependency_injector-0.1.0/finalsa_dependency_injector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finalsa-dependency-injector-0.0.1/setup.py` & `finalsa_dependency_injector-0.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
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
        
     ],
     extras_require={
     
     },
```

### Comparing `finalsa-dependency-injector-0.0.1/tests/test_client.py` & `finalsa_dependency_injector-0.1.0/tests/test_client.py`

 * *Files identical despite different names*

