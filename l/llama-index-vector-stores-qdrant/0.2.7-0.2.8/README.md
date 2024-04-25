# Comparing `tmp/llama_index_vector_stores_qdrant-0.2.7.tar.gz` & `tmp/llama_index_vector_stores_qdrant-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_vector_stores_qdrant-0.2.7.tar", max compression
+gzip compressed data, was "llama_index_vector_stores_qdrant-0.2.8.tar", max compression
```

## Comparing `llama_index_vector_stores_qdrant-0.2.7.tar` & `llama_index_vector_stores_qdrant-0.2.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       47 2024-04-24 16:49:49.341016 llama_index_vector_stores_qdrant-0.2.7/README.md
--rw-r--r--   0        0        0      101 2024-04-24 16:49:49.341016 llama_index_vector_stores_qdrant-0.2.7/llama_index/vector_stores/qdrant/__init__.py
--rw-r--r--   0        0        0    34385 2024-04-24 16:49:49.341016 llama_index_vector_stores_qdrant-0.2.7/llama_index/vector_stores/qdrant/base.py
--rw-r--r--   0        0        0     6897 2024-04-24 16:49:49.341016 llama_index_vector_stores_qdrant-0.2.7/llama_index/vector_stores/qdrant/utils.py
--rw-r--r--   0        0        0     1600 2024-04-24 16:49:49.345016 llama_index_vector_stores_qdrant-0.2.7/pyproject.toml
--rw-r--r--   0        0        0      723 1970-01-01 00:00:00.000000 llama_index_vector_stores_qdrant-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0       47 2024-04-25 19:49:25.720608 llama_index_vector_stores_qdrant-0.2.8/README.md
+-rw-r--r--   0        0        0      101 2024-04-25 19:49:25.720608 llama_index_vector_stores_qdrant-0.2.8/llama_index/vector_stores/qdrant/__init__.py
+-rw-r--r--   0        0        0    35207 2024-04-25 19:49:25.720608 llama_index_vector_stores_qdrant-0.2.8/llama_index/vector_stores/qdrant/base.py
+-rw-r--r--   0        0        0     6897 2024-04-25 19:49:25.720608 llama_index_vector_stores_qdrant-0.2.8/llama_index/vector_stores/qdrant/utils.py
+-rw-r--r--   0        0        0     1600 2024-04-25 19:49:25.720608 llama_index_vector_stores_qdrant-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0      723 1970-01-01 00:00:00.000000 llama_index_vector_stores_qdrant-0.2.8/PKG-INFO
```

### Comparing `llama_index_vector_stores_qdrant-0.2.7/llama_index/vector_stores/qdrant/base.py` & `llama_index_vector_stores_qdrant-0.2.8/llama_index/vector_stores/qdrant/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 from llama_index.core.schema import BaseNode, MetadataMode, TextNode
 from llama_index.core.utils import iter_batch
 from llama_index.core.vector_stores.types import (
     BasePydanticVectorStore,
     VectorStoreQuery,
     VectorStoreQueryMode,
     VectorStoreQueryResult,
+    MetadataFilters,
+    FilterOperator,
+    FilterCondition,
 )
 from llama_index.core.vector_stores.utils import (
     legacy_metadata_dict_to_node,
     metadata_dict_to_node,
     node_to_metadata_dict,
 )
 from llama_index.vector_stores.qdrant.utils import (
@@ -764,114 +767,130 @@
                 )
             nodes.append(node)
             similarities.append(point.score)
             ids.append(str(point.id))
 
         return VectorStoreQueryResult(nodes=nodes, similarities=similarities, ids=ids)
 
-    def _build_query_filter(self, query: VectorStoreQuery) -> Optional[Any]:
-        if not query.doc_ids and not query.query_str:
-            return None
-
-        must_conditions = []
-
-        if query.doc_ids:
-            must_conditions.append(
-                FieldCondition(
-                    key="doc_id",
-                    match=MatchAny(any=query.doc_ids),
-                )
-            )
-
-        # Point id is a “service” id, it is not stored in payload. There is ‘HasId’ condition to filter by point id
-        # https://qdrant.tech/documentation/concepts/filtering/#has-id
-        if query.node_ids:
-            must_conditions.append(
-                HasIdCondition(has_id=query.node_ids),
-            )
-
-        # Qdrant does not use the query.query_str property for the filtering. Full-text
-        # filtering cannot handle longer queries and can effectively filter our all the
-        # nodes. See: https://github.com/jerryjliu/llama_index/pull/1181
-
-        if query.filters is None:
-            return Filter(must=must_conditions)
-
-        for subfilter in query.filters.filters:
+    def _build_subfilter(self, filters: MetadataFilters) -> Filter:
+        conditions = []
+        for subfilter in filters.filters:
             # only for exact match
-            if not subfilter.operator or subfilter.operator == "==":
+            if isinstance(subfilter, MetadataFilters) and len(subfilter.filters) > 0:
+                conditions.append(self._build_subfilter(subfilter))
+            elif not subfilter.operator or subfilter.operator == FilterOperator.EQ:
                 if isinstance(subfilter.value, float):
