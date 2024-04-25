# Comparing `tmp/dlt-0.4.9a1.tar.gz` & `tmp/dlt-0.4.9a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlt-0.4.9a1.tar", max compression
+gzip compressed data, was "dlt-0.4.9a2.tar", max compression
```

## Comparing `dlt-0.4.9a1.tar` & `dlt-0.4.9a2.tar`

### file list

```diff
@@ -1,348 +1,348 @@
--rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 dlt-0.4.9a1/LICENSE.txt
--rw-r--r--   0        0        0     5298 2024-04-15 15:36:23.382155 dlt-0.4.9a1/README.md
--rw-r--r--   0        0        0     2229 2024-04-07 14:59:43.705656 dlt-0.4.9a1/dlt/__init__.py
--rw-r--r--   0        0        0       69 2024-03-08 19:36:32.659855 dlt-0.4.9a1/dlt/__main__.py
--rw-r--r--   0        0        0        0 2023-11-18 17:38:04.257189 dlt-0.4.9a1/dlt/cli/__init__.py
--rw-r--r--   0        0        0    21512 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/cli/_dlt.py
--rw-r--r--   0        0        0     4187 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/cli/config_toml_writer.py
--rw-r--r--   0        0        0    18229 2024-01-24 17:23:08.476518 dlt-0.4.9a1/dlt/cli/deploy_command.py
--rw-r--r--   0        0        0    16912 2024-04-13 11:38:43.050742 dlt-0.4.9a1/dlt/cli/deploy_command_helpers.py
--rw-r--r--   0        0        0     1944 2024-01-25 20:07:33.363195 dlt-0.4.9a1/dlt/cli/echo.py
--rw-r--r--   0        0        0      435 2023-11-18 17:38:04.257189 dlt-0.4.9a1/dlt/cli/exceptions.py
--rw-r--r--   0        0        0    21105 2024-04-13 11:38:33.320742 dlt-0.4.9a1/dlt/cli/init_command.py
--rw-r--r--   0        0        0    14157 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/cli/pipeline_command.py
--rw-r--r--   0        0        0    10152 2024-04-13 11:38:50.650742 dlt-0.4.9a1/dlt/cli/pipeline_files.py
--rw-r--r--   0        0        0     2524 2024-01-24 17:23:08.476518 dlt-0.4.9a1/dlt/cli/requirements.py
--rw-r--r--   0        0        0     4895 2024-01-24 17:23:08.476518 dlt-0.4.9a1/dlt/cli/source_detection.py
--rw-r--r--   0        0        0     1912 2024-01-24 17:23:08.476518 dlt-0.4.9a1/dlt/cli/telemetry_command.py
--rw-r--r--   0        0        0     1999 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/cli/utils.py
--rw-r--r--   0        0        0      292 2024-04-09 13:29:46.170457 dlt-0.4.9a1/dlt/common/__init__.py
--rw-r--r--   0        0        0     1311 2024-01-24 17:23:08.476518 dlt-0.4.9a1/dlt/common/arithmetics.py
--rw-r--r--   0        0        0      808 2024-04-07 14:59:43.705656 dlt-0.4.9a1/dlt/common/configuration/__init__.py
--rw-r--r--   0        0        0     5144 2024-01-24 17:23:08.476518 dlt-0.4.9a1/dlt/common/configuration/accessors.py
--rw-r--r--   0        0        0     7410 2024-04-07 14:59:43.705656 dlt-0.4.9a1/dlt/common/configuration/container.py
--rw-r--r--   0        0        0     8457 2024-01-24 17:23:08.486518 dlt-0.4.9a1/dlt/common/configuration/exceptions.py
--rw-r--r--   0        0        0    11848 2024-04-13 11:29:48.720735 dlt-0.4.9a1/dlt/common/configuration/inject.py
--rw-r--r--   0        0        0     1777 2024-01-25 20:07:33.363195 dlt-0.4.9a1/dlt/common/configuration/paths.py
--rw-r--r--   0        0        0      682 2024-01-24 17:23:08.486518 dlt-0.4.9a1/dlt/common/configuration/providers/__init__.py
--rw-r--r--   0        0        0      805 2024-03-05 18:21:35.930419 dlt-0.4.9a1/dlt/common/configuration/providers/airflow.py
--rw-r--r--   0        0        0     1129 2024-01-24 17:23:08.486518 dlt-0.4.9a1/dlt/common/configuration/providers/context.py
--rw-r--r--   0        0        0     1346 2024-01-24 17:23:08.486518 dlt-0.4.9a1/dlt/common/configuration/providers/dictionary.py
--rw-r--r--   0        0        0     1995 2024-01-24 17:23:08.486518 dlt-0.4.9a1/dlt/common/configuration/providers/environ.py
--rw-r--r--   0        0        0     5141 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/configuration/providers/google_secrets.py
--rw-r--r--   0        0        0     1319 2024-01-24 17:23:08.486518 dlt-0.4.9a1/dlt/common/configuration/providers/provider.py
--rw-r--r--   0        0        0    13416 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/configuration/providers/toml.py
--rw-r--r--   0        0        0    20983 2024-04-09 13:29:46.170457 dlt-0.4.9a1/dlt/common/configuration/resolve.py
--rw-r--r--   0        0        0     1742 2024-01-24 17:23:08.486518 dlt-0.4.9a1/dlt/common/configuration/specs/__init__.py
--rw-r--r--   0        0        0     1836 2024-04-09 13:29:46.170457 dlt-0.4.9a1/dlt/common/configuration/specs/api_credentials.py
--rw-r--r--   0        0        0     5263 2024-04-09 13:29:46.170457 dlt-0.4.9a1/dlt/common/configuration/specs/aws_credentials.py
--rw-r--r--   0        0        0     2591 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/configuration/specs/azure_credentials.py
--rw-r--r--   0        0        0    18147 2024-04-11 11:44:50.568746 dlt-0.4.9a1/dlt/common/configuration/specs/base_configuration.py
--rw-r--r--   0        0        0     6498 2024-04-09 13:29:46.170457 dlt-0.4.9a1/dlt/common/configuration/specs/config_providers_context.py
--rw-r--r--   0        0        0     3456 2024-04-09 13:29:46.170457 dlt-0.4.9a1/dlt/common/configuration/specs/config_section_context.py
--rw-r--r--   0        0        0     2339 2024-04-09 13:29:46.170457 dlt-0.4.9a1/dlt/common/configuration/specs/connection_string_credentials.py
--rw-r--r--   0        0        0     2667 2024-01-24 17:23:08.486518 dlt-0.4.9a1/dlt/common/configuration/specs/exceptions.py
--rw-r--r--   0        0        0    13349 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/configuration/specs/gcp_credentials.py
--rw-r--r--   0        0        0      874 2024-04-09 13:29:46.170457 dlt-0.4.9a1/dlt/common/configuration/specs/known_sections.py
--rw-r--r--   0        0        0     2856 2024-04-09 13:29:46.170457 dlt-0.4.9a1/dlt/common/configuration/specs/run_configuration.py
--rw-r--r--   0        0        0     6650 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/configuration/utils.py
--rw-r--r--   0        0        0      220 2024-01-24 17:23:08.486518 dlt-0.4.9a1/dlt/common/data_types/__init__.py
--rw-r--r--   0        0        0     6832 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/data_types/type_helpers.py
--rw-r--r--   0        0        0      269 2024-01-24 17:23:08.486518 dlt-0.4.9a1/dlt/common/data_types/typing.py
--rw-r--r--   0        0        0      754 2024-04-16 09:06:12.375886 dlt-0.4.9a1/dlt/common/data_writers/__init__.py
--rw-r--r--   0        0        0    10766 2024-04-16 09:06:12.375886 dlt-0.4.9a1/dlt/common/data_writers/buffered.py
--rw-r--r--   0        0        0     5665 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/data_writers/escape.py
--rw-r--r--   0        0        0     2894 2024-04-16 09:06:12.375886 dlt-0.4.9a1/dlt/common/data_writers/exceptions.py
--rw-r--r--   0        0        0    27064 2024-04-16 09:06:12.375886 dlt-0.4.9a1/dlt/common/data_writers/writers.py
--rw-r--r--   0        0        0      483 2024-04-16 09:06:12.375886 dlt-0.4.9a1/dlt/common/destination/__init__.py
--rw-r--r--   0        0        0     5375 2024-04-16 09:06:12.375886 dlt-0.4.9a1/dlt/common/destination/capabilities.py
--rw-r--r--   0        0        0     5132 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/common/destination/exceptions.py
--rw-r--r--   0        0        0    25485 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/destination/reference.py
--rw-r--r--   0        0        0     6274 2024-04-09 13:29:46.180457 dlt-0.4.9a1/dlt/common/exceptions.py
--rw-r--r--   0        0        0     5149 2024-01-24 17:23:08.496518 dlt-0.4.9a1/dlt/common/git.py
--rw-r--r--   0        0        0     7099 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/json/__init__.py
--rw-r--r--   0        0        0     1814 2024-02-16 18:38:47.332466 dlt-0.4.9a1/dlt/common/json/_orjson.py
--rw-r--r--   0        0        0     2948 2024-01-24 17:23:08.496518 dlt-0.4.9a1/dlt/common/json/_simplejson.py
--rw-r--r--   0        0        0     1562 2023-11-18 17:38:04.257189 dlt-0.4.9a1/dlt/common/jsonpath.py
--rw-r--r--   0        0        0        0 2023-11-18 17:38:04.257189 dlt-0.4.9a1/dlt/common/libs/__init__.py
--rw-r--r--   0        0        0      181 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/libs/numpy.py
--rw-r--r--   0        0        0      436 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/libs/pandas.py
--rw-r--r--   0        0        0      217 2024-04-07 14:59:43.715656 dlt-0.4.9a1/dlt/common/libs/pandas_sql.py
--rw-r--r--   0        0        0    14934 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/libs/pyarrow.py
--rw-r--r--   0        0        0    15624 2024-02-27 21:03:24.137544 dlt-0.4.9a1/dlt/common/libs/pydantic.py
--rw-r--r--   0        0        0    15486 2024-03-08 19:36:32.669855 dlt-0.4.9a1/dlt/common/libs/sql_alchemy.py
--rw-r--r--   0        0        0     3652 2024-04-09 13:29:46.180457 dlt-0.4.9a1/dlt/common/logger.py
--rw-r--r--   0        0        0      854 2024-03-01 09:52:05.856761 dlt-0.4.9a1/dlt/common/managed_thread_pool.py
--rw-r--r--   0        0        0      384 2024-03-18 14:01:48.098768 dlt-0.4.9a1/dlt/common/normalizers/__init__.py
--rw-r--r--   0        0        0     1408 2024-04-09 13:29:46.180457 dlt-0.4.9a1/dlt/common/normalizers/configuration.py
--rw-r--r--   0        0        0      510 2024-01-24 17:23:08.496518 dlt-0.4.9a1/dlt/common/normalizers/exceptions.py
--rw-r--r--   0        0        0     1905 2024-01-24 17:23:08.496518 dlt-0.4.9a1/dlt/common/normalizers/json/__init__.py
--rw-r--r--   0        0        0    16970 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/normalizers/json/relational.py
--rw-r--r--   0        0        0      123 2024-03-18 14:01:48.098768 dlt-0.4.9a1/dlt/common/normalizers/naming/__init__.py
--rw-r--r--   0        0        0      810 2024-02-27 21:03:24.137544 dlt-0.4.9a1/dlt/common/normalizers/naming/direct.py
--rw-r--r--   0        0        0      798 2024-01-24 17:23:08.496518 dlt-0.4.9a1/dlt/common/normalizers/naming/duck_case.py
--rw-r--r--   0        0        0      830 2024-03-18 14:01:48.098768 dlt-0.4.9a1/dlt/common/normalizers/naming/exceptions.py
--rw-r--r--   0        0        0     4570 2024-03-18 14:01:48.098768 dlt-0.4.9a1/dlt/common/normalizers/naming/naming.py
--rw-r--r--   0        0        0     2967 2024-01-24 17:23:08.496518 dlt-0.4.9a1/dlt/common/normalizers/naming/snake_case.py
--rw-r--r--   0        0        0      359 2024-03-18 14:01:48.108768 dlt-0.4.9a1/dlt/common/normalizers/typing.py
--rw-r--r--   0        0        0     3426 2024-04-07 14:59:43.715656 dlt-0.4.9a1/dlt/common/normalizers/utils.py
--rw-r--r--   0        0        0      461 2024-02-27 21:03:24.137544 dlt-0.4.9a1/dlt/common/pendulum.py
--rw-r--r--   0        0        0    31127 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/pipeline.py
--rw-r--r--   0        0        0        0 2023-11-18 17:38:04.267189 dlt-0.4.9a1/dlt/common/reflection/__init__.py
--rw-r--r--   0        0        0      375 2024-01-24 17:23:08.496518 dlt-0.4.9a1/dlt/common/reflection/function_visitor.py
--rw-r--r--   0        0        0     6119 2024-04-07 14:59:43.715656 dlt-0.4.9a1/dlt/common/reflection/spec.py
--rw-r--r--   0        0        0     5103 2024-01-24 17:23:08.496518 dlt-0.4.9a1/dlt/common/reflection/utils.py
--rw-r--r--   0        0        0      329 2024-01-24 17:23:08.496518 dlt-0.4.9a1/dlt/common/runners/__init__.py
--rw-r--r--   0        0        0      665 2024-04-09 13:29:46.180457 dlt-0.4.9a1/dlt/common/runners/configuration.py
--rw-r--r--   0        0        0     3678 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/runners/pool_runner.py
--rw-r--r--   0        0        0     4132 2024-01-24 17:23:08.496518 dlt-0.4.9a1/dlt/common/runners/runnable.py
--rw-r--r--   0        0        0     3162 2024-01-24 17:23:08.496518 dlt-0.4.9a1/dlt/common/runners/stdout.py
--rw-r--r--   0        0        0     2137 2024-01-24 17:23:08.496518 dlt-0.4.9a1/dlt/common/runners/synth_pickle.py
--rw-r--r--   0        0        0      105 2023-11-18 17:38:04.267189 dlt-0.4.9a1/dlt/common/runners/typing.py
--rw-r--r--   0        0        0     5583 2024-01-24 17:23:08.496518 dlt-0.4.9a1/dlt/common/runners/venv.py
--rw-r--r--   0        0        0       71 2023-11-18 17:38:04.267189 dlt-0.4.9a1/dlt/common/runtime/__init__.py
--rw-r--r--   0        0        0    14599 2024-04-13 11:30:10.760740 dlt-0.4.9a1/dlt/common/runtime/collector.py
--rw-r--r--   0        0        0     5461 2024-01-25 20:07:33.363195 dlt-0.4.9a1/dlt/common/runtime/exec_info.py
--rw-r--r--   0        0        0     1067 2024-04-13 11:30:15.860741 dlt-0.4.9a1/dlt/common/runtime/init.py
--rw-r--r--   0        0        0     6616 2024-01-24 17:23:08.496518 dlt-0.4.9a1/dlt/common/runtime/json_logging.py
--rw-r--r--   0        0        0     2044 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/runtime/prometheus.py
--rw-r--r--   0        0        0     6702 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/runtime/segment.py
--rw-r--r--   0        0        0     2784 2024-01-24 17:23:08.496518 dlt-0.4.9a1/dlt/common/runtime/sentry.py
--rw-r--r--   0        0        0     1938 2024-04-13 11:30:29.100742 dlt-0.4.9a1/dlt/common/runtime/signals.py
--rw-r--r--   0        0        0      613 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/runtime/slack.py
--rw-r--r--   0        0        0     2960 2024-01-24 17:23:08.496518 dlt-0.4.9a1/dlt/common/runtime/telemetry.py
--rw-r--r--   0        0        0      579 2024-01-24 17:23:08.496518 dlt-0.4.9a1/dlt/common/runtime/typing.py
--rw-r--r--   0        0        0      805 2024-01-24 17:23:08.496518 dlt-0.4.9a1/dlt/common/schema/__init__.py
--rw-r--r--   0        0        0     2454 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/schema/detections.py
--rw-r--r--   0        0        0     5308 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/schema/exceptions.py
--rw-r--r--   0        0        0     5269 2024-03-18 14:01:48.108768 dlt-0.4.9a1/dlt/common/schema/migrations.py
--rw-r--r--   0        0        0    42497 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/schema/schema.py
--rw-r--r--   0        0        0     5865 2024-04-15 15:36:23.392155 dlt-0.4.9a1/dlt/common/schema/typing.py
--rw-r--r--   0        0        0    28875 2024-04-15 15:36:23.392155 dlt-0.4.9a1/dlt/common/schema/utils.py
--rw-r--r--   0        0        0     1672 2024-02-10 23:59:00.181729 dlt-0.4.9a1/dlt/common/source.py
--rw-r--r--   0        0        0     1224 2024-04-15 15:36:23.392155 dlt-0.4.9a1/dlt/common/storages/__init__.py
--rw-r--r--   0        0        0     4869 2024-04-09 13:29:46.180457 dlt-0.4.9a1/dlt/common/storages/configuration.py
--rw-r--r--   0        0        0     4175 2024-04-16 09:06:12.375886 dlt-0.4.9a1/dlt/common/storages/data_item_storage.py
--rw-r--r--   0        0        0     4184 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/common/storages/exceptions.py
--rw-r--r--   0        0        0    14242 2024-01-24 17:23:08.506518 dlt-0.4.9a1/dlt/common/storages/file_storage.py
--rw-r--r--   0        0        0    11065 2024-04-15 15:36:23.392155 dlt-0.4.9a1/dlt/common/storages/fsspec_filesystem.py
--rw-r--r--   0        0        0        0 2024-02-26 22:08:47.270507 dlt-0.4.9a1/dlt/common/storages/fsspecs/__init__.py
--rw-r--r--   0        0        0    20479 2024-04-15 15:36:23.392155 dlt-0.4.9a1/dlt/common/storages/fsspecs/google_drive.py
--rw-r--r--   0        0        0     3513 2024-04-09 13:29:46.180457 dlt-0.4.9a1/dlt/common/storages/live_schema_storage.py
--rw-r--r--   0        0        0    26784 2024-04-15 15:36:23.392155 dlt-0.4.9a1/dlt/common/storages/load_package.py
--rw-r--r--   0        0        0     9920 2024-04-16 09:06:12.375886 dlt-0.4.9a1/dlt/common/storages/load_storage.py
--rw-r--r--   0        0        0     3197 2024-04-07 14:59:43.715656 dlt-0.4.9a1/dlt/common/storages/normalize_storage.py
--rw-r--r--   0        0        0     9551 2024-04-15 17:18:10.812104 dlt-0.4.9a1/dlt/common/storages/schema_storage.py
--rw-r--r--   0        0        0     9065 2024-01-24 17:23:08.506518 dlt-0.4.9a1/dlt/common/storages/transactional_file.py
--rw-r--r--   0        0        0     2867 2024-01-24 17:23:08.506518 dlt-0.4.9a1/dlt/common/storages/versioned_storage.py
--rw-r--r--   0        0        0     7604 2024-04-15 15:36:23.392155 dlt-0.4.9a1/dlt/common/time.py
--rw-r--r--   0        0        0     8878 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/common/typing.py
--rw-r--r--   0        0        0    19596 2024-04-15 15:36:23.392155 dlt-0.4.9a1/dlt/common/utils.py
--rw-r--r--   0        0        0     7978 2024-04-07 14:59:43.715656 dlt-0.4.9a1/dlt/common/validation.py
--rw-r--r--   0        0        0     2369 2024-04-15 15:36:23.392155 dlt-0.4.9a1/dlt/common/versioned_state.py
--rw-r--r--   0        0        0     5528 2024-01-24 17:23:08.506518 dlt-0.4.9a1/dlt/common/warnings.py
--rw-r--r--   0        0        0     1219 2024-01-24 17:23:08.506518 dlt-0.4.9a1/dlt/common/wei.py
--rw-r--r--   0        0        0     1217 2024-04-11 11:44:50.568746 dlt-0.4.9a1/dlt/destinations/__init__.py
--rw-r--r--   0        0        0      404 2024-02-27 21:03:24.137544 dlt-0.4.9a1/dlt/destinations/adapters.py
--rw-r--r--   0        0        0     4856 2024-04-15 15:36:23.392155 dlt-0.4.9a1/dlt/destinations/decorators.py
--rw-r--r--   0        0        0     6070 2024-04-16 09:06:12.375886 dlt-0.4.9a1/dlt/destinations/exceptions.py
--rw-r--r--   0        0        0        0 2024-01-24 17:23:08.506518 dlt-0.4.9a1/dlt/destinations/impl/__init__.py
--rw-r--r--   0        0        0     1311 2024-03-18 14:01:48.108768 dlt-0.4.9a1/dlt/destinations/impl/athena/__init__.py
--rw-r--r--   0        0        0    18693 2024-04-13 11:31:25.760744 dlt-0.4.9a1/dlt/destinations/impl/athena/athena.py
--rw-r--r--   0        0        0     1054 2024-04-09 13:29:46.180457 dlt-0.4.9a1/dlt/destinations/impl/athena/configuration.py
--rw-r--r--   0        0        0     2169 2024-01-24 17:23:08.506518 dlt-0.4.9a1/dlt/destinations/impl/athena/factory.py
--rw-r--r--   0        0        0      439 2024-02-27 21:03:24.137544 dlt-0.4.9a1/dlt/destinations/impl/bigquery/README.md
--rw-r--r--   0        0        0     1118 2024-03-18 14:01:48.108768 dlt-0.4.9a1/dlt/destinations/impl/bigquery/__init__.py
--rw-r--r--   0        0        0    21073 2024-04-15 15:36:23.392155 dlt-0.4.9a1/dlt/destinations/impl/bigquery/bigquery.py
--rw-r--r--   0        0        0     8397 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/bigquery/bigquery_adapter.py
--rw-r--r--   0        0        0     1740 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/bigquery/configuration.py
--rw-r--r--   0        0        0     1309 2024-02-07 18:59:43.276965 dlt-0.4.9a1/dlt/destinations/impl/bigquery/factory.py
--rw-r--r--   0        0        0    10772 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/bigquery/sql_client.py
--rw-r--r--   0        0        0     1430 2024-03-18 14:01:48.118769 dlt-0.4.9a1/dlt/destinations/impl/databricks/__init__.py
--rw-r--r--   0        0        0     2043 2024-04-09 13:29:46.180457 dlt-0.4.9a1/dlt/destinations/impl/databricks/configuration.py
--rw-r--r--   0        0        0    13640 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/databricks/databricks.py
--rw-r--r--   0        0        0     1741 2024-02-07 18:59:43.276965 dlt-0.4.9a1/dlt/destinations/impl/databricks/factory.py
--rw-r--r--   0        0        0     6074 2024-04-15 15:36:23.392155 dlt-0.4.9a1/dlt/destinations/impl/databricks/sql_client.py
--rw-r--r--   0        0        0      673 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/destination/__init__.py
--rw-r--r--   0        0        0     1047 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/destination/configuration.py
--rw-r--r--   0        0        0     3675 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/destination/destination.py
--rw-r--r--   0        0        0     5626 2024-04-15 15:36:23.392155 dlt-0.4.9a1/dlt/destinations/impl/destination/factory.py
--rw-r--r--   0        0        0     1243 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/dremio/__init__.py
--rw-r--r--   0        0        0     1617 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/dremio/configuration.py
--rw-r--r--   0        0        0     8692 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/dremio/dremio.py
--rw-r--r--   0        0        0     1787 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/dremio/factory.py
--rw-r--r--   0        0        0     9314 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/dremio/pydremio.py
--rw-r--r--   0        0        0     5934 2024-04-13 11:31:52.880745 dlt-0.4.9a1/dlt/destinations/impl/dremio/sql_client.py
--rw-r--r--   0        0        0     1236 2024-03-18 14:01:48.118769 dlt-0.4.9a1/dlt/destinations/impl/duckdb/__init__.py
--rw-r--r--   0        0        0     9013 2024-04-13 11:31:56.870745 dlt-0.4.9a1/dlt/destinations/impl/duckdb/configuration.py
--rw-r--r--   0        0        0     7022 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/duckdb/duck.py
--rw-r--r--   0        0        0     1969 2024-01-24 17:23:08.516518 dlt-0.4.9a1/dlt/destinations/impl/duckdb/factory.py
--rw-r--r--   0        0        0     6828 2024-04-05 22:42:00.549456 dlt-0.4.9a1/dlt/destinations/impl/duckdb/sql_client.py
--rw-r--r--   0        0        0     1485 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/dummy/__init__.py
--rw-r--r--   0        0        0     1027 2024-04-09 13:29:46.180457 dlt-0.4.9a1/dlt/destinations/impl/dummy/configuration.py
--rw-r--r--   0        0        0     6693 2024-04-16 09:06:12.375886 dlt-0.4.9a1/dlt/destinations/impl/dummy/dummy.py
--rw-r--r--   0        0        0     1111 2024-02-23 11:16:27.641941 dlt-0.4.9a1/dlt/destinations/impl/dummy/factory.py
--rw-r--r--   0        0        0      194 2024-01-24 17:23:08.516518 dlt-0.4.9a1/dlt/destinations/impl/filesystem/__init__.py
--rw-r--r--   0        0        0     1712 2024-04-16 09:06:12.375886 dlt-0.4.9a1/dlt/destinations/impl/filesystem/configuration.py
--rw-r--r--   0        0        0     2411 2024-03-24 19:55:58.511453 dlt-0.4.9a1/dlt/destinations/impl/filesystem/factory.py
--rw-r--r--   0        0        0     9541 2024-04-16 09:06:12.385886 dlt-0.4.9a1/dlt/destinations/impl/filesystem/filesystem.py
--rw-r--r--   0        0        0      790 2024-04-16 09:06:12.385886 dlt-0.4.9a1/dlt/destinations/impl/filesystem/typing.py
--rw-r--r--   0        0        0     1134 2024-03-18 14:01:48.118769 dlt-0.4.9a1/dlt/destinations/impl/motherduck/__init__.py
--rw-r--r--   0        0        0     3111 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/motherduck/configuration.py
--rw-r--r--   0        0        0     1966 2024-01-24 17:23:08.516518 dlt-0.4.9a1/dlt/destinations/impl/motherduck/factory.py
--rw-r--r--   0        0        0      911 2024-01-24 17:23:08.516518 dlt-0.4.9a1/dlt/destinations/impl/motherduck/motherduck.py
--rw-r--r--   0        0        0     1515 2024-03-18 14:01:48.118769 dlt-0.4.9a1/dlt/destinations/impl/motherduck/sql_client.py
--rw-r--r--   0        0        0      253 2024-01-24 17:23:08.516518 dlt-0.4.9a1/dlt/destinations/impl/mssql/README.md
--rw-r--r--   0        0        0     1385 2024-01-24 17:23:08.516518 dlt-0.4.9a1/dlt/destinations/impl/mssql/__init__.py
--rw-r--r--   0        0        0     3971 2024-04-09 13:29:46.180457 dlt-0.4.9a1/dlt/destinations/impl/mssql/configuration.py
--rw-r--r--   0        0        0     1764 2024-01-24 17:23:08.516518 dlt-0.4.9a1/dlt/destinations/impl/mssql/factory.py
--rw-r--r--   0        0        0     7537 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/mssql/mssql.py
--rw-r--r--   0        0        0     6629 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/mssql/sql_client.py
--rw-r--r--   0        0        0      251 2024-01-24 17:23:08.516518 dlt-0.4.9a1/dlt/destinations/impl/postgres/README.md
--rw-r--r--   0        0        0     1356 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/postgres/__init__.py
--rw-r--r--   0        0        0     1794 2024-04-09 13:29:46.180457 dlt-0.4.9a1/dlt/destinations/impl/postgres/configuration.py
--rw-r--r--   0        0        0     1840 2024-01-24 17:23:08.516518 dlt-0.4.9a1/dlt/destinations/impl/postgres/factory.py
--rw-r--r--   0        0        0     6940 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/postgres/postgres.py
--rw-r--r--   0        0        0     5678 2024-03-31 18:13:49.090176 dlt-0.4.9a1/dlt/destinations/impl/postgres/sql_client.py
--rw-r--r--   0        0        0      677 2024-03-18 14:01:48.118769 dlt-0.4.9a1/dlt/destinations/impl/qdrant/__init__.py
--rw-r--r--   0        0        0     3044 2024-04-09 13:29:46.180457 dlt-0.4.9a1/dlt/destinations/impl/qdrant/configuration.py
--rw-r--r--   0        0        0     1146 2024-01-24 17:23:08.516518 dlt-0.4.9a1/dlt/destinations/impl/qdrant/factory.py
--rw-r--r--   0        0        0     1831 2024-02-07 18:59:43.276965 dlt-0.4.9a1/dlt/destinations/impl/qdrant/qdrant_adapter.py
--rw-r--r--   0        0        0    17960 2024-04-15 15:36:23.392155 dlt-0.4.9a1/dlt/destinations/impl/qdrant/qdrant_client.py
--rw-r--r--   0        0        0     1159 2024-01-24 17:23:08.516518 dlt-0.4.9a1/dlt/destinations/impl/redshift/README.md
--rw-r--r--   0        0        0     1181 2024-03-18 14:01:48.118769 dlt-0.4.9a1/dlt/destinations/impl/redshift/__init__.py
--rw-r--r--   0        0        0     1005 2024-04-09 13:29:46.180457 dlt-0.4.9a1/dlt/destinations/impl/redshift/configuration.py
--rw-r--r--   0        0        0     2006 2024-01-24 17:23:08.516518 dlt-0.4.9a1/dlt/destinations/impl/redshift/factory.py
--rw-r--r--   0        0        0    10832 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/redshift/redshift.py
--rw-r--r--   0        0        0     1218 2024-03-18 14:01:48.118769 dlt-0.4.9a1/dlt/destinations/impl/snowflake/__init__.py
--rw-r--r--   0        0        0     5449 2024-04-09 13:29:46.190457 dlt-0.4.9a1/dlt/destinations/impl/snowflake/configuration.py
--rw-r--r--   0        0        0     2008 2024-01-24 17:23:08.516518 dlt-0.4.9a1/dlt/destinations/impl/snowflake/factory.py
--rw-r--r--   0        0        0    11468 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/snowflake/snowflake.py
--rw-r--r--   0        0        0     6885 2024-03-18 14:01:48.118769 dlt-0.4.9a1/dlt/destinations/impl/snowflake/sql_client.py
--rw-r--r--   0        0        0     2851 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/synapse/__init__.py
--rw-r--r--   0        0        0     2746 2024-04-09 13:29:46.190457 dlt-0.4.9a1/dlt/destinations/impl/synapse/configuration.py
--rw-r--r--   0        0        0     2640 2024-04-09 13:29:46.190457 dlt-0.4.9a1/dlt/destinations/impl/synapse/factory.py
--rw-r--r--   0        0        0     1179 2024-02-07 18:59:43.276965 dlt-0.4.9a1/dlt/destinations/impl/synapse/sql_client.py
--rw-r--r--   0        0        0    13201 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/synapse/synapse.py
--rw-r--r--   0        0        0     2231 2024-03-08 19:36:32.679855 dlt-0.4.9a1/dlt/destinations/impl/synapse/synapse_adapter.py
--rw-r--r--   0        0        0      526 2024-01-24 17:23:08.516518 dlt-0.4.9a1/dlt/destinations/impl/weaviate/README.md
--rw-r--r--   0        0        0      752 2024-03-18 14:01:48.118769 dlt-0.4.9a1/dlt/destinations/impl/weaviate/__init__.py
--rw-r--r--   0        0        0      280 2024-01-24 17:23:08.516518 dlt-0.4.9a1/dlt/destinations/impl/weaviate/ci_naming.py
--rw-r--r--   0        0        0     2009 2024-04-09 13:29:46.190457 dlt-0.4.9a1/dlt/destinations/impl/weaviate/configuration.py
--rw-r--r--   0        0        0      666 2024-04-09 13:29:46.190457 dlt-0.4.9a1/dlt/destinations/impl/weaviate/exceptions.py
--rw-r--r--   0        0        0     1935 2024-01-24 17:23:08.516518 dlt-0.4.9a1/dlt/destinations/impl/weaviate/factory.py
--rw-r--r--   0        0        0     3259 2024-01-24 17:23:08.516518 dlt-0.4.9a1/dlt/destinations/impl/weaviate/naming.py
--rw-r--r--   0        0        0     3914 2024-02-07 18:59:43.276965 dlt-0.4.9a1/dlt/destinations/impl/weaviate/weaviate_adapter.py
--rw-r--r--   0        0        0    26468 2024-04-15 15:36:23.392155 dlt-0.4.9a1/dlt/destinations/impl/weaviate/weaviate_client.py
--rw-r--r--   0        0        0     6149 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/insert_job_client.py
--rw-r--r--   0        0        0    23940 2024-04-15 15:36:23.392155 dlt-0.4.9a1/dlt/destinations/job_client_impl.py
--rw-r--r--   0        0        0     6300 2024-04-15 15:36:23.392155 dlt-0.4.9a1/dlt/destinations/job_impl.py
--rw-r--r--   0        0        0     8366 2024-04-16 09:06:12.385886 dlt-0.4.9a1/dlt/destinations/path_utils.py
--rw-r--r--   0        0        0     9279 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/sql_client.py
--rw-r--r--   0        0        0    26428 2024-04-15 15:36:23.392155 dlt-0.4.9a1/dlt/destinations/sql_jobs.py
--rw-r--r--   0        0        0     4895 2024-02-27 21:03:24.137544 dlt-0.4.9a1/dlt/destinations/type_mapping.py
--rw-r--r--   0        0        0     1877 2024-01-24 17:23:08.516518 dlt-0.4.9a1/dlt/destinations/typing.py
--rw-r--r--   0        0        0      506 2024-04-11 11:44:50.568746 dlt-0.4.9a1/dlt/destinations/utils.py
--rw-r--r--   0        0        0      639 2024-04-07 14:59:43.715656 dlt-0.4.9a1/dlt/extract/__init__.py
--rw-r--r--   0        0        0     8539 2024-03-08 19:36:32.679855 dlt-0.4.9a1/dlt/extract/concurrency.py
--rw-r--r--   0        0        0    35950 2024-04-15 15:36:23.392155 dlt-0.4.9a1/dlt/extract/decorators.py
--rw-r--r--   0        0        0    16480 2024-03-08 19:36:32.679855 dlt-0.4.9a1/dlt/extract/exceptions.py
--rw-r--r--   0        0        0    17697 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/extract/extract.py
--rw-r--r--   0        0        0    15690 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/extract/extractors.py
--rw-r--r--   0        0        0    21382 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/extract/hints.py
--rw-r--r--   0        0        0    29587 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/extract/incremental/__init__.py
--rw-r--r--   0        0        0     1142 2024-01-24 17:23:08.526518 dlt-0.4.9a1/dlt/extract/incremental/exceptions.py
--rw-r--r--   0        0        0    14951 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/extract/incremental/transform.py
--rw-r--r--   0        0        0      322 2024-01-24 17:23:08.526518 dlt-0.4.9a1/dlt/extract/incremental/typing.py
--rw-r--r--   0        0        0     6786 2024-04-09 13:29:46.190457 dlt-0.4.9a1/dlt/extract/items.py
--rw-r--r--   0        0        0    16368 2024-03-08 19:36:32.679855 dlt-0.4.9a1/dlt/extract/pipe.py
--rw-r--r--   0        0        0    16344 2024-04-09 13:29:46.190457 dlt-0.4.9a1/dlt/extract/pipe_iterator.py
--rw-r--r--   0        0        0    26683 2024-04-09 13:29:46.190457 dlt-0.4.9a1/dlt/extract/resource.py
--rw-r--r--   0        0        0    19990 2024-03-18 14:01:48.118769 dlt-0.4.9a1/dlt/extract/source.py
--rw-r--r--   0        0        0     4650 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/extract/storage.py
--rw-r--r--   0        0        0    10122 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/extract/utils.py
--rw-r--r--   0        0        0     3500 2024-03-08 19:36:32.679855 dlt-0.4.9a1/dlt/extract/validation.py
--rw-r--r--   0        0        0      832 2024-04-07 14:59:43.715656 dlt-0.4.9a1/dlt/extract/wrappers.py
--rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 dlt-0.4.9a1/dlt/helpers/__init__.py
--rw-r--r--   0        0        0    23547 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/helpers/airflow_helper.py
--rw-r--r--   0        0        0     3701 2024-01-24 17:23:08.526518 dlt-0.4.9a1/dlt/helpers/dbt/__init__.py
--rw-r--r--   0        0        0     1241 2024-04-09 13:29:46.190457 dlt-0.4.9a1/dlt/helpers/dbt/configuration.py
--rw-r--r--   0        0        0     6848 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/helpers/dbt/dbt_utils.py
--rw-r--r--   0        0        0      772 2024-01-24 17:23:08.526518 dlt-0.4.9a1/dlt/helpers/dbt/exceptions.py
--rw-r--r--   0        0        0     7163 2024-02-07 18:59:43.286965 dlt-0.4.9a1/dlt/helpers/dbt/profiles.yml
--rw-r--r--   0        0        0    15742 2024-04-13 11:33:15.710743 dlt-0.4.9a1/dlt/helpers/dbt/runner.py
--rw-r--r--   0        0        0     4881 2023-11-18 17:38:04.277189 dlt-0.4.9a1/dlt/helpers/dbt_cloud/__init__.py
--rw-r--r--   0        0        0     4926 2024-01-24 17:23:08.526518 dlt-0.4.9a1/dlt/helpers/dbt_cloud/client.py
--rw-r--r--   0        0        0      623 2024-04-09 13:29:46.190457 dlt-0.4.9a1/dlt/helpers/dbt_cloud/configuration.py
--rw-r--r--   0        0        0      349 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/helpers/streamlit_app/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 14:59:43.715656 dlt-0.4.9a1/dlt/helpers/streamlit_app/blocks/__init__.py
--rw-r--r--   0        0        0     1239 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/helpers/streamlit_app/blocks/load_info.py
--rw-r--r--   0        0        0      483 2024-04-07 14:59:43.715656 dlt-0.4.9a1/dlt/helpers/streamlit_app/blocks/menu.py
--rw-r--r--   0        0        0     2451 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/helpers/streamlit_app/blocks/query.py
--rw-r--r--   0        0        0     1139 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/helpers/streamlit_app/blocks/resource_state.py
--rw-r--r--   0        0        0      618 2024-04-07 14:59:43.715656 dlt-0.4.9a1/dlt/helpers/streamlit_app/blocks/show_data.py
--rw-r--r--   0        0        0     2842 2024-04-07 14:59:43.725656 dlt-0.4.9a1/dlt/helpers/streamlit_app/blocks/table_hints.py
--rw-r--r--   0        0        0      150 2024-04-07 14:59:43.725656 dlt-0.4.9a1/dlt/helpers/streamlit_app/index.py
--rw-r--r--   0        0        0        0 2024-04-07 14:59:43.725656 dlt-0.4.9a1/dlt/helpers/streamlit_app/pages/__init__.py
--rw-r--r--   0        0        0     1668 2024-04-07 14:59:43.725656 dlt-0.4.9a1/dlt/helpers/streamlit_app/pages/dashboard.py
--rw-r--r--   0        0        0     4446 2024-04-07 14:59:43.725656 dlt-0.4.9a1/dlt/helpers/streamlit_app/pages/load_info.py
--rw-r--r--   0        0        0      757 2024-04-07 14:59:43.725656 dlt-0.4.9a1/dlt/helpers/streamlit_app/theme.py
--rw-r--r--   0        0        0     2361 2024-04-09 13:29:46.190457 dlt-0.4.9a1/dlt/helpers/streamlit_app/utils.py
--rw-r--r--   0        0        0      386 2024-04-07 14:59:43.725656 dlt-0.4.9a1/dlt/helpers/streamlit_app/widgets/__init__.py
--rw-r--r--   0        0        0      901 2024-04-07 14:59:43.725656 dlt-0.4.9a1/dlt/helpers/streamlit_app/widgets/color_mode_selector.py
--rw-r--r--   0        0        0     1004 2024-04-07 14:59:43.725656 dlt-0.4.9a1/dlt/helpers/streamlit_app/widgets/logo.py
--rw-r--r--   0        0        0      613 2024-04-07 14:59:43.725656 dlt-0.4.9a1/dlt/helpers/streamlit_app/widgets/schema.py
--rw-r--r--   0        0        0     1542 2024-04-07 14:59:43.725656 dlt-0.4.9a1/dlt/helpers/streamlit_app/widgets/stats.py
--rw-r--r--   0        0        0      805 2024-04-07 14:59:43.725656 dlt-0.4.9a1/dlt/helpers/streamlit_app/widgets/summary.py
--rw-r--r--   0        0        0     1189 2024-04-07 14:59:43.725656 dlt-0.4.9a1/dlt/helpers/streamlit_app/widgets/tags.py
--rw-r--r--   0        0        0       51 2023-11-18 17:38:04.277189 dlt-0.4.9a1/dlt/load/__init__.py
--rw-r--r--   0        0        0      807 2024-04-09 13:29:46.190457 dlt-0.4.9a1/dlt/load/configuration.py
--rw-r--r--   0        0        0     2061 2024-04-09 13:29:46.190457 dlt-0.4.9a1/dlt/load/exceptions.py
--rw-r--r--   0        0        0    25029 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/load/load.py
--rw-r--r--   0        0        0     8096 2024-04-13 11:33:36.000744 dlt-0.4.9a1/dlt/load/utils.py
--rw-r--r--   0        0        0       58 2024-01-24 17:23:08.526518 dlt-0.4.9a1/dlt/normalize/__init__.py
--rw-r--r--   0        0        0     1598 2024-04-16 09:06:12.385886 dlt-0.4.9a1/dlt/normalize/configuration.py
--rw-r--r--   0        0        0      644 2024-04-09 20:42:07.320460 dlt-0.4.9a1/dlt/normalize/exceptions.py
--rw-r--r--   0        0        0    18280 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/normalize/items_normalizers.py
--rw-r--r--   0        0        0    23745 2024-04-16 09:06:12.385886 dlt-0.4.9a1/dlt/normalize/normalize.py
--rw-r--r--   0        0        0    15006 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/pipeline/__init__.py
--rw-r--r--   0        0        0     2097 2024-04-09 20:42:07.320460 dlt-0.4.9a1/dlt/pipeline/configuration.py
--rw-r--r--   0        0        0      709 2024-04-07 14:59:43.725656 dlt-0.4.9a1/dlt/pipeline/current.py
--rw-r--r--   0        0        0     4950 2024-01-24 17:23:08.536518 dlt-0.4.9a1/dlt/pipeline/dbt.py
--rw-r--r--   0        0        0     4599 2024-04-07 14:59:43.725656 dlt-0.4.9a1/dlt/pipeline/exceptions.py
--rw-r--r--   0        0        0     9785 2024-04-09 20:42:07.320460 dlt-0.4.9a1/dlt/pipeline/helpers.py
--rw-r--r--   0        0        0      212 2024-04-07 14:59:43.725656 dlt-0.4.9a1/dlt/pipeline/mark.py
--rw-r--r--   0        0        0    72369 2024-04-16 09:06:12.385886 dlt-0.4.9a1/dlt/pipeline/pipeline.py
--rw-r--r--   0        0        0     3864 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/pipeline/platform.py
--rw-r--r--   0        0        0     1007 2024-01-24 17:23:08.536518 dlt-0.4.9a1/dlt/pipeline/progress.py
--rw-r--r--   0        0        0     4856 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/pipeline/state_sync.py
--rw-r--r--   0        0        0    13259 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/pipeline/trace.py
--rw-r--r--   0        0        0     5610 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/pipeline/track.py
--rw-r--r--   0        0        0       92 2024-01-24 17:23:08.536518 dlt-0.4.9a1/dlt/pipeline/typing.py
--rw-r--r--   0        0        0      796 2024-01-24 17:23:08.536518 dlt-0.4.9a1/dlt/pipeline/warnings.py
--rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 dlt-0.4.9a1/dlt/py.typed
--rw-r--r--   0        0        0        0 2023-11-18 17:38:04.277189 dlt-0.4.9a1/dlt/reflection/__init__.py
--rw-r--r--   0        0        0      565 2024-01-24 17:23:08.536518 dlt-0.4.9a1/dlt/reflection/names.py
--rw-r--r--   0        0        0     5818 2024-04-13 11:34:58.380741 dlt-0.4.9a1/dlt/reflection/script_inspector.py
--rw-r--r--   0        0        0     6278 2024-01-24 17:23:08.536518 dlt-0.4.9a1/dlt/reflection/script_visitor.py
--rw-r--r--   0        0        0      417 2024-01-24 17:23:08.536518 dlt-0.4.9a1/dlt/sources/__init__.py
--rw-r--r--   0        0        0      110 2024-01-24 17:23:08.536518 dlt-0.4.9a1/dlt/sources/config.py
--rw-r--r--   0        0        0      790 2024-01-24 17:23:08.536518 dlt-0.4.9a1/dlt/sources/credentials.py
--rw-r--r--   0        0        0      200 2024-01-24 17:23:08.536518 dlt-0.4.9a1/dlt/sources/filesystem.py
--rw-r--r--   0        0        0        0 2023-11-18 17:38:04.277189 dlt-0.4.9a1/dlt/sources/helpers/__init__.py
--rw-r--r--   0        0        0     1291 2024-04-09 20:42:07.320460 dlt-0.4.9a1/dlt/sources/helpers/requests/__init__.py
--rw-r--r--   0        0        0    10965 2024-01-24 17:23:08.536518 dlt-0.4.9a1/dlt/sources/helpers/requests/retry.py
--rw-r--r--   0        0        0     1969 2024-01-24 17:23:08.536518 dlt-0.4.9a1/dlt/sources/helpers/requests/session.py
--rw-r--r--   0        0        0      234 2023-11-18 17:38:04.277189 dlt-0.4.9a1/dlt/sources/helpers/requests/typing.py
--rw-r--r--   0        0        0     1210 2024-04-13 11:26:19.690742 dlt-0.4.9a1/dlt/sources/helpers/rest_client/__init__.py
--rw-r--r--   0        0        0     7190 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/sources/helpers/rest_client/auth.py
--rw-r--r--   0        0        0     9181 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/sources/helpers/rest_client/client.py
--rw-r--r--   0        0        0     4456 2024-04-13 22:20:19.334997 dlt-0.4.9a1/dlt/sources/helpers/rest_client/detector.py
--rw-r--r--   0        0        0      103 2024-04-09 13:29:46.190457 dlt-0.4.9a1/dlt/sources/helpers/rest_client/exceptions.py
--rw-r--r--   0        0        0     6001 2024-04-13 22:20:19.334997 dlt-0.4.9a1/dlt/sources/helpers/rest_client/paginators.py
--rw-r--r--   0        0        0      426 2024-04-13 22:20:19.334997 dlt-0.4.9a1/dlt/sources/helpers/rest_client/typing.py
--rw-r--r--   0        0        0      406 2024-04-09 13:29:46.190457 dlt-0.4.9a1/dlt/sources/helpers/rest_client/utils.py
--rw-r--r--   0        0        0     4860 2024-04-15 15:36:23.412155 dlt-0.4.9a1/dlt/sources/helpers/transform.py
--rw-r--r--   0        0        0     1130 2024-04-15 15:36:23.412155 dlt-0.4.9a1/dlt/version.py
--rw-r--r--   0        0        0     7009 2024-04-16 09:07:01.515887 dlt-0.4.9a1/pyproject.toml
--rw-r--r--   0        0        0     9936 1970-01-01 00:00:00.000000 dlt-0.4.9a1/PKG-INFO
+-rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 dlt-0.4.9a2/LICENSE.txt
+-rw-r--r--   0        0        0     5298 2024-04-17 22:48:56.892849 dlt-0.4.9a2/README.md
+-rw-r--r--   0        0        0     2229 2024-04-17 22:48:56.892849 dlt-0.4.9a2/dlt/__init__.py
+-rw-r--r--   0        0        0       69 2024-04-17 22:48:56.892849 dlt-0.4.9a2/dlt/__main__.py
+-rw-r--r--   0        0        0        0 2023-11-18 17:38:04.257189 dlt-0.4.9a2/dlt/cli/__init__.py
+-rw-r--r--   0        0        0    21512 2024-04-17 22:48:56.892849 dlt-0.4.9a2/dlt/cli/_dlt.py
+-rw-r--r--   0        0        0     4187 2024-04-17 22:48:56.892849 dlt-0.4.9a2/dlt/cli/config_toml_writer.py
+-rw-r--r--   0        0        0    18229 2024-01-24 17:23:08.476518 dlt-0.4.9a2/dlt/cli/deploy_command.py
+-rw-r--r--   0        0        0    16912 2024-04-17 10:21:33.106065 dlt-0.4.9a2/dlt/cli/deploy_command_helpers.py
+-rw-r--r--   0        0        0     1944 2024-01-25 20:07:33.363195 dlt-0.4.9a2/dlt/cli/echo.py
+-rw-r--r--   0        0        0      435 2023-11-18 17:38:04.257189 dlt-0.4.9a2/dlt/cli/exceptions.py
+-rw-r--r--   0        0        0    21105 2024-04-13 11:38:33.320742 dlt-0.4.9a2/dlt/cli/init_command.py
+-rw-r--r--   0        0        0    14157 2024-04-17 22:48:56.892849 dlt-0.4.9a2/dlt/cli/pipeline_command.py
+-rw-r--r--   0        0        0    10152 2024-04-13 11:38:50.650742 dlt-0.4.9a2/dlt/cli/pipeline_files.py
+-rw-r--r--   0        0        0     2524 2024-01-24 17:23:08.476518 dlt-0.4.9a2/dlt/cli/requirements.py
+-rw-r--r--   0        0        0     4895 2024-01-24 17:23:08.476518 dlt-0.4.9a2/dlt/cli/source_detection.py
+-rw-r--r--   0        0        0     1912 2024-01-24 17:23:08.476518 dlt-0.4.9a2/dlt/cli/telemetry_command.py
+-rw-r--r--   0        0        0     1999 2024-04-17 22:48:56.892849 dlt-0.4.9a2/dlt/cli/utils.py
+-rw-r--r--   0        0        0      292 2024-04-17 22:48:56.892849 dlt-0.4.9a2/dlt/common/__init__.py
+-rw-r--r--   0        0        0     1311 2024-01-24 17:23:08.476518 dlt-0.4.9a2/dlt/common/arithmetics.py
+-rw-r--r--   0        0        0      808 2024-04-17 22:48:56.892849 dlt-0.4.9a2/dlt/common/configuration/__init__.py
+-rw-r--r--   0        0        0     5144 2024-01-24 17:23:08.476518 dlt-0.4.9a2/dlt/common/configuration/accessors.py
+-rw-r--r--   0        0        0     7410 2024-04-17 22:48:56.892849 dlt-0.4.9a2/dlt/common/configuration/container.py
+-rw-r--r--   0        0        0     8457 2024-01-24 17:23:08.486518 dlt-0.4.9a2/dlt/common/configuration/exceptions.py
+-rw-r--r--   0        0        0    11848 2024-04-17 22:48:56.892849 dlt-0.4.9a2/dlt/common/configuration/inject.py
+-rw-r--r--   0        0        0     1777 2024-01-25 20:07:33.363195 dlt-0.4.9a2/dlt/common/configuration/paths.py
+-rw-r--r--   0        0        0      682 2024-01-24 17:23:08.486518 dlt-0.4.9a2/dlt/common/configuration/providers/__init__.py
+-rw-r--r--   0        0        0      805 2024-03-05 18:21:35.930419 dlt-0.4.9a2/dlt/common/configuration/providers/airflow.py
+-rw-r--r--   0        0        0     1129 2024-01-24 17:23:08.486518 dlt-0.4.9a2/dlt/common/configuration/providers/context.py
+-rw-r--r--   0        0        0     1346 2024-01-24 17:23:08.486518 dlt-0.4.9a2/dlt/common/configuration/providers/dictionary.py
+-rw-r--r--   0        0        0     1995 2024-01-24 17:23:08.486518 dlt-0.4.9a2/dlt/common/configuration/providers/environ.py
+-rw-r--r--   0        0        0     5141 2024-04-17 22:48:56.892849 dlt-0.4.9a2/dlt/common/configuration/providers/google_secrets.py
+-rw-r--r--   0        0        0     1319 2024-01-24 17:23:08.486518 dlt-0.4.9a2/dlt/common/configuration/providers/provider.py
+-rw-r--r--   0        0        0    13416 2024-04-17 22:48:56.892849 dlt-0.4.9a2/dlt/common/configuration/providers/toml.py
+-rw-r--r--   0        0        0    20983 2024-04-17 22:48:56.892849 dlt-0.4.9a2/dlt/common/configuration/resolve.py
+-rw-r--r--   0        0        0     1742 2024-01-24 17:23:08.486518 dlt-0.4.9a2/dlt/common/configuration/specs/__init__.py
+-rw-r--r--   0        0        0     1836 2024-04-17 22:48:56.892849 dlt-0.4.9a2/dlt/common/configuration/specs/api_credentials.py
+-rw-r--r--   0        0        0     5263 2024-04-17 22:48:56.892849 dlt-0.4.9a2/dlt/common/configuration/specs/aws_credentials.py
+-rw-r--r--   0        0        0     2591 2024-04-17 22:48:56.892849 dlt-0.4.9a2/dlt/common/configuration/specs/azure_credentials.py
+-rw-r--r--   0        0        0    18147 2024-04-17 22:48:56.892849 dlt-0.4.9a2/dlt/common/configuration/specs/base_configuration.py
+-rw-r--r--   0        0        0     6498 2024-04-17 22:48:56.892849 dlt-0.4.9a2/dlt/common/configuration/specs/config_providers_context.py
+-rw-r--r--   0        0        0     3456 2024-04-17 22:48:56.892849 dlt-0.4.9a2/dlt/common/configuration/specs/config_section_context.py
+-rw-r--r--   0        0        0     2339 2024-04-17 22:48:56.892849 dlt-0.4.9a2/dlt/common/configuration/specs/connection_string_credentials.py
+-rw-r--r--   0        0        0     2667 2024-01-24 17:23:08.486518 dlt-0.4.9a2/dlt/common/configuration/specs/exceptions.py
+-rw-r--r--   0        0        0    13349 2024-04-17 22:48:56.892849 dlt-0.4.9a2/dlt/common/configuration/specs/gcp_credentials.py
+-rw-r--r--   0        0        0      874 2024-04-17 22:48:56.892849 dlt-0.4.9a2/dlt/common/configuration/specs/known_sections.py
+-rw-r--r--   0        0        0     2856 2024-04-17 22:48:56.892849 dlt-0.4.9a2/dlt/common/configuration/specs/run_configuration.py
+-rw-r--r--   0        0        0     6650 2024-04-17 22:48:56.892849 dlt-0.4.9a2/dlt/common/configuration/utils.py
+-rw-r--r--   0        0        0      220 2024-01-24 17:23:08.486518 dlt-0.4.9a2/dlt/common/data_types/__init__.py
+-rw-r--r--   0        0        0     6832 2024-04-17 22:48:56.892849 dlt-0.4.9a2/dlt/common/data_types/type_helpers.py
+-rw-r--r--   0        0        0      269 2024-01-24 17:23:08.486518 dlt-0.4.9a2/dlt/common/data_types/typing.py
+-rw-r--r--   0        0        0      754 2024-04-17 22:48:56.892849 dlt-0.4.9a2/dlt/common/data_writers/__init__.py
+-rw-r--r--   0        0        0    10766 2024-04-17 22:48:56.892849 dlt-0.4.9a2/dlt/common/data_writers/buffered.py
+-rw-r--r--   0        0        0     5665 2024-04-17 22:48:56.892849 dlt-0.4.9a2/dlt/common/data_writers/escape.py
+-rw-r--r--   0        0        0     2894 2024-04-17 22:48:56.892849 dlt-0.4.9a2/dlt/common/data_writers/exceptions.py
+-rw-r--r--   0        0        0    27725 2024-04-19 07:08:50.183863 dlt-0.4.9a2/dlt/common/data_writers/writers.py
+-rw-r--r--   0        0        0      483 2024-04-17 22:48:56.892849 dlt-0.4.9a2/dlt/common/destination/__init__.py
+-rw-r--r--   0        0        0     5375 2024-04-17 22:48:56.892849 dlt-0.4.9a2/dlt/common/destination/capabilities.py
+-rw-r--r--   0        0        0     5132 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/destination/exceptions.py
+-rw-r--r--   0        0        0    25552 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/destination/reference.py
+-rw-r--r--   0        0        0     6274 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/exceptions.py
+-rw-r--r--   0        0        0     5149 2024-01-24 17:23:08.496518 dlt-0.4.9a2/dlt/common/git.py
+-rw-r--r--   0        0        0     7099 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/json/__init__.py
+-rw-r--r--   0        0        0     1814 2024-02-16 18:38:47.332466 dlt-0.4.9a2/dlt/common/json/_orjson.py
+-rw-r--r--   0        0        0     2948 2024-01-24 17:23:08.496518 dlt-0.4.9a2/dlt/common/json/_simplejson.py
+-rw-r--r--   0        0        0     1562 2023-11-18 17:38:04.257189 dlt-0.4.9a2/dlt/common/jsonpath.py
+-rw-r--r--   0        0        0        0 2023-11-18 17:38:04.257189 dlt-0.4.9a2/dlt/common/libs/__init__.py
+-rw-r--r--   0        0        0      181 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/libs/numpy.py
+-rw-r--r--   0        0        0      436 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/libs/pandas.py
+-rw-r--r--   0        0        0      217 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/libs/pandas_sql.py
+-rw-r--r--   0        0        0    14934 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/libs/pyarrow.py
+-rw-r--r--   0        0        0    15624 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/libs/pydantic.py
+-rw-r--r--   0        0        0    15486 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/libs/sql_alchemy.py
+-rw-r--r--   0        0        0     3652 2024-04-17 22:48:57.012849 dlt-0.4.9a2/dlt/common/logger.py
+-rw-r--r--   0        0        0      854 2024-03-01 09:52:05.856761 dlt-0.4.9a2/dlt/common/managed_thread_pool.py
+-rw-r--r--   0        0        0      384 2024-03-18 14:01:48.098768 dlt-0.4.9a2/dlt/common/normalizers/__init__.py
+-rw-r--r--   0        0        0     1408 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/normalizers/configuration.py
+-rw-r--r--   0        0        0      510 2024-01-24 17:23:08.496518 dlt-0.4.9a2/dlt/common/normalizers/exceptions.py
+-rw-r--r--   0        0        0     1905 2024-01-24 17:23:08.496518 dlt-0.4.9a2/dlt/common/normalizers/json/__init__.py
+-rw-r--r--   0        0        0    16970 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/normalizers/json/relational.py
+-rw-r--r--   0        0        0      123 2024-03-18 14:01:48.098768 dlt-0.4.9a2/dlt/common/normalizers/naming/__init__.py
+-rw-r--r--   0        0        0      810 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/normalizers/naming/direct.py
+-rw-r--r--   0        0        0      798 2024-01-24 17:23:08.496518 dlt-0.4.9a2/dlt/common/normalizers/naming/duck_case.py
+-rw-r--r--   0        0        0      830 2024-03-18 14:01:48.098768 dlt-0.4.9a2/dlt/common/normalizers/naming/exceptions.py
+-rw-r--r--   0        0        0     4570 2024-03-18 14:01:48.098768 dlt-0.4.9a2/dlt/common/normalizers/naming/naming.py
+-rw-r--r--   0        0        0     2967 2024-01-24 17:23:08.496518 dlt-0.4.9a2/dlt/common/normalizers/naming/snake_case.py
+-rw-r--r--   0        0        0      359 2024-03-18 14:01:48.108768 dlt-0.4.9a2/dlt/common/normalizers/typing.py
+-rw-r--r--   0        0        0     3426 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/normalizers/utils.py
+-rw-r--r--   0        0        0      461 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/pendulum.py
+-rw-r--r--   0        0        0    31127 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/pipeline.py
+-rw-r--r--   0        0        0        0 2023-11-18 17:38:04.267189 dlt-0.4.9a2/dlt/common/reflection/__init__.py
+-rw-r--r--   0        0        0      375 2024-01-24 17:23:08.496518 dlt-0.4.9a2/dlt/common/reflection/function_visitor.py
+-rw-r--r--   0        0        0     6119 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/reflection/spec.py
+-rw-r--r--   0        0        0     5210 2024-04-19 07:08:50.183863 dlt-0.4.9a2/dlt/common/reflection/utils.py
+-rw-r--r--   0        0        0      329 2024-01-24 17:23:08.496518 dlt-0.4.9a2/dlt/common/runners/__init__.py
+-rw-r--r--   0        0        0      665 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/runners/configuration.py
+-rw-r--r--   0        0        0     3678 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/runners/pool_runner.py
+-rw-r--r--   0        0        0     4132 2024-01-24 17:23:08.496518 dlt-0.4.9a2/dlt/common/runners/runnable.py
+-rw-r--r--   0        0        0     3162 2024-01-24 17:23:08.496518 dlt-0.4.9a2/dlt/common/runners/stdout.py
+-rw-r--r--   0        0        0     2137 2024-01-24 17:23:08.496518 dlt-0.4.9a2/dlt/common/runners/synth_pickle.py
+-rw-r--r--   0        0        0      105 2023-11-18 17:38:04.267189 dlt-0.4.9a2/dlt/common/runners/typing.py
+-rw-r--r--   0        0        0     5583 2024-01-24 17:23:08.496518 dlt-0.4.9a2/dlt/common/runners/venv.py
+-rw-r--r--   0        0        0       71 2023-11-18 17:38:04.267189 dlt-0.4.9a2/dlt/common/runtime/__init__.py
+-rw-r--r--   0        0        0    14599 2024-04-13 11:30:10.760740 dlt-0.4.9a2/dlt/common/runtime/collector.py
+-rw-r--r--   0        0        0     5461 2024-01-25 20:07:33.363195 dlt-0.4.9a2/dlt/common/runtime/exec_info.py
+-rw-r--r--   0        0        0     1067 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/runtime/init.py
+-rw-r--r--   0        0        0     6616 2024-01-24 17:23:08.496518 dlt-0.4.9a2/dlt/common/runtime/json_logging.py
+-rw-r--r--   0        0        0     2044 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/runtime/prometheus.py
+-rw-r--r--   0        0        0     6702 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/runtime/segment.py
+-rw-r--r--   0        0        0     2784 2024-01-24 17:23:08.496518 dlt-0.4.9a2/dlt/common/runtime/sentry.py
+-rw-r--r--   0        0        0     1938 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/runtime/signals.py
+-rw-r--r--   0        0        0      613 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/runtime/slack.py
+-rw-r--r--   0        0        0     2960 2024-01-24 17:23:08.496518 dlt-0.4.9a2/dlt/common/runtime/telemetry.py
+-rw-r--r--   0        0        0      579 2024-01-24 17:23:08.496518 dlt-0.4.9a2/dlt/common/runtime/typing.py
+-rw-r--r--   0        0        0      805 2024-01-24 17:23:08.496518 dlt-0.4.9a2/dlt/common/schema/__init__.py
+-rw-r--r--   0        0        0     2454 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/schema/detections.py
+-rw-r--r--   0        0        0     5308 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/schema/exceptions.py
+-rw-r--r--   0        0        0     5269 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/schema/migrations.py
+-rw-r--r--   0        0        0    42497 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/schema/schema.py
+-rw-r--r--   0        0        0     5865 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/schema/typing.py
+-rw-r--r--   0        0        0    28875 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/schema/utils.py
+-rw-r--r--   0        0        0     1672 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/source.py
+-rw-r--r--   0        0        0     1224 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/storages/__init__.py
+-rw-r--r--   0        0        0     4869 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/storages/configuration.py
+-rw-r--r--   0        0        0     4175 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/storages/data_item_storage.py
+-rw-r--r--   0        0        0     4184 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/storages/exceptions.py
+-rw-r--r--   0        0        0    14242 2024-01-24 17:23:08.506518 dlt-0.4.9a2/dlt/common/storages/file_storage.py
+-rw-r--r--   0        0        0    11065 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/storages/fsspec_filesystem.py
+-rw-r--r--   0        0        0        0 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/storages/fsspecs/__init__.py
+-rw-r--r--   0        0        0    20512 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/storages/fsspecs/google_drive.py
+-rw-r--r--   0        0        0     3513 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/storages/live_schema_storage.py
+-rw-r--r--   0        0        0    27168 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/storages/load_package.py
+-rw-r--r--   0        0        0     9920 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/storages/load_storage.py
+-rw-r--r--   0        0        0     3197 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/storages/normalize_storage.py
+-rw-r--r--   0        0        0     9551 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/storages/schema_storage.py
+-rw-r--r--   0        0        0     9065 2024-01-24 17:23:08.506518 dlt-0.4.9a2/dlt/common/storages/transactional_file.py
+-rw-r--r--   0        0        0     2867 2024-01-24 17:23:08.506518 dlt-0.4.9a2/dlt/common/storages/versioned_storage.py
+-rw-r--r--   0        0        0     7681 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/time.py
+-rw-r--r--   0        0        0     8878 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/typing.py
+-rw-r--r--   0        0        0    19596 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/utils.py
+-rw-r--r--   0        0        0     7978 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/validation.py
+-rw-r--r--   0        0        0     2369 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/common/versioned_state.py
+-rw-r--r--   0        0        0     5528 2024-01-24 17:23:08.506518 dlt-0.4.9a2/dlt/common/warnings.py
+-rw-r--r--   0        0        0     1219 2024-01-24 17:23:08.506518 dlt-0.4.9a2/dlt/common/wei.py
+-rw-r--r--   0        0        0     1217 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/__init__.py
+-rw-r--r--   0        0        0      404 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/adapters.py
+-rw-r--r--   0        0        0     4856 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/decorators.py
+-rw-r--r--   0        0        0     6070 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/exceptions.py
+-rw-r--r--   0        0        0        0 2024-01-24 17:23:08.506518 dlt-0.4.9a2/dlt/destinations/impl/__init__.py
+-rw-r--r--   0        0        0     1311 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/athena/__init__.py
+-rw-r--r--   0        0        0    18705 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/athena/athena.py
+-rw-r--r--   0        0        0     1054 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/athena/configuration.py
+-rw-r--r--   0        0        0     2169 2024-01-24 17:23:08.506518 dlt-0.4.9a2/dlt/destinations/impl/athena/factory.py
+-rw-r--r--   0        0        0      439 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/bigquery/README.md
+-rw-r--r--   0        0        0     1118 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/bigquery/__init__.py
+-rw-r--r--   0        0        0    21073 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/bigquery/bigquery.py
+-rw-r--r--   0        0        0     8397 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/bigquery/bigquery_adapter.py
+-rw-r--r--   0        0        0     1740 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/bigquery/configuration.py
+-rw-r--r--   0        0        0     1309 2024-02-07 18:59:43.276965 dlt-0.4.9a2/dlt/destinations/impl/bigquery/factory.py
+-rw-r--r--   0        0        0    10772 2024-04-19 08:12:26.163860 dlt-0.4.9a2/dlt/destinations/impl/bigquery/sql_client.py
+-rw-r--r--   0        0        0     1430 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/databricks/__init__.py
+-rw-r--r--   0        0        0     2043 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/databricks/configuration.py
+-rw-r--r--   0        0        0    13640 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/databricks/databricks.py
+-rw-r--r--   0        0        0     1741 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/databricks/factory.py
+-rw-r--r--   0        0        0     6074 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/databricks/sql_client.py
+-rw-r--r--   0        0        0      673 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/destination/__init__.py
+-rw-r--r--   0        0        0     1047 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/destination/configuration.py
+-rw-r--r--   0        0        0     3692 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/destination/destination.py
+-rw-r--r--   0        0        0     5626 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/destination/factory.py
+-rw-r--r--   0        0        0     1243 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/dremio/__init__.py
+-rw-r--r--   0        0        0     1617 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/dremio/configuration.py
+-rw-r--r--   0        0        0     8692 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/dremio/dremio.py
+-rw-r--r--   0        0        0     1787 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/dremio/factory.py
+-rw-r--r--   0        0        0     9314 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/dremio/pydremio.py
+-rw-r--r--   0        0        0     5934 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/dremio/sql_client.py
+-rw-r--r--   0        0        0     1236 2024-03-18 14:01:48.118769 dlt-0.4.9a2/dlt/destinations/impl/duckdb/__init__.py
+-rw-r--r--   0        0        0     9013 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/duckdb/configuration.py
+-rw-r--r--   0        0        0     7022 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/duckdb/duck.py
+-rw-r--r--   0        0        0     1969 2024-01-24 17:23:08.516518 dlt-0.4.9a2/dlt/destinations/impl/duckdb/factory.py
+-rw-r--r--   0        0        0     6828 2024-04-05 22:42:00.549456 dlt-0.4.9a2/dlt/destinations/impl/duckdb/sql_client.py
+-rw-r--r--   0        0        0     1485 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/dummy/__init__.py
+-rw-r--r--   0        0        0     1027 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/dummy/configuration.py
+-rw-r--r--   0        0        0     6710 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/dummy/dummy.py
+-rw-r--r--   0        0        0     1111 2024-02-23 11:16:27.641941 dlt-0.4.9a2/dlt/destinations/impl/dummy/factory.py
+-rw-r--r--   0        0        0      194 2024-01-24 17:23:08.516518 dlt-0.4.9a2/dlt/destinations/impl/filesystem/__init__.py
+-rw-r--r--   0        0        0     1712 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/filesystem/configuration.py
+-rw-r--r--   0        0        0     2411 2024-03-24 19:55:58.511453 dlt-0.4.9a2/dlt/destinations/impl/filesystem/factory.py
+-rw-r--r--   0        0        0    17294 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/filesystem/filesystem.py
+-rw-r--r--   0        0        0      790 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/filesystem/typing.py
+-rw-r--r--   0        0        0     1134 2024-03-18 14:01:48.118769 dlt-0.4.9a2/dlt/destinations/impl/motherduck/__init__.py
+-rw-r--r--   0        0        0     3111 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/motherduck/configuration.py
+-rw-r--r--   0        0        0     1966 2024-01-24 17:23:08.516518 dlt-0.4.9a2/dlt/destinations/impl/motherduck/factory.py
+-rw-r--r--   0        0        0      911 2024-01-24 17:23:08.516518 dlt-0.4.9a2/dlt/destinations/impl/motherduck/motherduck.py
+-rw-r--r--   0        0        0     1515 2024-03-18 14:01:48.118769 dlt-0.4.9a2/dlt/destinations/impl/motherduck/sql_client.py
+-rw-r--r--   0        0        0      253 2024-01-24 17:23:08.516518 dlt-0.4.9a2/dlt/destinations/impl/mssql/README.md
+-rw-r--r--   0        0        0     1385 2024-04-17 19:33:15.912844 dlt-0.4.9a2/dlt/destinations/impl/mssql/__init__.py
+-rw-r--r--   0        0        0     3971 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/mssql/configuration.py
+-rw-r--r--   0        0        0     1764 2024-01-24 17:23:08.516518 dlt-0.4.9a2/dlt/destinations/impl/mssql/factory.py
+-rw-r--r--   0        0        0     7537 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/mssql/mssql.py
+-rw-r--r--   0        0        0     6629 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/mssql/sql_client.py
+-rw-r--r--   0        0        0      251 2024-01-24 17:23:08.516518 dlt-0.4.9a2/dlt/destinations/impl/postgres/README.md
+-rw-r--r--   0        0        0     1356 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/postgres/__init__.py
+-rw-r--r--   0        0        0     1794 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/postgres/configuration.py
+-rw-r--r--   0        0        0     1840 2024-01-24 17:23:08.516518 dlt-0.4.9a2/dlt/destinations/impl/postgres/factory.py
+-rw-r--r--   0        0        0     6940 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/postgres/postgres.py
+-rw-r--r--   0        0        0     5678 2024-03-31 18:13:49.090176 dlt-0.4.9a2/dlt/destinations/impl/postgres/sql_client.py
+-rw-r--r--   0        0        0      677 2024-03-18 14:01:48.118769 dlt-0.4.9a2/dlt/destinations/impl/qdrant/__init__.py
+-rw-r--r--   0        0        0     3044 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/qdrant/configuration.py
+-rw-r--r--   0        0        0     1146 2024-01-24 17:23:08.516518 dlt-0.4.9a2/dlt/destinations/impl/qdrant/factory.py
+-rw-r--r--   0        0        0     1831 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/qdrant/qdrant_adapter.py
+-rw-r--r--   0        0        0    17977 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/qdrant/qdrant_client.py
+-rw-r--r--   0        0        0     1159 2024-01-24 17:23:08.516518 dlt-0.4.9a2/dlt/destinations/impl/redshift/README.md
+-rw-r--r--   0        0        0     1181 2024-03-18 14:01:48.118769 dlt-0.4.9a2/dlt/destinations/impl/redshift/__init__.py
+-rw-r--r--   0        0        0     1005 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/redshift/configuration.py
+-rw-r--r--   0        0        0     2006 2024-01-24 17:23:08.516518 dlt-0.4.9a2/dlt/destinations/impl/redshift/factory.py
+-rw-r--r--   0        0        0    10832 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/redshift/redshift.py
+-rw-r--r--   0        0        0     1218 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/snowflake/__init__.py
+-rw-r--r--   0        0        0     5449 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/snowflake/configuration.py
+-rw-r--r--   0        0        0     2008 2024-01-24 17:23:08.516518 dlt-0.4.9a2/dlt/destinations/impl/snowflake/factory.py
+-rw-r--r--   0        0        0    11468 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/snowflake/snowflake.py
+-rw-r--r--   0        0        0     6885 2024-03-18 14:01:48.118769 dlt-0.4.9a2/dlt/destinations/impl/snowflake/sql_client.py
+-rw-r--r--   0        0        0     2851 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/synapse/__init__.py
+-rw-r--r--   0        0        0     2746 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/synapse/configuration.py
+-rw-r--r--   0        0        0     2640 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/synapse/factory.py
+-rw-r--r--   0        0        0     1179 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/synapse/sql_client.py
+-rw-r--r--   0        0        0    11169 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/synapse/synapse.py
+-rw-r--r--   0        0        0     2231 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/synapse/synapse_adapter.py
+-rw-r--r--   0        0        0      526 2024-01-24 17:23:08.516518 dlt-0.4.9a2/dlt/destinations/impl/weaviate/README.md
+-rw-r--r--   0        0        0      752 2024-03-18 14:01:48.118769 dlt-0.4.9a2/dlt/destinations/impl/weaviate/__init__.py
+-rw-r--r--   0        0        0      280 2024-01-24 17:23:08.516518 dlt-0.4.9a2/dlt/destinations/impl/weaviate/ci_naming.py
+-rw-r--r--   0        0        0     2009 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/weaviate/configuration.py
+-rw-r--r--   0        0        0      666 2024-04-17 22:48:56.902849 dlt-0.4.9a2/dlt/destinations/impl/weaviate/exceptions.py
+-rw-r--r--   0        0        0     1935 2024-01-24 17:23:08.516518 dlt-0.4.9a2/dlt/destinations/impl/weaviate/factory.py
+-rw-r--r--   0        0        0     3259 2024-01-24 17:23:08.516518 dlt-0.4.9a2/dlt/destinations/impl/weaviate/naming.py
+-rw-r--r--   0        0        0     3914 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/destinations/impl/weaviate/weaviate_adapter.py
+-rw-r--r--   0        0        0    26041 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/destinations/impl/weaviate/weaviate_client.py
+-rw-r--r--   0        0        0     6149 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/destinations/insert_job_client.py
+-rw-r--r--   0        0        0    23403 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/destinations/job_client_impl.py
+-rw-r--r--   0        0        0     6300 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/destinations/job_impl.py
+-rw-r--r--   0        0        0     8366 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/destinations/path_utils.py
+-rw-r--r--   0        0        0     9279 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/destinations/sql_client.py
+-rw-r--r--   0        0        0    26428 2024-04-19 08:12:26.173860 dlt-0.4.9a2/dlt/destinations/sql_jobs.py
+-rw-r--r--   0        0        0     4895 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/destinations/type_mapping.py
+-rw-r--r--   0        0        0     1877 2024-01-24 17:23:08.516518 dlt-0.4.9a2/dlt/destinations/typing.py
+-rw-r--r--   0        0        0      506 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/destinations/utils.py
+-rw-r--r--   0        0        0      639 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/extract/__init__.py
+-rw-r--r--   0        0        0     8539 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/extract/concurrency.py
+-rw-r--r--   0        0        0    35950 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/extract/decorators.py
+-rw-r--r--   0        0        0    16480 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/extract/exceptions.py
+-rw-r--r--   0        0        0    18432 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/extract/extract.py
+-rw-r--r--   0        0        0    15690 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/extract/extractors.py
+-rw-r--r--   0        0        0    21382 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/extract/hints.py
+-rw-r--r--   0        0        0    29587 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/extract/incremental/__init__.py
+-rw-r--r--   0        0        0     1142 2024-01-24 17:23:08.526518 dlt-0.4.9a2/dlt/extract/incremental/exceptions.py
+-rw-r--r--   0        0        0    14951 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/extract/incremental/transform.py
+-rw-r--r--   0        0        0      322 2024-01-24 17:23:08.526518 dlt-0.4.9a2/dlt/extract/incremental/typing.py
+-rw-r--r--   0        0        0     6786 2024-04-17 22:48:57.012849 dlt-0.4.9a2/dlt/extract/items.py
+-rw-r--r--   0        0        0    16368 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/extract/pipe.py
+-rw-r--r--   0        0        0    16344 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/extract/pipe_iterator.py
+-rw-r--r--   0        0        0    26683 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/extract/resource.py
+-rw-r--r--   0        0        0    19990 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/extract/source.py
+-rw-r--r--   0        0        0     4650 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/extract/storage.py
+-rw-r--r--   0        0        0    10122 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/extract/utils.py
+-rw-r--r--   0        0        0     3500 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/extract/validation.py
+-rw-r--r--   0        0        0      832 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/extract/wrappers.py
+-rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 dlt-0.4.9a2/dlt/helpers/__init__.py
+-rw-r--r--   0        0        0    23547 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/helpers/airflow_helper.py
+-rw-r--r--   0        0        0     3701 2024-01-24 17:23:08.526518 dlt-0.4.9a2/dlt/helpers/dbt/__init__.py
+-rw-r--r--   0        0        0     1241 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/helpers/dbt/configuration.py
+-rw-r--r--   0        0        0     6848 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/helpers/dbt/dbt_utils.py
+-rw-r--r--   0        0        0      772 2024-01-24 17:23:08.526518 dlt-0.4.9a2/dlt/helpers/dbt/exceptions.py
+-rw-r--r--   0        0        0     7163 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/helpers/dbt/profiles.yml
+-rw-r--r--   0        0        0    15742 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/helpers/dbt/runner.py
+-rw-r--r--   0        0        0     4881 2023-11-18 17:38:04.277189 dlt-0.4.9a2/dlt/helpers/dbt_cloud/__init__.py
+-rw-r--r--   0        0        0     4926 2024-01-24 17:23:08.526518 dlt-0.4.9a2/dlt/helpers/dbt_cloud/client.py
+-rw-r--r--   0        0        0      623 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/helpers/dbt_cloud/configuration.py
+-rw-r--r--   0        0        0      349 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/helpers/streamlit_app/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/helpers/streamlit_app/blocks/__init__.py
+-rw-r--r--   0        0        0     1239 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/helpers/streamlit_app/blocks/load_info.py
+-rw-r--r--   0        0        0      483 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/helpers/streamlit_app/blocks/menu.py
+-rw-r--r--   0        0        0     2451 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/helpers/streamlit_app/blocks/query.py
+-rw-r--r--   0        0        0     1139 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/helpers/streamlit_app/blocks/resource_state.py
+-rw-r--r--   0        0        0      618 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/helpers/streamlit_app/blocks/show_data.py
+-rw-r--r--   0        0        0     2842 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/helpers/streamlit_app/blocks/table_hints.py
+-rw-r--r--   0        0        0      150 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/helpers/streamlit_app/index.py
+-rw-r--r--   0        0        0        0 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/helpers/streamlit_app/pages/__init__.py
+-rw-r--r--   0        0        0     1668 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/helpers/streamlit_app/pages/dashboard.py
+-rw-r--r--   0        0        0     4446 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/helpers/streamlit_app/pages/load_info.py
+-rw-r--r--   0        0        0      757 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/helpers/streamlit_app/theme.py
+-rw-r--r--   0        0        0     2361 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/helpers/streamlit_app/utils.py
+-rw-r--r--   0        0        0      386 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/helpers/streamlit_app/widgets/__init__.py
+-rw-r--r--   0        0        0      901 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/helpers/streamlit_app/widgets/color_mode_selector.py
+-rw-r--r--   0        0        0     1004 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/helpers/streamlit_app/widgets/logo.py
+-rw-r--r--   0        0        0      613 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/helpers/streamlit_app/widgets/schema.py
+-rw-r--r--   0        0        0     1542 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/helpers/streamlit_app/widgets/stats.py
+-rw-r--r--   0        0        0      805 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/helpers/streamlit_app/widgets/summary.py
+-rw-r--r--   0        0        0     1189 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/helpers/streamlit_app/widgets/tags.py
+-rw-r--r--   0        0        0       51 2023-11-18 17:38:04.277189 dlt-0.4.9a2/dlt/load/__init__.py
+-rw-r--r--   0        0        0      807 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/load/configuration.py
+-rw-r--r--   0        0        0     2061 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/load/exceptions.py
+-rw-r--r--   0        0        0    25264 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/load/load.py
+-rw-r--r--   0        0        0     8096 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/load/utils.py
+-rw-r--r--   0        0        0       58 2024-01-24 17:23:08.526518 dlt-0.4.9a2/dlt/normalize/__init__.py
+-rw-r--r--   0        0        0     1598 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/normalize/configuration.py
+-rw-r--r--   0        0        0      644 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/normalize/exceptions.py
+-rw-r--r--   0        0        0    18280 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/normalize/items_normalizers.py
+-rw-r--r--   0        0        0    23745 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/normalize/normalize.py
+-rw-r--r--   0        0        0    15006 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/pipeline/__init__.py
+-rw-r--r--   0        0        0     2097 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/pipeline/configuration.py
+-rw-r--r--   0        0        0      709 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/pipeline/current.py
+-rw-r--r--   0        0        0     4950 2024-01-24 17:23:08.536518 dlt-0.4.9a2/dlt/pipeline/dbt.py
+-rw-r--r--   0        0        0     4599 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/pipeline/exceptions.py
+-rw-r--r--   0        0        0     9785 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/pipeline/helpers.py
+-rw-r--r--   0        0        0      212 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/pipeline/mark.py
+-rw-r--r--   0        0        0    72582 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/pipeline/pipeline.py
+-rw-r--r--   0        0        0     3864 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/pipeline/platform.py
+-rw-r--r--   0        0        0     1007 2024-01-24 17:23:08.536518 dlt-0.4.9a2/dlt/pipeline/progress.py
+-rw-r--r--   0        0        0     5256 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/pipeline/state_sync.py
+-rw-r--r--   0        0        0    13259 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/pipeline/trace.py
+-rw-r--r--   0        0        0     5610 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/pipeline/track.py
+-rw-r--r--   0        0        0       92 2024-01-24 17:23:08.536518 dlt-0.4.9a2/dlt/pipeline/typing.py
+-rw-r--r--   0        0        0      796 2024-04-17 10:21:33.946065 dlt-0.4.9a2/dlt/pipeline/warnings.py
+-rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 dlt-0.4.9a2/dlt/py.typed
+-rw-r--r--   0        0        0        0 2023-11-18 17:38:04.277189 dlt-0.4.9a2/dlt/reflection/__init__.py
+-rw-r--r--   0        0        0      565 2024-01-24 17:23:08.536518 dlt-0.4.9a2/dlt/reflection/names.py
+-rw-r--r--   0        0        0     5818 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/reflection/script_inspector.py
+-rw-r--r--   0        0        0     6278 2024-01-24 17:23:08.536518 dlt-0.4.9a2/dlt/reflection/script_visitor.py
+-rw-r--r--   0        0        0      417 2024-01-24 17:23:08.536518 dlt-0.4.9a2/dlt/sources/__init__.py
+-rw-r--r--   0        0        0      110 2024-01-24 17:23:08.536518 dlt-0.4.9a2/dlt/sources/config.py
+-rw-r--r--   0        0        0      790 2024-01-24 17:23:08.536518 dlt-0.4.9a2/dlt/sources/credentials.py
+-rw-r--r--   0        0        0      200 2024-01-24 17:23:08.536518 dlt-0.4.9a2/dlt/sources/filesystem.py
+-rw-r--r--   0        0        0        0 2023-11-18 17:38:04.277189 dlt-0.4.9a2/dlt/sources/helpers/__init__.py
+-rw-r--r--   0        0        0     1291 2024-04-09 20:42:07.320460 dlt-0.4.9a2/dlt/sources/helpers/requests/__init__.py
+-rw-r--r--   0        0        0    10965 2024-01-24 17:23:08.536518 dlt-0.4.9a2/dlt/sources/helpers/requests/retry.py
+-rw-r--r--   0        0        0     1969 2024-01-24 17:23:08.536518 dlt-0.4.9a2/dlt/sources/helpers/requests/session.py
+-rw-r--r--   0        0        0      234 2023-11-18 17:38:04.277189 dlt-0.4.9a2/dlt/sources/helpers/requests/typing.py
+-rw-r--r--   0        0        0     1210 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/sources/helpers/rest_client/__init__.py
+-rw-r--r--   0        0        0     7190 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/sources/helpers/rest_client/auth.py
+-rw-r--r--   0        0        0     9181 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/sources/helpers/rest_client/client.py
+-rw-r--r--   0        0        0     4456 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/sources/helpers/rest_client/detector.py
+-rw-r--r--   0        0        0      103 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/sources/helpers/rest_client/exceptions.py
+-rw-r--r--   0        0        0     6001 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/sources/helpers/rest_client/paginators.py
+-rw-r--r--   0        0        0      426 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/sources/helpers/rest_client/typing.py
+-rw-r--r--   0        0        0      406 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/sources/helpers/rest_client/utils.py
+-rw-r--r--   0        0        0     4860 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/sources/helpers/transform.py
+-rw-r--r--   0        0        0     1130 2024-04-17 22:48:56.912849 dlt-0.4.9a2/dlt/version.py
+-rw-r--r--   0        0        0     7026 2024-04-19 08:18:57.503858 dlt-0.4.9a2/pyproject.toml
+-rw-r--r--   0        0        0     9968 1970-01-01 00:00:00.000000 dlt-0.4.9a2/PKG-INFO
```

### Comparing `dlt-0.4.9a1/LICENSE.txt` & `dlt-0.4.9a2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/README.md` & `dlt-0.4.9a2/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/__init__.py` & `dlt-0.4.9a2/dlt/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/cli/_dlt.py` & `dlt-0.4.9a2/dlt/cli/_dlt.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/cli/config_toml_writer.py` & `dlt-0.4.9a2/dlt/cli/config_toml_writer.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/cli/deploy_command.py` & `dlt-0.4.9a2/dlt/cli/deploy_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/cli/deploy_command_helpers.py` & `dlt-0.4.9a2/dlt/cli/deploy_command_helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/cli/echo.py` & `dlt-0.4.9a2/dlt/cli/echo.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/cli/init_command.py` & `dlt-0.4.9a2/dlt/cli/init_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/cli/pipeline_command.py` & `dlt-0.4.9a2/dlt/cli/pipeline_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/cli/pipeline_files.py` & `dlt-0.4.9a2/dlt/cli/pipeline_files.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/cli/requirements.py` & `dlt-0.4.9a2/dlt/cli/requirements.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/cli/source_detection.py` & `dlt-0.4.9a2/dlt/cli/source_detection.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/cli/telemetry_command.py` & `dlt-0.4.9a2/dlt/cli/telemetry_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/cli/utils.py` & `dlt-0.4.9a2/dlt/cli/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/arithmetics.py` & `dlt-0.4.9a2/dlt/common/arithmetics.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/configuration/__init__.py` & `dlt-0.4.9a2/dlt/common/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/configuration/accessors.py` & `dlt-0.4.9a2/dlt/common/configuration/accessors.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/configuration/container.py` & `dlt-0.4.9a2/dlt/common/configuration/container.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/configuration/exceptions.py` & `dlt-0.4.9a2/dlt/common/configuration/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/configuration/inject.py` & `dlt-0.4.9a2/dlt/common/configuration/inject.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/configuration/paths.py` & `dlt-0.4.9a2/dlt/common/configuration/paths.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/configuration/providers/__init__.py` & `dlt-0.4.9a2/dlt/common/configuration/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/configuration/providers/airflow.py` & `dlt-0.4.9a2/dlt/common/configuration/providers/airflow.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/configuration/providers/context.py` & `dlt-0.4.9a2/dlt/common/configuration/providers/context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/configuration/providers/dictionary.py` & `dlt-0.4.9a2/dlt/common/configuration/providers/dictionary.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/configuration/providers/environ.py` & `dlt-0.4.9a2/dlt/common/configuration/providers/environ.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/configuration/providers/google_secrets.py` & `dlt-0.4.9a2/dlt/common/configuration/providers/google_secrets.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/configuration/providers/provider.py` & `dlt-0.4.9a2/dlt/common/configuration/providers/provider.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/configuration/providers/toml.py` & `dlt-0.4.9a2/dlt/common/configuration/providers/toml.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/configuration/resolve.py` & `dlt-0.4.9a2/dlt/common/configuration/resolve.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/configuration/specs/__init__.py` & `dlt-0.4.9a2/dlt/common/configuration/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/configuration/specs/api_credentials.py` & `dlt-0.4.9a2/dlt/common/configuration/specs/api_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/configuration/specs/aws_credentials.py` & `dlt-0.4.9a2/dlt/common/configuration/specs/aws_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/configuration/specs/azure_credentials.py` & `dlt-0.4.9a2/dlt/common/configuration/specs/azure_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/configuration/specs/base_configuration.py` & `dlt-0.4.9a2/dlt/common/configuration/specs/base_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/configuration/specs/config_providers_context.py` & `dlt-0.4.9a2/dlt/common/configuration/specs/config_providers_context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/configuration/specs/config_section_context.py` & `dlt-0.4.9a2/dlt/common/configuration/specs/config_section_context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/configuration/specs/connection_string_credentials.py` & `dlt-0.4.9a2/dlt/common/configuration/specs/connection_string_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/configuration/specs/exceptions.py` & `dlt-0.4.9a2/dlt/common/configuration/specs/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/configuration/specs/gcp_credentials.py` & `dlt-0.4.9a2/dlt/common/configuration/specs/gcp_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/configuration/specs/known_sections.py` & `dlt-0.4.9a2/dlt/common/configuration/specs/known_sections.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/configuration/specs/run_configuration.py` & `dlt-0.4.9a2/dlt/common/configuration/specs/run_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/configuration/utils.py` & `dlt-0.4.9a2/dlt/common/configuration/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/data_types/type_helpers.py` & `dlt-0.4.9a2/dlt/common/data_types/type_helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/data_writers/__init__.py` & `dlt-0.4.9a2/dlt/common/data_writers/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/data_writers/buffered.py` & `dlt-0.4.9a2/dlt/common/data_writers/buffered.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/data_writers/escape.py` & `dlt-0.4.9a2/dlt/common/data_writers/escape.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/data_writers/exceptions.py` & `dlt-0.4.9a2/dlt/common/data_writers/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/data_writers/writers.py` & `dlt-0.4.9a2/dlt/common/data_writers/writers.py`

 * *Files 2% similar despite different names*

```diff
@@ -377,38 +377,51 @@
             is_binary_format=True,
             supports_schema_changes="Buffer",
             requires_destination_capabilities=True,
             supports_compression=False,
         )
 
 
