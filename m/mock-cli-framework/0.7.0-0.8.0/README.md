# Comparing `tmp/mock-cli-framework-0.7.0.tar.gz` & `tmp/mock_cli_framework-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mock-cli-framework-0.7.0.tar", last modified: Fri Oct  6 20:28:50 2023, max compression
+gzip compressed data, was "mock_cli_framework-0.8.0.tar", last modified: Thu Apr 25 20:54:54 2024, max compression
```

## Comparing `mock-cli-framework-0.7.0.tar` & `mock_cli_framework-0.8.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-10-06 20:28:50.899348 mock-cli-framework-0.7.0/
--rw-r--r--   0 zach       (502) staff       (20)     1071 2020-12-02 02:55:12.000000 mock-cli-framework-0.7.0/LICENSE
--rw-r--r--   0 zach       (502) staff       (20)     9890 2023-10-06 20:28:50.899264 mock-cli-framework-0.7.0/PKG-INFO
--rw-r--r--   0 zach       (502) staff       (20)     9452 2023-07-10 22:44:06.000000 mock-cli-framework-0.7.0/README.md
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-10-06 20:28:50.896562 mock-cli-framework-0.7.0/mock_cli/
--rw-r--r--   0 zach       (502) staff       (20)      541 2023-10-06 20:27:50.000000 mock-cli-framework-0.7.0/mock_cli/__about__.py
--rw-r--r--   0 zach       (502) staff       (20)      513 2023-07-01 05:01:04.000000 mock-cli-framework-0.7.0/mock_cli/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)      147 2021-02-04 03:22:02.000000 mock-cli-framework-0.7.0/mock_cli/about.py
--rw-r--r--   0 zach       (502) staff       (20)      791 2023-06-16 22:37:28.000000 mock-cli-framework-0.7.0/mock_cli/argv_conversion.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-10-06 20:28:50.898324 mock-cli-framework-0.7.0/mock_cli/data/
--rw-r--r--   0 zach       (502) staff       (20)       87 2022-09-12 01:48:18.000000 mock-cli-framework-0.7.0/mock_cli/data/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)       33 2023-07-01 05:01:04.000000 mock-cli-framework-0.7.0/mock_cli/data/_env-template.json
--rw-r--r--   0 zach       (502) staff       (20)      624 2022-09-12 00:59:53.000000 mock-cli-framework-0.7.0/mock_cli/data/config-example.json
--rw-r--r--   0 zach       (502) staff       (20)       71 2023-07-01 05:01:04.000000 mock-cli-framework-0.7.0/mock_cli/data/config-template.json
--rw-r--r--   0 zach       (502) staff       (20)      357 2023-02-17 23:11:41.000000 mock-cli-framework-0.7.0/mock_cli/hashing.py
--rw-r--r--   0 zach       (502) staff       (20)     2507 2023-06-21 02:46:51.000000 mock-cli-framework-0.7.0/mock_cli/mock_cmd.py
--rw-r--r--   0 zach       (502) staff       (20)     7849 2023-08-29 03:39:06.000000 mock-cli-framework-0.7.0/mock_cli/mock_cmd_state.py
--rw-r--r--   0 zach       (502) staff       (20)     2802 2023-10-06 20:25:25.000000 mock-cli-framework-0.7.0/mock_cli/path.py
--rw-r--r--   0 zach       (502) staff       (20)      161 2022-09-12 00:48:54.000000 mock-cli-framework-0.7.0/mock_cli/pkg_resources.py
--rw-r--r--   0 zach       (502) staff       (20)     8928 2023-10-06 19:54:59.000000 mock-cli-framework-0.7.0/mock_cli/responses.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-10-06 20:28:50.899040 mock-cli-framework-0.7.0/mock_cli_framework.egg-info/
--rw-r--r--   0 zach       (502) staff       (20)     9890 2023-10-06 20:28:50.000000 mock-cli-framework-0.7.0/mock_cli_framework.egg-info/PKG-INFO
--rw-r--r--   0 zach       (502) staff       (20)      554 2023-10-06 20:28:50.000000 mock-cli-framework-0.7.0/mock_cli_framework.egg-info/SOURCES.txt
--rw-r--r--   0 zach       (502) staff       (20)        1 2023-10-06 20:28:50.000000 mock-cli-framework-0.7.0/mock_cli_framework.egg-info/dependency_links.txt
--rw-r--r--   0 zach       (502) staff       (20)        9 2023-10-06 20:28:50.000000 mock-cli-framework-0.7.0/mock_cli_framework.egg-info/top_level.txt
--rw-r--r--   0 zach       (502) staff       (20)      156 2023-10-06 20:28:50.899597 mock-cli-framework-0.7.0/setup.cfg
--rw-r--r--   0 zach       (502) staff       (20)      725 2023-08-16 02:59:57.000000 mock-cli-framework-0.7.0/setup.py
+drwxr-xr-x   0 zach       (503) staff       (20)        0 2024-04-25 20:54:54.531828 mock_cli_framework-0.8.0/
+-rw-r--r--   0 zach       (503) staff       (20)     1071 2020-12-02 02:55:12.000000 mock_cli_framework-0.8.0/LICENSE
+-rw-r--r--   0 zach       (503) staff       (20)     9890 2024-04-25 20:54:54.531744 mock_cli_framework-0.8.0/PKG-INFO
+-rw-r--r--   0 zach       (503) staff       (20)     9452 2023-07-10 22:44:06.000000 mock_cli_framework-0.8.0/README.md
+drwxr-xr-x   0 zach       (503) staff       (20)        0 2024-04-25 20:54:54.530211 mock_cli_framework-0.8.0/mock_cli/
+-rw-r--r--   0 zach       (503) staff       (20)      541 2024-04-25 20:48:25.000000 mock_cli_framework-0.8.0/mock_cli/__about__.py
+-rw-r--r--   0 zach       (503) staff       (20)      513 2023-07-01 05:01:04.000000 mock_cli_framework-0.8.0/mock_cli/__init__.py
+-rw-r--r--   0 zach       (503) staff       (20)      147 2021-02-04 03:22:02.000000 mock_cli_framework-0.8.0/mock_cli/about.py
+-rw-r--r--   0 zach       (503) staff       (20)      791 2023-06-16 22:37:28.000000 mock_cli_framework-0.8.0/mock_cli/argv_conversion.py
+drwxr-xr-x   0 zach       (503) staff       (20)        0 2024-04-25 20:54:54.530826 mock_cli_framework-0.8.0/mock_cli/data/
+-rw-r--r--   0 zach       (503) staff       (20)       87 2022-09-12 01:48:18.000000 mock_cli_framework-0.8.0/mock_cli/data/__init__.py
+-rw-r--r--   0 zach       (503) staff       (20)       33 2023-07-01 05:01:04.000000 mock_cli_framework-0.8.0/mock_cli/data/_env-template.json
+-rw-r--r--   0 zach       (503) staff       (20)      624 2022-09-12 00:59:53.000000 mock_cli_framework-0.8.0/mock_cli/data/config-example.json
+-rw-r--r--   0 zach       (503) staff       (20)       71 2023-07-01 05:01:04.000000 mock_cli_framework-0.8.0/mock_cli/data/config-template.json
+-rw-r--r--   0 zach       (503) staff       (20)      357 2023-02-17 23:11:41.000000 mock_cli_framework-0.8.0/mock_cli/hashing.py
+-rw-r--r--   0 zach       (503) staff       (20)     2683 2024-04-25 20:44:10.000000 mock_cli_framework-0.8.0/mock_cli/mock_cmd.py
+-rw-r--r--   0 zach       (503) staff       (20)     7849 2023-08-29 03:39:06.000000 mock_cli_framework-0.8.0/mock_cli/mock_cmd_state.py
+-rw-r--r--   0 zach       (503) staff       (20)     2802 2023-10-06 20:25:25.000000 mock_cli_framework-0.8.0/mock_cli/path.py
+-rw-r--r--   0 zach       (503) staff       (20)      161 2022-09-12 00:48:54.000000 mock_cli_framework-0.8.0/mock_cli/pkg_resources.py
+-rw-r--r--   0 zach       (503) staff       (20)     8928 2023-10-06 19:54:59.000000 mock_cli_framework-0.8.0/mock_cli/responses.py
+drwxr-xr-x   0 zach       (503) staff       (20)        0 2024-04-25 20:54:54.531529 mock_cli_framework-0.8.0/mock_cli_framework.egg-info/
+-rw-r--r--   0 zach       (503) staff       (20)     9890 2024-04-25 20:54:54.000000 mock_cli_framework-0.8.0/mock_cli_framework.egg-info/PKG-INFO
+-rw-r--r--   0 zach       (503) staff       (20)      554 2024-04-25 20:54:54.000000 mock_cli_framework-0.8.0/mock_cli_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 zach       (503) staff       (20)        1 2024-04-25 20:54:54.000000 mock_cli_framework-0.8.0/mock_cli_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 zach       (503) staff       (20)        9 2024-04-25 20:54:54.000000 mock_cli_framework-0.8.0/mock_cli_framework.egg-info/top_level.txt
+-rw-r--r--   0 zach       (503) staff       (20)      156 2024-04-25 20:54:54.532027 mock_cli_framework-0.8.0/setup.cfg
+-rw-r--r--   0 zach       (503) staff       (20)      725 2023-08-16 02:59:57.000000 mock_cli_framework-0.8.0/setup.py
```

### Comparing `mock-cli-framework-0.7.0/LICENSE` & `mock_cli_framework-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mock-cli-framework-0.7.0/PKG-INFO` & `mock_cli_framework-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mock-cli-framework
-Version: 0.7.0
+Version: 0.8.0
 Summary: A framework for creating stand-ins for CLI tools that pretend to be the real thing for when "the real thing" isn't suitable, such as in automated tests.
 Home-page: https://github.com/zcutlip/mock-cli-framework.git
 Author: Zachary Cutlip
 Author-email: uid000@gmail.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `mock-cli-framework-0.7.0/README.md` & `mock_cli_framework-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `mock-cli-framework-0.7.0/mock_cli/__about__.py` & `mock_cli_framework-0.8.0/mock_cli/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __title__ = "Mock CLI Framework"
