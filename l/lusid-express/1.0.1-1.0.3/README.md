# Comparing `tmp/lusid_express-1.0.1.tar.gz` & `tmp/lusid_express-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_express-1.0.1.tar", last modified: Wed Apr 24 16:28:17 2024, max compression
+gzip compressed data, was "lusid_express-1.0.3.tar", last modified: Thu Apr 25 19:05:43 2024, max compression
```

## Comparing `lusid_express-1.0.1.tar` & `lusid_express-1.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 16:28:17.410393 lusid_express-1.0.1/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-04-24 16:27:33.000000 lusid_express-1.0.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-04-24 16:27:33.000000 lusid_express-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6659 2024-04-24 16:28:17.410393 lusid_express-1.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6019 2024-04-24 16:27:33.000000 lusid_express-1.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 16:28:17.410393 lusid_express-1.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1536 2024-04-24 16:27:33.000000 lusid_express-1.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 16:28:17.404394 lusid_express-1.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 16:28:17.406393 lusid_express-1.0.1/src/lusid_express/
--rw-rw-rw-   0 root         (0) root         (0)       30 2024-04-24 16:27:33.000000 lusid_express-1.0.1/src/lusid_express/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5616 2024-04-24 16:27:33.000000 lusid_express-1.0.1/src/lusid_express/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 16:28:17.407394 lusid_express-1.0.1/src/lusid_express/apis/
--rw-rw-rw-   0 root         (0) root         (0)  2240138 2024-04-24 16:28:16.000000 lusid_express-1.0.1/src/lusid_express/apis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 16:28:17.409393 lusid_express-1.0.1/src/lusid_express/config/
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-24 16:27:33.000000 lusid_express-1.0.1/src/lusid_express/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 16:28:17.409393 lusid_express-1.0.1/src/lusid_express/display/
--rw-rw-rw-   0 root         (0) root         (0)      518 2024-04-24 16:27:33.000000 lusid_express-1.0.1/src/lusid_express/display/PRELOADED_VARS.md
--rw-rw-rw-   0 root         (0) root         (0)     7681 2024-04-24 16:27:33.000000 lusid_express-1.0.1/src/lusid_express/display/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2352 2024-04-24 16:27:33.000000 lusid_express-1.0.1/src/lusid_express/load.le
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 16:28:17.407394 lusid_express-1.0.1/src/lusid_express.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6659 2024-04-24 16:28:17.000000 lusid_express-1.0.1/src/lusid_express.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      482 2024-04-24 16:28:17.000000 lusid_express-1.0.1/src/lusid_express.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 16:28:17.000000 lusid_express-1.0.1/src/lusid_express.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      479 2024-04-24 16:28:17.000000 lusid_express-1.0.1/src/lusid_express.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-24 16:28:17.000000 lusid_express-1.0.1/src/lusid_express.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:43.985122 lusid_express-1.0.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-04-25 19:05:03.000000 lusid_express-1.0.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-04-25 19:05:03.000000 lusid_express-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6659 2024-04-25 19:05:43.985122 lusid_express-1.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6019 2024-04-25 19:05:03.000000 lusid_express-1.0.3/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 19:05:43.985122 lusid_express-1.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1536 2024-04-25 19:05:03.000000 lusid_express-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:43.980122 lusid_express-1.0.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:43.981122 lusid_express-1.0.3/src/lusid_express/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2024-04-25 19:05:03.000000 lusid_express-1.0.3/src/lusid_express/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5616 2024-04-25 19:05:03.000000 lusid_express-1.0.3/src/lusid_express/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:43.982122 lusid_express-1.0.3/src/lusid_express/apis/
+-rw-rw-rw-   0 root         (0) root         (0)  2240138 2024-04-25 19:05:43.000000 lusid_express-1.0.3/src/lusid_express/apis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:43.984122 lusid_express-1.0.3/src/lusid_express/config/
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-25 19:05:03.000000 lusid_express-1.0.3/src/lusid_express/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:43.985122 lusid_express-1.0.3/src/lusid_express/display/
+-rw-rw-rw-   0 root         (0) root         (0)      518 2024-04-25 19:05:03.000000 lusid_express-1.0.3/src/lusid_express/display/PRELOADED_VARS.md
+-rw-rw-rw-   0 root         (0) root         (0)     7768 2024-04-25 19:05:03.000000 lusid_express-1.0.3/src/lusid_express/display/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2352 2024-04-25 19:05:03.000000 lusid_express-1.0.3/src/lusid_express/load.le
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:43.982122 lusid_express-1.0.3/src/lusid_express.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6659 2024-04-25 19:05:43.000000 lusid_express-1.0.3/src/lusid_express.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      482 2024-04-25 19:05:43.000000 lusid_express-1.0.3/src/lusid_express.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 19:05:43.000000 lusid_express-1.0.3/src/lusid_express.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      479 2024-04-25 19:05:43.000000 lusid_express-1.0.3/src/lusid_express.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-25 19:05:43.000000 lusid_express-1.0.3/src/lusid_express.egg-info/top_level.txt
```

### Comparing `lusid_express-1.0.1/LICENSE` & `lusid_express-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lusid_express-1.0.1/PKG-INFO` & `lusid_express-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid_express
-Version: 1.0.1
+Version: 1.0.3
 Summary: lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-express
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lusid_express-1.0.1/README.md` & `lusid_express-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `lusid_express-1.0.1/setup.py` & `lusid_express-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,25 +13,25 @@
 'finbourne-insights-sdk-preview==0.0.763',
 'finbourne-sdk-utilities==0.0.10',
 'lusid-configuration-sdk-preview==0.1.514',
 'lusid-drive-sdk-preview==0.1.617',
 'lusid-notifications-sdk-preview==0.1.923',
 'lusid-scheduler-sdk-preview==0.0.829',
 'lusid-workflow-sdk-preview==0.1.810',
-'lusidtools==1.0.14',
+'lusidtools==1.0.34',
 'dve-lumipy-preview==0.1.1075',
 
 ]
 
 
 
 
 setup(
     name='lusid_express',
-    version='1.0.1',
+    version='1.0.3',
     package_dir={'': 'src'},  # tells setuptools that packages are under src
     packages=find_packages(where='src'),  # tells setuptools to look for packages in src
     install_requires=requirements,
     description='lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.',
     long_description=open('README.md').read(),
     include_package_data=True,  
     long_description_content_type='text/markdown',
```

