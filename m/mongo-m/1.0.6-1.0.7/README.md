# Comparing `tmp/mongo_m-1.0.6.tar.gz` & `tmp/mongo_m-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongo_m-1.0.6.tar", last modified: Thu Apr 25 07:06:42 2024, max compression
+gzip compressed data, was "mongo_m-1.0.7.tar", last modified: Thu Apr 25 07:23:26 2024, max compression
```

## Comparing `mongo_m-1.0.6.tar` & `mongo_m-1.0.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 07:06:42.446007 mongo_m-1.0.6/
--rw-rw-rw-   0        0        0     1560 2024-04-25 07:06:42.446007 mongo_m-1.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-25 07:06:42.419071 mongo_m-1.0.6/mongo_m/
--rw-rw-rw-   0        0        0        0 2024-04-22 13:51:52.000000 mongo_m-1.0.6/mongo_m/__init__.py
--rw-rw-rw-   0        0        0     3254 2024-04-25 06:02:36.000000 mongo_m-1.0.6/mongo_m/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 07:06:42.439779 mongo_m-1.0.6/mongo_m/core/
--rw-rw-rw-   0        0        0       99 2024-04-23 16:31:26.000000 mongo_m-1.0.6/mongo_m/core/__init__.py
--rw-rw-rw-   0        0        0      511 2024-04-22 14:19:36.000000 mongo_m-1.0.6/mongo_m/core/creator.py
--rw-rw-rw-   0        0        0      602 2024-04-25 05:23:36.000000 mongo_m-1.0.6/mongo_m/core/ini_file.py
--rw-rw-rw-   0        0        0     2960 2024-04-25 07:01:18.000000 mongo_m-1.0.6/mongo_m/core/inspect_module.py
--rw-rw-rw-   0        0        0      764 2024-04-15 10:37:27.000000 mongo_m-1.0.6/mongo_m/core/mongodb.py
--rw-rw-rw-   0        0        0      487 2024-04-25 06:48:57.000000 mongo_m-1.0.6/mongo_m/core/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-25 07:06:42.439779 mongo_m-1.0.6/mongo_m/repository/
--rw-rw-rw-   0        0        0        0 2024-04-22 12:24:01.000000 mongo_m-1.0.6/mongo_m/repository/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 07:06:42.441779 mongo_m-1.0.6/mongo_m/repository/collections/
--rw-rw-rw-   0        0        0       28 2024-04-15 10:26:39.000000 mongo_m-1.0.6/mongo_m/repository/collections/__init__.py
--rw-rw-rw-   0        0        0      805 2024-04-25 05:23:36.000000 mongo_m-1.0.6/mongo_m/repository/collections/collections.py
--rw-rw-rw-   0        0        0      490 2024-04-25 05:23:36.000000 mongo_m-1.0.6/mongo_m/repository/collections/models.py
--rw-rw-rw-   0        0        0      938 2024-04-22 10:42:33.000000 mongo_m-1.0.6/mongo_m/repository/collections/query.py
-drwxrwxrwx   0        0        0        0 2024-04-25 07:06:42.442778 mongo_m-1.0.6/mongo_m/services/
--rw-rw-rw-   0        0        0        0 2024-04-22 12:24:10.000000 mongo_m-1.0.6/mongo_m/services/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 07:06:42.443640 mongo_m-1.0.6/mongo_m/services/migration/
--rw-rw-rw-   0        0        0       47 2024-04-25 05:23:36.000000 mongo_m-1.0.6/mongo_m/services/migration/__init__.py
--rw-rw-rw-   0        0        0     2643 2024-04-25 05:56:57.000000 mongo_m-1.0.6/mongo_m/services/migration/file.py
--rw-rw-rw-   0        0        0     1672 2024-04-25 05:56:57.000000 mongo_m-1.0.6/mongo_m/services/migration/migration.py
-drwxrwxrwx   0        0        0        0 2024-04-25 07:06:42.444646 mongo_m-1.0.6/mongo_m.egg-info/
--rw-rw-rw-   0        0        0     1560 2024-04-25 07:06:42.000000 mongo_m-1.0.6/mongo_m.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      745 2024-04-25 07:06:42.000000 mongo_m-1.0.6/mongo_m.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 07:06:42.000000 mongo_m-1.0.6/mongo_m.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-25 07:06:42.000000 mongo_m-1.0.6/mongo_m.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      185 2024-04-25 07:06:42.000000 mongo_m-1.0.6/mongo_m.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-25 07:06:42.000000 mongo_m-1.0.6/mongo_m.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 07:06:42.446007 mongo_m-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1922 2024-04-25 07:06:41.000000 mongo_m-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 07:06:42.444646 mongo_m-1.0.6/tests/
--rw-rw-rw-   0        0        0        0 2024-04-22 12:21:08.000000 mongo_m-1.0.6/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 07:23:26.114513 mongo_m-1.0.7/
+-rw-rw-rw-   0        0        0     1560 2024-04-25 07:23:26.114513 mongo_m-1.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-25 07:23:26.089952 mongo_m-1.0.7/mongo_m/
+-rw-rw-rw-   0        0        0        0 2024-04-22 13:51:52.000000 mongo_m-1.0.7/mongo_m/__init__.py
+-rw-rw-rw-   0        0        0     3254 2024-04-25 06:02:36.000000 mongo_m-1.0.7/mongo_m/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 07:23:26.107833 mongo_m-1.0.7/mongo_m/core/
+-rw-rw-rw-   0        0        0       99 2024-04-23 16:31:26.000000 mongo_m-1.0.7/mongo_m/core/__init__.py
+-rw-rw-rw-   0        0        0      511 2024-04-22 14:19:36.000000 mongo_m-1.0.7/mongo_m/core/creator.py
+-rw-rw-rw-   0        0        0      602 2024-04-25 05:23:36.000000 mongo_m-1.0.7/mongo_m/core/ini_file.py
+-rw-rw-rw-   0        0        0     2960 2024-04-25 07:01:18.000000 mongo_m-1.0.7/mongo_m/core/inspect_module.py
+-rw-rw-rw-   0        0        0      764 2024-04-15 10:37:27.000000 mongo_m-1.0.7/mongo_m/core/mongodb.py
+-rw-rw-rw-   0        0        0      487 2024-04-25 06:48:57.000000 mongo_m-1.0.7/mongo_m/core/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-25 07:23:26.109310 mongo_m-1.0.7/mongo_m/repository/
+-rw-rw-rw-   0        0        0        0 2024-04-22 12:24:01.000000 mongo_m-1.0.7/mongo_m/repository/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 07:23:26.111320 mongo_m-1.0.7/mongo_m/repository/collections/
+-rw-rw-rw-   0        0        0       28 2024-04-15 10:26:39.000000 mongo_m-1.0.7/mongo_m/repository/collections/__init__.py
+-rw-rw-rw-   0        0        0      805 2024-04-25 05:23:36.000000 mongo_m-1.0.7/mongo_m/repository/collections/collections.py
+-rw-rw-rw-   0        0        0      490 2024-04-25 05:23:36.000000 mongo_m-1.0.7/mongo_m/repository/collections/models.py
+-rw-rw-rw-   0        0        0      938 2024-04-22 10:42:33.000000 mongo_m-1.0.7/mongo_m/repository/collections/query.py
+drwxrwxrwx   0        0        0        0 2024-04-25 07:23:26.111320 mongo_m-1.0.7/mongo_m/services/
+-rw-rw-rw-   0        0        0        0 2024-04-22 12:24:10.000000 mongo_m-1.0.7/mongo_m/services/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 07:23:26.113214 mongo_m-1.0.7/mongo_m/services/migration/
+-rw-rw-rw-   0        0        0       47 2024-04-25 05:23:36.000000 mongo_m-1.0.7/mongo_m/services/migration/__init__.py
+-rw-rw-rw-   0        0        0     2770 2024-04-25 07:20:32.000000 mongo_m-1.0.7/mongo_m/services/migration/file.py
+-rw-rw-rw-   0        0        0     1672 2024-04-25 05:56:57.000000 mongo_m-1.0.7/mongo_m/services/migration/migration.py
+drwxrwxrwx   0        0        0        0 2024-04-25 07:23:26.113214 mongo_m-1.0.7/mongo_m.egg-info/
+-rw-rw-rw-   0        0        0     1560 2024-04-25 07:23:26.000000 mongo_m-1.0.7/mongo_m.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      745 2024-04-25 07:23:26.000000 mongo_m-1.0.7/mongo_m.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 07:23:26.000000 mongo_m-1.0.7/mongo_m.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-25 07:23:26.000000 mongo_m-1.0.7/mongo_m.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      185 2024-04-25 07:23:26.000000 mongo_m-1.0.7/mongo_m.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-25 07:23:26.000000 mongo_m-1.0.7/mongo_m.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 07:23:26.114513 mongo_m-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1922 2024-04-25 07:23:17.000000 mongo_m-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 07:23:26.113214 mongo_m-1.0.7/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-22 12:21:08.000000 mongo_m-1.0.7/tests/__init__.py
```

### Comparing `mongo_m-1.0.6/PKG-INFO` & `mongo_m-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongo_m
-Version: 1.0.6
+Version: 1.0.7
 Summary: A database migration tool for MongoDB
 Home-page: https://github.com/BeyonD311/mongo-m
 Author: Dankov Sergey
 Author-email: beyond31@mail.ru
 License: GNU General Public License v3 (GPLv3)
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mongo_m-1.0.6/mongo_m/__main__.py` & `mongo_m-1.0.7/mongo_m/__main__.py`

 * *Files identical despite different names*

### Comparing `mongo_m-1.0.6/mongo_m/core/ini_file.py` & `mongo_m-1.0.7/mongo_m/core/ini_file.py`

 * *Files identical despite different names*

### Comparing `mongo_m-1.0.6/mongo_m/core/inspect_module.py` & `mongo_m-1.0.7/mongo_m/core/inspect_module.py`

 * *Files identical despite different names*

### Comparing `mongo_m-1.0.6/mongo_m/core/mongodb.py` & `mongo_m-1.0.7/mongo_m/core/mongodb.py`

 * *Files identical despite different names*

### Comparing `mongo_m-1.0.6/mongo_m/repository/collections/collections.py` & `mongo_m-1.0.7/mongo_m/repository/collections/collections.py`

 * *Files identical despite different names*

### Comparing `mongo_m-1.0.6/mongo_m/repository/collections/query.py` & `mongo_m-1.0.7/mongo_m/repository/collections/query.py`

 * *Files identical despite different names*

### Comparing `mongo_m-1.0.6/mongo_m/services/migration/file.py` & `mongo_m-1.0.7/mongo_m/services/migration/file.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,20 +14,23 @@
     @classmethod
     def create_migration_catalog(cls):
         if not check_catalog(cls.PATH_MIGRATION.name):
             create_catalog(cls.PATH_MIGRATION.name)
 
     @classmethod
     async def make_migration(cls, module_path: str):
