# Comparing `tmp/hsfs-3.7.2.tar.gz` & `tmp/hsfs-3.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsfs-3.7.2.tar", last modified: Mon Apr 15 10:29:30 2024, max compression
+gzip compressed data, was "hsfs-3.7.3.tar", last modified: Thu Apr 25 17:32:47 2024, max compression
```

## Comparing `hsfs-3.7.2.tar` & `hsfs-3.7.3.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0     1006     1006        0 2024-04-15 10:29:30.384649 hsfs-3.7.2/
--rw-r--r--   0     1006     1006       40 2024-01-11 15:40:27.000000 hsfs-3.7.2/MANIFEST.in
--rw-r--r--   0     1006     1006     8377 2024-04-15 10:29:30.384649 hsfs-3.7.2/PKG-INFO
--rw-r--r--   0     1006     1006     5950 2024-04-15 10:29:29.000000 hsfs-3.7.2/README.md
-drwxr-xr-x   0     1006     1006        0 2024-04-15 10:29:30.344649 hsfs-3.7.2/hsfs/
--rw-r--r--   0     1006     1006     1421 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/__init__.py
-drwxr-xr-x   0     1006     1006        0 2024-04-15 10:29:30.348649 hsfs-3.7.2/hsfs/client/
--rw-r--r--   0     1006     1006     1694 2024-01-11 15:40:27.000000 hsfs-3.7.2/hsfs/client/__init__.py
--rw-r--r--   0     1006     1006     1401 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/client/auth.py
--rw-r--r--   0     1006     1006     9570 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/client/base.py
--rw-r--r--   0     1006     1006     3028 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/client/exceptions.py
--rw-r--r--   0     1006     1006    13155 2024-04-15 10:29:25.000000 hsfs-3.7.2/hsfs/client/external.py
--rw-r--r--   0     1006     1006     6207 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/client/hopsworks.py
--rw-r--r--   0     1006     1006    15180 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/client/online_store_rest_client.py
--rw-r--r--   0     1006     1006     1554 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/code.py
--rw-r--r--   0     1006     1006    14393 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/connection.py
-drwxr-xr-x   0     1006     1006        0 2024-04-15 10:29:30.348649 hsfs-3.7.2/hsfs/constructor/
--rw-r--r--   0     1006     1006      605 2024-01-11 15:40:27.000000 hsfs-3.7.2/hsfs/constructor/__init__.py
--rw-r--r--   0     1006     1006     1497 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/constructor/external_feature_group_alias.py
--rw-r--r--   0     1006     1006     5612 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/constructor/filter.py
--rw-r--r--   0     1006     1006     3635 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/constructor/fs_query.py
--rw-r--r--   0     1006     1006     1749 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/constructor/hudi_feature_group_alias.py
--rw-r--r--   0     1006     1006     2161 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/constructor/join.py
--rw-r--r--   0     1006     1006     1587 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/constructor/prepared_statement_parameter.py
--rw-r--r--   0     1006     1006    29539 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/constructor/query.py
--rw-r--r--   0     1006     1006     3349 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/constructor/serving_prepared_statement.py
-drwxr-xr-x   0     1006     1006        0 2024-04-15 10:29:30.380649 hsfs-3.7.2/hsfs/core/
--rw-r--r--   0     1006     1006      605 2024-01-11 15:40:27.000000 hsfs-3.7.2/hsfs/core/__init__.py
--rw-r--r--   0     1006     1006    15490 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/arrow_flight_client.py
--rw-r--r--   0     1006     1006     4156 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/builtin_transformation_function.py
--rw-r--r--   0     1006     1006     1853 2024-01-11 15:40:27.000000 hsfs-3.7.2/hsfs/core/code_api.py
--rw-r--r--   0     1006     1006     2032 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/code_engine.py
--rw-r--r--   0     1006     1006     3629 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/dataset_api.py
--rw-r--r--   0     1006     1006     7809 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/delta_engine.py
--rw-r--r--   0     1006     1006     1040 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/deltastreamer_jobconf.py
--rw-r--r--   0     1006     1006     1627 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/execution.py
--rw-r--r--   0     1006     1006     5396 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/expectation_api.py
--rw-r--r--   0     1006     1006     2632 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/expectation_engine.py
--rw-r--r--   0     1006     1006     6356 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/expectation_suite_api.py
--rw-r--r--   0     1006     1006     4060 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/expectation_suite_engine.py
--rw-r--r--   0     1006     1006     9810 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/explicit_provenance.py
--rw-r--r--   0     1006     1006     6198 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/external_feature_group_engine.py
--rw-r--r--   0     1006     1006    11207 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/feature_descriptive_statistics.py
--rw-r--r--   0     1006     1006    13837 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/feature_group_api.py
--rw-r--r--   0     1006     1006     6663 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/feature_group_base_engine.py
--rw-r--r--   0     1006     1006    14833 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/feature_group_engine.py
--rw-r--r--   0     1006     1006    34734 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/feature_monitoring_config.py
--rw-r--r--   0     1006     1006    10497 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/feature_monitoring_config_api.py
--rw-r--r--   0     1006     1006    21382 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/feature_monitoring_config_engine.py
--rw-r--r--   0     1006     1006     7864 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/feature_monitoring_result.py
--rw-r--r--   0     1006     1006     5921 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/feature_monitoring_result_api.py
--rw-r--r--   0     1006     1006    24868 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/feature_monitoring_result_engine.py
--rw-r--r--   0     1006     1006     1238 2024-01-11 15:40:27.000000 hsfs-3.7.2/hsfs/core/feature_store_api.py
--rw-r--r--   0     1006     1006    10499 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/feature_view_api.py
--rw-r--r--   0     1006     1006    32376 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/feature_view_engine.py
--rw-r--r--   0     1006     1006     5023 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/great_expectation_engine.py
--rw-r--r--   0     1006     1006      828 2024-01-11 15:40:27.000000 hsfs-3.7.2/hsfs/core/hosts_api.py
--rw-r--r--   0     1006     1006    11737 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/hudi_engine.py
--rw-r--r--   0     1006     1006     1229 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/ingestion_job.py
--rw-r--r--   0     1006     1006     2262 2024-01-11 15:40:27.000000 hsfs-3.7.2/hsfs/core/ingestion_job_conf.py
--rw-r--r--   0     1006     1006     1087 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/inode.py
--rw-r--r--   0     1006     1006     8626 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/job.py
--rw-r--r--   0     1006     1006     2814 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/job_api.py
--rw-r--r--   0     1006     1006     2065 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/job_configuration.py
--rw-r--r--   0     1006     1006     3079 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/job_schedule.py
--rw-r--r--   0     1006     1006     1205 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/kafka_api.py
--rw-r--r--   0     1006     1006    11557 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/monitoring_window_config.py
--rw-r--r--   0     1006     1006    17012 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/monitoring_window_config_engine.py
--rw-r--r--   0     1006     1006     8709 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/online_store_rest_client_api.py
--rw-r--r--   0     1006     1006    32516 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/online_store_rest_client_engine.py
--rw-r--r--   0     1006     1006     3090 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/opensearch.py
--rw-r--r--   0     1006     1006     4419 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/opensearch_api.py
--rw-r--r--   0     1006     1006      898 2024-01-11 15:40:27.000000 hsfs-3.7.2/hsfs/core/project_api.py
--rw-r--r--   0     1006     1006     1093 2024-01-11 15:40:27.000000 hsfs-3.7.2/hsfs/core/query_constructor_api.py
--rw-r--r--   0     1006     1006      875 2024-01-11 15:40:27.000000 hsfs-3.7.2/hsfs/core/services_api.py
--rw-r--r--   0     1006     1006     1981 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/spine_group_engine.py
--rw-r--r--   0     1006     1006    12655 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/statistics_api.py
--rw-r--r--   0     1006     1006    20903 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/statistics_engine.py
--rw-r--r--   0     1006     1006     3072 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/storage_connector_api.py
--rw-r--r--   0     1006     1006     4696 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/tags_api.py
--rw-r--r--   0     1006     1006     6685 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/training_dataset_api.py
--rw-r--r--   0     1006     1006     6210 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/training_dataset_engine.py
--rw-r--r--   0     1006     1006     2148 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/training_dataset_job_conf.py
--rw-r--r--   0     1006     1006     4161 2024-01-11 15:40:27.000000 hsfs-3.7.2/hsfs/core/transformation_function_api.py
--rw-r--r--   0     1006     1006    12712 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/transformation_function_engine.py
--rw-r--r--   0     1006     1006     4773 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/validation_report_api.py
--rw-r--r--   0     1006     1006     3640 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/validation_report_engine.py
--rw-r--r--   0     1006     1006     2158 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/validation_result_api.py
--rw-r--r--   0     1006     1006     5469 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/validation_result_engine.py
--rw-r--r--   0     1006     1006     2297 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/variable_api.py
--rw-r--r--   0     1006     1006    11843 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/vector_db_client.py
--rwxr-xr-x   0     1006     1006    41829 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/core/vector_server.py
--rw-r--r--   0     1006     1006     1655 2024-01-11 15:40:27.000000 hsfs-3.7.2/hsfs/decorators.py
--rw-r--r--   0     1006     1006     5552 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/embedding.py
-drwxr-xr-x   0     1006     1006        0 2024-04-15 10:29:30.380649 hsfs-3.7.2/hsfs/engine/
--rw-r--r--   0     1006     1006     2486 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/engine/__init__.py
--rw-r--r--   0     1006     1006    53717 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/engine/python.py
--rw-r--r--   0     1006     1006    47336 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/engine/spark.py
--rw-r--r--   0     1006     1006     1118 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/engine/spark_no_metastore.py
--rw-r--r--   0     1006     1006    23612 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/expectation_suite.py
--rw-r--r--   0     1006     1006     6960 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/feature.py
--rw-r--r--   0     1006     1006   156932 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/feature_group.py
--rw-r--r--   0     1006     1006     3955 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/feature_group_commit.py
--rw-r--r--   0     1006     1006     1992 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/feature_group_writer.py
--rw-r--r--   0     1006     1006    78556 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/feature_store.py
--rw-r--r--   0     1006     1006   163846 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/feature_view.py
--rw-r--r--   0     1006     1006     4822 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/ge_expectation.py
--rw-r--r--   0     1006     1006     8651 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/ge_validation_result.py
--rw-r--r--   0     1006     1006     3456 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/serving_key.py
--rw-r--r--   0     1006     1006     2081 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/split_statistics.py
--rw-r--r--   0     1006     1006     8298 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/statistics.py
--rw-r--r--   0     1006     1006     3331 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/statistics_config.py
--rw-r--r--   0     1006     1006    49738 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/storage_connector.py
--rw-r--r--   0     1006     1006     1868 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/tag.py
--rw-r--r--   0     1006     1006    39576 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/training_dataset.py
--rw-r--r--   0     1006     1006     4836 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/training_dataset_feature.py
--rw-r--r--   0     1006     1006     2816 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/training_dataset_split.py
--rw-r--r--   0     1006     1006     8947 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/transformation_function.py
--rw-r--r--   0     1006     1006     2197 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/transformation_function_attached.py
--rw-r--r--   0     1006     1006     7760 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/usage.py
--rw-r--r--   0     1006     1006     3323 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/user.py
--rw-r--r--   0     1006     1006    15871 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/util.py
--rw-r--r--   0     1006     1006     7537 2024-04-11 18:09:58.000000 hsfs-3.7.2/hsfs/validation_report.py
--rw-r--r--   0     1006     1006      628 2024-04-15 10:29:25.000000 hsfs-3.7.2/hsfs/version.py
-drwxr-xr-x   0     1006     1006        0 2024-04-15 10:29:30.344649 hsfs-3.7.2/hsfs.egg-info/
--rw-r--r--   0     1006     1006     8377 2024-04-15 10:29:30.000000 hsfs-3.7.2/hsfs.egg-info/PKG-INFO
--rw-r--r--   0     1006     1006     3650 2024-04-15 10:29:30.000000 hsfs-3.7.2/hsfs.egg-info/SOURCES.txt
--rw-r--r--   0     1006     1006        1 2024-04-15 10:29:30.000000 hsfs-3.7.2/hsfs.egg-info/dependency_links.txt
--rw-r--r--   0     1006     1006      892 2024-04-15 10:29:30.000000 hsfs-3.7.2/hsfs.egg-info/requires.txt
--rw-r--r--   0     1006     1006        5 2024-04-15 10:29:30.000000 hsfs-3.7.2/hsfs.egg-info/top_level.txt
--rw-r--r--   0     1006     1006       38 2024-04-15 10:29:30.384649 hsfs-3.7.2/setup.cfg
--rw-r--r--   0     1006     1006     3310 2024-04-11 18:09:58.000000 hsfs-3.7.2/setup.py
-drwxr-xr-x   0     1006     1006        0 2024-04-15 10:29:30.380649 hsfs-3.7.2/tests/
--rw-r--r--   0     1006     1006      605 2024-01-11 15:40:27.000000 hsfs-3.7.2/tests/__init__.py
--rw-r--r--   0     1006     1006    34202 2024-04-11 18:09:58.000000 hsfs-3.7.2/tests/test_storage_connector.py
+drwxr-xr-x   0     1006     1006        0 2024-04-25 17:32:47.847803 hsfs-3.7.3/
+-rw-r--r--   0     1006     1006       40 2024-01-11 15:40:27.000000 hsfs-3.7.3/MANIFEST.in
+-rw-r--r--   0     1006     1006     8377 2024-04-25 17:32:47.843803 hsfs-3.7.3/PKG-INFO
+-rw-r--r--   0     1006     1006     5950 2024-04-25 17:32:46.000000 hsfs-3.7.3/README.md
+drwxr-xr-x   0     1006     1006        0 2024-04-25 17:32:47.803803 hsfs-3.7.3/hsfs/
+-rw-r--r--   0     1006     1006     1421 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/__init__.py
+drwxr-xr-x   0     1006     1006        0 2024-04-25 17:32:47.807803 hsfs-3.7.3/hsfs/client/
+-rw-r--r--   0     1006     1006     1694 2024-01-11 15:40:27.000000 hsfs-3.7.3/hsfs/client/__init__.py
+-rw-r--r--   0     1006     1006     1401 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/client/auth.py
+-rw-r--r--   0     1006     1006     9570 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/client/base.py
+-rw-r--r--   0     1006     1006     3028 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/client/exceptions.py
+-rw-r--r--   0     1006     1006    13155 2024-04-15 10:29:25.000000 hsfs-3.7.3/hsfs/client/external.py
+-rw-r--r--   0     1006     1006     6207 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/client/hopsworks.py
+-rw-r--r--   0     1006     1006    15180 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/client/online_store_rest_client.py
+-rw-r--r--   0     1006     1006     1554 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/code.py
+-rw-r--r--   0     1006     1006    14393 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/connection.py
+drwxr-xr-x   0     1006     1006        0 2024-04-25 17:32:47.811803 hsfs-3.7.3/hsfs/constructor/
+-rw-r--r--   0     1006     1006      605 2024-01-11 15:40:27.000000 hsfs-3.7.3/hsfs/constructor/__init__.py
+-rw-r--r--   0     1006     1006     1497 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/constructor/external_feature_group_alias.py
+-rw-r--r--   0     1006     1006     5612 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/constructor/filter.py
+-rw-r--r--   0     1006     1006     3635 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/constructor/fs_query.py
+-rw-r--r--   0     1006     1006     1749 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/constructor/hudi_feature_group_alias.py
+-rw-r--r--   0     1006     1006     2161 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/constructor/join.py
+-rw-r--r--   0     1006     1006     1587 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/constructor/prepared_statement_parameter.py
+-rw-r--r--   0     1006     1006    29539 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/constructor/query.py
+-rw-r--r--   0     1006     1006     3349 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/constructor/serving_prepared_statement.py
+drwxr-xr-x   0     1006     1006        0 2024-04-25 17:32:47.843803 hsfs-3.7.3/hsfs/core/
+-rw-r--r--   0     1006     1006      605 2024-01-11 15:40:27.000000 hsfs-3.7.3/hsfs/core/__init__.py
+-rw-r--r--   0     1006     1006    15490 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/arrow_flight_client.py
+-rw-r--r--   0     1006     1006     4156 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/builtin_transformation_function.py
+-rw-r--r--   0     1006     1006     1853 2024-01-11 15:40:27.000000 hsfs-3.7.3/hsfs/core/code_api.py
+-rw-r--r--   0     1006     1006     2032 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/code_engine.py
+-rw-r--r--   0     1006     1006     3629 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/dataset_api.py
+-rw-r--r--   0     1006     1006     7809 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/delta_engine.py
+-rw-r--r--   0     1006     1006     1040 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/deltastreamer_jobconf.py
+-rw-r--r--   0     1006     1006     1627 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/execution.py
+-rw-r--r--   0     1006     1006     5396 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/expectation_api.py
+-rw-r--r--   0     1006     1006     2632 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/expectation_engine.py
+-rw-r--r--   0     1006     1006     6356 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/expectation_suite_api.py
+-rw-r--r--   0     1006     1006     4060 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/expectation_suite_engine.py
+-rw-r--r--   0     1006     1006     9810 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/explicit_provenance.py
+-rw-r--r--   0     1006     1006     6198 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/external_feature_group_engine.py
+-rw-r--r--   0     1006     1006    11207 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/feature_descriptive_statistics.py
+-rw-r--r--   0     1006     1006    13837 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/feature_group_api.py
+-rw-r--r--   0     1006     1006     6663 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/feature_group_base_engine.py
+-rw-r--r--   0     1006     1006    14833 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/feature_group_engine.py
+-rw-r--r--   0     1006     1006    34734 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/feature_monitoring_config.py
+-rw-r--r--   0     1006     1006    10497 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/feature_monitoring_config_api.py
+-rw-r--r--   0     1006     1006    21382 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/feature_monitoring_config_engine.py
+-rw-r--r--   0     1006     1006     7864 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/feature_monitoring_result.py
+-rw-r--r--   0     1006     1006     5921 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/feature_monitoring_result_api.py
+-rw-r--r--   0     1006     1006    24868 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/feature_monitoring_result_engine.py
+-rw-r--r--   0     1006     1006     1238 2024-01-11 15:40:27.000000 hsfs-3.7.3/hsfs/core/feature_store_api.py
+-rw-r--r--   0     1006     1006    10499 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/feature_view_api.py
+-rw-r--r--   0     1006     1006    32376 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/feature_view_engine.py
+-rw-r--r--   0     1006     1006     5023 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/great_expectation_engine.py
+-rw-r--r--   0     1006     1006      828 2024-01-11 15:40:27.000000 hsfs-3.7.3/hsfs/core/hosts_api.py
+-rw-r--r--   0     1006     1006    11737 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/hudi_engine.py
+-rw-r--r--   0     1006     1006     1229 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/ingestion_job.py
+-rw-r--r--   0     1006     1006     2262 2024-01-11 15:40:27.000000 hsfs-3.7.3/hsfs/core/ingestion_job_conf.py
+-rw-r--r--   0     1006     1006     1087 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/inode.py
+-rw-r--r--   0     1006     1006     8626 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/job.py
+-rw-r--r--   0     1006     1006     2814 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/job_api.py
+-rw-r--r--   0     1006     1006     2065 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/job_configuration.py
+-rw-r--r--   0     1006     1006     3079 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/job_schedule.py
+-rw-r--r--   0     1006     1006     1205 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/kafka_api.py
+-rw-r--r--   0     1006     1006    11557 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/monitoring_window_config.py
+-rw-r--r--   0     1006     1006    17012 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/monitoring_window_config_engine.py
+-rw-r--r--   0     1006     1006     8709 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/online_store_rest_client_api.py
+-rw-r--r--   0     1006     1006    32516 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/online_store_rest_client_engine.py
+-rw-r--r--   0     1006     1006     3090 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/opensearch.py
+-rw-r--r--   0     1006     1006     4419 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/opensearch_api.py
+-rw-r--r--   0     1006     1006      898 2024-01-11 15:40:27.000000 hsfs-3.7.3/hsfs/core/project_api.py
+-rw-r--r--   0     1006     1006     1093 2024-01-11 15:40:27.000000 hsfs-3.7.3/hsfs/core/query_constructor_api.py
+-rw-r--r--   0     1006     1006      875 2024-01-11 15:40:27.000000 hsfs-3.7.3/hsfs/core/services_api.py
+-rw-r--r--   0     1006     1006     1981 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/spine_group_engine.py
+-rw-r--r--   0     1006     1006    12655 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/statistics_api.py
+-rw-r--r--   0     1006     1006    20903 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/statistics_engine.py
+-rw-r--r--   0     1006     1006     3072 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/storage_connector_api.py
+-rw-r--r--   0     1006     1006     4696 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/tags_api.py
+-rw-r--r--   0     1006     1006     6685 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/training_dataset_api.py
+-rw-r--r--   0     1006     1006     6210 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/training_dataset_engine.py
+-rw-r--r--   0     1006     1006     2148 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/training_dataset_job_conf.py
+-rw-r--r--   0     1006     1006     4161 2024-01-11 15:40:27.000000 hsfs-3.7.3/hsfs/core/transformation_function_api.py
+-rw-r--r--   0     1006     1006    12712 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/transformation_function_engine.py
+-rw-r--r--   0     1006     1006     4773 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/validation_report_api.py
+-rw-r--r--   0     1006     1006     3640 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/validation_report_engine.py
+-rw-r--r--   0     1006     1006     2158 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/validation_result_api.py
+-rw-r--r--   0     1006     1006     5469 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/validation_result_engine.py
+-rw-r--r--   0     1006     1006     2297 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/variable_api.py
+-rw-r--r--   0     1006     1006    11843 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/vector_db_client.py
+-rwxr-xr-x   0     1006     1006    41829 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/core/vector_server.py
+-rw-r--r--   0     1006     1006     1655 2024-01-11 15:40:27.000000 hsfs-3.7.3/hsfs/decorators.py
+-rw-r--r--   0     1006     1006     5552 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/embedding.py
+drwxr-xr-x   0     1006     1006        0 2024-04-25 17:32:47.843803 hsfs-3.7.3/hsfs/engine/
+-rw-r--r--   0     1006     1006     2486 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/engine/__init__.py
+-rw-r--r--   0     1006     1006    53838 2024-04-25 17:32:42.000000 hsfs-3.7.3/hsfs/engine/python.py
+-rw-r--r--   0     1006     1006    47336 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/engine/spark.py
+-rw-r--r--   0     1006     1006     1118 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/engine/spark_no_metastore.py
+-rw-r--r--   0     1006     1006    23612 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/expectation_suite.py
+-rw-r--r--   0     1006     1006     6960 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/feature.py
+-rw-r--r--   0     1006     1006   156932 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/feature_group.py
+-rw-r--r--   0     1006     1006     3955 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/feature_group_commit.py
+-rw-r--r--   0     1006     1006     1992 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/feature_group_writer.py
+-rw-r--r--   0     1006     1006    78556 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/feature_store.py
+-rw-r--r--   0     1006     1006   163846 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/feature_view.py
+-rw-r--r--   0     1006     1006     4822 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/ge_expectation.py
+-rw-r--r--   0     1006     1006     8651 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/ge_validation_result.py
+-rw-r--r--   0     1006     1006     3456 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/serving_key.py
+-rw-r--r--   0     1006     1006     2081 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/split_statistics.py
+-rw-r--r--   0     1006     1006     8298 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/statistics.py
+-rw-r--r--   0     1006     1006     3331 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/statistics_config.py
+-rw-r--r--   0     1006     1006    49738 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/storage_connector.py
+-rw-r--r--   0     1006     1006     1868 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/tag.py
+-rw-r--r--   0     1006     1006    39576 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/training_dataset.py
+-rw-r--r--   0     1006     1006     4836 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/training_dataset_feature.py
+-rw-r--r--   0     1006     1006     2816 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/training_dataset_split.py
+-rw-r--r--   0     1006     1006     8947 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/transformation_function.py
+-rw-r--r--   0     1006     1006     2197 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/transformation_function_attached.py
+-rw-r--r--   0     1006     1006     7760 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/usage.py
+-rw-r--r--   0     1006     1006     3323 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/user.py
+-rw-r--r--   0     1006     1006    15871 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/util.py
+-rw-r--r--   0     1006     1006     7537 2024-04-11 18:09:58.000000 hsfs-3.7.3/hsfs/validation_report.py
+-rw-r--r--   0     1006     1006      628 2024-04-25 17:32:42.000000 hsfs-3.7.3/hsfs/version.py
+drwxr-xr-x   0     1006     1006        0 2024-04-25 17:32:47.803803 hsfs-3.7.3/hsfs.egg-info/
+-rw-r--r--   0     1006     1006     8377 2024-04-25 17:32:47.000000 hsfs-3.7.3/hsfs.egg-info/PKG-INFO
+-rw-r--r--   0     1006     1006     3650 2024-04-25 17:32:47.000000 hsfs-3.7.3/hsfs.egg-info/SOURCES.txt
+-rw-r--r--   0     1006     1006        1 2024-04-25 17:32:47.000000 hsfs-3.7.3/hsfs.egg-info/dependency_links.txt
+-rw-r--r--   0     1006     1006      892 2024-04-25 17:32:47.000000 hsfs-3.7.3/hsfs.egg-info/requires.txt
+-rw-r--r--   0     1006     1006        5 2024-04-25 17:32:47.000000 hsfs-3.7.3/hsfs.egg-info/top_level.txt
+-rw-r--r--   0     1006     1006       38 2024-04-25 17:32:47.847803 hsfs-3.7.3/setup.cfg
+-rw-r--r--   0     1006     1006     3310 2024-04-11 18:09:58.000000 hsfs-3.7.3/setup.py
+drwxr-xr-x   0     1006     1006        0 2024-04-25 17:32:47.843803 hsfs-3.7.3/tests/
+-rw-r--r--   0     1006     1006      605 2024-01-11 15:40:27.000000 hsfs-3.7.3/tests/__init__.py
+-rw-r--r--   0     1006     1006    34202 2024-04-11 18:09:58.000000 hsfs-3.7.3/tests/test_storage_connector.py
```

### Comparing `hsfs-3.7.2/PKG-INFO` & `hsfs-3.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hsfs
-Version: 3.7.2
+Version: 3.7.3
 Summary: HSFS: An environment independent client to interact with the Hopsworks Featurestore
 Home-page: https://github.com/logicalclocks/feature-store-api
 Author: Hopsworks AB
 Author-email: moritz@logicalclocks.com
 License: Apache License 2.0
