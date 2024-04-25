# Comparing `tmp/pyhasura-1.0.3.tar.gz` & `tmp/pyhasura-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhasura-1.0.3.tar", last modified: Sat Apr 20 12:51:01 2024, max compression
+gzip compressed data, was "pyhasura-1.0.4.tar", last modified: Thu Apr 25 13:22:11 2024, max compression
```

## Comparing `pyhasura-1.0.3.tar` & `pyhasura-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-20 12:51:01.919523 pyhasura-1.0.3/
--rw-r--r--   0 kennethstott   (501) staff       (20)     1065 2024-04-20 12:02:03.000000 pyhasura-1.0.3/LICENSE
--rw-r--r--   0 kennethstott   (501) staff       (20)     3545 2024-04-20 12:51:01.919300 pyhasura-1.0.3/PKG-INFO
--rw-r--r--   0 kennethstott   (501) staff       (20)     2967 2024-04-19 21:24:41.000000 pyhasura-1.0.3/README.md
-drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-20 12:51:01.917891 pyhasura-1.0.3/pyhasura/
--rw-r--r--   0 kennethstott   (501) staff       (20)      136 2024-04-19 18:25:03.000000 pyhasura-1.0.3/pyhasura/__init__.py
--rw-r--r--   0 kennethstott   (501) staff       (20)      745 2024-04-19 10:52:53.000000 pyhasura-1.0.3/pyhasura/flatten_dict.py
--rw-r--r--   0 kennethstott   (501) staff       (20)      359 2024-04-20 12:07:08.000000 pyhasura-1.0.3/pyhasura/gql_client.py
--rw-r--r--   0 kennethstott   (501) staff       (20)    13008 2024-04-19 21:13:47.000000 pyhasura-1.0.3/pyhasura/hasura_client.py
-drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-20 12:51:01.919037 pyhasura-1.0.3/pyhasura.egg-info/
--rw-r--r--   0 kennethstott   (501) staff       (20)     3545 2024-04-20 12:51:01.000000 pyhasura-1.0.3/pyhasura.egg-info/PKG-INFO
--rw-r--r--   0 kennethstott   (501) staff       (20)      295 2024-04-20 12:51:01.000000 pyhasura-1.0.3/pyhasura.egg-info/SOURCES.txt
--rw-r--r--   0 kennethstott   (501) staff       (20)        1 2024-04-20 12:51:01.000000 pyhasura-1.0.3/pyhasura.egg-info/dependency_links.txt
--rw-r--r--   0 kennethstott   (501) staff       (20)       82 2024-04-20 12:51:01.000000 pyhasura-1.0.3/pyhasura.egg-info/requires.txt
--rw-r--r--   0 kennethstott   (501) staff       (20)        9 2024-04-20 12:51:01.000000 pyhasura-1.0.3/pyhasura.egg-info/top_level.txt
--rw-r--r--   0 kennethstott   (501) staff       (20)      711 2024-04-20 12:50:35.000000 pyhasura-1.0.3/pyproject.toml
--rw-r--r--   0 kennethstott   (501) staff       (20)       38 2024-04-20 12:51:01.919684 pyhasura-1.0.3/setup.cfg
--rw-r--r--   0 kennethstott   (501) staff       (20)      427 2024-04-20 12:22:29.000000 pyhasura-1.0.3/setup.py
+drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-25 13:22:11.219079 pyhasura-1.0.4/
+-rw-r--r--   0 kennethstott   (501) staff       (20)     1065 2024-04-20 12:02:03.000000 pyhasura-1.0.4/LICENSE
+-rw-r--r--   0 kennethstott   (501) staff       (20)     3545 2024-04-25 13:22:11.218865 pyhasura-1.0.4/PKG-INFO
+-rw-r--r--   0 kennethstott   (501) staff       (20)     2967 2024-04-19 21:24:41.000000 pyhasura-1.0.4/README.md
+drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-25 13:22:11.217671 pyhasura-1.0.4/pyhasura/
+-rw-r--r--   0 kennethstott   (501) staff       (20)      136 2024-04-19 18:25:03.000000 pyhasura-1.0.4/pyhasura/__init__.py
+-rw-r--r--   0 kennethstott   (501) staff       (20)      745 2024-04-19 10:52:53.000000 pyhasura-1.0.4/pyhasura/flatten_dict.py
+-rw-r--r--   0 kennethstott   (501) staff       (20)      359 2024-04-20 12:07:08.000000 pyhasura-1.0.4/pyhasura/gql_client.py
+-rw-r--r--   0 kennethstott   (501) staff       (20)    13008 2024-04-19 21:13:47.000000 pyhasura-1.0.4/pyhasura/hasura_client.py
+drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-25 13:22:11.218581 pyhasura-1.0.4/pyhasura.egg-info/
+-rw-r--r--   0 kennethstott   (501) staff       (20)     3545 2024-04-25 13:22:11.000000 pyhasura-1.0.4/pyhasura.egg-info/PKG-INFO
+-rw-r--r--   0 kennethstott   (501) staff       (20)      295 2024-04-25 13:22:11.000000 pyhasura-1.0.4/pyhasura.egg-info/SOURCES.txt
+-rw-r--r--   0 kennethstott   (501) staff       (20)        1 2024-04-25 13:22:11.000000 pyhasura-1.0.4/pyhasura.egg-info/dependency_links.txt
+-rw-r--r--   0 kennethstott   (501) staff       (20)       82 2024-04-25 13:22:11.000000 pyhasura-1.0.4/pyhasura.egg-info/requires.txt
+-rw-r--r--   0 kennethstott   (501) staff       (20)        9 2024-04-25 13:22:11.000000 pyhasura-1.0.4/pyhasura.egg-info/top_level.txt
+-rw-r--r--   0 kennethstott   (501) staff       (20)      711 2024-04-20 12:50:35.000000 pyhasura-1.0.4/pyproject.toml
+-rw-r--r--   0 kennethstott   (501) staff       (20)       38 2024-04-25 13:22:11.219164 pyhasura-1.0.4/setup.cfg
+-rw-r--r--   0 kennethstott   (501) staff       (20)      427 2024-04-20 12:22:29.000000 pyhasura-1.0.4/setup.py
```

### Comparing `pyhasura-1.0.3/LICENSE` & `pyhasura-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhasura-1.0.3/PKG-INFO` & `pyhasura-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhasura
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python library to simplify Hasura, GraphQL and Machine Learning
 Author-email: Kenneth Stott <ken@kenstott.com>
 Project-URL: repository, https://github.com/kenstott/pyhasura
 Keywords: graphql,hasura,ml,ai,machine learning,arrow
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyhasura-1.0.3/README.md` & `pyhasura-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyhasura-1.0.3/pyhasura/flatten_dict.py` & `pyhasura-1.0.4/pyhasura/flatten_dict.py`

 * *Files identical despite different names*

### Comparing `pyhasura-1.0.3/pyhasura/hasura_client.py` & `pyhasura-1.0.4/pyhasura/hasura_client.py`

 * *Files identical despite different names*

### Comparing `pyhasura-1.0.3/pyhasura.egg-info/PKG-INFO` & `pyhasura-1.0.4/pyhasura.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhasura
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python library to simplify Hasura, GraphQL and Machine Learning
 Author-email: Kenneth Stott <ken@kenstott.com>
 Project-URL: repository, https://github.com/kenstott/pyhasura
 Keywords: graphql,hasura,ml,ai,machine learning,arrow
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyhasura-1.0.3/pyproject.toml` & `pyhasura-1.0.4/pyproject.toml`

 * *Files identical despite different names*

