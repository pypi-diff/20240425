# Comparing `tmp/sqlx-executor-1.1.5.tar.gz` & `tmp/sqlx-executor-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlx-executor-1.1.5.tar", last modified: Fri Mar 29 05:51:49 2024, max compression
+gzip compressed data, was "sqlx-executor-1.1.6.tar", last modified: Thu Apr 25 08:12:50 2024, max compression
```

## Comparing `sqlx-executor-1.1.5.tar` & `sqlx-executor-1.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-03-29 05:51:49.603476 sqlx-executor-1.1.5/
--rw-rw-r--   0 summy      (501) staff       (20)    11357 2024-03-14 05:16:15.000000 sqlx-executor-1.1.5/LICENSE
--rw-r--r--   0 summy      (501) staff       (20)     2038 2024-03-29 05:51:49.601384 sqlx-executor-1.1.5/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)     1569 2024-03-29 02:15:47.000000 sqlx-executor-1.1.5/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-03-29 05:51:49.591966 sqlx-executor-1.1.5/executor/
--rw-rw-r--   0 summy      (501) staff       (20)      347 2024-03-28 02:27:57.000000 sqlx-executor-1.1.5/executor/__init__.py
--rw-rw-r--   0 summy      (501) staff       (20)      205 2024-03-29 05:41:40.000000 sqlx-executor-1.1.5/executor/constant.py
--rw-rw-r--   0 summy      (501) staff       (20)     8623 2024-03-28 02:27:46.000000 sqlx-executor-1.1.5/executor/core.py
--rw-r--r--   0 summy      (501) staff       (20)      901 2024-03-23 15:57:10.000000 sqlx-executor-1.1.5/executor/engine.py
--rw-rw-r--   0 summy      (501) staff       (20)     2042 2024-03-23 16:12:52.000000 sqlx-executor-1.1.5/executor/init_import.py
--rw-rw-r--   0 summy      (501) staff       (20)      740 2024-03-25 03:02:59.000000 sqlx-executor-1.1.5/executor/log_support.py
--rw-rw-r--   0 summy      (501) staff       (20)     1027 2024-03-22 15:37:38.000000 sqlx-executor-1.1.5/executor/pooling.py
--rw-r--r--   0 summy      (501) staff       (20)      422 2024-03-29 05:50:43.000000 sqlx-executor-1.1.5/executor/sql_support.py
--rw-rw-r--   0 summy      (501) staff       (20)     3892 2024-03-25 02:25:33.000000 sqlx-executor-1.1.5/executor/support.py
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-03-29 05:51:49.603953 sqlx-executor-1.1.5/setup.cfg
--rw-rw-r--   0 summy      (501) staff       (20)     1189 2024-03-29 05:51:42.000000 sqlx-executor-1.1.5/setup.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-03-29 05:51:49.600104 sqlx-executor-1.1.5/sqlx_executor.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)     2038 2024-03-29 05:51:49.000000 sqlx-executor-1.1.5/sqlx_executor.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      401 2024-03-29 05:51:49.000000 sqlx-executor-1.1.5/sqlx_executor.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-03-29 05:51:49.000000 sqlx-executor-1.1.5/sqlx_executor.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-03-27 09:27:58.000000 sqlx-executor-1.1.5/sqlx_executor.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)        9 2024-03-29 05:51:49.000000 sqlx-executor-1.1.5/sqlx_executor.egg-info/top_level.txt
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-25 08:12:50.213291 sqlx-executor-1.1.6/
+-rw-rw-r--   0 summy      (501) staff       (20)    11357 2024-03-14 05:16:15.000000 sqlx-executor-1.1.6/LICENSE
+-rw-r--r--   0 summy      (501) staff       (20)     2020 2024-04-25 08:12:50.211896 sqlx-executor-1.1.6/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)     1569 2024-03-29 02:15:47.000000 sqlx-executor-1.1.6/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-25 08:12:50.198313 sqlx-executor-1.1.6/executor/
+-rw-rw-r--   0 summy      (501) staff       (20)      347 2024-03-28 02:27:57.000000 sqlx-executor-1.1.6/executor/__init__.py
+-rw-rw-r--   0 summy      (501) staff       (20)      205 2024-03-29 05:41:40.000000 sqlx-executor-1.1.6/executor/constant.py
+-rw-rw-r--   0 summy      (501) staff       (20)     8635 2024-04-04 00:56:53.000000 sqlx-executor-1.1.6/executor/core.py
+-rw-r--r--   0 summy      (501) staff       (20)      901 2024-03-23 15:57:10.000000 sqlx-executor-1.1.6/executor/engine.py
+-rw-rw-r--   0 summy      (501) staff       (20)     2042 2024-03-23 16:12:52.000000 sqlx-executor-1.1.6/executor/init_import.py
+-rw-rw-r--   0 summy      (501) staff       (20)      740 2024-03-25 03:02:59.000000 sqlx-executor-1.1.6/executor/log_support.py
+-rw-rw-r--   0 summy      (501) staff       (20)     1027 2024-03-22 15:37:38.000000 sqlx-executor-1.1.6/executor/pooling.py
+-rw-r--r--   0 summy      (501) staff       (20)      422 2024-03-29 05:50:43.000000 sqlx-executor-1.1.6/executor/sql_support.py
+-rw-rw-r--   0 summy      (501) staff       (20)     3892 2024-03-25 02:25:33.000000 sqlx-executor-1.1.6/executor/support.py
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-04-25 08:12:50.213602 sqlx-executor-1.1.6/setup.cfg
+-rw-rw-r--   0 summy      (501) staff       (20)     1165 2024-04-25 08:11:56.000000 sqlx-executor-1.1.6/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-25 08:12:50.208936 sqlx-executor-1.1.6/sqlx_executor.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)     2020 2024-04-25 08:12:50.000000 sqlx-executor-1.1.6/sqlx_executor.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      401 2024-04-25 08:12:50.000000 sqlx-executor-1.1.6/sqlx_executor.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-04-25 08:12:50.000000 sqlx-executor-1.1.6/sqlx_executor.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-03-27 09:27:58.000000 sqlx-executor-1.1.6/sqlx_executor.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)        9 2024-04-25 08:12:50.000000 sqlx-executor-1.1.6/sqlx_executor.egg-info/top_level.txt
```

### Comparing `sqlx-executor-1.1.5/LICENSE` & `sqlx-executor-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlx-executor-1.1.5/PKG-INFO` & `sqlx-executor-1.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: sqlx-executor
-Version: 1.1.5
+Version: 1.1.6
 Summary: A simple thread safe sql executor for Python with connection pool. Support MySQL, PostgreSQL, SQLite etc.
 Home-page: https://gitee.com/summry/sql-executor
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
-Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Database,Python,RDB
+Keywords: SQL,MySQL,PostgreSQL,SQLite,Database,Python,RDB
 Platform: UNKNOWN
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Usage Sample
 ''''''''''''
 
 .. code::
