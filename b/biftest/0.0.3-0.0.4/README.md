# Comparing `tmp/biftest-0.0.3.tar.gz` & `tmp/biftest-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biftest-0.0.3.tar", last modified: Thu Apr 25 05:51:29 2024, max compression
+gzip compressed data, was "biftest-0.0.4.tar", last modified: Thu Apr 25 06:04:48 2024, max compression
```

## Comparing `biftest-0.0.3.tar` & `biftest-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 youngjin   (501) staff       (20)        0 2024-04-25 05:51:29.393361 biftest-0.0.3/
--rw-r--r--   0 youngjin   (501) staff       (20)      132 2024-04-25 05:51:29.393252 biftest-0.0.3/PKG-INFO
-drwxr-xr-x   0 youngjin   (501) staff       (20)        0 2024-04-25 05:51:29.392507 biftest-0.0.3/biftest/
--rw-r--r--   0 youngjin   (501) staff       (20)        0 2024-04-05 00:39:13.000000 biftest-0.0.3/biftest/__init__.py
--rw-r--r--   0 youngjin   (501) staff       (20)     2133 2024-04-25 05:49:59.000000 biftest-0.0.3/biftest/data_manager.py
--rw-r--r--   0 youngjin   (501) staff       (20)      747 2024-04-15 11:54:36.000000 biftest-0.0.3/biftest/hel.py
--rw-r--r--   0 youngjin   (501) staff       (20)     2315 2024-04-25 05:48:51.000000 biftest-0.0.3/biftest/request.py
-drwxr-xr-x   0 youngjin   (501) staff       (20)        0 2024-04-25 05:51:29.393103 biftest-0.0.3/biftest.egg-info/
--rw-r--r--   0 youngjin   (501) staff       (20)      132 2024-04-25 05:51:29.000000 biftest-0.0.3/biftest.egg-info/PKG-INFO
--rw-r--r--   0 youngjin   (501) staff       (20)      240 2024-04-25 05:51:29.000000 biftest-0.0.3/biftest.egg-info/SOURCES.txt
--rw-r--r--   0 youngjin   (501) staff       (20)        1 2024-04-25 05:51:29.000000 biftest-0.0.3/biftest.egg-info/dependency_links.txt
--rw-r--r--   0 youngjin   (501) staff       (20)       56 2024-04-25 05:51:29.000000 biftest-0.0.3/biftest.egg-info/requires.txt
--rw-r--r--   0 youngjin   (501) staff       (20)        8 2024-04-25 05:51:29.000000 biftest-0.0.3/biftest.egg-info/top_level.txt
--rw-r--r--   0 youngjin   (501) staff       (20)       38 2024-04-25 05:51:29.393406 biftest-0.0.3/setup.cfg
--rw-r--r--   0 youngjin   (501) staff       (20)      251 2024-04-25 05:51:12.000000 biftest-0.0.3/setup.py
+drwxr-xr-x   0 youngjin   (501) staff       (20)        0 2024-04-25 06:04:48.083923 biftest-0.0.4/
+-rw-r--r--   0 youngjin   (501) staff       (20)      132 2024-04-25 06:04:48.083804 biftest-0.0.4/PKG-INFO
+drwxr-xr-x   0 youngjin   (501) staff       (20)        0 2024-04-25 06:04:48.082954 biftest-0.0.4/biftest/
+-rw-r--r--   0 youngjin   (501) staff       (20)        0 2024-04-05 00:39:13.000000 biftest-0.0.4/biftest/__init__.py
+-rw-r--r--   0 youngjin   (501) staff       (20)     2133 2024-04-25 05:49:59.000000 biftest-0.0.4/biftest/data_manager.py
+-rw-r--r--   0 youngjin   (501) staff       (20)      747 2024-04-15 11:54:36.000000 biftest-0.0.4/biftest/hel.py
+-rw-r--r--   0 youngjin   (501) staff       (20)     2315 2024-04-25 05:48:51.000000 biftest-0.0.4/biftest/request.py
+drwxr-xr-x   0 youngjin   (501) staff       (20)        0 2024-04-25 06:04:48.083650 biftest-0.0.4/biftest.egg-info/
+-rw-r--r--   0 youngjin   (501) staff       (20)      132 2024-04-25 06:04:48.000000 biftest-0.0.4/biftest.egg-info/PKG-INFO
+-rw-r--r--   0 youngjin   (501) staff       (20)      240 2024-04-25 06:04:48.000000 biftest-0.0.4/biftest.egg-info/SOURCES.txt
+-rw-r--r--   0 youngjin   (501) staff       (20)        1 2024-04-25 06:04:48.000000 biftest-0.0.4/biftest.egg-info/dependency_links.txt
+-rw-r--r--   0 youngjin   (501) staff       (20)       51 2024-04-25 06:04:48.000000 biftest-0.0.4/biftest.egg-info/requires.txt
+-rw-r--r--   0 youngjin   (501) staff       (20)        8 2024-04-25 06:04:48.000000 biftest-0.0.4/biftest.egg-info/top_level.txt
+-rw-r--r--   0 youngjin   (501) staff       (20)       38 2024-04-25 06:04:48.083981 biftest-0.0.4/setup.cfg
+-rw-r--r--   0 youngjin   (501) staff       (20)      235 2024-04-25 06:04:44.000000 biftest-0.0.4/setup.py
```

### Comparing `biftest-0.0.3/biftest/data_manager.py` & `biftest-0.0.4/biftest/data_manager.py`

 * *Files identical despite different names*

### Comparing `biftest-0.0.3/biftest/hel.py` & `biftest-0.0.4/biftest/hel.py`

 * *Files identical despite different names*

### Comparing `biftest-0.0.3/biftest/request.py` & `biftest-0.0.4/biftest/request.py`

 * *Files identical despite different names*

