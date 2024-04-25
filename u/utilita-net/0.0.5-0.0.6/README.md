# Comparing `tmp/utilita-net-0.0.5.tar.gz` & `tmp/utilita-net-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utilita-net-0.0.5.tar", last modified: Mon Feb 26 17:53:31 2024, max compression
+gzip compressed data, was "utilita-net-0.0.6.tar", last modified: Thu Apr 25 20:00:51 2024, max compression
```

## Comparing `utilita-net-0.0.5.tar` & `utilita-net-0.0.6.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-02-26 17:53:31.585881 utilita-net-0.0.5/
--rw-rw-rw-   0        0        0       33 2023-11-17 17:58:22.000000 utilita-net-0.0.5/.gitattributes
--rw-rw-rw-   0        0        0     2074 2023-11-26 04:16:26.000000 utilita-net-0.0.5/.gitignore
--rw-rw-rw-   0        0        0     1100 2023-11-17 17:58:22.000000 utilita-net-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      158 2024-02-26 17:45:45.000000 utilita-net-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      507 2024-02-26 17:53:31.585881 utilita-net-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      337 2023-11-17 19:52:57.000000 utilita-net-0.0.5/README.md
--rwxrwxrwx   0        0        0       42 2024-02-26 17:53:27.000000 utilita-net-0.0.5/deploy.bat
--rw-rw-rw-   0        0        0       64 2023-11-17 17:58:22.000000 utilita-net-0.0.5/deploy.sh
--rwxrwxrwx   0        0        0      102 2023-11-26 02:19:34.000000 utilita-net-0.0.5/localdeploy.bat
--rw-rw-rw-   0        0        0        0 2023-11-17 17:58:22.000000 utilita-net-0.0.5/requirements.tests.txt
--rw-rw-rw-   0        0        0      101 2023-11-17 17:58:22.000000 utilita-net-0.0.5/requirements.txt
--rw-rw-rw-   0        0        0       86 2024-02-26 17:53:31.587881 utilita-net-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1430 2024-02-26 17:53:28.000000 utilita-net-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-26 17:53:31.498528 utilita-net-0.0.5/utilita/
-drwxrwxrwx   0        0        0        0 2024-02-26 17:53:31.539883 utilita-net-0.0.5/utilita/net/
--rw-rw-rw-   0        0        0       54 2023-11-17 17:58:22.000000 utilita-net-0.0.5/utilita/net/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-26 17:53:31.544882 utilita-net-0.0.5/utilita/net/gcshelper/
--rw-rw-rw-   0        0        0       32 2023-11-26 01:59:00.000000 utilita-net-0.0.5/utilita/net/gcshelper/__init__.py
--rw-rw-rw-   0        0        0    14074 2023-11-26 02:19:01.000000 utilita-net-0.0.5/utilita/net/gcshelper/gcshelper.py
-drwxrwxrwx   0        0        0        0 2024-02-26 17:53:31.561882 utilita-net-0.0.5/utilita/net/microsofthelper/
--rw-rw-rw-   0        0        0       44 2023-11-17 17:58:22.000000 utilita-net-0.0.5/utilita/net/microsofthelper/__init__.py
--rw-rw-rw-   0        0        0    23328 2023-11-26 04:06:08.000000 utilita-net-0.0.5/utilita/net/microsofthelper/auth.py
--rw-rw-rw-   0        0        0      181 2023-11-17 17:58:22.000000 utilita-net-0.0.5/utilita/net/microsofthelper/constants.py
--rw-rw-rw-   0        0        0      788 2023-11-17 17:58:22.000000 utilita-net-0.0.5/utilita/net/microsofthelper/log.py
--rw-rw-rw-   0        0        0    21247 2024-02-26 17:33:43.000000 utilita-net-0.0.5/utilita/net/microsofthelper/sharepoint.py
-drwxrwxrwx   0        0        0        0 2024-02-26 17:53:31.567898 utilita-net-0.0.5/utilita/net/scripts/
--rw-rw-rw-   0        0        0     2019 2024-01-23 18:15:36.000000 utilita-net-0.0.5/utilita/net/scripts/init_microsofthelper.py
-drwxrwxrwx   0        0        0        0 2024-02-26 17:53:31.584881 utilita-net-0.0.5/utilita_net.egg-info/
--rw-rw-rw-   0        0        0      507 2024-02-26 17:53:31.000000 utilita-net-0.0.5/utilita_net.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      694 2024-02-26 17:53:31.000000 utilita-net-0.0.5/utilita_net.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-26 17:53:31.000000 utilita-net-0.0.5/utilita_net.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2024-02-26 17:53:31.000000 utilita-net-0.0.5/utilita_net.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       98 2024-02-26 17:53:31.000000 utilita-net-0.0.5/utilita_net.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-02-26 17:53:31.000000 utilita-net-0.0.5/utilita_net.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 20:00:51.781455 utilita-net-0.0.6/
+-rw-rw-rw-   0        0        0       33 2023-11-17 17:58:22.000000 utilita-net-0.0.6/.gitattributes
+-rw-rw-rw-   0        0        0     2074 2023-11-26 04:16:26.000000 utilita-net-0.0.6/.gitignore
+-rw-rw-rw-   0        0        0     1100 2023-11-17 17:58:22.000000 utilita-net-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      158 2024-02-26 17:59:23.000000 utilita-net-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      507 2024-04-25 20:00:51.781455 utilita-net-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2023-11-17 19:52:57.000000 utilita-net-0.0.6/README.md
+-rwxrwxrwx   0        0        0       42 2024-02-26 17:53:27.000000 utilita-net-0.0.6/deploy.bat
+-rw-rw-rw-   0        0        0       64 2023-11-17 17:58:22.000000 utilita-net-0.0.6/deploy.sh
+-rwxrwxrwx   0        0        0      102 2023-11-26 02:19:34.000000 utilita-net-0.0.6/localdeploy.bat
+-rw-rw-rw-   0        0        0        0 2023-11-17 17:58:22.000000 utilita-net-0.0.6/requirements.tests.txt
+-rw-rw-rw-   0        0        0      101 2023-11-17 17:58:22.000000 utilita-net-0.0.6/requirements.txt
+-rw-rw-rw-   0        0        0       86 2024-04-25 20:00:51.783457 utilita-net-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1430 2024-04-25 20:00:25.000000 utilita-net-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 20:00:51.716455 utilita-net-0.0.6/utilita/
+drwxrwxrwx   0        0        0        0 2024-04-25 20:00:51.744475 utilita-net-0.0.6/utilita/net/
+-rw-rw-rw-   0        0        0       54 2023-11-17 17:58:22.000000 utilita-net-0.0.6/utilita/net/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 20:00:51.747456 utilita-net-0.0.6/utilita/net/gcshelper/
+-rw-rw-rw-   0        0        0       32 2023-11-26 01:59:00.000000 utilita-net-0.0.6/utilita/net/gcshelper/__init__.py
+-rw-rw-rw-   0        0        0    14074 2023-11-26 02:19:01.000000 utilita-net-0.0.6/utilita/net/gcshelper/gcshelper.py
+drwxrwxrwx   0        0        0        0 2024-04-25 20:00:51.761457 utilita-net-0.0.6/utilita/net/microsofthelper/
+-rw-rw-rw-   0        0        0       44 2023-11-17 17:58:22.000000 utilita-net-0.0.6/utilita/net/microsofthelper/__init__.py
+-rw-rw-rw-   0        0        0    23328 2023-11-26 04:06:08.000000 utilita-net-0.0.6/utilita/net/microsofthelper/auth.py
+-rw-rw-rw-   0        0        0      181 2023-11-17 17:58:22.000000 utilita-net-0.0.6/utilita/net/microsofthelper/constants.py
+-rw-rw-rw-   0        0        0      788 2023-11-17 17:58:22.000000 utilita-net-0.0.6/utilita/net/microsofthelper/log.py
+-rw-rw-rw-   0        0        0    21486 2024-04-25 20:00:13.000000 utilita-net-0.0.6/utilita/net/microsofthelper/sharepoint.py
+drwxrwxrwx   0        0        0        0 2024-04-25 20:00:51.765455 utilita-net-0.0.6/utilita/net/scripts/
+-rw-rw-rw-   0        0        0     2019 2024-01-23 18:15:36.000000 utilita-net-0.0.6/utilita/net/scripts/init_microsofthelper.py
+drwxrwxrwx   0        0        0        0 2024-04-25 20:00:51.768455 utilita-net-0.0.6/utilita/net/sftphelper/
+-rw-rw-rw-   0        0        0        0 2024-04-05 20:23:11.000000 utilita-net-0.0.6/utilita/net/sftphelper/sftphelper.py
+drwxrwxrwx   0        0        0        0 2024-04-25 20:00:51.779458 utilita-net-0.0.6/utilita_net.egg-info/
+-rw-rw-rw-   0        0        0      507 2024-04-25 20:00:51.000000 utilita-net-0.0.6/utilita_net.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      731 2024-04-25 20:00:51.000000 utilita-net-0.0.6/utilita_net.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 20:00:51.000000 utilita-net-0.0.6/utilita_net.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2024-04-25 20:00:51.000000 utilita-net-0.0.6/utilita_net.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       98 2024-04-25 20:00:51.000000 utilita-net-0.0.6/utilita_net.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-25 20:00:51.000000 utilita-net-0.0.6/utilita_net.egg-info/top_level.txt
```

### Comparing `utilita-net-0.0.5/.gitignore` & `utilita-net-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `utilita-net-0.0.5/LICENSE` & `utilita-net-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `utilita-net-0.0.5/setup.py` & `utilita-net-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_namespace_packages
 setup(
   name = 'utilita-net', # How you named your package folder (MyLib)
-  version = '0.0.5', # Start with a small number and increase it with every change you make
+  version = '0.0.6', # Start with a small number and increase it with every change you make
   packages=find_namespace_packages(include=['utilita.*']),
   license= 'MIT', # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'utilita but with helpers for web services', # Give a short description about your library
   author = 'Tommy Rojo',
   author_email = 'tr.trojo@gmail.com',
   url = 'https://github.com/trtrojo', # Provide either the link to your github or to your website
   download_url = 'https://github.com/trtrojo',
```

### Comparing `utilita-net-0.0.5/utilita/net/gcshelper/gcshelper.py` & `utilita-net-0.0.6/utilita/net/gcshelper/gcshelper.py`

 * *Files identical despite different names*

### Comparing `utilita-net-0.0.5/utilita/net/microsofthelper/auth.py` & `utilita-net-0.0.6/utilita/net/microsofthelper/auth.py`

 * *Files identical despite different names*

### Comparing `utilita-net-0.0.5/utilita/net/microsofthelper/log.py` & `utilita-net-0.0.6/utilita/net/microsofthelper/log.py`

 * *Files identical despite different names*

### Comparing `utilita-net-0.0.5/utilita/net/microsofthelper/sharepoint.py` & `utilita-net-0.0.6/utilita/net/microsofthelper/sharepoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import requests
 import json
 import urllib
 import os
+import io
 
 def attribute_allowed_list(value: str, allowed_list: list, raise_exception=False, hint='') -> bool:
     """Checks if a value is in a list of accepted values. Will raise a ValueError exception when raise_exception is true."""
     if value in allowed_list:
         return True
     if raise_exception:
         raise ValueError(f'{hint}Expected {allowed_list} but got {value}')
@@ -161,15 +162,23 @@
             Raises:
                 APIException: In the event we get any response of >= 400
         """
         if_exists = validate_attribute_allowed_list(value=if_exists, allowed_list=['fail', 'warn', 'ignore'], hint='upload_from_bytes if_exists ')
         web_path = urllib.parse.quote(upload_path)
         # https://learn.microsoft.com/en-us/graph/api/driveitem-createuploadsession?view=graph-rest-1.0#upload-bytes-to-the-upload-session
         preferred_chunk_size = 26214400 # ~25mb # This is for the future when we support more than 64mb of data. Must be divsible by 320KiB
-        file_size = os.fstat(file_bytes.fileno()).st_size
+
+        if isinstance(file_bytes, bytes):
+            file_bytes = io.BytesIO(file_bytes)
+        
+        if isinstance(file_bytes, io.BytesIO):
+            file_size = file_bytes.getbuffer().nbytes
+        else:
+            file_size = os.fstat(file_bytes.fileno()).st_size
+
         max_single_request_size = 61865984 # Microsoft graph only allows 64mb per POST. We must chunk the file if we want to do more.
 
         initial_body = {
             "@microsoft.graph.conflictBehavior": "fail", # fail (default) | replace | rename THIS LINE DOES NOT WORK WITH UPLOAD SESSIONS
             "fileSize": file_size,
             "deferCommit": True # Do not make file available until its completed.
         }
```

### Comparing `utilita-net-0.0.5/utilita/net/scripts/init_microsofthelper.py` & `utilita-net-0.0.6/utilita/net/scripts/init_microsofthelper.py`

 * *Files identical despite different names*

### Comparing `utilita-net-0.0.5/utilita_net.egg-info/SOURCES.txt` & `utilita-net-0.0.6/utilita_net.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -15,13 +15,14 @@
 utilita/net/gcshelper/gcshelper.py
 utilita/net/microsofthelper/__init__.py
 utilita/net/microsofthelper/auth.py
 utilita/net/microsofthelper/constants.py
 utilita/net/microsofthelper/log.py
 utilita/net/microsofthelper/sharepoint.py
 utilita/net/scripts/init_microsofthelper.py
+utilita/net/sftphelper/sftphelper.py
 utilita_net.egg-info/PKG-INFO
 utilita_net.egg-info/SOURCES.txt
 utilita_net.egg-info/dependency_links.txt
 utilita_net.egg-info/entry_points.txt
 utilita_net.egg-info/requires.txt
 utilita_net.egg-info/top_level.txt
```

