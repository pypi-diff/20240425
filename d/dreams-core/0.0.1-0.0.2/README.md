# Comparing `tmp/dreams_core-0.0.1.tar.gz` & `tmp/dreams_core-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreams_core-0.0.1.tar", last modified: Wed Apr 24 21:54:37 2024, max compression
+gzip compressed data, was "dreams_core-0.0.2.tar", last modified: Wed Apr 24 22:12:57 2024, max compression
```

## Comparing `dreams_core-0.0.1.tar` & `dreams_core-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-04-24 21:54:37.987853 dreams_core-0.0.1/
--rw-r--r--   0 jeremy     (502) staff       (20)     1126 2024-04-24 21:32:45.000000 dreams_core-0.0.1/LICENSE
--rw-r--r--   0 jeremy     (502) staff       (20)      144 2024-04-24 21:54:22.000000 dreams_core-0.0.1/MANIFEST.in
--rw-r--r--   0 jeremy     (502) staff       (20)     1040 2024-04-24 21:54:37.987599 dreams_core-0.0.1/PKG-INFO
--rw-r--r--   0 jeremy     (502) staff       (20)      170 2024-04-24 21:32:45.000000 dreams_core-0.0.1/README.md
--rw-r--r--   0 jeremy     (502) staff       (20)      884 2024-04-24 21:54:35.000000 dreams_core-0.0.1/pyproject.toml
--rw-r--r--   0 jeremy     (502) staff       (20)       38 2024-04-24 21:54:37.987893 dreams_core-0.0.1/setup.cfg
-drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-04-24 21:54:37.984384 dreams_core-0.0.1/src/
-drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-04-24 21:54:37.986441 dreams_core-0.0.1/src/dreams_core/
--rw-r--r--   0 jeremy     (502) staff       (20)     4101 2024-04-24 21:14:06.000000 dreams_core-0.0.1/src/dreams_core/BigQuery.py
--rw-r--r--   0 jeremy     (502) staff       (20)       49 2024-04-17 19:02:52.000000 dreams_core-0.0.1/src/dreams_core/__init__.py
--rw-r--r--   0 jeremy     (502) staff       (20)     6469 2024-04-24 21:15:38.000000 dreams_core-0.0.1/src/dreams_core/dreams_core.py
-drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-04-24 21:54:37.987334 dreams_core-0.0.1/src/dreams_core.egg-info/
--rw-r--r--   0 jeremy     (502) staff       (20)     1040 2024-04-24 21:54:37.000000 dreams_core-0.0.1/src/dreams_core.egg-info/PKG-INFO
--rw-r--r--   0 jeremy     (502) staff       (20)      325 2024-04-24 21:54:37.000000 dreams_core-0.0.1/src/dreams_core.egg-info/SOURCES.txt
--rw-r--r--   0 jeremy     (502) staff       (20)        1 2024-04-24 21:54:37.000000 dreams_core-0.0.1/src/dreams_core.egg-info/dependency_links.txt
--rw-r--r--   0 jeremy     (502) staff       (20)      159 2024-04-24 21:54:37.000000 dreams_core-0.0.1/src/dreams_core.egg-info/requires.txt
--rw-r--r--   0 jeremy     (502) staff       (20)       12 2024-04-24 21:54:37.000000 dreams_core-0.0.1/src/dreams_core.egg-info/top_level.txt
+drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-04-24 22:12:57.417262 dreams_core-0.0.2/
+-rw-r--r--   0 jeremy     (502) staff       (20)     1126 2024-04-24 21:32:45.000000 dreams_core-0.0.2/LICENSE
+-rw-r--r--   0 jeremy     (502) staff       (20)      178 2024-04-24 21:59:31.000000 dreams_core-0.0.2/MANIFEST.in
+-rw-r--r--   0 jeremy     (502) staff       (20)     1187 2024-04-24 22:12:57.417045 dreams_core-0.0.2/PKG-INFO
+-rw-r--r--   0 jeremy     (502) staff       (20)      317 2024-04-24 22:09:04.000000 dreams_core-0.0.2/README.md
+-rw-r--r--   0 jeremy     (502) staff       (20)      884 2024-04-24 22:10:41.000000 dreams_core-0.0.2/pyproject.toml
+-rw-r--r--   0 jeremy     (502) staff       (20)       38 2024-04-24 22:12:57.417300 dreams_core-0.0.2/setup.cfg
+drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-04-24 22:12:57.414596 dreams_core-0.0.2/src/
+drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-04-24 22:12:57.416082 dreams_core-0.0.2/src/dreams_core/
+-rw-r--r--   0 jeremy     (502) staff       (20)     4101 2024-04-24 21:14:06.000000 dreams_core-0.0.2/src/dreams_core/BigQuery.py
+-rw-r--r--   0 jeremy     (502) staff       (20)     3527 2024-04-24 22:09:36.000000 dreams_core-0.0.2/src/dreams_core/Dune.py
+-rw-r--r--   0 jeremy     (502) staff       (20)       49 2024-04-17 19:02:52.000000 dreams_core-0.0.2/src/dreams_core/__init__.py
+-rw-r--r--   0 jeremy     (502) staff       (20)     3024 2024-04-24 22:09:47.000000 dreams_core-0.0.2/src/dreams_core/dreams_core.py
+drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-04-24 22:12:57.416810 dreams_core-0.0.2/src/dreams_core.egg-info/
+-rw-r--r--   0 jeremy     (502) staff       (20)     1187 2024-04-24 22:12:57.000000 dreams_core-0.0.2/src/dreams_core.egg-info/PKG-INFO
+-rw-r--r--   0 jeremy     (502) staff       (20)      349 2024-04-24 22:12:57.000000 dreams_core-0.0.2/src/dreams_core.egg-info/SOURCES.txt
+-rw-r--r--   0 jeremy     (502) staff       (20)        1 2024-04-24 22:12:57.000000 dreams_core-0.0.2/src/dreams_core.egg-info/dependency_links.txt
+-rw-r--r--   0 jeremy     (502) staff       (20)      159 2024-04-24 22:12:57.000000 dreams_core-0.0.2/src/dreams_core.egg-info/requires.txt
+-rw-r--r--   0 jeremy     (502) staff       (20)       12 2024-04-24 22:12:57.000000 dreams_core-0.0.2/src/dreams_core.egg-info/top_level.txt
```

### Comparing `dreams_core-0.0.1/LICENSE` & `dreams_core-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dreams_core-0.0.1/PKG-INFO` & `dreams_core-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreams_core
-Version: 0.0.1
+Version: 0.0.2
 Summary: brought to you by the dreamslabs discord community
 Author-email: tentabs <tentabs00@gmail.com>
 Project-URL: Community, https://discord.gg/dreamcrypto
 Project-URL: Github, https://github.com/dreams-labs/core-functions
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -17,12 +17,13 @@
 Requires-Dist: pandas>=1.2.0
 Requires-Dist: numpy>=1.19.5
 Requires-Dist: google-auth>=1.24.0
 Requires-Dist: google-cloud-secret-manager>=2.3.0
 Requires-Dist: google-cloud-bigquery>=2.13.1
 Requires-Dist: google-cloud-storage>=1.37.1
 