-__version__ = "0.7.0"
+__version__ = "0.8.0"
 __summary__ = """A framework for creating stand-ins for CLI tools that pretend to be the real thing for when "the real thing" isn't suitable, such as in automated tests."""
 
 """
 See PEP 440 for version scheme
 https://www.python.org/dev/peps/pep-0440/#examples-of-compliant-version-schemes
 Examples:
```

### Comparing `mock-cli-framework-0.7.0/mock_cli/__init__.py` & `mock_cli_framework-0.8.0/mock_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `mock-cli-framework-0.7.0/mock_cli/argv_conversion.py` & `mock_cli_framework-0.8.0/mock_cli/argv_conversion.py`

 * *Files identical despite different names*

### Comparing `mock-cli-framework-0.7.0/mock_cli/data/config-example.json` & `mock_cli_framework-0.8.0/mock_cli/data/config-example.json`

 * *Files identical despite different names*

### Comparing `mock-cli-framework-0.7.0/mock_cli/mock_cmd.py` & `mock_cli_framework-0.8.0/mock_cli/mock_cmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import sys
 from pathlib import Path
+from typing import IO
 
 from .mock_cmd_state import MockCMDState, MockCMDStateNoDirectoryException
 from .responses import (
     CommandResponse,
     ResponseDirectory,
     ResponseReadException
 )
@@ -32,15 +33,20 @@
             pass
 
         if response_directory is None:
             raise MockCommandResponseDirException(
                 "No response directory provided")
         return response_directory
 
-    def _write_binary(self, output_handle, data):
+    @classmethod
+    def write_binary_output(cls, output_handle: IO, data: bytes):
+        return cls._write_binary(output_handle, data)
+
+    @classmethod
+    def _write_binary(cls, output_handle, data):
         with os.fdopen(output_handle.fileno(), "wb", closefd=False) as fd:
             fd.write(data)
             fd.flush()
 
     def get_response(self, args, input=None) -> CommandResponse:
         response = self.response_directory.response_lookup(args, input=input)
         return response
```

### Comparing `mock-cli-framework-0.7.0/mock_cli/mock_cmd_state.py` & `mock_cli_framework-0.8.0/mock_cli/mock_cmd_state.py`

 * *Files identical despite different names*

### Comparing `mock-cli-framework-0.7.0/mock_cli/path.py` & `mock_cli_framework-0.8.0/mock_cli/path.py`

 * *Files identical despite different names*

### Comparing `mock-cli-framework-0.7.0/mock_cli/responses.py` & `mock_cli_framework-0.8.0/mock_cli/responses.py`

 * *Files identical despite different names*

### Comparing `mock-cli-framework-0.7.0/mock_cli_framework.egg-info/PKG-INFO` & `mock_cli_framework-0.8.0/mock_cli_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mock-cli-framework
-Version: 0.7.0
+Version: 0.8.0
 Summary: A framework for creating stand-ins for CLI tools that pretend to be the real thing for when "the real thing" isn't suitable, such as in automated tests.
 Home-page: https://github.com/zcutlip/mock-cli-framework.git
 Author: Zachary Cutlip
 Author-email: uid000@gmail.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `mock-cli-framework-0.7.0/mock_cli_framework.egg-info/SOURCES.txt` & `mock_cli_framework-0.8.0/mock_cli_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mock-cli-framework-0.7.0/setup.py` & `mock_cli_framework-0.8.0/setup.py`

 * *Files identical despite different names*

