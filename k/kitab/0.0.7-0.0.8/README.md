# Comparing `tmp/kitab-0.0.7.tar.gz` & `tmp/kitab-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kitab-0.0.7.tar", last modified: Thu Apr 25 18:39:57 2024, max compression
+gzip compressed data, was "kitab-0.0.8.tar", last modified: Thu Apr 25 18:49:54 2024, max compression
```

## Comparing `kitab-0.0.7.tar` & `kitab-0.0.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 18:39:57.972271 kitab-0.0.7/
--rw-rw-rw-   0        0        0     1100 2024-04-07 17:53:03.000000 kitab-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      478 2024-04-25 18:39:57.962576 kitab-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     4274 2024-04-25 14:50:27.000000 kitab-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 18:39:57.905976 kitab-0.0.7/kitab/
--rw-rw-rw-   0        0        0      131 2024-04-08 06:51:45.000000 kitab-0.0.7/kitab/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 18:39:57.935125 kitab-0.0.7/kitab/api/
--rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.7/kitab/api/__init__.py
--rw-rw-rw-   0        0        0     7500 2024-04-25 14:26:03.000000 kitab-0.0.7/kitab/api/app.py
-drwxrwxrwx   0        0        0        0 2024-04-25 18:39:57.950271 kitab-0.0.7/kitab/db/
--rw-rw-rw-   0        0        0      370 2024-04-21 06:34:18.000000 kitab-0.0.7/kitab/db/__init__.py
--rw-rw-rw-   0        0        0     2193 2024-04-25 18:32:29.000000 kitab-0.0.7/kitab/db/db_info.py
--rw-rw-rw-   0        0        0    15703 2024-04-25 14:41:33.000000 kitab-0.0.7/kitab/db/functions.py
--rw-rw-rw-   0        0        0     4993 2024-04-25 13:50:18.000000 kitab-0.0.7/kitab/db/get_data.py
--rw-rw-rw-   0        0        0    12309 2024-04-25 14:41:05.000000 kitab-0.0.7/kitab/db/sql_interactions.py
-drwxrwxrwx   0        0        0        0 2024-04-25 18:39:57.955262 kitab-0.0.7/kitab/logger/
--rw-rw-rw-   0        0        0       37 2024-04-07 17:53:03.000000 kitab-0.0.7/kitab/logger/__init__.py
--rw-rw-rw-   0        0        0     1812 2024-04-25 14:42:46.000000 kitab-0.0.7/kitab/logger/logger.py
-drwxrwxrwx   0        0        0        0 2024-04-25 18:39:57.959610 kitab-0.0.7/kitab/recommendation_model/
--rw-rw-rw-   0        0        0       88 2024-04-08 13:12:13.000000 kitab-0.0.7/kitab/recommendation_model/__init__.py
--rw-rw-rw-   0        0        0     4216 2024-04-25 14:23:05.000000 kitab-0.0.7/kitab/recommendation_model/models.py
--rw-rw-rw-   0        0        0     4769 2024-04-25 18:32:53.000000 kitab-0.0.7/kitab/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-25 18:39:57.962576 kitab-0.0.7/kitab.egg-info/
--rw-rw-rw-   0        0        0      478 2024-04-25 18:39:57.000000 kitab-0.0.7/kitab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      523 2024-04-25 18:39:57.000000 kitab-0.0.7/kitab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 18:39:57.000000 kitab-0.0.7/kitab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2024-04-25 18:39:57.000000 kitab-0.0.7/kitab.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-25 18:39:57.000000 kitab-0.0.7/kitab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 18:39:57.972271 kitab-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      592 2024-04-25 18:39:48.000000 kitab-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 18:39:57.962576 kitab-0.0.7/tests/
--rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.7/tests/test_module1.py
--rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.7/tests/test_module2.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:49:54.045028 kitab-0.0.8/
+-rw-rw-rw-   0        0        0     1100 2024-04-07 17:53:03.000000 kitab-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      499 2024-04-25 18:49:54.036514 kitab-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4274 2024-04-25 14:50:27.000000 kitab-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 18:49:53.869655 kitab-0.0.8/kitab/
+-rw-rw-rw-   0        0        0      131 2024-04-08 06:51:45.000000 kitab-0.0.8/kitab/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:49:53.936463 kitab-0.0.8/kitab/api/
+-rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.8/kitab/api/__init__.py
+-rw-rw-rw-   0        0        0     7498 2024-04-25 18:43:54.000000 kitab-0.0.8/kitab/api/app.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:49:53.969900 kitab-0.0.8/kitab/db/
+-rw-rw-rw-   0        0        0      370 2024-04-21 06:34:18.000000 kitab-0.0.8/kitab/db/__init__.py
+-rw-rw-rw-   0        0        0     2193 2024-04-25 18:32:29.000000 kitab-0.0.8/kitab/db/db_info.py
+-rw-rw-rw-   0        0        0    15669 2024-04-25 18:43:52.000000 kitab-0.0.8/kitab/db/functions.py
+-rw-rw-rw-   0        0        0     4993 2024-04-25 13:50:18.000000 kitab-0.0.8/kitab/db/get_data.py
+-rw-rw-rw-   0        0        0    12306 2024-04-25 18:43:52.000000 kitab-0.0.8/kitab/db/sql_interactions.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:49:53.997425 kitab-0.0.8/kitab/logger/
+-rw-rw-rw-   0        0        0       37 2024-04-07 17:53:03.000000 kitab-0.0.8/kitab/logger/__init__.py
+-rw-rw-rw-   0        0        0     1811 2024-04-25 18:43:52.000000 kitab-0.0.8/kitab/logger/logger.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:49:54.013513 kitab-0.0.8/kitab/recommendation_model/
+-rw-rw-rw-   0        0        0       88 2024-04-08 13:12:13.000000 kitab-0.0.8/kitab/recommendation_model/__init__.py
+-rw-rw-rw-   0        0        0     4216 2024-04-25 14:23:05.000000 kitab-0.0.8/kitab/recommendation_model/models.py
+-rw-rw-rw-   0        0        0     5309 2024-04-25 18:48:31.000000 kitab-0.0.8/kitab/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:49:54.020814 kitab-0.0.8/kitab.egg-info/
+-rw-rw-rw-   0        0        0      499 2024-04-25 18:49:53.000000 kitab-0.0.8/kitab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      523 2024-04-25 18:49:53.000000 kitab-0.0.8/kitab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 18:49:53.000000 kitab-0.0.8/kitab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2024-04-25 18:49:53.000000 kitab-0.0.8/kitab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-25 18:49:53.000000 kitab-0.0.8/kitab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 18:49:54.045028 kitab-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      600 2024-04-25 18:49:38.000000 kitab-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:49:54.020814 kitab-0.0.8/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.8/tests/test_module1.py
+-rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.8/tests/test_module2.py
```

### Comparing `kitab-0.0.7/LICENSE` & `kitab-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `kitab-0.0.7/README.md` & `kitab-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `kitab-0.0.7/kitab/api/app.py` & `kitab-0.0.8/kitab/api/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,26 +107,26 @@
         return {"message": "Nothing passed."}
     
     # Compare the old book with the new one
     new_book = new_book.model_dump()
     old_book= get_book_by_ISBN(isbn)
     
     # Remove unchanged fields
