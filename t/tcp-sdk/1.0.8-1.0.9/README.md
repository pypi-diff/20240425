# Comparing `tmp/tcp-sdk-1.0.8.tar.gz` & `tmp/tcp-sdk-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcp-sdk-1.0.8.tar", last modified: Wed Nov  8 09:54:47 2023, max compression
+gzip compressed data, was "tcp-sdk-1.0.9.tar", last modified: Tue Nov 14 10:14:03 2023, max compression
```

## Comparing `tcp-sdk-1.0.8.tar` & `tcp-sdk-1.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 chabardt  (1000) users      (100)        0 2023-11-08 09:54:47.097457 tcp-sdk-1.0.8/
--rw-r--r--   0 chabardt  (1000) users      (100)      252 2023-10-16 08:08:40.000000 tcp-sdk-1.0.8/LICENSE.txt
--rw-r--r--   0 chabardt  (1000) users      (100)       81 2023-07-31 13:30:06.000000 tcp-sdk-1.0.8/MANIFEST.in
--rw-r--r--   0 chabardt  (1000) users      (100)     1110 2023-11-08 09:54:47.097457 tcp-sdk-1.0.8/PKG-INFO
--rw-r--r--   0 chabardt  (1000) users      (100)      920 2023-07-31 13:30:06.000000 tcp-sdk-1.0.8/README.rst
-drwxr-xr-x   0 chabardt  (1000) users      (100)        0 2023-11-08 09:54:47.096457 tcp-sdk-1.0.8/notebook/
--rwxr-xr-x   0 chabardt  (1000) users      (100)    19305 2023-08-14 07:58:05.000000 tcp-sdk-1.0.8/notebook/TCP_Training.ipynb
--rw-r--r--   0 chabardt  (1000) users      (100)      314 2023-08-09 08:28:13.000000 tcp-sdk-1.0.8/pyproject.toml
--rw-r--r--   0 chabardt  (1000) users      (100)       38 2023-11-08 09:54:47.097457 tcp-sdk-1.0.8/setup.cfg
--rw-r--r--   0 chabardt  (1000) users      (100)     1519 2023-10-30 15:11:16.000000 tcp-sdk-1.0.8/setup.py
-drwxr-xr-x   0 chabardt  (1000) users      (100)        0 2023-11-08 09:54:47.096457 tcp-sdk-1.0.8/tcp/
--rw-r--r--   0 chabardt  (1000) users      (100)       27 2023-07-31 13:30:06.000000 tcp-sdk-1.0.8/tcp/__init__.py
--rw-r--r--   0 chabardt  (1000) users      (100)       94 2023-08-10 12:18:34.000000 tcp-sdk-1.0.8/tcp/__main__.py
--rw-r--r--   0 chabardt  (1000) users      (100)       22 2023-11-08 09:54:30.000000 tcp-sdk-1.0.8/tcp/_version.py
--rw-r--r--   0 chabardt  (1000) users      (100)    15693 2023-11-08 09:38:15.000000 tcp-sdk-1.0.8/tcp/client.py
--rw-r--r--   0 chabardt  (1000) users      (100)     2758 2023-08-21 11:17:19.000000 tcp-sdk-1.0.8/tcp/clientAPI.py
--rw-r--r--   0 chabardt  (1000) users      (100)    12202 2023-09-15 09:10:47.000000 tcp-sdk-1.0.8/tcp/dashboard.py
--rw-r--r--   0 chabardt  (1000) users      (100)     1073 2023-07-31 13:30:06.000000 tcp-sdk-1.0.8/tcp/exceptions.py
--rw-r--r--   0 chabardt  (1000) users      (100)     2488 2023-08-11 13:49:35.000000 tcp-sdk-1.0.8/tcp/files.py
--rw-r--r--   0 chabardt  (1000) users      (100)     1036 2023-07-31 13:30:06.000000 tcp-sdk-1.0.8/tcp/logs.py
--rw-r--r--   0 chabardt  (1000) users      (100)      332 2023-08-21 11:16:27.000000 tcp-sdk-1.0.8/tcp/text_serializer.py
--rw-r--r--   0 chabardt  (1000) users      (100)      509 2023-10-31 16:26:09.000000 tcp-sdk-1.0.8/tcp/upload.py
-drwxr-xr-x   0 chabardt  (1000) users      (100)        0 2023-11-08 09:54:47.097457 tcp-sdk-1.0.8/tcp_sdk.egg-info/
--rw-r--r--   0 chabardt  (1000) users      (100)     1110 2023-11-08 09:54:47.000000 tcp-sdk-1.0.8/tcp_sdk.egg-info/PKG-INFO
--rw-r--r--   0 chabardt  (1000) users      (100)      543 2023-11-08 09:54:47.000000 tcp-sdk-1.0.8/tcp_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 chabardt  (1000) users      (100)        1 2023-11-08 09:54:47.000000 tcp-sdk-1.0.8/tcp_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 chabardt  (1000) users      (100)       52 2023-11-08 09:54:47.000000 tcp-sdk-1.0.8/tcp_sdk.egg-info/entry_points.txt
--rw-r--r--   0 chabardt  (1000) users      (100)       47 2023-11-08 09:54:47.000000 tcp-sdk-1.0.8/tcp_sdk.egg-info/requires.txt
--rw-r--r--   0 chabardt  (1000) users      (100)       10 2023-11-08 09:54:47.000000 tcp-sdk-1.0.8/tcp_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 chabardt  (1000) users      (100)        0 2023-11-08 09:54:47.097457 tcp-sdk-1.0.8/tests/
--rw-r--r--   0 chabardt  (1000) users      (100)      163 2023-07-31 13:30:06.000000 tcp-sdk-1.0.8/tests/__init__.py
--rw-r--r--   0 chabardt  (1000) users      (100)    21680 2023-10-23 12:21:58.000000 tcp-sdk-1.0.8/tests/test_app.py
--rw-r--r--   0 chabardt  (1000) users      (100)     4008 2023-08-07 08:16:11.000000 tcp-sdk-1.0.8/tests/test_auth.py
--rw-r--r--   0 chabardt  (1000) users      (100)     1902 2023-10-17 12:25:04.000000 tcp-sdk-1.0.8/tests/test_data.py
--rw-r--r--   0 chabardt  (1000) users      (100)     2649 2023-08-29 11:35:29.000000 tcp-sdk-1.0.8/tests/test_lics.py
+drwxr-xr-x   0 chabardt  (1000) users      (100)        0 2023-11-14 10:14:03.290326 tcp-sdk-1.0.9/
+-rw-r--r--   0 chabardt  (1000) users      (100)      252 2023-10-16 08:08:40.000000 tcp-sdk-1.0.9/LICENSE.txt
+-rw-r--r--   0 chabardt  (1000) users      (100)       81 2023-07-31 13:30:06.000000 tcp-sdk-1.0.9/MANIFEST.in
+-rw-r--r--   0 chabardt  (1000) users      (100)     1110 2023-11-14 10:14:03.290326 tcp-sdk-1.0.9/PKG-INFO
+-rw-r--r--   0 chabardt  (1000) users      (100)      920 2023-07-31 13:30:06.000000 tcp-sdk-1.0.9/README.rst
+drwxr-xr-x   0 chabardt  (1000) users      (100)        0 2023-11-14 10:14:03.287326 tcp-sdk-1.0.9/notebook/
+-rwxr-xr-x   0 chabardt  (1000) users      (100)    19305 2023-08-14 07:58:05.000000 tcp-sdk-1.0.9/notebook/TCP_Training.ipynb
+-rw-r--r--   0 chabardt  (1000) users      (100)      314 2023-08-09 08:28:13.000000 tcp-sdk-1.0.9/pyproject.toml
+-rw-r--r--   0 chabardt  (1000) users      (100)       38 2023-11-14 10:14:03.290326 tcp-sdk-1.0.9/setup.cfg
+-rw-r--r--   0 chabardt  (1000) users      (100)     1519 2023-10-30 15:11:16.000000 tcp-sdk-1.0.9/setup.py
+drwxr-xr-x   0 chabardt  (1000) users      (100)        0 2023-11-14 10:14:03.288326 tcp-sdk-1.0.9/tcp/
+-rw-r--r--   0 chabardt  (1000) users      (100)       27 2023-07-31 13:30:06.000000 tcp-sdk-1.0.9/tcp/__init__.py
+-rw-r--r--   0 chabardt  (1000) users      (100)       94 2023-08-10 12:18:34.000000 tcp-sdk-1.0.9/tcp/__main__.py
+-rw-r--r--   0 chabardt  (1000) users      (100)       22 2023-11-14 10:13:14.000000 tcp-sdk-1.0.9/tcp/_version.py
+-rw-r--r--   0 chabardt  (1000) users      (100)    15729 2023-11-14 10:12:42.000000 tcp-sdk-1.0.9/tcp/client.py
+-rw-r--r--   0 chabardt  (1000) users      (100)     2758 2023-08-21 11:17:19.000000 tcp-sdk-1.0.9/tcp/clientAPI.py
+-rw-r--r--   0 chabardt  (1000) users      (100)    12202 2023-09-15 09:10:47.000000 tcp-sdk-1.0.9/tcp/dashboard.py
+-rw-r--r--   0 chabardt  (1000) users      (100)     1073 2023-07-31 13:30:06.000000 tcp-sdk-1.0.9/tcp/exceptions.py
+-rw-r--r--   0 chabardt  (1000) users      (100)     2488 2023-08-11 13:49:35.000000 tcp-sdk-1.0.9/tcp/files.py
+-rw-r--r--   0 chabardt  (1000) users      (100)     1036 2023-07-31 13:30:06.000000 tcp-sdk-1.0.9/tcp/logs.py
+-rw-r--r--   0 chabardt  (1000) users      (100)      332 2023-08-21 11:16:27.000000 tcp-sdk-1.0.9/tcp/text_serializer.py
+-rw-r--r--   0 chabardt  (1000) users      (100)      509 2023-10-31 16:26:09.000000 tcp-sdk-1.0.9/tcp/upload.py
+drwxr-xr-x   0 chabardt  (1000) users      (100)        0 2023-11-14 10:14:03.289326 tcp-sdk-1.0.9/tcp_sdk.egg-info/
+-rw-r--r--   0 chabardt  (1000) users      (100)     1110 2023-11-14 10:14:03.000000 tcp-sdk-1.0.9/tcp_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 chabardt  (1000) users      (100)      543 2023-11-14 10:14:03.000000 tcp-sdk-1.0.9/tcp_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 chabardt  (1000) users      (100)        1 2023-11-14 10:14:03.000000 tcp-sdk-1.0.9/tcp_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 chabardt  (1000) users      (100)       52 2023-11-14 10:14:03.000000 tcp-sdk-1.0.9/tcp_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 chabardt  (1000) users      (100)       47 2023-11-14 10:14:03.000000 tcp-sdk-1.0.9/tcp_sdk.egg-info/requires.txt
+-rw-r--r--   0 chabardt  (1000) users      (100)       10 2023-11-14 10:14:03.000000 tcp-sdk-1.0.9/tcp_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 chabardt  (1000) users      (100)        0 2023-11-14 10:14:03.290326 tcp-sdk-1.0.9/tests/
+-rw-r--r--   0 chabardt  (1000) users      (100)      163 2023-07-31 13:30:06.000000 tcp-sdk-1.0.9/tests/__init__.py
+-rw-r--r--   0 chabardt  (1000) users      (100)    21680 2023-10-23 12:21:58.000000 tcp-sdk-1.0.9/tests/test_app.py
+-rw-r--r--   0 chabardt  (1000) users      (100)     4008 2023-08-07 08:16:11.000000 tcp-sdk-1.0.9/tests/test_auth.py
+-rw-r--r--   0 chabardt  (1000) users      (100)     1902 2023-10-17 12:25:04.000000 tcp-sdk-1.0.9/tests/test_data.py
+-rw-r--r--   0 chabardt  (1000) users      (100)     2649 2023-08-29 11:35:29.000000 tcp-sdk-1.0.9/tests/test_lics.py
```

### Comparing `tcp-sdk-1.0.8/PKG-INFO` & `tcp-sdk-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcp-sdk
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python SDK to query The Cross Product API.
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 TCP python SDK 
 ==============
