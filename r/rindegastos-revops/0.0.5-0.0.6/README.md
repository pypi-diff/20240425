# Comparing `tmp/rindegastos_revops-0.0.5.tar.gz` & `tmp/rindegastos_revops-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rindegastos_revops-0.0.5.tar", last modified: Tue Apr 23 19:55:47 2024, max compression
+gzip compressed data, was "rindegastos_revops-0.0.6.tar", last modified: Thu Apr 25 16:47:03 2024, max compression
```

## Comparing `rindegastos_revops-0.0.5.tar` & `rindegastos_revops-0.0.6.tar`

### file list

```diff
@@ -1,37 +1,42 @@
-drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 19:55:47.125235 rindegastos_revops-0.0.5/
--rw-r--r--   0 joseizam   (501) staff       (20)      538 2024-04-23 19:55:47.125145 rindegastos_revops-0.0.5/PKG-INFO
--rw-r--r--   0 joseizam   (501) staff       (20)        0 2024-04-23 14:06:12.000000 rindegastos_revops-0.0.5/README.md
--rw-r--r--   0 joseizam   (501) staff       (20)       86 2024-04-23 14:09:38.000000 rindegastos_revops-0.0.5/pyproject.toml
--rw-r--r--   0 joseizam   (501) staff       (20)      678 2024-04-23 19:55:47.125567 rindegastos_revops-0.0.5/setup.cfg
-drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 19:55:47.119480 rindegastos_revops-0.0.5/src/
-drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 19:55:47.120670 rindegastos_revops-0.0.5/src/rindegastos_revops/
--rw-r--r--   0 joseizam   (501) staff       (20)       26 2024-04-23 19:33:10.000000 rindegastos_revops-0.0.5/src/rindegastos_revops/__init__.py
-drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 19:55:47.121810 rindegastos_revops-0.0.5/src/rindegastos_revops/data_engineering/
--rw-r--r--   0 joseizam   (501) staff       (20)        0 2024-04-23 19:00:35.000000 rindegastos_revops-0.0.5/src/rindegastos_revops/data_engineering/__init__.py
-drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 19:55:47.121988 rindegastos_revops-0.0.5/src/rindegastos_revops/hubspot_api/
--rw-r--r--   0 joseizam   (501) staff       (20)       71 2024-04-23 16:04:11.000000 rindegastos_revops-0.0.5/src/rindegastos_revops/hubspot_api/__init__.py
-drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 19:55:47.122907 rindegastos_revops-0.0.5/src/rindegastos_revops/hubspot_api/helpers/
--rw-r--r--   0 joseizam   (501) staff       (20)      104 2024-04-23 16:03:30.000000 rindegastos_revops-0.0.5/src/rindegastos_revops/hubspot_api/helpers/__init__.py
--rw-r--r--   0 joseizam   (501) staff       (20)      129 2024-04-23 16:54:01.000000 rindegastos_revops-0.0.5/src/rindegastos_revops/hubspot_api/helpers/dates.py
--rw-r--r--   0 joseizam   (501) staff       (20)      183 2024-04-23 15:11:06.000000 rindegastos_revops-0.0.5/src/rindegastos_revops/hubspot_api/helpers/file_name.py
--rw-r--r--   0 joseizam   (501) staff       (20)      852 2024-04-23 16:16:16.000000 rindegastos_revops-0.0.5/src/rindegastos_revops/hubspot_api/helpers/hubspot.py
--rw-r--r--   0 joseizam   (501) staff       (20)     2025 2024-04-23 15:11:06.000000 rindegastos_revops-0.0.5/src/rindegastos_revops/hubspot_api/helpers/properties_selection.py
-drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 19:55:47.123109 rindegastos_revops-0.0.5/src/rindegastos_revops/hubspot_api/objects/
--rw-r--r--   0 joseizam   (501) staff       (20)       48 2024-04-23 16:03:05.000000 rindegastos_revops-0.0.5/src/rindegastos_revops/hubspot_api/objects/__init__.py
-drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 19:55:47.123481 rindegastos_revops-0.0.5/src/rindegastos_revops/hubspot_api/objects/companies/
--rw-r--r--   0 joseizam   (501) staff       (20)       21 2024-04-23 16:01:55.000000 rindegastos_revops-0.0.5/src/rindegastos_revops/hubspot_api/objects/companies/__init__.py
--rw-r--r--   0 joseizam   (501) staff       (20)     2661 2024-04-23 19:50:00.000000 rindegastos_revops-0.0.5/src/rindegastos_revops/hubspot_api/objects/companies/search.py
-drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 19:55:47.124116 rindegastos_revops-0.0.5/src/rindegastos_revops/hubspot_api/objects/contacts/
--rw-r--r--   0 joseizam   (501) staff       (20)       21 2024-04-23 16:01:43.000000 rindegastos_revops-0.0.5/src/rindegastos_revops/hubspot_api/objects/contacts/__init__.py
--rw-r--r--   0 joseizam   (501) staff       (20)     3372 2024-04-23 19:50:11.000000 rindegastos_revops-0.0.5/src/rindegastos_revops/hubspot_api/objects/contacts/search.py
-drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 19:55:47.124448 rindegastos_revops-0.0.5/src/rindegastos_revops/hubspot_api/properties/
--rw-r--r--   0 joseizam   (501) staff       (20)       23 2024-04-23 16:02:25.000000 rindegastos_revops-0.0.5/src/rindegastos_revops/hubspot_api/properties/__init__.py
--rw-r--r--   0 joseizam   (501) staff       (20)      823 2024-04-23 19:50:20.000000 rindegastos_revops-0.0.5/src/rindegastos_revops/hubspot_api/properties/read_all.py
-drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 19:55:47.124909 rindegastos_revops-0.0.5/src/rindegastos_revops.egg-info/
--rw-r--r--   0 joseizam   (501) staff       (20)      538 2024-04-23 19:55:47.000000 rindegastos_revops-0.0.5/src/rindegastos_revops.egg-info/PKG-INFO
--rw-r--r--   0 joseizam   (501) staff       (20)     1141 2024-04-23 19:55:47.000000 rindegastos_revops-0.0.5/src/rindegastos_revops.egg-info/SOURCES.txt
--rw-r--r--   0 joseizam   (501) staff       (20)        1 2024-04-23 19:55:47.000000 rindegastos_revops-0.0.5/src/rindegastos_revops.egg-info/dependency_links.txt
--rw-r--r--   0 joseizam   (501) staff       (20)       16 2024-04-23 19:55:47.000000 rindegastos_revops-0.0.5/src/rindegastos_revops.egg-info/requires.txt
--rw-r--r--   0 joseizam   (501) staff       (20)       19 2024-04-23 19:55:47.000000 rindegastos_revops-0.0.5/src/rindegastos_revops.egg-info/top_level.txt
-drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 19:55:47.124651 rindegastos_revops-0.0.5/tests/
--rw-r--r--   0 joseizam   (501) staff       (20)     1007 2024-04-23 19:03:08.000000 rindegastos_revops-0.0.5/tests/test_hubspot_api_contacts.py
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-25 16:47:03.472015 rindegastos_revops-0.0.6/
+-rw-r--r--   0 joseizam   (501) staff       (20)      538 2024-04-25 16:47:03.471943 rindegastos_revops-0.0.6/PKG-INFO
+-rw-r--r--   0 joseizam   (501) staff       (20)        0 2024-04-23 14:06:12.000000 rindegastos_revops-0.0.6/README.md
+-rw-r--r--   0 joseizam   (501) staff       (20)       86 2024-04-23 14:09:38.000000 rindegastos_revops-0.0.6/pyproject.toml
+-rw-r--r--   0 joseizam   (501) staff       (20)      678 2024-04-25 16:47:03.472336 rindegastos_revops-0.0.6/setup.cfg
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-25 16:47:03.465432 rindegastos_revops-0.0.6/src/
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-25 16:47:03.466856 rindegastos_revops-0.0.6/src/rindegastos_revops/
+-rw-r--r--   0 joseizam   (501) staff       (20)       26 2024-04-23 20:44:59.000000 rindegastos_revops-0.0.6/src/rindegastos_revops/__init__.py
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-25 16:47:03.468188 rindegastos_revops-0.0.6/src/rindegastos_revops/data_engineering/
+-rw-r--r--   0 joseizam   (501) staff       (20)        0 2024-04-23 19:00:35.000000 rindegastos_revops-0.0.6/src/rindegastos_revops/data_engineering/__init__.py
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-25 16:47:03.468365 rindegastos_revops-0.0.6/src/rindegastos_revops/hubspot_api/
+-rw-r--r--   0 joseizam   (501) staff       (20)       47 2024-04-23 20:44:40.000000 rindegastos_revops-0.0.6/src/rindegastos_revops/hubspot_api/__init__.py
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-25 16:47:03.469512 rindegastos_revops-0.0.6/src/rindegastos_revops/hubspot_api/helpers/
+-rw-r--r--   0 joseizam   (501) staff       (20)      133 2024-04-24 14:22:46.000000 rindegastos_revops-0.0.6/src/rindegastos_revops/hubspot_api/helpers/__init__.py
+-rw-r--r--   0 joseizam   (501) staff       (20)      129 2024-04-23 16:54:01.000000 rindegastos_revops-0.0.6/src/rindegastos_revops/hubspot_api/helpers/dates.py
+-rw-r--r--   0 joseizam   (501) staff       (20)      183 2024-04-23 15:11:06.000000 rindegastos_revops-0.0.6/src/rindegastos_revops/hubspot_api/helpers/file_name.py
+-rw-r--r--   0 joseizam   (501) staff       (20)      273 2024-04-24 19:30:42.000000 rindegastos_revops-0.0.6/src/rindegastos_revops/hubspot_api/helpers/get_dataframe.py
+-rw-r--r--   0 joseizam   (501) staff       (20)      932 2024-04-25 15:39:09.000000 rindegastos_revops-0.0.6/src/rindegastos_revops/hubspot_api/helpers/hubspot.py
+-rw-r--r--   0 joseizam   (501) staff       (20)     2025 2024-04-23 15:11:06.000000 rindegastos_revops-0.0.6/src/rindegastos_revops/hubspot_api/helpers/properties_selection.py
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-25 16:47:03.469686 rindegastos_revops-0.0.6/src/rindegastos_revops/hubspot_api/objects/
+-rw-r--r--   0 joseizam   (501) staff       (20)       36 2024-04-23 20:45:30.000000 rindegastos_revops-0.0.6/src/rindegastos_revops/hubspot_api/objects/__init__.py
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-25 16:47:03.470039 rindegastos_revops-0.0.6/src/rindegastos_revops/hubspot_api/objects/companies/
+-rw-r--r--   0 joseizam   (501) staff       (20)       21 2024-04-23 20:43:33.000000 rindegastos_revops-0.0.6/src/rindegastos_revops/hubspot_api/objects/companies/__init__.py
+-rw-r--r--   0 joseizam   (501) staff       (20)     1885 2024-04-25 15:24:33.000000 rindegastos_revops-0.0.6/src/rindegastos_revops/hubspot_api/objects/companies/search.py
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-25 16:47:03.470415 rindegastos_revops-0.0.6/src/rindegastos_revops/hubspot_api/objects/contacts/
+-rw-r--r--   0 joseizam   (501) staff       (20)       21 2024-04-23 20:44:10.000000 rindegastos_revops-0.0.6/src/rindegastos_revops/hubspot_api/objects/contacts/__init__.py
+-rw-r--r--   0 joseizam   (501) staff       (20)     1873 2024-04-25 15:53:10.000000 rindegastos_revops-0.0.6/src/rindegastos_revops/hubspot_api/objects/contacts/search.py
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-25 16:47:03.470757 rindegastos_revops-0.0.6/src/rindegastos_revops/hubspot_api/objects/deals/
+-rw-r--r--   0 joseizam   (501) staff       (20)       20 2024-04-25 15:13:41.000000 rindegastos_revops-0.0.6/src/rindegastos_revops/hubspot_api/objects/deals/__init__.py
+-rw-r--r--   0 joseizam   (501) staff       (20)     1878 2024-04-25 15:25:06.000000 rindegastos_revops-0.0.6/src/rindegastos_revops/hubspot_api/objects/deals/search.py
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-25 16:47:03.471119 rindegastos_revops-0.0.6/src/rindegastos_revops/hubspot_api/objects/tickets/
+-rw-r--r--   0 joseizam   (501) staff       (20)       20 2024-04-25 15:38:33.000000 rindegastos_revops-0.0.6/src/rindegastos_revops/hubspot_api/objects/tickets/__init__.py
+-rw-r--r--   0 joseizam   (501) staff       (20)     1882 2024-04-25 15:39:23.000000 rindegastos_revops-0.0.6/src/rindegastos_revops/hubspot_api/objects/tickets/search.py
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-25 16:47:03.471451 rindegastos_revops-0.0.6/src/rindegastos_revops/hubspot_api/properties/
+-rw-r--r--   0 joseizam   (501) staff       (20)       23 2024-04-23 21:07:41.000000 rindegastos_revops-0.0.6/src/rindegastos_revops/hubspot_api/properties/__init__.py
+-rw-r--r--   0 joseizam   (501) staff       (20)      800 2024-04-24 19:57:32.000000 rindegastos_revops-0.0.6/src/rindegastos_revops/hubspot_api/properties/read_all.py
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-25 16:47:03.471678 rindegastos_revops-0.0.6/src/rindegastos_revops.egg-info/
+-rw-r--r--   0 joseizam   (501) staff       (20)      538 2024-04-25 16:47:03.000000 rindegastos_revops-0.0.6/src/rindegastos_revops.egg-info/PKG-INFO
+-rw-r--r--   0 joseizam   (501) staff       (20)     1410 2024-04-25 16:47:03.000000 rindegastos_revops-0.0.6/src/rindegastos_revops.egg-info/SOURCES.txt
+-rw-r--r--   0 joseizam   (501) staff       (20)        1 2024-04-25 16:47:03.000000 rindegastos_revops-0.0.6/src/rindegastos_revops.egg-info/dependency_links.txt
+-rw-r--r--   0 joseizam   (501) staff       (20)       16 2024-04-25 16:47:03.000000 rindegastos_revops-0.0.6/src/rindegastos_revops.egg-info/requires.txt
+-rw-r--r--   0 joseizam   (501) staff       (20)       19 2024-04-25 16:47:03.000000 rindegastos_revops-0.0.6/src/rindegastos_revops.egg-info/top_level.txt
```

### Comparing `rindegastos_revops-0.0.5/PKG-INFO` & `rindegastos_revops-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rindegastos_revops
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simple sdk for revops packages
 Home-page: https://github.com/joigmz/rindegastos_revops
 Author: Jose Izam
 Author-email: jose.izam99@gmail.com
 Project-URL: Bug Tracker, https://github.com/joigmz/rindegastos_revops
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rindegastos_revops-0.0.5/setup.cfg` & `rindegastos_revops-0.0.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rindegastos_revops
-version = 0.0.5
+version = 0.0.6
 author = Jose Izam
 author_email = jose.izam99@gmail.com
 description = Simple sdk for revops packages
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/joigmz/rindegastos_revops
 project_urls =
