# Comparing `tmp/athena_intelligence-0.1.50.tar.gz` & `tmp/athena_intelligence-0.1.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athena_intelligence-0.1.50.tar", max compression
+gzip compressed data, was "athena_intelligence-0.1.51.tar", max compression
```

## Comparing `athena_intelligence-0.1.50.tar` & `athena_intelligence-0.1.51.tar`

### file list

```diff
@@ -1,65 +1,66 @@
--rw-r--r--   0        0        0     4235 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/README.md
--rw-r--r--   0        0        0      603 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/pyproject.toml
--rw-r--r--   0        0        0     1547 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/__init__.py
--rw-r--r--   0        0        0     6860 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/base_client.py
--rw-r--r--   0        0        0       65 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/chain/__init__.py
--rw-r--r--   0        0        0     8024 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/chain/client.py
--rw-r--r--   0        0        0     3576 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/client.py
--rw-r--r--   0        0        0      853 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/core/api_error.py
--rw-r--r--   0        0        0     1495 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/core/file.py
--rw-r--r--   0        0        0     5059 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/core/jsonable_encoder.py
--rw-r--r--   0        0        0      329 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/core/pydantic_utilities.py
--rw-r--r--   0        0        0      330 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/core/request_options.py
--rw-r--r--   0        0        0       65 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/dataset/__init__.py
--rw-r--r--   0        0        0     6182 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/dataset/client.py
--rw-r--r--   0        0        0      165 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/environment.py
--rw-r--r--   0        0        0      170 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/errors/__init__.py
--rw-r--r--   0        0        0      313 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0       65 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/message/__init__.py
--rw-r--r--   0        0        0    12498 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/message/client.py
--rw-r--r--   0        0        0     3998 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/polling_message_client.py
--rw-r--r--   0        0        0        0 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/py.typed
--rw-r--r--   0        0        0       65 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/query/__init__.py
--rw-r--r--   0        0        0     6338 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/query/client.py
--rw-r--r--   0        0        0       65 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/report/__init__.py
--rw-r--r--   0        0        0     6623 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/report/client.py
--rw-r--r--   0        0        0       65 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/search/__init__.py
--rw-r--r--   0        0        0     7610 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/search/client.py
--rw-r--r--   0        0        0       65 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/snippet/__init__.py
--rw-r--r--   0        0        0     6182 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/snippet/client.py
--rw-r--r--   0        0        0       65 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/tasks/__init__.py
--rw-r--r--   0        0        0     8214 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/tasks/client.py
--rw-r--r--   0        0        0       65 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/tools/__init__.py
--rw-r--r--   0        0        0    20114 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/tools/client.py
--rw-r--r--   0        0        0     1722 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/types/__init__.py
--rw-r--r--   0        0        0      994 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/types/dataset.py
--rw-r--r--   0        0        0     1061 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/types/document.py
--rw-r--r--   0        0        0      875 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/types/excecute_tool_first_workflow_out.py
--rw-r--r--   0        0        0     1001 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/types/firecrawl_scrape_url_data_reponse_dto.py
--rw-r--r--   0        0        0     1143 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/types/firecrawl_scrape_url_metadata.py
--rw-r--r--   0        0        0      969 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/types/get_datasets_response.py
--rw-r--r--   0        0        0      969 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/types/get_snippets_response.py
--rw-r--r--   0        0        0      953 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/types/http_validation_error.py
--rw-r--r--   0        0        0      919 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/types/langchain_documents_request_out.py
--rw-r--r--   0        0        0     4101 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/types/llm_model.py
--rw-r--r--   0        0        0      845 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/types/message_out.py
--rw-r--r--   0        0        0     1031 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/types/message_out_dto.py
--rw-r--r--   0        0        0     2991 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/types/model.py
--rw-r--r--   0        0        0     1034 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/types/plan_execute_out.py
--rw-r--r--   0        0        0      926 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/types/report.py
--rw-r--r--   0        0        0     1106 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/types/snippet.py
--rw-r--r--   0        0        0      880 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/types/sql_results.py
--rw-r--r--   0        0        0      672 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/types/status_enum.py
--rw-r--r--   0        0        0      885 2024-04-24 20:50:10.423406 athena_intelligence-0.1.50/src/athena/types/structured_parse_result.py
--rw-r--r--   0        0        0     1829 2024-04-24 20:50:10.427406 athena_intelligence-0.1.50/src/athena/types/tool_models.py
--rw-r--r--   0        0        0     1422 2024-04-24 20:50:10.427406 athena_intelligence-0.1.50/src/athena/types/tools.py
--rw-r--r--   0        0        0      873 2024-04-24 20:50:10.427406 athena_intelligence-0.1.50/src/athena/types/url_result.py
--rw-r--r--   0        0        0      972 2024-04-24 20:50:10.427406 athena_intelligence-0.1.50/src/athena/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-04-24 20:50:10.427406 athena_intelligence-0.1.50/src/athena/types/validation_error_loc_item.py
--rw-r--r--   0        0        0       87 2024-04-24 20:50:10.427406 athena_intelligence-0.1.50/src/athena/version.py
--rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 athena_intelligence-0.1.50/PKG-INFO
+-rw-r--r--   0        0        0     4235 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/README.md
+-rw-r--r--   0        0        0      603 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/pyproject.toml
+-rw-r--r--   0        0        0     1595 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/__init__.py
+-rw-r--r--   0        0        0     6860 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/base_client.py
+-rw-r--r--   0        0        0       65 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/chain/__init__.py
+-rw-r--r--   0        0        0    16236 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/chain/client.py
+-rw-r--r--   0        0        0     3576 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/client.py
+-rw-r--r--   0        0        0      853 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/core/api_error.py
+-rw-r--r--   0        0        0     1495 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/core/file.py
+-rw-r--r--   0        0        0     5059 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      329 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/core/request_options.py
+-rw-r--r--   0        0        0       65 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/dataset/__init__.py
+-rw-r--r--   0        0        0     6182 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/dataset/client.py
+-rw-r--r--   0        0        0      165 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/environment.py
+-rw-r--r--   0        0        0      170 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/errors/__init__.py
+-rw-r--r--   0        0        0      313 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0       65 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/message/__init__.py
+-rw-r--r--   0        0        0    12498 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/message/client.py
+-rw-r--r--   0        0        0     3998 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/polling_message_client.py
+-rw-r--r--   0        0        0        0 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/py.typed
+-rw-r--r--   0        0        0       65 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/query/__init__.py
+-rw-r--r--   0        0        0     6338 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/query/client.py
+-rw-r--r--   0        0        0       65 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/report/__init__.py
+-rw-r--r--   0        0        0     6623 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/report/client.py
+-rw-r--r--   0        0        0       65 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/search/__init__.py
+-rw-r--r--   0        0        0     7610 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/search/client.py
+-rw-r--r--   0        0        0       65 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/snippet/__init__.py
+-rw-r--r--   0        0        0     6182 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/snippet/client.py
+-rw-r--r--   0        0        0       65 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/tasks/__init__.py
+-rw-r--r--   0        0        0     8234 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/tasks/client.py
+-rw-r--r--   0        0        0       65 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/tools/__init__.py
+-rw-r--r--   0        0        0    20114 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/tools/client.py
+-rw-r--r--   0        0        0     1799 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/types/__init__.py
+-rw-r--r--   0        0        0      994 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/types/dataset.py
+-rw-r--r--   0        0        0     1061 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/types/document.py
+-rw-r--r--   0        0        0      875 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/types/excecute_tool_first_workflow_out.py
+-rw-r--r--   0        0        0     1001 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/types/firecrawl_scrape_url_data_reponse_dto.py
+-rw-r--r--   0        0        0     1143 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/types/firecrawl_scrape_url_metadata.py
+-rw-r--r--   0        0        0      969 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/types/get_datasets_response.py
+-rw-r--r--   0        0        0      969 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/types/get_snippets_response.py
+-rw-r--r--   0        0        0      953 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/types/http_validation_error.py
+-rw-r--r--   0        0        0      919 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/types/langchain_documents_request_out.py
+-rw-r--r--   0        0        0     4101 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/types/llm_model.py
+-rw-r--r--   0        0        0      950 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/types/map_reduce_chain_out.py
+-rw-r--r--   0        0        0      845 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/types/message_out.py
+-rw-r--r--   0        0        0     1031 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/types/message_out_dto.py
+-rw-r--r--   0        0        0     2991 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/types/model.py
+-rw-r--r--   0        0        0     1034 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/types/plan_execute_out.py
+-rw-r--r--   0        0        0      926 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/types/report.py
+-rw-r--r--   0        0        0     1106 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/types/snippet.py
+-rw-r--r--   0        0        0      880 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/types/sql_results.py
+-rw-r--r--   0        0        0      672 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/types/status_enum.py
+-rw-r--r--   0        0        0      885 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/types/structured_parse_result.py
+-rw-r--r--   0        0        0     1829 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/types/tool_models.py
+-rw-r--r--   0        0        0     1422 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/types/tools.py
+-rw-r--r--   0        0        0      873 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/types/url_result.py
+-rw-r--r--   0        0        0      972 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0       87 2024-04-24 23:43:55.546674 athena_intelligence-0.1.51/src/athena/version.py
+-rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 athena_intelligence-0.1.51/PKG-INFO
```

### Comparing `athena_intelligence-0.1.50/README.md` & `athena_intelligence-0.1.51/README.md`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.50/pyproject.toml` & `athena_intelligence-0.1.51/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "athena-intelligence"
-version = "0.1.50"
+version = "0.1.51"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
     { include = "athena", from = "src"}
 ]
```

