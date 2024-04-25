# Comparing `tmp/biftest-0.0.2.tar.gz` & `tmp/biftest-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biftest-0.0.2.tar", last modified: Mon Apr 15 11:56:19 2024, max compression
+gzip compressed data, was "biftest-0.0.3.tar", last modified: Thu Apr 25 05:51:29 2024, max compression
```

## Comparing `biftest-0.0.2.tar` & `biftest-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 youngjin   (501) staff       (20)        0 2024-04-15 11:56:19.461657 biftest-0.0.2/
--rw-r--r--   0 youngjin   (501) staff       (20)      132 2024-04-15 11:56:19.461501 biftest-0.0.2/PKG-INFO
-drwxr-xr-x   0 youngjin   (501) staff       (20)        0 2024-04-15 11:56:19.460695 biftest-0.0.2/biftest/
--rw-r--r--   0 youngjin   (501) staff       (20)        0 2024-04-05 00:39:13.000000 biftest-0.0.2/biftest/__init__.py
--rw-r--r--   0 youngjin   (501) staff       (20)      747 2024-04-15 11:54:36.000000 biftest-0.0.2/biftest/hel.py
-drwxr-xr-x   0 youngjin   (501) staff       (20)        0 2024-04-15 11:56:19.461312 biftest-0.0.2/biftest.egg-info/
--rw-r--r--   0 youngjin   (501) staff       (20)      132 2024-04-15 11:56:19.000000 biftest-0.0.2/biftest.egg-info/PKG-INFO
--rw-r--r--   0 youngjin   (501) staff       (20)      197 2024-04-15 11:56:19.000000 biftest-0.0.2/biftest.egg-info/SOURCES.txt
--rw-r--r--   0 youngjin   (501) staff       (20)        1 2024-04-15 11:56:19.000000 biftest-0.0.2/biftest.egg-info/dependency_links.txt
--rw-r--r--   0 youngjin   (501) staff       (20)       42 2024-04-15 11:56:19.000000 biftest-0.0.2/biftest.egg-info/requires.txt
--rw-r--r--   0 youngjin   (501) staff       (20)        8 2024-04-15 11:56:19.000000 biftest-0.0.2/biftest.egg-info/top_level.txt
--rw-r--r--   0 youngjin   (501) staff       (20)       38 2024-04-15 11:56:19.461713 biftest-0.0.2/setup.cfg
--rw-r--r--   0 youngjin   (501) staff       (20)      215 2024-04-15 11:55:36.000000 biftest-0.0.2/setup.py
+drwxr-xr-x   0 youngjin   (501) staff       (20)        0 2024-04-25 05:51:29.393361 biftest-0.0.3/
+-rw-r--r--   0 youngjin   (501) staff       (20)      132 2024-04-25 05:51:29.393252 biftest-0.0.3/PKG-INFO
+drwxr-xr-x   0 youngjin   (501) staff       (20)        0 2024-04-25 05:51:29.392507 biftest-0.0.3/biftest/
+-rw-r--r--   0 youngjin   (501) staff       (20)        0 2024-04-05 00:39:13.000000 biftest-0.0.3/biftest/__init__.py
+-rw-r--r--   0 youngjin   (501) staff       (20)     2133 2024-04-25 05:49:59.000000 biftest-0.0.3/biftest/data_manager.py
+-rw-r--r--   0 youngjin   (501) staff       (20)      747 2024-04-15 11:54:36.000000 biftest-0.0.3/biftest/hel.py
+-rw-r--r--   0 youngjin   (501) staff       (20)     2315 2024-04-25 05:48:51.000000 biftest-0.0.3/biftest/request.py
+drwxr-xr-x   0 youngjin   (501) staff       (20)        0 2024-04-25 05:51:29.393103 biftest-0.0.3/biftest.egg-info/
+-rw-r--r--   0 youngjin   (501) staff       (20)      132 2024-04-25 05:51:29.000000 biftest-0.0.3/biftest.egg-info/PKG-INFO
+-rw-r--r--   0 youngjin   (501) staff       (20)      240 2024-04-25 05:51:29.000000 biftest-0.0.3/biftest.egg-info/SOURCES.txt
+-rw-r--r--   0 youngjin   (501) staff       (20)        1 2024-04-25 05:51:29.000000 biftest-0.0.3/biftest.egg-info/dependency_links.txt
+-rw-r--r--   0 youngjin   (501) staff       (20)       56 2024-04-25 05:51:29.000000 biftest-0.0.3/biftest.egg-info/requires.txt
+-rw-r--r--   0 youngjin   (501) staff       (20)        8 2024-04-25 05:51:29.000000 biftest-0.0.3/biftest.egg-info/top_level.txt
+-rw-r--r--   0 youngjin   (501) staff       (20)       38 2024-04-25 05:51:29.393406 biftest-0.0.3/setup.cfg
+-rw-r--r--   0 youngjin   (501) staff       (20)      251 2024-04-25 05:51:12.000000 biftest-0.0.3/setup.py
```

### Comparing `biftest-0.0.2/biftest/hel.py` & `biftest-0.0.3/biftest/hel.py`

 * *Files identical despite different names*

