# Comparing `tmp/database-common-tools-1.1.6.tar.gz` & `tmp/database-common-tools-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database-common-tools-1.1.6.tar", last modified: Tue Apr 23 12:24:42 2024, max compression
+gzip compressed data, was "database-common-tools-1.1.7.tar", last modified: Thu Apr 25 09:24:15 2024, max compression
```

## Comparing `database-common-tools-1.1.6.tar` & `database-common-tools-1.1.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-23 12:24:42.243451 database-common-tools-1.1.6/
--rw-r--r--   0 yangming   (501) staff       (20)     1066 2024-01-24 08:52:12.000000 database-common-tools-1.1.6/LICENSE
--rw-r--r--   0 yangming   (501) staff       (20)      701 2024-04-23 12:24:42.242954 database-common-tools-1.1.6/PKG-INFO
--rw-r--r--   0 yangming   (501) staff       (20)       23 2024-01-24 08:52:12.000000 database-common-tools-1.1.6/README.md
-drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-23 12:24:42.228240 database-common-tools-1.1.6/database_common_tools.egg-info/
--rw-r--r--   0 yangming   (501) staff       (20)      701 2024-04-23 12:24:42.000000 database-common-tools-1.1.6/database_common_tools.egg-info/PKG-INFO
--rw-r--r--   0 yangming   (501) staff       (20)      682 2024-04-23 12:24:42.000000 database-common-tools-1.1.6/database_common_tools.egg-info/SOURCES.txt
--rw-r--r--   0 yangming   (501) staff       (20)        1 2024-04-23 12:24:42.000000 database-common-tools-1.1.6/database_common_tools.egg-info/dependency_links.txt
--rw-r--r--   0 yangming   (501) staff       (20)       85 2024-04-23 12:24:42.000000 database-common-tools-1.1.6/database_common_tools.egg-info/requires.txt
--rw-r--r--   0 yangming   (501) staff       (20)       19 2024-04-23 12:24:42.000000 database-common-tools-1.1.6/database_common_tools.egg-info/top_level.txt
-drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-23 12:24:42.241610 database-common-tools-1.1.6/databasetools/
--rw-r--r--   0 yangming   (501) staff       (20)     1636 2024-01-25 08:25:09.000000 database-common-tools-1.1.6/databasetools/__init__.py
--rw-r--r--   0 yangming   (501) staff       (20)     1990 2024-01-24 09:06:09.000000 database-common-tools-1.1.6/databasetools/analysis_json.py
--rw-r--r--   0 yangming   (501) staff       (20)     2090 2024-04-16 11:58:05.000000 database-common-tools-1.1.6/databasetools/analysis_json_v2.py
--rw-r--r--   0 yangming   (501) staff       (20)     2604 2024-04-23 12:15:27.000000 database-common-tools-1.1.6/databasetools/analysis_json_v3.py
--rw-r--r--   0 yangming   (501) staff       (20)     3191 2024-01-24 09:06:09.000000 database-common-tools-1.1.6/databasetools/data_analysis.py
--rw-r--r--   0 yangming   (501) staff       (20)     3562 2024-04-16 12:39:11.000000 database-common-tools-1.1.6/databasetools/data_analysis_v2.py
--rw-r--r--   0 yangming   (501) staff       (20)     4515 2024-04-17 05:55:14.000000 database-common-tools-1.1.6/databasetools/data_analysis_v3.py
--rw-r--r--   0 yangming   (501) staff       (20)      844 2024-04-23 12:14:40.000000 database-common-tools-1.1.6/databasetools/kafka_connect.py
--rw-r--r--   0 yangming   (501) staff       (20)     2180 2024-03-14 06:55:26.000000 database-common-tools-1.1.6/databasetools/mongo_connect.py
--rw-r--r--   0 yangming   (501) staff       (20)      721 2024-01-26 07:55:44.000000 database-common-tools-1.1.6/databasetools/mt_wx_message.py
--rw-r--r--   0 yangming   (501) staff       (20)      279 2024-04-15 02:52:56.000000 database-common-tools-1.1.6/databasetools/mysql_connect.py
--rw-r--r--   0 yangming   (501) staff       (20)     1047 2024-04-16 08:35:37.000000 database-common-tools-1.1.6/databasetools/opensearch_connect.py
--rw-r--r--   0 yangming   (501) staff       (20)     5458 2024-01-26 08:31:58.000000 database-common-tools-1.1.6/databasetools/redis_connect.py
--rw-r--r--   0 yangming   (501) staff       (20)       38 2024-04-23 12:24:42.243641 database-common-tools-1.1.6/setup.cfg
--rw-r--r--   0 yangming   (501) staff       (20)     3932 2024-04-23 12:00:16.000000 database-common-tools-1.1.6/setup.py
-drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-23 12:24:42.242512 database-common-tools-1.1.6/test/
--rw-r--r--   0 yangming   (501) staff       (20)        0 2024-01-26 07:51:53.000000 database-common-tools-1.1.6/test/__init__.py
+drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-25 09:24:15.191930 database-common-tools-1.1.7/
+-rw-r--r--   0 yangming   (501) staff       (20)     1066 2024-01-24 08:52:12.000000 database-common-tools-1.1.7/LICENSE
+-rw-r--r--   0 yangming   (501) staff       (20)      701 2024-04-25 09:24:15.191403 database-common-tools-1.1.7/PKG-INFO
+-rw-r--r--   0 yangming   (501) staff       (20)       23 2024-01-24 08:52:12.000000 database-common-tools-1.1.7/README.md
+drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-25 09:24:15.177289 database-common-tools-1.1.7/database_common_tools.egg-info/
+-rw-r--r--   0 yangming   (501) staff       (20)      701 2024-04-25 09:24:15.000000 database-common-tools-1.1.7/database_common_tools.egg-info/PKG-INFO
+-rw-r--r--   0 yangming   (501) staff       (20)      682 2024-04-25 09:24:15.000000 database-common-tools-1.1.7/database_common_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 yangming   (501) staff       (20)        1 2024-04-25 09:24:15.000000 database-common-tools-1.1.7/database_common_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 yangming   (501) staff       (20)       85 2024-04-25 09:24:15.000000 database-common-tools-1.1.7/database_common_tools.egg-info/requires.txt
+-rw-r--r--   0 yangming   (501) staff       (20)       19 2024-04-25 09:24:15.000000 database-common-tools-1.1.7/database_common_tools.egg-info/top_level.txt
+drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-25 09:24:15.189665 database-common-tools-1.1.7/databasetools/
+-rw-r--r--   0 yangming   (501) staff       (20)     1636 2024-01-25 08:25:09.000000 database-common-tools-1.1.7/databasetools/__init__.py
+-rw-r--r--   0 yangming   (501) staff       (20)     1990 2024-01-24 09:06:09.000000 database-common-tools-1.1.7/databasetools/analysis_json.py
+-rw-r--r--   0 yangming   (501) staff       (20)     2090 2024-04-16 11:58:05.000000 database-common-tools-1.1.7/databasetools/analysis_json_v2.py
+-rw-r--r--   0 yangming   (501) staff       (20)     2604 2024-04-25 08:27:14.000000 database-common-tools-1.1.7/databasetools/analysis_json_v3.py
+-rw-r--r--   0 yangming   (501) staff       (20)     3191 2024-01-24 09:06:09.000000 database-common-tools-1.1.7/databasetools/data_analysis.py
+-rw-r--r--   0 yangming   (501) staff       (20)     3562 2024-04-16 12:39:11.000000 database-common-tools-1.1.7/databasetools/data_analysis_v2.py
+-rw-r--r--   0 yangming   (501) staff       (20)     4515 2024-04-17 05:55:14.000000 database-common-tools-1.1.7/databasetools/data_analysis_v3.py
+-rw-r--r--   0 yangming   (501) staff       (20)      844 2024-04-23 12:14:40.000000 database-common-tools-1.1.7/databasetools/kafka_connect.py
+-rw-r--r--   0 yangming   (501) staff       (20)     2300 2024-04-25 09:23:19.000000 database-common-tools-1.1.7/databasetools/mongo_connect.py
+-rw-r--r--   0 yangming   (501) staff       (20)      721 2024-01-26 07:55:44.000000 database-common-tools-1.1.7/databasetools/mt_wx_message.py
+-rw-r--r--   0 yangming   (501) staff       (20)      279 2024-04-15 02:52:56.000000 database-common-tools-1.1.7/databasetools/mysql_connect.py
+-rw-r--r--   0 yangming   (501) staff       (20)     1047 2024-04-25 08:26:57.000000 database-common-tools-1.1.7/databasetools/opensearch_connect.py
+-rw-r--r--   0 yangming   (501) staff       (20)     5458 2024-01-26 08:31:58.000000 database-common-tools-1.1.7/databasetools/redis_connect.py
+-rw-r--r--   0 yangming   (501) staff       (20)       38 2024-04-25 09:24:15.192142 database-common-tools-1.1.7/setup.cfg
+-rw-r--r--   0 yangming   (501) staff       (20)     3932 2024-04-25 09:23:36.000000 database-common-tools-1.1.7/setup.py
+drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-25 09:24:15.190811 database-common-tools-1.1.7/test/
+-rw-r--r--   0 yangming   (501) staff       (20)        0 2024-01-26 07:51:53.000000 database-common-tools-1.1.7/test/__init__.py
```

### Comparing `database-common-tools-1.1.6/LICENSE` & `database-common-tools-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.1.6/database_common_tools.egg-info/SOURCES.txt` & `database-common-tools-1.1.7/database_common_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.1.6/databasetools/__init__.py` & `database-common-tools-1.1.7/databasetools/__init__.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.1.6/databasetools/analysis_json.py` & `database-common-tools-1.1.7/databasetools/analysis_json.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.1.6/databasetools/analysis_json_v2.py` & `database-common-tools-1.1.7/databasetools/analysis_json_v2.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.1.6/databasetools/analysis_json_v3.py` & `database-common-tools-1.1.7/databasetools/analysis_json_v3.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.1.6/databasetools/data_analysis.py` & `database-common-tools-1.1.7/databasetools/data_analysis.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.1.6/databasetools/data_analysis_v2.py` & `database-common-tools-1.1.7/databasetools/data_analysis_v2.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.1.6/databasetools/data_analysis_v3.py` & `database-common-tools-1.1.7/databasetools/data_analysis_v3.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.1.6/databasetools/kafka_connect.py` & `database-common-tools-1.1.7/databasetools/kafka_connect.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.1.6/databasetools/mongo_connect.py` & `database-common-tools-1.1.7/databasetools/mongo_connect.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,14 +65,18 @@
 def mongo_count_total(collection):
     return collection.count_documents({})
 
 
 def mongo_find_start(collection, start, size):
     return collection.find().skip(start).limit(size)
 
+
+def mongo_find_query_start(collection, query, start, size):
+    return collection.find(query).skip(start).limit(size)
+
 ##################################################
 # mongo connect
 ##################################################
 # url 连接mongo域名
 # db  连接mongo 数据库
 # tb  连接mongo 数据表
 def mongo_conn(url, db, tb):
```

### Comparing `database-common-tools-1.1.6/databasetools/mt_wx_message.py` & `database-common-tools-1.1.7/databasetools/mt_wx_message.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.1.6/databasetools/opensearch_connect.py` & `database-common-tools-1.1.7/databasetools/opensearch_connect.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.1.6/databasetools/redis_connect.py` & `database-common-tools-1.1.7/databasetools/redis_connect.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.1.6/setup.py` & `database-common-tools-1.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'database-common-tools'
 DESCRIPTION = 'let message middleware and use database more easy'
 URL = 'https://github.com/yangming9/database-common-tools.git'
 EMAIL = 'yma91412@gmail.com'
 AUTHOR = 'Coder Yang'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '1.1.6'
+VERSION = '1.1.7'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'requests',
     'jsonpath',
     'pymongo',
     'redis',
```