-# Example Package
+# Dreams Labs Core Python Functions
 
-This is a simple example package. You can use
-[GitHub-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
-to write your content.
+these are split into multile subfiles based on use case:
+* dreams_core includes standard functions that should be useful across many use cases, such as help with formatting and importing secrets
+* BigQuery is functions related to bigquery
+* Dune includes functions related to dune
```

### Comparing `dreams_core-0.0.1/pyproject.toml` & `dreams_core-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dreams_core"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="tentabs", email="tentabs00@gmail.com" },
 ]
 description = "brought to you by the dreamslabs discord community"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [
```

### Comparing `dreams_core-0.0.1/src/dreams_core/BigQuery.py` & `dreams_core-0.0.2/src/dreams_core/BigQuery.py`

 * *Files identical despite different names*

### Comparing `dreams_core-0.0.1/src/dreams_core.egg-info/PKG-INFO` & `dreams_core-0.0.2/src/dreams_core.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreams_core
-Version: 0.0.1
+Version: 0.0.2
 Summary: brought to you by the dreamslabs discord community
 Author-email: tentabs <tentabs00@gmail.com>
 Project-URL: Community, https://discord.gg/dreamcrypto
 Project-URL: Github, https://github.com/dreams-labs/core-functions
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -17,12 +17,13 @@
 Requires-Dist: pandas>=1.2.0
 Requires-Dist: numpy>=1.19.5
 Requires-Dist: google-auth>=1.24.0
 Requires-Dist: google-cloud-secret-manager>=2.3.0
 Requires-Dist: google-cloud-bigquery>=2.13.1
 Requires-Dist: google-cloud-storage>=1.37.1
 
-# Example Package
+# Dreams Labs Core Python Functions
 
-This is a simple example package. You can use
-[GitHub-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
-to write your content.
+these are split into multile subfiles based on use case:
+* dreams_core includes standard functions that should be useful across many use cases, such as help with formatting and importing secrets
+* BigQuery is functions related to bigquery
+* Dune includes functions related to dune
```

