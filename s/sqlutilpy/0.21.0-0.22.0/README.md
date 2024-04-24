# Comparing `tmp/sqlutilpy-0.21.0.tar.gz` & `tmp/sqlutilpy-0.22.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlutilpy-0.21.0.tar", last modified: Wed Nov 29 18:45:34 2023, max compression
+gzip compressed data, was "sqlutilpy-0.22.0.tar", last modified: Wed Apr 24 22:01:20 2024, max compression
```

## Comparing `sqlutilpy-0.21.0.tar` & `sqlutilpy-0.22.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 skoposov  (1000) skoposov  (1000)        0 2023-11-29 18:45:34.680360 sqlutilpy-0.21.0/
--rw-rw-r--   0 skoposov  (1000) skoposov  (1000)     1500 2021-05-04 10:55:43.000000 sqlutilpy-0.21.0/LICENSE.txt
--rw-rw-r--   0 skoposov  (1000) skoposov  (1000)      168 2021-05-04 10:55:43.000000 sqlutilpy-0.21.0/MANIFEST.in
--rw-r--r--   0 skoposov  (1000) skoposov  (1000)     3950 2023-11-29 18:45:34.680360 sqlutilpy-0.21.0/PKG-INFO
--rw-rw-r--   0 skoposov  (1000) skoposov  (1000)     3409 2023-02-01 20:34:51.000000 sqlutilpy-0.21.0/README.md
-drwxrwxr-x   0 skoposov  (1000) skoposov  (1000)        0 2023-11-29 18:45:34.676360 sqlutilpy-0.21.0/py/
-drwxrwxr-x   0 skoposov  (1000) skoposov  (1000)        0 2023-11-29 18:45:34.676360 sqlutilpy-0.21.0/py/sqlutilpy/
--rw-rw-r--   0 skoposov  (1000) skoposov  (1000)      245 2022-07-07 18:16:22.000000 sqlutilpy-0.21.0/py/sqlutilpy/__init__.py
--rw-rw-r--   0 skoposov  (1000) skoposov  (1000)    26587 2023-11-29 18:32:45.000000 sqlutilpy-0.21.0/py/sqlutilpy/sqlutil.py
--rw-rw-r--   0 skoposov  (1000) skoposov  (1000)       23 2023-11-29 18:41:46.000000 sqlutilpy-0.21.0/py/sqlutilpy/version.py
-drwxrwxr-x   0 skoposov  (1000) skoposov  (1000)        0 2023-11-29 18:45:34.680360 sqlutilpy-0.21.0/py/sqlutilpy.egg-info/
--rw-r--r--   0 skoposov  (1000) skoposov  (1000)     3950 2023-11-29 18:45:34.000000 sqlutilpy-0.21.0/py/sqlutilpy.egg-info/PKG-INFO
--rw-rw-r--   0 skoposov  (1000) skoposov  (1000)      359 2023-11-29 18:45:34.000000 sqlutilpy-0.21.0/py/sqlutilpy.egg-info/SOURCES.txt
--rw-rw-r--   0 skoposov  (1000) skoposov  (1000)        1 2023-11-29 18:45:34.000000 sqlutilpy-0.21.0/py/sqlutilpy.egg-info/dependency_links.txt
--rw-rw-r--   0 skoposov  (1000) skoposov  (1000)       31 2023-11-29 18:45:34.000000 sqlutilpy-0.21.0/py/sqlutilpy.egg-info/requires.txt
--rw-rw-r--   0 skoposov  (1000) skoposov  (1000)       10 2023-11-29 18:45:34.000000 sqlutilpy-0.21.0/py/sqlutilpy.egg-info/top_level.txt
--rw-rw-r--   0 skoposov  (1000) skoposov  (1000)       31 2021-05-04 10:55:43.000000 sqlutilpy-0.21.0/requirements.txt
--rw-rw-r--   0 skoposov  (1000) skoposov  (1000)       79 2023-11-29 18:45:34.680360 sqlutilpy-0.21.0/setup.cfg
--rw-rw-r--   0 skoposov  (1000) skoposov  (1000)     1870 2021-05-04 10:55:43.000000 sqlutilpy-0.21.0/setup.py
-drwxrwxr-x   0 skoposov  (1000) skoposov  (1000)        0 2023-11-29 18:45:34.676360 sqlutilpy-0.21.0/tests/
--rw-rw-r--   0 skoposov  (1000) skoposov  (1000)      261 2021-05-04 10:55:43.000000 sqlutilpy-0.21.0/tests/killer.py
--rw-rw-r--   0 skoposov  (1000) skoposov  (1000)    15970 2023-11-29 18:33:39.000000 sqlutilpy-0.21.0/tests/sqlutil_test.py
+drwxrwxr-x   0 koposov   (1000) koposov   (1000)        0 2024-04-24 22:01:20.071288 sqlutilpy-0.22.0/
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)     1500 2024-04-24 22:01:15.000000 sqlutilpy-0.22.0/LICENSE.txt
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)      168 2024-04-24 22:01:15.000000 sqlutilpy-0.22.0/MANIFEST.in
+-rw-r--r--   0 koposov   (1000) koposov   (1000)     4401 2024-04-24 22:01:20.071288 sqlutilpy-0.22.0/PKG-INFO
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)     3826 2024-04-24 22:01:15.000000 sqlutilpy-0.22.0/README.md
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)      751 2024-04-24 22:01:15.000000 sqlutilpy-0.22.0/pyproject.toml
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)       38 2024-04-24 22:01:20.071288 sqlutilpy-0.22.0/setup.cfg
+drwxrwxr-x   0 koposov   (1000) koposov   (1000)        0 2024-04-24 22:01:20.067288 sqlutilpy-0.22.0/src/
+drwxrwxr-x   0 koposov   (1000) koposov   (1000)        0 2024-04-24 22:01:20.067288 sqlutilpy-0.22.0/src/sqlutilpy/
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)      245 2024-04-24 22:01:15.000000 sqlutilpy-0.22.0/src/sqlutilpy/__init__.py
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)    26587 2024-04-24 22:01:15.000000 sqlutilpy-0.22.0/src/sqlutilpy/sqlutil.py
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)       23 2024-04-24 22:01:15.000000 sqlutilpy-0.22.0/src/sqlutilpy/version.py
+drwxrwxr-x   0 koposov   (1000) koposov   (1000)        0 2024-04-24 22:01:20.071288 sqlutilpy-0.22.0/src/sqlutilpy.egg-info/
+-rw-r--r--   0 koposov   (1000) koposov   (1000)     4401 2024-04-24 22:01:20.000000 sqlutilpy-0.22.0/src/sqlutilpy.egg-info/PKG-INFO
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)      362 2024-04-24 22:01:20.000000 sqlutilpy-0.22.0/src/sqlutilpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)        1 2024-04-24 22:01:20.000000 sqlutilpy-0.22.0/src/sqlutilpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)       31 2024-04-24 22:01:20.000000 sqlutilpy-0.22.0/src/sqlutilpy.egg-info/requires.txt
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)       10 2024-04-24 22:01:20.000000 sqlutilpy-0.22.0/src/sqlutilpy.egg-info/top_level.txt
+drwxrwxr-x   0 koposov   (1000) koposov   (1000)        0 2024-04-24 22:01:20.071288 sqlutilpy-0.22.0/tests/
+-rw-r--r--   0 koposov   (1000) koposov   (1000)      261 2024-04-24 22:01:15.000000 sqlutilpy-0.22.0/tests/killer.py
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)    13557 2024-04-24 22:01:15.000000 sqlutilpy-0.22.0/tests/test_pg.py
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)      837 2024-04-24 22:01:15.000000 sqlutilpy-0.22.0/tests/test_sqlite.py
```

### Comparing `sqlutilpy-0.21.0/LICENSE.txt` & `sqlutilpy-0.22.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sqlutilpy-0.21.0/PKG-INFO` & `sqlutilpy-0.22.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,70 +1,75 @@
 Metadata-Version: 2.1
 Name: sqlutilpy
