# Comparing `tmp/llama_index_vector_stores_pinecone-0.1.5.tar.gz` & `tmp/llama_index_vector_stores_pinecone-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_vector_stores_pinecone-0.1.5.tar", max compression
+gzip compressed data, was "llama_index_vector_stores_pinecone-0.1.6.tar", max compression
```

## Comparing `llama_index_vector_stores_pinecone-0.1.5.tar` & `llama_index_vector_stores_pinecone-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       49 2024-04-22 16:36:26.335350 llama_index_vector_stores_pinecone-0.1.5/README.md
--rw-r--r--   0        0        0      107 2024-04-22 16:36:26.335350 llama_index_vector_stores_pinecone-0.1.5/llama_index/vector_stores/pinecone/__init__.py
--rw-r--r--   0        0        0    16721 2024-04-22 16:36:26.335350 llama_index_vector_stores_pinecone-0.1.5/llama_index/vector_stores/pinecone/base.py
--rw-r--r--   0        0        0      814 2024-04-22 16:36:26.335350 llama_index_vector_stores_pinecone-0.1.5/llama_index/vector_stores/pinecone/utils.py
--rw-r--r--   0        0        0     1502 2024-04-22 16:36:26.335350 llama_index_vector_stores_pinecone-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      674 1970-01-01 00:00:00.000000 llama_index_vector_stores_pinecone-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       49 2024-04-25 19:49:25.720608 llama_index_vector_stores_pinecone-0.1.6/README.md
+-rw-r--r--   0        0        0      107 2024-04-25 19:49:25.720608 llama_index_vector_stores_pinecone-0.1.6/llama_index/vector_stores/pinecone/__init__.py
+-rw-r--r--   0        0        0    16915 2024-04-25 19:49:25.720608 llama_index_vector_stores_pinecone-0.1.6/llama_index/vector_stores/pinecone/base.py
+-rw-r--r--   0        0        0      814 2024-04-25 19:49:25.720608 llama_index_vector_stores_pinecone-0.1.6/llama_index/vector_stores/pinecone/utils.py
+-rw-r--r--   0        0        0     1502 2024-04-25 19:49:25.720608 llama_index_vector_stores_pinecone-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      674 1970-01-01 00:00:00.000000 llama_index_vector_stores_pinecone-0.1.6/PKG-INFO
```

### Comparing `llama_index_vector_stores_pinecone-0.1.5/llama_index/vector_stores/pinecone/base.py` & `llama_index_vector_stores_pinecone-0.1.6/llama_index/vector_stores/pinecone/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,19 @@
     """Convert from standard dataclass to pinecone filter dict."""
     filters = {}
     filters_list = []
     condition = standard_filters.condition or "and"
     condition = _transform_pinecone_filter_condition(condition)
     if standard_filters.filters:
         for filter in standard_filters.filters:
-            if filter.operator:
+            if isinstance(filter, MetadataFilters):
+                sub_filter = _to_pinecone_filter(filter)
+                if sub_filter:
+                    filters_list.append(sub_filter)
+            elif filter.operator:
                 filters_list.append(
                     {
                         filter.key: {
                             _transform_pinecone_filter_operator(
                                 filter.operator
                             ): filter.value
                         }
```

### Comparing `llama_index_vector_stores_pinecone-0.1.5/llama_index/vector_stores/pinecone/utils.py` & `llama_index_vector_stores_pinecone-0.1.6/llama_index/vector_stores/pinecone/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_vector_stores_pinecone-0.1.5/pyproject.toml` & `llama_index_vector_stores_pinecone-0.1.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index vector_stores pinecone integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-vector-stores-pinecone"
 readme = "README.md"
-version = "0.1.5"
+version = "0.1.6"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.13"
 llama-index-core = "^0.10.11.post1"
 pinecone-client = "^3.0.2"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_vector_stores_pinecone-0.1.5/PKG-INFO` & `llama_index_vector_stores_pinecone-0.1.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-vector-stores-pinecone
-Version: 0.1.5
+Version: 0.1.6
 Summary: llama-index vector_stores pinecone integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

