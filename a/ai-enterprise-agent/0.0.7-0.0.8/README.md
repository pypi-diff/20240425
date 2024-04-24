# Comparing `tmp/ai-enterprise-agent-0.0.7.tar.gz` & `tmp/ai_enterprise_agent-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai-enterprise-agent-0.0.7.tar", last modified: Thu Apr 11 21:13:09 2024, max compression
+gzip compressed data, was "ai_enterprise_agent-0.0.8.tar", last modified: Wed Apr 24 22:29:16 2024, max compression
```

## Comparing `ai-enterprise-agent-0.0.7.tar` & `ai_enterprise_agent-0.0.8.tar`

### file list

```diff
@@ -1,52 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:13:09.216196 ai-enterprise-agent-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-11 21:13:04.000000 ai-enterprise-agent-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7620 2024-04-11 21:13:09.216196 ai-enterprise-agent-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-04-11 21:13:04.000000 ai-enterprise-agent-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:13:09.208196 ai-enterprise-agent-0.0.7/ai_enterprise_agent/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 21:13:04.000000 ai-enterprise-agent-0.0.7/ai_enterprise_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-04-11 21:13:04.000000 ai-enterprise-agent-0.0.7/ai_enterprise_agent/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:13:09.208196 ai-enterprise-agent-0.0.7/ai_enterprise_agent/interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 21:13:04.000000 ai-enterprise-agent-0.0.7/ai_enterprise_agent/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-11 21:13:04.000000 ai-enterprise-agent-0.0.7/ai_enterprise_agent/interface/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-11 21:13:04.000000 ai-enterprise-agent-0.0.7/ai_enterprise_agent/interface/chat_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-11 21:13:04.000000 ai-enterprise-agent-0.0.7/ai_enterprise_agent/interface/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-11 21:13:04.000000 ai-enterprise-agent-0.0.7/ai_enterprise_agent/interface/vector_search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:13:09.208196 ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 21:13:04.000000 ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:13:09.212196 ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/chains/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 21:13:04.000000 ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/chains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-11 21:13:04.000000 ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/chains/chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-04-11 21:13:04.000000 ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/chains/open_api_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-11 21:13:04.000000 ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/chains/orchestrator_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-11 21:13:04.000000 ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/chains/sequential_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-11 21:13:04.000000 ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/chains/simple_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-11 21:13:04.000000 ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/chains/sql_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-11 21:13:04.000000 ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/chains/vector_store_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:13:09.212196 ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/chat_history/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 21:13:04.000000 ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/chat_history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-11 21:13:04.000000 ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/chat_history/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-11 21:13:04.000000 ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/chat_history/memory_chat_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-11 21:13:04.000000 ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/chat_history/memory_chat_redis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:13:09.212196 ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/llm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 21:13:04.000000 ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-11 21:13:04.000000 ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/llm/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-11 21:13:04.000000 ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/llm/google.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-11 21:13:04.000000 ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/llm/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:13:09.212196 ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/vector_store/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 21:13:04.000000 ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/vector_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-11 21:13:04.000000 ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/vector_store/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-11 21:13:04.000000 ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/vector_store/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-11 21:13:04.000000 ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/vector_store/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-11 21:13:04.000000 ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/vector_store/pinecone.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-11 21:13:04.000000 ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/vector_store/vector_store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:13:09.212196 ai-enterprise-agent-0.0.7/ai_enterprise_agent/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 21:13:04.000000 ai-enterprise-agent-0.0.7/ai_enterprise_agent/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-11 21:13:04.000000 ai-enterprise-agent-0.0.7/ai_enterprise_agent/utils/fetch_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:13:09.216196 ai-enterprise-agent-0.0.7/ai_enterprise_agent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7620 2024-04-11 21:13:09.000000 ai-enterprise-agent-0.0.7/ai_enterprise_agent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-11 21:13:09.000000 ai-enterprise-agent-0.0.7/ai_enterprise_agent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 21:13:09.000000 ai-enterprise-agent-0.0.7/ai_enterprise_agent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-11 21:13:09.000000 ai-enterprise-agent-0.0.7/ai_enterprise_agent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-11 21:13:09.000000 ai-enterprise-agent-0.0.7/ai_enterprise_agent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 21:13:09.216196 ai-enterprise-agent-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-04-11 21:13:04.000000 ai-enterprise-agent-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:16.861020 ai_enterprise_agent-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7620 2024-04-24 22:29:16.861020 ai_enterprise_agent-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:16.853021 ai_enterprise_agent-0.0.8/ai_enterprise_agent/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:16.853021 ai_enterprise_agent-0.0.8/ai_enterprise_agent/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/interface/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/interface/chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/interface/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/interface/vector_search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:16.853021 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:16.853021 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chains/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chains/chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chains/open_api_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chains/orchestrator_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chains/sequential_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chains/simple_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chains/sql_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chains/vector_store_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:16.853021 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chat_history/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chat_history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chat_history/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chat_history/memory_chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chat_history/memory_chat_redis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:16.857020 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/ingestion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/ingestion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/ingestion/csv_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/ingestion/ingestion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/ingestion/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/ingestion/msft_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/ingestion/pdf_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/ingestion/txt_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:16.857020 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/llm/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/llm/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/llm/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:16.857020 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/vector_store/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/vector_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/vector_store/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/vector_store/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/vector_store/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/vector_store/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/vector_store/vector_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:16.857020 ai_enterprise_agent-0.0.8/ai_enterprise_agent/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/utils/fetch_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:16.861020 ai_enterprise_agent-0.0.8/ai_enterprise_agent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7620 2024-04-24 22:29:16.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-24 22:29:16.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 22:29:16.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-24 22:29:16.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-24 22:29:16.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 22:29:16.861020 ai_enterprise_agent-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/setup.py
```

### Comparing `ai-enterprise-agent-0.0.7/LICENSE` & `ai_enterprise_agent-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.7/PKG-INFO` & `ai_enterprise_agent-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-enterprise-agent
-Version: 0.0.7
+Version: 0.0.8
 Summary: AI Agent simplifies the implementation and use of generative AI with LangChain.
 Author: Author
 Author-email: autor@autor.com.br
 License: Apache 2.0 License
 Keywords: ai ai-agent agent assistant enterprise
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `ai-enterprise-agent-0.0.7/README.md` & `ai_enterprise_agent-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.7/ai_enterprise_agent/agent.py` & `ai_enterprise_agent-0.0.8/ai_enterprise_agent/agent.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.7/ai_enterprise_agent/interface/chat_history.py` & `ai_enterprise_agent-0.0.8/ai_enterprise_agent/interface/chat_history.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.7/ai_enterprise_agent/interface/settings.py` & `ai_enterprise_agent-0.0.8/ai_enterprise_agent/interface/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,9 +116,9 @@
     model: IModel
     chains: List[CHAIN_TYPE]
     processing_type: PROCESSING_TYPE
     database: Optional[IDatabase]
     open_api: Optional[IOpenApi]
     vector_store: Optional[IVectorSearch]
     history: Optional[IChatHistory]
-    document_intelligence: Optional[DOCUMENT_INTELLIGENCE_TYPE]
+    document_intelligence: Optional[IDocumentIntelligence]
     system: ISystem
```

