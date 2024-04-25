# Comparing `tmp/kitab-0.0.5.tar.gz` & `tmp/kitab-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kitab-0.0.5.tar", last modified: Thu Apr 25 08:15:14 2024, max compression
+gzip compressed data, was "kitab-0.0.6.tar", last modified: Thu Apr 25 18:17:07 2024, max compression
```

## Comparing `kitab-0.0.5.tar` & `kitab-0.0.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 08:15:14.667136 kitab-0.0.5/
--rw-rw-rw-   0        0        0     1100 2024-04-07 17:53:03.000000 kitab-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      448 2024-04-25 08:15:14.664557 kitab-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      770 2024-04-07 17:53:03.000000 kitab-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 08:15:14.604807 kitab-0.0.5/kitab/
--rw-rw-rw-   0        0        0      131 2024-04-08 06:51:45.000000 kitab-0.0.5/kitab/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 08:15:14.621039 kitab-0.0.5/kitab/api/
--rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.5/kitab/api/__init__.py
--rw-rw-rw-   0        0        0     7424 2024-04-24 20:41:38.000000 kitab-0.0.5/kitab/api/app.py
-drwxrwxrwx   0        0        0        0 2024-04-25 08:15:14.637996 kitab-0.0.5/kitab/db/
--rw-rw-rw-   0        0        0      370 2024-04-21 06:34:18.000000 kitab-0.0.5/kitab/db/__init__.py
--rw-rw-rw-   0        0        0     2187 2024-04-25 07:42:15.000000 kitab-0.0.5/kitab/db/db_info.py
--rw-rw-rw-   0        0        0    15561 2024-04-24 20:40:19.000000 kitab-0.0.5/kitab/db/functions.py
--rw-rw-rw-   0        0        0     4982 2024-04-25 07:45:16.000000 kitab-0.0.5/kitab/db/get_data.py
--rw-rw-rw-   0        0        0    11876 2024-04-24 20:46:49.000000 kitab-0.0.5/kitab/db/sql_interactions.py
-drwxrwxrwx   0        0        0        0 2024-04-25 08:15:14.647307 kitab-0.0.5/kitab/logger/
--rw-rw-rw-   0        0        0       37 2024-04-07 17:53:03.000000 kitab-0.0.5/kitab/logger/__init__.py
--rw-rw-rw-   0        0        0     1737 2024-04-24 20:44:07.000000 kitab-0.0.5/kitab/logger/logger.py
-drwxrwxrwx   0        0        0        0 2024-04-25 08:15:14.651127 kitab-0.0.5/kitab/recommendation_model/
--rw-rw-rw-   0        0        0       88 2024-04-08 13:12:13.000000 kitab-0.0.5/kitab/recommendation_model/__init__.py
--rw-rw-rw-   0        0        0     4145 2024-04-24 20:42:55.000000 kitab-0.0.5/kitab/recommendation_model/models.py
--rw-rw-rw-   0        0        0     4568 2024-04-25 07:45:42.000000 kitab-0.0.5/kitab/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-25 08:15:14.654666 kitab-0.0.5/kitab.egg-info/
--rw-rw-rw-   0        0        0      448 2024-04-25 08:15:14.000000 kitab-0.0.5/kitab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      523 2024-04-25 08:15:14.000000 kitab-0.0.5/kitab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 08:15:14.000000 kitab-0.0.5/kitab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2024-04-25 08:15:14.000000 kitab-0.0.5/kitab.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-25 08:15:14.000000 kitab-0.0.5/kitab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 08:15:14.667136 kitab-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      575 2024-04-25 08:14:54.000000 kitab-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 08:15:14.654666 kitab-0.0.5/tests/
--rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.5/tests/test_module1.py
--rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.5/tests/test_module2.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:17:07.469263 kitab-0.0.6/
+-rw-rw-rw-   0        0        0     1100 2024-04-07 17:53:03.000000 kitab-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      478 2024-04-25 18:17:07.466216 kitab-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4274 2024-04-25 14:50:27.000000 kitab-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 18:17:07.400076 kitab-0.0.6/kitab/
+-rw-rw-rw-   0        0        0      131 2024-04-08 06:51:45.000000 kitab-0.0.6/kitab/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:17:07.428100 kitab-0.0.6/kitab/api/
+-rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.6/kitab/api/__init__.py
+-rw-rw-rw-   0        0        0     7500 2024-04-25 14:26:03.000000 kitab-0.0.6/kitab/api/app.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:17:07.443007 kitab-0.0.6/kitab/db/
+-rw-rw-rw-   0        0        0      370 2024-04-21 06:34:18.000000 kitab-0.0.6/kitab/db/__init__.py
+-rw-rw-rw-   0        0        0     2206 2024-04-25 13:49:11.000000 kitab-0.0.6/kitab/db/db_info.py
+-rw-rw-rw-   0        0        0    15703 2024-04-25 14:41:33.000000 kitab-0.0.6/kitab/db/functions.py
+-rw-rw-rw-   0        0        0     4993 2024-04-25 13:50:18.000000 kitab-0.0.6/kitab/db/get_data.py
+-rw-rw-rw-   0        0        0    12309 2024-04-25 14:41:05.000000 kitab-0.0.6/kitab/db/sql_interactions.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:17:07.449895 kitab-0.0.6/kitab/logger/
+-rw-rw-rw-   0        0        0       37 2024-04-07 17:53:03.000000 kitab-0.0.6/kitab/logger/__init__.py
+-rw-rw-rw-   0        0        0     1812 2024-04-25 14:42:46.000000 kitab-0.0.6/kitab/logger/logger.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:17:07.454394 kitab-0.0.6/kitab/recommendation_model/
+-rw-rw-rw-   0        0        0       88 2024-04-08 13:12:13.000000 kitab-0.0.6/kitab/recommendation_model/__init__.py
+-rw-rw-rw-   0        0        0     4216 2024-04-25 14:23:05.000000 kitab-0.0.6/kitab/recommendation_model/models.py
+-rw-rw-rw-   0        0        0     4657 2024-04-25 14:43:09.000000 kitab-0.0.6/kitab/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:17:07.464378 kitab-0.0.6/kitab.egg-info/
+-rw-rw-rw-   0        0        0      478 2024-04-25 18:17:07.000000 kitab-0.0.6/kitab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      523 2024-04-25 18:17:07.000000 kitab-0.0.6/kitab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 18:17:07.000000 kitab-0.0.6/kitab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-04-25 18:17:07.000000 kitab-0.0.6/kitab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-25 18:17:07.000000 kitab-0.0.6/kitab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 18:17:07.469263 kitab-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      592 2024-04-25 18:17:00.000000 kitab-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:17:07.462945 kitab-0.0.6/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.6/tests/test_module1.py
+-rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.6/tests/test_module2.py
```

### Comparing `kitab-0.0.5/LICENSE` & `kitab-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kitab-0.0.5/kitab/api/app.py` & `kitab-0.0.6/kitab/api/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""
+This module contains the API for the book recommendation system.
+"""
 from ..db.functions import get_book_by_ISBN, get_book_by_title, add_book_db, update_book_db, add_recommendation_log, get_history_by_recommendation_isbn
 from ..recommendation_model.models import recommend_books, recommend_books_by_ISBN, recommend_books_by_title
 from fastapi import FastAPI
 from pydantic import BaseModel
 import uvicorn
 import logging
```

### Comparing `kitab-0.0.5/kitab/db/db_info.py` & `kitab-0.0.6/kitab/db/db_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import os
 from dotenv import load_dotenv, find_dotenv
 load_dotenv(find_dotenv())
 
-REQUIRED_COLUMNS = ["isbn", "title", "description", "available"]
-
 # Get DB credentials from the environment variables
 DB_USER = os.getenv("DB_USER")
 DB_PASSWORD = os.getenv("DB_PASSWORD")
 DB_HOST = os.getenv("DB_HOST")
 DB_PORT = os.getenv("DB_PORT")
 DB_NAME = os.getenv("DB_NAME")
 
+REQUIRED_COLUMNS = ["isbn", "title", "description", "author", "genre", "available"]
+
 COMMANDS = (
     "CREATE EXTENSION IF NOT EXISTS vector;"
 
     "DROP TABLE IF EXISTS BookAuthor;",
         
     "DROP TABLE IF EXISTS Author;",
```

### Comparing `kitab-0.0.5/kitab/db/functions.py` & `kitab-0.0.6/kitab/db/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""
+This module contains tailored functions for interacting with the database. These are used by the API and the recommendation model.
+"""
 import pandas as pd
 from kitab.utils import get_embedding
 from .db_info import DB_USER, DB_PASSWORD, DB_HOST, DB_PORT, DB_NAME
 from .sql_interactions import SqlHandler
 import logging
 
 from ..logger.logger import CustomFormatter