-Download-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.7.2
+Download-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.7.3
 Description: # Hopsworks Feature Store
         
         <p align="center">
           <a href="https://community.hopsworks.ai"><img
             src="https://img.shields.io/discourse/users?label=Hopsworks%20Community&server=https%3A%2F%2Fcommunity.hopsworks.ai"
             alt="Hopsworks Community"
           /></a>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: hsfs Version: 3.7.2 Summary: HSFS: An environment
+Metadata-Version: 2.1 Name: hsfs Version: 3.7.3 Summary: HSFS: An environment
 independent client to interact with the Hopsworks Featurestore Home-page:
 https://github.com/logicalclocks/feature-store-api Author: Hopsworks AB Author-
 email: moritz@logicalclocks.com License: Apache License 2.0 Download-URL:
-https://github.com/logicalclocks/feature-store-api/releases/tag/3.7.2
+https://github.com/logicalclocks/feature-store-api/releases/tag/3.7.3
 Description: # Hopsworks Feature Store
 _[_H_o_p_s_w_o_r_k_s_ _C_o_m_m_u_n_i_t_y_]_[_H_o_p_s_w_o_r_k_s_ _F_e_a_t_u_r_e_ _S_t_o_r_e_ _D_o_c_u_m_e_n_t_a_t_i_o_n_]_[_P_y_P_i_S_t_a_t_u_s_]_[_S_c_a_l_a_/
                 _J_a_v_a_ _A_r_t_i_f_a_c_t_s_]_[_D_o_w_n_l_o_a_d_s_]_[_C_o_d_e_S_t_y_l_e_][License]
 HSFS is the library to interact with the Hopsworks Feature Store. The library
 makes creating new features, feature groups and training datasets easy. The
 library is environment independent and can be used in two modes: - Spark mode:
 For data engineering jobs that create and write features into the feature store
