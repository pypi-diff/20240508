# Comparing `tmp/vellum_ai-0.5.1.tar.gz` & `tmp/vellum_ai-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vellum_ai-0.5.1.tar", max compression
+gzip compressed data, was "vellum_ai-0.5.2.tar", max compression
```

## Comparing `vellum_ai-0.5.1.tar` & `vellum_ai-0.5.2.tar`

### file list

```diff
@@ -1,382 +1,386 @@
--rw-r--r--   0        0        0     1073 2024-04-25 18:57:02.582595 vellum_ai-0.5.1/LICENSE
--rw-r--r--   0        0        0     2980 2024-04-25 18:57:02.582595 vellum_ai-0.5.1/README.md
--rw-r--r--   0        0        0      632 2024-04-25 18:57:02.582595 vellum_ai-0.5.1/pyproject.toml
--rw-r--r--   0        0        0    35591 2024-04-25 18:57:02.582595 vellum_ai-0.5.1/src/vellum/__init__.py
--rw-r--r--   0        0        0    97089 2024-04-25 18:57:02.582595 vellum_ai-0.5.1/src/vellum/client.py
--rw-r--r--   0        0        0      853 2024-04-25 18:57:02.582595 vellum_ai-0.5.1/src/vellum/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-25 18:57:02.582595 vellum_ai-0.5.1/src/vellum/core/api_error.py
--rw-r--r--   0        0        0     1697 2024-04-25 18:57:02.582595 vellum_ai-0.5.1/src/vellum/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-25 18:57:02.582595 vellum_ai-0.5.1/src/vellum/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-04-25 18:57:02.582595 vellum_ai-0.5.1/src/vellum/core/file.py
--rw-r--r--   0        0        0     5059 2024-04-25 18:57:02.582595 vellum_ai-0.5.1/src/vellum/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-04-25 18:57:02.582595 vellum_ai-0.5.1/src/vellum/core/jsonable_encoder.py
--rw-r--r--   0        0        0      329 2024-04-25 18:57:02.582595 vellum_ai-0.5.1/src/vellum/core/pydantic_utilities.py
--rw-r--r--   0        0        0      330 2024-04-25 18:57:02.582595 vellum_ai-0.5.1/src/vellum/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-04-25 18:57:02.582595 vellum_ai-0.5.1/src/vellum/core/request_options.py
--rw-r--r--   0        0        0      498 2024-04-25 18:57:02.582595 vellum_ai-0.5.1/src/vellum/environment.py
--rw-r--r--   0        0        0      343 2024-04-25 18:57:02.582595 vellum_ai-0.5.1/src/vellum/errors/__init__.py
--rw-r--r--   0        0        0      248 2024-04-25 18:57:02.582595 vellum_ai-0.5.1/src/vellum/errors/bad_request_error.py
--rw-r--r--   0        0        0      247 2024-04-25 18:57:02.582595 vellum_ai-0.5.1/src/vellum/errors/forbidden_error.py
--rw-r--r--   0        0        0      252 2024-04-25 18:57:02.582595 vellum_ai-0.5.1/src/vellum/errors/internal_server_error.py
--rw-r--r--   0        0        0      246 2024-04-25 18:57:02.582595 vellum_ai-0.5.1/src/vellum/errors/not_found_error.py
--rw-r--r--   0        0        0       79 2024-04-25 18:57:02.582595 vellum_ai-0.5.1/src/vellum/lib/__init__.py
--rw-r--r--   0        0        0       77 2024-04-25 18:57:02.582595 vellum_ai-0.5.1/src/vellum/lib/test_suites/__init__.py
--rw-r--r--   0        0        0      116 2024-04-25 18:57:02.582595 vellum_ai-0.5.1/src/vellum/lib/test_suites/constants.py
--rw-r--r--   0        0        0       56 2024-04-25 18:57:02.582595 vellum_ai-0.5.1/src/vellum/lib/test_suites/exceptions.py
--rw-r--r--   0        0        0    12323 2024-04-25 18:57:02.582595 vellum_ai-0.5.1/src/vellum/lib/test_suites/resources.py
--rw-r--r--   0        0        0        0 2024-04-25 18:57:02.582595 vellum_ai-0.5.1/src/vellum/lib/utils/__init__.py
--rw-r--r--   0        0        0      298 2024-04-25 18:57:02.582595 vellum_ai-0.5.1/src/vellum/lib/utils/env.py
--rw-r--r--   0        0        0       49 2024-04-25 18:57:02.582595 vellum_ai-0.5.1/src/vellum/lib/utils/exceptions.py
--rw-r--r--   0        0        0      698 2024-04-25 18:57:02.582595 vellum_ai-0.5.1/src/vellum/lib/utils/paginator.py
--rw-r--r--   0        0        0        0 2024-04-25 18:57:02.582595 vellum_ai-0.5.1/src/vellum/py.typed
--rw-r--r--   0        0        0      730 2024-04-25 18:57:02.582595 vellum_ai-0.5.1/src/vellum/resources/__init__.py
--rw-r--r--   0        0        0      157 2024-04-25 18:57:02.582595 vellum_ai-0.5.1/src/vellum/resources/deployments/__init__.py
--rw-r--r--   0        0        0    19588 2024-04-25 18:57:02.582595 vellum_ai-0.5.1/src/vellum/resources/deployments/client.py
--rw-r--r--   0        0        0      183 2024-04-25 18:57:02.582595 vellum_ai-0.5.1/src/vellum/resources/deployments/types/__init__.py
--rw-r--r--   0        0        0      174 2024-04-25 18:57:02.582595 vellum_ai-0.5.1/src/vellum/resources/deployments/types/deployments_list_request_status.py
--rw-r--r--   0        0        0      165 2024-04-25 18:57:02.582595 vellum_ai-0.5.1/src/vellum/resources/document_indexes/__init__.py
--rw-r--r--   0        0        0    39845 2024-04-25 18:57:02.582595 vellum_ai-0.5.1/src/vellum/resources/document_indexes/client.py
--rw-r--r--   0        0        0      196 2024-04-25 18:57:02.582595 vellum_ai-0.5.1/src/vellum/resources/document_indexes/types/__init__.py
--rw-r--r--   0        0        0      178 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/resources/document_indexes/types/document_indexes_list_request_status.py
--rw-r--r--   0        0        0       65 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/resources/documents/__init__.py
--rw-r--r--   0        0        0    34010 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/resources/documents/client.py
--rw-r--r--   0        0        0       65 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/resources/folder_entities/__init__.py
--rw-r--r--   0        0        0     6435 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/resources/folder_entities/client.py
--rw-r--r--   0        0        0       65 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/resources/sandboxes/__init__.py
--rw-r--r--   0        0        0    12738 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/resources/sandboxes/client.py
--rw-r--r--   0        0        0       65 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/resources/test_suite_runs/__init__.py
--rw-r--r--   0        0        0    18728 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/resources/test_suite_runs/client.py
--rw-r--r--   0        0        0       65 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/resources/test_suites/__init__.py
--rw-r--r--   0        0        0    18982 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/resources/test_suites/client.py
--rw-r--r--   0        0        0      173 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/resources/workflow_deployments/__init__.py
--rw-r--r--   0        0        0    11158 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/resources/workflow_deployments/client.py
--rw-r--r--   0        0        0      208 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/resources/workflow_deployments/types/__init__.py
--rw-r--r--   0        0        0      182 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/resources/workflow_deployments/types/workflow_deployments_list_request_status.py
--rw-r--r--   0        0        0      454 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/terraform/__init__.py
--rw-r--r--   0        0        0      473 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/terraform/_jsii/__init__.py
--rw-r--r--   0        0        0    15887 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/terraform/_jsii/vellum-ai_vellum@0.0.0.jsii.tgz
--rw-r--r--   0        0        0       43 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/terraform/constraints.json
--rw-r--r--   0        0        0    21484 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/terraform/data_vellum_document_index/__init__.py
--rw-r--r--   0        0        0    25018 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/terraform/document_index/__init__.py
--rw-r--r--   0        0        0    10298 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/terraform/provider/__init__.py
--rw-r--r--   0        0        0        1 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/terraform/py.typed
--rw-r--r--   0        0        0       56 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/terraform/versions.json
--rw-r--r--   0        0        0    47325 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/__init__.py
--rw-r--r--   0        0        0      983 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/api_node_result.py
--rw-r--r--   0        0        0     1161 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/api_node_result_data.py
--rw-r--r--   0        0        0     1030 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/array_chat_message_content.py
--rw-r--r--   0        0        0     1297 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/array_chat_message_content_item.py
--rw-r--r--   0        0        0     1421 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/array_chat_message_content_item_request.py
--rw-r--r--   0        0        0     1059 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/array_chat_message_content_request.py
--rw-r--r--   0        0        0      116 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/array_enum.py
--rw-r--r--   0        0        0     3002 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/array_variable_value_item.py
--rw-r--r--   0        0        0      129 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/chat_history_enum.py
--rw-r--r--   0        0        0     1121 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/chat_history_input_request.py
--rw-r--r--   0        0        0      945 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/chat_history_variable_value.py
--rw-r--r--   0        0        0     1213 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/chat_message.py
--rw-r--r--   0        0        0     1573 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/chat_message_content.py
--rw-r--r--   0        0        0     1737 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/chat_message_content_request.py
--rw-r--r--   0        0        0     1242 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/chat_message_request.py
--rw-r--r--   0        0        0      182 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/chat_message_role.py
--rw-r--r--   0        0        0      996 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/code_execution_node_array_result.py
--rw-r--r--   0        0        0      967 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/code_execution_node_chat_history_result.py
--rw-r--r--   0        0        0      948 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/code_execution_node_error_result.py
--rw-r--r--   0        0        0      958 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/code_execution_node_function_call_result.py
--rw-r--r--   0        0        0      926 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/code_execution_node_json_result.py
--rw-r--r--   0        0        0      905 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/code_execution_node_number_result.py
--rw-r--r--   0        0        0     1034 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/code_execution_node_result.py
--rw-r--r--   0        0        0     1016 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/code_execution_node_result_data.py
--rw-r--r--   0        0        0     3377 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/code_execution_node_result_output.py
--rw-r--r--   0        0        0      972 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/code_execution_node_search_results_result.py
--rw-r--r--   0        0        0      903 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/code_execution_node_string_result.py
--rw-r--r--   0        0        0     1022 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/conditional_node_result.py
--rw-r--r--   0        0        0      898 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/conditional_node_result_data.py
--rw-r--r--   0        0        0      898 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/deployment_provider_payload_response.py
--rw-r--r--   0        0        0     1938 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/deployment_read.py
--rw-r--r--   0        0        0     1532 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/document_document_to_document_index.py
--rw-r--r--   0        0        0     1783 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/document_index_read.py
--rw-r--r--   0        0        0     2200 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/document_read.py
--rw-r--r--   0        0        0      122 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/document_status.py
--rw-r--r--   0        0        0     2108 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/enriched_normalized_completion.py
--rw-r--r--   0        0        0      158 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/entity_status.py
--rw-r--r--   0        0        0      179 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/environment_enum.py
--rw-r--r--   0        0        0      116 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/error_enum.py
--rw-r--r--   0        0        0      926 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/error_variable_value.py
--rw-r--r--   0        0        0      948 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/execute_prompt_api_error_response.py
--rw-r--r--   0        0        0     1636 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/execute_prompt_event.py
--rw-r--r--   0        0        0      914 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/execute_prompt_response.py
--rw-r--r--   0        0        0      947 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/execute_workflow_error_response.py
--rw-r--r--   0        0        0     1085 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/execute_workflow_response.py
--rw-r--r--   0        0        0      953 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/execute_workflow_stream_error_response.py
--rw-r--r--   0        0        0     1067 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/execute_workflow_workflow_result_event.py
--rw-r--r--   0        0        0     1099 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/execution_array_vellum_value.py
--rw-r--r--   0        0        0     1070 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/execution_chat_history_vellum_value.py
--rw-r--r--   0        0        0     1051 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/execution_error_vellum_value.py
--rw-r--r--   0        0        0     1061 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/execution_function_call_vellum_value.py
--rw-r--r--   0        0        0     1029 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/execution_json_vellum_value.py
--rw-r--r--   0        0        0     1008 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/execution_number_vellum_value.py
--rw-r--r--   0        0        0     1075 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/execution_search_results_vellum_value.py
--rw-r--r--   0        0        0     1006 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/execution_string_vellum_value.py
--rw-r--r--   0        0        0     3144 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/execution_vellum_value.py
--rw-r--r--   0        0        0     1125 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/external_test_case_execution.py
--rw-r--r--   0        0        0     1154 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/external_test_case_execution_request.py
--rw-r--r--   0        0        0      169 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/finish_reason_enum.py
--rw-r--r--   0        0        0      124 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/fulfilled_enum.py
--rw-r--r--   0        0        0     1235 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/fulfilled_execute_prompt_event.py
--rw-r--r--   0        0        0     1457 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/fulfilled_execute_prompt_response.py
--rw-r--r--   0        0        0     1089 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/fulfilled_execute_workflow_workflow_result_event.py
--rw-r--r--   0        0        0      999 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/fulfilled_function_call.py
--rw-r--r--   0        0        0     1073 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/fulfilled_function_call_request.py
--rw-r--r--   0        0        0     1228 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/fulfilled_prompt_execution_meta.py
--rw-r--r--   0        0        0     1373 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/fulfilled_workflow_node_result_event.py
--rw-r--r--   0        0        0      813 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/function_call.py
--rw-r--r--   0        0        0     1065 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/function_call_chat_message_content.py
--rw-r--r--   0        0        0     1094 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/function_call_chat_message_content_request.py
--rw-r--r--   0        0        0     1013 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/function_call_chat_message_content_value.py
--rw-r--r--   0        0        0     1020 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/function_call_chat_message_content_value_request.py
--rw-r--r--   0        0        0      131 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/function_call_enum.py
--rw-r--r--   0        0        0      912 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/function_call_variable_value.py
--rw-r--r--   0        0        0      940 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/generate_error_response.py
--rw-r--r--   0        0        0     1079 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/generate_options_request.py
--rw-r--r--   0        0        0     1572 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/generate_request.py
--rw-r--r--   0        0        0     1342 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/generate_response.py
--rw-r--r--   0        0        0     1394 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/generate_result.py
--rw-r--r--   0        0        0     1087 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/generate_result_data.py
--rw-r--r--   0        0        0      949 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/generate_result_error.py
--rw-r--r--   0        0        0      934 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/generate_stream_response.py
--rw-r--r--   0        0        0     1101 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/generate_stream_result.py
--rw-r--r--   0        0        0      991 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/generate_stream_result_data.py
--rw-r--r--   0        0        0      975 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/image_chat_message_content.py
--rw-r--r--   0        0        0     1004 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/image_chat_message_content_request.py
--rw-r--r--   0        0        0      116 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/image_enum.py
--rw-r--r--   0        0        0     1000 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/image_variable_value.py
--rw-r--r--   0        0        0      213 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/indexing_state_enum.py
--rw-r--r--   0        0        0      124 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/initiated_enum.py
--rw-r--r--   0        0        0     1134 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/initiated_execute_prompt_event.py
--rw-r--r--   0        0        0     1181 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/initiated_prompt_execution_meta.py
--rw-r--r--   0        0        0     1377 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/initiated_workflow_node_result_event.py
--rw-r--r--   0        0        0      114 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/json_enum.py
--rw-r--r--   0        0        0     1048 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/json_input_request.py
--rw-r--r--   0        0        0      904 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/json_variable_value.py
--rw-r--r--   0        0        0      487 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/logical_operator.py
--rw-r--r--   0        0        0      151 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/logprobs_enum.py
--rw-r--r--   0        0        0     1355 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/metadata_filter_config_request.py
--rw-r--r--   0        0        0      165 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/metadata_filter_rule_combinator.py
--rw-r--r--   0        0        0     1371 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/metadata_filter_rule_request.py
--rw-r--r--   0        0        0     1086 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/ml_model_usage.py
--rw-r--r--   0        0        0     1098 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/named_scenario_input_chat_history_variable_value_request.py
--rw-r--r--   0        0        0     1043 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/named_scenario_input_request.py
--rw-r--r--   0        0        0     1006 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/named_scenario_input_string_variable_value_request.py
--rw-r--r--   0        0        0     1044 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/named_test_case_chat_history_variable_value.py
--rw-r--r--   0        0        0     1073 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/named_test_case_chat_history_variable_value_request.py
--rw-r--r--   0        0        0     1018 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/named_test_case_error_variable_value.py
--rw-r--r--   0        0        0     1047 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/named_test_case_error_variable_value_request.py
--rw-r--r--   0        0        0     1064 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/named_test_case_function_call_variable_value.py
--rw-r--r--   0        0        0     1093 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/named_test_case_function_call_variable_value_request.py
--rw-r--r--   0        0        0      995 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/named_test_case_json_variable_value.py
--rw-r--r--   0        0        0     1002 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/named_test_case_json_variable_value_request.py
--rw-r--r--   0        0        0      976 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/named_test_case_number_variable_value.py
--rw-r--r--   0        0        0      983 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/named_test_case_number_variable_value_request.py
--rw-r--r--   0        0        0     1051 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/named_test_case_search_results_variable_value.py
--rw-r--r--   0        0        0     1080 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/named_test_case_search_results_variable_value_request.py
--rw-r--r--   0        0        0      974 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/named_test_case_string_variable_value.py
--rw-r--r--   0        0        0      981 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/named_test_case_string_variable_value_request.py
--rw-r--r--   0        0        0     3021 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/named_test_case_variable_value.py
--rw-r--r--   0        0        0     3280 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/named_test_case_variable_value_request.py
--rw-r--r--   0        0        0     1019 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/node_input_compiled_array_value.py
--rw-r--r--   0        0        0      990 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/node_input_compiled_chat_history_value.py
--rw-r--r--   0        0        0      971 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/node_input_compiled_error_value.py
--rw-r--r--   0        0        0      976 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/node_input_compiled_function_call.py
--rw-r--r--   0        0        0      949 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/node_input_compiled_json_value.py
--rw-r--r--   0        0        0      928 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/node_input_compiled_number_value.py
--rw-r--r--   0        0        0      995 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/node_input_compiled_search_results_value.py
--rw-r--r--   0        0        0      926 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/node_input_compiled_string_value.py
--rw-r--r--   0        0        0     3354 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/node_input_variable_compiled_value.py
--rw-r--r--   0        0        0     1008 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/node_output_compiled_array_value.py
--rw-r--r--   0        0        0      979 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/node_output_compiled_chat_history_value.py
--rw-r--r--   0        0        0      960 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/node_output_compiled_error_value.py
--rw-r--r--   0        0        0      966 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/node_output_compiled_function_value.py
--rw-r--r--   0        0        0      938 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/node_output_compiled_json_value.py
--rw-r--r--   0        0        0      917 2024-04-25 18:57:02.586595 vellum_ai-0.5.1/src/vellum/types/node_output_compiled_number_value.py
--rw-r--r--   0        0        0      984 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/node_output_compiled_search_results_value.py
--rw-r--r--   0        0        0      915 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/node_output_compiled_string_value.py
--rw-r--r--   0        0        0     3262 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/node_output_compiled_value.py
--rw-r--r--   0        0        0     1000 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/normalized_log_probs.py
--rw-r--r--   0        0        0     1008 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/normalized_token_log_probs.py
--rw-r--r--   0        0        0      118 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/number_enum.py
--rw-r--r--   0        0        0      883 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/number_variable_value.py
--rw-r--r--   0        0        0     1091 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/paginated_document_index_read_list.py
--rw-r--r--   0        0        0     1095 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/paginated_slim_deployment_read_list.py
--rw-r--r--   0        0        0     1070 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/paginated_slim_document_list.py
--rw-r--r--   0        0        0     1111 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/paginated_slim_workflow_deployment_list.py
--rw-r--r--   0        0        0     1060 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/paginated_test_suite_run_execution_list.py
--rw-r--r--   0        0        0     1044 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/paginated_test_suite_test_case_list.py
--rw-r--r--   0        0        0      195 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/processing_failure_reason_enum.py
--rw-r--r--   0        0        0      190 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/processing_state_enum.py
--rw-r--r--   0        0        0     2044 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/prompt_deployment_expand_meta_request_request.py
--rw-r--r--   0        0        0     1233 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/prompt_deployment_input_request.py
--rw-r--r--   0        0        0     1370 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/prompt_execution_meta.py
--rw-r--r--   0        0        0      997 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/prompt_node_result.py
--rw-r--r--   0        0        0      988 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/prompt_node_result_data.py
--rw-r--r--   0        0        0     1442 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/prompt_output.py
--rw-r--r--   0        0        0     1210 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/raw_prompt_execution_overrides_request.py
--rw-r--r--   0        0        0      122 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/rejected_enum.py
--rw-r--r--   0        0        0     1159 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/rejected_execute_prompt_event.py
--rw-r--r--   0        0        0     1417 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/rejected_execute_prompt_response.py
--rw-r--r--   0        0        0     1103 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/rejected_execute_workflow_workflow_result_event.py
--rw-r--r--   0        0        0     1038 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/rejected_function_call.py
--rw-r--r--   0        0        0     1138 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/rejected_prompt_execution_meta.py
--rw-r--r--   0        0        0     1293 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/rejected_workflow_node_result_event.py
--rw-r--r--   0        0        0     1144 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/sandbox_scenario.py
--rw-r--r--   0        0        0      907 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/scenario_input.py
--rw-r--r--   0        0        0     1071 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/scenario_input_chat_history_variable_value.py
--rw-r--r--   0        0        0     1001 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/scenario_input_string_variable_value.py
--rw-r--r--   0        0        0      938 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/search_error_response.py
--rw-r--r--   0        0        0     1218 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/search_filters_request.py
--rw-r--r--   0        0        0      997 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/search_node_result.py
--rw-r--r--   0        0        0     1143 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/search_node_result_data.py
--rw-r--r--   0        0        0     1622 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/search_request_options_request.py
--rw-r--r--   0        0        0     1047 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/search_response.py
--rw-r--r--   0        0        0     1304 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/search_result.py
--rw-r--r--   0        0        0     1437 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/search_result_document.py
--rw-r--r--   0        0        0     1365 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/search_result_document_request.py
--rw-r--r--   0        0        0      972 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/search_result_merging_request.py
--rw-r--r--   0        0        0     1333 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/search_result_request.py
--rw-r--r--   0        0        0      133 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/search_results_enum.py
--rw-r--r--   0        0        0      950 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/search_results_variable_value.py
--rw-r--r--   0        0        0     1128 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/search_weights_request.py
--rw-r--r--   0        0        0     1753 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/slim_deployment_read.py
--rw-r--r--   0        0        0     2975 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/slim_document.py
--rw-r--r--   0        0        0     2104 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/slim_workflow_deployment.py
--rw-r--r--   0        0        0      124 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/streaming_enum.py
--rw-r--r--   0        0        0     1388 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/streaming_execute_prompt_event.py
--rw-r--r--   0        0        0     1030 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/streaming_prompt_execution_meta.py
--rw-r--r--   0        0        0     1383 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/streaming_workflow_node_result_event.py
--rw-r--r--   0        0        0      930 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/string_chat_message_content.py
--rw-r--r--   0        0        0      937 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/string_chat_message_content_request.py
--rw-r--r--   0        0        0      118 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/string_enum.py
--rw-r--r--   0        0        0     1026 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/string_input_request.py
--rw-r--r--   0        0        0      881 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/string_variable_value.py
--rw-r--r--   0        0        0     1825 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/submit_completion_actual_request.py
--rw-r--r--   0        0        0      875 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/submit_completion_actuals_error_response.py
--rw-r--r--   0        0        0     1487 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/submit_workflow_execution_actual_request.py
--rw-r--r--   0        0        0      128 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/subworkflow_enum.py
--rw-r--r--   0        0        0      917 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/subworkflow_node_result.py
--rw-r--r--   0        0        0      993 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/templating_node_array_result.py
--rw-r--r--   0        0        0      964 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/templating_node_chat_history_result.py
--rw-r--r--   0        0        0      945 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/templating_node_error_result.py
--rw-r--r--   0        0        0      955 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/templating_node_function_call_result.py
--rw-r--r--   0        0        0      923 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/templating_node_json_result.py
--rw-r--r--   0        0        0      902 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/templating_node_number_result.py
--rw-r--r--   0        0        0     1017 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/templating_node_result.py
--rw-r--r--   0        0        0      956 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/templating_node_result_data.py
--rw-r--r--   0        0        0     3246 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/templating_node_result_output.py
--rw-r--r--   0        0        0      969 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/templating_node_search_results_result.py
--rw-r--r--   0        0        0      900 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/templating_node_string_result.py
--rw-r--r--   0        0        0     1142 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/terminal_node_array_result.py
--rw-r--r--   0        0        0     1113 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/terminal_node_chat_history_result.py
--rw-r--r--   0        0        0     1094 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/terminal_node_error_result.py
--rw-r--r--   0        0        0     1104 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/terminal_node_function_call_result.py
--rw-r--r--   0        0        0     1072 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/terminal_node_json_result.py
--rw-r--r--   0        0        0     1051 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/terminal_node_number_result.py
--rw-r--r--   0        0        0     1007 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/terminal_node_result.py
--rw-r--r--   0        0        0      948 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/terminal_node_result_data.py
--rw-r--r--   0        0        0     3164 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/terminal_node_result_output.py
--rw-r--r--   0        0        0     1118 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/terminal_node_search_results_result.py
--rw-r--r--   0        0        0     1049 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/terminal_node_string_result.py
--rw-r--r--   0        0        0     1061 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_case_chat_history_variable_value.py
--rw-r--r--   0        0        0     1036 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_case_error_variable_value.py
--rw-r--r--   0        0        0     1081 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_case_function_call_variable_value.py
--rw-r--r--   0        0        0     1012 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_case_json_variable_value.py
--rw-r--r--   0        0        0      996 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_case_number_variable_value.py
--rw-r--r--   0        0        0     1068 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_case_search_results_variable_value.py
--rw-r--r--   0        0        0      991 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_case_string_variable_value.py
--rw-r--r--   0        0        0     2834 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_case_variable_value.py
--rw-r--r--   0        0        0     1373 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_suite_run_deployment_release_tag_exec_config.py
--rw-r--r--   0        0        0     1228 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_data.py
--rw-r--r--   0        0        0     1235 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_data_request.py
--rw-r--r--   0        0        0     1411 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_request.py
--rw-r--r--   0        0        0      174 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_type_enum.py
--rw-r--r--   0        0        0     1483 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_suite_run_exec_config.py
--rw-r--r--   0        0        0     1598 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_suite_run_exec_config_request.py
--rw-r--r--   0        0        0     1158 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_suite_run_execution.py
--rw-r--r--   0        0        0     1115 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_suite_run_execution_chat_history_output.py
--rw-r--r--   0        0        0     1089 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_suite_run_execution_error_output.py
--rw-r--r--   0        0        0     1135 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_suite_run_execution_function_call_output.py
--rw-r--r--   0        0        0     1066 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_suite_run_execution_json_output.py
--rw-r--r--   0        0        0      973 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_suite_run_execution_metric_definition.py
--rw-r--r--   0        0        0     1218 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_suite_run_execution_metric_result.py
--rw-r--r--   0        0        0     1047 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_suite_run_execution_number_output.py
--rw-r--r--   0        0        0     3057 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_suite_run_execution_output.py
--rw-r--r--   0        0        0     1122 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_suite_run_execution_search_results_output.py
--rw-r--r--   0        0        0     1045 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_suite_run_execution_string_output.py
--rw-r--r--   0        0        0     1331 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_suite_run_external_exec_config.py
--rw-r--r--   0        0        0     1115 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_suite_run_external_exec_config_data.py
--rw-r--r--   0        0        0     1144 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_suite_run_external_exec_config_data_request.py
--rw-r--r--   0        0        0     1360 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_suite_run_external_exec_config_request.py
--rw-r--r--   0        0        0      148 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_suite_run_external_exec_config_type_enum.py
--rw-r--r--   0        0        0     1005 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_suite_run_metric_error_output.py
--rw-r--r--   0        0        0      144 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_suite_run_metric_error_output_type_enum.py
--rw-r--r--   0        0        0      963 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_suite_run_metric_number_output.py
--rw-r--r--   0        0        0      146 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_suite_run_metric_number_output_type_enum.py
--rw-r--r--   0        0        0     1291 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_suite_run_metric_output.py
--rw-r--r--   0        0        0      961 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_suite_run_metric_string_output.py
--rw-r--r--   0        0        0      146 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_suite_run_metric_string_output_type_enum.py
--rw-r--r--   0        0        0     1500 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_suite_run_read.py
--rw-r--r--   0        0        0      197 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_suite_run_state.py
--rw-r--r--   0        0        0      896 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_suite_run_test_suite.py
--rw-r--r--   0        0        0     1367 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_suite_run_workflow_release_tag_exec_config.py
--rw-r--r--   0        0        0     1241 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_data.py
--rw-r--r--   0        0        0     1248 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_data_request.py
--rw-r--r--   0        0        0     1405 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_request.py
--rw-r--r--   0        0        0      170 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_type_enum.py
--rw-r--r--   0        0        0     1086 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/test_suite_test_case.py
--rw-r--r--   0        0        0      866 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/upload_document_error_response.py
--rw-r--r--   0        0        0      946 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/upload_document_response.py
--rw-r--r--   0        0        0      937 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/vellum_error.py
--rw-r--r--   0        0        0      233 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/vellum_error_code_enum.py
--rw-r--r--   0        0        0      944 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/vellum_error_request.py
--rw-r--r--   0        0        0      914 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/vellum_image.py
--rw-r--r--   0        0        0      921 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/vellum_image_request.py
--rw-r--r--   0        0        0      944 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/vellum_variable.py
--rw-r--r--   0        0        0      281 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/vellum_variable_type.py
--rw-r--r--   0        0        0     2110 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/workflow_deployment_read.py
--rw-r--r--   0        0        0      981 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/workflow_event_error.py
--rw-r--r--   0        0        0     2038 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/workflow_execution_actual_chat_history_request.py
--rw-r--r--   0        0        0     1975 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/workflow_execution_actual_json_request.py
--rw-r--r--   0        0        0     1952 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/workflow_execution_actual_string_request.py
--rw-r--r--   0        0        0      425 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/workflow_execution_event_error_code.py
--rw-r--r--   0        0        0      170 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/workflow_execution_event_type.py
--rw-r--r--   0        0        0     1139 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/workflow_execution_node_result_event.py
--rw-r--r--   0        0        0     1134 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/workflow_execution_workflow_result_event.py
--rw-r--r--   0        0        0     2966 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/workflow_node_result_data.py
--rw-r--r--   0        0        0     1745 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/workflow_node_result_event.py
--rw-r--r--   0        0        0      209 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/workflow_node_result_event_state.py
--rw-r--r--   0        0        0     3212 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/workflow_output.py
--rw-r--r--   0        0        0     1154 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/workflow_output_array.py
--rw-r--r--   0        0        0     1131 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/workflow_output_chat_history.py
--rw-r--r--   0        0        0     1106 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/workflow_output_error.py
--rw-r--r--   0        0        0     1123 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/workflow_output_function_call.py
--rw-r--r--   0        0        0     1106 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/workflow_output_image.py
--rw-r--r--   0        0        0     1082 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/workflow_output_json.py
--rw-r--r--   0        0        0     1063 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/workflow_output_number.py
--rw-r--r--   0        0        0     1138 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/workflow_output_search_results.py
--rw-r--r--   0        0        0     1061 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/workflow_output_string.py
--rw-r--r--   0        0        0     1137 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/workflow_request_chat_history_input_request.py
--rw-r--r--   0        0        0     1772 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/workflow_request_input_request.py
--rw-r--r--   0        0        0     1066 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/workflow_request_json_input_request.py
--rw-r--r--   0        0        0     1047 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/workflow_request_number_input_request.py
--rw-r--r--   0        0        0     1045 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/workflow_request_string_input_request.py
--rw-r--r--   0        0        0     1475 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/workflow_result_event.py
--rw-r--r--   0        0        0     3529 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/workflow_result_event_output_data.py
--rw-r--r--   0        0        0     1423 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/workflow_result_event_output_data_array.py
--rw-r--r--   0        0        0     1400 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/workflow_result_event_output_data_chat_history.py
--rw-r--r--   0        0        0     1375 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/workflow_result_event_output_data_error.py
--rw-r--r--   0        0        0     1392 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/workflow_result_event_output_data_function_call.py
--rw-r--r--   0        0        0     1351 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/workflow_result_event_output_data_json.py
--rw-r--r--   0        0        0     1332 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/workflow_result_event_output_data_number.py
--rw-r--r--   0        0        0     1407 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/workflow_result_event_output_data_search_results.py
--rw-r--r--   0        0        0     1482 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/workflow_result_event_output_data_string.py
--rw-r--r--   0        0        0      911 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/types/workflow_stream_event.py
--rw-r--r--   0        0        0       77 2024-04-25 18:57:02.590595 vellum_ai-0.5.1/src/vellum/version.py
--rw-r--r--   0        0        0     3549 1970-01-01 00:00:00.000000 vellum_ai-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/LICENSE
+-rw-r--r--   0        0        0     2980 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/README.md
+-rw-r--r--   0        0        0      632 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0    35797 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/__init__.py
+-rw-r--r--   0        0        0    97089 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/client.py
+-rw-r--r--   0        0        0      853 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/core/api_error.py
+-rw-r--r--   0        0        0     1697 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/core/file.py
+-rw-r--r--   0        0        0     5059 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      329 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/core/request_options.py
+-rw-r--r--   0        0        0      498 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/environment.py
+-rw-r--r--   0        0        0      343 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/errors/__init__.py
+-rw-r--r--   0        0        0      248 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/errors/bad_request_error.py
+-rw-r--r--   0        0        0      247 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/errors/forbidden_error.py
+-rw-r--r--   0        0        0      252 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/errors/internal_server_error.py
+-rw-r--r--   0        0        0      246 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/errors/not_found_error.py
+-rw-r--r--   0        0        0       79 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/lib/__init__.py
+-rw-r--r--   0        0        0       77 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/lib/test_suites/__init__.py
+-rw-r--r--   0        0        0      116 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/lib/test_suites/constants.py
+-rw-r--r--   0        0        0       56 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/lib/test_suites/exceptions.py
+-rw-r--r--   0        0        0    12323 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/lib/test_suites/resources.py
+-rw-r--r--   0        0        0        0 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/lib/utils/__init__.py
+-rw-r--r--   0        0        0      298 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/lib/utils/env.py
+-rw-r--r--   0        0        0       49 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/lib/utils/exceptions.py
+-rw-r--r--   0        0        0      698 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/lib/utils/paginator.py
+-rw-r--r--   0        0        0        0 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/py.typed
+-rw-r--r--   0        0        0      730 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/__init__.py
+-rw-r--r--   0        0        0      157 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/deployments/__init__.py
+-rw-r--r--   0        0        0    19588 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/deployments/client.py
+-rw-r--r--   0        0        0      183 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/deployments/types/__init__.py
+-rw-r--r--   0        0        0      174 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/deployments/types/deployments_list_request_status.py
+-rw-r--r--   0        0        0      165 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/document_indexes/__init__.py
+-rw-r--r--   0        0        0    39845 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/document_indexes/client.py
+-rw-r--r--   0        0        0      196 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/document_indexes/types/__init__.py
+-rw-r--r--   0        0        0      178 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/document_indexes/types/document_indexes_list_request_status.py
+-rw-r--r--   0        0        0       65 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/documents/__init__.py
+-rw-r--r--   0        0        0    34010 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/documents/client.py
+-rw-r--r--   0        0        0       65 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/folder_entities/__init__.py
+-rw-r--r--   0        0        0     6435 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/folder_entities/client.py
+-rw-r--r--   0        0        0       65 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/sandboxes/__init__.py
+-rw-r--r--   0        0        0    12738 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/sandboxes/client.py
+-rw-r--r--   0        0        0       65 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/test_suite_runs/__init__.py
+-rw-r--r--   0        0        0    18728 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/test_suite_runs/client.py
+-rw-r--r--   0        0        0       65 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/test_suites/__init__.py
+-rw-r--r--   0        0        0    18982 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/test_suites/client.py
+-rw-r--r--   0        0        0      173 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/workflow_deployments/__init__.py
+-rw-r--r--   0        0        0    11158 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/workflow_deployments/client.py
+-rw-r--r--   0        0        0      208 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/workflow_deployments/types/__init__.py
+-rw-r--r--   0        0        0      182 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/workflow_deployments/types/workflow_deployments_list_request_status.py
+-rw-r--r--   0        0        0      454 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/terraform/__init__.py
+-rw-r--r--   0        0        0      473 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/terraform/_jsii/__init__.py
+-rw-r--r--   0        0        0    15887 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/terraform/_jsii/vellum-ai_vellum@0.0.0.jsii.tgz
+-rw-r--r--   0        0        0       43 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/terraform/constraints.json
+-rw-r--r--   0        0        0    21484 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/terraform/data_vellum_document_index/__init__.py
+-rw-r--r--   0        0        0    25018 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/terraform/document_index/__init__.py
+-rw-r--r--   0        0        0    10298 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/terraform/provider/__init__.py
+-rw-r--r--   0        0        0        1 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/terraform/py.typed
+-rw-r--r--   0        0        0       56 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/terraform/versions.json
+-rw-r--r--   0        0        0    47652 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/types/__init__.py
+-rw-r--r--   0        0        0      983 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/types/api_node_result.py
+-rw-r--r--   0        0        0     1161 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/types/api_node_result_data.py
+-rw-r--r--   0        0        0     1030 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/types/array_chat_message_content.py
+-rw-r--r--   0        0        0     1297 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/types/array_chat_message_content_item.py
+-rw-r--r--   0        0        0     1421 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/types/array_chat_message_content_item_request.py
+-rw-r--r--   0        0        0     1059 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/types/array_chat_message_content_request.py
+-rw-r--r--   0        0        0      116 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/types/array_enum.py
+-rw-r--r--   0        0        0     3002 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/types/array_variable_value_item.py
+-rw-r--r--   0        0        0      129 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/types/chat_history_enum.py
+-rw-r--r--   0        0        0     1121 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/types/chat_history_input_request.py
+-rw-r--r--   0        0        0      945 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/types/chat_history_variable_value.py
+-rw-r--r--   0        0        0     1213 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/types/chat_message.py
+-rw-r--r--   0        0        0     1573 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/types/chat_message_content.py
+-rw-r--r--   0        0        0     1737 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/chat_message_content_request.py
+-rw-r--r--   0        0        0     1242 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/chat_message_request.py
+-rw-r--r--   0        0        0      182 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/chat_message_role.py
+-rw-r--r--   0        0        0      996 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/code_execution_node_array_result.py
+-rw-r--r--   0        0        0      967 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/code_execution_node_chat_history_result.py
+-rw-r--r--   0        0        0      948 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/code_execution_node_error_result.py
+-rw-r--r--   0        0        0      958 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/code_execution_node_function_call_result.py
+-rw-r--r--   0        0        0      926 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/code_execution_node_json_result.py
+-rw-r--r--   0        0        0      905 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/code_execution_node_number_result.py
+-rw-r--r--   0        0        0     1034 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/code_execution_node_result.py
+-rw-r--r--   0        0        0     1016 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/code_execution_node_result_data.py
+-rw-r--r--   0        0        0     3377 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/code_execution_node_result_output.py
+-rw-r--r--   0        0        0      972 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/code_execution_node_search_results_result.py
+-rw-r--r--   0        0        0      903 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/code_execution_node_string_result.py
+-rw-r--r--   0        0        0     1022 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/conditional_node_result.py
+-rw-r--r--   0        0        0      898 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/conditional_node_result_data.py
+-rw-r--r--   0        0        0      898 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/deployment_provider_payload_response.py
+-rw-r--r--   0        0        0     1938 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/deployment_read.py
+-rw-r--r--   0        0        0     1532 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/document_document_to_document_index.py
+-rw-r--r--   0        0        0     1783 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/document_index_read.py
+-rw-r--r--   0        0        0     2200 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/document_read.py
+-rw-r--r--   0        0        0      122 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/document_status.py
+-rw-r--r--   0        0        0     2108 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/enriched_normalized_completion.py
+-rw-r--r--   0        0        0      158 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/entity_status.py
+-rw-r--r--   0        0        0      179 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/environment_enum.py
+-rw-r--r--   0        0        0      116 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/error_enum.py
+-rw-r--r--   0        0        0      926 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/error_variable_value.py
+-rw-r--r--   0        0        0      976 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/error_vellum_value.py
+-rw-r--r--   0        0        0      948 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/execute_prompt_api_error_response.py
+-rw-r--r--   0        0        0     1636 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/execute_prompt_event.py
+-rw-r--r--   0        0        0      914 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/execute_prompt_response.py
+-rw-r--r--   0        0        0      947 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/execute_workflow_error_response.py
+-rw-r--r--   0        0        0     1085 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/execute_workflow_response.py
+-rw-r--r--   0        0        0      953 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/execute_workflow_stream_error_response.py
+-rw-r--r--   0        0        0     1067 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/execute_workflow_workflow_result_event.py
+-rw-r--r--   0        0        0     1099 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/execution_array_vellum_value.py
+-rw-r--r--   0        0        0     1070 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/execution_chat_history_vellum_value.py
+-rw-r--r--   0        0        0     1051 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/execution_error_vellum_value.py
+-rw-r--r--   0        0        0     1061 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/execution_function_call_vellum_value.py
+-rw-r--r--   0        0        0     1029 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/execution_json_vellum_value.py
+-rw-r--r--   0        0        0     1008 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/execution_number_vellum_value.py
+-rw-r--r--   0        0        0     1075 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/execution_search_results_vellum_value.py
+-rw-r--r--   0        0        0     1006 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/execution_string_vellum_value.py
+-rw-r--r--   0        0        0     3144 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/execution_vellum_value.py
+-rw-r--r--   0        0        0     1125 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/external_test_case_execution.py
+-rw-r--r--   0        0        0     1154 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/external_test_case_execution_request.py
+-rw-r--r--   0        0        0      169 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/finish_reason_enum.py
+-rw-r--r--   0        0        0      124 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/fulfilled_enum.py
+-rw-r--r--   0        0        0     1235 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/fulfilled_execute_prompt_event.py
+-rw-r--r--   0        0        0     1457 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/fulfilled_execute_prompt_response.py
+-rw-r--r--   0        0        0     1089 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/fulfilled_execute_workflow_workflow_result_event.py
+-rw-r--r--   0        0        0      999 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/fulfilled_function_call.py
+-rw-r--r--   0        0        0     1073 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/fulfilled_function_call_request.py
+-rw-r--r--   0        0        0     1228 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/fulfilled_prompt_execution_meta.py
+-rw-r--r--   0        0        0     1373 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/fulfilled_workflow_node_result_event.py
+-rw-r--r--   0        0        0      813 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/function_call.py
+-rw-r--r--   0        0        0     1065 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/function_call_chat_message_content.py
+-rw-r--r--   0        0        0     1094 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/function_call_chat_message_content_request.py
+-rw-r--r--   0        0        0     1013 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/function_call_chat_message_content_value.py
+-rw-r--r--   0        0        0     1020 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/function_call_chat_message_content_value_request.py
+-rw-r--r--   0        0        0      131 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/function_call_enum.py
+-rw-r--r--   0        0        0      936 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/function_call_variable_value.py
+-rw-r--r--   0        0        0      969 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/function_call_vellum_value.py
+-rw-r--r--   0        0        0      940 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/generate_error_response.py
+-rw-r--r--   0        0        0     1079 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/generate_options_request.py
+-rw-r--r--   0        0        0     1572 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/generate_request.py
+-rw-r--r--   0        0        0     1342 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/generate_response.py
+-rw-r--r--   0        0        0     1394 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/generate_result.py
+-rw-r--r--   0        0        0     1087 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/generate_result_data.py
+-rw-r--r--   0        0        0      949 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/generate_result_error.py
+-rw-r--r--   0        0        0      934 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/generate_stream_response.py
+-rw-r--r--   0        0        0     1101 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/generate_stream_result.py
+-rw-r--r--   0        0        0      991 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/generate_stream_result_data.py
+-rw-r--r--   0        0        0      975 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/image_chat_message_content.py
+-rw-r--r--   0        0        0     1004 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/image_chat_message_content_request.py
+-rw-r--r--   0        0        0      116 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/image_enum.py
+-rw-r--r--   0        0        0     1000 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/image_variable_value.py
+-rw-r--r--   0        0        0      213 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/indexing_state_enum.py
+-rw-r--r--   0        0        0      124 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/initiated_enum.py
+-rw-r--r--   0        0        0     1134 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/initiated_execute_prompt_event.py
+-rw-r--r--   0        0        0     1181 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/initiated_prompt_execution_meta.py
+-rw-r--r--   0        0        0     1377 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/initiated_workflow_node_result_event.py
+-rw-r--r--   0        0        0      114 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/json_enum.py
+-rw-r--r--   0        0        0     1048 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/json_input_request.py
+-rw-r--r--   0        0        0      904 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/json_variable_value.py
+-rw-r--r--   0        0        0      959 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/json_vellum_value.py
+-rw-r--r--   0        0        0      487 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/logical_operator.py
+-rw-r--r--   0        0        0      151 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/logprobs_enum.py
+-rw-r--r--   0        0        0     1355 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/metadata_filter_config_request.py
+-rw-r--r--   0        0        0      165 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/metadata_filter_rule_combinator.py
+-rw-r--r--   0        0        0     1371 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/metadata_filter_rule_request.py
+-rw-r--r--   0        0        0     1086 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/ml_model_usage.py
+-rw-r--r--   0        0        0     1098 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/named_scenario_input_chat_history_variable_value_request.py
+-rw-r--r--   0        0        0     1043 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/named_scenario_input_request.py
+-rw-r--r--   0        0        0     1006 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/named_scenario_input_string_variable_value_request.py
+-rw-r--r--   0        0        0     1044 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/named_test_case_chat_history_variable_value.py
+-rw-r--r--   0        0        0     1073 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/named_test_case_chat_history_variable_value_request.py
+-rw-r--r--   0        0        0     1018 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/named_test_case_error_variable_value.py
+-rw-r--r--   0        0        0     1047 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/named_test_case_error_variable_value_request.py
+-rw-r--r--   0        0        0     1064 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/named_test_case_function_call_variable_value.py
+-rw-r--r--   0        0        0     1093 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/named_test_case_function_call_variable_value_request.py
+-rw-r--r--   0        0        0      995 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/named_test_case_json_variable_value.py
+-rw-r--r--   0        0        0     1002 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/named_test_case_json_variable_value_request.py
+-rw-r--r--   0        0        0      976 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/named_test_case_number_variable_value.py
+-rw-r--r--   0        0        0      983 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/named_test_case_number_variable_value_request.py
+-rw-r--r--   0        0        0     1051 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/named_test_case_search_results_variable_value.py
+-rw-r--r--   0        0        0     1080 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/named_test_case_search_results_variable_value_request.py
+-rw-r--r--   0        0        0      974 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/named_test_case_string_variable_value.py
+-rw-r--r--   0        0        0      981 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/named_test_case_string_variable_value_request.py
+-rw-r--r--   0        0        0     3021 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/named_test_case_variable_value.py
+-rw-r--r--   0        0        0     3280 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/named_test_case_variable_value_request.py
+-rw-r--r--   0        0        0     1019 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/node_input_compiled_array_value.py
+-rw-r--r--   0        0        0      990 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/node_input_compiled_chat_history_value.py
+-rw-r--r--   0        0        0      971 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/node_input_compiled_error_value.py
+-rw-r--r--   0        0        0      976 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/node_input_compiled_function_call.py
+-rw-r--r--   0        0        0      949 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/node_input_compiled_json_value.py
+-rw-r--r--   0        0        0      928 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/node_input_compiled_number_value.py
+-rw-r--r--   0        0        0      995 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/node_input_compiled_search_results_value.py
+-rw-r--r--   0        0        0      926 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/node_input_compiled_string_value.py
+-rw-r--r--   0        0        0     3354 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/node_input_variable_compiled_value.py
+-rw-r--r--   0        0        0     1220 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/node_output_compiled_array_value.py
+-rw-r--r--   0        0        0     1198 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/node_output_compiled_chat_history_value.py
+-rw-r--r--   0        0        0     1172 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/node_output_compiled_error_value.py
+-rw-r--r--   0        0        0     1190 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/node_output_compiled_function_call_value.py
+-rw-r--r--   0        0        0     1149 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/node_output_compiled_json_value.py
+-rw-r--r--   0        0        0     1130 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/node_output_compiled_number_value.py
+-rw-r--r--   0        0        0     1205 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/node_output_compiled_search_results_value.py
+-rw-r--r--   0        0        0     1128 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/node_output_compiled_string_value.py
+-rw-r--r--   0        0        0     3275 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/node_output_compiled_value.py
+-rw-r--r--   0        0        0     1000 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/normalized_log_probs.py
+-rw-r--r--   0        0        0     1008 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/normalized_token_log_probs.py
+-rw-r--r--   0        0        0      118 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/number_enum.py
+-rw-r--r--   0        0        0      883 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/number_variable_value.py
+-rw-r--r--   0        0        0     1091 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/paginated_document_index_read_list.py
+-rw-r--r--   0        0        0     1095 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/paginated_slim_deployment_read_list.py
+-rw-r--r--   0        0        0     1070 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/paginated_slim_document_list.py
+-rw-r--r--   0        0        0     1111 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/paginated_slim_workflow_deployment_list.py
+-rw-r--r--   0        0        0     1060 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/paginated_test_suite_run_execution_list.py
+-rw-r--r--   0        0        0     1044 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/paginated_test_suite_test_case_list.py
+-rw-r--r--   0        0        0      195 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/processing_failure_reason_enum.py
+-rw-r--r--   0        0        0      190 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/processing_state_enum.py
+-rw-r--r--   0        0        0     2044 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/prompt_deployment_expand_meta_request_request.py
+-rw-r--r--   0        0        0     1233 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/prompt_deployment_input_request.py
+-rw-r--r--   0        0        0     1370 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/prompt_execution_meta.py
+-rw-r--r--   0        0        0      997 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/prompt_node_result.py
+-rw-r--r--   0        0        0      988 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/prompt_node_result_data.py
+-rw-r--r--   0        0        0     1418 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/prompt_output.py
+-rw-r--r--   0        0        0     1210 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/raw_prompt_execution_overrides_request.py
+-rw-r--r--   0        0        0      122 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/rejected_enum.py
+-rw-r--r--   0        0        0     1159 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/rejected_execute_prompt_event.py
+-rw-r--r--   0        0        0     1417 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/rejected_execute_prompt_response.py
+-rw-r--r--   0        0        0     1103 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/rejected_execute_workflow_workflow_result_event.py
+-rw-r--r--   0        0        0     1038 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/rejected_function_call.py
+-rw-r--r--   0        0        0     1138 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/rejected_prompt_execution_meta.py
+-rw-r--r--   0        0        0     1293 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/rejected_workflow_node_result_event.py
+-rw-r--r--   0        0        0     1144 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/sandbox_scenario.py
+-rw-r--r--   0        0        0      907 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/scenario_input.py
+-rw-r--r--   0        0        0     1071 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/scenario_input_chat_history_variable_value.py
+-rw-r--r--   0        0        0     1001 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/scenario_input_string_variable_value.py
+-rw-r--r--   0        0        0      938 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/search_error_response.py
+-rw-r--r--   0        0        0     1218 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/search_filters_request.py
+-rw-r--r--   0        0        0      997 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/search_node_result.py
+-rw-r--r--   0        0        0     1143 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/search_node_result_data.py
+-rw-r--r--   0        0        0     1622 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/search_request_options_request.py
+-rw-r--r--   0        0        0     1047 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/search_response.py
+-rw-r--r--   0        0        0     1304 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/search_result.py
+-rw-r--r--   0        0        0     1437 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/search_result_document.py
+-rw-r--r--   0        0        0     1365 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/search_result_document_request.py
+-rw-r--r--   0        0        0      972 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/search_result_merging_request.py
+-rw-r--r--   0        0        0     1333 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/search_result_request.py
+-rw-r--r--   0        0        0      133 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/search_results_enum.py
+-rw-r--r--   0        0        0      950 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/search_results_variable_value.py
+-rw-r--r--   0        0        0     1128 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/search_weights_request.py
+-rw-r--r--   0        0        0     1753 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/slim_deployment_read.py
+-rw-r--r--   0        0        0     2975 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/slim_document.py
+-rw-r--r--   0        0        0     2104 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/slim_workflow_deployment.py
+-rw-r--r--   0        0        0      124 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/streaming_enum.py
+-rw-r--r--   0        0        0     1388 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/streaming_execute_prompt_event.py
+-rw-r--r--   0        0        0     1030 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/streaming_prompt_execution_meta.py
+-rw-r--r--   0        0        0     1383 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/streaming_workflow_node_result_event.py
+-rw-r--r--   0        0        0      930 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/string_chat_message_content.py
+-rw-r--r--   0        0        0      937 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/string_chat_message_content_request.py
+-rw-r--r--   0        0        0      118 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/string_enum.py
+-rw-r--r--   0        0        0     1026 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/string_input_request.py
+-rw-r--r--   0        0        0      881 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/string_variable_value.py
+-rw-r--r--   0        0        0      931 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/string_vellum_value.py
+-rw-r--r--   0        0        0     1825 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/submit_completion_actual_request.py
+-rw-r--r--   0        0        0      875 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/submit_completion_actuals_error_response.py
+-rw-r--r--   0        0        0     1487 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/submit_workflow_execution_actual_request.py
+-rw-r--r--   0        0        0      128 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/subworkflow_enum.py
+-rw-r--r--   0        0        0      917 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/subworkflow_node_result.py
+-rw-r--r--   0        0        0      993 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/templating_node_array_result.py
+-rw-r--r--   0        0        0      964 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/templating_node_chat_history_result.py
+-rw-r--r--   0        0        0      945 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/templating_node_error_result.py
+-rw-r--r--   0        0        0      955 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/templating_node_function_call_result.py
+-rw-r--r--   0        0        0      923 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/templating_node_json_result.py
+-rw-r--r--   0        0        0      902 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/templating_node_number_result.py
+-rw-r--r--   0        0        0     1017 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/templating_node_result.py
+-rw-r--r--   0        0        0      956 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/templating_node_result_data.py
+-rw-r--r--   0        0        0     3246 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/templating_node_result_output.py
+-rw-r--r--   0        0        0      969 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/templating_node_search_results_result.py
+-rw-r--r--   0        0        0      900 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/templating_node_string_result.py
+-rw-r--r--   0        0        0     1142 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/terminal_node_array_result.py
+-rw-r--r--   0        0        0     1113 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/terminal_node_chat_history_result.py
+-rw-r--r--   0        0        0     1094 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/terminal_node_error_result.py
+-rw-r--r--   0        0        0     1104 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/terminal_node_function_call_result.py
+-rw-r--r--   0        0        0     1072 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/terminal_node_json_result.py
+-rw-r--r--   0        0        0     1051 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/terminal_node_number_result.py
+-rw-r--r--   0        0        0     1007 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/terminal_node_result.py
+-rw-r--r--   0        0        0      948 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/terminal_node_result_data.py
+-rw-r--r--   0        0        0     3164 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/terminal_node_result_output.py
+-rw-r--r--   0        0        0     1118 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/terminal_node_search_results_result.py
+-rw-r--r--   0        0        0     1049 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/terminal_node_string_result.py
+-rw-r--r--   0        0        0     1061 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_case_chat_history_variable_value.py
+-rw-r--r--   0        0        0     1036 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_case_error_variable_value.py
+-rw-r--r--   0        0        0     1081 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_case_function_call_variable_value.py
+-rw-r--r--   0        0        0     1012 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_case_json_variable_value.py
+-rw-r--r--   0        0        0      996 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_case_number_variable_value.py
+-rw-r--r--   0        0        0     1068 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_case_search_results_variable_value.py
+-rw-r--r--   0        0        0      991 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_case_string_variable_value.py
+-rw-r--r--   0        0        0     2834 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_case_variable_value.py
+-rw-r--r--   0        0        0     1373 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_deployment_release_tag_exec_config.py
+-rw-r--r--   0        0        0     1228 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_data.py
+-rw-r--r--   0        0        0     1235 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_data_request.py
+-rw-r--r--   0        0        0     1411 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_request.py
+-rw-r--r--   0        0        0      174 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_type_enum.py
+-rw-r--r--   0        0        0     1483 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_exec_config.py
+-rw-r--r--   0        0        0     1598 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_exec_config_request.py
+-rw-r--r--   0        0        0     1158 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution.py
+-rw-r--r--   0        0        0     1115 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_chat_history_output.py
+-rw-r--r--   0        0        0     1089 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_error_output.py
+-rw-r--r--   0        0        0     1135 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_function_call_output.py
+-rw-r--r--   0        0        0     1066 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_json_output.py
+-rw-r--r--   0        0        0      973 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_metric_definition.py
+-rw-r--r--   0        0        0     1218 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_metric_result.py
+-rw-r--r--   0        0        0     1047 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_number_output.py
+-rw-r--r--   0        0        0     3057 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_output.py
+-rw-r--r--   0        0        0     1122 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_search_results_output.py
+-rw-r--r--   0        0        0     1045 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_string_output.py
+-rw-r--r--   0        0        0     1331 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_external_exec_config.py
+-rw-r--r--   0        0        0     1115 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_external_exec_config_data.py
+-rw-r--r--   0        0        0     1144 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_external_exec_config_data_request.py
+-rw-r--r--   0        0        0     1360 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_external_exec_config_request.py
+-rw-r--r--   0        0        0      148 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_external_exec_config_type_enum.py
+-rw-r--r--   0        0        0     1005 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_metric_error_output.py
+-rw-r--r--   0        0        0      144 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_metric_error_output_type_enum.py
+-rw-r--r--   0        0        0      963 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_metric_number_output.py
+-rw-r--r--   0        0        0      146 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_metric_number_output_type_enum.py
+-rw-r--r--   0        0        0     1291 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_metric_output.py
+-rw-r--r--   0        0        0      961 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_metric_string_output.py
+-rw-r--r--   0        0        0      146 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_metric_string_output_type_enum.py
+-rw-r--r--   0        0        0     1500 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_read.py
+-rw-r--r--   0        0        0      197 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_state.py
+-rw-r--r--   0        0        0      896 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_test_suite.py
+-rw-r--r--   0        0        0     1367 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_workflow_release_tag_exec_config.py
+-rw-r--r--   0        0        0     1241 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_data.py
+-rw-r--r--   0        0        0     1248 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_data_request.py
+-rw-r--r--   0        0        0     1405 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_request.py
+-rw-r--r--   0        0        0      170 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_type_enum.py
+-rw-r--r--   0        0        0     1086 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_test_case.py
+-rw-r--r--   0        0        0      866 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/upload_document_error_response.py
+-rw-r--r--   0        0        0      946 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/upload_document_response.py
+-rw-r--r--   0        0        0      937 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/vellum_error.py
+-rw-r--r--   0        0        0      233 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/vellum_error_code_enum.py
+-rw-r--r--   0        0        0      944 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/vellum_error_request.py
+-rw-r--r--   0        0        0      914 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/vellum_image.py
+-rw-r--r--   0        0        0      921 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/vellum_image_request.py
+-rw-r--r--   0        0        0      944 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/vellum_variable.py
+-rw-r--r--   0        0        0      281 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/vellum_variable_type.py
+-rw-r--r--   0        0        0     2110 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_deployment_read.py
+-rw-r--r--   0        0        0      981 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_event_error.py
+-rw-r--r--   0        0        0     2038 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_execution_actual_chat_history_request.py
+-rw-r--r--   0        0        0     1975 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_execution_actual_json_request.py
+-rw-r--r--   0        0        0     1952 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_execution_actual_string_request.py
+-rw-r--r--   0        0        0      425 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_execution_event_error_code.py
+-rw-r--r--   0        0        0      170 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_execution_event_type.py
+-rw-r--r--   0        0        0     1139 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_execution_node_result_event.py
+-rw-r--r--   0        0        0     1134 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_execution_workflow_result_event.py
+-rw-r--r--   0        0        0     2966 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_node_result_data.py
+-rw-r--r--   0        0        0     1745 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_node_result_event.py
+-rw-r--r--   0        0        0      209 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_node_result_event_state.py
+-rw-r--r--   0        0        0     3212 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_output.py
+-rw-r--r--   0        0        0     1154 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_output_array.py
+-rw-r--r--   0        0        0     1131 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_output_chat_history.py
+-rw-r--r--   0        0        0     1106 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_output_error.py
+-rw-r--r--   0        0        0     1123 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_output_function_call.py
+-rw-r--r--   0        0        0     1106 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_output_image.py
+-rw-r--r--   0        0        0     1082 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_output_json.py
+-rw-r--r--   0        0        0     1063 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_output_number.py
+-rw-r--r--   0        0        0     1138 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_output_search_results.py
+-rw-r--r--   0        0        0     1061 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_output_string.py
+-rw-r--r--   0        0        0     1137 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_request_chat_history_input_request.py
+-rw-r--r--   0        0        0     1772 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_request_input_request.py
+-rw-r--r--   0        0        0     1066 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_request_json_input_request.py
+-rw-r--r--   0        0        0     1047 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_request_number_input_request.py
+-rw-r--r--   0        0        0     1045 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_request_string_input_request.py
+-rw-r--r--   0        0        0     1475 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_result_event.py
+-rw-r--r--   0        0        0     3529 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_result_event_output_data.py
+-rw-r--r--   0        0        0     1423 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_result_event_output_data_array.py
+-rw-r--r--   0        0        0     1400 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_result_event_output_data_chat_history.py
+-rw-r--r--   0        0        0     1375 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_result_event_output_data_error.py
+-rw-r--r--   0        0        0     1392 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_result_event_output_data_function_call.py
+-rw-r--r--   0        0        0     1351 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_result_event_output_data_json.py
+-rw-r--r--   0        0        0     1332 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_result_event_output_data_number.py
+-rw-r--r--   0        0        0     1407 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_result_event_output_data_search_results.py
+-rw-r--r--   0        0        0     1482 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_result_event_output_data_string.py
+-rw-r--r--   0        0        0      911 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_stream_event.py
+-rw-r--r--   0        0        0       77 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/version.py
+-rw-r--r--   0        0        0     3549 1970-01-01 00:00:00.000000 vellum_ai-0.5.2/PKG-INFO
```

### Comparing `vellum_ai-0.5.1/LICENSE` & `vellum_ai-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/README.md` & `vellum_ai-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/pyproject.toml` & `vellum_ai-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vellum-ai"
-version = "0.5.1"
+version = "0.5.2"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
     { include = "vellum", from = "src"}
 ]
