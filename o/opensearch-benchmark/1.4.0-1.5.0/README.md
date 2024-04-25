# Comparing `tmp/opensearch-benchmark-1.4.0.tar.gz` & `tmp/opensearch_benchmark-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensearch-benchmark-1.4.0.tar", last modified: Thu Mar 28 17:40:52 2024, max compression
+gzip compressed data, was "opensearch_benchmark-1.5.0.tar", last modified: Thu Apr 25 17:39:17 2024, max compression
```

## Comparing `opensearch-benchmark-1.4.0.tar` & `opensearch_benchmark-1.5.0.tar`

### file list

```diff
@@ -1,318 +1,318 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.199572 opensearch-benchmark-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     7922 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-03-28 17:40:52.199572 opensearch-benchmark-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.155572 opensearch-benchmark-1.4.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.155572 opensearch-benchmark-1.4.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/docs/api/client-options.md
--rw-r--r--   0 runner    (1001) docker     (127)     8586 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/docs/api/execute-test.md
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/docs/api/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/docs/api/kill-running-process.md
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/docs/api/pipeline.md
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/docs/api/target-hosts.md
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/docs/api/test-mode.md
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/docs/api/workload.md
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/docs/get-started.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.155572 opensearch-benchmark-1.4.0/docs/user-guides/
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/docs/user-guides/create-pipeline.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/docs/user-guides/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.195572 opensearch-benchmark-1.4.0/opensearch_benchmark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-03-28 17:40:52.000000 opensearch-benchmark-1.4.0/opensearch_benchmark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12861 2024-03-28 17:40:52.000000 opensearch-benchmark-1.4.0/opensearch_benchmark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 17:40:52.000000 opensearch-benchmark-1.4.0/opensearch_benchmark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-28 17:40:52.000000 opensearch-benchmark-1.4.0/opensearch_benchmark.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 17:40:51.000000 opensearch-benchmark-1.4.0/opensearch_benchmark.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-03-28 17:40:52.000000 opensearch-benchmark-1.4.0/opensearch_benchmark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-28 17:40:52.000000 opensearch-benchmark-1.4.0/opensearch_benchmark.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.159572 opensearch-benchmark-1.4.0/osbenchmark/
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11675 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/actor.py
--rw-r--r--   0 runner    (1001) docker     (127)    11039 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/async_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    51164 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/benchmarkd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.163572 opensearch-benchmark-1.4.0/osbenchmark/builder/
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31535 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/cluster_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.163572 opensearch-benchmark-1.4.0/osbenchmark/builder/configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.163572 opensearch-benchmark-1.4.0/osbenchmark/builder/configs/listers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/configs/listers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/configs/listers/plugin_config_instance_lister.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.163572 opensearch-benchmark-1.4.0/osbenchmark/builder/configs/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/configs/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/configs/utils/config_path_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.167572 opensearch-benchmark-1.4.0/osbenchmark/builder/downloaders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/downloaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.167572 opensearch-benchmark-1.4.0/osbenchmark/builder/downloaders/builders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/downloaders/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/downloaders/builders/binary_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/downloaders/builders/source_binary_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/downloaders/core_plugin_source_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/downloaders/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/downloaders/external_plugin_source_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/downloaders/opensearch_distribution_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/downloaders/opensearch_source_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/downloaders/plugin_distribution_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.167572 opensearch-benchmark-1.4.0/osbenchmark/builder/downloaders/repositories/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/downloaders/repositories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/downloaders/repositories/opensearch_distribution_repository_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/downloaders/repositories/plugin_distribution_repository_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/downloaders/repositories/repository_url_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/downloaders/repositories/source_repository_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.167572 opensearch-benchmark-1.4.0/osbenchmark/builder/executors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/executors/exception_handling_shell_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/executors/local_shell_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/executors/shell_executor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.167572 opensearch-benchmark-1.4.0/osbenchmark/builder/installers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/installers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/installers/bare_installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/installers/docker_installer.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/installers/exception_handling_installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/installers/installer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.171572 opensearch-benchmark-1.4.0/osbenchmark/builder/installers/preparers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/installers/preparers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/installers/preparers/opensearch_preparer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/installers/preparers/plugin_preparer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/installers/preparers/preparer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/java_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    12170 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.171572 opensearch-benchmark-1.4.0/osbenchmark/builder/launchers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/launchers/docker_launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/launchers/exception_handling_launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/launchers/launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     8421 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/launchers/local_process_launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/launchers/no_op_launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.171572 opensearch-benchmark-1.4.0/osbenchmark/builder/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/models/architecture_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/models/bootstrap_phase.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/models/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/models/cluster_flavors.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/models/cluster_infra_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/models/config_instance_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/models/host.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/models/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/models/plugin_config_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/models/provision_config_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/models/provision_config_instance_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/models/provision_config_instance_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    24300 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/provision_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    23247 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/provisioner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.171572 opensearch-benchmark-1.4.0/osbenchmark/builder/provisioners/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/provisioners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/provisioners/provisioner.py
--rw-r--r--   0 runner    (1001) docker     (127)    34133 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/supplier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.175572 opensearch-benchmark-1.4.0/osbenchmark/builder/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/utils/artifact_variables_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/utils/binary_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/utils/config_applier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/utils/git_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/utils/host_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/utils/java_home_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/utils/jdk_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/utils/path_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/builder/utils/template_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)    21056 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12970 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    99370 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/min-os-version.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.175572 opensearch-benchmark-1.4.0/osbenchmark/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/base-workload.json.j2
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/benchmark.ini
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/custom-operations.json.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/custom-test-procedures.json.j2
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/default-operations.json.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/default-test-procedures.json.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/docker-compose.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/logging.json
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/metrics-template.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.147571 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.147571 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.147571 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.179572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/core-plugins.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.179572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.179572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.179572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.179572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.147571 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/default/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.147571 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/default/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.179572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/default/templates/config/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/default/templates/config/opensearch.yml
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/http.ini
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/transport.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.147571 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.183572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/16gheap.ini
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/1gheap.ini
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/24gheap.ini
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/2gheap.ini
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/4gheap.ini
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/8gheap.ini
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/basic-license.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.147571 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/dbg_non_safepoints/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.147571 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/dbg_non_safepoints/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.183572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/dbg_non_safepoints/templates/config/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/dbg_non_safepoints/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/debug-non-safepoints.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.183572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/config.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.147571 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.183572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/templates/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/templates/config/opensearch.yml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/defaults.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.147571 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.147571 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.183572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea/templates/config/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.147571 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.147571 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.183572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp/templates/config/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp.ini
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/g1gc.ini
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/trial-license.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.147571 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.147571 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.183572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled/templates/config/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.183572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/config.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.147571 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.183572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (127)    11731 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/log4j2.properties
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/opensearch.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.151572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.147571 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.183572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/plugins/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/plugins/v1/core-plugins.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.183572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.183572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.183572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.183572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.151572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/default/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.151572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/default/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.187572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/default/templates/config/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/default/templates/config/opensearch.yml
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/http.ini
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/transport.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.151572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.187572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/16gheap.ini
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/1gheap.ini
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/24gheap.ini
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/2gheap.ini
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/4gheap.ini
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/8gheap.ini
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/basic-license.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.151572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/dbg_non_safepoints/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.151572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/dbg_non_safepoints/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.187572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/dbg_non_safepoints/templates/config/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/dbg_non_safepoints/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/debug-non-safepoints.ini
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/defaults.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.151572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.151572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.187572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea/templates/config/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.151572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.151572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.187572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp/templates/config/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp.ini
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/g1gc.ini
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/parallelgc.ini
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/trial-license.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.151572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.151572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.187572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled/templates/config/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.191572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/config.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.151572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.191572 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/log4j2.properties
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/opensearch.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/results-template.json
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/test-executions-template.json
--rw-r--r--   0 runner    (1001) docker     (127)    23167 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/resources/workload-schema.json
--rw-r--r--   0 runner    (1001) docker     (127)    36056 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/results_publisher.py
--rw-r--r--   0 runner    (1001) docker     (127)    83463 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)    18831 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/test_execution_orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/time.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.191572 opensearch-benchmark-1.4.0/osbenchmark/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/utils/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/utils/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/utils/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     8354 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/utils/git.py
--rw-r--r--   0 runner    (1001) docker     (127)    21980 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     7537 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/utils/jvm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/utils/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    12386 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/utils/net.py
--rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/utils/opts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/utils/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/utils/periodic_waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6901 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/utils/process.py
--rw-r--r--   0 runner    (1001) docker     (127)     8279 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/utils/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/utils/sysstats.py
--rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/utils/versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.195572 opensearch-benchmark-1.4.0/osbenchmark/worker_coordinator/
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/worker_coordinator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/worker_coordinator/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)   100853 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/worker_coordinator/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    12317 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/worker_coordinator/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    99934 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/worker_coordinator/worker_coordinator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.195572 opensearch-benchmark-1.4.0/osbenchmark/workload/
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/workload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    92616 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/workload/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    76510 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/workload/params.py
--rw-r--r--   0 runner    (1001) docker     (127)    38583 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/workload/workload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.195572 opensearch-benchmark-1.4.0/osbenchmark/workload_generator/
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/workload_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/workload_generator/corpus.py
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/workload_generator/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     8569 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/osbenchmark/workload_generator/workload_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.195572 opensearch-benchmark-1.4.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)    10512 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/scripts/expand-data-corpus.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-28 17:40:52.199572 opensearch-benchmark-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6730 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:40:52.195572 opensearch-benchmark-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/tests/test_async_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/tests/test_execution_orchestrator_test.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-28 17:39:00.000000 opensearch-benchmark-1.4.0/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.392388 opensearch_benchmark-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     8852 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-25 17:39:17.392388 opensearch_benchmark-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.348387 opensearch_benchmark-1.5.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.348387 opensearch_benchmark-1.5.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/docs/api/client-options.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8586 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/docs/api/execute-test.md
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/docs/api/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/docs/api/kill-running-process.md
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/docs/api/pipeline.md
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/docs/api/target-hosts.md
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/docs/api/test-mode.md
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/docs/api/workload.md
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/docs/get-started.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.348387 opensearch_benchmark-1.5.0/docs/user-guides/
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/docs/user-guides/create-pipeline.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/docs/user-guides/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.388388 opensearch_benchmark-1.5.0/opensearch_benchmark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-25 17:39:17.000000 opensearch_benchmark-1.5.0/opensearch_benchmark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12861 2024-04-25 17:39:17.000000 opensearch_benchmark-1.5.0/opensearch_benchmark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 17:39:17.000000 opensearch_benchmark-1.5.0/opensearch_benchmark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-25 17:39:17.000000 opensearch_benchmark-1.5.0/opensearch_benchmark.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 17:39:17.000000 opensearch_benchmark-1.5.0/opensearch_benchmark.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-25 17:39:17.000000 opensearch_benchmark-1.5.0/opensearch_benchmark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 17:39:17.000000 opensearch_benchmark-1.5.0/opensearch_benchmark.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.356387 opensearch_benchmark-1.5.0/osbenchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11675 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11039 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/async_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51772 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/benchmarkd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.356387 opensearch_benchmark-1.5.0/osbenchmark/builder/
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31535 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/cluster_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.356387 opensearch_benchmark-1.5.0/osbenchmark/builder/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.356387 opensearch_benchmark-1.5.0/osbenchmark/builder/configs/listers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/configs/listers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/configs/listers/plugin_config_instance_lister.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.356387 opensearch_benchmark-1.5.0/osbenchmark/builder/configs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/configs/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/configs/utils/config_path_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.360387 opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.360387 opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/builders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/builders/binary_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/builders/source_binary_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/core_plugin_source_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/external_plugin_source_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/opensearch_distribution_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/opensearch_source_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/plugin_distribution_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.360387 opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/repositories/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/repositories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/repositories/opensearch_distribution_repository_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/repositories/plugin_distribution_repository_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/repositories/repository_url_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/repositories/source_repository_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.360387 opensearch_benchmark-1.5.0/osbenchmark/builder/executors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/executors/exception_handling_shell_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/executors/local_shell_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/executors/shell_executor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.360387 opensearch_benchmark-1.5.0/osbenchmark/builder/installers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/installers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/installers/bare_installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/installers/docker_installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/installers/exception_handling_installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/installers/installer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.364387 opensearch_benchmark-1.5.0/osbenchmark/builder/installers/preparers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/installers/preparers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/installers/preparers/opensearch_preparer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/installers/preparers/plugin_preparer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/installers/preparers/preparer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/java_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12170 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.364387 opensearch_benchmark-1.5.0/osbenchmark/builder/launchers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/launchers/docker_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/launchers/exception_handling_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/launchers/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8421 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/launchers/local_process_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/launchers/no_op_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.364387 opensearch_benchmark-1.5.0/osbenchmark/builder/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/models/architecture_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/models/bootstrap_phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/models/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/models/cluster_flavors.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/models/cluster_infra_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/models/config_instance_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/models/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/models/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/models/plugin_config_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/models/provision_config_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/models/provision_config_instance_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/models/provision_config_instance_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24300 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/provision_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23247 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/provisioner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.364387 opensearch_benchmark-1.5.0/osbenchmark/builder/provisioners/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/provisioners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/provisioners/provisioner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34133 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/supplier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.368388 opensearch_benchmark-1.5.0/osbenchmark/builder/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/utils/artifact_variables_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/utils/binary_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/utils/config_applier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/utils/git_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/utils/host_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/utils/java_home_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/utils/jdk_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/utils/path_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/utils/template_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21056 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12970 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    99370 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/min-os-version.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.368388 opensearch_benchmark-1.5.0/osbenchmark/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/base-workload.json.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/benchmark.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/custom-operations.json.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/custom-test-procedures.json.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/default-operations.json.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/default-test-procedures.json.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/docker-compose.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/logging.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/metrics-template.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.344387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.340387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.340387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.368388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/core-plugins.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.372388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.372388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.372388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.372388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.340387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/default/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.340387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/default/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.372388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/default/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/default/templates/config/opensearch.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/http.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/transport.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.340387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.372388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/16gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/1gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/24gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/2gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/4gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/8gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/basic-license.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.340387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/dbg_non_safepoints/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.340387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/dbg_non_safepoints/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.376388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/dbg_non_safepoints/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/dbg_non_safepoints/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/debug-non-safepoints.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.376388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/config.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.340387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.376388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/templates/config/opensearch.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/defaults.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.340387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.340387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.376388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.340387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.340387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.376388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/g1gc.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/trial-license.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.340387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.340387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.376388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.376388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/config.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.344387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.376388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (127)    11731 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/log4j2.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/opensearch.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.344387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.344387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.376388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/core-plugins.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.376388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.376388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.376388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.376388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.344387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/default/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.344387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/default/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.376388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/default/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/default/templates/config/opensearch.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/http.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/transport.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.344387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.380388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/16gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/1gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/24gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/2gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/4gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/8gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/basic-license.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.344387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/dbg_non_safepoints/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.344387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/dbg_non_safepoints/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.380388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/dbg_non_safepoints/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/dbg_non_safepoints/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/debug-non-safepoints.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/defaults.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.344387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.344387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.380388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.344387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.344387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.380388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/g1gc.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/parallelgc.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/trial-license.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.344387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.344387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.380388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.380388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/config.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.344387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.384388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/log4j2.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/opensearch.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/results-template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/test-executions-template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23167 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/workload-schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)    36092 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/results_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83463 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18831 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/test_execution_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.384388 opensearch_benchmark-1.5.0/osbenchmark/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/utils/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/utils/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/utils/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8354 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21980 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7537 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/utils/jvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/utils/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12386 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/utils/net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/utils/opts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/utils/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/utils/periodic_waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6901 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/utils/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8279 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/utils/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/utils/sysstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/utils/versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.388388 opensearch_benchmark-1.5.0/osbenchmark/worker_coordinator/
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/worker_coordinator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/worker_coordinator/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)   107234 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/worker_coordinator/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12317 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/worker_coordinator/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    99934 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/worker_coordinator/worker_coordinator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.388388 opensearch_benchmark-1.5.0/osbenchmark/workload/
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/workload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92616 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/workload/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76510 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/workload/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39027 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/workload/workload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.388388 opensearch_benchmark-1.5.0/osbenchmark/workload_generator/
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/workload_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/workload_generator/corpus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/workload_generator/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8569 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/workload_generator/workload_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.388388 opensearch_benchmark-1.5.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10512 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/scripts/expand-data-corpus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-25 17:39:17.392388 opensearch_benchmark-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6817 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.388388 opensearch_benchmark-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/tests/test_async_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/tests/test_execution_orchestrator_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/version.txt
```

### Comparing `opensearch-benchmark-1.4.0/AUTHORS` & `opensearch_benchmark-1.5.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/CONTRIBUTING.md` & `opensearch_benchmark-1.5.0/CONTRIBUTING.md`

 * *Files 8% similar despite different names*

```diff
@@ -86,14 +86,18 @@
 ```
 Signed-off-by: Jane Smith <jane.smith@email.com>
 ```
 You may type this line on your own when writing your commit messages. However, if your user.name and user.email are set in your git configs, you can use `-s` or `--signoff` to add the `Signed-off-by` line to the end of the commit message.
 
 ## Review Process
 