### Comparing `athena_intelligence-0.1.50/src/athena/__init__.py` & `athena_intelligence-0.1.51/src/athena/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     FirecrawlScrapeUrlDataReponseDto,
     FirecrawlScrapeUrlMetadata,
     GetDatasetsResponse,
     GetSnippetsResponse,
     HttpValidationError,
     LangchainDocumentsRequestOut,
     LlmModel,
+    MapReduceChainOut,
     MessageOut,
     MessageOutDto,
     Model,
     PlanExecuteOut,
     Report,
     Snippet,
     SqlResults,
@@ -39,14 +40,15 @@
     "FirecrawlScrapeUrlDataReponseDto",
     "FirecrawlScrapeUrlMetadata",
     "GetDatasetsResponse",
     "GetSnippetsResponse",
     "HttpValidationError",
     "LangchainDocumentsRequestOut",
     "LlmModel",
+    "MapReduceChainOut",
     "MessageOut",
     "MessageOutDto",
     "Model",
     "PlanExecuteOut",
     "Report",
     "Snippet",
     "SqlResults",
```

### Comparing `athena_intelligence-0.1.50/src/athena/base_client.py` & `athena_intelligence-0.1.51/src/athena/base_client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.50/src/athena/chain/client.py` & `athena_intelligence-0.1.51/src/athena/query/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,65 +8,55 @@
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
 from ..core.pydantic_utilities import pydantic_v1
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
 from ..types.http_validation_error import HttpValidationError
