# Comparing `tmp/redis_mutator-0.1.1.tar.gz` & `tmp/redis_mutator-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_mutator-0.1.1.tar", max compression
+gzip compressed data, was "redis_mutator-0.2.0.tar", max compression
```

## Comparing `redis_mutator-0.1.1.tar` & `redis_mutator-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2024-04-25 02:57:39.950196 redis_mutator-0.1.1/README.md
--rw-r--r--   0        0        0      297 2024-04-25 03:48:15.238180 redis_mutator-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       91 2024-04-25 03:48:09.782197 redis_mutator-0.1.1/redis_mutator/__init__.py
--rw-r--r--   0        0        0     2664 2024-04-25 03:41:49.259412 redis_mutator-0.1.1/redis_mutator/method_names.py
--rw-r--r--   0        0        0     1290 2024-04-25 03:00:33.262043 redis_mutator-0.1.1/redis_mutator/mutate.py
--rw-r--r--   0        0        0     2919 2024-04-25 03:39:40.231818 redis_mutator-0.1.1/redis_mutator/redis_mutator.py
--rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 redis_mutator-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1684 2024-04-25 07:06:59.241545 redis_mutator-0.2.0/README.md
+-rw-r--r--   0        0        0      297 2024-04-25 07:10:31.002372 redis_mutator-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       91 2024-04-25 03:48:09.782197 redis_mutator-0.2.0/redis_mutator/__init__.py
+-rw-r--r--   0        0        0     2778 2024-04-25 05:54:28.822062 redis_mutator-0.2.0/redis_mutator/method_names.py
+-rw-r--r--   0        0        0     1290 2024-04-25 03:00:33.262043 redis_mutator-0.2.0/redis_mutator/mutate.py
+-rw-r--r--   0        0        0     4198 2024-04-25 07:09:35.934159 redis_mutator-0.2.0/redis_mutator/redis_mutator.py
+-rw-r--r--   0        0        0     2223 1970-01-01 00:00:00.000000 redis_mutator-0.2.0/PKG-INFO
```

### Comparing `redis_mutator-0.1.1/redis_mutator/method_names.py` & `redis_mutator-0.2.0/redis_mutator/method_names.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,14 +88,17 @@
     "hdel",
     "hincrby",
     "hincrbyfloat",
     "hset",
     "hsetnx",
     "hmset",
 ]
+"""
+List of Redis methods that involves writing.
+"""
 
 READ_METHOD_NAMES = [
     # BasicKeyCommands
     "bitcount",
     "bitpos",
     "dump",
     "exists",
@@ -167,7 +170,10 @@
     "hgetall",
     "hkeys",
     "hlen",
     "hmget",
     "hvals",
     "hstrlen",
 ]
+"""
+List of Redis methods that does not involve writing.
+"""
```

### Comparing `redis_mutator-0.1.1/redis_mutator/mutate.py` & `redis_mutator-0.2.0/redis_mutator/mutate.py`

 * *Files identical despite different names*

