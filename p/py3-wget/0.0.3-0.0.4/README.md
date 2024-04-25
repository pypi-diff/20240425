# Comparing `tmp/py3_wget-0.0.3.tar.gz` & `tmp/py3_wget-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3_wget-0.0.3.tar", last modified: Wed Apr 24 23:40:04 2024, max compression
+gzip compressed data, was "py3_wget-0.0.4.tar", last modified: Wed Apr 24 23:42:45 2024, max compression
```

## Comparing `py3_wget-0.0.3.tar` & `py3_wget-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 gaber     (1000) gaber     (1000)        0 2024-04-24 23:40:04.161670 py3_wget-0.0.3/
--rw-rw-r--   0 gaber     (1000) gaber     (1000)     1072 2024-04-24 23:14:23.000000 py3_wget-0.0.3/LICENSE
--rw-r--r--   0 gaber     (1000) gaber     (1000)      686 2024-04-24 23:40:04.157670 py3_wget-0.0.3/PKG-INFO
--rw-rw-r--   0 gaber     (1000) gaber     (1000)       66 2024-04-24 23:29:58.000000 py3_wget-0.0.3/README.md
-drwxrwxr-x   0 gaber     (1000) gaber     (1000)        0 2024-04-24 23:40:04.157670 py3_wget-0.0.3/py3_wget/
--rw-rw-r--   0 gaber     (1000) gaber     (1000)       32 2024-04-24 23:39:45.000000 py3_wget-0.0.3/py3_wget/__init__.py
--rw-rw-r--   0 gaber     (1000) gaber     (1000)     1744 2024-04-24 23:32:58.000000 py3_wget-0.0.3/py3_wget/main.py
-drwxrwxr-x   0 gaber     (1000) gaber     (1000)        0 2024-04-24 23:40:04.157670 py3_wget-0.0.3/py3_wget.egg-info/
--rw-r--r--   0 gaber     (1000) gaber     (1000)      686 2024-04-24 23:40:04.000000 py3_wget-0.0.3/py3_wget.egg-info/PKG-INFO
--rw-rw-r--   0 gaber     (1000) gaber     (1000)      223 2024-04-24 23:40:04.000000 py3_wget-0.0.3/py3_wget.egg-info/SOURCES.txt
--rw-rw-r--   0 gaber     (1000) gaber     (1000)        1 2024-04-24 23:40:04.000000 py3_wget-0.0.3/py3_wget.egg-info/dependency_links.txt
--rw-rw-r--   0 gaber     (1000) gaber     (1000)       14 2024-04-24 23:40:04.000000 py3_wget-0.0.3/py3_wget.egg-info/requires.txt
--rw-rw-r--   0 gaber     (1000) gaber     (1000)        9 2024-04-24 23:40:04.000000 py3_wget-0.0.3/py3_wget.egg-info/top_level.txt
--rw-rw-r--   0 gaber     (1000) gaber     (1000)       38 2024-04-24 23:40:04.161670 py3_wget-0.0.3/setup.cfg
--rw-rw-r--   0 gaber     (1000) gaber     (1000)     1022 2024-04-24 23:39:55.000000 py3_wget-0.0.3/setup.py
+drwxrwxr-x   0 gaber     (1000) gaber     (1000)        0 2024-04-24 23:42:45.339780 py3_wget-0.0.4/
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)     1072 2024-04-24 23:14:23.000000 py3_wget-0.0.4/LICENSE
+-rw-r--r--   0 gaber     (1000) gaber     (1000)      686 2024-04-24 23:42:45.339780 py3_wget-0.0.4/PKG-INFO
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)       66 2024-04-24 23:29:58.000000 py3_wget-0.0.4/README.md
+drwxrwxr-x   0 gaber     (1000) gaber     (1000)        0 2024-04-24 23:42:45.335780 py3_wget-0.0.4/py3_wget/
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)       32 2024-04-24 23:39:45.000000 py3_wget-0.0.4/py3_wget/__init__.py
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)     1733 2024-04-24 23:42:34.000000 py3_wget-0.0.4/py3_wget/main.py
+drwxrwxr-x   0 gaber     (1000) gaber     (1000)        0 2024-04-24 23:42:45.339780 py3_wget-0.0.4/py3_wget.egg-info/
+-rw-r--r--   0 gaber     (1000) gaber     (1000)      686 2024-04-24 23:42:45.000000 py3_wget-0.0.4/py3_wget.egg-info/PKG-INFO
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)      223 2024-04-24 23:42:45.000000 py3_wget-0.0.4/py3_wget.egg-info/SOURCES.txt
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)        1 2024-04-24 23:42:45.000000 py3_wget-0.0.4/py3_wget.egg-info/dependency_links.txt
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)       14 2024-04-24 23:42:45.000000 py3_wget-0.0.4/py3_wget.egg-info/requires.txt
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)        9 2024-04-24 23:42:45.000000 py3_wget-0.0.4/py3_wget.egg-info/top_level.txt
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)       38 2024-04-24 23:42:45.339780 py3_wget-0.0.4/setup.cfg
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)     1022 2024-04-24 23:42:42.000000 py3_wget-0.0.4/setup.py
```

### Comparing `py3_wget-0.0.3/LICENSE` & `py3_wget-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py3_wget-0.0.3/PKG-INFO` & `py3_wget-0.0.4/py3_wget.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: py3_wget
-Version: 0.0.3
+Name: py3-wget
+Version: 0.0.4
 Summary: A simple tool to download files with python, supporting a progress bar
 Author: Gabriele Berton
 Author-email: <berton.gabri@gmail.com>
 Keywords: python,download,progress bar
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `py3_wget-0.0.3/py3_wget/main.py` & `py3_wget-0.0.4/py3_wget/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     for attempt_num in range(max_tries):  # In case of errors, try 'max_tries' times
         try:
             req = requests.get(url, stream=True)
             total_size = int(req.headers.get('content-length', 0))  # Total size in bytes
             block_size = 1024  # 1 KB
             tqdm_bar = tqdm(total=total_size, desc=os.path.basename(output_path),
-                            unit='iB', unit_scale=True, ncols=100)
+                            unit='iB', unit_scale=True)
             with open(tmp_filename, 'wb') as f:
                 for data in req.iter_content(block_size):
                     tqdm_bar.update(len(data))
                     f.write(data)
             tqdm_bar.close()
             if total_size != 0 and tqdm_bar.n != total_size:
                 print(tqdm_bar.n)
```

### Comparing `py3_wget-0.0.3/py3_wget.egg-info/PKG-INFO` & `py3_wget-0.0.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: py3-wget
-Version: 0.0.3
+Name: py3_wget
+Version: 0.0.4
 Summary: A simple tool to download files with python, supporting a progress bar
 Author: Gabriele Berton
 Author-email: <berton.gabri@gmail.com>
 Keywords: python,download,progress bar
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `py3_wget-0.0.3/setup.py` & `py3_wget-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'A simple tool to download files with python, supporting a progress bar'
 
 # Setting up
 setup(
     name="py3_wget",
     version=VERSION,
     author="Gabriele Berton",
```

