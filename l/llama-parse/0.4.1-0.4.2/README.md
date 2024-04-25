# Comparing `tmp/llama_parse-0.4.1.tar.gz` & `tmp/llama_parse-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_parse-0.4.1.tar", max compression
+gzip compressed data, was "llama_parse-0.4.2.tar", max compression
```

## Comparing `llama_parse-0.4.1.tar` & `llama_parse-0.4.2.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1067 2024-04-14 19:10:02.541219 llama_parse-0.4.1/LICENSE
--rw-r--r--   0        0        0     2858 2024-04-14 19:10:02.541219 llama_parse-0.4.1/README.md
--rw-r--r--   0        0        0       92 2024-04-14 19:10:02.557219 llama_parse-0.4.1/llama_parse/__init__.py
--rw-r--r--   0        0        0    15192 2024-04-14 19:10:02.557219 llama_parse-0.4.1/llama_parse/base.py
--rw-r--r--   0        0        0      483 2024-04-14 19:10:02.561219 llama_parse-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     3451 1970-01-01 00:00:00.000000 llama_parse-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-25 02:41:07.980219 llama_parse-0.4.2/LICENSE
+-rw-r--r--   0        0        0     2858 2024-04-25 02:41:07.980219 llama_parse-0.4.2/README.md
+-rw-r--r--   0        0        0       92 2024-04-25 02:41:07.992219 llama_parse-0.4.2/llama_parse/__init__.py
+-rw-r--r--   0        0        0    12892 2024-04-25 02:41:07.992219 llama_parse-0.4.2/llama_parse/base.py
+-rw-r--r--   0        0        0     2819 2024-04-25 02:41:07.996219 llama_parse-0.4.2/llama_parse/utils.py
+-rw-r--r--   0        0        0      483 2024-04-25 02:41:07.996219 llama_parse-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     3451 1970-01-01 00:00:00.000000 llama_parse-0.4.2/PKG-INFO
```

### Comparing `llama_parse-0.4.1/LICENSE` & `llama_parse-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_parse-0.4.1/README.md` & `llama_parse-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `llama_parse-0.4.1/PKG-INFO` & `llama_parse-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-parse
-Version: 0.4.1
+Version: 0.4.2
 Summary: Parse files into RAG-Optimized formats.
 License: MIT
 Author: Logan Markewich
 Author-email: logan@llamaindex.ai
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

