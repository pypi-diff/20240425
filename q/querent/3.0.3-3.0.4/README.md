# Comparing `tmp/querent-3.0.3.tar.gz` & `tmp/querent-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "querent-3.0.3.tar", last modified: Thu Apr 18 21:26:32 2024, max compression
+gzip compressed data, was "querent-3.0.4.tar", last modified: Thu Apr 25 04:36:46 2024, max compression
```

## Comparing `querent-3.0.3.tar` & `querent-3.0.4.tar`

### file list

```diff
@@ -1,262 +1,262 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.857486 querent-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-18 21:20:47.000000 querent-3.0.3/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)    17092 2024-04-18 21:26:32.857486 querent-3.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12233 2024-04-18 21:20:47.000000 querent-3.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.797486 querent-3.0.3/querent/
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-18 21:20:47.000000 querent-3.0.3/querent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.797486 querent-3.0.3/querent/callback/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-18 21:20:47.000000 querent-3.0.3/querent/callback/event_callback_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-18 21:20:47.000000 querent-3.0.3/querent/callback/event_callback_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.797486 querent-3.0.3/querent/channel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-18 21:20:47.000000 querent-3.0.3/querent/channel/channel_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.797486 querent-3.0.3/querent/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.801486 querent-3.0.3/querent/collectors/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.801486 querent-3.0.3/querent/collectors/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/aws/aws_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.801486 querent-3.0.3/querent/collectors/azure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/azure/azure_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/collector_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/collector_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/collector_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/collector_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.801486 querent-3.0.3/querent/collectors/drive/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/drive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/drive/google_drive_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.801486 querent-3.0.3/querent/collectors/dropbox/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/dropbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/dropbox/dropbox_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.805486 querent-3.0.3/querent/collectors/email/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/email/email_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/email/imap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.805486 querent-3.0.3/querent/collectors/fs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/fs/fs_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.805486 querent-3.0.3/querent/collectors/gcs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/gcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/gcs/gcs_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.805486 querent-3.0.3/querent/collectors/github/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/github/github_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.805486 querent-3.0.3/querent/collectors/jira/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/jira/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/jira/jira_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.805486 querent-3.0.3/querent/collectors/news/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/news/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/news/news_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.805486 querent-3.0.3/querent/collectors/slack/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/slack/slack_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.809486 querent-3.0.3/querent/collectors/webscaper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/webscaper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/webscaper/web_scraper_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.809486 querent-3.0.3/querent/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-04-18 21:20:47.000000 querent-3.0.3/querent/common/common_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.809486 querent-3.0.3/querent/common/errors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/common/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-18 21:20:47.000000 querent-3.0.3/querent/common/errors/metric_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.813486 querent-3.0.3/querent/common/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/common/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-18 21:20:47.000000 querent-3.0.3/querent/common/types/collected_bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-18 21:20:47.000000 querent-3.0.3/querent/common/types/collector_config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-18 21:20:47.000000 querent-3.0.3/querent/common/types/config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-18 21:20:47.000000 querent-3.0.3/querent/common/types/engine_config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-18 21:20:47.000000 querent-3.0.3/querent/common/types/file_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-18 21:20:47.000000 querent-3.0.3/querent/common/types/ingested_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-18 21:20:47.000000 querent-3.0.3/querent/common/types/ingested_images.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-18 21:20:47.000000 querent-3.0.3/querent/common/types/ingested_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-18 21:20:47.000000 querent-3.0.3/querent/common/types/ingested_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-18 21:20:47.000000 querent-3.0.3/querent/common/types/querent_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-18 21:20:47.000000 querent-3.0.3/querent/common/types/querent_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-18 21:20:47.000000 querent-3.0.3/querent/common/types/resource_config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-18 21:20:47.000000 querent-3.0.3/querent/common/types/workflow_config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-18 21:20:47.000000 querent-3.0.3/querent/common/uri.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.817486 querent-3.0.3/querent/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.817486 querent-3.0.3/querent/config/collector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/collector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13454 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/collector/collector_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.817486 querent-3.0.3/querent/config/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/core/gpt_llm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/core/llm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/core/opensource_llm_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.817486 querent-3.0.3/querent/config/engine/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/engine/engine_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/graph_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.817486 querent-3.0.3/querent/config/ingestor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/ingestor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/ingestor/ingestor_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.817486 querent-3.0.3/querent/config/logger/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/logger/logger_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.821486 querent-3.0.3/querent/config/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/metric/prometheus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.821486 querent-3.0.3/querent/config/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/resource/resource_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.821486 querent-3.0.3/querent/config/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/workflow/workflow_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.821486 querent-3.0.3/querent/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/controllers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.821486 querent-3.0.3/querent/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-04-18 21:20:47.000000 querent-3.0.3/querent/core/base_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.825486 querent-3.0.3/querent/core/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/core/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13817 2024-04-18 21:20:47.000000 querent-3.0.3/querent/core/transformers/bert_ner_opensourcellm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10455 2024-04-18 21:20:47.000000 querent-3.0.3/querent/core/transformers/fixed_entities_set_opensourcellm.py
--rw-r--r--   0 runner    (1001) docker     (127)    16897 2024-04-18 21:20:47.000000 querent-3.0.3/querent/core/transformers/gpt_llm_bert_ner_or_fixed_entities_set_ner.py
--rw-r--r--   0 runner    (1001) docker     (127)    21490 2024-04-18 21:20:47.000000 querent-3.0.3/querent/core/transformers/gpt_llm_gpt_ner.py
--rw-r--r--   0 runner    (1001) docker     (127)    12910 2024-04-18 21:20:47.000000 querent-3.0.3/querent/core/transformers/relationship_extraction_llm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.825486 querent-3.0.3/querent/dal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/dal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.825486 querent-3.0.3/querent/gnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/gnn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.825486 querent-3.0.3/querent/graph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-18 21:20:47.000000 querent-3.0.3/querent/graph/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-04-18 21:20:47.000000 querent-3.0.3/querent/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-04-18 21:20:47.000000 querent-3.0.3/querent/graph/graph_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-18 21:20:47.000000 querent-3.0.3/querent/graph/ontology.py
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-18 21:20:47.000000 querent-3.0.3/querent/graph/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-04-18 21:20:47.000000 querent-3.0.3/querent/graph/shacl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-04-18 21:20:47.000000 querent-3.0.3/querent/graph/subject.py
--rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-04-18 21:20:47.000000 querent-3.0.3/querent/graph/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.829486 querent-3.0.3/querent/ingestors/
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.829486 querent-3.0.3/querent/ingestors/audio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/audio/audio_ingestors.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/base_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.829486 querent-3.0.3/querent/ingestors/code/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/code/code_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.829486 querent-3.0.3/querent/ingestors/csv/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/csv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/csv/csv_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.829486 querent-3.0.3/querent/ingestors/doc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/doc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/doc/doc_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.833486 querent-3.0.3/querent/ingestors/email/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8651 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/email/email_ingestor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/email/email_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.833486 querent-3.0.3/querent/ingestors/github/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/github/github_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.833486 querent-3.0.3/querent/ingestors/html/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/html/html_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.833486 querent-3.0.3/querent/ingestors/images/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/images/image_ingestor.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/ingestor_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8332 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/ingestor_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.833486 querent-3.0.3/querent/ingestors/json/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/json/json_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.833486 querent-3.0.3/querent/ingestors/pdfs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/pdfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/pdfs/pdf_ingestor_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.833486 querent-3.0.3/querent/ingestors/ppt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/ppt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/ppt/ppt_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.837486 querent-3.0.3/querent/ingestors/texts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/texts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/texts/text_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.837486 querent-3.0.3/querent/ingestors/video/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/video/video_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.837486 querent-3.0.3/querent/ingestors/xlsx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/xlsx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/xlsx/xlsx_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.837486 querent-3.0.3/querent/ingestors/xml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/xml/xml_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.837486 querent-3.0.3/querent/kg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.841486 querent-3.0.3/querent/kg/ner_helperfunctions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/ner_helperfunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/ner_helperfunctions/attn_scores.py
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/ner_helperfunctions/contextual_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/ner_helperfunctions/dependency_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/ner_helperfunctions/filter_triples.py
--rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/ner_helperfunctions/fixed_entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/ner_helperfunctions/fixed_predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)    16152 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/ner_helperfunctions/ner_llm_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/querent_kg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.845486 querent-3.0.3/querent/kg/rel_helperfunctions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/rel_helperfunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/rel_helperfunctions/contextual_predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/rel_helperfunctions/embedding_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/rel_helperfunctions/filter_semantic_triples.py
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/rel_helperfunctions/fixed_relationships.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/rel_helperfunctions/gpt_pydantic_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/rel_helperfunctions/opeai_ratelimiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/rel_helperfunctions/openai_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/rel_helperfunctions/openllm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/rel_helperfunctions/questionanswer_llama2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/rel_helperfunctions/rag_retriever.py
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/rel_helperfunctions/rel_normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/rel_helperfunctions/triple_to_json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.845486 querent-3.0.3/querent/logging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-18 21:20:47.000000 querent-3.0.3/querent/logging/custom_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-18 21:20:47.000000 querent-3.0.3/querent/logging/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-18 21:20:47.000000 querent-3.0.3/querent/logging/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-18 21:20:47.000000 querent-3.0.3/querent/logging/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.849486 querent-3.0.3/querent/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/metric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.849486 querent-3.0.3/querent/metric/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/metric/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-18 21:20:47.000000 querent-3.0.3/querent/metric/adapters/promethus_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-18 21:20:47.000000 querent-3.0.3/querent/metric/base_metric_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-18 21:20:47.000000 querent-3.0.3/querent/metric/metric_logging_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-18 21:20:47.000000 querent-3.0.3/querent/metric/metric_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.849486 querent-3.0.3/querent/processors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-18 21:20:47.000000 querent-3.0.3/querent/processors/async_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-18 21:20:47.000000 querent-3.0.3/querent/processors/text_cleanup_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-18 21:20:47.000000 querent-3.0.3/querent/processors/text_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.853486 querent-3.0.3/querent/querent/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/querent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-18 21:20:47.000000 querent-3.0.3/querent/querent/auto_scaler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-18 21:20:47.000000 querent-3.0.3/querent/querent/querent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-18 21:20:47.000000 querent-3.0.3/querent/querent/resource_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/querent/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.853486 querent-3.0.3/querent/storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-18 21:20:47.000000 querent-3.0.3/querent/storage/gcs_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-18 21:20:47.000000 querent-3.0.3/querent/storage/milvus_vectorevent_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-18 21:20:47.000000 querent-3.0.3/querent/storage/neo4j_graphevent_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-18 21:20:47.000000 querent-3.0.3/querent/storage/postgres_graphevent_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.853486 querent-3.0.3/querent/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10882 2024-04-18 21:20:47.000000 querent-3.0.3/querent/tools/web_page_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.853486 querent-3.0.3/querent/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-04-18 21:20:47.000000 querent-3.0.3/querent/utils/webpage_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.853486 querent-3.0.3/querent/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-18 21:20:47.000000 querent-3.0.3/querent/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7143 2024-04-18 21:20:47.000000 querent-3.0.3/querent/workflow/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-04-18 21:20:47.000000 querent-3.0.3/querent/workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.857486 querent-3.0.3/querent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17092 2024-04-18 21:26:32.000000 querent-3.0.3/querent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-04-18 21:26:32.000000 querent-3.0.3/querent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 21:26:32.000000 querent-3.0.3/querent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-18 21:26:32.000000 querent-3.0.3/querent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 21:26:32.000000 querent-3.0.3/querent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 21:26:32.857486 querent-3.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-04-18 21:20:47.000000 querent-3.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.280917 querent-3.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-25 04:30:56.000000 querent-3.0.4/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)    16983 2024-04-25 04:36:46.276917 querent-3.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12233 2024-04-25 04:30:56.000000 querent-3.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.204917 querent-3.0.4/querent/
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-25 04:30:56.000000 querent-3.0.4/querent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.208917 querent-3.0.4/querent/callback/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/callback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-25 04:30:56.000000 querent-3.0.4/querent/callback/event_callback_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-25 04:30:56.000000 querent-3.0.4/querent/callback/event_callback_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.208917 querent-3.0.4/querent/channel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-25 04:30:56.000000 querent-3.0.4/querent/channel/channel_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.208917 querent-3.0.4/querent/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.212917 querent-3.0.4/querent/collectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.212917 querent-3.0.4/querent/collectors/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/aws/aws_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.216917 querent-3.0.4/querent/collectors/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/azure/azure_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/collector_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/collector_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/collector_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/collector_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.216917 querent-3.0.4/querent/collectors/drive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/drive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/drive/google_drive_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.216917 querent-3.0.4/querent/collectors/dropbox/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/dropbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/dropbox/dropbox_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.216917 querent-3.0.4/querent/collectors/email/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/email/email_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/email/imap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.216917 querent-3.0.4/querent/collectors/fs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/fs/fs_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.220917 querent-3.0.4/querent/collectors/gcs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/gcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/gcs/gcs_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.220917 querent-3.0.4/querent/collectors/github/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/github/github_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.220917 querent-3.0.4/querent/collectors/jira/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/jira/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/jira/jira_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.220917 querent-3.0.4/querent/collectors/news/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/news/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/news/news_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.220917 querent-3.0.4/querent/collectors/slack/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/slack/slack_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.224917 querent-3.0.4/querent/collectors/webscaper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/webscaper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/webscaper/web_scraper_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.224917 querent-3.0.4/querent/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-04-25 04:30:56.000000 querent-3.0.4/querent/common/common_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.224917 querent-3.0.4/querent/common/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/common/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-25 04:30:56.000000 querent-3.0.4/querent/common/errors/metric_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.228917 querent-3.0.4/querent/common/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/common/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-25 04:30:56.000000 querent-3.0.4/querent/common/types/collected_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-25 04:30:56.000000 querent-3.0.4/querent/common/types/collector_config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-25 04:30:56.000000 querent-3.0.4/querent/common/types/config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-25 04:30:56.000000 querent-3.0.4/querent/common/types/engine_config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-25 04:30:56.000000 querent-3.0.4/querent/common/types/file_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-25 04:30:56.000000 querent-3.0.4/querent/common/types/ingested_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-25 04:30:56.000000 querent-3.0.4/querent/common/types/ingested_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-25 04:30:56.000000 querent-3.0.4/querent/common/types/ingested_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-25 04:30:56.000000 querent-3.0.4/querent/common/types/ingested_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-25 04:30:56.000000 querent-3.0.4/querent/common/types/querent_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-25 04:30:56.000000 querent-3.0.4/querent/common/types/querent_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-25 04:30:56.000000 querent-3.0.4/querent/common/types/resource_config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-25 04:30:56.000000 querent-3.0.4/querent/common/types/workflow_config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-25 04:30:56.000000 querent-3.0.4/querent/common/uri.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.232917 querent-3.0.4/querent/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.232917 querent-3.0.4/querent/config/collector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/collector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13454 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/collector/collector_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.232917 querent-3.0.4/querent/config/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/core/gpt_llm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/core/llm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/core/opensource_llm_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.236917 querent-3.0.4/querent/config/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/engine/engine_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/graph_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.236917 querent-3.0.4/querent/config/ingestor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/ingestor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/ingestor/ingestor_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.236917 querent-3.0.4/querent/config/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/logger/logger_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.236917 querent-3.0.4/querent/config/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/metric/prometheus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.236917 querent-3.0.4/querent/config/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/resource/resource_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.236917 querent-3.0.4/querent/config/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/workflow/workflow_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.240917 querent-3.0.4/querent/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/controllers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.240917 querent-3.0.4/querent/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-04-25 04:30:56.000000 querent-3.0.4/querent/core/base_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.240917 querent-3.0.4/querent/core/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/core/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13817 2024-04-25 04:30:56.000000 querent-3.0.4/querent/core/transformers/bert_ner_opensourcellm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10455 2024-04-25 04:30:56.000000 querent-3.0.4/querent/core/transformers/fixed_entities_set_opensourcellm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16897 2024-04-25 04:30:56.000000 querent-3.0.4/querent/core/transformers/gpt_llm_bert_ner_or_fixed_entities_set_ner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21490 2024-04-25 04:30:56.000000 querent-3.0.4/querent/core/transformers/gpt_llm_gpt_ner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12910 2024-04-25 04:30:56.000000 querent-3.0.4/querent/core/transformers/relationship_extraction_llm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.244917 querent-3.0.4/querent/dal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/dal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.244917 querent-3.0.4/querent/gnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/gnn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.248917 querent-3.0.4/querent/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-25 04:30:56.000000 querent-3.0.4/querent/graph/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-04-25 04:30:56.000000 querent-3.0.4/querent/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-04-25 04:30:56.000000 querent-3.0.4/querent/graph/graph_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-25 04:30:56.000000 querent-3.0.4/querent/graph/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-25 04:30:56.000000 querent-3.0.4/querent/graph/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-04-25 04:30:56.000000 querent-3.0.4/querent/graph/shacl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-04-25 04:30:56.000000 querent-3.0.4/querent/graph/subject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-04-25 04:30:56.000000 querent-3.0.4/querent/graph/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.248917 querent-3.0.4/querent/ingestors/
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.248917 querent-3.0.4/querent/ingestors/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/audio/audio_ingestors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/base_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.248917 querent-3.0.4/querent/ingestors/code/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/code/code_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.248917 querent-3.0.4/querent/ingestors/csv/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/csv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/csv/csv_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.252917 querent-3.0.4/querent/ingestors/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/doc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/doc/doc_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.252917 querent-3.0.4/querent/ingestors/email/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8651 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/email/email_ingestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/email/email_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.252917 querent-3.0.4/querent/ingestors/github/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/github/github_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.252917 querent-3.0.4/querent/ingestors/html/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/html/html_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.252917 querent-3.0.4/querent/ingestors/images/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/images/image_ingestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/ingestor_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8332 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/ingestor_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.256917 querent-3.0.4/querent/ingestors/json/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/json/json_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.256917 querent-3.0.4/querent/ingestors/pdfs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/pdfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/pdfs/pdf_ingestor_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.256917 querent-3.0.4/querent/ingestors/ppt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/ppt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/ppt/ppt_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.256917 querent-3.0.4/querent/ingestors/texts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/texts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/texts/text_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.256917 querent-3.0.4/querent/ingestors/video/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/video/video_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.256917 querent-3.0.4/querent/ingestors/xlsx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/xlsx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/xlsx/xlsx_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.256917 querent-3.0.4/querent/ingestors/xml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/xml/xml_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.260917 querent-3.0.4/querent/kg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.260917 querent-3.0.4/querent/kg/ner_helperfunctions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/ner_helperfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/ner_helperfunctions/attn_scores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/ner_helperfunctions/contextual_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/ner_helperfunctions/dependency_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/ner_helperfunctions/filter_triples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/ner_helperfunctions/fixed_entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/ner_helperfunctions/fixed_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16152 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/ner_helperfunctions/ner_llm_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/querent_kg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.268917 querent-3.0.4/querent/kg/rel_helperfunctions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/rel_helperfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/rel_helperfunctions/contextual_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/rel_helperfunctions/embedding_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/rel_helperfunctions/filter_semantic_triples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/rel_helperfunctions/fixed_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/rel_helperfunctions/gpt_pydantic_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/rel_helperfunctions/opeai_ratelimiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/rel_helperfunctions/openai_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/rel_helperfunctions/openllm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/rel_helperfunctions/questionanswer_llama2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/rel_helperfunctions/rag_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/rel_helperfunctions/rel_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/rel_helperfunctions/triple_to_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.268917 querent-3.0.4/querent/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-25 04:30:56.000000 querent-3.0.4/querent/logging/custom_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-25 04:30:56.000000 querent-3.0.4/querent/logging/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-25 04:30:56.000000 querent-3.0.4/querent/logging/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-25 04:30:56.000000 querent-3.0.4/querent/logging/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.268917 querent-3.0.4/querent/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/metric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.272917 querent-3.0.4/querent/metric/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/metric/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-25 04:30:56.000000 querent-3.0.4/querent/metric/adapters/promethus_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-25 04:30:56.000000 querent-3.0.4/querent/metric/base_metric_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-25 04:30:56.000000 querent-3.0.4/querent/metric/metric_logging_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-25 04:30:56.000000 querent-3.0.4/querent/metric/metric_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.272917 querent-3.0.4/querent/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-25 04:30:56.000000 querent-3.0.4/querent/processors/async_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-25 04:30:56.000000 querent-3.0.4/querent/processors/text_cleanup_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-25 04:30:56.000000 querent-3.0.4/querent/processors/text_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.272917 querent-3.0.4/querent/querent/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/querent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-25 04:30:56.000000 querent-3.0.4/querent/querent/auto_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-25 04:30:56.000000 querent-3.0.4/querent/querent/querent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-25 04:30:56.000000 querent-3.0.4/querent/querent/resource_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/querent/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.276917 querent-3.0.4/querent/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-25 04:30:56.000000 querent-3.0.4/querent/storage/gcs_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-25 04:30:56.000000 querent-3.0.4/querent/storage/milvus_vectorevent_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-25 04:30:56.000000 querent-3.0.4/querent/storage/neo4j_graphevent_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-25 04:30:56.000000 querent-3.0.4/querent/storage/postgres_graphevent_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.276917 querent-3.0.4/querent/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10882 2024-04-25 04:30:56.000000 querent-3.0.4/querent/tools/web_page_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.276917 querent-3.0.4/querent/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-04-25 04:30:56.000000 querent-3.0.4/querent/utils/webpage_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.276917 querent-3.0.4/querent/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 04:30:56.000000 querent-3.0.4/querent/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7143 2024-04-25 04:30:56.000000 querent-3.0.4/querent/workflow/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-04-25 04:30:56.000000 querent-3.0.4/querent/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.276917 querent-3.0.4/querent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16983 2024-04-25 04:36:46.000000 querent-3.0.4/querent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-04-25 04:36:46.000000 querent-3.0.4/querent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 04:36:46.000000 querent-3.0.4/querent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-25 04:36:46.000000 querent-3.0.4/querent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 04:36:46.000000 querent-3.0.4/querent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 04:36:46.280917 querent-3.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-04-25 04:30:56.000000 querent-3.0.4/setup.py
```

### Comparing `querent-3.0.3/LICENCE` & `querent-3.0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/PKG-INFO` & `querent-3.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: querent
-Version: 3.0.3
+Version: 3.0.4
 Summary: The Asynchronous Data Dynamo and Graph Neural Network Catalyst
 Home-page: https://github.com/Querent-ai/querent-ai
 Author: Querent AI
 License: Business Source License 1.1
 Project-URL: Documentation, https://github.com/Querent-ai/querent-ai/docs
 Project-URL: Issue Tracker, https://github.com/Querent-ai/querent-ai/issues
 Keywords: Graph Neural Network,Scalability,Data-Driven Insights,GNN,Async,Knowledge Graphs,KG,Large Language Models,asyncio,Insights,aysnchronous,LLM,transformers,pytorch,Llama-index,AI,Artificial Intelligence,Neo4j,Queues,QuiAssisstant,Collectors,Data,Data Science,Data Engineering,Data Analysis,Data Analytics,News,NLP,Natural Language Processing,Text,Text Analysis,Deep Learning,Graphs,Graph Theory,Graph Algorithms,Graph Analytics,Graph Databases,Graph Processing,Graph Mining,Graph Neural Networks,GNN,GNNs,Graph Neural Network
