# Comparing `tmp/kitab-0.0.4.tar.gz` & `tmp/kitab-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kitab-0.0.4.tar", last modified: Thu Apr 25 08:12:13 2024, max compression
+gzip compressed data, was "kitab-0.0.5.tar", last modified: Thu Apr 25 08:15:14 2024, max compression
```

## Comparing `kitab-0.0.4.tar` & `kitab-0.0.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 08:12:13.365378 kitab-0.0.4/
--rw-rw-rw-   0        0        0     1100 2024-04-07 17:53:03.000000 kitab-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      472 2024-04-25 08:12:13.360584 kitab-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      770 2024-04-07 17:53:03.000000 kitab-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 08:12:13.302805 kitab-0.0.4/kitab/
--rw-rw-rw-   0        0        0      131 2024-04-08 06:51:45.000000 kitab-0.0.4/kitab/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 08:12:13.326194 kitab-0.0.4/kitab/api/
--rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.4/kitab/api/__init__.py
--rw-rw-rw-   0        0        0     7424 2024-04-24 20:41:38.000000 kitab-0.0.4/kitab/api/app.py
-drwxrwxrwx   0        0        0        0 2024-04-25 08:12:13.339681 kitab-0.0.4/kitab/db/
--rw-rw-rw-   0        0        0      370 2024-04-21 06:34:18.000000 kitab-0.0.4/kitab/db/__init__.py
--rw-rw-rw-   0        0        0     2187 2024-04-25 07:42:15.000000 kitab-0.0.4/kitab/db/db_info.py
--rw-rw-rw-   0        0        0    15561 2024-04-24 20:40:19.000000 kitab-0.0.4/kitab/db/functions.py
--rw-rw-rw-   0        0        0     4982 2024-04-25 07:45:16.000000 kitab-0.0.4/kitab/db/get_data.py
--rw-rw-rw-   0        0        0    11876 2024-04-24 20:46:49.000000 kitab-0.0.4/kitab/db/sql_interactions.py
-drwxrwxrwx   0        0        0        0 2024-04-25 08:12:13.344515 kitab-0.0.4/kitab/logger/
--rw-rw-rw-   0        0        0       37 2024-04-07 17:53:03.000000 kitab-0.0.4/kitab/logger/__init__.py
--rw-rw-rw-   0        0        0     1737 2024-04-24 20:44:07.000000 kitab-0.0.4/kitab/logger/logger.py
-drwxrwxrwx   0        0        0        0 2024-04-25 08:12:13.350925 kitab-0.0.4/kitab/recommendation_model/
--rw-rw-rw-   0        0        0       88 2024-04-08 13:12:13.000000 kitab-0.0.4/kitab/recommendation_model/__init__.py
--rw-rw-rw-   0        0        0     4145 2024-04-24 20:42:55.000000 kitab-0.0.4/kitab/recommendation_model/models.py
--rw-rw-rw-   0        0        0     4568 2024-04-25 07:45:42.000000 kitab-0.0.4/kitab/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-25 08:12:13.358761 kitab-0.0.4/kitab.egg-info/
--rw-rw-rw-   0        0        0      472 2024-04-25 08:12:13.000000 kitab-0.0.4/kitab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      523 2024-04-25 08:12:13.000000 kitab-0.0.4/kitab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 08:12:13.000000 kitab-0.0.4/kitab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-04-25 08:12:13.000000 kitab-0.0.4/kitab.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-25 08:12:13.000000 kitab-0.0.4/kitab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 08:12:13.365378 kitab-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      586 2024-04-25 08:09:45.000000 kitab-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 08:12:13.356028 kitab-0.0.4/tests/
--rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.4/tests/test_module1.py
--rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.4/tests/test_module2.py
+drwxrwxrwx   0        0        0        0 2024-04-25 08:15:14.667136 kitab-0.0.5/
+-rw-rw-rw-   0        0        0     1100 2024-04-07 17:53:03.000000 kitab-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      448 2024-04-25 08:15:14.664557 kitab-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      770 2024-04-07 17:53:03.000000 kitab-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 08:15:14.604807 kitab-0.0.5/kitab/
+-rw-rw-rw-   0        0        0      131 2024-04-08 06:51:45.000000 kitab-0.0.5/kitab/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 08:15:14.621039 kitab-0.0.5/kitab/api/
+-rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.5/kitab/api/__init__.py
+-rw-rw-rw-   0        0        0     7424 2024-04-24 20:41:38.000000 kitab-0.0.5/kitab/api/app.py
+drwxrwxrwx   0        0        0        0 2024-04-25 08:15:14.637996 kitab-0.0.5/kitab/db/
+-rw-rw-rw-   0        0        0      370 2024-04-21 06:34:18.000000 kitab-0.0.5/kitab/db/__init__.py
+-rw-rw-rw-   0        0        0     2187 2024-04-25 07:42:15.000000 kitab-0.0.5/kitab/db/db_info.py
+-rw-rw-rw-   0        0        0    15561 2024-04-24 20:40:19.000000 kitab-0.0.5/kitab/db/functions.py
+-rw-rw-rw-   0        0        0     4982 2024-04-25 07:45:16.000000 kitab-0.0.5/kitab/db/get_data.py
+-rw-rw-rw-   0        0        0    11876 2024-04-24 20:46:49.000000 kitab-0.0.5/kitab/db/sql_interactions.py
+drwxrwxrwx   0        0        0        0 2024-04-25 08:15:14.647307 kitab-0.0.5/kitab/logger/
+-rw-rw-rw-   0        0        0       37 2024-04-07 17:53:03.000000 kitab-0.0.5/kitab/logger/__init__.py
+-rw-rw-rw-   0        0        0     1737 2024-04-24 20:44:07.000000 kitab-0.0.5/kitab/logger/logger.py
+drwxrwxrwx   0        0        0        0 2024-04-25 08:15:14.651127 kitab-0.0.5/kitab/recommendation_model/
+-rw-rw-rw-   0        0        0       88 2024-04-08 13:12:13.000000 kitab-0.0.5/kitab/recommendation_model/__init__.py
+-rw-rw-rw-   0        0        0     4145 2024-04-24 20:42:55.000000 kitab-0.0.5/kitab/recommendation_model/models.py
+-rw-rw-rw-   0        0        0     4568 2024-04-25 07:45:42.000000 kitab-0.0.5/kitab/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-25 08:15:14.654666 kitab-0.0.5/kitab.egg-info/
+-rw-rw-rw-   0        0        0      448 2024-04-25 08:15:14.000000 kitab-0.0.5/kitab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      523 2024-04-25 08:15:14.000000 kitab-0.0.5/kitab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 08:15:14.000000 kitab-0.0.5/kitab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2024-04-25 08:15:14.000000 kitab-0.0.5/kitab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-25 08:15:14.000000 kitab-0.0.5/kitab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 08:15:14.667136 kitab-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      575 2024-04-25 08:14:54.000000 kitab-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 08:15:14.654666 kitab-0.0.5/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.5/tests/test_module1.py
+-rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.5/tests/test_module2.py
```

### Comparing `kitab-0.0.4/LICENSE` & `kitab-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kitab-0.0.4/README.md` & `kitab-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `kitab-0.0.4/kitab/api/app.py` & `kitab-0.0.5/kitab/api/app.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.4/kitab/db/db_info.py` & `kitab-0.0.5/kitab/db/db_info.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.4/kitab/db/functions.py` & `kitab-0.0.5/kitab/db/functions.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.4/kitab/db/get_data.py` & `kitab-0.0.5/kitab/db/get_data.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.4/kitab/db/sql_interactions.py` & `kitab-0.0.5/kitab/db/sql_interactions.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.4/kitab/logger/logger.py` & `kitab-0.0.5/kitab/logger/logger.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.4/kitab/recommendation_model/models.py` & `kitab-0.0.5/kitab/recommendation_model/models.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.4/kitab/utils.py` & `kitab-0.0.5/kitab/utils.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.4/kitab.egg-info/SOURCES.txt` & `kitab-0.0.5/kitab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kitab-0.0.4/setup.py` & `kitab-0.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 # Add install requirements
 setup(
     author="Alexander Shahramanyan",
     description="A package for book recommendation.",
     name="kitab",
     packages=find_packages(include=["kitab", "kitab.*"]),
-    version="0.0.4",
+    version="0.0.5",
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
-    install_requires=['pandas', 'sentence-transformers>=2.6', 'psycopg2-binary', 'pgvector', 'logging'],
+    install_requires=['pandas', 'sentence-transformers>=2.6', 'psycopg2-binary', 'pgvector'],
     python_requires=">=3.7",
 )
```

