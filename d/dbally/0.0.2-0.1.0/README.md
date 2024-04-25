# Comparing `tmp/dbally-0.0.2.tar.gz` & `tmp/dbally-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbally-0.0.2.tar", last modified: Wed Apr 17 13:10:20 2024, max compression
+gzip compressed data, was "dbally-0.1.0.tar", last modified: Thu Apr 25 10:31:00 2024, max compression
```

## Comparing `dbally-0.0.2.tar` & `dbally-0.1.0.tar`

### file list

```diff
@@ -1,103 +1,113 @@
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.619255 dbally-0.0.2/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1089 2024-04-17 13:06:55.000000 dbally-0.0.2/LICENSE
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       97 2024-04-03 11:01:33.000000 dbally-0.0.2/MANIFEST.in
--rw-r--r--   0 mateusz   (1001) mateusz   (1001)     2140 2024-04-17 13:10:20.619255 dbally-0.0.2/PKG-INFO
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     6104 2024-04-17 13:06:58.000000 dbally-0.0.2/README.md
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2969 2024-04-03 11:01:33.000000 dbally-0.0.2/pyproject.toml
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1655 2024-04-17 13:10:20.623255 dbally-0.0.2/setup.cfg
--rwxrwxr-x   0 mateusz   (1001) mateusz   (1001)      150 2024-04-03 11:01:33.000000 dbally-0.0.2/setup.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.515254 dbally-0.0.2/src/
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.519254 dbally-0.0.2/src/dbally/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        5 2024-04-17 13:07:28.000000 dbally-0.0.2/src/dbally/VERSION
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      658 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      180 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/__version__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3106 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/_main.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.531254 dbally-0.0.2/src/dbally/assistants/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/assistants/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     4192 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/assistants/base.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     6238 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/assistants/openai.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.535254 dbally-0.0.2/src/dbally/audit/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      347 2024-04-10 06:42:50.000000 dbally-0.0.2/src/dbally/audit/__init__.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.539255 dbally-0.0.2/src/dbally/audit/event_handlers/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       59 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/audit/event_handlers/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2060 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/audit/event_handlers/base.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3988 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/audit/event_handlers/cli_event_handler.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2938 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/audit/event_handlers/langsmith_event_handler.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      409 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/audit/event_span.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2670 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/audit/event_tracker.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)    12040 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/collection.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.543254 dbally-0.0.2/src/dbally/data_models/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/data_models/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      838 2024-04-10 07:45:19.000000 dbally-0.0.2/src/dbally/data_models/audit.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1817 2024-04-10 07:45:19.000000 dbally-0.0.2/src/dbally/data_models/execution_result.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      610 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/data_models/llm_options.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.555255 dbally-0.0.2/src/dbally/data_models/prompts/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      522 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/data_models/prompts/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1379 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/data_models/prompts/common_validation_utils.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1948 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/data_models/prompts/iql_explainer_prompt_template.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2192 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/data_models/prompts/iql_prompt_template.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1686 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/data_models/prompts/nl_responder_prompt_template.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2638 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/data_models/prompts/prompt_template.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1777 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/data_models/prompts/view_selector_prompt_template.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.563254 dbally-0.0.2/src/dbally/embedding_client/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      132 2024-04-10 06:42:50.000000 dbally-0.0.2/src/dbally/embedding_client/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      545 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/embedding_client/base.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1661 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/embedding_client/openai.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.571255 dbally-0.0.2/src/dbally/iql/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      238 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/iql/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1510 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/iql/_exceptions.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     4839 2024-04-17 13:06:55.000000 dbally-0.0.2/src/dbally/iql/_processor.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      834 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/iql/_query.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2573 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/iql/_type_validators.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2440 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/iql/syntax.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.571255 dbally-0.0.2/src/dbally/iql_generator/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/iql_generator/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     4243 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/iql_generator/iql_generator.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.575255 dbally-0.0.2/src/dbally/llm_client/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/llm_client/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3020 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/llm_client/base.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2393 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/llm_client/openai_client.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.579255 dbally-0.0.2/src/dbally/nl_responder/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/nl_responder/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     4025 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/nl_responder/nl_responder.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2060 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/nl_responder/token_counters.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.583255 dbally-0.0.2/src/dbally/prompts/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       71 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/prompts/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2361 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/prompts/prompt_builder.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/py.typed
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.595255 dbally-0.0.2/src/dbally/similarity/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      503 2024-04-10 06:42:50.000000 dbally-0.0.2/src/dbally/similarity/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     7653 2024-04-17 13:06:55.000000 dbally-0.0.2/src/dbally/similarity/detector.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3388 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/similarity/faiss_store.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      432 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/similarity/fetcher.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2146 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/similarity/index.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3560 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/similarity/sqlalchemy_base.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1000 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/similarity/store.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.599255 dbally-0.0.2/src/dbally/utils/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/utils/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      249 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/utils/errors.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.603255 dbally-0.0.2/src/dbally/view_selection/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       99 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/view_selection/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      748 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/view_selection/base.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3012 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/view_selection/llm_view_selector.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      865 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/view_selection/random_view_selector.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.611255 dbally-0.0.2/src/dbally/views/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/views/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2879 2024-04-17 13:06:55.000000 dbally-0.0.2/src/dbally/views/base.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      414 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/views/decorators.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3422 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/views/methods_base.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3296 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/views/pandas_base.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3484 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/views/sqlalchemy_base.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.615255 dbally-0.0.2/src/dbally.egg-info/
--rw-r--r--   0 mateusz   (1001) mateusz   (1001)     2140 2024-04-17 13:10:20.000000 dbally-0.0.2/src/dbally.egg-info/PKG-INFO
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2762 2024-04-17 13:10:20.000000 dbally-0.0.2/src/dbally.egg-info/SOURCES.txt
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        1 2024-04-17 13:10:20.000000 dbally-0.0.2/src/dbally.egg-info/dependency_links.txt
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       47 2024-04-17 13:10:20.000000 dbally-0.0.2/src/dbally.egg-info/entry_points.txt
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        1 2024-01-26 12:33:13.000000 dbally-0.0.2/src/dbally.egg-info/not-zip-safe
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      496 2024-04-17 13:10:20.000000 dbally-0.0.2/src/dbally.egg-info/requires.txt
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       18 2024-04-17 13:10:20.000000 dbally-0.0.2/src/dbally.egg-info/top_level.txt
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.611255 dbally-0.0.2/src/dbally_cli/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally_cli/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      178 2024-04-17 13:06:55.000000 dbally-0.0.2/src/dbally_cli/main.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1842 2024-04-17 13:06:55.000000 dbally-0.0.2/src/dbally_cli/similarity.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.0.2/src/py.typed
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.917163 dbally-0.1.0/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1089 2024-04-19 10:03:11.000000 dbally-0.1.0/LICENSE
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       97 2024-04-03 11:01:33.000000 dbally-0.1.0/MANIFEST.in
+-rw-r--r--   0 mateusz   (1001) mateusz   (1001)     8363 2024-04-25 10:31:00.913163 dbally-0.1.0/PKG-INFO
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     6104 2024-04-19 10:03:11.000000 dbally-0.1.0/README.md
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     4477 2024-04-19 10:03:11.000000 dbally-0.1.0/pyproject.toml
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1747 2024-04-25 10:31:00.917163 dbally-0.1.0/setup.cfg
+-rwxrwxr-x   0 mateusz   (1001) mateusz   (1001)      150 2024-04-03 11:01:33.000000 dbally-0.1.0/setup.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.801161 dbally-0.1.0/src/
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.809161 dbally-0.1.0/src/dbally/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      668 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       49 2024-04-25 10:22:49.000000 dbally-0.1.0/src/dbally/__version__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2685 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/_main.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.821161 dbally-0.1.0/src/dbally/assistants/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/assistants/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     4192 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/assistants/base.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     6238 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/assistants/openai.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.825161 dbally-0.1.0/src/dbally/audit/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      347 2024-04-10 06:42:50.000000 dbally-0.1.0/src/dbally/audit/__init__.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.829161 dbally-0.1.0/src/dbally/audit/event_handlers/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       59 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/audit/event_handlers/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2060 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/audit/event_handlers/base.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3988 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/audit/event_handlers/cli_event_handler.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2938 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/audit/event_handlers/langsmith_event_handler.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      409 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/audit/event_span.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2670 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/audit/event_tracker.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)    11270 2024-04-25 10:22:49.000000 dbally-0.1.0/src/dbally/collection.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.833161 dbally-0.1.0/src/dbally/data_models/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/data_models/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      838 2024-04-10 07:45:19.000000 dbally-0.1.0/src/dbally/data_models/audit.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1729 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/data_models/execution_result.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      610 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/data_models/llm_options.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.841162 dbally-0.1.0/src/dbally/data_models/prompts/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      522 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/data_models/prompts/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1379 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/data_models/prompts/common_validation_utils.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2192 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/data_models/prompts/iql_prompt_template.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1686 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/data_models/prompts/nl_responder_prompt_template.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2638 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/data_models/prompts/prompt_template.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2028 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/data_models/prompts/query_explainer_prompt_template.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1777 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/data_models/prompts/view_selector_prompt_template.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.845162 dbally-0.1.0/src/dbally/embedding_client/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      132 2024-04-10 06:42:50.000000 dbally-0.1.0/src/dbally/embedding_client/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      545 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/embedding_client/base.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1661 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/embedding_client/openai.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.853162 dbally-0.1.0/src/dbally/iql/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      238 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/iql/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1510 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/iql/_exceptions.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     4845 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/iql/_processor.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      840 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/iql/_query.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2573 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/iql/_type_validators.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2440 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/iql/syntax.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.857162 dbally-0.1.0/src/dbally/iql_generator/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/iql_generator/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     4256 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/iql_generator/iql_generator.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.857162 dbally-0.1.0/src/dbally/llm_client/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/llm_client/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3093 2024-04-25 10:22:46.000000 dbally-0.1.0/src/dbally/llm_client/base.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2393 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/llm_client/openai_client.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.861162 dbally-0.1.0/src/dbally/nl_responder/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/nl_responder/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     4267 2024-04-22 11:03:10.000000 dbally-0.1.0/src/dbally/nl_responder/nl_responder.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2060 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/nl_responder/token_counters.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.865162 dbally-0.1.0/src/dbally/prompts/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       71 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/prompts/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2361 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/prompts/prompt_builder.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/py.typed
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.877162 dbally-0.1.0/src/dbally/similarity/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      603 2024-04-25 10:22:46.000000 dbally-0.1.0/src/dbally/similarity/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3477 2024-04-25 10:22:46.000000 dbally-0.1.0/src/dbally/similarity/chroma_store.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     7666 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/similarity/detector.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3388 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/similarity/faiss_store.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      432 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/similarity/fetcher.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2146 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/similarity/index.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3560 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/similarity/sqlalchemy_base.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1000 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/similarity/store.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.877162 dbally-0.1.0/src/dbally/utils/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/utils/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      249 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/utils/errors.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.881162 dbally-0.1.0/src/dbally/view_selection/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       99 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/view_selection/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      748 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/view_selection/base.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3012 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/view_selection/llm_view_selector.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      865 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/view_selection/random_view_selector.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.893162 dbally-0.1.0/src/dbally/views/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/views/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1161 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/views/base.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      414 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/views/decorators.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1822 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/views/exposed_functions.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.897163 dbally-0.1.0/src/dbally/views/freeform/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:22:46.000000 dbally-0.1.0/src/dbally/views/freeform/__init__.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.901162 dbally-0.1.0/src/dbally/views/freeform/text2sql/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      358 2024-04-25 10:22:46.000000 dbally-0.1.0/src/dbally/views/freeform/text2sql/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)    12232 2024-04-25 10:22:46.000000 dbally-0.1.0/src/dbally/views/freeform/text2sql/_autodiscovery.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1358 2024-04-25 10:22:46.000000 dbally-0.1.0/src/dbally/views/freeform/text2sql/_config.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      316 2024-04-25 10:22:46.000000 dbally-0.1.0/src/dbally/views/freeform/text2sql/_errors.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     4275 2024-04-25 10:22:46.000000 dbally-0.1.0/src/dbally/views/freeform/text2sql/_view.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3474 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/views/methods_base.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3296 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/views/pandas_base.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3484 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/views/sqlalchemy_base.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3521 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/views/structured.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.905163 dbally-0.1.0/src/dbally.egg-info/
+-rw-r--r--   0 mateusz   (1001) mateusz   (1001)     8363 2024-04-25 10:31:00.000000 dbally-0.1.0/src/dbally.egg-info/PKG-INFO
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3126 2024-04-25 10:31:00.000000 dbally-0.1.0/src/dbally.egg-info/SOURCES.txt
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        1 2024-04-25 10:31:00.000000 dbally-0.1.0/src/dbally.egg-info/dependency_links.txt
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       47 2024-04-25 10:31:00.000000 dbally-0.1.0/src/dbally.egg-info/entry_points.txt
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        1 2024-01-26 12:33:13.000000 dbally-0.1.0/src/dbally.egg-info/not-zip-safe
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      525 2024-04-25 10:31:00.000000 dbally-0.1.0/src/dbally.egg-info/requires.txt
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       18 2024-04-25 10:31:00.000000 dbally-0.1.0/src/dbally.egg-info/top_level.txt
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.905163 dbally-0.1.0/src/dbally_cli/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally_cli/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      178 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally_cli/main.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1842 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally_cli/similarity.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.1.0/src/py.typed
```

### Comparing `dbally-0.0.2/LICENSE` & `dbally-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbally-0.0.2/README.md` & `dbally-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `dbally-0.0.2/setup.cfg` & `dbally-0.1.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 [metadata]
 name = dbally
-version = file: src/dbally/VERSION
+version = 0.1.0
 description = "Efficient, consistent and secure library for querying structured data with natural language"
+long_description = file: README.md
+long_description_content_type = text/markdown
 author = deepsense.ai
 author_email = contact@deepsense.ai
 license = MIT
 license_files = LICENSE
 classifiers = 
 	Development Status :: 2 - Pre-Alpha
 	Environment :: Console
@@ -57,14 +59,16 @@
 	hydra-core~=1.3.2
 	loguru~=0.7.0
 	neptune~=1.6.3
 	pydantic~=2.6.1
 	pydantic-core~=2.16.2
 	pydantic-settings~=2.0.3
 	psycopg2-binary~=2.9.9
+chromadb = 
+	chromadb>=0.4.24
 
 [options.packages.find]
 where = src
 
 [bdist_wheel]
 universal = 1
```

