# Comparing `tmp/kpops-4.1.2.tar.gz` & `tmp/kpops-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kpops-4.1.2.tar", max compression
+gzip compressed data, was "kpops-4.2.0.tar", max compression
```

## Comparing `kpops-4.1.2.tar` & `kpops-4.2.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     1064 2024-03-11 15:42:11.354073 kpops-4.1.2/LICENSE
--rw-r--r--   0        0        0     2678 2024-03-11 15:42:11.354073 kpops-4.1.2/README.md
--rw-r--r--   0        0        0      250 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/__init__.py
--rw-r--r--   0        0        0        0 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/cli/__init__.py
--rw-r--r--   0        0        0      761 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/cli/custom_formatter.py
--rw-r--r--   0        0        0      124 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/cli/exception.py
--rw-r--r--   0        0        0    16065 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/cli/main.py
--rw-r--r--   0        0        0      101 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/cli/options.py
--rw-r--r--   0        0        0     2512 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/cli/registry.py
--rw-r--r--   0        0        0      699 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/component_handlers/__init__.py
--rw-r--r--   0        0        0        0 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/component_handlers/helm_wrapper/__init__.py
--rw-r--r--   0        0        0     1168 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/component_handlers/helm_wrapper/dry_run_handler.py
--rw-r--r--   0        0        0       92 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/component_handlers/helm_wrapper/exception.py
--rw-r--r--   0        0        0     8950 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/component_handlers/helm_wrapper/helm.py
--rw-r--r--   0        0        0     2125 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/component_handlers/helm_wrapper/helm_diff.py
--rw-r--r--   0        0        0     7076 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/component_handlers/helm_wrapper/model.py
--rw-r--r--   0        0        0      974 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/component_handlers/helm_wrapper/utils.py
--rw-r--r--   0        0        0        0 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/component_handlers/kafka_connect/__init__.py
--rw-r--r--   0        0        0     7412 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/component_handlers/kafka_connect/connect_wrapper.py
--rw-r--r--   0        0        0      229 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/component_handlers/kafka_connect/exception.py
--rw-r--r--   0        0        0     5460 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/component_handlers/kafka_connect/kafka_connect_handler.py
--rw-r--r--   0        0        0     3543 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/component_handlers/kafka_connect/model.py
--rw-r--r--   0        0        0      797 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/component_handlers/kafka_connect/timeout.py
--rw-r--r--   0        0        0        0 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/component_handlers/kubernetes/__init__.py
--rw-r--r--   0        0        0      841 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/component_handlers/kubernetes/model.py
--rw-r--r--   0        0        0     1116 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/component_handlers/kubernetes/utils.py
--rw-r--r--   0        0        0        0 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/component_handlers/schema_handler/__init__.py
--rw-r--r--   0        0        0     6774 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/component_handlers/schema_handler/schema_handler.py
--rw-r--r--   0        0        0      499 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/component_handlers/schema_handler/schema_provider.py
--rw-r--r--   0        0        0        0 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/component_handlers/topic/__init__.py
--rw-r--r--   0        0        0      225 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/component_handlers/topic/exception.py
--rw-r--r--   0        0        0     9534 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/component_handlers/topic/handler.py
--rw-r--r--   0        0        0     2420 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/component_handlers/topic/model.py
--rw-r--r--   0        0        0     7345 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/component_handlers/topic/proxy_wrapper.py
--rw-r--r--   0        0        0     2385 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/component_handlers/topic/utils.py
--rw-r--r--   0        0        0        0 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/component_handlers/utils/__init__.py
--rw-r--r--   0        0        0      625 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/component_handlers/utils/exception.py
--rw-r--r--   0        0        0      906 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/components/__init__.py
--rw-r--r--   0        0        0        0 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/components/base_components/__init__.py
--rw-r--r--   0        0        0    10674 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/components/base_components/base_defaults_component.py
--rw-r--r--   0        0        0     1061 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/components/base_components/cleaner.py
--rw-r--r--   0        0        0     7235 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/components/base_components/helm_app.py
--rw-r--r--   0        0        0     4748 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/components/base_components/kafka_app.py
--rw-r--r--   0        0        0     9178 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/components/base_components/kafka_connector.py
--rw-r--r--   0        0        0     1828 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/components/base_components/kubernetes_app.py
--rw-r--r--   0        0        0      149 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/components/base_components/models/__init__.py
--rw-r--r--   0        0        0     1882 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/components/base_components/models/from_section.py
--rw-r--r--   0        0        0      217 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/components/base_components/models/resource.py
--rw-r--r--   0        0        0      994 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/components/base_components/models/to_section.py
--rw-r--r--   0        0        0     3801 2024-03-11 15:42:11.362073 kpops-4.1.2/kpops/components/base_components/models/topic.py
--rw-r--r--   0        0        0     8324 2024-03-11 15:42:11.366073 kpops-4.1.2/kpops/components/base_components/pipeline_component.py
--rw-r--r--   0        0        0     1031 2024-03-11 15:42:11.366073 kpops-4.1.2/kpops/components/streams_bootstrap/__init__.py
--rw-r--r--   0        0        0      217 2024-03-11 15:42:11.366073 kpops-4.1.2/kpops/components/streams_bootstrap/app_type.py
--rw-r--r--   0        0        0        0 2024-03-11 15:42:11.366073 kpops-4.1.2/kpops/components/streams_bootstrap/producer/__init__.py
--rw-r--r--   0        0        0      595 2024-03-11 15:42:11.366073 kpops-4.1.2/kpops/components/streams_bootstrap/producer/model.py
--rw-r--r--   0        0        0     2873 2024-03-11 15:42:11.366073 kpops-4.1.2/kpops/components/streams_bootstrap/producer/producer_app.py
--rw-r--r--   0        0        0        0 2024-03-11 15:42:11.366073 kpops-4.1.2/kpops/components/streams_bootstrap/streams/__init__.py
--rw-r--r--   0        0        0     8649 2024-03-11 15:42:11.366073 kpops-4.1.2/kpops/components/streams_bootstrap/streams/model.py
--rw-r--r--   0        0        0     3309 2024-03-11 15:42:11.366073 kpops-4.1.2/kpops/components/streams_bootstrap/streams/streams_app.py
--rw-r--r--   0        0        0     5147 2024-03-11 15:42:11.366073 kpops-4.1.2/kpops/config.py
--rw-r--r--   0        0        0    15199 2024-03-11 15:42:11.366073 kpops-4.1.2/kpops/pipeline.py
--rw-r--r--   0        0        0      278 2024-03-11 15:42:11.366073 kpops-4.1.2/kpops/utils/__init__.py
--rw-r--r--   0        0        0     3060 2024-03-11 15:42:11.366073 kpops-4.1.2/kpops/utils/cli_commands.py
--rw-r--r--   0        0        0      375 2024-03-11 15:42:11.366073 kpops-4.1.2/kpops/utils/colorify.py
--rw-r--r--   0        0        0     3178 2024-03-11 15:42:11.366073 kpops-4.1.2/kpops/utils/dict_differ.py
--rw-r--r--   0        0        0     4996 2024-03-11 15:42:11.366073 kpops-4.1.2/kpops/utils/dict_ops.py
--rw-r--r--   0        0        0     2431 2024-03-11 15:42:11.366073 kpops-4.1.2/kpops/utils/docstring.py
--rw-r--r--   0        0        0     1176 2024-03-11 15:42:11.366073 kpops-4.1.2/kpops/utils/environment.py
--rw-r--r--   0        0        0     5928 2024-03-11 15:42:11.366073 kpops-4.1.2/kpops/utils/gen_schema.py
--rw-r--r--   0        0        0      298 2024-03-11 15:42:11.366073 kpops-4.1.2/kpops/utils/json.py
--rw-r--r--   0        0        0     6533 2024-03-11 15:42:11.366073 kpops-4.1.2/kpops/utils/pydantic.py
--rw-r--r--   0        0        0      238 2024-03-11 15:42:11.366073 kpops-4.1.2/kpops/utils/types.py
--rw-r--r--   0        0        0     4332 2024-03-11 15:42:11.366073 kpops-4.1.2/kpops/utils/yaml.py
--rw-r--r--   0        0        0     7175 2024-03-11 15:42:11.366073 kpops-4.1.2/pyproject.toml
--rw-r--r--   0        0        0     4238 1970-01-01 00:00:00.000000 kpops-4.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-25 12:04:45.132307 kpops-4.2.0/LICENSE
+-rw-r--r--   0        0        0     2678 2024-04-25 12:04:45.132307 kpops-4.2.0/README.md
+-rw-r--r--   0        0        0      250 2024-04-25 12:04:45.136307 kpops-4.2.0/kpops/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:04:45.136307 kpops-4.2.0/kpops/cli/__init__.py
+-rw-r--r--   0        0        0      761 2024-04-25 12:04:45.136307 kpops-4.2.0/kpops/cli/custom_formatter.py
+-rw-r--r--   0        0        0      124 2024-04-25 12:04:45.136307 kpops-4.2.0/kpops/cli/exception.py
+-rw-r--r--   0        0        0    16061 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/cli/main.py
+-rw-r--r--   0        0        0      101 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/cli/options.py
+-rw-r--r--   0        0        0     2512 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/cli/registry.py
+-rw-r--r--   0        0        0      699 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/component_handlers/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/component_handlers/helm_wrapper/__init__.py
+-rw-r--r--   0        0        0     1168 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/component_handlers/helm_wrapper/dry_run_handler.py
+-rw-r--r--   0        0        0       92 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/component_handlers/helm_wrapper/exception.py
+-rw-r--r--   0        0        0     8950 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/component_handlers/helm_wrapper/helm.py
+-rw-r--r--   0        0        0     2125 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/component_handlers/helm_wrapper/helm_diff.py
+-rw-r--r--   0        0        0     7072 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/component_handlers/helm_wrapper/model.py
+-rw-r--r--   0        0        0      974 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/component_handlers/helm_wrapper/utils.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/component_handlers/kafka_connect/__init__.py
+-rw-r--r--   0        0        0     7412 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/component_handlers/kafka_connect/connect_wrapper.py
+-rw-r--r--   0        0        0      229 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/component_handlers/kafka_connect/exception.py
+-rw-r--r--   0        0        0     5460 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/component_handlers/kafka_connect/kafka_connect_handler.py
+-rw-r--r--   0        0        0     3543 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/component_handlers/kafka_connect/model.py
+-rw-r--r--   0        0        0      797 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/component_handlers/kafka_connect/timeout.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/component_handlers/kubernetes/__init__.py
+-rw-r--r--   0        0        0      841 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/component_handlers/kubernetes/model.py
+-rw-r--r--   0        0        0     1116 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/component_handlers/kubernetes/utils.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/component_handlers/schema_handler/__init__.py
+-rw-r--r--   0        0        0     6774 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/component_handlers/schema_handler/schema_handler.py
+-rw-r--r--   0        0        0      491 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/component_handlers/schema_handler/schema_provider.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/component_handlers/topic/__init__.py
+-rw-r--r--   0        0        0      225 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/component_handlers/topic/exception.py
+-rw-r--r--   0        0        0     9534 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/component_handlers/topic/handler.py
+-rw-r--r--   0        0        0     2420 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/component_handlers/topic/model.py
+-rw-r--r--   0        0        0     7345 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/component_handlers/topic/proxy_wrapper.py
+-rw-r--r--   0        0        0     2385 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/component_handlers/topic/utils.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/component_handlers/utils/__init__.py
+-rw-r--r--   0        0        0      625 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/component_handlers/utils/exception.py
+-rw-r--r--   0        0        0      906 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/components/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/components/base_components/__init__.py
+-rw-r--r--   0        0        0    10674 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/components/base_components/base_defaults_component.py
+-rw-r--r--   0        0        0     1061 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/components/base_components/cleaner.py
+-rw-r--r--   0        0        0     7237 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/components/base_components/helm_app.py
+-rw-r--r--   0        0        0     4748 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/components/base_components/kafka_app.py
+-rw-r--r--   0        0        0     9178 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/components/base_components/kafka_connector.py
+-rw-r--r--   0        0        0     1828 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/components/base_components/kubernetes_app.py
+-rw-r--r--   0        0        0      149 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/components/base_components/models/__init__.py
+-rw-r--r--   0        0        0     1882 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/components/base_components/models/from_section.py
+-rw-r--r--   0        0        0      217 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/components/base_components/models/resource.py
+-rw-r--r--   0        0        0      994 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/components/base_components/models/to_section.py
+-rw-r--r--   0        0        0     3801 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/components/base_components/models/topic.py
+-rw-r--r--   0        0        0     8324 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/components/base_components/pipeline_component.py
+-rw-r--r--   0        0        0     1031 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/components/streams_bootstrap/__init__.py
+-rw-r--r--   0        0        0      217 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/components/streams_bootstrap/app_type.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/components/streams_bootstrap/producer/__init__.py
+-rw-r--r--   0        0        0      595 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/components/streams_bootstrap/producer/model.py
+-rw-r--r--   0        0        0     2873 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/components/streams_bootstrap/producer/producer_app.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/components/streams_bootstrap/streams/__init__.py
+-rw-r--r--   0        0        0     8649 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/components/streams_bootstrap/streams/model.py
+-rw-r--r--   0        0        0     3309 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/components/streams_bootstrap/streams/streams_app.py
+-rw-r--r--   0        0        0     5147 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/config.py
+-rw-r--r--   0        0        0    15340 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/pipeline.py
+-rw-r--r--   0        0        0      278 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/utils/__init__.py
+-rw-r--r--   0        0        0     3060 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/utils/cli_commands.py
+-rw-r--r--   0        0        0      375 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/utils/colorify.py
+-rw-r--r--   0        0        0     3178 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/utils/dict_differ.py
+-rw-r--r--   0        0        0     4996 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/utils/dict_ops.py
+-rw-r--r--   0        0        0     2431 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/utils/docstring.py
+-rw-r--r--   0        0        0     1176 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/utils/environment.py
+-rw-r--r--   0        0        0     5924 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/utils/gen_schema.py
+-rw-r--r--   0        0        0      298 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/utils/json.py
+-rw-r--r--   0        0        0     6533 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/utils/pydantic.py
+-rw-r--r--   0        0        0      238 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/utils/types.py
+-rw-r--r--   0        0        0     4332 2024-04-25 12:04:45.140307 kpops-4.2.0/kpops/utils/yaml.py
+-rw-r--r--   0        0        0     7412 2024-04-25 12:04:45.140307 kpops-4.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4276 1970-01-01 00:00:00.000000 kpops-4.2.0/PKG-INFO
```

### Comparing `kpops-4.1.2/LICENSE` & `kpops-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/README.md` & `kpops-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/cli/custom_formatter.py` & `kpops-4.2.0/kpops/cli/custom_formatter.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/cli/main.py` & `kpops-4.2.0/kpops/cli/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -504,13 +504,12 @@
         False,
         "--version",
         "-V",
         help="Print KPOps version",
         callback=version_callback,
         is_eager=True,
     ),
