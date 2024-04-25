# Comparing `tmp/gasconsumption-0.0.4.tar.gz` & `tmp/gasconsumption-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gasconsumption-0.0.4.tar", last modified: Wed Apr 24 19:02:55 2024, max compression
+gzip compressed data, was "gasconsumption-0.0.6.tar", last modified: Thu Apr 25 12:14:12 2024, max compression
```

## Comparing `gasconsumption-0.0.4.tar` & `gasconsumption-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 19:02:55.975647 gasconsumption-0.0.4/
--rw-rw-rw-   0        0        0      611 2024-04-24 19:02:55.975647 gasconsumption-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-24 19:02:55.972619 gasconsumption-0.0.4/gasconsumption.egg-info/
--rw-rw-rw-   0        0        0      611 2024-04-24 19:02:55.000000 gasconsumption-0.0.4/gasconsumption.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2024-04-24 19:02:55.000000 gasconsumption-0.0.4/gasconsumption.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 19:02:55.000000 gasconsumption-0.0.4/gasconsumption.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-24 19:02:55.000000 gasconsumption-0.0.4/gasconsumption.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-24 19:02:55.000000 gasconsumption-0.0.4/gasconsumption.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-24 19:02:55.974618 gasconsumption-0.0.4/libname/
--rw-rw-rw-   0        0        0       37 2024-04-24 18:49:33.000000 gasconsumption-0.0.4/libname/__init__.py
--rw-rw-rw-   0        0        0      752 2024-04-24 15:49:40.000000 gasconsumption-0.0.4/libname/apiexample.py
--rw-rw-rw-   0        0        0     7876 2024-04-24 18:33:05.000000 gasconsumption-0.0.4/libname/fastapiwrapper.py
--rw-rw-rw-   0        0        0       42 2024-04-24 19:02:55.975647 gasconsumption-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      937 2024-04-24 19:02:50.000000 gasconsumption-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:14:12.324068 gasconsumption-0.0.6/
+-rw-rw-rw-   0        0        0      611 2024-04-25 12:14:12.323068 gasconsumption-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-25 12:14:12.322068 gasconsumption-0.0.6/gasconsumption.egg-info/
+-rw-rw-rw-   0        0        0      611 2024-04-25 12:14:12.000000 gasconsumption-0.0.6/gasconsumption.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2024-04-25 12:14:12.000000 gasconsumption-0.0.6/gasconsumption.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 12:14:12.000000 gasconsumption-0.0.6/gasconsumption.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-25 12:14:12.000000 gasconsumption-0.0.6/gasconsumption.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-25 12:14:12.000000 gasconsumption-0.0.6/gasconsumption.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 12:14:12.323068 gasconsumption-0.0.6/libname/
+-rw-rw-rw-   0        0        0       37 2024-04-24 18:49:33.000000 gasconsumption-0.0.6/libname/__init__.py
+-rw-rw-rw-   0        0        0     8217 2024-04-25 12:05:44.000000 gasconsumption-0.0.6/libname/fastapiwrapper.py
+-rw-rw-rw-   0        0        0       42 2024-04-25 12:14:12.324068 gasconsumption-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      937 2024-04-25 12:11:59.000000 gasconsumption-0.0.6/setup.py
```

### Comparing `gasconsumption-0.0.4/PKG-INFO` & `gasconsumption-0.0.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gasconsumption
-Version: 0.0.4
+Version: 0.0.6
 Summary: fitching Deftable and timeseries table
 Author: Ahmad Riad
 Author-email: meuralengine@outlook.com
 Keywords: python,Deftable,timeseries table
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `gasconsumption-0.0.4/gasconsumption.egg-info/PKG-INFO` & `gasconsumption-0.0.6/gasconsumption.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gasconsumption
-Version: 0.0.4
+Version: 0.0.6
 Summary: fitching Deftable and timeseries table
 Author: Ahmad Riad
 Author-email: meuralengine@outlook.com
 Keywords: python,Deftable,timeseries table
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `gasconsumption-0.0.4/libname/fastapiwrapper.py` & `gasconsumption-0.0.6/libname/fastapiwrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import requests
 import pandas as pd 
 from datetime import datetime
 import logging 
+from functools import lru_cache
 
 logging.basicConfig(level=logging.WARNING)
 
 
 
 class Analysis:
     def __init__(self, username, password):
@@ -29,14 +30,16 @@
         if response.status_code == 202:
             data = response.json()
             
             return data['access_token']
         else:
             raise ValueError(f"Authentication failed: {data['detail']}", response.status_code)
 
+
+    @lru_cache(maxsize=None)
     def DefTable(self,curveid = None):
         if curveid is None:
             url_1 = self.url+'get/DefTable'
             headers_1 = {
                 'accept': 'application/json',
                 'Authorization': f"Bearer {self.token}"
             }
@@ -66,15 +69,15 @@
                 return df
             
             else:
                 raise ValueError(f"Failed to get table: {data_1['detail']}", response_1.status_code)
     
             
     
-            
+    @lru_cache(maxsize=None)
     def TimeSeries(self, curveid = None, startdate = None, enddate = None):
         if curveid is None:
             if startdate is not None and enddate is not None:
                 
                 url_1= self.url+f'get/TimeSeries?startdate={startdate}&enddate={enddate}'
                 headers_1 = {
                     'accept': 'application/json',
@@ -138,15 +141,15 @@
                     df = pd.DataFrame(data_1)
                     return df
                 else:
                     raise ValueError(f"Failed to get table: {data_1['detail']}", response_1.status_code)
                     
                     
             elif startdate is not None and enddate == None:
-                url_1= self.url+ 'get/cur={curveid}&TimeSeries?startdate={startdate}'
+                url_1= self.url+ f'get/TimeSeries?cur={curveid}&startdate={startdate}'
                 headers_1 = {
                     'accept': 'application/json',
                     'Authorization': f"Bearer {self.token}"
                 }
                         
                 response_1 = requests.get(url_1, headers=headers_1)
                 if response_1.status_code == 200:
@@ -184,22 +187,32 @@
         #     sliced_by_date_range = table[(table['ValueDate'] >= startdate)]
         #     return sliced_by_date_range
         
         # else:
         #     return table
   
     
-#%%%%%%%%%%%      
-curveid=2
-analysis = Analysis('ahmadriad2@gmail.com', '12345678')
-
-
-table = analysis.DefTable()
-table_1= analysis.TimeSeries()
-
+#%%%%%%%%%%%   
+# from datetime import datetime
+   
+# curveid=2
+# analysis = Analysis('ahmadriad3@gmail.com', '12345678')
+
+# start = datetime.now()
+# table = analysis.DefTable()
+# end = datetime.now()
+# timing = end - start
+# print(timing)
+      
+      
+# start = datetime.now()
+# table_1= analysis.TimeSeries(startdate="2024-04-25")
+# end = datetime.now()
+# timing = end - start
+# print(timing)
 #%%%%%%%%%%%
```

### Comparing `gasconsumption-0.0.4/setup.py` & `gasconsumption-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.4'
+VERSION = '0.0.6'
 DESCRIPTION = 'fitching Deftable and timeseries table'
 LONG_DESCRIPTION = 'contain an api wrapper that helps to fetch gas cconsumption data.'
 
 # Setting up
 setup(
     name="gasconsumption",
     version=VERSION,
```