-        modules = []
+        modules = {}
         async for module in make_module(module_path):
             module = inspect_module(module)
             if module != {}:
-                modules.append(module)
-        modules = json.dumps(modules, indent=4)
+                for name, value in module.items():
+                    modules[name] = {
+                        name: value,
+                    }
+        modules = json.dumps(list(modules.values()), indent=4)
         hash_name = hashlib.md5(modules.encode())
         file_name = f"{hash_name.hexdigest()}.json"
         with open(file=f"{cls.PATH_MIGRATION}/{file_name}", mode='w') as f:
             f.write(modules)
         return file_name
 
     @classmethod
```

### Comparing `mongo_m-1.0.6/mongo_m/services/migration/migration.py` & `mongo_m-1.0.7/mongo_m/services/migration/migration.py`

 * *Files identical despite different names*

### Comparing `mongo_m-1.0.6/mongo_m.egg-info/PKG-INFO` & `mongo_m-1.0.7/mongo_m.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongo_m
-Version: 1.0.6
+Version: 1.0.7
 Summary: A database migration tool for MongoDB
 Home-page: https://github.com/BeyonD311/mongo-m
 Author: Dankov Sergey
 Author-email: beyond31@mail.ru
 License: GNU General Public License v3 (GPLv3)
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mongo_m-1.0.6/mongo_m.egg-info/SOURCES.txt` & `mongo_m-1.0.7/mongo_m.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mongo_m-1.0.6/setup.py` & `mongo_m-1.0.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         with open('README.md') as f:
             return f.read()
     except IOError:
         return DESCRIPTION
 
 setup(
     name='mongo_m',
-    version='1.0.6',
+    version='1.0.7',
     description=DESCRIPTION,
     long_description=get_read_me(),
     long_description_content_type="text/markdown",
     author='Dankov Sergey',
     author_email='beyond31@mail.ru',
     license='GNU General Public License v3 (GPLv3)',
     url='https://github.com/BeyonD311/mongo-m',
```