-    logging.info("Removing unchanged fields.")
+    logger.info("Removing unchanged fields.")
     to_remove = []
     for field in new_book:
         if old_book[field] == new_book[field] or new_book[field] is None:
             to_remove.append(field)
             
     for field in to_remove:
         new_book.pop(field)
 
     # If no fields to be changed remained, return a message
     if len(new_book.keys()) == 0:
-        logging.info("No fields to be updated.")
+        logger.info("No fields to be updated.")
         return {"message": "Nothing new passed."}
 
     # Update the book
     if update_book_db(isbn, new_book):
         return {"message": "Book updated successfully"}
     
     return {"message": "Something went wrong. Book not updated."}
```

### Comparing `kitab-0.0.7/kitab/db/db_info.py` & `kitab-0.0.8/kitab/db/db_info.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.7/kitab/db/functions.py` & `kitab-0.0.8/kitab/db/functions.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,23 +25,23 @@
 
     Returns:
     dict or None: A dictionary containing the book information if found, or None if no book is found.
     """
 
     # Open connection to the database
     db = SqlHandler(DB_NAME, user=DB_USER, password=DB_PASSWORD, host=DB_HOST, port=DB_PORT)
-    logging.info("Database connection opened.")
+    logger.info("Database connection opened.")
     
     # Retrieve the book with the given ISBN
     book = db.get_table("book", conditions={"isbn": ISBN})
     
     if len(book) == 0:
-        logging.info("Book not found.")
+        logger.info("Book not found.")
         return None
-    logging.info("Book retrieved.")
+    logger.info("Book retrieved.")
     
     book_author = db.get_table("bookauthor", conditions={"isbn": ISBN})
     book_genre = db.get_table("bookgenre", conditions={"isbn": ISBN})
         
     # If no book found, return None
     if len(book) == 0:
         return None, None, None
@@ -50,26 +50,26 @@
     book = book.to_dict(orient='records')[0]
 
     author_ids = book_author["author_id"].tolist()
     authors = []
     if len(author_ids) > 0:
         author = db.get_table("author", conditions={"author_id": author_ids})
         authors = author["full_name"].tolist()
-        logging.info(f"Authors retrieved.")
+        logger.info(f"Authors retrieved.")
     else:
-        logging.info("No authors found.")
+        logger.info("No authors found.")
     
     genre_ids = book_genre["genre_id"].tolist()
     genres = []
     if len(genre_ids) > 0:
         genre = db.get_table("genre", conditions={"genre_id": genre_ids})
         genres = genre["genre"].tolist()
-        logging.info(f"Genres retrieved.")
+        logger.info(f"Genres retrieved.")
     else:
-        logging.info("No genres found.")
+        logger.info("No genres found.")
     
     book["authors"] = authors
     book["genres"] = genres
 
     # Return the book
     return book
 
@@ -82,26 +82,26 @@
     title (str): The title of the book to retrieve.
 
     Returns:
     dict or None: A dictionary containing the book information if found, or None if no book is found.
     """
     # Open connection to the database
     db = SqlHandler(DB_NAME, user=DB_USER, password=DB_PASSWORD, host=DB_HOST, port=DB_PORT)