-):
-    ...
+): ...
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `kpops-4.1.2/kpops/cli/registry.py` & `kpops-4.2.0/kpops/cli/registry.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/component_handlers/__init__.py` & `kpops-4.2.0/kpops/component_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/component_handlers/helm_wrapper/dry_run_handler.py` & `kpops-4.2.0/kpops/component_handlers/helm_wrapper/dry_run_handler.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/component_handlers/helm_wrapper/helm.py` & `kpops-4.2.0/kpops/component_handlers/helm_wrapper/helm.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/component_handlers/helm_wrapper/helm_diff.py` & `kpops-4.2.0/kpops/component_handlers/helm_wrapper/helm_diff.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/component_handlers/helm_wrapper/model.py` & `kpops-4.2.0/kpops/component_handlers/helm_wrapper/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,16 +136,15 @@
         if self.wait:
             command.append("--wait")
         if self.wait_for_jobs:
             command.append("--wait-for-jobs")
         return command
 
 
-class HelmUpgradeInstallFlags(HelmFlags):
-    ...
+class HelmUpgradeInstallFlags(HelmFlags): ...
 
 
 class HelmTemplateFlags(HelmFlags):
     api_version: str | None = None
 
     @override
     def to_command(self) -> list[str]:
```

### Comparing `kpops-4.1.2/kpops/component_handlers/helm_wrapper/utils.py` & `kpops-4.2.0/kpops/component_handlers/helm_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/component_handlers/kafka_connect/connect_wrapper.py` & `kpops-4.2.0/kpops/component_handlers/kafka_connect/connect_wrapper.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/component_handlers/kafka_connect/kafka_connect_handler.py` & `kpops-4.2.0/kpops/component_handlers/kafka_connect/kafka_connect_handler.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/component_handlers/kafka_connect/model.py` & `kpops-4.2.0/kpops/component_handlers/kafka_connect/model.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/component_handlers/kafka_connect/timeout.py` & `kpops-4.2.0/kpops/component_handlers/kafka_connect/timeout.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/component_handlers/kubernetes/model.py` & `kpops-4.2.0/kpops/component_handlers/kubernetes/model.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/component_handlers/kubernetes/utils.py` & `kpops-4.2.0/kpops/component_handlers/kubernetes/utils.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/component_handlers/schema_handler/schema_handler.py` & `kpops-4.2.0/kpops/component_handlers/schema_handler/schema_handler.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/component_handlers/topic/handler.py` & `kpops-4.2.0/kpops/component_handlers/topic/handler.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/component_handlers/topic/model.py` & `kpops-4.2.0/kpops/component_handlers/topic/model.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/component_handlers/topic/proxy_wrapper.py` & `kpops-4.2.0/kpops/component_handlers/topic/proxy_wrapper.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/component_handlers/topic/utils.py` & `kpops-4.2.0/kpops/component_handlers/topic/utils.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/component_handlers/utils/exception.py` & `kpops-4.2.0/kpops/component_handlers/utils/exception.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/components/__init__.py` & `kpops-4.2.0/kpops/components/__init__.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/components/base_components/base_defaults_component.py` & `kpops-4.2.0/kpops/components/base_components/base_defaults_component.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/components/base_components/cleaner.py` & `kpops-4.2.0/kpops/components/base_components/cleaner.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/components/base_components/helm_app.py` & `kpops-4.2.0/kpops/components/base_components/helm_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,17 +36,17 @@
 
 class HelmAppValues(KubernetesAppValues):
     """Helm app values.
 
     :param name_override: Helm chart name override, assigned automatically
     """
 
