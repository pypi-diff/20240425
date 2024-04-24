# Comparing `tmp/py3_wget-0.0.1.tar.gz` & `tmp/py3_wget-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3_wget-0.0.1.tar", last modified: Wed Apr 24 23:30:37 2024, max compression
+gzip compressed data, was "py3_wget-0.0.2.tar", last modified: Wed Apr 24 23:38:26 2024, max compression
```

## Comparing `py3_wget-0.0.1.tar` & `py3_wget-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 gaber     (1000) gaber     (1000)        0 2024-04-24 23:30:37.451730 py3_wget-0.0.1/
--rw-rw-r--   0 gaber     (1000) gaber     (1000)     1072 2024-04-24 23:14:23.000000 py3_wget-0.0.1/LICENSE
--rw-r--r--   0 gaber     (1000) gaber     (1000)      686 2024-04-24 23:30:37.451730 py3_wget-0.0.1/PKG-INFO
--rw-rw-r--   0 gaber     (1000) gaber     (1000)       66 2024-04-24 23:29:58.000000 py3_wget-0.0.1/README.md
-drwxrwxr-x   0 gaber     (1000) gaber     (1000)        0 2024-04-24 23:30:37.451730 py3_wget-0.0.1/py3_wget/
--rw-rw-r--   0 gaber     (1000) gaber     (1000)       35 2024-04-24 23:29:25.000000 py3_wget-0.0.1/py3_wget/__init__.py
--rw-rw-r--   0 gaber     (1000) gaber     (1000)     1750 2024-04-24 23:12:21.000000 py3_wget-0.0.1/py3_wget/py3_wget.py
-drwxrwxr-x   0 gaber     (1000) gaber     (1000)        0 2024-04-24 23:30:37.451730 py3_wget-0.0.1/py3_wget.egg-info/
--rw-r--r--   0 gaber     (1000) gaber     (1000)      686 2024-04-24 23:30:37.000000 py3_wget-0.0.1/py3_wget.egg-info/PKG-INFO
--rw-rw-r--   0 gaber     (1000) gaber     (1000)      227 2024-04-24 23:30:37.000000 py3_wget-0.0.1/py3_wget.egg-info/SOURCES.txt
--rw-rw-r--   0 gaber     (1000) gaber     (1000)        1 2024-04-24 23:30:37.000000 py3_wget-0.0.1/py3_wget.egg-info/dependency_links.txt
--rw-rw-r--   0 gaber     (1000) gaber     (1000)       14 2024-04-24 23:30:37.000000 py3_wget-0.0.1/py3_wget.egg-info/requires.txt
--rw-rw-r--   0 gaber     (1000) gaber     (1000)        9 2024-04-24 23:30:37.000000 py3_wget-0.0.1/py3_wget.egg-info/top_level.txt
--rw-rw-r--   0 gaber     (1000) gaber     (1000)       38 2024-04-24 23:30:37.451730 py3_wget-0.0.1/setup.cfg
--rw-rw-r--   0 gaber     (1000) gaber     (1000)     1022 2024-04-24 23:30:07.000000 py3_wget-0.0.1/setup.py
+drwxrwxr-x   0 gaber     (1000) gaber     (1000)        0 2024-04-24 23:38:26.948289 py3_wget-0.0.2/
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)     1072 2024-04-24 23:14:23.000000 py3_wget-0.0.2/LICENSE
+-rw-r--r--   0 gaber     (1000) gaber     (1000)      686 2024-04-24 23:38:26.948289 py3_wget-0.0.2/PKG-INFO
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)       66 2024-04-24 23:29:58.000000 py3_wget-0.0.2/README.md
+drwxrwxr-x   0 gaber     (1000) gaber     (1000)        0 2024-04-24 23:38:26.944289 py3_wget-0.0.2/py3_wget/
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)       37 2024-04-24 23:36:53.000000 py3_wget-0.0.2/py3_wget/__init__.py
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)     1744 2024-04-24 23:32:58.000000 py3_wget-0.0.2/py3_wget/downloader.py
+drwxrwxr-x   0 gaber     (1000) gaber     (1000)        0 2024-04-24 23:38:26.948289 py3_wget-0.0.2/py3_wget.egg-info/
+-rw-r--r--   0 gaber     (1000) gaber     (1000)      686 2024-04-24 23:38:26.000000 py3_wget-0.0.2/py3_wget.egg-info/PKG-INFO
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)      229 2024-04-24 23:38:26.000000 py3_wget-0.0.2/py3_wget.egg-info/SOURCES.txt
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)        1 2024-04-24 23:38:26.000000 py3_wget-0.0.2/py3_wget.egg-info/dependency_links.txt
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)       14 2024-04-24 23:38:26.000000 py3_wget-0.0.2/py3_wget.egg-info/requires.txt
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)        9 2024-04-24 23:38:26.000000 py3_wget-0.0.2/py3_wget.egg-info/top_level.txt
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)       38 2024-04-24 23:38:26.948289 py3_wget-0.0.2/setup.cfg
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)     1022 2024-04-24 23:38:06.000000 py3_wget-0.0.2/setup.py
```

### Comparing `py3_wget-0.0.1/LICENSE` & `py3_wget-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py3_wget-0.0.1/PKG-INFO` & `py3_wget-0.0.2/py3_wget.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: py3_wget
-Version: 0.0.1
+Name: py3-wget
+Version: 0.0.2
 Summary: A simple tool to download files with python, supporting a progress bar
 Author: Gabriele Berton
 Author-email: <berton.gabri@gmail.com>
 Keywords: python,download,progress bar
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `py3_wget-0.0.1/py3_wget/py3_wget.py` & `py3_wget-0.0.2/py3_wget/downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import shutil
 import requests
 from tqdm import tqdm
 
 RETRY_SECONDS = 2
 
 
-def download_heavy_file(url, output_path, max_tries=10):
+def download_file(url, output_path, max_tries=10):
     tmp_filename = os.path.join(f".tmp_{int(time.time()*1000)}")
     if os.path.exists(output_path):
         print(f"File {output_path} already exists, I won't download it again")
         return
     
     for attempt_num in range(max_tries):  # In case of errors, try 'max_tries' times
         try:
```

### Comparing `py3_wget-0.0.1/py3_wget.egg-info/PKG-INFO` & `py3_wget-0.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: py3-wget
-Version: 0.0.1
+Name: py3_wget
+Version: 0.0.2
 Summary: A simple tool to download files with python, supporting a progress bar
 Author: Gabriele Berton
 Author-email: <berton.gabri@gmail.com>
 Keywords: python,download,progress bar
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `py3_wget-0.0.1/setup.py` & `py3_wget-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'A simple tool to download files with python, supporting a progress bar'
 
 # Setting up
 setup(
     name="py3_wget",
     version=VERSION,
     author="Gabriele Berton",
```