-    logging.info("Database connection opened.")
+    logger.info("Database connection opened.")
     
     # Retrieve the book with the given title
     books = db.get_table("book", conditions={"title": title})
     
     print(books)
     
     if len(books) == 0:
-        logging.info("Book not found.")
+        logger.info("Book not found.")
         return None
     else:
-        logging.info("Book ISBN retrieved.")
+        logger.info("Book ISBN retrieved.")
         ISBN = books["isbn"].values[0]
 
     # Return the book
     return get_book_by_ISBN(ISBN)
 
 
 def add_book_db(book: dict) -> bool:
@@ -113,47 +113,47 @@
     
     Returns:
     bool: True if the book was successfully added, False otherwise.
     """
     try:
         # Open connection to the database
         db = SqlHandler(DB_NAME, user=DB_USER, password=DB_PASSWORD, host=DB_HOST, port=DB_PORT)
-        logging.info("Database connection opened.")
+        logger.info("Database connection opened.")
             
         # Extract information from the book dictionary
         ISBN = book["isbn"]
         title = book["title"]
         description = book["description"]
         available = book["available"]
         embedding = get_embedding(book["description"]).tolist()
         
         db.insert_records("book", [{"isbn": ISBN, "title": title, "description": description, "embedding": embedding, "available": available}])
-        logging.info("Book table populated.")
+        logger.info("Book table populated.")
         
         # Add author(s) to the author table if doesn't exist
         authors = book["authors"]
         if len(authors) > 0:
-            logging.info("Authors to be added.")
+            logger.info("Authors to be added.")
             author_ids = _get_or_add_authors(db, authors)
             
             db.insert_records("bookauthor", [{"isbn": ISBN, "author_id": int(author_id)} for author_id in author_ids])
-            logging.info("Author table populated.")
+            logger.info("Author table populated.")
         else:
-            logging.info("No authors to be added.")
+            logger.info("No authors to be added.")
         
         # Add genres to the genres table if doesn't exist
         genres = book["genres"]    
         if len(genres) > 0:
-            logging.info("Genres to be added.")
+            logger.info("Genres to be added.")
             genre_ids = _get_or_add_genres(db, genres)
             
             db.insert_records("bookgenre", [{"isbn": ISBN, "genre_id": int(genre_id)} for genre_id in genre_ids])
-            logging.info("Genre table populated.")
+            logger.info("Genre table populated.")
         else:
-            logging.info("No genres to be added.")
+            logger.info("No genres to be added.")
 
         return True
     except:
         return False    
     
 def update_book_db(ISBN: str, new_book: dict) -> bool:
     """
