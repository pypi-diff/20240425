# Comparing `tmp/limelightlib-python-0.9.1.tar.gz` & `tmp/limelightlib_python-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "limelightlib-python-0.9.1.tar", last modified: Fri Feb 16 16:57:19 2024, max compression
+gzip compressed data, was "limelightlib_python-0.9.3.tar", last modified: Wed Apr 24 22:02:58 2024, max compression
```

## Comparing `limelightlib-python-0.9.1.tar` & `limelightlib_python-0.9.3.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 16:57:19.239662 limelightlib-python-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-02-16 16:57:19.239662 limelightlib-python-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-02-16 16:57:15.000000 limelightlib-python-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 16:57:19.239662 limelightlib-python-0.9.1/limelightlib_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-02-16 16:57:19.000000 limelightlib-python-0.9.1/limelightlib_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-16 16:57:19.000000 limelightlib-python-0.9.1/limelightlib_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 16:57:19.000000 limelightlib-python-0.9.1/limelightlib_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-16 16:57:19.000000 limelightlib-python-0.9.1/limelightlib_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 16:57:19.000000 limelightlib-python-0.9.1/limelightlib_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-16 16:57:19.239662 limelightlib-python-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-02-16 16:57:15.000000 limelightlib-python-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:02:58.729390 limelightlib_python-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-24 22:02:58.729390 limelightlib_python-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-24 22:02:52.000000 limelightlib_python-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:02:58.729390 limelightlib_python-0.9.3/limelightlib-python/
+-rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-04-24 22:02:52.000000 limelightlib_python-0.9.3/limelightlib-python/limelight.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:02:58.729390 limelightlib_python-0.9.3/limelightlib-python/limelightlib_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-24 22:02:58.000000 limelightlib_python-0.9.3/limelightlib-python/limelightlib_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-24 22:02:58.000000 limelightlib_python-0.9.3/limelightlib-python/limelightlib_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 22:02:58.000000 limelightlib_python-0.9.3/limelightlib-python/limelightlib_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 22:02:58.000000 limelightlib_python-0.9.3/limelightlib-python/limelightlib_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-24 22:02:58.000000 limelightlib_python-0.9.3/limelightlib-python/limelightlib_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-24 22:02:52.000000 limelightlib_python-0.9.3/limelightlib-python/limelightresults.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 22:02:58.729390 limelightlib_python-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-24 22:02:53.000000 limelightlib_python-0.9.3/setup.py
```

### Comparing `limelightlib-python-0.9.1/README.md` & `limelightlib_python-0.9.3/README.md`

 * *Files identical despite different names*

