# Comparing `tmp/edx-i18n-tools-1.5.0.tar.gz` & `tmp/edx_i18n_tools-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-i18n-tools-1.5.0.tar", last modified: Thu Apr 11 17:29:25 2024, max compression
+gzip compressed data, was "edx_i18n_tools-1.6.0.tar", last modified: Thu Apr 25 06:59:47 2024, max compression
```

## Comparing `edx-i18n-tools-1.5.0.tar` & `edx_i18n_tools-1.6.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:29:25.066615 edx-i18n-tools-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-04-11 17:29:25.066615 edx-i18n-tools-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:29:25.066615 edx-i18n-tools-1.5.0/edx_i18n_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-04-11 17:29:25.000000 edx-i18n-tools-1.5.0/edx_i18n_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-11 17:29:25.000000 edx-i18n-tools-1.5.0/edx_i18n_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 17:29:25.000000 edx-i18n-tools-1.5.0/edx_i18n_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-11 17:29:25.000000 edx-i18n-tools-1.5.0/edx_i18n_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-11 17:29:25.000000 edx-i18n-tools-1.5.0/edx_i18n_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-11 17:29:25.000000 edx-i18n-tools-1.5.0/edx_i18n_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:29:25.062615 edx-i18n-tools-1.5.0/i18n/
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/i18n/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/i18n/branch_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/i18n/changed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/i18n/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/i18n/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8965 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/i18n/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/i18n/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)    12450 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/i18n/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)     8003 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/i18n/generate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1431 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/i18n/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/i18n/segment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/i18n/transifex.py
--rw-r--r--   0 runner    (1001) docker     (127)    10162 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/i18n/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:29:25.062615 edx-i18n-tools-1.5.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-11 17:29:25.066615 edx-i18n-tools-1.5.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2478 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:29:25.066615 edx-i18n-tools-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/tests/test_changed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/tests/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/tests/test_dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9402 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/tests/test_extract.py
--rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/tests/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/tests/test_segment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/tests/test_transifex.py
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/tests/test_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:59:47.387310 edx_i18n_tools-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-25 06:59:42.000000 edx_i18n_tools-1.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-25 06:59:42.000000 edx_i18n_tools-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-25 06:59:42.000000 edx_i18n_tools-1.6.0/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-04-25 06:59:47.387310 edx_i18n_tools-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-04-25 06:59:42.000000 edx_i18n_tools-1.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:59:47.387310 edx_i18n_tools-1.6.0/edx_i18n_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-04-25 06:59:47.000000 edx_i18n_tools-1.6.0/edx_i18n_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-25 06:59:47.000000 edx_i18n_tools-1.6.0/edx_i18n_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 06:59:47.000000 edx_i18n_tools-1.6.0/edx_i18n_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-25 06:59:47.000000 edx_i18n_tools-1.6.0/edx_i18n_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-25 06:59:47.000000 edx_i18n_tools-1.6.0/edx_i18n_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-25 06:59:47.000000 edx_i18n_tools-1.6.0/edx_i18n_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:59:47.387310 edx_i18n_tools-1.6.0/i18n/
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-25 06:59:42.000000 edx_i18n_tools-1.6.0/i18n/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-25 06:59:42.000000 edx_i18n_tools-1.6.0/i18n/branch_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-25 06:59:42.000000 edx_i18n_tools-1.6.0/i18n/changed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-04-25 06:59:42.000000 edx_i18n_tools-1.6.0/i18n/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-25 06:59:42.000000 edx_i18n_tools-1.6.0/i18n/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8965 2024-04-25 06:59:42.000000 edx_i18n_tools-1.6.0/i18n/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-25 06:59:42.000000 edx_i18n_tools-1.6.0/i18n/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12450 2024-04-25 06:59:42.000000 edx_i18n_tools-1.6.0/i18n/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8003 2024-04-25 06:59:42.000000 edx_i18n_tools-1.6.0/i18n/generate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1431 2024-04-25 06:59:42.000000 edx_i18n_tools-1.6.0/i18n/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-04-25 06:59:42.000000 edx_i18n_tools-1.6.0/i18n/segment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-04-25 06:59:42.000000 edx_i18n_tools-1.6.0/i18n/transifex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10162 2024-04-25 06:59:42.000000 edx_i18n_tools-1.6.0/i18n/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:59:47.387310 edx_i18n_tools-1.6.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-25 06:59:42.000000 edx_i18n_tools-1.6.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-25 06:59:47.387310 edx_i18n_tools-1.6.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2478 2024-04-25 06:59:42.000000 edx_i18n_tools-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:59:47.387310 edx_i18n_tools-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-25 06:59:42.000000 edx_i18n_tools-1.6.0/tests/test_changed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-25 06:59:42.000000 edx_i18n_tools-1.6.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-25 06:59:42.000000 edx_i18n_tools-1.6.0/tests/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-25 06:59:42.000000 edx_i18n_tools-1.6.0/tests/test_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9401 2024-04-25 06:59:42.000000 edx_i18n_tools-1.6.0/tests/test_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-04-25 06:59:42.000000 edx_i18n_tools-1.6.0/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-25 06:59:42.000000 edx_i18n_tools-1.6.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-25 06:59:42.000000 edx_i18n_tools-1.6.0/tests/test_segment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-04-25 06:59:42.000000 edx_i18n_tools-1.6.0/tests/test_transifex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-04-25 06:59:42.000000 edx_i18n_tools-1.6.0/tests/test_validate.py
```

### Comparing `edx-i18n-tools-1.5.0/LICENSE.txt` & `edx_i18n_tools-1.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.5.0/NOTICE.txt` & `edx_i18n_tools-1.6.0/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.5.0/PKG-INFO` & `edx_i18n_tools-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-i18n-tools
-Version: 1.5.0
+Version: 1.6.0
 Summary: edX Internationalization Tools
 Home-page: https://github.com/openedx/i18n-tools
 Author: edX
 Author-email: oscm@edx.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -15,18 +15,18 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 License-File: NOTICE.txt
