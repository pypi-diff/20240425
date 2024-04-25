# Comparing `tmp/hermitage_alchemy-0.1.2.tar.gz` & `tmp/hermitage_alchemy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hermitage_alchemy-0.1.2.tar", max compression
+gzip compressed data, was "hermitage_alchemy-0.1.3.tar", max compression
```

## Comparing `hermitage_alchemy-0.1.2.tar` & `hermitage_alchemy-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      120 2024-04-15 11:40:18.155284 hermitage_alchemy-0.1.2/README.md
--rw-r--r--   0        0        0      609 2024-04-02 15:23:42.890138 hermitage_alchemy-0.1.2/hermitage_alchemy/__init__.py
--rw-r--r--   0        0        0    10395 2024-04-13 13:59:52.794872 hermitage_alchemy-0.1.2/hermitage_alchemy/assembling.py
--rw-r--r--   0        0        0      826 2024-04-13 14:00:09.650913 hermitage_alchemy-0.1.2/hermitage_alchemy/bootstraping.py
--rw-r--r--   0        0        0     6903 2024-04-02 15:23:42.890449 hermitage_alchemy-0.1.2/hermitage_alchemy/configuration.py
--rw-r--r--   0        0        0        0 2024-04-02 15:23:42.890486 hermitage_alchemy-0.1.2/hermitage_alchemy/definition/__init__.py
--rw-r--r--   0        0        0     2762 2024-04-13 13:56:13.202035 hermitage_alchemy-0.1.2/hermitage_alchemy/definition/contracts.py
--rw-r--r--   0        0        0      660 2024-04-02 15:23:42.890980 hermitage_alchemy-0.1.2/hermitage_alchemy/definition/exceptions.py
--rw-r--r--   0        0        0        1 2024-04-02 15:23:42.891065 hermitage_alchemy-0.1.2/hermitage_alchemy/execution/__init__.py
--rw-r--r--   0        0        0     6217 2024-04-13 13:58:57.410241 hermitage_alchemy-0.1.2/hermitage_alchemy/execution/fetching.py
--rw-r--r--   0        0        0     3929 2024-04-13 13:58:57.403359 hermitage_alchemy-0.1.2/hermitage_alchemy/execution/storing.py
--rw-r--r--   0        0        0       97 2024-04-02 15:23:42.891391 hermitage_alchemy-0.1.2/hermitage_alchemy/plugins/__init__.py
--rw-r--r--   0        0        0      251 2024-04-02 15:23:42.891483 hermitage_alchemy-0.1.2/hermitage_alchemy/plugins/generic.py
--rw-r--r--   0        0        0     1163 2024-04-02 15:23:42.891584 hermitage_alchemy-0.1.2/hermitage_alchemy/plugins/total.py
--rw-r--r--   0        0        0      907 2024-04-11 15:13:54.800420 hermitage_alchemy-0.1.2/hermitage_alchemy/plugins/upsert.py
--rw-r--r--   0        0        0      416 2024-04-15 11:39:16.867361 hermitage_alchemy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      602 1970-01-01 00:00:00.000000 hermitage_alchemy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      120 2024-04-15 11:40:18.155284 hermitage_alchemy-0.1.3/README.md
+-rw-r--r--   0        0        0      609 2024-04-02 15:23:42.890138 hermitage_alchemy-0.1.3/hermitage_alchemy/__init__.py
+-rw-r--r--   0        0        0    10395 2024-04-13 13:59:52.794872 hermitage_alchemy-0.1.3/hermitage_alchemy/assembling.py
+-rw-r--r--   0        0        0      826 2024-04-13 14:00:09.650913 hermitage_alchemy-0.1.3/hermitage_alchemy/bootstraping.py
+-rw-r--r--   0        0        0     6903 2024-04-02 15:23:42.890449 hermitage_alchemy-0.1.3/hermitage_alchemy/configuration.py
+-rw-r--r--   0        0        0        0 2024-04-02 15:23:42.890486 hermitage_alchemy-0.1.3/hermitage_alchemy/definition/__init__.py
+-rw-r--r--   0        0        0     2762 2024-04-13 13:56:13.202035 hermitage_alchemy-0.1.3/hermitage_alchemy/definition/contracts.py
+-rw-r--r--   0        0        0      660 2024-04-02 15:23:42.890980 hermitage_alchemy-0.1.3/hermitage_alchemy/definition/exceptions.py
+-rw-r--r--   0        0        0        1 2024-04-02 15:23:42.891065 hermitage_alchemy-0.1.3/hermitage_alchemy/execution/__init__.py
+-rw-r--r--   0        0        0     6217 2024-04-13 13:58:57.410241 hermitage_alchemy-0.1.3/hermitage_alchemy/execution/fetching.py
+-rw-r--r--   0        0        0     3929 2024-04-13 13:58:57.403359 hermitage_alchemy-0.1.3/hermitage_alchemy/execution/storing.py
+-rw-r--r--   0        0        0       97 2024-04-02 15:23:42.891391 hermitage_alchemy-0.1.3/hermitage_alchemy/plugins/__init__.py
+-rw-r--r--   0        0        0      251 2024-04-02 15:23:42.891483 hermitage_alchemy-0.1.3/hermitage_alchemy/plugins/generic.py
+-rw-r--r--   0        0        0     1163 2024-04-02 15:23:42.891584 hermitage_alchemy-0.1.3/hermitage_alchemy/plugins/total.py
+-rw-r--r--   0        0        0      907 2024-04-11 15:13:54.800420 hermitage_alchemy-0.1.3/hermitage_alchemy/plugins/upsert.py
+-rw-r--r--   0        0        0      416 2024-04-25 11:51:48.129530 hermitage_alchemy-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      602 1970-01-01 00:00:00.000000 hermitage_alchemy-0.1.3/PKG-INFO
```

### Comparing `hermitage_alchemy-0.1.2/hermitage_alchemy/__init__.py` & `hermitage_alchemy-0.1.3/hermitage_alchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.1.2/hermitage_alchemy/assembling.py` & `hermitage_alchemy-0.1.3/hermitage_alchemy/assembling.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.1.2/hermitage_alchemy/bootstraping.py` & `hermitage_alchemy-0.1.3/hermitage_alchemy/bootstraping.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.1.2/hermitage_alchemy/configuration.py` & `hermitage_alchemy-0.1.3/hermitage_alchemy/configuration.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.1.2/hermitage_alchemy/definition/contracts.py` & `hermitage_alchemy-0.1.3/hermitage_alchemy/definition/contracts.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.1.2/hermitage_alchemy/definition/exceptions.py` & `hermitage_alchemy-0.1.3/hermitage_alchemy/definition/exceptions.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.1.2/hermitage_alchemy/execution/fetching.py` & `hermitage_alchemy-0.1.3/hermitage_alchemy/execution/fetching.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.1.2/hermitage_alchemy/execution/storing.py` & `hermitage_alchemy-0.1.3/hermitage_alchemy/execution/storing.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.1.2/hermitage_alchemy/plugins/total.py` & `hermitage_alchemy-0.1.3/hermitage_alchemy/plugins/total.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.1.2/hermitage_alchemy/plugins/upsert.py` & `hermitage_alchemy-0.1.3/hermitage_alchemy/plugins/upsert.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.1.2/PKG-INFO` & `hermitage_alchemy-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: hermitage-alchemy
-Version: 0.1.2
+Version: 0.1.3
 Summary: Implementation of hermitage contracts for sqlalchemy engine
 Author: Smairon
 Author-email: man@smairon.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: hermitage (>=0.1.0,<0.2.0)
+Requires-Dist: hermitage (>=0.1.4,<0.2.0)
 Requires-Dist: sqlalchemy (>=2.0.20,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Hermitage Alchemy
 
 Implementation of [hermitage](https://github.com/smairon/hermitage) contracts for sqlalchemy engine
```

