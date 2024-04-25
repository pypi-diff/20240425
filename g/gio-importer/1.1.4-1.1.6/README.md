# Comparing `tmp/gio_importer-1.1.4.tar.gz` & `tmp/gio_importer-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gio_importer-1.1.4.tar", last modified: Thu Apr 25 08:01:43 2024, max compression
+gzip compressed data, was "gio_importer-1.1.6.tar", last modified: Thu Apr 25 08:11:31 2024, max compression
```

## Comparing `gio_importer-1.1.4.tar` & `gio_importer-1.1.6.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-25 08:01:43.220562 gio_importer-1.1.4/
--rw-r--r--   0 chengcheng   (501) staff       (20)     1061 2024-04-25 07:46:34.000000 gio_importer-1.1.4/LICENSE
--rw-r--r--   0 chengcheng   (501) staff       (20)       71 2024-04-25 07:46:34.000000 gio_importer-1.1.4/MANIFEST.in
--rw-r--r--   0 chengcheng   (501) staff       (20)    12295 2024-04-25 08:01:43.220227 gio_importer-1.1.4/PKG-INFO
--rw-r--r--   0 chengcheng   (501) staff       (20)      792 2024-04-25 07:46:34.000000 gio_importer-1.1.4/README.md
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-25 08:01:43.184992 gio_importer-1.1.4/gio_importer.egg-info/
--rw-r--r--   0 chengcheng   (501) staff       (20)    12295 2024-04-25 08:01:43.000000 gio_importer-1.1.4/gio_importer.egg-info/PKG-INFO
--rw-r--r--   0 chengcheng   (501) staff       (20)     1381 2024-04-25 08:01:43.000000 gio_importer-1.1.4/gio_importer.egg-info/SOURCES.txt
--rw-r--r--   0 chengcheng   (501) staff       (20)        1 2024-04-25 08:01:43.000000 gio_importer-1.1.4/gio_importer.egg-info/dependency_links.txt
--rw-r--r--   0 chengcheng   (501) staff       (20)      196 2024-04-25 08:01:43.000000 gio_importer-1.1.4/gio_importer.egg-info/entry_points.txt
--rw-r--r--   0 chengcheng   (501) staff       (20)       84 2024-04-25 08:01:43.000000 gio_importer-1.1.4/gio_importer.egg-info/requires.txt
--rw-r--r--   0 chengcheng   (501) staff       (20)       10 2024-04-25 08:01:43.000000 gio_importer-1.1.4/gio_importer.egg-info/top_level.txt
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-25 08:01:43.194199 gio_importer-1.1.4/importers/
--rw-r--r--   0 chengcheng   (501) staff       (20)    11711 2024-04-25 07:46:34.000000 gio_importer-1.1.4/importers/README.md
--rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-04-25 07:46:34.000000 gio_importer-1.1.4/importers/__init__.py
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-25 08:01:43.195899 gio_importer-1.1.4/importers/clear_data/
--rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-04-25 07:46:34.000000 gio_importer-1.1.4/importers/clear_data/__init__.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     2779 2024-04-25 07:46:34.000000 gio_importer-1.1.4/importers/clear_data/clear_data.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     1714 2024-04-25 07:46:34.000000 gio_importer-1.1.4/importers/clear_user.py
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-25 08:01:43.200229 gio_importer-1.1.4/importers/common/
--rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-04-25 07:46:34.000000 gio_importer-1.1.4/importers/common/__init__.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     5581 2024-04-25 07:46:34.000000 gio_importer-1.1.4/importers/common/common_util.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     2620 2024-04-25 07:46:34.000000 gio_importer-1.1.4/importers/common/config_util.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     2506 2024-04-25 07:46:34.000000 gio_importer-1.1.4/importers/common/http_util.py
--rw-r--r--   0 chengcheng   (501) staff       (20)      955 2024-04-25 07:46:34.000000 gio_importer-1.1.4/importers/common/log_util.py
--rw-r--r--   0 chengcheng   (501) staff       (20)      771 2024-04-25 07:46:34.000000 gio_importer-1.1.4/importers/conf.cfg
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-25 08:01:43.208170 gio_importer-1.1.4/importers/data_import/
--rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-04-25 07:46:34.000000 gio_importer-1.1.4/importers/data_import/__init__.py
--rw-r--r--   0 chengcheng   (501) staff       (20)    21768 2024-04-25 07:46:34.000000 gio_importer-1.1.4/importers/data_import/data_ads.py
--rw-r--r--   0 chengcheng   (501) staff       (20)    21685 2024-04-25 07:46:34.000000 gio_importer-1.1.4/importers/data_import/data_events.py
--rw-r--r--   0 chengcheng   (501) staff       (20)    11251 2024-04-25 07:46:34.000000 gio_importer-1.1.4/importers/data_import/data_format_util.py
--rw-r--r--   0 chengcheng   (501) staff       (20)    17685 2024-04-25 07:46:34.000000 gio_importer-1.1.4/importers/data_import/data_item_variable.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     6455 2024-04-25 07:46:34.000000 gio_importer-1.1.4/importers/data_import/data_model.py
--rw-r--r--   0 chengcheng   (501) staff       (20)    15336 2024-04-25 07:46:34.000000 gio_importer-1.1.4/importers/data_import/data_user_variable.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     6943 2024-04-25 07:46:34.000000 gio_importer-1.1.4/importers/data_importer.py
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-25 08:01:43.211688 gio_importer-1.1.4/importers/db_import/
--rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-04-25 07:46:34.000000 gio_importer-1.1.4/importers/db_import/__init__.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     2717 2024-04-25 07:46:34.000000 gio_importer-1.1.4/importers/db_import/database_import.py
--rw-r--r--   0 chengcheng   (501) staff       (20)    14400 2024-04-25 07:57:38.000000 gio_importer-1.1.4/importers/db_import/hive_import.py
--rw-r--r--   0 chengcheng   (501) staff       (20)    14506 2024-04-25 07:57:38.000000 gio_importer-1.1.4/importers/db_import/mysql_import.py
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-25 08:01:43.212695 gio_importer-1.1.4/importers/example/
--rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-04-25 07:46:34.000000 gio_importer-1.1.4/importers/example/__init__.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     5144 2024-04-25 07:46:34.000000 gio_importer-1.1.4/importers/format_importer.py
--rw-r--r--   0 chengcheng   (501) staff       (20)      472 2024-04-25 07:46:34.000000 gio_importer-1.1.4/importers/log_conf.yaml
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-25 08:01:43.218063 gio_importer-1.1.4/importers/meta/
--rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-04-25 07:46:34.000000 gio_importer-1.1.4/importers/meta/__init__.py
--rw-r--r--   0 chengcheng   (501) staff       (20)    10172 2024-04-25 07:46:34.000000 gio_importer-1.1.4/importers/meta/check_util.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     7963 2024-04-25 07:46:34.000000 gio_importer-1.1.4/importers/meta/data_center.py
--rw-r--r--   0 chengcheng   (501) staff       (20)    21049 2024-04-25 07:46:34.000000 gio_importer-1.1.4/importers/meta/meta_create.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     4782 2024-04-25 07:46:34.000000 gio_importer-1.1.4/importers/meta_importer.py
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-25 08:01:43.219639 gio_importer-1.1.4/importers/saas_export/
--rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-04-25 07:46:34.000000 gio_importer-1.1.4/importers/saas_export/__init__.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     3303 2024-04-25 07:46:34.000000 gio_importer-1.1.4/importers/saas_export/saas_meta.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     1179 2024-04-25 07:46:34.000000 gio_importer-1.1.4/importers/saas_export.py
--rw-r--r--   0 chengcheng   (501) staff       (20)      232 2024-04-25 07:46:34.000000 gio_importer-1.1.4/importers/setup.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     1372 2024-04-25 07:46:34.000000 gio_importer-1.1.4/importers/trigger_job.py
--rw-r--r--   0 chengcheng   (501) staff       (20)       95 2024-04-25 07:46:34.000000 gio_importer-1.1.4/importers/zk.py
--rw-r--r--   0 chengcheng   (501) staff       (20)       38 2024-04-25 08:01:43.220621 gio_importer-1.1.4/setup.cfg
--rw-r--r--   0 chengcheng   (501) staff       (20)     1251 2024-04-25 08:01:07.000000 gio_importer-1.1.4/setup.py
+drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-25 08:11:31.738061 gio_importer-1.1.6/
+-rw-r--r--   0 chengcheng   (501) staff       (20)     1061 2024-04-25 07:46:34.000000 gio_importer-1.1.6/LICENSE
+-rw-r--r--   0 chengcheng   (501) staff       (20)       71 2024-04-25 07:46:34.000000 gio_importer-1.1.6/MANIFEST.in
+-rw-r--r--   0 chengcheng   (501) staff       (20)    12295 2024-04-25 08:11:31.737780 gio_importer-1.1.6/PKG-INFO
+-rw-r--r--   0 chengcheng   (501) staff       (20)      792 2024-04-25 07:46:34.000000 gio_importer-1.1.6/README.md
+drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-25 08:11:31.710390 gio_importer-1.1.6/gio_importer.egg-info/
+-rw-r--r--   0 chengcheng   (501) staff       (20)    12295 2024-04-25 08:11:31.000000 gio_importer-1.1.6/gio_importer.egg-info/PKG-INFO
+-rw-r--r--   0 chengcheng   (501) staff       (20)     1381 2024-04-25 08:11:31.000000 gio_importer-1.1.6/gio_importer.egg-info/SOURCES.txt
+-rw-r--r--   0 chengcheng   (501) staff       (20)        1 2024-04-25 08:11:31.000000 gio_importer-1.1.6/gio_importer.egg-info/dependency_links.txt
+-rw-r--r--   0 chengcheng   (501) staff       (20)      196 2024-04-25 08:11:31.000000 gio_importer-1.1.6/gio_importer.egg-info/entry_points.txt
+-rw-r--r--   0 chengcheng   (501) staff       (20)       84 2024-04-25 08:11:31.000000 gio_importer-1.1.6/gio_importer.egg-info/requires.txt
+-rw-r--r--   0 chengcheng   (501) staff       (20)       10 2024-04-25 08:11:31.000000 gio_importer-1.1.6/gio_importer.egg-info/top_level.txt
+drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-25 08:11:31.715422 gio_importer-1.1.6/importers/
+-rw-r--r--   0 chengcheng   (501) staff       (20)    11711 2024-04-25 07:46:34.000000 gio_importer-1.1.6/importers/README.md
+-rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-04-25 07:46:34.000000 gio_importer-1.1.6/importers/__init__.py
+drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-25 08:11:31.716199 gio_importer-1.1.6/importers/clear_data/
+-rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-04-25 07:46:34.000000 gio_importer-1.1.6/importers/clear_data/__init__.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     2779 2024-04-25 07:46:34.000000 gio_importer-1.1.6/importers/clear_data/clear_data.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     1714 2024-04-25 07:46:34.000000 gio_importer-1.1.6/importers/clear_user.py
+drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-25 08:11:31.718129 gio_importer-1.1.6/importers/common/
+-rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-04-25 07:46:34.000000 gio_importer-1.1.6/importers/common/__init__.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     5581 2024-04-25 07:46:34.000000 gio_importer-1.1.6/importers/common/common_util.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     2620 2024-04-25 07:46:34.000000 gio_importer-1.1.6/importers/common/config_util.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     2506 2024-04-25 07:46:34.000000 gio_importer-1.1.6/importers/common/http_util.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)      955 2024-04-25 07:46:34.000000 gio_importer-1.1.6/importers/common/log_util.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)      771 2024-04-25 07:46:34.000000 gio_importer-1.1.6/importers/conf.cfg
+drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-25 08:11:31.728214 gio_importer-1.1.6/importers/data_import/
+-rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-04-25 07:46:34.000000 gio_importer-1.1.6/importers/data_import/__init__.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)    21768 2024-04-25 07:46:34.000000 gio_importer-1.1.6/importers/data_import/data_ads.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)    21685 2024-04-25 07:46:34.000000 gio_importer-1.1.6/importers/data_import/data_events.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)    11251 2024-04-25 07:46:34.000000 gio_importer-1.1.6/importers/data_import/data_format_util.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)    17685 2024-04-25 07:46:34.000000 gio_importer-1.1.6/importers/data_import/data_item_variable.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     6455 2024-04-25 07:46:34.000000 gio_importer-1.1.6/importers/data_import/data_model.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)    15336 2024-04-25 07:46:34.000000 gio_importer-1.1.6/importers/data_import/data_user_variable.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     6943 2024-04-25 07:46:34.000000 gio_importer-1.1.6/importers/data_importer.py
+drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-25 08:11:31.731370 gio_importer-1.1.6/importers/db_import/
+-rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-04-25 07:46:34.000000 gio_importer-1.1.6/importers/db_import/__init__.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     2717 2024-04-25 07:46:34.000000 gio_importer-1.1.6/importers/db_import/database_import.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)    14400 2024-04-25 08:10:51.000000 gio_importer-1.1.6/importers/db_import/hive_import.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)    14506 2024-04-25 08:10:51.000000 gio_importer-1.1.6/importers/db_import/mysql_import.py
+drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-25 08:11:31.732174 gio_importer-1.1.6/importers/example/
+-rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-04-25 07:46:34.000000 gio_importer-1.1.6/importers/example/__init__.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     5144 2024-04-25 07:46:34.000000 gio_importer-1.1.6/importers/format_importer.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)      472 2024-04-25 07:46:34.000000 gio_importer-1.1.6/importers/log_conf.yaml
+drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-25 08:11:31.735210 gio_importer-1.1.6/importers/meta/
+-rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-04-25 07:46:34.000000 gio_importer-1.1.6/importers/meta/__init__.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)    10172 2024-04-25 07:46:34.000000 gio_importer-1.1.6/importers/meta/check_util.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     7963 2024-04-25 07:46:34.000000 gio_importer-1.1.6/importers/meta/data_center.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)    21049 2024-04-25 07:46:34.000000 gio_importer-1.1.6/importers/meta/meta_create.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     4782 2024-04-25 07:46:34.000000 gio_importer-1.1.6/importers/meta_importer.py
+drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-25 08:11:31.737222 gio_importer-1.1.6/importers/saas_export/
+-rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-04-25 07:46:34.000000 gio_importer-1.1.6/importers/saas_export/__init__.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     3303 2024-04-25 07:46:34.000000 gio_importer-1.1.6/importers/saas_export/saas_meta.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     1179 2024-04-25 07:46:34.000000 gio_importer-1.1.6/importers/saas_export.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)      232 2024-04-25 07:46:34.000000 gio_importer-1.1.6/importers/setup.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     1372 2024-04-25 07:46:34.000000 gio_importer-1.1.6/importers/trigger_job.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)       95 2024-04-25 07:46:34.000000 gio_importer-1.1.6/importers/zk.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)       38 2024-04-25 08:11:31.738112 gio_importer-1.1.6/setup.cfg
+-rw-r--r--   0 chengcheng   (501) staff       (20)     1251 2024-04-25 08:11:20.000000 gio_importer-1.1.6/setup.py
```

### Comparing `gio_importer-1.1.4/LICENSE` & `gio_importer-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gio_importer-1.1.4/PKG-INFO` & `gio_importer-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gio_importer
-Version: 1.1.4
+Version: 1.1.6
 Summary: GrowingIO Importer是GrowingIO CDP平台元数据创建和数据导入工具
 Author: gio
 Author-email: dev-growing@startdt.com
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gio_importer-1.1.4/README.md` & `gio_importer-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `gio_importer-1.1.4/gio_importer.egg-info/PKG-INFO` & `gio_importer-1.1.6/gio_importer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gio-importer
-Version: 1.1.4
+Version: 1.1.6
 Summary: GrowingIO Importer是GrowingIO CDP平台元数据创建和数据导入工具
 Author: gio
 Author-email: dev-growing@startdt.com
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gio_importer-1.1.4/gio_importer.egg-info/SOURCES.txt` & `gio_importer-1.1.6/gio_importer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gio_importer-1.1.4/importers/README.md` & `gio_importer-1.1.6/importers/README.md`

 * *Files identical despite different names*

