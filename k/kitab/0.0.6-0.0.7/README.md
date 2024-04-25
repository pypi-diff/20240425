# Comparing `tmp/kitab-0.0.6.tar.gz` & `tmp/kitab-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kitab-0.0.6.tar", last modified: Thu Apr 25 18:17:07 2024, max compression
+gzip compressed data, was "kitab-0.0.7.tar", last modified: Thu Apr 25 18:39:57 2024, max compression
```

## Comparing `kitab-0.0.6.tar` & `kitab-0.0.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 18:17:07.469263 kitab-0.0.6/
--rw-rw-rw-   0        0        0     1100 2024-04-07 17:53:03.000000 kitab-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      478 2024-04-25 18:17:07.466216 kitab-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     4274 2024-04-25 14:50:27.000000 kitab-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 18:17:07.400076 kitab-0.0.6/kitab/
--rw-rw-rw-   0        0        0      131 2024-04-08 06:51:45.000000 kitab-0.0.6/kitab/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 18:17:07.428100 kitab-0.0.6/kitab/api/
--rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.6/kitab/api/__init__.py
--rw-rw-rw-   0        0        0     7500 2024-04-25 14:26:03.000000 kitab-0.0.6/kitab/api/app.py
-drwxrwxrwx   0        0        0        0 2024-04-25 18:17:07.443007 kitab-0.0.6/kitab/db/
--rw-rw-rw-   0        0        0      370 2024-04-21 06:34:18.000000 kitab-0.0.6/kitab/db/__init__.py
--rw-rw-rw-   0        0        0     2206 2024-04-25 13:49:11.000000 kitab-0.0.6/kitab/db/db_info.py
--rw-rw-rw-   0        0        0    15703 2024-04-25 14:41:33.000000 kitab-0.0.6/kitab/db/functions.py
--rw-rw-rw-   0        0        0     4993 2024-04-25 13:50:18.000000 kitab-0.0.6/kitab/db/get_data.py
--rw-rw-rw-   0        0        0    12309 2024-04-25 14:41:05.000000 kitab-0.0.6/kitab/db/sql_interactions.py
-drwxrwxrwx   0        0        0        0 2024-04-25 18:17:07.449895 kitab-0.0.6/kitab/logger/
--rw-rw-rw-   0        0        0       37 2024-04-07 17:53:03.000000 kitab-0.0.6/kitab/logger/__init__.py
--rw-rw-rw-   0        0        0     1812 2024-04-25 14:42:46.000000 kitab-0.0.6/kitab/logger/logger.py
-drwxrwxrwx   0        0        0        0 2024-04-25 18:17:07.454394 kitab-0.0.6/kitab/recommendation_model/
--rw-rw-rw-   0        0        0       88 2024-04-08 13:12:13.000000 kitab-0.0.6/kitab/recommendation_model/__init__.py
--rw-rw-rw-   0        0        0     4216 2024-04-25 14:23:05.000000 kitab-0.0.6/kitab/recommendation_model/models.py
--rw-rw-rw-   0        0        0     4657 2024-04-25 14:43:09.000000 kitab-0.0.6/kitab/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-25 18:17:07.464378 kitab-0.0.6/kitab.egg-info/
--rw-rw-rw-   0        0        0      478 2024-04-25 18:17:07.000000 kitab-0.0.6/kitab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      523 2024-04-25 18:17:07.000000 kitab-0.0.6/kitab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 18:17:07.000000 kitab-0.0.6/kitab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2024-04-25 18:17:07.000000 kitab-0.0.6/kitab.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-25 18:17:07.000000 kitab-0.0.6/kitab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 18:17:07.469263 kitab-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      592 2024-04-25 18:17:00.000000 kitab-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 18:17:07.462945 kitab-0.0.6/tests/
--rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.6/tests/test_module1.py
--rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.6/tests/test_module2.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:39:57.972271 kitab-0.0.7/
+-rw-rw-rw-   0        0        0     1100 2024-04-07 17:53:03.000000 kitab-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      478 2024-04-25 18:39:57.962576 kitab-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4274 2024-04-25 14:50:27.000000 kitab-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 18:39:57.905976 kitab-0.0.7/kitab/
+-rw-rw-rw-   0        0        0      131 2024-04-08 06:51:45.000000 kitab-0.0.7/kitab/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:39:57.935125 kitab-0.0.7/kitab/api/
+-rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.7/kitab/api/__init__.py
+-rw-rw-rw-   0        0        0     7500 2024-04-25 14:26:03.000000 kitab-0.0.7/kitab/api/app.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:39:57.950271 kitab-0.0.7/kitab/db/
+-rw-rw-rw-   0        0        0      370 2024-04-21 06:34:18.000000 kitab-0.0.7/kitab/db/__init__.py
+-rw-rw-rw-   0        0        0     2193 2024-04-25 18:32:29.000000 kitab-0.0.7/kitab/db/db_info.py
+-rw-rw-rw-   0        0        0    15703 2024-04-25 14:41:33.000000 kitab-0.0.7/kitab/db/functions.py
+-rw-rw-rw-   0        0        0     4993 2024-04-25 13:50:18.000000 kitab-0.0.7/kitab/db/get_data.py
+-rw-rw-rw-   0        0        0    12309 2024-04-25 14:41:05.000000 kitab-0.0.7/kitab/db/sql_interactions.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:39:57.955262 kitab-0.0.7/kitab/logger/
+-rw-rw-rw-   0        0        0       37 2024-04-07 17:53:03.000000 kitab-0.0.7/kitab/logger/__init__.py
+-rw-rw-rw-   0        0        0     1812 2024-04-25 14:42:46.000000 kitab-0.0.7/kitab/logger/logger.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:39:57.959610 kitab-0.0.7/kitab/recommendation_model/
+-rw-rw-rw-   0        0        0       88 2024-04-08 13:12:13.000000 kitab-0.0.7/kitab/recommendation_model/__init__.py
+-rw-rw-rw-   0        0        0     4216 2024-04-25 14:23:05.000000 kitab-0.0.7/kitab/recommendation_model/models.py
+-rw-rw-rw-   0        0        0     4769 2024-04-25 18:32:53.000000 kitab-0.0.7/kitab/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:39:57.962576 kitab-0.0.7/kitab.egg-info/
+-rw-rw-rw-   0        0        0      478 2024-04-25 18:39:57.000000 kitab-0.0.7/kitab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      523 2024-04-25 18:39:57.000000 kitab-0.0.7/kitab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 18:39:57.000000 kitab-0.0.7/kitab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-04-25 18:39:57.000000 kitab-0.0.7/kitab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-25 18:39:57.000000 kitab-0.0.7/kitab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 18:39:57.972271 kitab-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      592 2024-04-25 18:39:48.000000 kitab-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:39:57.962576 kitab-0.0.7/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.7/tests/test_module1.py
+-rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.7/tests/test_module2.py
```

### Comparing `kitab-0.0.6/LICENSE` & `kitab-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kitab-0.0.6/README.md` & `kitab-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `kitab-0.0.6/kitab/api/app.py` & `kitab-0.0.7/kitab/api/app.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.6/kitab/db/db_info.py` & `kitab-0.0.7/kitab/db/db_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Get DB credentials from the environment variables
 DB_USER = os.getenv("DB_USER")
 DB_PASSWORD = os.getenv("DB_PASSWORD")
 DB_HOST = os.getenv("DB_HOST")
 DB_PORT = os.getenv("DB_PORT")
 DB_NAME = os.getenv("DB_NAME")
 
-REQUIRED_COLUMNS = ["isbn", "title", "description", "author", "genre", "available"]
+REQUIRED_COLUMNS = ["isbn", "title", "description", "author", "genre"]
 
 COMMANDS = (
     "CREATE EXTENSION IF NOT EXISTS vector;"
 
     "DROP TABLE IF EXISTS BookAuthor;",
         
     "DROP TABLE IF EXISTS Author;",
```

