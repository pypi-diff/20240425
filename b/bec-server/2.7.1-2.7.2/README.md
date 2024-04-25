# Comparing `tmp/bec_server-2.7.1.tar.gz` & `tmp/bec_server-2.7.2.tar.gz`

## Comparing `bec_server-2.7.1.tar` & `bec_server-2.7.2.tar`

### file list

```diff
@@ -1,114 +1,114 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.7.1/README.md
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/bec_server_utils/__init__.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/bec_server_utils/launch.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/bec_server_utils/service_handler.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/bec_server_utils/subprocess_launch.py
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/bec_server_utils/tmux_launch.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/data_processing/__init__.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/data_processing/dap_server.py
--rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/data_processing/dap_service.py
--rw-r--r--   0        0        0     9648 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/data_processing/dap_service_manager.py
--rw-r--r--   0        0        0    12174 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/data_processing/lmfit1d_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/data_processing/cli/__init__.py
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/data_processing/cli/launch.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/device_server/__init__.py
--rw-r--r--   0        0        0    18964 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/device_server/device_server.py
--rw-r--r--   0        0        0     7707 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/device_server/rpc_mixin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/device_server/cli/__init__.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/device_server/cli/launch.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/device_server/devices/__init__.py
--rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/device_server/devices/config_update_handler.py
--rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/device_server/devices/device_serializer.py
--rw-r--r--   0        0        0    22518 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/device_server/devices/devicemanager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/device_server/tests/__init__.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/device_server/tests/utils.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/file_writer/__init__.py
--rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/file_writer/default_writer.py
--rw-r--r--   0        0        0     8713 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/file_writer/file_writer.py
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/file_writer/file_writer_manager.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/file_writer/merged_dicts.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/file_writer/cli/__init__.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/file_writer/cli/launch.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/file_writer_plugins/__init__.py
--rw-r--r--   0        0        0    22190 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/file_writer_plugins/cSAXS.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/scan_bundler/__init__.py
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/scan_bundler/bec_emitter.py
--rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/scan_bundler/bluesky_emitter.py
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/scan_bundler/emitter.py
--rw-r--r--   0        0        0    15950 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/scan_bundler/scan_bundler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/scan_bundler/cli/__init__.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/scan_bundler/cli/launch.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/scan_server/__init__.py
--rw-r--r--   0        0        0     6531 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/scan_server/device_validation.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/scan_server/errors.py
--rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/scan_server/path_optimization.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/scan_server/scan_assembler.py
--rw-r--r--   0        0        0     6304 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/scan_server/scan_guard.py
--rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/scan_server/scan_manager.py
--rw-r--r--   0        0        0    34791 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/scan_server/scan_queue.py
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/scan_server/scan_server.py
--rw-r--r--   0        0        0    18416 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/scan_server/scan_stubs.py
--rw-r--r--   0        0        0    35666 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/scan_server/scan_worker.py
--rw-r--r--   0        0        0    52578 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/scan_server/scans.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/scan_server/cli/__init__.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/scan_server/cli/launch.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/scan_server/scan_plugins/__init__.py
--rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/scan_server/scan_plugins/otf_scan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/scan_server/tests/__init__.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/scan_server/tests/fixtures.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/scan_server/tests/utils.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/scihub/__init__.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/scihub/repeated_timer.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/scihub/scihub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/scihub/cli/__init__.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/scihub/cli/launch.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/scihub/scibec/__init__.py
--rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/scihub/scibec/config_handler.py
--rw-r--r--   0        0        0     7549 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/scihub/scibec/scibec_connector.py
--rw-r--r--   0        0        0    10557 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/scihub/scibec/scibec_metadata_handler.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/scihub/scilog/__init__.py
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 bec_server-2.7.1/bec_server/scihub/scilog/scilog.py
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_bec_server_utils/test_main.py
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_bec_server_utils/test_service_handler.py
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_bec_server_utils/test_tmux_launch.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_data_processing/conftest.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_data_processing/test_dap_cli_launch.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_data_processing/test_dap_server.py
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_data_processing/test_dap_service_manager.py
--rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_data_processing/test_lmfit1d_service.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_device_server/conftest.py
--rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_device_server/test_config_handler.py
--rw-r--r--   0        0        0     6020 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_device_server/test_device_manager_ds.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_device_server/test_device_serializer.py
--rw-r--r--   0        0        0    28297 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_device_server/test_device_server.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_device_server/test_device_server_cli_launch.py
--rw-r--r--   0        0        0     9555 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_device_server/test_rpc_mixin.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_file_writer/conftest.py
--rw-r--r--   0        0        0     6829 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_file_writer/test_file_writer.py
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_file_writer/test_file_writer_cli_launch.py
--rw-r--r--   0        0        0    11233 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_file_writer/test_file_writer_manager.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_scan_bundler/conftest.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_scan_bundler/test_bec_emitter.py
--rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_scan_bundler/test_bluesky_emitter.py
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_scan_bundler/test_emitter.py
--rw-r--r--   0        0        0    25541 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_scan_bundler/test_scan_bundler.py
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_scan_bundler/test_scan_bundler_cli_launch.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_scan_server/conftest.py
--rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_scan_server/test_path_optimization.py
--rw-r--r--   0        0        0    11602 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_scan_server/test_scan_guard.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_scan_server/test_scan_server_cli_launch.py
--rw-r--r--   0        0        0    26404 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_scan_server/test_scan_server_queue.py
--rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_scan_server/test_scan_stubs.py
--rw-r--r--   0        0        0    54003 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_scan_server/test_scan_worker.py
--rw-r--r--   0        0        0    87804 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_scan_server/test_scans.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_scihub/conftest.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_scihub/test_repeated_timer.py
--rw-r--r--   0        0        0    16951 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_scihub/test_scibec_config_handler.py
--rw-r--r--   0        0        0     5641 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_scihub/test_scibec_connector.py
--rw-r--r--   0        0        0     8663 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_scihub/test_scibec_metadata_handler.py
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_scihub/test_scihub_cli_launch.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 bec_server-2.7.1/tests/tests_scihub/test_scilog_connector.py
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 bec_server-2.7.1/.gitignore
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 bec_server-2.7.1/pyproject.toml
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 bec_server-2.7.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.7.2/README.md
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/bec_server_utils/__init__.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/bec_server_utils/launch.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/bec_server_utils/service_handler.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/bec_server_utils/subprocess_launch.py
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/bec_server_utils/tmux_launch.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/data_processing/__init__.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/data_processing/dap_server.py
+-rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/data_processing/dap_service.py
+-rw-r--r--   0        0        0     9648 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/data_processing/dap_service_manager.py
+-rw-r--r--   0        0        0    12174 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/data_processing/lmfit1d_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/data_processing/cli/__init__.py
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/data_processing/cli/launch.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/device_server/__init__.py
+-rw-r--r--   0        0        0    18964 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/device_server/device_server.py
+-rw-r--r--   0        0        0     7707 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/device_server/rpc_mixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/device_server/cli/__init__.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/device_server/cli/launch.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/device_server/devices/__init__.py
+-rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/device_server/devices/config_update_handler.py
+-rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/device_server/devices/device_serializer.py
+-rw-r--r--   0        0        0    22518 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/device_server/devices/devicemanager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/device_server/tests/__init__.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/device_server/tests/utils.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/file_writer/__init__.py
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/file_writer/default_writer.py
+-rw-r--r--   0        0        0     8713 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/file_writer/file_writer.py
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/file_writer/file_writer_manager.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/file_writer/merged_dicts.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/file_writer/cli/__init__.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/file_writer/cli/launch.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/file_writer_plugins/__init__.py
+-rw-r--r--   0        0        0    22190 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/file_writer_plugins/cSAXS.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/scan_bundler/__init__.py
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/scan_bundler/bec_emitter.py
+-rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/scan_bundler/bluesky_emitter.py
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/scan_bundler/emitter.py
+-rw-r--r--   0        0        0    15950 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/scan_bundler/scan_bundler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/scan_bundler/cli/__init__.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/scan_bundler/cli/launch.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/scan_server/__init__.py
+-rw-r--r--   0        0        0     6531 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/scan_server/device_validation.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/scan_server/errors.py
+-rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/scan_server/path_optimization.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/scan_server/scan_assembler.py
+-rw-r--r--   0        0        0     6304 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/scan_server/scan_guard.py
+-rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/scan_server/scan_manager.py
+-rw-r--r--   0        0        0    34791 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/scan_server/scan_queue.py
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/scan_server/scan_server.py
+-rw-r--r--   0        0        0    18416 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/scan_server/scan_stubs.py
+-rw-r--r--   0        0        0    35666 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/scan_server/scan_worker.py
+-rw-r--r--   0        0        0    52578 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/scan_server/scans.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/scan_server/cli/__init__.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/scan_server/cli/launch.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/scan_server/scan_plugins/__init__.py
+-rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/scan_server/scan_plugins/otf_scan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/scan_server/tests/__init__.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/scan_server/tests/fixtures.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/scan_server/tests/utils.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/scihub/__init__.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/scihub/repeated_timer.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/scihub/scihub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/scihub/cli/__init__.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/scihub/cli/launch.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/scihub/scibec/__init__.py
+-rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/scihub/scibec/config_handler.py
+-rw-r--r--   0        0        0     7549 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/scihub/scibec/scibec_connector.py
+-rw-r--r--   0        0        0    10557 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/scihub/scibec/scibec_metadata_handler.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/scihub/scilog/__init__.py
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 bec_server-2.7.2/bec_server/scihub/scilog/scilog.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_bec_server_utils/test_main.py
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_bec_server_utils/test_service_handler.py
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_bec_server_utils/test_tmux_launch.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_data_processing/conftest.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_data_processing/test_dap_cli_launch.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_data_processing/test_dap_server.py
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_data_processing/test_dap_service_manager.py
+-rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_data_processing/test_lmfit1d_service.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_device_server/conftest.py
+-rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_device_server/test_config_handler.py
+-rw-r--r--   0        0        0     6020 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_device_server/test_device_manager_ds.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_device_server/test_device_serializer.py
+-rw-r--r--   0        0        0    28297 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_device_server/test_device_server.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_device_server/test_device_server_cli_launch.py
+-rw-r--r--   0        0        0     9555 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_device_server/test_rpc_mixin.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_file_writer/conftest.py
+-rw-r--r--   0        0        0     6829 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_file_writer/test_file_writer.py
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_file_writer/test_file_writer_cli_launch.py
+-rw-r--r--   0        0        0    11233 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_file_writer/test_file_writer_manager.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_scan_bundler/conftest.py
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_scan_bundler/test_bec_emitter.py
+-rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_scan_bundler/test_bluesky_emitter.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_scan_bundler/test_emitter.py
+-rw-r--r--   0        0        0    25541 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_scan_bundler/test_scan_bundler.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_scan_bundler/test_scan_bundler_cli_launch.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_scan_server/conftest.py
+-rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_scan_server/test_path_optimization.py
+-rw-r--r--   0        0        0    11602 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_scan_server/test_scan_guard.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_scan_server/test_scan_server_cli_launch.py
+-rw-r--r--   0        0        0    26404 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_scan_server/test_scan_server_queue.py
+-rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_scan_server/test_scan_stubs.py
+-rw-r--r--   0        0        0    54003 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_scan_server/test_scan_worker.py
+-rw-r--r--   0        0        0    87804 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_scan_server/test_scans.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_scihub/conftest.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_scihub/test_repeated_timer.py
+-rw-r--r--   0        0        0    16951 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_scihub/test_scibec_config_handler.py
+-rw-r--r--   0        0        0     5641 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_scihub/test_scibec_connector.py
+-rw-r--r--   0        0        0     8663 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_scihub/test_scibec_metadata_handler.py
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_scihub/test_scihub_cli_launch.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 bec_server-2.7.2/tests/tests_scihub/test_scilog_connector.py
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 bec_server-2.7.2/.gitignore
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 bec_server-2.7.2/pyproject.toml
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 bec_server-2.7.2/PKG-INFO
```

