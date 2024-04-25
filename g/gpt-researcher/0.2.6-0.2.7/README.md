# Comparing `tmp/gpt-researcher-0.2.6.tar.gz` & `tmp/gpt-researcher-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-researcher-0.2.6.tar", last modified: Fri Apr 12 14:15:59 2024, max compression
+gzip compressed data, was "gpt-researcher-0.2.7.tar", last modified: Thu Apr 25 07:49:30 2024, max compression
```

## Comparing `gpt-researcher-0.2.6.tar` & `gpt-researcher-0.2.7.tar`

### file list

```diff
@@ -1,103 +1,119 @@
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 14:15:59.882588 gpt-researcher-0.2.6/
--rw-r--r--   0 assafel    (501) staff       (20)     1069 2024-04-01 15:55:34.000000 gpt-researcher-0.2.6/LICENSE
--rw-r--r--   0 assafel    (501) staff       (20)    12514 2024-04-12 14:15:59.881738 gpt-researcher-0.2.6/PKG-INFO
--rw-r--r--   0 assafel    (501) staff       (20)    11791 2024-04-09 08:07:24.000000 gpt-researcher-0.2.6/README.md
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 14:15:59.824163 gpt-researcher-0.2.6/backend/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-12 13:32:44.000000 gpt-researcher-0.2.6/backend/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 14:15:59.824801 gpt-researcher-0.2.6/backend/report_type/
--rw-r--r--   0 assafel    (501) staff       (20)      165 2024-04-01 15:55:34.000000 gpt-researcher-0.2.6/backend/report_type/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 14:15:59.826074 gpt-researcher-0.2.6/backend/report_type/basic_report/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-01 15:55:34.000000 gpt-researcher-0.2.6/backend/report_type/basic_report/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      777 2024-04-01 15:55:34.000000 gpt-researcher-0.2.6/backend/report_type/basic_report/basic_report.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 14:15:59.827824 gpt-researcher-0.2.6/backend/report_type/detailed_report/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-01 15:55:34.000000 gpt-researcher-0.2.6/backend/report_type/detailed_report/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     6012 2024-04-12 13:55:52.000000 gpt-researcher-0.2.6/backend/report_type/detailed_report/detailed_report.py
--rw-r--r--   0 assafel    (501) staff       (20)     2130 2024-04-12 13:33:01.000000 gpt-researcher-0.2.6/backend/server.py
--rw-r--r--   0 assafel    (501) staff       (20)     2396 2024-03-31 16:54:34.000000 gpt-researcher-0.2.6/backend/utils.py
--rw-r--r--   0 assafel    (501) staff       (20)     2822 2024-04-12 13:55:35.000000 gpt-researcher-0.2.6/backend/websocket_manager.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 14:15:59.828749 gpt-researcher-0.2.6/gpt_researcher/
--rw-r--r--   0 assafel    (501) staff       (20)      100 2023-11-13 18:29:19.000000 gpt-researcher-0.2.6/gpt_researcher/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 14:15:59.834315 gpt-researcher-0.2.6/gpt_researcher/config/
--rw-r--r--   0 assafel    (501) staff       (20)       48 2023-11-13 18:29:19.000000 gpt-researcher-0.2.6/gpt_researcher/config/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2101 2024-04-01 15:55:34.000000 gpt-researcher-0.2.6/gpt_researcher/config/config.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 14:15:59.837387 gpt-researcher-0.2.6/gpt_researcher/context/
--rw-r--r--   0 assafel    (501) staff       (20)      140 2023-11-19 07:01:11.000000 gpt-researcher-0.2.6/gpt_researcher/context/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1812 2024-04-01 15:55:34.000000 gpt-researcher-0.2.6/gpt_researcher/context/compression.py
--rw-r--r--   0 assafel    (501) staff       (20)      801 2023-11-19 07:01:11.000000 gpt-researcher-0.2.6/gpt_researcher/context/retriever.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 14:15:59.838311 gpt-researcher-0.2.6/gpt_researcher/llm_provider/
--rw-r--r--   0 assafel    (501) staff       (20)      226 2024-04-01 15:55:37.000000 gpt-researcher-0.2.6/gpt_researcher/llm_provider/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 14:15:59.840129 gpt-researcher-0.2.6/gpt_researcher/llm_provider/azureopenai/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-01 15:55:37.000000 gpt-researcher-0.2.6/gpt_researcher/llm_provider/azureopenai/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     3068 2024-04-09 08:07:24.000000 gpt-researcher-0.2.6/gpt_researcher/llm_provider/azureopenai/azureopenai.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 14:15:59.842358 gpt-researcher-0.2.6/gpt_researcher/llm_provider/google/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-31 16:54:34.000000 gpt-researcher-0.2.6/gpt_researcher/llm_provider/google/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     3670 2024-03-31 16:54:34.000000 gpt-researcher-0.2.6/gpt_researcher/llm_provider/google/google.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 14:15:59.844151 gpt-researcher-0.2.6/gpt_researcher/llm_provider/openai/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-31 16:54:34.000000 gpt-researcher-0.2.6/gpt_researcher/llm_provider/openai/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2091 2024-03-31 16:54:34.000000 gpt-researcher-0.2.6/gpt_researcher/llm_provider/openai/openai.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 14:15:59.847909 gpt-researcher-0.2.6/gpt_researcher/master/
--rw-r--r--   0 assafel    (501) staff       (20)       61 2023-11-13 18:29:19.000000 gpt-researcher-0.2.6/gpt_researcher/master/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     8922 2024-04-12 13:20:00.000000 gpt-researcher-0.2.6/gpt_researcher/master/agent.py
--rw-r--r--   0 assafel    (501) staff       (20)    12199 2024-04-12 13:09:04.000000 gpt-researcher-0.2.6/gpt_researcher/master/functions.py
--rw-r--r--   0 assafel    (501) staff       (20)    13087 2024-04-12 14:15:48.000000 gpt-researcher-0.2.6/gpt_researcher/master/prompts.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 14:15:59.849824 gpt-researcher-0.2.6/gpt_researcher/memory/
--rw-r--r--   0 assafel    (501) staff       (20)       31 2023-11-19 07:01:11.000000 gpt-researcher-0.2.6/gpt_researcher/memory/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1047 2024-04-01 15:55:37.000000 gpt-researcher-0.2.6/gpt_researcher/memory/embeddings.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 14:15:59.850670 gpt-researcher-0.2.6/gpt_researcher/retrievers/
--rw-r--r--   0 assafel    (501) staff       (20)      510 2023-12-18 08:18:37.000000 gpt-researcher-0.2.6/gpt_researcher/retrievers/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 14:15:59.852435 gpt-researcher-0.2.6/gpt_researcher/retrievers/bing/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-08 11:24:31.000000 gpt-researcher-0.2.6/gpt_researcher/retrievers/bing/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2240 2023-12-08 11:24:31.000000 gpt-researcher-0.2.6/gpt_researcher/retrievers/bing/bing.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 14:15:59.854217 gpt-researcher-0.2.6/gpt_researcher/retrievers/duckduckgo/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.6/gpt_researcher/retrievers/duckduckgo/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      479 2024-04-12 11:24:29.000000 gpt-researcher-0.2.6/gpt_researcher/retrievers/duckduckgo/duckduckgo.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 14:15:59.855988 gpt-researcher-0.2.6/gpt_researcher/retrievers/google/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.6/gpt_researcher/retrievers/google/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2535 2023-11-19 07:01:11.000000 gpt-researcher-0.2.6/gpt_researcher/retrievers/google/google.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 14:15:59.857832 gpt-researcher-0.2.6/gpt_researcher/retrievers/searx/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.6/gpt_researcher/retrievers/searx/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1294 2024-03-31 16:54:34.000000 gpt-researcher-0.2.6/gpt_researcher/retrievers/searx/searx.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 14:15:59.859609 gpt-researcher-0.2.6/gpt_researcher/retrievers/serpapi/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-12 13:06:43.000000 gpt-researcher-0.2.6/gpt_researcher/retrievers/serpapi/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2232 2023-11-25 13:46:26.000000 gpt-researcher-0.2.6/gpt_researcher/retrievers/serpapi/serpapi.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 14:15:59.861521 gpt-researcher-0.2.6/gpt_researcher/retrievers/serper/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.6/gpt_researcher/retrievers/serper/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2117 2023-11-25 13:46:26.000000 gpt-researcher-0.2.6/gpt_researcher/retrievers/serper/serper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 14:15:59.863351 gpt-researcher-0.2.6/gpt_researcher/retrievers/tavily_news/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-18 08:18:37.000000 gpt-researcher-0.2.6/gpt_researcher/retrievers/tavily_news/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1281 2023-12-18 08:18:37.000000 gpt-researcher-0.2.6/gpt_researcher/retrievers/tavily_news/tavily_news.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 14:15:59.864987 gpt-researcher-0.2.6/gpt_researcher/retrievers/tavily_search/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.6/gpt_researcher/retrievers/tavily_search/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1506 2024-04-01 15:55:34.000000 gpt-researcher-0.2.6/gpt_researcher/retrievers/tavily_search/tavily_search.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 14:15:59.866883 gpt-researcher-0.2.6/gpt_researcher/scraper/
--rw-r--r--   0 assafel    (501) staff       (20)      398 2024-03-17 08:29:46.000000 gpt-researcher-0.2.6/gpt_researcher/scraper/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 14:15:59.869343 gpt-researcher-0.2.6/gpt_researcher/scraper/arxiv/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.6/gpt_researcher/scraper/arxiv/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      762 2024-03-12 13:09:58.000000 gpt-researcher-0.2.6/gpt_researcher/scraper/arxiv/arxiv.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 14:15:59.871108 gpt-researcher-0.2.6/gpt_researcher/scraper/beautiful_soup/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.6/gpt_researcher/scraper/beautiful_soup/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1992 2024-03-12 13:09:58.000000 gpt-researcher-0.2.6/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 14:15:59.872906 gpt-researcher-0.2.6/gpt_researcher/scraper/newspaper/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.6/gpt_researcher/scraper/newspaper/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1312 2024-03-12 13:09:58.000000 gpt-researcher-0.2.6/gpt_researcher/scraper/newspaper/newspaper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 14:15:59.874353 gpt-researcher-0.2.6/gpt_researcher/scraper/pymupdf/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.6/gpt_researcher/scraper/pymupdf/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      640 2024-03-12 13:09:58.000000 gpt-researcher-0.2.6/gpt_researcher/scraper/pymupdf/pymupdf.py
--rw-r--r--   0 assafel    (501) staff       (20)     3111 2024-03-17 08:29:46.000000 gpt-researcher-0.2.6/gpt_researcher/scraper/scraper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 14:15:59.876088 gpt-researcher-0.2.6/gpt_researcher/scraper/web_base_loader/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.6/gpt_researcher/scraper/web_base_loader/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1074 2024-03-12 13:09:58.000000 gpt-researcher-0.2.6/gpt_researcher/scraper/web_base_loader/web_base_loader.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 14:15:59.880394 gpt-researcher-0.2.6/gpt_researcher/utils/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.6/gpt_researcher/utils/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      274 2024-04-12 12:40:03.000000 gpt-researcher-0.2.6/gpt_researcher/utils/enum.py
--rw-r--r--   0 assafel    (501) staff       (20)     5108 2024-04-09 08:07:24.000000 gpt-researcher-0.2.6/gpt_researcher/utils/llm.py
--rw-r--r--   0 assafel    (501) staff       (20)      216 2024-04-01 15:55:34.000000 gpt-researcher-0.2.6/gpt_researcher/utils/validators.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 14:15:59.832365 gpt-researcher-0.2.6/gpt_researcher.egg-info/
--rw-r--r--   0 assafel    (501) staff       (20)    12514 2024-04-12 14:15:59.000000 gpt-researcher-0.2.6/gpt_researcher.egg-info/PKG-INFO
--rw-r--r--   0 assafel    (501) staff       (20)     2727 2024-04-12 14:15:59.000000 gpt-researcher-0.2.6/gpt_researcher.egg-info/SOURCES.txt
--rw-r--r--   0 assafel    (501) staff       (20)        1 2024-04-12 14:15:59.000000 gpt-researcher-0.2.6/gpt_researcher.egg-info/dependency_links.txt
--rw-r--r--   0 assafel    (501) staff       (20)      331 2024-04-12 14:15:59.000000 gpt-researcher-0.2.6/gpt_researcher.egg-info/requires.txt
--rw-r--r--   0 assafel    (501) staff       (20)       23 2024-04-12 14:15:59.000000 gpt-researcher-0.2.6/gpt_researcher.egg-info/top_level.txt
--rw-r--r--   0 assafel    (501) staff       (20)     1130 2024-04-09 08:07:24.000000 gpt-researcher-0.2.6/pyproject.toml
--rw-r--r--   0 assafel    (501) staff       (20)       38 2024-04-12 14:15:59.882842 gpt-researcher-0.2.6/setup.cfg
--rw-r--r--   0 assafel    (501) staff       (20)     1176 2024-04-12 14:15:56.000000 gpt-researcher-0.2.6/setup.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.503021 gpt-researcher-0.2.7/
+-rw-r--r--   0 assafel    (501) staff       (20)     1069 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/LICENSE
+-rw-r--r--   0 assafel    (501) staff       (20)    10018 2024-04-25 07:49:30.502472 gpt-researcher-0.2.7/PKG-INFO
+-rw-r--r--   0 assafel    (501) staff       (20)     9295 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/README.md
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.454889 gpt-researcher-0.2.7/backend/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/backend/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.455448 gpt-researcher-0.2.7/backend/report_type/
+-rw-r--r--   0 assafel    (501) staff       (20)      165 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/backend/report_type/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.456434 gpt-researcher-0.2.7/backend/report_type/basic_report/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/backend/report_type/basic_report/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      777 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/backend/report_type/basic_report/basic_report.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.457444 gpt-researcher-0.2.7/backend/report_type/detailed_report/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/backend/report_type/detailed_report/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     6012 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/backend/report_type/detailed_report/detailed_report.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2130 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/backend/server.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2396 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/backend/utils.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2822 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/backend/websocket_manager.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.458160 gpt-researcher-0.2.7/gpt_researcher/
+-rw-r--r--   0 assafel    (501) staff       (20)      100 2023-11-13 18:29:19.000000 gpt-researcher-0.2.7/gpt_researcher/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.462469 gpt-researcher-0.2.7/gpt_researcher/config/
+-rw-r--r--   0 assafel    (501) staff       (20)       48 2023-11-13 18:29:19.000000 gpt-researcher-0.2.7/gpt_researcher/config/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2094 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/gpt_researcher/config/config.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.464114 gpt-researcher-0.2.7/gpt_researcher/context/
+-rw-r--r--   0 assafel    (501) staff       (20)      140 2023-11-19 07:01:11.000000 gpt-researcher-0.2.7/gpt_researcher/context/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1812 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/gpt_researcher/context/compression.py
+-rw-r--r--   0 assafel    (501) staff       (20)      801 2023-11-19 07:01:11.000000 gpt-researcher-0.2.7/gpt_researcher/context/retriever.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.464688 gpt-researcher-0.2.7/gpt_researcher/llm_provider/
+-rw-r--r--   0 assafel    (501) staff       (20)      226 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/gpt_researcher/llm_provider/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.465733 gpt-researcher-0.2.7/gpt_researcher/llm_provider/azureopenai/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/gpt_researcher/llm_provider/azureopenai/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3068 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/gpt_researcher/llm_provider/azureopenai/azureopenai.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.466719 gpt-researcher-0.2.7/gpt_researcher/llm_provider/google/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/gpt_researcher/llm_provider/google/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3670 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/gpt_researcher/llm_provider/google/google.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.467737 gpt-researcher-0.2.7/gpt_researcher/llm_provider/openai/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/gpt_researcher/llm_provider/openai/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2091 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/gpt_researcher/llm_provider/openai/openai.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.470007 gpt-researcher-0.2.7/gpt_researcher/master/
+-rw-r--r--   0 assafel    (501) staff       (20)       61 2023-11-13 18:29:19.000000 gpt-researcher-0.2.7/gpt_researcher/master/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     8728 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/gpt_researcher/master/agent.py
+-rw-r--r--   0 assafel    (501) staff       (20)    12199 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/gpt_researcher/master/functions.py
+-rw-r--r--   0 assafel    (501) staff       (20)    13137 2024-04-25 07:48:20.000000 gpt-researcher-0.2.7/gpt_researcher/master/prompts.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.471282 gpt-researcher-0.2.7/gpt_researcher/memory/
+-rw-r--r--   0 assafel    (501) staff       (20)       31 2023-11-19 07:01:11.000000 gpt-researcher-0.2.7/gpt_researcher/memory/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1047 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/gpt_researcher/memory/embeddings.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.472317 gpt-researcher-0.2.7/gpt_researcher/retrievers/
+-rw-r--r--   0 assafel    (501) staff       (20)      510 2023-12-18 08:18:37.000000 gpt-researcher-0.2.7/gpt_researcher/retrievers/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.473491 gpt-researcher-0.2.7/gpt_researcher/retrievers/bing/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-08 11:24:31.000000 gpt-researcher-0.2.7/gpt_researcher/retrievers/bing/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2240 2023-12-08 11:24:31.000000 gpt-researcher-0.2.7/gpt_researcher/retrievers/bing/bing.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.474531 gpt-researcher-0.2.7/gpt_researcher/retrievers/duckduckgo/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.7/gpt_researcher/retrievers/duckduckgo/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      479 2024-04-12 11:24:29.000000 gpt-researcher-0.2.7/gpt_researcher/retrievers/duckduckgo/duckduckgo.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.475739 gpt-researcher-0.2.7/gpt_researcher/retrievers/google/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.7/gpt_researcher/retrievers/google/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2535 2023-11-19 07:01:11.000000 gpt-researcher-0.2.7/gpt_researcher/retrievers/google/google.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.477153 gpt-researcher-0.2.7/gpt_researcher/retrievers/searx/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.7/gpt_researcher/retrievers/searx/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1294 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/gpt_researcher/retrievers/searx/searx.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.478165 gpt-researcher-0.2.7/gpt_researcher/retrievers/serpapi/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/gpt_researcher/retrievers/serpapi/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2232 2023-11-25 13:46:26.000000 gpt-researcher-0.2.7/gpt_researcher/retrievers/serpapi/serpapi.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.479188 gpt-researcher-0.2.7/gpt_researcher/retrievers/serper/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.7/gpt_researcher/retrievers/serper/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2117 2023-11-25 13:46:26.000000 gpt-researcher-0.2.7/gpt_researcher/retrievers/serper/serper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.480198 gpt-researcher-0.2.7/gpt_researcher/retrievers/tavily_news/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-18 08:18:37.000000 gpt-researcher-0.2.7/gpt_researcher/retrievers/tavily_news/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1281 2023-12-18 08:18:37.000000 gpt-researcher-0.2.7/gpt_researcher/retrievers/tavily_news/tavily_news.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.481227 gpt-researcher-0.2.7/gpt_researcher/retrievers/tavily_search/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.7/gpt_researcher/retrievers/tavily_search/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1506 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/gpt_researcher/retrievers/tavily_search/tavily_search.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.482879 gpt-researcher-0.2.7/gpt_researcher/scraper/
+-rw-r--r--   0 assafel    (501) staff       (20)      398 2024-03-17 08:29:46.000000 gpt-researcher-0.2.7/gpt_researcher/scraper/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.484799 gpt-researcher-0.2.7/gpt_researcher/scraper/arxiv/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.7/gpt_researcher/scraper/arxiv/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      762 2024-03-12 13:09:58.000000 gpt-researcher-0.2.7/gpt_researcher/scraper/arxiv/arxiv.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.486270 gpt-researcher-0.2.7/gpt_researcher/scraper/beautiful_soup/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.7/gpt_researcher/scraper/beautiful_soup/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1992 2024-03-12 13:09:58.000000 gpt-researcher-0.2.7/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.487616 gpt-researcher-0.2.7/gpt_researcher/scraper/newspaper/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.7/gpt_researcher/scraper/newspaper/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1312 2024-03-12 13:09:58.000000 gpt-researcher-0.2.7/gpt_researcher/scraper/newspaper/newspaper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.489157 gpt-researcher-0.2.7/gpt_researcher/scraper/pymupdf/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.7/gpt_researcher/scraper/pymupdf/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      640 2024-03-12 13:09:58.000000 gpt-researcher-0.2.7/gpt_researcher/scraper/pymupdf/pymupdf.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3111 2024-03-17 08:29:46.000000 gpt-researcher-0.2.7/gpt_researcher/scraper/scraper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.490900 gpt-researcher-0.2.7/gpt_researcher/scraper/web_base_loader/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.7/gpt_researcher/scraper/web_base_loader/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1074 2024-03-12 13:09:58.000000 gpt-researcher-0.2.7/gpt_researcher/scraper/web_base_loader/web_base_loader.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.494117 gpt-researcher-0.2.7/gpt_researcher/utils/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.7/gpt_researcher/utils/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      274 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/gpt_researcher/utils/enum.py
+-rw-r--r--   0 assafel    (501) staff       (20)     5108 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/gpt_researcher/utils/llm.py
+-rw-r--r--   0 assafel    (501) staff       (20)      216 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/gpt_researcher/utils/validators.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.461156 gpt-researcher-0.2.7/gpt_researcher.egg-info/
+-rw-r--r--   0 assafel    (501) staff       (20)    10018 2024-04-25 07:49:30.000000 gpt-researcher-0.2.7/gpt_researcher.egg-info/PKG-INFO
+-rw-r--r--   0 assafel    (501) staff       (20)     3134 2024-04-25 07:49:30.000000 gpt-researcher-0.2.7/gpt_researcher.egg-info/SOURCES.txt
+-rw-r--r--   0 assafel    (501) staff       (20)        1 2024-04-25 07:49:30.000000 gpt-researcher-0.2.7/gpt_researcher.egg-info/dependency_links.txt
+-rw-r--r--   0 assafel    (501) staff       (20)      331 2024-04-25 07:49:30.000000 gpt-researcher-0.2.7/gpt_researcher.egg-info/requires.txt
+-rw-r--r--   0 assafel    (501) staff       (20)       36 2024-04-25 07:49:30.000000 gpt-researcher-0.2.7/gpt_researcher.egg-info/top_level.txt
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.495562 gpt-researcher-0.2.7/multi_agents/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:48:05.000000 gpt-researcher-0.2.7/multi_agents/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.500726 gpt-researcher-0.2.7/multi_agents/agents/
+-rw-r--r--   0 assafel    (501) staff       (20)      396 2024-04-24 07:58:50.000000 gpt-researcher-0.2.7/multi_agents/agents/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1727 2024-03-19 10:01:22.000000 gpt-researcher-0.2.7/multi_agents/agents/critique.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1666 2024-03-19 10:01:22.000000 gpt-researcher-0.2.7/multi_agents/agents/curator.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2351 2024-04-24 15:50:47.000000 gpt-researcher-0.2.7/multi_agents/agents/editor.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2482 2024-04-25 07:27:33.000000 gpt-researcher-0.2.7/multi_agents/agents/master.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1092 2024-04-25 07:26:30.000000 gpt-researcher-0.2.7/multi_agents/agents/publisher.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2477 2024-04-25 07:44:43.000000 gpt-researcher-0.2.7/multi_agents/agents/researcher.py
+-rw-r--r--   0 assafel    (501) staff       (20)      361 2024-04-22 12:37:36.000000 gpt-researcher-0.2.7/multi_agents/agents/reviser.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 07:49:30.501767 gpt-researcher-0.2.7/multi_agents/agents/utils/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-25 07:20:14.000000 gpt-researcher-0.2.7/multi_agents/agents/utils/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2410 2024-04-25 07:24:00.000000 gpt-researcher-0.2.7/multi_agents/agents/utils/file_utils.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2686 2024-04-25 07:29:04.000000 gpt-researcher-0.2.7/multi_agents/agents/writer.py
+-rw-r--r--   0 assafel    (501) staff       (20)      375 2024-04-25 07:25:23.000000 gpt-researcher-0.2.7/multi_agents/main.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1156 2024-04-22 11:21:41.000000 gpt-researcher-0.2.7/pyproject.toml
+-rw-r--r--   0 assafel    (501) staff       (20)       38 2024-04-25 07:49:30.503158 gpt-researcher-0.2.7/setup.cfg
+-rw-r--r--   0 assafel    (501) staff       (20)     1176 2024-04-25 07:49:24.000000 gpt-researcher-0.2.7/setup.py
```

### Comparing `gpt-researcher-0.2.6/LICENSE` & `gpt-researcher-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.6/PKG-INFO` & `gpt-researcher-0.2.7/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-researcher
-Version: 0.2.6
+Version: 0.2.7
 Summary: GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.
 Home-page: https://github.com/assafelovic/gpt-researcher
 Author: Assaf Elovic
 Author-email: assaf.elovic@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🔎 GPT Researcher
