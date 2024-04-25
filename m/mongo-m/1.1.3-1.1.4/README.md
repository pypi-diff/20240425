# Comparing `tmp/mongo_m-1.1.3.tar.gz` & `tmp/mongo_m-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongo_m-1.1.3.tar", last modified: Thu Apr 25 10:26:20 2024, max compression
+gzip compressed data, was "mongo_m-1.1.4.tar", last modified: Thu Apr 25 12:58:19 2024, max compression
```

## Comparing `mongo_m-1.1.3.tar` & `mongo_m-1.1.4.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 10:26:20.218249 mongo_m-1.1.3/
--rw-rw-rw-   0        0        0     1560 2024-04-25 10:26:20.218249 mongo_m-1.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-25 10:26:20.192544 mongo_m-1.1.3/mongo_m/
--rw-rw-rw-   0        0        0        0 2024-04-22 13:51:52.000000 mongo_m-1.1.3/mongo_m/__init__.py
--rw-rw-rw-   0        0        0     2375 2024-04-25 10:24:31.000000 mongo_m-1.1.3/mongo_m/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 10:26:20.208241 mongo_m-1.1.3/mongo_m/core/
--rw-rw-rw-   0        0        0       99 2024-04-23 16:31:26.000000 mongo_m-1.1.3/mongo_m/core/__init__.py
--rw-rw-rw-   0        0        0      511 2024-04-22 14:19:36.000000 mongo_m-1.1.3/mongo_m/core/creator.py
--rw-rw-rw-   0        0        0      602 2024-04-25 05:23:36.000000 mongo_m-1.1.3/mongo_m/core/ini_file.py
--rw-rw-rw-   0        0        0     3164 2024-04-25 10:00:11.000000 mongo_m-1.1.3/mongo_m/core/inspect_module.py
--rw-rw-rw-   0        0        0      764 2024-04-15 10:37:27.000000 mongo_m-1.1.3/mongo_m/core/mongodb.py
--rw-rw-rw-   0        0        0      487 2024-04-25 06:48:57.000000 mongo_m-1.1.3/mongo_m/core/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-25 10:26:20.209249 mongo_m-1.1.3/mongo_m/repository/
--rw-rw-rw-   0        0        0        0 2024-04-22 12:24:01.000000 mongo_m-1.1.3/mongo_m/repository/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 10:26:20.212248 mongo_m-1.1.3/mongo_m/repository/collections/
--rw-rw-rw-   0        0        0       28 2024-04-15 10:26:39.000000 mongo_m-1.1.3/mongo_m/repository/collections/__init__.py
--rw-rw-rw-   0        0        0      805 2024-04-25 05:23:36.000000 mongo_m-1.1.3/mongo_m/repository/collections/collections.py
--rw-rw-rw-   0        0        0      490 2024-04-25 05:23:36.000000 mongo_m-1.1.3/mongo_m/repository/collections/models.py
--rw-rw-rw-   0        0        0      938 2024-04-22 10:42:33.000000 mongo_m-1.1.3/mongo_m/repository/collections/query.py
-drwxrwxrwx   0        0        0        0 2024-04-25 10:26:20.213248 mongo_m-1.1.3/mongo_m/services/
--rw-rw-rw-   0        0        0        0 2024-04-22 12:24:10.000000 mongo_m-1.1.3/mongo_m/services/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 10:26:20.215248 mongo_m-1.1.3/mongo_m/services/migration/
--rw-rw-rw-   0        0        0       47 2024-04-25 05:23:36.000000 mongo_m-1.1.3/mongo_m/services/migration/__init__.py
--rw-rw-rw-   0        0        0     2770 2024-04-25 08:49:49.000000 mongo_m-1.1.3/mongo_m/services/migration/file.py
--rw-rw-rw-   0        0        0     1672 2024-04-25 05:56:57.000000 mongo_m-1.1.3/mongo_m/services/migration/migration.py
-drwxrwxrwx   0        0        0        0 2024-04-25 10:26:20.217249 mongo_m-1.1.3/mongo_m.egg-info/
--rw-rw-rw-   0        0        0     1560 2024-04-25 10:26:20.000000 mongo_m-1.1.3/mongo_m.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      745 2024-04-25 10:26:20.000000 mongo_m-1.1.3/mongo_m.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 10:26:20.000000 mongo_m-1.1.3/mongo_m.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-25 10:00:52.000000 mongo_m-1.1.3/mongo_m.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      185 2024-04-25 10:26:20.000000 mongo_m-1.1.3/mongo_m.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-25 10:26:20.000000 mongo_m-1.1.3/mongo_m.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 10:26:20.219248 mongo_m-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1922 2024-04-25 10:25:56.000000 mongo_m-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 10:26:20.216247 mongo_m-1.1.3/tests/
--rw-rw-rw-   0        0        0        0 2024-04-22 12:21:08.000000 mongo_m-1.1.3/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:58:19.721705 mongo_m-1.1.4/
+-rw-rw-rw-   0        0        0     1560 2024-04-25 12:58:19.721705 mongo_m-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2288 2024-04-25 12:48:38.000000 mongo_m-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 12:58:19.687572 mongo_m-1.1.4/mongo_m/
+-rw-rw-rw-   0        0        0        0 2024-04-22 13:51:52.000000 mongo_m-1.1.4/mongo_m/__init__.py
+-rw-rw-rw-   0        0        0     1952 2024-04-25 12:19:06.000000 mongo_m-1.1.4/mongo_m/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:58:19.714379 mongo_m-1.1.4/mongo_m/core/
+-rw-rw-rw-   0        0        0       99 2024-04-23 16:31:26.000000 mongo_m-1.1.4/mongo_m/core/__init__.py
+-rw-rw-rw-   0        0        0      511 2024-04-22 14:19:36.000000 mongo_m-1.1.4/mongo_m/core/creator.py
+-rw-rw-rw-   0        0        0      602 2024-04-25 05:23:36.000000 mongo_m-1.1.4/mongo_m/core/ini_file.py
+-rw-rw-rw-   0        0        0     3164 2024-04-25 10:00:11.000000 mongo_m-1.1.4/mongo_m/core/inspect_module.py
+-rw-rw-rw-   0        0        0      764 2024-04-15 10:37:27.000000 mongo_m-1.1.4/mongo_m/core/mongodb.py
+-rw-rw-rw-   0        0        0      487 2024-04-25 06:48:57.000000 mongo_m-1.1.4/mongo_m/core/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:58:19.714379 mongo_m-1.1.4/mongo_m/repository/
+-rw-rw-rw-   0        0        0        0 2024-04-22 12:24:01.000000 mongo_m-1.1.4/mongo_m/repository/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:58:19.716530 mongo_m-1.1.4/mongo_m/repository/collections/
+-rw-rw-rw-   0        0        0       28 2024-04-15 10:26:39.000000 mongo_m-1.1.4/mongo_m/repository/collections/__init__.py
+-rw-rw-rw-   0        0        0      805 2024-04-25 05:23:36.000000 mongo_m-1.1.4/mongo_m/repository/collections/collections.py
+-rw-rw-rw-   0        0        0      490 2024-04-25 05:23:36.000000 mongo_m-1.1.4/mongo_m/repository/collections/models.py
+-rw-rw-rw-   0        0        0      938 2024-04-22 10:42:33.000000 mongo_m-1.1.4/mongo_m/repository/collections/query.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:58:19.717531 mongo_m-1.1.4/mongo_m/services/
+-rw-rw-rw-   0        0        0        0 2024-04-22 12:24:10.000000 mongo_m-1.1.4/mongo_m/services/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:58:19.718695 mongo_m-1.1.4/mongo_m/services/migration/
+-rw-rw-rw-   0        0        0       47 2024-04-25 05:23:36.000000 mongo_m-1.1.4/mongo_m/services/migration/__init__.py
+-rw-rw-rw-   0        0        0     2770 2024-04-25 08:49:49.000000 mongo_m-1.1.4/mongo_m/services/migration/file.py
+-rw-rw-rw-   0        0        0     3259 2024-04-25 12:16:37.000000 mongo_m-1.1.4/mongo_m/services/migration/migration.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:58:19.720704 mongo_m-1.1.4/mongo_m.egg-info/
+-rw-rw-rw-   0        0        0     1560 2024-04-25 12:58:19.000000 mongo_m-1.1.4/mongo_m.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      755 2024-04-25 12:58:19.000000 mongo_m-1.1.4/mongo_m.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 12:58:19.000000 mongo_m-1.1.4/mongo_m.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-25 12:58:19.000000 mongo_m-1.1.4/mongo_m.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      185 2024-04-25 12:58:19.000000 mongo_m-1.1.4/mongo_m.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-25 12:58:19.000000 mongo_m-1.1.4/mongo_m.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 12:58:19.721705 mongo_m-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1920 2024-04-25 12:58:05.000000 mongo_m-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:58:19.719706 mongo_m-1.1.4/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-22 12:21:08.000000 mongo_m-1.1.4/tests/__init__.py
```

### Comparing `mongo_m-1.1.3/PKG-INFO` & `mongo_m-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongo_m
-Version: 1.1.3
+Version: 1.1.4
 Summary: A database migration tool for MongoDB
 Home-page: https://github.com/BeyonD311/mongo-m
 Author: Dankov Sergey
 Author-email: beyond31@mail.ru
 License: GNU General Public License v3 (GPLv3)
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mongo_m-1.1.3/mongo_m/__main__.py` & `mongo_m-1.1.4/mongo_m/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,66 +1,69 @@
 import sys, asyncio