```

### Comparing `kitab-0.0.5/kitab/db/get_data.py` & `kitab-0.0.6/kitab/db/get_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     try:
         # Getting the full data
         data = get_full_data(folder_path)
         
         data.fillna({"genre": ""}, inplace=True)
         data = data[REQUIRED_COLUMNS]
         
-        data.dropna(subset = ["isbn", "desc"], inplace=True)
+        data.dropna(subset = ["isbn", "description"], inplace=True)
 
         book_table = data[["isbn", "title", "description", "embedding", "available"]]
 
         def split_and_filter(cell):
             if cell:
                 genres = cell.split(",")
                 return [g.strip() for g in genres if g]
@@ -75,29 +75,29 @@
         data["author"] = authors
         unique_authors = authors.explode().dropna().unique()
         author_table = pd.DataFrame({"author_id": range(1, len(unique_authors)+1), "full_name": unique_authors})
 
         books_with_authors = data[data['author'].map(lambda d: len(d)) > 0]
         book_author = books_with_authors.explode("author")[["author", "isbn"]]
         book_author = pd.merge(book_author, author_table, how='left', left_on='author', right_on='full_name')[["isbn", "author_id"]]
-        book_author.rename(columns={"isbn":"ISBN"}, inplace=True)
+        # book_author.rename(columns={"isbn":"ISBN"}, inplace=True)
         book_author.drop_duplicates(inplace=True)
         book_author.reset_index(drop=True, inplace=True)
         book_author["author_id"] = book_author["author_id"].astype(int)
 
         genres = data["genre"].apply(lambda x: split_and_filter(x))
         data["genre"] = genres
         unique_genres = genres.explode().dropna().unique()
         genre_table = pd.DataFrame({"genre_id": range(1, len(unique_genres)+1), "genre": unique_genres})
 
         books_with_genres = data[data['genre'].map(lambda d: len(d)) > 0]
         book_genre = books_with_genres.explode("genre")[["genre", "isbn"]]
         book_genre["genre"] = book_genre["genre"].str.strip()
         book_genre = pd.merge(book_genre, genre_table, how='left', left_on='genre', right_on='genre')[["isbn", "genre_id"]]
