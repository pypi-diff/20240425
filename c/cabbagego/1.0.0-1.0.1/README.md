# Comparing `tmp/cabbagego-1.0.0.tar.gz` & `tmp/cabbagego-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cabbagego-1.0.0.tar", last modified: Thu Apr 25 18:22:08 2024, max compression
+gzip compressed data, was "cabbagego-1.0.1.tar", last modified: Thu Apr 25 18:22:51 2024, max compression
```

## Comparing `cabbagego-1.0.0.tar` & `cabbagego-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 18:22:08.212879 cabbagego-1.0.0/
--rw-rw-rw-   0        0        0     1276 2024-04-25 18:22:08.212267 cabbagego-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      281 2024-04-25 18:19:24.000000 cabbagego-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 18:22:08.179232 cabbagego-1.0.0/cabbage/
--rw-rw-rw-   0        0        0     3173 2024-04-25 18:14:21.000000 cabbagego-1.0.0/cabbage/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 18:22:08.181243 cabbagego-1.0.0/cabbage/core/
--rw-rw-rw-   0        0        0        0 2024-04-24 05:16:34.000000 cabbagego-1.0.0/cabbage/core/__init__.py
--rw-rw-rw-   0        0        0     1523 2024-04-25 18:03:12.000000 cabbagego-1.0.0/cabbage/core/bcore.py
--rw-rw-rw-   0        0        0     1666 2024-04-25 18:03:08.000000 cabbagego-1.0.0/cabbage/core/dcore.py
-drwxrwxrwx   0        0        0        0 2024-04-25 18:22:08.182922 cabbagego-1.0.0/cabbage/io/
--rw-rw-rw-   0        0        0        0 2024-04-24 05:16:43.000000 cabbagego-1.0.0/cabbage/io/__init__.py
--rw-rw-rw-   0        0        0      590 2024-04-25 18:05:06.000000 cabbagego-1.0.0/cabbage/io/reader.py
--rw-rw-rw-   0        0        0      762 2024-04-25 18:07:34.000000 cabbagego-1.0.0/cabbage/io/saver.py
-drwxrwxrwx   0        0        0        0 2024-04-25 18:22:08.184079 cabbagego-1.0.0/cabbage/model/
--rw-rw-rw-   0        0        0        0 2024-04-25 15:42:20.000000 cabbagego-1.0.0/cabbage/model/__init__.py
--rw-rw-rw-   0        0        0      912 2024-04-25 18:02:45.000000 cabbagego-1.0.0/cabbage/model/data.py
-drwxrwxrwx   0        0        0        0 2024-04-25 18:22:08.211759 cabbagego-1.0.0/cabbagego.egg-info/
--rw-rw-rw-   0        0        0     1276 2024-04-25 18:22:08.000000 cabbagego-1.0.0/cabbagego.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2024-04-25 18:22:08.000000 cabbagego-1.0.0/cabbagego.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 18:22:08.000000 cabbagego-1.0.0/cabbagego.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-04-25 18:22:08.000000 cabbagego-1.0.0/cabbagego.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-25 18:22:08.000000 cabbagego-1.0.0/cabbagego.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 18:22:08.212879 cabbagego-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     4290 2024-04-25 18:22:04.000000 cabbagego-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:22:51.025050 cabbagego-1.0.1/
+-rw-rw-rw-   0        0        0     1280 2024-04-25 18:22:51.024457 cabbagego-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2024-04-25 18:22:34.000000 cabbagego-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 18:22:51.000849 cabbagego-1.0.1/cabbage/
+-rw-rw-rw-   0        0        0     3173 2024-04-25 18:14:21.000000 cabbagego-1.0.1/cabbage/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:22:51.002861 cabbagego-1.0.1/cabbage/core/
+-rw-rw-rw-   0        0        0        0 2024-04-24 05:16:34.000000 cabbagego-1.0.1/cabbage/core/__init__.py
+-rw-rw-rw-   0        0        0     1523 2024-04-25 18:03:12.000000 cabbagego-1.0.1/cabbage/core/bcore.py
+-rw-rw-rw-   0        0        0     1666 2024-04-25 18:03:08.000000 cabbagego-1.0.1/cabbage/core/dcore.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:22:51.003932 cabbagego-1.0.1/cabbage/io/
+-rw-rw-rw-   0        0        0        0 2024-04-24 05:16:43.000000 cabbagego-1.0.1/cabbage/io/__init__.py
+-rw-rw-rw-   0        0        0      590 2024-04-25 18:05:06.000000 cabbagego-1.0.1/cabbage/io/reader.py
+-rw-rw-rw-   0        0        0      762 2024-04-25 18:07:34.000000 cabbagego-1.0.1/cabbage/io/saver.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:22:51.005997 cabbagego-1.0.1/cabbage/model/
+-rw-rw-rw-   0        0        0        0 2024-04-25 15:42:20.000000 cabbagego-1.0.1/cabbage/model/__init__.py
+-rw-rw-rw-   0        0        0      912 2024-04-25 18:02:45.000000 cabbagego-1.0.1/cabbage/model/data.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:22:51.023952 cabbagego-1.0.1/cabbagego.egg-info/
+-rw-rw-rw-   0        0        0     1280 2024-04-25 18:22:50.000000 cabbagego-1.0.1/cabbagego.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2024-04-25 18:22:50.000000 cabbagego-1.0.1/cabbagego.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 18:22:50.000000 cabbagego-1.0.1/cabbagego.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-04-25 18:22:50.000000 cabbagego-1.0.1/cabbagego.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-25 18:22:50.000000 cabbagego-1.0.1/cabbagego.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 18:22:51.025556 cabbagego-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     4290 2024-04-25 18:22:47.000000 cabbagego-1.0.1/setup.py
```

### Comparing `cabbagego-1.0.0/PKG-INFO` & `cabbagego-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cabbagego
-Version: 1.0.0
+Version: 1.0.1
 Summary: Cabbage
 Home-page: 
 Author: Keyork
 Author-email: 
 License: Apache Software License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -26,15 +26,15 @@
 
 
 # Cabbage
 
 ## 使用方法
 
 ```python
-import cabbage
-client = cabbage.Cabbage()
+import cabbagego
+client = cabbagego.Cabbage()
 client.get_bilibili_path("datalist-bilibili.txt")
 client.set_target_dir("result")
 client.get_bilibili_data()  
 client.get_douyin_path("datalist-douyin.txt")
 client.get_douyin_data()  
 ```