+from pymongo import MongoClient
 from dotenv import load_dotenv
 from pathlib import Path
 from .core import create_file_ini, get_config
-from .repository.collections.models import Query
 from .services.migration import (
-    FileMigration, get_collections, connect_to_mongo, get_database,
-    add_fields, delete_fields
+    FileMigration, connect_to_mongo,
+    add_fields, delete_fields,
+    screening_fields,
+    get_database
 )
 
 load_dotenv()
 PATH = Path(__file__).parent.resolve()
 
 
-async def update_migration(client):
-    collections_migration = FileMigration.get_migration()
+def update_migration(client: MongoClient, type_action: bool):
+    """
+    Выполнение миграции
+    :param client:
+    :type client:
+    :param type_action: bool True добавление полей False удаление
+    :type type_action:
+    :return:
+    :rtype:
+    """
     db = get_database(client)
-    for collection in get_collections(client):
-        if collection.name in collections_migration:
-            fields = set(collections_migration[collection.name].keys())
-            #Симметрическая разность множеств
-            disjunctive = fields ^ collection.fields
-            if "_id" in disjunctive:
-                disjunctive.remove("_id")
-            delete = Query()
-            add = Query()
-            for field in disjunctive:
-                if field in fields:
-                    add.query.append({field: {"$exists": False}})
-                    add.fields[field] = collections_migration[collection.name][field]
-                    add.empty = False
-                if field not in fields and collection.fields:
-                    delete.query.append({field: {"$exists": True}})
-                    delete.fields[field] = ""
-                    delete.empty = False
-            add_fields(db, collection.name, add)
-            # delete_fields(db, collection.name, delete)
+    for collection_name, add, delete in screening_fields(client):
+        if type_action:
+            add_fields(db, collection_name, add)
+        else:
+            delete_fields(db, collection_name, delete)
 
 
 async def create_migration():
     config = get_config()
     module_path = config.get("MONGO", "module_path")
     migration_file = await FileMigration.make_migration(module_path)
     FileMigration.update_migration_file(migration_file)
 
 
 async def main():
     FileMigration.create_migration_catalog()
     params = tuple(sys.argv[1:])
     client = None
     try:
