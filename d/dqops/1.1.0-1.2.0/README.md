# Comparing `tmp/dqops-1.1.0.tar.gz` & `tmp/dqops-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dqops-1.1.0.tar", last modified: Sun Mar 24 19:56:52 2024, max compression
+gzip compressed data, was "dqops-1.2.0.tar", last modified: Thu Apr 25 12:11:50 2024, max compression
```

## Comparing `dqops-1.1.0.tar` & `dqops-1.2.0.tar`

### file list

```diff
@@ -1,1249 +1,1264 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 19:56:52.914817 dqops-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11353 2024-03-24 19:44:21.000000 dqops-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-03-24 19:56:52.914817 dqops-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9142 2024-03-24 19:44:21.000000 dqops-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 19:56:52.702816 dqops-1.1.0/dqops/
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 19:56:52.706816 dqops-1.1.0/dqops/client/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 19:56:52.706816 dqops-1.1.0/dqops/client/api/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 19:56:52.706816 dqops-1.1.0/dqops/client/api/check_results/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/check_results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11604 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/check_results/get_column_monitoring_checks_results.py
--rw-r--r--   0 runner    (1001) docker     (127)    11573 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/check_results/get_column_partitioned_checks_results.py
--rw-r--r--   0 runner    (1001) docker     (127)    11067 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/check_results/get_column_profiling_checks_results.py
--rw-r--r--   0 runner    (1001) docker     (127)    14194 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/check_results/get_table_data_quality_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    11225 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/check_results/get_table_monitoring_checks_results.py
--rw-r--r--   0 runner    (1001) docker     (127)    11150 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/check_results/get_table_partitioned_checks_results.py
--rw-r--r--   0 runner    (1001) docker     (127)    10680 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/check_results/get_table_profiling_checks_results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 19:56:52.710816 dqops-1.1.0/dqops/client/api/check_results_overview/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/check_results_overview/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/check_results_overview/get_column_monitoring_checks_overview.py
--rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/check_results_overview/get_column_partitioned_checks_overview.py
--rw-r--r--   0 runner    (1001) docker     (127)     7367 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/check_results_overview/get_column_profiling_checks_overview.py
--rw-r--r--   0 runner    (1001) docker     (127)     7489 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/check_results_overview/get_table_monitoring_checks_overview.py
--rw-r--r--   0 runner    (1001) docker     (127)     7454 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/check_results_overview/get_table_partitioned_checks_overview.py
--rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/check_results_overview/get_table_profiling_checks_overview.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 19:56:52.710816 dqops-1.1.0/dqops/client/api/checks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/checks/create_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/checks/delete_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/checks/get_all_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/checks/get_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/checks/get_check_folder_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/checks/update_check.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 19:56:52.718816 dqops-1.1.0/dqops/client/api/columns/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/columns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/columns/create_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/columns/delete_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/columns/get_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/columns/get_column_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5418 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/columns/get_column_comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/columns/get_column_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     6089 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/columns/get_column_monitoring_checks_basic_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5753 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/columns/get_column_monitoring_checks_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/columns/get_column_monitoring_checks_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/columns/get_column_monitoring_checks_model_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/columns/get_column_monitoring_checks_monthly.py
--rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/columns/get_column_partitioned_checks_basic_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/columns/get_column_partitioned_checks_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/columns/get_column_partitioned_checks_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7044 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/columns/get_column_partitioned_checks_model_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/columns/get_column_partitioned_checks_monthly.py
--rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/columns/get_column_profiling_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/columns/get_column_profiling_checks_basic_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/columns/get_column_profiling_checks_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6434 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/columns/get_column_profiling_checks_model_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/columns/get_column_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/columns/get_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/columns/get_columns_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/columns/update_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/columns/update_column_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/columns/update_column_comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/columns/update_column_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/columns/update_column_monitoring_checks_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/columns/update_column_monitoring_checks_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/columns/update_column_monitoring_checks_monthly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/columns/update_column_partitioned_checks_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/columns/update_column_partitioned_checks_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/columns/update_column_partitioned_checks_monthly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/columns/update_column_profiling_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/columns/update_column_profiling_checks_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 19:56:52.722816 dqops-1.1.0/dqops/client/api/connections/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/connections/bulk_activate_connection_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/connections/bulk_deactivate_connection_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/connections/create_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/connections/create_connection_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/connections/delete_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/connections/get_all_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/connections/get_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/connections/get_connection_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/connections/get_connection_comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/connections/get_connection_common_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/connections/get_connection_default_grouping_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/connections/get_connection_incident_grouping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/connections/get_connection_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/connections/get_connection_scheduling_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/connections/update_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/connections/update_connection_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/connections/update_connection_comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/connections/update_connection_default_grouping_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/connections/update_connection_incident_grouping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/connections/update_connection_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/connections/update_connection_scheduling_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 19:56:52.722816 dqops-1.1.0/dqops/client/api/dashboards/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/dashboards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/dashboards/get_all_dashboards.py
--rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/dashboards/get_dashboard_level_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/dashboards/get_dashboard_level_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/dashboards/get_dashboard_level_3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/dashboards/get_dashboard_level_4.py
--rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/dashboards/get_dashboard_level_5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 19:56:52.726816 dqops-1.1.0/dqops/client/api/data_grouping_configurations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/data_grouping_configurations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/data_grouping_configurations/create_table_grouping_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/data_grouping_configurations/delete_table_grouping_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/data_grouping_configurations/get_table_grouping_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/data_grouping_configurations/get_table_grouping_configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/data_grouping_configurations/set_table_default_grouping_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4220 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/data_grouping_configurations/update_table_grouping_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 19:56:52.726816 dqops-1.1.0/dqops/client/api/data_sources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/data_sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/data_sources/get_remote_data_source_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/data_sources/get_remote_data_source_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     5594 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/data_sources/test_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 19:56:52.730816 dqops-1.1.0/dqops/client/api/default_column_check_patterns/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/default_column_check_patterns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/default_column_check_patterns/create_default_column_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/default_column_check_patterns/create_default_column_checks_pattern_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/default_column_check_patterns/delete_default_column_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/default_column_check_patterns/get_all_default_column_checks_patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/default_column_check_patterns/get_default_column_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/default_column_check_patterns/get_default_column_checks_pattern_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/default_column_check_patterns/get_default_monitoring_daily_column_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/default_column_check_patterns/get_default_monitoring_monthly_column_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/default_column_check_patterns/get_default_partitioned_daily_column_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/default_column_check_patterns/get_default_partitioned_monthly_column_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/default_column_check_patterns/get_default_profiling_column_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/default_column_check_patterns/update_default_column_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/default_column_check_patterns/update_default_column_checks_pattern_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/default_column_check_patterns/update_default_monitoring_daily_column_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/default_column_check_patterns/update_default_monitoring_monthly_column_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/default_column_check_patterns/update_default_partitioned_daily_column_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/default_column_check_patterns/update_default_partitioned_monthly_column_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/default_column_check_patterns/update_default_profiling_column_checks_pattern.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 19:56:52.734816 dqops-1.1.0/dqops/client/api/default_table_check_patterns/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/default_table_check_patterns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/default_table_check_patterns/create_default_table_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/default_table_check_patterns/create_default_table_checks_pattern_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/default_table_check_patterns/delete_default_table_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/default_table_check_patterns/get_all_default_table_checks_patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/default_table_check_patterns/get_default_monitoring_daily_table_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/default_table_check_patterns/get_default_monitoring_monthly_table_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/default_table_check_patterns/get_default_partitioned_daily_table_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/default_table_check_patterns/get_default_partitioned_monthly_table_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/default_table_check_patterns/get_default_profiling_table_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/default_table_check_patterns/get_default_table_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/default_table_check_patterns/get_default_table_checks_pattern_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/default_table_check_patterns/update_default_monitoring_daily_table_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/default_table_check_patterns/update_default_monitoring_monthly_table_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/default_table_check_patterns/update_default_partitioned_daily_table_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/default_table_check_patterns/update_default_partitioned_monthly_table_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/default_table_check_patterns/update_default_profiling_table_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/default_table_check_patterns/update_default_table_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/default_table_check_patterns/update_default_table_checks_pattern_target.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 19:56:52.734816 dqops-1.1.0/dqops/client/api/defaults/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/defaults/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/defaults/get_default_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/defaults/get_default_webhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/defaults/update_default_schedules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/defaults/update_default_webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 19:56:52.734816 dqops-1.1.0/dqops/client/api/dictionaries/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/dictionaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/dictionaries/create_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/dictionaries/delete_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/dictionaries/download_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/dictionaries/get_all_dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/dictionaries/get_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/dictionaries/update_dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 19:56:52.734816 dqops-1.1.0/dqops/client/api/environment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/environment/get_dqo_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/environment/get_user_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/environment/issue_api_key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 19:56:52.738816 dqops-1.1.0/dqops/client/api/errors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/errors/get_column_monitoring_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    11473 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/errors/get_column_partitioned_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    10967 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/errors/get_column_profiling_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    11109 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/errors/get_table_monitoring_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    11038 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/errors/get_table_partitioned_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    10564 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/errors/get_table_profiling_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 19:56:52.738816 dqops-1.1.0/dqops/client/api/healthcheck/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/healthcheck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/healthcheck/is_healthy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 19:56:52.738816 dqops-1.1.0/dqops/client/api/incidents/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/incidents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/incidents/find_connection_incident_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/incidents/find_recent_incidents_on_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/incidents/get_incident.py
--rw-r--r--   0 runner    (1001) docker     (127)     8575 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/incidents/get_incident_histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)    11115 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/incidents/get_incident_issues.py
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/incidents/set_incident_issue_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/incidents/set_incident_status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 19:56:52.742816 dqops-1.1.0/dqops/client/api/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/jobs/cancel_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/jobs/collect_statistics_on_data_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/jobs/collect_statistics_on_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     6655 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/jobs/delete_stored_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/jobs/get_all_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/jobs/get_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/jobs/get_job_changes_since.py
--rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/jobs/import_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/jobs/is_cron_scheduler_running.py
--rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/jobs/run_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/jobs/start_cron_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/jobs/stop_cron_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7575 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/jobs/synchronize_folders.py
--rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/jobs/wait_for_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/jobs/wait_for_run_checks_job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 19:56:52.742816 dqops-1.1.0/dqops/client/api/log_shipping/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/log_shipping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/log_shipping/log_debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/log_shipping/log_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/log_shipping/log_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/log_shipping/log_warn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 19:56:52.742816 dqops-1.1.0/dqops/client/api/rules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/rules/create_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/rules/delete_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/rules/get_all_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/rules/get_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/rules/get_rule_folder_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/rules/update_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 19:56:52.746816 dqops-1.1.0/dqops/client/api/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12030 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/schemas/get_schema_monitoring_checks_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7663 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/schemas/get_schema_monitoring_checks_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    12039 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/schemas/get_schema_partitioned_checks_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7668 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/schemas/get_schema_partitioned_checks_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    11401 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/schemas/get_schema_profiling_checks_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7122 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/schemas/get_schema_profiling_checks_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/schemas/get_schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 19:56:52.746816 dqops-1.1.0/dqops/client/api/sensor_readouts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/sensor_readouts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11745 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/sensor_readouts/get_column_monitoring_sensor_readouts.py
--rw-r--r--   0 runner    (1001) docker     (127)    11674 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/sensor_readouts/get_column_partitioned_sensor_readouts.py
--rw-r--r--   0 runner    (1001) docker     (127)    11120 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/sensor_readouts/get_column_profiling_sensor_readouts.py
--rw-r--r--   0 runner    (1001) docker     (127)    11286 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/sensor_readouts/get_table_monitoring_sensor_readouts.py
--rw-r--r--   0 runner    (1001) docker     (127)    11275 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/sensor_readouts/get_table_partitioned_sensor_readouts.py
--rw-r--r--   0 runner    (1001) docker     (127)    10741 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/sensor_readouts/get_table_profiling_sensor_readouts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 19:56:52.746816 dqops-1.1.0/dqops/client/api/sensors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/sensors/create_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/sensors/delete_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/sensors/get_all_sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/sensors/get_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/sensors/get_sensor_folder_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/sensors/update_sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 19:56:52.750816 dqops-1.1.0/dqops/client/api/shared_credentials/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/shared_credentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/shared_credentials/create_shared_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/shared_credentials/delete_shared_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/shared_credentials/download_shared_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/shared_credentials/get_all_shared_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/shared_credentials/get_shared_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/shared_credentials/update_shared_credential.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 19:56:52.750816 dqops-1.1.0/dqops/client/api/table_comparison_results/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/table_comparison_results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/table_comparison_results/get_table_comparison_monitoring_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/table_comparison_results/get_table_comparison_partitioned_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/table_comparison_results/get_table_comparison_profiling_results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 19:56:52.754816 dqops-1.1.0/dqops/client/api/table_comparisons/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/table_comparisons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/table_comparisons/create_table_comparison_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/table_comparisons/create_table_comparison_monitoring_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/table_comparisons/create_table_comparison_monitoring_monthly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/table_comparisons/create_table_comparison_partitioned_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/table_comparisons/create_table_comparison_partitioned_monthly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/table_comparisons/create_table_comparison_profiling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/table_comparisons/delete_table_comparison_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/table_comparisons/get_table_comparison_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     7589 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/table_comparisons/get_table_comparison_configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/table_comparisons/get_table_comparison_monitoring_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/table_comparisons/get_table_comparison_monitoring_monthly.py
--rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/table_comparisons/get_table_comparison_partitioned_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/table_comparisons/get_table_comparison_partitioned_monthly.py
--rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/table_comparisons/get_table_comparison_profiling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/table_comparisons/update_table_comparison_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/table_comparisons/update_table_comparison_monitoring_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/table_comparisons/update_table_comparison_monitoring_monthly.py
--rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/table_comparisons/update_table_comparison_partitioned_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/table_comparisons/update_table_comparison_partitioned_monthly.py
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/table_comparisons/update_table_comparison_profiling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 19:56:52.762817 dqops-1.1.0/dqops/client/api/tables/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/create_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/delete_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/get_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/get_table_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    10845 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/get_table_columns_monitoring_checks_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10854 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/get_table_columns_partitioned_checks_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10300 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/get_table_columns_profiling_checks_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4987 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/get_table_comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/get_table_daily_monitoring_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/get_table_daily_partitioned_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/get_table_default_grouping_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/get_table_incident_grouping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/get_table_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/get_table_monitoring_checks_basic_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/get_table_monitoring_checks_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/get_table_monitoring_checks_model_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/get_table_monitoring_checks_monthly.py
--rw-r--r--   0 runner    (1001) docker     (127)     7115 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/get_table_monitoring_checks_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/get_table_partitioned_checks_basic_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5764 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/get_table_partitioned_checks_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6793 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/get_table_partitioned_checks_model_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/get_table_partitioned_checks_monthly.py
--rw-r--r--   0 runner    (1001) docker     (127)     7120 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/get_table_partitioned_checks_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/get_table_partitioning.py
--rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/get_table_profiling_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/get_table_profiling_checks_basic_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/get_table_profiling_checks_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/get_table_profiling_checks_model_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6574 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/get_table_profiling_checks_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/get_table_scheduling_group_override.py
--rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/get_table_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/get_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/update_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/update_table_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/update_table_comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/update_table_daily_monitoring_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/update_table_default_grouping_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/update_table_incident_grouping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/update_table_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/update_table_monitoring_checks_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/update_table_monitoring_checks_monthly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/update_table_partitioned_checks_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     6611 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/update_table_partitioned_checks_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/update_table_partitioned_checks_monthly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/update_table_partitioning.py
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/update_table_profiling_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/update_table_profiling_checks_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/tables/update_table_scheduling_group_override.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 19:56:52.762817 dqops-1.1.0/dqops/client/api/timezones/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/timezones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/timezones/get_available_zone_ids.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 19:56:52.762817 dqops-1.1.0/dqops/client/api/users/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/users/change_caller_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/users/change_user_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/users/create_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/users/delete_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/users/get_all_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/users/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/api/users/update_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    12241 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 19:56:52.914817 dqops-1.1.0/dqops/client/models/
--rw-r--r--   0 runner    (1001) docker     (127)   127711 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/all_checks_patch_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/all_checks_patch_parameters_selected_tables_to_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/anomaly_differencing_percentile_moving_average_rule_error_05_pct_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/anomaly_differencing_percentile_moving_average_rule_fatal_01_pct_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/anomaly_differencing_percentile_moving_average_rule_warning_1_pct_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/anomaly_stationary_percentile_moving_average_rule_error_05_pct_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/anomaly_stationary_percentile_moving_average_rule_fatal_01_pct_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/anomaly_stationary_percentile_moving_average_rule_warning_1_pct_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/athena_authentication_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/authenticated_dashboard_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/between_floats_rule_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/between_ints_rule_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/between_percent_rule_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/big_query_authentication_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/big_query_jobs_create_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/big_query_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/bulk_check_deactivate_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/bulk_check_deactivate_parameters_selected_tables_to_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/change_percent_1_day_rule_10_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/change_percent_1_day_rule_20_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/change_percent_1_day_rule_50_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/change_percent_30_days_rule_10_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/change_percent_30_days_rule_20_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/change_percent_30_days_rule_50_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/change_percent_7_days_rule_10_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/change_percent_7_days_rule_20_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/change_percent_7_days_rule_50_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/change_percent_rule_10_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/change_percent_rule_20_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/change_percent_rule_50_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10580 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/check_configuration_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/check_container_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9069 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/check_container_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/check_container_type_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/check_current_data_quality_status_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/check_definition_folder_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/check_definition_folder_model_folders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/check_definition_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/check_definition_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/check_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    21543 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/check_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/check_result_entry_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/check_result_sort_order.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/check_result_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     5386 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/check_results_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7726 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/check_results_overview_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/check_run_schedule_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11585 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/check_search_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/check_target.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/check_target_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8642 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/check_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/check_time_scale.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/check_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    10325 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/cloud_synchronization_folders_status_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/collect_statistics_on_table_queue_job_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/collect_statistics_queue_job_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/collect_statistics_queue_job_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/collect_statistics_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    14850 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_accepted_values_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_accepted_values_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_accepted_values_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_accepted_values_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    15128 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_accepted_values_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_accepted_values_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    16655 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_accepted_values_monthly_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_accepted_values_monthly_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    14997 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_accepted_values_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_accepted_values_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_accepted_values_text_found_in_set_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10945 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_accuracy_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_accuracy_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    11425 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_accuracy_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_accuracy_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    11240 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_accuracy_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_accuracy_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10794 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_accuracy_total_average_match_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_accuracy_total_average_match_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10720 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_accuracy_total_max_match_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_accuracy_total_max_match_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10720 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_accuracy_total_min_match_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_accuracy_total_min_match_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10853 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_accuracy_total_not_null_count_match_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_accuracy_total_not_null_count_match_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10720 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_accuracy_total_sum_match_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_accuracy_total_sum_match_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    22723 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_anomaly_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_anomaly_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    27374 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_anomaly_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_anomaly_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    23256 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_anomaly_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_anomaly_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_bool_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_bool_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_bool_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_bool_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_bool_false_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_bool_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_bool_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_bool_monthly_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_bool_monthly_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_bool_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_bool_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_bool_true_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_column_exists_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_column_type_hash_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10518 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_comparison_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_comparison_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    11855 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_comparison_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_comparison_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_comparison_max_match_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_comparison_mean_match_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_comparison_min_match_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9735 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_comparison_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10800 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_comparison_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_comparison_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    12139 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_comparison_monthly_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_comparison_monthly_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10579 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_comparison_not_null_count_match_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10535 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_comparison_null_count_match_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_comparison_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_comparison_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_comparison_sum_match_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9827 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_conversions_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_conversions_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10648 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_conversions_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_conversions_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9997 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_conversions_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_conversions_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10862 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_conversions_monthly_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_conversions_monthly_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_conversions_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_conversions_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7988 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_current_data_quality_status_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_current_data_quality_status_model_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9810 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_custom_sql_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_custom_sql_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10653 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_custom_sql_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_custom_sql_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9980 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_custom_sql_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_custom_sql_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10835 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_custom_sql_monthly_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_custom_sql_monthly_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9809 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_custom_sql_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_custom_sql_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    20452 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_daily_monitoring_check_categories_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_daily_monitoring_check_categories_spec_comparisons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_daily_monitoring_check_categories_spec_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)    18781 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_daily_partitioned_check_categories_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_daily_partitioned_check_categories_spec_comparisons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_daily_partitioned_check_categories_spec_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_datatype_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_datatype_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_datatype_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_datatype_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10250 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_datatype_detected_datatype_in_text_changed_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_datatype_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_datatype_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_datatype_monthly_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_datatype_monthly_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6281 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_datatype_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_datatype_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_datatype_string_datatype_detect_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10569 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_date_in_range_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_date_in_range_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10767 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_date_values_in_future_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_datetime_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_datetime_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8372 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_datetime_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_datetime_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_datetime_date_values_in_future_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     7763 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_datetime_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_datetime_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8506 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_datetime_monthly_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_datetime_monthly_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_datetime_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_datetime_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_default_checks_pattern_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10307 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_detected_datatype_in_text_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    11810 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_distinct_count_anomaly_differencing_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    11785 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_distinct_count_anomaly_stationary_partition_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10713 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_distinct_count_change_1_day_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10771 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_distinct_count_change_30_days_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10742 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_distinct_count_change_7_days_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10579 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_distinct_count_change_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10012 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_distinct_count_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    11739 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_distinct_percent_anomaly_stationary_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_distinct_percent_change_1_day_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10797 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_distinct_percent_change_30_days_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10768 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_distinct_percent_change_7_days_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10605 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_distinct_percent_change_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10616 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_distinct_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10531 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_duplicate_count_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10589 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_duplicate_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10759 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_expected_numbers_in_use_count_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10803 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_expected_text_values_in_use_count_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10776 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_expected_texts_in_top_values_count_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9969 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_false_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10720 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_integer_in_range_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_integrity_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_integrity_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6528 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_integrity_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_integrity_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10819 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_integrity_foreign_key_match_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_integrity_foreign_key_match_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_integrity_foreign_key_not_match_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10528 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_integrity_lookup_key_not_found_count_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_integrity_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_integrity_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_integrity_monthly_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_integrity_monthly_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_integrity_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_integrity_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10704 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_invalid_email_format_found_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_invalid_ip_4_address_format_found_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_invalid_ip_6_address_format_found_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10630 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_invalid_latitude_count_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10643 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_invalid_longitude_count_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10691 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_invalid_uuid_format_found_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    16978 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11607 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_max_anomaly_differencing_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    11510 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_max_anomaly_stationary_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_max_in_range_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    11523 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_mean_anomaly_stationary_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10523 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_mean_change_1_day_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10581 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_mean_change_30_days_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10552 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_mean_change_7_days_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10389 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_mean_change_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9879 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_mean_in_range_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    11549 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_median_anomaly_stationary_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10549 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_median_change_1_day_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_median_change_30_days_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10578 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_median_change_7_days_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10415 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_median_change_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9905 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_median_in_range_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    11607 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_min_anomaly_differencing_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    11510 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_min_anomaly_stationary_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_min_in_range_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_monitoring_check_categories_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    19879 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_monthly_monitoring_check_categories_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_monthly_monitoring_check_categories_spec_comparisons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_monthly_monitoring_check_categories_spec_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)    18220 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_monthly_partitioned_check_categories_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_monthly_partitioned_check_categories_spec_comparisons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_monthly_partitioned_check_categories_spec_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)    10480 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_negative_count_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_negative_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_non_negative_count_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10596 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_non_negative_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9900 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_not_nulls_count_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_not_nulls_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_null_percent_anomaly_stationary_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10641 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_null_percent_change_1_day_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10699 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_null_percent_change_30_days_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_null_percent_change_7_days_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10507 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_null_percent_change_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10425 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_nulls_count_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    14733 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_nulls_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_nulls_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    16920 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_nulls_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_nulls_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7474 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_nulls_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_nulls_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_nulls_monthly_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_nulls_monthly_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_nulls_not_nulls_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_nulls_not_nulls_count_statistics_collector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_nulls_not_nulls_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_nulls_not_nulls_percent_statistics_collector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_nulls_nulls_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_nulls_nulls_count_statistics_collector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_nulls_nulls_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_nulls_nulls_percent_statistics_collector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10483 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_nulls_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    15004 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_nulls_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_nulls_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_nulls_statistics_collectors_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10686 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_number_above_max_value_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10772 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_number_above_max_value_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10686 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_number_below_min_value_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10772 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_number_below_min_value_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_number_found_in_set_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10707 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_number_in_range_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    40287 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    47758 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_expected_numbers_in_use_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_integer_in_range_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_invalid_latitude_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_invalid_longitude_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_max_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_mean_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_median_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_min_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    42487 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    49106 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_monthly_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_monthly_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_negative_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_negative_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_non_negative_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_non_negative_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_number_above_max_value_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_number_above_max_value_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_number_below_min_value_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_number_below_min_value_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_number_found_in_set_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_number_in_range_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_percentile_10_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_percentile_25_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_percentile_75_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_percentile_90_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_percentile_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_population_stddev_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_population_variance_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    42302 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_sample_stddev_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_sample_variance_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_sum_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_valid_latitude_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_numeric_valid_longitude_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_partitioned_check_categories_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    19822 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_patterns_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_patterns_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    21913 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_patterns_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_patterns_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_patterns_invalid_email_format_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_patterns_invalid_ip_4_address_format_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_patterns_invalid_ip_6_address_format_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_patterns_invalid_uuid_format_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    20252 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_patterns_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_patterns_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    22409 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_patterns_monthly_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_patterns_monthly_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    20067 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_patterns_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_patterns_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_patterns_text_matching_date_pattern_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_patterns_text_matching_name_pattern_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_patterns_text_not_matching_date_pattern_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_patterns_text_not_matching_regex_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_patterns_texts_matching_regex_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_patterns_valid_uuid_format_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_percentile_10_in_range_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_percentile_25_in_range_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_percentile_75_in_range_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_percentile_90_in_range_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_percentile_in_range_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10608 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_pii_contains_email_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_pii_contains_email_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10573 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_pii_contains_ip_4_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_pii_contains_ip_4_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10573 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_pii_contains_ip_6_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_pii_contains_ip_6_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10652 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_pii_contains_usa_phone_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_pii_contains_usa_phone_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10718 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_pii_contains_usa_zipcode_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_pii_contains_usa_zipcode_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10186 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_pii_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_pii_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    11497 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_pii_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_pii_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10534 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_pii_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_pii_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    11725 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_pii_monthly_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_pii_monthly_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10411 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_pii_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_pii_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10084 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_population_stddev_in_range_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10110 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_population_variance_in_range_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    19300 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_profiling_check_categories_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_profiling_check_categories_spec_comparisons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_profiling_check_categories_spec_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_range_max_value_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_range_max_value_statistics_collector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_range_median_value_statistics_collector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_range_min_value_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_range_min_value_statistics_collector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_range_statistics_collectors_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_range_sum_value_statistics_collector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_sample_stddev_in_range_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_sample_variance_in_range_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_sampling_column_samples_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_sampling_column_samples_statistics_collector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_sampling_statistics_collectors_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9784 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_schema_column_exists_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_schema_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_schema_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_schema_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_schema_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_schema_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_schema_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9919 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_schema_type_changed_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9687 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_sql_aggregate_expression_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_sql_aggregated_expression_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10548 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_sql_condition_failed_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_sql_condition_failed_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10674 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_sql_condition_passed_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_sql_condition_passed_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_sql_import_custom_result_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_sql_import_custom_result_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     6749 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_statistics_collectors_root_categories_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     8114 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_statistics_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_strings_expected_text_values_in_use_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_strings_expected_texts_in_top_values_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    11607 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_sum_anomaly_differencing_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_sum_anomaly_stationary_partition_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10510 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_sum_change_1_day_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10568 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_sum_change_30_days_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10539 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_sum_change_7_days_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_sum_change_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_sum_in_range_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    14842 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    16767 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10805 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_found_in_set_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_length_above_max_length_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_length_above_max_length_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_length_below_min_length_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_length_below_min_length_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10740 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_length_in_range_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_match_date_format_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_match_date_format_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10832 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_matching_date_pattern_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10832 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_matching_name_pattern_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_max_length_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9984 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_mean_length_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_min_length_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    15200 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    17161 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_monthly_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_monthly_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10778 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_not_matching_date_pattern_found_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10735 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_not_matching_regex_found_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10814 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_parsable_to_boolean_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_parsable_to_date_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10788 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_parsable_to_float_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10814 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_parsable_to_integer_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    15077 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_statistics_collectors_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_text_datatype_detect_statistics_collector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_text_length_above_max_length_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_text_length_above_max_length_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_text_length_below_min_length_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_text_length_below_min_length_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_text_length_in_range_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_text_max_length_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_text_max_length_statistics_collector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_text_mean_length_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_text_mean_length_statistics_collector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_text_min_length_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_text_min_length_statistics_collector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_text_parsable_to_boolean_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_text_parsable_to_date_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_text_parsable_to_float_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_text_parsable_to_integer_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_text_valid_country_code_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_text_valid_currency_code_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10801 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_valid_country_code_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10814 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_text_valid_currency_code_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10802 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_texts_matching_regex_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9956 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_true_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_type_snapshot_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    23392 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_uniqueness_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_uniqueness_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    26847 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_uniqueness_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_uniqueness_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_uniqueness_distinct_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_uniqueness_distinct_count_statistics_collector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_uniqueness_distinct_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_uniqueness_distinct_percent_statistics_collector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_uniqueness_duplicate_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_uniqueness_duplicate_count_statistics_collector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_uniqueness_duplicate_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_uniqueness_duplicate_percent_statistics_collector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_uniqueness_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_uniqueness_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    12425 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_uniqueness_monthly_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_uniqueness_monthly_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    23959 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_uniqueness_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_uniqueness_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_uniqueness_statistics_collectors_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10702 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_valid_latitude_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10715 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_valid_longitude_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10763 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_valid_uuid_format_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_whitespace_blank_null_placeholder_text_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_whitespace_blank_null_placeholder_text_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    15940 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_whitespace_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_whitespace_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    17913 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_whitespace_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_whitespace_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_whitespace_empty_text_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10589 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_whitespace_empty_text_found_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10647 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_whitespace_empty_text_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_whitespace_empty_text_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_whitespace_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_whitespace_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    18227 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_whitespace_monthly_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_whitespace_monthly_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10812 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_whitespace_null_placeholder_text_found_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10870 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_whitespace_null_placeholder_text_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    16229 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_whitespace_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_whitespace_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_whitespace_text_surrounded_by_whitespace_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10866 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_whitespace_text_surrounded_by_whitespace_found_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10924 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_whitespace_text_surrounded_by_whitespace_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_whitespace_text_surrounded_by_whitespace_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_whitespace_whitespace_text_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10716 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_whitespace_whitespace_text_found_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10774 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_whitespace_whitespace_text_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/column_whitespace_whitespace_text_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/comment_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/common_column_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/compare_thresholds_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/comparison_check_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/compression_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     6267 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/connection_incident_grouping_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    22688 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/connection_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    16568 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/connection_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/connection_specification_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/connection_test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/connection_test_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/count_between_rule_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/credential_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/csv_file_format_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10788 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/custom_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/custom_rule_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/custom_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/dashboard_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/dashboard_spec_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/dashboards_folder_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/data_delete_result_partition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/data_dictionary_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/data_dictionary_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/data_grouping_configuration_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4876 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/data_grouping_configuration_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/data_grouping_configuration_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/data_grouping_configuration_trimmed_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/data_grouping_dimension_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/data_grouping_dimension_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/data_type_category.py
--rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/databricks_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/databricks_parameters_spec_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/datetime_built_in_date_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/default_column_checks_pattern_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/default_column_checks_pattern_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/default_schedules_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/default_table_checks_pattern_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/default_table_checks_pattern_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11837 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/delete_stored_data_queue_job_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/delete_stored_data_queue_job_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/delete_stored_data_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/delete_stored_data_result_partition_results.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/detected_datatype_category.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/detected_datatype_equals_rule_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/display_hint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/dqo_cloud_user_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/dqo_job_change_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    16949 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/dqo_job_entry_parameters_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/dqo_job_history_entry_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/dqo_job_queue_incremental_snapshot_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/dqo_job_queue_initial_snapshot_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/dqo_job_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/dqo_job_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/dqo_queue_job_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/dqo_root.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/dqo_settings_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/dqo_settings_model_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/dqo_settings_model_properties_additional_property.py
--rw-r--r--   0 runner    (1001) docker     (127)    14643 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/dqo_user_profile_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/dqo_user_role.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/duckdb_files_format_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/duckdb_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/duckdb_parameters_spec_directories.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/duckdb_parameters_spec_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/duckdb_read_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/duckdb_storage_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/duration.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/effective_schedule_level_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/effective_schedule_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/equals_1_rule_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/equals_integer_rule_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     8316 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/error_entry_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/errors_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/external_log_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/field_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/file_format_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/file_synchronization_direction.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/folder_synchronization_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/hierarchy_id_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/hierarchy_id_model_path_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/historic_data_points_grouping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/import_schema_queue_job_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/import_severity_rule_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/import_tables_queue_job_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/import_tables_queue_job_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/import_tables_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/incident_daily_issues_count.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/incident_grouping_level.py
--rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/incident_issue_histogram_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/incident_issue_histogram_model_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/incident_issue_histogram_model_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/incident_issue_histogram_model_days.py
--rw-r--r--   0 runner    (1001) docker     (127)     9890 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/incident_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/incident_sort_order.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/incident_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/incident_webhook_notifications_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/incidents_per_connection_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7404 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/json_file_format_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/json_format_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/json_records_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/max_count_rule_0_error_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/max_count_rule_0_warning_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/max_count_rule_100_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/max_days_rule_1_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/max_days_rule_2_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/max_days_rule_7_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/max_diff_percent_rule_0_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/max_diff_percent_rule_1_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/max_diff_percent_rule_5_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/max_failures_rule_0_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/max_failures_rule_1_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/max_failures_rule_5_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/max_missing_rule_0_error_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/max_missing_rule_0_warning_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/max_missing_rule_2_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/max_percent_rule_0_error_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/max_percent_rule_0_warning_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/max_percent_rule_5_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/min_count_rule_1_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/min_percent_rule_100_error_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/min_percent_rule_100_warning_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/min_percent_rule_95_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/minimum_grouping_severity_level.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/monitoring_schedule_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/mono.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/mono_dqo_queue_job_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/mono_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/mono_void.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/my_sql_ssl_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/mysql_engine_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/mysql_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/mysql_parameters_spec_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/new_line_character_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/optional.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/optional_incident_webhook_notifications_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/optional_monitoring_schedule_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/oracle_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/oracle_parameters_spec_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/parameter_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/parameter_definition_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/parquet_file_format_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/partition_incremental_time_window_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/physical_table_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/postgresql_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/postgresql_parameters_spec_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/postgresql_ssl_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/presto_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/presto_parameters_spec_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/profiling_time_period_truncation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/provider_sensor_definition_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/provider_sensor_definition_spec_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/provider_sensor_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/provider_sensor_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/provider_sensor_runner_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/provider_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     6239 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/quality_category_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/redshift_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/redshift_parameters_spec_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/remote_table_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/repair_stored_data_queue_job_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/rule_folder_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/rule_folder_model_folders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/rule_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8052 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/rule_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/rule_model_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/rule_parameters_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/rule_runner_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/rule_severity_level.py
--rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/rule_thresholds_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/rule_time_window_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/rule_time_window_settings_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/run_checks_on_table_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/run_checks_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/run_checks_queue_job_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/run_checks_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/schedule_enabled_status_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13462 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/schema_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/schema_remote_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5648 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/sensor_definition_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/sensor_definition_spec_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/sensor_folder_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/sensor_folder_model_folders.py
--rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/sensor_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/sensor_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7283 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/sensor_readout_entry_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/sensor_readouts_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/shared_credential_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/shared_credential_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/similar_check_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/single_store_db_load_balancing_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/single_store_db_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/snowflake_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/snowflake_parameters_spec_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/sort_direction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/spark_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/spark_parameters_spec_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/spring_error_payload.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/sql_server_authentication_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/sql_server_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/sql_server_parameters_spec_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     9001 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/statistics_collector_search_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/statistics_collector_target.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/statistics_data_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/statistics_metric_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/statistics_metric_model_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/statistics_result_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     8752 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/synchronize_multiple_folders_dqo_queue_job_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/synchronize_multiple_folders_queue_job_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/synchronize_root_folder_dqo_queue_job_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/synchronize_root_folder_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_accuracy_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_accuracy_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_accuracy_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_accuracy_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_accuracy_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_accuracy_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10823 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_accuracy_total_row_count_match_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_accuracy_total_row_count_match_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10317 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_availability_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_availability_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_availability_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_availability_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_availability_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_availability_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_availability_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_availability_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_column_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_column_list_ordered_hash_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_column_list_unordered_hash_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_column_types_hash_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_columns_statistics_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_comparison_column_count_match_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_comparison_column_results_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_comparison_column_results_model_column_comparison_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     9448 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_comparison_configuration_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7836 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_comparison_configuration_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_comparison_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_comparison_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_comparison_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_comparison_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_comparison_grouping_column_pair_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_comparison_grouping_columns_pair_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    16678 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_comparison_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_comparison_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_comparison_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_comparison_monthly_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_comparison_monthly_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_comparison_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_comparison_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_comparison_results_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_comparison_results_model_column_comparison_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_comparison_results_model_table_comparison_results.py
--rw-r--r--   0 runner    (1001) docker     (127)    10479 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_comparison_row_count_match_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10906 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_current_data_quality_status_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_current_data_quality_status_model_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_current_data_quality_status_model_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     9671 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_custom_sql_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_custom_sql_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10536 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_custom_sql_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_custom_sql_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9863 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_custom_sql_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_custom_sql_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10706 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_custom_sql_monthly_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_custom_sql_monthly_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_custom_sql_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_custom_sql_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9780 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_daily_monitoring_check_categories_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_daily_monitoring_check_categories_spec_comparisons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_daily_monitoring_check_categories_spec_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_daily_partitioned_check_categories_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_daily_partitioned_check_categories_spec_comparisons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_daily_partitioned_check_categories_spec_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)    10225 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_data_freshness_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_data_ingestion_delay_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10225 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_data_staleness_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     5907 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_default_checks_pattern_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_incident_grouping_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    20607 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_monitoring_check_categories_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_monthly_monitoring_check_categories_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_monthly_monitoring_check_categories_spec_comparisons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_monthly_monitoring_check_categories_spec_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_monthly_partitioned_check_categories_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_monthly_partitioned_check_categories_spec_comparisons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_monthly_partitioned_check_categories_spec_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_owner_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_partition_reload_lag_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_partitioned_check_categories_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_partitioning_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10183 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_profiling_check_categories_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_profiling_check_categories_spec_comparisons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_profiling_check_categories_spec_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)    11656 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_row_count_anomaly_differencing_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    11631 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_row_count_anomaly_stationary_partition_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10559 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_row_count_change_1_day_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10617 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_row_count_change_30_days_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_row_count_change_7_days_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10425 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_row_count_change_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9795 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_row_count_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9918 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_schema_column_count_changed_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9896 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_schema_column_count_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_schema_column_count_statistics_collector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_schema_column_list_changed_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10068 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_schema_column_list_or_order_changed_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_schema_column_types_changed_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9710 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_schema_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_schema_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10040 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_schema_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_schema_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9877 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_schema_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_schema_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_schema_statistics_collectors_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    19622 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_spec_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_spec_groupings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_spec_table_comparisons.py
--rw-r--r--   0 runner    (1001) docker     (127)    10049 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_sql_aggregate_expression_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_sql_aggregated_expression_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10521 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_sql_condition_failed_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_sql_condition_failed_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10661 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_sql_condition_passed_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_sql_condition_passed_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10049 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_sql_import_custom_result_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_sql_import_custom_result_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_statistics_collectors_root_categories_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_statistics_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_timeliness_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_timeliness_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_timeliness_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_timeliness_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_timeliness_data_freshness_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_timeliness_data_ingestion_delay_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_timeliness_data_staleness_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_timeliness_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_timeliness_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_timeliness_monthly_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_timeliness_monthly_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_timeliness_partition_reload_lag_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     6387 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_timeliness_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_timeliness_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10418 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_volume_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_volume_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    12139 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_volume_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_volume_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_volume_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_volume_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_volume_monthly_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_volume_monthly_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_volume_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_volume_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_volume_row_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_volume_row_count_statistics_collector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/table_volume_statistics_collectors_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/target_column_pattern_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/target_table_pattern_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/temporal_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/text_built_in_date_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/time_period_gradient.py
--rw-r--r--   0 runner    (1001) docker     (127)    11573 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/time_window_filter_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/timestamp_columns_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/trino_engine_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     7909 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/trino_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/trino_parameters_spec_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/models/value_changed_rule_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/client/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7486 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/install.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/startdqo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-24 19:44:21.000000 dqops-1.1.0/dqops/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 19:56:52.914817 dqops-1.1.0/dqops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-03-24 19:56:52.000000 dqops-1.1.0/dqops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    77987 2024-03-24 19:56:52.000000 dqops-1.1.0/dqops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 19:56:52.000000 dqops-1.1.0/dqops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-24 19:56:52.000000 dqops-1.1.0/dqops.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-24 19:56:52.000000 dqops-1.1.0/dqops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-24 19:56:52.000000 dqops-1.1.0/dqops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-24 19:44:21.000000 dqops-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-24 19:56:52.914817 dqops-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-03-24 19:44:21.000000 dqops-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:11:50.504365 dqops-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11353 2024-04-25 11:58:27.000000 dqops-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-04-25 12:11:50.504365 dqops-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9142 2024-04-25 11:58:27.000000 dqops-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:11:50.028370 dqops-1.2.0/dqops/
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:11:50.032370 dqops-1.2.0/dqops/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:11:50.032370 dqops-1.2.0/dqops/client/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:11:50.032370 dqops-1.2.0/dqops/client/api/check_results/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/check_results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11604 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/check_results/get_column_monitoring_checks_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11573 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/check_results/get_column_partitioned_checks_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11067 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/check_results/get_column_profiling_checks_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14194 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/check_results/get_table_data_quality_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11225 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/check_results/get_table_monitoring_checks_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11150 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/check_results/get_table_partitioned_checks_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10680 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/check_results/get_table_profiling_checks_results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:11:50.036370 dqops-1.2.0/dqops/client/api/check_results_overview/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/check_results_overview/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/check_results_overview/get_column_monitoring_checks_overview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/check_results_overview/get_column_partitioned_checks_overview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7367 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/check_results_overview/get_column_profiling_checks_overview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7489 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/check_results_overview/get_table_monitoring_checks_overview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7454 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/check_results_overview/get_table_partitioned_checks_overview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/check_results_overview/get_table_profiling_checks_overview.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:11:50.036370 dqops-1.2.0/dqops/client/api/checks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/checks/create_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/checks/delete_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/checks/get_all_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/checks/get_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/checks/get_check_folder_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/checks/update_check.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:11:50.052370 dqops-1.2.0/dqops/client/api/columns/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/columns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/columns/create_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/columns/delete_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/columns/get_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/columns/get_column_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5418 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/columns/get_column_comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/columns/get_column_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6089 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/columns/get_column_monitoring_checks_basic_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5753 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/columns/get_column_monitoring_checks_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/columns/get_column_monitoring_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/columns/get_column_monitoring_checks_model_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/columns/get_column_monitoring_checks_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/columns/get_column_partitioned_checks_basic_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/columns/get_column_partitioned_checks_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/columns/get_column_partitioned_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7044 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/columns/get_column_partitioned_checks_model_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/columns/get_column_partitioned_checks_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/columns/get_column_profiling_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/columns/get_column_profiling_checks_basic_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/columns/get_column_profiling_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6434 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/columns/get_column_profiling_checks_model_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/columns/get_column_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/columns/get_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/columns/get_columns_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/columns/update_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/columns/update_column_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/columns/update_column_comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/columns/update_column_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/columns/update_column_monitoring_checks_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/columns/update_column_monitoring_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/columns/update_column_monitoring_checks_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/columns/update_column_partitioned_checks_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/columns/update_column_partitioned_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/columns/update_column_partitioned_checks_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/columns/update_column_profiling_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/columns/update_column_profiling_checks_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:11:50.056370 dqops-1.2.0/dqops/client/api/connections/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/connections/bulk_activate_connection_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/connections/bulk_deactivate_connection_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/connections/create_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/connections/create_connection_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/connections/delete_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/connections/get_all_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/connections/get_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/connections/get_connection_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/connections/get_connection_comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/connections/get_connection_common_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/connections/get_connection_default_grouping_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/connections/get_connection_incident_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/connections/get_connection_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/connections/get_connection_scheduling_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/connections/update_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/connections/update_connection_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/connections/update_connection_comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/connections/update_connection_default_grouping_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/connections/update_connection_incident_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/connections/update_connection_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/connections/update_connection_scheduling_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:11:50.060370 dqops-1.2.0/dqops/client/api/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/dashboards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/dashboards/get_all_dashboards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/dashboards/get_dashboard_level_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/dashboards/get_dashboard_level_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/dashboards/get_dashboard_level_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/dashboards/get_dashboard_level_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/dashboards/get_dashboard_level_5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:11:50.064370 dqops-1.2.0/dqops/client/api/data_grouping_configurations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/data_grouping_configurations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/data_grouping_configurations/create_table_grouping_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/data_grouping_configurations/delete_table_grouping_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/data_grouping_configurations/get_table_grouping_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/data_grouping_configurations/get_table_grouping_configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/data_grouping_configurations/set_table_default_grouping_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4220 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/data_grouping_configurations/update_table_grouping_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:11:50.072370 dqops-1.2.0/dqops/client/api/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/data_sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/data_sources/get_remote_data_source_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/data_sources/get_remote_data_source_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5594 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/data_sources/test_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:11:50.080370 dqops-1.2.0/dqops/client/api/default_column_check_patterns/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/default_column_check_patterns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/default_column_check_patterns/create_default_column_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/default_column_check_patterns/create_default_column_checks_pattern_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/default_column_check_patterns/delete_default_column_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/default_column_check_patterns/get_all_default_column_checks_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/default_column_check_patterns/get_default_column_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/default_column_check_patterns/get_default_column_checks_pattern_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/default_column_check_patterns/get_default_monitoring_daily_column_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/default_column_check_patterns/get_default_monitoring_monthly_column_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/default_column_check_patterns/get_default_partitioned_daily_column_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/default_column_check_patterns/get_default_partitioned_monthly_column_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/default_column_check_patterns/get_default_profiling_column_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/default_column_check_patterns/update_default_column_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/default_column_check_patterns/update_default_column_checks_pattern_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/default_column_check_patterns/update_default_monitoring_daily_column_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/default_column_check_patterns/update_default_monitoring_monthly_column_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/default_column_check_patterns/update_default_partitioned_daily_column_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/default_column_check_patterns/update_default_partitioned_monthly_column_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/default_column_check_patterns/update_default_profiling_column_checks_pattern.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:11:50.084370 dqops-1.2.0/dqops/client/api/default_table_check_patterns/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/default_table_check_patterns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/default_table_check_patterns/create_default_table_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/default_table_check_patterns/create_default_table_checks_pattern_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/default_table_check_patterns/delete_default_table_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/default_table_check_patterns/get_all_default_table_checks_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/default_table_check_patterns/get_default_monitoring_daily_table_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/default_table_check_patterns/get_default_monitoring_monthly_table_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/default_table_check_patterns/get_default_partitioned_daily_table_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/default_table_check_patterns/get_default_partitioned_monthly_table_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/default_table_check_patterns/get_default_profiling_table_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/default_table_check_patterns/get_default_table_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/default_table_check_patterns/get_default_table_checks_pattern_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/default_table_check_patterns/update_default_monitoring_daily_table_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/default_table_check_patterns/update_default_monitoring_monthly_table_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/default_table_check_patterns/update_default_partitioned_daily_table_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/default_table_check_patterns/update_default_partitioned_monthly_table_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/default_table_check_patterns/update_default_profiling_table_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/default_table_check_patterns/update_default_table_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/default_table_check_patterns/update_default_table_checks_pattern_target.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:11:50.088370 dqops-1.2.0/dqops/client/api/defaults/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/defaults/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/defaults/get_default_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/defaults/get_default_webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/defaults/update_default_schedules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/defaults/update_default_webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:11:50.088370 dqops-1.2.0/dqops/client/api/dictionaries/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/dictionaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/dictionaries/create_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/dictionaries/delete_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/dictionaries/download_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/dictionaries/get_all_dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/dictionaries/get_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/dictionaries/update_dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:11:50.092370 dqops-1.2.0/dqops/client/api/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/environment/get_dqo_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/environment/get_user_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/environment/issue_api_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:11:50.092370 dqops-1.2.0/dqops/client/api/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/errors/get_column_monitoring_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11473 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/errors/get_column_partitioned_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10967 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/errors/get_column_profiling_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11109 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/errors/get_table_monitoring_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11038 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/errors/get_table_partitioned_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10564 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/errors/get_table_profiling_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:11:50.092370 dqops-1.2.0/dqops/client/api/healthcheck/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/healthcheck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/healthcheck/is_healthy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:11:50.096370 dqops-1.2.0/dqops/client/api/incidents/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/incidents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/incidents/find_connection_incident_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/incidents/find_recent_incidents_on_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/incidents/get_incident.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8575 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/incidents/get_incident_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11115 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/incidents/get_incident_issues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/incidents/set_incident_issue_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/incidents/set_incident_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:11:50.100370 dqops-1.2.0/dqops/client/api/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/jobs/cancel_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/jobs/collect_statistics_on_data_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/jobs/collect_statistics_on_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6655 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/jobs/delete_stored_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/jobs/get_all_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/jobs/get_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/jobs/get_job_changes_since.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/jobs/import_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/jobs/is_cron_scheduler_running.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/jobs/run_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/jobs/start_cron_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/jobs/stop_cron_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7575 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/jobs/synchronize_folders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/jobs/wait_for_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/jobs/wait_for_run_checks_job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:11:50.104369 dqops-1.2.0/dqops/client/api/labels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/labels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/labels/get_all_labels_for_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/labels/get_all_labels_for_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6145 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/labels/get_all_labels_for_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:11:50.104369 dqops-1.2.0/dqops/client/api/log_shipping/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/log_shipping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/log_shipping/log_debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/log_shipping/log_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/log_shipping/log_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/log_shipping/log_warn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:11:50.104369 dqops-1.2.0/dqops/client/api/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/rules/create_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/rules/delete_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/rules/get_all_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/rules/get_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/rules/get_rule_folder_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/rules/update_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:11:50.108369 dqops-1.2.0/dqops/client/api/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12030 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/schemas/get_schema_monitoring_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7663 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/schemas/get_schema_monitoring_checks_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12039 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/schemas/get_schema_partitioned_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7668 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/schemas/get_schema_partitioned_checks_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11401 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/schemas/get_schema_profiling_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7122 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/schemas/get_schema_profiling_checks_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/schemas/get_schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:11:50.108369 dqops-1.2.0/dqops/client/api/search/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8062 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/search/find_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:11:50.112369 dqops-1.2.0/dqops/client/api/sensor_readouts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/sensor_readouts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11745 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/sensor_readouts/get_column_monitoring_sensor_readouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11674 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/sensor_readouts/get_column_partitioned_sensor_readouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11120 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/sensor_readouts/get_column_profiling_sensor_readouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11286 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/sensor_readouts/get_table_monitoring_sensor_readouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11275 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/sensor_readouts/get_table_partitioned_sensor_readouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10741 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/sensor_readouts/get_table_profiling_sensor_readouts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:11:50.112369 dqops-1.2.0/dqops/client/api/sensors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/sensors/create_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/sensors/delete_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/sensors/get_all_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/sensors/get_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/sensors/get_sensor_folder_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/sensors/update_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:11:50.116369 dqops-1.2.0/dqops/client/api/shared_credentials/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/shared_credentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/shared_credentials/create_shared_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/shared_credentials/delete_shared_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/shared_credentials/download_shared_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/shared_credentials/get_all_shared_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/shared_credentials/get_shared_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/shared_credentials/update_shared_credential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:11:50.116369 dqops-1.2.0/dqops/client/api/table_comparison_results/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/table_comparison_results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/table_comparison_results/get_table_comparison_monitoring_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/table_comparison_results/get_table_comparison_partitioned_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/table_comparison_results/get_table_comparison_profiling_results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:11:50.128369 dqops-1.2.0/dqops/client/api/table_comparisons/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/table_comparisons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/table_comparisons/create_table_comparison_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/table_comparisons/create_table_comparison_monitoring_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/table_comparisons/create_table_comparison_monitoring_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/table_comparisons/create_table_comparison_partitioned_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/table_comparisons/create_table_comparison_partitioned_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/table_comparisons/create_table_comparison_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/table_comparisons/delete_table_comparison_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/table_comparisons/get_table_comparison_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7589 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/table_comparisons/get_table_comparison_configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/table_comparisons/get_table_comparison_monitoring_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/table_comparisons/get_table_comparison_monitoring_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/table_comparisons/get_table_comparison_partitioned_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/table_comparisons/get_table_comparison_partitioned_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/table_comparisons/get_table_comparison_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/table_comparisons/update_table_comparison_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/table_comparisons/update_table_comparison_monitoring_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/table_comparisons/update_table_comparison_monitoring_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/table_comparisons/update_table_comparison_partitioned_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/table_comparisons/update_table_comparison_partitioned_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/table_comparisons/update_table_comparison_profiling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:11:50.144369 dqops-1.2.0/dqops/client/api/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/create_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/delete_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/get_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/get_table_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10845 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/get_table_columns_monitoring_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10854 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/get_table_columns_partitioned_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10300 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/get_table_columns_profiling_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4987 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/get_table_comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/get_table_daily_monitoring_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/get_table_daily_partitioned_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/get_table_default_grouping_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/get_table_incident_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/get_table_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/get_table_monitoring_checks_basic_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/get_table_monitoring_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/get_table_monitoring_checks_model_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/get_table_monitoring_checks_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7115 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/get_table_monitoring_checks_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/get_table_partitioned_checks_basic_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5764 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/get_table_partitioned_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6793 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/get_table_partitioned_checks_model_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/get_table_partitioned_checks_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7120 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/get_table_partitioned_checks_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/get_table_partitioning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/get_table_profiling_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/get_table_profiling_checks_basic_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/get_table_profiling_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/get_table_profiling_checks_model_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6574 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/get_table_profiling_checks_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/get_table_scheduling_group_override.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/get_table_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7932 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/get_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/update_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/update_table_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/update_table_comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/update_table_daily_monitoring_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/update_table_default_grouping_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/update_table_incident_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/update_table_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/update_table_monitoring_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/update_table_monitoring_checks_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/update_table_partitioned_checks_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6611 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/update_table_partitioned_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/update_table_partitioned_checks_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/update_table_partitioning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/update_table_profiling_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/update_table_profiling_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/tables/update_table_scheduling_group_override.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:11:50.144369 dqops-1.2.0/dqops/client/api/timezones/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/timezones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/timezones/get_available_zone_ids.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:11:50.148369 dqops-1.2.0/dqops/client/api/users/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/users/change_caller_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/users/change_user_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/users/create_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/users/delete_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/users/get_all_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/users/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/api/users/update_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12241 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:11:50.504365 dqops-1.2.0/dqops/client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)   128728 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/all_checks_patch_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/all_checks_patch_parameters_selected_tables_to_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/anomaly_differencing_percentile_moving_average_rule_error_05_pct_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/anomaly_differencing_percentile_moving_average_rule_fatal_01_pct_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/anomaly_differencing_percentile_moving_average_rule_warning_1_pct_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/anomaly_stationary_percentile_moving_average_rule_error_05_pct_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/anomaly_stationary_percentile_moving_average_rule_fatal_01_pct_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/anomaly_stationary_percentile_moving_average_rule_warning_1_pct_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/authenticated_dashboard_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/aws_authentication_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/between_floats_rule_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/between_ints_rule_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/between_percent_rule_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/big_query_authentication_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/big_query_jobs_create_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/big_query_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/bulk_check_deactivate_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/bulk_check_deactivate_parameters_selected_tables_to_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/change_percent_1_day_rule_10_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/change_percent_1_day_rule_20_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/change_percent_1_day_rule_50_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/change_percent_30_days_rule_10_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/change_percent_30_days_rule_20_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/change_percent_30_days_rule_50_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/change_percent_7_days_rule_10_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/change_percent_7_days_rule_20_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/change_percent_7_days_rule_50_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/change_percent_rule_10_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/change_percent_rule_20_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/change_percent_rule_50_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10580 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/check_configuration_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/check_container_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9069 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/check_container_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/check_container_type_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9269 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/check_current_data_quality_status_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/check_definition_folder_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/check_definition_folder_model_folders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/check_definition_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/check_definition_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/check_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22351 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/check_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/check_result_entry_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/check_result_sort_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/check_result_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5386 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/check_results_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7726 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/check_results_overview_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/check_run_schedule_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12440 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/check_search_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/check_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/check_target_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8642 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/check_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/check_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/check_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10325 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/cloud_synchronization_folders_status_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/collect_statistics_on_table_queue_job_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/collect_statistics_queue_job_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/collect_statistics_queue_job_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/collect_statistics_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14850 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_accepted_values_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_accepted_values_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_accepted_values_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_accepted_values_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15128 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_accepted_values_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_accepted_values_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16655 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_accepted_values_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_accepted_values_monthly_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14997 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_accepted_values_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_accepted_values_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_accepted_values_text_found_in_set_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10945 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_accuracy_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_accuracy_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11425 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_accuracy_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_accuracy_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11240 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_accuracy_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_accuracy_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10794 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_accuracy_total_average_match_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_accuracy_total_average_match_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10720 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_accuracy_total_max_match_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_accuracy_total_max_match_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10720 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_accuracy_total_min_match_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_accuracy_total_min_match_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10853 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_accuracy_total_not_null_count_match_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_accuracy_total_not_null_count_match_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10720 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_accuracy_total_sum_match_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_accuracy_total_sum_match_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22723 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_anomaly_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_anomaly_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27374 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_anomaly_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_anomaly_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23256 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_anomaly_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_anomaly_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_bool_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_bool_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_bool_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_bool_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_bool_false_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_bool_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_bool_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_bool_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_bool_monthly_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_bool_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_bool_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_bool_true_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_column_exists_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_column_type_hash_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10518 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_comparison_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_comparison_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11855 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_comparison_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_comparison_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_comparison_max_match_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_comparison_mean_match_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_comparison_min_match_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9735 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_comparison_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10800 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_comparison_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_comparison_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12139 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_comparison_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_comparison_monthly_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10579 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_comparison_not_null_count_match_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10535 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_comparison_null_count_match_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_comparison_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_comparison_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_comparison_sum_match_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9827 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_conversions_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_conversions_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10648 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_conversions_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_conversions_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9997 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_conversions_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_conversions_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10862 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_conversions_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_conversions_monthly_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_conversions_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_conversions_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9171 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_current_data_quality_status_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_current_data_quality_status_model_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_current_data_quality_status_model_dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9810 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_custom_sql_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_custom_sql_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10653 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_custom_sql_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_custom_sql_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9980 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_custom_sql_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_custom_sql_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10835 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_custom_sql_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_custom_sql_monthly_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9809 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_custom_sql_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_custom_sql_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20452 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_daily_monitoring_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_daily_monitoring_check_categories_spec_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_daily_monitoring_check_categories_spec_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18781 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_daily_partitioned_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_daily_partitioned_check_categories_spec_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_daily_partitioned_check_categories_spec_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_datatype_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_datatype_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_datatype_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_datatype_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10250 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_datatype_detected_datatype_in_text_changed_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_datatype_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_datatype_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_datatype_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_datatype_monthly_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6281 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_datatype_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_datatype_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_datatype_string_datatype_detect_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10569 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_date_in_range_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_date_in_range_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10767 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_date_values_in_future_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_datetime_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_datetime_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8372 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_datetime_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_datetime_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_datetime_date_values_in_future_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7763 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_datetime_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_datetime_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8506 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_datetime_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_datetime_monthly_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_datetime_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_datetime_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_default_checks_pattern_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10307 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_detected_datatype_in_text_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11810 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_distinct_count_anomaly_differencing_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11785 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_distinct_count_anomaly_stationary_partition_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10713 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_distinct_count_change_1_day_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10771 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_distinct_count_change_30_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10742 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_distinct_count_change_7_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10579 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_distinct_count_change_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10012 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_distinct_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11739 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_distinct_percent_anomaly_stationary_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_distinct_percent_change_1_day_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10797 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_distinct_percent_change_30_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10768 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_distinct_percent_change_7_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10605 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_distinct_percent_change_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10616 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_distinct_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10531 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_duplicate_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10589 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_duplicate_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10759 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_expected_numbers_in_use_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10803 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_expected_text_values_in_use_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10776 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_expected_texts_in_top_values_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9969 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_false_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10720 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_integer_in_range_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_integrity_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_integrity_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6528 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_integrity_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_integrity_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10819 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_integrity_foreign_key_match_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_integrity_foreign_key_match_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_integrity_foreign_key_not_match_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10528 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_integrity_lookup_key_not_found_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_integrity_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_integrity_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_integrity_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_integrity_monthly_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_integrity_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_integrity_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10704 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_invalid_email_format_found_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10762 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_invalid_email_format_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_invalid_ip_4_address_format_found_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_invalid_ip_6_address_format_found_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10630 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_invalid_latitude_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10643 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_invalid_longitude_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10691 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_invalid_uuid_format_found_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17399 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11607 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_max_anomaly_differencing_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11510 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_max_anomaly_stationary_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_max_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11523 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_mean_anomaly_stationary_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10523 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_mean_change_1_day_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10581 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_mean_change_30_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10552 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_mean_change_7_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10389 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_mean_change_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9879 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_mean_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11549 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_median_anomaly_stationary_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10549 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_median_change_1_day_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_median_change_30_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10578 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_median_change_7_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10415 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_median_change_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9905 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_median_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11607 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_min_anomaly_differencing_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11510 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_min_anomaly_stationary_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_min_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_monitoring_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19879 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_monthly_monitoring_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_monthly_monitoring_check_categories_spec_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_monthly_monitoring_check_categories_spec_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18220 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_monthly_partitioned_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_monthly_partitioned_check_categories_spec_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_monthly_partitioned_check_categories_spec_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10480 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_negative_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_negative_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_non_negative_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10596 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_non_negative_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9900 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_not_nulls_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_not_nulls_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_null_percent_anomaly_stationary_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10641 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_null_percent_change_1_day_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10699 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_null_percent_change_30_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_null_percent_change_7_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10507 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_null_percent_change_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10425 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_nulls_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14733 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_nulls_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_nulls_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16920 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_nulls_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_nulls_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7474 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_nulls_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_nulls_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_nulls_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_nulls_monthly_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_nulls_not_nulls_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_nulls_not_nulls_count_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_nulls_not_nulls_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_nulls_not_nulls_percent_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_nulls_nulls_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_nulls_nulls_count_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_nulls_nulls_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_nulls_nulls_percent_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10483 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_nulls_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15004 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_nulls_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_nulls_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_nulls_statistics_collectors_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10686 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_number_above_max_value_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10772 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_number_above_max_value_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10686 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_number_below_min_value_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10772 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_number_below_min_value_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_number_found_in_set_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10707 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_number_in_range_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40287 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47758 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_expected_numbers_in_use_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_integer_in_range_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_invalid_latitude_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_invalid_longitude_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_max_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_mean_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_median_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_min_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42487 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49106 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_monthly_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_negative_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_negative_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_non_negative_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_non_negative_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_number_above_max_value_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_number_above_max_value_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_number_below_min_value_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_number_below_min_value_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_number_found_in_set_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_number_in_range_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_percentile_10_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_percentile_25_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_percentile_75_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_percentile_90_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_percentile_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_population_stddev_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_population_variance_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42302 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_sample_stddev_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_sample_variance_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_sum_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_valid_latitude_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_numeric_valid_longitude_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_partitioned_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21457 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_patterns_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_patterns_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23750 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_patterns_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_patterns_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_patterns_invalid_email_format_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_patterns_invalid_email_format_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_patterns_invalid_ip_4_address_format_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_patterns_invalid_ip_6_address_format_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_patterns_invalid_uuid_format_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21923 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_patterns_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_patterns_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24282 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_patterns_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_patterns_monthly_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21738 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_patterns_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_patterns_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_patterns_text_matching_date_pattern_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_patterns_text_matching_name_pattern_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_patterns_text_not_matching_date_pattern_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_patterns_text_not_matching_regex_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_patterns_texts_matching_regex_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_patterns_valid_uuid_format_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_percentile_10_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_percentile_25_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_percentile_75_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_percentile_90_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_percentile_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10608 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_pii_contains_email_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_pii_contains_email_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10573 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_pii_contains_ip_4_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_pii_contains_ip_4_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10573 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_pii_contains_ip_6_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_pii_contains_ip_6_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10652 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_pii_contains_usa_phone_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_pii_contains_usa_phone_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10718 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_pii_contains_usa_zipcode_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_pii_contains_usa_zipcode_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10186 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_pii_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_pii_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11497 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_pii_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_pii_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10534 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_pii_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_pii_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11725 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_pii_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_pii_monthly_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10411 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_pii_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_pii_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10084 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_population_stddev_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10110 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_population_variance_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19300 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_profiling_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_profiling_check_categories_spec_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_profiling_check_categories_spec_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_range_max_value_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_range_max_value_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_range_median_value_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_range_min_value_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_range_min_value_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_range_statistics_collectors_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_range_sum_value_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_sample_stddev_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_sample_variance_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_sampling_column_samples_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_sampling_column_samples_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_sampling_statistics_collectors_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9784 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_schema_column_exists_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_schema_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_schema_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_schema_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_schema_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_schema_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_schema_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9919 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_schema_type_changed_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9687 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_sql_aggregate_expression_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_sql_aggregated_expression_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10548 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_sql_condition_failed_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_sql_condition_failed_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10674 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_sql_condition_passed_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_sql_condition_passed_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_sql_import_custom_result_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_sql_import_custom_result_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6749 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_statistics_collectors_root_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8114 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_statistics_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_strings_expected_text_values_in_use_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_strings_expected_texts_in_top_values_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11607 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_sum_anomaly_differencing_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_sum_anomaly_stationary_partition_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10510 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_sum_change_1_day_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10568 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_sum_change_30_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10539 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_sum_change_7_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_sum_change_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_sum_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14842 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16767 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10805 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_found_in_set_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_length_above_max_length_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_length_above_max_length_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_length_below_min_length_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_length_below_min_length_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10740 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_length_in_range_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_match_date_format_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_match_date_format_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10832 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_matching_date_pattern_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10832 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_matching_name_pattern_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_max_length_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9984 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_mean_length_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_min_length_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15200 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17161 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_monthly_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10778 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_not_matching_date_pattern_found_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10735 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_not_matching_regex_found_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10814 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_parsable_to_boolean_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_parsable_to_date_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10788 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_parsable_to_float_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10814 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_parsable_to_integer_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15077 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_statistics_collectors_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_text_datatype_detect_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_text_length_above_max_length_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_text_length_above_max_length_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_text_length_below_min_length_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_text_length_below_min_length_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_text_length_in_range_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_text_max_length_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_text_max_length_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_text_mean_length_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_text_mean_length_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_text_min_length_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_text_min_length_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_text_parsable_to_boolean_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_text_parsable_to_date_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_text_parsable_to_float_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_text_parsable_to_integer_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_text_valid_country_code_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_text_valid_currency_code_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10801 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_valid_country_code_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10814 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_text_valid_currency_code_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10802 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_texts_matching_regex_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9956 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_true_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_type_snapshot_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23392 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_uniqueness_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_uniqueness_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26847 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_uniqueness_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_uniqueness_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_uniqueness_distinct_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_uniqueness_distinct_count_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_uniqueness_distinct_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_uniqueness_distinct_percent_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_uniqueness_duplicate_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_uniqueness_duplicate_count_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_uniqueness_duplicate_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_uniqueness_duplicate_percent_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_uniqueness_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_uniqueness_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12425 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_uniqueness_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_uniqueness_monthly_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23959 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_uniqueness_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_uniqueness_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_uniqueness_statistics_collectors_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10702 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_valid_latitude_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10715 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_valid_longitude_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10763 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_valid_uuid_format_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_whitespace_blank_null_placeholder_text_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_whitespace_blank_null_placeholder_text_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15940 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_whitespace_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_whitespace_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17913 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_whitespace_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_whitespace_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_whitespace_empty_text_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10589 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_whitespace_empty_text_found_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10647 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_whitespace_empty_text_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_whitespace_empty_text_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_whitespace_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_whitespace_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18227 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_whitespace_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_whitespace_monthly_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10812 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_whitespace_null_placeholder_text_found_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10870 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_whitespace_null_placeholder_text_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16229 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_whitespace_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_whitespace_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_whitespace_text_surrounded_by_whitespace_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10866 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_whitespace_text_surrounded_by_whitespace_found_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10924 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_whitespace_text_surrounded_by_whitespace_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_whitespace_text_surrounded_by_whitespace_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_whitespace_whitespace_text_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10716 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_whitespace_whitespace_text_found_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10774 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_whitespace_whitespace_text_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/column_whitespace_whitespace_text_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/comment_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/common_column_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/compare_thresholds_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/comparison_check_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/compression_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6267 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/connection_incident_grouping_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22688 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/connection_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16568 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/connection_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/connection_specification_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/connection_test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/connection_test_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/count_between_rule_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/credential_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/csv_file_format_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10788 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/custom_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/custom_rule_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/custom_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/dashboard_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/dashboard_spec_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/dashboards_folder_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/data_delete_result_partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/data_dictionary_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/data_dictionary_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/data_grouping_configuration_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4876 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/data_grouping_configuration_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/data_grouping_configuration_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/data_grouping_configuration_trimmed_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/data_grouping_dimension_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/data_grouping_dimension_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/data_type_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/databricks_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/databricks_parameters_spec_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/datetime_built_in_date_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/default_column_checks_pattern_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/default_column_checks_pattern_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/default_schedules_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/default_table_checks_pattern_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/default_table_checks_pattern_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11837 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/delete_stored_data_queue_job_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/delete_stored_data_queue_job_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/delete_stored_data_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/delete_stored_data_result_partition_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/detected_datatype_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/detected_datatype_equals_rule_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7659 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/dimension_current_data_quality_status_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/display_hint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/dqo_cloud_user_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/dqo_job_change_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16949 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/dqo_job_entry_parameters_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/dqo_job_history_entry_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/dqo_job_queue_incremental_snapshot_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/dqo_job_queue_initial_snapshot_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/dqo_job_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/dqo_job_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/dqo_queue_job_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/dqo_root.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/dqo_settings_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/dqo_settings_model_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/dqo_settings_model_properties_additional_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14643 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/dqo_user_profile_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/dqo_user_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/duckdb_files_format_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10263 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/duckdb_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/duckdb_parameters_spec_directories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/duckdb_parameters_spec_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/duckdb_read_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/duckdb_storage_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/effective_schedule_level_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/effective_schedule_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/equals_1_rule_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/equals_integer_rule_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8316 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/error_entry_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/errors_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/external_log_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/field_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/file_format_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/file_synchronization_direction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/folder_synchronization_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/hierarchy_id_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/hierarchy_id_model_path_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/historic_data_points_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/import_schema_queue_job_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/import_severity_rule_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/import_tables_queue_job_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/import_tables_queue_job_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/import_tables_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/incident_daily_issues_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/incident_grouping_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/incident_issue_histogram_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/incident_issue_histogram_model_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/incident_issue_histogram_model_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/incident_issue_histogram_model_days.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9890 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/incident_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/incident_sort_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/incident_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/incident_webhook_notifications_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/incidents_per_connection_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7404 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/json_file_format_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/json_format_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/json_records_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/label_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/max_count_rule_0_error_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/max_count_rule_0_warning_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/max_count_rule_100_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/max_days_rule_1_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/max_days_rule_2_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/max_days_rule_7_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/max_diff_percent_rule_0_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/max_diff_percent_rule_1_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/max_diff_percent_rule_5_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/max_failures_rule_0_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/max_failures_rule_1_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/max_failures_rule_5_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/max_missing_rule_0_error_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/max_missing_rule_0_warning_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/max_missing_rule_2_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/max_percent_rule_0_error_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/max_percent_rule_0_warning_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/max_percent_rule_5_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/min_count_rule_1_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/min_percent_rule_100_error_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/min_percent_rule_100_warning_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/min_percent_rule_95_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/minimum_grouping_severity_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/monitoring_schedule_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/mono.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/mono_dqo_queue_job_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/mono_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/mono_void.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/my_sql_ssl_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/mysql_engine_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/mysql_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/mysql_parameters_spec_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/new_line_character_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/optional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/optional_incident_webhook_notifications_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/optional_monitoring_schedule_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/oracle_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/oracle_parameters_spec_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/parameter_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/parameter_definition_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/parquet_file_format_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/partition_incremental_time_window_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/physical_table_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/postgresql_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/postgresql_parameters_spec_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/postgresql_ssl_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/presto_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/presto_parameters_spec_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/profiling_time_period_truncation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/provider_sensor_definition_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/provider_sensor_definition_spec_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/provider_sensor_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/provider_sensor_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/provider_sensor_runner_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/provider_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6239 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/quality_category_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/redshift_authentication_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5363 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/redshift_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/redshift_parameters_spec_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/remote_table_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/repair_stored_data_queue_job_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/rule_folder_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/rule_folder_model_folders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/rule_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8052 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/rule_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/rule_model_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/rule_parameters_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/rule_runner_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/rule_severity_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/rule_thresholds_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/rule_time_window_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/rule_time_window_settings_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/run_checks_on_table_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/run_checks_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/run_checks_queue_job_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/run_checks_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/schedule_enabled_status_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13462 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/schema_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/schema_remote_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5648 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/sensor_definition_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/sensor_definition_spec_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/sensor_folder_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/sensor_folder_model_folders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/sensor_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/sensor_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7283 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/sensor_readout_entry_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/sensor_readouts_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/shared_credential_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/shared_credential_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/similar_check_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/single_store_db_load_balancing_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/single_store_db_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/snowflake_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/snowflake_parameters_spec_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/sort_direction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/spark_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/spark_parameters_spec_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/spring_error_payload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/sql_server_authentication_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/sql_server_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/sql_server_parameters_spec_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9359 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/statistics_collector_search_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/statistics_collector_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/statistics_data_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/statistics_metric_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/statistics_metric_model_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/statistics_result_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8752 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/synchronize_multiple_folders_dqo_queue_job_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/synchronize_multiple_folders_queue_job_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/synchronize_root_folder_dqo_queue_job_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/synchronize_root_folder_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_accuracy_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_accuracy_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_accuracy_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_accuracy_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_accuracy_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_accuracy_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10823 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_accuracy_total_row_count_match_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_accuracy_total_row_count_match_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10317 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_availability_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_availability_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_availability_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_availability_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_availability_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_availability_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_availability_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_availability_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_column_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_column_list_ordered_hash_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_column_list_unordered_hash_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_column_types_hash_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_columns_statistics_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_comparison_column_count_match_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_comparison_column_results_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_comparison_column_results_model_column_comparison_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9448 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_comparison_configuration_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7836 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_comparison_configuration_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_comparison_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_comparison_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_comparison_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_comparison_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_comparison_grouping_column_pair_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_comparison_grouping_columns_pair_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16678 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_comparison_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_comparison_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_comparison_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_comparison_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_comparison_monthly_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_comparison_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_comparison_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_comparison_results_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_comparison_results_model_column_comparison_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_comparison_results_model_table_comparison_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10479 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_comparison_row_count_match_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12081 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_current_data_quality_status_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_current_data_quality_status_model_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_current_data_quality_status_model_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_current_data_quality_status_model_dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9671 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_custom_sql_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_custom_sql_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10536 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_custom_sql_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_custom_sql_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9863 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_custom_sql_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_custom_sql_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10706 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_custom_sql_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_custom_sql_monthly_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_custom_sql_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_custom_sql_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9780 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_daily_monitoring_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_daily_monitoring_check_categories_spec_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_daily_monitoring_check_categories_spec_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_daily_partitioned_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_daily_partitioned_check_categories_spec_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_daily_partitioned_check_categories_spec_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10225 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_data_freshness_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_data_ingestion_delay_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10225 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_data_staleness_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5907 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_default_checks_pattern_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_incident_grouping_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22643 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_monitoring_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_monthly_monitoring_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_monthly_monitoring_check_categories_spec_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_monthly_monitoring_check_categories_spec_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_monthly_partitioned_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_monthly_partitioned_check_categories_spec_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_monthly_partitioned_check_categories_spec_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_owner_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_partition_reload_lag_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_partitioned_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_partitioning_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10183 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_profiling_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_profiling_check_categories_spec_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_profiling_check_categories_spec_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11656 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_row_count_anomaly_differencing_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11631 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_row_count_anomaly_stationary_partition_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10559 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_row_count_change_1_day_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10617 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_row_count_change_30_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_row_count_change_7_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10425 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_row_count_change_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9795 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_row_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9918 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_schema_column_count_changed_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9896 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_schema_column_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_schema_column_count_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_schema_column_list_changed_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10068 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_schema_column_list_or_order_changed_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_schema_column_types_changed_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9710 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_schema_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_schema_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10040 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_schema_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_schema_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9877 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_schema_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_schema_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_schema_statistics_collectors_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19622 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_spec_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_spec_groupings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_spec_table_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10049 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_sql_aggregate_expression_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_sql_aggregated_expression_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10521 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_sql_condition_failed_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_sql_condition_failed_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10661 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_sql_condition_passed_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_sql_condition_passed_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10049 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_sql_import_custom_result_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_sql_import_custom_result_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_statistics_collectors_root_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_statistics_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_timeliness_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_timeliness_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_timeliness_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_timeliness_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_timeliness_data_freshness_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_timeliness_data_ingestion_delay_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_timeliness_data_staleness_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_timeliness_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_timeliness_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_timeliness_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_timeliness_monthly_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_timeliness_partition_reload_lag_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6387 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_timeliness_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_timeliness_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10418 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_volume_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_volume_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12139 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_volume_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_volume_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_volume_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_volume_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_volume_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_volume_monthly_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_volume_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_volume_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_volume_row_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_volume_row_count_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/table_volume_statistics_collectors_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/target_column_pattern_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/target_table_pattern_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/temporal_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/text_built_in_date_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/time_period_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11573 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/time_window_filter_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/timestamp_columns_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/trino_engine_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7807 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/trino_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/trino_parameters_spec_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/models/value_changed_rule_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/client/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7486 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/startdqo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-25 11:58:27.000000 dqops-1.2.0/dqops/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:11:50.504365 dqops-1.2.0/dqops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-04-25 12:11:49.000000 dqops-1.2.0/dqops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    78724 2024-04-25 12:11:50.000000 dqops-1.2.0/dqops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 12:11:49.000000 dqops-1.2.0/dqops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-25 12:11:49.000000 dqops-1.2.0/dqops.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-25 12:11:49.000000 dqops-1.2.0/dqops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 12:11:49.000000 dqops-1.2.0/dqops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-25 11:58:27.000000 dqops-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-25 12:11:50.504365 dqops-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-04-25 11:58:27.000000 dqops-1.2.0/setup.py
```

### Comparing `dqops-1.1.0/LICENSE` & `dqops-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/PKG-INFO` & `dqops-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dqops
-Version: 1.1.0
+Version: 1.2.0
 Summary: DQOps Data Quality Operations Center
 Home-page: https://github.com/dqops/dqo/tree/master/distribution/python
 Author: DQOps Developers
 Author-email: support@dqops.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `dqops-1.1.0/README.md` & `dqops-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/__init__.py` & `dqops-1.2.0/dqops/__init__.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/__main__.py` & `dqops-1.2.0/dqops/__main__.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/check_results/get_column_monitoring_checks_results.py` & `dqops-1.2.0/dqops/client/api/check_results/get_column_monitoring_checks_results.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/check_results/get_column_partitioned_checks_results.py` & `dqops-1.2.0/dqops/client/api/check_results/get_column_partitioned_checks_results.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/check_results/get_column_profiling_checks_results.py` & `dqops-1.2.0/dqops/client/api/check_results/get_column_profiling_checks_results.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/check_results/get_table_data_quality_status.py` & `dqops-1.2.0/dqops/client/api/check_results/get_table_data_quality_status.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/check_results/get_table_monitoring_checks_results.py` & `dqops-1.2.0/dqops/client/api/check_results/get_table_monitoring_checks_results.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/check_results/get_table_partitioned_checks_results.py` & `dqops-1.2.0/dqops/client/api/check_results/get_table_partitioned_checks_results.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/check_results/get_table_profiling_checks_results.py` & `dqops-1.2.0/dqops/client/api/check_results/get_table_profiling_checks_results.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/check_results_overview/get_column_monitoring_checks_overview.py` & `dqops-1.2.0/dqops/client/api/check_results_overview/get_column_monitoring_checks_overview.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/check_results_overview/get_column_partitioned_checks_overview.py` & `dqops-1.2.0/dqops/client/api/check_results_overview/get_column_partitioned_checks_overview.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/check_results_overview/get_column_profiling_checks_overview.py` & `dqops-1.2.0/dqops/client/api/check_results_overview/get_column_profiling_checks_overview.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/check_results_overview/get_table_monitoring_checks_overview.py` & `dqops-1.2.0/dqops/client/api/check_results_overview/get_table_monitoring_checks_overview.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/check_results_overview/get_table_partitioned_checks_overview.py` & `dqops-1.2.0/dqops/client/api/check_results_overview/get_table_partitioned_checks_overview.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/check_results_overview/get_table_profiling_checks_overview.py` & `dqops-1.2.0/dqops/client/api/check_results_overview/get_table_profiling_checks_overview.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/checks/create_check.py` & `dqops-1.2.0/dqops/client/api/checks/create_check.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/checks/delete_check.py` & `dqops-1.2.0/dqops/client/api/checks/delete_check.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/checks/get_all_checks.py` & `dqops-1.2.0/dqops/client/api/checks/get_all_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/checks/get_check.py` & `dqops-1.2.0/dqops/client/api/checks/get_check.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/checks/get_check_folder_tree.py` & `dqops-1.2.0/dqops/client/api/checks/get_check_folder_tree.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/checks/update_check.py` & `dqops-1.2.0/dqops/client/api/checks/update_check.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/columns/create_column.py` & `dqops-1.2.0/dqops/client/api/columns/create_column.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/columns/delete_column.py` & `dqops-1.2.0/dqops/client/api/columns/delete_column.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/columns/get_column.py` & `dqops-1.2.0/dqops/client/api/columns/get_column.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/columns/get_column_basic.py` & `dqops-1.2.0/dqops/client/api/columns/get_column_basic.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/columns/get_column_comments.py` & `dqops-1.2.0/dqops/client/api/columns/get_column_comments.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/columns/get_column_labels.py` & `dqops-1.2.0/dqops/client/api/columns/get_column_labels.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/columns/get_column_monitoring_checks_basic_model.py` & `dqops-1.2.0/dqops/client/api/columns/get_column_monitoring_checks_basic_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/columns/get_column_monitoring_checks_daily.py` & `dqops-1.2.0/dqops/client/api/columns/get_column_monitoring_checks_daily.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/columns/get_column_monitoring_checks_model.py` & `dqops-1.2.0/dqops/client/api/columns/get_column_monitoring_checks_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/columns/get_column_monitoring_checks_model_filter.py` & `dqops-1.2.0/dqops/client/api/columns/get_column_monitoring_checks_model_filter.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/columns/get_column_monitoring_checks_monthly.py` & `dqops-1.2.0/dqops/client/api/columns/get_column_monitoring_checks_monthly.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/columns/get_column_partitioned_checks_basic_model.py` & `dqops-1.2.0/dqops/client/api/columns/get_column_partitioned_checks_basic_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/columns/get_column_partitioned_checks_daily.py` & `dqops-1.2.0/dqops/client/api/columns/get_column_partitioned_checks_daily.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/columns/get_column_partitioned_checks_model.py` & `dqops-1.2.0/dqops/client/api/columns/get_column_partitioned_checks_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/columns/get_column_partitioned_checks_model_filter.py` & `dqops-1.2.0/dqops/client/api/columns/get_column_partitioned_checks_model_filter.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/columns/get_column_partitioned_checks_monthly.py` & `dqops-1.2.0/dqops/client/api/columns/get_column_partitioned_checks_monthly.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/columns/get_column_profiling_checks.py` & `dqops-1.2.0/dqops/client/api/columns/get_column_profiling_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/columns/get_column_profiling_checks_basic_model.py` & `dqops-1.2.0/dqops/client/api/columns/get_column_profiling_checks_basic_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/columns/get_column_profiling_checks_model.py` & `dqops-1.2.0/dqops/client/api/columns/get_column_profiling_checks_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/columns/get_column_profiling_checks_model_filter.py` & `dqops-1.2.0/dqops/client/api/columns/get_column_profiling_checks_model_filter.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/columns/get_column_statistics.py` & `dqops-1.2.0/dqops/client/api/columns/get_column_statistics.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/columns/get_columns.py` & `dqops-1.2.0/dqops/client/api/columns/get_columns.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/columns/get_columns_statistics.py` & `dqops-1.2.0/dqops/client/api/columns/get_columns_statistics.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/columns/update_column.py` & `dqops-1.2.0/dqops/client/api/columns/update_column.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/columns/update_column_basic.py` & `dqops-1.2.0/dqops/client/api/columns/update_column_basic.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/columns/update_column_comments.py` & `dqops-1.2.0/dqops/client/api/columns/update_column_comments.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/columns/update_column_labels.py` & `dqops-1.2.0/dqops/client/api/columns/update_column_labels.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/columns/update_column_monitoring_checks_daily.py` & `dqops-1.2.0/dqops/client/api/columns/update_column_monitoring_checks_daily.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/columns/update_column_monitoring_checks_model.py` & `dqops-1.2.0/dqops/client/api/columns/update_column_monitoring_checks_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/columns/update_column_monitoring_checks_monthly.py` & `dqops-1.2.0/dqops/client/api/columns/update_column_monitoring_checks_monthly.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/columns/update_column_partitioned_checks_daily.py` & `dqops-1.2.0/dqops/client/api/columns/update_column_partitioned_checks_daily.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/columns/update_column_partitioned_checks_model.py` & `dqops-1.2.0/dqops/client/api/columns/update_column_partitioned_checks_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/columns/update_column_partitioned_checks_monthly.py` & `dqops-1.2.0/dqops/client/api/columns/update_column_partitioned_checks_monthly.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/columns/update_column_profiling_checks.py` & `dqops-1.2.0/dqops/client/api/columns/update_column_profiling_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/columns/update_column_profiling_checks_model.py` & `dqops-1.2.0/dqops/client/api/columns/update_column_profiling_checks_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/connections/bulk_activate_connection_checks.py` & `dqops-1.2.0/dqops/client/api/connections/bulk_activate_connection_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/connections/bulk_deactivate_connection_checks.py` & `dqops-1.2.0/dqops/client/api/connections/bulk_deactivate_connection_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/connections/create_connection.py` & `dqops-1.2.0/dqops/client/api/connections/create_connection.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/connections/create_connection_basic.py` & `dqops-1.2.0/dqops/client/api/connections/create_connection_basic.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/connections/delete_connection.py` & `dqops-1.2.0/dqops/client/api/connections/delete_connection.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/connections/get_all_connections.py` & `dqops-1.2.0/dqops/client/api/connections/get_all_connections.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/connections/get_connection.py` & `dqops-1.2.0/dqops/client/api/connections/get_connection.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/connections/get_connection_basic.py` & `dqops-1.2.0/dqops/client/api/connections/get_connection_basic.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/connections/get_connection_comments.py` & `dqops-1.2.0/dqops/client/api/connections/get_connection_comments.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/connections/get_connection_common_columns.py` & `dqops-1.2.0/dqops/client/api/connections/get_connection_common_columns.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/connections/get_connection_default_grouping_configuration.py` & `dqops-1.2.0/dqops/client/api/connections/get_connection_default_grouping_configuration.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/connections/get_connection_incident_grouping.py` & `dqops-1.2.0/dqops/client/api/connections/get_connection_incident_grouping.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/connections/get_connection_labels.py` & `dqops-1.2.0/dqops/client/api/connections/get_connection_labels.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/connections/get_connection_scheduling_group.py` & `dqops-1.2.0/dqops/client/api/connections/get_connection_scheduling_group.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/connections/update_connection.py` & `dqops-1.2.0/dqops/client/api/connections/update_connection.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/connections/update_connection_basic.py` & `dqops-1.2.0/dqops/client/api/connections/update_connection_basic.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/connections/update_connection_comments.py` & `dqops-1.2.0/dqops/client/api/connections/update_connection_comments.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/connections/update_connection_default_grouping_configuration.py` & `dqops-1.2.0/dqops/client/api/connections/update_connection_default_grouping_configuration.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/connections/update_connection_incident_grouping.py` & `dqops-1.2.0/dqops/client/api/connections/update_connection_incident_grouping.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/connections/update_connection_labels.py` & `dqops-1.2.0/dqops/client/api/connections/update_connection_labels.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/connections/update_connection_scheduling_group.py` & `dqops-1.2.0/dqops/client/api/connections/update_connection_scheduling_group.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/dashboards/get_all_dashboards.py` & `dqops-1.2.0/dqops/client/api/dashboards/get_all_dashboards.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/dashboards/get_dashboard_level_1.py` & `dqops-1.2.0/dqops/client/api/dashboards/get_dashboard_level_1.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/dashboards/get_dashboard_level_2.py` & `dqops-1.2.0/dqops/client/api/dashboards/get_dashboard_level_2.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/dashboards/get_dashboard_level_3.py` & `dqops-1.2.0/dqops/client/api/dashboards/get_dashboard_level_3.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/dashboards/get_dashboard_level_4.py` & `dqops-1.2.0/dqops/client/api/dashboards/get_dashboard_level_4.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/dashboards/get_dashboard_level_5.py` & `dqops-1.2.0/dqops/client/api/dashboards/get_dashboard_level_5.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/data_grouping_configurations/create_table_grouping_configuration.py` & `dqops-1.2.0/dqops/client/api/data_grouping_configurations/create_table_grouping_configuration.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/data_grouping_configurations/delete_table_grouping_configuration.py` & `dqops-1.2.0/dqops/client/api/data_grouping_configurations/delete_table_grouping_configuration.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/data_grouping_configurations/get_table_grouping_configuration.py` & `dqops-1.2.0/dqops/client/api/data_grouping_configurations/get_table_grouping_configuration.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/data_grouping_configurations/get_table_grouping_configurations.py` & `dqops-1.2.0/dqops/client/api/data_grouping_configurations/get_table_grouping_configurations.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/data_grouping_configurations/set_table_default_grouping_configuration.py` & `dqops-1.2.0/dqops/client/api/data_grouping_configurations/set_table_default_grouping_configuration.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/data_grouping_configurations/update_table_grouping_configuration.py` & `dqops-1.2.0/dqops/client/api/data_grouping_configurations/update_table_grouping_configuration.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/data_sources/get_remote_data_source_schemas.py` & `dqops-1.2.0/dqops/client/api/data_sources/get_remote_data_source_schemas.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/data_sources/get_remote_data_source_tables.py` & `dqops-1.2.0/dqops/client/api/data_sources/get_remote_data_source_tables.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/data_sources/test_connection.py` & `dqops-1.2.0/dqops/client/api/data_sources/test_connection.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/default_column_check_patterns/create_default_column_checks_pattern.py` & `dqops-1.2.0/dqops/client/api/default_column_check_patterns/create_default_column_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/default_column_check_patterns/create_default_column_checks_pattern_target.py` & `dqops-1.2.0/dqops/client/api/default_column_check_patterns/create_default_column_checks_pattern_target.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/default_column_check_patterns/delete_default_column_checks_pattern.py` & `dqops-1.2.0/dqops/client/api/default_column_check_patterns/delete_default_column_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/default_column_check_patterns/get_all_default_column_checks_patterns.py` & `dqops-1.2.0/dqops/client/api/default_column_check_patterns/get_all_default_column_checks_patterns.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/default_column_check_patterns/get_default_column_checks_pattern.py` & `dqops-1.2.0/dqops/client/api/default_column_check_patterns/get_default_column_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/default_column_check_patterns/get_default_column_checks_pattern_target.py` & `dqops-1.2.0/dqops/client/api/default_column_check_patterns/get_default_column_checks_pattern_target.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/default_column_check_patterns/get_default_monitoring_daily_column_checks_pattern.py` & `dqops-1.2.0/dqops/client/api/default_column_check_patterns/get_default_monitoring_daily_column_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/default_column_check_patterns/get_default_monitoring_monthly_column_checks_pattern.py` & `dqops-1.2.0/dqops/client/api/default_column_check_patterns/get_default_monitoring_monthly_column_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/default_column_check_patterns/get_default_partitioned_daily_column_checks_pattern.py` & `dqops-1.2.0/dqops/client/api/default_column_check_patterns/get_default_partitioned_daily_column_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/default_column_check_patterns/get_default_partitioned_monthly_column_checks_pattern.py` & `dqops-1.2.0/dqops/client/api/default_column_check_patterns/get_default_partitioned_monthly_column_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/default_column_check_patterns/get_default_profiling_column_checks_pattern.py` & `dqops-1.2.0/dqops/client/api/default_column_check_patterns/get_default_profiling_column_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/default_column_check_patterns/update_default_column_checks_pattern.py` & `dqops-1.2.0/dqops/client/api/default_column_check_patterns/update_default_column_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/default_column_check_patterns/update_default_column_checks_pattern_target.py` & `dqops-1.2.0/dqops/client/api/default_column_check_patterns/update_default_column_checks_pattern_target.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/default_column_check_patterns/update_default_monitoring_daily_column_checks_pattern.py` & `dqops-1.2.0/dqops/client/api/default_column_check_patterns/update_default_monitoring_daily_column_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/default_column_check_patterns/update_default_monitoring_monthly_column_checks_pattern.py` & `dqops-1.2.0/dqops/client/api/default_column_check_patterns/update_default_monitoring_monthly_column_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/default_column_check_patterns/update_default_partitioned_daily_column_checks_pattern.py` & `dqops-1.2.0/dqops/client/api/default_column_check_patterns/update_default_partitioned_daily_column_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/default_column_check_patterns/update_default_partitioned_monthly_column_checks_pattern.py` & `dqops-1.2.0/dqops/client/api/default_column_check_patterns/update_default_partitioned_monthly_column_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/default_column_check_patterns/update_default_profiling_column_checks_pattern.py` & `dqops-1.2.0/dqops/client/api/default_column_check_patterns/update_default_profiling_column_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/default_table_check_patterns/create_default_table_checks_pattern.py` & `dqops-1.2.0/dqops/client/api/default_table_check_patterns/create_default_table_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/default_table_check_patterns/create_default_table_checks_pattern_target.py` & `dqops-1.2.0/dqops/client/api/default_table_check_patterns/create_default_table_checks_pattern_target.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/default_table_check_patterns/delete_default_table_checks_pattern.py` & `dqops-1.2.0/dqops/client/api/default_table_check_patterns/delete_default_table_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/default_table_check_patterns/get_all_default_table_checks_patterns.py` & `dqops-1.2.0/dqops/client/api/default_table_check_patterns/get_all_default_table_checks_patterns.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/default_table_check_patterns/get_default_monitoring_daily_table_checks_pattern.py` & `dqops-1.2.0/dqops/client/api/default_table_check_patterns/get_default_monitoring_daily_table_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/default_table_check_patterns/get_default_monitoring_monthly_table_checks_pattern.py` & `dqops-1.2.0/dqops/client/api/default_table_check_patterns/get_default_monitoring_monthly_table_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/default_table_check_patterns/get_default_partitioned_daily_table_checks_pattern.py` & `dqops-1.2.0/dqops/client/api/default_table_check_patterns/get_default_partitioned_daily_table_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/default_table_check_patterns/get_default_partitioned_monthly_table_checks_pattern.py` & `dqops-1.2.0/dqops/client/api/default_table_check_patterns/get_default_partitioned_monthly_table_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/default_table_check_patterns/get_default_profiling_table_checks_pattern.py` & `dqops-1.2.0/dqops/client/api/default_table_check_patterns/get_default_profiling_table_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/default_table_check_patterns/get_default_table_checks_pattern.py` & `dqops-1.2.0/dqops/client/api/default_table_check_patterns/get_default_table_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/default_table_check_patterns/get_default_table_checks_pattern_target.py` & `dqops-1.2.0/dqops/client/api/default_table_check_patterns/get_default_table_checks_pattern_target.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/default_table_check_patterns/update_default_monitoring_daily_table_checks_pattern.py` & `dqops-1.2.0/dqops/client/api/default_table_check_patterns/update_default_monitoring_daily_table_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/default_table_check_patterns/update_default_monitoring_monthly_table_checks_pattern.py` & `dqops-1.2.0/dqops/client/api/default_table_check_patterns/update_default_monitoring_monthly_table_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/default_table_check_patterns/update_default_partitioned_daily_table_checks_pattern.py` & `dqops-1.2.0/dqops/client/api/default_table_check_patterns/update_default_partitioned_daily_table_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/default_table_check_patterns/update_default_partitioned_monthly_table_checks_pattern.py` & `dqops-1.2.0/dqops/client/api/default_table_check_patterns/update_default_partitioned_monthly_table_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/default_table_check_patterns/update_default_profiling_table_checks_pattern.py` & `dqops-1.2.0/dqops/client/api/default_table_check_patterns/update_default_profiling_table_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/default_table_check_patterns/update_default_table_checks_pattern.py` & `dqops-1.2.0/dqops/client/api/default_table_check_patterns/update_default_table_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/default_table_check_patterns/update_default_table_checks_pattern_target.py` & `dqops-1.2.0/dqops/client/api/default_table_check_patterns/update_default_table_checks_pattern_target.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/defaults/get_default_schedule.py` & `dqops-1.2.0/dqops/client/api/defaults/get_default_schedule.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/defaults/get_default_webhooks.py` & `dqops-1.2.0/dqops/client/api/defaults/get_default_webhooks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/defaults/update_default_schedules.py` & `dqops-1.2.0/dqops/client/api/defaults/update_default_schedules.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/defaults/update_default_webhooks.py` & `dqops-1.2.0/dqops/client/api/defaults/update_default_webhooks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/dictionaries/create_dictionary.py` & `dqops-1.2.0/dqops/client/api/dictionaries/create_dictionary.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/dictionaries/delete_dictionary.py` & `dqops-1.2.0/dqops/client/api/dictionaries/delete_dictionary.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/dictionaries/download_dictionary.py` & `dqops-1.2.0/dqops/client/api/dictionaries/download_dictionary.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/dictionaries/get_all_dictionaries.py` & `dqops-1.2.0/dqops/client/api/dictionaries/get_all_dictionaries.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/dictionaries/get_dictionary.py` & `dqops-1.2.0/dqops/client/api/dictionaries/get_dictionary.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/dictionaries/update_dictionary.py` & `dqops-1.2.0/dqops/client/api/dictionaries/update_dictionary.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/environment/get_dqo_settings.py` & `dqops-1.2.0/dqops/client/api/environment/get_dqo_settings.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/environment/get_user_profile.py` & `dqops-1.2.0/dqops/client/api/environment/get_user_profile.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/environment/issue_api_key.py` & `dqops-1.2.0/dqops/client/api/environment/issue_api_key.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/errors/get_column_monitoring_errors.py` & `dqops-1.2.0/dqops/client/api/errors/get_column_monitoring_errors.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/errors/get_column_partitioned_errors.py` & `dqops-1.2.0/dqops/client/api/errors/get_column_partitioned_errors.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/errors/get_column_profiling_errors.py` & `dqops-1.2.0/dqops/client/api/errors/get_column_profiling_errors.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/errors/get_table_monitoring_errors.py` & `dqops-1.2.0/dqops/client/api/errors/get_table_monitoring_errors.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/errors/get_table_partitioned_errors.py` & `dqops-1.2.0/dqops/client/api/errors/get_table_partitioned_errors.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/errors/get_table_profiling_errors.py` & `dqops-1.2.0/dqops/client/api/errors/get_table_profiling_errors.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/healthcheck/is_healthy.py` & `dqops-1.2.0/dqops/client/api/healthcheck/is_healthy.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/incidents/find_connection_incident_stats.py` & `dqops-1.2.0/dqops/client/api/incidents/find_connection_incident_stats.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/incidents/find_recent_incidents_on_connection.py` & `dqops-1.2.0/dqops/client/api/incidents/find_recent_incidents_on_connection.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/incidents/get_incident.py` & `dqops-1.2.0/dqops/client/api/incidents/get_incident.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/incidents/get_incident_histogram.py` & `dqops-1.2.0/dqops/client/api/incidents/get_incident_histogram.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/incidents/get_incident_issues.py` & `dqops-1.2.0/dqops/client/api/incidents/get_incident_issues.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/incidents/set_incident_issue_url.py` & `dqops-1.2.0/dqops/client/api/incidents/set_incident_issue_url.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/incidents/set_incident_status.py` & `dqops-1.2.0/dqops/client/api/incidents/set_incident_status.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/jobs/cancel_job.py` & `dqops-1.2.0/dqops/client/api/jobs/cancel_job.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/jobs/collect_statistics_on_data_groups.py` & `dqops-1.2.0/dqops/client/api/jobs/collect_statistics_on_data_groups.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/jobs/collect_statistics_on_table.py` & `dqops-1.2.0/dqops/client/api/jobs/collect_statistics_on_table.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/jobs/delete_stored_data.py` & `dqops-1.2.0/dqops/client/api/jobs/delete_stored_data.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/jobs/get_all_jobs.py` & `dqops-1.2.0/dqops/client/api/jobs/get_all_jobs.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/jobs/get_job.py` & `dqops-1.2.0/dqops/client/api/jobs/get_job.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/jobs/get_job_changes_since.py` & `dqops-1.2.0/dqops/client/api/jobs/get_job_changes_since.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/jobs/import_tables.py` & `dqops-1.2.0/dqops/client/api/jobs/import_tables.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/jobs/is_cron_scheduler_running.py` & `dqops-1.2.0/dqops/client/api/jobs/is_cron_scheduler_running.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/jobs/run_checks.py` & `dqops-1.2.0/dqops/client/api/jobs/run_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/jobs/start_cron_scheduler.py` & `dqops-1.2.0/dqops/client/api/jobs/start_cron_scheduler.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/jobs/stop_cron_scheduler.py` & `dqops-1.2.0/dqops/client/api/jobs/stop_cron_scheduler.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/jobs/synchronize_folders.py` & `dqops-1.2.0/dqops/client/api/jobs/synchronize_folders.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/jobs/wait_for_job.py` & `dqops-1.2.0/dqops/client/api/jobs/wait_for_job.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/jobs/wait_for_run_checks_job.py` & `dqops-1.2.0/dqops/client/api/jobs/wait_for_run_checks_job.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/log_shipping/log_debug.py` & `dqops-1.2.0/dqops/client/api/log_shipping/log_debug.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/log_shipping/log_error.py` & `dqops-1.2.0/dqops/client/api/log_shipping/log_error.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/log_shipping/log_info.py` & `dqops-1.2.0/dqops/client/api/log_shipping/log_info.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/log_shipping/log_warn.py` & `dqops-1.2.0/dqops/client/api/log_shipping/log_warn.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/rules/create_rule.py` & `dqops-1.2.0/dqops/client/api/rules/create_rule.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/rules/delete_rule.py` & `dqops-1.2.0/dqops/client/api/rules/delete_rule.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/rules/get_all_rules.py` & `dqops-1.2.0/dqops/client/api/rules/get_all_rules.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/rules/get_rule.py` & `dqops-1.2.0/dqops/client/api/rules/get_rule.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/rules/get_rule_folder_tree.py` & `dqops-1.2.0/dqops/client/api/rules/get_rule_folder_tree.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/rules/update_rule.py` & `dqops-1.2.0/dqops/client/api/rules/update_rule.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/schemas/get_schema_monitoring_checks_model.py` & `dqops-1.2.0/dqops/client/api/schemas/get_schema_monitoring_checks_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/schemas/get_schema_monitoring_checks_templates.py` & `dqops-1.2.0/dqops/client/api/schemas/get_schema_monitoring_checks_templates.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/schemas/get_schema_partitioned_checks_model.py` & `dqops-1.2.0/dqops/client/api/schemas/get_schema_partitioned_checks_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/schemas/get_schema_partitioned_checks_templates.py` & `dqops-1.2.0/dqops/client/api/schemas/get_schema_partitioned_checks_templates.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/schemas/get_schema_profiling_checks_model.py` & `dqops-1.2.0/dqops/client/api/schemas/get_schema_profiling_checks_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/schemas/get_schema_profiling_checks_templates.py` & `dqops-1.2.0/dqops/client/api/schemas/get_schema_profiling_checks_templates.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/schemas/get_schemas.py` & `dqops-1.2.0/dqops/client/api/schemas/get_schemas.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/sensor_readouts/get_column_monitoring_sensor_readouts.py` & `dqops-1.2.0/dqops/client/api/sensor_readouts/get_column_monitoring_sensor_readouts.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/sensor_readouts/get_column_partitioned_sensor_readouts.py` & `dqops-1.2.0/dqops/client/api/sensor_readouts/get_column_partitioned_sensor_readouts.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/sensor_readouts/get_column_profiling_sensor_readouts.py` & `dqops-1.2.0/dqops/client/api/sensor_readouts/get_column_profiling_sensor_readouts.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/sensor_readouts/get_table_monitoring_sensor_readouts.py` & `dqops-1.2.0/dqops/client/api/sensor_readouts/get_table_monitoring_sensor_readouts.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/sensor_readouts/get_table_partitioned_sensor_readouts.py` & `dqops-1.2.0/dqops/client/api/sensor_readouts/get_table_partitioned_sensor_readouts.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/sensor_readouts/get_table_profiling_sensor_readouts.py` & `dqops-1.2.0/dqops/client/api/sensor_readouts/get_table_profiling_sensor_readouts.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/sensors/create_sensor.py` & `dqops-1.2.0/dqops/client/api/sensors/create_sensor.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/sensors/delete_sensor.py` & `dqops-1.2.0/dqops/client/api/sensors/delete_sensor.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/sensors/get_all_sensors.py` & `dqops-1.2.0/dqops/client/api/sensors/get_all_sensors.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/sensors/get_sensor.py` & `dqops-1.2.0/dqops/client/api/sensors/get_sensor.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/sensors/get_sensor_folder_tree.py` & `dqops-1.2.0/dqops/client/api/sensors/get_sensor_folder_tree.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/sensors/update_sensor.py` & `dqops-1.2.0/dqops/client/api/sensors/update_sensor.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/shared_credentials/create_shared_credential.py` & `dqops-1.2.0/dqops/client/api/shared_credentials/create_shared_credential.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/shared_credentials/delete_shared_credential.py` & `dqops-1.2.0/dqops/client/api/shared_credentials/delete_shared_credential.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/shared_credentials/download_shared_credential.py` & `dqops-1.2.0/dqops/client/api/shared_credentials/download_shared_credential.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/shared_credentials/get_all_shared_credentials.py` & `dqops-1.2.0/dqops/client/api/shared_credentials/get_all_shared_credentials.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/shared_credentials/get_shared_credential.py` & `dqops-1.2.0/dqops/client/api/shared_credentials/get_shared_credential.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/shared_credentials/update_shared_credential.py` & `dqops-1.2.0/dqops/client/api/shared_credentials/update_shared_credential.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/table_comparison_results/get_table_comparison_monitoring_results.py` & `dqops-1.2.0/dqops/client/api/table_comparison_results/get_table_comparison_monitoring_results.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/table_comparison_results/get_table_comparison_partitioned_results.py` & `dqops-1.2.0/dqops/client/api/table_comparison_results/get_table_comparison_partitioned_results.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/table_comparison_results/get_table_comparison_profiling_results.py` & `dqops-1.2.0/dqops/client/api/table_comparison_results/get_table_comparison_profiling_results.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/table_comparisons/create_table_comparison_configuration.py` & `dqops-1.2.0/dqops/client/api/table_comparisons/create_table_comparison_configuration.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/table_comparisons/create_table_comparison_monitoring_daily.py` & `dqops-1.2.0/dqops/client/api/table_comparisons/create_table_comparison_monitoring_daily.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/table_comparisons/create_table_comparison_monitoring_monthly.py` & `dqops-1.2.0/dqops/client/api/table_comparisons/create_table_comparison_monitoring_monthly.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/table_comparisons/create_table_comparison_partitioned_daily.py` & `dqops-1.2.0/dqops/client/api/table_comparisons/create_table_comparison_partitioned_daily.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/table_comparisons/create_table_comparison_partitioned_monthly.py` & `dqops-1.2.0/dqops/client/api/table_comparisons/create_table_comparison_partitioned_monthly.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/table_comparisons/create_table_comparison_profiling.py` & `dqops-1.2.0/dqops/client/api/table_comparisons/create_table_comparison_profiling.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/table_comparisons/delete_table_comparison_configuration.py` & `dqops-1.2.0/dqops/client/api/table_comparisons/delete_table_comparison_configuration.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/table_comparisons/get_table_comparison_configuration.py` & `dqops-1.2.0/dqops/client/api/table_comparisons/get_table_comparison_configuration.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/table_comparisons/get_table_comparison_configurations.py` & `dqops-1.2.0/dqops/client/api/table_comparisons/get_table_comparison_configurations.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/table_comparisons/get_table_comparison_monitoring_daily.py` & `dqops-1.2.0/dqops/client/api/table_comparisons/get_table_comparison_monitoring_daily.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/table_comparisons/get_table_comparison_monitoring_monthly.py` & `dqops-1.2.0/dqops/client/api/table_comparisons/get_table_comparison_monitoring_monthly.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/table_comparisons/get_table_comparison_partitioned_daily.py` & `dqops-1.2.0/dqops/client/api/table_comparisons/get_table_comparison_partitioned_daily.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/table_comparisons/get_table_comparison_partitioned_monthly.py` & `dqops-1.2.0/dqops/client/api/table_comparisons/get_table_comparison_partitioned_monthly.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/table_comparisons/get_table_comparison_profiling.py` & `dqops-1.2.0/dqops/client/api/table_comparisons/get_table_comparison_profiling.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/table_comparisons/update_table_comparison_configuration.py` & `dqops-1.2.0/dqops/client/api/table_comparisons/update_table_comparison_configuration.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/table_comparisons/update_table_comparison_monitoring_daily.py` & `dqops-1.2.0/dqops/client/api/table_comparisons/update_table_comparison_monitoring_daily.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/table_comparisons/update_table_comparison_monitoring_monthly.py` & `dqops-1.2.0/dqops/client/api/table_comparisons/update_table_comparison_monitoring_monthly.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/table_comparisons/update_table_comparison_partitioned_daily.py` & `dqops-1.2.0/dqops/client/api/table_comparisons/update_table_comparison_partitioned_daily.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/table_comparisons/update_table_comparison_partitioned_monthly.py` & `dqops-1.2.0/dqops/client/api/table_comparisons/update_table_comparison_partitioned_monthly.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/table_comparisons/update_table_comparison_profiling.py` & `dqops-1.2.0/dqops/client/api/table_comparisons/update_table_comparison_profiling.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/create_table.py` & `dqops-1.2.0/dqops/client/api/tables/create_table.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/delete_table.py` & `dqops-1.2.0/dqops/client/api/tables/delete_table.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/get_table.py` & `dqops-1.2.0/dqops/client/api/tables/get_table.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/get_table_basic.py` & `dqops-1.2.0/dqops/client/api/tables/get_table_basic.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/get_table_columns_monitoring_checks_model.py` & `dqops-1.2.0/dqops/client/api/tables/get_table_columns_monitoring_checks_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/get_table_columns_partitioned_checks_model.py` & `dqops-1.2.0/dqops/client/api/tables/get_table_columns_partitioned_checks_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/get_table_columns_profiling_checks_model.py` & `dqops-1.2.0/dqops/client/api/tables/get_table_columns_profiling_checks_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/get_table_comments.py` & `dqops-1.2.0/dqops/client/api/tables/get_table_comments.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/get_table_daily_monitoring_checks.py` & `dqops-1.2.0/dqops/client/api/tables/get_table_daily_monitoring_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/get_table_daily_partitioned_checks.py` & `dqops-1.2.0/dqops/client/api/tables/get_table_daily_partitioned_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/get_table_default_grouping_configuration.py` & `dqops-1.2.0/dqops/client/api/tables/get_table_default_grouping_configuration.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/get_table_incident_grouping.py` & `dqops-1.2.0/dqops/client/api/tables/get_table_incident_grouping.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/get_table_labels.py` & `dqops-1.2.0/dqops/client/api/tables/get_table_labels.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/get_table_monitoring_checks_basic_model.py` & `dqops-1.2.0/dqops/client/api/tables/get_table_monitoring_checks_basic_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/get_table_monitoring_checks_model.py` & `dqops-1.2.0/dqops/client/api/tables/get_table_monitoring_checks_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/get_table_monitoring_checks_model_filter.py` & `dqops-1.2.0/dqops/client/api/tables/get_table_monitoring_checks_model_filter.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/get_table_monitoring_checks_monthly.py` & `dqops-1.2.0/dqops/client/api/tables/get_table_monitoring_checks_monthly.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/get_table_monitoring_checks_templates.py` & `dqops-1.2.0/dqops/client/api/tables/get_table_monitoring_checks_templates.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/get_table_partitioned_checks_basic_model.py` & `dqops-1.2.0/dqops/client/api/tables/get_table_partitioned_checks_basic_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/get_table_partitioned_checks_model.py` & `dqops-1.2.0/dqops/client/api/tables/get_table_partitioned_checks_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/get_table_partitioned_checks_model_filter.py` & `dqops-1.2.0/dqops/client/api/tables/get_table_partitioned_checks_model_filter.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/get_table_partitioned_checks_monthly.py` & `dqops-1.2.0/dqops/client/api/tables/get_table_partitioned_checks_monthly.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/get_table_partitioned_checks_templates.py` & `dqops-1.2.0/dqops/client/api/tables/get_table_partitioned_checks_templates.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/get_table_partitioning.py` & `dqops-1.2.0/dqops/client/api/tables/get_table_partitioning.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/get_table_profiling_checks.py` & `dqops-1.2.0/dqops/client/api/tables/get_table_profiling_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/get_table_profiling_checks_basic_model.py` & `dqops-1.2.0/dqops/client/api/tables/get_table_profiling_checks_basic_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/get_table_profiling_checks_model.py` & `dqops-1.2.0/dqops/client/api/tables/get_table_profiling_checks_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/get_table_profiling_checks_model_filter.py` & `dqops-1.2.0/dqops/client/api/tables/get_table_profiling_checks_model_filter.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/get_table_profiling_checks_templates.py` & `dqops-1.2.0/dqops/client/api/tables/get_table_profiling_checks_templates.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/get_table_scheduling_group_override.py` & `dqops-1.2.0/dqops/client/api/tables/get_table_scheduling_group_override.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/get_table_statistics.py` & `dqops-1.2.0/dqops/client/api/tables/get_table_statistics.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/update_table.py` & `dqops-1.2.0/dqops/client/api/tables/update_table.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/update_table_basic.py` & `dqops-1.2.0/dqops/client/api/tables/update_table_basic.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/update_table_comments.py` & `dqops-1.2.0/dqops/client/api/tables/update_table_comments.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/update_table_daily_monitoring_checks.py` & `dqops-1.2.0/dqops/client/api/tables/update_table_daily_monitoring_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/update_table_default_grouping_configuration.py` & `dqops-1.2.0/dqops/client/api/tables/update_table_default_grouping_configuration.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/update_table_incident_grouping.py` & `dqops-1.2.0/dqops/client/api/tables/update_table_incident_grouping.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/update_table_labels.py` & `dqops-1.2.0/dqops/client/api/tables/update_table_labels.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/update_table_monitoring_checks_model.py` & `dqops-1.2.0/dqops/client/api/tables/update_table_monitoring_checks_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/update_table_monitoring_checks_monthly.py` & `dqops-1.2.0/dqops/client/api/tables/update_table_monitoring_checks_monthly.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/update_table_partitioned_checks_daily.py` & `dqops-1.2.0/dqops/client/api/tables/update_table_partitioned_checks_daily.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/update_table_partitioned_checks_model.py` & `dqops-1.2.0/dqops/client/api/tables/update_table_partitioned_checks_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/update_table_partitioned_checks_monthly.py` & `dqops-1.2.0/dqops/client/api/tables/update_table_partitioned_checks_monthly.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/update_table_partitioning.py` & `dqops-1.2.0/dqops/client/api/tables/update_table_partitioning.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/update_table_profiling_checks.py` & `dqops-1.2.0/dqops/client/api/tables/update_table_profiling_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/update_table_profiling_checks_model.py` & `dqops-1.2.0/dqops/client/api/tables/update_table_profiling_checks_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/tables/update_table_scheduling_group_override.py` & `dqops-1.2.0/dqops/client/api/tables/update_table_scheduling_group_override.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/timezones/get_available_zone_ids.py` & `dqops-1.2.0/dqops/client/api/timezones/get_available_zone_ids.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/users/change_caller_password.py` & `dqops-1.2.0/dqops/client/api/users/change_caller_password.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/users/change_user_password.py` & `dqops-1.2.0/dqops/client/api/users/change_user_password.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/users/create_user.py` & `dqops-1.2.0/dqops/client/api/users/create_user.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/users/delete_user.py` & `dqops-1.2.0/dqops/client/api/users/delete_user.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/users/get_all_users.py` & `dqops-1.2.0/dqops/client/api/users/get_all_users.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/users/get_user.py` & `dqops-1.2.0/dqops/client/api/users/get_user.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/api/users/update_user.py` & `dqops-1.2.0/dqops/client/api/users/update_user.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/client.py` & `dqops-1.2.0/dqops/client/client.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/__init__.py` & `dqops-1.2.0/dqops/client/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 )
 from .anomaly_stationary_percentile_moving_average_rule_fatal_01_pct_parameters_spec import (
     AnomalyStationaryPercentileMovingAverageRuleFatal01PctParametersSpec,
 )
 from .anomaly_stationary_percentile_moving_average_rule_warning_1_pct_parameters_spec import (
     AnomalyStationaryPercentileMovingAverageRuleWarning1PctParametersSpec,
 )
-from .athena_authentication_mode import AthenaAuthenticationMode
 from .authenticated_dashboard_model import AuthenticatedDashboardModel
+from .aws_authentication_mode import AwsAuthenticationMode
 from .between_floats_rule_parameters_spec import BetweenFloatsRuleParametersSpec
 from .between_ints_rule_parameters_spec import BetweenIntsRuleParametersSpec
 from .between_percent_rule_parameters_spec import BetweenPercentRuleParametersSpec
 from .big_query_authentication_mode import BigQueryAuthenticationMode
 from .big_query_jobs_create_project import BigQueryJobsCreateProject
 from .big_query_parameters_spec import BigQueryParametersSpec
 from .bulk_check_deactivate_parameters import BulkCheckDeactivateParameters
@@ -302,14 +302,17 @@
 )
 from .column_current_data_quality_status_model import (
     ColumnCurrentDataQualityStatusModel,
 )
 from .column_current_data_quality_status_model_checks import (
     ColumnCurrentDataQualityStatusModelChecks,
 )
+from .column_current_data_quality_status_model_dimensions import (
+    ColumnCurrentDataQualityStatusModelDimensions,
+)
 from .column_custom_sql_daily_monitoring_checks_spec import (
     ColumnCustomSqlDailyMonitoringChecksSpec,
 )
 from .column_custom_sql_daily_monitoring_checks_spec_custom_checks import (
     ColumnCustomSqlDailyMonitoringChecksSpecCustomChecks,
 )
 from .column_custom_sql_daily_partitioned_checks_spec import (
@@ -515,14 +518,17 @@
 from .column_integrity_profiling_checks_spec import ColumnIntegrityProfilingChecksSpec
 from .column_integrity_profiling_checks_spec_custom_checks import (
     ColumnIntegrityProfilingChecksSpecCustomChecks,
 )
 from .column_invalid_email_format_found_check_spec import (
     ColumnInvalidEmailFormatFoundCheckSpec,
 )
+from .column_invalid_email_format_percent_check_spec import (
+    ColumnInvalidEmailFormatPercentCheckSpec,
+)
 from .column_invalid_ip_4_address_format_found_check_spec import (
     ColumnInvalidIp4AddressFormatFoundCheckSpec,
 )
 from .column_invalid_ip_6_address_format_found_check_spec import (
     ColumnInvalidIp6AddressFormatFoundCheckSpec,
 )
 from .column_invalid_latitude_count_check_spec import (
@@ -805,14 +811,17 @@
 )
 from .column_patterns_daily_partitioned_checks_spec_custom_checks import (
     ColumnPatternsDailyPartitionedChecksSpecCustomChecks,
 )
 from .column_patterns_invalid_email_format_count_sensor_parameters_spec import (
     ColumnPatternsInvalidEmailFormatCountSensorParametersSpec,
 )
+from .column_patterns_invalid_email_format_percent_sensor_parameters_spec import (
+    ColumnPatternsInvalidEmailFormatPercentSensorParametersSpec,
+)
 from .column_patterns_invalid_ip_4_address_format_count_sensor_parameters_spec import (
     ColumnPatternsInvalidIp4AddressFormatCountSensorParametersSpec,
 )
 from .column_patterns_invalid_ip_6_address_format_count_sensor_parameters_spec import (
     ColumnPatternsInvalidIp6AddressFormatCountSensorParametersSpec,
 )
 from .column_patterns_invalid_uuid_format_count_sensor_parameters_spec import (
@@ -1353,14 +1362,17 @@
 from .delete_stored_data_result_partition_results import (
     DeleteStoredDataResultPartitionResults,
 )
 from .detected_datatype_category import DetectedDatatypeCategory
 from .detected_datatype_equals_rule_parameters_spec import (
     DetectedDatatypeEqualsRuleParametersSpec,
 )
+from .dimension_current_data_quality_status_model import (
+    DimensionCurrentDataQualityStatusModel,
+)
 from .display_hint import DisplayHint
 from .dqo_cloud_user_model import DqoCloudUserModel
 from .dqo_job_change_model import DqoJobChangeModel
 from .dqo_job_entry_parameters_model import DqoJobEntryParametersModel
 from .dqo_job_history_entry_model import DqoJobHistoryEntryModel
 from .dqo_job_queue_incremental_snapshot_model import (
     DqoJobQueueIncrementalSnapshotModel,
@@ -1413,14 +1425,15 @@
 from .incident_sort_order import IncidentSortOrder
 from .incident_status import IncidentStatus
 from .incident_webhook_notifications_spec import IncidentWebhookNotificationsSpec
 from .incidents_per_connection_model import IncidentsPerConnectionModel
 from .json_file_format_spec import JsonFileFormatSpec
 from .json_format_type import JsonFormatType
 from .json_records_type import JsonRecordsType
+from .label_model import LabelModel
 from .max_count_rule_0_error_parameters_spec import MaxCountRule0ErrorParametersSpec
 from .max_count_rule_0_warning_parameters_spec import MaxCountRule0WarningParametersSpec
 from .max_count_rule_100_parameters_spec import MaxCountRule100ParametersSpec
 from .max_days_rule_1_parameters_spec import MaxDaysRule1ParametersSpec
 from .max_days_rule_2_parameters_spec import MaxDaysRule2ParametersSpec
 from .max_days_rule_7_parameters_spec import MaxDaysRule7ParametersSpec
 from .max_diff_percent_rule_0_parameters_spec import MaxDiffPercentRule0ParametersSpec
@@ -1481,14 +1494,15 @@
     ProviderSensorDefinitionSpecParameters,
 )
 from .provider_sensor_list_model import ProviderSensorListModel
 from .provider_sensor_model import ProviderSensorModel
 from .provider_sensor_runner_type import ProviderSensorRunnerType
 from .provider_type import ProviderType
 from .quality_category_model import QualityCategoryModel
+from .redshift_authentication_mode import RedshiftAuthenticationMode
 from .redshift_parameters_spec import RedshiftParametersSpec
 from .redshift_parameters_spec_properties import RedshiftParametersSpecProperties
 from .remote_table_list_model import RemoteTableListModel
 from .repair_stored_data_queue_job_parameters import RepairStoredDataQueueJobParameters
 from .rule_folder_model import RuleFolderModel
 from .rule_folder_model_folders import RuleFolderModelFolders
 from .rule_list_model import RuleListModel
@@ -1659,14 +1673,17 @@
 from .table_current_data_quality_status_model import TableCurrentDataQualityStatusModel
 from .table_current_data_quality_status_model_checks import (
     TableCurrentDataQualityStatusModelChecks,
 )
 from .table_current_data_quality_status_model_columns import (
     TableCurrentDataQualityStatusModelColumns,
 )
+from .table_current_data_quality_status_model_dimensions import (
+    TableCurrentDataQualityStatusModelDimensions,
+)
 from .table_custom_sql_daily_monitoring_checks_spec import (
     TableCustomSqlDailyMonitoringChecksSpec,
 )
 from .table_custom_sql_daily_monitoring_checks_spec_custom_checks import (
     TableCustomSqlDailyMonitoringChecksSpecCustomChecks,
 )
 from .table_custom_sql_daily_partitioned_checks_spec import (
@@ -1914,16 +1931,16 @@
     "AllChecksPatchParametersSelectedTablesToColumns",
     "AnomalyDifferencingPercentileMovingAverageRuleError05PctParametersSpec",
     "AnomalyDifferencingPercentileMovingAverageRuleFatal01PctParametersSpec",
     "AnomalyDifferencingPercentileMovingAverageRuleWarning1PctParametersSpec",
     "AnomalyStationaryPercentileMovingAverageRuleError05PctParametersSpec",
     "AnomalyStationaryPercentileMovingAverageRuleFatal01PctParametersSpec",
     "AnomalyStationaryPercentileMovingAverageRuleWarning1PctParametersSpec",
-    "AthenaAuthenticationMode",
     "AuthenticatedDashboardModel",
+    "AwsAuthenticationMode",
     "BetweenFloatsRuleParametersSpec",
     "BetweenIntsRuleParametersSpec",
     "BetweenPercentRuleParametersSpec",
     "BigQueryAuthenticationMode",
     "BigQueryJobsCreateProject",
     "BigQueryParametersSpec",
     "BulkCheckDeactivateParameters",
@@ -2040,14 +2057,15 @@
     "ColumnConversionsMonthlyMonitoringChecksSpecCustomChecks",
     "ColumnConversionsMonthlyPartitionedChecksSpec",
     "ColumnConversionsMonthlyPartitionedChecksSpecCustomChecks",
     "ColumnConversionsProfilingChecksSpec",
     "ColumnConversionsProfilingChecksSpecCustomChecks",
     "ColumnCurrentDataQualityStatusModel",
     "ColumnCurrentDataQualityStatusModelChecks",
+    "ColumnCurrentDataQualityStatusModelDimensions",
     "ColumnCustomSqlDailyMonitoringChecksSpec",
     "ColumnCustomSqlDailyMonitoringChecksSpecCustomChecks",
     "ColumnCustomSqlDailyPartitionedChecksSpec",
     "ColumnCustomSqlDailyPartitionedChecksSpecCustomChecks",
     "ColumnCustomSqlMonthlyMonitoringChecksSpec",
     "ColumnCustomSqlMonthlyMonitoringChecksSpecCustomChecks",
     "ColumnCustomSqlMonthlyPartitionedChecksSpec",
@@ -2119,14 +2137,15 @@
     "ColumnIntegrityMonthlyMonitoringChecksSpec",
     "ColumnIntegrityMonthlyMonitoringChecksSpecCustomChecks",
     "ColumnIntegrityMonthlyPartitionedChecksSpec",
     "ColumnIntegrityMonthlyPartitionedChecksSpecCustomChecks",
     "ColumnIntegrityProfilingChecksSpec",
     "ColumnIntegrityProfilingChecksSpecCustomChecks",
     "ColumnInvalidEmailFormatFoundCheckSpec",
+    "ColumnInvalidEmailFormatPercentCheckSpec",
     "ColumnInvalidIp4AddressFormatFoundCheckSpec",
     "ColumnInvalidIp6AddressFormatFoundCheckSpec",
     "ColumnInvalidLatitudeCountCheckSpec",
     "ColumnInvalidLongitudeCountCheckSpec",
     "ColumnInvalidUuidFormatFoundCheckSpec",
     "ColumnListModel",
     "ColumnMaxAnomalyDifferencingCheckSpec",
@@ -2235,14 +2254,15 @@
     "ColumnNumericValidLongitudePercentSensorParametersSpec",
     "ColumnPartitionedCheckCategoriesSpec",
     "ColumnPatternsDailyMonitoringChecksSpec",
     "ColumnPatternsDailyMonitoringChecksSpecCustomChecks",
     "ColumnPatternsDailyPartitionedChecksSpec",
     "ColumnPatternsDailyPartitionedChecksSpecCustomChecks",
     "ColumnPatternsInvalidEmailFormatCountSensorParametersSpec",
+    "ColumnPatternsInvalidEmailFormatPercentSensorParametersSpec",
     "ColumnPatternsInvalidIp4AddressFormatCountSensorParametersSpec",
     "ColumnPatternsInvalidIp6AddressFormatCountSensorParametersSpec",
     "ColumnPatternsInvalidUuidFormatCountSensorParametersSpec",
     "ColumnPatternsMonthlyMonitoringChecksSpec",
     "ColumnPatternsMonthlyMonitoringChecksSpecCustomChecks",
     "ColumnPatternsMonthlyPartitionedChecksSpec",
     "ColumnPatternsMonthlyPartitionedChecksSpecCustomChecks",
@@ -2465,14 +2485,15 @@
     "DefaultTableChecksPatternModel",
     "DeleteStoredDataQueueJobParameters",
     "DeleteStoredDataQueueJobResult",
     "DeleteStoredDataResult",
     "DeleteStoredDataResultPartitionResults",
     "DetectedDatatypeCategory",
     "DetectedDatatypeEqualsRuleParametersSpec",
+    "DimensionCurrentDataQualityStatusModel",
     "DisplayHint",
     "DqoCloudUserModel",
     "DqoJobChangeModel",
     "DqoJobEntryParametersModel",
     "DqoJobHistoryEntryModel",
     "DqoJobQueueIncrementalSnapshotModel",
     "DqoJobQueueInitialSnapshotModel",
@@ -2521,14 +2542,15 @@
     "IncidentSortOrder",
     "IncidentsPerConnectionModel",
     "IncidentStatus",
     "IncidentWebhookNotificationsSpec",
     "JsonFileFormatSpec",
     "JsonFormatType",
     "JsonRecordsType",
+    "LabelModel",
     "MaxCountRule0ErrorParametersSpec",
     "MaxCountRule0WarningParametersSpec",
     "MaxCountRule100ParametersSpec",
     "MaxDaysRule1ParametersSpec",
     "MaxDaysRule2ParametersSpec",
     "MaxDaysRule7ParametersSpec",
     "MaxDiffPercentRule0ParametersSpec",
@@ -2577,14 +2599,15 @@
     "ProviderSensorDefinitionSpec",
     "ProviderSensorDefinitionSpecParameters",
     "ProviderSensorListModel",
     "ProviderSensorModel",
     "ProviderSensorRunnerType",
     "ProviderType",
     "QualityCategoryModel",
+    "RedshiftAuthenticationMode",
     "RedshiftParametersSpec",
     "RedshiftParametersSpecProperties",
     "RemoteTableListModel",
     "RepairStoredDataQueueJobParameters",
     "RuleFolderModel",
     "RuleFolderModelFolders",
     "RuleListModel",
@@ -2677,14 +2700,15 @@
     "TableComparisonResultsModel",
     "TableComparisonResultsModelColumnComparisonResults",
     "TableComparisonResultsModelTableComparisonResults",
     "TableComparisonRowCountMatchCheckSpec",
     "TableCurrentDataQualityStatusModel",
     "TableCurrentDataQualityStatusModelChecks",
     "TableCurrentDataQualityStatusModelColumns",
+    "TableCurrentDataQualityStatusModelDimensions",
     "TableCustomSqlDailyMonitoringChecksSpec",
     "TableCustomSqlDailyMonitoringChecksSpecCustomChecks",
     "TableCustomSqlDailyPartitionedChecksSpec",
     "TableCustomSqlDailyPartitionedChecksSpecCustomChecks",
     "TableCustomSqlMonthlyMonitoringChecksSpec",
     "TableCustomSqlMonthlyMonitoringChecksSpecCustomChecks",
     "TableCustomSqlMonthlyPartitionedChecksSpec",
```

### Comparing `dqops-1.1.0/dqops/client/models/all_checks_patch_parameters.py` & `dqops-1.2.0/dqops/client/models/all_checks_patch_parameters.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/all_checks_patch_parameters_selected_tables_to_columns.py` & `dqops-1.2.0/dqops/client/models/all_checks_patch_parameters_selected_tables_to_columns.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/anomaly_differencing_percentile_moving_average_rule_error_05_pct_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/anomaly_differencing_percentile_moving_average_rule_error_05_pct_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/anomaly_differencing_percentile_moving_average_rule_fatal_01_pct_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/anomaly_differencing_percentile_moving_average_rule_fatal_01_pct_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/anomaly_differencing_percentile_moving_average_rule_warning_1_pct_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/anomaly_differencing_percentile_moving_average_rule_warning_1_pct_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/anomaly_stationary_percentile_moving_average_rule_error_05_pct_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/anomaly_stationary_percentile_moving_average_rule_error_05_pct_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/anomaly_stationary_percentile_moving_average_rule_fatal_01_pct_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/anomaly_stationary_percentile_moving_average_rule_fatal_01_pct_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/anomaly_stationary_percentile_moving_average_rule_warning_1_pct_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/anomaly_stationary_percentile_moving_average_rule_warning_1_pct_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/authenticated_dashboard_model.py` & `dqops-1.2.0/dqops/client/models/authenticated_dashboard_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/between_floats_rule_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/between_floats_rule_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/between_ints_rule_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/between_ints_rule_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/between_percent_rule_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/between_percent_rule_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/big_query_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/big_query_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/bulk_check_deactivate_parameters.py` & `dqops-1.2.0/dqops/client/models/bulk_check_deactivate_parameters.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/bulk_check_deactivate_parameters_selected_tables_to_columns.py` & `dqops-1.2.0/dqops/client/models/bulk_check_deactivate_parameters_selected_tables_to_columns.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/change_percent_1_day_rule_10_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/change_percent_1_day_rule_10_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/change_percent_1_day_rule_20_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/change_percent_1_day_rule_20_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/change_percent_1_day_rule_50_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/change_percent_1_day_rule_50_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/change_percent_30_days_rule_10_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/change_percent_30_days_rule_10_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/change_percent_30_days_rule_20_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/change_percent_30_days_rule_20_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/change_percent_30_days_rule_50_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/change_percent_30_days_rule_50_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/change_percent_7_days_rule_10_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/change_percent_7_days_rule_10_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/change_percent_7_days_rule_20_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/change_percent_7_days_rule_20_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/change_percent_7_days_rule_50_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/change_percent_7_days_rule_50_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/change_percent_rule_10_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/change_percent_rule_10_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/change_percent_rule_20_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/change_percent_rule_20_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/change_percent_rule_50_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/change_percent_rule_50_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/check_configuration_model.py` & `dqops-1.2.0/dqops/client/models/check_configuration_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/check_container_list_model.py` & `dqops-1.2.0/dqops/client/models/check_container_list_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/check_container_model.py` & `dqops-1.2.0/dqops/client/models/check_container_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/check_container_type_model.py` & `dqops-1.2.0/dqops/client/models/check_container_type_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/check_current_data_quality_status_model.py` & `dqops-1.2.0/dqops/client/models/errors_list_model.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,139 +1,134 @@
-from typing import Any, Dict, List, Type, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union, cast
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
-from ..models.check_result_status import CheckResultStatus
-from ..models.check_time_scale import CheckTimeScale
 from ..models.check_type import CheckType
-from ..models.rule_severity_level import RuleSeverityLevel
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CheckCurrentDataQualityStatusModel")
+if TYPE_CHECKING:
+    from ..models.error_entry_model import ErrorEntryModel
+
+
+T = TypeVar("T", bound="ErrorsListModel")
 
 
 @_attrs_define
-class CheckCurrentDataQualityStatusModel:
-    """The most recent data quality status for a single data quality check. If data grouping is enabled, the
-    *current_severity* will be the highest data quality issue status from all data quality results for all data groups.
-    For partitioned checks, it is the highest severity of all results for all partitions (time periods) in the analyzed
-    time range.
-
-        Attributes:
-            current_severity (Union[Unset, CheckResultStatus]):
-            highest_historical_severity (Union[Unset, RuleSeverityLevel]):
-            last_executed_at (Union[Unset, int]): The UTC timestamp when the check was recently executed.
-            check_type (Union[Unset, CheckType]):
-            time_scale (Union[Unset, CheckTimeScale]):
-            category (Union[Unset, str]): Check category name, such as nulls, schema, strings, volume.
-            quality_dimension (Union[Unset, str]): Data quality dimension, such as Completeness, Uniqueness, Validity.
+class ErrorsListModel:
+    """
+    Attributes:
+        check_name (Union[Unset, str]): Check name
+        check_display_name (Union[Unset, str]): Check display name
+        check_type (Union[Unset, CheckType]):
+        check_hash (Union[Unset, int]): Check hash
+        check_category (Union[Unset, str]): Check category name
+        data_groups_names (Union[Unset, List[str]]): Data groups list
+        data_group (Union[Unset, str]): Selected data group
+        error_entries (Union[Unset, List['ErrorEntryModel']]): Error entries
     """
 
-    current_severity: Union[Unset, CheckResultStatus] = UNSET
-    highest_historical_severity: Union[Unset, RuleSeverityLevel] = UNSET
-    last_executed_at: Union[Unset, int] = UNSET
+    check_name: Union[Unset, str] = UNSET
+    check_display_name: Union[Unset, str] = UNSET
     check_type: Union[Unset, CheckType] = UNSET
-    time_scale: Union[Unset, CheckTimeScale] = UNSET
-    category: Union[Unset, str] = UNSET
-    quality_dimension: Union[Unset, str] = UNSET
+    check_hash: Union[Unset, int] = UNSET
+    check_category: Union[Unset, str] = UNSET
+    data_groups_names: Union[Unset, List[str]] = UNSET
+    data_group: Union[Unset, str] = UNSET
+    error_entries: Union[Unset, List["ErrorEntryModel"]] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        current_severity: Union[Unset, str] = UNSET
-        if not isinstance(self.current_severity, Unset):
-            current_severity = self.current_severity.value
-
-        highest_historical_severity: Union[Unset, str] = UNSET
-        if not isinstance(self.highest_historical_severity, Unset):
-            highest_historical_severity = self.highest_historical_severity.value
-
-        last_executed_at = self.last_executed_at
+        check_name = self.check_name
+        check_display_name = self.check_display_name
         check_type: Union[Unset, str] = UNSET
         if not isinstance(self.check_type, Unset):
             check_type = self.check_type.value
 
-        time_scale: Union[Unset, str] = UNSET
-        if not isinstance(self.time_scale, Unset):
-            time_scale = self.time_scale.value
+        check_hash = self.check_hash
+        check_category = self.check_category
+        data_groups_names: Union[Unset, List[str]] = UNSET
+        if not isinstance(self.data_groups_names, Unset):
+            data_groups_names = self.data_groups_names
+
+        data_group = self.data_group
+        error_entries: Union[Unset, List[Dict[str, Any]]] = UNSET
+        if not isinstance(self.error_entries, Unset):
+            error_entries = []
+            for error_entries_item_data in self.error_entries:
+                error_entries_item = error_entries_item_data.to_dict()
 
-        category = self.category
-        quality_dimension = self.quality_dimension
+                error_entries.append(error_entries_item)
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if current_severity is not UNSET:
-            field_dict["current_severity"] = current_severity
-        if highest_historical_severity is not UNSET:
-            field_dict["highest_historical_severity"] = highest_historical_severity
-        if last_executed_at is not UNSET:
-            field_dict["last_executed_at"] = last_executed_at
+        if check_name is not UNSET:
+            field_dict["checkName"] = check_name
+        if check_display_name is not UNSET:
+            field_dict["checkDisplayName"] = check_display_name
         if check_type is not UNSET:
-            field_dict["check_type"] = check_type
-        if time_scale is not UNSET:
-            field_dict["time_scale"] = time_scale
-        if category is not UNSET:
-            field_dict["category"] = category
-        if quality_dimension is not UNSET:
-            field_dict["quality_dimension"] = quality_dimension
+            field_dict["checkType"] = check_type
+        if check_hash is not UNSET:
+            field_dict["checkHash"] = check_hash
+        if check_category is not UNSET:
+            field_dict["checkCategory"] = check_category
+        if data_groups_names is not UNSET:
+            field_dict["dataGroupsNames"] = data_groups_names
+        if data_group is not UNSET:
+            field_dict["dataGroup"] = data_group
+        if error_entries is not UNSET:
+            field_dict["errorEntries"] = error_entries
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _current_severity = d.pop("current_severity", UNSET)
-        current_severity: Union[Unset, CheckResultStatus]
-        if isinstance(_current_severity, Unset):
-            current_severity = UNSET
-        else:
-            current_severity = CheckResultStatus(_current_severity)
+        from ..models.error_entry_model import ErrorEntryModel
 
-        _highest_historical_severity = d.pop("highest_historical_severity", UNSET)
-        highest_historical_severity: Union[Unset, RuleSeverityLevel]
-        if isinstance(_highest_historical_severity, Unset):
-            highest_historical_severity = UNSET
-        else:
-            highest_historical_severity = RuleSeverityLevel(
-                _highest_historical_severity
-            )
+        d = src_dict.copy()
+        check_name = d.pop("checkName", UNSET)
 
-        last_executed_at = d.pop("last_executed_at", UNSET)
+        check_display_name = d.pop("checkDisplayName", UNSET)
 
-        _check_type = d.pop("check_type", UNSET)
+        _check_type = d.pop("checkType", UNSET)
         check_type: Union[Unset, CheckType]
         if isinstance(_check_type, Unset):
             check_type = UNSET
         else:
             check_type = CheckType(_check_type)
 
-        _time_scale = d.pop("time_scale", UNSET)
-        time_scale: Union[Unset, CheckTimeScale]
-        if isinstance(_time_scale, Unset):
-            time_scale = UNSET
-        else:
-            time_scale = CheckTimeScale(_time_scale)
+        check_hash = d.pop("checkHash", UNSET)
+
+        check_category = d.pop("checkCategory", UNSET)
+
+        data_groups_names = cast(List[str], d.pop("dataGroupsNames", UNSET))
+
+        data_group = d.pop("dataGroup", UNSET)
 
-        category = d.pop("category", UNSET)
+        error_entries = []
+        _error_entries = d.pop("errorEntries", UNSET)
+        for error_entries_item_data in _error_entries or []:
+            error_entries_item = ErrorEntryModel.from_dict(error_entries_item_data)
 
-        quality_dimension = d.pop("quality_dimension", UNSET)
+            error_entries.append(error_entries_item)
 
-        check_current_data_quality_status_model = cls(
-            current_severity=current_severity,
-            highest_historical_severity=highest_historical_severity,
-            last_executed_at=last_executed_at,
+        errors_list_model = cls(
+            check_name=check_name,
+            check_display_name=check_display_name,
             check_type=check_type,
-            time_scale=time_scale,
-            category=category,
-            quality_dimension=quality_dimension,
+            check_hash=check_hash,
+            check_category=check_category,
+            data_groups_names=data_groups_names,
+            data_group=data_group,
+            error_entries=error_entries,
         )
 
-        check_current_data_quality_status_model.additional_properties = d
-        return check_current_data_quality_status_model
+        errors_list_model.additional_properties = d
+        return errors_list_model
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dqops-1.1.0/dqops/client/models/check_definition_folder_model.py` & `dqops-1.2.0/dqops/client/models/check_definition_folder_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/check_definition_folder_model_folders.py` & `dqops-1.2.0/dqops/client/models/check_definition_folder_model_folders.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/check_definition_list_model.py` & `dqops-1.2.0/dqops/client/models/check_definition_list_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/check_definition_model.py` & `dqops-1.2.0/dqops/client/models/check_definition_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
     Attributes:
         check_name (Union[Unset, str]): Check name
         sensor_name (Union[Unset, str]): Sensor name
         rule_name (Union[Unset, str]): Rule name
         help_text (Union[Unset, str]): Help text that is shown in the check editor that describes the purpose and usage
             of the check
+        friendly_name (Union[Unset, str]): An alternative check's name that is shown on the check editor.
         standard (Union[Unset, bool]): This is a standard data quality check that is always shown on the data quality
             checks editor screen. Non-standard data quality checks (when the value is false) are advanced checks that are
             shown when the user decides to expand the list of checks.
         custom (Union[Unset, bool]): This check has is a custom check or was customized by the user.
         built_in (Union[Unset, bool]): This check is provided with DQOps as a built-in check.
         can_edit (Union[Unset, bool]): Boolean flag that decides if the current user can update or delete this object.
         yaml_parsing_error (Union[Unset, str]): Optional parsing error that was captured when parsing the YAML file.
@@ -29,26 +30,28 @@
             error message and the file location.
     """
 
     check_name: Union[Unset, str] = UNSET
     sensor_name: Union[Unset, str] = UNSET
     rule_name: Union[Unset, str] = UNSET
     help_text: Union[Unset, str] = UNSET
+    friendly_name: Union[Unset, str] = UNSET
     standard: Union[Unset, bool] = UNSET
     custom: Union[Unset, bool] = UNSET
     built_in: Union[Unset, bool] = UNSET
     can_edit: Union[Unset, bool] = UNSET
     yaml_parsing_error: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         check_name = self.check_name
         sensor_name = self.sensor_name
         rule_name = self.rule_name
         help_text = self.help_text
+        friendly_name = self.friendly_name
         standard = self.standard
         custom = self.custom
         built_in = self.built_in
         can_edit = self.can_edit
         yaml_parsing_error = self.yaml_parsing_error
 
         field_dict: Dict[str, Any] = {}
@@ -58,14 +61,16 @@
             field_dict["check_name"] = check_name
         if sensor_name is not UNSET:
             field_dict["sensor_name"] = sensor_name
         if rule_name is not UNSET:
             field_dict["rule_name"] = rule_name
         if help_text is not UNSET:
             field_dict["help_text"] = help_text
+        if friendly_name is not UNSET:
+            field_dict["friendly_name"] = friendly_name
         if standard is not UNSET:
             field_dict["standard"] = standard
         if custom is not UNSET:
             field_dict["custom"] = custom
         if built_in is not UNSET:
             field_dict["built_in"] = built_in
         if can_edit is not UNSET:
@@ -82,14 +87,16 @@
 
         sensor_name = d.pop("sensor_name", UNSET)
 
         rule_name = d.pop("rule_name", UNSET)
 
         help_text = d.pop("help_text", UNSET)
 
+        friendly_name = d.pop("friendly_name", UNSET)
+
         standard = d.pop("standard", UNSET)
 
         custom = d.pop("custom", UNSET)
 
         built_in = d.pop("built_in", UNSET)
 
         can_edit = d.pop("can_edit", UNSET)
@@ -97,14 +104,15 @@
         yaml_parsing_error = d.pop("yaml_parsing_error", UNSET)
 
         check_definition_model = cls(
             check_name=check_name,
             sensor_name=sensor_name,
             rule_name=rule_name,
             help_text=help_text,
+            friendly_name=friendly_name,
             standard=standard,
             custom=custom,
             built_in=built_in,
             can_edit=can_edit,
             yaml_parsing_error=yaml_parsing_error,
         )
```

### Comparing `dqops-1.1.0/dqops/client/models/check_list_model.py` & `dqops-1.2.0/dqops/client/models/check_list_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/check_model.py` & `dqops-1.2.0/dqops/client/models/check_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,17 @@
 @_attrs_define
 class CheckModel:
     """Model that returns the form definition and the form data to edit a single data quality check.
 
     Attributes:
         check_name (Union[Unset, str]): Data quality check name that is used in YAML.
         help_text (Union[Unset, str]): Help text that describes the data quality check.
+        display_name (Union[Unset, str]): User assigned display name that is shown instead of the original data quality
+            check name.
+        friendly_name (Union[Unset, str]): An alternative check's name that is shown on the check editor as a hint.
         sensor_parameters (Union[Unset, List['FieldModel']]): List of fields for editing the sensor parameters.
         sensor_name (Union[Unset, str]): Full sensor name. This field is for information purposes and can be used to
             create additional custom checks that reuse the same data quality sensor.
         quality_dimension (Union[Unset, str]): Data quality dimension used for tagging the results of this data quality
             checks.
         rule (Union[Unset, RuleThresholdsModel]): Model that returns the form definition and the form data to edit a
             single rule with all three threshold levels (low, medium, high).
@@ -80,14 +83,16 @@
         can_run_checks (Union[Unset, bool]): Boolean flag that decides if the current user can run checks.
         can_delete_data (Union[Unset, bool]): Boolean flag that decides if the current user can delete data (results).
         check_hash (Union[Unset, int]): The check hash code that identifies the check instance.
     """
 
     check_name: Union[Unset, str] = UNSET
     help_text: Union[Unset, str] = UNSET
+    display_name: Union[Unset, str] = UNSET
+    friendly_name: Union[Unset, str] = UNSET
     sensor_parameters: Union[Unset, List["FieldModel"]] = UNSET
     sensor_name: Union[Unset, str] = UNSET
     quality_dimension: Union[Unset, str] = UNSET
     rule: Union[Unset, "RuleThresholdsModel"] = UNSET
     supports_grouping: Union[Unset, bool] = UNSET
     standard: Union[Unset, bool] = UNSET
     default_check: Union[Unset, bool] = UNSET
@@ -112,14 +117,16 @@
     can_delete_data: Union[Unset, bool] = UNSET
     check_hash: Union[Unset, int] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         check_name = self.check_name
         help_text = self.help_text
+        display_name = self.display_name
+        friendly_name = self.friendly_name
         sensor_parameters: Union[Unset, List[Dict[str, Any]]] = UNSET
         if not isinstance(self.sensor_parameters, Unset):
             sensor_parameters = []
             for sensor_parameters_item_data in self.sensor_parameters:
                 sensor_parameters_item = sensor_parameters_item_data.to_dict()
 
                 sensor_parameters.append(sensor_parameters_item)
@@ -195,14 +202,18 @@
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if check_name is not UNSET:
             field_dict["check_name"] = check_name
         if help_text is not UNSET:
             field_dict["help_text"] = help_text
+        if display_name is not UNSET:
+            field_dict["display_name"] = display_name
+        if friendly_name is not UNSET:
+            field_dict["friendly_name"] = friendly_name
         if sensor_parameters is not UNSET:
             field_dict["sensor_parameters"] = sensor_parameters
         if sensor_name is not UNSET:
             field_dict["sensor_name"] = sensor_name
         if quality_dimension is not UNSET:
             field_dict["quality_dimension"] = quality_dimension
         if rule is not UNSET:
@@ -275,14 +286,18 @@
         from ..models.similar_check_model import SimilarCheckModel
 
         d = src_dict.copy()
         check_name = d.pop("check_name", UNSET)
 
         help_text = d.pop("help_text", UNSET)
 
+        display_name = d.pop("display_name", UNSET)
+
+        friendly_name = d.pop("friendly_name", UNSET)
+
         sensor_parameters = []
         _sensor_parameters = d.pop("sensor_parameters", UNSET)
         for sensor_parameters_item_data in _sensor_parameters or []:
             sensor_parameters_item = FieldModel.from_dict(sensor_parameters_item_data)
 
             sensor_parameters.append(sensor_parameters_item)
 
@@ -397,14 +412,16 @@
         can_delete_data = d.pop("can_delete_data", UNSET)
 
         check_hash = d.pop("check_hash", UNSET)
 
         check_model = cls(
             check_name=check_name,
             help_text=help_text,
+            display_name=display_name,
+            friendly_name=friendly_name,
             sensor_parameters=sensor_parameters,
             sensor_name=sensor_name,
             quality_dimension=quality_dimension,
             rule=rule,
             supports_grouping=supports_grouping,
             standard=standard,
             default_check=default_check,
```

### Comparing `dqops-1.1.0/dqops/client/models/check_result_entry_model.py` & `dqops-1.2.0/dqops/client/models/check_result_entry_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/check_result_sort_order.py` & `dqops-1.2.0/dqops/client/models/check_result_sort_order.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/check_results_list_model.py` & `dqops-1.2.0/dqops/client/models/check_results_list_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/check_results_overview_data_model.py` & `dqops-1.2.0/dqops/client/models/check_results_overview_data_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/check_search_filters.py` & `dqops-1.2.0/dqops/client/models/check_search_filters.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,26 +32,29 @@
         tags (Union[Unset, List[str]]): An array of tags assigned to the table. All tags must be present on a table to
             match. The tags can use patterns:  'prefix\*', '\*suffix', 'prefix\*suffix'. The tags are assigned to the table
             on the data grouping screen when any of the data grouping hierarchy level is assigned a static value, which is a
             tag.
         labels (Union[Unset, List[str]]): An array of labels assigned to the table. All labels must be present on a
             table to match. The labels can use patterns:  'prefix\*', '\*suffix', 'prefix\*suffix'. The labels are assigned
             on the labels screen and stored in the *labels* node in the *.dqotable.yaml* file.
+        max_results (Union[Unset, int]): Optional limit for the maximum number of results to return.
         column (Union[Unset, str]): The column name. This field accepts search patterns in the format: 'fk_\*', '\*_id',
             'prefix\*suffix'.
         column_data_type (Union[Unset, str]): The column data type that was imported from the data source and is stored
             in the [columns -> column_name -> type_snapshot ->
             column_type](/docs/reference/yaml/TableYaml/#columntypesnapshotspec) field in the *.dqotable.yaml* file.
         column_nullable (Union[Unset, bool]): Optional filter to find only nullable (when the value is *true*) or not
             nullable (when the value is *false*) columns, based on the value of the [columns -> column_name -> type_snapshot
             -> nullable](/docs/reference/yaml/TableYaml/#columntypesnapshotspec) field in the *.dqotable.yaml* file.
         check_target (Union[Unset, CheckTarget]):
         check_type (Union[Unset, CheckType]):
         time_scale (Union[Unset, CheckTimeScale]):
         check_category (Union[Unset, str]): The target check category, for example: *nulls*, *volume*, *anomaly*.
+        quality_dimension (Union[Unset, str]): The target data quality dimension, for example: *Completeness*,
+            *Accuracy*, *Consistency*, *Timeliness*, *Availability*.
         table_comparison_name (Union[Unset, str]): The name of a configured table comparison. When the table comparison
             is provided, DQOps will only perform table comparison checks that compare data between tables.
         check_name (Union[Unset, str]): The target check name to run only this named check. Uses the short check name
             which is the name of the deepest folder in the *checks* folder. This field supports search patterns such as:
             'profiling_\*', '\*_count', 'profiling_\*_percent'.
         sensor_name (Union[Unset, str]): The target sensor name to run only data quality checks that are using this
             sensor. Uses the full sensor name which is the full folder path within the *sensors* folder. This field supports
@@ -60,21 +63,23 @@
     """
 
     connection: Union[Unset, str] = UNSET
     full_table_name: Union[Unset, str] = UNSET
     enabled: Union[Unset, bool] = UNSET
     tags: Union[Unset, List[str]] = UNSET
     labels: Union[Unset, List[str]] = UNSET
+    max_results: Union[Unset, int] = UNSET
     column: Union[Unset, str] = UNSET
     column_data_type: Union[Unset, str] = UNSET
     column_nullable: Union[Unset, bool] = UNSET
     check_target: Union[Unset, CheckTarget] = UNSET
     check_type: Union[Unset, CheckType] = UNSET
     time_scale: Union[Unset, CheckTimeScale] = UNSET
     check_category: Union[Unset, str] = UNSET
+    quality_dimension: Union[Unset, str] = UNSET
     table_comparison_name: Union[Unset, str] = UNSET
     check_name: Union[Unset, str] = UNSET
     sensor_name: Union[Unset, str] = UNSET
     check_hierarchy_ids_models: Union[Unset, List["HierarchyIdModel"]] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
@@ -85,14 +90,15 @@
         if not isinstance(self.tags, Unset):
             tags = self.tags
 
         labels: Union[Unset, List[str]] = UNSET
         if not isinstance(self.labels, Unset):
             labels = self.labels
 
+        max_results = self.max_results
         column = self.column
         column_data_type = self.column_data_type
         column_nullable = self.column_nullable
         check_target: Union[Unset, str] = UNSET
         if not isinstance(self.check_target, Unset):
             check_target = self.check_target.value
 
@@ -101,14 +107,15 @@
             check_type = self.check_type.value
 
         time_scale: Union[Unset, str] = UNSET
         if not isinstance(self.time_scale, Unset):
             time_scale = self.time_scale.value
 
         check_category = self.check_category
+        quality_dimension = self.quality_dimension
         table_comparison_name = self.table_comparison_name
         check_name = self.check_name
         sensor_name = self.sensor_name
         check_hierarchy_ids_models: Union[Unset, List[Dict[str, Any]]] = UNSET
         if not isinstance(self.check_hierarchy_ids_models, Unset):
             check_hierarchy_ids_models = []
             for check_hierarchy_ids_models_item_data in self.check_hierarchy_ids_models:
@@ -127,28 +134,32 @@
             field_dict["fullTableName"] = full_table_name
         if enabled is not UNSET:
             field_dict["enabled"] = enabled
         if tags is not UNSET:
             field_dict["tags"] = tags
         if labels is not UNSET:
             field_dict["labels"] = labels
+        if max_results is not UNSET:
+            field_dict["maxResults"] = max_results
         if column is not UNSET:
             field_dict["column"] = column
         if column_data_type is not UNSET:
             field_dict["columnDataType"] = column_data_type
         if column_nullable is not UNSET:
             field_dict["columnNullable"] = column_nullable
         if check_target is not UNSET:
             field_dict["checkTarget"] = check_target
         if check_type is not UNSET:
             field_dict["checkType"] = check_type
         if time_scale is not UNSET:
             field_dict["timeScale"] = time_scale
         if check_category is not UNSET:
             field_dict["checkCategory"] = check_category
+        if quality_dimension is not UNSET:
+            field_dict["qualityDimension"] = quality_dimension
         if table_comparison_name is not UNSET:
             field_dict["tableComparisonName"] = table_comparison_name
         if check_name is not UNSET:
             field_dict["checkName"] = check_name
         if sensor_name is not UNSET:
             field_dict["sensorName"] = sensor_name
         if check_hierarchy_ids_models is not UNSET:
@@ -167,14 +178,16 @@
 
         enabled = d.pop("enabled", UNSET)
 
         tags = cast(List[str], d.pop("tags", UNSET))
 
         labels = cast(List[str], d.pop("labels", UNSET))
 
+        max_results = d.pop("maxResults", UNSET)
+
         column = d.pop("column", UNSET)
 
         column_data_type = d.pop("columnDataType", UNSET)
 
         column_nullable = d.pop("columnNullable", UNSET)
 
         _check_target = d.pop("checkTarget", UNSET)
@@ -196,14 +209,16 @@
         if isinstance(_time_scale, Unset):
             time_scale = UNSET
         else:
             time_scale = CheckTimeScale(_time_scale)
 
         check_category = d.pop("checkCategory", UNSET)
 
+        quality_dimension = d.pop("qualityDimension", UNSET)
+
         table_comparison_name = d.pop("tableComparisonName", UNSET)
 
         check_name = d.pop("checkName", UNSET)
 
         sensor_name = d.pop("sensorName", UNSET)
 
         check_hierarchy_ids_models = []
@@ -217,21 +232,23 @@
 
         check_search_filters = cls(
             connection=connection,
             full_table_name=full_table_name,
             enabled=enabled,
             tags=tags,
             labels=labels,
+            max_results=max_results,
             column=column,
             column_data_type=column_data_type,
             column_nullable=column_nullable,
             check_target=check_target,
             check_type=check_type,
             time_scale=time_scale,
             check_category=check_category,
+            quality_dimension=quality_dimension,
             table_comparison_name=table_comparison_name,
             check_name=check_name,
             sensor_name=sensor_name,
             check_hierarchy_ids_models=check_hierarchy_ids_models,
         )
 
         check_search_filters.additional_properties = d
```

### Comparing `dqops-1.1.0/dqops/client/models/check_template.py` & `dqops-1.2.0/dqops/client/models/check_template.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/cloud_synchronization_folders_status_model.py` & `dqops-1.2.0/dqops/client/models/cloud_synchronization_folders_status_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/collect_statistics_on_table_queue_job_parameters.py` & `dqops-1.2.0/dqops/client/models/collect_statistics_on_table_queue_job_parameters.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/collect_statistics_queue_job_parameters.py` & `dqops-1.2.0/dqops/client/models/collect_statistics_queue_job_parameters.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/collect_statistics_queue_job_result.py` & `dqops-1.2.0/dqops/client/models/collect_statistics_queue_job_result.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/collect_statistics_result.py` & `dqops-1.2.0/dqops/client/models/collect_statistics_result.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_accepted_values_daily_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_accepted_values_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_accepted_values_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_accepted_values_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_accepted_values_daily_partitioned_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_accepted_values_daily_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_accepted_values_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_accepted_values_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_accepted_values_monthly_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_accepted_values_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_accepted_values_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_accepted_values_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_accepted_values_monthly_partitioned_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_accepted_values_monthly_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_accepted_values_monthly_partitioned_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_accepted_values_monthly_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_accepted_values_profiling_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_accepted_values_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_accepted_values_profiling_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_accepted_values_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_accepted_values_text_found_in_set_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_accepted_values_text_found_in_set_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_accuracy_daily_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_accuracy_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_accuracy_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_accuracy_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_accuracy_monthly_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_accuracy_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_accuracy_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_accuracy_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_accuracy_profiling_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_accuracy_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_accuracy_profiling_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_accuracy_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_accuracy_total_average_match_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_accuracy_total_average_match_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_accuracy_total_average_match_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_accuracy_total_average_match_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_accuracy_total_max_match_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_accuracy_total_max_match_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_accuracy_total_max_match_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_accuracy_total_max_match_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_accuracy_total_min_match_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_accuracy_total_min_match_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_accuracy_total_min_match_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_accuracy_total_min_match_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_accuracy_total_not_null_count_match_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_accuracy_total_not_null_count_match_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_accuracy_total_not_null_count_match_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_accuracy_total_not_null_count_match_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_accuracy_total_sum_match_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_accuracy_total_sum_match_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_accuracy_total_sum_match_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_accuracy_total_sum_match_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_anomaly_daily_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_anomaly_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_anomaly_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_anomaly_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_anomaly_daily_partitioned_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_anomaly_daily_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_anomaly_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_anomaly_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_anomaly_profiling_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_anomaly_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_anomaly_profiling_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_anomaly_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_bool_daily_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_bool_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_bool_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_bool_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_bool_daily_partitioned_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_bool_daily_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_bool_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_bool_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_bool_false_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_bool_false_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_bool_monthly_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_bool_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_bool_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_bool_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_bool_monthly_partitioned_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_bool_monthly_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_bool_monthly_partitioned_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_bool_monthly_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_bool_profiling_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_bool_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_bool_profiling_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_bool_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_bool_true_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_bool_true_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_column_exists_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_column_exists_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_column_type_hash_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_column_type_hash_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_comparison_daily_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_comparison_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_comparison_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_comparison_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_comparison_daily_partitioned_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_comparison_daily_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_comparison_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_comparison_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_comparison_max_match_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_comparison_max_match_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_comparison_mean_match_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_comparison_mean_match_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_comparison_min_match_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_comparison_min_match_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_comparison_model.py` & `dqops-1.2.0/dqops/client/models/column_comparison_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_comparison_monthly_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_comparison_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_comparison_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_comparison_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_comparison_monthly_partitioned_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_comparison_monthly_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_comparison_monthly_partitioned_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_comparison_monthly_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_comparison_not_null_count_match_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_comparison_not_null_count_match_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_comparison_null_count_match_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_comparison_null_count_match_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_comparison_profiling_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_comparison_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_comparison_profiling_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_comparison_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_comparison_sum_match_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_comparison_sum_match_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_conversions_daily_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_conversions_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_conversions_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_conversions_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_conversions_daily_partitioned_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_conversions_daily_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_conversions_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_conversions_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_conversions_monthly_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_conversions_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_conversions_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_conversions_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_conversions_monthly_partitioned_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_conversions_monthly_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_conversions_monthly_partitioned_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_conversions_monthly_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_conversions_profiling_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_conversions_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_conversions_profiling_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_conversions_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_current_data_quality_status_model.py` & `dqops-1.2.0/dqops/client/models/dimension_current_data_quality_status_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,64 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..models.rule_severity_level import RuleSeverityLevel
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.column_current_data_quality_status_model_checks import (
-        ColumnCurrentDataQualityStatusModelChecks,
-    )
-
-
-T = TypeVar("T", bound="ColumnCurrentDataQualityStatusModel")
+T = TypeVar("T", bound="DimensionCurrentDataQualityStatusModel")
 
 
 @_attrs_define
-class ColumnCurrentDataQualityStatusModel:
-    """The column's most recent data quality status. It is a summary of the results of the most recently executed data
-    quality checks on the column. Verify the value of the current_severity to see if there are any data quality issues
-    on the column.
-
-        Attributes:
-            current_severity (Union[Unset, RuleSeverityLevel]):
-            highest_historical_severity (Union[Unset, RuleSeverityLevel]):
-            last_check_executed_at (Union[Unset, int]): The UTC timestamp when the most recent data quality check was
-                executed on the column.
-            executed_checks (Union[Unset, int]): The total number of most recent checks that were executed on the column.
-                Table comparison checks that are comparing groups of data are counted as the number of compared data groups.
-            valid_results (Union[Unset, int]): The number of most recent valid data quality checks that passed without
-                raising any issues.
-            warnings (Union[Unset, int]): The number of most recent data quality checks that failed by raising a warning
-                severity data quality issue.
-            errors (Union[Unset, int]): The number of most recent data quality checks that failed by raising an error
-                severity data quality issue.
-            fatals (Union[Unset, int]): The number of most recent data quality checks that failed by raising a fatal
-                severity data quality issue.
-            execution_errors (Union[Unset, int]): The number of data quality check execution errors that were reported due
-                to access issues to the data source, invalid mapping in DQOps, invalid queries in data quality sensors or
-                invalid python rules. When an execution error is reported, the configuration of a data quality check on a column
-                must be updated.
-            checks (Union[Unset, ColumnCurrentDataQualityStatusModelChecks]): The dictionary of statuses for data quality
-                checks. The keys are data quality check names, the values are the current data quality check statuses that
-                describe the most current status.
+class DimensionCurrentDataQualityStatusModel:
+    """The summary of the current data quality status for one data quality dimension
+
+    Attributes:
+        dimension (Union[Unset, str]): Data quality dimension name. The most popular dimensions are: Completeness,
+            Uniqueness, Timeliness, Validity, Consistency, Accuracy, Availability.
+        current_severity (Union[Unset, RuleSeverityLevel]):
+        highest_historical_severity (Union[Unset, RuleSeverityLevel]):
+        last_check_executed_at (Union[Unset, int]): The UTC timestamp when the most recent data quality check was
+            executed on the table.
+        executed_checks (Union[Unset, int]): The total number of most recent checks that were executed on the table for
+            one data quality dimension. Table comparison checks that are comparing groups of data are counted as the number
+            of compared data groups.
+        valid_results (Union[Unset, int]): The number of most recent valid data quality checks that passed without
+            raising any issues.
+        warnings (Union[Unset, int]): The number of most recent data quality checks that failed by raising a warning
+            severity data quality issue.
+        errors (Union[Unset, int]): The number of most recent data quality checks that failed by raising an error
+            severity data quality issue.
+        fatals (Union[Unset, int]): The number of most recent data quality checks that failed by raising a fatal
+            severity data quality issue.
+        execution_errors (Union[Unset, int]): The number of data quality check execution errors that were reported due
+            to access issues to the data source, invalid mapping in DQOps, invalid queries in data quality sensors or
+            invalid python rules. When an execution error is reported, the configuration of a data quality check on a table
+            must be updated.
+        data_quality_kpi (Union[Unset, float]): Data quality KPI score for the data quality dimension, measured as a
+            percentage of passed data quality checks. DQOps counts data quality issues at a warning severity level as passed
+            checks. The data quality KPI score is a value in the range 0..100.
     """
 
+    dimension: Union[Unset, str] = UNSET
     current_severity: Union[Unset, RuleSeverityLevel] = UNSET
     highest_historical_severity: Union[Unset, RuleSeverityLevel] = UNSET
     last_check_executed_at: Union[Unset, int] = UNSET
     executed_checks: Union[Unset, int] = UNSET
     valid_results: Union[Unset, int] = UNSET
     warnings: Union[Unset, int] = UNSET
     errors: Union[Unset, int] = UNSET
     fatals: Union[Unset, int] = UNSET
     execution_errors: Union[Unset, int] = UNSET
-    checks: Union[Unset, "ColumnCurrentDataQualityStatusModelChecks"] = UNSET
+    data_quality_kpi: Union[Unset, float] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
+        dimension = self.dimension
         current_severity: Union[Unset, str] = UNSET
         if not isinstance(self.current_severity, Unset):
             current_severity = self.current_severity.value
 
         highest_historical_severity: Union[Unset, str] = UNSET
         if not isinstance(self.highest_historical_severity, Unset):
             highest_historical_severity = self.highest_historical_severity.value
@@ -69,21 +66,21 @@
         last_check_executed_at = self.last_check_executed_at
         executed_checks = self.executed_checks
         valid_results = self.valid_results
         warnings = self.warnings
         errors = self.errors
         fatals = self.fatals
         execution_errors = self.execution_errors
-        checks: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.checks, Unset):
-            checks = self.checks.to_dict()
+        data_quality_kpi = self.data_quality_kpi
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
+        if dimension is not UNSET:
+            field_dict["dimension"] = dimension
         if current_severity is not UNSET:
             field_dict["current_severity"] = current_severity
         if highest_historical_severity is not UNSET:
             field_dict["highest_historical_severity"] = highest_historical_severity
         if last_check_executed_at is not UNSET:
             field_dict["last_check_executed_at"] = last_check_executed_at
         if executed_checks is not UNSET:
@@ -94,26 +91,24 @@
             field_dict["warnings"] = warnings
         if errors is not UNSET:
             field_dict["errors"] = errors
         if fatals is not UNSET:
             field_dict["fatals"] = fatals
         if execution_errors is not UNSET:
             field_dict["execution_errors"] = execution_errors
-        if checks is not UNSET:
-            field_dict["checks"] = checks
+        if data_quality_kpi is not UNSET:
+            field_dict["data_quality_kpi"] = data_quality_kpi
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.column_current_data_quality_status_model_checks import (
-            ColumnCurrentDataQualityStatusModelChecks,
-        )
-
         d = src_dict.copy()
+        dimension = d.pop("dimension", UNSET)
+
         _current_severity = d.pop("current_severity", UNSET)
         current_severity: Union[Unset, RuleSeverityLevel]
         if isinstance(_current_severity, Unset):
             current_severity = UNSET
         else:
             current_severity = RuleSeverityLevel(_current_severity)
 
@@ -136,36 +131,32 @@
 
         errors = d.pop("errors", UNSET)
 
         fatals = d.pop("fatals", UNSET)
 
         execution_errors = d.pop("execution_errors", UNSET)
 
-        _checks = d.pop("checks", UNSET)
-        checks: Union[Unset, ColumnCurrentDataQualityStatusModelChecks]
-        if isinstance(_checks, Unset):
-            checks = UNSET
-        else:
-            checks = ColumnCurrentDataQualityStatusModelChecks.from_dict(_checks)
+        data_quality_kpi = d.pop("data_quality_kpi", UNSET)
 
-        column_current_data_quality_status_model = cls(
+        dimension_current_data_quality_status_model = cls(
+            dimension=dimension,
             current_severity=current_severity,
             highest_historical_severity=highest_historical_severity,
             last_check_executed_at=last_check_executed_at,
             executed_checks=executed_checks,
             valid_results=valid_results,
             warnings=warnings,
             errors=errors,
             fatals=fatals,
             execution_errors=execution_errors,
-            checks=checks,
+            data_quality_kpi=data_quality_kpi,
         )
 
-        column_current_data_quality_status_model.additional_properties = d
-        return column_current_data_quality_status_model
+        dimension_current_data_quality_status_model.additional_properties = d
+        return dimension_current_data_quality_status_model
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dqops-1.1.0/dqops/client/models/column_current_data_quality_status_model_checks.py` & `dqops-1.2.0/dqops/client/models/column_current_data_quality_status_model_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_custom_sql_daily_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_custom_sql_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_custom_sql_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_custom_sql_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_custom_sql_daily_partitioned_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_custom_sql_daily_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_custom_sql_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_custom_sql_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_custom_sql_monthly_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_custom_sql_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_custom_sql_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_custom_sql_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_custom_sql_monthly_partitioned_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_custom_sql_monthly_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_custom_sql_monthly_partitioned_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_custom_sql_monthly_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_custom_sql_profiling_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_custom_sql_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_custom_sql_profiling_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_custom_sql_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_daily_monitoring_check_categories_spec.py` & `dqops-1.2.0/dqops/client/models/column_daily_monitoring_check_categories_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_daily_monitoring_check_categories_spec_comparisons.py` & `dqops-1.2.0/dqops/client/models/column_daily_monitoring_check_categories_spec_comparisons.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_daily_monitoring_check_categories_spec_custom.py` & `dqops-1.2.0/dqops/client/models/column_daily_monitoring_check_categories_spec_custom.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_daily_partitioned_check_categories_spec.py` & `dqops-1.2.0/dqops/client/models/column_daily_partitioned_check_categories_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_daily_partitioned_check_categories_spec_comparisons.py` & `dqops-1.2.0/dqops/client/models/column_daily_partitioned_check_categories_spec_comparisons.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_daily_partitioned_check_categories_spec_custom.py` & `dqops-1.2.0/dqops/client/models/column_daily_partitioned_check_categories_spec_custom.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_datatype_daily_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_datatype_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_datatype_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_datatype_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_datatype_daily_partitioned_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_datatype_daily_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_datatype_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_datatype_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_datatype_detected_datatype_in_text_changed_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_datatype_detected_datatype_in_text_changed_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_datatype_monthly_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_datatype_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_datatype_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_datatype_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_datatype_monthly_partitioned_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_datatype_monthly_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_datatype_monthly_partitioned_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_datatype_monthly_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_datatype_profiling_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_datatype_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_datatype_profiling_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_datatype_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_datatype_string_datatype_detect_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_datatype_string_datatype_detect_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_date_in_range_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_date_in_range_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_date_in_range_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_date_in_range_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_date_values_in_future_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_date_values_in_future_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_datetime_daily_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_datetime_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_datetime_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_datetime_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_datetime_daily_partitioned_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_datetime_daily_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_datetime_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_datetime_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_datetime_date_values_in_future_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_datetime_date_values_in_future_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_datetime_monthly_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_datetime_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_datetime_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_datetime_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_datetime_monthly_partitioned_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_datetime_monthly_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_datetime_monthly_partitioned_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_datetime_monthly_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_datetime_profiling_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_datetime_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_datetime_profiling_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_datetime_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_default_checks_pattern_spec.py` & `dqops-1.2.0/dqops/client/models/column_default_checks_pattern_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_detected_datatype_in_text_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_detected_datatype_in_text_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_distinct_count_anomaly_differencing_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_distinct_count_anomaly_differencing_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_distinct_count_anomaly_stationary_partition_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_distinct_count_anomaly_stationary_partition_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_distinct_count_change_1_day_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_distinct_count_change_1_day_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_distinct_count_change_30_days_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_distinct_count_change_30_days_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_distinct_count_change_7_days_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_distinct_count_change_7_days_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_distinct_count_change_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_distinct_count_change_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_distinct_count_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_distinct_count_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_distinct_percent_anomaly_stationary_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_distinct_percent_anomaly_stationary_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_distinct_percent_change_1_day_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_distinct_percent_change_1_day_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_distinct_percent_change_30_days_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_distinct_percent_change_30_days_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_distinct_percent_change_7_days_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_distinct_percent_change_7_days_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_distinct_percent_change_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_distinct_percent_change_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_distinct_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_distinct_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_duplicate_count_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_duplicate_count_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_duplicate_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_duplicate_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_expected_numbers_in_use_count_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_expected_numbers_in_use_count_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_expected_text_values_in_use_count_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_expected_text_values_in_use_count_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_expected_texts_in_top_values_count_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_expected_texts_in_top_values_count_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_false_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_false_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_integer_in_range_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_integer_in_range_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_integrity_daily_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_integrity_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_integrity_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_integrity_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_integrity_daily_partitioned_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_integrity_daily_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_integrity_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_integrity_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_integrity_foreign_key_match_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_integrity_foreign_key_match_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_integrity_foreign_key_match_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_integrity_foreign_key_match_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_integrity_foreign_key_not_match_count_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_integrity_foreign_key_not_match_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_integrity_lookup_key_not_found_count_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_integrity_lookup_key_not_found_count_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_integrity_monthly_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_integrity_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_integrity_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_integrity_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_integrity_monthly_partitioned_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_integrity_monthly_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_integrity_monthly_partitioned_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_integrity_monthly_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_integrity_profiling_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_integrity_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_integrity_profiling_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_integrity_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_invalid_email_format_found_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_invalid_email_format_found_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_invalid_ip_4_address_format_found_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_invalid_ip_4_address_format_found_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_invalid_ip_6_address_format_found_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_invalid_ip_6_address_format_found_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_invalid_latitude_count_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_invalid_latitude_count_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_invalid_longitude_count_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_invalid_longitude_count_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_invalid_uuid_format_found_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_invalid_uuid_format_found_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_list_model.py` & `dqops-1.2.0/dqops/client/models/column_list_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union, cast
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
@@ -25,14 +25,15 @@
     """Column list model that returns the basic fields from a column specification, excluding nested nodes like a list of
     activated checks.
 
         Attributes:
             connection_name (Union[Unset, str]): Connection name.
             table (Union[Unset, PhysicalTableName]):
             column_name (Union[Unset, str]): Column names.
+            labels (Union[Unset, List[str]]): List of labels applied to the table.
             sql_expression (Union[Unset, str]): SQL expression.
             column_hash (Union[Unset, int]): Column hash that identifies the column using a unique hash code.
             disabled (Union[Unset, bool]): Disables all data quality checks on the column. Data quality checks will not be
                 executed.
             has_any_configured_checks (Union[Unset, bool]): True when the column has any checks configured.
             has_any_configured_profiling_checks (Union[Unset, bool]): True when the column has any profiling checks
                 configured.
@@ -57,14 +58,15 @@
             can_run_checks (Union[Unset, bool]): Boolean flag that decides if the current user can run checks.
             can_delete_data (Union[Unset, bool]): Boolean flag that decides if the current user can delete data (results).
     """
 
     connection_name: Union[Unset, str] = UNSET
     table: Union[Unset, "PhysicalTableName"] = UNSET
     column_name: Union[Unset, str] = UNSET
+    labels: Union[Unset, List[str]] = UNSET
     sql_expression: Union[Unset, str] = UNSET
     column_hash: Union[Unset, int] = UNSET
     disabled: Union[Unset, bool] = UNSET
     has_any_configured_checks: Union[Unset, bool] = UNSET
     has_any_configured_profiling_checks: Union[Unset, bool] = UNSET
     has_any_configured_monitoring_checks: Union[Unset, bool] = UNSET
     has_any_configured_partition_checks: Union[Unset, bool] = UNSET
@@ -86,14 +88,18 @@
     def to_dict(self) -> Dict[str, Any]:
         connection_name = self.connection_name
         table: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.table, Unset):
             table = self.table.to_dict()
 
         column_name = self.column_name
+        labels: Union[Unset, List[str]] = UNSET
+        if not isinstance(self.labels, Unset):
+            labels = self.labels
+
         sql_expression = self.sql_expression
         column_hash = self.column_hash
         disabled = self.disabled
         has_any_configured_checks = self.has_any_configured_checks
         has_any_configured_profiling_checks = self.has_any_configured_profiling_checks
         has_any_configured_monitoring_checks = self.has_any_configured_monitoring_checks
         has_any_configured_partition_checks = self.has_any_configured_partition_checks
@@ -143,14 +149,16 @@
         field_dict.update({})
         if connection_name is not UNSET:
             field_dict["connection_name"] = connection_name
         if table is not UNSET:
             field_dict["table"] = table
         if column_name is not UNSET:
             field_dict["column_name"] = column_name
+        if labels is not UNSET:
+            field_dict["labels"] = labels
         if sql_expression is not UNSET:
             field_dict["sql_expression"] = sql_expression
         if column_hash is not UNSET:
             field_dict["column_hash"] = column_hash
         if disabled is not UNSET:
             field_dict["disabled"] = disabled
         if has_any_configured_checks is not UNSET:
@@ -220,14 +228,16 @@
         if isinstance(_table, Unset):
             table = UNSET
         else:
             table = PhysicalTableName.from_dict(_table)
 
         column_name = d.pop("column_name", UNSET)
 
+        labels = cast(List[str], d.pop("labels", UNSET))
+
         sql_expression = d.pop("sql_expression", UNSET)
 
         column_hash = d.pop("column_hash", UNSET)
 
         disabled = d.pop("disabled", UNSET)
 
         has_any_configured_checks = d.pop("has_any_configured_checks", UNSET)
@@ -323,14 +333,15 @@
 
         can_delete_data = d.pop("can_delete_data", UNSET)
 
         column_list_model = cls(
             connection_name=connection_name,
             table=table,
             column_name=column_name,
+            labels=labels,
             sql_expression=sql_expression,
             column_hash=column_hash,
             disabled=disabled,
             has_any_configured_checks=has_any_configured_checks,
             has_any_configured_profiling_checks=has_any_configured_profiling_checks,
             has_any_configured_monitoring_checks=has_any_configured_monitoring_checks,
             has_any_configured_partition_checks=has_any_configured_partition_checks,
```

### Comparing `dqops-1.1.0/dqops/client/models/column_max_anomaly_differencing_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_max_anomaly_differencing_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_max_anomaly_stationary_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_max_anomaly_stationary_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_max_in_range_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_max_in_range_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_mean_anomaly_stationary_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_mean_anomaly_stationary_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_mean_change_1_day_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_mean_change_1_day_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_mean_change_30_days_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_mean_change_30_days_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_mean_change_7_days_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_mean_change_7_days_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_mean_change_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_mean_change_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_mean_in_range_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_mean_in_range_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_median_anomaly_stationary_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_median_anomaly_stationary_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_median_change_1_day_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_median_change_1_day_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_median_change_30_days_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_median_change_30_days_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_median_change_7_days_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_median_change_7_days_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_median_change_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_median_change_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_median_in_range_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_median_in_range_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_min_anomaly_differencing_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_min_anomaly_differencing_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_min_anomaly_stationary_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_min_anomaly_stationary_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_min_in_range_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_min_in_range_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_model.py` & `dqops-1.2.0/dqops/client/models/column_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_monitoring_check_categories_spec.py` & `dqops-1.2.0/dqops/client/models/column_monitoring_check_categories_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_monthly_monitoring_check_categories_spec.py` & `dqops-1.2.0/dqops/client/models/column_monthly_monitoring_check_categories_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_monthly_monitoring_check_categories_spec_comparisons.py` & `dqops-1.2.0/dqops/client/models/column_monthly_monitoring_check_categories_spec_comparisons.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_monthly_monitoring_check_categories_spec_custom.py` & `dqops-1.2.0/dqops/client/models/column_monthly_monitoring_check_categories_spec_custom.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_monthly_partitioned_check_categories_spec.py` & `dqops-1.2.0/dqops/client/models/column_monthly_partitioned_check_categories_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_monthly_partitioned_check_categories_spec_comparisons.py` & `dqops-1.2.0/dqops/client/models/column_monthly_partitioned_check_categories_spec_comparisons.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_monthly_partitioned_check_categories_spec_custom.py` & `dqops-1.2.0/dqops/client/models/column_monthly_partitioned_check_categories_spec_custom.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_negative_count_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_negative_count_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_negative_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_negative_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_non_negative_count_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_non_negative_count_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_non_negative_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_non_negative_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_not_nulls_count_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_not_nulls_count_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_not_nulls_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_not_nulls_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_null_percent_anomaly_stationary_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_null_percent_anomaly_stationary_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_null_percent_change_1_day_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_null_percent_change_1_day_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_null_percent_change_30_days_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_null_percent_change_30_days_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_null_percent_change_7_days_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_null_percent_change_7_days_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_null_percent_change_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_null_percent_change_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_nulls_count_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_nulls_count_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_nulls_daily_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_nulls_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_nulls_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_nulls_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_nulls_daily_partitioned_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_nulls_daily_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_nulls_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_nulls_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_nulls_monthly_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_nulls_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_nulls_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_nulls_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_nulls_monthly_partitioned_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_nulls_monthly_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_nulls_monthly_partitioned_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_nulls_monthly_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_nulls_not_nulls_count_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_nulls_not_nulls_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_nulls_not_nulls_count_statistics_collector_spec.py` & `dqops-1.2.0/dqops/client/models/column_nulls_not_nulls_count_statistics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_nulls_not_nulls_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_nulls_not_nulls_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_nulls_not_nulls_percent_statistics_collector_spec.py` & `dqops-1.2.0/dqops/client/models/column_nulls_not_nulls_percent_statistics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_nulls_nulls_count_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_nulls_nulls_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_nulls_nulls_count_statistics_collector_spec.py` & `dqops-1.2.0/dqops/client/models/column_nulls_nulls_count_statistics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_nulls_nulls_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_nulls_nulls_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_nulls_nulls_percent_statistics_collector_spec.py` & `dqops-1.2.0/dqops/client/models/column_nulls_nulls_percent_statistics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_nulls_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_nulls_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_nulls_profiling_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_nulls_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_nulls_profiling_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_nulls_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_nulls_statistics_collectors_spec.py` & `dqops-1.2.0/dqops/client/models/column_nulls_statistics_collectors_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_number_above_max_value_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_number_above_max_value_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_number_above_max_value_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_number_above_max_value_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_number_below_min_value_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_number_below_min_value_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_number_below_min_value_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_number_below_min_value_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_number_found_in_set_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_number_found_in_set_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_number_in_range_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_number_in_range_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_daily_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_numeric_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_numeric_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_daily_partitioned_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_numeric_daily_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_numeric_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_expected_numbers_in_use_count_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_numeric_expected_numbers_in_use_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_integer_in_range_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_numeric_integer_in_range_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_invalid_latitude_count_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_numeric_invalid_latitude_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_invalid_longitude_count_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_numeric_invalid_longitude_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_max_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_numeric_max_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_mean_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_numeric_mean_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_median_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_numeric_median_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_min_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_numeric_min_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_monthly_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_numeric_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_numeric_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_monthly_partitioned_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_numeric_monthly_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_monthly_partitioned_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_numeric_monthly_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_negative_count_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_numeric_negative_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_negative_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_numeric_negative_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_non_negative_count_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_numeric_non_negative_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_non_negative_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_numeric_non_negative_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_number_above_max_value_count_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_numeric_number_above_max_value_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_number_above_max_value_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_numeric_number_above_max_value_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_number_below_min_value_count_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_numeric_number_below_min_value_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_number_below_min_value_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_numeric_number_below_min_value_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_number_found_in_set_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_numeric_number_found_in_set_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_number_in_range_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_numeric_number_in_range_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_percentile_10_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_numeric_percentile_10_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_percentile_25_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_numeric_percentile_25_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_percentile_75_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_numeric_percentile_75_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_percentile_90_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_numeric_percentile_90_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_percentile_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_numeric_percentile_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_population_stddev_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_numeric_population_stddev_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_population_variance_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_numeric_population_variance_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_profiling_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_numeric_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_profiling_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_numeric_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_sample_stddev_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_numeric_sample_stddev_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_sample_variance_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_numeric_sample_variance_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_sum_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_numeric_sum_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_valid_latitude_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_numeric_valid_latitude_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_numeric_valid_longitude_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_numeric_valid_longitude_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_partitioned_check_categories_spec.py` & `dqops-1.2.0/dqops/client/models/column_partitioned_check_categories_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_patterns_daily_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_patterns_daily_monitoring_checks_spec.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
     from ..models.column_invalid_email_format_found_check_spec import (
         ColumnInvalidEmailFormatFoundCheckSpec,
     )
+    from ..models.column_invalid_email_format_percent_check_spec import (
+        ColumnInvalidEmailFormatPercentCheckSpec,
+    )
     from ..models.column_invalid_ip_4_address_format_found_check_spec import (
         ColumnInvalidIp4AddressFormatFoundCheckSpec,
     )
     from ..models.column_invalid_ip_6_address_format_found_check_spec import (
         ColumnInvalidIp6AddressFormatFoundCheckSpec,
     )
     from ..models.column_invalid_uuid_format_found_check_spec import (
@@ -50,14 +53,15 @@
     Attributes:
         custom_checks (Union[Unset, ColumnPatternsDailyMonitoringChecksSpecCustomChecks]): Dictionary of additional
             custom checks within this category. The keys are check names defined in the definition section. The sensor
             parameters and rules should match the type of the configured sensor and rule for the custom check.
         daily_text_not_matching_regex_found (Union[Unset, ColumnTextNotMatchingRegexFoundCheckSpec]):
         daily_texts_matching_regex_percent (Union[Unset, ColumnTextsMatchingRegexPercentCheckSpec]):
         daily_invalid_email_format_found (Union[Unset, ColumnInvalidEmailFormatFoundCheckSpec]):
+        daily_invalid_email_format_percent (Union[Unset, ColumnInvalidEmailFormatPercentCheckSpec]):
         daily_text_not_matching_date_pattern_found (Union[Unset, ColumnTextNotMatchingDatePatternFoundCheckSpec]):
         daily_text_matching_date_pattern_percent (Union[Unset, ColumnTextMatchingDatePatternPercentCheckSpec]):
         daily_text_matching_name_pattern_percent (Union[Unset, ColumnTextMatchingNamePatternPercentCheckSpec]):
         daily_invalid_uuid_format_found (Union[Unset, ColumnInvalidUuidFormatFoundCheckSpec]):
         daily_valid_uuid_format_percent (Union[Unset, ColumnValidUuidFormatPercentCheckSpec]):
         daily_invalid_ip4_address_format_found (Union[Unset, ColumnInvalidIp4AddressFormatFoundCheckSpec]):
         daily_invalid_ip6_address_format_found (Union[Unset, ColumnInvalidIp6AddressFormatFoundCheckSpec]):
@@ -71,14 +75,17 @@
     ] = UNSET
     daily_texts_matching_regex_percent: Union[
         Unset, "ColumnTextsMatchingRegexPercentCheckSpec"
     ] = UNSET
     daily_invalid_email_format_found: Union[
         Unset, "ColumnInvalidEmailFormatFoundCheckSpec"
     ] = UNSET
+    daily_invalid_email_format_percent: Union[
+        Unset, "ColumnInvalidEmailFormatPercentCheckSpec"
+    ] = UNSET
     daily_text_not_matching_date_pattern_found: Union[
         Unset, "ColumnTextNotMatchingDatePatternFoundCheckSpec"
     ] = UNSET
     daily_text_matching_date_pattern_percent: Union[
         Unset, "ColumnTextMatchingDatePatternPercentCheckSpec"
     ] = UNSET
     daily_text_matching_name_pattern_percent: Union[
@@ -117,14 +124,20 @@
 
         daily_invalid_email_format_found: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.daily_invalid_email_format_found, Unset):
             daily_invalid_email_format_found = (
                 self.daily_invalid_email_format_found.to_dict()
             )
 
+        daily_invalid_email_format_percent: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.daily_invalid_email_format_percent, Unset):
+            daily_invalid_email_format_percent = (
+                self.daily_invalid_email_format_percent.to_dict()
+            )
+
         daily_text_not_matching_date_pattern_found: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.daily_text_not_matching_date_pattern_found, Unset):
             daily_text_not_matching_date_pattern_found = (
                 self.daily_text_not_matching_date_pattern_found.to_dict()
             )
 
         daily_text_matching_date_pattern_percent: Union[Unset, Dict[str, Any]] = UNSET
@@ -176,14 +189,18 @@
             field_dict[
                 "daily_texts_matching_regex_percent"
             ] = daily_texts_matching_regex_percent
         if daily_invalid_email_format_found is not UNSET:
             field_dict[
                 "daily_invalid_email_format_found"
             ] = daily_invalid_email_format_found
+        if daily_invalid_email_format_percent is not UNSET:
+            field_dict[
+                "daily_invalid_email_format_percent"
+            ] = daily_invalid_email_format_percent
         if daily_text_not_matching_date_pattern_found is not UNSET:
             field_dict[
                 "daily_text_not_matching_date_pattern_found"
             ] = daily_text_not_matching_date_pattern_found
         if daily_text_matching_date_pattern_percent is not UNSET:
             field_dict[
                 "daily_text_matching_date_pattern_percent"
@@ -212,14 +229,17 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.column_invalid_email_format_found_check_spec import (
             ColumnInvalidEmailFormatFoundCheckSpec,
         )
+        from ..models.column_invalid_email_format_percent_check_spec import (
+            ColumnInvalidEmailFormatPercentCheckSpec,
+        )
         from ..models.column_invalid_ip_4_address_format_found_check_spec import (
             ColumnInvalidIp4AddressFormatFoundCheckSpec,
         )
         from ..models.column_invalid_ip_6_address_format_found_check_spec import (
             ColumnInvalidIp6AddressFormatFoundCheckSpec,
         )
         from ..models.column_invalid_uuid_format_found_check_spec import (
@@ -300,14 +320,29 @@
         else:
             daily_invalid_email_format_found = (
                 ColumnInvalidEmailFormatFoundCheckSpec.from_dict(
                     _daily_invalid_email_format_found
                 )
             )
 
+        _daily_invalid_email_format_percent = d.pop(
+            "daily_invalid_email_format_percent", UNSET
+        )
+        daily_invalid_email_format_percent: Union[
+            Unset, ColumnInvalidEmailFormatPercentCheckSpec
+        ]
+        if isinstance(_daily_invalid_email_format_percent, Unset):
+            daily_invalid_email_format_percent = UNSET
+        else:
+            daily_invalid_email_format_percent = (
+                ColumnInvalidEmailFormatPercentCheckSpec.from_dict(
+                    _daily_invalid_email_format_percent
+                )
+            )
+
         _daily_text_not_matching_date_pattern_found = d.pop(
             "daily_text_not_matching_date_pattern_found", UNSET
         )
         daily_text_not_matching_date_pattern_found: Union[
             Unset, ColumnTextNotMatchingDatePatternFoundCheckSpec
         ]
         if isinstance(_daily_text_not_matching_date_pattern_found, Unset):
@@ -410,14 +445,15 @@
             )
 
         column_patterns_daily_monitoring_checks_spec = cls(
             custom_checks=custom_checks,
             daily_text_not_matching_regex_found=daily_text_not_matching_regex_found,
             daily_texts_matching_regex_percent=daily_texts_matching_regex_percent,
             daily_invalid_email_format_found=daily_invalid_email_format_found,
+            daily_invalid_email_format_percent=daily_invalid_email_format_percent,
             daily_text_not_matching_date_pattern_found=daily_text_not_matching_date_pattern_found,
             daily_text_matching_date_pattern_percent=daily_text_matching_date_pattern_percent,
             daily_text_matching_name_pattern_percent=daily_text_matching_name_pattern_percent,
             daily_invalid_uuid_format_found=daily_invalid_uuid_format_found,
             daily_valid_uuid_format_percent=daily_valid_uuid_format_percent,
             daily_invalid_ip4_address_format_found=daily_invalid_ip4_address_format_found,
             daily_invalid_ip6_address_format_found=daily_invalid_ip6_address_format_found,
```

### Comparing `dqops-1.1.0/dqops/client/models/column_patterns_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_patterns_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_patterns_daily_partitioned_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_patterns_daily_partitioned_checks_spec.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
     from ..models.column_invalid_email_format_found_check_spec import (
         ColumnInvalidEmailFormatFoundCheckSpec,
     )
+    from ..models.column_invalid_email_format_percent_check_spec import (
+        ColumnInvalidEmailFormatPercentCheckSpec,
+    )
     from ..models.column_invalid_ip_4_address_format_found_check_spec import (
         ColumnInvalidIp4AddressFormatFoundCheckSpec,
     )
     from ..models.column_invalid_ip_6_address_format_found_check_spec import (
         ColumnInvalidIp6AddressFormatFoundCheckSpec,
     )
     from ..models.column_invalid_uuid_format_found_check_spec import (
@@ -50,14 +53,15 @@
     Attributes:
         custom_checks (Union[Unset, ColumnPatternsDailyPartitionedChecksSpecCustomChecks]): Dictionary of additional
             custom checks within this category. The keys are check names defined in the definition section. The sensor
             parameters and rules should match the type of the configured sensor and rule for the custom check.
         daily_partition_text_not_matching_regex_found (Union[Unset, ColumnTextNotMatchingRegexFoundCheckSpec]):
         daily_partition_texts_matching_regex_percent (Union[Unset, ColumnTextsMatchingRegexPercentCheckSpec]):
         daily_partition_invalid_email_format_found (Union[Unset, ColumnInvalidEmailFormatFoundCheckSpec]):
+        daily_partition_invalid_email_format_percent (Union[Unset, ColumnInvalidEmailFormatPercentCheckSpec]):
         daily_partition_text_not_matching_date_pattern_found (Union[Unset,
             ColumnTextNotMatchingDatePatternFoundCheckSpec]):
         daily_partition_text_matching_date_pattern_percent (Union[Unset,
             ColumnTextMatchingDatePatternPercentCheckSpec]):
         daily_partition_text_matching_name_pattern_percent (Union[Unset,
             ColumnTextMatchingNamePatternPercentCheckSpec]):
         daily_partition_invalid_uuid_format_found (Union[Unset, ColumnInvalidUuidFormatFoundCheckSpec]):
@@ -74,14 +78,17 @@
     ] = UNSET
     daily_partition_texts_matching_regex_percent: Union[
         Unset, "ColumnTextsMatchingRegexPercentCheckSpec"
     ] = UNSET
     daily_partition_invalid_email_format_found: Union[
         Unset, "ColumnInvalidEmailFormatFoundCheckSpec"
     ] = UNSET
+    daily_partition_invalid_email_format_percent: Union[
+        Unset, "ColumnInvalidEmailFormatPercentCheckSpec"
+    ] = UNSET
     daily_partition_text_not_matching_date_pattern_found: Union[
         Unset, "ColumnTextNotMatchingDatePatternFoundCheckSpec"
     ] = UNSET
     daily_partition_text_matching_date_pattern_percent: Union[
         Unset, "ColumnTextMatchingDatePatternPercentCheckSpec"
     ] = UNSET
     daily_partition_text_matching_name_pattern_percent: Union[
@@ -124,14 +131,22 @@
 
         daily_partition_invalid_email_format_found: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.daily_partition_invalid_email_format_found, Unset):
             daily_partition_invalid_email_format_found = (
                 self.daily_partition_invalid_email_format_found.to_dict()
             )
 
+        daily_partition_invalid_email_format_percent: Union[
+            Unset, Dict[str, Any]
+        ] = UNSET
+        if not isinstance(self.daily_partition_invalid_email_format_percent, Unset):
+            daily_partition_invalid_email_format_percent = (
+                self.daily_partition_invalid_email_format_percent.to_dict()
+            )
+
         daily_partition_text_not_matching_date_pattern_found: Union[
             Unset, Dict[str, Any]
         ] = UNSET
         if not isinstance(
             self.daily_partition_text_not_matching_date_pattern_found, Unset
         ):
             daily_partition_text_not_matching_date_pattern_found = (
@@ -199,14 +214,18 @@
             field_dict[
                 "daily_partition_texts_matching_regex_percent"
             ] = daily_partition_texts_matching_regex_percent
         if daily_partition_invalid_email_format_found is not UNSET:
             field_dict[
                 "daily_partition_invalid_email_format_found"
             ] = daily_partition_invalid_email_format_found
+        if daily_partition_invalid_email_format_percent is not UNSET:
+            field_dict[
+                "daily_partition_invalid_email_format_percent"
+            ] = daily_partition_invalid_email_format_percent
         if daily_partition_text_not_matching_date_pattern_found is not UNSET:
             field_dict[
                 "daily_partition_text_not_matching_date_pattern_found"
             ] = daily_partition_text_not_matching_date_pattern_found
         if daily_partition_text_matching_date_pattern_percent is not UNSET:
             field_dict[
                 "daily_partition_text_matching_date_pattern_percent"
@@ -235,14 +254,17 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.column_invalid_email_format_found_check_spec import (
             ColumnInvalidEmailFormatFoundCheckSpec,
         )
+        from ..models.column_invalid_email_format_percent_check_spec import (
+            ColumnInvalidEmailFormatPercentCheckSpec,
+        )
         from ..models.column_invalid_ip_4_address_format_found_check_spec import (
             ColumnInvalidIp4AddressFormatFoundCheckSpec,
         )
         from ..models.column_invalid_ip_6_address_format_found_check_spec import (
             ColumnInvalidIp6AddressFormatFoundCheckSpec,
         )
         from ..models.column_invalid_uuid_format_found_check_spec import (
@@ -325,14 +347,29 @@
         else:
             daily_partition_invalid_email_format_found = (
                 ColumnInvalidEmailFormatFoundCheckSpec.from_dict(
                     _daily_partition_invalid_email_format_found
                 )
             )
 
+        _daily_partition_invalid_email_format_percent = d.pop(
+            "daily_partition_invalid_email_format_percent", UNSET
+        )
+        daily_partition_invalid_email_format_percent: Union[
+            Unset, ColumnInvalidEmailFormatPercentCheckSpec
+        ]
+        if isinstance(_daily_partition_invalid_email_format_percent, Unset):
+            daily_partition_invalid_email_format_percent = UNSET
+        else:
+            daily_partition_invalid_email_format_percent = (
+                ColumnInvalidEmailFormatPercentCheckSpec.from_dict(
+                    _daily_partition_invalid_email_format_percent
+                )
+            )
+
         _daily_partition_text_not_matching_date_pattern_found = d.pop(
             "daily_partition_text_not_matching_date_pattern_found", UNSET
         )
         daily_partition_text_not_matching_date_pattern_found: Union[
             Unset, ColumnTextNotMatchingDatePatternFoundCheckSpec
         ]
         if isinstance(_daily_partition_text_not_matching_date_pattern_found, Unset):
@@ -435,14 +472,15 @@
             )
 
         column_patterns_daily_partitioned_checks_spec = cls(
             custom_checks=custom_checks,
             daily_partition_text_not_matching_regex_found=daily_partition_text_not_matching_regex_found,
             daily_partition_texts_matching_regex_percent=daily_partition_texts_matching_regex_percent,
             daily_partition_invalid_email_format_found=daily_partition_invalid_email_format_found,
+            daily_partition_invalid_email_format_percent=daily_partition_invalid_email_format_percent,
             daily_partition_text_not_matching_date_pattern_found=daily_partition_text_not_matching_date_pattern_found,
             daily_partition_text_matching_date_pattern_percent=daily_partition_text_matching_date_pattern_percent,
             daily_partition_text_matching_name_pattern_percent=daily_partition_text_matching_name_pattern_percent,
             daily_partition_invalid_uuid_format_found=daily_partition_invalid_uuid_format_found,
             daily_partition_valid_uuid_format_percent=daily_partition_valid_uuid_format_percent,
             daily_partition_invalid_ip4_address_format_found=daily_partition_invalid_ip4_address_format_found,
             daily_partition_invalid_ip6_address_format_found=daily_partition_invalid_ip6_address_format_found,
```

### Comparing `dqops-1.1.0/dqops/client/models/column_patterns_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_patterns_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_patterns_invalid_email_format_count_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_patterns_invalid_email_format_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_patterns_invalid_ip_4_address_format_count_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_patterns_invalid_ip_4_address_format_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_patterns_invalid_ip_6_address_format_count_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_patterns_invalid_ip_6_address_format_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_patterns_invalid_uuid_format_count_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_patterns_invalid_uuid_format_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_patterns_monthly_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_patterns_monthly_monitoring_checks_spec.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
     from ..models.column_invalid_email_format_found_check_spec import (
         ColumnInvalidEmailFormatFoundCheckSpec,
     )
+    from ..models.column_invalid_email_format_percent_check_spec import (
+        ColumnInvalidEmailFormatPercentCheckSpec,
+    )
     from ..models.column_invalid_ip_4_address_format_found_check_spec import (
         ColumnInvalidIp4AddressFormatFoundCheckSpec,
     )
     from ..models.column_invalid_ip_6_address_format_found_check_spec import (
         ColumnInvalidIp6AddressFormatFoundCheckSpec,
     )
     from ..models.column_invalid_uuid_format_found_check_spec import (
@@ -50,14 +53,15 @@
     Attributes:
         custom_checks (Union[Unset, ColumnPatternsMonthlyMonitoringChecksSpecCustomChecks]): Dictionary of additional
             custom checks within this category. The keys are check names defined in the definition section. The sensor
             parameters and rules should match the type of the configured sensor and rule for the custom check.
         monthly_text_not_matching_regex_found (Union[Unset, ColumnTextNotMatchingRegexFoundCheckSpec]):
         monthly_texts_matching_regex_percent (Union[Unset, ColumnTextsMatchingRegexPercentCheckSpec]):
         monthly_invalid_email_format_found (Union[Unset, ColumnInvalidEmailFormatFoundCheckSpec]):
+        monthly_invalid_email_format_percent (Union[Unset, ColumnInvalidEmailFormatPercentCheckSpec]):
         monthly_text_not_matching_date_pattern_found (Union[Unset, ColumnTextNotMatchingDatePatternFoundCheckSpec]):
         monthly_text_matching_date_pattern_percent (Union[Unset, ColumnTextMatchingDatePatternPercentCheckSpec]):
         monthly_text_matching_name_pattern_percent (Union[Unset, ColumnTextMatchingNamePatternPercentCheckSpec]):
         monthly_invalid_uuid_format_found (Union[Unset, ColumnInvalidUuidFormatFoundCheckSpec]):
         monthly_valid_uuid_format_percent (Union[Unset, ColumnValidUuidFormatPercentCheckSpec]):
         monthly_invalid_ip4_address_format_found (Union[Unset, ColumnInvalidIp4AddressFormatFoundCheckSpec]):
         monthly_invalid_ip6_address_format_found (Union[Unset, ColumnInvalidIp6AddressFormatFoundCheckSpec]):
@@ -71,14 +75,17 @@
     ] = UNSET
     monthly_texts_matching_regex_percent: Union[
         Unset, "ColumnTextsMatchingRegexPercentCheckSpec"
     ] = UNSET
     monthly_invalid_email_format_found: Union[
         Unset, "ColumnInvalidEmailFormatFoundCheckSpec"
     ] = UNSET
+    monthly_invalid_email_format_percent: Union[
+        Unset, "ColumnInvalidEmailFormatPercentCheckSpec"
+    ] = UNSET
     monthly_text_not_matching_date_pattern_found: Union[
         Unset, "ColumnTextNotMatchingDatePatternFoundCheckSpec"
     ] = UNSET
     monthly_text_matching_date_pattern_percent: Union[
         Unset, "ColumnTextMatchingDatePatternPercentCheckSpec"
     ] = UNSET
     monthly_text_matching_name_pattern_percent: Union[
@@ -117,14 +124,20 @@
 
         monthly_invalid_email_format_found: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.monthly_invalid_email_format_found, Unset):
             monthly_invalid_email_format_found = (
                 self.monthly_invalid_email_format_found.to_dict()
             )
 
+        monthly_invalid_email_format_percent: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.monthly_invalid_email_format_percent, Unset):
+            monthly_invalid_email_format_percent = (
+                self.monthly_invalid_email_format_percent.to_dict()
+            )
+
         monthly_text_not_matching_date_pattern_found: Union[
             Unset, Dict[str, Any]
         ] = UNSET
         if not isinstance(self.monthly_text_not_matching_date_pattern_found, Unset):
             monthly_text_not_matching_date_pattern_found = (
                 self.monthly_text_not_matching_date_pattern_found.to_dict()
             )
@@ -178,14 +191,18 @@
             field_dict[
                 "monthly_texts_matching_regex_percent"
             ] = monthly_texts_matching_regex_percent
         if monthly_invalid_email_format_found is not UNSET:
             field_dict[
                 "monthly_invalid_email_format_found"
             ] = monthly_invalid_email_format_found
+        if monthly_invalid_email_format_percent is not UNSET:
+            field_dict[
+                "monthly_invalid_email_format_percent"
+            ] = monthly_invalid_email_format_percent
         if monthly_text_not_matching_date_pattern_found is not UNSET:
             field_dict[
                 "monthly_text_not_matching_date_pattern_found"
             ] = monthly_text_not_matching_date_pattern_found
         if monthly_text_matching_date_pattern_percent is not UNSET:
             field_dict[
                 "monthly_text_matching_date_pattern_percent"
@@ -214,14 +231,17 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.column_invalid_email_format_found_check_spec import (
             ColumnInvalidEmailFormatFoundCheckSpec,
         )
+        from ..models.column_invalid_email_format_percent_check_spec import (
+            ColumnInvalidEmailFormatPercentCheckSpec,
+        )
         from ..models.column_invalid_ip_4_address_format_found_check_spec import (
             ColumnInvalidIp4AddressFormatFoundCheckSpec,
         )
         from ..models.column_invalid_ip_6_address_format_found_check_spec import (
             ColumnInvalidIp6AddressFormatFoundCheckSpec,
         )
         from ..models.column_invalid_uuid_format_found_check_spec import (
@@ -304,14 +324,29 @@
         else:
             monthly_invalid_email_format_found = (
                 ColumnInvalidEmailFormatFoundCheckSpec.from_dict(
                     _monthly_invalid_email_format_found
                 )
             )
 
+        _monthly_invalid_email_format_percent = d.pop(
+            "monthly_invalid_email_format_percent", UNSET
+        )
+        monthly_invalid_email_format_percent: Union[
+            Unset, ColumnInvalidEmailFormatPercentCheckSpec
+        ]
+        if isinstance(_monthly_invalid_email_format_percent, Unset):
+            monthly_invalid_email_format_percent = UNSET
+        else:
+            monthly_invalid_email_format_percent = (
+                ColumnInvalidEmailFormatPercentCheckSpec.from_dict(
+                    _monthly_invalid_email_format_percent
+                )
+            )
+
         _monthly_text_not_matching_date_pattern_found = d.pop(
             "monthly_text_not_matching_date_pattern_found", UNSET
         )
         monthly_text_not_matching_date_pattern_found: Union[
             Unset, ColumnTextNotMatchingDatePatternFoundCheckSpec
         ]
         if isinstance(_monthly_text_not_matching_date_pattern_found, Unset):
@@ -414,14 +449,15 @@
             )
 
         column_patterns_monthly_monitoring_checks_spec = cls(
             custom_checks=custom_checks,
             monthly_text_not_matching_regex_found=monthly_text_not_matching_regex_found,
             monthly_texts_matching_regex_percent=monthly_texts_matching_regex_percent,
             monthly_invalid_email_format_found=monthly_invalid_email_format_found,
+            monthly_invalid_email_format_percent=monthly_invalid_email_format_percent,
             monthly_text_not_matching_date_pattern_found=monthly_text_not_matching_date_pattern_found,
             monthly_text_matching_date_pattern_percent=monthly_text_matching_date_pattern_percent,
             monthly_text_matching_name_pattern_percent=monthly_text_matching_name_pattern_percent,
             monthly_invalid_uuid_format_found=monthly_invalid_uuid_format_found,
             monthly_valid_uuid_format_percent=monthly_valid_uuid_format_percent,
             monthly_invalid_ip4_address_format_found=monthly_invalid_ip4_address_format_found,
             monthly_invalid_ip6_address_format_found=monthly_invalid_ip6_address_format_found,
```

### Comparing `dqops-1.1.0/dqops/client/models/column_patterns_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_patterns_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_patterns_monthly_partitioned_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_patterns_monthly_partitioned_checks_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
     from ..models.column_invalid_email_format_found_check_spec import (
         ColumnInvalidEmailFormatFoundCheckSpec,
     )
+    from ..models.column_invalid_email_format_percent_check_spec import (
+        ColumnInvalidEmailFormatPercentCheckSpec,
+    )
     from ..models.column_invalid_ip_4_address_format_found_check_spec import (
         ColumnInvalidIp4AddressFormatFoundCheckSpec,
     )
     from ..models.column_invalid_ip_6_address_format_found_check_spec import (
         ColumnInvalidIp6AddressFormatFoundCheckSpec,
     )
     from ..models.column_invalid_uuid_format_found_check_spec import (
@@ -50,14 +53,15 @@
     Attributes:
         custom_checks (Union[Unset, ColumnPatternsMonthlyPartitionedChecksSpecCustomChecks]): Dictionary of additional
             custom checks within this category. The keys are check names defined in the definition section. The sensor
             parameters and rules should match the type of the configured sensor and rule for the custom check.
         monthly_partition_text_not_matching_regex_found (Union[Unset, ColumnTextNotMatchingRegexFoundCheckSpec]):
         monthly_partition_texts_matching_regex_percent (Union[Unset, ColumnTextsMatchingRegexPercentCheckSpec]):
         monthly_partition_invalid_email_format_found (Union[Unset, ColumnInvalidEmailFormatFoundCheckSpec]):
+        monthly_partition_invalid_email_format_percent (Union[Unset, ColumnInvalidEmailFormatPercentCheckSpec]):
         monthly_partition_text_not_matching_date_pattern_found (Union[Unset,
             ColumnTextNotMatchingDatePatternFoundCheckSpec]):
         monthly_partition_text_matching_date_pattern_percent (Union[Unset,
             ColumnTextMatchingDatePatternPercentCheckSpec]):
         monthly_partition_text_matching_name_pattern_percent (Union[Unset,
             ColumnTextMatchingNamePatternPercentCheckSpec]):
         monthly_partition_invalid_uuid_format_found (Union[Unset, ColumnInvalidUuidFormatFoundCheckSpec]):
@@ -74,14 +78,17 @@
     ] = UNSET
     monthly_partition_texts_matching_regex_percent: Union[
         Unset, "ColumnTextsMatchingRegexPercentCheckSpec"
     ] = UNSET
     monthly_partition_invalid_email_format_found: Union[
         Unset, "ColumnInvalidEmailFormatFoundCheckSpec"
     ] = UNSET
+    monthly_partition_invalid_email_format_percent: Union[
+        Unset, "ColumnInvalidEmailFormatPercentCheckSpec"
+    ] = UNSET
     monthly_partition_text_not_matching_date_pattern_found: Union[
         Unset, "ColumnTextNotMatchingDatePatternFoundCheckSpec"
     ] = UNSET
     monthly_partition_text_matching_date_pattern_percent: Union[
         Unset, "ColumnTextMatchingDatePatternPercentCheckSpec"
     ] = UNSET
     monthly_partition_text_matching_name_pattern_percent: Union[
@@ -126,14 +133,22 @@
             Unset, Dict[str, Any]
         ] = UNSET
         if not isinstance(self.monthly_partition_invalid_email_format_found, Unset):
             monthly_partition_invalid_email_format_found = (
                 self.monthly_partition_invalid_email_format_found.to_dict()
             )
 
+        monthly_partition_invalid_email_format_percent: Union[
+            Unset, Dict[str, Any]
+        ] = UNSET
+        if not isinstance(self.monthly_partition_invalid_email_format_percent, Unset):
+            monthly_partition_invalid_email_format_percent = (
+                self.monthly_partition_invalid_email_format_percent.to_dict()
+            )
+
         monthly_partition_text_not_matching_date_pattern_found: Union[
             Unset, Dict[str, Any]
         ] = UNSET
         if not isinstance(
             self.monthly_partition_text_not_matching_date_pattern_found, Unset
         ):
             monthly_partition_text_not_matching_date_pattern_found = (
@@ -209,14 +224,18 @@
             field_dict[
                 "monthly_partition_texts_matching_regex_percent"
             ] = monthly_partition_texts_matching_regex_percent
         if monthly_partition_invalid_email_format_found is not UNSET:
             field_dict[
                 "monthly_partition_invalid_email_format_found"
             ] = monthly_partition_invalid_email_format_found
+        if monthly_partition_invalid_email_format_percent is not UNSET:
+            field_dict[
+                "monthly_partition_invalid_email_format_percent"
+            ] = monthly_partition_invalid_email_format_percent
         if monthly_partition_text_not_matching_date_pattern_found is not UNSET:
             field_dict[
                 "monthly_partition_text_not_matching_date_pattern_found"
             ] = monthly_partition_text_not_matching_date_pattern_found
         if monthly_partition_text_matching_date_pattern_percent is not UNSET:
             field_dict[
                 "monthly_partition_text_matching_date_pattern_percent"
@@ -245,14 +264,17 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.column_invalid_email_format_found_check_spec import (
             ColumnInvalidEmailFormatFoundCheckSpec,
         )
+        from ..models.column_invalid_email_format_percent_check_spec import (
+            ColumnInvalidEmailFormatPercentCheckSpec,
+        )
         from ..models.column_invalid_ip_4_address_format_found_check_spec import (
             ColumnInvalidIp4AddressFormatFoundCheckSpec,
         )
         from ..models.column_invalid_ip_6_address_format_found_check_spec import (
             ColumnInvalidIp6AddressFormatFoundCheckSpec,
         )
         from ..models.column_invalid_uuid_format_found_check_spec import (
@@ -335,14 +357,29 @@
         else:
             monthly_partition_invalid_email_format_found = (
                 ColumnInvalidEmailFormatFoundCheckSpec.from_dict(
                     _monthly_partition_invalid_email_format_found
                 )
             )
 
+        _monthly_partition_invalid_email_format_percent = d.pop(
+            "monthly_partition_invalid_email_format_percent", UNSET
+        )
+        monthly_partition_invalid_email_format_percent: Union[
+            Unset, ColumnInvalidEmailFormatPercentCheckSpec
+        ]
+        if isinstance(_monthly_partition_invalid_email_format_percent, Unset):
+            monthly_partition_invalid_email_format_percent = UNSET
+        else:
+            monthly_partition_invalid_email_format_percent = (
+                ColumnInvalidEmailFormatPercentCheckSpec.from_dict(
+                    _monthly_partition_invalid_email_format_percent
+                )
+            )
+
         _monthly_partition_text_not_matching_date_pattern_found = d.pop(
             "monthly_partition_text_not_matching_date_pattern_found", UNSET
         )
         monthly_partition_text_not_matching_date_pattern_found: Union[
             Unset, ColumnTextNotMatchingDatePatternFoundCheckSpec
         ]
         if isinstance(_monthly_partition_text_not_matching_date_pattern_found, Unset):
@@ -445,14 +482,15 @@
             )
 
         column_patterns_monthly_partitioned_checks_spec = cls(
             custom_checks=custom_checks,
             monthly_partition_text_not_matching_regex_found=monthly_partition_text_not_matching_regex_found,
             monthly_partition_texts_matching_regex_percent=monthly_partition_texts_matching_regex_percent,
             monthly_partition_invalid_email_format_found=monthly_partition_invalid_email_format_found,
+            monthly_partition_invalid_email_format_percent=monthly_partition_invalid_email_format_percent,
             monthly_partition_text_not_matching_date_pattern_found=monthly_partition_text_not_matching_date_pattern_found,
             monthly_partition_text_matching_date_pattern_percent=monthly_partition_text_matching_date_pattern_percent,
             monthly_partition_text_matching_name_pattern_percent=monthly_partition_text_matching_name_pattern_percent,
             monthly_partition_invalid_uuid_format_found=monthly_partition_invalid_uuid_format_found,
             monthly_partition_valid_uuid_format_percent=monthly_partition_valid_uuid_format_percent,
             monthly_partition_invalid_ip4_address_format_found=monthly_partition_invalid_ip4_address_format_found,
             monthly_partition_invalid_ip6_address_format_found=monthly_partition_invalid_ip6_address_format_found,
```

### Comparing `dqops-1.1.0/dqops/client/models/column_patterns_monthly_partitioned_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_patterns_monthly_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_patterns_profiling_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_patterns_profiling_checks_spec.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
     from ..models.column_invalid_email_format_found_check_spec import (
         ColumnInvalidEmailFormatFoundCheckSpec,
     )
+    from ..models.column_invalid_email_format_percent_check_spec import (
+        ColumnInvalidEmailFormatPercentCheckSpec,
+    )
     from ..models.column_invalid_ip_4_address_format_found_check_spec import (
         ColumnInvalidIp4AddressFormatFoundCheckSpec,
     )
     from ..models.column_invalid_ip_6_address_format_found_check_spec import (
         ColumnInvalidIp6AddressFormatFoundCheckSpec,
     )
     from ..models.column_invalid_uuid_format_found_check_spec import (
@@ -50,14 +53,15 @@
     Attributes:
         custom_checks (Union[Unset, ColumnPatternsProfilingChecksSpecCustomChecks]): Dictionary of additional custom
             checks within this category. The keys are check names defined in the definition section. The sensor parameters
             and rules should match the type of the configured sensor and rule for the custom check.
         profile_text_not_matching_regex_found (Union[Unset, ColumnTextNotMatchingRegexFoundCheckSpec]):
         profile_texts_matching_regex_percent (Union[Unset, ColumnTextsMatchingRegexPercentCheckSpec]):
         profile_invalid_email_format_found (Union[Unset, ColumnInvalidEmailFormatFoundCheckSpec]):
+        profile_invalid_email_format_percent (Union[Unset, ColumnInvalidEmailFormatPercentCheckSpec]):
         profile_text_not_matching_date_pattern_found (Union[Unset, ColumnTextNotMatchingDatePatternFoundCheckSpec]):
         profile_text_matching_date_pattern_percent (Union[Unset, ColumnTextMatchingDatePatternPercentCheckSpec]):
         profile_text_matching_name_pattern_percent (Union[Unset, ColumnTextMatchingNamePatternPercentCheckSpec]):
         profile_invalid_uuid_format_found (Union[Unset, ColumnInvalidUuidFormatFoundCheckSpec]):
         profile_valid_uuid_format_percent (Union[Unset, ColumnValidUuidFormatPercentCheckSpec]):
         profile_invalid_ip4_address_format_found (Union[Unset, ColumnInvalidIp4AddressFormatFoundCheckSpec]):
         profile_invalid_ip6_address_format_found (Union[Unset, ColumnInvalidIp6AddressFormatFoundCheckSpec]):
@@ -69,14 +73,17 @@
     ] = UNSET
     profile_texts_matching_regex_percent: Union[
         Unset, "ColumnTextsMatchingRegexPercentCheckSpec"
     ] = UNSET
     profile_invalid_email_format_found: Union[
         Unset, "ColumnInvalidEmailFormatFoundCheckSpec"
     ] = UNSET
+    profile_invalid_email_format_percent: Union[
+        Unset, "ColumnInvalidEmailFormatPercentCheckSpec"
+    ] = UNSET
     profile_text_not_matching_date_pattern_found: Union[
         Unset, "ColumnTextNotMatchingDatePatternFoundCheckSpec"
     ] = UNSET
     profile_text_matching_date_pattern_percent: Union[
         Unset, "ColumnTextMatchingDatePatternPercentCheckSpec"
     ] = UNSET
     profile_text_matching_name_pattern_percent: Union[
@@ -115,14 +122,20 @@
 
         profile_invalid_email_format_found: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.profile_invalid_email_format_found, Unset):
             profile_invalid_email_format_found = (
                 self.profile_invalid_email_format_found.to_dict()
             )
 
+        profile_invalid_email_format_percent: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.profile_invalid_email_format_percent, Unset):
+            profile_invalid_email_format_percent = (
+                self.profile_invalid_email_format_percent.to_dict()
+            )
+
         profile_text_not_matching_date_pattern_found: Union[
             Unset, Dict[str, Any]
         ] = UNSET
         if not isinstance(self.profile_text_not_matching_date_pattern_found, Unset):
             profile_text_not_matching_date_pattern_found = (
                 self.profile_text_not_matching_date_pattern_found.to_dict()
             )
@@ -176,14 +189,18 @@
             field_dict[
                 "profile_texts_matching_regex_percent"
             ] = profile_texts_matching_regex_percent
         if profile_invalid_email_format_found is not UNSET:
             field_dict[
                 "profile_invalid_email_format_found"
             ] = profile_invalid_email_format_found
+        if profile_invalid_email_format_percent is not UNSET:
+            field_dict[
+                "profile_invalid_email_format_percent"
+            ] = profile_invalid_email_format_percent
         if profile_text_not_matching_date_pattern_found is not UNSET:
             field_dict[
                 "profile_text_not_matching_date_pattern_found"
             ] = profile_text_not_matching_date_pattern_found
         if profile_text_matching_date_pattern_percent is not UNSET:
             field_dict[
                 "profile_text_matching_date_pattern_percent"
@@ -212,14 +229,17 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.column_invalid_email_format_found_check_spec import (
             ColumnInvalidEmailFormatFoundCheckSpec,
         )
+        from ..models.column_invalid_email_format_percent_check_spec import (
+            ColumnInvalidEmailFormatPercentCheckSpec,
+        )
         from ..models.column_invalid_ip_4_address_format_found_check_spec import (
             ColumnInvalidIp4AddressFormatFoundCheckSpec,
         )
         from ..models.column_invalid_ip_6_address_format_found_check_spec import (
             ColumnInvalidIp6AddressFormatFoundCheckSpec,
         )
         from ..models.column_invalid_uuid_format_found_check_spec import (
@@ -298,14 +318,29 @@
         else:
             profile_invalid_email_format_found = (
                 ColumnInvalidEmailFormatFoundCheckSpec.from_dict(
                     _profile_invalid_email_format_found
                 )
             )
 
+        _profile_invalid_email_format_percent = d.pop(
+            "profile_invalid_email_format_percent", UNSET
+        )
+        profile_invalid_email_format_percent: Union[
+            Unset, ColumnInvalidEmailFormatPercentCheckSpec
+        ]
+        if isinstance(_profile_invalid_email_format_percent, Unset):
+            profile_invalid_email_format_percent = UNSET
+        else:
+            profile_invalid_email_format_percent = (
+                ColumnInvalidEmailFormatPercentCheckSpec.from_dict(
+                    _profile_invalid_email_format_percent
+                )
+            )
+
         _profile_text_not_matching_date_pattern_found = d.pop(
             "profile_text_not_matching_date_pattern_found", UNSET
         )
         profile_text_not_matching_date_pattern_found: Union[
             Unset, ColumnTextNotMatchingDatePatternFoundCheckSpec
         ]
         if isinstance(_profile_text_not_matching_date_pattern_found, Unset):
@@ -408,14 +443,15 @@
             )
 
         column_patterns_profiling_checks_spec = cls(
             custom_checks=custom_checks,
             profile_text_not_matching_regex_found=profile_text_not_matching_regex_found,
             profile_texts_matching_regex_percent=profile_texts_matching_regex_percent,
             profile_invalid_email_format_found=profile_invalid_email_format_found,
+            profile_invalid_email_format_percent=profile_invalid_email_format_percent,
             profile_text_not_matching_date_pattern_found=profile_text_not_matching_date_pattern_found,
             profile_text_matching_date_pattern_percent=profile_text_matching_date_pattern_percent,
             profile_text_matching_name_pattern_percent=profile_text_matching_name_pattern_percent,
             profile_invalid_uuid_format_found=profile_invalid_uuid_format_found,
             profile_valid_uuid_format_percent=profile_valid_uuid_format_percent,
             profile_invalid_ip4_address_format_found=profile_invalid_ip4_address_format_found,
             profile_invalid_ip6_address_format_found=profile_invalid_ip6_address_format_found,
```

### Comparing `dqops-1.1.0/dqops/client/models/column_patterns_profiling_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_patterns_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_patterns_text_matching_date_pattern_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_patterns_text_matching_date_pattern_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_patterns_text_matching_name_pattern_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_patterns_text_matching_name_pattern_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_patterns_text_not_matching_date_pattern_count_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_patterns_text_not_matching_date_pattern_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_patterns_text_not_matching_regex_count_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_patterns_text_not_matching_regex_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_patterns_texts_matching_regex_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_patterns_texts_matching_regex_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_patterns_valid_uuid_format_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_patterns_valid_uuid_format_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_percentile_10_in_range_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_percentile_10_in_range_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_percentile_25_in_range_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_percentile_25_in_range_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_percentile_75_in_range_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_percentile_75_in_range_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_percentile_90_in_range_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_percentile_90_in_range_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_percentile_in_range_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_percentile_in_range_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_pii_contains_email_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_pii_contains_email_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_pii_contains_email_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_pii_contains_email_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_pii_contains_ip_4_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_pii_contains_ip_4_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_pii_contains_ip_4_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_pii_contains_ip_4_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_pii_contains_ip_6_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_pii_contains_ip_6_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_pii_contains_ip_6_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_pii_contains_ip_6_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_pii_contains_usa_phone_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_pii_contains_usa_phone_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_pii_contains_usa_phone_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_pii_contains_usa_phone_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_pii_contains_usa_zipcode_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_pii_contains_usa_zipcode_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_pii_contains_usa_zipcode_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_pii_contains_usa_zipcode_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_pii_daily_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_pii_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_pii_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_pii_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_pii_daily_partitioned_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_pii_daily_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_pii_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_pii_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_pii_monthly_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_pii_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_pii_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_pii_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_pii_monthly_partitioned_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_pii_monthly_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_pii_monthly_partitioned_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_pii_monthly_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_pii_profiling_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_pii_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_pii_profiling_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_pii_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_population_stddev_in_range_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_population_stddev_in_range_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_population_variance_in_range_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_population_variance_in_range_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_profiling_check_categories_spec.py` & `dqops-1.2.0/dqops/client/models/column_profiling_check_categories_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_profiling_check_categories_spec_comparisons.py` & `dqops-1.2.0/dqops/client/models/column_profiling_check_categories_spec_comparisons.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_profiling_check_categories_spec_custom.py` & `dqops-1.2.0/dqops/client/models/column_profiling_check_categories_spec_custom.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_range_max_value_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_range_max_value_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_range_max_value_statistics_collector_spec.py` & `dqops-1.2.0/dqops/client/models/column_range_max_value_statistics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_range_median_value_statistics_collector_spec.py` & `dqops-1.2.0/dqops/client/models/column_range_median_value_statistics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_range_min_value_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_range_min_value_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_range_min_value_statistics_collector_spec.py` & `dqops-1.2.0/dqops/client/models/column_range_min_value_statistics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_range_statistics_collectors_spec.py` & `dqops-1.2.0/dqops/client/models/column_range_statistics_collectors_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_range_sum_value_statistics_collector_spec.py` & `dqops-1.2.0/dqops/client/models/column_range_sum_value_statistics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_sample_stddev_in_range_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_sample_stddev_in_range_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_sample_variance_in_range_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_sample_variance_in_range_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_sampling_column_samples_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_sampling_column_samples_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_sampling_column_samples_statistics_collector_spec.py` & `dqops-1.2.0/dqops/client/models/column_sampling_column_samples_statistics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_sampling_statistics_collectors_spec.py` & `dqops-1.2.0/dqops/client/models/column_sampling_statistics_collectors_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_schema_column_exists_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_schema_column_exists_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_schema_daily_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_schema_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_schema_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_schema_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_schema_monthly_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_schema_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_schema_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_schema_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_schema_profiling_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_schema_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_schema_profiling_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_schema_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_schema_type_changed_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_schema_type_changed_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_spec.py` & `dqops-1.2.0/dqops/client/models/column_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_sql_aggregate_expression_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_sql_aggregate_expression_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_sql_aggregated_expression_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_sql_aggregated_expression_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_sql_condition_failed_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_sql_condition_failed_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_sql_condition_failed_count_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_sql_condition_failed_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_sql_condition_passed_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_sql_condition_passed_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_sql_condition_passed_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_sql_condition_passed_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_sql_import_custom_result_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_sql_import_custom_result_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_sql_import_custom_result_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_sql_import_custom_result_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_statistics_collectors_root_categories_spec.py` & `dqops-1.2.0/dqops/client/models/column_statistics_collectors_root_categories_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_statistics_model.py` & `dqops-1.2.0/dqops/client/models/column_statistics_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_strings_expected_text_values_in_use_count_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_strings_expected_text_values_in_use_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_strings_expected_texts_in_top_values_count_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_strings_expected_texts_in_top_values_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_sum_anomaly_differencing_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_sum_anomaly_differencing_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_sum_anomaly_stationary_partition_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_sum_anomaly_stationary_partition_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_sum_change_1_day_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_sum_change_1_day_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_sum_change_30_days_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_sum_change_30_days_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_sum_change_7_days_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_sum_change_7_days_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_sum_change_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_sum_change_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_sum_in_range_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_sum_in_range_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_daily_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_text_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_daily_partitioned_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_daily_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_text_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_found_in_set_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_found_in_set_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_length_above_max_length_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_length_above_max_length_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_length_above_max_length_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_length_above_max_length_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_length_below_min_length_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_length_below_min_length_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_length_below_min_length_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_length_below_min_length_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_length_in_range_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_length_in_range_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_match_date_format_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_match_date_format_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_match_date_format_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_match_date_format_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_matching_date_pattern_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_matching_date_pattern_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_matching_name_pattern_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_matching_name_pattern_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_max_length_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_max_length_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_mean_length_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_mean_length_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_min_length_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_min_length_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_monthly_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_text_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_monthly_partitioned_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_monthly_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_monthly_partitioned_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_text_monthly_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_not_matching_date_pattern_found_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_not_matching_date_pattern_found_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_not_matching_regex_found_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_not_matching_regex_found_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_parsable_to_boolean_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_parsable_to_boolean_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_parsable_to_date_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_parsable_to_date_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_parsable_to_float_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_parsable_to_float_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_parsable_to_integer_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_parsable_to_integer_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_profiling_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_profiling_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_text_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_statistics_collectors_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_statistics_collectors_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_text_datatype_detect_statistics_collector_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_text_datatype_detect_statistics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_text_length_above_max_length_count_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_text_length_above_max_length_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_text_length_above_max_length_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_text_length_above_max_length_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_text_length_below_min_length_count_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_text_length_below_min_length_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_text_length_below_min_length_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_text_length_below_min_length_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_text_length_in_range_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_text_length_in_range_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_text_max_length_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_text_max_length_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_text_max_length_statistics_collector_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_text_max_length_statistics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_text_mean_length_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_text_mean_length_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_text_mean_length_statistics_collector_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_text_mean_length_statistics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_text_min_length_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_text_min_length_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_text_min_length_statistics_collector_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_text_min_length_statistics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_text_parsable_to_boolean_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_text_parsable_to_boolean_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_text_parsable_to_date_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_text_parsable_to_date_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_text_parsable_to_float_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_text_parsable_to_float_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_text_parsable_to_integer_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_text_parsable_to_integer_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_text_valid_country_code_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_text_valid_country_code_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_text_valid_currency_code_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_text_valid_currency_code_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_valid_country_code_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_valid_country_code_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_text_valid_currency_code_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_text_valid_currency_code_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_texts_matching_regex_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_texts_matching_regex_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_true_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_true_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_type_snapshot_spec.py` & `dqops-1.2.0/dqops/client/models/column_type_snapshot_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_uniqueness_daily_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_uniqueness_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_uniqueness_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_uniqueness_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_uniqueness_daily_partitioned_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_uniqueness_daily_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_uniqueness_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_uniqueness_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_uniqueness_distinct_count_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_uniqueness_distinct_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_uniqueness_distinct_count_statistics_collector_spec.py` & `dqops-1.2.0/dqops/client/models/column_uniqueness_distinct_count_statistics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_uniqueness_distinct_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_uniqueness_distinct_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_uniqueness_distinct_percent_statistics_collector_spec.py` & `dqops-1.2.0/dqops/client/models/column_uniqueness_distinct_percent_statistics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_uniqueness_duplicate_count_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_uniqueness_duplicate_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_uniqueness_duplicate_count_statistics_collector_spec.py` & `dqops-1.2.0/dqops/client/models/column_uniqueness_duplicate_count_statistics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_uniqueness_duplicate_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_uniqueness_duplicate_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_uniqueness_duplicate_percent_statistics_collector_spec.py` & `dqops-1.2.0/dqops/client/models/column_uniqueness_duplicate_percent_statistics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_uniqueness_monthly_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_uniqueness_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_uniqueness_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_uniqueness_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_uniqueness_monthly_partitioned_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_uniqueness_monthly_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_uniqueness_monthly_partitioned_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_uniqueness_monthly_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_uniqueness_profiling_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_uniqueness_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_uniqueness_profiling_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_uniqueness_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_uniqueness_statistics_collectors_spec.py` & `dqops-1.2.0/dqops/client/models/column_uniqueness_statistics_collectors_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_valid_latitude_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_valid_latitude_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_valid_longitude_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_valid_longitude_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_valid_uuid_format_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_valid_uuid_format_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_whitespace_blank_null_placeholder_text_count_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_whitespace_blank_null_placeholder_text_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_whitespace_blank_null_placeholder_text_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_whitespace_blank_null_placeholder_text_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_whitespace_daily_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_whitespace_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_whitespace_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_whitespace_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_whitespace_daily_partitioned_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_whitespace_daily_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_whitespace_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_whitespace_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_whitespace_empty_text_count_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_whitespace_empty_text_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_whitespace_empty_text_found_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_whitespace_empty_text_found_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_whitespace_empty_text_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_whitespace_empty_text_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_whitespace_empty_text_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_whitespace_empty_text_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_whitespace_monthly_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_whitespace_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_whitespace_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_whitespace_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_whitespace_monthly_partitioned_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_whitespace_monthly_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_whitespace_monthly_partitioned_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_whitespace_monthly_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_whitespace_null_placeholder_text_found_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_whitespace_null_placeholder_text_found_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_whitespace_null_placeholder_text_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_whitespace_null_placeholder_text_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_whitespace_profiling_checks_spec.py` & `dqops-1.2.0/dqops/client/models/column_whitespace_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_whitespace_profiling_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/column_whitespace_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_whitespace_text_surrounded_by_whitespace_count_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_whitespace_text_surrounded_by_whitespace_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_whitespace_text_surrounded_by_whitespace_found_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_whitespace_text_surrounded_by_whitespace_found_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_whitespace_text_surrounded_by_whitespace_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_whitespace_text_surrounded_by_whitespace_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_whitespace_text_surrounded_by_whitespace_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_whitespace_text_surrounded_by_whitespace_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_whitespace_whitespace_text_count_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_whitespace_whitespace_text_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_whitespace_whitespace_text_found_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_whitespace_whitespace_text_found_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_whitespace_whitespace_text_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/column_whitespace_whitespace_text_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/column_whitespace_whitespace_text_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/column_whitespace_whitespace_text_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/comment_spec.py` & `dqops-1.2.0/dqops/client/models/comment_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/common_column_model.py` & `dqops-1.2.0/dqops/client/models/common_column_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/compare_thresholds_model.py` & `dqops-1.2.0/dqops/client/models/compare_thresholds_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/comparison_check_result_model.py` & `dqops-1.2.0/dqops/client/models/comparison_check_result_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/connection_incident_grouping_spec.py` & `dqops-1.2.0/dqops/client/models/connection_incident_grouping_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/connection_model.py` & `dqops-1.2.0/dqops/client/models/connection_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/connection_spec.py` & `dqops-1.2.0/dqops/client/models/connection_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/connection_specification_model.py` & `dqops-1.2.0/dqops/client/models/connection_specification_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/connection_test_model.py` & `dqops-1.2.0/dqops/client/models/connection_test_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/count_between_rule_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/count_between_rule_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/csv_file_format_spec.py` & `dqops-1.2.0/dqops/client/models/csv_file_format_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/custom_check_spec.py` & `dqops-1.2.0/dqops/client/models/custom_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/custom_rule_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/custom_rule_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/custom_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/custom_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/dashboard_spec.py` & `dqops-1.2.0/dqops/client/models/dashboard_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/dashboard_spec_parameters.py` & `dqops-1.2.0/dqops/client/models/dashboard_spec_parameters.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/dashboards_folder_spec.py` & `dqops-1.2.0/dqops/client/models/dashboards_folder_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/data_delete_result_partition.py` & `dqops-1.2.0/dqops/client/models/data_delete_result_partition.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/data_dictionary_list_model.py` & `dqops-1.2.0/dqops/client/models/data_dictionary_list_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/data_dictionary_model.py` & `dqops-1.2.0/dqops/client/models/data_dictionary_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/data_grouping_configuration_list_model.py` & `dqops-1.2.0/dqops/client/models/data_grouping_configuration_list_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/data_grouping_configuration_model.py` & `dqops-1.2.0/dqops/client/models/data_grouping_configuration_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/data_grouping_configuration_spec.py` & `dqops-1.2.0/dqops/client/models/data_grouping_configuration_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/data_grouping_configuration_trimmed_model.py` & `dqops-1.2.0/dqops/client/models/data_grouping_configuration_trimmed_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/data_grouping_dimension_spec.py` & `dqops-1.2.0/dqops/client/models/data_grouping_dimension_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/data_type_category.py` & `dqops-1.2.0/dqops/client/models/data_type_category.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/databricks_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/databricks_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/databricks_parameters_spec_properties.py` & `dqops-1.2.0/dqops/client/models/databricks_parameters_spec_properties.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/default_column_checks_pattern_list_model.py` & `dqops-1.2.0/dqops/client/models/default_column_checks_pattern_list_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/default_column_checks_pattern_model.py` & `dqops-1.2.0/dqops/client/models/default_column_checks_pattern_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/default_schedules_spec.py` & `dqops-1.2.0/dqops/client/models/default_schedules_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/default_table_checks_pattern_list_model.py` & `dqops-1.2.0/dqops/client/models/default_table_checks_pattern_list_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/default_table_checks_pattern_model.py` & `dqops-1.2.0/dqops/client/models/default_table_checks_pattern_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/delete_stored_data_queue_job_parameters.py` & `dqops-1.2.0/dqops/client/models/delete_stored_data_queue_job_parameters.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/delete_stored_data_queue_job_result.py` & `dqops-1.2.0/dqops/client/models/delete_stored_data_queue_job_result.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/delete_stored_data_result.py` & `dqops-1.2.0/dqops/client/models/delete_stored_data_result.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/delete_stored_data_result_partition_results.py` & `dqops-1.2.0/dqops/client/models/delete_stored_data_result_partition_results.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/detected_datatype_equals_rule_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/detected_datatype_equals_rule_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/dqo_cloud_user_model.py` & `dqops-1.2.0/dqops/client/models/dqo_cloud_user_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/dqo_job_change_model.py` & `dqops-1.2.0/dqops/client/models/dqo_job_change_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/dqo_job_entry_parameters_model.py` & `dqops-1.2.0/dqops/client/models/dqo_job_entry_parameters_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/dqo_job_history_entry_model.py` & `dqops-1.2.0/dqops/client/models/dqo_job_history_entry_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/dqo_job_queue_incremental_snapshot_model.py` & `dqops-1.2.0/dqops/client/models/dqo_job_queue_incremental_snapshot_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/dqo_job_queue_initial_snapshot_model.py` & `dqops-1.2.0/dqops/client/models/dqo_job_queue_initial_snapshot_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/dqo_job_type.py` & `dqops-1.2.0/dqops/client/models/dqo_job_type.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/dqo_queue_job_id.py` & `dqops-1.2.0/dqops/client/models/dqo_queue_job_id.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/dqo_root.py` & `dqops-1.2.0/dqops/client/models/dqo_root.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/dqo_settings_model.py` & `dqops-1.2.0/dqops/client/models/dqo_settings_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/dqo_settings_model_properties.py` & `dqops-1.2.0/dqops/client/models/dqo_settings_model_properties.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/dqo_settings_model_properties_additional_property.py` & `dqops-1.2.0/dqops/client/models/dqo_settings_model_properties_additional_property.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/dqo_user_profile_model.py` & `dqops-1.2.0/dqops/client/models/dqo_user_profile_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/duckdb_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/duckdb_parameters_spec.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
+from ..models.aws_authentication_mode import AwsAuthenticationMode
 from ..models.duckdb_files_format_type import DuckdbFilesFormatType
 from ..models.duckdb_read_mode import DuckdbReadMode
 from ..models.duckdb_storage_type import DuckdbStorageType
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
     from ..models.csv_file_format_spec import CsvFileFormatSpec
@@ -35,14 +36,15 @@
             to the JDBC connection string, a key/value dictionary.
         csv (Union[Unset, CsvFileFormatSpec]):
         json (Union[Unset, JsonFileFormatSpec]):
         parquet (Union[Unset, ParquetFileFormatSpec]):
         directories (Union[Unset, DuckdbParametersSpecDirectories]): Virtual schema name to directory mappings. The path
             must be an absolute path.
         storage_type (Union[Unset, DuckdbStorageType]):
+        aws_authentication_mode (Union[Unset, AwsAuthenticationMode]):
         user (Union[Unset, str]): DuckDB user name for a remote storage type. The value can be in the
             ${ENVIRONMENT_VARIABLE_NAME} format to use dynamic substitution.
         password (Union[Unset, str]): DuckDB password for a remote storage type. The value can be in the
             ${ENVIRONMENT_VARIABLE_NAME} format to use dynamic substitution.
         region (Union[Unset, str]): The region for the storage credentials. The value can be in the
             ${ENVIRONMENT_VARIABLE_NAME} format to use dynamic substitution.
     """
@@ -52,14 +54,15 @@
     database: Union[Unset, str] = UNSET
     properties: Union[Unset, "DuckdbParametersSpecProperties"] = UNSET
     csv: Union[Unset, "CsvFileFormatSpec"] = UNSET
     json: Union[Unset, "JsonFileFormatSpec"] = UNSET
     parquet: Union[Unset, "ParquetFileFormatSpec"] = UNSET
     directories: Union[Unset, "DuckdbParametersSpecDirectories"] = UNSET
     storage_type: Union[Unset, DuckdbStorageType] = UNSET
+    aws_authentication_mode: Union[Unset, AwsAuthenticationMode] = UNSET
     user: Union[Unset, str] = UNSET
     password: Union[Unset, str] = UNSET
     region: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         read_mode: Union[Unset, str] = UNSET
@@ -91,14 +94,18 @@
         if not isinstance(self.directories, Unset):
             directories = self.directories.to_dict()
 
         storage_type: Union[Unset, str] = UNSET
         if not isinstance(self.storage_type, Unset):
             storage_type = self.storage_type.value
 
+        aws_authentication_mode: Union[Unset, str] = UNSET
+        if not isinstance(self.aws_authentication_mode, Unset):
+            aws_authentication_mode = self.aws_authentication_mode.value
+
         user = self.user
         password = self.password
         region = self.region
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
@@ -116,14 +123,16 @@
             field_dict["json"] = json
         if parquet is not UNSET:
             field_dict["parquet"] = parquet
         if directories is not UNSET:
             field_dict["directories"] = directories
         if storage_type is not UNSET:
             field_dict["storage_type"] = storage_type
+        if aws_authentication_mode is not UNSET:
+            field_dict["aws_authentication_mode"] = aws_authentication_mode
         if user is not UNSET:
             field_dict["user"] = user
         if password is not UNSET:
             field_dict["password"] = password
         if region is not UNSET:
             field_dict["region"] = region
 
@@ -196,14 +205,21 @@
         _storage_type = d.pop("storage_type", UNSET)
         storage_type: Union[Unset, DuckdbStorageType]
         if isinstance(_storage_type, Unset):
             storage_type = UNSET
         else:
             storage_type = DuckdbStorageType(_storage_type)
 
+        _aws_authentication_mode = d.pop("aws_authentication_mode", UNSET)
+        aws_authentication_mode: Union[Unset, AwsAuthenticationMode]
+        if isinstance(_aws_authentication_mode, Unset):
+            aws_authentication_mode = UNSET
+        else:
+            aws_authentication_mode = AwsAuthenticationMode(_aws_authentication_mode)
+
         user = d.pop("user", UNSET)
 
         password = d.pop("password", UNSET)
 
         region = d.pop("region", UNSET)
 
         duckdb_parameters_spec = cls(
@@ -212,14 +228,15 @@
             database=database,
             properties=properties,
             csv=csv,
             json=json,
             parquet=parquet,
             directories=directories,
             storage_type=storage_type,
+            aws_authentication_mode=aws_authentication_mode,
             user=user,
             password=password,
             region=region,
         )
 
         duckdb_parameters_spec.additional_properties = d
         return duckdb_parameters_spec
```

### Comparing `dqops-1.1.0/dqops/client/models/duckdb_parameters_spec_directories.py` & `dqops-1.2.0/dqops/client/models/duckdb_parameters_spec_directories.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/duckdb_parameters_spec_properties.py` & `dqops-1.2.0/dqops/client/models/duckdb_parameters_spec_properties.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/duration.py` & `dqops-1.2.0/dqops/client/models/duration.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/effective_schedule_model.py` & `dqops-1.2.0/dqops/client/models/effective_schedule_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/equals_1_rule_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/equals_1_rule_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/equals_integer_rule_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/equals_integer_rule_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/error_entry_model.py` & `dqops-1.2.0/dqops/client/models/error_entry_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/errors_list_model.py` & `dqops-1.2.0/dqops/client/models/sensor_readouts_list_model.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,91 +3,97 @@
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..models.check_type import CheckType
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.error_entry_model import ErrorEntryModel
+    from ..models.sensor_readout_entry_model import SensorReadoutEntryModel
 
 
-T = TypeVar("T", bound="ErrorsListModel")
+T = TypeVar("T", bound="SensorReadoutsListModel")
 
 
 @_attrs_define
-class ErrorsListModel:
+class SensorReadoutsListModel:
     """
     Attributes:
         check_name (Union[Unset, str]): Check name
         check_display_name (Union[Unset, str]): Check display name
         check_type (Union[Unset, CheckType]):
         check_hash (Union[Unset, int]): Check hash
         check_category (Union[Unset, str]): Check category name
-        data_groups_names (Union[Unset, List[str]]): Data groups list
+        sensor_name (Union[Unset, str]): Sensor name
+        data_group_names (Union[Unset, List[str]]): List of data groups that have values for this sensor readout (list
+            of time series)
         data_group (Union[Unset, str]): Selected data group
-        error_entries (Union[Unset, List['ErrorEntryModel']]): Error entries
+        sensor_readout_entries (Union[Unset, List['SensorReadoutEntryModel']]): Sensor readout entries
     """
 
     check_name: Union[Unset, str] = UNSET
     check_display_name: Union[Unset, str] = UNSET
     check_type: Union[Unset, CheckType] = UNSET
     check_hash: Union[Unset, int] = UNSET
     check_category: Union[Unset, str] = UNSET
-    data_groups_names: Union[Unset, List[str]] = UNSET
+    sensor_name: Union[Unset, str] = UNSET
+    data_group_names: Union[Unset, List[str]] = UNSET
     data_group: Union[Unset, str] = UNSET
-    error_entries: Union[Unset, List["ErrorEntryModel"]] = UNSET
+    sensor_readout_entries: Union[Unset, List["SensorReadoutEntryModel"]] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         check_name = self.check_name
         check_display_name = self.check_display_name
         check_type: Union[Unset, str] = UNSET
         if not isinstance(self.check_type, Unset):
             check_type = self.check_type.value
 
         check_hash = self.check_hash
         check_category = self.check_category
-        data_groups_names: Union[Unset, List[str]] = UNSET
-        if not isinstance(self.data_groups_names, Unset):
-            data_groups_names = self.data_groups_names
+        sensor_name = self.sensor_name
+        data_group_names: Union[Unset, List[str]] = UNSET
+        if not isinstance(self.data_group_names, Unset):
+            data_group_names = self.data_group_names
 
         data_group = self.data_group
-        error_entries: Union[Unset, List[Dict[str, Any]]] = UNSET
-        if not isinstance(self.error_entries, Unset):
-            error_entries = []
-            for error_entries_item_data in self.error_entries:
-                error_entries_item = error_entries_item_data.to_dict()
+        sensor_readout_entries: Union[Unset, List[Dict[str, Any]]] = UNSET
+        if not isinstance(self.sensor_readout_entries, Unset):
+            sensor_readout_entries = []
+            for sensor_readout_entries_item_data in self.sensor_readout_entries:
+                sensor_readout_entries_item = sensor_readout_entries_item_data.to_dict()
 
-                error_entries.append(error_entries_item)
+                sensor_readout_entries.append(sensor_readout_entries_item)
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if check_name is not UNSET:
             field_dict["checkName"] = check_name
         if check_display_name is not UNSET:
             field_dict["checkDisplayName"] = check_display_name
         if check_type is not UNSET:
             field_dict["checkType"] = check_type
         if check_hash is not UNSET:
             field_dict["checkHash"] = check_hash
         if check_category is not UNSET:
             field_dict["checkCategory"] = check_category
-        if data_groups_names is not UNSET:
-            field_dict["dataGroupsNames"] = data_groups_names
+        if sensor_name is not UNSET:
+            field_dict["sensorName"] = sensor_name
+        if data_group_names is not UNSET:
+            field_dict["dataGroupNames"] = data_group_names
         if data_group is not UNSET:
             field_dict["dataGroup"] = data_group
-        if error_entries is not UNSET:
-            field_dict["errorEntries"] = error_entries
+        if sensor_readout_entries is not UNSET:
+            field_dict["sensorReadoutEntries"] = sensor_readout_entries
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.error_entry_model import ErrorEntryModel
+        from ..models.sensor_readout_entry_model import SensorReadoutEntryModel
 
         d = src_dict.copy()
         check_name = d.pop("checkName", UNSET)
 
         check_display_name = d.pop("checkDisplayName", UNSET)
 
         _check_type = d.pop("checkType", UNSET)
@@ -97,38 +103,43 @@
         else:
             check_type = CheckType(_check_type)
 
         check_hash = d.pop("checkHash", UNSET)
 
         check_category = d.pop("checkCategory", UNSET)
 
-        data_groups_names = cast(List[str], d.pop("dataGroupsNames", UNSET))
+        sensor_name = d.pop("sensorName", UNSET)
+
+        data_group_names = cast(List[str], d.pop("dataGroupNames", UNSET))
 
         data_group = d.pop("dataGroup", UNSET)
 
-        error_entries = []
-        _error_entries = d.pop("errorEntries", UNSET)
-        for error_entries_item_data in _error_entries or []:
-            error_entries_item = ErrorEntryModel.from_dict(error_entries_item_data)
+        sensor_readout_entries = []
+        _sensor_readout_entries = d.pop("sensorReadoutEntries", UNSET)
+        for sensor_readout_entries_item_data in _sensor_readout_entries or []:
+            sensor_readout_entries_item = SensorReadoutEntryModel.from_dict(
+                sensor_readout_entries_item_data
+            )
 
-            error_entries.append(error_entries_item)
+            sensor_readout_entries.append(sensor_readout_entries_item)
 
-        errors_list_model = cls(
+        sensor_readouts_list_model = cls(
             check_name=check_name,
             check_display_name=check_display_name,
             check_type=check_type,
             check_hash=check_hash,
             check_category=check_category,
-            data_groups_names=data_groups_names,
+            sensor_name=sensor_name,
+            data_group_names=data_group_names,
             data_group=data_group,
-            error_entries=error_entries,
+            sensor_readout_entries=sensor_readout_entries,
         )
 
-        errors_list_model.additional_properties = d
-        return errors_list_model
+        sensor_readouts_list_model.additional_properties = d
+        return sensor_readouts_list_model
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dqops-1.1.0/dqops/client/models/external_log_entry.py` & `dqops-1.2.0/dqops/client/models/external_log_entry.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/field_model.py` & `dqops-1.2.0/dqops/client/models/field_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/file_format_spec.py` & `dqops-1.2.0/dqops/client/models/file_format_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/hierarchy_id_model.py` & `dqops-1.2.0/dqops/client/models/hierarchy_id_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/hierarchy_id_model_path_item.py` & `dqops-1.2.0/dqops/client/models/hierarchy_id_model_path_item.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/import_schema_queue_job_parameters.py` & `dqops-1.2.0/dqops/client/models/import_schema_queue_job_parameters.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/import_severity_rule_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/import_severity_rule_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/import_tables_queue_job_parameters.py` & `dqops-1.2.0/dqops/client/models/import_tables_queue_job_parameters.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/import_tables_queue_job_result.py` & `dqops-1.2.0/dqops/client/models/import_tables_queue_job_result.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/import_tables_result.py` & `dqops-1.2.0/dqops/client/models/import_tables_result.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/incident_daily_issues_count.py` & `dqops-1.2.0/dqops/client/models/incident_daily_issues_count.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/incident_issue_histogram_model.py` & `dqops-1.2.0/dqops/client/models/incident_issue_histogram_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/incident_issue_histogram_model_checks.py` & `dqops-1.2.0/dqops/client/models/incident_issue_histogram_model_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/incident_issue_histogram_model_columns.py` & `dqops-1.2.0/dqops/client/models/incident_issue_histogram_model_columns.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/incident_issue_histogram_model_days.py` & `dqops-1.2.0/dqops/client/models/incident_issue_histogram_model_days.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/incident_model.py` & `dqops-1.2.0/dqops/client/models/incident_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/incident_webhook_notifications_spec.py` & `dqops-1.2.0/dqops/client/models/incident_webhook_notifications_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/incidents_per_connection_model.py` & `dqops-1.2.0/dqops/client/models/incidents_per_connection_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/json_file_format_spec.py` & `dqops-1.2.0/dqops/client/models/json_file_format_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/max_count_rule_0_error_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/max_count_rule_0_error_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/max_count_rule_0_warning_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/max_count_rule_0_warning_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/max_count_rule_100_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/max_count_rule_100_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/max_days_rule_1_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/max_days_rule_1_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/max_days_rule_2_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/max_days_rule_2_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/max_days_rule_7_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/max_days_rule_7_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/max_diff_percent_rule_0_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/max_diff_percent_rule_0_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/max_diff_percent_rule_1_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/max_diff_percent_rule_1_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/max_diff_percent_rule_5_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/max_diff_percent_rule_5_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/max_failures_rule_0_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/max_failures_rule_0_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/max_failures_rule_1_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/max_failures_rule_1_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/max_failures_rule_5_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/max_failures_rule_5_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/max_missing_rule_0_error_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/max_missing_rule_0_error_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/max_missing_rule_0_warning_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/max_missing_rule_0_warning_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/max_missing_rule_2_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/max_missing_rule_2_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/max_percent_rule_0_error_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/max_percent_rule_0_error_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/max_percent_rule_0_warning_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/max_percent_rule_0_warning_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/max_percent_rule_5_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/max_percent_rule_5_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/min_count_rule_1_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/min_count_rule_1_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/min_percent_rule_100_error_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/min_percent_rule_100_error_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/min_percent_rule_100_warning_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/min_percent_rule_100_warning_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/min_percent_rule_95_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/min_percent_rule_95_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/monitoring_schedule_spec.py` & `dqops-1.2.0/dqops/client/models/monitoring_schedule_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/mono.py` & `dqops-1.2.0/dqops/client/models/mono.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/mono_dqo_queue_job_id.py` & `dqops-1.2.0/dqops/client/models/mono_dqo_queue_job_id.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/mono_object.py` & `dqops-1.2.0/dqops/client/models/mono_object.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/mono_void.py` & `dqops-1.2.0/dqops/client/models/mono_void.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/mysql_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/mysql_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/mysql_parameters_spec_properties.py` & `dqops-1.2.0/dqops/client/models/mysql_parameters_spec_properties.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/optional.py` & `dqops-1.2.0/dqops/client/models/optional.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/optional_incident_webhook_notifications_spec.py` & `dqops-1.2.0/dqops/client/models/optional_incident_webhook_notifications_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/optional_monitoring_schedule_spec.py` & `dqops-1.2.0/dqops/client/models/optional_monitoring_schedule_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/oracle_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/oracle_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/oracle_parameters_spec_properties.py` & `dqops-1.2.0/dqops/client/models/oracle_parameters_spec_properties.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/parameter_definition_spec.py` & `dqops-1.2.0/dqops/client/models/parameter_definition_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/parquet_file_format_spec.py` & `dqops-1.2.0/dqops/client/models/parquet_file_format_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/partition_incremental_time_window_spec.py` & `dqops-1.2.0/dqops/client/models/partition_incremental_time_window_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/physical_table_name.py` & `dqops-1.2.0/dqops/client/models/physical_table_name.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/postgresql_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/postgresql_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/postgresql_parameters_spec_properties.py` & `dqops-1.2.0/dqops/client/models/postgresql_parameters_spec_properties.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/presto_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/presto_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/presto_parameters_spec_properties.py` & `dqops-1.2.0/dqops/client/models/presto_parameters_spec_properties.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/profiling_time_period_truncation.py` & `dqops-1.2.0/dqops/client/models/profiling_time_period_truncation.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/provider_sensor_definition_spec.py` & `dqops-1.2.0/dqops/client/models/provider_sensor_definition_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/provider_sensor_definition_spec_parameters.py` & `dqops-1.2.0/dqops/client/models/provider_sensor_definition_spec_parameters.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/provider_sensor_list_model.py` & `dqops-1.2.0/dqops/client/models/provider_sensor_list_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/provider_sensor_model.py` & `dqops-1.2.0/dqops/client/models/provider_sensor_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/quality_category_model.py` & `dqops-1.2.0/dqops/client/models/quality_category_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/redshift_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/spark_parameters_spec.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,111 +2,109 @@
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.redshift_parameters_spec_properties import (
-        RedshiftParametersSpecProperties,
-    )
+    from ..models.spark_parameters_spec_properties import SparkParametersSpecProperties
 
 
-T = TypeVar("T", bound="RedshiftParametersSpec")
+T = TypeVar("T", bound="SparkParametersSpec")
 
 
 @_attrs_define
-class RedshiftParametersSpec:
+class SparkParametersSpec:
     """
     Attributes:
-        host (Union[Unset, str]): Redshift host name. Supports also a ${REDSHIFT_HOST} configuration with a custom
-            environment variable.
-        port (Union[Unset, str]): Redshift port number. The default port is 5432. Supports also a ${REDSHIFT_PORT}
+        host (Union[Unset, str]): Spark host name. Supports also a ${SPARK_HOST} configuration with a custom environment
+            variable.
+        port (Union[Unset, str]): Spark port number. The default port is 10000. Supports also a ${SPARK_PORT}
             configuration with a custom environment variable.
-        database (Union[Unset, str]): Redshift database name. The value can be in the ${ENVIRONMENT_VARIABLE_NAME}
-            format to use dynamic substitution.
-        user (Union[Unset, str]): Redshift user name. The value can be in the ${ENVIRONMENT_VARIABLE_NAME} format to use
+        user (Union[Unset, str]): Spark user name. The value can be in the ${ENVIRONMENT_VARIABLE_NAME} format to use
             dynamic substitution.
-        password (Union[Unset, str]): Redshift database password. The value can be in the ${ENVIRONMENT_VARIABLE_NAME}
+        password (Union[Unset, str]): Spark database password. The value can be in the ${ENVIRONMENT_VARIABLE_NAME}
             format to use dynamic substitution.
-        properties (Union[Unset, RedshiftParametersSpecProperties]): A dictionary of custom JDBC parameters that are
-            added to the JDBC connection string, a key/value dictionary.
+        properties (Union[Unset, SparkParametersSpecProperties]): A dictionary of custom JDBC parameters that are added
+            to the JDBC connection string, a key/value dictionary.
+        database (Union[Unset, str]):
     """
 
     host: Union[Unset, str] = UNSET
     port: Union[Unset, str] = UNSET
-    database: Union[Unset, str] = UNSET
     user: Union[Unset, str] = UNSET
     password: Union[Unset, str] = UNSET
-    properties: Union[Unset, "RedshiftParametersSpecProperties"] = UNSET
+    properties: Union[Unset, "SparkParametersSpecProperties"] = UNSET
+    database: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         host = self.host
         port = self.port
-        database = self.database
         user = self.user
         password = self.password
         properties: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.properties, Unset):
             properties = self.properties.to_dict()
 
+        database = self.database
+
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if host is not UNSET:
             field_dict["host"] = host
         if port is not UNSET:
             field_dict["port"] = port
-        if database is not UNSET:
-            field_dict["database"] = database
         if user is not UNSET:
             field_dict["user"] = user
         if password is not UNSET:
             field_dict["password"] = password
         if properties is not UNSET:
             field_dict["properties"] = properties
+        if database is not UNSET:
+            field_dict["database"] = database
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.redshift_parameters_spec_properties import (
-            RedshiftParametersSpecProperties,
+        from ..models.spark_parameters_spec_properties import (
+            SparkParametersSpecProperties,
         )
 
         d = src_dict.copy()
         host = d.pop("host", UNSET)
 
         port = d.pop("port", UNSET)
 
-        database = d.pop("database", UNSET)
-
         user = d.pop("user", UNSET)
 
         password = d.pop("password", UNSET)
 
         _properties = d.pop("properties", UNSET)
-        properties: Union[Unset, RedshiftParametersSpecProperties]
+        properties: Union[Unset, SparkParametersSpecProperties]
         if isinstance(_properties, Unset):
             properties = UNSET
         else:
-            properties = RedshiftParametersSpecProperties.from_dict(_properties)
+            properties = SparkParametersSpecProperties.from_dict(_properties)
 
-        redshift_parameters_spec = cls(
+        database = d.pop("database", UNSET)
+
+        spark_parameters_spec = cls(
             host=host,
             port=port,
-            database=database,
             user=user,
             password=password,
             properties=properties,
+            database=database,
         )
 
-        redshift_parameters_spec.additional_properties = d
-        return redshift_parameters_spec
+        spark_parameters_spec.additional_properties = d
+        return spark_parameters_spec
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dqops-1.1.0/dqops/client/models/redshift_parameters_spec_properties.py` & `dqops-1.2.0/dqops/client/models/redshift_parameters_spec_properties.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/remote_table_list_model.py` & `dqops-1.2.0/dqops/client/models/remote_table_list_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/repair_stored_data_queue_job_parameters.py` & `dqops-1.2.0/dqops/client/models/repair_stored_data_queue_job_parameters.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/rule_folder_model.py` & `dqops-1.2.0/dqops/client/models/rule_folder_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/rule_folder_model_folders.py` & `dqops-1.2.0/dqops/client/models/rule_folder_model_folders.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/rule_list_model.py` & `dqops-1.2.0/dqops/client/models/rule_list_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/rule_model.py` & `dqops-1.2.0/dqops/client/models/rule_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/rule_model_parameters.py` & `dqops-1.2.0/dqops/client/models/rule_model_parameters.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/rule_parameters_model.py` & `dqops-1.2.0/dqops/client/models/rule_parameters_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/rule_thresholds_model.py` & `dqops-1.2.0/dqops/client/models/rule_thresholds_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/rule_time_window_settings_spec.py` & `dqops-1.2.0/dqops/client/models/rule_time_window_settings_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/run_checks_on_table_parameters.py` & `dqops-1.2.0/dqops/client/models/run_checks_on_table_parameters.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/run_checks_parameters.py` & `dqops-1.2.0/dqops/client/models/run_checks_parameters.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/run_checks_queue_job_result.py` & `dqops-1.2.0/dqops/client/models/run_checks_queue_job_result.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/run_checks_result.py` & `dqops-1.2.0/dqops/client/models/run_checks_result.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/schema_model.py` & `dqops-1.2.0/dqops/client/models/schema_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/schema_remote_model.py` & `dqops-1.2.0/dqops/client/models/schema_remote_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/sensor_definition_spec.py` & `dqops-1.2.0/dqops/client/models/sensor_definition_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/sensor_definition_spec_parameters.py` & `dqops-1.2.0/dqops/client/models/sensor_definition_spec_parameters.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/sensor_folder_model.py` & `dqops-1.2.0/dqops/client/models/sensor_folder_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/sensor_folder_model_folders.py` & `dqops-1.2.0/dqops/client/models/sensor_folder_model_folders.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/sensor_list_model.py` & `dqops-1.2.0/dqops/client/models/sensor_list_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/sensor_model.py` & `dqops-1.2.0/dqops/client/models/sensor_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/sensor_readout_entry_model.py` & `dqops-1.2.0/dqops/client/models/sensor_readout_entry_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/sensor_readouts_list_model.py` & `dqops-1.2.0/dqops/client/models/table_timeliness_monthly_monitoring_checks_spec.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,145 +1,142 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union, cast
+from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
-from ..models.check_type import CheckType
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.sensor_readout_entry_model import SensorReadoutEntryModel
+    from ..models.table_data_freshness_check_spec import TableDataFreshnessCheckSpec
+    from ..models.table_data_ingestion_delay_check_spec import (
+        TableDataIngestionDelayCheckSpec,
+    )
+    from ..models.table_data_staleness_check_spec import TableDataStalenessCheckSpec
+    from ..models.table_timeliness_monthly_monitoring_checks_spec_custom_checks import (
+        TableTimelinessMonthlyMonitoringChecksSpecCustomChecks,
+    )
 
 
-T = TypeVar("T", bound="SensorReadoutsListModel")
+T = TypeVar("T", bound="TableTimelinessMonthlyMonitoringChecksSpec")
 
 
 @_attrs_define
-class SensorReadoutsListModel:
+class TableTimelinessMonthlyMonitoringChecksSpec:
     """
     Attributes:
-        check_name (Union[Unset, str]): Check name
-        check_display_name (Union[Unset, str]): Check display name
-        check_type (Union[Unset, CheckType]):
-        check_hash (Union[Unset, int]): Check hash
-        check_category (Union[Unset, str]): Check category name
-        sensor_name (Union[Unset, str]): Sensor name
-        data_group_names (Union[Unset, List[str]]): List of data groups that have values for this sensor readout (list
-            of time series)
-        data_group (Union[Unset, str]): Selected data group
-        sensor_readout_entries (Union[Unset, List['SensorReadoutEntryModel']]): Sensor readout entries
+        custom_checks (Union[Unset, TableTimelinessMonthlyMonitoringChecksSpecCustomChecks]): Dictionary of additional
+            custom checks within this category. The keys are check names defined in the definition section. The sensor
+            parameters and rules should match the type of the configured sensor and rule for the custom check.
+        monthly_data_freshness (Union[Unset, TableDataFreshnessCheckSpec]):
+        monthly_data_staleness (Union[Unset, TableDataStalenessCheckSpec]):
+        monthly_data_ingestion_delay (Union[Unset, TableDataIngestionDelayCheckSpec]):
     """
 
-    check_name: Union[Unset, str] = UNSET
-    check_display_name: Union[Unset, str] = UNSET
-    check_type: Union[Unset, CheckType] = UNSET
-    check_hash: Union[Unset, int] = UNSET
-    check_category: Union[Unset, str] = UNSET
-    sensor_name: Union[Unset, str] = UNSET
-    data_group_names: Union[Unset, List[str]] = UNSET
-    data_group: Union[Unset, str] = UNSET
-    sensor_readout_entries: Union[Unset, List["SensorReadoutEntryModel"]] = UNSET
+    custom_checks: Union[
+        Unset, "TableTimelinessMonthlyMonitoringChecksSpecCustomChecks"
+    ] = UNSET
+    monthly_data_freshness: Union[Unset, "TableDataFreshnessCheckSpec"] = UNSET
+    monthly_data_staleness: Union[Unset, "TableDataStalenessCheckSpec"] = UNSET
+    monthly_data_ingestion_delay: Union[
+        Unset, "TableDataIngestionDelayCheckSpec"
+    ] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        check_name = self.check_name
-        check_display_name = self.check_display_name
-        check_type: Union[Unset, str] = UNSET
-        if not isinstance(self.check_type, Unset):
-            check_type = self.check_type.value
-
-        check_hash = self.check_hash
-        check_category = self.check_category
-        sensor_name = self.sensor_name
-        data_group_names: Union[Unset, List[str]] = UNSET
-        if not isinstance(self.data_group_names, Unset):
-            data_group_names = self.data_group_names
-
-        data_group = self.data_group
-        sensor_readout_entries: Union[Unset, List[Dict[str, Any]]] = UNSET
-        if not isinstance(self.sensor_readout_entries, Unset):
-            sensor_readout_entries = []
-            for sensor_readout_entries_item_data in self.sensor_readout_entries:
-                sensor_readout_entries_item = sensor_readout_entries_item_data.to_dict()
-
-                sensor_readout_entries.append(sensor_readout_entries_item)
+        custom_checks: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.custom_checks, Unset):
+            custom_checks = self.custom_checks.to_dict()
+
+        monthly_data_freshness: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.monthly_data_freshness, Unset):
+            monthly_data_freshness = self.monthly_data_freshness.to_dict()
+
+        monthly_data_staleness: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.monthly_data_staleness, Unset):
+            monthly_data_staleness = self.monthly_data_staleness.to_dict()
+
+        monthly_data_ingestion_delay: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.monthly_data_ingestion_delay, Unset):
+            monthly_data_ingestion_delay = self.monthly_data_ingestion_delay.to_dict()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if check_name is not UNSET:
-            field_dict["checkName"] = check_name
-        if check_display_name is not UNSET:
-            field_dict["checkDisplayName"] = check_display_name
-        if check_type is not UNSET:
-            field_dict["checkType"] = check_type
-        if check_hash is not UNSET:
-            field_dict["checkHash"] = check_hash
-        if check_category is not UNSET:
-            field_dict["checkCategory"] = check_category
-        if sensor_name is not UNSET:
-            field_dict["sensorName"] = sensor_name
-        if data_group_names is not UNSET:
-            field_dict["dataGroupNames"] = data_group_names
-        if data_group is not UNSET:
-            field_dict["dataGroup"] = data_group
-        if sensor_readout_entries is not UNSET:
-            field_dict["sensorReadoutEntries"] = sensor_readout_entries
+        if custom_checks is not UNSET:
+            field_dict["custom_checks"] = custom_checks
+        if monthly_data_freshness is not UNSET:
+            field_dict["monthly_data_freshness"] = monthly_data_freshness
+        if monthly_data_staleness is not UNSET:
+            field_dict["monthly_data_staleness"] = monthly_data_staleness
+        if monthly_data_ingestion_delay is not UNSET:
+            field_dict["monthly_data_ingestion_delay"] = monthly_data_ingestion_delay
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.sensor_readout_entry_model import SensorReadoutEntryModel
+        from ..models.table_data_freshness_check_spec import TableDataFreshnessCheckSpec
+        from ..models.table_data_ingestion_delay_check_spec import (
+            TableDataIngestionDelayCheckSpec,
+        )
+        from ..models.table_data_staleness_check_spec import TableDataStalenessCheckSpec
+        from ..models.table_timeliness_monthly_monitoring_checks_spec_custom_checks import (
+            TableTimelinessMonthlyMonitoringChecksSpecCustomChecks,
+        )
 
         d = src_dict.copy()
-        check_name = d.pop("checkName", UNSET)
-
-        check_display_name = d.pop("checkDisplayName", UNSET)
-
-        _check_type = d.pop("checkType", UNSET)
-        check_type: Union[Unset, CheckType]
-        if isinstance(_check_type, Unset):
-            check_type = UNSET
+        _custom_checks = d.pop("custom_checks", UNSET)
+        custom_checks: Union[
+            Unset, TableTimelinessMonthlyMonitoringChecksSpecCustomChecks
+        ]
+        if isinstance(_custom_checks, Unset):
+            custom_checks = UNSET
         else:
-            check_type = CheckType(_check_type)
-
-        check_hash = d.pop("checkHash", UNSET)
-
-        check_category = d.pop("checkCategory", UNSET)
-
-        sensor_name = d.pop("sensorName", UNSET)
-
-        data_group_names = cast(List[str], d.pop("dataGroupNames", UNSET))
+            custom_checks = (
+                TableTimelinessMonthlyMonitoringChecksSpecCustomChecks.from_dict(
+                    _custom_checks
+                )
+            )
 
-        data_group = d.pop("dataGroup", UNSET)
+        _monthly_data_freshness = d.pop("monthly_data_freshness", UNSET)
+        monthly_data_freshness: Union[Unset, TableDataFreshnessCheckSpec]
+        if isinstance(_monthly_data_freshness, Unset):
+            monthly_data_freshness = UNSET
+        else:
+            monthly_data_freshness = TableDataFreshnessCheckSpec.from_dict(
+                _monthly_data_freshness
+            )
 
-        sensor_readout_entries = []
-        _sensor_readout_entries = d.pop("sensorReadoutEntries", UNSET)
-        for sensor_readout_entries_item_data in _sensor_readout_entries or []:
-            sensor_readout_entries_item = SensorReadoutEntryModel.from_dict(
-                sensor_readout_entries_item_data
+        _monthly_data_staleness = d.pop("monthly_data_staleness", UNSET)
+        monthly_data_staleness: Union[Unset, TableDataStalenessCheckSpec]
+        if isinstance(_monthly_data_staleness, Unset):
+            monthly_data_staleness = UNSET
+        else:
+            monthly_data_staleness = TableDataStalenessCheckSpec.from_dict(
+                _monthly_data_staleness
             )
 
-            sensor_readout_entries.append(sensor_readout_entries_item)
+        _monthly_data_ingestion_delay = d.pop("monthly_data_ingestion_delay", UNSET)
+        monthly_data_ingestion_delay: Union[Unset, TableDataIngestionDelayCheckSpec]
+        if isinstance(_monthly_data_ingestion_delay, Unset):
+            monthly_data_ingestion_delay = UNSET
+        else:
+            monthly_data_ingestion_delay = TableDataIngestionDelayCheckSpec.from_dict(
+                _monthly_data_ingestion_delay
+            )
 
-        sensor_readouts_list_model = cls(
-            check_name=check_name,
-            check_display_name=check_display_name,
-            check_type=check_type,
-            check_hash=check_hash,
-            check_category=check_category,
-            sensor_name=sensor_name,
-            data_group_names=data_group_names,
-            data_group=data_group,
-            sensor_readout_entries=sensor_readout_entries,
+        table_timeliness_monthly_monitoring_checks_spec = cls(
+            custom_checks=custom_checks,
+            monthly_data_freshness=monthly_data_freshness,
+            monthly_data_staleness=monthly_data_staleness,
+            monthly_data_ingestion_delay=monthly_data_ingestion_delay,
         )
 
-        sensor_readouts_list_model.additional_properties = d
-        return sensor_readouts_list_model
+        table_timeliness_monthly_monitoring_checks_spec.additional_properties = d
+        return table_timeliness_monthly_monitoring_checks_spec
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dqops-1.1.0/dqops/client/models/shared_credential_list_model.py` & `dqops-1.2.0/dqops/client/models/shared_credential_list_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/shared_credential_model.py` & `dqops-1.2.0/dqops/client/models/shared_credential_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/similar_check_model.py` & `dqops-1.2.0/dqops/client/models/similar_check_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/single_store_db_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/single_store_db_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/snowflake_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/snowflake_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/snowflake_parameters_spec_properties.py` & `dqops-1.2.0/dqops/client/models/snowflake_parameters_spec_properties.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/spark_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/sql_server_parameters_spec.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,110 +1,138 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
+from ..models.sql_server_authentication_mode import SqlServerAuthenticationMode
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.spark_parameters_spec_properties import SparkParametersSpecProperties
+    from ..models.sql_server_parameters_spec_properties import (
+        SqlServerParametersSpecProperties,
+    )
 
 
-T = TypeVar("T", bound="SparkParametersSpec")
+T = TypeVar("T", bound="SqlServerParametersSpec")
 
 
 @_attrs_define
-class SparkParametersSpec:
+class SqlServerParametersSpec:
     """
     Attributes:
-        host (Union[Unset, str]): Spark host name. Supports also a ${SPARK_HOST} configuration with a custom environment
-            variable.
-        port (Union[Unset, str]): Spark port number. The default port is 10000. Supports also a ${SPARK_PORT}
+        host (Union[Unset, str]): SQL Server host name. Supports also a ${SQLSERVER_HOST} configuration with a custom
+            environment variable.
+        port (Union[Unset, str]): SQL Server port number. The default port is 1433. Supports also a ${SQLSERVER_PORT}
             configuration with a custom environment variable.
-        user (Union[Unset, str]): Spark user name. The value can be in the ${ENVIRONMENT_VARIABLE_NAME} format to use
-            dynamic substitution.
-        password (Union[Unset, str]): Spark database password. The value can be in the ${ENVIRONMENT_VARIABLE_NAME}
+        database (Union[Unset, str]): SQL Server database name. The value can be in the ${ENVIRONMENT_VARIABLE_NAME}
             format to use dynamic substitution.
-        properties (Union[Unset, SparkParametersSpecProperties]): A dictionary of custom JDBC parameters that are added
-            to the JDBC connection string, a key/value dictionary.
-        database (Union[Unset, str]):
+        user (Union[Unset, str]): SQL Server user name. The value can be in the ${ENVIRONMENT_VARIABLE_NAME} format to
+            use dynamic substitution.
+        password (Union[Unset, str]): SQL Server database password. The value can be in the ${ENVIRONMENT_VARIABLE_NAME}
+            format to use dynamic substitution.
+        disable_encryption (Union[Unset, bool]): Disable SSL encryption parameter. The default value is false. You may
+            need to disable encryption when SQL Server is started in Docker.
+        authentication_mode (Union[Unset, SqlServerAuthenticationMode]):
+        properties (Union[Unset, SqlServerParametersSpecProperties]): A dictionary of custom JDBC parameters that are
+            added to the JDBC connection string, a key/value dictionary.
     """
 
     host: Union[Unset, str] = UNSET
     port: Union[Unset, str] = UNSET
+    database: Union[Unset, str] = UNSET
     user: Union[Unset, str] = UNSET
     password: Union[Unset, str] = UNSET
-    properties: Union[Unset, "SparkParametersSpecProperties"] = UNSET
-    database: Union[Unset, str] = UNSET
+    disable_encryption: Union[Unset, bool] = UNSET
+    authentication_mode: Union[Unset, SqlServerAuthenticationMode] = UNSET
+    properties: Union[Unset, "SqlServerParametersSpecProperties"] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         host = self.host
         port = self.port
+        database = self.database
         user = self.user
         password = self.password
+        disable_encryption = self.disable_encryption
+        authentication_mode: Union[Unset, str] = UNSET
+        if not isinstance(self.authentication_mode, Unset):
+            authentication_mode = self.authentication_mode.value
+
         properties: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.properties, Unset):
             properties = self.properties.to_dict()
 
-        database = self.database
-
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if host is not UNSET:
             field_dict["host"] = host
         if port is not UNSET:
             field_dict["port"] = port
+        if database is not UNSET:
+            field_dict["database"] = database
         if user is not UNSET:
             field_dict["user"] = user
         if password is not UNSET:
             field_dict["password"] = password
+        if disable_encryption is not UNSET:
+            field_dict["disable_encryption"] = disable_encryption
+        if authentication_mode is not UNSET:
+            field_dict["authentication_mode"] = authentication_mode
         if properties is not UNSET:
             field_dict["properties"] = properties
-        if database is not UNSET:
-            field_dict["database"] = database
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.spark_parameters_spec_properties import (
-            SparkParametersSpecProperties,
+        from ..models.sql_server_parameters_spec_properties import (
+            SqlServerParametersSpecProperties,
         )
 
         d = src_dict.copy()
         host = d.pop("host", UNSET)
 
         port = d.pop("port", UNSET)
 
+        database = d.pop("database", UNSET)
+
         user = d.pop("user", UNSET)
 
         password = d.pop("password", UNSET)
 
+        disable_encryption = d.pop("disable_encryption", UNSET)
+
+        _authentication_mode = d.pop("authentication_mode", UNSET)
+        authentication_mode: Union[Unset, SqlServerAuthenticationMode]
+        if isinstance(_authentication_mode, Unset):
+            authentication_mode = UNSET
+        else:
+            authentication_mode = SqlServerAuthenticationMode(_authentication_mode)
+
         _properties = d.pop("properties", UNSET)
-        properties: Union[Unset, SparkParametersSpecProperties]
+        properties: Union[Unset, SqlServerParametersSpecProperties]
         if isinstance(_properties, Unset):
             properties = UNSET
         else:
-            properties = SparkParametersSpecProperties.from_dict(_properties)
-
-        database = d.pop("database", UNSET)
+            properties = SqlServerParametersSpecProperties.from_dict(_properties)
 
-        spark_parameters_spec = cls(
+        sql_server_parameters_spec = cls(
             host=host,
             port=port,
+            database=database,
             user=user,
             password=password,
+            disable_encryption=disable_encryption,
+            authentication_mode=authentication_mode,
             properties=properties,
-            database=database,
         )
 
-        spark_parameters_spec.additional_properties = d
-        return spark_parameters_spec
+        sql_server_parameters_spec.additional_properties = d
+        return sql_server_parameters_spec
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dqops-1.1.0/dqops/client/models/spark_parameters_spec_properties.py` & `dqops-1.2.0/dqops/client/models/spark_parameters_spec_properties.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/spring_error_payload.py` & `dqops-1.2.0/dqops/client/models/spring_error_payload.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/sql_server_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/redshift_parameters_spec.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,138 +1,131 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
-from ..models.sql_server_authentication_mode import SqlServerAuthenticationMode
+from ..models.redshift_authentication_mode import RedshiftAuthenticationMode
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.sql_server_parameters_spec_properties import (
-        SqlServerParametersSpecProperties,
+    from ..models.redshift_parameters_spec_properties import (
+        RedshiftParametersSpecProperties,
     )
 
 
-T = TypeVar("T", bound="SqlServerParametersSpec")
+T = TypeVar("T", bound="RedshiftParametersSpec")
 
 
 @_attrs_define
-class SqlServerParametersSpec:
+class RedshiftParametersSpec:
     """
     Attributes:
-        host (Union[Unset, str]): SQL Server host name. Supports also a ${SQLSERVER_HOST} configuration with a custom
+        host (Union[Unset, str]): Redshift host name. Supports also a ${REDSHIFT_HOST} configuration with a custom
             environment variable.
-        port (Union[Unset, str]): SQL Server port number. The default port is 1433. Supports also a ${SQLSERVER_PORT}
+        port (Union[Unset, str]): Redshift port number. The default port is 5432. Supports also a ${REDSHIFT_PORT}
             configuration with a custom environment variable.
-        database (Union[Unset, str]): SQL Server database name. The value can be in the ${ENVIRONMENT_VARIABLE_NAME}
+        database (Union[Unset, str]): Redshift database name. The value can be in the ${ENVIRONMENT_VARIABLE_NAME}
             format to use dynamic substitution.
-        user (Union[Unset, str]): SQL Server user name. The value can be in the ${ENVIRONMENT_VARIABLE_NAME} format to
-            use dynamic substitution.
-        password (Union[Unset, str]): SQL Server database password. The value can be in the ${ENVIRONMENT_VARIABLE_NAME}
+        redshift_authentication_mode (Union[Unset, RedshiftAuthenticationMode]):
+        user (Union[Unset, str]): Redshift user name. The value can be in the ${ENVIRONMENT_VARIABLE_NAME} format to use
+            dynamic substitution.
+        password (Union[Unset, str]): Redshift database password. The value can be in the ${ENVIRONMENT_VARIABLE_NAME}
             format to use dynamic substitution.
-        disable_encryption (Union[Unset, bool]): Disable SSL encryption parameter. The default value is false. You may
-            need to disable encryption when SQL Server is started in Docker.
-        authentication_mode (Union[Unset, SqlServerAuthenticationMode]):
-        properties (Union[Unset, SqlServerParametersSpecProperties]): A dictionary of custom JDBC parameters that are
+        properties (Union[Unset, RedshiftParametersSpecProperties]): A dictionary of custom JDBC parameters that are
             added to the JDBC connection string, a key/value dictionary.
     """
 
     host: Union[Unset, str] = UNSET
     port: Union[Unset, str] = UNSET
     database: Union[Unset, str] = UNSET
+    redshift_authentication_mode: Union[Unset, RedshiftAuthenticationMode] = UNSET
     user: Union[Unset, str] = UNSET
     password: Union[Unset, str] = UNSET
-    disable_encryption: Union[Unset, bool] = UNSET
-    authentication_mode: Union[Unset, SqlServerAuthenticationMode] = UNSET
-    properties: Union[Unset, "SqlServerParametersSpecProperties"] = UNSET
+    properties: Union[Unset, "RedshiftParametersSpecProperties"] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         host = self.host
         port = self.port
         database = self.database
+        redshift_authentication_mode: Union[Unset, str] = UNSET
+        if not isinstance(self.redshift_authentication_mode, Unset):
+            redshift_authentication_mode = self.redshift_authentication_mode.value
+
         user = self.user
         password = self.password
-        disable_encryption = self.disable_encryption
-        authentication_mode: Union[Unset, str] = UNSET
-        if not isinstance(self.authentication_mode, Unset):
-            authentication_mode = self.authentication_mode.value
-
         properties: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.properties, Unset):
             properties = self.properties.to_dict()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if host is not UNSET:
             field_dict["host"] = host
         if port is not UNSET:
             field_dict["port"] = port
         if database is not UNSET:
             field_dict["database"] = database
+        if redshift_authentication_mode is not UNSET:
+            field_dict["redshift_authentication_mode"] = redshift_authentication_mode
         if user is not UNSET:
             field_dict["user"] = user
         if password is not UNSET:
             field_dict["password"] = password
-        if disable_encryption is not UNSET:
-            field_dict["disable_encryption"] = disable_encryption
-        if authentication_mode is not UNSET:
-            field_dict["authentication_mode"] = authentication_mode
         if properties is not UNSET:
             field_dict["properties"] = properties
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.sql_server_parameters_spec_properties import (
-            SqlServerParametersSpecProperties,
+        from ..models.redshift_parameters_spec_properties import (
+            RedshiftParametersSpecProperties,
         )
 
         d = src_dict.copy()
         host = d.pop("host", UNSET)
 
         port = d.pop("port", UNSET)
 
         database = d.pop("database", UNSET)
 
+        _redshift_authentication_mode = d.pop("redshift_authentication_mode", UNSET)
+        redshift_authentication_mode: Union[Unset, RedshiftAuthenticationMode]
+        if isinstance(_redshift_authentication_mode, Unset):
+            redshift_authentication_mode = UNSET
+        else:
+            redshift_authentication_mode = RedshiftAuthenticationMode(
+                _redshift_authentication_mode
+            )
+
         user = d.pop("user", UNSET)
 
         password = d.pop("password", UNSET)
 
-        disable_encryption = d.pop("disable_encryption", UNSET)
-
-        _authentication_mode = d.pop("authentication_mode", UNSET)
-        authentication_mode: Union[Unset, SqlServerAuthenticationMode]
-        if isinstance(_authentication_mode, Unset):
-            authentication_mode = UNSET
-        else:
-            authentication_mode = SqlServerAuthenticationMode(_authentication_mode)
-
         _properties = d.pop("properties", UNSET)
-        properties: Union[Unset, SqlServerParametersSpecProperties]
+        properties: Union[Unset, RedshiftParametersSpecProperties]
         if isinstance(_properties, Unset):
             properties = UNSET
         else:
-            properties = SqlServerParametersSpecProperties.from_dict(_properties)
+            properties = RedshiftParametersSpecProperties.from_dict(_properties)
 
-        sql_server_parameters_spec = cls(
+        redshift_parameters_spec = cls(
             host=host,
             port=port,
             database=database,
+            redshift_authentication_mode=redshift_authentication_mode,
             user=user,
             password=password,
-            disable_encryption=disable_encryption,
-            authentication_mode=authentication_mode,
             properties=properties,
         )
 
-        sql_server_parameters_spec.additional_properties = d
-        return sql_server_parameters_spec
+        redshift_parameters_spec.additional_properties = d
+        return redshift_parameters_spec
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dqops-1.1.0/dqops/client/models/sql_server_parameters_spec_properties.py` & `dqops-1.2.0/dqops/client/models/sql_server_parameters_spec_properties.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/statistics_collector_search_filters.py` & `dqops-1.2.0/dqops/client/models/statistics_collector_search_filters.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         tags (Union[Unset, List[str]]): An array of tags assigned to the table. All tags must be present on a table to
             match. The tags can use patterns:  'prefix\*', '\*suffix', 'prefix\*suffix'. The tags are assigned to the table
             on the data grouping screen when any of the data grouping hierarchy level is assigned a static value, which is a
             tag.
         labels (Union[Unset, List[str]]): An array of labels assigned to the table. All labels must be present on a
             table to match. The labels can use patterns:  'prefix\*', '\*suffix', 'prefix\*suffix'. The labels are assigned
             on the labels screen and stored in the *labels* node in the *.dqotable.yaml* file.
+        max_results (Union[Unset, int]): Optional limit for the maximum number of results to return.
         column_names (Union[Unset, List[str]]): The list of column names or column name patters. This field accepts
             search patterns in the format: 'fk_\*', '\*_id', 'prefix\*suffix'.
         collector_name (Union[Unset, str]): The target statistics collector name to capture only selected statistics.
             Uses the short collector nameThis field supports search patterns such as: 'prefix\*', '\*suffix',
             'prefix_\*_suffix'. In order to collect only top 10 most common column samples, use 'column_samples'.
         sensor_name (Union[Unset, str]): The target sensor name to run only data quality checks that are using this
             sensor. Uses the full sensor name which is the full folder path within the *sensors* folder. This field supports
@@ -48,14 +49,15 @@
     """
 
     connection: Union[Unset, str] = UNSET
     full_table_name: Union[Unset, str] = UNSET
     enabled: Union[Unset, bool] = UNSET
     tags: Union[Unset, List[str]] = UNSET
     labels: Union[Unset, List[str]] = UNSET
+    max_results: Union[Unset, int] = UNSET
     column_names: Union[Unset, List[str]] = UNSET
     collector_name: Union[Unset, str] = UNSET
     sensor_name: Union[Unset, str] = UNSET
     collector_category: Union[Unset, str] = UNSET
     target: Union[Unset, StatisticsCollectorTarget] = UNSET
     collectors_hierarchy_ids_models: Union[Unset, List["HierarchyIdModel"]] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
@@ -68,14 +70,15 @@
         if not isinstance(self.tags, Unset):
             tags = self.tags
 
         labels: Union[Unset, List[str]] = UNSET
         if not isinstance(self.labels, Unset):
             labels = self.labels
 
+        max_results = self.max_results
         column_names: Union[Unset, List[str]] = UNSET
         if not isinstance(self.column_names, Unset):
             column_names = self.column_names
 
         collector_name = self.collector_name
         sensor_name = self.sensor_name
         collector_category = self.collector_category
@@ -106,14 +109,16 @@
             field_dict["fullTableName"] = full_table_name
         if enabled is not UNSET:
             field_dict["enabled"] = enabled
         if tags is not UNSET:
             field_dict["tags"] = tags
         if labels is not UNSET:
             field_dict["labels"] = labels
+        if max_results is not UNSET:
+            field_dict["maxResults"] = max_results
         if column_names is not UNSET:
             field_dict["columnNames"] = column_names
         if collector_name is not UNSET:
             field_dict["collectorName"] = collector_name
         if sensor_name is not UNSET:
             field_dict["sensorName"] = sensor_name
         if collector_category is not UNSET:
@@ -136,14 +141,16 @@
 
         enabled = d.pop("enabled", UNSET)
 
         tags = cast(List[str], d.pop("tags", UNSET))
 
         labels = cast(List[str], d.pop("labels", UNSET))
 
+        max_results = d.pop("maxResults", UNSET)
+
         column_names = cast(List[str], d.pop("columnNames", UNSET))
 
         collector_name = d.pop("collectorName", UNSET)
 
         sensor_name = d.pop("sensorName", UNSET)
 
         collector_category = d.pop("collectorCategory", UNSET)
@@ -168,14 +175,15 @@
 
         statistics_collector_search_filters = cls(
             connection=connection,
             full_table_name=full_table_name,
             enabled=enabled,
             tags=tags,
             labels=labels,
+            max_results=max_results,
             column_names=column_names,
             collector_name=collector_name,
             sensor_name=sensor_name,
             collector_category=collector_category,
             target=target,
             collectors_hierarchy_ids_models=collectors_hierarchy_ids_models,
         )
```

### Comparing `dqops-1.1.0/dqops/client/models/statistics_metric_model.py` & `dqops-1.2.0/dqops/client/models/statistics_metric_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/statistics_metric_model_result.py` & `dqops-1.2.0/dqops/client/models/statistics_metric_model_result.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/synchronize_multiple_folders_dqo_queue_job_parameters.py` & `dqops-1.2.0/dqops/client/models/synchronize_multiple_folders_dqo_queue_job_parameters.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/synchronize_multiple_folders_queue_job_result.py` & `dqops-1.2.0/dqops/client/models/synchronize_multiple_folders_queue_job_result.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/synchronize_root_folder_dqo_queue_job_parameters.py` & `dqops-1.2.0/dqops/client/models/synchronize_root_folder_dqo_queue_job_parameters.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/synchronize_root_folder_parameters.py` & `dqops-1.2.0/dqops/client/models/synchronize_root_folder_parameters.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_accuracy_daily_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/table_accuracy_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_accuracy_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/table_accuracy_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_accuracy_monthly_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/table_accuracy_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_accuracy_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/table_accuracy_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_accuracy_profiling_checks_spec.py` & `dqops-1.2.0/dqops/client/models/table_accuracy_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_accuracy_profiling_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/table_accuracy_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_accuracy_total_row_count_match_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/table_accuracy_total_row_count_match_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_accuracy_total_row_count_match_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/table_accuracy_total_row_count_match_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_availability_check_spec.py` & `dqops-1.2.0/dqops/client/models/table_availability_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_availability_daily_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/table_availability_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_availability_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/table_availability_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_availability_monthly_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/table_availability_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_availability_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/table_availability_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_availability_profiling_checks_spec.py` & `dqops-1.2.0/dqops/client/models/table_availability_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_availability_profiling_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/table_availability_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_availability_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/table_availability_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_column_count_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/table_column_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_column_list_ordered_hash_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/table_column_list_ordered_hash_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_column_list_unordered_hash_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/table_column_list_unordered_hash_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_column_types_hash_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/table_column_types_hash_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_columns_statistics_model.py` & `dqops-1.2.0/dqops/client/models/table_columns_statistics_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_comparison_column_count_match_check_spec.py` & `dqops-1.2.0/dqops/client/models/table_comparison_column_count_match_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_comparison_column_results_model.py` & `dqops-1.2.0/dqops/client/models/table_comparison_column_results_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_comparison_column_results_model_column_comparison_results.py` & `dqops-1.2.0/dqops/client/models/table_comparison_column_results_model_column_comparison_results.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_comparison_configuration_model.py` & `dqops-1.2.0/dqops/client/models/table_comparison_configuration_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_comparison_configuration_spec.py` & `dqops-1.2.0/dqops/client/models/table_comparison_configuration_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_comparison_daily_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/table_comparison_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_comparison_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/table_comparison_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_comparison_daily_partitioned_checks_spec.py` & `dqops-1.2.0/dqops/client/models/table_comparison_daily_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_comparison_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/table_comparison_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_comparison_grouping_column_pair_model.py` & `dqops-1.2.0/dqops/client/models/table_comparison_grouping_column_pair_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_comparison_grouping_columns_pair_spec.py` & `dqops-1.2.0/dqops/client/models/table_comparison_grouping_columns_pair_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_comparison_model.py` & `dqops-1.2.0/dqops/client/models/table_comparison_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_comparison_monthly_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/table_comparison_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_comparison_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/table_comparison_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_comparison_monthly_partitioned_checks_spec.py` & `dqops-1.2.0/dqops/client/models/table_comparison_monthly_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_comparison_monthly_partitioned_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/table_comparison_monthly_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_comparison_profiling_checks_spec.py` & `dqops-1.2.0/dqops/client/models/table_comparison_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_comparison_profiling_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/table_comparison_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_comparison_results_model.py` & `dqops-1.2.0/dqops/client/models/table_comparison_results_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_comparison_results_model_column_comparison_results.py` & `dqops-1.2.0/dqops/client/models/table_comparison_results_model_column_comparison_results.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_comparison_results_model_table_comparison_results.py` & `dqops-1.2.0/dqops/client/models/table_comparison_results_model_table_comparison_results.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_comparison_row_count_match_check_spec.py` & `dqops-1.2.0/dqops/client/models/table_comparison_row_count_match_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_current_data_quality_status_model.py` & `dqops-1.2.0/dqops/client/models/table_current_data_quality_status_model.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 if TYPE_CHECKING:
     from ..models.table_current_data_quality_status_model_checks import (
         TableCurrentDataQualityStatusModelChecks,
     )
     from ..models.table_current_data_quality_status_model_columns import (
         TableCurrentDataQualityStatusModelColumns,
     )
+    from ..models.table_current_data_quality_status_model_dimensions import (
+        TableCurrentDataQualityStatusModelDimensions,
+    )
 
 
 T = TypeVar("T", bound="TableCurrentDataQualityStatusModel")
 
 
 @_attrs_define
 class TableCurrentDataQualityStatusModel:
@@ -51,14 +54,16 @@
                 data quality checks. DQOps counts data quality issues at a warning severity level as passed checks. The data
                 quality KPI score is a value in the range 0..100.
             checks (Union[Unset, TableCurrentDataQualityStatusModelChecks]): The dictionary of statuses for data quality
                 checks. The keys are data quality check names, the values are the current data quality check statuses that
                 describe the most current status.
             columns (Union[Unset, TableCurrentDataQualityStatusModelColumns]): Dictionary of data statues for all columns
                 that have any known data quality results. The keys in the dictionary are the column names.
+            dimensions (Union[Unset, TableCurrentDataQualityStatusModelDimensions]): Dictionary of the current data quality
+                statues for each data quality dimension.
     """
 
     connection_name: Union[Unset, str] = UNSET
     schema_name: Union[Unset, str] = UNSET
     table_name: Union[Unset, str] = UNSET
     current_severity: Union[Unset, RuleSeverityLevel] = UNSET
     highest_historical_severity: Union[Unset, RuleSeverityLevel] = UNSET
@@ -68,14 +73,15 @@
     warnings: Union[Unset, int] = UNSET
     errors: Union[Unset, int] = UNSET
     fatals: Union[Unset, int] = UNSET
     execution_errors: Union[Unset, int] = UNSET
     data_quality_kpi: Union[Unset, float] = UNSET
     checks: Union[Unset, "TableCurrentDataQualityStatusModelChecks"] = UNSET
     columns: Union[Unset, "TableCurrentDataQualityStatusModelColumns"] = UNSET
+    dimensions: Union[Unset, "TableCurrentDataQualityStatusModelDimensions"] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         connection_name = self.connection_name
         schema_name = self.schema_name
         table_name = self.table_name
         current_severity: Union[Unset, str] = UNSET
@@ -98,14 +104,18 @@
         if not isinstance(self.checks, Unset):
             checks = self.checks.to_dict()
 
         columns: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.columns, Unset):
             columns = self.columns.to_dict()
 
+        dimensions: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.dimensions, Unset):
+            dimensions = self.dimensions.to_dict()
+
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if connection_name is not UNSET:
             field_dict["connection_name"] = connection_name
         if schema_name is not UNSET:
             field_dict["schema_name"] = schema_name
@@ -131,25 +141,30 @@
             field_dict["execution_errors"] = execution_errors
         if data_quality_kpi is not UNSET:
             field_dict["data_quality_kpi"] = data_quality_kpi
         if checks is not UNSET:
             field_dict["checks"] = checks
         if columns is not UNSET:
             field_dict["columns"] = columns
+        if dimensions is not UNSET:
+            field_dict["dimensions"] = dimensions
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.table_current_data_quality_status_model_checks import (
             TableCurrentDataQualityStatusModelChecks,
         )
         from ..models.table_current_data_quality_status_model_columns import (
             TableCurrentDataQualityStatusModelColumns,
         )
+        from ..models.table_current_data_quality_status_model_dimensions import (
+            TableCurrentDataQualityStatusModelDimensions,
+        )
 
         d = src_dict.copy()
         connection_name = d.pop("connection_name", UNSET)
 
         schema_name = d.pop("schema_name", UNSET)
 
         table_name = d.pop("table_name", UNSET)
@@ -196,14 +211,23 @@
         _columns = d.pop("columns", UNSET)
         columns: Union[Unset, TableCurrentDataQualityStatusModelColumns]
         if isinstance(_columns, Unset):
             columns = UNSET
         else:
             columns = TableCurrentDataQualityStatusModelColumns.from_dict(_columns)
 
+        _dimensions = d.pop("dimensions", UNSET)
+        dimensions: Union[Unset, TableCurrentDataQualityStatusModelDimensions]
+        if isinstance(_dimensions, Unset):
+            dimensions = UNSET
+        else:
+            dimensions = TableCurrentDataQualityStatusModelDimensions.from_dict(
+                _dimensions
+            )
+
         table_current_data_quality_status_model = cls(
             connection_name=connection_name,
             schema_name=schema_name,
             table_name=table_name,
             current_severity=current_severity,
             highest_historical_severity=highest_historical_severity,
             last_check_executed_at=last_check_executed_at,
@@ -212,14 +236,15 @@
             warnings=warnings,
             errors=errors,
             fatals=fatals,
             execution_errors=execution_errors,
             data_quality_kpi=data_quality_kpi,
             checks=checks,
             columns=columns,
+            dimensions=dimensions,
         )
 
         table_current_data_quality_status_model.additional_properties = d
         return table_current_data_quality_status_model
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `dqops-1.1.0/dqops/client/models/table_current_data_quality_status_model_checks.py` & `dqops-1.2.0/dqops/client/models/table_current_data_quality_status_model_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_current_data_quality_status_model_columns.py` & `dqops-1.2.0/dqops/client/models/table_current_data_quality_status_model_columns.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_custom_sql_daily_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/table_custom_sql_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_custom_sql_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/table_custom_sql_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_custom_sql_daily_partitioned_checks_spec.py` & `dqops-1.2.0/dqops/client/models/table_custom_sql_daily_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_custom_sql_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/table_custom_sql_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_custom_sql_monthly_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/table_custom_sql_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_custom_sql_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/table_custom_sql_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_custom_sql_monthly_partitioned_checks_spec.py` & `dqops-1.2.0/dqops/client/models/table_custom_sql_monthly_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_custom_sql_monthly_partitioned_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/table_custom_sql_monthly_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_custom_sql_profiling_checks_spec.py` & `dqops-1.2.0/dqops/client/models/table_custom_sql_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_custom_sql_profiling_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/table_custom_sql_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_daily_monitoring_check_categories_spec.py` & `dqops-1.2.0/dqops/client/models/table_daily_monitoring_check_categories_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_daily_monitoring_check_categories_spec_comparisons.py` & `dqops-1.2.0/dqops/client/models/table_daily_monitoring_check_categories_spec_comparisons.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_daily_monitoring_check_categories_spec_custom.py` & `dqops-1.2.0/dqops/client/models/table_daily_monitoring_check_categories_spec_custom.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_daily_partitioned_check_categories_spec.py` & `dqops-1.2.0/dqops/client/models/table_daily_partitioned_check_categories_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_daily_partitioned_check_categories_spec_comparisons.py` & `dqops-1.2.0/dqops/client/models/table_daily_partitioned_check_categories_spec_comparisons.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_daily_partitioned_check_categories_spec_custom.py` & `dqops-1.2.0/dqops/client/models/table_daily_partitioned_check_categories_spec_custom.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_data_freshness_check_spec.py` & `dqops-1.2.0/dqops/client/models/table_data_freshness_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_data_ingestion_delay_check_spec.py` & `dqops-1.2.0/dqops/client/models/table_data_ingestion_delay_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_data_staleness_check_spec.py` & `dqops-1.2.0/dqops/client/models/table_data_staleness_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_default_checks_pattern_spec.py` & `dqops-1.2.0/dqops/client/models/table_default_checks_pattern_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_incident_grouping_spec.py` & `dqops-1.2.0/dqops/client/models/table_incident_grouping_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_list_model.py` & `dqops-1.2.0/dqops/client/models/table_list_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union, cast
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..models.profiling_time_period_truncation import ProfilingTimePeriodTruncation
 from ..types import UNSET, Unset
 
@@ -12,39 +12,48 @@
         DeleteStoredDataQueueJobParameters,
     )
     from ..models.file_format_spec import FileFormatSpec
     from ..models.physical_table_name import PhysicalTableName
     from ..models.statistics_collector_search_filters import (
         StatisticsCollectorSearchFilters,
     )
+    from ..models.table_current_data_quality_status_model import (
+        TableCurrentDataQualityStatusModel,
+    )
     from ..models.table_owner_spec import TableOwnerSpec
 
 
 T = TypeVar("T", bound="TableListModel")
 
 
 @_attrs_define
 class TableListModel:
     """Table list model with a subset of parameters, excluding all nested objects.
 
     Attributes:
         connection_name (Union[Unset, str]): Connection name.
         table_hash (Union[Unset, int]): Table hash that identifies the table using a unique hash code.
         target (Union[Unset, PhysicalTableName]):
+        labels (Union[Unset, List[str]]): List of labels applied to the table.
         disabled (Union[Unset, bool]): Disables all data quality checks on the table. Data quality checks will not be
             executed.
         stage (Union[Unset, str]): Stage name.
         filter_ (Union[Unset, str]): SQL WHERE clause added to the sensor queries.
         priority (Union[Unset, int]): Table priority (1, 2, 3, 4, ...). The tables can be assigned a priority level. The
             table priority is copied into each data quality check result and a sensor result, enabling efficient grouping of
             more and less important tables during a data quality improvement project, when the data quality issues on higher
             priority tables are fixed before data quality issues on less important tables.
         owner (Union[Unset, TableOwnerSpec]):
         profiling_checks_result_truncation (Union[Unset, ProfilingTimePeriodTruncation]):
         file_format (Union[Unset, FileFormatSpec]):
+        data_quality_status (Union[Unset, TableCurrentDataQualityStatusModel]): The table's most recent data quality
+            status. It is a summary of the results of the most recently executed data quality checks on the table. Verify
+            the value of the highest_severity_level to see if there are any data quality issues on the table. The values of
+            severity levels are: 0 - all data quality checks passed, 1 - a warning was detected, 2 - an error was detected,
+            3 - a fatal data quality issue was detected.
         has_any_configured_checks (Union[Unset, bool]): True when the table has any checks configured.
         has_any_configured_profiling_checks (Union[Unset, bool]): True when the table has any profiling checks
             configured.
         has_any_configured_monitoring_checks (Union[Unset, bool]): True when the table has any monitoring checks
             configured.
         has_any_configured_partition_checks (Union[Unset, bool]): True when the table has any partition checks
             configured.
@@ -69,23 +78,25 @@
             This field is null when the YAML file is valid. If an error was captured, this field returns the file parsing
             error message and the file location.
     """
 
     connection_name: Union[Unset, str] = UNSET
     table_hash: Union[Unset, int] = UNSET
     target: Union[Unset, "PhysicalTableName"] = UNSET
+    labels: Union[Unset, List[str]] = UNSET
     disabled: Union[Unset, bool] = UNSET
     stage: Union[Unset, str] = UNSET
     filter_: Union[Unset, str] = UNSET
     priority: Union[Unset, int] = UNSET
     owner: Union[Unset, "TableOwnerSpec"] = UNSET
     profiling_checks_result_truncation: Union[
         Unset, ProfilingTimePeriodTruncation
     ] = UNSET
     file_format: Union[Unset, "FileFormatSpec"] = UNSET
+    data_quality_status: Union[Unset, "TableCurrentDataQualityStatusModel"] = UNSET
     has_any_configured_checks: Union[Unset, bool] = UNSET
     has_any_configured_profiling_checks: Union[Unset, bool] = UNSET
     has_any_configured_monitoring_checks: Union[Unset, bool] = UNSET
     has_any_configured_partition_checks: Union[Unset, bool] = UNSET
     partitioning_configuration_missing: Union[Unset, bool] = UNSET
     run_checks_job_template: Union[Unset, "CheckSearchFilters"] = UNSET
     run_profiling_checks_job_template: Union[Unset, "CheckSearchFilters"] = UNSET
@@ -105,14 +116,18 @@
     def to_dict(self) -> Dict[str, Any]:
         connection_name = self.connection_name
         table_hash = self.table_hash
         target: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.target, Unset):
             target = self.target.to_dict()
 
+        labels: Union[Unset, List[str]] = UNSET
+        if not isinstance(self.labels, Unset):
+            labels = self.labels
+
         disabled = self.disabled
         stage = self.stage
         filter_ = self.filter_
         priority = self.priority
         owner: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.owner, Unset):
             owner = self.owner.to_dict()
@@ -123,14 +138,18 @@
                 self.profiling_checks_result_truncation.value
             )
 
         file_format: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.file_format, Unset):
             file_format = self.file_format.to_dict()
 
+        data_quality_status: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.data_quality_status, Unset):
+            data_quality_status = self.data_quality_status.to_dict()
+
         has_any_configured_checks = self.has_any_configured_checks
         has_any_configured_profiling_checks = self.has_any_configured_profiling_checks
         has_any_configured_monitoring_checks = self.has_any_configured_monitoring_checks
         has_any_configured_partition_checks = self.has_any_configured_partition_checks
         partitioning_configuration_missing = self.partitioning_configuration_missing
         run_checks_job_template: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.run_checks_job_template, Unset):
@@ -175,14 +194,16 @@
         field_dict.update({})
         if connection_name is not UNSET:
             field_dict["connection_name"] = connection_name
         if table_hash is not UNSET:
             field_dict["table_hash"] = table_hash
         if target is not UNSET:
             field_dict["target"] = target
+        if labels is not UNSET:
+            field_dict["labels"] = labels
         if disabled is not UNSET:
             field_dict["disabled"] = disabled
         if stage is not UNSET:
             field_dict["stage"] = stage
         if filter_ is not UNSET:
             field_dict["filter"] = filter_
         if priority is not UNSET:
@@ -191,14 +212,16 @@
             field_dict["owner"] = owner
         if profiling_checks_result_truncation is not UNSET:
             field_dict[
                 "profiling_checks_result_truncation"
             ] = profiling_checks_result_truncation
         if file_format is not UNSET:
             field_dict["file_format"] = file_format
+        if data_quality_status is not UNSET:
+            field_dict["data_quality_status"] = data_quality_status
         if has_any_configured_checks is not UNSET:
             field_dict["has_any_configured_checks"] = has_any_configured_checks
         if has_any_configured_profiling_checks is not UNSET:
             field_dict[
                 "has_any_configured_profiling_checks"
             ] = has_any_configured_profiling_checks
         if has_any_configured_monitoring_checks is not UNSET:
@@ -253,28 +276,33 @@
             DeleteStoredDataQueueJobParameters,
         )
         from ..models.file_format_spec import FileFormatSpec
         from ..models.physical_table_name import PhysicalTableName
         from ..models.statistics_collector_search_filters import (
             StatisticsCollectorSearchFilters,
         )
+        from ..models.table_current_data_quality_status_model import (
+            TableCurrentDataQualityStatusModel,
+        )
         from ..models.table_owner_spec import TableOwnerSpec
 
         d = src_dict.copy()
         connection_name = d.pop("connection_name", UNSET)
 
         table_hash = d.pop("table_hash", UNSET)
 
         _target = d.pop("target", UNSET)
         target: Union[Unset, PhysicalTableName]
         if isinstance(_target, Unset):
             target = UNSET
         else:
             target = PhysicalTableName.from_dict(_target)
 
+        labels = cast(List[str], d.pop("labels", UNSET))
+
         disabled = d.pop("disabled", UNSET)
 
         stage = d.pop("stage", UNSET)
 
         filter_ = d.pop("filter", UNSET)
 
         priority = d.pop("priority", UNSET)
@@ -300,14 +328,23 @@
         _file_format = d.pop("file_format", UNSET)
         file_format: Union[Unset, FileFormatSpec]
         if isinstance(_file_format, Unset):
             file_format = UNSET
         else:
             file_format = FileFormatSpec.from_dict(_file_format)
 
+        _data_quality_status = d.pop("data_quality_status", UNSET)
+        data_quality_status: Union[Unset, TableCurrentDataQualityStatusModel]
+        if isinstance(_data_quality_status, Unset):
+            data_quality_status = UNSET
+        else:
+            data_quality_status = TableCurrentDataQualityStatusModel.from_dict(
+                _data_quality_status
+            )
+
         has_any_configured_checks = d.pop("has_any_configured_checks", UNSET)
 
         has_any_configured_profiling_checks = d.pop(
             "has_any_configured_profiling_checks", UNSET
         )
 
         has_any_configured_monitoring_checks = d.pop(
@@ -396,21 +433,23 @@
 
         yaml_parsing_error = d.pop("yaml_parsing_error", UNSET)
 
         table_list_model = cls(
             connection_name=connection_name,
             table_hash=table_hash,
             target=target,
+            labels=labels,
             disabled=disabled,
             stage=stage,
             filter_=filter_,
             priority=priority,
             owner=owner,
             profiling_checks_result_truncation=profiling_checks_result_truncation,
             file_format=file_format,
+            data_quality_status=data_quality_status,
             has_any_configured_checks=has_any_configured_checks,
             has_any_configured_profiling_checks=has_any_configured_profiling_checks,
             has_any_configured_monitoring_checks=has_any_configured_monitoring_checks,
             has_any_configured_partition_checks=has_any_configured_partition_checks,
             partitioning_configuration_missing=partitioning_configuration_missing,
             run_checks_job_template=run_checks_job_template,
             run_profiling_checks_job_template=run_profiling_checks_job_template,
```

### Comparing `dqops-1.1.0/dqops/client/models/table_model.py` & `dqops-1.2.0/dqops/client/models/table_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_monitoring_check_categories_spec.py` & `dqops-1.2.0/dqops/client/models/table_monitoring_check_categories_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_monthly_monitoring_check_categories_spec.py` & `dqops-1.2.0/dqops/client/models/table_monthly_monitoring_check_categories_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_monthly_monitoring_check_categories_spec_comparisons.py` & `dqops-1.2.0/dqops/client/models/table_monthly_monitoring_check_categories_spec_comparisons.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_monthly_monitoring_check_categories_spec_custom.py` & `dqops-1.2.0/dqops/client/models/table_monthly_monitoring_check_categories_spec_custom.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_monthly_partitioned_check_categories_spec.py` & `dqops-1.2.0/dqops/client/models/table_monthly_partitioned_check_categories_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_monthly_partitioned_check_categories_spec_comparisons.py` & `dqops-1.2.0/dqops/client/models/table_monthly_partitioned_check_categories_spec_comparisons.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_monthly_partitioned_check_categories_spec_custom.py` & `dqops-1.2.0/dqops/client/models/table_monthly_partitioned_check_categories_spec_custom.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_owner_spec.py` & `dqops-1.2.0/dqops/client/models/table_owner_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_partition_reload_lag_check_spec.py` & `dqops-1.2.0/dqops/client/models/table_partition_reload_lag_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_partitioned_check_categories_spec.py` & `dqops-1.2.0/dqops/client/models/table_partitioned_check_categories_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_partitioning_model.py` & `dqops-1.2.0/dqops/client/models/table_partitioning_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_profiling_check_categories_spec.py` & `dqops-1.2.0/dqops/client/models/table_profiling_check_categories_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_profiling_check_categories_spec_comparisons.py` & `dqops-1.2.0/dqops/client/models/table_profiling_check_categories_spec_comparisons.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_profiling_check_categories_spec_custom.py` & `dqops-1.2.0/dqops/client/models/table_profiling_check_categories_spec_custom.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_row_count_anomaly_differencing_check_spec.py` & `dqops-1.2.0/dqops/client/models/table_row_count_anomaly_differencing_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_row_count_anomaly_stationary_partition_check_spec.py` & `dqops-1.2.0/dqops/client/models/table_row_count_anomaly_stationary_partition_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_row_count_change_1_day_check_spec.py` & `dqops-1.2.0/dqops/client/models/table_row_count_change_1_day_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_row_count_change_30_days_check_spec.py` & `dqops-1.2.0/dqops/client/models/table_row_count_change_30_days_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_row_count_change_7_days_check_spec.py` & `dqops-1.2.0/dqops/client/models/table_row_count_change_7_days_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_row_count_change_check_spec.py` & `dqops-1.2.0/dqops/client/models/table_row_count_change_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_row_count_check_spec.py` & `dqops-1.2.0/dqops/client/models/table_row_count_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_schema_column_count_changed_check_spec.py` & `dqops-1.2.0/dqops/client/models/table_schema_column_count_changed_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_schema_column_count_check_spec.py` & `dqops-1.2.0/dqops/client/models/table_schema_column_count_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_schema_column_count_statistics_collector_spec.py` & `dqops-1.2.0/dqops/client/models/table_schema_column_count_statistics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_schema_column_list_changed_check_spec.py` & `dqops-1.2.0/dqops/client/models/table_schema_column_list_changed_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_schema_column_list_or_order_changed_check_spec.py` & `dqops-1.2.0/dqops/client/models/table_schema_column_list_or_order_changed_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_schema_column_types_changed_check_spec.py` & `dqops-1.2.0/dqops/client/models/table_schema_column_types_changed_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_schema_daily_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/table_schema_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_schema_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/table_schema_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_schema_monthly_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/table_schema_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_schema_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/table_schema_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_schema_profiling_checks_spec.py` & `dqops-1.2.0/dqops/client/models/table_schema_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_schema_profiling_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/table_schema_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_schema_statistics_collectors_spec.py` & `dqops-1.2.0/dqops/client/models/table_schema_statistics_collectors_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_spec.py` & `dqops-1.2.0/dqops/client/models/table_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_spec_columns.py` & `dqops-1.2.0/dqops/client/models/table_spec_columns.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_spec_groupings.py` & `dqops-1.2.0/dqops/client/models/table_spec_groupings.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_spec_table_comparisons.py` & `dqops-1.2.0/dqops/client/models/table_spec_table_comparisons.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_sql_aggregate_expression_check_spec.py` & `dqops-1.2.0/dqops/client/models/table_sql_aggregate_expression_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_sql_aggregated_expression_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/table_sql_aggregated_expression_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_sql_condition_failed_check_spec.py` & `dqops-1.2.0/dqops/client/models/table_sql_condition_failed_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_sql_condition_failed_count_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/table_sql_condition_failed_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_sql_condition_passed_percent_check_spec.py` & `dqops-1.2.0/dqops/client/models/table_sql_condition_passed_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_sql_condition_passed_percent_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/table_sql_condition_passed_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_sql_import_custom_result_check_spec.py` & `dqops-1.2.0/dqops/client/models/table_sql_import_custom_result_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_sql_import_custom_result_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/table_sql_import_custom_result_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_statistics_collectors_root_categories_spec.py` & `dqops-1.2.0/dqops/client/models/table_statistics_collectors_root_categories_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_statistics_model.py` & `dqops-1.2.0/dqops/client/models/table_statistics_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_timeliness_daily_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/table_timeliness_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_timeliness_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/table_timeliness_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_timeliness_daily_partitioned_checks_spec.py` & `dqops-1.2.0/dqops/client/models/table_timeliness_daily_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_timeliness_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/table_timeliness_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_timeliness_data_freshness_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/table_timeliness_data_freshness_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_timeliness_data_ingestion_delay_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/table_timeliness_data_ingestion_delay_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_timeliness_data_staleness_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/table_timeliness_data_staleness_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_timeliness_monthly_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/table_timeliness_profiling_checks_spec.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,136 +7,132 @@
 
 if TYPE_CHECKING:
     from ..models.table_data_freshness_check_spec import TableDataFreshnessCheckSpec
     from ..models.table_data_ingestion_delay_check_spec import (
         TableDataIngestionDelayCheckSpec,
     )
     from ..models.table_data_staleness_check_spec import TableDataStalenessCheckSpec
-    from ..models.table_timeliness_monthly_monitoring_checks_spec_custom_checks import (
-        TableTimelinessMonthlyMonitoringChecksSpecCustomChecks,
+    from ..models.table_timeliness_profiling_checks_spec_custom_checks import (
+        TableTimelinessProfilingChecksSpecCustomChecks,
     )
 
 
-T = TypeVar("T", bound="TableTimelinessMonthlyMonitoringChecksSpec")
+T = TypeVar("T", bound="TableTimelinessProfilingChecksSpec")
 
 
 @_attrs_define
-class TableTimelinessMonthlyMonitoringChecksSpec:
+class TableTimelinessProfilingChecksSpec:
     """
     Attributes:
-        custom_checks (Union[Unset, TableTimelinessMonthlyMonitoringChecksSpecCustomChecks]): Dictionary of additional
-            custom checks within this category. The keys are check names defined in the definition section. The sensor
-            parameters and rules should match the type of the configured sensor and rule for the custom check.
-        monthly_data_freshness (Union[Unset, TableDataFreshnessCheckSpec]):
-        monthly_data_staleness (Union[Unset, TableDataStalenessCheckSpec]):
-        monthly_data_ingestion_delay (Union[Unset, TableDataIngestionDelayCheckSpec]):
+        custom_checks (Union[Unset, TableTimelinessProfilingChecksSpecCustomChecks]): Dictionary of additional custom
+            checks within this category. The keys are check names defined in the definition section. The sensor parameters
+            and rules should match the type of the configured sensor and rule for the custom check.
+        profile_data_freshness (Union[Unset, TableDataFreshnessCheckSpec]):
+        profile_data_staleness (Union[Unset, TableDataStalenessCheckSpec]):
+        profile_data_ingestion_delay (Union[Unset, TableDataIngestionDelayCheckSpec]):
     """
 
     custom_checks: Union[
-        Unset, "TableTimelinessMonthlyMonitoringChecksSpecCustomChecks"
+        Unset, "TableTimelinessProfilingChecksSpecCustomChecks"
     ] = UNSET
-    monthly_data_freshness: Union[Unset, "TableDataFreshnessCheckSpec"] = UNSET
-    monthly_data_staleness: Union[Unset, "TableDataStalenessCheckSpec"] = UNSET
-    monthly_data_ingestion_delay: Union[
+    profile_data_freshness: Union[Unset, "TableDataFreshnessCheckSpec"] = UNSET
+    profile_data_staleness: Union[Unset, "TableDataStalenessCheckSpec"] = UNSET
+    profile_data_ingestion_delay: Union[
         Unset, "TableDataIngestionDelayCheckSpec"
     ] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         custom_checks: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.custom_checks, Unset):
             custom_checks = self.custom_checks.to_dict()
 
-        monthly_data_freshness: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.monthly_data_freshness, Unset):
-            monthly_data_freshness = self.monthly_data_freshness.to_dict()
-
-        monthly_data_staleness: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.monthly_data_staleness, Unset):
-            monthly_data_staleness = self.monthly_data_staleness.to_dict()
-
-        monthly_data_ingestion_delay: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.monthly_data_ingestion_delay, Unset):
-            monthly_data_ingestion_delay = self.monthly_data_ingestion_delay.to_dict()
+        profile_data_freshness: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.profile_data_freshness, Unset):
+            profile_data_freshness = self.profile_data_freshness.to_dict()
+
+        profile_data_staleness: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.profile_data_staleness, Unset):
+            profile_data_staleness = self.profile_data_staleness.to_dict()
+
+        profile_data_ingestion_delay: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.profile_data_ingestion_delay, Unset):
+            profile_data_ingestion_delay = self.profile_data_ingestion_delay.to_dict()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if custom_checks is not UNSET:
             field_dict["custom_checks"] = custom_checks
-        if monthly_data_freshness is not UNSET:
-            field_dict["monthly_data_freshness"] = monthly_data_freshness
-        if monthly_data_staleness is not UNSET:
-            field_dict["monthly_data_staleness"] = monthly_data_staleness
-        if monthly_data_ingestion_delay is not UNSET:
-            field_dict["monthly_data_ingestion_delay"] = monthly_data_ingestion_delay
+        if profile_data_freshness is not UNSET:
+            field_dict["profile_data_freshness"] = profile_data_freshness
+        if profile_data_staleness is not UNSET:
+            field_dict["profile_data_staleness"] = profile_data_staleness
+        if profile_data_ingestion_delay is not UNSET:
+            field_dict["profile_data_ingestion_delay"] = profile_data_ingestion_delay
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.table_data_freshness_check_spec import TableDataFreshnessCheckSpec
         from ..models.table_data_ingestion_delay_check_spec import (
             TableDataIngestionDelayCheckSpec,
         )
         from ..models.table_data_staleness_check_spec import TableDataStalenessCheckSpec
-        from ..models.table_timeliness_monthly_monitoring_checks_spec_custom_checks import (
-            TableTimelinessMonthlyMonitoringChecksSpecCustomChecks,
+        from ..models.table_timeliness_profiling_checks_spec_custom_checks import (
+            TableTimelinessProfilingChecksSpecCustomChecks,
         )
 
         d = src_dict.copy()
         _custom_checks = d.pop("custom_checks", UNSET)
-        custom_checks: Union[
-            Unset, TableTimelinessMonthlyMonitoringChecksSpecCustomChecks
-        ]
+        custom_checks: Union[Unset, TableTimelinessProfilingChecksSpecCustomChecks]
         if isinstance(_custom_checks, Unset):
             custom_checks = UNSET
         else:
-            custom_checks = (
-                TableTimelinessMonthlyMonitoringChecksSpecCustomChecks.from_dict(
-                    _custom_checks
-                )
+            custom_checks = TableTimelinessProfilingChecksSpecCustomChecks.from_dict(
+                _custom_checks
             )
 
-        _monthly_data_freshness = d.pop("monthly_data_freshness", UNSET)
-        monthly_data_freshness: Union[Unset, TableDataFreshnessCheckSpec]
-        if isinstance(_monthly_data_freshness, Unset):
-            monthly_data_freshness = UNSET
+        _profile_data_freshness = d.pop("profile_data_freshness", UNSET)
+        profile_data_freshness: Union[Unset, TableDataFreshnessCheckSpec]
+        if isinstance(_profile_data_freshness, Unset):
+            profile_data_freshness = UNSET
         else:
-            monthly_data_freshness = TableDataFreshnessCheckSpec.from_dict(
-                _monthly_data_freshness
+            profile_data_freshness = TableDataFreshnessCheckSpec.from_dict(
+                _profile_data_freshness
             )
 
-        _monthly_data_staleness = d.pop("monthly_data_staleness", UNSET)
-        monthly_data_staleness: Union[Unset, TableDataStalenessCheckSpec]
-        if isinstance(_monthly_data_staleness, Unset):
-            monthly_data_staleness = UNSET
+        _profile_data_staleness = d.pop("profile_data_staleness", UNSET)
+        profile_data_staleness: Union[Unset, TableDataStalenessCheckSpec]
+        if isinstance(_profile_data_staleness, Unset):
+            profile_data_staleness = UNSET
         else:
-            monthly_data_staleness = TableDataStalenessCheckSpec.from_dict(
-                _monthly_data_staleness
+            profile_data_staleness = TableDataStalenessCheckSpec.from_dict(
+                _profile_data_staleness
             )
 
-        _monthly_data_ingestion_delay = d.pop("monthly_data_ingestion_delay", UNSET)
-        monthly_data_ingestion_delay: Union[Unset, TableDataIngestionDelayCheckSpec]
-        if isinstance(_monthly_data_ingestion_delay, Unset):
-            monthly_data_ingestion_delay = UNSET
+        _profile_data_ingestion_delay = d.pop("profile_data_ingestion_delay", UNSET)
+        profile_data_ingestion_delay: Union[Unset, TableDataIngestionDelayCheckSpec]
+        if isinstance(_profile_data_ingestion_delay, Unset):
+            profile_data_ingestion_delay = UNSET
         else:
-            monthly_data_ingestion_delay = TableDataIngestionDelayCheckSpec.from_dict(
-                _monthly_data_ingestion_delay
+            profile_data_ingestion_delay = TableDataIngestionDelayCheckSpec.from_dict(
+                _profile_data_ingestion_delay
             )
 
-        table_timeliness_monthly_monitoring_checks_spec = cls(
+        table_timeliness_profiling_checks_spec = cls(
             custom_checks=custom_checks,
-            monthly_data_freshness=monthly_data_freshness,
-            monthly_data_staleness=monthly_data_staleness,
-            monthly_data_ingestion_delay=monthly_data_ingestion_delay,
+            profile_data_freshness=profile_data_freshness,
+            profile_data_staleness=profile_data_staleness,
+            profile_data_ingestion_delay=profile_data_ingestion_delay,
         )
 
-        table_timeliness_monthly_monitoring_checks_spec.additional_properties = d
-        return table_timeliness_monthly_monitoring_checks_spec
+        table_timeliness_profiling_checks_spec.additional_properties = d
+        return table_timeliness_profiling_checks_spec
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dqops-1.1.0/dqops/client/models/table_timeliness_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/table_timeliness_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_timeliness_monthly_partitioned_checks_spec.py` & `dqops-1.2.0/dqops/client/models/table_timeliness_monthly_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_timeliness_monthly_partitioned_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/table_timeliness_monthly_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_timeliness_partition_reload_lag_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/table_timeliness_partition_reload_lag_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_timeliness_profiling_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/table_timeliness_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_volume_daily_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/table_volume_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_volume_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/table_volume_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_volume_daily_partitioned_checks_spec.py` & `dqops-1.2.0/dqops/client/models/table_volume_daily_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_volume_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/table_volume_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_volume_monthly_monitoring_checks_spec.py` & `dqops-1.2.0/dqops/client/models/table_volume_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_volume_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/table_volume_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_volume_monthly_partitioned_checks_spec.py` & `dqops-1.2.0/dqops/client/models/table_volume_monthly_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_volume_monthly_partitioned_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/table_volume_monthly_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_volume_profiling_checks_spec.py` & `dqops-1.2.0/dqops/client/models/table_volume_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_volume_profiling_checks_spec_custom_checks.py` & `dqops-1.2.0/dqops/client/models/table_volume_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_volume_row_count_sensor_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/table_volume_row_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_volume_row_count_statistics_collector_spec.py` & `dqops-1.2.0/dqops/client/models/table_volume_row_count_statistics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/table_volume_statistics_collectors_spec.py` & `dqops-1.2.0/dqops/client/models/table_volume_statistics_collectors_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/target_column_pattern_spec.py` & `dqops-1.2.0/dqops/client/models/target_column_pattern_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/target_table_pattern_spec.py` & `dqops-1.2.0/dqops/client/models/target_table_pattern_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/temporal_unit.py` & `dqops-1.2.0/dqops/client/models/temporal_unit.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/time_window_filter_parameters.py` & `dqops-1.2.0/dqops/client/models/time_window_filter_parameters.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/timestamp_columns_spec.py` & `dqops-1.2.0/dqops/client/models/timestamp_columns_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/trino_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/trino_parameters_spec.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
-from ..models.athena_authentication_mode import AthenaAuthenticationMode
+from ..models.aws_authentication_mode import AwsAuthenticationMode
 from ..models.trino_engine_type import TrinoEngineType
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
     from ..models.trino_parameters_spec_properties import TrinoParametersSpecProperties
 
 
@@ -23,15 +23,15 @@
             variable.
         port (Union[Unset, str]): Trino port number. The default port is 8080. Supports also a ${TRINO_PORT}
             configuration with a custom environment variable.
         user (Union[Unset, str]): Trino user name. The value can be in the ${ENVIRONMENT_VARIABLE_NAME} format to use
             dynamic substitution.
         password (Union[Unset, str]): Trino database password. The value can be in the ${ENVIRONMENT_VARIABLE_NAME}
             format to use dynamic substitution.
-        athena_authentication_mode (Union[Unset, AthenaAuthenticationMode]):
+        aws_authentication_mode (Union[Unset, AwsAuthenticationMode]):
         athena_region (Union[Unset, str]): The AWS Region where queries will be run. Supports also a ${ATHENA_REGION}
             configuration with a custom environment variable.
         catalog (Union[Unset, str]): The catalog that contains the databases and the tables that will be accessed with
             the driver. Supports also a ${TRINO_CATALOG} configuration with a custom environment variable.
         athena_work_group (Union[Unset, str]): The workgroup in which queries will run. Supports also a
             ${ATHENA_WORK_GROUP} configuration with a custom environment variable.
         athena_output_location (Union[Unset, str]): The location in Amazon S3 where query results will be stored.
@@ -42,15 +42,15 @@
     """
 
     trino_engine_type: Union[Unset, TrinoEngineType] = UNSET
     host: Union[Unset, str] = UNSET
     port: Union[Unset, str] = UNSET
     user: Union[Unset, str] = UNSET
     password: Union[Unset, str] = UNSET
-    athena_authentication_mode: Union[Unset, AthenaAuthenticationMode] = UNSET
+    aws_authentication_mode: Union[Unset, AwsAuthenticationMode] = UNSET
     athena_region: Union[Unset, str] = UNSET
     catalog: Union[Unset, str] = UNSET
     athena_work_group: Union[Unset, str] = UNSET
     athena_output_location: Union[Unset, str] = UNSET
     properties: Union[Unset, "TrinoParametersSpecProperties"] = UNSET
     database: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
@@ -60,17 +60,17 @@
         if not isinstance(self.trino_engine_type, Unset):
             trino_engine_type = self.trino_engine_type.value
 
         host = self.host
         port = self.port
         user = self.user
         password = self.password
-        athena_authentication_mode: Union[Unset, str] = UNSET
-        if not isinstance(self.athena_authentication_mode, Unset):
-            athena_authentication_mode = self.athena_authentication_mode.value
+        aws_authentication_mode: Union[Unset, str] = UNSET
+        if not isinstance(self.aws_authentication_mode, Unset):
+            aws_authentication_mode = self.aws_authentication_mode.value
 
         athena_region = self.athena_region
         catalog = self.catalog
         athena_work_group = self.athena_work_group
         athena_output_location = self.athena_output_location
         properties: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.properties, Unset):
@@ -87,16 +87,16 @@
             field_dict["host"] = host
         if port is not UNSET:
             field_dict["port"] = port
         if user is not UNSET:
             field_dict["user"] = user
         if password is not UNSET:
             field_dict["password"] = password
-        if athena_authentication_mode is not UNSET:
-            field_dict["athena_authentication_mode"] = athena_authentication_mode
+        if aws_authentication_mode is not UNSET:
+            field_dict["aws_authentication_mode"] = aws_authentication_mode
         if athena_region is not UNSET:
             field_dict["athena_region"] = athena_region
         if catalog is not UNSET:
             field_dict["catalog"] = catalog
         if athena_work_group is not UNSET:
             field_dict["athena_work_group"] = athena_work_group
         if athena_output_location is not UNSET:
@@ -126,22 +126,20 @@
 
         port = d.pop("port", UNSET)
 
         user = d.pop("user", UNSET)
 
         password = d.pop("password", UNSET)
 
-        _athena_authentication_mode = d.pop("athena_authentication_mode", UNSET)
-        athena_authentication_mode: Union[Unset, AthenaAuthenticationMode]
-        if isinstance(_athena_authentication_mode, Unset):
-            athena_authentication_mode = UNSET
+        _aws_authentication_mode = d.pop("aws_authentication_mode", UNSET)
+        aws_authentication_mode: Union[Unset, AwsAuthenticationMode]
+        if isinstance(_aws_authentication_mode, Unset):
+            aws_authentication_mode = UNSET
         else:
-            athena_authentication_mode = AthenaAuthenticationMode(
-                _athena_authentication_mode
-            )
+            aws_authentication_mode = AwsAuthenticationMode(_aws_authentication_mode)
 
         athena_region = d.pop("athena_region", UNSET)
 
         catalog = d.pop("catalog", UNSET)
 
         athena_work_group = d.pop("athena_work_group", UNSET)
 
@@ -158,15 +156,15 @@
 
         trino_parameters_spec = cls(
             trino_engine_type=trino_engine_type,
             host=host,
             port=port,
             user=user,
             password=password,
-            athena_authentication_mode=athena_authentication_mode,
+            aws_authentication_mode=aws_authentication_mode,
             athena_region=athena_region,
             catalog=catalog,
             athena_work_group=athena_work_group,
             athena_output_location=athena_output_location,
             properties=properties,
             database=database,
         )
```

### Comparing `dqops-1.1.0/dqops/client/models/trino_parameters_spec_properties.py` & `dqops-1.2.0/dqops/client/models/trino_parameters_spec_properties.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/models/value_changed_rule_parameters_spec.py` & `dqops-1.2.0/dqops/client/models/value_changed_rule_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/client/types.py` & `dqops-1.2.0/dqops/client/types.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/install.py` & `dqops-1.2.0/dqops/install.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/startdqo.py` & `dqops-1.2.0/dqops/startdqo.py`

 * *Files identical despite different names*

### Comparing `dqops-1.1.0/dqops/version.py` & `dqops-1.2.0/dqops/version.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limit
 
 # WARNING: the next two lines with the version numbers (VERSION =, PIP_VERSION =) should not be modified manually. They are changed by a maven profile at compile time.
-VERSION = "1.1.0"
-PIP_VERSION = "1.1.0"
+VERSION = "1.2.0"
+PIP_VERSION = "1.2.0"
 GITHUB_RELEASE = "v" + VERSION + ""
 JAVA_VERSION = "17"
 
 
 def get_dqo_version():
     return VERSION, PIP_VERSION, GITHUB_RELEASE, JAVA_VERSION
```

### Comparing `dqops-1.1.0/dqops.egg-info/PKG-INFO` & `dqops-1.2.0/dqops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dqops
-Version: 1.1.0
+Version: 1.2.0
 Summary: DQOps Data Quality Operations Center
 Home-page: https://github.com/dqops/dqo/tree/master/distribution/python
 Author: DQOps Developers
 Author-email: support@dqops.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `dqops-1.1.0/dqops.egg-info/SOURCES.txt` & `dqops-1.2.0/dqops.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -202,14 +202,18 @@
 dqops/client/api/jobs/is_cron_scheduler_running.py
 dqops/client/api/jobs/run_checks.py
 dqops/client/api/jobs/start_cron_scheduler.py
 dqops/client/api/jobs/stop_cron_scheduler.py
 dqops/client/api/jobs/synchronize_folders.py
 dqops/client/api/jobs/wait_for_job.py
 dqops/client/api/jobs/wait_for_run_checks_job.py
+dqops/client/api/labels/__init__.py
+dqops/client/api/labels/get_all_labels_for_columns.py
+dqops/client/api/labels/get_all_labels_for_connections.py
+dqops/client/api/labels/get_all_labels_for_tables.py
 dqops/client/api/log_shipping/__init__.py
 dqops/client/api/log_shipping/log_debug.py
 dqops/client/api/log_shipping/log_error.py
 dqops/client/api/log_shipping/log_info.py
 dqops/client/api/log_shipping/log_warn.py
 dqops/client/api/rules/__init__.py
 dqops/client/api/rules/create_rule.py
@@ -222,14 +226,16 @@
 dqops/client/api/schemas/get_schema_monitoring_checks_model.py
 dqops/client/api/schemas/get_schema_monitoring_checks_templates.py
 dqops/client/api/schemas/get_schema_partitioned_checks_model.py
 dqops/client/api/schemas/get_schema_partitioned_checks_templates.py
 dqops/client/api/schemas/get_schema_profiling_checks_model.py
 dqops/client/api/schemas/get_schema_profiling_checks_templates.py
 dqops/client/api/schemas/get_schemas.py
+dqops/client/api/search/__init__.py
+dqops/client/api/search/find_tables.py
 dqops/client/api/sensor_readouts/__init__.py
 dqops/client/api/sensor_readouts/get_column_monitoring_sensor_readouts.py
 dqops/client/api/sensor_readouts/get_column_partitioned_sensor_readouts.py
 dqops/client/api/sensor_readouts/get_column_profiling_sensor_readouts.py
 dqops/client/api/sensor_readouts/get_table_monitoring_sensor_readouts.py
 dqops/client/api/sensor_readouts/get_table_partitioned_sensor_readouts.py
 dqops/client/api/sensor_readouts/get_table_profiling_sensor_readouts.py
@@ -336,16 +342,16 @@
 dqops/client/models/all_checks_patch_parameters_selected_tables_to_columns.py
 dqops/client/models/anomaly_differencing_percentile_moving_average_rule_error_05_pct_parameters_spec.py
 dqops/client/models/anomaly_differencing_percentile_moving_average_rule_fatal_01_pct_parameters_spec.py
 dqops/client/models/anomaly_differencing_percentile_moving_average_rule_warning_1_pct_parameters_spec.py
 dqops/client/models/anomaly_stationary_percentile_moving_average_rule_error_05_pct_parameters_spec.py
 dqops/client/models/anomaly_stationary_percentile_moving_average_rule_fatal_01_pct_parameters_spec.py
 dqops/client/models/anomaly_stationary_percentile_moving_average_rule_warning_1_pct_parameters_spec.py
-dqops/client/models/athena_authentication_mode.py
 dqops/client/models/authenticated_dashboard_model.py
+dqops/client/models/aws_authentication_mode.py
 dqops/client/models/between_floats_rule_parameters_spec.py
 dqops/client/models/between_ints_rule_parameters_spec.py
 dqops/client/models/between_percent_rule_parameters_spec.py
 dqops/client/models/big_query_authentication_mode.py
 dqops/client/models/big_query_jobs_create_project.py
 dqops/client/models/big_query_parameters_spec.py
 dqops/client/models/bulk_check_deactivate_parameters.py
@@ -462,14 +468,15 @@
 dqops/client/models/column_conversions_monthly_monitoring_checks_spec_custom_checks.py
 dqops/client/models/column_conversions_monthly_partitioned_checks_spec.py
 dqops/client/models/column_conversions_monthly_partitioned_checks_spec_custom_checks.py
 dqops/client/models/column_conversions_profiling_checks_spec.py
 dqops/client/models/column_conversions_profiling_checks_spec_custom_checks.py
 dqops/client/models/column_current_data_quality_status_model.py
 dqops/client/models/column_current_data_quality_status_model_checks.py
+dqops/client/models/column_current_data_quality_status_model_dimensions.py
 dqops/client/models/column_custom_sql_daily_monitoring_checks_spec.py
 dqops/client/models/column_custom_sql_daily_monitoring_checks_spec_custom_checks.py
 dqops/client/models/column_custom_sql_daily_partitioned_checks_spec.py
 dqops/client/models/column_custom_sql_daily_partitioned_checks_spec_custom_checks.py
 dqops/client/models/column_custom_sql_monthly_monitoring_checks_spec.py
 dqops/client/models/column_custom_sql_monthly_monitoring_checks_spec_custom_checks.py
 dqops/client/models/column_custom_sql_monthly_partitioned_checks_spec.py
@@ -541,14 +548,15 @@
 dqops/client/models/column_integrity_monthly_monitoring_checks_spec.py
 dqops/client/models/column_integrity_monthly_monitoring_checks_spec_custom_checks.py
 dqops/client/models/column_integrity_monthly_partitioned_checks_spec.py
 dqops/client/models/column_integrity_monthly_partitioned_checks_spec_custom_checks.py
 dqops/client/models/column_integrity_profiling_checks_spec.py
 dqops/client/models/column_integrity_profiling_checks_spec_custom_checks.py
 dqops/client/models/column_invalid_email_format_found_check_spec.py
+dqops/client/models/column_invalid_email_format_percent_check_spec.py
 dqops/client/models/column_invalid_ip_4_address_format_found_check_spec.py
 dqops/client/models/column_invalid_ip_6_address_format_found_check_spec.py
 dqops/client/models/column_invalid_latitude_count_check_spec.py
 dqops/client/models/column_invalid_longitude_count_check_spec.py
 dqops/client/models/column_invalid_uuid_format_found_check_spec.py
 dqops/client/models/column_list_model.py
 dqops/client/models/column_max_anomaly_differencing_check_spec.py
@@ -657,14 +665,15 @@
 dqops/client/models/column_numeric_valid_longitude_percent_sensor_parameters_spec.py
 dqops/client/models/column_partitioned_check_categories_spec.py
 dqops/client/models/column_patterns_daily_monitoring_checks_spec.py
 dqops/client/models/column_patterns_daily_monitoring_checks_spec_custom_checks.py
 dqops/client/models/column_patterns_daily_partitioned_checks_spec.py
 dqops/client/models/column_patterns_daily_partitioned_checks_spec_custom_checks.py
 dqops/client/models/column_patterns_invalid_email_format_count_sensor_parameters_spec.py
+dqops/client/models/column_patterns_invalid_email_format_percent_sensor_parameters_spec.py
 dqops/client/models/column_patterns_invalid_ip_4_address_format_count_sensor_parameters_spec.py
 dqops/client/models/column_patterns_invalid_ip_6_address_format_count_sensor_parameters_spec.py
 dqops/client/models/column_patterns_invalid_uuid_format_count_sensor_parameters_spec.py
 dqops/client/models/column_patterns_monthly_monitoring_checks_spec.py
 dqops/client/models/column_patterns_monthly_monitoring_checks_spec_custom_checks.py
 dqops/client/models/column_patterns_monthly_partitioned_checks_spec.py
 dqops/client/models/column_patterns_monthly_partitioned_checks_spec_custom_checks.py
@@ -887,14 +896,15 @@
 dqops/client/models/default_table_checks_pattern_model.py
 dqops/client/models/delete_stored_data_queue_job_parameters.py
 dqops/client/models/delete_stored_data_queue_job_result.py
 dqops/client/models/delete_stored_data_result.py
 dqops/client/models/delete_stored_data_result_partition_results.py
 dqops/client/models/detected_datatype_category.py
 dqops/client/models/detected_datatype_equals_rule_parameters_spec.py
+dqops/client/models/dimension_current_data_quality_status_model.py
 dqops/client/models/display_hint.py
 dqops/client/models/dqo_cloud_user_model.py
 dqops/client/models/dqo_job_change_model.py
 dqops/client/models/dqo_job_entry_parameters_model.py
 dqops/client/models/dqo_job_history_entry_model.py
 dqops/client/models/dqo_job_queue_incremental_snapshot_model.py
 dqops/client/models/dqo_job_queue_initial_snapshot_model.py
@@ -943,14 +953,15 @@
 dqops/client/models/incident_sort_order.py
 dqops/client/models/incident_status.py
 dqops/client/models/incident_webhook_notifications_spec.py
 dqops/client/models/incidents_per_connection_model.py
 dqops/client/models/json_file_format_spec.py
 dqops/client/models/json_format_type.py
 dqops/client/models/json_records_type.py
+dqops/client/models/label_model.py
 dqops/client/models/max_count_rule_0_error_parameters_spec.py
 dqops/client/models/max_count_rule_0_warning_parameters_spec.py
 dqops/client/models/max_count_rule_100_parameters_spec.py
 dqops/client/models/max_days_rule_1_parameters_spec.py
 dqops/client/models/max_days_rule_2_parameters_spec.py
 dqops/client/models/max_days_rule_7_parameters_spec.py
 dqops/client/models/max_diff_percent_rule_0_parameters_spec.py
@@ -999,14 +1010,15 @@
 dqops/client/models/provider_sensor_definition_spec.py
 dqops/client/models/provider_sensor_definition_spec_parameters.py
 dqops/client/models/provider_sensor_list_model.py
 dqops/client/models/provider_sensor_model.py
 dqops/client/models/provider_sensor_runner_type.py
 dqops/client/models/provider_type.py
 dqops/client/models/quality_category_model.py
+dqops/client/models/redshift_authentication_mode.py
 dqops/client/models/redshift_parameters_spec.py
 dqops/client/models/redshift_parameters_spec_properties.py
 dqops/client/models/remote_table_list_model.py
 dqops/client/models/repair_stored_data_queue_job_parameters.py
 dqops/client/models/rule_folder_model.py
 dqops/client/models/rule_folder_model_folders.py
 dqops/client/models/rule_list_model.py
@@ -1099,14 +1111,15 @@
 dqops/client/models/table_comparison_results_model.py
 dqops/client/models/table_comparison_results_model_column_comparison_results.py
 dqops/client/models/table_comparison_results_model_table_comparison_results.py
 dqops/client/models/table_comparison_row_count_match_check_spec.py
 dqops/client/models/table_current_data_quality_status_model.py
 dqops/client/models/table_current_data_quality_status_model_checks.py
 dqops/client/models/table_current_data_quality_status_model_columns.py
+dqops/client/models/table_current_data_quality_status_model_dimensions.py
 dqops/client/models/table_custom_sql_daily_monitoring_checks_spec.py
 dqops/client/models/table_custom_sql_daily_monitoring_checks_spec_custom_checks.py
 dqops/client/models/table_custom_sql_daily_partitioned_checks_spec.py
 dqops/client/models/table_custom_sql_daily_partitioned_checks_spec_custom_checks.py
 dqops/client/models/table_custom_sql_monthly_monitoring_checks_spec.py
 dqops/client/models/table_custom_sql_monthly_monitoring_checks_spec_custom_checks.py
 dqops/client/models/table_custom_sql_monthly_partitioned_checks_spec.py
```

### Comparing `dqops-1.1.0/setup.py` & `dqops-1.2.0/setup.py`

 * *Files identical despite different names*