```

### Comparing `hsfs-3.7.2/README.md` & `hsfs-3.7.3/README.md`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/__init__.py` & `hsfs-3.7.3/hsfs/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/client/__init__.py` & `hsfs-3.7.3/hsfs/client/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/client/auth.py` & `hsfs-3.7.3/hsfs/client/auth.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/client/base.py` & `hsfs-3.7.3/hsfs/client/base.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/client/exceptions.py` & `hsfs-3.7.3/hsfs/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/client/external.py` & `hsfs-3.7.3/hsfs/client/external.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/client/hopsworks.py` & `hsfs-3.7.3/hsfs/client/hopsworks.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/client/online_store_rest_client.py` & `hsfs-3.7.3/hsfs/client/online_store_rest_client.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/code.py` & `hsfs-3.7.3/hsfs/code.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/connection.py` & `hsfs-3.7.3/hsfs/connection.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/constructor/__init__.py` & `hsfs-3.7.3/hsfs/constructor/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/constructor/external_feature_group_alias.py` & `hsfs-3.7.3/hsfs/constructor/external_feature_group_alias.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/constructor/filter.py` & `hsfs-3.7.3/hsfs/constructor/filter.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/constructor/fs_query.py` & `hsfs-3.7.3/hsfs/constructor/fs_query.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/constructor/hudi_feature_group_alias.py` & `hsfs-3.7.3/hsfs/constructor/hudi_feature_group_alias.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/constructor/join.py` & `hsfs-3.7.3/hsfs/constructor/join.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/constructor/prepared_statement_parameter.py` & `hsfs-3.7.3/hsfs/constructor/prepared_statement_parameter.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/constructor/query.py` & `hsfs-3.7.3/hsfs/constructor/query.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/constructor/serving_prepared_statement.py` & `hsfs-3.7.3/hsfs/constructor/serving_prepared_statement.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/__init__.py` & `hsfs-3.7.3/hsfs/core/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/arrow_flight_client.py` & `hsfs-3.7.3/hsfs/core/arrow_flight_client.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/builtin_transformation_function.py` & `hsfs-3.7.3/hsfs/core/builtin_transformation_function.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/code_api.py` & `hsfs-3.7.3/hsfs/core/code_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/code_engine.py` & `hsfs-3.7.3/hsfs/core/code_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/dataset_api.py` & `hsfs-3.7.3/hsfs/core/dataset_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/delta_engine.py` & `hsfs-3.7.3/hsfs/core/delta_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/deltastreamer_jobconf.py` & `hsfs-3.7.3/hsfs/core/deltastreamer_jobconf.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/execution.py` & `hsfs-3.7.3/hsfs/core/execution.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/expectation_api.py` & `hsfs-3.7.3/hsfs/core/expectation_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/expectation_engine.py` & `hsfs-3.7.3/hsfs/core/expectation_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/expectation_suite_api.py` & `hsfs-3.7.3/hsfs/core/expectation_suite_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/expectation_suite_engine.py` & `hsfs-3.7.3/hsfs/core/expectation_suite_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/explicit_provenance.py` & `hsfs-3.7.3/hsfs/core/explicit_provenance.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/external_feature_group_engine.py` & `hsfs-3.7.3/hsfs/core/external_feature_group_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/feature_descriptive_statistics.py` & `hsfs-3.7.3/hsfs/core/feature_descriptive_statistics.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/feature_group_api.py` & `hsfs-3.7.3/hsfs/core/feature_group_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/feature_group_base_engine.py` & `hsfs-3.7.3/hsfs/core/feature_group_base_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/feature_group_engine.py` & `hsfs-3.7.3/hsfs/core/feature_group_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/feature_monitoring_config.py` & `hsfs-3.7.3/hsfs/core/feature_monitoring_config.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/feature_monitoring_config_api.py` & `hsfs-3.7.3/hsfs/core/feature_monitoring_config_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/feature_monitoring_config_engine.py` & `hsfs-3.7.3/hsfs/core/feature_monitoring_config_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/feature_monitoring_result.py` & `hsfs-3.7.3/hsfs/core/feature_monitoring_result.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/feature_monitoring_result_api.py` & `hsfs-3.7.3/hsfs/core/feature_monitoring_result_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/feature_monitoring_result_engine.py` & `hsfs-3.7.3/hsfs/core/feature_monitoring_result_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/feature_store_api.py` & `hsfs-3.7.3/hsfs/core/feature_store_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/feature_view_api.py` & `hsfs-3.7.3/hsfs/core/feature_view_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/feature_view_engine.py` & `hsfs-3.7.3/hsfs/core/feature_view_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/great_expectation_engine.py` & `hsfs-3.7.3/hsfs/core/great_expectation_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/hosts_api.py` & `hsfs-3.7.3/hsfs/core/hosts_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/hudi_engine.py` & `hsfs-3.7.3/hsfs/core/hudi_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/ingestion_job.py` & `hsfs-3.7.3/hsfs/core/ingestion_job.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/ingestion_job_conf.py` & `hsfs-3.7.3/hsfs/core/ingestion_job_conf.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/inode.py` & `hsfs-3.7.3/hsfs/core/inode.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/job.py` & `hsfs-3.7.3/hsfs/core/job.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/job_api.py` & `hsfs-3.7.3/hsfs/core/job_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/job_configuration.py` & `hsfs-3.7.3/hsfs/core/job_configuration.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/job_schedule.py` & `hsfs-3.7.3/hsfs/core/job_schedule.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/kafka_api.py` & `hsfs-3.7.3/hsfs/core/kafka_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/monitoring_window_config.py` & `hsfs-3.7.3/hsfs/core/monitoring_window_config.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/monitoring_window_config_engine.py` & `hsfs-3.7.3/hsfs/core/monitoring_window_config_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/online_store_rest_client_api.py` & `hsfs-3.7.3/hsfs/core/online_store_rest_client_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/online_store_rest_client_engine.py` & `hsfs-3.7.3/hsfs/core/online_store_rest_client_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/opensearch.py` & `hsfs-3.7.3/hsfs/core/opensearch.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/opensearch_api.py` & `hsfs-3.7.3/hsfs/core/opensearch_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/project_api.py` & `hsfs-3.7.3/hsfs/core/project_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/query_constructor_api.py` & `hsfs-3.7.3/hsfs/core/query_constructor_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/services_api.py` & `hsfs-3.7.3/hsfs/core/services_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/spine_group_engine.py` & `hsfs-3.7.3/hsfs/core/spine_group_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/statistics_api.py` & `hsfs-3.7.3/hsfs/core/statistics_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/statistics_engine.py` & `hsfs-3.7.3/hsfs/core/statistics_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/storage_connector_api.py` & `hsfs-3.7.3/hsfs/core/storage_connector_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/tags_api.py` & `hsfs-3.7.3/hsfs/core/tags_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/training_dataset_api.py` & `hsfs-3.7.3/hsfs/core/training_dataset_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/training_dataset_engine.py` & `hsfs-3.7.3/hsfs/core/training_dataset_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/training_dataset_job_conf.py` & `hsfs-3.7.3/hsfs/core/training_dataset_job_conf.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/transformation_function_api.py` & `hsfs-3.7.3/hsfs/core/transformation_function_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/transformation_function_engine.py` & `hsfs-3.7.3/hsfs/core/transformation_function_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/validation_report_api.py` & `hsfs-3.7.3/hsfs/core/validation_report_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/validation_report_engine.py` & `hsfs-3.7.3/hsfs/core/validation_report_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/validation_result_api.py` & `hsfs-3.7.3/hsfs/core/validation_result_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/validation_result_engine.py` & `hsfs-3.7.3/hsfs/core/validation_result_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/variable_api.py` & `hsfs-3.7.3/hsfs/core/variable_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/vector_db_client.py` & `hsfs-3.7.3/hsfs/core/vector_db_client.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/core/vector_server.py` & `hsfs-3.7.3/hsfs/core/vector_server.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/decorators.py` & `hsfs-3.7.3/hsfs/decorators.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/embedding.py` & `hsfs-3.7.3/hsfs/embedding.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/engine/__init__.py` & `hsfs-3.7.3/hsfs/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/engine/python.py` & `hsfs-3.7.3/hsfs/engine/python.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 import decimal
 import numbers
 import math
 import os
 import sys
 import pytz
 from datetime import datetime, timezone
+from pathlib import Path
 
 import great_expectations as ge
 
 from io import BytesIO
 from pyhive import hive
 from typing import TypeVar, Optional, Dict, Any
 from confluent_kafka import Consumer, Producer, TopicPartition, KafkaError
@@ -235,28 +236,31 @@
         else:
             raise TypeError(
                 "{} training dataset format is not supported to read as pandas dataframe.".format(
                     data_format
                 )
             )
 
+    def _is_metadata_file(self, path):
+        return Path(path).stem.startswith("_")
+
     def _read_hopsfs(self, location, data_format, read_options={}):
         # providing more informative error
         try:
             from pydoop import hdfs
         except ModuleNotFoundError:
             return self._read_hopsfs_remote(location, data_format, read_options)
         util.setup_pydoop()
         path_list = hdfs.ls(location, recursive=True)
 
         df_list = []
         for path in path_list:
             if (
                 hdfs.path.isfile(path)
-                and not path.endswith("_SUCCESS")
+                and not self._is_metadata_file(path)
                 and hdfs.path.getsize(path) > 0
             ):
                 df_list.append(self._read_pandas(data_format, path))
         return df_list
 
     # This is a version of the read method that uses the Hopsworks REST APIs or Flyginduck Server
     # To read the training dataset content, this to avoid the pydoop dependency
@@ -268,15 +272,15 @@
 
         while offset < total_count:
             total_count, inode_list = self._dataset_api.list_files(
                 location, offset, 100
             )
 
             for inode in inode_list:
-                if not inode.path.endswith("_SUCCESS"):
+                if not self._is_metadata_file(inode.path):
                     if arrow_flight_client.get_instance().is_data_format_supported(
                         data_format, read_options
                     ):
                         arrow_flight_config = read_options.get("arrow_flight_config")
                         df = arrow_flight_client.get_instance().read_path(
                             inode.path, arrow_flight_config
                         )
@@ -326,15 +330,15 @@
                 object_list = s3.list_objects_v2(
                     Bucket=storage_connector.bucket,
                     Prefix=prefix,
                     MaxKeys=1000,
                 )
 
             for obj in object_list["Contents"]:
-                if not obj["Key"].endswith("_SUCCESS") and obj["Size"] > 0:
+                if not self._is_metadata_file(obj["Key"]) and obj["Size"] > 0:
                     obj = s3.get_object(
                         Bucket=storage_connector.bucket,
                         Key=obj["Key"],
                     )
                     df_list.append(self._read_pandas(data_format, obj["Body"]))
         return df_list
```

