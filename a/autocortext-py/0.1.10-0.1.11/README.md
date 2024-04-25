# Comparing `tmp/autocortext_py-0.1.10.tar.gz` & `tmp/autocortext_py-0.1.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autocortext_py-0.1.10.tar", last modified: Thu Apr 25 10:23:42 2024, max compression
+gzip compressed data, was "autocortext_py-0.1.11.tar", last modified: Thu Apr 25 10:30:20 2024, max compression
```

## Comparing `autocortext_py-0.1.10.tar` & `autocortext_py-0.1.11.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mark       (502) staff       (20)        0 2024-04-25 10:23:42.492099 autocortext_py-0.1.10/
--rw-r--r--   0 mark       (502) staff       (20)     1072 2024-04-24 23:42:07.000000 autocortext_py-0.1.10/LICENSE
--rw-r--r--   0 mark       (502) staff       (20)     1370 2024-04-25 10:23:42.491949 autocortext_py-0.1.10/PKG-INFO
--rw-r--r--   0 mark       (502) staff       (20)      882 2024-04-25 01:47:51.000000 autocortext_py-0.1.10/README.md
-drwxr-xr-x   0 mark       (502) staff       (20)        0 2024-04-25 10:23:42.490810 autocortext_py-0.1.10/autocortext_py/
--rw-r--r--   0 mark       (502) staff       (20)       32 2024-04-24 23:10:13.000000 autocortext_py-0.1.10/autocortext_py/__init__.py
--rw-r--r--   0 mark       (502) staff       (20)     3518 2024-04-25 10:23:19.000000 autocortext_py-0.1.10/autocortext_py/client.py
-drwxr-xr-x   0 mark       (502) staff       (20)        0 2024-04-25 10:23:42.491582 autocortext_py-0.1.10/autocortext_py.egg-info/
--rw-r--r--   0 mark       (502) staff       (20)     1370 2024-04-25 10:23:42.000000 autocortext_py-0.1.10/autocortext_py.egg-info/PKG-INFO
--rw-r--r--   0 mark       (502) staff       (20)      267 2024-04-25 10:23:42.000000 autocortext_py-0.1.10/autocortext_py.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (502) staff       (20)        1 2024-04-25 10:23:42.000000 autocortext_py-0.1.10/autocortext_py.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (502) staff       (20)        9 2024-04-25 10:23:42.000000 autocortext_py-0.1.10/autocortext_py.egg-info/requires.txt
--rw-r--r--   0 mark       (502) staff       (20)       15 2024-04-25 10:23:42.000000 autocortext_py-0.1.10/autocortext_py.egg-info/top_level.txt
--rw-r--r--   0 mark       (502) staff       (20)       38 2024-04-25 10:23:42.492254 autocortext_py-0.1.10/setup.cfg
--rw-r--r--   0 mark       (502) staff       (20)      668 2024-04-25 10:23:34.000000 autocortext_py-0.1.10/setup.py
+drwxr-xr-x   0 mark       (502) staff       (20)        0 2024-04-25 10:30:20.095195 autocortext_py-0.1.11/
+-rw-r--r--   0 mark       (502) staff       (20)     1072 2024-04-24 23:42:07.000000 autocortext_py-0.1.11/LICENSE
+-rw-r--r--   0 mark       (502) staff       (20)     1389 2024-04-25 10:30:20.094985 autocortext_py-0.1.11/PKG-INFO
+-rw-r--r--   0 mark       (502) staff       (20)      901 2024-04-25 10:29:05.000000 autocortext_py-0.1.11/README.md
+drwxr-xr-x   0 mark       (502) staff       (20)        0 2024-04-25 10:30:20.093191 autocortext_py-0.1.11/autocortext_py/
+-rw-r--r--   0 mark       (502) staff       (20)       32 2024-04-24 23:10:13.000000 autocortext_py-0.1.11/autocortext_py/__init__.py
+-rw-r--r--   0 mark       (502) staff       (20)     3524 2024-04-25 10:28:35.000000 autocortext_py-0.1.11/autocortext_py/client.py
+drwxr-xr-x   0 mark       (502) staff       (20)        0 2024-04-25 10:30:20.094434 autocortext_py-0.1.11/autocortext_py.egg-info/
+-rw-r--r--   0 mark       (502) staff       (20)     1389 2024-04-25 10:30:20.000000 autocortext_py-0.1.11/autocortext_py.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (502) staff       (20)      267 2024-04-25 10:30:20.000000 autocortext_py-0.1.11/autocortext_py.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (502) staff       (20)        1 2024-04-25 10:30:20.000000 autocortext_py-0.1.11/autocortext_py.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (502) staff       (20)        9 2024-04-25 10:30:20.000000 autocortext_py-0.1.11/autocortext_py.egg-info/requires.txt
+-rw-r--r--   0 mark       (502) staff       (20)       15 2024-04-25 10:30:20.000000 autocortext_py-0.1.11/autocortext_py.egg-info/top_level.txt
+-rw-r--r--   0 mark       (502) staff       (20)       38 2024-04-25 10:30:20.095270 autocortext_py-0.1.11/setup.cfg
+-rw-r--r--   0 mark       (502) staff       (20)      668 2024-04-25 10:30:13.000000 autocortext_py-0.1.11/setup.py
```

### Comparing `autocortext_py-0.1.10/LICENSE` & `autocortext_py-0.1.11/LICENSE`

 * *Files identical despite different names*

### Comparing `autocortext_py-0.1.10/PKG-INFO` & `autocortext_py-0.1.11/autocortext_py.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: autocortext_py
-Version: 0.1.10
+Name: autocortext-py
+Version: 0.1.11
 Summary: Simple client for AutoCortext API
 Home-page: https://autocortext.com
 Author: Mark Watson
 Author-email: markus.c.watson@gmail.com
 License: UNKNOWN
 Keywords: autocortext
 Platform: UNKNOWN