@@ -35,85 +35,81 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Typing :: Typed
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 License-File: LICENCE
-Requires-Dist: cachetools==5.3.3
+Requires-Dist: aiofiles==23.2.1
 Requires-Dist: aiohttp==3.9.3
 Requires-Dist: attrs==23.1.0
+Requires-Dist: azure-storage-blob==12.19.0
 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: boto3==1.26.146
 Requires-Dist: botocore==1.29.146
 Requires-Dist: bs4==0.0.1
+Requires-Dist: cachetools==5.3.3
+Requires-Dist: coverage==7.3.3
+Requires-Dist: dropbox==11.36.2
 Requires-Dist: faiss-cpu==1.7.4
+Requires-Dist: ffmpeg-python==0.2.0
 Requires-Dist: gensim==4.3.2
+Requires-Dist: google-api-python-client==2.105.0
+Requires-Dist: google-cloud-storage==2.14.0
+Requires-Dist: google-cloud-storage==2.14.0
+Requires-Dist: google-cloud-storage==2.14.0
 Requires-Dist: hdbscan==0.8.33
 Requires-Dist: jira==3.6.0
 Requires-Dist: jmespath==1.0.1
 Requires-Dist: joblib==1.2.0
 Requires-Dist: json5==0.9.24
 Requires-Dist: jsonmerge==1.9.0
 Requires-Dist: jsonschema==4.17.3
 Requires-Dist: kombu==5.2.4
