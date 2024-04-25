# Comparing `tmp/hscloud-0.0.8.tar.gz` & `tmp/hscloud-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hscloud-0.0.8.tar", last modified: Tue Apr 23 09:26:03 2024, max compression
+gzip compressed data, was "hscloud-0.0.9.tar", last modified: Thu Apr 25 06:50:32 2024, max compression
```

## Comparing `hscloud-0.0.8.tar` & `hscloud-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 09:26:03.528226 hscloud-0.0.8/
--rw-rw-rw-   0        0        0        0 2023-12-18 08:14:13.000000 hscloud-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      437 2024-04-23 09:26:03.527225 hscloud-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-22 09:32:34.000000 hscloud-0.0.8/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-23 09:26:03.516227 hscloud-0.0.8/hscloud/
--rw-rw-rw-   0        0        0        0 2024-04-23 06:50:43.000000 hscloud-0.0.8/hscloud/__init__.py
--rw-rw-rw-   0        0        0     2911 2024-04-23 07:32:17.000000 hscloud-0.0.8/hscloud/helpers.py
--rw-rw-rw-   0        0        0     1082 2024-04-23 09:25:13.000000 hscloud-0.0.8/hscloud/hscloud.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:26:03.524226 hscloud-0.0.8/hscloud.egg-info/
--rw-rw-rw-   0        0        0      437 2024-04-23 09:26:03.000000 hscloud-0.0.8/hscloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2024-04-23 09:26:03.000000 hscloud-0.0.8/hscloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 09:26:03.000000 hscloud-0.0.8/hscloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-23 09:26:03.000000 hscloud-0.0.8/hscloud.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 09:26:03.528226 hscloud-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      657 2024-04-23 09:25:26.000000 hscloud-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 06:50:32.469322 hscloud-0.0.9/
+-rw-rw-rw-   0        0        0        0 2023-12-18 08:14:13.000000 hscloud-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      437 2024-04-25 06:50:32.467324 hscloud-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-22 09:32:34.000000 hscloud-0.0.9/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-25 06:50:32.457320 hscloud-0.0.9/hscloud/
+-rw-rw-rw-   0        0        0        0 2024-04-23 06:50:43.000000 hscloud-0.0.9/hscloud/__init__.py
+-rw-rw-rw-   0        0        0     2926 2024-04-25 06:08:05.000000 hscloud-0.0.9/hscloud/helpers.py
+-rw-rw-rw-   0        0        0     1062 2024-04-25 06:09:26.000000 hscloud-0.0.9/hscloud/hscloud.py
+drwxrwxrwx   0        0        0        0 2024-04-25 06:50:32.466320 hscloud-0.0.9/hscloud.egg-info/
+-rw-rw-rw-   0        0        0      437 2024-04-25 06:50:32.000000 hscloud-0.0.9/hscloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2024-04-25 06:50:32.000000 hscloud-0.0.9/hscloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 06:50:32.000000 hscloud-0.0.9/hscloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-25 06:50:32.000000 hscloud-0.0.9/hscloud.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 06:50:32.470322 hscloud-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      657 2024-04-25 06:46:19.000000 hscloud-0.0.9/setup.py
```

### Comparing `hscloud-0.0.8/hscloud/helpers.py` & `hscloud-0.0.9/hscloud/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import requests
 from datetime import datetime
 import logging
 from typing import NamedTuple, Optional, Union
 
 logger = logging.getLogger(__name__)
 
-URL = 'http://10.10.20.109:2070'
+ENDPOINT = 'http://10.10.20.109:2070'
 TIMEOUT = 8
 
 class Helpers:
 
     @staticmethod
     def headers(access_token=None):
         headers = None
@@ -74,23 +74,23 @@
     def call_api(api: str, method: str, headers: Optional[dict] = None, params: Optional[dict] = None, json_body: Optional[dict] = None) -> tuple:
         response = None
         response_code = False
         response_data = None
 
         try:
             if method.lower() == 'get':
-                response = requests.get(URL + api, headers=headers, params=params, timeout=TIMEOUT)
+                response = requests.get(ENDPOINT + api, headers=headers, params=params, timeout=TIMEOUT)
 
             elif method.lower() == 'post':
-                response = requests.post(URL + api, headers=headers, params=params, json=json_body, timeout=TIMEOUT)
+                response = requests.post(ENDPOINT + api, headers=headers, params=params, json=json_body, timeout=TIMEOUT)
 
         except requests.exceptions.RequestException as e:
-            logger.debug(e)
+            logger.error(e)
         except Exception as e:
-            logger.debug(e)
+            logger.error(e)
         else:
             if response.status_code == 200:
                 response_body = response.json()
                 if response_body.get("code") == 0:
                     response_code = True
                     response_data = response_body.get("data")
         return response_code, response_data
```

### Comparing `hscloud-0.0.8/hscloud/hscloud.py` & `hscloud-0.0.9/hscloud/hscloud.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,19 +6,19 @@
         super().__init__()
         self.username = username
         self.password = password
         self.access_token = None
 
     def login(self) -> tuple:
         response = Helpers.call_api("/api/oauth/login", "post", Helpers.headers(), Helpers.params(), Helpers.login_body(self.username, self.password))
-        self.access_token = response[1].get("access_token")
+        if response[0]:
+            self.access_token = response[1].get("access_token")
         return response
 
     def devices(self) -> tuple:
         return Helpers.call_api("/api/device/list", "get", Helpers.headers(self.access_token), Helpers.params())
 
-    def status(self, access_token, devicesn) -> tuple:
-        return Helpers.call_api("/api/device/state", "get", Helpers.headers(access_token), Helpers.params(devicesn))
+    def status(self, devicesn) -> tuple:
+        return Helpers.call_api("/api/device/state", "get", Helpers.headers(self.access_token), Helpers.params(devicesn))
 
-    def update(self, access_token, devicesn, **kwargs) -> bool:
-        response = Helpers.call_api("/api/device/control", "post", Helpers.headers(access_token), Helpers.params(), Helpers.update_body(devicesn, **kwargs))
-        return response[0]
+    def update(self, devicesn, **kwargs) -> tuple:
+        return Helpers.call_api("/api/device/control", "post", Helpers.headers(self.access_token), Helpers.params(), Helpers.update_body(devicesn, **kwargs))
```

### Comparing `hscloud-0.0.8/setup.py` & `hscloud-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.rst", "r") as f:
     long_description = f.read()
 
 setup(
     name="hscloud",
-    version="0.0.8",
+    version="0.0.9",
     author="kane",
     author_email="wang.xiangtao@qq.com",
     description="A small package to work with prime numbers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/clement-bonnet/medium-first-package",
     packages=find_packages(),
```

