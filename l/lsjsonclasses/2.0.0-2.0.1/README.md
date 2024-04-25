# Comparing `tmp/lsjsonclasses-2.0.0.tar.gz` & `tmp/lsjsonclasses-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsjsonclasses-2.0.0.tar", max compression
+gzip compressed data, was "lsjsonclasses-2.0.1.tar", max compression
```

## Comparing `lsjsonclasses-2.0.0.tar` & `lsjsonclasses-2.0.1.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0     1227 2023-07-25 13:46:20.436557 lsjsonclasses-2.0.0/lsjsonclasses/__init__.py
--rw-r--r--   0        0        0      408 2023-10-12 12:59:30.938863 lsjsonclasses-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      326 1970-01-01 00:00:00.000000 lsjsonclasses-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1227 2023-07-25 13:46:20.436557 lsjsonclasses-2.0.1/lsjsonclasses/__init__.py
+-rw-r--r--   0        0        0      407 2024-04-25 07:57:30.145952 lsjsonclasses-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0      426 1970-01-01 00:00:00.000000 lsjsonclasses-2.0.1/PKG-INFO
```

### Comparing `lsjsonclasses-2.0.0/lsjsonclasses/__init__.py` & `lsjsonclasses-2.0.1/lsjsonclasses/__init__.py`

 * *Files identical despite different names*

