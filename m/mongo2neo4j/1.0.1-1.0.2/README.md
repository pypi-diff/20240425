# Comparing `tmp/mongo2neo4j-1.0.1.tar.gz` & `tmp/mongo2neo4j-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongo2neo4j-1.0.1.tar", last modified: Wed Apr 24 15:56:56 2024, max compression
+gzip compressed data, was "mongo2neo4j-1.0.2.tar", last modified: Thu Apr 25 17:15:40 2024, max compression
```

## Comparing `mongo2neo4j-1.0.1.tar` & `mongo2neo4j-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 luther     (501) staff       (20)        0 2024-04-24 15:56:56.776553 mongo2neo4j-1.0.1/
--rw-r--r--   0 luther     (501) staff       (20)    35821 2023-08-05 21:05:58.000000 mongo2neo4j-1.0.1/LICENSE
--rw-r--r--   0 luther     (501) staff       (20)    46256 2024-04-24 15:56:56.775457 mongo2neo4j-1.0.1/PKG-INFO
--rw-r--r--   0 luther     (501) staff       (20)     4347 2023-09-28 10:35:23.000000 mongo2neo4j-1.0.1/README.md
--rw-r--r--   0 luther     (501) staff       (20)     6987 2024-04-22 12:53:21.000000 mongo2neo4j-1.0.1/pyproject.toml
--rw-r--r--   0 luther     (501) staff       (20)      170 2024-04-19 13:47:32.000000 mongo2neo4j-1.0.1/requirements-dev.txt
--rw-r--r--   0 luther     (501) staff       (20)       29 2024-04-16 11:28:39.000000 mongo2neo4j-1.0.1/requirements.txt
--rw-r--r--   0 luther     (501) staff       (20)       38 2024-04-24 15:56:56.776751 mongo2neo4j-1.0.1/setup.cfg
-drwxr-xr-x   0 luther     (501) staff       (20)        0 2024-04-24 15:56:56.758468 mongo2neo4j-1.0.1/src/
-drwxr-xr-x   0 luther     (501) staff       (20)        0 2024-04-24 15:56:56.762651 mongo2neo4j-1.0.1/src/mongo2neo4j/
--rw-rw-r--   0 luther     (501) staff       (20)    50723 2024-04-24 15:56:27.000000 mongo2neo4j-1.0.1/src/mongo2neo4j/__init__.py
--rw-rw-r--   0 luther     (501) staff       (20)      138 2024-04-19 14:06:59.000000 mongo2neo4j-1.0.1/src/mongo2neo4j/__main__.py
--rw-rw-r--   0 luther     (501) staff       (20)        0 2023-08-10 06:05:58.000000 mongo2neo4j-1.0.1/src/mongo2neo4j/py.typed
-drwxr-xr-x   0 luther     (501) staff       (20)        0 2024-04-24 15:56:56.770164 mongo2neo4j-1.0.1/src/mongo2neo4j.egg-info/
--rw-r--r--   0 luther     (501) staff       (20)    46256 2024-04-24 15:56:56.000000 mongo2neo4j-1.0.1/src/mongo2neo4j.egg-info/PKG-INFO
--rw-r--r--   0 luther     (501) staff       (20)      441 2024-04-24 15:56:56.000000 mongo2neo4j-1.0.1/src/mongo2neo4j.egg-info/SOURCES.txt
--rw-r--r--   0 luther     (501) staff       (20)        1 2024-04-24 15:56:56.000000 mongo2neo4j-1.0.1/src/mongo2neo4j.egg-info/dependency_links.txt
--rw-r--r--   0 luther     (501) staff       (20)       57 2024-04-24 15:56:56.000000 mongo2neo4j-1.0.1/src/mongo2neo4j.egg-info/entry_points.txt
--rw-r--r--   0 luther     (501) staff       (20)      206 2024-04-24 15:56:56.000000 mongo2neo4j-1.0.1/src/mongo2neo4j.egg-info/requires.txt
--rw-r--r--   0 luther     (501) staff       (20)       12 2024-04-24 15:56:56.000000 mongo2neo4j-1.0.1/src/mongo2neo4j.egg-info/top_level.txt
-drwxr-xr-x   0 luther     (501) staff       (20)        0 2024-04-24 15:56:56.768847 mongo2neo4j-1.0.1/tests/
--rw-rw-r--   0 luther     (501) staff       (20)       41 2023-07-06 07:53:53.000000 mongo2neo4j-1.0.1/tests/test_basic.py
--rw-rw-r--   0 luther     (501) staff       (20)     9949 2023-10-15 11:38:33.000000 mongo2neo4j-1.0.1/tests/test_flatten_and_cleanse.py
+drwxr-xr-x   0 luther     (501) staff       (20)        0 2024-04-25 17:15:40.439511 mongo2neo4j-1.0.2/
+-rw-r--r--   0 luther     (501) staff       (20)    35821 2023-08-05 21:05:58.000000 mongo2neo4j-1.0.2/LICENSE
+-rw-r--r--   0 luther     (501) staff       (20)    46334 2024-04-25 17:15:40.438287 mongo2neo4j-1.0.2/PKG-INFO
+-rw-r--r--   0 luther     (501) staff       (20)     4425 2024-04-25 17:13:23.000000 mongo2neo4j-1.0.2/README.md
+-rw-r--r--   0 luther     (501) staff       (20)     6987 2024-04-25 16:13:24.000000 mongo2neo4j-1.0.2/pyproject.toml
+-rw-r--r--   0 luther     (501) staff       (20)      170 2024-04-19 13:47:32.000000 mongo2neo4j-1.0.2/requirements-dev.txt
+-rw-r--r--   0 luther     (501) staff       (20)       29 2024-04-16 11:28:39.000000 mongo2neo4j-1.0.2/requirements.txt
+-rw-r--r--   0 luther     (501) staff       (20)       38 2024-04-25 17:15:40.439793 mongo2neo4j-1.0.2/setup.cfg
+drwxr-xr-x   0 luther     (501) staff       (20)        0 2024-04-25 17:15:40.419967 mongo2neo4j-1.0.2/src/
+drwxr-xr-x   0 luther     (501) staff       (20)        0 2024-04-25 17:15:40.424398 mongo2neo4j-1.0.2/src/mongo2neo4j/
+-rw-rw-r--   0 luther     (501) staff       (20)    50768 2024-04-25 16:15:35.000000 mongo2neo4j-1.0.2/src/mongo2neo4j/__init__.py
+-rw-rw-r--   0 luther     (501) staff       (20)      138 2024-04-19 14:06:59.000000 mongo2neo4j-1.0.2/src/mongo2neo4j/__main__.py
+-rw-rw-r--   0 luther     (501) staff       (20)        0 2023-08-10 06:05:58.000000 mongo2neo4j-1.0.2/src/mongo2neo4j/py.typed
+drwxr-xr-x   0 luther     (501) staff       (20)        0 2024-04-25 17:15:40.432577 mongo2neo4j-1.0.2/src/mongo2neo4j.egg-info/
+-rw-r--r--   0 luther     (501) staff       (20)    46334 2024-04-25 17:15:40.000000 mongo2neo4j-1.0.2/src/mongo2neo4j.egg-info/PKG-INFO
+-rw-r--r--   0 luther     (501) staff       (20)      441 2024-04-25 17:15:40.000000 mongo2neo4j-1.0.2/src/mongo2neo4j.egg-info/SOURCES.txt
+-rw-r--r--   0 luther     (501) staff       (20)        1 2024-04-25 17:15:40.000000 mongo2neo4j-1.0.2/src/mongo2neo4j.egg-info/dependency_links.txt
+-rw-r--r--   0 luther     (501) staff       (20)       57 2024-04-25 17:15:40.000000 mongo2neo4j-1.0.2/src/mongo2neo4j.egg-info/entry_points.txt
+-rw-r--r--   0 luther     (501) staff       (20)      206 2024-04-25 17:15:40.000000 mongo2neo4j-1.0.2/src/mongo2neo4j.egg-info/requires.txt
+-rw-r--r--   0 luther     (501) staff       (20)       12 2024-04-25 17:15:40.000000 mongo2neo4j-1.0.2/src/mongo2neo4j.egg-info/top_level.txt
+drwxr-xr-x   0 luther     (501) staff       (20)        0 2024-04-25 17:15:40.431165 mongo2neo4j-1.0.2/tests/
+-rw-rw-r--   0 luther     (501) staff       (20)       41 2023-07-06 07:53:53.000000 mongo2neo4j-1.0.2/tests/test_basic.py
+-rw-rw-r--   0 luther     (501) staff       (20)     9949 2023-10-15 11:38:33.000000 mongo2neo4j-1.0.2/tests/test_flatten_and_cleanse.py
```

### Comparing `mongo2neo4j-1.0.1/LICENSE` & `mongo2neo4j-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mongo2neo4j-1.0.1/PKG-INFO` & `mongo2neo4j-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongo2neo4j
-Version: 1.0.1
+Version: 1.0.2
 Summary: Imports object structures generated by MongoDB object relation mappers (like Mongoose) into Neo4j for exploration with SemSpect
 Author: Marko Luther, Paul Holleis, Thorsten Liebig, Vincent Vialard
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -681,15 +681,15 @@
 Project-URL: Homepage, https://makomo.github.io/mongo2neo4j/
 Project-URL: Issue Tracker, https://github.com/MAKOMO/mongo2neo4j/issues
 Keywords: MongoDB,Neo4j,Mongoose,SemSpect,exploration,conversion
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Other/Nonlisted Topic
-Requires-Python: >=3.12
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pymongo>=4.6.3
 Requires-Dist: neo4j>=5.19.0
 Provides-Extra: dev
 Requires-Dist: mypy>=1.9.0; extra == "dev"
 Requires-Dist: pyright>=1.1.359; extra == "dev"