### Comparing `ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/chains/chain.py` & `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chains/chain.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/chains/open_api_chain.py` & `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chains/open_api_chain.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     open_api = self.open_api
     schema = open_api.get('data')
     template = """
       You are an AI with expertise in OpenAPI and Swagger.
       You should follow the following rules when generating an answer:
       - Only execute the request on the service if the question is not in History, if the question has already been answered, use the same answer and do not make a request on the service.
       - The response must be a JSON object containing an url, content type, method, and data, without triple quotes, json string on start and the end.
+      - Remember add header parameters on the JSON request object.
       {custom_system_message}
       -------------------------------------------\n
       Schema: {schema}\n
       -------------------------------------------\n
       History: {history}\n
       -------------------------------------------\n
       Question: {question}\n
@@ -58,15 +59,15 @@
     prompt = ChatPromptTemplate.from_template(template)
     chain = prompt | self.model | StrOutputParser()
     return chain.invoke({"schema": schema, "question": question, "history": self.memory.get_messages(), "custom_system_message": custom_system_message})
 
   def chain(self, question, custom_system_message) -> RunnableSerializable[Any, Any]:
     fetch_sentence = self.get_fetch(question, custom_system_message)
     request = json.loads(fetch_sentence)
-    response = fetch(url=request.get('url'), method=request.get('method'), data=request.get('data'), headers={})
+    response = fetch(url=request.get('url'), method=request.get('method'), data=request.get('data'), headers=request.get('headers'))
     template = """
         Based on the context below, answer the question with natural language.
         You should follow the following rules when generating and answer:
         - Only attempt to answer if a question was posed.
         - Always answer the question in the language in which the question was asked.
         Context: {context}
         Question: {question}
