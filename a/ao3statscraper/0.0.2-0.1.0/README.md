# Comparing `tmp/ao3statscraper-0.0.2.tar.gz` & `tmp/ao3statscraper-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ao3statscraper-0.0.2.tar", last modified: Wed Apr 24 22:55:47 2024, max compression
+gzip compressed data, was "ao3statscraper-0.1.0.tar", last modified: Wed Apr 24 23:05:01 2024, max compression
```

## Comparing `ao3statscraper-0.0.2.tar` & `ao3statscraper-0.1.0.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-04-24 22:55:47.801983 ao3statscraper-0.0.2/
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)    35137 2024-04-10 17:46:52.000000 ao3statscraper-0.0.2/LICENSE
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      220 2024-04-24 14:13:41.000000 ao3statscraper-0.0.2/MANIFEST.in
--rw-r--r--   0 mivkov    (1000) mivkov    (1000)    47047 2024-04-24 22:55:47.801983 ao3statscraper-0.0.2/PKG-INFO
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     5669 2024-04-24 22:54:15.000000 ao3statscraper-0.0.2/README.md
-drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-04-24 22:55:47.801983 ao3statscraper-0.0.2/ao3statscraper/
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      523 2024-04-24 14:13:41.000000 ao3statscraper-0.0.2/ao3statscraper/__init__.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)       22 2024-04-24 22:55:41.000000 ao3statscraper-0.0.2/ao3statscraper/__version__.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     2355 2024-04-24 14:13:41.000000 ao3statscraper-0.0.2/ao3statscraper/ao3requester.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     6517 2024-04-24 21:10:25.000000 ao3statscraper-0.0.2/ao3statscraper/configuration.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     6530 2024-04-24 14:13:41.000000 ao3statscraper-0.0.2/ao3statscraper/plotting.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     3862 2024-04-24 14:13:41.000000 ao3statscraper-0.0.2/ao3statscraper/pw.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     8015 2024-04-24 22:00:25.000000 ao3statscraper-0.0.2/ao3statscraper/scrape.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)    11255 2024-04-24 14:13:41.000000 ao3statscraper-0.0.2/ao3statscraper/statsdata.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     1396 2024-04-24 14:13:41.000000 ao3statscraper-0.0.2/ao3statscraper/utils.py
-drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-04-24 22:55:47.801983 ao3statscraper-0.0.2/ao3statscraper.egg-info/
--rw-r--r--   0 mivkov    (1000) mivkov    (1000)    47047 2024-04-24 22:55:47.000000 ao3statscraper-0.0.2/ao3statscraper.egg-info/PKG-INFO
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      570 2024-04-24 22:55:47.000000 ao3statscraper-0.0.2/ao3statscraper.egg-info/SOURCES.txt
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)        1 2024-04-24 22:55:47.000000 ao3statscraper-0.0.2/ao3statscraper.egg-info/dependency_links.txt
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      263 2024-04-24 22:55:47.000000 ao3statscraper-0.0.2/ao3statscraper.egg-info/entry_points.txt
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      109 2024-04-24 22:55:47.000000 ao3statscraper-0.0.2/ao3statscraper.egg-info/requires.txt
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)       15 2024-04-24 22:55:47.000000 ao3statscraper-0.0.2/ao3statscraper.egg-info/top_level.txt
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     1586 2024-04-24 22:55:41.000000 ao3statscraper-0.0.2/pyproject.toml
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)       38 2024-04-24 22:55:47.801983 ao3statscraper-0.0.2/setup.cfg
-drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-04-24 22:55:47.801983 ao3statscraper-0.0.2/tests/
--rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)      933 2024-04-24 14:13:41.000000 ao3statscraper-0.0.2/tests/test_passwords.py
--rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)      642 2024-04-24 14:13:41.000000 ao3statscraper-0.0.2/tests/test_writing_data.py
+drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-04-24 23:05:01.368738 ao3statscraper-0.1.0/
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)    35137 2024-04-10 17:46:52.000000 ao3statscraper-0.1.0/LICENSE
+-rw-r--r--   0 mivkov    (1000) mivkov    (1000)    47047 2024-04-24 23:05:01.368738 ao3statscraper-0.1.0/PKG-INFO
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     5669 2024-04-24 22:54:15.000000 ao3statscraper-0.1.0/README.md
+drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-04-24 23:05:01.368738 ao3statscraper-0.1.0/ao3statscraper/
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      523 2024-04-24 14:13:41.000000 ao3statscraper-0.1.0/ao3statscraper/__init__.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)       22 2024-04-24 23:04:55.000000 ao3statscraper-0.1.0/ao3statscraper/__version__.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     2428 2024-04-24 23:01:50.000000 ao3statscraper-0.1.0/ao3statscraper/ao3requester.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     6508 2024-04-24 22:59:18.000000 ao3statscraper-0.1.0/ao3statscraper/configuration.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     6530 2024-04-24 14:13:41.000000 ao3statscraper-0.1.0/ao3statscraper/plotting.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     3862 2024-04-24 14:13:41.000000 ao3statscraper-0.1.0/ao3statscraper/pw.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     8015 2024-04-24 22:00:25.000000 ao3statscraper-0.1.0/ao3statscraper/scrape.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)    11255 2024-04-24 14:13:41.000000 ao3statscraper-0.1.0/ao3statscraper/statsdata.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     1396 2024-04-24 14:13:41.000000 ao3statscraper-0.1.0/ao3statscraper/utils.py
+drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-04-24 23:05:01.368738 ao3statscraper-0.1.0/ao3statscraper.egg-info/
+-rw-r--r--   0 mivkov    (1000) mivkov    (1000)    47047 2024-04-24 23:05:01.000000 ao3statscraper-0.1.0/ao3statscraper.egg-info/PKG-INFO
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      558 2024-04-24 23:05:01.000000 ao3statscraper-0.1.0/ao3statscraper.egg-info/SOURCES.txt
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)        1 2024-04-24 23:05:01.000000 ao3statscraper-0.1.0/ao3statscraper.egg-info/dependency_links.txt
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      263 2024-04-24 23:05:01.000000 ao3statscraper-0.1.0/ao3statscraper.egg-info/entry_points.txt
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      109 2024-04-24 23:05:01.000000 ao3statscraper-0.1.0/ao3statscraper.egg-info/requires.txt
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)       15 2024-04-24 23:05:01.000000 ao3statscraper-0.1.0/ao3statscraper.egg-info/top_level.txt
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     1586 2024-04-24 23:04:55.000000 ao3statscraper-0.1.0/pyproject.toml
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)       38 2024-04-24 23:05:01.368738 ao3statscraper-0.1.0/setup.cfg
+drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-04-24 23:05:01.368738 ao3statscraper-0.1.0/tests/
+-rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)      933 2024-04-24 14:13:41.000000 ao3statscraper-0.1.0/tests/test_passwords.py
+-rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)      642 2024-04-24 14:13:41.000000 ao3statscraper-0.1.0/tests/test_writing_data.py
```

### Comparing `ao3statscraper-0.0.2/LICENSE` & `ao3statscraper-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.0.2/PKG-INFO` & `ao3statscraper-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ao3statscraper
-Version: 0.0.2
+Version: 0.1.0
 Summary: Scrape stats from your AO3 stats page.
 Author-email: Lars Ikarion <lars.ikarion@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ao3statscraper-0.0.2/README.md` & `ao3statscraper-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.0.2/ao3statscraper/__init__.py` & `ao3statscraper-0.1.0/ao3statscraper/__init__.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.0.2/ao3statscraper/ao3requester.py` & `ao3statscraper-0.1.0/ao3statscraper/ao3requester.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import requests
 
 
 class Requester:
