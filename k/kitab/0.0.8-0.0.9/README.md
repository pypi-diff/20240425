# Comparing `tmp/kitab-0.0.8.tar.gz` & `tmp/kitab-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kitab-0.0.8.tar", last modified: Thu Apr 25 18:49:54 2024, max compression
+gzip compressed data, was "kitab-0.0.9.tar", last modified: Thu Apr 25 18:53:57 2024, max compression
```

## Comparing `kitab-0.0.8.tar` & `kitab-0.0.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 18:49:54.045028 kitab-0.0.8/
--rw-rw-rw-   0        0        0     1100 2024-04-07 17:53:03.000000 kitab-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      499 2024-04-25 18:49:54.036514 kitab-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     4274 2024-04-25 14:50:27.000000 kitab-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 18:49:53.869655 kitab-0.0.8/kitab/
--rw-rw-rw-   0        0        0      131 2024-04-08 06:51:45.000000 kitab-0.0.8/kitab/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 18:49:53.936463 kitab-0.0.8/kitab/api/
--rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.8/kitab/api/__init__.py
--rw-rw-rw-   0        0        0     7498 2024-04-25 18:43:54.000000 kitab-0.0.8/kitab/api/app.py
-drwxrwxrwx   0        0        0        0 2024-04-25 18:49:53.969900 kitab-0.0.8/kitab/db/
--rw-rw-rw-   0        0        0      370 2024-04-21 06:34:18.000000 kitab-0.0.8/kitab/db/__init__.py
--rw-rw-rw-   0        0        0     2193 2024-04-25 18:32:29.000000 kitab-0.0.8/kitab/db/db_info.py
--rw-rw-rw-   0        0        0    15669 2024-04-25 18:43:52.000000 kitab-0.0.8/kitab/db/functions.py
--rw-rw-rw-   0        0        0     4993 2024-04-25 13:50:18.000000 kitab-0.0.8/kitab/db/get_data.py
--rw-rw-rw-   0        0        0    12306 2024-04-25 18:43:52.000000 kitab-0.0.8/kitab/db/sql_interactions.py
-drwxrwxrwx   0        0        0        0 2024-04-25 18:49:53.997425 kitab-0.0.8/kitab/logger/
--rw-rw-rw-   0        0        0       37 2024-04-07 17:53:03.000000 kitab-0.0.8/kitab/logger/__init__.py
--rw-rw-rw-   0        0        0     1811 2024-04-25 18:43:52.000000 kitab-0.0.8/kitab/logger/logger.py
-drwxrwxrwx   0        0        0        0 2024-04-25 18:49:54.013513 kitab-0.0.8/kitab/recommendation_model/
--rw-rw-rw-   0        0        0       88 2024-04-08 13:12:13.000000 kitab-0.0.8/kitab/recommendation_model/__init__.py
--rw-rw-rw-   0        0        0     4216 2024-04-25 14:23:05.000000 kitab-0.0.8/kitab/recommendation_model/models.py
--rw-rw-rw-   0        0        0     5309 2024-04-25 18:48:31.000000 kitab-0.0.8/kitab/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-25 18:49:54.020814 kitab-0.0.8/kitab.egg-info/
--rw-rw-rw-   0        0        0      499 2024-04-25 18:49:53.000000 kitab-0.0.8/kitab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      523 2024-04-25 18:49:53.000000 kitab-0.0.8/kitab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 18:49:53.000000 kitab-0.0.8/kitab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2024-04-25 18:49:53.000000 kitab-0.0.8/kitab.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-25 18:49:53.000000 kitab-0.0.8/kitab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 18:49:54.045028 kitab-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      600 2024-04-25 18:49:38.000000 kitab-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 18:49:54.020814 kitab-0.0.8/tests/
--rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.8/tests/test_module1.py
--rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.8/tests/test_module2.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:53:57.004573 kitab-0.0.9/
+-rw-rw-rw-   0        0        0     1100 2024-04-07 17:53:03.000000 kitab-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      499 2024-04-25 18:53:57.003070 kitab-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4274 2024-04-25 14:50:27.000000 kitab-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 18:53:56.936387 kitab-0.0.9/kitab/
+-rw-rw-rw-   0        0        0      131 2024-04-08 06:51:45.000000 kitab-0.0.9/kitab/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:53:56.960994 kitab-0.0.9/kitab/api/
+-rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.9/kitab/api/__init__.py
+-rw-rw-rw-   0        0        0     7496 2024-04-25 18:53:20.000000 kitab-0.0.9/kitab/api/app.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:53:56.979446 kitab-0.0.9/kitab/db/
+-rw-rw-rw-   0        0        0      370 2024-04-21 06:34:18.000000 kitab-0.0.9/kitab/db/__init__.py
+-rw-rw-rw-   0        0        0     2193 2024-04-25 18:32:29.000000 kitab-0.0.9/kitab/db/db_info.py
+-rw-rw-rw-   0        0        0    15667 2024-04-25 18:53:20.000000 kitab-0.0.9/kitab/db/functions.py
+-rw-rw-rw-   0        0        0     4993 2024-04-25 13:50:18.000000 kitab-0.0.9/kitab/db/get_data.py
+-rw-rw-rw-   0        0        0    12304 2024-04-25 18:53:20.000000 kitab-0.0.9/kitab/db/sql_interactions.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:53:56.987321 kitab-0.0.9/kitab/logger/
+-rw-rw-rw-   0        0        0       37 2024-04-07 17:53:03.000000 kitab-0.0.9/kitab/logger/__init__.py
+-rw-rw-rw-   0        0        0     1812 2024-04-25 18:53:05.000000 kitab-0.0.9/kitab/logger/logger.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:53:56.988122 kitab-0.0.9/kitab/recommendation_model/
+-rw-rw-rw-   0        0        0       88 2024-04-08 13:12:13.000000 kitab-0.0.9/kitab/recommendation_model/__init__.py
+-rw-rw-rw-   0        0        0     4216 2024-04-25 14:23:05.000000 kitab-0.0.9/kitab/recommendation_model/models.py
+-rw-rw-rw-   0        0        0     5307 2024-04-25 18:53:20.000000 kitab-0.0.9/kitab/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:53:56.994810 kitab-0.0.9/kitab.egg-info/
+-rw-rw-rw-   0        0        0      499 2024-04-25 18:53:56.000000 kitab-0.0.9/kitab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      523 2024-04-25 18:53:56.000000 kitab-0.0.9/kitab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 18:53:56.000000 kitab-0.0.9/kitab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2024-04-25 18:53:56.000000 kitab-0.0.9/kitab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-25 18:53:56.000000 kitab-0.0.9/kitab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 18:53:57.004573 kitab-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      600 2024-04-25 18:53:45.000000 kitab-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:53:56.994810 kitab-0.0.9/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.9/tests/test_module1.py
+-rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.9/tests/test_module2.py
```

### Comparing `kitab-0.0.8/LICENSE` & `kitab-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kitab-0.0.8/README.md` & `kitab-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `kitab-0.0.8/kitab/api/app.py` & `kitab-0.0.9/kitab/api/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 """
 from ..db.functions import get_book_by_ISBN, get_book_by_title, add_book_db, update_book_db, add_recommendation_log, get_history_by_recommendation_isbn
 from ..recommendation_model.models import recommend_books, recommend_books_by_ISBN, recommend_books_by_title
 from fastapi import FastAPI
 from pydantic import BaseModel
 import uvicorn
 import logging
-
 from ..logger.logger import CustomFormatter
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 ch = logging.StreamHandler()
 ch.setLevel(logging.DEBUG)
 ch.setFormatter(CustomFormatter())
```

