# Comparing `tmp/inferless-0.1.7.tar.gz` & `tmp/inferless-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inferless-0.1.7.tar", max compression
+gzip compressed data, was "inferless-0.1.8.tar", max compression
```

## Comparing `inferless-0.1.7.tar` & `inferless-0.1.8.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1822 2023-12-18 13:06:18.355865 inferless-0.1.7/README.md
--rw-r--r--   0        0        0      114 2023-12-18 13:05:03.561481 inferless-0.1.7/inferless/__init__.py
--rw-r--r--   0        0        0     1799 2023-12-18 13:05:03.556208 inferless-0.1.7/inferless/api.py
--rw-r--r--   0        0        0        0 2023-12-01 08:30:15.546459 inferless-0.1.7/inferless/utils/__init__.py
--rw-r--r--   0        0        0      264 2023-12-18 13:05:12.108588 inferless-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2316 1970-01-01 00:00:00.000000 inferless-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     2196 2024-04-25 13:52:25.406985 inferless-0.1.8/README.md
+-rw-r--r--   0        0        0      114 2023-12-18 13:10:49.190353 inferless-0.1.8/inferless/__init__.py
+-rw-r--r--   0        0        0     2489 2024-04-25 14:13:33.435568 inferless-0.1.8/inferless/api.py
+-rw-r--r--   0        0        0       59 2024-04-25 13:52:25.407586 inferless-0.1.8/inferless/utils/__init__.py
+-rw-r--r--   0        0        0     2124 2024-04-25 13:52:25.407890 inferless-0.1.8/inferless/utils/inputs.py
+-rw-r--r--   0        0        0      282 2024-04-25 13:52:25.408278 inferless-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2729 1970-01-01 00:00:00.000000 inferless-0.1.8/PKG-INFO
```

### Comparing `inferless-0.1.7/README.md` & `inferless-0.1.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,20 @@
 ## Usage
 This client can be used to call Inferless API from your python code. It supports both synchronous and asynchronous calls.
 ### Constants
 Fetch the URL and API_KEY from the Inferless console https://console-dev.inferless.com/
 ```python
 URL = "<url>"
 API_KEY = "<api_key>"
-data = { "inputs" : 
+```
+
+### Input Data
+Input data can be provided in two formats, as shown below as inputs and data.
+```python
+INPUTS = { "inputs" : 
           [
               {
                 "name": "prompt",
                 "shape": [
                   1
                 ],
                 "datatype": "BYTES",
@@ -24,22 +29,29 @@
                   "Once upon a time"
                 ]
               }
           ]
         }
 ```
 
+This other format is simpler and can be used if other parameters are not required. `datatype` and `shape` are automatically inferred.
+```python
+DATA = {
+    "prompt": "Once upon a time"
+}
+```
+
 ### Synchrounous call
 An example to call Inferless API synchronously
 ```python
 import inferless
 import datetime
 def main():
     t1 = datetime.datetime.now()
-    data = inferless.call(URL, API_KEY, data)
+    data = inferless.call(url=URL, workspace_api_key=API_KEY, inputs=INPUTS)
     t2 = datetime.datetime.now()
     print(f"time taken: {t2-t1}")
 
 main()
 ```
 Output
 ```console
@@ -57,16 +69,16 @@
     # e is the error object
     # response is the response object
     with open("response.json", "w") as f:
         f.write(json.dumps(response))
     
 
 t1 = datetime.now()
-inferless.call_async(URL, KEY, DATA, callback_func)
+inferless.call_async(url=URL, workspace_api_key=KEY, data=data, callback=callback_func)
 t2 = datetime.now()
 print(t2 - t1)
 ```
 Output
 ```console
 time taken: 0:00:00.000141
 ```
-It can be seen that the program exits without waiting for the response. The response is written to a file by the callback function after it is received.
+It can be seen that the program continues without waiting for the response. The response is written to a file by the callback function after it is received.
```

### Comparing `inferless-0.1.7/PKG-INFO` & `inferless-0.1.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: inferless
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Author: Inferless
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: numpy (>=1.21.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Python Client to call Inferless API
 
 ## Installation
 ```console
@@ -23,15 +24,20 @@
 ## Usage
 This client can be used to call Inferless API from your python code. It supports both synchronous and asynchronous calls.
 ### Constants
 Fetch the URL and API_KEY from the Inferless console https://console-dev.inferless.com/
 ```python
 URL = "<url>"
 API_KEY = "<api_key>"
-data = { "inputs" : 
+```
+
+### Input Data
+Input data can be provided in two formats, as shown below as inputs and data.
+```python
+INPUTS = { "inputs" : 
           [
               {
                 "name": "prompt",
                 "shape": [
                   1
                 ],
                 "datatype": "BYTES",
@@ -39,22 +45,29 @@
                   "Once upon a time"
                 ]
               }
           ]
         }
 ```
 
+This other format is simpler and can be used if other parameters are not required. `datatype` and `shape` are automatically inferred.
+```python
+DATA = {
+    "prompt": "Once upon a time"
+}
+```
+
 ### Synchrounous call
 An example to call Inferless API synchronously
 ```python
 import inferless
 import datetime
 def main():
     t1 = datetime.datetime.now()
-    data = inferless.call(URL, API_KEY, data)
+    data = inferless.call(url=URL, workspace_api_key=API_KEY, inputs=INPUTS)
     t2 = datetime.datetime.now()
     print(f"time taken: {t2-t1}")
 
 main()
 ```
 Output
 ```console
@@ -72,17 +85,17 @@
     # e is the error object
     # response is the response object
     with open("response.json", "w") as f:
         f.write(json.dumps(response))
     
 
 t1 = datetime.now()
-inferless.call_async(URL, KEY, DATA, callback_func)
+inferless.call_async(url=URL, workspace_api_key=KEY, data=data, callback=callback_func)
 t2 = datetime.now()
 print(t2 - t1)
 ```
 Output
 ```console
 time taken: 0:00:00.000141
 ```
-It can be seen that the program exits without waiting for the response. The response is written to a file by the callback function after it is received.
+It can be seen that the program continues without waiting for the response. The response is written to a file by the callback function after it is received.
```