```

### Comparing `vellum_ai-0.5.1/src/vellum/__init__.py` & `vellum_ai-0.5.2/src/vellum/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     DocumentRead,
     DocumentStatus,
     EnrichedNormalizedCompletion,
     EntityStatus,
     EnvironmentEnum,
     ErrorEnum,
     ErrorVariableValue,
+    ErrorVellumValue,
     ExecutePromptApiErrorResponse,
     ExecutePromptEvent,
     ExecutePromptEvent_Fulfilled,
     ExecutePromptEvent_Initiated,
     ExecutePromptEvent_Rejected,
     ExecutePromptEvent_Streaming,
     ExecutePromptResponse,
@@ -117,14 +118,15 @@
     FunctionCall,
     FunctionCallChatMessageContent,
     FunctionCallChatMessageContentRequest,
     FunctionCallChatMessageContentValue,
     FunctionCallChatMessageContentValueRequest,
     FunctionCallEnum,
     FunctionCallVariableValue,
+    FunctionCallVellumValue,
     FunctionCall_Fulfilled,
     FunctionCall_Rejected,
     GenerateErrorResponse,
     GenerateOptionsRequest,
     GenerateRequest,
     GenerateResponse,
     GenerateResult,
@@ -141,14 +143,15 @@
     InitiatedEnum,
     InitiatedExecutePromptEvent,
     InitiatedPromptExecutionMeta,
     InitiatedWorkflowNodeResultEvent,
     JsonEnum,
     JsonInputRequest,
     JsonVariableValue,
