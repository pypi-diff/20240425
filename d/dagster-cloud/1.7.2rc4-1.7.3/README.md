# Comparing `tmp/dagster-cloud-1.7.2rc4.tar.gz` & `tmp/dagster-cloud-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-cloud-1.7.2rc4.tar", last modified: Fri Apr 19 18:15:29 2024, max compression
+gzip compressed data, was "dagster-cloud-1.7.3.tar", last modified: Thu Apr 25 20:21:35 2024, max compression
```

## Comparing `dagster-cloud-1.7.2rc4.tar` & `dagster-cloud-1.7.3.tar`

### file list

```diff
@@ -1,14 +1,140 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:15:29.691013 dagster-cloud-1.7.2rc4/
--rw-r--r--   0 root         (0) root         (0)     3463 2024-04-19 18:15:29.691013 dagster-cloud-1.7.2rc4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1960 2024-04-19 18:02:15.000000 dagster-cloud-1.7.2rc4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:15:29.687013 dagster-cloud-1.7.2rc4/dagster_cloud/
--rw-r--r--   0 root         (0) root         (0)      116 2024-04-19 18:02:15.000000 dagster-cloud-1.7.2rc4/dagster_cloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-19 18:02:15.000000 dagster-cloud-1.7.2rc4/dagster_cloud/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:15:29.687013 dagster-cloud-1.7.2rc4/dagster_cloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3463 2024-04-19 18:15:29.000000 dagster-cloud-1.7.2rc4/dagster_cloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      253 2024-04-19 18:15:29.000000 dagster-cloud-1.7.2rc4/dagster_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 18:15:29.000000 dagster-cloud-1.7.2rc4/dagster_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      359 2024-04-19 18:15:29.000000 dagster-cloud-1.7.2rc4/dagster_cloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-19 18:15:29.000000 dagster-cloud-1.7.2rc4/dagster_cloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-19 18:15:29.691013 dagster-cloud-1.7.2rc4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2539 2024-04-19 18:02:15.000000 dagster-cloud-1.7.2rc4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.897462 dagster-cloud-1.7.3/
+-rw-r--r--   0 root         (0) root         (0)     4562 2024-04-25 20:21:35.897462 dagster-cloud-1.7.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3062 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.833463 dagster-cloud-1.7.3/dagster_cloud/
+-rw-r--r--   0 root         (0) root         (0)      160 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.833463 dagster-cloud-1.7.3/dagster_cloud/agent/
+-rw-r--r--   0 root         (0) root         (0)      796 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.837463 dagster-cloud-1.7.3/dagster_cloud/agent/cli/
+-rw-r--r--   0 root         (0) root         (0)     7584 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/agent/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45467 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/agent/dagster_cloud_agent.py
+-rw-r--r--   0 root         (0) root         (0)     1770 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/agent/queries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.841463 dagster-cloud-1.7.3/dagster_cloud/anomaly_detection/
+-rw-r--r--   0 root         (0) root         (0)      279 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/anomaly_detection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9296 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/anomaly_detection/defs.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/anomaly_detection/mutation.py
+-rw-r--r--   0 root         (0) root         (0)     1986 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/anomaly_detection/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.841463 dagster-cloud-1.7.3/dagster_cloud/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19251 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/api/dagster_cloud_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.841463 dagster-cloud-1.7.3/dagster_cloud/artifacts/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/artifacts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.841463 dagster-cloud-1.7.3/dagster_cloud/auth/
+-rw-r--r--   0 root         (0) root         (0)      248 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1242 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/auth/constants.py
+-rw-r--r--   0 root         (0) root         (0)      455 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.845463 dagster-cloud-1.7.3/dagster_cloud/dagster_insights/
+-rw-r--r--   0 root         (0) root         (0)     1873 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/dagster_insights/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.845463 dagster-cloud-1.7.3/dagster_cloud/dagster_insights/bigquery/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/dagster_insights/bigquery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      816 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/dagster_insights/bigquery/bigquery_utils.py
+-rw-r--r--   0 root         (0) root         (0)     7964 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/dagster_insights/bigquery/dbt_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     3234 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/dagster_insights/bigquery/insights_bigquery_resource.py
+-rw-r--r--   0 root         (0) root         (0)      138 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/dagster_insights/errors.py
+-rw-r--r--   0 root         (0) root         (0)     2524 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/dagster_insights/insights_utils.py
+-rw-r--r--   0 root         (0) root         (0)    10835 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/dagster_insights/metrics_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1403 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/dagster_insights/query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.849463 dagster-cloud-1.7.3/dagster_cloud/dagster_insights/snowflake/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/dagster_insights/snowflake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5611 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/dagster_insights/snowflake/dagster_snowflake_insights.py
+-rw-r--r--   0 root         (0) root         (0)     5185 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/dagster_insights/snowflake/dbt_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     7064 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/dagster_insights/snowflake/definitions.py
+-rw-r--r--   0 root         (0) root         (0)     9358 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/dagster_insights/snowflake/insights_snowflake_resource.py
+-rw-r--r--   0 root         (0) root         (0)     3808 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/dagster_insights/snowflake/snowflake_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.849463 dagster-cloud-1.7.3/dagster_cloud/execution/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/execution/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.853463 dagster-cloud-1.7.3/dagster_cloud/execution/cloud_run_launcher/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/execution/cloud_run_launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      327 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/execution/cloud_run_launcher/k8s.py
+-rw-r--r--   0 root         (0) root         (0)     3098 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/execution/cloud_run_launcher/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.853463 dagster-cloud-1.7.3/dagster_cloud/execution/monitoring/
+-rw-r--r--   0 root         (0) root         (0)    17256 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/execution/monitoring/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.853463 dagster-cloud-1.7.3/dagster_cloud/execution/utils/
+-rw-r--r--   0 root         (0) root         (0)      254 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/execution/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      875 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/execution/utils/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.857463 dagster-cloud-1.7.3/dagster_cloud/instance/
+-rw-r--r--   0 root         (0) root         (0)    22345 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/instance/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.857463 dagster-cloud-1.7.3/dagster_cloud/metrics/
+-rw-r--r--   0 root         (0) root         (0)    10090 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/metrics/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.857463 dagster-cloud-1.7.3/dagster_cloud/pex/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/pex/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.857463 dagster-cloud-1.7.3/dagster_cloud/pex/grpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.861463 dagster-cloud-1.7.3/dagster_cloud/pex/grpc/__generated__/
+-rw-r--r--   0 root         (0) root         (0)      285 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/pex/grpc/__generated__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3907 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9301 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      327 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/pex/grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5251 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/pex/grpc/client.py
+-rw-r--r--   0 root         (0) root         (0)     3790 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/pex/grpc/compile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.865463 dagster-cloud-1.7.3/dagster_cloud/pex/grpc/server/
+-rw-r--r--   0 root         (0) root         (0)      119 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/pex/grpc/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.865463 dagster-cloud-1.7.3/dagster_cloud/pex/grpc/server/cli/
+-rw-r--r--   0 root         (0) root         (0)     2115 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/pex/grpc/server/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17843 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/pex/grpc/server/manager.py
+-rw-r--r--   0 root         (0) root         (0)    12797 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/pex/grpc/server/registry.py
+-rw-r--r--   0 root         (0) root         (0)    15703 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/pex/grpc/server/server.py
+-rw-r--r--   0 root         (0) root         (0)     3322 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/pex/grpc/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.865463 dagster-cloud-1.7.3/dagster_cloud/secrets/
+-rw-r--r--   0 root         (0) root         (0)       75 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1620 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/secrets/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.865463 dagster-cloud-1.7.3/dagster_cloud/serverless/
+-rw-r--r--   0 root         (0) root         (0)       71 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/serverless/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4247 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/serverless/io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.869463 dagster-cloud-1.7.3/dagster_cloud/storage/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1690 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/storage/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.869463 dagster-cloud-1.7.3/dagster_cloud/storage/compute_logs/
+-rw-r--r--   0 root         (0) root         (0)       82 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/storage/compute_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4753 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/storage/compute_logs/compute_log_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.873463 dagster-cloud-1.7.3/dagster_cloud/storage/event_logs/
+-rw-r--r--   0 root         (0) root         (0)       70 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/storage/event_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16377 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/storage/event_logs/queries.py
+-rw-r--r--   0 root         (0) root         (0)    46580 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/storage/event_logs/storage.py
+-rw-r--r--   0 root         (0) root         (0)      658 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/storage/event_logs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.873463 dagster-cloud-1.7.3/dagster_cloud/storage/runs/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/storage/runs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6446 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/storage/runs/queries.py
+-rw-r--r--   0 root         (0) root         (0)    18839 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/storage/runs/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.873463 dagster-cloud-1.7.3/dagster_cloud/storage/schedules/
+-rw-r--r--   0 root         (0) root         (0)       70 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/storage/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1930 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/storage/schedules/queries.py
+-rw-r--r--   0 root         (0) root         (0)     7575 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/storage/schedules/storage.py
+-rw-r--r--   0 root         (0) root         (0)      502 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/storage/tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.877463 dagster-cloud-1.7.3/dagster_cloud/util/
+-rw-r--r--   0 root         (0) root         (0)     2778 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4693 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/util/container_resources.py
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.877463 dagster-cloud-1.7.3/dagster_cloud/workspace/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.881463 dagster-cloud-1.7.3/dagster_cloud/workspace/config_schema/
+-rw-r--r--   0 root         (0) root         (0)    10918 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/config_schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      967 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/config_schema/docker.py
+-rw-r--r--   0 root         (0) root         (0)     6575 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/config_schema/ecs.py
+-rw-r--r--   0 root         (0) root         (0)     5319 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/config_schema/kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.881463 dagster-cloud-1.7.3/dagster_cloud/workspace/docker/
+-rw-r--r--   0 root         (0) root         (0)    12977 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/docker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      352 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/docker/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.885463 dagster-cloud-1.7.3/dagster_cloud/workspace/ecs/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/ecs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28818 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/ecs/client.py
+-rw-r--r--   0 root         (0) root         (0)    28623 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/ecs/launcher.py
+-rw-r--r--   0 root         (0) root         (0)      534 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/ecs/run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     4126 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/ecs/service.py
+-rw-r--r--   0 root         (0) root         (0)     2746 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/ecs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.889463 dagster-cloud-1.7.3/dagster_cloud/workspace/kubernetes/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/kubernetes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26248 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/kubernetes/launcher.py
+-rw-r--r--   0 root         (0) root         (0)     9825 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/kubernetes/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.897462 dagster-cloud-1.7.3/dagster_cloud/workspace/user_code_launcher/
+-rw-r--r--   0 root         (0) root         (0)      745 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/user_code_launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14248 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/user_code_launcher/process.py
+-rw-r--r--   0 root         (0) root         (0)    83997 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1209 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/user_code_launcher/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.833463 dagster-cloud-1.7.3/dagster_cloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4562 2024-04-25 20:21:35.000000 dagster-cloud-1.7.3/dagster_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4274 2024-04-25 20:21:35.000000 dagster-cloud-1.7.3/dagster_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 20:21:35.000000 dagster-cloud-1.7.3/dagster_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      509 2024-04-25 20:21:35.000000 dagster-cloud-1.7.3/dagster_cloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-25 20:21:35.000000 dagster-cloud-1.7.3/dagster_cloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 20:21:35.897462 dagster-cloud-1.7.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3078 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/setup.py
```

### Comparing `dagster-cloud-1.7.2rc4/PKG-INFO` & `dagster-cloud-1.7.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,7 @@
-Metadata-Version: 2.1
-Name: dagster-cloud
-Version: 1.7.2rc4
-Author: Elementl
-Author-email: support@elementl.com
-License: Apache-2.0
-Project-URL: Homepage, https://dagster.io/cloud
-Project-URL: GitHub, https://github.com/dagster-io/dagster-cloud
-Project-URL: Changelog, https://github.com/dagster-io/dagster-cloud/blob/main/CHANGES.md
-Project-URL: Issue Tracker, https://github.com/dagster-io/dagster-cloud/issues
-Project-URL: Twitter, https://twitter.com/dagster
-Project-URL: LinkedIn, https://www.linkedin.com/showcase/dagster
-Project-URL: YouTube, https://www.youtube.com/channel/UCfLnv9X8jyHTe6gJ4hVBo9Q
-Project-URL: Slack, https://dagster.io/slack
-Project-URL: Blog, https://dagster.io/blog
-Project-URL: Newsletter, https://dagster.io/newsletter-signup
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: System Administrators
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Topic :: System :: Monitoring
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-Provides-Extra: insights
-Provides-Extra: docker
-Provides-Extra: kubernetes
-Provides-Extra: ecs
-Provides-Extra: sandbox
-Provides-Extra: pex
-Provides-Extra: serverless
-
 <p align="center">
   <a target="_blank" href="https://dagster.io/cloud" style="background:none">
     <img src="https://github.com/dagster-io/dagster-cloud/raw/main/assets/dagster-cloud-logo.png" width="auto"/>
   </a>
   <br /><br />
   <a target="_blank" href="https://twitter.com/dagster" style="background:none">
     <img src="https://img.shields.io/badge/twitter-dagster-blue.svg?labelColor=4F43DD&color=163B36&logo=twitter" />
