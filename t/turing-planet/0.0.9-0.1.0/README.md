# Comparing `tmp/turing-planet-0.0.9.tar.gz` & `tmp/turing-planet-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turing-planet-0.0.9.tar", last modified: Tue Apr 23 07:13:43 2024, max compression
+gzip compressed data, was "turing-planet-0.1.0.tar", last modified: Thu Apr 25 12:08:21 2024, max compression
```

## Comparing `turing-planet-0.0.9.tar` & `turing-planet-0.1.0.tar`

### file list

```diff
@@ -1,126 +1,127 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 07:13:43.854124 turing-planet-0.0.9/
--rw-rw-rw-   0        0        0     2850 2024-04-23 07:13:43.853127 turing-planet-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-23 07:13:43.855121 turing-planet-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      893 2024-04-23 07:13:31.000000 turing-planet-0.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 07:13:43.634708 turing-planet-0.0.9/test/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:36.000000 turing-planet-0.0.9/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 07:13:43.638698 turing-planet-0.0.9/test/api/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:36.000000 turing-planet-0.0.9/test/api/__init__.py
--rw-rw-rw-   0        0        0     2914 2024-04-18 03:49:36.000000 turing-planet-0.0.9/test/api/sample_spark_chat_client.py
--rw-rw-rw-   0        0        0     6166 2024-04-18 03:49:36.000000 turing-planet-0.0.9/test/api/sample_spark_embedding.py
-drwxrwxrwx   0        0        0        0 2024-04-23 07:13:43.655653 turing-planet-0.0.9/test/langchain/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:36.000000 turing-planet-0.0.9/test/langchain/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 07:13:43.676597 turing-planet-0.0.9/test/langchain/agents/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:36.000000 turing-planet-0.0.9/test/langchain/agents/__init__.py
--rw-rw-rw-   0        0        0     1722 2024-04-18 03:49:36.000000 turing-planet-0.0.9/test/langchain/agents/agent_qa.py
--rw-rw-rw-   0        0        0     1842 2024-04-18 03:49:36.000000 turing-planet-0.0.9/test/langchain/agents/ask.py
--rw-rw-rw-   0        0        0     2006 2024-04-18 03:49:36.000000 turing-planet-0.0.9/test/langchain/agents/ask2.py
--rw-rw-rw-   0        0        0     3471 2024-04-18 03:49:36.000000 turing-planet-0.0.9/test/langchain/agents/plan.py
--rw-rw-rw-   0        0        0     1178 2024-04-18 03:49:36.000000 turing-planet-0.0.9/test/langchain/agents/quick_start.py
--rw-rw-rw-   0        0        0     4196 2024-04-18 03:49:36.000000 turing-planet-0.0.9/test/langchain/agents/react.py
--rw-rw-rw-   0        0        0     2021 2024-04-18 03:49:36.000000 turing-planet-0.0.9/test/langchain/agents/slot.py
--rw-rw-rw-   0        0        0     2335 2024-04-18 03:49:36.000000 turing-planet-0.0.9/test/langchain/agents/slot2.py
--rw-rw-rw-   0        0        0     8842 2024-04-18 03:49:36.000000 turing-planet-0.0.9/test/langchain/agents/sparkai_agent.py
--rw-rw-rw-   0        0        0     2223 2024-04-18 03:49:36.000000 turing-planet-0.0.9/test/langchain/agents/tools.py
--rw-rw-rw-   0        0        0     2822 2024-04-18 03:49:36.000000 turing-planet-0.0.9/test/langchain/agents.py
--rw-rw-rw-   0        0        0     3405 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/langchain/chat_model.py
--rw-rw-rw-   0        0        0     2771 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/langchain/embed.py
--rw-rw-rw-   0        0        0     4898 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/langchain/function_call.py
--rw-rw-rw-   0        0        0     2554 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/langchain/function_call_aiui.py
--rw-rw-rw-   0        0        0     2332 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/langchain/llm.py
--rw-rw-rw-   0        0        0     3279 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/langchain/memory.py
--rw-rw-rw-   0        0        0     4790 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/langchain/retrieval.py
-drwxrwxrwx   0        0        0        0 2024-04-23 07:13:43.687568 turing-planet-0.0.9/test/llama_index/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/__init__.py
--rw-rw-rw-   0        0        0      148 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/base.py
--rw-rw-rw-   0        0        0     4881 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/indexing.py
-drwxrwxrwx   0        0        0        0 2024-04-23 07:13:43.719483 turing-planet-0.0.9/test/llama_index/introduce/
--rw-rw-rw-   0        0        0     1137 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/introduce/01_start.py
--rw-rw-rw-   0        0        0     1425 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/introduce/02_reader.py
--rw-rw-rw-   0        0        0     1059 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/introduce/03_custom_file_reader.py
--rw-rw-rw-   0        0        0      915 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/introduce/04_doc_metadata.py
--rw-rw-rw-   0        0        0     1831 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/introduce/05_splitter.py
--rw-rw-rw-   0        0        0     3489 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/introduce/06_node_metadata.py
--rw-rw-rw-   0        0        0     1526 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/introduce/07_retriever.py
--rw-rw-rw-   0        0        0     4161 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/introduce/07_retriever_custom.py
--rw-rw-rw-   0        0        0     1951 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/introduce/08_postprocessor.py
--rw-rw-rw-   0        0        0      907 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/introduce/09_prompt.py
--rw-rw-rw-   0        0        0     1750 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/introduce/10_multistep_query_engine.py
--rw-rw-rw-   0        0        0     3578 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/introduce/11_route_query_engine.py
--rw-rw-rw-   0        0        0      716 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/introduce/12_llamahub.py
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/introduce/__init__.py
--rw-rw-rw-   0        0        0     1697 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/introduce/introduce_base.py
--rw-rw-rw-   0        0        0      487 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/introduce/nltk_demo.py
--rw-rw-rw-   0        0        0     5620 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/metadata.py
-drwxrwxrwx   0        0        0        0 2024-04-23 07:13:43.746410 turing-planet-0.0.9/test/llama_index/optimizing/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/optimizing/__init__.py
--rw-rw-rw-   0        0        0     8043 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/optimizing/base.py
--rw-rw-rw-   0        0        0     3303 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/optimizing/custom_keyword_extractor.py
--rw-rw-rw-   0        0        0     4712 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/optimizing/docx_keyword_vector.py
--rw-rw-rw-   0        0        0       27 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/optimizing/kg_index.py
--rw-rw-rw-   0        0        0     7157 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/optimizing/qa_metadata.py
--rw-rw-rw-   0        0        0     4300 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/optimizing/summary_index.py
--rw-rw-rw-   0        0        0      366 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/optimizing/summary_metadata.py
--rw-rw-rw-   0        0        0     4361 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/optimizing/turing_knowledge.py
--rw-rw-rw-   0        0        0    12176 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/optimizing/vector_index.py
--rw-rw-rw-   0        0        0     9280 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/optimizing/vector_index_cq.py
-drwxrwxrwx   0        0        0        0 2024-04-23 07:13:43.768351 turing-planet-0.0.9/test/llama_index/pk/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/pk/__init__.py
--rw-rw-rw-   0        0        0     3390 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/pk/llama_index_spark-0131.py
--rw-rw-rw-   0        0        0     5812 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/pk/pk.py
--rw-rw-rw-   0        0        0     5869 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/pk/pk_excel_chunsize.py
--rw-rw-rw-   0        0        0     6154 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/pk/pk_excel_chunsize_rerank.py
--rw-rw-rw-   0        0        0     5852 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/pk/pk_excel_embedding.py
--rw-rw-rw-   0        0        0     6736 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/pk/pk_word_0201.py
--rw-rw-rw-   0        0        0     9096 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/pk/pk_word_es_0201.py
--rw-rw-rw-   0        0        0     4089 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/pk/sample_excel.py
--rw-rw-rw-   0        0        0     3719 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/skydoc-embedding.py
--rw-rw-rw-   0        0        0     5093 2024-04-18 03:49:37.000000 turing-planet-0.0.9/test/llama_index/start.py
-drwxrwxrwx   0        0        0        0 2024-04-23 07:13:43.771345 turing-planet-0.0.9/turing_planet/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.0.9/turing_planet/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 07:13:43.789330 turing-planet-0.0.9/turing_planet/api/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.0.9/turing_planet/api/__init__.py
--rw-rw-rw-   0        0        0     2478 2024-04-18 03:49:37.000000 turing-planet-0.0.9/turing_planet/api/planet_embedding_client.py
--rw-rw-rw-   0        0        0     4873 2024-04-18 03:49:37.000000 turing-planet-0.0.9/turing_planet/api/planet_vector_client.py
--rw-rw-rw-   0        0        0     8107 2024-04-18 03:49:37.000000 turing-planet-0.0.9/turing_planet/api/spark_chat_client.py
-drwxrwxrwx   0        0        0        0 2024-04-23 07:13:43.794283 turing-planet-0.0.9/turing_planet/deprecated/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.0.9/turing_planet/deprecated/__init__.py
--rw-rw-rw-   0        0        0     6952 2024-04-18 03:49:37.000000 turing-planet-0.0.9/turing_planet/deprecated/spark_embedding_client.py
-drwxrwxrwx   0        0        0        0 2024-04-23 07:13:43.796278 turing-planet-0.0.9/turing_planet/langchain/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.0.9/turing_planet/langchain/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 07:13:43.800266 turing-planet-0.0.9/turing_planet/langchain/chat_models/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.0.9/turing_planet/langchain/chat_models/__init__.py
--rw-rw-rw-   0        0        0     8133 2024-04-18 03:49:37.000000 turing-planet-0.0.9/turing_planet/langchain/chat_models/sparkai.py
-drwxrwxrwx   0        0        0        0 2024-04-23 07:13:43.804289 turing-planet-0.0.9/turing_planet/langchain/embeddings/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.0.9/turing_planet/langchain/embeddings/__init__.py
--rw-rw-rw-   0        0        0      765 2024-04-18 03:49:37.000000 turing-planet-0.0.9/turing_planet/langchain/embeddings/sparkai.py
-drwxrwxrwx   0        0        0        0 2024-04-23 07:13:43.808244 turing-planet-0.0.9/turing_planet/langchain/llm/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.0.9/turing_planet/langchain/llm/__init__.py
--rw-rw-rw-   0        0        0     5350 2024-04-18 03:49:37.000000 turing-planet-0.0.9/turing_planet/langchain/llm/sparkai.py
-drwxrwxrwx   0        0        0        0 2024-04-23 07:13:43.811239 turing-planet-0.0.9/turing_planet/llama_index/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.0.9/turing_planet/llama_index/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 07:13:43.816225 turing-planet-0.0.9/turing_planet/llama_index/embeddings/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.0.9/turing_planet/llama_index/embeddings/__init__.py
--rw-rw-rw-   0        0        0     1582 2024-04-18 03:49:37.000000 turing-planet-0.0.9/turing_planet/llama_index/embeddings/sparkai.py
-drwxrwxrwx   0        0        0        0 2024-04-23 07:13:43.821211 turing-planet-0.0.9/turing_planet/llama_index/llms/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.0.9/turing_planet/llama_index/llms/__init__.py
--rw-rw-rw-   0        0        0     3083 2024-04-18 03:49:37.000000 turing-planet-0.0.9/turing_planet/llama_index/llms/sparkai.py
-drwxrwxrwx   0        0        0        0 2024-04-23 07:13:43.824202 turing-planet-0.0.9/turing_planet/llama_index/readers/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.0.9/turing_planet/llama_index/readers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 07:13:43.833179 turing-planet-0.0.9/turing_planet/llama_index/readers/file/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.0.9/turing_planet/llama_index/readers/file/__init__.py
--rw-rw-rw-   0        0        0     1695 2024-04-18 03:49:37.000000 turing-planet-0.0.9/turing_planet/llama_index/readers/file/excel.py
--rw-rw-rw-   0        0        0     1201 2024-04-18 03:49:37.000000 turing-planet-0.0.9/turing_planet/llama_index/readers/file/turing_markdown_reader.py
-drwxrwxrwx   0        0        0        0 2024-04-23 07:13:43.839162 turing-planet-0.0.9/turing_planet/llama_index/vector_stores/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.0.9/turing_planet/llama_index/vector_stores/__init__.py
--rw-rw-rw-   0        0        0     3300 2024-04-18 03:49:37.000000 turing-planet-0.0.9/turing_planet/llama_index/vector_stores/planet.py
-drwxrwxrwx   0        0        0        0 2024-04-23 07:13:43.848140 turing-planet-0.0.9/turing_planet/utils/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.0.9/turing_planet/utils/__init__.py
--rw-rw-rw-   0        0        0     2102 2024-04-18 03:49:37.000000 turing-planet-0.0.9/turing_planet/utils/auth_util.py
--rw-rw-rw-   0        0        0     1009 2024-04-18 03:49:37.000000 turing-planet-0.0.9/turing_planet/utils/env.py
-drwxrwxrwx   0        0        0        0 2024-04-23 07:13:43.851130 turing-planet-0.0.9/turing_planet.egg-info/
--rw-rw-rw-   0        0        0     2850 2024-04-23 07:13:43.000000 turing-planet-0.0.9/turing_planet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3843 2024-04-23 07:13:43.000000 turing-planet-0.0.9/turing_planet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 07:13:43.000000 turing-planet-0.0.9/turing_planet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-04-23 07:13:43.000000 turing-planet-0.0.9/turing_planet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-23 07:13:43.000000 turing-planet-0.0.9/turing_planet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 12:08:21.127676 turing-planet-0.1.0/
+-rw-rw-rw-   0        0        0     2581 2024-04-25 12:08:21.125681 turing-planet-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-25 12:08:21.127676 turing-planet-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      893 2024-04-25 12:06:55.000000 turing-planet-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:08:20.890740 turing-planet-0.1.0/test/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:36.000000 turing-planet-0.1.0/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:08:20.895760 turing-planet-0.1.0/test/api/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:36.000000 turing-planet-0.1.0/test/api/__init__.py
+-rw-rw-rw-   0        0        0     2914 2024-04-18 03:49:36.000000 turing-planet-0.1.0/test/api/sample_spark_chat_client.py
+-rw-rw-rw-   0        0        0     6166 2024-04-18 03:49:36.000000 turing-planet-0.1.0/test/api/sample_spark_embedding.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:08:20.914676 turing-planet-0.1.0/test/langchain/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:36.000000 turing-planet-0.1.0/test/langchain/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:08:20.933624 turing-planet-0.1.0/test/langchain/agents/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:36.000000 turing-planet-0.1.0/test/langchain/agents/__init__.py
+-rw-rw-rw-   0        0        0     1722 2024-04-18 03:49:36.000000 turing-planet-0.1.0/test/langchain/agents/agent_qa.py
+-rw-rw-rw-   0        0        0     1842 2024-04-18 03:49:36.000000 turing-planet-0.1.0/test/langchain/agents/ask.py
+-rw-rw-rw-   0        0        0     2006 2024-04-18 03:49:36.000000 turing-planet-0.1.0/test/langchain/agents/ask2.py
+-rw-rw-rw-   0        0        0     3471 2024-04-18 03:49:36.000000 turing-planet-0.1.0/test/langchain/agents/plan.py
+-rw-rw-rw-   0        0        0     1178 2024-04-18 03:49:36.000000 turing-planet-0.1.0/test/langchain/agents/quick_start.py
+-rw-rw-rw-   0        0        0     4196 2024-04-18 03:49:36.000000 turing-planet-0.1.0/test/langchain/agents/react.py
+-rw-rw-rw-   0        0        0     2021 2024-04-18 03:49:36.000000 turing-planet-0.1.0/test/langchain/agents/slot.py
+-rw-rw-rw-   0        0        0     2335 2024-04-18 03:49:36.000000 turing-planet-0.1.0/test/langchain/agents/slot2.py
+-rw-rw-rw-   0        0        0     8842 2024-04-18 03:49:36.000000 turing-planet-0.1.0/test/langchain/agents/sparkai_agent.py
+-rw-rw-rw-   0        0        0     2223 2024-04-18 03:49:36.000000 turing-planet-0.1.0/test/langchain/agents/tools.py
+-rw-rw-rw-   0        0        0     2822 2024-04-18 03:49:36.000000 turing-planet-0.1.0/test/langchain/agents.py
+-rw-rw-rw-   0        0        0     3405 2024-04-25 12:06:55.000000 turing-planet-0.1.0/test/langchain/chat_model.py
+-rw-rw-rw-   0        0        0     2987 2024-04-25 12:06:55.000000 turing-planet-0.1.0/test/langchain/embed.py
+-rw-rw-rw-   0        0        0     4898 2024-04-18 03:49:37.000000 turing-planet-0.1.0/test/langchain/function_call.py
+-rw-rw-rw-   0        0        0     2554 2024-04-18 03:49:37.000000 turing-planet-0.1.0/test/langchain/function_call_aiui.py
+-rw-rw-rw-   0        0        0     2332 2024-04-18 03:49:37.000000 turing-planet-0.1.0/test/langchain/llm.py
+-rw-rw-rw-   0        0        0     3279 2024-04-25 12:06:55.000000 turing-planet-0.1.0/test/langchain/memory.py
+-rw-rw-rw-   0        0        0     4790 2024-04-18 03:49:37.000000 turing-planet-0.1.0/test/langchain/retrieval.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:08:20.944595 turing-planet-0.1.0/test/llama_index/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.0/test/llama_index/__init__.py
+-rw-rw-rw-   0        0        0      148 2024-04-18 03:49:37.000000 turing-planet-0.1.0/test/llama_index/base.py
+-rw-rw-rw-   0        0        0     4960 2024-04-25 12:06:55.000000 turing-planet-0.1.0/test/llama_index/indexing.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:08:20.974522 turing-planet-0.1.0/test/llama_index/introduce/
+-rw-rw-rw-   0        0        0     1282 2024-04-25 12:06:55.000000 turing-planet-0.1.0/test/llama_index/introduce/01_start.py
+-rw-rw-rw-   0        0        0     1154 2024-04-25 12:06:55.000000 turing-planet-0.1.0/test/llama_index/introduce/02_reader.py
+-rw-rw-rw-   0        0        0     1064 2024-04-25 12:06:55.000000 turing-planet-0.1.0/test/llama_index/introduce/03_custom_file_reader.py
+-rw-rw-rw-   0        0        0      920 2024-04-25 12:06:55.000000 turing-planet-0.1.0/test/llama_index/introduce/04_doc_metadata.py
+-rw-rw-rw-   0        0        0     1716 2024-04-25 12:06:55.000000 turing-planet-0.1.0/test/llama_index/introduce/05_splitter.py
+-rw-rw-rw-   0        0        0     3275 2024-04-25 12:06:55.000000 turing-planet-0.1.0/test/llama_index/introduce/06_node_metadata.py
+-rw-rw-rw-   0        0        0     1296 2024-04-25 12:06:55.000000 turing-planet-0.1.0/test/llama_index/introduce/07_retriever.py
+-rw-rw-rw-   0        0        0     4030 2024-04-25 12:06:55.000000 turing-planet-0.1.0/test/llama_index/introduce/07_retriever_custom.py
+-rw-rw-rw-   0        0        0     1891 2024-04-25 12:06:55.000000 turing-planet-0.1.0/test/llama_index/introduce/08_postprocessor.py
+-rw-rw-rw-   0        0        0      791 2024-04-25 12:06:55.000000 turing-planet-0.1.0/test/llama_index/introduce/09_prompt.py
+-rw-rw-rw-   0        0        0     1441 2024-04-25 12:06:55.000000 turing-planet-0.1.0/test/llama_index/introduce/10_multistep_query_engine.py
+-rw-rw-rw-   0        0        0     3375 2024-04-25 12:06:55.000000 turing-planet-0.1.0/test/llama_index/introduce/11_route_query_engine.py
+-rw-rw-rw-   0        0        0      716 2024-04-18 03:49:37.000000 turing-planet-0.1.0/test/llama_index/introduce/12_llamahub.py
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.0/test/llama_index/introduce/__init__.py
+-rw-rw-rw-   0        0        0     2423 2024-04-25 12:06:55.000000 turing-planet-0.1.0/test/llama_index/introduce/introduce_base.py
+-rw-rw-rw-   0        0        0      497 2024-04-25 12:06:55.000000 turing-planet-0.1.0/test/llama_index/introduce/nltk_demo.py
+-rw-rw-rw-   0        0        0     5622 2024-04-25 12:06:55.000000 turing-planet-0.1.0/test/llama_index/metadata.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:08:21.000448 turing-planet-0.1.0/test/llama_index/optimizing/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.0/test/llama_index/optimizing/__init__.py
+-rw-rw-rw-   0        0        0     8086 2024-04-25 12:06:55.000000 turing-planet-0.1.0/test/llama_index/optimizing/base.py
+-rw-rw-rw-   0        0        0     3311 2024-04-25 12:06:55.000000 turing-planet-0.1.0/test/llama_index/optimizing/custom_keyword_extractor.py
+-rw-rw-rw-   0        0        0     4533 2024-04-25 12:06:55.000000 turing-planet-0.1.0/test/llama_index/optimizing/docx_keyword_vector.py
+-rw-rw-rw-   0        0        0       27 2024-04-18 03:49:37.000000 turing-planet-0.1.0/test/llama_index/optimizing/kg_index.py
+-rw-rw-rw-   0        0        0     7180 2024-04-25 12:06:55.000000 turing-planet-0.1.0/test/llama_index/optimizing/qa_metadata.py
+-rw-rw-rw-   0        0        0     4294 2024-04-25 12:06:55.000000 turing-planet-0.1.0/test/llama_index/optimizing/summary_index.py
+-rw-rw-rw-   0        0        0      301 2024-04-25 12:06:55.000000 turing-planet-0.1.0/test/llama_index/optimizing/summary_metadata.py
+-rw-rw-rw-   0        0        0     4301 2024-04-25 12:06:55.000000 turing-planet-0.1.0/test/llama_index/optimizing/turing_knowledge.py
+-rw-rw-rw-   0        0        0    12176 2024-04-18 03:49:37.000000 turing-planet-0.1.0/test/llama_index/optimizing/vector_index.py
+-rw-rw-rw-   0        0        0     8677 2024-04-25 12:06:55.000000 turing-planet-0.1.0/test/llama_index/optimizing/vector_index_cq.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:08:21.031366 turing-planet-0.1.0/test/llama_index/pk/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.0/test/llama_index/pk/__init__.py
+-rw-rw-rw-   0        0        0     1615 2024-04-25 12:06:55.000000 turing-planet-0.1.0/test/llama_index/pk/base.py
+-rw-rw-rw-   0        0        0     3819 2024-04-25 12:06:55.000000 turing-planet-0.1.0/test/llama_index/pk/llama_index_spark-0131.py
+-rw-rw-rw-   0        0        0     5240 2024-04-25 12:06:55.000000 turing-planet-0.1.0/test/llama_index/pk/pk.py
+-rw-rw-rw-   0        0        0     5585 2024-04-25 12:06:55.000000 turing-planet-0.1.0/test/llama_index/pk/pk_excel_chunsize.py
+-rw-rw-rw-   0        0        0     5904 2024-04-25 12:06:55.000000 turing-planet-0.1.0/test/llama_index/pk/pk_excel_chunsize_rerank.py
+-rw-rw-rw-   0        0        0     5320 2024-04-25 12:06:55.000000 turing-planet-0.1.0/test/llama_index/pk/pk_excel_embedding.py
+-rw-rw-rw-   0        0        0     6263 2024-04-25 12:06:55.000000 turing-planet-0.1.0/test/llama_index/pk/pk_word_0201.py
+-rw-rw-rw-   0        0        0     8691 2024-04-25 12:06:55.000000 turing-planet-0.1.0/test/llama_index/pk/pk_word_es_0201.py
+-rw-rw-rw-   0        0        0     3881 2024-04-25 12:06:55.000000 turing-planet-0.1.0/test/llama_index/pk/sample_excel.py
+-rw-rw-rw-   0        0        0     3730 2024-04-25 12:06:55.000000 turing-planet-0.1.0/test/llama_index/skydoc-embedding.py
+-rw-rw-rw-   0        0        0     5113 2024-04-25 12:06:55.000000 turing-planet-0.1.0/test/llama_index/start.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:08:21.034387 turing-planet-0.1.0/turing_planet/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.0/turing_planet/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:08:21.058876 turing-planet-0.1.0/turing_planet/api/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.0/turing_planet/api/__init__.py
+-rw-rw-rw-   0        0        0     2478 2024-04-18 03:49:37.000000 turing-planet-0.1.0/turing_planet/api/planet_embedding_client.py
+-rw-rw-rw-   0        0        0     4873 2024-04-18 03:49:37.000000 turing-planet-0.1.0/turing_planet/api/planet_vector_client.py
+-rw-rw-rw-   0        0        0     8107 2024-04-18 03:49:37.000000 turing-planet-0.1.0/turing_planet/api/spark_chat_client.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:08:21.064844 turing-planet-0.1.0/turing_planet/deprecated/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.0/turing_planet/deprecated/__init__.py
+-rw-rw-rw-   0        0        0     6952 2024-04-18 03:49:37.000000 turing-planet-0.1.0/turing_planet/deprecated/spark_embedding_client.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:08:21.066839 turing-planet-0.1.0/turing_planet/langchain/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.0/turing_planet/langchain/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:08:21.071825 turing-planet-0.1.0/turing_planet/langchain/chat_models/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.0/turing_planet/langchain/chat_models/__init__.py
+-rw-rw-rw-   0        0        0     8131 2024-04-25 12:06:55.000000 turing-planet-0.1.0/turing_planet/langchain/chat_models/sparkai.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:08:21.078807 turing-planet-0.1.0/turing_planet/langchain/embeddings/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.0/turing_planet/langchain/embeddings/__init__.py
+-rw-rw-rw-   0        0        0      765 2024-04-18 03:49:37.000000 turing-planet-0.1.0/turing_planet/langchain/embeddings/sparkai.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:08:21.083824 turing-planet-0.1.0/turing_planet/langchain/llm/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.0/turing_planet/langchain/llm/__init__.py
+-rw-rw-rw-   0        0        0     5350 2024-04-18 03:49:37.000000 turing-planet-0.1.0/turing_planet/langchain/llm/sparkai.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:08:21.086791 turing-planet-0.1.0/turing_planet/llama_index/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.0/turing_planet/llama_index/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:08:21.091810 turing-planet-0.1.0/turing_planet/llama_index/embeddings/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.0/turing_planet/llama_index/embeddings/__init__.py
+-rw-rw-rw-   0        0        0     1592 2024-04-25 12:06:55.000000 turing-planet-0.1.0/turing_planet/llama_index/embeddings/sparkai.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:08:21.095764 turing-planet-0.1.0/turing_planet/llama_index/llms/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.0/turing_planet/llama_index/llms/__init__.py
+-rw-rw-rw-   0        0        0     3143 2024-04-25 12:06:55.000000 turing-planet-0.1.0/turing_planet/llama_index/llms/sparkai.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:08:21.098757 turing-planet-0.1.0/turing_planet/llama_index/readers/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.0/turing_planet/llama_index/readers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:08:21.106732 turing-planet-0.1.0/turing_planet/llama_index/readers/file/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.0/turing_planet/llama_index/readers/file/__init__.py
+-rw-rw-rw-   0        0        0     1705 2024-04-25 12:06:55.000000 turing-planet-0.1.0/turing_planet/llama_index/readers/file/excel.py
+-rw-rw-rw-   0        0        0     1190 2024-04-25 12:06:55.000000 turing-planet-0.1.0/turing_planet/llama_index/readers/file/turing_markdown_reader.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:08:21.112716 turing-planet-0.1.0/turing_planet/llama_index/vector_stores/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.0/turing_planet/llama_index/vector_stores/__init__.py
+-rw-rw-rw-   0        0        0     3320 2024-04-25 12:06:55.000000 turing-planet-0.1.0/turing_planet/llama_index/vector_stores/planet.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:08:21.120695 turing-planet-0.1.0/turing_planet/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.0/turing_planet/utils/__init__.py
+-rw-rw-rw-   0        0        0     2102 2024-04-18 03:49:37.000000 turing-planet-0.1.0/turing_planet/utils/auth_util.py
+-rw-rw-rw-   0        0        0     1009 2024-04-18 03:49:37.000000 turing-planet-0.1.0/turing_planet/utils/env.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:08:21.124688 turing-planet-0.1.0/turing_planet.egg-info/
+-rw-rw-rw-   0        0        0     2581 2024-04-25 12:08:20.000000 turing-planet-0.1.0/turing_planet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3871 2024-04-25 12:08:20.000000 turing-planet-0.1.0/turing_planet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 12:08:20.000000 turing-planet-0.1.0/turing_planet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-04-25 12:08:20.000000 turing-planet-0.1.0/turing_planet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-25 12:08:20.000000 turing-planet-0.1.0/turing_planet.egg-info/top_level.txt
```

### Comparing `turing-planet-0.0.9/PKG-INFO` & `turing-planet-0.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: turing-planet
-Version: 0.0.9
+Version: 0.1.0
 Summary: Python Extension Framework For Turing Planet
 Home-page: https://code.iflytek.com/osc/_source/Y_RDG-TURING/gpt/turing-planet/-/tree/heads%2Fdevelop
 Author: jianwu6
 Author-email: jianwu6@iflytek.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9.0, <3.10.0
 Description-Content-Type: text/markdown
 Requires-Dist: langchain==0.0.340
