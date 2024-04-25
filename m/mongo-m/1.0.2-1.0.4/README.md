# Comparing `tmp/mongo_m-1.0.2.tar.gz` & `tmp/mongo_m-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongo_m-1.0.2.tar", last modified: Thu Apr 25 05:58:03 2024, max compression
+gzip compressed data, was "mongo_m-1.0.4.tar", last modified: Thu Apr 25 06:25:04 2024, max compression
```

## Comparing `mongo_m-1.0.2.tar` & `mongo_m-1.0.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 05:58:03.755687 mongo_m-1.0.2/
--rw-rw-rw-   0        0        0     1560 2024-04-25 05:58:03.754664 mongo_m-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-25 05:58:03.715026 mongo_m-1.0.2/mongo_m/
--rw-rw-rw-   0        0        0        0 2024-04-22 13:51:52.000000 mongo_m-1.0.2/mongo_m/__init__.py
--rw-rw-rw-   0        0        0     3195 2024-04-25 05:23:36.000000 mongo_m-1.0.2/mongo_m/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 05:58:03.737345 mongo_m-1.0.2/mongo_m/core/
--rw-rw-rw-   0        0        0       99 2024-04-23 16:31:26.000000 mongo_m-1.0.2/mongo_m/core/__init__.py
--rw-rw-rw-   0        0        0      511 2024-04-22 14:19:36.000000 mongo_m-1.0.2/mongo_m/core/creator.py
--rw-rw-rw-   0        0        0      602 2024-04-25 05:23:36.000000 mongo_m-1.0.2/mongo_m/core/ini_file.py
--rw-rw-rw-   0        0        0     2747 2024-04-23 16:31:26.000000 mongo_m-1.0.2/mongo_m/core/inspect_module.py
--rw-rw-rw-   0        0        0      764 2024-04-15 10:37:27.000000 mongo_m-1.0.2/mongo_m/core/mongodb.py
--rw-rw-rw-   0        0        0      452 2024-04-23 16:31:26.000000 mongo_m-1.0.2/mongo_m/core/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-25 05:58:03.739353 mongo_m-1.0.2/mongo_m/repository/
--rw-rw-rw-   0        0        0        0 2024-04-22 12:24:01.000000 mongo_m-1.0.2/mongo_m/repository/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 05:58:03.744517 mongo_m-1.0.2/mongo_m/repository/collections/
--rw-rw-rw-   0        0        0       28 2024-04-15 10:26:39.000000 mongo_m-1.0.2/mongo_m/repository/collections/__init__.py
--rw-rw-rw-   0        0        0      805 2024-04-25 05:23:36.000000 mongo_m-1.0.2/mongo_m/repository/collections/collections.py
--rw-rw-rw-   0        0        0      490 2024-04-25 05:23:36.000000 mongo_m-1.0.2/mongo_m/repository/collections/models.py
--rw-rw-rw-   0        0        0      938 2024-04-22 10:42:33.000000 mongo_m-1.0.2/mongo_m/repository/collections/query.py
-drwxrwxrwx   0        0        0        0 2024-04-25 05:58:03.745537 mongo_m-1.0.2/mongo_m/services/
--rw-rw-rw-   0        0        0        0 2024-04-22 12:24:10.000000 mongo_m-1.0.2/mongo_m/services/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 05:58:03.748544 mongo_m-1.0.2/mongo_m/services/migration/
--rw-rw-rw-   0        0        0       47 2024-04-25 05:23:36.000000 mongo_m-1.0.2/mongo_m/services/migration/__init__.py
--rw-rw-rw-   0        0        0     2643 2024-04-25 05:56:57.000000 mongo_m-1.0.2/mongo_m/services/migration/file.py
--rw-rw-rw-   0        0        0     1672 2024-04-25 05:56:57.000000 mongo_m-1.0.2/mongo_m/services/migration/migration.py
-drwxrwxrwx   0        0        0        0 2024-04-25 05:58:03.753544 mongo_m-1.0.2/mongo_m.egg-info/
--rw-rw-rw-   0        0        0     1560 2024-04-25 05:58:03.000000 mongo_m-1.0.2/mongo_m.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      745 2024-04-25 05:58:03.000000 mongo_m-1.0.2/mongo_m.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 05:58:03.000000 mongo_m-1.0.2/mongo_m.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-25 05:58:03.000000 mongo_m-1.0.2/mongo_m.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      185 2024-04-25 05:58:03.000000 mongo_m-1.0.2/mongo_m.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-25 05:58:03.000000 mongo_m-1.0.2/mongo_m.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 05:58:03.756696 mongo_m-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1922 2024-04-25 05:57:34.000000 mongo_m-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 05:58:03.749544 mongo_m-1.0.2/tests/
--rw-rw-rw-   0        0        0        0 2024-04-22 12:21:08.000000 mongo_m-1.0.2/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 06:25:04.814534 mongo_m-1.0.4/
+-rw-rw-rw-   0        0        0     1560 2024-04-25 06:25:04.814534 mongo_m-1.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-25 06:25:04.789006 mongo_m-1.0.4/mongo_m/
+-rw-rw-rw-   0        0        0        0 2024-04-22 13:51:52.000000 mongo_m-1.0.4/mongo_m/__init__.py
+-rw-rw-rw-   0        0        0     3254 2024-04-25 06:02:36.000000 mongo_m-1.0.4/mongo_m/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 06:25:04.807439 mongo_m-1.0.4/mongo_m/core/
+-rw-rw-rw-   0        0        0       99 2024-04-23 16:31:26.000000 mongo_m-1.0.4/mongo_m/core/__init__.py
+-rw-rw-rw-   0        0        0      511 2024-04-22 14:19:36.000000 mongo_m-1.0.4/mongo_m/core/creator.py
+-rw-rw-rw-   0        0        0      602 2024-04-25 05:23:36.000000 mongo_m-1.0.4/mongo_m/core/ini_file.py
+-rw-rw-rw-   0        0        0     2785 2024-04-25 06:23:11.000000 mongo_m-1.0.4/mongo_m/core/inspect_module.py
+-rw-rw-rw-   0        0        0      764 2024-04-15 10:37:27.000000 mongo_m-1.0.4/mongo_m/core/mongodb.py
+-rw-rw-rw-   0        0        0      452 2024-04-23 16:31:26.000000 mongo_m-1.0.4/mongo_m/core/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-25 06:25:04.807439 mongo_m-1.0.4/mongo_m/repository/
+-rw-rw-rw-   0        0        0        0 2024-04-22 12:24:01.000000 mongo_m-1.0.4/mongo_m/repository/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 06:25:04.810777 mongo_m-1.0.4/mongo_m/repository/collections/
+-rw-rw-rw-   0        0        0       28 2024-04-15 10:26:39.000000 mongo_m-1.0.4/mongo_m/repository/collections/__init__.py
+-rw-rw-rw-   0        0        0      805 2024-04-25 05:23:36.000000 mongo_m-1.0.4/mongo_m/repository/collections/collections.py
+-rw-rw-rw-   0        0        0      490 2024-04-25 05:23:36.000000 mongo_m-1.0.4/mongo_m/repository/collections/models.py
+-rw-rw-rw-   0        0        0      938 2024-04-22 10:42:33.000000 mongo_m-1.0.4/mongo_m/repository/collections/query.py
+drwxrwxrwx   0        0        0        0 2024-04-25 06:25:04.810777 mongo_m-1.0.4/mongo_m/services/
+-rw-rw-rw-   0        0        0        0 2024-04-22 12:24:10.000000 mongo_m-1.0.4/mongo_m/services/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 06:25:04.811961 mongo_m-1.0.4/mongo_m/services/migration/
+-rw-rw-rw-   0        0        0       47 2024-04-25 05:23:36.000000 mongo_m-1.0.4/mongo_m/services/migration/__init__.py
+-rw-rw-rw-   0        0        0     2643 2024-04-25 05:56:57.000000 mongo_m-1.0.4/mongo_m/services/migration/file.py
+-rw-rw-rw-   0        0        0     1672 2024-04-25 05:56:57.000000 mongo_m-1.0.4/mongo_m/services/migration/migration.py
+drwxrwxrwx   0        0        0        0 2024-04-25 06:25:04.813403 mongo_m-1.0.4/mongo_m.egg-info/
+-rw-rw-rw-   0        0        0     1560 2024-04-25 06:25:04.000000 mongo_m-1.0.4/mongo_m.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      745 2024-04-25 06:25:04.000000 mongo_m-1.0.4/mongo_m.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 06:25:04.000000 mongo_m-1.0.4/mongo_m.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-25 06:25:04.000000 mongo_m-1.0.4/mongo_m.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      185 2024-04-25 06:25:04.000000 mongo_m-1.0.4/mongo_m.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-25 06:25:04.000000 mongo_m-1.0.4/mongo_m.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 06:25:04.814534 mongo_m-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1922 2024-04-25 06:25:03.000000 mongo_m-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 06:25:04.811961 mongo_m-1.0.4/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-22 12:21:08.000000 mongo_m-1.0.4/tests/__init__.py
```

### Comparing `mongo_m-1.0.2/PKG-INFO` & `mongo_m-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongo_m
-Version: 1.0.2
+Version: 1.0.4
 Summary: A database migration tool for MongoDB
 Home-page: https://github.com/BeyonD311/mongo-m
 Author: Dankov Sergey
 Author-email: beyond31@mail.ru
 License: GNU General Public License v3 (GPLv3)
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mongo_m-1.0.2/mongo_m/__main__.py` & `mongo_m-1.0.4/mongo_m/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,27 +42,29 @@
     module_path = config.get("MONGO", "module_path")
     migration_file = await FileMigration.make_migration(module_path)
     FileMigration.update_migration_file(migration_file)
 
 
 async def main():
     FileMigration.create_migration_catalog()
