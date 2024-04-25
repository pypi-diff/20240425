# Comparing `tmp/onnxscript-0.1.0.dev20240423.tar.gz` & `tmp/onnxscript-0.1.0.dev20240424.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnxscript-0.1.0.dev20240423.tar", last modified: Tue Apr 23 00:01:14 2024, max compression
+gzip compressed data, was "onnxscript-0.1.0.dev20240424.tar", last modified: Wed Apr 24 00:01:52 2024, max compression
```

## Comparing `onnxscript-0.1.0.dev20240423.tar` & `onnxscript-0.1.0.dev20240424.tar`

### file list

```diff
@@ -1,218 +1,218 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:14.036362 onnxscript-0.1.0.dev20240423/
--rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    10897 2024-04-23 00:01:14.036362 onnxscript-0.1.0.dev20240423/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8680 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/VERSION
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:13.988362 onnxscript-0.1.0.dev20240423/onnxscript/
--rw-r--r--   0 vsts      (1001) docker     (127)     2282 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:13.992362 onnxscript-0.1.0.dev20240423/onnxscript/_internal/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/_internal/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/_internal/analysis.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/_internal/ast_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/_internal/autocast.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/_internal/deprecation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/_internal/param_manipulation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1176 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/_internal/runtime_typing.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/_internal/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1018 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/_internal/version_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:13.992362 onnxscript-0.1.0.dev20240423/onnxscript/_legacy_ir/
--rw-r--r--   0 vsts      (1001) docker     (127)    11316 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/_legacy_ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36198 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/_legacy_ir/visitor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:13.992362 onnxscript-0.1.0.dev20240423/onnxscript/_thirdparty/
--rw-r--r--   0 vsts      (1001) docker     (127)    10608 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/_thirdparty/asciichartpy.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:13.996362 onnxscript-0.1.0.dev20240423/onnxscript/backend/
--rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/backend/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/backend/onnx_backend.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/backend/onnx_export.py
--rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/converter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:13.980362 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:13.996362 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/
--rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/_infra.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/context.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/decorator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/formatter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:14.008362 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/
--rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_address.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_artifact.py
--rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_artifact_change.py
--rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_artifact_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_artifact_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_attachment.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_code_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_configuration_override.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_conversion.py
--rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_edge.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_exception.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_external_properties.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_fix.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_invocation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_location_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_logical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_message.py
--rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_node.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_notification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_physical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_property_bag.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_rectangle.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_region.py
--rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_replacement.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_result.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_result_provenance.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_run.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_sarif_log.py
--rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_special_locations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_stack.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_stack_frame.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_suppression.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_thread_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_tool.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_tool_component.py
--rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_version_control_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_web_request.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_web_response.py
--rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/version.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/evaluator.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:13.980362 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:13.980362 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/tools/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:14.012362 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/tools/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:14.012362 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/_constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/_flags.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:14.012362 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/graph_building/
--rw-r--r--   0 vsts      (1001) docker     (127)     2291 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/graph_building/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    27757 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43814 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:14.016362 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/
--rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/common.py
--rw-r--r--   0 vsts      (1001) docker     (127)   290367 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/core.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/fft.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/linalg.py
--rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/nested.py
--rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/nn.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/prims.py
--rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/sparse.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/special.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/vision.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/registration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/tensor_typing.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:14.020362 onnxscript-0.1.0.dev20240423/onnxscript/ir/
--rw-r--r--   0 vsts      (1001) docker     (127)     2394 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8489 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/ir/_convenience.py
--rw-r--r--   0 vsts      (1001) docker     (127)    77495 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/ir/_core.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1775 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/ir/_display.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3908 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/ir/_enums.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/ir/_graph_comparison.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1853 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/ir/_invariants.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10417 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/ir/_linked_list.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1684 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/ir/_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1064 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/ir/_name_authority.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19580 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/ir/_protocols.py
--rw-r--r--   0 vsts      (1001) docker     (127)    47188 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/ir/serde.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/irbuilder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/main.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:14.020362 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/
--rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:14.028362 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/
--rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset1.py
--rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset10.py
--rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset11.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset12.py
--rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset13.py
--rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset14.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset15.py
--rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset16.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset17.py
--rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset18.py
--rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset19.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset20.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset4.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset5.py
--rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset6.py
--rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset7.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset8.py
--rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset9.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_types.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:14.028362 onnxscript-0.1.0.dev20240423/onnxscript/optimizer/
--rw-r--r--   0 vsts      (1001) docker     (127)     4316 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/optimizer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10166 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/optimizer/constant_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2872 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/optimizer/copy_propagation.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15603 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/optimizer/evaluator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/optimizer/fold_constants_v0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/optimizer/remove_unused.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2080 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/optimizer/remove_unused_function.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9852 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/optimizer/simple_function_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/py.typed
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:14.032362 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/
--rw-r--r--   0 vsts      (1001) docker     (127)     1375 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1342 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/_ir_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1782 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/_tape.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6926 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/broadcast_to_matmul.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2170 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/cast_constant_of_shape.py
--rw-r--r--   0 vsts      (1001) docker     (127)      686 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/erfgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8918 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/function_rule.py
--rw-r--r--   0 vsts      (1001) docker     (127)      756 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/gemm_to_matmul_add.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36273 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/generic_pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)      828 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/no_op.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:14.032362 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/onnxruntime/
--rw-r--r--   0 vsts      (1001) docker     (127)     2139 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/onnxruntime/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1222 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5746 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1922 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/onnxruntime/softmax.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:14.036362 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/onnxruntime/transformers/
--rw-r--r--   0 vsts      (1001) docker     (127)      543 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/onnxruntime/transformers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1097 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)      885 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1628 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24688 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
--rw-r--r--   0 vsts      (1001) docker     (127)    41992 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/sourceinfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/tensor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:14.036362 onnxscript-0.1.0.dev20240423/onnxscript/testing/
--rw-r--r--   0 vsts      (1001) docker     (127)    17350 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/testing/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/type_annotation.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:14.036362 onnxscript-0.1.0.dev20240423/onnxscript/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/utils/evaluation_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/utils/timing_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/utils/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24803 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/values.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:14.036362 onnxscript-0.1.0.dev20240423/onnxscript.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    10897 2024-04-23 00:01:13.000000 onnxscript-0.1.0.dev20240423/onnxscript.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8203 2024-04-23 00:01:13.000000 onnxscript-0.1.0.dev20240423/onnxscript.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-23 00:01:13.000000 onnxscript-0.1.0.dev20240423/onnxscript.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-04-23 00:01:13.000000 onnxscript-0.1.0.dev20240423/onnxscript.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-04-23 00:01:13.000000 onnxscript-0.1.0.dev20240423/onnxscript.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     6453 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-23 00:01:14.036362 onnxscript-0.1.0.dev20240423/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1292 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.570317 onnxscript-0.1.0.dev20240424/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    10863 2024-04-24 00:01:52.570317 onnxscript-0.1.0.dev20240424/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8680 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/VERSION
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.510317 onnxscript-0.1.0.dev20240424/onnxscript/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2282 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.514317 onnxscript-0.1.0.dev20240424/onnxscript/_internal/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/_internal/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/_internal/analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/_internal/ast_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/_internal/autocast.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/_internal/deprecation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/_internal/param_manipulation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1176 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/_internal/runtime_typing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/_internal/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1018 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/_internal/version_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.514317 onnxscript-0.1.0.dev20240424/onnxscript/_legacy_ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11316 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/_legacy_ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36198 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/_legacy_ir/visitor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.514317 onnxscript-0.1.0.dev20240424/onnxscript/_thirdparty/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10608 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/_thirdparty/asciichartpy.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.514317 onnxscript-0.1.0.dev20240424/onnxscript/backend/
+-rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/backend/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/backend/onnx_backend.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/backend/onnx_export.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/converter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.506317 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.514317 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/
+-rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/_infra.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/context.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/decorator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/formatter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.538317 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_address.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_artifact.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_artifact_change.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_artifact_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_artifact_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_attachment.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_code_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_configuration_override.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_conversion.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_edge.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_exception.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_external_properties.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_fix.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_invocation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_location_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_logical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_message.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_node.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_notification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_physical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_property_bag.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_rectangle.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_region.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_replacement.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_result.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_result_provenance.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_run.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_sarif_log.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_special_locations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_stack.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_stack_frame.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_suppression.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_thread_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_tool.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_tool_component.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_version_control_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_web_request.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_web_response.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/version.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/evaluator.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.506317 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.506317 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/tools/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.538317 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/tools/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.538317 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/_flags.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.542317 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/graph_building/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2291 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/graph_building/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    27757 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43814 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.546317 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/
+-rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/common.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   290367 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/fft.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/linalg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/nested.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/nn.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/prims.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/sparse.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/special.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/vision.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/registration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/tensor_typing.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.550317 onnxscript-0.1.0.dev20240424/onnxscript/ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2394 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8474 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/ir/_convenience.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    77357 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/ir/_core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1775 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/ir/_display.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3908 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/ir/_enums.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/ir/_graph_comparison.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1853 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/ir/_invariants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10518 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/ir/_linked_list.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1684 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/ir/_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1064 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/ir/_name_authority.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19570 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/ir/_protocols.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    47188 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/ir/serde.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/irbuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/main.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.550317 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.558317 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/
+-rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset10.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset11.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset12.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset13.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset14.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset15.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset16.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset17.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset18.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset19.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset20.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset5.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset6.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset7.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset8.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset9.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/onnx_types.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.562317 onnxscript-0.1.0.dev20240424/onnxscript/optimizer/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4316 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/optimizer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10166 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/optimizer/constant_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2872 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/optimizer/copy_propagation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15603 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/optimizer/evaluator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/optimizer/fold_constants_v0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/optimizer/remove_unused.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2080 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/optimizer/remove_unused_function.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9852 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/optimizer/simple_function_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.566317 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1253 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1342 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/_ir_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1782 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/_tape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6926 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/broadcast_to_matmul.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2170 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/cast_constant_of_shape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      686 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/erfgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8567 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/function_rule.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      756 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/gemm_to_matmul_add.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36263 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/generic_pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      828 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/no_op.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.566317 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/onnxruntime/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2139 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/onnxruntime/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1222 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5746 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1922 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/onnxruntime/softmax.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.570317 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/onnxruntime/transformers/
+-rw-r--r--   0 vsts      (1001) docker     (127)      543 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/onnxruntime/transformers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1019 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      826 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1647 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24160 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    41987 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/rewriter/pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/sourceinfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/tensor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.570317 onnxscript-0.1.0.dev20240424/onnxscript/testing/
+-rw-r--r--   0 vsts      (1001) docker     (127)    17350 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/testing/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/type_annotation.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.570317 onnxscript-0.1.0.dev20240424/onnxscript/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/utils/evaluation_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/utils/timing_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/utils/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24803 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/onnxscript/values.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 00:01:52.570317 onnxscript-0.1.0.dev20240424/onnxscript.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10863 2024-04-24 00:01:52.000000 onnxscript-0.1.0.dev20240424/onnxscript.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8203 2024-04-24 00:01:52.000000 onnxscript-0.1.0.dev20240424/onnxscript.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-24 00:01:52.000000 onnxscript-0.1.0.dev20240424/onnxscript.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-04-24 00:01:52.000000 onnxscript-0.1.0.dev20240424/onnxscript.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-04-24 00:01:52.000000 onnxscript-0.1.0.dev20240424/onnxscript.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     6453 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-24 00:01:52.570317 onnxscript-0.1.0.dev20240424/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1304 2024-04-24 00:00:47.000000 onnxscript-0.1.0.dev20240424/setup.py
```

### Comparing `onnxscript-0.1.0.dev20240423/LICENSE` & `onnxscript-0.1.0.dev20240424/LICENSE`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/PKG-INFO` & `onnxscript-0.1.0.dev20240424/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240423
+Version: 0.1.0.dev20240424
 Summary: Naturally author ONNX functions and models using a subset of Python
-Home-page: https://onnxscript.ai/
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `onnxscript-0.1.0.dev20240423/README.md` & `onnxscript-0.1.0.dev20240424/README.md`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/__init__.py` & `onnxscript-0.1.0.dev20240424/onnxscript/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/_internal/analysis.py` & `onnxscript-0.1.0.dev20240424/onnxscript/_internal/analysis.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/_internal/ast_utils.py` & `onnxscript-0.1.0.dev20240424/onnxscript/_internal/ast_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/_internal/autocast.py` & `onnxscript-0.1.0.dev20240424/onnxscript/_internal/autocast.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/_internal/deprecation.py` & `onnxscript-0.1.0.dev20240424/onnxscript/_internal/deprecation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/_internal/param_manipulation.py` & `onnxscript-0.1.0.dev20240424/onnxscript/_internal/param_manipulation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/_internal/runtime_typing.py` & `onnxscript-0.1.0.dev20240424/onnxscript/_internal/runtime_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/_internal/utils.py` & `onnxscript-0.1.0.dev20240424/onnxscript/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/_internal/version_utils.py` & `onnxscript-0.1.0.dev20240424/onnxscript/_internal/version_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/_legacy_ir/__init__.py` & `onnxscript-0.1.0.dev20240424/onnxscript/_legacy_ir/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/_legacy_ir/visitor.py` & `onnxscript-0.1.0.dev20240424/onnxscript/_legacy_ir/visitor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/_thirdparty/asciichartpy.py` & `onnxscript-0.1.0.dev20240424/onnxscript/_thirdparty/asciichartpy.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/backend/onnx_backend.py` & `onnxscript-0.1.0.dev20240424/onnxscript/backend/onnx_backend.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/backend/onnx_export.py` & `onnxscript-0.1.0.dev20240424/onnxscript/backend/onnx_export.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/converter.py` & `onnxscript-0.1.0.dev20240424/onnxscript/converter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/__init__.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/_infra.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/_infra.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/context.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/context.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/decorator.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/decorator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/formatter.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/formatter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/__init__.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_address.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_address.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_artifact.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_artifact.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_artifact_change.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_artifact_change.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_artifact_content.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_artifact_content.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_artifact_location.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_artifact_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_attachment.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_attachment.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_code_flow.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_code_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_configuration_override.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_configuration_override.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_conversion.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_conversion.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_edge.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_edge.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_edge_traversal.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_edge_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_exception.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_exception.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_external_properties.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_external_properties.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_fix.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_fix.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_graph.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_graph.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_graph_traversal.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_graph_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_invocation.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_invocation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_location.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_location_relationship.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_location_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_logical_location.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_logical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_message.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_message.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_node.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_node.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_notification.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_notification.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_physical_location.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_physical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_rectangle.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_rectangle.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_region.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_region.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_replacement.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_replacement.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_result.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_result.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_result_provenance.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_result_provenance.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_run.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_run.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_run_automation_details.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_run_automation_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_sarif_log.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_sarif_log.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_special_locations.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_special_locations.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_stack.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_stack.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_stack_frame.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_stack_frame.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_suppression.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_suppression.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_thread_flow.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_thread_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_tool.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_tool.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_tool_component.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_tool_component.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_translation_metadata.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_translation_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_version_control_details.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_version_control_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_web_request.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_web_request.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_web_response.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/sarif/_web_response.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/utils.py` & `onnxscript-0.1.0.dev20240424/onnxscript/diagnostics/infra/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/evaluator.py` & `onnxscript-0.1.0.dev20240424/onnxscript/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py` & `onnxscript-0.1.0.dev20240424/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py` & `onnxscript-0.1.0.dev20240424/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py` & `onnxscript-0.1.0.dev20240424/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/_flags.py` & `onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/_flags.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/graph_building/__init__.py` & `onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/graph_building/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py` & `onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py` & `onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/common.py` & `onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/common.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/core.py` & `onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/core.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/fft.py` & `onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/fft.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/linalg.py` & `onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/nested.py` & `onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/nested.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/nn.py` & `onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/nn.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/prims.py` & `onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/prims.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/sparse.py` & `onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/sparse.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/special.py` & `onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/special.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/vision.py` & `onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/ops/vision.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/registration.py` & `onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/registration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/tensor_typing.py` & `onnxscript-0.1.0.dev20240424/onnxscript/function_libs/torch_lib/tensor_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/ir/__init__.py` & `onnxscript-0.1.0.dev20240424/onnxscript/ir/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/ir/_convenience.py` & `onnxscript-0.1.0.dev20240424/onnxscript/ir/_convenience.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
     return attributes
 
 
 def replace_all_uses_with(
     values: _protocols.ValueProtocol | Sequence[_protocols.ValueProtocol],
     replacements: _protocols.ValueProtocol | Sequence[_protocols.ValueProtocol],
 ) -> None:
-    """Replace all consumers of the given values with the replacements.
+    """Replace all uses of the given values with the replacements.
 
     This is useful when nodes in the graph are replaced with new nodes, where
     the old users need to be updated to use the outputs of the new nodes.
 
     For example, suppose we have the following graph::
 
         A -> {B, C}
@@ -190,15 +190,15 @@
         1
         >>> node_b.inputs[0].producer().op_type
         'D'
         >>> len(node_c.inputs)
         1
         >>> node_c.inputs[0].producer().op_type
         'D'
-        >>> len(node_a.outputs[0].consumers())
+        >>> len(node_a.outputs[0].uses())
         0
 
     When values and replacements are sequences, they are zipped into pairs. All
     users of the first value is replaced with the first replacement, and so on.
 
     .. note::
         You still need to update the graph outputs if any of the values being
@@ -212,9 +212,9 @@
     if not isinstance(values, Sequence):
         values = (values,)
     if not isinstance(replacements, Sequence):
         replacements = (replacements,)
     if len(values) != len(replacements):
         raise ValueError("The number of values and replacements must match.")
     for value, replacement in zip(values, replacements):
-        for user_node, index in tuple(value.consumers()):
+        for user_node, index in tuple(value.uses()):
             user_node.replace_input_with(index, replacement)
```

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/ir/_core.py` & `onnxscript-0.1.0.dev20240424/onnxscript/ir/_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -631,19 +631,19 @@
 class Node(_protocols.NodeProtocol, _display.PrettyPrintable):
     """IR Node.
 
     If the ``graph`` is provided, the node will be added to the graph. Otherwise,
     user is responsible to call ``graph.append(node)`` (or other mutation methods
     in :class:`Graph`) to add the node to the graph.
 
-    After the node is initialized, it will add itself as a consumer of the input values.
+    After the node is initialized, it will add itself as a user of the input values.
 
     The output values of the node are created during node initialization and are immutable.
-    To change the output values, create a new node and replace the each of the inputs of ``output.consumers`` with
-    the new output values by calling :meth:`replace_input_with` on the consumer nodes
+    To change the output values, create a new node and replace the each of the inputs of ``output.uses()`` with
+    the new output values by calling :meth:`replace_input_with` on the using nodes
     of this node's outputs.
     """
 
     __slots__ = (
         "_name",
         "_domain",
         "_op_type",
@@ -669,15 +669,15 @@
         num_outputs: int = 1,
         version: int | None = None,
         graph: Graph | None = None,
         name: str | None = None,
         doc_string: str | None = None,
         metadata_props: dict[str, str] | None = None,
     ):
