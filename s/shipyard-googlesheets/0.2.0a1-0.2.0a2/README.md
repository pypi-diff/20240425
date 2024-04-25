# Comparing `tmp/shipyard_googlesheets-0.2.0a1.tar.gz` & `tmp/shipyard_googlesheets-0.2.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_googlesheets-0.2.0a1.tar", max compression
+gzip compressed data, was "shipyard_googlesheets-0.2.0a2.tar", max compression
```

## Comparing `shipyard_googlesheets-0.2.0a1.tar` & `shipyard_googlesheets-0.2.0a2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2023-07-26 19:00:30.088676 shipyard_googlesheets-0.2.0a1/README.md
--rw-r--r--   0        0        0      621 2024-04-18 15:52:18.859561 shipyard_googlesheets-0.2.0a1/pyproject.toml
--rw-r--r--   0        0        0       45 2023-05-12 18:48:21.832867 shipyard_googlesheets-0.2.0a1/shipyard_googlesheets/__init__.py
--rw-r--r--   0        0        0        0 2024-02-05 20:53:35.436611 shipyard_googlesheets-0.2.0a1/shipyard_googlesheets/cli/__init__.py
--rw-r--r--   0        0        0      619 2024-04-17 14:16:05.060075 shipyard_googlesheets-0.2.0a1/shipyard_googlesheets/cli/authtest.py
--rw-r--r--   0        0        0     3702 2024-04-18 15:52:06.157346 shipyard_googlesheets-0.2.0a1/shipyard_googlesheets/cli/clear_data.py
--rw-r--r--   0        0        0     4814 2024-04-18 15:32:57.785255 shipyard_googlesheets-0.2.0a1/shipyard_googlesheets/cli/download.py
--rw-r--r--   0        0        0     5715 2024-04-18 15:52:06.173180 shipyard_googlesheets-0.2.0a1/shipyard_googlesheets/cli/upload.py
--rw-r--r--   0        0        0      538 2024-04-17 22:49:13.749017 shipyard_googlesheets-0.2.0a1/shipyard_googlesheets/exceptions.py
--rw-r--r--   0        0        0     1238 2024-04-17 14:16:05.061443 shipyard_googlesheets-0.2.0a1/shipyard_googlesheets/googlesheets.py
--rw-r--r--   0        0        0     5076 2024-04-18 15:52:06.167455 shipyard_googlesheets-0.2.0a1/shipyard_googlesheets/utils.py
--rw-r--r--   0        0        0      770 1970-01-01 00:00:00.000000 shipyard_googlesheets-0.2.0a1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-26 19:00:30.088676 shipyard_googlesheets-0.2.0a2/README.md
+-rw-r--r--   0        0        0      621 2024-04-25 12:57:04.010402 shipyard_googlesheets-0.2.0a2/pyproject.toml
+-rw-r--r--   0        0        0       45 2023-05-12 18:48:21.832867 shipyard_googlesheets-0.2.0a2/shipyard_googlesheets/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-05 20:53:35.436611 shipyard_googlesheets-0.2.0a2/shipyard_googlesheets/cli/__init__.py
+-rw-r--r--   0        0        0      619 2024-04-18 20:05:26.103690 shipyard_googlesheets-0.2.0a2/shipyard_googlesheets/cli/authtest.py
+-rw-r--r--   0        0        0     3702 2024-04-18 20:05:26.104065 shipyard_googlesheets-0.2.0a2/shipyard_googlesheets/cli/clear_data.py
+-rw-r--r--   0        0        0     4849 2024-04-23 15:54:54.518590 shipyard_googlesheets-0.2.0a2/shipyard_googlesheets/cli/download.py
+-rw-r--r--   0        0        0     5715 2024-04-18 20:05:26.104702 shipyard_googlesheets-0.2.0a2/shipyard_googlesheets/cli/upload.py
+-rw-r--r--   0        0        0     1053 2024-04-25 12:56:24.315403 shipyard_googlesheets-0.2.0a2/shipyard_googlesheets/exceptions.py
+-rw-r--r--   0        0        0     1238 2024-04-18 20:05:26.105110 shipyard_googlesheets-0.2.0a2/shipyard_googlesheets/googlesheets.py
+-rw-r--r--   0        0        0     5154 2024-04-25 12:55:47.964225 shipyard_googlesheets-0.2.0a2/shipyard_googlesheets/utils.py
+-rw-r--r--   0        0        0      770 1970-01-01 00:00:00.000000 shipyard_googlesheets-0.2.0a2/PKG-INFO
```

### Comparing `shipyard_googlesheets-0.2.0a1/pyproject.toml` & `shipyard_googlesheets-0.2.0a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "shipyard-googlesheets"
-version = "0.2.0a1"
+version = "0.2.0a2"
 description = "A local client for connecting and working with Google Sheets"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "shipyard_googlesheets"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 google-api-python-client = "2.95.0"
 google-auth-httplib2 = "0.1.0"
 google-auth-oauthlib = "1.0.0"
