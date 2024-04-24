# Comparing `tmp/infuzu-python-sdk-0.8.tar.gz` & `tmp/infuzu-python-sdk-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infuzu-python-sdk-0.8.tar", last modified: Tue Dec  5 06:02:35 2023, max compression
+gzip compressed data, was "infuzu-python-sdk-0.9.tar", last modified: Tue Dec  5 23:50:28 2023, max compression
```

## Comparing `infuzu-python-sdk-0.8.tar` & `infuzu-python-sdk-0.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 06:02:35.010060 infuzu-python-sdk-0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-12-05 06:02:23.000000 infuzu-python-sdk-0.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2023-12-05 06:02:35.010060 infuzu-python-sdk-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2023-12-05 06:02:23.000000 infuzu-python-sdk-0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 06:02:35.006060 infuzu-python-sdk-0.8/infuzu/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 06:02:23.000000 infuzu-python-sdk-0.8/infuzu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 06:02:35.006060 infuzu-python-sdk-0.8/infuzu/auth/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-05 06:02:23.000000 infuzu-python-sdk-0.8/infuzu/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3943 2023-12-05 06:02:23.000000 infuzu-python-sdk-0.8/infuzu/auth/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 06:02:35.006060 infuzu-python-sdk-0.8/infuzu/clockwise/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2023-12-05 06:02:23.000000 infuzu-python-sdk-0.8/infuzu/clockwise/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 06:02:35.006060 infuzu-python-sdk-0.8/infuzu/clockwise/assignments/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2023-12-05 06:02:23.000000 infuzu-python-sdk-0.8/infuzu/clockwise/assignments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2023-12-05 06:02:23.000000 infuzu-python-sdk-0.8/infuzu/clockwise/assignments/complete_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5665 2023-12-05 06:02:23.000000 infuzu-python-sdk-0.8/infuzu/clockwise/assignments/retrieve_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-12-05 06:02:23.000000 infuzu-python-sdk-0.8/infuzu/clockwise/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 06:02:35.006060 infuzu-python-sdk-0.8/infuzu/clockwise/rules/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2023-12-05 06:02:23.000000 infuzu-python-sdk-0.8/infuzu/clockwise/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2023-12-05 06:02:23.000000 infuzu-python-sdk-0.8/infuzu/clockwise/rules/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2023-12-05 06:02:23.000000 infuzu-python-sdk-0.8/infuzu/clockwise/rules/calls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2023-12-05 06:02:23.000000 infuzu-python-sdk-0.8/infuzu/clockwise/rules/execution_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2023-12-05 06:02:23.000000 infuzu-python-sdk-0.8/infuzu/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 06:02:35.006060 infuzu-python-sdk-0.8/infuzu/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 06:02:23.000000 infuzu-python-sdk-0.8/infuzu/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 06:02:35.010060 infuzu-python-sdk-0.8/infuzu/utils/api_calls/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 06:02:23.000000 infuzu-python-sdk-0.8/infuzu/utils/api_calls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8049 2023-12-05 06:02:23.000000 infuzu-python-sdk-0.8/infuzu/utils/api_calls/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2023-12-05 06:02:23.000000 infuzu-python-sdk-0.8/infuzu/utils/api_calls/clockwise.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2023-12-05 06:02:23.000000 infuzu-python-sdk-0.8/infuzu/utils/api_calls/infuzu.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2023-12-05 06:02:23.000000 infuzu-python-sdk-0.8/infuzu/utils/api_calls/serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2023-12-05 06:02:23.000000 infuzu-python-sdk-0.8/infuzu/utils/encryption.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 06:02:35.010060 infuzu-python-sdk-0.8/infuzu/utils/enums/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 06:02:23.000000 infuzu-python-sdk-0.8/infuzu/utils/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2023-12-05 06:02:23.000000 infuzu-python-sdk-0.8/infuzu/utils/enums/api_calls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2023-12-05 06:02:23.000000 infuzu-python-sdk-0.8/infuzu/utils/enums/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2023-12-05 06:02:23.000000 infuzu-python-sdk-0.8/infuzu/utils/random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 06:02:35.010060 infuzu-python-sdk-0.8/infuzu_python_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2023-12-05 06:02:34.000000 infuzu-python-sdk-0.8/infuzu_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      966 2023-12-05 06:02:34.000000 infuzu-python-sdk-0.8/infuzu_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-05 06:02:34.000000 infuzu-python-sdk-0.8/infuzu_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-05 06:02:34.000000 infuzu-python-sdk-0.8/infuzu_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-12-05 06:02:23.000000 infuzu-python-sdk-0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-05 06:02:35.010060 infuzu-python-sdk-0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      660 2023-12-05 06:02:23.000000 infuzu-python-sdk-0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 23:50:28.163313 infuzu-python-sdk-0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2023-12-05 23:50:28.163313 infuzu-python-sdk-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 23:50:28.155313 infuzu-python-sdk-0.9/infuzu/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 23:50:28.155313 infuzu-python-sdk-0.9/infuzu/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3943 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/auth/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 23:50:28.155313 infuzu-python-sdk-0.9/infuzu/clockwise/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/clockwise/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 23:50:28.155313 infuzu-python-sdk-0.9/infuzu/clockwise/assignments/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/clockwise/assignments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/clockwise/assignments/complete_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5665 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/clockwise/assignments/retrieve_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/clockwise/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 23:50:28.155313 infuzu-python-sdk-0.9/infuzu/clockwise/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/clockwise/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/clockwise/rules/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/clockwise/rules/calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/clockwise/rules/execution_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 23:50:28.159313 infuzu-python-sdk-0.9/infuzu/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 23:50:28.159313 infuzu-python-sdk-0.9/infuzu/utils/api_calls/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/utils/api_calls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8049 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/utils/api_calls/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/utils/api_calls/clockwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/utils/api_calls/infuzu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/utils/api_calls/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/utils/encryption.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 23:50:28.159313 infuzu-python-sdk-0.9/infuzu/utils/enums/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/utils/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/utils/enums/api_calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/utils/enums/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/utils/random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 23:50:28.159313 infuzu-python-sdk-0.9/infuzu_python_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2023-12-05 23:50:28.000000 infuzu-python-sdk-0.9/infuzu_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2023-12-05 23:50:28.000000 infuzu-python-sdk-0.9/infuzu_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-05 23:50:28.000000 infuzu-python-sdk-0.9/infuzu_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-05 23:50:28.000000 infuzu-python-sdk-0.9/infuzu_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-05 23:50:28.163313 infuzu-python-sdk-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/setup.py
```

### Comparing `infuzu-python-sdk-0.8/LICENSE.md` & `infuzu-python-sdk-0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `infuzu-python-sdk-0.8/infuzu/auth/base.py` & `infuzu-python-sdk-0.9/infuzu/auth/base.py`

 * *Files identical despite different names*