-from ..types.llm_model import LlmModel
-from ..types.structured_parse_result import StructuredParseResult
+from ..types.sql_results import SqlResults
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class ChainClient:
+class QueryClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def structured_parse(
-        self,
-        *,
-        text_input: str,
-        custom_type_dict: typing.Dict[str, typing.Any],
-        model: LlmModel,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> StructuredParseResult:
+    def execute(
+        self, *, sql_command: str, database_id: int, request_options: typing.Optional[RequestOptions] = None
+    ) -> SqlResults:
         """
         Parameters:
-            - text_input: str. The text input to be parsed.
+            - sql_command: str.
 
-            - custom_type_dict: typing.Dict[str, typing.Any]. A dictionary of field names and their default values.
-
-            - model: LlmModel.
+            - database_id: int.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from athena import LlmModel
         from athena.client import Athena
 
         client = Athena(
             api_key="YOUR_API_KEY",
         )
-        client.chain.structured_parse(
-            text_input='Athena is an AI-native analytics platform and artificial employee built to accelerate analytics workflows \n                by offering enterprise teams co-pilot and auto-pilot modes. Athena learns your workflow as a co-pilot, \n                allowing you to hand over controls to her for autonomous execution with confidence." \n                \n                Give me all of the modes Athena provides.',
-            custom_type_dict={"modes": {}},
-            model=LlmModel.GPT_4_TURBO,
+        client.query.execute(
+            sql_command="sql_command",
+            database_id=1,
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="POST",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/structured-parse"),
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/execute-sql"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder({"text_input": text_input, "custom_type_dict": custom_type_dict, "model": model})
+            json=jsonable_encoder({"sql_command": sql_command, "database_id": database_id})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder({"text_input": text_input, "custom_type_dict": custom_type_dict, "model": model}),
+                **jsonable_encoder({"sql_command": sql_command, "database_id": database_id}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -76,70 +66,61 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(StructuredParseResult, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(SqlResults, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(
                 pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncChainClient:
+class AsyncQueryClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def structured_parse(
-        self,
-        *,
-        text_input: str,
-        custom_type_dict: typing.Dict[str, typing.Any],
-        model: LlmModel,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> StructuredParseResult:
+    async def execute(
+        self, *, sql_command: str, database_id: int, request_options: typing.Optional[RequestOptions] = None
+    ) -> SqlResults:
         """
         Parameters:
-            - text_input: str. The text input to be parsed.
-
-            - custom_type_dict: typing.Dict[str, typing.Any]. A dictionary of field names and their default values.
+            - sql_command: str.
 
-            - model: LlmModel.
+            - database_id: int.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from athena import LlmModel
         from athena.client import AsyncAthena
 
         client = AsyncAthena(
             api_key="YOUR_API_KEY",
         )
-        await client.chain.structured_parse(
-            text_input='Athena is an AI-native analytics platform and artificial employee built to accelerate analytics workflows \n                by offering enterprise teams co-pilot and auto-pilot modes. Athena learns your workflow as a co-pilot, \n                allowing you to hand over controls to her for autonomous execution with confidence." \n                \n                Give me all of the modes Athena provides.',
-            custom_type_dict={"modes": {}},
-            model=LlmModel.GPT_4_TURBO,
+        await client.query.execute(
+            sql_command="sql_command",
+            database_id=1,
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="POST",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/structured-parse"),
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/execute-sql"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder({"text_input": text_input, "custom_type_dict": custom_type_dict, "model": model})
+            json=jsonable_encoder({"sql_command": sql_command, "database_id": database_id})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder({"text_input": text_input, "custom_type_dict": custom_type_dict, "model": model}),
+                **jsonable_encoder({"sql_command": sql_command, "database_id": database_id}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -149,15 +130,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(StructuredParseResult, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(SqlResults, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(
                 pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
```

### Comparing `athena_intelligence-0.1.50/src/athena/client.py` & `athena_intelligence-0.1.51/src/athena/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.50/src/athena/core/__init__.py` & `athena_intelligence-0.1.51/src/athena/core/__init__.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.50/src/athena/core/client_wrapper.py` & `athena_intelligence-0.1.51/src/athena/core/client_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self._base_url = base_url
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "athena-intelligence",
-            "X-Fern-SDK-Version": "0.1.50",
+            "X-Fern-SDK-Version": "0.1.51",
         }
         headers["X-API-KEY"] = self.api_key
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `athena_intelligence-0.1.50/src/athena/core/datetime_utils.py` & `athena_intelligence-0.1.51/src/athena/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.50/src/athena/core/file.py` & `athena_intelligence-0.1.51/src/athena/core/file.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.50/src/athena/core/http_client.py` & `athena_intelligence-0.1.51/src/athena/core/http_client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.50/src/athena/core/jsonable_encoder.py` & `athena_intelligence-0.1.51/src/athena/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.50/src/athena/core/request_options.py` & `athena_intelligence-0.1.51/src/athena/core/request_options.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.50/src/athena/dataset/client.py` & `athena_intelligence-0.1.51/src/athena/dataset/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.50/src/athena/message/client.py` & `athena_intelligence-0.1.51/src/athena/message/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.50/src/athena/polling_message_client.py` & `athena_intelligence-0.1.51/src/athena/polling_message_client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.50/src/athena/query/client.py` & `athena_intelligence-0.1.51/src/athena/report/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,55 +8,61 @@
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
 from ..core.pydantic_utilities import pydantic_v1
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
 from ..types.http_validation_error import HttpValidationError
-from ..types.sql_results import SqlResults
+from ..types.report import Report
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class QueryClient:
+class ReportClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def execute(
-        self, *, sql_command: str, database_id: int, request_options: typing.Optional[RequestOptions] = None
-    ) -> SqlResults:
+    def create(
+        self,
+        *,
+        name: typing.Optional[str] = OMIT,
+        workspace_access: typing.Optional[bool] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> Report:
         """
         Parameters:
-            - sql_command: str.
+            - name: typing.Optional[str].
 
-            - database_id: int.
+            - workspace_access: typing.Optional[bool].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from athena.client import Athena
 
         client = Athena(
             api_key="YOUR_API_KEY",
         )
-        client.query.execute(
-            sql_command="sql_command",
-            database_id=1,
-        )
+        client.report.create()
         """
+        _request: typing.Dict[str, typing.Any] = {}
+        if name is not OMIT:
+            _request["name"] = name
+        if workspace_access is not OMIT:
+            _request["workspace_access"] = workspace_access
         _response = self._client_wrapper.httpx_client.request(
             method="POST",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/execute-sql"),
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/report"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder({"sql_command": sql_command, "database_id": database_id})
+            json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder({"sql_command": sql_command, "database_id": database_id}),
+                **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -66,61 +72,67 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(SqlResults, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(Report, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(
                 pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncQueryClient:
+class AsyncReportClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def execute(
-        self, *, sql_command: str, database_id: int, request_options: typing.Optional[RequestOptions] = None
-    ) -> SqlResults:
+    async def create(
+        self,
+        *,
+        name: typing.Optional[str] = OMIT,
+        workspace_access: typing.Optional[bool] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> Report:
         """
         Parameters:
-            - sql_command: str.
+            - name: typing.Optional[str].
 
-            - database_id: int.
+            - workspace_access: typing.Optional[bool].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from athena.client import AsyncAthena
 
         client = AsyncAthena(
             api_key="YOUR_API_KEY",
         )
-        await client.query.execute(
-            sql_command="sql_command",
-            database_id=1,
-        )
+        await client.report.create()
         """
+        _request: typing.Dict[str, typing.Any] = {}
+        if name is not OMIT:
+            _request["name"] = name
+        if workspace_access is not OMIT:
+            _request["workspace_access"] = workspace_access
         _response = await self._client_wrapper.httpx_client.request(
             method="POST",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/execute-sql"),
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/report"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder({"sql_command": sql_command, "database_id": database_id})
+            json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder({"sql_command": sql_command, "database_id": database_id}),
+                **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -130,15 +142,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(SqlResults, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(Report, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(
                 pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
```

### Comparing `athena_intelligence-0.1.50/src/athena/report/client.py` & `athena_intelligence-0.1.51/src/athena/snippet/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,64 +7,60 @@
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
 from ..core.pydantic_utilities import pydantic_v1
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
+from ..types.get_snippets_response import GetSnippetsResponse
 from ..types.http_validation_error import HttpValidationError
-from ..types.report import Report
 
-# this is used as the default value for optional parameters
-OMIT = typing.cast(typing.Any, ...)
 
-
-class ReportClient:
+class SnippetClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def create(
+    def get(
         self,
         *,
-        name: typing.Optional[str] = OMIT,
-        workspace_access: typing.Optional[bool] = OMIT,
+        page: typing.Optional[int] = None,
+        page_size: typing.Optional[int] = None,
         request_options: typing.Optional[RequestOptions] = None,
-    ) -> Report:
+    ) -> GetSnippetsResponse:
         """
         Parameters:
-            - name: typing.Optional[str].
+            - page: typing.Optional[int]. Page number starting from 1
 
-            - workspace_access: typing.Optional[bool].
+            - page_size: typing.Optional[int]. Number of items per page
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from athena.client import Athena
 
         client = Athena(
             api_key="YOUR_API_KEY",
         )
-        client.report.create()
+        client.snippet.get()
         """
-        _request: typing.Dict[str, typing.Any] = {}
-        if name is not OMIT:
-            _request["name"] = name
-        if workspace_access is not OMIT:
-            _request["workspace_access"] = workspace_access
         _response = self._client_wrapper.httpx_client.request(
-            method="POST",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/report"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/snippets"),
             params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+                remove_none_from_dict(
+                    {
+                        "page": page,
+                        "page_size": page_size,
+                        **(
+                            request_options.get("additional_query_parameters", {})
+                            if request_options is not None
+                            else {}
+                        ),
+                    }
+                )
             ),
-            json=jsonable_encoder(_request)
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder(_request),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -72,69 +68,68 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(Report, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(GetSnippetsResponse, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(
                 pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncReportClient:
+class AsyncSnippetClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def create(
+    async def get(
         self,
         *,
-        name: typing.Optional[str] = OMIT,
-        workspace_access: typing.Optional[bool] = OMIT,
+        page: typing.Optional[int] = None,
+        page_size: typing.Optional[int] = None,
         request_options: typing.Optional[RequestOptions] = None,
-    ) -> Report:
+    ) -> GetSnippetsResponse:
         """
         Parameters:
-            - name: typing.Optional[str].
+            - page: typing.Optional[int]. Page number starting from 1
 
-            - workspace_access: typing.Optional[bool].
+            - page_size: typing.Optional[int]. Number of items per page
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from athena.client import AsyncAthena
 
         client = AsyncAthena(
             api_key="YOUR_API_KEY",
         )
-        await client.report.create()
+        await client.snippet.get()
         """
-        _request: typing.Dict[str, typing.Any] = {}
-        if name is not OMIT:
-            _request["name"] = name
-        if workspace_access is not OMIT:
-            _request["workspace_access"] = workspace_access
         _response = await self._client_wrapper.httpx_client.request(
-            method="POST",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/report"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/snippets"),
             params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+                remove_none_from_dict(
+                    {
+                        "page": page,
+                        "page_size": page_size,
+                        **(
+                            request_options.get("additional_query_parameters", {})
+                            if request_options is not None
+                            else {}
+                        ),
+                    }
+                )
             ),
-            json=jsonable_encoder(_request)
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder(_request),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -142,15 +137,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(Report, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(GetSnippetsResponse, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(
                 pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
```

### Comparing `athena_intelligence-0.1.50/src/athena/search/client.py` & `athena_intelligence-0.1.51/src/athena/search/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.50/src/athena/tasks/client.py` & `athena_intelligence-0.1.51/src/athena/tasks/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,54 +8,54 @@
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
 from ..core.pydantic_utilities import pydantic_v1
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
 from ..types.http_validation_error import HttpValidationError
-from ..types.llm_model import LlmModel
 from ..types.plan_execute_out import PlanExecuteOut
+from ..types.tool_models import ToolModels
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class TasksClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def planned_task(
         self,
         *,
-        model: LlmModel,
+        model: ToolModels,
         instructions: str,
         input_data: str,
         output_format: str,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> PlanExecuteOut:
         """
         Parameters:
-            - model: LlmModel.
+            - model: ToolModels.
 
             - instructions: str.
 
             - input_data: str.
 
             - output_format: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from athena import LlmModel
+        from athena import ToolModels
         from athena.client import Athena
 
         client = Athena(
             api_key="YOUR_API_KEY",
         )
         client.tasks.planned_task(
-            model=LlmModel.MISTRAL_LARGE_0224,
+            model=ToolModels.MISTRAL_LARGE_0224,
             instructions="summarize the content",
             input_data="Athena is an AI-native analytics platform and artificial employee built to accelerate analytics workflows by offering enterprise teams co-pilot and auto-pilot modes. Athena learns your workflow as a co-pilot, allowing you to hand over controls to her for autonomous execution with confidence.",
             output_format="return a summary in a single sentence",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="POST",
@@ -108,40 +108,40 @@
 class AsyncTasksClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def planned_task(
         self,
         *,
-        model: LlmModel,
+        model: ToolModels,
         instructions: str,
         input_data: str,
         output_format: str,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> PlanExecuteOut:
         """
         Parameters:
-            - model: LlmModel.
+            - model: ToolModels.
 
             - instructions: str.
 
             - input_data: str.
 
             - output_format: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from athena import LlmModel
+        from athena import ToolModels
         from athena.client import AsyncAthena
 
         client = AsyncAthena(
             api_key="YOUR_API_KEY",
         )
         await client.tasks.planned_task(
-            model=LlmModel.MISTRAL_LARGE_0224,
+            model=ToolModels.MISTRAL_LARGE_0224,
             instructions="summarize the content",
             input_data="Athena is an AI-native analytics platform and artificial employee built to accelerate analytics workflows by offering enterprise teams co-pilot and auto-pilot modes. Athena learns your workflow as a co-pilot, allowing you to hand over controls to her for autonomous execution with confidence.",
             output_format="return a summary in a single sentence",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="POST",
```

### Comparing `athena_intelligence-0.1.50/src/athena/tools/client.py` & `athena_intelligence-0.1.51/src/athena/tools/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.50/src/athena/types/__init__.py` & `athena_intelligence-0.1.51/src/athena/types/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from .firecrawl_scrape_url_data_reponse_dto import FirecrawlScrapeUrlDataReponseDto
 from .firecrawl_scrape_url_metadata import FirecrawlScrapeUrlMetadata
 from .get_datasets_response import GetDatasetsResponse
 from .get_snippets_response import GetSnippetsResponse
 from .http_validation_error import HttpValidationError
 from .langchain_documents_request_out import LangchainDocumentsRequestOut
 from .llm_model import LlmModel
+from .map_reduce_chain_out import MapReduceChainOut
 from .message_out import MessageOut
 from .message_out_dto import MessageOutDto
 from .model import Model
 from .plan_execute_out import PlanExecuteOut
 from .report import Report
 from .snippet import Snippet
 from .sql_results import SqlResults
@@ -32,14 +33,15 @@
     "FirecrawlScrapeUrlDataReponseDto",
     "FirecrawlScrapeUrlMetadata",
     "GetDatasetsResponse",
     "GetSnippetsResponse",
     "HttpValidationError",
     "LangchainDocumentsRequestOut",
     "LlmModel",
+    "MapReduceChainOut",
     "MessageOut",
     "MessageOutDto",
     "Model",
     "PlanExecuteOut",
     "Report",
     "Snippet",
     "SqlResults",
```

### Comparing `athena_intelligence-0.1.50/src/athena/types/dataset.py` & `athena_intelligence-0.1.51/src/athena/types/dataset.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.50/src/athena/types/document.py` & `athena_intelligence-0.1.51/src/athena/types/document.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.50/src/athena/types/excecute_tool_first_workflow_out.py` & `athena_intelligence-0.1.51/src/athena/types/excecute_tool_first_workflow_out.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.50/src/athena/types/firecrawl_scrape_url_data_reponse_dto.py` & `athena_intelligence-0.1.51/src/athena/types/firecrawl_scrape_url_data_reponse_dto.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.50/src/athena/types/firecrawl_scrape_url_metadata.py` & `athena_intelligence-0.1.51/src/athena/types/firecrawl_scrape_url_metadata.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.50/src/athena/types/get_datasets_response.py` & `athena_intelligence-0.1.51/src/athena/types/get_datasets_response.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.50/src/athena/types/get_snippets_response.py` & `athena_intelligence-0.1.51/src/athena/types/get_snippets_response.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.50/src/athena/types/http_validation_error.py` & `athena_intelligence-0.1.51/src/athena/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.50/src/athena/types/langchain_documents_request_out.py` & `athena_intelligence-0.1.51/src/athena/types/langchain_documents_request_out.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.50/src/athena/types/llm_model.py` & `athena_intelligence-0.1.51/src/athena/types/llm_model.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.50/src/athena/types/message_out.py` & `athena_intelligence-0.1.51/src/athena/types/message_out.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.50/src/athena/types/message_out_dto.py` & `athena_intelligence-0.1.51/src/athena/types/message_out_dto.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.50/src/athena/types/model.py` & `athena_intelligence-0.1.51/src/athena/types/model.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.50/src/athena/types/plan_execute_out.py` & `athena_intelligence-0.1.51/src/athena/types/plan_execute_out.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.50/src/athena/types/report.py` & `athena_intelligence-0.1.51/src/athena/types/report.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.50/src/athena/types/snippet.py` & `athena_intelligence-0.1.51/src/athena/types/snippet.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.50/src/athena/types/sql_results.py` & `athena_intelligence-0.1.51/src/athena/types/sql_results.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.50/src/athena/types/status_enum.py` & `athena_intelligence-0.1.51/src/athena/types/status_enum.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.50/src/athena/types/structured_parse_result.py` & `athena_intelligence-0.1.51/src/athena/types/structured_parse_result.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.50/src/athena/types/tool_models.py` & `athena_intelligence-0.1.51/src/athena/types/tool_models.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.50/src/athena/types/tools.py` & `athena_intelligence-0.1.51/src/athena/types/tools.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.50/src/athena/types/url_result.py` & `athena_intelligence-0.1.51/src/athena/types/url_result.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.50/src/athena/types/validation_error.py` & `athena_intelligence-0.1.51/src/athena/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.50/PKG-INFO` & `athena_intelligence-0.1.51/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athena-intelligence
-Version: 0.1.50
+Version: 0.1.51
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

