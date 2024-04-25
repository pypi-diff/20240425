# Comparing `tmp/flops_utils-0.2.4.tar.gz` & `tmp/flops_utils-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flops_utils-0.2.4.tar", max compression
+gzip compressed data, was "flops_utils-0.2.5.tar", max compression
```

## Comparing `flops_utils-0.2.4.tar` & `flops_utils-0.2.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        5 2024-04-24 16:17:22.069103 flops_utils-0.2.4/README.md
--rw-r--r--   0        0        0     1428 2024-04-25 13:27:44.818515 flops_utils-0.2.4/flops_utils/logging.py
--rw-r--r--   0        0        0     1393 2024-04-24 16:17:22.077103 flops_utils-0.2.4/flops_utils/notifications.py
--rw-r--r--   0        0        0      414 2024-04-25 13:28:06.638514 flops_utils-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 flops_utils-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0        5 2024-04-24 16:17:22.069103 flops_utils-0.2.5/README.md
+-rw-r--r--   0        0        0     1511 2024-04-25 13:32:02.994507 flops_utils-0.2.5/flops_utils/logging.py
+-rw-r--r--   0        0        0     1393 2024-04-24 16:17:22.077103 flops_utils-0.2.5/flops_utils/notifications.py
+-rw-r--r--   0        0        0      414 2024-04-25 13:32:24.354506 flops_utils-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 flops_utils-0.2.5/PKG-INFO
```

### Comparing `flops_utils-0.2.4/flops_utils/notifications.py` & `flops_utils-0.2.5/flops_utils/notifications.py`

 * *Files identical despite different names*

