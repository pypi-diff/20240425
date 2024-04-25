# Comparing `tmp/enhancedwebdriver-0.1.4.tar.gz` & `tmp/enhancedwebdriver-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enhancedwebdriver-0.1.4.tar", last modified: Wed Apr 24 07:06:14 2024, max compression
+gzip compressed data, was "enhancedwebdriver-0.1.5.tar", last modified: Thu Apr 25 09:05:43 2024, max compression
```

## Comparing `enhancedwebdriver-0.1.4.tar` & `enhancedwebdriver-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-24 07:06:14.311576 enhancedwebdriver-0.1.4/
--rw-rw-r--   0 tesla     (1000) tesla     (1000)     1070 2024-04-12 20:08:24.000000 enhancedwebdriver-0.1.4/LICENSE
--rw-r--r--   0 tesla     (1000) tesla     (1000)     1089 2024-04-24 07:06:14.311576 enhancedwebdriver-0.1.4/PKG-INFO
--rw-rw-r--   0 tesla     (1000) tesla     (1000)      465 2024-04-13 15:12:35.000000 enhancedwebdriver-0.1.4/README.md
--rw-rw-r--   0 tesla     (1000) tesla     (1000)      106 2024-04-12 19:44:41.000000 enhancedwebdriver-0.1.4/pyproject.toml
--rw-rw-r--   0 tesla     (1000) tesla     (1000)      726 2024-04-24 07:06:14.311576 enhancedwebdriver-0.1.4/setup.cfg
-drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-24 07:06:14.307576 enhancedwebdriver-0.1.4/src/
-drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-24 07:06:14.311576 enhancedwebdriver-0.1.4/src/EnhancedWebdriver.egg-info/
--rw-r--r--   0 tesla     (1000) tesla     (1000)     1089 2024-04-24 07:06:14.000000 enhancedwebdriver-0.1.4/src/EnhancedWebdriver.egg-info/PKG-INFO
--rw-rw-r--   0 tesla     (1000) tesla     (1000)      345 2024-04-24 07:06:14.000000 enhancedwebdriver-0.1.4/src/EnhancedWebdriver.egg-info/SOURCES.txt
--rw-rw-r--   0 tesla     (1000) tesla     (1000)        1 2024-04-24 07:06:14.000000 enhancedwebdriver-0.1.4/src/EnhancedWebdriver.egg-info/dependency_links.txt
--rw-rw-r--   0 tesla     (1000) tesla     (1000)       46 2024-04-24 07:06:14.000000 enhancedwebdriver-0.1.4/src/EnhancedWebdriver.egg-info/requires.txt
--rw-rw-r--   0 tesla     (1000) tesla     (1000)       19 2024-04-24 07:06:14.000000 enhancedwebdriver-0.1.4/src/EnhancedWebdriver.egg-info/top_level.txt
-drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-24 07:06:14.311576 enhancedwebdriver-0.1.4/src/enhanced_webdriver/
--rw-rw-r--   0 tesla     (1000) tesla     (1000)    14311 2024-04-24 07:04:55.000000 enhancedwebdriver-0.1.4/src/enhanced_webdriver/EnhancedWebdriver.py
--rw-rw-r--   0 tesla     (1000) tesla     (1000)       82 2024-04-12 20:08:24.000000 enhancedwebdriver-0.1.4/src/enhanced_webdriver/__init__.py
+drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-25 09:05:43.070170 enhancedwebdriver-0.1.5/
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)     1070 2024-04-12 20:08:24.000000 enhancedwebdriver-0.1.5/LICENSE
+-rw-r--r--   0 tesla     (1000) tesla     (1000)     1106 2024-04-25 09:05:43.070170 enhancedwebdriver-0.1.5/PKG-INFO
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)      465 2024-04-13 15:12:35.000000 enhancedwebdriver-0.1.5/README.md
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)      106 2024-04-12 19:44:41.000000 enhancedwebdriver-0.1.5/pyproject.toml
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)      743 2024-04-25 09:05:43.070170 enhancedwebdriver-0.1.5/setup.cfg
+drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-25 09:05:43.066170 enhancedwebdriver-0.1.5/src/
+drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-25 09:05:43.070170 enhancedwebdriver-0.1.5/src/EnhancedWebdriver.egg-info/
+-rw-r--r--   0 tesla     (1000) tesla     (1000)     1106 2024-04-25 09:05:43.000000 enhancedwebdriver-0.1.5/src/EnhancedWebdriver.egg-info/PKG-INFO
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)      345 2024-04-25 09:05:43.000000 enhancedwebdriver-0.1.5/src/EnhancedWebdriver.egg-info/SOURCES.txt
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)        1 2024-04-25 09:05:43.000000 enhancedwebdriver-0.1.5/src/EnhancedWebdriver.egg-info/dependency_links.txt
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)       64 2024-04-25 09:05:43.000000 enhancedwebdriver-0.1.5/src/EnhancedWebdriver.egg-info/requires.txt
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)       19 2024-04-25 09:05:43.000000 enhancedwebdriver-0.1.5/src/EnhancedWebdriver.egg-info/top_level.txt
+drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-25 09:05:43.070170 enhancedwebdriver-0.1.5/src/enhanced_webdriver/
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)    10303 2024-04-25 09:01:33.000000 enhancedwebdriver-0.1.5/src/enhanced_webdriver/EnhancedWebdriver.py
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)       82 2024-04-12 20:08:24.000000 enhancedwebdriver-0.1.5/src/enhanced_webdriver/__init__.py
```

### Comparing `enhancedwebdriver-0.1.4/LICENSE` & `enhancedwebdriver-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `enhancedwebdriver-0.1.4/PKG-INFO` & `enhancedwebdriver-0.1.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: EnhancedWebdriver
-Version: 0.1.4
+Version: 0.1.5
 Summary: Extension of webdriver with less boilerplate
 Home-page: https://github.com/Tesla2000/EnhancedWebdriver
 Author: Tesla2000
 Author-email: fratajczak124@gmail.com
 Project-URL: Homepage, https://github.com/Tesla2000/EnhancedWebdriver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.05
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: selenium>=4.18.0
-Requires-Dist: download>=0.3.5
 Requires-Dist: retry>=0.9.2
+Requires-Dist: chromedriver-autoinstaller>=0.6.4
 
 # EnhancedWebdriver
 An informal extension of selenium webdriver with more error handling and more complex functions. Like keeping driver up to date with Chrome version
 
 Installation:
 `