-    client = connect_to_mongo()
     params = tuple(sys.argv[1:])
     # module_path = "app/src/app/schemes"
     # module_path = "utils/schemas/db_schemas_q_service"
+    client = None
     try:
         if params[0] == "--create-migration":
             await create_migration()
         elif params[0] == "--update-migration":
+            client = connect_to_mongo()
             await update_migration(client)
         elif params[0] == "--init":
             create_file_ini()
     finally:
-        client.close()
+        if client != None:
+            client.close()
     # for collection in db_collections:
     #     if collection.name == "text_queue":
     #         for field in collection.fields:
     #             print(collection.name, field.name, field.type)
     # find_collection = list(filter(lambda x: x.name in {"customer_request"}, db_collections))
     # query = {
     #     "$or": [{field.name: {"$exists": False}} for field in find_collection[0].fields]
```

### Comparing `mongo_m-1.0.2/mongo_m/core/ini_file.py` & `mongo_m-1.0.4/mongo_m/core/ini_file.py`

 * *Files identical despite different names*

### Comparing `mongo_m-1.0.2/mongo_m/core/inspect_module.py` & `mongo_m-1.0.4/mongo_m/core/inspect_module.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from pathlib import Path
 from .utils import get_default_value
 
 __all__ = ["make_module", "inspect_module", "get_module"]
 
 async def make_module(module_path: str):
     path = f"{os.getcwd()}/{module_path}".replace("\\", "/")
