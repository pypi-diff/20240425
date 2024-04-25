# Comparing `tmp/lusid_express-1.0.3.tar.gz` & `tmp/lusid_express-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_express-1.0.3.tar", last modified: Thu Apr 25 19:05:43 2024, max compression
+gzip compressed data, was "lusid_express-1.0.4.tar", last modified: Thu Apr 25 19:36:05 2024, max compression
```

## Comparing `lusid_express-1.0.3.tar` & `lusid_express-1.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:43.985122 lusid_express-1.0.3/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-04-25 19:05:03.000000 lusid_express-1.0.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-04-25 19:05:03.000000 lusid_express-1.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6659 2024-04-25 19:05:43.985122 lusid_express-1.0.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6019 2024-04-25 19:05:03.000000 lusid_express-1.0.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 19:05:43.985122 lusid_express-1.0.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1536 2024-04-25 19:05:03.000000 lusid_express-1.0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:43.980122 lusid_express-1.0.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:43.981122 lusid_express-1.0.3/src/lusid_express/
--rw-rw-rw-   0 root         (0) root         (0)       30 2024-04-25 19:05:03.000000 lusid_express-1.0.3/src/lusid_express/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5616 2024-04-25 19:05:03.000000 lusid_express-1.0.3/src/lusid_express/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:43.982122 lusid_express-1.0.3/src/lusid_express/apis/
--rw-rw-rw-   0 root         (0) root         (0)  2240138 2024-04-25 19:05:43.000000 lusid_express-1.0.3/src/lusid_express/apis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:43.984122 lusid_express-1.0.3/src/lusid_express/config/
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-25 19:05:03.000000 lusid_express-1.0.3/src/lusid_express/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:43.985122 lusid_express-1.0.3/src/lusid_express/display/
--rw-rw-rw-   0 root         (0) root         (0)      518 2024-04-25 19:05:03.000000 lusid_express-1.0.3/src/lusid_express/display/PRELOADED_VARS.md
--rw-rw-rw-   0 root         (0) root         (0)     7768 2024-04-25 19:05:03.000000 lusid_express-1.0.3/src/lusid_express/display/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2352 2024-04-25 19:05:03.000000 lusid_express-1.0.3/src/lusid_express/load.le
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:43.982122 lusid_express-1.0.3/src/lusid_express.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6659 2024-04-25 19:05:43.000000 lusid_express-1.0.3/src/lusid_express.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      482 2024-04-25 19:05:43.000000 lusid_express-1.0.3/src/lusid_express.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 19:05:43.000000 lusid_express-1.0.3/src/lusid_express.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      479 2024-04-25 19:05:43.000000 lusid_express-1.0.3/src/lusid_express.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-25 19:05:43.000000 lusid_express-1.0.3/src/lusid_express.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:36:05.792996 lusid_express-1.0.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-04-25 19:35:24.000000 lusid_express-1.0.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-04-25 19:35:24.000000 lusid_express-1.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6659 2024-04-25 19:36:05.792996 lusid_express-1.0.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6019 2024-04-25 19:35:24.000000 lusid_express-1.0.4/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 19:36:05.793996 lusid_express-1.0.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1536 2024-04-25 19:35:24.000000 lusid_express-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:36:05.787996 lusid_express-1.0.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:36:05.788996 lusid_express-1.0.4/src/lusid_express/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2024-04-25 19:35:24.000000 lusid_express-1.0.4/src/lusid_express/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5616 2024-04-25 19:35:24.000000 lusid_express-1.0.4/src/lusid_express/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:36:05.789996 lusid_express-1.0.4/src/lusid_express/apis/
+-rw-rw-rw-   0 root         (0) root         (0)  2240138 2024-04-25 19:36:05.000000 lusid_express-1.0.4/src/lusid_express/apis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:36:05.792996 lusid_express-1.0.4/src/lusid_express/config/
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-25 19:35:24.000000 lusid_express-1.0.4/src/lusid_express/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:36:05.792996 lusid_express-1.0.4/src/lusid_express/display/
+-rw-rw-rw-   0 root         (0) root         (0)      518 2024-04-25 19:35:24.000000 lusid_express-1.0.4/src/lusid_express/display/PRELOADED_VARS.md
+-rw-rw-rw-   0 root         (0) root         (0)     8675 2024-04-25 19:35:24.000000 lusid_express-1.0.4/src/lusid_express/display/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2352 2024-04-25 19:35:24.000000 lusid_express-1.0.4/src/lusid_express/load.le
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:36:05.789996 lusid_express-1.0.4/src/lusid_express.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6659 2024-04-25 19:36:05.000000 lusid_express-1.0.4/src/lusid_express.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      482 2024-04-25 19:36:05.000000 lusid_express-1.0.4/src/lusid_express.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 19:36:05.000000 lusid_express-1.0.4/src/lusid_express.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      479 2024-04-25 19:36:05.000000 lusid_express-1.0.4/src/lusid_express.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-25 19:36:05.000000 lusid_express-1.0.4/src/lusid_express.egg-info/top_level.txt
```

### Comparing `lusid_express-1.0.3/LICENSE` & `lusid_express-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lusid_express-1.0.3/PKG-INFO` & `lusid_express-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid_express
-Version: 1.0.3
+Version: 1.0.4
 Summary: lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-express
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lusid_express-1.0.3/README.md` & `lusid_express-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `lusid_express-1.0.3/setup.py` & `lusid_express-1.0.4/setup.py`

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
-'lusidtools==1.0.34',
+'lusidtools==1.0.44',
 'dve-lumipy-preview==0.1.1075',
 
 ]
 
 
 
 
 setup(
     name='lusid_express',
-    version='1.0.3',
+    version='1.0.4',
     package_dir={'': 'src'},  # tells setuptools that packages are under src
     packages=find_packages(where='src'),  # tells setuptools to look for packages in src
     install_requires=requirements,
     description='lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.',
     long_description=open('README.md').read(),
     include_package_data=True,  
     long_description_content_type='text/markdown',
```

### Comparing `lusid_express-1.0.3/src/lusid_express/__main__.py` & `lusid_express-1.0.4/src/lusid_express/__main__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-1.0.3/src/lusid_express/apis/__init__.py` & `lusid_express-1.0.4/src/lusid_express/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-1.0.3/src/lusid_express/display/PRELOADED_VARS.md` & `lusid_express-1.0.4/src/lusid_express/display/PRELOADED_VARS.md`

 * *Files identical despite different names*

### Comparing `lusid_express-1.0.3/src/lusid_express/display/__init__.py` & `lusid_express-1.0.4/src/lusid_express/display/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,54 @@
     for key, value in data.items():
         # Ensure the value is converted to a string if necessary
         markdown_table += f"{key} | {str(value)}\n"
 
     return f"## {title}\n{markdown_table}"
 
 
-COPY_SCRIPT = """ <button  onclick='copyTable()'>Copy to Clipboard</button>
+COPY_SCRIPT = """ 
+<style>
+.button {
+  background-color: #FFFFFF;
+  border: 1px solid rgb(209,213,219);
+  border-radius: .5rem;
+  box-sizing: border-box;
+  color: #111827;
+  font-family: "Inter var",ui-sans-serif,system-ui,-apple-system,system-ui,"Segoe UI",Roboto,"Helvetica Neue",Arial,"Noto Sans",sans-serif,"Apple Color Emoji","Segoe UI Emoji","Segoe UI Symbol","Noto Color Emoji";
+  font-size: .875rem;
+  font-weight: 600;
+  line-height: 1.25rem;
+  padding: .75rem 1rem;
+  text-align: center;
+  text-decoration: none #D1D5DB solid;
+  text-decoration-thickness: auto;
+  box-shadow: 0 1px 2px 0 rgba(0, 0, 0, 0.05);
+  cursor: pointer;
+  user-select: none;
+  -webkit-user-select: none;
+  touch-action: manipulation;
+}
+
+.button:hover {
+  background-color: rgb(249,250,251);
+}
+
+.button:focus {
+  outline: 2px solid transparent;
+  outline-offset: 2px;
+}
+
+.button:focus-visible {
+  box-shadow: none;
+}
+</style>
+<button 
+class="button"
+
+onclick='copyTable()'>Copy to Clipboard</button>
  <script>
         function copyTable() {{
             var rows = document.querySelectorAll('#data_table tr');
             var csvContent = '';
             rows.forEach(function(row, index) {{
                 var cols = row.querySelectorAll('th, td');
                 var rowData = [];
```

### Comparing `lusid_express-1.0.3/src/lusid_express/load.le` & `lusid_express-1.0.4/src/lusid_express/load.le`

 * *Files identical despite different names*

### Comparing `lusid_express-1.0.3/src/lusid_express.egg-info/PKG-INFO` & `lusid_express-1.0.4/src/lusid_express.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid-express
-Version: 1.0.3
+Version: 1.0.4
 Summary: lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-express
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

