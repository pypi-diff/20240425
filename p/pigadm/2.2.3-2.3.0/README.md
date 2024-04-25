# Comparing `tmp/pigadm-2.2.3.tar.gz` & `tmp/pigadm-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pigadm-2.2.3.tar", last modified: Wed Sep 20 09:30:35 2023, max compression
+gzip compressed data, was "pigadm-2.3.0.tar", last modified: Thu Apr 25 13:47:46 2024, max compression
```

## Comparing `pigadm-2.2.3.tar` & `pigadm-2.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-09-20 09:30:35.307817 pigadm-2.2.3/
--rw-r--r--   0 yrobin     (501) staff       (20)    35149 2023-05-10 12:23:42.000000 pigadm-2.2.3/LICENSE
--rw-r--r--   0 yrobin     (501) staff       (20)      509 2023-09-20 09:30:35.307624 pigadm-2.2.3/PKG-INFO
--rw-r--r--   0 yrobin     (501) staff       (20)      968 2023-09-20 05:56:24.000000 pigadm-2.2.3/README.md
-drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-09-20 09:30:35.307230 pigadm-2.2.3/pigadm.egg-info/
--rw-r--r--   0 yrobin     (501) staff       (20)      509 2023-09-20 09:30:35.000000 pigadm-2.2.3/pigadm.egg-info/PKG-INFO
--rw-r--r--   0 yrobin     (501) staff       (20)      566 2023-09-20 09:30:35.000000 pigadm-2.2.3/pigadm.egg-info/SOURCES.txt
--rw-r--r--   0 yrobin     (501) staff       (20)        1 2023-09-20 09:30:35.000000 pigadm-2.2.3/pigadm.egg-info/dependency_links.txt
--rw-r--r--   0 yrobin     (501) staff       (20)        7 2023-09-20 09:30:35.000000 pigadm-2.2.3/pigadm.egg-info/top_level.txt
-drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-09-20 09:30:35.307389 pigadm-2.2.3/scripts/
--rw-r--r--   0 yrobin     (501) staff       (20)      866 2023-05-10 12:39:54.000000 pigadm-2.2.3/scripts/pigadm
--rw-r--r--   0 yrobin     (501) staff       (20)       38 2023-09-20 09:30:35.307852 pigadm-2.2.3/setup.cfg
--rw-r--r--   0 yrobin     (501) staff       (20)     2248 2023-09-20 05:56:24.000000 pigadm-2.2.3/setup.py
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2024-04-25 13:47:46.187700 pigadm-2.3.0/
+-rw-r--r--   0 yrobin     (501) staff       (20)    35149 2023-05-10 12:23:42.000000 pigadm-2.3.0/LICENSE
+-rw-r--r--   0 yrobin     (501) staff       (20)      509 2024-04-25 13:47:46.187508 pigadm-2.3.0/PKG-INFO
+-rw-r--r--   0 yrobin     (501) staff       (20)      968 2023-09-20 05:56:24.000000 pigadm-2.3.0/README.md
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2024-04-25 13:47:46.187287 pigadm-2.3.0/pigadm.egg-info/
+-rw-r--r--   0 yrobin     (501) staff       (20)      509 2024-04-25 13:47:46.000000 pigadm-2.3.0/pigadm.egg-info/PKG-INFO
+-rw-r--r--   0 yrobin     (501) staff       (20)      566 2024-04-25 13:47:46.000000 pigadm-2.3.0/pigadm.egg-info/SOURCES.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)        1 2024-04-25 13:47:46.000000 pigadm-2.3.0/pigadm.egg-info/dependency_links.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)        7 2024-04-25 13:47:46.000000 pigadm-2.3.0/pigadm.egg-info/top_level.txt
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2024-04-25 13:47:46.186887 pigadm-2.3.0/scripts/
+-rw-r--r--   0 yrobin     (501) staff       (20)      866 2023-05-10 12:39:54.000000 pigadm-2.3.0/scripts/pigadm
+-rw-r--r--   0 yrobin     (501) staff       (20)       38 2024-04-25 13:47:46.187744 pigadm-2.3.0/setup.cfg
+-rw-r--r--   0 yrobin     (501) staff       (20)     2248 2023-09-20 05:56:24.000000 pigadm-2.3.0/setup.py
```

### Comparing `pigadm-2.2.3/LICENSE` & `pigadm-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pigadm-2.2.3/README.md` & `pigadm-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pigadm-2.2.3/pigadm.egg-info/SOURCES.txt` & `pigadm-2.3.0/pigadm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pigadm-2.2.3/scripts/pigadm` & `pigadm-2.3.0/scripts/pigadm`

 * *Files identical despite different names*

### Comparing `pigadm-2.2.3/setup.py` & `pigadm-2.3.0/setup.py`

 * *Files identical despite different names*

