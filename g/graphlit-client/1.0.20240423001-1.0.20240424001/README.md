# Comparing `tmp/graphlit_client-1.0.20240423001.tar.gz` & `tmp/graphlit_client-1.0.20240424001.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphlit_client-1.0.20240423001.tar", last modified: Wed Apr 24 05:27:37 2024, max compression
+gzip compressed data, was "graphlit_client-1.0.20240424001.tar", last modified: Thu Apr 25 00:06:37 2024, max compression
```

## Comparing `graphlit_client-1.0.20240423001.tar` & `graphlit_client-1.0.20240424001.tar`

### file list

```diff
@@ -1,98 +1,99 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 05:27:37.983565 graphlit_client-1.0.20240423001/
--rw-r--r--   0 vsts      (1001) docker     (127)     1095 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-04-24 05:27:37.983565 graphlit_client-1.0.20240423001/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2321 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 05:27:37.963565 graphlit_client-1.0.20240423001/graphlit/
--rw-r--r--   0 vsts      (1001) docker     (127)       32 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1796 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit/graphlit.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 05:27:37.983565 graphlit_client-1.0.20240423001/graphlit_api/
--rw-r--r--   0 vsts      (1001) docker     (127)    59431 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      888 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/add_contents_to_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12578 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/async_base_client.py
--rw-r--r--   0 vsts      (1001) docker     (127)      620 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/base_model.py
--rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/clear_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)    42943 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/client.py
--rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/close_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/create_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/create_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/create_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/create_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/create_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8453 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/create_workflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      984 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/credits.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/delete_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/delete_alerts.py
--rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/delete_all_alerts.py
--rw-r--r--   0 vsts      (1001) docker     (127)      507 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/delete_all_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/delete_all_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/delete_all_conversations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/delete_all_feeds.py
--rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/delete_all_workflows.py
--rw-r--r--   0 vsts      (1001) docker     (127)      452 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/delete_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      482 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/delete_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/delete_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/delete_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/delete_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      498 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/delete_conversations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/delete_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      434 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/delete_feeds.py
--rw-r--r--   0 vsts      (1001) docker     (127)      476 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/delete_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/delete_workflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/delete_workflows.py
--rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/disable_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/disable_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/enable_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/enable_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16949 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/enums.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2411 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (127)      957 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/extract_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3609 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/get_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      799 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/get_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7230 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/get_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4014 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/get_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7138 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/get_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1269 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/get_project.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4502 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/get_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7887 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/get_workflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      677 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/ingest_encoded_file.py
--rw-r--r--   0 vsts      (1001) docker     (127)      606 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/ingest_text.py
--rw-r--r--   0 vsts      (1001) docker     (127)      598 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/ingest_uri.py
--rw-r--r--   0 vsts      (1001) docker     (127)    69218 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/input_types.py
--rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/is_content_done.py
--rw-r--r--   0 vsts      (1001) docker     (127)      352 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/is_feed_done.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1050 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/lookup_credits.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1568 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/lookup_usage.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39649 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/operations.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3256 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/prompt_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2055 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/prompt_specifications.py
--rw-r--r--   0 vsts      (1001) docker     (127)      796 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/publish_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      828 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/publish_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4196 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/query_alerts.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/query_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1112 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/query_content_facets.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7934 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/query_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4623 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/query_conversations.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7942 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/query_feeds.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4953 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/query_specifications.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8865 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/query_workflows.py
--rw-r--r--   0 vsts      (1001) docker     (127)      950 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/remove_contents_from_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/suggest_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1096 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/summarize_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/update_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/update_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      644 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/update_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/update_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/update_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/update_project.py
--rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/update_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8453 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/update_workflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1482 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/usage.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 05:27:37.983565 graphlit_client-1.0.20240423001/graphlit_client.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-04-24 05:27:37.000000 graphlit_client-1.0.20240423001/graphlit_client.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2870 2024-04-24 05:27:37.000000 graphlit_client-1.0.20240423001/graphlit_client.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-24 05:27:37.000000 graphlit_client-1.0.20240423001/graphlit_client.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       46 2024-04-24 05:27:37.000000 graphlit_client-1.0.20240423001/graphlit_client.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-04-24 05:27:37.000000 graphlit_client-1.0.20240423001/graphlit_client.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      295 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-24 05:27:37.983565 graphlit_client-1.0.20240423001/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)      766 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:06:37.430676 graphlit_client-1.0.20240424001/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1095 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-04-25 00:06:37.430676 graphlit_client-1.0.20240424001/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2321 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:06:37.418676 graphlit_client-1.0.20240424001/graphlit/
+-rw-r--r--   0 vsts      (1001) docker     (127)       32 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1796 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit/graphlit.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:06:37.426676 graphlit_client-1.0.20240424001/graphlit_api/
+-rw-r--r--   0 vsts      (1001) docker     (127)    59588 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      888 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/add_contents_to_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12578 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/async_base_client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      620 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/base_model.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/clear_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    44094 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/close_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/create_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/create_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/create_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/create_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/create_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8453 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/create_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      984 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/credits.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/delete_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/delete_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/delete_all_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      507 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/delete_all_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/delete_all_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/delete_all_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/delete_all_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/delete_all_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      452 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/delete_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      482 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/delete_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/delete_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/delete_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/delete_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      498 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/delete_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/delete_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      434 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/delete_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      476 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/delete_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/delete_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/delete_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/disable_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/disable_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/enable_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/enable_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16949 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/enums.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2411 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      957 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/extract_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3609 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/get_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      799 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/get_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7230 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/get_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4014 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/get_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7138 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/get_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1269 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/get_project.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4502 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/get_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7887 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/get_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      677 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/ingest_encoded_file.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      606 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/ingest_text.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      598 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/ingest_uri.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    69307 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/input_types.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/is_content_done.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      352 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/is_feed_done.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1050 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/lookup_credits.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1568 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/lookup_usage.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    40274 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/operations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3256 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/prompt_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2055 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/prompt_specifications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      796 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/publish_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      828 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/publish_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      750 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/publish_text.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4196 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/query_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/query_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1112 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/query_content_facets.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7934 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/query_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4623 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/query_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7942 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/query_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4953 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/query_specifications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8865 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/query_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      950 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/remove_contents_from_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/suggest_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1096 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/summarize_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/update_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/update_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      644 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/update_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/update_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/update_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/update_project.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/update_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8453 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/update_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1482 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/graphlit_api/usage.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 00:06:37.430676 graphlit_client-1.0.20240424001/graphlit_client.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-04-25 00:06:37.000000 graphlit_client-1.0.20240424001/graphlit_client.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2899 2024-04-25 00:06:37.000000 graphlit_client-1.0.20240424001/graphlit_client.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-25 00:06:37.000000 graphlit_client-1.0.20240424001/graphlit_client.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       46 2024-04-25 00:06:37.000000 graphlit_client-1.0.20240424001/graphlit_client.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-04-25 00:06:37.000000 graphlit_client-1.0.20240424001/graphlit_client.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      295 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-25 00:06:37.430676 graphlit_client-1.0.20240424001/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)      766 2024-04-25 00:06:20.000000 graphlit_client-1.0.20240424001/setup.py
```

### Comparing `graphlit_client-1.0.20240423001/LICENSE` & `graphlit_client-1.0.20240424001/LICENSE`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/PKG-INFO` & `graphlit_client-1.0.20240424001/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphlit-client
-Version: 1.0.20240423001
+Version: 1.0.20240424001
 Summary: Graphlit API Python Client
 Home-page: https://github.com/graphlit/graphlit-client-python
 Author: Unstruk Data Inc.
 Author-email: questions@graphlit.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `graphlit_client-1.0.20240423001/README.md` & `graphlit_client-1.0.20240424001/README.md`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit/graphlit.py` & `graphlit_client-1.0.20240424001/graphlit/graphlit.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/__init__.py` & `graphlit_client-1.0.20240424001/graphlit_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -581,14 +581,15 @@
     IS_FEED_DONE_GQL,
     LOOKUP_CREDITS_GQL,
     LOOKUP_USAGE_GQL,
     PROMPT_CONVERSATION_GQL,
     PROMPT_SPECIFICATIONS_GQL,
     PUBLISH_CONTENTS_GQL,
     PUBLISH_CONVERSATION_GQL,
+    PUBLISH_TEXT_GQL,
     QUERY_ALERTS_GQL,
     QUERY_COLLECTIONS_GQL,
     QUERY_CONTENT_FACETS_GQL,
     QUERY_CONTENTS_GQL,
     QUERY_CONVERSATIONS_GQL,
     QUERY_FEEDS_GQL,
     QUERY_SPECIFICATIONS_GQL,
@@ -627,14 +628,15 @@
     PromptSpecificationsPromptSpecificationsSpecification,
 )
 from .publish_contents import PublishContents, PublishContentsPublishContents
 from .publish_conversation import (
     PublishConversation,
     PublishConversationPublishConversation,
 )
+from .publish_text import PublishText, PublishTextPublishText
 from .query_alerts import (
     QueryAlerts,
     QueryAlertsAlerts,
     QueryAlertsAlertsResults,
     QueryAlertsAlertsResultsFilter,
     QueryAlertsAlertsResultsFilterCollections,
     QueryAlertsAlertsResultsFilterContents,
@@ -1332,14 +1334,15 @@
     "OrganizationInput",
     "OrganizationUpdateInput",
     "OrientationTypes",
     "PROMPT_CONVERSATION_GQL",
     "PROMPT_SPECIFICATIONS_GQL",
     "PUBLISH_CONTENTS_GQL",
     "PUBLISH_CONVERSATION_GQL",
+    "PUBLISH_TEXT_GQL",
     "PersonFacetInput",
     "PersonFacetTypes",
     "PersonFilter",
     "PersonInput",
     "PersonUpdateInput",
     "PlaceFacetInput",
     "PlaceFacetTypes",
@@ -1379,14 +1382,16 @@
     "PromptStrategyInput",
     "PromptStrategyTypes",
     "PromptStrategyUpdateInput",
     "PublishContents",
     "PublishContentsPublishContents",
     "PublishConversation",
     "PublishConversationPublishConversation",
+    "PublishText",
+    "PublishTextPublishText",
     "QUERY_ALERTS_GQL",
     "QUERY_COLLECTIONS_GQL",
     "QUERY_CONTENTS_GQL",
     "QUERY_CONTENT_FACETS_GQL",
     "QUERY_CONVERSATIONS_GQL",
     "QUERY_FEEDS_GQL",
     "QUERY_SPECIFICATIONS_GQL",
```

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/add_contents_to_collections.py` & `graphlit_client-1.0.20240424001/graphlit_api/add_contents_to_collections.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/async_base_client.py` & `graphlit_client-1.0.20240424001/graphlit_api/async_base_client.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/base_model.py` & `graphlit_client-1.0.20240424001/graphlit_api/base_model.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/clear_conversation.py` & `graphlit_client-1.0.20240424001/graphlit_api/clear_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/client.py` & `graphlit_client-1.0.20240424001/graphlit_api/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,14 +132,15 @@
     IS_FEED_DONE_GQL,
     LOOKUP_CREDITS_GQL,
     LOOKUP_USAGE_GQL,
     PROMPT_CONVERSATION_GQL,
     PROMPT_SPECIFICATIONS_GQL,
     PUBLISH_CONTENTS_GQL,
     PUBLISH_CONVERSATION_GQL,