-        """Initialize a node and add it as a consumer of the input values.
+        """Initialize a node and add it as a user of the input values.
 
         Args:
             domain: The domain of the operator. For onnx operators, this is an empty string.
             op_type: The name of the operator.
             inputs: The input values. When an input is None, it is an empty input.
             attributes: The attributes. RefAttr can be used only when the node is defined in a Function.
             overload: The overload name when the node is invoking a function.
@@ -714,18 +714,18 @@
         # TODO(justinchuby): Potentially support a version range
         self._version: int | None = version
         self._metadata: _metadata.MetadataStore | None = None
         self._metadata_props: dict[str, str] | None = metadata_props
         self._graph: Graph | None = graph
         self.doc_string = doc_string
 
-        # Add the node as a consumer of the inputs
+        # Add the node as a use of the inputs
         for i, input_value in enumerate(self._inputs):
             if input_value is not None:
-                input_value._add_consumer(self, i)  # pylint: disable=protected-access
+                input_value._add_usage(self, i)  # pylint: disable=protected-access
 
         # Add the node to the graph if graph is specified
         if self._graph is not None:
             self._graph.append(self)
 
     def __str__(self) -> str:
         node_type_text = f"{self._domain}::{self._op_type}" + f":{self._overload}" * (
@@ -817,17 +817,17 @@
         if index < 0 or index >= len(self.inputs):
             raise ValueError(f"Index out of range: {index}")
         old_input = self.inputs[index]
         self._inputs = tuple(
             value if i == index else old_input for i, old_input in enumerate(self.inputs)
         )
         if old_input is not None:
-            old_input._remove_consumer(self, index)  # pylint: disable=protected-access
+            old_input._remove_usage(self, index)  # pylint: disable=protected-access
         if value is not None:
-            value._add_consumer(self, index)  # pylint: disable=protected-access
+            value._add_usage(self, index)  # pylint: disable=protected-access
 
     def prepend(self, /, nodes: Node | Iterable[Node]) -> None:
         """Insert a node before this node in the list of nodes in the graph.
 
         It is the same as calling ``graph.insert_before(self, nodes)``.
 
         Example::
@@ -1012,15 +1012,15 @@
     are ``None``.
 
     When the value is owned by a node, it is an output of the node.
     The node that produces the value can be accessed with :meth:`producer`.
     The index of the output of the node that produces the value can be accessed with
     :meth:`index`.
 
-    To find all the nodes that use this value as an input, call :meth:`consumers`.
+    To find all the nodes that use this value as an input, call :meth:`uses`.
 
     To check if the value is an output of a graph, call :meth:`is_graph_output`.
 
     Attributes:
         name: The name of the value. A value is always named when it is part of a graph.
         shape: The shape of the value.
         type: The type of the value.
@@ -1032,15 +1032,15 @@
         "_index",
         "_metadata",
         "_metadata_props",
         "_name",
         "_shape",
         "_type",
         "_const_value",
-        "_consumers",
+        "_uses",
     )
 
     def __init__(
         self,
         producer: Node | None,
         *,
         index: int | None,
@@ -1059,18 +1059,18 @@
 
         self._name: str | None = name
         self._shape: Shape | None = shape
         self._type: _protocols.TypeProtocol | None = type
         # TODO(justinchuby): Handle initialization when a const value is provided
         # We can get shape and type information from the const value
         self._const_value = const_value
-        # Use a collection of (Node, int) to store consumers. This is needed
-        # because a single consumer can use the same value multiple times.
+        # Use a collection of (Node, int) to store uses. This is needed
+        # because a single use can use the same value multiple times.
         # Use a dictionary to preserve insertion order so that the visiting order is deterministic
-        self._consumers: dict[tuple[Node, int], None] = {}
+        self._uses: dict[tuple[Node, int], None] = {}
 
     def __repr__(self) -> str:
         value_name = self.name if self.name else "anonymous:" + str(id(self))
         producer = self.producer()
         producer_text = (
             producer.name or "anonymous_node:" + str(id(producer))
             if producer is not None
@@ -1091,35 +1091,35 @@
         """The node that produces this value."""
         return self._producer
 
     def index(self) -> int | None:
         """The index of the output of the defining node."""
         return self._index
 
-    def consumers(self) -> Collection[tuple[Node, int]]:
-        """Return a set of consumers of the value.
+    def uses(self) -> Collection[tuple[Node, int]]:
+        """Return a set of uses of the value.
 
         The set contains tuples of ``(Node, index)`` where the index is the index of the input
-        of the node. For example, if ``node.inputs[1] == value``, then the consumer is ``(node, 1)``.
+        of the node. For example, if ``node.inputs[1] == value``, then the use is ``(node, 1)``.
         """
-        return self._consumers.keys()
+        return self._uses.keys()
 
-    def _add_consumer(self, consumer: Node, index: int) -> None:
-        """Add a consumer node.
+    def _add_usage(self, use: Node, index: int) -> None:
+        """Add a usage of this value.
 
         This is an internal method. It should only be called by the Node class.
         """
-        self._consumers[(consumer, index)] = None
+        self._uses[(use, index)] = None
 
-    def _remove_consumer(self, consumer: Node, index: int) -> None:
-        """Remove a node from the consumers of this value.
+    def _remove_usage(self, use: Node, index: int) -> None:
+        """Remove a node from the uses of this value.
 
         This is an internal method. It should only be called by the Node class.
         """
-        self._consumers.pop((consumer, index))
+        self._uses.pop((use, index))
 
     @property
     def name(self) -> str | None:
         return self._name
 
     @name.setter
     def name(self, value: str | None) -> None:
@@ -1242,15 +1242,15 @@
 ) -> None:
     """Check if a node is safe to remove.
 
     1. It checks to make sure there are no users of the node that are not
         to be removed before removing it.
     2. It checks the node does not contribute to any graph outputs.
 
-    This check is typically O(1) assuming the number of consumers of the node is small
+    This check is typically O(1) assuming the number of uses of the node is small
 
     Args:
         node: The node to check.
         to_remove: A set of nodes that are to be removed.
             This set is used to check if the node is still being used by other
             nodes that are not to be removed.
         graph_outputs: A set of values that are outputs of the graph.
@@ -1260,20 +1260,20 @@
         ValueError: If the node is still being used by other nodes not to be removed.
     """
     for output in node.outputs:
         if output in graph_outputs:
             raise ValueError(
                 f"Node '{node!r}' is still an output of the graph and cannot be removed when safe=True."
             )