### Comparing `hsfs-3.7.2/hsfs/engine/spark.py` & `hsfs-3.7.3/hsfs/engine/spark.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/engine/spark_no_metastore.py` & `hsfs-3.7.3/hsfs/engine/spark_no_metastore.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/expectation_suite.py` & `hsfs-3.7.3/hsfs/expectation_suite.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/feature.py` & `hsfs-3.7.3/hsfs/feature.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/feature_group.py` & `hsfs-3.7.3/hsfs/feature_group.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/feature_group_commit.py` & `hsfs-3.7.3/hsfs/feature_group_commit.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/feature_group_writer.py` & `hsfs-3.7.3/hsfs/feature_group_writer.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/feature_store.py` & `hsfs-3.7.3/hsfs/feature_store.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/feature_view.py` & `hsfs-3.7.3/hsfs/feature_view.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/ge_expectation.py` & `hsfs-3.7.3/hsfs/ge_expectation.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/ge_validation_result.py` & `hsfs-3.7.3/hsfs/ge_validation_result.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/serving_key.py` & `hsfs-3.7.3/hsfs/serving_key.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/split_statistics.py` & `hsfs-3.7.3/hsfs/split_statistics.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/statistics.py` & `hsfs-3.7.3/hsfs/statistics.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/statistics_config.py` & `hsfs-3.7.3/hsfs/statistics_config.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/storage_connector.py` & `hsfs-3.7.3/hsfs/storage_connector.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/tag.py` & `hsfs-3.7.3/hsfs/tag.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/training_dataset.py` & `hsfs-3.7.3/hsfs/training_dataset.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/training_dataset_feature.py` & `hsfs-3.7.3/hsfs/training_dataset_feature.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/training_dataset_split.py` & `hsfs-3.7.3/hsfs/training_dataset_split.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/transformation_function.py` & `hsfs-3.7.3/hsfs/transformation_function.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/transformation_function_attached.py` & `hsfs-3.7.3/hsfs/transformation_function_attached.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/usage.py` & `hsfs-3.7.3/hsfs/usage.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/user.py` & `hsfs-3.7.3/hsfs/user.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/util.py` & `hsfs-3.7.3/hsfs/util.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/validation_report.py` & `hsfs-3.7.3/hsfs/validation_report.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs/version.py` & `hsfs-3.7.3/hsfs/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
-__version__ = "3.7.2"
+__version__ = "3.7.3"
```

### Comparing `hsfs-3.7.2/hsfs.egg-info/PKG-INFO` & `hsfs-3.7.3/hsfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hsfs
-Version: 3.7.2
+Version: 3.7.3
 Summary: HSFS: An environment independent client to interact with the Hopsworks Featurestore
 Home-page: https://github.com/logicalclocks/feature-store-api
 Author: Hopsworks AB
 Author-email: moritz@logicalclocks.com
 License: Apache License 2.0
