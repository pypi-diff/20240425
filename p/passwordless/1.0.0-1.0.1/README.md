# Comparing `tmp/passwordless-1.0.0.tar.gz` & `tmp/passwordless-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passwordless-1.0.0.tar", max compression
+gzip compressed data, was "passwordless-1.0.1.tar", max compression
```

## Comparing `passwordless-1.0.0.tar` & `passwordless-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2024-04-08 07:45:36.813967 passwordless-1.0.0/LICENSE
--rw-r--r--   0        0        0     2882 2024-04-08 07:45:36.813967 passwordless-1.0.0/README.md
--rw-r--r--   0        0        0     1996 2024-04-08 07:45:36.817967 passwordless-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1097 2024-04-08 07:45:36.817967 passwordless-1.0.0/src/passwordless/__init__.py
--rw-r--r--   0        0        0    13669 2024-04-08 07:45:36.817967 passwordless-1.0.0/src/passwordless/client.py
--rw-r--r--   0        0        0      497 2024-04-08 07:45:36.817967 passwordless-1.0.0/src/passwordless/config.py
--rw-r--r--   0        0        0     1083 2024-04-08 07:45:36.817967 passwordless-1.0.0/src/passwordless/errors.py
--rw-r--r--   0        0        0     2548 2024-04-08 07:45:36.817967 passwordless-1.0.0/src/passwordless/models.py
--rw-r--r--   0        0        0     6653 2024-04-08 07:45:36.817967 passwordless-1.0.0/src/passwordless/serialization.py
--rw-r--r--   0        0        0     3839 1970-01-01 00:00:00.000000 passwordless-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-25 10:38:10.767718 passwordless-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3261 2024-04-25 10:38:10.767718 passwordless-1.0.1/README.md
+-rw-r--r--   0        0        0     2001 2024-04-25 10:38:10.771718 passwordless-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1097 2024-04-25 10:38:10.771718 passwordless-1.0.1/src/passwordless/__init__.py
+-rw-r--r--   0        0        0    13669 2024-04-25 10:38:10.771718 passwordless-1.0.1/src/passwordless/client.py
+-rw-r--r--   0        0        0      497 2024-04-25 10:38:10.771718 passwordless-1.0.1/src/passwordless/config.py
+-rw-r--r--   0        0        0     1083 2024-04-25 10:38:10.771718 passwordless-1.0.1/src/passwordless/errors.py
+-rw-r--r--   0        0        0     2548 2024-04-25 10:38:10.771718 passwordless-1.0.1/src/passwordless/models.py
+-rw-r--r--   0        0        0     6653 2024-04-25 10:38:10.771718 passwordless-1.0.1/src/passwordless/serialization.py
+-rw-r--r--   0        0        0     4457 1970-01-01 00:00:00.000000 passwordless-1.0.1/PKG-INFO
```

### Comparing `passwordless-1.0.0/LICENSE` & `passwordless-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `passwordless-1.0.0/README.md` & `passwordless-1.0.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Passwordless Python SDK
 
+[![Build](https://img.shields.io/github/actions/workflow/status/bitwarden/passwordless-python/ci.yml?branch=main)](https://github.com/bitwarden/passwordless-python/actions)
+[![Version](https://img.shields.io/pypi/v/Passwordless.svg)](https://pypi.org/project/passwordless/)
+[![Downloads](https://img.shields.io/pypi/dm/Passwordless.svg)](https://pypi.org/project/passwordless/)
+
 The official [Bitwarden Passwordless.dev](https://passwordless.dev/) Python library, for Python 3+.
 
 ## Installation
 
 Install with `python -m pip install passwordless`.
 
 ### Dependencies
```

### Comparing `passwordless-1.0.0/pyproject.toml` & `passwordless-1.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "passwordless"
-version = "1.0.0"
+version = "1.0.1"
 description = "Passwordless.dev Python SDK"
 authors = [
     "Bitwarden <hello@bitwarden.com>"
 ]
 maintainers = [
     "Maciej Zieniuk <zieniuk.maciej@gmail.com>"
 ]