-        for consumer, _ in output.consumers():
-            if consumer in to_remove:
+        for use, _ in output.uses():
+            if use in to_remove:
                 continue
             raise ValueError(
-                f"Node '{consumer!r}' is still being used by other nodes that are not to be "
-                f"removed. All of its uses: {list(output.consumers())!r}"
+                f"Node '{use!r}' is still being used by other nodes that are not to be "
+                f"removed. All of its uses: {list(output.uses())!r}"
             )
 
 
 class Graph(_protocols.GraphProtocol, Sequence[Node], _display.PrettyPrintable):
     """IR Graph.
 
     Graph represents a computation graph. In addition to the ONNX specification
```

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/ir/_display.py` & `onnxscript-0.1.0.dev20240424/onnxscript/ir/_display.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/ir/_enums.py` & `onnxscript-0.1.0.dev20240424/onnxscript/ir/_enums.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/ir/_graph_comparison.py` & `onnxscript-0.1.0.dev20240424/onnxscript/ir/_graph_comparison.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/ir/_invariants.py` & `onnxscript-0.1.0.dev20240424/onnxscript/ir/_invariants.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/ir/_linked_list.py` & `onnxscript-0.1.0.dev20240424/onnxscript/ir/_linked_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,15 @@
     Values need to be hashable. ``None`` is not a valid value in the set.
     """
 
     __slots__ = ("_root", "_length", "_value_ids_to_boxes")
 
     def __init__(self, values: Iterable[T] | None = None) -> None:
         # Using the root node simplifies the mutation implementation a lot
