# Comparing `tmp/flexible_semantic_kernel-1.0.2.dev0.tar.gz` & `tmp/flexible_semantic_kernel-1.0.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flexible_semantic_kernel-1.0.2.dev0.tar", last modified: Wed Apr 24 09:04:43 2024, max compression
+gzip compressed data, was "flexible_semantic_kernel-1.0.3.dev0.tar", last modified: Thu Apr 25 09:09:57 2024, max compression
```

## Comparing `flexible_semantic_kernel-1.0.2.dev0.tar` & `flexible_semantic_kernel-1.0.3.dev0.tar`

### file list

```diff
@@ -1,445 +1,445 @@
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.789598 flexible_semantic_kernel-1.0.2.dev0/
--rw-r--r--   0 caoyitong   (502) staff       (20)     2050 2024-03-29 07:13:13.000000 flexible_semantic_kernel-1.0.2.dev0/.gitignore
--rw-r--r--   0 caoyitong   (502) staff       (20)     1547 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.2.dev0/Makefile
--rw-r--r--   0 caoyitong   (502) staff       (20)     1641 2024-04-24 09:04:43.789275 flexible_semantic_kernel-1.0.2.dev0/PKG-INFO
--rw-r--r--   0 caoyitong   (502) staff       (20)      127 2024-04-24 06:46:33.000000 flexible_semantic_kernel-1.0.2.dev0/README.md
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.696514 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/
--rw-r--r--   0 caoyitong   (502) staff       (20)     2150 2024-04-19 09:02:20.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/__init__.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.697934 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/
--rw-r--r--   0 caoyitong   (502) staff       (20)       48 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/__init__.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.699647 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/
--rw-r--r--   0 caoyitong   (502) staff       (20)      617 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/__init__.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     1735 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/ai_exception.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     3442 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/ai_request_settings.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     1242 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/ai_service_client_base.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     2021 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/chat_completion_client_base.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.699954 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/embeddings/
--rw-r--r--   0 caoyitong   (502) staff       (20)      321 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.700590 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/google_palm/
--rw-r--r--   0 caoyitong   (502) staff       (20)      763 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/google_palm/__init__.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     1645 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/google_palm/gp_request_settings.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.701533 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/google_palm/services/
--rw-r--r--   0 caoyitong   (502) staff       (20)     8338 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     3243 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/google_palm/services/gp_text_completion.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     2365 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.702131 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/hugging_face/
--rw-r--r--   0 caoyitong   (502) staff       (20)      535 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/hugging_face/__init__.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     1354 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/hugging_face/hf_request_settings.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.702740 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/hugging_face/services/
--rw-r--r--   0 caoyitong   (502) staff       (20)     6001 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     2305 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.703328 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/ollama/
--rw-r--r--   0 caoyitong   (502) staff       (20)        0 2024-01-25 07:19:10.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/ollama/__init__.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      710 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/ollama/ollama_request_settings.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.704240 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/ollama/services/
--rw-r--r--   0 caoyitong   (502) staff       (20)     5419 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     3466 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     1785 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      338 2024-01-25 07:19:10.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/ollama/utils.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.705024 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/
--rw-r--r--   0 caoyitong   (502) staff       (20)     1405 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/__init__.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      246 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/const.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.705654 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/exceptions/
--rw-r--r--   0 caoyitong   (502) staff       (20)       48 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/exceptions/__init__.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     3523 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.666651 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/models/
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.706521 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/models/chat/
--rw-r--r--   0 caoyitong   (502) staff       (20)     3360 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/models/chat/azure_chat_with_data_response.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     1246 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/models/chat/function_call.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      463 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/models/chat/open_ai_chat_message.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.707101 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/request_settings/
--rw-r--r--   0 caoyitong   (502) staff       (20)     2858 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/request_settings/azure_chat_request_settings.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     3757 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/request_settings/open_ai_request_settings.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.707374 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/semantic_functions/
--rw-r--r--   0 caoyitong   (502) staff       (20)     4239 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/semantic_functions/open_ai_chat_prompt_template.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.711168 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/
--rw-r--r--   0 caoyitong   (502) staff       (20)    16579 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     5657 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     8813 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     5207 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     8467 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     3895 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     4603 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/open_ai_handler.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      230 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/open_ai_model_types.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     4653 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     4551 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     3070 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     1921 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     9797 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/utils.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     1707 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/text_completion_client_base.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.711440 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/
--rw-r--r--   0 caoyitong   (502) staff       (20)       48 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/__init__.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.712274 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/azure_cognitive_search/
--rw-r--r--   0 caoyitong   (502) staff       (20)      251 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/azure_cognitive_search/__init__.py
--rw-r--r--   0 caoyitong   (502) staff       (20)    15436 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     8187 2024-04-19 07:51:57.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/azure_cognitive_search/utils.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.713832 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/azure_cosmosdb/
--rw-r--r--   0 caoyitong   (502) staff       (20)      222 2024-04-19 09:02:20.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/azure_cosmosdb/__init__.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     9514 2024-04-19 09:02:20.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     2239 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_store_api.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      403 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/azure_cosmosdb/cosmosdb_utils.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     7397 2024-04-19 09:02:20.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/azure_cosmosdb/mongo_vcore_store_api.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.714809 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/chroma/
--rw-r--r--   0 caoyitong   (502) staff       (20)      191 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/chroma/__init__.py
--rw-r--r--   0 caoyitong   (502) staff       (20)    14974 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/chroma/chroma_memory_store.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     4612 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/chroma/utils.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.715417 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/milvus/
--rw-r--r--   0 caoyitong   (502) staff       (20)      142 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/milvus/__init__.py
--rw-r--r--   0 caoyitong   (502) staff       (20)    16441 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/milvus/milvus_memory_store.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.716807 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/mongodb_atlas/
--rw-r--r--   0 caoyitong   (502) staff       (20)     1458 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/mongodb_atlas/README.md
--rw-r--r--   0 caoyitong   (502) staff       (20)      168 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/mongodb_atlas/__init__.py
--rw-r--r--   0 caoyitong   (502) staff       (20)    12682 2024-04-19 09:02:20.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     2311 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/mongodb_atlas/utils.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.717700 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/pinecone/
--rw-r--r--   0 caoyitong   (502) staff       (20)      199 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/pinecone/__init__.py
--rw-r--r--   0 caoyitong   (502) staff       (20)    14643 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     1163 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/pinecone/utils.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.718282 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/postgres/
--rw-r--r--   0 caoyitong   (502) staff       (20)      199 2024-04-19 09:02:20.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/postgres/__init__.py
--rw-r--r--   0 caoyitong   (502) staff       (20)    20169 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/postgres/postgres_memory_store.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.719088 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/qdrant/
--rw-r--r--   0 caoyitong   (502) staff       (20)      191 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/qdrant/__init__.py
--rw-r--r--   0 caoyitong   (502) staff       (20)    11743 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.720131 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/redis/
--rw-r--r--   0 caoyitong   (502) staff       (20)     1294 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/redis/README.md
--rw-r--r--   0 caoyitong   (502) staff       (20)      187 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/redis/__init__.py
--rw-r--r--   0 caoyitong   (502) staff       (20)    15491 2024-04-19 09:02:20.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/redis/redis_memory_store.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     3686 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/redis/utils.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.720690 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/usearch/
--rw-r--r--   0 caoyitong   (502) staff       (20)      195 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/usearch/__init__.py
--rw-r--r--   0 caoyitong   (502) staff       (20)    23333 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/usearch/usearch_memory_store.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.721380 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/weaviate/
--rw-r--r--   0 caoyitong   (502) staff       (20)      197 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/weaviate/__init__.py
--rw-r--r--   0 caoyitong   (502) staff       (20)    11033 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.721953 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/openapi/
--rw-r--r--   0 caoyitong   (502) staff       (20)      137 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/openapi/__init__.py
--rw-r--r--   0 caoyitong   (502) staff       (20)    11180 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/openapi/sk_openapi.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.723205 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/search_engine/
--rw-r--r--   0 caoyitong   (502) staff       (20)      283 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/search_engine/__init__.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     2838 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/search_engine/bing_connector.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      254 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/search_engine/connector.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     3189 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/search_engine/google_connector.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      484 2024-04-19 07:56:23.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/telemetry.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.725919 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/core_plugins/
--rw-r--r--   0 caoyitong   (502) staff       (20)      908 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/core_plugins/__init__.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     2593 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/core_plugins/conversation_summary_plugin.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     2038 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/core_plugins/file_io_plugin.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     3833 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/core_plugins/http_plugin.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     3348 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/core_plugins/math_plugin.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     5327 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/core_plugins/text_memory_plugin.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     2551 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/core_plugins/text_plugin.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     7984 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/core_plugins/time_plugin.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      775 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/core_plugins/wait_plugin.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     2010 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/core_plugins/web_search_engine_plugin.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.727051 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/events/
--rw-r--r--   0 caoyitong   (502) staff       (20)      334 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/events/__init__.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      452 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/events/function_invoked_event_args.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      443 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/events/function_invoking_event_args.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      892 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/events/sk_events_args.py
--rw-r--r--   0 caoyitong   (502) staff       (20)    35066 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/kernel.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     1728 2024-01-25 07:19:10.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/kernel_exception.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.729116 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/memory/
--rw-r--r--   0 caoyitong   (502) staff       (20)      169 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/memory/__init__.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     2553 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/memory/memory_query_result.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     4267 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/memory/memory_record.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     7239 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/memory/memory_store_base.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     1670 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/memory/null_memory.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     6368 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/memory/semantic_text_memory.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     3586 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/memory/semantic_text_memory_base.py
--rw-r--r--   0 caoyitong   (502) staff       (20)    11877 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/memory/volatile_memory_store.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.668819 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/models/
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.729418 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/models/chat/
--rw-r--r--   0 caoyitong   (502) staff       (20)     1543 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/models/chat/chat_message.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.731527 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/orchestration/
--rw-r--r--   0 caoyitong   (502) staff       (20)     4774 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/orchestration/context_variables.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     6058 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/orchestration/delegate_handlers.py
--rw-r--r--   0 caoyitong   (502) staff       (20)    12075 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/orchestration/delegate_inference.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      781 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/orchestration/delegate_types.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     7855 2024-04-23 04:41:13.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/orchestration/sk_context.py
--rw-r--r--   0 caoyitong   (502) staff       (20)    22539 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/orchestration/sk_function.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     5933 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/orchestration/sk_function_base.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.732829 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/
--rw-r--r--   0 caoyitong   (502) staff       (20)      655 2024-04-19 06:49:52.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/__init__.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.733953 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/action_planner/
--rw-r--r--   0 caoyitong   (502) staff       (20)      135 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/action_planner/__init__.py
--rw-r--r--   0 caoyitong   (502) staff       (20)    11525 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/action_planner/action_planner.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      363 2024-03-29 07:04:59.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/action_planner/config.json
--rw-r--r--   0 caoyitong   (502) staff       (20)     3087 2024-03-29 07:04:15.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/action_planner/skprompt.txt
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.735123 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/basic_planner/
--rw-r--r--   0 caoyitong   (502) staff       (20)      131 2024-04-19 06:51:32.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/basic_planner/__init__.py
--rw-r--r--   0 caoyitong   (502) staff       (20)    10875 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/basic_planner/basic_planner.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      363 2024-03-29 07:05:10.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/basic_planner/config.json
--rw-r--r--   0 caoyitong   (502) staff       (20)     6310 2024-03-29 03:35:11.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/basic_planner/skprompt.txt
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.736346 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/multimodal_planner/
--rw-r--r--   0 caoyitong   (502) staff       (20)      376 2024-04-11 02:49:35.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/multimodal_planner/__init__.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      363 2024-04-23 06:38:36.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/multimodal_planner/config.json
--rw-r--r--   0 caoyitong   (502) staff       (20)    10981 2024-04-23 07:02:33.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/multimodal_planner/multimodal_planner.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     7907 2024-04-19 02:26:50.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/multimodal_planner/skprompt.txt
--rw-r--r--   0 caoyitong   (502) staff       (20)    17750 2024-04-24 03:07:39.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/plan.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     1632 2024-03-29 07:03:53.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/planner_config.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     1198 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/planning_exception.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.737874 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/sequential_planner/
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.669595 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/sequential_planner/Plugins/
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.738469 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/sequential_planner/Plugins/SequentialPlanning/
--rw-r--r--   0 caoyitong   (502) staff       (20)      687 2024-01-25 07:19:10.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/sequential_planner/Plugins/SequentialPlanning/config.json
--rw-r--r--   0 caoyitong   (502) staff       (20)     3019 2024-01-25 07:19:10.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/sequential_planner/Plugins/SequentialPlanning/skprompt.txt
--rw-r--r--   0 caoyitong   (502) staff       (20)      151 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/sequential_planner/__init__.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     5764 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/sequential_planner/sequential_planner.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     1153 2024-01-25 07:19:10.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/sequential_planner/sequential_planner_config.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     7958 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/sequential_planner/sequential_planner_extensions.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     5403 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/sequential_planner/sequential_planner_parser.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.739515 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/stepwise_planner/
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.669857 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/stepwise_planner/Plugins/
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.739953 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/stepwise_planner/Plugins/StepwiseStep/
--rw-r--r--   0 caoyitong   (502) staff       (20)      860 2024-01-25 07:19:10.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/stepwise_planner/Plugins/StepwiseStep/config.json
--rw-r--r--   0 caoyitong   (502) staff       (20)     2822 2024-01-25 07:19:10.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/stepwise_planner/Plugins/StepwiseStep/skprompt.txt
--rw-r--r--   0 caoyitong   (502) staff       (20)      134 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/stepwise_planner/__init__.py
--rw-r--r--   0 caoyitong   (502) staff       (20)    16147 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/stepwise_planner/stepwise_planner.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      982 2024-01-25 07:19:10.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/stepwise_planner/stepwise_planner_config.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      371 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/stepwise_planner/system_step.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.742711 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/plugin_definition/
--rw-r--r--   0 caoyitong   (502) staff       (20)      342 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/plugin_definition/__init__.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      119 2024-01-25 07:19:10.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/plugin_definition/constants.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      990 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/plugin_definition/function_view.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     2243 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/plugin_definition/functions_view.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      613 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/plugin_definition/parameter_view.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     4477 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/plugin_definition/plugin_collection.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      892 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/plugin_definition/plugin_collection_base.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     4755 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/plugin_definition/read_only_plugin_collection.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     1362 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/plugin_definition/read_only_plugin_collection_base.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     1071 2024-01-25 07:19:10.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/plugin_definition/sk_function_context_parameter_decorator.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      840 2024-01-25 07:19:10.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/plugin_definition/sk_function_decorator.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.743218 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/reliability/
--rw-r--r--   0 caoyitong   (502) staff       (20)     1160 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/reliability/pass_through_without_retry.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      836 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/reliability/retry_mechanism_base.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.744485 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/semantic_functions/
--rw-r--r--   0 caoyitong   (502) staff       (20)     5642 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/semantic_functions/chat_prompt_template.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     2665 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/semantic_functions/prompt_template.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      600 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/semantic_functions/prompt_template_base.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     3299 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/semantic_functions/prompt_template_config.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      698 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/semantic_functions/semantic_function_config.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      602 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/sk_pydantic.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.745560 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/template_engine/
--rw-r--r--   0 caoyitong   (502) staff       (20)     1115 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/template_engine/README.md
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.747624 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/template_engine/blocks/
--rw-r--r--   0 caoyitong   (502) staff       (20)      827 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/template_engine/blocks/block.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      228 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/template_engine/blocks/block_types.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     4711 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/template_engine/blocks/code_block.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     3214 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/template_engine/blocks/function_id_block.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      276 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/template_engine/blocks/symbols.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     1636 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/template_engine/blocks/text_block.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     2369 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/template_engine/blocks/val_block.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     2754 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/template_engine/blocks/var_block.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     6607 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/template_engine/code_tokenizer.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     6243 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/template_engine/prompt_template_engine.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.748457 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/template_engine/protocols/
--rw-r--r--   0 caoyitong   (502) staff       (20)      541 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/template_engine/protocols/code_renderer.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     3110 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/template_engine/protocols/prompt_templating_engine.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      605 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/template_engine/protocols/text_renderer.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     7354 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/template_engine/template_tokenizer.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.749253 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/text/
--rw-r--r--   0 caoyitong   (502) staff       (20)      491 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/text/__init__.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      685 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/text/function_extension.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     8474 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/text/text_chunker.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.750292 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/utils/
--rw-r--r--   0 caoyitong   (502) staff       (20)      276 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/utils/logging.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     1161 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/utils/null_logger.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     8264 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/utils/settings.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      221 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/utils/static_property.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     2218 2024-01-25 07:19:10.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/utils/validation.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.788754 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel.egg-info/
--rw-r--r--   0 caoyitong   (502) staff       (20)     1641 2024-04-24 09:04:43.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel.egg-info/PKG-INFO
--rw-r--r--   0 caoyitong   (502) staff       (20)    20173 2024-04-24 09:04:43.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel.egg-info/SOURCES.txt
--rw-r--r--   0 caoyitong   (502) staff       (20)        1 2024-04-24 09:04:43.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel.egg-info/dependency_links.txt
--rw-r--r--   0 caoyitong   (502) staff       (20)      626 2024-04-24 09:04:43.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel.egg-info/requires.txt
--rw-r--r--   0 caoyitong   (502) staff       (20)       25 2024-04-24 09:04:43.000000 flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel.egg-info/top_level.txt
--rw-r--r--   0 caoyitong   (502) staff       (20)        0 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.2.dev0/log.txt
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.754947 flexible_semantic_kernel-1.0.2.dev0/notebooks/
--rw-r--r--   0 caoyitong   (502) staff       (20)      164 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.2.dev0/notebooks/.env.example
--rw-r--r--   0 caoyitong   (502) staff       (20)     3658 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/notebooks/00-getting-started.ipynb
--rw-r--r--   0 caoyitong   (502) staff       (20)     4399 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/notebooks/01-basic-loading-the-kernel.ipynb
--rw-r--r--   0 caoyitong   (502) staff       (20)     5980 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/notebooks/02-running-prompts-from-file.ipynb
--rw-r--r--   0 caoyitong   (502) staff       (20)     9993 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/notebooks/03-semantic-function-inline.ipynb
--rw-r--r--   0 caoyitong   (502) staff       (20)     7306 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/notebooks/04-context-variables-chat.ipynb
--rw-r--r--   0 caoyitong   (502) staff       (20)    17829 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/notebooks/05-using-the-planner.ipynb
--rw-r--r--   0 caoyitong   (502) staff       (20)    85718 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/notebooks/06-memory-and-embeddings.ipynb
--rw-r--r--   0 caoyitong   (502) staff       (20)     6213 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/notebooks/07-hugging-face-for-plugins.ipynb
--rw-r--r--   0 caoyitong   (502) staff       (20)    19082 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/notebooks/08-native-function-inline.ipynb
--rw-r--r--   0 caoyitong   (502) staff       (20)    14004 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/notebooks/09-groundedness-checking.ipynb
--rw-r--r--   0 caoyitong   (502) staff       (20)    12330 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/notebooks/10-multiple-results-per-prompt.ipynb
--rw-r--r--   0 caoyitong   (502) staff       (20)     9589 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/notebooks/11-streaming-completions.ipynb
--rw-r--r--   0 caoyitong   (502) staff       (20)      421 2024-01-25 07:19:10.000000 flexible_semantic_kernel-1.0.2.dev0/notebooks/services.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.755468 flexible_semantic_kernel-1.0.2.dev0/notebooks/third_party/
--rw-r--r--   0 caoyitong   (502) staff       (20)      175 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.2.dev0/notebooks/third_party/.env.example
--rw-r--r--   0 caoyitong   (502) staff       (20)    17395 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/notebooks/third_party/weaviate-persistent-memory.ipynb
--rw-r--r--   0 caoyitong   (502) staff       (20)     1684 2024-04-24 09:04:33.000000 flexible_semantic_kernel-1.0.2.dev0/pyproject.toml
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.755893 flexible_semantic_kernel-1.0.2.dev0/samples/
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.762169 flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/
--rw-r--r--   0 caoyitong   (502) staff       (20)     1339 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/action_planner.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     4252 2024-04-19 09:02:20.000000 flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/azure_chat_gpt_api.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     3533 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/azure_chat_gpt_with_data_api.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     3274 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/azure_chat_gpt_with_data_api_cross_lingual.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     4678 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/azure_chat_gpt_with_data_api_function_calling.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     3622 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/azure_chat_gpt_with_data_api_vector_search.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     3039 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/azure_cognitive_search_memory.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     2226 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/bing_search_plugin.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     1779 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/chat.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     1910 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/chat_gpt_api.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     4140 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/chat_gpt_api_function_calling.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     1683 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/google_palm_chat.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     4949 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/google_palm_chat_with_memory.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     2664 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/google_palm_chat_with_plugin.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     1898 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/google_palm_text_completion.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     3227 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/google_search_plugin.py
--rw-r--r--   0 caoyitong   (502) staff       (20)    10532 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/grounded.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     4079 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/memory.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     4207 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/openai_function_calling.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     6577 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/openai_logit_bias.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.763272 flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/openapi_example/
--rw-r--r--   0 caoyitong   (502) staff       (20)      456 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/openapi_example/README.md
--rw-r--r--   0 caoyitong   (502) staff       (20)     1003 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/openapi_example/openapi.yaml
--rw-r--r--   0 caoyitong   (502) staff       (20)      785 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/openapi_example/openapi_client.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      540 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/openapi_example/openapi_server.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     1163 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/plugins_from_dir.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     5052 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/self-critique_rag.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     1504 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/sequential_planner.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      862 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/setup_logging.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      991 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.2.dev0/samples/utils.py
--rw-r--r--   0 caoyitong   (502) staff       (20)       38 2024-04-24 09:04:43.789656 flexible_semantic_kernel-1.0.2.dev0/setup.cfg
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.763669 flexible_semantic_kernel-1.0.2.dev0/tests/
--rw-r--r--   0 caoyitong   (502) staff       (20)       48 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.2.dev0/tests/__init__.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     3564 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/conftest.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.671751 flexible_semantic_kernel-1.0.2.dev0/tests/integration/
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.766320 flexible_semantic_kernel-1.0.2.dev0/tests/integration/completions/
--rw-r--r--   0 caoyitong   (502) staff       (20)     6407 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/integration/completions/conftest.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     2904 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/integration/completions/test_azure_oai_chat_service.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     5404 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/tests/integration/completions/test_azure_oai_chat_service_extensions.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     2974 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/integration/completions/test_azure_oai_text_service.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     2499 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/tests/integration/completions/test_conversation_summary_plugin.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     1991 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/integration/completions/test_gp_chat_service.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     3845 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/integration/completions/test_gp_text_service.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     5171 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/integration/completions/test_hf_local_text_completions.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     3856 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/tests/integration/completions/test_hf_local_text_summarization.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     3548 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/integration/completions/test_oai_chat_service.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     3644 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/integration/completions/test_oai_text_service.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      608 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.2.dev0/tests/integration/completions/test_utils.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.671477 flexible_semantic_kernel-1.0.2.dev0/tests/integration/connectors/
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.769493 flexible_semantic_kernel-1.0.2.dev0/tests/integration/connectors/memory/
--rw-r--r--   0 caoyitong   (502) staff       (20)     5225 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/integration/connectors/memory/test_azure_cognitive_search.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     5909 2024-04-19 09:02:20.000000 flexible_semantic_kernel-1.0.2.dev0/tests/integration/connectors/memory/test_azure_cosmosdb_memory_store.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     7822 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/integration/connectors/memory/test_chroma.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     8566 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/tests/integration/connectors/memory/test_milvus.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     8917 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/integration/connectors/memory/test_mongodb_atlas.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     9908 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/integration/connectors/memory/test_pinecone.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     8182 2024-04-19 09:02:20.000000 flexible_semantic_kernel-1.0.2.dev0/tests/integration/connectors/memory/test_postgres.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     8014 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/tests/integration/connectors/memory/test_qdrant_memory_store.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     8972 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/integration/connectors/memory/test_redis.py
--rw-r--r--   0 caoyitong   (502) staff       (20)    12860 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/integration/connectors/memory/test_usearch.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     9925 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/integration/connectors/memory/test_weaviate_memory_store.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.771498 flexible_semantic_kernel-1.0.2.dev0/tests/integration/embeddings/
--rw-r--r--   0 caoyitong   (502) staff       (20)     3033 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/integration/embeddings/test_azure_oai_embedding_service.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     1168 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/integration/embeddings/test_gp_embedding_service.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     2190 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/integration/embeddings/test_hf_embedding_service.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     1681 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/integration/embeddings/test_oai_embedding_service.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.772431 flexible_semantic_kernel-1.0.2.dev0/tests/integration/fakes/
--rw-r--r--   0 caoyitong   (502) staff       (20)      888 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/tests/integration/fakes/email_plugin_fake.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      510 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/integration/fakes/fun_plugin_fake.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      513 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/integration/fakes/summarize_plugin_fake.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      901 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/integration/fakes/writer_plugin_fake.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.671913 flexible_semantic_kernel-1.0.2.dev0/tests/integration/planning/
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.772932 flexible_semantic_kernel-1.0.2.dev0/tests/integration/planning/sequential_planner/
--rw-r--r--   0 caoyitong   (502) staff       (20)     2635 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/integration/planning/sequential_planner/test_sequential_plan_parser.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     5127 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/tests/integration/planning/sequential_planner/test_sequential_planner.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.773199 flexible_semantic_kernel-1.0.2.dev0/tests/integration/planning/stepwise_planner/
--rw-r--r--   0 caoyitong   (502) staff       (20)     5835 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/integration/planning/stepwise_planner/test_stepwise_planner.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.773750 flexible_semantic_kernel-1.0.2.dev0/tests/template_engine/
--rw-r--r--   0 caoyitong   (502) staff       (20)     4613 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/template_engine/prompt_template_e2e_tests.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     1571 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.2.dev0/tests/template_engine/tests.txt
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.672228 flexible_semantic_kernel-1.0.2.dev0/tests/test_native_plugins/
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.773996 flexible_semantic_kernel-1.0.2.dev0/tests/test_native_plugins/TestNativePlugin/
--rw-r--r--   0 caoyitong   (502) staff       (20)      582 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/test_native_plugins/TestNativePlugin/native_function.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.672465 flexible_semantic_kernel-1.0.2.dev0/tests/test_plugins/
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.672533 flexible_semantic_kernel-1.0.2.dev0/tests/test_plugins/TestPlugin/
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.774523 flexible_semantic_kernel-1.0.2.dev0/tests/test_plugins/TestPlugin/TestFunction/
--rw-r--r--   0 caoyitong   (502) staff       (20)      284 2024-01-25 07:19:10.000000 flexible_semantic_kernel-1.0.2.dev0/tests/test_plugins/TestPlugin/TestFunction/config.json
--rw-r--r--   0 caoyitong   (502) staff       (20)       31 2024-01-25 07:19:10.000000 flexible_semantic_kernel-1.0.2.dev0/tests/test_plugins/TestPlugin/TestFunction/skprompt.txt
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.775025 flexible_semantic_kernel-1.0.2.dev0/tests/unit/
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.775351 flexible_semantic_kernel-1.0.2.dev0/tests/unit/ai/
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.672891 flexible_semantic_kernel-1.0.2.dev0/tests/unit/ai/google_palm/
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.776128 flexible_semantic_kernel-1.0.2.dev0/tests/unit/ai/google_palm/services/
--rw-r--r--   0 caoyitong   (502) staff       (20)     2546 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/ai/google_palm/services/test_palm_chat_completion.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     2572 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/ai/google_palm/services/test_palm_text_completion.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     1954 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/ai/google_palm/services/test_palm_text_embedding.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.776380 flexible_semantic_kernel-1.0.2.dev0/tests/unit/ai/ollama/
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.776871 flexible_semantic_kernel-1.0.2.dev0/tests/unit/ai/ollama/services/
--rw-r--r--   0 caoyitong   (502) staff       (20)     3409 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/ai/ollama/services/test_ollama_chat_completion.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     1738 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/ai/ollama/services/test_ollama_test_completion.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      830 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/ai/ollama/services/test_ollama_text_embedding.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      578 2024-01-25 07:19:10.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/ai/ollama/utils.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.777114 flexible_semantic_kernel-1.0.2.dev0/tests/unit/ai/open_ai/
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.673310 flexible_semantic_kernel-1.0.2.dev0/tests/unit/ai/open_ai/models/
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.777385 flexible_semantic_kernel-1.0.2.dev0/tests/unit/ai/open_ai/models/chat/
--rw-r--r--   0 caoyitong   (502) staff       (20)     1078 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/ai/open_ai/models/chat/test_function_call.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.778764 flexible_semantic_kernel-1.0.2.dev0/tests/unit/ai/open_ai/services/
--rw-r--r--   0 caoyitong   (502) staff       (20)    18931 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/ai/open_ai/services/test_azure_chat_completion.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     7893 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/ai/open_ai/services/test_azure_text_completion.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     5864 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/ai/open_ai/services/test_azure_text_embedding.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     3851 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/ai/open_ai/services/test_openai_chat_completion.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     3356 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/ai/open_ai/services/test_openai_text_completion.py
--rw-r--r--   0 caoyitong   (502) staff       (20)    10256 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/ai/open_ai/test_openai_request_settings.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      540 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/ai/test_ai_request_settings.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.780030 flexible_semantic_kernel-1.0.2.dev0/tests/unit/core_plugins/
--rw-r--r--   0 caoyitong   (502) staff       (20)     2520 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/core_plugins/test_file_io_plugin.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     3697 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/core_plugins/test_http_plugin.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     4585 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/core_plugins/test_math_plugin.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     1361 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/core_plugins/test_text_plugin.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     4018 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/core_plugins/test_time_plugin.py
--rw-r--r--   0 caoyitong   (502) staff       (20)      995 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/core_plugins/test_wait_plugin.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.780443 flexible_semantic_kernel-1.0.2.dev0/tests/unit/kernel_extensions/
--rw-r--r--   0 caoyitong   (502) staff       (20)     1631 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/kernel_extensions/test_import_plugins.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     1756 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/kernel_extensions/test_register_functions.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.780696 flexible_semantic_kernel-1.0.2.dev0/tests/unit/memory/
--rw-r--r--   0 caoyitong   (502) staff       (20)     2032 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/memory/test_volatile_memory_store.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.674690 flexible_semantic_kernel-1.0.2.dev0/tests/unit/models/
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.780958 flexible_semantic_kernel-1.0.2.dev0/tests/unit/models/chat/
--rw-r--r--   0 caoyitong   (502) staff       (20)     1397 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/models/chat/test_chat_message.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.781746 flexible_semantic_kernel-1.0.2.dev0/tests/unit/openapi/
--rw-r--r--   0 caoyitong   (502) staff       (20)      423 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/openapi/invalid_openapi.yaml
--rw-r--r--   0 caoyitong   (502) staff       (20)     3215 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/openapi/openapi.yaml
--rw-r--r--   0 caoyitong   (502) staff       (20)    10819 2024-04-19 07:51:57.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/openapi/test_sk_openapi.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.782268 flexible_semantic_kernel-1.0.2.dev0/tests/unit/orchestration/
--rw-r--r--   0 caoyitong   (502) staff       (20)     6301 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/orchestration/test_context_variables.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     4791 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/orchestration/test_native_function.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.782801 flexible_semantic_kernel-1.0.2.dev0/tests/unit/planning/
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.783122 flexible_semantic_kernel-1.0.2.dev0/tests/unit/planning/action_planner/
--rw-r--r--   0 caoyitong   (502) staff       (20)     9042 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/planning/action_planner/test_action_planner.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.784108 flexible_semantic_kernel-1.0.2.dev0/tests/unit/planning/sequential_planner/
--rw-r--r--   0 caoyitong   (502) staff       (20)        0 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/planning/sequential_planner/__init__.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     5560 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/planning/sequential_planner/test_sequential_planner.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     8207 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/planning/sequential_planner/test_sequential_planner_extensions.py
--rw-r--r--   0 caoyitong   (502) staff       (20)    11874 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/planning/sequential_planner/test_sequential_planner_parser.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.784429 flexible_semantic_kernel-1.0.2.dev0/tests/unit/planning/stepwise_planner/
--rw-r--r--   0 caoyitong   (502) staff       (20)     1522 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/planning/stepwise_planner/test_stepwise_planner_parse_result.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     6424 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/planning/test_plan_creation.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     6231 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/planning/test_plan_execution.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.785335 flexible_semantic_kernel-1.0.2.dev0/tests/unit/plugin_definition/
--rw-r--r--   0 caoyitong   (502) staff       (20)     4843 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/plugin_definition/test_functions_view.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     6993 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/plugin_definition/test_prompt_templates.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     1001 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/plugin_definition/test_sk_function_decorators.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.786052 flexible_semantic_kernel-1.0.2.dev0/tests/unit/template_engine/
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.787697 flexible_semantic_kernel-1.0.2.dev0/tests/unit/template_engine/blocks/
--rw-r--r--   0 caoyitong   (502) staff       (20)      551 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/template_engine/blocks/test_block.py
--rw-r--r--   0 caoyitong   (502) staff       (20)    12579 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/template_engine/blocks/test_code_block.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     3091 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/template_engine/blocks/test_function_id_block.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     3722 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/template_engine/blocks/test_text_block.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     2765 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/template_engine/blocks/test_val_block.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     4421 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/template_engine/blocks/test_var_block.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     3247 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/template_engine/test_code_tokenizer.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     5741 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/template_engine/test_prompt_template_engine.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     5694 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/template_engine/test_template_tokenizer.py
--rw-r--r--   0 caoyitong   (502) staff       (20)     5626 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/test_kernel.py
--rw-r--r--   0 caoyitong   (502) staff       (20)    10090 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/test_serialization.py
-drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-24 09:04:43.788293 flexible_semantic_kernel-1.0.2.dev0/tests/unit/text/
--rw-r--r--   0 caoyitong   (502) staff       (20)     1088 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/text/test_function_extension.py
--rw-r--r--   0 caoyitong   (502) staff       (20)    19572 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.2.dev0/tests/unit/text/test_text_chunker.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.571137 flexible_semantic_kernel-1.0.3.dev0/
+-rw-r--r--   0 caoyitong   (502) staff       (20)     2050 2024-03-29 07:13:13.000000 flexible_semantic_kernel-1.0.3.dev0/.gitignore
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1547 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.3.dev0/Makefile
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1641 2024-04-25 09:09:57.570860 flexible_semantic_kernel-1.0.3.dev0/PKG-INFO
+-rw-r--r--   0 caoyitong   (502) staff       (20)      127 2024-04-24 06:46:33.000000 flexible_semantic_kernel-1.0.3.dev0/README.md
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.477488 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/
+-rw-r--r--   0 caoyitong   (502) staff       (20)     2150 2024-04-19 09:02:20.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/__init__.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.478827 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/
+-rw-r--r--   0 caoyitong   (502) staff       (20)       48 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/__init__.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.480418 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/
+-rw-r--r--   0 caoyitong   (502) staff       (20)      617 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/__init__.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1735 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/ai_exception.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     3442 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/ai_request_settings.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1242 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/ai_service_client_base.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     2021 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/chat_completion_client_base.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.480705 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/embeddings/
+-rw-r--r--   0 caoyitong   (502) staff       (20)      321 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.481283 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/google_palm/
+-rw-r--r--   0 caoyitong   (502) staff       (20)      763 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/google_palm/__init__.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1645 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/google_palm/gp_request_settings.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.482166 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/google_palm/services/
+-rw-r--r--   0 caoyitong   (502) staff       (20)     8338 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     3243 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/google_palm/services/gp_text_completion.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     2365 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.482715 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/hugging_face/
+-rw-r--r--   0 caoyitong   (502) staff       (20)      535 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/hugging_face/__init__.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1354 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/hugging_face/hf_request_settings.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.483342 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/hugging_face/services/
+-rw-r--r--   0 caoyitong   (502) staff       (20)     6001 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     2305 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.483959 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/ollama/
+-rw-r--r--   0 caoyitong   (502) staff       (20)        0 2024-01-25 07:19:10.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/ollama/__init__.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      710 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/ollama/ollama_request_settings.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.484755 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/ollama/services/
+-rw-r--r--   0 caoyitong   (502) staff       (20)     5419 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     3466 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1785 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      338 2024-01-25 07:19:10.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/ollama/utils.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.485546 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1405 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/__init__.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      246 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/const.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.486151 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/exceptions/
+-rw-r--r--   0 caoyitong   (502) staff       (20)       48 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/exceptions/__init__.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     3523 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.466062 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/models/
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.487057 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/models/chat/
+-rw-r--r--   0 caoyitong   (502) staff       (20)     3360 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/models/chat/azure_chat_with_data_response.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1246 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/models/chat/function_call.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      463 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/models/chat/open_ai_chat_message.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.487596 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/request_settings/
+-rw-r--r--   0 caoyitong   (502) staff       (20)     2858 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/request_settings/azure_chat_request_settings.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     3757 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/request_settings/open_ai_request_settings.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.487849 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/semantic_functions/
+-rw-r--r--   0 caoyitong   (502) staff       (20)     4239 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/semantic_functions/open_ai_chat_prompt_template.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.492033 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/
+-rw-r--r--   0 caoyitong   (502) staff       (20)    16579 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     5657 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     8813 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     5207 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     8467 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     3895 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     4603 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/open_ai_handler.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      230 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/open_ai_model_types.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     4653 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     4551 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     3070 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1921 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     9797 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/utils.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1707 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/text_completion_client_base.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.492327 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/
+-rw-r--r--   0 caoyitong   (502) staff       (20)       48 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/__init__.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.493445 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/azure_cognitive_search/
+-rw-r--r--   0 caoyitong   (502) staff       (20)      251 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/azure_cognitive_search/__init__.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)    15436 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     8187 2024-04-19 07:51:57.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/azure_cognitive_search/utils.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.494953 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/azure_cosmosdb/
+-rw-r--r--   0 caoyitong   (502) staff       (20)      222 2024-04-19 09:02:20.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/azure_cosmosdb/__init__.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     9514 2024-04-19 09:02:20.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     2239 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_store_api.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      403 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/azure_cosmosdb/cosmosdb_utils.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     7397 2024-04-19 09:02:20.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/azure_cosmosdb/mongo_vcore_store_api.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.495825 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/chroma/
+-rw-r--r--   0 caoyitong   (502) staff       (20)      191 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/chroma/__init__.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)    14974 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/chroma/chroma_memory_store.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     4612 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/chroma/utils.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.496427 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/milvus/
+-rw-r--r--   0 caoyitong   (502) staff       (20)      142 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/milvus/__init__.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)    16441 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/milvus/milvus_memory_store.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.497655 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/mongodb_atlas/
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1458 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/mongodb_atlas/README.md
+-rw-r--r--   0 caoyitong   (502) staff       (20)      168 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/mongodb_atlas/__init__.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)    12682 2024-04-19 09:02:20.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     2311 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/mongodb_atlas/utils.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.498466 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/pinecone/
+-rw-r--r--   0 caoyitong   (502) staff       (20)      199 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/pinecone/__init__.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)    14643 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1163 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/pinecone/utils.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.498978 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/postgres/
+-rw-r--r--   0 caoyitong   (502) staff       (20)      199 2024-04-19 09:02:20.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/postgres/__init__.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)    20169 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/postgres/postgres_memory_store.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.499755 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/qdrant/
+-rw-r--r--   0 caoyitong   (502) staff       (20)      191 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/qdrant/__init__.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)    11743 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.500884 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/redis/
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1294 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/redis/README.md
+-rw-r--r--   0 caoyitong   (502) staff       (20)      187 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/redis/__init__.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)    15491 2024-04-19 09:02:20.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/redis/redis_memory_store.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     3686 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/redis/utils.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.501398 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/usearch/
+-rw-r--r--   0 caoyitong   (502) staff       (20)      195 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/usearch/__init__.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)    23333 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/usearch/usearch_memory_store.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.502107 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/weaviate/
+-rw-r--r--   0 caoyitong   (502) staff       (20)      197 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/weaviate/__init__.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)    11033 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.502678 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/openapi/
+-rw-r--r--   0 caoyitong   (502) staff       (20)      137 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/openapi/__init__.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)    11180 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/openapi/sk_openapi.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.503737 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/search_engine/
+-rw-r--r--   0 caoyitong   (502) staff       (20)      283 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/search_engine/__init__.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     2838 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/search_engine/bing_connector.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      254 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/search_engine/connector.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     3189 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/search_engine/google_connector.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      484 2024-04-19 07:56:23.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/telemetry.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.506204 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/core_plugins/
+-rw-r--r--   0 caoyitong   (502) staff       (20)      908 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/core_plugins/__init__.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     2593 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/core_plugins/conversation_summary_plugin.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     2038 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/core_plugins/file_io_plugin.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     3833 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/core_plugins/http_plugin.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     3348 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/core_plugins/math_plugin.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     5327 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/core_plugins/text_memory_plugin.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     2551 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/core_plugins/text_plugin.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     7984 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/core_plugins/time_plugin.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      775 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/core_plugins/wait_plugin.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     2010 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/core_plugins/web_search_engine_plugin.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.507292 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/events/
+-rw-r--r--   0 caoyitong   (502) staff       (20)      334 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/events/__init__.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      452 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/events/function_invoked_event_args.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      443 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/events/function_invoking_event_args.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      892 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/events/sk_events_args.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)    35066 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/kernel.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1728 2024-01-25 07:19:10.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/kernel_exception.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.509414 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/memory/
+-rw-r--r--   0 caoyitong   (502) staff       (20)      169 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/memory/__init__.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     2553 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/memory/memory_query_result.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     4267 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/memory/memory_record.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     7239 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/memory/memory_store_base.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1670 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/memory/null_memory.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     6368 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/memory/semantic_text_memory.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     3586 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/memory/semantic_text_memory_base.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)    11877 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/memory/volatile_memory_store.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.468127 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/models/
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.509703 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/models/chat/
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1543 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/models/chat/chat_message.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.511830 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/orchestration/
+-rw-r--r--   0 caoyitong   (502) staff       (20)     4774 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/orchestration/context_variables.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     6058 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/orchestration/delegate_handlers.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)    12075 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/orchestration/delegate_inference.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      781 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/orchestration/delegate_types.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     7855 2024-04-23 04:41:13.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/orchestration/sk_context.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)    22571 2024-04-25 06:50:34.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/orchestration/sk_function.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     5933 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/orchestration/sk_function_base.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.513159 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/
+-rw-r--r--   0 caoyitong   (502) staff       (20)      655 2024-04-19 06:49:52.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/__init__.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.514341 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/action_planner/
+-rw-r--r--   0 caoyitong   (502) staff       (20)      135 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/action_planner/__init__.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)    11525 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/action_planner/action_planner.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      363 2024-03-29 07:04:59.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/action_planner/config.json
+-rw-r--r--   0 caoyitong   (502) staff       (20)     3087 2024-03-29 07:04:15.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/action_planner/skprompt.txt
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.515414 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/basic_planner/
+-rw-r--r--   0 caoyitong   (502) staff       (20)      131 2024-04-19 06:51:32.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/basic_planner/__init__.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)    11086 2024-04-25 06:51:59.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/basic_planner/basic_planner.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      363 2024-03-29 07:05:10.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/basic_planner/config.json
+-rw-r--r--   0 caoyitong   (502) staff       (20)     6310 2024-03-29 03:35:11.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/basic_planner/skprompt.txt
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.516549 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/multimodal_planner/
+-rw-r--r--   0 caoyitong   (502) staff       (20)      376 2024-04-11 02:49:35.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/multimodal_planner/__init__.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      363 2024-04-23 06:38:36.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/multimodal_planner/config.json
+-rw-r--r--   0 caoyitong   (502) staff       (20)    10981 2024-04-23 07:02:33.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/multimodal_planner/multimodal_planner.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     7907 2024-04-19 02:26:50.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/multimodal_planner/skprompt.txt
+-rw-r--r--   0 caoyitong   (502) staff       (20)    17750 2024-04-24 03:07:39.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/plan.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1632 2024-04-25 02:26:27.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/planner_config.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1198 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/planning_exception.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.517926 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/sequential_planner/
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.468833 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/sequential_planner/Plugins/
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.518530 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/sequential_planner/Plugins/SequentialPlanning/
+-rw-r--r--   0 caoyitong   (502) staff       (20)      687 2024-01-25 07:19:10.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/sequential_planner/Plugins/SequentialPlanning/config.json
+-rw-r--r--   0 caoyitong   (502) staff       (20)     3019 2024-01-25 07:19:10.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/sequential_planner/Plugins/SequentialPlanning/skprompt.txt
+-rw-r--r--   0 caoyitong   (502) staff       (20)      151 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/sequential_planner/__init__.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     5764 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/sequential_planner/sequential_planner.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1153 2024-01-25 07:19:10.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/sequential_planner/sequential_planner_config.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     7958 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/sequential_planner/sequential_planner_extensions.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     5403 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/sequential_planner/sequential_planner_parser.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.519529 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/stepwise_planner/
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.469075 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/stepwise_planner/Plugins/
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.519941 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/stepwise_planner/Plugins/StepwiseStep/
+-rw-r--r--   0 caoyitong   (502) staff       (20)      860 2024-01-25 07:19:10.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/stepwise_planner/Plugins/StepwiseStep/config.json
+-rw-r--r--   0 caoyitong   (502) staff       (20)     2822 2024-01-25 07:19:10.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/stepwise_planner/Plugins/StepwiseStep/skprompt.txt
+-rw-r--r--   0 caoyitong   (502) staff       (20)      134 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/stepwise_planner/__init__.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)    16147 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/stepwise_planner/stepwise_planner.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      982 2024-01-25 07:19:10.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/stepwise_planner/stepwise_planner_config.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      371 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/stepwise_planner/system_step.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.523281 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/plugin_definition/
+-rw-r--r--   0 caoyitong   (502) staff       (20)      342 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/plugin_definition/__init__.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      119 2024-01-25 07:19:10.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/plugin_definition/constants.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      990 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/plugin_definition/function_view.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     2243 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/plugin_definition/functions_view.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      613 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/plugin_definition/parameter_view.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     4477 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/plugin_definition/plugin_collection.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      892 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/plugin_definition/plugin_collection_base.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     4755 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/plugin_definition/read_only_plugin_collection.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1362 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/plugin_definition/read_only_plugin_collection_base.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1071 2024-01-25 07:19:10.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/plugin_definition/sk_function_context_parameter_decorator.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      840 2024-01-25 07:19:10.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/plugin_definition/sk_function_decorator.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.523772 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/reliability/
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1160 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/reliability/pass_through_without_retry.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      836 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/reliability/retry_mechanism_base.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.524993 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/semantic_functions/
+-rw-r--r--   0 caoyitong   (502) staff       (20)     5642 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/semantic_functions/chat_prompt_template.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     2665 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/semantic_functions/prompt_template.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      600 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/semantic_functions/prompt_template_base.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     3299 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/semantic_functions/prompt_template_config.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      698 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/semantic_functions/semantic_function_config.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      602 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/sk_pydantic.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.526123 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/template_engine/
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1115 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/template_engine/README.md
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.528286 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/template_engine/blocks/
+-rw-r--r--   0 caoyitong   (502) staff       (20)      827 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/template_engine/blocks/block.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      228 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/template_engine/blocks/block_types.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     4711 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/template_engine/blocks/code_block.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     3214 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/template_engine/blocks/function_id_block.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      276 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/template_engine/blocks/symbols.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1636 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/template_engine/blocks/text_block.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     2369 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/template_engine/blocks/val_block.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     2754 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/template_engine/blocks/var_block.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     6607 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/template_engine/code_tokenizer.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     6243 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/template_engine/prompt_template_engine.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.529023 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/template_engine/protocols/
+-rw-r--r--   0 caoyitong   (502) staff       (20)      541 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/template_engine/protocols/code_renderer.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     3110 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/template_engine/protocols/prompt_templating_engine.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      605 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/template_engine/protocols/text_renderer.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     7354 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/template_engine/template_tokenizer.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.529761 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/text/
+-rw-r--r--   0 caoyitong   (502) staff       (20)      491 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/text/__init__.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      685 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/text/function_extension.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     8474 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/text/text_chunker.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.530746 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/utils/
+-rw-r--r--   0 caoyitong   (502) staff       (20)      276 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/utils/logging.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1161 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/utils/null_logger.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     8264 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/utils/settings.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      221 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/utils/static_property.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     2218 2024-01-25 07:19:10.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/utils/validation.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.570362 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel.egg-info/
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1641 2024-04-25 09:09:57.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel.egg-info/PKG-INFO
+-rw-r--r--   0 caoyitong   (502) staff       (20)    20173 2024-04-25 09:09:57.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel.egg-info/SOURCES.txt
+-rw-r--r--   0 caoyitong   (502) staff       (20)        1 2024-04-25 09:09:57.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel.egg-info/dependency_links.txt
+-rw-r--r--   0 caoyitong   (502) staff       (20)      626 2024-04-25 09:09:57.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel.egg-info/requires.txt
+-rw-r--r--   0 caoyitong   (502) staff       (20)       25 2024-04-25 09:09:57.000000 flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel.egg-info/top_level.txt
+-rw-r--r--   0 caoyitong   (502) staff       (20)        0 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.3.dev0/log.txt
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.535508 flexible_semantic_kernel-1.0.3.dev0/notebooks/
+-rw-r--r--   0 caoyitong   (502) staff       (20)      164 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.3.dev0/notebooks/.env.example
+-rw-r--r--   0 caoyitong   (502) staff       (20)     3658 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/notebooks/00-getting-started.ipynb
+-rw-r--r--   0 caoyitong   (502) staff       (20)     4399 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/notebooks/01-basic-loading-the-kernel.ipynb
+-rw-r--r--   0 caoyitong   (502) staff       (20)     5980 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/notebooks/02-running-prompts-from-file.ipynb
+-rw-r--r--   0 caoyitong   (502) staff       (20)     9993 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/notebooks/03-semantic-function-inline.ipynb
+-rw-r--r--   0 caoyitong   (502) staff       (20)     7306 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/notebooks/04-context-variables-chat.ipynb
+-rw-r--r--   0 caoyitong   (502) staff       (20)    17829 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/notebooks/05-using-the-planner.ipynb
+-rw-r--r--   0 caoyitong   (502) staff       (20)    85718 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/notebooks/06-memory-and-embeddings.ipynb
+-rw-r--r--   0 caoyitong   (502) staff       (20)     6213 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/notebooks/07-hugging-face-for-plugins.ipynb
+-rw-r--r--   0 caoyitong   (502) staff       (20)    19082 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/notebooks/08-native-function-inline.ipynb
+-rw-r--r--   0 caoyitong   (502) staff       (20)    14004 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/notebooks/09-groundedness-checking.ipynb
+-rw-r--r--   0 caoyitong   (502) staff       (20)    12330 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/notebooks/10-multiple-results-per-prompt.ipynb
+-rw-r--r--   0 caoyitong   (502) staff       (20)     9589 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/notebooks/11-streaming-completions.ipynb
+-rw-r--r--   0 caoyitong   (502) staff       (20)      421 2024-01-25 07:19:10.000000 flexible_semantic_kernel-1.0.3.dev0/notebooks/services.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.536036 flexible_semantic_kernel-1.0.3.dev0/notebooks/third_party/
+-rw-r--r--   0 caoyitong   (502) staff       (20)      175 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.3.dev0/notebooks/third_party/.env.example
+-rw-r--r--   0 caoyitong   (502) staff       (20)    17395 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/notebooks/third_party/weaviate-persistent-memory.ipynb
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1684 2024-04-25 09:09:37.000000 flexible_semantic_kernel-1.0.3.dev0/pyproject.toml
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.536452 flexible_semantic_kernel-1.0.3.dev0/samples/
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.543104 flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1339 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/action_planner.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     4252 2024-04-19 09:02:20.000000 flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/azure_chat_gpt_api.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     3533 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/azure_chat_gpt_with_data_api.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     3274 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/azure_chat_gpt_with_data_api_cross_lingual.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     4678 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/azure_chat_gpt_with_data_api_function_calling.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     3622 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/azure_chat_gpt_with_data_api_vector_search.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     3039 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/azure_cognitive_search_memory.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     2226 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/bing_search_plugin.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1779 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/chat.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1910 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/chat_gpt_api.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     4140 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/chat_gpt_api_function_calling.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1683 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/google_palm_chat.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     4949 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/google_palm_chat_with_memory.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     2664 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/google_palm_chat_with_plugin.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1898 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/google_palm_text_completion.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     3227 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/google_search_plugin.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)    10532 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/grounded.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     4079 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/memory.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     4207 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/openai_function_calling.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     6577 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/openai_logit_bias.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.544465 flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/openapi_example/
+-rw-r--r--   0 caoyitong   (502) staff       (20)      456 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/openapi_example/README.md
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1003 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/openapi_example/openapi.yaml
+-rw-r--r--   0 caoyitong   (502) staff       (20)      785 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/openapi_example/openapi_client.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      540 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/openapi_example/openapi_server.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1163 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/plugins_from_dir.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     5052 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/self-critique_rag.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1504 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/sequential_planner.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      862 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/setup_logging.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      991 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.3.dev0/samples/utils.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)       38 2024-04-25 09:09:57.571182 flexible_semantic_kernel-1.0.3.dev0/setup.cfg
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.544867 flexible_semantic_kernel-1.0.3.dev0/tests/
+-rw-r--r--   0 caoyitong   (502) staff       (20)       48 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.3.dev0/tests/__init__.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     3564 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/conftest.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.471805 flexible_semantic_kernel-1.0.3.dev0/tests/integration/
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.547613 flexible_semantic_kernel-1.0.3.dev0/tests/integration/completions/
+-rw-r--r--   0 caoyitong   (502) staff       (20)     6407 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/integration/completions/conftest.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     2904 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/integration/completions/test_azure_oai_chat_service.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     5404 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/tests/integration/completions/test_azure_oai_chat_service_extensions.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     2974 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/integration/completions/test_azure_oai_text_service.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     2499 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/tests/integration/completions/test_conversation_summary_plugin.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1991 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/integration/completions/test_gp_chat_service.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     3845 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/integration/completions/test_gp_text_service.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     5171 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/integration/completions/test_hf_local_text_completions.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     3856 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/tests/integration/completions/test_hf_local_text_summarization.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     3548 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/integration/completions/test_oai_chat_service.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     3644 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/integration/completions/test_oai_text_service.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      608 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.3.dev0/tests/integration/completions/test_utils.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.471418 flexible_semantic_kernel-1.0.3.dev0/tests/integration/connectors/
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.550799 flexible_semantic_kernel-1.0.3.dev0/tests/integration/connectors/memory/
+-rw-r--r--   0 caoyitong   (502) staff       (20)     5225 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/integration/connectors/memory/test_azure_cognitive_search.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     5909 2024-04-19 09:02:20.000000 flexible_semantic_kernel-1.0.3.dev0/tests/integration/connectors/memory/test_azure_cosmosdb_memory_store.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     7822 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/integration/connectors/memory/test_chroma.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     8566 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/tests/integration/connectors/memory/test_milvus.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     8917 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/integration/connectors/memory/test_mongodb_atlas.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     9908 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/integration/connectors/memory/test_pinecone.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     8182 2024-04-19 09:02:20.000000 flexible_semantic_kernel-1.0.3.dev0/tests/integration/connectors/memory/test_postgres.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     8014 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/tests/integration/connectors/memory/test_qdrant_memory_store.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     8972 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/integration/connectors/memory/test_redis.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)    12860 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/integration/connectors/memory/test_usearch.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     9925 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/integration/connectors/memory/test_weaviate_memory_store.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.551859 flexible_semantic_kernel-1.0.3.dev0/tests/integration/embeddings/
+-rw-r--r--   0 caoyitong   (502) staff       (20)     3033 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/integration/embeddings/test_azure_oai_embedding_service.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1168 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/integration/embeddings/test_gp_embedding_service.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     2190 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/integration/embeddings/test_hf_embedding_service.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1681 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/integration/embeddings/test_oai_embedding_service.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.552772 flexible_semantic_kernel-1.0.3.dev0/tests/integration/fakes/
+-rw-r--r--   0 caoyitong   (502) staff       (20)      888 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/tests/integration/fakes/email_plugin_fake.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      510 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/integration/fakes/fun_plugin_fake.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      513 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/integration/fakes/summarize_plugin_fake.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      901 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/integration/fakes/writer_plugin_fake.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.471986 flexible_semantic_kernel-1.0.3.dev0/tests/integration/planning/
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.553378 flexible_semantic_kernel-1.0.3.dev0/tests/integration/planning/sequential_planner/
+-rw-r--r--   0 caoyitong   (502) staff       (20)     2635 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/integration/planning/sequential_planner/test_sequential_plan_parser.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     5127 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/tests/integration/planning/sequential_planner/test_sequential_planner.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.553674 flexible_semantic_kernel-1.0.3.dev0/tests/integration/planning/stepwise_planner/
+-rw-r--r--   0 caoyitong   (502) staff       (20)     5835 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/integration/planning/stepwise_planner/test_stepwise_planner.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.554248 flexible_semantic_kernel-1.0.3.dev0/tests/template_engine/
+-rw-r--r--   0 caoyitong   (502) staff       (20)     4613 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/template_engine/prompt_template_e2e_tests.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1571 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.3.dev0/tests/template_engine/tests.txt
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.472232 flexible_semantic_kernel-1.0.3.dev0/tests/test_native_plugins/
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.554522 flexible_semantic_kernel-1.0.3.dev0/tests/test_native_plugins/TestNativePlugin/
+-rw-r--r--   0 caoyitong   (502) staff       (20)      582 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/test_native_plugins/TestNativePlugin/native_function.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.472386 flexible_semantic_kernel-1.0.3.dev0/tests/test_plugins/
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.472453 flexible_semantic_kernel-1.0.3.dev0/tests/test_plugins/TestPlugin/
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.555076 flexible_semantic_kernel-1.0.3.dev0/tests/test_plugins/TestPlugin/TestFunction/
+-rw-r--r--   0 caoyitong   (502) staff       (20)      284 2024-01-25 07:19:10.000000 flexible_semantic_kernel-1.0.3.dev0/tests/test_plugins/TestPlugin/TestFunction/config.json
+-rw-r--r--   0 caoyitong   (502) staff       (20)       31 2024-01-25 07:19:10.000000 flexible_semantic_kernel-1.0.3.dev0/tests/test_plugins/TestPlugin/TestFunction/skprompt.txt
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.555584 flexible_semantic_kernel-1.0.3.dev0/tests/unit/
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.555979 flexible_semantic_kernel-1.0.3.dev0/tests/unit/ai/
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.472840 flexible_semantic_kernel-1.0.3.dev0/tests/unit/ai/google_palm/
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.557481 flexible_semantic_kernel-1.0.3.dev0/tests/unit/ai/google_palm/services/
+-rw-r--r--   0 caoyitong   (502) staff       (20)     2546 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/ai/google_palm/services/test_palm_chat_completion.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     2572 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/ai/google_palm/services/test_palm_text_completion.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1954 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/ai/google_palm/services/test_palm_text_embedding.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.557768 flexible_semantic_kernel-1.0.3.dev0/tests/unit/ai/ollama/
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.558268 flexible_semantic_kernel-1.0.3.dev0/tests/unit/ai/ollama/services/
+-rw-r--r--   0 caoyitong   (502) staff       (20)     3409 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/ai/ollama/services/test_ollama_chat_completion.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1738 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/ai/ollama/services/test_ollama_test_completion.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      830 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/ai/ollama/services/test_ollama_text_embedding.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      578 2024-01-25 07:19:10.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/ai/ollama/utils.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.558529 flexible_semantic_kernel-1.0.3.dev0/tests/unit/ai/open_ai/
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.473324 flexible_semantic_kernel-1.0.3.dev0/tests/unit/ai/open_ai/models/
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.558823 flexible_semantic_kernel-1.0.3.dev0/tests/unit/ai/open_ai/models/chat/
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1078 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/ai/open_ai/models/chat/test_function_call.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.560268 flexible_semantic_kernel-1.0.3.dev0/tests/unit/ai/open_ai/services/
+-rw-r--r--   0 caoyitong   (502) staff       (20)    18931 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/ai/open_ai/services/test_azure_chat_completion.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     7893 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/ai/open_ai/services/test_azure_text_completion.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     5864 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/ai/open_ai/services/test_azure_text_embedding.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     3851 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/ai/open_ai/services/test_openai_chat_completion.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     3356 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/ai/open_ai/services/test_openai_text_completion.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)    10256 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/ai/open_ai/test_openai_request_settings.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      540 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/ai/test_ai_request_settings.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.561663 flexible_semantic_kernel-1.0.3.dev0/tests/unit/core_plugins/
+-rw-r--r--   0 caoyitong   (502) staff       (20)     2520 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/core_plugins/test_file_io_plugin.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     3697 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/core_plugins/test_http_plugin.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     4585 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/core_plugins/test_math_plugin.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1361 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/core_plugins/test_text_plugin.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     4018 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/core_plugins/test_time_plugin.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)      995 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/core_plugins/test_wait_plugin.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.562119 flexible_semantic_kernel-1.0.3.dev0/tests/unit/kernel_extensions/
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1631 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/kernel_extensions/test_import_plugins.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1756 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/kernel_extensions/test_register_functions.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.562372 flexible_semantic_kernel-1.0.3.dev0/tests/unit/memory/
+-rw-r--r--   0 caoyitong   (502) staff       (20)     2032 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/memory/test_volatile_memory_store.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.473962 flexible_semantic_kernel-1.0.3.dev0/tests/unit/models/
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.562636 flexible_semantic_kernel-1.0.3.dev0/tests/unit/models/chat/
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1397 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/models/chat/test_chat_message.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.563442 flexible_semantic_kernel-1.0.3.dev0/tests/unit/openapi/
+-rw-r--r--   0 caoyitong   (502) staff       (20)      423 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/openapi/invalid_openapi.yaml
+-rw-r--r--   0 caoyitong   (502) staff       (20)     3215 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/openapi/openapi.yaml
+-rw-r--r--   0 caoyitong   (502) staff       (20)    10819 2024-04-19 07:51:57.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/openapi/test_sk_openapi.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.564017 flexible_semantic_kernel-1.0.3.dev0/tests/unit/orchestration/
+-rw-r--r--   0 caoyitong   (502) staff       (20)     6301 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/orchestration/test_context_variables.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     4791 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/orchestration/test_native_function.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.564576 flexible_semantic_kernel-1.0.3.dev0/tests/unit/planning/
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.564904 flexible_semantic_kernel-1.0.3.dev0/tests/unit/planning/action_planner/
+-rw-r--r--   0 caoyitong   (502) staff       (20)     9042 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/planning/action_planner/test_action_planner.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.566064 flexible_semantic_kernel-1.0.3.dev0/tests/unit/planning/sequential_planner/
+-rw-r--r--   0 caoyitong   (502) staff       (20)        0 2024-01-09 01:41:32.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/planning/sequential_planner/__init__.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     5560 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/planning/sequential_planner/test_sequential_planner.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     8207 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/planning/sequential_planner/test_sequential_planner_extensions.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)    11874 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/planning/sequential_planner/test_sequential_planner_parser.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.566358 flexible_semantic_kernel-1.0.3.dev0/tests/unit/planning/stepwise_planner/
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1522 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/planning/stepwise_planner/test_stepwise_planner_parse_result.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     6424 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/planning/test_plan_creation.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     6231 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/planning/test_plan_execution.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.567186 flexible_semantic_kernel-1.0.3.dev0/tests/unit/plugin_definition/
+-rw-r--r--   0 caoyitong   (502) staff       (20)     4843 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/plugin_definition/test_functions_view.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     6993 2024-04-16 08:04:11.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/plugin_definition/test_prompt_templates.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1001 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/plugin_definition/test_sk_function_decorators.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.567862 flexible_semantic_kernel-1.0.3.dev0/tests/unit/template_engine/
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.569429 flexible_semantic_kernel-1.0.3.dev0/tests/unit/template_engine/blocks/
+-rw-r--r--   0 caoyitong   (502) staff       (20)      551 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/template_engine/blocks/test_block.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)    12579 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/template_engine/blocks/test_code_block.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     3091 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/template_engine/blocks/test_function_id_block.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     3722 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/template_engine/blocks/test_text_block.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     2765 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/template_engine/blocks/test_val_block.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     4421 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/template_engine/blocks/test_var_block.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     3247 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/template_engine/test_code_tokenizer.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     5741 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/template_engine/test_prompt_template_engine.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     5694 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/template_engine/test_template_tokenizer.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)     5626 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/test_kernel.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)    10090 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/test_serialization.py
+drwxr-xr-x   0 caoyitong   (502) staff       (20)        0 2024-04-25 09:09:57.569954 flexible_semantic_kernel-1.0.3.dev0/tests/unit/text/
+-rw-r--r--   0 caoyitong   (502) staff       (20)     1088 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/text/test_function_extension.py
+-rw-r--r--   0 caoyitong   (502) staff       (20)    19572 2024-04-16 08:04:12.000000 flexible_semantic_kernel-1.0.3.dev0/tests/unit/text/test_text_chunker.py
```

### Comparing `flexible_semantic_kernel-1.0.2.dev0/.gitignore` & `flexible_semantic_kernel-1.0.3.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/Makefile` & `flexible_semantic_kernel-1.0.3.dev0/Makefile`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/PKG-INFO` & `flexible_semantic_kernel-1.0.3.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flexible_semantic_kernel
-Version: 1.0.2.dev0
+Version: 1.0.3.dev0
 Summary: flexible-semantic-kernel
 Author-email: YitongCao <ytea.cao@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/__init__.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/__init__.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/__init__.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/ai_exception.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/ai_exception.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/ai_request_settings.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/ai_request_settings.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/ai_service_client_base.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/ai_service_client_base.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/chat_completion_client_base.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/chat_completion_client_base.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/google_palm/__init__.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/google_palm/__init__.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/google_palm/gp_request_settings.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/google_palm/gp_request_settings.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/google_palm/services/gp_text_completion.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/google_palm/services/gp_text_completion.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/hugging_face/__init__.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/hugging_face/__init__.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/hugging_face/hf_request_settings.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/hugging_face/hf_request_settings.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/ollama/ollama_request_settings.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/ollama/ollama_request_settings.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/__init__.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/models/chat/azure_chat_with_data_response.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/models/chat/azure_chat_with_data_response.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/models/chat/function_call.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/models/chat/function_call.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/request_settings/azure_chat_request_settings.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/request_settings/azure_chat_request_settings.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/request_settings/open_ai_request_settings.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/request_settings/open_ai_request_settings.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/semantic_functions/open_ai_chat_prompt_template.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/semantic_functions/open_ai_chat_prompt_template.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/open_ai_handler.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/open_ai_handler.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/open_ai/utils.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/open_ai/utils.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/ai/text_completion_client_base.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/ai/text_completion_client_base.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/azure_cognitive_search/utils.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/azure_cognitive_search/utils.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_store_api.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_store_api.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/azure_cosmosdb/mongo_vcore_store_api.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/azure_cosmosdb/mongo_vcore_store_api.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/chroma/chroma_memory_store.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/chroma/chroma_memory_store.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/chroma/utils.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/chroma/utils.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/milvus/milvus_memory_store.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/milvus/milvus_memory_store.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/mongodb_atlas/README.md` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/mongodb_atlas/README.md`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/mongodb_atlas/utils.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/mongodb_atlas/utils.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/pinecone/utils.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/pinecone/utils.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/postgres/postgres_memory_store.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/postgres/postgres_memory_store.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/redis/README.md` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/redis/README.md`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/redis/redis_memory_store.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/redis/redis_memory_store.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/redis/utils.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/redis/utils.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/usearch/usearch_memory_store.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/usearch/usearch_memory_store.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/openapi/sk_openapi.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/openapi/sk_openapi.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/search_engine/bing_connector.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/search_engine/bing_connector.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/connectors/search_engine/google_connector.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/connectors/search_engine/google_connector.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/core_plugins/__init__.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/core_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/core_plugins/conversation_summary_plugin.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/core_plugins/conversation_summary_plugin.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/core_plugins/file_io_plugin.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/core_plugins/file_io_plugin.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/core_plugins/http_plugin.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/core_plugins/http_plugin.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/core_plugins/math_plugin.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/core_plugins/math_plugin.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/core_plugins/text_memory_plugin.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/core_plugins/text_memory_plugin.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/core_plugins/text_plugin.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/core_plugins/text_plugin.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/core_plugins/time_plugin.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/core_plugins/time_plugin.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/core_plugins/wait_plugin.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/core_plugins/wait_plugin.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/core_plugins/web_search_engine_plugin.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/core_plugins/web_search_engine_plugin.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/events/sk_events_args.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/events/sk_events_args.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/kernel.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/kernel.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/kernel_exception.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/kernel_exception.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/memory/memory_query_result.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/memory/memory_query_result.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/memory/memory_record.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/memory/memory_record.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/memory/memory_store_base.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/memory/memory_store_base.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/memory/null_memory.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/memory/null_memory.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/memory/semantic_text_memory.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/memory/semantic_text_memory.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/memory/semantic_text_memory_base.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/memory/semantic_text_memory_base.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/memory/volatile_memory_store.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/memory/volatile_memory_store.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/models/chat/chat_message.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/models/chat/chat_message.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/orchestration/context_variables.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/orchestration/context_variables.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/orchestration/delegate_handlers.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/orchestration/delegate_handlers.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/orchestration/delegate_inference.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/orchestration/delegate_inference.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/orchestration/delegate_types.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/orchestration/delegate_types.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/orchestration/sk_context.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/orchestration/sk_context.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/orchestration/sk_function.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/orchestration/sk_function.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,14 +129,15 @@
                 if not function_config.has_chat_prompt:
                     prompt = await function_config.prompt_template.render_async(context)
                     completion = await client.complete_async(prompt, request_settings)
                     context.variables.update(completion)
                     return context
             except Exception as e:
                 # TODO: "critical exceptions"
+                logger.error(e)
                 context.fail(str(e), e)
                 return context
 
             as_chat_prompt = function_config.prompt_template
             # Similar to non-chat, render prompt (which renders to a
             # dict of <role, content, name> messages)
             messages = await as_chat_prompt.render_messages_async(context)
```

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/orchestration/sk_function_base.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/orchestration/sk_function_base.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/__init__.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/__init__.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/action_planner/action_planner.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/action_planner/action_planner.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/action_planner/skprompt.txt` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/action_planner/skprompt.txt`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/basic_planner/basic_planner.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/basic_planner/basic_planner.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,15 +240,22 @@
 
         # Add the goal to the context
         self._context.variables.update(goal)
         generated_plan_raw = await self._planner_function.invoke_async(context=self._context)
 
         # plan字符串
         json_regex = r"\{(?:[^{}]|(?R))*\}"
