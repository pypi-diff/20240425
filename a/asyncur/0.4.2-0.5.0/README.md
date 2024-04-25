# Comparing `tmp/asyncur-0.4.2.tar.gz` & `tmp/asyncur-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncur-0.4.2.tar", max compression
+gzip compressed data, was "asyncur-0.5.0.tar", max compression
```

## Comparing `asyncur-0.4.2.tar` & `asyncur-0.5.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1068 2023-09-07 09:10:14.471122 asyncur-0.4.2/LICENSE
--rw-r--r--   0        0        0     1877 2024-03-28 09:03:58.829102 asyncur-0.4.2/README.md
--rw-r--r--   0        0        0      334 2024-03-28 08:55:33.030394 asyncur-0.4.2/asyncur/__init__.py
--rw-r--r--   0        0        0     3552 2024-04-08 08:11:37.298520 asyncur-0.4.2/asyncur/aio.py
--rw-r--r--   0        0        0        0 2023-09-19 11:58:47.096600 asyncur-0.4.2/asyncur/py.typed
--rw-r--r--   0        0        0     4084 2024-04-05 15:00:30.881587 asyncur-0.4.2/asyncur/timing.py
--rw-r--r--   0        0        0      927 2023-10-26 09:32:47.265695 asyncur-0.4.2/asyncur/xls.py
--rw-r--r--   0        0        0      892 2024-04-08 07:30:36.372766 asyncur-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     2590 1970-01-01 00:00:00.000000 asyncur-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-09-07 09:10:14.471122 asyncur-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1870 2024-04-25 08:31:01.627968 asyncur-0.5.0/README.md
+-rw-r--r--   0        0        0      380 2024-04-25 03:15:51.639066 asyncur-0.5.0/asyncur/__init__.py
+-rw-r--r--   0        0        0     4438 2024-04-18 07:08:46.175588 asyncur-0.5.0/asyncur/aio.py
+-rw-r--r--   0        0        0        0 2023-09-19 11:58:47.096600 asyncur-0.5.0/asyncur/py.typed
+-rw-r--r--   0        0        0     4084 2024-04-05 15:00:30.881587 asyncur-0.5.0/asyncur/timing.py
+-rw-r--r--   0        0        0      859 2024-04-18 09:24:22.041437 asyncur-0.5.0/asyncur/utils.py
+-rw-r--r--   0        0        0      927 2023-10-26 09:32:47.265695 asyncur-0.5.0/asyncur/xls.py
+-rw-r--r--   0        0        0      976 2024-04-25 03:22:46.699512 asyncur-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2660 1970-01-01 00:00:00.000000 asyncur-0.5.0/PKG-INFO
```

### Comparing `asyncur-0.4.2/LICENSE` & `asyncur-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncur-0.4.2/README.md` & `asyncur-0.5.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # asyncur
 ![Python Versions](https://img.shields.io/pypi/pyversions/asyncur)
 [![LatestVersionInPypi](https://img.shields.io/pypi/v/asyncur.svg?style=flat)](https://pypi.python.org/pypi/asyncur)
 [![GithubActionResult](https://github.com/waketzheng/asyncur/workflows/ci/badge.svg)](https://github.com/waketzheng/asyncur/actions?query=workflow:ci)
 [![Coverage Status](https://coveralls.io/repos/github/waketzheng/asyncur/badge.svg?branch=main)](https://coveralls.io/github/waketzheng/asyncur?branch=main)
 ![Mypy coverage](https://img.shields.io/badge/mypy-100%25-green.svg)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
-[![code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Some async functions that using anyio, and toolkit for excel read.
 
 ## Installation
 
 <div class="termy">
 
@@ -21,20 +20,24 @@
 Or use poetry:
 ```console
 poetry add asyncur
 ```
 
 ## Usage
 
-- gather/run_async
+- bulk_gather/gather/run_async
 ```py
 >>> from asyncur import gather, run_async
 >>> async def foo():
 ...     return 1
 ...
+>>> await bulk_gather([foo(), foo()], limit=200)
+(1, 1)
+>>> await gather(foo(), foo())
+(1, 1)
 >>> run_async(gather(foo(), foo()))
 (1, 1)
 ```
 - timeit
 ```py
 >>> import time
 >>> import anyio
```

### Comparing `asyncur-0.4.2/asyncur/aio.py` & `asyncur-0.5.0/asyncur/aio.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,91 +1,119 @@
 import sys
 from contextlib import asynccontextmanager
-from typing import Any, Callable, Coroutine, Sequence
+from typing import Any, Awaitable, Callable, Coroutine, Sequence, TypeVar
+
+if sys.version_info >= (3, 11):
+    from typing import TypeVarTuple, Unpack
+else:
+    from exceptiongroup import ExceptionGroup  # pragma: no cover
+    from typing_extensions import TypeVarTuple, Unpack  # pragma: no cover
 
 import anyio
 
-if sys.version_info < (3, 11):
-    from exceptiongroup import ExceptionGroup  # pragma: no cover
+T_Retval = TypeVar("T_Retval")
+PosArgsT = TypeVarTuple("PosArgsT")
 
 
-def ensure_afunc(coro: Coroutine | Callable) -> Callable:
+def ensure_afunc(
+    coro: Coroutine[None, None, T_Retval] | Callable[..., Awaitable[T_Retval]],
+) -> Callable[..., Awaitable[T_Retval]]:
     """Wrap coroutine to be async function"""
     if callable(coro):
         return coro
 
     async def do_await():
         return await coro
 
     return do_await
 
 
-def run_async(coro: Coroutine | Callable) -> Any:
+def run_async(
+    coro: Coroutine[None, None, T_Retval] | Callable[..., Awaitable[T_Retval]],
+) -> T_Retval:
     """Compare with anyio.run and asyncio.run
 
     Usage::
         >>> async def afunc(n=1):
         ...     return n
         ...
         >>> run_async(afunc)  # get the same result as: await afunc()
         1
         >>> run_async(afunc(2))  # get the same result as: await afunc(2)
         2
     """
     return anyio.run(ensure_afunc(coro))
 
 
-async def gather(*coros: Coroutine) -> tuple:
-    """Similar like asyncio.gather"""
-    return await bulk_gather(coros)
+def run(
+    func: (
+        Coroutine[None, None, T_Retval]
+        | Callable[[Unpack[PosArgsT]], Awaitable[T_Retval]]
+    ),
+    *args: Unpack[PosArgsT],
+    backend: str = "asyncio",
+    backend_options: dict[str, Any] | None = None,
+) -> T_Retval:
+    if not callable(func):
+
+        async def do_await() -> T_Retval:
+            return await func
+
+        return anyio.run(do_await, backend=backend, backend_options=backend_options)
+    return anyio.run(func, *args, backend=backend, backend_options=backend_options)
 
 
 async def bulk_gather(
-    coros: Sequence[Coroutine], bulk=0, wait_last=False, raises=True
+    coros: Sequence[Coroutine], limit=0, wait_last=False, raises=True
 ) -> tuple:
     """Similar like asyncio.gather, if bulk is not zero, running tasks will limit to {bulk} every moment.
 
     :param coros: Coroutines
-    :param bulk: running tasks limit number, set 0 to be unlimit
+    :param limit: running tasks limit number, set 0 to be unlimit
     :param wait_last: if True, wait last bulk tasks to complete then start new task group, else use anyio.CapacityLimiter to limit task number
     :param raises: if True, raise Exception when coroutine failed, else return None
     """
     total = len(coros)
     results = [None] * total
 
     async def runner(coro, i) -> None:
         results[i] = await coro
 
     async def limited_runner(coro, i, limiter) -> None:
         async with limiter:
             results[i] = await coro
 
     try:
-        if bulk:
+        if limit:
             if wait_last:
-                for start in range(0, total, bulk):
+                for start in range(0, total, limit):
                     async with anyio.create_task_group() as tg:
-                        for index, coro in enumerate(coros[start : start + bulk]):
+                        for index, coro in enumerate(coros[start : start + limit]):
                             tg.start_soon(runner, coro, start + index)
             else:
-                limiter = anyio.CapacityLimiter(bulk)
+                limiter = anyio.CapacityLimiter(limit)
                 async with anyio.create_task_group() as tg:
                     for i, coro in enumerate(coros):
                         tg.start_soon(limited_runner, coro, i, limiter)
         else:
             async with anyio.create_task_group() as tg:
                 for i, coro in enumerate(coros):
                     tg.start_soon(runner, coro, i)
     except ExceptionGroup as e:
         if raises:
             raise e.exceptions[0]
 
     return tuple(results)
 
 
+async def gather(*coros: Coroutine) -> tuple:
+    """Similar like asyncio.gather"""
+    return await bulk_gather(coros)
+
+
 @asynccontextmanager
 async def start_tasks(coro: Coroutine | Callable, *more: Coroutine | Callable):
     """Make it easy to convert asyncio.create_task
 
     Usage:
 
     .. code-block:: python3
```

### Comparing `asyncur-0.4.2/asyncur/timing.py` & `asyncur-0.5.0/asyncur/timing.py`

 * *Files identical despite different names*

### Comparing `asyncur-0.4.2/asyncur/xls.py` & `asyncur-0.5.0/asyncur/xls.py`

 * *Files identical despite different names*

### Comparing `asyncur-0.4.2/PKG-INFO` & `asyncur-0.5.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: asyncur
-Version: 0.4.2
+Version: 0.5.0
 Summary: Async functions to compare with anyio and asyncio, and toolkit to read excel with async/await.
 Author: Waket Zheng
 Author-email: waketzheng@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: xls
 Requires-Dist: anyio (>=3.7.1)
 Requires-Dist: exceptiongroup (>=1.2.0) ; python_version < "3.11"
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0) ; extra == "xls"
-Requires-Dist: pandas (>=2.2.1,<3.0.0) ; extra == "xls"
+Requires-Dist: pandas (>=2.2.2,<3.0.0) ; extra == "xls"
+Requires-Dist: typing-extensions (>=4.11.0,<5.0.0) ; python_version < "3.11"
 Description-Content-Type: text/markdown
 
 # asyncur
 ![Python Versions](https://img.shields.io/pypi/pyversions/asyncur)
 [![LatestVersionInPypi](https://img.shields.io/pypi/v/asyncur.svg?style=flat)](https://pypi.python.org/pypi/asyncur)
 [![GithubActionResult](https://github.com/waketzheng/asyncur/workflows/ci/badge.svg)](https://github.com/waketzheng/asyncur/actions?query=workflow:ci)
 [![Coverage Status](https://coveralls.io/repos/github/waketzheng/asyncur/badge.svg?branch=main)](https://coveralls.io/github/waketzheng/asyncur?branch=main)
 ![Mypy coverage](https://img.shields.io/badge/mypy-100%25-green.svg)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
-[![code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Some async functions that using anyio, and toolkit for excel read.
 
 ## Installation
 
 <div class="termy">
 
@@ -39,20 +39,24 @@
 Or use poetry:
 ```console
 poetry add asyncur
 ```
 
 ## Usage
 
-- gather/run_async
+- bulk_gather/gather/run_async
 ```py
 >>> from asyncur import gather, run_async
 >>> async def foo():
 ...     return 1
 ...
+>>> await bulk_gather([foo(), foo()], limit=200)
+(1, 1)
+>>> await gather(foo(), foo())
+(1, 1)
 >>> run_async(gather(foo(), foo()))
 (1, 1)
 ```
 - timeit
 ```py
 >>> import time
 >>> import anyio
```