### Comparing `dbally-0.0.2/src/dbally/__init__.py` & `dbally-0.1.0/src/dbally/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """ dbally """
 
 from dbally.data_models.execution_result import ExecutionResult
 from dbally.views import decorators
-from dbally.views.base import AbstractBaseView
 from dbally.views.methods_base import MethodsBaseView
 from dbally.views.pandas_base import DataFrameBaseView
 from dbally.views.sqlalchemy_base import SqlAlchemyBaseView
+from dbally.views.structured import BaseStructuredView
 
 from .__version__ import __version__
 from ._main import create_collection
 from .collection import Collection
 
 __all__ = [
     "__version__",
     "create_collection",
     "decorators",
     "MethodsBaseView",
     "SqlAlchemyBaseView",
     "Collection",
-    "AbstractBaseView",
+    "BaseStructuredView",
     "DataFrameBaseView",
     "ExecutionResult",
 ]
```

### Comparing `dbally-0.0.2/src/dbally/_main.py` & `dbally-0.1.0/src/dbally/_main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from typing import List, Optional
 
 from .audit.event_handlers.base import EventHandler
 from .collection import Collection
-from .iql_generator.iql_generator import IQLGenerator
 from .llm_client.base import LLMClient
 from .nl_responder.nl_responder import NLResponder
 from .view_selection.base import ViewSelector
 from .view_selection.llm_view_selector import LLMViewSelector
 
 
 def create_collection(
     name: str,
     llm_client: LLMClient,
     event_handlers: Optional[List[EventHandler]] = None,
     view_selector: Optional[ViewSelector] = None,
-    iql_generator: Optional[IQLGenerator] = None,
     nl_responder: Optional[NLResponder] = None,
 ) -> Collection:
     """
     Create a new [Collection](collection.md) that is a container for registering views and the\
     main entrypoint to db-ally features.
 
     Unlike instantiating a [Collection][dbally.Collection] directly, this function\
@@ -41,31 +39,27 @@
         queries.
         event_handlers: Event handlers used by the collection during query executions. Can be used to\
         log events as [CLIEventHandler](event_handlers/cli_handler.md) or to validate system performance as\
         [LangSmithEventHandler](event_handlers/langsmith_handler.md).
         view_selector: View selector used by the collection to select the best view for the given query.\
         If None, a new instance of [LLMViewSelector][dbally.view_selection.llm_view_selector.LLMViewSelector]\
         will be used.
-        iql_generator: IQL generator used by the collection to generate IQL queries from natural language\
-        queries. If None, a new instance of [IQLGenerator][dbally.iql_generator.iql_generator.IQLGenerator]\
-        will be used.
         nl_responder: NL responder used by the collection to respond to natural language queries. If None,\
         a new instance of [NLResponder][dbally.nl_responder.nl_responder.NLResponder] will be used.
 
     Returns:
         a new instance of db-ally Collection
 
     Raises:
         ValueError: if default LLM client is not configured
     """
     view_selector = view_selector or LLMViewSelector(llm_client=llm_client)