+    JsonVellumValue,
     LogicalOperator,
     LogprobsEnum,
     MetadataFilterConfigRequest,
     MetadataFilterRuleCombinator,
     MetadataFilterRuleRequest,
     MlModelUsage,
     NamedScenarioInputChatHistoryVariableValueRequest,
@@ -202,15 +205,15 @@
     NodeInputVariableCompiledValue_Json,
     NodeInputVariableCompiledValue_Number,
     NodeInputVariableCompiledValue_SearchResults,
     NodeInputVariableCompiledValue_String,
     NodeOutputCompiledArrayValue,
     NodeOutputCompiledChatHistoryValue,
     NodeOutputCompiledErrorValue,
-    NodeOutputCompiledFunctionValue,
+    NodeOutputCompiledFunctionCallValue,
     NodeOutputCompiledJsonValue,
     NodeOutputCompiledNumberValue,
     NodeOutputCompiledSearchResultsValue,
     NodeOutputCompiledStringValue,
     NodeOutputCompiledValue,
     NodeOutputCompiledValue_Array,
     NodeOutputCompiledValue_ChatHistory,
@@ -281,14 +284,15 @@
     StreamingPromptExecutionMeta,
     StreamingWorkflowNodeResultEvent,
     StringChatMessageContent,
     StringChatMessageContentRequest,
     StringEnum,
     StringInputRequest,
     StringVariableValue,