+Requires-Dist: langchain==0.1.11
+Requires-Dist: langchain-community==0.0.25
 Requires-Dist: llama_cpp_python==0.2.15
 Requires-Dist: lxml==4.9.2
+Requires-Dist: moviepy==1.0.3
 Requires-Dist: newspaper3k==0.2.8
+Requires-Dist: newsapi-python==0.2.7
 Requires-Dist: nltk==3.8.1
 Requires-Dist: numpy==1.24.3
-Requires-Dist: Pillow==10.3.0
+Requires-Dist: openai==1.13.3
+Requires-Dist: openpyxl==3.1.2
+Requires-Dist: pandas==2.1.4
+Requires-Dist: pdfminer==20191125
+Requires-Dist: pillow==10.3.0
+Requires-Dist: prometheus-client==0.17.1
+Requires-Dist: psutil==5.9.8
+Requires-Dist: pybase64==1.3.1
 Requires-Dist: pydantic==2.6.4
-Requires-Dist: PyJWT==2.4.0
-Requires-Dist: pytest==7.3.2
-Requires-Dist: python-dotenv==1.0.0
-Requires-Dist: redis==5.0.3
-Requires-Dist: regex==2023.5.5
-Requires-Dist: sentence-transformers==2.2.2
-Requires-Dist: spacy==3.7.2
-Requires-Dist: uvicorn==0.29.0
-Requires-Dist: slack-sdk==3.26.1
+Requires-Dist: pydub==0.25.1
+Requires-Dist: pyjwt==2.4.0
 Requires-Dist: pylint==2.17.4
