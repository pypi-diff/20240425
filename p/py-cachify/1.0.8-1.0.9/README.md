# Comparing `tmp/py_cachify-1.0.8.tar.gz` & `tmp/py_cachify-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_cachify-1.0.8.tar", max compression
+gzip compressed data, was "py_cachify-1.0.9.tar", max compression
```

## Comparing `py_cachify-1.0.8.tar` & `py_cachify-1.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1064 2024-04-02 19:19:45.372753 py_cachify-1.0.8/LICENSE
--rw-r--r--   0        0        0     3316 2024-04-02 19:19:45.372753 py_cachify-1.0.8/README.md
--rw-r--r--   0        0        0      342 2024-04-02 19:19:45.372753 py_cachify-1.0.8/py_cachify/__init__.py
--rw-r--r--   0        0        0      201 2024-04-02 19:19:45.372753 py_cachify-1.0.8/py_cachify/async.py
--rw-r--r--   0        0        0        0 2024-04-02 19:19:45.372753 py_cachify-1.0.8/py_cachify/backend/__init__.py
--rw-r--r--   0        0        0      733 2024-04-02 19:19:45.372753 py_cachify-1.0.8/py_cachify/backend/base.py
--rw-r--r--   0        0        0     2449 2024-04-02 19:19:45.372753 py_cachify-1.0.8/py_cachify/backend/cached.py
--rw-r--r--   0        0        0     1210 2024-04-02 19:19:45.372753 py_cachify-1.0.8/py_cachify/backend/clients.py
--rw-r--r--   0        0        0      127 2024-04-02 19:19:45.372753 py_cachify-1.0.8/py_cachify/backend/exceptions.py
--rw-r--r--   0        0        0     1941 2024-04-02 19:19:45.372753 py_cachify-1.0.8/py_cachify/backend/lib.py
--rw-r--r--   0        0        0     3918 2024-04-02 19:19:45.372753 py_cachify-1.0.8/py_cachify/backend/lock.py
--rw-r--r--   0        0        0      719 2024-04-02 19:19:45.372753 py_cachify-1.0.8/py_cachify/backend/types.py
--rw-r--r--   0        0        0        0 2024-04-02 19:19:45.372753 py_cachify-1.0.8/py_cachify/py.typed
--rw-r--r--   0        0        0      183 2024-04-02 19:19:45.372753 py_cachify-1.0.8/py_cachify/sync.py
--rw-r--r--   0        0        0     4092 2024-04-02 19:19:45.372753 py_cachify-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     3981 1970-01-01 00:00:00.000000 py_cachify-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-12 22:19:34.629519 py_cachify-1.0.9/LICENSE
+-rw-r--r--   0        0        0     3316 2024-04-12 22:19:34.629519 py_cachify-1.0.9/README.md
+-rw-r--r--   0        0        0      342 2024-04-12 22:19:34.633519 py_cachify-1.0.9/py_cachify/__init__.py
+-rw-r--r--   0        0        0      201 2024-04-12 22:19:34.633519 py_cachify-1.0.9/py_cachify/async.py
+-rw-r--r--   0        0        0        0 2024-04-12 22:19:34.633519 py_cachify-1.0.9/py_cachify/backend/__init__.py
+-rw-r--r--   0        0        0      733 2024-04-12 22:19:34.633519 py_cachify-1.0.9/py_cachify/backend/base.py
+-rw-r--r--   0        0        0     2449 2024-04-12 22:19:34.633519 py_cachify-1.0.9/py_cachify/backend/cached.py
+-rw-r--r--   0        0        0     1210 2024-04-12 22:19:34.633519 py_cachify-1.0.9/py_cachify/backend/clients.py
+-rw-r--r--   0        0        0      127 2024-04-12 22:19:34.633519 py_cachify-1.0.9/py_cachify/backend/exceptions.py
+-rw-r--r--   0        0        0     1941 2024-04-12 22:19:34.633519 py_cachify-1.0.9/py_cachify/backend/lib.py
+-rw-r--r--   0        0        0     3918 2024-04-12 22:19:34.633519 py_cachify-1.0.9/py_cachify/backend/lock.py
+-rw-r--r--   0        0        0      719 2024-04-12 22:19:34.633519 py_cachify-1.0.9/py_cachify/backend/types.py
+-rw-r--r--   0        0        0        0 2024-04-12 22:19:34.633519 py_cachify-1.0.9/py_cachify/py.typed
+-rw-r--r--   0        0        0      183 2024-04-12 22:19:34.633519 py_cachify-1.0.9/py_cachify/sync.py
+-rw-r--r--   0        0        0     4123 2024-04-12 22:19:34.633519 py_cachify-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4032 1970-01-01 00:00:00.000000 py_cachify-1.0.9/PKG-INFO
```

### Comparing `py_cachify-1.0.8/LICENSE` & `py_cachify-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `py_cachify-1.0.8/README.md` & `py_cachify-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `py_cachify-1.0.8/py_cachify/backend/base.py` & `py_cachify-1.0.9/py_cachify/backend/base.py`

 * *Files identical despite different names*

### Comparing `py_cachify-1.0.8/py_cachify/backend/cached.py` & `py_cachify-1.0.9/py_cachify/backend/cached.py`

 * *Files identical despite different names*

### Comparing `py_cachify-1.0.8/py_cachify/backend/clients.py` & `py_cachify-1.0.9/py_cachify/backend/clients.py`

 * *Files identical despite different names*

### Comparing `py_cachify-1.0.8/py_cachify/backend/lib.py` & `py_cachify-1.0.9/py_cachify/backend/lib.py`

 * *Files identical despite different names*

### Comparing `py_cachify-1.0.8/py_cachify/backend/lock.py` & `py_cachify-1.0.9/py_cachify/backend/lock.py`

 * *Files identical despite different names*

### Comparing `py_cachify-1.0.8/py_cachify/backend/types.py` & `py_cachify-1.0.9/py_cachify/backend/types.py`

 * *Files identical despite different names*

### Comparing `py_cachify-1.0.8/pyproject.toml` & `py_cachify-1.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 [tool.poetry]
 name = "py-cachify"
