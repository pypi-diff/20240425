# Comparing `tmp/dagster-1.7.2rc4.tar.gz` & `tmp/dagster-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-1.7.2rc4.tar", last modified: Fri Apr 19 18:02:21 2024, max compression
+gzip compressed data, was "dagster-1.7.3.tar", last modified: Thu Apr 25 20:08:56 2024, max compression
```

## Comparing `dagster-1.7.2rc4.tar` & `dagster-1.7.3.tar`

### file list

```diff
@@ -1,693 +1,693 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.701783 dagster-1.7.2rc4/
--rw-r--r--   0 root         (0) root         (0)      553 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/COPYING
--rw-r--r--   0 root         (0) root         (0)    11349 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      533 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     9870 2024-04-19 18:02:21.701783 dagster-1.7.2rc4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8153 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.369781 dagster-1.7.2rc4/dagster/
--rw-r--r--   0 root         (0) root         (0)    29906 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/__init__.py
--rw-r--r--   0 root         (0) root         (0)       31 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/__main__.py
--rw-r--r--   0 root         (0) root         (0)    20744 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_annotations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.377781 dagster-1.7.2rc4/dagster/_api/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)      731 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_api/get_server_id.py
--rw-r--r--   0 root         (0) root         (0)     2147 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_api/list_repositories.py
--rw-r--r--   0 root         (0) root         (0)      531 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_api/notebook_data.py
--rw-r--r--   0 root         (0) root         (0)     3224 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_api/snapshot_execution_plan.py
--rw-r--r--   0 root         (0) root         (0)     1964 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_api/snapshot_job.py
--rw-r--r--   0 root         (0) root         (0)     5483 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_api/snapshot_partition.py
--rw-r--r--   0 root         (0) root         (0)     1670 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_api/snapshot_repository.py
--rw-r--r--   0 root         (0) root         (0)     3021 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_api/snapshot_schedule.py
--rw-r--r--   0 root         (0) root         (0)     3370 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_api/snapshot_sensor.py
--rw-r--r--   0 root         (0) root         (0)      478 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_builtins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.381781 dagster-1.7.2rc4/dagster/_check/
--rw-r--r--   0 root         (0) root         (0)     1352 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_check/README.md
--rw-r--r--   0 root         (0) root         (0)    52040 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_check/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.393781 dagster-1.7.2rc4/dagster/_cli/
--rw-r--r--   0 root         (0) root         (0)     1182 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26898 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_cli/api.py
--rw-r--r--   0 root         (0) root         (0)     8030 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_cli/asset.py
--rw-r--r--   0 root         (0) root         (0)     8302 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_cli/code_server.py
--rw-r--r--   0 root         (0) root         (0)     2374 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_cli/config_scaffolder.py
--rw-r--r--   0 root         (0) root         (0)     3513 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_cli/debug.py
--rw-r--r--   0 root         (0) root         (0)     8134 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_cli/dev.py
--rw-r--r--   0 root         (0) root         (0)     6651 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_cli/instance.py
--rw-r--r--   0 root         (0) root         (0)    30542 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_cli/job.py
--rw-r--r--   0 root         (0) root         (0)     1695 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_cli/load_handle.py
--rw-r--r--   0 root         (0) root         (0)     9114 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_cli/project.py
--rw-r--r--   0 root         (0) root         (0)     5120 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_cli/run.py
--rw-r--r--   0 root         (0) root         (0)    19351 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_cli/schedule.py
--rw-r--r--   0 root         (0) root         (0)    15461 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_cli/sensor.py
--rw-r--r--   0 root         (0) root         (0)     4259 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_cli/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.393781 dagster-1.7.2rc4/dagster/_cli/workspace/
--rw-r--r--   0 root         (0) root         (0)      180 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_cli/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27910 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_cli/workspace/cli_target.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.409781 dagster-1.7.2rc4/dagster/_config/
--rw-r--r--   0 root         (0) root         (0)     3186 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3403 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_config/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    15830 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_config/config_type.py
--rw-r--r--   0 root         (0) root         (0)    18787 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_config/errors.py
--rw-r--r--   0 root         (0) root         (0)     1783 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_config/evaluate_value_result.py
--rw-r--r--   0 root         (0) root         (0)    14918 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_config/field.py
--rw-r--r--   0 root         (0) root         (0)    19728 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_config/field_utils.py
--rw-r--r--   0 root         (0) root         (0)     9536 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_config/post_process.py
--rw-r--r--   0 root         (0) root         (0)      855 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_config/primitive_mapping.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.409781 dagster-1.7.2rc4/dagster/_config/pythonic_config/
--rw-r--r--   0 root         (0) root         (0)     1394 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_config/pythonic_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1641 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_config/pythonic_config/attach_other_object_to_context.py
--rw-r--r--   0 root         (0) root         (0)    18116 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_config/pythonic_config/config.py
--rw-r--r--   0 root         (0) root         (0)    11510 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_config/pythonic_config/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)    11583 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_config/pythonic_config/io_manager.py
--rw-r--r--   0 root         (0) root         (0)    41265 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_config/pythonic_config/resource.py
--rw-r--r--   0 root         (0) root         (0)     1996 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_config/pythonic_config/type_check_utils.py
--rw-r--r--   0 root         (0) root         (0)     8375 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_config/pythonic_config/typing_utils.py
--rw-r--r--   0 root         (0) root         (0)    12532 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_config/snap.py
--rw-r--r--   0 root         (0) root         (0)     3087 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_config/source.py
--rw-r--r--   0 root         (0) root         (0)     3528 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_config/stack.py
--rw-r--r--   0 root         (0) root         (0)     7772 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_config/traversal_context.py
--rw-r--r--   0 root         (0) root         (0)     4167 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_config/type_printer.py
--rw-r--r--   0 root         (0) root         (0)    17137 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_config/validate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.413782 dagster-1.7.2rc4/dagster/_core/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.413782 dagster-1.7.2rc4/dagster/_core/asset_graph_view/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/asset_graph_view/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21047 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/asset_graph_view/asset_graph_view.py
--rw-r--r--   0 root         (0) root         (0)      994 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/assets.py
--rw-r--r--   0 root         (0) root         (0)    13427 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/code_pointer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.413782 dagster-1.7.2rc4/dagster/_core/container_context/
--rw-r--r--   0 root         (0) root         (0)      184 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/container_context/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1278 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/container_context/config.py
--rw-r--r--   0 root         (0) root         (0)     2310 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/debug.py
--rw-r--r--   0 root         (0) root         (0)     9665 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/decorator_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.457782 dagster-1.7.2rc4/dagster/_core/definitions/
--rw-r--r--   0 root         (0) root         (0)     7827 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4506 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/asset_check_evaluation.py
--rw-r--r--   0 root         (0) root         (0)     7052 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/asset_check_result.py
--rw-r--r--   0 root         (0) root         (0)     5416 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/asset_check_spec.py
--rw-r--r--   0 root         (0) root         (0)     6092 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/asset_checks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.465782 dagster-1.7.2rc4/dagster/_core/definitions/asset_condition/
--rw-r--r--   0 root         (0) root         (0)       62 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/asset_condition/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21064 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/asset_condition/asset_condition.py
--rw-r--r--   0 root         (0) root         (0)    16508 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/asset_condition/asset_condition_evaluation_context.py
--rw-r--r--   0 root         (0) root         (0)    26314 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/asset_daemon_context.py
--rw-r--r--   0 root         (0) root         (0)    10648 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/asset_daemon_cursor.py
--rw-r--r--   0 root         (0) root         (0)     4628 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/asset_dep.py
--rw-r--r--   0 root         (0) root         (0)    10133 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/asset_graph.py
--rw-r--r--   0 root         (0) root         (0)     7696 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/asset_graph_differ.py
--rw-r--r--   0 root         (0) root         (0)    16636 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/asset_graph_subset.py
--rw-r--r--   0 root         (0) root         (0)     3644 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/asset_in.py
--rw-r--r--   0 root         (0) root         (0)    29917 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/asset_job.py
--rw-r--r--   0 root         (0) root         (0)     6060 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/asset_key.py
--rw-r--r--   0 root         (0) root         (0)    30355 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/asset_layer.py
--rw-r--r--   0 root         (0) root         (0)     6945 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/asset_out.py
--rw-r--r--   0 root         (0) root         (0)    39535 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/asset_selection.py
--rw-r--r--   0 root         (0) root         (0)     7444 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)     6764 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/asset_spec.py
--rw-r--r--   0 root         (0) root         (0)    10466 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/asset_subset.py
--rw-r--r--   0 root         (0) root         (0)    79909 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/assets.py
--rw-r--r--   0 root         (0) root         (0)    13905 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/auto_materialize_policy.py
--rw-r--r--   0 root         (0) root         (0)    54478 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/auto_materialize_rule.py
--rw-r--r--   0 root         (0) root         (0)    21726 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/auto_materialize_rule_evaluation.py
--rw-r--r--   0 root         (0) root         (0)     2768 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/auto_materialize_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)     2939 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/backfill_policy.py
--rw-r--r--   0 root         (0) root         (0)    34666 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/base_asset_graph.py
--rw-r--r--   0 root         (0) root         (0)    16772 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/cacheable_assets.py
--rw-r--r--   0 root         (0) root         (0)    40623 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/composition.py
--rw-r--r--   0 root         (0) root         (0)     4278 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/config.py
--rw-r--r--   0 root         (0) root         (0)    14811 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/configurable.py
--rw-r--r--   0 root         (0) root         (0)    22990 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/data_time.py
--rw-r--r--   0 root         (0) root         (0)    30060 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/data_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.465782 dagster-1.7.2rc4/dagster/_core/definitions/decorators/
--rw-r--r--   0 root         (0) root         (0)      620 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16572 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/decorators/asset_check_decorator.py
--rw-r--r--   0 root         (0) root         (0)    69618 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/decorators/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     4907 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/decorators/config_mapping_decorator.py
--rw-r--r--   0 root         (0) root         (0)     9077 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/decorators/graph_decorator.py
--rw-r--r--   0 root         (0) root         (0)     9353 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/decorators/hook_decorator.py
--rw-r--r--   0 root         (0) root         (0)    10815 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/decorators/job_decorator.py
--rw-r--r--   0 root         (0) root         (0)    19011 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/decorators/op_decorator.py
--rw-r--r--   0 root         (0) root         (0)    15668 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/decorators/repository_decorator.py
--rw-r--r--   0 root         (0) root         (0)     8718 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/decorators/schedule_decorator.py
--rw-r--r--   0 root         (0) root         (0)    12463 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/decorators/sensor_decorator.py
--rw-r--r--   0 root         (0) root         (0)    12664 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/decorators/source_asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     5267 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/definition_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    23545 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/definitions_class.py
--rw-r--r--   0 root         (0) root         (0)    42243 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/dependency.py
--rw-r--r--   0 root         (0) root         (0)    26888 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/events.py
--rw-r--r--   0 root         (0) root         (0)    21182 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/executor_definition.py
--rw-r--r--   0 root         (0) root         (0)     9379 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/external_asset.py
--rw-r--r--   0 root         (0) root         (0)     9766 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/freshness_based_auto_materialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.473782 dagster-1.7.2rc4/dagster/_core/definitions/freshness_checks/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/freshness_checks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5838 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/freshness_checks/last_update.py
--rw-r--r--   0 root         (0) root         (0)     7677 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/freshness_checks/sensor.py
--rw-r--r--   0 root         (0) root         (0)     7938 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/freshness_checks/shared_builder.py
--rw-r--r--   0 root         (0) root         (0)     4669 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/freshness_checks/time_partition.py
--rw-r--r--   0 root         (0) root         (0)    10573 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/freshness_checks/utils.py
--rw-r--r--   0 root         (0) root         (0)     8801 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/freshness_policy.py
--rw-r--r--   0 root         (0) root         (0)    16401 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/freshness_policy_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    47569 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/graph_definition.py
--rw-r--r--   0 root         (0) root         (0)     6546 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/hook_definition.py
--rw-r--r--   0 root         (0) root         (0)     1524 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/hook_invocation.py
--rw-r--r--   0 root         (0) root         (0)     3537 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/inference.py
--rw-r--r--   0 root         (0) root         (0)    21027 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/input.py
--rw-r--r--   0 root         (0) root         (0)     6410 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/instigation_logger.py
--rw-r--r--   0 root         (0) root         (0)     2991 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/job_base.py
--rw-r--r--   0 root         (0) root         (0)    53689 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/job_definition.py
--rw-r--r--   0 root         (0) root         (0)     5693 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/load_asset_checks_from_modules.py
--rw-r--r--   0 root         (0) root         (0)    22306 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/load_assets_from_modules.py
--rw-r--r--   0 root         (0) root         (0)     7171 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/logger_definition.py
--rw-r--r--   0 root         (0) root         (0)      636 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/logger_invocation.py
--rw-r--r--   0 root         (0) root         (0)     8959 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/materialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.473782 dagster-1.7.2rc4/dagster/_core/definitions/metadata/
--rw-r--r--   0 root         (0) root         (0)    42209 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/metadata/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12410 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/metadata/table.py
--rw-r--r--   0 root         (0) root         (0)    57203 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/multi_asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    22029 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/multi_dimensional_partitions.py
--rw-r--r--   0 root         (0) root         (0)      197 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/no_step_launcher.py
--rw-r--r--   0 root         (0) root         (0)    11892 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/node_container.py
--rw-r--r--   0 root         (0) root         (0)     8016 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/node_definition.py
--rw-r--r--   0 root         (0) root         (0)     2892 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/observe.py
--rw-r--r--   0 root         (0) root         (0)    23078 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/op_definition.py
--rw-r--r--   0 root         (0) root         (0)    23141 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/op_invocation.py
--rw-r--r--   0 root         (0) root         (0)     7551 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/op_selection.py
--rw-r--r--   0 root         (0) root         (0)    19237 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/output.py
--rw-r--r--   0 root         (0) root         (0)    50520 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/partition.py
--rw-r--r--   0 root         (0) root         (0)      630 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/partition_key_range.py
--rw-r--r--   0 root         (0) root         (0)    47665 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)    11087 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/partitioned_schedule.py
--rw-r--r--   0 root         (0) root         (0)     3779 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/policy.py
--rw-r--r--   0 root         (0) root         (0)    27733 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/reconstruct.py
--rw-r--r--   0 root         (0) root         (0)    21602 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/remote_asset_graph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.473782 dagster-1.7.2rc4/dagster/_core/definitions/repository_definition/
--rw-r--r--   0 root         (0) root         (0)      654 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/repository_definition/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6024 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/repository_definition/caching_index.py
--rw-r--r--   0 root         (0) root         (0)    21698 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/repository_definition/repository_data.py
--rw-r--r--   0 root         (0) root         (0)    20892 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/repository_definition/repository_data_builder.py
--rw-r--r--   0 root         (0) root         (0)    20432 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/repository_definition/repository_definition.py
--rw-r--r--   0 root         (0) root         (0)     1479 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/repository_definition/valid_definitions.py
--rw-r--r--   0 root         (0) root         (0)     8858 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/resolved_asset_deps.py
--rw-r--r--   0 root         (0) root         (0)     1465 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/resource_annotation.py
--rw-r--r--   0 root         (0) root         (0)    17900 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/resource_definition.py
--rw-r--r--   0 root         (0) root         (0)     5382 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/resource_invocation.py
--rw-r--r--   0 root         (0) root         (0)    10320 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/resource_requirement.py
--rw-r--r--   0 root         (0) root         (0)     3383 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/result.py
--rw-r--r--   0 root         (0) root         (0)    23076 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/run_config.py
--rw-r--r--   0 root         (0) root         (0)     1445 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/run_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    19555 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/run_request.py
--rw-r--r--   0 root         (0) root         (0)    44126 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/run_status_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    39363 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/schedule_definition.py
--rw-r--r--   0 root         (0) root         (0)     6209 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/schema_change_checks.py
--rw-r--r--   0 root         (0) root         (0)     5134 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/scoped_resources_builder.py
--rw-r--r--   0 root         (0) root         (0)    14134 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/selector.py
--rw-r--r--   0 root         (0) root         (0)    53797 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    19244 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/source_asset.py
--rw-r--r--   0 root         (0) root         (0)     2481 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/step_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1530 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/target.py
--rw-r--r--   0 root         (0) root         (0)    21859 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/time_window_partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)   102142 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/time_window_partitions.py
--rw-r--r--   0 root         (0) root         (0)    15160 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/unresolved_asset_job_definition.py
--rw-r--r--   0 root         (0) root         (0)    11017 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/utils.py
--rw-r--r--   0 root         (0) root         (0)     3982 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/definitions/version_strategy.py
--rw-r--r--   0 root         (0) root         (0)    27136 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/errors.py
--rw-r--r--   0 root         (0) root         (0)    17452 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/event_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.481782 dagster-1.7.2rc4/dagster/_core/events/
--rw-r--r--   0 root         (0) root         (0)    71913 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/events/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7635 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/events/log.py
--rw-r--r--   0 root         (0) root         (0)     1614 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/events/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.489782 dagster-1.7.2rc4/dagster/_core/execution/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38363 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/api.py
--rw-r--r--   0 root         (0) root         (0)    64654 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/asset_backfill.py
--rw-r--r--   0 root         (0) root         (0)    17100 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/backfill.py
--rw-r--r--   0 root         (0) root         (0)     6296 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/build_resources.py
--rw-r--r--   0 root         (0) root         (0)      224 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/bulk_actions.py
--rw-r--r--   0 root         (0) root         (0)     5587 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/compute_logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.497782 dagster-1.7.2rc4/dagster/_core/execution/context/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/context/__init__.py
--rw-r--r--   0 root         (0) root         (0)    79687 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/context/compute.py
--rw-r--r--   0 root         (0) root         (0)    17598 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/context/hook.py
--rw-r--r--   0 root         (0) root         (0)     9613 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/context/init.py
--rw-r--r--   0 root         (0) root         (0)    29167 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/context/input.py
--rw-r--r--   0 root         (0) root         (0)    40124 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/context/invocation.py
--rw-r--r--   0 root         (0) root         (0)     3164 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/context/logger.py
--rw-r--r--   0 root         (0) root         (0)    37256 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/context/output.py
--rw-r--r--   0 root         (0) root         (0)    56002 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/context/system.py
--rw-r--r--   0 root         (0) root         (0)    18837 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/context_creation_job.py
--rw-r--r--   0 root         (0) root         (0)     5135 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/execute_in_process.py
--rw-r--r--   0 root         (0) root         (0)     5897 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/execute_in_process_result.py
--rw-r--r--   0 root         (0) root         (0)     9633 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/execution_result.py
--rw-r--r--   0 root         (0) root         (0)     8602 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/host_mode.py
--rw-r--r--   0 root         (0) root         (0)    14247 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/job_backfill.py
--rw-r--r--   0 root         (0) root         (0)     6723 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/job_execution_result.py
--rw-r--r--   0 root         (0) root         (0)      998 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/memoization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.501782 dagster-1.7.2rc4/dagster/_core/execution/plan/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/plan/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26460 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/plan/active.py
--rw-r--r--   0 root         (0) root         (0)     9850 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/plan/compute.py
--rw-r--r--   0 root         (0) root         (0)    17019 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/plan/compute_generator.py
--rw-r--r--   0 root         (0) root         (0)    16974 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/plan/execute_plan.py
--rw-r--r--   0 root         (0) root         (0)    40549 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/plan/execute_step.py
--rw-r--r--   0 root         (0) root         (0)    11032 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/plan/external_step.py
--rw-r--r--   0 root         (0) root         (0)     3664 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/plan/handle.py
--rw-r--r--   0 root         (0) root         (0)    39260 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/plan/inputs.py
--rw-r--r--   0 root         (0) root         (0)     6251 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/plan/instance_concurrency_context.py
--rw-r--r--   0 root         (0) root         (0)     1197 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/plan/local_external_step_main.py
--rw-r--r--   0 root         (0) root         (0)     5706 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/plan/objects.py
--rw-r--r--   0 root         (0) root         (0)     7326 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/plan/outputs.py
--rw-r--r--   0 root         (0) root         (0)    61075 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/plan/plan.py
--rw-r--r--   0 root         (0) root         (0)      114 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/plan/resume_retry.py
--rw-r--r--   0 root         (0) root         (0)    17174 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/plan/state.py
--rw-r--r--   0 root         (0) root         (0)    15985 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/plan/step.py
--rw-r--r--   0 root         (0) root         (0)     3796 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/plan/utils.py
--rw-r--r--   0 root         (0) root         (0)     1762 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/poll_compute_logs.py
--rw-r--r--   0 root         (0) root         (0)     8230 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/resolve_versions.py
--rw-r--r--   0 root         (0) root         (0)    19141 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/resources_init.py
--rw-r--r--   0 root         (0) root         (0)     2100 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/retries.py
--rw-r--r--   0 root         (0) root         (0)     1564 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/run_cancellation_thread.py
--rw-r--r--   0 root         (0) root         (0)     9950 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/stats.py
--rw-r--r--   0 root         (0) root         (0)    14043 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/submit_asset_runs.py
--rw-r--r--   0 root         (0) root         (0)     1125 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/tags.py
--rw-r--r--   0 root         (0) root         (0)     1172 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/validate_run_config.py
--rw-r--r--   0 root         (0) root         (0)     1282 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/watch_orphans.py
--rw-r--r--   0 root         (0) root         (0)     4311 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/execution/with_resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.509782 dagster-1.7.2rc4/dagster/_core/executor/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/executor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1265 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/executor/base.py
--rw-r--r--   0 root         (0) root         (0)     5989 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/executor/child_process_executor.py
--rw-r--r--   0 root         (0) root         (0)     3366 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/executor/in_process.py
--rw-r--r--   0 root         (0) root         (0)     1509 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/executor/init.py
--rw-r--r--   0 root         (0) root         (0)    15497 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/executor/multiprocess.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.509782 dagster-1.7.2rc4/dagster/_core/executor/step_delegating/
--rw-r--r--   0 root         (0) root         (0)      247 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/executor/step_delegating/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16894 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/executor/step_delegating/step_delegating_executor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.509782 dagster-1.7.2rc4/dagster/_core/executor/step_delegating/step_handler/
--rw-r--r--   0 root         (0) root         (0)      152 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/executor/step_delegating/step_handler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3078 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/executor/step_delegating/step_handler/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.509782 dagster-1.7.2rc4/dagster/_core/instance/
--rw-r--r--   0 root         (0) root         (0)   132705 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/instance/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16905 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/instance/config.py
--rw-r--r--   0 root         (0) root         (0)    24178 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/instance/ref.py
--rw-r--r--   0 root         (0) root         (0)     3899 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/instance_for_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.517782 dagster-1.7.2rc4/dagster/_core/launcher/
--rw-r--r--   0 root         (0) root         (0)      297 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3819 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/launcher/base.py
--rw-r--r--   0 root         (0) root         (0)     6645 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/launcher/default_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1566 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/launcher/sync_in_memory_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)      473 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/libraries.py
--rw-r--r--   0 root         (0) root         (0)    18041 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1029 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/nux.py
--rw-r--r--   0 root         (0) root         (0)     5736 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/op_concurrency_limits_counter.py
--rw-r--r--   0 root         (0) root         (0)     3691 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/origin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.517782 dagster-1.7.2rc4/dagster/_core/pipes/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/pipes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8974 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/pipes/client.py
--rw-r--r--   0 root         (0) root         (0)    18318 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/pipes/context.py
--rw-r--r--   0 root         (0) root         (0)     5648 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/pipes/subprocess.py
--rw-r--r--   0 root         (0) root         (0)    25661 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/pipes/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.525782 dagster-1.7.2rc4/dagster/_core/remote_representation/
--rw-r--r--   0 root         (0) root         (0)     2793 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/remote_representation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    36695 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/remote_representation/code_location.py
--rw-r--r--   0 root         (0) root         (0)    37482 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/remote_representation/external.py
--rw-r--r--   0 root         (0) root         (0)    83392 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/remote_representation/external_data.py
--rw-r--r--   0 root         (0) root         (0)     1450 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/remote_representation/feature_flags.py
--rw-r--r--   0 root         (0) root         (0)    12429 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/remote_representation/grpc_server_registry.py
--rw-r--r--   0 root         (0) root         (0)     1487 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/remote_representation/grpc_server_state_subscriber.py
--rw-r--r--   0 root         (0) root         (0)     4356 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/remote_representation/handle.py
--rw-r--r--   0 root         (0) root         (0)     1581 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/remote_representation/historical.py
--rw-r--r--   0 root         (0) root         (0)     4850 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/remote_representation/job_index.py
--rw-r--r--   0 root         (0) root         (0)    19669 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/remote_representation/origin.py
--rw-r--r--   0 root         (0) root         (0)     3602 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/remote_representation/represented.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.525782 dagster-1.7.2rc4/dagster/_core/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      267 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2005 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/run_coordinator/base.py
--rw-r--r--   0 root         (0) root         (0)     1922 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/run_coordinator/default_run_coordinator.py
--rw-r--r--   0 root         (0) root         (0)    13364 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/run_coordinator/queued_run_coordinator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.525782 dagster-1.7.2rc4/dagster/_core/scheduler/
--rw-r--r--   0 root         (0) root         (0)      534 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1241 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/scheduler/execution.py
--rw-r--r--   0 root         (0) root         (0)    28809 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/scheduler/instigation.py
--rw-r--r--   0 root         (0) root         (0)    10917 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/scheduler/scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.525782 dagster-1.7.2rc4/dagster/_core/secrets/
--rw-r--r--   0 root         (0) root         (0)       51 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1801 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/secrets/env_file.py
--rw-r--r--   0 root         (0) root         (0)      388 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/secrets/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.525782 dagster-1.7.2rc4/dagster/_core/selector/
--rw-r--r--   0 root         (0) root         (0)      295 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/selector/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18109 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/selector/subset_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.525782 dagster-1.7.2rc4/dagster/_core/snap/
--rw-r--r--   0 root         (0) root         (0)     2842 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/snap/__init__.py
--rw-r--r--   0 root         (0) root         (0)      494 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/snap/config_types.py
--rw-r--r--   0 root         (0) root         (0)     3999 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/snap/dagster_types.py
--rw-r--r--   0 root         (0) root         (0)     9302 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/snap/dep_snapshot.py
--rw-r--r--   0 root         (0) root         (0)    12155 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/snap/execution_plan_snapshot.py
--rw-r--r--   0 root         (0) root         (0)    16934 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/snap/job_snapshot.py
--rw-r--r--   0 root         (0) root         (0)     4561 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/snap/mode.py
--rw-r--r--   0 root         (0) root         (0)    14185 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/snap/node.py
--rw-r--r--   0 root         (0) root         (0)     3183 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/snap/snap_to_yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.545782 dagster-1.7.2rc4/dagster/_core/storage/
--rw-r--r--   0 root         (0) root         (0)     3058 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/DEVELOPING.md
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.545782 dagster-1.7.2rc4/dagster/_core/storage/alembic/
--rw-r--r--   0 root         (0) root         (0)     6686 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/README.md
--rw-r--r--   0 root         (0) root         (0)      687 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      494 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.589783 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     3150 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/001_initial_1.py
--rw-r--r--   0 root         (0) root         (0)      312 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/001_initial_schedule.py
--rw-r--r--   0 root         (0) root         (0)     1486 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
--rw-r--r--   0 root         (0) root         (0)      599 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      973 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
--rw-r--r--   0 root         (0) root         (0)      973 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     2729 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
--rw-r--r--   0 root         (0) root         (0)     1406 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1406 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1131 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
--rw-r--r--   0 root         (0) root         (0)      953 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      953 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      956 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      956 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1171 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1171 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1730 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1730 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1147 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1125 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
--rw-r--r--   0 root         (0) root         (0)     1143 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
--rw-r--r--   0 root         (0) root         (0)      417 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      417 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      435 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      435 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      432 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      432 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     3927 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
--rw-r--r--   0 root         (0) root         (0)     3927 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      409 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      409 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      936 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      936 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      325 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/017_initial_mysql.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1570 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1570 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1034 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1032 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1034 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      433 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
--rw-r--r--   0 root         (0) root         (0)      433 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)      433 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      531 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1275 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1275 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      404 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      404 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      404 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      635 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
--rw-r--r--   0 root         (0) root         (0)      434 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      434 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      434 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      416 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      416 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      416 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1893 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
--rw-r--r--   0 root         (0) root         (0)      958 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
--rw-r--r--   0 root         (0) root         (0)      499 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
--rw-r--r--   0 root         (0) root         (0)     1951 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
--rw-r--r--   0 root         (0) root         (0)      428 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
--rw-r--r--   0 root         (0) root         (0)      427 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
--rw-r--r--   0 root         (0) root         (0)     1537 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
--rw-r--r--   0 root         (0) root         (0)     2481 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
--rw-r--r--   0 root         (0) root         (0)     1177 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py
--rw-r--r--   0 root         (0) root         (0)     2062 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py
--rw-r--r--   0 root         (0) root         (0)     2359 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py
--rw-r--r--   0 root         (0) root         (0)     2898 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/041_add_asset_check_executions_table.py
--rw-r--r--   0 root         (0) root         (0)     1322 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/042_46b412388816_add_concurrency_limits_table.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3887 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/asset_check_execution_record.py
--rw-r--r--   0 root         (0) root         (0)     7301 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/asset_value_loader.py
--rw-r--r--   0 root         (0) root         (0)     1227 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/base_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.589783 dagster-1.7.2rc4/dagster/_core/storage/branching/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/branching/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5579 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/branching/branching_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8725 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/captured_log_manager.py
--rw-r--r--   0 root         (0) root         (0)    16223 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/cloud_storage_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     9557 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1863 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/config.py
--rw-r--r--   0 root         (0) root         (0)      417 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/daemon_cursor.py
--rw-r--r--   0 root         (0) root         (0)    25652 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/dagster_run.py
--rw-r--r--   0 root         (0) root         (0)    11187 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/db_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.589783 dagster-1.7.2rc4/dagster/_core/storage/event_log/
--rw-r--r--   0 root         (0) root         (0)      742 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/event_log/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18869 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/event_log/base.py
--rw-r--r--   0 root         (0) root         (0)     3801 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/event_log/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     7289 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/event_log/migration.py
--rw-r--r--   0 root         (0) root         (0)     8037 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/event_log/polling_event_watcher.py
--rw-r--r--   0 root         (0) root         (0)     9250 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/event_log/schema.py
--rw-r--r--   0 root         (0) root         (0)   121159 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/event_log/sql_event_log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.593783 dagster-1.7.2rc4/dagster/_core/storage/event_log/sqlite/
--rw-r--r--   0 root         (0) root         (0)      200 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/event_log/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.597783 dagster-1.7.2rc4/dagster/_core/storage/event_log/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)      986 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     7508 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    22497 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    10983 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/file_manager.py
--rw-r--r--   0 root         (0) root         (0)    13492 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/fs_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8819 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/input_manager.py
--rw-r--r--   0 root         (0) root         (0)    10882 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/io_manager.py
--rw-r--r--   0 root         (0) root         (0)    32629 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/legacy_storage.py
--rw-r--r--   0 root         (0) root         (0)    17558 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/local_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1167 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/mem_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     4355 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/memoizable_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.597783 dagster-1.7.2rc4/dagster/_core/storage/migration/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/migration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5964 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/migration/bigint_migration.py
--rw-r--r--   0 root         (0) root         (0)    15491 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/migration/utils.py
--rw-r--r--   0 root         (0) root         (0)     3270 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/noop_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     2361 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/output_manager.py
--rw-r--r--   0 root         (0) root         (0)    17398 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/partition_status_cache.py
--rw-r--r--   0 root         (0) root         (0)     2121 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/root.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.597783 dagster-1.7.2rc4/dagster/_core/storage/runs/
--rw-r--r--   0 root         (0) root         (0)      386 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/runs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13903 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/runs/base.py
--rw-r--r--   0 root         (0) root         (0)     2452 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/runs/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     8716 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/runs/migration.py
--rw-r--r--   0 root         (0) root         (0)     6391 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/runs/schema.py
--rw-r--r--   0 root         (0) root         (0)    37611 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/runs/sql_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.597783 dagster-1.7.2rc4/dagster/_core/storage/runs/sqlite/
--rw-r--r--   0 root         (0) root         (0)       69 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/runs/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.597783 dagster-1.7.2rc4/dagster/_core/storage/runs/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)      986 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     6310 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.597783 dagster-1.7.2rc4/dagster/_core/storage/schedules/
--rw-r--r--   0 root         (0) root         (0)      272 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7236 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/schedules/base.py
--rw-r--r--   0 root         (0) root         (0)     4133 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/schedules/migration.py
--rw-r--r--   0 root         (0) root         (0)     4086 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/schedules/schema.py
--rw-r--r--   0 root         (0) root         (0)    25146 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/schedules/sql_schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.597783 dagster-1.7.2rc4/dagster/_core/storage/schedules/sqlite/
--rw-r--r--   0 root         (0) root         (0)       84 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/schedules/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.605783 dagster-1.7.2rc4/dagster/_core/storage/schedules/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)      986 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     3684 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
--rw-r--r--   0 root         (0) root         (0)     7691 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/sql.py
--rw-r--r--   0 root         (0) root         (0)     1391 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/sqlalchemy_compat.py
--rw-r--r--   0 root         (0) root         (0)      926 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/sqlite.py
--rw-r--r--   0 root         (0) root         (0)     4875 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/sqlite_storage.py
--rw-r--r--   0 root         (0) root         (0)     3546 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/tags.py
--rw-r--r--   0 root         (0) root         (0)     1186 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/temp_file_manager.py
--rw-r--r--   0 root         (0) root         (0)    19215 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/storage/upath_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.609783 dagster-1.7.2rc4/dagster/_core/system_config/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/system_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13962 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/system_config/composite_descent.py
--rw-r--r--   0 root         (0) root         (0)    15178 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/system_config/objects.py
--rw-r--r--   0 root         (0) root         (0)    29921 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     4824 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/telemetry_upload.py
--rw-r--r--   0 root         (0) root         (0)    22361 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.613783 dagster-1.7.2rc4/dagster/_core/types/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3084 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/types/builtin_config_schemas.py
--rw-r--r--   0 root         (0) root         (0)     7042 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/types/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    36504 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/types/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)     3571 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/types/decorator.py
--rw-r--r--   0 root         (0) root         (0)     1846 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/types/loadable_target_origin.py
--rw-r--r--   0 root         (0) root         (0)     1027 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/types/primitive_mapping.py
--rw-r--r--   0 root         (0) root         (0)     4764 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/types/python_dict.py
--rw-r--r--   0 root         (0) root         (0)     2769 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/types/python_set.py
--rw-r--r--   0 root         (0) root         (0)     3620 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/types/python_tuple.py
--rw-r--r--   0 root         (0) root         (0)     1772 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/types/transform_typing.py
--rw-r--r--   0 root         (0) root         (0)     1441 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/utility_ops.py
--rw-r--r--   0 root         (0) root         (0)     6652 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.617783 dagster-1.7.2rc4/dagster/_core/workspace/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4457 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/workspace/autodiscovery.py
--rw-r--r--   0 root         (0) root         (0)     2679 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/workspace/batch_asset_record_loader.py
--rw-r--r--   0 root         (0) root         (0)     3422 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/workspace/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    29210 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/workspace/context.py
--rw-r--r--   0 root         (0) root         (0)    11852 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/workspace/load.py
--rw-r--r--   0 root         (0) root         (0)     4721 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/workspace/load_target.py
--rw-r--r--   0 root         (0) root         (0)     4311 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/workspace/permissions.py
--rw-r--r--   0 root         (0) root         (0)     3463 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_core/workspace/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.621783 dagster-1.7.2rc4/dagster/_daemon/
--rw-r--r--   0 root         (0) root         (0)     1971 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_daemon/__init__.py
--rw-r--r--   0 root         (0) root         (0)       30 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_daemon/__main__.py
--rw-r--r--   0 root         (0) root         (0)    41795 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_daemon/asset_daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.621783 dagster-1.7.2rc4/dagster/_daemon/auto_run_reexecution/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_daemon/auto_run_reexecution/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7402 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
--rw-r--r--   0 root         (0) root         (0)     9036 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
--rw-r--r--   0 root         (0) root         (0)     2665 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_daemon/backfill.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.621783 dagster-1.7.2rc4/dagster/_daemon/cli/
--rw-r--r--   0 root         (0) root         (0)     5118 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_daemon/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19590 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_daemon/controller.py
--rw-r--r--   0 root         (0) root         (0)    12112 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_daemon/daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.621783 dagster-1.7.2rc4/dagster/_daemon/monitoring/
--rw-r--r--   0 root         (0) root         (0)      320 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_daemon/monitoring/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1792 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_daemon/monitoring/concurrency.py
--rw-r--r--   0 root         (0) root         (0)     9904 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_daemon/monitoring/run_monitoring.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.621783 dagster-1.7.2rc4/dagster/_daemon/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      100 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_daemon/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18369 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
--rw-r--r--   0 root         (0) root         (0)    39110 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_daemon/sensor.py
--rw-r--r--   0 root         (0) root         (0)     2860 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_daemon/types.py
--rw-r--r--   0 root         (0) root         (0)      678 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_daemon/utils.py
--rw-r--r--   0 root         (0) root         (0)     4114 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_daemon/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.621783 dagster-1.7.2rc4/dagster/_experimental/
--rw-r--r--   0 root         (0) root         (0)      300 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_experimental/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.625783 dagster-1.7.2rc4/dagster/_generate/
--rw-r--r--   0 root         (0) root         (0)      253 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_generate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2997 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_generate/download.py
--rw-r--r--   0 root         (0) root         (0)     4805 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_generate/generate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.357781 dagster-1.7.2rc4/dagster/_generate/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.629783 dagster-1.7.2rc4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.629783 dagster-1.7.2rc4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)      175 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.629783 dagster-1.7.2rc4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)      137 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
--rw-r--r--   0 root         (0) root         (0)       43 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      297 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.629783 dagster-1.7.2rc4/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)     1753 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.633783 dagster-1.7.2rc4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.633783 dagster-1.7.2rc4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)       40 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
--rw-r--r--   0 root         (0) root         (0)      164 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.633783 dagster-1.7.2rc4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)       80 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       34 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      279 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.637783 dagster-1.7.2rc4/dagster/_grpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.641783 dagster-1.7.2rc4/dagster/_grpc/__generated__/
--rw-r--r--   0 root         (0) root         (0)      178 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_grpc/__generated__/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13462 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_grpc/__generated__/api_pb2.py
--rw-r--r--   0 root         (0) root         (0)    27262 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_grpc/__generated__/api_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)    43164 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_grpc/__generated__/api_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2060 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)       89 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_grpc/__main__.py
--rw-r--r--   0 root         (0) root         (0)    22739 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_grpc/client.py
--rw-r--r--   0 root         (0) root         (0)     3584 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_grpc/compile.py
--rw-r--r--   0 root         (0) root         (0)    23173 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_grpc/impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.641783 dagster-1.7.2rc4/dagster/_grpc/protos/
--rw-r--r--   0 root         (0) root         (0)     5993 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_grpc/protos/api.proto
--rw-r--r--   0 root         (0) root         (0)    13431 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_grpc/proxy_server.py
--rw-r--r--   0 root         (0) root         (0)    60914 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_grpc/server.py
--rw-r--r--   0 root         (0) root         (0)     5297 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_grpc/server_watcher.py
--rw-r--r--   0 root         (0) root         (0)    29291 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_grpc/types.py
--rw-r--r--   0 root         (0) root         (0)     3693 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_grpc/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.641783 dagster-1.7.2rc4/dagster/_legacy/
--rw-r--r--   0 root         (0) root         (0)      180 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_legacy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.641783 dagster-1.7.2rc4/dagster/_loggers/
--rw-r--r--   0 root         (0) root         (0)     3781 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_loggers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.641783 dagster-1.7.2rc4/dagster/_model/
--rw-r--r--   0 root         (0) root         (0)     1373 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3897 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_model/pydantic_compat_layer.py
--rw-r--r--   0 root         (0) root         (0)     3269 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_module_alias_map.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.645783 dagster-1.7.2rc4/dagster/_scheduler/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41378 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_scheduler/scheduler.py
--rw-r--r--   0 root         (0) root         (0)     1262 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_scheduler/stale.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.645783 dagster-1.7.2rc4/dagster/_serdes/
--rw-r--r--   0 root         (0) root         (0)      701 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_serdes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9674 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_serdes/config_class.py
--rw-r--r--   0 root         (0) root         (0)      142 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_serdes/errors.py
--rw-r--r--   0 root         (0) root         (0)     7292 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_serdes/ipc.py
--rw-r--r--   0 root         (0) root         (0)    42415 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_serdes/serdes.py
--rw-r--r--   0 root         (0) root         (0)      674 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_serdes/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.649783 dagster-1.7.2rc4/dagster/_seven/
--rw-r--r--   0 root         (0) root         (0)     5455 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_seven/__init__.py
--rw-r--r--   0 root         (0) root         (0)      553 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_seven/abc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.649783 dagster-1.7.2rc4/dagster/_seven/compat/
--rw-r--r--   0 root         (0) root         (0)      105 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_seven/compat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3967 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_seven/compat/pendulum.py
--rw-r--r--   0 root         (0) root         (0)      383 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_seven/json.py
--rw-r--r--   0 root         (0) root         (0)      354 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_seven/temp_dir.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.689783 dagster-1.7.2rc4/dagster/_utils/
--rw-r--r--   0 root         (0) root         (0)    24377 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9314 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/alert.py
--rw-r--r--   0 root         (0) root         (0)     2250 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/backoff.py
--rw-r--r--   0 root         (0) root         (0)     5404 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/cached_method.py
--rw-r--r--   0 root         (0) root         (0)    42615 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/caching_instance_queryer.py
--rw-r--r--   0 root         (0) root         (0)     5865 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/concurrency.py
--rw-r--r--   0 root         (0) root         (0)    12887 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/container.py
--rw-r--r--   0 root         (0) root         (0)     2412 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)      799 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/env.py
--rw-r--r--   0 root         (0) root         (0)     5477 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/error.py
--rw-r--r--   0 root         (0) root         (0)     1255 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/external.py
--rw-r--r--   0 root         (0) root         (0)      891 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/forked_pdb.py
--rw-r--r--   0 root         (0) root         (0)     1870 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/hosted_user_process.py
--rw-r--r--   0 root         (0) root         (0)     2796 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/indenting_printer.py
--rw-r--r--   0 root         (0) root         (0)      745 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/internal_init.py
--rw-r--r--   0 root         (0) root         (0)     3227 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/interrupts.py
--rw-r--r--   0 root         (0) root         (0)    11214 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/log.py
--rw-r--r--   0 root         (0) root         (0)     2313 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/merger.py
--rw-r--r--   0 root         (0) root         (0)     1507 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/net.py
--rw-r--r--   0 root         (0) root         (0)      208 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/partitions.py
--rw-r--r--   0 root         (0) root         (0)    33171 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/schedules.py
--rw-r--r--   0 root         (0) root         (0)      477 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/security.py
--rw-r--r--   0 root         (0) root         (0)     3289 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/tags.py
--rw-r--r--   0 root         (0) root         (0)     1820 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/temp_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.701783 dagster-1.7.2rc4/dagster/_utils/test/
--rw-r--r--   0 root         (0) root         (0)    13678 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7622 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/test/data_versions.py
--rw-r--r--   0 root         (0) root         (0)      119 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/test/hello_world_defs.py
--rw-r--r--   0 root         (0) root         (0)      214 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/test/hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     8622 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/test/mysql_instance.py
--rw-r--r--   0 root         (0) root         (0)      256 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/test/named_hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     8959 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/test/postgres_instance.py
--rw-r--r--   0 root         (0) root         (0)    36138 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/test/schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.701783 dagster-1.7.2rc4/dagster/_utils/test/toys/
--rw-r--r--   0 root         (0) root         (0)       83 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/test/toys/__init__.py
--rw-r--r--   0 root         (0) root         (0)       84 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/test/toys/single_repository.py
--rw-r--r--   0 root         (0) root         (0)     2004 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/timing.py
--rw-r--r--   0 root         (0) root         (0)     1032 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/typed_dict.py
--rw-r--r--   0 root         (0) root         (0)      170 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/types.py
--rw-r--r--   0 root         (0) root         (0)     3334 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/typing_api.py
--rw-r--r--   0 root         (0) root         (0)     4740 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/warnings.py
--rw-r--r--   0 root         (0) root         (0)     4902 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/_utils/yaml_utils.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/py.typed
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/dagster/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:21.373781 dagster-1.7.2rc4/dagster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9870 2024-04-19 18:02:20.000000 dagster-1.7.2rc4/dagster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    28024 2024-04-19 18:02:21.000000 dagster-1.7.2rc4/dagster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 18:02:20.000000 dagster-1.7.2rc4/dagster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       86 2024-04-19 18:02:20.000000 dagster-1.7.2rc4/dagster.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     1461 2024-04-19 18:02:20.000000 dagster-1.7.2rc4/dagster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-19 18:02:20.000000 dagster-1.7.2rc4/dagster.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      154 2024-04-19 18:02:21.701783 dagster-1.7.2rc4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     6830 2024-04-19 18:01:50.000000 dagster-1.7.2rc4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.772266 dagster-1.7.3/
+-rw-r--r--   0 root         (0) root         (0)      553 2024-04-25 20:08:31.000000 dagster-1.7.3/COPYING
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-04-25 20:08:31.000000 dagster-1.7.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      533 2024-04-25 20:08:31.000000 dagster-1.7.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     9867 2024-04-25 20:08:56.772266 dagster-1.7.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8153 2024-04-25 20:08:31.000000 dagster-1.7.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.688266 dagster-1.7.3/dagster/
+-rw-r--r--   0 root         (0) root         (0)    29906 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    20744 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_annotations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.692266 dagster-1.7.3/dagster/_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      731 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_api/get_server_id.py
+-rw-r--r--   0 root         (0) root         (0)     2147 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_api/list_repositories.py
+-rw-r--r--   0 root         (0) root         (0)      531 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_api/notebook_data.py
+-rw-r--r--   0 root         (0) root         (0)     3224 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_api/snapshot_execution_plan.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_api/snapshot_job.py
+-rw-r--r--   0 root         (0) root         (0)     5483 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_api/snapshot_partition.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_api/snapshot_repository.py
+-rw-r--r--   0 root         (0) root         (0)     3021 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_api/snapshot_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     3370 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_api/snapshot_sensor.py
+-rw-r--r--   0 root         (0) root         (0)      478 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_builtins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.692266 dagster-1.7.3/dagster/_check/
+-rw-r--r--   0 root         (0) root         (0)     1352 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_check/README.md
+-rw-r--r--   0 root         (0) root         (0)    52040 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_check/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.692266 dagster-1.7.3/dagster/_cli/
+-rw-r--r--   0 root         (0) root         (0)     1182 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26898 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_cli/api.py
+-rw-r--r--   0 root         (0) root         (0)     8030 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_cli/asset.py
+-rw-r--r--   0 root         (0) root         (0)     8302 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_cli/code_server.py
+-rw-r--r--   0 root         (0) root         (0)     2374 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_cli/config_scaffolder.py
+-rw-r--r--   0 root         (0) root         (0)     3513 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_cli/debug.py
+-rw-r--r--   0 root         (0) root         (0)     8134 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_cli/dev.py
+-rw-r--r--   0 root         (0) root         (0)     6651 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_cli/instance.py
+-rw-r--r--   0 root         (0) root         (0)    30542 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_cli/job.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_cli/load_handle.py
+-rw-r--r--   0 root         (0) root         (0)     9114 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_cli/project.py
+-rw-r--r--   0 root         (0) root         (0)     5120 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_cli/run.py
+-rw-r--r--   0 root         (0) root         (0)    19351 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_cli/schedule.py
+-rw-r--r--   0 root         (0) root         (0)    15461 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_cli/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     4259 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_cli/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.692266 dagster-1.7.3/dagster/_cli/workspace/
+-rw-r--r--   0 root         (0) root         (0)      180 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_cli/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27910 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_cli/workspace/cli_target.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.696266 dagster-1.7.3/dagster/_config/
+-rw-r--r--   0 root         (0) root         (0)     3186 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3403 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    15830 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/config_type.py
+-rw-r--r--   0 root         (0) root         (0)    18787 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1783 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/evaluate_value_result.py
+-rw-r--r--   0 root         (0) root         (0)    14918 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/field.py
+-rw-r--r--   0 root         (0) root         (0)    19728 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/field_utils.py
+-rw-r--r--   0 root         (0) root         (0)     9536 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/post_process.py
+-rw-r--r--   0 root         (0) root         (0)      855 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/primitive_mapping.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.696266 dagster-1.7.3/dagster/_config/pythonic_config/
+-rw-r--r--   0 root         (0) root         (0)     1394 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/pythonic_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1641 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/pythonic_config/attach_other_object_to_context.py
+-rw-r--r--   0 root         (0) root         (0)    18116 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/pythonic_config/config.py
+-rw-r--r--   0 root         (0) root         (0)    11510 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/pythonic_config/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)    11583 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/pythonic_config/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)    41265 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/pythonic_config/resource.py
+-rw-r--r--   0 root         (0) root         (0)     1996 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/pythonic_config/type_check_utils.py
+-rw-r--r--   0 root         (0) root         (0)     8375 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/pythonic_config/typing_utils.py
+-rw-r--r--   0 root         (0) root         (0)    12532 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/snap.py
+-rw-r--r--   0 root         (0) root         (0)     3087 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/source.py
+-rw-r--r--   0 root         (0) root         (0)     3528 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/stack.py
+-rw-r--r--   0 root         (0) root         (0)     7772 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/traversal_context.py
+-rw-r--r--   0 root         (0) root         (0)     4167 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/type_printer.py
+-rw-r--r--   0 root         (0) root         (0)    17137 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/validate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.700266 dagster-1.7.3/dagster/_core/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.700266 dagster-1.7.3/dagster/_core/asset_graph_view/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/asset_graph_view/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21047 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/asset_graph_view/asset_graph_view.py
+-rw-r--r--   0 root         (0) root         (0)      994 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/assets.py
+-rw-r--r--   0 root         (0) root         (0)    13427 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/code_pointer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.700266 dagster-1.7.3/dagster/_core/container_context/
+-rw-r--r--   0 root         (0) root         (0)      184 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/container_context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1278 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/container_context/config.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/debug.py
+-rw-r--r--   0 root         (0) root         (0)     9665 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/decorator_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.712266 dagster-1.7.3/dagster/_core/definitions/
+-rw-r--r--   0 root         (0) root         (0)     7827 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4506 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_check_evaluation.py
+-rw-r--r--   0 root         (0) root         (0)     7052 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_check_result.py
+-rw-r--r--   0 root         (0) root         (0)     5628 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_check_spec.py
+-rw-r--r--   0 root         (0) root         (0)     6092 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_checks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.712266 dagster-1.7.3/dagster/_core/definitions/asset_condition/
+-rw-r--r--   0 root         (0) root         (0)       62 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_condition/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21064 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_condition/asset_condition.py
+-rw-r--r--   0 root         (0) root         (0)    16508 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_condition/asset_condition_evaluation_context.py
+-rw-r--r--   0 root         (0) root         (0)    26314 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_daemon_context.py
+-rw-r--r--   0 root         (0) root         (0)    10648 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_daemon_cursor.py
+-rw-r--r--   0 root         (0) root         (0)     4628 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_dep.py
+-rw-r--r--   0 root         (0) root         (0)    10133 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)     7696 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_graph_differ.py
+-rw-r--r--   0 root         (0) root         (0)    16636 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_graph_subset.py
+-rw-r--r--   0 root         (0) root         (0)     3644 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_in.py
+-rw-r--r--   0 root         (0) root         (0)    29917 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_job.py
+-rw-r--r--   0 root         (0) root         (0)     6060 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_key.py
+-rw-r--r--   0 root         (0) root         (0)    30355 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_layer.py
+-rw-r--r--   0 root         (0) root         (0)     6945 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_out.py
+-rw-r--r--   0 root         (0) root         (0)    39535 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_selection.py
+-rw-r--r--   0 root         (0) root         (0)     7444 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6764 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_spec.py
+-rw-r--r--   0 root         (0) root         (0)    10723 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_subset.py
+-rw-r--r--   0 root         (0) root         (0)    79909 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/assets.py
+-rw-r--r--   0 root         (0) root         (0)    13905 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/auto_materialize_policy.py
+-rw-r--r--   0 root         (0) root         (0)    54478 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/auto_materialize_rule.py
+-rw-r--r--   0 root         (0) root         (0)    21726 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/auto_materialize_rule_evaluation.py
+-rw-r--r--   0 root         (0) root         (0)     2768 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/auto_materialize_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)     2939 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/backfill_policy.py
+-rw-r--r--   0 root         (0) root         (0)    34666 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/base_asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)    16772 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/cacheable_assets.py
+-rw-r--r--   0 root         (0) root         (0)    40623 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/composition.py
+-rw-r--r--   0 root         (0) root         (0)     4278 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/config.py
+-rw-r--r--   0 root         (0) root         (0)    14811 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/configurable.py
+-rw-r--r--   0 root         (0) root         (0)    22990 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/data_time.py
+-rw-r--r--   0 root         (0) root         (0)    30155 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/data_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.712266 dagster-1.7.3/dagster/_core/definitions/decorators/
+-rw-r--r--   0 root         (0) root         (0)      620 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16572 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/decorators/asset_check_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    69618 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/decorators/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     4907 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/decorators/config_mapping_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     9077 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/decorators/graph_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     9353 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/decorators/hook_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    10815 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/decorators/job_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    19011 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/decorators/op_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    15668 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/decorators/repository_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     8718 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/decorators/schedule_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    12463 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/decorators/sensor_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    12664 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/decorators/source_asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     5267 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/definition_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    23545 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/definitions_class.py
+-rw-r--r--   0 root         (0) root         (0)    42243 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/dependency.py
+-rw-r--r--   0 root         (0) root         (0)    26888 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/events.py
+-rw-r--r--   0 root         (0) root         (0)    21182 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/executor_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9379 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/external_asset.py
+-rw-r--r--   0 root         (0) root         (0)     9766 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/freshness_based_auto_materialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.716266 dagster-1.7.3/dagster/_core/definitions/freshness_checks/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/freshness_checks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5838 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/freshness_checks/last_update.py
+-rw-r--r--   0 root         (0) root         (0)     7685 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/freshness_checks/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     9349 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/freshness_checks/shared_builder.py
+-rw-r--r--   0 root         (0) root         (0)     4669 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/freshness_checks/time_partition.py
+-rw-r--r--   0 root         (0) root         (0)    10409 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/freshness_checks/utils.py
+-rw-r--r--   0 root         (0) root         (0)     8801 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/freshness_policy.py
+-rw-r--r--   0 root         (0) root         (0)    16401 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/freshness_policy_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    47569 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/graph_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6546 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/hook_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1524 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/hook_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3537 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/inference.py
+-rw-r--r--   0 root         (0) root         (0)    21027 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/input.py
+-rw-r--r--   0 root         (0) root         (0)     6410 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/instigation_logger.py
+-rw-r--r--   0 root         (0) root         (0)     2991 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/job_base.py
+-rw-r--r--   0 root         (0) root         (0)    53689 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/job_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5693 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/load_asset_checks_from_modules.py
+-rw-r--r--   0 root         (0) root         (0)    22306 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/load_assets_from_modules.py
+-rw-r--r--   0 root         (0) root         (0)     7171 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/logger_definition.py
+-rw-r--r--   0 root         (0) root         (0)      636 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/logger_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     8959 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/materialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.716266 dagster-1.7.3/dagster/_core/definitions/metadata/
+-rw-r--r--   0 root         (0) root         (0)    42209 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12410 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/metadata/table.py
+-rw-r--r--   0 root         (0) root         (0)    57203 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/multi_asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    22029 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/multi_dimensional_partitions.py
+-rw-r--r--   0 root         (0) root         (0)      197 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/no_step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)    11892 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/node_container.py
+-rw-r--r--   0 root         (0) root         (0)     8016 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/node_definition.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/observe.py
+-rw-r--r--   0 root         (0) root         (0)    23078 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/op_definition.py
+-rw-r--r--   0 root         (0) root         (0)    23141 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/op_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     7551 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/op_selection.py
+-rw-r--r--   0 root         (0) root         (0)    19237 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/output.py
+-rw-r--r--   0 root         (0) root         (0)    50520 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/partition.py
+-rw-r--r--   0 root         (0) root         (0)      630 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/partition_key_range.py
+-rw-r--r--   0 root         (0) root         (0)    47665 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)    11087 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/partitioned_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     3779 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/policy.py
+-rw-r--r--   0 root         (0) root         (0)    27733 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/reconstruct.py
+-rw-r--r--   0 root         (0) root         (0)    21602 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/remote_asset_graph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.716266 dagster-1.7.3/dagster/_core/definitions/repository_definition/
+-rw-r--r--   0 root         (0) root         (0)      654 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/repository_definition/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6024 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/repository_definition/caching_index.py
+-rw-r--r--   0 root         (0) root         (0)    21698 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/repository_definition/repository_data.py
+-rw-r--r--   0 root         (0) root         (0)    20892 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/repository_definition/repository_data_builder.py
+-rw-r--r--   0 root         (0) root         (0)    20432 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/repository_definition/repository_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/repository_definition/valid_definitions.py
+-rw-r--r--   0 root         (0) root         (0)     8858 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/resolved_asset_deps.py
+-rw-r--r--   0 root         (0) root         (0)     1465 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/resource_annotation.py
+-rw-r--r--   0 root         (0) root         (0)    17900 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/resource_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5382 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/resource_invocation.py
+-rw-r--r--   0 root         (0) root         (0)    10320 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/resource_requirement.py
+-rw-r--r--   0 root         (0) root         (0)     3383 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/result.py
+-rw-r--r--   0 root         (0) root         (0)    23076 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/run_config.py
+-rw-r--r--   0 root         (0) root         (0)     1445 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/run_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    19555 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/run_request.py
+-rw-r--r--   0 root         (0) root         (0)    44126 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/run_status_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    39363 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/schedule_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6209 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/schema_change_checks.py
+-rw-r--r--   0 root         (0) root         (0)     5134 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/scoped_resources_builder.py
+-rw-r--r--   0 root         (0) root         (0)    14134 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/selector.py
+-rw-r--r--   0 root         (0) root         (0)    53797 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    19244 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/source_asset.py
+-rw-r--r--   0 root         (0) root         (0)     2481 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/target.py
+-rw-r--r--   0 root         (0) root         (0)    21859 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/time_window_partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)   102142 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/time_window_partitions.py
+-rw-r--r--   0 root         (0) root         (0)    15160 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/unresolved_asset_job_definition.py
+-rw-r--r--   0 root         (0) root         (0)    11017 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3982 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/version_strategy.py
+-rw-r--r--   0 root         (0) root         (0)    26986 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/errors.py
+-rw-r--r--   0 root         (0) root         (0)    17452 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/event_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.716266 dagster-1.7.3/dagster/_core/events/
+-rw-r--r--   0 root         (0) root         (0)    71913 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/events/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8142 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/events/log.py
+-rw-r--r--   0 root         (0) root         (0)     1614 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/events/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.720266 dagster-1.7.3/dagster/_core/execution/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38363 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/api.py
+-rw-r--r--   0 root         (0) root         (0)    64654 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/asset_backfill.py
+-rw-r--r--   0 root         (0) root         (0)    17100 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/backfill.py
+-rw-r--r--   0 root         (0) root         (0)     6296 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/build_resources.py
+-rw-r--r--   0 root         (0) root         (0)      224 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/bulk_actions.py
+-rw-r--r--   0 root         (0) root         (0)     5587 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/compute_logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.720266 dagster-1.7.3/dagster/_core/execution/context/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    79687 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/context/compute.py
+-rw-r--r--   0 root         (0) root         (0)    17598 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/context/hook.py
+-rw-r--r--   0 root         (0) root         (0)     9613 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/context/init.py
+-rw-r--r--   0 root         (0) root         (0)    29167 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/context/input.py
+-rw-r--r--   0 root         (0) root         (0)    40124 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/context/invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3164 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/context/logger.py
+-rw-r--r--   0 root         (0) root         (0)    37256 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/context/output.py
+-rw-r--r--   0 root         (0) root         (0)    56002 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/context/system.py
+-rw-r--r--   0 root         (0) root         (0)    18837 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/context_creation_job.py
+-rw-r--r--   0 root         (0) root         (0)     5135 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/execute_in_process.py
+-rw-r--r--   0 root         (0) root         (0)     5897 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/execute_in_process_result.py
+-rw-r--r--   0 root         (0) root         (0)     9633 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/execution_result.py
+-rw-r--r--   0 root         (0) root         (0)     8602 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/host_mode.py
+-rw-r--r--   0 root         (0) root         (0)    14247 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/job_backfill.py
+-rw-r--r--   0 root         (0) root         (0)     6723 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/job_execution_result.py
+-rw-r--r--   0 root         (0) root         (0)      998 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/memoization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.724266 dagster-1.7.3/dagster/_core/execution/plan/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/plan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26460 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/plan/active.py
+-rw-r--r--   0 root         (0) root         (0)     9850 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/plan/compute.py
+-rw-r--r--   0 root         (0) root         (0)    17019 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/plan/compute_generator.py
+-rw-r--r--   0 root         (0) root         (0)    16974 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/plan/execute_plan.py
+-rw-r--r--   0 root         (0) root         (0)    40691 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/plan/execute_step.py
+-rw-r--r--   0 root         (0) root         (0)    11032 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/plan/external_step.py
+-rw-r--r--   0 root         (0) root         (0)     3664 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/plan/handle.py
+-rw-r--r--   0 root         (0) root         (0)    39260 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/plan/inputs.py
+-rw-r--r--   0 root         (0) root         (0)     6251 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/plan/instance_concurrency_context.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/plan/local_external_step_main.py
+-rw-r--r--   0 root         (0) root         (0)     5706 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/plan/objects.py
+-rw-r--r--   0 root         (0) root         (0)     7326 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/plan/outputs.py
+-rw-r--r--   0 root         (0) root         (0)    61075 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/plan/plan.py
+-rw-r--r--   0 root         (0) root         (0)      114 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/plan/resume_retry.py
+-rw-r--r--   0 root         (0) root         (0)    17174 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/plan/state.py
+-rw-r--r--   0 root         (0) root         (0)    15985 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/plan/step.py
+-rw-r--r--   0 root         (0) root         (0)     3796 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/plan/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/poll_compute_logs.py
+-rw-r--r--   0 root         (0) root         (0)     8230 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/resolve_versions.py
+-rw-r--r--   0 root         (0) root         (0)    19141 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/resources_init.py
+-rw-r--r--   0 root         (0) root         (0)     2100 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/retries.py
+-rw-r--r--   0 root         (0) root         (0)     1564 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/run_cancellation_thread.py
+-rw-r--r--   0 root         (0) root         (0)     9950 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/stats.py
+-rw-r--r--   0 root         (0) root         (0)    14043 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/submit_asset_runs.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1172 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/validate_run_config.py
+-rw-r--r--   0 root         (0) root         (0)     1282 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/watch_orphans.py
+-rw-r--r--   0 root         (0) root         (0)     4311 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/with_resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.724266 dagster-1.7.3/dagster/_core/executor/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/executor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/executor/base.py
+-rw-r--r--   0 root         (0) root         (0)     5989 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/executor/child_process_executor.py
+-rw-r--r--   0 root         (0) root         (0)     3366 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/executor/in_process.py
+-rw-r--r--   0 root         (0) root         (0)     1509 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/executor/init.py
+-rw-r--r--   0 root         (0) root         (0)    15497 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/executor/multiprocess.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.724266 dagster-1.7.3/dagster/_core/executor/step_delegating/
+-rw-r--r--   0 root         (0) root         (0)      247 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/executor/step_delegating/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16894 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/executor/step_delegating/step_delegating_executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.724266 dagster-1.7.3/dagster/_core/executor/step_delegating/step_handler/
+-rw-r--r--   0 root         (0) root         (0)      152 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/executor/step_delegating/step_handler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3078 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/executor/step_delegating/step_handler/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.724266 dagster-1.7.3/dagster/_core/instance/
+-rw-r--r--   0 root         (0) root         (0)   132334 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/instance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15788 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/instance/config.py
+-rw-r--r--   0 root         (0) root         (0)    24141 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/instance/ref.py
+-rw-r--r--   0 root         (0) root         (0)     3899 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/instance_for_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.724266 dagster-1.7.3/dagster/_core/launcher/
+-rw-r--r--   0 root         (0) root         (0)      297 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3819 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/launcher/base.py
+-rw-r--r--   0 root         (0) root         (0)     6645 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/launcher/default_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1566 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/launcher/sync_in_memory_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)      473 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/libraries.py
+-rw-r--r--   0 root         (0) root         (0)    18041 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1029 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/nux.py
+-rw-r--r--   0 root         (0) root         (0)     6656 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/op_concurrency_limits_counter.py
+-rw-r--r--   0 root         (0) root         (0)     3691 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/origin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.724266 dagster-1.7.3/dagster/_core/pipes/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/pipes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8974 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/pipes/client.py
+-rw-r--r--   0 root         (0) root         (0)    18318 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/pipes/context.py
+-rw-r--r--   0 root         (0) root         (0)     5648 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/pipes/subprocess.py
+-rw-r--r--   0 root         (0) root         (0)    25661 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/pipes/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.728266 dagster-1.7.3/dagster/_core/remote_representation/
+-rw-r--r--   0 root         (0) root         (0)     2793 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/remote_representation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    36695 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/remote_representation/code_location.py
+-rw-r--r--   0 root         (0) root         (0)    37482 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/remote_representation/external.py
+-rw-r--r--   0 root         (0) root         (0)    83582 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/remote_representation/external_data.py
+-rw-r--r--   0 root         (0) root         (0)     1450 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/remote_representation/feature_flags.py
+-rw-r--r--   0 root         (0) root         (0)    12429 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/remote_representation/grpc_server_registry.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/remote_representation/grpc_server_state_subscriber.py
+-rw-r--r--   0 root         (0) root         (0)     4356 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/remote_representation/handle.py
+-rw-r--r--   0 root         (0) root         (0)     1581 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/remote_representation/historical.py
+-rw-r--r--   0 root         (0) root         (0)     4850 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/remote_representation/job_index.py
+-rw-r--r--   0 root         (0) root         (0)    19669 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/remote_representation/origin.py
+-rw-r--r--   0 root         (0) root         (0)     3602 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/remote_representation/represented.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.728266 dagster-1.7.3/dagster/_core/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      267 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2005 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/run_coordinator/base.py
+-rw-r--r--   0 root         (0) root         (0)     1922 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/run_coordinator/default_run_coordinator.py
+-rw-r--r--   0 root         (0) root         (0)    13364 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/run_coordinator/queued_run_coordinator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.728266 dagster-1.7.3/dagster/_core/scheduler/
+-rw-r--r--   0 root         (0) root         (0)      534 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/scheduler/execution.py
+-rw-r--r--   0 root         (0) root         (0)    28809 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/scheduler/instigation.py
+-rw-r--r--   0 root         (0) root         (0)    10917 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/scheduler/scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.728266 dagster-1.7.3/dagster/_core/secrets/
+-rw-r--r--   0 root         (0) root         (0)       51 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1801 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/secrets/env_file.py
+-rw-r--r--   0 root         (0) root         (0)      388 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/secrets/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.728266 dagster-1.7.3/dagster/_core/selector/
+-rw-r--r--   0 root         (0) root         (0)      295 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/selector/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18109 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/selector/subset_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.732266 dagster-1.7.3/dagster/_core/snap/
+-rw-r--r--   0 root         (0) root         (0)     2842 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/snap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      494 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/snap/config_types.py
+-rw-r--r--   0 root         (0) root         (0)     3999 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/snap/dagster_types.py
+-rw-r--r--   0 root         (0) root         (0)     9302 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/snap/dep_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    12155 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/snap/execution_plan_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    16934 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/snap/job_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     4561 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/snap/mode.py
+-rw-r--r--   0 root         (0) root         (0)    14185 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/snap/node.py
+-rw-r--r--   0 root         (0) root         (0)     3183 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/snap/snap_to_yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.736266 dagster-1.7.3/dagster/_core/storage/
+-rw-r--r--   0 root         (0) root         (0)     3058 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/DEVELOPING.md
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.736266 dagster-1.7.3/dagster/_core/storage/alembic/
+-rw-r--r--   0 root         (0) root         (0)     6686 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/README.md
+-rw-r--r--   0 root         (0) root         (0)      687 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      494 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.748266 dagster-1.7.3/dagster/_core/storage/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     3150 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/001_initial_1.py
+-rw-r--r--   0 root         (0) root         (0)      312 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/001_initial_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     1486 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      599 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      973 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      973 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     2729 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      953 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      953 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      956 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      956 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1171 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1171 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
+-rw-r--r--   0 root         (0) root         (0)      417 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      417 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      435 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      435 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      432 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      432 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     3927 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     3927 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      409 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      409 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      936 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      936 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      325 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/017_initial_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1032 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      433 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      433 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      433 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      531 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      404 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      404 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      404 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      635 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      434 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      434 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      434 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      416 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      416 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      416 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1893 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
+-rw-r--r--   0 root         (0) root         (0)      958 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
+-rw-r--r--   0 root         (0) root         (0)      499 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
+-rw-r--r--   0 root         (0) root         (0)     1951 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
+-rw-r--r--   0 root         (0) root         (0)      428 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
+-rw-r--r--   0 root         (0) root         (0)      427 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
+-rw-r--r--   0 root         (0) root         (0)     1537 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
+-rw-r--r--   0 root         (0) root         (0)     2481 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py
+-rw-r--r--   0 root         (0) root         (0)     2062 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py
+-rw-r--r--   0 root         (0) root         (0)     2359 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py
+-rw-r--r--   0 root         (0) root         (0)     2898 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/041_add_asset_check_executions_table.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/042_46b412388816_add_concurrency_limits_table.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3887 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/asset_check_execution_record.py
+-rw-r--r--   0 root         (0) root         (0)     7301 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/asset_value_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1227 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/base_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.748266 dagster-1.7.3/dagster/_core/storage/branching/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/branching/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5579 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/branching/branching_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8725 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/captured_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)    16223 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/cloud_storage_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     9557 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1863 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/config.py
+-rw-r--r--   0 root         (0) root         (0)      417 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/daemon_cursor.py
+-rw-r--r--   0 root         (0) root         (0)    25652 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/dagster_run.py
+-rw-r--r--   0 root         (0) root         (0)    11187 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/db_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.748266 dagster-1.7.3/dagster/_core/storage/event_log/
+-rw-r--r--   0 root         (0) root         (0)      742 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/event_log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19078 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/event_log/base.py
+-rw-r--r--   0 root         (0) root         (0)     3801 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/event_log/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     7289 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/event_log/migration.py
+-rw-r--r--   0 root         (0) root         (0)     8037 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/event_log/polling_event_watcher.py
+-rw-r--r--   0 root         (0) root         (0)     9250 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/event_log/schema.py
+-rw-r--r--   0 root         (0) root         (0)   121159 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/event_log/sql_event_log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.752266 dagster-1.7.3/dagster/_core/storage/event_log/sqlite/
+-rw-r--r--   0 root         (0) root         (0)      200 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/event_log/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.752266 dagster-1.7.3/dagster/_core/storage/event_log/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)      986 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     7508 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    22497 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    10983 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/file_manager.py
+-rw-r--r--   0 root         (0) root         (0)    13492 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/fs_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8819 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/input_manager.py
+-rw-r--r--   0 root         (0) root         (0)    10882 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)    32629 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/legacy_storage.py
+-rw-r--r--   0 root         (0) root         (0)    17558 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/local_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1167 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/mem_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4355 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/memoizable_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.752266 dagster-1.7.3/dagster/_core/storage/migration/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/migration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5964 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/migration/bigint_migration.py
+-rw-r--r--   0 root         (0) root         (0)    15491 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/migration/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3270 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/noop_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2361 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/output_manager.py
+-rw-r--r--   0 root         (0) root         (0)    17398 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/partition_status_cache.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/root.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.752266 dagster-1.7.3/dagster/_core/storage/runs/
+-rw-r--r--   0 root         (0) root         (0)      386 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/runs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13903 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/runs/base.py
+-rw-r--r--   0 root         (0) root         (0)     2452 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/runs/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     8716 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/runs/migration.py
+-rw-r--r--   0 root         (0) root         (0)     6391 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/runs/schema.py
+-rw-r--r--   0 root         (0) root         (0)    37611 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/runs/sql_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.752266 dagster-1.7.3/dagster/_core/storage/runs/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       69 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/runs/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.752266 dagster-1.7.3/dagster/_core/storage/runs/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)      986 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     6310 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.752266 dagster-1.7.3/dagster/_core/storage/schedules/
+-rw-r--r--   0 root         (0) root         (0)      272 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7236 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/schedules/base.py
+-rw-r--r--   0 root         (0) root         (0)     4133 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/schedules/migration.py
+-rw-r--r--   0 root         (0) root         (0)     4086 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/schedules/schema.py
+-rw-r--r--   0 root         (0) root         (0)    25146 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/schedules/sql_schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.752266 dagster-1.7.3/dagster/_core/storage/schedules/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       84 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/schedules/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.752266 dagster-1.7.3/dagster/_core/storage/schedules/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)      986 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     3684 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
+-rw-r--r--   0 root         (0) root         (0)     7691 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/sql.py
+-rw-r--r--   0 root         (0) root         (0)     1391 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/sqlalchemy_compat.py
+-rw-r--r--   0 root         (0) root         (0)      926 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     4875 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/sqlite_storage.py
+-rw-r--r--   0 root         (0) root         (0)     3546 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1186 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/temp_file_manager.py
+-rw-r--r--   0 root         (0) root         (0)    19215 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/upath_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.752266 dagster-1.7.3/dagster/_core/system_config/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/system_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13962 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/system_config/composite_descent.py
+-rw-r--r--   0 root         (0) root         (0)    15178 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/system_config/objects.py
+-rw-r--r--   0 root         (0) root         (0)    29921 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     4824 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/telemetry_upload.py
+-rw-r--r--   0 root         (0) root         (0)    22361 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.756266 dagster-1.7.3/dagster/_core/types/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3084 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/types/builtin_config_schemas.py
+-rw-r--r--   0 root         (0) root         (0)     7042 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/types/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    36504 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/types/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)     3571 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/types/decorator.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/types/loadable_target_origin.py
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/types/primitive_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     4764 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/types/python_dict.py
+-rw-r--r--   0 root         (0) root         (0)     2769 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/types/python_set.py
+-rw-r--r--   0 root         (0) root         (0)     3620 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/types/python_tuple.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/types/transform_typing.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/utility_ops.py
+-rw-r--r--   0 root         (0) root         (0)     6652 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.756266 dagster-1.7.3/dagster/_core/workspace/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4457 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/workspace/autodiscovery.py
+-rw-r--r--   0 root         (0) root         (0)     3160 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/workspace/batch_asset_record_loader.py
+-rw-r--r--   0 root         (0) root         (0)     3422 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/workspace/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    29210 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/workspace/context.py
+-rw-r--r--   0 root         (0) root         (0)    11852 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/workspace/load.py
+-rw-r--r--   0 root         (0) root         (0)     4721 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/workspace/load_target.py
+-rw-r--r--   0 root         (0) root         (0)     4311 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/workspace/permissions.py
+-rw-r--r--   0 root         (0) root         (0)     3463 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/workspace/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.760266 dagster-1.7.3/dagster/_daemon/
+-rw-r--r--   0 root         (0) root         (0)     1971 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_daemon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       30 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_daemon/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    41795 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_daemon/asset_daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.760266 dagster-1.7.3/dagster/_daemon/auto_run_reexecution/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_daemon/auto_run_reexecution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7402 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
+-rw-r--r--   0 root         (0) root         (0)     9036 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
+-rw-r--r--   0 root         (0) root         (0)     2665 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_daemon/backfill.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.760266 dagster-1.7.3/dagster/_daemon/cli/
+-rw-r--r--   0 root         (0) root         (0)     5118 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_daemon/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19590 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_daemon/controller.py
+-rw-r--r--   0 root         (0) root         (0)    12112 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_daemon/daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.760266 dagster-1.7.3/dagster/_daemon/monitoring/
+-rw-r--r--   0 root         (0) root         (0)      320 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_daemon/monitoring/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1792 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_daemon/monitoring/concurrency.py
+-rw-r--r--   0 root         (0) root         (0)     9904 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_daemon/monitoring/run_monitoring.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.760266 dagster-1.7.3/dagster/_daemon/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      100 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_daemon/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18725 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
+-rw-r--r--   0 root         (0) root         (0)    39110 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_daemon/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     2860 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_daemon/types.py
+-rw-r--r--   0 root         (0) root         (0)      678 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_daemon/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4114 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_daemon/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.760266 dagster-1.7.3/dagster/_experimental/
+-rw-r--r--   0 root         (0) root         (0)      300 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_experimental/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.760266 dagster-1.7.3/dagster/_generate/
+-rw-r--r--   0 root         (0) root         (0)      253 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_generate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_generate/download.py
+-rw-r--r--   0 root         (0) root         (0)     4805 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_generate/generate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.688266 dagster-1.7.3/dagster/_generate/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.760266 dagster-1.7.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.760266 dagster-1.7.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)      175 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.760266 dagster-1.7.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)      137 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
+-rw-r--r--   0 root         (0) root         (0)       43 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      297 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.760266 dagster-1.7.3/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)     1753 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.760266 dagster-1.7.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.764266 dagster-1.7.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)       40 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
+-rw-r--r--   0 root         (0) root         (0)      164 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.764266 dagster-1.7.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)       80 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       34 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      279 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.764266 dagster-1.7.3/dagster/_grpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.764266 dagster-1.7.3/dagster/_grpc/__generated__/
+-rw-r--r--   0 root         (0) root         (0)      178 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_grpc/__generated__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13462 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_grpc/__generated__/api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    27262 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_grpc/__generated__/api_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)    43164 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_grpc/__generated__/api_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2060 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       89 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_grpc/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    22739 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_grpc/client.py
+-rw-r--r--   0 root         (0) root         (0)     3584 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_grpc/compile.py
+-rw-r--r--   0 root         (0) root         (0)    23173 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_grpc/impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.764266 dagster-1.7.3/dagster/_grpc/protos/
+-rw-r--r--   0 root         (0) root         (0)     5993 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_grpc/protos/api.proto
+-rw-r--r--   0 root         (0) root         (0)    13431 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_grpc/proxy_server.py
+-rw-r--r--   0 root         (0) root         (0)    60914 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_grpc/server.py
+-rw-r--r--   0 root         (0) root         (0)     5297 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_grpc/server_watcher.py
+-rw-r--r--   0 root         (0) root         (0)    29291 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_grpc/types.py
+-rw-r--r--   0 root         (0) root         (0)     3693 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_grpc/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.764266 dagster-1.7.3/dagster/_legacy/
+-rw-r--r--   0 root         (0) root         (0)      180 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_legacy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.764266 dagster-1.7.3/dagster/_loggers/
+-rw-r--r--   0 root         (0) root         (0)     3781 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_loggers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.764266 dagster-1.7.3/dagster/_model/
+-rw-r--r--   0 root         (0) root         (0)     1373 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3897 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_model/pydantic_compat_layer.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_module_alias_map.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.764266 dagster-1.7.3/dagster/_scheduler/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    41378 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_scheduler/scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     1262 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_scheduler/stale.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.768266 dagster-1.7.3/dagster/_serdes/
+-rw-r--r--   0 root         (0) root         (0)      701 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_serdes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8916 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_serdes/config_class.py
+-rw-r--r--   0 root         (0) root         (0)      142 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_serdes/errors.py
+-rw-r--r--   0 root         (0) root         (0)     7292 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_serdes/ipc.py
+-rw-r--r--   0 root         (0) root         (0)    43115 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_serdes/serdes.py
+-rw-r--r--   0 root         (0) root         (0)      674 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_serdes/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.768266 dagster-1.7.3/dagster/_seven/
+-rw-r--r--   0 root         (0) root         (0)     5455 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_seven/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      553 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_seven/abc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.768266 dagster-1.7.3/dagster/_seven/compat/
+-rw-r--r--   0 root         (0) root         (0)      105 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_seven/compat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3967 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_seven/compat/pendulum.py
+-rw-r--r--   0 root         (0) root         (0)      383 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_seven/json.py
+-rw-r--r--   0 root         (0) root         (0)      354 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_seven/temp_dir.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.772266 dagster-1.7.3/dagster/_utils/
+-rw-r--r--   0 root         (0) root         (0)    24377 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9314 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/alert.py
+-rw-r--r--   0 root         (0) root         (0)     2250 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/backoff.py
+-rw-r--r--   0 root         (0) root         (0)     5404 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/cached_method.py
+-rw-r--r--   0 root         (0) root         (0)    42998 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/caching_instance_queryer.py
+-rw-r--r--   0 root         (0) root         (0)     5865 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/concurrency.py
+-rw-r--r--   0 root         (0) root         (0)    12887 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/container.py
+-rw-r--r--   0 root         (0) root         (0)     2412 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)      799 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/env.py
+-rw-r--r--   0 root         (0) root         (0)     5477 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/error.py
+-rw-r--r--   0 root         (0) root         (0)     1255 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/external.py
+-rw-r--r--   0 root         (0) root         (0)      891 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/forked_pdb.py
+-rw-r--r--   0 root         (0) root         (0)     1870 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/hosted_user_process.py
+-rw-r--r--   0 root         (0) root         (0)     2796 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/indenting_printer.py
+-rw-r--r--   0 root         (0) root         (0)      745 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/internal_init.py
+-rw-r--r--   0 root         (0) root         (0)     3227 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/interrupts.py
+-rw-r--r--   0 root         (0) root         (0)    11214 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/log.py
+-rw-r--r--   0 root         (0) root         (0)     2313 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/merger.py
+-rw-r--r--   0 root         (0) root         (0)     1507 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/net.py
+-rw-r--r--   0 root         (0) root         (0)      208 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/partitions.py
+-rw-r--r--   0 root         (0) root         (0)    33445 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/schedules.py
+-rw-r--r--   0 root         (0) root         (0)      477 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/security.py
+-rw-r--r--   0 root         (0) root         (0)     3289 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/temp_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.772266 dagster-1.7.3/dagster/_utils/test/
+-rw-r--r--   0 root         (0) root         (0)    13678 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7790 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/test/data_versions.py
+-rw-r--r--   0 root         (0) root         (0)      119 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/test/hello_world_defs.py
+-rw-r--r--   0 root         (0) root         (0)      214 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/test/hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     8622 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/test/mysql_instance.py
+-rw-r--r--   0 root         (0) root         (0)      256 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/test/named_hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     8959 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/test/postgres_instance.py
+-rw-r--r--   0 root         (0) root         (0)    36138 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/test/schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.772266 dagster-1.7.3/dagster/_utils/test/toys/
+-rw-r--r--   0 root         (0) root         (0)       83 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/test/toys/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       84 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/test/toys/single_repository.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/timing.py
+-rw-r--r--   0 root         (0) root         (0)     1032 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/typed_dict.py
+-rw-r--r--   0 root         (0) root         (0)      170 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/types.py
+-rw-r--r--   0 root         (0) root         (0)     3334 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/typing_api.py
+-rw-r--r--   0 root         (0) root         (0)     4740 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/warnings.py
+-rw-r--r--   0 root         (0) root         (0)     4902 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/yaml_utils.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/py.typed
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.688266 dagster-1.7.3/dagster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9867 2024-04-25 20:08:56.000000 dagster-1.7.3/dagster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    28024 2024-04-25 20:08:56.000000 dagster-1.7.3/dagster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 20:08:56.000000 dagster-1.7.3/dagster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2024-04-25 20:08:56.000000 dagster-1.7.3/dagster.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     1458 2024-04-25 20:08:56.000000 dagster-1.7.3/dagster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-25 20:08:56.000000 dagster-1.7.3/dagster.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      154 2024-04-25 20:08:56.772266 dagster-1.7.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     6827 2024-04-25 20:08:31.000000 dagster-1.7.3/setup.py
```

### Comparing `dagster-1.7.2rc4/COPYING` & `dagster-1.7.3/COPYING`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/LICENSE` & `dagster-1.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/MANIFEST.in` & `dagster-1.7.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/PKG-INFO` & `dagster-1.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.7.2rc4
+Version: 1.7.3
 Summary: Dagster is an orchestration platform for the development, production, and observation of data assets.
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Documentation, https://docs.dagster.io
```

