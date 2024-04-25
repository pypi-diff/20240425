# Comparing `tmp/redis_mutator-0.1.0.tar.gz` & `tmp/redis_mutator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_mutator-0.1.0.tar", max compression
+gzip compressed data, was "redis_mutator-0.1.1.tar", max compression
```

## Comparing `redis_mutator-0.1.0.tar` & `redis_mutator-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2024-04-25 02:57:39.950196 redis_mutator-0.1.0/README.md
--rw-r--r--   0        0        0      297 2024-04-25 02:58:42.498161 redis_mutator-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       89 2024-04-25 03:42:13.447337 redis_mutator-0.1.0/redis_mutator/__init__.py
--rw-r--r--   0        0        0     2664 2024-04-25 03:41:49.259412 redis_mutator-0.1.0/redis_mutator/method_names.py
--rw-r--r--   0        0        0     1290 2024-04-25 03:00:33.262043 redis_mutator-0.1.0/redis_mutator/mutate.py
--rw-r--r--   0        0        0     2919 2024-04-25 03:39:40.231818 redis_mutator-0.1.0/redis_mutator/redis_mutator.py
--rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 redis_mutator-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-25 02:57:39.950196 redis_mutator-0.1.1/README.md
+-rw-r--r--   0        0        0      297 2024-04-25 03:48:15.238180 redis_mutator-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       91 2024-04-25 03:48:09.782197 redis_mutator-0.1.1/redis_mutator/__init__.py
+-rw-r--r--   0        0        0     2664 2024-04-25 03:41:49.259412 redis_mutator-0.1.1/redis_mutator/method_names.py
+-rw-r--r--   0        0        0     1290 2024-04-25 03:00:33.262043 redis_mutator-0.1.1/redis_mutator/mutate.py
+-rw-r--r--   0        0        0     2919 2024-04-25 03:39:40.231818 redis_mutator-0.1.1/redis_mutator/redis_mutator.py
+-rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 redis_mutator-0.1.1/PKG-INFO
```

### Comparing `redis_mutator-0.1.0/redis_mutator/method_names.py` & `redis_mutator-0.1.1/redis_mutator/method_names.py`

 * *Files identical despite different names*

### Comparing `redis_mutator-0.1.0/redis_mutator/mutate.py` & `redis_mutator-0.1.1/redis_mutator/mutate.py`

 * *Files identical despite different names*

### Comparing `redis_mutator-0.1.0/redis_mutator/redis_mutator.py` & `redis_mutator-0.1.1/redis_mutator/redis_mutator.py`

 * *Files identical despite different names*

### Comparing `redis_mutator-0.1.0/PKG-INFO` & `redis_mutator-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-mutator
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: MisterNyan
 Author-email: michael.edmund.wong@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

