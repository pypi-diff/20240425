# Comparing `tmp/facet-0.9.0.tar.gz` & `tmp/facet-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/facet-0.9.0.tar", last modified: Sat Jul 10 13:42:34 2021, max compression
+gzip compressed data, was "facet-0.9.1.tar", last modified: Tue Jan 11 17:11:01 2022, max compression
```

## Comparing `facet-0.9.0.tar` & `facet-0.9.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-07-10 13:42:34.000000 facet-0.9.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5390 2021-07-10 13:42:34.000000 facet-0.9.0/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-07-10 13:42:34.000000 facet-0.9.0/facet.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5390 2021-07-10 13:42:34.000000 facet-0.9.0/facet.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      183 2021-07-10 13:42:34.000000 facet-0.9.0/facet.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-07-10 13:42:34.000000 facet-0.9.0/facet.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       47 2021-07-10 13:42:34.000000 facet-0.9.0/facet.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        6 2021-07-10 13:42:34.000000 facet-0.9.0/facet.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     3846 2021-07-10 13:42:18.000000 facet-0.9.0/facet.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1072 2021-07-10 13:42:18.000000 facet-0.9.0/license.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      575 2021-07-10 13:42:34.000000 facet-0.9.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-07-10 13:42:18.000000 facet-0.9.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-01-11 17:11:01.606182 facet-0.9.1/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5390 2022-01-11 17:11:01.606182 facet-0.9.1/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-01-11 17:11:01.606182 facet-0.9.1/facet.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5390 2022-01-11 17:11:01.000000 facet-0.9.1/facet.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      183 2022-01-11 17:11:01.000000 facet-0.9.1/facet.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-01-11 17:11:01.000000 facet-0.9.1/facet.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       47 2022-01-11 17:11:01.000000 facet-0.9.1/facet.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        6 2022-01-11 17:11:01.000000 facet-0.9.1/facet.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3879 2022-01-11 17:10:46.000000 facet-0.9.1/facet.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1072 2022-01-11 17:10:46.000000 facet-0.9.1/license.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      575 2022-01-11 17:11:01.610180 facet-0.9.1/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2022-01-11 17:10:46.000000 facet-0.9.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `facet-0.9.0/PKG-INFO` & `facet-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facet
-Version: 0.9.0
+Version: 0.9.1
 Summary: service manager for asyncio
 Home-page: https://github.com/pohmelie/facet
 Author: pohmelie
 Author-email: multisosnooley@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `facet-0.9.0/facet.egg-info/PKG-INFO` & `facet-0.9.1/facet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facet
-Version: 0.9.0
+Version: 0.9.1
 Summary: service manager for asyncio
 Home-page: https://github.com/pohmelie/facet
 Author: pohmelie
 Author-email: multisosnooley@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `facet-0.9.0/facet.py` & `facet-0.9.1/facet.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 try:
     from asyncio import create_task
 except ImportError:
     from asyncio import ensure_future as create_task
 
 __all__ = ("ServiceMixin",)
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 version = tuple(map(int, __version__.split(".")))
 
 
 class ServiceMixin:
 
     __running = False
     __tasks = ()
@@ -99,15 +99,15 @@
         await self.__stop()
 
     def __task_callback(self, task):
         self.__tasks.discard(task)
         if task.cancelled():
             return
         exc = task.exception()
-        if exc:
+        if exc and not self.__exit_point.done():
             self.__exit_point.set_exception(exc)
 
     async def wait(self):
         await self.__exit_point
 
     async def run(self):
         async with self:
```

### Comparing `facet-0.9.0/license.txt` & `facet-0.9.1/license.txt`

 * *Files identical despite different names*

### Comparing `facet-0.9.0/setup.cfg` & `facet-0.9.1/setup.cfg`

 * *Files identical despite different names*