+    StringVellumValue,
     SubmitCompletionActualRequest,
     SubmitCompletionActualsErrorResponse,
     SubmitWorkflowExecutionActualRequest,
     SubmitWorkflowExecutionActualRequest_ChatHistory,
     SubmitWorkflowExecutionActualRequest_Json,
     SubmitWorkflowExecutionActualRequest_String,
     SubworkflowEnum,
@@ -571,14 +575,15 @@
     "DocumentRead",
     "DocumentStatus",
     "EnrichedNormalizedCompletion",
     "EntityStatus",
     "EnvironmentEnum",
     "ErrorEnum",
     "ErrorVariableValue",
+    "ErrorVellumValue",
     "ExecutePromptApiErrorResponse",
     "ExecutePromptEvent",
     "ExecutePromptEvent_Fulfilled",
     "ExecutePromptEvent_Initiated",
     "ExecutePromptEvent_Rejected",
     "ExecutePromptEvent_Streaming",
     "ExecutePromptResponse",
@@ -622,14 +627,15 @@
     "FunctionCall",
     "FunctionCallChatMessageContent",
     "FunctionCallChatMessageContentRequest",
     "FunctionCallChatMessageContentValue",
     "FunctionCallChatMessageContentValueRequest",
     "FunctionCallEnum",
     "FunctionCallVariableValue",
