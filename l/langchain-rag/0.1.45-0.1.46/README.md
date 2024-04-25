# Comparing `tmp/langchain_rag-0.1.45.tar.gz` & `tmp/langchain_rag-0.1.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_rag-0.1.45.tar", max compression
+gzip compressed data, was "langchain_rag-0.1.46.tar", max compression
```

## Comparing `langchain_rag-0.1.45.tar` & `langchain_rag-0.1.46.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11357 2023-10-19 05:47:38.233379 langchain_rag-0.1.45/LICENSE.txt
--rw-r--r--   0        0        0     2155 2024-02-07 08:38:30.870089 langchain_rag-0.1.45/README.md
--rw-r--r--   0        0        0        0 2023-10-23 07:07:51.650962 langchain_rag-0.1.45/langchain_rag/__init__.py
--rw-r--r--   0        0        0      698 2024-04-23 11:15:14.817186 langchain_rag-0.1.45/langchain_rag/document_transformers/__init__.py
--rw-r--r--   0        0        0     1096 2024-01-29 11:57:32.041286 langchain_rag-0.1.45/langchain_rag/document_transformers/copy_transformer.py
--rw-r--r--   0        0        0     2859 2024-04-23 11:15:14.817186 langchain_rag-0.1.45/langchain_rag/document_transformers/document_transform_pipeline.py
--rw-r--r--   0        0        0     6134 2024-04-23 11:15:14.817186 langchain_rag-0.1.45/langchain_rag/document_transformers/document_transformers.py
--rw-r--r--   0        0        0     3978 2024-01-29 11:07:27.844752 langchain_rag-0.1.45/langchain_rag/document_transformers/generate_questions.py
--rw-r--r--   0        0        0     9254 2024-04-23 11:17:36.261006 langchain_rag-0.1.45/langchain_rag/document_transformers/runnable_document_transformer.py
--rw-r--r--   0        0        0     4740 2024-04-23 11:15:14.821186 langchain_rag-0.1.45/langchain_rag/document_transformers/summarize_and_questions_transformer.py
--rw-r--r--   0        0        0     3257 2024-04-23 11:15:14.821186 langchain_rag-0.1.45/langchain_rag/document_transformers/summarize_transformer.py
--rw-r--r--   0        0        0       89 2024-01-24 09:40:10.848052 langchain_rag-0.1.45/langchain_rag/indexes/__init__.py
--rw-r--r--   0        0        0     3637 2024-01-24 07:30:49.261495 langchain_rag-0.1.45/langchain_rag/indexes/memory_recordmanager.py
--rw-r--r--   0        0        0        0 2024-04-23 11:15:14.821186 langchain_rag-0.1.45/langchain_rag/patch_langchain/__init__.py
--rw-r--r--   0        0        0       81 2024-04-23 11:15:14.821186 langchain_rag-0.1.45/langchain_rag/patch_langchain/storage/__init__.py
--rw-r--r--   0        0        0     4047 2024-04-23 11:15:14.821186 langchain_rag-0.1.45/langchain_rag/patch_langchain/storage/encoder_backed.py
--rw-r--r--   0        0        0        0 2024-04-23 11:15:14.821186 langchain_rag-0.1.45/langchain_rag/patch_langchain_community/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 11:15:14.821186 langchain_rag-0.1.45/langchain_rag/patch_langchain_community/indexes/__init__.py
--rw-r--r--   0        0        0    21023 2024-04-23 11:15:14.821186 langchain_rag-0.1.45/langchain_rag/patch_langchain_community/indexes/_sql_record_manager.py
--rw-r--r--   0        0        0       59 2023-11-02 16:16:50.944534 langchain_rag-0.1.45/langchain_rag/storage/__init__.py
--rw-r--r--   0        0        0     8277 2024-04-23 11:15:14.821186 langchain_rag-0.1.45/langchain_rag/storage/sql_docstore.py
--rw-r--r--   0        0        0      148 2023-11-02 16:16:50.948534 langchain_rag-0.1.45/langchain_rag/vectorstores/__init__.py
--rw-r--r--   0        0        0    32450 2024-04-23 11:15:14.821186 langchain_rag-0.1.45/langchain_rag/vectorstores/rag_vectorstore.py
--rw-r--r--   0        0        0     6658 2024-01-24 07:30:49.265495 langchain_rag-0.1.45/langchain_rag/vectorstores/wrapper_vectorstore.py
--rw-r--r--   0        0        0     3816 2024-04-23 11:15:14.825186 langchain_rag-0.1.45/pyproject.toml
--rw-r--r--   0        0        0     2940 1970-01-01 00:00:00.000000 langchain_rag-0.1.45/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-10-19 05:47:38.233379 langchain_rag-0.1.46/LICENSE.txt
+-rw-r--r--   0        0        0     2155 2024-02-07 08:38:30.870089 langchain_rag-0.1.46/README.md
+-rw-r--r--   0        0        0        0 2023-10-23 07:07:51.650962 langchain_rag-0.1.46/langchain_rag/__init__.py
+-rw-r--r--   0        0        0      698 2024-04-23 11:15:14.817186 langchain_rag-0.1.46/langchain_rag/document_transformers/__init__.py
+-rw-r--r--   0        0        0     1096 2024-01-29 11:57:32.041286 langchain_rag-0.1.46/langchain_rag/document_transformers/copy_transformer.py
+-rw-r--r--   0        0        0     2859 2024-04-23 11:15:14.817186 langchain_rag-0.1.46/langchain_rag/document_transformers/document_transform_pipeline.py
+-rw-r--r--   0        0        0     6134 2024-04-23 11:15:14.817186 langchain_rag-0.1.46/langchain_rag/document_transformers/document_transformers.py
+-rw-r--r--   0        0        0     3978 2024-01-29 11:07:27.844752 langchain_rag-0.1.46/langchain_rag/document_transformers/generate_questions.py
+-rw-r--r--   0        0        0     9254 2024-04-23 11:17:36.261006 langchain_rag-0.1.46/langchain_rag/document_transformers/runnable_document_transformer.py
+-rw-r--r--   0        0        0     4740 2024-04-23 11:15:14.821186 langchain_rag-0.1.46/langchain_rag/document_transformers/summarize_and_questions_transformer.py
+-rw-r--r--   0        0        0     3257 2024-04-23 11:15:14.821186 langchain_rag-0.1.46/langchain_rag/document_transformers/summarize_transformer.py
+-rw-r--r--   0        0        0       89 2024-01-24 09:40:10.848052 langchain_rag-0.1.46/langchain_rag/indexes/__init__.py
+-rw-r--r--   0        0        0     3637 2024-01-24 07:30:49.261495 langchain_rag-0.1.46/langchain_rag/indexes/memory_recordmanager.py
+-rw-r--r--   0        0        0        0 2024-04-23 11:15:14.821186 langchain_rag-0.1.46/langchain_rag/patch_langchain/__init__.py
+-rw-r--r--   0        0        0       81 2024-04-23 11:15:14.821186 langchain_rag-0.1.46/langchain_rag/patch_langchain/storage/__init__.py
+-rw-r--r--   0        0        0     4047 2024-04-23 11:15:14.821186 langchain_rag-0.1.46/langchain_rag/patch_langchain/storage/encoder_backed.py
+-rw-r--r--   0        0        0        0 2024-04-23 11:15:14.821186 langchain_rag-0.1.46/langchain_rag/patch_langchain_community/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 11:15:14.821186 langchain_rag-0.1.46/langchain_rag/patch_langchain_community/indexes/__init__.py
+-rw-r--r--   0        0        0    21023 2024-04-23 11:15:14.821186 langchain_rag-0.1.46/langchain_rag/patch_langchain_community/indexes/_sql_record_manager.py
+-rw-r--r--   0        0        0       59 2023-11-02 16:16:50.944534 langchain_rag-0.1.46/langchain_rag/storage/__init__.py
+-rw-r--r--   0        0        0     8277 2024-04-23 11:15:14.821186 langchain_rag-0.1.46/langchain_rag/storage/sql_docstore.py
+-rw-r--r--   0        0        0      148 2023-11-02 16:16:50.948534 langchain_rag-0.1.46/langchain_rag/vectorstores/__init__.py
+-rw-r--r--   0        0        0    35370 2024-04-25 08:50:07.798706 langchain_rag-0.1.46/langchain_rag/vectorstores/rag_vectorstore.py
+-rw-r--r--   0        0        0     6658 2024-01-24 07:30:49.265495 langchain_rag-0.1.46/langchain_rag/vectorstores/wrapper_vectorstore.py
+-rw-r--r--   0        0        0     3816 2024-04-23 11:15:14.825186 langchain_rag-0.1.46/pyproject.toml
+-rw-r--r--   0        0        0     2940 1970-01-01 00:00:00.000000 langchain_rag-0.1.46/PKG-INFO
```

### Comparing `langchain_rag-0.1.45/LICENSE.txt` & `langchain_rag-0.1.46/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.45/README.md` & `langchain_rag-0.1.46/README.md`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.45/langchain_rag/document_transformers/__init__.py` & `langchain_rag-0.1.46/langchain_rag/document_transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.45/langchain_rag/document_transformers/copy_transformer.py` & `langchain_rag-0.1.46/langchain_rag/document_transformers/copy_transformer.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.45/langchain_rag/document_transformers/document_transform_pipeline.py` & `langchain_rag-0.1.46/langchain_rag/document_transformers/document_transform_pipeline.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.45/langchain_rag/document_transformers/document_transformers.py` & `langchain_rag-0.1.46/langchain_rag/document_transformers/document_transformers.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.45/langchain_rag/document_transformers/generate_questions.py` & `langchain_rag-0.1.46/langchain_rag/document_transformers/generate_questions.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.45/langchain_rag/document_transformers/runnable_document_transformer.py` & `langchain_rag-0.1.46/langchain_rag/document_transformers/runnable_document_transformer.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.45/langchain_rag/document_transformers/summarize_and_questions_transformer.py` & `langchain_rag-0.1.46/langchain_rag/document_transformers/summarize_and_questions_transformer.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.45/langchain_rag/document_transformers/summarize_transformer.py` & `langchain_rag-0.1.46/langchain_rag/document_transformers/summarize_transformer.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.45/langchain_rag/indexes/memory_recordmanager.py` & `langchain_rag-0.1.46/langchain_rag/indexes/memory_recordmanager.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.45/langchain_rag/patch_langchain/storage/encoder_backed.py` & `langchain_rag-0.1.46/langchain_rag/patch_langchain/storage/encoder_backed.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.45/langchain_rag/patch_langchain_community/indexes/_sql_record_manager.py` & `langchain_rag-0.1.46/langchain_rag/patch_langchain_community/indexes/_sql_record_manager.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.45/langchain_rag/storage/sql_docstore.py` & `langchain_rag-0.1.46/langchain_rag/storage/sql_docstore.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.45/langchain_rag/vectorstores/rag_vectorstore.py` & `langchain_rag-0.1.46/langchain_rag/vectorstores/rag_vectorstore.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import asyncio
 import concurrent
 import hashlib
+import logging
 import uuid
+from copy import copy
 from typing import (
     Any,
     Callable,
     Dict,
     List,
     Optional,
     Sequence,
@@ -30,14 +32,16 @@
     AsyncEngine,
     create_async_engine,
 )
 from sqlalchemy.orm import scoped_session, sessionmaker
 
 from .wrapper_vectorstore import WrapperVectorStore
 
+logger = logging.getLogger(__name__)
+
 # %%
 VST = TypeVar("VST", bound="VectorStore")
 
 
 def _get_source_id_assigner(
     source_id_key: Union[str, Callable[[Document], str], None],
 ) -> Callable[[Document], Union[str, None]]:
@@ -176,25 +180,58 @@
         map_ids = {doc.metadata[key]: i for doc, i in zip(docs, ids) if doc}
         return sorted(
             [(d, scores[map_ids[d.metadata[key]]]) for d in docs if d is not None],
             key=lambda x: x[1],
             reverse=True,
         )
 
+    async def _aupdate_score_of_chunk(
+        self, sub_chunks_and_score: List[Tuple[Document, float]]
+    ) -> List[Tuple[Document, float]]:
+        if not self.chunk_transformer:
+            return sub_chunks_and_score
+        ids = []
+        scores: Dict[str, float] = {}
+        key = self.chunk_id_key
+        for d, s in sub_chunks_and_score:
+            if d.metadata[key] not in ids:
+                id = d.metadata[key]
+                ids.append(id)
+                chunk_s = scores.get(id, 1.0)
+                scores[id] = min(chunk_s, s)
+        docs = cast(Sequence[Document], await self.docstore.amget(ids))
+        map_ids = {doc.metadata[key]: i for doc, i in zip(docs, ids) if doc}
+        return sorted(
+            [(d, scores[map_ids[d.metadata[key]]]) for d in docs if d is not None],
+            key=lambda x: x[1],
+            reverse=True,
+        )
+
     def _get_trunk_from_sub_docs_and_score(
         self, sub_docs_and_score: List[Tuple[Document, float]], k: int, **kwargs: Any
     ) -> List[Tuple[Document, float]]:
         if self.chunk_transformer:
             result = self._update_score_of_chunk(sub_docs_and_score)
         else:
             result = sub_docs_and_score
         if self.search_kwargs.get("k", k) < k:
             raise ValueError("The search_kwargs['k'] must be >= 'k'")
         return result[:k]
 
+    async def _aget_trunk_from_sub_docs_and_score(
+        self, sub_docs_and_score: List[Tuple[Document, float]], k: int, **kwargs: Any
+    ) -> List[Tuple[Document, float]]:
+        if self.chunk_transformer:
+            result = await self._aupdate_score_of_chunk(sub_docs_and_score)
+        else:
+            result = sub_docs_and_score
+        if self.search_kwargs.get("k", k) < k:
+            raise ValueError("The search_kwargs['k'] must be >= 'k'")
+        return result[:k]
+
     def as_retriever(
         self, search_type: str = "similarity", search_kwargs: dict = {}, **kwargs: Any
     ) -> VectorStoreRetriever:
         if not self.chunk_transformer:
             return self.vectorstore.as_retriever(
                 search_type=search_type, search_kwargs=search_kwargs, *kwargs
             )
@@ -619,15 +656,15 @@
         trunk_k: Optional[int] = self.search_kwargs.get("k")
         if not trunk_k:
             _search_kwargs["k"] = k * self.coef_trunk_k
 
         subdocs_and_score = await self.vectorstore.asimilarity_search_with_score(
             query=query, **_search_kwargs
         )
-        return self._get_trunk_from_sub_docs_and_score(subdocs_and_score, k=k)
+        return await self._aget_trunk_from_sub_docs_and_score(subdocs_and_score, k=k)
 
     def similarity_search_with_relevance_scores(
         self,
         query: str,
         k: int = 4,
         **kwargs: Any,
     ) -> List[Tuple[Document, float]]:
@@ -642,15 +679,15 @@
     ) -> List[Tuple[Document, float]]:
         _search_kwargs = {**kwargs, **self.search_kwargs}
         subdocs_and_score = (
             await self.vectorstore.asimilarity_search_with_relevance_scores(
                 query=query, **_search_kwargs
             )
         )
-        return self._update_score_of_chunk(subdocs_and_score)[:k]
+        return (await self._aupdate_score_of_chunk(subdocs_and_score))[:k]
 
     def similarity_search_by_vector(
         self, embedding: List[float], k: int = 4, **kwargs: Any
     ) -> List[Document]:
         subdocs = self.vectorstore.similarity_search_by_vector(
             embedding=embedding, k=k, **kwargs
         )
@@ -835,7 +872,40 @@
             rag_vectorstore,
             {
                 "record_manager": record_manager,
                 "vector_store": vectorstore,
                 "source_id_key": kwargs.get("source_id_key", "source"),
             },
         )
+
+    @staticmethod
+    def copy_with_session_maker(
+        session_maker: Any,
+        rag_vectorstore: "RAGVectorStore",
+        index_kwargs: Dict[str, Any],
+    ) -> Tuple["RAGVectorStore", Dict[str, Any]]:
+        """Duplicate the RAGVectorStore and index_kwargs with a new session_maker."""
+        assert isinstance(rag_vectorstore, RAGVectorStore)
+        new_rag_vectorstore = copy(rag_vectorstore)
+        new_rag_vectorstore.docstore = copy(rag_vectorstore.docstore)
+        new_rag_vectorstore.vectorstore = copy(rag_vectorstore.vectorstore)
+
+        if hasattr(new_rag_vectorstore.docstore, "session_factory"):
+            new_rag_vectorstore.docstore.session_factory = session_maker
+
+        if hasattr(new_rag_vectorstore.vectorstore, "session_factory"):
+            new_rag_vectorstore.vectorstore.session_factory = session_maker
+        elif hasattr(new_rag_vectorstore.vectorstore, "session_maker"):
+            new_rag_vectorstore.vectorstore.session_maker = session_maker
+        else:
+            logger.warning(
+                "The vectorstore has no session_factory or session_maker attribute"
+            )
+
+        new_record_manager = copy(index_kwargs["record_manager"])
+        new_record_manager.session_factory = session_maker
+
+        return new_rag_vectorstore, {
+            "record_manager": new_record_manager,
+            "source_id_key": index_kwargs["source_id_key"],
+            "vector_store": new_rag_vectorstore,
+        }
```

### Comparing `langchain_rag-0.1.45/langchain_rag/vectorstores/wrapper_vectorstore.py` & `langchain_rag-0.1.46/langchain_rag/vectorstores/wrapper_vectorstore.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.45/pyproject.toml` & `langchain_rag-0.1.46/pyproject.toml`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.45/PKG-INFO` & `langchain_rag-0.1.46/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-rag
-Version: 0.1.45
+Version: 0.1.46
 Summary: This is a temporary project while I wait for my langchain [pull-request](https://github.com/langchain-ai/langchain/pull/7278) to be validated.
 Home-page: https://www.github.com/pprados/langchain-rag
 License: Apache 2.0
 Author: Philippe PRADOS
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