+        # The list is circular. The root node is the only node that is not a part of the list values
         root_ = _LinkBox(self, None)
         self._root: _LinkBox = root_
         self._length = 0
         self._value_ids_to_boxes: dict[int, _LinkBox] = {}
         if values is not None:
             self.extend(values)
```

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/ir/_metadata.py` & `onnxscript-0.1.0.dev20240424/onnxscript/ir/_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/ir/_name_authority.py` & `onnxscript-0.1.0.dev20240424/onnxscript/ir/_name_authority.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/ir/_protocols.py` & `onnxscript-0.1.0.dev20240424/onnxscript/ir/_protocols.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
     are ``None``.
 
     When the value is owned by a node, it is an output of the node.
     The node that produces the value can be accessed with :meth:`producer`.
     The index of the output of the node that produces the value can be accessed with
     :meth:`index`.
 
-    To find all the nodes that use this value as an input, call :meth:`consumers`.
+    To find all the nodes that use this value as an input, call :meth:`uses`.
 
     To check if the value is an output of a graph, call :meth:`is_graph_output`.
 
     Attributes:
         name: The name of the value. A value is always named when it is part of a graph.
         shape: The shape of the value.
         type: The type of the value.
@@ -159,15 +159,15 @@
         """The node that produces this value."""
         ...
 
     def index(self) -> int | None:
         """The index of the output of the node that produces this value."""
         ...
 
-    def consumers(self) -> Collection[tuple[NodeProtocol, int]]:
+    def uses(self) -> Collection[tuple[NodeProtocol, int]]:
         """The set of (node, input_index) with node being those that use this value as an input."""
         ...
 
     def is_graph_output(self) -> bool:
         """Whether this value is an output of a graph."""
         ...
```

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/ir/serde.py` & `onnxscript-0.1.0.dev20240424/onnxscript/ir/serde.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/irbuilder.py` & `onnxscript-0.1.0.dev20240424/onnxscript/irbuilder.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/main.py` & `onnxscript-0.1.0.dev20240424/onnxscript/main.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/__init__.py` & `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset1.py` & `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset10.py` & `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset10.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset11.py` & `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset11.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset12.py` & `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset12.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset13.py` & `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset13.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset14.py` & `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset14.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset15.py` & `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset15.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset16.py` & `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset16.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset17.py` & `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset17.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset18.py` & `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset18.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset19.py` & `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset19.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset2.py` & `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset20.py` & `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset20.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset3.py` & `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset4.py` & `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset5.py` & `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset5.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset6.py` & `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset6.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset7.py` & `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset7.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset8.py` & `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset8.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset9.py` & `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset9.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py` & `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py` & `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py` & `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py` & `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py` & `onnxscript-0.1.0.dev20240424/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/onnx_types.py` & `onnxscript-0.1.0.dev20240424/onnxscript/onnx_types.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/optimizer/__init__.py` & `onnxscript-0.1.0.dev20240424/onnxscript/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/optimizer/constant_folding.py` & `onnxscript-0.1.0.dev20240424/onnxscript/optimizer/constant_folding.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/optimizer/copy_propagation.py` & `onnxscript-0.1.0.dev20240424/onnxscript/optimizer/copy_propagation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/optimizer/evaluator.py` & `onnxscript-0.1.0.dev20240424/onnxscript/optimizer/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/optimizer/fold_constants_v0.py` & `onnxscript-0.1.0.dev20240424/onnxscript/optimizer/fold_constants_v0.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/optimizer/remove_unused.py` & `onnxscript-0.1.0.dev20240424/onnxscript/optimizer/remove_unused.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/optimizer/remove_unused_function.py` & `onnxscript-0.1.0.dev20240424/onnxscript/optimizer/remove_unused_function.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/optimizer/simple_function_folding.py` & `onnxscript-0.1.0.dev20240424/onnxscript/optimizer/simple_function_folding.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/rewriter/__init__.py` & `onnxscript-0.1.0.dev20240424/onnxscript/rewriter/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,21 +21,19 @@
 
 
 def rewrite(
     model: onnx.ModelProto,
     function_rewrite_rules: Sequence[type[FunctionRewriteRule]] = (),
     pattern_rewrite_rules: Sequence[PatternRewriteRule] = (),
 ) -> onnx.ModelProto:
