# Comparing `tmp/tf_tools-0.1.2.tar.gz` & `tmp/tf_tools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tf_tools-0.1.2.tar", last modified: Mon Apr 22 10:25:19 2024, max compression
+gzip compressed data, was "tf_tools-0.1.3.tar", last modified: Thu Apr 25 14:34:06 2024, max compression
```

## Comparing `tf_tools-0.1.2.tar` & `tf_tools-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:25:19.096985 tf_tools-0.1.2/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      283 2024-04-22 10:25:19.096985 tf_tools-0.1.2/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      456 2024-04-22 10:25:16.000000 tf_tools-0.1.2/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-22 10:25:19.096985 tf_tools-0.1.2/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:25:19.096985 tf_tools-0.1.2/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:25:19.096985 tf_tools-0.1.2/src/tf_tools/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      118 2024-03-14 14:58:08.000000 tf_tools-0.1.2/src/tf_tools/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      712 2024-03-14 08:46:06.000000 tf_tools-0.1.2/src/tf_tools/pad.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      336 2024-03-14 08:46:00.000000 tf_tools-0.1.2/src/tf_tools/set.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:25:19.096985 tf_tools-0.1.2/src/tf_tools/sparse/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       36 2024-03-14 07:19:40.000000 tf_tools-0.1.2/src/tf_tools/sparse/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      934 2024-03-14 08:45:39.000000 tf_tools-0.1.2/src/tf_tools/sparse/sparse.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      426 2024-03-15 06:35:00.000000 tf_tools-0.1.2/src/tf_tools/typing.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:25:19.096985 tf_tools-0.1.2/src/tf_tools.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      283 2024-04-22 10:25:19.000000 tf_tools-0.1.2/src/tf_tools.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      343 2024-04-22 10:25:19.000000 tf_tools-0.1.2/src/tf_tools.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-22 10:25:19.000000 tf_tools-0.1.2/src/tf_tools.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       21 2024-04-22 10:25:19.000000 tf_tools-0.1.2/src/tf_tools.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-04-22 10:25:19.000000 tf_tools-0.1.2/src/tf_tools.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 14:34:06.129446 tf_tools-0.1.3/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      331 2024-04-25 14:34:06.129446 tf_tools-0.1.3/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      480 2024-04-25 14:34:03.000000 tf_tools-0.1.3/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-25 14:34:06.129446 tf_tools-0.1.3/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 14:34:06.119444 tf_tools-0.1.3/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 14:34:06.129446 tf_tools-0.1.3/src/tf_tools/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-25 10:13:29.000000 tf_tools-0.1.3/src/tf_tools/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      192 2024-04-25 10:14:33.000000 tf_tools-0.1.3/src/tf_tools/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      712 2024-03-14 08:46:06.000000 tf_tools-0.1.3/src/tf_tools/pad.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      336 2024-03-14 08:46:00.000000 tf_tools-0.1.3/src/tf_tools/set.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 14:34:06.129446 tf_tools-0.1.3/src/tf_tools/sparse/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       36 2024-03-14 07:19:40.000000 tf_tools-0.1.3/src/tf_tools/sparse/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      934 2024-03-14 08:45:39.000000 tf_tools-0.1.3/src/tf_tools/sparse/sparse.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      426 2024-03-15 06:35:00.000000 tf_tools-0.1.3/src/tf_tools/typing.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 14:34:06.129446 tf_tools-0.1.3/src/tf_tools.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      331 2024-04-25 14:34:06.000000 tf_tools-0.1.3/src/tf_tools.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      369 2024-04-25 14:34:06.000000 tf_tools-0.1.3/src/tf_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-25 14:34:06.000000 tf_tools-0.1.3/src/tf_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       39 2024-04-25 14:34:06.000000 tf_tools-0.1.3/src/tf_tools.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-04-25 14:34:06.000000 tf_tools-0.1.3/src/tf_tools.egg-info/top_level.txt
```

### Comparing `tf_tools-0.1.2/src/tf_tools/pad.py` & `tf_tools-0.1.3/src/tf_tools/pad.py`

 * *Files identical despite different names*

### Comparing `tf_tools-0.1.2/src/tf_tools/sparse/sparse.py` & `tf_tools-0.1.3/src/tf_tools/sparse/sparse.py`

 * *Files identical despite different names*