```

### Comparing `enhancedwebdriver-0.1.4/setup.cfg` & `enhancedwebdriver-0.1.5/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = EnhancedWebdriver
-version = 0.1.4
+version = 0.1.5
 author = Tesla2000
 author_email = fratajczak124@gmail.com
 description = Extension of webdriver with less boilerplate
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Tesla2000/EnhancedWebdriver
 project_urls = 
@@ -14,19 +14,19 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
-python_requires = >=3.05
+python_requires = >=3.8
 install_requires = 
 	selenium>=4.18.0
-	download>=0.3.5
 	retry>=0.9.2
+	chromedriver-autoinstaller>=0.6.4
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `enhancedwebdriver-0.1.4/src/EnhancedWebdriver.egg-info/PKG-INFO` & `enhancedwebdriver-0.1.5/src/EnhancedWebdriver.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: EnhancedWebdriver
-Version: 0.1.4
+Version: 0.1.5
 Summary: Extension of webdriver with less boilerplate
 Home-page: https://github.com/Tesla2000/EnhancedWebdriver
 Author: Tesla2000
 Author-email: fratajczak124@gmail.com
 Project-URL: Homepage, https://github.com/Tesla2000/EnhancedWebdriver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.05
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: selenium>=4.18.0
-Requires-Dist: download>=0.3.5
 Requires-Dist: retry>=0.9.2
+Requires-Dist: chromedriver-autoinstaller>=0.6.4
 
 # EnhancedWebdriver
 An informal extension of selenium webdriver with more error handling and more complex functions. Like keeping driver up to date with Chrome version
 
 Installation:
 `
```