-    print(f"len(value_info): {len(model.graph.value_info)}")
     model_ir = ir.serde.deserialize_model(model)
     if function_rewrite_rules:
         for rule_cls in function_rewrite_rules:
             count, model_ir = rule_cls().apply_to_model(model_ir)
             print(f"Applied {count} of onnxruntime specific function rewrite rules.")
     if pattern_rewrite_rules:
         count = pattern.RewriteRuleSet(pattern_rewrite_rules).apply_to_model(model_ir)
         print(f"Applied {count} of general pattern rewrite rules.")
     model = ir.serde.serialize_model(model_ir)
     remove_unused.remove_unused_nodes(model)
     remove_unused_function.remove_unused_functions(model)
-    print(f"len(value_info): {len(model.graph.value_info)}")
     return model
```

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/rewriter/_ir_utils.py` & `onnxscript-0.1.0.dev20240424/onnxscript/rewriter/_ir_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/rewriter/_tape.py` & `onnxscript-0.1.0.dev20240424/onnxscript/rewriter/_tape.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/rewriter/broadcast_to_matmul.py` & `onnxscript-0.1.0.dev20240424/onnxscript/rewriter/broadcast_to_matmul.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/rewriter/cast_constant_of_shape.py` & `onnxscript-0.1.0.dev20240424/onnxscript/rewriter/cast_constant_of_shape.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/rewriter/erfgelu.py` & `onnxscript-0.1.0.dev20240424/onnxscript/rewriter/erfgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/rewriter/function_rule.py` & `onnxscript-0.1.0.dev20240424/onnxscript/rewriter/function_rule.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 import functools
 import logging
+from typing import Callable
 
 import onnx
 from packaging import version
 
 import onnxscript
 from onnxscript import ir
-from onnxscript._legacy_ir import visitor
 from onnxscript.rewriter import pattern
 
 logger = logging.getLogger(__name__)
 
 
 class FunctionRewriteError(RuntimeError): ...
 
@@ -34,15 +34,15 @@
 MIN_VERSION = version.parse("0")
 MAX_VERSION = version.parse("9999")
 
 
 class VersionController:
     def __init__(self):
         # A dispatch table for rewrite implementation based on the function package version.
-        self.dispatch_table: dict[tuple[version.Version, version.Version], callable] = {}
+        self.dispatch_table: dict[tuple[version.Version, version.Version], Callable] = {}
 
     def register_version(
         self,
         min_version: version.Version | str | None = None,
         max_version: version.Version | str | None = None,
     ):
         """Register a function implementation for a specific package version range [min_version, max_version).
@@ -62,15 +62,15 @@
 
         def deco(func):
             self.dispatch_table[(min_version, max_version)] = func
             return func
 
         return deco
 
-    def dispatch(self, version: version.Version | None) -> callable | None:
+    def dispatch(self, version: version.Version | None) -> Callable | None:
         if version is None:
             if len(self.dispatch_table) == 1:
                 return next(iter(self.dispatch_table.values()))
             raise ValueError(
                 "No function package version specified, however there are multiple "
                 f"fusion rules based on package version: {self.dispatch_table.keys()}."
             )
@@ -90,32 +90,30 @@
     """The package name to match.
 
     For example, 'transformers' to match for domain name 'pkg.transformers.4.36.2'.
     """
 
     _opset_imports: dict[str, int]
     onnx_opset: onnxscript.values.Opset
-    _function_shape_env: visitor.FunctionShapeEnv
 
-    def __init__(self, opset: onnxscript.values.Opset = onnxscript.opset18) -> None:
+    def __init__(self, opset: onnxscript.values.Opset = onnxscript.opset18) -> None:  # type: ignore[has-type]
         self.onnx_opset = opset
 
-    def _match_function(self, function: onnx.FunctionProto, pkg_name: str) -> bool:
+    def _match_function(self, function: ir.Function, pkg_name: str) -> bool:
         # TODO: Consolidate more checks from `compose_new_function` to here.
         if pkg_name != self.PACKAGE_NAME:
             logger.info(
                 "Rule %s did not match function %s::%s. Package name mismatch '%s' != '%s'.",
                 self.__class__.__name__,
                 function.domain,
                 function.name,
                 self.PACKAGE_NAME,
                 pkg_name,
             )
             return False
-
         if isinstance(self.FUNCTION_KEYWORD, str):
             return function.name.find(self.FUNCTION_KEYWORD) != -1
         elif isinstance(self.FUNCTION_KEYWORD, tuple):
             return any(function.name.find(keyword) != -1 for keyword in self.FUNCTION_KEYWORD)
         else:
             raise ValueError(  # noqa: TRY004
                 f"Function keyword must be str or tuple, got {self.FUNCTION_KEYWORD}"
@@ -126,119 +124,107 @@
     ) -> onnx.NodeProto | None:
         for node in function.node:
             if node.name.find(keyword) != -1:
                 return node
         return None
 
     def _find_node_by_type(
-        self, function: onnx.FunctionProto, domain: str, op_type: str
-    ) -> onnx.NodeProto | None:
+        self, function: ir.Function, domain: str, op_type: str
+    ) -> ir.Node | None:
         # Repeat
-        for node in function.node:
+        for node in function:
             if node.domain == domain and node.op_type == op_type:
                 return node
         return None
 
-    def _find_constant_node(
-        self, function: onnx.FunctionProto, value_name: str
-    ) -> onnx.NodeProto | None:
-        # Potentially repeat, utility function.
-        for node in function.node:
-            for output in node.output:
-                if output == value_name:
-                    return node
-        return None
-
     def compose_new_function(
-        self, old_function: onnx.FunctionProto, pkg_version: version.Version | None
-    ) -> tuple[onnx.FunctionProto, tuple[onnx.OperatorSetIdProto]]:
+        self, old_function: ir.Function, pkg_version: version.Version | None
+    ) -> ir.Function:
         """Compose a new function from the old function.
 
         Returns:
             A tuple of the new function and the opset imports.
 
         Raises:
             FunctionRewriteError: If the rewrite fails.
         """
-        func = self._version_controller.dispatch(pkg_version)
+        # self._version_controller is created in the subclass
+        func = self._version_controller.dispatch(pkg_version)  # type: ignore[attr-defined]
         if func is not None:
-            return func(self, old_function)
+            new_function = func(self, old_function)
+            return new_function
         raise FunctionRewriteError(
             f"No rewrite implementation for package version {pkg_version}."
         )
 
     def try_rewrite_function(
-        self, function: onnx.FunctionProto, model: onnx.ModelProto
-    ) -> bool:
+        self, function: ir.Function
+    ) -> tuple[ir.OperatorIdentifier, ir.Function] | None:
         try:
             pkg_name, pkg_version = parse_domain(function.domain)
         except FunctionRewriteError as e:
             logger.warning("Could not parse domain: %s", e)
-            return False
+            return None
 
         if pkg_version is None and not pkg_name.startswith("onnxscript"):
             logger.warning(
                 "Could not parse version for domain of function %s::%s. "
                 "Usually this implies the model source is not from a package, but from arbitrary python files instead. "
                 "For example, models not defined in huggingface/transformers but loaded via 'trust_remote_code=True'.",
                 function.domain,
                 function.name,
             )
 
         if not self._match_function(function, pkg_name):
-            return False
+            return None
         logger.info(
             "Rule %s matched function %s::%s",
             self.__class__.__name__,
             function.domain,
             function.name,
         )
-
         try:
-            new_function, opset_imports = self.compose_new_function(function, pkg_version)
+            new_function = self.compose_new_function(function, pkg_version)
         except FunctionRewriteError as e:
             logger.warning("Could not rewrite function: %s", e)
-            return False
+            return None
 
-        nodes = new_function.node
+        new_function.name = function.name
+        new_function.domain = function.domain
 
-        del function.input[:]
-        function.input.extend(new_function.input)
-        del function.output[:]
-        function.output.extend(new_function.output)
-
-        del function.node[:]
-        function.node.extend(nodes)
-        for new_opset in opset_imports:
-            function.opset_import.append(new_opset)
-            if new_opset.domain not in self._opset_imports:
-                model.opset_import.append(new_opset)
-        return True
+        return function.identifier(), new_function
 
     def try_rewrite(self, model: ir.Model, value) -> bool:
         raise NotImplementedError(
             "Use `try_rewrite_function` instead for function based rewrites."
         )
 
-    def lookup(self, function: onnx.FunctionProto, value_name: str) -> ir.Value | None:
-        return self._function_shape_env.lookup(function, value_name)
-
     def apply_to_model(
         self, model: ir.Model, *, commute: bool = False
     ) -> tuple[int, ir.Model]:
         del commute  # unused
-        model_proto: onnx.ModelProto = ir.serde.serialize_model(model)
-        self._function_shape_env = visitor.FunctionShapeEnv()
-        self._function_shape_env.load_from_model_proto(model_proto)
-        self._opset_imports = {x.domain: x.version for x in model_proto.opset_import}
-
-        rewrite_count = 0
-        for function in model_proto.functions:
-            rewrite_count += self.try_rewrite_function(function, model_proto)
-        model = ir.serde.deserialize_model(model_proto)
-        return rewrite_count, model
+
+        old_function_to_new_function: dict[ir.OperatorIdentifier, ir.Function] = {}
+        for function in model.functions.values():
+            rewrite_or_none = self.try_rewrite_function(function)
+            if rewrite_or_none is not None:
+                old_function_to_new_function[rewrite_or_none[0]] = rewrite_or_none[1]
+        model = self.update_to_new_function(model, old_function_to_new_function)
+        return len(old_function_to_new_function), model
+
+    def update_to_new_function(
+        self,
+        model: ir.Model,
+        old_function_to_new_function: dict[ir.OperatorIdentifier, ir.Function],
+    ) -> ir.Model:
+        for old_function_id, new_function_ir in old_function_to_new_function.items():
+            model.functions[old_function_id] = new_function_ir
+            for new_opset, opset_version in new_function_ir.opset_imports.items():
+                if new_opset not in model.opset_imports:
+                    model.opset_imports[new_opset] = opset_version
+        return model
 
     def count_matches(self, model, *, commute: bool = False) -> int:
         raise NotImplementedError()
 
     def commute(self) -> list[pattern.RewriteRule]:
         raise NotImplementedError()
```

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/rewriter/gemm_to_matmul_add.py` & `onnxscript-0.1.0.dev20240424/onnxscript/rewriter/gemm_to_matmul_add.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/rewriter/generic_pattern.py` & `onnxscript-0.1.0.dev20240424/onnxscript/rewriter/generic_pattern.py`

 * *Files 0% similar despite different names*

```diff
@@ -501,16 +501,16 @@
                 pattern_node,
                 "-- model",
                 graph_node,
             )
             return self.none(root_node, inspect.currentframe().f_lineno)
 
         for o, op in zip(graph_node.outputs, pattern_node.outputs):
