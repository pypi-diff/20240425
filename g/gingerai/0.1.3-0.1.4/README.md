# Comparing `tmp/gingerai-0.1.3.tar.gz` & `tmp/gingerai-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gingerai-0.1.3.tar", last modified: Thu Apr 25 13:35:26 2024, max compression
+gzip compressed data, was "gingerai-0.1.4.tar", last modified: Thu Apr 25 13:38:23 2024, max compression
```

## Comparing `gingerai-0.1.3.tar` & `gingerai-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 tomjurien  (1000) tomjurien  (1000)        0 2024-04-25 13:35:26.086300 gingerai-0.1.3/
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)      340 2024-04-25 13:35:26.076300 gingerai-0.1.3/PKG-INFO
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)        0 2024-04-25 13:35:25.000000 gingerai-0.1.3/README.md
-drwxr-xr-x   0 tomjurien  (1000) tomjurien  (1000)        0 2024-04-25 13:35:26.076300 gingerai-0.1.3/gingerai/
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)     1291 2024-04-25 13:35:03.000000 gingerai-0.1.3/gingerai/TorchNetWrapper.py
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)       69 2024-04-25 13:35:25.000000 gingerai-0.1.3/gingerai/__init__.py
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)     1291 2024-04-25 13:35:25.000000 gingerai-0.1.3/gingerai/torch.py
-drwxr-xr-x   0 tomjurien  (1000) tomjurien  (1000)        0 2024-04-25 13:35:26.076300 gingerai-0.1.3/gingerai.egg-info/
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)      340 2024-04-25 13:35:26.000000 gingerai-0.1.3/gingerai.egg-info/PKG-INFO
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)      244 2024-04-25 13:35:26.000000 gingerai-0.1.3/gingerai.egg-info/SOURCES.txt
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)        1 2024-04-25 13:35:26.000000 gingerai-0.1.3/gingerai.egg-info/dependency_links.txt
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)        6 2024-04-25 13:35:26.000000 gingerai-0.1.3/gingerai.egg-info/requires.txt
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)        9 2024-04-25 13:35:26.000000 gingerai-0.1.3/gingerai.egg-info/top_level.txt
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)       38 2024-04-25 13:35:26.086300 gingerai-0.1.3/setup.cfg
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)      439 2024-04-25 13:35:25.000000 gingerai-0.1.3/setup.py
+drwxr-xr-x   0 tomjurien  (1000) tomjurien  (1000)        0 2024-04-25 13:38:23.826394 gingerai-0.1.4/
+-rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)      340 2024-04-25 13:38:23.826394 gingerai-0.1.4/PKG-INFO
+-rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)        0 2024-04-25 13:38:23.000000 gingerai-0.1.4/README.md
+drwxr-xr-x   0 tomjurien  (1000) tomjurien  (1000)        0 2024-04-25 13:38:23.826394 gingerai-0.1.4/gingerai/
+-rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)     1291 2024-04-25 13:38:23.000000 gingerai-0.1.4/gingerai/TorchNetWrapper.py
+-rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)       72 2024-04-25 13:38:23.000000 gingerai-0.1.4/gingerai/__init__.py
+drwxr-xr-x   0 tomjurien  (1000) tomjurien  (1000)        0 2024-04-25 13:38:23.826394 gingerai-0.1.4/gingerai.egg-info/
+-rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)      340 2024-04-25 13:38:23.000000 gingerai-0.1.4/gingerai.egg-info/PKG-INFO
+-rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)      226 2024-04-25 13:38:23.000000 gingerai-0.1.4/gingerai.egg-info/SOURCES.txt
+-rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)        1 2024-04-25 13:38:23.000000 gingerai-0.1.4/gingerai.egg-info/dependency_links.txt
+-rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)        6 2024-04-25 13:38:23.000000 gingerai-0.1.4/gingerai.egg-info/requires.txt
+-rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)        9 2024-04-25 13:38:23.000000 gingerai-0.1.4/gingerai.egg-info/top_level.txt
+-rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)       38 2024-04-25 13:38:23.826394 gingerai-0.1.4/setup.cfg
+-rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)      439 2024-04-25 13:38:23.000000 gingerai-0.1.4/setup.py
```

### Comparing `gingerai-0.1.3/gingerai/TorchNetWrapper.py` & `gingerai-0.1.4/gingerai/TorchNetWrapper.py`

 * *Files identical despite different names*