-We deeply appreciate everyone who takes the time to make a contribution. We will review all contributions as quickly as possible. As a reminder, [opening an issue](https://github.com/opensearch-project/OpenSearch-Benchmark/issues/new/choose) discussing your change before you make it is the best way to smooth the PR process. This will prevent a rejection because someone else is already working on the problem, or because the solution is incompatible with the architectural direction.
+We deeply appreciate everyone who takes the time to make a contribution. We aim to review all contributions promptly but cannot guarantee quick turnaround times. It can take time for appropriate analysis, verification and testing, to understand the implications and ramifications of the proposed change, and for discussion with other maintainers and developers. Furthermore, it is essential that contributions remain accessible for an adequate duration to allow healthy engagement by community members, other than maintainers.
+
+Please note that there is a code freeze imposed starting a week before every release to ensure stability of the codebase and a smooth release process. If you are interested in getting a change into the next release, please submit your change well in advance, so that it is approved and merged in prior to the deadline for the freeze. We are in the process of implementing snapshot releases, so if your change does not make a particular release, the appropriate snapshot release can be used until the next official release is cut.
+
+As a reminder, [opening an issue](https://github.com/opensearch-project/OpenSearch-Benchmark/issues/new/choose) discussing your change before you make it is the best way to smooth the PR process. This will prevent a rejection because someone else is already working on the problem, or because the solution is incompatible with the architectural direction.
 
 During the PR process, expect that there will be some back-and-forth. Please try to respond to comments in a timely fashion, and if you don't wish to continue with the PR, let us know. If a PR takes too many iterations for its complexity or size, we may reject it. Additionally, if you stop responding we may close the PR as abandoned. In either case, if you feel this was done in error, please add a comment on the PR.
 
 If we accept the PR, a [maintainer](MAINTAINERS.md) will merge your change and usually take care of backporting it to appropriate branches ourselves.
 
-If we reject the PR, we will close the pull request with a comment explaining why. This decision isn't always final: if you feel we have misunderstood your intended change or otherwise think that we should reconsider then please continue the conversation with a comment on the PR and we'll do our best to address any further points you raise.
+If we reject the PR, we will close the pull request with a comment explaining why. This decision isn't always final: if you feel we have misunderstood your intended change or otherwise think that we should reconsider then please continue the conversation with a comment on the PR and we'll do our best to address any further points you raise.
```

### Comparing `opensearch-benchmark-1.4.0/LICENSE` & `opensearch_benchmark-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/PKG-INFO` & `opensearch_benchmark-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensearch-benchmark
-Version: 1.4.0
+Version: 1.5.0
 Summary: Macrobenchmarking framework for OpenSearch
 Home-page: https://github.com/opensearch-project/OpenSearch-Benchmark
 Maintainer: Ian Hoang, Govind Kamat
 Maintainer-email: hoangia@amazon.com, govkamat@amazon.com
 License: Apache License, Version 2.0
 Classifier: Topic :: System :: Benchmark
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,32 +19,32 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8,<3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 License-File: AUTHORS
-Requires-Dist: opensearch-py[async]==2.5.0
-Requires-Dist: psutil==5.8.0
-Requires-Dist: py-cpuinfo==7.0.0
-Requires-Dist: tabulate==0.9.0
-Requires-Dist: jsonschema==3.1.1
-Requires-Dist: Jinja2==3.1.3
-Requires-Dist: markupsafe==2.0.1
-Requires-Dist: thespian==3.10.1
+Requires-Dist: opensearch-py[async]>=2.5.0
+Requires-Dist: psutil>=5.8.0
+Requires-Dist: py-cpuinfo>=7.0.0
+Requires-Dist: tabulate>=0.9.0
+Requires-Dist: jsonschema>=3.1.1
+Requires-Dist: Jinja2>=3.1.3
+Requires-Dist: markupsafe>=2.0.1
+Requires-Dist: thespian<3.10.7,>=3.10.1
 Requires-Dist: certifi
-Requires-Dist: yappi==1.4.0
-Requires-Dist: ijson==2.6.1
-Requires-Dist: google-resumable-media==1.1.0
-Requires-Dist: google-auth==1.22.1
-Requires-Dist: wheel==0.38.4
-Requires-Dist: boto3==1.28.62
-Requires-Dist: zstandard==0.22.0
-Requires-Dist: h5py==3.10.0
-Requires-Dist: numpy==1.24.2
+Requires-Dist: yappi>=1.4.0
+Requires-Dist: ijson>=2.6.1
+Requires-Dist: google-resumable-media>=1.1.0
+Requires-Dist: google-auth>=1.22.1
+Requires-Dist: wheel>=0.38.4
+Requires-Dist: boto3>=1.28.62
+Requires-Dist: zstandard>=0.22.0
+Requires-Dist: h5py>=3.10.0
+Requires-Dist: numpy>=1.24.2
 Provides-Extra: develop
 Requires-Dist: ujson; extra == "develop"
 Requires-Dist: pytest==7.2.2; extra == "develop"
 Requires-Dist: pytest-benchmark==3.2.2; extra == "develop"
 Requires-Dist: pytest-asyncio==0.14.0; extra == "develop"
 Requires-Dist: tox==3.14.0; extra == "develop"
 Requires-Dist: coverage==5.5; extra == "develop"
```

### Comparing `opensearch-benchmark-1.4.0/README.md` & `opensearch_benchmark-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/docs/api/execute-test.md` & `opensearch_benchmark-1.5.0/docs/api/execute-test.md`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/docs/user-guides/create-pipeline.md` & `opensearch_benchmark-1.5.0/docs/user-guides/create-pipeline.md`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/opensearch_benchmark.egg-info/PKG-INFO` & `opensearch_benchmark-1.5.0/opensearch_benchmark.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensearch-benchmark
-Version: 1.4.0
+Version: 1.5.0
 Summary: Macrobenchmarking framework for OpenSearch
 Home-page: https://github.com/opensearch-project/OpenSearch-Benchmark
 Maintainer: Ian Hoang, Govind Kamat
 Maintainer-email: hoangia@amazon.com, govkamat@amazon.com
 License: Apache License, Version 2.0
 Classifier: Topic :: System :: Benchmark
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,32 +19,32 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8,<3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 License-File: AUTHORS
-Requires-Dist: opensearch-py[async]==2.5.0
-Requires-Dist: psutil==5.8.0
-Requires-Dist: py-cpuinfo==7.0.0
-Requires-Dist: tabulate==0.9.0
-Requires-Dist: jsonschema==3.1.1
-Requires-Dist: Jinja2==3.1.3
-Requires-Dist: markupsafe==2.0.1
-Requires-Dist: thespian==3.10.1
+Requires-Dist: opensearch-py[async]>=2.5.0
+Requires-Dist: psutil>=5.8.0
+Requires-Dist: py-cpuinfo>=7.0.0
+Requires-Dist: tabulate>=0.9.0
+Requires-Dist: jsonschema>=3.1.1
+Requires-Dist: Jinja2>=3.1.3
+Requires-Dist: markupsafe>=2.0.1
+Requires-Dist: thespian<3.10.7,>=3.10.1
 Requires-Dist: certifi
-Requires-Dist: yappi==1.4.0
-Requires-Dist: ijson==2.6.1
-Requires-Dist: google-resumable-media==1.1.0
-Requires-Dist: google-auth==1.22.1
-Requires-Dist: wheel==0.38.4
-Requires-Dist: boto3==1.28.62
-Requires-Dist: zstandard==0.22.0
-Requires-Dist: h5py==3.10.0
-Requires-Dist: numpy==1.24.2
+Requires-Dist: yappi>=1.4.0
+Requires-Dist: ijson>=2.6.1
+Requires-Dist: google-resumable-media>=1.1.0
+Requires-Dist: google-auth>=1.22.1
+Requires-Dist: wheel>=0.38.4
+Requires-Dist: boto3>=1.28.62
+Requires-Dist: zstandard>=0.22.0
+Requires-Dist: h5py>=3.10.0
+Requires-Dist: numpy>=1.24.2
 Provides-Extra: develop
 Requires-Dist: ujson; extra == "develop"
 Requires-Dist: pytest==7.2.2; extra == "develop"
 Requires-Dist: pytest-benchmark==3.2.2; extra == "develop"
 Requires-Dist: pytest-asyncio==0.14.0; extra == "develop"
 Requires-Dist: tox==3.14.0; extra == "develop"
 Requires-Dist: coverage==5.5; extra == "develop"
```

### Comparing `opensearch-benchmark-1.4.0/opensearch_benchmark.egg-info/SOURCES.txt` & `opensearch_benchmark-1.5.0/opensearch_benchmark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/__init__.py` & `opensearch_benchmark-1.5.0/osbenchmark/__init__.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/actor.py` & `opensearch_benchmark-1.5.0/osbenchmark/actor.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/async_connection.py` & `opensearch_benchmark-1.5.0/osbenchmark/async_connection.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/benchmark.py` & `opensearch_benchmark-1.5.0/osbenchmark/benchmark.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,14 +194,19 @@
         required=True,
         help=f"TestExecution ID of the baseline (see {PROGRAM_NAME} list test_executions).")
     compare_parser.add_argument(
         "--contender",
         required=True,
         help=f"TestExecution ID of the contender (see {PROGRAM_NAME} list test_executions).")
     compare_parser.add_argument(
+        "--percentiles",
+        help=f"A comma-separated list of percentiles to report latency and service time."
+             f"(default: {metrics.GlobalStatsCalculator.DEFAULT_LATENCY_PERCENTILES}).",
+        default=metrics.GlobalStatsCalculator.DEFAULT_LATENCY_PERCENTILES)
+    compare_parser.add_argument(
         "--results-format",
         help="Define the output format for the command line results (default: markdown).",
         choices=["markdown", "csv"],
         default="markdown")
     compare_parser.add_argument(
         "--results-numbers-align",
         help="Define the output column number alignment for the command line results (default: right).",
@@ -818,23 +823,27 @@
 def configure_results_publishing_params(args, cfg):
     cfg.add(config.Scope.applicationOverride, "results_publishing", "format", args.results_format)
     cfg.add(config.Scope.applicationOverride, "results_publishing", "values", args.show_in_results)
     cfg.add(config.Scope.applicationOverride, "results_publishing", "output.path", args.results_file)
     cfg.add(config.Scope.applicationOverride, "results_publishing", "numbers.align", args.results_numbers_align)
 
 
+def print_test_execution_id(args):
+    console.info(f"[Test Execution ID]: {args.test_execution_id}")
+
 def dispatch_sub_command(arg_parser, args, cfg):
     sub_command = args.subcommand
 
     cfg.add(config.Scope.application, "system", "quiet.mode", args.quiet)
     cfg.add(config.Scope.application, "system", "offline.mode", args.offline)
 
     try:
         if sub_command == "compare":
             configure_results_publishing_params(args, cfg)
+            cfg.add(config.Scope.applicationOverride, "results_publishing", "percentiles", args.percentiles)
             results_publisher.compare(cfg, args.baseline, args.contender)
         elif sub_command == "list":
             cfg.add(config.Scope.applicationOverride, "system", "list.config.option", args.configuration)
             cfg.add(config.Scope.applicationOverride, "system", "list.test_executions.max_results", args.limit)
             configure_builder_params(args, cfg, command_requires_provision_config_instance=False)
             configure_workload_params(arg_parser, args, cfg, command_requires_workload=False)
             dispatch_list(cfg)
@@ -856,28 +865,30 @@
             cfg.add(config.Scope.applicationOverride, "builder",
             "provision_config_instance.plugins", opts.csv_to_list(
                 args.opensearch_plugins))
             cfg.add(config.Scope.applicationOverride, "builder", "plugin.params", opts.to_dict(args.plugin_params))
             configure_builder_params(args, cfg)
             builder.install(cfg)
         elif sub_command == "start":
+            print_test_execution_id(args)
             cfg.add(config.Scope.applicationOverride, "system", "test_execution.id", args.test_execution_id)
             cfg.add(config.Scope.applicationOverride, "system", "install.id", args.installation_id)
             cfg.add(config.Scope.applicationOverride, "builder", "runtime.jdk", args.runtime_jdk)
             configure_telemetry_params(args, cfg)
             builder.start(cfg)
         elif sub_command == "stop":
             cfg.add(config.Scope.applicationOverride, "builder", "preserve.install", convert.to_bool(args.preserve_install))
             cfg.add(config.Scope.applicationOverride, "system", "install.id", args.installation_id)
             builder.stop(cfg)
         elif sub_command == "execute-test":
             # As the execute-test command is doing more work than necessary at the moment, we duplicate several parameters
             # in this section that actually belong to dedicated subcommands (like install, start or stop). Over time
             # these duplicated parameters will vanish as we move towards dedicated subcommands and use "execute-test" only
             # to run the actual benchmark (i.e. generating load).
+            print_test_execution_id(args)
             if args.effective_start_date:
                 cfg.add(config.Scope.applicationOverride, "system", "time.start", args.effective_start_date)
             cfg.add(config.Scope.applicationOverride, "system", "test_execution.id", args.test_execution_id)
             # use the test_execution id implicitly also as the install id.
             cfg.add(config.Scope.applicationOverride, "system", "install.id", args.test_execution_id)
             cfg.add(config.Scope.applicationOverride, "test_execution", "pipeline", args.pipeline)
             cfg.add(config.Scope.applicationOverride, "test_execution", "user.tag", args.user_tag)
```

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/benchmarkd.py` & `opensearch_benchmark-1.5.0/osbenchmark/benchmarkd.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/__init__.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/builder.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/builder.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/cluster.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/cluster.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/cluster_builder.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/cluster_builder.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/configs/listers/plugin_config_instance_lister.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/configs/listers/plugin_config_instance_lister.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/configs/utils/config_path_resolver.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/configs/utils/config_path_resolver.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/downloaders/builders/binary_builder.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/builders/binary_builder.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/downloaders/builders/source_binary_builder.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/builders/source_binary_builder.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/downloaders/core_plugin_source_downloader.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/core_plugin_source_downloader.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/downloaders/downloader.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/downloader.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/downloaders/external_plugin_source_downloader.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/external_plugin_source_downloader.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/downloaders/opensearch_distribution_downloader.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/opensearch_distribution_downloader.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/downloaders/opensearch_source_downloader.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/opensearch_source_downloader.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/downloaders/plugin_distribution_downloader.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/plugin_distribution_downloader.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/downloaders/repositories/opensearch_distribution_repository_provider.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/repositories/opensearch_distribution_repository_provider.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/downloaders/repositories/plugin_distribution_repository_provider.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/repositories/plugin_distribution_repository_provider.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/downloaders/repositories/repository_url_provider.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/repositories/repository_url_provider.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/downloaders/repositories/source_repository_provider.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/repositories/source_repository_provider.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/executors/local_shell_executor.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/executors/local_shell_executor.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/executors/shell_executor.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/executors/shell_executor.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/installers/bare_installer.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/installers/bare_installer.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/installers/docker_installer.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/installers/docker_installer.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/installers/exception_handling_installer.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/installers/exception_handling_installer.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/installers/installer.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/installers/installer.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/installers/preparers/opensearch_preparer.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/installers/preparers/opensearch_preparer.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/installers/preparers/plugin_preparer.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/installers/preparers/plugin_preparer.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/installers/preparers/preparer.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/installers/preparers/preparer.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/java_resolver.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/java_resolver.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/launcher.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/launcher.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/launchers/docker_launcher.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/launchers/docker_launcher.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/launchers/exception_handling_launcher.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/launchers/exception_handling_launcher.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/launchers/launcher.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/launchers/launcher.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/launchers/local_process_launcher.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/launchers/local_process_launcher.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/models/architecture_types.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/models/architecture_types.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/models/config_instance_types.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/models/config_instance_types.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/models/plugin_config_instance.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/models/plugin_config_instance.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/models/provision_config_instance.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/models/provision_config_instance.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/models/provision_config_instance_descriptor.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/models/provision_config_instance_descriptor.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/provision_config.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/provision_config.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/provisioner.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/provisioner.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/provisioners/provisioner.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/provisioners/provisioner.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/supplier.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/supplier.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/utils/artifact_variables_provider.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/utils/artifact_variables_provider.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/utils/config_applier.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/utils/config_applier.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/utils/git_manager.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/utils/git_manager.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/utils/host_cleaner.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/utils/host_cleaner.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/utils/java_home_resolver.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/utils/java_home_resolver.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/utils/jdk_resolver.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/utils/jdk_resolver.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/utils/path_manager.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/utils/path_manager.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/builder/utils/template_renderer.py` & `opensearch_benchmark-1.5.0/osbenchmark/builder/utils/template_renderer.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/client.py` & `opensearch_benchmark-1.5.0/osbenchmark/client.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/config.py` & `opensearch_benchmark-1.5.0/osbenchmark/config.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/exceptions.py` & `opensearch_benchmark-1.5.0/osbenchmark/exceptions.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/log.py` & `opensearch_benchmark-1.5.0/osbenchmark/log.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/metrics.py` & `opensearch_benchmark-1.5.0/osbenchmark/metrics.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/paths.py` & `opensearch_benchmark-1.5.0/osbenchmark/paths.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/resources/base-workload.json.j2` & `opensearch_benchmark-1.5.0/osbenchmark/resources/base-workload.json.j2`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/resources/benchmark.ini` & `opensearch_benchmark-1.5.0/osbenchmark/resources/benchmark.ini`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/resources/custom-operations.json.j2` & `opensearch_benchmark-1.5.0/osbenchmark/resources/custom-operations.json.j2`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/resources/custom-test-procedures.json.j2` & `opensearch_benchmark-1.5.0/osbenchmark/resources/custom-test-procedures.json.j2`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/resources/default-operations.json.j2` & `opensearch_benchmark-1.5.0/osbenchmark/resources/default-operations.json.j2`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/resources/default-test-procedures.json.j2` & `opensearch_benchmark-1.5.0/osbenchmark/resources/default-test-procedures.json.j2`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/resources/docker-compose.yml.j2` & `opensearch_benchmark-1.5.0/osbenchmark/resources/docker-compose.yml.j2`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/resources/logging.json` & `opensearch_benchmark-1.5.0/osbenchmark/resources/logging.json`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/resources/metrics-template.json` & `opensearch_benchmark-1.5.0/osbenchmark/resources/metrics-template.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'settings'": "{'index': {replace: OrderedDict([('mapping.total_fields.limit', 2000)])}}"}*

```diff
@@ -85,10 +85,12 @@
             },
             "workload": {
                 "type": "keyword"
             }
         }
     },
     "settings": {
-        "index": {}
+        "index": {
+            "mapping.total_fields.limit": 2000
+        }
     }
 }