-        generated_plan_str = regex.search(json_regex, generated_plan_raw.result).group()
+        try:
+            generated_plan_str = regex.search(json_regex, generated_plan_raw.result).group()
+        except (AttributeError, ) as error:
+            raise PlanningException(
+                PlanningException.ErrorCodes.InvalidPlan,
+                "Plan format not match"
+            )
+
         generated_plan_str = generated_plan_str.replace('""', '"')
         generated_plan_str = generated_plan_str.replace('\\_', '_')
         # 去除json中的注释
         generated_plan_str_list = []
         for line in generated_plan_str.split("\n"):
             generated_plan_str_list.append(line.split("//")[0])
         generated_plan_str = " ".join(generated_plan_str_list)
```

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/basic_planner/skprompt.txt` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/basic_planner/skprompt.txt`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/multimodal_planner/multimodal_planner.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/multimodal_planner/multimodal_planner.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/multimodal_planner/skprompt.txt` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/multimodal_planner/skprompt.txt`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/plan.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/plan.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/planner_config.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/planner_config.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/planning_exception.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/planning_exception.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/sequential_planner/Plugins/SequentialPlanning/config.json` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/sequential_planner/Plugins/SequentialPlanning/config.json`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/sequential_planner/Plugins/SequentialPlanning/skprompt.txt` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/sequential_planner/Plugins/SequentialPlanning/skprompt.txt`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/sequential_planner/sequential_planner.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/sequential_planner/sequential_planner.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/sequential_planner/sequential_planner_config.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/sequential_planner/sequential_planner_config.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/sequential_planner/sequential_planner_extensions.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/sequential_planner/sequential_planner_extensions.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/sequential_planner/sequential_planner_parser.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/sequential_planner/sequential_planner_parser.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/stepwise_planner/Plugins/StepwiseStep/config.json` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/stepwise_planner/Plugins/StepwiseStep/config.json`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/stepwise_planner/Plugins/StepwiseStep/skprompt.txt` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/stepwise_planner/Plugins/StepwiseStep/skprompt.txt`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/stepwise_planner/stepwise_planner.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/stepwise_planner/stepwise_planner.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/planning/stepwise_planner/stepwise_planner_config.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/planning/stepwise_planner/stepwise_planner_config.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/plugin_definition/function_view.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/plugin_definition/function_view.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/plugin_definition/functions_view.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/plugin_definition/functions_view.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/plugin_definition/parameter_view.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/plugin_definition/parameter_view.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/plugin_definition/plugin_collection.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/plugin_definition/plugin_collection.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/plugin_definition/plugin_collection_base.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/plugin_definition/plugin_collection_base.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/plugin_definition/read_only_plugin_collection.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/plugin_definition/read_only_plugin_collection.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/plugin_definition/read_only_plugin_collection_base.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/plugin_definition/read_only_plugin_collection_base.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/plugin_definition/sk_function_context_parameter_decorator.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/plugin_definition/sk_function_context_parameter_decorator.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/plugin_definition/sk_function_decorator.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/plugin_definition/sk_function_decorator.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/reliability/pass_through_without_retry.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/reliability/pass_through_without_retry.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/reliability/retry_mechanism_base.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/reliability/retry_mechanism_base.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/semantic_functions/chat_prompt_template.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/semantic_functions/chat_prompt_template.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/semantic_functions/prompt_template.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/semantic_functions/prompt_template.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/semantic_functions/prompt_template_base.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/semantic_functions/prompt_template_base.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/semantic_functions/prompt_template_config.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/semantic_functions/prompt_template_config.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/semantic_functions/semantic_function_config.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/semantic_functions/semantic_function_config.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/sk_pydantic.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/sk_pydantic.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/template_engine/README.md` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/template_engine/README.md`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/template_engine/blocks/block.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/template_engine/blocks/block.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/template_engine/blocks/code_block.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/template_engine/blocks/code_block.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/template_engine/blocks/function_id_block.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/template_engine/blocks/function_id_block.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/template_engine/blocks/text_block.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/template_engine/blocks/text_block.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/template_engine/blocks/val_block.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/template_engine/blocks/val_block.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/template_engine/blocks/var_block.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/template_engine/blocks/var_block.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/template_engine/code_tokenizer.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/template_engine/code_tokenizer.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/template_engine/prompt_template_engine.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/template_engine/prompt_template_engine.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/template_engine/protocols/code_renderer.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/template_engine/protocols/code_renderer.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/template_engine/protocols/prompt_templating_engine.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/template_engine/protocols/prompt_templating_engine.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/template_engine/protocols/text_renderer.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/template_engine/protocols/text_renderer.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/template_engine/template_tokenizer.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/template_engine/template_tokenizer.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/text/function_extension.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/text/function_extension.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/text/text_chunker.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/text/text_chunker.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/utils/null_logger.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/utils/null_logger.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/utils/settings.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/utils/settings.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel/utils/validation.py` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel/utils/validation.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel.egg-info/PKG-INFO` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flexible_semantic_kernel
-Version: 1.0.2.dev0
+Version: 1.0.3.dev0
 Summary: flexible-semantic-kernel
 Author-email: YitongCao <ytea.cao@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel.egg-info/SOURCES.txt` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/flexible_semantic_kernel.egg-info/requires.txt` & `flexible_semantic_kernel-1.0.3.dev0/flexible_semantic_kernel.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/notebooks/00-getting-started.ipynb` & `flexible_semantic_kernel-1.0.3.dev0/notebooks/00-getting-started.ipynb`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/notebooks/01-basic-loading-the-kernel.ipynb` & `flexible_semantic_kernel-1.0.3.dev0/notebooks/01-basic-loading-the-kernel.ipynb`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/notebooks/02-running-prompts-from-file.ipynb` & `flexible_semantic_kernel-1.0.3.dev0/notebooks/02-running-prompts-from-file.ipynb`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/notebooks/03-semantic-function-inline.ipynb` & `flexible_semantic_kernel-1.0.3.dev0/notebooks/03-semantic-function-inline.ipynb`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/notebooks/04-context-variables-chat.ipynb` & `flexible_semantic_kernel-1.0.3.dev0/notebooks/04-context-variables-chat.ipynb`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/notebooks/05-using-the-planner.ipynb` & `flexible_semantic_kernel-1.0.3.dev0/notebooks/05-using-the-planner.ipynb`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/notebooks/06-memory-and-embeddings.ipynb` & `flexible_semantic_kernel-1.0.3.dev0/notebooks/06-memory-and-embeddings.ipynb`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/notebooks/07-hugging-face-for-plugins.ipynb` & `flexible_semantic_kernel-1.0.3.dev0/notebooks/07-hugging-face-for-plugins.ipynb`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/notebooks/08-native-function-inline.ipynb` & `flexible_semantic_kernel-1.0.3.dev0/notebooks/08-native-function-inline.ipynb`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/notebooks/09-groundedness-checking.ipynb` & `flexible_semantic_kernel-1.0.3.dev0/notebooks/09-groundedness-checking.ipynb`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/notebooks/10-multiple-results-per-prompt.ipynb` & `flexible_semantic_kernel-1.0.3.dev0/notebooks/10-multiple-results-per-prompt.ipynb`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/notebooks/11-streaming-completions.ipynb` & `flexible_semantic_kernel-1.0.3.dev0/notebooks/11-streaming-completions.ipynb`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/notebooks/third_party/weaviate-persistent-memory.ipynb` & `flexible_semantic_kernel-1.0.3.dev0/notebooks/third_party/weaviate-persistent-memory.ipynb`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/pyproject.toml` & `flexible_semantic_kernel-1.0.3.dev0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "setuptools-scm",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "flexible_semantic_kernel" # 项目名
-version = "1.0.2.dev0" # 版本号
+version = "1.0.3.dev0" # 版本号
 authors = [
   { name="YitongCao", email="ytea.cao@gmail.com" },
 ]
 description = "flexible-semantic-kernel" # 说明
 readme = "README.md" # pypi介绍内容会读取的readme文件
 requires-python = ">=3.10" # 依赖
 classifiers = [
```

