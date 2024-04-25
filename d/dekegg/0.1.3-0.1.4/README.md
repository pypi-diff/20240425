# Comparing `tmp/dekegg-0.1.3.tar.gz` & `tmp/dekegg-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dekegg-0.1.3.tar", last modified: Mon Feb 19 14:52:47 2024, max compression
+gzip compressed data, was "dekegg-0.1.4.tar", last modified: Thu Apr 25 19:15:27 2024, max compression
```

## Comparing `dekegg-0.1.3.tar` & `dekegg-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        9 2024-02-19 14:52:46.339669 dekegg-0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-02-19 14:52:46.343669 dekegg-0.1.3/dekegg/__init__.py
--rw-r--r--   0        0        0     2337 2024-02-19 14:52:46.343669 dekegg-0.1.3/dekegg/bdist.py
--rw-r--r--   0        0        0     1211 2024-02-19 14:52:46.343669 dekegg-0.1.3/dekegg/core.py
--rw-r--r--   0        0        0      194 2024-02-19 14:52:46.343669 dekegg-0.1.3/dekegg/templatefiles/project/pyproject.toml-tpl
--rw-r--r--   0        0        0      320 2024-02-19 14:52:46.343669 dekegg-0.1.3/dekegg/tmpl.py
--rw-r--r--   0        0        0      510 2024-02-19 14:52:47.871687 dekegg-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      267 1970-01-01 00:00:00.000000 dekegg-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        9 2024-04-25 19:15:25.883469 dekegg-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-25 19:15:25.883469 dekegg-0.1.4/dekegg/__init__.py
+-rw-r--r--   0        0        0     2337 2024-04-25 19:15:25.883469 dekegg-0.1.4/dekegg/bdist.py
+-rw-r--r--   0        0        0     1314 2024-04-25 19:15:25.883469 dekegg-0.1.4/dekegg/core.py
+-rw-r--r--   0        0        0      194 2024-04-25 19:15:25.883469 dekegg-0.1.4/dekegg/templatefiles/project/pyproject.toml-tpl
+-rw-r--r--   0        0        0      320 2024-04-25 19:15:25.883469 dekegg-0.1.4/dekegg/tmpl.py
+-rw-r--r--   0        0        0      510 2024-04-25 19:15:27.131473 dekegg-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      267 1970-01-01 00:00:00.000000 dekegg-0.1.4/PKG-INFO
```

### Comparing `dekegg-0.1.3/dekegg/bdist.py` & `dekegg-0.1.4/dekegg/bdist.py`

 * *Files identical despite different names*