### Comparing `gio_importer-1.1.4/importers/clear_data/clear_data.py` & `gio_importer-1.1.6/importers/clear_data/clear_data.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.1.4/importers/clear_user.py` & `gio_importer-1.1.6/importers/clear_user.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.1.4/importers/common/common_util.py` & `gio_importer-1.1.6/importers/common/common_util.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.1.4/importers/common/config_util.py` & `gio_importer-1.1.6/importers/common/config_util.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.1.4/importers/common/http_util.py` & `gio_importer-1.1.6/importers/common/http_util.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.1.4/importers/common/log_util.py` & `gio_importer-1.1.6/importers/common/log_util.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.1.4/importers/conf.cfg` & `gio_importer-1.1.6/importers/conf.cfg`

 * *Files identical despite different names*

### Comparing `gio_importer-1.1.4/importers/data_import/data_ads.py` & `gio_importer-1.1.6/importers/data_import/data_ads.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.1.4/importers/data_import/data_events.py` & `gio_importer-1.1.6/importers/data_import/data_events.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.1.4/importers/data_import/data_format_util.py` & `gio_importer-1.1.6/importers/data_import/data_format_util.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.1.4/importers/data_import/data_item_variable.py` & `gio_importer-1.1.6/importers/data_import/data_item_variable.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.1.4/importers/data_import/data_model.py` & `gio_importer-1.1.6/importers/data_import/data_model.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.1.4/importers/data_import/data_user_variable.py` & `gio_importer-1.1.6/importers/data_import/data_user_variable.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.1.4/importers/data_importer.py` & `gio_importer-1.1.6/importers/data_importer.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.1.4/importers/db_import/database_import.py` & `gio_importer-1.1.6/importers/db_import/database_import.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.1.4/importers/db_import/hive_import.py` & `gio_importer-1.1.6/importers/db_import/hive_import.py`

 * *Files 0% similar despite different names*

