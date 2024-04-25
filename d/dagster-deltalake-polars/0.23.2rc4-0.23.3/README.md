# Comparing `tmp/dagster-deltalake-polars-0.23.2rc4.tar.gz` & `tmp/dagster-deltalake-polars-0.23.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-deltalake-polars-0.23.2rc4.tar", last modified: Fri Apr 19 18:12:57 2024, max compression
+gzip compressed data, was "dagster-deltalake-polars-0.23.3.tar", last modified: Thu Apr 25 20:16:58 2024, max compression
```

## Comparing `dagster-deltalake-polars-0.23.2rc4.tar` & `dagster-deltalake-polars-0.23.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:12:57.734020 dagster-deltalake-polars-0.23.2rc4/
--rw-r--r--   0 root         (0) root         (0)    11344 2024-04-19 18:01:50.000000 dagster-deltalake-polars-0.23.2rc4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       58 2024-04-19 18:01:50.000000 dagster-deltalake-polars-0.23.2rc4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      781 2024-04-19 18:12:57.734020 dagster-deltalake-polars-0.23.2rc4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      158 2024-04-19 18:01:50.000000 dagster-deltalake-polars-0.23.2rc4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:12:57.734020 dagster-deltalake-polars-0.23.2rc4/dagster_deltalake_polars/
--rw-r--r--   0 root         (0) root         (0)      334 2024-04-19 18:01:50.000000 dagster-deltalake-polars-0.23.2rc4/dagster_deltalake_polars/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2617 2024-04-19 18:01:50.000000 dagster-deltalake-polars-0.23.2rc4/dagster_deltalake_polars/deltalake_polars_type_handler.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-19 18:01:50.000000 dagster-deltalake-polars-0.23.2rc4/dagster_deltalake_polars/py.typed
--rw-r--r--   0 root         (0) root         (0)       26 2024-04-19 18:01:50.000000 dagster-deltalake-polars-0.23.2rc4/dagster_deltalake_polars/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:12:57.734020 dagster-deltalake-polars-0.23.2rc4/dagster_deltalake_polars.egg-info/
--rw-r--r--   0 root         (0) root         (0)      781 2024-04-19 18:12:57.000000 dagster-deltalake-polars-0.23.2rc4/dagster_deltalake_polars.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      499 2024-04-19 18:12:57.000000 dagster-deltalake-polars-0.23.2rc4/dagster_deltalake_polars.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 18:12:57.000000 dagster-deltalake-polars-0.23.2rc4/dagster_deltalake_polars.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 18:12:57.000000 dagster-deltalake-polars-0.23.2rc4/dagster_deltalake_polars.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       63 2024-04-19 18:12:57.000000 dagster-deltalake-polars-0.23.2rc4/dagster_deltalake_polars.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-19 18:12:57.000000 dagster-deltalake-polars-0.23.2rc4/dagster_deltalake_polars.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      135 2024-04-19 18:12:57.738020 dagster-deltalake-polars-0.23.2rc4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1499 2024-04-19 18:01:50.000000 dagster-deltalake-polars-0.23.2rc4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:16:58.239961 dagster-deltalake-polars-0.23.3/
+-rw-r--r--   0 root         (0) root         (0)    11344 2024-04-25 20:08:31.000000 dagster-deltalake-polars-0.23.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       58 2024-04-25 20:08:31.000000 dagster-deltalake-polars-0.23.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      778 2024-04-25 20:16:58.239961 dagster-deltalake-polars-0.23.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      158 2024-04-25 20:08:31.000000 dagster-deltalake-polars-0.23.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:16:58.239961 dagster-deltalake-polars-0.23.3/dagster_deltalake_polars/
+-rw-r--r--   0 root         (0) root         (0)      334 2024-04-25 20:08:31.000000 dagster-deltalake-polars-0.23.3/dagster_deltalake_polars/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2617 2024-04-25 20:08:31.000000 dagster-deltalake-polars-0.23.3/dagster_deltalake_polars/deltalake_polars_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-deltalake-polars-0.23.3/dagster_deltalake_polars/py.typed
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-25 20:08:31.000000 dagster-deltalake-polars-0.23.3/dagster_deltalake_polars/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:16:58.239961 dagster-deltalake-polars-0.23.3/dagster_deltalake_polars.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      778 2024-04-25 20:16:58.000000 dagster-deltalake-polars-0.23.3/dagster_deltalake_polars.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      499 2024-04-25 20:16:58.000000 dagster-deltalake-polars-0.23.3/dagster_deltalake_polars.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 20:16:58.000000 dagster-deltalake-polars-0.23.3/dagster_deltalake_polars.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 20:16:58.000000 dagster-deltalake-polars-0.23.3/dagster_deltalake_polars.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       57 2024-04-25 20:16:58.000000 dagster-deltalake-polars-0.23.3/dagster_deltalake_polars.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-25 20:16:58.000000 dagster-deltalake-polars-0.23.3/dagster_deltalake_polars.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      135 2024-04-25 20:16:58.239961 dagster-deltalake-polars-0.23.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1493 2024-04-25 20:08:31.000000 dagster-deltalake-polars-0.23.3/setup.py
```

### Comparing `dagster-deltalake-polars-0.23.2rc4/LICENSE` & `dagster-deltalake-polars-0.23.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-deltalake-polars-0.23.2rc4/PKG-INFO` & `dagster-deltalake-polars-0.23.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-deltalake-polars
-Version: 0.23.2rc4
+Version: 0.23.3
 Summary: Package for storing Polars DataFrames in Delta tables.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-deltalake-polars
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-deltalake-polars-0.23.2rc4/dagster_deltalake_polars/deltalake_polars_type_handler.py` & `dagster-deltalake-polars-0.23.3/dagster_deltalake_polars/deltalake_polars_type_handler.py`

 * *Files identical despite different names*

### Comparing `dagster-deltalake-polars-0.23.2rc4/dagster_deltalake_polars.egg-info/PKG-INFO` & `dagster-deltalake-polars-0.23.3/dagster_deltalake_polars.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-deltalake-polars
-Version: 0.23.2rc4
+Version: 0.23.3
 Summary: Package for storing Polars DataFrames in Delta tables.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-deltalake-polars
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-deltalake-polars-0.23.2rc4/setup.py` & `dagster-deltalake-polars-0.23.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,13 +33,13 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_deltalake_polars_tests*"]),
     include_package_data=True,
     python_requires=">=3.8,<3.13",
     install_requires=[
-        "dagster==1.7.2rc4",
-        "dagster-deltalake==0.23.2rc4",
+        "dagster==1.7.3",
+        "dagster-deltalake==0.23.3",
         "polars[pyarrow]",
     ],
     zip_safe=False,
 )
```

