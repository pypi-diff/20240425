# Comparing `tmp/vellum_ai-0.3.9.tar.gz` & `tmp/vellum_ai-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vellum_ai-0.3.9.tar", max compression
+gzip compressed data, was "vellum_ai-0.5.0.tar", max compression
```

## Comparing `vellum_ai-0.3.9.tar` & `vellum_ai-0.5.0.tar`

### file list

```diff
@@ -1,311 +1,382 @@
--rw-r--r--   0        0        0     1073 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/LICENSE
--rw-r--r--   0        0        0     2980 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/README.md
--rw-r--r--   0        0        0      401 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/pyproject.toml
--rw-r--r--   0        0        0    27647 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/__init__.py
--rw-r--r--   0        0        0    61957 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/client.py
--rw-r--r--   0        0        0      519 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/core/__init__.py
--rw-r--r--   0        0        0      426 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/core/api_error.py
--rw-r--r--   0        0        0     1212 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/core/datetime_utils.py
--rw-r--r--   0        0        0     3799 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      498 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/environment.py
--rw-r--r--   0        0        0      402 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/errors/__init__.py
--rw-r--r--   0        0        0      248 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/errors/bad_request_error.py
--rw-r--r--   0        0        0      327 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/errors/conflict_error.py
--rw-r--r--   0        0        0      247 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/errors/forbidden_error.py
--rw-r--r--   0        0        0      252 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/errors/internal_server_error.py
--rw-r--r--   0        0        0      246 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/errors/not_found_error.py
--rw-r--r--   0        0        0        0 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/py.typed
--rw-r--r--   0        0        0      675 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/__init__.py
--rw-r--r--   0        0        0      157 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/deployments/__init__.py
--rw-r--r--   0        0        0    10752 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/deployments/client.py
--rw-r--r--   0        0        0      183 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/deployments/types/__init__.py
--rw-r--r--   0        0        0      518 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/deployments/types/deployments_list_request_status.py
--rw-r--r--   0        0        0       65 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/document_indexes/__init__.py
--rw-r--r--   0        0        0    10894 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/document_indexes/client.py
--rw-r--r--   0        0        0       65 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/documents/__init__.py
--rw-r--r--   0        0        0    17776 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/documents/client.py
--rw-r--r--   0        0        0       65 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/folder_entities/__init__.py
--rw-r--r--   0        0        0     3748 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/folder_entities/client.py
--rw-r--r--   0        0        0       65 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/model_versions/__init__.py
--rw-r--r--   0        0        0     3053 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/model_versions/client.py
--rw-r--r--   0        0        0       65 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/registered_prompts/__init__.py
--rw-r--r--   0        0        0    12451 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/registered_prompts/client.py
--rw-r--r--   0        0        0       65 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/sandboxes/__init__.py
--rw-r--r--   0        0        0     9182 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/sandboxes/client.py
--rw-r--r--   0        0        0       65 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/test_suites/__init__.py
--rw-r--r--   0        0        0     8693 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/test_suites/client.py
--rw-r--r--   0        0        0      173 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/workflow_deployments/__init__.py
--rw-r--r--   0        0        0     6711 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/workflow_deployments/client.py
--rw-r--r--   0        0        0      208 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/workflow_deployments/types/__init__.py
--rw-r--r--   0        0        0      542 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/workflow_deployments/types/workflow_deployments_list_request_status.py
--rw-r--r--   0        0        0    36776 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/__init__.py
--rw-r--r--   0        0        0     1003 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/api_node_result.py
--rw-r--r--   0        0        0     1125 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/api_node_result_data.py
--rw-r--r--   0        0        0     1050 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/array_chat_message_content.py
--rw-r--r--   0        0        0     1221 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/array_chat_message_content_item.py
--rw-r--r--   0        0        0     1345 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/array_chat_message_content_item_request.py
--rw-r--r--   0        0        0     1079 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/array_chat_message_content_request.py
--rw-r--r--   0        0        0      138 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/array_enum.py
--rw-r--r--   0        0        0     2451 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/array_variable_value_item.py
--rw-r--r--   0        0        0     1051 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/block_type_enum.py
--rw-r--r--   0        0        0      151 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/chat_history_enum.py
--rw-r--r--   0        0        0     1130 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/chat_history_input_request.py
--rw-r--r--   0        0        0      958 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/chat_history_variable_value.py
--rw-r--r--   0        0        0     1060 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/chat_message.py
--rw-r--r--   0        0        0     1466 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/chat_message_content.py
--rw-r--r--   0        0        0     1630 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/chat_message_content_request.py
--rw-r--r--   0        0        0     1089 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/chat_message_request.py
--rw-r--r--   0        0        0      914 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/chat_message_role.py
--rw-r--r--   0        0        0      980 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/code_execution_node_chat_history_result.py
--rw-r--r--   0        0        0      961 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/code_execution_node_error_result.py
--rw-r--r--   0        0        0      939 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/code_execution_node_json_result.py
--rw-r--r--   0        0        0      918 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/code_execution_node_number_result.py
--rw-r--r--   0        0        0     1054 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/code_execution_node_result.py
--rw-r--r--   0        0        0     1029 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/code_execution_node_result_data.py
--rw-r--r--   0        0        0     2386 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/code_execution_node_result_output.py
--rw-r--r--   0        0        0      985 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/code_execution_node_search_results_result.py
--rw-r--r--   0        0        0      916 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/code_execution_node_string_result.py
--rw-r--r--   0        0        0     1042 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/conditional_node_result.py
--rw-r--r--   0        0        0      911 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/conditional_node_result_data.py
--rw-r--r--   0        0        0      918 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/deployment_provider_payload_response.py
--rw-r--r--   0        0        0     2000 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/deployment_read.py
--rw-r--r--   0        0        0     1634 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/document_document_to_document_index.py
--rw-r--r--   0        0        0     1867 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/document_index_read.py
--rw-r--r--   0        0        0     2264 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/document_read.py
--rw-r--r--   0        0        0      144 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/document_status.py
--rw-r--r--   0        0        0     2135 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/enriched_normalized_completion.py
--rw-r--r--   0        0        0      539 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/entity_status.py
--rw-r--r--   0        0        0      799 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/environment_enum.py
--rw-r--r--   0        0        0      138 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/error_enum.py
--rw-r--r--   0        0        0      939 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/error_variable_value.py
--rw-r--r--   0        0        0      958 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/execute_prompt_api_error_response.py
--rw-r--r--   0        0        0     1523 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/execute_prompt_event.py
--rw-r--r--   0        0        0      871 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/execute_prompt_response.py
--rw-r--r--   0        0        0      957 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/execute_workflow_error_response.py
--rw-r--r--   0        0        0     1091 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/execute_workflow_response.py
--rw-r--r--   0        0        0      963 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/execute_workflow_stream_error_response.py
--rw-r--r--   0        0        0     1024 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/execute_workflow_workflow_result_event.py
--rw-r--r--   0        0        0      726 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/finish_reason_enum.py
--rw-r--r--   0        0        0      146 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/fulfilled_enum.py
--rw-r--r--   0        0        0     1248 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/fulfilled_execute_prompt_event.py
--rw-r--r--   0        0        0     1450 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/fulfilled_execute_prompt_response.py
--rw-r--r--   0        0        0     1109 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/fulfilled_execute_workflow_workflow_result_event.py
--rw-r--r--   0        0        0     1012 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/fulfilled_function_call.py
--rw-r--r--   0        0        0     1145 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/fulfilled_prompt_execution_meta.py
--rw-r--r--   0        0        0     1302 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/fulfilled_workflow_node_result_event.py
--rw-r--r--   0        0        0      770 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/function_call.py
--rw-r--r--   0        0        0     1085 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/function_call_chat_message_content.py
--rw-r--r--   0        0        0     1114 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/function_call_chat_message_content_request.py
--rw-r--r--   0        0        0     1026 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/function_call_chat_message_content_value.py
--rw-r--r--   0        0        0     1033 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/function_call_chat_message_content_value_request.py
--rw-r--r--   0        0        0      153 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/function_call_enum.py
--rw-r--r--   0        0        0      932 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/function_call_variable_value.py
--rw-r--r--   0        0        0      950 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/generate_error_response.py
--rw-r--r--   0        0        0     1117 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/generate_options_request.py
--rw-r--r--   0        0        0     1581 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/generate_request.py
--rw-r--r--   0        0        0     1342 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/generate_response.py
--rw-r--r--   0        0        0     1397 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/generate_result.py
--rw-r--r--   0        0        0     1111 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/generate_result_data.py
--rw-r--r--   0        0        0      959 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/generate_result_error.py
--rw-r--r--   0        0        0      954 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/generate_stream_response.py
--rw-r--r--   0        0        0     1107 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/generate_stream_result.py
--rw-r--r--   0        0        0     1011 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/generate_stream_result_data.py
--rw-r--r--   0        0        0      995 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/image_chat_message_content.py
--rw-r--r--   0        0        0     1024 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/image_chat_message_content_request.py
--rw-r--r--   0        0        0      138 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/image_enum.py
--rw-r--r--   0        0        0     1181 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/indexing_state_enum.py
--rw-r--r--   0        0        0      146 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/initiated_enum.py
--rw-r--r--   0        0        0     1147 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/initiated_execute_prompt_event.py
--rw-r--r--   0        0        0     1173 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/initiated_prompt_execution_meta.py
--rw-r--r--   0        0        0     1323 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/initiated_workflow_node_result_event.py
--rw-r--r--   0        0        0      136 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/json_enum.py
--rw-r--r--   0        0        0     1057 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/json_input_request.py
--rw-r--r--   0        0        0      917 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/json_variable_value.py
--rw-r--r--   0        0        0     4282 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/logical_operator.py
--rw-r--r--   0        0        0      490 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/logprobs_enum.py
--rw-r--r--   0        0        0     1333 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/metadata_filter_config_request.py
--rw-r--r--   0        0        0      528 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/metadata_filter_rule_combinator.py
--rw-r--r--   0        0        0     1349 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/metadata_filter_rule_request.py
--rw-r--r--   0        0        0     1356 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/model_version_build_config.py
--rw-r--r--   0        0        0     1632 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/model_version_exec_config.py
--rw-r--r--   0        0        0     1247 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/model_version_exec_config_parameters.py
--rw-r--r--   0        0        0     2575 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/model_version_read.py
--rw-r--r--   0        0        0     1032 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/model_version_read_status_enum.py
--rw-r--r--   0        0        0     1217 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/model_version_sandbox_snapshot.py
--rw-r--r--   0        0        0     1014 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/named_test_case_chat_history_variable_value_request.py
--rw-r--r--   0        0        0      995 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/named_test_case_error_variable_value_request.py
--rw-r--r--   0        0        0      951 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/named_test_case_json_variable_value_request.py
--rw-r--r--   0        0        0      930 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/named_test_case_number_variable_value_request.py
--rw-r--r--   0        0        0     1019 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/named_test_case_search_results_variable_value_request.py
--rw-r--r--   0        0        0      928 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/named_test_case_string_variable_value_request.py
--rw-r--r--   0        0        0     2630 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/named_test_case_variable_value_request.py
--rw-r--r--   0        0        0     1032 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/node_input_compiled_array_value.py
--rw-r--r--   0        0        0     1003 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/node_input_compiled_chat_history_value.py
--rw-r--r--   0        0        0      984 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/node_input_compiled_error_value.py
--rw-r--r--   0        0        0      962 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/node_input_compiled_json_value.py
--rw-r--r--   0        0        0      941 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/node_input_compiled_number_value.py
--rw-r--r--   0        0        0     1008 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/node_input_compiled_search_results_value.py
--rw-r--r--   0        0        0      939 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/node_input_compiled_string_value.py
--rw-r--r--   0        0        0     2730 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/node_input_variable_compiled_value.py
--rw-r--r--   0        0        0     1021 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/node_output_compiled_array_value.py
--rw-r--r--   0        0        0      992 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/node_output_compiled_chat_history_value.py
--rw-r--r--   0        0        0      973 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/node_output_compiled_error_value.py
--rw-r--r--   0        0        0      979 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/node_output_compiled_function_value.py
--rw-r--r--   0        0        0      951 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/node_output_compiled_json_value.py
--rw-r--r--   0        0        0      930 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/node_output_compiled_number_value.py
--rw-r--r--   0        0        0      997 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/node_output_compiled_search_results_value.py
--rw-r--r--   0        0        0      928 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/node_output_compiled_string_value.py
--rw-r--r--   0        0        0     3015 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/node_output_compiled_value.py
--rw-r--r--   0        0        0     1013 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/normalized_log_probs.py
--rw-r--r--   0        0        0     1014 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/normalized_token_log_probs.py
--rw-r--r--   0        0        0      140 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/number_enum.py
--rw-r--r--   0        0        0      896 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/number_variable_value.py
--rw-r--r--   0        0        0     1087 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/paginated_slim_deployment_read_list.py
--rw-r--r--   0        0        0     1062 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/paginated_slim_document_list.py
--rw-r--r--   0        0        0     1103 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/paginated_slim_workflow_deployment_list.py
--rw-r--r--   0        0        0      752 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/processing_failure_reason_enum.py
--rw-r--r--   0        0        0      962 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/processing_state_enum.py
--rw-r--r--   0        0        0     1819 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/prompt_deployment_expand_meta_request_request.py
--rw-r--r--   0        0        0     1159 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/prompt_deployment_input_request.py
--rw-r--r--   0        0        0     1266 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/prompt_execution_meta.py
--rw-r--r--   0        0        0     1017 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/prompt_node_result.py
--rw-r--r--   0        0        0      987 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/prompt_node_result_data.py
--rw-r--r--   0        0        0     1336 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/prompt_output.py
--rw-r--r--   0        0        0     1164 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/prompt_template_block.py
--rw-r--r--   0        0        0      983 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/prompt_template_block_data.py
--rw-r--r--   0        0        0     1012 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/prompt_template_block_data_request.py
--rw-r--r--   0        0        0     1586 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/prompt_template_block_properties.py
--rw-r--r--   0        0        0     1622 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/prompt_template_block_properties_request.py
--rw-r--r--   0        0        0     1200 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/prompt_template_block_request.py
--rw-r--r--   0        0        0     2516 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/provider_enum.py
--rw-r--r--   0        0        0     1192 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/raw_prompt_execution_overrides_request.py
--rw-r--r--   0        0        0      956 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/register_prompt_error_response.py
--rw-r--r--   0        0        0     1215 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/register_prompt_model_parameters_request.py
--rw-r--r--   0        0        0     1035 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/register_prompt_prompt.py
--rw-r--r--   0        0        0     1269 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/register_prompt_prompt_info_request.py
--rw-r--r--   0        0        0     1926 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/register_prompt_response.py
--rw-r--r--   0        0        0     1149 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/registered_prompt_deployment.py
--rw-r--r--   0        0        0     1020 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/registered_prompt_input_variable_request.py
--rw-r--r--   0        0        0     1057 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/registered_prompt_model_version.py
--rw-r--r--   0        0        0     1040 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/registered_prompt_sandbox.py
--rw-r--r--   0        0        0      960 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/registered_prompt_sandbox_snapshot.py
--rw-r--r--   0        0        0      144 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/rejected_enum.py
--rw-r--r--   0        0        0     1172 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/rejected_execute_prompt_event.py
--rw-r--r--   0        0        0     1410 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/rejected_execute_prompt_response.py
--rw-r--r--   0        0        0     1123 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/rejected_execute_workflow_workflow_result_event.py
--rw-r--r--   0        0        0     1051 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/rejected_function_call.py
--rw-r--r--   0        0        0     1144 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/rejected_prompt_execution_meta.py
--rw-r--r--   0        0        0     1246 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/rejected_workflow_node_result_event.py
--rw-r--r--   0        0        0     1098 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/sandbox_scenario.py
--rw-r--r--   0        0        0     1108 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/scenario_input.py
--rw-r--r--   0        0        0     1137 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/scenario_input_request.py
--rw-r--r--   0        0        0      580 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/scenario_input_type_enum.py
--rw-r--r--   0        0        0      948 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/search_error_response.py
--rw-r--r--   0        0        0     1221 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/search_filters_request.py
--rw-r--r--   0        0        0     1017 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/search_node_result.py
--rw-r--r--   0        0        0     1159 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/search_node_result_data.py
--rw-r--r--   0        0        0     1579 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/search_request_options_request.py
--rw-r--r--   0        0        0     1071 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/search_response.py
--rw-r--r--   0        0        0     1306 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/search_result.py
--rw-r--r--   0        0        0     1418 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/search_result_document.py
--rw-r--r--   0        0        0     1357 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/search_result_document_request.py
--rw-r--r--   0        0        0      970 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/search_result_merging_request.py
--rw-r--r--   0        0        0     1335 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/search_result_request.py
--rw-r--r--   0        0        0      155 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/search_results_enum.py
--rw-r--r--   0        0        0      963 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/search_results_variable_value.py
--rw-r--r--   0        0        0     1117 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/search_weights_request.py
--rw-r--r--   0        0        0     1811 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/slim_deployment_read.py
--rw-r--r--   0        0        0     3074 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/slim_document.py
--rw-r--r--   0        0        0     2205 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/slim_workflow_deployment.py
--rw-r--r--   0        0        0      146 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/streaming_enum.py
--rw-r--r--   0        0        0     1393 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/streaming_execute_prompt_event.py
--rw-r--r--   0        0        0     1043 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/streaming_prompt_execution_meta.py
--rw-r--r--   0        0        0     1322 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/streaming_workflow_node_result_event.py
--rw-r--r--   0        0        0      950 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/string_chat_message_content.py
--rw-r--r--   0        0        0      957 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/string_chat_message_content_request.py
--rw-r--r--   0        0        0      140 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/string_enum.py
--rw-r--r--   0        0        0     1035 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/string_input_request.py
--rw-r--r--   0        0        0      894 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/string_variable_value.py
--rw-r--r--   0        0        0     1787 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/submit_completion_actual_request.py
--rw-r--r--   0        0        0      895 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/submit_completion_actuals_error_response.py
--rw-r--r--   0        0        0     1413 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/submit_workflow_execution_actual_request.py
--rw-r--r--   0        0        0      150 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/subworkflow_enum.py
--rw-r--r--   0        0        0      937 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/subworkflow_node_result.py
--rw-r--r--   0        0        0      977 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/templating_node_chat_history_result.py
--rw-r--r--   0        0        0      958 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/templating_node_error_result.py
--rw-r--r--   0        0        0      936 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/templating_node_json_result.py
--rw-r--r--   0        0        0      915 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/templating_node_number_result.py
--rw-r--r--   0        0        0     1037 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/templating_node_result.py
--rw-r--r--   0        0        0      976 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/templating_node_result_data.py
--rw-r--r--   0        0        0     2287 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/templating_node_result_output.py
--rw-r--r--   0        0        0      982 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/templating_node_search_results_result.py
--rw-r--r--   0        0        0      913 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/templating_node_string_result.py
--rw-r--r--   0        0        0     1137 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/terminal_node_array_result.py
--rw-r--r--   0        0        0     1108 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/terminal_node_chat_history_result.py
--rw-r--r--   0        0        0     1089 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/terminal_node_error_result.py
--rw-r--r--   0        0        0     1099 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/terminal_node_function_call_result.py
--rw-r--r--   0        0        0     1067 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/terminal_node_json_result.py
--rw-r--r--   0        0        0     1046 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/terminal_node_number_result.py
--rw-r--r--   0        0        0     1027 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/terminal_node_result.py
--rw-r--r--   0        0        0      968 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/terminal_node_result_data.py
--rw-r--r--   0        0        0     2917 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/terminal_node_result_output.py
--rw-r--r--   0        0        0     1113 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/terminal_node_search_results_result.py
--rw-r--r--   0        0        0     1044 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/terminal_node_string_result.py
--rw-r--r--   0        0        0      987 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/test_case_chat_history_variable_value.py
--rw-r--r--   0        0        0      968 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/test_case_error_variable_value.py
--rw-r--r--   0        0        0      946 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/test_case_json_variable_value.py
--rw-r--r--   0        0        0      925 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/test_case_number_variable_value.py
--rw-r--r--   0        0        0      992 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/test_case_search_results_variable_value.py
--rw-r--r--   0        0        0      923 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/test_case_string_variable_value.py
--rw-r--r--   0        0        0     2246 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/test_case_variable_value.py
--rw-r--r--   0        0        0     1092 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/test_suite_test_case.py
--rw-r--r--   0        0        0      886 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/upload_document_error_response.py
--rw-r--r--   0        0        0      956 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/upload_document_response.py
--rw-r--r--   0        0        0      957 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/vellum_error.py
--rw-r--r--   0        0        0     1221 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/vellum_error_code_enum.py
--rw-r--r--   0        0        0      964 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/vellum_error_request.py
--rw-r--r--   0        0        0      927 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/vellum_image.py
--rw-r--r--   0        0        0      934 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/vellum_image_request.py
--rw-r--r--   0        0        0      964 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/vellum_variable.py
--rw-r--r--   0        0        0     1855 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/vellum_variable_type.py
--rw-r--r--   0        0        0     2211 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_deployment_read.py
--rw-r--r--   0        0        0     1001 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_event_error.py
--rw-r--r--   0        0        0     2014 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_execution_actual_chat_history_request.py
--rw-r--r--   0        0        0     1951 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_execution_actual_json_request.py
--rw-r--r--   0        0        0     1928 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_execution_actual_string_request.py
--rw-r--r--   0        0        0     2185 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_execution_event_error_code.py
--rw-r--r--   0        0        0      567 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_execution_event_type.py
--rw-r--r--   0        0        0     1145 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_execution_node_result_event.py
--rw-r--r--   0        0        0     1140 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_execution_workflow_result_event.py
--rw-r--r--   0        0        0     2715 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_node_result_data.py
--rw-r--r--   0        0        0     1632 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_node_result_event.py
--rw-r--r--   0        0        0     1035 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_node_result_event_state.py
--rw-r--r--   0        0        0     2934 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_output.py
--rw-r--r--   0        0        0     1139 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_output_array.py
--rw-r--r--   0        0        0     1116 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_output_chat_history.py
--rw-r--r--   0        0        0     1091 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_output_error.py
--rw-r--r--   0        0        0     1108 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_output_function_call.py
--rw-r--r--   0        0        0     1091 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_output_image.py
--rw-r--r--   0        0        0     1067 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_output_json.py
--rw-r--r--   0        0        0     1048 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_output_number.py
--rw-r--r--   0        0        0     1123 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_output_search_results.py
--rw-r--r--   0        0        0     1046 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_output_string.py
--rw-r--r--   0        0        0     1146 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_request_chat_history_input_request.py
--rw-r--r--   0        0        0     1666 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_request_input_request.py
--rw-r--r--   0        0        0     1075 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_request_json_input_request.py
--rw-r--r--   0        0        0     1056 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_request_number_input_request.py
--rw-r--r--   0        0        0     1054 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_request_string_input_request.py
--rw-r--r--   0        0        0     1347 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_result_event.py
--rw-r--r--   0        0        0     3282 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_result_event_output_data.py
--rw-r--r--   0        0        0     1420 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_result_event_output_data_array.py
--rw-r--r--   0        0        0     1397 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_result_event_output_data_chat_history.py
--rw-r--r--   0        0        0     1372 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_result_event_output_data_error.py
--rw-r--r--   0        0        0     1389 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_result_event_output_data_function_call.py
--rw-r--r--   0        0        0     1348 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_result_event_output_data_json.py
--rw-r--r--   0        0        0     1329 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_result_event_output_data_number.py
--rw-r--r--   0        0        0     1404 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_result_event_output_data_search_results.py
--rw-r--r--   0        0        0     1478 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_result_event_output_data_string.py
--rw-r--r--   0        0        0      873 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_stream_event.py
--rw-r--r--   0        0        0     3486 1970-01-01 00:00:00.000000 vellum_ai-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2980 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/README.md
+-rw-r--r--   0        0        0      632 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    35591 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/__init__.py
+-rw-r--r--   0        0        0    97089 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/client.py
+-rw-r--r--   0        0        0      853 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/core/api_error.py
+-rw-r--r--   0        0        0     1697 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/core/file.py
+-rw-r--r--   0        0        0     5059 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      329 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/core/request_options.py
+-rw-r--r--   0        0        0      498 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/environment.py
+-rw-r--r--   0        0        0      343 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/errors/__init__.py
+-rw-r--r--   0        0        0      248 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/errors/bad_request_error.py
+-rw-r--r--   0        0        0      247 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/errors/forbidden_error.py
+-rw-r--r--   0        0        0      252 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/errors/internal_server_error.py
+-rw-r--r--   0        0        0      246 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/errors/not_found_error.py
+-rw-r--r--   0        0        0       79 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/lib/__init__.py
+-rw-r--r--   0        0        0       77 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/lib/test_suites/__init__.py
+-rw-r--r--   0        0        0      116 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/lib/test_suites/constants.py
+-rw-r--r--   0        0        0       56 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/lib/test_suites/exceptions.py
+-rw-r--r--   0        0        0     9197 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/lib/test_suites/resources.py
+-rw-r--r--   0        0        0        0 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/lib/utils/__init__.py
+-rw-r--r--   0        0        0      280 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/lib/utils/env.py
+-rw-r--r--   0        0        0       48 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/lib/utils/exceptions.py
+-rw-r--r--   0        0        0      693 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/lib/utils/paginator.py
+-rw-r--r--   0        0        0        0 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/py.typed
+-rw-r--r--   0        0        0      730 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/resources/__init__.py
+-rw-r--r--   0        0        0      157 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/resources/deployments/__init__.py
+-rw-r--r--   0        0        0    19588 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/resources/deployments/client.py
+-rw-r--r--   0        0        0      183 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/resources/deployments/types/__init__.py
+-rw-r--r--   0        0        0      174 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/resources/deployments/types/deployments_list_request_status.py
+-rw-r--r--   0        0        0      165 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/resources/document_indexes/__init__.py
+-rw-r--r--   0        0        0    39845 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/resources/document_indexes/client.py
+-rw-r--r--   0        0        0      196 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/resources/document_indexes/types/__init__.py
+-rw-r--r--   0        0        0      178 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/resources/document_indexes/types/document_indexes_list_request_status.py
+-rw-r--r--   0        0        0       65 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/resources/documents/__init__.py
+-rw-r--r--   0        0        0    34010 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/resources/documents/client.py
+-rw-r--r--   0        0        0       65 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/resources/folder_entities/__init__.py
+-rw-r--r--   0        0        0     6435 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/resources/folder_entities/client.py
+-rw-r--r--   0        0        0       65 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/resources/sandboxes/__init__.py
+-rw-r--r--   0        0        0    12738 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/resources/sandboxes/client.py
+-rw-r--r--   0        0        0       65 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/resources/test_suite_runs/__init__.py
+-rw-r--r--   0        0        0    18728 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/resources/test_suite_runs/client.py
+-rw-r--r--   0        0        0       65 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/resources/test_suites/__init__.py
+-rw-r--r--   0        0        0    18982 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/resources/test_suites/client.py
+-rw-r--r--   0        0        0      173 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/resources/workflow_deployments/__init__.py
+-rw-r--r--   0        0        0    11158 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/resources/workflow_deployments/client.py
+-rw-r--r--   0        0        0      208 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/resources/workflow_deployments/types/__init__.py
+-rw-r--r--   0        0        0      182 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/resources/workflow_deployments/types/workflow_deployments_list_request_status.py
+-rw-r--r--   0        0        0      454 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/terraform/__init__.py
+-rw-r--r--   0        0        0      473 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/terraform/_jsii/__init__.py
+-rw-r--r--   0        0        0    15887 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/terraform/_jsii/vellum-ai_vellum@0.0.0.jsii.tgz
+-rw-r--r--   0        0        0       43 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/terraform/constraints.json
+-rw-r--r--   0        0        0    21484 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/terraform/data_vellum_document_index/__init__.py
+-rw-r--r--   0        0        0    25018 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/terraform/document_index/__init__.py
+-rw-r--r--   0        0        0    10298 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/terraform/provider/__init__.py
+-rw-r--r--   0        0        0        1 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/terraform/py.typed
+-rw-r--r--   0        0        0       56 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/terraform/versions.json
+-rw-r--r--   0        0        0    47325 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/__init__.py
+-rw-r--r--   0        0        0      983 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/api_node_result.py
+-rw-r--r--   0        0        0     1161 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/api_node_result_data.py
+-rw-r--r--   0        0        0     1030 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/array_chat_message_content.py
+-rw-r--r--   0        0        0     1297 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/array_chat_message_content_item.py
+-rw-r--r--   0        0        0     1421 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/array_chat_message_content_item_request.py
+-rw-r--r--   0        0        0     1059 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/array_chat_message_content_request.py
+-rw-r--r--   0        0        0      116 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/array_enum.py
+-rw-r--r--   0        0        0     3002 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/array_variable_value_item.py
+-rw-r--r--   0        0        0      129 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/chat_history_enum.py
+-rw-r--r--   0        0        0     1121 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/chat_history_input_request.py
+-rw-r--r--   0        0        0      945 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/chat_history_variable_value.py
+-rw-r--r--   0        0        0     1213 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/chat_message.py
+-rw-r--r--   0        0        0     1573 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/chat_message_content.py
+-rw-r--r--   0        0        0     1737 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/chat_message_content_request.py
+-rw-r--r--   0        0        0     1242 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/chat_message_request.py
+-rw-r--r--   0        0        0      182 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/chat_message_role.py
+-rw-r--r--   0        0        0      996 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/code_execution_node_array_result.py
+-rw-r--r--   0        0        0      967 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/code_execution_node_chat_history_result.py
+-rw-r--r--   0        0        0      948 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/code_execution_node_error_result.py
+-rw-r--r--   0        0        0      958 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/code_execution_node_function_call_result.py
+-rw-r--r--   0        0        0      926 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/code_execution_node_json_result.py
+-rw-r--r--   0        0        0      905 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/code_execution_node_number_result.py
+-rw-r--r--   0        0        0     1034 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/code_execution_node_result.py
+-rw-r--r--   0        0        0     1016 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/code_execution_node_result_data.py
+-rw-r--r--   0        0        0     3377 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/code_execution_node_result_output.py
+-rw-r--r--   0        0        0      972 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/code_execution_node_search_results_result.py
+-rw-r--r--   0        0        0      903 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/code_execution_node_string_result.py
+-rw-r--r--   0        0        0     1022 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/conditional_node_result.py
+-rw-r--r--   0        0        0      898 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/conditional_node_result_data.py
+-rw-r--r--   0        0        0      898 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/deployment_provider_payload_response.py
+-rw-r--r--   0        0        0     1938 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/deployment_read.py
+-rw-r--r--   0        0        0     1532 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/document_document_to_document_index.py
+-rw-r--r--   0        0        0     1783 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/document_index_read.py
+-rw-r--r--   0        0        0     2200 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/document_read.py
+-rw-r--r--   0        0        0      122 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/document_status.py
+-rw-r--r--   0        0        0     2108 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/enriched_normalized_completion.py
+-rw-r--r--   0        0        0      158 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/entity_status.py
+-rw-r--r--   0        0        0      179 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/environment_enum.py
+-rw-r--r--   0        0        0      116 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/error_enum.py
+-rw-r--r--   0        0        0      926 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/error_variable_value.py
+-rw-r--r--   0        0        0      948 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/execute_prompt_api_error_response.py
+-rw-r--r--   0        0        0     1636 2024-04-25 14:28:47.342349 vellum_ai-0.5.0/src/vellum/types/execute_prompt_event.py
+-rw-r--r--   0        0        0      914 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/execute_prompt_response.py
+-rw-r--r--   0        0        0      947 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/execute_workflow_error_response.py
+-rw-r--r--   0        0        0     1085 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/execute_workflow_response.py
+-rw-r--r--   0        0        0      953 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/execute_workflow_stream_error_response.py
+-rw-r--r--   0        0        0     1067 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/execute_workflow_workflow_result_event.py
+-rw-r--r--   0        0        0     1099 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/execution_array_vellum_value.py
+-rw-r--r--   0        0        0     1070 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/execution_chat_history_vellum_value.py
+-rw-r--r--   0        0        0     1051 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/execution_error_vellum_value.py
+-rw-r--r--   0        0        0     1061 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/execution_function_call_vellum_value.py
+-rw-r--r--   0        0        0     1029 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/execution_json_vellum_value.py
+-rw-r--r--   0        0        0     1008 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/execution_number_vellum_value.py
+-rw-r--r--   0        0        0     1075 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/execution_search_results_vellum_value.py
+-rw-r--r--   0        0        0     1006 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/execution_string_vellum_value.py
+-rw-r--r--   0        0        0     3144 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/execution_vellum_value.py
+-rw-r--r--   0        0        0     1125 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/external_test_case_execution.py
+-rw-r--r--   0        0        0     1154 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/external_test_case_execution_request.py
+-rw-r--r--   0        0        0      169 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/finish_reason_enum.py
+-rw-r--r--   0        0        0      124 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/fulfilled_enum.py
+-rw-r--r--   0        0        0     1235 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/fulfilled_execute_prompt_event.py
+-rw-r--r--   0        0        0     1457 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/fulfilled_execute_prompt_response.py
+-rw-r--r--   0        0        0     1089 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/fulfilled_execute_workflow_workflow_result_event.py
+-rw-r--r--   0        0        0      999 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/fulfilled_function_call.py
+-rw-r--r--   0        0        0     1073 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/fulfilled_function_call_request.py
+-rw-r--r--   0        0        0     1228 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/fulfilled_prompt_execution_meta.py
+-rw-r--r--   0        0        0     1373 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/fulfilled_workflow_node_result_event.py
+-rw-r--r--   0        0        0      813 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/function_call.py
+-rw-r--r--   0        0        0     1065 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/function_call_chat_message_content.py
+-rw-r--r--   0        0        0     1094 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/function_call_chat_message_content_request.py
+-rw-r--r--   0        0        0     1013 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/function_call_chat_message_content_value.py
+-rw-r--r--   0        0        0     1020 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/function_call_chat_message_content_value_request.py
+-rw-r--r--   0        0        0      131 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/function_call_enum.py
+-rw-r--r--   0        0        0      912 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/function_call_variable_value.py
+-rw-r--r--   0        0        0      940 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/generate_error_response.py
+-rw-r--r--   0        0        0     1079 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/generate_options_request.py
+-rw-r--r--   0        0        0     1572 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/generate_request.py
+-rw-r--r--   0        0        0     1342 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/generate_response.py
+-rw-r--r--   0        0        0     1394 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/generate_result.py
+-rw-r--r--   0        0        0     1087 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/generate_result_data.py
+-rw-r--r--   0        0        0      949 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/generate_result_error.py
+-rw-r--r--   0        0        0      934 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/generate_stream_response.py
+-rw-r--r--   0        0        0     1101 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/generate_stream_result.py
+-rw-r--r--   0        0        0      991 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/generate_stream_result_data.py
+-rw-r--r--   0        0        0      975 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/image_chat_message_content.py
+-rw-r--r--   0        0        0     1004 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/image_chat_message_content_request.py
+-rw-r--r--   0        0        0      116 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/image_enum.py
+-rw-r--r--   0        0        0     1000 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/image_variable_value.py
+-rw-r--r--   0        0        0      213 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/indexing_state_enum.py
+-rw-r--r--   0        0        0      124 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/initiated_enum.py
+-rw-r--r--   0        0        0     1134 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/initiated_execute_prompt_event.py
+-rw-r--r--   0        0        0     1181 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/initiated_prompt_execution_meta.py
+-rw-r--r--   0        0        0     1377 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/initiated_workflow_node_result_event.py
+-rw-r--r--   0        0        0      114 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/json_enum.py
+-rw-r--r--   0        0        0     1048 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/json_input_request.py
+-rw-r--r--   0        0        0      904 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/json_variable_value.py
+-rw-r--r--   0        0        0      487 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/logical_operator.py
+-rw-r--r--   0        0        0      151 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/logprobs_enum.py
+-rw-r--r--   0        0        0     1355 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/metadata_filter_config_request.py
+-rw-r--r--   0        0        0      165 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/metadata_filter_rule_combinator.py
+-rw-r--r--   0        0        0     1371 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/metadata_filter_rule_request.py
+-rw-r--r--   0        0        0     1086 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/ml_model_usage.py
+-rw-r--r--   0        0        0     1098 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/named_scenario_input_chat_history_variable_value_request.py
+-rw-r--r--   0        0        0     1043 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/named_scenario_input_request.py
+-rw-r--r--   0        0        0     1006 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/named_scenario_input_string_variable_value_request.py
+-rw-r--r--   0        0        0     1044 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/named_test_case_chat_history_variable_value.py
+-rw-r--r--   0        0        0     1073 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/named_test_case_chat_history_variable_value_request.py
+-rw-r--r--   0        0        0     1018 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/named_test_case_error_variable_value.py
+-rw-r--r--   0        0        0     1047 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/named_test_case_error_variable_value_request.py
+-rw-r--r--   0        0        0     1064 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/named_test_case_function_call_variable_value.py
+-rw-r--r--   0        0        0     1093 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/named_test_case_function_call_variable_value_request.py
+-rw-r--r--   0        0        0      995 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/named_test_case_json_variable_value.py
+-rw-r--r--   0        0        0     1002 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/named_test_case_json_variable_value_request.py
+-rw-r--r--   0        0        0      976 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/named_test_case_number_variable_value.py
+-rw-r--r--   0        0        0      983 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/named_test_case_number_variable_value_request.py
+-rw-r--r--   0        0        0     1051 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/named_test_case_search_results_variable_value.py
+-rw-r--r--   0        0        0     1080 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/named_test_case_search_results_variable_value_request.py
+-rw-r--r--   0        0        0      974 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/named_test_case_string_variable_value.py
+-rw-r--r--   0        0        0      981 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/named_test_case_string_variable_value_request.py
+-rw-r--r--   0        0        0     3021 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/named_test_case_variable_value.py
+-rw-r--r--   0        0        0     3280 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/named_test_case_variable_value_request.py
+-rw-r--r--   0        0        0     1019 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/node_input_compiled_array_value.py
+-rw-r--r--   0        0        0      990 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/node_input_compiled_chat_history_value.py
+-rw-r--r--   0        0        0      971 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/node_input_compiled_error_value.py
+-rw-r--r--   0        0        0      976 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/node_input_compiled_function_call.py
+-rw-r--r--   0        0        0      949 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/node_input_compiled_json_value.py
+-rw-r--r--   0        0        0      928 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/node_input_compiled_number_value.py
+-rw-r--r--   0        0        0      995 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/node_input_compiled_search_results_value.py
+-rw-r--r--   0        0        0      926 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/node_input_compiled_string_value.py
+-rw-r--r--   0        0        0     3354 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/node_input_variable_compiled_value.py
+-rw-r--r--   0        0        0     1008 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/node_output_compiled_array_value.py
+-rw-r--r--   0        0        0      979 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/node_output_compiled_chat_history_value.py
+-rw-r--r--   0        0        0      960 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/node_output_compiled_error_value.py
+-rw-r--r--   0        0        0      966 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/node_output_compiled_function_value.py
+-rw-r--r--   0        0        0      938 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/node_output_compiled_json_value.py
+-rw-r--r--   0        0        0      917 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/node_output_compiled_number_value.py
+-rw-r--r--   0        0        0      984 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/node_output_compiled_search_results_value.py
+-rw-r--r--   0        0        0      915 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/node_output_compiled_string_value.py
+-rw-r--r--   0        0        0     3262 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/node_output_compiled_value.py
+-rw-r--r--   0        0        0     1000 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/normalized_log_probs.py
+-rw-r--r--   0        0        0     1008 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/normalized_token_log_probs.py
+-rw-r--r--   0        0        0      118 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/number_enum.py
+-rw-r--r--   0        0        0      883 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/number_variable_value.py
+-rw-r--r--   0        0        0     1091 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/paginated_document_index_read_list.py
+-rw-r--r--   0        0        0     1095 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/paginated_slim_deployment_read_list.py
+-rw-r--r--   0        0        0     1070 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/paginated_slim_document_list.py
+-rw-r--r--   0        0        0     1111 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/paginated_slim_workflow_deployment_list.py
+-rw-r--r--   0        0        0     1060 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/paginated_test_suite_run_execution_list.py
+-rw-r--r--   0        0        0     1044 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/paginated_test_suite_test_case_list.py
+-rw-r--r--   0        0        0      195 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/processing_failure_reason_enum.py
+-rw-r--r--   0        0        0      190 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/processing_state_enum.py
+-rw-r--r--   0        0        0     2044 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/prompt_deployment_expand_meta_request_request.py
+-rw-r--r--   0        0        0     1233 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/prompt_deployment_input_request.py
+-rw-r--r--   0        0        0     1370 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/prompt_execution_meta.py
+-rw-r--r--   0        0        0      997 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/prompt_node_result.py
+-rw-r--r--   0        0        0      988 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/prompt_node_result_data.py
+-rw-r--r--   0        0        0     1442 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/prompt_output.py
+-rw-r--r--   0        0        0     1210 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/raw_prompt_execution_overrides_request.py
+-rw-r--r--   0        0        0      122 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/rejected_enum.py
+-rw-r--r--   0        0        0     1159 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/rejected_execute_prompt_event.py
+-rw-r--r--   0        0        0     1417 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/rejected_execute_prompt_response.py
+-rw-r--r--   0        0        0     1103 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/rejected_execute_workflow_workflow_result_event.py
+-rw-r--r--   0        0        0     1038 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/rejected_function_call.py
+-rw-r--r--   0        0        0     1138 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/rejected_prompt_execution_meta.py
+-rw-r--r--   0        0        0     1293 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/rejected_workflow_node_result_event.py
+-rw-r--r--   0        0        0     1144 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/sandbox_scenario.py
+-rw-r--r--   0        0        0      907 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/scenario_input.py
+-rw-r--r--   0        0        0     1071 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/scenario_input_chat_history_variable_value.py
+-rw-r--r--   0        0        0     1001 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/scenario_input_string_variable_value.py
+-rw-r--r--   0        0        0      938 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/search_error_response.py
+-rw-r--r--   0        0        0     1218 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/search_filters_request.py
+-rw-r--r--   0        0        0      997 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/search_node_result.py
+-rw-r--r--   0        0        0     1143 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/search_node_result_data.py
+-rw-r--r--   0        0        0     1622 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/search_request_options_request.py
+-rw-r--r--   0        0        0     1047 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/search_response.py
+-rw-r--r--   0        0        0     1304 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/search_result.py
+-rw-r--r--   0        0        0     1437 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/search_result_document.py
+-rw-r--r--   0        0        0     1365 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/search_result_document_request.py
+-rw-r--r--   0        0        0      972 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/search_result_merging_request.py
+-rw-r--r--   0        0        0     1333 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/search_result_request.py
+-rw-r--r--   0        0        0      133 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/search_results_enum.py
+-rw-r--r--   0        0        0      950 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/search_results_variable_value.py
+-rw-r--r--   0        0        0     1128 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/search_weights_request.py
+-rw-r--r--   0        0        0     1753 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/slim_deployment_read.py
+-rw-r--r--   0        0        0     2975 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/slim_document.py
+-rw-r--r--   0        0        0     2104 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/slim_workflow_deployment.py
+-rw-r--r--   0        0        0      124 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/streaming_enum.py
+-rw-r--r--   0        0        0     1388 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/streaming_execute_prompt_event.py
+-rw-r--r--   0        0        0     1030 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/streaming_prompt_execution_meta.py
+-rw-r--r--   0        0        0     1383 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/streaming_workflow_node_result_event.py
+-rw-r--r--   0        0        0      930 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/string_chat_message_content.py
+-rw-r--r--   0        0        0      937 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/string_chat_message_content_request.py
+-rw-r--r--   0        0        0      118 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/string_enum.py
+-rw-r--r--   0        0        0     1026 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/string_input_request.py
+-rw-r--r--   0        0        0      881 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/string_variable_value.py
+-rw-r--r--   0        0        0     1825 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/submit_completion_actual_request.py
+-rw-r--r--   0        0        0      875 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/submit_completion_actuals_error_response.py
+-rw-r--r--   0        0        0     1487 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/submit_workflow_execution_actual_request.py
+-rw-r--r--   0        0        0      128 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/subworkflow_enum.py
+-rw-r--r--   0        0        0      917 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/subworkflow_node_result.py
+-rw-r--r--   0        0        0      993 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/templating_node_array_result.py
+-rw-r--r--   0        0        0      964 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/templating_node_chat_history_result.py
+-rw-r--r--   0        0        0      945 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/templating_node_error_result.py
+-rw-r--r--   0        0        0      955 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/templating_node_function_call_result.py
+-rw-r--r--   0        0        0      923 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/templating_node_json_result.py
+-rw-r--r--   0        0        0      902 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/templating_node_number_result.py
+-rw-r--r--   0        0        0     1017 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/templating_node_result.py
+-rw-r--r--   0        0        0      956 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/templating_node_result_data.py
+-rw-r--r--   0        0        0     3246 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/templating_node_result_output.py
+-rw-r--r--   0        0        0      969 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/templating_node_search_results_result.py
+-rw-r--r--   0        0        0      900 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/templating_node_string_result.py
+-rw-r--r--   0        0        0     1142 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/terminal_node_array_result.py
+-rw-r--r--   0        0        0     1113 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/terminal_node_chat_history_result.py
+-rw-r--r--   0        0        0     1094 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/terminal_node_error_result.py
+-rw-r--r--   0        0        0     1104 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/terminal_node_function_call_result.py
+-rw-r--r--   0        0        0     1072 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/terminal_node_json_result.py
+-rw-r--r--   0        0        0     1051 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/terminal_node_number_result.py
+-rw-r--r--   0        0        0     1007 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/terminal_node_result.py
+-rw-r--r--   0        0        0      948 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/terminal_node_result_data.py
+-rw-r--r--   0        0        0     3164 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/terminal_node_result_output.py
+-rw-r--r--   0        0        0     1118 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/terminal_node_search_results_result.py
+-rw-r--r--   0        0        0     1049 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/terminal_node_string_result.py
+-rw-r--r--   0        0        0     1061 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/test_case_chat_history_variable_value.py
+-rw-r--r--   0        0        0     1036 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/test_case_error_variable_value.py
+-rw-r--r--   0        0        0     1081 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/test_case_function_call_variable_value.py
+-rw-r--r--   0        0        0     1012 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/test_case_json_variable_value.py
+-rw-r--r--   0        0        0      996 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/test_case_number_variable_value.py
+-rw-r--r--   0        0        0     1068 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/test_case_search_results_variable_value.py
+-rw-r--r--   0        0        0      991 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/test_case_string_variable_value.py
+-rw-r--r--   0        0        0     2834 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/test_case_variable_value.py
+-rw-r--r--   0        0        0     1373 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/test_suite_run_deployment_release_tag_exec_config.py
+-rw-r--r--   0        0        0     1228 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_data.py
+-rw-r--r--   0        0        0     1235 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_data_request.py
+-rw-r--r--   0        0        0     1411 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_request.py
+-rw-r--r--   0        0        0      174 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_type_enum.py
+-rw-r--r--   0        0        0     1483 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/test_suite_run_exec_config.py
+-rw-r--r--   0        0        0     1598 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/test_suite_run_exec_config_request.py
+-rw-r--r--   0        0        0     1158 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/test_suite_run_execution.py
+-rw-r--r--   0        0        0     1115 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/test_suite_run_execution_chat_history_output.py
+-rw-r--r--   0        0        0     1089 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/test_suite_run_execution_error_output.py
+-rw-r--r--   0        0        0     1135 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/test_suite_run_execution_function_call_output.py
+-rw-r--r--   0        0        0     1066 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/test_suite_run_execution_json_output.py
+-rw-r--r--   0        0        0      973 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/test_suite_run_execution_metric_definition.py
+-rw-r--r--   0        0        0     1218 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/test_suite_run_execution_metric_result.py
+-rw-r--r--   0        0        0     1047 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/test_suite_run_execution_number_output.py
+-rw-r--r--   0        0        0     3057 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/test_suite_run_execution_output.py
+-rw-r--r--   0        0        0     1122 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/test_suite_run_execution_search_results_output.py
+-rw-r--r--   0        0        0     1045 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/test_suite_run_execution_string_output.py
+-rw-r--r--   0        0        0     1331 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/test_suite_run_external_exec_config.py
+-rw-r--r--   0        0        0     1115 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/test_suite_run_external_exec_config_data.py
+-rw-r--r--   0        0        0     1144 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/test_suite_run_external_exec_config_data_request.py
+-rw-r--r--   0        0        0     1360 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/test_suite_run_external_exec_config_request.py
+-rw-r--r--   0        0        0      148 2024-04-25 14:28:47.346349 vellum_ai-0.5.0/src/vellum/types/test_suite_run_external_exec_config_type_enum.py
+-rw-r--r--   0        0        0     1005 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/test_suite_run_metric_error_output.py
+-rw-r--r--   0        0        0      144 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/test_suite_run_metric_error_output_type_enum.py
+-rw-r--r--   0        0        0      963 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/test_suite_run_metric_number_output.py
+-rw-r--r--   0        0        0      146 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/test_suite_run_metric_number_output_type_enum.py
+-rw-r--r--   0        0        0     1291 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/test_suite_run_metric_output.py
+-rw-r--r--   0        0        0      961 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/test_suite_run_metric_string_output.py
+-rw-r--r--   0        0        0      146 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/test_suite_run_metric_string_output_type_enum.py
+-rw-r--r--   0        0        0     1500 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/test_suite_run_read.py
+-rw-r--r--   0        0        0      197 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/test_suite_run_state.py
+-rw-r--r--   0        0        0      896 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/test_suite_run_test_suite.py
+-rw-r--r--   0        0        0     1367 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/test_suite_run_workflow_release_tag_exec_config.py
+-rw-r--r--   0        0        0     1241 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_data.py
+-rw-r--r--   0        0        0     1248 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_data_request.py
+-rw-r--r--   0        0        0     1405 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_request.py
+-rw-r--r--   0        0        0      170 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_type_enum.py
+-rw-r--r--   0        0        0     1086 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/test_suite_test_case.py
+-rw-r--r--   0        0        0      866 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/upload_document_error_response.py
+-rw-r--r--   0        0        0      946 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/upload_document_response.py
+-rw-r--r--   0        0        0      937 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/vellum_error.py
+-rw-r--r--   0        0        0      233 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/vellum_error_code_enum.py
+-rw-r--r--   0        0        0      944 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/vellum_error_request.py
+-rw-r--r--   0        0        0      914 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/vellum_image.py
+-rw-r--r--   0        0        0      921 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/vellum_image_request.py
+-rw-r--r--   0        0        0      944 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/vellum_variable.py
+-rw-r--r--   0        0        0      281 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/vellum_variable_type.py
+-rw-r--r--   0        0        0     2110 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/workflow_deployment_read.py
+-rw-r--r--   0        0        0      981 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/workflow_event_error.py
+-rw-r--r--   0        0        0     2038 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/workflow_execution_actual_chat_history_request.py
+-rw-r--r--   0        0        0     1975 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/workflow_execution_actual_json_request.py
+-rw-r--r--   0        0        0     1952 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/workflow_execution_actual_string_request.py
+-rw-r--r--   0        0        0      425 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/workflow_execution_event_error_code.py
+-rw-r--r--   0        0        0      170 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/workflow_execution_event_type.py
+-rw-r--r--   0        0        0     1139 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/workflow_execution_node_result_event.py
+-rw-r--r--   0        0        0     1134 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/workflow_execution_workflow_result_event.py
+-rw-r--r--   0        0        0     2966 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/workflow_node_result_data.py
+-rw-r--r--   0        0        0     1745 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/workflow_node_result_event.py
+-rw-r--r--   0        0        0      209 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/workflow_node_result_event_state.py
+-rw-r--r--   0        0        0     3212 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/workflow_output.py
+-rw-r--r--   0        0        0     1154 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/workflow_output_array.py
+-rw-r--r--   0        0        0     1131 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/workflow_output_chat_history.py
+-rw-r--r--   0        0        0     1106 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/workflow_output_error.py
+-rw-r--r--   0        0        0     1123 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/workflow_output_function_call.py
+-rw-r--r--   0        0        0     1106 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/workflow_output_image.py
+-rw-r--r--   0        0        0     1082 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/workflow_output_json.py
+-rw-r--r--   0        0        0     1063 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/workflow_output_number.py
+-rw-r--r--   0        0        0     1138 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/workflow_output_search_results.py
+-rw-r--r--   0        0        0     1061 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/workflow_output_string.py
+-rw-r--r--   0        0        0     1137 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/workflow_request_chat_history_input_request.py
+-rw-r--r--   0        0        0     1772 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/workflow_request_input_request.py
+-rw-r--r--   0        0        0     1066 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/workflow_request_json_input_request.py
+-rw-r--r--   0        0        0     1047 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/workflow_request_number_input_request.py
+-rw-r--r--   0        0        0     1045 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/workflow_request_string_input_request.py
+-rw-r--r--   0        0        0     1475 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/workflow_result_event.py
+-rw-r--r--   0        0        0     3529 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/workflow_result_event_output_data.py
+-rw-r--r--   0        0        0     1423 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/workflow_result_event_output_data_array.py
+-rw-r--r--   0        0        0     1400 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/workflow_result_event_output_data_chat_history.py
+-rw-r--r--   0        0        0     1375 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/workflow_result_event_output_data_error.py
+-rw-r--r--   0        0        0     1392 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/workflow_result_event_output_data_function_call.py
+-rw-r--r--   0        0        0     1351 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/workflow_result_event_output_data_json.py
+-rw-r--r--   0        0        0     1332 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/workflow_result_event_output_data_number.py
+-rw-r--r--   0        0        0     1407 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/workflow_result_event_output_data_search_results.py
+-rw-r--r--   0        0        0     1482 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/workflow_result_event_output_data_string.py
+-rw-r--r--   0        0        0      911 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/types/workflow_stream_event.py
+-rw-r--r--   0        0        0       77 2024-04-25 14:28:47.350349 vellum_ai-0.5.0/src/vellum/version.py
+-rw-r--r--   0        0        0     3549 1970-01-01 00:00:00.000000 vellum_ai-0.5.0/PKG-INFO
```

### Comparing `vellum_ai-0.3.9/LICENSE` & `vellum_ai-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.9/README.md` & `vellum_ai-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.9/src/vellum/__init__.py` & `vellum_ai-0.5.0/src/vellum/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,19 +14,19 @@
     ArrayChatMessageContentItem_String,
     ArrayChatMessageContentRequest,
     ArrayEnum,
     ArrayVariableValueItem,
     ArrayVariableValueItem_ChatHistory,
     ArrayVariableValueItem_Error,
     ArrayVariableValueItem_FunctionCall,
+    ArrayVariableValueItem_Image,
     ArrayVariableValueItem_Json,
     ArrayVariableValueItem_Number,
     ArrayVariableValueItem_SearchResults,
     ArrayVariableValueItem_String,
-    BlockTypeEnum,
     ChatHistoryEnum,
     ChatHistoryInputRequest,
     ChatHistoryVariableValue,
     ChatMessage,
     ChatMessageContent,
     ChatMessageContentRequest,
     ChatMessageContentRequest_Array,
@@ -35,23 +35,27 @@
     ChatMessageContentRequest_String,
     ChatMessageContent_Array,
     ChatMessageContent_FunctionCall,
     ChatMessageContent_Image,
     ChatMessageContent_String,
     ChatMessageRequest,
     ChatMessageRole,
+    CodeExecutionNodeArrayResult,
     CodeExecutionNodeChatHistoryResult,
     CodeExecutionNodeErrorResult,
+    CodeExecutionNodeFunctionCallResult,
     CodeExecutionNodeJsonResult,
     CodeExecutionNodeNumberResult,
     CodeExecutionNodeResult,
     CodeExecutionNodeResultData,
     CodeExecutionNodeResultOutput,
+    CodeExecutionNodeResultOutput_Array,
     CodeExecutionNodeResultOutput_ChatHistory,
     CodeExecutionNodeResultOutput_Error,
+    CodeExecutionNodeResultOutput_FunctionCall,
     CodeExecutionNodeResultOutput_Json,
     CodeExecutionNodeResultOutput_Number,
     CodeExecutionNodeResultOutput_SearchResults,
     CodeExecutionNodeResultOutput_String,
     CodeExecutionNodeSearchResultsResult,
     CodeExecutionNodeStringResult,
     ConditionalNodeResult,
@@ -78,20 +82,40 @@
     ExecutePromptResponse_Rejected,
     ExecuteWorkflowErrorResponse,
     ExecuteWorkflowResponse,
     ExecuteWorkflowStreamErrorResponse,
     ExecuteWorkflowWorkflowResultEvent,
     ExecuteWorkflowWorkflowResultEvent_Fulfilled,
     ExecuteWorkflowWorkflowResultEvent_Rejected,
+    ExecutionArrayVellumValue,
+    ExecutionChatHistoryVellumValue,
+    ExecutionErrorVellumValue,
+    ExecutionFunctionCallVellumValue,
+    ExecutionJsonVellumValue,
+    ExecutionNumberVellumValue,
+    ExecutionSearchResultsVellumValue,
+    ExecutionStringVellumValue,
+    ExecutionVellumValue,
+    ExecutionVellumValue_Array,
+    ExecutionVellumValue_ChatHistory,
+    ExecutionVellumValue_Error,
+    ExecutionVellumValue_FunctionCall,
+    ExecutionVellumValue_Json,
+    ExecutionVellumValue_Number,
+    ExecutionVellumValue_SearchResults,
+    ExecutionVellumValue_String,
+    ExternalTestCaseExecution,
+    ExternalTestCaseExecutionRequest,
     FinishReasonEnum,
     FulfilledEnum,
     FulfilledExecutePromptEvent,
     FulfilledExecutePromptResponse,
     FulfilledExecuteWorkflowWorkflowResultEvent,
     FulfilledFunctionCall,
+    FulfilledFunctionCallRequest,
     FulfilledPromptExecutionMeta,
     FulfilledWorkflowNodeResultEvent,
     FunctionCall,
     FunctionCallChatMessageContent,
     FunctionCallChatMessageContentRequest,
     FunctionCallChatMessageContentValue,
     FunctionCallChatMessageContentValueRequest,
@@ -108,57 +132,77 @@
     GenerateResultError,
     GenerateStreamResponse,
     GenerateStreamResult,
     GenerateStreamResultData,
     ImageChatMessageContent,
     ImageChatMessageContentRequest,
     ImageEnum,
+    ImageVariableValue,
     IndexingStateEnum,
     InitiatedEnum,
     InitiatedExecutePromptEvent,
     InitiatedPromptExecutionMeta,
     InitiatedWorkflowNodeResultEvent,
     JsonEnum,
     JsonInputRequest,
     JsonVariableValue,
     LogicalOperator,
     LogprobsEnum,
     MetadataFilterConfigRequest,
     MetadataFilterRuleCombinator,
     MetadataFilterRuleRequest,
-    ModelVersionBuildConfig,
-    ModelVersionExecConfig,
-    ModelVersionExecConfigParameters,
-    ModelVersionRead,
-    ModelVersionReadStatusEnum,
-    ModelVersionSandboxSnapshot,
+    MlModelUsage,
+    NamedScenarioInputChatHistoryVariableValueRequest,
+    NamedScenarioInputRequest,
+    NamedScenarioInputRequest_ChatHistory,
+    NamedScenarioInputRequest_String,
+    NamedScenarioInputStringVariableValueRequest,
+    NamedTestCaseChatHistoryVariableValue,
     NamedTestCaseChatHistoryVariableValueRequest,
+    NamedTestCaseErrorVariableValue,
     NamedTestCaseErrorVariableValueRequest,
+    NamedTestCaseFunctionCallVariableValue,
+    NamedTestCaseFunctionCallVariableValueRequest,
+    NamedTestCaseJsonVariableValue,
     NamedTestCaseJsonVariableValueRequest,
+    NamedTestCaseNumberVariableValue,
     NamedTestCaseNumberVariableValueRequest,
+    NamedTestCaseSearchResultsVariableValue,
     NamedTestCaseSearchResultsVariableValueRequest,
+    NamedTestCaseStringVariableValue,
     NamedTestCaseStringVariableValueRequest,
+    NamedTestCaseVariableValue,
     NamedTestCaseVariableValueRequest,
     NamedTestCaseVariableValueRequest_ChatHistory,
     NamedTestCaseVariableValueRequest_Error,
+    NamedTestCaseVariableValueRequest_FunctionCall,
     NamedTestCaseVariableValueRequest_Json,
     NamedTestCaseVariableValueRequest_Number,
     NamedTestCaseVariableValueRequest_SearchResults,
     NamedTestCaseVariableValueRequest_String,
+    NamedTestCaseVariableValue_ChatHistory,
+    NamedTestCaseVariableValue_Error,
+    NamedTestCaseVariableValue_FunctionCall,
+    NamedTestCaseVariableValue_Json,
+    NamedTestCaseVariableValue_Number,
+    NamedTestCaseVariableValue_SearchResults,
+    NamedTestCaseVariableValue_String,
     NodeInputCompiledArrayValue,
     NodeInputCompiledChatHistoryValue,
     NodeInputCompiledErrorValue,
+    NodeInputCompiledFunctionCall,
     NodeInputCompiledJsonValue,
     NodeInputCompiledNumberValue,
     NodeInputCompiledSearchResultsValue,
     NodeInputCompiledStringValue,
     NodeInputVariableCompiledValue,
     NodeInputVariableCompiledValue_Array,
     NodeInputVariableCompiledValue_ChatHistory,
     NodeInputVariableCompiledValue_Error,
+    NodeInputVariableCompiledValue_FunctionCall,
     NodeInputVariableCompiledValue_Json,
     NodeInputVariableCompiledValue_Number,
     NodeInputVariableCompiledValue_SearchResults,
     NodeInputVariableCompiledValue_String,
     NodeOutputCompiledArrayValue,
     NodeOutputCompiledChatHistoryValue,
     NodeOutputCompiledErrorValue,
@@ -176,17 +220,20 @@
     NodeOutputCompiledValue_Number,
     NodeOutputCompiledValue_SearchResults,
     NodeOutputCompiledValue_String,
     NormalizedLogProbs,
     NormalizedTokenLogProbs,
     NumberEnum,
     NumberVariableValue,
+    PaginatedDocumentIndexReadList,
     PaginatedSlimDeploymentReadList,
     PaginatedSlimDocumentList,
     PaginatedSlimWorkflowDeploymentList,
+    PaginatedTestSuiteRunExecutionList,
+    PaginatedTestSuiteTestCaseList,
     ProcessingFailureReasonEnum,
     ProcessingStateEnum,
     PromptDeploymentExpandMetaRequestRequest,
     PromptDeploymentInputRequest,
     PromptDeploymentInputRequest_ChatHistory,
     PromptDeploymentInputRequest_Json,
     PromptDeploymentInputRequest_String,
@@ -194,43 +241,28 @@
     PromptNodeResult,
     PromptNodeResultData,
     PromptOutput,
     PromptOutput_Error,
     PromptOutput_FunctionCall,
     PromptOutput_Json,
     PromptOutput_String,
-    PromptTemplateBlock,
-    PromptTemplateBlockData,
-    PromptTemplateBlockDataRequest,
-    PromptTemplateBlockProperties,
-    PromptTemplateBlockPropertiesRequest,
-    PromptTemplateBlockRequest,
-    ProviderEnum,
     RawPromptExecutionOverridesRequest,
-    RegisterPromptErrorResponse,
-    RegisterPromptModelParametersRequest,
-    RegisterPromptPrompt,
-    RegisterPromptPromptInfoRequest,
-    RegisterPromptResponse,
-    RegisteredPromptDeployment,
-    RegisteredPromptInputVariableRequest,
-    RegisteredPromptModelVersion,
-    RegisteredPromptSandbox,
-    RegisteredPromptSandboxSnapshot,
     RejectedEnum,
     RejectedExecutePromptEvent,
     RejectedExecutePromptResponse,
     RejectedExecuteWorkflowWorkflowResultEvent,
     RejectedFunctionCall,
     RejectedPromptExecutionMeta,
     RejectedWorkflowNodeResultEvent,
     SandboxScenario,
     ScenarioInput,
-    ScenarioInputRequest,
-    ScenarioInputTypeEnum,
+    ScenarioInputChatHistoryVariableValue,
+    ScenarioInputStringVariableValue,
+    ScenarioInput_ChatHistory,
+    ScenarioInput_String,
     SearchErrorResponse,
     SearchFiltersRequest,
     SearchNodeResult,
     SearchNodeResultData,
     SearchRequestOptionsRequest,
     SearchResponse,
     SearchResult,
@@ -257,23 +289,27 @@
     SubmitCompletionActualsErrorResponse,
     SubmitWorkflowExecutionActualRequest,
     SubmitWorkflowExecutionActualRequest_ChatHistory,
     SubmitWorkflowExecutionActualRequest_Json,
     SubmitWorkflowExecutionActualRequest_String,
     SubworkflowEnum,
     SubworkflowNodeResult,
+    TemplatingNodeArrayResult,
     TemplatingNodeChatHistoryResult,
     TemplatingNodeErrorResult,
+    TemplatingNodeFunctionCallResult,
     TemplatingNodeJsonResult,
     TemplatingNodeNumberResult,
     TemplatingNodeResult,
     TemplatingNodeResultData,
     TemplatingNodeResultOutput,
+    TemplatingNodeResultOutput_Array,
     TemplatingNodeResultOutput_ChatHistory,
     TemplatingNodeResultOutput_Error,
+    TemplatingNodeResultOutput_FunctionCall,
     TemplatingNodeResultOutput_Json,
     TemplatingNodeResultOutput_Number,
     TemplatingNodeResultOutput_SearchResults,
     TemplatingNodeResultOutput_String,
     TemplatingNodeSearchResultsResult,
     TemplatingNodeStringResult,
     TerminalNodeArrayResult,
@@ -293,25 +329,81 @@
     TerminalNodeResultOutput_Number,
     TerminalNodeResultOutput_SearchResults,
     TerminalNodeResultOutput_String,
     TerminalNodeSearchResultsResult,
     TerminalNodeStringResult,
     TestCaseChatHistoryVariableValue,
     TestCaseErrorVariableValue,
+    TestCaseFunctionCallVariableValue,
     TestCaseJsonVariableValue,
     TestCaseNumberVariableValue,
     TestCaseSearchResultsVariableValue,
     TestCaseStringVariableValue,
     TestCaseVariableValue,
     TestCaseVariableValue_ChatHistory,
     TestCaseVariableValue_Error,
+    TestCaseVariableValue_FunctionCall,
     TestCaseVariableValue_Json,
     TestCaseVariableValue_Number,
     TestCaseVariableValue_SearchResults,
     TestCaseVariableValue_String,
+    TestSuiteRunDeploymentReleaseTagExecConfig,
+    TestSuiteRunDeploymentReleaseTagExecConfigData,
+    TestSuiteRunDeploymentReleaseTagExecConfigDataRequest,
+    TestSuiteRunDeploymentReleaseTagExecConfigRequest,
+    TestSuiteRunDeploymentReleaseTagExecConfigTypeEnum,
+    TestSuiteRunExecConfig,
+    TestSuiteRunExecConfigRequest,
+    TestSuiteRunExecConfigRequest_DeploymentReleaseTag,
+    TestSuiteRunExecConfigRequest_External,
+    TestSuiteRunExecConfigRequest_WorkflowReleaseTag,
+    TestSuiteRunExecConfig_DeploymentReleaseTag,
+    TestSuiteRunExecConfig_External,
+    TestSuiteRunExecConfig_WorkflowReleaseTag,
+    TestSuiteRunExecution,
+    TestSuiteRunExecutionChatHistoryOutput,
+    TestSuiteRunExecutionErrorOutput,
+    TestSuiteRunExecutionFunctionCallOutput,
+    TestSuiteRunExecutionJsonOutput,
+    TestSuiteRunExecutionMetricDefinition,
+    TestSuiteRunExecutionMetricResult,
+    TestSuiteRunExecutionNumberOutput,
+    TestSuiteRunExecutionOutput,
+    TestSuiteRunExecutionOutput_ChatHistory,
+    TestSuiteRunExecutionOutput_Error,
+    TestSuiteRunExecutionOutput_FunctionCall,
+    TestSuiteRunExecutionOutput_Json,
+    TestSuiteRunExecutionOutput_Number,
+    TestSuiteRunExecutionOutput_SearchResults,
+    TestSuiteRunExecutionOutput_String,
+    TestSuiteRunExecutionSearchResultsOutput,
+    TestSuiteRunExecutionStringOutput,
+    TestSuiteRunExternalExecConfig,
+    TestSuiteRunExternalExecConfigData,
+    TestSuiteRunExternalExecConfigDataRequest,
+    TestSuiteRunExternalExecConfigRequest,
+    TestSuiteRunExternalExecConfigTypeEnum,
+    TestSuiteRunMetricErrorOutput,
+    TestSuiteRunMetricErrorOutputTypeEnum,
+    TestSuiteRunMetricNumberOutput,
+    TestSuiteRunMetricNumberOutputTypeEnum,
+    TestSuiteRunMetricOutput,
+    TestSuiteRunMetricOutput_Error,
+    TestSuiteRunMetricOutput_Number,
+    TestSuiteRunMetricOutput_String,
+    TestSuiteRunMetricStringOutput,
+    TestSuiteRunMetricStringOutputTypeEnum,
+    TestSuiteRunRead,
+    TestSuiteRunState,
+    TestSuiteRunTestSuite,
+    TestSuiteRunWorkflowReleaseTagExecConfig,
+    TestSuiteRunWorkflowReleaseTagExecConfigData,
+    TestSuiteRunWorkflowReleaseTagExecConfigDataRequest,
+    TestSuiteRunWorkflowReleaseTagExecConfigRequest,
+    TestSuiteRunWorkflowReleaseTagExecConfigTypeEnum,
     TestSuiteTestCase,
     UploadDocumentErrorResponse,
     UploadDocumentResponse,
     VellumError,
     VellumErrorCodeEnum,
     VellumErrorRequest,
     VellumImage,
@@ -388,29 +480,30 @@
     WorkflowResultEventOutputData_Number,
     WorkflowResultEventOutputData_SearchResults,
     WorkflowResultEventOutputData_String,
     WorkflowStreamEvent,
     WorkflowStreamEvent_Node,
     WorkflowStreamEvent_Workflow,
 )
-from .errors import BadRequestError, ConflictError, ForbiddenError, InternalServerError, NotFoundError
+from .errors import BadRequestError, ForbiddenError, InternalServerError, NotFoundError
 from .resources import (
     DeploymentsListRequestStatus,
+    DocumentIndexesListRequestStatus,
     WorkflowDeploymentsListRequestStatus,
     deployments,
     document_indexes,
     documents,
     folder_entities,
-    model_versions,
-    registered_prompts,
     sandboxes,
+    test_suite_runs,
     test_suites,
     workflow_deployments,
 )
 from .environment import VellumEnvironment
+from .version import __version__
 
 __all__ = [
     "ApiNodeResult",
     "ApiNodeResultData",
     "ArrayChatMessageContent",
     "ArrayChatMessageContentItem",
     "ArrayChatMessageContentItemRequest",
@@ -422,20 +515,20 @@
     "ArrayChatMessageContentItem_String",
     "ArrayChatMessageContentRequest",
     "ArrayEnum",
     "ArrayVariableValueItem",
     "ArrayVariableValueItem_ChatHistory",
     "ArrayVariableValueItem_Error",
     "ArrayVariableValueItem_FunctionCall",
+    "ArrayVariableValueItem_Image",
     "ArrayVariableValueItem_Json",
     "ArrayVariableValueItem_Number",
     "ArrayVariableValueItem_SearchResults",
     "ArrayVariableValueItem_String",
     "BadRequestError",
-    "BlockTypeEnum",
     "ChatHistoryEnum",
     "ChatHistoryInputRequest",
     "ChatHistoryVariableValue",
     "ChatMessage",
     "ChatMessageContent",
     "ChatMessageContentRequest",
     "ChatMessageContentRequest_Array",
@@ -444,37 +537,41 @@
     "ChatMessageContentRequest_String",
     "ChatMessageContent_Array",
     "ChatMessageContent_FunctionCall",
     "ChatMessageContent_Image",
     "ChatMessageContent_String",
     "ChatMessageRequest",
     "ChatMessageRole",
+    "CodeExecutionNodeArrayResult",
     "CodeExecutionNodeChatHistoryResult",
     "CodeExecutionNodeErrorResult",
+    "CodeExecutionNodeFunctionCallResult",
     "CodeExecutionNodeJsonResult",
     "CodeExecutionNodeNumberResult",
     "CodeExecutionNodeResult",
     "CodeExecutionNodeResultData",
     "CodeExecutionNodeResultOutput",
+    "CodeExecutionNodeResultOutput_Array",
     "CodeExecutionNodeResultOutput_ChatHistory",
     "CodeExecutionNodeResultOutput_Error",
+    "CodeExecutionNodeResultOutput_FunctionCall",
     "CodeExecutionNodeResultOutput_Json",
     "CodeExecutionNodeResultOutput_Number",
     "CodeExecutionNodeResultOutput_SearchResults",
     "CodeExecutionNodeResultOutput_String",
     "CodeExecutionNodeSearchResultsResult",
     "CodeExecutionNodeStringResult",
     "ConditionalNodeResult",
     "ConditionalNodeResultData",
-    "ConflictError",
     "DeploymentProviderPayloadResponse",
     "DeploymentRead",
     "DeploymentsListRequestStatus",
     "DocumentDocumentToDocumentIndex",
     "DocumentIndexRead",
+    "DocumentIndexesListRequestStatus",
     "DocumentRead",
     "DocumentStatus",
     "EnrichedNormalizedCompletion",
     "EntityStatus",
     "EnvironmentEnum",
     "ErrorEnum",
     "ErrorVariableValue",
@@ -489,21 +586,41 @@
     "ExecutePromptResponse_Rejected",
     "ExecuteWorkflowErrorResponse",
     "ExecuteWorkflowResponse",
     "ExecuteWorkflowStreamErrorResponse",
     "ExecuteWorkflowWorkflowResultEvent",
     "ExecuteWorkflowWorkflowResultEvent_Fulfilled",
     "ExecuteWorkflowWorkflowResultEvent_Rejected",
+    "ExecutionArrayVellumValue",
+    "ExecutionChatHistoryVellumValue",
+    "ExecutionErrorVellumValue",
+    "ExecutionFunctionCallVellumValue",
+    "ExecutionJsonVellumValue",
+    "ExecutionNumberVellumValue",
+    "ExecutionSearchResultsVellumValue",
+    "ExecutionStringVellumValue",
+    "ExecutionVellumValue",
+    "ExecutionVellumValue_Array",
+    "ExecutionVellumValue_ChatHistory",
+    "ExecutionVellumValue_Error",
+    "ExecutionVellumValue_FunctionCall",
+    "ExecutionVellumValue_Json",
+    "ExecutionVellumValue_Number",
+    "ExecutionVellumValue_SearchResults",
+    "ExecutionVellumValue_String",
+    "ExternalTestCaseExecution",
+    "ExternalTestCaseExecutionRequest",
     "FinishReasonEnum",
     "ForbiddenError",
     "FulfilledEnum",
     "FulfilledExecutePromptEvent",
     "FulfilledExecutePromptResponse",
     "FulfilledExecuteWorkflowWorkflowResultEvent",
     "FulfilledFunctionCall",
+    "FulfilledFunctionCallRequest",
     "FulfilledPromptExecutionMeta",
     "FulfilledWorkflowNodeResultEvent",
     "FunctionCall",
     "FunctionCallChatMessageContent",
     "FunctionCallChatMessageContentRequest",
     "FunctionCallChatMessageContentValue",
     "FunctionCallChatMessageContentValueRequest",
@@ -520,58 +637,78 @@
     "GenerateResultError",
     "GenerateStreamResponse",
     "GenerateStreamResult",
     "GenerateStreamResultData",
     "ImageChatMessageContent",
     "ImageChatMessageContentRequest",
     "ImageEnum",
+    "ImageVariableValue",
     "IndexingStateEnum",
     "InitiatedEnum",
     "InitiatedExecutePromptEvent",
     "InitiatedPromptExecutionMeta",
     "InitiatedWorkflowNodeResultEvent",
     "InternalServerError",
     "JsonEnum",
     "JsonInputRequest",
     "JsonVariableValue",
     "LogicalOperator",
     "LogprobsEnum",
     "MetadataFilterConfigRequest",
     "MetadataFilterRuleCombinator",
     "MetadataFilterRuleRequest",
-    "ModelVersionBuildConfig",
-    "ModelVersionExecConfig",
-    "ModelVersionExecConfigParameters",
-    "ModelVersionRead",
-    "ModelVersionReadStatusEnum",
-    "ModelVersionSandboxSnapshot",
+    "MlModelUsage",
+    "NamedScenarioInputChatHistoryVariableValueRequest",
+    "NamedScenarioInputRequest",
+    "NamedScenarioInputRequest_ChatHistory",
+    "NamedScenarioInputRequest_String",
+    "NamedScenarioInputStringVariableValueRequest",
+    "NamedTestCaseChatHistoryVariableValue",
     "NamedTestCaseChatHistoryVariableValueRequest",
+    "NamedTestCaseErrorVariableValue",
     "NamedTestCaseErrorVariableValueRequest",
+    "NamedTestCaseFunctionCallVariableValue",
+    "NamedTestCaseFunctionCallVariableValueRequest",
+    "NamedTestCaseJsonVariableValue",
     "NamedTestCaseJsonVariableValueRequest",
+    "NamedTestCaseNumberVariableValue",
     "NamedTestCaseNumberVariableValueRequest",
+    "NamedTestCaseSearchResultsVariableValue",
     "NamedTestCaseSearchResultsVariableValueRequest",
+    "NamedTestCaseStringVariableValue",
     "NamedTestCaseStringVariableValueRequest",
+    "NamedTestCaseVariableValue",
     "NamedTestCaseVariableValueRequest",
     "NamedTestCaseVariableValueRequest_ChatHistory",
     "NamedTestCaseVariableValueRequest_Error",
+    "NamedTestCaseVariableValueRequest_FunctionCall",
     "NamedTestCaseVariableValueRequest_Json",
     "NamedTestCaseVariableValueRequest_Number",
     "NamedTestCaseVariableValueRequest_SearchResults",
     "NamedTestCaseVariableValueRequest_String",
+    "NamedTestCaseVariableValue_ChatHistory",
+    "NamedTestCaseVariableValue_Error",
+    "NamedTestCaseVariableValue_FunctionCall",
+    "NamedTestCaseVariableValue_Json",
+    "NamedTestCaseVariableValue_Number",
+    "NamedTestCaseVariableValue_SearchResults",
+    "NamedTestCaseVariableValue_String",
     "NodeInputCompiledArrayValue",
     "NodeInputCompiledChatHistoryValue",
     "NodeInputCompiledErrorValue",
+    "NodeInputCompiledFunctionCall",
     "NodeInputCompiledJsonValue",
     "NodeInputCompiledNumberValue",
     "NodeInputCompiledSearchResultsValue",
     "NodeInputCompiledStringValue",
     "NodeInputVariableCompiledValue",
     "NodeInputVariableCompiledValue_Array",
     "NodeInputVariableCompiledValue_ChatHistory",
     "NodeInputVariableCompiledValue_Error",
+    "NodeInputVariableCompiledValue_FunctionCall",
     "NodeInputVariableCompiledValue_Json",
     "NodeInputVariableCompiledValue_Number",
     "NodeInputVariableCompiledValue_SearchResults",
     "NodeInputVariableCompiledValue_String",
     "NodeOutputCompiledArrayValue",
     "NodeOutputCompiledChatHistoryValue",
     "NodeOutputCompiledErrorValue",
@@ -590,17 +727,20 @@
     "NodeOutputCompiledValue_SearchResults",
     "NodeOutputCompiledValue_String",
     "NormalizedLogProbs",
     "NormalizedTokenLogProbs",
     "NotFoundError",
     "NumberEnum",
     "NumberVariableValue",
+    "PaginatedDocumentIndexReadList",
     "PaginatedSlimDeploymentReadList",
     "PaginatedSlimDocumentList",
     "PaginatedSlimWorkflowDeploymentList",
+    "PaginatedTestSuiteRunExecutionList",
+    "PaginatedTestSuiteTestCaseList",
     "ProcessingFailureReasonEnum",
     "ProcessingStateEnum",
     "PromptDeploymentExpandMetaRequestRequest",
     "PromptDeploymentInputRequest",
     "PromptDeploymentInputRequest_ChatHistory",
     "PromptDeploymentInputRequest_Json",
     "PromptDeploymentInputRequest_String",
@@ -608,43 +748,28 @@
     "PromptNodeResult",
     "PromptNodeResultData",
     "PromptOutput",
     "PromptOutput_Error",
     "PromptOutput_FunctionCall",
     "PromptOutput_Json",
     "PromptOutput_String",
-    "PromptTemplateBlock",
-    "PromptTemplateBlockData",
-    "PromptTemplateBlockDataRequest",
-    "PromptTemplateBlockProperties",
-    "PromptTemplateBlockPropertiesRequest",
-    "PromptTemplateBlockRequest",
-    "ProviderEnum",
     "RawPromptExecutionOverridesRequest",
-    "RegisterPromptErrorResponse",
-    "RegisterPromptModelParametersRequest",
-    "RegisterPromptPrompt",
-    "RegisterPromptPromptInfoRequest",
-    "RegisterPromptResponse",
-    "RegisteredPromptDeployment",
-    "RegisteredPromptInputVariableRequest",
-    "RegisteredPromptModelVersion",
-    "RegisteredPromptSandbox",
-    "RegisteredPromptSandboxSnapshot",
     "RejectedEnum",
     "RejectedExecutePromptEvent",
     "RejectedExecutePromptResponse",
     "RejectedExecuteWorkflowWorkflowResultEvent",
     "RejectedFunctionCall",
     "RejectedPromptExecutionMeta",
     "RejectedWorkflowNodeResultEvent",
     "SandboxScenario",
     "ScenarioInput",
-    "ScenarioInputRequest",
-    "ScenarioInputTypeEnum",
+    "ScenarioInputChatHistoryVariableValue",
+    "ScenarioInputStringVariableValue",
+    "ScenarioInput_ChatHistory",
+    "ScenarioInput_String",
     "SearchErrorResponse",
     "SearchFiltersRequest",
     "SearchNodeResult",
     "SearchNodeResultData",
     "SearchRequestOptionsRequest",
     "SearchResponse",
     "SearchResult",
@@ -671,23 +796,27 @@
     "SubmitCompletionActualsErrorResponse",
     "SubmitWorkflowExecutionActualRequest",
     "SubmitWorkflowExecutionActualRequest_ChatHistory",
     "SubmitWorkflowExecutionActualRequest_Json",
     "SubmitWorkflowExecutionActualRequest_String",
     "SubworkflowEnum",
     "SubworkflowNodeResult",
+    "TemplatingNodeArrayResult",
     "TemplatingNodeChatHistoryResult",
     "TemplatingNodeErrorResult",
+    "TemplatingNodeFunctionCallResult",
     "TemplatingNodeJsonResult",
     "TemplatingNodeNumberResult",
     "TemplatingNodeResult",
     "TemplatingNodeResultData",
     "TemplatingNodeResultOutput",
+    "TemplatingNodeResultOutput_Array",
     "TemplatingNodeResultOutput_ChatHistory",
     "TemplatingNodeResultOutput_Error",
+    "TemplatingNodeResultOutput_FunctionCall",
     "TemplatingNodeResultOutput_Json",
     "TemplatingNodeResultOutput_Number",
     "TemplatingNodeResultOutput_SearchResults",
     "TemplatingNodeResultOutput_String",
     "TemplatingNodeSearchResultsResult",
     "TemplatingNodeStringResult",
     "TerminalNodeArrayResult",
@@ -707,25 +836,81 @@
     "TerminalNodeResultOutput_Number",
     "TerminalNodeResultOutput_SearchResults",
     "TerminalNodeResultOutput_String",
     "TerminalNodeSearchResultsResult",
     "TerminalNodeStringResult",
     "TestCaseChatHistoryVariableValue",
     "TestCaseErrorVariableValue",
+    "TestCaseFunctionCallVariableValue",
     "TestCaseJsonVariableValue",
     "TestCaseNumberVariableValue",
     "TestCaseSearchResultsVariableValue",
     "TestCaseStringVariableValue",
     "TestCaseVariableValue",
     "TestCaseVariableValue_ChatHistory",
     "TestCaseVariableValue_Error",
+    "TestCaseVariableValue_FunctionCall",
     "TestCaseVariableValue_Json",
     "TestCaseVariableValue_Number",
     "TestCaseVariableValue_SearchResults",
     "TestCaseVariableValue_String",
+    "TestSuiteRunDeploymentReleaseTagExecConfig",
+    "TestSuiteRunDeploymentReleaseTagExecConfigData",
+    "TestSuiteRunDeploymentReleaseTagExecConfigDataRequest",
+    "TestSuiteRunDeploymentReleaseTagExecConfigRequest",
+    "TestSuiteRunDeploymentReleaseTagExecConfigTypeEnum",
+    "TestSuiteRunExecConfig",
+    "TestSuiteRunExecConfigRequest",
+    "TestSuiteRunExecConfigRequest_DeploymentReleaseTag",
+    "TestSuiteRunExecConfigRequest_External",
+    "TestSuiteRunExecConfigRequest_WorkflowReleaseTag",
+    "TestSuiteRunExecConfig_DeploymentReleaseTag",
+    "TestSuiteRunExecConfig_External",
+    "TestSuiteRunExecConfig_WorkflowReleaseTag",
+    "TestSuiteRunExecution",
+    "TestSuiteRunExecutionChatHistoryOutput",
+    "TestSuiteRunExecutionErrorOutput",
+    "TestSuiteRunExecutionFunctionCallOutput",
+    "TestSuiteRunExecutionJsonOutput",
+    "TestSuiteRunExecutionMetricDefinition",
+    "TestSuiteRunExecutionMetricResult",
+    "TestSuiteRunExecutionNumberOutput",
+    "TestSuiteRunExecutionOutput",
+    "TestSuiteRunExecutionOutput_ChatHistory",
+    "TestSuiteRunExecutionOutput_Error",
+    "TestSuiteRunExecutionOutput_FunctionCall",
+    "TestSuiteRunExecutionOutput_Json",
+    "TestSuiteRunExecutionOutput_Number",
+    "TestSuiteRunExecutionOutput_SearchResults",
+    "TestSuiteRunExecutionOutput_String",
+    "TestSuiteRunExecutionSearchResultsOutput",
+    "TestSuiteRunExecutionStringOutput",
+    "TestSuiteRunExternalExecConfig",
+    "TestSuiteRunExternalExecConfigData",
+    "TestSuiteRunExternalExecConfigDataRequest",
+    "TestSuiteRunExternalExecConfigRequest",
+    "TestSuiteRunExternalExecConfigTypeEnum",
+    "TestSuiteRunMetricErrorOutput",
+    "TestSuiteRunMetricErrorOutputTypeEnum",
+    "TestSuiteRunMetricNumberOutput",
+    "TestSuiteRunMetricNumberOutputTypeEnum",
+    "TestSuiteRunMetricOutput",
+    "TestSuiteRunMetricOutput_Error",
+    "TestSuiteRunMetricOutput_Number",
+    "TestSuiteRunMetricOutput_String",
+    "TestSuiteRunMetricStringOutput",
+    "TestSuiteRunMetricStringOutputTypeEnum",
+    "TestSuiteRunRead",
+    "TestSuiteRunState",
+    "TestSuiteRunTestSuite",
+    "TestSuiteRunWorkflowReleaseTagExecConfig",
+    "TestSuiteRunWorkflowReleaseTagExecConfigData",
+    "TestSuiteRunWorkflowReleaseTagExecConfigDataRequest",
+    "TestSuiteRunWorkflowReleaseTagExecConfigRequest",
+    "TestSuiteRunWorkflowReleaseTagExecConfigTypeEnum",
     "TestSuiteTestCase",
     "UploadDocumentErrorResponse",
     "UploadDocumentResponse",
     "VellumEnvironment",
     "VellumError",
     "VellumErrorCodeEnum",
     "VellumErrorRequest",
@@ -803,17 +988,17 @@
     "WorkflowResultEventOutputData_Json",
     "WorkflowResultEventOutputData_Number",
     "WorkflowResultEventOutputData_SearchResults",
     "WorkflowResultEventOutputData_String",
     "WorkflowStreamEvent",
     "WorkflowStreamEvent_Node",
     "WorkflowStreamEvent_Workflow",
+    "__version__",
     "deployments",
     "document_indexes",
     "documents",
     "folder_entities",
-    "model_versions",
-    "registered_prompts",
     "sandboxes",
+    "test_suite_runs",
     "test_suites",
     "workflow_deployments",
 ]
```

### Comparing `vellum_ai-0.3.9/src/vellum/core/client_wrapper.py` & `vellum_ai-0.5.0/src/vellum/core/client_wrapper.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,56 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import typing
 
 import httpx
 
 from ..environment import VellumEnvironment
+from .http_client import AsyncHttpClient, HttpClient
 
 
 class BaseClientWrapper:
-    def __init__(self, *, api_key: str, environment: VellumEnvironment):
+    def __init__(self, *, api_key: str, environment: VellumEnvironment, timeout: typing.Optional[float] = None):
         self.api_key = api_key
         self._environment = environment
+        self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "vellum-ai",
-            "X-Fern-SDK-Version": "0.3.9",
+            "X-Fern-SDK-Version": "0.5.0",
         }
         headers["X_API_KEY"] = self.api_key
         return headers
 
     def get_environment(self) -> VellumEnvironment:
         return self._environment
 
+    def get_timeout(self) -> typing.Optional[float]:
+        return self._timeout
+
 
 class SyncClientWrapper(BaseClientWrapper):
-    def __init__(self, *, api_key: str, environment: VellumEnvironment, httpx_client: httpx.Client):
-        super().__init__(api_key=api_key, environment=environment)
-        self.httpx_client = httpx_client
+    def __init__(
+        self,
+        *,
+        api_key: str,
+        environment: VellumEnvironment,
+        timeout: typing.Optional[float] = None,
+        httpx_client: httpx.Client
+    ):
+        super().__init__(api_key=api_key, environment=environment, timeout=timeout)
+        self.httpx_client = HttpClient(httpx_client=httpx_client)
 
 
 class AsyncClientWrapper(BaseClientWrapper):
-    def __init__(self, *, api_key: str, environment: VellumEnvironment, httpx_client: httpx.AsyncClient):
-        super().__init__(api_key=api_key, environment=environment)
-        self.httpx_client = httpx_client
+    def __init__(
+        self,
+        *,
+        api_key: str,
+        environment: VellumEnvironment,
+        timeout: typing.Optional[float] = None,
+        httpx_client: httpx.AsyncClient
+    ):
+        super().__init__(api_key=api_key, environment=environment, timeout=timeout)
+        self.httpx_client = AsyncHttpClient(httpx_client=httpx_client)
```

### Comparing `vellum_ai-0.3.9/src/vellum/core/datetime_utils.py` & `vellum_ai-0.5.0/src/vellum/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.9/src/vellum/core/jsonable_encoder.py` & `vellum_ai-0.5.0/src/vellum/core/jsonable_encoder.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,47 +12,43 @@
 import datetime as dt
 from collections import defaultdict
 from enum import Enum
 from pathlib import PurePath
 from types import GeneratorType
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 from .datetime_utils import serialize_datetime
+from .pydantic_utilities import pydantic_v1
 
 SetIntStr = Set[Union[int, str]]
 DictIntStrAny = Dict[Union[int, str], Any]
 
 
 def generate_encoders_by_class_tuples(
     type_encoder_map: Dict[Any, Callable[[Any], Any]]
 ) -> Dict[Callable[[Any], Any], Tuple[Any, ...]]:
     encoders_by_class_tuples: Dict[Callable[[Any], Any], Tuple[Any, ...]] = defaultdict(tuple)
     for type_, encoder in type_encoder_map.items():
         encoders_by_class_tuples[encoder] += (type_,)
     return encoders_by_class_tuples
 
 
-encoders_by_class_tuples = generate_encoders_by_class_tuples(pydantic.json.ENCODERS_BY_TYPE)
+encoders_by_class_tuples = generate_encoders_by_class_tuples(pydantic_v1.json.ENCODERS_BY_TYPE)
 
 
 def jsonable_encoder(obj: Any, custom_encoder: Optional[Dict[Any, Callable[[Any], Any]]] = None) -> Any:
     custom_encoder = custom_encoder or {}
     if custom_encoder:
         if type(obj) in custom_encoder:
             return custom_encoder[type(obj)](obj)
         else:
             for encoder_type, encoder_instance in custom_encoder.items():
                 if isinstance(obj, encoder_type):
                     return encoder_instance(obj)
-    if isinstance(obj, pydantic.BaseModel):
+    if isinstance(obj, pydantic_v1.BaseModel):
         encoder = getattr(obj.__config__, "json_encoders", {})
         if custom_encoder:
             encoder.update(custom_encoder)
         obj_dict = obj.dict(by_alias=True)
         if "__root__" in obj_dict:
             obj_dict = obj_dict["__root__"]
         return jsonable_encoder(obj_dict, custom_encoder=encoder)
@@ -61,18 +57,18 @@
         return jsonable_encoder(obj_dict, custom_encoder=custom_encoder)
     if isinstance(obj, Enum):
         return obj.value
     if isinstance(obj, PurePath):
         return str(obj)
     if isinstance(obj, (str, int, float, type(None))):
         return obj
-    if isinstance(obj, dt.date):
-        return str(obj)
     if isinstance(obj, dt.datetime):
         return serialize_datetime(obj)
+    if isinstance(obj, dt.date):
+        return str(obj)
     if isinstance(obj, dict):
         encoded_dict = {}
         allowed_keys = set(obj.keys())
         for key, value in obj.items():
             if key in allowed_keys:
                 encoded_key = jsonable_encoder(key, custom_encoder=custom_encoder)
                 encoded_value = jsonable_encoder(value, custom_encoder=custom_encoder)
@@ -80,16 +76,16 @@
         return encoded_dict
     if isinstance(obj, (list, set, frozenset, GeneratorType, tuple)):
         encoded_list = []
         for item in obj:
             encoded_list.append(jsonable_encoder(item, custom_encoder=custom_encoder))
         return encoded_list
 
-    if type(obj) in pydantic.json.ENCODERS_BY_TYPE:
-        return pydantic.json.ENCODERS_BY_TYPE[type(obj)](obj)
+    if type(obj) in pydantic_v1.json.ENCODERS_BY_TYPE:
+        return pydantic_v1.json.ENCODERS_BY_TYPE[type(obj)](obj)
     for encoder, classes_tuple in encoders_by_class_tuples.items():
         if isinstance(obj, classes_tuple):
             return encoder(obj)
 
     try:
         data = dict(obj)
     except Exception as e:
```

### Comparing `vellum_ai-0.3.9/src/vellum/resources/__init__.py` & `vellum_ai-0.5.0/src/vellum/resources/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from . import (
     deployments,
     document_indexes,
     documents,
     folder_entities,
-    model_versions,
-    registered_prompts,
     sandboxes,
+    test_suite_runs,
     test_suites,
     workflow_deployments,
 )
 from .deployments import DeploymentsListRequestStatus
+from .document_indexes import DocumentIndexesListRequestStatus
 from .workflow_deployments import WorkflowDeploymentsListRequestStatus
 
 __all__ = [
     "DeploymentsListRequestStatus",
+    "DocumentIndexesListRequestStatus",
     "WorkflowDeploymentsListRequestStatus",
     "deployments",
     "document_indexes",
     "documents",
     "folder_entities",
-    "model_versions",
-    "registered_prompts",
     "sandboxes",
+    "test_suite_runs",
     "test_suites",
     "workflow_deployments",
 ]
```

### Comparing `vellum_ai-0.3.9/src/vellum/resources/deployments/client.py` & `vellum_ai-0.5.0/src/vellum/resources/workflow_deployments/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,263 +3,257 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ...core.api_error import ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
+from ...core.pydantic_utilities import pydantic_v1
 from ...core.remove_none_from_dict import remove_none_from_dict
-from ...types.deployment_provider_payload_response import DeploymentProviderPayloadResponse
-from ...types.deployment_read import DeploymentRead
-from ...types.paginated_slim_deployment_read_list import PaginatedSlimDeploymentReadList
-from ...types.prompt_deployment_input_request import PromptDeploymentInputRequest
-from .types.deployments_list_request_status import DeploymentsListRequestStatus
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
+from ...core.request_options import RequestOptions
+from ...types.paginated_slim_workflow_deployment_list import PaginatedSlimWorkflowDeploymentList
+from ...types.workflow_deployment_read import WorkflowDeploymentRead
+from .types.workflow_deployments_list_request_status import WorkflowDeploymentsListRequestStatus
 
-# this is used as the default value for optional parameters
-OMIT = typing.cast(typing.Any, ...)
 
-
-class DeploymentsClient:
+class WorkflowDeploymentsClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def list(
         self,
         *,
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
         ordering: typing.Optional[str] = None,
-        status: typing.Optional[DeploymentsListRequestStatus] = None,
-    ) -> PaginatedSlimDeploymentReadList:
+        status: typing.Optional[WorkflowDeploymentsListRequestStatus] = None,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> PaginatedSlimWorkflowDeploymentList:
         """
         Parameters:
             - limit: typing.Optional[int]. Number of results to return per page.
 
             - offset: typing.Optional[int]. The initial index from which to return the results.
 
             - ordering: typing.Optional[str]. Which field to use when ordering the results.
 
-            - status: typing.Optional[DeploymentsListRequestStatus]. status
-        ---
-        from vellum.client import Vellum
-
-        client = Vellum(
-            api_key="YOUR_API_KEY",
-        )
-        client.deployments.list()
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_environment().default}/", "v1/deployments"),
-            params=remove_none_from_dict({"limit": limit, "offset": offset, "ordering": ordering, "status": status}),
-            headers=self._client_wrapper.get_headers(),
-            timeout=None,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PaginatedSlimDeploymentReadList, _response.json())  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def retrieve(self, id: str) -> DeploymentRead:
-        """
-        Used to retrieve a deployment given its ID or name.
+            - status: typing.Optional[WorkflowDeploymentsListRequestStatus]. status
 
-        Parameters:
-            - id: str. Either the Deployment's ID or its unique name
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from vellum.client import Vellum
 
         client = Vellum(
             api_key="YOUR_API_KEY",
         )
-        client.deployments.retrieve(
-            id="id",
-        )
+        client.workflow_deployments.list()
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_environment().default}/", f"v1/deployments/{id}"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=None,
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_environment().default}/", "v1/workflow-deployments"),
+            params=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        "limit": limit,
+                        "offset": offset,
+                        "ordering": ordering,
+                        "status": status,
+                        **(
+                            request_options.get("additional_query_parameters", {})
+                            if request_options is not None
+                            else {}
+                        ),
+                    }
+                )
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DeploymentRead, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(PaginatedSlimWorkflowDeploymentList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def retrieve_provider_payload(
-        self,
-        *,
-        deployment_id: typing.Optional[str] = OMIT,
-        deployment_name: typing.Optional[str] = OMIT,
-        inputs: typing.List[PromptDeploymentInputRequest],
-    ) -> DeploymentProviderPayloadResponse:
+    def retrieve(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> WorkflowDeploymentRead:
         """
-        Parameters:
-            - deployment_id: typing.Optional[str]. The ID of the deployment. Must provide either this or deployment_name.
+        Used to retrieve a workflow deployment given its ID or name.
 
-            - deployment_name: typing.Optional[str]. The name of the deployment. Must provide either this or deployment_id.
+        Parameters:
+            - id: str. Either the Workflow Deployment's ID or its unique name
 
-            - inputs: typing.List[PromptDeploymentInputRequest]. The list of inputs defined in the Prompt's deployment with their corresponding values.
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from vellum.client import Vellum
 
         client = Vellum(
             api_key="YOUR_API_KEY",
         )
-        client.deployments.retrieve_provider_payload(
-            inputs=[],
+        client.workflow_deployments.retrieve(
+            id="id",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"inputs": inputs}
-        if deployment_id is not OMIT:
-            _request["deployment_id"] = deployment_id
-        if deployment_name is not OMIT:
-            _request["deployment_name"] = deployment_name
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_environment().default}/", "v1/deployments/provider-payload"
+            method="GET",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_environment().default}/", f"v1/workflow-deployments/{jsonable_encoder(id)}"
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
             ),
-            json=jsonable_encoder(_request),
-            headers=self._client_wrapper.get_headers(),
-            timeout=None,
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DeploymentProviderPayloadResponse, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(WorkflowDeploymentRead, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncDeploymentsClient:
+class AsyncWorkflowDeploymentsClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def list(
         self,
         *,
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
         ordering: typing.Optional[str] = None,
-        status: typing.Optional[DeploymentsListRequestStatus] = None,
-    ) -> PaginatedSlimDeploymentReadList:
+        status: typing.Optional[WorkflowDeploymentsListRequestStatus] = None,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> PaginatedSlimWorkflowDeploymentList:
         """
         Parameters:
             - limit: typing.Optional[int]. Number of results to return per page.
 
             - offset: typing.Optional[int]. The initial index from which to return the results.
 
             - ordering: typing.Optional[str]. Which field to use when ordering the results.
 
-            - status: typing.Optional[DeploymentsListRequestStatus]. status
-        ---
-        from vellum.client import AsyncVellum
-
-        client = AsyncVellum(
-            api_key="YOUR_API_KEY",
-        )
-        await client.deployments.list()
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_environment().default}/", "v1/deployments"),
-            params=remove_none_from_dict({"limit": limit, "offset": offset, "ordering": ordering, "status": status}),
-            headers=self._client_wrapper.get_headers(),
-            timeout=None,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PaginatedSlimDeploymentReadList, _response.json())  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            - status: typing.Optional[WorkflowDeploymentsListRequestStatus]. status
 
-    async def retrieve(self, id: str) -> DeploymentRead:
-        """
-        Used to retrieve a deployment given its ID or name.
-
-        Parameters:
-            - id: str. Either the Deployment's ID or its unique name
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from vellum.client import AsyncVellum
 
         client = AsyncVellum(
             api_key="YOUR_API_KEY",
         )
-        await client.deployments.retrieve(
-            id="id",
-        )
+        await client.workflow_deployments.list()
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_environment().default}/", f"v1/deployments/{id}"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=None,
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_environment().default}/", "v1/workflow-deployments"),
+            params=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        "limit": limit,
+                        "offset": offset,
+                        "ordering": ordering,
+                        "status": status,
+                        **(
+                            request_options.get("additional_query_parameters", {})
+                            if request_options is not None
+                            else {}
+                        ),
+                    }
+                )
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DeploymentRead, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(PaginatedSlimWorkflowDeploymentList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def retrieve_provider_payload(
-        self,
-        *,
-        deployment_id: typing.Optional[str] = OMIT,
-        deployment_name: typing.Optional[str] = OMIT,
-        inputs: typing.List[PromptDeploymentInputRequest],
-    ) -> DeploymentProviderPayloadResponse:
+    async def retrieve(
+        self, id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> WorkflowDeploymentRead:
         """
-        Parameters:
-            - deployment_id: typing.Optional[str]. The ID of the deployment. Must provide either this or deployment_name.
+        Used to retrieve a workflow deployment given its ID or name.
 
-            - deployment_name: typing.Optional[str]. The name of the deployment. Must provide either this or deployment_id.
+        Parameters:
+            - id: str. Either the Workflow Deployment's ID or its unique name
 
-            - inputs: typing.List[PromptDeploymentInputRequest]. The list of inputs defined in the Prompt's deployment with their corresponding values.
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from vellum.client import AsyncVellum
 
         client = AsyncVellum(
             api_key="YOUR_API_KEY",
         )
-        await client.deployments.retrieve_provider_payload(
-            inputs=[],
+        await client.workflow_deployments.retrieve(
+            id="id",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"inputs": inputs}
-        if deployment_id is not OMIT:
-            _request["deployment_id"] = deployment_id
-        if deployment_name is not OMIT:
-            _request["deployment_name"] = deployment_name
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_environment().default}/", "v1/deployments/provider-payload"
+            method="GET",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_environment().default}/", f"v1/workflow-deployments/{jsonable_encoder(id)}"
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
             ),
-            json=jsonable_encoder(_request),
-            headers=self._client_wrapper.get_headers(),
-            timeout=None,
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DeploymentProviderPayloadResponse, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(WorkflowDeploymentRead, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `vellum_ai-0.3.9/src/vellum/resources/documents/client.py` & `vellum_ai-0.5.0/src/vellum/resources/deployments/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,413 +3,426 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ...core.api_error import ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
+from ...core.pydantic_utilities import pydantic_v1
 from ...core.remove_none_from_dict import remove_none_from_dict
+from ...core.request_options import RequestOptions
 from ...errors.bad_request_error import BadRequestError
+from ...errors.forbidden_error import ForbiddenError
 from ...errors.internal_server_error import InternalServerError
 from ...errors.not_found_error import NotFoundError
-from ...types.document_read import DocumentRead
-from ...types.document_status import DocumentStatus
-from ...types.paginated_slim_document_list import PaginatedSlimDocumentList
-from ...types.upload_document_response import UploadDocumentResponse
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
+from ...types.deployment_provider_payload_response import DeploymentProviderPayloadResponse
+from ...types.deployment_read import DeploymentRead
+from ...types.paginated_slim_deployment_read_list import PaginatedSlimDeploymentReadList
+from ...types.prompt_deployment_input_request import PromptDeploymentInputRequest
+from .types.deployments_list_request_status import DeploymentsListRequestStatus
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class DocumentsClient:
+class DeploymentsClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def list(
         self,
         *,
-        document_index_id: typing.Optional[str] = None,
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
         ordering: typing.Optional[str] = None,
-    ) -> PaginatedSlimDocumentList:
+        status: typing.Optional[DeploymentsListRequestStatus] = None,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> PaginatedSlimDeploymentReadList:
         """
-        Used to list documents. Optionally filter on supported fields.
-
         Parameters:
-            - document_index_id: typing.Optional[str]. Filter down to only those documents that are included in the specified index. You may provide either the Vellum-generated ID or the unique name of the index specified upon initial creation.
-
             - limit: typing.Optional[int]. Number of results to return per page.
 
             - offset: typing.Optional[int]. The initial index from which to return the results.
 
             - ordering: typing.Optional[str]. Which field to use when ordering the results.
+
+            - status: typing.Optional[DeploymentsListRequestStatus]. status
+
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from vellum.client import Vellum
 
         client = Vellum(
             api_key="YOUR_API_KEY",
         )
-        client.documents.list()
+        client.deployments.list()
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_environment().default}/", "v1/documents"),
-            params=remove_none_from_dict(
-                {"document_index_id": document_index_id, "limit": limit, "offset": offset, "ordering": ordering}
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_environment().default}/", "v1/deployments"),
+            params=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        "limit": limit,
+                        "offset": offset,
+                        "ordering": ordering,
+                        "status": status,
+                        **(
+                            request_options.get("additional_query_parameters", {})
+                            if request_options is not None
+                            else {}
+                        ),
+                    }
+                )
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
             ),
-            headers=self._client_wrapper.get_headers(),
-            timeout=None,
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PaginatedSlimDocumentList, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(PaginatedSlimDeploymentReadList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def destroy(self, id: str) -> None:
+    def retrieve(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> DeploymentRead:
         """
+        Used to retrieve a deployment given its ID or name.
+
         Parameters:
-            - id: str. A UUID string identifying this document.
+            - id: str. Either the Deployment's ID or its unique name
+
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from vellum.client import Vellum
 
         client = Vellum(
             api_key="YOUR_API_KEY",
         )
-        client.documents.destroy(
+        client.deployments.retrieve(
             id="id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_environment().default}/", f"v1/documents/{id}"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=None,
+            method="GET",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_environment().default}/", f"v1/deployments/{jsonable_encoder(id)}"
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
+            return pydantic_v1.parse_obj_as(DeploymentRead, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def partial_update(
+    def retrieve_provider_payload(
         self,
-        id: str,
         *,
-        label: typing.Optional[str] = OMIT,
-        status: typing.Optional[DocumentStatus] = OMIT,
-        metadata: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
-    ) -> DocumentRead:
+        deployment_id: typing.Optional[str] = OMIT,
+        deployment_name: typing.Optional[str] = OMIT,
+        inputs: typing.Sequence[PromptDeploymentInputRequest],
+        release_tag: typing.Optional[str] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> DeploymentProviderPayloadResponse:
         """
-        Update a Document, keying off of its Vellum-generated ID. Particularly useful for updating its metadata.
-
         Parameters:
-            - id: str. A UUID string identifying this document.
+            - deployment_id: typing.Optional[str]. The ID of the deployment. Must provide either this or deployment_name.
+
+            - deployment_name: typing.Optional[str]. The name of the deployment. Must provide either this or deployment_id.
 
-            - label: typing.Optional[str]. A human-readable label for the document. Defaults to the originally uploaded file's file name.
+            - inputs: typing.Sequence[PromptDeploymentInputRequest]. The list of inputs defined in the Prompt's deployment with their corresponding values.
 
-            - status: typing.Optional[DocumentStatus]. The current status of the document
+            - release_tag: typing.Optional[str]. Optionally specify a release tag if you want to pin to a specific release of the Workflow Deployment
 
-                                                       * `ACTIVE` - Active
-            - metadata: typing.Optional[typing.Dict[str, typing.Any]]. A JSON object containing any metadata associated with the document that you'd like to filter upon later.
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from vellum.client import Vellum
 
         client = Vellum(
             api_key="YOUR_API_KEY",
         )
-        client.documents.partial_update(
-            id="id",
+        client.deployments.retrieve_provider_payload(
+            inputs=[],
         )
         """
-        _request: typing.Dict[str, typing.Any] = {}
-        if label is not OMIT:
-            _request["label"] = label
-        if status is not OMIT:
-            _request["status"] = status
-        if metadata is not OMIT:
-            _request["metadata"] = metadata
+        _request: typing.Dict[str, typing.Any] = {"inputs": inputs}
+        if deployment_id is not OMIT:
+            _request["deployment_id"] = deployment_id
+        if deployment_name is not OMIT:
+            _request["deployment_name"] = deployment_name
+        if release_tag is not OMIT:
+            _request["release_tag"] = release_tag
         _response = self._client_wrapper.httpx_client.request(
-            "PATCH",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_environment().default}/", f"v1/documents/{id}"),
-            json=jsonable_encoder(_request),
-            headers=self._client_wrapper.get_headers(),
-            timeout=None,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DocumentRead, _response.json())  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def upload(
-        self,
-        *,
-        add_to_index_names: typing.Optional[typing.List[str]] = None,
-        external_id: typing.Optional[str] = None,
-        label: str,
-        contents: typing.IO,
-        keywords: typing.Optional[typing.List[str]] = None,
-        metadata: typing.Optional[str] = None,
-    ) -> UploadDocumentResponse:
-        """
-        Upload a document to be indexed and used for search.
-
-        **Note:** Uses a base url of `https://documents.vellum.ai`.
-
-        This is a multipart/form-data request. The `contents` field should be a file upload. It also expects a JSON body with the following fields:
-
-        - `add_to_index_names: list[str]` - Optionally include the names of all indexes that you'd like this document to be included in
-        - `external_id: str | None` - Optionally include an external ID for this document. This is useful if you want to re-upload the same document later when its contents change and would like it to be re-indexed.
-        - `label: str` - A human-friendly name for this document. Typically the filename.
-        - `keywords: list[str] | None` - Optionally include a list of keywords that'll be associated with this document. Used when performing keyword searches.
-        - `metadata: dict[str, Any]` - A stringified JSON object containing any metadata associated with the document that you'd like to filter upon later.
-
-        Parameters:
-            - add_to_index_names: typing.Optional[typing.List[str]].
-
-            - external_id: typing.Optional[str].
-
-            - label: str.
-
-            - contents: typing.IO.
-
-            - keywords: typing.Optional[typing.List[str]].
-
-            - metadata: typing.Optional[str].
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_environment().documents}/", "v1/upload-document"),
-            data=jsonable_encoder(
-                {
-                    "add_to_index_names": add_to_index_names,
-                    "external_id": external_id,
-                    "label": label,
-                    "keywords": keywords,
-                    "metadata": metadata,
-                }
-            ),
-            files={"contents": contents},
-            headers=self._client_wrapper.get_headers(),
-            timeout=None,
+            method="POST",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_environment().default}/", "v1/deployments/provider-payload"
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(UploadDocumentResponse, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(DeploymentProviderPayloadResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise BadRequestError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+        if _response.status_code == 403:
+            raise ForbiddenError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 404:
-            raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise NotFoundError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 500:
-            raise InternalServerError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise InternalServerError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncDocumentsClient:
+class AsyncDeploymentsClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def list(
         self,
         *,
-        document_index_id: typing.Optional[str] = None,
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
         ordering: typing.Optional[str] = None,
-    ) -> PaginatedSlimDocumentList:
+        status: typing.Optional[DeploymentsListRequestStatus] = None,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> PaginatedSlimDeploymentReadList:
         """
-        Used to list documents. Optionally filter on supported fields.
-
         Parameters:
-            - document_index_id: typing.Optional[str]. Filter down to only those documents that are included in the specified index. You may provide either the Vellum-generated ID or the unique name of the index specified upon initial creation.
-
             - limit: typing.Optional[int]. Number of results to return per page.
 
             - offset: typing.Optional[int]. The initial index from which to return the results.
 
             - ordering: typing.Optional[str]. Which field to use when ordering the results.
+
+            - status: typing.Optional[DeploymentsListRequestStatus]. status
+
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from vellum.client import AsyncVellum
 
         client = AsyncVellum(
             api_key="YOUR_API_KEY",
         )
-        await client.documents.list()
+        await client.deployments.list()
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_environment().default}/", "v1/documents"),
-            params=remove_none_from_dict(
-                {"document_index_id": document_index_id, "limit": limit, "offset": offset, "ordering": ordering}
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_environment().default}/", "v1/deployments"),
+            params=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        "limit": limit,
+                        "offset": offset,
+                        "ordering": ordering,
+                        "status": status,
+                        **(
+                            request_options.get("additional_query_parameters", {})
+                            if request_options is not None
+                            else {}
+                        ),
+                    }
+                )
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
             ),
-            headers=self._client_wrapper.get_headers(),
-            timeout=None,
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PaginatedSlimDocumentList, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(PaginatedSlimDeploymentReadList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def destroy(self, id: str) -> None:
+    async def retrieve(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> DeploymentRead:
         """
+        Used to retrieve a deployment given its ID or name.
+
         Parameters:
-            - id: str. A UUID string identifying this document.
+            - id: str. Either the Deployment's ID or its unique name
+
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from vellum.client import AsyncVellum
 
         client = AsyncVellum(
             api_key="YOUR_API_KEY",
         )
-        await client.documents.destroy(
+        await client.deployments.retrieve(
             id="id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_environment().default}/", f"v1/documents/{id}"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=None,
+            method="GET",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_environment().default}/", f"v1/deployments/{jsonable_encoder(id)}"
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
+            return pydantic_v1.parse_obj_as(DeploymentRead, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def partial_update(
+    async def retrieve_provider_payload(
         self,
-        id: str,
         *,
-        label: typing.Optional[str] = OMIT,
-        status: typing.Optional[DocumentStatus] = OMIT,
-        metadata: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
-    ) -> DocumentRead:
+        deployment_id: typing.Optional[str] = OMIT,
+        deployment_name: typing.Optional[str] = OMIT,
+        inputs: typing.Sequence[PromptDeploymentInputRequest],
+        release_tag: typing.Optional[str] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> DeploymentProviderPayloadResponse:
         """
-        Update a Document, keying off of its Vellum-generated ID. Particularly useful for updating its metadata.
-
         Parameters:
-            - id: str. A UUID string identifying this document.
+            - deployment_id: typing.Optional[str]. The ID of the deployment. Must provide either this or deployment_name.
+
+            - deployment_name: typing.Optional[str]. The name of the deployment. Must provide either this or deployment_id.
 
-            - label: typing.Optional[str]. A human-readable label for the document. Defaults to the originally uploaded file's file name.
+            - inputs: typing.Sequence[PromptDeploymentInputRequest]. The list of inputs defined in the Prompt's deployment with their corresponding values.
 
-            - status: typing.Optional[DocumentStatus]. The current status of the document
+            - release_tag: typing.Optional[str]. Optionally specify a release tag if you want to pin to a specific release of the Workflow Deployment
 
-                                                       * `ACTIVE` - Active
-            - metadata: typing.Optional[typing.Dict[str, typing.Any]]. A JSON object containing any metadata associated with the document that you'd like to filter upon later.
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from vellum.client import AsyncVellum
 
         client = AsyncVellum(
             api_key="YOUR_API_KEY",
         )
-        await client.documents.partial_update(
-            id="id",
+        await client.deployments.retrieve_provider_payload(
+            inputs=[],
         )
         """
-        _request: typing.Dict[str, typing.Any] = {}
-        if label is not OMIT:
-            _request["label"] = label
-        if status is not OMIT:
-            _request["status"] = status
-        if metadata is not OMIT:
-            _request["metadata"] = metadata
+        _request: typing.Dict[str, typing.Any] = {"inputs": inputs}
+        if deployment_id is not OMIT:
+            _request["deployment_id"] = deployment_id
+        if deployment_name is not OMIT:
+            _request["deployment_name"] = deployment_name
+        if release_tag is not OMIT:
+            _request["release_tag"] = release_tag
         _response = await self._client_wrapper.httpx_client.request(
-            "PATCH",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_environment().default}/", f"v1/documents/{id}"),
-            json=jsonable_encoder(_request),
-            headers=self._client_wrapper.get_headers(),
-            timeout=None,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DocumentRead, _response.json())  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def upload(
-        self,
-        *,
-        add_to_index_names: typing.Optional[typing.List[str]] = None,
-        external_id: typing.Optional[str] = None,
-        label: str,
-        contents: typing.IO,
-        keywords: typing.Optional[typing.List[str]] = None,
-        metadata: typing.Optional[str] = None,
-    ) -> UploadDocumentResponse:
-        """
-        Upload a document to be indexed and used for search.
-
-        **Note:** Uses a base url of `https://documents.vellum.ai`.
-
-        This is a multipart/form-data request. The `contents` field should be a file upload. It also expects a JSON body with the following fields:
-
-        - `add_to_index_names: list[str]` - Optionally include the names of all indexes that you'd like this document to be included in
-        - `external_id: str | None` - Optionally include an external ID for this document. This is useful if you want to re-upload the same document later when its contents change and would like it to be re-indexed.
-        - `label: str` - A human-friendly name for this document. Typically the filename.
-        - `keywords: list[str] | None` - Optionally include a list of keywords that'll be associated with this document. Used when performing keyword searches.
-        - `metadata: dict[str, Any]` - A stringified JSON object containing any metadata associated with the document that you'd like to filter upon later.
-
-        Parameters:
-            - add_to_index_names: typing.Optional[typing.List[str]].
-
-            - external_id: typing.Optional[str].
-
-            - label: str.
-
-            - contents: typing.IO.
-
-            - keywords: typing.Optional[typing.List[str]].
-
-            - metadata: typing.Optional[str].
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_environment().documents}/", "v1/upload-document"),
-            data=jsonable_encoder(
-                {
-                    "add_to_index_names": add_to_index_names,
-                    "external_id": external_id,
-                    "label": label,
-                    "keywords": keywords,
-                    "metadata": metadata,
-                }
-            ),
-            files={"contents": contents},
-            headers=self._client_wrapper.get_headers(),
-            timeout=None,
+            method="POST",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_environment().default}/", "v1/deployments/provider-payload"
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(UploadDocumentResponse, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(DeploymentProviderPayloadResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise BadRequestError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+        if _response.status_code == 403:
+            raise ForbiddenError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 404:
-            raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise NotFoundError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 500:
-            raise InternalServerError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise InternalServerError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `vellum_ai-0.3.9/src/vellum/resources/test_suites/client.py` & `vellum_ai-0.5.0/src/vellum/lib/test_suites/resources.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,223 +1,253 @@
-# This file was auto-generated by Fern from our API Definition.
+from __future__ import annotations
 
-import typing
-import urllib.parse
-from json.decoder import JSONDecodeError
-
-from ...core.api_error import ApiError
-from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
-from ...core.jsonable_encoder import jsonable_encoder
-from ...types.named_test_case_variable_value_request import NamedTestCaseVariableValueRequest
-from ...types.test_suite_test_case import TestSuiteTestCase
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-# this is used as the default value for optional parameters
-OMIT = typing.cast(typing.Any, ...)
-
-
-class TestSuitesClient:
-    def __init__(self, *, client_wrapper: SyncClientWrapper):
-        self._client_wrapper = client_wrapper
+import logging
+import time
+from typing import Callable, Generator, List
+
+from vellum.client import Vellum
+from vellum.lib.test_suites.constants import (
+    DEFAULT_MAX_POLLING_DURATION_MS,
+    DEFAULT_POLLING_INTERVAL_MS,
+)
+from vellum.lib.test_suites.exceptions import TestSuiteRunResultsException
+from vellum.lib.utils.env import get_api_key
+from vellum.types import (
+    ExternalTestCaseExecutionRequest,
+    NamedTestCaseVariableValueRequest,
+    TestCaseVariableValue,
+    TestSuiteRunExecConfigRequest_External,
+    TestSuiteRunExecution,
+    TestSuiteRunExternalExecConfigDataRequest,
+    TestSuiteRunMetricOutput,
+    TestSuiteRunState,
+)
+
+from vellum.lib.utils.paginator import PaginatedResults, get_all_results
+
+
+logger = logging.getLogger(__name__)
+
+
+class VellumTestSuiteRunExecution(TestSuiteRunExecution):
+    @classmethod
+    def from_api(cls, execution: TestSuiteRunExecution) -> VellumTestSuiteRunExecution:
+        return cls(
+            id=execution.id,
+            test_case_id=execution.test_case_id,
+            outputs=execution.outputs,
+            metric_results=execution.metric_results,
+        )
 
-    def upsert_test_suite_test_case(
+    def get_metric_output(
         self,
-        id: str,
-        *,
-        upsert_test_suite_test_case_request_id: typing.Optional[str] = OMIT,
-        label: typing.Optional[str] = OMIT,
-        input_values: typing.List[NamedTestCaseVariableValueRequest],
-        evaluation_values: typing.List[NamedTestCaseVariableValueRequest],
-    ) -> TestSuiteTestCase:
-        """
-        Upserts a new test case for a test suite, keying off of the optionally provided test case id.
+        metric_identifier: str | None = None,
+        output_identifier: str | None = None,
+    ) -> TestSuiteRunMetricOutput:
+        """Retrieve a metric's output by specifying the info needed to uniquely identify that metric and output.
 
-        If an id is provided and has a match, the test case will be updated. If no id is provided or no match
-        is found, a new test case will be appended to the end.
-
-        Note that a full replacement of the test case is performed, so any fields not provided will be removed
-        or overwritten with default values.
+        metric_identifier: Anything that uniquely identifies the metric to retrieve (e.g. it's label, name or id)
+        output_identifier: Anything that uniquely identifies the output to retrieve (e.g. it's name)
+        """
 
-        Parameters:
-            - id: str. A UUID string identifying this test suite.
+        metric_outputs = self.get_metric_outputs(metric_identifier)
 
-            - upsert_test_suite_test_case_request_id: typing.Optional[str].
+        filtered_metric_outputs = [
+            metric_output
+            for metric_output in metric_outputs
+            if output_identifier is None or metric_output.name == output_identifier
+        ]
 
-            - label: typing.Optional[str].
+        if len(filtered_metric_outputs) == 0:
+            raise TestSuiteRunResultsException(
+                f"No metric outputs found with identifier: {output_identifier}"
+            )
 
-            - input_values: typing.List[NamedTestCaseVariableValueRequest].
+        if len(filtered_metric_outputs) > 1:
+            raise TestSuiteRunResultsException(
+                f"Multiple metric outputs found with identifier: {output_identifier}"
+            )
 
-            - evaluation_values: typing.List[NamedTestCaseVariableValueRequest].
-        ---
-        from vellum.client import Vellum
+        return filtered_metric_outputs[0]
 
-        client = Vellum(
-            api_key="YOUR_API_KEY",
-        )
-        client.test_suites.upsert_test_suite_test_case(
-            id="id",
-            input_values=[],
-            evaluation_values=[],
-        )
-        """
-        _request: typing.Dict[str, typing.Any] = {"input_values": input_values, "evaluation_values": evaluation_values}
-        if upsert_test_suite_test_case_request_id is not OMIT:
-            _request["id"] = upsert_test_suite_test_case_request_id
-        if label is not OMIT:
-            _request["label"] = label
-        _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_environment().default}/", f"v1/test-suites/{id}/test-cases"
-            ),
-            json=jsonable_encoder(_request),
-            headers=self._client_wrapper.get_headers(),
-            timeout=None,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(TestSuiteTestCase, _response.json())  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+    def get_metric_outputs(
+        self,
+        metric_identifier: str | None = None,
+    ) -> List[TestSuiteRunMetricOutput]:
+        """Return a metric's output across all executions by providing the info needed to uniquely identify it.
+
+        metric_identifier: Anything that uniquely identifies the metric to retrieve (e.g. it's label, name or id).
+        """
+
+        filtered_metric_results = [
+            metric_output
+            for metric_output in self.metric_results
+            if metric_identifier is None
+            or (metric_output.metric_id == metric_identifier)
+            or (metric_output.metric_label == metric_identifier)
+            or (
+                metric_output.metric_definition
+                and metric_output.metric_definition.id == metric_identifier
+            )
+            or (
+                metric_output.metric_definition
+                and metric_output.metric_definition.name == metric_identifier
+            )
+            or (
+                metric_output.metric_definition
+                and metric_output.metric_definition.label == metric_identifier
+            )
+        ]
+
+        if len(filtered_metric_results) == 0:
+            raise TestSuiteRunResultsException(
+                f"No metric results found with identifier: {metric_identifier}"
+            )
+
+        if len(filtered_metric_results) > 1:
+            raise TestSuiteRunResultsException(
+                f"Multiple metric results found with identifier: {metric_identifier}"
+            )
 
-    def delete_test_suite_test_case(self, id: str, test_case_id: str) -> None:
-        """
-        Deletes an existing test case for a test suite, keying off of the test case id.
+        return filtered_metric_results[0].outputs
 
-        Parameters:
-            - id: str. A UUID string identifying this test suite.
 
-            - test_case_id: str. An id identifying the test case that you'd like to delete
-        ---
-        from vellum.client import Vellum
+class VellumTestSuiteRunResults:
+    """A utility class with methods for conveniently operating on a Test Suite Run and its results."""
 
-        client = Vellum(
-            api_key="YOUR_API_KEY",
-        )
-        client.test_suites.delete_test_suite_test_case(
-            id="id",
-            test_case_id="test_case_id",
-        )
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_environment().default}/", f"v1/test-suites/{id}/test-cases/{test_case_id}"
-            ),
-            headers=self._client_wrapper.get_headers(),
-            timeout=None,
-        )
-        if 200 <= _response.status_code < 300:
-            return
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-
-class AsyncTestSuitesClient:
-    def __init__(self, *, client_wrapper: AsyncClientWrapper):
-        self._client_wrapper = client_wrapper
-
-    async def upsert_test_suite_test_case(
+    def __init__(
         self,
-        id: str,
+        test_suite_run_id: str,
         *,
-        upsert_test_suite_test_case_request_id: typing.Optional[str] = OMIT,
-        label: typing.Optional[str] = OMIT,
-        input_values: typing.List[NamedTestCaseVariableValueRequest],
-        evaluation_values: typing.List[NamedTestCaseVariableValueRequest],
-    ) -> TestSuiteTestCase:
-        """
-        Upserts a new test case for a test suite, keying off of the optionally provided test case id.
+        client: Vellum | None = None,
+        polling_interval: int = DEFAULT_POLLING_INTERVAL_MS,
+        max_polling_duration: int = DEFAULT_MAX_POLLING_DURATION_MS,
+    ) -> None:
+        self._test_suite_run_id = test_suite_run_id
+        self._client = client or Vellum(
+            api_key=get_api_key(),
+        )
+        self._state = "QUEUED"
+        self._executions: Generator[VellumTestSuiteRunExecution, None, None] | None = (
+            None
+        )
+        self._polling_interval = polling_interval
+        self._max_polling_duration = max_polling_duration
+
+    def get_metric_outputs(
+        self, metric_identifier: str | None = None, output_identifier: str | None = None
+    ) -> Generator[TestSuiteRunMetricOutput, None, None]:
+        """Retrieve a metric's output across all executions by providing the info needed to uniquely identify it."""
+
+        executions = self._get_test_suite_run_executions()
+
+        for execution in executions:
+            yield execution.get_metric_output(
+                metric_identifier=metric_identifier, output_identifier=output_identifier
+            )
+
+    def _refresh_test_suite_run_state(self):
+        test_suite_run = self._client.test_suite_runs.retrieve(self._test_suite_run_id)
+        self._state = test_suite_run.state
+
+    def _list_paginated_executions(
+        self, offset: int | None, limit: int | None
+    ) -> PaginatedResults[TestSuiteRunExecution]:
+        response = self._client.test_suite_runs.list_executions(
+            self._test_suite_run_id,
+            offset=offset,
+            limit=limit,
+            expand=[
+                "results.metric_results.metric_definition",
+                "results.metric_results.metric_label",
+            ],
+        )
+        return PaginatedResults(results=response.results, count=response.count)
+
+    def _wrap_api_executions(
+        self, executions: Generator[TestSuiteRunExecution, None, None]
+    ) -> Generator[VellumTestSuiteRunExecution, None, None]:
+        for execution in executions:
+            yield VellumTestSuiteRunExecution.from_api(execution)
 
-        If an id is provided and has a match, the test case will be updated. If no id is provided or no match
-        is found, a new test case will be appended to the end.
+    def _get_test_suite_run_executions(
+        self,
+    ) -> Generator[VellumTestSuiteRunExecution, None, None]:
+        if self._executions is not None:
+            return self._executions
 
-        Note that a full replacement of the test case is performed, so any fields not provided will be removed
-        or overwritten with default values.
+        start_time = time.time_ns()
+        while True:
+            logger.debug("Polling for latest test suite run state...")
+            self._refresh_test_suite_run_state()
+            if self._state not in {"QUEUED", "RUNNING"}:
+                break
 
-        Parameters:
-            - id: str. A UUID string identifying this test suite.
+            current_time = time.time_ns()
+            if ((current_time - start_time) / 1e6) > self._max_polling_duration:
+                raise TestSuiteRunResultsException(
+                    "Test suite run timed out polling for executions"
+                )
 
-            - upsert_test_suite_test_case_request_id: typing.Optional[str].
+            time.sleep(self._polling_interval / 1000.0)
 
-            - label: typing.Optional[str].
+        if self._state == "FAILED":
+            raise TestSuiteRunResultsException("Test suite run failed")
 
-            - input_values: typing.List[NamedTestCaseVariableValueRequest].
+        if self._state == "CANCELLED":
+            raise TestSuiteRunResultsException("Test suite run was cancelled")
 
-            - evaluation_values: typing.List[NamedTestCaseVariableValueRequest].
-        ---
-        from vellum.client import AsyncVellum
+        raw_api_executions = get_all_results(self._list_paginated_executions)
+        self._executions = self._wrap_api_executions(raw_api_executions)
+        return self._executions
 
-        client = AsyncVellum(
-            api_key="YOUR_API_KEY",
-        )
-        await client.test_suites.upsert_test_suite_test_case(
-            id="id",
-            input_values=[],
-            evaluation_values=[],
-        )
-        """
-        _request: typing.Dict[str, typing.Any] = {"input_values": input_values, "evaluation_values": evaluation_values}
-        if upsert_test_suite_test_case_request_id is not OMIT:
-            _request["id"] = upsert_test_suite_test_case_request_id
-        if label is not OMIT:
-            _request["label"] = label
-        _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_environment().default}/", f"v1/test-suites/{id}/test-cases"
-            ),
-            json=jsonable_encoder(_request),
-            headers=self._client_wrapper.get_headers(),
-            timeout=None,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(TestSuiteTestCase, _response.json())  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def delete_test_suite_test_case(self, id: str, test_case_id: str) -> None:
-        """
-        Deletes an existing test case for a test suite, keying off of the test case id.
-
-        Parameters:
-            - id: str. A UUID string identifying this test suite.
-
-            - test_case_id: str. An id identifying the test case that you'd like to delete
-        ---
-        from vellum.client import AsyncVellum
+class VellumTestSuite:
+    """A utility class that provides methods for running a Vellum Test Suite and interacting with its results."""
 
-        client = AsyncVellum(
-            api_key="YOUR_API_KEY",
-        )
-        await client.test_suites.delete_test_suite_test_case(
-            id="id",
-            test_case_id="test_case_id",
+    def __init__(
+        self,
+        test_suite_id: str,
+        *,
+        client: Vellum | None = None,
+    ) -> None:
+        self.client = client or Vellum(
+            api_key=get_api_key(),
         )
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_environment().default}/", f"v1/test-suites/{id}/test-cases/{test_case_id}"
+        self._test_suite_id = test_suite_id
+
+    def run_external(
+        self,
+        executable: Callable[
+            [List[TestCaseVariableValue]], List[NamedTestCaseVariableValueRequest]
+        ],
+    ) -> VellumTestSuiteRunResults:
+        """
+        Runs this Vellum Test Suite on any executable function defined external to Vellum.
+
+        Returns a wrapper that polls the generated Test Suite Run until it's done running and returns its results.
+        """
+        test_cases = self.client.test_suites.list_test_suite_test_cases(
+            id=self._test_suite_id
+        )
+        executions: List[ExternalTestCaseExecutionRequest] = []
+
+        for test_case in test_cases.results:
+            outputs = executable(test_case.input_values)
+
+            executions.append(
+                ExternalTestCaseExecutionRequest(
+                    test_case_id=test_case.id,  # type: ignore[arg-type]
+                    outputs=outputs,
+                )
+            )
+
+        test_suite_run = self.client.test_suite_runs.create(
+            test_suite_id=self._test_suite_id,
+            exec_config=TestSuiteRunExecConfigRequest_External(
+                type="EXTERNAL",
+                data=TestSuiteRunExternalExecConfigDataRequest(
+                    executions=executions,
+                ),
             ),
-            headers=self._client_wrapper.get_headers(),
-            timeout=None,
         )
-        if 200 <= _response.status_code < 300:
-            return
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+        return VellumTestSuiteRunResults(test_suite_run.id, client=self.client)
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/api_node_result.py` & `vellum_ai-0.5.0/src/vellum/types/api_node_result.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .api_node_result_data import ApiNodeResultData
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ApiNodeResult(pydantic.BaseModel):
+class ApiNodeResult(pydantic_v1.BaseModel):
     """
     A Node Result Event emitted from an API Node.
     """
 
     data: ApiNodeResultData
 
     def json(self, **kwargs: typing.Any) -> str:
@@ -26,8 +22,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/api_node_result_data.py` & `vellum_ai-0.5.0/src/vellum/types/api_node_result_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ApiNodeResultData(pydantic.BaseModel):
+class ApiNodeResultData(pydantic_v1.BaseModel):
     text_output_id: str
-    text: typing.Optional[str]
+    text: typing.Optional[str] = None
     json_output_id: str
-    json_: typing.Optional[typing.Dict[str, typing.Any]] = pydantic.Field(alias="json")
+    json_: typing.Optional[typing.Dict[str, typing.Any]] = pydantic_v1.Field(alias="json", default=None)
     status_code_output_id: str
     status_code: int
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
@@ -27,8 +23,10 @@
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/array_chat_message_content.py` & `vellum_ai-0.5.0/src/vellum/types/array_chat_message_content.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .array_chat_message_content_item import ArrayChatMessageContentItem
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ArrayChatMessageContent(pydantic.BaseModel):
+class ArrayChatMessageContent(pydantic_v1.BaseModel):
     """
     A list of chat message content items.
     """
 
     value: typing.List[ArrayChatMessageContentItem]
 
     def json(self, **kwargs: typing.Any) -> str:
@@ -26,8 +22,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/array_chat_message_content_item.py` & `vellum_ai-0.5.0/src/vellum/types/array_chat_message_content_item.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from __future__ import annotations
 
 import typing
 
-import typing_extensions
-
 from .function_call_chat_message_content import FunctionCallChatMessageContent
 from .image_chat_message_content import ImageChatMessageContent
 from .string_chat_message_content import StringChatMessageContent
 
 
 class ArrayChatMessageContentItem_String(StringChatMessageContent):
-    type: typing_extensions.Literal["STRING"]
+    type: typing.Literal["STRING"] = "STRING"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class ArrayChatMessageContentItem_FunctionCall(FunctionCallChatMessageContent):
-    type: typing_extensions.Literal["FUNCTION_CALL"]
+    type: typing.Literal["FUNCTION_CALL"] = "FUNCTION_CALL"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class ArrayChatMessageContentItem_Image(ImageChatMessageContent):
-    type: typing_extensions.Literal["IMAGE"]
+    type: typing.Literal["IMAGE"] = "IMAGE"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 ArrayChatMessageContentItem = typing.Union[
     ArrayChatMessageContentItem_String, ArrayChatMessageContentItem_FunctionCall, ArrayChatMessageContentItem_Image
 ]
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/array_chat_message_content_item_request.py` & `vellum_ai-0.5.0/src/vellum/types/array_chat_message_content_item_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from __future__ import annotations
 
 import typing
 
-import typing_extensions
-
 from .function_call_chat_message_content_request import FunctionCallChatMessageContentRequest
 from .image_chat_message_content_request import ImageChatMessageContentRequest
 from .string_chat_message_content_request import StringChatMessageContentRequest
 
 
 class ArrayChatMessageContentItemRequest_String(StringChatMessageContentRequest):
-    type: typing_extensions.Literal["STRING"]
+    type: typing.Literal["STRING"] = "STRING"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class ArrayChatMessageContentItemRequest_FunctionCall(FunctionCallChatMessageContentRequest):
-    type: typing_extensions.Literal["FUNCTION_CALL"]
+    type: typing.Literal["FUNCTION_CALL"] = "FUNCTION_CALL"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class ArrayChatMessageContentItemRequest_Image(ImageChatMessageContentRequest):
-    type: typing_extensions.Literal["IMAGE"]
+    type: typing.Literal["IMAGE"] = "IMAGE"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 ArrayChatMessageContentItemRequest = typing.Union[
     ArrayChatMessageContentItemRequest_String,
     ArrayChatMessageContentItemRequest_FunctionCall,
     ArrayChatMessageContentItemRequest_Image,
 ]
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/array_chat_message_content_request.py` & `vellum_ai-0.5.0/src/vellum/types/array_chat_message_content_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .array_chat_message_content_item_request import ArrayChatMessageContentItemRequest
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ArrayChatMessageContentRequest(pydantic.BaseModel):
+class ArrayChatMessageContentRequest(pydantic_v1.BaseModel):
     """
     A list of chat message content items.
     """
 
     value: typing.List[ArrayChatMessageContentItemRequest]
 
     def json(self, **kwargs: typing.Any) -> str:
@@ -26,8 +22,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/array_variable_value_item.py` & `vellum_ai-0.5.0/src/vellum/types/array_variable_value_item.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,89 +1,106 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from __future__ import annotations
 
 import typing
 
-import typing_extensions
-
 from .chat_history_variable_value import ChatHistoryVariableValue
 from .error_variable_value import ErrorVariableValue
 from .function_call_variable_value import FunctionCallVariableValue
+from .image_variable_value import ImageVariableValue
 from .json_variable_value import JsonVariableValue
 from .number_variable_value import NumberVariableValue
 from .search_results_variable_value import SearchResultsVariableValue
 from .string_variable_value import StringVariableValue
 
 
 class ArrayVariableValueItem_String(StringVariableValue):
-    type: typing_extensions.Literal["STRING"]
+    type: typing.Literal["STRING"] = "STRING"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class ArrayVariableValueItem_Number(NumberVariableValue):
-    type: typing_extensions.Literal["NUMBER"]
+    type: typing.Literal["NUMBER"] = "NUMBER"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class ArrayVariableValueItem_Json(JsonVariableValue):
-    type: typing_extensions.Literal["JSON"]
+    type: typing.Literal["JSON"] = "JSON"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class ArrayVariableValueItem_ChatHistory(ChatHistoryVariableValue):
-    type: typing_extensions.Literal["CHAT_HISTORY"]
+    type: typing.Literal["CHAT_HISTORY"] = "CHAT_HISTORY"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class ArrayVariableValueItem_SearchResults(SearchResultsVariableValue):
-    type: typing_extensions.Literal["SEARCH_RESULTS"]
+    type: typing.Literal["SEARCH_RESULTS"] = "SEARCH_RESULTS"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class ArrayVariableValueItem_Error(ErrorVariableValue):
-    type: typing_extensions.Literal["ERROR"]
+    type: typing.Literal["ERROR"] = "ERROR"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class ArrayVariableValueItem_FunctionCall(FunctionCallVariableValue):
-    type: typing_extensions.Literal["FUNCTION_CALL"]
+    type: typing.Literal["FUNCTION_CALL"] = "FUNCTION_CALL"
+
+    class Config:
+        frozen = True
+        smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+
+
+class ArrayVariableValueItem_Image(ImageVariableValue):
+    type: typing.Literal["IMAGE"] = "IMAGE"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 ArrayVariableValueItem = typing.Union[
     ArrayVariableValueItem_String,
     ArrayVariableValueItem_Number,
     ArrayVariableValueItem_Json,
     ArrayVariableValueItem_ChatHistory,
     ArrayVariableValueItem_SearchResults,
     ArrayVariableValueItem_Error,
     ArrayVariableValueItem_FunctionCall,
+    ArrayVariableValueItem_Image,
 ]
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/chat_history_input_request.py` & `vellum_ai-0.5.0/src/vellum/types/workflow_request_chat_history_input_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .chat_message_request import ChatMessageRequest
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class WorkflowRequestChatHistoryInputRequest(pydantic_v1.BaseModel):
+    """
+    The input for a chat history variable in a Workflow.
+    """
 
-class ChatHistoryInputRequest(pydantic.BaseModel):
+    name: str = pydantic_v1.Field()
     """
-    A user input representing a list of chat messages
+    The variable's name, as defined in the Workflow.
     """
 
-    name: str = pydantic.Field(description="The variable's name, as defined in the deployment.")
     value: typing.List[ChatMessageRequest]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/chat_history_variable_value.py` & `vellum_ai-0.5.0/src/vellum/types/execution_chat_history_vellum_value.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .chat_message import ChatMessage
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class ExecutionChatHistoryVellumValue(pydantic_v1.BaseModel):
+    id: str = pydantic_v1.Field()
+    """
+    The variable's uniquely identifying internal id.
+    """
 
-class ChatHistoryVariableValue(pydantic.BaseModel):
-    value: typing.Optional[typing.List[ChatMessage]]
+    name: str
+    value: typing.Optional[typing.List[ChatMessage]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/chat_message.py` & `vellum_ai-0.5.0/src/vellum/types/chat_message_request.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .chat_message_content import ChatMessageContent
+from ..core.pydantic_utilities import pydantic_v1
+from .chat_message_content_request import ChatMessageContentRequest
 from .chat_message_role import ChatMessageRole
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ChatMessage(pydantic.BaseModel):
-    text: typing.Optional[str]
+class ChatMessageRequest(pydantic_v1.BaseModel):
+    text: typing.Optional[str] = None
     role: ChatMessageRole
-    content: typing.Optional[ChatMessageContent]
+    content: typing.Optional[ChatMessageContentRequest] = None
+    source: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    An optional identifier representing who or what generated this message.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/chat_message_content.py` & `vellum_ai-0.5.0/src/vellum/types/chat_message_content.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from __future__ import annotations
 
 import typing
 
-import typing_extensions
-
 from .array_chat_message_content import ArrayChatMessageContent
 from .function_call_chat_message_content import FunctionCallChatMessageContent
 from .image_chat_message_content import ImageChatMessageContent
 from .string_chat_message_content import StringChatMessageContent
 
 
 class ChatMessageContent_String(StringChatMessageContent):
-    type: typing_extensions.Literal["STRING"]
+    type: typing.Literal["STRING"] = "STRING"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class ChatMessageContent_FunctionCall(FunctionCallChatMessageContent):
-    type: typing_extensions.Literal["FUNCTION_CALL"]
+    type: typing.Literal["FUNCTION_CALL"] = "FUNCTION_CALL"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class ChatMessageContent_Array(ArrayChatMessageContent):
-    type: typing_extensions.Literal["ARRAY"]
+    type: typing.Literal["ARRAY"] = "ARRAY"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class ChatMessageContent_Image(ImageChatMessageContent):
-    type: typing_extensions.Literal["IMAGE"]
+    type: typing.Literal["IMAGE"] = "IMAGE"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 ChatMessageContent = typing.Union[
     ChatMessageContent_String, ChatMessageContent_FunctionCall, ChatMessageContent_Array, ChatMessageContent_Image
 ]
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/chat_message_content_request.py` & `vellum_ai-0.5.0/src/vellum/types/chat_message_content_request.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,57 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from __future__ import annotations
 
 import typing
 
-import typing_extensions
-
 from .array_chat_message_content_request import ArrayChatMessageContentRequest
 from .function_call_chat_message_content_request import FunctionCallChatMessageContentRequest
 from .image_chat_message_content_request import ImageChatMessageContentRequest
 from .string_chat_message_content_request import StringChatMessageContentRequest
 
 
 class ChatMessageContentRequest_String(StringChatMessageContentRequest):
-    type: typing_extensions.Literal["STRING"]
+    type: typing.Literal["STRING"] = "STRING"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class ChatMessageContentRequest_FunctionCall(FunctionCallChatMessageContentRequest):
-    type: typing_extensions.Literal["FUNCTION_CALL"]
+    type: typing.Literal["FUNCTION_CALL"] = "FUNCTION_CALL"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class ChatMessageContentRequest_Array(ArrayChatMessageContentRequest):
-    type: typing_extensions.Literal["ARRAY"]
+    type: typing.Literal["ARRAY"] = "ARRAY"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class ChatMessageContentRequest_Image(ImageChatMessageContentRequest):
-    type: typing_extensions.Literal["IMAGE"]
+    type: typing.Literal["IMAGE"] = "IMAGE"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 ChatMessageContentRequest = typing.Union[
     ChatMessageContentRequest_String,
     ChatMessageContentRequest_FunctionCall,
     ChatMessageContentRequest_Array,
     ChatMessageContentRequest_Image,
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/chat_message_request.py` & `vellum_ai-0.5.0/src/vellum/types/workflow_result_event_output_data_chat_history.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .chat_message_content_request import ChatMessageContentRequest
-from .chat_message_role import ChatMessageRole
+from ..core.pydantic_utilities import pydantic_v1
+from .chat_message import ChatMessage
+from .workflow_node_result_event_state import WorkflowNodeResultEventState
+
+
+class WorkflowResultEventOutputDataChatHistory(pydantic_v1.BaseModel):
+    """
+    A Chat History output streamed from a Workflow execution.
+    """
+
+    id: typing.Optional[str] = None
+    name: str
+    state: WorkflowNodeResultEventState
+    node_id: str
+    delta: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The newly output string value. Only relevant for string outputs with a state of STREAMING.
+    """
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class ChatMessageRequest(pydantic.BaseModel):
-    text: typing.Optional[str]
-    role: ChatMessageRole
-    content: typing.Optional[ChatMessageContentRequest]
+    value: typing.Optional[typing.List[ChatMessage]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/code_execution_node_chat_history_result.py` & `vellum_ai-0.5.0/src/vellum/types/generate_result_error.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .chat_message import ChatMessage
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class CodeExecutionNodeChatHistoryResult(pydantic.BaseModel):
-    id: str
-    value: typing.Optional[typing.List[ChatMessage]]
+class GenerateResultError(pydantic_v1.BaseModel):
+    message: str = pydantic_v1.Field()
+    """
+    The error message returned by the LLM provider.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/code_execution_node_error_result.py` & `vellum_ai-0.5.0/src/vellum/types/execute_workflow_error_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .vellum_error import VellumError
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class CodeExecutionNodeErrorResult(pydantic.BaseModel):
-    id: str
-    value: typing.Optional[VellumError]
+class ExecuteWorkflowErrorResponse(pydantic_v1.BaseModel):
+    detail: str = pydantic_v1.Field()
+    """
+    Details about why the request failed.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/code_execution_node_json_result.py` & `vellum_ai-0.5.0/src/vellum/types/code_execution_node_number_result.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class CodeExecutionNodeJsonResult(pydantic.BaseModel):
+class CodeExecutionNodeNumberResult(pydantic_v1.BaseModel):
     id: str
-    value: typing.Optional[typing.Dict[str, typing.Any]]
+    value: typing.Optional[float] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/code_execution_node_number_result.py` & `vellum_ai-0.5.0/src/vellum/types/execute_workflow_stream_error_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class CodeExecutionNodeNumberResult(pydantic.BaseModel):
-    id: str
-    value: typing.Optional[float]
+class ExecuteWorkflowStreamErrorResponse(pydantic_v1.BaseModel):
+    detail: str = pydantic_v1.Field()
+    """
+    Details about why the request failed.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/code_execution_node_result.py` & `vellum_ai-0.5.0/src/vellum/types/execution_array_vellum_value.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .code_execution_node_result_data import CodeExecutionNodeResultData
+from ..core.pydantic_utilities import pydantic_v1
+from .array_variable_value_item import ArrayVariableValueItem
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class CodeExecutionNodeResult(pydantic.BaseModel):
+class ExecutionArrayVellumValue(pydantic_v1.BaseModel):
+    id: str = pydantic_v1.Field()
     """
-    A Node Result Event emitted from a Code Execution Node.
+    The variable's uniquely identifying internal id.
     """
 
-    data: CodeExecutionNodeResultData
+    name: str
+    value: typing.Optional[typing.List[ArrayVariableValueItem]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/code_execution_node_result_data.py` & `vellum_ai-0.5.0/src/vellum/types/code_execution_node_result_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .code_execution_node_result_output import CodeExecutionNodeResultOutput
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class CodeExecutionNodeResultData(pydantic.BaseModel):
+class CodeExecutionNodeResultData(pydantic_v1.BaseModel):
     output: CodeExecutionNodeResultOutput
-    log_output_id: typing.Optional[str]
+    log_output_id: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/code_execution_node_search_results_result.py` & `vellum_ai-0.5.0/src/vellum/types/node_input_compiled_search_results_value.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .search_result import SearchResult
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class CodeExecutionNodeSearchResultsResult(pydantic.BaseModel):
-    id: str
-    value: typing.Optional[typing.List[SearchResult]]
+class NodeInputCompiledSearchResultsValue(pydantic_v1.BaseModel):
+    node_input_id: str
+    key: str
+    value: typing.Optional[typing.List[SearchResult]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/code_execution_node_string_result.py` & `vellum_ai-0.5.0/src/vellum/types/conditional_node_result_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class CodeExecutionNodeStringResult(pydantic.BaseModel):
-    id: str
-    value: typing.Optional[str]
+class ConditionalNodeResultData(pydantic_v1.BaseModel):
+    source_handle_id: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/conditional_node_result.py` & `vellum_ai-0.5.0/src/vellum/types/initiated_workflow_node_result_event.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .conditional_node_result_data import ConditionalNodeResultData
+from ..core.pydantic_utilities import pydantic_v1
+from .node_input_variable_compiled_value import NodeInputVariableCompiledValue
+from .workflow_node_result_data import WorkflowNodeResultData
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ConditionalNodeResult(pydantic.BaseModel):
+class InitiatedWorkflowNodeResultEvent(pydantic_v1.BaseModel):
     """
-    A Node Result Event emitted from a Conditional Node.
+    An event that indicates that the node has initiated its execution.
     """
 
-    data: ConditionalNodeResultData
+    id: str
+    node_id: str
+    node_result_id: str
+    ts: typing.Optional[dt.datetime] = None
+    data: typing.Optional[WorkflowNodeResultData] = None
+    source_execution_id: typing.Optional[str] = None
+    input_values: typing.Optional[typing.List[NodeInputVariableCompiledValue]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/conditional_node_result_data.py` & `vellum_ai-0.5.0/src/vellum/types/named_test_case_string_variable_value_request.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class NamedTestCaseStringVariableValueRequest(pydantic_v1.BaseModel):
+    """
+    Named Test Case value that is of type STRING
+    """
 
-class ConditionalNodeResultData(pydantic.BaseModel):
-    source_handle_id: typing.Optional[str]
+    value: typing.Optional[str] = None
+    name: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/deployment_provider_payload_response.py` & `vellum_ai-0.5.0/src/vellum/types/execute_prompt_api_error_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class DeploymentProviderPayloadResponse(pydantic.BaseModel):
-    payload: typing.Dict[str, typing.Any]
+class ExecutePromptApiErrorResponse(pydantic_v1.BaseModel):
+    detail: str = pydantic_v1.Field()
+    """
+    Details about why the request failed.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/deployment_read.py` & `vellum_ai-0.5.0/src/vellum/types/slim_deployment_read.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,58 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .entity_status import EntityStatus
 from .environment_enum import EnvironmentEnum
 from .vellum_variable import VellumVariable
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class DeploymentRead(pydantic.BaseModel):
+class SlimDeploymentRead(pydantic_v1.BaseModel):
     id: str
     created: dt.datetime
-    label: str = pydantic.Field(description="A human-readable label for the deployment")
-    name: str = pydantic.Field(description="A name that uniquely identifies this deployment within its workspace")
-    status: typing.Optional[EntityStatus] = pydantic.Field(
-        description=("The current status of the deployment\n" "\n" "- `ACTIVE` - Active\n" "- `ARCHIVED` - Archived\n")
-    )
-    environment: typing.Optional[EnvironmentEnum] = pydantic.Field(
-        description=(
-            "The environment this deployment is used in\n"
-            "\n"
-            "- `DEVELOPMENT` - Development\n"
-            "- `STAGING` - Staging\n"
-            "- `PRODUCTION` - Production\n"
-        )
-    )
+    label: str = pydantic_v1.Field()
+    """
+    A human-readable label for the deployment
+    """
+
+    name: str = pydantic_v1.Field()
+    """
+    A name that uniquely identifies this deployment within its workspace
+    """
+
+    status: typing.Optional[EntityStatus] = pydantic_v1.Field(default=None)
+    """
+    The current status of the deployment
+    
+    - `ACTIVE` - Active
+    - `ARCHIVED` - Archived
+    """
+
+    environment: typing.Optional[EnvironmentEnum] = pydantic_v1.Field(default=None)
+    """
+    The environment this deployment is used in
+    
+    - `DEVELOPMENT` - Development
+    - `STAGING` - Staging
+    - `PRODUCTION` - Production
+    """
+
     last_deployed_on: dt.datetime
     input_variables: typing.List[VellumVariable]
-    active_model_version_ids: typing.List[str] = pydantic.Field(
-        description="Deprecated. The Prompt execution endpoints return a `prompt_version_id` that could be used instead."
-    )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/document_document_to_document_index.py` & `vellum_ai-0.5.0/src/vellum/types/workflow_result_event_output_data_error.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .indexing_state_enum import IndexingStateEnum
+from ..core.pydantic_utilities import pydantic_v1
+from .vellum_error import VellumError
+from .workflow_node_result_event_state import WorkflowNodeResultEventState
+
+
+class WorkflowResultEventOutputDataError(pydantic_v1.BaseModel):
+    """
+    An Error output streamed from a Workflow execution.
+    """
+
+    id: typing.Optional[str] = None
+    name: str
+    state: WorkflowNodeResultEventState
+    node_id: str
+    delta: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The newly output string value. Only relevant for string outputs with a state of STREAMING.
+    """
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class DocumentDocumentToDocumentIndex(pydantic.BaseModel):
-    id: str = pydantic.Field(description="Vellum-generated ID that uniquely identifies this link.")
-    document_index_id: str = pydantic.Field(
-        description="Vellum-generated ID that uniquely identifies the index this document is included in."
-    )
-    indexing_state: typing.Optional[IndexingStateEnum] = pydantic.Field(
-        description=(
-            "An enum value representing where this document is along its indexing lifecycle for this index.\n"
-            "\n"
-            "- `AWAITING_PROCESSING` - Awaiting Processing\n"
-            "- `QUEUED` - Queued\n"
-            "- `INDEXING` - Indexing\n"
-            "- `INDEXED` - Indexed\n"
-            "- `FAILED` - Failed\n"
-        )
-    )
+    value: typing.Optional[VellumError] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/document_index_read.py` & `vellum_ai-0.5.0/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_data.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,50 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .entity_status import EntityStatus
-from .environment_enum import EnvironmentEnum
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class DocumentIndexRead(pydantic.BaseModel):
-    id: str
-    created: dt.datetime
-    label: str = pydantic.Field(description="A human-readable label for the document index")
-    name: str = pydantic.Field(description="A name that uniquely identifies this index within its workspace")
-    status: typing.Optional[EntityStatus] = pydantic.Field(
-        description=(
-            "The current status of the document index\n" "\n" "- `ACTIVE` - Active\n" "- `ARCHIVED` - Archived\n"
-        )
-    )
-    environment: typing.Optional[EnvironmentEnum] = pydantic.Field(
-        description=(
-            "The environment this document index is used in\n"
-            "\n"
-            "- `DEVELOPMENT` - Development\n"
-            "- `STAGING` - Staging\n"
-            "- `PRODUCTION` - Production\n"
-        )
-    )
-    indexing_config: typing.Dict[str, typing.Any] = pydantic.Field(
-        description="Configuration representing how documents should be indexed"
-    )
+
+class TestSuiteRunWorkflowReleaseTagExecConfigData(pydantic_v1.BaseModel):
+    workflow_deployment_id: str = pydantic_v1.Field()
+    """
+    The ID of the Workflow Deployment to run the Test Suite against.
+    """
+
+    tag: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    A tag identifying which release of the Workflow Deployment to run the Test Suite against. Useful for testing past versions of the Workflow Deployment
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/document_read.py` & `vellum_ai-0.5.0/src/vellum/types/document_read.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,57 +1,63 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .document_document_to_document_index import DocumentDocumentToDocumentIndex
 from .document_status import DocumentStatus
 from .processing_state_enum import ProcessingStateEnum
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class DocumentRead(pydantic.BaseModel):
+class DocumentRead(pydantic_v1.BaseModel):
     id: str
-    external_id: typing.Optional[str] = pydantic.Field(
-        description="The unique id of this document as it exists in the user's system."
-    )
+    external_id: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The unique id of this document as it exists in the user's system.
+    """
+
     last_uploaded_at: dt.datetime
-    label: str = pydantic.Field(
-        description="A human-readable label for the document. Defaults to the originally uploaded file's file name."
-    )
-    processing_state: typing.Optional[ProcessingStateEnum] = pydantic.Field(
-        description=(
-            "The current processing state of the document\n"
-            "\n"
-            "- `QUEUED` - Queued\n"
-            "- `PROCESSING` - Processing\n"
-            "- `PROCESSED` - Processed\n"
-            "- `FAILED` - Failed\n"
-        )
-    )
-    status: typing.Optional[DocumentStatus] = pydantic.Field(
-        description=("The current status of the document\n" "\n" "- `ACTIVE` - Active\n")
-    )
-    original_file_url: typing.Optional[str]
-    processed_file_url: typing.Optional[str]
+    label: str = pydantic_v1.Field()
+    """
+    A human-readable label for the document. Defaults to the originally uploaded file's file name.
+    """
+
+    processing_state: typing.Optional[ProcessingStateEnum] = pydantic_v1.Field(default=None)
+    """
+    The current processing state of the document
+    
+    - `QUEUED` - Queued
+    - `PROCESSING` - Processing
+    - `PROCESSED` - Processed
+    - `FAILED` - Failed
+    """
+
+    status: typing.Optional[DocumentStatus] = pydantic_v1.Field(default=None)
+    """
+    The current status of the document
+    
+    - `ACTIVE` - Active
+    """
+
+    original_file_url: typing.Optional[str] = None
+    processed_file_url: typing.Optional[str] = None
     document_to_document_indexes: typing.List[DocumentDocumentToDocumentIndex]
-    metadata: typing.Optional[typing.Dict[str, typing.Any]] = pydantic.Field(
-        description="A previously supplied JSON object containing metadata that can be filtered on when searching."
-    )
+    metadata: typing.Optional[typing.Dict[str, typing.Any]] = pydantic_v1.Field(default=None)
+    """
+    A previously supplied JSON object containing metadata that can be filtered on when searching.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/enriched_normalized_completion.py` & `vellum_ai-0.5.0/src/vellum/types/document_index_read.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,59 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .finish_reason_enum import FinishReasonEnum
-from .normalized_log_probs import NormalizedLogProbs
-from .vellum_variable_type import VellumVariableType
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class EnrichedNormalizedCompletion(pydantic.BaseModel):
-    id: str = pydantic.Field(description="The Vellum-generated ID of the completion.")
-    external_id: typing.Optional[str] = pydantic.Field(
-        description="The external ID that was originally provided along with the generation request, which uniquely identifies this generation in an external system."
-    )
-    text: str = pydantic.Field(description="The text generated by the LLM.")
-    finish_reason: typing.Optional[FinishReasonEnum] = pydantic.Field(
-        description=(
-            "The reason the generation finished.\n"
-            "\n"
-            "- `LENGTH` - LENGTH\n"
-            "- `STOP` - STOP\n"
-            "- `UNKNOWN` - UNKNOWN\n"
-        )
-    )
-    logprobs: typing.Optional[NormalizedLogProbs] = pydantic.Field(
-        description="The logprobs of the completion. Only present if specified in the original request options."
-    )
-    model_version_id: str = pydantic.Field(description="The ID of the model version used to generate this completion.")
-    prompt_version_id: str
-    type: typing.Optional[VellumVariableType]
-    deployment_release_tag: str
-    model_name: str
+from ..core.pydantic_utilities import pydantic_v1
+from .entity_status import EntityStatus
+from .environment_enum import EnvironmentEnum
+
+
+class DocumentIndexRead(pydantic_v1.BaseModel):
+    id: str
+    created: dt.datetime
+    label: str = pydantic_v1.Field()
+    """
+    A human-readable label for the document index
+    """
+
+    name: str = pydantic_v1.Field()
+    """
+    A name that uniquely identifies this index within its workspace
+    """
+
+    status: typing.Optional[EntityStatus] = pydantic_v1.Field(default=None)
+    """
+    The current status of the document index
+    
+    - `ACTIVE` - Active
+    - `ARCHIVED` - Archived
+    """
+
+    environment: typing.Optional[EnvironmentEnum] = pydantic_v1.Field(default=None)
+    """
+    The environment this document index is used in
+    
+    - `DEVELOPMENT` - Development
+    - `STAGING` - Staging
+    - `PRODUCTION` - Production
+    """
+
+    indexing_config: typing.Dict[str, typing.Any] = pydantic_v1.Field()
+    """
+    Configuration representing how documents should be indexed
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/error_variable_value.py` & `vellum_ai-0.5.0/src/vellum/types/number_variable_value.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .vellum_error import VellumError
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ErrorVariableValue(pydantic.BaseModel):
-    value: typing.Optional[VellumError]
+class NumberVariableValue(pydantic_v1.BaseModel):
+    value: typing.Optional[float] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/execute_prompt_api_error_response.py` & `vellum_ai-0.5.0/src/vellum/types/paginated_test_suite_test_case_list.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from .test_suite_test_case import TestSuiteTestCase
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ExecutePromptApiErrorResponse(pydantic.BaseModel):
-    detail: str = pydantic.Field(description="Details about why the request failed.")
+class PaginatedTestSuiteTestCaseList(pydantic_v1.BaseModel):
+    count: int
+    next: typing.Optional[str] = None
+    previous: typing.Optional[str] = None
+    results: typing.List[TestSuiteTestCase]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/execute_prompt_event.py` & `vellum_ai-0.5.0/src/vellum/types/execute_prompt_event.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,57 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from __future__ import annotations
 
 import typing
 
-import typing_extensions
-
 from .fulfilled_execute_prompt_event import FulfilledExecutePromptEvent
 from .initiated_execute_prompt_event import InitiatedExecutePromptEvent
 from .rejected_execute_prompt_event import RejectedExecutePromptEvent
 from .streaming_execute_prompt_event import StreamingExecutePromptEvent
 
 
 class ExecutePromptEvent_Initiated(InitiatedExecutePromptEvent):
-    state: typing_extensions.Literal["INITIATED"]
+    state: typing.Literal["INITIATED"] = "INITIATED"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class ExecutePromptEvent_Streaming(StreamingExecutePromptEvent):
-    state: typing_extensions.Literal["STREAMING"]
+    state: typing.Literal["STREAMING"] = "STREAMING"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class ExecutePromptEvent_Fulfilled(FulfilledExecutePromptEvent):
-    state: typing_extensions.Literal["FULFILLED"]
+    state: typing.Literal["FULFILLED"] = "FULFILLED"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class ExecutePromptEvent_Rejected(RejectedExecutePromptEvent):
-    state: typing_extensions.Literal["REJECTED"]
+    state: typing.Literal["REJECTED"] = "REJECTED"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 ExecutePromptEvent = typing.Union[
     ExecutePromptEvent_Initiated,
     ExecutePromptEvent_Streaming,
     ExecutePromptEvent_Fulfilled,
     ExecutePromptEvent_Rejected,
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/execute_prompt_response.py` & `vellum_ai-0.5.0/src/vellum/types/execute_prompt_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from __future__ import annotations
 
 import typing
 
-import typing_extensions
-
 from .fulfilled_execute_prompt_response import FulfilledExecutePromptResponse
 from .rejected_execute_prompt_response import RejectedExecutePromptResponse
 
 
 class ExecutePromptResponse_Fulfilled(FulfilledExecutePromptResponse):
-    state: typing_extensions.Literal["FULFILLED"]
+    state: typing.Literal["FULFILLED"] = "FULFILLED"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class ExecutePromptResponse_Rejected(RejectedExecutePromptResponse):
-    state: typing_extensions.Literal["REJECTED"]
+    state: typing.Literal["REJECTED"] = "REJECTED"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 ExecutePromptResponse = typing.Union[ExecutePromptResponse_Fulfilled, ExecutePromptResponse_Rejected]
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/execute_workflow_error_response.py` & `vellum_ai-0.5.0/src/vellum/types/rejected_execute_prompt_event.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from .rejected_prompt_execution_meta import RejectedPromptExecutionMeta
+from .vellum_error import VellumError
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ExecuteWorkflowErrorResponse(pydantic.BaseModel):
-    detail: str = pydantic.Field(description="Details about why the request failed.")
+class RejectedExecutePromptEvent(pydantic_v1.BaseModel):
+    """
+    The final data returned indicating an error occurred during the stream.
+    """
+
+    error: VellumError
+    execution_id: str
+    meta: typing.Optional[RejectedPromptExecutionMeta] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/execute_workflow_response.py` & `vellum_ai-0.5.0/src/vellum/types/terminal_node_error_result.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .execute_workflow_workflow_result_event import ExecuteWorkflowWorkflowResultEvent
+from ..core.pydantic_utilities import pydantic_v1
+from .vellum_error import VellumError
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class TerminalNodeErrorResult(pydantic_v1.BaseModel):
+    id: typing.Optional[str] = None
+    name: str = pydantic_v1.Field()
+    """
+    The unique name given to the terminal node that produced this output.
+    """
 
-class ExecuteWorkflowResponse(pydantic.BaseModel):
-    execution_id: str
-    run_id: typing.Optional[str]
-    external_id: typing.Optional[str]
-    data: ExecuteWorkflowWorkflowResultEvent
+    value: typing.Optional[VellumError] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/execute_workflow_stream_error_response.py` & `vellum_ai-0.5.0/src/vellum/types/vellum_variable.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from .vellum_variable_type import VellumVariableType
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ExecuteWorkflowStreamErrorResponse(pydantic.BaseModel):
-    detail: str = pydantic.Field(description="Details about why the request failed.")
+class VellumVariable(pydantic_v1.BaseModel):
+    id: str
+    key: str
+    type: VellumVariableType
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/execute_workflow_workflow_result_event.py` & `vellum_ai-0.5.0/src/vellum/types/execute_workflow_workflow_result_event.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from __future__ import annotations
 
 import typing
 
-import typing_extensions
-
 from .fulfilled_execute_workflow_workflow_result_event import FulfilledExecuteWorkflowWorkflowResultEvent
 from .rejected_execute_workflow_workflow_result_event import RejectedExecuteWorkflowWorkflowResultEvent
 
 
 class ExecuteWorkflowWorkflowResultEvent_Fulfilled(FulfilledExecuteWorkflowWorkflowResultEvent):
-    state: typing_extensions.Literal["FULFILLED"]
+    state: typing.Literal["FULFILLED"] = "FULFILLED"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class ExecuteWorkflowWorkflowResultEvent_Rejected(RejectedExecuteWorkflowWorkflowResultEvent):
-    state: typing_extensions.Literal["REJECTED"]
+    state: typing.Literal["REJECTED"] = "REJECTED"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 ExecuteWorkflowWorkflowResultEvent = typing.Union[
     ExecuteWorkflowWorkflowResultEvent_Fulfilled, ExecuteWorkflowWorkflowResultEvent_Rejected
 ]
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/fulfilled_execute_prompt_event.py` & `vellum_ai-0.5.0/src/vellum/types/fulfilled_execute_prompt_event.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .fulfilled_prompt_execution_meta import FulfilledPromptExecutionMeta
 from .prompt_output import PromptOutput
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class FulfilledExecutePromptEvent(pydantic.BaseModel):
+class FulfilledExecutePromptEvent(pydantic_v1.BaseModel):
     """
     The final data event returned indicating that the stream has ended and all final resolved values from the model can be found.
     """
 
     outputs: typing.List[PromptOutput]
     execution_id: str
-    meta: typing.Optional[FulfilledPromptExecutionMeta]
+    meta: typing.Optional[FulfilledPromptExecutionMeta] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/fulfilled_execute_prompt_response.py` & `vellum_ai-0.5.0/src/vellum/types/streaming_execute_prompt_event.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .prompt_execution_meta import PromptExecutionMeta
+from ..core.pydantic_utilities import pydantic_v1
 from .prompt_output import PromptOutput
+from .streaming_prompt_execution_meta import StreamingPromptExecutionMeta
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class FulfilledExecutePromptResponse(pydantic.BaseModel):
+class StreamingExecutePromptEvent(pydantic_v1.BaseModel):
     """
-    The successful response from the model containing all of the resolved values generated by the prompt.
+    The data returned for each delta during the prompt execution stream.
     """
 
-    meta: typing.Optional[PromptExecutionMeta]
-    raw: typing.Optional[typing.Dict[str, typing.Any]] = pydantic.Field(
-        description="The subset of the raw response from the model that the request opted into with `expand_raw`."
-    )
-    execution_id: str = pydantic.Field(description="The ID of the execution.")
-    outputs: typing.List[PromptOutput]
+    output: PromptOutput
+    output_index: int
+    execution_id: str
+    meta: typing.Optional[StreamingPromptExecutionMeta] = None
+    raw: typing.Optional[typing.Dict[str, typing.Any]] = pydantic_v1.Field(default=None)
+    """
+    The subset of the raw response from the model that the request opted into with `expand_raw`.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/fulfilled_execute_workflow_workflow_result_event.py` & `vellum_ai-0.5.0/src/vellum/types/generate_result_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .workflow_output import WorkflowOutput
+from ..core.pydantic_utilities import pydantic_v1
+from .enriched_normalized_completion import EnrichedNormalizedCompletion
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class FulfilledExecuteWorkflowWorkflowResultEvent(pydantic.BaseModel):
+class GenerateResultData(pydantic_v1.BaseModel):
+    completions: typing.List[EnrichedNormalizedCompletion] = pydantic_v1.Field()
     """
-    The successful response from the Workflow execution containing the produced outputs.
+    The generated completions. This will generally be a list of length one.
     """
 
-    id: str
-    ts: dt.datetime
-    outputs: typing.List[WorkflowOutput]
-
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/fulfilled_function_call.py` & `vellum_ai-0.5.0/src/vellum/types/paginated_test_suite_run_execution_list.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from .test_suite_run_execution import TestSuiteRunExecution
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class FulfilledFunctionCall(pydantic.BaseModel):
-    """
-    The final resolved function call value.
-    """
-
-    arguments: typing.Dict[str, typing.Any]
-    id: typing.Optional[str]
-    name: str
+class PaginatedTestSuiteRunExecutionList(pydantic_v1.BaseModel):
+    count: int
+    next: typing.Optional[str] = None
+    previous: typing.Optional[str] = None
+    results: typing.List[TestSuiteRunExecution]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/fulfilled_prompt_execution_meta.py` & `vellum_ai-0.5.0/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_data_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .finish_reason_enum import FinishReasonEnum
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class FulfilledPromptExecutionMeta(pydantic.BaseModel):
+class TestSuiteRunDeploymentReleaseTagExecConfigDataRequest(pydantic_v1.BaseModel):
+    deployment_id: str = pydantic_v1.Field()
     """
-    The subset of the metadata tracked by Vellum during prompt execution that the request opted into with `expand_meta`.
+    The ID of the Prompt Deployment to run the Test Suite against.
     """
 
-    latency: typing.Optional[int]
-    finish_reason: typing.Optional[FinishReasonEnum]
+    tag: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    A tag identifying which release of the Prompt Deployment to run the Test Suite against. Useful for testing past versions of the Prompt Deployment
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/fulfilled_workflow_node_result_event.py` & `vellum_ai-0.5.0/src/vellum/types/streaming_workflow_node_result_event.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .node_output_compiled_value import NodeOutputCompiledValue
 from .workflow_node_result_data import WorkflowNodeResultData
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class FulfilledWorkflowNodeResultEvent(pydantic.BaseModel):
+class StreamingWorkflowNodeResultEvent(pydantic_v1.BaseModel):
     """
-    An event that indicates that the node has fulfilled its execution.
+    An event that indicates that the node has execution is in progress.
     """
 
     id: str
     node_id: str
     node_result_id: str
-    ts: typing.Optional[dt.datetime]
-    data: typing.Optional[WorkflowNodeResultData]
-    output_values: typing.Optional[typing.List[NodeOutputCompiledValue]]
+    ts: typing.Optional[dt.datetime] = None
+    data: typing.Optional[WorkflowNodeResultData] = None
+    source_execution_id: typing.Optional[str] = None
+    output: typing.Optional[NodeOutputCompiledValue] = None
+    output_index: typing.Optional[int] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/function_call.py` & `vellum_ai-0.5.0/src/vellum/types/function_call.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from __future__ import annotations
 
 import typing
 
-import typing_extensions
-
 from .fulfilled_function_call import FulfilledFunctionCall
 from .rejected_function_call import RejectedFunctionCall
 
 
 class FunctionCall_Fulfilled(FulfilledFunctionCall):
-    state: typing_extensions.Literal["FULFILLED"]
+    state: typing.Literal["FULFILLED"] = "FULFILLED"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class FunctionCall_Rejected(RejectedFunctionCall):
-    state: typing_extensions.Literal["REJECTED"]
+    state: typing.Literal["REJECTED"] = "REJECTED"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 FunctionCall = typing.Union[FunctionCall_Fulfilled, FunctionCall_Rejected]
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/function_call_chat_message_content.py` & `vellum_ai-0.5.0/src/vellum/types/function_call_chat_message_content_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .function_call_chat_message_content_value import FunctionCallChatMessageContentValue
+from ..core.pydantic_utilities import pydantic_v1
+from .function_call_chat_message_content_value_request import FunctionCallChatMessageContentValueRequest
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class FunctionCallChatMessageContent(pydantic.BaseModel):
+class FunctionCallChatMessageContentRequest(pydantic_v1.BaseModel):
     """
     A function call value that is used in a chat message.
     """
 
-    value: FunctionCallChatMessageContentValue
+    value: FunctionCallChatMessageContentValueRequest
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/function_call_chat_message_content_request.py` & `vellum_ai-0.5.0/src/vellum/types/function_call_chat_message_content_value_request.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .function_call_chat_message_content_value_request import FunctionCallChatMessageContentValueRequest
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class FunctionCallChatMessageContentRequest(pydantic.BaseModel):
+class FunctionCallChatMessageContentValueRequest(pydantic_v1.BaseModel):
     """
-    A function call value that is used in a chat message.
+    The final resolved function call value.
     """
 
-    value: FunctionCallChatMessageContentValueRequest
+    name: str
+    arguments: typing.Dict[str, typing.Any]
+    id: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/function_call_chat_message_content_value.py` & `vellum_ai-0.5.0/src/vellum/types/test_case_string_variable_value.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class FunctionCallChatMessageContentValue(pydantic.BaseModel):
+class TestCaseStringVariableValue(pydantic_v1.BaseModel):
     """
-    The final resolved function call value.
+    A string value for a variable in a Test Case.
     """
 
+    variable_id: str
     name: str
-    arguments: typing.Dict[str, typing.Any]
-    id: typing.Optional[str]
+    value: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/function_call_chat_message_content_value_request.py` & `vellum_ai-0.5.0/src/vellum/types/workflow_execution_node_result_event.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from .workflow_node_result_event import WorkflowNodeResultEvent
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class FunctionCallChatMessageContentValueRequest(pydantic.BaseModel):
+class WorkflowExecutionNodeResultEvent(pydantic_v1.BaseModel):
     """
-    The final resolved function call value.
+    A NODE-level event emitted from the workflow's execution.
     """
 
-    name: str
-    arguments: typing.Dict[str, typing.Any]
-    id: typing.Optional[str]
+    execution_id: str
+    run_id: typing.Optional[str] = None
+    external_id: typing.Optional[str] = None
+    data: WorkflowNodeResultEvent
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/function_call_variable_value.py` & `vellum_ai-0.5.0/src/vellum/types/deployment_provider_payload_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .function_call import FunctionCall
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class FunctionCallVariableValue(pydantic.BaseModel):
-    value: FunctionCall
+class DeploymentProviderPayloadResponse(pydantic_v1.BaseModel):
+    payload: typing.Dict[str, typing.Any]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/generate_error_response.py` & `vellum_ai-0.5.0/src/vellum/types/generate_stream_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from .generate_stream_result import GenerateStreamResult
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class GenerateErrorResponse(pydantic.BaseModel):
-    detail: str = pydantic.Field(description="Details about why the request failed.")
+class GenerateStreamResponse(pydantic_v1.BaseModel):
+    delta: GenerateStreamResult
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/generate_options_request.py` & `vellum_ai-0.5.0/src/vellum/types/generate_options_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .logprobs_enum import LogprobsEnum
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class GenerateOptionsRequest(pydantic.BaseModel):
-    logprobs: typing.Optional[LogprobsEnum] = pydantic.Field(
-        description=(
-            "Which logprobs to include, if any. Defaults to NONE.\n" "\n" "- `ALL` - ALL\n" "- `NONE` - NONE\n"
-        )
-    )
+class GenerateOptionsRequest(pydantic_v1.BaseModel):
+    logprobs: typing.Optional[LogprobsEnum] = pydantic_v1.Field(default=None)
+    """
+    Which logprobs to include, if any. Defaults to NONE.
+    
+    - `ALL` - ALL
+    - `NONE` - NONE
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/generate_request.py` & `vellum_ai-0.5.0/src/vellum/types/generate_result.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .chat_message_request import ChatMessageRequest
+from ..core.pydantic_utilities import pydantic_v1
+from .generate_result_data import GenerateResultData
+from .generate_result_error import GenerateResultError
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class GenerateRequest(pydantic.BaseModel):
-    input_values: typing.Dict[str, typing.Any] = pydantic.Field(
-        description="Key/value pairs for each template variable defined in the deployment's prompt."
-    )
-    chat_history: typing.Optional[typing.List[ChatMessageRequest]] = pydantic.Field(
-        description="Optionally provide a list of chat messages that'll be used in place of the special {$chat_history} variable, if included in the prompt."
-    )
-    external_ids: typing.Optional[typing.List[str]] = pydantic.Field(
-        description="Optionally include a unique identifier for each generation, as represented outside of Vellum. Note that this should generally be a list of length one."
-    )
+
+class GenerateResult(pydantic_v1.BaseModel):
+    data: typing.Optional[GenerateResultData] = pydantic_v1.Field(default=None)
+    """
+    An object containing the resulting generation. This key will be absent if the LLM provider experienced an error.
+    """
+
+    error: typing.Optional[GenerateResultError] = pydantic_v1.Field(default=None)
+    """
+    An object containing details about the error that occurred. This key will be absent if the LLM provider did not experience an error.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/generate_response.py` & `vellum_ai-0.5.0/src/vellum/types/generate_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.9/src/vellum/types/generate_result.py` & `vellum_ai-0.5.0/src/vellum/types/prompt_node_result_data.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .generate_result_data import GenerateResultData
-from .generate_result_error import GenerateResultError
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class GenerateResult(pydantic.BaseModel):
-    data: typing.Optional[GenerateResultData] = pydantic.Field(
-        description="An object containing the resulting generation. This key will be absent if the LLM provider experienced an error."
-    )
-    error: typing.Optional[GenerateResultError] = pydantic.Field(
-        description="An object containing details about the error that occurred. This key will be absent if the LLM provider did not experience an error."
-    )
+
+class PromptNodeResultData(pydantic_v1.BaseModel):
+    output_id: str
+    array_output_id: typing.Optional[str] = None
+    text: typing.Optional[str] = None
+    delta: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/generate_result_data.py` & `vellum_ai-0.5.0/src/vellum/types/search_result_request.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .enriched_normalized_completion import EnrichedNormalizedCompletion
+from ..core.pydantic_utilities import pydantic_v1
+from .search_result_document_request import SearchResultDocumentRequest
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class GenerateResultData(pydantic.BaseModel):
-    completions: typing.List[EnrichedNormalizedCompletion] = pydantic.Field(
-        description="The generated completions. This will generally be a list of length one."
-    )
+class SearchResultRequest(pydantic_v1.BaseModel):
+    text: str = pydantic_v1.Field()
+    """
+    The text of the chunk that matched the search query.
+    """
+
+    score: float = pydantic_v1.Field()
+    """
+    A score representing how well the chunk matches the search query.
+    """
+
+    keywords: typing.List[str]
+    document: SearchResultDocumentRequest = pydantic_v1.Field()
+    """
+    The document that contains the chunk that matched the search query.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/generate_result_error.py` & `vellum_ai-0.5.0/src/vellum/types/initiated_execute_prompt_event.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from .initiated_prompt_execution_meta import InitiatedPromptExecutionMeta
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class InitiatedExecutePromptEvent(pydantic_v1.BaseModel):
+    """
+    The initial data returned indicating that the response from the model has returned and begun streaming.
+    """
 
-class GenerateResultError(pydantic.BaseModel):
-    message: str = pydantic.Field(description="The error message returned by the LLM provider.")
+    meta: typing.Optional[InitiatedPromptExecutionMeta] = None
+    execution_id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/generate_stream_response.py` & `vellum_ai-0.5.0/src/vellum/types/named_test_case_chat_history_variable_value.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .generate_stream_result import GenerateStreamResult
+from ..core.pydantic_utilities import pydantic_v1
+from .chat_message import ChatMessage
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class NamedTestCaseChatHistoryVariableValue(pydantic_v1.BaseModel):
+    """
+    Named Test Case value that is of type CHAT_HISTORY
+    """
 
-class GenerateStreamResponse(pydantic.BaseModel):
-    delta: GenerateStreamResult
+    value: typing.Optional[typing.List[ChatMessage]] = None
+    name: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/generate_stream_result.py` & `vellum_ai-0.5.0/src/vellum/types/generate_stream_result.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .generate_result_error import GenerateResultError
 from .generate_stream_result_data import GenerateStreamResultData
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class GenerateStreamResult(pydantic.BaseModel):
+class GenerateStreamResult(pydantic_v1.BaseModel):
     request_index: int
-    data: typing.Optional[GenerateStreamResultData]
-    error: typing.Optional[GenerateResultError]
+    data: typing.Optional[GenerateStreamResultData] = None
+    error: typing.Optional[GenerateResultError] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/generate_stream_result_data.py` & `vellum_ai-0.5.0/src/vellum/types/templating_node_result_data.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .enriched_normalized_completion import EnrichedNormalizedCompletion
+from ..core.pydantic_utilities import pydantic_v1
+from .templating_node_result_output import TemplatingNodeResultOutput
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class GenerateStreamResultData(pydantic.BaseModel):
-    completion_index: int
-    completion: EnrichedNormalizedCompletion
+class TemplatingNodeResultData(pydantic_v1.BaseModel):
+    output: TemplatingNodeResultOutput
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/image_chat_message_content.py` & `vellum_ai-0.5.0/src/vellum/types/named_test_case_json_variable_value.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .vellum_image import VellumImage
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ImageChatMessageContent(pydantic.BaseModel):
+class NamedTestCaseJsonVariableValue(pydantic_v1.BaseModel):
     """
-    An image value that is used in a chat message.
+    Named Test Case value that is of type JSON
     """
 
-    value: VellumImage
+    value: typing.Optional[typing.Dict[str, typing.Any]] = None
+    name: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/image_chat_message_content_request.py` & `vellum_ai-0.5.0/src/vellum/types/image_chat_message_content.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .vellum_image_request import VellumImageRequest
+from ..core.pydantic_utilities import pydantic_v1
+from .vellum_image import VellumImage
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ImageChatMessageContentRequest(pydantic.BaseModel):
+class ImageChatMessageContent(pydantic_v1.BaseModel):
     """
     An image value that is used in a chat message.
     """
 
-    value: VellumImageRequest
+    value: VellumImage
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/initiated_execute_prompt_event.py` & `vellum_ai-0.5.0/src/vellum/types/workflow_execution_workflow_result_event.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .initiated_prompt_execution_meta import InitiatedPromptExecutionMeta
+from ..core.pydantic_utilities import pydantic_v1
+from .workflow_result_event import WorkflowResultEvent
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class InitiatedExecutePromptEvent(pydantic.BaseModel):
+class WorkflowExecutionWorkflowResultEvent(pydantic_v1.BaseModel):
     """
-    The initial data returned indicating that the response from the model has returned and begun streaming.
+    A WORKFLOW-level event emitted from the workflow's execution.
     """
 
-    meta: typing.Optional[InitiatedPromptExecutionMeta]
     execution_id: str
+    run_id: typing.Optional[str] = None
+    external_id: typing.Optional[str] = None
+    data: WorkflowResultEvent
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/initiated_prompt_execution_meta.py` & `vellum_ai-0.5.0/src/vellum/types/initiated_prompt_execution_meta.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class InitiatedPromptExecutionMeta(pydantic.BaseModel):
+class InitiatedPromptExecutionMeta(pydantic_v1.BaseModel):
     """
     The subset of the metadata tracked by Vellum during prompt execution that the request opted into with `expand_meta`.
     """
 
-    model_name: typing.Optional[str]
-    latency: typing.Optional[int]
-    deployment_release_tag: typing.Optional[str]
-    prompt_version_id: typing.Optional[str]
+    model_name: typing.Optional[str] = None
+    latency: typing.Optional[int] = None
+    deployment_release_tag: typing.Optional[str] = None
+    prompt_version_id: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/initiated_workflow_node_result_event.py` & `vellum_ai-0.5.0/src/vellum/types/fulfilled_workflow_node_result_event.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .node_input_variable_compiled_value import NodeInputVariableCompiledValue
+from ..core.pydantic_utilities import pydantic_v1
+from .node_output_compiled_value import NodeOutputCompiledValue
 from .workflow_node_result_data import WorkflowNodeResultData
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class InitiatedWorkflowNodeResultEvent(pydantic.BaseModel):
+class FulfilledWorkflowNodeResultEvent(pydantic_v1.BaseModel):
     """
-    An event that indicates that the node has initiated its execution.
+    An event that indicates that the node has fulfilled its execution.
     """
 
     id: str
     node_id: str
     node_result_id: str
-    ts: typing.Optional[dt.datetime]
-    data: typing.Optional[WorkflowNodeResultData]
-    input_values: typing.Optional[typing.List[NodeInputVariableCompiledValue]]
+    ts: typing.Optional[dt.datetime] = None
+    data: typing.Optional[WorkflowNodeResultData] = None
+    source_execution_id: typing.Optional[str] = None
+    output_values: typing.List[NodeOutputCompiledValue]
+    mocked: typing.Optional[bool] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/json_input_request.py` & `vellum_ai-0.5.0/src/vellum/types/fulfilled_function_call_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from .fulfilled_enum import FulfilledEnum
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class JsonInputRequest(pydantic.BaseModel):
+class FulfilledFunctionCallRequest(pydantic_v1.BaseModel):
     """
-    A user input representing a JSON object
+    The final resolved function call value.
     """
 
-    name: str = pydantic.Field(description="The variable's name, as defined in the deployment.")
-    value: typing.Dict[str, typing.Any]
+    state: FulfilledEnum
+    arguments: typing.Dict[str, typing.Any]
+    id: typing.Optional[str] = None
+    name: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/json_variable_value.py` & `vellum_ai-0.5.0/src/vellum/types/error_variable_value.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from .vellum_error import VellumError
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class JsonVariableValue(pydantic.BaseModel):
-    value: typing.Optional[typing.Dict[str, typing.Any]]
+class ErrorVariableValue(pydantic_v1.BaseModel):
+    value: typing.Optional[VellumError] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/metadata_filter_config_request.py` & `vellum_ai-0.5.0/src/vellum/types/metadata_filter_rule_request.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 # This file was auto-generated by Fern from our API Definition.
 
+from __future__ import annotations
+
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .logical_operator import LogicalOperator
 from .metadata_filter_rule_combinator import MetadataFilterRuleCombinator
-from .metadata_filter_rule_request import MetadataFilterRuleRequest
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
 
-class MetadataFilterConfigRequest(pydantic.BaseModel):
-    combinator: typing.Optional[MetadataFilterRuleCombinator]
-    negated: typing.Optional[bool]
-    rules: typing.Optional[typing.List[MetadataFilterRuleRequest]]
-    field: typing.Optional[str]
-    operator: typing.Optional[LogicalOperator]
-    value: typing.Optional[str]
+class MetadataFilterRuleRequest(pydantic_v1.BaseModel):
+    combinator: typing.Optional[MetadataFilterRuleCombinator] = None
+    negated: typing.Optional[bool] = None
+    rules: typing.Optional[typing.List[MetadataFilterRuleRequest]] = None
+    field: typing.Optional[str] = None
+    operator: typing.Optional[LogicalOperator] = None
+    value: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
+
+
+MetadataFilterRuleRequest.update_forward_refs()
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/metadata_filter_rule_request.py` & `vellum_ai-0.5.0/src/vellum/types/paginated_document_index_read_list.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from __future__ import annotations
-
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .logical_operator import LogicalOperator
-from .metadata_filter_rule_combinator import MetadataFilterRuleCombinator
+from ..core.pydantic_utilities import pydantic_v1
+from .document_index_read import DocumentIndexRead
+
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class MetadataFilterRuleRequest(pydantic.BaseModel):
-    combinator: typing.Optional[MetadataFilterRuleCombinator]
-    negated: typing.Optional[bool]
-    rules: typing.Optional[typing.List[MetadataFilterRuleRequest]]
-    field: typing.Optional[str]
-    operator: typing.Optional[LogicalOperator]
-    value: typing.Optional[str]
+class PaginatedDocumentIndexReadList(pydantic_v1.BaseModel):
+    count: typing.Optional[int] = None
+    next: typing.Optional[str] = None
+    previous: typing.Optional[str] = None
+    results: typing.Optional[typing.List[DocumentIndexRead]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
-
-
-MetadataFilterRuleRequest.update_forward_refs()
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/model_version_build_config.py` & `vellum_ai-0.5.0/src/vellum/types/named_test_case_search_results_variable_value.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .model_version_sandbox_snapshot import ModelVersionSandboxSnapshot
+from ..core.pydantic_utilities import pydantic_v1
+from .search_result import SearchResult
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class ModelVersionBuildConfig(pydantic.BaseModel):
-    base_model: str = pydantic.Field(
-        description="The name of the base model used to create this model version, as identified by the LLM provider."
-    )
-    sandbox_snapshot: typing.Optional[ModelVersionSandboxSnapshot] = pydantic.Field(
-        description="Information about the sandbox snapshot that was used to create this model version, if applicable."
-    )
-    prompt_version_id: typing.Optional[str]
+
+class NamedTestCaseSearchResultsVariableValue(pydantic_v1.BaseModel):
+    """
+    Named Test Case value that is of type SEARCH_RESULTS
+    """
+
+    value: typing.Optional[typing.List[SearchResult]] = None
+    name: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/model_version_exec_config.py` & `vellum_ai-0.5.0/src/vellum/types/workflow_result_event_output_data_json.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .model_version_exec_config_parameters import ModelVersionExecConfigParameters
-from .prompt_template_block_data import PromptTemplateBlockData
-from .vellum_variable import VellumVariable
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class ModelVersionExecConfig(pydantic.BaseModel):
-    parameters: ModelVersionExecConfigParameters = pydantic.Field(
-        description="The generation parameters that are passed to the LLM provider at runtime."
-    )
-    input_variables: typing.List[VellumVariable] = pydantic.Field(
-        description="Input variables specified in the prompt template."
-    )
-    prompt_template: typing.Optional[str] = pydantic.Field(
-        description="The template used to generate prompts for this model version."
-    )
-    prompt_block_data: typing.Optional[PromptTemplateBlockData]
-    prompt_syntax_version: typing.Optional[int]
+from ..core.pydantic_utilities import pydantic_v1
+from .workflow_node_result_event_state import WorkflowNodeResultEventState
+
+
+class WorkflowResultEventOutputDataJson(pydantic_v1.BaseModel):
+    """
+    A JSON output streamed from a Workflow execution.
+    """
+
+    id: typing.Optional[str] = None
+    name: str
+    state: WorkflowNodeResultEventState
+    node_id: str
+    delta: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The newly output string value. Only relevant for string outputs with a state of STREAMING.
+    """
+
+    value: typing.Optional[typing.Dict[str, typing.Any]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/model_version_exec_config_parameters.py` & `vellum_ai-0.5.0/src/vellum/types/test_suite_run_execution_metric_definition.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class ModelVersionExecConfigParameters(pydantic.BaseModel):
-    temperature: typing.Optional[float]
-    max_tokens: typing.Optional[int]
-    top_p: float
-    frequency_penalty: float
-    presence_penalty: float
-    logit_bias: typing.Optional[typing.Dict[str, typing.Optional[float]]]
-    stop: typing.Optional[typing.List[str]]
-    top_k: typing.Optional[float]
-    custom_parameters: typing.Optional[typing.Dict[str, typing.Any]]
+
+class TestSuiteRunExecutionMetricDefinition(pydantic_v1.BaseModel):
+    id: typing.Optional[str] = None
+    label: typing.Optional[str] = None
+    name: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/model_version_sandbox_snapshot.py` & `vellum_ai-0.5.0/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_data_request.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ModelVersionSandboxSnapshot(pydantic.BaseModel):
-    id: str = pydantic.Field(description="The ID of the sandbox snapshot.")
-    prompt_index: typing.Optional[int] = pydantic.Field(description="The index of the prompt in the sandbox snapshot.")
-    prompt_id: typing.Optional[str] = pydantic.Field(description="The id of the prompt in the sandbox snapshot.")
-    sandbox_id: typing.Optional[str]
+class TestSuiteRunWorkflowReleaseTagExecConfigDataRequest(pydantic_v1.BaseModel):
+    workflow_deployment_id: str = pydantic_v1.Field()
+    """
+    The ID of the Workflow Deployment to run the Test Suite against.
+    """
+
+    tag: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    A tag identifying which release of the Workflow Deployment to run the Test Suite against. Useful for testing past versions of the Workflow Deployment
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/named_test_case_chat_history_variable_value_request.py` & `vellum_ai-0.5.0/src/vellum/types/named_scenario_input_chat_history_variable_value_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .chat_message_request import ChatMessageRequest
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class NamedScenarioInputChatHistoryVariableValueRequest(pydantic_v1.BaseModel):
+    """
+    Named Prompt Sandbox Scenario input value that is of type CHAT_HISTORY
+    """
 
-class NamedTestCaseChatHistoryVariableValueRequest(pydantic.BaseModel):
+    value: typing.Optional[typing.List[ChatMessageRequest]] = None
     name: str
-    value: typing.Optional[typing.List[ChatMessageRequest]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/named_test_case_error_variable_value_request.py` & `vellum_ai-0.5.0/src/vellum/types/named_test_case_search_results_variable_value_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .vellum_error_request import VellumErrorRequest
+from ..core.pydantic_utilities import pydantic_v1
+from .search_result_request import SearchResultRequest
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class NamedTestCaseSearchResultsVariableValueRequest(pydantic_v1.BaseModel):
+    """
+    Named Test Case value that is of type SEARCH_RESULTS
+    """
 
-class NamedTestCaseErrorVariableValueRequest(pydantic.BaseModel):
+    value: typing.Optional[typing.List[SearchResultRequest]] = None
     name: str
-    value: typing.Optional[VellumErrorRequest]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/named_test_case_json_variable_value_request.py` & `vellum_ai-0.5.0/src/vellum/types/named_test_case_json_variable_value_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class NamedTestCaseJsonVariableValueRequest(pydantic_v1.BaseModel):
+    """
+    Named Test Case value that is of type JSON
+    """
 
-class NamedTestCaseJsonVariableValueRequest(pydantic.BaseModel):
+    value: typing.Optional[typing.Dict[str, typing.Any]] = None
     name: str
-    value: typing.Optional[typing.Dict[str, typing.Any]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/named_test_case_number_variable_value_request.py` & `vellum_ai-0.5.0/src/vellum/types/function_call_chat_message_content_value.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class FunctionCallChatMessageContentValue(pydantic_v1.BaseModel):
+    """
+    The final resolved function call value.
+    """
 
-class NamedTestCaseNumberVariableValueRequest(pydantic.BaseModel):
     name: str
-    value: typing.Optional[float]
+    arguments: typing.Dict[str, typing.Any]
+    id: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/named_test_case_search_results_variable_value_request.py` & `vellum_ai-0.5.0/src/vellum/types/rejected_function_call.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .search_result_request import SearchResultRequest
+from ..core.pydantic_utilities import pydantic_v1
+from .vellum_error import VellumError
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class RejectedFunctionCall(pydantic_v1.BaseModel):
+    """
+    Returned if the function call failed to parse for some reason.
+    """
 
-class NamedTestCaseSearchResultsVariableValueRequest(pydantic.BaseModel):
+    error: VellumError
+    id: typing.Optional[str] = None
     name: str
-    value: typing.Optional[typing.List[SearchResultRequest]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/named_test_case_string_variable_value_request.py` & `vellum_ai-0.5.0/src/vellum/types/test_case_search_results_variable_value.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from .search_result import SearchResult
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class TestCaseSearchResultsVariableValue(pydantic_v1.BaseModel):
+    """
+    A search results value for a variable in a Test Case.
+    """
 
-class NamedTestCaseStringVariableValueRequest(pydantic.BaseModel):
+    variable_id: str
     name: str
-    value: typing.Optional[str]
+    value: typing.Optional[typing.List[SearchResult]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/named_test_case_variable_value_request.py` & `vellum_ai-0.5.0/src/vellum/types/named_test_case_variable_value_request.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,78 +1,94 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from __future__ import annotations
 
 import typing
 
-import typing_extensions
-
 from .named_test_case_chat_history_variable_value_request import NamedTestCaseChatHistoryVariableValueRequest
 from .named_test_case_error_variable_value_request import NamedTestCaseErrorVariableValueRequest
+from .named_test_case_function_call_variable_value_request import NamedTestCaseFunctionCallVariableValueRequest
 from .named_test_case_json_variable_value_request import NamedTestCaseJsonVariableValueRequest
 from .named_test_case_number_variable_value_request import NamedTestCaseNumberVariableValueRequest
 from .named_test_case_search_results_variable_value_request import NamedTestCaseSearchResultsVariableValueRequest
 from .named_test_case_string_variable_value_request import NamedTestCaseStringVariableValueRequest
 
 
 class NamedTestCaseVariableValueRequest_String(NamedTestCaseStringVariableValueRequest):
-    type: typing_extensions.Literal["STRING"]
+    type: typing.Literal["STRING"] = "STRING"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class NamedTestCaseVariableValueRequest_Number(NamedTestCaseNumberVariableValueRequest):
-    type: typing_extensions.Literal["NUMBER"]
+    type: typing.Literal["NUMBER"] = "NUMBER"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class NamedTestCaseVariableValueRequest_Json(NamedTestCaseJsonVariableValueRequest):
-    type: typing_extensions.Literal["JSON"]
+    type: typing.Literal["JSON"] = "JSON"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class NamedTestCaseVariableValueRequest_ChatHistory(NamedTestCaseChatHistoryVariableValueRequest):
-    type: typing_extensions.Literal["CHAT_HISTORY"]
+    type: typing.Literal["CHAT_HISTORY"] = "CHAT_HISTORY"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class NamedTestCaseVariableValueRequest_SearchResults(NamedTestCaseSearchResultsVariableValueRequest):
-    type: typing_extensions.Literal["SEARCH_RESULTS"]
+    type: typing.Literal["SEARCH_RESULTS"] = "SEARCH_RESULTS"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class NamedTestCaseVariableValueRequest_Error(NamedTestCaseErrorVariableValueRequest):
-    type: typing_extensions.Literal["ERROR"]
+    type: typing.Literal["ERROR"] = "ERROR"
+
+    class Config:
+        frozen = True
+        smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+
+
+class NamedTestCaseVariableValueRequest_FunctionCall(NamedTestCaseFunctionCallVariableValueRequest):
+    type: typing.Literal["FUNCTION_CALL"] = "FUNCTION_CALL"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 NamedTestCaseVariableValueRequest = typing.Union[
     NamedTestCaseVariableValueRequest_String,
     NamedTestCaseVariableValueRequest_Number,
     NamedTestCaseVariableValueRequest_Json,
     NamedTestCaseVariableValueRequest_ChatHistory,
     NamedTestCaseVariableValueRequest_SearchResults,
     NamedTestCaseVariableValueRequest_Error,
+    NamedTestCaseVariableValueRequest_FunctionCall,
 ]
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/node_input_compiled_array_value.py` & `vellum_ai-0.5.0/src/vellum/types/named_test_case_number_variable_value_request.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .array_variable_value_item import ArrayVariableValueItem
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class NamedTestCaseNumberVariableValueRequest(pydantic_v1.BaseModel):
+    """
+    Named Test Case value that is of type NUMBER
+    """
 
-class NodeInputCompiledArrayValue(pydantic.BaseModel):
-    node_input_id: str
-    key: str
-    value: typing.Optional[typing.List[ArrayVariableValueItem]]
+    value: typing.Optional[float] = None
+    name: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/node_input_compiled_chat_history_value.py` & `vellum_ai-0.5.0/src/vellum/types/node_input_compiled_error_value.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .chat_message import ChatMessage
+from ..core.pydantic_utilities import pydantic_v1
+from .vellum_error import VellumError
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class NodeInputCompiledChatHistoryValue(pydantic.BaseModel):
+class NodeInputCompiledErrorValue(pydantic_v1.BaseModel):
     node_input_id: str
     key: str
-    value: typing.Optional[typing.List[ChatMessage]]
+    value: typing.Optional[VellumError] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/node_input_compiled_error_value.py` & `vellum_ai-0.5.0/src/vellum/types/node_output_compiled_error_value.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .vellum_error import VellumError
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class NodeInputCompiledErrorValue(pydantic.BaseModel):
-    node_input_id: str
-    key: str
-    value: typing.Optional[VellumError]
+class NodeOutputCompiledErrorValue(pydantic_v1.BaseModel):
+    node_output_id: str
+    value: typing.Optional[VellumError] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/node_input_compiled_json_value.py` & `vellum_ai-0.5.0/src/vellum/types/search_weights_request.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class NodeInputCompiledJsonValue(pydantic.BaseModel):
-    node_input_id: str
-    key: str
-    value: typing.Optional[typing.Dict[str, typing.Any]]
+class SearchWeightsRequest(pydantic_v1.BaseModel):
+    semantic_similarity: typing.Optional[float] = pydantic_v1.Field(default=None)
+    """
+    The relative weight to give to semantic similarity
+    """
+
+    keywords: typing.Optional[float] = pydantic_v1.Field(default=None)
+    """
+    The relative weight to give to keywords
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/node_input_compiled_number_value.py` & `vellum_ai-0.5.0/src/vellum/types/named_test_case_function_call_variable_value.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from .fulfilled_function_call import FulfilledFunctionCall
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class NamedTestCaseFunctionCallVariableValue(pydantic_v1.BaseModel):
+    """
+    Named Test Case value that is of type FUNCTION_CALL
+    """
 
-class NodeInputCompiledNumberValue(pydantic.BaseModel):
-    node_input_id: str
-    key: str
-    value: typing.Optional[float]
+    value: typing.Optional[FulfilledFunctionCall] = None
+    name: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/node_input_compiled_search_results_value.py` & `vellum_ai-0.5.0/src/vellum/types/named_test_case_string_variable_value.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .search_result import SearchResult
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class NamedTestCaseStringVariableValue(pydantic_v1.BaseModel):
+    """
+    Named Test Case value that is of type STRING
+    """
 
-class NodeInputCompiledSearchResultsValue(pydantic.BaseModel):
-    node_input_id: str
-    key: str
-    value: typing.Optional[typing.List[SearchResult]]
+    value: typing.Optional[str] = None
+    name: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/node_input_compiled_string_value.py` & `vellum_ai-0.5.0/src/vellum/types/workflow_result_event_output_data_number.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from .workflow_node_result_event_state import WorkflowNodeResultEventState
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class WorkflowResultEventOutputDataNumber(pydantic_v1.BaseModel):
+    """
+    A number output streamed from a Workflow execution.
+    """
+
+    id: typing.Optional[str] = None
+    name: str
+    state: WorkflowNodeResultEventState
+    node_id: str
+    delta: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The newly output string value. Only relevant for string outputs with a state of STREAMING.
+    """
 
-class NodeInputCompiledStringValue(pydantic.BaseModel):
-    node_input_id: str
-    key: str
-    value: typing.Optional[str]
+    value: typing.Optional[float] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/node_input_variable_compiled_value.py` & `vellum_ai-0.5.0/src/vellum/types/node_input_variable_compiled_value.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,89 +1,106 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from __future__ import annotations
 
 import typing
 
-import typing_extensions
-
 from .node_input_compiled_array_value import NodeInputCompiledArrayValue
 from .node_input_compiled_chat_history_value import NodeInputCompiledChatHistoryValue
 from .node_input_compiled_error_value import NodeInputCompiledErrorValue
+from .node_input_compiled_function_call import NodeInputCompiledFunctionCall
 from .node_input_compiled_json_value import NodeInputCompiledJsonValue
 from .node_input_compiled_number_value import NodeInputCompiledNumberValue
 from .node_input_compiled_search_results_value import NodeInputCompiledSearchResultsValue
 from .node_input_compiled_string_value import NodeInputCompiledStringValue
 
 
 class NodeInputVariableCompiledValue_String(NodeInputCompiledStringValue):
-    type: typing_extensions.Literal["STRING"]
+    type: typing.Literal["STRING"] = "STRING"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class NodeInputVariableCompiledValue_Number(NodeInputCompiledNumberValue):
-    type: typing_extensions.Literal["NUMBER"]
+    type: typing.Literal["NUMBER"] = "NUMBER"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class NodeInputVariableCompiledValue_Json(NodeInputCompiledJsonValue):
-    type: typing_extensions.Literal["JSON"]
+    type: typing.Literal["JSON"] = "JSON"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class NodeInputVariableCompiledValue_ChatHistory(NodeInputCompiledChatHistoryValue):
-    type: typing_extensions.Literal["CHAT_HISTORY"]
+    type: typing.Literal["CHAT_HISTORY"] = "CHAT_HISTORY"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class NodeInputVariableCompiledValue_SearchResults(NodeInputCompiledSearchResultsValue):
-    type: typing_extensions.Literal["SEARCH_RESULTS"]
+    type: typing.Literal["SEARCH_RESULTS"] = "SEARCH_RESULTS"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class NodeInputVariableCompiledValue_Error(NodeInputCompiledErrorValue):
-    type: typing_extensions.Literal["ERROR"]
+    type: typing.Literal["ERROR"] = "ERROR"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class NodeInputVariableCompiledValue_Array(NodeInputCompiledArrayValue):
-    type: typing_extensions.Literal["ARRAY"]
+    type: typing.Literal["ARRAY"] = "ARRAY"
+
+    class Config:
+        frozen = True
+        smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+
+
+class NodeInputVariableCompiledValue_FunctionCall(NodeInputCompiledFunctionCall):
+    type: typing.Literal["FUNCTION_CALL"] = "FUNCTION_CALL"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 NodeInputVariableCompiledValue = typing.Union[
     NodeInputVariableCompiledValue_String,
     NodeInputVariableCompiledValue_Number,
     NodeInputVariableCompiledValue_Json,
     NodeInputVariableCompiledValue_ChatHistory,
     NodeInputVariableCompiledValue_SearchResults,
     NodeInputVariableCompiledValue_Error,
     NodeInputVariableCompiledValue_Array,
+    NodeInputVariableCompiledValue_FunctionCall,
 ]
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/node_output_compiled_array_value.py` & `vellum_ai-0.5.0/src/vellum/types/node_output_compiled_array_value.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .array_variable_value_item import ArrayVariableValueItem
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class NodeOutputCompiledArrayValue(pydantic.BaseModel):
+class NodeOutputCompiledArrayValue(pydantic_v1.BaseModel):
     node_output_id: str
-    value: typing.Optional[typing.List[ArrayVariableValueItem]]
+    value: typing.Optional[typing.List[ArrayVariableValueItem]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/node_output_compiled_chat_history_value.py` & `vellum_ai-0.5.0/src/vellum/types/node_input_compiled_chat_history_value.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .chat_message import ChatMessage
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class NodeOutputCompiledChatHistoryValue(pydantic.BaseModel):
-    node_output_id: str
-    value: typing.Optional[typing.List[ChatMessage]]
+class NodeInputCompiledChatHistoryValue(pydantic_v1.BaseModel):
+    node_input_id: str
+    key: str
+    value: typing.Optional[typing.List[ChatMessage]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/node_output_compiled_error_value.py` & `vellum_ai-0.5.0/src/vellum/types/execution_json_vellum_value.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .vellum_error import VellumError
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class ExecutionJsonVellumValue(pydantic_v1.BaseModel):
+    id: str = pydantic_v1.Field()
+    """
+    The variable's uniquely identifying internal id.
+    """
 
-class NodeOutputCompiledErrorValue(pydantic.BaseModel):
-    node_output_id: str
-    value: typing.Optional[VellumError]
+    name: str
+    value: typing.Optional[typing.Dict[str, typing.Any]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/node_output_compiled_function_value.py` & `vellum_ai-0.5.0/src/vellum/types/node_input_compiled_function_call.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .function_call import FunctionCall
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class NodeOutputCompiledFunctionValue(pydantic.BaseModel):
-    node_output_id: str
-    value: typing.Optional[FunctionCall]
+class NodeInputCompiledFunctionCall(pydantic_v1.BaseModel):
+    node_input_id: str
+    key: str
+    value: typing.Optional[FunctionCall] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/node_output_compiled_json_value.py` & `vellum_ai-0.5.0/src/vellum/types/test_case_json_variable_value.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class TestCaseJsonVariableValue(pydantic_v1.BaseModel):
+    """
+    A JSON value for a variable in a Test Case.
+    """
 
-class NodeOutputCompiledJsonValue(pydantic.BaseModel):
-    node_output_id: str
-    value: typing.Optional[typing.Dict[str, typing.Any]]
+    variable_id: str
+    name: str
+    value: typing.Optional[typing.Dict[str, typing.Any]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/node_output_compiled_number_value.py` & `vellum_ai-0.5.0/src/vellum/types/templating_node_result.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from .templating_node_result_data import TemplatingNodeResultData
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class TemplatingNodeResult(pydantic_v1.BaseModel):
+    """
+    A Node Result Event emitted from a Templating Node.
+    """
 
-class NodeOutputCompiledNumberValue(pydantic.BaseModel):
-    node_output_id: str
-    value: typing.Optional[float]
+    data: TemplatingNodeResultData
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/node_output_compiled_search_results_value.py` & `vellum_ai-0.5.0/src/vellum/types/image_variable_value.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .search_result import SearchResult
+from ..core.pydantic_utilities import pydantic_v1
+from .vellum_image import VellumImage
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class ImageVariableValue(pydantic_v1.BaseModel):
+    """
+    A base Vellum primitive value representing an image.
+    """
 
-class NodeOutputCompiledSearchResultsValue(pydantic.BaseModel):
-    node_output_id: str
-    value: typing.Optional[typing.List[SearchResult]]
+    value: typing.Optional[VellumImage] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/node_output_compiled_string_value.py` & `vellum_ai-0.5.0/src/vellum/types/json_input_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class JsonInputRequest(pydantic_v1.BaseModel):
+    """
+    A user input representing a JSON object
+    """
 
-class NodeOutputCompiledStringValue(pydantic.BaseModel):
-    node_output_id: str
-    value: typing.Optional[str]
+    name: str = pydantic_v1.Field()
+    """
+    The variable's name, as defined in the deployment.
+    """
+
+    value: typing.Dict[str, typing.Any]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/node_output_compiled_value.py` & `vellum_ai-0.5.0/src/vellum/types/node_output_compiled_value.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,95 +1,101 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from __future__ import annotations
 
 import typing
 
-import typing_extensions
-
 from .node_output_compiled_array_value import NodeOutputCompiledArrayValue
 from .node_output_compiled_chat_history_value import NodeOutputCompiledChatHistoryValue
 from .node_output_compiled_error_value import NodeOutputCompiledErrorValue
 from .node_output_compiled_function_value import NodeOutputCompiledFunctionValue
 from .node_output_compiled_json_value import NodeOutputCompiledJsonValue
 from .node_output_compiled_number_value import NodeOutputCompiledNumberValue
 from .node_output_compiled_search_results_value import NodeOutputCompiledSearchResultsValue
 from .node_output_compiled_string_value import NodeOutputCompiledStringValue
 
 
 class NodeOutputCompiledValue_String(NodeOutputCompiledStringValue):
-    type: typing_extensions.Literal["STRING"]
+    type: typing.Literal["STRING"] = "STRING"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class NodeOutputCompiledValue_Number(NodeOutputCompiledNumberValue):
-    type: typing_extensions.Literal["NUMBER"]
+    type: typing.Literal["NUMBER"] = "NUMBER"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class NodeOutputCompiledValue_Json(NodeOutputCompiledJsonValue):
-    type: typing_extensions.Literal["JSON"]
+    type: typing.Literal["JSON"] = "JSON"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class NodeOutputCompiledValue_ChatHistory(NodeOutputCompiledChatHistoryValue):
-    type: typing_extensions.Literal["CHAT_HISTORY"]
+    type: typing.Literal["CHAT_HISTORY"] = "CHAT_HISTORY"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class NodeOutputCompiledValue_SearchResults(NodeOutputCompiledSearchResultsValue):
-    type: typing_extensions.Literal["SEARCH_RESULTS"]
+    type: typing.Literal["SEARCH_RESULTS"] = "SEARCH_RESULTS"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class NodeOutputCompiledValue_Error(NodeOutputCompiledErrorValue):
-    type: typing_extensions.Literal["ERROR"]
+    type: typing.Literal["ERROR"] = "ERROR"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class NodeOutputCompiledValue_Array(NodeOutputCompiledArrayValue):
-    type: typing_extensions.Literal["ARRAY"]
+    type: typing.Literal["ARRAY"] = "ARRAY"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class NodeOutputCompiledValue_FunctionCall(NodeOutputCompiledFunctionValue):
-    type: typing_extensions.Literal["FUNCTION_CALL"]
+    type: typing.Literal["FUNCTION_CALL"] = "FUNCTION_CALL"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 NodeOutputCompiledValue = typing.Union[
     NodeOutputCompiledValue_String,
     NodeOutputCompiledValue_Number,
     NodeOutputCompiledValue_Json,
     NodeOutputCompiledValue_ChatHistory,
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/normalized_log_probs.py` & `vellum_ai-0.5.0/src/vellum/types/generate_error_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .normalized_token_log_probs import NormalizedTokenLogProbs
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class NormalizedLogProbs(pydantic.BaseModel):
-    tokens: typing.List[NormalizedTokenLogProbs]
-    likelihood: typing.Optional[float]
+class GenerateErrorResponse(pydantic_v1.BaseModel):
+    detail: str = pydantic_v1.Field()
+    """
+    Details about why the request failed.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/normalized_token_log_probs.py` & `vellum_ai-0.5.0/src/vellum/types/normalized_token_log_probs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class NormalizedTokenLogProbs(pydantic.BaseModel):
+class NormalizedTokenLogProbs(pydantic_v1.BaseModel):
     token: str
-    logprob: typing.Optional[float]
-    top_logprobs: typing.Optional[typing.Dict[str, typing.Optional[float]]]
+    logprob: typing.Optional[float] = None
+    top_logprobs: typing.Optional[typing.Dict[str, typing.Optional[float]]] = None
     text_offset: int
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/number_variable_value.py` & `vellum_ai-0.5.0/src/vellum/types/search_result_document.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,43 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class NumberVariableValue(pydantic.BaseModel):
-    value: typing.Optional[float]
+class SearchResultDocument(pydantic_v1.BaseModel):
+    id: str = pydantic_v1.Field()
+    """
+    The ID of the document.
+    """
+
+    label: str = pydantic_v1.Field()
+    """
+    The human-readable name for the document.
+    """
+
+    external_id: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The unique ID of the document as represented in an external system and specified when it was originally uploaded.
+    """
+
+    metadata: typing.Optional[typing.Dict[str, typing.Any]] = pydantic_v1.Field(default=None)
+    """
+    A previously supplied JSON object containing metadata that can be filtered on when searching.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/paginated_slim_deployment_read_list.py` & `vellum_ai-0.5.0/src/vellum/types/terminal_node_array_result.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .slim_deployment_read import SlimDeploymentRead
+from ..core.pydantic_utilities import pydantic_v1
+from .array_variable_value_item import ArrayVariableValueItem
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class TerminalNodeArrayResult(pydantic_v1.BaseModel):
+    id: typing.Optional[str] = None
+    name: str = pydantic_v1.Field()
+    """
+    The unique name given to the terminal node that produced this output.
+    """
 
-class PaginatedSlimDeploymentReadList(pydantic.BaseModel):
-    count: typing.Optional[int]
-    next: typing.Optional[str]
-    previous: typing.Optional[str]
-    results: typing.Optional[typing.List[SlimDeploymentRead]]
+    value: typing.Optional[typing.List[ArrayVariableValueItem]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/paginated_slim_document_list.py` & `vellum_ai-0.5.0/src/vellum/types/test_suite_run_execution.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .slim_document import SlimDocument
+from ..core.pydantic_utilities import pydantic_v1
+from .test_suite_run_execution_metric_result import TestSuiteRunExecutionMetricResult
+from .test_suite_run_execution_output import TestSuiteRunExecutionOutput
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class PaginatedSlimDocumentList(pydantic.BaseModel):
-    count: typing.Optional[int]
-    next: typing.Optional[str]
-    previous: typing.Optional[str]
-    results: typing.Optional[typing.List[SlimDocument]]
+class TestSuiteRunExecution(pydantic_v1.BaseModel):
+    id: str
+    test_case_id: str
+    outputs: typing.List[TestSuiteRunExecutionOutput]
+    metric_results: typing.List[TestSuiteRunExecutionMetricResult]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/paginated_slim_workflow_deployment_list.py` & `vellum_ai-0.5.0/src/vellum/types/prompt_execution_meta.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .slim_workflow_deployment import SlimWorkflowDeployment
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class PaginatedSlimWorkflowDeploymentList(pydantic.BaseModel):
-    count: typing.Optional[int]
-    next: typing.Optional[str]
-    previous: typing.Optional[str]
-    results: typing.Optional[typing.List[SlimWorkflowDeployment]]
+from ..core.pydantic_utilities import pydantic_v1
+from .finish_reason_enum import FinishReasonEnum
+from .ml_model_usage import MlModelUsage
+
+
+class PromptExecutionMeta(pydantic_v1.BaseModel):
+    """
+    The subset of the metadata tracked by Vellum during prompt execution that the request opted into with `expand_meta`.
+    """
+
+    usage: typing.Optional[MlModelUsage] = None
+    model_name: typing.Optional[str] = None
+    latency: typing.Optional[int] = None
+    deployment_release_tag: typing.Optional[str] = None
+    prompt_version_id: typing.Optional[str] = None
+    finish_reason: typing.Optional[FinishReasonEnum] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/prompt_deployment_expand_meta_request_request.py` & `vellum_ai-0.5.0/src/vellum/types/prompt_deployment_expand_meta_request_request.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,53 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class PromptDeploymentExpandMetaRequestRequest(pydantic.BaseModel):
-    model_name: typing.Optional[bool] = pydantic.Field(
-        description="If enabled, the response will include the model identifier representing the ML Model invoked by the Prompt Deployment."
-    )
-    latency: typing.Optional[bool] = pydantic.Field(
-        description="If enabled, the response will include the time in nanoseconds it took to execute the Prompt Deployment."
-    )
-    deployment_release_tag: typing.Optional[bool] = pydantic.Field(
-        description="If enabled, the response will include the release tag of the Prompt Deployment."
-    )
-    prompt_version_id: typing.Optional[bool] = pydantic.Field(
-        description="If enabled, the response will include the ID of the Prompt Version backing the deployment."
-    )
-    finish_reason: typing.Optional[bool] = pydantic.Field(
-        description="If enabled, the response will include the reason provided by the model for why the execution finished."
-    )
+
+class PromptDeploymentExpandMetaRequestRequest(pydantic_v1.BaseModel):
+    model_name: typing.Optional[bool] = pydantic_v1.Field(default=None)
+    """
+    If enabled, the response will include the model identifier representing the ML Model invoked by the Prompt Deployment.
+    """
+
+    latency: typing.Optional[bool] = pydantic_v1.Field(default=None)
+    """
+    If enabled, the response will include the time in nanoseconds it took to execute the Prompt Deployment.
+    """
+
+    deployment_release_tag: typing.Optional[bool] = pydantic_v1.Field(default=None)
+    """
+    If enabled, the response will include the release tag of the Prompt Deployment.
+    """
+
+    prompt_version_id: typing.Optional[bool] = pydantic_v1.Field(default=None)
+    """
+    If enabled, the response will include the ID of the Prompt Version backing the deployment.
+    """
+
+    finish_reason: typing.Optional[bool] = pydantic_v1.Field(default=None)
+    """
+    If enabled, the response will include the reason provided by the model for why the execution finished.
+    """
+
+    usage: typing.Optional[bool] = pydantic_v1.Field(default=None)
+    """
+    If enabled, the response will include model host usage tracking. This may increase latency for some model hosts.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/prompt_deployment_input_request.py` & `vellum_ai-0.5.0/src/vellum/types/prompt_deployment_input_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from __future__ import annotations
 
 import typing
 
-import typing_extensions
-
 from .chat_history_input_request import ChatHistoryInputRequest
 from .json_input_request import JsonInputRequest
 from .string_input_request import StringInputRequest
 
 
 class PromptDeploymentInputRequest_String(StringInputRequest):
-    type: typing_extensions.Literal["STRING"]
+    type: typing.Literal["STRING"] = "STRING"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class PromptDeploymentInputRequest_Json(JsonInputRequest):
-    type: typing_extensions.Literal["JSON"]
+    type: typing.Literal["JSON"] = "JSON"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class PromptDeploymentInputRequest_ChatHistory(ChatHistoryInputRequest):
-    type: typing_extensions.Literal["CHAT_HISTORY"]
+    type: typing.Literal["CHAT_HISTORY"] = "CHAT_HISTORY"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 PromptDeploymentInputRequest = typing.Union[
     PromptDeploymentInputRequest_String, PromptDeploymentInputRequest_Json, PromptDeploymentInputRequest_ChatHistory
 ]
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/prompt_execution_meta.py` & `vellum_ai-0.5.0/src/vellum/types/rejected_prompt_execution_meta.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .finish_reason_enum import FinishReasonEnum
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class PromptExecutionMeta(pydantic.BaseModel):
+class RejectedPromptExecutionMeta(pydantic_v1.BaseModel):
     """
     The subset of the metadata tracked by Vellum during prompt execution that the request opted into with `expand_meta`.
     """
 
-    model_name: typing.Optional[str]
-    latency: typing.Optional[int]
-    deployment_release_tag: typing.Optional[str]
-    prompt_version_id: typing.Optional[str]
-    finish_reason: typing.Optional[FinishReasonEnum]
+    latency: typing.Optional[int] = None
+    finish_reason: typing.Optional[FinishReasonEnum] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/prompt_node_result.py` & `vellum_ai-0.5.0/src/vellum/types/terminal_node_number_result.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .prompt_node_result_data import PromptNodeResultData
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class PromptNodeResult(pydantic.BaseModel):
+class TerminalNodeNumberResult(pydantic_v1.BaseModel):
+    id: typing.Optional[str] = None
+    name: str = pydantic_v1.Field()
     """
-    A Node Result Event emitted from a Prompt Node.
+    The unique name given to the terminal node that produced this output.
     """
 
-    data: PromptNodeResultData
+    value: typing.Optional[float] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/prompt_node_result_data.py` & `vellum_ai-0.5.0/src/vellum/types/templating_node_number_result.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class PromptNodeResultData(pydantic.BaseModel):
-    output_id: str
-    array_output_id: typing.Optional[str]
-    text: typing.Optional[str]
-    delta: typing.Optional[str]
+class TemplatingNodeNumberResult(pydantic_v1.BaseModel):
+    id: str
+    value: typing.Optional[float] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/prompt_output.py` & `vellum_ai-0.5.0/src/vellum/types/prompt_output.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from __future__ import annotations
 
 import typing
 
-import typing_extensions
-
 from .error_variable_value import ErrorVariableValue
 from .function_call_variable_value import FunctionCallVariableValue
 from .json_variable_value import JsonVariableValue
 from .string_variable_value import StringVariableValue
 
 
 class PromptOutput_String(StringVariableValue):
-    type: typing_extensions.Literal["STRING"]
+    type: typing.Literal["STRING"] = "STRING"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class PromptOutput_Json(JsonVariableValue):
-    type: typing_extensions.Literal["JSON"]
+    type: typing.Literal["JSON"] = "JSON"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class PromptOutput_Error(ErrorVariableValue):
-    type: typing_extensions.Literal["ERROR"]
+    type: typing.Literal["ERROR"] = "ERROR"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class PromptOutput_FunctionCall(FunctionCallVariableValue):
-    type: typing_extensions.Literal["FUNCTION_CALL"]
+    type: typing.Literal["FUNCTION_CALL"] = "FUNCTION_CALL"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 PromptOutput = typing.Union[PromptOutput_String, PromptOutput_Json, PromptOutput_Error, PromptOutput_FunctionCall]
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/prompt_template_block.py` & `vellum_ai-0.5.0/src/vellum/types/generate_stream_result_data.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from __future__ import annotations
-
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .block_type_enum import BlockTypeEnum
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
+from ..core.pydantic_utilities import pydantic_v1
+from .enriched_normalized_completion import EnrichedNormalizedCompletion
 
 
-class PromptTemplateBlock(pydantic.BaseModel):
-    id: str
-    block_type: BlockTypeEnum
-    properties: PromptTemplateBlockProperties
+class GenerateStreamResultData(pydantic_v1.BaseModel):
+    completion_index: int
+    completion: EnrichedNormalizedCompletion
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
-
-
-from .prompt_template_block_properties import PromptTemplateBlockProperties  # noqa: E402
-
-PromptTemplateBlock.update_forward_refs()
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/prompt_template_block_data.py` & `vellum_ai-0.5.0/src/vellum/types/node_input_compiled_array_value.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .prompt_template_block import PromptTemplateBlock
+from ..core.pydantic_utilities import pydantic_v1
+from .array_variable_value_item import ArrayVariableValueItem
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class PromptTemplateBlockData(pydantic.BaseModel):
-    version: int
-    blocks: typing.List[PromptTemplateBlock]
+class NodeInputCompiledArrayValue(pydantic_v1.BaseModel):
+    node_input_id: str
+    key: str
+    value: typing.Optional[typing.List[ArrayVariableValueItem]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/prompt_template_block_data_request.py` & `vellum_ai-0.5.0/src/vellum/types/named_test_case_chat_history_variable_value_request.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .prompt_template_block_request import PromptTemplateBlockRequest
+from ..core.pydantic_utilities import pydantic_v1
+from .chat_message_request import ChatMessageRequest
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class NamedTestCaseChatHistoryVariableValueRequest(pydantic_v1.BaseModel):
+    """
+    Named Test Case value that is of type CHAT_HISTORY
+    """
 
-class PromptTemplateBlockDataRequest(pydantic.BaseModel):
-    version: int
-    blocks: typing.List[PromptTemplateBlockRequest]
+    value: typing.Optional[typing.List[ChatMessageRequest]] = None
+    name: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/prompt_template_block_properties.py` & `vellum_ai-0.5.0/src/vellum/types/slim_workflow_deployment.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,66 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from __future__ import annotations
-
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .chat_message_role import ChatMessageRole
-from .vellum_variable_type import VellumVariableType
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class PromptTemplateBlockProperties(pydantic.BaseModel):
-    chat_role: typing.Optional[ChatMessageRole]
-    chat_message_unterminated: typing.Optional[bool]
-    template: typing.Optional[str]
-    template_type: typing.Optional[VellumVariableType]
-    function_name: typing.Optional[str]
-    function_description: typing.Optional[str]
-    function_parameters: typing.Optional[typing.Dict[str, typing.Any]]
-    function_forced: typing.Optional[bool]
-    blocks: typing.Optional[typing.List[PromptTemplateBlock]]
+from ..core.pydantic_utilities import pydantic_v1
+from .entity_status import EntityStatus
+from .environment_enum import EnvironmentEnum
+from .vellum_variable import VellumVariable
+
+
+class SlimWorkflowDeployment(pydantic_v1.BaseModel):
+    id: str
+    name: str = pydantic_v1.Field()
+    """
+    A name that uniquely identifies this workflow deployment within its workspace
+    """
+
+    label: str = pydantic_v1.Field()
+    """
+    A human-readable label for the workflow deployment
+    """
+
+    status: typing.Optional[EntityStatus] = pydantic_v1.Field(default=None)
+    """
+    The current status of the workflow deployment
+    
+    - `ACTIVE` - Active
+    - `ARCHIVED` - Archived
+    """
+
+    environment: typing.Optional[EnvironmentEnum] = pydantic_v1.Field(default=None)
+    """
+    The environment this workflow deployment is used in
+    
+    - `DEVELOPMENT` - Development
+    - `STAGING` - Staging
+    - `PRODUCTION` - Production
+    """
+
+    created: dt.datetime
+    last_deployed_on: dt.datetime
+    input_variables: typing.List[VellumVariable] = pydantic_v1.Field()
+    """
+    The input variables this Workflow Deployment expects to receive values for when it is executed.
+    """
+
+    output_variables: typing.List[VellumVariable] = pydantic_v1.Field()
+    """
+    The output variables this Workflow Deployment will produce when it is executed.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
-
-
-from .prompt_template_block import PromptTemplateBlock  # noqa: E402
-
-PromptTemplateBlockProperties.update_forward_refs()
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/prompt_template_block_properties_request.py` & `vellum_ai-0.5.0/src/vellum/types/generate_request.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,39 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from __future__ import annotations
-
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .chat_message_role import ChatMessageRole
-from .vellum_variable_type import VellumVariableType
+from ..core.pydantic_utilities import pydantic_v1
+from .chat_message_request import ChatMessageRequest
+
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class PromptTemplateBlockPropertiesRequest(pydantic.BaseModel):
-    chat_role: typing.Optional[ChatMessageRole]
-    chat_message_unterminated: typing.Optional[bool]
-    template: typing.Optional[str]
-    template_type: typing.Optional[VellumVariableType]
-    function_name: typing.Optional[str]
-    function_description: typing.Optional[str]
-    function_parameters: typing.Optional[typing.Dict[str, typing.Any]]
-    function_forced: typing.Optional[bool]
-    blocks: typing.Optional[typing.List[PromptTemplateBlockRequest]]
+class GenerateRequest(pydantic_v1.BaseModel):
+    input_values: typing.Dict[str, typing.Any] = pydantic_v1.Field()
+    """
+    Key/value pairs for each template variable defined in the deployment's prompt.
+    """
+
+    chat_history: typing.Optional[typing.List[ChatMessageRequest]] = pydantic_v1.Field(default=None)
+    """
+    Optionally provide a list of chat messages that'll be used in place of the special chat_history variable, if included in the prompt.
+    """
+
+    external_ids: typing.Optional[typing.List[str]] = pydantic_v1.Field(default=None)
+    """
+    Optionally include a unique identifier for each generation, as represented outside of Vellum. Note that this should generally be a list of length one.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
-
-
-from .prompt_template_block_request import PromptTemplateBlockRequest  # noqa: E402
-
-PromptTemplateBlockPropertiesRequest.update_forward_refs()
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/prompt_template_block_request.py` & `vellum_ai-0.5.0/src/vellum/types/fulfilled_function_call.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from __future__ import annotations
-
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .block_type_enum import BlockTypeEnum
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class FulfilledFunctionCall(pydantic_v1.BaseModel):
+    """
+    The final resolved function call value.
+    """
 
-class PromptTemplateBlockRequest(pydantic.BaseModel):
-    id: str
-    block_type: BlockTypeEnum
-    properties: PromptTemplateBlockPropertiesRequest
+    arguments: typing.Dict[str, typing.Any]
+    id: typing.Optional[str] = None
+    name: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
-
-
-from .prompt_template_block_properties_request import PromptTemplateBlockPropertiesRequest  # noqa: E402
-
-PromptTemplateBlockRequest.update_forward_refs()
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/raw_prompt_execution_overrides_request.py` & `vellum_ai-0.5.0/src/vellum/types/paginated_slim_deployment_read_list.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from .slim_deployment_read import SlimDeploymentRead
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class RawPromptExecutionOverridesRequest(pydantic.BaseModel):
-    body: typing.Optional[typing.Dict[str, typing.Any]]
-    headers: typing.Optional[typing.Dict[str, typing.Optional[str]]] = pydantic.Field(
-        description="The raw headers to send to the model host."
-    )
-    url: typing.Optional[str] = pydantic.Field(description="The raw URL to send to the model host.")
+class PaginatedSlimDeploymentReadList(pydantic_v1.BaseModel):
+    count: typing.Optional[int] = None
+    next: typing.Optional[str] = None
+    previous: typing.Optional[str] = None
+    results: typing.Optional[typing.List[SlimDeploymentRead]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/register_prompt_error_response.py` & `vellum_ai-0.5.0/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_data.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class RegisterPromptErrorResponse(pydantic.BaseModel):
-    detail: str = pydantic.Field(description="Details about why the request failed.")
+class TestSuiteRunDeploymentReleaseTagExecConfigData(pydantic_v1.BaseModel):
+    deployment_id: str = pydantic_v1.Field()
+    """
+    The ID of the Prompt Deployment to run the Test Suite against.
+    """
+
+    tag: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    A tag identifying which release of the Prompt Deployment to run the Test Suite against. Useful for testing past versions of the Prompt Deployment
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/register_prompt_model_parameters_request.py` & `vellum_ai-0.5.0/src/vellum/types/node_input_compiled_number_value.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class RegisterPromptModelParametersRequest(pydantic.BaseModel):
-    temperature: float
-    max_tokens: int
-    stop: typing.Optional[typing.List[str]]
-    top_p: float
-    top_k: typing.Optional[int]
-    frequency_penalty: float
-    presence_penalty: float
-    logit_bias: typing.Optional[typing.Dict[str, typing.Optional[float]]]
-    custom_parameters: typing.Optional[typing.Dict[str, typing.Any]]
+
+class NodeInputCompiledNumberValue(pydantic_v1.BaseModel):
+    node_input_id: str
+    key: str
+    value: typing.Optional[float] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/register_prompt_prompt.py` & `vellum_ai-0.5.0/src/vellum/types/test_suite_run_deployment_release_tag_exec_config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from .test_suite_run_deployment_release_tag_exec_config_data import TestSuiteRunDeploymentReleaseTagExecConfigData
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class RegisterPromptPrompt(pydantic.BaseModel):
-    id: str = pydantic.Field(description="The ID of the generated prompt.")
-    label: str = pydantic.Field(description="A human-friendly label for the generated prompt.")
+class TestSuiteRunDeploymentReleaseTagExecConfig(pydantic_v1.BaseModel):
+    """
+    Execution configuration for running a Test Suite against a Prompt Deployment
+    """
+
+    data: TestSuiteRunDeploymentReleaseTagExecConfigData
+    test_case_ids: typing.Optional[typing.List[str]] = pydantic_v1.Field(default=None)
+    """
+    Optionally specify a subset of test case ids to run. If not provided, all test cases within the test suite will be run by default.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/register_prompt_prompt_info_request.py` & `vellum_ai-0.5.0/src/vellum/types/workflow_result_event_output_data_function_call.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .prompt_template_block_data_request import PromptTemplateBlockDataRequest
-from .registered_prompt_input_variable_request import RegisteredPromptInputVariableRequest
+from ..core.pydantic_utilities import pydantic_v1
+from .function_call import FunctionCall
+from .workflow_node_result_event_state import WorkflowNodeResultEventState
+
+
+class WorkflowResultEventOutputDataFunctionCall(pydantic_v1.BaseModel):
+    """
+    A Function Call output returned from a Workflow execution.
+    """
+
+    id: typing.Optional[str] = None
+    name: str
+    state: WorkflowNodeResultEventState
+    node_id: str
+    delta: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The newly output string value. Only relevant for string outputs with a state of STREAMING.
+    """
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class RegisterPromptPromptInfoRequest(pydantic.BaseModel):
-    prompt_block_data: PromptTemplateBlockDataRequest
-    input_variables: typing.List[RegisteredPromptInputVariableRequest] = pydantic.Field(
-        description="The input variables specified in the prompt template."
-    )
+    value: typing.Optional[FunctionCall] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/registered_prompt_deployment.py` & `vellum_ai-0.5.0/src/vellum/types/workflow_result_event_output_data_search_results.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from .search_result import SearchResult
+from .workflow_node_result_event_state import WorkflowNodeResultEventState
+
+
+class WorkflowResultEventOutputDataSearchResults(pydantic_v1.BaseModel):
+    """
+    A Search Results output streamed from a Workflow execution.
+    """
+
+    id: typing.Optional[str] = None
+    name: str
+    state: WorkflowNodeResultEventState
+    node_id: str
+    delta: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The newly output string value. Only relevant for string outputs with a state of STREAMING.
+    """
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class RegisteredPromptDeployment(pydantic.BaseModel):
-    id: str = pydantic.Field(description="The ID of the generated deployment.")
-    name: str = pydantic.Field(description="A uniquely-identifying name for generated deployment.")
-    label: str = pydantic.Field(description="A human-friendly label for the generated deployment.")
+    value: typing.Optional[typing.List[SearchResult]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/registered_prompt_input_variable_request.py` & `vellum_ai-0.5.0/src/vellum/types/rejected_workflow_node_result_event.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .vellum_variable_type import VellumVariableType
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class RegisteredPromptInputVariableRequest(pydantic.BaseModel):
-    key: str
-    id: typing.Optional[str]
-    type: typing.Optional[VellumVariableType]
+from ..core.pydantic_utilities import pydantic_v1
+from .workflow_event_error import WorkflowEventError
+from .workflow_node_result_data import WorkflowNodeResultData
+
+
+class RejectedWorkflowNodeResultEvent(pydantic_v1.BaseModel):
+    """
+    An event that indicates that the node has rejected its execution.
+    """
+
+    id: str
+    node_id: str
+    node_result_id: str
+    ts: typing.Optional[dt.datetime] = None
+    data: typing.Optional[WorkflowNodeResultData] = None
+    source_execution_id: typing.Optional[str] = None
+    error: WorkflowEventError
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/registered_prompt_sandbox_snapshot.py` & `vellum_ai-0.5.0/src/vellum/types/search_node_result.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from .search_node_result_data import SearchNodeResultData
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class SearchNodeResult(pydantic_v1.BaseModel):
+    """
+    A Node Result Event emitted from a Search Node.
+    """
 
-class RegisteredPromptSandboxSnapshot(pydantic.BaseModel):
-    id: str = pydantic.Field(description="The ID of the generated sandbox snapshot.")
+    data: SearchNodeResultData
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/rejected_execute_prompt_event.py` & `vellum_ai-0.5.0/src/vellum/types/rejected_execute_prompt_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .rejected_prompt_execution_meta import RejectedPromptExecutionMeta
+from ..core.pydantic_utilities import pydantic_v1
+from .prompt_execution_meta import PromptExecutionMeta
 from .vellum_error import VellumError
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class RejectedExecutePromptResponse(pydantic_v1.BaseModel):
+    """
+    The unsuccessful response from the model containing an error of what went wrong.
+    """
+
+    meta: typing.Optional[PromptExecutionMeta] = None
+    raw: typing.Optional[typing.Dict[str, typing.Any]] = pydantic_v1.Field(default=None)
+    """
+    The subset of the raw response from the model that the request opted into with `expand_raw`.
+    """
 
-class RejectedExecutePromptEvent(pydantic.BaseModel):
+    execution_id: str = pydantic_v1.Field()
     """
-    The final data returned indicating an error occurred during the stream.
+    The ID of the execution.
     """
 
     error: VellumError
-    execution_id: str
-    meta: typing.Optional[RejectedPromptExecutionMeta]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/rejected_execute_prompt_response.py` & `vellum_ai-0.5.0/src/vellum/types/fulfilled_execute_prompt_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .prompt_execution_meta import PromptExecutionMeta
-from .vellum_error import VellumError
+from .prompt_output import PromptOutput
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class FulfilledExecutePromptResponse(pydantic_v1.BaseModel):
+    """
+    The successful response from the model containing all of the resolved values generated by the prompt.
+    """
+
+    meta: typing.Optional[PromptExecutionMeta] = None
+    raw: typing.Optional[typing.Dict[str, typing.Any]] = pydantic_v1.Field(default=None)
+    """
+    The subset of the raw response from the model that the request opted into with `expand_raw`.
+    """
 
-class RejectedExecutePromptResponse(pydantic.BaseModel):
+    execution_id: str = pydantic_v1.Field()
     """
-    The unsuccessful response from the model containing an error of what went wrong.
+    The ID of the execution.
     """
 
-    meta: typing.Optional[PromptExecutionMeta]
-    raw: typing.Optional[typing.Dict[str, typing.Any]] = pydantic.Field(
-        description="The subset of the raw response from the model that the request opted into with `expand_raw`."
-    )
-    execution_id: str = pydantic.Field(description="The ID of the execution.")
-    error: VellumError
+    outputs: typing.List[PromptOutput]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/rejected_execute_workflow_workflow_result_event.py` & `vellum_ai-0.5.0/src/vellum/types/rejected_execute_workflow_workflow_result_event.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .workflow_event_error import WorkflowEventError
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class RejectedExecuteWorkflowWorkflowResultEvent(pydantic.BaseModel):
+class RejectedExecuteWorkflowWorkflowResultEvent(pydantic_v1.BaseModel):
     """
     The unsuccessful response from the Workflow execution containing an error specifying what went wrong.
     """
 
     id: str
     ts: dt.datetime
     error: WorkflowEventError
@@ -28,8 +24,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/rejected_function_call.py` & `vellum_ai-0.5.0/src/vellum/types/execution_error_vellum_value.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .vellum_error import VellumError
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class RejectedFunctionCall(pydantic.BaseModel):
+class ExecutionErrorVellumValue(pydantic_v1.BaseModel):
+    id: str = pydantic_v1.Field()
     """
-    Returned if the function call failed to parse for some reason.
+    The variable's uniquely identifying internal id.
     """
 
-    error: VellumError
-    id: typing.Optional[str]
     name: str
+    value: typing.Optional[VellumError] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/rejected_prompt_execution_meta.py` & `vellum_ai-0.5.0/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_request.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .finish_reason_enum import FinishReasonEnum
+from ..core.pydantic_utilities import pydantic_v1
+from .test_suite_run_workflow_release_tag_exec_config_data_request import (
+    TestSuiteRunWorkflowReleaseTagExecConfigDataRequest,
+)
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class RejectedPromptExecutionMeta(pydantic.BaseModel):
+class TestSuiteRunWorkflowReleaseTagExecConfigRequest(pydantic_v1.BaseModel):
     """
-    The subset of the metadata tracked by Vellum during prompt execution that the request opted into with `expand_meta`.
+    Execution configuration for running a Test Suite against a Workflow Deployment
     """
 
-    latency: typing.Optional[int]
-    finish_reason: typing.Optional[FinishReasonEnum]
+    data: TestSuiteRunWorkflowReleaseTagExecConfigDataRequest
+    test_case_ids: typing.Optional[typing.List[str]] = pydantic_v1.Field(default=None)
+    """
+    Optionally specify a subset of test case ids to run. If not provided, all test cases within the test suite will be run by default.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/rejected_workflow_node_result_event.py` & `vellum_ai-0.5.0/src/vellum/types/prompt_node_result.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .workflow_event_error import WorkflowEventError
-from .workflow_node_result_data import WorkflowNodeResultData
+from ..core.pydantic_utilities import pydantic_v1
+from .prompt_node_result_data import PromptNodeResultData
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class RejectedWorkflowNodeResultEvent(pydantic.BaseModel):
+class PromptNodeResult(pydantic_v1.BaseModel):
     """
-    An event that indicates that the node has rejected its execution.
+    A Node Result Event emitted from a Prompt Node.
     """
 
-    id: str
-    node_id: str
-    node_result_id: str
-    ts: typing.Optional[dt.datetime]
-    data: typing.Optional[WorkflowNodeResultData]
-    error: WorkflowEventError
+    data: PromptNodeResultData
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/sandbox_scenario.py` & `vellum_ai-0.5.0/src/vellum/types/templating_node_array_result.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .scenario_input import ScenarioInput
+from ..core.pydantic_utilities import pydantic_v1
+from .array_variable_value_item import ArrayVariableValueItem
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class SandboxScenario(pydantic.BaseModel):
-    label: typing.Optional[str]
-    inputs: typing.List[ScenarioInput] = pydantic.Field(description="The inputs for the scenario")
-    id: str = pydantic.Field(description="The id of the scenario")
+class TemplatingNodeArrayResult(pydantic_v1.BaseModel):
+    id: str
+    value: typing.Optional[typing.List[ArrayVariableValueItem]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/scenario_input.py` & `vellum_ai-0.5.0/src/vellum/types/templating_node_string_result.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .chat_message import ChatMessage
-from .scenario_input_type_enum import ScenarioInputTypeEnum
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ScenarioInput(pydantic.BaseModel):
-    key: str
-    type: typing.Optional[ScenarioInputTypeEnum]
-    value: typing.Optional[str]
-    chat_history: typing.Optional[typing.List[ChatMessage]]
+class TemplatingNodeStringResult(pydantic_v1.BaseModel):
+    id: str
+    value: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/scenario_input_request.py` & `vellum_ai-0.5.0/src/vellum/types/search_result_merging_request.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .chat_message_request import ChatMessageRequest
-from .scenario_input_type_enum import ScenarioInputTypeEnum
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ScenarioInputRequest(pydantic.BaseModel):
-    key: str
-    type: typing.Optional[ScenarioInputTypeEnum]
-    value: typing.Optional[str]
-    chat_history: typing.Optional[typing.List[ChatMessageRequest]]
+class SearchResultMergingRequest(pydantic_v1.BaseModel):
+    enabled: typing.Optional[bool] = pydantic_v1.Field(default=None)
+    """
+    Whether to enable merging results
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/search_error_response.py` & `vellum_ai-0.5.0/src/vellum/types/terminal_node_search_results_result.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from .search_result import SearchResult
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class TerminalNodeSearchResultsResult(pydantic_v1.BaseModel):
+    id: typing.Optional[str] = None
+    name: str = pydantic_v1.Field()
+    """
+    The unique name given to the terminal node that produced this output.
+    """
 
-class SearchErrorResponse(pydantic.BaseModel):
-    detail: str = pydantic.Field(description="Details about why the request failed.")
+    value: typing.Optional[typing.List[SearchResult]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/search_filters_request.py` & `vellum_ai-0.5.0/src/vellum/types/external_test_case_execution_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .metadata_filter_config_request import MetadataFilterConfigRequest
+from ..core.pydantic_utilities import pydantic_v1
+from .named_test_case_variable_value_request import NamedTestCaseVariableValueRequest
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class ExternalTestCaseExecutionRequest(pydantic_v1.BaseModel):
+    outputs: typing.List[NamedTestCaseVariableValueRequest] = pydantic_v1.Field()
+    """
+    The output values of a callable that was executed against a Test Case outside of Vellum
+    """
 
-class SearchFiltersRequest(pydantic.BaseModel):
-    external_ids: typing.Optional[typing.List[str]] = pydantic.Field(
-        description="The document external IDs to filter by"
-    )
-    metadata: typing.Optional[MetadataFilterConfigRequest] = pydantic.Field(
-        description="The metadata filters to apply to the search"
-    )
+    test_case_id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/search_node_result.py` & `vellum_ai-0.5.0/src/vellum/types/subworkflow_node_result.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .search_node_result_data import SearchNodeResultData
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class SearchNodeResult(pydantic.BaseModel):
+class SubworkflowNodeResult(pydantic_v1.BaseModel):
     """
-    A Node Result Event emitted from a Search Node.
+    A Node Result Event emitted from a Subworkflow Node.
     """
 
-    data: SearchNodeResultData
-
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/search_node_result_data.py` & `vellum_ai-0.5.0/src/vellum/types/search_results_variable_value.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .search_result import SearchResult
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class SearchNodeResultData(pydantic.BaseModel):
-    results_output_id: str
-    results: typing.List[SearchResult] = pydantic.Field(
-        description="The results of the search. Each result represents a chunk that matches the search query."
-    )
-    text_output_id: str
-    text: typing.Optional[str]
+class SearchResultsVariableValue(pydantic_v1.BaseModel):
+    value: typing.Optional[typing.List[SearchResult]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/search_request_options_request.py` & `vellum_ai-0.5.0/src/vellum/types/search_request_options_request.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,46 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .search_filters_request import SearchFiltersRequest
 from .search_result_merging_request import SearchResultMergingRequest
 from .search_weights_request import SearchWeightsRequest
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class SearchRequestOptionsRequest(pydantic.BaseModel):
-    limit: typing.Optional[int] = pydantic.Field(description="The maximum number of results to return.")
-    weights: typing.Optional[SearchWeightsRequest] = pydantic.Field(
-        description="The weights to use for the search. Must add up to 1.0."
-    )
-    result_merging: typing.Optional[SearchResultMergingRequest] = pydantic.Field(
-        description="The configuration for merging results."
-    )
-    filters: typing.Optional[SearchFiltersRequest] = pydantic.Field(description="The filters to apply to the search.")
+class SearchRequestOptionsRequest(pydantic_v1.BaseModel):
+    limit: typing.Optional[int] = pydantic_v1.Field(default=None)
+    """
+    The maximum number of results to return.
+    """
+
+    weights: typing.Optional[SearchWeightsRequest] = pydantic_v1.Field(default=None)
+    """
+    The weights to use for the search. Must add up to 1.0.
+    """
+
+    result_merging: typing.Optional[SearchResultMergingRequest] = pydantic_v1.Field(default=None)
+    """
+    The configuration for merging results.
+    """
+
+    filters: typing.Optional[SearchFiltersRequest] = pydantic_v1.Field(default=None)
+    """
+    The filters to apply to the search.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/search_response.py` & `vellum_ai-0.5.0/src/vellum/types/search_error_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .search_result import SearchResult
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class SearchResponse(pydantic.BaseModel):
-    results: typing.List[SearchResult] = pydantic.Field(
-        description="The results of the search. Each result represents a chunk that matches the search query."
-    )
+class SearchErrorResponse(pydantic_v1.BaseModel):
+    detail: str = pydantic_v1.Field()
+    """
+    Details about why the request failed.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/search_result.py` & `vellum_ai-0.5.0/src/vellum/types/search_result.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .search_result_document import SearchResultDocument
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class SearchResult(pydantic_v1.BaseModel):
+    text: str = pydantic_v1.Field()
+    """
+    The text of the chunk that matched the search query.
+    """
+
+    score: float = pydantic_v1.Field()
+    """
+    A score representing how well the chunk matches the search query.
+    """
 
-class SearchResult(pydantic.BaseModel):
-    text: str = pydantic.Field(description="The text of the chunk that matched the search query.")
-    score: float = pydantic.Field(description="A score representing how well the chunk matches the search query.")
     keywords: typing.List[str]
-    document: SearchResultDocument = pydantic.Field(
-        description="The document that contains the chunk that matched the search query."
-    )
+    document: SearchResultDocument = pydantic_v1.Field()
+    """
+    The document that contains the chunk that matched the search query.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/search_result_document.py` & `vellum_ai-0.5.0/src/vellum/types/search_result_document_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class SearchResultDocument(pydantic.BaseModel):
-    id: str = pydantic.Field(description="The ID of the document.")
-    label: str = pydantic.Field(description="The human-readable name for the document.")
-    external_id: typing.Optional[str] = pydantic.Field(
-        description="The unique ID of the document as represented in an external system and specified when it was originally uploaded."
-    )
-    metadata: typing.Optional[typing.Dict[str, typing.Any]] = pydantic.Field(
-        description="A previously supplied JSON object containing metadata that can be filtered on when searching."
-    )
+class SearchResultDocumentRequest(pydantic_v1.BaseModel):
+    label: str = pydantic_v1.Field()
+    """
+    The human-readable name for the document.
+    """
+
+    external_id: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The unique ID of the document as represented in an external system and specified when it was originally uploaded.
+    """
+
+    metadata: typing.Optional[typing.Dict[str, typing.Any]] = pydantic_v1.Field(default=None)
+    """
+    A previously supplied JSON object containing metadata that can be filtered on when searching.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/search_result_document_request.py` & `vellum_ai-0.5.0/src/vellum/types/execute_workflow_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from .execute_workflow_workflow_result_event import ExecuteWorkflowWorkflowResultEvent
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class SearchResultDocumentRequest(pydantic.BaseModel):
-    label: str = pydantic.Field(description="The human-readable name for the document.")
-    external_id: typing.Optional[str] = pydantic.Field(
-        description="The unique ID of the document as represented in an external system and specified when it was originally uploaded."
-    )
-    metadata: typing.Optional[typing.Dict[str, typing.Any]] = pydantic.Field(
-        description="A previously supplied JSON object containing metadata that can be filtered on when searching."
-    )
+class ExecuteWorkflowResponse(pydantic_v1.BaseModel):
+    execution_id: str
+    run_id: typing.Optional[str] = None
+    external_id: typing.Optional[str] = None
+    data: ExecuteWorkflowWorkflowResultEvent
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/search_result_merging_request.py` & `vellum_ai-0.5.0/src/vellum/types/upload_document_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class SearchResultMergingRequest(pydantic.BaseModel):
-    enabled: typing.Optional[bool] = pydantic.Field(description="Whether to enable merging results")
+class UploadDocumentResponse(pydantic_v1.BaseModel):
+    document_id: str = pydantic_v1.Field()
+    """
+    The ID of the newly created document.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/search_result_request.py` & `vellum_ai-0.5.0/src/vellum/types/search_node_result_data.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .search_result_document_request import SearchResultDocumentRequest
+from ..core.pydantic_utilities import pydantic_v1
+from .search_result import SearchResult
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class SearchNodeResultData(pydantic_v1.BaseModel):
+    results_output_id: str
+    results: typing.List[SearchResult] = pydantic_v1.Field()
+    """
+    The results of the search. Each result represents a chunk that matches the search query.
+    """
 
-class SearchResultRequest(pydantic.BaseModel):
-    text: str = pydantic.Field(description="The text of the chunk that matched the search query.")
-    score: float = pydantic.Field(description="A score representing how well the chunk matches the search query.")
-    keywords: typing.List[str]
-    document: SearchResultDocumentRequest = pydantic.Field(
-        description="The document that contains the chunk that matched the search query."
-    )
+    text_output_id: str
+    text: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/search_results_variable_value.py` & `vellum_ai-0.5.0/src/vellum/types/node_output_compiled_search_results_value.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .search_result import SearchResult
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class SearchResultsVariableValue(pydantic.BaseModel):
-    value: typing.Optional[typing.List[SearchResult]]
+class NodeOutputCompiledSearchResultsValue(pydantic_v1.BaseModel):
+    node_output_id: str
+    value: typing.Optional[typing.List[SearchResult]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/search_weights_request.py` & `vellum_ai-0.5.0/src/vellum/types/workflow_result_event_output_data_array.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from .array_variable_value_item import ArrayVariableValueItem
+from .workflow_node_result_event_state import WorkflowNodeResultEventState
+
+
+class WorkflowResultEventOutputDataArray(pydantic_v1.BaseModel):
+    """
+    An Array output returned from a Workflow execution.
+    """
+
+    id: typing.Optional[str] = None
+    name: str
+    state: WorkflowNodeResultEventState
+    node_id: str
+    delta: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The newly output string value. Only relevant for string outputs with a state of STREAMING.
+    """
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class SearchWeightsRequest(pydantic.BaseModel):
-    semantic_similarity: typing.Optional[float] = pydantic.Field(
-        description="The relative weight to give to semantic similarity"
-    )
-    keywords: typing.Optional[float] = pydantic.Field(description="The relative weight to give to keywords")
+    value: typing.Optional[typing.List[ArrayVariableValueItem]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/slim_deployment_read.py` & `vellum_ai-0.5.0/src/vellum/types/workflow_deployment_read.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,66 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .entity_status import EntityStatus
 from .environment_enum import EnvironmentEnum
 from .vellum_variable import VellumVariable
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class SlimDeploymentRead(pydantic.BaseModel):
+class WorkflowDeploymentRead(pydantic_v1.BaseModel):
     id: str
+    name: str = pydantic_v1.Field()
+    """
+    A name that uniquely identifies this workflow deployment within its workspace
+    """
+
+    label: str = pydantic_v1.Field()
+    """
+    A human-readable label for the workflow deployment
+    """
+
+    status: typing.Optional[EntityStatus] = pydantic_v1.Field(default=None)
+    """
+    The current status of the workflow deployment
+    
+    - `ACTIVE` - Active
+    - `ARCHIVED` - Archived
+    """
+
+    environment: typing.Optional[EnvironmentEnum] = pydantic_v1.Field(default=None)
+    """
+    The environment this workflow deployment is used in
+    
+    - `DEVELOPMENT` - Development
+    - `STAGING` - Staging
+    - `PRODUCTION` - Production
+    """
+
     created: dt.datetime
-    label: str = pydantic.Field(description="A human-readable label for the deployment")
-    name: str = pydantic.Field(description="A name that uniquely identifies this deployment within its workspace")
-    status: typing.Optional[EntityStatus] = pydantic.Field(
-        description=("The current status of the deployment\n" "\n" "- `ACTIVE` - Active\n" "- `ARCHIVED` - Archived\n")
-    )
-    environment: typing.Optional[EnvironmentEnum] = pydantic.Field(
-        description=(
-            "The environment this deployment is used in\n"
-            "\n"
-            "- `DEVELOPMENT` - Development\n"
-            "- `STAGING` - Staging\n"
-            "- `PRODUCTION` - Production\n"
-        )
-    )
     last_deployed_on: dt.datetime
-    input_variables: typing.List[VellumVariable]
+    input_variables: typing.List[VellumVariable] = pydantic_v1.Field()
+    """
+    The input variables this Workflow Deployment expects to receive values for when it is executed.
+    """
+
+    output_variables: typing.List[VellumVariable] = pydantic_v1.Field()
+    """
+    The output variables this Workflow Deployment produces values for when it's executed.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/slim_document.py` & `vellum_ai-0.5.0/src/vellum/types/slim_document.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,67 +1,84 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .document_document_to_document_index import DocumentDocumentToDocumentIndex
 from .document_status import DocumentStatus
 from .processing_failure_reason_enum import ProcessingFailureReasonEnum
 from .processing_state_enum import ProcessingStateEnum
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class SlimDocument(pydantic.BaseModel):
-    id: str = pydantic.Field(description="Vellum-generated ID that uniquely identifies this document.")
-    external_id: typing.Optional[str] = pydantic.Field(
-        description="The external ID that was originally provided when uploading the document."
-    )
-    last_uploaded_at: dt.datetime = pydantic.Field(
-        description="A timestamp representing when this document was most recently uploaded."
-    )
-    label: str = pydantic.Field(description="Human-friendly name for this document.")
-    processing_state: typing.Optional[ProcessingStateEnum] = pydantic.Field(
-        description=(
-            "An enum value representing where this document is along its processing lifecycle. Note that this is different than its indexing lifecycle.\n"
-            "\n"
-            "- `QUEUED` - Queued\n"
-            "- `PROCESSING` - Processing\n"
-            "- `PROCESSED` - Processed\n"
-            "- `FAILED` - Failed\n"
-        )
-    )
-    processing_failure_reason: typing.Optional[ProcessingFailureReasonEnum] = pydantic.Field(
-        description=(
-            "An enum value representing why the document could not be processed. Is null unless processing_state is FAILED.\n"
-            "\n"
-            "- `EXCEEDED_CHARACTER_LIMIT` - Exceeded Character Limit\n"
-            "- `INVALID_FILE` - Invalid File\n"
-        )
-    )
-    status: typing.Optional[DocumentStatus] = pydantic.Field(
-        description=("The document's current status.\n" "\n" "- `ACTIVE` - Active\n")
-    )
-    keywords: typing.Optional[typing.List[str]] = pydantic.Field(
-        description="A list of keywords associated with this document. Originally provided when uploading the document."
-    )
-    metadata: typing.Optional[typing.Dict[str, typing.Any]] = pydantic.Field(
-        description="A previously supplied JSON object containing metadata that can be filtered on when searching."
-    )
+
+class SlimDocument(pydantic_v1.BaseModel):
+    id: str = pydantic_v1.Field()
+    """
+    Vellum-generated ID that uniquely identifies this document.
+    """
+
+    external_id: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The external ID that was originally provided when uploading the document.
+    """
+
+    last_uploaded_at: dt.datetime = pydantic_v1.Field()
+    """
+    A timestamp representing when this document was most recently uploaded.
+    """
+
+    label: str = pydantic_v1.Field()
+    """
+    Human-friendly name for this document.
+    """
+
+    processing_state: typing.Optional[ProcessingStateEnum] = pydantic_v1.Field(default=None)
+    """
+    An enum value representing where this document is along its processing lifecycle. Note that this is different than its indexing lifecycle.
+    
+    - `QUEUED` - Queued
+    - `PROCESSING` - Processing
+    - `PROCESSED` - Processed
+    - `FAILED` - Failed
+    """
+
+    processing_failure_reason: typing.Optional[ProcessingFailureReasonEnum] = pydantic_v1.Field(default=None)
+    """
+    An enum value representing why the document could not be processed. Is null unless processing_state is FAILED.
+    
+    - `EXCEEDED_CHARACTER_LIMIT` - Exceeded Character Limit
+    - `INVALID_FILE` - Invalid File
+    """
+
+    status: typing.Optional[DocumentStatus] = pydantic_v1.Field(default=None)
+    """
+    The document's current status.
+    
+    - `ACTIVE` - Active
+    """
+
+    keywords: typing.Optional[typing.List[str]] = pydantic_v1.Field(default=None)
+    """
+    A list of keywords associated with this document. Originally provided when uploading the document.
+    """
+
+    metadata: typing.Optional[typing.Dict[str, typing.Any]] = pydantic_v1.Field(default=None)
+    """
+    A previously supplied JSON object containing metadata that can be filtered on when searching.
+    """
+
     document_to_document_indexes: typing.List[DocumentDocumentToDocumentIndex]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/slim_workflow_deployment.py` & `vellum_ai-0.5.0/src/vellum/types/deployment_read.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,62 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .entity_status import EntityStatus
 from .environment_enum import EnvironmentEnum
 from .vellum_variable import VellumVariable
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class SlimWorkflowDeployment(pydantic.BaseModel):
+class DeploymentRead(pydantic_v1.BaseModel):
     id: str
-    name: str = pydantic.Field(
-        description="A name that uniquely identifies this workflow deployment within its workspace"
-    )
-    label: str = pydantic.Field(description="A human-readable label for the workflow deployment")
-    status: typing.Optional[EntityStatus] = pydantic.Field(
-        description=(
-            "The current status of the workflow deployment\n" "\n" "- `ACTIVE` - Active\n" "- `ARCHIVED` - Archived\n"
-        )
-    )
-    environment: typing.Optional[EnvironmentEnum] = pydantic.Field(
-        description=(
-            "The environment this workflow deployment is used in\n"
-            "\n"
-            "- `DEVELOPMENT` - Development\n"
-            "- `STAGING` - Staging\n"
-            "- `PRODUCTION` - Production\n"
-        )
-    )
     created: dt.datetime
+    label: str = pydantic_v1.Field()
+    """
+    A human-readable label for the deployment
+    """
+
+    name: str = pydantic_v1.Field()
+    """
+    A name that uniquely identifies this deployment within its workspace
+    """
+
+    status: typing.Optional[EntityStatus] = pydantic_v1.Field(default=None)
+    """
+    The current status of the deployment
+    
+    - `ACTIVE` - Active
+    - `ARCHIVED` - Archived
+    """
+
+    environment: typing.Optional[EnvironmentEnum] = pydantic_v1.Field(default=None)
+    """
+    The environment this deployment is used in
+    
+    - `DEVELOPMENT` - Development
+    - `STAGING` - Staging
+    - `PRODUCTION` - Production
+    """
+
     last_deployed_on: dt.datetime
-    input_variables: typing.List[VellumVariable] = pydantic.Field(
-        description="The input variables this Workflow Deployment expects to receive values for when it is executed."
-    )
-    output_variables: typing.List[VellumVariable] = pydantic.Field(
-        description="The output variables this Workflow Deployment will produce when it is executed."
-    )
+    input_variables: typing.List[VellumVariable]
+    active_model_version_ids: typing.List[str] = pydantic_v1.Field()
+    """
+    Deprecated. The Prompt execution endpoints return a `prompt_version_id` that could be used instead.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/streaming_execute_prompt_event.py` & `vellum_ai-0.5.0/src/vellum/types/test_suite_run_external_exec_config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .prompt_output import PromptOutput
-from .streaming_prompt_execution_meta import StreamingPromptExecutionMeta
+from ..core.pydantic_utilities import pydantic_v1
+from .test_suite_run_external_exec_config_data import TestSuiteRunExternalExecConfigData
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class StreamingExecutePromptEvent(pydantic.BaseModel):
+class TestSuiteRunExternalExecConfig(pydantic_v1.BaseModel):
     """
-    The data returned for each delta during the prompt execution stream.
+    Execution configuration for running a Vellum Test Suite against an external callable
     """
 
-    output: PromptOutput
-    output_index: int
-    execution_id: str
-    meta: typing.Optional[StreamingPromptExecutionMeta]
-    raw: typing.Optional[typing.Dict[str, typing.Any]] = pydantic.Field(
-        description="The subset of the raw response from the model that the request opted into with `expand_raw`."
-    )
+    data: TestSuiteRunExternalExecConfigData
+    test_case_ids: typing.Optional[typing.List[str]] = pydantic_v1.Field(default=None)
+    """
+    Optionally specify a subset of test case ids to run. If not provided, all test cases within the test suite will be run by default.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/streaming_prompt_execution_meta.py` & `vellum_ai-0.5.0/src/vellum/types/test_case_error_variable_value.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from .vellum_error import VellumError
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class StreamingPromptExecutionMeta(pydantic.BaseModel):
+class TestCaseErrorVariableValue(pydantic_v1.BaseModel):
     """
-    The subset of the metadata tracked by Vellum during prompt execution that the request opted into with `expand_meta`.
+    An error value for a variable in a Test Case.
     """
 
-    latency: typing.Optional[int]
+    variable_id: str
+    name: str
+    value: typing.Optional[VellumError] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/streaming_workflow_node_result_event.py` & `vellum_ai-0.5.0/src/vellum/types/terminal_node_chat_history_result.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .node_output_compiled_value import NodeOutputCompiledValue
-from .workflow_node_result_data import WorkflowNodeResultData
+from ..core.pydantic_utilities import pydantic_v1
+from .chat_message import ChatMessage
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class StreamingWorkflowNodeResultEvent(pydantic.BaseModel):
+class TerminalNodeChatHistoryResult(pydantic_v1.BaseModel):
+    id: typing.Optional[str] = None
+    name: str = pydantic_v1.Field()
     """
-    An event that indicates that the node has execution is in progress.
+    The unique name given to the terminal node that produced this output.
     """
 
-    id: str
-    node_id: str
-    node_result_id: str
-    ts: typing.Optional[dt.datetime]
-    data: typing.Optional[WorkflowNodeResultData]
-    output: typing.Optional[NodeOutputCompiledValue]
-    output_index: typing.Optional[int]
+    value: typing.Optional[typing.List[ChatMessage]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/string_chat_message_content.py` & `vellum_ai-0.5.0/src/vellum/types/workflow_output_string.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class WorkflowOutputString(pydantic_v1.BaseModel):
+    """
+    A string output from a Workflow execution.
+    """
 
-class StringChatMessageContent(pydantic.BaseModel):
+    id: str
+    name: str = pydantic_v1.Field()
     """
-    A string value that is used in a chat message.
+    The output's name, as defined in the workflow
     """
 
-    value: str
+    value: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/string_chat_message_content_request.py` & `vellum_ai-0.5.0/src/vellum/types/scenario_input_chat_history_variable_value.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from .chat_message import ChatMessage
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class StringChatMessageContentRequest(pydantic.BaseModel):
+class ScenarioInputChatHistoryVariableValue(pydantic_v1.BaseModel):
     """
-    A string value that is used in a chat message.
+    Prompt Sandbox Scenario input value that is of type CHAT_HISTORY
     """
 
-    value: str
+    value: typing.Optional[typing.List[ChatMessage]] = None
+    input_variable_id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/string_input_request.py` & `vellum_ai-0.5.0/src/vellum/types/named_test_case_error_variable_value_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from .vellum_error_request import VellumErrorRequest
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class StringInputRequest(pydantic.BaseModel):
+class NamedTestCaseErrorVariableValueRequest(pydantic_v1.BaseModel):
     """
-    A user input representing a string value
+    Named Test Case value that is of type ERROR
     """
 
-    name: str = pydantic.Field(description="The variable's name, as defined in the deployment.")
-    value: str
+    value: typing.Optional[VellumErrorRequest] = None
+    name: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/string_variable_value.py` & `vellum_ai-0.5.0/src/vellum/types/execution_function_call_vellum_value.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from .function_call import FunctionCall
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class ExecutionFunctionCallVellumValue(pydantic_v1.BaseModel):
+    id: str = pydantic_v1.Field()
+    """
+    The variable's uniquely identifying internal id.
+    """
 
-class StringVariableValue(pydantic.BaseModel):
-    value: typing.Optional[str]
+    name: str
+    value: typing.Optional[FunctionCall] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/submit_completion_actual_request.py` & `vellum_ai-0.5.0/src/vellum/types/workflow_execution_actual_json_request.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,48 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class SubmitCompletionActualRequest(pydantic.BaseModel):
-    id: typing.Optional[str] = pydantic.Field(
-        description="The Vellum-generated ID of a previously generated completion. Must provide either this or external_id."
-    )
-    external_id: typing.Optional[str] = pydantic.Field(
-        description="The external ID that was originally provided when generating the completion that you'd now like to submit actuals for. Must provide either this or id."
-    )
-    text: typing.Optional[str] = pydantic.Field(description="Text representing what the completion _should_ have been.")
-    quality: typing.Optional[float] = pydantic.Field(
-        description="A number between 0 and 1 representing the quality of the completion. 0 is the worst, 1 is the best."
-    )
-    timestamp: typing.Optional[dt.datetime] = pydantic.Field(
-        description="Optionally provide the timestamp representing when this feedback was collected. Used for reporting purposes."
-    )
+
+class WorkflowExecutionActualJsonRequest(pydantic_v1.BaseModel):
+    output_id: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The Vellum-generated ID of a workflow output. Must provide either this or output_key. output_key is typically preferred.
+    """
+
+    output_key: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The user-defined name of a workflow output. Must provide either this or output_id. Should correspond to the `Name` specified in a Final Output Node. Generally preferred over output_id.
+    """
+
+    quality: typing.Optional[float] = pydantic_v1.Field(default=None)
+    """
+    Optionally provide a decimal number between 0.0 and 1.0 (inclusive) representing the quality of the output. 0 is the worst, 1 is the best.
+    """
+
+    timestamp: typing.Optional[float] = pydantic_v1.Field(default=None)
+    """
+    Optionally provide the timestamp representing when this feedback was collected. Used for reporting purposes.
+    """
+
+    desired_output_value: typing.Optional[typing.Dict[str, typing.Any]] = pydantic_v1.Field(default=None)
+    """
+    Optionally provide the value that the output ideally should have been.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/submit_completion_actuals_error_response.py` & `vellum_ai-0.5.0/src/vellum/types/code_execution_node_error_result.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from .vellum_error import VellumError
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class SubmitCompletionActualsErrorResponse(pydantic.BaseModel):
-    detail: str
+class CodeExecutionNodeErrorResult(pydantic_v1.BaseModel):
+    id: str
+    value: typing.Optional[VellumError] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/submit_workflow_execution_actual_request.py` & `vellum_ai-0.5.0/src/vellum/types/submit_workflow_execution_actual_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from __future__ import annotations
 
 import typing
 
-import typing_extensions
-
 from .workflow_execution_actual_chat_history_request import WorkflowExecutionActualChatHistoryRequest
 from .workflow_execution_actual_json_request import WorkflowExecutionActualJsonRequest
 from .workflow_execution_actual_string_request import WorkflowExecutionActualStringRequest
 
 
 class SubmitWorkflowExecutionActualRequest_String(WorkflowExecutionActualStringRequest):
-    output_type: typing_extensions.Literal["STRING"]
+    output_type: typing.Literal["STRING"] = "STRING"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class SubmitWorkflowExecutionActualRequest_Json(WorkflowExecutionActualJsonRequest):
-    output_type: typing_extensions.Literal["JSON"]
+    output_type: typing.Literal["JSON"] = "JSON"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class SubmitWorkflowExecutionActualRequest_ChatHistory(WorkflowExecutionActualChatHistoryRequest):
-    output_type: typing_extensions.Literal["CHAT_HISTORY"]
+    output_type: typing.Literal["CHAT_HISTORY"] = "CHAT_HISTORY"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 SubmitWorkflowExecutionActualRequest = typing.Union[
     SubmitWorkflowExecutionActualRequest_String,
     SubmitWorkflowExecutionActualRequest_Json,
     SubmitWorkflowExecutionActualRequest_ChatHistory,
 ]
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/subworkflow_node_result.py` & `vellum_ai-0.5.0/src/vellum/types/test_suite_run_metric_number_output.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class SubworkflowNodeResult(pydantic.BaseModel):
+class TestSuiteRunMetricNumberOutput(pydantic_v1.BaseModel):
     """
-    A Node Result Event emitted from a Subworkflow Node.
+    Output for a test suite run metric that is of type NUMBER
     """
 
+    value: float
+    name: str
+
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/templating_node_chat_history_result.py` & `vellum_ai-0.5.0/src/vellum/types/templating_node_error_result.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .chat_message import ChatMessage
+from ..core.pydantic_utilities import pydantic_v1
+from .vellum_error import VellumError
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class TemplatingNodeChatHistoryResult(pydantic.BaseModel):
+class TemplatingNodeErrorResult(pydantic_v1.BaseModel):
     id: str
-    value: typing.Optional[typing.List[ChatMessage]]
+    value: typing.Optional[VellumError] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/templating_node_error_result.py` & `vellum_ai-0.5.0/src/vellum/types/terminal_node_result.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .vellum_error import VellumError
+from ..core.pydantic_utilities import pydantic_v1
+from .terminal_node_result_data import TerminalNodeResultData
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class TerminalNodeResult(pydantic_v1.BaseModel):
+    """
+    A Node Result Event emitted from a Terminal Node.
+    """
 
-class TemplatingNodeErrorResult(pydantic.BaseModel):
-    id: str
-    value: typing.Optional[VellumError]
+    data: TerminalNodeResultData
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/templating_node_json_result.py` & `vellum_ai-0.5.0/src/vellum/types/test_suite_run_test_suite.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class TemplatingNodeJsonResult(pydantic.BaseModel):
+class TestSuiteRunTestSuite(pydantic_v1.BaseModel):
     id: str
-    value: typing.Optional[typing.Dict[str, typing.Any]]
+    history_item_id: str
+    label: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/templating_node_number_result.py` & `vellum_ai-0.5.0/src/vellum/types/terminal_node_string_result.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class TerminalNodeStringResult(pydantic_v1.BaseModel):
+    id: typing.Optional[str] = None
+    name: str = pydantic_v1.Field()
+    """
+    The unique name given to the terminal node that produced this output.
+    """
 
-class TemplatingNodeNumberResult(pydantic.BaseModel):
-    id: str
-    value: typing.Optional[float]
+    value: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/templating_node_result.py` & `vellum_ai-0.5.0/src/vellum/types/test_case_number_variable_value.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .templating_node_result_data import TemplatingNodeResultData
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class TemplatingNodeResult(pydantic.BaseModel):
+class TestCaseNumberVariableValue(pydantic_v1.BaseModel):
     """
-    A Node Result Event emitted from a Templating Node.
+    A numerical value for a variable in a Test Case.
     """
 
-    data: TemplatingNodeResultData
+    variable_id: str
+    name: str
+    value: typing.Optional[float] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/templating_node_result_data.py` & `vellum_ai-0.5.0/src/vellum/types/named_test_case_function_call_variable_value_request.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .templating_node_result_output import TemplatingNodeResultOutput
+from ..core.pydantic_utilities import pydantic_v1
+from .fulfilled_function_call_request import FulfilledFunctionCallRequest
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class NamedTestCaseFunctionCallVariableValueRequest(pydantic_v1.BaseModel):
+    """
+    Named Test Case value that is of type FUNCTION_CALL
+    """
 
-class TemplatingNodeResultData(pydantic.BaseModel):
-    output: TemplatingNodeResultOutput
+    value: typing.Optional[FulfilledFunctionCallRequest] = None
+    name: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/templating_node_result_output.py` & `vellum_ai-0.5.0/src/vellum/types/terminal_node_result_output.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,78 +1,106 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from __future__ import annotations
 
 import typing
 
-import typing_extensions
+from .terminal_node_array_result import TerminalNodeArrayResult
+from .terminal_node_chat_history_result import TerminalNodeChatHistoryResult
+from .terminal_node_error_result import TerminalNodeErrorResult
+from .terminal_node_function_call_result import TerminalNodeFunctionCallResult
+from .terminal_node_json_result import TerminalNodeJsonResult
+from .terminal_node_number_result import TerminalNodeNumberResult
+from .terminal_node_search_results_result import TerminalNodeSearchResultsResult
+from .terminal_node_string_result import TerminalNodeStringResult
 
-from .templating_node_chat_history_result import TemplatingNodeChatHistoryResult
-from .templating_node_error_result import TemplatingNodeErrorResult
-from .templating_node_json_result import TemplatingNodeJsonResult
-from .templating_node_number_result import TemplatingNodeNumberResult
-from .templating_node_search_results_result import TemplatingNodeSearchResultsResult
-from .templating_node_string_result import TemplatingNodeStringResult
 
+class TerminalNodeResultOutput_String(TerminalNodeStringResult):
+    type: typing.Literal["STRING"] = "STRING"
 
-class TemplatingNodeResultOutput_String(TemplatingNodeStringResult):
-    type: typing_extensions.Literal["STRING"]
+    class Config:
+        frozen = True
+        smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+
+
+class TerminalNodeResultOutput_Number(TerminalNodeNumberResult):
+    type: typing.Literal["NUMBER"] = "NUMBER"
+
+    class Config:
+        frozen = True
+        smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+
+
+class TerminalNodeResultOutput_Json(TerminalNodeJsonResult):
+    type: typing.Literal["JSON"] = "JSON"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
-class TemplatingNodeResultOutput_Number(TemplatingNodeNumberResult):
-    type: typing_extensions.Literal["NUMBER"]
+class TerminalNodeResultOutput_ChatHistory(TerminalNodeChatHistoryResult):
+    type: typing.Literal["CHAT_HISTORY"] = "CHAT_HISTORY"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
-class TemplatingNodeResultOutput_Json(TemplatingNodeJsonResult):
-    type: typing_extensions.Literal["JSON"]
+class TerminalNodeResultOutput_SearchResults(TerminalNodeSearchResultsResult):
+    type: typing.Literal["SEARCH_RESULTS"] = "SEARCH_RESULTS"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
-class TemplatingNodeResultOutput_ChatHistory(TemplatingNodeChatHistoryResult):
-    type: typing_extensions.Literal["CHAT_HISTORY"]
+class TerminalNodeResultOutput_Array(TerminalNodeArrayResult):
+    type: typing.Literal["ARRAY"] = "ARRAY"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
-class TemplatingNodeResultOutput_SearchResults(TemplatingNodeSearchResultsResult):
-    type: typing_extensions.Literal["SEARCH_RESULTS"]
+class TerminalNodeResultOutput_FunctionCall(TerminalNodeFunctionCallResult):
+    type: typing.Literal["FUNCTION_CALL"] = "FUNCTION_CALL"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
-class TemplatingNodeResultOutput_Error(TemplatingNodeErrorResult):
-    type: typing_extensions.Literal["ERROR"]
+class TerminalNodeResultOutput_Error(TerminalNodeErrorResult):
+    type: typing.Literal["ERROR"] = "ERROR"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
-TemplatingNodeResultOutput = typing.Union[
-    TemplatingNodeResultOutput_String,
-    TemplatingNodeResultOutput_Number,
-    TemplatingNodeResultOutput_Json,
-    TemplatingNodeResultOutput_ChatHistory,
-    TemplatingNodeResultOutput_SearchResults,
-    TemplatingNodeResultOutput_Error,
+TerminalNodeResultOutput = typing.Union[
+    TerminalNodeResultOutput_String,
+    TerminalNodeResultOutput_Number,
+    TerminalNodeResultOutput_Json,
+    TerminalNodeResultOutput_ChatHistory,
+    TerminalNodeResultOutput_SearchResults,
+    TerminalNodeResultOutput_Array,
+    TerminalNodeResultOutput_FunctionCall,
+    TerminalNodeResultOutput_Error,
 ]
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/templating_node_search_results_result.py` & `vellum_ai-0.5.0/src/vellum/types/string_variable_value.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .search_result import SearchResult
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class TemplatingNodeSearchResultsResult(pydantic.BaseModel):
-    id: str
-    value: typing.Optional[typing.List[SearchResult]]
+class StringVariableValue(pydantic_v1.BaseModel):
+    value: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/templating_node_string_result.py` & `vellum_ai-0.5.0/src/vellum/types/workflow_output_array.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from .array_variable_value_item import ArrayVariableValueItem
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class WorkflowOutputArray(pydantic_v1.BaseModel):
+    """
+    An array output from a Workflow execution.
+    """
 
-class TemplatingNodeStringResult(pydantic.BaseModel):
     id: str
-    value: typing.Optional[str]
+    name: str = pydantic_v1.Field()
+    """
+    The output's name, as defined in the workflow
+    """
+
+    value: typing.Optional[typing.List[ArrayVariableValueItem]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/terminal_node_array_result.py` & `vellum_ai-0.5.0/src/vellum/types/document_document_to_document_index.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,45 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .array_variable_value_item import ArrayVariableValueItem
+from ..core.pydantic_utilities import pydantic_v1
+from .indexing_state_enum import IndexingStateEnum
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class TerminalNodeArrayResult(pydantic.BaseModel):
-    id: typing.Optional[str]
-    name: str = pydantic.Field(description="The unique name given to the terminal node that produced this output.")
-    value: typing.Optional[typing.List[ArrayVariableValueItem]]
+class DocumentDocumentToDocumentIndex(pydantic_v1.BaseModel):
+    id: str = pydantic_v1.Field()
+    """
+    Vellum-generated ID that uniquely identifies this link.
+    """
+
+    document_index_id: str = pydantic_v1.Field()
+    """
+    Vellum-generated ID that uniquely identifies the index this document is included in.
+    """
+
+    indexing_state: typing.Optional[IndexingStateEnum] = pydantic_v1.Field(default=None)
+    """
+    An enum value representing where this document is along its indexing lifecycle for this index.
+    
+    - `AWAITING_PROCESSING` - Awaiting Processing
+    - `QUEUED` - Queued
+    - `INDEXING` - Indexing
+    - `INDEXED` - Indexed
+    - `FAILED` - Failed
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/terminal_node_chat_history_result.py` & `vellum_ai-0.5.0/src/vellum/types/sandbox_scenario.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .chat_message import ChatMessage
+from ..core.pydantic_utilities import pydantic_v1
+from .scenario_input import ScenarioInput
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class TerminalNodeChatHistoryResult(pydantic.BaseModel):
-    id: typing.Optional[str]
-    name: str = pydantic.Field(description="The unique name given to the terminal node that produced this output.")
-    value: typing.Optional[typing.List[ChatMessage]]
+class SandboxScenario(pydantic_v1.BaseModel):
+    """
+    Sandbox Scenario
+    """
+
+    label: typing.Optional[str] = None
+    inputs: typing.List[ScenarioInput] = pydantic_v1.Field()
+    """
+    The inputs for the scenario
+    """
+
+    id: str = pydantic_v1.Field()
+    """
+    The id of the scenario
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/terminal_node_error_result.py` & `vellum_ai-0.5.0/src/vellum/types/test_suite_run_workflow_release_tag_exec_config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .vellum_error import VellumError
+from ..core.pydantic_utilities import pydantic_v1
+from .test_suite_run_workflow_release_tag_exec_config_data import TestSuiteRunWorkflowReleaseTagExecConfigData
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class TerminalNodeErrorResult(pydantic.BaseModel):
-    id: typing.Optional[str]
-    name: str = pydantic.Field(description="The unique name given to the terminal node that produced this output.")
-    value: typing.Optional[VellumError]
+class TestSuiteRunWorkflowReleaseTagExecConfig(pydantic_v1.BaseModel):
+    """
+    Execution configuration for running a Test Suite against a Workflow Deployment
+    """
+
+    data: TestSuiteRunWorkflowReleaseTagExecConfigData
+    test_case_ids: typing.Optional[typing.List[str]] = pydantic_v1.Field(default=None)
+    """
+    Optionally specify a subset of test case ids to run. If not provided, all test cases within the test suite will be run by default.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/terminal_node_function_call_result.py` & `vellum_ai-0.5.0/src/vellum/types/test_suite_run_external_exec_config_request.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .function_call import FunctionCall
+from ..core.pydantic_utilities import pydantic_v1
+from .test_suite_run_external_exec_config_data_request import TestSuiteRunExternalExecConfigDataRequest
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class TerminalNodeFunctionCallResult(pydantic.BaseModel):
-    id: typing.Optional[str]
-    name: str = pydantic.Field(description="The unique name given to the terminal node that produced this output.")
-    value: typing.Optional[FunctionCall]
+class TestSuiteRunExternalExecConfigRequest(pydantic_v1.BaseModel):
+    """
+    Execution configuration for running a Vellum Test Suite against an external callable
+    """
+
+    data: TestSuiteRunExternalExecConfigDataRequest
+    test_case_ids: typing.Optional[typing.List[str]] = pydantic_v1.Field(default=None)
+    """
+    Optionally specify a subset of test case ids to run. If not provided, all test cases within the test suite will be run by default.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/terminal_node_json_result.py` & `vellum_ai-0.5.0/src/vellum/types/node_input_compiled_json_value.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class TerminalNodeJsonResult(pydantic.BaseModel):
-    id: typing.Optional[str]
-    name: str = pydantic.Field(description="The unique name given to the terminal node that produced this output.")
-    value: typing.Optional[typing.Dict[str, typing.Any]]
+class NodeInputCompiledJsonValue(pydantic_v1.BaseModel):
+    node_input_id: str
+    key: str
+    value: typing.Optional[typing.Dict[str, typing.Any]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/terminal_node_number_result.py` & `vellum_ai-0.5.0/src/vellum/types/submit_completion_actuals_error_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class TerminalNodeNumberResult(pydantic.BaseModel):
-    id: typing.Optional[str]
-    name: str = pydantic.Field(description="The unique name given to the terminal node that produced this output.")
-    value: typing.Optional[float]
+class SubmitCompletionActualsErrorResponse(pydantic_v1.BaseModel):
+    detail: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/terminal_node_result_data.py` & `vellum_ai-0.5.0/src/vellum/types/node_output_compiled_chat_history_value.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .terminal_node_result_output import TerminalNodeResultOutput
+from ..core.pydantic_utilities import pydantic_v1
+from .chat_message import ChatMessage
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class TerminalNodeResultData(pydantic.BaseModel):
-    output: TerminalNodeResultOutput
+class NodeOutputCompiledChatHistoryValue(pydantic_v1.BaseModel):
+    node_output_id: str
+    value: typing.Optional[typing.List[ChatMessage]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/terminal_node_search_results_result.py` & `vellum_ai-0.5.0/src/vellum/types/workflow_result_event_output_data_string.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,42 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .search_result import SearchResult
+from ..core.pydantic_utilities import pydantic_v1
+from .workflow_node_result_event_state import WorkflowNodeResultEventState
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class TerminalNodeSearchResultsResult(pydantic.BaseModel):
-    id: typing.Optional[str]
-    name: str = pydantic.Field(description="The unique name given to the terminal node that produced this output.")
-    value: typing.Optional[typing.List[SearchResult]]
+class WorkflowResultEventOutputDataString(pydantic_v1.BaseModel):
+    """
+    A string output streamed from a Workflow execution.
+    """
+
+    id: typing.Optional[str] = None
+    name: str
+    state: WorkflowNodeResultEventState
+    node_id: str
+    delta: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The newly output string value, meant to be concatenated with all previous. Will be non-null for events of state STREAMING.
+    """
+
+    value: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The entire string value. Will be non-null for events of state FULFILLED.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/terminal_node_string_result.py` & `vellum_ai-0.5.0/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_request.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class TerminalNodeStringResult(pydantic.BaseModel):
-    id: typing.Optional[str]
-    name: str = pydantic.Field(description="The unique name given to the terminal node that produced this output.")
-    value: typing.Optional[str]
+from ..core.pydantic_utilities import pydantic_v1
+from .test_suite_run_deployment_release_tag_exec_config_data_request import (
+    TestSuiteRunDeploymentReleaseTagExecConfigDataRequest,
+)
+
+
+class TestSuiteRunDeploymentReleaseTagExecConfigRequest(pydantic_v1.BaseModel):
+    """
+    Execution configuration for running a Test Suite against a Prompt Deployment
+    """
+
+    data: TestSuiteRunDeploymentReleaseTagExecConfigDataRequest
+    test_case_ids: typing.Optional[typing.List[str]] = pydantic_v1.Field(default=None)
+    """
+    Optionally specify a subset of test case ids to run. If not provided, all test cases within the test suite will be run by default.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/test_case_chat_history_variable_value.py` & `vellum_ai-0.5.0/src/vellum/types/chat_history_variable_value.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .chat_message import ChatMessage
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class TestCaseChatHistoryVariableValue(pydantic.BaseModel):
-    variable_id: str
-    value: typing.Optional[typing.List[ChatMessage]]
+class ChatHistoryVariableValue(pydantic_v1.BaseModel):
+    value: typing.Optional[typing.List[ChatMessage]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/test_case_error_variable_value.py` & `vellum_ai-0.5.0/src/vellum/types/test_suite_run_execution_error_output.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .vellum_error import VellumError
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class TestCaseErrorVariableValue(pydantic.BaseModel):
-    variable_id: str
-    value: typing.Optional[VellumError]
+class TestSuiteRunExecutionErrorOutput(pydantic_v1.BaseModel):
+    """
+    Execution output of an entity evaluated during a Test Suite Run that is of type ERROR
+    """
+
+    name: str
+    value: typing.Optional[VellumError] = None
+    output_variable_id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/test_case_json_variable_value.py` & `vellum_ai-0.5.0/src/vellum/types/named_test_case_error_variable_value.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from .vellum_error import VellumError
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class NamedTestCaseErrorVariableValue(pydantic_v1.BaseModel):
+    """
+    Named Test Case value that is of type ERROR
+    """
 
-class TestCaseJsonVariableValue(pydantic.BaseModel):
-    variable_id: str
-    value: typing.Optional[typing.Dict[str, typing.Any]]
+    value: typing.Optional[VellumError] = None
+    name: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/test_case_number_variable_value.py` & `vellum_ai-0.5.0/src/vellum/types/test_suite_run_metric_string_output.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class TestSuiteRunMetricStringOutput(pydantic_v1.BaseModel):
+    """
+    Output for a test suite run metric that is of type STRING
+    """
 
-class TestCaseNumberVariableValue(pydantic.BaseModel):
-    variable_id: str
-    value: typing.Optional[float]
+    value: str
+    name: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/test_case_search_results_variable_value.py` & `vellum_ai-0.5.0/src/vellum/types/execution_search_results_vellum_value.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .search_result import SearchResult
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class ExecutionSearchResultsVellumValue(pydantic_v1.BaseModel):
+    id: str = pydantic_v1.Field()
+    """
+    The variable's uniquely identifying internal id.
+    """
 
-class TestCaseSearchResultsVariableValue(pydantic.BaseModel):
-    variable_id: str
-    value: typing.Optional[typing.List[SearchResult]]
+    name: str
+    value: typing.Optional[typing.List[SearchResult]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/test_case_variable_value.py` & `vellum_ai-0.5.0/src/vellum/types/test_case_variable_value.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,78 +1,94 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from __future__ import annotations
 
 import typing
 
-import typing_extensions
-
 from .test_case_chat_history_variable_value import TestCaseChatHistoryVariableValue
 from .test_case_error_variable_value import TestCaseErrorVariableValue
+from .test_case_function_call_variable_value import TestCaseFunctionCallVariableValue
 from .test_case_json_variable_value import TestCaseJsonVariableValue
 from .test_case_number_variable_value import TestCaseNumberVariableValue
 from .test_case_search_results_variable_value import TestCaseSearchResultsVariableValue
 from .test_case_string_variable_value import TestCaseStringVariableValue
 
 
 class TestCaseVariableValue_String(TestCaseStringVariableValue):
-    type: typing_extensions.Literal["STRING"]
+    type: typing.Literal["STRING"] = "STRING"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class TestCaseVariableValue_Number(TestCaseNumberVariableValue):
-    type: typing_extensions.Literal["NUMBER"]
+    type: typing.Literal["NUMBER"] = "NUMBER"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class TestCaseVariableValue_Json(TestCaseJsonVariableValue):
-    type: typing_extensions.Literal["JSON"]
+    type: typing.Literal["JSON"] = "JSON"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class TestCaseVariableValue_ChatHistory(TestCaseChatHistoryVariableValue):
-    type: typing_extensions.Literal["CHAT_HISTORY"]
+    type: typing.Literal["CHAT_HISTORY"] = "CHAT_HISTORY"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class TestCaseVariableValue_SearchResults(TestCaseSearchResultsVariableValue):
-    type: typing_extensions.Literal["SEARCH_RESULTS"]
+    type: typing.Literal["SEARCH_RESULTS"] = "SEARCH_RESULTS"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class TestCaseVariableValue_Error(TestCaseErrorVariableValue):
-    type: typing_extensions.Literal["ERROR"]
+    type: typing.Literal["ERROR"] = "ERROR"
+
+    class Config:
+        frozen = True
+        smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+
+
+class TestCaseVariableValue_FunctionCall(TestCaseFunctionCallVariableValue):
+    type: typing.Literal["FUNCTION_CALL"] = "FUNCTION_CALL"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 TestCaseVariableValue = typing.Union[
     TestCaseVariableValue_String,
     TestCaseVariableValue_Number,
     TestCaseVariableValue_Json,
     TestCaseVariableValue_ChatHistory,
     TestCaseVariableValue_SearchResults,
     TestCaseVariableValue_Error,
+    TestCaseVariableValue_FunctionCall,
 ]
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/test_suite_test_case.py` & `vellum_ai-0.5.0/src/vellum/types/external_test_case_execution.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .test_case_variable_value import TestCaseVariableValue
+from ..core.pydantic_utilities import pydantic_v1
+from .named_test_case_variable_value import NamedTestCaseVariableValue
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class ExternalTestCaseExecution(pydantic_v1.BaseModel):
+    outputs: typing.List[NamedTestCaseVariableValue] = pydantic_v1.Field()
+    """
+    The output values of a callable that was executed against a Test Case outside of Vellum
+    """
 
-class TestSuiteTestCase(pydantic.BaseModel):
-    id: typing.Optional[str]
-    label: typing.Optional[str]
-    input_values: typing.List[TestCaseVariableValue]
-    evaluation_values: typing.List[TestCaseVariableValue]
+    test_case_id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/upload_document_error_response.py` & `vellum_ai-0.5.0/src/vellum/types/templating_node_json_result.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class UploadDocumentErrorResponse(pydantic.BaseModel):
-    detail: str
+class TemplatingNodeJsonResult(pydantic_v1.BaseModel):
+    id: str
+    value: typing.Optional[typing.Dict[str, typing.Any]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/upload_document_response.py` & `vellum_ai-0.5.0/src/vellum/types/normalized_log_probs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from .normalized_token_log_probs import NormalizedTokenLogProbs
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class UploadDocumentResponse(pydantic.BaseModel):
-    document_id: str = pydantic.Field(description="The ID of the newly created document.")
+class NormalizedLogProbs(pydantic_v1.BaseModel):
+    tokens: typing.List[NormalizedTokenLogProbs]
+    likelihood: typing.Optional[float] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/vellum_error.py` & `vellum_ai-0.5.0/src/vellum/types/test_suite_run_metric_error_output.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .vellum_error_code_enum import VellumErrorCodeEnum
+from ..core.pydantic_utilities import pydantic_v1
+from .vellum_error import VellumError
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class TestSuiteRunMetricErrorOutput(pydantic_v1.BaseModel):
+    """
+    Output for a test suite run metric that is of type ERROR
+    """
 
-class VellumError(pydantic.BaseModel):
-    message: str
-    code: VellumErrorCodeEnum
+    value: VellumError
+    name: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/vellum_error_request.py` & `vellum_ai-0.5.0/src/vellum/types/execution_string_vellum_value.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .vellum_error_code_enum import VellumErrorCodeEnum
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class ExecutionStringVellumValue(pydantic_v1.BaseModel):
+    id: str = pydantic_v1.Field()
+    """
+    The variable's uniquely identifying internal id.
+    """
 
-class VellumErrorRequest(pydantic.BaseModel):
-    message: str
-    code: VellumErrorCodeEnum
+    name: str
+    value: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/vellum_image.py` & `vellum_ai-0.5.0/src/vellum/types/code_execution_node_json_result.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class VellumImage(pydantic.BaseModel):
-    src: str
-    metadata: typing.Optional[typing.Dict[str, typing.Any]]
+class CodeExecutionNodeJsonResult(pydantic_v1.BaseModel):
+    id: str
+    value: typing.Optional[typing.Dict[str, typing.Any]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/vellum_image_request.py` & `vellum_ai-0.5.0/src/vellum/types/terminal_node_json_result.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class TerminalNodeJsonResult(pydantic_v1.BaseModel):
+    id: typing.Optional[str] = None
+    name: str = pydantic_v1.Field()
+    """
+    The unique name given to the terminal node that produced this output.
+    """
 
-class VellumImageRequest(pydantic.BaseModel):
-    src: str
-    metadata: typing.Optional[typing.Dict[str, typing.Any]]
+    value: typing.Optional[typing.Dict[str, typing.Any]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/vellum_variable.py` & `vellum_ai-0.5.0/src/vellum/types/code_execution_node_array_result.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .vellum_variable_type import VellumVariableType
+from ..core.pydantic_utilities import pydantic_v1
+from .array_variable_value_item import ArrayVariableValueItem
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class VellumVariable(pydantic.BaseModel):
+class CodeExecutionNodeArrayResult(pydantic_v1.BaseModel):
     id: str
-    key: str
-    type: VellumVariableType
+    value: typing.Optional[typing.List[ArrayVariableValueItem]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/workflow_deployment_read.py` & `vellum_ai-0.5.0/src/vellum/types/workflow_execution_actual_string_request.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,57 +1,48 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .entity_status import EntityStatus
-from .environment_enum import EnvironmentEnum
-from .vellum_variable import VellumVariable
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class WorkflowDeploymentRead(pydantic.BaseModel):
-    id: str
-    name: str = pydantic.Field(
-        description="A name that uniquely identifies this workflow deployment within its workspace"
-    )
-    label: str = pydantic.Field(description="A human-readable label for the workflow deployment")
-    status: typing.Optional[EntityStatus] = pydantic.Field(
-        description=(
-            "The current status of the workflow deployment\n" "\n" "- `ACTIVE` - Active\n" "- `ARCHIVED` - Archived\n"
-        )
-    )
-    environment: typing.Optional[EnvironmentEnum] = pydantic.Field(
-        description=(
-            "The environment this workflow deployment is used in\n"
-            "\n"
-            "- `DEVELOPMENT` - Development\n"
-            "- `STAGING` - Staging\n"
-            "- `PRODUCTION` - Production\n"
-        )
-    )
-    created: dt.datetime
-    last_deployed_on: dt.datetime
-    input_variables: typing.List[VellumVariable] = pydantic.Field(
-        description="The input variables this Workflow Deployment expects to receive values for when it is executed."
-    )
-    output_variables: typing.List[VellumVariable] = pydantic.Field(
-        description="The output variables this Workflow Deployment produces values for when it's executed."
-    )
+from ..core.pydantic_utilities import pydantic_v1
+
+
+class WorkflowExecutionActualStringRequest(pydantic_v1.BaseModel):
+    output_id: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The Vellum-generated ID of a workflow output. Must provide either this or output_key. output_key is typically preferred.
+    """
+
+    output_key: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The user-defined name of a workflow output. Must provide either this or output_id. Should correspond to the `Name` specified in a Final Output Node. Generally preferred over output_id.
+    """
+
+    quality: typing.Optional[float] = pydantic_v1.Field(default=None)
+    """
+    Optionally provide a decimal number between 0.0 and 1.0 (inclusive) representing the quality of the output. 0 is the worst, 1 is the best.
+    """
+
+    timestamp: typing.Optional[float] = pydantic_v1.Field(default=None)
+    """
+    Optionally provide the timestamp representing when this feedback was collected. Used for reporting purposes.
+    """
+
+    desired_output_value: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    Optionally provide the value that the output ideally should have been.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/workflow_event_error.py` & `vellum_ai-0.5.0/src/vellum/types/workflow_event_error.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .workflow_execution_event_error_code import WorkflowExecutionEventErrorCode
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class WorkflowEventError(pydantic.BaseModel):
+class WorkflowEventError(pydantic_v1.BaseModel):
     message: str
     code: WorkflowExecutionEventErrorCode
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/workflow_execution_actual_chat_history_request.py` & `vellum_ai-0.5.0/src/vellum/types/workflow_execution_actual_chat_history_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,49 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .chat_message_request import ChatMessageRequest
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class WorkflowExecutionActualChatHistoryRequest(pydantic.BaseModel):
-    output_id: typing.Optional[str] = pydantic.Field(
-        description="The Vellum-generated ID of a workflow output. Must provide either this or output_key. output_key is typically preferred."
-    )
-    output_key: typing.Optional[str] = pydantic.Field(
-        description="The user-defined name of a workflow output. Must provide either this or output_id. Should correspond to the `Name` specified in a Final Output Node. Generally preferred over output_id."
-    )
-    quality: typing.Optional[float] = pydantic.Field(
-        description="Optionally provide a decimal number between 0.0 and 1.0 (inclusive) representing the quality of the output. 0 is the worst, 1 is the best."
-    )
-    timestamp: typing.Optional[float] = pydantic.Field(
-        description="Optionally provide the timestamp representing when this feedback was collected. Used for reporting purposes."
-    )
-    desired_output_value: typing.Optional[typing.List[ChatMessageRequest]] = pydantic.Field(
-        description="Optionally provide the value that the output ideally should have been."
-    )
+
+class WorkflowExecutionActualChatHistoryRequest(pydantic_v1.BaseModel):
+    output_id: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The Vellum-generated ID of a workflow output. Must provide either this or output_key. output_key is typically preferred.
+    """
+
+    output_key: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The user-defined name of a workflow output. Must provide either this or output_id. Should correspond to the `Name` specified in a Final Output Node. Generally preferred over output_id.
+    """
+
+    quality: typing.Optional[float] = pydantic_v1.Field(default=None)
+    """
+    Optionally provide a decimal number between 0.0 and 1.0 (inclusive) representing the quality of the output. 0 is the worst, 1 is the best.
+    """
+
+    timestamp: typing.Optional[float] = pydantic_v1.Field(default=None)
+    """
+    Optionally provide the timestamp representing when this feedback was collected. Used for reporting purposes.
+    """
+
+    desired_output_value: typing.Optional[typing.List[ChatMessageRequest]] = pydantic_v1.Field(default=None)
+    """
+    Optionally provide the value that the output ideally should have been.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/workflow_execution_actual_json_request.py` & `vellum_ai-0.5.0/src/vellum/types/submit_completion_actual_request.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,48 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class WorkflowExecutionActualJsonRequest(pydantic.BaseModel):
-    output_id: typing.Optional[str] = pydantic.Field(
-        description="The Vellum-generated ID of a workflow output. Must provide either this or output_key. output_key is typically preferred."
-    )
-    output_key: typing.Optional[str] = pydantic.Field(
-        description="The user-defined name of a workflow output. Must provide either this or output_id. Should correspond to the `Name` specified in a Final Output Node. Generally preferred over output_id."
-    )
-    quality: typing.Optional[float] = pydantic.Field(
-        description="Optionally provide a decimal number between 0.0 and 1.0 (inclusive) representing the quality of the output. 0 is the worst, 1 is the best."
-    )
-    timestamp: typing.Optional[float] = pydantic.Field(
-        description="Optionally provide the timestamp representing when this feedback was collected. Used for reporting purposes."
-    )
-    desired_output_value: typing.Optional[typing.Dict[str, typing.Any]] = pydantic.Field(
-        description="Optionally provide the value that the output ideally should have been."
-    )
+
+class SubmitCompletionActualRequest(pydantic_v1.BaseModel):
+    id: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The Vellum-generated ID of a previously generated completion. Must provide either this or external_id.
+    """
+
+    external_id: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The external ID that was originally provided when generating the completion that you'd now like to submit actuals for. Must provide either this or id.
+    """
+
+    text: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    Text representing what the completion _should_ have been.
+    """
+
+    quality: typing.Optional[float] = pydantic_v1.Field(default=None)
+    """
+    A number between 0 and 1 representing the quality of the completion. 0 is the worst, 1 is the best.
+    """
+
+    timestamp: typing.Optional[dt.datetime] = pydantic_v1.Field(default=None)
+    """
+    Optionally provide the timestamp representing when this feedback was collected. Used for reporting purposes.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/workflow_execution_actual_string_request.py` & `vellum_ai-0.5.0/src/vellum/types/enriched_normalized_completion.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,65 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class WorkflowExecutionActualStringRequest(pydantic.BaseModel):
-    output_id: typing.Optional[str] = pydantic.Field(
-        description="The Vellum-generated ID of a workflow output. Must provide either this or output_key. output_key is typically preferred."
-    )
-    output_key: typing.Optional[str] = pydantic.Field(
-        description="The user-defined name of a workflow output. Must provide either this or output_id. Should correspond to the `Name` specified in a Final Output Node. Generally preferred over output_id."
-    )
-    quality: typing.Optional[float] = pydantic.Field(
-        description="Optionally provide a decimal number between 0.0 and 1.0 (inclusive) representing the quality of the output. 0 is the worst, 1 is the best."
-    )
-    timestamp: typing.Optional[float] = pydantic.Field(
-        description="Optionally provide the timestamp representing when this feedback was collected. Used for reporting purposes."
-    )
-    desired_output_value: typing.Optional[str] = pydantic.Field(
-        description="Optionally provide the value that the output ideally should have been."
-    )
+from ..core.pydantic_utilities import pydantic_v1
+from .finish_reason_enum import FinishReasonEnum
+from .normalized_log_probs import NormalizedLogProbs
+from .vellum_variable_type import VellumVariableType
+
+
+class EnrichedNormalizedCompletion(pydantic_v1.BaseModel):
+    id: str = pydantic_v1.Field()
+    """
+    The Vellum-generated ID of the completion.
+    """
+
+    external_id: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The external ID that was originally provided along with the generation request, which uniquely identifies this generation in an external system.
+    """
+
+    text: str = pydantic_v1.Field()
+    """
+    The text generated by the LLM.
+    """
+
+    finish_reason: typing.Optional[FinishReasonEnum] = pydantic_v1.Field(default=None)
+    """
+    The reason the generation finished.
+    
+    - `LENGTH` - LENGTH
+    - `STOP` - STOP
+    - `UNKNOWN` - UNKNOWN
+    """
+
+    logprobs: typing.Optional[NormalizedLogProbs] = pydantic_v1.Field(default=None)
+    """
+    The logprobs of the completion. Only present if specified in the original request options.
+    """
+
+    model_version_id: str = pydantic_v1.Field()
+    """
+    The ID of the model version used to generate this completion.
+    """
+
+    prompt_version_id: str
+    type: typing.Optional[VellumVariableType] = None
+    deployment_release_tag: str
+    model_name: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/workflow_execution_workflow_result_event.py` & `vellum_ai-0.5.0/src/vellum/types/test_suite_run_external_exec_config_data_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .workflow_result_event import WorkflowResultEvent
+from ..core.pydantic_utilities import pydantic_v1
+from .external_test_case_execution_request import ExternalTestCaseExecutionRequest
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class WorkflowExecutionWorkflowResultEvent(pydantic.BaseModel):
+class TestSuiteRunExternalExecConfigDataRequest(pydantic_v1.BaseModel):
+    executions: typing.List[ExternalTestCaseExecutionRequest] = pydantic_v1.Field()
     """
-    A WORKFLOW-level event emitted from the workflow's execution.
+    The executions of some callable external to Vellum whose outputs you would like to evaluate.
     """
 
-    execution_id: str
-    run_id: typing.Optional[str]
-    external_id: typing.Optional[str]
-    data: WorkflowResultEvent
-
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/workflow_node_result_data.py` & `vellum_ai-0.5.0/src/vellum/types/workflow_node_result_data.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,95 +1,101 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from __future__ import annotations
 
 import typing
 
-import typing_extensions
-
 from .api_node_result import ApiNodeResult
 from .code_execution_node_result import CodeExecutionNodeResult
 from .conditional_node_result import ConditionalNodeResult
 from .prompt_node_result import PromptNodeResult
 from .search_node_result import SearchNodeResult
 from .subworkflow_node_result import SubworkflowNodeResult
 from .templating_node_result import TemplatingNodeResult
 from .terminal_node_result import TerminalNodeResult
 
 
 class WorkflowNodeResultData_Prompt(PromptNodeResult):
-    type: typing_extensions.Literal["PROMPT"]
+    type: typing.Literal["PROMPT"] = "PROMPT"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class WorkflowNodeResultData_Search(SearchNodeResult):
-    type: typing_extensions.Literal["SEARCH"]
+    type: typing.Literal["SEARCH"] = "SEARCH"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class WorkflowNodeResultData_Templating(TemplatingNodeResult):
-    type: typing_extensions.Literal["TEMPLATING"]
+    type: typing.Literal["TEMPLATING"] = "TEMPLATING"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class WorkflowNodeResultData_CodeExecution(CodeExecutionNodeResult):
-    type: typing_extensions.Literal["CODE_EXECUTION"]
+    type: typing.Literal["CODE_EXECUTION"] = "CODE_EXECUTION"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class WorkflowNodeResultData_Conditional(ConditionalNodeResult):
-    type: typing_extensions.Literal["CONDITIONAL"]
+    type: typing.Literal["CONDITIONAL"] = "CONDITIONAL"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class WorkflowNodeResultData_Api(ApiNodeResult):
-    type: typing_extensions.Literal["API"]
+    type: typing.Literal["API"] = "API"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class WorkflowNodeResultData_Terminal(TerminalNodeResult):
-    type: typing_extensions.Literal["TERMINAL"]
+    type: typing.Literal["TERMINAL"] = "TERMINAL"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class WorkflowNodeResultData_Subworkflow(SubworkflowNodeResult):
-    type: typing_extensions.Literal["SUBWORKFLOW"]
+    type: typing.Literal["SUBWORKFLOW"] = "SUBWORKFLOW"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 WorkflowNodeResultData = typing.Union[
     WorkflowNodeResultData_Prompt,
     WorkflowNodeResultData_Search,
     WorkflowNodeResultData_Templating,
     WorkflowNodeResultData_CodeExecution,
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/workflow_node_result_event.py` & `vellum_ai-0.5.0/src/vellum/types/workflow_node_result_event.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,57 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from __future__ import annotations
 
 import typing
 
-import typing_extensions
-
 from .fulfilled_workflow_node_result_event import FulfilledWorkflowNodeResultEvent
 from .initiated_workflow_node_result_event import InitiatedWorkflowNodeResultEvent
 from .rejected_workflow_node_result_event import RejectedWorkflowNodeResultEvent
 from .streaming_workflow_node_result_event import StreamingWorkflowNodeResultEvent
 
 
 class WorkflowNodeResultEvent_Initiated(InitiatedWorkflowNodeResultEvent):
-    state: typing_extensions.Literal["INITIATED"]
+    state: typing.Literal["INITIATED"] = "INITIATED"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class WorkflowNodeResultEvent_Streaming(StreamingWorkflowNodeResultEvent):
-    state: typing_extensions.Literal["STREAMING"]
+    state: typing.Literal["STREAMING"] = "STREAMING"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class WorkflowNodeResultEvent_Fulfilled(FulfilledWorkflowNodeResultEvent):
-    state: typing_extensions.Literal["FULFILLED"]
+    state: typing.Literal["FULFILLED"] = "FULFILLED"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class WorkflowNodeResultEvent_Rejected(RejectedWorkflowNodeResultEvent):
-    state: typing_extensions.Literal["REJECTED"]
+    state: typing.Literal["REJECTED"] = "REJECTED"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 WorkflowNodeResultEvent = typing.Union[
     WorkflowNodeResultEvent_Initiated,
     WorkflowNodeResultEvent_Streaming,
     WorkflowNodeResultEvent_Fulfilled,
     WorkflowNodeResultEvent_Rejected,
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/workflow_output.py` & `vellum_ai-0.5.0/src/vellum/types/workflow_output.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,105 +1,112 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from __future__ import annotations
 
 import typing
 
-import typing_extensions
-
 from .workflow_output_array import WorkflowOutputArray
 from .workflow_output_chat_history import WorkflowOutputChatHistory
 from .workflow_output_error import WorkflowOutputError
 from .workflow_output_function_call import WorkflowOutputFunctionCall
 from .workflow_output_image import WorkflowOutputImage
 from .workflow_output_json import WorkflowOutputJson
 from .workflow_output_number import WorkflowOutputNumber
 from .workflow_output_search_results import WorkflowOutputSearchResults
 from .workflow_output_string import WorkflowOutputString
 
 
 class WorkflowOutput_String(WorkflowOutputString):
-    type: typing_extensions.Literal["STRING"]
+    type: typing.Literal["STRING"] = "STRING"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class WorkflowOutput_Number(WorkflowOutputNumber):
-    type: typing_extensions.Literal["NUMBER"]
+    type: typing.Literal["NUMBER"] = "NUMBER"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class WorkflowOutput_Json(WorkflowOutputJson):
-    type: typing_extensions.Literal["JSON"]
+    type: typing.Literal["JSON"] = "JSON"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class WorkflowOutput_ChatHistory(WorkflowOutputChatHistory):
-    type: typing_extensions.Literal["CHAT_HISTORY"]
+    type: typing.Literal["CHAT_HISTORY"] = "CHAT_HISTORY"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class WorkflowOutput_SearchResults(WorkflowOutputSearchResults):
-    type: typing_extensions.Literal["SEARCH_RESULTS"]
+    type: typing.Literal["SEARCH_RESULTS"] = "SEARCH_RESULTS"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class WorkflowOutput_Array(WorkflowOutputArray):
-    type: typing_extensions.Literal["ARRAY"]
+    type: typing.Literal["ARRAY"] = "ARRAY"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class WorkflowOutput_Error(WorkflowOutputError):
-    type: typing_extensions.Literal["ERROR"]
+    type: typing.Literal["ERROR"] = "ERROR"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class WorkflowOutput_FunctionCall(WorkflowOutputFunctionCall):
-    type: typing_extensions.Literal["FUNCTION_CALL"]
+    type: typing.Literal["FUNCTION_CALL"] = "FUNCTION_CALL"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class WorkflowOutput_Image(WorkflowOutputImage):
-    type: typing_extensions.Literal["IMAGE"]
+    type: typing.Literal["IMAGE"] = "IMAGE"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 WorkflowOutput = typing.Union[
     WorkflowOutput_String,
     WorkflowOutput_Number,
     WorkflowOutput_Json,
     WorkflowOutput_ChatHistory,
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/workflow_output_array.py` & `vellum_ai-0.5.0/src/vellum/types/test_case_function_call_variable_value.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .array_variable_value_item import ArrayVariableValueItem
+from ..core.pydantic_utilities import pydantic_v1
+from .fulfilled_function_call import FulfilledFunctionCall
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class WorkflowOutputArray(pydantic.BaseModel):
+class TestCaseFunctionCallVariableValue(pydantic_v1.BaseModel):
     """
-    An array output from a Workflow execution.
+    A function call value for a variable in a Test Case.
     """
 
-    id: str
-    name: str = pydantic.Field(description="The output's name, as defined in the workflow")
-    value: typing.List[ArrayVariableValueItem]
+    variable_id: str
+    name: str
+    value: typing.Optional[FulfilledFunctionCall] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/workflow_output_chat_history.py` & `vellum_ai-0.5.0/src/vellum/types/vellum_error_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .chat_message import ChatMessage
+from ..core.pydantic_utilities import pydantic_v1
+from .vellum_error_code_enum import VellumErrorCodeEnum
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class WorkflowOutputChatHistory(pydantic.BaseModel):
-    """
-    A chat history output from a Workflow execution.
-    """
-
-    id: str
-    name: str = pydantic.Field(description="The output's name, as defined in the workflow")
-    value: typing.List[ChatMessage]
+
+class VellumErrorRequest(pydantic_v1.BaseModel):
+    message: str
+    code: VellumErrorCodeEnum
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/workflow_output_error.py` & `vellum_ai-0.5.0/src/vellum/types/named_test_case_number_variable_value.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .vellum_error import VellumError
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class WorkflowOutputError(pydantic.BaseModel):
+class NamedTestCaseNumberVariableValue(pydantic_v1.BaseModel):
     """
-    An error output from a Workflow execution.
+    Named Test Case value that is of type NUMBER
     """
 
-    id: str
-    name: str = pydantic.Field(description="The output's name, as defined in the workflow")
-    value: VellumError
+    value: typing.Optional[float] = None
+    name: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/workflow_output_function_call.py` & `vellum_ai-0.5.0/src/vellum/types/test_case_chat_history_variable_value.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .function_call import FunctionCall
+from ..core.pydantic_utilities import pydantic_v1
+from .chat_message import ChatMessage
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class WorkflowOutputFunctionCall(pydantic.BaseModel):
+class TestCaseChatHistoryVariableValue(pydantic_v1.BaseModel):
     """
-    A function call output from a Workflow execution.
+    A chat history value for a variable in a Test Case.
     """
 
-    id: str
-    name: str = pydantic.Field(description="The output's name, as defined in the workflow")
-    value: FunctionCall
+    variable_id: str
+    name: str
+    value: typing.Optional[typing.List[ChatMessage]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/workflow_output_image.py` & `vellum_ai-0.5.0/src/vellum/types/function_call_variable_value.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .vellum_image import VellumImage
+from ..core.pydantic_utilities import pydantic_v1
+from .function_call import FunctionCall
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class WorkflowOutputImage(pydantic.BaseModel):
-    """
-    An image output from a Workflow execution.
-    """
-
-    id: str
-    name: str = pydantic.Field(description="The output's name, as defined in the workflow")
-    value: VellumImage
+
+class FunctionCallVariableValue(pydantic_v1.BaseModel):
+    value: FunctionCall
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/workflow_output_json.py` & `vellum_ai-0.5.0/src/vellum/types/node_output_compiled_function_value.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from .function_call import FunctionCall
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class WorkflowOutputJson(pydantic.BaseModel):
-    """
-    A JSON output from a Workflow execution.
-    """
-
-    id: str
-    name: str = pydantic.Field(description="The output's name, as defined in the workflow")
-    value: typing.Dict[str, typing.Any]
+class NodeOutputCompiledFunctionValue(pydantic_v1.BaseModel):
+    node_output_id: str
+    value: typing.Optional[FunctionCall] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/workflow_output_number.py` & `vellum_ai-0.5.0/src/vellum/types/named_scenario_input_string_variable_value_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class WorkflowOutputNumber(pydantic.BaseModel):
+class NamedScenarioInputStringVariableValueRequest(pydantic_v1.BaseModel):
     """
-    A number output from a Workflow execution.
+    Named Prompt Sandbox Scenario input value that is of type STRING
     """
 
-    id: str
-    name: str = pydantic.Field(description="The output's name, as defined in the workflow")
-    value: float
+    value: typing.Optional[str] = None
+    name: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/workflow_output_search_results.py` & `vellum_ai-0.5.0/src/vellum/types/paginated_slim_document_list.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .search_result import SearchResult
+from ..core.pydantic_utilities import pydantic_v1
+from .slim_document import SlimDocument
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class WorkflowOutputSearchResults(pydantic.BaseModel):
-    """
-    A search results output from a Workflow execution.
-    """
-
-    id: str
-    name: str = pydantic.Field(description="The output's name, as defined in the workflow")
-    value: typing.List[SearchResult]
+
+class PaginatedSlimDocumentList(pydantic_v1.BaseModel):
+    count: typing.Optional[int] = None
+    next: typing.Optional[str] = None
+    previous: typing.Optional[str] = None
+    results: typing.Optional[typing.List[SlimDocument]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/workflow_output_string.py` & `vellum_ai-0.5.0/src/vellum/types/node_output_compiled_number_value.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class WorkflowOutputString(pydantic.BaseModel):
-    """
-    A string output from a Workflow execution.
-    """
-
-    id: str
-    name: str = pydantic.Field(description="The output's name, as defined in the workflow")
-    value: str
+class NodeOutputCompiledNumberValue(pydantic_v1.BaseModel):
+    node_output_id: str
+    value: typing.Optional[float] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/workflow_request_chat_history_input_request.py` & `vellum_ai-0.5.0/src/vellum/types/chat_message.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .chat_message_request import ChatMessageRequest
+from ..core.pydantic_utilities import pydantic_v1
+from .chat_message_content import ChatMessageContent
+from .chat_message_role import ChatMessageRole
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class WorkflowRequestChatHistoryInputRequest(pydantic.BaseModel):
+class ChatMessage(pydantic_v1.BaseModel):
+    text: typing.Optional[str] = None
+    role: ChatMessageRole
+    content: typing.Optional[ChatMessageContent] = None
+    source: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    The input for a chat history variable in a Workflow.
+    An optional identifier representing who or what generated this message.
     """
 
-    name: str = pydantic.Field(description="The variable's name, as defined in the Workflow.")
-    value: typing.List[ChatMessageRequest]
-
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/workflow_request_input_request.py` & `vellum_ai-0.5.0/src/vellum/types/workflow_request_input_request.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,55 +1,57 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from __future__ import annotations
 
 import typing
 
-import typing_extensions
-
 from .workflow_request_chat_history_input_request import WorkflowRequestChatHistoryInputRequest
 from .workflow_request_json_input_request import WorkflowRequestJsonInputRequest
 from .workflow_request_number_input_request import WorkflowRequestNumberInputRequest
 from .workflow_request_string_input_request import WorkflowRequestStringInputRequest
 
 
 class WorkflowRequestInputRequest_String(WorkflowRequestStringInputRequest):
-    type: typing_extensions.Literal["STRING"]
+    type: typing.Literal["STRING"] = "STRING"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class WorkflowRequestInputRequest_Json(WorkflowRequestJsonInputRequest):
-    type: typing_extensions.Literal["JSON"]
+    type: typing.Literal["JSON"] = "JSON"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class WorkflowRequestInputRequest_ChatHistory(WorkflowRequestChatHistoryInputRequest):
-    type: typing_extensions.Literal["CHAT_HISTORY"]
+    type: typing.Literal["CHAT_HISTORY"] = "CHAT_HISTORY"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class WorkflowRequestInputRequest_Number(WorkflowRequestNumberInputRequest):
-    type: typing_extensions.Literal["NUMBER"]
+    type: typing.Literal["NUMBER"] = "NUMBER"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 WorkflowRequestInputRequest = typing.Union[
     WorkflowRequestInputRequest_String,
     WorkflowRequestInputRequest_Json,
     WorkflowRequestInputRequest_ChatHistory,
     WorkflowRequestInputRequest_Number,
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/workflow_request_json_input_request.py` & `vellum_ai-0.5.0/src/vellum/types/test_suite_run_execution_string_output.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class WorkflowRequestJsonInputRequest(pydantic.BaseModel):
+class TestSuiteRunExecutionStringOutput(pydantic_v1.BaseModel):
     """
-    The input for a JSON variable in a Workflow.
+    Execution output of an entity evaluated during a Test Suite Run that is of type STRING
     """
 
-    name: str = pydantic.Field(description="The variable's name, as defined in the Workflow.")
-    value: typing.Dict[str, typing.Any]
+    name: str
+    value: typing.Optional[str] = None
+    output_variable_id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/workflow_request_number_input_request.py` & `vellum_ai-0.5.0/src/vellum/types/workflow_output_error.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from .vellum_error import VellumError
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class WorkflowOutputError(pydantic_v1.BaseModel):
+    """
+    An error output from a Workflow execution.
+    """
 
-class WorkflowRequestNumberInputRequest(pydantic.BaseModel):
+    id: str
+    name: str = pydantic_v1.Field()
     """
-    The input for a number variable in a Workflow.
+    The output's name, as defined in the workflow
     """
 
-    name: str = pydantic.Field(description="The variable's name, as defined in the Workflow.")
-    value: float
+    value: typing.Optional[VellumError] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/workflow_request_string_input_request.py` & `vellum_ai-0.5.0/src/vellum/types/fulfilled_prompt_execution_meta.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from .finish_reason_enum import FinishReasonEnum
+from .ml_model_usage import MlModelUsage
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class WorkflowRequestStringInputRequest(pydantic.BaseModel):
+class FulfilledPromptExecutionMeta(pydantic_v1.BaseModel):
     """
-    The input for a string variable in a Workflow.
+    The subset of the metadata tracked by Vellum during prompt execution that the request opted into with `expand_meta`.
     """
 
-    name: str = pydantic.Field(description="The variable's name, as defined in the Workflow.")
-    value: str
+    latency: typing.Optional[int] = None
+    finish_reason: typing.Optional[FinishReasonEnum] = None
+    usage: typing.Optional[MlModelUsage] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/workflow_result_event.py` & `vellum_ai-0.5.0/src/vellum/types/workflow_result_event.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from .execution_vellum_value import ExecutionVellumValue
 from .workflow_event_error import WorkflowEventError
 from .workflow_node_result_event_state import WorkflowNodeResultEventState
 from .workflow_output import WorkflowOutput
 from .workflow_result_event_output_data import WorkflowResultEventOutputData
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class WorkflowResultEvent(pydantic.BaseModel):
+class WorkflowResultEvent(pydantic_v1.BaseModel):
     id: str
     state: WorkflowNodeResultEventState
     ts: dt.datetime
-    output: typing.Optional[WorkflowResultEventOutputData]
-    error: typing.Optional[WorkflowEventError]
-    outputs: typing.Optional[typing.List[WorkflowOutput]]
+    output: typing.Optional[WorkflowResultEventOutputData] = None
+    error: typing.Optional[WorkflowEventError] = None
+    outputs: typing.Optional[typing.List[WorkflowOutput]] = None
+    inputs: typing.Optional[typing.List[ExecutionVellumValue]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/workflow_result_event_output_data.py` & `vellum_ai-0.5.0/src/vellum/types/workflow_result_event_output_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,95 +1,101 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from __future__ import annotations
 
 import typing
 
-import typing_extensions
-
 from .workflow_result_event_output_data_array import WorkflowResultEventOutputDataArray
 from .workflow_result_event_output_data_chat_history import WorkflowResultEventOutputDataChatHistory
 from .workflow_result_event_output_data_error import WorkflowResultEventOutputDataError
 from .workflow_result_event_output_data_function_call import WorkflowResultEventOutputDataFunctionCall
 from .workflow_result_event_output_data_json import WorkflowResultEventOutputDataJson
 from .workflow_result_event_output_data_number import WorkflowResultEventOutputDataNumber
 from .workflow_result_event_output_data_search_results import WorkflowResultEventOutputDataSearchResults
 from .workflow_result_event_output_data_string import WorkflowResultEventOutputDataString
 
 
 class WorkflowResultEventOutputData_String(WorkflowResultEventOutputDataString):
-    type: typing_extensions.Literal["STRING"]
+    type: typing.Literal["STRING"] = "STRING"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class WorkflowResultEventOutputData_Number(WorkflowResultEventOutputDataNumber):
-    type: typing_extensions.Literal["NUMBER"]
+    type: typing.Literal["NUMBER"] = "NUMBER"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class WorkflowResultEventOutputData_Json(WorkflowResultEventOutputDataJson):
-    type: typing_extensions.Literal["JSON"]
+    type: typing.Literal["JSON"] = "JSON"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class WorkflowResultEventOutputData_ChatHistory(WorkflowResultEventOutputDataChatHistory):
-    type: typing_extensions.Literal["CHAT_HISTORY"]
+    type: typing.Literal["CHAT_HISTORY"] = "CHAT_HISTORY"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class WorkflowResultEventOutputData_SearchResults(WorkflowResultEventOutputDataSearchResults):
-    type: typing_extensions.Literal["SEARCH_RESULTS"]
+    type: typing.Literal["SEARCH_RESULTS"] = "SEARCH_RESULTS"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class WorkflowResultEventOutputData_Array(WorkflowResultEventOutputDataArray):
-    type: typing_extensions.Literal["ARRAY"]
+    type: typing.Literal["ARRAY"] = "ARRAY"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class WorkflowResultEventOutputData_FunctionCall(WorkflowResultEventOutputDataFunctionCall):
-    type: typing_extensions.Literal["FUNCTION_CALL"]
+    type: typing.Literal["FUNCTION_CALL"] = "FUNCTION_CALL"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class WorkflowResultEventOutputData_Error(WorkflowResultEventOutputDataError):
-    type: typing_extensions.Literal["ERROR"]
+    type: typing.Literal["ERROR"] = "ERROR"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 WorkflowResultEventOutputData = typing.Union[
     WorkflowResultEventOutputData_String,
     WorkflowResultEventOutputData_Number,
     WorkflowResultEventOutputData_Json,
     WorkflowResultEventOutputData_ChatHistory,
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/workflow_result_event_output_data_search_results.py` & `vellum_ai-0.5.0/src/vellum/types/fulfilled_execute_workflow_workflow_result_event.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .search_result import SearchResult
-from .workflow_node_result_event_state import WorkflowNodeResultEventState
+from ..core.pydantic_utilities import pydantic_v1
+from .workflow_output import WorkflowOutput
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class WorkflowResultEventOutputDataSearchResults(pydantic.BaseModel):
+class FulfilledExecuteWorkflowWorkflowResultEvent(pydantic_v1.BaseModel):
     """
-    A Search Results output streamed from a Workflow execution.
+    The successful response from the Workflow execution containing the produced outputs.
     """
 
-    id: typing.Optional[str]
-    name: str
-    state: WorkflowNodeResultEventState
-    node_id: str
-    delta: typing.Optional[str] = pydantic.Field(
-        description="The newly output string value. Only relevant for string outputs with a state of STREAMING."
-    )
-    value: typing.Optional[typing.List[SearchResult]]
+    id: str
+    ts: dt.datetime
+    outputs: typing.List[WorkflowOutput]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vellum_ai-0.3.9/src/vellum/types/workflow_stream_event.py` & `vellum_ai-0.5.0/src/vellum/types/workflow_stream_event.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from __future__ import annotations
 
 import typing
 
-import typing_extensions
-
 from .workflow_execution_node_result_event import WorkflowExecutionNodeResultEvent
 from .workflow_execution_workflow_result_event import WorkflowExecutionWorkflowResultEvent
 
 
 class WorkflowStreamEvent_Workflow(WorkflowExecutionWorkflowResultEvent):
-    type: typing_extensions.Literal["WORKFLOW"]
+    type: typing.Literal["WORKFLOW"] = "WORKFLOW"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class WorkflowStreamEvent_Node(WorkflowExecutionNodeResultEvent):
-    type: typing_extensions.Literal["NODE"]
+    type: typing.Literal["NODE"] = "NODE"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
 
 
 WorkflowStreamEvent = typing.Union[WorkflowStreamEvent_Workflow, WorkflowStreamEvent_Node]
```

### Comparing `vellum_ai-0.3.9/PKG-INFO` & `vellum_ai-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: vellum-ai
-Version: 0.3.9
+Version: 0.5.0
 Summary: 
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: cdktf (>=0.20.5,<0.21.0)
 Requires-Dist: httpx (>=0.21.2)
-Requires-Dist: pydantic (>=1.9.2,<2.5.0)
+Requires-Dist: publication (==0.0.3)
+Requires-Dist: pydantic (>=1.9.2)
+Requires-Dist: typing_extensions (>=4.0.0)
 Description-Content-Type: text/markdown
 
 # Vellum Python Library
 
 [![pypi](https://img.shields.io/pypi/v/vellum-ai.svg)](https://pypi.python.org/pypi/vellum-ai)
 [![fern shield](https://img.shields.io/badge/%F0%9F%8C%BF-SDK%20generated%20by%20Fern-brightgreen)](https://github.com/fern-api/fern)
```