-Download-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.7.2
+Download-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.7.3
 Description: # Hopsworks Feature Store
         
         <p align="center">
           <a href="https://community.hopsworks.ai"><img
             src="https://img.shields.io/discourse/users?label=Hopsworks%20Community&server=https%3A%2F%2Fcommunity.hopsworks.ai"
             alt="Hopsworks Community"
           /></a>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: hsfs Version: 3.7.2 Summary: HSFS: An environment
+Metadata-Version: 2.1 Name: hsfs Version: 3.7.3 Summary: HSFS: An environment
 independent client to interact with the Hopsworks Featurestore Home-page:
 https://github.com/logicalclocks/feature-store-api Author: Hopsworks AB Author-
 email: moritz@logicalclocks.com License: Apache License 2.0 Download-URL:
-https://github.com/logicalclocks/feature-store-api/releases/tag/3.7.2
+https://github.com/logicalclocks/feature-store-api/releases/tag/3.7.3
 Description: # Hopsworks Feature Store
 _[_H_o_p_s_w_o_r_k_s_ _C_o_m_m_u_n_i_t_y_]_[_H_o_p_s_w_o_r_k_s_ _F_e_a_t_u_r_e_ _S_t_o_r_e_ _D_o_c_u_m_e_n_t_a_t_i_o_n_]_[_P_y_P_i_S_t_a_t_u_s_]_[_S_c_a_l_a_/
                 _J_a_v_a_ _A_r_t_i_f_a_c_t_s_]_[_D_o_w_n_l_o_a_d_s_]_[_C_o_d_e_S_t_y_l_e_][License]
 HSFS is the library to interact with the Hopsworks Feature Store. The library
 makes creating new features, feature groups and training datasets easy. The
 library is environment independent and can be used in two modes: - Spark mode:
 For data engineering jobs that create and write features into the feature store
```

### Comparing `hsfs-3.7.2/hsfs.egg-info/SOURCES.txt` & `hsfs-3.7.3/hsfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/hsfs.egg-info/requires.txt` & `hsfs-3.7.3/hsfs.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/setup.py` & `hsfs-3.7.3/setup.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/tests/__init__.py` & `hsfs-3.7.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.2/tests/test_storage_connector.py` & `hsfs-3.7.3/tests/test_storage_connector.py`

 * *Files identical despite different names*