@@ -66,10 +30,37 @@
 
 ## Getting Started
 
 The complete Dagster Cloud feature set can be found on our [website](https://dagster.io/cloud). You
 can [sign up for Dagster Cloud](https://dagster.cloud/signup) and get started with a free 30 day
 trial.
 
-## Deprecation
+## Installation
+
+The Dagster Cloud Agent is available on PyPI and officially supports Python 3.8.
+
+```
+pip install dagster-cloud
+```
+
+## Documentation
+
+You can find the full Dagster Cloud documentation on our
+[website](https://docs.dagster.io/dagster-cloud).
+
+## Community
+
+Connect with thousands of other data practitioners building with Dagster. Share knowledge, get help,
+and contribute to the open-source project. To see featured material and upcoming events, check out
+our [Dagster Community](https://dagster.io/community) page.
+
+Join our community here:
 
-This package has been renamed. Use pip install dagster-plus instead.
+- 🌟 [Star us on Github](https://github.com/dagster-io/dagster)
+- 📥 [Subscribe to our Newsletter](https://dagster.io/newsletter-signup)
+- 🐦 [Follow us on Twitter](https://twitter.com/dagster)
+- 🕴️ [Follow us on LinkedIn](https://linkedin.com/showcase/dagster)
+- 📺 [Subscribe to our YouTube channel](https://www.youtube.com/channel/UCfLnv9X8jyHTe6gJ4hVBo9Q)
+- 📚 [Read our blog posts](https://dagster.io/blog)
+- 👋 [Join us on Slack](https://dagster.io/slack)
+- 🗃 [Browse Slack archives](https://discuss.dagster.io)
+- ✏️ [Start a Github Discussion](https://github.com/dagster-io/dagster/discussions)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dagster-cloud-1.7.2rc4/dagster_cloud.egg-info/PKG-INFO` & `dagster-cloud-1.7.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-cloud
-Version: 1.7.2rc4
+Version: 1.7.3
 Author: Elementl
 Author-email: support@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io/cloud
 Project-URL: GitHub, https://github.com/dagster-io/dagster-cloud
 Project-URL: Changelog, https://github.com/dagster-io/dagster-cloud/blob/main/CHANGES.md
 Project-URL: Issue Tracker, https://github.com/dagster-io/dagster-cloud/issues
@@ -66,10 +66,37 @@
 
 ## Getting Started
 
 The complete Dagster Cloud feature set can be found on our [website](https://dagster.io/cloud). You
 can [sign up for Dagster Cloud](https://dagster.cloud/signup) and get started with a free 30 day
 trial.
 
-## Deprecation
+## Installation
 
-This package has been renamed. Use pip install dagster-plus instead.
+The Dagster Cloud Agent is available on PyPI and officially supports Python 3.8.
+
+```
+pip install dagster-cloud
+```
+
+## Documentation
+
+You can find the full Dagster Cloud documentation on our
+[website](https://docs.dagster.io/dagster-cloud).
+
+## Community
+
+Connect with thousands of other data practitioners building with Dagster. Share knowledge, get help,
+and contribute to the open-source project. To see featured material and upcoming events, check out
+our [Dagster Community](https://dagster.io/community) page.
+
+Join our community here:
+
+- 🌟 [Star us on Github](https://github.com/dagster-io/dagster)
+- 📥 [Subscribe to our Newsletter](https://dagster.io/newsletter-signup)
+- 🐦 [Follow us on Twitter](https://twitter.com/dagster)
+- 🕴️ [Follow us on LinkedIn](https://linkedin.com/showcase/dagster)
+- 📺 [Subscribe to our YouTube channel](https://www.youtube.com/channel/UCfLnv9X8jyHTe6gJ4hVBo9Q)
+- 📚 [Read our blog posts](https://dagster.io/blog)
+- 👋 [Join us on Slack](https://dagster.io/slack)
+- 🗃 [Browse Slack archives](https://discuss.dagster.io)
+- ✏️ [Start a Github Discussion](https://github.com/dagster-io/dagster/discussions)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dagster-cloud-1.7.2rc4/setup.py` & `dagster-cloud-1.7.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -36,25 +36,50 @@
         "Slack": "https://dagster.io/slack",
         "Blog": "https://dagster.io/blog",
         "Newsletter": "https://dagster.io/newsletter-signup",
     },
     packages=find_packages(exclude=["dagster_cloud_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster-plus==1.7.2rc4",
+        "dagster==1.7.3",
+        "dagster-cloud-cli==1.7.3",
+        "pex>=2.1.132,<3",
+        "questionary",
+        "requests",
+        "typer[all]",
     ],
     extras_require={
-        "tests": [f"dagster-plus[tests]{pin}"],
-        "insights": [f"dagster-plus[insights]{pin}"],
-        "docker": [f"dagster-plus[docker]{pin}"],
-        "kubernetes": [f"dagster-plus[kubernetes]{pin}"],
-        "ecs": [f"dagster-plus[ecs]{pin}"],
-        "sandbox": [f"dagster-plus[sandbox]{pin}"],
-        "pex": [f"dagster-plus[pex]{pin}"],
-        "serverless": [f"dagster-plus[serverless]{pin}"],
+        "tests": [
+            "docker",
+            "httpretty",
+            "isort",
+            "kubernetes",
+            "moto[all]",
+            "mypy",
+            "paramiko",
+            "psutil",
+            "pylint",
+            "pytest",
+            "types-PyYAML",
+            "types-requests",
+            "dagster-cloud-test-infra",
+            "dbt-core",
+            "dbt-snowflake",
+            "dbt-postgres",
+            "dbt-duckdb",
+            "dagster-dbt==0.23.3",
+            "dagster_k8s==0.23.3",
+        ],
+        "insights": ["pyarrow"],
+        "docker": ["docker", "dagster_docker==0.23.3"],
+        "kubernetes": ["kubernetes", "dagster_k8s==0.23.3"],
+        "ecs": ["dagster_aws==0.23.3", "boto3"],
+        "sandbox": ["supervisor"],
+        "pex": ["boto3"],
+        "serverless": ["boto3"],
     },
     author="Elementl",
     license="Apache-2.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Environment :: Web Environment",
```

