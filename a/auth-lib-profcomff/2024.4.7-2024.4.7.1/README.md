# Comparing `tmp/auth_lib_profcomff-2024.4.7.tar.gz` & `tmp/auth_lib_profcomff-2024.4.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auth_lib_profcomff-2024.4.7.tar", last modified: Sun Apr  7 00:09:36 2024, max compression
+gzip compressed data, was "auth_lib_profcomff-2024.4.7.1.tar", last modified: Sun Apr  7 00:36:11 2024, max compression
```

## Comparing `auth_lib_profcomff-2024.4.7.tar` & `auth_lib_profcomff-2024.4.7.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:09:36.044084 auth_lib_profcomff-2024.4.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-07 00:09:28.000000 auth_lib_profcomff-2024.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-04-07 00:09:36.044084 auth_lib_profcomff-2024.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5553 2024-04-07 00:09:28.000000 auth_lib_profcomff-2024.4.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:09:36.040084 auth_lib_profcomff-2024.4.7/auth_lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:09:28.000000 auth_lib_profcomff-2024.4.7/auth_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-07 00:09:28.000000 auth_lib_profcomff-2024.4.7/auth_lib/aiomethods.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-07 00:09:28.000000 auth_lib_profcomff-2024.4.7/auth_lib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-07 00:09:28.000000 auth_lib_profcomff-2024.4.7/auth_lib/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-07 00:09:28.000000 auth_lib_profcomff-2024.4.7/auth_lib/methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:09:36.044084 auth_lib_profcomff-2024.4.7/auth_lib/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-07 00:09:28.000000 auth_lib_profcomff-2024.4.7/auth_lib/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-07 00:09:28.000000 auth_lib_profcomff-2024.4.7/auth_lib/testing/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:09:36.044084 auth_lib_profcomff-2024.4.7/auth_lib_profcomff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-04-07 00:09:36.000000 auth_lib_profcomff-2024.4.7/auth_lib_profcomff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-07 00:09:36.000000 auth_lib_profcomff-2024.4.7/auth_lib_profcomff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 00:09:36.000000 auth_lib_profcomff-2024.4.7/auth_lib_profcomff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-07 00:09:36.000000 auth_lib_profcomff-2024.4.7/auth_lib_profcomff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-07 00:09:36.000000 auth_lib_profcomff-2024.4.7/auth_lib_profcomff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 00:09:36.000000 auth_lib_profcomff-2024.4.7/auth_lib_profcomff.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 00:09:36.044084 auth_lib_profcomff-2024.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-07 00:09:28.000000 auth_lib_profcomff-2024.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:36:11.857489 auth_lib_profcomff-2024.4.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-07 00:36:04.000000 auth_lib_profcomff-2024.4.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-04-07 00:36:11.857489 auth_lib_profcomff-2024.4.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5553 2024-04-07 00:36:04.000000 auth_lib_profcomff-2024.4.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:36:11.857489 auth_lib_profcomff-2024.4.7.1/auth_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:36:04.000000 auth_lib_profcomff-2024.4.7.1/auth_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-07 00:36:04.000000 auth_lib_profcomff-2024.4.7.1/auth_lib/aiomethods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-07 00:36:04.000000 auth_lib_profcomff-2024.4.7.1/auth_lib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-04-07 00:36:04.000000 auth_lib_profcomff-2024.4.7.1/auth_lib/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-07 00:36:04.000000 auth_lib_profcomff-2024.4.7.1/auth_lib/methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:36:11.857489 auth_lib_profcomff-2024.4.7.1/auth_lib/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-07 00:36:04.000000 auth_lib_profcomff-2024.4.7.1/auth_lib/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-07 00:36:04.000000 auth_lib_profcomff-2024.4.7.1/auth_lib/testing/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:36:11.857489 auth_lib_profcomff-2024.4.7.1/auth_lib_profcomff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-04-07 00:36:11.000000 auth_lib_profcomff-2024.4.7.1/auth_lib_profcomff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-07 00:36:11.000000 auth_lib_profcomff-2024.4.7.1/auth_lib_profcomff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 00:36:11.000000 auth_lib_profcomff-2024.4.7.1/auth_lib_profcomff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-07 00:36:11.000000 auth_lib_profcomff-2024.4.7.1/auth_lib_profcomff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-07 00:36:11.000000 auth_lib_profcomff-2024.4.7.1/auth_lib_profcomff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 00:36:11.000000 auth_lib_profcomff-2024.4.7.1/auth_lib_profcomff.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 00:36:11.857489 auth_lib_profcomff-2024.4.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-07 00:36:04.000000 auth_lib_profcomff-2024.4.7.1/setup.py
```

### Comparing `auth_lib_profcomff-2024.4.7/LICENSE` & `auth_lib_profcomff-2024.4.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2024.4.7/PKG-INFO` & `auth_lib_profcomff-2024.4.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auth_lib_profcomff
-Version: 2024.4.7
+Version: 2024.4.7.1
 Home-page: https://github.com/profcomff/auth-lib
 Author: Semyon Grigoriev
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: aiohttp
```

### Comparing `auth_lib_profcomff-2024.4.7/README.md` & `auth_lib_profcomff-2024.4.7.1/README.md`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2024.4.7/auth_lib/aiomethods.py` & `auth_lib_profcomff-2024.4.7.1/auth_lib/aiomethods.py`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2024.4.7/auth_lib/exceptions.py` & `auth_lib_profcomff-2024.4.7.1/auth_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2024.4.7/auth_lib/fastapi.py` & `auth_lib_profcomff-2024.4.7.1/auth_lib/fastapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from fastapi.exceptions import HTTPException
 from fastapi.openapi.models import APIKey, APIKeyIn
 from fastapi.security.base import SecurityBase
 from pydantic import ConfigDict
 from pydantic_settings import BaseSettings
 from starlette.requests import Request
-from starlette.status import HTTP_403_FORBIDDEN
+from starlette.status import HTTP_401_UNAUTHORIZED, HTTP_403_FORBIDDEN
 
 from auth_lib.aiomethods import AsyncAuthLib
 
 
 class UnionAuthSettings(BaseSettings):
     AUTH_URL: str = "https://api.test.profcomff.com/auth/"
     USERDATA_URL: str = "https://api.test.profcomff.com/userdata/"
```

### Comparing `auth_lib_profcomff-2024.4.7/auth_lib/methods.py` & `auth_lib_profcomff-2024.4.7.1/auth_lib/methods.py`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2024.4.7/auth_lib/testing/testutils.py` & `auth_lib_profcomff-2024.4.7.1/auth_lib/testing/testutils.py`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2024.4.7/auth_lib_profcomff.egg-info/PKG-INFO` & `auth_lib_profcomff-2024.4.7.1/auth_lib_profcomff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auth_lib_profcomff
-Version: 2024.4.7
+Version: 2024.4.7.1
 Home-page: https://github.com/profcomff/auth-lib
 Author: Semyon Grigoriev
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: aiohttp
```

### Comparing `auth_lib_profcomff-2024.4.7/setup.py` & `auth_lib_profcomff-2024.4.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with open("requirements.txt", "r", encoding="utf-8") as req_file:
     req = req_file.read().split("\n")
 
 
 setup(
     name="auth_lib_profcomff",
-    version="2024.04.07",
+    version="2024.04.07.1",
     author="Semyon Grigoriev",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/profcomff/auth-lib",
     packages=find_packages(),
     install_requires=req,
     extras_require={
```