@@ -165,15 +165,15 @@
     
     Returns:
     bool: True if the book was successfully updated, False otherwise.
     """
     try:
         # Open connection to the database
         db = SqlHandler(DB_NAME, user=DB_USER, password=DB_PASSWORD, host=DB_HOST, port=DB_PORT)
-        logging.info("Database connection opened.")
+        logger.info("Database connection opened.")
         
         condition = {"ISBN": ISBN}
         new_values = {}
         
         latest_ISBN = ISBN
         
         for key in new_book.keys():
@@ -181,57 +181,57 @@
                 new_values[key] = new_book[key]
             if key == "ISBN":
                 latest_ISBN = new_book["ISBN"]
             if key == "description":
                 new_values["embedding"] = get_embedding(new_book["description"]).tolist()
 
         db.update_records("book", new_values, condition)
-        logging.info("Book table updated.")
+        logger.info("Book table updated.")
         
         ISBN = latest_ISBN
         
         # Get the tables
         book_author = db.get_table("bookauthor", conditions={"isbn": ISBN})
         book_genre = db.get_table("bookgenre", conditions={"isbn": ISBN})
         
         # Add author(s) to the author table if doesn't exist
         if "authors" in new_book:
-            logging.info("Authors to be updated.")
+            logger.info("Authors to be updated.")
             
             authors = new_book["authors"]
             new_author_ids = set(_get_or_add_authors(db, authors))
             current_author_ids = set(book_author[book_author["isbn"] == ISBN]["author_id"].tolist())
             
             removed_authors = current_author_ids - new_author_ids
             added_authors = new_author_ids - current_author_ids
             
             db.remove_records("bookauthor", [{"isbn": ISBN, "author_id": int(removed_author)} for removed_author in removed_authors])
             db.insert_records("bookauthor", [{"isbn": ISBN, "author_id": int(added_author)} for added_author in added_authors])
             
-            logging.info("Author table updated.")
+            logger.info("Author table updated.")
         else:
-            logging.info("No authors to be updated.")
+            logger.info("No authors to be updated.")
         
         # Add genres to the genres table if doesn't exist
         if "genres" in new_book:
-            logging.info("Genres to be updated.")
+            logger.info("Genres to be updated.")
             
             genres = new_book["genres"]    
             new_genre_ids = set(_get_or_add_genres(db, genres))
             current_genre_ids = set(book_genre[book_genre["isbn"] == ISBN]["genre_id"].tolist())
         
             removed_genres = current_genre_ids - new_genre_ids
             added_genres = new_genre_ids - current_genre_ids
             
             db.remove_records("bookgenre", [{"isbn": ISBN, "genre_id": int(removed_genre)} for removed_genre in removed_genres])
             db.insert_records("bookgenre", [{"isbn": ISBN, "genre_id": int(added_genre)} for added_genre in added_genres])
             
-            logging.info("Genre table updated.")
+            logger.info("Genre table updated.")
         else:
-            logging.info("No genres to be updated.")
+            logger.info("No genres to be updated.")
             
         return True
     except:
         return False
 
 def get_table_from_db(table_name: str, conditions: dict = None) -> pd.DataFrame:
     """
@@ -242,23 +242,23 @@
     conditions (dict): A dictionary of conditions to filter the table.
 
     Returns:
     pd.DataFrame: A DataFrame containing the table information.
     """
     # Open connection to the database
     db = SqlHandler(DB_NAME, user=DB_USER, password=DB_PASSWORD, host=DB_HOST, port=DB_PORT)
-    logging.info("Database connection opened.")
+    logger.info("Database connection opened.")
     
     # Retrieve the table from the database
     if conditions:
         table = db.get_table(table_name, conditions=conditions)
     else:
         table = db.get_table(table_name)
         
-    logging.info(f"Table {table_name} retrieved.")
+    logger.info(f"Table {table_name} retrieved.")
     
     # Return the table
     return table
 
 def _get_or_add_genres(db: SqlHandler, genres: list[str]) -> list[int]:
     """
     Get the genre IDs for the given list of genres. If the genres do not exist in the database, add them to the genre table.
@@ -283,15 +283,15 @@
             genre_id = cur_index
             cur_index += 1
             to_insert.append({"genre_id": genre_id, "genre": genre})
         genre_ids.append(genre_id)
     
     # Insert the records
     db.insert_records("genre", to_insert)