-Requires-Dist: llama-index==0.9.13
+Requires-Dist: llama-index==0.10.0
 Requires-Dist: websocket-client==1.6.4
 
 # turing-planet星球扩展组件
-+ _版本v0.0.4_
++ _版本v0.0.10_
 
 此模块是星球服务的python扩展组件程序，实现`langchain`和`llamaIndex`的大模型和向量提取接口。
 安装本组件后，用户可以按照`langchain`和`llamaIndex`的api调用星球API服务，完成注入会话，文档问答等功能
 
 ## 主要模块
 - turing_planet.langchain
 
@@ -27,20 +27,21 @@
 
 - turing_planet.llama_index
 
 llama_index 模块扩展，集成方式参照`llamaIndex-说明文档`
 
 ## 环境准备
 
-- 本机安装python3，要求最低3.9+
-- 部署好星球API服务, 版本要求1.2.0_build1026+
-- 安装本类库
+- 本机安装python3，要求3.9
+- 部署好星球服务, 版本要求1.2.0_build1026+
 
 ```shell
-pip install --index-url https://depend.iflytek.com/api/pypi/pypi-repo/simple --extra-index-url https://depend.iflytek.com/api/pypi/hy-pypi-private/simple turing-planet
+pip install turing-planet
+# 如果通过清华镜像无法拉取，尝试以下命令
+pip install turing-planet --index-url https://pypi.org/simple
 ```
 
 
 
 ## 快速开始
 安装`turing-planet`类库后，开始编写你的应用
 
@@ -76,34 +77,23 @@
 
 当然，如果不设置环境变量，也可以通过参数传入。例如
 ```python
 sparkChat = ChatSparkAI(endpoint="127.0.0.1:9980", domain="turing-general")
 ```
 
 **domain说明**
+
     公有云
     xfyun-generalv3.5: V3.5协议
     xfyun-generalv3: V3.0协议
     xfyun-generalv2: V2.0协议
     xfyun-general: V1.5协议
     私有化
     turing-general：通用版本
     turing-iflycode.ge: 私有化代码大模型
     AIUI
     aiui-rewrite-v1: 改写
     aiui-slot-v1: 抽槽
 
 
-## 附录
-
- - 打包
 
-```shell
-python3 setup.py sdist bdist_wheel
-```
 
