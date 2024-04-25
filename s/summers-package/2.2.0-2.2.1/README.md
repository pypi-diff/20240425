# Comparing `tmp/summers_package-2.2.0.tar.gz` & `tmp/summers_package-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "summers_package-2.2.0.tar", last modified: Thu Apr 25 16:36:29 2024, max compression
+gzip compressed data, was "summers_package-2.2.1.tar", last modified: Thu Apr 25 16:38:52 2024, max compression
```

## Comparing `summers_package-2.2.0.tar` & `summers_package-2.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 16:36:29.227150 summers_package-2.2.0/
--rw-rw-rw-   0        0        0     1098 2024-04-25 07:54:50.000000 summers_package-2.2.0/License.txt
--rw-rw-rw-   0        0        0     1201 2024-04-25 16:36:29.225153 summers_package-2.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      743 2024-04-25 16:36:13.000000 summers_package-2.2.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-25 16:36:29.228151 summers_package-2.2.0/setup.cfg
--rw-rw-rw-   0        0        0      662 2024-04-25 16:36:26.000000 summers_package-2.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 16:36:29.198150 summers_package-2.2.0/summers_package/
--rw-rw-rw-   0        0        0      114 2024-04-24 19:55:40.000000 summers_package-2.2.0/summers_package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 16:36:29.224158 summers_package-2.2.0/summers_package.egg-info/
--rw-rw-rw-   0        0        0     1201 2024-04-25 16:36:29.000000 summers_package-2.2.0/summers_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2024-04-25 16:36:29.000000 summers_package-2.2.0/summers_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 16:36:29.000000 summers_package-2.2.0/summers_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-25 16:36:29.000000 summers_package-2.2.0/summers_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 16:38:52.105395 summers_package-2.2.1/
+-rw-rw-rw-   0        0        0     1098 2024-04-25 07:54:50.000000 summers_package-2.2.1/License.txt
+-rw-rw-rw-   0        0        0     1299 2024-04-25 16:38:52.103395 summers_package-2.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      841 2024-04-25 16:38:41.000000 summers_package-2.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-25 16:38:52.105395 summers_package-2.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      662 2024-04-25 16:38:50.000000 summers_package-2.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 16:38:52.081395 summers_package-2.2.1/summers_package/
+-rw-rw-rw-   0        0        0      114 2024-04-24 19:55:40.000000 summers_package-2.2.1/summers_package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 16:38:52.101395 summers_package-2.2.1/summers_package.egg-info/
+-rw-rw-rw-   0        0        0     1299 2024-04-25 16:38:51.000000 summers_package-2.2.1/summers_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2024-04-25 16:38:52.000000 summers_package-2.2.1/summers_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 16:38:51.000000 summers_package-2.2.1/summers_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-25 16:38:51.000000 summers_package-2.2.1/summers_package.egg-info/top_level.txt
```

### Comparing `summers_package-2.2.0/License.txt` & `summers_package-2.2.1/License.txt`

 * *Files identical despite different names*

### Comparing `summers_package-2.2.0/PKG-INFO` & `summers_package-2.2.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: summers_package
-Version: 2.2.0
+Version: 2.2.1
 Summary: For doing calculations like Addition, Multiplication and Subtraction
 Author: Ansh Gupta
 Author-email: Ansh.Gupta@iiitb.ac.in
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,11 +24,11 @@
 
 ## 3. _subtract_
     This function subtracts two numbers and returns the result.
 
 # __Instructions to install the package__
 
 ## Open Terminal and type __pip install summers_package__
-![Terminal](https://i.im.ge/2024/04/25/Z02vwr.WhatsApp-Image-2024-04-25-at-9-06-51-PM.jpeg)
+![Terminal](https://iiitbac-my.sharepoint.com/:i:/g/personal/ansh_gupta_iiitb_ac_in/EZIYr2H_ndNJhn--lE5ifHIBHKTkTSCY_oXMzMuMa2wAVw?e=tMVS5r)
 
 ## After installing, this message will appear
-![Terminal](https://i.im.ge/2024/04/25/Z02kA1.WhatsApp-Image-2024-04-25-at-9-12-46-PM.jpeg)
+![Terminal](https://iiitbac-my.sharepoint.com/:i:/g/personal/ansh_gupta_iiitb_ac_in/ESG_vHRUTahPvZXOB4Y7DHsBBnQwF34FwIolcE-byd43ew?e=6fW0yF)
```

### Comparing `summers_package-2.2.0/setup.py` & `summers_package-2.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh: 
 	long_description = fh.read() 
 
 setuptools.setup( 
 	name="summers_package", 
 
-	version="2.2.0", 
+	version="2.2.1", 
 
 	author="Ansh Gupta", 
 
 	author_email="Ansh.Gupta@iiitb.ac.in", 
 
 	description="For doing calculations like Addition, Multiplication and Subtraction",
```

### Comparing `summers_package-2.2.0/summers_package.egg-info/PKG-INFO` & `summers_package-2.2.1/summers_package.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: summers_package
-Version: 2.2.0
+Version: 2.2.1
 Summary: For doing calculations like Addition, Multiplication and Subtraction
 Author: Ansh Gupta
 Author-email: Ansh.Gupta@iiitb.ac.in
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,11 +24,11 @@
 
 ## 3. _subtract_
     This function subtracts two numbers and returns the result.
 
 # __Instructions to install the package__
 
 ## Open Terminal and type __pip install summers_package__
-![Terminal](https://i.im.ge/2024/04/25/Z02vwr.WhatsApp-Image-2024-04-25-at-9-06-51-PM.jpeg)
+![Terminal](https://iiitbac-my.sharepoint.com/:i:/g/personal/ansh_gupta_iiitb_ac_in/EZIYr2H_ndNJhn--lE5ifHIBHKTkTSCY_oXMzMuMa2wAVw?e=tMVS5r)
 
 ## After installing, this message will appear
-![Terminal](https://i.im.ge/2024/04/25/Z02kA1.WhatsApp-Image-2024-04-25-at-9-12-46-PM.jpeg)
+![Terminal](https://iiitbac-my.sharepoint.com/:i:/g/personal/ansh_gupta_iiitb_ac_in/ESG_vHRUTahPvZXOB4Y7DHsBBnQwF34FwIolcE-byd43ew?e=6fW0yF)
```

