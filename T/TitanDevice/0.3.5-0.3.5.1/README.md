# Comparing `tmp/TitanDevice-0.3.5.tar.gz` & `tmp/TitanDevice-0.3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TitanDevice-0.3.5.tar", last modified: Thu Apr 25 02:43:53 2024, max compression
+gzip compressed data, was "TitanDevice-0.3.5.1.tar", last modified: Thu Apr 25 02:45:05 2024, max compression
```

## Comparing `TitanDevice-0.3.5.tar` & `TitanDevice-0.3.5.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-25 02:43:53.780698 TitanDevice-0.3.5/
--rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-25 02:43:53.780698 TitanDevice-0.3.5/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 TitanDevice-0.3.5/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-25 02:43:53.780698 TitanDevice-0.3.5/TitanDevice.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-25 02:43:53.000000 TitanDevice-0.3.5/TitanDevice.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      286 2024-04-25 02:43:53.000000 TitanDevice-0.3.5/TitanDevice.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-25 02:43:53.000000 TitanDevice-0.3.5/TitanDevice.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-25 02:43:53.000000 TitanDevice-0.3.5/TitanDevice.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-04-25 02:43:53.000000 TitanDevice-0.3.5/TitanDevice.egg-info/top_level.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-25 02:43:53.780698 TitanDevice-0.3.5/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-04-25 02:43:47.000000 TitanDevice-0.3.5/setup.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-25 02:43:53.780698 TitanDevice-0.3.5/titan/
--rw-rw-r--   0 mark      (1000) mark      (1000)     3278 2024-04-25 02:18:35.000000 TitanDevice-0.3.5/titan/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1242 2024-04-25 02:18:35.000000 TitanDevice-0.3.5/titan/_device_exception.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     6152 2024-04-25 02:43:20.000000 TitanDevice-0.3.5/titan/_device_manager.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      465 2024-04-25 01:48:01.000000 TitanDevice-0.3.5/titan/_device_models.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-25 02:45:05.453466 TitanDevice-0.3.5.1/
+-rw-r--r--   0 mark      (1000) mark      (1000)      598 2024-04-25 02:45:05.453466 TitanDevice-0.3.5.1/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 TitanDevice-0.3.5.1/README.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-25 02:45:05.453466 TitanDevice-0.3.5.1/TitanDevice.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)      598 2024-04-25 02:45:05.000000 TitanDevice-0.3.5.1/TitanDevice.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      286 2024-04-25 02:45:05.000000 TitanDevice-0.3.5.1/TitanDevice.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-25 02:45:05.000000 TitanDevice-0.3.5.1/TitanDevice.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-25 02:45:05.000000 TitanDevice-0.3.5.1/TitanDevice.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-04-25 02:45:05.000000 TitanDevice-0.3.5.1/TitanDevice.egg-info/top_level.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-25 02:45:05.453466 TitanDevice-0.3.5.1/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      798 2024-04-25 02:45:02.000000 TitanDevice-0.3.5.1/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-25 02:45:05.453466 TitanDevice-0.3.5.1/titan/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     3278 2024-04-25 02:18:35.000000 TitanDevice-0.3.5.1/titan/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1242 2024-04-25 02:18:35.000000 TitanDevice-0.3.5.1/titan/_device_exception.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     6152 2024-04-25 02:43:20.000000 TitanDevice-0.3.5.1/titan/_device_manager.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      472 2024-04-25 02:45:02.000000 TitanDevice-0.3.5.1/titan/_device_models.py
```

### Comparing `TitanDevice-0.3.5/PKG-INFO` & `TitanDevice-0.3.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TitanDevice
-Version: 0.3.5
+Version: 0.3.5.1
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `TitanDevice-0.3.5/TitanDevice.egg-info/PKG-INFO` & `TitanDevice-0.3.5.1/TitanDevice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TitanDevice
-Version: 0.3.5
+Version: 0.3.5.1
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `TitanDevice-0.3.5/setup.py` & `TitanDevice-0.3.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read_readme():
     with open(os.path.join(os.getcwd(), 'README.md'), 'r', encoding='utf-8') as file:
         return file.read()
 
 
 setup(
     name="TitanDevice",
-    version="0.3.5",
+    version="0.3.5.1",
     author="369",
     author_email="luck.yangbo@gmai.com",
     description="A Python library used for managing device",
     long_description=read_readme(),
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `TitanDevice-0.3.5/titan/__init__.py` & `TitanDevice-0.3.5.1/titan/__init__.py`

 * *Files identical despite different names*

### Comparing `TitanDevice-0.3.5/titan/_device_exception.py` & `TitanDevice-0.3.5.1/titan/_device_exception.py`

 * *Files identical despite different names*

### Comparing `TitanDevice-0.3.5/titan/_device_manager.py` & `TitanDevice-0.3.5.1/titan/_device_manager.py`

 * *Files identical despite different names*