### Comparing `dagster-1.7.2rc4/README.md` & `dagster-1.7.3/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/__init__.py` & `dagster-1.7.3/dagster/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_annotations.py` & `dagster-1.7.3/dagster/_annotations.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_api/get_server_id.py` & `dagster-1.7.3/dagster/_api/get_server_id.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_api/list_repositories.py` & `dagster-1.7.3/dagster/_api/list_repositories.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_api/notebook_data.py` & `dagster-1.7.3/dagster/_api/notebook_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_api/snapshot_execution_plan.py` & `dagster-1.7.3/dagster/_api/snapshot_execution_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_api/snapshot_job.py` & `dagster-1.7.3/dagster/_api/snapshot_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_api/snapshot_partition.py` & `dagster-1.7.3/dagster/_api/snapshot_partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_api/snapshot_repository.py` & `dagster-1.7.3/dagster/_api/snapshot_repository.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_api/snapshot_schedule.py` & `dagster-1.7.3/dagster/_api/snapshot_schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_api/snapshot_sensor.py` & `dagster-1.7.3/dagster/_api/snapshot_sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_check/README.md` & `dagster-1.7.3/dagster/_check/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_check/__init__.py` & `dagster-1.7.3/dagster/_check/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_cli/__init__.py` & `dagster-1.7.3/dagster/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_cli/api.py` & `dagster-1.7.3/dagster/_cli/api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_cli/asset.py` & `dagster-1.7.3/dagster/_cli/asset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_cli/code_server.py` & `dagster-1.7.3/dagster/_cli/code_server.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_cli/config_scaffolder.py` & `dagster-1.7.3/dagster/_cli/config_scaffolder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_cli/debug.py` & `dagster-1.7.3/dagster/_cli/debug.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_cli/dev.py` & `dagster-1.7.3/dagster/_cli/dev.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_cli/instance.py` & `dagster-1.7.3/dagster/_cli/instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_cli/job.py` & `dagster-1.7.3/dagster/_cli/job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_cli/load_handle.py` & `dagster-1.7.3/dagster/_cli/load_handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_cli/project.py` & `dagster-1.7.3/dagster/_cli/project.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_cli/run.py` & `dagster-1.7.3/dagster/_cli/run.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_cli/schedule.py` & `dagster-1.7.3/dagster/_cli/schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_cli/sensor.py` & `dagster-1.7.3/dagster/_cli/sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_cli/utils.py` & `dagster-1.7.3/dagster/_cli/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_cli/workspace/cli_target.py` & `dagster-1.7.3/dagster/_cli/workspace/cli_target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_config/__init__.py` & `dagster-1.7.3/dagster/_config/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_config/config_schema.py` & `dagster-1.7.3/dagster/_config/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_config/config_type.py` & `dagster-1.7.3/dagster/_config/config_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_config/errors.py` & `dagster-1.7.3/dagster/_config/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_config/evaluate_value_result.py` & `dagster-1.7.3/dagster/_config/evaluate_value_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_config/field.py` & `dagster-1.7.3/dagster/_config/field.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_config/field_utils.py` & `dagster-1.7.3/dagster/_config/field_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_config/post_process.py` & `dagster-1.7.3/dagster/_config/post_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_config/primitive_mapping.py` & `dagster-1.7.3/dagster/_config/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_config/pythonic_config/__init__.py` & `dagster-1.7.3/dagster/_config/pythonic_config/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_config/pythonic_config/attach_other_object_to_context.py` & `dagster-1.7.3/dagster/_config/pythonic_config/attach_other_object_to_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_config/pythonic_config/config.py` & `dagster-1.7.3/dagster/_config/pythonic_config/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_config/pythonic_config/conversion_utils.py` & `dagster-1.7.3/dagster/_config/pythonic_config/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_config/pythonic_config/io_manager.py` & `dagster-1.7.3/dagster/_config/pythonic_config/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_config/pythonic_config/resource.py` & `dagster-1.7.3/dagster/_config/pythonic_config/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_config/pythonic_config/type_check_utils.py` & `dagster-1.7.3/dagster/_config/pythonic_config/type_check_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_config/pythonic_config/typing_utils.py` & `dagster-1.7.3/dagster/_config/pythonic_config/typing_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_config/snap.py` & `dagster-1.7.3/dagster/_config/snap.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_config/source.py` & `dagster-1.7.3/dagster/_config/source.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_config/stack.py` & `dagster-1.7.3/dagster/_config/stack.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_config/traversal_context.py` & `dagster-1.7.3/dagster/_config/traversal_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_config/type_printer.py` & `dagster-1.7.3/dagster/_config/type_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_config/validate.py` & `dagster-1.7.3/dagster/_config/validate.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/asset_graph_view/asset_graph_view.py` & `dagster-1.7.3/dagster/_core/asset_graph_view/asset_graph_view.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/assets.py` & `dagster-1.7.3/dagster/_core/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/code_pointer.py` & `dagster-1.7.3/dagster/_core/code_pointer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/container_context/config.py` & `dagster-1.7.3/dagster/_core/container_context/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/debug.py` & `dagster-1.7.3/dagster/_core/debug.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/decorator_utils.py` & `dagster-1.7.3/dagster/_core/decorator_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/__init__.py` & `dagster-1.7.3/dagster/_core/definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/asset_check_evaluation.py` & `dagster-1.7.3/dagster/_core/definitions/asset_check_evaluation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/asset_check_result.py` & `dagster-1.7.3/dagster/_core/definitions/asset_check_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/asset_check_spec.py` & `dagster-1.7.3/dagster/_core/definitions/asset_check_spec.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,19 @@
 
     def with_asset_key_prefix(self, prefix: CoercibleToAssetKeyPrefix) -> "AssetCheckKey":
         return self._replace(asset_key=self.asset_key.with_prefix(prefix))
 
     def to_user_string(self) -> str:
         return f"{self.asset_key.to_user_string()}:{self.name}"
 
