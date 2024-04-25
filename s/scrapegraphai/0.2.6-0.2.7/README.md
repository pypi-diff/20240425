# Comparing `tmp/scrapegraphai-0.2.6.tar.gz` & `tmp/scrapegraphai-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapegraphai-0.2.6.tar", max compression
+gzip compressed data, was "scrapegraphai-0.2.7.tar", max compression
```

## Comparing `scrapegraphai-0.2.6.tar` & `scrapegraphai-0.2.7.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1065 2024-03-03 14:00:51.183606 scrapegraphai-0.2.6/LICENSE
--rw-r--r--   0        0        0     7784 2024-04-20 20:58:42.211169 scrapegraphai-0.2.6/README.md
--rw-r--r--   0        0        0     1644 2024-04-21 18:19:33.070264 scrapegraphai-0.2.6/pyproject.toml
--rw-r--r--   0        0        0       54 2024-03-03 14:00:51.196394 scrapegraphai-0.2.6/scrapegraphai/__init__.py
--rw-r--r--   0        0        0       90 2024-03-03 14:00:51.196546 scrapegraphai-0.2.6/scrapegraphai/builders/__init__.py
--rw-r--r--   0        0        0     6670 2024-03-24 19:34:24.965713 scrapegraphai-0.2.6/scrapegraphai/builders/graph_builder.py
--rw-r--r--   0        0        0      258 2024-04-20 20:58:42.218942 scrapegraphai-0.2.6/scrapegraphai/graphs/__init__.py
--rw-r--r--   0        0        0     3623 2024-04-20 20:58:42.219086 scrapegraphai-0.2.6/scrapegraphai/graphs/abstract_graph.py
--rw-r--r--   0        0        0     4644 2024-04-20 20:58:42.219311 scrapegraphai-0.2.6/scrapegraphai/graphs/base_graph.py
--rw-r--r--   0        0        0     2494 2024-04-20 20:58:42.219422 scrapegraphai-0.2.6/scrapegraphai/graphs/script_creator_graph.py
--rw-r--r--   0        0        0     2191 2024-04-12 10:59:59.484979 scrapegraphai-0.2.6/scrapegraphai/graphs/search_graph.py
--rw-r--r--   0        0        0     2380 2024-04-20 20:58:42.219513 scrapegraphai-0.2.6/scrapegraphai/graphs/smart_scraper_graph.py
--rw-r--r--   0        0        0     3120 2024-04-20 20:58:42.219606 scrapegraphai-0.2.6/scrapegraphai/graphs/speech_graph.py
--rw-r--r--   0        0        0      164 2024-03-03 14:00:51.197634 scrapegraphai-0.2.6/scrapegraphai/helpers/__init__.py
--rw-r--r--   0        0        0      756 2024-04-21 15:12:37.105821 scrapegraphai-0.2.6/scrapegraphai/helpers/models_tokens.py
--rw-r--r--   0        0        0     3807 2024-04-09 11:20:43.626222 scrapegraphai-0.2.6/scrapegraphai/helpers/nodes_metadata.py
--rw-r--r--   0        0        0     2363 2024-04-08 20:25:15.266957 scrapegraphai-0.2.6/scrapegraphai/helpers/schemas.py
--rw-r--r--   0        0        0      290 2024-04-12 10:59:59.485515 scrapegraphai-0.2.6/scrapegraphai/models/__init__.py
--rw-r--r--   0        0        0      601 2024-04-09 11:20:43.626608 scrapegraphai-0.2.6/scrapegraphai/models/azure_openai.py
--rw-r--r--   0        0        0      651 2024-04-08 20:25:27.931161 scrapegraphai-0.2.6/scrapegraphai/models/gemini.py
--rw-r--r--   0        0        0      839 2024-04-12 10:59:59.485625 scrapegraphai-0.2.6/scrapegraphai/models/hugging_face.py
--rw-r--r--   0        0        0      590 2024-04-08 20:25:35.475199 scrapegraphai-0.2.6/scrapegraphai/models/ollama.py
--rw-r--r--   0        0        0      575 2024-04-08 20:25:42.545477 scrapegraphai-0.2.6/scrapegraphai/models/openai.py
--rw-r--r--   0        0        0     1721 2024-04-08 20:25:31.195250 scrapegraphai-0.2.6/scrapegraphai/models/openai_itt.py
--rw-r--r--   0        0        0     1657 2024-04-08 20:25:37.349894 scrapegraphai-0.2.6/scrapegraphai/models/openai_tts.py
--rw-r--r--   0        0        0      503 2024-04-20 20:58:42.219766 scrapegraphai-0.2.6/scrapegraphai/nodes/__init__.py
--rw-r--r--   0        0        0     7544 2024-04-08 20:25:53.786578 scrapegraphai-0.2.6/scrapegraphai/nodes/base_node.py
--rw-r--r--   0        0        0     2914 2024-04-20 20:58:42.219990 scrapegraphai-0.2.6/scrapegraphai/nodes/conditional_node.py
--rw-r--r--   0        0        0     3375 2024-04-20 20:58:42.220349 scrapegraphai-0.2.6/scrapegraphai/nodes/fetch_node.py
--rw-r--r--   0        0        0     6893 2024-04-20 20:58:42.220641 scrapegraphai-0.2.6/scrapegraphai/nodes/generate_answer_node.py
--rw-r--r--   0        0        0     7249 2024-04-20 20:58:42.220842 scrapegraphai-0.2.6/scrapegraphai/nodes/generate_scraper_node.py
--rw-r--r--   0        0        0     4097 2024-04-20 20:58:42.221320 scrapegraphai-0.2.6/scrapegraphai/nodes/get_probable_tags_node.py
--rw-r--r--   0        0        0     1592 2024-04-20 20:58:42.221535 scrapegraphai-0.2.6/scrapegraphai/nodes/image_to_text_node.py
--rw-r--r--   0        0        0     3337 2024-04-20 20:58:42.221690 scrapegraphai-0.2.6/scrapegraphai/nodes/parse_node.py
--rw-r--r--   0        0        0     5177 2024-04-21 09:27:38.253618 scrapegraphai-0.2.6/scrapegraphai/nodes/rag_node.py
--rw-r--r--   0        0        0     4545 2024-04-20 20:58:42.222355 scrapegraphai-0.2.6/scrapegraphai/nodes/search_internet_node.py
--rw-r--r--   0        0        0     1635 2024-04-20 20:58:42.222570 scrapegraphai-0.2.6/scrapegraphai/nodes/text_to_speech_node.py
--rw-r--r--   0        0        0      242 2024-04-12 10:55:27.494820 scrapegraphai-0.2.6/scrapegraphai/utils/__init__.py
--rw-r--r--   0        0        0     1856 2024-04-03 10:39:06.250892 scrapegraphai-0.2.6/scrapegraphai/utils/convert_to_csv.py
--rw-r--r--   0        0        0     1437 2024-04-03 10:39:06.251121 scrapegraphai-0.2.6/scrapegraphai/utils/convert_to_json.py
--rw-r--r--   0        0        0     3630 2024-04-06 12:43:33.712449 scrapegraphai-0.2.6/scrapegraphai/utils/parse_state_keys.py
--rw-r--r--   0        0        0     1504 2024-04-12 11:30:08.598599 scrapegraphai-0.2.6/scrapegraphai/utils/prettify_exec_info.py
--rw-r--r--   0        0        0     1070 2024-04-20 20:58:42.222753 scrapegraphai-0.2.6/scrapegraphai/utils/remover.py
--rw-r--r--   0        0        0     1118 2024-04-06 12:46:22.008255 scrapegraphai-0.2.6/scrapegraphai/utils/research_web.py
--rw-r--r--   0        0        0      631 2024-04-06 12:44:50.349656 scrapegraphai-0.2.6/scrapegraphai/utils/save_audio_from_bytes.py
--rw-r--r--   0        0        0      990 2024-03-18 13:23:59.117686 scrapegraphai-0.2.6/scrapegraphai/utils/token_calculator.py
--rw-r--r--   0        0        0     9409 1970-01-01 00:00:00.000000 scrapegraphai-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-03-03 14:00:51.183606 scrapegraphai-0.2.7/LICENSE
+-rw-r--r--   0        0        0     7907 2024-04-25 10:10:10.131040 scrapegraphai-0.2.7/README.md
+-rw-r--r--   0        0        0     1644 2024-04-25 10:10:20.262032 scrapegraphai-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-03-03 14:00:51.196394 scrapegraphai-0.2.7/scrapegraphai/__init__.py
+-rw-r--r--   0        0        0       90 2024-03-03 14:00:51.196546 scrapegraphai-0.2.7/scrapegraphai/builders/__init__.py
+-rw-r--r--   0        0        0     6670 2024-03-24 19:34:24.965713 scrapegraphai-0.2.7/scrapegraphai/builders/graph_builder.py
+-rw-r--r--   0        0        0      258 2024-04-20 20:58:42.218942 scrapegraphai-0.2.7/scrapegraphai/graphs/__init__.py
+-rw-r--r--   0        0        0     3623 2024-04-25 10:10:10.154362 scrapegraphai-0.2.7/scrapegraphai/graphs/abstract_graph.py
+-rw-r--r--   0        0        0     4644 2024-04-25 07:16:29.915661 scrapegraphai-0.2.7/scrapegraphai/graphs/base_graph.py
+-rw-r--r--   0        0        0     2494 2024-04-25 10:10:10.154636 scrapegraphai-0.2.7/scrapegraphai/graphs/script_creator_graph.py
+-rw-r--r--   0        0        0     2191 2024-04-12 10:59:59.484979 scrapegraphai-0.2.7/scrapegraphai/graphs/search_graph.py
+-rw-r--r--   0        0        0     2380 2024-04-20 20:58:42.219513 scrapegraphai-0.2.7/scrapegraphai/graphs/smart_scraper_graph.py
+-rw-r--r--   0        0        0     3120 2024-04-20 20:58:42.219606 scrapegraphai-0.2.7/scrapegraphai/graphs/speech_graph.py
+-rw-r--r--   0        0        0      164 2024-04-25 07:16:29.916420 scrapegraphai-0.2.7/scrapegraphai/helpers/__init__.py
+-rw-r--r--   0        0        0      829 2024-04-25 10:10:10.154906 scrapegraphai-0.2.7/scrapegraphai/helpers/models_tokens.py
+-rw-r--r--   0        0        0     3807 2024-04-09 11:20:43.626222 scrapegraphai-0.2.7/scrapegraphai/helpers/nodes_metadata.py
+-rw-r--r--   0        0        0     2363 2024-04-08 20:25:15.266957 scrapegraphai-0.2.7/scrapegraphai/helpers/schemas.py
+-rw-r--r--   0        0        0      290 2024-04-12 10:59:59.485515 scrapegraphai-0.2.7/scrapegraphai/models/__init__.py
+-rw-r--r--   0        0        0      601 2024-04-09 11:20:43.626608 scrapegraphai-0.2.7/scrapegraphai/models/azure_openai.py
+-rw-r--r--   0        0        0      651 2024-04-08 20:25:27.931161 scrapegraphai-0.2.7/scrapegraphai/models/gemini.py
+-rw-r--r--   0        0        0      839 2024-04-12 10:59:59.485625 scrapegraphai-0.2.7/scrapegraphai/models/hugging_face.py
+-rw-r--r--   0        0        0      590 2024-04-08 20:25:35.475199 scrapegraphai-0.2.7/scrapegraphai/models/ollama.py
+-rw-r--r--   0        0        0      575 2024-04-08 20:25:42.545477 scrapegraphai-0.2.7/scrapegraphai/models/openai.py
+-rw-r--r--   0        0        0     1721 2024-04-08 20:25:31.195250 scrapegraphai-0.2.7/scrapegraphai/models/openai_itt.py
+-rw-r--r--   0        0        0     1657 2024-04-08 20:25:37.349894 scrapegraphai-0.2.7/scrapegraphai/models/openai_tts.py
+-rw-r--r--   0        0        0      503 2024-04-25 07:16:29.917364 scrapegraphai-0.2.7/scrapegraphai/nodes/__init__.py
+-rw-r--r--   0        0        0     7544 2024-04-08 20:25:53.786578 scrapegraphai-0.2.7/scrapegraphai/nodes/base_node.py
+-rw-r--r--   0        0        0     2914 2024-04-20 20:58:42.219990 scrapegraphai-0.2.7/scrapegraphai/nodes/conditional_node.py
+-rw-r--r--   0        0        0     3375 2024-04-25 10:10:10.155199 scrapegraphai-0.2.7/scrapegraphai/nodes/fetch_node.py
+-rw-r--r--   0        0        0     6893 2024-04-24 08:02:38.694607 scrapegraphai-0.2.7/scrapegraphai/nodes/generate_answer_node.py
+-rw-r--r--   0        0        0     7236 2024-04-25 10:10:10.155594 scrapegraphai-0.2.7/scrapegraphai/nodes/generate_scraper_node.py
+-rw-r--r--   0        0        0     4097 2024-04-20 20:58:42.221320 scrapegraphai-0.2.7/scrapegraphai/nodes/get_probable_tags_node.py
+-rw-r--r--   0        0        0     1592 2024-04-20 20:58:42.221535 scrapegraphai-0.2.7/scrapegraphai/nodes/image_to_text_node.py
+-rw-r--r--   0        0        0     3337 2024-04-20 20:58:42.221690 scrapegraphai-0.2.7/scrapegraphai/nodes/parse_node.py
+-rw-r--r--   0        0        0     5177 2024-04-25 10:10:10.156010 scrapegraphai-0.2.7/scrapegraphai/nodes/rag_node.py
+-rw-r--r--   0        0        0     4507 2024-04-25 10:10:10.156452 scrapegraphai-0.2.7/scrapegraphai/nodes/search_internet_node.py
+-rw-r--r--   0        0        0     1635 2024-04-22 19:30:38.104934 scrapegraphai-0.2.7/scrapegraphai/nodes/text_to_speech_node.py
+-rw-r--r--   0        0        0      242 2024-04-12 10:55:27.494820 scrapegraphai-0.2.7/scrapegraphai/utils/__init__.py
+-rw-r--r--   0        0        0     1742 2024-04-25 10:10:10.156867 scrapegraphai-0.2.7/scrapegraphai/utils/convert_to_csv.py
+-rw-r--r--   0        0        0     1443 2024-04-25 10:10:10.157249 scrapegraphai-0.2.7/scrapegraphai/utils/convert_to_json.py
+-rw-r--r--   0        0        0     3630 2024-04-06 12:43:33.712449 scrapegraphai-0.2.7/scrapegraphai/utils/parse_state_keys.py
+-rw-r--r--   0        0        0     1504 2024-04-12 11:30:08.598599 scrapegraphai-0.2.7/scrapegraphai/utils/prettify_exec_info.py
+-rw-r--r--   0        0        0     1070 2024-04-25 10:10:10.157483 scrapegraphai-0.2.7/scrapegraphai/utils/remover.py
+-rw-r--r--   0        0        0     1118 2024-04-06 12:46:22.008255 scrapegraphai-0.2.7/scrapegraphai/utils/research_web.py
+-rw-r--r--   0        0        0      631 2024-04-06 12:44:50.349656 scrapegraphai-0.2.7/scrapegraphai/utils/save_audio_from_bytes.py
+-rw-r--r--   0        0        0      990 2024-03-18 13:23:59.117686 scrapegraphai-0.2.7/scrapegraphai/utils/token_calculator.py
+-rw-r--r--   0        0        0     9532 1970-01-01 00:00:00.000000 scrapegraphai-0.2.7/PKG-INFO
```

### Comparing `scrapegraphai-0.2.6/LICENSE` & `scrapegraphai-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.6/README.md` & `scrapegraphai-0.2.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 
 # 🕷️ ScrapeGraphAI: You Only Scrape Once
 [![Downloads](https://static.pepy.tech/badge/scrapegraphai)](https://pepy.tech/project/scrapegraphai)
 [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
 [![Pylint](https://github.com/VinciGit00/Scrapegraph-ai/actions/workflows/pylint.yml/badge.svg)](https://github.com/VinciGit00/Scrapegraph-ai/actions/workflows/pylint.yml)
+[![CodeQL](https://github.com/VinciGit00/Scrapegraph-ai/actions/workflows/codeql.yml/badge.svg)](https://github.com/VinciGit00/Scrapegraph-ai/actions/workflows/codeql.yml)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![](https://dcbadge.vercel.app/api/server/gkxQDAjfeX)](https://discord.gg/gkxQDAjfeX)
 
 
 ScrapeGraphAI is a *web scraping* python library that uses LLM and direct graph logic to create scraping pipelines for websites, documents and XML files.
 Just say which information you want to extract and the library will do it for you!
 
@@ -49,20 +50,19 @@
 from scrapegraphai.graphs import SmartScraperGraph
 
 graph_config = {
     "llm": {
         "model": "ollama/mistral",
         "temperature": 0,
         "format": "json",  # Ollama needs the format to be specified explicitly
-        "base_url": "http://localhost:11434",  # set Ollama URL arbitrarily
+        "base_url": "http://localhost:11434",  # set Ollama URL
     },
     "embeddings": {
         "model": "ollama/nomic-embed-text",
-        "temperature": 0,
-        "base_url": "http://localhost:11434",  # set Ollama URL arbitrarily
+        "base_url": "http://localhost:11434",  # set Ollama URL
     }
 }
 
 smart_scraper_graph = SmartScraperGraph(
     prompt="List me all the articles",
     # also accepts a string with the already downloaded HTML code
     source="https://perinim.github.io/projects",
@@ -75,15 +75,15 @@
 ```
 
 ### Case 2: Extracting information using Docker
 
 Note: before using the local model remember to create the docker container!
 ```text
     docker-compose up -d
-    docker exec -it ollama ollama run stablelm-zephyr
+    docker exec -it ollama ollama pull stablelm-zephyr
 ```
 You can use which models avaiable on Ollama or your own model instead of stablelm-zephyr
 ```python
 from scrapegraphai.graphs import SmartScraperGraph
 
 graph_config = {
     "llm": {
```

### Comparing `scrapegraphai-0.2.6/pyproject.toml` & `scrapegraphai-0.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scrapegraphai"
-version = "0.2.6"
+version = "0.2.7"
 description = "A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines."
 authors = [
     "Marco Vinciguerra <mvincig11@gmail.com>",
     "Marco Perini <perinim.98@gmail.com>",
     "Lorenzo Padoan <lorenzo.padoan977@gmail.com>"
 ]
 license = "MIT"
```

### Comparing `scrapegraphai-0.2.6/scrapegraphai/builders/graph_builder.py` & `scrapegraphai-0.2.7/scrapegraphai/builders/graph_builder.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.6/scrapegraphai/graphs/abstract_graph.py` & `scrapegraphai-0.2.7/scrapegraphai/graphs/abstract_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.6/scrapegraphai/graphs/base_graph.py` & `scrapegraphai-0.2.7/scrapegraphai/graphs/base_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.6/scrapegraphai/graphs/script_creator_graph.py` & `scrapegraphai-0.2.7/scrapegraphai/graphs/script_creator_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.6/scrapegraphai/graphs/search_graph.py` & `scrapegraphai-0.2.7/scrapegraphai/graphs/search_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.6/scrapegraphai/graphs/smart_scraper_graph.py` & `scrapegraphai-0.2.7/scrapegraphai/graphs/smart_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.6/scrapegraphai/graphs/speech_graph.py` & `scrapegraphai-0.2.7/scrapegraphai/graphs/speech_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.6/scrapegraphai/helpers/models_tokens.py` & `scrapegraphai-0.2.7/scrapegraphai/helpers/models_tokens.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,14 +5,16 @@
     "openai": {
         "gpt-3.5-turbo-0125": 16385,
         "gpt-3.5-turbo": 4096,
         "gpt-3.5-turbo-1106": 16385,
         "gpt-3.5-turbo-instruct": 4096,
         "gpt-4-0125-preview": 128000,
         "gpt-4-turbo-preview": 128000,
+        "gpt-4-turbo": 128000,
+        "gpt-4-turbo-2024-04-09": 128000,
         "gpt-4-1106-preview": 128000,
         "gpt-4-vision-preview": 128000,
         "gpt-4": 8192,
         "gpt-4-0613": 8192,
         "gpt-4-32k": 32768,
         "gpt-4-32k-0613": 32768,
     },
```

### Comparing `scrapegraphai-0.2.6/scrapegraphai/helpers/nodes_metadata.py` & `scrapegraphai-0.2.7/scrapegraphai/helpers/nodes_metadata.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.6/scrapegraphai/helpers/schemas.py` & `scrapegraphai-0.2.7/scrapegraphai/helpers/schemas.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.6/scrapegraphai/models/azure_openai.py` & `scrapegraphai-0.2.7/scrapegraphai/models/azure_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.6/scrapegraphai/models/gemini.py` & `scrapegraphai-0.2.7/scrapegraphai/models/gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.6/scrapegraphai/models/hugging_face.py` & `scrapegraphai-0.2.7/scrapegraphai/models/hugging_face.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.6/scrapegraphai/models/ollama.py` & `scrapegraphai-0.2.7/scrapegraphai/models/ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.6/scrapegraphai/models/openai.py` & `scrapegraphai-0.2.7/scrapegraphai/models/openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.6/scrapegraphai/models/openai_itt.py` & `scrapegraphai-0.2.7/scrapegraphai/models/openai_itt.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.6/scrapegraphai/models/openai_tts.py` & `scrapegraphai-0.2.7/scrapegraphai/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.6/scrapegraphai/nodes/base_node.py` & `scrapegraphai-0.2.7/scrapegraphai/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.6/scrapegraphai/nodes/conditional_node.py` & `scrapegraphai-0.2.7/scrapegraphai/nodes/conditional_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.6/scrapegraphai/nodes/fetch_node.py` & `scrapegraphai-0.2.7/scrapegraphai/nodes/fetch_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.6/scrapegraphai/nodes/generate_answer_node.py` & `scrapegraphai-0.2.7/scrapegraphai/nodes/generate_answer_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.6/scrapegraphai/nodes/generate_scraper_node.py` & `scrapegraphai-0.2.7/scrapegraphai/nodes/generate_scraper_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     """
     A node that generates an answer using a language model (LLM) based on the user's input
     and the content extracted from a webpage. It constructs a prompt from the user's input
     and the scraped content, feeds it to the LLM, and parses the LLM's response to produce
     an answer.
 
     Attributes:
-        llm (ChatOpenAI): An instance of a language model client, configured for generating answers.
+        llm: An instance of a language model client, configured for generating answers.
         node_name (str): The unique identifier name for the node, defaulting 
         to "GenerateScraperNode".
         node_type (str): The type of the node, set to "node" indicating a 
         standard operational node.
 
     Args:
         llm: An instance of the language model client (e.g., ChatOpenAI) used
```

### Comparing `scrapegraphai-0.2.6/scrapegraphai/nodes/get_probable_tags_node.py` & `scrapegraphai-0.2.7/scrapegraphai/nodes/get_probable_tags_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.6/scrapegraphai/nodes/image_to_text_node.py` & `scrapegraphai-0.2.7/scrapegraphai/nodes/image_to_text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.6/scrapegraphai/nodes/parse_node.py` & `scrapegraphai-0.2.7/scrapegraphai/nodes/parse_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.6/scrapegraphai/nodes/rag_node.py` & `scrapegraphai-0.2.7/scrapegraphai/nodes/rag_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.6/scrapegraphai/nodes/search_internet_node.py` & `scrapegraphai-0.2.7/scrapegraphai/nodes/search_internet_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 
     Args:
         input (str): The user input used to construct the prompt.
         output (List[str]): The keys in the state dictionary where the
                              generated answer will be stored.
         model_config (dict): Configuration parameters for the language model client.
         node_name (str, optional): The unique identifier name for the node. 
-        Defaults to "GenerateAnswer".
 
     Methods:
         execute(state): Processes the input and document from the state to generate an answer,
                         updating the state with the generated answer under the 'answer' key.
     """
 
     def __init__(self, input: str, output: List[str], node_config: dict,
```

### Comparing `scrapegraphai-0.2.6/scrapegraphai/nodes/text_to_speech_node.py` & `scrapegraphai-0.2.7/scrapegraphai/nodes/text_to_speech_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.6/scrapegraphai/utils/convert_to_csv.py` & `scrapegraphai-0.2.7/scrapegraphai/utils/convert_to_csv.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,28 +8,26 @@
 
 def convert_to_csv(data: dict, filename: str, position: str = None):
     """
     Converts a dictionary to a CSV file and saves it.
 
     Args:
     data (dict): Data to be converted to CSV.
-    filename (str): Name of the CSV file (without the .csv extension).
     position (str): Optional path where the file should be saved. If not provided,
     the directory of the caller script will be used.
 
     Raises:
-    ValueError: If the filename contains '.csv'.
     FileNotFoundError: If the specified directory does not exist.
     PermissionError: If the program lacks write permission for the directory.
     TypeError: If the input data is not a dictionary.
     Exception: For other potential errors during DataFrame creation or CSV saving.
     """
 
     if ".csv" in filename:
-        raise ValueError("The filename should not contain '.csv'")
+        filename = filename.replace(".csv", "")  # Remove .csv extension
 
     # Get the directory of the caller script if position is not provided
     if position is None:
         caller_dir = os.path.dirname(os.path.abspath(sys.argv[0]))
         position = caller_dir
 
     try:
```

### Comparing `scrapegraphai-0.2.6/scrapegraphai/utils/convert_to_json.py` & `scrapegraphai-0.2.7/scrapegraphai/utils/convert_to_json.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     Raises:
     ValueError: If filename contains '.json'.
     FileNotFoundError: If the specified directory does not exist.
     PermissionError: If the program does not have permission to write to the directory.
     """
     if ".json" in filename:
-        raise ValueError("The filename should not contain '.json'")
+        filename = filename.replace(".json", "")  # Remove .csv extension
 
   # Get the directory of the caller script
     if position is None:
         # Get directory of the main script
         caller_dir = os.path.dirname(os.path.abspath(sys.argv[0]))
         position = caller_dir
```

### Comparing `scrapegraphai-0.2.6/scrapegraphai/utils/parse_state_keys.py` & `scrapegraphai-0.2.7/scrapegraphai/utils/parse_state_keys.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.6/scrapegraphai/utils/prettify_exec_info.py` & `scrapegraphai-0.2.7/scrapegraphai/utils/prettify_exec_info.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.6/scrapegraphai/utils/remover.py` & `scrapegraphai-0.2.7/scrapegraphai/utils/remover.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.6/scrapegraphai/utils/research_web.py` & `scrapegraphai-0.2.7/scrapegraphai/utils/research_web.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.6/scrapegraphai/utils/save_audio_from_bytes.py` & `scrapegraphai-0.2.7/scrapegraphai/utils/save_audio_from_bytes.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.6/scrapegraphai/utils/token_calculator.py` & `scrapegraphai-0.2.7/scrapegraphai/utils/token_calculator.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.6/PKG-INFO` & `scrapegraphai-0.2.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapegraphai
-Version: 0.2.6
+Version: 0.2.7
 Summary: A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines.
 Home-page: https://scrapegraph-ai.readthedocs.io/
 License: MIT
 Keywords: scrapegraph,scrapegraphai,langchain,ai,artificial intelligence,gpt,machine learning,rag,nlp,natural language processing,openai,scraping,web scraping,web scraping library,web scraping tool,webscraping,graph
 Author: Marco Vinciguerra
 Author-email: mvincig11@gmail.com
 Requires-Python: >3.9,<4.0
@@ -34,14 +34,15 @@
 Description-Content-Type: text/markdown
 
 
 # 🕷️ ScrapeGraphAI: You Only Scrape Once
 [![Downloads](https://static.pepy.tech/badge/scrapegraphai)](https://pepy.tech/project/scrapegraphai)
 [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
 [![Pylint](https://github.com/VinciGit00/Scrapegraph-ai/actions/workflows/pylint.yml/badge.svg)](https://github.com/VinciGit00/Scrapegraph-ai/actions/workflows/pylint.yml)
+[![CodeQL](https://github.com/VinciGit00/Scrapegraph-ai/actions/workflows/codeql.yml/badge.svg)](https://github.com/VinciGit00/Scrapegraph-ai/actions/workflows/codeql.yml)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![](https://dcbadge.vercel.app/api/server/gkxQDAjfeX)](https://discord.gg/gkxQDAjfeX)
 
 
 ScrapeGraphAI is a *web scraping* python library that uses LLM and direct graph logic to create scraping pipelines for websites, documents and XML files.
 Just say which information you want to extract and the library will do it for you!
 
@@ -84,20 +85,19 @@
 from scrapegraphai.graphs import SmartScraperGraph
 
 graph_config = {
     "llm": {
         "model": "ollama/mistral",
         "temperature": 0,
         "format": "json",  # Ollama needs the format to be specified explicitly
-        "base_url": "http://localhost:11434",  # set Ollama URL arbitrarily
+        "base_url": "http://localhost:11434",  # set Ollama URL
     },
     "embeddings": {
         "model": "ollama/nomic-embed-text",
-        "temperature": 0,
-        "base_url": "http://localhost:11434",  # set Ollama URL arbitrarily
+        "base_url": "http://localhost:11434",  # set Ollama URL
     }
 }
 
 smart_scraper_graph = SmartScraperGraph(
     prompt="List me all the articles",
     # also accepts a string with the already downloaded HTML code
     source="https://perinim.github.io/projects",
@@ -110,15 +110,15 @@
 ```
 
 ### Case 2: Extracting information using Docker
 
 Note: before using the local model remember to create the docker container!
 ```text
     docker-compose up -d
-    docker exec -it ollama ollama run stablelm-zephyr
+    docker exec -it ollama ollama pull stablelm-zephyr
 ```
 You can use which models avaiable on Ollama or your own model instead of stablelm-zephyr
 ```python
 from scrapegraphai.graphs import SmartScraperGraph
 
 graph_config = {
     "llm": {
```

