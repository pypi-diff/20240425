# Comparing `tmp/kitab-0.0.1.tar.gz` & `tmp/kitab-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kitab-0.0.1.tar", last modified: Wed Apr 24 22:03:28 2024, max compression
+gzip compressed data, was "kitab-0.0.2.tar", last modified: Thu Apr 25 06:25:06 2024, max compression
```

## Comparing `kitab-0.0.1.tar` & `kitab-0.0.2.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 22:03:28.839113 kitab-0.0.1/
--rw-rw-rw-   0        0        0     1100 2024-04-07 17:53:03.000000 kitab-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      324 2024-04-24 22:03:28.831809 kitab-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      770 2024-04-07 17:53:03.000000 kitab-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 22:03:28.724740 kitab-0.0.1/kitab/
--rw-rw-rw-   0        0        0      131 2024-04-08 06:51:45.000000 kitab-0.0.1/kitab/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 22:03:28.769506 kitab-0.0.1/kitab/api/
--rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.1/kitab/api/__init__.py
--rw-rw-rw-   0        0        0     7424 2024-04-24 20:41:38.000000 kitab-0.0.1/kitab/api/app.py
-drwxrwxrwx   0        0        0        0 2024-04-24 22:03:28.795436 kitab-0.0.1/kitab/db/
--rw-rw-rw-   0        0        0      370 2024-04-21 06:34:18.000000 kitab-0.0.1/kitab/db/__init__.py
--rw-rw-rw-   0        0        0     2119 2024-04-21 06:22:05.000000 kitab-0.0.1/kitab/db/db_info.py
--rw-rw-rw-   0        0        0    15561 2024-04-24 20:40:19.000000 kitab-0.0.1/kitab/db/functions.py
--rw-rw-rw-   0        0        0      798 2024-04-24 20:35:25.000000 kitab-0.0.1/kitab/db/get_data.py
--rw-rw-rw-   0        0        0    11876 2024-04-24 20:46:49.000000 kitab-0.0.1/kitab/db/sql_interactions.py
-drwxrwxrwx   0        0        0        0 2024-04-24 22:03:28.805965 kitab-0.0.1/kitab/logger/
--rw-rw-rw-   0        0        0       37 2024-04-07 17:53:03.000000 kitab-0.0.1/kitab/logger/__init__.py
--rw-rw-rw-   0        0        0     1737 2024-04-24 20:44:07.000000 kitab-0.0.1/kitab/logger/logger.py
-drwxrwxrwx   0        0        0        0 2024-04-24 22:03:28.814063 kitab-0.0.1/kitab/recommendation_model/
--rw-rw-rw-   0        0        0       88 2024-04-08 13:12:13.000000 kitab-0.0.1/kitab/recommendation_model/__init__.py
--rw-rw-rw-   0        0        0     4145 2024-04-24 20:42:55.000000 kitab-0.0.1/kitab/recommendation_model/models.py
--rw-rw-rw-   0        0        0     1544 2024-04-24 20:48:16.000000 kitab-0.0.1/kitab/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-24 22:03:28.828808 kitab-0.0.1/kitab.egg-info/
--rw-rw-rw-   0        0        0      324 2024-04-24 22:03:28.000000 kitab-0.0.1/kitab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      495 2024-04-24 22:03:28.000000 kitab-0.0.1/kitab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 22:03:28.000000 kitab-0.0.1/kitab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-24 22:03:28.000000 kitab-0.0.1/kitab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 22:03:28.841136 kitab-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      530 2024-04-24 22:02:30.000000 kitab-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-24 22:03:28.822802 kitab-0.0.1/tests/
--rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.1/tests/test_module1.py
--rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.1/tests/test_module2.py
+drwxrwxrwx   0        0        0        0 2024-04-25 06:25:06.028571 kitab-0.0.2/
+-rw-rw-rw-   0        0        0     1100 2024-04-07 17:53:03.000000 kitab-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      466 2024-04-25 06:25:06.028571 kitab-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      770 2024-04-07 17:53:03.000000 kitab-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 06:25:05.911872 kitab-0.0.2/kitab/
+-rw-rw-rw-   0        0        0      131 2024-04-08 06:51:45.000000 kitab-0.0.2/kitab/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 06:25:05.945117 kitab-0.0.2/kitab/api/
+-rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.2/kitab/api/__init__.py
+-rw-rw-rw-   0        0        0     7424 2024-04-24 20:41:38.000000 kitab-0.0.2/kitab/api/app.py
+drwxrwxrwx   0        0        0        0 2024-04-25 06:25:05.998492 kitab-0.0.2/kitab/db/
+-rw-rw-rw-   0        0        0      370 2024-04-21 06:34:18.000000 kitab-0.0.2/kitab/db/__init__.py
+-rw-rw-rw-   0        0        0     2119 2024-04-21 06:22:05.000000 kitab-0.0.2/kitab/db/db_info.py
+-rw-rw-rw-   0        0        0    15561 2024-04-24 20:40:19.000000 kitab-0.0.2/kitab/db/functions.py
+-rw-rw-rw-   0        0        0      798 2024-04-24 20:35:25.000000 kitab-0.0.2/kitab/db/get_data.py
+-rw-rw-rw-   0        0        0    11876 2024-04-24 20:46:49.000000 kitab-0.0.2/kitab/db/sql_interactions.py
+drwxrwxrwx   0        0        0        0 2024-04-25 06:25:06.012644 kitab-0.0.2/kitab/logger/
+-rw-rw-rw-   0        0        0       37 2024-04-07 17:53:03.000000 kitab-0.0.2/kitab/logger/__init__.py
+-rw-rw-rw-   0        0        0     1737 2024-04-24 20:44:07.000000 kitab-0.0.2/kitab/logger/logger.py
+drwxrwxrwx   0        0        0        0 2024-04-25 06:25:06.018592 kitab-0.0.2/kitab/recommendation_model/
+-rw-rw-rw-   0        0        0       88 2024-04-08 13:12:13.000000 kitab-0.0.2/kitab/recommendation_model/__init__.py
+-rw-rw-rw-   0        0        0     4145 2024-04-24 20:42:55.000000 kitab-0.0.2/kitab/recommendation_model/models.py
+-rw-rw-rw-   0        0        0     1544 2024-04-24 20:48:16.000000 kitab-0.0.2/kitab/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-25 06:25:06.028059 kitab-0.0.2/kitab.egg-info/
+-rw-rw-rw-   0        0        0      466 2024-04-25 06:25:05.000000 kitab-0.0.2/kitab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      523 2024-04-25 06:25:05.000000 kitab-0.0.2/kitab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 06:25:05.000000 kitab-0.0.2/kitab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-25 06:25:05.000000 kitab-0.0.2/kitab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-25 06:25:05.000000 kitab-0.0.2/kitab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 06:25:06.028571 kitab-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      580 2024-04-25 06:24:44.000000 kitab-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 06:25:06.025018 kitab-0.0.2/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.2/tests/test_module1.py
+-rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.2/tests/test_module2.py
```

### Comparing `kitab-0.0.1/LICENSE` & `kitab-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kitab-0.0.1/README.md` & `kitab-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `kitab-0.0.1/kitab/api/app.py` & `kitab-0.0.2/kitab/api/app.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.1/kitab/db/db_info.py` & `kitab-0.0.2/kitab/db/db_info.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.1/kitab/db/functions.py` & `kitab-0.0.2/kitab/db/functions.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.1/kitab/db/get_data.py` & `kitab-0.0.2/kitab/db/get_data.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.1/kitab/db/sql_interactions.py` & `kitab-0.0.2/kitab/db/sql_interactions.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.1/kitab/logger/logger.py` & `kitab-0.0.2/kitab/logger/logger.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.1/kitab/recommendation_model/models.py` & `kitab-0.0.2/kitab/recommendation_model/models.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.1/kitab/utils.py` & `kitab-0.0.2/kitab/utils.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.1/setup.py` & `kitab-0.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 # Add install requirements
 setup(
-    author="Alexander Shahramanyn",
+    author="Alexander Shahramanyan",
     description="A package for book recommendation.",
     name="kitab",
     packages=find_packages(include=["kitab", "kitab.*"]),
-    version="0.0.1",
+    version="0.0.2",
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
-    # install_requires=['numpy>=1.10', 'pandas'],
-    python_requires=">=3.7",
+    install_requires=['pandas', 'sentence-transformers>=2.6', 'psycopg2', 'pgvector', 'logging'],
+    python_requires=">=3.10",
 )
```

