# Comparing `tmp/clovers-0.1.4.post1.tar.gz` & `tmp/clovers-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clovers-0.1.4.post1.tar", max compression
+gzip compressed data, was "clovers-0.1.5.tar", max compression
```

## Comparing `clovers-0.1.4.post1.tar` & `clovers-0.1.5.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0        0 2024-04-15 12:37:36.317298 clovers-0.1.4.post1/clovers/__init__.py
--rw-r--r--   0        0        0     4524 2024-04-23 16:15:55.123859 clovers-0.1.4.post1/clovers/core/adapter.py
--rw-r--r--   0        0        0      582 2024-04-15 03:01:44.120813 clovers-0.1.4.post1/clovers/core/config.py
--rw-r--r--   0        0        0     6659 2024-04-23 17:07:21.079825 clovers-0.1.4.post1/clovers/core/plugin.py
--rw-r--r--   0        0        0     2774 2024-04-15 02:23:00.885679 clovers-0.1.4.post1/clovers/utils/library.py
--rw-r--r--   0        0        0    10961 2024-04-16 04:46:17.581644 clovers-0.1.4.post1/clovers/utils/linecard.py
--rw-r--r--   0        0        0     1884 2024-04-15 08:48:00.582248 clovers-0.1.4.post1/clovers/utils/tools.py
--rw-r--r--   0        0        0     1086 2024-04-15 03:18:25.255783 clovers-0.1.4.post1/LICENSE
--rw-r--r--   0        0        0      647 2024-04-23 17:08:39.503342 clovers-0.1.4.post1/pyproject.toml
--rw-r--r--   0        0        0    10284 2024-04-23 16:13:55.973406 clovers-0.1.4.post1/README.md
--rw-r--r--   0        0        0    10633 1970-01-01 00:00:00.000000 clovers-0.1.4.post1/PKG-INFO
+-rw-r--r--   0        0        0     2975 2024-04-25 16:17:20.354668 clovers-0.1.5/clovers/__init__.py
+-rw-r--r--   0        0        0     3250 2024-04-25 15:57:07.509856 clovers-0.1.5/clovers/core/adapter.py
+-rw-r--r--   0        0        0      582 2024-04-15 03:01:44.120813 clovers-0.1.5/clovers/core/config.py
+-rw-r--r--   0        0        0       57 2024-04-25 15:35:33.878533 clovers-0.1.5/clovers/core/logger.py
+-rw-r--r--   0        0        0     6815 2024-04-25 15:57:43.990068 clovers-0.1.5/clovers/core/plugin.py
+-rw-r--r--   0        0        0     2774 2024-04-15 02:23:00.885679 clovers-0.1.5/clovers/utils/library.py
+-rw-r--r--   0        0        0    10961 2024-04-16 04:46:17.581644 clovers-0.1.5/clovers/utils/linecard.py
+-rw-r--r--   0        0        0     1884 2024-04-15 08:48:00.582248 clovers-0.1.5/clovers/utils/tools.py
+-rw-r--r--   0        0        0     1086 2024-04-15 03:18:25.255783 clovers-0.1.5/LICENSE
+-rw-r--r--   0        0        0      645 2024-04-25 14:38:39.377101 clovers-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0    10284 2024-04-23 16:13:55.973406 clovers-0.1.5/README.md
+-rw-r--r--   0        0        0    10627 1970-01-01 00:00:00.000000 clovers-0.1.5/PKG-INFO
```

### Comparing `clovers-0.1.4.post1/clovers/core/config.py` & `clovers-0.1.5/clovers/core/config.py`

 * *Files identical despite different names*

### Comparing `clovers-0.1.4.post1/clovers/core/plugin.py` & `clovers-0.1.5/clovers/core/plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import importlib
-import traceback
 import time
 import re
 from pathlib import Path
 from collections.abc import Callable, Coroutine, Iterable, Sequence
+from .logger import logger
 
 
 class PluginError(Exception):
     def __init__(self, message: str):
         super().__init__(message)
 
 
@@ -40,38 +40,42 @@
         return await self.func(event)
 
 
 PluginCommands = str | set[str] | re.Pattern | None
 
 
 class Plugin:
