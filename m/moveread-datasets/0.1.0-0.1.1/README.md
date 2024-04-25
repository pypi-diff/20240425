# Comparing `tmp/moveread_datasets-0.1.0.tar.gz` & `tmp/moveread_datasets-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread_datasets-0.1.0.tar", last modified: Thu Apr 25 05:48:44 2024, max compression
+gzip compressed data, was "moveread_datasets-0.1.1.tar", last modified: Thu Apr 25 06:46:20 2024, max compression
```

## Comparing `moveread_datasets-0.1.0.tar` & `moveread_datasets-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 05:48:44.844240 moveread_datasets-0.1.0/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      471 2024-04-25 05:48:44.844240 moveread_datasets-0.1.0/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       33 2024-04-24 09:15:05.000000 moveread_datasets-0.1.0/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      528 2024-04-25 05:48:17.000000 moveread_datasets-0.1.0/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-25 05:48:44.844240 moveread_datasets-0.1.0/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 05:48:44.844240 moveread_datasets-0.1.0/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 05:48:44.844240 moveread_datasets-0.1.0/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 05:48:44.844240 moveread_datasets-0.1.0/src/moveread/datasets/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      104 2024-04-24 09:22:28.000000 moveread_datasets-0.1.0/src/moveread/datasets/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      653 2024-04-25 05:48:07.000000 moveread_datasets-0.1.0/src/moveread/datasets/main.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 05:48:44.844240 moveread_datasets-0.1.0/src/moveread_datasets.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      471 2024-04-25 05:48:44.000000 moveread_datasets-0.1.0/src/moveread_datasets.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      312 2024-04-25 05:48:44.000000 moveread_datasets-0.1.0/src/moveread_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-25 05:48:44.000000 moveread_datasets-0.1.0/src/moveread_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       43 2024-04-25 05:48:44.000000 moveread_datasets-0.1.0/src/moveread_datasets.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-04-25 05:48:44.000000 moveread_datasets-0.1.0/src/moveread_datasets.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:46:20.274238 moveread_datasets-0.1.1/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      471 2024-04-25 06:46:20.274238 moveread_datasets-0.1.1/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       33 2024-04-24 09:15:05.000000 moveread_datasets-0.1.1/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      528 2024-04-25 06:46:15.000000 moveread_datasets-0.1.1/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-25 06:46:20.274238 moveread_datasets-0.1.1/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:46:20.274238 moveread_datasets-0.1.1/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:46:20.274238 moveread_datasets-0.1.1/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:46:20.274238 moveread_datasets-0.1.1/src/moveread/datasets/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      112 2024-04-25 05:56:30.000000 moveread_datasets-0.1.1/src/moveread/datasets/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1116 2024-04-25 06:38:05.000000 moveread_datasets-0.1.1/src/moveread/datasets/main.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:46:20.274238 moveread_datasets-0.1.1/src/moveread_datasets.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      471 2024-04-25 06:46:20.000000 moveread_datasets-0.1.1/src/moveread_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      312 2024-04-25 06:46:20.000000 moveread_datasets-0.1.1/src/moveread_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-25 06:46:20.000000 moveread_datasets-0.1.1/src/moveread_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       43 2024-04-25 06:46:20.000000 moveread_datasets-0.1.1/src/moveread_datasets.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-04-25 06:46:20.000000 moveread_datasets-0.1.1/src/moveread_datasets.egg-info/top_level.txt
```

### Comparing `moveread_datasets-0.1.0/pyproject.toml` & `moveread_datasets-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-datasets"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Datasets storage API for Moveread"
 dependencies = [
   "kv-api", "kv-fs"
 ]
```

