# Comparing `tmp/mo_sql-4.603.24115.tar.gz` & `tmp/mo_sql-4.605.24115.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo_sql-4.603.24115.tar", last modified: Wed Apr 24 11:34:48 2024, max compression
+gzip compressed data, was "mo_sql-4.605.24115.tar", last modified: Wed Apr 24 22:40:49 2024, max compression
```

## Comparing `mo_sql-4.603.24115.tar` & `mo_sql-4.605.24115.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 11:34:48.232913 mo_sql-4.603.24115/
--rw-rw-rw-   0        0        0    16725 2020-01-28 21:55:32.000000 mo_sql-4.603.24115/LICENSE
--rw-rw-rw-   0        0        0     1478 2024-04-24 11:34:48.231627 mo_sql-4.603.24115/PKG-INFO
--rw-rw-rw-   0        0        0      324 2024-01-20 19:08:03.000000 mo_sql-4.603.24115/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 11:34:48.220173 mo_sql-4.603.24115/mo_sql/
--rw-rw-rw-   0        0        0     7604 2024-03-21 02:38:31.000000 mo_sql-4.603.24115/mo_sql/__init__.py
--rw-rw-rw-   0        0        0     5460 2024-03-17 15:14:27.000000 mo_sql-4.603.24115/mo_sql/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-24 11:34:48.230553 mo_sql-4.603.24115/mo_sql.egg-info/
--rw-rw-rw-   0        0        0     1478 2024-04-24 11:34:48.000000 mo_sql-4.603.24115/mo_sql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2024-04-24 11:34:48.000000 mo_sql-4.603.24115/mo_sql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 11:34:48.000000 mo_sql-4.603.24115/mo_sql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2024-04-24 11:34:48.000000 mo_sql-4.603.24115/mo_sql.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-24 11:34:48.000000 mo_sql-4.603.24115/mo_sql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 11:34:48.232913 mo_sql-4.603.24115/setup.cfg
--rw-rw-rw-   0        0        0     1468 2024-04-24 11:34:43.000000 mo_sql-4.603.24115/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:40:49.595694 mo_sql-4.605.24115/
+-rw-rw-rw-   0        0        0    16725 2020-01-28 21:55:32.000000 mo_sql-4.605.24115/LICENSE
+-rw-rw-rw-   0        0        0     1478 2024-04-24 22:40:49.595694 mo_sql-4.605.24115/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2024-01-20 19:08:03.000000 mo_sql-4.605.24115/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 22:40:49.584232 mo_sql-4.605.24115/mo_sql/
+-rw-rw-rw-   0        0        0     7604 2024-03-21 02:38:31.000000 mo_sql-4.605.24115/mo_sql/__init__.py
+-rw-rw-rw-   0        0        0     5460 2024-03-17 15:14:27.000000 mo_sql-4.605.24115/mo_sql/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:40:49.593170 mo_sql-4.605.24115/mo_sql.egg-info/
+-rw-rw-rw-   0        0        0     1478 2024-04-24 22:40:49.000000 mo_sql-4.605.24115/mo_sql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2024-04-24 22:40:49.000000 mo_sql-4.605.24115/mo_sql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 22:40:49.000000 mo_sql-4.605.24115/mo_sql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2024-04-24 22:40:49.000000 mo_sql-4.605.24115/mo_sql.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-24 22:40:49.000000 mo_sql-4.605.24115/mo_sql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 22:40:49.595694 mo_sql-4.605.24115/setup.cfg
+-rw-rw-rw-   0        0        0     1468 2024-04-24 22:40:44.000000 mo_sql-4.605.24115/setup.py
```

### Comparing `mo_sql-4.603.24115/LICENSE` & `mo_sql-4.605.24115/LICENSE`

 * *Files identical despite different names*

### Comparing `mo_sql-4.603.24115/PKG-INFO` & `mo_sql-4.605.24115/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-sql
-Version: 4.603.24115
+Version: 4.605.24115
 Summary: More SQL!  For safely assembling SQL
 Home-page: https://github.com/klahnakoski/mo-sql
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
@@ -16,18 +16,18 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-dots==9.603.24115
+Requires-Dist: mo-dots==9.605.24115
 Requires-Dist: mo-future==7.584.24095
-Requires-Dist: mo-json==6.603.24115
-Requires-Dist: mo-logs==8.603.24115
+Requires-Dist: mo-json==6.605.24115
+Requires-Dist: mo-logs==8.605.24115
 Provides-Extra: tests
 Requires-Dist: mo-testing>=8.591.24112; extra == "tests"
 
 # More SQL!
 
 A number of generator functions for type-safe SQL composition.
```

### Comparing `mo_sql-4.603.24115/mo_sql/__init__.py` & `mo_sql-4.605.24115/mo_sql/__init__.py`

 * *Files identical despite different names*

### Comparing `mo_sql-4.603.24115/mo_sql/utils.py` & `mo_sql-4.605.24115/mo_sql/utils.py`

 * *Files identical despite different names*

### Comparing `mo_sql-4.603.24115/mo_sql.egg-info/PKG-INFO` & `mo_sql-4.605.24115/mo_sql.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-sql
-Version: 4.603.24115
+Version: 4.605.24115
 Summary: More SQL!  For safely assembling SQL
 Home-page: https://github.com/klahnakoski/mo-sql
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
@@ -16,18 +16,18 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-dots==9.603.24115
+Requires-Dist: mo-dots==9.605.24115
 Requires-Dist: mo-future==7.584.24095
-Requires-Dist: mo-json==6.603.24115
-Requires-Dist: mo-logs==8.603.24115
+Requires-Dist: mo-json==6.605.24115
+Requires-Dist: mo-logs==8.605.24115
 Provides-Extra: tests
 Requires-Dist: mo-testing>=8.591.24112; extra == "tests"
 
 # More SQL!
 
 A number of generator functions for type-safe SQL composition.
```

### Comparing `mo_sql-4.603.24115/setup.py` & `mo_sql-4.605.24115/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 setup(
     author='Kyle Lahnakoski',
     author_email='kyle@lahnakoski.com',
     classifiers=["Development Status :: 4 - Beta","Topic :: Software Development :: Libraries","Topic :: Software Development :: Libraries :: Python Modules","License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)","Topic :: Database","Topic :: Utilities","Programming Language :: SQL","Programming Language :: Python :: 3.8","Programming Language :: Python :: 3.9","Programming Language :: Python :: 3.10","Programming Language :: Python :: 3.11","Programming Language :: Python :: 3.12"],
     description='More SQL!  For safely assembling SQL',
     extras_require={"tests":["mo-testing>=8.591.24112"]},
     include_package_data=True,
-    install_requires=["mo-dots==9.603.24115","mo-future==7.584.24095","mo-json==6.603.24115","mo-logs==8.603.24115"],
+    install_requires=["mo-dots==9.605.24115","mo-future==7.584.24095","mo-json==6.605.24115","mo-logs==8.605.24115"],
     license='MPL 2.0',
     long_description='# More SQL!\n\nA number of generator functions for type-safe SQL composition.\n\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/jx-sqlite.svg)](https://pypi.org/project/mo-sql/)\n[![Build Status](https://app.travis-ci.com/klahnakoski/mo-sql.svg?branch=master)](https://travis-ci.com/github/klahnakoski/mo-sql)\n\n## Summary',
     long_description_content_type='text/markdown',
     name='mo-sql',
     packages=["mo_sql"],
     url='https://github.com/klahnakoski/mo-sql',
-    version='4.603.24115'
+    version='4.605.24115'
 )
```