+    @staticmethod
+    def from_user_string(user_string: str) -> "AssetCheckKey":
+        asset_key_str, name = user_string.split(":")
+        return AssetCheckKey(AssetKey.from_user_string(asset_key_str), name)
+
 
 class AssetCheckSpec(
     NamedTuple(
         "_AssetCheckSpec",
         [
             ("name", PublicAttr[str]),
             ("asset_key", PublicAttr[AssetKey]),
```

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/asset_checks.py` & `dagster-1.7.3/dagster/_core/definitions/asset_checks.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/asset_condition/asset_condition.py` & `dagster-1.7.3/dagster/_core/definitions/asset_condition/asset_condition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/asset_condition/asset_condition_evaluation_context.py` & `dagster-1.7.3/dagster/_core/definitions/asset_condition/asset_condition_evaluation_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/asset_daemon_context.py` & `dagster-1.7.3/dagster/_core/definitions/asset_daemon_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/asset_daemon_cursor.py` & `dagster-1.7.3/dagster/_core/definitions/asset_daemon_cursor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/asset_dep.py` & `dagster-1.7.3/dagster/_core/definitions/asset_dep.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/asset_graph.py` & `dagster-1.7.3/dagster/_core/definitions/asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/asset_graph_differ.py` & `dagster-1.7.3/dagster/_core/definitions/asset_graph_differ.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/asset_graph_subset.py` & `dagster-1.7.3/dagster/_core/definitions/asset_graph_subset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/asset_in.py` & `dagster-1.7.3/dagster/_core/definitions/asset_in.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/asset_job.py` & `dagster-1.7.3/dagster/_core/definitions/asset_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/asset_key.py` & `dagster-1.7.3/dagster/_core/definitions/asset_key.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/asset_layer.py` & `dagster-1.7.3/dagster/_core/definitions/asset_layer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/asset_out.py` & `dagster-1.7.3/dagster/_core/definitions/asset_out.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/asset_selection.py` & `dagster-1.7.3/dagster/_core/definitions/asset_selection.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/asset_sensor_definition.py` & `dagster-1.7.3/dagster/_core/definitions/asset_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/asset_spec.py` & `dagster-1.7.3/dagster/_core/definitions/asset_spec.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/asset_subset.py` & `dagster-1.7.3/dagster/_core/definitions/asset_subset.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,14 +180,20 @@
     def dict(self, **kwargs) -> dict:
         # Must be overridden as the Pydantic implementation errors when encountering NamedTuples
         # which have different fields than their __new__ method, which TimeWindowPartitionsSubset
         # unfortunately has.
         # This can likely be removed once TimeWindowPartitionsSubset is converted into a DagsterModel
         return {"asset_key": self.asset_key, "value": self.value}
 
+    def __eq__(self, other: Any) -> bool:
+        # Pydantic 2.x does not handle this comparison correctly for some reason, just override it
+        if not isinstance(other, AssetSubset):
+            return False
+        return self.dict() == other.dict()
+
 
 @whitelist_for_serdes(serializer=AssetSubsetSerializer)
 class ValidAssetSubset(AssetSubset):
     """Represents an AssetSubset which is known to be compatible with the current PartitionsDefinition
     of the asset represents.
 
     This class serializes to a regular AssetSubset, as it is unknown if this value will still be
```

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/assets.py` & `dagster-1.7.3/dagster/_core/definitions/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/auto_materialize_policy.py` & `dagster-1.7.3/dagster/_core/definitions/auto_materialize_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/auto_materialize_rule.py` & `dagster-1.7.3/dagster/_core/definitions/auto_materialize_rule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/auto_materialize_rule_evaluation.py` & `dagster-1.7.3/dagster/_core/definitions/auto_materialize_rule_evaluation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/auto_materialize_sensor_definition.py` & `dagster-1.7.3/dagster/_core/definitions/auto_materialize_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/backfill_policy.py` & `dagster-1.7.3/dagster/_core/definitions/backfill_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/base_asset_graph.py` & `dagster-1.7.3/dagster/_core/definitions/base_asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/cacheable_assets.py` & `dagster-1.7.3/dagster/_core/definitions/cacheable_assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/composition.py` & `dagster-1.7.3/dagster/_core/definitions/composition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/config.py` & `dagster-1.7.3/dagster/_core/definitions/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/configurable.py` & `dagster-1.7.3/dagster/_core/definitions/configurable.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/data_time.py` & `dagster-1.7.3/dagster/_core/definitions/data_time.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/data_version.py` & `dagster-1.7.3/dagster/_core/definitions/data_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -513,15 +513,18 @@
         # If a partition has greater than or equal to SKIP_PARTITION_DATA_VERSION_DEPENDENCY_THRESHOLD of
         # dependencies, it is not included in partition_deps. This is for performance reasons. This
         # constraint can be removed when we have thoroughly tested performance for large upstream
         # partition counts.
         partition_deps = self._get_partition_dependencies(key=key)
         for dep_key in sorted(partition_deps):
             dep_asset = self.asset_graph.get(dep_key.asset_key)
-            if self._get_status(key=dep_key) == StaleStatus.STALE:
+            if (
+                self._instance.use_transitive_stale_causes
+                and self._get_status(key=dep_key) == StaleStatus.STALE
+            ):
                 yield StaleCause(
                     key,
                     StaleCauseCategory.DATA,
                     "stale dependency",
                     dep_key,
                     self._get_stale_causes(key=dep_key),
                 )
```

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/decorators/__init__.py` & `dagster-1.7.3/dagster/_core/definitions/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/decorators/asset_check_decorator.py` & `dagster-1.7.3/dagster/_core/definitions/decorators/asset_check_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/decorators/asset_decorator.py` & `dagster-1.7.3/dagster/_core/definitions/decorators/asset_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/decorators/config_mapping_decorator.py` & `dagster-1.7.3/dagster/_core/definitions/decorators/config_mapping_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/decorators/graph_decorator.py` & `dagster-1.7.3/dagster/_core/definitions/decorators/graph_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/decorators/hook_decorator.py` & `dagster-1.7.3/dagster/_core/definitions/decorators/hook_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/decorators/job_decorator.py` & `dagster-1.7.3/dagster/_core/definitions/decorators/job_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/decorators/op_decorator.py` & `dagster-1.7.3/dagster/_core/definitions/decorators/op_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/decorators/repository_decorator.py` & `dagster-1.7.3/dagster/_core/definitions/decorators/repository_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/decorators/schedule_decorator.py` & `dagster-1.7.3/dagster/_core/definitions/decorators/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/decorators/sensor_decorator.py` & `dagster-1.7.3/dagster/_core/definitions/decorators/sensor_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/decorators/source_asset_decorator.py` & `dagster-1.7.3/dagster/_core/definitions/decorators/source_asset_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/definition_config_schema.py` & `dagster-1.7.3/dagster/_core/definitions/definition_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/definitions_class.py` & `dagster-1.7.3/dagster/_core/definitions/definitions_class.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/dependency.py` & `dagster-1.7.3/dagster/_core/definitions/dependency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/events.py` & `dagster-1.7.3/dagster/_core/definitions/events.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/executor_definition.py` & `dagster-1.7.3/dagster/_core/definitions/executor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/external_asset.py` & `dagster-1.7.3/dagster/_core/definitions/external_asset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/freshness_based_auto_materialize.py` & `dagster-1.7.3/dagster/_core/definitions/freshness_based_auto_materialize.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/freshness_checks/last_update.py` & `dagster-1.7.3/dagster/_core/definitions/freshness_checks/last_update.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/freshness_checks/shared_builder.py` & `dagster-1.7.3/dagster/_core/definitions/freshness_checks/shared_builder.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,46 @@
 import datetime
-from typing import Any, Callable, Iterable, Optional, Sequence, Union, cast
+from typing import Any, Callable, Dict, Iterable, Optional, Sequence, Union, cast
 
 import pendulum
 
 from dagster import _check as check
 from dagster._core.definitions.asset_check_result import AssetCheckResult
 from dagster._core.definitions.asset_check_spec import AssetCheckSeverity, AssetCheckSpec
 from dagster._core.definitions.asset_checks import AssetChecksDefinition
 from dagster._core.definitions.decorators.asset_check_decorator import (
     multi_asset_check,
 )
-from dagster._core.definitions.metadata import FloatMetadataValue, TimestampMetadataValue
+from dagster._core.definitions.metadata import (
+    FloatMetadataValue,
+    JsonMetadataValue,
+    MetadataValue,
+    TimestampMetadataValue,
+)
 from dagster._core.definitions.time_window_partitions import TimeWindowPartitionsDefinition
 from dagster._core.execution.context.compute import (
     AssetCheckExecutionContext,
 )
-from dagster._utils.schedules import get_latest_completed_cron_tick, is_valid_cron_string
+from dagster._utils.schedules import (
+    get_latest_completed_cron_tick,
+    get_next_cron_tick,
+    is_valid_cron_string,
+)
 
 from ..assets import AssetsDefinition, SourceAsset
 from ..events import AssetKey, CoercibleToAssetKey
 from .utils import (
-    DEADLINE_CRON_METADATA_KEY,
+    DEADLINE_CRON_PARAM_KEY,
+    EXPECTED_BY_TIMESTAMP_METADATA_KEY,
+    FRESH_UNTIL_METADATA_KEY,
     FRESHNESS_PARAMS_METADATA_KEY,
-    FRESHNESS_TIMEZONE_METADATA_KEY,
     LAST_UPDATED_TIMESTAMP_METADATA_KEY,
-    LOWER_BOUND_DELTA_METADATA_KEY,
-    OVERDUE_DEADLINE_TIMESTAMP_METADATA_KEY,
+    LOWER_BOUND_DELTA_PARAM_KEY,
     OVERDUE_SECONDS_METADATA_KEY,
+    TIMEZONE_PARAM_KEY,
     asset_to_keys_iterable,
     ensure_no_duplicate_assets,
     get_description_for_freshness_check_result,
     get_last_updated_timestamp,
     retrieve_latest_record,
     unique_id_from_asset_keys,
 )
@@ -40,19 +50,19 @@
     asset_keys: Sequence[AssetKey],
     deadline_cron: Optional[str],
     timezone: str,
     severity: AssetCheckSeverity,
     lower_bound_delta: Optional[datetime.timedelta],
     asset_property_enforcement_lambda: Optional[Callable[[AssetsDefinition], bool]],
 ) -> AssetChecksDefinition:
-    params_metadata: dict[str, Any] = {FRESHNESS_TIMEZONE_METADATA_KEY: timezone}
+    params_metadata: dict[str, Any] = {TIMEZONE_PARAM_KEY: timezone}
     if deadline_cron:
-        params_metadata[DEADLINE_CRON_METADATA_KEY] = deadline_cron
+        params_metadata[DEADLINE_CRON_PARAM_KEY] = deadline_cron
     if lower_bound_delta:
-        params_metadata[LOWER_BOUND_DELTA_METADATA_KEY] = lower_bound_delta.total_seconds()
+        params_metadata[LOWER_BOUND_DELTA_PARAM_KEY] = lower_bound_delta.total_seconds()
 
     @multi_asset_check(
         specs=[
             AssetCheckSpec(
                 "freshness_check",
                 asset=asset_key,
                 metadata={FRESHNESS_PARAMS_METADATA_KEY: params_metadata},
@@ -80,16 +90,20 @@
 
             check.invariant(
                 partitions_def is None
                 or isinstance(partitions_def, TimeWindowPartitionsDefinition),
                 "Expected partitions_def to be time-windowed.",
             )
             current_time_in_freshness_tz = pendulum.from_timestamp(current_timestamp, tz=timezone)
-            latest_completed_cron_tick = get_latest_completed_cron_tick(
-                deadline_cron, current_time_in_freshness_tz, timezone
+            latest_completed_cron_tick = (
+                get_latest_completed_cron_tick(
+                    deadline_cron, current_time_in_freshness_tz, timezone
+                )
+                if deadline_cron
+                else None
             )
             deadline = check.inst_param(
                 latest_completed_cron_tick or current_time_in_freshness_tz,
                 "deadline",
                 datetime.datetime,
             )
             if not partitions_def:
@@ -119,24 +133,46 @@
             )
             update_timestamp = get_last_updated_timestamp(latest_record, context)
             passed = (
                 update_timestamp is not None
                 and update_timestamp >= last_update_time_lower_bound.timestamp()
             )
 
-            metadata = {
-                FRESHNESS_PARAMS_METADATA_KEY: params_metadata,
-                OVERDUE_DEADLINE_TIMESTAMP_METADATA_KEY: TimestampMetadataValue(
-                    deadline.timestamp()
-                ),
+            metadata: Dict[str, MetadataValue] = {
+                FRESHNESS_PARAMS_METADATA_KEY: JsonMetadataValue(params_metadata),
             }
             if not passed:
                 metadata[OVERDUE_SECONDS_METADATA_KEY] = FloatMetadataValue(
                     current_timestamp - deadline.timestamp()
                 )
+                expected_by = (
+                    deadline.timestamp()
+                    if deadline_cron
+                    else update_timestamp + check.not_none(lower_bound_delta).total_seconds()
+                    if update_timestamp
+                    else None
+                )
+                if expected_by:
+                    metadata[EXPECTED_BY_TIMESTAMP_METADATA_KEY] = TimestampMetadataValue(
+                        expected_by
+                    )
+            else:
+                # If the asset is fresh, we can potentially determine when it has the possibility of becoming stale again.
+                # In the case of a deadline cron, this is the next cron tick after the current time.
+                # In the case of just a lower_bound_delta, this is the last update time plus the
+                # lower_bound_delta.
+                fresh_until = (
+                    check.not_none(
+                        get_next_cron_tick(deadline_cron, current_time_in_freshness_tz, timezone)
+                    ).timestamp()
+                    if deadline_cron
+                    else check.not_none(update_timestamp)
+                    + check.not_none(lower_bound_delta).total_seconds()
+                )
+                metadata[FRESH_UNTIL_METADATA_KEY] = TimestampMetadataValue(fresh_until)
             if update_timestamp:
                 metadata[LAST_UPDATED_TIMESTAMP_METADATA_KEY] = TimestampMetadataValue(
                     update_timestamp
                 )
 
             yield AssetCheckResult(
                 passed=passed,
```

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/freshness_checks/time_partition.py` & `dagster-1.7.3/dagster/_core/definitions/freshness_checks/time_partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/freshness_checks/utils.py` & `dagster-1.7.3/dagster/_core/definitions/freshness_checks/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,24 +9,32 @@
 from dagster._core.events import DagsterEventType
 from dagster._core.execution.context.compute import AssetCheckExecutionContext
 from dagster._core.instance import DagsterInstance
 
 from ..assets import AssetsDefinition, SourceAsset
 from ..events import AssetKey, CoercibleToAssetKey
 
+# Constants
 DEFAULT_FRESHNESS_SEVERITY = AssetCheckSeverity.WARN
 DEFAULT_FRESHNESS_TIMEZONE = "UTC"
-LOWER_BOUND_DELTA_METADATA_KEY = "dagster/lower_bound_delta"
-DEADLINE_CRON_METADATA_KEY = "dagster/deadline_cron"
-FRESHNESS_TIMEZONE_METADATA_KEY = "dagster/freshness_timezone"
+
+# Top-level metadata keys
 LAST_UPDATED_TIMESTAMP_METADATA_KEY = "dagster/last_updated_timestamp"
 FRESHNESS_PARAMS_METADATA_KEY = "dagster/freshness_params"
-OVERDUE_DEADLINE_TIMESTAMP_METADATA_KEY = "dagster/overdue_deadline_timestamp"
+# When an asset is overdue, this represents the timestamp by which the asset was expected to arrive.
+EXPECTED_BY_TIMESTAMP_METADATA_KEY = "dagster/expected_by_timestamp"
+# When an asset is fresh, this represents the timestamp when the asset can become stale again.
+FRESH_UNTIL_METADATA_KEY = "dagster/fresh_until_timestamp"
 OVERDUE_SECONDS_METADATA_KEY = "dagster/overdue_seconds"
 
+# dagster/freshness_params inner keys
+LOWER_BOUND_DELTA_PARAM_KEY = "lower_bound_delta"
+DEADLINE_CRON_PARAM_KEY = "deadline_cron"
+TIMEZONE_PARAM_KEY = "timezone"
+
 
 def ensure_no_duplicate_assets(
     assets: Sequence[Union[CoercibleToAssetKey, AssetsDefinition, SourceAsset]],
 ) -> None:
     """Finds duplicate assets in the provided list of assets, and errors if any are present.
 
     Args:
@@ -155,23 +163,14 @@
                 "assets which have freshness checks."
             )
             return None
     else:
         check.failed("Expected record to be an observation or materialization")
 
 
-def ensure_freshness_checks(checks: Sequence[AssetChecksDefinition]) -> None:
-    for check_def in checks:
-        for check_spec in check_def.check_specs:
-            check.invariant(
-                check_spec.metadata and check_spec.metadata.get(FRESHNESS_PARAMS_METADATA_KEY),
-                f"Asset check {check_spec.key} didn't have expected metadata. Please ensure that the asset check is a freshness check.",
-            )
-
-
 def get_description_for_freshness_check_result(
     passed: bool,
     update_timestamp: Optional[float],
     last_update_time_lower_bound: datetime.datetime,
     current_timestamp: float,
     expected_partition_key: Optional[str],
     record_arrival_timestamp: Optional[float],
```

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/freshness_policy.py` & `dagster-1.7.3/dagster/_core/definitions/freshness_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/freshness_policy_sensor_definition.py` & `dagster-1.7.3/dagster/_core/definitions/freshness_policy_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/graph_definition.py` & `dagster-1.7.3/dagster/_core/definitions/graph_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/hook_definition.py` & `dagster-1.7.3/dagster/_core/definitions/hook_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/hook_invocation.py` & `dagster-1.7.3/dagster/_core/definitions/hook_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/inference.py` & `dagster-1.7.3/dagster/_core/definitions/inference.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/input.py` & `dagster-1.7.3/dagster/_core/definitions/input.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/instigation_logger.py` & `dagster-1.7.3/dagster/_core/definitions/instigation_logger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/job_base.py` & `dagster-1.7.3/dagster/_core/definitions/job_base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/job_definition.py` & `dagster-1.7.3/dagster/_core/definitions/job_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/load_asset_checks_from_modules.py` & `dagster-1.7.3/dagster/_core/definitions/load_asset_checks_from_modules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/load_assets_from_modules.py` & `dagster-1.7.3/dagster/_core/definitions/load_assets_from_modules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/logger_definition.py` & `dagster-1.7.3/dagster/_core/definitions/logger_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/logger_invocation.py` & `dagster-1.7.3/dagster/_core/definitions/logger_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/materialize.py` & `dagster-1.7.3/dagster/_core/definitions/materialize.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/metadata/__init__.py` & `dagster-1.7.3/dagster/_core/definitions/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/metadata/table.py` & `dagster-1.7.3/dagster/_core/definitions/metadata/table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/multi_asset_sensor_definition.py` & `dagster-1.7.3/dagster/_core/definitions/multi_asset_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/multi_dimensional_partitions.py` & `dagster-1.7.3/dagster/_core/definitions/multi_dimensional_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/node_container.py` & `dagster-1.7.3/dagster/_core/definitions/node_container.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/node_definition.py` & `dagster-1.7.3/dagster/_core/definitions/node_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/observe.py` & `dagster-1.7.3/dagster/_core/definitions/observe.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/op_definition.py` & `dagster-1.7.3/dagster/_core/definitions/op_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/op_invocation.py` & `dagster-1.7.3/dagster/_core/definitions/op_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/op_selection.py` & `dagster-1.7.3/dagster/_core/definitions/op_selection.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/output.py` & `dagster-1.7.3/dagster/_core/definitions/output.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/partition.py` & `dagster-1.7.3/dagster/_core/definitions/partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/partition_key_range.py` & `dagster-1.7.3/dagster/_core/definitions/partition_key_range.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/partition_mapping.py` & `dagster-1.7.3/dagster/_core/definitions/partition_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/partitioned_schedule.py` & `dagster-1.7.3/dagster/_core/definitions/partitioned_schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/policy.py` & `dagster-1.7.3/dagster/_core/definitions/policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/reconstruct.py` & `dagster-1.7.3/dagster/_core/definitions/reconstruct.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/remote_asset_graph.py` & `dagster-1.7.3/dagster/_core/definitions/remote_asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/repository_definition/__init__.py` & `dagster-1.7.3/dagster/_core/definitions/repository_definition/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/repository_definition/caching_index.py` & `dagster-1.7.3/dagster/_core/definitions/repository_definition/caching_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/repository_definition/repository_data.py` & `dagster-1.7.3/dagster/_core/definitions/repository_definition/repository_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/repository_definition/repository_data_builder.py` & `dagster-1.7.3/dagster/_core/definitions/repository_definition/repository_data_builder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/repository_definition/repository_definition.py` & `dagster-1.7.3/dagster/_core/definitions/repository_definition/repository_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/repository_definition/valid_definitions.py` & `dagster-1.7.3/dagster/_core/definitions/repository_definition/valid_definitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/resolved_asset_deps.py` & `dagster-1.7.3/dagster/_core/definitions/resolved_asset_deps.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/resource_annotation.py` & `dagster-1.7.3/dagster/_core/definitions/resource_annotation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/resource_definition.py` & `dagster-1.7.3/dagster/_core/definitions/resource_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/resource_invocation.py` & `dagster-1.7.3/dagster/_core/definitions/resource_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/resource_requirement.py` & `dagster-1.7.3/dagster/_core/definitions/resource_requirement.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/result.py` & `dagster-1.7.3/dagster/_core/definitions/result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/run_config.py` & `dagster-1.7.3/dagster/_core/definitions/run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/run_config_schema.py` & `dagster-1.7.3/dagster/_core/definitions/run_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/run_request.py` & `dagster-1.7.3/dagster/_core/definitions/run_request.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/run_status_sensor_definition.py` & `dagster-1.7.3/dagster/_core/definitions/run_status_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/schedule_definition.py` & `dagster-1.7.3/dagster/_core/definitions/schedule_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/schema_change_checks.py` & `dagster-1.7.3/dagster/_core/definitions/schema_change_checks.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/scoped_resources_builder.py` & `dagster-1.7.3/dagster/_core/definitions/scoped_resources_builder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/selector.py` & `dagster-1.7.3/dagster/_core/definitions/selector.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/sensor_definition.py` & `dagster-1.7.3/dagster/_core/definitions/sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/source_asset.py` & `dagster-1.7.3/dagster/_core/definitions/source_asset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/step_launcher.py` & `dagster-1.7.3/dagster/_core/definitions/step_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/target.py` & `dagster-1.7.3/dagster/_core/definitions/target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/time_window_partition_mapping.py` & `dagster-1.7.3/dagster/_core/definitions/time_window_partition_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/time_window_partitions.py` & `dagster-1.7.3/dagster/_core/definitions/time_window_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/unresolved_asset_job_definition.py` & `dagster-1.7.3/dagster/_core/definitions/unresolved_asset_job_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/utils.py` & `dagster-1.7.3/dagster/_core/definitions/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/definitions/version_strategy.py` & `dagster-1.7.3/dagster/_core/definitions/version_strategy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/errors.py` & `dagster-1.7.3/dagster/_core/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -682,11 +682,7 @@
     """Indicates that a stored value can't be deserialized because the definition needed to interpret
     it has changed.
     """
 
 
 class DagsterPipesExecutionError(DagsterError):
     """Indicates that an error occurred during the execution of an external process."""
-
-
-class DagsterImportClassFromCodePointerError(DagsterError):
-    """Indicates that an error occurred while importing a class from a code pointer."""
```

### Comparing `dagster-1.7.2rc4/dagster/_core/event_api.py` & `dagster-1.7.3/dagster/_core/event_api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/events/__init__.py` & `dagster-1.7.3/dagster/_core/events/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/events/log.py` & `dagster-1.7.3/dagster/_core/events/log.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Callable, Mapping, NamedTuple, Optional, Union
 
 import dagster._check as check
 from dagster._annotations import PublicAttr, public
+from dagster._core.definitions.asset_check_evaluation import AssetCheckEvaluation
 from dagster._core.definitions.events import AssetMaterialization, AssetObservation
 from dagster._core.definitions.logger_definition import LoggerDefinition
 from dagster._core.events import DagsterEvent, DagsterEventType
 from dagster._core.utils import coerce_valid_log_level
 from dagster._serdes.serdes import (
     deserialize_value,
     serialize_value,
@@ -152,14 +153,26 @@
             observation = self.dagster_event.asset_observation_data.asset_observation
             if isinstance(observation, AssetObservation):
                 return observation
 
         return None
 
     @property
+    def asset_check_evaluation(self) -> Optional[AssetCheckEvaluation]:
+        if (
+            self.dagster_event
+            and self.dagster_event.event_type_value == DagsterEventType.ASSET_CHECK_EVALUATION
+        ):
+            evaluation = self.dagster_event.asset_check_evaluation_data
+            if isinstance(evaluation, AssetCheckEvaluation):
+                return evaluation
+
+        return None
+
+    @property
     def tags(self) -> Optional[Mapping[str, str]]:
         materialization = self.asset_materialization
         if materialization:
             return materialization.tags
 
         observation = self.asset_observation
         if observation:
```

### Comparing `dagster-1.7.2rc4/dagster/_core/events/utils.py` & `dagster-1.7.3/dagster/_core/events/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/api.py` & `dagster-1.7.3/dagster/_core/execution/api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/asset_backfill.py` & `dagster-1.7.3/dagster/_core/execution/asset_backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/backfill.py` & `dagster-1.7.3/dagster/_core/execution/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/build_resources.py` & `dagster-1.7.3/dagster/_core/execution/build_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/compute_logs.py` & `dagster-1.7.3/dagster/_core/execution/compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/context/compute.py` & `dagster-1.7.3/dagster/_core/execution/context/compute.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/context/hook.py` & `dagster-1.7.3/dagster/_core/execution/context/hook.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/context/init.py` & `dagster-1.7.3/dagster/_core/execution/context/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/context/input.py` & `dagster-1.7.3/dagster/_core/execution/context/input.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/context/invocation.py` & `dagster-1.7.3/dagster/_core/execution/context/invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/context/logger.py` & `dagster-1.7.3/dagster/_core/execution/context/logger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/context/output.py` & `dagster-1.7.3/dagster/_core/execution/context/output.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/context/system.py` & `dagster-1.7.3/dagster/_core/execution/context/system.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/context_creation_job.py` & `dagster-1.7.3/dagster/_core/execution/context_creation_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/execute_in_process.py` & `dagster-1.7.3/dagster/_core/execution/execute_in_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/execute_in_process_result.py` & `dagster-1.7.3/dagster/_core/execution/execute_in_process_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/execution_result.py` & `dagster-1.7.3/dagster/_core/execution/execution_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/host_mode.py` & `dagster-1.7.3/dagster/_core/execution/host_mode.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/job_backfill.py` & `dagster-1.7.3/dagster/_core/execution/job_backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/job_execution_result.py` & `dagster-1.7.3/dagster/_core/execution/job_execution_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/memoization.py` & `dagster-1.7.3/dagster/_core/execution/memoization.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/plan/active.py` & `dagster-1.7.3/dagster/_core/execution/plan/active.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/plan/compute.py` & `dagster-1.7.3/dagster/_core/execution/plan/compute.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/plan/compute_generator.py` & `dagster-1.7.3/dagster/_core/execution/plan/compute_generator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/plan/execute_plan.py` & `dagster-1.7.3/dagster/_core/execution/plan/execute_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/plan/execute_step.py` & `dagster-1.7.3/dagster/_core/execution/plan/execute_step.py`

 * *Files 0% similar despite different names*

```diff
@@ -467,52 +467,54 @@
     check.inst_param(step_context, "step_context", StepExecutionContext)
 
     if step_context.previous_attempt_count > 0:
         yield DagsterEvent.step_restarted_event(step_context, step_context.previous_attempt_count)
     else:
         yield DagsterEvent.step_start_event(step_context)
 
-    inputs = {}
-
-    if step_context.is_sda_step:
-        step_context.fetch_external_input_asset_version_info()
-
-    for step_input in step_context.step.step_inputs:
-        input_def = step_context.op_def.input_def_named(step_input.name)
-        dagster_type = input_def.dagster_type
-
-        if dagster_type.is_nothing:
-            continue
-
-        for event_or_input_value in step_input.source.load_input_object(step_context, input_def):
-            if isinstance(event_or_input_value, DagsterEvent):
-                yield event_or_input_value
-            else:
-                check.invariant(step_input.name not in inputs)
-                inputs[step_input.name] = event_or_input_value
-
-    for input_name, input_value in inputs.items():
-        for evt in check.generator(
-            _type_checked_event_sequence_for_input(step_context, input_name, input_value)
-        ):
-            yield evt
-
-    # The core execution loop expects a compute generator in a specific format: a generator that
-    # takes a context and dictionary of inputs as input, yields output events. If an op definition
-    # was generated from the @op decorator, then compute_fn needs to be coerced
-    # into this format. If the op definition was created directly, then it is expected that the
-    # compute_fn is already in this format.
-    if isinstance(step_context.op_def.compute_fn, DecoratedOpFunction):
-        core_gen = create_op_compute_wrapper(step_context.op_def)
-    else:
-        core_gen = step_context.op_def.compute_fn
-
     with time_execution_scope() as timer_result, enter_execution_context(
         step_context
     ) as compute_context:
+        inputs = {}
+
+        if step_context.is_sda_step:
+            step_context.fetch_external_input_asset_version_info()
+
+        for step_input in step_context.step.step_inputs:
+            input_def = step_context.op_def.input_def_named(step_input.name)
+            dagster_type = input_def.dagster_type
+
+            if dagster_type.is_nothing:
+                continue
+
+            for event_or_input_value in step_input.source.load_input_object(
+                step_context, input_def
+            ):
+                if isinstance(event_or_input_value, DagsterEvent):
+                    yield event_or_input_value
+                else:
+                    check.invariant(step_input.name not in inputs)
+                    inputs[step_input.name] = event_or_input_value
+
+        for input_name, input_value in inputs.items():
+            for evt in check.generator(
+                _type_checked_event_sequence_for_input(step_context, input_name, input_value)
+            ):
+                yield evt
+
+        # The core execution loop expects a compute generator in a specific format: a generator that
+        # takes a context and dictionary of inputs as input, yields output events. If an op definition
+        # was generated from the @op decorator, then compute_fn needs to be coerced
+        # into this format. If the op definition was created directly, then it is expected that the
+        # compute_fn is already in this format.
+        if isinstance(step_context.op_def.compute_fn, DecoratedOpFunction):
+            core_gen = create_op_compute_wrapper(step_context.op_def)
+        else:
+            core_gen = step_context.op_def.compute_fn
+
         user_event_sequence = execute_core_compute(
             step_context,
             inputs,
             core_gen,
             compute_context,
         )
```

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/plan/external_step.py` & `dagster-1.7.3/dagster/_core/execution/plan/external_step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/plan/handle.py` & `dagster-1.7.3/dagster/_core/execution/plan/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/plan/inputs.py` & `dagster-1.7.3/dagster/_core/execution/plan/inputs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/plan/instance_concurrency_context.py` & `dagster-1.7.3/dagster/_core/execution/plan/instance_concurrency_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/plan/local_external_step_main.py` & `dagster-1.7.3/dagster/_core/execution/plan/local_external_step_main.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/plan/objects.py` & `dagster-1.7.3/dagster/_core/execution/plan/objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/plan/outputs.py` & `dagster-1.7.3/dagster/_core/execution/plan/outputs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/plan/plan.py` & `dagster-1.7.3/dagster/_core/execution/plan/plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/plan/state.py` & `dagster-1.7.3/dagster/_core/execution/plan/state.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/plan/step.py` & `dagster-1.7.3/dagster/_core/execution/plan/step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/plan/utils.py` & `dagster-1.7.3/dagster/_core/execution/plan/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/poll_compute_logs.py` & `dagster-1.7.3/dagster/_core/execution/poll_compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/resolve_versions.py` & `dagster-1.7.3/dagster/_core/execution/resolve_versions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/resources_init.py` & `dagster-1.7.3/dagster/_core/execution/resources_init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/retries.py` & `dagster-1.7.3/dagster/_core/execution/retries.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/run_cancellation_thread.py` & `dagster-1.7.3/dagster/_core/execution/run_cancellation_thread.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/stats.py` & `dagster-1.7.3/dagster/_core/execution/stats.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/submit_asset_runs.py` & `dagster-1.7.3/dagster/_core/execution/submit_asset_runs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/tags.py` & `dagster-1.7.3/dagster/_core/execution/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/validate_run_config.py` & `dagster-1.7.3/dagster/_core/execution/validate_run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/watch_orphans.py` & `dagster-1.7.3/dagster/_core/execution/watch_orphans.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/execution/with_resources.py` & `dagster-1.7.3/dagster/_core/execution/with_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/executor/base.py` & `dagster-1.7.3/dagster/_core/executor/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/executor/child_process_executor.py` & `dagster-1.7.3/dagster/_core/executor/child_process_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/executor/in_process.py` & `dagster-1.7.3/dagster/_core/executor/in_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/executor/init.py` & `dagster-1.7.3/dagster/_core/executor/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/executor/multiprocess.py` & `dagster-1.7.3/dagster/_core/executor/multiprocess.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/executor/step_delegating/step_delegating_executor.py` & `dagster-1.7.3/dagster/_core/executor/step_delegating/step_delegating_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/executor/step_delegating/step_handler/base.py` & `dagster-1.7.3/dagster/_core/executor/step_delegating/step_handler/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/instance/__init__.py` & `dagster-1.7.3/dagster/_core/instance/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,14 @@
     PARENT_RUN_ID_TAG,
     PARTITION_NAME_TAG,
     RESUME_RETRY_TAG,
     ROOT_RUN_ID_TAG,
     RUN_FAILURE_REASON_TAG,
 )
 from dagster._serdes import ConfigurableClass
-from dagster._serdes.config_class import ConfigurableClassData
 from dagster._seven import get_current_datetime_in_utc
 from dagster._utils import PrintFn, is_uuid, traced
 from dagster._utils.error import serializable_error_info_from_exc_info
 from dagster._utils.merger import merge_dicts
 from dagster._utils.warnings import (
     deprecation_warning,
     experimental_warning,
@@ -153,15 +152,18 @@
     from dagster._core.secrets import SecretsLoader
     from dagster._core.snap import (
         ExecutionPlanSnapshot,
         ExecutionStepOutputSnap,
         ExecutionStepSnap,
         JobSnapshot,
     )
-    from dagster._core.storage.asset_check_execution_record import AssetCheckInstanceSupport
+    from dagster._core.storage.asset_check_execution_record import (
+        AssetCheckExecutionRecord,
+        AssetCheckInstanceSupport,
+    )
     from dagster._core.storage.compute_log_manager import ComputeLogManager
     from dagster._core.storage.daemon_cursor import DaemonCursorStorage
     from dagster._core.storage.event_log import EventLogStorage
     from dagster._core.storage.event_log.base import (
         AssetRecord,
         EventLogConnection,
         EventLogRecord,
@@ -475,26 +477,14 @@
 
         self._secrets_loader = check.opt_inst_param(secrets_loader, "secrets_loader", SecretsLoader)
 
         if self._secrets_loader:
             self._secrets_loader.register_instance(self)
 
         self._ref = check.opt_inst_param(ref, "ref", InstanceRef)
-        # Fetch backcompat version of instance ref that points to the dagster_cloud
-        # module to ensure compatibility with older versions of agent/user code.
-        if ref and ref.custom_instance_class_data:
-            module_elems = ref.custom_instance_class_data.module_name.split(".")
-            if "dagster_plus" == module_elems[0]:
-                self._ref = ref._replace(
-                    custom_instance_class_data=ConfigurableClassData(
-                        module_name=".".join(["dagster_cloud", *module_elems[1:]]),
-                        class_name=ref.custom_instance_class_data.class_name,
-                        config_yaml=ref.custom_instance_class_data.config_yaml,
-                    )
-                )
 
         self._subscribers: Dict[str, List[Callable]] = defaultdict(list)
 
         run_monitoring_enabled = self.run_monitoring_settings.get("enabled", False)
         self._run_monitoring_enabled = run_monitoring_enabled
         if self.run_monitoring_enabled and self.run_monitoring_max_resume_run_attempts:
             check.invariant(
@@ -972,14 +962,18 @@
     def auto_materialize_use_sensors(self) -> int:
         return self.get_settings("auto_materialize").get("use_sensors", False)
 
     @property
     def global_op_concurrency_default_limit(self) -> Optional[int]:
         return self.get_settings("concurrency").get("default_op_concurrency_limit")
 
+    @property
+    def use_transitive_stale_causes(self) -> bool:
+        return True
+
     # python logs
 
     @property
     def managed_python_loggers(self) -> Sequence[str]:
         python_log_settings = self.get_settings("python_logs") or {}
         loggers: Sequence[str] = python_log_settings.get("managed_python_loggers", [])
         return loggers
@@ -1999,14 +1993,22 @@
 
         Returns:
             Optional[AssetMaterialization]: The latest materialization event for the given asset
                 key, or `None` if the asset has not been materialized.
         """
         return self._event_storage.get_latest_materialization_events([asset_key]).get(asset_key)
 
+    @traced
+    def get_latest_asset_check_evaluation_record(
+        self, asset_check_key: "AssetCheckKey"
+    ) -> Optional["AssetCheckExecutionRecord"]:
+        return self._event_storage.get_latest_asset_check_execution_by_key([asset_check_key]).get(
+            asset_check_key
+        )
+
     @public
     @traced
     def get_event_records(
         self,
         event_records_filter: "EventRecordsFilter",
         limit: Optional[int] = None,
         ascending: bool = False,
```

### Comparing `dagster-1.7.2rc4/dagster/_core/instance/config.py` & `dagster-1.7.3/dagster/_core/instance/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import importlib.util
 import logging
 import os
 from typing import TYPE_CHECKING, Any, Mapping, Optional, Tuple, Type, cast
 
 from dagster import (
     Array,
     Bool,
@@ -14,15 +13,15 @@
     Permissive,
     ScalarUnion,
     Selector,
     StringSource,
     validate_config,
 )
 from dagster._config.source import BoolSource
-from dagster._core.errors import DagsterImportClassFromCodePointerError, DagsterInvalidConfigError
+from dagster._core.errors import DagsterInvalidConfigError
 from dagster._core.storage.config import mysql_config, pg_config
 from dagster._serdes import class_from_code_pointer
 from dagster._utils.concurrency import get_max_concurrency_limit_value
 from dagster._utils.merger import merge_dicts
 from dagster._utils.yaml_utils import load_yaml_from_globs
 
 if TYPE_CHECKING:
@@ -33,41 +32,14 @@
 DAGSTER_CONFIG_YAML_FILENAME = "dagster.yaml"
 
 
 def is_dagster_home_set() -> bool:
     return bool(os.getenv("DAGSTER_HOME"))
 
 
-def dagster_instance_class_from_code_pointer(
-    module_name: str, class_name: str
-) -> Type["DagsterInstance"]:
-    module_elems = module_name.split(".")
-    # When attempting to rehydrate a configurable class, attempt to load from dagster_plus
-    # instead of dagster_cloud if the dagster_plus package exists
-    if "dagster_cloud" == module_elems[0] and importlib.util.find_spec("dagster_plus") is not None:
-        try:
-            return cast(
-                Type["DagsterInstance"],
-                class_from_code_pointer(
-                    ".".join(["dagster_plus", *module_elems[1:]]),
-                    class_name,
-                ),
-            )
-        except DagsterImportClassFromCodePointerError:
-            logger = logging.getLogger("dagster")
-            logger.exception("Error importing DagsterInstance class from dagster_plus module")
-
-    # If the module is not in dagster_plus, or if the dagster_plus package does not exist,
-    # load it from the original module
-    return cast(
-        Type["DagsterInstance"],
-        class_from_code_pointer(module_name, class_name),
-    )
-
-
 def dagster_instance_config(
     base_dir: str,
     config_filename: str = DAGSTER_CONFIG_YAML_FILENAME,
     overrides: Optional[Mapping[str, object]] = None,
 ) -> Tuple[Mapping[str, Any], Optional[Type["DagsterInstance"]]]:
     check.str_param(base_dir, "base_dir")
     check.invariant(os.path.isdir(base_dir), "base_dir should be a directory")
@@ -94,16 +66,19 @@
         if not validate_custom_config.success:
             raise DagsterInvalidConfigError(
                 f"Errors whilst loading dagster custom class config at {config_filename}",
                 validate_custom_config.errors,
                 custom_instance_class_data,
             )
 
-        custom_instance_class = dagster_instance_class_from_code_pointer(
-            custom_instance_class_data["module"], custom_instance_class_data["class"]
+        custom_instance_class = cast(
+            Type["DagsterInstance"],
+            class_from_code_pointer(
+                custom_instance_class_data["module"], custom_instance_class_data["class"]
+            ),
         )
 
         schema: Mapping[str, Field]
         if hasattr(custom_instance_class, "config_schema"):
             schema = merge_dicts(
                 dagster_instance_config_schema(),
                 custom_instance_class.config_schema(),  # type: ignore
```

### Comparing `dagster-1.7.2rc4/dagster/_core/instance/ref.py` & `dagster-1.7.3/dagster/_core/instance/ref.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,16 @@
 import os
 from typing import TYPE_CHECKING, Any, Mapping, NamedTuple, Optional, Sequence, Type
 
 import yaml
 
 import dagster._check as check
-from dagster._serdes import (
-    ConfigurableClassData,
-    whitelist_for_serdes,
-)
-
-from .config import (
-    DAGSTER_CONFIG_YAML_FILENAME,
-    dagster_instance_class_from_code_pointer,
-    dagster_instance_config,
-)
+from dagster._serdes import ConfigurableClassData, class_from_code_pointer, whitelist_for_serdes
+
+from .config import DAGSTER_CONFIG_YAML_FILENAME, dagster_instance_config
 
 if TYPE_CHECKING:
     from dagster._core.instance import DagsterInstance, DagsterInstanceOverrides
     from dagster._core.launcher.base import RunLauncher
     from dagster._core.run_coordinator.base import RunCoordinator
     from dagster._core.scheduler.scheduler import Scheduler
     from dagster._core.secrets.loader import SecretsLoader
@@ -576,22 +569,22 @@
             self.secrets_loader_data.rehydrate(as_type=SecretsLoader)
             if self.secrets_loader_data
             else None
         )
 
     @property
     def custom_instance_class(self) -> Type["DagsterInstance"]:
-        return (
-            dagster_instance_class_from_code_pointer(
+        return (  # type: ignore  # (ambiguous return type)
+            class_from_code_pointer(
                 self.custom_instance_class_data.module_name,
                 self.custom_instance_class_data.class_name,
             )
             if self.custom_instance_class_data
             else None
-        )  # type: ignore
+        )
 
     @property
     def custom_instance_class_config(self) -> Mapping[str, Any]:
         return (
             self.custom_instance_class_data.config_dict if self.custom_instance_class_data else {}
         )
```

### Comparing `dagster-1.7.2rc4/dagster/_core/instance_for_test.py` & `dagster-1.7.3/dagster/_core/instance_for_test.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/launcher/base.py` & `dagster-1.7.3/dagster/_core/launcher/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/launcher/default_run_launcher.py` & `dagster-1.7.3/dagster/_core/launcher/default_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/launcher/sync_in_memory_run_launcher.py` & `dagster-1.7.3/dagster/_core/launcher/sync_in_memory_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/log_manager.py` & `dagster-1.7.3/dagster/_core/log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/nux.py` & `dagster-1.7.3/dagster/_core/nux.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/op_concurrency_limits_counter.py` & `dagster-1.7.3/dagster/_core/op_concurrency_limits_counter.py`

 * *Files 7% similar despite different names*

```diff
@@ -123,13 +123,34 @@
             if available_count > -1 * self._slot_count_offset:
                 # there exists a root concurrency key that is not blocked, we should dequeue
                 return False
 
         # if we reached here, then every root concurrency key is blocked, so we should not dequeue
         return True
 
+    def get_blocked_run_debug_info(self, run: DagsterRun) -> Mapping:
+        if not run.run_op_concurrency:
+            return {}
+
+        log_info = {}
+        for concurrency_key in run.run_op_concurrency.root_key_counts.keys():
+            concurrency_info = self._concurrency_info_by_key.get(concurrency_key)
+            if not concurrency_info:
+                continue
+
+            log_info[concurrency_key] = {
+                "slot_count": concurrency_info.slot_count,
+                "pending_step_count": len(concurrency_info.pending_steps),
+                "pending_step_run_ids": list(
+                    {step.run_id for step in concurrency_info.pending_steps}
+                ),
+                "launched_count": self._launched_concurrency_key_counts[concurrency_key],
+                "in_progress_count": self._in_progress_concurrency_key_counts[concurrency_key],
+            }
+        return log_info
+
     def update_counters_with_launched_item(self, run: DagsterRun):
         if not run.run_op_concurrency:
             return
         for concurrency_key, count in run.run_op_concurrency.root_key_counts.items():
             if concurrency_key:
                 self._launched_concurrency_key_counts[concurrency_key] += count
```

### Comparing `dagster-1.7.2rc4/dagster/_core/origin.py` & `dagster-1.7.3/dagster/_core/origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/pipes/client.py` & `dagster-1.7.3/dagster/_core/pipes/client.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/pipes/context.py` & `dagster-1.7.3/dagster/_core/pipes/context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/pipes/subprocess.py` & `dagster-1.7.3/dagster/_core/pipes/subprocess.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/pipes/utils.py` & `dagster-1.7.3/dagster/_core/pipes/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/remote_representation/__init__.py` & `dagster-1.7.3/dagster/_core/remote_representation/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/remote_representation/code_location.py` & `dagster-1.7.3/dagster/_core/remote_representation/code_location.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/remote_representation/external.py` & `dagster-1.7.3/dagster/_core/remote_representation/external.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/remote_representation/external_data.py` & `dagster-1.7.3/dagster/_core/remote_representation/external_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1741,15 +1741,17 @@
             required_top_level_resources = []
 
         # Partition mappings are only exposed on the ExternalAssetNode if at least one asset is
         # partitioned and the partition mapping is one of the builtin types.
         partition_mappings: Dict[AssetKey, Optional[PartitionMapping]] = {}
         builtin_partition_mapping_types = get_builtin_partition_mapping_types()
         for pk in asset_node.parent_keys:
-            partition_mapping = asset_graph.get_partition_mapping(key, pk)
+            # directly access the partition mapping to avoid the inference step of
+            # get_partition_mapping, as we want to defer the inference to the global RemoteAssetGraph
+            partition_mapping = asset_graph.get(key).partition_mappings.get(pk)
             if (asset_node.partitions_def or asset_graph.get(pk).partitions_def) and isinstance(
                 partition_mapping, builtin_partition_mapping_types
             ):
                 partition_mappings[pk] = partition_mapping
 
         external_asset_nodes.append(
             ExternalAssetNode(
```

### Comparing `dagster-1.7.2rc4/dagster/_core/remote_representation/feature_flags.py` & `dagster-1.7.3/dagster/_core/remote_representation/feature_flags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/remote_representation/grpc_server_registry.py` & `dagster-1.7.3/dagster/_core/remote_representation/grpc_server_registry.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/remote_representation/grpc_server_state_subscriber.py` & `dagster-1.7.3/dagster/_core/remote_representation/grpc_server_state_subscriber.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/remote_representation/handle.py` & `dagster-1.7.3/dagster/_core/remote_representation/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/remote_representation/historical.py` & `dagster-1.7.3/dagster/_core/remote_representation/historical.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/remote_representation/job_index.py` & `dagster-1.7.3/dagster/_core/remote_representation/job_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/remote_representation/origin.py` & `dagster-1.7.3/dagster/_core/remote_representation/origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/remote_representation/represented.py` & `dagster-1.7.3/dagster/_core/remote_representation/represented.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/run_coordinator/base.py` & `dagster-1.7.3/dagster/_core/run_coordinator/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/run_coordinator/default_run_coordinator.py` & `dagster-1.7.3/dagster/_core/run_coordinator/default_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/run_coordinator/queued_run_coordinator.py` & `dagster-1.7.3/dagster/_core/run_coordinator/queued_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/scheduler/__init__.py` & `dagster-1.7.3/dagster/_core/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/scheduler/execution.py` & `dagster-1.7.3/dagster/_core/scheduler/execution.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/scheduler/instigation.py` & `dagster-1.7.3/dagster/_core/scheduler/instigation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/scheduler/scheduler.py` & `dagster-1.7.3/dagster/_core/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/secrets/env_file.py` & `dagster-1.7.3/dagster/_core/secrets/env_file.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/selector/subset_selector.py` & `dagster-1.7.3/dagster/_core/selector/subset_selector.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/snap/__init__.py` & `dagster-1.7.3/dagster/_core/snap/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/snap/dagster_types.py` & `dagster-1.7.3/dagster/_core/snap/dagster_types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/snap/dep_snapshot.py` & `dagster-1.7.3/dagster/_core/snap/dep_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/snap/execution_plan_snapshot.py` & `dagster-1.7.3/dagster/_core/snap/execution_plan_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/snap/job_snapshot.py` & `dagster-1.7.3/dagster/_core/snap/job_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/snap/mode.py` & `dagster-1.7.3/dagster/_core/snap/mode.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/snap/node.py` & `dagster-1.7.3/dagster/_core/snap/node.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/snap/snap_to_yaml.py` & `dagster-1.7.3/dagster/_core/snap/snap_to_yaml.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/DEVELOPING.md` & `dagster-1.7.3/dagster/_core/storage/DEVELOPING.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/README.md` & `dagster-1.7.3/dagster/_core/storage/alembic/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/env.py` & `dagster-1.7.3/dagster/_core/storage/alembic/env.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/001_initial_1.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/001_initial_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/031_add_kvs_table.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/031_add_kvs_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/041_add_asset_check_executions_table.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/041_add_asset_check_executions_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/alembic/versions/042_46b412388816_add_concurrency_limits_table.py` & `dagster-1.7.3/dagster/_core/storage/alembic/versions/042_46b412388816_add_concurrency_limits_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/asset_check_execution_record.py` & `dagster-1.7.3/dagster/_core/storage/asset_check_execution_record.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/asset_value_loader.py` & `dagster-1.7.3/dagster/_core/storage/asset_value_loader.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/base_storage.py` & `dagster-1.7.3/dagster/_core/storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/branching/branching_io_manager.py` & `dagster-1.7.3/dagster/_core/storage/branching/branching_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/captured_log_manager.py` & `dagster-1.7.3/dagster/_core/storage/captured_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/cloud_storage_compute_log_manager.py` & `dagster-1.7.3/dagster/_core/storage/cloud_storage_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/compute_log_manager.py` & `dagster-1.7.3/dagster/_core/storage/compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/config.py` & `dagster-1.7.3/dagster/_core/storage/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/dagster_run.py` & `dagster-1.7.3/dagster/_core/storage/dagster_run.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/db_io_manager.py` & `dagster-1.7.3/dagster/_core/storage/db_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/event_log/__init__.py` & `dagster-1.7.3/dagster/_core/storage/event_log/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/event_log/base.py` & `dagster-1.7.3/dagster/_core/storage/event_log/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,14 +93,20 @@
     @property
     def last_materialization(self) -> Optional["EventLogEntry"]:
         if self.last_materialization_record is None:
             return None
         return self.last_materialization_record.event_log_entry
 
     @property
+    def last_observation(self) -> Optional["EventLogEntry"]:
+        if self.last_observation_record is None:
+            return None
+        return self.last_observation_record.event_log_entry
+
+    @property
     def last_materialization_storage_id(self) -> Optional[int]:
         if self.last_materialization_record is None:
             return None
         return self.last_materialization_record.storage_id
 
 
 class AssetRecord(NamedTuple):
```

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/event_log/in_memory.py` & `dagster-1.7.3/dagster/_core/storage/event_log/in_memory.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/event_log/migration.py` & `dagster-1.7.3/dagster/_core/storage/event_log/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/event_log/polling_event_watcher.py` & `dagster-1.7.3/dagster/_core/storage/event_log/polling_event_watcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/event_log/schema.py` & `dagster-1.7.3/dagster/_core/storage/event_log/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/event_log/sql_event_log.py` & `dagster-1.7.3/dagster/_core/storage/event_log/sql_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini` & `dagster-1.7.3/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py` & `dagster-1.7.3/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py` & `dagster-1.7.3/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/file_manager.py` & `dagster-1.7.3/dagster/_core/storage/file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/fs_io_manager.py` & `dagster-1.7.3/dagster/_core/storage/fs_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/input_manager.py` & `dagster-1.7.3/dagster/_core/storage/input_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/io_manager.py` & `dagster-1.7.3/dagster/_core/storage/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/legacy_storage.py` & `dagster-1.7.3/dagster/_core/storage/legacy_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/local_compute_log_manager.py` & `dagster-1.7.3/dagster/_core/storage/local_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/mem_io_manager.py` & `dagster-1.7.3/dagster/_core/storage/mem_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/memoizable_io_manager.py` & `dagster-1.7.3/dagster/_core/storage/memoizable_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/migration/bigint_migration.py` & `dagster-1.7.3/dagster/_core/storage/migration/bigint_migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/migration/utils.py` & `dagster-1.7.3/dagster/_core/storage/migration/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/noop_compute_log_manager.py` & `dagster-1.7.3/dagster/_core/storage/noop_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/output_manager.py` & `dagster-1.7.3/dagster/_core/storage/output_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/partition_status_cache.py` & `dagster-1.7.3/dagster/_core/storage/partition_status_cache.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/root.py` & `dagster-1.7.3/dagster/_core/storage/root.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/runs/base.py` & `dagster-1.7.3/dagster/_core/storage/runs/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/runs/in_memory.py` & `dagster-1.7.3/dagster/_core/storage/runs/in_memory.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/runs/migration.py` & `dagster-1.7.3/dagster/_core/storage/runs/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/runs/schema.py` & `dagster-1.7.3/dagster/_core/storage/runs/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/runs/sql_run_storage.py` & `dagster-1.7.3/dagster/_core/storage/runs/sql_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/runs/sqlite/alembic/alembic.ini` & `dagster-1.7.3/dagster/_core/storage/runs/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py` & `dagster-1.7.3/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/schedules/base.py` & `dagster-1.7.3/dagster/_core/storage/schedules/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/schedules/migration.py` & `dagster-1.7.3/dagster/_core/storage/schedules/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/schedules/schema.py` & `dagster-1.7.3/dagster/_core/storage/schedules/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/schedules/sql_schedule_storage.py` & `dagster-1.7.3/dagster/_core/storage/schedules/sql_schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini` & `dagster-1.7.3/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py` & `dagster-1.7.3/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/sql.py` & `dagster-1.7.3/dagster/_core/storage/sql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/sqlalchemy_compat.py` & `dagster-1.7.3/dagster/_core/storage/sqlalchemy_compat.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/sqlite.py` & `dagster-1.7.3/dagster/_core/storage/sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/sqlite_storage.py` & `dagster-1.7.3/dagster/_core/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/tags.py` & `dagster-1.7.3/dagster/_core/storage/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/temp_file_manager.py` & `dagster-1.7.3/dagster/_core/storage/temp_file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/storage/upath_io_manager.py` & `dagster-1.7.3/dagster/_core/storage/upath_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/system_config/composite_descent.py` & `dagster-1.7.3/dagster/_core/system_config/composite_descent.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/system_config/objects.py` & `dagster-1.7.3/dagster/_core/system_config/objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/telemetry.py` & `dagster-1.7.3/dagster/_core/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/telemetry_upload.py` & `dagster-1.7.3/dagster/_core/telemetry_upload.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/test_utils.py` & `dagster-1.7.3/dagster/_core/test_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/types/builtin_config_schemas.py` & `dagster-1.7.3/dagster/_core/types/builtin_config_schemas.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/types/config_schema.py` & `dagster-1.7.3/dagster/_core/types/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/types/dagster_type.py` & `dagster-1.7.3/dagster/_core/types/dagster_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/types/decorator.py` & `dagster-1.7.3/dagster/_core/types/decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/types/loadable_target_origin.py` & `dagster-1.7.3/dagster/_core/types/loadable_target_origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/types/primitive_mapping.py` & `dagster-1.7.3/dagster/_core/types/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/types/python_dict.py` & `dagster-1.7.3/dagster/_core/types/python_dict.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/types/python_set.py` & `dagster-1.7.3/dagster/_core/types/python_set.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/types/python_tuple.py` & `dagster-1.7.3/dagster/_core/types/python_tuple.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/types/transform_typing.py` & `dagster-1.7.3/dagster/_core/types/transform_typing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/utility_ops.py` & `dagster-1.7.3/dagster/_core/utility_ops.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/utils.py` & `dagster-1.7.3/dagster/_core/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/workspace/autodiscovery.py` & `dagster-1.7.3/dagster/_core/workspace/autodiscovery.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/workspace/batch_asset_record_loader.py` & `dagster-1.7.3/dagster/_core/workspace/batch_asset_record_loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,14 +49,26 @@
     ) -> Optional[EventLogEntry]:
         asset_record = self.get_asset_record(asset_key)
         if not asset_record:
             return None
 
         return asset_record.asset_entry.last_materialization
 
+    def get_latest_observation_for_asset_key(self, asset_key: AssetKey) -> Optional[EventLogEntry]:
+        check.invariant(
+            self._instance.event_log_storage.asset_records_have_last_observation,
+            "Event log storage must support fetching the last observation from asset records",
+        )
+
+        asset_record = self.get_asset_record(asset_key)
+        if not asset_record:
+            return None
+
+        return asset_record.asset_entry.last_observation
+
     def _fetch(self) -> None:
         if not self._unfetched_asset_keys:
             return
 
         new_records = {
             record.asset_entry.asset_key: record
             for record in self._instance.get_asset_records(list(self._unfetched_asset_keys))
```

### Comparing `dagster-1.7.2rc4/dagster/_core/workspace/config_schema.py` & `dagster-1.7.3/dagster/_core/workspace/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/workspace/context.py` & `dagster-1.7.3/dagster/_core/workspace/context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/workspace/load.py` & `dagster-1.7.3/dagster/_core/workspace/load.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/workspace/load_target.py` & `dagster-1.7.3/dagster/_core/workspace/load_target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/workspace/permissions.py` & `dagster-1.7.3/dagster/_core/workspace/permissions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_core/workspace/workspace.py` & `dagster-1.7.3/dagster/_core/workspace/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_daemon/__init__.py` & `dagster-1.7.3/dagster/_daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_daemon/asset_daemon.py` & `dagster-1.7.3/dagster/_daemon/asset_daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py` & `dagster-1.7.3/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_daemon/auto_run_reexecution/event_log_consumer.py` & `dagster-1.7.3/dagster/_daemon/auto_run_reexecution/event_log_consumer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_daemon/backfill.py` & `dagster-1.7.3/dagster/_daemon/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_daemon/cli/__init__.py` & `dagster-1.7.3/dagster/_daemon/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_daemon/controller.py` & `dagster-1.7.3/dagster/_daemon/controller.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_daemon/daemon.py` & `dagster-1.7.3/dagster/_daemon/daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_daemon/monitoring/concurrency.py` & `dagster-1.7.3/dagster/_daemon/monitoring/concurrency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_daemon/monitoring/run_monitoring.py` & `dagster-1.7.3/dagster/_daemon/monitoring/run_monitoring.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py` & `dagster-1.7.3/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import sys
 import threading
 import time
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from contextlib import ExitStack
 from typing import Dict, Iterable, Iterator, List, Optional, Sequence
 
@@ -288,14 +289,20 @@
                 else:
                     tag_concurrency_limits_counter.update_counters_with_launched_item(run)
 
                 if (
                     global_concurrency_limits_counter
                     and global_concurrency_limits_counter.is_blocked(run)
                 ):
+                    concurrency_blocked_info = json.dumps(
+                        global_concurrency_limits_counter.get_blocked_run_debug_info(run)
+                    )
+                    self._logger.info(
+                        f"Run {run.run_id} is blocked by global concurrency limits: {concurrency_blocked_info}"
+                    )
                     to_remove.append(run)
                     continue
                 elif global_concurrency_limits_counter:
                     global_concurrency_limits_counter.update_counters_with_launched_item(run)
 
                 location_name = (
                     run.external_job_origin.location_name if run.external_job_origin else None
```

### Comparing `dagster-1.7.2rc4/dagster/_daemon/sensor.py` & `dagster-1.7.3/dagster/_daemon/sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_daemon/types.py` & `dagster-1.7.3/dagster/_daemon/types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_daemon/utils.py` & `dagster-1.7.3/dagster/_daemon/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_daemon/workspace.py` & `dagster-1.7.3/dagster/_daemon/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_generate/download.py` & `dagster-1.7.3/dagster/_generate/download.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_generate/generate.py` & `dagster-1.7.3/dagster/_generate/generate.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md` & `dagster-1.7.3/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_grpc/__generated__/api_pb2.py` & `dagster-1.7.3/dagster/_grpc/__generated__/api_pb2.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_grpc/__generated__/api_pb2.pyi` & `dagster-1.7.3/dagster/_grpc/__generated__/api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_grpc/__generated__/api_pb2_grpc.py` & `dagster-1.7.3/dagster/_grpc/__generated__/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_grpc/__init__.py` & `dagster-1.7.3/dagster/_grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_grpc/client.py` & `dagster-1.7.3/dagster/_grpc/client.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_grpc/compile.py` & `dagster-1.7.3/dagster/_grpc/compile.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_grpc/impl.py` & `dagster-1.7.3/dagster/_grpc/impl.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_grpc/protos/api.proto` & `dagster-1.7.3/dagster/_grpc/protos/api.proto`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_grpc/proxy_server.py` & `dagster-1.7.3/dagster/_grpc/proxy_server.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_grpc/server.py` & `dagster-1.7.3/dagster/_grpc/server.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_grpc/server_watcher.py` & `dagster-1.7.3/dagster/_grpc/server_watcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_grpc/types.py` & `dagster-1.7.3/dagster/_grpc/types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_grpc/utils.py` & `dagster-1.7.3/dagster/_grpc/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_loggers/__init__.py` & `dagster-1.7.3/dagster/_loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_model/__init__.py` & `dagster-1.7.3/dagster/_model/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_model/pydantic_compat_layer.py` & `dagster-1.7.3/dagster/_model/pydantic_compat_layer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_module_alias_map.py` & `dagster-1.7.3/dagster/_module_alias_map.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_scheduler/scheduler.py` & `dagster-1.7.3/dagster/_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_scheduler/stale.py` & `dagster-1.7.3/dagster/_scheduler/stale.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_serdes/__init__.py` & `dagster-1.7.3/dagster/_serdes/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_serdes/config_class.py` & `dagster-1.7.3/dagster/_serdes/config_class.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 import importlib
-import importlib.util
-import logging
 from abc import ABC, abstractmethod
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     Mapping,
     NamedTuple,
@@ -15,15 +13,14 @@
     cast,
     overload,
 )
 
 from typing_extensions import Self
 
 import dagster._check as check
-from dagster._core.errors import DagsterImportClassFromCodePointerError
 from dagster._utils import convert_dagster_submodule_name
 from dagster._utils.yaml_utils import load_run_config_yaml
 
 from .serdes import (
     NamedTupleSerializer,
     whitelist_for_serdes,
 )
@@ -85,53 +82,40 @@
 
     @overload
     def rehydrate(self, as_type: None = ...) -> "ConfigurableClass": ...
 
     @overload
     def rehydrate(self, as_type: Type[T_ConfigurableClass]) -> T_ConfigurableClass: ...
 
-    def _rehydrate_klass_with_dagster_plus(self) -> Type["ConfigurableClass"]:
-        module_elems = self.module_name.split(".")
-        # When attempting to rehydrate a configurable class, attempt to load from dagster_plus
-        # instead of dagster_cloud if the dagster_plus package exists
-        if (
-            "dagster_cloud" == module_elems[0]
-            and importlib.util.find_spec("dagster_plus") is not None
-        ):
-            try:
-                return cast(
-                    Type[ConfigurableClass],
-                    class_from_code_pointer(
-                        ".".join(["dagster_plus", *module_elems[1:]]),
-                        self.class_name,
-                    ),
-                )
-            except DagsterImportClassFromCodePointerError:
-                logger = logging.getLogger("dagster")
-                logger.exception("Error importing DagsterInstance class from dagster_plus module")
-
-        # If the module is not in dagster_plus, or if the dagster_plus package does not exist,
-        # load it from the original module
-        return cast(
-            Type[ConfigurableClass], class_from_code_pointer(self.module_name, self.class_name)
-        )
-
     def rehydrate(
         self, as_type: Optional[Type[T_ConfigurableClass]] = None
     ) -> Union["ConfigurableClass", T_ConfigurableClass]:
         from dagster._config import process_config, resolve_to_config_type
         from dagster._core.errors import DagsterInvalidConfigError
 
-        klass = self._rehydrate_klass_with_dagster_plus()
+        try:
+            module = importlib.import_module(self.module_name)
+        except ModuleNotFoundError:
+            check.failed(
+                f"Couldn't import module {self.module_name} when attempting to load the "
+                f"configurable class {self.module_name}.{self.class_name}"
+            )
+        try:
+            # All rehydrated classes are expected to implement the ConfigurableClass interface and
+            # will error when we call `klass.from_config_value` and `klass.config_type` below if
+            # they do not. However, not all rehydrated classes actually have `ConfigurableClass` as
+            # an ancestor due to some subtleties around multiple abstract classes that cause an
+            # error when `ConfigurableClass` is added as an ancestor to storage classes.
+            klass = cast(Type[ConfigurableClass], getattr(module, self.class_name))
+        except AttributeError:
+            check.failed(
+                f"Couldn't find class {self.class_name} in module when attempting to load the "
+                f"configurable class {self.module_name}.{self.class_name}"
+            )
 
-        # All rehydrated classes are expected to implement the ConfigurableClass interface and
-        # will error when we call `klass.from_config_value` and `klass.config_type` below if
-        # they do not. However, not all rehydrated classes actually have `ConfigurableClass` as
-        # an ancestor due to some subtleties around multiple abstract classes that cause an
-        # error when `ConfigurableClass` is added as an ancestor to storage classes.
         if not issubclass(klass, as_type or ConfigurableClass):
             raise check.CheckError(
                 klass,
                 f"class {self.class_name} in module {self.module_name}",
                 ConfigurableClass,
             )
 
@@ -230,23 +214,23 @@
         """
 
 
 def class_from_code_pointer(module_name: str, class_name: str) -> Type[object]:
     try:
         module = importlib.import_module(module_name)
     except ModuleNotFoundError:
-        raise DagsterImportClassFromCodePointerError(
+        check.failed(
             "Couldn't import module {module_name} when attempting to load the class {klass}".format(
                 module_name=module_name,
                 klass=module_name + "." + class_name,
             )
         )
     try:
         return getattr(module, class_name)
     except AttributeError:
-        raise DagsterImportClassFromCodePointerError(
+        check.failed(
             "Couldn't find class {class_name} in module when attempting to load the "
             "class {klass}".format(
                 class_name=class_name,
                 klass=module_name + "." + class_name,
             )
         )
```

### Comparing `dagster-1.7.2rc4/dagster/_serdes/ipc.py` & `dagster-1.7.3/dagster/_serdes/ipc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_serdes/serdes.py` & `dagster-1.7.3/dagster/_serdes/serdes.py`

 * *Files 1% similar despite different names*

```diff
@@ -668,19 +668,34 @@
 
 
 T_PydanticModel = TypeVar("T_PydanticModel", bound=pydantic.BaseModel, default=pydantic.BaseModel)
 
 
 class PydanticModelSerializer(ObjectSerializer[T_PydanticModel]):
     def object_as_mapping(self, value: T_PydanticModel) -> Mapping[str, Any]:
-        return value.__dict__
+        value_dict = value.__dict__
+
+        result = {}
+        for key, field in self.klass.__fields__.items():
+            if field.alias is None and (
+                getattr(field, "serialization_alias", None) is not None
+                or getattr(field, "validation_alias", None) is not None
+            ):
+                raise SerializationError(
+                    "Can't serialize pydantic models with serialization or validation aliases. Use "
+                    "the storage_field_names argument to whitelist_for_serdes instead."
+                )
+            result_key = field.alias if field.alias else key
+            result[result_key] = value_dict[key]
+
+        return result
 
     @property
     def constructor_param_names(self) -> Sequence[str]:
-        return list(self.klass.__fields__.keys())
+        return [field.alias or key for key, field in self.klass.__fields__.items()]
 
 
 class FieldSerializer(Serializer):
     _instance = None
 
     # Because `FieldSerializer` is not currently parameterizable (all variation is contained in the
     # logic of pack/unpack), we store references to a singleton instance in the whitelist map to
```

### Comparing `dagster-1.7.2rc4/dagster/_serdes/utils.py` & `dagster-1.7.3/dagster/_serdes/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_seven/__init__.py` & `dagster-1.7.3/dagster/_seven/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_seven/abc.py` & `dagster-1.7.3/dagster/_seven/abc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_seven/compat/pendulum.py` & `dagster-1.7.3/dagster/_seven/compat/pendulum.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_utils/__init__.py` & `dagster-1.7.3/dagster/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_utils/alert.py` & `dagster-1.7.3/dagster/_utils/alert.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_utils/backoff.py` & `dagster-1.7.3/dagster/_utils/backoff.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_utils/cached_method.py` & `dagster-1.7.3/dagster/_utils/cached_method.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_utils/caching_instance_queryer.py` & `dagster-1.7.3/dagster/_utils/caching_instance_queryer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import os
 from collections import defaultdict
 from datetime import datetime
 from typing import (
     TYPE_CHECKING,
     AbstractSet,
     Dict,
     Iterable,
@@ -24,14 +25,15 @@
 from dagster._core.definitions.data_version import (
     DATA_VERSION_TAG,
     DataVersion,
     extract_data_version_from_entry,
 )
 from dagster._core.definitions.events import AssetKey, AssetKeyPartitionKey
 from dagster._core.definitions.partition import (
+    PartitionsDefinition,
     PartitionsSubset,
 )
 from dagster._core.definitions.time_window_partitions import (
     TimeWindowPartitionsDefinition,
     get_time_partition_key,
     get_time_partitions_def,
 )
@@ -570,15 +572,17 @@
             # keep track of the maximum storage id that we've seen for a given parent
             max_storage_ids.append(
                 self.get_latest_materialization_or_observation_storage_id(
                     AssetKeyPartitionKey(parent_asset_key)
                 )
             )
 
-            parent_partitions_def = self.asset_graph.get(parent_asset_key).partitions_def
+            parent_partitions_def: PartitionsDefinition = self.asset_graph.get(
+                parent_asset_key
+            ).partitions_def
             if parent_partitions_def is None:
                 latest_parent_record = check.not_none(
                     self.get_latest_materialization_or_observation_record(
                         AssetKeyPartitionKey(parent_asset_key), after_cursor=latest_storage_id
                     )
                 )
                 for child_partition_key in (
@@ -611,18 +615,20 @@
                 # we know a parent updated, and because the parent has a partitions def and the
                 # child does not, the child could not have been materialized in the same run
                 if child_asset.partitions_def is None:
                     child_asset_partitions_with_updated_parents = {
                         AssetKeyPartitionKey(child_asset_key)
                     }
                     break
+
                 # the set of asset partitions which have been updated since the latest storage id
                 parent_partitions_subset = self.get_asset_subset_updated_after_cursor(
                     asset_key=parent_asset_key, after_cursor=latest_storage_id
                 ).subset_value
+
                 # we are mapping from the partitions of the parent asset to the partitions of
                 # the child asset
                 partition_mapping = self.asset_graph.get_partition_mapping(
                     asset_key=child_asset_key, parent_asset_key=parent_asset_key
                 )
                 try:
                     child_partitions_subset = (
@@ -636,15 +642,21 @@
                     )
                 except DagsterInvalidDefinitionError as e:
                     # add a more helpful error message to the stack
                     raise DagsterInvalidDefinitionError(
                         f"Could not map partitions between parent {parent_asset_key.to_string()} "
                         f"and child {child_asset_key.to_string()}."
                     ) from e
-                for child_partition in child_partitions_subset.get_partition_keys():
+
+                child_partitions = reversed(list(child_partitions_subset.get_partition_keys()))
+                max_child_partitions = os.getenv("DAGSTER_MAX_AMP_CHILD_PARTITIONS", None)
+                if max_child_partitions:
+                    child_partitions = list(child_partitions)[: int(max_child_partitions)]
+
+                for child_partition in child_partitions:
                     # we need to see if the child is planned for the same run, but this is
                     # expensive, so we try to avoid doing so in as many situations as possible
                     child_asset_partition = AssetKeyPartitionKey(child_asset_key, child_partition)
                     if (
                         # if child has a different partitions def than the parent, then it must
                         # have been executed in a different run, so it's a valid candidate
                         child_asset.partitions_def != parent_partitions_def
```

### Comparing `dagster-1.7.2rc4/dagster/_utils/concurrency.py` & `dagster-1.7.3/dagster/_utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_utils/container.py` & `dagster-1.7.3/dagster/_utils/container.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_utils/dagster_type.py` & `dagster-1.7.3/dagster/_utils/dagster_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_utils/env.py` & `dagster-1.7.3/dagster/_utils/env.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_utils/error.py` & `dagster-1.7.3/dagster/_utils/error.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_utils/external.py` & `dagster-1.7.3/dagster/_utils/external.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_utils/forked_pdb.py` & `dagster-1.7.3/dagster/_utils/forked_pdb.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_utils/hosted_user_process.py` & `dagster-1.7.3/dagster/_utils/hosted_user_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_utils/indenting_printer.py` & `dagster-1.7.3/dagster/_utils/indenting_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_utils/internal_init.py` & `dagster-1.7.3/dagster/_utils/internal_init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_utils/interrupts.py` & `dagster-1.7.3/dagster/_utils/interrupts.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_utils/log.py` & `dagster-1.7.3/dagster/_utils/log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_utils/merger.py` & `dagster-1.7.3/dagster/_utils/merger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_utils/net.py` & `dagster-1.7.3/dagster/_utils/net.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_utils/schedules.py` & `dagster-1.7.3/dagster/_utils/schedules.py`

 * *Files 0% similar despite different names*

```diff
@@ -900,18 +900,26 @@
             # Increment all iterators that generated the earliest subsequent datetime.
             for i, next_date in enumerate(next_dates):
                 if next_date == earliest_next_date:
                     next_dates[i] = next(iterators[i])
 
 
 def get_latest_completed_cron_tick(
-    cron_string: Optional[str], current_time: datetime.datetime, timezone: Optional[str]
-) -> Optional[datetime.datetime]:
-    if not cron_string:
-        return None
-
+    cron_string: str, current_time: datetime.datetime, timezone: Optional[str]
+) -> datetime.datetime:
     cron_iter = reverse_cron_string_iterator(
         end_timestamp=current_time.timestamp(),
         cron_string=cron_string,
         execution_timezone=timezone,
     )
     return pendulum.instance(next(cron_iter))
+
+
+def get_next_cron_tick(
+    cron_string: str, current_time: datetime.datetime, timezone: Optional[str]
+) -> datetime.datetime:
+    cron_iter = cron_string_iterator(
+        start_timestamp=current_time.timestamp(),
+        cron_string=cron_string,
+        execution_timezone=timezone,
+    )
+    return pendulum.instance(next(cron_iter))
```

### Comparing `dagster-1.7.2rc4/dagster/_utils/tags.py` & `dagster-1.7.3/dagster/_utils/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_utils/temp_file.py` & `dagster-1.7.3/dagster/_utils/temp_file.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_utils/test/__init__.py` & `dagster-1.7.3/dagster/_utils/test/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_utils/test/data_versions.py` & `dagster-1.7.3/dagster/_utils/test/data_versions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any, Dict, List, Mapping, Optional, Sequence, Tuple, Union, cast, overload
 
 from typing_extensions import Literal
 
 from dagster._core.definitions.asset_graph import AssetGraph
+from dagster._core.definitions.asset_selection import CoercibleToAssetSelection
 from dagster._core.definitions.assets import AssetsDefinition
 from dagster._core.definitions.data_version import (
     CODE_VERSION_TAG,
     DATA_VERSION_TAG,
     INPUT_DATA_VERSION_TAG_PREFIX,
     CachingStaleStatusResolver,
     DataVersion,
@@ -182,22 +183,24 @@
 
 def materialize_assets(
     assets: Sequence[AssetsDefinition],
     instance: DagsterInstance,
     partition_key: Optional[str] = None,
     run_config: Optional[Mapping[str, Any]] = None,
     tags: Optional[Mapping[str, str]] = None,
+    selection: Optional[CoercibleToAssetSelection] = None,
 ) -> MaterializationTable:
     result = materialize(
         assets,
         instance=instance,
         resources={"io_manager": mock_io_manager},
         partition_key=partition_key,
         run_config=run_config,
         tags=tags,
+        selection=selection,
     )
     return get_mats_from_result(result, assets)
 
 
 def materialize_twice(
     all_assets: Sequence[Union[AssetsDefinition, SourceAsset]],
     asset_to_materialize: AssetsDefinition,
```

### Comparing `dagster-1.7.2rc4/dagster/_utils/test/mysql_instance.py` & `dagster-1.7.3/dagster/_utils/test/mysql_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_utils/test/postgres_instance.py` & `dagster-1.7.3/dagster/_utils/test/postgres_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_utils/test/schedule_storage.py` & `dagster-1.7.3/dagster/_utils/test/schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_utils/timing.py` & `dagster-1.7.3/dagster/_utils/timing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_utils/typed_dict.py` & `dagster-1.7.3/dagster/_utils/typed_dict.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_utils/typing_api.py` & `dagster-1.7.3/dagster/_utils/typing_api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_utils/warnings.py` & `dagster-1.7.3/dagster/_utils/warnings.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster/_utils/yaml_utils.py` & `dagster-1.7.3/dagster/_utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster.egg-info/PKG-INFO` & `dagster-1.7.3/dagster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.7.2rc4
+Version: 1.7.3
 Summary: Dagster is an orchestration platform for the development, production, and observation of data assets.
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Documentation, https://docs.dagster.io
```

### Comparing `dagster-1.7.2rc4/dagster.egg-info/SOURCES.txt` & `dagster-1.7.3/dagster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc4/dagster.egg-info/requires.txt` & `dagster-1.7.3/dagster.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 structlog
 sqlalchemy<3,>=1.0
 toposort>=1.0
 watchdog>=0.8.3
 docstring-parser
 pydantic!=1.10.7,<3,>1.10.0
 rich
-dagster-pipes==1.7.2rc4
+dagster-pipes==1.7.3
 
 [:platform_system == "Windows"]
 psutil>=1.0
 pywin32!=226
 
 [:python_version < "3.11"]
 protobuf<5,>=3.20.0
```

### Comparing `dagster-1.7.2rc4/setup.py` & `dagster-1.7.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         'pywin32!=226; platform_system=="Windows"',
         "docstring-parser",
         "universal_pathlib; python_version<'3.12'",
         "universal_pathlib>=0.2.0; python_version>='3.12'",
         # https://github.com/pydantic/pydantic/issues/5821
         "pydantic>1.10.0,!= 1.10.7,<3",
         "rich",
-        "dagster-pipes==1.7.2rc4",
+        "dagster-pipes==1.7.3",
     ],
     extras_require={
         "docker": ["docker"],
         "test": [
             "buildkite-test-collector",
             "docker",
             f"grpcio-tools>={GRPC_VERSION_FLOOR}",
```