-    name_override: Annotated[
-        str, pydantic.StringConstraints(max_length=K8S_LABEL_MAX_LEN)
-    ] | None = Field(
+    name_override: (
+        Annotated[str, pydantic.StringConstraints(max_length=K8S_LABEL_MAX_LEN)] | None
+    ) = Field(
         default=None,
         title="Nameoverride",
         description=describe_attr("name_override", __doc__),
     )
 
     # TODO(Ivan Yordanov): Replace with a function decorated with `@model_serializer`
     # BEWARE! All default values are enforced, hard to replicate without
```

### Comparing `kpops-4.1.2/kpops/components/base_components/kafka_app.py` & `kpops-4.2.0/kpops/components/base_components/kafka_app.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/components/base_components/kafka_connector.py` & `kpops-4.2.0/kpops/components/base_components/kafka_connector.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/components/base_components/kubernetes_app.py` & `kpops-4.2.0/kpops/components/base_components/kubernetes_app.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/components/base_components/models/from_section.py` & `kpops-4.2.0/kpops/components/base_components/models/from_section.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/components/base_components/models/to_section.py` & `kpops-4.2.0/kpops/components/base_components/models/to_section.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/components/base_components/models/topic.py` & `kpops-4.2.0/kpops/components/base_components/models/topic.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/components/base_components/pipeline_component.py` & `kpops-4.2.0/kpops/components/base_components/pipeline_component.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/components/streams_bootstrap/__init__.py` & `kpops-4.2.0/kpops/components/streams_bootstrap/__init__.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/components/streams_bootstrap/producer/model.py` & `kpops-4.2.0/kpops/components/streams_bootstrap/producer/model.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/components/streams_bootstrap/producer/producer_app.py` & `kpops-4.2.0/kpops/components/streams_bootstrap/producer/producer_app.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/components/streams_bootstrap/streams/model.py` & `kpops-4.2.0/kpops/components/streams_bootstrap/streams/model.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/components/streams_bootstrap/streams/streams_app.py` & `kpops-4.2.0/kpops/components/streams_bootstrap/streams/streams_app.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/config.py` & `kpops-4.2.0/kpops/config.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/pipeline.py` & `kpops-4.2.0/kpops/pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,23 +101,28 @@
 
     def to_yaml(self) -> str:
         return yaml.dump(
             self.model_dump(mode="json", by_alias=True, exclude_none=True)["components"]
         )
 
     def build_execution_graph(
-        self, runner: Callable[[PipelineComponent], Coroutine], /, reverse: bool = False
-    ) -> Awaitable:
-        async def run_parallel_tasks(coroutines: list[Coroutine]) -> None:
+        self,
+        runner: Callable[[PipelineComponent], Coroutine[Any, Any, None]],
+        /,
+        reverse: bool = False,
+    ) -> Awaitable[None]:
+        async def run_parallel_tasks(
+            coroutines: list[Coroutine[Any, Any, None]],
+        ) -> None:
             tasks = []
             for coro in coroutines:
                 tasks.append(asyncio.create_task(coro))
             await asyncio.gather(*tasks)
 