-Requires-Dist: Django
-Requires-Dist: path
-Requires-Dist: lxml
 Requires-Dist: polib
+Requires-Dist: path
+Requires-Dist: Django
+Requires-Dist: lxml[html_clean]
 Requires-Dist: pyYaml
 
 edX i18n Tools |build-status| |coverage-status|
 ###############################################
 
 Installing
 ==========
```

### Comparing `edx-i18n-tools-1.5.0/README.rst` & `edx_i18n_tools-1.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.5.0/edx_i18n_tools.egg-info/PKG-INFO` & `edx_i18n_tools-1.6.0/edx_i18n_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-i18n-tools
-Version: 1.5.0
+Version: 1.6.0
 Summary: edX Internationalization Tools
 Home-page: https://github.com/openedx/i18n-tools
 Author: edX
 Author-email: oscm@edx.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -15,18 +15,18 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 License-File: NOTICE.txt
-Requires-Dist: Django
-Requires-Dist: path
-Requires-Dist: lxml
 Requires-Dist: polib
+Requires-Dist: path
+Requires-Dist: Django
+Requires-Dist: lxml[html_clean]
 Requires-Dist: pyYaml
 
 edX i18n Tools |build-status| |coverage-status|
 ###############################################
 
 Installing
 ==========
```

### Comparing `edx-i18n-tools-1.5.0/edx_i18n_tools.egg-info/SOURCES.txt` & `edx_i18n_tools-1.6.0/edx_i18n_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.5.0/i18n/__init__.py` & `edx_i18n_tools-1.6.0/i18n/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Tool to be used by other IDAs for internationalization.
 """
 import argparse
 import sys
 
 from . import config
 
-__version__ = '1.5.0'
+__version__ = '1.6.0'
 
 
 class Runner:
     """
     Runner class for internationalization.
     """
     def __init__(self):
```

### Comparing `edx-i18n-tools-1.5.0/i18n/branch_cleanup.py` & `edx_i18n_tools-1.6.0/i18n/branch_cleanup.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.5.0/i18n/changed.py` & `edx_i18n_tools-1.6.0/i18n/changed.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.5.0/i18n/config.py` & `edx_i18n_tools-1.6.0/i18n/config.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.5.0/i18n/converter.py` & `edx_i18n_tools-1.6.0/i18n/converter.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.5.0/i18n/dummy.py` & `edx_i18n_tools-1.6.0/i18n/dummy.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.5.0/i18n/execute.py` & `edx_i18n_tools-1.6.0/i18n/execute.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.5.0/i18n/extract.py` & `edx_i18n_tools-1.6.0/i18n/extract.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.5.0/i18n/generate.py` & `edx_i18n_tools-1.6.0/i18n/generate.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.5.0/i18n/main.py` & `edx_i18n_tools-1.6.0/i18n/main.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.5.0/i18n/segment.py` & `edx_i18n_tools-1.6.0/i18n/segment.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.5.0/i18n/transifex.py` & `edx_i18n_tools-1.6.0/i18n/transifex.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.5.0/i18n/validate.py` & `edx_i18n_tools-1.6.0/i18n/validate.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.5.0/setup.py` & `edx_i18n_tools-1.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.5.0/tests/test_changed.py` & `edx_i18n_tools-1.6.0/tests/test_changed.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.5.0/tests/test_config.py` & `edx_i18n_tools-1.6.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.5.0/tests/test_converter.py` & `edx_i18n_tools-1.6.0/tests/test_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,8 +58,8 @@
     def test_converter(self, data):
         """
         Tests with a simple converter (converts strings to uppercase).
         Assert that embedded HTML and python tags are not converted.
         """
         source, expected = data
         result = UpcaseConverter().convert(source)
-        self.assertEquals(result, expected)
+        self.assertEqual(result, expected)
```

### Comparing `edx-i18n-tools-1.5.0/tests/test_dummy.py` & `edx_i18n_tools-1.6.0/tests/test_dummy.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,22 +15,22 @@
     """
 
     def setUp(self):
         super().setUp()
         self.converter = dummy.Dummy()
 
     def assertUnicodeEquals(self, str1, str2):