```

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/core-plugins.txt` & `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/core-plugins.txt`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/README.md` & `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/README.md`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/plugin.py` & `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/plugin.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/README.md` & `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/README.md`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/plugin.py` & `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/plugin.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/README.md` & `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/README.md`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/plugin.py` & `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/plugin.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/config.ini` & `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/config.ini`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/README.md` & `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/README.md`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/config.ini` & `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/config.ini`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/jvm.options` & `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/jvm.options`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/log4j2.properties` & `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/log4j2.properties`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/opensearch.yml` & `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/opensearch.yml`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/plugins/v1/core-plugins.txt` & `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/core-plugins.txt`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/README.md` & `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/README.md`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/plugin.py` & `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/plugin.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/README.md` & `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/README.md`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/plugin.py` & `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/plugin.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/README.md` & `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/README.md`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/plugin.py` & `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/plugin.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/README.md` & `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/README.md`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/config.ini` & `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/config.ini`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/jvm.options` & `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/jvm.options`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/log4j2.properties` & `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/log4j2.properties`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/opensearch.yml` & `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/opensearch.yml`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/resources/results-template.json` & `opensearch_benchmark-1.5.0/osbenchmark/resources/results-template.json`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/resources/test-executions-template.json` & `opensearch_benchmark-1.5.0/osbenchmark/resources/test-executions-template.json`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/resources/workload-schema.json` & `opensearch_benchmark-1.5.0/osbenchmark/resources/workload-schema.json`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/results_publisher.py` & `opensearch_benchmark-1.5.0/osbenchmark/results_publisher.py`

 * *Files 0% similar despite different names*