```diff
@@ -282,18 +282,18 @@
     try:
         wf = open(json_file_abs_path, 'w')
         cnt = 0
         count = 0
         while True:
             cnt += 1
             data = cursor.fetchmany(size=args.get('batch'))
-            if len(data) == 0 and cnt == 1 or not data:
+            if len(data) == 0 and cnt == 1:
                 logger.error("数据为空")
                 exit(-1)
-            elif len(data) == 0 and cnt > 1:
+            elif len(data) == 0 and cnt > 1 or not data:
                 my_logger.info(f"临时文件总共写入{count}条数据")
                 end_time = time.time()
                 cost_time = end_time - start_time
                 my_logger.info("读取SQL数据,写入临时文件耗时:%.3f秒" % cost_time)
                 if len(str(args.get('jobName'))) == 0 or args.get('jobName') is None:
                     job_name = f"Python_item_{time.strftime('%Y%m%d_%H%M%S', time.localtime(time.time()))}"
                 else:
```

### Comparing `gio_importer-1.1.4/importers/db_import/mysql_import.py` & `gio_importer-1.1.6/importers/db_import/mysql_import.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,18 +63,18 @@
         start_time = time.time()
         wf = open(json_file_abs_path, 'w')
         cnt = 0
         count = 0
         while True:
             batch = cursor.fetchmany(size=args.get('batch'))
             cnt += 1