-        if params[0] == "--create-migration":
+        if params[0] == "create-migration":
             await create_migration()
-        elif params[0] == "--update-migration":
+        elif params[0] == "update-migration":
             client = connect_to_mongo()
-            await update_migration(client)
-        elif params[0] == "--init":
+            action = None
+
+            if params[1] == '-a':
+                action = True
+            elif params[1] == '-d':
+                action = False
+
+            if action is not None:
+                update_migration(client, action)
+        elif params[0] == "init":
             create_file_ini()
     except Exception as e:
         print(e)
     finally:
         if client != None:
             client.close()
 
 if __name__ == "__main__":
-    asyncio.run(main())
+    asyncio.run(main())
```

### Comparing `mongo_m-1.1.3/mongo_m/core/ini_file.py` & `mongo_m-1.1.4/mongo_m/core/ini_file.py`

 * *Files identical despite different names*

### Comparing `mongo_m-1.1.3/mongo_m/core/inspect_module.py` & `mongo_m-1.1.4/mongo_m/core/inspect_module.py`

 * *Files identical despite different names*

### Comparing `mongo_m-1.1.3/mongo_m/core/mongodb.py` & `mongo_m-1.1.4/mongo_m/core/mongodb.py`

 * *Files identical despite different names*

### Comparing `mongo_m-1.1.3/mongo_m/repository/collections/collections.py` & `mongo_m-1.1.4/mongo_m/repository/collections/collections.py`

 * *Files identical despite different names*

### Comparing `mongo_m-1.1.3/mongo_m/repository/collections/query.py` & `mongo_m-1.1.4/mongo_m/repository/collections/query.py`

 * *Files identical despite different names*

### Comparing `mongo_m-1.1.3/mongo_m/services/migration/file.py` & `mongo_m-1.1.4/mongo_m/services/migration/file.py`

 * *Files identical despite different names*

### Comparing `mongo_m-1.1.3/mongo_m.egg-info/PKG-INFO` & `mongo_m-1.1.4/mongo_m.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongo_m
-Version: 1.1.3
+Version: 1.1.4
 Summary: A database migration tool for MongoDB
 Home-page: https://github.com/BeyonD311/mongo-m
 Author: Dankov Sergey
 Author-email: beyond31@mail.ru
 License: GNU General Public License v3 (GPLv3)
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mongo_m-1.1.3/mongo_m.egg-info/SOURCES.txt` & `mongo_m-1.1.4/mongo_m.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+README.md
 setup.py
 mongo_m/__init__.py
 mongo_m/__main__.py
 mongo_m.egg-info/PKG-INFO
 mongo_m.egg-info/SOURCES.txt
 mongo_m.egg-info/dependency_links.txt
 mongo_m.egg-info/not-zip-safe
```

### Comparing `mongo_m-1.1.3/setup.py` & `mongo_m-1.1.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,17 +20,17 @@
         with open('README.md') as f:
             return f.read()
     except IOError:
         return DESCRIPTION
 
 setup(
     name='mongo_m',
-    version='1.1.3',
+    version='1.1.4',
     description=DESCRIPTION,
-    long_description=get_read_me(),
+    long_description=DESCRIPTION,
     long_description_content_type="text/markdown",
     author='Dankov Sergey',
     author_email='beyond31@mail.ru',
     license='GNU General Public License v3 (GPLv3)',
     url='https://github.com/BeyonD311/mongo-m',
     packages=find_packages(),
     include_package_data=True,
```

