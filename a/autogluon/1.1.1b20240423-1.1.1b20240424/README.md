# Comparing `tmp/autogluon-1.1.1b20240423.tar.gz` & `tmp/autogluon-1.1.1b20240424.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon-1.1.1b20240423.tar", last modified: Tue Apr 23 09:05:42 2024, max compression
+gzip compressed data, was "autogluon-1.1.1b20240424.tar", last modified: Wed Apr 24 09:05:30 2024, max compression
```

## Comparing `autogluon-1.1.1b20240423.tar` & `autogluon-1.1.1b20240424.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:05:42.405142 autogluon-1.1.1b20240423/
--rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-04-23 09:05:42.405142 autogluon-1.1.1b20240423/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 09:05:42.405142 autogluon-1.1.1b20240423/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-23 09:03:56.000000 autogluon-1.1.1b20240423/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:05:42.405142 autogluon-1.1.1b20240423/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:05:42.405142 autogluon-1.1.1b20240423/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:05:42.405142 autogluon-1.1.1b20240423/src/autogluon/_internal_/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 09:03:56.000000 autogluon-1.1.1b20240423/src/autogluon/_internal_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:05:42.405142 autogluon-1.1.1b20240423/src/autogluon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-04-23 09:05:42.000000 autogluon-1.1.1b20240423/src/autogluon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-23 09:05:42.000000 autogluon-1.1.1b20240423/src/autogluon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 09:05:42.000000 autogluon-1.1.1b20240423/src/autogluon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 09:05:42.000000 autogluon-1.1.1b20240423/src/autogluon.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-23 09:05:42.000000 autogluon-1.1.1b20240423/src/autogluon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 09:05:42.000000 autogluon-1.1.1b20240423/src/autogluon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 09:05:42.000000 autogluon-1.1.1b20240423/src/autogluon.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:05:30.706704 autogluon-1.1.1b20240424/
+-rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-04-24 09:05:30.706704 autogluon-1.1.1b20240424/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 09:05:30.706704 autogluon-1.1.1b20240424/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-24 09:03:44.000000 autogluon-1.1.1b20240424/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:05:30.702704 autogluon-1.1.1b20240424/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:05:30.702704 autogluon-1.1.1b20240424/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:05:30.702704 autogluon-1.1.1b20240424/src/autogluon/_internal_/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 09:03:44.000000 autogluon-1.1.1b20240424/src/autogluon/_internal_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:05:30.702704 autogluon-1.1.1b20240424/src/autogluon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-04-24 09:05:30.000000 autogluon-1.1.1b20240424/src/autogluon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-24 09:05:30.000000 autogluon-1.1.1b20240424/src/autogluon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 09:05:30.000000 autogluon-1.1.1b20240424/src/autogluon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-24 09:05:30.000000 autogluon-1.1.1b20240424/src/autogluon.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-24 09:05:30.000000 autogluon-1.1.1b20240424/src/autogluon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-24 09:05:30.000000 autogluon-1.1.1b20240424/src/autogluon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 09:05:30.000000 autogluon-1.1.1b20240424/src/autogluon.egg-info/zip-safe
```

### Comparing `autogluon-1.1.1b20240423/PKG-INFO` & `autogluon-1.1.1b20240424/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 1.1.1b20240423
+Version: 1.1.1b20240424
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon-1.1.1b20240423/setup.py` & `autogluon-1.1.1b20240424/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon-1.1.1b20240423/src/autogluon.egg-info/PKG-INFO` & `autogluon-1.1.1b20240424/src/autogluon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 1.1.1b20240423
+Version: 1.1.1b20240424
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

