# Comparing `tmp/Plone-6.1.0a1.tar.gz` & `tmp/Plone-6.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Plone-6.1.0a1.tar", last modified: Fri Jan 26 00:49:46 2024, max compression
+gzip compressed data, was "Plone-6.1.0a2.tar", last modified: Tue Feb 27 16:17:28 2024, max compression
```

## Comparing `Plone-6.1.0a1.tar` & `Plone-6.1.0a2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-01-26 00:49:46.726990 Plone-6.1.0a1/
--rw-r--r--   0 maurits    (501) staff       (20)     7038 2024-01-26 00:49:46.000000 Plone-6.1.0a1/CHANGES.md
--rw-r--r--   0 maurits    (501) staff       (20)       73 2024-01-26 00:49:46.000000 Plone-6.1.0a1/CONTRIBUTING.md
--rw-r--r--   0 maurits    (501) staff       (20)       24 2024-01-26 00:49:46.000000 Plone-6.1.0a1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    15249 2024-01-26 00:49:46.726805 Plone-6.1.0a1/PKG-INFO
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-01-26 00:49:46.726003 Plone-6.1.0a1/Plone.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    15249 2024-01-26 00:49:46.000000 Plone-6.1.0a1/Plone.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      324 2024-01-26 00:49:46.000000 Plone-6.1.0a1/Plone.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-01-26 00:49:46.000000 Plone-6.1.0a1/Plone.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-01-26 00:49:46.000000 Plone-6.1.0a1/Plone.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      188 2024-01-26 00:49:46.000000 Plone-6.1.0a1/Plone.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-01-26 00:49:46.000000 Plone-6.1.0a1/Plone.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     6411 2024-01-26 00:49:46.000000 Plone-6.1.0a1/README.md
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-01-26 00:49:46.725671 Plone-6.1.0a1/docs/
--rw-r--r--   0 maurits    (501) staff       (20)     6320 2024-01-26 00:49:46.000000 Plone-6.1.0a1/docs/CREDITS.txt
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2024-01-26 00:49:46.000000 Plone-6.1.0a1/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)     2070 2024-01-26 00:49:46.000000 Plone-6.1.0a1/docs/LICENSE.ZPL
--rw-r--r--   0 maurits    (501) staff       (20)      667 2024-01-26 00:49:46.000000 Plone-6.1.0a1/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1538 2024-01-26 00:49:46.000000 Plone-6.1.0a1/docs/UPGRADE.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1619 2024-01-26 00:49:46.727528 Plone-6.1.0a1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)       38 2024-01-26 00:49:46.000000 Plone-6.1.0a1/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:17:28.724643 Plone-6.1.0a2/
+-rw-r--r--   0 maurits    (501) staff       (20)     7109 2024-02-27 16:17:28.000000 Plone-6.1.0a2/CHANGES.md
+-rw-r--r--   0 maurits    (501) staff       (20)       73 2024-02-27 16:17:28.000000 Plone-6.1.0a2/CONTRIBUTING.md
+-rw-r--r--   0 maurits    (501) staff       (20)       24 2024-02-27 16:17:28.000000 Plone-6.1.0a2/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    15320 2024-02-27 16:17:28.724451 Plone-6.1.0a2/PKG-INFO
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:17:28.723622 Plone-6.1.0a2/Plone.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    15320 2024-02-27 16:17:28.000000 Plone-6.1.0a2/Plone.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      324 2024-02-27 16:17:28.000000 Plone-6.1.0a2/Plone.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-02-27 16:17:28.000000 Plone-6.1.0a2/Plone.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-02-27 16:17:28.000000 Plone-6.1.0a2/Plone.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      188 2024-02-27 16:17:28.000000 Plone-6.1.0a2/Plone.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-02-27 16:17:28.000000 Plone-6.1.0a2/Plone.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     6411 2024-02-27 16:17:28.000000 Plone-6.1.0a2/README.md
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:17:28.722990 Plone-6.1.0a2/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)     6320 2024-02-27 16:17:28.000000 Plone-6.1.0a2/docs/CREDITS.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2024-02-27 16:17:28.000000 Plone-6.1.0a2/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)     2070 2024-02-27 16:17:28.000000 Plone-6.1.0a2/docs/LICENSE.ZPL
+-rw-r--r--   0 maurits    (501) staff       (20)      667 2024-02-27 16:17:28.000000 Plone-6.1.0a2/docs/LICENSE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1538 2024-02-27 16:17:28.000000 Plone-6.1.0a2/docs/UPGRADE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1619 2024-02-27 16:17:28.725194 Plone-6.1.0a2/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2024-02-27 16:17:28.000000 Plone-6.1.0a2/setup.py
```

### Comparing `Plone-6.1.0a1/CHANGES.md` & `Plone-6.1.0a2/CHANGES.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 # Changelog
 