-Requires-Dist: pytest-cov==4.1.0
-Requires-Dist: pytest-mock==3.11.1
-Requires-Dist: tensorflow==2.14.0
-Requires-Dist: transformers==4.36.0
-Requires-Dist: asyncio==3.4.3
-Requires-Dist: aiofiles==23.2.1
-Requires-Dist: prometheus-client==0.17.1
-Requires-Dist: rdflib==7.0.0
-Requires-Dist: pytest-asyncio==0.23.2
+Requires-Dist: pymupdf==1.24.0
 Requires-Dist: pyshacl==0.25.0
-Requires-Dist: google-cloud-storage==2.14.0
-Requires-Dist: PyMuPDF==1.24.0
-Requires-Dist: pydub==0.25.1
-Requires-Dist: SpeechRecognition==3.10.1
 Requires-Dist: pytesseract==0.3.10
 Requires-Dist: pytextract==2.0.1
-Requires-Dist: pandas==2.1.4
-Requires-Dist: python-pptx==0.6.23
-Requires-Dist: tika==2.6.0
-Requires-Dist: openpyxl==3.1.2
-Requires-Dist: coverage==7.3.3
-Requires-Dist: azure-storage-blob==12.19.0
-Requires-Dist: moviepy==1.0.3
+Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: python-docx==1.1.0
-Requires-Dist: dropbox==11.36.2
+Requires-Dist: python-pptx==0.6.23
+Requires-Dist: rdflib==7.0.0
+Requires-Dist: redis==5.0.3
+Requires-Dist: regex==2023.5.5
 Requires-Dist: requests==2.31.0
