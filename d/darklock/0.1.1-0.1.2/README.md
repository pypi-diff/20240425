# Comparing `tmp/darklock-0.1.1.tar.gz` & `tmp/darklock-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "darklock-0.1.1.tar", last modified: Wed Apr 24 02:47:22 2024, max compression
+gzip compressed data, was "darklock-0.1.2.tar", last modified: Thu Apr 25 17:38:21 2024, max compression
```

## Comparing `darklock-0.1.1.tar` & `darklock-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:47:22.559034 darklock-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 02:47:16.000000 darklock-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-24 02:47:22.555034 darklock-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-24 02:47:16.000000 darklock-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 02:47:22.559034 darklock-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-24 02:47:16.000000 darklock-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:47:22.555034 darklock-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:47:22.555034 darklock-0.1.1/src/darklock/
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-24 02:47:16.000000 darklock-0.1.1/src/darklock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-24 02:47:16.000000 darklock-0.1.1/src/darklock/log_disc_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-24 02:47:16.000000 darklock-0.1.1/src/darklock/no_internet_socket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-24 02:47:16.000000 darklock-0.1.1/src/darklock/restrict_network_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-04-24 02:47:16.000000 darklock-0.1.1/src/darklock/restrict_os_access.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-24 02:47:16.000000 darklock-0.1.1/src/darklock/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:47:22.555034 darklock-0.1.1/src/darklock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-24 02:47:22.000000 darklock-0.1.1/src/darklock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-24 02:47:22.000000 darklock-0.1.1/src/darklock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 02:47:22.000000 darklock-0.1.1/src/darklock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 02:47:22.000000 darklock-0.1.1/src/darklock.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:47:22.555034 darklock-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-24 02:47:16.000000 darklock-0.1.1/tests/test_no_internet_socket.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-24 02:47:16.000000 darklock-0.1.1/tests/test_restrict_internet_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-24 02:47:16.000000 darklock-0.1.1/tests/test_restrict_os.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:21.623223 darklock-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-25 17:38:17.000000 darklock-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-25 17:38:21.623223 darklock-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-25 17:38:17.000000 darklock-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 17:38:21.623223 darklock-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-25 17:38:17.000000 darklock-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:21.619223 darklock-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:21.619223 darklock-0.1.2/src/darklock/
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-25 17:38:17.000000 darklock-0.1.2/src/darklock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-25 17:38:17.000000 darklock-0.1.2/src/darklock/log_disc_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-25 17:38:17.000000 darklock-0.1.2/src/darklock/no_internet_socket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-25 17:38:17.000000 darklock-0.1.2/src/darklock/restrict_network_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-04-25 17:38:17.000000 darklock-0.1.2/src/darklock/restrict_os_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-25 17:38:17.000000 darklock-0.1.2/src/darklock/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:21.623223 darklock-0.1.2/src/darklock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-25 17:38:21.000000 darklock-0.1.2/src/darklock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-25 17:38:21.000000 darklock-0.1.2/src/darklock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 17:38:21.000000 darklock-0.1.2/src/darklock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 17:38:21.000000 darklock-0.1.2/src/darklock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:21.623223 darklock-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-25 17:38:17.000000 darklock-0.1.2/tests/test_no_internet_socket.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-25 17:38:17.000000 darklock-0.1.2/tests/test_restrict_internet_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-25 17:38:17.000000 darklock-0.1.2/tests/test_restrict_os.py
```

### Comparing `darklock-0.1.1/LICENSE` & `darklock-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `darklock-0.1.1/PKG-INFO` & `darklock-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: darklock
-Version: 0.1.1
+Version: 0.1.2
 Home-page: https://github.com/Capsize-Games/darklock
 Author: Capsize LLC
 Author-email: contact@capsizegames.com
 License: GPL-3.0
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `darklock-0.1.1/README.md` & `darklock-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `darklock-0.1.1/setup.py` & `darklock-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="darklock",
-    version="0.1.1",
+    version="0.1.2",
     author="Capsize LLC",
     description="",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="",
     license="GPL-3.0",
     author_email="contact@capsizegames.com",
```

### Comparing `darklock-0.1.1/src/darklock/__init__.py` & `darklock-0.1.2/src/darklock/__init__.py`

 * *Files identical despite different names*

### Comparing `darklock-0.1.1/src/darklock/no_internet_socket.py` & `darklock-0.1.2/src/darklock/no_internet_socket.py`

 * *Files identical despite different names*

### Comparing `darklock-0.1.1/src/darklock/restrict_network_access.py` & `darklock-0.1.2/src/darklock/restrict_network_access.py`

 * *Files identical despite different names*

### Comparing `darklock-0.1.1/src/darklock/restrict_os_access.py` & `darklock-0.1.2/src/darklock/restrict_os_access.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from darklock.singleton import Singleton
 from darklock.log_disc_writer import LogDiscWriter
 import builtins
 import re
 import os
 import sys
 import traceback
-import importlib.abc
-import importlib.util
 
 
 class RestrictOSAccess(metaclass=Singleton):
     def __init__(self):
         self.original_open = None
         self.original_import = None
         self.logging_importer = None
@@ -21,18 +19,23 @@
         self.whitelisted_filenames = []
         self.whitelisted_imports = []
         self.blacklisted_filenames = []
 
     def restrict_os_write(self, *args, **kwargs):
         return self.original_os_write(*args, **kwargs)
 
+    def restricted_open(self, *args, **kwargs):
+        if ('open', args[0]) in self.whitelisted_operations or self.check_stack_trace():
+            return self.original_open(*args, **kwargs)
+        raise PermissionError("File system operations are not allowed")
+
     def restricted_os_makedirs(self, *args, **kwargs):
         if ('makedirs', args[0]) in self.whitelisted_operations or self.check_stack_trace():
             return self.original_makedirs(*args, **kwargs)
-        raise PermissionError("File system operations are not allowed")
+        #raise PermissionError("File system operations are not allowed")
 
     def restricted_open(self, *args, **kwargs):
         if ('open', args[0]) in self.whitelisted_operations or self.check_stack_trace():
             return self.original_open(*args, **kwargs)
         raise PermissionError("File system operations are not allowed")
 
     def restricted_exec(self, *args, **kwargs):
@@ -102,14 +105,16 @@
         self.original_os_write = os.write
         self.original_makedirs = os.makedirs
 
         os.makedirs = self.restricted_os_makedirs
 
         os.write = self.restrict_os_write
 
+        #builtins.open = self.restricted_open
+
         self.log_writes()
 
     def deactivate(self):
         """
         Uninstall the restrictions on OS access.
         :return:
         """
```

### Comparing `darklock-0.1.1/src/darklock.egg-info/PKG-INFO` & `darklock-0.1.2/src/darklock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: darklock
-Version: 0.1.1
+Version: 0.1.2
 Home-page: https://github.com/Capsize-Games/darklock
 Author: Capsize LLC
 Author-email: contact@capsizegames.com
 License: GPL-3.0
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `darklock-0.1.1/tests/test_restrict_internet_access.py` & `darklock-0.1.2/tests/test_restrict_internet_access.py`

 * *Files identical despite different names*

### Comparing `darklock-0.1.1/tests/test_restrict_os.py` & `darklock-0.1.2/tests/test_restrict_os.py`

 * *Files identical despite different names*