@@ -31,30 +31,30 @@
 ```shell
 pip install autocortext-py
 ```
 
 Use the client in your source code.
 
 ```python
-from autocortext_py import AutoCortext
 import os
+from autocortext_py import AutoCortext
 from dotenv import load_dotenv
 
 load_dotenv()
 
 client = AutoCortext(
     org_id=os.getenv("AUTOCORTEXT_ORG_ID"),
     api_key=os.getenv("AUTOCORTEXT_API_KEY"),
 )
 
 query = [
-    {"id": 1, "content": "How can I help you?", "role": "assistant"},
+    {"id": 1, "content": "AutoCortext: How can I help you?", "role": "assistant"},
     {
         "id": 2,
-        "content": "The 24 volt system in the conveyor is not powering on.",
+        "content": "User: The 24 volt system in the conveyor is not powering on.",
         "role": "user",
     },
 ]
 
 res = client.troubleshoot(query)
 print(res)
 ```
```

### Comparing `autocortext_py-0.1.10/README.md` & `autocortext_py-0.1.11/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -14,30 +14,30 @@
 ```shell
 pip install autocortext-py
 ```
 
 Use the client in your source code.
 
 ```python
-from autocortext_py import AutoCortext
 import os
+from autocortext_py import AutoCortext
 from dotenv import load_dotenv
 
 load_dotenv()
 
 client = AutoCortext(
     org_id=os.getenv("AUTOCORTEXT_ORG_ID"),
     api_key=os.getenv("AUTOCORTEXT_API_KEY"),
 )
 
 query = [
-    {"id": 1, "content": "How can I help you?", "role": "assistant"},
+    {"id": 1, "content": "AutoCortext: How can I help you?", "role": "assistant"},
     {
         "id": 2,
-        "content": "The 24 volt system in the conveyor is not powering on.",
+        "content": "User: The 24 volt system in the conveyor is not powering on.",
         "role": "user",
     },
 ]
 
 res = client.troubleshoot(query)
 print(res)
 ```
```

### Comparing `autocortext_py-0.1.10/autocortext_py/client.py` & `autocortext_py-0.1.11/autocortext_py/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         # Ensure message is a list of dicts
         if isinstance(message, list) and all(isinstance(m, dict) for m in message):
             # Find the highest current ID and add 1
             max_id = max(msg["id"] for msg in message) if message else 0
             message.append(
                 {
                     "id": max_id + 1,
-                    "content": "Also, please keep your response as short as possible.",
+                    "content": "User: Also, please keep your response as short as possible.",
                     "role": "user",
                 }
             )
         else:
             raise ValueError(
                 "Message must be a list of dictionaries with at least an 'id' key."
             )
```

### Comparing `autocortext_py-0.1.10/autocortext_py.egg-info/PKG-INFO` & `autocortext_py-0.1.11/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: autocortext-py
-Version: 0.1.10
+Name: autocortext_py
+Version: 0.1.11
 Summary: Simple client for AutoCortext API
 Home-page: https://autocortext.com
 Author: Mark Watson
 Author-email: markus.c.watson@gmail.com
 License: UNKNOWN
 Keywords: autocortext
 Platform: UNKNOWN
@@ -31,30 +31,30 @@
 ```shell
 pip install autocortext-py
 ```
 
 Use the client in your source code.
 
 ```python
-from autocortext_py import AutoCortext
 import os
+from autocortext_py import AutoCortext
 from dotenv import load_dotenv
 
 load_dotenv()
 
 client = AutoCortext(
     org_id=os.getenv("AUTOCORTEXT_ORG_ID"),
     api_key=os.getenv("AUTOCORTEXT_API_KEY"),
 )
 
 query = [
-    {"id": 1, "content": "How can I help you?", "role": "assistant"},
+    {"id": 1, "content": "AutoCortext: How can I help you?", "role": "assistant"},
     {
         "id": 2,
-        "content": "The 24 volt system in the conveyor is not powering on.",
+        "content": "User: The 24 volt system in the conveyor is not powering on.",
         "role": "user",
     },
 ]
 
 res = client.troubleshoot(query)
 print(res)
 ```
```

### Comparing `autocortext_py-0.1.10/setup.py` & `autocortext_py-0.1.11/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="autocortext_py",
-    version="0.1.10",
+    version="0.1.11",
     description="Simple client for AutoCortext API",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Mark Watson",
     author_email="markus.c.watson@gmail.com",
     url="https://autocortext.com",
     keywords=["autocortext"],
```