### Comparing `flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/action_planner.py` & `flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/action_planner.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/azure_chat_gpt_api.py` & `flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/azure_chat_gpt_api.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/azure_chat_gpt_with_data_api.py` & `flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/azure_chat_gpt_with_data_api.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/azure_chat_gpt_with_data_api_cross_lingual.py` & `flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/azure_chat_gpt_with_data_api_cross_lingual.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/azure_chat_gpt_with_data_api_function_calling.py` & `flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/azure_chat_gpt_with_data_api_function_calling.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/azure_chat_gpt_with_data_api_vector_search.py` & `flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/azure_chat_gpt_with_data_api_vector_search.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/azure_cognitive_search_memory.py` & `flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/azure_cognitive_search_memory.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/bing_search_plugin.py` & `flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/bing_search_plugin.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/chat.py` & `flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/chat.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/chat_gpt_api.py` & `flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/chat_gpt_api.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/chat_gpt_api_function_calling.py` & `flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/chat_gpt_api_function_calling.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/google_palm_chat.py` & `flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/google_palm_chat.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/google_palm_chat_with_memory.py` & `flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/google_palm_chat_with_memory.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/google_palm_chat_with_plugin.py` & `flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/google_palm_chat_with_plugin.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/google_palm_text_completion.py` & `flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/google_palm_text_completion.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/google_search_plugin.py` & `flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/google_search_plugin.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/grounded.py` & `flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/grounded.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/memory.py` & `flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/memory.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/openai_function_calling.py` & `flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/openai_function_calling.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/openai_logit_bias.py` & `flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/openai_logit_bias.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/openapi_example/openapi.yaml` & `flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/openapi_example/openapi.yaml`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/openapi_example/openapi_client.py` & `flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/openapi_example/openapi_client.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/openapi_example/openapi_server.py` & `flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/openapi_example/openapi_server.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/plugins_from_dir.py` & `flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/plugins_from_dir.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/self-critique_rag.py` & `flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/self-critique_rag.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/sequential_planner.py` & `flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/sequential_planner.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/samples/kernel-syntax-examples/setup_logging.py` & `flexible_semantic_kernel-1.0.3.dev0/samples/kernel-syntax-examples/setup_logging.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/samples/utils.py` & `flexible_semantic_kernel-1.0.3.dev0/samples/utils.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/conftest.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/integration/completions/conftest.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/integration/completions/conftest.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/integration/completions/test_azure_oai_chat_service.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/integration/completions/test_azure_oai_chat_service.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/integration/completions/test_azure_oai_chat_service_extensions.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/integration/completions/test_azure_oai_chat_service_extensions.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/integration/completions/test_azure_oai_text_service.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/integration/completions/test_azure_oai_text_service.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/integration/completions/test_conversation_summary_plugin.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/integration/completions/test_conversation_summary_plugin.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/integration/completions/test_gp_chat_service.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/integration/completions/test_gp_chat_service.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/integration/completions/test_gp_text_service.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/integration/completions/test_gp_text_service.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/integration/completions/test_hf_local_text_completions.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/integration/completions/test_hf_local_text_completions.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/integration/completions/test_hf_local_text_summarization.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/integration/completions/test_hf_local_text_summarization.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/integration/completions/test_oai_chat_service.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/integration/completions/test_oai_chat_service.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/integration/completions/test_oai_text_service.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/integration/completions/test_oai_text_service.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/integration/completions/test_utils.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/integration/completions/test_utils.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/integration/connectors/memory/test_azure_cognitive_search.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/integration/connectors/memory/test_azure_cognitive_search.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/integration/connectors/memory/test_azure_cosmosdb_memory_store.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/integration/connectors/memory/test_azure_cosmosdb_memory_store.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/integration/connectors/memory/test_chroma.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/integration/connectors/memory/test_chroma.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/integration/connectors/memory/test_milvus.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/integration/connectors/memory/test_milvus.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/integration/connectors/memory/test_mongodb_atlas.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/integration/connectors/memory/test_mongodb_atlas.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/integration/connectors/memory/test_pinecone.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/integration/connectors/memory/test_pinecone.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/integration/connectors/memory/test_postgres.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/integration/connectors/memory/test_postgres.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/integration/connectors/memory/test_qdrant_memory_store.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/integration/connectors/memory/test_qdrant_memory_store.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/integration/connectors/memory/test_redis.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/integration/connectors/memory/test_redis.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/integration/connectors/memory/test_usearch.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/integration/connectors/memory/test_usearch.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/integration/connectors/memory/test_weaviate_memory_store.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/integration/connectors/memory/test_weaviate_memory_store.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/integration/embeddings/test_azure_oai_embedding_service.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/integration/embeddings/test_azure_oai_embedding_service.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/integration/embeddings/test_gp_embedding_service.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/integration/embeddings/test_gp_embedding_service.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/integration/embeddings/test_hf_embedding_service.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/integration/embeddings/test_hf_embedding_service.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/integration/embeddings/test_oai_embedding_service.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/integration/embeddings/test_oai_embedding_service.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/integration/fakes/email_plugin_fake.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/integration/fakes/email_plugin_fake.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/integration/fakes/summarize_plugin_fake.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/integration/fakes/summarize_plugin_fake.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/integration/fakes/writer_plugin_fake.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/integration/fakes/writer_plugin_fake.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/integration/planning/sequential_planner/test_sequential_plan_parser.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/integration/planning/sequential_planner/test_sequential_plan_parser.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/integration/planning/sequential_planner/test_sequential_planner.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/integration/planning/sequential_planner/test_sequential_planner.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/integration/planning/stepwise_planner/test_stepwise_planner.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/integration/planning/stepwise_planner/test_stepwise_planner.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/template_engine/prompt_template_e2e_tests.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/template_engine/prompt_template_e2e_tests.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/template_engine/tests.txt` & `flexible_semantic_kernel-1.0.3.dev0/tests/template_engine/tests.txt`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/test_native_plugins/TestNativePlugin/native_function.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/test_native_plugins/TestNativePlugin/native_function.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/ai/google_palm/services/test_palm_chat_completion.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/ai/google_palm/services/test_palm_chat_completion.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/ai/google_palm/services/test_palm_text_completion.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/ai/google_palm/services/test_palm_text_completion.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/ai/google_palm/services/test_palm_text_embedding.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/ai/google_palm/services/test_palm_text_embedding.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/ai/ollama/services/test_ollama_chat_completion.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/ai/ollama/services/test_ollama_chat_completion.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/ai/ollama/services/test_ollama_test_completion.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/ai/ollama/services/test_ollama_test_completion.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/ai/ollama/services/test_ollama_text_embedding.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/ai/ollama/services/test_ollama_text_embedding.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/ai/ollama/utils.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/ai/ollama/utils.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/ai/open_ai/models/chat/test_function_call.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/ai/open_ai/models/chat/test_function_call.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/ai/open_ai/services/test_azure_chat_completion.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/ai/open_ai/services/test_azure_chat_completion.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/ai/open_ai/services/test_azure_text_completion.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/ai/open_ai/services/test_azure_text_completion.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/ai/open_ai/services/test_azure_text_embedding.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/ai/open_ai/services/test_azure_text_embedding.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/ai/open_ai/services/test_openai_chat_completion.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/ai/open_ai/services/test_openai_chat_completion.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/ai/open_ai/services/test_openai_text_completion.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/ai/open_ai/services/test_openai_text_completion.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/ai/open_ai/test_openai_request_settings.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/ai/open_ai/test_openai_request_settings.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/ai/test_ai_request_settings.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/ai/test_ai_request_settings.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/core_plugins/test_file_io_plugin.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/core_plugins/test_file_io_plugin.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/core_plugins/test_http_plugin.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/core_plugins/test_http_plugin.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/core_plugins/test_math_plugin.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/core_plugins/test_math_plugin.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/core_plugins/test_text_plugin.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/core_plugins/test_text_plugin.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/core_plugins/test_time_plugin.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/core_plugins/test_time_plugin.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/core_plugins/test_wait_plugin.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/core_plugins/test_wait_plugin.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/kernel_extensions/test_import_plugins.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/kernel_extensions/test_import_plugins.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/kernel_extensions/test_register_functions.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/kernel_extensions/test_register_functions.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/memory/test_volatile_memory_store.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/memory/test_volatile_memory_store.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/models/chat/test_chat_message.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/models/chat/test_chat_message.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/openapi/openapi.yaml` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/openapi/openapi.yaml`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/openapi/test_sk_openapi.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/openapi/test_sk_openapi.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/orchestration/test_context_variables.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/orchestration/test_context_variables.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/orchestration/test_native_function.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/orchestration/test_native_function.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/planning/action_planner/test_action_planner.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/planning/action_planner/test_action_planner.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/planning/sequential_planner/test_sequential_planner.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/planning/sequential_planner/test_sequential_planner.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/planning/sequential_planner/test_sequential_planner_extensions.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/planning/sequential_planner/test_sequential_planner_extensions.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/planning/sequential_planner/test_sequential_planner_parser.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/planning/sequential_planner/test_sequential_planner_parser.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/planning/stepwise_planner/test_stepwise_planner_parse_result.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/planning/stepwise_planner/test_stepwise_planner_parse_result.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/planning/test_plan_creation.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/planning/test_plan_creation.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/planning/test_plan_execution.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/planning/test_plan_execution.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/plugin_definition/test_functions_view.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/plugin_definition/test_functions_view.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/plugin_definition/test_prompt_templates.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/plugin_definition/test_prompt_templates.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/plugin_definition/test_sk_function_decorators.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/plugin_definition/test_sk_function_decorators.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/template_engine/blocks/test_block.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/template_engine/blocks/test_block.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/template_engine/blocks/test_code_block.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/template_engine/blocks/test_code_block.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/template_engine/blocks/test_function_id_block.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/template_engine/blocks/test_function_id_block.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/template_engine/blocks/test_text_block.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/template_engine/blocks/test_text_block.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/template_engine/blocks/test_val_block.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/template_engine/blocks/test_val_block.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/template_engine/blocks/test_var_block.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/template_engine/blocks/test_var_block.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/template_engine/test_code_tokenizer.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/template_engine/test_code_tokenizer.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/template_engine/test_prompt_template_engine.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/template_engine/test_prompt_template_engine.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/template_engine/test_template_tokenizer.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/template_engine/test_template_tokenizer.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/test_kernel.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/test_kernel.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/test_serialization.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/test_serialization.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/text/test_function_extension.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/text/test_function_extension.py`

 * *Files identical despite different names*

### Comparing `flexible_semantic_kernel-1.0.2.dev0/tests/unit/text/test_text_chunker.py` & `flexible_semantic_kernel-1.0.3.dev0/tests/unit/text/test_text_chunker.py`

 * *Files identical despite different names*

