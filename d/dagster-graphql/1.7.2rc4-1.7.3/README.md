# Comparing `tmp/dagster-graphql-1.7.2rc4.tar.gz` & `tmp/dagster-graphql-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-graphql-1.7.2rc4.tar", last modified: Fri Apr 19 18:02:49 2024, max compression
+gzip compressed data, was "dagster-graphql-1.7.3.tar", last modified: Thu Apr 25 20:09:27 2024, max compression
```

## Comparing `dagster-graphql-1.7.2rc4.tar` & `dagster-graphql-1.7.3.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:49.529970 dagster-graphql-1.7.2rc4/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       49 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      694 2024-04-19 18:02:49.529970 dagster-graphql-1.7.2rc4/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:49.509970 dagster-graphql-1.7.2rc4/dagster_graphql/
--rw-r--r--   0 root         (0) root         (0)      641 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7401 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:49.513970 dagster-graphql-1.7.2rc4/dagster_graphql/client/
--rw-r--r--   0 root         (0) root         (0)      482 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18338 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/client/client.py
--rw-r--r--   0 root         (0) root         (0)     2917 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/client/client_queries.py
--rw-r--r--   0 root         (0) root         (0)     6966 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/client/query.py
--rw-r--r--   0 root         (0) root         (0)     2917 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/client/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:49.517970 dagster-graphql-1.7.2rc4/dagster_graphql/implementation/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/implementation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12826 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/implementation/asset_checks_loader.py
--rw-r--r--   0 root         (0) root         (0)    20532 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/implementation/events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:49.517970 dagster-graphql-1.7.2rc4/dagster_graphql/implementation/execution/
--rw-r--r--   0 root         (0) root         (0)    14499 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/implementation/execution/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12314 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/implementation/execution/backfill.py
--rw-r--r--   0 root         (0) root         (0)     3727 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/implementation/execution/dynamic_partitions.py
--rw-r--r--   0 root         (0) root         (0)     4819 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/implementation/execution/launch_execution.py
--rw-r--r--   0 root         (0) root         (0)     4895 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/implementation/execution/run_lifecycle.py
--rw-r--r--   0 root         (0) root         (0)     7310 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/implementation/external.py
--rw-r--r--   0 root         (0) root         (0)     4251 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/implementation/fetch_asset_checks.py
--rw-r--r--   0 root         (0) root         (0)     4926 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/implementation/fetch_asset_condition_evaluations.py
--rw-r--r--   0 root         (0) root         (0)    28971 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/implementation/fetch_assets.py
--rw-r--r--   0 root         (0) root         (0)     3658 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py
--rw-r--r--   0 root         (0) root         (0)     1237 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/implementation/fetch_backfills.py
--rw-r--r--   0 root         (0) root         (0)     1179 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/implementation/fetch_env_vars.py
--rw-r--r--   0 root         (0) root         (0)     3009 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/implementation/fetch_instigators.py
--rw-r--r--   0 root         (0) root         (0)      951 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/implementation/fetch_logs.py
--rw-r--r--   0 root         (0) root         (0)    12681 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/implementation/fetch_partition_sets.py
--rw-r--r--   0 root         (0) root         (0)     3726 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/implementation/fetch_pipelines.py
--rw-r--r--   0 root         (0) root         (0)     2438 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/implementation/fetch_resources.py
--rw-r--r--   0 root         (0) root         (0)    15163 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/implementation/fetch_runs.py
--rw-r--r--   0 root         (0) root         (0)     9069 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/implementation/fetch_schedules.py
--rw-r--r--   0 root         (0) root         (0)    10352 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/implementation/fetch_sensors.py
--rw-r--r--   0 root         (0) root         (0)     2912 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/implementation/fetch_solids.py
--rw-r--r--   0 root         (0) root         (0)     2345 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/implementation/fetch_ticks.py
--rw-r--r--   0 root         (0) root         (0)    14555 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/implementation/loader.py
--rw-r--r--   0 root         (0) root         (0)     3097 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/implementation/run_config_schema.py
--rw-r--r--   0 root         (0) root         (0)      930 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/implementation/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     9774 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/implementation/utils.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:49.525970 dagster-graphql-1.7.2rc4/dagster_graphql/schema/
--rw-r--r--   0 root         (0) root         (0)     2877 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8533 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/asset_checks.py
--rw-r--r--   0 root         (0) root         (0)    11979 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/asset_condition_evaluations.py
--rw-r--r--   0 root         (0) root         (0)    55189 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/asset_graph.py
--rw-r--r--   0 root         (0) root         (0)      385 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/asset_key.py
--rw-r--r--   0 root         (0) root         (0)     1606 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/asset_selections.py
--rw-r--r--   0 root         (0) root         (0)    10990 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/auto_materialize_asset_evaluations.py
--rw-r--r--   0 root         (0) root         (0)     2586 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/auto_materialize_policy.py
--rw-r--r--   0 root         (0) root         (0)    20849 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/backfill.py
--rw-r--r--   0 root         (0) root         (0)      627 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/config_type_or_error.py
--rw-r--r--   0 root         (0) root         (0)    15855 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/config_types.py
--rw-r--r--   0 root         (0) root         (0)     4823 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/dagster_types.py
--rw-r--r--   0 root         (0) root         (0)     1743 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/env_vars.py
--rw-r--r--   0 root         (0) root         (0)    17941 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/errors.py
--rw-r--r--   0 root         (0) root         (0)     5491 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/execution.py
--rw-r--r--   0 root         (0) root         (0)    18785 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/external.py
--rw-r--r--   0 root         (0) root         (0)     1769 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/freshness_policy.py
--rw-r--r--   0 root         (0) root         (0)    13742 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/inputs.py
--rw-r--r--   0 root         (0) root         (0)    11731 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/instance.py
--rw-r--r--   0 root         (0) root         (0)    28766 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/instigation.py
--rw-r--r--   0 root         (0) root         (0)      232 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/instigators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:49.525970 dagster-graphql-1.7.2rc4/dagster_graphql/schema/logs/
--rw-r--r--   0 root         (0) root         (0)     3632 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2868 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/logs/compute_logs.py
--rw-r--r--   0 root         (0) root         (0)    21701 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/logs/events.py
--rw-r--r--   0 root         (0) root         (0)      816 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/logs/log_level.py
--rw-r--r--   0 root         (0) root         (0)     5440 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/metadata.py
--rw-r--r--   0 root         (0) root         (0)      111 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/paging.py
--rw-r--r--   0 root         (0) root         (0)      529 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/partition_mappings.py
--rw-r--r--   0 root         (0) root         (0)    17797 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/partition_sets.py
--rw-r--r--   0 root         (0) root         (0)      748 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/permissions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:49.525970 dagster-graphql-1.7.2rc4/dagster_graphql/schema/pipelines/
--rw-r--r--   0 root         (0) root         (0)     3263 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/pipelines/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11060 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/pipelines/config.py
--rw-r--r--   0 root         (0) root         (0)      582 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/pipelines/config_result.py
--rw-r--r--   0 root         (0) root         (0)     1369 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/pipelines/logger.py
--rw-r--r--   0 root         (0) root         (0)     1768 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/pipelines/mode.py
--rw-r--r--   0 root         (0) root         (0)    39840 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/pipelines/pipeline.py
--rw-r--r--   0 root         (0) root         (0)      855 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/pipelines/pipeline_ref.py
--rw-r--r--   0 root         (0) root         (0)     2213 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/pipelines/pipeline_run_stats.py
--rw-r--r--   0 root         (0) root         (0)     1496 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/pipelines/resource.py
--rw-r--r--   0 root         (0) root         (0)     1263 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/pipelines/snapshot.py
--rw-r--r--   0 root         (0) root         (0)     1621 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/pipelines/status.py
--rw-r--r--   0 root         (0) root         (0)      993 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/pipelines/subscription.py
--rw-r--r--   0 root         (0) root         (0)     1654 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/repository_origin.py
--rw-r--r--   0 root         (0) root         (0)     9025 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:49.529970 dagster-graphql-1.7.2rc4/dagster_graphql/schema/roots/
--rw-r--r--   0 root         (0) root         (0)     2094 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/roots/__init__.py
--rw-r--r--   0 root         (0) root         (0)      620 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/roots/assets.py
--rw-r--r--   0 root         (0) root         (0)      564 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/roots/execution_plan.py
--rw-r--r--   0 root         (0) root         (0)    32162 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/roots/mutation.py
--rw-r--r--   0 root         (0) root         (0)      723 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/roots/pipeline.py
--rw-r--r--   0 root         (0) root         (0)    46584 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/roots/query.py
--rw-r--r--   0 root         (0) root         (0)     2905 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/roots/subscription.py
--rw-r--r--   0 root         (0) root         (0)     5092 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/run_config.py
--rw-r--r--   0 root         (0) root         (0)     6523 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/runs.py
--rw-r--r--   0 root         (0) root         (0)     1438 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/schedule_dry_run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:49.529970 dagster-graphql-1.7.2rc4/dagster_graphql/schema/schedules/
--rw-r--r--   0 root         (0) root         (0)     4945 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9135 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/schedules/schedules.py
--rw-r--r--   0 root         (0) root         (0)     1833 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/schedules/ticks.py
--rw-r--r--   0 root         (0) root         (0)     1312 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/sensor_dry_run.py
--rw-r--r--   0 root         (0) root         (0)    10196 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/sensors.py
--rw-r--r--   0 root         (0) root         (0)    30059 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/solids.py
--rw-r--r--   0 root         (0) root         (0)     2390 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/table.py
--rw-r--r--   0 root         (0) root         (0)     1421 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/tags.py
--rw-r--r--   0 root         (0) root         (0)      574 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/test.py
--rw-r--r--   0 root         (0) root         (0)      744 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/used_solid.py
--rw-r--r--   0 root         (0) root         (0)      950 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/schema/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:49.529970 dagster-graphql-1.7.2rc4/dagster_graphql/test/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7078 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/test/utils.py
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/dagster_graphql/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:49.513970 dagster-graphql-1.7.2rc4/dagster_graphql.egg-info/
--rw-r--r--   0 root         (0) root         (0)      694 2024-04-19 18:02:49.000000 dagster-graphql-1.7.2rc4/dagster_graphql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4726 2024-04-19 18:02:49.000000 dagster-graphql-1.7.2rc4/dagster_graphql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 18:02:49.000000 dagster-graphql-1.7.2rc4/dagster_graphql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2024-04-19 18:02:49.000000 dagster-graphql-1.7.2rc4/dagster_graphql.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       72 2024-04-19 18:02:49.000000 dagster-graphql-1.7.2rc4/dagster_graphql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-04-19 18:02:49.000000 dagster-graphql-1.7.2rc4/dagster_graphql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      180 2024-04-19 18:02:49.529970 dagster-graphql-1.7.2rc4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1534 2024-04-19 18:01:50.000000 dagster-graphql-1.7.2rc4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:09:27.019996 dagster-graphql-1.7.3/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       49 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      691 2024-04-25 20:09:27.019996 dagster-graphql-1.7.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:09:27.007995 dagster-graphql-1.7.3/dagster_graphql/
+-rw-r--r--   0 root         (0) root         (0)      641 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7401 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:09:27.007995 dagster-graphql-1.7.3/dagster_graphql/client/
+-rw-r--r--   0 root         (0) root         (0)      482 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18338 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     2917 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/client/client_queries.py
+-rw-r--r--   0 root         (0) root         (0)     6966 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/client/query.py
+-rw-r--r--   0 root         (0) root         (0)     2917 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/client/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:09:27.011995 dagster-graphql-1.7.3/dagster_graphql/implementation/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/implementation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12826 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/implementation/asset_checks_loader.py
+-rw-r--r--   0 root         (0) root         (0)    20532 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/implementation/events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:09:27.011995 dagster-graphql-1.7.3/dagster_graphql/implementation/execution/
+-rw-r--r--   0 root         (0) root         (0)    14499 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/implementation/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12314 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/implementation/execution/backfill.py
+-rw-r--r--   0 root         (0) root         (0)     3727 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/implementation/execution/dynamic_partitions.py
+-rw-r--r--   0 root         (0) root         (0)     4819 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/implementation/execution/launch_execution.py
+-rw-r--r--   0 root         (0) root         (0)     4895 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/implementation/execution/run_lifecycle.py
+-rw-r--r--   0 root         (0) root         (0)     7310 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/implementation/external.py
+-rw-r--r--   0 root         (0) root         (0)     4251 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/implementation/fetch_asset_checks.py
+-rw-r--r--   0 root         (0) root         (0)     4926 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/implementation/fetch_asset_condition_evaluations.py
+-rw-r--r--   0 root         (0) root         (0)    28971 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/implementation/fetch_assets.py
+-rw-r--r--   0 root         (0) root         (0)     3658 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py
+-rw-r--r--   0 root         (0) root         (0)     1237 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/implementation/fetch_backfills.py
+-rw-r--r--   0 root         (0) root         (0)     1179 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/implementation/fetch_env_vars.py
+-rw-r--r--   0 root         (0) root         (0)     3009 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/implementation/fetch_instigators.py
+-rw-r--r--   0 root         (0) root         (0)      951 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/implementation/fetch_logs.py
+-rw-r--r--   0 root         (0) root         (0)    12681 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/implementation/fetch_partition_sets.py
+-rw-r--r--   0 root         (0) root         (0)     3726 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/implementation/fetch_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)     2438 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/implementation/fetch_resources.py
+-rw-r--r--   0 root         (0) root         (0)    15163 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/implementation/fetch_runs.py
+-rw-r--r--   0 root         (0) root         (0)     9069 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/implementation/fetch_schedules.py
+-rw-r--r--   0 root         (0) root         (0)    10352 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/implementation/fetch_sensors.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/implementation/fetch_solids.py
+-rw-r--r--   0 root         (0) root         (0)     2345 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/implementation/fetch_ticks.py
+-rw-r--r--   0 root         (0) root         (0)    14555 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/implementation/loader.py
+-rw-r--r--   0 root         (0) root         (0)     3097 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/implementation/run_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)      930 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/implementation/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     9774 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/implementation/utils.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:09:27.015996 dagster-graphql-1.7.3/dagster_graphql/schema/
+-rw-r--r--   0 root         (0) root         (0)     2877 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8533 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/asset_checks.py
+-rw-r--r--   0 root         (0) root         (0)    11979 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/asset_condition_evaluations.py
+-rw-r--r--   0 root         (0) root         (0)    55809 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)      385 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/asset_key.py
+-rw-r--r--   0 root         (0) root         (0)     2188 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/asset_selections.py
+-rw-r--r--   0 root         (0) root         (0)    10990 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/auto_materialize_asset_evaluations.py
+-rw-r--r--   0 root         (0) root         (0)     2586 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/auto_materialize_policy.py
+-rw-r--r--   0 root         (0) root         (0)    20849 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/backfill.py
+-rw-r--r--   0 root         (0) root         (0)      627 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/config_type_or_error.py
+-rw-r--r--   0 root         (0) root         (0)    15855 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/config_types.py
+-rw-r--r--   0 root         (0) root         (0)     4823 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/dagster_types.py
+-rw-r--r--   0 root         (0) root         (0)     1743 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/env_vars.py
+-rw-r--r--   0 root         (0) root         (0)    17941 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/errors.py
+-rw-r--r--   0 root         (0) root         (0)     5491 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/execution.py
+-rw-r--r--   0 root         (0) root         (0)    18785 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/external.py
+-rw-r--r--   0 root         (0) root         (0)     1769 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/freshness_policy.py
+-rw-r--r--   0 root         (0) root         (0)    13742 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/inputs.py
+-rw-r--r--   0 root         (0) root         (0)    12491 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/instance.py
+-rw-r--r--   0 root         (0) root         (0)    28766 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/instigation.py
+-rw-r--r--   0 root         (0) root         (0)      232 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/instigators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:09:27.015996 dagster-graphql-1.7.3/dagster_graphql/schema/logs/
+-rw-r--r--   0 root         (0) root         (0)     3632 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2868 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/logs/compute_logs.py
+-rw-r--r--   0 root         (0) root         (0)    21701 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/logs/events.py
+-rw-r--r--   0 root         (0) root         (0)      816 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/logs/log_level.py
+-rw-r--r--   0 root         (0) root         (0)     5440 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/metadata.py
+-rw-r--r--   0 root         (0) root         (0)      111 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/paging.py
+-rw-r--r--   0 root         (0) root         (0)      529 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/partition_mappings.py
+-rw-r--r--   0 root         (0) root         (0)    17797 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/partition_sets.py
+-rw-r--r--   0 root         (0) root         (0)      748 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/permissions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:09:27.019996 dagster-graphql-1.7.3/dagster_graphql/schema/pipelines/
+-rw-r--r--   0 root         (0) root         (0)     3263 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/pipelines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11060 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/pipelines/config.py
+-rw-r--r--   0 root         (0) root         (0)      582 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/pipelines/config_result.py
+-rw-r--r--   0 root         (0) root         (0)     1369 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/pipelines/logger.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/pipelines/mode.py
+-rw-r--r--   0 root         (0) root         (0)    39840 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/pipelines/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)      855 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/pipelines/pipeline_ref.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/pipelines/pipeline_run_stats.py
+-rw-r--r--   0 root         (0) root         (0)     1496 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/pipelines/resource.py
+-rw-r--r--   0 root         (0) root         (0)     1263 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/pipelines/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     1621 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/pipelines/status.py
+-rw-r--r--   0 root         (0) root         (0)      993 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/pipelines/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     1654 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/repository_origin.py
+-rw-r--r--   0 root         (0) root         (0)     9025 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:09:27.019996 dagster-graphql-1.7.3/dagster_graphql/schema/roots/
+-rw-r--r--   0 root         (0) root         (0)     2094 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/roots/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      620 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/roots/assets.py
+-rw-r--r--   0 root         (0) root         (0)      564 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/roots/execution_plan.py
+-rw-r--r--   0 root         (0) root         (0)    32162 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/roots/mutation.py
+-rw-r--r--   0 root         (0) root         (0)      723 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/roots/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    46584 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/roots/query.py
+-rw-r--r--   0 root         (0) root         (0)     2905 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/roots/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     5092 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/run_config.py
+-rw-r--r--   0 root         (0) root         (0)     6523 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/runs.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/schedule_dry_run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:09:27.019996 dagster-graphql-1.7.3/dagster_graphql/schema/schedules/
+-rw-r--r--   0 root         (0) root         (0)     4945 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9135 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/schedules/schedules.py
+-rw-r--r--   0 root         (0) root         (0)     1833 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/schedules/ticks.py
+-rw-r--r--   0 root         (0) root         (0)     1312 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/sensor_dry_run.py
+-rw-r--r--   0 root         (0) root         (0)    10196 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/sensors.py
+-rw-r--r--   0 root         (0) root         (0)    30059 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/solids.py
+-rw-r--r--   0 root         (0) root         (0)     2390 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/table.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/tags.py
+-rw-r--r--   0 root         (0) root         (0)      574 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/test.py
+-rw-r--r--   0 root         (0) root         (0)      744 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/used_solid.py
+-rw-r--r--   0 root         (0) root         (0)      950 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/schema/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:09:27.019996 dagster-graphql-1.7.3/dagster_graphql/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7078 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/test/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/dagster_graphql/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:09:27.007995 dagster-graphql-1.7.3/dagster_graphql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      691 2024-04-25 20:09:26.000000 dagster-graphql-1.7.3/dagster_graphql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4726 2024-04-25 20:09:26.000000 dagster-graphql-1.7.3/dagster_graphql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 20:09:26.000000 dagster-graphql-1.7.3/dagster_graphql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2024-04-25 20:09:26.000000 dagster-graphql-1.7.3/dagster_graphql.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2024-04-25 20:09:26.000000 dagster-graphql-1.7.3/dagster_graphql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-25 20:09:26.000000 dagster-graphql-1.7.3/dagster_graphql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      180 2024-04-25 20:09:27.019996 dagster-graphql-1.7.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1531 2024-04-25 20:08:31.000000 dagster-graphql-1.7.3/setup.py
```

### Comparing `dagster-graphql-1.7.2rc4/LICENSE` & `dagster-graphql-1.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/PKG-INFO` & `dagster-graphql-1.7.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-graphql
-Version: 1.7.2rc4
+Version: 1.7.3
 Summary: The GraphQL frontend to python dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-graphql
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/__init__.py` & `dagster-graphql-1.7.3/dagster_graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/cli.py` & `dagster-graphql-1.7.3/dagster_graphql/cli.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/client/client.py` & `dagster-graphql-1.7.3/dagster_graphql/client/client.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/client/client_queries.py` & `dagster-graphql-1.7.3/dagster_graphql/client/client_queries.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/client/query.py` & `dagster-graphql-1.7.3/dagster_graphql/client/query.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/client/utils.py` & `dagster-graphql-1.7.3/dagster_graphql/client/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/implementation/asset_checks_loader.py` & `dagster-graphql-1.7.3/dagster_graphql/implementation/asset_checks_loader.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/implementation/events.py` & `dagster-graphql-1.7.3/dagster_graphql/implementation/events.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/implementation/execution/__init__.py` & `dagster-graphql-1.7.3/dagster_graphql/implementation/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/implementation/execution/backfill.py` & `dagster-graphql-1.7.3/dagster_graphql/implementation/execution/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/implementation/execution/dynamic_partitions.py` & `dagster-graphql-1.7.3/dagster_graphql/implementation/execution/dynamic_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/implementation/execution/launch_execution.py` & `dagster-graphql-1.7.3/dagster_graphql/implementation/execution/launch_execution.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/implementation/execution/run_lifecycle.py` & `dagster-graphql-1.7.3/dagster_graphql/implementation/execution/run_lifecycle.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/implementation/external.py` & `dagster-graphql-1.7.3/dagster_graphql/implementation/external.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/implementation/fetch_asset_checks.py` & `dagster-graphql-1.7.3/dagster_graphql/implementation/fetch_asset_checks.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/implementation/fetch_asset_condition_evaluations.py` & `dagster-graphql-1.7.3/dagster_graphql/implementation/fetch_asset_condition_evaluations.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/implementation/fetch_assets.py` & `dagster-graphql-1.7.3/dagster_graphql/implementation/fetch_assets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py` & `dagster-graphql-1.7.3/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/implementation/fetch_backfills.py` & `dagster-graphql-1.7.3/dagster_graphql/implementation/fetch_backfills.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/implementation/fetch_env_vars.py` & `dagster-graphql-1.7.3/dagster_graphql/implementation/fetch_env_vars.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/implementation/fetch_instigators.py` & `dagster-graphql-1.7.3/dagster_graphql/implementation/fetch_instigators.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/implementation/fetch_logs.py` & `dagster-graphql-1.7.3/dagster_graphql/implementation/fetch_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/implementation/fetch_partition_sets.py` & `dagster-graphql-1.7.3/dagster_graphql/implementation/fetch_partition_sets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/implementation/fetch_pipelines.py` & `dagster-graphql-1.7.3/dagster_graphql/implementation/fetch_pipelines.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/implementation/fetch_resources.py` & `dagster-graphql-1.7.3/dagster_graphql/implementation/fetch_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/implementation/fetch_runs.py` & `dagster-graphql-1.7.3/dagster_graphql/implementation/fetch_runs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/implementation/fetch_schedules.py` & `dagster-graphql-1.7.3/dagster_graphql/implementation/fetch_schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/implementation/fetch_sensors.py` & `dagster-graphql-1.7.3/dagster_graphql/implementation/fetch_sensors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/implementation/fetch_solids.py` & `dagster-graphql-1.7.3/dagster_graphql/implementation/fetch_solids.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/implementation/fetch_ticks.py` & `dagster-graphql-1.7.3/dagster_graphql/implementation/fetch_ticks.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/implementation/loader.py` & `dagster-graphql-1.7.3/dagster_graphql/implementation/loader.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/implementation/run_config_schema.py` & `dagster-graphql-1.7.3/dagster_graphql/implementation/run_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/implementation/telemetry.py` & `dagster-graphql-1.7.3/dagster_graphql/implementation/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/implementation/utils.py` & `dagster-graphql-1.7.3/dagster_graphql/implementation/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/__init__.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/asset_checks.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/asset_checks.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/asset_condition_evaluations.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/asset_condition_evaluations.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/asset_graph.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/asset_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -653,14 +653,33 @@
     ) -> Sequence[GrapheneObservationEvent]:
         try:
             before_timestamp = (
                 int(beforeTimestampMillis) / 1000.0 if beforeTimestampMillis else None
             )
         except ValueError:
             before_timestamp = None
