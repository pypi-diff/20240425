# Comparing `tmp/nullscream-0.1.0.tar.gz` & `tmp/nullscream-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nullscream-0.1.0.tar", last modified: Wed Apr 24 00:52:29 2024, max compression
+gzip compressed data, was "nullscream-0.1.1.tar", last modified: Thu Apr 25 17:38:51 2024, max compression
```

## Comparing `nullscream-0.1.0.tar` & `nullscream-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:52:29.627022 nullscream-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 00:52:25.000000 nullscream-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-24 00:52:29.623021 nullscream-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-24 00:52:25.000000 nullscream-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 00:52:29.627022 nullscream-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-24 00:52:25.000000 nullscream-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:52:29.623021 nullscream-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:52:29.623021 nullscream-0.1.0/src/nullscream/
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-24 00:52:25.000000 nullscream-0.1.0/src/nullscream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-24 00:52:25.000000 nullscream-0.1.0/src/nullscream/noop_class.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-24 00:52:25.000000 nullscream-0.1.0/src/nullscream/noop_function.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:52:29.623021 nullscream-0.1.0/src/nullscream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-24 00:52:29.000000 nullscream-0.1.0/src/nullscream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-24 00:52:29.000000 nullscream-0.1.0/src/nullscream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 00:52:29.000000 nullscream-0.1.0/src/nullscream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-24 00:52:29.000000 nullscream-0.1.0/src/nullscream.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:52:29.623021 nullscream-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-24 00:52:25.000000 nullscream-0.1.0/tests/test_blacklist.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-24 00:52:25.000000 nullscream-0.1.0/tests/test_whitelist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:51.891032 nullscream-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-25 17:38:47.000000 nullscream-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-25 17:38:51.891032 nullscream-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-25 17:38:47.000000 nullscream-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 17:38:51.891032 nullscream-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-25 17:38:47.000000 nullscream-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:51.891032 nullscream-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:51.891032 nullscream-0.1.1/src/nullscream/
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-25 17:38:47.000000 nullscream-0.1.1/src/nullscream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-25 17:38:47.000000 nullscream-0.1.1/src/nullscream/noop_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-25 17:38:47.000000 nullscream-0.1.1/src/nullscream/noop_function.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:51.891032 nullscream-0.1.1/src/nullscream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-25 17:38:51.000000 nullscream-0.1.1/src/nullscream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-25 17:38:51.000000 nullscream-0.1.1/src/nullscream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 17:38:51.000000 nullscream-0.1.1/src/nullscream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-25 17:38:51.000000 nullscream-0.1.1/src/nullscream.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:51.891032 nullscream-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-25 17:38:47.000000 nullscream-0.1.1/tests/test_blacklist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-25 17:38:47.000000 nullscream-0.1.1/tests/test_whitelist.py
```

### Comparing `nullscream-0.1.0/LICENSE` & `nullscream-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nullscream-0.1.0/PKG-INFO` & `nullscream-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,15 @@
-Metadata-Version: 2.1
-Name: nullscream
-Version: 0.1.0
-Home-page: https://github.com/Capsize-Games/nullscream
-Author: Capsize LLC
-Author-email: contact@capsizegames.com
-License: GPL-3.0
-Requires-Python: >=3.10.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # NULLSCREAM
 
 ---
 
 ![img.png](img.png)
 
