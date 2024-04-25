# Comparing `tmp/ALLMDEV-1.2.2-py3-none-any.whl.zip` & `tmp/ALLMDEV-1.2.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,15 @@
-Zip file size: 6787 bytes, number of entries: 10
+Zip file size: 10608 bytes, number of entries: 13
 -rw-rw-rw-  2.0 fat       39 b- defN 24-Apr-17 06:01 ALLMDEV/__init__.py
 -rw-rw-rw-  2.0 fat     1904 b- defN 24-Apr-20 05:31 ALLMDEV/api.py
 -rw-rw-rw-  2.0 fat      757 b- defN 24-Apr-17 06:35 ALLMDEV/cli.py
 -rw-rw-rw-  2.0 fat     2579 b- defN 24-Apr-20 10:27 ALLMDEV/generate.py
 -rw-rw-rw-  2.0 fat    10334 b- defN 24-Apr-19 14:10 ALLMDEV/instruct.py
--rw-rw-rw-  2.0 fat     2366 b- defN 24-Apr-20 10:27 ALLMDEV-1.2.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-20 10:27 ALLMDEV-1.2.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       81 b- defN 24-Apr-20 10:27 ALLMDEV-1.2.2.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-20 10:27 ALLMDEV-1.2.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      760 b- defN 24-Apr-20 10:27 ALLMDEV-1.2.2.dist-info/RECORD
-10 files, 18920 bytes uncompressed, 5499 bytes compressed:  70.9%
+-rw-rw-rw-  2.0 fat     1985 b- defN 24-Apr-25 11:09 ALLMDEV/rag.py
+-rw-rw-rw-  2.0 fat     3016 b- defN 24-Apr-25 07:21 ALLMDEV/ragrun.py
+-rw-rw-rw-  2.0 fat     3144 b- defN 24-Apr-25 07:25 ALLMDEV/ragserve.py
+-rw-rw-rw-  2.0 fat     2538 b- defN 24-Apr-25 11:10 ALLMDEV-1.2.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-25 11:10 ALLMDEV-1.2.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      183 b- defN 24-Apr-25 11:10 ALLMDEV-1.2.3.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-25 11:10 ALLMDEV-1.2.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      982 b- defN 24-Apr-25 11:10 ALLMDEV-1.2.3.dist-info/RECORD
+13 files, 27561 bytes uncompressed, 8992 bytes compressed:  67.4%
```

## zipnote {}

```diff
@@ -9,23 +9,32 @@
 
 Filename: ALLMDEV/generate.py
 Comment: 
 
 Filename: ALLMDEV/instruct.py
 Comment: 
 
-Filename: ALLMDEV-1.2.2.dist-info/METADATA
+Filename: ALLMDEV/rag.py
 Comment: 
 
-Filename: ALLMDEV-1.2.2.dist-info/WHEEL
+Filename: ALLMDEV/ragrun.py
 Comment: 
 
-Filename: ALLMDEV-1.2.2.dist-info/entry_points.txt
+Filename: ALLMDEV/ragserve.py
 Comment: 
 
-Filename: ALLMDEV-1.2.2.dist-info/top_level.txt
+Filename: ALLMDEV-1.2.3.dist-info/METADATA
 Comment: 
 
-Filename: ALLMDEV-1.2.2.dist-info/RECORD
+Filename: ALLMDEV-1.2.3.dist-info/WHEEL
+Comment: 
+
+Filename: ALLMDEV-1.2.3.dist-info/entry_points.txt
+Comment: 
+
+Filename: ALLMDEV-1.2.3.dist-info/top_level.txt
+Comment: 
+
+Filename: ALLMDEV-1.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ALLMDEV-1.2.2.dist-info/METADATA` & `ALLMDEV-1.2.3.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: ALLMDEV
-Version: 1.2.2
+Version: 1.2.3
 Summary: A simple and efficient python library for fast inference of GGUF Large Language Models.
 Author: All Advance AI
 Author-email: allmdev@allaai.com
 Maintainer: Soham Ghadge
 Maintainer-email: soham.ghadge@allaai.com
 Keywords: GGUF,GGUF Large Language Model,GGUF Large Language Models,GGUF Large Language Modeling,GGUF Large Language Modeling Library
 Description-Content-Type: text/markdown
 Requires-Dist: Flask
 Requires-Dist: click
 Requires-Dist: llama-index
 Requires-Dist: llama-cpp-python
 Requires-Dist: aiohttp
 Requires-Dist: llama-index-llms-llama-cpp
 Requires-Dist: huggingface-hub
+Requires-Dist: langchain ==0.0.267
+Requires-Dist: chromadb ==0.3.26
+Requires-Dist: pdfminer.six
+Requires-Dist: pydantic ==1.10.13
+Requires-Dist: sentence-transformers
 
 # ALLM
 
 ALLM is a Python library designed for fast inference of GGUF (Generic Global Unsupervised Features) Large Language Models (LLMs) on both CPU and GPU. It provides a convenient interface for loading pre-trained GGUF models and performing inference using them. This library is ideal for applications where quick response times are crucial, such as chatbots, text generation, and more.
 
 ## Features
```