### Comparing `kitab-0.0.6/kitab/db/functions.py` & `kitab-0.0.7/kitab/db/functions.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.6/kitab/db/get_data.py` & `kitab-0.0.7/kitab/db/get_data.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.6/kitab/db/sql_interactions.py` & `kitab-0.0.7/kitab/db/sql_interactions.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.6/kitab/logger/logger.py` & `kitab-0.0.7/kitab/logger/logger.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.6/kitab/recommendation_model/models.py` & `kitab-0.0.7/kitab/recommendation_model/models.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.6/kitab/utils.py` & `kitab-0.0.7/kitab/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,23 +54,24 @@
     Returns:
     np.ndarray: The embedding of the text.
     """
     return model.encode(text)    
             
 
 # To add in the future: function gets embedding_func: function = None, or gets the embeddings from the user
-def process_data(data_file: str, destination_folder: str = "data", column_names: dict[str:str] = None, random_availability: bool = False) -> None:
+def process_data(data_file: str, destination_folder: str = "data", column_names: dict[str:str] = None, random_availability: bool = False, chunk_size: int = 20000) -> None:
     """
     Process the given data file, perform data cleaning, and save the processed data and embeddings.
 
     Parameters:
     data_file (str): The path to the data file.
     destination_folder (str): The path to the destination folder where the processed data and embeddings will be saved.
     column_names (dict[str:str], optional): A dictionary mapping required column names to the corresponding column names in the data file. Defaults to None.
     random_availability (bool, optional): If True, add random book availability to the data. If False, the data must contain an 'availability' column. Defaults to False.
+    chunk_size (int, optional): The size of the chunks to split the data into. Defaults to 20000.
 
     Returns:
         None
     """
     # Check the destination folder
     if not os.path.exists(destination_folder):
         os.makedirs(destination_folder)
@@ -84,17 +85,17 @@
     for req_col in REQUIRED_COLUMNS:
         if (column_names and column_names[req_col] not in data.columns) or req_col not in data.columns:
                 raise Exception(f"{req_col} column required, but missing in the given data.")
     
     if random_availability:
         # Add random book availability
         np.random.seed(42)
-        data['availability'] = np.random.choice([True, False], size=len(data), p=[0.3, 0.7])
-    elif (column_names and column_names["availability"] not in data.columns) or "availability" not in data.columns:
-        raise Exception("Availability column required, but missing in the given data. Either add it, or set random_availability to True.")
+        data['available'] = np.random.choice([True, False], size=len(data), p=[0.3, 0.7])
+    elif (column_names and column_names["available"] not in data.columns) or "available" not in data.columns:
+        raise Exception("available column required, but missing in the given data. Either add it, or set random_availability to True.")
     
     # Rename the columns to the default column names
     if column_names:
         reverse_mapping = {v: k for k, v in column_names.items()}
         data.rename(columns=reverse_mapping, inplace=True)
     
     # TODO data cleaning here, you need to be able to explain what you did and why
```

### Comparing `kitab-0.0.6/kitab.egg-info/SOURCES.txt` & `kitab-0.0.7/kitab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kitab-0.0.6/setup.py` & `kitab-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Add install requirements
 setup(
     author="Alexander Shahramanyan",
     description="A package for book recommendation.",
     name="kitab",
     packages=find_packages(include=["kitab", "kitab.*"]),
-    version="0.0.6",
+    version="0.0.7",
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     install_requires=['pandas', 'sentence-transformers>=2.6', 'psycopg2-binary', 'pgvector', 'python-dotenv'],
     python_requires=">=3.7",
```

