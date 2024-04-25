# Comparing `tmp/mongo_m-1.1.1.tar.gz` & `tmp/mongo_m-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongo_m-1.1.1.tar", last modified: Thu Apr 25 09:53:49 2024, max compression
+gzip compressed data, was "mongo_m-1.1.2.tar", last modified: Thu Apr 25 10:00:52 2024, max compression
```

## Comparing `mongo_m-1.1.1.tar` & `mongo_m-1.1.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 09:53:49.332117 mongo_m-1.1.1/
--rw-rw-rw-   0        0        0     1560 2024-04-25 09:53:49.332117 mongo_m-1.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-25 09:53:49.313652 mongo_m-1.1.1/mongo_m/
--rw-rw-rw-   0        0        0        0 2024-04-22 13:51:52.000000 mongo_m-1.1.1/mongo_m/__init__.py
--rw-rw-rw-   0        0        0     3300 2024-04-25 08:49:07.000000 mongo_m-1.1.1/mongo_m/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 09:53:49.325699 mongo_m-1.1.1/mongo_m/core/
--rw-rw-rw-   0        0        0       99 2024-04-23 16:31:26.000000 mongo_m-1.1.1/mongo_m/core/__init__.py
--rw-rw-rw-   0        0        0      511 2024-04-22 14:19:36.000000 mongo_m-1.1.1/mongo_m/core/creator.py
--rw-rw-rw-   0        0        0      602 2024-04-25 05:23:36.000000 mongo_m-1.1.1/mongo_m/core/ini_file.py
--rw-rw-rw-   0        0        0     3164 2024-04-25 08:55:17.000000 mongo_m-1.1.1/mongo_m/core/inspect_module.py
--rw-rw-rw-   0        0        0      764 2024-04-15 10:37:27.000000 mongo_m-1.1.1/mongo_m/core/mongodb.py
--rw-rw-rw-   0        0        0      487 2024-04-25 06:48:57.000000 mongo_m-1.1.1/mongo_m/core/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-25 09:53:49.326700 mongo_m-1.1.1/mongo_m/repository/
--rw-rw-rw-   0        0        0        0 2024-04-22 12:24:01.000000 mongo_m-1.1.1/mongo_m/repository/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 09:53:49.327699 mongo_m-1.1.1/mongo_m/repository/collections/
--rw-rw-rw-   0        0        0       28 2024-04-15 10:26:39.000000 mongo_m-1.1.1/mongo_m/repository/collections/__init__.py
--rw-rw-rw-   0        0        0      805 2024-04-25 05:23:36.000000 mongo_m-1.1.1/mongo_m/repository/collections/collections.py
--rw-rw-rw-   0        0        0      490 2024-04-25 05:23:36.000000 mongo_m-1.1.1/mongo_m/repository/collections/models.py
--rw-rw-rw-   0        0        0      938 2024-04-22 10:42:33.000000 mongo_m-1.1.1/mongo_m/repository/collections/query.py
-drwxrwxrwx   0        0        0        0 2024-04-25 09:53:49.328699 mongo_m-1.1.1/mongo_m/services/
--rw-rw-rw-   0        0        0        0 2024-04-22 12:24:10.000000 mongo_m-1.1.1/mongo_m/services/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 09:53:49.330102 mongo_m-1.1.1/mongo_m/services/migration/
--rw-rw-rw-   0        0        0       47 2024-04-25 05:23:36.000000 mongo_m-1.1.1/mongo_m/services/migration/__init__.py
--rw-rw-rw-   0        0        0     2770 2024-04-25 08:49:49.000000 mongo_m-1.1.1/mongo_m/services/migration/file.py
--rw-rw-rw-   0        0        0     1672 2024-04-25 05:56:57.000000 mongo_m-1.1.1/mongo_m/services/migration/migration.py
-drwxrwxrwx   0        0        0        0 2024-04-25 09:53:49.330102 mongo_m-1.1.1/mongo_m.egg-info/
--rw-rw-rw-   0        0        0     1560 2024-04-25 09:53:49.000000 mongo_m-1.1.1/mongo_m.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      745 2024-04-25 09:53:49.000000 mongo_m-1.1.1/mongo_m.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 09:53:49.000000 mongo_m-1.1.1/mongo_m.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-25 09:52:24.000000 mongo_m-1.1.1/mongo_m.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      185 2024-04-25 09:53:49.000000 mongo_m-1.1.1/mongo_m.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-25 09:53:49.000000 mongo_m-1.1.1/mongo_m.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 09:53:49.332117 mongo_m-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1922 2024-04-25 09:53:18.000000 mongo_m-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 09:53:49.330102 mongo_m-1.1.1/tests/
--rw-rw-rw-   0        0        0        0 2024-04-22 12:21:08.000000 mongo_m-1.1.1/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 10:00:52.635805 mongo_m-1.1.2/
+-rw-rw-rw-   0        0        0     1560 2024-04-25 10:00:52.634883 mongo_m-1.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-25 10:00:52.608835 mongo_m-1.1.2/mongo_m/
+-rw-rw-rw-   0        0        0        0 2024-04-22 13:51:52.000000 mongo_m-1.1.2/mongo_m/__init__.py
+-rw-rw-rw-   0        0        0     2373 2024-04-25 09:59:55.000000 mongo_m-1.1.2/mongo_m/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 10:00:52.628746 mongo_m-1.1.2/mongo_m/core/
+-rw-rw-rw-   0        0        0       99 2024-04-23 16:31:26.000000 mongo_m-1.1.2/mongo_m/core/__init__.py
+-rw-rw-rw-   0        0        0      511 2024-04-22 14:19:36.000000 mongo_m-1.1.2/mongo_m/core/creator.py
+-rw-rw-rw-   0        0        0      602 2024-04-25 05:23:36.000000 mongo_m-1.1.2/mongo_m/core/ini_file.py
+-rw-rw-rw-   0        0        0     3164 2024-04-25 10:00:11.000000 mongo_m-1.1.2/mongo_m/core/inspect_module.py
+-rw-rw-rw-   0        0        0      764 2024-04-15 10:37:27.000000 mongo_m-1.1.2/mongo_m/core/mongodb.py
+-rw-rw-rw-   0        0        0      487 2024-04-25 06:48:57.000000 mongo_m-1.1.2/mongo_m/core/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-25 10:00:52.629747 mongo_m-1.1.2/mongo_m/repository/
+-rw-rw-rw-   0        0        0        0 2024-04-22 12:24:01.000000 mongo_m-1.1.2/mongo_m/repository/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 10:00:52.631746 mongo_m-1.1.2/mongo_m/repository/collections/
+-rw-rw-rw-   0        0        0       28 2024-04-15 10:26:39.000000 mongo_m-1.1.2/mongo_m/repository/collections/__init__.py
+-rw-rw-rw-   0        0        0      805 2024-04-25 05:23:36.000000 mongo_m-1.1.2/mongo_m/repository/collections/collections.py
+-rw-rw-rw-   0        0        0      490 2024-04-25 05:23:36.000000 mongo_m-1.1.2/mongo_m/repository/collections/models.py
+-rw-rw-rw-   0        0        0      938 2024-04-22 10:42:33.000000 mongo_m-1.1.2/mongo_m/repository/collections/query.py
+drwxrwxrwx   0        0        0        0 2024-04-25 10:00:52.631746 mongo_m-1.1.2/mongo_m/services/
+-rw-rw-rw-   0        0        0        0 2024-04-22 12:24:10.000000 mongo_m-1.1.2/mongo_m/services/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 10:00:52.633747 mongo_m-1.1.2/mongo_m/services/migration/
+-rw-rw-rw-   0        0        0       47 2024-04-25 05:23:36.000000 mongo_m-1.1.2/mongo_m/services/migration/__init__.py
+-rw-rw-rw-   0        0        0     2770 2024-04-25 08:49:49.000000 mongo_m-1.1.2/mongo_m/services/migration/file.py
+-rw-rw-rw-   0        0        0     1672 2024-04-25 05:56:57.000000 mongo_m-1.1.2/mongo_m/services/migration/migration.py
+drwxrwxrwx   0        0        0        0 2024-04-25 10:00:52.634746 mongo_m-1.1.2/mongo_m.egg-info/
+-rw-rw-rw-   0        0        0     1560 2024-04-25 10:00:52.000000 mongo_m-1.1.2/mongo_m.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      745 2024-04-25 10:00:52.000000 mongo_m-1.1.2/mongo_m.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 10:00:52.000000 mongo_m-1.1.2/mongo_m.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-25 10:00:52.000000 mongo_m-1.1.2/mongo_m.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      185 2024-04-25 10:00:52.000000 mongo_m-1.1.2/mongo_m.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-25 10:00:52.000000 mongo_m-1.1.2/mongo_m.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 10:00:52.635805 mongo_m-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1922 2024-04-25 10:00:23.000000 mongo_m-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 10:00:52.633747 mongo_m-1.1.2/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-22 12:21:08.000000 mongo_m-1.1.2/tests/__init__.py
```

### Comparing `mongo_m-1.1.1/PKG-INFO` & `mongo_m-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongo_m
-Version: 1.1.1
+Version: 1.1.2
 Summary: A database migration tool for MongoDB
 Home-page: https://github.com/BeyonD311/mongo-m
 Author: Dankov Sergey
 Author-email: beyond31@mail.ru
 License: GNU General Public License v3 (GPLv3)
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mongo_m-1.1.1/mongo_m/core/ini_file.py` & `mongo_m-1.1.2/mongo_m/core/ini_file.py`

 * *Files identical despite different names*

### Comparing `mongo_m-1.1.1/mongo_m/core/inspect_module.py` & `mongo_m-1.1.2/mongo_m/core/inspect_module.py`

 * *Files identical despite different names*

### Comparing `mongo_m-1.1.1/mongo_m/core/mongodb.py` & `mongo_m-1.1.2/mongo_m/core/mongodb.py`

 * *Files identical despite different names*

### Comparing `mongo_m-1.1.1/mongo_m/repository/collections/collections.py` & `mongo_m-1.1.2/mongo_m/repository/collections/collections.py`

 * *Files identical despite different names*

### Comparing `mongo_m-1.1.1/mongo_m/repository/collections/query.py` & `mongo_m-1.1.2/mongo_m/repository/collections/query.py`

 * *Files identical despite different names*

### Comparing `mongo_m-1.1.1/mongo_m/services/migration/file.py` & `mongo_m-1.1.2/mongo_m/services/migration/file.py`

 * *Files identical despite different names*

### Comparing `mongo_m-1.1.1/mongo_m/services/migration/migration.py` & `mongo_m-1.1.2/mongo_m/services/migration/migration.py`

 * *Files identical despite different names*

### Comparing `mongo_m-1.1.1/mongo_m.egg-info/PKG-INFO` & `mongo_m-1.1.2/mongo_m.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongo_m
-Version: 1.1.1
+Version: 1.1.2
 Summary: A database migration tool for MongoDB
 Home-page: https://github.com/BeyonD311/mongo-m
 Author: Dankov Sergey
 Author-email: beyond31@mail.ru
 License: GNU General Public License v3 (GPLv3)
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mongo_m-1.1.1/mongo_m.egg-info/SOURCES.txt` & `mongo_m-1.1.2/mongo_m.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mongo_m-1.1.1/setup.py` & `mongo_m-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         with open('README.md') as f:
             return f.read()
     except IOError:
         return DESCRIPTION
 
 setup(
     name='mongo_m',
-    version='1.1.1',
+    version='1.1.2',
     description=DESCRIPTION,
     long_description=get_read_me(),
     long_description_content_type="text/markdown",
     author='Dankov Sergey',
     author_email='beyond31@mail.ru',
     license='GNU General Public License v3 (GPLv3)',
     url='https://github.com/BeyonD311/mongo-m',
```

