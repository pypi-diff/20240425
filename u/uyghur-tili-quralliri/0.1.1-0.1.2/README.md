# Comparing `tmp/uyghur-tili-quralliri-0.1.1.tar.gz` & `tmp/uyghur-tili-quralliri-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uyghur-tili-quralliri-0.1.1.tar", last modified: Thu Apr 25 11:55:23 2024, max compression
+gzip compressed data, was "uyghur-tili-quralliri-0.1.2.tar", last modified: Thu Apr 25 12:14:05 2024, max compression
```

## Comparing `uyghur-tili-quralliri-0.1.1.tar` & `uyghur-tili-quralliri-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 11:55:23.424584 uyghur-tili-quralliri-0.1.1/
--rw-rw-rw-   0        0        0     1173 2024-04-25 11:55:23.424584 uyghur-tili-quralliri-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      625 2024-04-25 11:45:12.000000 uyghur-tili-quralliri-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-25 11:55:23.425555 uyghur-tili-quralliri-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      889 2024-04-25 11:43:59.000000 uyghur-tili-quralliri-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 11:55:23.422564 uyghur-tili-quralliri-0.1.1/uyghur_tili_quralliri.egg-info/
--rw-rw-rw-   0        0        0     1173 2024-04-25 11:55:23.000000 uyghur-tili-quralliri-0.1.1/uyghur_tili_quralliri.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2024-04-25 11:55:23.000000 uyghur-tili-quralliri-0.1.1/uyghur_tili_quralliri.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 11:55:23.000000 uyghur-tili-quralliri-0.1.1/uyghur_tili_quralliri.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 11:55:23.000000 uyghur-tili-quralliri-0.1.1/uyghur_tili_quralliri.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 12:14:05.405646 uyghur-tili-quralliri-0.1.2/
+-rw-rw-rw-   0        0        0     1131 2024-04-25 12:14:05.405646 uyghur-tili-quralliri-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      604 2024-04-25 12:11:17.000000 uyghur-tili-quralliri-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-25 12:14:05.406643 uyghur-tili-quralliri-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      889 2024-04-25 12:11:50.000000 uyghur-tili-quralliri-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:14:05.397668 uyghur-tili-quralliri-0.1.2/uyghur_language_tools/
+-rw-rw-rw-   0        0        0   104707 2024-04-25 12:14:05.000000 uyghur-tili-quralliri-0.1.2/uyghur_language_tools/UyghurLanguageTools.py
+-rw-rw-rw-   0        0        0       54 2024-04-25 10:47:20.000000 uyghur-tili-quralliri-0.1.2/uyghur_language_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:14:05.404650 uyghur-tili-quralliri-0.1.2/uyghur_tili_quralliri.egg-info/
+-rw-rw-rw-   0        0        0     1131 2024-04-25 12:14:05.000000 uyghur-tili-quralliri-0.1.2/uyghur_tili_quralliri.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2024-04-25 12:14:05.000000 uyghur-tili-quralliri-0.1.2/uyghur_tili_quralliri.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 12:14:05.000000 uyghur-tili-quralliri-0.1.2/uyghur_tili_quralliri.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-04-25 12:14:05.000000 uyghur-tili-quralliri-0.1.2/uyghur_tili_quralliri.egg-info/top_level.txt
```

### Comparing `uyghur-tili-quralliri-0.1.1/PKG-INFO` & `uyghur-tili-quralliri-0.1.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uyghur-tili-quralliri
-Version: 0.1.1
+Version: 0.1.2
 Summary: uyghur language writing and processing tool box ...
 Home-page: https://github.com/kompasim/uyghur-tili-quralliri
 Author: kompasim
 Author-email: kompasim@163.com
 License: MIT Licence
 Keywords: uyghur,uighur,til,yeziq,qural,language,tools
 Platform: any
@@ -27,18 +27,18 @@
 
 ## 2. Usage
 
 ```python
 from UyghurLanguageTools import UyghurLanguageTools as Tools
 Tools.main()
 # Uyghur Language Tools (0.1), for more infomation please visit ...
-origin = "賲蹠乇诰丕亘丕"
+origin = "merhaba"
 print(origin)
-# 賲蹠乇诰丕亘丕
+# merhaba
 target = Tools.toExtended(origin)
 print(target)
-# 賲蹠乇 诰丕 亘丕
+# mer ha ba
 ```
 
 ## 3. others
 
 > for more information please visit [github](https://github.com/kompasim/uyghur-tili-quralliri).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `uyghur-tili-quralliri-0.1.1/setup.py` & `uyghur-tili-quralliri-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name = "uyghur-tili-quralliri",
-    version = "0.1.1",
+    version = "0.1.2",
     keywords = ("uyghur", "uighur","til", "yeziq", "qural", "language", "tools"),
     description = "uyghur language writing and processing tool box ...",
     long_description = long_description,
     long_description_content_type="text/markdown",
     license = "MIT Licence",
 
     url = "https://github.com/kompasim/uyghur-tili-quralliri",
```

### Comparing `uyghur-tili-quralliri-0.1.1/uyghur_tili_quralliri.egg-info/PKG-INFO` & `uyghur-tili-quralliri-0.1.2/uyghur_tili_quralliri.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uyghur-tili-quralliri
-Version: 0.1.1
+Version: 0.1.2
 Summary: uyghur language writing and processing tool box ...
 Home-page: https://github.com/kompasim/uyghur-tili-quralliri
 Author: kompasim
 Author-email: kompasim@163.com
 License: MIT Licence
 Keywords: uyghur,uighur,til,yeziq,qural,language,tools
 Platform: any
@@ -27,18 +27,18 @@
 
 ## 2. Usage
 
 ```python
 from UyghurLanguageTools import UyghurLanguageTools as Tools
 Tools.main()
 # Uyghur Language Tools (0.1), for more infomation please visit ...
-origin = "賲蹠乇诰丕亘丕"
+origin = "merhaba"
 print(origin)
-# 賲蹠乇诰丕亘丕
+# merhaba
 target = Tools.toExtended(origin)
 print(target)
-# 賲蹠乇 诰丕 亘丕
+# mer ha ba
 ```
 
 ## 3. others
 
 > for more information please visit [github](https://github.com/kompasim/uyghur-tili-quralliri).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