```

### Comparing `tcp-sdk-1.0.8/README.rst` & `tcp-sdk-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `tcp-sdk-1.0.8/notebook/TCP_Training.ipynb` & `tcp-sdk-1.0.9/notebook/TCP_Training.ipynb`

 * *Files identical despite different names*

### Comparing `tcp-sdk-1.0.8/setup.py` & `tcp-sdk-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `tcp-sdk-1.0.8/tcp/client.py` & `tcp-sdk-1.0.9/tcp/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,18 +233,18 @@
         # Uploading directory
         if os.path.isdir (src_local):
             root_in_s3 = os.path.basename (src_local)
 
             for root, dirs, files in os.walk (src_local):
                 for file in files:
                     self.upload (os.path.join(root,file), 
-                                 os.path.join(
+                                 os.path.normpath(os.path.join(
                                      os.path.join(dest_s3,root_in_s3), 
                                      os.path.join(root[len(src_local):],file)
-                                     ),
+                                     )).replace('\\','/'),
                                  max_part_size
                                  )
             return
 
         print (f"Uploading {src_local} to {dest_s3} (max part size: {max_part_size})")
 
         #TODO adding multithread and retry process when error
```

### Comparing `tcp-sdk-1.0.8/tcp/clientAPI.py` & `tcp-sdk-1.0.9/tcp/clientAPI.py`

 * *Files identical despite different names*

### Comparing `tcp-sdk-1.0.8/tcp/dashboard.py` & `tcp-sdk-1.0.9/tcp/dashboard.py`

 * *Files identical despite different names*

### Comparing `tcp-sdk-1.0.8/tcp/exceptions.py` & `tcp-sdk-1.0.9/tcp/exceptions.py`

 * *Files identical despite different names*

### Comparing `tcp-sdk-1.0.8/tcp/files.py` & `tcp-sdk-1.0.9/tcp/files.py`

 * *Files identical despite different names*

### Comparing `tcp-sdk-1.0.8/tcp/logs.py` & `tcp-sdk-1.0.9/tcp/logs.py`

 * *Files identical despite different names*

### Comparing `tcp-sdk-1.0.8/tcp_sdk.egg-info/PKG-INFO` & `tcp-sdk-1.0.9/tcp_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcp-sdk
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python SDK to query The Cross Product API.
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 TCP python SDK 
 ==============
```

### Comparing `tcp-sdk-1.0.8/tcp_sdk.egg-info/SOURCES.txt` & `tcp-sdk-1.0.9/tcp_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tcp-sdk-1.0.8/tests/test_app.py` & `tcp-sdk-1.0.9/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `tcp-sdk-1.0.8/tests/test_auth.py` & `tcp-sdk-1.0.9/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `tcp-sdk-1.0.8/tests/test_data.py` & `tcp-sdk-1.0.9/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `tcp-sdk-1.0.8/tests/test_lics.py` & `tcp-sdk-1.0.9/tests/test_lics.py`

 * *Files identical despite different names*