```diff
@@ -333,22 +333,23 @@
             return [k, task, converter(v), u]
         else:
             return []
 
 
 class ComparisonResultsPublisher:
     def __init__(self, config):
+        self.logger = logging.getLogger(__name__)
         self.results_file = config.opts("results_publishing", "output.path")
         self.results_format = config.opts("results_publishing", "format")
         self.numbers_align = config.opts("results_publishing", "numbers.align",
                                          mandatory=False, default_value="right")
         self.cwd = config.opts("node", "benchmark.cwd")
         self.show_processing_time = convert.to_bool(config.opts("results_publishing", "output.processingtime",
                                                                 mandatory=False, default_value=False))
-        self.latency_percentiles = comma_separated_string_to_number_list(config.opts("workload", "latency.percentiles", mandatory=False))
+        self.percentiles = comma_separated_string_to_number_list(config.opts("results_publishing", "percentiles", mandatory=False))
         self.plain = False
 
     def publish(self, r1, r2):
         # we don't verify anything about the test_executions as it is possible
         # that the user benchmarks two different workloads intentionally
         baseline_stats = metrics.GlobalStats(r1.results)
         contender_stats = metrics.GlobalStats(r2.results)
@@ -438,15 +439,15 @@
     def _publish_processing_time(self, baseline_stats, contender_stats, task):
         baseline_processing_time = baseline_stats.metrics(task)["processing_time"]
         contender_processing_time = contender_stats.metrics(task)["processing_time"]
         return self._publish_percentiles("processing time", task, baseline_processing_time, contender_processing_time)
 
     def _publish_percentiles(self, name, task, baseline_values, contender_values):
         lines = []
-        for percentile in metrics.percentiles_for_sample_size(sys.maxsize, percentiles_list=self.latency_percentiles):
+        for percentile in metrics.percentiles_for_sample_size(sys.maxsize, percentiles_list=self.percentiles):
             baseline_value = baseline_values.get(metrics.encode_float_key(percentile))
             contender_value = contender_values.get(metrics.encode_float_key(percentile))
             self._append_non_empty(lines, self._line("%sth percentile %s" % (percentile, name),
                                                      baseline_value, contender_value, task, "ms",
                                                      treat_increase_as_improvement=False))
         return lines
```

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/telemetry.py` & `opensearch_benchmark-1.5.0/osbenchmark/telemetry.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/test_execution_orchestrator.py` & `opensearch_benchmark-1.5.0/osbenchmark/test_execution_orchestrator.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/time.py` & `opensearch_benchmark-1.5.0/osbenchmark/time.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/utils/__init__.py` & `opensearch_benchmark-1.5.0/osbenchmark/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/utils/collections.py` & `opensearch_benchmark-1.5.0/osbenchmark/utils/collections.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/utils/console.py` & `opensearch_benchmark-1.5.0/osbenchmark/utils/console.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/utils/convert.py` & `opensearch_benchmark-1.5.0/osbenchmark/utils/convert.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/utils/dataset.py` & `opensearch_benchmark-1.5.0/osbenchmark/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/utils/git.py` & `opensearch_benchmark-1.5.0/osbenchmark/utils/git.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/utils/io.py` & `opensearch_benchmark-1.5.0/osbenchmark/utils/io.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/utils/jvm.py` & `opensearch_benchmark-1.5.0/osbenchmark/utils/jvm.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/utils/modules.py` & `opensearch_benchmark-1.5.0/osbenchmark/utils/modules.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/utils/net.py` & `opensearch_benchmark-1.5.0/osbenchmark/utils/net.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/utils/opts.py` & `opensearch_benchmark-1.5.0/osbenchmark/utils/opts.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/utils/parse.py` & `opensearch_benchmark-1.5.0/osbenchmark/utils/parse.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/utils/periodic_waiter.py` & `opensearch_benchmark-1.5.0/osbenchmark/utils/periodic_waiter.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/utils/process.py` & `opensearch_benchmark-1.5.0/osbenchmark/utils/process.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/utils/repo.py` & `opensearch_benchmark-1.5.0/osbenchmark/utils/repo.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/utils/sysstats.py` & `opensearch_benchmark-1.5.0/osbenchmark/utils/sysstats.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/utils/versions.py` & `opensearch_benchmark-1.5.0/osbenchmark/utils/versions.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/version.py` & `opensearch_benchmark-1.5.0/osbenchmark/version.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/worker_coordinator/__init__.py` & `opensearch_benchmark-1.5.0/osbenchmark/worker_coordinator/__init__.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/worker_coordinator/errors.py` & `opensearch_benchmark-1.5.0/osbenchmark/worker_coordinator/errors.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/worker_coordinator/runner.py` & `opensearch_benchmark-1.5.0/osbenchmark/worker_coordinator/runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 from functools import total_ordering
 from io import BytesIO
 from os.path import commonprefix
 from typing import List, Optional
 
 import ijson
 from opensearchpy import ConnectionTimeout