-    logging.info("New genres added.")
+    logger.info("New genres added.")
     
     return genre_ids
 
 def _get_or_add_authors(db: SqlHandler, authors: list[str]) -> list[int]:
     """
     Get the author IDs for the given list of authors. If the authors do not exist in the database, add them to the author table.
 
@@ -315,15 +315,15 @@
             author_id = cur_index
             cur_index += 1
             to_insert.append({"author_id": author_id, "full_name": author})
         author_ids.append(author_id)
     
     # Insert the records
     db.insert_records("author", to_insert)
-    logging.info("New authors added.")
+    logger.info("New authors added.")
     
     return author_ids
 
 def get_authors(ISBNs: list[str]) -> dict[str:list]:
     """
     Get the authors for the given list of ISBNs.
     
@@ -331,15 +331,15 @@
     ISBNs (list[str]): A list of ISBNs.
 
     Returns:
     dict[str:list]: A dictionary containing the authors for each ISBN.
     """
     # Open connection to the database
     db = SqlHandler(DB_NAME, user=DB_USER, password=DB_PASSWORD, host=DB_HOST, port=DB_PORT)
-    logging.info("Database connection opened.")
+    logger.info("Database connection opened.")
     
     # Retrieve the authors of the books with the given ISBNs
     authors = db.get_table("bookauthor", conditions={"isbn": ISBNs})
     author_ids = authors["author_id"].tolist()
     
     author_table = db.get_table("author", conditions={"author_id": author_ids})
     
@@ -364,15 +364,15 @@
     ISBNs (list[str]): A list of ISBNs.
 
     Returns:
     dict[str:list]: A dictionary containing the genres for each ISBN.
     """
     # Open connection to the database
     db = SqlHandler(DB_NAME, user=DB_USER, password=DB_PASSWORD, host=DB_HOST, port=DB_PORT)
-    logging.info("Database connection opened.")
+    logger.info("Database connection opened.")
 
     # Retrieve the genres of the books with the given ISBNs
     genres = db.get_table("bookgenre", conditions={"isbn": ISBNs})
     genre_ids = genres["genre_id"].tolist()
     
     genre_table = db.get_table("genre", conditions={"genre_id": genre_ids})
     
@@ -398,15 +398,15 @@
     recommendation_ISBN (str): The ISBN of the recommended book.
 
     Returns:
     dict: A dictionary containing the history of recommendations for the book.
     """
     # Open connection to the database
     db = SqlHandler(DB_NAME, user=DB_USER, password=DB_PASSWORD, host=DB_HOST, port=DB_PORT)
-    logging.info("Database connection opened.")
+    logger.info("Database connection opened.")
     
     # Retrieve the history of books that have been recommended
     history = db.get_table("history", conditions={"recommendation_ISBN": recommendation_isbn})
     
     # Return the history
     return history.drop(columns="log_id").to_dict(orient='records')
 
@@ -422,15 +422,15 @@
 
     Returns:
     bool: True if the recommendation log was successfully added, False otherwise.
     """
     try:
         # Open connection to the database
         db = SqlHandler(DB_NAME, user=DB_USER, password=DB_PASSWORD, host=DB_HOST, port=DB_PORT)
-        logging.info("Database connection opened.")
+        logger.info("Database connection opened.")
         
         # Insert the recommendation log into the history table
         db.insert_records("history", [{"description": description, "recommendation_ISBN": recommendation_ISBN, "successful": successful}])
     
         return True
     except Exception as e:
         print(e)
```

### Comparing `kitab-0.0.7/kitab/db/get_data.py` & `kitab-0.0.8/kitab/db/get_data.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.7/kitab/db/sql_interactions.py` & `kitab-0.0.8/kitab/db/sql_interactions.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,36 +127,36 @@
         table_name (str): The name of the table to be truncated.
 
         Returns:
         None
         """
         query = f""" TRUNCATE TABLE {table_name} CASCADE; """   #if exists
         self.cursor.execute(query)
-        logging.info(f'the {table_name} is truncated')
+        logger.info(f'the {table_name} is truncated')
         # self.cursor.close()
 
 
     def drop_table(self, table_name: str) -> None:
         """
         Drops a table from the database if it exists.
 
         Parameters:
         table_name (str): The name of the table to be dropped.
 
         Returns:
         None
         """
         query = f"DROP TABLE IF EXISTS {table_name};"
-        logging.info(query)
+        logger.info(query)
 
         self.cursor.execute(query)
 
         self.close_cnxn.commit()
 
-        logging.info(f"table '{table_name}' deleted.")
+        logger.info(f"table '{table_name}' deleted.")
         logger.debug('using drop table function')
 
 
     # def from_sql_to_pandas(self, chunksize:int, id_value:str, table_name: str) -> pd.DataFrame:
         
     #     offset=0
     #     dfs=[]
```

### Comparing `kitab-0.0.7/kitab/logger/logger.py` & `kitab-0.0.8/kitab/logger/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     yellow = "\x1b[33;20m"
     red = "\x1b[31;20m"
     bold_red = "\x1b[31;1m"
     reset = "\x1b[0m"
     format = "%(asctime)s - %(name)s - %(funcName)s - %(levelname)s - (%(message)s) - line: %(lineno)d"
     FORMATS = {
         logging.DEBUG: grey + format + reset,
-        logging.INFO: violet + format + reset,
+        logger.info: violet + format + reset,
         logging.WARNING: yellow + format + reset,
         logging.ERROR: red + format + reset,
         logging.CRITICAL: bold_red + format + reset
     }
 
     def format(self, record):
         """