-            graph_node_users = [user for user, _ in o.consumers()]
-            pattern_node_users = [user for user, _ in op.consumers()]
+            graph_node_users = [user for user, _ in o.uses()]
+            pattern_node_users = [user for user, _ in op.uses()]
             if not pattern_node_users:
                 # The pattern has no node forward, the matching stops.
                 continue
             if len(graph_node_users) < len(pattern_node_users):
                 # Not enough node in the graph to match the pattern. A match is not possible
                 return self.none(root_node, inspect.currentframe().f_lineno)
```

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/rewriter/no_op.py` & `onnxscript-0.1.0.dev20240424/onnxscript/rewriter/no_op.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/rewriter/onnxruntime/__init__.py` & `onnxscript-0.1.0.dev20240424/onnxscript/rewriter/onnxruntime/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py` & `onnxscript-0.1.0.dev20240424/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py` & `onnxscript-0.1.0.dev20240424/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/rewriter/onnxruntime/softmax.py` & `onnxscript-0.1.0.dev20240424/onnxscript/rewriter/onnxruntime/softmax.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/rewriter/onnxruntime/transformers/__init__.py` & `onnxscript-0.1.0.dev20240424/onnxscript/rewriter/onnxruntime/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py` & `onnxscript-0.1.0.dev20240424/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 from __future__ import annotations
 
 import logging
 
-import onnx
-
 import onnxscript
+from onnxscript import ir
 from onnxscript.rewriter import function_rule
 
 logger = logging.getLogger(__name__)
 
 
 class GeluRewriteRule(function_rule.FunctionRewriteRule):
     FUNCTION_KEYWORD = "GELUActivation"
     PACKAGE_NAME = "transformers"
     _version_controller = function_rule.VersionController()
 
     @_version_controller.register_version()
-    def _fusion(
-        self, function: onnx.FunctionProto
-    ) -> tuple[onnx.FunctionProto, list[onnx.OperatorSetIdProto]]:
+    def _fusion(self, function: ir.Function) -> ir.Function:
         del function  # Unused
         op = self.onnx_opset
         msft_opset = onnxscript.values.Opset("com.microsoft", 1)
 
         def gelu(input):
             return msft_opset.FastGelu(input)
 
-        return onnxscript.script(default_opset=op)(gelu).to_function_proto(), (
-            onnx.helper.make_operatorsetid("com.microsoft", 1),
-        )
+        function_proto = onnxscript.script(default_opset=op)(gelu).to_function_proto()
+        return ir.serde.deserialize_function(function_proto)
```

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/rewriter/onnxruntime/transformers/layernorm.py` & `onnxscript-0.1.0.dev20240424/onnxscript/rewriter/onnxruntime/transformers/layernorm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,42 @@
 from __future__ import annotations
 
 import logging
 
-import onnx
-from onnx import numpy_helper
-
 import onnxscript
-from onnxscript.rewriter import function_rule
+from onnxscript import ir
+from onnxscript.rewriter import _ir_utils, function_rule
 
 logger = logging.getLogger(__name__)
 
 
 class LNRewriteRule(function_rule.FunctionRewriteRule):
     FUNCTION_KEYWORD = "layernorm"
     PACKAGE_NAME = "transformers"
     _version_controller = function_rule.VersionController()
 
     @_version_controller.register_version()
-    def _fusion(  # type: ignore[misc]
-        self, function: onnx.FunctionProto
-    ) -> tuple[onnx.FunctionProto, list[onnx.OperatorSetIdProto]]:
+    def _fusion(self, function: ir.Function) -> ir.Function:
         # TODO(bowbao): Might be more desirable to annotate as attribute in nn.Module
         aten_add_node = self._find_node_by_type(function, "", "Add")
         if aten_add_node is None:
             raise function_rule.FunctionRewriteError("Could not find Add node")
 
-        eps_node = self._find_constant_node(function, aten_add_node.input[1])
-        if eps_node is None:
-            raise function_rule.FunctionRewriteError("Could not find eps node")
-
-        eps = numpy_helper.to_array(eps_node.attribute[0].t).item()
+        eps_ir_value = _ir_utils.propagate_const_value(aten_add_node.inputs[1])
+        eps_numpy_value = _ir_utils.get_numpy_from_ir_value(eps_ir_value)
+        if eps_numpy_value is None:
+            raise function_rule.FunctionRewriteError("Could not find eps")
+        eps = eps_numpy_value.item()
         logger.info("eps: %s", eps)
 
         # TODO(ORT): SimplifiedLayerNormalization in ort is defined under onnx domain.
         # https://github.com/microsoft/onnxruntime/issues/7573
         # msft_op = onnxscript.values.Opset("com.microsoft", 1)
         op = self.onnx_opset
 
         def ln(input, weight):
             return op.SimplifiedLayerNormalization(
                 input, weight, axis=-1, epsilon=eps, stash_type=1
             )
 
