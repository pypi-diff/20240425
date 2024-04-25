# Comparing `tmp/solafune-tools-0.1.8.tar.gz` & `tmp/solafune_tools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solafune-tools-0.1.8.tar", last modified: Sun Mar  3 18:04:59 2024, max compression
+gzip compressed data, was "solafune_tools-0.3.0.tar", last modified: Thu Apr 25 03:05:19 2024, max compression
```

## Comparing `solafune-tools-0.1.8.tar` & `solafune_tools-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 18:04:59.452615 solafune-tools-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-03-03 18:04:59.452615 solafune-tools-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-03-03 18:04:49.000000 solafune-tools-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-03-03 18:04:49.000000 solafune-tools-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-03 18:04:49.000000 solafune-tools-0.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-03 18:04:59.452615 solafune-tools-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 18:04:59.452615 solafune-tools-0.1.8/solafune_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-03 18:04:49.000000 solafune-tools-0.1.8/solafune_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-03-03 18:04:49.000000 solafune-tools-0.1.8/solafune_tools/image_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-03 18:04:49.000000 solafune-tools-0.1.8/solafune_tools/junk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-03-03 18:04:49.000000 solafune-tools-0.1.8/solafune_tools/make_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-03-03 18:04:49.000000 solafune-tools-0.1.8/solafune_tools/make_mosaic.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-03-03 18:04:49.000000 solafune-tools-0.1.8/solafune_tools/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 18:04:59.452615 solafune-tools-0.1.8/solafune_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-03-03 18:04:59.000000 solafune-tools-0.1.8/solafune_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-03 18:04:59.000000 solafune-tools-0.1.8/solafune_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-03 18:04:59.000000 solafune-tools-0.1.8/solafune_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-03 18:04:59.000000 solafune-tools-0.1.8/solafune_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-03 18:04:59.000000 solafune-tools-0.1.8/solafune_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 18:04:59.452615 solafune-tools-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-03 18:04:49.000000 solafune-tools-0.1.8/tests/test_get_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-03 18:04:49.000000 solafune-tools-0.1.8/tests/test_image_fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:05:19.874372 solafune_tools-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-25 03:05:15.000000 solafune_tools-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-04-25 03:05:19.874372 solafune_tools-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-04-25 03:05:15.000000 solafune_tools-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-25 03:05:15.000000 solafune_tools-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-25 03:05:15.000000 solafune_tools-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 03:05:19.874372 solafune_tools-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:05:19.874372 solafune_tools-0.3.0/solafune_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-25 03:05:15.000000 solafune_tools-0.3.0/solafune_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7630 2024-04-25 03:05:15.000000 solafune_tools-0.3.0/solafune_tools/image_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-25 03:05:15.000000 solafune_tools-0.3.0/solafune_tools/junk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-04-25 03:05:15.000000 solafune_tools-0.3.0/solafune_tools/make_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8074 2024-04-25 03:05:15.000000 solafune_tools-0.3.0/solafune_tools/make_mosaic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-25 03:05:15.000000 solafune_tools-0.3.0/solafune_tools/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-25 03:05:15.000000 solafune_tools-0.3.0/solafune_tools/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:05:19.874372 solafune_tools-0.3.0/solafune_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-04-25 03:05:19.000000 solafune_tools-0.3.0/solafune_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-25 03:05:19.000000 solafune_tools-0.3.0/solafune_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 03:05:19.000000 solafune_tools-0.3.0/solafune_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-25 03:05:19.000000 solafune_tools-0.3.0/solafune_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-25 03:05:19.000000 solafune_tools-0.3.0/solafune_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:05:19.874372 solafune_tools-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 03:05:15.000000 solafune_tools-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-25 03:05:15.000000 solafune_tools-0.3.0/tests/mock_get_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-25 03:05:15.000000 solafune_tools-0.3.0/tests/test_make_mosaic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-25 03:05:15.000000 solafune_tools-0.3.0/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-25 03:05:15.000000 solafune_tools-0.3.0/tests/test_write_catalog.py
```

### Comparing `solafune-tools-0.1.8/solafune_tools/settings.py` & `solafune_tools-0.3.0/solafune_tools/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import os
 
 
 def set_data_directory(dir_path=os.path.join(os.getcwd(), "data/")):
     """
-    Sets the data directory as an environment variable and creates 
+    Sets the data directory as an environment variable and creates
     various subdirectories used by this package.
     """
     dir_path = os.path.abspath(dir_path)
     if not os.path.isdir(dir_path):
         os.mkdir(dir_path)
-        for each in ["stac", "geojson", "tif", "parquet", "logs"]:
+        for each in ["stac", "geojson", "tif", "parquet", "logs", "mosaic"]:
             os.mkdir(os.path.join(dir_path, each))
     os.environ["solafune_tools_data_dir"] = dir_path
     assert os.environ.get("solafune_tools_data_dir") == dir_path
     return None
 
 
 def get_data_directory():
-    """ Gets the data directory from the environment variable """
+    """Gets the data directory from the environment variable"""
     if os.getenv("solafune_tools_data_dir") is None:
         set_data_directory()
     return os.getenv("solafune_tools_data_dir")
```