```

### Comparing `ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/chains/orchestrator_chain.py` & `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chains/orchestrator_chain.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/chains/sequential_chain.py` & `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chains/sequential_chain.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/chains/simple_chain.py` & `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chains/simple_chain.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/chains/sql_chain.py` & `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chains/sql_chain.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/chains/vector_store_chain.py` & `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chains/vector_store_chain.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/chat_history/memory.py` & `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chat_history/memory.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/chat_history/memory_chat_history.py` & `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chat_history/memory_chat_history.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/chat_history/memory_chat_redis.py` & `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chat_history/memory_chat_redis.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/llm/azure.py` & `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/llm/azure.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/llm/google.py` & `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/llm/google.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/llm/model.py` & `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/llm/model.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/vector_store/aws.py` & `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/vector_store/aws.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/vector_store/azure.py` & `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/vector_store/azure.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,32 +27,33 @@
 
   def build(self):
     config = self.config.get('vector_store')
     embeddings = EmbeddingFactory.build(VECTOR_STORE_TYPE.azure_search, self.config)
 
     fields = [
       SimpleField(name='id', type=SearchFieldDataType.String, key=True, filterable=True),
-      SearchableField(name=config.get('fields_content'), type=SearchFieldDataType.String),
-      SearchField(name=config.get('fields_content_vector'), type=SearchFieldDataType.Collection(SearchFieldDataType.Single), searchable=True, vector_search_dimensions=len(embeddings.embed_query("Text")), vector_search_profile_name=config.get('vector_search_profile_name')),
+      SearchableField(name=config.get('fields_content', 'content'), type=SearchFieldDataType.String),
+      SearchField(name=config.get('fields_content_vector', 'content_vector'), type=SearchFieldDataType.Collection(SearchFieldDataType.Single), searchable=True, vector_search_dimensions=len(embeddings.embed_query("Text")), vector_search_profile_name=config.get('vector_search_profile_name')),
       SearchableField(name='metadata', type=SearchFieldDataType.String),
     ]
 
     return AzureSearch(
       azure_search_endpoint=config.get('endpoint'),
       azure_search_key=config.get('api_key'),
       index_name=config.get('index_name'),
       embedding_function=embeddings.embed_query,
       fields=fields
     )
 