+    "FunctionCallVellumValue",
     "FunctionCall_Fulfilled",
     "FunctionCall_Rejected",
     "GenerateErrorResponse",
     "GenerateOptionsRequest",
     "GenerateRequest",
     "GenerateResponse",
     "GenerateResult",
@@ -647,14 +653,15 @@
     "InitiatedExecutePromptEvent",
     "InitiatedPromptExecutionMeta",
     "InitiatedWorkflowNodeResultEvent",
     "InternalServerError",
     "JsonEnum",
     "JsonInputRequest",
     "JsonVariableValue",
+    "JsonVellumValue",
     "LogicalOperator",
     "LogprobsEnum",
     "MetadataFilterConfigRequest",
     "MetadataFilterRuleCombinator",
     "MetadataFilterRuleRequest",
     "MlModelUsage",
     "NamedScenarioInputChatHistoryVariableValueRequest",
@@ -708,15 +715,15 @@
     "NodeInputVariableCompiledValue_Json",
     "NodeInputVariableCompiledValue_Number",
     "NodeInputVariableCompiledValue_SearchResults",
     "NodeInputVariableCompiledValue_String",
     "NodeOutputCompiledArrayValue",
     "NodeOutputCompiledChatHistoryValue",
     "NodeOutputCompiledErrorValue",
-    "NodeOutputCompiledFunctionValue",
+    "NodeOutputCompiledFunctionCallValue",
     "NodeOutputCompiledJsonValue",
     "NodeOutputCompiledNumberValue",
     "NodeOutputCompiledSearchResultsValue",
     "NodeOutputCompiledStringValue",
     "NodeOutputCompiledValue",
     "NodeOutputCompiledValue_Array",
     "NodeOutputCompiledValue_ChatHistory",
@@ -788,14 +795,15 @@
     "StreamingPromptExecutionMeta",
     "StreamingWorkflowNodeResultEvent",
     "StringChatMessageContent",
     "StringChatMessageContentRequest",
     "StringEnum",
     "StringInputRequest",
     "StringVariableValue",
+    "StringVellumValue",
     "SubmitCompletionActualRequest",
     "SubmitCompletionActualsErrorResponse",
     "SubmitWorkflowExecutionActualRequest",
     "SubmitWorkflowExecutionActualRequest_ChatHistory",
     "SubmitWorkflowExecutionActualRequest_Json",
     "SubmitWorkflowExecutionActualRequest_String",
     "SubworkflowEnum",
```

### Comparing `vellum_ai-0.5.1/src/vellum/client.py` & `vellum_ai-0.5.2/src/vellum/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/core/__init__.py` & `vellum_ai-0.5.2/src/vellum/core/__init__.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/core/client_wrapper.py` & `vellum_ai-0.5.2/src/vellum/core/client_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         self._environment = environment
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "vellum-ai",
-            "X-Fern-SDK-Version": "0.5.1",
+            "X-Fern-SDK-Version": "0.5.2",
         }
         headers["X_API_KEY"] = self.api_key
         return headers
 
     def get_environment(self) -> VellumEnvironment:
         return self._environment
```

### Comparing `vellum_ai-0.5.1/src/vellum/core/datetime_utils.py` & `vellum_ai-0.5.2/src/vellum/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/core/file.py` & `vellum_ai-0.5.2/src/vellum/core/file.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/core/http_client.py` & `vellum_ai-0.5.2/src/vellum/core/http_client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/core/jsonable_encoder.py` & `vellum_ai-0.5.2/src/vellum/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/core/request_options.py` & `vellum_ai-0.5.2/src/vellum/core/request_options.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/lib/test_suites/resources.py` & `vellum_ai-0.5.2/src/vellum/lib/test_suites/resources.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/lib/utils/paginator.py` & `vellum_ai-0.5.2/src/vellum/lib/utils/paginator.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/resources/__init__.py` & `vellum_ai-0.5.2/src/vellum/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/resources/deployments/client.py` & `vellum_ai-0.5.2/src/vellum/resources/deployments/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/resources/document_indexes/client.py` & `vellum_ai-0.5.2/src/vellum/resources/document_indexes/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/resources/documents/client.py` & `vellum_ai-0.5.2/src/vellum/resources/documents/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/resources/folder_entities/client.py` & `vellum_ai-0.5.2/src/vellum/resources/folder_entities/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/resources/sandboxes/client.py` & `vellum_ai-0.5.2/src/vellum/resources/sandboxes/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/resources/test_suite_runs/client.py` & `vellum_ai-0.5.2/src/vellum/resources/test_suite_runs/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/resources/test_suites/client.py` & `vellum_ai-0.5.2/src/vellum/resources/test_suites/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/resources/workflow_deployments/client.py` & `vellum_ai-0.5.2/src/vellum/resources/workflow_deployments/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/terraform/_jsii/vellum-ai_vellum@0.0.0.jsii.tgz` & `vellum_ai-0.5.2/src/vellum/terraform/_jsii/vellum-ai_vellum@0.0.0.jsii.tgz`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/terraform/data_vellum_document_index/__init__.py` & `vellum_ai-0.5.2/src/vellum/terraform/data_vellum_document_index/__init__.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/terraform/document_index/__init__.py` & `vellum_ai-0.5.2/src/vellum/terraform/document_index/__init__.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/terraform/provider/__init__.py` & `vellum_ai-0.5.2/src/vellum/terraform/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/__init__.py` & `vellum_ai-0.5.2/src/vellum/types/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,15 @@
 from .document_read import DocumentRead
 from .document_status import DocumentStatus
 from .enriched_normalized_completion import EnrichedNormalizedCompletion
 from .entity_status import EntityStatus
 from .environment_enum import EnvironmentEnum
 from .error_enum import ErrorEnum
 from .error_variable_value import ErrorVariableValue
+from .error_vellum_value import ErrorVellumValue
 from .execute_prompt_api_error_response import ExecutePromptApiErrorResponse
 from .execute_prompt_event import (
     ExecutePromptEvent,
     ExecutePromptEvent_Fulfilled,
     ExecutePromptEvent_Initiated,
     ExecutePromptEvent_Rejected,
     ExecutePromptEvent_Streaming,
@@ -136,14 +137,15 @@
 from .function_call import FunctionCall, FunctionCall_Fulfilled, FunctionCall_Rejected
 from .function_call_chat_message_content import FunctionCallChatMessageContent
 from .function_call_chat_message_content_request import FunctionCallChatMessageContentRequest
 from .function_call_chat_message_content_value import FunctionCallChatMessageContentValue
 from .function_call_chat_message_content_value_request import FunctionCallChatMessageContentValueRequest
 from .function_call_enum import FunctionCallEnum
 from .function_call_variable_value import FunctionCallVariableValue
+from .function_call_vellum_value import FunctionCallVellumValue
 from .generate_error_response import GenerateErrorResponse
 from .generate_options_request import GenerateOptionsRequest
 from .generate_request import GenerateRequest
 from .generate_response import GenerateResponse
 from .generate_result import GenerateResult
 from .generate_result_data import GenerateResultData
 from .generate_result_error import GenerateResultError
@@ -158,14 +160,15 @@
 from .initiated_enum import InitiatedEnum
 from .initiated_execute_prompt_event import InitiatedExecutePromptEvent
 from .initiated_prompt_execution_meta import InitiatedPromptExecutionMeta
 from .initiated_workflow_node_result_event import InitiatedWorkflowNodeResultEvent
 from .json_enum import JsonEnum
 from .json_input_request import JsonInputRequest
 from .json_variable_value import JsonVariableValue
+from .json_vellum_value import JsonVellumValue
 from .logical_operator import LogicalOperator
 from .logprobs_enum import LogprobsEnum
 from .metadata_filter_config_request import MetadataFilterConfigRequest
 from .metadata_filter_rule_combinator import MetadataFilterRuleCombinator
 from .metadata_filter_rule_request import MetadataFilterRuleRequest
 from .ml_model_usage import MlModelUsage
 from .named_scenario_input_chat_history_variable_value_request import NamedScenarioInputChatHistoryVariableValueRequest
@@ -227,15 +230,15 @@
     NodeInputVariableCompiledValue_Number,
     NodeInputVariableCompiledValue_SearchResults,
     NodeInputVariableCompiledValue_String,
 )
 from .node_output_compiled_array_value import NodeOutputCompiledArrayValue
 from .node_output_compiled_chat_history_value import NodeOutputCompiledChatHistoryValue
 from .node_output_compiled_error_value import NodeOutputCompiledErrorValue
-from .node_output_compiled_function_value import NodeOutputCompiledFunctionValue
+from .node_output_compiled_function_call_value import NodeOutputCompiledFunctionCallValue
 from .node_output_compiled_json_value import NodeOutputCompiledJsonValue
 from .node_output_compiled_number_value import NodeOutputCompiledNumberValue
 from .node_output_compiled_search_results_value import NodeOutputCompiledSearchResultsValue
 from .node_output_compiled_string_value import NodeOutputCompiledStringValue
 from .node_output_compiled_value import (
     NodeOutputCompiledValue,
     NodeOutputCompiledValue_Array,
@@ -310,14 +313,15 @@
 from .streaming_prompt_execution_meta import StreamingPromptExecutionMeta
 from .streaming_workflow_node_result_event import StreamingWorkflowNodeResultEvent
 from .string_chat_message_content import StringChatMessageContent
 from .string_chat_message_content_request import StringChatMessageContentRequest
 from .string_enum import StringEnum
 from .string_input_request import StringInputRequest
 from .string_variable_value import StringVariableValue
+from .string_vellum_value import StringVellumValue
 from .submit_completion_actual_request import SubmitCompletionActualRequest
 from .submit_completion_actuals_error_response import SubmitCompletionActualsErrorResponse
 from .submit_workflow_execution_actual_request import (
     SubmitWorkflowExecutionActualRequest,
     SubmitWorkflowExecutionActualRequest_ChatHistory,
     SubmitWorkflowExecutionActualRequest_Json,
     SubmitWorkflowExecutionActualRequest_String,
@@ -610,14 +614,15 @@
     "DocumentRead",
     "DocumentStatus",
     "EnrichedNormalizedCompletion",
     "EntityStatus",
     "EnvironmentEnum",
     "ErrorEnum",
     "ErrorVariableValue",
+    "ErrorVellumValue",
     "ExecutePromptApiErrorResponse",
     "ExecutePromptEvent",
     "ExecutePromptEvent_Fulfilled",
     "ExecutePromptEvent_Initiated",
     "ExecutePromptEvent_Rejected",
     "ExecutePromptEvent_Streaming",
     "ExecutePromptResponse",
@@ -660,14 +665,15 @@
     "FunctionCall",
     "FunctionCallChatMessageContent",
     "FunctionCallChatMessageContentRequest",
     "FunctionCallChatMessageContentValue",
     "FunctionCallChatMessageContentValueRequest",
     "FunctionCallEnum",
     "FunctionCallVariableValue",
+    "FunctionCallVellumValue",
     "FunctionCall_Fulfilled",
     "FunctionCall_Rejected",
     "GenerateErrorResponse",
     "GenerateOptionsRequest",
     "GenerateRequest",
     "GenerateResponse",
     "GenerateResult",
@@ -684,14 +690,15 @@
     "InitiatedEnum",
     "InitiatedExecutePromptEvent",
     "InitiatedPromptExecutionMeta",
     "InitiatedWorkflowNodeResultEvent",
     "JsonEnum",
     "JsonInputRequest",
     "JsonVariableValue",
+    "JsonVellumValue",
     "LogicalOperator",
     "LogprobsEnum",
     "MetadataFilterConfigRequest",
     "MetadataFilterRuleCombinator",
     "MetadataFilterRuleRequest",
     "MlModelUsage",
     "NamedScenarioInputChatHistoryVariableValueRequest",
@@ -745,15 +752,15 @@
     "NodeInputVariableCompiledValue_Json",
     "NodeInputVariableCompiledValue_Number",
     "NodeInputVariableCompiledValue_SearchResults",
     "NodeInputVariableCompiledValue_String",
     "NodeOutputCompiledArrayValue",
     "NodeOutputCompiledChatHistoryValue",
     "NodeOutputCompiledErrorValue",
-    "NodeOutputCompiledFunctionValue",
+    "NodeOutputCompiledFunctionCallValue",
     "NodeOutputCompiledJsonValue",
     "NodeOutputCompiledNumberValue",
     "NodeOutputCompiledSearchResultsValue",
     "NodeOutputCompiledStringValue",
     "NodeOutputCompiledValue",
     "NodeOutputCompiledValue_Array",
     "NodeOutputCompiledValue_ChatHistory",
@@ -824,14 +831,15 @@
     "StreamingPromptExecutionMeta",
     "StreamingWorkflowNodeResultEvent",
     "StringChatMessageContent",
     "StringChatMessageContentRequest",
     "StringEnum",
     "StringInputRequest",
     "StringVariableValue",
+    "StringVellumValue",
     "SubmitCompletionActualRequest",
     "SubmitCompletionActualsErrorResponse",
     "SubmitWorkflowExecutionActualRequest",
     "SubmitWorkflowExecutionActualRequest_ChatHistory",
     "SubmitWorkflowExecutionActualRequest_Json",
     "SubmitWorkflowExecutionActualRequest_String",
     "SubworkflowEnum",
```

