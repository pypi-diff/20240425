# Comparing `tmp/glow-0.13.5.tar.gz` & `tmp/glow-0.13.6.tar.gz`

## Comparing `glow-0.13.5.tar` & `glow-0.13.6.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 glow-0.13.5/src/glow/__init__.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 glow-0.13.5/src/glow/_array.py
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 glow-0.13.5/src/glow/_coro.py
--rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 glow-0.13.5/src/glow/_debug.py
--rw-r--r--   0        0        0     9133 2020-02-02 00:00:00.000000 glow-0.13.5/src/glow/_ic.py
--rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 glow-0.13.5/src/glow/_import_hook.py
--rw-r--r--   0        0        0     6833 2020-02-02 00:00:00.000000 glow-0.13.5/src/glow/_more.py
--rw-r--r--   0        0        0    16339 2020-02-02 00:00:00.000000 glow-0.13.5/src/glow/_parallel.py
--rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 glow-0.13.5/src/glow/_parallel.pyi
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 glow-0.13.5/src/glow/_patch_len.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 glow-0.13.5/src/glow/_patch_print.py
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 glow-0.13.5/src/glow/_patch_scipy.py
--rw-r--r--   0        0        0     5762 2020-02-02 00:00:00.000000 glow-0.13.5/src/glow/_profile.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 glow-0.13.5/src/glow/_profile.pyi
--rw-r--r--   0        0        0     4746 2020-02-02 00:00:00.000000 glow-0.13.5/src/glow/_reduction.py
--rw-r--r--   0        0        0     3835 2020-02-02 00:00:00.000000 glow-0.13.5/src/glow/_repr.py
--rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 glow-0.13.5/src/glow/_sizeof.py
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 glow-0.13.5/src/glow/_thread_quota.py
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 glow-0.13.5/src/glow/_uuid.py
--rw-r--r--   0        0        0     7930 2020-02-02 00:00:00.000000 glow-0.13.5/src/glow/cli.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 glow-0.13.5/src/glow/cli.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.13.5/src/glow/py.typed
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 glow-0.13.5/src/glow/api/__init__.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 glow-0.13.5/src/glow/api/config.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 glow-0.13.5/src/glow/api/exporting.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 glow-0.13.5/src/glow/io/__init__.py
--rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 glow-0.13.5/src/glow/io/_sound.py
--rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 glow-0.13.5/src/glow/io/_svg.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 glow-0.13.5/src/glow/wrap/__init__.py
--rw-r--r--   0        0        0    10337 2020-02-02 00:00:00.000000 glow-0.13.5/src/glow/wrap/cache.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 glow-0.13.5/src/glow/wrap/cache.pyi
--rw-r--r--   0        0        0     7687 2020-02-02 00:00:00.000000 glow-0.13.5/src/glow/wrap/concurrency.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 glow-0.13.5/src/glow/wrap/concurrency.pyi
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 glow-0.13.5/src/glow/wrap/reusable.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 glow-0.13.5/src/glow/wrap/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.13.5/test/__init__.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 glow-0.13.5/test/test_api.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 glow-0.13.5/test/test_batch.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 glow-0.13.5/test/test_buffered.py
--rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 glow-0.13.5/test/test_cli.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 glow-0.13.5/test/test_iter.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 glow-0.13.5/test/test_shm.py
--rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 glow-0.13.5/test/test_thread_pool.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 glow-0.13.5/test/test_timed.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 glow-0.13.5/test/test_timer.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 glow-0.13.5/test/test_uuid.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 glow-0.13.5/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 glow-0.13.5/LICENSE
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 glow-0.13.5/README.md
--rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 glow-0.13.5/pyproject.toml
--rw-r--r--   0        0        0     4573 2020-02-02 00:00:00.000000 glow-0.13.5/PKG-INFO
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/__init__.py
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/_array.py
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/_coro.py
+-rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/_debug.py
+-rw-r--r--   0        0        0    12097 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/_ic.py
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/_import_hook.py
+-rw-r--r--   0        0        0     6833 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/_more.py
+-rw-r--r--   0        0        0    16339 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/_parallel.py
+-rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/_parallel.pyi
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/_patch_len.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/_patch_print.py
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/_patch_scipy.py
+-rw-r--r--   0        0        0     6346 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/_profile.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/_profile.pyi
+-rw-r--r--   0        0        0     4746 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/_reduction.py
+-rw-r--r--   0        0        0     3835 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/_repr.py
+-rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/_sizeof.py
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/_thread_quota.py
+-rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/_uuid.py
+-rw-r--r--   0        0        0     7930 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/cli.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/cli.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/py.typed
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/api/__init__.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/api/config.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/api/exporting.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/io/__init__.py
+-rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/io/_sound.py
+-rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/io/_svg.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/wrap/__init__.py
+-rw-r--r--   0        0        0    10337 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/wrap/cache.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/wrap/cache.pyi
+-rw-r--r--   0        0        0     7687 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/wrap/concurrency.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/wrap/concurrency.pyi
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/wrap/reusable.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/wrap/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.13.6/test/__init__.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 glow-0.13.6/test/test_api.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 glow-0.13.6/test/test_batch.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 glow-0.13.6/test/test_buffered.py
+-rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 glow-0.13.6/test/test_cli.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 glow-0.13.6/test/test_iter.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 glow-0.13.6/test/test_shm.py
+-rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 glow-0.13.6/test/test_thread_pool.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 glow-0.13.6/test/test_timed.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 glow-0.13.6/test/test_timer.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 glow-0.13.6/test/test_uuid.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 glow-0.13.6/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 glow-0.13.6/LICENSE
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 glow-0.13.6/README.md
+-rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 glow-0.13.6/pyproject.toml
+-rw-r--r--   0        0        0     5507 2020-02-02 00:00:00.000000 glow-0.13.6/PKG-INFO
```

### Comparing `glow-0.13.5/src/glow/__init__.py` & `glow-0.13.6/src/glow/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # flake8: noqa
 """Functional Python tools"""
 
 from importlib import import_module
 from typing import TYPE_CHECKING
 
 from . import _patch_len, _patch_print, _patch_scipy