@@ -745,16 +745,18 @@
 
 ### Install SemSpect Plugin
 
 The free SemSpect Graph App for Neo4j works well (see [SemSpect](https://www.semspect.de/))
 
 ### Install `mongo2neo4j`
 
+Note: mongo2neo4j requires [Python 3.11](https://www.python.org/) or newer.
+
 ```sh
-% pip install mongo2neo4j
+% pip3 install mongo2neo4j
 ```
 
 ## Run the importer
 
 You can run the `mongo2neo4j`importer from the shell by providing at least the name of the [MongoDB](https://www.mongodb.com/) DB the data should be imported from. If not specified the default `neo4j` DB is targeted with the default `neo4j` user. It is likely that you will have to add passwords.
 
 ```sh
```

### Comparing `mongo2neo4j-1.0.1/README.md` & `mongo2neo4j-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -40,16 +40,18 @@
 
 ### Install SemSpect Plugin
 
 The free SemSpect Graph App for Neo4j works well (see [SemSpect](https://www.semspect.de/))
 
 ### Install `mongo2neo4j`
 
+Note: mongo2neo4j requires [Python 3.11](https://www.python.org/) or newer.
+
 ```sh
-% pip install mongo2neo4j
+% pip3 install mongo2neo4j
 ```
 
 ## Run the importer
 
 You can run the `mongo2neo4j`importer from the shell by providing at least the name of the [MongoDB](https://www.mongodb.com/) DB the data should be imported from. If not specified the default `neo4j` DB is targeted with the default `neo4j` user. It is likely that you will have to add passwords.
 
 ```sh
```

### Comparing `mongo2neo4j-1.0.1/pyproject.toml` & `mongo2neo4j-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
   { name="Marko Luther" },
   { name="Paul Holleis" },
   { name="Thorsten Liebig" },
   { name="Vincent Vialard" }
 ]
 license = {file = 'LICENSE'}
 readme = "README.md"
-requires-python = ">=3.12"
+requires-python = ">=3.11"
 keywords = ['MongoDB', 'Neo4j', 'Mongoose', 'SemSpect', 'exploration', 'conversion']
 classifiers = [
     "Programming Language :: Python :: 3 :: Only",
     'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
     "Operating System :: OS Independent",
     'Topic :: Other/Nonlisted Topic'
 ]
@@ -70,15 +70,15 @@
 ]
 
 # Use multiple processes to speed up Pylint. Specifying 0 will auto-detect the
 # number of processors available to use.
 jobs = "0"
 
 # Minimum supported python version
-py-version = "3.12"
+py-version = "3.11"
 
 # Pickle collected data for later comparisons.
 persistent = "no"
 
 [tool.pylint.'MESSAGES CONTROL']
 
 # Disable the message, report, category or checker with the given id(s). You
@@ -131,15 +131,15 @@
 enable='''c-extension-no-member,'''
 
 
 ## mypy conf
 
 [tool.mypy]
 files = ["src/mongo2neo4j/*.py"]
-python_version = "3.12"
+python_version = "3.11"
 
 # Ensure full coverage
 check_untyped_defs = true
 disallow_incomplete_defs = true
 disallow_untyped_calls = true
 disallow_untyped_defs = true
 disallow_untyped_decorators = true
@@ -183,28 +183,28 @@
 
 # Never enforce `E501` (line length violations).
 lint.ignore = ["E402", "E501", "E741", "PLR0913", "PLR2004", "COM812", "PLR0912", "PLR0915", "PLW0603", "PLR0911", "SIM105", "SIM114"]
 
 # Exclude a variety of commonly ignored directories.
 exclude = ["dist", "build", "proto", ".pytype", ".mypy_cache", ".git"]
 
-# Assume Python 3.12
-target-version = "py312"
+# Assume Python 3.11
+target-version = "py311"
 
 
 
 ## pyright conf
 
 [tool.pyright]
 include = ["src/mongo2neo4j"]
 
 reportMissingImports = true
 reportMissingTypeStubs = false
 
-pythonVersion = "3.12"
+pythonVersion = "3.11"
 pythonPlatform = "All"
 
 #typeCheckingMode = "strict" # "off", "basic", "strict"
 
 # strict disabled checks # "error", "warning", false, true
 #reportUnboundVariable = "error"
 #reportUnknownParameterType = false
```

### Comparing `mongo2neo4j-1.0.1/src/mongo2neo4j/__init__.py` & `mongo2neo4j-1.0.2/src/mongo2neo4j/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 """Imports object structures generated by the ORM Mongoose <https://mongoosejs.com/> and
 stored in MongoDB <https://www.mongodb.com/> into Neo4j <https://neo4j.com/> for exploration with
 SemSpect <https://www.semspect.de/>.
 """
 
 # Changelog:
+#  v1.0.2 (04/25/2024) : back to Python 3.11
 #  v1.0.1 (04/22/2024) :
 #     - adds <super_label> to sublabel spec to play nice with SemSpects subtree facets
 #     - escapes single quites in sublabels
 #     - renames attrib to field to correspond to the MongoDB terminology
 #     - moved to Python 3.12
 #  v1.0.0 (04/12/2024) : minor rework and lib updates
 #  v0.5.0 (09/28/2023) : makes import idempotent
@@ -44,15 +45,15 @@
 if TYPE_CHECKING:
     from pymongo.database import Database
     from pymongo.cursor import Cursor
     from neo4j import ManagedTransaction
 
 __author__ = 'Marko Luther, Paul Holleis, Thorsten Liebig, Vincent Vialard, Maximilian Wenzel'
 __license__ = 'GPLv3 <https://www.gnu.org/licenses/gpl-3.0.html>'
-__version__ = '1.0.1'
+__version__ = '1.0.2'
 
 
 # Types
 
 Item = dict[str, Any]
 Items = list[Item]
 Link = tuple[str, str]  # holds source and target IDs
@@ -1092,15 +1093,15 @@
         )
         mapping_group.add_argument(
             '-r',
             '--relations',
             dest='relations',
             action='append',
             default=[],
-            help='List of <Collection>.<field>,<collection>.<field> tuples to relations between nodes of equal str/number values',
+            help='List of <collection>.<field>,<collection>.<field> tuples to relations between nodes of equal str/number values',
         )
         mapping_group.add_argument(
             '-lr',
             '--list_relations',
             dest='list_relations',
             action='append',
             default=[],
```

### Comparing `mongo2neo4j-1.0.1/src/mongo2neo4j.egg-info/PKG-INFO` & `mongo2neo4j-1.0.2/src/mongo2neo4j.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongo2neo4j
-Version: 1.0.1
+Version: 1.0.2
 Summary: Imports object structures generated by MongoDB object relation mappers (like Mongoose) into Neo4j for exploration with SemSpect
 Author: Marko Luther, Paul Holleis, Thorsten Liebig, Vincent Vialard
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -681,15 +681,15 @@
 Project-URL: Homepage, https://makomo.github.io/mongo2neo4j/
 Project-URL: Issue Tracker, https://github.com/MAKOMO/mongo2neo4j/issues
 Keywords: MongoDB,Neo4j,Mongoose,SemSpect,exploration,conversion
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Other/Nonlisted Topic
-Requires-Python: >=3.12
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pymongo>=4.6.3
 Requires-Dist: neo4j>=5.19.0
 Provides-Extra: dev
 Requires-Dist: mypy>=1.9.0; extra == "dev"
 Requires-Dist: pyright>=1.1.359; extra == "dev"
@@ -745,16 +745,18 @@
 
 ### Install SemSpect Plugin
 
 The free SemSpect Graph App for Neo4j works well (see [SemSpect](https://www.semspect.de/))
 
 ### Install `mongo2neo4j`
 
+Note: mongo2neo4j requires [Python 3.11](https://www.python.org/) or newer.
+
 ```sh
-% pip install mongo2neo4j
+% pip3 install mongo2neo4j
 ```
 
 ## Run the importer
 
 You can run the `mongo2neo4j`importer from the shell by providing at least the name of the [MongoDB](https://www.mongodb.com/) DB the data should be imported from. If not specified the default `neo4j` DB is targeted with the default `neo4j` user. It is likely that you will have to add passwords.
 
 ```sh
```

### Comparing `mongo2neo4j-1.0.1/tests/test_flatten_and_cleanse.py` & `mongo2neo4j-1.0.2/tests/test_flatten_and_cleanse.py`

 * *Files identical despite different names*