+@configspec
+class CsvDataWriterConfiguration(BaseConfiguration):
+    delimiter: str = ","
+    include_header: bool = True
+
+    __section__: ClassVar[str] = known_sections.DATA_WRITER
+
+
 class CsvWriter(DataWriter):
+    @with_config(spec=CsvDataWriterConfiguration)
     def __init__(
         self,
         f: IO[Any],
         caps: DestinationCapabilitiesContext = None,
+        *,
         delimiter: str = ",",
+        include_header: bool = True,
         bytes_encoding: str = "utf-8",
     ) -> None:
         super().__init__(f, caps)
+        self.include_header = include_header
         self.delimiter = delimiter
         self.writer: csv.DictWriter[str] = None
         self.bytes_encoding = bytes_encoding
 
     def write_header(self, columns_schema: TTableSchemaColumns) -> None:
         self._columns_schema = columns_schema
         self.writer = csv.DictWriter(
             self._f,
             fieldnames=list(columns_schema.keys()),
             extrasaction="ignore",
             dialect=csv.unix_dialect,
             delimiter=self.delimiter,
             quoting=csv.QUOTE_NONNUMERIC,
         )
-        self.writer.writeheader()
+        if self.include_header:
+            self.writer.writeheader()
         # find row items that are of the complex type (could be abstracted out for use in other writers?)
         self.complex_indices = [
             i for i, field in columns_schema.items() if field["data_type"] == "complex"
         ]
         # find row items that are of the complex type (could be abstracted out for use in other writers?)
         self.bytes_indices = [
             i for i, field in columns_schema.items() if field["data_type"] == "binary"
@@ -495,19 +508,27 @@
             supports_schema_changes="False",
             requires_destination_capabilities=False,
             supports_compression=False,
         )
 
 
 class ArrowToCsvWriter(DataWriter):