+from opensearchpy import NotFoundError
 
 from osbenchmark import exceptions, workload
 from osbenchmark.utils import convert
 from osbenchmark.client import RequestContextHolder
 # Mapping from operation type to specific runner
 from osbenchmark.utils.parse import parse_int_parameter, parse_string_parameter
 
@@ -74,14 +75,15 @@
     register_runner(workload.OperationType.Sleep, Sleep(), async_runner=True)
     # these requests should not be retried as they are not idempotent
     register_runner(workload.OperationType.CreateSnapshot, CreateSnapshot(), async_runner=True)
     register_runner(workload.OperationType.RestoreSnapshot, RestoreSnapshot(), async_runner=True)
     # We treat the following as administrative commands and thus already start to wrap them in a retry.
     register_runner(workload.OperationType.ClusterHealth, Retry(ClusterHealth()), async_runner=True)
     register_runner(workload.OperationType.PutPipeline, Retry(PutPipeline()), async_runner=True)
+    register_runner(workload.OperationType.DeletePipeline, Retry(DeletePipeline()), async_runner=True)
     register_runner(workload.OperationType.Refresh, Retry(Refresh()), async_runner=True)
     register_runner(workload.OperationType.CreateIndex, Retry(CreateIndex()), async_runner=True)
     register_runner(workload.OperationType.DeleteIndex, Retry(DeleteIndex()), async_runner=True)
     register_runner(workload.OperationType.CreateComponentTemplate, Retry(CreateComponentTemplate()), async_runner=True)
     register_runner(workload.OperationType.DeleteComponentTemplate, Retry(DeleteComponentTemplate()), async_runner=True)
     register_runner(workload.OperationType.CreateComposableTemplate, Retry(CreateComposableTemplate()), async_runner=True)
     register_runner(workload.OperationType.DeleteComposableTemplate, Retry(DeleteComposableTemplate()), async_runner=True)