### Comparing `infuzu-python-sdk-0.8/infuzu/clockwise/assignments/complete_assignment.py` & `infuzu-python-sdk-0.9/infuzu/clockwise/assignments/complete_assignment.py`

 * *Files identical despite different names*

### Comparing `infuzu-python-sdk-0.8/infuzu/clockwise/assignments/retrieve_assignment.py` & `infuzu-python-sdk-0.9/infuzu/clockwise/assignments/retrieve_assignment.py`

 * *Files identical despite different names*

### Comparing `infuzu-python-sdk-0.8/infuzu/clockwise/rules/base.py` & `infuzu-python-sdk-0.9/infuzu/clockwise/rules/base.py`

 * *Files identical despite different names*

### Comparing `infuzu-python-sdk-0.8/infuzu/clockwise/rules/calls.py` & `infuzu-python-sdk-0.9/infuzu/clockwise/rules/calls.py`

 * *Files identical despite different names*

### Comparing `infuzu-python-sdk-0.8/infuzu/clockwise/rules/execution_log.py` & `infuzu-python-sdk-0.9/infuzu/clockwise/rules/execution_log.py`

 * *Files identical despite different names*

### Comparing `infuzu-python-sdk-0.8/infuzu/constants.py` & `infuzu-python-sdk-0.9/infuzu/constants.py`

 * *Files identical despite different names*

### Comparing `infuzu-python-sdk-0.8/infuzu/utils/api_calls/base.py` & `infuzu-python-sdk-0.9/infuzu/utils/api_calls/base.py`

 * *Files identical despite different names*

### Comparing `infuzu-python-sdk-0.8/infuzu/utils/api_calls/clockwise.py` & `infuzu-python-sdk-0.9/infuzu/utils/api_calls/clockwise.py`

 * *Files identical despite different names*

### Comparing `infuzu-python-sdk-0.8/infuzu/utils/api_calls/infuzu.py` & `infuzu-python-sdk-0.9/infuzu/utils/api_calls/infuzu.py`

 * *Files identical despite different names*

### Comparing `infuzu-python-sdk-0.8/infuzu/utils/encryption.py` & `infuzu-python-sdk-0.9/infuzu/utils/encryption.py`

 * *Files identical despite different names*

### Comparing `infuzu-python-sdk-0.8/infuzu/utils/enums/api_calls.py` & `infuzu-python-sdk-0.9/infuzu/utils/enums/api_calls.py`

 * *Files identical despite different names*

### Comparing `infuzu-python-sdk-0.8/infuzu/utils/enums/base.py` & `infuzu-python-sdk-0.9/infuzu/utils/enums/base.py`

 * *Files identical despite different names*

### Comparing `infuzu-python-sdk-0.8/infuzu_python_sdk.egg-info/SOURCES.txt` & `infuzu-python-sdk-0.9/infuzu_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `infuzu-python-sdk-0.8/setup.py` & `infuzu-python-sdk-0.9/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import (setup, find_packages)
 
 setup(
     name="infuzu-python-sdk",
-    version="0.8",
+    version="0.9",
     packages=find_packages(),
     install_requires=[],
     author="Infuzu",
     author_email="help@infuzu.com",
     description="This SDK provides a set of tools to manage assignments from Clockwise. Primarily, it allows you to fetch, represent, and mark assignments as complete.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