### Comparing `vellum_ai-0.5.1/src/vellum/types/api_node_result.py` & `vellum_ai-0.5.2/src/vellum/types/api_node_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/api_node_result_data.py` & `vellum_ai-0.5.2/src/vellum/types/api_node_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/array_chat_message_content.py` & `vellum_ai-0.5.2/src/vellum/types/array_chat_message_content.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/array_chat_message_content_item.py` & `vellum_ai-0.5.2/src/vellum/types/array_chat_message_content_item.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/array_chat_message_content_item_request.py` & `vellum_ai-0.5.2/src/vellum/types/array_chat_message_content_item_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/array_chat_message_content_request.py` & `vellum_ai-0.5.2/src/vellum/types/array_chat_message_content_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/array_variable_value_item.py` & `vellum_ai-0.5.2/src/vellum/types/array_variable_value_item.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/chat_history_input_request.py` & `vellum_ai-0.5.2/src/vellum/types/chat_history_input_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/chat_history_variable_value.py` & `vellum_ai-0.5.2/src/vellum/types/chat_history_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/chat_message.py` & `vellum_ai-0.5.2/src/vellum/types/chat_message.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/chat_message_content.py` & `vellum_ai-0.5.2/src/vellum/types/chat_message_content.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/chat_message_content_request.py` & `vellum_ai-0.5.2/src/vellum/types/chat_message_content_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/chat_message_request.py` & `vellum_ai-0.5.2/src/vellum/types/chat_message_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/code_execution_node_array_result.py` & `vellum_ai-0.5.2/src/vellum/types/code_execution_node_array_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/code_execution_node_chat_history_result.py` & `vellum_ai-0.5.2/src/vellum/types/code_execution_node_chat_history_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/code_execution_node_error_result.py` & `vellum_ai-0.5.2/src/vellum/types/code_execution_node_error_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/code_execution_node_function_call_result.py` & `vellum_ai-0.5.2/src/vellum/types/code_execution_node_function_call_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/code_execution_node_json_result.py` & `vellum_ai-0.5.2/src/vellum/types/code_execution_node_json_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/code_execution_node_number_result.py` & `vellum_ai-0.5.2/src/vellum/types/code_execution_node_number_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/code_execution_node_result.py` & `vellum_ai-0.5.2/src/vellum/types/code_execution_node_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/code_execution_node_result_data.py` & `vellum_ai-0.5.2/src/vellum/types/code_execution_node_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/code_execution_node_result_output.py` & `vellum_ai-0.5.2/src/vellum/types/code_execution_node_result_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/code_execution_node_search_results_result.py` & `vellum_ai-0.5.2/src/vellum/types/code_execution_node_search_results_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/code_execution_node_string_result.py` & `vellum_ai-0.5.2/src/vellum/types/code_execution_node_string_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/conditional_node_result.py` & `vellum_ai-0.5.2/src/vellum/types/conditional_node_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/conditional_node_result_data.py` & `vellum_ai-0.5.2/src/vellum/types/conditional_node_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/deployment_provider_payload_response.py` & `vellum_ai-0.5.2/src/vellum/types/deployment_provider_payload_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/deployment_read.py` & `vellum_ai-0.5.2/src/vellum/types/deployment_read.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/document_document_to_document_index.py` & `vellum_ai-0.5.2/src/vellum/types/document_document_to_document_index.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/document_index_read.py` & `vellum_ai-0.5.2/src/vellum/types/document_index_read.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/document_read.py` & `vellum_ai-0.5.2/src/vellum/types/document_read.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/enriched_normalized_completion.py` & `vellum_ai-0.5.2/src/vellum/types/enriched_normalized_completion.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/error_variable_value.py` & `vellum_ai-0.5.2/src/vellum/types/error_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/execute_prompt_api_error_response.py` & `vellum_ai-0.5.2/src/vellum/types/execute_prompt_api_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/execute_prompt_event.py` & `vellum_ai-0.5.2/src/vellum/types/execute_prompt_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/execute_prompt_response.py` & `vellum_ai-0.5.2/src/vellum/types/execute_prompt_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/execute_workflow_error_response.py` & `vellum_ai-0.5.2/src/vellum/types/execute_workflow_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/execute_workflow_response.py` & `vellum_ai-0.5.2/src/vellum/types/execute_workflow_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/execute_workflow_stream_error_response.py` & `vellum_ai-0.5.2/src/vellum/types/execute_workflow_stream_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/execute_workflow_workflow_result_event.py` & `vellum_ai-0.5.2/src/vellum/types/execute_workflow_workflow_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/execution_array_vellum_value.py` & `vellum_ai-0.5.2/src/vellum/types/execution_array_vellum_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/execution_chat_history_vellum_value.py` & `vellum_ai-0.5.2/src/vellum/types/execution_chat_history_vellum_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/execution_error_vellum_value.py` & `vellum_ai-0.5.2/src/vellum/types/execution_error_vellum_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/execution_function_call_vellum_value.py` & `vellum_ai-0.5.2/src/vellum/types/execution_function_call_vellum_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/execution_json_vellum_value.py` & `vellum_ai-0.5.2/src/vellum/types/execution_json_vellum_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/execution_number_vellum_value.py` & `vellum_ai-0.5.2/src/vellum/types/execution_number_vellum_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/execution_search_results_vellum_value.py` & `vellum_ai-0.5.2/src/vellum/types/execution_search_results_vellum_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/execution_string_vellum_value.py` & `vellum_ai-0.5.2/src/vellum/types/execution_string_vellum_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/execution_vellum_value.py` & `vellum_ai-0.5.2/src/vellum/types/execution_vellum_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/external_test_case_execution.py` & `vellum_ai-0.5.2/src/vellum/types/external_test_case_execution.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/external_test_case_execution_request.py` & `vellum_ai-0.5.2/src/vellum/types/external_test_case_execution_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/fulfilled_execute_prompt_event.py` & `vellum_ai-0.5.2/src/vellum/types/fulfilled_execute_prompt_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/fulfilled_execute_prompt_response.py` & `vellum_ai-0.5.2/src/vellum/types/fulfilled_execute_prompt_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/fulfilled_execute_workflow_workflow_result_event.py` & `vellum_ai-0.5.2/src/vellum/types/fulfilled_execute_workflow_workflow_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/fulfilled_function_call.py` & `vellum_ai-0.5.2/src/vellum/types/fulfilled_function_call.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/fulfilled_function_call_request.py` & `vellum_ai-0.5.2/src/vellum/types/fulfilled_function_call_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/fulfilled_prompt_execution_meta.py` & `vellum_ai-0.5.2/src/vellum/types/fulfilled_prompt_execution_meta.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/fulfilled_workflow_node_result_event.py` & `vellum_ai-0.5.2/src/vellum/types/fulfilled_workflow_node_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/function_call.py` & `vellum_ai-0.5.2/src/vellum/types/function_call.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/function_call_chat_message_content.py` & `vellum_ai-0.5.2/src/vellum/types/function_call_chat_message_content.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/function_call_chat_message_content_request.py` & `vellum_ai-0.5.2/src/vellum/types/function_call_chat_message_content_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/function_call_chat_message_content_value.py` & `vellum_ai-0.5.2/src/vellum/types/function_call_chat_message_content_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/function_call_chat_message_content_value_request.py` & `vellum_ai-0.5.2/src/vellum/types/function_call_chat_message_content_value_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/function_call_variable_value.py` & `vellum_ai-0.5.2/src/vellum/types/function_call_variable_value.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 from .function_call import FunctionCall
 
 
 class FunctionCallVariableValue(pydantic_v1.BaseModel):