```

### Comparing `cabbagego-1.0.0/cabbage/__init__.py` & `cabbagego-1.0.1/cabbage/__init__.py`

 * *Files identical despite different names*

### Comparing `cabbagego-1.0.0/cabbage/core/bcore.py` & `cabbagego-1.0.1/cabbage/core/bcore.py`

 * *Files identical despite different names*

### Comparing `cabbagego-1.0.0/cabbage/core/dcore.py` & `cabbagego-1.0.1/cabbage/core/dcore.py`

 * *Files identical despite different names*

### Comparing `cabbagego-1.0.0/cabbage/io/reader.py` & `cabbagego-1.0.1/cabbage/io/reader.py`

 * *Files identical despite different names*

### Comparing `cabbagego-1.0.0/cabbage/io/saver.py` & `cabbagego-1.0.1/cabbage/io/saver.py`

 * *Files identical despite different names*

### Comparing `cabbagego-1.0.0/cabbage/model/data.py` & `cabbagego-1.0.1/cabbage/model/data.py`

 * *Files identical despite different names*

### Comparing `cabbagego-1.0.0/cabbagego.egg-info/PKG-INFO` & `cabbagego-1.0.1/cabbagego.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cabbagego
-Version: 1.0.0
+Version: 1.0.1
 Summary: Cabbage
 Home-page: 
 Author: Keyork
 Author-email: 
 License: Apache Software License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -26,15 +26,15 @@
 
 
 # Cabbage
 
 ## 使用方法
 
 ```python
-import cabbage
-client = cabbage.Cabbage()
+import cabbagego
+client = cabbagego.Cabbage()
 client.get_bilibili_path("datalist-bilibili.txt")
 client.set_target_dir("result")
 client.get_bilibili_data()  
 client.get_douyin_path("datalist-douyin.txt")
 client.get_douyin_data()  
 ```
```

### Comparing `cabbagego-1.0.0/setup.py` & `cabbagego-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # Package meta-data.
 NAME = "cabbagego"
 DESCRIPTION = "Cabbage"
 URL = ""
 EMAIL = ""
 AUTHOR = "Keyork"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "1.0.0"
+VERSION = "1.0.1"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "selenium",
     "webdriver_manager",
 ]
```