-        """Just like assertEquals, but doesn't put Unicode into the fail message.
+        """Just like assertEqual, but doesn't put Unicode into the fail message.
 
         Either nose, or rake, or something, deals very badly with unusual
         Unicode characters in the assertions, so we use repr here to keep
         things safe.
 
         """
-        self.assertEquals(
+        self.assertEqual(
             str1, str2,
             "Mismatch: %r != %r" % (str1, str2),
         )
 
     @ddt.data(
         ("sign in",
          "sïgn ïn Ⱡ'σяєм ιρѕυм #"),
```

### Comparing `edx-i18n-tools-1.5.0/tests/test_extract.py` & `edx_i18n_tools-1.6.0/tests/test_extract.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
         Verify all metadata has been modified
         """
         for path in self.get_files():
             po = polib.pofile(path)
             metadata = po.metadata
             value = metadata['Report-Msgid-Bugs-To']
             expected = 'openedx-translation@googlegroups.com'
-            self.assertEquals(expected, value)
+            self.assertEqual(expected, value)
 
     @perform_extract_with_options()
     def test_metadata_fixed_creation_and_revision_dates(self):
         """
         Verify `POT-Creation-Date` and `PO-Revision-Date` metadata are always set to a fixed date-time
         """
         for path in self.get_files():
```

### Comparing `edx-i18n-tools-1.5.0/tests/test_generate.py` & `edx_i18n_tools-1.6.0/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.5.0/tests/test_integration.py` & `edx_i18n_tools-1.6.0/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.5.0/tests/test_segment.py` & `edx_i18n_tools-1.6.0/tests/test_segment.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.5.0/tests/test_transifex.py` & `edx_i18n_tools-1.6.0/tests/test_transifex.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,8 +100,8 @@
             )
 
     def test_clean_locale(self):
         with mock.patch('i18n.transifex.clean_file') as patched:
             transifex.clean_locale(self.configuration, 'fr')
             self.assertEqual(12, patched.call_count)
             for callarg in patched.call_args_list:
-                self.assertRegexpMatches(callarg[0][1].name, r'.*\.po')
+                self.assertRegex(callarg[0][1].name, r'.*\.po')
```

### Comparing `edx-i18n-tools-1.5.0/tests/test_validate.py` & `edx_i18n_tools-1.6.0/tests/test_validate.py`

 * *Files identical despite different names*