-    iql_generator = iql_generator or IQLGenerator(llm_client=llm_client)
     nl_responder = nl_responder or NLResponder(llm_client=llm_client)
     event_handlers = event_handlers or []
 
     return Collection(
         name,
         nl_responder=nl_responder,
         view_selector=view_selector,
-        iql_generator=iql_generator,
+        llm_client=llm_client,
         event_handlers=event_handlers,
     )
```

### Comparing `dbally-0.0.2/src/dbally/assistants/base.py` & `dbally-0.1.0/src/dbally/assistants/base.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.2/src/dbally/assistants/openai.py` & `dbally-0.1.0/src/dbally/assistants/openai.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.2/src/dbally/audit/event_handlers/base.py` & `dbally-0.1.0/src/dbally/audit/event_handlers/base.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.2/src/dbally/audit/event_handlers/cli_event_handler.py` & `dbally-0.1.0/src/dbally/audit/event_handlers/cli_event_handler.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.2/src/dbally/audit/event_handlers/langsmith_event_handler.py` & `dbally-0.1.0/src/dbally/audit/event_handlers/langsmith_event_handler.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.2/src/dbally/audit/event_tracker.py` & `dbally-0.1.0/src/dbally/audit/event_tracker.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.2/src/dbally/collection.py` & `dbally-0.1.0/src/dbally/collection.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,22 +4,21 @@
 import time
 from typing import Callable, Dict, List, Optional, Tuple, Type, TypeVar
 
 from dbally.audit.event_handlers.base import EventHandler
 from dbally.audit.event_tracker import EventTracker
 from dbally.data_models.audit import RequestEnd, RequestStart
 from dbally.data_models.execution_result import ExecutionResult