+## 6.1.0a2 (2024-02-27)
+
+
+Bug fixes:
+
+- Release 6.1.0a2.
+  [maurits]
+
+
 ## 6.1.0a1 (2024-01-26)
 
 New features:
 
 - Depend on plone.app.discussion here, this makes it an core addon. [jensens]
 
 - Depend on plone.app.multilingual here, this makes it an core addon. [jensens]
```

### Comparing `Plone-6.1.0a1/PKG-INFO` & `Plone-6.1.0a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Plone
-Version: 6.1.0a1
+Version: 6.1.0a2
 Summary: The Plone Content Management System
 Home-page: https://plone.org/
 Author: Plone Foundation
 Author-email: releaseteam@plone.org
 License: GPL version 2
 Project-URL: Homepage, https://plone.org
 Project-URL: Documentation, https://6.docs.plone.org
@@ -184,14 +184,23 @@
 <h2 align="center">
 License
 </h2>
 The project is licensed under the GPLv2.
 
 # Changelog
 
+## 6.1.0a2 (2024-02-27)
+
+
+Bug fixes:
+
+- Release 6.1.0a2.
+  [maurits]
+
+
 ## 6.1.0a1 (2024-01-26)
 
 New features:
 
 - Depend on plone.app.discussion here, this makes it an core addon. [jensens]
 
 - Depend on plone.app.multilingual here, this makes it an core addon. [jensens]
```

### Comparing `Plone-6.1.0a1/Plone.egg-info/PKG-INFO` & `Plone-6.1.0a2/Plone.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Plone
-Version: 6.1.0a1
+Version: 6.1.0a2
 Summary: The Plone Content Management System
 Home-page: https://plone.org/
 Author: Plone Foundation
 Author-email: releaseteam@plone.org
 License: GPL version 2
 Project-URL: Homepage, https://plone.org
 Project-URL: Documentation, https://6.docs.plone.org
@@ -184,14 +184,23 @@
 <h2 align="center">
 License
 </h2>
 The project is licensed under the GPLv2.
 
 # Changelog
 
+## 6.1.0a2 (2024-02-27)
+
+
+Bug fixes:
+
+- Release 6.1.0a2.
+  [maurits]
+
+
 ## 6.1.0a1 (2024-01-26)
 
 New features:
 
 - Depend on plone.app.discussion here, this makes it an core addon. [jensens]
 
 - Depend on plone.app.multilingual here, this makes it an core addon. [jensens]
```

### Comparing `Plone-6.1.0a1/README.md` & `Plone-6.1.0a2/README.md`

 * *Files identical despite different names*

### Comparing `Plone-6.1.0a1/docs/CREDITS.txt` & `Plone-6.1.0a2/docs/CREDITS.txt`

 * *Files identical despite different names*

### Comparing `Plone-6.1.0a1/docs/LICENSE.GPL` & `Plone-6.1.0a2/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `Plone-6.1.0a1/docs/LICENSE.ZPL` & `Plone-6.1.0a2/docs/LICENSE.ZPL`

 * *Files identical despite different names*

### Comparing `Plone-6.1.0a1/docs/LICENSE.txt` & `Plone-6.1.0a2/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Plone-6.1.0a1/docs/UPGRADE.txt` & `Plone-6.1.0a2/docs/UPGRADE.txt`

 * *Files identical despite different names*

### Comparing `Plone-6.1.0a1/setup.cfg` & `Plone-6.1.0a2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 6.1.0a1
+version = 6.1.0a2
 name = Plone
 description = The Plone Content Management System
 long_description = file: README.md, CHANGES.md
 long_description_content_type = text/markdown
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Environment :: Web Environment
```