-shipyard-bp-utils = "^1.2.0"
 shipyard-templates = "^0.8.0"
+shipyard-bp-utils = "^1.2.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `shipyard_googlesheets-0.2.0a1/shipyard_googlesheets/cli/authtest.py` & `shipyard_googlesheets-0.2.0a2/shipyard_googlesheets/cli/authtest.py`

 * *Files identical despite different names*

### Comparing `shipyard_googlesheets-0.2.0a1/shipyard_googlesheets/cli/clear_data.py` & `shipyard_googlesheets-0.2.0a2/shipyard_googlesheets/cli/clear_data.py`

 * *Files identical despite different names*

### Comparing `shipyard_googlesheets-0.2.0a1/shipyard_googlesheets/cli/download.py` & `shipyard_googlesheets-0.2.0a2/shipyard_googlesheets/cli/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             .values()
             .get(spreadsheetId=spreadsheet_id, range=cell_range)
             .execute()
         )
 
         if not sheet.get("values"):
             logger.warning(f"No values for {file_name}.. Not downloading")
-            return
+            raise exceptions.DownloadError(file_name)
 
         values = sheet["values"]
         with open(local_path, "+w") as f:
             writer = csv.writer(f)
             writer.writerows(values)
         logger.info(f"Successfully downloaded {file_name} - {tab_name} to {local_path}")
     except Exception as e:
```

### Comparing `shipyard_googlesheets-0.2.0a1/shipyard_googlesheets/cli/upload.py` & `shipyard_googlesheets-0.2.0a2/shipyard_googlesheets/cli/upload.py`

 * *Files identical despite different names*

### Comparing `shipyard_googlesheets-0.2.0a1/shipyard_googlesheets/googlesheets.py` & `shipyard_googlesheets-0.2.0a2/shipyard_googlesheets/googlesheets.py`

 * *Files identical despite different names*

### Comparing `shipyard_googlesheets-0.2.0a1/shipyard_googlesheets/utils.py` & `shipyard_googlesheets-0.2.0a2/shipyard_googlesheets/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import json
 import os
-import tempfile
 import socket
+import tempfile
 
 from google.oauth2 import service_account
 from googleapiclient.discovery import build
 from shipyard_templates import ShipyardLogger
 
+from shipyard_googlesheets import exceptions
+
 logger = ShipyardLogger.get_logger()
 SCOPES = [
     "https://spreadsheets.google.com/feeds",
     "https://www.googleapis.com/auth/drive",
 ]
 socket.setdefaulttimeout(600)
 
@@ -150,8 +152,8 @@
 
         return (
             service.spreadsheets()
             .batchUpdate(spreadsheetId=spreadsheet_id, body=request_body)
             .execute()
         )
     except Exception as e:
-        logger.error(e)
+        raise exceptions.WorkbookAddException(e) from e
```

### Comparing `shipyard_googlesheets-0.2.0a1/PKG-INFO` & `shipyard_googlesheets-0.2.0a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: shipyard-googlesheets
-Version: 0.2.0a1
+Version: 0.2.0a2
 Summary: A local client for connecting and working with Google Sheets
 License: Apache 2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: google-api-python-client (==2.95.0)
 Requires-Dist: google-auth-httplib2 (==0.1.0)
 Requires-Dist: google-auth-oauthlib (==1.0.0)
-Requires-Dist: shipyard-bp-utils (>=1.2.0,<2.0.0)
+Requires-Dist: shipyard-bp-utils (>=1.2.1,<2.0.0)
 Requires-Dist: shipyard-templates (>=0.8.0,<0.9.0)
 Description-Content-Type: text/markdown
```

