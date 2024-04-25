# Comparing `tmp/autocortext_py-0.1.10.tar.gz` & `tmp/autocortext_py-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autocortext_py-0.1.10.tar", last modified: Thu Apr 25 10:23:42 2024, max compression
+gzip compressed data, was "autocortext_py-0.1.9.tar", last modified: Thu Apr 25 01:48:39 2024, max compression
```

## Comparing `autocortext_py-0.1.10.tar` & `autocortext_py-0.1.9.tar`

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
+drwxr-xr-x   0 mark       (502) staff       (20)        0 2024-04-25 01:48:39.932837 autocortext_py-0.1.9/
+-rw-r--r--   0 mark       (502) staff       (20)     1072 2024-04-24 23:42:07.000000 autocortext_py-0.1.9/LICENSE
+-rw-r--r--   0 mark       (502) staff       (20)     1369 2024-04-25 01:48:39.932659 autocortext_py-0.1.9/PKG-INFO
+-rw-r--r--   0 mark       (502) staff       (20)      882 2024-04-25 01:47:51.000000 autocortext_py-0.1.9/README.md
+drwxr-xr-x   0 mark       (502) staff       (20)        0 2024-04-25 01:48:39.931601 autocortext_py-0.1.9/autocortext_py/
+-rw-r--r--   0 mark       (502) staff       (20)       32 2024-04-24 23:10:13.000000 autocortext_py-0.1.9/autocortext_py/__init__.py
+-rw-r--r--   0 mark       (502) staff       (20)     2138 2024-04-25 01:27:13.000000 autocortext_py-0.1.9/autocortext_py/client.py
+drwxr-xr-x   0 mark       (502) staff       (20)        0 2024-04-25 01:48:39.932406 autocortext_py-0.1.9/autocortext_py.egg-info/
+-rw-r--r--   0 mark       (502) staff       (20)     1369 2024-04-25 01:48:39.000000 autocortext_py-0.1.9/autocortext_py.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (502) staff       (20)      267 2024-04-25 01:48:39.000000 autocortext_py-0.1.9/autocortext_py.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (502) staff       (20)        1 2024-04-25 01:48:39.000000 autocortext_py-0.1.9/autocortext_py.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (502) staff       (20)        9 2024-04-25 01:48:39.000000 autocortext_py-0.1.9/autocortext_py.egg-info/requires.txt
+-rw-r--r--   0 mark       (502) staff       (20)       15 2024-04-25 01:48:39.000000 autocortext_py-0.1.9/autocortext_py.egg-info/top_level.txt
+-rw-r--r--   0 mark       (502) staff       (20)       38 2024-04-25 01:48:39.932908 autocortext_py-0.1.9/setup.cfg
+-rw-r--r--   0 mark       (502) staff       (20)      667 2024-04-25 01:48:36.000000 autocortext_py-0.1.9/setup.py
```

### Comparing `autocortext_py-0.1.10/LICENSE` & `autocortext_py-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `autocortext_py-0.1.10/PKG-INFO` & `autocortext_py-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autocortext_py
-Version: 0.1.10
+Version: 0.1.9
 Summary: Simple client for AutoCortext API
 Home-page: https://autocortext.com
 Author: Mark Watson
 Author-email: markus.c.watson@gmail.com
 License: UNKNOWN
 Keywords: autocortext
 Platform: UNKNOWN
```

### Comparing `autocortext_py-0.1.10/README.md` & `autocortext_py-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `autocortext_py-0.1.10/autocortext_py/client.py` & `autocortext_py-0.1.9/autocortext_py/client.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,66 +1,29 @@
 import requests
 import json
 
 
 class AutoCortext:
-    """
-    A client for interacting with the AutoCortext API.
-
-    This class provides methods to send messages and receive responses from the AutoCortext API.
-
-    Attributes:
-        org_id (str): The organization ID required for API requests.
-        api_key (str): The API key used for secure communication with the API.
-        base_url (str): The base URL for the API endpoints.
-    """
-
     def __init__(self, org_id, api_key):
-        """
-        Initializes the AutoCortext client with necessary authentication credentials.
-
-        Args:
-            org_id (str): The organization ID for the API.
-            api_key (str): The API key for accessing the API.
-
-        Raises:
-            ValueError: If either org_id or api_key is not provided.
-        """
         if not org_id:
             raise ValueError("Organization ID must be provided and cannot be empty.")
         if not api_key:
             raise ValueError("API key must be provided and cannot be empty.")
 
         self.base_url = "https://ascend-six.vercel.app/"
         self.org_id = org_id
         self.headers = {
             "Authorization": f"Bearer {api_key}",
             "Content-Type": "application/json",
         }
 
     def troubleshoot(self, message):
-        """
-        Sends a troubleshooting message to the API and returns the response.
-
-        The method expects a message in the form of a string or a dictionary and sends it
-        as a JSON payload to the API's troubleshooting endpoint.
-
-        Args:
-            message (str or dict): The message or context to be sent for troubleshooting.
-
-        Returns:
-            str: The response from the API, typically containing troubleshooting information.
-
-        Raises:
-            ValueError: If the message is neither a string nor a dictionary.
-            JSONDecodeError: If the response from the API is not valid JSON.
-        """
+        # Convert message to a Python dict if it's not already one
         if isinstance(message, str):
             try:
-                # Convert message to a Python dict if it's not already one
                 message = json.loads(message)
             except json.JSONDecodeError:
                 raise ValueError("Message must be a valid JSON string or a dictionary.")
 
         # Ensure message is a list of dicts
         if isinstance(message, list) and all(isinstance(m, dict) for m in message):
             # Find the highest current ID and add 1
```

### Comparing `autocortext_py-0.1.10/autocortext_py.egg-info/PKG-INFO` & `autocortext_py-0.1.9/autocortext_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autocortext-py
-Version: 0.1.10
+Version: 0.1.9
 Summary: Simple client for AutoCortext API
 Home-page: https://autocortext.com
 Author: Mark Watson
 Author-email: markus.c.watson@gmail.com
 License: UNKNOWN
 Keywords: autocortext
 Platform: UNKNOWN
```

### Comparing `autocortext_py-0.1.10/setup.py` & `autocortext_py-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="autocortext_py",
-    version="0.1.10",
+    version="0.1.9",
     description="Simple client for AutoCortext API",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Mark Watson",
     author_email="markus.c.watson@gmail.com",
     url="https://autocortext.com",
     keywords=["autocortext"],
```