-        async def run_graph_tasks(pending_tasks: list[Awaitable]) -> None:
+        async def run_graph_tasks(pending_tasks: list[Awaitable[None]]) -> None:
             for pending_task in pending_tasks:
                 await pending_task
 
         graph: nx.DiGraph = self._graph.copy()  # pyright: ignore[reportAssignmentType, reportGeneralTypeIssues] imprecise type hint in networkx
 
         # We add an extra node to the graph, connecting all the leaf nodes to it
         # in that way we make this node the root of the graph, avoiding backtracking
@@ -171,16 +176,18 @@
         self._graph.add_edge(source, topic_id)
 
     def __add_input(self, topic_id: str, target: str) -> None:
         self._graph.add_node(topic_id)
         self._graph.add_edge(topic_id, target)
 
     def __get_parallel_tasks_from(
-        self, layer: list[str], runner: Callable[[PipelineComponent], Coroutine]
-    ) -> list[Coroutine]:
+        self,
+        layer: list[str],
+        runner: Callable[[PipelineComponent], Coroutine[Any, Any, None]],
+    ) -> list[Coroutine[Any, Any, None]]:
         def gen_parallel_tasks():
             for node_in_layer in layer:
                 # check if component, skip topics
                 if (component := self._component_index.get(node_in_layer)) is not None:
                     yield runner(component)
 
         return list(gen_parallel_tasks())