-- 上传 
-域账号 & 依赖库的密码
-
-```shell
-twine upload --repository-url https://depend.iflytek.com/api/pypi/hy-pypi-private dist/*
-```
```

### Comparing `turing-planet-0.0.9/setup.py` & `turing-planet-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import setuptools
 
 with open('readme.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="turing-planet",
-    version="0.0.9",
+    version="0.1.0",
     author="jianwu6",
     author_email="jianwu6@iflytek.com",
     description="Python Extension Framework For Turing Planet",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://code.iflytek.com/osc/_source/Y_RDG-TURING/gpt/turing-planet/-/tree/heads%2Fdevelop",
     python_requires=">=3.9.0, <3.10.0",
     packages=setuptools.find_packages(),
     install_requires=[
         'langchain==0.0.340',
-        'llama-index==0.9.13',
+        'llama-index==0.10.0',
         'websocket-client==1.6.4',
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

### Comparing `turing-planet-0.0.9/test/api/sample_spark_chat_client.py` & `turing-planet-0.1.0/test/api/sample_spark_chat_client.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.0.9/test/api/sample_spark_embedding.py` & `turing-planet-0.1.0/test/api/sample_spark_embedding.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.0.9/test/langchain/agents/agent_qa.py` & `turing-planet-0.1.0/test/langchain/agents/agent_qa.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.0.9/test/langchain/agents/ask.py` & `turing-planet-0.1.0/test/langchain/agents/ask.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.0.9/test/langchain/agents/ask2.py` & `turing-planet-0.1.0/test/langchain/agents/ask2.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.0.9/test/langchain/agents/plan.py` & `turing-planet-0.1.0/test/langchain/agents/plan.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.0.9/test/langchain/agents/quick_start.py` & `turing-planet-0.1.0/test/langchain/agents/quick_start.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.0.9/test/langchain/agents/react.py` & `turing-planet-0.1.0/test/langchain/agents/react.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.0.9/test/langchain/agents/slot.py` & `turing-planet-0.1.0/test/langchain/agents/slot.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.0.9/test/langchain/agents/slot2.py` & `turing-planet-0.1.0/test/langchain/agents/slot2.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.0.9/test/langchain/agents/sparkai_agent.py` & `turing-planet-0.1.0/test/langchain/agents/sparkai_agent.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.0.9/test/langchain/agents/tools.py` & `turing-planet-0.1.0/test/langchain/agents/tools.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.0.9/test/langchain/agents.py` & `turing-planet-0.1.0/test/langchain/agents.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.0.9/test/langchain/chat_model.py` & `turing-planet-0.1.0/test/langchain/chat_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,14 +97,14 @@
 
 
 if __name__ == "__main__":
     print("==========sample_llm===========")
     # sample_llm()
 
     # print("==========sample_stream===========")
-    sample_stream()
+    # sample_stream()
 
     # print("==========sample_history===========")
     # sample_history()
 
     # print("==========sample_output_parser===========")
-    # sample_output_parser()
+    sample_output_parser()
```

### Comparing `turing-planet-0.0.9/test/langchain/function_call.py` & `turing-planet-0.1.0/test/langchain/function_call.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.0.9/test/langchain/function_call_aiui.py` & `turing-planet-0.1.0/test/langchain/function_call_aiui.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.0.9/test/langchain/llm.py` & `turing-planet-0.1.0/test/langchain/llm.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.0.9/test/langchain/memory.py` & `turing-planet-0.1.0/test/langchain/memory.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from turing_planet.langchain.chat_models.sparkai import ChatSparkAI
 
 logging.basicConfig(
     level=logging.INFO,
     format="%(asctime)s - %(levelname)s - %(message)s",
 )
 
-chat = ChatSparkAI(endpoint="172.31.101.142:9980")
+chat = ChatSparkAI(endpoint="172.31.164.103:9980")
 
 mongodb_url = "mongodb://root:Mgadmin_1234@172.31.164.103:30006"
 
 session_id = "sid_lc"
 
 def mongodb():
     """Test the memory with a message store."""
```

### Comparing `turing-planet-0.0.9/test/langchain/retrieval.py` & `turing-planet-0.1.0/test/langchain/retrieval.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.0.9/test/llama_index/indexing.py` & `turing-planet-0.1.0/test/llama_index/indexing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 
-from llama_index import StorageContext, SimpleDirectoryReader, VectorStoreIndex, ServiceContext, DocumentSummaryIndex
-from llama_index.storage.docstore import MongoDocumentStore
-from llama_index.storage.index_store import MongoIndexStore
-from llama_index.vector_stores import ElasticsearchStore, RedisVectorStore
+from llama_index.core import StorageContext, SimpleDirectoryReader, VectorStoreIndex, ServiceContext, DocumentSummaryIndex
+from llama_index.storage.docstore.mongodb import MongoDocumentStore
+from llama_index.storage.index_store.mongodb import MongoIndexStore
+from llama_index.vector_stores.elasticsearch import ElasticsearchStore
+from llama_index.vector_stores.redis import RedisVectorStore
 
 from turing_planet.llama_index.embeddings.sparkai import SparkAIEmbedding
 from turing_planet.llama_index.llms.sparkai import SparkAI
 from turing_planet.llama_index.vector_stores.planet import PlanetVectorStore
 
 logging.basicConfig(
     level=logging.DEBUG,  # 设置日志级别为DEBUG，可以根据需要修改
```

### Comparing `turing-planet-0.0.9/test/llama_index/introduce/02_reader.py` & `turing-planet-0.1.0/test/llama_index/introduce/02_reader.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,9 @@
-from llama_index import Document, SimpleDirectoryReader
-from llama_index.ingestion import IngestionPipeline
-from llama_index.readers import SimpleMongoReader
-from llama_index.readers.file.base import DEFAULT_FILE_READER_CLS
-from llama_index.text_splitter import SentenceSplitter
-
-from turing_planet.llama_index.readers.file.turing_markdown_reader import TuringMarkdownReader
+from llama_index.core import SimpleDirectoryReader
+from llama_index.readers.mongodb import SimpleMongoReader
 
 
 def reader():
     simple_reader = SimpleDirectoryReader(
         # 文件目录
         input_dir="/Users/wujian/workspace/code/llm/turing-planet/turing-planet/test/llama_index/data",
         # 是否递归子目录
```

### Comparing `turing-planet-0.0.9/test/llama_index/introduce/03_custom_file_reader.py` & `turing-planet-0.1.0/test/llama_index/introduce/03_custom_file_reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Optional, Dict, List
 from pathlib import Path
-from llama_index.readers.base import BaseReader
-from llama_index.schema import Document
+
 import pandas as pd
+from llama_index.core import Document
+from llama_index.core.readers.base import BaseReader
 
 # 显示全部列
 pd.set_option('display.max_columns', None)
 # 显示全部行
 pd.set_option('display.max_row', None)
 # 设置数据的显示长度（解决自动换行）
 pd.set_option('display.width', None)
```

### Comparing `turing-planet-0.0.9/test/llama_index/introduce/04_doc_metadata.py` & `turing-planet-0.1.0/test/llama_index/introduce/04_doc_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 
 from dotenv import load_dotenv
-from llama_index import SimpleDirectoryReader
+from llama_index.core import SimpleDirectoryReader
 
 from test.llama_index.introduce.introduce_base import vector_filter_key
 
 # 加载环境变量
 load_dotenv()
 logging.basicConfig(
     level=logging.DEBUG,  # 设置日志级别为DEBUG，可以根据需要修改
```

### Comparing `turing-planet-0.0.9/test/llama_index/introduce/05_splitter.py` & `turing-planet-0.1.0/test/llama_index/introduce/05_splitter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,10 @@
-from llama_index import Document, SimpleDirectoryReader
-from llama_index.ingestion import IngestionPipeline
-from llama_index.readers.file.base import DEFAULT_FILE_READER_CLS
-from llama_index.text_splitter import SentenceSplitter
-
-from turing_planet.llama_index.readers.file.turing_markdown_reader import TuringMarkdownReader
+from llama_index.core import Document, SimpleDirectoryReader
+from llama_index.core.ingestion import IngestionPipeline
+from llama_index.core.node_parser import SentenceSplitter
 
 
 # 演示文档加载 切分过程
 def sample_splitter():
     # 按照chunk_size大小切分，chunk_overlap：表示相连两个node重叠部分大小
     node_parser = SentenceSplitter(chunk_size=10, chunk_overlap=3)
     nodes = node_parser.get_nodes_from_documents(
@@ -42,7 +39,9 @@
     nodes = pipeline.run(documents=documents)
     for node in nodes:
         print(node)
 
 
 if __name__ == '__main__':
     sample_splitter()
+    sample_pipeline()
+    sample()
```

### Comparing `turing-planet-0.0.9/test/llama_index/introduce/06_node_metadata.py` & `turing-planet-0.1.0/test/llama_index/introduce/06_node_metadata.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from llama_index import ServiceContext, SimpleDirectoryReader, VectorStoreIndex, Document
-from llama_index.extractors import TitleExtractor, QuestionsAnsweredExtractor
-from llama_index.ingestion import IngestionPipeline
-from llama_index.node_parser import SentenceSplitter
+from llama_index.core import SimpleDirectoryReader, VectorStoreIndex, Document
+from llama_index.core.extractors import TitleExtractor, QuestionsAnsweredExtractor
+from llama_index.core.ingestion import IngestionPipeline
+from llama_index.core.node_parser import SentenceSplitter
 
-from introduce_base import llm, embed_model, storage_context, vector_filter_key
+from introduce_base import storage_context, vector_filter_key
 from test.llama_index.optimizing.custom_keyword_extractor import MyKeywordExtractor
 from turing_planet.llama_index.llms.sparkai import SparkAI
 
 TEXT = """七、资金筹集及拨付
 （一）资金筹集。
 政府购买居家养老服务所需资金由市、区（开发区）财政按1：1比例分担。
 （二）资金拨付。
@@ -15,15 +15,15 @@
 （三）资金结算。
 政府购买居家养老服务资金结算由各区（开发区）财政部门负责。
 八、其他事项
 1．各县（市）政府购买居家养老服务工作，可结合本地实际参照本方案执行；继续优化实施农村低收入老年人养老服务补贴制度。
 2．本方案自印发之日起满30日后施行，有效期5年。《合肥市政府购买居家养老服务实施方案》（合民〔2017〕136号）、《合肥市居家养老服务标准服务流程及服务收费参考意见》（合民〔2014〕105号）同时废止。"""
 
 # 提取每个节点上下文的标题，关联节点数5
-title_extractor = TitleExtractor(nodes=5, llm=llm)
+title_extractor = TitleExtractor(nodes=5)
 
 QA_PROMPT_TEMPLATE = """
 以下是上下文:
 {context_str}
 
 
 根据给定的上下信息，生成此上下文可以回答的{num_questions}个问题。
@@ -32,48 +32,40 @@
 
 def qa_metadata():
     text_splitter = SentenceSplitter(
         chunk_size=4096,
         chunk_overlap=20,
     )
     #  提取每个节点可以回答的2组问题
-    extractor = QuestionsAnsweredExtractor(questions=2, llm=llm, prompt_template=QA_PROMPT_TEMPLATE)
+    extractor = QuestionsAnsweredExtractor(questions=2, prompt_template=QA_PROMPT_TEMPLATE)
     transformations = [text_splitter, extractor]
     pipeline = IngestionPipeline(transformations=transformations)
     documents = [Document(text=TEXT)]
     nodes = pipeline.run(documents=documents)
     print(nodes)
 
 
 # 自动抽取元数据
 def keywords_metadata():
     extractor = MyKeywordExtractor(llm=SparkAI(), keywords=3)
 
-    # 关联上下文
-    kw_service_context = ServiceContext.from_defaults(
-        embed_model=embed_model,
-        llm=llm,
-        transformations=[
-            SentenceSplitter(chunk_size=2048),
-            extractor
-        ],
-    )
-
-    documents = (SimpleDirectoryReader(input_files=[
-        "/Users/wujian/workspace/code/llm/turing-planet/turing-planet/test/llama_index/data/合政〔2022〕176号.docx"])
-                 .load_data(show_progress=True))
+    documents = (SimpleDirectoryReader(input_files=["../data/合政〔2022〕176号.docx"]).load_data(show_progress=True))
 
     # 添加自定义metadata
     for document in documents:
         document.metadata[vector_filter_key] = "hf"
         # 默认添加的元数据会 被llm和embed使用
         document.excluded_llm_metadata_keys = [vector_filter_key]
         document.excluded_embed_metadata_keys = [vector_filter_key]
 
     # 创建索引
     VectorStoreIndex.from_documents(documents=documents,
                                     storage_context=storage_context,
-                                    service_context=kw_service_context)
+                                    transformations=[
+                                        SentenceSplitter(chunk_size=2048),
+                                        extractor
+                                    ], )
 
 
 if __name__ == '__main__':
     keywords_metadata()
+    # qa_metadata()
```

### Comparing `turing-planet-0.0.9/test/llama_index/introduce/07_retriever.py` & `turing-planet-0.1.0/test/llama_index/introduce/07_retriever.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,30 @@
-from llama_index import VectorStoreIndex, get_response_synthesizer
-from llama_index.indices.vector_store import VectorIndexRetriever
-from llama_index.query_engine import RetrieverQueryEngine
-from llama_index.vector_stores import MetadataFilters, MetadataFilter, FilterOperator
+from llama_index.core import VectorStoreIndex, get_response_synthesizer, ServiceContext
+from llama_index.core.indices.vector_store import VectorIndexRetriever
+from llama_index.core.query_engine import RetrieverQueryEngine
+from llama_index.core.vector_stores import MetadataFilters, MetadataFilter, FilterOperator
 
-from introduce_base import llm, redis_store, service_context, vector_filter_key
+from test.llama_index.introduce.introduce_base import redis_store, vector_filter_key
 
 
 def query():
     #  向量检索
-    vector_index = VectorStoreIndex.from_vector_store(vector_store=redis_store,
-                                                      service_context=service_context)
-
-    # vector_retriever = vector_index.as_retriever(similarity_top_k=3)
+    vector_index = VectorStoreIndex.from_vector_store(vector_store=redis_store)
 
     # 设置过滤条件
     filters = MetadataFilters(
         filters=[
-            MetadataFilter(key=vector_filter_key, operator=FilterOperator.EQ, value="hf"),
+            MetadataFilter(key=vector_filter_key, operator=FilterOperator.TEXT_MATCH, value="hf"),
         ]
     )
     vector_retriever = VectorIndexRetriever(index=vector_index, similarity_top_k=3, filters=filters)
 
-    response_synthesizer = get_response_synthesizer(
-        service_context=service_context
-    )
-
-    query_engine = RetrieverQueryEngine(retriever=vector_retriever, response_synthesizer=response_synthesizer)
+    query_engine = RetrieverQueryEngine(retriever=vector_retriever, response_synthesizer=get_response_synthesizer())
 
-    question = "截止2024年1月，合肥市创建国家卫生城市计划实施步骤进展到什么阶段了？ 简单介绍下。"
+    question = "截止2024年1月，合肥市创建国家卫生城市计划实施步骤进展到什么阶段了？"
     response = query_engine.query(question)
     print(f"Q:{question}")
     print("A:" + response.response.replace("<ret>", "\n").replace("<end>", "\n"))
     print("---------------\n")
 
 
 if __name__ == '__main__':
```

### Comparing `turing-planet-0.0.9/test/llama_index/introduce/07_retriever_custom.py` & `turing-planet-0.1.0/test/llama_index/introduce/07_retriever_custom.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,22 +3,23 @@
  1. 用户问题 --> 向量召回TopK=3, --> vector_nodes
  2. 用户问题抽取关键词 和 给定的关键词列表（向量召回，返回的metadata keywords），通过LLM， 判断相似度
  3. 取相似度最高top1，调用 LLM
 
 """
 from typing import List
 
-from llama_index import VectorStoreIndex, get_response_synthesizer, QueryBundle
-from llama_index.core import BaseRetriever
-from llama_index.indices.vector_store import VectorIndexRetriever
-from llama_index.query_engine import RetrieverQueryEngine
-from llama_index.schema import NodeWithScore
+from llama_index.core import QueryBundle, VectorStoreIndex, get_response_synthesizer
+from llama_index.core.base.base_retriever import BaseRetriever
+from llama_index.core.indices.vector_store import VectorIndexRetriever
+from llama_index.core.query_engine import RetrieverQueryEngine
+from llama_index.core.schema import NodeWithScore
+from llama_index.core.settings import Settings
+
+from test.llama_index.introduce.introduce_base import redis_store
 
-from test.llama_index.introduce.introduce_base import redis_store, service_context
-from test.llama_index.optimizing.base import llm
 from turing_planet.llama_index.llms.sparkai import SparkAI
 
 prompt_template = """
   根据用户的关键词，选择出给定的上下文关键词列表中最匹配的关键词，地点名称不作为关键词。
   要求只返回一个序号数字，不知道就返回0
   上下文关键词列表：
   {context_str}
@@ -34,17 +35,16 @@
 上下文：
 {context_str}
 """
 
 
 # 向量检索重排检索器
 class VectorReRankRetriever(BaseRetriever):
-    def __init__(self, vector_retriever: VectorIndexRetriever, llm: SparkAI):
+    def __init__(self, vector_retriever: VectorIndexRetriever, ):
         self._vector_retriever = vector_retriever
-        self._llm = llm
         super().__init__()
 
     def _retrieve(self, query_bundle: QueryBundle) -> List[NodeWithScore]:
         # 1. 向量检索，选取topN重排集合
         vector_nodes = self._vector_retriever.retrieve(query_bundle)
         if len(vector_nodes) <= 1:
             return vector_nodes
@@ -52,20 +52,20 @@
         # 2. 选取待选node的关键词
         keyword_context = ""
         for i, vector_node in enumerate(vector_nodes):
             keyword_context = keyword_context + f"{i} <--> {vector_node.metadata.get('excerpt_keywords')}\n"
 
         # 3. 获取用户问题关键词
         q_keywords_prompt = question_keywords_prompt_template.replace("{context_str}", query_bundle.query_str)
-        question_keywords = llm.complete(q_keywords_prompt).text
+        question_keywords = Settings.llm.complete(q_keywords_prompt).text
         print(f"===提取用户问题关键词\n问题：{q_keywords_prompt}\n用户关键词结果：{question_keywords}")
 
         # 4. 选取和用户关键词最匹配的待选node
         prompt = prompt_template.replace("{context_str}", keyword_context).replace("{keywords}", question_keywords)
-        keyword_index = llm.complete(prompt).text
+        keyword_index = Settings.llm.complete(prompt).text
         print(f"===匹配关键词\n问题：{prompt}\n命中关键词结果：{keyword_index}")
         target_index = 0
         try:
             target_index = int(keyword_index)
         except ValueError:
             print("转换index失败", keyword_index)
         if target_index >= len(vector_nodes):
@@ -74,28 +74,27 @@
 
         retrieve_nodes = [vector_nodes[target_index]]
         return retrieve_nodes
 
 
 def query():
     #  向量检索
-    vector_index = VectorStoreIndex.from_vector_store(vector_store=redis_store,
-                                                      service_context=service_context)
+    #  向量检索
+    vector_index = VectorStoreIndex.from_vector_store(vector_store=redis_store)
     vector_retriever = VectorIndexRetriever(index=vector_index, similarity_top_k=3)
 
     # 向量重排检索
-    rerank_retriever = VectorReRankRetriever(vector_retriever=vector_retriever, llm=llm)
+    rerank_retriever = VectorReRankRetriever(vector_retriever=vector_retriever, )
     response_synthesizer = get_response_synthesizer(
-        service_context=service_context,
         response_mode="refine",
     )
 
     query_engine = RetrieverQueryEngine(retriever=rerank_retriever, response_synthesizer=response_synthesizer)
 
-    question = "截止2024年1月，合肥市创建国家卫生城市计划实施步骤进展到什么阶段了？ 简单介绍下。"
+    question = "截止2024年1月，合肥市创建国家卫生城市计划实施步骤进展到什么阶段了？"
     response = query_engine.query(question + "\n中文回答")
     print(f"Q:{question}")
     print("A:" + response.response.replace("<ret>", "\n").replace("<end>", "\n"))
     print("---------------\n")
 
 
 if __name__ == '__main__':
```

### Comparing `turing-planet-0.0.9/test/llama_index/introduce/08_postprocessor.py` & `turing-planet-0.1.0/test/llama_index/introduce/08_postprocessor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from typing import List, Optional
 
-from llama_index import VectorStoreIndex
-from llama_index.postprocessor import KeywordNodePostprocessor
-from llama_index.postprocessor.types import BaseNodePostprocessor
-from llama_index.schema import NodeWithScore, QueryBundle
-from pydantic import Field
+from llama_index.core import VectorStoreIndex
+from llama_index.core.postprocessor import KeywordNodePostprocessor
+from llama_index.core.postprocessor.types import BaseNodePostprocessor
+from llama_index.core.schema import NodeWithScore, QueryBundle
+
 from pydantic.v1 import PrivateAttr
 
-from test.llama_index.introduce.introduce_base import service_context, redis_store
+from test.llama_index.introduce.introduce_base import redis_store
 
 
 def post_processor():
     keyword_postprocessor = KeywordNodePostprocessor(
         # 包含哪些关键词
         required_keywords=[""],
         # 排除那些关键词
         exclude_keywords=["合肥"],
         lang="zh"
     )
 
-    index = VectorStoreIndex.from_vector_store(vector_store=redis_store, service_context=service_context)
+    index = VectorStoreIndex.from_vector_store(vector_store=redis_store)
 
     query_engine = index.as_query_engine(
         node_postprocessors=[keyword_postprocessor]
     )
 
     response = query_engine.query("截止2024年1月，合肥市创建国家卫生城市计划实施步骤进展到什么阶段了？ ")
     print(response)
@@ -50,13 +50,11 @@
     #     self._combine_retriever = combine_retriever
     #
     # def set_response_synthesizer(self, response_synthesizer):
     #     self._response_synthesizer = response_synthesizer
 
 
 if __name__ == '__main__':
-
     llm_rerank = CustomLLMRerank(top_n=111)
     print(llm_rerank._format_node_batch_fn)
 
-
     # post_processor()
```

### Comparing `turing-planet-0.0.9/test/llama_index/introduce/09_prompt.py` & `turing-planet-0.1.0/test/llama_index/introduce/09_prompt.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-from llama_index import SimpleDirectoryReader, VectorStoreIndex, PromptTemplate
+from llama_index.core import VectorStoreIndex, PromptTemplate
 
-from test.llama_index.introduce.introduce_base import service_context, redis_store
+from test.llama_index.introduce.introduce_base import redis_store
 
 qa_prompt_tmpl_str = """
 下面是上下文信息.
 ---------------------
 {context_str}
 ---------------------
 根据上下文信息和知识回答问题
 问题: {query_str}
 答案:
 """
 
 if __name__ == '__main__':
-    index = VectorStoreIndex.from_vector_store(vector_store=redis_store,
-                                               service_context=service_context)
+    index = VectorStoreIndex.from_vector_store(vector_store=redis_store)
 
     qa_prompt_tmpl = PromptTemplate(qa_prompt_tmpl_str)
     # 创建查询引擎
     query_engine = index.as_query_engine(similarity_top_k=3, text_qa_template=qa_prompt_tmpl)
 
     # 执行查询
     response = query_engine.query("截止2024年1月，合肥市创建国家卫生城市计划实施步骤进展到什么阶段了？")
```

### Comparing `turing-planet-0.0.9/test/llama_index/introduce/10_multistep_query_engine.py` & `turing-planet-0.1.0/test/llama_index/introduce/10_multistep_query_engine.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from llama_index import SimpleDirectoryReader, VectorStoreIndex, get_response_synthesizer, PromptTemplate
-from llama_index.indices.query.query_transform import StepDecomposeQueryTransform
-from llama_index.query_engine import MultiStepQueryEngine
+from llama_index.core import VectorStoreIndex, get_response_synthesizer, PromptTemplate
+from llama_index.core.indices.query.query_transform import StepDecomposeQueryTransform
+from llama_index.core.query_engine import MultiStepQueryEngine
 
-from test.llama_index.introduce.introduce_base import service_context, redis_store
+from test.llama_index.introduce.introduce_base import redis_store
 
 # 多步检索，将一个复杂的问题拆成多个连续的子问题
 prompt = """
 原始的问题如下:{query_str}
 
 请针对这个问题逐步思考，将每一步推理生成一个新问题。如果有上下文信息，还需结合上下文思考
 
@@ -18,23 +18,20 @@
 
 新问题: 
 
 """
 
 if __name__ == '__main__':
     # 加载数据
-    vector_index = VectorStoreIndex.from_vector_store(vector_store=redis_store,
-                                                      service_context=service_context)
+    vector_index = VectorStoreIndex.from_vector_store(vector_store=redis_store)
 
-    transform = StepDecomposeQueryTransform(llm_predictor=service_context.llm_predictor, verbose=True,
-                                            step_decompose_query_prompt=PromptTemplate(prompt)
-                                            )
-    vector_engine = vector_index.as_query_engine(service_context=service_context)
+    transform = StepDecomposeQueryTransform(step_decompose_query_prompt=PromptTemplate(prompt), verbose=True, )
+    vector_engine = vector_index.as_query_engine()
 
     engine = MultiStepQueryEngine(query_engine=vector_engine,
                                   query_transform=transform,
                                   # 拆分两步
                                   num_steps=2,
-                                  response_synthesizer=get_response_synthesizer(service_context=service_context))
+                                  response_synthesizer=get_response_synthesizer())
 
     response = engine.query("截止2024年1月，合肥市创建国家卫生城市计划实施步骤进展到什么阶段了？")
     print(response)
```

### Comparing `turing-planet-0.0.9/test/llama_index/introduce/11_route_query_engine.py` & `turing-planet-0.1.0/test/llama_index/introduce/11_route_query_engine.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from llama_index import SimpleDirectoryReader, VectorStoreIndex, SummaryIndex
-from llama_index.output_parsers import selection
-from llama_index.query_engine import RouterQueryEngine
-from llama_index.selectors import LLMMultiSelector, LLMSingleSelector
-from llama_index.tools import QueryEngineTool
+from llama_index.core import SimpleDirectoryReader, VectorStoreIndex, SummaryIndex
+from llama_index.core.output_parsers import selection
+from llama_index.core.query_engine import RouterQueryEngine
+from llama_index.core.selectors import LLMSingleSelector
+from llama_index.core.tools import QueryEngineTool
 
-from test.llama_index.introduce.introduce_base import service_context, redis_store
+from test.llama_index.introduce.introduce_base import redis_store
 
 # 路由查询引擎
 
 # 默认的prompt 的模版，导致星火大模型返回的json是非法的无法解析
 selection.FORMAT_STR = """The output should be ONLY JSON formatted as a JSON instance.
 
 Here is an example:
@@ -21,18 +21,17 @@
 """
 
 if __name__ == '__main__':
     # load data
     documents = SimpleDirectoryReader("../data").load_data(show_progress=True)
 
     #  define index
-    vector_index = VectorStoreIndex.from_vector_store(vector_store=redis_store,
-                                                      service_context=service_context)
+    vector_index = VectorStoreIndex.from_vector_store(vector_store=redis_store)
 
-    summary_index = SummaryIndex.from_documents(documents=documents, service_context=service_context)
+    summary_index = SummaryIndex.from_documents(documents=documents)
 
     #  define query engine tool
     vector_engine = vector_index.as_query_engine()
     summary_engine = summary_index.as_query_engine()
 
     vector_tool = QueryEngineTool.from_defaults(query_engine=vector_engine,
                                                 description="Useful for retrieving specific context")
@@ -72,16 +71,15 @@
     
     第二部：根据choice选择tool，执行tool
         1) 如果是LLMSingleSelector，选择一个索引查询器完成问答
         2） 如果是 LLMMultiSelector，选择其中多个索引查询器，将检索到的结果合并，再次调用LLM（QA），得到最终结果
     
     """
     query_engine = RouterQueryEngine(
-        selector=LLMSingleSelector.from_defaults(service_context=service_context),
+        selector=LLMSingleSelector.from_defaults(),
         # selector=LLMMultiSelector.from_defaults(service_context=service_context),
         query_engine_tools=[vector_tool, summary_tool],
-        service_context=service_context
     )
 
     #   query
     response = query_engine.query("简要总结下合肥市创建国家卫生城市三年行动计划通知的主要内容？")
     print(response)
```

### Comparing `turing-planet-0.0.9/test/llama_index/introduce/12_llamahub.py` & `turing-planet-0.1.0/test/llama_index/introduce/12_llamahub.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.0.9/test/llama_index/introduce/introduce_base.py` & `turing-planet-0.1.0/test/llama_index/introduce/introduce_base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,61 @@
 import logging
 
 from dotenv import load_dotenv
-from llama_index import StorageContext, ServiceContext
-from llama_index.storage.docstore import MongoDocumentStore
-from llama_index.storage.index_store import MongoIndexStore
-from llama_index.vector_stores import RedisVectorStore
+from llama_index.core import StorageContext
+from llama_index.core.settings import Settings
+from llama_index.storage.docstore.mongodb import MongoDocumentStore
+from llama_index.storage.index_store.mongodb import MongoIndexStore
+from llama_index.vector_stores.redis import RedisVectorStore
+from redis import Redis
+from redisvl.schema import IndexSchema
 
 from turing_planet.llama_index.embeddings.sparkai import SparkAIEmbedding
 from turing_planet.llama_index.llms.sparkai import SparkAI
 
 # 加载环境变量
 load_dotenv()
 logging.basicConfig(
     level=logging.DEBUG,  # 设置日志级别为DEBUG，可以根据需要修改
     format="%(asctime)s - %(levelname)s - %(message)s",
 )
+# 向量特征维度
+dims = 2560
+endpoint = "172.31.164.103:9980"
+Settings.llm = SparkAI(endpoint=endpoint)
+Settings.embed_model = SparkAIEmbedding(endpoint=endpoint, domain="emb_xfyun")
+Settings.chunk_size = 1024
 
+# TODO 额外参数
 vector_filter_key = "location"
 
-redis_store = RedisVectorStore(index_name=f"llamaindex-introduce",
-                               index_prefix=f"llamaindex-introduce_vector",
-                               redis_url="redis://172.31.128.153:6379",
-                               overwrite=True,
-                               metadata_fields=[vector_filter_key])
+redis_index_schema = IndexSchema.from_dict(
+    {
+        # customize basic index specs
+        "index": {
+            "name": "llamaindex-introduce",
+            "prefix": "llamaindex-introduce_vector",
+            "key_separator": ":",
+        },
+        # customize fields that are indexed
+        "fields": [
+            {"name": "id", "type": "tag"},
+            {"name": "doc_id", "type": "tag"},
+            {"name": "text", "type": "text"},
+            {"name": "vector", "type": "vector",
+             "attrs": {"dims": dims, "algorithm": "flat", "distance_metric": "cosine", }},
+            {"name": vector_filter_key, "type": "text"}
+        ],
+    }
+)
+
+redis_client = Redis.from_url("redis://172.31.128.153:6379")
+redis_store = RedisVectorStore(schema=redis_index_schema, redis_client=redis_client, overwrite=False)
 
 mongo_doc_store = MongoDocumentStore.from_uri(uri="mongodb://root:Mgadmin_1234@172.31.164.103:30006",
                                               db_name="llamaindex-introduce")
 
 mongo_index_store = MongoIndexStore.from_uri(uri="mongodb://root:Mgadmin_1234@172.31.164.103:30006",
                                              db_name="llamaindex-introduce")
 
 storage_context = StorageContext.from_defaults(vector_store=redis_store, docstore=mongo_doc_store,
                                                index_store=mongo_index_store)
-
-embed_model = SparkAIEmbedding(domain="emb_v1")
-
-llm = SparkAI()
-
-service_context = ServiceContext.from_defaults(embed_model=embed_model, llm=llm)
```

### Comparing `turing-planet-0.0.9/test/llama_index/metadata.py` & `turing-planet-0.1.0/test/llama_index/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 
 from dotenv import load_dotenv
-from llama_index import ServiceContext, SimpleDirectoryReader, VectorStoreIndex, StorageContext, PromptTemplate, \
+from llama_index.core import ServiceContext, SimpleDirectoryReader, VectorStoreIndex, StorageContext, PromptTemplate, \
     Document
-from llama_index.extractors import TitleExtractor, QuestionsAnsweredExtractor, SummaryExtractor, KeywordExtractor
-from llama_index.ingestion import IngestionPipeline
-from llama_index.node_parser import TokenTextSplitter, SentenceSplitter
+from llama_index.core.extractors import TitleExtractor, QuestionsAnsweredExtractor, SummaryExtractor
+from llama_index.core.ingestion import IngestionPipeline
+from llama_index.core.node_parser import TokenTextSplitter, SentenceSplitter
 
 from test.llama_index.optimizing.custom_keyword_extractor import MyKeywordExtractor
 from turing_planet.llama_index.embeddings.sparkai import SparkAIEmbedding
 from turing_planet.llama_index.llms.sparkai import SparkAI
 from turing_planet.llama_index.vector_stores.planet import PlanetVectorStore
 
 # 加载环境变量
```

### Comparing `turing-planet-0.0.9/test/llama_index/optimizing/base.py` & `turing-planet-0.1.0/test/llama_index/optimizing/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,19 +27,24 @@
 Q: 合肥市既有住宅加装电梯工作基本原则以及实施的条件
 A: 基本原则：既有住宅加装电梯工作坚持“业主自主、社区主导、政府扶持、各方支持”的原则。
 实施条件：（一）具有合法的房屋权属证明；
 （二）5年内未列入棚户区（危旧房）、城中村改造范围和计划；
 （三）已建成投入使用的4层以上（含4层）无电梯住宅；
 （四）满足建筑物结构安全、消防安全等有关规范要求。
 """
+from typing import Optional, List
+
 from dotenv import load_dotenv
-from llama_index import SimpleDirectoryReader, VectorStoreIndex, StorageContext, ServiceContext
-from llama_index.extractors import QuestionsAnsweredExtractor, SummaryExtractor
-from llama_index.node_parser import SentenceSplitter
-from llama_index.vector_stores import RedisVectorStore
+from llama_index.core import SimpleDirectoryReader, VectorStoreIndex, StorageContext, ServiceContext, Settings
+from llama_index.core.extractors import QuestionsAnsweredExtractor, SummaryExtractor
+from llama_index.core.node_parser import SentenceSplitter
+from llama_index.core.schema import TransformComponent
+from llama_index.vector_stores.redis import RedisVectorStore
+from redis import Redis
+from redisvl.schema import IndexSchema
 
 from turing_planet.llama_index.embeddings.sparkai import SparkAIEmbedding
 from turing_planet.llama_index.llms.sparkai import SparkAI
 
 user_questions = ["合肥市政府购买居家养老服务服务对象以及服务标准",
                   "阐述合肥市“菜篮子”市长负责制的指导思想和总体目标。",
                   "合肥市城镇老旧小区改造提升工作实施意见的指导思想和工作目标是什么",
@@ -47,85 +52,80 @@
                   "合肥市火灾事故应急预案专家组的构成以及相应的职责",
                   "火灾分为哪几种情形以及对应的处理单位",
                   "合肥市既有住宅加装电梯工作基本原则以及实施的条件"
                   ]
 
 load_dotenv()
 
-llm = SparkAI()
-embed_model = SparkAIEmbedding(domain="emb_xfyun")
+dims = 2560
+endpoint = "172.31.164.103:9980"
+Settings.llm = SparkAI(endpoint=endpoint)
+Settings.embed_model = SparkAIEmbedding(endpoint=endpoint, domain="emb_xfyun")
+Settings.chunk_size = 1024
+
+splitter = SentenceSplitter(
+    chunk_size=1024,
+    chunk_overlap=20,
+)
+
+summary_prompt_template = """\
+ 这是本节的内容:
+ {context_str}
+
+ 总结本节的主要主题和实体。 \
+
+ 总结: """
+extractor = SummaryExtractor(summaries=["prev", "self"], prompt_template=summary_prompt_template)
 
 
 def load_documents():
     simple_reader = SimpleDirectoryReader(input_dir="../../../doc/合肥市政府公文")
     documents = simple_reader.load_data(show_progress=True)
     return documents
 
 
 def build_vector_store(index_name: str) -> RedisVectorStore:
-    return RedisVectorStore(index_name=index_name, index_prefix="_".join([index_name, "vector"]),
-                            redis_url="redis://172.31.128.153:6379", overwrite=True)
-
-
-def build_service_context(chunk_size: int = 2048):
-    return ServiceContext.from_defaults(embed_model=embed_model, llm=llm, chunk_size=chunk_size)
-
-
-def build_qa_service_context(questions: int):
-    extractor = QuestionsAnsweredExtractor(questions=questions, llm=llm)
-    return build_extractor_service_context(extractor=extractor)
-
-
-def build_summary_service_context():
-    summary_prompt_template = """\
-    这是本节的内容:
-    {context_str}
-
-    总结本节的主要主题和实体。 \
-
-    总结: """
-
-    extractor = SummaryExtractor(summaries=["prev", "self"], llm=llm, prompt_template=summary_prompt_template)
-    return build_extractor_service_context(extractor=extractor)
-
-
-def build_extractor_service_context(extractor):
-    splitter = SentenceSplitter(
-        chunk_size=4096,
-        chunk_overlap=20,
-    )
-    return ServiceContext.from_defaults(
-        embed_model=embed_model,
-        llm=llm,
-        transformations=[
-            splitter,
-            extractor
-        ]
+    redis_index_schema = IndexSchema.from_dict(
+        {
+            # customize basic index specs
+            "index": {
+                "name": index_name,
+                "prefix": f"{index_name}_vector",
+                "key_separator": ":",
+            },
+            # customize fields that are indexed
+            "fields": [
+                {"name": "id", "type": "tag"},
+                {"name": "doc_id", "type": "tag"},
+                {"name": "text", "type": "text"},
+                {"name": "vector", "type": "vector",
+                 "attrs": {"dims": 2560, "algorithm": "flat", "distance_metric": "cosine", }},
+            ],
+        }
     )
 
+    redis_client = Redis.from_url("redis://172.31.128.153:6379")
+    return RedisVectorStore(schema=redis_index_schema, redis_client=redis_client, overwrite=False)
+
 
 def add_vector_index(index_name: str, chunk_size: int = 2048):
-    add_vector_index(service_context=build_service_context(chunk_size), index_name=index_name)
+    Settings.chunk_size = chunk_size
+    add_vector_index(index_name=index_name)
 
 
-def add_vector_index(service_context, index_name: str):
+def add_vector_index(index_name: str, transformations: Optional[List[TransformComponent]] = None):
     storage_context = StorageContext.from_defaults(vector_store=build_vector_store(index_name))
     VectorStoreIndex.from_documents(documents=load_documents(),
                                     storage_context=storage_context,
-                                    service_context=service_context,
-                                    show_progress=True)
+                                    show_progress=True,
+                                    transformations=transformations)
 
 
-def query(service_context, index_name: str, top_k: int = 1):
-    index = VectorStoreIndex.from_vector_store(vector_store=build_vector_store(index_name),
-                                               service_context=service_context)
+def query(index_name: str, top_k: int = 1):
+    index = VectorStoreIndex.from_vector_store(vector_store=build_vector_store(index_name))
     query_engine = index.as_query_engine(similarity_top_k=top_k)
     for question in user_questions:
         response = query_engine.query(question + "\nResponse in Chinese")
         print(f"Q:{question}")
         print("A:" + response.response.replace("<ret>", "\n").replace("<end>", "\n"))
         # print(f"source:{response.source_nodes[0].text}")
         print("---------------\n")
-
-
-def query(index_name: str, top_k: int = 1):
-    query(service_context=build_service_context(), index_name=index_name, top_k=top_k)
```

### Comparing `turing-planet-0.0.9/test/llama_index/optimizing/custom_keyword_extractor.py` & `turing-planet-0.1.0/test/llama_index/optimizing/custom_keyword_extractor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Any, Dict, List, Optional, Sequence, cast
 
-from llama_index.async_utils import DEFAULT_NUM_WORKERS, run_jobs
-from llama_index.bridge.pydantic import Field
-from llama_index.extractors.interface import BaseExtractor
-from llama_index.llm_predictor.base import LLMPredictor
-from llama_index.llms.base import LLM
-from llama_index.prompts import PromptTemplate
-from llama_index.schema import BaseNode, TextNode
+from llama_index.core import PromptTemplate
+from llama_index.core.async_utils import DEFAULT_NUM_WORKERS, run_jobs
+from llama_index.core.extractors import BaseExtractor
+from llama_index.core.llms import LLM
+from llama_index.core.schema import BaseNode, TextNode
+from llama_index.core.service_context_elements.llm_predictor import LLMPredictor
+from pydantic import Field
 
 DEFAULT_KEYWORD_GEN_TMPL = """
 根据给出的文档内容，提取唯一的标题，最多不超过{keywords}个，每个标题使用空格隔开。
 
 文档内容
 {context_str}
```

### Comparing `turing-planet-0.0.9/test/llama_index/optimizing/docx_keyword_vector.py` & `turing-planet-0.1.0/test/llama_index/optimizing/docx_keyword_vector.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,22 +8,22 @@
  1. 用户问题 --> 向量召回TopK=3, --> vector_nodes
  2. 用户问题抽取关键词 和 给定的关键词列表（向量召回，返回的metadata keywords），通过LLM， 判断相似度
  3. 取相似度最高top1，调用 LLM
 
 """
 from typing import List
 
-from llama_index import VectorStoreIndex, get_response_synthesizer, QueryBundle
-from llama_index.core import BaseRetriever
-from llama_index.indices.vector_store import VectorIndexRetriever
-from llama_index.query_engine import RetrieverQueryEngine
-from llama_index.schema import NodeWithScore
+from llama_index.core import VectorStoreIndex, get_response_synthesizer, QueryBundle, Settings
+from llama_index.core.base.base_retriever import BaseRetriever
+from llama_index.core.indices.vector_store import VectorIndexRetriever
+from llama_index.core.query_engine import RetrieverQueryEngine
+from llama_index.core.schema import NodeWithScore
 
 from test.llama_index.optimizing.base import build_extractor_service_context, add_vector_index, build_vector_store, \
-    build_service_context, llm, user_questions
+    user_questions, splitter
 from test.llama_index.optimizing.custom_keyword_extractor import MyKeywordExtractor
 from turing_planet.llama_index.llms.sparkai import SparkAI
 
 INDEX_NAME = "hf_llamaindex_kw"
 
 prompt_template = """
   根据用户的关键词，选择出给定的上下文关键词列表中最匹配的关键词，地点名称不作为关键词。
@@ -42,17 +42,16 @@
 上下文：
 {context_str}
 """
 
 
 # 向量检索重排检索器
 class VectorReRankRetriever(BaseRetriever):
-    def __init__(self, vector_retriever: VectorIndexRetriever, llm: SparkAI):
+    def __init__(self, vector_retriever: VectorIndexRetriever):
         self._vector_retriever = vector_retriever
-        self._llm = llm
         super().__init__()
 
     def _retrieve(self, query_bundle: QueryBundle) -> List[NodeWithScore]:
         # 1. 向量检索，选取topN重排集合
         vector_nodes = self._vector_retriever.retrieve(query_bundle)
         if len(vector_nodes) <= 1:
             return vector_nodes
@@ -60,20 +59,20 @@
         # 2. 选取待选node的关键词
         keyword_context = ""
         for i, vector_node in enumerate(vector_nodes):
             keyword_context = keyword_context + f"{i} <--> {vector_node.metadata.get('excerpt_keywords')}\n"
 
         # 3. 获取用户问题关键词
         q_keywords_prompt = question_keywords_prompt_template.replace("{context_str}", query_bundle.query_str)
-        question_keywords = llm.complete(q_keywords_prompt).text
+        question_keywords = Settings.llm.complete(q_keywords_prompt).text
         print(f"===提取用户问题关键词\n问题：{q_keywords_prompt}\n用户关键词结果：{question_keywords}")
 
         # 4. 选取和用户关键词最匹配的待选node
         prompt = prompt_template.replace("{context_str}", keyword_context).replace("{keywords}", question_keywords)
-        keyword_index = llm.complete(prompt).text
+        keyword_index = Settings.llm.complete(prompt).text
         print(f"===匹配关键词\n问题：{prompt}\n命中关键词结果：{keyword_index}")
         target_index = 0
         try:
             target_index = int(keyword_index)
         except ValueError:
             print("转换index失败", keyword_index)
         if target_index >= len(vector_nodes):
@@ -82,28 +81,28 @@
 
         retrieve_nodes = [vector_nodes[target_index]]
         return retrieve_nodes
 
 
 def index():
     extractor = MyKeywordExtractor(llm=SparkAI(), keywords=3)
-    service_context = build_extractor_service_context(extractor)
-    add_vector_index(service_context=service_context, index_name=INDEX_NAME)
+    add_vector_index(index_name=INDEX_NAME, transformations=[
+        splitter,
+        extractor
+    ])
 
 
 def query():
     #  向量检索
-    vector_index = VectorStoreIndex.from_vector_store(vector_store=build_vector_store(index_name=INDEX_NAME),
-                                                      service_context=build_service_context())
+    vector_index = VectorStoreIndex.from_vector_store(vector_store=build_vector_store(index_name=INDEX_NAME))
     vector_retriever = VectorIndexRetriever(index=vector_index, similarity_top_k=3)
 
     # 向量重排检索
-    rerank_retriever = VectorReRankRetriever(vector_retriever=vector_retriever, llm=llm)
+    rerank_retriever = VectorReRankRetriever(vector_retriever=vector_retriever)
     response_synthesizer = get_response_synthesizer(
-        service_context=build_service_context(),
         response_mode="tree_summarize",
     )
 
     query_engine = RetrieverQueryEngine(retriever=rerank_retriever, response_synthesizer=response_synthesizer)
 
     for question in user_questions:
         response = query_engine.query(question + "\nResponse in Chinese")
```

### Comparing `turing-planet-0.0.9/test/llama_index/optimizing/qa_metadata.py` & `turing-planet-0.1.0/test/llama_index/optimizing/qa_metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-from test.llama_index.optimizing.base import add_vector_index, query, build_qa_service_context
+from llama_index.core.extractors import QuestionsAnsweredExtractor
+
+from test.llama_index.optimizing.base import add_vector_index, query, splitter
 
 # 增加问题对，没有明显提升
 INDEX_NAME = "hf_llamaindex_qa"
 
 if __name__ == '__main__':
-    service_context = build_qa_service_context(questions=2)
+    extractor = QuestionsAnsweredExtractor(questions=2)
 
-    add_vector_index(service_context=service_context, index_name=INDEX_NAME)
+    add_vector_index(index_name=INDEX_NAME, transformations=[splitter, extractor])
 
-    query(service_context=service_context, index_name=INDEX_NAME)
+    query(index_name=INDEX_NAME)
 
 # Q:合肥市政府购买居家养老服务服务对象以及服务标准
 # A:在合肥市，政府购买居家养老服务的服务对象主要包括以下三类：
 # 1. 70周岁以上低保老年人；
 # 2. 70周岁以上空巢（无子女）老年人；
 # 3. 90周岁以上高龄老年人。
 #
```

### Comparing `turing-planet-0.0.9/test/llama_index/optimizing/summary_index.py` & `turing-planet-0.1.0/test/llama_index/optimizing/summary_index.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # 向量 + 摘要索引
 from typing import List
 
-from llama_index import get_response_synthesizer, QueryBundle, DocumentSummaryIndex, VectorStoreIndex, StorageContext
-from llama_index.core import BaseRetriever
-from llama_index.indices.document_summary import DocumentSummaryIndexLLMRetriever
-from llama_index.indices.knowledge_graph import KGTableRetriever
-from llama_index.indices.vector_store import VectorIndexRetriever
-from llama_index.query_engine import RetrieverQueryEngine
-from llama_index.schema import NodeWithScore
-from llama_index.storage.index_store import MongoIndexStore
+from llama_index.core import get_response_synthesizer, QueryBundle, DocumentSummaryIndex, VectorStoreIndex, \
+    StorageContext
+from llama_index.core.base.base_retriever import BaseRetriever
+from llama_index.core.indices.document_summary import DocumentSummaryIndexLLMRetriever
+from llama_index.core.indices.vector_store import VectorIndexRetriever
+from llama_index.core.query_engine import RetrieverQueryEngine
+from llama_index.core.schema import NodeWithScore
+from llama_index.storage.index_store.mongodb import MongoIndexStore
 
 from test.llama_index.optimizing.base import build_vector_store, load_documents, build_service_context, user_questions
 
 
 class CustomRetriever(BaseRetriever):
 
     def __init__(
```

### Comparing `turing-planet-0.0.9/test/llama_index/optimizing/turing_knowledge.py` & `turing-planet-0.1.0/test/llama_index/optimizing/turing_knowledge.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import time
 
-from llama_index import SimpleDirectoryReader
-from llama_index.readers.file.base import DEFAULT_FILE_READER_CLS
+from llama_index.core import SimpleDirectoryReader
 
 from turing_planet.langchain.llm.sparkai import SparkAI
 from turing_planet.llama_index.readers.file.turing_markdown_reader import TuringMarkdownReader
 
 SUMMARY_PROMPT_TEMPL = """
 ## 任务
 你是一个文档总结高手，根据文档内容，总结出这篇文档的摘要。
@@ -107,15 +106,15 @@
 
     print("===answer===")
     print(spark.invoke(prompt))
 
 
 def summary_doc():
     # 替换默认的md文件解析
-    DEFAULT_FILE_READER_CLS.update({".md": TuringMarkdownReader})
+    # DEFAULT_FILE_READER_CLS.update({".md": TuringMarkdownReader})
 
     spark = SparkAI(endpoint="172.31.164.103:9980")
     spark.temperature = 0
 
     input_dir = "/Users/wujian/Downloads/skynet-doc-center/turing-zhiwen/4.0.14/"
     simple_reader = SimpleDirectoryReader(
         input_dir=input_dir,
```

### Comparing `turing-planet-0.0.9/test/llama_index/optimizing/vector_index.py` & `turing-planet-0.1.0/test/llama_index/optimizing/vector_index.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.0.9/test/llama_index/optimizing/vector_index_cq.py` & `turing-planet-0.1.0/test/llama_index/optimizing/vector_index_cq.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,21 +19,19 @@
 
 Q: 现在是169的套餐只有300M，可以转成现在的169元500的全屋智能套餐吗？
 A: 原169元套餐不能平迁全屋智能169元套餐，仅限169元以下用户办理。
 """
 from typing import List
 
 from dotenv import load_dotenv
-from llama_index import SimpleDirectoryReader, StorageContext, VectorStoreIndex, ServiceContext
-from llama_index.callbacks import EventPayload, CBEventType
-from llama_index.node_parser import SentenceSplitter
-from llama_index.vector_stores import RedisVectorStore
+from llama_index.core import SimpleDirectoryReader, StorageContext, VectorStoreIndex
+from llama_index.core.callbacks import EventPayload, CBEventType
+from llama_index.core.node_parser import SentenceSplitter
 
-from turing_planet.llama_index.embeddings.sparkai import SparkAIEmbedding
-from turing_planet.llama_index.llms.sparkai import SparkAI
+from test.llama_index.optimizing.base import build_vector_store
 
 load_dotenv()
 
 
 # 这里粗暴的按照句子拆分了，效果有提升 （2/7）--》（3/7）
 class MySentenceSplitter(SentenceSplitter):
 
@@ -51,21 +49,17 @@
                 if not split.text.isspace():
                     chunks.append(split.text)
             event.on_end(payload={EventPayload.CHUNKS: chunks})
 
         return chunks
 
 
-llm = SparkAI()
-embed_model = SparkAIEmbedding(domain="emb_v2")
-redis_store = RedisVectorStore(index_name="cq_llamaindex", index_prefix="cq_llamaindex_vector", redis_url="redis://172.31.128.153:6379", overwrite=True)
+redis_store = build_vector_store(index_name="cq_llamaindex")
 storage_context = StorageContext.from_defaults(vector_store=redis_store)
-service_context = ServiceContext.from_defaults(embed_model=embed_model, llm=llm,
-                                               # text_splitter=MySentenceSplitter()
-                                               )
+
 
 # 基准测试（纯向量）
 
 user_questions = ["我办理的海量卡29元的套餐，可以再加一张副卡吗?",
                   "149元档次的5G融合套餐用户已经添加了两张副卡，现在用户还想再添加一张副卡，请问可以办理吗？",
                   "我在去年（2022年）办理了一个电信电视，现在我想办理安防宽带139档，然后把电视和宽带合在一起，电视是不是可以免费呀？",
                   "办理了5G套餐，是不是就可以使用5G网络了?",
@@ -80,20 +74,19 @@
     documents = simple_reader.load_data(show_progress=True)
     return documents
 
 
 def add_vector_index():
     VectorStoreIndex.from_documents(documents=load_documents(),
                                     storage_context=storage_context,
-                                    service_context=service_context,
                                     show_progress=True)
 
 
 def query():
-    index = VectorStoreIndex.from_vector_store(vector_store=redis_store, service_context=service_context)
+    index = VectorStoreIndex.from_vector_store(vector_store=redis_store)
     query_engine = index.as_query_engine(similarity_top_k=1)
     for question in user_questions:
         response = query_engine.query(question)
         print(f"Q:{question}")
         print(f"A:{response}")
         print(f"file:{response.source_nodes[0].metadata['file_name']}")
         # print(f"source:{response.source_nodes[0].text}")
```

### Comparing `turing-planet-0.0.9/test/llama_index/pk/llama_index_spark-0131.py` & `turing-planet-0.1.0/test/llama_index/pk/llama_index_spark-0131.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,53 +1,59 @@
 import logging
 
 import openpyxl
-from llama_index import (
+from llama_index.core import (
     StorageContext,
     SimpleDirectoryReader,
     VectorStoreIndex,
-    ServiceContext,
+    Settings,
 )
-from llama_index.vector_stores import RedisVectorStore
+from llama_index.vector_stores.redis import RedisVectorStore
+from redis import Redis
+from redisvl.schema import IndexSchema
 
 from turing_planet.llama_index.embeddings.sparkai import SparkAIEmbedding
 from turing_planet.llama_index.llms.sparkai import SparkAI
 
 logging.basicConfig(
     level=logging.ERROR,
     format="%(asctime)s - %(levelname)s - %(message)s",
 )
 
 # 使用自定义embedding和llm
 endpoint = "172.31.164.103:9980"
-llm = SparkAI(endpoint=endpoint, timeout=10000)
-embed_model = SparkAIEmbedding(endpoint=endpoint, domain="emb_v1")
-
-# 使用自定义embedding和llm
-service_context = ServiceContext.from_defaults(
-    embed_model=embed_model,
-    llm=llm,
-    chunk_size=1024,
-    chunk_size_limit=256,
-    chunk_overlap=128,
-)
-
-
-# set_global_service_context(service_context)
+Settings.llm = SparkAI(endpoint=endpoint)
+Settings.embed_model = SparkAIEmbedding(endpoint=endpoint, domain="emb_xfyun")
+Settings.chunk_size = 1024
 
 
 def vector_store():
     print("init redis store begin ...")
-    return RedisVectorStore(
-        index_name="llamaindex-0131-2048-emb_v1",
-        index_prefix=f"llamaindex-0131-2048-emb_v1_vector",
-        redis_url="redis://172.31.128.153:6379",
-        overwrite=True
+    redis_index_schema = IndexSchema.from_dict(
+        {
+            # customize basic index specs
+            "index": {
+                "name": "llamaindex-0131-2048-emb_v1",
+                "prefix": "llamaindex-0131-2048-emb_v1_vector",
+                "key_separator": ":",
+            },
+            # customize fields that are indexed
+            "fields": [
+                {"name": "id", "type": "tag"},
+                {"name": "doc_id", "type": "tag"},
+                {"name": "text", "type": "text"},
+                {"name": "vector", "type": "vector",
+                 "attrs": {"dims": 2560, "algorithm": "flat", "distance_metric": "cosine", }},
+            ],
+        }
     )
 
+    redis_client = Redis.from_url("redis://172.31.128.153:6379")
+    return RedisVectorStore(schema=redis_index_schema, redis_client=redis_client, overwrite=True)
+
 
 def build_index(vector_store):
     # 加载data目录下文件，
 
     docPath = "/Users/wujian/Downloads/test/合同"
     print("load data begin ...")
 
@@ -61,25 +67,24 @@
 
     storage_context = StorageContext.from_defaults(vector_store=vector_store)
 
     # 创建索引，这一步会触发embedding操作，特征默认存储在本机内存中
     print("build index begin ...")
     index = VectorStoreIndex.from_documents(
         documents=documents,
-        service_context=service_context,
         storage_context=storage_context,
         show_progress=True,
     )
     print("build index end.")
 
 
 def query(vector_store):
     # 直接从向量库中加载
     index = VectorStoreIndex.from_vector_store(
-        vector_store=vector_store, service_context=service_context, show_progress=True
+        vector_store=vector_store, show_progress=True
     )
 
     # 执行查询，询问文档里面的内容
     query_engine = index.as_query_engine(similarity_top_k=1)
 
     # 读取Excel文件
     workbook = openpyxl.load_workbook('/Users/wujian/Downloads/test/合同query.xlsx')
```

### Comparing `turing-planet-0.0.9/test/llama_index/pk/pk.py` & `turing-planet-0.1.0/test/llama_index/pk/pk_excel_embedding.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 import logging
 import os
 from typing import List
 
 import pandas as pd
 
-from llama_index import StorageContext, SimpleDirectoryReader, VectorStoreIndex, ServiceContext, PromptTemplate
-from llama_index.readers.file.base import DEFAULT_FILE_READER_CLS
-from llama_index.vector_stores import RedisVectorStore, FilterOperator, MetadataFilters, MetadataFilter
+from llama_index.core import StorageContext, SimpleDirectoryReader, VectorStoreIndex, ServiceContext, PromptTemplate, \
+    Settings
+from llama_index.core.vector_stores import FilterOperator, MetadataFilters, MetadataFilter
 from pydantic.v1 import BaseModel
 
+from test.llama_index.pk.base import build_vector_store
 from turing_planet.llama_index.embeddings.sparkai import SparkAIEmbedding
 from turing_planet.llama_index.llms.sparkai import SparkAI
-from turing_planet.llama_index.readers.file.excel import ExcelReader
+from turing_planet.llama_index.readers.file.excel import ExcelReader, ExcelSummaryReader
 
 logging.basicConfig(
-    level=logging.INFO,
+    level=logging.ERROR,
     format="%(asctime)s - %(levelname)s - %(message)s",
 )
 
-DEFAULT_FILE_READER_CLS.update({".xlsx": ExcelReader, ".xls": ExcelReader})
+
+# DEFAULT_FILE_READER_CLS.update({".xlsx": ExcelSummaryReader, ".xls": ExcelSummaryReader})
 
 
 class Config(BaseModel):
     endpoint: str = "172.31.164.103:9980"
     # model_domain = "general"
     model_domain = "65B"
     emb_domain: str = "emb_v1"
     # 默认值
-    chunk_size: int = 1024
+    chunk_size: int = 7000
+    context_window: int = 7500
     # 默认值 20
-    chunk_overlap: int = 200
+    chunk_overlap: int = 20
     top_k: int = 3
-    know_input_dir: str = "/Users/wujian/Downloads/30/know"
-    query_input_dir: str = "/Users/wujian/Downloads/30/query"
-    answer_input_dir: str = "/Users/wujian/Downloads/30/answer"
+    know_input_dir: str = "/Users/wujian/Downloads/30/know/execl"
+    query_input_dir: str = "/Users/wujian/Downloads/30/query/execl"
+    answer_input_dir: str = "/Users/wujian/Downloads/30/answer_emb/execl"
     filter_key: str = "dir"
 
 
 config = Config()
+redis_store = build_vector_store(index_name=f"llamaindex-pk-excel-7900cs-{config.emb_domain}", dims=config.dims)
 
-redis_store = RedisVectorStore(index_name=f"llamaindex-pk-all-{config.emb_domain}",
-                               index_prefix=f"llamaindex-pk-all-{config.emb_domain}_vector",
-                               redis_url="redis://172.31.128.153:6379",
-                               overwrite=True,
-                               metadata_fields=[config.filter_key])
 storage_context = StorageContext.from_defaults(vector_store=redis_store)
 
-llm = SparkAI(endpoint=config.endpoint, domain=config.model_domain, timeout=10000, temperature=0.5)
-embed_model = SparkAIEmbedding(endpoint=config.endpoint, domain=config.emb_domain)
-service_context = ServiceContext.from_defaults(embed_model=embed_model, llm=llm, chunk_size=config.chunk_size,
-                                               chunk_overlap=config.chunk_overlap)
+Settings.llm = SparkAI(endpoint=config.endpoint, domain=config.model_domain, timeout=10000, temperature=0.5)
+Settings.embed_model = SparkAIEmbedding(endpoint=config.endpoint, domain=config.emb_domain)
+Settings.chunk_size = config.chunk_size
+Settings.chunk_overlap = config.chunk_overlap
+Settings.context_window = config.context_window
 
 
 def find_excel_files():
     file_paths = []
     for root, dirs, files in os.walk(config.query_input_dir):
         for filename in files:
             if filename.lower().endswith(('.xlsx', '.xls')) and not filename.startswith('.~'):
@@ -106,40 +106,39 @@
         document.metadata[config.filter_key] = directory
         # 默认添加的元数据会 被llm和embed使用
         document.excluded_llm_metadata_keys = [config.filter_key]
         document.excluded_embed_metadata_keys = [config.filter_key]
 
     VectorStoreIndex.from_documents(documents=documents,
                                     storage_context=storage_context,
-                                    service_context=service_context,
                                     show_progress=True)
 
 
 def query():
-    index = VectorStoreIndex.from_vector_store(vector_store=redis_store, service_context=service_context,
+    index = VectorStoreIndex.from_vector_store(vector_store=redis_store,
                                                show_progress=True)
+
     question_file_list = find_excel_files()
+
     for excel_file in question_file_list:
         print(f"==== query start: {excel_file}")
         # 设置过滤条件, 找到对应的目录的知识点
         directory, filename = os.path.split(excel_file)
         filters = MetadataFilters(
             filters=[
                 MetadataFilter(key=config.filter_key, operator=FilterOperator.EQ,
                                value=directory.replace("query", "know")),
             ]
         )
-        query_engine = index.as_query_engine(similarity_top_k=config.top_k, filters=filters)
+        retriever = index.as_retriever(similarity_top_k=config.top_k, filters=filters)
 
-        result_list = []
         for question in read_excel(excel_file):
-            result = query_engine.query(question + "\n\n当用户的问题涉及推理和计算方面时，请认真思考并逐步进行推理，然后用中文回答。") #
-            r = result.response.replace("<ret>", "\n").replace("<end>", "")
-            result_list.append(r)
-            print(f"question: {question}\n answer: {r}\n=== query end === ")
-        save_excel(excel_file, result_list)
+            print(f"question: {question}")
+            recall_node_list = retriever.retrieve(question)
+            node_list = " ; ".join([recall_node.metadata['file_name'] for recall_node in recall_node_list])
+            print(f"node: {node_list}")
     print("----- finish-----")
 
 
 if __name__ == '__main__':
     # doc_index()
     query()
```

### Comparing `turing-planet-0.0.9/test/llama_index/pk/pk_excel_chunsize.py` & `turing-planet-0.1.0/test/llama_index/pk/pk_excel_chunsize_rerank.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,62 +1,64 @@
 import logging
 import os
 from typing import List
 
 import pandas as pd
 
-from llama_index import StorageContext, SimpleDirectoryReader, VectorStoreIndex, ServiceContext, PromptTemplate
-from llama_index.readers.file.base import DEFAULT_FILE_READER_CLS
-from llama_index.vector_stores import RedisVectorStore, FilterOperator, MetadataFilters, MetadataFilter
+from llama_index.core import StorageContext, SimpleDirectoryReader, VectorStoreIndex, ServiceContext, PromptTemplate, \
+    Settings
+from llama_index.core.postprocessor import LLMRerank
+from llama_index.core.vector_stores import FilterOperator, MetadataFilters, MetadataFilter
 from pydantic.v1 import BaseModel
 
+from test.llama_index.pk.base import build_vector_store
 from turing_planet.llama_index.embeddings.sparkai import SparkAIEmbedding
 from turing_planet.llama_index.llms.sparkai import SparkAI
 from turing_planet.llama_index.readers.file.excel import ExcelReader
 
 logging.basicConfig(
     level=logging.DEBUG,
     format="%(asctime)s - %(levelname)s - %(message)s",
 )
 
-DEFAULT_FILE_READER_CLS.update({".xlsx": ExcelReader, ".xls": ExcelReader})
 
+# DEFAULT_FILE_READER_CLS.update({".xlsx": ExcelReader, ".xls": ExcelReader})
+
+
+# 召回二次精排
 
 class Config(BaseModel):
     endpoint: str = "172.31.164.103:9980"
     model_domain = "generalv3"
     # model_domain = "65B"
     emb_domain: str = "emb_v1"
+    dims: int = 1024
     # 默认值
     chunk_size: int = 7000
     context_window: int = 7500
     # 默认值 20
     chunk_overlap: int = 20
     top_k: int = 3
     know_input_dir: str = "/Users/wujian/Downloads/30/know/execl"
     query_input_dir: str = "/Users/wujian/Downloads/30/query/execl"
     answer_input_dir: str = "/Users/wujian/Downloads/30/answer/execl"
     filter_key: str = "dir"
 
 
 config = Config()
 
-redis_store = RedisVectorStore(
-    index_name=f"llamaindex-pk-excel-7900cs-{config.emb_domain}",
-    index_prefix=f"llamaindex-pk-excel-7900cs-{config.emb_domain}_vector",
-    redis_url="redis://172.31.128.153:6379",
-    overwrite=True,
-    metadata_fields=[config.filter_key])
+redis_store = build_vector_store(index_name=f"llamaindex-pk-excel-7900cs-{config.emb_domain}", dims=config.dims)
+
 storage_context = StorageContext.from_defaults(vector_store=redis_store)
 
-llm = SparkAI(endpoint=config.endpoint, domain=config.model_domain, timeout=10000, temperature=0.5)
-embed_model = SparkAIEmbedding(endpoint=config.endpoint, domain=config.emb_domain)
-service_context = ServiceContext.from_defaults(embed_model=embed_model, llm=llm, chunk_size=config.chunk_size,
-                                               chunk_overlap=config.chunk_overlap)
-service_context.prompt_helper.context_window = config.context_window
+Settings.llm = SparkAI(endpoint=config.endpoint, domain=config.model_domain, timeout=10000, temperature=0.5)
+Settings.embed_model = SparkAIEmbedding(endpoint=config.endpoint, domain=config.emb_domain)
+Settings.chunk_size = config.chunk_size
+Settings.chunk_overlap = config.chunk_overlap
+Settings.context_window = config.context_window
 
 
 def find_excel_files():
     file_paths = []
     for root, dirs, files in os.walk(config.query_input_dir):
         for filename in files:
             if filename.lower().endswith(('.xlsx', '.xls')) and not filename.startswith('.~'):
@@ -127,23 +129,31 @@
         directory, filename = os.path.split(excel_file)
         filters = MetadataFilters(
             filters=[
                 MetadataFilter(key=config.filter_key, operator=FilterOperator.EQ,
                                value=directory.replace("query", "know")),
             ]
         )
-        query_engine = index.as_query_engine(similarity_top_k=config.top_k, filters=filters)
+
+        # todo rerank
+        postprocessor = LLMRerank(top_n=2, service_context=service_context)
+
+        query_engine = index.as_query_engine(similarity_top_k=config.top_k, filters=filters,
+                                             node_postprocessors=[postprocessor])
 
         result_list = []
         for question in read_excel(excel_file):
             result = query_engine.query(
                 question + "\n\n当用户的问题涉及推理和计算方面时，请认真思考并逐步进行推理，然后用中文回答。")  #
             r = result.response.replace("<ret>", "\n").replace("<end>", "")
             result_list.append(r)
             print(f"question: {question}\n answer: {r}\n=== query end === ")
-        save_excel(excel_file, result_list)
+
+            break
+
+        # save_excel(excel_file, result_list)
     print("----- finish-----")
 
 
 if __name__ == '__main__':
     # doc_index()
     query()
```

### Comparing `turing-planet-0.0.9/test/llama_index/pk/pk_excel_chunsize_rerank.py` & `turing-planet-0.1.0/test/llama_index/pk/pk.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,65 +1,55 @@
 import logging
 import os
 from typing import List
 
 import pandas as pd
-
-from llama_index import StorageContext, SimpleDirectoryReader, VectorStoreIndex, ServiceContext, PromptTemplate
-from llama_index.postprocessor import LLMRerank
-from llama_index.readers.file.base import DEFAULT_FILE_READER_CLS
-from llama_index.vector_stores import RedisVectorStore, FilterOperator, MetadataFilters, MetadataFilter
+from llama_index.core import StorageContext, SimpleDirectoryReader, VectorStoreIndex, Settings
+from llama_index.core.vector_stores import FilterOperator, MetadataFilters, MetadataFilter
 from pydantic.v1 import BaseModel
 
+from test.llama_index.pk.base import build_vector_store
 from turing_planet.llama_index.embeddings.sparkai import SparkAIEmbedding
 from turing_planet.llama_index.llms.sparkai import SparkAI
-from turing_planet.llama_index.readers.file.excel import ExcelReader
 
 logging.basicConfig(
-    level=logging.DEBUG,
+    level=logging.INFO,
     format="%(asctime)s - %(levelname)s - %(message)s",
 )
 
-DEFAULT_FILE_READER_CLS.update({".xlsx": ExcelReader, ".xls": ExcelReader})
 
+# DEFAULT_FILE_READER_CLS.update({".xlsx": ExcelReader, ".xls": ExcelReader})
 
-# 召回二次精排
 
 class Config(BaseModel):
     endpoint: str = "172.31.164.103:9980"
-    model_domain = "generalv3"
-    # model_domain = "65B"
+    # model_domain = "general"
+    model_domain = "65B"
     emb_domain: str = "emb_v1"
+    dims: int = 1024
     # 默认值
-    chunk_size: int = 7000
-    context_window: int = 7500
+    chunk_size: int = 1024
     # 默认值 20
-    chunk_overlap: int = 20
+    chunk_overlap: int = 200
     top_k: int = 3
-    know_input_dir: str = "/Users/wujian/Downloads/30/know/execl"
-    query_input_dir: str = "/Users/wujian/Downloads/30/query/execl"
-    answer_input_dir: str = "/Users/wujian/Downloads/30/answer/execl"
+    know_input_dir: str = "/Users/wujian/Downloads/30/know"
+    query_input_dir: str = "/Users/wujian/Downloads/30/query"
+    answer_input_dir: str = "/Users/wujian/Downloads/30/answer"
     filter_key: str = "dir"
 
 
 config = Config()
+redis_store = build_vector_store(index_name=f"llamaindex-pk-all-{config.emb_domain}", dims=config.dims)
 
-redis_store = RedisVectorStore(
-    index_name=f"llamaindex-pk-excel-7900cs-{config.emb_domain}",
-    index_prefix=f"llamaindex-pk-excel-7900cs-{config.emb_domain}_vector",
-    redis_url="redis://172.31.128.153:6379",
-    overwrite=True,
-    metadata_fields=[config.filter_key])
 storage_context = StorageContext.from_defaults(vector_store=redis_store)
 
-llm = SparkAI(endpoint=config.endpoint, domain=config.model_domain, timeout=10000, temperature=0.5)
-embed_model = SparkAIEmbedding(endpoint=config.endpoint, domain=config.emb_domain)
-service_context = ServiceContext.from_defaults(embed_model=embed_model, llm=llm, chunk_size=config.chunk_size,
-                                               chunk_overlap=config.chunk_overlap)
-service_context.prompt_helper.context_window = config.context_window
+Settings.llm = SparkAI(endpoint=config.endpoint, domain=config.model_domain, timeout=10000, temperature=0.5)
+Settings.embed_model = SparkAIEmbedding(endpoint=config.endpoint, domain=config.emb_domain)
+Settings.chunk_size = config.chunk_size
+Settings.chunk_overlap = config.chunk_overlap
 
 
 def find_excel_files():
     file_paths = []
     for root, dirs, files in os.walk(config.query_input_dir):
         for filename in files:
             if filename.lower().endswith(('.xlsx', '.xls')) and not filename.startswith('.~'):
@@ -112,49 +102,39 @@
         document.metadata[config.filter_key] = directory
         # 默认添加的元数据会 被llm和embed使用
         document.excluded_llm_metadata_keys = [config.filter_key]
         document.excluded_embed_metadata_keys = [config.filter_key]
 
     VectorStoreIndex.from_documents(documents=documents,
                                     storage_context=storage_context,
-                                    service_context=service_context,
                                     show_progress=True)
 
 
 def query():
-    index = VectorStoreIndex.from_vector_store(vector_store=redis_store, service_context=service_context,
-                                               show_progress=True)
+    index = VectorStoreIndex.from_vector_store(vector_store=redis_store, show_progress=True)
     question_file_list = find_excel_files()
     for excel_file in question_file_list:
         print(f"==== query start: {excel_file}")
         # 设置过滤条件, 找到对应的目录的知识点
         directory, filename = os.path.split(excel_file)
         filters = MetadataFilters(
             filters=[
                 MetadataFilter(key=config.filter_key, operator=FilterOperator.EQ,
                                value=directory.replace("query", "know")),
             ]
         )
-
-        # todo rerank
-        postprocessor = LLMRerank(top_n=2, service_context=service_context)
-
-        query_engine = index.as_query_engine(similarity_top_k=config.top_k, filters=filters,
-                                             node_postprocessors=[postprocessor])
+        query_engine = index.as_query_engine(similarity_top_k=config.top_k, filters=filters)
 
         result_list = []
         for question in read_excel(excel_file):
             result = query_engine.query(
                 question + "\n\n当用户的问题涉及推理和计算方面时，请认真思考并逐步进行推理，然后用中文回答。")  #
             r = result.response.replace("<ret>", "\n").replace("<end>", "")
             result_list.append(r)
             print(f"question: {question}\n answer: {r}\n=== query end === ")
-
-            break
-
-        # save_excel(excel_file, result_list)
+        save_excel(excel_file, result_list)
     print("----- finish-----")
 
 
 if __name__ == '__main__':
     # doc_index()
     query()
```

### Comparing `turing-planet-0.0.9/test/llama_index/pk/pk_excel_embedding.py` & `turing-planet-0.1.0/test/llama_index/pk/pk_excel_chunsize.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,64 +1,60 @@
 import logging
 import os
 from typing import List
 
 import pandas as pd
-
-from llama_index import StorageContext, SimpleDirectoryReader, VectorStoreIndex, ServiceContext, PromptTemplate
-from llama_index.readers.file.base import DEFAULT_FILE_READER_CLS
-from llama_index.vector_stores import RedisVectorStore, FilterOperator, MetadataFilters, MetadataFilter
+from llama_index.core import StorageContext, SimpleDirectoryReader, VectorStoreIndex, Settings
+from llama_index.core.vector_stores import FilterOperator, MetadataFilters, MetadataFilter
 from pydantic.v1 import BaseModel
 
+from test.llama_index.pk.base import build_vector_store
 from turing_planet.llama_index.embeddings.sparkai import SparkAIEmbedding
 from turing_planet.llama_index.llms.sparkai import SparkAI
-from turing_planet.llama_index.readers.file.excel import ExcelReader, ExcelSummaryReader
 
 logging.basicConfig(
-    level=logging.ERROR,
+    level=logging.DEBUG,
     format="%(asctime)s - %(levelname)s - %(message)s",
 )
 
-DEFAULT_FILE_READER_CLS.update({".xlsx": ExcelSummaryReader, ".xls": ExcelSummaryReader})
+
+# DEFAULT_FILE_READER_CLS.update({".xlsx": ExcelReader, ".xls": ExcelReader})
 
 
 class Config(BaseModel):
     endpoint: str = "172.31.164.103:9980"
-    # model_domain = "general"
-    model_domain = "65B"
+    model_domain = "generalv3"
+    # model_domain = "65B"
     emb_domain: str = "emb_v1"
+    dims: int = 1024
     # 默认值
     chunk_size: int = 7000
     context_window: int = 7500
     # 默认值 20
     chunk_overlap: int = 20
     top_k: int = 3
     know_input_dir: str = "/Users/wujian/Downloads/30/know/execl"
     query_input_dir: str = "/Users/wujian/Downloads/30/query/execl"
-    answer_input_dir: str = "/Users/wujian/Downloads/30/answer_emb/execl"
+    answer_input_dir: str = "/Users/wujian/Downloads/30/answer/execl"
     filter_key: str = "dir"
 
 
 config = Config()
+redis_store = build_vector_store(index_name=f"llamaindex-pk-excel-7900cs-{config.emb_domain}", dims=config.dims)
 
-redis_store = RedisVectorStore(
-    index_name=f"llamaindex-pk-excel-7900cs-{config.emb_domain}",
-    index_prefix=f"llamaindex-pk-excel-7900cs-{config.emb_domain}_vector",
-    #  index_name=f"llamaindex-pk-excel-summary-{config.emb_domain}",
-    # index_prefix=f"llamaindex-pk-excel-summary-{config.emb_domain}_vector",
-    redis_url="redis://172.31.128.153:6379",
-    overwrite=True,
-    metadata_fields=[config.filter_key])
 storage_context = StorageContext.from_defaults(vector_store=redis_store)
 
 llm = SparkAI(endpoint=config.endpoint, domain=config.model_domain, timeout=10000, temperature=0.5)
 embed_model = SparkAIEmbedding(endpoint=config.endpoint, domain=config.emb_domain)
-service_context = ServiceContext.from_defaults(embed_model=embed_model, llm=llm, chunk_size=config.chunk_size,
-                                               chunk_overlap=config.chunk_overlap)
-service_context.prompt_helper.context_window = config.context_window
+
+Settings.llm = SparkAI(endpoint=config.endpoint, domain=config.model_domain, timeout=10000, temperature=0.5)
+Settings.embed_model = SparkAIEmbedding(endpoint=config.endpoint, domain=config.emb_domain)
+Settings.chunk_size = config.chunk_size
+Settings.chunk_overlap = config.chunk_overlap
+Settings.context_window = config.context_window
 
 
 def find_excel_files():
     file_paths = []
     for root, dirs, files in os.walk(config.query_input_dir):
         for filename in files:
             if filename.lower().endswith(('.xlsx', '.xls')) and not filename.startswith('.~'):
@@ -111,40 +107,40 @@
         document.metadata[config.filter_key] = directory
         # 默认添加的元数据会 被llm和embed使用
         document.excluded_llm_metadata_keys = [config.filter_key]
         document.excluded_embed_metadata_keys = [config.filter_key]
 
     VectorStoreIndex.from_documents(documents=documents,
                                     storage_context=storage_context,
-                                    service_context=service_context,
                                     show_progress=True)
 
 
 def query():
-    index = VectorStoreIndex.from_vector_store(vector_store=redis_store, service_context=service_context,
+    index = VectorStoreIndex.from_vector_store(vector_store=redis_store,
                                                show_progress=True)
-
     question_file_list = find_excel_files()
-
     for excel_file in question_file_list:
         print(f"==== query start: {excel_file}")
         # 设置过滤条件, 找到对应的目录的知识点
         directory, filename = os.path.split(excel_file)
         filters = MetadataFilters(
             filters=[
                 MetadataFilter(key=config.filter_key, operator=FilterOperator.EQ,
                                value=directory.replace("query", "know")),
             ]
         )
-        retriever = index.as_retriever(similarity_top_k=config.top_k, filters=filters)
+        query_engine = index.as_query_engine(similarity_top_k=config.top_k, filters=filters)
 
+        result_list = []
         for question in read_excel(excel_file):
-            print(f"question: {question}")
-            recall_node_list = retriever.retrieve(question)
-            node_list = " ; ".join([recall_node.metadata['file_name'] for recall_node in recall_node_list])
-            print(f"node: {node_list}")
+            result = query_engine.query(
+                question + "\n\n当用户的问题涉及推理和计算方面时，请认真思考并逐步进行推理，然后用中文回答。")  #
+            r = result.response.replace("<ret>", "\n").replace("<end>", "")
+            result_list.append(r)
+            print(f"question: {question}\n answer: {r}\n=== query end === ")
+        save_excel(excel_file, result_list)
     print("----- finish-----")
 
 
 if __name__ == '__main__':
     # doc_index()
     query()
```

### Comparing `turing-planet-0.0.9/test/llama_index/pk/pk_word_0201.py` & `turing-planet-0.1.0/test/llama_index/pk/pk_word_0201.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,59 +1,61 @@
 import logging
 import os
 from typing import List
 
 import pandas as pd
-from llama_index import StorageContext, SimpleDirectoryReader, VectorStoreIndex, ServiceContext, PromptTemplate
-from llama_index.readers.file.base import DEFAULT_FILE_READER_CLS
-from llama_index.vector_stores import RedisVectorStore, FilterOperator, MetadataFilters, MetadataFilter
+from llama_index.core import StorageContext, SimpleDirectoryReader, VectorStoreIndex, ServiceContext, PromptTemplate, \
+    Settings
+from llama_index.core.vector_stores import FilterOperator, MetadataFilters, MetadataFilter
 from pydantic.v1 import BaseModel
 
+from test.llama_index.pk.base import build_vector_store
 from turing_planet.llama_index.embeddings.sparkai import SparkAIEmbedding
 from turing_planet.llama_index.llms.sparkai import SparkAI
 from turing_planet.llama_index.readers.file.excel import ExcelReader
 
 logging.basicConfig(
     level=logging.DEBUG,
     format="%(asctime)s - %(levelname)s - %(message)s",
 )
 
-DEFAULT_FILE_READER_CLS.update({".xlsx": ExcelReader, ".xls": ExcelReader})
+# DEFAULT_FILE_READER_CLS.update({".xlsx": ExcelReader, ".xls": ExcelReader})
 
 # 调整了context windows size & top & prompt
 
 
-#LLamaIndex
+# LLamaIndex
 qa_prompt_tmpl_str = """
 下面是上下文信息：
 ---------------------
 {context_str}
 ---------------------
 
 根据上下文信息和知识回答问题。
 当用户的问题涉及推理和计算方面时，请认真思考并逐步进行推理，然后用中文回答。
 
 问题: {query_str}
 答案:
 """
 
-#DocQA
+# DocQA
 """
 你是一个AI助手，从输入的内容和上下文中回答我提出的问题。
 如果找到答案，可以对其进行润色，但不要改变原文的意思，也不要额外增加信息。
 如果没有答案，请回答：“抱歉，没有查询到什么是晚走晚到模式的相关内容”，在检索过程中请忽略英文大小写。
 输入的内容：{
     {context_str}
 }
 
 我提出的问题：{
     {query_str}
 }
 """
 
+
 class Config(BaseModel):
     endpoint: str = "172.31.164.103:9980"
     model_domain = "generalv3"
     # model_domain = "65B"
     emb_domain: str = "emb_v1"
     context_window: int = 7500
     # 默认值
@@ -64,27 +66,23 @@
     know_input_dir: str = "/Users/wujian/Downloads/30/know"
     query_input_dir: str = "/Users/wujian/Downloads/30/query"
     answer_input_dir: str = "/Users/wujian/Downloads/30/answer"
     filter_key: str = "dir"
 
 
 config = Config()
+redis_store = build_vector_store(index_name=f"llamaindex-pk-all-{config.emb_domain}", dims=config.dims)
 
-redis_store = RedisVectorStore(index_name=f"llamaindex-pk-all-{config.emb_domain}",
-                               index_prefix=f"llamaindex-pk-all-{config.emb_domain}_vector",
-                               redis_url="redis://172.31.128.153:6379",
-                               overwrite=True,
-                               metadata_fields=[config.filter_key])
 storage_context = StorageContext.from_defaults(vector_store=redis_store)
 
-llm = SparkAI(endpoint=config.endpoint, domain=config.model_domain, timeout=10000, temperature=0.5)
-embed_model = SparkAIEmbedding(endpoint=config.endpoint, domain=config.emb_domain)
-service_context = ServiceContext.from_defaults(embed_model=embed_model, llm=llm, chunk_size=config.chunk_size,
-                                               chunk_overlap=config.chunk_overlap)
-service_context.prompt_helper.context_window = config.context_window
+Settings.llm = SparkAI(endpoint=config.endpoint, domain=config.model_domain, timeout=10000, temperature=0.5)
+Settings.embed_model = SparkAIEmbedding(endpoint=config.endpoint, domain=config.emb_domain)
+Settings.chunk_size = config.chunk_size
+Settings.chunk_overlap = config.chunk_overlap
+Settings.context_window = config.context_window
 
 
 def find_excel_files():
     file_paths = []
     for root, dirs, files in os.walk(config.query_input_dir):
         for filename in files:
             if filename.lower().endswith(('.xlsx', '.xls')) and not filename.startswith('.~'):
@@ -137,20 +135,19 @@
         document.metadata[config.filter_key] = directory
         # 默认添加的元数据会 被llm和embed使用
         document.excluded_llm_metadata_keys = [config.filter_key]
         document.excluded_embed_metadata_keys = [config.filter_key]
 
     VectorStoreIndex.from_documents(documents=documents,
                                     storage_context=storage_context,
-                                    service_context=service_context,
                                     show_progress=True)
 
 
 def query():
-    index = VectorStoreIndex.from_vector_store(vector_store=redis_store, service_context=service_context,
+    index = VectorStoreIndex.from_vector_store(vector_store=redis_store,
                                                show_progress=True)
     question_file_list = find_excel_files()
     for excel_file in question_file_list:
         print(f"==== query start: {excel_file}")
         # 设置过滤条件, 找到对应的目录的知识点
         directory, filename = os.path.split(excel_file)
         filters = MetadataFilters(
```

### Comparing `turing-planet-0.0.9/test/llama_index/pk/pk_word_es_0201.py` & `turing-planet-0.1.0/test/llama_index/pk/pk_word_es_0201.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 import logging
 import os
 from typing import List
 
 import pandas as pd
-from llama_index import StorageContext, SimpleDirectoryReader, VectorStoreIndex, ServiceContext, PromptTemplate, \
-    QueryBundle, get_response_synthesizer
-from llama_index.core import BaseRetriever
-from llama_index.indices.vector_store import VectorIndexRetriever
-from llama_index.query_engine import RetrieverQueryEngine
-from llama_index.readers.file.base import DEFAULT_FILE_READER_CLS
-from llama_index.schema import NodeWithScore
-from llama_index.vector_stores import RedisVectorStore, FilterOperator, MetadataFilters, MetadataFilter, \
-    ElasticsearchStore
-from llama_index.vector_stores.types import VectorStoreQueryMode
+from llama_index.core import StorageContext, SimpleDirectoryReader, VectorStoreIndex, PromptTemplate, \
+    QueryBundle, get_response_synthesizer, Settings
+from llama_index.core.base.base_retriever import BaseRetriever
+from llama_index.core.indices.vector_store import VectorIndexRetriever
+from llama_index.core.query_engine import RetrieverQueryEngine
+from llama_index.core.schema import NodeWithScore
+from llama_index.core.vector_stores import FilterOperator, MetadataFilters, MetadataFilter
+from llama_index.core.vector_stores.types import VectorStoreQueryMode
+from llama_index.vector_stores.elasticsearch import ElasticsearchStore
 from pydantic.v1 import BaseModel
 
 from turing_planet.llama_index.embeddings.sparkai import SparkAIEmbedding
 from turing_planet.llama_index.llms.sparkai import SparkAI
-from turing_planet.llama_index.readers.file.excel import ExcelReader
 
 logging.basicConfig(
     level=logging.DEBUG,
     format="%(asctime)s - %(levelname)s - %(message)s",
     # filename='pk.log',
 )
 
-DEFAULT_FILE_READER_CLS.update({".xlsx": ExcelReader, ".xls": ExcelReader})
+# DEFAULT_FILE_READER_CLS.update({".xlsx": ExcelReader, ".xls": ExcelReader})
 
 qa_prompt_tmpl_str = """
 Context information is below.
 ---------------------
 {context_str}
 ---------------------
 
@@ -118,20 +116,19 @@
 config = Config()
 
 es_vector_store = ElasticsearchStore(es_url="http://172.31.164.103:49200", index_name="llamaindex-pk-doc-1024",
                                      batch_size=10)
 
 storage_context = StorageContext.from_defaults(vector_store=es_vector_store)
 
-llm = SparkAI(endpoint=config.endpoint, domain=config.model_domain, timeout=10000, temperature=0.5,
-              punish=config.punish)
-embed_model = SparkAIEmbedding(endpoint=config.endpoint, domain=config.emb_domain)
-service_context = ServiceContext.from_defaults(embed_model=embed_model, llm=llm, chunk_size=config.chunk_size,
-                                               chunk_overlap=config.chunk_overlap)
-service_context.prompt_helper.context_window = config.context_window
+Settings.llm = SparkAI(endpoint=config.endpoint, domain=config.model_domain, timeout=10000, temperature=0.5)
+Settings.embed_model = SparkAIEmbedding(endpoint=config.endpoint, domain=config.emb_domain)
+Settings.chunk_size = config.chunk_size
+Settings.chunk_overlap = config.chunk_overlap
+Settings.context_window = config.context_window
 
 
 def find_excel_files():
     file_paths = []
     for root, dirs, files in os.walk(config.query_input_dir):
         for filename in files:
             if filename.lower().endswith(('.xlsx', '.xls')) and not filename.startswith('.~'):
@@ -184,20 +181,19 @@
         document.metadata[config.filter_key] = directory
         # 默认添加的元数据会 被llm和embed使用
         document.excluded_llm_metadata_keys = [config.filter_key]
         document.excluded_embed_metadata_keys = [config.filter_key]
 
     VectorStoreIndex.from_documents(documents=documents,
                                     storage_context=storage_context,
-                                    service_context=service_context,
                                     show_progress=True)
 
 
 def query():
-    index = VectorStoreIndex.from_vector_store(vector_store=es_vector_store, service_context=service_context,
+    index = VectorStoreIndex.from_vector_store(vector_store=es_vector_store,
                                                show_progress=True)
     question_file_list = find_excel_files()
     for excel_file in question_file_list:
         print(f"==== query start: {excel_file}")
         # 设置过滤条件, 找到对应的目录的知识点
         directory, filename = os.path.split(excel_file)
         filters = MetadataFilters(
@@ -205,16 +201,15 @@
                 MetadataFilter(key=config.filter_key, operator=FilterOperator.EQ,
                                value=directory.replace("query", "know")),
             ]
         )
 
         vector_retriever = index.as_retriever(similarity_top_k=config.top_k, filters=filters, )
         combine_retriever = VectorCombineRetriever(vector_retriever=vector_retriever)
-        response_synthesizer = get_response_synthesizer(service_context=service_context,
-                                                        text_qa_template=PromptTemplate(qa_prompt_tmpl_str))
+        response_synthesizer = get_response_synthesizer(text_qa_template=PromptTemplate(qa_prompt_tmpl_str))
         query_engine = RetrieverQueryEngine.from_args(retriever=combine_retriever,
                                                       response_synthesizer=response_synthesizer)
 
         result_list = []
         for question in read_excel(excel_file):
             result = query_engine.query(question)
             r = result.response.replace("<ret>", "\n").replace("<end>", "")
```

### Comparing `turing-planet-0.0.9/test/llama_index/pk/sample_excel.py` & `turing-planet-0.1.0/test/llama_index/pk/sample_excel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 import logging
 
 import pandas as pd
-from llama_index import ServiceContext, SimpleDirectoryReader, VectorStoreIndex
-from llama_index.constants import DEFAULT_CONTEXT_WINDOW
-from llama_index.readers.file.base import DEFAULT_FILE_READER_CLS
+from llama_index.core import ServiceContext, SimpleDirectoryReader, VectorStoreIndex
 
 from turing_planet.llama_index.embeddings.sparkai import SparkAIEmbedding
 from turing_planet.llama_index.llms.sparkai import SparkAI
-from turing_planet.llama_index.readers.file.excel import ExcelReader, ExcelSummaryReader
 
 logging.basicConfig(
     level=logging.INFO,
     format="%(asctime)s - %(levelname)s - %(message)s",
 )
 # DEFAULT_CONTEXT_WINDOW = 200
-DEFAULT_FILE_READER_CLS.update({".xlsx": ExcelSummaryReader, ".xls": ExcelSummaryReader})
+# DEFAULT_FILE_READER_CLS.update({".xlsx": ExcelSummaryReader, ".xls": ExcelSummaryReader})
 excel_file_path = "/Users/wujian/Downloads/30/know/execl/银行/产品表/合肥科技农村商业银行产品介绍.xlsx"
 # /Users/wujian/Downloads/30/know/execl/银行/产品表/合肥科技农村商业银行产品介绍-.xlsx
 # /Users/wujian/Downloads/30/know/execl/银行/产品表/徽商银行-.xlsx
 # /Users/wujian/Downloads/30/know/execl/报表/企业财务报表1.xlsx
 
 # /Users/wujian/Downloads/30/query/execl/银行/产品表/中国银行理财产品.xlsx
```

### Comparing `turing-planet-0.0.9/test/llama_index/skydoc-embedding.py` & `turing-planet-0.1.0/test/llama_index/skydoc-embedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 
-from llama_index import SimpleDirectoryReader, ServiceContext, StorageContext, VectorStoreIndex
-from llama_index.vector_stores import RedisVectorStore
+from llama_index.core import SimpleDirectoryReader, ServiceContext, StorageContext, VectorStoreIndex
+from llama_index.vector_stores.redis import RedisVectorStore
 
 from turing_planet.llama_index.embeddings.sparkai import SparkAIEmbedding
 from turing_planet.llama_index.llms.sparkai import SparkAI
 from turing_planet.llama_index.vector_stores.planet import PlanetVectorStore
 
 logging.basicConfig(
     level=logging.DEBUG,  # 设置日志级别为DEBUG，可以根据需要修改
```

### Comparing `turing-planet-0.0.9/test/llama_index/start.py` & `turing-planet-0.1.0/test/llama_index/start.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 
-from llama_index import ServiceContext, SimpleDirectoryReader, VectorStoreIndex, StorageContext, KnowledgeGraphIndex, \
+from llama_index.core import ServiceContext, SimpleDirectoryReader, VectorStoreIndex, StorageContext, KnowledgeGraphIndex, \
     TreeIndex, PromptTemplate
-from llama_index.graph_stores import SimpleGraphStore
-from llama_index.postprocessor import KeywordNodePostprocessor
-from llama_index.vector_stores import MetadataFilters, MetadataFilter, FilterOperator
+from llama_index.core.graph_stores import SimpleGraphStore
+from llama_index.core.postprocessor import KeywordNodePostprocessor
+from llama_index.core.vector_stores import MetadataFilters, MetadataFilter, FilterOperator
 
 from turing_planet.llama_index.embeddings.sparkai import SparkAIEmbedding
 from turing_planet.llama_index.llms.sparkai import SparkAI
 
 # optionally set a global service context to avoid passing it into other objects every time
 
 logging.basicConfig(
```

### Comparing `turing-planet-0.0.9/turing_planet/api/planet_embedding_client.py` & `turing-planet-0.1.0/turing_planet/api/planet_embedding_client.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.0.9/turing_planet/api/planet_vector_client.py` & `turing-planet-0.1.0/turing_planet/api/planet_vector_client.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.0.9/turing_planet/api/spark_chat_client.py` & `turing-planet-0.1.0/turing_planet/api/spark_chat_client.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.0.9/turing_planet/deprecated/spark_embedding_client.py` & `turing-planet-0.1.0/turing_planet/deprecated/spark_embedding_client.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.0.9/turing_planet/langchain/chat_models/sparkai.py` & `turing-planet-0.1.0/turing_planet/langchain/chat_models/sparkai.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Any, Dict, Iterator, List, Mapping, Optional, Type
 
 from turing_planet.api.spark_chat_client import SparkLLMClient
 
 from langchain.callbacks.manager import CallbackManagerForLLMRun
 from langchain.chat_models.base import (
     BaseChatModel,
-    _generate_from_stream,
+    generate_from_stream,
 )
 from langchain.pydantic_v1 import Field, root_validator
 from langchain.schema import (
     AIMessage,
     BaseMessage,
     ChatGeneration,
     ChatMessage,
@@ -195,15 +195,15 @@
             run_manager: Optional[CallbackManagerForLLMRun] = None,
             **kwargs: Any,
     ) -> ChatResult:
         if self.streaming:
             stream_iter = self._stream(
                 messages=messages, stop=stop, run_manager=run_manager, **kwargs
             )
-            return _generate_from_stream(stream_iter)
+            return generate_from_stream(stream_iter)
 
         self.client.arun(
             [_convert_message_to_dict(m) for m in messages],
             self.model_kwargs,
             kwargs,
             False,
         )
```

### Comparing `turing-planet-0.0.9/turing_planet/langchain/embeddings/sparkai.py` & `turing-planet-0.1.0/turing_planet/langchain/embeddings/sparkai.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.0.9/turing_planet/langchain/llm/sparkai.py` & `turing-planet-0.1.0/turing_planet/langchain/llm/sparkai.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.0.9/turing_planet/llama_index/embeddings/sparkai.py` & `turing-planet-0.1.0/turing_planet/llama_index/embeddings/sparkai.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Any, Optional
 
-from llama_index.embeddings.base import BaseEmbedding, Embedding
+from llama_index.core.base.embeddings.base import BaseEmbedding, Embedding
 
 from turing_planet.api.planet_embedding_client import PlanetEmbeddingClient
 
 
 class SparkAIEmbedding(BaseEmbedding):
     client: Any
```

### Comparing `turing-planet-0.0.9/turing_planet/llama_index/llms/sparkai.py` & `turing-planet-0.1.0/turing_planet/llama_index/llms/sparkai.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # 自定义大模型
 from typing import Any, Optional
 
-from llama_index.llms import CustomLLM, LLMMetadata
-from llama_index.llms.base import llm_completion_callback, CompletionResponse, CompletionResponseGen
+from llama_index.core.base.llms.types import LLMMetadata, CompletionResponse, CompletionResponseGen
+from llama_index.core.llms import CustomLLM
+from llama_index.core.llms.callbacks import llm_completion_callback
 
 from turing_planet.api.spark_chat_client import SparkLLMClient
 from turing_planet.utils.env import get_from_dict_or_env
 
 
 def _convert_prompt_to_dict(
         prompt: str,
```

### Comparing `turing-planet-0.0.9/turing_planet/llama_index/readers/file/excel.py` & `turing-planet-0.1.0/turing_planet/llama_index/readers/file/excel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional, Dict, List
 from pathlib import Path
-from llama_index.readers.base import BaseReader
-from llama_index.schema import Document
+from llama_index.core.readers.base import BaseReader
+from llama_index.core.schema import Document
 import pandas as pd
 
 # 显示全部列
 pd.set_option('display.max_columns', None)
 # 显示全部行
 pd.set_option('display.max_row', None)
 # 设置数据的显示长度（解决自动换行）
```

### Comparing `turing-planet-0.0.9/turing_planet/llama_index/readers/file/turing_markdown_reader.py` & `turing-planet-0.1.0/turing_planet/llama_index/readers/file/turing_markdown_reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 继承MarkdownReader，重写load_data函数，将文档的主标题，拼接到子标题，增强段落的上下文关系
 
 """
 from pathlib import Path
 from typing import Dict, List, Optional
 
-from llama_index.readers.file.markdown_reader import MarkdownReader
-from llama_index.schema import Document
+from llama_index.core.schema import Document
+from llama_index.readers.file import MarkdownReader
 
 
 class TuringMarkdownReader(MarkdownReader):
 
     def load_data(
             self, file: Path, extra_info: Optional[Dict] = None
     ) -> List[Document]:
```

### Comparing `turing-planet-0.0.9/turing_planet/llama_index/vector_stores/planet.py` & `turing-planet-0.1.0/turing_planet/llama_index/vector_stores/planet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import uuid
 from typing import List, Any
 
-from llama_index.schema import BaseNode, MetadataMode, TextNode
-from llama_index.vector_stores import VectorStoreQuery, VectorStoreQueryResult
-from llama_index.vector_stores.types import VectorStore
-from llama_index.vector_stores.utils import node_to_metadata_dict, metadata_dict_to_node
+from llama_index.core.schema import BaseNode, MetadataMode, TextNode
+from llama_index.core.vector_stores import VectorStoreQuery, VectorStoreQueryResult
+from llama_index.core.vector_stores.types import VectorStore
+from llama_index.core.vector_stores.utils import node_to_metadata_dict, metadata_dict_to_node
 
 from turing_planet.api.planet_vector_client import PlanetVectorClient, VectorAddRequest
 
 logger = logging.getLogger(__name__)
 
 
 # 星球向量数据库
```

### Comparing `turing-planet-0.0.9/turing_planet/utils/auth_util.py` & `turing-planet-0.1.0/turing_planet/utils/auth_util.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.0.9/turing_planet/utils/env.py` & `turing-planet-0.1.0/turing_planet/utils/env.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.0.9/turing_planet.egg-info/PKG-INFO` & `turing-planet-0.1.0/turing_planet.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: turing-planet
-Version: 0.0.9
+Version: 0.1.0
 Summary: Python Extension Framework For Turing Planet
 Home-page: https://code.iflytek.com/osc/_source/Y_RDG-TURING/gpt/turing-planet/-/tree/heads%2Fdevelop
 Author: jianwu6
 Author-email: jianwu6@iflytek.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9.0, <3.10.0
 Description-Content-Type: text/markdown
 Requires-Dist: langchain==0.0.340
-Requires-Dist: llama-index==0.9.13
+Requires-Dist: llama-index==0.10.0
 Requires-Dist: websocket-client==1.6.4
 
 # turing-planet星球扩展组件
-+ _版本v0.0.4_
++ _版本v0.0.10_
 
 此模块是星球服务的python扩展组件程序，实现`langchain`和`llamaIndex`的大模型和向量提取接口。
 安装本组件后，用户可以按照`langchain`和`llamaIndex`的api调用星球API服务，完成注入会话，文档问答等功能
 
 ## 主要模块
 - turing_planet.langchain
 
@@ -27,20 +27,21 @@
 
 - turing_planet.llama_index
 
 llama_index 模块扩展，集成方式参照`llamaIndex-说明文档`
 
 ## 环境准备
 
-- 本机安装python3，要求最低3.9+
-- 部署好星球API服务, 版本要求1.2.0_build1026+
-- 安装本类库
+- 本机安装python3，要求3.9
+- 部署好星球服务, 版本要求1.2.0_build1026+
 
 ```shell
-pip install --index-url https://depend.iflytek.com/api/pypi/pypi-repo/simple --extra-index-url https://depend.iflytek.com/api/pypi/hy-pypi-private/simple turing-planet
+pip install turing-planet
+# 如果通过清华镜像无法拉取，尝试以下命令
+pip install turing-planet --index-url https://pypi.org/simple
 ```
 
 
 
 ## 快速开始
 安装`turing-planet`类库后，开始编写你的应用
 
@@ -76,34 +77,23 @@
 
 当然，如果不设置环境变量，也可以通过参数传入。例如
 ```python
 sparkChat = ChatSparkAI(endpoint="127.0.0.1:9980", domain="turing-general")
 ```
 
 **domain说明**
+
     公有云
     xfyun-generalv3.5: V3.5协议
     xfyun-generalv3: V3.0协议
     xfyun-generalv2: V2.0协议
     xfyun-general: V1.5协议
     私有化
     turing-general：通用版本
     turing-iflycode.ge: 私有化代码大模型
     AIUI
     aiui-rewrite-v1: 改写
     aiui-slot-v1: 抽槽
 
 
-## 附录
-
- - 打包
 
-```shell
-python3 setup.py sdist bdist_wheel
-```
 
-- 上传 
-域账号 & 依赖库的密码
-
-```shell
-twine upload --repository-url https://depend.iflytek.com/api/pypi/hy-pypi-private dist/*
-```
```

### Comparing `turing-planet-0.0.9/turing_planet.egg-info/SOURCES.txt` & `turing-planet-0.1.0/turing_planet.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 test/llama_index/optimizing/qa_metadata.py
 test/llama_index/optimizing/summary_index.py
 test/llama_index/optimizing/summary_metadata.py
 test/llama_index/optimizing/turing_knowledge.py
 test/llama_index/optimizing/vector_index.py
 test/llama_index/optimizing/vector_index_cq.py
 test/llama_index/pk/__init__.py
+test/llama_index/pk/base.py
 test/llama_index/pk/llama_index_spark-0131.py
 test/llama_index/pk/pk.py
 test/llama_index/pk/pk_excel_chunsize.py
 test/llama_index/pk/pk_excel_chunsize_rerank.py
 test/llama_index/pk/pk_excel_embedding.py
 test/llama_index/pk/pk_word_0201.py
 test/llama_index/pk/pk_word_es_0201.py
```