+    PUBLISH_TEXT_GQL,
     QUERY_ALERTS_GQL,
     QUERY_COLLECTIONS_GQL,
     QUERY_CONTENT_FACETS_GQL,
     QUERY_CONTENTS_GQL,
     QUERY_CONVERSATIONS_GQL,
     QUERY_FEEDS_GQL,
     QUERY_SPECIFICATIONS_GQL,
@@ -157,14 +158,15 @@
     UPDATE_WORKFLOW_GQL,
     USAGE_GQL,
 )
 from .prompt_conversation import PromptConversation
 from .prompt_specifications import PromptSpecifications
 from .publish_contents import PublishContents
 from .publish_conversation import PublishConversation
+from .publish_text import PublishText
 from .query_alerts import QueryAlerts
 from .query_collections import QueryCollections
 from .query_content_facets import QueryContentFacets
 from .query_contents import QueryContents
 from .query_conversations import QueryConversations
 from .query_feeds import QueryFeeds
 from .query_specifications import QuerySpecifications
@@ -587,14 +589,15 @@
         data = self.get_data(response)
         return IsContentDone.model_validate(data)
 
     async def publish_contents(
         self,
         publish_prompt: str,
         connector: ContentPublishingConnectorInput,
+        is_synchronous: bool,
         summary_prompt: Union[Optional[str], UnsetType] = UNSET,
         filter: Union[Optional[ContentFilter], UnsetType] = UNSET,
         correlation_id: Union[Optional[str], UnsetType] = UNSET,
         name: Union[Optional[str], UnsetType] = UNSET,
         summary_specification: Union[Optional[EntityReferenceInput], UnsetType] = UNSET,
         publish_specification: Union[Optional[EntityReferenceInput], UnsetType] = UNSET,
         workflow: Union[Optional[EntityReferenceInput], UnsetType] = UNSET,
@@ -606,24 +609,54 @@
             "connector": connector,
             "filter": filter,
             "correlationId": correlation_id,
             "name": name,
             "summarySpecification": summary_specification,
             "publishSpecification": publish_specification,
             "workflow": workflow,
+            "isSynchronous": is_synchronous,
         }
         response = await self.execute(
             query=PUBLISH_CONTENTS_GQL,
             operation_name="PublishContents",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return PublishContents.model_validate(data)
 
+    async def publish_text(
+        self,
+        text: str,
+        connector: ContentPublishingConnectorInput,
+        is_synchronous: bool,
+        text_type: Union[Optional[TextTypes], UnsetType] = UNSET,
+        correlation_id: Union[Optional[str], UnsetType] = UNSET,
+        name: Union[Optional[str], UnsetType] = UNSET,
+        workflow: Union[Optional[EntityReferenceInput], UnsetType] = UNSET,
+        **kwargs: Any
+    ) -> PublishText:
+        variables: Dict[str, object] = {
+            "text": text,
+            "textType": text_type,
+            "connector": connector,
+            "correlationId": correlation_id,
+            "name": name,
+            "workflow": workflow,
+            "isSynchronous": is_synchronous,
+        }
+        response = await self.execute(
+            query=PUBLISH_TEXT_GQL,
+            operation_name="PublishText",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return PublishText.model_validate(data)
+
     async def query_content_facets(
         self,
         filter: Union[Optional[ContentFilter], UnsetType] = UNSET,
         facets: Union[Optional[List[ContentFacetInput]], UnsetType] = UNSET,
         **kwargs: Any
     ) -> QueryContentFacets:
         variables: Dict[str, object] = {"filter": filter, "facets": facets}
```

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/close_conversation.py` & `graphlit_client-1.0.20240424001/graphlit_api/close_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/create_collection.py` & `graphlit_client-1.0.20240424001/graphlit_api/create_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/create_conversation.py` & `graphlit_client-1.0.20240424001/graphlit_api/create_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/create_specification.py` & `graphlit_client-1.0.20240424001/graphlit_api/create_specification.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/create_workflow.py` & `graphlit_client-1.0.20240424001/graphlit_api/create_workflow.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/credits.py` & `graphlit_client-1.0.20240424001/graphlit_api/credits.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/delete_all_conversations.py` & `graphlit_client-1.0.20240424001/graphlit_api/delete_all_conversations.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/enums.py` & `graphlit_client-1.0.20240424001/graphlit_api/enums.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/exceptions.py` & `graphlit_client-1.0.20240424001/graphlit_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/extract_contents.py` & `graphlit_client-1.0.20240424001/graphlit_api/extract_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/get_alert.py` & `graphlit_client-1.0.20240424001/graphlit_api/get_alert.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/get_collection.py` & `graphlit_client-1.0.20240424001/graphlit_api/get_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/get_content.py` & `graphlit_client-1.0.20240424001/graphlit_api/get_content.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/get_conversation.py` & `graphlit_client-1.0.20240424001/graphlit_api/get_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/get_feed.py` & `graphlit_client-1.0.20240424001/graphlit_api/get_feed.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/get_project.py` & `graphlit_client-1.0.20240424001/graphlit_api/get_project.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/get_specification.py` & `graphlit_client-1.0.20240424001/graphlit_api/get_specification.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/get_workflow.py` & `graphlit_client-1.0.20240424001/graphlit_api/get_workflow.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/ingest_encoded_file.py` & `graphlit_client-1.0.20240424001/graphlit_api/ingest_encoded_file.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/ingest_text.py` & `graphlit_client-1.0.20240424001/graphlit_api/ingest_text.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/ingest_uri.py` & `graphlit_client-1.0.20240424001/graphlit_api/ingest_uri.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/input_types.py` & `graphlit_client-1.0.20240424001/graphlit_api/input_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1820,14 +1820,15 @@
     )
 
 
 class OpenAIImageExtractionPropertiesInput(BaseModel):
     detail_level: Optional[OpenAIVisionDetailLevels] = Field(
         alias="detailLevel", default=None
     )
+    custom_instructions: Optional[str] = Field(alias="customInstructions", default=None)
     confidence_threshold: Optional[float] = Field(
         alias="confidenceThreshold", default=None
     )
 
 
 class ModelTextExtractionPropertiesInput(BaseModel):
     specification: Optional["EntityReferenceInput"] = None
```

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/lookup_credits.py` & `graphlit_client-1.0.20240424001/graphlit_api/lookup_credits.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/lookup_usage.py` & `graphlit_client-1.0.20240424001/graphlit_api/lookup_usage.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/operations.py` & `graphlit_client-1.0.20240424001/graphlit_api/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     "IS_FEED_DONE_GQL",
     "LOOKUP_CREDITS_GQL",
     "LOOKUP_USAGE_GQL",
     "PROMPT_CONVERSATION_GQL",
     "PROMPT_SPECIFICATIONS_GQL",
     "PUBLISH_CONTENTS_GQL",
     "PUBLISH_CONVERSATION_GQL",
+    "PUBLISH_TEXT_GQL",
     "QUERY_ALERTS_GQL",
     "QUERY_COLLECTIONS_GQL",
     "QUERY_CONTENTS_GQL",
     "QUERY_CONTENT_FACETS_GQL",
     "QUERY_CONVERSATIONS_GQL",
     "QUERY_FEEDS_GQL",
     "QUERY_SPECIFICATIONS_GQL",
@@ -696,25 +697,51 @@
   isContentDone(id: $id) {
     result
   }
 }
 """
 
 PUBLISH_CONTENTS_GQL = """
-mutation PublishContents($summaryPrompt: String, $publishPrompt: String!, $connector: ContentPublishingConnectorInput!, $filter: ContentFilter, $correlationId: String, $name: String, $summarySpecification: EntityReferenceInput, $publishSpecification: EntityReferenceInput, $workflow: EntityReferenceInput) {
+mutation PublishContents($summaryPrompt: String, $publishPrompt: String!, $connector: ContentPublishingConnectorInput!, $filter: ContentFilter, $correlationId: String, $name: String, $summarySpecification: EntityReferenceInput, $publishSpecification: EntityReferenceInput, $workflow: EntityReferenceInput, $isSynchronous: Boolean!) {
   publishContents(
     summaryPrompt: $summaryPrompt
     publishPrompt: $publishPrompt
     connector: $connector
     filter: $filter
     correlationId: $correlationId
     name: $name
     summarySpecification: $summarySpecification
     publishSpecification: $publishSpecification
     workflow: $workflow
+    isSynchronous: $isSynchronous
+  ) {
+    id
+    name
+    state
+    type
+    fileType
+    mimeType
+    uri
+    textUri
+    audioUri
+    markdown
+  }
+}
+"""
+
+PUBLISH_TEXT_GQL = """
+mutation PublishText($text: String!, $textType: TextTypes, $connector: ContentPublishingConnectorInput!, $correlationId: String, $name: String, $workflow: EntityReferenceInput, $isSynchronous: Boolean!) {
+  publishText(
+    text: $text
+    textType: $textType
+    connector: $connector
+    correlationId: $correlationId
+    name: $name
+    workflow: $workflow
+    isSynchronous: $isSynchronous
   ) {
     id
     name
     state
     type
     fileType
     mimeType
```

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/prompt_conversation.py` & `graphlit_client-1.0.20240424001/graphlit_api/prompt_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/prompt_specifications.py` & `graphlit_client-1.0.20240424001/graphlit_api/prompt_specifications.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/publish_contents.py` & `graphlit_client-1.0.20240424001/graphlit_api/publish_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/publish_conversation.py` & `graphlit_client-1.0.20240424001/graphlit_api/publish_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/query_alerts.py` & `graphlit_client-1.0.20240424001/graphlit_api/query_alerts.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/query_collections.py` & `graphlit_client-1.0.20240424001/graphlit_api/query_collections.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/query_content_facets.py` & `graphlit_client-1.0.20240424001/graphlit_api/query_content_facets.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/query_contents.py` & `graphlit_client-1.0.20240424001/graphlit_api/query_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/query_conversations.py` & `graphlit_client-1.0.20240424001/graphlit_api/query_conversations.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/query_feeds.py` & `graphlit_client-1.0.20240424001/graphlit_api/query_feeds.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/query_specifications.py` & `graphlit_client-1.0.20240424001/graphlit_api/query_specifications.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/query_workflows.py` & `graphlit_client-1.0.20240424001/graphlit_api/query_workflows.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/remove_contents_from_collection.py` & `graphlit_client-1.0.20240424001/graphlit_api/remove_contents_from_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/summarize_contents.py` & `graphlit_client-1.0.20240424001/graphlit_api/summarize_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/update_collection.py` & `graphlit_client-1.0.20240424001/graphlit_api/update_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/update_content.py` & `graphlit_client-1.0.20240424001/graphlit_api/update_content.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/update_conversation.py` & `graphlit_client-1.0.20240424001/graphlit_api/update_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/update_specification.py` & `graphlit_client-1.0.20240424001/graphlit_api/update_specification.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/update_workflow.py` & `graphlit_client-1.0.20240424001/graphlit_api/update_workflow.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_api/usage.py` & `graphlit_client-1.0.20240424001/graphlit_api/usage.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240423001/graphlit_client.egg-info/PKG-INFO` & `graphlit_client-1.0.20240424001/graphlit_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphlit-client
-Version: 1.0.20240423001
+Version: 1.0.20240424001
 Summary: Graphlit API Python Client
 Home-page: https://github.com/graphlit/graphlit-client-python
 Author: Unstruk Data Inc.
 Author-email: questions@graphlit.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `graphlit_client-1.0.20240423001/graphlit_client.egg-info/SOURCES.txt` & `graphlit_client-1.0.20240424001/graphlit_client.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 graphlit_api/lookup_credits.py
 graphlit_api/lookup_usage.py
 graphlit_api/operations.py
 graphlit_api/prompt_conversation.py
 graphlit_api/prompt_specifications.py
 graphlit_api/publish_contents.py
 graphlit_api/publish_conversation.py
+graphlit_api/publish_text.py
 graphlit_api/query_alerts.py
 graphlit_api/query_collections.py
 graphlit_api/query_content_facets.py
 graphlit_api/query_contents.py
 graphlit_api/query_conversations.py
 graphlit_api/query_feeds.py
 graphlit_api/query_specifications.py
```

### Comparing `graphlit_client-1.0.20240423001/setup.py` & `graphlit_client-1.0.20240424001/setup.py`

 * *Files identical despite different names*