@@ -96,14 +98,17 @@
     register_runner(workload.OperationType.WaitForRecovery, Retry(IndicesRecovery()), async_runner=True)
     register_runner(workload.OperationType.PutSettings, Retry(PutSettings()), async_runner=True)
     register_runner(workload.OperationType.CreateTransform, Retry(CreateTransform()), async_runner=True)
     register_runner(workload.OperationType.StartTransform, Retry(StartTransform()), async_runner=True)
     register_runner(workload.OperationType.WaitForTransform, Retry(WaitForTransform()), async_runner=True)
     register_runner(workload.OperationType.DeleteTransform, Retry(DeleteTransform()), async_runner=True)
     register_runner(workload.OperationType.CreateSearchPipeline, Retry(CreateSearchPipeline()), async_runner=True)
+    register_runner(workload.OperationType.DeleteMlModel, Retry(DeleteMlModel()), async_runner=True)
+    register_runner(workload.OperationType.RegisterMlModel, Retry(RegisterMlModel()), async_runner=True)
+    register_runner(workload.OperationType.DeployMlModel, Retry(DeployMlModel()), async_runner=True)
 
 
 def runner_for(operation_type):
     try:
         return __RUNNERS[operation_type]
     except KeyError:
         raise exceptions.BenchmarkError("No runner available for operation type [%s]" % operation_type)
@@ -149,15 +154,14 @@
     else:
         if logger.isEnabledFor(logging.DEBUG):
             logger.debug("Registering runner object [%s] for [%s].", str(runner), str(operation_type))
         cluster_aware_runner = _single_cluster_runner(runner, str(runner))
 
     __RUNNERS[operation_type] = _with_completion(_with_assertions(cluster_aware_runner))
 
-
 # Only intended for unit-testing!
 def remove_runner(operation_type):
     del __RUNNERS[operation_type]
 
 
 class Runner:
     """
@@ -212,17 +216,19 @@
         return request_params, headers
 
 request_context_holder = RequestContextHolder()
 
 def time_func(func):
     async def advised(*args, **kwargs):
         request_context_holder.on_client_request_start()
-        response = await func(*args, **kwargs)
-        request_context_holder.on_client_request_end()
-        return response
+        try:
+            response = await func(*args, **kwargs)
+            return response
+        finally:
+            request_context_holder.on_client_request_end()
     return advised
 
 
 class Delegator:
     """
     Mixin to unify delegate handling
     """
@@ -471,31 +477,37 @@
         contain actual documents to index)
         * ``index``: The name of the affected index in case ``action_metadata_present`` is ``False``.
         * ``type``: The name of the affected type in case ``action_metadata_present`` is ``False``.
 
         The following keys are optional:
 
         * ``pipeline``: If present, runs the the specified ingest pipeline for this bulk.
+        * ``request-params``: If present, they will be passed as parameters of bulk.
         * ``detailed-results``: If ``True``, the runner will analyze the response and add detailed meta-data. Defaults to ``False``. Note
         that this has a very significant impact on performance and will very
         likely cause a bottleneck in the benchmark worker_coordinator so please
         be very cautious enabling this feature. Our own measurements have shown a median overhead of several thousand times (execution time
          is in the single digit microsecond range when this feature is disabled and in the single digit millisecond range when this feature
          is enabled; numbers based on a bulk size of 500 elements and no errors). For details please refer to the respective benchmarks
          in ``benchmarks/worker_coordinator``.
         * ``request-timeout``: a non-negative float indicating the client-side timeout for the operation.  If not present, defaults to
          ``None`` and potentially falls back to the global timeout setting.
         """
         detailed_results = params.get("detailed-results", False)
-        api_kwargs = self._default_kw_params(params)
 
         bulk_params = {}
         if "pipeline" in params:
             bulk_params["pipeline"] = params["pipeline"]
 