@@ -21,32 +21,32 @@
     "License :: OSI Approved :: Apache Software License"
 ]
 keywords = ["passwordless", "bitwarden"]
 homepage = "https://bitwarden.com/products/passwordless"
 documentation = "https://docs.passwordless.dev/guide"
 
 [tool.poetry.dependencies]
-python = "3.8.18"
-requests = "2.31.0"
-marshmallow = "3.21.1"
-python-dateutil = "2.9.0.post0"
+python = ">=3.8"
+requests = "^2"
+marshmallow = "^3"
+python-dateutil = "^2"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-dotenv = "1.0.1"
 flake8 = "5.0.4"
-black = "24.3.0"
+black = "24.4.1"
 mypy = "1.9.0"
 isort = "5.13.2"
 pre-commit = "3.5.0"
 pre-commit-hooks = "4.5.0"
 types-requests = "2.31.0.20240406"
-docformatter = {extras = ["tomli"], version = "1.7.5"}
+docformatter = {extras = ["tomli"], version = "1.7.5", python = ">=3.8,<4.0"}
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "8.0.2"
 pytest-mock = "3.12.0"
```

### Comparing `passwordless-1.0.0/src/passwordless/__init__.py` & `passwordless-1.0.1/src/passwordless/__init__.py`

 * *Files identical despite different names*

### Comparing `passwordless-1.0.0/src/passwordless/client.py` & `passwordless-1.0.1/src/passwordless/client.py`

 * *Files identical despite different names*

### Comparing `passwordless-1.0.0/src/passwordless/errors.py` & `passwordless-1.0.1/src/passwordless/errors.py`

 * *Files identical despite different names*

### Comparing `passwordless-1.0.0/src/passwordless/models.py` & `passwordless-1.0.1/src/passwordless/models.py`

 * *Files identical despite different names*

### Comparing `passwordless-1.0.0/src/passwordless/serialization.py` & `passwordless-1.0.1/src/passwordless/serialization.py`

 * *Files identical despite different names*

### Comparing `passwordless-1.0.0/PKG-INFO` & `passwordless-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,44 @@
 Metadata-Version: 2.1
 Name: passwordless
-Version: 1.0.0
+Version: 1.0.1
 Summary: Passwordless.dev Python SDK
 Home-page: https://bitwarden.com/products/passwordless
 License: Apache-2.0
 Keywords: passwordless,bitwarden
 Author: Bitwarden
 Author-email: hello@bitwarden.com
 Maintainer: Maciej Zieniuk
 Maintainer-email: zieniuk.maciej@gmail.com
-Requires-Python: ==3.8.18
+Requires-Python: >=3.8
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Communications :: FIDO
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries
-Requires-Dist: marshmallow (==3.21.1)
-Requires-Dist: python-dateutil (==2.9.0.post0)
-Requires-Dist: requests (==2.31.0)
+Requires-Dist: marshmallow (>=3,<4)
+Requires-Dist: python-dateutil (>=2,<3)
+Requires-Dist: requests (>=2,<3)
 Project-URL: Documentation, https://docs.passwordless.dev/guide
 Description-Content-Type: text/markdown
 
 # Passwordless Python SDK
 
+[![Build](https://img.shields.io/github/actions/workflow/status/bitwarden/passwordless-python/ci.yml?branch=main)](https://github.com/bitwarden/passwordless-python/actions)
+[![Version](https://img.shields.io/pypi/v/Passwordless.svg)](https://pypi.org/project/passwordless/)
+[![Downloads](https://img.shields.io/pypi/dm/Passwordless.svg)](https://pypi.org/project/passwordless/)
+
 The official [Bitwarden Passwordless.dev](https://passwordless.dev/) Python library, for Python 3+.
 
 ## Installation
 
 Install with `python -m pip install passwordless`.
 
 ### Dependencies
```