### Comparing `lusid_express-1.0.1/src/lusid_express/__main__.py` & `lusid_express-1.0.3/src/lusid_express/__main__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-1.0.1/src/lusid_express/apis/__init__.py` & `lusid_express-1.0.3/src/lusid_express/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-1.0.1/src/lusid_express/display/PRELOADED_VARS.md` & `lusid_express-1.0.3/src/lusid_express/display/PRELOADED_VARS.md`

 * *Files identical despite different names*

### Comparing `lusid_express-1.0.1/src/lusid_express/display/__init__.py` & `lusid_express-1.0.3/src/lusid_express/display/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from IPython.display import Markdown as render_markdown, HTML as render_html
 import os as __os
 import json as __json
 import re
+from uuid import uuid4 as UUID
 
 with open(__os.path.join(__os.path.dirname(__file__), "PRELOADED_VARS.md"), "r") as __f:
     PRELOADED_VARS_MARKDOWN = __f.read()
 
 
 def data_to_markdown(data, col_name_key="Key", col_name_value="Value", title="table"):
     """
@@ -199,19 +200,22 @@
 
     table = ""
 
     # return f"## {title}\n{markdown_table}"
     def get_row(key, value):
         return f"<tr><td><h3>{key}</h3></td><td><p>{value}</p></td></tr>"
 
+    
+    id = f"DATA_TABLE-{UUID()}"
     # Add each key-value pair as a row in the table
     for key, value in data.items():
         # Ensure the value is converted to a string if necessary
         table += get_row(key, value)
-    return f"""<h1>{title}</h1> <table id='data_table'><tr><th><h2>{col_name_key}</h2></th><th><h2>{col_name_value}</h2></th></tr>{table}</table  >{COPY_SCRIPT}"""
+
+    return f"""<h1>{title}</h1> <table id={id}><tr><th><h2>{col_name_key}</h2></th><th><h2>{col_name_value}</h2></th></tr>{table}</table  >{COPY_SCRIPT.replace('data_table', id)}"""
 
 
 def render_table(data, col_name_key="Key", col_name_value="Value", title="table"):
     """
     Renders table from data.
 
     Parameters:
```

### Comparing `lusid_express-1.0.1/src/lusid_express/load.le` & `lusid_express-1.0.3/src/lusid_express/load.le`

 * *Files identical despite different names*

### Comparing `lusid_express-1.0.1/src/lusid_express.egg-info/PKG-INFO` & `lusid_express-1.0.3/src/lusid_express.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid-express
-Version: 1.0.1
+Version: 1.0.3
 Summary: lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-express
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