-        book_genre.rename(columns={"isbn":"ISBN"}, inplace=True)
+        # book_genre.rename(columns={"isbn":"ISBN"}, inplace=True)
         book_genre.drop_duplicates(inplace=True)
         book_genre.reset_index(drop=True, inplace=True)
         book_genre["genre_id"] = book_genre["genre_id"].astype(int)
 
         # Establish connection with the database
         sql_handler = SqlHandler(DB_NAME, user=DB_USER, password=DB_PASSWORD, host=DB_HOST, port=DB_PORT)
```

### Comparing `kitab-0.0.5/kitab/db/sql_interactions.py` & `kitab-0.0.6/kitab/db/sql_interactions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""
+This module contains the functions for interacting with the SQL database.
+"""
 import psycopg2
 from pgvector.psycopg2 import register_vector
 import logging
 import pandas as pd
 import numpy as np
 
 from ..logger.logger import CustomFormatter
@@ -12,14 +15,19 @@
 ch.setLevel(logging.DEBUG)
 ch.setFormatter(CustomFormatter())
 logger.addHandler(ch)
 
 class SqlHandler:
 
     def __init__(self, dbname: str, user: str, password: str, host: str, port: str) -> None:
+        # Check credentials
+        print([dbname, user, password, host, port])
+        if any(not cred for cred in [dbname, user, password, host, port]):
+            raise Exception("Some database credentials were not passed. Please fill in the database credentials (DB_USER, DB_PASSWORD, DB_HOST, DB_PORT, DB_NAME) in db_info.py.")
+        
         self.connection = psycopg2.connect(dbname=dbname, user=user, password=password, host=host, port=port)
         self.cursor = self.connection.cursor()
         register_vector(self.connection)
     
     def close_cnxn(self) -> None:
         """
         Close the connection to the database.
