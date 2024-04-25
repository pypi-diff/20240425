# Comparing `tmp/viessmann-gridbox-connector-1.0.1.tar.gz` & `tmp/viessmann_gridbox_connector-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viessmann-gridbox-connector-1.0.1.tar", last modified: Tue Mar 26 11:50:53 2024, max compression
+gzip compressed data, was "viessmann_gridbox_connector-1.2.0.tar", last modified: Thu Apr 25 11:07:16 2024, max compression
```

## Comparing `viessmann-gridbox-connector-1.0.1.tar` & `viessmann_gridbox_connector-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:50:53.279429 viessmann-gridbox-connector-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-03-26 11:50:47.000000 viessmann-gridbox-connector-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-03-26 11:50:53.279429 viessmann-gridbox-connector-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-03-26 11:50:47.000000 viessmann-gridbox-connector-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:50:53.275429 viessmann-gridbox-connector-1.0.1/gridbox_connector/
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-03-26 11:50:47.000000 viessmann-gridbox-connector-1.0.1/gridbox_connector/GridboxConnector.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-26 11:50:47.000000 viessmann-gridbox-connector-1.0.1/gridbox_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-26 11:50:47.000000 viessmann-gridbox-connector-1.0.1/gridbox_connector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 11:50:53.279429 viessmann-gridbox-connector-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-26 11:50:47.000000 viessmann-gridbox-connector-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:50:53.279429 viessmann-gridbox-connector-1.0.1/viessmann_gridbox_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-03-26 11:50:53.000000 viessmann-gridbox-connector-1.0.1/viessmann_gridbox_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-26 11:50:53.000000 viessmann-gridbox-connector-1.0.1/viessmann_gridbox_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 11:50:53.000000 viessmann-gridbox-connector-1.0.1/viessmann_gridbox_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-26 11:50:53.000000 viessmann-gridbox-connector-1.0.1/viessmann_gridbox_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-26 11:50:53.000000 viessmann-gridbox-connector-1.0.1/viessmann_gridbox_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:07:16.839453 viessmann_gridbox_connector-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-25 11:07:12.000000 viessmann_gridbox_connector-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-25 11:07:16.839453 viessmann_gridbox_connector-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-25 11:07:12.000000 viessmann_gridbox_connector-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:07:16.839453 viessmann_gridbox_connector-1.2.0/gridbox_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-25 11:07:12.000000 viessmann_gridbox_connector-1.2.0/gridbox_connector/GridboxConnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-25 11:07:12.000000 viessmann_gridbox_connector-1.2.0/gridbox_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-25 11:07:12.000000 viessmann_gridbox_connector-1.2.0/gridbox_connector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 11:07:16.839453 viessmann_gridbox_connector-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-25 11:07:12.000000 viessmann_gridbox_connector-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:07:16.839453 viessmann_gridbox_connector-1.2.0/viessmann_gridbox_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-25 11:07:16.000000 viessmann_gridbox_connector-1.2.0/viessmann_gridbox_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-25 11:07:16.000000 viessmann_gridbox_connector-1.2.0/viessmann_gridbox_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 11:07:16.000000 viessmann_gridbox_connector-1.2.0/viessmann_gridbox_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 11:07:16.000000 viessmann_gridbox_connector-1.2.0/viessmann_gridbox_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 11:07:16.000000 viessmann_gridbox_connector-1.2.0/viessmann_gridbox_connector.egg-info/top_level.txt
```

### Comparing `viessmann-gridbox-connector-1.0.1/LICENSE` & `viessmann_gridbox_connector-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `viessmann-gridbox-connector-1.0.1/PKG-INFO` & `viessmann_gridbox_connector-1.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,7 @@
-Metadata-Version: 2.1
-Name: viessmann-gridbox-connector
-Version: 1.0.1
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-
 # Viessmann Gridbox Connector
 **This is not an official Viessmann library**
 
 a GridboxConnector Lib to fetch your Data from the Cloud.
 It is using the same Rest-API like the Dashboard and the App.
 
 ## Installation
@@ -51,20 +44,28 @@
 
 # Usage
 ```python
 from gridbox_connector import GridboxConnector
 
 # Initialize the connector with your configuration
 config = {
-    "urls": {
-        "login": "https://example.com/login",
-        "gateways": "https://example.com/gateways",
-        "live": "https://example.com/live/{}",
-    },
-    "login": {"username": "your_username", "password": "your_password"},
+  "urls": {
+    "login":"https://gridx.eu.auth0.com/oauth/token",
+    "gateways":"https://api.gridx.de/gateways",
+    "live":"https://api.gridx.de/systems/{}/live"
+  },
+  "login":{
+    "grant_type":"http://auth0.com/oauth/grant-type/password-realm",
+    "username":"email",
+    "password":"password",
+    "audience":"my.gridx",
+    "client_id":"oZpr934Ikn8OZOHTJEcrgXkjio0I0Q7b",
+    "scope":"email openid",
+    "realm":"viessmann-authentication-db"
+  }
 }
 
 connector = GridboxConnector(config)
 
 # Retrieve live data
 live_data = connector.retrieve_live_data()
 print(live_data)