-            if len(batch) == 0 and cnt == 1 or not batch:
+            if len(batch) == 0 and cnt == 1:
                 logger.error("数据为空")
                 exit(-1)
-            elif len(batch) == 0 and cnt > 1:
+            elif len(batch) == 0 and cnt > 1 or not batch:
                 end_time = time.time()
                 cost_time = end_time - start_time
                 my_logger.info("读取SQL数据,写入临时文件耗时:%.3f秒" % cost_time)
                 if len(str(args.get('jobName'))) == 0 or args.get('jobName') is None:
                     job_name = f"Python_events_{time.strftime('%Y%m%d_%H%M%S', time.localtime(time.time()))}"
                 else:
                     job_name = args.get('jobName')
```

### Comparing `gio_importer-1.1.4/importers/format_importer.py` & `gio_importer-1.1.6/importers/format_importer.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.1.4/importers/meta/check_util.py` & `gio_importer-1.1.6/importers/meta/check_util.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.1.4/importers/meta/data_center.py` & `gio_importer-1.1.6/importers/meta/data_center.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.1.4/importers/meta/meta_create.py` & `gio_importer-1.1.6/importers/meta/meta_create.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.1.4/importers/meta_importer.py` & `gio_importer-1.1.6/importers/meta_importer.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.1.4/importers/saas_export/saas_meta.py` & `gio_importer-1.1.6/importers/saas_export/saas_meta.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.1.4/importers/saas_export.py` & `gio_importer-1.1.6/importers/saas_export.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.1.4/importers/trigger_job.py` & `gio_importer-1.1.6/importers/trigger_job.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.1.4/setup.py` & `gio_importer-1.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     'pyhive',
     'thrift',
     'sasl'
 ]
 
 setup(
     name='gio_importer',
-    version='1.1.4',
+    version='1.1.6',
     description='GrowingIO Importer是GrowingIO CDP平台元数据创建和数据导入工具',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='gio',
     author_email='dev-growing@startdt.com',
     packages=find_packages(include=["importers*"]),
     include_package_data=True,
```