-        return onnxscript.script(default_opset=op)(ln).to_function_proto(), []
+        function_proto = onnxscript.script(default_opset=op)(ln).to_function_proto()
+        return ir.serde.deserialize_function(function_proto)
```

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py` & `onnxscript-0.1.0.dev20240424/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,45 +50,42 @@
 import dataclasses
 import logging
 
 import onnx
 from onnx import helper as onnx_helper
 
 import onnxscript
+from onnxscript import ir
 from onnxscript.rewriter import function_rule
 
 logger = logging.getLogger(__name__)
 
 
 @dataclasses.dataclass
 class AttnSizeConfig:
     num_attention_heads: int
     num_key_value_heads: int
     head_size: int
     hidden_size: int
 
 
 class AttentionRewriteRule(function_rule.FunctionRewriteRule, abc.ABC):
-    def infer_attn_size_config(self, function: onnx.FunctionProto) -> AttnSizeConfig:
-        if len(function.output) != 3:
+    def infer_attn_size_config(self, function: ir.Function) -> AttnSizeConfig:
+        if len(function.outputs) != 3:
             raise function_rule.FunctionRewriteError(
-                f"Unexpected number of outputs. Expected 3, got {len(function.output)}."
+                f"Unexpected number of outputs. Expected 3, got {len(function.outputs)}."
             )
-        present_value, _, attn_output = function.output
-        if (
-            present_value_ir := self.lookup(function, present_value)
-        ) is None or present_value_ir.shape is None:
+        present_value, _, attn_output = function.outputs
+        if present_value.shape is None:
             raise function_rule.FunctionRewriteError("Failed to find shape for present_value.")
-        if (
-            attn_output_ir := self.lookup(function, attn_output)
-        ) is None or attn_output_ir.shape is None:
+        if attn_output.shape is None:
             raise function_rule.FunctionRewriteError("Failed to find shape for attn_output.")
-        head_size = present_value_ir.shape[3]
-        num_key_value_heads = present_value_ir.shape[1]
-        hidden_size = attn_output_ir.shape[2]
+        head_size = present_value.shape[3]
+        num_key_value_heads = present_value.shape[1]
+        hidden_size = attn_output.shape[2]
         num_attention_heads = hidden_size // head_size
         return AttnSizeConfig(
             num_attention_heads=num_attention_heads,
             num_key_value_heads=num_key_value_heads,
             head_size=head_size,
             hidden_size=hidden_size,
         )
@@ -99,17 +96,15 @@
     PACKAGE_NAME = "transformers"
     _version_controller = function_rule.VersionController()
 
     def __init__(self) -> None:
         super().__init__()
 
     @_version_controller.register_version(min_version="4.33", max_version="4.36")
-    def _fusion_with_4d_cache(
-        self, function: onnx.FunctionProto
-    ) -> tuple[onnx.FunctionProto, tuple[onnx.OperatorSetIdProto]]:
+    def _fusion_with_4d_cache(self, function: ir.Function) -> ir.Function:
         if len(function.input) != 9:
             raise function_rule.FunctionRewriteError(
                 f"Unexpected number of inputs. Expected 9, got {len(function.input)}."
             )
 
         # Infer size configurations from the function.
         attn_size_config = self.infer_attn_size_config(function)
@@ -163,22 +158,21 @@
                 None,
                 expanded_mask,
                 num_heads=attn_size_config.num_attention_heads,
             )
             attn_output = op.MatMul(mha_output, op.Transpose(o_proj_weight, [1, 0]))
             return present_value, present_key, attn_output
 
-        return onnxscript.script(default_opset=onnxscript.opset18)(mha).to_function_proto(), (
-            onnx.helper.make_operatorsetid("com.microsoft", 1),
-        )
+        function_proto = onnxscript.script(default_opset=onnxscript.opset18)(
+            mha
+        ).to_function_proto()
+        return ir.serde.deserialize_function(function_proto)
 
     @_version_controller.register_version(min_version="4.36", max_version="4.38")
-    def _fusion_with_2d_cache(
-        self, function: onnx.FunctionProto
-    ) -> tuple[onnx.FunctionProto, tuple[onnx.OperatorSetIdProto]]:
+    def _fusion_with_2d_cache(self, function: ir.Function) -> ir.Function:
         # Infer size configurations from the function.
         attn_size_config = self.infer_attn_size_config(function)
 
         if len(function.input) != 9:
             raise function_rule.FunctionRewriteError(
                 f"Unexpected number of inputs. Expected 9, got {len(function.input)}."
             )
@@ -225,34 +219,33 @@
                 None,
                 expanded_mask,
                 num_heads=attn_size_config.num_attention_heads,
             )
             attn_output = op.MatMul(mha_output, op.Transpose(o_proj_weight, [1, 0]))
             return present_value, present_key, attn_output
 
-        return onnxscript.script(default_opset=onnxscript.opset18)(mha).to_function_proto(), (
-            onnx.helper.make_operatorsetid("com.microsoft", 1),
-        )
+        function_proto = onnxscript.script(default_opset=onnxscript.opset18)(
+            mha
+        ).to_function_proto()
+        return ir.serde.deserialize_function(function_proto)
 
 
 class GQALlama2RewriteRule(AttentionRewriteRule):
     FUNCTION_KEYWORD = "LlamaAttention"
     PACKAGE_NAME = "transformers"
     _version_controller = function_rule.VersionController()
 
     def __init__(self) -> None:
         super().__init__()
 
     @_version_controller.register_version(min_version="4.33", max_version="4.36")
-    def _fusion_with_4d_cache(
-        self, function: onnx.FunctionProto
-    ) -> tuple[onnx.FunctionProto, tuple[onnx.OperatorSetIdProto]]:
-        if len(function.input) != 9:
+    def _fusion_with_4d_cache(self, function: ir.Function) -> ir.Function:
+        if len(function.inputs) != 9:
             raise function_rule.FunctionRewriteError(
-                f"Unexpected number of inputs. Expected 9, got {len(function.input)}."
+                f"Unexpected number of inputs. Expected 9, got {len(function.inputs)}."
             )
 
         # Infer size configurations from the function.
         attn_size_config = self.infer_attn_size_config(function)
 
         # Code new pattern with onnxscript.
         op = onnxscript.opset18
@@ -305,28 +298,27 @@
                 total_seq_lengths,
                 kv_num_heads=attn_size_config.num_key_value_heads,
                 num_heads=attn_size_config.num_attention_heads,
             )
             attn_output = op.MatMul(gqa_output, op.Transpose(o_proj_weight, [1, 0]))
             return present_value, present_key, attn_output
 
-        return onnxscript.script(default_opset=onnxscript.opset18)(gqa).to_function_proto(), (
-            onnx.helper.make_operatorsetid("com.microsoft", 1),
-        )
+        function_proto = onnxscript.script(default_opset=onnxscript.opset18)(
+            gqa
+        ).to_function_proto()
+        return ir.serde.deserialize_function(function_proto)
 
     @_version_controller.register_version(min_version="4.36", max_version="4.38")
-    def _fusion_with_2d_cache(
-        self, function: onnx.FunctionProto
-    ) -> tuple[onnx.FunctionProto, tuple[onnx.OperatorSetIdProto]]:
+    def _fusion_with_2d_cache(self, function: ir.Function) -> ir.Function:
         # Infer size configurations from the function.
         attn_size_config = self.infer_attn_size_config(function)
 
-        if len(function.input) != 9:
+        if len(function.inputs) != 9:
             raise function_rule.FunctionRewriteError(
-                f"Unexpected number of inputs. Expected 9, got {len(function.input)}."
+                f"Unexpected number of inputs. Expected 9, got {len(function.inputs)}."
             )
 
         # Code new pattern with onnxscript.
         op = onnxscript.opset18
         msft_op = onnxscript.values.Opset("com.microsoft", 1)
 
         # Workaround onnxscript error by specifying the output shape here.
@@ -373,17 +365,18 @@
                 total_seq_lengths,
                 kv_num_heads=attn_size_config.num_key_value_heads,
                 num_heads=attn_size_config.num_attention_heads,
             )
             attn_output = op.MatMul(gqa_output, op.Transpose(o_proj_weight, [1, 0]))
             return present_value, present_key, attn_output
 
-        return onnxscript.script(default_opset=onnxscript.opset18)(gqa).to_function_proto(), (
-            onnx.helper.make_operatorsetid("com.microsoft", 1),
-        )
+        function_proto = onnxscript.script(default_opset=onnxscript.opset18)(
+            gqa
+        ).to_function_proto()
+        return ir.serde.deserialize_function(function_proto)
 
 
 class GQALlamaSdpa2RewriteRule(AttentionRewriteRule):
     # TODO: There are a lot of duplicated code with `MHALlama2RewriteRule`.
     # The pitfall is that the source function signature is slightly different.
     # One has `attention_mask` as input while the other does not.
     # Possibly designing a function template system could help reduce the boilerplate.
@@ -391,17 +384,15 @@
     PACKAGE_NAME = "transformers"
     _version_controller = function_rule.VersionController()
 
     def __init__(self) -> None:
         super().__init__()
 
     @_version_controller.register_version(min_version="4.36", max_version="4.38")
-    def _fusion(
-        self, function: onnx.FunctionProto
-    ) -> tuple[onnx.FunctionProto, tuple[onnx.OperatorSetIdProto]]:
+    def _fusion(self, function: ir.Function) -> ir.Function:
         # Infer size configurations from the function.
         attn_size_config = self.infer_attn_size_config(function)
 
         # Code new pattern with onnxscript.
         op = onnxscript.opset18
         msft_op = onnxscript.values.Opset("com.microsoft", 1)
 
@@ -447,22 +438,21 @@
                 total_seq_lengths,
                 kv_num_heads=attn_size_config.num_key_value_heads,
                 num_heads=attn_size_config.num_attention_heads,
             )
             attn_output = op.MatMul(gqa_output, op.Transpose(o_proj_weight, [1, 0]))
             return present_value, present_key, attn_output
 
-        return onnxscript.script(default_opset=onnxscript.opset18)(
-            gqa,
-        ).to_function_proto(), (onnx.helper.make_operatorsetid("com.microsoft", 1),)
+        function_proto = onnxscript.script(default_opset=onnxscript.opset18)(
+            gqa
+        ).to_function_proto()
+        return ir.serde.deserialize_function(function_proto)
 
     @_version_controller.register_version(min_version="4.38")
-    def _fusion_without_cos_sin_cache(
-        self, function: onnx.FunctionProto
-    ) -> tuple[onnx.FunctionProto, tuple[onnx.OperatorSetIdProto]]:
+    def _fusion_without_cos_sin_cache(self, function: ir.Function) -> ir.Function:
         # Infer size configurations from the function.
         attn_size_config = self.infer_attn_size_config(function)
 
         # Code new pattern with onnxscript.
         op = onnxscript.opset18
         msft_op = onnxscript.values.Opset("com.microsoft", 1)
 
@@ -523,31 +513,30 @@
                 total_seq_lengths,
                 kv_num_heads=attn_size_config.num_key_value_heads,
                 num_heads=attn_size_config.num_attention_heads,
             )
             attn_output = op.MatMul(gqa_output, op.Transpose(o_proj_weight, [1, 0]))
             return present_value, present_key, attn_output
 
-        return onnxscript.script(default_opset=onnxscript.opset18)(
-            gqa,
-        ).to_function_proto(), (onnx.helper.make_operatorsetid("com.microsoft", 1),)
+        function_proto = onnxscript.script(default_opset=onnxscript.opset18)(
+            gqa
+        ).to_function_proto()
+        return ir.serde.deserialize_function(function_proto)
 
 
 class AttnPhi15RewriteRule(AttentionRewriteRule):
     FUNCTION_KEYWORD = "PhiAttention"
     PACKAGE_NAME = "transformers_modules"
     _version_controller = function_rule.VersionController()
 
     def __init__(self) -> None:
         super().__init__()
 
     @_version_controller.register_version()
-    def _fusion(
-        self, function: onnx.FunctionProto
-    ) -> tuple[onnx.FunctionProto, tuple[onnx.OperatorSetIdProto]]:
+    def _fusion(self, function: ir.Function) -> ir.Function:
         # Infer size configurations from the function.
         attn_size_config = self.infer_attn_size_config(function)
 
         # Code new pattern with onnxscript.
         op = onnxscript.opset18
         msft_opset = onnxscript.values.Opset("com.microsoft", 1)
 
@@ -595,10 +584,11 @@
             present_value = op.Gather(present, 1)
             output = op.Add(
                 op.MatMul(attn_output, op.Transpose(dense_weight, [1, 0])), dense_bias
             )
 
             return present_value, present_key, output
 
-        return onnxscript.script(default_opset=onnxscript.opset18)(
+        function_proto = onnxscript.script(default_opset=onnxscript.opset18)(
             phi_attention
-        ).to_function_proto(), (onnx.helper.make_operatorsetid("com.microsoft", 1),)
+        ).to_function_proto()
+        return ir.serde.deserialize_function(function_proto)
```

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/rewriter/pattern.py` & `onnxscript-0.1.0.dev20240424/onnxscript/rewriter/pattern.py`

 * *Files 1% similar despite different names*

```diff
@@ -776,15 +776,15 @@
     # (intermediate) values. (Not necessary for now. Guaranteed.)
     deleted_nodes = matched_nodes[:-1]
     for n in deleted_nodes:
         for v in n.outputs:
             if v.is_graph_output():
                 # value is an output-value of the graph/function.
                 return False