```

### Comparing `viessmann-gridbox-connector-1.0.1/README.md` & `viessmann_gridbox_connector-1.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+Metadata-Version: 2.1
+Name: viessmann-gridbox-connector
+Version: 1.2.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+
 # Viessmann Gridbox Connector
 **This is not an official Viessmann library**
 
 a GridboxConnector Lib to fetch your Data from the Cloud.
 It is using the same Rest-API like the Dashboard and the App.
 
 ## Installation
@@ -44,20 +51,28 @@
 
 # Usage
 ```python
 from gridbox_connector import GridboxConnector
 
 # Initialize the connector with your configuration
 config = {
-    "urls": {
-        "login": "https://example.com/login",
-        "gateways": "https://example.com/gateways",
-        "live": "https://example.com/live/{}",
-    },
-    "login": {"username": "your_username", "password": "your_password"},
+  "urls": {
+    "login":"https://gridx.eu.auth0.com/oauth/token",
+    "gateways":"https://api.gridx.de/gateways",
+    "live":"https://api.gridx.de/systems/{}/live"
+  },
+  "login":{
+    "grant_type":"http://auth0.com/oauth/grant-type/password-realm",
+    "username":"email",
+    "password":"password",
+    "audience":"my.gridx",
+    "client_id":"oZpr934Ikn8OZOHTJEcrgXkjio0I0Q7b",
+    "scope":"email openid",
+    "realm":"viessmann-authentication-db"
+  }
 }
 
 connector = GridboxConnector(config)
 
 # Retrieve live data
 live_data = connector.retrieve_live_data()
 print(live_data)
```

### Comparing `viessmann-gridbox-connector-1.0.1/gridbox_connector/GridboxConnector.py` & `viessmann_gridbox_connector-1.2.0/gridbox_connector/GridboxConnector.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import requests
 import time
 class GridboxConnector:
     id_token = ""
+    gateways = []
 
     def __init__(self,config):
         self.login_url = config["urls"]["login"]
         self.login_body = config["login"]
         self.gateway_url = config["urls"]["gateways"]
         self.live_url = config["urls"]["live"]
         self.init_auth()
@@ -27,24 +28,29 @@
             time.wait(60)
             self.get_token()
        
     def generate_header(self):
         self.headers = {"Authorization": "Bearer {}".format(self.id_token)}
 
     def get_gateway_id(self):
+        self.gateways.clear()
         response = requests.get(self.gateway_url,headers=self.headers)
         response_json = response.json()
-        gateway = response_json[0]
-        self.gateway_id = gateway["system"]["id"]
+        for gateway in response_json:
+            self.gateways.append(gateway["system"]["id"])
+        
 
     def retrieve_live_data(self):
-        response = requests.get(self.live_url.format(self.gateway_id),headers=self.headers)
-        if response.status_code == 200:
-            response_json = response.json()
-            #print(response_json)
-            return response_json
-        else:
-            print("Status Code {}".format(response.status_code))
-            print("Response {}".format(response.json()))
-            time.sleep(60)
-            self.init_auth()
-            return self.retrieve_live_data()
+        responses = []
+        for id in self.gateways:
+            response = requests.get(self.live_url.format(self.id), headers=self.headers)
+            if response.status_code == 200:
+                response_json = response.json()
+                responses.append(response_json)
+                #print(response_json)
+            else:
+                print("Status Code {}".format(response.status_code))
+                print("Response {}".format(response.json()))
+                time.sleep(60)
+                self.init_auth()
+                return self.retrieve_live_data()
+        return responses
```

### Comparing `viessmann-gridbox-connector-1.0.1/viessmann_gridbox_connector.egg-info/PKG-INFO` & `viessmann_gridbox_connector-1.2.0/viessmann_gridbox_connector.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viessmann-gridbox-connector
-Version: 1.0.1
+Version: 1.2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 
 # Viessmann Gridbox Connector
 **This is not an official Viessmann library**
 
@@ -51,20 +51,28 @@
 
 # Usage
 ```python
 from gridbox_connector import GridboxConnector
 
 # Initialize the connector with your configuration
 config = {
-    "urls": {
-        "login": "https://example.com/login",
-        "gateways": "https://example.com/gateways",
-        "live": "https://example.com/live/{}",
-    },
-    "login": {"username": "your_username", "password": "your_password"},
+  "urls": {
+    "login":"https://gridx.eu.auth0.com/oauth/token",
+    "gateways":"https://api.gridx.de/gateways",
+    "live":"https://api.gridx.de/systems/{}/live"
+  },
+  "login":{
+    "grant_type":"http://auth0.com/oauth/grant-type/password-realm",
+    "username":"email",
+    "password":"password",
+    "audience":"my.gridx",
+    "client_id":"oZpr934Ikn8OZOHTJEcrgXkjio0I0Q7b",
+    "scope":"email openid",
+    "realm":"viessmann-authentication-db"
+  }
 }
 
 connector = GridboxConnector(config)
 
 # Retrieve live data
 live_data = connector.retrieve_live_data()
 print(live_data)
```