```

### Comparing `kpops-4.1.2/kpops/utils/cli_commands.py` & `kpops-4.2.0/kpops/utils/cli_commands.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/utils/dict_differ.py` & `kpops-4.2.0/kpops/utils/dict_differ.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/utils/dict_ops.py` & `kpops-4.2.0/kpops/utils/dict_ops.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/utils/docstring.py` & `kpops-4.2.0/kpops/utils/docstring.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/utils/environment.py` & `kpops-4.2.0/kpops/utils/environment.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/utils/gen_schema.py` & `kpops-4.2.0/kpops/utils/gen_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,16 +30,15 @@
 
 class SchemaScope(str, Enum):
     PIPELINE = "pipeline"
     DEFAULTS = "defaults"
     CONFIG = "config"
 
 
-class MultiComponentGenerateJsonSchema(GenerateJsonSchema):
-    ...
+class MultiComponentGenerateJsonSchema(GenerateJsonSchema): ...
 
 
 log = logging.getLogger("")
 
 
 def print_schema(model: type[BaseModel]) -> None:
     schema = model_json_schema(model, by_alias=True)
```

### Comparing `kpops-4.1.2/kpops/utils/pydantic.py` & `kpops-4.2.0/kpops/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/kpops/utils/yaml.py` & `kpops-4.2.0/kpops/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `kpops-4.1.2/pyproject.toml` & `kpops-4.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kpops"
-version = "4.1.2"
+version = "4.2.0"
 description = "KPOps is a tool to deploy Kafka pipelines to Kubernetes"
 authors = ["bakdata <opensource@bakdata.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bakdata/kpops"
 documentation = "https://bakdata.github.io/kpops/latest"
 keywords = ["kafka", "kubernetes", "stream-processing", "pipelines"]
@@ -19,14 +19,15 @@
 ]
 
 [tool.poetry.scripts]
 kpops = "kpops.cli.main:app"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <3.13"
+anyio = "^4.3.0"
 pydantic = "^2.5.3"
 pydantic-settings = "^2.0.3"
 rich = "^12.4.4"
 PyYAML = "^6.0"
 typer = { extras = ["all"], version = "^0.6.1" }
 dtyper = "^2.1.0"
 pyhumps = "^3.7.3"
@@ -38,15 +39,15 @@
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.2"
 pytest-mock = "^3.10.0"
 pytest-timeout = "^2.1.0"
 pytest-snapshot = "^0.9.0"
 pre-commit = "^2.19.0"
-ruff = "^0.1.7"
+ruff = "^0.3.4"
 typer-cli = "^0.0.13"
 pyright = "^1.1.352"
 pytest-rerunfailures = "^11.1.2"
 pytest-asyncio = "^0.21.1"
 pytest-httpx = "^0.30.0"
 pytablewriter = { extras = ["from"], version = "^1.0.0" }
 polyfactory = "^2.13.0"
@@ -61,22 +62,33 @@
 mkdocs-glightbox = "^0.3.1"
 mkdocs-exclude-search = "^0.6.5"
 mike = "^1.1.2"
 
 [tool.poetry_bumpversion.file."kpops/__init__.py"]
 
 [tool.pyright]
+reportUnknownParameterType = "warning"
+reportUnknownArgumentType = "warning"
+reportUnknownLambdaType = "warning"
+reportUnknownVariableType = "warning"
+reportUnknownMemberType = "warning"
+
 reportIncompatibleVariableOverride = false
 reportIncompatibleMethodOverride = false
-
 # FIXME: causes issues on Python 3.10
 # reportIncompatibleVariableOverride = "warning"
 # reportIncompatibleMethodOverride = "warning"
 
 [tool.ruff]
+output-format = "grouped"
+show-fixes = true
+target-version = "py310"
+extend-exclude = ["tests/*snapshots/*"]
+
+[tool.ruff.lint]
 ignore = [
   # Rules in conflict with `ruff-format` -- START
   "W191", # Checks for indentation that uses tabs. Spaces are preferred.
   # "E111", # Checks for indentation with a non-multiple of 4 spaces, add when out of nursery
   # "E114", # Checks for indentation of comments with a non-multiple of 4 spaces, add when out of nursery
   # "E117", # Checks for over-indented code, add when out of nursery
   "E501", # Line too long
@@ -157,25 +169,21 @@
   "PTH", # flake8-use-pathlib
   "PGH", # pygrep-hooks
   "PL", # Pylint
   "TRY", # tryceratops
   # "FURB", # refurb, add when out of nursery
   # "LOG", # flake8-logging, add when out of nursery
 ]
-output-format = "grouped"
-show-fixes = true
 task-tags = ["TODO", "HACK", "FIXME", "XXX"]
-target-version = "py310"
-extend-exclude = ["tests/*snapshots/*"]
 
-[tool.ruff.extend-per-file-ignores]
+[tool.ruff.lint.extend-per-file-ignores]
 "tests/*/__init__.py" = ["F401"]
 
-[tool.ruff.flake8-bugbear]
+[tool.ruff.lint.flake8-bugbear]
 extend-immutable-calls = ["typer.Argument"]
 
-[tool.ruff.flake8-type-checking]
+[tool.ruff.lint.flake8-type-checking]
 runtime-evaluated-base-classes = ["pydantic.BaseModel"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `kpops-4.1.2/PKG-INFO` & `kpops-4.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kpops
-Version: 4.1.2
+Version: 4.2.0
 Summary: KPOps is a tool to deploy Kafka pipelines to Kubernetes
 Home-page: https://github.com/bakdata/kpops
 License: MIT
 Keywords: kafka,kubernetes,stream-processing,pipelines
 Author: bakdata
 Author-email: opensource@bakdata.com
 Requires-Python: >=3.10,<3.13
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: anyio (>=4.3.0,<5.0.0)
 Requires-Dist: cachetools (>=5.2.0,<6.0.0)
 Requires-Dist: dictdiffer (>=0.9.0,<0.10.0)
 Requires-Dist: dtyper (>=2.1.0,<3.0.0)
 Requires-Dist: httpx (>=0.24.1,<1)
 Requires-Dist: networkx (>=3.1,<4.0)
 Requires-Dist: pydantic (>=2.5.3,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.0.3,<3.0.0)
```