-from ._array import aceil, afloor, around
+from ._array import aceil, afloor, apack, around
 from ._coro import as_actor, coroutine, summary
 from ._debug import lock_seed, trace, trace_module, whereami
 from ._import_hook import register_post_import_hook, when_imported
 from ._more import (as_iter, chunked, eat, groupby, ichunked, ilen, roundrobin,
                     windowed)
 from ._parallel import (buffered, get_executor, map_n, map_n_dict,
                         max_cpu_count, starmap_n)
@@ -40,16 +40,16 @@
 
 
 __all__ = [
     'Reusable', 'Uid', 'aceil', 'afloor', 'around', 'as_actor', 'as_iter',
     'buffered', 'call_once', 'chunked', 'coroutine', 'countable', 'eat',
     'get_executor', 'groupby', 'ic', 'ic_repr', 'ichunked', 'ilen',
     'lock_seed', 'mangle', 'map_n', 'map_n_dict', 'max_cpu_count', 'memoize',
-    'memprof', 'register_post_import_hook', 'repr_as_obj', 'roundrobin',
-    'shared_call', 'si', 'si_bin', 'sizeof', 'starmap_n', 'streaming',
-    'summary', 'threadlocal', 'time_this', 'timer', 'trace', 'trace_module',
-    'weak_memoize', 'when_imported', 'whereami', 'windowed'
+    'memprof', 'apack', 'register_post_import_hook', 'repr_as_obj',
+    'roundrobin', 'shared_call', 'si', 'si_bin', 'sizeof', 'starmap_n',
+    'streaming', 'summary', 'threadlocal', 'time_this', 'timer', 'trace',
+    'trace_module', 'weak_memoize', 'when_imported', 'whereami', 'windowed'
 ]
 
 _patch_print.apply()
 _patch_len.apply()
 _patch_scipy.apply()
```

### Comparing `glow-0.13.5/src/glow/_coro.py` & `glow-0.13.6/src/glow/_coro.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.5/src/glow/_debug.py` & `glow-0.13.6/src/glow/_debug.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.5/src/glow/_import_hook.py` & `glow-0.13.6/src/glow/_import_hook.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.5/src/glow/_more.py` & `glow-0.13.6/src/glow/_more.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.5/src/glow/_parallel.py` & `glow-0.13.6/src/glow/_parallel.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.5/src/glow/_parallel.pyi` & `glow-0.13.6/src/glow/_parallel.pyi`

 * *Files identical despite different names*

### Comparing `glow-0.13.5/src/glow/_patch_len.py` & `glow-0.13.6/src/glow/_patch_len.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.5/src/glow/_patch_print.py` & `glow-0.13.6/src/glow/_patch_print.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.5/src/glow/_patch_scipy.py` & `glow-0.13.6/src/glow/_patch_scipy.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.5/src/glow/_profile.py` & `glow-0.13.6/src/glow/_profile.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 __all__ = ['memprof', 'time_this', 'timer']
 
 import atexit
 from collections import defaultdict, deque
 from collections.abc import Callable, Iterator
