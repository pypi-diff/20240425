# Comparing `tmp/redvert-1.0.1.tar.gz` & `tmp/redvert-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redvert-1.0.1.tar", last modified: Thu Apr 25 20:47:04 2024, max compression
+gzip compressed data, was "redvert-1.0.2.tar", last modified: Thu Apr 25 20:57:09 2024, max compression
```

## Comparing `redvert-1.0.1.tar` & `redvert-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 20:47:04.739463 redvert-1.0.1/
--rw-rw-rw-   0        0        0      447 2024-04-25 20:47:04.739463 redvert-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-25 20:47:04.739463 redvert-1.0.1/RedVert.egg-info/
--rw-rw-rw-   0        0        0      447 2024-04-25 20:47:04.000000 redvert-1.0.1/RedVert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2024-04-25 20:47:04.000000 redvert-1.0.1/RedVert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 20:47:04.000000 redvert-1.0.1/RedVert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-04-25 20:47:04.000000 redvert-1.0.1/RedVert.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2024-04-25 20:47:04.000000 redvert-1.0.1/RedVert.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-25 20:47:04.735981 redvert-1.0.1/redvert/
--rw-rw-rw-   0        0        0       19 2024-04-24 21:45:28.000000 redvert-1.0.1/redvert/__init__.py
--rw-rw-rw-   0        0        0     7379 2024-04-24 22:41:17.000000 redvert-1.0.1/redvert/main.py
--rw-rw-rw-   0        0        0       42 2024-04-25 20:47:04.739463 redvert-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      466 2024-04-25 20:46:53.000000 redvert-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 20:57:09.116911 redvert-1.0.2/
+-rw-rw-rw-   0        0        0     1308 2024-04-25 20:57:09.116911 redvert-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-25 20:57:09.116911 redvert-1.0.2/RedVert.egg-info/
+-rw-rw-rw-   0        0        0     1308 2024-04-25 20:57:08.000000 redvert-1.0.2/RedVert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2024-04-25 20:57:08.000000 redvert-1.0.2/RedVert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 20:57:08.000000 redvert-1.0.2/RedVert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-25 20:57:08.000000 redvert-1.0.2/RedVert.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2024-04-25 20:57:08.000000 redvert-1.0.2/RedVert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 20:57:09.113113 redvert-1.0.2/redvert/
+-rw-rw-rw-   0        0        0       19 2024-04-24 21:45:28.000000 redvert-1.0.2/redvert/__init__.py
+-rw-rw-rw-   0        0        0     7379 2024-04-24 22:41:17.000000 redvert-1.0.2/redvert/main.py
+-rw-rw-rw-   0        0        0       42 2024-04-25 20:57:09.116911 redvert-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      466 2024-04-25 20:50:13.000000 redvert-1.0.2/setup.py
```

### Comparing `redvert-1.0.1/redvert/main.py` & `redvert-1.0.2/redvert/main.py`

 * *Files identical despite different names*

