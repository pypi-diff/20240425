# Comparing `tmp/shadowlogger-0.1.0.tar.gz` & `tmp/shadowlogger-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shadowlogger-0.1.0.tar", last modified: Wed Apr 24 00:55:18 2024, max compression
+gzip compressed data, was "shadowlogger-0.1.1.tar", last modified: Thu Apr 25 17:37:23 2024, max compression
```

## Comparing `shadowlogger-0.1.0.tar` & `shadowlogger-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:55:18.768134 shadowlogger-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 00:55:12.000000 shadowlogger-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-24 00:55:18.768134 shadowlogger-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-24 00:55:12.000000 shadowlogger-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 00:55:18.768134 shadowlogger-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-24 00:55:12.000000 shadowlogger-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:55:18.764134 shadowlogger-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:55:18.764134 shadowlogger-0.1.0/src/shadowlogger/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-24 00:55:12.000000 shadowlogger-0.1.0/src/shadowlogger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7976 2024-04-24 00:55:12.000000 shadowlogger-0.1.0/src/shadowlogger/intercept_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-04-24 00:55:12.000000 shadowlogger-0.1.0/src/shadowlogger/shadowlogger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-24 00:55:12.000000 shadowlogger-0.1.0/src/shadowlogger/shadowlogger_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-24 00:55:12.000000 shadowlogger-0.1.0/src/shadowlogger/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:55:18.768134 shadowlogger-0.1.0/src/shadowlogger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-24 00:55:18.000000 shadowlogger-0.1.0/src/shadowlogger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-24 00:55:18.000000 shadowlogger-0.1.0/src/shadowlogger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 00:55:18.000000 shadowlogger-0.1.0/src/shadowlogger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-24 00:55:18.000000 shadowlogger-0.1.0/src/shadowlogger.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:55:18.768134 shadowlogger-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-24 00:55:12.000000 shadowlogger-0.1.0/tests/test_custom_format.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-24 00:55:12.000000 shadowlogger-0.1.0/tests/test_custom_level.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-24 00:55:12.000000 shadowlogger-0.1.0/tests/test_custom_prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-24 00:55:12.000000 shadowlogger-0.1.0/tests/test_handle_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-24 00:55:12.000000 shadowlogger-0.1.0/tests/test_intercept_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-24 00:55:12.000000 shadowlogger-0.1.0/tests/test_shadow_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-24 00:55:12.000000 shadowlogger-0.1.0/tests/test_shadow_logger_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:37:23.730759 shadowlogger-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-25 17:37:19.000000 shadowlogger-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-25 17:37:23.730759 shadowlogger-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-25 17:37:19.000000 shadowlogger-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 17:37:23.730759 shadowlogger-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-25 17:37:19.000000 shadowlogger-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:37:23.726759 shadowlogger-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:37:23.726759 shadowlogger-0.1.1/src/shadowlogger/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-25 17:37:19.000000 shadowlogger-0.1.1/src/shadowlogger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-25 17:37:19.000000 shadowlogger-0.1.1/src/shadowlogger/base_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8761 2024-04-25 17:37:19.000000 shadowlogger-0.1.1/src/shadowlogger/intercept_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-04-25 17:37:19.000000 shadowlogger-0.1.1/src/shadowlogger/shadowlogger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-25 17:37:19.000000 shadowlogger-0.1.1/src/shadowlogger/shadowlogger_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-25 17:37:19.000000 shadowlogger-0.1.1/src/shadowlogger/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:37:23.730759 shadowlogger-0.1.1/src/shadowlogger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-25 17:37:23.000000 shadowlogger-0.1.1/src/shadowlogger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-25 17:37:23.000000 shadowlogger-0.1.1/src/shadowlogger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 17:37:23.000000 shadowlogger-0.1.1/src/shadowlogger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-25 17:37:23.000000 shadowlogger-0.1.1/src/shadowlogger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:37:23.730759 shadowlogger-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-25 17:37:19.000000 shadowlogger-0.1.1/tests/test_custom_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-25 17:37:19.000000 shadowlogger-0.1.1/tests/test_custom_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-25 17:37:19.000000 shadowlogger-0.1.1/tests/test_custom_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-25 17:37:19.000000 shadowlogger-0.1.1/tests/test_handle_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-25 17:37:19.000000 shadowlogger-0.1.1/tests/test_intercept_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-25 17:37:19.000000 shadowlogger-0.1.1/tests/test_shadow_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-25 17:37:19.000000 shadowlogger-0.1.1/tests/test_shadow_logger_manager.py
```

### Comparing `shadowlogger-0.1.0/LICENSE` & `shadowlogger-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shadowlogger-0.1.0/PKG-INFO` & `shadowlogger-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,17 @@
-Metadata-Version: 2.1
-Name: shadowlogger
-Version: 0.1.0
-Home-page: https://github.com/Capsize-Games/shadowlogger
-Author: Capsize LLC
-Author-email: contact@capsizegames.com
-License: GPL-3.0
-Requires-Python: >=3.10.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Shadowlogger
 
 Simple wrapper for built-in logger module which intercepts all logs and shadows them, preventing sensitive information from being leaked.
 
 ---
 
 ![img.png](img.png)
 
