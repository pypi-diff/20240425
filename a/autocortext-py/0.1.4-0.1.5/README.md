# Comparing `tmp/autocortext_py-0.1.4.tar.gz` & `tmp/autocortext_py-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autocortext_py-0.1.4.tar", last modified: Thu Apr 25 00:31:09 2024, max compression
+gzip compressed data, was "autocortext_py-0.1.5.tar", last modified: Thu Apr 25 00:43:52 2024, max compression
```

## Comparing `autocortext_py-0.1.4.tar` & `autocortext_py-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mark       (502) staff       (20)        0 2024-04-25 00:31:09.671326 autocortext_py-0.1.4/
--rw-r--r--   0 mark       (502) staff       (20)     1072 2024-04-24 23:42:07.000000 autocortext_py-0.1.4/LICENSE
--rw-r--r--   0 mark       (502) staff       (20)     1247 2024-04-25 00:31:09.671172 autocortext_py-0.1.4/PKG-INFO
--rw-r--r--   0 mark       (502) staff       (20)      760 2024-04-25 00:30:52.000000 autocortext_py-0.1.4/README.md
-drwxr-xr-x   0 mark       (502) staff       (20)        0 2024-04-25 00:31:09.669929 autocortext_py-0.1.4/autocortext_py/
--rw-r--r--   0 mark       (502) staff       (20)       32 2024-04-24 23:10:13.000000 autocortext_py-0.1.4/autocortext_py/__init__.py
--rw-r--r--   0 mark       (502) staff       (20)      485 2024-04-25 00:29:55.000000 autocortext_py-0.1.4/autocortext_py/client.py
-drwxr-xr-x   0 mark       (502) staff       (20)        0 2024-04-25 00:31:09.670953 autocortext_py-0.1.4/autocortext_py.egg-info/
--rw-r--r--   0 mark       (502) staff       (20)     1247 2024-04-25 00:31:09.000000 autocortext_py-0.1.4/autocortext_py.egg-info/PKG-INFO
--rw-r--r--   0 mark       (502) staff       (20)      267 2024-04-25 00:31:09.000000 autocortext_py-0.1.4/autocortext_py.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (502) staff       (20)        1 2024-04-25 00:31:09.000000 autocortext_py-0.1.4/autocortext_py.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (502) staff       (20)        9 2024-04-25 00:31:09.000000 autocortext_py-0.1.4/autocortext_py.egg-info/requires.txt
--rw-r--r--   0 mark       (502) staff       (20)       15 2024-04-25 00:31:09.000000 autocortext_py-0.1.4/autocortext_py.egg-info/top_level.txt
--rw-r--r--   0 mark       (502) staff       (20)       38 2024-04-25 00:31:09.671375 autocortext_py-0.1.4/setup.cfg
--rw-r--r--   0 mark       (502) staff       (20)      667 2024-04-25 00:31:01.000000 autocortext_py-0.1.4/setup.py
+drwxr-xr-x   0 mark       (502) staff       (20)        0 2024-04-25 00:43:52.827152 autocortext_py-0.1.5/
+-rw-r--r--   0 mark       (502) staff       (20)     1072 2024-04-24 23:42:07.000000 autocortext_py-0.1.5/LICENSE
+-rw-r--r--   0 mark       (502) staff       (20)     1283 2024-04-25 00:43:52.827000 autocortext_py-0.1.5/PKG-INFO
+-rw-r--r--   0 mark       (502) staff       (20)      796 2024-04-25 00:39:28.000000 autocortext_py-0.1.5/README.md
+drwxr-xr-x   0 mark       (502) staff       (20)        0 2024-04-25 00:43:52.826090 autocortext_py-0.1.5/autocortext_py/
+-rw-r--r--   0 mark       (502) staff       (20)       32 2024-04-24 23:10:13.000000 autocortext_py-0.1.5/autocortext_py/__init__.py
+-rw-r--r--   0 mark       (502) staff       (20)     1043 2024-04-25 00:43:42.000000 autocortext_py-0.1.5/autocortext_py/client.py
+drwxr-xr-x   0 mark       (502) staff       (20)        0 2024-04-25 00:43:52.826797 autocortext_py-0.1.5/autocortext_py.egg-info/
+-rw-r--r--   0 mark       (502) staff       (20)     1283 2024-04-25 00:43:52.000000 autocortext_py-0.1.5/autocortext_py.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (502) staff       (20)      267 2024-04-25 00:43:52.000000 autocortext_py-0.1.5/autocortext_py.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (502) staff       (20)        1 2024-04-25 00:43:52.000000 autocortext_py-0.1.5/autocortext_py.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (502) staff       (20)        9 2024-04-25 00:43:52.000000 autocortext_py-0.1.5/autocortext_py.egg-info/requires.txt
+-rw-r--r--   0 mark       (502) staff       (20)       15 2024-04-25 00:43:52.000000 autocortext_py-0.1.5/autocortext_py.egg-info/top_level.txt
+-rw-r--r--   0 mark       (502) staff       (20)       38 2024-04-25 00:43:52.827208 autocortext_py-0.1.5/setup.cfg
+-rw-r--r--   0 mark       (502) staff       (20)      667 2024-04-25 00:43:49.000000 autocortext_py-0.1.5/setup.py
```

### Comparing `autocortext_py-0.1.4/LICENSE` & `autocortext_py-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `autocortext_py-0.1.4/PKG-INFO` & `autocortext_py-0.1.5/autocortext_py.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: autocortext_py
-Version: 0.1.4
+Name: autocortext-py
+Version: 0.1.5
 Summary: Simple client for AutoCortext API
 Home-page: https://autocortext.com
 Author: Mark Watson
 Author-email: markus.c.watson@gmail.com
 License: UNKNOWN
 Keywords: autocortext
 Platform: UNKNOWN
@@ -33,18 +33,21 @@
 ```
 
 Use the client in your source code.
 
 ```python
 from autocortext_py import AutoCortext
 import os
+from dotenv import load_dotenv
+
+load_dotenv()
 
 client = AutoCortext(
-    org_id=os.environ.get("AUTOCORTEXT_ORG_ID"),
-    api_key=os.environ.get("AUTOCORTEXT_API_KEY"),
+    org_id=os.getenv("AUTOCORTEXT_ORG_ID"),
+    api_key=os.getenv("AUTOCORTEXT_API_KEY"),
 )
 
 query = '[{ "id":1, "content":"How can I help you?" ,"role":"assistant"}, { "id":2, "content":"Why is the sky blue?","role":"user"}]'
 
 res = client.troubleshoot(query)
 print(res)
 ```