+    print(path, os.path.isdir(path))
     if os.path.isdir(path):
         files = make_module_dir(path, module_path)
     else:
         path_module = module_path.replace("/", ".")
         files = [path_module]
     for name in files:
         try:
```

### Comparing `mongo_m-1.0.2/mongo_m/core/mongodb.py` & `mongo_m-1.0.4/mongo_m/core/mongodb.py`

 * *Files identical despite different names*

### Comparing `mongo_m-1.0.2/mongo_m/repository/collections/collections.py` & `mongo_m-1.0.4/mongo_m/repository/collections/collections.py`

 * *Files identical despite different names*

### Comparing `mongo_m-1.0.2/mongo_m/repository/collections/query.py` & `mongo_m-1.0.4/mongo_m/repository/collections/query.py`

 * *Files identical despite different names*

### Comparing `mongo_m-1.0.2/mongo_m/services/migration/file.py` & `mongo_m-1.0.4/mongo_m/services/migration/file.py`

 * *Files identical despite different names*

### Comparing `mongo_m-1.0.2/mongo_m/services/migration/migration.py` & `mongo_m-1.0.4/mongo_m/services/migration/migration.py`

 * *Files identical despite different names*

### Comparing `mongo_m-1.0.2/mongo_m.egg-info/PKG-INFO` & `mongo_m-1.0.4/mongo_m.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongo_m
-Version: 1.0.2
+Version: 1.0.4
 Summary: A database migration tool for MongoDB
 Home-page: https://github.com/BeyonD311/mongo-m
 Author: Dankov Sergey
 Author-email: beyond31@mail.ru
 License: GNU General Public License v3 (GPLv3)
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mongo_m-1.0.2/mongo_m.egg-info/SOURCES.txt` & `mongo_m-1.0.4/mongo_m.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mongo_m-1.0.2/setup.py` & `mongo_m-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         with open('README.md') as f:
             return f.read()
     except IOError:
         return DESCRIPTION
 
 setup(
     name='mongo_m',
-    version='1.0.2',
+    version='1.0.4',
     description=DESCRIPTION,
     long_description=get_read_me(),
     long_description_content_type="text/markdown",
     author='Dankov Sergey',
     author_email='beyond31@mail.ru',
     license='GNU General Public License v3 (GPLv3)',
     url='https://github.com/BeyonD311/mongo-m',
```

