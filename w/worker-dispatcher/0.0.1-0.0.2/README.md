# Comparing `tmp/worker_dispatcher-0.0.1.tar.gz` & `tmp/worker_dispatcher-0.0.2.tar.gz`

## Comparing `worker_dispatcher-0.0.1.tar` & `worker_dispatcher-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 worker_dispatcher-0.0.1/src/worker_dispatcher/WorkerDispatcher.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 worker_dispatcher-0.0.1/src/worker_dispatcher/__init__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 worker_dispatcher-0.0.1/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 worker_dispatcher-0.0.1/LICENSE
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 worker_dispatcher-0.0.1/README.md
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 worker_dispatcher-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 worker_dispatcher-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 worker_dispatcher-0.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 worker_dispatcher-0.0.2/src/worker_dispatcher/__init__.py
+-rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 worker_dispatcher-0.0.2/src/worker_dispatcher/worker_dispatcher.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 worker_dispatcher-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 worker_dispatcher-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 worker_dispatcher-0.0.2/README.md
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 worker_dispatcher-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 worker_dispatcher-0.0.2/PKG-INFO
```

### Comparing `worker_dispatcher-0.0.1/.gitignore` & `worker_dispatcher-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `worker_dispatcher-0.0.1/LICENSE` & `worker_dispatcher-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `worker_dispatcher-0.0.1/pyproject.toml` & `worker_dispatcher-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "worker_dispatcher"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Nick Tsai", email="myintaer@gmail.com" },
 ]
 description = "Developing"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

