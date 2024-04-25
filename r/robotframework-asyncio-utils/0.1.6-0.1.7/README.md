# Comparing `tmp/robotframework_asyncio_utils-0.1.6.tar.gz` & `tmp/robotframework_asyncio_utils-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_asyncio_utils-0.1.6.tar", max compression
+gzip compressed data, was "robotframework_asyncio_utils-0.1.7.tar", max compression
```

## Comparing `robotframework_asyncio_utils-0.1.6.tar` & `robotframework_asyncio_utils-0.1.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       40 2023-08-02 23:28:36.742811 robotframework_asyncio_utils-0.1.6/AsyncioUtils/__init__.py
--rw-r--r--   0        0        0     5990 2023-08-03 00:20:58.985412 robotframework_asyncio_utils-0.1.6/AsyncioUtils/AsyncioUtils.py
--rw-r--r--   0        0        0     1090 2023-08-02 22:42:06.375801 robotframework_asyncio_utils-0.1.6/LICENSE
--rw-r--r--   0        0        0      550 2023-08-03 00:31:54.773759 robotframework_asyncio_utils-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      592 2023-08-03 00:31:56.182029 robotframework_asyncio_utils-0.1.6/README.md
--rw-r--r--   0        0        0     1198 1970-01-01 00:00:00.000000 robotframework_asyncio_utils-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     5835 2024-04-25 00:27:34.490973 robotframework_asyncio_utils-0.1.7/AsyncioUtils/AsyncioUtils.py
+-rw-r--r--   0        0        0       39 2024-04-25 00:25:17.000354 robotframework_asyncio_utils-0.1.7/AsyncioUtils/__init__.py
+-rw-r--r--   0        0        0     1069 2024-04-25 00:25:17.000354 robotframework_asyncio_utils-0.1.7/LICENSE
+-rw-r--r--   0        0        0      566 2024-04-25 00:25:17.000354 robotframework_asyncio_utils-0.1.7/README.md
+-rw-r--r--   0        0        0      528 2024-04-25 00:28:13.702581 robotframework_asyncio_utils-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1242 1970-01-01 00:00:00.000000 robotframework_asyncio_utils-0.1.7/PKG-INFO
```

### Comparing `robotframework_asyncio_utils-0.1.6/AsyncioUtils/AsyncioUtils.py` & `robotframework_asyncio_utils-0.1.7/AsyncioUtils/AsyncioUtils.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,155 +1,155 @@
-"""
-Utility functions to help using asyncio features.
-
-Some implementations used part of functions from the BuiltIn module from robot itself.
-"""
-
-
-import time
-import inspect
-import asyncio
-
-from robot.libraries.BuiltIn import BuiltIn
-from robot.utils.robottime import timestr_to_secs, secs_to_timestr
-from robot.errors import DataError, ExecutionPassed, ExecutionFailed, ExecutionFailures
-
-
-class AsyncioUtils:
-
-    def __init__(self) -> None:
-        try:
-            self.builtIn = BuiltIn()
-        except Exception:
-            self.builtIn = None
-
-    async def async_gather_keywords(self, *keywords):
-        """Executes all the given keywords concurrently.
-
-        This keyword is mainly useful to run multiple keywords concurrently
-        just like calling asyncio.gather() in python.
-        The keywords passed need to be async, else an error is raised.
-
-        By default all arguments are expected to be keywords to be executed.
-
-        Examples:
-        | `Run Keywords` | `Initialize database` | `Start servers` | `Clear logs` |
-        | `Run Keywords` | ${KW 1} | ${KW 2} |
-        | `Run Keywords` | @{KEYWORDS} |
-
-        Keywords can also be run with arguments using upper case ``AND`` as
-        a separator between keywords. The keywords are executed so that the
-        first argument is the first keyword and proceeding arguments until
-        the first ``AND`` are arguments to it. First argument after the first
-        ``AND`` is the second keyword and proceeding arguments until the next
-        ``AND`` are its arguments. And so on.
-
-        Examples:
-        | `Run Keywords` | `Initialize database` | db1 | AND | `Start servers` | server1 | server2 |
-        | `Run Keywords` | `Initialize database` | ${DB NAME} | AND | `Start servers` | @{SERVERS} | AND | `Clear logs` |
-        | `Run Keywords` | ${KW} | AND | @{KW WITH ARGS} |
-
-        Notice that the ``AND`` control argument must be used explicitly and
-        cannot itself come from a variable. If you need to use literal ``AND``
-        string as argument, you can either use variables or escape it with
-        a backslash like ``\\AND``.
-        """
-
-        return await self._async_gather_keywords(
-            self.builtIn._split_run_keywords(list(keywords))
-        )
-
-    async def _async_gather_keywords(self, iterable):
-        tasks = []
-        errors = []
-        try:
-            for kw, args in iterable:
-                try:
-                    task = self.builtIn.run_keyword(kw, *args)
-                    if not inspect.iscoroutine(task):
-                        raise DataError(f"Keyword '{kw}' is not async")
-                    tasks.append(task)
-                except ExecutionPassed as err:
-                    err.set_earlier_failures(errors)
-                    raise err
-                except ExecutionFailed as err:
-                    errors.extend(err.get_errors())
-                    if not err.can_continue(self.builtIn._context):
-                        break
-            if errors:
-                raise ExecutionFailures(errors)
-        except Exception as err:
-            for t in tasks:
-                t.close()
-            raise err
-        return await asyncio.gather(*tasks)
-
-    async def async_sleep(self, time_, reason=None):
-        """
-        Pauses the test executed for the given time asynchronously.
-        This is useful for allowing other coroutines to continue running in the
-        backgroud. Normal sleep blocks all execution.
-
-        ``time`` may be either a number or a time string. Time strings are in
-        a format such as ``1 day 2 hours 3 minutes 4 seconds 5milliseconds`` or
-        ``1d 2h 3m 4s 5ms``, and they are fully explained in an appendix of
-        Robot Framework User Guide. Providing a value without specifying minutes
-        or seconds, defaults to seconds.
-        Optional `reason` can be used to explain why
-        sleeping is necessary. Both the time slept and the reason are logged.
-
-        Examples:
-        | Sleep | 42                   |
-        | Sleep | 1.5                  |
-        | Sleep | 2 minutes 10 seconds |
-        | Sleep | 10s                  | Wait for a reply |
-        """
-
-        seconds = timestr_to_secs(time_)
-        # Python hangs with negative values
-        if seconds < 0:
-            seconds = 0
-        await self._async_sleep_in_parts(seconds)
-        self.builtIn.log("Slept %s" % secs_to_timestr(seconds))
-        if reason:
-            self.builtIn.log(reason)
-
-    async def _async_sleep_in_parts(self, seconds):
-        """
-        time.sleep can't be stopped in windows
-        to ensure that we can signal stop (with timeout)
-        split sleeping to small pieces
-        """
-
-        endtime = time.time() + float(seconds)
-        while True:
-            remaining = endtime - time.time()
-            if remaining <= 0:
-                break
-            await asyncio.sleep(min(remaining, 0.01))
-
-    async def async_create_task(self, name, *args):
-        """
-        Schedules an async keyword to run in background.
-
-        If keyword is not async, DataError will be raised.
-
-        Because the name of the keyword to execute is given as an argument, it
-        can be a variable and thus set dynamically, e.g. from a return value of
-        another keyword or from the command line.
-        """
-
-        task = self.builtIn.run_keyword(name, *args)
-        if not inspect.iscoroutine(task):
-            raise DataError(f"Keyword '{name}' is not async")
-        return asyncio.create_task(task)
-
-    async def async_await_task(self, task):
-        """
-        Get the result from a scheduled async task.
-
-        If obj is not a task, DataError will be raised.
-        """
-
-        if not inspect.isawaitable(task):
-            raise DataError("Obj is not an async Task")
-        return await task
+"""
+Utility functions to help using asyncio features.
+
+Some implementations used part of functions from the BuiltIn module from robot itself.
+"""
+
+
+import time
+import inspect
+import asyncio
+
+from robot.libraries.BuiltIn import BuiltIn
+from robot.utils.robottime import timestr_to_secs, secs_to_timestr
+from robot.errors import DataError, ExecutionPassed, ExecutionFailed, ExecutionFailures
+
+
+class AsyncioUtils:
+
+    def __init__(self) -> None:
+        try:
+            self.builtIn = BuiltIn()
+        except Exception:
+            self.builtIn = None
+
+    async def async_gather_keywords(self, *keywords):
+        """Executes all the given keywords concurrently.
+
+        This keyword is mainly useful to run multiple keywords concurrently
+        just like calling asyncio.gather() in python.
+        The keywords passed need to be async, else an error is raised.
+
+        By default all arguments are expected to be keywords to be executed.
+
+        Examples:
+        | `Run Keywords` | `Initialize database` | `Start servers` | `Clear logs` |
+        | `Run Keywords` | ${KW 1} | ${KW 2} |
+        | `Run Keywords` | @{KEYWORDS} |
+
+        Keywords can also be run with arguments using upper case ``AND`` as
+        a separator between keywords. The keywords are executed so that the
+        first argument is the first keyword and proceeding arguments until
+        the first ``AND`` are arguments to it. First argument after the first
+        ``AND`` is the second keyword and proceeding arguments until the next
+        ``AND`` are its arguments. And so on.
+
+        Examples:
+        | `Run Keywords` | `Initialize database` | db1 | AND | `Start servers` | server1 | server2 |
+        | `Run Keywords` | `Initialize database` | ${DB NAME} | AND | `Start servers` | @{SERVERS} | AND | `Clear logs` |
+        | `Run Keywords` | ${KW} | AND | @{KW WITH ARGS} |
+
+        Notice that the ``AND`` control argument must be used explicitly and
+        cannot itself come from a variable. If you need to use literal ``AND``
+        string as argument, you can either use variables or escape it with
+        a backslash like ``\\AND``.
+        """
+
+        return await self._async_gather_keywords(
+            self.builtIn._split_run_keywords(list(keywords))
+        )
+
+    async def _async_gather_keywords(self, iterable):
+        tasks = []
+        errors = []
+        try:
+            for kw, args in iterable:
+                try:
+                    task = self.builtIn.run_keyword(kw, *args)
+                    if not inspect.iscoroutine(task):
+                        raise DataError(f"Keyword '{kw}' is not async")
+                    tasks.append(task)
+                except ExecutionPassed as err:
+                    err.set_earlier_failures(errors)
+                    raise err
+                except ExecutionFailed as err:
+                    errors.extend(err.get_errors())
+                    if not err.can_continue(self.builtIn._context):
+                        break
+            if errors:
+                raise ExecutionFailures(errors)
+        except Exception as err:
+            for t in tasks:
+                t.close()
+            raise err
+        return await asyncio.gather(*tasks)
+
+    async def async_sleep(self, time_, reason=None):
+        """
+        Pauses the test executed for the given time asynchronously.
+        This is useful for allowing other coroutines to continue running in the
+        backgroud. Normal sleep blocks all execution.
+
+        ``time`` may be either a number or a time string. Time strings are in
+        a format such as ``1 day 2 hours 3 minutes 4 seconds 5milliseconds`` or
+        ``1d 2h 3m 4s 5ms``, and they are fully explained in an appendix of
+        Robot Framework User Guide. Providing a value without specifying minutes
+        or seconds, defaults to seconds.
+        Optional `reason` can be used to explain why
+        sleeping is necessary. Both the time slept and the reason are logged.
+
+        Examples:
+        | Sleep | 42                   |
+        | Sleep | 1.5                  |
+        | Sleep | 2 minutes 10 seconds |
+        | Sleep | 10s                  | Wait for a reply |
+        """
+
+        seconds = timestr_to_secs(time_)
+        # Python hangs with negative values
+        if seconds < 0:
+            seconds = 0
+        await self._async_sleep_in_parts(seconds)
+        self.builtIn.log("Slept %s" % secs_to_timestr(seconds))
+        if reason:
+            self.builtIn.log(reason)
+
+    async def _async_sleep_in_parts(self, seconds):
+        """
+        time.sleep can't be stopped in windows
+        to ensure that we can signal stop (with timeout)
+        split sleeping to small pieces
+        """
+
+        endtime = time.time() + float(seconds)
+        while True:
+            remaining = endtime - time.time()
+            if remaining <= 0:
+                break
+            await asyncio.sleep(min(remaining, 0.01))
+
+    async def async_create_task(self, name, *args):
+        """
+        Schedules an async keyword to run in background.
+
+        If keyword is not async, DataError will be raised.
+
+        Because the name of the keyword to execute is given as an argument, it
+        can be a variable and thus set dynamically, e.g. from a return value of
+        another keyword or from the command line.
+        """
+
+        task = self.builtIn.run_keyword(name, *args)
+        if not inspect.iscoroutine(task):
+            raise DataError(f"Keyword '{name}' is not async")
+        return asyncio.create_task(task)
+
+    async def async_await_task(self, task):
+        """
+        Get the result from a scheduled async task.
+
+        If obj is not a task, DataError will be raised.
+        """
+
+        if not inspect.isawaitable(task):
+            raise DataError("Obj is not an async Task")
+        return await task
```

### Comparing `robotframework_asyncio_utils-0.1.6/LICENSE` & `robotframework_asyncio_utils-0.1.7/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Ygor Pontelo
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Ygor Pontelo
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `robotframework_asyncio_utils-0.1.6/README.md` & `robotframework_asyncio_utils-0.1.7/README.md`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-## Description
-
-This library contains utility functions to use asyncio features from robot easier.
-
-## Requirements
-
-To use this library you need python >=3.8 and Robot Framework >=6.1.0
-
-## Installation
-
-```
-pip install robotframework-asyncio-utils
-```
-
-Once you installed, just put "Library    AsyncioUtils" in the settings section of your robot file.
-
-## Available Keywords
-
-- Async Gather Keywords
-- Async Sleep
-- Async Create Task
-- Async Await Task
-
-Each keyword has a doc string too.
-
-Probably more keywords will be added to cover more features from asyncio.
+## Description
+
+This library contains utility functions to use asyncio features from robot easier.
+
+## Requirements
+
+To use this library you need python >=3.8 and Robot Framework >=6.1.0
+
+## Installation
+
+```
+pip install robotframework-asyncio-utils
+```
+
+Once you installed, just put "Library    AsyncioUtils" in the settings section of your robot file.
+
+## Available Keywords
+
+- Async Gather Keywords
+- Async Sleep
+- Async Create Task
+- Async Await Task
+
+Each keyword has a doc string too.
+
+Probably more keywords will be added to cover more features from asyncio.
```

### Comparing `robotframework_asyncio_utils-0.1.6/PKG-INFO` & `robotframework_asyncio_utils-0.1.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: robotframework-asyncio-utils
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Home-page: https://github.com/ygorpontelo/robot-asyncio-utils
 License: MIT
 Author: Ygor Pontelo
 Author-email: ygorpontelo@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: robotframework (>=6.1.0,<7.0.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: robotframework (>=6.1.0)
 Description-Content-Type: text/markdown
 
 ## Description
 
 This library contains utility functions to use asyncio features from robot easier.
 
 ## Requirements
```

