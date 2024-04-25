# Comparing `tmp/spider-client-0.0.6.tar.gz` & `tmp/spider-client-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spider-client-0.0.6.tar", last modified: Tue Apr 23 13:58:15 2024, max compression
+gzip compressed data, was "spider-client-0.0.7.tar", last modified: Thu Apr 25 15:26:30 2024, max compression
```

## Comparing `spider-client-0.0.6.tar` & `spider-client-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jeffreymendez   (501) staff       (20)        0 2024-04-23 13:58:15.200502 spider-client-0.0.6/
--rw-r--r--   0 jeffreymendez   (501) staff       (20)       10 2024-04-18 16:30:24.000000 spider-client-0.0.6/LICENSE
--rw-r--r--   0 jeffreymendez   (501) staff       (20)     4417 2024-04-23 13:58:15.200374 spider-client-0.0.6/PKG-INFO
--rw-r--r--   0 jeffreymendez   (501) staff       (20)     3676 2024-04-23 13:53:54.000000 spider-client-0.0.6/README.md
--rw-r--r--   0 jeffreymendez   (501) staff       (20)       38 2024-04-23 13:58:15.200541 spider-client-0.0.6/setup.cfg
--rw-r--r--   0 jeffreymendez   (501) staff       (20)     1060 2024-04-23 13:57:59.000000 spider-client-0.0.6/setup.py
-drwxr-xr-x   0 jeffreymendez   (501) staff       (20)        0 2024-04-23 13:58:15.199579 spider-client-0.0.6/spider/
--rw-r--r--   0 jeffreymendez   (501) staff       (20)       26 2024-04-22 13:01:33.000000 spider-client-0.0.6/spider/__init__.py
--rw-r--r--   0 jeffreymendez   (501) staff       (20)     6487 2024-04-23 13:52:54.000000 spider-client-0.0.6/spider/spider.py
-drwxr-xr-x   0 jeffreymendez   (501) staff       (20)        0 2024-04-23 13:58:15.200189 spider-client-0.0.6/spider_client.egg-info/
--rw-r--r--   0 jeffreymendez   (501) staff       (20)     4417 2024-04-23 13:58:15.000000 spider-client-0.0.6/spider_client.egg-info/PKG-INFO
--rw-r--r--   0 jeffreymendez   (501) staff       (20)      246 2024-04-23 13:58:15.000000 spider-client-0.0.6/spider_client.egg-info/SOURCES.txt
--rw-r--r--   0 jeffreymendez   (501) staff       (20)        1 2024-04-23 13:58:15.000000 spider-client-0.0.6/spider_client.egg-info/dependency_links.txt
--rw-r--r--   0 jeffreymendez   (501) staff       (20)        9 2024-04-23 13:58:15.000000 spider-client-0.0.6/spider_client.egg-info/requires.txt
--rw-r--r--   0 jeffreymendez   (501) staff       (20)        7 2024-04-23 13:58:15.000000 spider-client-0.0.6/spider_client.egg-info/top_level.txt
+drwxr-xr-x   0 jeffreymendez   (501) staff       (20)        0 2024-04-25 15:26:30.482147 spider-client-0.0.7/
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)       10 2024-04-18 16:30:24.000000 spider-client-0.0.7/LICENSE
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)     4417 2024-04-25 15:26:30.482005 spider-client-0.0.7/PKG-INFO
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)     3676 2024-04-23 13:53:54.000000 spider-client-0.0.7/README.md
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)       38 2024-04-25 15:26:30.482187 spider-client-0.0.7/setup.cfg
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)     1060 2024-04-25 15:26:16.000000 spider-client-0.0.7/setup.py
+drwxr-xr-x   0 jeffreymendez   (501) staff       (20)        0 2024-04-25 15:26:30.481162 spider-client-0.0.7/spider/
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)       26 2024-04-22 13:01:33.000000 spider-client-0.0.7/spider/__init__.py
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)     6471 2024-04-25 15:26:01.000000 spider-client-0.0.7/spider/spider.py
+drwxr-xr-x   0 jeffreymendez   (501) staff       (20)        0 2024-04-25 15:26:30.481811 spider-client-0.0.7/spider_client.egg-info/
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)     4417 2024-04-25 15:26:30.000000 spider-client-0.0.7/spider_client.egg-info/PKG-INFO
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)      246 2024-04-25 15:26:30.000000 spider-client-0.0.7/spider_client.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)        1 2024-04-25 15:26:30.000000 spider-client-0.0.7/spider_client.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)        9 2024-04-25 15:26:30.000000 spider-client-0.0.7/spider_client.egg-info/requires.txt
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)        7 2024-04-25 15:26:30.000000 spider-client-0.0.7/spider_client.egg-info/top_level.txt
```

### Comparing `spider-client-0.0.6/PKG-INFO` & `spider-client-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spider-client
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python SDK for Spider Cloud API
 Home-page: https://github.com/spider-rs/spider-clients/tree/main/python
 Author: Spider
 Author-email: jeff@a11ywatch.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

### Comparing `spider-client-0.0.6/README.md` & `spider-client-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `spider-client-0.0.6/setup.py` & `spider-client-0.0.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def read_file(fname):
     return open(os.path.join(os.path.dirname(__file__), fname), encoding="utf-8").read()
 
 
 setup(
     name="spider-client",
-    version="0.0.6",
+    version="0.0.7",
     url="https://github.com/spider-rs/spider-clients/tree/main/python",
     author="Spider",
     author_email="jeff@a11ywatch.com",
     description="Python SDK for Spider Cloud API",
     packages=find_packages(),
     install_requires=[
         "requests",
```

### Comparing `spider-client-0.0.6/spider/spider.py` & `spider-client-0.0.7/spider/spider.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         :param endpoint: The API endpoint to which the POST request is sent.
         :param data: The data (dictionary) to be sent in the POST request.
         :param stream: Boolean indicating if the response should be streamed.
         :return: The JSON response or the raw response stream if stream is True.
         """
         headers = self._prepare_headers(content_type)
         response = self._post_request(
-            f"https://https://spider.cloud/v1/{endpoint}", data, headers, stream
+            f"https://spider.cloud/v1/{endpoint}", data, headers, stream
         )
         if stream:
             return response
         elif response.status_code == 200:
             return response.json()
         else:
             self._handle_error(response, f"post to {endpoint}")
@@ -39,15 +39,15 @@
         Send a GET request to the specified endpoint.
 
         :param endpoint: The API endpoint from which to retrieve data.
         :return: The JSON decoded response.
         """
         headers = self._prepare_headers(content_type)
         response = self._get_request(
-            f"https://https://spider.cloud/v1/{endpoint}", headers, stream
+            f"https://spider.cloud/v1/{endpoint}", headers, stream
         )
         if response.status_code == 200:
             return response.json()
         else:
             self._handle_error(response, f"get from {endpoint}")
 
     def scrape_url(
```

### Comparing `spider-client-0.0.6/spider_client.egg-info/PKG-INFO` & `spider-client-0.0.7/spider_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spider-client
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python SDK for Spider Cloud API
 Home-page: https://github.com/spider-rs/spider-clients/tree/main/python
 Author: Spider
 Author-email: jeff@a11ywatch.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