-Version: 0.21.0
+Version: 0.22.0
 Summary: Database query code returning numpy arrays
-Home-page: https://github.com/segasai/sqlutilpy
-Author: Sergey Koposov
-Author-email: skoposov@ed.ac.uk
+Author-email: "Sergey E. Koposov" <skoposov@ed.ac.uk>
 License: BSD
+Project-URL: Homepage, https://github.com/segasai/sqlutilpy
 Keywords: numpy postgresql query sql sqlite array
 Classifier: Development Status :: 3 - Alpha
-Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: BSD License
+Classifier: Topic :: Utilities
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy
 Requires-Dist: psycopg2-binary
 Requires-Dist: numpydoc
 
 [![Build Status](https://github.com/segasai/sqlutilpy/workflows/Testing/badge.svg)](https://github.com/segasai/sqlutilpy/actions)
 [![Documentation Status](https://readthedocs.org/projects/sqlutilpy/badge/?version=latest)](http://sqlutilpy.readthedocs.io/en/latest/?badge=latest)
 [![Coverage Status](https://coveralls.io/repos/github/segasai/sqlutilpy/badge.svg?branch=master)](https://coveralls.io/github/segasai/sqlutilpy?branch=master)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6867957.svg)](https://doi.org/10.5281/zenodo.6867957)
 
 # sqlutilpy
 Python module to query SQL databases and return numpy arrays, upload
 tables and run join queries involving local arrays and the tables in the DB.
-The module only works with PostgreSQL and SQLite databases.
+This module is optimized to be able to deal efficiently with query results with millions of rows.
+The module only works with PostgreSQL, SQLite and DuckDB databases.
 
 The full documentation is available [here](http://sqlutilpy.readthedocs.io/en/latest/)
 
 Author: Sergey Koposov (Uni of Cambridge/CMU/Uni of Edinburgh)
 
 ## Installation
 To install the package you just need to do pip install. 
 
 ```
 pip install sqlutilpy
 ```
-## Authentification
-Throughout this readme, I'll assume that the .pgpass file ( https://www.postgresql.org/docs/11/libpq-pgpass.html ) 
-has been created with the login/password details for Postgresql. If that is not the case, all of the 
-commands given above will also need user='....' and password='...' options
+## Authentication
+
+Throughout this readme, I will assume that the .pgpass file ( https://www.postgresql.org/docs/11/libpq-pgpass.html ) 
+has been created with your login/password details for Postgresql. If that is not the case, all of the 
+commands given below will also need user='....' and password='...' options
 
 ## Connection information
 
 Most of the sqlutilpy commands require hostname, database name, user etc. 
 If you don't want to always type it, you can use standard PostgreSQL environment variables
 like PGPORT, PGDATABASE, PGUSER, PGHOST for the port, database name, user name and hostname
 of the connection. 
 
 
 ## Querying the database and retrieving the results
+
+This command will run the query and put the columns into variables ra,dec
 ```python
 import sqlutilpy
 ra,dec = squtilpy.get('select ra,dec from mytable', 
                  host='HOST_NAME_OF_MY_PG_SERVER', 
                  db='THE_NAME_OF_MY_DB')
 ```
 
-By default sqlutilpy.get executes the result and returns the tuple of 
-results. But you can return the results as dictionary using asDict option.
+By default sqlutilpy.get executes the query and returns the tuple with 
+results. You can return the results as dictionary using asDict option.
 
 ## Uploading your arrays as column in a table
+
 ```python
 x = np.arange(10)                                                   
 y = x**.5                                                           
 sqlutilpy.upload('mytable',(x,y),('xcol','ycol'))    
 ``` 
 This will create a table called mytable with columns xcol and ycol 
 
@@ -72,24 +77,32 @@
 
 Imagine you have arrays myid and y and you want to to extract all the 
 information from somebigtable for objects with id=myid. In principle
 you could upload the arrays in the DB and run a query, but local_join function does that for you.
 
 ```python
 myid = np.arange(10)
-y = x**.5
+y = np.random.uniform(size=10)
+
 R=sqlutilpy.local_join('''select * from mytmptable as m, 
-           somebigtable as s where s.id=m.myid order by m.myid''',                                                                       'mytmptable',(x,y),('myid','ycol'))
+           somebigtable as s where s.id=m.myid order by m.myid''',                                              
+           'mytmptable',(myid, y),('myid','ycol'))
 ```
-It executes a query as if you arrays where in a mytmptable. ( behind the scenes
-it uploads the data to the db and runs a query)
 
+It executes a query as if you arrays were in mytmptable. (behind the scenes
+it uploads the data to the db and runs a query)
 
 ## Keeping the connection open. 
 
-Often it's benefitial to preserve an open connection. You can do that if you first 
+Often it is beneficial to preserve an open connection to the database. You can do that if you first 
 obtain the connection using sqlutilpy.getConnection() and then provide it directly
 to sqlutil.get() and friends using conn=conn argument
+```python
+conn = sqlutilpy.getConnection(db='mydb', user='meuser', password='something', host='hostname')
+R= sqlutilpy.get('select 1', conn=conn)
+R1= sqlutilpy.get('select 1', conn=conn)
+```
+
+# How to cite the software
 
+If you use this package, please cite it through zenodo https://doi.org/10.5281/zenodo.6867957
 
-# How to cite it
-If you use this, please cite it through zenodo https://doi.org/10.5281/zenodo.6867957
```

### Comparing `sqlutilpy-0.21.0/README.md` & `sqlutilpy-0.22.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -2,51 +2,56 @@
 [![Documentation Status](https://readthedocs.org/projects/sqlutilpy/badge/?version=latest)](http://sqlutilpy.readthedocs.io/en/latest/?badge=latest)
 [![Coverage Status](https://coveralls.io/repos/github/segasai/sqlutilpy/badge.svg?branch=master)](https://coveralls.io/github/segasai/sqlutilpy?branch=master)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6867957.svg)](https://doi.org/10.5281/zenodo.6867957)
 
 # sqlutilpy
 Python module to query SQL databases and return numpy arrays, upload
 tables and run join queries involving local arrays and the tables in the DB.
-The module only works with PostgreSQL and SQLite databases.
+This module is optimized to be able to deal efficiently with query results with millions of rows.
+The module only works with PostgreSQL, SQLite and DuckDB databases.
 
 The full documentation is available [here](http://sqlutilpy.readthedocs.io/en/latest/)
 
 Author: Sergey Koposov (Uni of Cambridge/CMU/Uni of Edinburgh)
 
 ## Installation
 To install the package you just need to do pip install. 
 
 ```
 pip install sqlutilpy
 ```
-## Authentification
-Throughout this readme, I'll assume that the .pgpass file ( https://www.postgresql.org/docs/11/libpq-pgpass.html ) 
-has been created with the login/password details for Postgresql. If that is not the case, all of the 
-commands given above will also need user='....' and password='...' options
+## Authentication
+
+Throughout this readme, I will assume that the .pgpass file ( https://www.postgresql.org/docs/11/libpq-pgpass.html ) 
+has been created with your login/password details for Postgresql. If that is not the case, all of the 
+commands given below will also need user='....' and password='...' options
 
 ## Connection information
 
 Most of the sqlutilpy commands require hostname, database name, user etc. 
 If you don't want to always type it, you can use standard PostgreSQL environment variables
 like PGPORT, PGDATABASE, PGUSER, PGHOST for the port, database name, user name and hostname
 of the connection. 
 
 
 ## Querying the database and retrieving the results
+
+This command will run the query and put the columns into variables ra,dec
 ```python
 import sqlutilpy
 ra,dec = squtilpy.get('select ra,dec from mytable', 
                  host='HOST_NAME_OF_MY_PG_SERVER', 
                  db='THE_NAME_OF_MY_DB')
 ```
 
-By default sqlutilpy.get executes the result and returns the tuple of 
-results. But you can return the results as dictionary using asDict option.
+By default sqlutilpy.get executes the query and returns the tuple with 
+results. You can return the results as dictionary using asDict option.
 
 ## Uploading your arrays as column in a table
+
 ```python
 x = np.arange(10)                                                   
 y = x**.5                                                           
 sqlutilpy.upload('mytable',(x,y),('xcol','ycol'))    
 ``` 
 This will create a table called mytable with columns xcol and ycol 
 
@@ -54,24 +59,32 @@
 
 Imagine you have arrays myid and y and you want to to extract all the 
 information from somebigtable for objects with id=myid. In principle
 you could upload the arrays in the DB and run a query, but local_join function does that for you.
 
 ```python
 myid = np.arange(10)
-y = x**.5
+y = np.random.uniform(size=10)
+
 R=sqlutilpy.local_join('''select * from mytmptable as m, 
-           somebigtable as s where s.id=m.myid order by m.myid''',                                                                       'mytmptable',(x,y),('myid','ycol'))
+           somebigtable as s where s.id=m.myid order by m.myid''',                                              
+           'mytmptable',(myid, y),('myid','ycol'))
 ```
-It executes a query as if you arrays where in a mytmptable. ( behind the scenes
-it uploads the data to the db and runs a query)
 
+It executes a query as if you arrays were in mytmptable. (behind the scenes
+it uploads the data to the db and runs a query)
 
 ## Keeping the connection open. 
 
-Often it's benefitial to preserve an open connection. You can do that if you first 
+Often it is beneficial to preserve an open connection to the database. You can do that if you first 
 obtain the connection using sqlutilpy.getConnection() and then provide it directly
 to sqlutil.get() and friends using conn=conn argument
+```python
+conn = sqlutilpy.getConnection(db='mydb', user='meuser', password='something', host='hostname')
+R= sqlutilpy.get('select 1', conn=conn)
+R1= sqlutilpy.get('select 1', conn=conn)
+```
+
+# How to cite the software
 
+If you use this package, please cite it through zenodo https://doi.org/10.5281/zenodo.6867957
 
-# How to cite it
-If you use this, please cite it through zenodo https://doi.org/10.5281/zenodo.6867957
```

### Comparing `sqlutilpy-0.21.0/py/sqlutilpy/sqlutil.py` & `sqlutilpy-0.22.0/src/sqlutilpy/sqlutil.py`

 * *Files identical despite different names*

### Comparing `sqlutilpy-0.21.0/py/sqlutilpy.egg-info/PKG-INFO` & `sqlutilpy-0.22.0/src/sqlutilpy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,70 +1,75 @@
 Metadata-Version: 2.1
 Name: sqlutilpy
-Version: 0.21.0
+Version: 0.22.0
 Summary: Database query code returning numpy arrays
-Home-page: https://github.com/segasai/sqlutilpy
-Author: Sergey Koposov
-Author-email: skoposov@ed.ac.uk
+Author-email: "Sergey E. Koposov" <skoposov@ed.ac.uk>
 License: BSD
+Project-URL: Homepage, https://github.com/segasai/sqlutilpy
 Keywords: numpy postgresql query sql sqlite array
 Classifier: Development Status :: 3 - Alpha
-Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: BSD License
+Classifier: Topic :: Utilities
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy
 Requires-Dist: psycopg2-binary
 Requires-Dist: numpydoc
 
 [![Build Status](https://github.com/segasai/sqlutilpy/workflows/Testing/badge.svg)](https://github.com/segasai/sqlutilpy/actions)
 [![Documentation Status](https://readthedocs.org/projects/sqlutilpy/badge/?version=latest)](http://sqlutilpy.readthedocs.io/en/latest/?badge=latest)
 [![Coverage Status](https://coveralls.io/repos/github/segasai/sqlutilpy/badge.svg?branch=master)](https://coveralls.io/github/segasai/sqlutilpy?branch=master)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6867957.svg)](https://doi.org/10.5281/zenodo.6867957)
 
 # sqlutilpy
 Python module to query SQL databases and return numpy arrays, upload
 tables and run join queries involving local arrays and the tables in the DB.
-The module only works with PostgreSQL and SQLite databases.
+This module is optimized to be able to deal efficiently with query results with millions of rows.
+The module only works with PostgreSQL, SQLite and DuckDB databases.
 
 The full documentation is available [here](http://sqlutilpy.readthedocs.io/en/latest/)
 
 Author: Sergey Koposov (Uni of Cambridge/CMU/Uni of Edinburgh)
 
 ## Installation
 To install the package you just need to do pip install. 
 
 ```
 pip install sqlutilpy
 ```
-## Authentification
-Throughout this readme, I'll assume that the .pgpass file ( https://www.postgresql.org/docs/11/libpq-pgpass.html ) 
-has been created with the login/password details for Postgresql. If that is not the case, all of the 
-commands given above will also need user='....' and password='...' options
+## Authentication
+
+Throughout this readme, I will assume that the .pgpass file ( https://www.postgresql.org/docs/11/libpq-pgpass.html ) 
+has been created with your login/password details for Postgresql. If that is not the case, all of the 
+commands given below will also need user='....' and password='...' options
 
 ## Connection information
 
 Most of the sqlutilpy commands require hostname, database name, user etc. 
 If you don't want to always type it, you can use standard PostgreSQL environment variables
 like PGPORT, PGDATABASE, PGUSER, PGHOST for the port, database name, user name and hostname
 of the connection. 
 
 
 ## Querying the database and retrieving the results
+
+This command will run the query and put the columns into variables ra,dec
 ```python
 import sqlutilpy
 ra,dec = squtilpy.get('select ra,dec from mytable', 
                  host='HOST_NAME_OF_MY_PG_SERVER', 
                  db='THE_NAME_OF_MY_DB')
 ```
 
-By default sqlutilpy.get executes the result and returns the tuple of 
-results. But you can return the results as dictionary using asDict option.
+By default sqlutilpy.get executes the query and returns the tuple with 
+results. You can return the results as dictionary using asDict option.
 
 ## Uploading your arrays as column in a table
+
 ```python
 x = np.arange(10)                                                   
 y = x**.5                                                           
 sqlutilpy.upload('mytable',(x,y),('xcol','ycol'))    
 ``` 
 This will create a table called mytable with columns xcol and ycol 
 
@@ -72,24 +77,32 @@
 
 Imagine you have arrays myid and y and you want to to extract all the 
 information from somebigtable for objects with id=myid. In principle
 you could upload the arrays in the DB and run a query, but local_join function does that for you.
 
 ```python
 myid = np.arange(10)
-y = x**.5
+y = np.random.uniform(size=10)
+
 R=sqlutilpy.local_join('''select * from mytmptable as m, 
-           somebigtable as s where s.id=m.myid order by m.myid''',                                                                       'mytmptable',(x,y),('myid','ycol'))
+           somebigtable as s where s.id=m.myid order by m.myid''',                                              
+           'mytmptable',(myid, y),('myid','ycol'))
 ```
-It executes a query as if you arrays where in a mytmptable. ( behind the scenes
-it uploads the data to the db and runs a query)
 
+It executes a query as if you arrays were in mytmptable. (behind the scenes
+it uploads the data to the db and runs a query)
 
 ## Keeping the connection open. 
 
-Often it's benefitial to preserve an open connection. You can do that if you first 
+Often it is beneficial to preserve an open connection to the database. You can do that if you first 
 obtain the connection using sqlutilpy.getConnection() and then provide it directly
 to sqlutil.get() and friends using conn=conn argument
+```python
+conn = sqlutilpy.getConnection(db='mydb', user='meuser', password='something', host='hostname')
+R= sqlutilpy.get('select 1', conn=conn)
+R1= sqlutilpy.get('select 1', conn=conn)
+```
+
+# How to cite the software
 
+If you use this package, please cite it through zenodo https://doi.org/10.5281/zenodo.6867957
 
-# How to cite it
-If you use this, please cite it through zenodo https://doi.org/10.5281/zenodo.6867957
```