-    NO_BUILD = lambda x: x
-
     def __init__(
         self,
         name: str = "",
-        build_event=NO_BUILD,
-        build_result=NO_BUILD,
+        build_event=None,
+        build_result=None,
     ) -> None:
         self.name: str = name
         self.handles: dict[int, Handle] = {}
         self.command_dict: dict[str, set[int]] = {}
         self.regex_dict: dict[re.Pattern, set[int]] = {}
         self.temp_handles: dict[str, tuple[float, Handle]] = {}
         self.startup_tasklist: list[Coroutine] = []
         self.shutdown_tasklist: list[Coroutine] = []
-        self.build_event: Callable = build_event
-        self.build_result: Callable = build_result
+        self.build_event: Callable | None = build_event
+        self.build_result: Callable | None = build_result
 
     def handle_warpper(self, func: Callable[..., Coroutine]):
-        async def wrapper(event: Event) -> Result | None:
-            if result := await func(self.build_event(event)):
-                return self.build_result(result)
+        if build_event := self.build_event:
+            func = lambda e: func(build_event(e))
+        if build_result := self.build_result:
+
+            async def wrapper(event):
+                if result := await func(event):
+                    return build_result(result)
 
-        return wrapper
+            return wrapper
+        else:
+            return lambda e: func(e)
 
     def commands_register(self, commands: PluginCommands, key: int):
         if not commands:
             self.command_dict.setdefault("", set()).add(key)
         elif isinstance(commands, set):
             for command in commands:
                 self.command_dict.setdefault(command, set()).add(key)
@@ -96,30 +100,25 @@
             self.handles[key] = handle
 
         return decorator
 
     def temp_handle(
         self,
         key: str,
-        timeout: float | int = 30.0,
         extra_args: Iterable[str] = [],
         get_extra_args: Iterable[str] = [],
+        timeout: float | int = 30.0,
     ):
 
         def decorator(func: Callable[..., Coroutine]):
-
             def finish():
                 del self.temp_handles[key]
 
-            async def wrapper(event: Event):
-                if result := await func(self.build_event(event), finish):
-                    return self.build_result(result)
-
             handle = Handle(extra_args, get_extra_args)
-            handle.func = wrapper
+            handle.func = self.handle_warpper(lambda e: func(e, finish))
             self.temp_handles[key] = time.time() + timeout, handle
 
         return decorator
 
     def startup(self, func: Callable[[], Coroutine]):
         """注册一个启动任务"""
         self.startup_tasklist.append(func())
@@ -169,20 +168,24 @@
 class PluginLoader:
     def __init__(self, plugins_path: str | Path | None = None, plugins_list: list[str] = []) -> None:
         self.plugins_path: Path | None = None if plugins_path is None else Path(plugins_path)
         self.plugins_list: list = plugins_list
 
     @staticmethod
     def load(name: str) -> Plugin | None:
-        print(f"【loading plugin】 {name} ...")
+        logger.info(f"【loading plugin】 {name} ...")
         try:
             module = importlib.import_module(name)
-            return getattr(module, "__plugin__", None)
-        except ImportError:
-            traceback.print_exc()
+            plugin = getattr(module, "__plugin__", None)
+            if not isinstance(plugin, Plugin):
+                return
+            plugin.name = plugin.name or name
+            return plugin
+        except:
+            logger.exception(name)
 
     def plugins_from_path(self):
         if self.plugins_path is None:
             return []
         plugins_path = ".".join(self.plugins_path.relative_to(Path()).parts)
         plugins = []
         for x in self.plugins_path.iterdir():
```

### Comparing `clovers-0.1.4.post1/clovers/utils/library.py` & `clovers-0.1.5/clovers/utils/library.py`

 * *Files identical despite different names*

### Comparing `clovers-0.1.4.post1/clovers/utils/linecard.py` & `clovers-0.1.5/clovers/utils/linecard.py`

 * *Files identical despite different names*

### Comparing `clovers-0.1.4.post1/clovers/utils/tools.py` & `clovers-0.1.5/clovers/utils/tools.py`

 * *Files identical despite different names*

### Comparing `clovers-0.1.4.post1/LICENSE` & `clovers-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `clovers-0.1.4.post1/pyproject.toml` & `clovers-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clovers"
-version = "0.1.4r1"
+version = "0.1.5"
 description = ""
 authors = ["KarisAya <1048827424@qq.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 toml = "^0.10.2"
```

### Comparing `clovers-0.1.4.post1/README.md` & `clovers-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `clovers-0.1.4.post1/PKG-INFO` & `clovers-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clovers
-Version: 0.1.4.post1
+Version: 0.1.5
 Summary: 
 Author: KarisAya
 Author-email: 1048827424@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

