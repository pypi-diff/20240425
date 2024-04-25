# Comparing `tmp/pytest_sentry-0.3.0.tar.gz` & `tmp/pytest_sentry-0.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_sentry-0.3.0.tar", last modified: Thu Apr 25 11:11:41 2024, max compression
+gzip compressed data, was "pytest_sentry-0.3.0rc1.tar", last modified: Fri Apr  5 13:54:49 2024, max compression
```

## Comparing `pytest_sentry-0.3.0.tar` & `pytest_sentry-0.3.0rc1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:11:41.045643 pytest_sentry-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-25 11:11:35.000000 pytest_sentry-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-04-25 11:11:41.045643 pytest_sentry-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-25 11:11:35.000000 pytest_sentry-0.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:11:41.045643 pytest_sentry-0.3.0/pytest_sentry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-04-25 11:11:41.000000 pytest_sentry-0.3.0/pytest_sentry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-25 11:11:41.000000 pytest_sentry-0.3.0/pytest_sentry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 11:11:41.000000 pytest_sentry-0.3.0/pytest_sentry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-25 11:11:41.000000 pytest_sentry-0.3.0/pytest_sentry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-25 11:11:41.000000 pytest_sentry-0.3.0/pytest_sentry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-25 11:11:41.000000 pytest_sentry-0.3.0/pytest_sentry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9911 2024-04-25 11:11:35.000000 pytest_sentry-0.3.0/pytest_sentry.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-25 11:11:41.045643 pytest_sentry-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-25 11:11:35.000000 pytest_sentry-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:11:41.045643 pytest_sentry-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-25 11:11:35.000000 pytest_sentry-0.3.0/tests/test_envvars.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-25 11:11:35.000000 pytest_sentry-0.3.0/tests/test_fixture.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-25 11:11:35.000000 pytest_sentry-0.3.0/tests/test_retries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-25 11:11:35.000000 pytest_sentry-0.3.0/tests/test_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-25 11:11:35.000000 pytest_sentry-0.3.0/tests/test_skip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-25 11:11:35.000000 pytest_sentry-0.3.0/tests/test_tracing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:54:49.055662 pytest_sentry-0.3.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-05 13:54:45.000000 pytest_sentry-0.3.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-04-05 13:54:49.055662 pytest_sentry-0.3.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-05 13:54:45.000000 pytest_sentry-0.3.0rc1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:54:49.055662 pytest_sentry-0.3.0rc1/pytest_sentry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-04-05 13:54:49.000000 pytest_sentry-0.3.0rc1/pytest_sentry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-05 13:54:49.000000 pytest_sentry-0.3.0rc1/pytest_sentry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 13:54:49.000000 pytest_sentry-0.3.0rc1/pytest_sentry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-05 13:54:49.000000 pytest_sentry-0.3.0rc1/pytest_sentry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-05 13:54:49.000000 pytest_sentry-0.3.0rc1/pytest_sentry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 13:54:49.000000 pytest_sentry-0.3.0rc1/pytest_sentry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9911 2024-04-05 13:54:45.000000 pytest_sentry-0.3.0rc1/pytest_sentry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-05 13:54:49.055662 pytest_sentry-0.3.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-05 13:54:45.000000 pytest_sentry-0.3.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:54:49.055662 pytest_sentry-0.3.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-05 13:54:45.000000 pytest_sentry-0.3.0rc1/tests/test_envvars.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-05 13:54:45.000000 pytest_sentry-0.3.0rc1/tests/test_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-05 13:54:45.000000 pytest_sentry-0.3.0rc1/tests/test_retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-05 13:54:45.000000 pytest_sentry-0.3.0rc1/tests/test_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-05 13:54:45.000000 pytest_sentry-0.3.0rc1/tests/test_skip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-05 13:54:45.000000 pytest_sentry-0.3.0rc1/tests/test_tracing.py
```

### Comparing `pytest_sentry-0.3.0/LICENSE` & `pytest_sentry-0.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_sentry-0.3.0/PKG-INFO` & `pytest_sentry-0.3.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pytest_sentry
-Version: 0.3.0
+Version: 0.3.0rc1
 Summary: A pytest plugin to send testrun information to Sentry.io
 Home-page: https://github.com/untitaker/pytest-sentry
 Author: Markus Unterwaditzer
 Author-email: markus@unterwaditzer.net
 License: BSD-2-Clause
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: pytest
-Requires-Dist: sentry-sdk>=2.0.0
+Requires-Dist: sentry-sdk<3,>=2.0.0a1
 Requires-Dist: wrapt
 
 =============
 pytest-sentry
 =============
 
 .. image:: https://img.shields.io/pypi/v/pytest-sentry
```

### Comparing `pytest_sentry-0.3.0/README.rst` & `pytest_sentry-0.3.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `pytest_sentry-0.3.0/pytest_sentry.egg-info/PKG-INFO` & `pytest_sentry-0.3.0rc1/pytest_sentry.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pytest_sentry
-Version: 0.3.0
+Version: 0.3.0rc1
 Summary: A pytest plugin to send testrun information to Sentry.io
 Home-page: https://github.com/untitaker/pytest-sentry
 Author: Markus Unterwaditzer
 Author-email: markus@unterwaditzer.net
 License: BSD-2-Clause
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: pytest
-Requires-Dist: sentry-sdk>=2.0.0
+Requires-Dist: sentry-sdk<3,>=2.0.0a1
 Requires-Dist: wrapt
 
 =============
 pytest-sentry
 =============
 
 .. image:: https://img.shields.io/pypi/v/pytest-sentry
```

### Comparing `pytest_sentry-0.3.0/pytest_sentry.py` & `pytest_sentry-0.3.0rc1/pytest_sentry.py`

 * *Files identical despite different names*

### Comparing `pytest_sentry-0.3.0/setup.cfg` & `pytest_sentry-0.3.0rc1/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pytest_sentry
-version = 0.3.0
+version = 0.3.0rc1
 description = A pytest plugin to send testrun information to Sentry.io
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/untitaker/pytest-sentry
 author = Markus Unterwaditzer
 author_email = markus@unterwaditzer.net
 license = BSD-2-Clause
@@ -12,15 +12,15 @@
 classifiers = 
 	License :: OSI Approved :: BSD License
 
 [options]
 py_modules = pytest_sentry
 install_requires = 
 	pytest
-	sentry-sdk>=2.0.0
+	sentry-sdk>=2.0.0a1,<3
 	wrapt
 
 [options.entry_points]
 pytest11 = 
 	sentry = pytest_sentry
 
 [egg_info]
```

### Comparing `pytest_sentry-0.3.0/tests/test_envvars.py` & `pytest_sentry-0.3.0rc1/tests/test_envvars.py`

 * *Files identical despite different names*

### Comparing `pytest_sentry-0.3.0/tests/test_retries.py` & `pytest_sentry-0.3.0rc1/tests/test_retries.py`

 * *Files identical despite different names*

### Comparing `pytest_sentry-0.3.0/tests/test_scope.py` & `pytest_sentry-0.3.0rc1/tests/test_scope.py`

 * *Files identical despite different names*

### Comparing `pytest_sentry-0.3.0/tests/test_skip.py` & `pytest_sentry-0.3.0rc1/tests/test_skip.py`

 * *Files identical despite different names*

### Comparing `pytest_sentry-0.3.0/tests/test_tracing.py` & `pytest_sentry-0.3.0rc1/tests/test_tracing.py`

 * *Files identical despite different names*

