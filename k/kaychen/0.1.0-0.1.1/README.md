# Comparing `tmp/kaychen-0.1.0.tar.gz` & `tmp/kaychen-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaychen-0.1.0.tar", last modified: Thu Apr 25 16:11:08 2024, max compression
+gzip compressed data, was "kaychen-0.1.1.tar", last modified: Thu Apr 25 18:20:04 2024, max compression
```

## Comparing `kaychen-0.1.0.tar` & `kaychen-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,15 @@
-drwxr-xr-x   0 kay       (1000) users      (984)        0 2024-04-25 16:11:08.826698 kaychen-0.1.0/
--rw-r--r--   0 kay       (1000) users      (984)      810 2024-04-25 16:11:08.826698 kaychen-0.1.0/PKG-INFO
-drwxr-xr-x   0 kay       (1000) users      (984)        0 2024-04-25 16:11:08.826698 kaychen-0.1.0/kaychen.egg-info/
--rw-r--r--   0 kay       (1000) users      (984)      810 2024-04-25 16:11:08.000000 kaychen-0.1.0/kaychen.egg-info/PKG-INFO
--rw-r--r--   0 kay       (1000) users      (984)      162 2024-04-25 16:11:08.000000 kaychen-0.1.0/kaychen.egg-info/SOURCES.txt
--rw-r--r--   0 kay       (1000) users      (984)        1 2024-04-25 16:11:08.000000 kaychen-0.1.0/kaychen.egg-info/dependency_links.txt
--rw-r--r--   0 kay       (1000) users      (984)      105 2024-04-25 16:11:08.000000 kaychen-0.1.0/kaychen.egg-info/requires.txt
--rw-r--r--   0 kay       (1000) users      (984)        1 2024-04-25 16:11:08.000000 kaychen-0.1.0/kaychen.egg-info/top_level.txt
--rw-r--r--   0 kay       (1000) users      (984)       38 2024-04-25 16:11:08.826698 kaychen-0.1.0/setup.cfg
--rw-r--r--   0 kay       (1000) users      (984)     3986 2024-04-25 16:02:50.000000 kaychen-0.1.0/setup.py
+drwxr-xr-x   0 kay       (1000) users      (984)        0 2024-04-25 18:20:04.680906 kaychen-0.1.1/
+-rw-r--r--   0 kay       (1000) users      (984)      810 2024-04-25 18:20:04.680906 kaychen-0.1.1/PKG-INFO
+drwxr-xr-x   0 kay       (1000) users      (984)        0 2024-04-25 18:20:04.677573 kaychen-0.1.1/kaychen/
+-rw-r--r--   0 kay       (1000) users      (984)        0 2024-04-25 18:17:40.000000 kaychen-0.1.1/kaychen/__init__.py
+-rw-r--r--   0 kay       (1000) users      (984)     3682 2024-04-25 15:50:52.000000 kaychen-0.1.1/kaychen/api.py
+-rw-r--r--   0 kay       (1000) users      (984)      669 2024-04-25 08:15:59.000000 kaychen-0.1.1/kaychen/middleware.py
+-rw-r--r--   0 kay       (1000) users      (984)     1093 2024-04-25 10:01:54.000000 kaychen-0.1.1/kaychen/response.py
+drwxr-xr-x   0 kay       (1000) users      (984)        0 2024-04-25 18:20:04.680906 kaychen-0.1.1/kaychen.egg-info/
+-rw-r--r--   0 kay       (1000) users      (984)      810 2024-04-25 18:20:04.000000 kaychen-0.1.1/kaychen.egg-info/PKG-INFO
+-rw-r--r--   0 kay       (1000) users      (984)      239 2024-04-25 18:20:04.000000 kaychen-0.1.1/kaychen.egg-info/SOURCES.txt
+-rw-r--r--   0 kay       (1000) users      (984)        1 2024-04-25 18:20:04.000000 kaychen-0.1.1/kaychen.egg-info/dependency_links.txt
+-rw-r--r--   0 kay       (1000) users      (984)      105 2024-04-25 18:20:04.000000 kaychen-0.1.1/kaychen.egg-info/requires.txt
+-rw-r--r--   0 kay       (1000) users      (984)        8 2024-04-25 18:20:04.000000 kaychen-0.1.1/kaychen.egg-info/top_level.txt
+-rw-r--r--   0 kay       (1000) users      (984)       38 2024-04-25 18:20:04.680906 kaychen-0.1.1/setup.cfg
+-rw-r--r--   0 kay       (1000) users      (984)     3986 2024-04-25 18:19:11.000000 kaychen-0.1.1/setup.py
```

### Comparing `kaychen-0.1.0/PKG-INFO` & `kaychen-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaychen
-Version: 0.1.0
+Version: 0.1.1
 Summary: This is a web framework build while completing the course https://testdriven.io/courses/python-web-framework/
 Home-page: https://github.com/Keisn1/web-framework-python.git
 Author: Kay Freyer
 Author-email: kay.freyer@icloud.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `kaychen-0.1.0/kaychen.egg-info/PKG-INFO` & `kaychen-0.1.1/kaychen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaychen
-Version: 0.1.0
+Version: 0.1.1
 Summary: This is a web framework build while completing the course https://testdriven.io/courses/python-web-framework/
 Home-page: https://github.com/Keisn1/web-framework-python.git
 Author: Kay Freyer
 Author-email: kay.freyer@icloud.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `kaychen-0.1.0/setup.py` & `kaychen-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = "kaychen"
 DESCRIPTION = "This is a web framework build while completing the course https://testdriven.io/courses/python-web-framework/"
 URL = "https://github.com/Keisn1/web-framework-python.git"
 EMAIL = "kay.freyer@icloud.com"
 AUTHOR = "Kay Freyer"
 REQUIRES_PYTHON = ">=3.11.0"
-VERSION = "0.1.0"
+VERSION = "0.1.1"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "Jinja2==3.1.3",
     "parse==1.20.1",
     "requests==2.31.0",
     "requests-wsgi-adapter==0.4.1",
```

