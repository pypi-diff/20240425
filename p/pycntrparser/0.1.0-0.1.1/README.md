# Comparing `tmp/pycntrparser-0.1.0.tar.gz` & `tmp/pycntrparser-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycntrparser-0.1.0.tar", max compression
+gzip compressed data, was "pycntrparser-0.1.1.tar", max compression
```

## Comparing `pycntrparser-0.1.0.tar` & `pycntrparser-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,16 @@
--rw-r--r--   0        0        0     1095 2023-09-13 08:25:16.959836 pycntrparser-0.1.0/LICENSE
--rw-r--r--   0        0        0      351 2024-01-10 11:03:15.410275 pycntrparser-0.1.0/pycntrparser/__init__.py
--rw-r--r--   0        0        0      199 2023-09-13 08:15:15.832955 pycntrparser-0.1.0/pycntrparser/args/parse.py
--rw-r--r--   0        0        0      350 2023-11-28 09:39:48.574744 pycntrparser-0.1.0/pycntrparser/ErrorListener.py
--rw-r--r--   0        0        0      194 2023-12-17 14:17:01.534807 pycntrparser-0.1.0/pycntrparser/expand.py
--rw-r--r--   0        0        0      564 2023-11-28 09:36:49.438743 pycntrparser-0.1.0/pycntrparser/parse.py
--rw-r--r--   0        0        0      514 2023-09-13 09:37:57.952873 pycntrparser-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      900 2024-01-10 11:15:21.577727 pycntrparser-0.1.0/README.md
--rw-r--r--   0        0        0     1423 1970-01-01 00:00:00.000000 pycntrparser-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1095 2024-04-25 11:55:00.405315 pycntrparser-0.1.1/LICENSE
+-rw-r--r--   0        0        0      351 2024-04-25 11:55:00.408362 pycntrparser-0.1.1/pycntrparser/__init__.py
+-rw-r--r--   0        0        0      199 2024-04-25 11:55:00.411047 pycntrparser-0.1.1/pycntrparser/args/parse.py
+-rw-r--r--   0        0        0    10237 2024-04-25 11:58:55.961557 pycntrparser-0.1.1/pycntrparser/CNTR.interp
+-rw-r--r--   0        0        0      607 2024-04-25 11:58:56.133443 pycntrparser-0.1.1/pycntrparser/CNTR.tokens
+-rw-r--r--   0        0        0     4468 2024-04-25 11:58:55.859402 pycntrparser-0.1.1/pycntrparser/CNTRLexer.interp
+-rw-r--r--   0        0        0     5641 2024-04-25 11:58:55.921899 pycntrparser-0.1.1/pycntrparser/CNTRLexer.py
+-rw-r--r--   0        0        0      607 2024-04-25 11:58:55.921899 pycntrparser-0.1.1/pycntrparser/CNTRLexer.tokens
+-rw-r--r--   0        0        0    13182 2024-04-25 11:58:56.117821 pycntrparser-0.1.1/pycntrparser/CNTRListener.py
+-rw-r--r--   0        0        0    93486 2024-04-25 11:58:56.117821 pycntrparser-0.1.1/pycntrparser/CNTRParser.py
+-rw-r--r--   0        0        0      350 2024-04-25 11:55:00.408362 pycntrparser-0.1.1/pycntrparser/ErrorListener.py
+-rw-r--r--   0        0        0      194 2024-04-25 11:55:00.411836 pycntrparser-0.1.1/pycntrparser/expand.py
+-rw-r--r--   0        0        0      564 2024-04-25 11:55:00.411836 pycntrparser-0.1.1/pycntrparser/parse.py
+-rw-r--r--   0        0        0      548 2024-04-25 12:00:30.689326 pycntrparser-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      900 2024-04-25 11:55:00.405315 pycntrparser-0.1.1/README.md
+-rw-r--r--   0        0        0     1474 1970-01-01 00:00:00.000000 pycntrparser-0.1.1/PKG-INFO
```

### Comparing `pycntrparser-0.1.0/LICENSE` & `pycntrparser-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycntrparser-0.1.0/pycntrparser/parse.py` & `pycntrparser-0.1.1/pycntrparser/parse.py`

 * *Files identical despite different names*

### Comparing `pycntrparser-0.1.0/pyproject.toml` & `pycntrparser-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "pycntrparser"
-version = "0.1.0"
+version = "0.1.1"
 description = "Parse CNTR transcriptions using ANTLR4"
 authors = ["Ivan Dustin Bilon <ivan22.dust@gmail.com>"]
 license = "MIT"
 readme = "README.md"
+include = ["pycntrparser/CNTR*"]
 
 [tool.poetry.scripts]
 cntr-check = "pycntrparser.__init__:main"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 antlr4-python3-runtime = "^4.13.1"
```

### Comparing `pycntrparser-0.1.0/README.md` & `pycntrparser-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pycntrparser-0.1.0/PKG-INFO` & `pycntrparser-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: pycntrparser
-Version: 0.1.0
+Version: 0.1.1
 Summary: Parse CNTR transcriptions using ANTLR4
 License: MIT
 Author: Ivan Dustin Bilon
 Author-email: ivan22.dust@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: antlr4-python3-runtime (>=4.13.1,<5.0.0)
 Description-Content-Type: text/markdown
 
 # pycntrparser
 
 ## Description
```