-                    must_conditions.append(
+                    conditions.append(
                         FieldCondition(
                             key=subfilter.key,
                             range=Range(
                                 gte=subfilter.value,
                                 lte=subfilter.value,
                             ),
                         )
                     )
                 else:
-                    must_conditions.append(
+                    conditions.append(
                         FieldCondition(
                             key=subfilter.key,
                             match=MatchValue(value=subfilter.value),
                         )
                     )
-            elif subfilter.operator == "<":
-                must_conditions.append(
+            elif subfilter.operator == FilterOperator.LT:
+                conditions.append(
                     FieldCondition(
                         key=subfilter.key,
                         range=Range(lt=subfilter.value),
                     )
                 )
-            elif subfilter.operator == ">":
-                must_conditions.append(
+            elif subfilter.operator == FilterOperator.GT:
+                conditions.append(
                     FieldCondition(
                         key=subfilter.key,
                         range=Range(gt=subfilter.value),
                     )
                 )
-            elif subfilter.operator == ">=":
-                must_conditions.append(
+            elif subfilter.operator == FilterOperator.GTE:
+                conditions.append(
                     FieldCondition(
                         key=subfilter.key,
                         range=Range(gte=subfilter.value),
                     )
                 )
-            elif subfilter.operator == "<=":
-                must_conditions.append(
+            elif subfilter.operator == FilterOperator.LTE:
+                conditions.append(
                     FieldCondition(
                         key=subfilter.key,
                         range=Range(lte=subfilter.value),
                     )
                 )
-            elif subfilter.operator == "text_match":
-                must_conditions.append(
+            elif subfilter.operator == FilterOperator.TEXT_MATCH:
+                conditions.append(
                     FieldCondition(
                         key=subfilter.key,
                         match=MatchText(text=subfilter.value),
                     )
                 )
-            elif subfilter.operator == "!=":
-                must_conditions.append(
+            elif subfilter.operator == FilterOperator.NE:
+                conditions.append(
                     FieldCondition(
                         key=subfilter.key,
                         match=MatchExcept(**{"except": [subfilter.value]}),
                     )
                 )
-            elif subfilter.operator == "in":
+            elif subfilter.operator == FilterOperator.IN:
                 # match any of the values
                 # https://qdrant.tech/documentation/concepts/filtering/#match-any
-                must_conditions.append(
+                if isinstance(subfilter.value, List):
+                    values = [str(val) for val in subfilter.value]
+                else:
+                    values = str(subfilter.value).split(",")
+
+                conditions.append(
                     FieldCondition(
                         key=subfilter.key,
-                        match=MatchAny(any=str(subfilter.value).split(",")),
+                        match=MatchAny(any=values),
                     )
                 )
 
+        filter = Filter()
+        if filters.condition == FilterCondition.AND:
+            filter.must = conditions
+        elif filters.condition == FilterCondition.OR:
+            filter.should = conditions
+        return filter
+
+    def _build_query_filter(self, query: VectorStoreQuery) -> Optional[Any]:
+        if not query.doc_ids and not query.query_str:
+            return None
+
+        must_conditions = []
+
+        if query.doc_ids:
+            must_conditions.append(
+                FieldCondition(
+                    key="doc_id",
+                    match=MatchAny(any=query.doc_ids),
+                )
+            )
+
+        # Point id is a “service” id, it is not stored in payload. There is ‘HasId’ condition to filter by point id
+        # https://qdrant.tech/documentation/concepts/filtering/#has-id
+        if query.node_ids:
+            must_conditions.append(
+                HasIdCondition(has_id=query.node_ids),
+            )
+
+        # Qdrant does not use the query.query_str property for the filtering. Full-text
+        # filtering cannot handle longer queries and can effectively filter our all the
+        # nodes. See: https://github.com/jerryjliu/llama_index/pull/1181
+
+        if query.filters and query.filters.filters:
+            must_conditions.append(self._build_subfilter(query.filters))
+
         return Filter(must=must_conditions)
 
     def use_old_sparse_encoder(self, collection_name: str) -> bool:
         collection_exists = self._collection_exists(collection_name)
         if collection_exists:
             cur_collection = self.client.get_collection(collection_name)
             return SPARSE_VECTOR_NAME_OLD in (
```

### Comparing `llama_index_vector_stores_qdrant-0.2.7/llama_index/vector_stores/qdrant/utils.py` & `llama_index_vector_stores_qdrant-0.2.8/llama_index/vector_stores/qdrant/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_vector_stores_qdrant-0.2.7/pyproject.toml` & `llama_index_vector_stores_qdrant-0.2.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index vector_stores qdrant integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-vector-stores-qdrant"
 readme = "README.md"
-version = "0.2.7"
+version = "0.2.8"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 llama-index-core = "^0.10.1"
 qdrant-client = "^1.7.1"
 grpcio = "^1.60.0"
```

### Comparing `llama_index_vector_stores_qdrant-0.2.7/PKG-INFO` & `llama_index_vector_stores_qdrant-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-vector-stores-qdrant
-Version: 0.2.7
+Version: 0.2.8
 Summary: llama-index vector_stores qdrant integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