-            for consumer, _ in v.consumers():
+            for consumer, _ in v.uses():
                 if consumer not in matched_nodes:
                     return False
     return True
 
 
 class TargetPatternFunction:
     """The targeted pattern that will be replaced by the replacement pattern.
```

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/sourceinfo.py` & `onnxscript-0.1.0.dev20240424/onnxscript/sourceinfo.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/tensor.py` & `onnxscript-0.1.0.dev20240424/onnxscript/tensor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/testing/__init__.py` & `onnxscript-0.1.0.dev20240424/onnxscript/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/type_annotation.py` & `onnxscript-0.1.0.dev20240424/onnxscript/type_annotation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/utils/evaluation_utils.py` & `onnxscript-0.1.0.dev20240424/onnxscript/utils/evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/utils/timing_utils.py` & `onnxscript-0.1.0.dev20240424/onnxscript/utils/timing_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/utils/utils.py` & `onnxscript-0.1.0.dev20240424/onnxscript/utils/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript/values.py` & `onnxscript-0.1.0.dev20240424/onnxscript/values.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript.egg-info/PKG-INFO` & `onnxscript-0.1.0.dev20240424/onnxscript.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240423
+Version: 0.1.0.dev20240424
 Summary: Naturally author ONNX functions and models using a subset of Python
-Home-page: https://onnxscript.ai/
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `onnxscript-0.1.0.dev20240423/onnxscript.egg-info/SOURCES.txt` & `onnxscript-0.1.0.dev20240424/onnxscript.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/pyproject.toml` & `onnxscript-0.1.0.dev20240424/pyproject.toml`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240423/setup.py` & `onnxscript-0.1.0.dev20240424/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 # Logic for computing the development version number.
 ROOT_DIR = pathlib.Path(__file__).parent
 VERSION_FILE = ROOT_DIR / "VERSION"
 version = VERSION_FILE.read_text().strip()
 
 project_urls = {
+    "Homepage": "https://onnxscript.ai/",
     "Repository": "https://github.com/microsoft/onnxscript",
 }
 if os.environ.get("ONNX_SCRIPT_RELEASE") != "1":
     date = datetime.date.today().strftime("%Y%m%d")
     version = f"{version}.dev{date}"
 
     commit_hash_cmd = subprocess.run(
@@ -28,8 +29,8 @@
     )
     if commit_hash_cmd.returncode == 0:
         project_urls["Commit"] = (
             f"https://github.com/microsoft/onnxscript/tree/{commit_hash_cmd.stdout.decode('utf-8').strip()}"
         )
 
 # NOTE: Do not include other metadata in setup.py. Put it in pyproject.toml.
-setuptools.setup(version=version, project_urls=project_urls, url="https://onnxscript.ai/")
+setuptools.setup(version=version, project_urls=project_urls)
```

