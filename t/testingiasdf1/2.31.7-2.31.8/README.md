# Comparing `tmp/testingiasdf1-2.31.7.tar.gz` & `tmp/testingiasdf1-2.31.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testingiasdf1-2.31.7.tar", last modified: Thu Apr 25 02:49:13 2024, max compression
+gzip compressed data, was "testingiasdf1-2.31.8.tar", last modified: Thu Apr 25 02:54:43 2024, max compression
```

## Comparing `testingiasdf1-2.31.7.tar` & `testingiasdf1-2.31.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 02:49:13.127293 testingiasdf1-2.31.7/
--rw-rw-rw-   0        0        0     3147 2024-04-25 02:49:13.119428 testingiasdf1-2.31.7/PKG-INFO
--rw-rw-rw-   0        0        0     2847 2024-04-24 22:34:38.000000 testingiasdf1-2.31.7/README.md
--rw-rw-rw-   0        0        0       42 2024-04-25 02:49:13.127293 testingiasdf1-2.31.7/setup.cfg
--rw-rw-rw-   0        0        0     1369 2024-04-25 02:49:06.000000 testingiasdf1-2.31.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 02:49:13.069619 testingiasdf1-2.31.7/src/
-drwxrwxrwx   0        0        0        0 2024-04-25 02:49:13.083662 testingiasdf1-2.31.7/src/roblox_api_wrapper/
--rw-rw-rw-   0        0        0        0 2024-04-24 22:03:09.000000 testingiasdf1-2.31.7/src/roblox_api_wrapper/__init__.py
--rw-rw-rw-   0        0        0      119 2024-04-24 22:03:09.000000 testingiasdf1-2.31.7/src/roblox_api_wrapper/getuserinfo.py
--rw-rw-rw-   0        0        0      145 2024-04-24 22:03:09.000000 testingiasdf1-2.31.7/src/roblox_api_wrapper/login.py
--rw-rw-rw-   0        0        0      107 2024-04-24 22:03:09.000000 testingiasdf1-2.31.7/src/roblox_api_wrapper/message.py
-drwxrwxrwx   0        0        0        0 2024-04-25 02:49:13.116993 testingiasdf1-2.31.7/src/testingiasdf1.egg-info/
--rw-rw-rw-   0        0        0     3147 2024-04-25 02:49:12.000000 testingiasdf1-2.31.7/src/testingiasdf1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      321 2024-04-25 02:49:12.000000 testingiasdf1-2.31.7/src/testingiasdf1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 02:49:12.000000 testingiasdf1-2.31.7/src/testingiasdf1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-04-25 02:49:12.000000 testingiasdf1-2.31.7/src/testingiasdf1.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 02:54:43.292016 testingiasdf1-2.31.8/
+-rw-rw-rw-   0        0        0     3147 2024-04-25 02:54:43.279125 testingiasdf1-2.31.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2847 2024-04-24 22:34:38.000000 testingiasdf1-2.31.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-25 02:54:43.292016 testingiasdf1-2.31.8/setup.cfg
+-rw-rw-rw-   0        0        0     2111 2024-04-25 02:54:31.000000 testingiasdf1-2.31.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 02:54:43.211389 testingiasdf1-2.31.8/src/
+drwxrwxrwx   0        0        0        0 2024-04-25 02:54:43.243253 testingiasdf1-2.31.8/src/roblox_api_wrapper/
+-rw-rw-rw-   0        0        0        0 2024-04-24 22:03:09.000000 testingiasdf1-2.31.8/src/roblox_api_wrapper/__init__.py
+-rw-rw-rw-   0        0        0      119 2024-04-24 22:03:09.000000 testingiasdf1-2.31.8/src/roblox_api_wrapper/getuserinfo.py
+-rw-rw-rw-   0        0        0      145 2024-04-24 22:03:09.000000 testingiasdf1-2.31.8/src/roblox_api_wrapper/login.py
+-rw-rw-rw-   0        0        0      107 2024-04-24 22:03:09.000000 testingiasdf1-2.31.8/src/roblox_api_wrapper/message.py
+drwxrwxrwx   0        0        0        0 2024-04-25 02:54:43.276788 testingiasdf1-2.31.8/src/testingiasdf1.egg-info/
+-rw-rw-rw-   0        0        0     3147 2024-04-25 02:54:43.000000 testingiasdf1-2.31.8/src/testingiasdf1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2024-04-25 02:54:43.000000 testingiasdf1-2.31.8/src/testingiasdf1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 02:54:43.000000 testingiasdf1-2.31.8/src/testingiasdf1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-04-25 02:54:43.000000 testingiasdf1-2.31.8/src/testingiasdf1.egg-info/top_level.txt
```

### Comparing `testingiasdf1-2.31.7/PKG-INFO` & `testingiasdf1-2.31.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testingiasdf1
-Version: 2.31.7
+Version: 2.31.8
 Summary: Python MultiHTTP for Humans.
 Author: testingiasdf1
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `testingiasdf1-2.31.7/README.md` & `testingiasdf1-2.31.8/README.md`

 * *Files identical despite different names*

### Comparing `testingiasdf1-2.31.7/src/testingiasdf1.egg-info/PKG-INFO` & `testingiasdf1-2.31.8/src/testingiasdf1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testingiasdf1
-Version: 2.31.7
+Version: 2.31.8
 Summary: Python MultiHTTP for Humans.
 Author: testingiasdf1
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

