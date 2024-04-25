# Comparing `tmp/webexception-1.0.4.tar.gz` & `tmp/webexception-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webexception-1.0.4.tar", max compression
+gzip compressed data, was "webexception-1.0.5.tar", max compression
```

## Comparing `webexception-1.0.4.tar` & `webexception-1.0.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     6185 2023-06-20 15:11:48.458636 webexception-1.0.4/README.md
--rw-r--r--   0        0        0      566 2023-07-03 12:45:09.159457 webexception-1.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-20 15:13:03.845839 webexception-1.0.4/webexception/__init__.py
--rw-r--r--   0        0        0      643 2023-07-03 12:45:03.967482 webexception-1.0.4/webexception/webexception.py
--rw-r--r--   0        0        0     6478 1970-01-01 00:00:00.000000 webexception-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     6185 2023-06-20 15:11:48.458636 webexception-1.0.5/README.md
+-rw-r--r--   0        0        0      565 2024-04-25 07:53:14.323553 webexception-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-20 15:13:03.845839 webexception-1.0.5/webexception/__init__.py
+-rw-r--r--   0        0        0      643 2023-07-03 12:45:03.967482 webexception-1.0.5/webexception/webexception.py
+-rw-r--r--   0        0        0     6578 1970-01-01 00:00:00.000000 webexception-1.0.5/PKG-INFO
```

### Comparing `webexception-1.0.4/README.md` & `webexception-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `webexception-1.0.4/pyproject.toml` & `webexception-1.0.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "webexception"
-version = "1.0.4"
+version = "1.0.5"
 description = ""
 authors = ["Marco Bartel <bsimpson888@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.9"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `webexception-1.0.4/webexception/webexception.py` & `webexception-1.0.5/webexception/webexception.py`

 * *Files identical despite different names*

### Comparing `webexception-1.0.4/PKG-INFO` & `webexception-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: webexception
-Version: 1.0.4
+Version: 1.0.5
 Summary: 
 Author: Marco Bartel
 Author-email: bsimpson888@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # webexception
```

