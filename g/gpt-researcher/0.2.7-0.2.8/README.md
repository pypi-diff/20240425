# Comparing `tmp/gpt-researcher-0.2.7.tar.gz` & `tmp/gpt-researcher-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-researcher-0.2.7.tar", last modified: Thu Apr 25 07:49:30 2024, max compression
+gzip compressed data, was "gpt-researcher-0.2.8.tar", last modified: Thu Apr 25 07:57:49 2024, max compression
```

## Comparing `gpt-researcher-0.2.7.tar` & `gpt-researcher-0.2.8.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.503021 gpt-researcher-0.2.7/
--rw-r--r--   0 assafel    (501) staff       (20)     1069 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/LICENSE
--rw-r--r--   0 assafel    (501) staff       (20)    10018 2024-04-25 07:49:30.502472 gpt-researcher-0.2.7/PKG-INFO
--rw-r--r--   0 assafel    (501) staff       (20)     9295 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/README.md
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.454889 gpt-researcher-0.2.7/backend/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/backend/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.455448 gpt-researcher-0.2.7/backend/report_type/
--rw-r--r--   0 assafel    (501) staff       (20)      165 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/backend/report_type/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.456434 gpt-researcher-0.2.7/backend/report_type/basic_report/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/backend/report_type/basic_report/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      777 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/backend/report_type/basic_report/basic_report.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.457444 gpt-researcher-0.2.7/backend/report_type/detailed_report/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/backend/report_type/detailed_report/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     6012 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/backend/report_type/detailed_report/detailed_report.py
--rw-r--r--   0 assafel    (501) staff       (20)     2130 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/backend/server.py
--rw-r--r--   0 assafel    (501) staff       (20)     2396 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/backend/utils.py
--rw-r--r--   0 assafel    (501) staff       (20)     2822 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/backend/websocket_manager.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.458160 gpt-researcher-0.2.7/gpt_researcher/
--rw-r--r--   0 assafel    (501) staff       (20)      100 2023-11-13 18:29:19.000000 gpt-researcher-0.2.7/gpt_researcher/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.462469 gpt-researcher-0.2.7/gpt_researcher/config/
--rw-r--r--   0 assafel    (501) staff       (20)       48 2023-11-13 18:29:19.000000 gpt-researcher-0.2.7/gpt_researcher/config/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2094 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/gpt_researcher/config/config.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.464114 gpt-researcher-0.2.7/gpt_researcher/context/
--rw-r--r--   0 assafel    (501) staff       (20)      140 2023-11-19 07:01:11.000000 gpt-researcher-0.2.7/gpt_researcher/context/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1812 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/gpt_researcher/context/compression.py
--rw-r--r--   0 assafel    (501) staff       (20)      801 2023-11-19 07:01:11.000000 gpt-researcher-0.2.7/gpt_researcher/context/retriever.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.464688 gpt-researcher-0.2.7/gpt_researcher/llm_provider/
--rw-r--r--   0 assafel    (501) staff       (20)      226 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/gpt_researcher/llm_provider/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.465733 gpt-researcher-0.2.7/gpt_researcher/llm_provider/azureopenai/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/gpt_researcher/llm_provider/azureopenai/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     3068 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/gpt_researcher/llm_provider/azureopenai/azureopenai.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.466719 gpt-researcher-0.2.7/gpt_researcher/llm_provider/google/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/gpt_researcher/llm_provider/google/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     3670 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/gpt_researcher/llm_provider/google/google.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.467737 gpt-researcher-0.2.7/gpt_researcher/llm_provider/openai/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/gpt_researcher/llm_provider/openai/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2091 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/gpt_researcher/llm_provider/openai/openai.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.470007 gpt-researcher-0.2.7/gpt_researcher/master/
--rw-r--r--   0 assafel    (501) staff       (20)       61 2023-11-13 18:29:19.000000 gpt-researcher-0.2.7/gpt_researcher/master/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     8728 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/gpt_researcher/master/agent.py
--rw-r--r--   0 assafel    (501) staff       (20)    12199 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/gpt_researcher/master/functions.py
--rw-r--r--   0 assafel    (501) staff       (20)    13137 2024-04-25 07:48:20.000000 gpt-researcher-0.2.7/gpt_researcher/master/prompts.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.471282 gpt-researcher-0.2.7/gpt_researcher/memory/
--rw-r--r--   0 assafel    (501) staff       (20)       31 2023-11-19 07:01:11.000000 gpt-researcher-0.2.7/gpt_researcher/memory/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1047 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/gpt_researcher/memory/embeddings.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.472317 gpt-researcher-0.2.7/gpt_researcher/retrievers/
--rw-r--r--   0 assafel    (501) staff       (20)      510 2023-12-18 08:18:37.000000 gpt-researcher-0.2.7/gpt_researcher/retrievers/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.473491 gpt-researcher-0.2.7/gpt_researcher/retrievers/bing/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-08 11:24:31.000000 gpt-researcher-0.2.7/gpt_researcher/retrievers/bing/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2240 2023-12-08 11:24:31.000000 gpt-researcher-0.2.7/gpt_researcher/retrievers/bing/bing.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.474531 gpt-researcher-0.2.7/gpt_researcher/retrievers/duckduckgo/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.7/gpt_researcher/retrievers/duckduckgo/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      479 2024-04-12 11:24:29.000000 gpt-researcher-0.2.7/gpt_researcher/retrievers/duckduckgo/duckduckgo.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.475739 gpt-researcher-0.2.7/gpt_researcher/retrievers/google/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.7/gpt_researcher/retrievers/google/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2535 2023-11-19 07:01:11.000000 gpt-researcher-0.2.7/gpt_researcher/retrievers/google/google.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.477153 gpt-researcher-0.2.7/gpt_researcher/retrievers/searx/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.7/gpt_researcher/retrievers/searx/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1294 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/gpt_researcher/retrievers/searx/searx.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.478165 gpt-researcher-0.2.7/gpt_researcher/retrievers/serpapi/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/gpt_researcher/retrievers/serpapi/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2232 2023-11-25 13:46:26.000000 gpt-researcher-0.2.7/gpt_researcher/retrievers/serpapi/serpapi.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.479188 gpt-researcher-0.2.7/gpt_researcher/retrievers/serper/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.7/gpt_researcher/retrievers/serper/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2117 2023-11-25 13:46:26.000000 gpt-researcher-0.2.7/gpt_researcher/retrievers/serper/serper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.480198 gpt-researcher-0.2.7/gpt_researcher/retrievers/tavily_news/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-18 08:18:37.000000 gpt-researcher-0.2.7/gpt_researcher/retrievers/tavily_news/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1281 2023-12-18 08:18:37.000000 gpt-researcher-0.2.7/gpt_researcher/retrievers/tavily_news/tavily_news.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.481227 gpt-researcher-0.2.7/gpt_researcher/retrievers/tavily_search/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.7/gpt_researcher/retrievers/tavily_search/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1506 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/gpt_researcher/retrievers/tavily_search/tavily_search.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.482879 gpt-researcher-0.2.7/gpt_researcher/scraper/
--rw-r--r--   0 assafel    (501) staff       (20)      398 2024-03-17 08:29:46.000000 gpt-researcher-0.2.7/gpt_researcher/scraper/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.484799 gpt-researcher-0.2.7/gpt_researcher/scraper/arxiv/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.7/gpt_researcher/scraper/arxiv/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      762 2024-03-12 13:09:58.000000 gpt-researcher-0.2.7/gpt_researcher/scraper/arxiv/arxiv.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.486270 gpt-researcher-0.2.7/gpt_researcher/scraper/beautiful_soup/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.7/gpt_researcher/scraper/beautiful_soup/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1992 2024-03-12 13:09:58.000000 gpt-researcher-0.2.7/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.487616 gpt-researcher-0.2.7/gpt_researcher/scraper/newspaper/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.7/gpt_researcher/scraper/newspaper/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1312 2024-03-12 13:09:58.000000 gpt-researcher-0.2.7/gpt_researcher/scraper/newspaper/newspaper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.489157 gpt-researcher-0.2.7/gpt_researcher/scraper/pymupdf/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.7/gpt_researcher/scraper/pymupdf/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      640 2024-03-12 13:09:58.000000 gpt-researcher-0.2.7/gpt_researcher/scraper/pymupdf/pymupdf.py
--rw-r--r--   0 assafel    (501) staff       (20)     3111 2024-03-17 08:29:46.000000 gpt-researcher-0.2.7/gpt_researcher/scraper/scraper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.490900 gpt-researcher-0.2.7/gpt_researcher/scraper/web_base_loader/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.7/gpt_researcher/scraper/web_base_loader/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1074 2024-03-12 13:09:58.000000 gpt-researcher-0.2.7/gpt_researcher/scraper/web_base_loader/web_base_loader.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.494117 gpt-researcher-0.2.7/gpt_researcher/utils/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.7/gpt_researcher/utils/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      274 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/gpt_researcher/utils/enum.py
--rw-r--r--   0 assafel    (501) staff       (20)     5108 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/gpt_researcher/utils/llm.py
--rw-r--r--   0 assafel    (501) staff       (20)      216 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/gpt_researcher/utils/validators.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.461156 gpt-researcher-0.2.7/gpt_researcher.egg-info/
--rw-r--r--   0 assafel    (501) staff       (20)    10018 2024-04-25 07:49:30.000000 gpt-researcher-0.2.7/gpt_researcher.egg-info/PKG-INFO
--rw-r--r--   0 assafel    (501) staff       (20)     3134 2024-04-25 07:49:30.000000 gpt-researcher-0.2.7/gpt_researcher.egg-info/SOURCES.txt
--rw-r--r--   0 assafel    (501) staff       (20)        1 2024-04-25 07:49:30.000000 gpt-researcher-0.2.7/gpt_researcher.egg-info/dependency_links.txt
--rw-r--r--   0 assafel    (501) staff       (20)      331 2024-04-25 07:49:30.000000 gpt-researcher-0.2.7/gpt_researcher.egg-info/requires.txt
--rw-r--r--   0 assafel    (501) staff       (20)       36 2024-04-25 07:49:30.000000 gpt-researcher-0.2.7/gpt_researcher.egg-info/top_level.txt
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.495562 gpt-researcher-0.2.7/multi_agents/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:48:05.000000 gpt-researcher-0.2.7/multi_agents/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.500726 gpt-researcher-0.2.7/multi_agents/agents/
--rw-r--r--   0 assafel    (501) staff       (20)      396 2024-04-24 07:58:50.000000 gpt-researcher-0.2.7/multi_agents/agents/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1727 2024-03-19 10:01:22.000000 gpt-researcher-0.2.7/multi_agents/agents/critique.py
--rw-r--r--   0 assafel    (501) staff       (20)     1666 2024-03-19 10:01:22.000000 gpt-researcher-0.2.7/multi_agents/agents/curator.py
--rw-r--r--   0 assafel    (501) staff       (20)     2351 2024-04-24 15:50:47.000000 gpt-researcher-0.2.7/multi_agents/agents/editor.py
--rw-r--r--   0 assafel    (501) staff       (20)     2482 2024-04-25 07:27:33.000000 gpt-researcher-0.2.7/multi_agents/agents/master.py
--rw-r--r--   0 assafel    (501) staff       (20)     1092 2024-04-25 07:26:30.000000 gpt-researcher-0.2.7/multi_agents/agents/publisher.py
--rw-r--r--   0 assafel    (501) staff       (20)     2477 2024-04-25 07:44:43.000000 gpt-researcher-0.2.7/multi_agents/agents/researcher.py
--rw-r--r--   0 assafel    (501) staff       (20)      361 2024-04-22 12:37:36.000000 gpt-researcher-0.2.7/multi_agents/agents/reviser.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.501767 gpt-researcher-0.2.7/multi_agents/agents/utils/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-25 07:20:14.000000 gpt-researcher-0.2.7/multi_agents/agents/utils/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2410 2024-04-25 07:24:00.000000 gpt-researcher-0.2.7/multi_agents/agents/utils/file_utils.py
--rw-r--r--   0 assafel    (501) staff       (20)     2686 2024-04-25 07:29:04.000000 gpt-researcher-0.2.7/multi_agents/agents/writer.py
--rw-r--r--   0 assafel    (501) staff       (20)      375 2024-04-25 07:25:23.000000 gpt-researcher-0.2.7/multi_agents/main.py
--rw-r--r--   0 assafel    (501) staff       (20)     1156 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/pyproject.toml
--rw-r--r--   0 assafel    (501) staff       (20)       38 2024-04-25 07:49:30.503158 gpt-researcher-0.2.7/setup.cfg
--rw-r--r--   0 assafel    (501) staff       (20)     1176 2024-04-25 07:49:24.000000 gpt-researcher-0.2.7/setup.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:57:49.202578 gpt-researcher-0.2.8/
+-rw-r--r--   0 assafel    (501) staff       (20)     1069 2024-04-22 11:21:41.000000 gpt-researcher-0.2.8/LICENSE
+-rw-r--r--   0 assafel    (501) staff       (20)    10018 2024-04-25 07:57:49.201621 gpt-researcher-0.2.8/PKG-INFO
+-rw-r--r--   0 assafel    (501) staff       (20)     9295 2024-04-22 11:21:41.000000 gpt-researcher-0.2.8/README.md
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:57:49.151789 gpt-researcher-0.2.8/backend/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.2.8/backend/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:57:49.152557 gpt-researcher-0.2.8/backend/report_type/
+-rw-r--r--   0 assafel    (501) staff       (20)      165 2024-04-22 11:21:41.000000 gpt-researcher-0.2.8/backend/report_type/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:57:49.153629 gpt-researcher-0.2.8/backend/report_type/basic_report/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.2.8/backend/report_type/basic_report/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      777 2024-04-22 11:21:41.000000 gpt-researcher-0.2.8/backend/report_type/basic_report/basic_report.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:57:49.154774 gpt-researcher-0.2.8/backend/report_type/detailed_report/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.2.8/backend/report_type/detailed_report/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     6012 2024-04-22 11:21:41.000000 gpt-researcher-0.2.8/backend/report_type/detailed_report/detailed_report.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2130 2024-04-22 11:21:41.000000 gpt-researcher-0.2.8/backend/server.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2396 2024-04-22 11:21:41.000000 gpt-researcher-0.2.8/backend/utils.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2822 2024-04-22 11:21:41.000000 gpt-researcher-0.2.8/backend/websocket_manager.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:57:49.155762 gpt-researcher-0.2.8/gpt_researcher/
+-rw-r--r--   0 assafel    (501) staff       (20)      100 2023-11-13 18:29:19.000000 gpt-researcher-0.2.8/gpt_researcher/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:57:49.160634 gpt-researcher-0.2.8/gpt_researcher/config/
+-rw-r--r--   0 assafel    (501) staff       (20)       48 2023-11-13 18:29:19.000000 gpt-researcher-0.2.8/gpt_researcher/config/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2094 2024-04-22 11:21:41.000000 gpt-researcher-0.2.8/gpt_researcher/config/config.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:57:49.162646 gpt-researcher-0.2.8/gpt_researcher/context/
+-rw-r--r--   0 assafel    (501) staff       (20)      140 2023-11-19 07:01:11.000000 gpt-researcher-0.2.8/gpt_researcher/context/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1812 2024-04-22 11:21:41.000000 gpt-researcher-0.2.8/gpt_researcher/context/compression.py
+-rw-r--r--   0 assafel    (501) staff       (20)      801 2023-11-19 07:01:11.000000 gpt-researcher-0.2.8/gpt_researcher/context/retriever.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:57:49.163314 gpt-researcher-0.2.8/gpt_researcher/llm_provider/
+-rw-r--r--   0 assafel    (501) staff       (20)      226 2024-04-22 11:21:41.000000 gpt-researcher-0.2.8/gpt_researcher/llm_provider/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:57:49.164502 gpt-researcher-0.2.8/gpt_researcher/llm_provider/azureopenai/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.2.8/gpt_researcher/llm_provider/azureopenai/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3068 2024-04-22 11:21:41.000000 gpt-researcher-0.2.8/gpt_researcher/llm_provider/azureopenai/azureopenai.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:57:49.165806 gpt-researcher-0.2.8/gpt_researcher/llm_provider/google/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.2.8/gpt_researcher/llm_provider/google/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3670 2024-04-22 11:21:41.000000 gpt-researcher-0.2.8/gpt_researcher/llm_provider/google/google.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:57:49.166877 gpt-researcher-0.2.8/gpt_researcher/llm_provider/openai/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.2.8/gpt_researcher/llm_provider/openai/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2091 2024-04-22 11:21:41.000000 gpt-researcher-0.2.8/gpt_researcher/llm_provider/openai/openai.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:57:49.169537 gpt-researcher-0.2.8/gpt_researcher/master/
+-rw-r--r--   0 assafel    (501) staff       (20)       61 2023-11-13 18:29:19.000000 gpt-researcher-0.2.8/gpt_researcher/master/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     8909 2024-04-25 07:55:48.000000 gpt-researcher-0.2.8/gpt_researcher/master/agent.py
+-rw-r--r--   0 assafel    (501) staff       (20)    12199 2024-04-22 11:21:41.000000 gpt-researcher-0.2.8/gpt_researcher/master/functions.py
+-rw-r--r--   0 assafel    (501) staff       (20)    13137 2024-04-25 07:48:20.000000 gpt-researcher-0.2.8/gpt_researcher/master/prompts.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:57:49.171024 gpt-researcher-0.2.8/gpt_researcher/memory/
+-rw-r--r--   0 assafel    (501) staff       (20)       31 2023-11-19 07:01:11.000000 gpt-researcher-0.2.8/gpt_researcher/memory/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1047 2024-04-22 11:21:41.000000 gpt-researcher-0.2.8/gpt_researcher/memory/embeddings.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:57:49.171710 gpt-researcher-0.2.8/gpt_researcher/retrievers/
+-rw-r--r--   0 assafel    (501) staff       (20)      510 2023-12-18 08:18:37.000000 gpt-researcher-0.2.8/gpt_researcher/retrievers/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:57:49.172922 gpt-researcher-0.2.8/gpt_researcher/retrievers/bing/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-08 11:24:31.000000 gpt-researcher-0.2.8/gpt_researcher/retrievers/bing/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2240 2023-12-08 11:24:31.000000 gpt-researcher-0.2.8/gpt_researcher/retrievers/bing/bing.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:57:49.174370 gpt-researcher-0.2.8/gpt_researcher/retrievers/duckduckgo/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.8/gpt_researcher/retrievers/duckduckgo/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      479 2024-04-12 11:24:29.000000 gpt-researcher-0.2.8/gpt_researcher/retrievers/duckduckgo/duckduckgo.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:57:49.175731 gpt-researcher-0.2.8/gpt_researcher/retrievers/google/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.8/gpt_researcher/retrievers/google/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2535 2023-11-19 07:01:11.000000 gpt-researcher-0.2.8/gpt_researcher/retrievers/google/google.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:57:49.176913 gpt-researcher-0.2.8/gpt_researcher/retrievers/searx/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.8/gpt_researcher/retrievers/searx/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1294 2024-04-22 11:21:41.000000 gpt-researcher-0.2.8/gpt_researcher/retrievers/searx/searx.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:57:49.177962 gpt-researcher-0.2.8/gpt_researcher/retrievers/serpapi/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.2.8/gpt_researcher/retrievers/serpapi/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2232 2023-11-25 13:46:26.000000 gpt-researcher-0.2.8/gpt_researcher/retrievers/serpapi/serpapi.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:57:49.179009 gpt-researcher-0.2.8/gpt_researcher/retrievers/serper/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.8/gpt_researcher/retrievers/serper/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2117 2023-11-25 13:46:26.000000 gpt-researcher-0.2.8/gpt_researcher/retrievers/serper/serper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:57:49.180025 gpt-researcher-0.2.8/gpt_researcher/retrievers/tavily_news/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-18 08:18:37.000000 gpt-researcher-0.2.8/gpt_researcher/retrievers/tavily_news/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1281 2023-12-18 08:18:37.000000 gpt-researcher-0.2.8/gpt_researcher/retrievers/tavily_news/tavily_news.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:57:49.181044 gpt-researcher-0.2.8/gpt_researcher/retrievers/tavily_search/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.8/gpt_researcher/retrievers/tavily_search/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1506 2024-04-22 11:21:41.000000 gpt-researcher-0.2.8/gpt_researcher/retrievers/tavily_search/tavily_search.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:57:49.182164 gpt-researcher-0.2.8/gpt_researcher/scraper/
+-rw-r--r--   0 assafel    (501) staff       (20)      398 2024-03-17 08:29:46.000000 gpt-researcher-0.2.8/gpt_researcher/scraper/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:57:49.183164 gpt-researcher-0.2.8/gpt_researcher/scraper/arxiv/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.8/gpt_researcher/scraper/arxiv/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      762 2024-03-12 13:09:58.000000 gpt-researcher-0.2.8/gpt_researcher/scraper/arxiv/arxiv.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:57:49.184161 gpt-researcher-0.2.8/gpt_researcher/scraper/beautiful_soup/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.8/gpt_researcher/scraper/beautiful_soup/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1992 2024-03-12 13:09:58.000000 gpt-researcher-0.2.8/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:57:49.185184 gpt-researcher-0.2.8/gpt_researcher/scraper/newspaper/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.8/gpt_researcher/scraper/newspaper/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1312 2024-03-12 13:09:58.000000 gpt-researcher-0.2.8/gpt_researcher/scraper/newspaper/newspaper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:57:49.186227 gpt-researcher-0.2.8/gpt_researcher/scraper/pymupdf/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.8/gpt_researcher/scraper/pymupdf/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      640 2024-03-12 13:09:58.000000 gpt-researcher-0.2.8/gpt_researcher/scraper/pymupdf/pymupdf.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3111 2024-03-17 08:29:46.000000 gpt-researcher-0.2.8/gpt_researcher/scraper/scraper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:57:49.187240 gpt-researcher-0.2.8/gpt_researcher/scraper/web_base_loader/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.8/gpt_researcher/scraper/web_base_loader/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1074 2024-03-12 13:09:58.000000 gpt-researcher-0.2.8/gpt_researcher/scraper/web_base_loader/web_base_loader.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:57:49.189547 gpt-researcher-0.2.8/gpt_researcher/utils/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.8/gpt_researcher/utils/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      274 2024-04-22 11:21:41.000000 gpt-researcher-0.2.8/gpt_researcher/utils/enum.py
+-rw-r--r--   0 assafel    (501) staff       (20)     5108 2024-04-22 11:21:41.000000 gpt-researcher-0.2.8/gpt_researcher/utils/llm.py
+-rw-r--r--   0 assafel    (501) staff       (20)      216 2024-04-22 11:21:41.000000 gpt-researcher-0.2.8/gpt_researcher/utils/validators.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:57:49.159326 gpt-researcher-0.2.8/gpt_researcher.egg-info/
+-rw-r--r--   0 assafel    (501) staff       (20)    10018 2024-04-25 07:57:48.000000 gpt-researcher-0.2.8/gpt_researcher.egg-info/PKG-INFO
+-rw-r--r--   0 assafel    (501) staff       (20)     3134 2024-04-25 07:57:49.000000 gpt-researcher-0.2.8/gpt_researcher.egg-info/SOURCES.txt
+-rw-r--r--   0 assafel    (501) staff       (20)        1 2024-04-25 07:57:48.000000 gpt-researcher-0.2.8/gpt_researcher.egg-info/dependency_links.txt
+-rw-r--r--   0 assafel    (501) staff       (20)      331 2024-04-25 07:57:48.000000 gpt-researcher-0.2.8/gpt_researcher.egg-info/requires.txt
+-rw-r--r--   0 assafel    (501) staff       (20)       36 2024-04-25 07:57:48.000000 gpt-researcher-0.2.8/gpt_researcher.egg-info/top_level.txt
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:57:49.190750 gpt-researcher-0.2.8/multi_agents/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:48:05.000000 gpt-researcher-0.2.8/multi_agents/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:57:49.198660 gpt-researcher-0.2.8/multi_agents/agents/
+-rw-r--r--   0 assafel    (501) staff       (20)      396 2024-04-24 07:58:50.000000 gpt-researcher-0.2.8/multi_agents/agents/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1727 2024-03-19 10:01:22.000000 gpt-researcher-0.2.8/multi_agents/agents/critique.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1666 2024-03-19 10:01:22.000000 gpt-researcher-0.2.8/multi_agents/agents/curator.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2351 2024-04-24 15:50:47.000000 gpt-researcher-0.2.8/multi_agents/agents/editor.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2482 2024-04-25 07:27:33.000000 gpt-researcher-0.2.8/multi_agents/agents/master.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1092 2024-04-25 07:26:30.000000 gpt-researcher-0.2.8/multi_agents/agents/publisher.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2477 2024-04-25 07:44:43.000000 gpt-researcher-0.2.8/multi_agents/agents/researcher.py
+-rw-r--r--   0 assafel    (501) staff       (20)      361 2024-04-22 12:37:36.000000 gpt-researcher-0.2.8/multi_agents/agents/reviser.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:57:49.200290 gpt-researcher-0.2.8/multi_agents/agents/utils/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-25 07:20:14.000000 gpt-researcher-0.2.8/multi_agents/agents/utils/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2410 2024-04-25 07:24:00.000000 gpt-researcher-0.2.8/multi_agents/agents/utils/file_utils.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2686 2024-04-25 07:29:04.000000 gpt-researcher-0.2.8/multi_agents/agents/writer.py
+-rw-r--r--   0 assafel    (501) staff       (20)      375 2024-04-25 07:25:23.000000 gpt-researcher-0.2.8/multi_agents/main.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1156 2024-04-22 11:21:41.000000 gpt-researcher-0.2.8/pyproject.toml
+-rw-r--r--   0 assafel    (501) staff       (20)       38 2024-04-25 07:57:49.202780 gpt-researcher-0.2.8/setup.cfg
+-rw-r--r--   0 assafel    (501) staff       (20)     1176 2024-04-25 07:57:21.000000 gpt-researcher-0.2.8/setup.py
```

### Comparing `gpt-researcher-0.2.7/LICENSE` & `gpt-researcher-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/PKG-INFO` & `gpt-researcher-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-researcher
-Version: 0.2.7
+Version: 0.2.8
 Summary: GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.
 Home-page: https://github.com/assafelovic/gpt-researcher
 Author: Assaf Elovic
 Author-email: assaf.elovic@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `gpt-researcher-0.2.7/README.md` & `gpt-researcher-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/backend/report_type/basic_report/basic_report.py` & `gpt-researcher-0.2.8/backend/report_type/basic_report/basic_report.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/backend/report_type/detailed_report/detailed_report.py` & `gpt-researcher-0.2.8/backend/report_type/detailed_report/detailed_report.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/backend/server.py` & `gpt-researcher-0.2.8/backend/server.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/backend/utils.py` & `gpt-researcher-0.2.8/backend/utils.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/backend/websocket_manager.py` & `gpt-researcher-0.2.8/backend/websocket_manager.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/gpt_researcher/config/config.py` & `gpt-researcher-0.2.8/gpt_researcher/config/config.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/gpt_researcher/context/compression.py` & `gpt-researcher-0.2.8/gpt_researcher/context/compression.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/gpt_researcher/context/retriever.py` & `gpt-researcher-0.2.8/gpt_researcher/context/retriever.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/gpt_researcher/llm_provider/azureopenai/azureopenai.py` & `gpt-researcher-0.2.8/gpt_researcher/llm_provider/azureopenai/azureopenai.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/gpt_researcher/llm_provider/google/google.py` & `gpt-researcher-0.2.8/gpt_researcher/llm_provider/google/google.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/gpt_researcher/llm_provider/openai/openai.py` & `gpt-researcher-0.2.8/gpt_researcher/llm_provider/openai/openai.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/gpt_researcher/master/agent.py` & `gpt-researcher-0.2.8/gpt_researcher/master/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,20 @@
         """
            Generates the context for the research task by searching the query and scraping the results
         Returns:
             context: List of context
         """
         context = []
         # Generate Sub-Queries including original query
-        sub_queries = await get_sub_queries(query, self.role, self.cfg, self.parent_query, self.report_type) + [query]
+        sub_queries = await get_sub_queries(query, self.role, self.cfg, self.parent_query, self.report_type)
+
+        # If this is not part of a sub researcher, add original query to research for better results
+        if self.report_type != "subtopic_report":
+            sub_queries.append(query)
+
         await stream_output("logs",
                             f"🧠 I will conduct my research based on the following queries: {sub_queries}...",
                             self.websocket)
 
         # Using asyncio.gather to process the sub_queries asynchronously
         context = await asyncio.gather(*[self.process_sub_query(sub_query) for sub_query in sub_queries])
         return context
```