-from dbally.iql import IQLQuery
-from dbally.iql._exceptions import IQLError
-from dbally.iql_generator.iql_generator import IQLGenerator
+from dbally.llm_client.base import LLMClient
 from dbally.nl_responder.nl_responder import NLResponder
 from dbally.similarity.index import AbstractSimilarityIndex
 from dbally.utils.errors import NoViewFoundError
 from dbally.view_selection.base import ViewSelector
-from dbally.views.base import AbstractBaseView
+from dbally.views.base import BaseView
+from dbally.views.structured import BaseStructuredView
 
 
 class IndexUpdateError(Exception):
     """
     Exception for when updating any of the Collection's similarity indexes fails.
 
     Provides a dictionary mapping failed indexes to their
@@ -44,53 +43,52 @@
         function instead of instantiating this class directly.
     """
 
     def __init__(
         self,
         name: str,
         view_selector: ViewSelector,
-        iql_generator: IQLGenerator,
+        llm_client: LLMClient,
         event_handlers: List[EventHandler],
         nl_responder: NLResponder,
         n_retries: int = 3,
     ) -> None:
         """
         Args:
             name: Name of the collection is available for [Event handlers](event_handlers/index.md) and is\
             used to distinguish different db-ally runs.
             view_selector: As you register more then one [View](views/index.md) within single collection,\
             before generating the IQL query, a View that fits query the most is selected by the\
             [ViewSelector](view_selection/index.md).
-            iql_generator: Objects that translates natural language to the\
-            [Intermediate Query Language (IQL)](../concepts/iql.md)
+            llm_client: LLM client used by the collection to generate views and respond to natural language queries.
             event_handlers: Event handlers used by the collection during query executions. Can be used\
             to log events as [CLIEventHandler](event_handlers/cli_handler.md) or to validate system performance\
             as [LangSmithEventHandler](event_handlers/langsmith_handler.md).
             nl_responder: Object that translates RAW response from db-ally into natural language.
             n_retries: IQL generator may produce invalid IQL. If this is the case this argument specifies\
             how many times db-ally will try to regenerate it. Previous try with the error message is\
             appended to the chat history to guide next generations.
         """
         self.name = name
         self.n_retries = n_retries
-        self._views: Dict[str, Callable[[], AbstractBaseView]] = {}
-        self._builders: Dict[str, Callable[[], AbstractBaseView]] = {}
+        self._views: Dict[str, Callable[[], BaseView]] = {}
+        self._builders: Dict[str, Callable[[], BaseView]] = {}
         self._view_selector = view_selector
-        self._iql_generator = iql_generator
         self._nl_responder = nl_responder
         self._event_handlers = event_handlers
+        self._llm_client = llm_client
 
-    T = TypeVar("T", bound=AbstractBaseView)
+    T = TypeVar("T", bound=BaseView)
 
     def add(self, view: Type[T], builder: Optional[Callable[[], T]] = None, name: Optional[str] = None) -> None:
         """
         Register new [View](views/index.md) that will be available to query via the collection.
 
         Args:
-            view: A class inherithing from AbstractBaseView. Object of this type will be initialized during\
+            view: A class inherithing from BaseView. Object of this type will be initialized during\
             query execution. We expect Class instead of object, as otherwise Views must have been implemented\
             stateless, which would be cumbersome.
             builder: Optional factory function that will be used to create the View instance. Use it when you\
             need to pass outcome of API call or database connection to the view and it can change over time.
             name: Custom name of the view (defaults to the name of the class).
 
         Raises:
@@ -125,15 +123,15 @@
         view_instance = builder()
         if not isinstance(view_instance, view):
             raise ValueError(f"The builder function for view {name} must return an instance of {view.__name__}")
 
         self._views[name] = view
         self._builders[name] = builder
 
-    def get(self, name: str) -> AbstractBaseView:
+    def get(self, name: str) -> BaseView:
         """
         Returns an instance of the view with the given name
 
         Args:
             name: Name of the view to return
 
         Returns:
