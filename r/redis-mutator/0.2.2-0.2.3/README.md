# Comparing `tmp/redis_mutator-0.2.2.tar.gz` & `tmp/redis_mutator-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_mutator-0.2.2.tar", max compression
+gzip compressed data, was "redis_mutator-0.2.3.tar", max compression
```

## Comparing `redis_mutator-0.2.2.tar` & `redis_mutator-0.2.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1684 2024-04-25 07:06:59.241545 redis_mutator-0.2.2/README.md
--rw-r--r--   0        0        0      297 2024-04-25 07:15:00.651395 redis_mutator-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       91 2024-04-25 03:48:09.782197 redis_mutator-0.2.2/redis_mutator/__init__.py
--rw-r--r--   0        0        0     2778 2024-04-25 05:54:28.822062 redis_mutator-0.2.2/redis_mutator/method_names.py
--rw-r--r--   0        0        0     1312 2024-04-25 07:14:53.523368 redis_mutator-0.2.2/redis_mutator/mutate.py
--rw-r--r--   0        0        0     2928 2024-04-25 07:14:48.547350 redis_mutator-0.2.2/redis_mutator/redis_mutator.py
--rw-r--r--   0        0        0     2223 1970-01-01 00:00:00.000000 redis_mutator-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1684 2024-04-25 07:06:59.241545 redis_mutator-0.2.3/README.md
+-rw-r--r--   0        0        0      297 2024-04-25 07:25:43.121766 redis_mutator-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0       91 2024-04-25 03:48:09.782197 redis_mutator-0.2.3/redis_mutator/__init__.py
+-rw-r--r--   0        0        0     2778 2024-04-25 05:54:28.822062 redis_mutator-0.2.3/redis_mutator/method_names.py
+-rw-r--r--   0        0        0     1312 2024-04-25 07:14:53.523368 redis_mutator-0.2.3/redis_mutator/mutate.py
+-rw-r--r--   0        0        0     2977 2024-04-25 07:24:33.345511 redis_mutator-0.2.3/redis_mutator/redis_mutator.py
+-rw-r--r--   0        0        0     2223 1970-01-01 00:00:00.000000 redis_mutator-0.2.3/PKG-INFO
```

### Comparing `redis_mutator-0.2.2/README.md` & `redis_mutator-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `redis_mutator-0.2.2/redis_mutator/method_names.py` & `redis_mutator-0.2.3/redis_mutator/method_names.py`

 * *Files identical despite different names*

### Comparing `redis_mutator-0.2.2/redis_mutator/mutate.py` & `redis_mutator-0.2.3/redis_mutator/mutate.py`

 * *Files identical despite different names*

### Comparing `redis_mutator-0.2.2/redis_mutator/redis_mutator.py` & `redis_mutator-0.2.3/redis_mutator/redis_mutator.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 
     def __wrap(self, name: str):
         raw = getattr(self.__redis, name)
 
         def wrapper(*args, **kwargs):
             if name in self.__prefixes:
                 for hook in self.__prefixes[name]:
-                    hook(*args, **kwargs)
+                    if hook(*args, **kwargs) == False:
+                        return None
 
             value = None
 
             if name in self.__mutations:
                 value = self.__mutations[name](*args, **kwargs)
             else:
                 value = raw(*args, **kwargs)
```

### Comparing `redis_mutator-0.2.2/PKG-INFO` & `redis_mutator-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-mutator
-Version: 0.2.2
+Version: 0.2.3
 Summary: 
 Author: MisterNyan
 Author-email: michael.edmund.wong@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