+        if "request-params" in params:
+            bulk_params.update(params["request-params"])
+            params.pop( "request-params" )
+
+        api_kwargs = self._default_kw_params(params)
+
         with_action_metadata = mandatory(params, "action-metadata-present", self)
         bulk_size = mandatory(params, "bulk-size", self)
         unit = mandatory(params, "unit", self)
         # parse responses lazily in the standard case - responses might be large thus parsing skews results and if no
         # errors have occurred we only need a small amount of information from the potentially large response.
         if not detailed_results:
             opensearch.return_raw_response()
@@ -672,38 +684,47 @@
 
 
 class ForceMerge(Runner):
     """
     Runs a force merge operation against OpenSearch.
     """
 
+    PARAM_WAIT_FOR_COMPLETION = "wait_for_completion"
+
     async def __call__(self, opensearch, params):
-        # pylint: disable=import-outside-toplevel
-        import opensearchpy
         max_num_segments = params.get("max-num-segments")
         mode = params.get("mode")
         merge_params = self._default_kw_params(params)
         if max_num_segments:
             merge_params["max_num_segments"] = max_num_segments
+        # Request end time will not be 100% accurate, since we are using polling
+        # to check whether task status is completed or not.
         if mode == "polling":
-            complete = False
-            try:
-                request_context_holder.on_client_request_start()
-                await opensearch.indices.forcemerge(**merge_params)
-                request_context_holder.on_client_request_end()
-                complete = True
-            except opensearchpy.ConnectionTimeout:
-                pass
-            while not complete:
-                await asyncio.sleep(params.get("poll-period"))
-                tasks = await opensearch.tasks.list(params={"actions": "indices:admin/forcemerge"})
-                if len(tasks["nodes"]) == 0:
-                    # empty nodes response indicates no tasks
+            self.logger.warning(
+                "%s will be updated to false to run force merge in asynchronous way", self.PARAM_WAIT_FOR_COMPLETION)
+            merge_params[self.PARAM_WAIT_FOR_COMPLETION] = "false"
+            request_context_holder.on_client_request_start()
+            response_task = await opensearch.indices.forcemerge(**merge_params)
+            while True:
+                force_merge_task_id = response_task['task']
+                task = await opensearch.tasks.get(task_id=force_merge_task_id)
+                if not task:
+                    self.logger.error("Failed to get task for task id: [%s]", force_merge_task_id)
+                    request_context_holder.on_client_request_end()
+                    raise exceptions.BenchmarkAssertionError(
+                        "Force merge request failure: task was expected but not found in the get tasks api response.")
+                if 'completed' not in task:
                     request_context_holder.on_client_request_end()
-                    complete = True
+                    raise exceptions.BenchmarkAssertionError(
+                        "Force merge request failure: 'completed' was expected but not found "
+                        "in the get task api response.")
+                if task['completed']:
+                    request_context_holder.on_client_request_end()
+                    break
+                await asyncio.sleep(params.get("poll-period"))
         else:
             request_context_holder.on_client_request_start()
             await opensearch.indices.forcemerge(**merge_params)
             request_context_holder.on_client_request_end()
 
     def __repr__(self, *args, **kwargs):
         return "force-merge"
@@ -1268,14 +1289,28 @@
                                      master_timeout=params.get("master-timeout"),
                                      timeout=params.get("timeout"),
                                      )
 
     def __repr__(self, *args, **kwargs):
         return "put-pipeline"
 
+class DeletePipeline(Runner):
+    @time_func
+    async def __call__(self, opensearch, params):
+        try:
+            await opensearch.ingest.delete_pipeline(id=mandatory(params, "id", self),
+                                                    master_timeout=params.get("master-timeout"),
+                                                    timeout=params.get("timeout"),
+                                                    )
+        except NotFoundError:
+            self.logger.info("No current pipeline [%s] to delete.", params.get("id"))
+
+    def __repr__(self, *args, **kwargs):
+        return "delete-pipeline"
+
 # TODO: refactor it after python client support search pipeline https://github.com/opensearch-project/opensearch-py/issues/474
 class CreateSearchPipeline(Runner):
     @time_func
     async def __call__(self, opensearch, params):
         endpoint = "/_search/pipeline/" + mandatory(params, "id", self)
         await opensearch.transport.perform_request(method="PUT", url=endpoint, body=mandatory(params, "body", self))
 
@@ -1665,18 +1700,21 @@
 
 class Sleep(Runner):
     """
     Sleeps for the specified duration not issuing any request.
     """
 
     async def __call__(self, opensearch, params):
+        sleep_duration = mandatory(params, "duration", "sleep")
         opensearch.on_request_start()
         try:
-            await asyncio.sleep(mandatory(params, "duration", "sleep"))
+            request_context_holder.on_client_request_start()
+            await asyncio.sleep(sleep_duration)
         finally:
+            request_context_holder.on_client_request_end()
             opensearch.on_request_end()
 
     def __repr__(self, *args, **kwargs):
         return "sleep"
 
 
 class DeleteSnapshotRepository(Runner):
@@ -2354,7 +2392,115 @@
                     raise e
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         return await self.delegate.__aexit__(exc_type, exc_val, exc_tb)
 
     def __repr__(self, *args, **kwargs):
         return "retryable %s" % repr(self.delegate)
+
+class DeleteMlModel(Runner):
+    @time_func
+    async def __call__(self, opensearch, params):
+        body= {
+            "query": {
+                "match_phrase": {
+                    "name": {
+                        "query": params.get('model-name')
+                    }
+                }
+            },
+            "size": params.get('number-of-hits-to-return', 1000)
+        }
+
+        model_ids = set()
+
+        resp = await opensearch.transport.perform_request('POST', '/_plugins/_ml/models/_search', body=body)
+        for item in resp['hits']['hits']:
+            doc = item.get('_source')
+            if doc:
+                id = doc.get('model_id')
+                if id:
+                    model_ids.add(id)
+
+        for model_id in model_ids:
+            resp=await opensearch.transport.perform_request('POST', '/_plugins/_ml/models/' + model_id + '/_undeploy')
+            resp=await opensearch.transport.perform_request('DELETE', '/_plugins/_ml/models/' + model_id)
+
+    def __repr__(self, *args, **kwargs):
+        return "delete-ml-model"
+
+class RegisterMlModel(Runner):
+    @time_func
+    async def __call__(self, opensearch, params):
+        config_file = params.get('model-config-file')
+        if config_file:
+            with open(config_file, 'r') as f:
+                body = json.loads(f.read())
+        else:
+            body = {
+                "name": params.get('model-name'),
+                "version": params.get('model-version'),
+                "model_format": params.get('model-format')
+            }
+        search_body = {
+            "query": {
+                "match": {
+                    "name": body['name']
+                }
+            }
+        }
+        model_id = None
+
+        resp = await opensearch.transport.perform_request('POST', '/_plugins/_ml/models/_search', body=search_body)
+        for item in resp['hits']['hits']:
+            doc = item.get('_source')
+            if doc:
+                model_id = doc.get('model_id')
+                if model_id:
+                    break
+
+        if not model_id:
+            resp = await opensearch.transport.perform_request('POST', '_plugins/_ml/models/_register', body=body)
+            task_id = resp.get('task_id')
+            timeout = params.get('timeout', 120)
+            end = time.time() + timeout
+            state = 'CREATED'
+            while state == 'CREATED' and time.time() < end:
+                await asyncio.sleep(5)
+                resp = await opensearch.transport.perform_request('GET', '_plugins/_ml/tasks/' + task_id)
+                state = resp.get('state')
+            if state == 'FAILED':
+                raise exceptions.BenchmarkError("Failed to register ml-model. Error: {}".format(resp['error']))
+            if state == 'CREATED':
+                raise TimeoutError("Timeout when registering ml-model.")
+            model_id = resp.get('model_id')
+
+        with open('model_id.json', 'w') as f:
+            d = { 'model_id': model_id }
+            f.write(json.dumps(d))
+
+    def __repr__(self, *args, **kwargs):
+        return "register-ml-model"
+
+class DeployMlModel(Runner):
+    @time_func
+    async def __call__(self, opensearch, params):
+        with open('model_id.json', 'r') as f:
+            d = json.loads(f.read())
+            model_id = d['model_id']
+
+        resp = await opensearch.transport.perform_request('POST', '_plugins/_ml/models/' + model_id + '/_deploy')
+        task_id = resp.get('task_id')
+        timeout = params.get('timeout', 120)
+        end = time.time() + timeout
+        state = 'RUNNING'
+        while state == 'RUNNING' and time.time() < end:
+            await asyncio.sleep(5)
+            resp = await opensearch.transport.perform_request('GET', '_plugins/_ml/tasks/' + task_id)
+            state = resp.get('state')
+        if state == 'FAILED':
+            raise exceptions.BenchmarkError("Failed to deploy ml-model. Error: {}".format(resp['error']))
+        if state == 'RUNNING':
+            raise TimeoutError("Timeout when deploying ml-model.")
+
+    def __repr__(self, *args, **kwargs):
+        return "deploy-ml-model"
```

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/worker_coordinator/scheduler.py` & `opensearch_benchmark-1.5.0/osbenchmark/worker_coordinator/scheduler.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/worker_coordinator/worker_coordinator.py` & `opensearch_benchmark-1.5.0/osbenchmark/worker_coordinator/worker_coordinator.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/workload/__init__.py` & `opensearch_benchmark-1.5.0/osbenchmark/workload/__init__.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/workload/loader.py` & `opensearch_benchmark-1.5.0/osbenchmark/workload/loader.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/workload/params.py` & `opensearch_benchmark-1.5.0/osbenchmark/workload/params.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/workload/workload.py` & `opensearch_benchmark-1.5.0/osbenchmark/workload/workload.py`

 * *Files 1% similar despite different names*