@@ -197,82 +195,68 @@
         if len(views) == 0:
             raise ValueError("Empty collection")
         if len(views) == 1:
             selected_view = next(iter(views))
         else:
             selected_view = await self._view_selector.select_view(question, views, event_tracker)
 
-        start_time_view = time.time()
         view = self.get(selected_view)
-        end_time_view = time.time()
-
-        filter_list = view.list_filters()
 
-        iql_filters, conversation = await self._iql_generator.generate_iql(
-            question=question, filters=filter_list, event_tracker=event_tracker
+        start_time_view = time.time()
+        view_result = await view.ask(
+            query=question,
+            llm_client=self._llm_client,
+            event_tracker=event_tracker,
+            n_retries=self.n_retries,
+            dry_run=dry_run,
         )
-
-        for _ in range(self.n_retries):
-            try:
-                filters = await IQLQuery.parse(iql_filters, filter_list)
-                await view.apply_filters(filters)
-                break
-            except (IQLError, ValueError) as e:
-                conversation = self._iql_generator.add_error_msg(conversation, [e])
-                iql_filters, conversation = await self._iql_generator.generate_iql(
-                    question=question,
-                    filters=filter_list,
-                    event_tracker=event_tracker,
-                    conversation=conversation,
-                )
-                continue
-
-        view_result = view.execute(dry_run=dry_run)
+        end_time_view = time.time()
 
         textual_response = None
         if not dry_run and return_natural_response:
-            textual_response = await self._nl_responder.generate_response(
-                view_result, question, iql_filters, event_tracker
-            )
+            textual_response = await self._nl_responder.generate_response(view_result, question, event_tracker)
 
         result = ExecutionResult(
             results=view_result.results,
             context=view_result.context,
             execution_time=time.time() - start_time,
             execution_time_view=end_time_view - start_time_view,
             view_name=selected_view,
-            iql_query=iql_filters,
             textual_response=textual_response,
         )
 
         await event_tracker.request_end(RequestEnd(result=result))
 
         return result
 
     def get_similarity_indexes(self) -> Dict[AbstractSimilarityIndex, List[Tuple[str, str, str]]]:
         """
-        List all similarity indexes from all views in the collection.
+        List all similarity indexes from all structured views in the collection.
 
         Returns:
             Dictionary with similarity indexes as keys and values containing lists of places where they are used
             (represented by a tupple containing view name, method name and argument name)
         """
         indexes: Dict[AbstractSimilarityIndex, List[Tuple[str, str, str]]] = {}
         for view_name in self._views:
             view = self.get(view_name)
+
+            if not isinstance(view, BaseStructuredView):
+                continue
+
             filters = view.list_filters()
             for filter_ in filters:
                 for param in filter_.parameters:
                     if param.similarity_index:
                         indexes.setdefault(param.similarity_index, []).append((view_name, filter_.name, param.name))
         return indexes
 
     async def update_similarity_indexes(self) -> None:
         """
-        Update all similarity indexes from all views in the collection.
+        Update all similarity indexes from all structured views in the collection.
 
         Raises:
             IndexUpdateError: if updating any of the indexes fails. The exception provides `failed_indexes` attribute,
                 a dictionary mapping failed indexes to their respective exceptions. Indexes not present in
                 the dictionary were updated successfully.
         """
         indexes = self.get_similarity_indexes()
```

### Comparing `dbally-0.0.2/src/dbally/data_models/audit.py` & `dbally-0.1.0/src/dbally/data_models/audit.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.2/src/dbally/data_models/execution_result.py` & `dbally-0.1.0/src/dbally/data_models/execution_result.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,19 +28,17 @@
             The exact structure of the result set depends on the view that was used to execute the query,
             which can be obtained from the `view_name` attribute.
         context: Dictionary containing addtional metadata about the query execution.
         execution_time: Time taken to execute the entire query, including view selection
             and all other operations, in seconds.
         execution_time_view: Time taken that the selected view took to execute the query, in seconds.
         view_name: Name of the view that was used to execute the query.
-        iql_query: The IQL query that was used to execute the query.
         textual_response: Optional text response that can be used to display the query results
             in a human-readable format.
     """
 
     results: List[Dict[str, Any]]
     context: Dict[str, Any]
     execution_time: float
     execution_time_view: float
     view_name: str
-    iql_query: str
     textual_response: Optional[str] = None
```

### Comparing `dbally-0.0.2/src/dbally/data_models/llm_options.py` & `dbally-0.1.0/src/dbally/data_models/llm_options.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.2/src/dbally/data_models/prompts/__init__.py` & `dbally-0.1.0/src/dbally/data_models/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.2/src/dbally/data_models/prompts/common_validation_utils.py` & `dbally-0.1.0/src/dbally/data_models/prompts/common_validation_utils.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.2/src/dbally/data_models/prompts/iql_explainer_prompt_template.py` & `dbally-0.1.0/src/dbally/data_models/prompts/query_explainer_prompt_template.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,49 @@
 from typing import Callable, Dict, Optional
 
 from dbally.data_models.prompts.common_validation_utils import _check_prompt_variables
 from dbally.data_models.prompts.prompt_template import ChatFormat, PromptTemplate
 
 
-class IQLExplainerPromptTemplate(PromptTemplate):
+class QueryExplainerPromptTemplate(PromptTemplate):
     """
-    Class for prompt templates meant for the IQL explanation.
+    Class for prompt templates meant to generate explanations for queries
+    (when the data cannot be shown due to token limit).
+
+        Args:
+            chat: chat format
+            response_format: response format
+            llm_response_parser: function to parse llm response
     """
 
     def __init__(
         self,
         chat: ChatFormat,
         response_format: Optional[Dict[str, str]] = None,
         llm_response_parser: Callable = lambda x: x,
     ) -> None:
-        """
-        Initializes IQLExplainerPromptTemplate class.
-
-        Args:
-            chat: chat format
-            response_format: response format
-            llm_response_parser: function to parse llm response
-        """
-
         super().__init__(chat, response_format, llm_response_parser)
-        self.chat = _check_prompt_variables(chat, {"question", "filters"})
+        self.chat = _check_prompt_variables(chat, {"question", "query", "number_of_results"})
 
 
-default_iql_explainer_template = IQLExplainerPromptTemplate(
+default_query_explainer_template = QueryExplainerPromptTemplate(
     chat=(
         {
             "role": "system",
-            "content": "You are a helpful assistant that helps describe a table generated by a query composed "
-            "of a list of filters that answers users' question. "
+            "content": "You are a helpful assistant that helps describe a table generated by a query "
+            "that answers users' question. "
             "You are very intelligent and obedient.\n"
             "Your task is to provide natural language description of the table used by the logical query "
             "to the database.\n"
             "Describe the table in a way that is short and informative.\n"
-            "Make your answer as short as possible and start it by infroming the user that the table is too long "
-            "to be used in LLM call due to token limit.\n"
+            "Make your answer as short as possible, start it by infroming the user that the underlying "
+            "data is too long to print and then describe the table based on the question and the query.\n"
             "DON'T MENTION using a query in your answer.\n",
         },
         {
             "role": "user",
-            "content": "The list of filters below represents the answer to a question: {question}.\n"
-            "Describe the table generated using this filters: {filters}.",
+            "content": "The query below represents the answer to a question: {question}.\n"
+            "Describe the table generated using this query: {query}.\n"
+            "Number of results to this query: {number_of_results}.\n",
         },
     )
 )
```

### Comparing `dbally-0.0.2/src/dbally/data_models/prompts/iql_prompt_template.py` & `dbally-0.1.0/src/dbally/data_models/prompts/iql_prompt_template.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.2/src/dbally/data_models/prompts/nl_responder_prompt_template.py` & `dbally-0.1.0/src/dbally/data_models/prompts/nl_responder_prompt_template.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.2/src/dbally/data_models/prompts/prompt_template.py` & `dbally-0.1.0/src/dbally/data_models/prompts/prompt_template.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.2/src/dbally/data_models/prompts/view_selector_prompt_template.py` & `dbally-0.1.0/src/dbally/data_models/prompts/view_selector_prompt_template.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.2/src/dbally/embedding_client/base.py` & `dbally-0.1.0/src/dbally/embedding_client/base.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.2/src/dbally/embedding_client/openai.py` & `dbally-0.1.0/src/dbally/embedding_client/openai.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.2/src/dbally/iql/_exceptions.py` & `dbally-0.1.0/src/dbally/iql/_exceptions.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.2/src/dbally/iql/_processor.py` & `dbally-0.1.0/src/dbally/iql/_processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     IQLError,
     IQLFunctionNotExists,
     IQLUnsupportedSyntaxError,
 )
 from dbally.iql._type_validators import validate_arg_type
 
 if TYPE_CHECKING:
-    from dbally.views.base import ExposedFunction
+    from dbally.views.structured import ExposedFunction
 
 
 class IQLProcessor:
     """
     Parses IQL string to tree structure.
     """
```

### Comparing `dbally-0.0.2/src/dbally/iql/_query.py` & `dbally-0.1.0/src/dbally/iql/_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import TYPE_CHECKING, List
 
 from . import syntax
 from ._processor import IQLProcessor
 
 if TYPE_CHECKING:
-    from dbally.views.base import ExposedFunction
+    from dbally.views.structured import ExposedFunction
 
 
 class IQLQuery:
     """
     IQLQuery container. It stores IQL as a syntax tree defined in `IQL` class.
     """
```

### Comparing `dbally-0.0.2/src/dbally/iql/_type_validators.py` & `dbally-0.1.0/src/dbally/iql/_type_validators.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.2/src/dbally/iql/syntax.py` & `dbally-0.1.0/src/dbally/iql/syntax.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.2/src/dbally/iql_generator/iql_generator.py` & `dbally-0.1.0/src/dbally/iql_generator/iql_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import copy
 from typing import Callable, List, Optional, Tuple, TypeVar
 
 from dbally.audit.event_tracker import EventTracker
 from dbally.data_models.prompts.iql_prompt_template import IQLPromptTemplate, default_iql_template
 from dbally.llm_client.base import LLMClient
 from dbally.prompts.prompt_builder import PromptBuilder
-from dbally.views.base import ExposedFunction
+from dbally.views.exposed_functions import ExposedFunction
 
 
 class IQLGenerator:
     """
     Class used to generate IQL from natural language question.
 
     In db-ally, LLM uses IQL (Intermediate Query Language) to express complex queries in a simplified way.
```

### Comparing `dbally-0.0.2/src/dbally/llm_client/base.py` & `dbally-0.1.0/src/dbally/llm_client/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,16 +24,16 @@
         self.model_name = model_name
         self._prompt_builder = PromptBuilder(self.model_name)
 
     async def text_generation(  # pylint: disable=R0913
         self,
         template: PromptTemplate,
         fmt: dict,
-        event_tracker: EventTracker,
         *,
+        event_tracker: Optional[EventTracker] = None,
         frequency_penalty: Optional[float] = 0.0,
         max_tokens: Optional[int] = 128,
         n: Optional[int] = 1,
         presence_penalty: Optional[float] = 0.0,
         seed: Optional[int] = None,
         stop: Optional[Union[str, List[str]]] = None,
         temperature: Optional[float] = 1.0,
@@ -58,14 +58,15 @@
             top_p=top_p,
         )
 
         prompt = self._prompt_builder.build(template, fmt)
 
         event = LLMEvent(prompt=prompt, type=type(template).__name__)
 
+        event_tracker = event_tracker or EventTracker()
         async with event_tracker.track_event(event) as span:
             event.response = await self.call(prompt, template.response_format, options, event)
             span(event)
 
         return event.response
 
     @abc.abstractmethod
```

### Comparing `dbally-0.0.2/src/dbally/llm_client/openai_client.py` & `dbally-0.1.0/src/dbally/llm_client/openai_client.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.2/src/dbally/nl_responder/nl_responder.py` & `dbally-0.1.0/src/dbally/nl_responder/nl_responder.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,65 +1,65 @@
 import copy
 from typing import Dict, List, Optional
 
 import pandas as pd
 
 from dbally.audit.event_tracker import EventTracker
 from dbally.data_models.execution_result import ViewExecutionResult
-from dbally.data_models.prompts.iql_explainer_prompt_template import (
-    IQLExplainerPromptTemplate,
-    default_iql_explainer_template,
-)
 from dbally.data_models.prompts.nl_responder_prompt_template import (
     NLResponderPromptTemplate,
     default_nl_responder_template,
 )
+from dbally.data_models.prompts.query_explainer_prompt_template import (
+    QueryExplainerPromptTemplate,
+    default_query_explainer_template,
+)
 from dbally.llm_client.base import LLMClient
 from dbally.nl_responder.token_counters import count_tokens_for_huggingface, count_tokens_for_openai
 
 
 class NLResponder:
     """Class used to generate natural language response from the database output."""
 
+    # Keys used to extract the query from the context (ordered by priority)
+    QUERY_KEYS = ["iql", "sql", "query"]
+
     def __init__(
         self,
         llm_client: LLMClient,
-        iql_explainer_prompt_template: Optional[IQLExplainerPromptTemplate] = None,
+        query_explainer_prompt_template: Optional[QueryExplainerPromptTemplate] = None,
         nl_responder_prompt_template: Optional[NLResponderPromptTemplate] = None,
         max_tokens_count: int = 4096,
     ) -> None:
         """
         Args:
             llm_client: LLM client used to generate natural language response
-            iql_explainer_prompt_template: template for the prompt used to generate the iql explanation\
-            if not set defaults to `default_iql_explainer_template`
+            query_explainer_prompt_template: template for the prompt used to generate the iql explanation\
+            if not set defaults to `default_query_explainer_template`
             nl_responder_prompt_template: template for the prompt used to generate the NL response\
             if not set defaults to `nl_responder_prompt_template`
             max_tokens_count: maximum number of tokens that can be used in the prompt
         """
 
         self._llm_client = llm_client
         self._nl_responder_prompt_template = nl_responder_prompt_template or copy.deepcopy(
             default_nl_responder_template
         )
-        self._iql_explainer_prompt_template = iql_explainer_prompt_template or copy.deepcopy(
-            default_iql_explainer_template
+        self._query_explainer_prompt_template = query_explainer_prompt_template or copy.deepcopy(
+            default_query_explainer_template
         )
         self._max_tokens_count = max_tokens_count
 
-    async def generate_response(
-        self, result: ViewExecutionResult, question: str, filters: str, event_tracker: EventTracker
-    ) -> str:
+    async def generate_response(self, result: ViewExecutionResult, question: str, event_tracker: EventTracker) -> str:
         """
         Uses LLM to generate a response in natural language form.
 
         Args:
             result: object representing the result of the query execution
             question: user question
-            filters: filters used in the query
             event_tracker: event store used to audit the generation process
 
         Returns:
             Natural language response to the user question.
         """
 
         rows = _promptify_rows(result.results)
@@ -75,17 +75,19 @@
             tokens_count = count_tokens_for_huggingface(
                 messages=self._nl_responder_prompt_template.chat,
                 fmt={"rows": rows, "question": question},
                 model=self._llm_client.model_name,
             )
 
         if tokens_count > self._max_tokens_count:
+            context = result.context
+            query = next((context.get(key) for key in self.QUERY_KEYS if context.get(key)), question)
             llm_response = await self._llm_client.text_generation(
-                template=self._iql_explainer_prompt_template,
-                fmt={"question": question, "filters": filters},
+                template=self._query_explainer_prompt_template,
+                fmt={"question": question, "query": query, "number_of_results": len(result.results)},
                 event_tracker=event_tracker,
             )
 
             return llm_response
 
         llm_response = await self._llm_client.text_generation(
             template=self._nl_responder_prompt_template,
```

### Comparing `dbally-0.0.2/src/dbally/nl_responder/token_counters.py` & `dbally-0.1.0/src/dbally/nl_responder/token_counters.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.2/src/dbally/prompts/prompt_builder.py` & `dbally-0.1.0/src/dbally/prompts/prompt_builder.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.2/src/dbally/similarity/detector.py` & `dbally-0.1.0/src/dbally/similarity/detector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import importlib
 from types import ModuleType
 from typing import Any, Dict, List, Optional, Type
 
 from dbally.similarity import AbstractSimilarityIndex
 from dbally.views import decorators
-from dbally.views.base import ExposedFunction, MethodParamWithTyping
+from dbally.views.exposed_functions import ExposedFunction, MethodParamWithTyping
 from dbally.views.methods_base import MethodsBaseView
 
 
 class SimilarityIndexDetectorException(Exception):
     """
     Exception that occured during similarity index discovery
     """
```

### Comparing `dbally-0.0.2/src/dbally/similarity/faiss_store.py` & `dbally-0.1.0/src/dbally/similarity/faiss_store.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.2/src/dbally/similarity/index.py` & `dbally-0.1.0/src/dbally/similarity/index.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.2/src/dbally/similarity/sqlalchemy_base.py` & `dbally-0.1.0/src/dbally/similarity/sqlalchemy_base.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.2/src/dbally/similarity/store.py` & `dbally-0.1.0/src/dbally/similarity/store.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.2/src/dbally/view_selection/base.py` & `dbally-0.1.0/src/dbally/view_selection/base.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.2/src/dbally/view_selection/llm_view_selector.py` & `dbally-0.1.0/src/dbally/view_selection/llm_view_selector.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.2/src/dbally/view_selection/random_view_selector.py` & `dbally-0.1.0/src/dbally/view_selection/random_view_selector.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.2/src/dbally/views/methods_base.py` & `dbally-0.1.0/src/dbally/views/methods_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import abc
 import inspect
 import textwrap
 from typing import Any, Callable, List, Tuple
 
 from dbally.iql import syntax
 from dbally.views import decorators
-from dbally.views.base import AbstractBaseView, ExposedFunction, MethodParamWithTyping
+from dbally.views.exposed_functions import ExposedFunction, MethodParamWithTyping
+from dbally.views.structured import BaseStructuredView
 
 
-class MethodsBaseView(AbstractBaseView, metaclass=abc.ABCMeta):
+class MethodsBaseView(BaseStructuredView, metaclass=abc.ABCMeta):
     """
     Base class for views that use view methods to expose filters.
     """
 
     # Method arguments that should be skipped when listing methods
     HIDDEN_ARGUMENTS = ["self", "select", "return"]
```

### Comparing `dbally-0.0.2/src/dbally/views/pandas_base.py` & `dbally-0.1.0/src/dbally/views/pandas_base.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.2/src/dbally/views/sqlalchemy_base.py` & `dbally-0.1.0/src/dbally/views/sqlalchemy_base.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.2/src/dbally.egg-info/SOURCES.txt` & `dbally-0.1.0/src/dbally.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 src/py.typed
-src/dbally/VERSION
 src/dbally/__init__.py
 src/dbally/__version__.py
 src/dbally/_main.py
 src/dbally/collection.py
 src/dbally/py.typed
 src/dbally.egg-info/PKG-INFO
 src/dbally.egg-info/SOURCES.txt
@@ -30,18 +29,18 @@
 src/dbally/audit/event_handlers/langsmith_event_handler.py
 src/dbally/data_models/__init__.py
 src/dbally/data_models/audit.py
 src/dbally/data_models/execution_result.py
 src/dbally/data_models/llm_options.py
 src/dbally/data_models/prompts/__init__.py
 src/dbally/data_models/prompts/common_validation_utils.py
-src/dbally/data_models/prompts/iql_explainer_prompt_template.py
 src/dbally/data_models/prompts/iql_prompt_template.py
 src/dbally/data_models/prompts/nl_responder_prompt_template.py
 src/dbally/data_models/prompts/prompt_template.py
+src/dbally/data_models/prompts/query_explainer_prompt_template.py
 src/dbally/data_models/prompts/view_selector_prompt_template.py
 src/dbally/embedding_client/__init__.py
 src/dbally/embedding_client/base.py
 src/dbally/embedding_client/openai.py
 src/dbally/iql/__init__.py
 src/dbally/iql/_exceptions.py
 src/dbally/iql/_processor.py
@@ -55,14 +54,15 @@
 src/dbally/llm_client/openai_client.py
 src/dbally/nl_responder/__init__.py
 src/dbally/nl_responder/nl_responder.py
 src/dbally/nl_responder/token_counters.py
 src/dbally/prompts/__init__.py
 src/dbally/prompts/prompt_builder.py
 src/dbally/similarity/__init__.py
+src/dbally/similarity/chroma_store.py
 src/dbally/similarity/detector.py
 src/dbally/similarity/faiss_store.py
 src/dbally/similarity/fetcher.py
 src/dbally/similarity/index.py
 src/dbally/similarity/sqlalchemy_base.py
 src/dbally/similarity/store.py
 src/dbally/utils/__init__.py
@@ -70,13 +70,21 @@
 src/dbally/view_selection/__init__.py
 src/dbally/view_selection/base.py
 src/dbally/view_selection/llm_view_selector.py
 src/dbally/view_selection/random_view_selector.py
 src/dbally/views/__init__.py
 src/dbally/views/base.py
 src/dbally/views/decorators.py
+src/dbally/views/exposed_functions.py
 src/dbally/views/methods_base.py
 src/dbally/views/pandas_base.py
 src/dbally/views/sqlalchemy_base.py
+src/dbally/views/structured.py
+src/dbally/views/freeform/__init__.py
+src/dbally/views/freeform/text2sql/__init__.py
+src/dbally/views/freeform/text2sql/_autodiscovery.py
+src/dbally/views/freeform/text2sql/_config.py
+src/dbally/views/freeform/text2sql/_errors.py
+src/dbally/views/freeform/text2sql/_view.py
 src/dbally_cli/__init__.py
 src/dbally_cli/main.py
 src/dbally_cli/similarity.py
```

### Comparing `dbally-0.0.2/src/dbally_cli/similarity.py` & `dbally-0.1.0/src/dbally_cli/similarity.py`

 * *Files identical despite different names*

