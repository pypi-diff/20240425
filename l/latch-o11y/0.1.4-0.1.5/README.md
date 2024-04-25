# Comparing `tmp/latch_o11y-0.1.4.tar.gz` & `tmp/latch_o11y-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latch_o11y-0.1.4.tar", max compression
+gzip compressed data, was "latch_o11y-0.1.5.tar", last modified: Thu Apr 25 19:12:24 2024, max compression
```

## Comparing `latch_o11y-0.1.4.tar` & `latch_o11y-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     7052 2023-04-27 17:53:53.729206 latch_o11y-0.1.4/LICENSE
--rw-r--r--   0        0        0       14 2023-04-27 17:54:11.934983 latch_o11y-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-05-10 16:18:11.991042 latch_o11y-0.1.4/latch_o11y/__init__.py
--rw-r--r--   0        0        0     7048 2023-05-09 21:34:27.276447 latch_o11y-0.1.4/latch_o11y/o11y.py
--rw-r--r--   0        0        0        0 2023-05-09 17:04:17.188957 latch_o11y-0.1.4/latch_o11y/py.typed
--rw-r--r--   0        0        0     1257 2023-05-10 16:19:01.224331 latch_o11y-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 latch_o11y-0.1.4/setup.py
--rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 latch_o11y-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     7052 2024-04-25 18:50:14.283254 latch_o11y-0.1.5/LICENSE
+-rw-r--r--   0        0        0       14 2024-04-25 18:50:14.283392 latch_o11y-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2024-04-25 18:50:14.283525 latch_o11y-0.1.5/latch_o11y/__init__.py
+-rw-r--r--   0        0        0     7048 2024-04-25 19:06:13.919299 latch_o11y-0.1.5/latch_o11y/o11y.py
+-rw-r--r--   0        0        0        0 2024-04-25 18:50:14.283811 latch_o11y-0.1.5/latch_o11y/py.typed
+-rw-r--r--   0        0        0     2135 2024-04-25 19:12:24.139693 latch_o11y-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      490 1970-01-01 00:00:00.000000 latch_o11y-0.1.5/PKG-INFO
```

### Comparing `latch_o11y-0.1.4/LICENSE` & `latch_o11y-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `latch_o11y-0.1.4/latch_o11y/o11y.py` & `latch_o11y-0.1.5/latch_o11y/o11y.py`

 * *Files identical despite different names*