### Comparing `gpt-researcher-0.2.7/gpt_researcher/master/functions.py` & `gpt-researcher-0.2.8/gpt_researcher/master/functions.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/gpt_researcher/master/prompts.py` & `gpt-researcher-0.2.8/gpt_researcher/master/prompts.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/gpt_researcher/memory/embeddings.py` & `gpt-researcher-0.2.8/gpt_researcher/memory/embeddings.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/gpt_researcher/retrievers/bing/bing.py` & `gpt-researcher-0.2.8/gpt_researcher/retrievers/bing/bing.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/gpt_researcher/retrievers/google/google.py` & `gpt-researcher-0.2.8/gpt_researcher/retrievers/google/google.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/gpt_researcher/retrievers/searx/searx.py` & `gpt-researcher-0.2.8/gpt_researcher/retrievers/searx/searx.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/gpt_researcher/retrievers/serpapi/serpapi.py` & `gpt-researcher-0.2.8/gpt_researcher/retrievers/serpapi/serpapi.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/gpt_researcher/retrievers/serper/serper.py` & `gpt-researcher-0.2.8/gpt_researcher/retrievers/serper/serper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/gpt_researcher/retrievers/tavily_news/tavily_news.py` & `gpt-researcher-0.2.8/gpt_researcher/retrievers/tavily_news/tavily_news.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/gpt_researcher/retrievers/tavily_search/tavily_search.py` & `gpt-researcher-0.2.8/gpt_researcher/retrievers/tavily_search/tavily_search.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/gpt_researcher/scraper/arxiv/arxiv.py` & `gpt-researcher-0.2.8/gpt_researcher/scraper/arxiv/arxiv.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py` & `gpt-researcher-0.2.8/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/gpt_researcher/scraper/newspaper/newspaper.py` & `gpt-researcher-0.2.8/gpt_researcher/scraper/newspaper/newspaper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/gpt_researcher/scraper/pymupdf/pymupdf.py` & `gpt-researcher-0.2.8/gpt_researcher/scraper/pymupdf/pymupdf.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/gpt_researcher/scraper/scraper.py` & `gpt-researcher-0.2.8/gpt_researcher/scraper/scraper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/gpt_researcher/scraper/web_base_loader/web_base_loader.py` & `gpt-researcher-0.2.8/gpt_researcher/scraper/web_base_loader/web_base_loader.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/gpt_researcher/utils/llm.py` & `gpt-researcher-0.2.8/gpt_researcher/utils/llm.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/gpt_researcher.egg-info/PKG-INFO` & `gpt-researcher-0.2.8/gpt_researcher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-researcher
-Version: 0.2.7
+Version: 0.2.8
 Summary: GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.
 Home-page: https://github.com/assafelovic/gpt-researcher
 Author: Assaf Elovic
 Author-email: assaf.elovic@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `gpt-researcher-0.2.7/gpt_researcher.egg-info/SOURCES.txt` & `gpt-researcher-0.2.8/gpt_researcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/multi_agents/agents/critique.py` & `gpt-researcher-0.2.8/multi_agents/agents/critique.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/multi_agents/agents/curator.py` & `gpt-researcher-0.2.8/multi_agents/agents/curator.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/multi_agents/agents/editor.py` & `gpt-researcher-0.2.8/multi_agents/agents/editor.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/multi_agents/agents/master.py` & `gpt-researcher-0.2.8/multi_agents/agents/master.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/multi_agents/agents/publisher.py` & `gpt-researcher-0.2.8/multi_agents/agents/publisher.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/multi_agents/agents/researcher.py` & `gpt-researcher-0.2.8/multi_agents/agents/researcher.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/multi_agents/agents/utils/file_utils.py` & `gpt-researcher-0.2.8/multi_agents/agents/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/multi_agents/agents/writer.py` & `gpt-researcher-0.2.8/multi_agents/agents/writer.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/pyproject.toml` & `gpt-researcher-0.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.7/setup.py` & `gpt-researcher-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open("requirements.txt", "r") as f:
     reqs = [line.strip() for line in f if ('selenium' not in line and 'webdriver' not in line)]
 
 setup(
     name="gpt-researcher",
-    version="0.2.7",
+    version="0.2.8",
     description="GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.",
     package_dir={'gpt_researcher': 'gpt_researcher'},
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/assafelovic/gpt-researcher",
     author="Assaf Elovic",
```