```

### Comparing `rindegastos_revops-0.0.5/src/rindegastos_revops/hubspot_api/helpers/hubspot.py` & `rindegastos_revops-0.0.6/src/rindegastos_revops/hubspot_api/helpers/hubspot.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from enum import Enum
 
 class Endpoints(Enum):
     # Contacts
-    CONTACTS = "objects/contacts"
     CONTACTS_SEARCH = "objects/contacts/search"
     # Companies
     COMPANIES_SEARCH = "objects/companies/search"
+    # Deals
+    DEALS_SEARCH = "objects/deals/search"
+    # Tickets
+    TICKETS_SEARCH = "objects/tickets/search"
     # Properties
     PROPERTIES_CONTACTS_READ_ALL = "properties/contacts"
     PROPERTIES_COMPANIES_READ_ALL = "properties/companies"
     PROPERTIES_DEALS_READ_ALL = "properties/deals"
     PROPERTIES_TICKETS_READ_ALL = "properties/tickets"
```

### Comparing `rindegastos_revops-0.0.5/src/rindegastos_revops/hubspot_api/helpers/properties_selection.py` & `rindegastos_revops-0.0.6/src/rindegastos_revops/hubspot_api/helpers/properties_selection.py`

 * *Files identical despite different names*

### Comparing `rindegastos_revops-0.0.5/src/rindegastos_revops/hubspot_api/properties/read_all.py` & `rindegastos_revops-0.0.6/src/rindegastos_revops/hubspot_api/properties/read_all.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-from src.rindegastos_revops.hubspot_api.helpers.hubspot import HubspotConnectorApi, Endpoints
+from ...hubspot_api.helpers.hubspot import HubspotConnectorApi, Endpoints
 
