# Comparing `tmp/qstd_core-0.2.2.tar.gz` & `tmp/qstd_core-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qstd_core-0.2.2.tar", last modified: Thu Apr 25 11:16:22 2024, max compression
+gzip compressed data, was "qstd_core-0.2.3.tar", last modified: Thu Apr 25 11:19:16 2024, max compression
```

## Comparing `qstd_core-0.2.2.tar` & `qstd_core-0.2.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-25 11:16:22.134508 qstd_core-0.2.2/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1054 2024-03-24 20:15:12.000000 qstd_core-0.2.2/LICENSE
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      362 2024-04-25 11:16:22.134508 qstd_core-0.2.2/PKG-INFO
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       42 2024-04-16 16:54:41.000000 qstd_core-0.2.2/README.md
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-25 11:16:22.130508 qstd_core-0.2.2/qstd_core/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      150 2024-04-16 15:25:55.000000 qstd_core-0.2.2/qstd_core/__init__.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-25 11:16:22.130508 qstd_core-0.2.2/qstd_core/exceptions/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       48 2024-04-16 16:15:44.000000 qstd_core-0.2.2/qstd_core/exceptions/__init__.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      830 2024-04-16 16:17:31.000000 qstd_core-0.2.2/qstd_core/exceptions/base.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1385 2024-04-16 16:17:31.000000 qstd_core-0.2.2/qstd_core/exceptions/localization.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-25 11:16:22.130508 qstd_core-0.2.2/qstd_core/localization/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2176 2024-04-16 16:33:14.000000 qstd_core-0.2.2/qstd_core/localization/__init__.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-25 11:16:22.130508 qstd_core-0.2.2/qstd_core/logger/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       69 2024-04-21 19:21:33.000000 qstd_core-0.2.2/qstd_core/logger/__init__.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-25 11:16:22.130508 qstd_core-0.2.2/qstd_core/marshmallow/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      177 2024-04-16 12:32:13.000000 qstd_core-0.2.2/qstd_core/marshmallow/__init__.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     5299 2024-03-13 13:59:27.000000 qstd_core-0.2.2/qstd_core/marshmallow/fields.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      465 2024-03-31 12:23:58.000000 qstd_core-0.2.2/qstd_core/marshmallow/schema.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2798 2024-03-31 12:24:08.000000 qstd_core-0.2.2/qstd_core/marshmallow/validate.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-25 11:16:22.130508 qstd_core-0.2.2/qstd_core/openapi/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       81 2024-03-31 12:25:01.000000 qstd_core-0.2.2/qstd_core/openapi/__init__.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     5616 2024-04-25 11:13:29.000000 qstd_core-0.2.2/qstd_core/openapi/decorators.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      244 2024-03-13 13:59:27.000000 qstd_core-0.2.2/qstd_core/openapi/enum.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     5368 2024-04-06 10:15:52.000000 qstd_core-0.2.2/qstd_core/openapi/mapper_marsmallow.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      238 2024-04-06 10:07:24.000000 qstd_core-0.2.2/qstd_core/openapi/mapper_pydantic.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      382 2024-03-31 12:25:14.000000 qstd_core-0.2.2/qstd_core/openapi/router.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     8925 2024-04-06 10:20:57.000000 qstd_core-0.2.2/qstd_core/openapi/spec.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     7459 2024-04-16 16:52:41.000000 qstd_core-0.2.2/qstd_core/openapi/utils.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-25 11:16:22.130508 qstd_core-0.2.2/qstd_core/sanic/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       22 2024-04-06 09:59:29.000000 qstd_core-0.2.2/qstd_core/sanic/__init__.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-25 11:16:22.130508 qstd_core-0.2.2/qstd_core/sanic/request/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      852 2024-04-16 16:31:39.000000 qstd_core-0.2.2/qstd_core/sanic/request/__init__.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-25 11:16:22.134508 qstd_core-0.2.2/qstd_core/sanic/server/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       20 2024-04-16 15:25:27.000000 qstd_core-0.2.2/qstd_core/sanic/server/__init__.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      319 2024-04-21 19:19:40.000000 qstd_core-0.2.2/qstd_core/sanic/server/utils.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-25 11:16:22.134508 qstd_core-0.2.2/qstd_core/validator/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2004 2024-04-25 11:10:45.000000 qstd_core-0.2.2/qstd_core/validator/ValidatorABS.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2334 2024-04-25 11:12:41.000000 qstd_core-0.2.2/qstd_core/validator/ValidatorMarshmallow.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1191 2024-04-25 11:11:00.000000 qstd_core-0.2.2/qstd_core/validator/ValidatorPydantic.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1834 2024-04-23 09:26:58.000000 qstd_core-0.2.2/qstd_core/validator/__init__.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      134 2024-04-21 19:14:09.000000 qstd_core-0.2.2/qstd_core/validator/enums.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1428 2024-04-21 19:14:09.000000 qstd_core-0.2.2/qstd_core/validator/exceptions.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      139 2024-04-16 14:18:23.000000 qstd_core-0.2.2/qstd_core/validator/types.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-25 11:16:22.130508 qstd_core-0.2.2/qstd_core.egg-info/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      362 2024-04-25 11:16:22.000000 qstd_core-0.2.2/qstd_core.egg-info/PKG-INFO
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1138 2024-04-25 11:16:22.000000 qstd_core-0.2.2/qstd_core.egg-info/SOURCES.txt
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)        1 2024-04-25 11:16:22.000000 qstd_core-0.2.2/qstd_core.egg-info/dependency_links.txt
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       82 2024-04-25 11:16:22.000000 qstd_core-0.2.2/qstd_core.egg-info/requires.txt
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       10 2024-04-25 11:16:22.000000 qstd_core-0.2.2/qstd_core.egg-info/top_level.txt
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       38 2024-04-25 11:16:22.134508 qstd_core-0.2.2/setup.cfg
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      734 2024-04-25 11:16:11.000000 qstd_core-0.2.2/setup.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-25 11:19:16.552635 qstd_core-0.2.3/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1054 2024-03-24 20:15:12.000000 qstd_core-0.2.3/LICENSE
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      362 2024-04-25 11:19:16.552635 qstd_core-0.2.3/PKG-INFO
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       42 2024-04-16 16:54:41.000000 qstd_core-0.2.3/README.md
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-25 11:19:16.548635 qstd_core-0.2.3/qstd_core/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      150 2024-04-16 15:25:55.000000 qstd_core-0.2.3/qstd_core/__init__.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-25 11:19:16.548635 qstd_core-0.2.3/qstd_core/exceptions/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       48 2024-04-16 16:15:44.000000 qstd_core-0.2.3/qstd_core/exceptions/__init__.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      830 2024-04-16 16:17:31.000000 qstd_core-0.2.3/qstd_core/exceptions/base.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1385 2024-04-16 16:17:31.000000 qstd_core-0.2.3/qstd_core/exceptions/localization.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-25 11:19:16.548635 qstd_core-0.2.3/qstd_core/localization/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2176 2024-04-16 16:33:14.000000 qstd_core-0.2.3/qstd_core/localization/__init__.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-25 11:19:16.548635 qstd_core-0.2.3/qstd_core/logger/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       69 2024-04-21 19:21:33.000000 qstd_core-0.2.3/qstd_core/logger/__init__.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-25 11:19:16.548635 qstd_core-0.2.3/qstd_core/marshmallow/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      177 2024-04-16 12:32:13.000000 qstd_core-0.2.3/qstd_core/marshmallow/__init__.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     5299 2024-03-13 13:59:27.000000 qstd_core-0.2.3/qstd_core/marshmallow/fields.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      465 2024-03-31 12:23:58.000000 qstd_core-0.2.3/qstd_core/marshmallow/schema.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2798 2024-03-31 12:24:08.000000 qstd_core-0.2.3/qstd_core/marshmallow/validate.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-25 11:19:16.552635 qstd_core-0.2.3/qstd_core/openapi/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       81 2024-03-31 12:25:01.000000 qstd_core-0.2.3/qstd_core/openapi/__init__.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     5616 2024-04-25 11:13:29.000000 qstd_core-0.2.3/qstd_core/openapi/decorators.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      244 2024-03-13 13:59:27.000000 qstd_core-0.2.3/qstd_core/openapi/enum.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     5368 2024-04-06 10:15:52.000000 qstd_core-0.2.3/qstd_core/openapi/mapper_marsmallow.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      238 2024-04-06 10:07:24.000000 qstd_core-0.2.3/qstd_core/openapi/mapper_pydantic.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      382 2024-03-31 12:25:14.000000 qstd_core-0.2.3/qstd_core/openapi/router.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     8925 2024-04-06 10:20:57.000000 qstd_core-0.2.3/qstd_core/openapi/spec.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     7459 2024-04-16 16:52:41.000000 qstd_core-0.2.3/qstd_core/openapi/utils.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-25 11:19:16.552635 qstd_core-0.2.3/qstd_core/sanic/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       22 2024-04-06 09:59:29.000000 qstd_core-0.2.3/qstd_core/sanic/__init__.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-25 11:19:16.552635 qstd_core-0.2.3/qstd_core/sanic/request/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      852 2024-04-16 16:31:39.000000 qstd_core-0.2.3/qstd_core/sanic/request/__init__.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-25 11:19:16.552635 qstd_core-0.2.3/qstd_core/sanic/server/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       20 2024-04-16 15:25:27.000000 qstd_core-0.2.3/qstd_core/sanic/server/__init__.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      319 2024-04-21 19:19:40.000000 qstd_core-0.2.3/qstd_core/sanic/server/utils.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-25 11:19:16.552635 qstd_core-0.2.3/qstd_core/validator/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2004 2024-04-25 11:10:45.000000 qstd_core-0.2.3/qstd_core/validator/ValidatorABS.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2334 2024-04-25 11:12:41.000000 qstd_core-0.2.3/qstd_core/validator/ValidatorMarshmallow.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1191 2024-04-25 11:11:00.000000 qstd_core-0.2.3/qstd_core/validator/ValidatorPydantic.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1834 2024-04-23 09:26:58.000000 qstd_core-0.2.3/qstd_core/validator/__init__.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      134 2024-04-21 19:14:09.000000 qstd_core-0.2.3/qstd_core/validator/enums.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1428 2024-04-21 19:14:09.000000 qstd_core-0.2.3/qstd_core/validator/exceptions.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      139 2024-04-16 14:18:23.000000 qstd_core-0.2.3/qstd_core/validator/types.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-25 11:19:16.548635 qstd_core-0.2.3/qstd_core.egg-info/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      362 2024-04-25 11:19:16.000000 qstd_core-0.2.3/qstd_core.egg-info/PKG-INFO
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1138 2024-04-25 11:19:16.000000 qstd_core-0.2.3/qstd_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)        1 2024-04-25 11:19:16.000000 qstd_core-0.2.3/qstd_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       82 2024-04-25 11:19:16.000000 qstd_core-0.2.3/qstd_core.egg-info/requires.txt
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       10 2024-04-25 11:19:16.000000 qstd_core-0.2.3/qstd_core.egg-info/top_level.txt
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       38 2024-04-25 11:19:16.552635 qstd_core-0.2.3/setup.cfg
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      734 2024-04-25 11:19:15.000000 qstd_core-0.2.3/setup.py
```

### Comparing `qstd_core-0.2.2/LICENSE` & `qstd_core-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qstd_core-0.2.2/qstd_core/exceptions/base.py` & `qstd_core-0.2.3/qstd_core/exceptions/base.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.2.2/qstd_core/exceptions/localization.py` & `qstd_core-0.2.3/qstd_core/exceptions/localization.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.2.2/qstd_core/localization/__init__.py` & `qstd_core-0.2.3/qstd_core/localization/__init__.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.2.2/qstd_core/marshmallow/fields.py` & `qstd_core-0.2.3/qstd_core/marshmallow/fields.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.2.2/qstd_core/marshmallow/validate.py` & `qstd_core-0.2.3/qstd_core/marshmallow/validate.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.2.2/qstd_core/openapi/decorators.py` & `qstd_core-0.2.3/qstd_core/openapi/decorators.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.2.2/qstd_core/openapi/mapper_marsmallow.py` & `qstd_core-0.2.3/qstd_core/openapi/mapper_marsmallow.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.2.2/qstd_core/openapi/spec.py` & `qstd_core-0.2.3/qstd_core/openapi/spec.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.2.2/qstd_core/openapi/utils.py` & `qstd_core-0.2.3/qstd_core/openapi/utils.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.2.2/qstd_core/sanic/request/__init__.py` & `qstd_core-0.2.3/qstd_core/sanic/request/__init__.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.2.2/qstd_core/validator/ValidatorABS.py` & `qstd_core-0.2.3/qstd_core/validator/ValidatorABS.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.2.2/qstd_core/validator/ValidatorMarshmallow.py` & `qstd_core-0.2.3/qstd_core/validator/ValidatorMarshmallow.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.2.2/qstd_core/validator/ValidatorPydantic.py` & `qstd_core-0.2.3/qstd_core/validator/ValidatorPydantic.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.2.2/qstd_core/validator/__init__.py` & `qstd_core-0.2.3/qstd_core/validator/__init__.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.2.2/qstd_core/validator/exceptions.py` & `qstd_core-0.2.3/qstd_core/validator/exceptions.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.2.2/qstd_core.egg-info/SOURCES.txt` & `qstd_core-0.2.3/qstd_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qstd_core-0.2.2/setup.py` & `qstd_core-0.2.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='qstd_core',
-    version='0.2.2',
+    version='0.2.3',
     author='QuisEgoSum',
     author_email='subbotin.evdokim@gmail.com',
     description='Application core based on sanic',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/QuisEgoSum/qstd-core',
     packages=find_packages(exclude=['tmp', 'example']),
```