### Comparing `bec_server-2.7.1/bec_server/bec_server_utils/launch.py` & `bec_server-2.7.2/bec_server/bec_server_utils/launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/bec_server_utils/service_handler.py` & `bec_server-2.7.2/bec_server/bec_server_utils/service_handler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/bec_server_utils/subprocess_launch.py` & `bec_server-2.7.2/bec_server/bec_server_utils/subprocess_launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/bec_server_utils/tmux_launch.py` & `bec_server-2.7.2/bec_server/bec_server_utils/tmux_launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/data_processing/dap_server.py` & `bec_server-2.7.2/bec_server/data_processing/dap_server.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/data_processing/dap_service.py` & `bec_server-2.7.2/bec_server/data_processing/dap_service.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/data_processing/dap_service_manager.py` & `bec_server-2.7.2/bec_server/data_processing/dap_service_manager.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/data_processing/lmfit1d_service.py` & `bec_server-2.7.2/bec_server/data_processing/lmfit1d_service.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/data_processing/cli/launch.py` & `bec_server-2.7.2/bec_server/data_processing/cli/launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/device_server/device_server.py` & `bec_server-2.7.2/bec_server/device_server/device_server.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/device_server/rpc_mixin.py` & `bec_server-2.7.2/bec_server/device_server/rpc_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/device_server/cli/launch.py` & `bec_server-2.7.2/bec_server/device_server/cli/launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/device_server/devices/config_update_handler.py` & `bec_server-2.7.2/bec_server/device_server/devices/config_update_handler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/device_server/devices/device_serializer.py` & `bec_server-2.7.2/bec_server/device_server/devices/device_serializer.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/device_server/devices/devicemanager.py` & `bec_server-2.7.2/bec_server/device_server/devices/devicemanager.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/device_server/tests/utils.py` & `bec_server-2.7.2/bec_server/device_server/tests/utils.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/file_writer/default_writer.py` & `bec_server-2.7.2/bec_server/file_writer/default_writer.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/file_writer/file_writer.py` & `bec_server-2.7.2/bec_server/file_writer/file_writer.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/file_writer/file_writer_manager.py` & `bec_server-2.7.2/bec_server/file_writer/file_writer_manager.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/file_writer/merged_dicts.py` & `bec_server-2.7.2/bec_server/file_writer/merged_dicts.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/file_writer/cli/launch.py` & `bec_server-2.7.2/bec_server/file_writer/cli/launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/file_writer_plugins/cSAXS.py` & `bec_server-2.7.2/bec_server/file_writer_plugins/cSAXS.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/scan_bundler/bec_emitter.py` & `bec_server-2.7.2/bec_server/scan_bundler/bec_emitter.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/scan_bundler/bluesky_emitter.py` & `bec_server-2.7.2/bec_server/scan_bundler/bluesky_emitter.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/scan_bundler/emitter.py` & `bec_server-2.7.2/bec_server/scan_bundler/emitter.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/scan_bundler/scan_bundler.py` & `bec_server-2.7.2/bec_server/scan_bundler/scan_bundler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/scan_bundler/cli/launch.py` & `bec_server-2.7.2/bec_server/scan_bundler/cli/launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/scan_server/device_validation.py` & `bec_server-2.7.2/bec_server/scan_server/device_validation.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/scan_server/path_optimization.py` & `bec_server-2.7.2/bec_server/scan_server/path_optimization.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/scan_server/scan_assembler.py` & `bec_server-2.7.2/bec_server/scan_server/scan_assembler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/scan_server/scan_guard.py` & `bec_server-2.7.2/bec_server/scan_server/scan_guard.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/scan_server/scan_manager.py` & `bec_server-2.7.2/bec_server/scan_server/scan_manager.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/scan_server/scan_queue.py` & `bec_server-2.7.2/bec_server/scan_server/scan_queue.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/scan_server/scan_server.py` & `bec_server-2.7.2/bec_server/scan_server/scan_server.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/scan_server/scan_stubs.py` & `bec_server-2.7.2/bec_server/scan_server/scan_stubs.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/scan_server/scan_worker.py` & `bec_server-2.7.2/bec_server/scan_server/scan_worker.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/scan_server/scans.py` & `bec_server-2.7.2/bec_server/scan_server/scans.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/scan_server/cli/launch.py` & `bec_server-2.7.2/bec_server/scan_server/cli/launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/scan_server/scan_plugins/otf_scan.py` & `bec_server-2.7.2/bec_server/scan_server/scan_plugins/otf_scan.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/scan_server/tests/utils.py` & `bec_server-2.7.2/bec_server/scan_server/tests/utils.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/scihub/repeated_timer.py` & `bec_server-2.7.2/bec_server/scihub/repeated_timer.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/scihub/scihub.py` & `bec_server-2.7.2/bec_server/scihub/scihub.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/scihub/cli/launch.py` & `bec_server-2.7.2/bec_server/scihub/cli/launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/scihub/scibec/config_handler.py` & `bec_server-2.7.2/bec_server/scihub/scibec/config_handler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/scihub/scibec/scibec_connector.py` & `bec_server-2.7.2/bec_server/scihub/scibec/scibec_connector.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/scihub/scibec/scibec_metadata_handler.py` & `bec_server-2.7.2/bec_server/scihub/scibec/scibec_metadata_handler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/bec_server/scihub/scilog/scilog.py` & `bec_server-2.7.2/bec_server/scihub/scilog/scilog.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/tests/tests_bec_server_utils/test_main.py` & `bec_server-2.7.2/tests/tests_bec_server_utils/test_main.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/tests/tests_bec_server_utils/test_service_handler.py` & `bec_server-2.7.2/tests/tests_bec_server_utils/test_service_handler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/tests/tests_bec_server_utils/test_tmux_launch.py` & `bec_server-2.7.2/tests/tests_bec_server_utils/test_tmux_launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/tests/tests_data_processing/test_dap_cli_launch.py` & `bec_server-2.7.2/tests/tests_data_processing/test_dap_cli_launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/tests/tests_data_processing/test_dap_service_manager.py` & `bec_server-2.7.2/tests/tests_data_processing/test_dap_service_manager.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/tests/tests_data_processing/test_lmfit1d_service.py` & `bec_server-2.7.2/tests/tests_data_processing/test_lmfit1d_service.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/tests/tests_device_server/conftest.py` & `bec_server-2.7.2/tests/tests_device_server/conftest.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/tests/tests_device_server/test_config_handler.py` & `bec_server-2.7.2/tests/tests_device_server/test_config_handler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/tests/tests_device_server/test_device_manager_ds.py` & `bec_server-2.7.2/tests/tests_device_server/test_device_manager_ds.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/tests/tests_device_server/test_device_serializer.py` & `bec_server-2.7.2/tests/tests_device_server/test_device_serializer.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/tests/tests_device_server/test_device_server.py` & `bec_server-2.7.2/tests/tests_device_server/test_device_server.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/tests/tests_device_server/test_device_server_cli_launch.py` & `bec_server-2.7.2/tests/tests_device_server/test_device_server_cli_launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/tests/tests_device_server/test_rpc_mixin.py` & `bec_server-2.7.2/tests/tests_device_server/test_rpc_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/tests/tests_file_writer/test_file_writer.py` & `bec_server-2.7.2/tests/tests_file_writer/test_file_writer.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/tests/tests_file_writer/test_file_writer_cli_launch.py` & `bec_server-2.7.2/tests/tests_file_writer/test_file_writer_cli_launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/tests/tests_file_writer/test_file_writer_manager.py` & `bec_server-2.7.2/tests/tests_file_writer/test_file_writer_manager.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/tests/tests_scan_bundler/conftest.py` & `bec_server-2.7.2/tests/tests_scan_bundler/conftest.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/tests/tests_scan_bundler/test_bec_emitter.py` & `bec_server-2.7.2/tests/tests_scan_bundler/test_bec_emitter.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/tests/tests_scan_bundler/test_bluesky_emitter.py` & `bec_server-2.7.2/tests/tests_scan_bundler/test_bluesky_emitter.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/tests/tests_scan_bundler/test_emitter.py` & `bec_server-2.7.2/tests/tests_scan_bundler/test_emitter.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/tests/tests_scan_bundler/test_scan_bundler.py` & `bec_server-2.7.2/tests/tests_scan_bundler/test_scan_bundler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/tests/tests_scan_bundler/test_scan_bundler_cli_launch.py` & `bec_server-2.7.2/tests/tests_scan_bundler/test_scan_bundler_cli_launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/tests/tests_scan_server/test_path_optimization.py` & `bec_server-2.7.2/tests/tests_scan_server/test_path_optimization.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/tests/tests_scan_server/test_scan_guard.py` & `bec_server-2.7.2/tests/tests_scan_server/test_scan_guard.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/tests/tests_scan_server/test_scan_server_cli_launch.py` & `bec_server-2.7.2/tests/tests_scan_server/test_scan_server_cli_launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/tests/tests_scan_server/test_scan_server_queue.py` & `bec_server-2.7.2/tests/tests_scan_server/test_scan_server_queue.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/tests/tests_scan_server/test_scan_stubs.py` & `bec_server-2.7.2/tests/tests_scan_server/test_scan_stubs.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/tests/tests_scan_server/test_scan_worker.py` & `bec_server-2.7.2/tests/tests_scan_server/test_scan_worker.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/tests/tests_scan_server/test_scans.py` & `bec_server-2.7.2/tests/tests_scan_server/test_scans.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/tests/tests_scihub/test_repeated_timer.py` & `bec_server-2.7.2/tests/tests_scihub/test_repeated_timer.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/tests/tests_scihub/test_scibec_config_handler.py` & `bec_server-2.7.2/tests/tests_scihub/test_scibec_config_handler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/tests/tests_scihub/test_scibec_connector.py` & `bec_server-2.7.2/tests/tests_scihub/test_scibec_connector.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/tests/tests_scihub/test_scibec_metadata_handler.py` & `bec_server-2.7.2/tests/tests_scihub/test_scibec_metadata_handler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/tests/tests_scihub/test_scihub_cli_launch.py` & `bec_server-2.7.2/tests/tests_scihub/test_scihub_cli_launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/tests/tests_scihub/test_scilog_connector.py` & `bec_server-2.7.2/tests/tests_scihub/test_scilog_connector.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/.gitignore` & `bec_server-2.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `bec_server-2.7.1/pyproject.toml` & `bec_server-2.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bec-server"
-version = "2.7.1"
+version = "2.7.2"
 description = "BEC server"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering",
 ]
```

### Comparing `bec_server-2.7.1/PKG-INFO` & `bec_server-2.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bec-server
-Version: 2.7.1
+Version: 2.7.2
 Summary: BEC server
 Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/bec/issues
 Project-URL: Homepage, https://gitlab.psi.ch/bec/bec
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.10
```