-import requests
 import pandas as pd
-
-
+import requests
 
 def read_all_properties(client:HubspotConnectorApi, endpoint:Endpoints) -> dict:
 
     response = requests.request("GET", client.endpoint(endpoint), headers=client.headers)
 
     context = {
         "status_done" : False,
@@ -22,8 +20,8 @@
             context["df"] = df
             context["status_done"] = True
 
     else:
         print("status_code: ", response.status_code)
         print("response:", response.text)
     
-    return context
+    return context
```

### Comparing `rindegastos_revops-0.0.5/src/rindegastos_revops.egg-info/PKG-INFO` & `rindegastos_revops-0.0.6/src/rindegastos_revops.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rindegastos_revops
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simple sdk for revops packages
 Home-page: https://github.com/joigmz/rindegastos_revops
 Author: Jose Izam
 Author-email: jose.izam99@gmail.com
 Project-URL: Bug Tracker, https://github.com/joigmz/rindegastos_revops
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rindegastos_revops-0.0.5/src/rindegastos_revops.egg-info/SOURCES.txt` & `rindegastos_revops-0.0.6/src/rindegastos_revops.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -8,17 +8,21 @@
 src/rindegastos_revops.egg-info/requires.txt
 src/rindegastos_revops.egg-info/top_level.txt
 src/rindegastos_revops/data_engineering/__init__.py
 src/rindegastos_revops/hubspot_api/__init__.py
 src/rindegastos_revops/hubspot_api/helpers/__init__.py
 src/rindegastos_revops/hubspot_api/helpers/dates.py
 src/rindegastos_revops/hubspot_api/helpers/file_name.py
+src/rindegastos_revops/hubspot_api/helpers/get_dataframe.py
 src/rindegastos_revops/hubspot_api/helpers/hubspot.py
 src/rindegastos_revops/hubspot_api/helpers/properties_selection.py
 src/rindegastos_revops/hubspot_api/objects/__init__.py
 src/rindegastos_revops/hubspot_api/objects/companies/__init__.py
 src/rindegastos_revops/hubspot_api/objects/companies/search.py
 src/rindegastos_revops/hubspot_api/objects/contacts/__init__.py
 src/rindegastos_revops/hubspot_api/objects/contacts/search.py
+src/rindegastos_revops/hubspot_api/objects/deals/__init__.py
+src/rindegastos_revops/hubspot_api/objects/deals/search.py
+src/rindegastos_revops/hubspot_api/objects/tickets/__init__.py
+src/rindegastos_revops/hubspot_api/objects/tickets/search.py
 src/rindegastos_revops/hubspot_api/properties/__init__.py
-src/rindegastos_revops/hubspot_api/properties/read_all.py
-tests/test_hubspot_api_contacts.py
+src/rindegastos_revops/hubspot_api/properties/read_all.py
```

