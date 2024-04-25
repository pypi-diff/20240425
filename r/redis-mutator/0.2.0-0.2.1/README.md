# Comparing `tmp/redis_mutator-0.2.0.tar.gz` & `tmp/redis_mutator-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_mutator-0.2.0.tar", max compression
+gzip compressed data, was "redis_mutator-0.2.1.tar", max compression
```

## Comparing `redis_mutator-0.2.0.tar` & `redis_mutator-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1684 2024-04-25 07:06:59.241545 redis_mutator-0.2.0/README.md
--rw-r--r--   0        0        0      297 2024-04-25 07:10:31.002372 redis_mutator-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       91 2024-04-25 03:48:09.782197 redis_mutator-0.2.0/redis_mutator/__init__.py
--rw-r--r--   0        0        0     2778 2024-04-25 05:54:28.822062 redis_mutator-0.2.0/redis_mutator/method_names.py
--rw-r--r--   0        0        0     1290 2024-04-25 03:00:33.262043 redis_mutator-0.2.0/redis_mutator/mutate.py
--rw-r--r--   0        0        0     4198 2024-04-25 07:09:35.934159 redis_mutator-0.2.0/redis_mutator/redis_mutator.py
--rw-r--r--   0        0        0     2223 1970-01-01 00:00:00.000000 redis_mutator-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1684 2024-04-25 07:06:59.241545 redis_mutator-0.2.1/README.md
+-rw-r--r--   0        0        0      297 2024-04-25 07:12:54.134918 redis_mutator-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       91 2024-04-25 03:48:09.782197 redis_mutator-0.2.1/redis_mutator/__init__.py
+-rw-r--r--   0        0        0     2778 2024-04-25 05:54:28.822062 redis_mutator-0.2.1/redis_mutator/method_names.py
+-rw-r--r--   0        0        0     1290 2024-04-25 03:00:33.262043 redis_mutator-0.2.1/redis_mutator/mutate.py
+-rw-r--r--   0        0        0     4144 2024-04-25 07:12:46.882891 redis_mutator-0.2.1/redis_mutator/redis_mutator.py
+-rw-r--r--   0        0        0     2223 1970-01-01 00:00:00.000000 redis_mutator-0.2.1/PKG-INFO
```

### Comparing `redis_mutator-0.2.0/README.md` & `redis_mutator-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `redis_mutator-0.2.0/redis_mutator/method_names.py` & `redis_mutator-0.2.1/redis_mutator/method_names.py`

 * *Files identical despite different names*

### Comparing `redis_mutator-0.2.0/redis_mutator/mutate.py` & `redis_mutator-0.2.1/redis_mutator/mutate.py`

 * *Files identical despite different names*

### Comparing `redis_mutator-0.2.0/redis_mutator/redis_mutator.py` & `redis_mutator-0.2.1/redis_mutator/redis_mutator.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,17 +43,16 @@
 
             if name in self.__mutations:
                 value = self.__mutations[name](*args, **kwargs)
             else:
                 value = raw(*args, **kwargs)
 
             if name in self.__postfixes:
-                for hook in self.__postfixes:
-                    for hook in self.__postfixes[name]:
-                        hook(value, args, kwargs)
+                for hook in self.__postfixes[name]:
+                    hook(value, args, kwargs)
 
             return value
 
         setattr(self.__redis, name, wrapper)
 
     def prefix(self, hook: Callable):
         for name in self.__names:
```

### Comparing `redis_mutator-0.2.0/PKG-INFO` & `redis_mutator-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-mutator
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: MisterNyan
 Author-email: michael.edmund.wong@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