```

### Comparing `kitab-0.0.7/kitab/recommendation_model/models.py` & `kitab-0.0.8/kitab/recommendation_model/models.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.7/kitab/utils.py` & `kitab-0.0.8/kitab/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,25 @@
 import numpy as np
 import pandas as pd
 import math
 import os
 import pickle as pkl
 from sentence_transformers import SentenceTransformer
 from .db.db_info import REQUIRED_COLUMNS
+from tqdm import tqdm
+import logging
 
+from .logger.logger import CustomFormatter
+
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.DEBUG)
+ch = logging.StreamHandler()
+ch.setLevel(logging.DEBUG)
+ch.setFormatter(CustomFormatter())
+logger.addHandler(ch)
 
 model = SentenceTransformer('sentence-transformers/all-MiniLM-L6-v2')
 
 def cos_vec_vec(vector1: np.ndarray, vector2: np.ndarray) -> float:
     """
     Compute the cosine similarity between two vectors.
     
@@ -77,38 +87,45 @@
         os.makedirs(destination_folder)
     elif os.listdir(destination_folder):
         raise Exception(f"Folder '{destination_folder}' is not empty.")
             
     # Load the data
     data = pd.read_csv(data_file)
     
+    logger.info("Data loaded successfully.")
+    
     # Make sure all required columns present
     for req_col in REQUIRED_COLUMNS:
         if (column_names and column_names[req_col] not in data.columns) or req_col not in data.columns:
                 raise Exception(f"{req_col} column required, but missing in the given data.")
     
     if random_availability:
         # Add random book availability
         np.random.seed(42)
         data['available'] = np.random.choice([True, False], size=len(data), p=[0.3, 0.7])
+        logger.info("Available column added.")
     elif (column_names and column_names["available"] not in data.columns) or "available" not in data.columns:
         raise Exception("available column required, but missing in the given data. Either add it, or set random_availability to True.")
     
+    logger.info("All columns available.")
+
     # Rename the columns to the default column names
     if column_names:
         reverse_mapping = {v: k for k, v in column_names.items()}
         data.rename(columns=reverse_mapping, inplace=True)
     
     # TODO data cleaning here, you need to be able to explain what you did and why
     
-    split_len = 20000
+    data = data[[REQUIRED_COLUMNS] + ["available"]]
+    
+    split_len = chunk_size
     split_data = [data[idx*split_len:(idx+1)*split_len] for idx in range(math.ceil(len(data)/split_len))]
 
-    for idx, d_part in enumerate(split_data):
-        
+    logger.info("Starting computing the embeddings.")
+    for idx, d_part in tqdm(enumerate(split_data)):        
         # Save the d_part as a CSV
         d_part.to_csv(f"{destination_folder}/data_{idx}.csv", index=False)
         
         # Generate embeddings for the cleaned descriptions
         embeddings = model.encode(d_part["description"].tolist())
 
         # Save the embeddings as a pickle file
```

### Comparing `kitab-0.0.7/kitab.egg-info/SOURCES.txt` & `kitab-0.0.8/kitab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kitab-0.0.7/setup.py` & `kitab-0.0.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 # Add install requirements
 setup(
     author="Alexander Shahramanyan",
     description="A package for book recommendation.",
     name="kitab",
     packages=find_packages(include=["kitab", "kitab.*"]),
-    version="0.0.7",
+    version="0.0.8",
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
-    install_requires=['pandas', 'sentence-transformers>=2.6', 'psycopg2-binary', 'pgvector', 'python-dotenv'],
+    install_requires=['pandas', 'sentence-transformers>=2.6', 'psycopg2-binary', 'pgvector', 'python-dotenv', 'tqdm'],
     python_requires=">=3.7",
 )
```