+    @with_config(spec=CsvDataWriterConfiguration)
     def __init__(
-        self, f: IO[Any], caps: DestinationCapabilitiesContext = None, delimiter: bytes = b","
+        self,
+        f: IO[Any],
+        caps: DestinationCapabilitiesContext = None,
+        *,
+        delimiter: str = ",",
+        include_header: bool = True,
     ) -> None:
         super().__init__(f, caps)
         self.delimiter = delimiter
+        self._delimiter_b = delimiter.encode("ascii")
+        self.include_header = include_header
         self.writer: Any = None
 
     def write_header(self, columns_schema: TTableSchemaColumns) -> None:
         self._columns_schema = columns_schema
 
     def write_data(self, rows: Sequence[Any]) -> None:
         from dlt.common.libs.pyarrow import pyarrow
@@ -517,15 +538,16 @@
             if isinstance(row, (pyarrow.Table, pyarrow.RecordBatch)):
                 if not self.writer:
                     try:
                         self.writer = pyarrow.csv.CSVWriter(
                             self._f,
                             row.schema,
                             write_options=pyarrow.csv.WriteOptions(
-                                include_header=True, delimiter=self.delimiter
+                                include_header=self.include_header,
+                                delimiter=self._delimiter_b,
                             ),
                         )
                         self._first_schema = row.schema
                     except pyarrow.ArrowInvalid as inv_ex:
                         if "Unsupported Type" in str(inv_ex):
                             raise InvalidDataItem(
                                 "csv",
@@ -569,18 +591,18 @@
                     raise
             else:
                 raise ValueError(f"Unsupported type {type(row)}")
             # count rows that got written
             self.items_count += row.num_rows
 
     def write_footer(self) -> None:
-        if self.writer is None:
+        if self.writer is None and self.include_header:
             # write empty file
             self._f.write(
-                self.delimiter.join(
+                self._delimiter_b.join(
                     [
                         b'"' + col["name"].encode("utf-8") + b'"'
                         for col in self._columns_schema.values()
                     ]
                 )
             )
```

### Comparing `dlt-0.4.9a1/dlt/common/destination/capabilities.py` & `dlt-0.4.9a2/dlt/common/destination/capabilities.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/destination/exceptions.py` & `dlt-0.4.9a2/dlt/common/destination/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/destination/reference.py` & `dlt-0.4.9a2/dlt/common/destination/reference.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,15 +269,17 @@
 
     @abstractmethod
     def drop_storage(self) -> None:
         """Brings storage back into not initialized state. Typically data in storage is destroyed."""
         pass
 
     def update_stored_schema(
-        self, only_tables: Iterable[str] = None, expected_update: TSchemaTables = None
+        self,
+        only_tables: Iterable[str] = None,
+        expected_update: TSchemaTables = None,
     ) -> Optional[TSchemaTables]:
         """Updates storage to the current schema.
 
         Implementations should not assume that `expected_update` is the exact difference between destination state and the self.schema. This is only the case if
         destination has single writer and no other processes modify the schema.
 
         Args:
@@ -430,14 +432,15 @@
     @abstractmethod
     def get_stored_schema(self) -> Optional[StorageSchemaInfo]:
         """Retrieves newest schema from destination storage"""
         pass
 
     @abstractmethod
     def get_stored_schema_by_hash(self, version_hash: str) -> StorageSchemaInfo:
+        """retrieves the stored schema by hash"""
         pass
 
     @abstractmethod
     def get_stored_state(self, pipeline_name: str) -> Optional[StateInfo]:
         """Loads compressed state from destination storage"""
         pass
```

### Comparing `dlt-0.4.9a1/dlt/common/exceptions.py` & `dlt-0.4.9a2/dlt/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/git.py` & `dlt-0.4.9a2/dlt/common/git.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/json/__init__.py` & `dlt-0.4.9a2/dlt/common/json/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/json/_orjson.py` & `dlt-0.4.9a2/dlt/common/json/_orjson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/json/_simplejson.py` & `dlt-0.4.9a2/dlt/common/json/_simplejson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/jsonpath.py` & `dlt-0.4.9a2/dlt/common/jsonpath.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/libs/pyarrow.py` & `dlt-0.4.9a2/dlt/common/libs/pyarrow.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/libs/pydantic.py` & `dlt-0.4.9a2/dlt/common/libs/pydantic.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/libs/sql_alchemy.py` & `dlt-0.4.9a2/dlt/common/libs/sql_alchemy.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/logger.py` & `dlt-0.4.9a2/dlt/common/logger.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/managed_thread_pool.py` & `dlt-0.4.9a2/dlt/common/managed_thread_pool.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/normalizers/configuration.py` & `dlt-0.4.9a2/dlt/common/normalizers/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/normalizers/json/__init__.py` & `dlt-0.4.9a2/dlt/common/normalizers/json/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/normalizers/json/relational.py` & `dlt-0.4.9a2/dlt/common/normalizers/json/relational.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/normalizers/naming/direct.py` & `dlt-0.4.9a2/dlt/common/normalizers/naming/direct.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/normalizers/naming/duck_case.py` & `dlt-0.4.9a2/dlt/common/normalizers/naming/duck_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/normalizers/naming/exceptions.py` & `dlt-0.4.9a2/dlt/common/normalizers/naming/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/normalizers/naming/naming.py` & `dlt-0.4.9a2/dlt/common/normalizers/naming/naming.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/normalizers/naming/snake_case.py` & `dlt-0.4.9a2/dlt/common/normalizers/naming/snake_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/normalizers/utils.py` & `dlt-0.4.9a2/dlt/common/normalizers/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/pipeline.py` & `dlt-0.4.9a2/dlt/common/pipeline.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/reflection/spec.py` & `dlt-0.4.9a2/dlt/common/reflection/spec.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/reflection/utils.py` & `dlt-0.4.9a2/dlt/common/reflection/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import ast
 import inspect
 import astunparse
-from typing import Any, Dict, List, Optional, Sequence, Tuple
+from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
 
 from dlt.common.typing import AnyFun
 
 
-def get_literal_defaults(node: ast.FunctionDef) -> Dict[str, str]:
+def get_literal_defaults(node: Union[ast.FunctionDef, ast.AsyncFunctionDef]) -> Dict[str, str]:
     """Extract defaults from function definition node literally, as pieces of source code"""
     defaults: List[ast.expr] = []
     if node.args.defaults:
         defaults.extend(node.args.defaults)
     if node.args.kw_defaults:
         defaults.extend(node.args.kw_defaults)
     args: List[ast.arg] = []
@@ -26,20 +26,20 @@
     for arg, default in zip(reversed(args), reversed(defaults)):
         if default:
             literal_defaults[str(arg.arg)] = astunparse.unparse(default).strip()
 
     return literal_defaults
 
 
-def get_func_def_node(f: AnyFun) -> ast.FunctionDef:
+def get_func_def_node(f: AnyFun) -> Union[ast.FunctionDef, ast.AsyncFunctionDef]:
     """Finds the function definition node for function f by parsing the source code of the f's module"""
     source, lineno = inspect.findsource(inspect.unwrap(f))
 
     for node in ast.walk(ast.parse("".join(source))):
-        if isinstance(node, ast.FunctionDef):
+        if isinstance(node, ast.FunctionDef) or isinstance(node, ast.AsyncFunctionDef):
             f_lineno = node.lineno - 1
             # get line number of first decorator
             if node.decorator_list:
                 f_lineno = node.decorator_list[0].lineno - 1
             # line number and function name must match
             if f_lineno == lineno and node.name == f.__name__:
                 return node
```

### Comparing `dlt-0.4.9a1/dlt/common/runners/configuration.py` & `dlt-0.4.9a2/dlt/common/runners/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/runners/pool_runner.py` & `dlt-0.4.9a2/dlt/common/runners/pool_runner.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/runners/runnable.py` & `dlt-0.4.9a2/dlt/common/runners/runnable.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/runners/stdout.py` & `dlt-0.4.9a2/dlt/common/runners/stdout.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/runners/synth_pickle.py` & `dlt-0.4.9a2/dlt/common/runners/synth_pickle.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/runners/venv.py` & `dlt-0.4.9a2/dlt/common/runners/venv.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/runtime/collector.py` & `dlt-0.4.9a2/dlt/common/runtime/collector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/runtime/exec_info.py` & `dlt-0.4.9a2/dlt/common/runtime/exec_info.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/runtime/init.py` & `dlt-0.4.9a2/dlt/common/runtime/init.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/runtime/json_logging.py` & `dlt-0.4.9a2/dlt/common/runtime/json_logging.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/runtime/prometheus.py` & `dlt-0.4.9a2/dlt/common/runtime/prometheus.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/runtime/segment.py` & `dlt-0.4.9a2/dlt/common/runtime/segment.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/runtime/sentry.py` & `dlt-0.4.9a2/dlt/common/runtime/sentry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/runtime/signals.py` & `dlt-0.4.9a2/dlt/common/runtime/signals.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/runtime/slack.py` & `dlt-0.4.9a2/dlt/common/runtime/slack.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/runtime/telemetry.py` & `dlt-0.4.9a2/dlt/common/runtime/telemetry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/runtime/typing.py` & `dlt-0.4.9a2/dlt/common/runtime/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/schema/__init__.py` & `dlt-0.4.9a2/dlt/common/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/schema/detections.py` & `dlt-0.4.9a2/dlt/common/schema/detections.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/schema/exceptions.py` & `dlt-0.4.9a2/dlt/common/schema/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/schema/migrations.py` & `dlt-0.4.9a2/dlt/common/schema/migrations.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/schema/schema.py` & `dlt-0.4.9a2/dlt/common/schema/schema.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/schema/typing.py` & `dlt-0.4.9a2/dlt/common/schema/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/schema/utils.py` & `dlt-0.4.9a2/dlt/common/schema/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/source.py` & `dlt-0.4.9a2/dlt/common/source.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/storages/__init__.py` & `dlt-0.4.9a2/dlt/common/storages/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/storages/configuration.py` & `dlt-0.4.9a2/dlt/common/storages/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/storages/data_item_storage.py` & `dlt-0.4.9a2/dlt/common/storages/data_item_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/storages/exceptions.py` & `dlt-0.4.9a2/dlt/common/storages/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/storages/file_storage.py` & `dlt-0.4.9a2/dlt/common/storages/file_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/storages/fsspec_filesystem.py` & `dlt-0.4.9a2/dlt/common/storages/fsspec_filesystem.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/storages/fsspecs/google_drive.py` & `dlt-0.4.9a2/dlt/common/storages/fsspecs/google_drive.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,15 +233,15 @@
         mime_type is something like "text/plain"
         """
         file_id = self.path_to_file_id(path)
         return self.service.export(
             fileId=file_id, mimeType=mime_type, supportsAllDrives=True
         ).execute()
 
-    def ls(self, path: str, detail: Optional[bool] = False) -> Any:
+    def ls(self, path: str, detail: Optional[bool] = False, refresh: Optional[bool] = False) -> Any:
         """List files in a directory.
 
         Args:
             path (str): The directory to list.
             detail (Optional[bool]): Whether to return detailed file information.
                 Defaults to False.
```

### Comparing `dlt-0.4.9a1/dlt/common/storages/live_schema_storage.py` & `dlt-0.4.9a2/dlt/common/storages/live_schema_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/storages/load_package.py` & `dlt-0.4.9a2/dlt/common/storages/load_package.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,17 +50,31 @@
 )
 from dlt.common.time import precise_time
 
 TJobFileFormat = Literal["sql", "reference", TLoaderFileFormat]
 """Loader file formats with internal job types"""
 
 
+class TPipelineStateDoc(TypedDict, total=False):
+    """Corresponds to the StateInfo Tuple"""
+
+    version: int
+    engine_version: int
+    pipeline_name: str
+    state: str
+    version_hash: str
+    created_at: datetime.datetime
+    dlt_load_id: NotRequired[str]
+
+
 class TLoadPackageState(TVersionedState, total=False):
     created_at: DateTime
     """Timestamp when the load package was created"""
+    pipeline_state: NotRequired[TPipelineStateDoc]
+    """Pipeline state, added at the end of the extraction phase"""
 
     """A section of state that does not participate in change merging and version control"""
     destination_state: NotRequired[Dict[str, Any]]
     """private space for destinations to store state relevant only to the load package"""
 
 
 class TLoadPackage(TypedDict, total=False):
```

### Comparing `dlt-0.4.9a1/dlt/common/storages/load_storage.py` & `dlt-0.4.9a2/dlt/common/storages/load_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/storages/normalize_storage.py` & `dlt-0.4.9a2/dlt/common/storages/normalize_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/storages/schema_storage.py` & `dlt-0.4.9a2/dlt/common/storages/schema_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/storages/transactional_file.py` & `dlt-0.4.9a2/dlt/common/storages/transactional_file.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/storages/versioned_storage.py` & `dlt-0.4.9a2/dlt/common/storages/versioned_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/time.py` & `dlt-0.4.9a2/dlt/common/time.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 import contextlib
-from typing import Any, Optional, Union, overload, TypeVar, Callable  # noqa
 import datetime  # noqa: I251
+from typing import Any, Optional, Union, overload, TypeVar, Callable  # noqa
 
-from dlt.common.pendulum import pendulum, timedelta
-from dlt.common.typing import TimedeltaSeconds, TAnyDateTime
-from pendulum.parsing import parse_iso8601, _parse_common as parse_datetime_common
+from pendulum.parsing import (
+    parse_iso8601,
+    DEFAULT_OPTIONS as pendulum_options,
+    _parse_common as parse_datetime_common,
+)
 from pendulum.tz import UTC
 
+from dlt.common.pendulum import pendulum, timedelta
+from dlt.common.typing import TimedeltaSeconds, TAnyDateTime
 
 PAST_TIMESTAMP: float = 0.0
 FUTURE_TIMESTAMP: float = 9999999999.0
 DAY_DURATION_SEC: float = 24 * 60 * 60.0
 
 precise_time: Callable[[], float] = None
 """A precise timer using win_precise_time library on windows and time.time on other systems"""
@@ -41,26 +45,26 @@
     check if timestamp is before max timestamp, inclusive
     """
     return timestamp <= (max_inclusive or FUTURE_TIMESTAMP)
 
 
 def parse_iso_like_datetime(value: Any) -> Union[pendulum.DateTime, pendulum.Date, pendulum.Time]:
     """Parses ISO8601 string into pendulum datetime, date or time. Preserves timezone info.
-    Note: naive datetimes will generated from string without timezone
+    Note: naive datetimes will be generated from string without timezone
 
        we use internal pendulum parse function. the generic function, for example, parses string "now" as now()
        it also tries to parse ISO intervals but the code is very low quality
     """
     # only iso dates are allowed
     dtv = None
     with contextlib.suppress(ValueError):
         dtv = parse_iso8601(value)
     # now try to parse a set of ISO like dates
     if not dtv:
-        dtv = parse_datetime_common(value)
+        dtv = parse_datetime_common(value, **pendulum_options)
     if isinstance(dtv, datetime.time):
         return pendulum.time(dtv.hour, dtv.minute, dtv.second, dtv.microsecond)
     if isinstance(dtv, datetime.datetime):
         return pendulum.instance(dtv, tz=dtv.tzinfo)
     if isinstance(dtv, pendulum.Duration):
         raise ValueError("Interval ISO 8601 not supported: " + value)
     return pendulum.date(dtv.year, dtv.month, dtv.day)  # type: ignore[union-attr]
```

### Comparing `dlt-0.4.9a1/dlt/common/typing.py` & `dlt-0.4.9a2/dlt/common/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/utils.py` & `dlt-0.4.9a2/dlt/common/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/validation.py` & `dlt-0.4.9a2/dlt/common/validation.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/versioned_state.py` & `dlt-0.4.9a2/dlt/common/versioned_state.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/warnings.py` & `dlt-0.4.9a2/dlt/common/warnings.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/common/wei.py` & `dlt-0.4.9a2/dlt/common/wei.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/__init__.py` & `dlt-0.4.9a2/dlt/destinations/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/decorators.py` & `dlt-0.4.9a2/dlt/destinations/decorators.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/exceptions.py` & `dlt-0.4.9a2/dlt/destinations/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/athena/__init__.py` & `dlt-0.4.9a2/dlt/destinations/impl/athena/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/athena/athena.py` & `dlt-0.4.9a2/dlt/destinations/impl/athena/athena.py`

 * *Files 1% similar despite different names*

```diff
@@ -363,15 +363,15 @@
         if generate_alter:
             # alter table to add new columns at the end
             sql.append(f"""ALTER TABLE {qualified_table_name} ADD COLUMNS ({columns});""")
         else:
             if is_iceberg:
                 sql.append(f"""CREATE TABLE {qualified_table_name}
                         ({columns})
-                        LOCATION '{location}'
+                        LOCATION '{location.rstrip('/')}'
                         TBLPROPERTIES ('table_type'='ICEBERG', 'format'='parquet');""")
             elif table_format == "jsonl":
                 sql.append(f"""CREATE EXTERNAL TABLE {qualified_table_name}
                         ({columns})
                         ROW FORMAT SERDE 'org.openx.data.jsonserde.JsonSerDe'
                         LOCATION '{location}';""")
             else:
```

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/athena/configuration.py` & `dlt-0.4.9a2/dlt/destinations/impl/athena/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/athena/factory.py` & `dlt-0.4.9a2/dlt/destinations/impl/athena/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/bigquery/__init__.py` & `dlt-0.4.9a2/dlt/destinations/impl/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/bigquery/bigquery.py` & `dlt-0.4.9a2/dlt/destinations/impl/bigquery/bigquery.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/bigquery/bigquery_adapter.py` & `dlt-0.4.9a2/dlt/destinations/impl/bigquery/bigquery_adapter.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/bigquery/configuration.py` & `dlt-0.4.9a2/dlt/destinations/impl/bigquery/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/bigquery/factory.py` & `dlt-0.4.9a2/dlt/destinations/impl/bigquery/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/bigquery/sql_client.py` & `dlt-0.4.9a2/dlt/destinations/impl/bigquery/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/databricks/__init__.py` & `dlt-0.4.9a2/dlt/destinations/impl/databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/databricks/configuration.py` & `dlt-0.4.9a2/dlt/destinations/impl/databricks/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/databricks/databricks.py` & `dlt-0.4.9a2/dlt/destinations/impl/databricks/databricks.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/databricks/factory.py` & `dlt-0.4.9a2/dlt/destinations/impl/databricks/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/databricks/sql_client.py` & `dlt-0.4.9a2/dlt/destinations/impl/databricks/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/destination/__init__.py` & `dlt-0.4.9a2/dlt/destinations/impl/destination/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/destination/configuration.py` & `dlt-0.4.9a2/dlt/destinations/impl/destination/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/destination/destination.py` & `dlt-0.4.9a2/dlt/destinations/impl/destination/destination.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,17 @@
     def is_storage_initialized(self) -> bool:
         return True
 
     def drop_storage(self) -> None:
         pass
 
     def update_stored_schema(
-        self, only_tables: Iterable[str] = None, expected_update: TSchemaTables = None
+        self,
+        only_tables: Iterable[str] = None,
+        expected_update: TSchemaTables = None,
     ) -> Optional[TSchemaTables]:
         return super().update_stored_schema(only_tables, expected_update)
 
     def start_file_load(self, table: TTableSchema, file_path: str, load_id: str) -> LoadJob:
         # skip internal tables and remove columns from schema if so configured
         skipped_columns: List[str] = []
         if self.config.skip_dlt_columns_and_tables:
```

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/destination/factory.py` & `dlt-0.4.9a2/dlt/destinations/impl/destination/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/dremio/__init__.py` & `dlt-0.4.9a2/dlt/destinations/impl/dremio/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/dremio/configuration.py` & `dlt-0.4.9a2/dlt/destinations/impl/dremio/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/dremio/dremio.py` & `dlt-0.4.9a2/dlt/destinations/impl/dremio/dremio.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/dremio/factory.py` & `dlt-0.4.9a2/dlt/destinations/impl/dremio/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/dremio/pydremio.py` & `dlt-0.4.9a2/dlt/destinations/impl/dremio/pydremio.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/dremio/sql_client.py` & `dlt-0.4.9a2/dlt/destinations/impl/dremio/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/duckdb/__init__.py` & `dlt-0.4.9a2/dlt/destinations/impl/duckdb/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/duckdb/configuration.py` & `dlt-0.4.9a2/dlt/destinations/impl/duckdb/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/duckdb/duck.py` & `dlt-0.4.9a2/dlt/destinations/impl/duckdb/duck.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/duckdb/factory.py` & `dlt-0.4.9a2/dlt/destinations/impl/duckdb/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/duckdb/sql_client.py` & `dlt-0.4.9a2/dlt/destinations/impl/duckdb/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/dummy/__init__.py` & `dlt-0.4.9a2/dlt/destinations/impl/dummy/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/dummy/configuration.py` & `dlt-0.4.9a2/dlt/destinations/impl/dummy/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/dummy/dummy.py` & `dlt-0.4.9a2/dlt/destinations/impl/dummy/dummy.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,17 @@
     def is_storage_initialized(self) -> bool:
         return True
 
     def drop_storage(self) -> None:
         pass
 
     def update_stored_schema(
-        self, only_tables: Iterable[str] = None, expected_update: TSchemaTables = None
+        self,
+        only_tables: Iterable[str] = None,
+        expected_update: TSchemaTables = None,
     ) -> Optional[TSchemaTables]:
         applied_update = super().update_stored_schema(only_tables, expected_update)
         if self.config.fail_schema_update:
             raise DestinationTransientException(
                 "Raise on schema update due to fail_schema_update config flag"
             )
         return applied_update
```

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/dummy/factory.py` & `dlt-0.4.9a2/dlt/destinations/impl/dummy/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/filesystem/configuration.py` & `dlt-0.4.9a2/dlt/destinations/impl/filesystem/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/filesystem/factory.py` & `dlt-0.4.9a2/dlt/destinations/impl/filesystem/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/filesystem/typing.py` & `dlt-0.4.9a2/dlt/destinations/impl/filesystem/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/motherduck/__init__.py` & `dlt-0.4.9a2/dlt/destinations/impl/motherduck/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/motherduck/configuration.py` & `dlt-0.4.9a2/dlt/destinations/impl/motherduck/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/motherduck/factory.py` & `dlt-0.4.9a2/dlt/destinations/impl/motherduck/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/motherduck/motherduck.py` & `dlt-0.4.9a2/dlt/destinations/impl/motherduck/motherduck.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/motherduck/sql_client.py` & `dlt-0.4.9a2/dlt/destinations/impl/motherduck/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/mssql/__init__.py` & `dlt-0.4.9a2/dlt/destinations/impl/mssql/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/mssql/configuration.py` & `dlt-0.4.9a2/dlt/destinations/impl/mssql/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/mssql/factory.py` & `dlt-0.4.9a2/dlt/destinations/impl/mssql/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/mssql/mssql.py` & `dlt-0.4.9a2/dlt/destinations/impl/mssql/mssql.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/mssql/sql_client.py` & `dlt-0.4.9a2/dlt/destinations/impl/mssql/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/postgres/__init__.py` & `dlt-0.4.9a2/dlt/destinations/impl/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/postgres/configuration.py` & `dlt-0.4.9a2/dlt/destinations/impl/postgres/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/postgres/factory.py` & `dlt-0.4.9a2/dlt/destinations/impl/postgres/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/postgres/postgres.py` & `dlt-0.4.9a2/dlt/destinations/impl/postgres/postgres.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/postgres/sql_client.py` & `dlt-0.4.9a2/dlt/destinations/impl/postgres/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/qdrant/__init__.py` & `dlt-0.4.9a2/dlt/destinations/impl/qdrant/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/qdrant/configuration.py` & `dlt-0.4.9a2/dlt/destinations/impl/qdrant/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/qdrant/factory.py` & `dlt-0.4.9a2/dlt/destinations/impl/qdrant/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/qdrant/qdrant_adapter.py` & `dlt-0.4.9a2/dlt/destinations/impl/qdrant/qdrant_adapter.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/qdrant/qdrant_client.py` & `dlt-0.4.9a2/dlt/destinations/impl/qdrant/qdrant_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,15 +279,17 @@
         self._create_collection(full_collection_name=self.sentinel_collection)
 
     def _delete_sentinel_collection(self) -> None:
         """Delete the sentinel collection."""
         self.db_client.delete_collection(self.sentinel_collection)
 
     def update_stored_schema(
-        self, only_tables: Iterable[str] = None, expected_update: TSchemaTables = None
+        self,
+        only_tables: Iterable[str] = None,
+        expected_update: TSchemaTables = None,
     ) -> Optional[TSchemaTables]:
         super().update_stored_schema(only_tables, expected_update)
         applied_update: TSchemaTables = {}
         schema_info = self.get_stored_schema_by_hash(self.schema.stored_version_hash)
         if schema_info is None:
             logger.info(
                 f"Schema with hash {self.schema.stored_version_hash} "
```

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/redshift/README.md` & `dlt-0.4.9a2/dlt/destinations/impl/redshift/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/redshift/__init__.py` & `dlt-0.4.9a2/dlt/destinations/impl/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/redshift/configuration.py` & `dlt-0.4.9a2/dlt/destinations/impl/redshift/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/redshift/factory.py` & `dlt-0.4.9a2/dlt/destinations/impl/redshift/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/redshift/redshift.py` & `dlt-0.4.9a2/dlt/destinations/impl/redshift/redshift.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/snowflake/__init__.py` & `dlt-0.4.9a2/dlt/destinations/impl/snowflake/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/snowflake/configuration.py` & `dlt-0.4.9a2/dlt/destinations/impl/snowflake/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/snowflake/factory.py` & `dlt-0.4.9a2/dlt/destinations/impl/snowflake/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/snowflake/snowflake.py` & `dlt-0.4.9a2/dlt/destinations/impl/snowflake/snowflake.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/snowflake/sql_client.py` & `dlt-0.4.9a2/dlt/destinations/impl/snowflake/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/synapse/__init__.py` & `dlt-0.4.9a2/dlt/destinations/impl/synapse/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/synapse/configuration.py` & `dlt-0.4.9a2/dlt/destinations/impl/synapse/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/synapse/factory.py` & `dlt-0.4.9a2/dlt/destinations/impl/synapse/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/synapse/sql_client.py` & `dlt-0.4.9a2/dlt/destinations/impl/synapse/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/synapse/synapse.py` & `dlt-0.4.9a2/dlt/destinations/impl/synapse/synapse.py`

 * *Files 13% similar despite different names*

```diff
@@ -123,39 +123,22 @@
         elif c["data_type"] in varbinary_source_types and "precision" not in c:
             return {**c, **{"precision": VARBINARY_MAX_N}}
         return c
 
     def _create_replace_followup_jobs(
         self, table_chain: Sequence[TTableSchema]
     ) -> List[NewLoadJob]:
-        if self.config.replace_strategy == "staging-optimized":
-            # we must recreate staging table after SCHEMA TRANSFER
-            job_params: SqlJobParams = {"table_chain_create_table_statements": {}}
-            create_statements = job_params["table_chain_create_table_statements"]
-            with self.with_staging_dataset():
-                for table in table_chain:
-                    columns = [c for c in self.schema.get_table_columns(table["name"]).values()]
-                    # generate CREATE TABLE statement
-                    create_statements[table["name"]] = self._get_table_update_sql(
-                        table["name"], columns, generate_alter=False
-                    )
-            return [
-                SynapseStagingCopyJob.from_table_chain(table_chain, self.sql_client, job_params)
-            ]
-        return super()._create_replace_followup_jobs(table_chain)
+        return SqlJobClientBase._create_replace_followup_jobs(self, table_chain)
 
     def prepare_load_table(self, table_name: str, staging: bool = False) -> TTableSchema:
         table = super().prepare_load_table(table_name, staging)
         if staging and self.config.replace_strategy == "insert-from-staging":
             # Staging tables should always be heap tables, because "when you are
             # temporarily landing data in dedicated SQL pool, you may find that
             # using a heap table makes the overall process faster."
-            # "staging-optimized" is not included, because in that strategy the
-            # staging table becomes the final table, so we should already create
-            # it with the desired index type.
             table[TABLE_INDEX_TYPE_HINT] = "heap"  # type: ignore[typeddict-unknown-key]
         elif table_name in self.schema.dlt_table_names():
             # dlt tables should always be heap tables, because "for small lookup
             # tables, less than 60 million rows, consider using HEAP or clustered
             # index for faster query performance."
             table[TABLE_INDEX_TYPE_HINT] = "heap"  # type: ignore[typeddict-unknown-key]
         # https://learn.microsoft.com/en-us/azure/synapse-analytics/sql-data-warehouse/sql-data-warehouse-tables-index#heap-tables
@@ -182,40 +165,14 @@
                 self.sql_client,
                 cast(AzureCredentialsWithoutDefaults, self.config.staging_config.credentials),
                 self.config.staging_use_msi,
             )
         return job
 
 
-class SynapseStagingCopyJob(SqlStagingCopyJob):
-    @classmethod
-    def generate_sql(
-        cls,
-        table_chain: Sequence[TTableSchema],
-        sql_client: SqlClientBase[Any],
-        params: Optional[SqlJobParams] = None,
-    ) -> List[str]:
-        sql: List[str] = []
-        for table in table_chain:
-            with sql_client.with_staging_dataset(staging=True):
-                staging_table_name = sql_client.make_qualified_table_name(table["name"])
-            table_name = sql_client.make_qualified_table_name(table["name"])
-            # drop destination table
-            sql.append(f"DROP TABLE {table_name};")
-            # moving staging table to destination schema
-            sql.append(
-                f"ALTER SCHEMA {sql_client.fully_qualified_dataset_name()} TRANSFER"
-                f" {staging_table_name};"
-            )
-            # recreate staging table
-            sql.extend(params["table_chain_create_table_statements"][table["name"]])
-
-        return sql
-
-
 class SynapseCopyFileLoadJob(CopyRemoteFileLoadJob):
     def __init__(
         self,
         table: TTableSchema,
         file_path: str,
         sql_client: SqlClientBase[Any],
         staging_credentials: Optional[AzureCredentialsWithoutDefaults] = None,
```

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/synapse/synapse_adapter.py` & `dlt-0.4.9a2/dlt/destinations/impl/synapse/synapse_adapter.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/weaviate/README.md` & `dlt-0.4.9a2/dlt/destinations/impl/weaviate/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/weaviate/__init__.py` & `dlt-0.4.9a2/dlt/destinations/impl/weaviate/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/weaviate/configuration.py` & `dlt-0.4.9a2/dlt/destinations/impl/weaviate/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/weaviate/exceptions.py` & `dlt-0.4.9a2/dlt/destinations/impl/weaviate/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/weaviate/factory.py` & `dlt-0.4.9a2/dlt/destinations/impl/weaviate/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/weaviate/naming.py` & `dlt-0.4.9a2/dlt/destinations/impl/weaviate/naming.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/weaviate/weaviate_adapter.py` & `dlt-0.4.9a2/dlt/destinations/impl/weaviate/weaviate_adapter.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/impl/weaviate/weaviate_client.py` & `dlt-0.4.9a2/dlt/destinations/impl/weaviate/weaviate_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -420,15 +420,17 @@
 
     def _delete_sentinel_class(self) -> None:
         """Delete the sentinel class."""
         self.db_client.schema.delete_class(self.sentinel_class)
 
     @wrap_weaviate_error
     def update_stored_schema(
-        self, only_tables: Iterable[str] = None, expected_update: TSchemaTables = None
+        self,
+        only_tables: Iterable[str] = None,
+        expected_update: TSchemaTables = None,
     ) -> Optional[TSchemaTables]:
         super().update_stored_schema(only_tables, expected_update)
         # Retrieve the schema from Weaviate
         applied_update: TSchemaTables = {}
         try:
             schema_info = self.get_stored_schema_by_hash(self.schema.stored_version_hash)
         except DestinationUndefinedEntity:
@@ -520,25 +522,14 @@
                     properties=["load_id", "status"],
                 )
                 # if there is a load for this state which was successful, return the state
                 if len(load_records):
                     state["dlt_load_id"] = state.pop("_dlt_load_id")
                     return StateInfo(**state)
 
-    # def get_stored_states(self, state_table: str) -> List[StateInfo]:
-    #     state_records = self.get_records(state_table,
-    #         sort={
-    #             "path": ["created_at"],
-    #             "order": "desc"
-    #         }, properties=self.state_properties)
-
-    #     for state in state_records:
-    #         state["dlt_load_id"] = state.pop("_dlt_load_id")
-    #     return [StateInfo(**state) for state in state_records]
-
     def get_stored_schema(self) -> Optional[StorageSchemaInfo]:
         """Retrieves newest schema from destination storage"""
         try:
             record = self.get_records(
                 self.schema.version_table_name,
                 sort={"path": ["inserted_at"], "order": "desc"},
                 where={
```

### Comparing `dlt-0.4.9a1/dlt/destinations/insert_job_client.py` & `dlt-0.4.9a2/dlt/destinations/insert_job_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/job_client_impl.py` & `dlt-0.4.9a2/dlt/destinations/job_client_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,17 @@
         elif truncate_tables:
             self.sql_client.truncate_tables(*truncate_tables)
 
     def is_storage_initialized(self) -> bool:
         return self.sql_client.has_dataset()
 
     def update_stored_schema(
-        self, only_tables: Iterable[str] = None, expected_update: TSchemaTables = None
+        self,
+        only_tables: Iterable[str] = None,
+        expected_update: TSchemaTables = None,
     ) -> Optional[TSchemaTables]:
         super().update_stored_schema(only_tables, expected_update)
         applied_update: TSchemaTables = {}
         schema_info = self.get_stored_schema_by_hash(self.schema.stored_version_hash)
         if schema_info is None:
             logger.info(
                 f"Schema with hash {self.schema.stored_version_hash} not found in the storage."
@@ -369,23 +371,14 @@
         )
         with self.sql_client.execute_query(query, pipeline_name) as cur:
             row = cur.fetchone()
         if not row:
             return None
         return StateInfo(row[0], row[1], row[2], row[3], pendulum.instance(row[4]))
 
-    # def get_stored_states(self, state_table: str) -> List[StateInfo]:
-    #     """Loads list of compressed states from destination storage, optionally filtered by pipeline name"""
-    #     query = f"SELECT {self.STATE_TABLE_COLUMNS} FROM {state_table} AS s ORDER BY created_at DESC"
-    #     result: List[StateInfo] = []
-    #     with self.sql_client.execute_query(query) as cur:
-    #         for row in cur.fetchall():
-    #             result.append(StateInfo(row[0], row[1], row[2], row[3], pendulum.instance(row[4])))
-    #     return result
-
     def get_stored_schema_by_hash(self, version_hash: str) -> StorageSchemaInfo:
         name = self.sql_client.make_qualified_table_name(self.schema.version_table_name)
         query = f"SELECT {self.version_table_schema_columns} FROM {name} WHERE version_hash = %s;"
         return self._row_to_schema_info(query, version_hash)
 
     def _execute_schema_update_sql(self, only_tables: Iterable[str]) -> TSchemaTables:
         sql_scripts, schema_update = self._build_schema_update_sql(only_tables)
```

### Comparing `dlt-0.4.9a1/dlt/destinations/job_impl.py` & `dlt-0.4.9a2/dlt/destinations/job_impl.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/path_utils.py` & `dlt-0.4.9a2/dlt/destinations/path_utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/sql_client.py` & `dlt-0.4.9a2/dlt/destinations/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/sql_jobs.py` & `dlt-0.4.9a2/dlt/destinations/sql_jobs.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/type_mapping.py` & `dlt-0.4.9a2/dlt/destinations/type_mapping.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/destinations/typing.py` & `dlt-0.4.9a2/dlt/destinations/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/extract/__init__.py` & `dlt-0.4.9a2/dlt/extract/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/extract/concurrency.py` & `dlt-0.4.9a2/dlt/extract/concurrency.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/extract/decorators.py` & `dlt-0.4.9a2/dlt/extract/decorators.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/extract/exceptions.py` & `dlt-0.4.9a2/dlt/extract/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/extract/extract.py` & `dlt-0.4.9a2/dlt/extract/extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,25 +13,32 @@
     ExtractDataInfo,
     ExtractInfo,
     ExtractMetrics,
     SupportsPipeline,
     WithStepInfo,
     reset_resource_state,
 )
+from dlt.common.typing import DictStrAny
 from dlt.common.runtime import signals
 from dlt.common.runtime.collector import Collector, NULL_COLLECTOR
 from dlt.common.schema import Schema, utils
 from dlt.common.schema.typing import (
     TAnySchemaColumns,
     TColumnNames,
     TSchemaContract,
     TWriteDispositionConfig,
 )
 from dlt.common.storages import NormalizeStorageConfiguration, LoadPackageInfo, SchemaStorage
-from dlt.common.storages.load_package import ParsedLoadJobFileName
+from dlt.common.storages.load_package import (
+    ParsedLoadJobFileName,
+    LoadPackageStateInjectableContext,
+    TPipelineStateDoc,
+)
+
+
 from dlt.common.utils import get_callable_name, get_full_class_name
 
 from dlt.extract.decorators import SourceInjectableContext, SourceSchemaInjectableContext
 from dlt.extract.exceptions import DataItemRequiredForDynamicTableHints
 from dlt.extract.incremental import IncrementalResourceWrapper
 from dlt.extract.pipe_iterator import PipeIterator
 from dlt.extract.source import DltSource
@@ -363,15 +370,21 @@
         max_parallel_items: int,
         workers: int,
     ) -> str:
         # generate load package to be able to commit all the sources together later
         load_id = self.extract_storage.create_load_package(source.discover_schema())
         with Container().injectable_context(
             SourceSchemaInjectableContext(source.schema)
-        ), Container().injectable_context(SourceInjectableContext(source)):
+        ), Container().injectable_context(
+            SourceInjectableContext(source)
+        ), Container().injectable_context(
+            LoadPackageStateInjectableContext(
+                storage=self.extract_storage.new_packages, load_id=load_id
+            )
+        ):
             # inject the config section with the current source name
             with inject_section(
                 ConfigSectionContext(
                     sections=(known_sections.SOURCES, source.section, source.name),
                     source_state_key=source.name,
                 )
             ):
@@ -385,18 +398,22 @@
                     load_id,
                     source,
                     max_parallel_items=max_parallel_items,
                     workers=workers,
                 )
         return load_id
 
-    def commit_packages(self) -> None:
-        """Commits all extracted packages to normalize storage"""
+    def commit_packages(self, pipline_state_doc: TPipelineStateDoc = None) -> None:
+        """Commits all extracted packages to normalize storage, and adds the pipeline state to the load package"""
         # commit load packages
         for load_id, metrics in self._load_id_metrics.items():
+            if pipline_state_doc:
+                package_state = self.extract_storage.new_packages.get_load_package_state(load_id)
+                package_state["pipeline_state"] = {**pipline_state_doc, "dlt_load_id": load_id}
+                self.extract_storage.new_packages.save_load_package_state(load_id, package_state)
             self.extract_storage.commit_new_load_package(
                 load_id, self.schema_storage[metrics[0]["schema_name"]]
             )
         # all load ids got processed, cleanup empty folder
         self.extract_storage.delete_empty_extract_folder()
 
     def get_step_info(self, pipeline: SupportsPipeline) -> ExtractInfo:
```

### Comparing `dlt-0.4.9a1/dlt/extract/extractors.py` & `dlt-0.4.9a2/dlt/extract/extractors.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/extract/hints.py` & `dlt-0.4.9a2/dlt/extract/hints.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/extract/incremental/__init__.py` & `dlt-0.4.9a2/dlt/extract/incremental/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/extract/incremental/exceptions.py` & `dlt-0.4.9a2/dlt/extract/incremental/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/extract/incremental/transform.py` & `dlt-0.4.9a2/dlt/extract/incremental/transform.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/extract/items.py` & `dlt-0.4.9a2/dlt/extract/items.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/extract/pipe.py` & `dlt-0.4.9a2/dlt/extract/pipe.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/extract/pipe_iterator.py` & `dlt-0.4.9a2/dlt/extract/pipe_iterator.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/extract/resource.py` & `dlt-0.4.9a2/dlt/extract/resource.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/extract/source.py` & `dlt-0.4.9a2/dlt/extract/source.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/extract/storage.py` & `dlt-0.4.9a2/dlt/extract/storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/extract/utils.py` & `dlt-0.4.9a2/dlt/extract/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/extract/validation.py` & `dlt-0.4.9a2/dlt/extract/validation.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/extract/wrappers.py` & `dlt-0.4.9a2/dlt/extract/wrappers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/helpers/airflow_helper.py` & `dlt-0.4.9a2/dlt/helpers/airflow_helper.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/helpers/dbt/__init__.py` & `dlt-0.4.9a2/dlt/helpers/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/helpers/dbt/configuration.py` & `dlt-0.4.9a2/dlt/helpers/dbt/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/helpers/dbt/dbt_utils.py` & `dlt-0.4.9a2/dlt/helpers/dbt/dbt_utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/helpers/dbt/exceptions.py` & `dlt-0.4.9a2/dlt/helpers/dbt/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/helpers/dbt/profiles.yml` & `dlt-0.4.9a2/dlt/helpers/dbt/profiles.yml`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/helpers/dbt/runner.py` & `dlt-0.4.9a2/dlt/helpers/dbt/runner.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/helpers/dbt_cloud/__init__.py` & `dlt-0.4.9a2/dlt/helpers/dbt_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/helpers/dbt_cloud/client.py` & `dlt-0.4.9a2/dlt/helpers/dbt_cloud/client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/helpers/dbt_cloud/configuration.py` & `dlt-0.4.9a2/dlt/helpers/dbt_cloud/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/helpers/streamlit_app/blocks/load_info.py` & `dlt-0.4.9a2/dlt/helpers/streamlit_app/blocks/load_info.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/helpers/streamlit_app/blocks/query.py` & `dlt-0.4.9a2/dlt/helpers/streamlit_app/blocks/query.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/helpers/streamlit_app/blocks/resource_state.py` & `dlt-0.4.9a2/dlt/helpers/streamlit_app/blocks/resource_state.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/helpers/streamlit_app/blocks/show_data.py` & `dlt-0.4.9a2/dlt/helpers/streamlit_app/blocks/show_data.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/helpers/streamlit_app/blocks/table_hints.py` & `dlt-0.4.9a2/dlt/helpers/streamlit_app/blocks/table_hints.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/helpers/streamlit_app/pages/dashboard.py` & `dlt-0.4.9a2/dlt/helpers/streamlit_app/pages/dashboard.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/helpers/streamlit_app/pages/load_info.py` & `dlt-0.4.9a2/dlt/helpers/streamlit_app/pages/load_info.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/helpers/streamlit_app/theme.py` & `dlt-0.4.9a2/dlt/helpers/streamlit_app/theme.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/helpers/streamlit_app/utils.py` & `dlt-0.4.9a2/dlt/helpers/streamlit_app/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/helpers/streamlit_app/widgets/color_mode_selector.py` & `dlt-0.4.9a2/dlt/helpers/streamlit_app/widgets/color_mode_selector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/helpers/streamlit_app/widgets/logo.py` & `dlt-0.4.9a2/dlt/helpers/streamlit_app/widgets/logo.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/helpers/streamlit_app/widgets/schema.py` & `dlt-0.4.9a2/dlt/helpers/streamlit_app/widgets/schema.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/helpers/streamlit_app/widgets/stats.py` & `dlt-0.4.9a2/dlt/helpers/streamlit_app/widgets/stats.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/helpers/streamlit_app/widgets/summary.py` & `dlt-0.4.9a2/dlt/helpers/streamlit_app/widgets/summary.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/helpers/streamlit_app/widgets/tags.py` & `dlt-0.4.9a2/dlt/helpers/streamlit_app/widgets/tags.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/load/configuration.py` & `dlt-0.4.9a2/dlt/load/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/load/exceptions.py` & `dlt-0.4.9a2/dlt/load/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/load/load.py` & `dlt-0.4.9a2/dlt/load/load.py`

 * *Files 1% similar despite different names*

```diff
@@ -337,15 +337,21 @@
 
         return remaining_jobs
 
     def complete_package(self, load_id: str, schema: Schema, aborted: bool = False) -> None:
         # do not commit load id for aborted packages
         if not aborted:
             with self.get_destination_client(schema) as job_client:
-                job_client.complete_load(load_id)
+                with Container().injectable_context(
+                    LoadPackageStateInjectableContext(
+                        storage=self.load_storage.normalized_packages,
+                        load_id=load_id,
+                    )
+                ):
+                    job_client.complete_load(load_id)
         self.load_storage.complete_load_package(load_id, aborted)
         # collect package info
         self._loaded_packages.append(self.load_storage.get_load_package_info(load_id))
         self._step_info_complete_load_id(load_id, metrics={"started_at": None, "finished_at": None})
         # delete jobs only now
         self.load_storage.maybe_remove_completed_jobs(load_id)
         logger.info(
@@ -465,18 +471,17 @@
 
         # load the schema from the package
         load_id = loads[0]
         logger.info(f"Loading schema from load package in {load_id}")
         schema = self.load_storage.normalized_packages.load_schema(load_id)
         logger.info(f"Loaded schema name {schema.name} and version {schema.stored_version}")
 
-        container = Container()
         # get top load id and mark as being processed
         with self.collector(f"Load {schema.name} in {load_id}"):
-            with container.injectable_context(
+            with Container().injectable_context(
                 LoadPackageStateInjectableContext(
                     storage=self.load_storage.normalized_packages,
                     load_id=load_id,
                 )
             ):
                 # the same load id may be processed across multiple runs
                 if not self.current_load_id:
```

### Comparing `dlt-0.4.9a1/dlt/load/utils.py` & `dlt-0.4.9a2/dlt/load/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/normalize/configuration.py` & `dlt-0.4.9a2/dlt/normalize/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/normalize/exceptions.py` & `dlt-0.4.9a2/dlt/normalize/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/normalize/items_normalizers.py` & `dlt-0.4.9a2/dlt/normalize/items_normalizers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/normalize/normalize.py` & `dlt-0.4.9a2/dlt/normalize/normalize.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/pipeline/__init__.py` & `dlt-0.4.9a2/dlt/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/pipeline/configuration.py` & `dlt-0.4.9a2/dlt/pipeline/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/pipeline/current.py` & `dlt-0.4.9a2/dlt/pipeline/current.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/pipeline/dbt.py` & `dlt-0.4.9a2/dlt/pipeline/dbt.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/pipeline/exceptions.py` & `dlt-0.4.9a2/dlt/pipeline/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/pipeline/helpers.py` & `dlt-0.4.9a2/dlt/pipeline/helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/pipeline/pipeline.py` & `dlt-0.4.9a2/dlt/pipeline/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,15 @@
     NormalizeStorageConfiguration,
     SchemaStorageConfiguration,
     LoadStorageConfiguration,
     PackageStorage,
     LoadJobInfo,
     LoadPackageInfo,
 )
+from dlt.common.storages.load_package import TPipelineStateDoc
 from dlt.common.destination import (
     DestinationCapabilitiesContext,
     merge_caps_file_formats,
     TDestination,
     ALL_SUPPORTED_FILE_FORMATS,
     TLoaderFileFormat,
 )
@@ -134,14 +135,15 @@
 from dlt.pipeline.state_sync import (
     PIPELINE_STATE_ENGINE_VERSION,
     bump_pipeline_state_version_if_modified,
     load_pipeline_state_from_destination,
     mark_state_extracted,
     migrate_pipeline_state,
     state_resource,
+    state_doc,
     default_pipeline_state,
 )
 from dlt.pipeline.warnings import credentials_argument_deprecated
 from dlt.common.storages.load_package import TLoadPackageState
 
 
 def with_state_sync(may_extract_state: bool = False) -> Callable[[TFun], TFun]:
@@ -423,21 +425,22 @@
                     primary_key,
                     schema_contract,
                 ):
                     if source.exhausted:
                         raise SourceExhausted(source.name)
                     self._extract_source(extract_step, source, max_parallel_items, workers)
                 # extract state
+                state: TPipelineStateDoc = None
                 if self.config.restore_from_destination:
                     # this will update state version hash so it will not be extracted again by with_state_sync
-                    self._bump_version_and_extract_state(
+                    state = self._bump_version_and_extract_state(
                         self._container[StateInjectableContext].state, True, extract_step
                     )
-                # commit load packages
-                extract_step.commit_packages()
+                # commit load packages with state
+                extract_step.commit_packages(state)
                 return self._get_step_info(extract_step)
         except Exception as exc:
             # emit step info
             step_info = self._get_step_info(extract_step)
             current_load_id = step_info.loads_ids[-1] if len(step_info.loads_ids) > 0 else None
             raise PipelineStepFailed(
                 self,
@@ -724,15 +727,14 @@
                                 f" {remote_state['pipeline_name']}",
                             )
                         # if state was modified force get all schemas
                         restored_schemas = self._get_schemas_from_destination(
                             remote_state["schema_names"], always_download=True
                         )
                         # TODO: we should probably wipe out pipeline here
-
                 # if we didn't full refresh schemas, get only missing schemas
                 if restored_schemas is None:
                     restored_schemas = self._get_schemas_from_destination(
                         state["schema_names"], always_download=False
                     )
                 # commit all the changes locally
                 if state_changed:
@@ -1509,34 +1511,36 @@
             state["staging_type"] = self.staging.destination_type
             state["staging_name"] = self.staging.destination_name
         state["schema_names"] = self._list_schemas_sorted()
         return state
 
     def _bump_version_and_extract_state(
         self, state: TPipelineState, extract_state: bool, extract: Extract = None
-    ) -> None:
+    ) -> TPipelineStateDoc:
         """Merges existing state into `state` and extracts state using `storage` if extract_state is True.
 
         Storage will be created on demand. In that case the extracted package will be immediately committed.
         """
         _, hash_, _ = bump_pipeline_state_version_if_modified(self._props_to_state(state))
         should_extract = hash_ != state["_local"].get("_last_extracted_hash")
         if should_extract and extract_state:
-            data = state_resource(state)
+            data, doc = state_resource(state)
             extract_ = extract or Extract(
                 self._schema_storage, self._normalize_storage_config(), original_data=data
             )
             self._extract_source(
                 extract_, data_to_sources(data, self, self.default_schema)[0], 1, 1
             )
             # set state to be extracted
             mark_state_extracted(state, hash_)
             # commit only if we created storage
             if not extract:
-                extract_.commit_packages()
+                extract_.commit_packages(doc)
+            return doc
+        return None
 
     def _list_schemas_sorted(self) -> List[str]:
         """Lists schema names sorted to have deterministic state"""
         return sorted(self._schema_storage.list_schemas())
 
     def _save_state(self, state: TPipelineState) -> None:
         self._pipeline_storage.save(Pipeline.STATE_FILE, json_encode_state(state))
```

### Comparing `dlt-0.4.9a1/dlt/pipeline/platform.py` & `dlt-0.4.9a2/dlt/pipeline/platform.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/pipeline/progress.py` & `dlt-0.4.9a2/dlt/pipeline/progress.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/pipeline/state_sync.py` & `dlt-0.4.9a2/dlt/pipeline/state_sync.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from copy import copy
 from typing import Tuple, cast
 
 import dlt
 from dlt.common.pendulum import pendulum
 from dlt.common.typing import DictStrAny
 from dlt.common.schema.typing import STATE_TABLE_NAME, TTableSchemaColumns
-from dlt.common.destination.reference import WithStateSync, Destination
+from dlt.common.destination.reference import WithStateSync, Destination, StateInfo
 from dlt.common.versioned_state import (
     generate_state_version_hash,
     bump_state_version_if_modified,
     default_versioned_state,
     compress_state,
     decompress_state,
 )
 from dlt.common.pipeline import TPipelineState
-
+from dlt.common.storages.load_package import TPipelineStateDoc
 from dlt.extract import DltResource
 
 from dlt.pipeline.exceptions import (
     PipelineStateEngineNoUpgradePathException,
 )
 
 PIPELINE_STATE_ENGINE_VERSION = 4
+LOAD_PACKAGE_STATE_KEY = "pipeline_state"
 
 # state table columns
 STATE_TABLE_COLUMNS: TTableSchemaColumns = {
     "version": {"name": "version", "data_type": "bigint", "nullable": False},
     "engine_version": {"name": "engine_version", "data_type": "bigint", "nullable": False},
     "pipeline_name": {"name": "pipeline_name", "data_type": "text", "nullable": False},
     "state": {"name": "state", "data_type": "text", "nullable": False},
@@ -89,28 +90,41 @@
         raise PipelineStateEngineNoUpgradePathException(
             pipeline_name, state["_state_engine_version"], from_engine, to_engine
         )
     state["_state_engine_version"] = from_engine
     return cast(TPipelineState, state)
 
 
-def state_resource(state: TPipelineState) -> DltResource:
+def state_doc(state: TPipelineState, load_id: str = None) -> TPipelineStateDoc:
     state = copy(state)
     state.pop("_local")
     state_str = compress_state(state)
-    state_doc = {
+    doc: TPipelineStateDoc = {
         "version": state["_state_version"],
         "engine_version": state["_state_engine_version"],
         "pipeline_name": state["pipeline_name"],
         "state": state_str,
         "created_at": pendulum.now(),
         "version_hash": state["_version_hash"],
     }
-    return dlt.resource(
-        [state_doc], name=STATE_TABLE_NAME, write_disposition="append", columns=STATE_TABLE_COLUMNS
+    if load_id:
+        doc["dlt_load_id"] = load_id
+    return doc
+
+
+def state_resource(state: TPipelineState) -> Tuple[DltResource, TPipelineStateDoc]:
+    doc = state_doc(state)
+    return (
+        dlt.resource(
+            [doc],
+            name=STATE_TABLE_NAME,
+            write_disposition="append",
+            columns=STATE_TABLE_COLUMNS,
+        ),
+        doc,
     )
 
 
 def load_pipeline_state_from_destination(
     pipeline_name: str, client: WithStateSync
 ) -> TPipelineState:
     # NOTE: if dataset or table holding state does not exist, the sql_client will rise DestinationUndefinedEntity. caller must handle this
```

### Comparing `dlt-0.4.9a1/dlt/pipeline/trace.py` & `dlt-0.4.9a2/dlt/pipeline/trace.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/pipeline/track.py` & `dlt-0.4.9a2/dlt/pipeline/track.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/pipeline/warnings.py` & `dlt-0.4.9a2/dlt/pipeline/warnings.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/reflection/names.py` & `dlt-0.4.9a2/dlt/reflection/names.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/reflection/script_inspector.py` & `dlt-0.4.9a2/dlt/reflection/script_inspector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/reflection/script_visitor.py` & `dlt-0.4.9a2/dlt/reflection/script_visitor.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/sources/credentials.py` & `dlt-0.4.9a2/dlt/sources/credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/sources/helpers/requests/__init__.py` & `dlt-0.4.9a2/dlt/sources/helpers/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/sources/helpers/requests/retry.py` & `dlt-0.4.9a2/dlt/sources/helpers/requests/retry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/sources/helpers/requests/session.py` & `dlt-0.4.9a2/dlt/sources/helpers/requests/session.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/sources/helpers/rest_client/__init__.py` & `dlt-0.4.9a2/dlt/sources/helpers/rest_client/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/sources/helpers/rest_client/auth.py` & `dlt-0.4.9a2/dlt/sources/helpers/rest_client/auth.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/sources/helpers/rest_client/client.py` & `dlt-0.4.9a2/dlt/sources/helpers/rest_client/client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/sources/helpers/rest_client/detector.py` & `dlt-0.4.9a2/dlt/sources/helpers/rest_client/detector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/sources/helpers/rest_client/paginators.py` & `dlt-0.4.9a2/dlt/sources/helpers/rest_client/paginators.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/sources/helpers/transform.py` & `dlt-0.4.9a2/dlt/sources/helpers/transform.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/dlt/version.py` & `dlt-0.4.9a2/dlt/version.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a1/pyproject.toml` & `dlt-0.4.9a2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dlt"
-version = "0.4.9a1"
+version = "0.4.9a2"
 description = "dlt is an open-source python-first scalable data loading library that does not require any backend to run."
 authors = ["dltHub Inc. <services@dlthub.com>"]
 maintainers = [ "Marcin Rudolf <marcin@dlthub.com>", "Adrian Brudaru <adrian@dlthub.com>", "Ty Dunn <ty@dlthub.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/dlt-hub"
 repository = "https://github.com/dlt-hub/dlt"
@@ -76,14 +76,15 @@
 pyathena = {version = ">=2.9.6", optional = true}
 weaviate-client = {version = ">=3.22", optional = true}
 adlfs = {version = ">=2022.4.0", optional = true}
 pyodbc = {version = "^4.0.39", optional = true}
 qdrant-client = {version = "^1.6.4", optional = true, extras = ["fastembed"]}
 databricks-sql-connector = {version = ">=2.9.3,<3.0.0", optional = true}
 dbt-databricks = {version = "^1.7.3", optional = true}
+black = "23.9.1"
 
 [tool.poetry.extras]
 dbt = ["dbt-core", "dbt-redshift", "dbt-bigquery", "dbt-duckdb", "dbt-snowflake", "dbt-athena-community", "dbt-databricks"]
 gcp = ["grpcio", "google-cloud-bigquery", "db-dtypes", "gcsfs"]
 # bigquery is alias on gcp extras
 bigquery = ["grpcio", "google-cloud-bigquery", "pyarrow", "db-dtypes", "gcsfs"]
 postgres = ["psycopg2-binary", "psycopg2cffi"]
```

### Comparing `dlt-0.4.9a1/PKG-INFO` & `dlt-0.4.9a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlt
-Version: 0.4.9a1
+Version: 0.4.9a2
 Summary: dlt is an open-source python-first scalable data loading library that does not require any backend to run.
 Home-page: https://github.com/dlt-hub
 License: Apache-2.0
 Keywords: etl
 Author: dltHub Inc.
 Author-email: services@dlthub.com
 Maintainer: Marcin Rudolf
@@ -42,14 +42,15 @@
 Provides-Extra: s3
 Provides-Extra: snowflake
 Provides-Extra: synapse
 Provides-Extra: weaviate
 Requires-Dist: PyYAML (>=5.4.1)
 Requires-Dist: adlfs (>=2022.4.0) ; extra == "az" or extra == "synapse"
 Requires-Dist: astunparse (>=1.6.3)
+Requires-Dist: black (==23.9.1)
 Requires-Dist: botocore (>=1.28) ; extra == "filesystem" or extra == "s3" or extra == "athena"
 Requires-Dist: click (>=7.1)
 Requires-Dist: cron-descriptor (>=1.2.32) ; extra == "cli"
 Requires-Dist: databricks-sql-connector (>=2.9.3,<3.0.0) ; extra == "databricks"
 Requires-Dist: dbt-athena-community (>=1.2.0) ; extra == "dbt"
 Requires-Dist: dbt-bigquery (>=1.2.0) ; extra == "dbt"
 Requires-Dist: dbt-core (>=1.2.0) ; extra == "dbt"
```