-[![Official Website](https://img.shields.io/badge/Official%20Website-tavily.com-blue?style=for-the-badge&logo=world&logoColor=white)](https://tavily.com)
+[![Official Website](https://img.shields.io/badge/Official%20Website-gptr.dev-blue?style=for-the-badge&logo=world&logoColor=white)](https://gptr.dev)
 [![Discord Follow](https://dcbadge.vercel.app/api/server/2pFkc83fRq?style=for-the-badge)](https://discord.com/invite/2pFkc83fRq)
 
 [![GitHub Repo stars](https://img.shields.io/github/stars/assafelovic/gpt-researcher?style=social)](https://github.com/assafelovic/gpt-researcher)
 [![Twitter Follow](https://img.shields.io/twitter/follow/assaf_elovic?style=social)](https://twitter.com/assaf_elovic)
 [![PyPI version](https://badge.fury.io/py/gpt-researcher.svg)](https://badge.fury.io/py/gpt-researcher)
 
 <!-- MARKDOWN LINKS & IMAGES -->
@@ -37,16 +37,16 @@
 
 **Our mission is to empower individuals and organizations with accurate, unbiased, and factual information by leveraging the power of AI.**
 
 ## Why GPT Researcher?
 
 - To form objective conclusions for manual research tasks can take time, sometimes weeks to find the right resources and information.
 - Current LLMs are trained on past and outdated information, with heavy risks of hallucinations, making them almost irrelevant for research tasks.
-- Solutions that enable web search (such as ChatGPT + Web Plugin), only consider limited resources and content that in some cases result in superficial conclusions or biased answers.
-- Using only a selection of resources can create bias in determining the right conclusions for research questions or tasks. 
+- Services that enable web search (such as ChatGPT + Web Plugin), only consider limited sources and content that in some cases result in superficial and biased answers.
+- Using only a selection of web sources can create bias in determining the right conclusions for research tasks. 
 
 ## Architecture
 The main idea is to run "planner" and "execution" agents, whereas the planner generates questions to research, and the execution agents seek the most related information based on each generated research question. Finally, the planner filters and aggregates all related information and creates a research report. <br /> <br /> 
 The agents leverage both gpt3.5-turbo and gpt-4-turbo (128K context) to complete a research task. We optimize for costs using each only when necessary. **The average research task takes around 3 minutes to complete, and costs ~$0.1.**
 
 <div align="center">
 <img align="center" height="500" src="https://cowriter-images.s3.amazonaws.com/architecture.png">
@@ -57,15 +57,16 @@
 * Create a domain specific agent based on research query or task.
 * Generate a set of research questions that together form an objective opinion on any given task. 
 * For each research question, trigger a crawler agent that scrapes online resources for information relevant to the given task.
 * For each scraped resources, summarize based on relevant information and keep track of its sources.
 * Finally, filter and aggregate all summarized sources and generate a final research report.
 
 ## Demo
-https://github.com/assafelovic/gpt-researcher/assets/13554167/d5df04a9-631a-4509-aa55-2049b5a9e9bc
+https://github.com/assafelovic/gpt-researcher/assets/13554167/dd6cf08f-b31e-40c6-9907-1915f52a7110
+
 
 ## Tutorials
  - [How it Works](https://docs.tavily.com/blog/building-gpt-researcher)
  - [How to Install](https://www.loom.com/share/04ebffb6ed2a4520a27c3e3addcdde20?sid=da1848e8-b1f1-42d1-93c3-5b0b9c3b24ea)
  - [Live Demo](https://www.loom.com/share/6a3385db4e8747a1913dd85a7834846f?sid=a740fd5b-2aa3-457e-8fb7-86976f59f9b8)
 
 ## Features
@@ -82,113 +83,62 @@
 Please see [here](https://docs.tavily.com/docs/gpt-researcher/getting-started) for full documentation on:
 
 - Getting started (installation, setting up the environment, simple examples)
 - Customization and configuration
 - How-To examples (demos, integrations, docker support)
 - Reference (full API docs)
 
-## Quickstart
+## ⚙️ Getting Started
 > **Step 0** - Install Python 3.11 or later. [See here](https://www.tutorialsteacher.com/python/install-python) for a step-by-step guide.
 
-<br />
-
-> **Step 1** - Download the project and navigate to its directory. You'll encounter two options: Virtual Environment and Poetry. Select either Step-2 or Step-3 based on your familiarity with each.:
+> **Step 1** - Download the project and navigate to its directory
 
 ```bash
 git clone https://github.com/assafelovic/gpt-researcher.git
 cd gpt-researcher
 ```
 
-<br />
-
-> **Step 2** - 🌐🌀 Virtual Environment 🛡️.
-
-#### *Establishing the Virtual Environment with Activate/Deactivate configuration*
-
-Create a virtual environment using the `venv` package with the environment name `<your_name>`, for example, `env`. Execute the following command in the PowerShell/CMD terminal:
-
-```bash
-python -m venv env
-```
-
-To activate the virtual environment, use the following activation script in PowerShell/CMD terminal:
-
-```bash
-.\env\Scripts\activate
-```
-
-To deactivate the virtual environment, run the following deactivation script in PowerShell/CMD terminal:
-
-```bash
-deactivate
-```
-
-#### *Install the dependencies for a Virtual environment*
-
-After activating the `env` environment, install dependencies using the `requirements.txt` file with the following command:
-
-```bash
-python -m pip install -r requirements.txt
-```
-
-<br />
-
-> **Step 3** - 📜🎭 Poetry 📝
-
-#### *Establishing the Poetry dependencies and virtual environment with Poetry version `~1.7.1`*
-
-Install project dependencies and simultaneously create a virtual environment for the specified project. By executing this command, Poetry reads the project's "pyproject.toml" file to determine the required dependencies and their versions, ensuring a consistent and isolated development environment. The virtual environment allows for a clean separation of project-specific dependencies, preventing conflicts with system-wide packages and enabling more straightforward dependency management throughout the project's lifecycle.
-
-```bash
-poetry install
-```
-
-#### *Activate the virtual environment associated with a Poetry project*
+> **Step 3** - Set up API keys using two methods: exporting them directly or storing them in a `.env` file.
 
-By running this command, the user enters a shell session within the isolated environment associated with the project, providing a dedicated space for development and execution. This virtual environment ensures that the project dependencies are encapsulated, avoiding conflicts with system-wide packages. Activating the Poetry shell is essential for seamlessly working on a project, as it ensures that the correct versions of dependencies are used and provides a controlled environment conducive to efficient development and testing.
-
-```bash
-poetry shell
-```
-
-<br />
-
-> **Step 4** - Set up API keys using two methods: exporting them directly and storing them in a `.env` file.
-
-For Linux/Temporary Windows Setup, use the export method:
+For Linux/Windows temporary setup, use the export method:
 
 ```bash
 export OPENAI_API_KEY={Your OpenAI API Key here}
 export TAVILY_API_KEY={Your Tavily API Key here}
 ```
 
-For a more permanent setup, create a `.env` file in the current `gpt-researcher` folder and input the keys as follows:
+For a more permanent setup, create a `.env` file in the current `gpt-researcher` directory and input the keys as follows:
 
 ```bash
 OPENAI_API_KEY={Your OpenAI API Key here}
 TAVILY_API_KEY={Your Tavily API Key here}
 ```
 
 - **For LLM, we recommend [OpenAI GPT](https://platform.openai.com/docs/guides/gpt)**, but you can use any other LLM model (including open sources) supported by [Langchain Adapter](https://python.langchain.com/docs/guides/adapters/openai), simply change the llm model and provider in config/config.py. 
-- **For search engine, we recommend [Tavily Search API](https://app.tavily.com)**, but you can also refer to other search engines of your choice by changing the search provider in config/config.py to `"duckduckgo"`, `"googleAPI"`, `"googleSerp"`, or `"searx"`. Then add the corresponding env API key as seen in the config.py file.
+- **For web search API, we recommend [Tavily Search API](https://app.tavily.com)**, but you can also refer to other search APIs of your choice by changing the search provider in config/config.py to `"duckduckgo"`, `"googleAPI"`, `"bing"`, `"googleSerp"`, `"searx"` and more. Then add the corresponding env API key as seen in the config.py file.
 
-<br />
+### Quickstart
+
+> **Step 1** - Install dependencies
 
-> **Step 5** - Launch the FastAPI application agent on a *Virtual Environment or Poetry* setup by executing the following command:
 ```bash
-python -m uvicorn main:app --reload
+pip install -r requirements.txt
 ```
 
-- **Issue: OSError** - For Windows 11 Pro/Home users encountering the 'OSError: cannot load library 'gobject-2.0-0'' error, please refer to [this OSError GitHub issue](https://github.com/assafelovic/gpt-researcher/issues/314). To resolve this issue, install the `WeasyPrint` software on your local machine by using the [GTK for Windows Runtime Environment Installer](https://github.com/tschoonj/GTK-for-Windows-Runtime-Environment-Installer/releases/tag/2022-01-04).
+> **Step 2** - Run the agent with FastAPI
 
-<br />
+```bash
+uvicorn main:app --reload
+```
 
-> **Step 6** - Visit http://localhost:8000 in any web browser and explore your research!
+> **Step 3** - Go to http://localhost:8000 on any browser and enjoy researching!
+
+<br />
 
-To learn how to get started with Docker or to learn more about the features and services check out the [documentation](https://docs.tavily.com) page.
+**To learn how to get started with [Docker](https://docs.tavily.com/docs/gpt-researcher/getting-started#try-it-with-docker), [Poetry](https://docs.tavily.com/docs/gpt-researcher/getting-started#poetry) or a [virtual environment](https://docs.tavily.com/docs/gpt-researcher/getting-started#virtual-environment) check out the [documentation](https://docs.tavily.com/docs/gpt-researcher/getting-started) page.**
 
 ## 🚀 Contributing
 We highly welcome contributions! Please check out [contributing](CONTRIBUTING.md) if you're interested.
 
 Please check out our [roadmap](https://trello.com/b/3O7KBePw/gpt-researcher-roadmap) page and reach out to us via our [Discord community](https://discord.gg/2pFkc83fRq) if you're interested in joining our mission.
 
 ## ✉️ Support / Contact us
@@ -196,15 +146,15 @@
 - Our email: assafelovic@gmail.com
 
 ## 🛡 Disclaimer
 
 This project, GPT Researcher, is an experimental application and is provided "as-is" without any warranty, express or implied. We are sharing codes for academic purposes under the MIT license. Nothing herein is academic advice, and NOT a recommendation to use in academic or research papers.
 
 Our view on unbiased research claims:
-1. The whole point of our scraping system is to reduce incorrect fact. How? The more sites we scrape the less chances of incorrect data. We are scraping 20 per research, the chances that they are all wrong is extremely low.
+1. The main goal of GPT Researcher is to reduce incorrect and biased facts. How? We assume that the more sites we scrape the less chances of incorrect data. By scraping over 20 sites per research, and choosing the most frequent information, the chances that they are all wrong is extremely low.
 2. We do not aim to eliminate biases; we aim to reduce it as much as possible. **We are here as a community to figure out the most effective human/llm interactions.**
 3. In research, people also tend towards biases as most have already opinions on the topics they research about. This tool scrapes many opinions and will evenly explain diverse views that a biased person would never have read.
 
 **Please note that the use of the GPT-4 language model can be expensive due to its token usage.** By utilizing this project, you acknowledge that you are responsible for monitoring and managing your own token usage and the associated costs. It is highly recommended to check your OpenAI API usage regularly and set up any necessary limits or alerts to prevent unexpected charges.
 
 ---
```

### Comparing `gpt-researcher-0.2.6/README.md` & `gpt-researcher-0.2.7/gpt_researcher.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,27 @@
+Metadata-Version: 2.1
+Name: gpt-researcher
+Version: 0.2.7
+Summary: GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.
+Home-page: https://github.com/assafelovic/gpt-researcher
+Author: Assaf Elovic
+Author-email: assaf.elovic@gmail.com
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # 🔎 GPT Researcher
-[![Official Website](https://img.shields.io/badge/Official%20Website-tavily.com-blue?style=for-the-badge&logo=world&logoColor=white)](https://tavily.com)
+[![Official Website](https://img.shields.io/badge/Official%20Website-gptr.dev-blue?style=for-the-badge&logo=world&logoColor=white)](https://gptr.dev)
 [![Discord Follow](https://dcbadge.vercel.app/api/server/2pFkc83fRq?style=for-the-badge)](https://discord.com/invite/2pFkc83fRq)
 
 [![GitHub Repo stars](https://img.shields.io/github/stars/assafelovic/gpt-researcher?style=social)](https://github.com/assafelovic/gpt-researcher)
 [![Twitter Follow](https://img.shields.io/twitter/follow/assaf_elovic?style=social)](https://twitter.com/assaf_elovic)
 [![PyPI version](https://badge.fury.io/py/gpt-researcher.svg)](https://badge.fury.io/py/gpt-researcher)
 
 <!-- MARKDOWN LINKS & IMAGES -->
@@ -19,16 +37,16 @@
 
 **Our mission is to empower individuals and organizations with accurate, unbiased, and factual information by leveraging the power of AI.**
 
 ## Why GPT Researcher?
 
 - To form objective conclusions for manual research tasks can take time, sometimes weeks to find the right resources and information.
 - Current LLMs are trained on past and outdated information, with heavy risks of hallucinations, making them almost irrelevant for research tasks.
-- Solutions that enable web search (such as ChatGPT + Web Plugin), only consider limited resources and content that in some cases result in superficial conclusions or biased answers.
-- Using only a selection of resources can create bias in determining the right conclusions for research questions or tasks. 
+- Services that enable web search (such as ChatGPT + Web Plugin), only consider limited sources and content that in some cases result in superficial and biased answers.
+- Using only a selection of web sources can create bias in determining the right conclusions for research tasks. 
 
 ## Architecture
 The main idea is to run "planner" and "execution" agents, whereas the planner generates questions to research, and the execution agents seek the most related information based on each generated research question. Finally, the planner filters and aggregates all related information and creates a research report. <br /> <br /> 
 The agents leverage both gpt3.5-turbo and gpt-4-turbo (128K context) to complete a research task. We optimize for costs using each only when necessary. **The average research task takes around 3 minutes to complete, and costs ~$0.1.**
 
 <div align="center">
 <img align="center" height="500" src="https://cowriter-images.s3.amazonaws.com/architecture.png">
@@ -39,15 +57,16 @@
 * Create a domain specific agent based on research query or task.
 * Generate a set of research questions that together form an objective opinion on any given task. 
 * For each research question, trigger a crawler agent that scrapes online resources for information relevant to the given task.
 * For each scraped resources, summarize based on relevant information and keep track of its sources.
 * Finally, filter and aggregate all summarized sources and generate a final research report.
 
 ## Demo
-https://github.com/assafelovic/gpt-researcher/assets/13554167/d5df04a9-631a-4509-aa55-2049b5a9e9bc
+https://github.com/assafelovic/gpt-researcher/assets/13554167/dd6cf08f-b31e-40c6-9907-1915f52a7110
+
 
 ## Tutorials
  - [How it Works](https://docs.tavily.com/blog/building-gpt-researcher)
  - [How to Install](https://www.loom.com/share/04ebffb6ed2a4520a27c3e3addcdde20?sid=da1848e8-b1f1-42d1-93c3-5b0b9c3b24ea)
  - [Live Demo](https://www.loom.com/share/6a3385db4e8747a1913dd85a7834846f?sid=a740fd5b-2aa3-457e-8fb7-86976f59f9b8)
 
 ## Features
@@ -64,113 +83,62 @@
 Please see [here](https://docs.tavily.com/docs/gpt-researcher/getting-started) for full documentation on:
 
 - Getting started (installation, setting up the environment, simple examples)
 - Customization and configuration
 - How-To examples (demos, integrations, docker support)
 - Reference (full API docs)
 
-## Quickstart
+## ⚙️ Getting Started
 > **Step 0** - Install Python 3.11 or later. [See here](https://www.tutorialsteacher.com/python/install-python) for a step-by-step guide.
 
-<br />
-
-> **Step 1** - Download the project and navigate to its directory. You'll encounter two options: Virtual Environment and Poetry. Select either Step-2 or Step-3 based on your familiarity with each.:
+> **Step 1** - Download the project and navigate to its directory
 
 ```bash
 git clone https://github.com/assafelovic/gpt-researcher.git
 cd gpt-researcher
 ```
 
-<br />
-
-> **Step 2** - 🌐🌀 Virtual Environment 🛡️.
-
-#### *Establishing the Virtual Environment with Activate/Deactivate configuration*
-
-Create a virtual environment using the `venv` package with the environment name `<your_name>`, for example, `env`. Execute the following command in the PowerShell/CMD terminal:
-
-```bash
-python -m venv env
-```
-
-To activate the virtual environment, use the following activation script in PowerShell/CMD terminal:
+> **Step 3** - Set up API keys using two methods: exporting them directly or storing them in a `.env` file.
 
-```bash
-.\env\Scripts\activate
-```
-
-To deactivate the virtual environment, run the following deactivation script in PowerShell/CMD terminal:
-
-```bash
-deactivate
-```
-
-#### *Install the dependencies for a Virtual environment*
-
-After activating the `env` environment, install dependencies using the `requirements.txt` file with the following command:
-
-```bash
-python -m pip install -r requirements.txt
-```
-
-<br />
-
-> **Step 3** - 📜🎭 Poetry 📝
-
-#### *Establishing the Poetry dependencies and virtual environment with Poetry version `~1.7.1`*
-
-Install project dependencies and simultaneously create a virtual environment for the specified project. By executing this command, Poetry reads the project's "pyproject.toml" file to determine the required dependencies and their versions, ensuring a consistent and isolated development environment. The virtual environment allows for a clean separation of project-specific dependencies, preventing conflicts with system-wide packages and enabling more straightforward dependency management throughout the project's lifecycle.
-
-```bash
-poetry install
-```
-
-#### *Activate the virtual environment associated with a Poetry project*
-
-By running this command, the user enters a shell session within the isolated environment associated with the project, providing a dedicated space for development and execution. This virtual environment ensures that the project dependencies are encapsulated, avoiding conflicts with system-wide packages. Activating the Poetry shell is essential for seamlessly working on a project, as it ensures that the correct versions of dependencies are used and provides a controlled environment conducive to efficient development and testing.
-
-```bash
-poetry shell
-```
-
-<br />
-
-> **Step 4** - Set up API keys using two methods: exporting them directly and storing them in a `.env` file.
-
-For Linux/Temporary Windows Setup, use the export method:
+For Linux/Windows temporary setup, use the export method:
 
 ```bash
 export OPENAI_API_KEY={Your OpenAI API Key here}
 export TAVILY_API_KEY={Your Tavily API Key here}
 ```
 
-For a more permanent setup, create a `.env` file in the current `gpt-researcher` folder and input the keys as follows:
+For a more permanent setup, create a `.env` file in the current `gpt-researcher` directory and input the keys as follows:
 
 ```bash
 OPENAI_API_KEY={Your OpenAI API Key here}
 TAVILY_API_KEY={Your Tavily API Key here}
 ```
 
 - **For LLM, we recommend [OpenAI GPT](https://platform.openai.com/docs/guides/gpt)**, but you can use any other LLM model (including open sources) supported by [Langchain Adapter](https://python.langchain.com/docs/guides/adapters/openai), simply change the llm model and provider in config/config.py. 
-- **For search engine, we recommend [Tavily Search API](https://app.tavily.com)**, but you can also refer to other search engines of your choice by changing the search provider in config/config.py to `"duckduckgo"`, `"googleAPI"`, `"googleSerp"`, or `"searx"`. Then add the corresponding env API key as seen in the config.py file.
+- **For web search API, we recommend [Tavily Search API](https://app.tavily.com)**, but you can also refer to other search APIs of your choice by changing the search provider in config/config.py to `"duckduckgo"`, `"googleAPI"`, `"bing"`, `"googleSerp"`, `"searx"` and more. Then add the corresponding env API key as seen in the config.py file.
 
-<br />
+### Quickstart
+
+> **Step 1** - Install dependencies
 
-> **Step 5** - Launch the FastAPI application agent on a *Virtual Environment or Poetry* setup by executing the following command:
 ```bash
-python -m uvicorn main:app --reload
+pip install -r requirements.txt
 ```
 
-- **Issue: OSError** - For Windows 11 Pro/Home users encountering the 'OSError: cannot load library 'gobject-2.0-0'' error, please refer to [this OSError GitHub issue](https://github.com/assafelovic/gpt-researcher/issues/314). To resolve this issue, install the `WeasyPrint` software on your local machine by using the [GTK for Windows Runtime Environment Installer](https://github.com/tschoonj/GTK-for-Windows-Runtime-Environment-Installer/releases/tag/2022-01-04).
+> **Step 2** - Run the agent with FastAPI
 
-<br />
+```bash
+uvicorn main:app --reload
+```
 
-> **Step 6** - Visit http://localhost:8000 in any web browser and explore your research!
+> **Step 3** - Go to http://localhost:8000 on any browser and enjoy researching!
+
+<br />
 
-To learn how to get started with Docker or to learn more about the features and services check out the [documentation](https://docs.tavily.com) page.
+**To learn how to get started with [Docker](https://docs.tavily.com/docs/gpt-researcher/getting-started#try-it-with-docker), [Poetry](https://docs.tavily.com/docs/gpt-researcher/getting-started#poetry) or a [virtual environment](https://docs.tavily.com/docs/gpt-researcher/getting-started#virtual-environment) check out the [documentation](https://docs.tavily.com/docs/gpt-researcher/getting-started) page.**
 
 ## 🚀 Contributing
 We highly welcome contributions! Please check out [contributing](CONTRIBUTING.md) if you're interested.
 
 Please check out our [roadmap](https://trello.com/b/3O7KBePw/gpt-researcher-roadmap) page and reach out to us via our [Discord community](https://discord.gg/2pFkc83fRq) if you're interested in joining our mission.
 
 ## ✉️ Support / Contact us
@@ -178,15 +146,15 @@
 - Our email: assafelovic@gmail.com
 
 ## 🛡 Disclaimer
 
 This project, GPT Researcher, is an experimental application and is provided "as-is" without any warranty, express or implied. We are sharing codes for academic purposes under the MIT license. Nothing herein is academic advice, and NOT a recommendation to use in academic or research papers.
 
 Our view on unbiased research claims:
-1. The whole point of our scraping system is to reduce incorrect fact. How? The more sites we scrape the less chances of incorrect data. We are scraping 20 per research, the chances that they are all wrong is extremely low.
+1. The main goal of GPT Researcher is to reduce incorrect and biased facts. How? We assume that the more sites we scrape the less chances of incorrect data. By scraping over 20 sites per research, and choosing the most frequent information, the chances that they are all wrong is extremely low.
 2. We do not aim to eliminate biases; we aim to reduce it as much as possible. **We are here as a community to figure out the most effective human/llm interactions.**
 3. In research, people also tend towards biases as most have already opinions on the topics they research about. This tool scrapes many opinions and will evenly explain diverse views that a biased person would never have read.
 
 **Please note that the use of the GPT-4 language model can be expensive due to its token usage.** By utilizing this project, you acknowledge that you are responsible for monitoring and managing your own token usage and the associated costs. It is highly recommended to check your OpenAI API usage regularly and set up any necessary limits or alerts to prevent unexpected charges.
 
 ---
```

### Comparing `gpt-researcher-0.2.6/backend/report_type/basic_report/basic_report.py` & `gpt-researcher-0.2.7/backend/report_type/basic_report/basic_report.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.6/backend/report_type/detailed_report/detailed_report.py` & `gpt-researcher-0.2.7/backend/report_type/detailed_report/detailed_report.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.6/backend/server.py` & `gpt-researcher-0.2.7/backend/server.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.6/backend/utils.py` & `gpt-researcher-0.2.7/backend/utils.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.6/backend/websocket_manager.py` & `gpt-researcher-0.2.7/backend/websocket_manager.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.6/gpt_researcher/config/config.py` & `gpt-researcher-0.2.7/gpt_researcher/config/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     def __init__(self, config_file: str = None):
         """Initialize the config class."""
         self.config_file = config_file if config_file else os.getenv('CONFIG_FILE')
         self.retriever = os.getenv('SEARCH_RETRIEVER', "tavily")
         self.embedding_provider = os.getenv('EMBEDDING_PROVIDER', 'openai')
         self.llm_provider = os.getenv('LLM_PROVIDER', "openai")
         self.fast_llm_model = os.getenv('FAST_LLM_MODEL', "gpt-3.5-turbo-16k")
-        self.smart_llm_model = os.getenv('SMART_LLM_MODEL', "gpt-4-1106-preview")
+        self.smart_llm_model = os.getenv('SMART_LLM_MODEL', "gpt-4-turbo")
         self.fast_token_limit = int(os.getenv('FAST_TOKEN_LIMIT', 2000))
         self.smart_token_limit = int(os.getenv('SMART_TOKEN_LIMIT', 4000))
         self.browse_chunk_max_length = int(os.getenv('BROWSE_CHUNK_MAX_LENGTH', 8192))
         self.summary_token_limit = int(os.getenv('SUMMARY_TOKEN_LIMIT', 700))
         self.temperature = float(os.getenv('TEMPERATURE', 0.55))
         self.user_agent = os.getenv('USER_AGENT', "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 "
                                                    "(KHTML, like Gecko) Chrome/119.0.0.0 Safari/537.36 Edg/119.0.0.0")
```

### Comparing `gpt-researcher-0.2.6/gpt_researcher/context/compression.py` & `gpt-researcher-0.2.7/gpt_researcher/context/compression.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.6/gpt_researcher/context/retriever.py` & `gpt-researcher-0.2.7/gpt_researcher/context/retriever.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.6/gpt_researcher/llm_provider/azureopenai/azureopenai.py` & `gpt-researcher-0.2.7/gpt_researcher/llm_provider/azureopenai/azureopenai.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.6/gpt_researcher/llm_provider/google/google.py` & `gpt-researcher-0.2.7/gpt_researcher/llm_provider/google/google.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.6/gpt_researcher/llm_provider/openai/openai.py` & `gpt-researcher-0.2.7/gpt_researcher/llm_provider/openai/openai.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.6/gpt_researcher/master/agent.py` & `gpt-researcher-0.2.7/gpt_researcher/master/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,24 +84,19 @@
     async def write_report(self, existing_headers: list = []):
         """
         Writes the report based on research conducted
 
         Returns:
             str: The report
         """
-        # Write Research Report
-        if self.report_type == "custom_report":
-            self.role = self.cfg.agent_role if self.cfg.agent_role else self.role
 
         await stream_output("logs", f"✍️ Writing summary for research task: {self.query}...", self.websocket)
 
         if self.report_type == "custom_report":
-            self.role = (
-                self.cfg.agent_role if self.cfg.agent_role else self.role
-            )
+            self.role = self.cfg.agent_role if self.cfg.agent_role else self.role
         elif self.report_type == "subtopic_report":
             report = await generate_report(
                 query=self.query,
                 context=self.context,
                 agent_role_prompt=self.role,
                 report_type=self.report_type,
                 websocket=self.websocket,
```

### Comparing `gpt-researcher-0.2.6/gpt_researcher/master/functions.py` & `gpt-researcher-0.2.7/gpt_researcher/master/functions.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.6/gpt_researcher/master/prompts.py` & `gpt-researcher-0.2.7/gpt_researcher/master/prompts.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
         parent_query (str): The main question (only relevant for detailed reports)
         report_type (str): The report type
         max_iterations (int): The maximum number of search queries to generate
     
     Returns: str: The search queries prompt for the given question
     """
     
-    if report_type == ReportType.DetailedReport.value:
-        task = f"{parent_query} : {question}"
+    if report_type == ReportType.DetailedReport.value or report_type == ReportType.SubtopicReport.value:
+        task = f"{parent_query} - {question}"
     else:
         task = question
 
     return f'Write {max_iterations} google search queries to search online that form an objective opinion from the following task: "{task}"' \
            f'Use the current date if needed: {datetime.now().strftime("%B %d, %Y")}.\n' \
            f'Also include in the queries specified task details such as locations, names, etc.\n' \
            f'You must respond with a list of strings in the following format: ["query 1", "query 2", "query 3"].'
```

### Comparing `gpt-researcher-0.2.6/gpt_researcher/memory/embeddings.py` & `gpt-researcher-0.2.7/gpt_researcher/memory/embeddings.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.6/gpt_researcher/retrievers/bing/bing.py` & `gpt-researcher-0.2.7/gpt_researcher/retrievers/bing/bing.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.6/gpt_researcher/retrievers/google/google.py` & `gpt-researcher-0.2.7/gpt_researcher/retrievers/google/google.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.6/gpt_researcher/retrievers/searx/searx.py` & `gpt-researcher-0.2.7/gpt_researcher/retrievers/searx/searx.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.6/gpt_researcher/retrievers/serpapi/serpapi.py` & `gpt-researcher-0.2.7/gpt_researcher/retrievers/serpapi/serpapi.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.6/gpt_researcher/retrievers/serper/serper.py` & `gpt-researcher-0.2.7/gpt_researcher/retrievers/serper/serper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.6/gpt_researcher/retrievers/tavily_news/tavily_news.py` & `gpt-researcher-0.2.7/gpt_researcher/retrievers/tavily_news/tavily_news.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.6/gpt_researcher/retrievers/tavily_search/tavily_search.py` & `gpt-researcher-0.2.7/gpt_researcher/retrievers/tavily_search/tavily_search.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.6/gpt_researcher/scraper/arxiv/arxiv.py` & `gpt-researcher-0.2.7/gpt_researcher/scraper/arxiv/arxiv.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.6/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py` & `gpt-researcher-0.2.7/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.6/gpt_researcher/scraper/newspaper/newspaper.py` & `gpt-researcher-0.2.7/gpt_researcher/scraper/newspaper/newspaper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.6/gpt_researcher/scraper/pymupdf/pymupdf.py` & `gpt-researcher-0.2.7/gpt_researcher/scraper/pymupdf/pymupdf.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.6/gpt_researcher/scraper/scraper.py` & `gpt-researcher-0.2.7/gpt_researcher/scraper/scraper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.6/gpt_researcher/scraper/web_base_loader/web_base_loader.py` & `gpt-researcher-0.2.7/gpt_researcher/scraper/web_base_loader/web_base_loader.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.6/gpt_researcher/utils/llm.py` & `gpt-researcher-0.2.7/gpt_researcher/utils/llm.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.6/gpt_researcher.egg-info/PKG-INFO` & `gpt-researcher-0.2.7/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,9 @@
-Metadata-Version: 2.1
-Name: gpt-researcher
-Version: 0.2.6
-Summary: GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.
-Home-page: https://github.com/assafelovic/gpt-researcher
-Author: Assaf Elovic
-Author-email: assaf.elovic@gmail.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # 🔎 GPT Researcher
-[![Official Website](https://img.shields.io/badge/Official%20Website-tavily.com-blue?style=for-the-badge&logo=world&logoColor=white)](https://tavily.com)
+[![Official Website](https://img.shields.io/badge/Official%20Website-gptr.dev-blue?style=for-the-badge&logo=world&logoColor=white)](https://gptr.dev)
 [![Discord Follow](https://dcbadge.vercel.app/api/server/2pFkc83fRq?style=for-the-badge)](https://discord.com/invite/2pFkc83fRq)
 
 [![GitHub Repo stars](https://img.shields.io/github/stars/assafelovic/gpt-researcher?style=social)](https://github.com/assafelovic/gpt-researcher)
 [![Twitter Follow](https://img.shields.io/twitter/follow/assaf_elovic?style=social)](https://twitter.com/assaf_elovic)
 [![PyPI version](https://badge.fury.io/py/gpt-researcher.svg)](https://badge.fury.io/py/gpt-researcher)
 
 <!-- MARKDOWN LINKS & IMAGES -->
@@ -37,16 +19,16 @@
 
 **Our mission is to empower individuals and organizations with accurate, unbiased, and factual information by leveraging the power of AI.**
 
 ## Why GPT Researcher?
 
 - To form objective conclusions for manual research tasks can take time, sometimes weeks to find the right resources and information.
 - Current LLMs are trained on past and outdated information, with heavy risks of hallucinations, making them almost irrelevant for research tasks.
-- Solutions that enable web search (such as ChatGPT + Web Plugin), only consider limited resources and content that in some cases result in superficial conclusions or biased answers.
-- Using only a selection of resources can create bias in determining the right conclusions for research questions or tasks. 
+- Services that enable web search (such as ChatGPT + Web Plugin), only consider limited sources and content that in some cases result in superficial and biased answers.
+- Using only a selection of web sources can create bias in determining the right conclusions for research tasks. 
 
 ## Architecture
 The main idea is to run "planner" and "execution" agents, whereas the planner generates questions to research, and the execution agents seek the most related information based on each generated research question. Finally, the planner filters and aggregates all related information and creates a research report. <br /> <br /> 
 The agents leverage both gpt3.5-turbo and gpt-4-turbo (128K context) to complete a research task. We optimize for costs using each only when necessary. **The average research task takes around 3 minutes to complete, and costs ~$0.1.**
 
 <div align="center">
 <img align="center" height="500" src="https://cowriter-images.s3.amazonaws.com/architecture.png">
@@ -57,15 +39,16 @@
 * Create a domain specific agent based on research query or task.
 * Generate a set of research questions that together form an objective opinion on any given task. 
 * For each research question, trigger a crawler agent that scrapes online resources for information relevant to the given task.
 * For each scraped resources, summarize based on relevant information and keep track of its sources.
 * Finally, filter and aggregate all summarized sources and generate a final research report.
 
 ## Demo
-https://github.com/assafelovic/gpt-researcher/assets/13554167/d5df04a9-631a-4509-aa55-2049b5a9e9bc
+https://github.com/assafelovic/gpt-researcher/assets/13554167/dd6cf08f-b31e-40c6-9907-1915f52a7110
+
 
 ## Tutorials
  - [How it Works](https://docs.tavily.com/blog/building-gpt-researcher)
  - [How to Install](https://www.loom.com/share/04ebffb6ed2a4520a27c3e3addcdde20?sid=da1848e8-b1f1-42d1-93c3-5b0b9c3b24ea)
  - [Live Demo](https://www.loom.com/share/6a3385db4e8747a1913dd85a7834846f?sid=a740fd5b-2aa3-457e-8fb7-86976f59f9b8)
 
 ## Features
@@ -82,113 +65,62 @@
 Please see [here](https://docs.tavily.com/docs/gpt-researcher/getting-started) for full documentation on:
 
 - Getting started (installation, setting up the environment, simple examples)
 - Customization and configuration
 - How-To examples (demos, integrations, docker support)
 - Reference (full API docs)
 
-## Quickstart
+## ⚙️ Getting Started
 > **Step 0** - Install Python 3.11 or later. [See here](https://www.tutorialsteacher.com/python/install-python) for a step-by-step guide.
 
-<br />
-
-> **Step 1** - Download the project and navigate to its directory. You'll encounter two options: Virtual Environment and Poetry. Select either Step-2 or Step-3 based on your familiarity with each.:
+> **Step 1** - Download the project and navigate to its directory
 
 ```bash
 git clone https://github.com/assafelovic/gpt-researcher.git
 cd gpt-researcher
 ```
 
-<br />
-
-> **Step 2** - 🌐🌀 Virtual Environment 🛡️.
-
-#### *Establishing the Virtual Environment with Activate/Deactivate configuration*
-
-Create a virtual environment using the `venv` package with the environment name `<your_name>`, for example, `env`. Execute the following command in the PowerShell/CMD terminal:
-
-```bash
-python -m venv env
-```
-
-To activate the virtual environment, use the following activation script in PowerShell/CMD terminal:
+> **Step 3** - Set up API keys using two methods: exporting them directly or storing them in a `.env` file.
 
-```bash
-.\env\Scripts\activate
-```
-
-To deactivate the virtual environment, run the following deactivation script in PowerShell/CMD terminal:
-
-```bash
-deactivate
-```
-
-#### *Install the dependencies for a Virtual environment*
-
-After activating the `env` environment, install dependencies using the `requirements.txt` file with the following command:
-
-```bash
-python -m pip install -r requirements.txt
-```
-
-<br />
-
-> **Step 3** - 📜🎭 Poetry 📝
-
-#### *Establishing the Poetry dependencies and virtual environment with Poetry version `~1.7.1`*
-
-Install project dependencies and simultaneously create a virtual environment for the specified project. By executing this command, Poetry reads the project's "pyproject.toml" file to determine the required dependencies and their versions, ensuring a consistent and isolated development environment. The virtual environment allows for a clean separation of project-specific dependencies, preventing conflicts with system-wide packages and enabling more straightforward dependency management throughout the project's lifecycle.
-
-```bash
-poetry install
-```
-
-#### *Activate the virtual environment associated with a Poetry project*
-
-By running this command, the user enters a shell session within the isolated environment associated with the project, providing a dedicated space for development and execution. This virtual environment ensures that the project dependencies are encapsulated, avoiding conflicts with system-wide packages. Activating the Poetry shell is essential for seamlessly working on a project, as it ensures that the correct versions of dependencies are used and provides a controlled environment conducive to efficient development and testing.
-
-```bash
-poetry shell
-```
-
-<br />
-
-> **Step 4** - Set up API keys using two methods: exporting them directly and storing them in a `.env` file.
-
-For Linux/Temporary Windows Setup, use the export method:
+For Linux/Windows temporary setup, use the export method:
 
 ```bash
 export OPENAI_API_KEY={Your OpenAI API Key here}
 export TAVILY_API_KEY={Your Tavily API Key here}
 ```
 
-For a more permanent setup, create a `.env` file in the current `gpt-researcher` folder and input the keys as follows:
+For a more permanent setup, create a `.env` file in the current `gpt-researcher` directory and input the keys as follows:
 
 ```bash
 OPENAI_API_KEY={Your OpenAI API Key here}
 TAVILY_API_KEY={Your Tavily API Key here}
 ```
 
 - **For LLM, we recommend [OpenAI GPT](https://platform.openai.com/docs/guides/gpt)**, but you can use any other LLM model (including open sources) supported by [Langchain Adapter](https://python.langchain.com/docs/guides/adapters/openai), simply change the llm model and provider in config/config.py. 
-- **For search engine, we recommend [Tavily Search API](https://app.tavily.com)**, but you can also refer to other search engines of your choice by changing the search provider in config/config.py to `"duckduckgo"`, `"googleAPI"`, `"googleSerp"`, or `"searx"`. Then add the corresponding env API key as seen in the config.py file.
+- **For web search API, we recommend [Tavily Search API](https://app.tavily.com)**, but you can also refer to other search APIs of your choice by changing the search provider in config/config.py to `"duckduckgo"`, `"googleAPI"`, `"bing"`, `"googleSerp"`, `"searx"` and more. Then add the corresponding env API key as seen in the config.py file.
 
-<br />
+### Quickstart
+
+> **Step 1** - Install dependencies
 
-> **Step 5** - Launch the FastAPI application agent on a *Virtual Environment or Poetry* setup by executing the following command:
 ```bash
-python -m uvicorn main:app --reload
+pip install -r requirements.txt
 ```
 
-- **Issue: OSError** - For Windows 11 Pro/Home users encountering the 'OSError: cannot load library 'gobject-2.0-0'' error, please refer to [this OSError GitHub issue](https://github.com/assafelovic/gpt-researcher/issues/314). To resolve this issue, install the `WeasyPrint` software on your local machine by using the [GTK for Windows Runtime Environment Installer](https://github.com/tschoonj/GTK-for-Windows-Runtime-Environment-Installer/releases/tag/2022-01-04).
+> **Step 2** - Run the agent with FastAPI
 
-<br />
+```bash
+uvicorn main:app --reload
+```
 
-> **Step 6** - Visit http://localhost:8000 in any web browser and explore your research!
+> **Step 3** - Go to http://localhost:8000 on any browser and enjoy researching!
+
+<br />
 
-To learn how to get started with Docker or to learn more about the features and services check out the [documentation](https://docs.tavily.com) page.
+**To learn how to get started with [Docker](https://docs.tavily.com/docs/gpt-researcher/getting-started#try-it-with-docker), [Poetry](https://docs.tavily.com/docs/gpt-researcher/getting-started#poetry) or a [virtual environment](https://docs.tavily.com/docs/gpt-researcher/getting-started#virtual-environment) check out the [documentation](https://docs.tavily.com/docs/gpt-researcher/getting-started) page.**
 
 ## 🚀 Contributing
 We highly welcome contributions! Please check out [contributing](CONTRIBUTING.md) if you're interested.
 
 Please check out our [roadmap](https://trello.com/b/3O7KBePw/gpt-researcher-roadmap) page and reach out to us via our [Discord community](https://discord.gg/2pFkc83fRq) if you're interested in joining our mission.
 
 ## ✉️ Support / Contact us
@@ -196,15 +128,15 @@
 - Our email: assafelovic@gmail.com
 
 ## 🛡 Disclaimer
 
 This project, GPT Researcher, is an experimental application and is provided "as-is" without any warranty, express or implied. We are sharing codes for academic purposes under the MIT license. Nothing herein is academic advice, and NOT a recommendation to use in academic or research papers.
 
 Our view on unbiased research claims:
-1. The whole point of our scraping system is to reduce incorrect fact. How? The more sites we scrape the less chances of incorrect data. We are scraping 20 per research, the chances that they are all wrong is extremely low.
+1. The main goal of GPT Researcher is to reduce incorrect and biased facts. How? We assume that the more sites we scrape the less chances of incorrect data. By scraping over 20 sites per research, and choosing the most frequent information, the chances that they are all wrong is extremely low.
 2. We do not aim to eliminate biases; we aim to reduce it as much as possible. **We are here as a community to figure out the most effective human/llm interactions.**
 3. In research, people also tend towards biases as most have already opinions on the topics they research about. This tool scrapes many opinions and will evenly explain diverse views that a biased person would never have read.
 
 **Please note that the use of the GPT-4 language model can be expensive due to its token usage.** By utilizing this project, you acknowledge that you are responsible for monitoring and managing your own token usage and the associated costs. It is highly recommended to check your OpenAI API usage regularly and set up any necessary limits or alerts to prevent unexpected charges.
 
 ---
```

### Comparing `gpt-researcher-0.2.6/gpt_researcher.egg-info/SOURCES.txt` & `gpt-researcher-0.2.7/gpt_researcher.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -63,8 +63,21 @@
 gpt_researcher/scraper/pymupdf/__init__.py
 gpt_researcher/scraper/pymupdf/pymupdf.py
 gpt_researcher/scraper/web_base_loader/__init__.py
 gpt_researcher/scraper/web_base_loader/web_base_loader.py
 gpt_researcher/utils/__init__.py
 gpt_researcher/utils/enum.py
 gpt_researcher/utils/llm.py
-gpt_researcher/utils/validators.py
+gpt_researcher/utils/validators.py
+multi_agents/__init__.py
+multi_agents/main.py
+multi_agents/agents/__init__.py
+multi_agents/agents/critique.py
+multi_agents/agents/curator.py
+multi_agents/agents/editor.py
+multi_agents/agents/master.py
+multi_agents/agents/publisher.py
+multi_agents/agents/researcher.py
+multi_agents/agents/reviser.py
+multi_agents/agents/writer.py
+multi_agents/agents/utils/__init__.py
+multi_agents/agents/utils/file_utils.py
```

### Comparing `gpt-researcher-0.2.6/pyproject.toml` & `gpt-researcher-0.2.7/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -12,22 +12,21 @@
 colorama = ">=0.4.6"
 duckduckgo_search = ">=4.1.1"
 md2pdf = ">=1.0.1"
 openai = ">=1.3.3"
 playwright = ">=1.39.0"
 python-dotenv = ">=1.0.0"
 pyyaml = ">=6.0.1"
-selenium = ">=4.15.2"
-webdriver-manager = ">=4.0.1"
 uvicorn = ">=0.24.0.post1"
 pydantic = ">=2.5.1"
 fastapi = ">=0.104.1"
 python-multipart = ">=0.0.6"
 markdown = ">=3.5.1"
 langchain = ">=0.0.350"
+langgraph = ">=0.0.29"
 tavily-python = ">=0.2.8"
 permchain = ">=0.0.6"
 arxiv = ">=2.0.0"
 PyMuPDF = ">=1.23.6"
 requests = ">=2.31.0"
 jinja2 = ">=3.1.2"
 aiofiles = ">=23.2.1"
@@ -35,12 +34,12 @@
 langchain_community = ">=0.0.28"
 SQLAlchemy = ">=2.0.28"
 mistune = "^3.0.2"
 htmldocx = "^0.0.6"
 python-docx = "^1.1.0"
 langchain-openai = "^0.1.0"
 langchain-google-genai = "^0.0.11"
-
+lxml = { version = ">=4.9.2", extras = ["html_clean"] }
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `gpt-researcher-0.2.6/setup.py` & `gpt-researcher-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open("requirements.txt", "r") as f:
     reqs = [line.strip() for line in f if ('selenium' not in line and 'webdriver' not in line)]
 
 setup(
     name="gpt-researcher",
-    version="0.2.6",
+    version="0.2.7",
     description="GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.",
     package_dir={'gpt_researcher': 'gpt_researcher'},
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/assafelovic/gpt-researcher",
     author="Assaf Elovic",
```