```

### Comparing `kitab-0.0.5/kitab/logger/logger.py` & `kitab-0.0.6/kitab/logger/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""
+This module contains the custom formatter for logging messages.
+"""
 import logging
 
 class CustomFormatter(logging.Formatter):
     """ 
     Custom formatter for logging
     
     This class provides a custom formatter for logging messages. It defines different color codes for different log levels and formats the log messages accordingly.
```

### Comparing `kitab-0.0.5/kitab/recommendation_model/models.py` & `kitab-0.0.6/kitab/recommendation_model/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""
+This module contains the functions for recommending books. 
+"""
 import numpy as np
 import pandas as pd
 from ..db.functions import get_table_from_db, get_authors, get_genres
 from kitab.utils import get_embedding, cos_mat_vec, cos_vec_vec
     
 def recommend_books(description: str, n: int, get_available: bool = True, data : pd.DataFrame = None) -> list[dict]:
     """
```

### Comparing `kitab-0.0.5/kitab/utils.py` & `kitab-0.0.6/kitab/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""
+This module contains utility functions for processing data and generating embeddings.
+"""
 import numpy as np
 import pandas as pd
 import math
 import os
 import pickle as pkl
 from sentence_transformers import SentenceTransformer
 from .db.db_info import REQUIRED_COLUMNS
@@ -50,17 +53,16 @@
     
     Returns:
     np.ndarray: The embedding of the text.
     """
     return model.encode(text)    
             
 
-# TODO
 # To add in the future: function gets embedding_func: function = None, or gets the embeddings from the user
-def process_date(data_file: str, destination_folder: str = "data", column_names: dict[str:str] = None, random_availability: bool = False) -> None:
+def process_data(data_file: str, destination_folder: str = "data", column_names: dict[str:str] = None, random_availability: bool = False) -> None:
     """
     Process the given data file, perform data cleaning, and save the processed data and embeddings.
 
     Parameters:
     data_file (str): The path to the data file.
     destination_folder (str): The path to the destination folder where the processed data and embeddings will be saved.
     column_names (dict[str:str], optional): A dictionary mapping required column names to the corresponding column names in the data file. Defaults to None.
```

### Comparing `kitab-0.0.5/kitab.egg-info/SOURCES.txt` & `kitab-0.0.6/kitab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kitab-0.0.5/setup.py` & `kitab-0.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 # Add install requirements
 setup(
     author="Alexander Shahramanyan",
     description="A package for book recommendation.",
     name="kitab",
     packages=find_packages(include=["kitab", "kitab.*"]),
-    version="0.0.5",
+    version="0.0.6",
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
-    install_requires=['pandas', 'sentence-transformers>=2.6', 'psycopg2-binary', 'pgvector'],
+    install_requires=['pandas', 'sentence-transformers>=2.6', 'psycopg2-binary', 'pgvector', 'python-dotenv'],
     python_requires=">=3.7",
 )
```