### Comparing `kitab-0.0.8/kitab/db/db_info.py` & `kitab-0.0.9/kitab/db/db_info.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.8/kitab/db/functions.py` & `kitab-0.0.9/kitab/db/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 This module contains tailored functions for interacting with the database. These are used by the API and the recommendation model.
 """
 import pandas as pd
 from kitab.utils import get_embedding
 from .db_info import DB_USER, DB_PASSWORD, DB_HOST, DB_PORT, DB_NAME
 from .sql_interactions import SqlHandler
 import logging
-
 from ..logger.logger import CustomFormatter
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 ch = logging.StreamHandler()
 ch.setLevel(logging.DEBUG)
 ch.setFormatter(CustomFormatter())
```

### Comparing `kitab-0.0.8/kitab/db/get_data.py` & `kitab-0.0.9/kitab/db/get_data.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.8/kitab/db/sql_interactions.py` & `kitab-0.0.9/kitab/db/sql_interactions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """
 This module contains the functions for interacting with the SQL database.
 """
 import psycopg2
 from pgvector.psycopg2 import register_vector
-import logging
 import pandas as pd
 import numpy as np
-
+import logging
 from ..logger.logger import CustomFormatter
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 ch = logging.StreamHandler()
 ch.setLevel(logging.DEBUG)
 ch.setFormatter(CustomFormatter())
```

### Comparing `kitab-0.0.8/kitab/logger/logger.py` & `kitab-0.0.9/kitab/logger/logger.py`

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
-        logger.info: violet + format + reset,
+        logging.INFO: violet + format + reset,
         logging.WARNING: yellow + format + reset,
         logging.ERROR: red + format + reset,
         logging.CRITICAL: bold_red + format + reset
     }
 
     def format(self, record):
         """
```

### Comparing `kitab-0.0.8/kitab/recommendation_model/models.py` & `kitab-0.0.9/kitab/recommendation_model/models.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.8/kitab/utils.py` & `kitab-0.0.9/kitab/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import math
 import os
 import pickle as pkl
 from sentence_transformers import SentenceTransformer
 from .db.db_info import REQUIRED_COLUMNS
 from tqdm import tqdm
 import logging
-
 from .logger.logger import CustomFormatter
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 ch = logging.StreamHandler()
 ch.setLevel(logging.DEBUG)
 ch.setFormatter(CustomFormatter())
```

### Comparing `kitab-0.0.8/kitab.egg-info/SOURCES.txt` & `kitab-0.0.9/kitab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kitab-0.0.8/setup.py` & `kitab-0.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 # Add install requirements
 setup(
     author="Alexander Shahramanyan",
     description="A package for book recommendation.",
     name="kitab",
     packages=find_packages(include=["kitab", "kitab.*"]),
-    version="0.0.8",
+    version="0.0.9",
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     install_requires=['pandas', 'sentence-transformers>=2.6', 'psycopg2-binary', 'pgvector', 'python-dotenv', 'tqdm'],
-    python_requires=">=3.7",
+    python_requires=">=3.9",
 )
```

