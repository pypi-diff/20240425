# Comparing `tmp/mongo_m-1.0.4.tar.gz` & `tmp/mongo_m-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongo_m-1.0.4.tar", last modified: Thu Apr 25 06:25:04 2024, max compression
+gzip compressed data, was "mongo_m-1.0.5.tar", last modified: Thu Apr 25 06:49:01 2024, max compression
```

## Comparing `mongo_m-1.0.4.tar` & `mongo_m-1.0.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 06:25:04.814534 mongo_m-1.0.4/
--rw-rw-rw-   0        0        0     1560 2024-04-25 06:25:04.814534 mongo_m-1.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-25 06:25:04.789006 mongo_m-1.0.4/mongo_m/
--rw-rw-rw-   0        0        0        0 2024-04-22 13:51:52.000000 mongo_m-1.0.4/mongo_m/__init__.py
--rw-rw-rw-   0        0        0     3254 2024-04-25 06:02:36.000000 mongo_m-1.0.4/mongo_m/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 06:25:04.807439 mongo_m-1.0.4/mongo_m/core/
--rw-rw-rw-   0        0        0       99 2024-04-23 16:31:26.000000 mongo_m-1.0.4/mongo_m/core/__init__.py
--rw-rw-rw-   0        0        0      511 2024-04-22 14:19:36.000000 mongo_m-1.0.4/mongo_m/core/creator.py
--rw-rw-rw-   0        0        0      602 2024-04-25 05:23:36.000000 mongo_m-1.0.4/mongo_m/core/ini_file.py
--rw-rw-rw-   0        0        0     2785 2024-04-25 06:23:11.000000 mongo_m-1.0.4/mongo_m/core/inspect_module.py
--rw-rw-rw-   0        0        0      764 2024-04-15 10:37:27.000000 mongo_m-1.0.4/mongo_m/core/mongodb.py
--rw-rw-rw-   0        0        0      452 2024-04-23 16:31:26.000000 mongo_m-1.0.4/mongo_m/core/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-25 06:25:04.807439 mongo_m-1.0.4/mongo_m/repository/
--rw-rw-rw-   0        0        0        0 2024-04-22 12:24:01.000000 mongo_m-1.0.4/mongo_m/repository/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 06:25:04.810777 mongo_m-1.0.4/mongo_m/repository/collections/
--rw-rw-rw-   0        0        0       28 2024-04-15 10:26:39.000000 mongo_m-1.0.4/mongo_m/repository/collections/__init__.py
--rw-rw-rw-   0        0        0      805 2024-04-25 05:23:36.000000 mongo_m-1.0.4/mongo_m/repository/collections/collections.py
--rw-rw-rw-   0        0        0      490 2024-04-25 05:23:36.000000 mongo_m-1.0.4/mongo_m/repository/collections/models.py
--rw-rw-rw-   0        0        0      938 2024-04-22 10:42:33.000000 mongo_m-1.0.4/mongo_m/repository/collections/query.py
-drwxrwxrwx   0        0        0        0 2024-04-25 06:25:04.810777 mongo_m-1.0.4/mongo_m/services/
--rw-rw-rw-   0        0        0        0 2024-04-22 12:24:10.000000 mongo_m-1.0.4/mongo_m/services/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 06:25:04.811961 mongo_m-1.0.4/mongo_m/services/migration/
--rw-rw-rw-   0        0        0       47 2024-04-25 05:23:36.000000 mongo_m-1.0.4/mongo_m/services/migration/__init__.py
--rw-rw-rw-   0        0        0     2643 2024-04-25 05:56:57.000000 mongo_m-1.0.4/mongo_m/services/migration/file.py
--rw-rw-rw-   0        0        0     1672 2024-04-25 05:56:57.000000 mongo_m-1.0.4/mongo_m/services/migration/migration.py
-drwxrwxrwx   0        0        0        0 2024-04-25 06:25:04.813403 mongo_m-1.0.4/mongo_m.egg-info/
--rw-rw-rw-   0        0        0     1560 2024-04-25 06:25:04.000000 mongo_m-1.0.4/mongo_m.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      745 2024-04-25 06:25:04.000000 mongo_m-1.0.4/mongo_m.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 06:25:04.000000 mongo_m-1.0.4/mongo_m.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-25 06:25:04.000000 mongo_m-1.0.4/mongo_m.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      185 2024-04-25 06:25:04.000000 mongo_m-1.0.4/mongo_m.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-25 06:25:04.000000 mongo_m-1.0.4/mongo_m.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 06:25:04.814534 mongo_m-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1922 2024-04-25 06:25:03.000000 mongo_m-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 06:25:04.811961 mongo_m-1.0.4/tests/
--rw-rw-rw-   0        0        0        0 2024-04-22 12:21:08.000000 mongo_m-1.0.4/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 06:49:01.712921 mongo_m-1.0.5/
+-rw-rw-rw-   0        0        0     1560 2024-04-25 06:49:01.711921 mongo_m-1.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-25 06:49:01.678515 mongo_m-1.0.5/mongo_m/
+-rw-rw-rw-   0        0        0        0 2024-04-22 13:51:52.000000 mongo_m-1.0.5/mongo_m/__init__.py
+-rw-rw-rw-   0        0        0     3254 2024-04-25 06:02:36.000000 mongo_m-1.0.5/mongo_m/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 06:49:01.704514 mongo_m-1.0.5/mongo_m/core/
+-rw-rw-rw-   0        0        0       99 2024-04-23 16:31:26.000000 mongo_m-1.0.5/mongo_m/core/__init__.py
+-rw-rw-rw-   0        0        0      511 2024-04-22 14:19:36.000000 mongo_m-1.0.5/mongo_m/core/creator.py
+-rw-rw-rw-   0        0        0      602 2024-04-25 05:23:36.000000 mongo_m-1.0.5/mongo_m/core/ini_file.py
+-rw-rw-rw-   0        0        0     2785 2024-04-25 06:23:11.000000 mongo_m-1.0.5/mongo_m/core/inspect_module.py
+-rw-rw-rw-   0        0        0      764 2024-04-15 10:37:27.000000 mongo_m-1.0.5/mongo_m/core/mongodb.py
+-rw-rw-rw-   0        0        0      487 2024-04-25 06:48:57.000000 mongo_m-1.0.5/mongo_m/core/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-25 06:49:01.705514 mongo_m-1.0.5/mongo_m/repository/
+-rw-rw-rw-   0        0        0        0 2024-04-22 12:24:01.000000 mongo_m-1.0.5/mongo_m/repository/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 06:49:01.707922 mongo_m-1.0.5/mongo_m/repository/collections/
+-rw-rw-rw-   0        0        0       28 2024-04-15 10:26:39.000000 mongo_m-1.0.5/mongo_m/repository/collections/__init__.py
+-rw-rw-rw-   0        0        0      805 2024-04-25 05:23:36.000000 mongo_m-1.0.5/mongo_m/repository/collections/collections.py
+-rw-rw-rw-   0        0        0      490 2024-04-25 05:23:36.000000 mongo_m-1.0.5/mongo_m/repository/collections/models.py
+-rw-rw-rw-   0        0        0      938 2024-04-22 10:42:33.000000 mongo_m-1.0.5/mongo_m/repository/collections/query.py
+drwxrwxrwx   0        0        0        0 2024-04-25 06:49:01.707922 mongo_m-1.0.5/mongo_m/services/
+-rw-rw-rw-   0        0        0        0 2024-04-22 12:24:10.000000 mongo_m-1.0.5/mongo_m/services/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 06:49:01.709934 mongo_m-1.0.5/mongo_m/services/migration/
+-rw-rw-rw-   0        0        0       47 2024-04-25 05:23:36.000000 mongo_m-1.0.5/mongo_m/services/migration/__init__.py
+-rw-rw-rw-   0        0        0     2643 2024-04-25 05:56:57.000000 mongo_m-1.0.5/mongo_m/services/migration/file.py
+-rw-rw-rw-   0        0        0     1672 2024-04-25 05:56:57.000000 mongo_m-1.0.5/mongo_m/services/migration/migration.py
+drwxrwxrwx   0        0        0        0 2024-04-25 06:49:01.711921 mongo_m-1.0.5/mongo_m.egg-info/
+-rw-rw-rw-   0        0        0     1560 2024-04-25 06:49:01.000000 mongo_m-1.0.5/mongo_m.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      745 2024-04-25 06:49:01.000000 mongo_m-1.0.5/mongo_m.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 06:49:01.000000 mongo_m-1.0.5/mongo_m.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-25 06:49:01.000000 mongo_m-1.0.5/mongo_m.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      185 2024-04-25 06:49:01.000000 mongo_m-1.0.5/mongo_m.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-25 06:49:01.000000 mongo_m-1.0.5/mongo_m.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 06:49:01.712921 mongo_m-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1922 2024-04-25 06:48:57.000000 mongo_m-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 06:49:01.710923 mongo_m-1.0.5/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-22 12:21:08.000000 mongo_m-1.0.5/tests/__init__.py
```

### Comparing `mongo_m-1.0.4/PKG-INFO` & `mongo_m-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongo_m
-Version: 1.0.4
+Version: 1.0.5
 Summary: A database migration tool for MongoDB
 Home-page: https://github.com/BeyonD311/mongo-m
 Author: Dankov Sergey
 Author-email: beyond31@mail.ru
 License: GNU General Public License v3 (GPLv3)
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mongo_m-1.0.4/mongo_m/__main__.py` & `mongo_m-1.0.5/mongo_m/__main__.py`

 * *Files identical despite different names*

### Comparing `mongo_m-1.0.4/mongo_m/core/ini_file.py` & `mongo_m-1.0.5/mongo_m/core/ini_file.py`

 * *Files identical despite different names*

### Comparing `mongo_m-1.0.4/mongo_m/core/inspect_module.py` & `mongo_m-1.0.5/mongo_m/core/inspect_module.py`

 * *Files identical despite different names*

### Comparing `mongo_m-1.0.4/mongo_m/core/mongodb.py` & `mongo_m-1.0.5/mongo_m/core/mongodb.py`

 * *Files identical despite different names*

### Comparing `mongo_m-1.0.4/mongo_m/repository/collections/collections.py` & `mongo_m-1.0.5/mongo_m/repository/collections/collections.py`

 * *Files identical despite different names*

### Comparing `mongo_m-1.0.4/mongo_m/repository/collections/query.py` & `mongo_m-1.0.5/mongo_m/repository/collections/query.py`

 * *Files identical despite different names*

### Comparing `mongo_m-1.0.4/mongo_m/services/migration/file.py` & `mongo_m-1.0.5/mongo_m/services/migration/file.py`

 * *Files identical despite different names*

### Comparing `mongo_m-1.0.4/mongo_m/services/migration/migration.py` & `mongo_m-1.0.5/mongo_m/services/migration/migration.py`

 * *Files identical despite different names*

### Comparing `mongo_m-1.0.4/mongo_m.egg-info/PKG-INFO` & `mongo_m-1.0.5/mongo_m.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongo_m
-Version: 1.0.4
+Version: 1.0.5
 Summary: A database migration tool for MongoDB
 Home-page: https://github.com/BeyonD311/mongo-m
 Author: Dankov Sergey
 Author-email: beyond31@mail.ru
 License: GNU General Public License v3 (GPLv3)
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mongo_m-1.0.4/mongo_m.egg-info/SOURCES.txt` & `mongo_m-1.0.5/mongo_m.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mongo_m-1.0.4/setup.py` & `mongo_m-1.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         with open('README.md') as f:
             return f.read()
     except IOError:
         return DESCRIPTION
 
 setup(
     name='mongo_m',
-    version='1.0.4',
+    version='1.0.5',
     description=DESCRIPTION,
     long_description=get_read_me(),
     long_description_content_type="text/markdown",
     author='Dankov Sergey',
     author_email='beyond31@mail.ru',
     license='GNU General Public License v3 (GPLv3)',
     url='https://github.com/BeyonD311/mongo-m',
```