+
+        if (
+            graphene_info.context.instance.event_log_storage.asset_records_have_last_observation
+            and self._asset_record_loader
+            and limit == 1
+            and not partitions
+            and not before_timestamp
+        ):
+            latest_observation_event = (
+                self._asset_record_loader.get_latest_observation_for_asset_key(
+                    self._external_asset_node.asset_key
+                )
+            )
+
+            if not latest_observation_event:
+                return []
+
+            return [GrapheneObservationEvent(event=latest_observation_event)]
+
         return [
             GrapheneObservationEvent(event=event)
             for event in get_asset_observations(
                 graphene_info,
                 self._external_asset_node.asset_key,
                 partitions,
                 before_timestamp=before_timestamp,
```

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/asset_selections.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/asset_selections.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,27 @@
+from typing import TYPE_CHECKING
+
 import graphene
 from dagster._core.definitions.asset_selection import AssetSelection
 from dagster._core.remote_representation.external import ExternalRepository
 
 from ..implementation.fetch_assets import get_asset_nodes_by_asset_key
+from ..implementation.utils import capture_error
 from .asset_key import GrapheneAssetKey
 from .util import non_null_list
 
+if TYPE_CHECKING:
+    from .roots.assets import GrapheneAssetConnection
+
 
 class GrapheneAssetSelection(graphene.ObjectType):
     assetSelectionString = graphene.String()
     assetKeys = non_null_list(GrapheneAssetKey)
     assets = non_null_list("dagster_graphql.schema.pipelines.pipeline.GrapheneAsset")
+    assetsOrError = graphene.NonNull("dagster_graphql.schema.roots.assets.GrapheneAssetsOrError")
 
     def __init__(self, asset_selection: AssetSelection, external_repository: ExternalRepository):
         self._asset_selection = asset_selection
         self._external_repository = external_repository
 
     def resolve_assetSelectionString(self, _graphene_info):
         return str(self._asset_selection)
@@ -22,20 +29,29 @@
     def resolve_assetKeys(self, _graphene_info):
         asset_graph = self._external_repository.asset_graph
         return [
             GrapheneAssetKey(path=asset_key.path)
             for asset_key in self._asset_selection.resolve(asset_graph)
         ]
 
-    def resolve_assets(self, graphene_info):
+    def _get_assets(self, graphene_info):
         from dagster_graphql.schema.pipelines.pipeline import GrapheneAsset
 
         asset_graph = self._external_repository.asset_graph
         asset_nodes_by_asset_key = get_asset_nodes_by_asset_key(graphene_info)
 
         return [
             GrapheneAsset(key=asset_key, definition=asset_nodes_by_asset_key.get(asset_key))
             for asset_key in self._asset_selection.resolve(asset_graph)
         ]
 
+    def resolve_assets(self, graphene_info):
+        return self._get_assets(graphene_info)
+
+    @capture_error
+    def resolve_assetsOrError(self, graphene_info) -> "GrapheneAssetConnection":
+        from .roots.assets import GrapheneAssetConnection
+
+        return GrapheneAssetConnection(nodes=self._get_assets(graphene_info))
+
     class Meta:
         name = "AssetSelection"
```

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/auto_materialize_asset_evaluations.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/auto_materialize_asset_evaluations.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/auto_materialize_policy.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/auto_materialize_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/backfill.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/config_type_or_error.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/config_type_or_error.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/config_types.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/config_types.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/dagster_types.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/dagster_types.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/env_vars.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/env_vars.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/errors.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/execution.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/execution.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/external.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/external.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/freshness_policy.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/freshness_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/inputs.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/inputs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/instance.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/instance.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from dagster._core.launcher.base import RunLauncher
 from dagster._core.storage.captured_log_manager import CapturedLogManager
 from dagster._core.storage.event_log.sql_event_log import SqlEventLogStorage
 from dagster._daemon.asset_daemon import get_auto_materialize_paused
 from dagster._daemon.types import DaemonStatus
 from dagster._utils.concurrency import (
     ClaimedSlotInfo,
-    ConcurrencyKeyInfo,
     PendingStepInfo,
     get_max_concurrency_limit_value,
 )
 
 from .errors import GraphenePythonError
 from .util import ResolveInfo, non_null_list
 
@@ -146,33 +145,60 @@
     pendingStepRunIds = non_null_list(graphene.String)
     assignedStepCount = graphene.NonNull(graphene.Int)
     assignedStepRunIds = non_null_list(graphene.String)
 
     class Meta:
         name = "ConcurrencyKeyInfo"
 
-    def __init__(self, concurrency_key_info: ConcurrencyKeyInfo):
-        self._claimed_slots = concurrency_key_info.claimed_slots
-        self._pending_steps = concurrency_key_info.pending_steps
-        super().__init__(
-            concurrencyKey=concurrency_key_info.concurrency_key,
-            slotCount=concurrency_key_info.slot_count,
-            activeSlotCount=concurrency_key_info.active_slot_count,
-            activeRunIds=list(concurrency_key_info.active_run_ids),
-            pendingStepCount=concurrency_key_info.pending_step_count,
-            pendingStepRunIds=list(concurrency_key_info.pending_run_ids),
-            assignedStepCount=concurrency_key_info.assigned_step_count,
-            assignedStepRunIds=list(concurrency_key_info.assigned_run_ids),
-        )
+    def __init__(self, concurrency_key: str):
+        self._concurrency_key = concurrency_key
+        self._concurrency_key_info = None
+        super().__init__(concurrencyKey=concurrency_key)
+
+    def _get_concurrency_key_info(self, graphene_info: ResolveInfo):
+        if not self._concurrency_key_info:
+            self._concurrency_key_info = (
+                graphene_info.context.instance.event_log_storage.get_concurrency_info(
+                    self._concurrency_key
+                )
+            )
+        return self._concurrency_key_info
+
+    def resolve_claimedSlots(self, graphene_info: ResolveInfo):
+        return [
+            GrapheneClaimedConcurrencySlot(slot)
+            for slot in self._get_concurrency_key_info(graphene_info).claimed_slots
+        ]
+
+    def resolve_pendingSteps(self, graphene_info: ResolveInfo):
+        return [
+            GraphenePendingConcurrencyStep(step)
+            for step in self._get_concurrency_key_info(graphene_info).pending_steps
+        ]
+
+    def resolve_slotCount(self, graphene_info: ResolveInfo):
+        return self._get_concurrency_key_info(graphene_info).slot_count
+
+    def resolve_activeSlotCount(self, graphene_info: ResolveInfo):
+        return self._get_concurrency_key_info(graphene_info).active_slot_count
+
+    def resolve_activeRunIds(self, graphene_info: ResolveInfo):
+        return list(self._get_concurrency_key_info(graphene_info).active_run_ids)
+
+    def resolve_pendingStepCount(self, graphene_info: ResolveInfo):
+        return self._get_concurrency_key_info(graphene_info).pending_step_count
+
+    def resolve_pendingStepRunIds(self, graphene_info: ResolveInfo):
+        return list(self._get_concurrency_key_info(graphene_info).pending_run_ids)
 
-    def resolve_claimedSlots(self, _graphene_info: ResolveInfo):
-        return [GrapheneClaimedConcurrencySlot(slot) for slot in self._claimed_slots]
+    def resolve_assignedStepCount(self, graphene_info: ResolveInfo):
+        return self._get_concurrency_key_info(graphene_info).assigned_step_count
 
-    def resolve_pendingSteps(self, _graphene_info: ResolveInfo):
-        return [GraphenePendingConcurrencyStep(step) for step in self._pending_steps]
+    def resolve_assignedStepRunIds(self, graphene_info: ResolveInfo):
+        return list(self._get_concurrency_key_info(graphene_info).assigned_run_ids)
 
 
 class GrapheneRunQueueConfig(graphene.ObjectType):
     maxConcurrentRuns = graphene.NonNull(graphene.Int)
     tagConcurrencyLimitsYaml = graphene.String()
     isOpConcurrencyAware = graphene.Boolean()
 
@@ -278,21 +304,19 @@
 
     def resolve_supportsConcurrencyLimits(self, _graphene_info: ResolveInfo):
         return self._instance.event_log_storage.supports_global_concurrency_limits
 
     def resolve_concurrencyLimits(self, _graphene_info: ResolveInfo):
         res = []
         for key in self._instance.event_log_storage.get_concurrency_keys():
-            key_info = self._instance.event_log_storage.get_concurrency_info(key)
-            res.append(GrapheneConcurrencyKeyInfo(key_info))
+            res.append(GrapheneConcurrencyKeyInfo(key))
         return res
 
     def resolve_concurrencyLimit(self, _graphene_info: ResolveInfo, concurrencyKey):
-        key_info = self._instance.event_log_storage.get_concurrency_info(concurrencyKey)
-        return GrapheneConcurrencyKeyInfo(key_info)
+        return GrapheneConcurrencyKeyInfo(concurrencyKey)
 
     def resolve_minConcurrencyLimitValue(self, _graphene_info: ResolveInfo):
         if isinstance(
             self._instance.event_log_storage, SqlEventLogStorage
         ) and not self._instance.event_log_storage.has_table("concurrency_limits"):
             return 1
         return 0
```

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/instigation.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/instigation.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/logs/__init__.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/logs/compute_logs.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/logs/compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/logs/events.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/logs/events.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/logs/log_level.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/logs/log_level.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/metadata.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/metadata.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/partition_mappings.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/partition_mappings.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/partition_sets.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/partition_sets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/permissions.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/permissions.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/pipelines/__init__.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/pipelines/config.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/pipelines/config.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/pipelines/config_result.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/pipelines/config_result.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/pipelines/logger.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/pipelines/logger.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/pipelines/mode.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/pipelines/mode.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/pipelines/pipeline.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/pipelines/pipeline_ref.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/pipelines/pipeline_ref.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/pipelines/pipeline_run_stats.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/pipelines/pipeline_run_stats.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/pipelines/resource.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/pipelines/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/pipelines/snapshot.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/pipelines/snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/pipelines/status.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/pipelines/status.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/pipelines/subscription.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/pipelines/subscription.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/repository_origin.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/repository_origin.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/resources.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/roots/__init__.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/roots/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/roots/assets.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/roots/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/roots/execution_plan.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/roots/execution_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/roots/mutation.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/roots/mutation.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/roots/pipeline.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/roots/pipeline.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/roots/query.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/roots/query.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/roots/subscription.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/roots/subscription.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/run_config.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/runs.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/runs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/schedule_dry_run.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/schedule_dry_run.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/schedules/__init__.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/schedules/schedules.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/schedules/schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/schedules/ticks.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/schedules/ticks.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/sensor_dry_run.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/sensor_dry_run.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/sensors.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/sensors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/solids.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/solids.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/table.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/table.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/tags.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/test.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/test.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/used_solid.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/used_solid.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/schema/util.py` & `dagster-graphql-1.7.3/dagster_graphql/schema/util.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql/test/utils.py` & `dagster-graphql-1.7.3/dagster_graphql/test/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql.egg-info/PKG-INFO` & `dagster-graphql-1.7.3/dagster_graphql.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-graphql
-Version: 1.7.2rc4
+Version: 1.7.3
 Summary: The GraphQL frontend to python dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-graphql
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-graphql-1.7.2rc4/dagster_graphql.egg-info/SOURCES.txt` & `dagster-graphql-1.7.3/dagster_graphql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc4/setup.py` & `dagster-graphql-1.7.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_graphql_tests*"]),
     include_package_data=True,
     python_requires=">=3.8,<3.13",
     install_requires=[
-        "dagster==1.7.2rc4",
+        "dagster==1.7.3",
         "graphene>=3,<4",
         "gql[requests]>=3,<4",
         "requests",
         "starlette",  # used for run_in_threadpool utility fn
     ],
     entry_points={"console_scripts": ["dagster-graphql = dagster_graphql.cli:main"]},
 )
```