-    value: FunctionCall
+    value: typing.Optional[FunctionCall] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.5.1/src/vellum/types/generate_error_response.py` & `vellum_ai-0.5.2/src/vellum/types/generate_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/generate_options_request.py` & `vellum_ai-0.5.2/src/vellum/types/generate_options_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/generate_request.py` & `vellum_ai-0.5.2/src/vellum/types/generate_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/generate_response.py` & `vellum_ai-0.5.2/src/vellum/types/generate_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/generate_result.py` & `vellum_ai-0.5.2/src/vellum/types/generate_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/generate_result_data.py` & `vellum_ai-0.5.2/src/vellum/types/generate_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/generate_result_error.py` & `vellum_ai-0.5.2/src/vellum/types/generate_result_error.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/generate_stream_response.py` & `vellum_ai-0.5.2/src/vellum/types/generate_stream_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/generate_stream_result.py` & `vellum_ai-0.5.2/src/vellum/types/generate_stream_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/generate_stream_result_data.py` & `vellum_ai-0.5.2/src/vellum/types/generate_stream_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/image_chat_message_content.py` & `vellum_ai-0.5.2/src/vellum/types/image_chat_message_content.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/image_chat_message_content_request.py` & `vellum_ai-0.5.2/src/vellum/types/image_chat_message_content_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/image_variable_value.py` & `vellum_ai-0.5.2/src/vellum/types/image_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/initiated_execute_prompt_event.py` & `vellum_ai-0.5.2/src/vellum/types/initiated_execute_prompt_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/initiated_prompt_execution_meta.py` & `vellum_ai-0.5.2/src/vellum/types/initiated_prompt_execution_meta.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/initiated_workflow_node_result_event.py` & `vellum_ai-0.5.2/src/vellum/types/initiated_workflow_node_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/json_input_request.py` & `vellum_ai-0.5.2/src/vellum/types/json_input_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/json_variable_value.py` & `vellum_ai-0.5.2/src/vellum/types/json_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/metadata_filter_config_request.py` & `vellum_ai-0.5.2/src/vellum/types/metadata_filter_config_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/metadata_filter_rule_request.py` & `vellum_ai-0.5.2/src/vellum/types/metadata_filter_rule_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/ml_model_usage.py` & `vellum_ai-0.5.2/src/vellum/types/ml_model_usage.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/named_scenario_input_chat_history_variable_value_request.py` & `vellum_ai-0.5.2/src/vellum/types/named_scenario_input_chat_history_variable_value_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/named_scenario_input_request.py` & `vellum_ai-0.5.2/src/vellum/types/named_scenario_input_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/named_scenario_input_string_variable_value_request.py` & `vellum_ai-0.5.2/src/vellum/types/named_scenario_input_string_variable_value_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/named_test_case_chat_history_variable_value.py` & `vellum_ai-0.5.2/src/vellum/types/named_test_case_chat_history_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/named_test_case_chat_history_variable_value_request.py` & `vellum_ai-0.5.2/src/vellum/types/named_test_case_chat_history_variable_value_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/named_test_case_error_variable_value.py` & `vellum_ai-0.5.2/src/vellum/types/named_test_case_error_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/named_test_case_error_variable_value_request.py` & `vellum_ai-0.5.2/src/vellum/types/named_test_case_error_variable_value_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/named_test_case_function_call_variable_value.py` & `vellum_ai-0.5.2/src/vellum/types/named_test_case_function_call_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/named_test_case_function_call_variable_value_request.py` & `vellum_ai-0.5.2/src/vellum/types/named_test_case_function_call_variable_value_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/named_test_case_json_variable_value.py` & `vellum_ai-0.5.2/src/vellum/types/named_test_case_json_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/named_test_case_json_variable_value_request.py` & `vellum_ai-0.5.2/src/vellum/types/named_test_case_json_variable_value_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/named_test_case_number_variable_value.py` & `vellum_ai-0.5.2/src/vellum/types/named_test_case_number_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/named_test_case_number_variable_value_request.py` & `vellum_ai-0.5.2/src/vellum/types/named_test_case_number_variable_value_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/named_test_case_search_results_variable_value.py` & `vellum_ai-0.5.2/src/vellum/types/named_test_case_search_results_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/named_test_case_search_results_variable_value_request.py` & `vellum_ai-0.5.2/src/vellum/types/named_test_case_search_results_variable_value_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/named_test_case_string_variable_value.py` & `vellum_ai-0.5.2/src/vellum/types/named_test_case_string_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/named_test_case_string_variable_value_request.py` & `vellum_ai-0.5.2/src/vellum/types/named_test_case_string_variable_value_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/named_test_case_variable_value.py` & `vellum_ai-0.5.2/src/vellum/types/named_test_case_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/named_test_case_variable_value_request.py` & `vellum_ai-0.5.2/src/vellum/types/named_test_case_variable_value_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/node_input_compiled_array_value.py` & `vellum_ai-0.5.2/src/vellum/types/node_input_compiled_array_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/node_input_compiled_chat_history_value.py` & `vellum_ai-0.5.2/src/vellum/types/node_input_compiled_chat_history_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/node_input_compiled_error_value.py` & `vellum_ai-0.5.2/src/vellum/types/node_input_compiled_error_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/node_input_compiled_function_call.py` & `vellum_ai-0.5.2/src/vellum/types/node_input_compiled_function_call.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/node_input_compiled_json_value.py` & `vellum_ai-0.5.2/src/vellum/types/node_input_compiled_json_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/node_input_compiled_number_value.py` & `vellum_ai-0.5.2/src/vellum/types/node_input_compiled_number_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/node_input_compiled_search_results_value.py` & `vellum_ai-0.5.2/src/vellum/types/node_input_compiled_search_results_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/node_input_compiled_string_value.py` & `vellum_ai-0.5.2/src/vellum/types/node_input_compiled_string_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/node_input_variable_compiled_value.py` & `vellum_ai-0.5.2/src/vellum/types/node_input_variable_compiled_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/node_output_compiled_array_value.py` & `vellum_ai-0.5.2/src/vellum/types/json_vellum_value.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
-from .array_variable_value_item import ArrayVariableValueItem
 
 
-class NodeOutputCompiledArrayValue(pydantic_v1.BaseModel):
-    node_output_id: str
-    value: typing.Optional[typing.List[ArrayVariableValueItem]] = None
+class JsonVellumValue(pydantic_v1.BaseModel):
+    """
+    A value representing a JSON object.
+    """
+
+    value: typing.Optional[typing.Dict[str, typing.Any]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.5.1/src/vellum/types/node_output_compiled_chat_history_value.py` & `vellum_ai-0.5.2/src/vellum/types/templating_node_chat_history_result.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 from .chat_message import ChatMessage
 
 
-class NodeOutputCompiledChatHistoryValue(pydantic_v1.BaseModel):
-    node_output_id: str
+class TemplatingNodeChatHistoryResult(pydantic_v1.BaseModel):
+    id: str
     value: typing.Optional[typing.List[ChatMessage]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `vellum_ai-0.5.1/src/vellum/types/node_output_compiled_error_value.py` & `vellum_ai-0.5.2/src/vellum/types/templating_node_error_result.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 from .vellum_error import VellumError
 
 
-class NodeOutputCompiledErrorValue(pydantic_v1.BaseModel):
-    node_output_id: str
+class TemplatingNodeErrorResult(pydantic_v1.BaseModel):
+    id: str
     value: typing.Optional[VellumError] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `vellum_ai-0.5.1/src/vellum/types/node_output_compiled_function_value.py` & `vellum_ai-0.5.2/src/vellum/types/function_call_vellum_value.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,17 +4,20 @@
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 from .function_call import FunctionCall
 
 
-class NodeOutputCompiledFunctionValue(pydantic_v1.BaseModel):
-    node_output_id: str
-    value: typing.Optional[FunctionCall] = None
+class FunctionCallVellumValue(pydantic_v1.BaseModel):
+    """
+    A value representing a Function Call.
+    """
+
+    value: FunctionCall
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.5.1/src/vellum/types/node_output_compiled_json_value.py` & `vellum_ai-0.5.2/src/vellum/types/templating_node_json_result.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 
 
-class NodeOutputCompiledJsonValue(pydantic_v1.BaseModel):
-    node_output_id: str
+class TemplatingNodeJsonResult(pydantic_v1.BaseModel):
+    id: str
     value: typing.Optional[typing.Dict[str, typing.Any]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `vellum_ai-0.5.1/src/vellum/types/node_output_compiled_number_value.py` & `vellum_ai-0.5.2/src/vellum/types/vellum_image.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 
 
-class NodeOutputCompiledNumberValue(pydantic_v1.BaseModel):
-    node_output_id: str
-    value: typing.Optional[float] = None
+class VellumImage(pydantic_v1.BaseModel):
+    src: str
+    metadata: typing.Optional[typing.Dict[str, typing.Any]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.5.1/src/vellum/types/node_output_compiled_search_results_value.py` & `vellum_ai-0.5.2/src/vellum/types/search_results_variable_value.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 from .search_result import SearchResult
 
 
-class NodeOutputCompiledSearchResultsValue(pydantic_v1.BaseModel):
-    node_output_id: str
+class SearchResultsVariableValue(pydantic_v1.BaseModel):
     value: typing.Optional[typing.List[SearchResult]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `vellum_ai-0.5.1/src/vellum/types/node_output_compiled_string_value.py` & `vellum_ai-0.5.2/src/vellum/types/vellum_image_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 
 
-class NodeOutputCompiledStringValue(pydantic_v1.BaseModel):
-    node_output_id: str
-    value: typing.Optional[str] = None
+class VellumImageRequest(pydantic_v1.BaseModel):
+    src: str
+    metadata: typing.Optional[typing.Dict[str, typing.Any]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.5.1/src/vellum/types/node_output_compiled_value.py` & `vellum_ai-0.5.2/src/vellum/types/node_output_compiled_value.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 
 import typing
 
 from .node_output_compiled_array_value import NodeOutputCompiledArrayValue
 from .node_output_compiled_chat_history_value import NodeOutputCompiledChatHistoryValue
 from .node_output_compiled_error_value import NodeOutputCompiledErrorValue
-from .node_output_compiled_function_value import NodeOutputCompiledFunctionValue
+from .node_output_compiled_function_call_value import NodeOutputCompiledFunctionCallValue
 from .node_output_compiled_json_value import NodeOutputCompiledJsonValue
 from .node_output_compiled_number_value import NodeOutputCompiledNumberValue
 from .node_output_compiled_search_results_value import NodeOutputCompiledSearchResultsValue
 from .node_output_compiled_string_value import NodeOutputCompiledStringValue
 
 
 class NodeOutputCompiledValue_String(NodeOutputCompiledStringValue):
@@ -80,15 +80,15 @@
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
 
 
-class NodeOutputCompiledValue_FunctionCall(NodeOutputCompiledFunctionValue):
+class NodeOutputCompiledValue_FunctionCall(NodeOutputCompiledFunctionCallValue):
     type: typing.Literal["FUNCTION_CALL"] = "FUNCTION_CALL"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
```

### Comparing `vellum_ai-0.5.1/src/vellum/types/normalized_log_probs.py` & `vellum_ai-0.5.2/src/vellum/types/normalized_log_probs.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/normalized_token_log_probs.py` & `vellum_ai-0.5.2/src/vellum/types/normalized_token_log_probs.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/number_variable_value.py` & `vellum_ai-0.5.2/src/vellum/types/number_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/paginated_document_index_read_list.py` & `vellum_ai-0.5.2/src/vellum/types/paginated_document_index_read_list.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/paginated_slim_deployment_read_list.py` & `vellum_ai-0.5.2/src/vellum/types/paginated_slim_deployment_read_list.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/paginated_slim_document_list.py` & `vellum_ai-0.5.2/src/vellum/types/paginated_slim_document_list.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/paginated_slim_workflow_deployment_list.py` & `vellum_ai-0.5.2/src/vellum/types/paginated_slim_workflow_deployment_list.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/paginated_test_suite_run_execution_list.py` & `vellum_ai-0.5.2/src/vellum/types/paginated_test_suite_run_execution_list.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/paginated_test_suite_test_case_list.py` & `vellum_ai-0.5.2/src/vellum/types/paginated_test_suite_test_case_list.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/prompt_deployment_expand_meta_request_request.py` & `vellum_ai-0.5.2/src/vellum/types/prompt_deployment_expand_meta_request_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/prompt_deployment_input_request.py` & `vellum_ai-0.5.2/src/vellum/types/prompt_deployment_input_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/prompt_execution_meta.py` & `vellum_ai-0.5.2/src/vellum/types/prompt_execution_meta.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/prompt_node_result.py` & `vellum_ai-0.5.2/src/vellum/types/prompt_node_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/prompt_node_result_data.py` & `vellum_ai-0.5.2/src/vellum/types/prompt_node_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/prompt_output.py` & `vellum_ai-0.5.2/src/vellum/types/prompt_output.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from __future__ import annotations
 
 import typing
 
-from .error_variable_value import ErrorVariableValue
-from .function_call_variable_value import FunctionCallVariableValue
-from .json_variable_value import JsonVariableValue
-from .string_variable_value import StringVariableValue
+from .error_vellum_value import ErrorVellumValue
+from .function_call_vellum_value import FunctionCallVellumValue
+from .json_vellum_value import JsonVellumValue
+from .string_vellum_value import StringVellumValue
 
 
-class PromptOutput_String(StringVariableValue):
+class PromptOutput_String(StringVellumValue):
     type: typing.Literal["STRING"] = "STRING"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
 
 
-class PromptOutput_Json(JsonVariableValue):
+class PromptOutput_Json(JsonVellumValue):
     type: typing.Literal["JSON"] = "JSON"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
 
 
-class PromptOutput_Error(ErrorVariableValue):
+class PromptOutput_Error(ErrorVellumValue):
     type: typing.Literal["ERROR"] = "ERROR"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
 
 
-class PromptOutput_FunctionCall(FunctionCallVariableValue):
+class PromptOutput_FunctionCall(FunctionCallVellumValue):
     type: typing.Literal["FUNCTION_CALL"] = "FUNCTION_CALL"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
```

### Comparing `vellum_ai-0.5.1/src/vellum/types/raw_prompt_execution_overrides_request.py` & `vellum_ai-0.5.2/src/vellum/types/raw_prompt_execution_overrides_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/rejected_execute_prompt_event.py` & `vellum_ai-0.5.2/src/vellum/types/rejected_execute_prompt_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/rejected_execute_prompt_response.py` & `vellum_ai-0.5.2/src/vellum/types/rejected_execute_prompt_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/rejected_execute_workflow_workflow_result_event.py` & `vellum_ai-0.5.2/src/vellum/types/rejected_execute_workflow_workflow_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/rejected_function_call.py` & `vellum_ai-0.5.2/src/vellum/types/rejected_function_call.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/rejected_prompt_execution_meta.py` & `vellum_ai-0.5.2/src/vellum/types/rejected_prompt_execution_meta.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/rejected_workflow_node_result_event.py` & `vellum_ai-0.5.2/src/vellum/types/rejected_workflow_node_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/sandbox_scenario.py` & `vellum_ai-0.5.2/src/vellum/types/sandbox_scenario.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/scenario_input.py` & `vellum_ai-0.5.2/src/vellum/types/scenario_input.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/scenario_input_chat_history_variable_value.py` & `vellum_ai-0.5.2/src/vellum/types/scenario_input_chat_history_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/scenario_input_string_variable_value.py` & `vellum_ai-0.5.2/src/vellum/types/scenario_input_string_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/search_error_response.py` & `vellum_ai-0.5.2/src/vellum/types/search_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/search_filters_request.py` & `vellum_ai-0.5.2/src/vellum/types/search_filters_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/search_node_result.py` & `vellum_ai-0.5.2/src/vellum/types/search_node_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/search_node_result_data.py` & `vellum_ai-0.5.2/src/vellum/types/search_node_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/search_request_options_request.py` & `vellum_ai-0.5.2/src/vellum/types/search_request_options_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/search_response.py` & `vellum_ai-0.5.2/src/vellum/types/search_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/search_result.py` & `vellum_ai-0.5.2/src/vellum/types/search_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/search_result_document.py` & `vellum_ai-0.5.2/src/vellum/types/search_result_document.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/search_result_document_request.py` & `vellum_ai-0.5.2/src/vellum/types/search_result_document_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/search_result_merging_request.py` & `vellum_ai-0.5.2/src/vellum/types/search_result_merging_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/search_result_request.py` & `vellum_ai-0.5.2/src/vellum/types/search_result_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/search_results_variable_value.py` & `vellum_ai-0.5.2/src/vellum/types/templating_node_search_results_result.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 from .search_result import SearchResult
 
 
-class SearchResultsVariableValue(pydantic_v1.BaseModel):
+class TemplatingNodeSearchResultsResult(pydantic_v1.BaseModel):
+    id: str
     value: typing.Optional[typing.List[SearchResult]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `vellum_ai-0.5.1/src/vellum/types/search_weights_request.py` & `vellum_ai-0.5.2/src/vellum/types/search_weights_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/slim_deployment_read.py` & `vellum_ai-0.5.2/src/vellum/types/slim_deployment_read.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/slim_document.py` & `vellum_ai-0.5.2/src/vellum/types/slim_document.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/slim_workflow_deployment.py` & `vellum_ai-0.5.2/src/vellum/types/slim_workflow_deployment.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/streaming_execute_prompt_event.py` & `vellum_ai-0.5.2/src/vellum/types/streaming_execute_prompt_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/streaming_prompt_execution_meta.py` & `vellum_ai-0.5.2/src/vellum/types/streaming_prompt_execution_meta.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/streaming_workflow_node_result_event.py` & `vellum_ai-0.5.2/src/vellum/types/streaming_workflow_node_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/string_chat_message_content.py` & `vellum_ai-0.5.2/src/vellum/types/string_chat_message_content.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/string_chat_message_content_request.py` & `vellum_ai-0.5.2/src/vellum/types/string_chat_message_content_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/string_input_request.py` & `vellum_ai-0.5.2/src/vellum/types/string_input_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/string_variable_value.py` & `vellum_ai-0.5.2/src/vellum/types/string_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/submit_completion_actual_request.py` & `vellum_ai-0.5.2/src/vellum/types/submit_completion_actual_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/submit_completion_actuals_error_response.py` & `vellum_ai-0.5.2/src/vellum/types/submit_completion_actuals_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/submit_workflow_execution_actual_request.py` & `vellum_ai-0.5.2/src/vellum/types/submit_workflow_execution_actual_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/subworkflow_node_result.py` & `vellum_ai-0.5.2/src/vellum/types/subworkflow_node_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/templating_node_array_result.py` & `vellum_ai-0.5.2/src/vellum/types/templating_node_array_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/templating_node_chat_history_result.py` & `vellum_ai-0.5.2/src/vellum/types/upload_document_error_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
-from .chat_message import ChatMessage
 
 
-class TemplatingNodeChatHistoryResult(pydantic_v1.BaseModel):
-    id: str
-    value: typing.Optional[typing.List[ChatMessage]] = None
+class UploadDocumentErrorResponse(pydantic_v1.BaseModel):
+    detail: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.5.1/src/vellum/types/templating_node_error_result.py` & `vellum_ai-0.5.2/src/vellum/types/templating_node_number_result.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
-from .vellum_error import VellumError
 
 
-class TemplatingNodeErrorResult(pydantic_v1.BaseModel):
+class TemplatingNodeNumberResult(pydantic_v1.BaseModel):
     id: str
-    value: typing.Optional[VellumError] = None
+    value: typing.Optional[float] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.5.1/src/vellum/types/templating_node_function_call_result.py` & `vellum_ai-0.5.2/src/vellum/types/templating_node_function_call_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/templating_node_json_result.py` & `vellum_ai-0.5.2/src/vellum/types/vellum_error.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from .vellum_error_code_enum import VellumErrorCodeEnum
 
 
-class TemplatingNodeJsonResult(pydantic_v1.BaseModel):
-    id: str
-    value: typing.Optional[typing.Dict[str, typing.Any]] = None
+class VellumError(pydantic_v1.BaseModel):
+    message: str
+    code: VellumErrorCodeEnum
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.5.1/src/vellum/types/templating_node_number_result.py` & `vellum_ai-0.5.2/src/vellum/types/templating_node_string_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 
 
-class TemplatingNodeNumberResult(pydantic_v1.BaseModel):
+class TemplatingNodeStringResult(pydantic_v1.BaseModel):
     id: str
-    value: typing.Optional[float] = None
+    value: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.5.1/src/vellum/types/templating_node_result.py` & `vellum_ai-0.5.2/src/vellum/types/templating_node_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/templating_node_result_data.py` & `vellum_ai-0.5.2/src/vellum/types/templating_node_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/templating_node_result_output.py` & `vellum_ai-0.5.2/src/vellum/types/templating_node_result_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/templating_node_search_results_result.py` & `vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_search_results_output.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,17 +4,22 @@
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 from .search_result import SearchResult
 
 
-class TemplatingNodeSearchResultsResult(pydantic_v1.BaseModel):
-    id: str
+class TestSuiteRunExecutionSearchResultsOutput(pydantic_v1.BaseModel):
+    """
+    Execution output of an entity evaluated during a Test Suite Run that is of type SEARCH_RESULTS
+    """
+
+    name: str
     value: typing.Optional[typing.List[SearchResult]] = None
+    output_variable_id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.5.1/src/vellum/types/templating_node_string_result.py` & `vellum_ai-0.5.2/src/vellum/types/upload_document_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 
 
-class TemplatingNodeStringResult(pydantic_v1.BaseModel):
-    id: str
-    value: typing.Optional[str] = None
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
```

### Comparing `vellum_ai-0.5.1/src/vellum/types/terminal_node_array_result.py` & `vellum_ai-0.5.2/src/vellum/types/terminal_node_array_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/terminal_node_chat_history_result.py` & `vellum_ai-0.5.2/src/vellum/types/terminal_node_chat_history_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/terminal_node_error_result.py` & `vellum_ai-0.5.2/src/vellum/types/terminal_node_error_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/terminal_node_function_call_result.py` & `vellum_ai-0.5.2/src/vellum/types/terminal_node_function_call_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/terminal_node_json_result.py` & `vellum_ai-0.5.2/src/vellum/types/terminal_node_json_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/terminal_node_number_result.py` & `vellum_ai-0.5.2/src/vellum/types/terminal_node_number_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/terminal_node_result.py` & `vellum_ai-0.5.2/src/vellum/types/terminal_node_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/terminal_node_result_data.py` & `vellum_ai-0.5.2/src/vellum/types/terminal_node_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/terminal_node_result_output.py` & `vellum_ai-0.5.2/src/vellum/types/terminal_node_result_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/terminal_node_search_results_result.py` & `vellum_ai-0.5.2/src/vellum/types/terminal_node_search_results_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/terminal_node_string_result.py` & `vellum_ai-0.5.2/src/vellum/types/terminal_node_string_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_case_chat_history_variable_value.py` & `vellum_ai-0.5.2/src/vellum/types/test_case_chat_history_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_case_error_variable_value.py` & `vellum_ai-0.5.2/src/vellum/types/test_case_error_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_case_function_call_variable_value.py` & `vellum_ai-0.5.2/src/vellum/types/test_case_function_call_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_case_json_variable_value.py` & `vellum_ai-0.5.2/src/vellum/types/test_case_json_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_case_number_variable_value.py` & `vellum_ai-0.5.2/src/vellum/types/test_case_number_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_case_search_results_variable_value.py` & `vellum_ai-0.5.2/src/vellum/types/test_case_search_results_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_case_string_variable_value.py` & `vellum_ai-0.5.2/src/vellum/types/test_case_string_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_case_variable_value.py` & `vellum_ai-0.5.2/src/vellum/types/test_case_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_suite_run_deployment_release_tag_exec_config.py` & `vellum_ai-0.5.2/src/vellum/types/test_suite_run_deployment_release_tag_exec_config.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_data.py` & `vellum_ai-0.5.2/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_data_request.py` & `vellum_ai-0.5.2/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_data_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_request.py` & `vellum_ai-0.5.2/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_suite_run_exec_config.py` & `vellum_ai-0.5.2/src/vellum/types/test_suite_run_exec_config.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_suite_run_exec_config_request.py` & `vellum_ai-0.5.2/src/vellum/types/test_suite_run_exec_config_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_suite_run_execution.py` & `vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_suite_run_execution_chat_history_output.py` & `vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_chat_history_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_suite_run_execution_error_output.py` & `vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_error_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_suite_run_execution_function_call_output.py` & `vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_function_call_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_suite_run_execution_json_output.py` & `vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_json_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_suite_run_execution_metric_definition.py` & `vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_metric_definition.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_suite_run_execution_metric_result.py` & `vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_metric_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_suite_run_execution_number_output.py` & `vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_number_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_suite_run_execution_output.py` & `vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_suite_run_execution_search_results_output.py` & `vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_string_output.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
-from .search_result import SearchResult
 
 
-class TestSuiteRunExecutionSearchResultsOutput(pydantic_v1.BaseModel):
+class TestSuiteRunExecutionStringOutput(pydantic_v1.BaseModel):
     """
-    Execution output of an entity evaluated during a Test Suite Run that is of type SEARCH_RESULTS
+    Execution output of an entity evaluated during a Test Suite Run that is of type STRING
     """
 
     name: str
-    value: typing.Optional[typing.List[SearchResult]] = None
+    value: typing.Optional[str] = None
     output_variable_id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_suite_run_execution_string_output.py` & `vellum_ai-0.5.2/src/vellum/types/workflow_output_error.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from .vellum_error import VellumError
 
 
-class TestSuiteRunExecutionStringOutput(pydantic_v1.BaseModel):
+class WorkflowOutputError(pydantic_v1.BaseModel):
     """
-    Execution output of an entity evaluated during a Test Suite Run that is of type STRING
+    An error output from a Workflow execution.
     """
 
-    name: str
-    value: typing.Optional[str] = None
-    output_variable_id: str
+    id: str
+    name: str = pydantic_v1.Field()
+    """
+    The output's name, as defined in the workflow
+    """
+
+    value: typing.Optional[VellumError] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_suite_run_external_exec_config.py` & `vellum_ai-0.5.2/src/vellum/types/test_suite_run_external_exec_config.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_suite_run_external_exec_config_data.py` & `vellum_ai-0.5.2/src/vellum/types/test_suite_run_external_exec_config_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_suite_run_external_exec_config_data_request.py` & `vellum_ai-0.5.2/src/vellum/types/test_suite_run_external_exec_config_data_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_suite_run_external_exec_config_request.py` & `vellum_ai-0.5.2/src/vellum/types/test_suite_run_external_exec_config_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_suite_run_metric_error_output.py` & `vellum_ai-0.5.2/src/vellum/types/test_suite_run_metric_error_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_suite_run_metric_number_output.py` & `vellum_ai-0.5.2/src/vellum/types/test_suite_run_metric_number_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_suite_run_metric_output.py` & `vellum_ai-0.5.2/src/vellum/types/test_suite_run_metric_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_suite_run_metric_string_output.py` & `vellum_ai-0.5.2/src/vellum/types/test_suite_run_metric_string_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_suite_run_read.py` & `vellum_ai-0.5.2/src/vellum/types/test_suite_run_read.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_suite_run_test_suite.py` & `vellum_ai-0.5.2/src/vellum/types/test_suite_run_test_suite.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_suite_run_workflow_release_tag_exec_config.py` & `vellum_ai-0.5.2/src/vellum/types/test_suite_run_workflow_release_tag_exec_config.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_data.py` & `vellum_ai-0.5.2/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_data_request.py` & `vellum_ai-0.5.2/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_data_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_request.py` & `vellum_ai-0.5.2/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/test_suite_test_case.py` & `vellum_ai-0.5.2/src/vellum/types/test_suite_test_case.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/upload_document_error_response.py` & `vellum_ai-0.5.2/src/vellum/types/vellum_error_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from .vellum_error_code_enum import VellumErrorCodeEnum
 
 
-class UploadDocumentErrorResponse(pydantic_v1.BaseModel):
-    detail: str
+class VellumErrorRequest(pydantic_v1.BaseModel):
+    message: str
+    code: VellumErrorCodeEnum
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.5.1/src/vellum/types/upload_document_response.py` & `vellum_ai-0.5.2/src/vellum/types/error_vellum_value.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from .vellum_error import VellumError
 
 
-class UploadDocumentResponse(pydantic_v1.BaseModel):
-    document_id: str = pydantic_v1.Field()
+class ErrorVellumValue(pydantic_v1.BaseModel):
     """
-    The ID of the newly created document.
+    A value representing an Error.
     """
 
+    value: typing.Optional[VellumError] = None
+
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `vellum_ai-0.5.1/src/vellum/types/vellum_error.py` & `vellum_ai-0.5.2/src/vellum/types/workflow_request_json_input_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
-from .vellum_error_code_enum import VellumErrorCodeEnum
 
 
-class VellumError(pydantic_v1.BaseModel):
-    message: str
-    code: VellumErrorCodeEnum
+class WorkflowRequestJsonInputRequest(pydantic_v1.BaseModel):
+    """
+    The input for a JSON variable in a Workflow.
+    """
+
+    name: str = pydantic_v1.Field()
+    """
+    The variable's name, as defined in the Workflow.
+    """
+
+    value: typing.Dict[str, typing.Any]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.5.1/src/vellum/types/vellum_error_request.py` & `vellum_ai-0.5.2/src/vellum/types/workflow_request_number_input_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
-from .vellum_error_code_enum import VellumErrorCodeEnum
 
 
-class VellumErrorRequest(pydantic_v1.BaseModel):
-    message: str
-    code: VellumErrorCodeEnum
+class WorkflowRequestNumberInputRequest(pydantic_v1.BaseModel):
+    """
+    The input for a number variable in a Workflow.
+    """
+
+    name: str = pydantic_v1.Field()
+    """
+    The variable's name, as defined in the Workflow.
+    """
+
+    value: float
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.5.1/src/vellum/types/vellum_image.py` & `vellum_ai-0.5.2/src/vellum/types/string_vellum_value.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,20 @@
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 
 
-class VellumImage(pydantic_v1.BaseModel):
-    src: str
-    metadata: typing.Optional[typing.Dict[str, typing.Any]] = None
+class StringVellumValue(pydantic_v1.BaseModel):
+    """
+    A value representing a string.
+    """
+
+    value: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.5.1/src/vellum/types/vellum_image_request.py` & `vellum_ai-0.5.2/src/vellum/types/workflow_output_image.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from .vellum_image import VellumImage
 
 
-class VellumImageRequest(pydantic_v1.BaseModel):
-    src: str
-    metadata: typing.Optional[typing.Dict[str, typing.Any]] = None
+class WorkflowOutputImage(pydantic_v1.BaseModel):
+    """
+    An image output from a Workflow execution.
+    """
+
+    id: str
+    name: str = pydantic_v1.Field()
+    """
+    The output's name, as defined in the workflow
+    """
+
+    value: typing.Optional[VellumImage] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.5.1/src/vellum/types/vellum_variable.py` & `vellum_ai-0.5.2/src/vellum/types/vellum_variable.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/workflow_deployment_read.py` & `vellum_ai-0.5.2/src/vellum/types/workflow_deployment_read.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/workflow_event_error.py` & `vellum_ai-0.5.2/src/vellum/types/workflow_event_error.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/workflow_execution_actual_chat_history_request.py` & `vellum_ai-0.5.2/src/vellum/types/workflow_execution_actual_chat_history_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/workflow_execution_actual_json_request.py` & `vellum_ai-0.5.2/src/vellum/types/workflow_execution_actual_json_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/workflow_execution_actual_string_request.py` & `vellum_ai-0.5.2/src/vellum/types/workflow_execution_actual_string_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/workflow_execution_node_result_event.py` & `vellum_ai-0.5.2/src/vellum/types/workflow_execution_node_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/workflow_execution_workflow_result_event.py` & `vellum_ai-0.5.2/src/vellum/types/workflow_execution_workflow_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/workflow_node_result_data.py` & `vellum_ai-0.5.2/src/vellum/types/workflow_node_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/workflow_node_result_event.py` & `vellum_ai-0.5.2/src/vellum/types/workflow_node_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/workflow_output.py` & `vellum_ai-0.5.2/src/vellum/types/workflow_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/workflow_output_array.py` & `vellum_ai-0.5.2/src/vellum/types/workflow_output_array.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/workflow_output_chat_history.py` & `vellum_ai-0.5.2/src/vellum/types/workflow_output_chat_history.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/workflow_output_error.py` & `vellum_ai-0.5.2/src/vellum/types/workflow_output_number.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
-from .vellum_error import VellumError
 
 
-class WorkflowOutputError(pydantic_v1.BaseModel):
+class WorkflowOutputNumber(pydantic_v1.BaseModel):
     """
-    An error output from a Workflow execution.
+    A number output from a Workflow execution.
     """
 
     id: str
     name: str = pydantic_v1.Field()
     """
     The output's name, as defined in the workflow
     """
 
-    value: typing.Optional[VellumError] = None
+    value: typing.Optional[float] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.5.1/src/vellum/types/workflow_output_function_call.py` & `vellum_ai-0.5.2/src/vellum/types/workflow_output_function_call.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/workflow_output_image.py` & `vellum_ai-0.5.2/src/vellum/types/workflow_output_search_results.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
-from .vellum_image import VellumImage
+from .search_result import SearchResult
 
 
-class WorkflowOutputImage(pydantic_v1.BaseModel):
+class WorkflowOutputSearchResults(pydantic_v1.BaseModel):
     """
-    An image output from a Workflow execution.
+    A search results output from a Workflow execution.
     """
 
     id: str
     name: str = pydantic_v1.Field()
     """
     The output's name, as defined in the workflow
     """
 
-    value: typing.Optional[VellumImage] = None
+    value: typing.Optional[typing.List[SearchResult]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.5.1/src/vellum/types/workflow_output_json.py` & `vellum_ai-0.5.2/src/vellum/types/workflow_output_json.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/workflow_output_number.py` & `vellum_ai-0.5.2/src/vellum/types/workflow_request_string_input_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,26 +3,25 @@
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 
 
-class WorkflowOutputNumber(pydantic_v1.BaseModel):
+class WorkflowRequestStringInputRequest(pydantic_v1.BaseModel):
     """
-    A number output from a Workflow execution.
+    The input for a string variable in a Workflow.
     """
 
-    id: str
     name: str = pydantic_v1.Field()
     """
-    The output's name, as defined in the workflow
+    The variable's name, as defined in the Workflow.
     """
 
-    value: typing.Optional[float] = None
+    value: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.5.1/src/vellum/types/workflow_output_search_results.py` & `vellum_ai-0.5.2/src/vellum/types/node_output_compiled_function_call_value.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
-from .search_result import SearchResult
+from .function_call import FunctionCall
+from .workflow_node_result_event_state import WorkflowNodeResultEventState
 
 
-class WorkflowOutputSearchResults(pydantic_v1.BaseModel):
+class NodeOutputCompiledFunctionCallValue(pydantic_v1.BaseModel):
     """
-    A search results output from a Workflow execution.
+    An output returned by a node that is of type FUNCTION_CALL.
     """
 
-    id: str
-    name: str = pydantic_v1.Field()
-    """
-    The output's name, as defined in the workflow
-    """
-
-    value: typing.Optional[typing.List[SearchResult]] = None
+    value: typing.Optional[FunctionCall] = None
+    node_output_id: str
+    state: typing.Optional[WorkflowNodeResultEventState] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.5.1/src/vellum/types/workflow_output_string.py` & `vellum_ai-0.5.2/src/vellum/types/workflow_output_string.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/workflow_request_chat_history_input_request.py` & `vellum_ai-0.5.2/src/vellum/types/workflow_request_chat_history_input_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/workflow_request_input_request.py` & `vellum_ai-0.5.2/src/vellum/types/workflow_request_input_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/workflow_request_json_input_request.py` & `vellum_ai-0.5.2/src/vellum/types/node_output_compiled_chat_history_value.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from .chat_message import ChatMessage
+from .workflow_node_result_event_state import WorkflowNodeResultEventState
 
 
-class WorkflowRequestJsonInputRequest(pydantic_v1.BaseModel):
+class NodeOutputCompiledChatHistoryValue(pydantic_v1.BaseModel):
     """
-    The input for a JSON variable in a Workflow.
+    An output returned by a node that is of type CHAT_HISTORY.
     """
 
-    name: str = pydantic_v1.Field()
-    """
-    The variable's name, as defined in the Workflow.
-    """
-
-    value: typing.Dict[str, typing.Any]
+    value: typing.Optional[typing.List[ChatMessage]] = None
+    node_output_id: str
+    state: typing.Optional[WorkflowNodeResultEventState] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.5.1/src/vellum/types/workflow_request_number_input_request.py` & `vellum_ai-0.5.2/src/vellum/types/node_output_compiled_array_value.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from .array_variable_value_item import ArrayVariableValueItem
+from .workflow_node_result_event_state import WorkflowNodeResultEventState
 
 
-class WorkflowRequestNumberInputRequest(pydantic_v1.BaseModel):
+class NodeOutputCompiledArrayValue(pydantic_v1.BaseModel):
     """
-    The input for a number variable in a Workflow.
+    An output returned by a node that is of type ARRAY.
     """
 
-    name: str = pydantic_v1.Field()
-    """
-    The variable's name, as defined in the Workflow.
-    """
-
-    value: float
+    value: typing.Optional[typing.List[ArrayVariableValueItem]] = None
+    node_output_id: str
+    state: typing.Optional[WorkflowNodeResultEventState] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.5.1/src/vellum/types/workflow_result_event.py` & `vellum_ai-0.5.2/src/vellum/types/workflow_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/workflow_result_event_output_data.py` & `vellum_ai-0.5.2/src/vellum/types/workflow_result_event_output_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/workflow_result_event_output_data_array.py` & `vellum_ai-0.5.2/src/vellum/types/workflow_result_event_output_data_array.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/workflow_result_event_output_data_chat_history.py` & `vellum_ai-0.5.2/src/vellum/types/workflow_result_event_output_data_chat_history.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/workflow_result_event_output_data_error.py` & `vellum_ai-0.5.2/src/vellum/types/workflow_result_event_output_data_error.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/workflow_result_event_output_data_function_call.py` & `vellum_ai-0.5.2/src/vellum/types/workflow_result_event_output_data_function_call.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/workflow_result_event_output_data_json.py` & `vellum_ai-0.5.2/src/vellum/types/workflow_result_event_output_data_json.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/workflow_result_event_output_data_number.py` & `vellum_ai-0.5.2/src/vellum/types/workflow_result_event_output_data_number.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/workflow_result_event_output_data_search_results.py` & `vellum_ai-0.5.2/src/vellum/types/workflow_result_event_output_data_search_results.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/workflow_result_event_output_data_string.py` & `vellum_ai-0.5.2/src/vellum/types/workflow_result_event_output_data_string.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/src/vellum/types/workflow_stream_event.py` & `vellum_ai-0.5.2/src/vellum/types/workflow_stream_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.1/PKG-INFO` & `vellum_ai-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vellum-ai
-Version: 0.5.1
+Version: 0.5.2
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

