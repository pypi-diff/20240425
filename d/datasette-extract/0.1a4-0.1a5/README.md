# Comparing `tmp/datasette-extract-0.1a4.tar.gz` & `tmp/datasette_extract-0.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette-extract-0.1a4.tar", last modified: Tue Apr  9 19:25:46 2024, max compression
+gzip compressed data, was "datasette_extract-0.1a5.tar", last modified: Wed Apr 24 23:11:57 2024, max compression
```

## Comparing `datasette-extract-0.1a4.tar` & `datasette_extract-0.1a5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:25:46.791438 datasette-extract-0.1a4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-09 19:25:40.000000 datasette-extract-0.1a4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-04-09 19:25:46.791438 datasette-extract-0.1a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-09 19:25:40.000000 datasette-extract-0.1a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:25:46.783438 datasette-extract-0.1a4/datasette_extract/
--rw-r--r--   0 runner    (1001) docker     (127)    15529 2024-04-09 19:25:40.000000 datasette-extract-0.1a4/datasette_extract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:25:46.787438 datasette-extract-0.1a4/datasette_extract/static/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-09 19:25:40.000000 datasette-extract-0.1a4/datasette_extract/static/extract.css
--rw-r--r--   0 runner    (1001) docker     (127)  1352452 2024-04-09 19:25:40.000000 datasette-extract-0.1a4/datasette_extract/static/heic2any-0.0.4.min.js
--rw-r--r--   0 runner    (1001) docker     (127)  1875780 2024-04-09 19:25:40.000000 datasette-extract-0.1a4/datasette_extract/static/pdf.worker.mjs
--rw-r--r--   0 runner    (1001) docker     (127)   317819 2024-04-09 19:25:40.000000 datasette-extract-0.1a4/datasette_extract/static/pdfjs-dist-4-0-379.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:25:46.787438 datasette-extract-0.1a4/datasette_extract/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-04-09 19:25:40.000000 datasette-extract-0.1a4/datasette_extract/templates/_extract_drop_handler.html
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-09 19:25:40.000000 datasette-extract-0.1a4/datasette_extract/templates/extract.html
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-09 19:25:40.000000 datasette-extract-0.1a4/datasette_extract/templates/extract_create_table.html
--rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-04-09 19:25:40.000000 datasette-extract-0.1a4/datasette_extract/templates/extract_progress.html
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-09 19:25:40.000000 datasette-extract-0.1a4/datasette_extract/templates/extract_to_table.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:25:46.787438 datasette-extract-0.1a4/datasette_extract.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-04-09 19:25:46.000000 datasette-extract-0.1a4/datasette_extract.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-09 19:25:46.000000 datasette-extract-0.1a4/datasette_extract.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:25:46.000000 datasette-extract-0.1a4/datasette_extract.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-09 19:25:46.000000 datasette-extract-0.1a4/datasette_extract.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-09 19:25:46.000000 datasette-extract-0.1a4/datasette_extract.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-09 19:25:46.000000 datasette-extract-0.1a4/datasette_extract.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-09 19:25:40.000000 datasette-extract-0.1a4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 19:25:46.791438 datasette-extract-0.1a4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:25:46.787438 datasette-extract-0.1a4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-09 19:25:40.000000 datasette-extract-0.1a4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-09 19:25:40.000000 datasette-extract-0.1a4/tests/test_web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:11:57.680354 datasette_extract-0.1a5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 23:11:45.000000 datasette_extract-0.1a5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-04-24 23:11:57.680354 datasette_extract-0.1a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-24 23:11:45.000000 datasette_extract-0.1a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:11:57.672354 datasette_extract-0.1a5/datasette_extract/
+-rw-r--r--   0 runner    (1001) docker     (127)    16004 2024-04-24 23:11:45.000000 datasette_extract-0.1a5/datasette_extract/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:11:57.680354 datasette_extract-0.1a5/datasette_extract/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-24 23:11:45.000000 datasette_extract-0.1a5/datasette_extract/static/extract.css
+-rw-r--r--   0 runner    (1001) docker     (127)  1352452 2024-04-24 23:11:45.000000 datasette_extract-0.1a5/datasette_extract/static/heic2any-0.0.4.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)  1875780 2024-04-24 23:11:45.000000 datasette_extract-0.1a5/datasette_extract/static/pdf.worker.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)   317819 2024-04-24 23:11:45.000000 datasette_extract-0.1a5/datasette_extract/static/pdfjs-dist-4-0-379.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:11:57.680354 datasette_extract-0.1a5/datasette_extract/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-04-24 23:11:45.000000 datasette_extract-0.1a5/datasette_extract/templates/_extract_drop_handler.html
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-24 23:11:45.000000 datasette_extract-0.1a5/datasette_extract/templates/extract.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-24 23:11:45.000000 datasette_extract-0.1a5/datasette_extract/templates/extract_create_table.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-04-24 23:11:45.000000 datasette_extract-0.1a5/datasette_extract/templates/extract_progress.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-24 23:11:45.000000 datasette_extract-0.1a5/datasette_extract/templates/extract_to_table.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:11:57.680354 datasette_extract-0.1a5/datasette_extract.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-04-24 23:11:57.000000 datasette_extract-0.1a5/datasette_extract.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-24 23:11:57.000000 datasette_extract-0.1a5/datasette_extract.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 23:11:57.000000 datasette_extract-0.1a5/datasette_extract.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-24 23:11:57.000000 datasette_extract-0.1a5/datasette_extract.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-24 23:11:57.000000 datasette_extract-0.1a5/datasette_extract.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-24 23:11:57.000000 datasette_extract-0.1a5/datasette_extract.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-24 23:11:45.000000 datasette_extract-0.1a5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 23:11:57.680354 datasette_extract-0.1a5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:11:57.680354 datasette_extract-0.1a5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-24 23:11:45.000000 datasette_extract-0.1a5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-04-24 23:11:45.000000 datasette_extract-0.1a5/tests/test_web.py
```

### Comparing `datasette-extract-0.1a4/LICENSE` & `datasette_extract-0.1a5/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette-extract-0.1a4/PKG-INFO` & `datasette_extract-0.1a5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: datasette-extract
-Version: 0.1a4
+Version: 0.1a5
 Summary: Import unstructured data (text and images) into structured tables
 Author: Simon Willison
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/datasette/datasette-extract
 Project-URL: Changelog, https://github.com/datasette/datasette-extract/releases
 Project-URL: Issues, https://github.com/datasette/datasette-extract/issues
 Project-URL: CI, https://github.com/datasette/datasette-extract/actions
 Classifier: Framework :: Datasette
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: datasette>=1.0a12
+Requires-Dist: datasette-secrets>=0.1a2
 Requires-Dist: sqlite-utils
 Requires-Dist: openai>=1.0
 Requires-Dist: ijson
 Requires-Dist: python-ulid
 Requires-Dist: starlette
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
@@ -38,15 +39,17 @@
 Install this plugin in the same environment as [Datasette](https://datasette.io/).
 ```bash
 datasette install datasette-extract
 ```
 
 ## Configuration
 
-This plugin requires an `OPENAI_API_KEY` environment variable with an [OpenAI API key](https://platform.openai.com/api-keys).
+This plugin requires an [OpenAI API key](https://platform.openai.com/api-keys).
+
+You can set this using the `DATASETTE_SECRETS_OPENAI_API_KEY` environment variable, or you can configure the [datasette-secrets](https://github.com/datasette/datasette-secrets) plugin to allow users to enter their own plugin and save it, encrypted, in their database.
 
 ## Usage
 
 This plugin provides the following features:
 
 - In the database action cog menu for a database select "Create table with extracted data" to create a new table with data extracted from text or an image
 - In the table action cog menu select "Extract data into this table" to extract data into an existing table
@@ -55,15 +58,15 @@
 
 When populating an existing table you can provide hints and select which columns should be populated.
 
 Text input can be pasted directly into the textarea.
 
 Drag and drop a PDF or text file onto the textarea to populate it with the contents of that file. PDF files will have their text extracted, but only if the file contains text as opposed to scanned images.
 
-Drag and drop a single image onto the textarea - or select it with the image file input box - to process an image. These will have OCR run against them using GPT-4 Vision and then that text will be used for structured data extraction.
+Drag and drop a single image onto the textarea - or select it with the image file input box - to process an image.
 
 ## Permissions
 
 Users must have the `datasette-extract` permission to use this tool.
 
 In order to create tables they also need the `create-table` permission.
```

### Comparing `datasette-extract-0.1a4/README.md` & `datasette_extract-0.1a5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 Install this plugin in the same environment as [Datasette](https://datasette.io/).
 ```bash
 datasette install datasette-extract
 ```
 
 ## Configuration
 
-This plugin requires an `OPENAI_API_KEY` environment variable with an [OpenAI API key](https://platform.openai.com/api-keys).
+This plugin requires an [OpenAI API key](https://platform.openai.com/api-keys).
+
+You can set this using the `DATASETTE_SECRETS_OPENAI_API_KEY` environment variable, or you can configure the [datasette-secrets](https://github.com/datasette/datasette-secrets) plugin to allow users to enter their own plugin and save it, encrypted, in their database.
 
 ## Usage
 
 This plugin provides the following features:
 
 - In the database action cog menu for a database select "Create table with extracted data" to create a new table with data extracted from text or an image
 - In the table action cog menu select "Extract data into this table" to extract data into an existing table
@@ -29,15 +31,15 @@
 
 When populating an existing table you can provide hints and select which columns should be populated.
 
 Text input can be pasted directly into the textarea.
 
 Drag and drop a PDF or text file onto the textarea to populate it with the contents of that file. PDF files will have their text extracted, but only if the file contains text as opposed to scanned images.
 
-Drag and drop a single image onto the textarea - or select it with the image file input box - to process an image. These will have OCR run against them using GPT-4 Vision and then that text will be used for structured data extraction.
+Drag and drop a single image onto the textarea - or select it with the image file input box - to process an image.
 
 ## Permissions
 
 Users must have the `datasette-extract` permission to use this tool.
 
 In order to create tables they also need the `create-table` permission.
```

### Comparing `datasette-extract-0.1a4/datasette_extract/__init__.py` & `datasette_extract-0.1a5/datasette_extract/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
 import base64
 from datasette import hookimpl, Response, NotFound, Permission, Forbidden
+from datasette_secrets import Secret, get_secret
 from datetime import datetime, timezone
-from openai import AsyncOpenAI, OpenAIError
+from openai import AsyncOpenAI
 from sqlite_utils import Database
 from starlette.requests import Request as StarletteRequest
 import ijson
 import json
 import ulid
 
 
@@ -21,14 +22,25 @@
             takes_resource=False,
             default=False,
         )
     ]
 
 
 @hookimpl
+def register_secrets():
+    return [
+        Secret(
+            name="OPENAI_API_KEY",
+            obtain_label="Get an OpenAI API key",
+            obtain_url="https://platform.openai.com/api-keys",
+        ),
+    ]
+
+
+@hookimpl
 def permission_allowed(action, actor):
     if action == "datasette-extract" and actor and actor.get("id") == "root":
         return True
 
 
 async def can_extract(datasette, actor, database_name, to_table=None):
     if actor is None:
@@ -262,15 +274,15 @@
                     "error": None,
                     "num_items": 0,
                 },
                 pk="id",
                 alter=True,
             )
 
-    async_client = AsyncOpenAI()
+    async_client = AsyncOpenAI(api_key=await get_secret(datasette, "OPENAI_API_KEY"))
     db = datasette.get_database(database)
 
     await db.execute_write_fn(start_write)
 
     def make_row_writer(row):
         def _write(conn):
             with conn:
@@ -449,15 +461,17 @@
         return "string"
 
 
 @hookimpl
 def database_actions(datasette, actor, database):
     async def inner():
         if not await can_extract(datasette, actor, database):
-            return []
+            return
+        if not await get_secret(datasette, "OPENAI_API_KEY"):
+            return
         return [
             {
                 "href": datasette.urls.database(database) + "/-/extract",
                 "label": "Create table with AI extracted data",
                 "description": "Paste in text or an image to extract structured data",
             }
         ]
@@ -465,15 +479,17 @@
     return inner
 
 
 @hookimpl
 def table_actions(datasette, actor, database, table):
     async def inner():
         if not await can_extract(datasette, actor, database, table):
-            return []
+            return
+        if not await get_secret(datasette, "OPENAI_API_KEY"):
+            return
         return [
             {
                 "href": datasette.urls.table(database, table) + "/-/extract",
                 "label": "Extract data into this table with AI",
                 "description": "Paste in text or an image to extract structured data",
             }
         ]
```

### Comparing `datasette-extract-0.1a4/datasette_extract/static/heic2any-0.0.4.min.js` & `datasette_extract-0.1a5/datasette_extract/static/heic2any-0.0.4.min.js`

 * *Files identical despite different names*

### Comparing `datasette-extract-0.1a4/datasette_extract/static/pdf.worker.mjs` & `datasette_extract-0.1a5/datasette_extract/static/pdf.worker.mjs`

 * *Files identical despite different names*

### Comparing `datasette-extract-0.1a4/datasette_extract/static/pdfjs-dist-4-0-379.js` & `datasette_extract-0.1a5/datasette_extract/static/pdfjs-dist-4-0-379.js`

 * *Files identical despite different names*

### Comparing `datasette-extract-0.1a4/datasette_extract/templates/_extract_drop_handler.html` & `datasette_extract-0.1a5/datasette_extract/templates/_extract_drop_handler.html`

 * *Files identical despite different names*

### Comparing `datasette-extract-0.1a4/datasette_extract/templates/extract_create_table.html` & `datasette_extract-0.1a5/datasette_extract/templates/extract_create_table.html`

 * *Files identical despite different names*

### Comparing `datasette-extract-0.1a4/datasette_extract/templates/extract_progress.html` & `datasette_extract-0.1a5/datasette_extract/templates/extract_progress.html`

 * *Files identical despite different names*

### Comparing `datasette-extract-0.1a4/datasette_extract/templates/extract_to_table.html` & `datasette_extract-0.1a5/datasette_extract/templates/extract_to_table.html`

 * *Files identical despite different names*

### Comparing `datasette-extract-0.1a4/datasette_extract.egg-info/PKG-INFO` & `datasette_extract-0.1a5/datasette_extract.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: datasette-extract
-Version: 0.1a4
+Version: 0.1a5
 Summary: Import unstructured data (text and images) into structured tables
 Author: Simon Willison
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/datasette/datasette-extract
 Project-URL: Changelog, https://github.com/datasette/datasette-extract/releases
 Project-URL: Issues, https://github.com/datasette/datasette-extract/issues
 Project-URL: CI, https://github.com/datasette/datasette-extract/actions
 Classifier: Framework :: Datasette
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: datasette>=1.0a12
+Requires-Dist: datasette-secrets>=0.1a2
 Requires-Dist: sqlite-utils
 Requires-Dist: openai>=1.0
 Requires-Dist: ijson
 Requires-Dist: python-ulid
 Requires-Dist: starlette
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
@@ -38,15 +39,17 @@
 Install this plugin in the same environment as [Datasette](https://datasette.io/).
 ```bash
 datasette install datasette-extract
 ```
 
 ## Configuration
 
-This plugin requires an `OPENAI_API_KEY` environment variable with an [OpenAI API key](https://platform.openai.com/api-keys).
+This plugin requires an [OpenAI API key](https://platform.openai.com/api-keys).
+
+You can set this using the `DATASETTE_SECRETS_OPENAI_API_KEY` environment variable, or you can configure the [datasette-secrets](https://github.com/datasette/datasette-secrets) plugin to allow users to enter their own plugin and save it, encrypted, in their database.
 
 ## Usage
 
 This plugin provides the following features:
 
 - In the database action cog menu for a database select "Create table with extracted data" to create a new table with data extracted from text or an image
 - In the table action cog menu select "Extract data into this table" to extract data into an existing table
@@ -55,15 +58,15 @@
 
 When populating an existing table you can provide hints and select which columns should be populated.
 
 Text input can be pasted directly into the textarea.
 
 Drag and drop a PDF or text file onto the textarea to populate it with the contents of that file. PDF files will have their text extracted, but only if the file contains text as opposed to scanned images.
 
-Drag and drop a single image onto the textarea - or select it with the image file input box - to process an image. These will have OCR run against them using GPT-4 Vision and then that text will be used for structured data extraction.
+Drag and drop a single image onto the textarea - or select it with the image file input box - to process an image.
 
 ## Permissions
 
 Users must have the `datasette-extract` permission to use this tool.
 
 In order to create tables they also need the `create-table` permission.
```

### Comparing `datasette-extract-0.1a4/datasette_extract.egg-info/SOURCES.txt` & `datasette_extract-0.1a5/datasette_extract.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datasette-extract-0.1a4/pyproject.toml` & `datasette_extract-0.1a5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [project]
 name = "datasette-extract"
-version = "0.1a4"
+version = "0.1a5"
 description = "Import unstructured data (text and images) into structured tables"
 readme = "README.md"
 authors = [{name = "Simon Willison"}]
 license = {text = "Apache-2.0"}
 classifiers=[
     "Framework :: Datasette",
     "License :: OSI Approved :: Apache Software License"
 ]
 requires-python = ">=3.8"
 dependencies = [
     "datasette>=1.0a12",
+    "datasette-secrets>=0.1a2",
     "sqlite-utils",
     "openai>=1.0",
     "ijson",
     "python-ulid",
     "starlette",
 ]
```

### Comparing `datasette-extract-0.1a4/tests/test_web.py` & `datasette_extract-0.1a5/tests/test_web.py`

 * *Files 12% similar despite different names*

```diff
@@ -105,7 +105,32 @@
         fetch_path = "/test/foo"
     html = (await ds.client.get(fetch_path, cookies=cookies)).text
     fragment = f'<a href="{path}"'
     if should_allow:
         assert fragment in html
     else:
         assert fragment not in html
+
+
+@pytest.mark.asyncio
+@pytest.mark.parametrize("path", ("/test2", "/test2/foo"))
+@pytest.mark.parametrize("has_env_variable", (True, False))
+async def test_action_menus_require_api_key(monkeypatch, path, has_env_variable):
+    if not has_env_variable:
+        monkeypatch.delenv("DATASETTE_SECRETS_OPENAI_API_KEY")
+    ds = Datasette(
+        config={
+            "permissions": {
+                "datasette-extract": {"id": "root"},
+            }
+        }
+    )
+    db = ds.add_memory_database("test2")
+    await db.execute_write("create table if not exists foo (id integer primary key)")
+    cookies = {"ds_actor": ds.client.actor_cookie({"id": "root"})}
+    response = await ds.client.get(path, cookies=cookies)
+
+    fragment = '/-/extract"'
+    if has_env_variable:
+        assert fragment in response.text
+    else:
+        assert fragment not in response.text
```

#### html2text {}

```diff
@@ -37,7 +37,17 @@
 ds.client.actor_cookie({"id": actor})} response = await ds.client.get(path,
 cookies=cookies) if should_allow: assert response.status_code == 200 else:
 assert response.status_code == 403 # Also check if the action items were
 visible if path == "/test/-/extract": fetch_path = "/test" else: fetch_path =
 "/test/foo" html = (await ds.client.get(fetch_path, cookies=cookies)).text
 fragment = f'
  if should_allow: assert fragment in html else: assert fragment not in html
+@pytest.mark.asyncio @pytest.mark.parametrize("path", ("/test2", "/test2/foo"))
+@pytest.mark.parametrize("has_env_variable", (True, False)) async def
+test_action_menus_require_api_key(monkeypatch, path, has_env_variable): if not
+has_env_variable: monkeypatch.delenv("DATASETTE_SECRETS_OPENAI_API_KEY") ds =
+Datasette( config={ "permissions": { "datasette-extract": {"id": "root"}, } } )
+db = ds.add_memory_database("test2") await db.execute_write("create table if
+not exists foo (id integer primary key)") cookies = {"ds_actor":
+ds.client.actor_cookie({"id": "root"})} response = await ds.client.get(path,
+cookies=cookies) fragment = '/-/extract"' if has_env_variable: assert fragment
+in response.text else: assert fragment not in response.text
```

