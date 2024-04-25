# Comparing `tmp/flops_utils-0.2.3.tar.gz` & `tmp/flops_utils-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flops_utils-0.2.3.tar", max compression
+gzip compressed data, was "flops_utils-0.2.4.tar", max compression
```

## Comparing `flops_utils-0.2.3.tar` & `flops_utils-0.2.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        5 2024-04-19 12:44:40.095872 flops_utils-0.2.3/README.md
--rw-r--r--   0        0        0     1355 2024-04-19 14:45:40.771859 flops_utils-0.2.3/flops_utils/logging.py
--rw-r--r--   0        0        0     1393 2024-04-19 16:20:49.607848 flops_utils-0.2.3/flops_utils/notifications.py
--rw-r--r--   0        0        0      414 2024-04-19 17:57:15.491837 flops_utils-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 flops_utils-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0        5 2024-04-24 16:17:22.069103 flops_utils-0.2.4/README.md
+-rw-r--r--   0        0        0     1428 2024-04-25 13:27:44.818515 flops_utils-0.2.4/flops_utils/logging.py
+-rw-r--r--   0        0        0     1393 2024-04-24 16:17:22.077103 flops_utils-0.2.4/flops_utils/notifications.py
+-rw-r--r--   0        0        0      414 2024-04-25 13:28:06.638514 flops_utils-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 flops_utils-0.2.4/PKG-INFO
```

### Comparing `flops_utils-0.2.3/flops_utils/logging.py` & `flops_utils-0.2.4/flops_utils/logging.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,17 +11,20 @@
     yellow = "\x1b[38;5;226m"
     red = "\x1b[38;5;196m"
     bold_red = "\x1b[31;1m"
     blue = "\x1b[38;5;33m"
     light_blue = "\x1b[38;5;45m"
     reset = "\x1b[0m"
 
-    def __init__(self, fmt):
+    def __init__(self, fmt, with_color: bool = False):
         super().__init__()
         self.fmt = fmt
+        if not with_color:
+            return
+
         self.FORMATS = {
             logging.DEBUG: self.grey + self.fmt + self.reset,
             logging.INFO: self.light_blue + self.fmt + self.reset,
             logging.WARNING: self.yellow + self.fmt + self.reset,
             logging.ERROR: self.red + self.fmt + self.reset,
             logging.CRITICAL: self.bold_red + self.fmt + self.reset,
         }
```

### Comparing `flops_utils-0.2.3/flops_utils/notifications.py` & `flops_utils-0.2.4/flops_utils/notifications.py`

 * *Files identical despite different names*