-from contextlib import contextmanager
-from dataclasses import dataclass, field
+from contextlib import AbstractContextManager, contextmanager, nullcontext
 from functools import partial
 from itertools import accumulate, count
 from threading import get_ident
 from time import perf_counter_ns, process_time_ns, thread_time_ns
 from typing import TYPE_CHECKING
 
 from wrapt import ObjectProxy
@@ -43,27 +42,47 @@
             if name is None:
                 name = f'{whereami(2, 1)} line'
             sign = '+' if size >= 0 else ''
             print(f'{name} done: {sign}{si_bin(size)}')
 
 
 @contextmanager
-def timer(name_or_callback: str | Callable[[int], object] | None = None,
-          time: Callable[[], int] = perf_counter_ns,
-          /) -> Iterator[None]:
+def _timer_callback(callback: Callable[[int], object],
+                    time: Callable[[], int] = perf_counter_ns,
+                    /) -> Iterator[None]:
+    begin = time()
+    try:
+        yield
+    finally:
+        callback(time() - begin)
+
+
+@contextmanager
+def _timer_print(name: str | None = None,
+                 time: Callable[[], int] = perf_counter_ns,
+                 /) -> Iterator[None]:
     begin = time()
     try:
         yield
     finally:
         end = time()
-        if callable(name_or_callback):
-            name_or_callback(end - begin)
-        else:
-            name = name_or_callback or f'{whereami(2, 1)} line'
-            print(f'{name} done in {si((end - begin) / 1e9)}s')
+        name = name or f'{whereami(2, 1)} line'
+        print(f'{name} done in {si((end - begin) / 1e9)}s')
+
+
+def timer(name_or_callback: str | Callable[[int], object] | None = None,
+          time: Callable[[], int] = perf_counter_ns,
+          /,
+          *,
+          disable: bool = False) -> AbstractContextManager[None]:
+    if disable:
+        return nullcontext()
+    if callable(name_or_callback):
+        return _timer_callback(name_or_callback, time)
+    return _timer_print(name_or_callback, time)
 
 
 def _to_fname(obj) -> str:
     if not hasattr(obj, '__module__') or not hasattr(obj, '__qualname__'):
         obj = type(obj)
     if obj.__module__ == 'builtins':
         return obj.__qualname__
@@ -100,20 +119,20 @@
         self._get_max()
 
     def max(self) -> int:
         self._add_event(0)
         return self._get_max()
 
 
-@dataclass(frozen=True)
 class _Stat:
-    calls: count = field(default_factory=count)
-    nlwp: _Nlwp = field(default_factory=_Nlwp)
-    cpu_ns: _Times = field(default_factory=_Times)
-    all_ns: _Times = field(default_factory=_Times)
+    def __init__(self):
+        self.calls = count()
+        self.nlwp = _Nlwp()
+        self.cpu_ns = _Times()
+        self.all_ns = _Times()
 
     def __call__(self, op, *args, **kwargs):
         with self.nlwp, \
                 timer(self.all_ns.add), \
                 timer(self.cpu_ns.add, thread_time_ns):
             return op(*args, **kwargs)
 
@@ -194,17 +213,22 @@
             f'{busy/all_busy:6.2%}',
             f'{si(busy):>5s}s + {si(idle):>5s}s',
             name,
             tail,
             sep=' - ')
 
 
-def time_this(fn=None, /, *, name: str | None = None):
+def time_this(fn=None, /, *, name: str | None = None, disable: bool = False):
     """Log function and/or generator timings at program exit"""
     if fn is None:
-        return partial(time_this, name=name)
+        return partial(time_this, name=name, disable=disable)
+    if disable:
+        return fn
 
     if name is None:
         name = _to_fname(fn)
 
-    fn.log_timing = partial(_print_stats, name)
+    time_this.finalizers[fn] = fn.log_timing = partial(_print_stats, name)
     return _TimedCall(fn, _stats[name])
+
+
+time_this.finalizers = {}
```

### Comparing `glow-0.13.5/src/glow/_profile.pyi` & `glow-0.13.6/src/glow/_profile.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -6,21 +6,35 @@
 
 
 def memprof(name_or_callback: str | Callable[[float], object] | None = ...,
             /) -> AbstractContextManager[None]:
     ...
 
 