-  def similarity_search(self, query: str, k: int = 4, search_type: ISearchType = ISearchType.similarity) -> List[Document]:
+  def similarity_search(self, query: str, k: int = 4, search_type: ISearchType = ISearchType.similarity, filters:str = None) -> List[Document]:
     return self.vector_store.similarity_search(
       query=query,
       k=k,
-      search_type=search_type
+      search_type=search_type,
+      filters=filters
     )
 
   def similarity_search_with_relevance_scores(self, query: str,  score_threshold: float, k: Optional[int]) -> List[Tuple[Document, float]]:
     return self.vector_store.similarity_search_with_relevance_scores(
       query=query,
       k=k,
       score_threshold=score_threshold,
```

### Comparing `ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/vector_store/embedding.py` & `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/vector_store/embedding.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/vector_store/pinecone.py` & `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/vector_store/pinecone.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.7/ai_enterprise_agent/services/vector_store/vector_store.py` & `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/vector_store/vector_store.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.7/ai_enterprise_agent/utils/fetch_helper.py` & `ai_enterprise_agent-0.0.8/ai_enterprise_agent/utils/fetch_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         headers (Dict[str, str], opcional): Os cabeçalhos da solicitação. Padrão é None.
 
     Returns:
         Dict[str, Any] or None: Os dados da resposta JSON, se a solicitação for bem-sucedida. None caso contrário.
     """
     try:
         if method.upper() == 'GET':
-            response = requests.get(url, headers=headers)
+            response = requests.get(url, json=data, headers=headers)
         elif method.upper() == 'POST':
             response = requests.post(url, json=data, headers=headers)
         else:
             raise ValueError("Método HTTP inválido. Use 'GET' ou 'POST'.")
 
         response.raise_for_status()
         return response.json()
```

### Comparing `ai-enterprise-agent-0.0.7/ai_enterprise_agent.egg-info/PKG-INFO` & `ai_enterprise_agent-0.0.8/ai_enterprise_agent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-enterprise-agent
-Version: 0.0.7
+Version: 0.0.8
 Summary: AI Agent simplifies the implementation and use of generative AI with LangChain.
 Author: Author
 Author-email: autor@autor.com.br
 License: Apache 2.0 License
 Keywords: ai ai-agent agent assistant enterprise
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `ai-enterprise-agent-0.0.7/ai_enterprise_agent.egg-info/SOURCES.txt` & `ai_enterprise_agent-0.0.8/ai_enterprise_agent.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,21 @@
 ./ai_enterprise_agent/services/chains/simple_chain.py
 ./ai_enterprise_agent/services/chains/sql_chain.py
 ./ai_enterprise_agent/services/chains/vector_store_chain.py
 ./ai_enterprise_agent/services/chat_history/__init__.py
 ./ai_enterprise_agent/services/chat_history/memory.py
 ./ai_enterprise_agent/services/chat_history/memory_chat_history.py
 ./ai_enterprise_agent/services/chat_history/memory_chat_redis.py
+./ai_enterprise_agent/services/ingestion/__init__.py
+./ai_enterprise_agent/services/ingestion/csv_loader.py
+./ai_enterprise_agent/services/ingestion/ingestion.py
+./ai_enterprise_agent/services/ingestion/loader.py
+./ai_enterprise_agent/services/ingestion/msft_loader.py
+./ai_enterprise_agent/services/ingestion/pdf_loader.py
+./ai_enterprise_agent/services/ingestion/txt_loader.py
 ./ai_enterprise_agent/services/llm/__init__.py
 ./ai_enterprise_agent/services/llm/azure.py
 ./ai_enterprise_agent/services/llm/google.py
 ./ai_enterprise_agent/services/llm/model.py
 ./ai_enterprise_agent/services/vector_store/__init__.py
 ./ai_enterprise_agent/services/vector_store/aws.py
 ./ai_enterprise_agent/services/vector_store/azure.py
```

### Comparing `ai-enterprise-agent-0.0.7/ai_enterprise_agent.egg-info/requires.txt` & `ai_enterprise_agent-0.0.8/ai_enterprise_agent.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.7/setup.py` & `ai_enterprise_agent-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(name='ai-enterprise-agent',
-    version='0.0.7',
+    version='0.0.8',
     license='Apache 2.0 License',
     author='Author',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='autor@autor.com.br',
     keywords='ai ai-agent agent assistant enterprise',
     description='AI Agent simplifies the implementation and use of generative AI with LangChain.',
-    packages=['ai_enterprise_agent', 'ai_enterprise_agent.interface', 'ai_enterprise_agent.services','ai_enterprise_agent.services.chains', 'ai_enterprise_agent.services.chat_history', 'ai_enterprise_agent.services.llm', 'ai_enterprise_agent.services.vector_store', 'ai_enterprise_agent.utils'],
+    packages=['ai_enterprise_agent', 'ai_enterprise_agent.interface', 'ai_enterprise_agent.services','ai_enterprise_agent.services.chains', 'ai_enterprise_agent.services.chat_history', 'ai_enterprise_agent.services.llm', 'ai_enterprise_agent.services.ingestion', 'ai_enterprise_agent.services.vector_store', 'ai_enterprise_agent.utils'],
     python_requires='>=3.9',
-    package_dir={'': '.', 'ai_enterprise_agent': './ai_enterprise_agent', 'ai_enterprise_agent.interface': './ai_enterprise_agent/interface', 'ai_enterprise_agent.services': './ai_enterprise_agent/services', 'ai_enterprise_agent.services.chains': './ai_enterprise_agent/services/chains', 'ai_enterprise_agent.services.chat_history': './ai_enterprise_agent/services/chat_history', 'ai_enterprise_agent.services.llm': './ai_enterprise_agent/services/llm', 'ai_enterprise_agent.services.vector_store': './ai_enterprise_agent/services/vector_store', 'ai_enterprise_agent.utils': './ai_enterprise_agent/utils'},
+    package_dir={'': '.', 'ai_enterprise_agent': './ai_enterprise_agent', 'ai_enterprise_agent.interface': './ai_enterprise_agent/interface', 'ai_enterprise_agent.services': './ai_enterprise_agent/services', 'ai_enterprise_agent.services.chains': './ai_enterprise_agent/services/chains', 'ai_enterprise_agent.services.chat_history': './ai_enterprise_agent/services/chat_history', 'ai_enterprise_agent.services.llm': './ai_enterprise_agent/services/llm', 'ai_enterprise_agent.services.vector_store': './ai_enterprise_agent/services/vector_store', 'ai_enterprise_agent.services.ingestion': './ai_enterprise_agent/services/ingestion','ai_enterprise_agent.utils': './ai_enterprise_agent/utils'},
     install_requires=[
       'aiohttp==3.9.3',
       'aiosignal==1.3.1',
       'annotated-types==0.6.0',
       'anyio==4.3.0',
       'attrs==23.2.0',
       'azure-ai-documentintelligence==1.0.0b3',
```