```

### Comparing `sqlx-executor-1.1.5/README.rst` & `sqlx-executor-1.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `sqlx-executor-1.1.5/executor/core.py` & `sqlx-executor-1.1.6/executor/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,18 +61,18 @@
 
     with DB_LOCK:
         if _DB_CTX is not None:
             raise DBError('DB is already initialized.')
         _DB_CTX = DBCtx(connect=connect, prepared=prepared)
 
     if pool_size > 0:
-        logger.info("Inited db <%s> of %s with driver: '%s' and pool size: %d." % (hex(id(_DB_CTX)), engine.value,
+        logger.info("Inited database <%s> of %s with driver: '%s' and pool size: %d." % (hex(id(_DB_CTX)), engine.value,
                                                                                           driver_name, pool_size))
     else:
-        logger.info("Inited db <%s> of %s with driver: '%s'." % (hex(id(_DB_CTX)), engine.value, driver_name))
+        logger.info("Inited database <%s> of %s with driver: '%s'." % (hex(id(_DB_CTX)), engine.value, driver_name))
 
     return engine
 
 
 def connection():
     """
     Return ConnectionCtx object that can be used by 'with' statement:
```

### Comparing `sqlx-executor-1.1.5/executor/engine.py` & `sqlx-executor-1.1.6/executor/engine.py`

 * *Files identical despite different names*

### Comparing `sqlx-executor-1.1.5/executor/init_import.py` & `sqlx-executor-1.1.6/executor/init_import.py`

 * *Files identical despite different names*

### Comparing `sqlx-executor-1.1.5/executor/log_support.py` & `sqlx-executor-1.1.6/executor/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-executor-1.1.5/executor/pooling.py` & `sqlx-executor-1.1.6/executor/pooling.py`

 * *Files identical despite different names*

### Comparing `sqlx-executor-1.1.5/executor/support.py` & `sqlx-executor-1.1.6/executor/support.py`

 * *Files identical despite different names*

### Comparing `sqlx-executor-1.1.5/setup.py` & `sqlx-executor-1.1.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 
 setup(
     name='sqlx-executor',
     packages=['executor'],
     description="A simple thread safe sql executor for Python with connection pool. Support MySQL, PostgreSQL, SQLite etc.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.1.5',
+    version='1.1.6',
     url='https://gitee.com/summry/sql-executor',
     author='summy',
     author_email='xiazhongbiao@126.com',
-    keywords=['SQL', 'MySQL', 'PostgreSQL', 'SQLite', 'Oracle', 'SQL Server', 'Database', 'Python', 'RDB'],
+    keywords=['SQL', 'MySQL', 'PostgreSQL', 'SQLite', 'Database', 'Python', 'RDB'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
     },
     include_package_data=True,
-    python_requires='>=3.5',
+    python_requires='>=3.6',
     zip_safe=False
 )
```

### Comparing `sqlx-executor-1.1.5/sqlx_executor.egg-info/PKG-INFO` & `sqlx-executor-1.1.6/sqlx_executor.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: sqlx-executor
-Version: 1.1.5
+Version: 1.1.6
 Summary: A simple thread safe sql executor for Python with connection pool. Support MySQL, PostgreSQL, SQLite etc.
 Home-page: https://gitee.com/summry/sql-executor
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
-Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Database,Python,RDB
+Keywords: SQL,MySQL,PostgreSQL,SQLite,Database,Python,RDB
 Platform: UNKNOWN
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Usage Sample
 ''''''''''''
 
 .. code::
```

