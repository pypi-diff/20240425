# Comparing `tmp/async-selective-queue-0.1.0.post0.tar.gz` & `tmp/async_selective_queue-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async-selective-queue-0.1.0.post0.tar", max compression
+gzip compressed data, was "async_selective_queue-0.1.1.tar", last modified: Wed Apr 24 22:10:00 2024, max compression
```

## Comparing `async-selective-queue-0.1.0.post0.tar` & `async_selective_queue-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2022-06-02 21:46:58.121471 async-selective-queue-0.1.0.post0/LICENSE
--rw-r--r--   0        0        0      604 2022-06-02 23:20:52.469992 async-selective-queue-0.1.0.post0/README.md
--rw-r--r--   0        0        0     3665 2022-06-02 23:00:52.550233 async-selective-queue-0.1.0.post0/async_selective_queue.py
--rw-r--r--   0        0        0      839 2022-06-02 23:23:19.269616 async-selective-queue-0.1.0.post0/pyproject.toml
--rw-r--r--   0        0        0     1148 2022-06-02 23:23:35.287302 async-selective-queue-0.1.0.post0/setup.py
--rw-r--r--   0        0        0     1264 2022-06-02 23:23:35.287649 async-selective-queue-0.1.0.post0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-24 22:09:39.983004 async_selective_queue-0.1.1/LICENSE
+-rw-r--r--   0        0        0      628 2024-04-24 22:09:39.983004 async_selective_queue-0.1.1/README.md
+-rw-r--r--   0        0        0     3716 2024-04-24 22:09:39.983004 async_selective_queue-0.1.1/async_selective_queue.py
+-rw-r--r--   0        0        0     1443 2024-04-24 22:10:00.398941 async_selective_queue-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2881 2024-04-24 22:09:39.983004 async_selective_queue-0.1.1/tests/test_msg_queue.py
+-rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 async_selective_queue-0.1.1/PKG-INFO
```

### Comparing `async-selective-queue-0.1.0.post0/LICENSE` & `async_selective_queue-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `async-selective-queue-0.1.0.post0/README.md` & `async_selective_queue-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Async Selective Queue
 
 [![PyPI](https://img.shields.io/pypi/v/async-selective-queue)](https://pypi.org/project/async-selective-queue/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/async-selective-queue)
-![GitHub Workflow Status](https://img.shields.io/github/workflow/status/dbluhm/async-selective-queue/Tests?label=tests)
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dbluhm/async-selective-queue/tests.yml?branch=main&label=tests)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 Python library for an asynchronous queue with the ability to selectively
 retrieve elements from the queue.
```

### Comparing `async-selective-queue-0.1.0.post0/async_selective_queue.py` & `async_selective_queue-0.1.1/async_selective_queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+"""Async Selective Queue."""
+
 import asyncio
 from typing import Callable, Generic, List, Optional, Sequence, TypeVar
 
 
 QueueEntry = TypeVar("QueueEntry")
 Select = Callable[[QueueEntry], bool]
 
 
 class AsyncSelectiveQueue(Generic[QueueEntry]):
     """Asynchronous Queue implementation with selective retrieval of entries."""
 
     def __init__(self):
+        """Initialize the queue."""
         self._queue: List[QueueEntry] = []
         self._cond: asyncio.Condition = asyncio.Condition()
 
     def _first_matching_index(self, select: Select):
         for index, entry in enumerate(self._queue):
             if select(entry):
                 return index
@@ -58,15 +61,15 @@
     def get_all(self, select: Optional[Select] = None) -> Sequence[QueueEntry]:
         """Return all entries matching a given select."""
         entries = []
         if not self._queue:
             return entries
 
         if not select:
-            entries = [entry for entry in self._queue]
+            entries = list(self._queue)
             self._queue.clear()
             return entries
 
         # Store entries that didn't match in the order they are seen
         filtered: List[QueueEntry] = []
         for entry in self._queue:
             if select(entry):
```

### Comparing `async-selective-queue-0.1.0.post0/setup.py` & `async_selective_queue-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: async-selective-queue
+Version: 0.1.1
+Summary: Async queue with selective retrieval
+Keywords: async,queue,conditional
+Home-page: https://github.com/dbluhm/async-selective-queue
+Author-Email: Daniel Bluhm <dbluhm@pm.me>
+License: Apache-2.0
+Project-URL: Homepage, https://github.com/dbluhm/async-selective-queue
+Requires-Python: <4.0,>=3.9
+Description-Content-Type: text/markdown
 
-modules = \
-['async_selective_queue']
-setup_kwargs = {
-    'name': 'async-selective-queue',
-    'version': '0.1.0.post0',
-    'description': 'Async queue with selective retrieval',
-    'long_description': '# Async Selective Queue\n\n[![PyPI](https://img.shields.io/pypi/v/async-selective-queue)](https://pypi.org/project/async-selective-queue/)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/async-selective-queue)\n![GitHub Workflow Status](https://img.shields.io/github/workflow/status/dbluhm/async-selective-queue/Tests?label=tests)\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)\n\nPython library for an asynchronous queue with the ability to selectively\nretrieve elements from the queue.\n',
-    'author': 'Daniel Bluhm',
-    'author_email': 'dbluhm@pm.me',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/dbluhm/async-selective-queue',
-    'py_modules': modules,
-    'python_requires': '>=3.7,<4.0',
-}
+# Async Selective Queue
 
+[![PyPI](https://img.shields.io/pypi/v/async-selective-queue)](https://pypi.org/project/async-selective-queue/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/async-selective-queue)
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dbluhm/async-selective-queue/tests.yml?branch=main&label=tests)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
-setup(**setup_kwargs)
+Python library for an asynchronous queue with the ability to selectively
+retrieve elements from the queue.
```