```

### Comparing `autocortext_py-0.1.4/README.md` & `autocortext_py-0.1.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -16,18 +16,21 @@
 ```
 
 Use the client in your source code.
 
 ```python
 from autocortext_py import AutoCortext
 import os
+from dotenv import load_dotenv
+
+load_dotenv()
 
 client = AutoCortext(
-    org_id=os.environ.get("AUTOCORTEXT_ORG_ID"),
-    api_key=os.environ.get("AUTOCORTEXT_API_KEY"),
+    org_id=os.getenv("AUTOCORTEXT_ORG_ID"),
+    api_key=os.getenv("AUTOCORTEXT_API_KEY"),
 )
 
 query = '[{ "id":1, "content":"How can I help you?" ,"role":"assistant"}, { "id":2, "content":"Why is the sky blue?","role":"user"}]'
 
 res = client.troubleshoot(query)
 print(res)
 ```
```

### Comparing `autocortext_py-0.1.4/autocortext_py.egg-info/PKG-INFO` & `autocortext_py-0.1.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: autocortext-py
-Version: 0.1.4
+Name: autocortext_py
+Version: 0.1.5
 Summary: Simple client for AutoCortext API
 Home-page: https://autocortext.com
 Author: Mark Watson
 Author-email: markus.c.watson@gmail.com
 License: UNKNOWN
 Keywords: autocortext
 Platform: UNKNOWN
@@ -33,18 +33,21 @@
 ```
 
 Use the client in your source code.
 
 ```python
 from autocortext_py import AutoCortext
 import os
+from dotenv import load_dotenv
+
+load_dotenv()
 
 client = AutoCortext(
-    org_id=os.environ.get("AUTOCORTEXT_ORG_ID"),
-    api_key=os.environ.get("AUTOCORTEXT_API_KEY"),
+    org_id=os.getenv("AUTOCORTEXT_ORG_ID"),
+    api_key=os.getenv("AUTOCORTEXT_API_KEY"),
 )
 
 query = '[{ "id":1, "content":"How can I help you?" ,"role":"assistant"}, { "id":2, "content":"Why is the sky blue?","role":"user"}]'
 
 res = client.troubleshoot(query)
 print(res)
 ```
```

### Comparing `autocortext_py-0.1.4/setup.py` & `autocortext_py-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="autocortext_py",
-    version="0.1.4",
+    version="0.1.5",
     description="Simple client for AutoCortext API",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Mark Watson",
     author_email="markus.c.watson@gmail.com",
     url="https://autocortext.com",
     keywords=["autocortext"],
```