-    """Requester object"""
+    """Requester object
+
+       Mostly lifted from https://github.com/ArmindoFlores/ao3_api
+    """
 
     def __init__(self, rqtw=-1, timew=60):
         """Limits the request rate to prevent HTTP 429 (rate limiting) responses.
         12 request per minute seems to be the limit.
 
         Args:
             rqm (int, optional): Maximum requests per time window (-1 -> no limit). Defaults to -1.
```

### Comparing `ao3statscraper-0.0.2/ao3statscraper/configuration.py` & `ao3statscraper-0.1.0/ao3statscraper/configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 
 
 import os
 import platform
 import yaml
+import pathlib
 from getpass import getpass
 
 from .utils import clear_terminal
 from .pw import get_credentials, read_secrets, store_secrets
 
 
 class PlottingConfig(object):
@@ -35,19 +36,18 @@
     def __init__(self, reset_conffile=False):
         """
         Initialize configuration.
         If `reset_conffile` is True, then write a new config file from scratch
         and exit.
         """
 
-        if platform.system() == "Windows":
-            raise NotImplementedError("Setup for windows is ToDo")
+        # TODO: storing stuff in .ao3statscraper is probably not the way to go on windows
 
         # Get config directory
-        userdir = os.path.expanduser("~")
+        userdir = pathlib.Path.home()
         ao3dir = os.path.join(userdir, ".ao3statscraper")
         self.ao3dir = ao3dir
 
         # Make sure it exists.
         try:
             os.mkdir(ao3dir)
         except FileExistsError:
```

### Comparing `ao3statscraper-0.0.2/ao3statscraper/plotting.py` & `ao3statscraper-0.1.0/ao3statscraper/plotting.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.0.2/ao3statscraper/pw.py` & `ao3statscraper-0.1.0/ao3statscraper/pw.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.0.2/ao3statscraper/scrape.py` & `ao3statscraper-0.1.0/ao3statscraper/scrape.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.0.2/ao3statscraper/statsdata.py` & `ao3statscraper-0.1.0/ao3statscraper/statsdata.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.0.2/ao3statscraper/utils.py` & `ao3statscraper-0.1.0/ao3statscraper/utils.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.0.2/ao3statscraper.egg-info/PKG-INFO` & `ao3statscraper-0.1.0/ao3statscraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ao3statscraper
-Version: 0.0.2
+Version: 0.1.0
 Summary: Scrape stats from your AO3 stats page.
 Author-email: Lars Ikarion <lars.ikarion@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ao3statscraper-0.0.2/ao3statscraper.egg-info/SOURCES.txt` & `ao3statscraper-0.1.0/ao3statscraper.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 LICENSE
-MANIFEST.in
 README.md
 pyproject.toml
 ao3statscraper/__init__.py
 ao3statscraper/__version__.py
 ao3statscraper/ao3requester.py
 ao3statscraper/configuration.py
 ao3statscraper/plotting.py
```

### Comparing `ao3statscraper-0.0.2/pyproject.toml` & `ao3statscraper-0.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.setuptools]
 packages = ["ao3statscraper"]
 
 [project]
 name = "ao3statscraper"
 description="Scrape stats from your AO3 stats page."
 readme = "README.md"
-version = "0.0.2"
+version = "0.1.0"
 authors= [
     { name = "Lars Ikarion", email="lars.ikarion@gmail.com"},
     ]
 license = { file = "LICENSE" }
 classifiers=[
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -43,15 +43,15 @@
 ao3get= "ao3statscraper.scripts:ao3scrape"
 
 
 [project.urls]
 "Homepage" = "https://gitlab.com/athenaslilowl1/AO3StatScraper"
 
 [tool.bumpver]
-current_version = "0.0.2"
+current_version = "0.1.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `ao3statscraper-0.0.2/tests/test_passwords.py` & `ao3statscraper-0.1.0/tests/test_passwords.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.0.2/tests/test_writing_data.py` & `ao3statscraper-0.1.0/tests/test_writing_data.py`

 * *Files identical despite different names*