-def timer(name_or_callback: str | Callable[[int], object] | None = ...,
+@overload
+def timer(name: str | None = ...,
+          time: Callable[[], int] = ...,
+          /,
+          *,
+          disable: bool = ...) -> AbstractContextManager[None]:
+    ...
+
+
+@overload
+def timer(callback: Callable[[int], object] | None,
           time: Callable[[], int] = ...,
-          /) -> AbstractContextManager[None]:
+          /,
+          *,
+          disable: bool = ...) -> AbstractContextManager[None]:
     ...
 
 
 @overload
-def time_this(fn: _F, /, *, name: str | None = ...) -> _F:
+def time_this(fn: _F, /, *, name: str | None = ..., disable: bool = ...) -> _F:
     ...
 
 
 @overload
-def time_this(*, name: str | None = ...) -> Callable[[_F], _F]:
+def time_this(*,
+              name: str | None = ...,
+              disable: bool = ...) -> Callable[[_F], _F]:
     ...
```

### Comparing `glow-0.13.5/src/glow/_reduction.py` & `glow-0.13.6/src/glow/_reduction.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.5/src/glow/_repr.py` & `glow-0.13.6/src/glow/_repr.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.5/src/glow/_sizeof.py` & `glow-0.13.6/src/glow/_sizeof.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.5/src/glow/_thread_quota.py` & `glow-0.13.6/src/glow/_thread_quota.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.5/src/glow/_uuid.py` & `glow-0.13.6/src/glow/_uuid.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.5/src/glow/cli.py` & `glow-0.13.6/src/glow/cli.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.5/src/glow/cli.pyi` & `glow-0.13.6/src/glow/cli.pyi`

 * *Files identical despite different names*

### Comparing `glow-0.13.5/src/glow/api/config.py` & `glow-0.13.6/src/glow/api/config.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.5/src/glow/api/exporting.py` & `glow-0.13.6/src/glow/api/exporting.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.5/src/glow/io/_sound.py` & `glow-0.13.6/src/glow/io/_sound.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import numpy as np
 import numpy.typing as npt
 from tqdm.auto import tqdm
 
 from .. import chunked
 
-_Scalar_co = TypeVar('_Scalar_co', bound=np.generic, covariant=True)
+_Scalar_co = TypeVar('_Scalar_co', bound=np.number, covariant=True)
 
 
 def _play(arr: np.ndarray,
           rate: int,
           blocksize: int = 1024,
           bufsize: int = 20) -> None:
     """Plays audio from array. Supports interruption via Crtl-C."""
```

### Comparing `glow-0.13.5/src/glow/io/_svg.py` & `glow-0.13.6/src/glow/io/_svg.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.5/src/glow/wrap/cache.py` & `glow-0.13.6/src/glow/wrap/cache.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.5/src/glow/wrap/cache.pyi` & `glow-0.13.6/src/glow/wrap/cache.pyi`

 * *Files identical despite different names*

### Comparing `glow-0.13.5/src/glow/wrap/concurrency.py` & `glow-0.13.6/src/glow/wrap/concurrency.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.5/src/glow/wrap/concurrency.pyi` & `glow-0.13.6/src/glow/wrap/concurrency.pyi`

 * *Files identical despite different names*

### Comparing `glow-0.13.5/src/glow/wrap/reusable.py` & `glow-0.13.6/src/glow/wrap/reusable.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.5/src/glow/wrap/util.py` & `glow-0.13.6/src/glow/wrap/util.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.5/test/test_api.py` & `glow-0.13.6/test/test_api.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.5/test/test_batch.py` & `glow-0.13.6/test/test_batch.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.5/test/test_buffered.py` & `glow-0.13.6/test/test_buffered.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.5/test/test_cli.py` & `glow-0.13.6/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.5/test/test_iter.py` & `glow-0.13.6/test/test_iter.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.5/test/test_shm.py` & `glow-0.13.6/test/test_shm.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.5/test/test_thread_pool.py` & `glow-0.13.6/test/test_thread_pool.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.5/test/test_timed.py` & `glow-0.13.6/test/test_timed.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.5/test/test_uuid.py` & `glow-0.13.6/test/test_uuid.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.5/LICENSE` & `glow-0.13.6/LICENSE`

 * *Files identical despite different names*

### Comparing `glow-0.13.5/README.md` & `glow-0.13.6/README.md`

 * *Files identical despite different names*

### Comparing `glow-0.13.5/pyproject.toml` & `glow-0.13.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build]
 only-packages = true
 
 [project]
 name = "glow"
-version = "0.13.5"
+version = "0.13.6"
 description = "Functional Python tools"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 keywords = []
 authors = [
     {name = "Paul Maevskikh", email = "arquolo@gmail.com"},
```