-version = "1.0.8"
+version = "1.0.9"
 homepage = "https://github.com/EzyGang/py-cachify"
 repository = "https://github.com/EzyGang/py-cachify"
 license = "MIT"
 description = ""
 authors = ["Galtozzy <galtozzy+git@gmail.com>"]
 readme = "README.md"
 include = ["README.md"]
 packages = [{include = 'py_cachify'}]
 
 [project]
 requires-python = ">=3.8,<4.0"
 
 [tool.poetry.dependencies]
 python = "^3.8"
+typing-extensions = "^4.11.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.3"
 pytest-mock = "^3.12.0"
-pytest-cov = "^4.1.0"
+pytest-cov = "^5.0.0"
 taskipy = "^1.12.2"
 mypy = "^1.7.1"
 ruff = "^0.3.2"
 coverage = "^7.3.2"
 pytest-asyncio = "^0.21.1"
 pytest-socket = "^0.6.0"
 
@@ -99,15 +100,15 @@
 check_untyped_defs = true
 disallow_untyped_decorators = true
 disallow_any_generics = false
 disallow_untyped_calls = true
 disallow_untyped_defs = true
 disallow_incomplete_defs = true
 ignore_errors = false
-ignore_missing_imports = true
+ignore_missing_imports = false
 implicit_reexport = true
 local_partial_types = true
 strict_optional = true
 strict_equality = true
 no_implicit_optional = true
 warn_unused_ignores = true
 warn_redundant_casts = true
```

### Comparing `py_cachify-1.0.8/PKG-INFO` & `py_cachify-1.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: py-cachify
-Version: 1.0.8
+Version: 1.0.9
 Summary: 
 Home-page: https://github.com/EzyGang/py-cachify
 License: MIT
 Author: Galtozzy
 Author-email: galtozzy+git@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: typing-extensions (>=4.11.0,<5.0.0)
 Project-URL: Repository, https://github.com/EzyGang/py-cachify
 Description-Content-Type: text/markdown
 
 # Py-Cachify
 
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![PyPI version](https://badge.fury.io/py/py-cachify.svg)](https://badge.fury.io/py/py-cachify)
```