+[![Upload Python Package](https://github.com/Capsize-Games/nullscream/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Capsize-Games/nullscream/actions/workflows/python-publish.yml)
+
 ---
 
 `nullscream` is a simple library that allows you to
 import noop functions and classes that you can use as drop in replacements for functions you wish to override.
 
 This allows anything on the blacklist to be importable, but not executable.
```

### Comparing `nullscream-0.1.0/setup.py` & `nullscream-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="nullscream",
-    version="0.1.0",
+    version="0.1.1",
     author="Capsize LLC",
     description="",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="",
     license="GPL-3.0",
     author_email="contact@capsizegames.com",
```

### Comparing `nullscream-0.1.0/src/nullscream/__init__.py` & `nullscream-0.1.1/src/nullscream/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,68 @@
+import logging
 import types
 import sys
 import importlib.machinery
 from importlib import abc
 
 from nullscream.noop_class import NoopClass
 
 
 class NoopLoader(abc.Loader):
     """
     Loader that creates noop stand-in modules.
     """
+    def __init__(self, function_blacklist=None):
+        self.function_blacklist = function_blacklist or []
+
     def create_module(self, spec):
         return types.ModuleType(spec.name)
 
     def exec_module(self, module):
         module.__dict__.update({
             "__all__": [],  # Empty export list
             "__doc__": "This is a noop stand-in module.",
             "__getattr__": NoopClass(),
             "__setattr__": NoopClass(),
             "__delattr__": NoopClass(),
             "__dir__": NoopClass(),
         })
 
+        # Override blacklisted functions
+        for func_name in self.function_blacklist:
+            if func_name in module.__dict__:
+                module.__dict__[func_name] = NoopClass()
+
 class NoopFinder(importlib.abc.MetaPathFinder):
-    def __init__(self, blacklist=None, whitelist=None):
+    def __init__(self, blacklist=None, whitelist=None, function_blacklist=None):
         self.blacklist = blacklist or []
         self.whitelist = whitelist or []
+        self.function_blacklist = function_blacklist or []
+
+        # Create a logger for this class
+        self.logger = logging.getLogger(__name__)
 
     def find_spec(self, fullname, path, target=None):
         root = fullname.split('.')[0]
-
         if (
-            (
-                fullname in self.blacklist and fullname not in self.whitelist
-            )
+            (root in self.blacklist and fullname not in self.whitelist)
+            or fullname in self.blacklist
         ):
-            return importlib.machinery.ModuleSpec(fullname, NoopLoader())
+            # Log the blocked module
+            self.logger.info(f"nullscream_block {fullname}")
+
+            return importlib.machinery.ModuleSpec(fullname, NoopLoader(self.function_blacklist))
+        else:
+            # Log the allowed module
+            self.logger.info(f"nullscream_allow {fullname}")
         return None
 
 
-def activate(blacklist=None, whitelist=None):
-    sys.meta_path.insert(0, NoopFinder(blacklist, whitelist))
+def activate(blacklist=None, whitelist=None, function_blacklist=None):
+    sys.meta_path.insert(0, NoopFinder(blacklist, whitelist, function_blacklist))
 
 
 def deactivate(blacklist=None):
     sys.meta_path = [finder for finder in sys.meta_path if not isinstance(finder, NoopFinder)]
     if blacklist:
         for module_name in blacklist:
             try:
```

### Comparing `nullscream-0.1.0/src/nullscream/noop_class.py` & `nullscream-0.1.1/src/nullscream/noop_class.py`

 * *Files identical despite different names*

### Comparing `nullscream-0.1.0/src/nullscream.egg-info/PKG-INFO` & `nullscream-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: nullscream
-Version: 0.1.0
+Version: 0.1.1
 Home-page: https://github.com/Capsize-Games/nullscream
 Author: Capsize LLC
 Author-email: contact@capsizegames.com
 License: GPL-3.0
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # NULLSCREAM
 
 ---
 
 ![img.png](img.png)
 
+[![Upload Python Package](https://github.com/Capsize-Games/nullscream/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Capsize-Games/nullscream/actions/workflows/python-publish.yml)
+
 ---
 
 `nullscream` is a simple library that allows you to
 import noop functions and classes that you can use as drop in replacements for functions you wish to override.
 
 This allows anything on the blacklist to be importable, but not executable.
```

### Comparing `nullscream-0.1.0/tests/test_whitelist.py` & `nullscream-0.1.1/tests/test_whitelist.py`

 * *Files identical despite different names*