-Requires-Dist: google-api-python-client==2.105.0
 Requires-Dist: requests_html==0.10.0
-Requires-Dist: pybase64==1.3.1
-Requires-Dist: pdfminer==20191125
+Requires-Dist: slack-sdk==3.26.1
+Requires-Dist: slack-sdk==3.26.1
+Requires-Dist: spacy==3.7.2
+Requires-Dist: speechrecognition==3.10.1
+Requires-Dist: tika==2.6.0
+Requires-Dist: transformers==4.36.0
 Requires-Dist: unidecode==1.3.7
-Requires-Dist: psutil==5.9.8
-Requires-Dist: langchain-community==0.0.25
-Requires-Dist: langchain==0.1.11
-Requires-Dist: openai==1.13.3
-Requires-Dist: newsapi-python==0.2.7
-Requires-Dist: ffmpeg-python==0.2.0
+Requires-Dist: sentence-transformers==2.2.2
 
 # Querent
 
 The Asynchronous Data Dynamo and Graph Neural Network Catalyst
 
 ![image](https://github.com/Querent-ai/querent-ai/assets/61435908/39124a0c-3d9e-434f-9b54-9aa51dcefbd7)
```

### Comparing `querent-3.0.3/README.md` & `querent-3.0.4/README.md`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/__init__.py` & `querent-3.0.4/querent/__init__.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/callback/event_callback_dispatcher.py` & `querent-3.0.4/querent/callback/event_callback_dispatcher.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/callback/event_callback_interface.py` & `querent-3.0.4/querent/callback/event_callback_interface.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/channel/channel_interface.py` & `querent-3.0.4/querent/channel/channel_interface.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/collectors/aws/aws_collector.py` & `querent-3.0.4/querent/collectors/aws/aws_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/collectors/azure/azure_collector.py` & `querent-3.0.4/querent/collectors/azure/azure_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/collectors/collector_errors.py` & `querent-3.0.4/querent/collectors/collector_errors.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/collectors/collector_factory.py` & `querent-3.0.4/querent/collectors/collector_factory.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/collectors/collector_resolver.py` & `querent-3.0.4/querent/collectors/collector_resolver.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/collectors/drive/google_drive_collector.py` & `querent-3.0.4/querent/collectors/drive/google_drive_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/collectors/dropbox/dropbox_collector.py` & `querent-3.0.4/querent/collectors/dropbox/dropbox_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/collectors/email/email_collector.py` & `querent-3.0.4/querent/collectors/email/email_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/collectors/email/imap.py` & `querent-3.0.4/querent/collectors/email/imap.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/collectors/fs/fs_collector.py` & `querent-3.0.4/querent/collectors/fs/fs_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/collectors/gcs/gcs_collector.py` & `querent-3.0.4/querent/collectors/gcs/gcs_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/collectors/github/github_collector.py` & `querent-3.0.4/querent/collectors/github/github_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/collectors/jira/jira_collector.py` & `querent-3.0.4/querent/collectors/jira/jira_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/collectors/news/news_collector.py` & `querent-3.0.4/querent/collectors/news/news_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/collectors/slack/slack_collector.py` & `querent-3.0.4/querent/collectors/slack/slack_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/collectors/webscaper/web_scraper_collector.py` & `querent-3.0.4/querent/collectors/webscaper/web_scraper_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/common/common_errors.py` & `querent-3.0.4/querent/common/common_errors.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/common/errors/metric_errors.py` & `querent-3.0.4/querent/common/errors/metric_errors.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/common/types/collected_bytes.py` & `querent-3.0.4/querent/common/types/collected_bytes.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/common/types/file_buffer.py` & `querent-3.0.4/querent/common/types/file_buffer.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/common/types/ingested_code.py` & `querent-3.0.4/querent/common/types/ingested_code.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/common/types/ingested_images.py` & `querent-3.0.4/querent/common/types/ingested_images.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/common/types/ingested_messages.py` & `querent-3.0.4/querent/common/types/ingested_messages.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/common/types/ingested_tokens.py` & `querent-3.0.4/querent/common/types/ingested_tokens.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/common/types/querent_queue.py` & `querent-3.0.4/querent/common/types/querent_queue.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/common/uri.py` & `querent-3.0.4/querent/common/uri.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/config/collector/collector_config.py` & `querent-3.0.4/querent/config/collector/collector_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/config/config.py` & `querent-3.0.4/querent/config/config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/config/core/gpt_llm_config.py` & `querent-3.0.4/querent/config/core/gpt_llm_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/config/core/llm_config.py` & `querent-3.0.4/querent/config/core/llm_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/config/core/opensource_llm_config.py` & `querent-3.0.4/querent/config/core/opensource_llm_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/config/engine/engine_config.py` & `querent-3.0.4/querent/config/engine/engine_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/config/graph_config.py` & `querent-3.0.4/querent/config/graph_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/config/ingestor/ingestor_config.py` & `querent-3.0.4/querent/config/ingestor/ingestor_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/config/metric/prometheus.py` & `querent-3.0.4/querent/config/metric/prometheus.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/config/resource/resource_config.py` & `querent-3.0.4/querent/config/resource/resource_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/config/workflow/workflow_config.py` & `querent-3.0.4/querent/config/workflow/workflow_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/core/base_engine.py` & `querent-3.0.4/querent/core/base_engine.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/core/transformers/bert_ner_opensourcellm.py` & `querent-3.0.4/querent/core/transformers/bert_ner_opensourcellm.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/core/transformers/fixed_entities_set_opensourcellm.py` & `querent-3.0.4/querent/core/transformers/fixed_entities_set_opensourcellm.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/core/transformers/gpt_llm_bert_ner_or_fixed_entities_set_ner.py` & `querent-3.0.4/querent/core/transformers/gpt_llm_bert_ner_or_fixed_entities_set_ner.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/core/transformers/gpt_llm_gpt_ner.py` & `querent-3.0.4/querent/core/transformers/gpt_llm_gpt_ner.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/core/transformers/relationship_extraction_llm.py` & `querent-3.0.4/querent/core/transformers/relationship_extraction_llm.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/graph/errors.py` & `querent-3.0.4/querent/graph/errors.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/graph/graph.py` & `querent-3.0.4/querent/graph/graph.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/graph/graph_namespace.py` & `querent-3.0.4/querent/graph/graph_namespace.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/graph/ontology.py` & `querent-3.0.4/querent/graph/ontology.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/graph/schema.py` & `querent-3.0.4/querent/graph/schema.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/graph/shacl.py` & `querent-3.0.4/querent/graph/shacl.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/graph/subject.py` & `querent-3.0.4/querent/graph/subject.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/graph/utils.py` & `querent-3.0.4/querent/graph/utils.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/ingestors/audio/audio_ingestors.py` & `querent-3.0.4/querent/ingestors/audio/audio_ingestors.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/ingestors/base_ingestor.py` & `querent-3.0.4/querent/ingestors/base_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/ingestors/code/code_ingestor.py` & `querent-3.0.4/querent/ingestors/code/code_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/ingestors/csv/csv_ingestor.py` & `querent-3.0.4/querent/ingestors/csv/csv_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/ingestors/doc/doc_ingestor.py` & `querent-3.0.4/querent/ingestors/doc/doc_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/ingestors/email/email_ingestor.py` & `querent-3.0.4/querent/ingestors/email/email_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/ingestors/email/email_reader.py` & `querent-3.0.4/querent/ingestors/email/email_reader.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/ingestors/github/github_ingestor.py` & `querent-3.0.4/querent/ingestors/github/github_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/ingestors/html/html_ingestor.py` & `querent-3.0.4/querent/ingestors/html/html_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/ingestors/images/image_ingestor.py` & `querent-3.0.4/querent/ingestors/images/image_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/ingestors/ingestor_factory.py` & `querent-3.0.4/querent/ingestors/ingestor_factory.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/ingestors/ingestor_manager.py` & `querent-3.0.4/querent/ingestors/ingestor_manager.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/ingestors/json/json_ingestor.py` & `querent-3.0.4/querent/ingestors/json/json_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/ingestors/pdfs/pdf_ingestor_v1.py` & `querent-3.0.4/querent/ingestors/pdfs/pdf_ingestor_v1.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/ingestors/ppt/ppt_ingestor.py` & `querent-3.0.4/querent/ingestors/ppt/ppt_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/ingestors/texts/text_ingestor.py` & `querent-3.0.4/querent/ingestors/texts/text_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/ingestors/video/video_ingestor.py` & `querent-3.0.4/querent/ingestors/video/video_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/ingestors/xlsx/xlsx_ingestor.py` & `querent-3.0.4/querent/ingestors/xlsx/xlsx_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/ingestors/xml/xml_ingestor.py` & `querent-3.0.4/querent/ingestors/xml/xml_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/kg/ner_helperfunctions/attn_scores.py` & `querent-3.0.4/querent/kg/ner_helperfunctions/attn_scores.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/kg/ner_helperfunctions/contextual_embeddings.py` & `querent-3.0.4/querent/kg/ner_helperfunctions/contextual_embeddings.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/kg/ner_helperfunctions/dependency_parsing.py` & `querent-3.0.4/querent/kg/ner_helperfunctions/dependency_parsing.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/kg/ner_helperfunctions/filter_triples.py` & `querent-3.0.4/querent/kg/ner_helperfunctions/filter_triples.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/kg/ner_helperfunctions/fixed_entities.py` & `querent-3.0.4/querent/kg/ner_helperfunctions/fixed_entities.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/kg/ner_helperfunctions/fixed_predicate.py` & `querent-3.0.4/querent/kg/ner_helperfunctions/fixed_predicate.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/kg/ner_helperfunctions/ner_llm_transformer.py` & `querent-3.0.4/querent/kg/ner_helperfunctions/ner_llm_transformer.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/kg/querent_kg.py` & `querent-3.0.4/querent/kg/querent_kg.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/kg/rel_helperfunctions/contextual_predicate.py` & `querent-3.0.4/querent/kg/rel_helperfunctions/contextual_predicate.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/kg/rel_helperfunctions/embedding_store.py` & `querent-3.0.4/querent/kg/rel_helperfunctions/embedding_store.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/kg/rel_helperfunctions/filter_semantic_triples.py` & `querent-3.0.4/querent/kg/rel_helperfunctions/filter_semantic_triples.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/kg/rel_helperfunctions/fixed_relationships.py` & `querent-3.0.4/querent/kg/rel_helperfunctions/fixed_relationships.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/kg/rel_helperfunctions/gpt_pydantic_classes.py` & `querent-3.0.4/querent/kg/rel_helperfunctions/gpt_pydantic_classes.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/kg/rel_helperfunctions/openai_functions.py` & `querent-3.0.4/querent/kg/rel_helperfunctions/openai_functions.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/kg/rel_helperfunctions/questionanswer_llama2.py` & `querent-3.0.4/querent/kg/rel_helperfunctions/questionanswer_llama2.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/kg/rel_helperfunctions/rag_retriever.py` & `querent-3.0.4/querent/kg/rel_helperfunctions/rag_retriever.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/kg/rel_helperfunctions/rel_normalize.py` & `querent-3.0.4/querent/kg/rel_helperfunctions/rel_normalize.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/kg/rel_helperfunctions/triple_to_json.py` & `querent-3.0.4/querent/kg/rel_helperfunctions/triple_to_json.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/logging/filters.py` & `querent-3.0.4/querent/logging/filters.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/logging/handlers.py` & `querent-3.0.4/querent/logging/handlers.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/logging/logger.py` & `querent-3.0.4/querent/logging/logger.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/metric/adapters/promethus_adapter.py` & `querent-3.0.4/querent/metric/adapters/promethus_adapter.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/metric/metric_logging_handler.py` & `querent-3.0.4/querent/metric/metric_logging_handler.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/metric/metric_registry.py` & `querent-3.0.4/querent/metric/metric_registry.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/processors/text_cleanup_processor.py` & `querent-3.0.4/querent/processors/text_cleanup_processor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/processors/text_processor.py` & `querent-3.0.4/querent/processors/text_processor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/querent/auto_scaler.py` & `querent-3.0.4/querent/querent/auto_scaler.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/querent/querent.py` & `querent-3.0.4/querent/querent/querent.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/querent/resource_manager.py` & `querent-3.0.4/querent/querent/resource_manager.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/storage/gcs_query.py` & `querent-3.0.4/querent/storage/gcs_query.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/storage/milvus_vectorevent_storage.py` & `querent-3.0.4/querent/storage/milvus_vectorevent_storage.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/storage/neo4j_graphevent_storage.py` & `querent-3.0.4/querent/storage/neo4j_graphevent_storage.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/storage/postgres_graphevent_storage.py` & `querent-3.0.4/querent/storage/postgres_graphevent_storage.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/tools/web_page_extractor.py` & `querent-3.0.4/querent/tools/web_page_extractor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/utils/webpage_extractor.py` & `querent-3.0.4/querent/utils/webpage_extractor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/workflow/_helpers.py` & `querent-3.0.4/querent/workflow/_helpers.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent/workflow/workflow.py` & `querent-3.0.4/querent/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent.egg-info/PKG-INFO` & `querent-3.0.4/querent.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: querent
-Version: 3.0.3
+Version: 3.0.4
 Summary: The Asynchronous Data Dynamo and Graph Neural Network Catalyst
 Home-page: https://github.com/Querent-ai/querent-ai
 Author: Querent AI
 License: Business Source License 1.1
 Project-URL: Documentation, https://github.com/Querent-ai/querent-ai/docs
 Project-URL: Issue Tracker, https://github.com/Querent-ai/querent-ai/issues
 Keywords: Graph Neural Network,Scalability,Data-Driven Insights,GNN,Async,Knowledge Graphs,KG,Large Language Models,asyncio,Insights,aysnchronous,LLM,transformers,pytorch,Llama-index,AI,Artificial Intelligence,Neo4j,Queues,QuiAssisstant,Collectors,Data,Data Science,Data Engineering,Data Analysis,Data Analytics,News,NLP,Natural Language Processing,Text,Text Analysis,Deep Learning,Graphs,Graph Theory,Graph Algorithms,Graph Analytics,Graph Databases,Graph Processing,Graph Mining,Graph Neural Networks,GNN,GNNs,Graph Neural Network
@@ -35,85 +35,81 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Typing :: Typed
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 License-File: LICENCE
-Requires-Dist: cachetools==5.3.3
+Requires-Dist: aiofiles==23.2.1
 Requires-Dist: aiohttp==3.9.3
 Requires-Dist: attrs==23.1.0
+Requires-Dist: azure-storage-blob==12.19.0
 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: boto3==1.26.146
 Requires-Dist: botocore==1.29.146
 Requires-Dist: bs4==0.0.1
+Requires-Dist: cachetools==5.3.3
+Requires-Dist: coverage==7.3.3
+Requires-Dist: dropbox==11.36.2
 Requires-Dist: faiss-cpu==1.7.4
+Requires-Dist: ffmpeg-python==0.2.0
 Requires-Dist: gensim==4.3.2
+Requires-Dist: google-api-python-client==2.105.0
+Requires-Dist: google-cloud-storage==2.14.0
+Requires-Dist: google-cloud-storage==2.14.0
+Requires-Dist: google-cloud-storage==2.14.0
 Requires-Dist: hdbscan==0.8.33
 Requires-Dist: jira==3.6.0
 Requires-Dist: jmespath==1.0.1
 Requires-Dist: joblib==1.2.0
 Requires-Dist: json5==0.9.24
 Requires-Dist: jsonmerge==1.9.0
 Requires-Dist: jsonschema==4.17.3
 Requires-Dist: kombu==5.2.4
+Requires-Dist: langchain==0.1.11
+Requires-Dist: langchain-community==0.0.25
 Requires-Dist: llama_cpp_python==0.2.15
 Requires-Dist: lxml==4.9.2
+Requires-Dist: moviepy==1.0.3
 Requires-Dist: newspaper3k==0.2.8
+Requires-Dist: newsapi-python==0.2.7
 Requires-Dist: nltk==3.8.1
 Requires-Dist: numpy==1.24.3
-Requires-Dist: Pillow==10.3.0
+Requires-Dist: openai==1.13.3
+Requires-Dist: openpyxl==3.1.2
+Requires-Dist: pandas==2.1.4
+Requires-Dist: pdfminer==20191125
+Requires-Dist: pillow==10.3.0
+Requires-Dist: prometheus-client==0.17.1
+Requires-Dist: psutil==5.9.8
+Requires-Dist: pybase64==1.3.1
 Requires-Dist: pydantic==2.6.4
-Requires-Dist: PyJWT==2.4.0
-Requires-Dist: pytest==7.3.2
-Requires-Dist: python-dotenv==1.0.0
-Requires-Dist: redis==5.0.3
-Requires-Dist: regex==2023.5.5
-Requires-Dist: sentence-transformers==2.2.2
-Requires-Dist: spacy==3.7.2
-Requires-Dist: uvicorn==0.29.0
-Requires-Dist: slack-sdk==3.26.1
+Requires-Dist: pydub==0.25.1
+Requires-Dist: pyjwt==2.4.0
 Requires-Dist: pylint==2.17.4
-Requires-Dist: pytest-cov==4.1.0
-Requires-Dist: pytest-mock==3.11.1
-Requires-Dist: tensorflow==2.14.0
-Requires-Dist: transformers==4.36.0
-Requires-Dist: asyncio==3.4.3
-Requires-Dist: aiofiles==23.2.1
-Requires-Dist: prometheus-client==0.17.1
-Requires-Dist: rdflib==7.0.0
-Requires-Dist: pytest-asyncio==0.23.2
+Requires-Dist: pymupdf==1.24.0
 Requires-Dist: pyshacl==0.25.0
-Requires-Dist: google-cloud-storage==2.14.0
-Requires-Dist: PyMuPDF==1.24.0
-Requires-Dist: pydub==0.25.1
-Requires-Dist: SpeechRecognition==3.10.1
 Requires-Dist: pytesseract==0.3.10
 Requires-Dist: pytextract==2.0.1
-Requires-Dist: pandas==2.1.4
-Requires-Dist: python-pptx==0.6.23
-Requires-Dist: tika==2.6.0
-Requires-Dist: openpyxl==3.1.2
-Requires-Dist: coverage==7.3.3
-Requires-Dist: azure-storage-blob==12.19.0
-Requires-Dist: moviepy==1.0.3
+Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: python-docx==1.1.0
-Requires-Dist: dropbox==11.36.2
+Requires-Dist: python-pptx==0.6.23
+Requires-Dist: rdflib==7.0.0
+Requires-Dist: redis==5.0.3
+Requires-Dist: regex==2023.5.5
 Requires-Dist: requests==2.31.0
-Requires-Dist: google-api-python-client==2.105.0
 Requires-Dist: requests_html==0.10.0
-Requires-Dist: pybase64==1.3.1
-Requires-Dist: pdfminer==20191125
+Requires-Dist: slack-sdk==3.26.1
+Requires-Dist: slack-sdk==3.26.1
+Requires-Dist: spacy==3.7.2
+Requires-Dist: speechrecognition==3.10.1
+Requires-Dist: tika==2.6.0
+Requires-Dist: transformers==4.36.0
 Requires-Dist: unidecode==1.3.7
-Requires-Dist: psutil==5.9.8
-Requires-Dist: langchain-community==0.0.25
-Requires-Dist: langchain==0.1.11
-Requires-Dist: openai==1.13.3
-Requires-Dist: newsapi-python==0.2.7
-Requires-Dist: ffmpeg-python==0.2.0
+Requires-Dist: sentence-transformers==2.2.2
 
 # Querent
 
 The Asynchronous Data Dynamo and Graph Neural Network Catalyst
 
 ![image](https://github.com/Querent-ai/querent-ai/assets/61435908/39124a0c-3d9e-434f-9b54-9aa51dcefbd7)
```

### Comparing `querent-3.0.3/querent.egg-info/SOURCES.txt` & `querent-3.0.4/querent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `querent-3.0.3/querent.egg-info/requires.txt` & `querent-3.0.4/querent.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,71 +1,67 @@
-cachetools==5.3.3
+aiofiles==23.2.1
 aiohttp==3.9.3
 attrs==23.1.0
+azure-storage-blob==12.19.0
 beautifulsoup4==4.12.3
 boto3==1.26.146
 botocore==1.29.146
 bs4==0.0.1
+cachetools==5.3.3
+coverage==7.3.3
+dropbox==11.36.2
 faiss-cpu==1.7.4
+ffmpeg-python==0.2.0
 gensim==4.3.2
+google-api-python-client==2.105.0
+google-cloud-storage==2.14.0
+google-cloud-storage==2.14.0
+google-cloud-storage==2.14.0
 hdbscan==0.8.33
 jira==3.6.0
 jmespath==1.0.1
 joblib==1.2.0
 json5==0.9.24
 jsonmerge==1.9.0
 jsonschema==4.17.3
 kombu==5.2.4
+langchain==0.1.11
+langchain-community==0.0.25
 llama_cpp_python==0.2.15
 lxml==4.9.2
+moviepy==1.0.3
 newspaper3k==0.2.8
+newsapi-python==0.2.7
 nltk==3.8.1
 numpy==1.24.3
-Pillow==10.3.0
+openai==1.13.3
+openpyxl==3.1.2
+pandas==2.1.4
+pdfminer==20191125
+pillow==10.3.0
+prometheus-client==0.17.1
+psutil==5.9.8
+pybase64==1.3.1
 pydantic==2.6.4
-PyJWT==2.4.0
-pytest==7.3.2
-python-dotenv==1.0.0
-redis==5.0.3
-regex==2023.5.5
-sentence-transformers==2.2.2
-spacy==3.7.2
-uvicorn==0.29.0
-slack-sdk==3.26.1
+pydub==0.25.1
+pyjwt==2.4.0
 pylint==2.17.4
-pytest-cov==4.1.0
-pytest-mock==3.11.1
-tensorflow==2.14.0
-transformers==4.36.0
-asyncio==3.4.3
-aiofiles==23.2.1
-prometheus-client==0.17.1
-rdflib==7.0.0
-pytest-asyncio==0.23.2
+pymupdf==1.24.0
 pyshacl==0.25.0
-google-cloud-storage==2.14.0
-PyMuPDF==1.24.0
-pydub==0.25.1
-SpeechRecognition==3.10.1
 pytesseract==0.3.10
 pytextract==2.0.1
-pandas==2.1.4
-python-pptx==0.6.23
-tika==2.6.0
-openpyxl==3.1.2
-coverage==7.3.3
-azure-storage-blob==12.19.0
-moviepy==1.0.3
+python-dotenv==1.0.0
 python-docx==1.1.0
-dropbox==11.36.2
+python-pptx==0.6.23
+rdflib==7.0.0
+redis==5.0.3
+regex==2023.5.5
 requests==2.31.0
-google-api-python-client==2.105.0
 requests_html==0.10.0
-pybase64==1.3.1
-pdfminer==20191125
+slack-sdk==3.26.1
+slack-sdk==3.26.1
+spacy==3.7.2
+speechrecognition==3.10.1
+tika==2.6.0
+transformers==4.36.0
 unidecode==1.3.7
-psutil==5.9.8
-langchain-community==0.0.25
-langchain==0.1.11
-openai==1.13.3
-newsapi-python==0.2.7
-ffmpeg-python==0.2.0
+sentence-transformers==2.2.2
```

### Comparing `querent-3.0.3/setup.py` & `querent-3.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,93 +1,90 @@
 """
     Querent AI: The Asynchronous Data Dynamo and Graph Neural Network Catalyst
 """
 
 from setuptools import setup, find_packages
 
 requirements = [
-    "cachetools==5.3.3",
+    "aiofiles==23.2.1",
     "aiohttp==3.9.3",
     "attrs==23.1.0",
+    "azure-storage-blob==12.19.0",
     "beautifulsoup4==4.12.3",
     "boto3==1.26.146",
     "botocore==1.29.146",
     "bs4==0.0.1",
+    "cachetools==5.3.3",
+    "coverage==7.3.3",
+    "dropbox==11.36.2",
     "faiss-cpu==1.7.4",
+    "ffmpeg-python==0.2.0",
     "gensim==4.3.2",
+    "google-api-python-client==2.105.0",
+    "google-cloud-storage==2.14.0",
+    "google-cloud-storage==2.14.0",
+    "google-cloud-storage==2.14.0",
     "hdbscan==0.8.33",
     "jira==3.6.0",
     "jmespath==1.0.1",
     "joblib==1.2.0",
     "json5==0.9.24",
     "jsonmerge==1.9.0",
     "jsonschema==4.17.3",
     "kombu==5.2.4",
+    "langchain==0.1.11",
+    "langchain-community==0.0.25",
     "llama_cpp_python==0.2.15",
     "lxml==4.9.2",
+    "moviepy==1.0.3",
     "newspaper3k==0.2.8",
+    "newsapi-python==0.2.7",
     "nltk==3.8.1",
     "numpy==1.24.3",
-    "Pillow==10.3.0",
+    "openai==1.13.3",
+    "openpyxl==3.1.2",
+    "pandas==2.1.4",
+    "pdfminer==20191125",
+    "pillow==10.3.0",
+    "prometheus-client==0.17.1",
+    "psutil==5.9.8",
+    "pybase64==1.3.1",
     "pydantic==2.6.4",
-    "PyJWT==2.4.0",
-    "pytest==7.3.2",
-    "python-dotenv==1.0.0",
-    "redis==5.0.3",
-    "regex==2023.5.5",
-    "sentence-transformers==2.2.2",
-    "spacy==3.7.2",
-    "uvicorn==0.29.0",
-    "slack-sdk==3.26.1",
+    "pydub==0.25.1",
+    "pyjwt==2.4.0",
     "pylint==2.17.4",
-    "pytest-cov==4.1.0",
-    "pytest-mock==3.11.1",
-    "tensorflow==2.14.0",
-    "transformers==4.36.0",
-    "asyncio==3.4.3",
-    "aiofiles==23.2.1",
-    "prometheus-client==0.17.1",
-    "rdflib==7.0.0",
-    "pytest-asyncio==0.23.2",
+    "pymupdf==1.24.0",
     "pyshacl==0.25.0",
-    "google-cloud-storage==2.14.0",
-    "PyMuPDF==1.24.0",
-    "pydub==0.25.1",
-    "SpeechRecognition==3.10.1",
     "pytesseract==0.3.10",
     "pytextract==2.0.1",
-    "pandas==2.1.4",
-    "python-pptx==0.6.23",
-    "tika==2.6.0",
-    "openpyxl==3.1.2",
-    "coverage==7.3.3",
-    "azure-storage-blob==12.19.0",
-    "moviepy==1.0.3",
+    "python-dotenv==1.0.0",
     "python-docx==1.1.0",
-    "dropbox==11.36.2",
+    "python-pptx==0.6.23",
+    "rdflib==7.0.0",
+    "redis==5.0.3",
+    "regex==2023.5.5",
     "requests==2.31.0",
-    "google-api-python-client==2.105.0",
     "requests_html==0.10.0",
-    "pybase64==1.3.1",
-    "pdfminer==20191125",
+    "slack-sdk==3.26.1",
+    "slack-sdk==3.26.1",
+    "spacy==3.7.2",
+    "speechrecognition==3.10.1",
+    "tika==2.6.0",
+    "transformers==4.36.0",
     "unidecode==1.3.7",
-    "psutil==5.9.8",
-    "langchain-community==0.0.25",
-    "langchain==0.1.11",
-    "openai==1.13.3",
-    "newsapi-python==0.2.7",
-    "ffmpeg-python==0.2.0"
+    "sentence-transformers==2.2.2",
 ]
 
+
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="querent",
-    version="3.0.3",
+    version="3.0.4",
     author="Querent AI",
     description="The Asynchronous Data Dynamo and Graph Neural Network Catalyst",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Querent-ai/querent-ai",
     project_urls={
         "Documentation": "https://github.com/Querent-ai/querent-ai/docs",
```