```diff
@@ -602,20 +602,21 @@
     VectorSearch = 17
     BulkVectorDataSet = 18
 
     # administrative actions
     ForceMerge = 1001
     ClusterHealth = 1002
     PutPipeline = 1003
-    Refresh = 1004
-    CreateIndex = 1005
-    DeleteIndex = 1006
-    CreateIndexTemplate = 1007
-    DeleteIndexTemplate = 1008
-    ShrinkIndex = 1009
+    DeletePipeline = 1004
+    Refresh = 1005
+    CreateIndex = 1006
+    DeleteIndex = 1007
+    CreateIndexTemplate = 1008
+    DeleteIndexTemplate = 1009
+    ShrinkIndex = 1010
     Sleep = 1018
     DeleteSnapshotRepository = 1019
     CreateSnapshotRepository = 1020
     CreateSnapshot = 1021
     RestoreSnapshot = 1022
     PutSettings = 1023
     CreateTransform = 1024
@@ -625,14 +626,17 @@
     CreateDataStream = 1028
     DeleteDataStream = 1029
     CreateComposableTemplate = 1030
     DeleteComposableTemplate = 1031
     CreateComponentTemplate = 1032
     DeleteComponentTemplate = 1033
     CreateSearchPipeline = 1040
+    DeleteMlModel = 1041
+    RegisterMlModel = 1042
+    DeployMlModel = 1043
 
     @property
     def admin_op(self):
         # pylint: disable=comparison-with-callable
         return self.value > 1000
 
     def to_hyphenated_string(self):
@@ -666,14 +670,16 @@
             return OperationType.ClusterHealth
         elif v == "bulk":
             return OperationType.Bulk
         elif v == "raw-request":
             return OperationType.RawRequest
         elif v == "put-pipeline":
             return OperationType.PutPipeline
+        elif v == "delete-pipeline":
+            return OperationType.DeletePipeline
         elif v == "refresh":
             return OperationType.Refresh
         elif v == "create-index":
             return OperationType.CreateIndex
         elif v == "delete-index":
             return OperationType.DeleteIndex
         elif v == "create-index-template":
@@ -730,14 +736,20 @@
             return OperationType.CreatePointInTime
         elif v == "delete-point-in-time":
             return OperationType.DeletePointInTime
         elif v == "list-all-point-in-time":
             return OperationType.ListAllPointInTime
         elif v == "create-search-pipeline":
             return OperationType.CreateSearchPipeline
+        elif v == "delete-ml-model":
+            return OperationType.DeleteMlModel
+        elif v == "register-ml-model":
+            return OperationType.RegisterMlModel
+        elif v == "deploy-ml-model":
+            return OperationType.DeployMlModel
         else:
             raise KeyError(f"No enum value for [{v}]")
 
 @unique
 class IndexCodec(Enum):
     Default = "default"
     BestCompression = "best_compression"
```

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/workload_generator/__init__.py` & `opensearch_benchmark-1.5.0/osbenchmark/workload_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/workload_generator/corpus.py` & `opensearch_benchmark-1.5.0/osbenchmark/workload_generator/corpus.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/workload_generator/index.py` & `opensearch_benchmark-1.5.0/osbenchmark/workload_generator/index.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/osbenchmark/workload_generator/workload_generator.py` & `opensearch_benchmark-1.5.0/osbenchmark/workload_generator/workload_generator.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/scripts/expand-data-corpus.py` & `opensearch_benchmark-1.5.0/scripts/expand-data-corpus.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/setup.py` & `opensearch_benchmark-1.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,60 +56,61 @@
 #
 ################################################################################################
 install_requires = [
     # License: Apache 2.0
     # transitive dependencies:
     #   urllib3: MIT
     #   aiohttp: Apache 2.0
-    "opensearch-py[async]==2.5.0",
+    "opensearch-py[async]>=2.5.0",
     # License: BSD
-    "psutil==5.8.0",
+    "psutil>=5.8.0",
     # License: MIT
-    "py-cpuinfo==7.0.0",
+    "py-cpuinfo>=7.0.0",
     # License: MIT
-    "tabulate==0.9.0",
+    "tabulate>=0.9.0",
     # License: MIT
-    "jsonschema==3.1.1",
+    "jsonschema>=3.1.1",
     # License: BSD
-    "Jinja2==3.1.3",
+    "Jinja2>=3.1.3",
     # License: BSD
-    "markupsafe==2.0.1",
+    "markupsafe>=2.0.1",
     # License: MIT
-    "thespian==3.10.1",
+    # With 3.10.7, we get InvalidActorAddress exception while initialize Actor
+    "thespian>=3.10.1,<3.10.7",
     # recommended library for thespian to identify actors more easily with `ps`
     # "setproctitle==1.1.10",
     # always use the latest version, these are certificate files...
     # License: MPL 2.0
     "certifi",
     # License: Apache 2.0
-    "yappi==1.4.0",
+    "yappi>=1.4.0",
     # License: BSD
-    "ijson==2.6.1",
+    "ijson>=2.6.1",
     # License: Apache 2.0
     # transitive dependencies:
     #   google-crc32c: Apache 2.0
-    "google-resumable-media==1.1.0",
+    "google-resumable-media>=1.1.0",
     # License: Apache 2.0
-    "google-auth==1.22.1",
+    "google-auth>=1.22.1",
     # License: MIT
-    "wheel==0.38.4",
+    "wheel>=0.38.4",
     # License: Apache 2.0
     # transitive dependencies:
     #   botocore: Apache 2.0
     #   jmespath: MIT
     #   s3transfer: Apache 2.0
-    "boto3==1.28.62",
+    "boto3>=1.28.62",
     # Licence: BSD-3-Clause
-    "zstandard==0.22.0",
+    "zstandard>=0.22.0",
     # License: BSD
     # Required for knnvector workload
-    "h5py==3.10.0",
+    "h5py>=3.10.0",
     # License: BSD
     # Required for knnvector workload
-    "numpy==1.24.2",
+    "numpy>=1.24.2",
 ]
 
 tests_require = [
     "ujson",
     "pytest==7.2.2",
     "pytest-benchmark==3.2.2",
     "pytest-asyncio==0.14.0"
```

### Comparing `opensearch-benchmark-1.4.0/tests/test_async_connection.py` & `opensearch_benchmark-1.5.0/tests/test_async_connection.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-1.4.0/tests/test_execution_orchestrator_test.py` & `opensearch_benchmark-1.5.0/tests/test_execution_orchestrator_test.py`

 * *Files identical despite different names*