+[![Upload Python Package](https://github.com/Capsize-Games/shadowlogger/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Capsize-Games/shadowlogger/actions/workflows/python-publish.yml)
+
 ---
 
 ## Installation
 
 ```bash
 pip install shadowlogger
 ```
```

### Comparing `shadowlogger-0.1.0/setup.py` & `shadowlogger-0.1.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="shadowlogger",
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

### Comparing `shadowlogger-0.1.0/src/shadowlogger/intercept_handler.py` & `shadowlogger-0.1.1/src/shadowlogger/intercept_handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,27 @@
 import logging
 import os
 import socket
 import sys
 
 
 class InterceptHandler(logging.Handler):
-    def __init__(self, shadow_logger):
+    def __init__(
+        self,
+        shadow_logger,
+        show_stdout: bool = True,
+        hook: callable = lambda x: None
+    ):
+        """
+        InterceptHandler intercepts and logs print statements, file operations, and network operations.
+
+        :param shadow_logger:
+        :param show_stdout:
+        :param hook: A callback function to process log entries.
+        """
         super().__init__()
         self.__original_sys_stdout = {
             "displayhook": None,
             "excepthook": None,
             "exc_info": None,
             "exit": None,
             "getdlopenflags": None,
@@ -20,14 +32,15 @@
             "getsizeof": None,
             "gettrace": None,
             "setdlopenflags": None,
             "setprofile": None,
             "setrecursionlimit": None,
             "settrace": None,
         }
+        self.__hook = hook
         self.__original_os_functions = {
             # "path": None,
             # "name": None,
             # "curdir": None,
             # "pardir": None,
             # "sep": None,
             # "extsep": None,
@@ -57,32 +70,41 @@
             # "inet_ntoa,": None,
             # "getdefaulttimeout": None,
             # "setdefaulttimeout": None,
             # "create_connection": None,
         }
         self.shadow_logger = shadow_logger
         self.lock = threading.Lock()
+        self.__show_stdout = show_stdout
 
         with self.lock:
             # Overriding sys.stdout to capture print statements
-            sys.stdout = self.LogStream(self.emit_record)
+            sys.stdout = self.LogStream(self.emit_record, show_stdout=self.show_stdout)
             for k, v in self.__original_sys_stdout.items():
                 self.__original_sys_stdout[k] = getattr(sys, k, None)
                 setattr(sys, k, self.__override_sys_stdout(getattr(sys, k, None)))
 
             # Overriding file writes
             for k, v in self.__original_os_functions.items():
                 self.__original_os_functions[k] = getattr(os, k, None)
                 setattr(os, k, self.__override_os_function(getattr(os, k, None)))
 
             # Overriding network operations
             for k, v in self.__original_socket_functions.items():
                 self.__original_socket_functions[k] = getattr(socket, k, None)
                 setattr(socket, k, self.__override_socket_function(getattr(socket, k, None)))
 
+    @property
+    def show_stdout(self):
+        return self.__show_stdout
+
+    @show_stdout.setter
+    def show_stdout(self, value):
+        self.__show_stdout = value
+
     def restore_original_functions(self):
         self.__restore_sys_stdout()
         self.__restore_os_functions()
         self.__restore_socket_functions()
 
     def __restore_sys_stdout(self):
         with self.lock:
@@ -99,17 +121,14 @@
             for k, v in self.__original_socket_functions.items():
                 setattr(socket, k, v)
 
     def __override_sys_stdout(self, original_function):
         """Override sys.stdout to capture print statements."""
 
         def custom_stdout(*args, **kwargs):
-            print("*" * 10)
-            print(args, kwargs)
-            print("*" * 10)
             with self.lock:
                 if original_function:
                     return original_function(*args, **kwargs)
 
         return custom_stdout
 
     def __override_os_function(self, original_function):
@@ -140,15 +159,17 @@
         # Manually emit log record from captured print statements
         record = self.shadow_logger.makeRecord(self.shadow_logger.name, level, fn='', lno='', msg=message, args=None, exc_info=None)
         self.process_log_record(record)
 
     def process_log_record(self, record):
         log_entry: str = self.__sanitized_log_entry(record)
         log_info = self.prepare_log_info(record, log_entry)
-        self.shadow_logger.handle_message(log_info, record.levelno, log_info)
+        if "Shadowlogger" not in log_entry:
+            self.shadow_logger.handle_message(log_entry, record.levelno, log_info)
+        self.__hook(log_entry)
 
     def prepare_log_info(self, record, log_entry):
         """Prepare log information dictionary with enhanced details."""
         return {
             'name': record.name,
             'level': record.levelno,
             'message': log_entry,
@@ -199,20 +220,23 @@
                 return original_function(data, *args, **kwargs)
 
         return custom_send
 
     class LogStream:
         """Stream object to capture print statements and redirect them as log entries."""
 
-        def __init__(self, log_function):
+        def __init__(self, log_function, show_stdout:bool = True):
             self.log_function = log_function
+            self.__show_stdout = show_stdout
 
         def write(self, message):
             if message.strip() != "":
                 self.log_function(message.strip())
+                if self.__show_stdout:
+                    sys.__stdout__.write((message.strip() + '\n'))
 
         def flush(self):
             pass
 
 
 class LogHandler:
     def handle(self, log):
```

### Comparing `shadowlogger-0.1.0/src/shadowlogger/shadowlogger_manager.py` & `shadowlogger-0.1.1/src/shadowlogger/shadowlogger_manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,73 @@
 import threading
 import logging
+from typing import List
 
-from shadowlogger.intercept_handler import InterceptHandler
+from shadowlogger.base_tracker import BaseTracker
 from shadowlogger.shadowlogger import ShadowLogger
 from shadowlogger.singleton import Singleton
 
 
 class ShadowLoggerManager(metaclass=Singleton):
-    def __init__(self):
+    def __init__(self, show_stdout: bool = True):
         self.original_handlers = None
-        self.handler = None
-        self.shadow_logger = ShadowLogger()
         self.lock = threading.Lock()
+        self.__shadowlogger = None
+        self.__show_stdout = show_stdout
+        self.__active = False
+
+    @property
+    def shadowlogger(self):
+        return self.__shadowlogger
+
+    def activate(
+        self,
+        show_stdout: bool = None,
+        trackers: List[BaseTracker] = None
+    ):
+        self.__show_stdout = show_stdout if show_stdout is not None else self.__show_stdout
 
-    def activate(self):
-        if self.handler is None:
-            self.handler = InterceptHandler(self.shadow_logger)
+        if self.__active:
+            self.deactivate()
 
+        self.__shadowlogger = ShadowLogger(self.__show_stdout, trackers=trackers)
+
+        self.__active = True
         with self.lock:
             # Get the root logger
             root_logger = logging.getLogger()
 
             # Keep track of the original handlers
             self.original_handlers = root_logger.handlers[:]
 
             # Remove all existing handlers from the root logger
             for h in root_logger.handlers[:]:
                 root_logger.removeHandler(h)
 
             # Add the InterceptHandler to the root logger
-            root_logger.addHandler(self.handler)
+            root_logger.addHandler(self.shadowlogger.intercept_handler)
 
             # Set the level for the root logger
             root_logger.setLevel(logging.INFO)
 
             # Prevent propagation of log records to other handlers
             root_logger.propagate = False
 
     def deactivate(self):
+        if not self.__active:
+            return
         with self.lock:
             # Get the root logger
             root_logger = logging.getLogger()
 
             # Remove the InterceptHandler from the root logger
-            root_logger.removeHandler(self.handler)
+            root_logger.removeHandler(self.shadowlogger.intercept_handler)
 
             # Restore the original handlers
             for h in self.original_handlers:
                 root_logger.addHandler(h)
 
             # Allow propagation of log records to other handlers
             root_logger.propagate = True
 
             # Restore the original os.write and socket.send functions
-            self.handler.restore_original_functions()
+            self.shadowlogger.intercept_handler.restore_original_functions()
```

### Comparing `shadowlogger-0.1.0/src/shadowlogger.egg-info/SOURCES.txt` & `shadowlogger-0.1.1/src/shadowlogger.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 src/shadowlogger/__init__.py
+src/shadowlogger/base_tracker.py
 src/shadowlogger/intercept_handler.py
 src/shadowlogger/shadowlogger.py
 src/shadowlogger/shadowlogger_manager.py
 src/shadowlogger/singleton.py
 src/shadowlogger.egg-info/PKG-INFO
 src/shadowlogger.egg-info/SOURCES.txt
 src/shadowlogger.egg-info/dependency_links.txt
```

### Comparing `shadowlogger-0.1.0/tests/test_custom_format.py` & `shadowlogger-0.1.1/tests/test_custom_format.py`

 * *Files identical despite different names*

### Comparing `shadowlogger-0.1.0/tests/test_custom_level.py` & `shadowlogger-0.1.1/tests/test_custom_level.py`

 * *Files identical despite different names*

### Comparing `shadowlogger-0.1.0/tests/test_custom_prefix.py` & `shadowlogger-0.1.1/tests/test_custom_prefix.py`

 * *Files identical despite different names*

### Comparing `shadowlogger-0.1.0/tests/test_handle_logger.py` & `shadowlogger-0.1.1/tests/test_handle_logger.py`

 * *Files identical despite different names*

### Comparing `shadowlogger-0.1.0/tests/test_intercept_handler.py` & `shadowlogger-0.1.1/tests/test_intercept_handler.py`

 * *Files identical despite different names*

### Comparing `shadowlogger-0.1.0/tests/test_shadow_logger.py` & `shadowlogger-0.1.1/tests/test_shadow_logger.py`

 * *Files identical despite different names*

### Comparing `shadowlogger-0.1.0/tests/test_shadow_logger_manager.py` & `shadowlogger-0.1.1/tests/test_shadow_logger_manager.py`

 * *Files identical despite different names*

