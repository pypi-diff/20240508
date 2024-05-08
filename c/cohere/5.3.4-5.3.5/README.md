# Comparing `tmp/cohere-5.3.4.tar.gz` & `tmp/cohere-5.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cohere-5.3.4.tar", max compression
+gzip compressed data, was "cohere-5.3.5.tar", max compression
```

## Comparing `cohere-5.3.4.tar` & `cohere-5.3.5.tar`

### file list

```diff
@@ -1,176 +1,180 @@
--rw-r--r--   0        0        0     1062 2024-04-30 10:29:15.125643 cohere-5.3.4/LICENSE
--rw-r--r--   0        0        0     2359 2024-04-30 10:29:15.125643 cohere-5.3.4/README.md
--rw-r--r--   0        0        0      698 2024-04-30 10:29:15.133643 cohere-5.3.4/pyproject.toml
--rw-r--r--   0        0        0     8012 2024-04-30 10:29:15.133643 cohere-5.3.4/src/cohere/__init__.py
--rw-r--r--   0        0        0   206571 2024-04-30 10:29:15.133643 cohere-5.3.4/src/cohere/base_client.py
--rw-r--r--   0        0        0    19723 2024-04-30 10:29:15.133643 cohere-5.3.4/src/cohere/client.py
--rw-r--r--   0        0        0       22 2024-04-30 10:29:15.133643 cohere-5.3.4/src/cohere/config.py
--rw-r--r--   0        0        0       65 2024-04-30 10:29:15.133643 cohere-5.3.4/src/cohere/connectors/__init__.py
--rw-r--r--   0        0        0    50199 2024-04-30 10:29:15.133643 cohere-5.3.4/src/cohere/connectors/client.py
--rw-r--r--   0        0        0     1006 2024-04-30 10:29:15.133643 cohere-5.3.4/src/cohere/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-30 10:29:15.133643 cohere-5.3.4/src/cohere/core/api_error.py
--rw-r--r--   0        0        0     2226 2024-04-30 10:29:15.133643 cohere-5.3.4/src/cohere/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-30 10:29:15.133643 cohere-5.3.4/src/cohere/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-04-30 10:29:15.133643 cohere-5.3.4/src/cohere/core/file.py
--rw-r--r--   0        0        0     5059 2024-04-30 10:29:15.133643 cohere-5.3.4/src/cohere/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-04-30 10:29:15.133643 cohere-5.3.4/src/cohere/core/jsonable_encoder.py
--rw-r--r--   0        0        0      329 2024-04-30 10:29:15.133643 cohere-5.3.4/src/cohere/core/pydantic_utilities.py
--rw-r--r--   0        0        0      330 2024-04-30 10:29:15.133643 cohere-5.3.4/src/cohere/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-04-30 10:29:15.133643 cohere-5.3.4/src/cohere/core/request_options.py
--rw-r--r--   0        0        0     7123 2024-04-30 10:29:15.133643 cohere-5.3.4/src/cohere/core/unchecked_base_model.py
--rw-r--r--   0        0        0      411 2024-04-30 10:29:15.133643 cohere-5.3.4/src/cohere/datasets/__init__.py
--rw-r--r--   0        0        0    35448 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/datasets/client.py
--rw-r--r--   0        0        0      565 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/datasets/types/__init__.py
--rw-r--r--   0        0        0     1002 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/datasets/types/datasets_create_response.py
--rw-r--r--   0        0        0     1398 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/datasets/types/datasets_create_response_dataset_parts.py
--rw-r--r--   0        0        0      959 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/datasets/types/datasets_get_response.py
--rw-r--r--   0        0        0     1057 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/datasets/types/datasets_get_usage_response.py
--rw-r--r--   0        0        0      998 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/datasets/types/datasets_list_response.py
--rw-r--r--   0        0        0      159 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/embed_jobs/__init__.py
--rw-r--r--   0        0        0    31599 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/embed_jobs/client.py
--rw-r--r--   0        0        0      187 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/embed_jobs/types/__init__.py
--rw-r--r--   0        0        0      169 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/embed_jobs/types/create_embed_job_request_truncate.py
--rw-r--r--   0        0        0      159 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/environment.py
--rw-r--r--   0        0        0      617 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/errors/__init__.py
--rw-r--r--   0        0        0      248 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/errors/bad_request_error.py
--rw-r--r--   0        0        0      247 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/errors/forbidden_error.py
--rw-r--r--   0        0        0      252 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/errors/internal_server_error.py
--rw-r--r--   0        0        0      246 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/errors/not_found_error.py
--rw-r--r--   0        0        0      290 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/errors/service_unavailable_error.py
--rw-r--r--   0        0        0      253 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/errors/too_many_requests_error.py
--rw-r--r--   0        0        0      284 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/errors/unauthorized_error.py
--rw-r--r--   0        0        0      953 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/finetuning/__init__.py
--rw-r--r--   0        0        0    62127 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/finetuning/client.py
--rw-r--r--   0        0        0      905 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/finetuning/finetuning/__init__.py
--rw-r--r--   0        0        0     1343 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/finetuning/finetuning/types/__init__.py
--rw-r--r--   0        0        0     1475 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/finetuning/finetuning/types/base_model.py
--rw-r--r--   0        0        0      305 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/finetuning/finetuning/types/base_type.py
--rw-r--r--   0        0        0     1175 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/finetuning/finetuning/types/create_finetuned_model_response.py
--rw-r--r--   0        0        0      140 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/finetuning/finetuning/types/delete_finetuned_model_response.py
--rw-r--r--   0        0        0     1083 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/finetuning/finetuning/types/error.py
--rw-r--r--   0        0        0     1400 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/finetuning/finetuning/types/event.py
--rw-r--r--   0        0        0     2357 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/finetuning/finetuning/types/finetuned_model.py
--rw-r--r--   0        0        0     1171 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/finetuning/finetuning/types/get_finetuned_model_response.py
--rw-r--r--   0        0        0     1823 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/finetuning/finetuning/types/hyperparameters.py
--rw-r--r--   0        0        0     1489 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/finetuning/finetuning/types/list_events_response.py
--rw-r--r--   0        0        0     1532 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/finetuning/finetuning/types/list_finetuned_models_response.py
--rw-r--r--   0        0        0     1463 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/finetuning/finetuning/types/list_training_step_metrics_response.py
--rw-r--r--   0        0        0     1577 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/finetuning/finetuning/types/settings.py
--rw-r--r--   0        0        0      402 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/finetuning/finetuning/types/status.py
--rw-r--r--   0        0        0      193 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/finetuning/finetuning/types/strategy.py
--rw-r--r--   0        0        0     1390 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/finetuning/finetuning/types/training_step_metrics.py
--rw-r--r--   0        0        0     1177 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/finetuning/finetuning/types/update_finetuned_model_response.py
--rw-r--r--   0        0        0      811 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/manually_maintained/cache.py
--rw-r--r--   0        0        0     3015 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/manually_maintained/tokenizers.py
--rw-r--r--   0        0        0       65 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/models/__init__.py
--rw-r--r--   0        0        0    13673 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/models/client.py
--rw-r--r--   0        0        0      730 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/overrides.py
--rw-r--r--   0        0        0        0 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/py.typed
--rw-r--r--   0        0        0    10202 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/__init__.py
--rw-r--r--   0        0        0     1260 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/api_meta.py
--rw-r--r--   0        0        0     1011 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/api_meta_api_version.py
--rw-r--r--   0        0        0     1434 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/api_meta_billed_units.py
--rw-r--r--   0        0        0     1177 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/api_meta_tokens.py
--rw-r--r--   0        0        0      168 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/auth_token_type.py
--rw-r--r--   0        0        0     1929 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/chat_citation.py
--rw-r--r--   0        0        0     1127 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/chat_citation_generation_event.py
--rw-r--r--   0        0        0     1861 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/chat_connector.py
--rw-r--r--   0        0        0     1297 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/chat_data_metrics.py
--rw-r--r--   0        0        0      117 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/chat_document.py
--rw-r--r--   0        0        0     1644 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/chat_message.py
--rw-r--r--   0        0        0      168 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/chat_message_role.py
--rw-r--r--   0        0        0      170 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/chat_request_citation_quality.py
--rw-r--r--   0        0        0     1708 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/chat_request_connectors_search_options.py
--rw-r--r--   0        0        0      189 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/chat_request_prompt_truncation.py
--rw-r--r--   0        0        0     1011 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/chat_request_tool_results_item.py
--rw-r--r--   0        0        0     1180 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/chat_search_queries_generation_event.py
--rw-r--r--   0        0        0     1247 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/chat_search_query.py
--rw-r--r--   0        0        0     1653 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/chat_search_result.py
--rw-r--r--   0        0        0     1055 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/chat_search_result_connector.py
--rw-r--r--   0        0        0     1417 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/chat_search_results_event.py
--rw-r--r--   0        0        0     1861 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/chat_stream_end_event.py
--rw-r--r--   0        0        0      225 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/chat_stream_end_event_finish_reason.py
--rw-r--r--   0        0        0      893 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/chat_stream_event.py
--rw-r--r--   0        0        0      176 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/chat_stream_request_citation_quality.py
--rw-r--r--   0        0        0     1714 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/chat_stream_request_connectors_search_options.py
--rw-r--r--   0        0        0      195 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/chat_stream_request_prompt_truncation.py
--rw-r--r--   0        0        0     1017 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/chat_stream_request_tool_results_item.py
--rw-r--r--   0        0        0     1102 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/chat_stream_start_event.py
--rw-r--r--   0        0        0     1068 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/chat_text_generation_event.py
--rw-r--r--   0        0        0     1040 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/chat_tool_calls_generation_event.py
--rw-r--r--   0        0        0     1004 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/classify_data_metrics.py
--rw-r--r--   0        0        0      971 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/classify_example.py
--rw-r--r--   0        0        0      171 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/classify_request_truncate.py
--rw-r--r--   0        0        0     1137 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/classify_response.py
--rw-r--r--   0        0        0     2560 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/classify_response_classifications_item.py
--rw-r--r--   0        0        0      214 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/classify_response_classifications_item_classification_type.py
--rw-r--r--   0        0        0      971 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/classify_response_classifications_item_labels_value.py
--rw-r--r--   0        0        0      220 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/compatible_endpoint.py
--rw-r--r--   0        0        0     3383 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/connector.py
--rw-r--r--   0        0        0      163 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/connector_auth_status.py
--rw-r--r--   0        0        0     1660 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/connector_o_auth.py
--rw-r--r--   0        0        0     1725 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/create_connector_o_auth.py
--rw-r--r--   0        0        0      960 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/create_connector_response.py
--rw-r--r--   0        0        0     1195 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/create_connector_service_auth.py
--rw-r--r--   0        0        0     1047 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/create_embed_job_response.py
--rw-r--r--   0        0        0     2209 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/dataset.py
--rw-r--r--   0        0        0     1648 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/dataset_part.py
--rw-r--r--   0        0        0      471 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/dataset_type.py
--rw-r--r--   0        0        0      222 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/dataset_validation_status.py
--rw-r--r--   0        0        0      135 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/delete_connector_response.py
--rw-r--r--   0        0        0     1068 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/detokenize_response.py
--rw-r--r--   0        0        0     1416 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/embed_by_type_response.py
--rw-r--r--   0        0        0     2271 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/embed_by_type_response_embeddings.py
--rw-r--r--   0        0        0     1364 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/embed_floats_response.py
--rw-r--r--   0        0        0      211 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/embed_input_type.py
--rw-r--r--   0        0        0     1864 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/embed_job.py
--rw-r--r--   0        0        0      201 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/embed_job_status.py
--rw-r--r--   0        0        0      156 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/embed_job_truncate.py
--rw-r--r--   0        0        0      168 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/embed_request_truncate.py
--rw-r--r--   0        0        0     1057 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/embed_response.py
--rw-r--r--   0        0        0      184 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/embedding_type.py
--rw-r--r--   0        0        0     1735 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/finetune_dataset_metrics.py
--rw-r--r--   0        0        0      222 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/finish_reason.py
--rw-r--r--   0        0        0      185 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/generate_request_return_likelihoods.py
--rw-r--r--   0        0        0      171 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/generate_request_truncate.py
--rw-r--r--   0        0        0     1197 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/generate_stream_end.py
--rw-r--r--   0        0        0     1101 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/generate_stream_end_response.py
--rw-r--r--   0        0        0     1311 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/generate_stream_error.py
--rw-r--r--   0        0        0      897 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/generate_stream_event.py
--rw-r--r--   0        0        0      191 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/generate_stream_request_return_likelihoods.py
--rw-r--r--   0        0        0      177 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/generate_stream_request_truncate.py
--rw-r--r--   0        0        0     1312 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/generate_stream_text.py
--rw-r--r--   0        0        0     1456 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/generate_streamed_response.py
--rw-r--r--   0        0        0     1254 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/generation.py
--rw-r--r--   0        0        0      957 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/get_connector_response.py
--rw-r--r--   0        0        0     2150 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/get_model_response.py
--rw-r--r--   0        0        0     1256 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/label_metric.py
--rw-r--r--   0        0        0     1095 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/list_connectors_response.py
--rw-r--r--   0        0        0      993 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/list_embed_job_response.py
--rw-r--r--   0        0        0     1187 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/list_models_response.py
--rw-r--r--   0        0        0     1024 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/metrics.py
--rw-r--r--   0        0        0     2953 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/non_streamed_chat_response.py
--rw-r--r--   0        0        0     1080 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/o_auth_authorize_response.py
--rw-r--r--   0        0        0      974 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/parse_info.py
--rw-r--r--   0        0        0      239 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/rerank_request_documents_item.py
--rw-r--r--   0        0        0     1001 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/rerank_request_documents_item_text.py
--rw-r--r--   0        0        0     1200 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/rerank_response.py
--rw-r--r--   0        0        0     1909 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/rerank_response_results_item.py
--rw-r--r--   0        0        0     1136 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/rerank_response_results_item_document.py
--rw-r--r--   0        0        0     1818 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/reranker_data_metrics.py
--rw-r--r--   0        0        0     1819 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/single_generation.py
--rw-r--r--   0        0        0     1248 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/single_generation_in_stream.py
--rw-r--r--   0        0        0      952 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/single_generation_token_likelihoods_item.py
--rw-r--r--   0        0        0     3157 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/streamed_chat_response.py
--rw-r--r--   0        0        0      179 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/summarize_request_extractiveness.py
--rw-r--r--   0        0        0      170 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/summarize_request_format.py
--rw-r--r--   0        0        0      173 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/summarize_request_length.py
--rw-r--r--   0        0        0     1201 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/summarize_response.py
--rw-r--r--   0        0        0     1127 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/tokenize_response.py
--rw-r--r--   0        0        0     1928 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/tool.py
--rw-r--r--   0        0        0     1221 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/tool_call.py
--rw-r--r--   0        0        0     1331 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/tool_parameter_definitions_value.py
--rw-r--r--   0        0        0      960 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/types/update_connector_response.py
--rw-r--r--   0        0        0    10036 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/utils.py
--rw-r--r--   0        0        0       74 2024-04-30 10:29:15.137643 cohere-5.3.4/src/cohere/version.py
--rw-r--r--   0        0        0     3060 1970-01-01 00:00:00.000000 cohere-5.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-08 11:43:14.680259 cohere-5.3.5/LICENSE
+-rw-r--r--   0        0        0     2359 2024-05-08 11:43:14.680259 cohere-5.3.5/README.md
+-rw-r--r--   0        0        0      698 2024-05-08 11:43:14.684259 cohere-5.3.5/pyproject.toml
+-rw-r--r--   0        0        0     8246 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/__init__.py
+-rw-r--r--   0        0        0   228964 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/base_client.py
+-rw-r--r--   0        0        0    19723 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/client.py
+-rw-r--r--   0        0        0       22 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/config.py
+-rw-r--r--   0        0        0       65 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/connectors/__init__.py
+-rw-r--r--   0        0        0    50609 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/connectors/client.py
+-rw-r--r--   0        0        0     1006 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/core/api_error.py
+-rw-r--r--   0        0        0     2226 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/core/file.py
+-rw-r--r--   0        0        0     5059 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      329 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/core/request_options.py
+-rw-r--r--   0        0        0     7123 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/core/unchecked_base_model.py
+-rw-r--r--   0        0        0      419 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/datasets/__init__.py
+-rw-r--r--   0        0        0    35730 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/datasets/client.py
+-rw-r--r--   0        0        0      578 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/datasets/types/__init__.py
+-rw-r--r--   0        0        0     1002 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/datasets/types/datasets_create_response.py
+-rw-r--r--   0        0        0     1402 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/datasets/types/datasets_create_response_dataset_parts_item.py
+-rw-r--r--   0        0        0      959 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/datasets/types/datasets_get_response.py
+-rw-r--r--   0        0        0     1057 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/datasets/types/datasets_get_usage_response.py
+-rw-r--r--   0        0        0      998 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/datasets/types/datasets_list_response.py
+-rw-r--r--   0        0        0      159 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/embed_jobs/__init__.py
+-rw-r--r--   0        0        0    31897 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/embed_jobs/client.py
+-rw-r--r--   0        0        0      187 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/embed_jobs/types/__init__.py
+-rw-r--r--   0        0        0      169 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/embed_jobs/types/create_embed_job_request_truncate.py
+-rw-r--r--   0        0        0      159 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/environment.py
+-rw-r--r--   0        0        0      617 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/errors/__init__.py
+-rw-r--r--   0        0        0      248 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/errors/bad_request_error.py
+-rw-r--r--   0        0        0      247 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/errors/forbidden_error.py
+-rw-r--r--   0        0        0      252 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/errors/internal_server_error.py
+-rw-r--r--   0        0        0      246 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/errors/not_found_error.py
+-rw-r--r--   0        0        0      290 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/errors/service_unavailable_error.py
+-rw-r--r--   0        0        0      326 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/errors/too_many_requests_error.py
+-rw-r--r--   0        0        0      284 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      953 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/__init__.py
+-rw-r--r--   0        0        0    62115 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/client.py
+-rw-r--r--   0        0        0      905 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/finetuning/__init__.py
+-rw-r--r--   0        0        0     1343 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/finetuning/types/__init__.py
+-rw-r--r--   0        0        0     1475 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/finetuning/types/base_model.py
+-rw-r--r--   0        0        0      273 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/finetuning/types/base_type.py
+-rw-r--r--   0        0        0     1175 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/finetuning/types/create_finetuned_model_response.py
+-rw-r--r--   0        0        0      140 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/finetuning/types/delete_finetuned_model_response.py
+-rw-r--r--   0        0        0     1083 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/finetuning/types/error.py
+-rw-r--r--   0        0        0     1400 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/finetuning/types/event.py
+-rw-r--r--   0        0        0     2357 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/finetuning/types/finetuned_model.py
+-rw-r--r--   0        0        0     1171 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/finetuning/types/get_finetuned_model_response.py
+-rw-r--r--   0        0        0     1823 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/finetuning/types/hyperparameters.py
+-rw-r--r--   0        0        0     1489 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/finetuning/types/list_events_response.py
+-rw-r--r--   0        0        0     1532 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/finetuning/types/list_finetuned_models_response.py
+-rw-r--r--   0        0        0     1463 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/finetuning/types/list_training_step_metrics_response.py
+-rw-r--r--   0        0        0     1577 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/finetuning/types/settings.py
+-rw-r--r--   0        0        0      402 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/finetuning/types/status.py
+-rw-r--r--   0        0        0      193 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/finetuning/types/strategy.py
+-rw-r--r--   0        0        0     1390 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/finetuning/types/training_step_metrics.py
+-rw-r--r--   0        0        0     1177 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/finetuning/types/update_finetuned_model_response.py
+-rw-r--r--   0        0        0      811 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/manually_maintained/cache.py
+-rw-r--r--   0        0        0     3015 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/manually_maintained/tokenizers.py
+-rw-r--r--   0        0        0       65 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/models/__init__.py
+-rw-r--r--   0        0        0    13859 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/models/client.py
+-rw-r--r--   0        0        0      730 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/overrides.py
+-rw-r--r--   0        0        0        0 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/py.typed
+-rw-r--r--   0        0        0    10562 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/__init__.py
+-rw-r--r--   0        0        0     1260 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/api_meta.py
+-rw-r--r--   0        0        0     1011 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/api_meta_api_version.py
+-rw-r--r--   0        0        0     1434 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/api_meta_billed_units.py
+-rw-r--r--   0        0        0     1177 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/api_meta_tokens.py
+-rw-r--r--   0        0        0      168 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/auth_token_type.py
+-rw-r--r--   0        0        0     1929 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_citation.py
+-rw-r--r--   0        0        0     1127 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_citation_generation_event.py
+-rw-r--r--   0        0        0     1861 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_connector.py
+-rw-r--r--   0        0        0     1297 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_data_metrics.py
+-rw-r--r--   0        0        0      117 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_document.py
+-rw-r--r--   0        0        0     1644 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_message.py
+-rw-r--r--   0        0        0      168 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_message_role.py
+-rw-r--r--   0        0        0      170 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_request_citation_quality.py
+-rw-r--r--   0        0        0     1708 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_request_connectors_search_options.py
+-rw-r--r--   0        0        0      189 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_request_prompt_truncation.py
+-rw-r--r--   0        0        0     1011 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_request_tool_results_item.py
+-rw-r--r--   0        0        0     1180 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_search_queries_generation_event.py
+-rw-r--r--   0        0        0     1247 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_search_query.py
+-rw-r--r--   0        0        0     1653 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_search_result.py
+-rw-r--r--   0        0        0     1055 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_search_result_connector.py
+-rw-r--r--   0        0        0     1417 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_search_results_event.py
+-rw-r--r--   0        0        0     1861 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_stream_end_event.py
+-rw-r--r--   0        0        0      225 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_stream_end_event_finish_reason.py
+-rw-r--r--   0        0        0      893 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_stream_event.py
+-rw-r--r--   0        0        0      176 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_stream_request_citation_quality.py
+-rw-r--r--   0        0        0     1714 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_stream_request_connectors_search_options.py
+-rw-r--r--   0        0        0      195 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_stream_request_prompt_truncation.py
+-rw-r--r--   0        0        0     1017 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_stream_request_tool_results_item.py
+-rw-r--r--   0        0        0     1102 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_stream_start_event.py
+-rw-r--r--   0        0        0     1068 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_text_generation_event.py
+-rw-r--r--   0        0        0     1040 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_tool_calls_generation_event.py
+-rw-r--r--   0        0        0     1005 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/check_api_key_response.py
+-rw-r--r--   0        0        0     1004 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/classify_data_metrics.py
+-rw-r--r--   0        0        0      971 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/classify_example.py
+-rw-r--r--   0        0        0      171 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/classify_request_truncate.py
+-rw-r--r--   0        0        0     1137 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/classify_response.py
+-rw-r--r--   0        0        0     2560 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/classify_response_classifications_item.py
+-rw-r--r--   0        0        0      214 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/classify_response_classifications_item_classification_type.py
+-rw-r--r--   0        0        0      971 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/classify_response_classifications_item_labels_value.py
+-rw-r--r--   0        0        0      220 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/compatible_endpoint.py
+-rw-r--r--   0        0        0     3383 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/connector.py
+-rw-r--r--   0        0        0      163 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/connector_auth_status.py
+-rw-r--r--   0        0        0     1660 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/connector_o_auth.py
+-rw-r--r--   0        0        0     1725 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/create_connector_o_auth.py
+-rw-r--r--   0        0        0      960 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/create_connector_response.py
+-rw-r--r--   0        0        0     1195 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/create_connector_service_auth.py
+-rw-r--r--   0        0        0     1047 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/create_embed_job_response.py
+-rw-r--r--   0        0        0     2209 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/dataset.py
+-rw-r--r--   0        0        0     1788 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/dataset_part.py
+-rw-r--r--   0        0        0      427 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/dataset_type.py
+-rw-r--r--   0        0        0      222 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/dataset_validation_status.py
+-rw-r--r--   0        0        0      135 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/delete_connector_response.py
+-rw-r--r--   0        0        0     1068 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/detokenize_response.py
+-rw-r--r--   0        0        0     1416 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/embed_by_type_response.py
+-rw-r--r--   0        0        0     2271 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/embed_by_type_response_embeddings.py
+-rw-r--r--   0        0        0     1364 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/embed_floats_response.py
+-rw-r--r--   0        0        0      211 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/embed_input_type.py
+-rw-r--r--   0        0        0     1864 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/embed_job.py
+-rw-r--r--   0        0        0      201 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/embed_job_status.py
+-rw-r--r--   0        0        0      156 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/embed_job_truncate.py
+-rw-r--r--   0        0        0      168 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/embed_request_truncate.py
+-rw-r--r--   0        0        0     1057 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/embed_response.py
+-rw-r--r--   0        0        0      184 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/embedding_type.py
+-rw-r--r--   0        0        0     1735 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/finetune_dataset_metrics.py
+-rw-r--r--   0        0        0      222 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/finish_reason.py
+-rw-r--r--   0        0        0      185 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/generate_request_return_likelihoods.py
+-rw-r--r--   0        0        0      171 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/generate_request_truncate.py
+-rw-r--r--   0        0        0     1197 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/generate_stream_end.py
+-rw-r--r--   0        0        0     1101 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/generate_stream_end_response.py
+-rw-r--r--   0        0        0     1311 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/generate_stream_error.py
+-rw-r--r--   0        0        0      897 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/generate_stream_event.py
+-rw-r--r--   0        0        0      191 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/generate_stream_request_return_likelihoods.py
+-rw-r--r--   0        0        0      177 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/generate_stream_request_truncate.py
+-rw-r--r--   0        0        0     1312 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/generate_stream_text.py
+-rw-r--r--   0        0        0     1456 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/generate_streamed_response.py
+-rw-r--r--   0        0        0     1254 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/generation.py
+-rw-r--r--   0        0        0      957 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/get_connector_response.py
+-rw-r--r--   0        0        0     2150 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/get_model_response.py
+-rw-r--r--   0        0        0     1256 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/label_metric.py
+-rw-r--r--   0        0        0     1095 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/list_connectors_response.py
+-rw-r--r--   0        0        0      993 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/list_embed_job_response.py
+-rw-r--r--   0        0        0     1187 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/list_models_response.py
+-rw-r--r--   0        0        0     1130 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/metrics.py
+-rw-r--r--   0        0        0     1115 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/metrics_embed_data.py
+-rw-r--r--   0        0        0     1154 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/metrics_embed_data_fields_item.py
+-rw-r--r--   0        0        0     2953 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/non_streamed_chat_response.py
+-rw-r--r--   0        0        0     1080 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/o_auth_authorize_response.py
+-rw-r--r--   0        0        0      974 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/parse_info.py
+-rw-r--r--   0        0        0      239 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/rerank_request_documents_item.py
+-rw-r--r--   0        0        0     1001 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/rerank_request_documents_item_text.py
+-rw-r--r--   0        0        0     1200 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/rerank_response.py
+-rw-r--r--   0        0        0     1909 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/rerank_response_results_item.py
+-rw-r--r--   0        0        0     1136 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/rerank_response_results_item_document.py
+-rw-r--r--   0        0        0     1818 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/reranker_data_metrics.py
+-rw-r--r--   0        0        0     1819 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/single_generation.py
+-rw-r--r--   0        0        0     1248 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/single_generation_in_stream.py
+-rw-r--r--   0        0        0      952 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/single_generation_token_likelihoods_item.py
+-rw-r--r--   0        0        0     3157 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/streamed_chat_response.py
+-rw-r--r--   0        0        0      179 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/summarize_request_extractiveness.py
+-rw-r--r--   0        0        0      170 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/summarize_request_format.py
+-rw-r--r--   0        0        0      173 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/summarize_request_length.py
+-rw-r--r--   0        0        0     1201 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/summarize_response.py
+-rw-r--r--   0        0        0     1127 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/tokenize_response.py
+-rw-r--r--   0        0        0      941 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/too_many_requests_error_body.py
+-rw-r--r--   0        0        0     1928 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/tool.py
+-rw-r--r--   0        0        0     1221 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/tool_call.py
+-rw-r--r--   0        0        0     1331 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/tool_parameter_definitions_value.py
+-rw-r--r--   0        0        0      960 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/update_connector_response.py
+-rw-r--r--   0        0        0    10036 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/utils.py
+-rw-r--r--   0        0        0       74 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/version.py
+-rw-r--r--   0        0        0     3060 1970-01-01 00:00:00.000000 cohere-5.3.5/PKG-INFO
```

### Comparing `cohere-5.3.4/LICENSE` & `cohere-5.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/README.md` & `cohere-5.3.5/README.md`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/pyproject.toml` & `cohere-5.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cohere"
-version = "5.3.4"
+version = "5.3.5"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
     { include = "cohere", from = "src"}
 ]
```

### Comparing `cohere-5.3.4/src/cohere/__init__.py` & `cohere-5.3.5/src/cohere/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     ChatStreamRequestCitationQuality,
     ChatStreamRequestConnectorsSearchOptions,
     ChatStreamRequestPromptTruncation,
     ChatStreamRequestToolResultsItem,
     ChatStreamStartEvent,
     ChatTextGenerationEvent,
     ChatToolCallsGenerationEvent,
+    CheckApiKeyResponse,
     ClassifyDataMetrics,
     ClassifyExample,
     ClassifyRequestTruncate,
     ClassifyResponse,
     ClassifyResponseClassificationsItem,
     ClassifyResponseClassificationsItemClassificationType,
     ClassifyResponseClassificationsItemLabelsValue,
@@ -84,14 +85,16 @@
     GetConnectorResponse,
     GetModelResponse,
     LabelMetric,
     ListConnectorsResponse,
     ListEmbedJobResponse,
     ListModelsResponse,
     Metrics,
+    MetricsEmbedData,
+    MetricsEmbedDataFieldsItem,
     NonStreamedChatResponse,
     OAuthAuthorizeResponse,
     ParseInfo,
     RerankRequestDocumentsItem,
     RerankRequestDocumentsItemText,
     RerankResponse,
     RerankResponseResultsItem,
@@ -109,14 +112,15 @@
     StreamedChatResponse_TextGeneration,
     StreamedChatResponse_ToolCallsGeneration,
     SummarizeRequestExtractiveness,
     SummarizeRequestFormat,
     SummarizeRequestLength,
     SummarizeResponse,
     TokenizeResponse,
+    TooManyRequestsErrorBody,
     Tool,
     ToolCall,
     ToolParameterDefinitionsValue,
     UpdateConnectorResponse,
 )
 from .errors import (
     BadRequestError,
@@ -127,15 +131,15 @@
     TooManyRequestsError,
     UnauthorizedError,
 )
 from . import connectors, datasets, embed_jobs, finetuning, models
 from .client import AsyncClient, Client
 from .datasets import (
     DatasetsCreateResponse,
-    DatasetsCreateResponseDatasetParts,
+    DatasetsCreateResponseDatasetPartsItem,
     DatasetsGetResponse,
     DatasetsGetUsageResponse,
     DatasetsListResponse,
 )
 from .embed_jobs import CreateEmbedJobRequestTruncate
 from .environment import ClientEnvironment
 from .version import __version__
@@ -170,14 +174,15 @@
     "ChatStreamRequestCitationQuality",
     "ChatStreamRequestConnectorsSearchOptions",
     "ChatStreamRequestPromptTruncation",
     "ChatStreamRequestToolResultsItem",
     "ChatStreamStartEvent",
     "ChatTextGenerationEvent",
     "ChatToolCallsGenerationEvent",
+    "CheckApiKeyResponse",
     "ClassifyDataMetrics",
     "ClassifyExample",
     "ClassifyRequestTruncate",
     "ClassifyResponse",
     "ClassifyResponseClassificationsItem",
     "ClassifyResponseClassificationsItemClassificationType",
     "ClassifyResponseClassificationsItemLabelsValue",
@@ -193,15 +198,15 @@
     "CreateEmbedJobRequestTruncate",
     "CreateEmbedJobResponse",
     "Dataset",
     "DatasetPart",
     "DatasetType",
     "DatasetValidationStatus",
     "DatasetsCreateResponse",
-    "DatasetsCreateResponseDatasetParts",
+    "DatasetsCreateResponseDatasetPartsItem",
     "DatasetsGetResponse",
     "DatasetsGetUsageResponse",
     "DatasetsListResponse",
     "DeleteConnectorResponse",
     "DetokenizeResponse",
     "EmbedByTypeResponse",
     "EmbedByTypeResponseEmbeddings",
@@ -236,14 +241,16 @@
     "GetModelResponse",
     "InternalServerError",
     "LabelMetric",
     "ListConnectorsResponse",
     "ListEmbedJobResponse",
     "ListModelsResponse",
     "Metrics",
+    "MetricsEmbedData",
+    "MetricsEmbedDataFieldsItem",
     "NonStreamedChatResponse",
     "NotFoundError",
     "OAuthAuthorizeResponse",
     "ParseInfo",
     "RerankRequestDocumentsItem",
     "RerankRequestDocumentsItemText",
     "RerankResponse",
@@ -264,14 +271,15 @@
     "StreamedChatResponse_ToolCallsGeneration",
     "SummarizeRequestExtractiveness",
     "SummarizeRequestFormat",
     "SummarizeRequestLength",
     "SummarizeResponse",
     "TokenizeResponse",
     "TooManyRequestsError",
+    "TooManyRequestsErrorBody",
     "Tool",
     "ToolCall",
     "ToolParameterDefinitionsValue",
     "UnauthorizedError",
     "UpdateConnectorResponse",
     "__version__",
     "connectors",
```

### Comparing `cohere-5.3.4/src/cohere/base_client.py` & `cohere-5.3.5/src/cohere/base_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from .types.chat_message import ChatMessage
 from .types.chat_request_citation_quality import ChatRequestCitationQuality
 from .types.chat_request_prompt_truncation import ChatRequestPromptTruncation
 from .types.chat_request_tool_results_item import ChatRequestToolResultsItem
 from .types.chat_stream_request_citation_quality import ChatStreamRequestCitationQuality
 from .types.chat_stream_request_prompt_truncation import ChatStreamRequestPromptTruncation
 from .types.chat_stream_request_tool_results_item import ChatStreamRequestToolResultsItem
+from .types.check_api_key_response import CheckApiKeyResponse
 from .types.classify_example import ClassifyExample
 from .types.classify_request_truncate import ClassifyRequestTruncate
 from .types.classify_response import ClassifyResponse
 from .types.detokenize_response import DetokenizeResponse
 from .types.embed_input_type import EmbedInputType
 from .types.embed_request_truncate import EmbedRequestTruncate
 from .types.embed_response import EmbedResponse
@@ -52,14 +53,15 @@
 from .types.rerank_response import RerankResponse
 from .types.streamed_chat_response import StreamedChatResponse
 from .types.summarize_request_extractiveness import SummarizeRequestExtractiveness
 from .types.summarize_request_format import SummarizeRequestFormat
 from .types.summarize_request_length import SummarizeRequestLength
 from .types.summarize_response import SummarizeResponse
 from .types.tokenize_response import TokenizeResponse
+from .types.too_many_requests_error_body import TooManyRequestsErrorBody
 from .types.tool import Tool
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class BaseCohere:
@@ -152,50 +154,58 @@
     ) -> typing.Iterator[StreamedChatResponse]:
         """
         Generates a text response to a user message.
         To learn how to use Chat with Streaming and RAG follow [this guide](https://docs.cohere.com/docs/cochat-beta#various-ways-of-using-the-chat-endpoint).
 
         Parameters:
             - message: str. Text input for the model to respond to.
+                            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - model: typing.Optional[str]. Defaults to `command-r-plus`.
 
                                            The name of a compatible [Cohere model](https://docs.cohere.com/docs/models) or the ID of a [fine-tuned](https://docs.cohere.com/docs/chat-fine-tuning) model.
+                                           Compatible Deployments: Cohere Platform, Private Deployments
 
             - preamble: typing.Optional[str]. When specified, the default Cohere preamble will be replaced with the provided one. Preambles are a part of the prompt used to adjust the model's overall behavior and conversation style, and use the `SYSTEM` role.
 
                                               The `SYSTEM` role is also used for the contents of the optional `chat_history=` parameter. When used with the `chat_history=` parameter it adds content throughout a conversation. Conversely, when used with the `preamble=` parameter it adds content at the start of the conversation only.
+                                              Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - chat_history: typing.Optional[typing.Sequence[ChatMessage]]. A list of previous messages between the user and the model, giving the model conversational context for responding to the user's `message`.
 
                                                                            Each item represents a single message in the chat history, excluding the current user turn. It has two properties: `role` and `message`. The `role` identifies the sender (`CHATBOT`, `SYSTEM`, or `USER`), while the `message` contains the text content.
 
                                                                            The chat_history parameter should not be used for `SYSTEM` messages in most cases. Instead, to add a `SYSTEM` role message at the beginning of a conversation, the `preamble` parameter should be used.
+                                                                           Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - conversation_id: typing.Optional[str]. An alternative to `chat_history`.
 
                                                      Providing a `conversation_id` creates or resumes a persisted conversation with the specified ID. The ID can be any non empty string.
+                                                     Compatible Deployments: Cohere Platform
 
             - prompt_truncation: typing.Optional[ChatStreamRequestPromptTruncation]. Defaults to `AUTO` when `connectors` are specified and `OFF` in all other cases.
 
                                                                                      Dictates how the prompt will be constructed.
 
                                                                                      With `prompt_truncation` set to "AUTO", some elements from `chat_history` and `documents` will be dropped in an attempt to construct a prompt that fits within the model's context length limit. During this process the order of the documents and chat history will be changed and ranked by relevance.
 
                                                                                      With `prompt_truncation` set to "AUTO_PRESERVE_ORDER", some elements from `chat_history` and `documents` will be dropped in an attempt to construct a prompt that fits within the model's context length limit. During this process the order of the documents and chat history will be preserved as they are inputted into the API.
 
                                                                                      With `prompt_truncation` set to "OFF", no elements will be dropped. If the sum of the inputs exceeds the model's context length limit, a `TooManyTokens` error will be returned.
+                                                                                     Compatible Deployments: Cohere Platform Only AUTO_PRESERVE_ORDER: Azure, AWS Sagemaker, Private Deployments
 
             - connectors: typing.Optional[typing.Sequence[ChatConnector]]. Accepts `{"id": "web-search"}`, and/or the `"id"` for a custom [connector](https://docs.cohere.com/docs/connectors), if you've [created](https://docs.cohere.com/docs/creating-and-deploying-a-connector) one.
 
                                                                            When specified, the model's reply will be enriched with information found by quering each of the connectors (RAG).
+                                                                           Compatible Deployments: Cohere Platform
 
             - search_queries_only: typing.Optional[bool]. Defaults to `false`.
 
                                                           When `true`, the response will only contain a list of generated search queries, but no search will take place, and no reply from the model to the user's `message` will be generated.
+                                                          Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - documents: typing.Optional[typing.Sequence[ChatDocument]]. A list of relevant documents that the model can cite to generate a more accurate reply. Each document is a string-string dictionary.
 
                                                                          Example:
                                                                          `[
                                                                            { "title": "Tall penguins", "text": "Emperor penguins are the tallest." },
                                                                            { "title": "Penguin habitats", "text": "Emperor penguins only live in Antarctica." },
@@ -206,56 +216,73 @@
                                                                          Some suggested keys are "text", "author", and "date". For better generation quality, it is recommended to keep the total word count of the strings in the dictionary to under 300 words.
 
                                                                          An `id` field (string) can be optionally supplied to identify the document in the citations. This field will not be passed to the model.
 
                                                                          An `_excludes` field (array of strings) can be optionally supplied to omit some key-value pairs from being shown to the model. The omitted fields will still show up in the citation object. The "_excludes" field will not be passed to the model.
 
                                                                          See ['Document Mode'](https://docs.cohere.com/docs/retrieval-augmented-generation-rag#document-mode) in the guide for more information.
+                                                                         Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - citation_quality: typing.Optional[ChatStreamRequestCitationQuality]. Defaults to `"accurate"`.
 
                                                                                    Dictates the approach taken to generating citations as part of the RAG flow by allowing the user to specify whether they want `"accurate"` results or `"fast"` results.
+                                                                                   Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - temperature: typing.Optional[float]. Defaults to `0.3`.
 
                                                    A non-negative float that tunes the degree of randomness in generation. Lower temperatures mean less random generations, and higher temperatures mean more random generations.
 
                                                    Randomness can be further maximized by increasing the  value of the `p` parameter.
+                                                   Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - max_tokens: typing.Optional[int]. The maximum number of tokens the model will generate as part of the response. Note: Setting a low value may result in incomplete generations.
+                                                Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - max_input_tokens: typing.Optional[int]. The maximum number of input tokens to send to the model. If not specified, `max_input_tokens` is the model's context length limit minus a small buffer.
 
                                                       Input will be truncated according to the `prompt_truncation` parameter.
+                                                      Compatible Deployments: Cohere Platform
 
             - k: typing.Optional[int]. Ensures only the top `k` most likely tokens are considered for generation at each step.
                                        Defaults to `0`, min value of `0`, max value of `500`.
+                                       Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - p: typing.Optional[float]. Ensures that only the most likely tokens, with total probability mass of `p`, are considered for generation at each step. If both `k` and `p` are enabled, `p` acts after `k`.
                                          Defaults to `0.75`. min value of `0.01`, max value of `0.99`.
+                                         Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - seed: typing.Optional[float]. If specified, the backend will make a best effort to sample tokens deterministically, such that repeated requests with the same seed and parameters should return the same result. However, determinism cannot be totally guaranteed.
+            - seed: typing.Optional[float]. If specified, the backend will make a best effort to sample tokens
+                                            deterministically, such that repeated requests with the same
+                                            seed and parameters should return the same result. However,
+                                            determinism cannot be totally guaranteed.
+                                            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - stop_sequences: typing.Optional[typing.Sequence[str]]. A list of up to 5 strings that the model will use to stop generation. If the model generates a string that matches any of the strings in the list, it will stop generating tokens and return the generated text up to that point not including the stop sequence.
+                                                                     Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - frequency_penalty: typing.Optional[float]. Defaults to `0.0`, min value of `0.0`, max value of `1.0`.
 
                                                          Used to reduce repetitiveness of generated tokens. The higher the value, the stronger a penalty is applied to previously present tokens, proportional to how many times they have already appeared in the prompt or prior generation.
+                                                         Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - presence_penalty: typing.Optional[float]. Defaults to `0.0`, min value of `0.0`, max value of `1.0`.
 
                                                         Used to reduce repetitiveness of generated tokens. Similar to `frequency_penalty`, except that this penalty is applied equally to all tokens that have already appeared, regardless of their exact frequencies.
+                                                        Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - raw_prompting: typing.Optional[bool]. When enabled, the user's prompt will be sent to the model without any pre-processing.
+            - raw_prompting: typing.Optional[bool]. When enabled, the user's prompt will be sent to the model without
+                                                    any pre-processing.
+                                                    Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - return_prompt: typing.Optional[bool]. The prompt is returned in the `prompt` response field when this is enabled.
 
             - tools: typing.Optional[typing.Sequence[Tool]]. A list of available tools (functions) that the model may suggest invoking before producing a text response.
 
                                                              When `tools` is passed (without `tool_results`), the `text` field in the response will be `""` and the `tool_calls` field in the response will be populated with a list of tool calls that need to be made. If no calls need to be made, the `tool_calls` array will be empty.
+                                                             Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - tool_results: typing.Optional[typing.Sequence[ChatStreamRequestToolResultsItem]]. A list of results from invoking tools recommended by the model in the previous chat turn. Results are used to produce a text response and will be referenced in citations. When using `tool_results`, `tools` must be passed as well.
                                                                                                 Each tool_result contains information about how it was invoked, as well as a list of outputs in the form of dictionaries.
 
                                                                                                 **Note**: `outputs` must be a list of objects. If your tool returns a single object (eg `{"status": 200}`), make sure to wrap it in a list.
                                                                                                 ```
                                                                                                 tool_results = [
@@ -270,38 +297,93 @@
                                                                                                       <key>: <value>
                                                                                                     }]
                                                                                                   },
                                                                                                   ...
                                                                                                 ]
                                                                                                 ```
                                                                                                 **Note**: Chat calls with `tool_results` should not be included in the Chat history to avoid duplication of the message text.
+                                                                                                Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from cohere import ChatMessage
+        from cohere import (
+            ChatConnector,
+            ChatMessage,
+            ChatStreamRequestConnectorsSearchOptions,
+            ChatStreamRequestToolResultsItem,
+            Tool,
+            ToolCall,
+            ToolParameterDefinitionsValue,
+        )
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         client.chat_stream(
-            message="Can you give me a global market overview of solar panels?",
+            message="string",
+            model="string",
+            preamble="string",
             chat_history=[
                 ChatMessage(
                     role="CHATBOT",
-                    message="Hi!",
-                ),
-                ChatMessage(
-                    role="CHATBOT",
-                    message="How can I help you today?",
-                ),
+                    message="string",
+                )
             ],
+            conversation_id="string",
             prompt_truncation="OFF",
-            temperature=0.3,
+            connectors=[
+                ChatConnector(
+                    id="string",
+                    user_access_token="string",
+                    continue_on_failure=True,
+                    options={"string": {"key": "value"}},
+                )
+            ],
+            search_queries_only=True,
+            documents=[{{"key": "value"}: {"key": "value"}}],
+            citation_quality="fast",
+            temperature=1.1,
+            max_tokens=1,
+            max_input_tokens=1,
+            k=1,
+            p=1.1,
+            seed=1.1,
+            stop_sequences=["string"],
+            connectors_search_options=ChatStreamRequestConnectorsSearchOptions(
+                model={"key": "value"},
+                temperature={"key": "value"},
+                max_tokens={"key": "value"},
+                preamble={"key": "value"},
+                seed=1.1,
+            ),
+            frequency_penalty=1.1,
+            presence_penalty=1.1,
+            raw_prompting=True,
+            return_prompt=True,
+            tools=[
+                Tool(
+                    name="string",
+                    description="string",
+                    parameter_definitions={
+                        "string": ToolParameterDefinitionsValue(
+                            description="string",
+                            type="string",
+                            required=True,
+                        )
+                    },
+                )
+            ],
+            tool_results=[
+                ChatStreamRequestToolResultsItem(
+                    call=ToolCall(),
+                    outputs=[{"string": {"key": "value"}}],
+                )
+            ],
         )
         """
         _request: typing.Dict[str, typing.Any] = {"message": message, "stream": True}
         if model is not OMIT:
             _request["model"] = model
         if preamble is not OMIT:
             _request["preamble"] = preamble
@@ -382,15 +464,15 @@
                         if len(_text) == 0:
                             continue
                         yield typing.cast(StreamedChatResponse, construct_type(type_=StreamedChatResponse, object_=json.loads(_text)))  # type: ignore
                 return
             _response.read()
             if _response.status_code == 429:
                 raise TooManyRequestsError(
-                    typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                    typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
                 )
             try:
                 _response_json = _response.json()
             except JSONDecodeError:
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
 
@@ -424,50 +506,58 @@
     ) -> NonStreamedChatResponse:
         """
         Generates a text response to a user message.
         To learn how to use Chat with Streaming and RAG follow [this guide](https://docs.cohere.com/docs/cochat-beta#various-ways-of-using-the-chat-endpoint).
 
         Parameters:
             - message: str. Text input for the model to respond to.
+                            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - model: typing.Optional[str]. Defaults to `command-r-plus`.
 
                                            The name of a compatible [Cohere model](https://docs.cohere.com/docs/models) or the ID of a [fine-tuned](https://docs.cohere.com/docs/chat-fine-tuning) model.
+                                           Compatible Deployments: Cohere Platform, Private Deployments
 
             - preamble: typing.Optional[str]. When specified, the default Cohere preamble will be replaced with the provided one. Preambles are a part of the prompt used to adjust the model's overall behavior and conversation style, and use the `SYSTEM` role.
 
                                               The `SYSTEM` role is also used for the contents of the optional `chat_history=` parameter. When used with the `chat_history=` parameter it adds content throughout a conversation. Conversely, when used with the `preamble=` parameter it adds content at the start of the conversation only.
+                                              Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - chat_history: typing.Optional[typing.Sequence[ChatMessage]]. A list of previous messages between the user and the model, giving the model conversational context for responding to the user's `message`.
 
                                                                            Each item represents a single message in the chat history, excluding the current user turn. It has two properties: `role` and `message`. The `role` identifies the sender (`CHATBOT`, `SYSTEM`, or `USER`), while the `message` contains the text content.
 
                                                                            The chat_history parameter should not be used for `SYSTEM` messages in most cases. Instead, to add a `SYSTEM` role message at the beginning of a conversation, the `preamble` parameter should be used.
+                                                                           Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - conversation_id: typing.Optional[str]. An alternative to `chat_history`.
 
                                                      Providing a `conversation_id` creates or resumes a persisted conversation with the specified ID. The ID can be any non empty string.
+                                                     Compatible Deployments: Cohere Platform
 
             - prompt_truncation: typing.Optional[ChatRequestPromptTruncation]. Defaults to `AUTO` when `connectors` are specified and `OFF` in all other cases.
 
                                                                                Dictates how the prompt will be constructed.
 
                                                                                With `prompt_truncation` set to "AUTO", some elements from `chat_history` and `documents` will be dropped in an attempt to construct a prompt that fits within the model's context length limit. During this process the order of the documents and chat history will be changed and ranked by relevance.
 
                                                                                With `prompt_truncation` set to "AUTO_PRESERVE_ORDER", some elements from `chat_history` and `documents` will be dropped in an attempt to construct a prompt that fits within the model's context length limit. During this process the order of the documents and chat history will be preserved as they are inputted into the API.
 
                                                                                With `prompt_truncation` set to "OFF", no elements will be dropped. If the sum of the inputs exceeds the model's context length limit, a `TooManyTokens` error will be returned.
+                                                                               Compatible Deployments: Cohere Platform Only AUTO_PRESERVE_ORDER: Azure, AWS Sagemaker, Private Deployments
 
             - connectors: typing.Optional[typing.Sequence[ChatConnector]]. Accepts `{"id": "web-search"}`, and/or the `"id"` for a custom [connector](https://docs.cohere.com/docs/connectors), if you've [created](https://docs.cohere.com/docs/creating-and-deploying-a-connector) one.
 
                                                                            When specified, the model's reply will be enriched with information found by quering each of the connectors (RAG).
+                                                                           Compatible Deployments: Cohere Platform
 
             - search_queries_only: typing.Optional[bool]. Defaults to `false`.
 
                                                           When `true`, the response will only contain a list of generated search queries, but no search will take place, and no reply from the model to the user's `message` will be generated.
+                                                          Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - documents: typing.Optional[typing.Sequence[ChatDocument]]. A list of relevant documents that the model can cite to generate a more accurate reply. Each document is a string-string dictionary.
 
                                                                          Example:
                                                                          `[
                                                                            { "title": "Tall penguins", "text": "Emperor penguins are the tallest." },
                                                                            { "title": "Penguin habitats", "text": "Emperor penguins only live in Antarctica." },
@@ -478,56 +568,73 @@
                                                                          Some suggested keys are "text", "author", and "date". For better generation quality, it is recommended to keep the total word count of the strings in the dictionary to under 300 words.
 
                                                                          An `id` field (string) can be optionally supplied to identify the document in the citations. This field will not be passed to the model.
 
                                                                          An `_excludes` field (array of strings) can be optionally supplied to omit some key-value pairs from being shown to the model. The omitted fields will still show up in the citation object. The "_excludes" field will not be passed to the model.
 
                                                                          See ['Document Mode'](https://docs.cohere.com/docs/retrieval-augmented-generation-rag#document-mode) in the guide for more information.
+                                                                         Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - citation_quality: typing.Optional[ChatRequestCitationQuality]. Defaults to `"accurate"`.
 
                                                                              Dictates the approach taken to generating citations as part of the RAG flow by allowing the user to specify whether they want `"accurate"` results or `"fast"` results.
+                                                                             Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - temperature: typing.Optional[float]. Defaults to `0.3`.
 
                                                    A non-negative float that tunes the degree of randomness in generation. Lower temperatures mean less random generations, and higher temperatures mean more random generations.
 
                                                    Randomness can be further maximized by increasing the  value of the `p` parameter.
+                                                   Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - max_tokens: typing.Optional[int]. The maximum number of tokens the model will generate as part of the response. Note: Setting a low value may result in incomplete generations.
+                                                Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - max_input_tokens: typing.Optional[int]. The maximum number of input tokens to send to the model. If not specified, `max_input_tokens` is the model's context length limit minus a small buffer.
 
                                                       Input will be truncated according to the `prompt_truncation` parameter.
+                                                      Compatible Deployments: Cohere Platform
 
             - k: typing.Optional[int]. Ensures only the top `k` most likely tokens are considered for generation at each step.
                                        Defaults to `0`, min value of `0`, max value of `500`.
+                                       Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - p: typing.Optional[float]. Ensures that only the most likely tokens, with total probability mass of `p`, are considered for generation at each step. If both `k` and `p` are enabled, `p` acts after `k`.
                                          Defaults to `0.75`. min value of `0.01`, max value of `0.99`.
+                                         Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - seed: typing.Optional[float]. If specified, the backend will make a best effort to sample tokens deterministically, such that repeated requests with the same seed and parameters should return the same result. However, determinism cannot be totally guaranteed.
+            - seed: typing.Optional[float]. If specified, the backend will make a best effort to sample tokens
+                                            deterministically, such that repeated requests with the same
+                                            seed and parameters should return the same result. However,
+                                            determinism cannot be totally guaranteed.
+                                            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - stop_sequences: typing.Optional[typing.Sequence[str]]. A list of up to 5 strings that the model will use to stop generation. If the model generates a string that matches any of the strings in the list, it will stop generating tokens and return the generated text up to that point not including the stop sequence.
+                                                                     Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - frequency_penalty: typing.Optional[float]. Defaults to `0.0`, min value of `0.0`, max value of `1.0`.
 
                                                          Used to reduce repetitiveness of generated tokens. The higher the value, the stronger a penalty is applied to previously present tokens, proportional to how many times they have already appeared in the prompt or prior generation.
+                                                         Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - presence_penalty: typing.Optional[float]. Defaults to `0.0`, min value of `0.0`, max value of `1.0`.
 
                                                         Used to reduce repetitiveness of generated tokens. Similar to `frequency_penalty`, except that this penalty is applied equally to all tokens that have already appeared, regardless of their exact frequencies.
+                                                        Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - raw_prompting: typing.Optional[bool]. When enabled, the user's prompt will be sent to the model without any pre-processing.
+            - raw_prompting: typing.Optional[bool]. When enabled, the user's prompt will be sent to the model without
+                                                    any pre-processing.
+                                                    Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - return_prompt: typing.Optional[bool]. The prompt is returned in the `prompt` response field when this is enabled.
 
             - tools: typing.Optional[typing.Sequence[Tool]]. A list of available tools (functions) that the model may suggest invoking before producing a text response.
 
                                                              When `tools` is passed (without `tool_results`), the `text` field in the response will be `""` and the `tool_calls` field in the response will be populated with a list of tool calls that need to be made. If no calls need to be made, the `tool_calls` array will be empty.
+                                                             Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - tool_results: typing.Optional[typing.Sequence[ChatRequestToolResultsItem]]. A list of results from invoking tools recommended by the model in the previous chat turn. Results are used to produce a text response and will be referenced in citations. When using `tool_results`, `tools` must be passed as well.
                                                                                           Each tool_result contains information about how it was invoked, as well as a list of outputs in the form of dictionaries.
 
                                                                                           **Note**: `outputs` must be a list of objects. If your tool returns a single object (eg `{"status": 200}`), make sure to wrap it in a list.
                                                                                           ```
                                                                                           tool_results = [
@@ -542,14 +649,15 @@
                                                                                                 <key>: <value>
                                                                                               }]
                                                                                             },
                                                                                             ...
                                                                                           ]
                                                                                           ```
                                                                                           **Note**: Chat calls with `tool_results` should not be included in the Chat history to avoid duplication of the message text.
+                                                                                          Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from cohere import ChatMessage
         from cohere.client import Client
 
         client = Client(
@@ -643,15 +751,15 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return typing.cast(NonStreamedChatResponse, construct_type(type_=NonStreamedChatResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
@@ -742,16 +850,30 @@
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         client.generate_stream(
-            prompt="Please explain to me how LLMs work",
-            preset="my-preset-a58sbd",
+            prompt="string",
+            model="string",
+            num_generations=1,
+            max_tokens=1,
+            truncate="NONE",
+            temperature=1.1,
+            seed=1.1,
+            preset="string",
+            end_sequences=["string"],
+            stop_sequences=["string"],
+            k=1,
+            p=1.1,
+            frequency_penalty=1.1,
+            presence_penalty=1.1,
+            return_likelihoods="GENERATION",
+            raw_prompting=True,
         )
         """
         _request: typing.Dict[str, typing.Any] = {"prompt": prompt, "stream": True}
         if model is not OMIT:
             _request["model"] = model
         if num_generations is not OMIT:
             _request["num_generations"] = num_generations
@@ -822,15 +944,15 @@
             _response.read()
             if _response.status_code == 400:
                 raise BadRequestError(
                     typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
                 )
             if _response.status_code == 429:
                 raise TooManyRequestsError(
-                    typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                    typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
                 )
             if _response.status_code == 500:
                 raise InternalServerError(
                     typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
                 )
             try:
                 _response_json = _response.json()
@@ -926,15 +1048,14 @@
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         client.generate(
             prompt="Please explain to me how LLMs work",
-            preset="my-preset-a58sbd",
         )
         """
         _request: typing.Dict[str, typing.Any] = {"prompt": prompt, "stream": False}
         if model is not OMIT:
             _request["model"] = model
         if num_generations is not OMIT:
             _request["num_generations"] = num_generations
@@ -994,15 +1115,15 @@
             return typing.cast(Generation, construct_type(type_=Generation, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 500:
             raise InternalServerError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
@@ -1113,15 +1234,15 @@
             return typing.cast(EmbedResponse, construct_type(type_=EmbedResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 500:
             raise InternalServerError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
@@ -1168,15 +1289,15 @@
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         client.rerank(
-            model="rerank-english-v2.0",
+            model="rerank-english-v3.0",
             query="What is the capital of the United States?",
             documents=[
                 "Carson City is the capital city of the American state of Nevada.",
                 "The Commonwealth of the Northern Mariana Islands is a group of islands in the Pacific Ocean. Its capital is Saipan.",
                 "Washington, D.C. (also known as simply Washington or D.C., and officially as the District of Columbia) is the capital of the United States. It is a federal district.",
                 "Capital punishment (the death penalty) has existed in the United States since beforethe United States was a country. As of 2017, capital punishment is legal in 30 of the 50 states.",
             ],
@@ -1219,15 +1340,15 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return typing.cast(RerankResponse, construct_type(type_=RerankResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
@@ -1307,15 +1428,14 @@
                     label="Not spam",
                 ),
                 ClassifyExample(
                     text="Pre-read for tomorrow",
                     label="Not spam",
                 ),
             ],
-            preset="my-preset-a58sbd",
         )
         """
         _request: typing.Dict[str, typing.Any] = {"inputs": inputs}
         if examples is not OMIT:
             _request["examples"] = examples
         if model is not OMIT:
             _request["model"] = model
@@ -1353,15 +1473,15 @@
             return typing.cast(ClassifyResponse, construct_type(type_=ClassifyResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 500:
             raise InternalServerError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
@@ -1454,15 +1574,15 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return typing.cast(SummarizeResponse, construct_type(type_=SummarizeResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
@@ -1520,15 +1640,15 @@
             return typing.cast(TokenizeResponse, construct_type(type_=TokenizeResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 500:
             raise InternalServerError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
@@ -1586,15 +1706,65 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return typing.cast(DetokenizeResponse, construct_type(type_=DetokenizeResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
+            )
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    def check_api_key(self, *, request_options: typing.Optional[RequestOptions] = None) -> CheckApiKeyResponse:
+        """
+        Checks that the api key in the Authorization header is valid and active
+
+        Parameters:
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from cohere.client import Client
+
+        client = Client(
+            client_name="YOUR_CLIENT_NAME",
+            token="YOUR_TOKEN",
+        )
+        client.check_api_key()
+        """
+        _response = self._client_wrapper.httpx_client.request(
+            "POST",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "check-api-key"),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
+            if request_options is not None
+            else None,
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
+        )
+        if 200 <= _response.status_code < 300:
+            return typing.cast(CheckApiKeyResponse, construct_type(type_=CheckApiKeyResponse, object_=_response.json()))  # type: ignore
+        if _response.status_code == 429:
+            raise TooManyRequestsError(
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
@@ -1689,50 +1859,58 @@
     ) -> typing.AsyncIterator[StreamedChatResponse]:
         """
         Generates a text response to a user message.
         To learn how to use Chat with Streaming and RAG follow [this guide](https://docs.cohere.com/docs/cochat-beta#various-ways-of-using-the-chat-endpoint).
 
         Parameters:
             - message: str. Text input for the model to respond to.
+                            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - model: typing.Optional[str]. Defaults to `command-r-plus`.
 
                                            The name of a compatible [Cohere model](https://docs.cohere.com/docs/models) or the ID of a [fine-tuned](https://docs.cohere.com/docs/chat-fine-tuning) model.
+                                           Compatible Deployments: Cohere Platform, Private Deployments
 
             - preamble: typing.Optional[str]. When specified, the default Cohere preamble will be replaced with the provided one. Preambles are a part of the prompt used to adjust the model's overall behavior and conversation style, and use the `SYSTEM` role.
 
                                               The `SYSTEM` role is also used for the contents of the optional `chat_history=` parameter. When used with the `chat_history=` parameter it adds content throughout a conversation. Conversely, when used with the `preamble=` parameter it adds content at the start of the conversation only.
+                                              Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - chat_history: typing.Optional[typing.Sequence[ChatMessage]]. A list of previous messages between the user and the model, giving the model conversational context for responding to the user's `message`.
 
                                                                            Each item represents a single message in the chat history, excluding the current user turn. It has two properties: `role` and `message`. The `role` identifies the sender (`CHATBOT`, `SYSTEM`, or `USER`), while the `message` contains the text content.
 
                                                                            The chat_history parameter should not be used for `SYSTEM` messages in most cases. Instead, to add a `SYSTEM` role message at the beginning of a conversation, the `preamble` parameter should be used.
+                                                                           Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - conversation_id: typing.Optional[str]. An alternative to `chat_history`.
 
                                                      Providing a `conversation_id` creates or resumes a persisted conversation with the specified ID. The ID can be any non empty string.
+                                                     Compatible Deployments: Cohere Platform
 
             - prompt_truncation: typing.Optional[ChatStreamRequestPromptTruncation]. Defaults to `AUTO` when `connectors` are specified and `OFF` in all other cases.
 
                                                                                      Dictates how the prompt will be constructed.
 
                                                                                      With `prompt_truncation` set to "AUTO", some elements from `chat_history` and `documents` will be dropped in an attempt to construct a prompt that fits within the model's context length limit. During this process the order of the documents and chat history will be changed and ranked by relevance.
 
                                                                                      With `prompt_truncation` set to "AUTO_PRESERVE_ORDER", some elements from `chat_history` and `documents` will be dropped in an attempt to construct a prompt that fits within the model's context length limit. During this process the order of the documents and chat history will be preserved as they are inputted into the API.
 
                                                                                      With `prompt_truncation` set to "OFF", no elements will be dropped. If the sum of the inputs exceeds the model's context length limit, a `TooManyTokens` error will be returned.
+                                                                                     Compatible Deployments: Cohere Platform Only AUTO_PRESERVE_ORDER: Azure, AWS Sagemaker, Private Deployments
 
             - connectors: typing.Optional[typing.Sequence[ChatConnector]]. Accepts `{"id": "web-search"}`, and/or the `"id"` for a custom [connector](https://docs.cohere.com/docs/connectors), if you've [created](https://docs.cohere.com/docs/creating-and-deploying-a-connector) one.
 
                                                                            When specified, the model's reply will be enriched with information found by quering each of the connectors (RAG).
+                                                                           Compatible Deployments: Cohere Platform
 
             - search_queries_only: typing.Optional[bool]. Defaults to `false`.
 
                                                           When `true`, the response will only contain a list of generated search queries, but no search will take place, and no reply from the model to the user's `message` will be generated.
+                                                          Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - documents: typing.Optional[typing.Sequence[ChatDocument]]. A list of relevant documents that the model can cite to generate a more accurate reply. Each document is a string-string dictionary.
 
                                                                          Example:
                                                                          `[
                                                                            { "title": "Tall penguins", "text": "Emperor penguins are the tallest." },
                                                                            { "title": "Penguin habitats", "text": "Emperor penguins only live in Antarctica." },
@@ -1743,56 +1921,73 @@
                                                                          Some suggested keys are "text", "author", and "date". For better generation quality, it is recommended to keep the total word count of the strings in the dictionary to under 300 words.
 
                                                                          An `id` field (string) can be optionally supplied to identify the document in the citations. This field will not be passed to the model.
 
                                                                          An `_excludes` field (array of strings) can be optionally supplied to omit some key-value pairs from being shown to the model. The omitted fields will still show up in the citation object. The "_excludes" field will not be passed to the model.
 
                                                                          See ['Document Mode'](https://docs.cohere.com/docs/retrieval-augmented-generation-rag#document-mode) in the guide for more information.
+                                                                         Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - citation_quality: typing.Optional[ChatStreamRequestCitationQuality]. Defaults to `"accurate"`.
 
                                                                                    Dictates the approach taken to generating citations as part of the RAG flow by allowing the user to specify whether they want `"accurate"` results or `"fast"` results.
+                                                                                   Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - temperature: typing.Optional[float]. Defaults to `0.3`.
 
                                                    A non-negative float that tunes the degree of randomness in generation. Lower temperatures mean less random generations, and higher temperatures mean more random generations.
 
                                                    Randomness can be further maximized by increasing the  value of the `p` parameter.
+                                                   Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - max_tokens: typing.Optional[int]. The maximum number of tokens the model will generate as part of the response. Note: Setting a low value may result in incomplete generations.
+                                                Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - max_input_tokens: typing.Optional[int]. The maximum number of input tokens to send to the model. If not specified, `max_input_tokens` is the model's context length limit minus a small buffer.
 
                                                       Input will be truncated according to the `prompt_truncation` parameter.
+                                                      Compatible Deployments: Cohere Platform
 
             - k: typing.Optional[int]. Ensures only the top `k` most likely tokens are considered for generation at each step.
                                        Defaults to `0`, min value of `0`, max value of `500`.
+                                       Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - p: typing.Optional[float]. Ensures that only the most likely tokens, with total probability mass of `p`, are considered for generation at each step. If both `k` and `p` are enabled, `p` acts after `k`.
                                          Defaults to `0.75`. min value of `0.01`, max value of `0.99`.
+                                         Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - seed: typing.Optional[float]. If specified, the backend will make a best effort to sample tokens deterministically, such that repeated requests with the same seed and parameters should return the same result. However, determinism cannot be totally guaranteed.
+            - seed: typing.Optional[float]. If specified, the backend will make a best effort to sample tokens
+                                            deterministically, such that repeated requests with the same
+                                            seed and parameters should return the same result. However,
+                                            determinism cannot be totally guaranteed.
+                                            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - stop_sequences: typing.Optional[typing.Sequence[str]]. A list of up to 5 strings that the model will use to stop generation. If the model generates a string that matches any of the strings in the list, it will stop generating tokens and return the generated text up to that point not including the stop sequence.
+                                                                     Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - frequency_penalty: typing.Optional[float]. Defaults to `0.0`, min value of `0.0`, max value of `1.0`.
 
                                                          Used to reduce repetitiveness of generated tokens. The higher the value, the stronger a penalty is applied to previously present tokens, proportional to how many times they have already appeared in the prompt or prior generation.
+                                                         Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - presence_penalty: typing.Optional[float]. Defaults to `0.0`, min value of `0.0`, max value of `1.0`.
 
                                                         Used to reduce repetitiveness of generated tokens. Similar to `frequency_penalty`, except that this penalty is applied equally to all tokens that have already appeared, regardless of their exact frequencies.
+                                                        Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - raw_prompting: typing.Optional[bool]. When enabled, the user's prompt will be sent to the model without any pre-processing.
+            - raw_prompting: typing.Optional[bool]. When enabled, the user's prompt will be sent to the model without
+                                                    any pre-processing.
+                                                    Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - return_prompt: typing.Optional[bool]. The prompt is returned in the `prompt` response field when this is enabled.
 
             - tools: typing.Optional[typing.Sequence[Tool]]. A list of available tools (functions) that the model may suggest invoking before producing a text response.
 
                                                              When `tools` is passed (without `tool_results`), the `text` field in the response will be `""` and the `tool_calls` field in the response will be populated with a list of tool calls that need to be made. If no calls need to be made, the `tool_calls` array will be empty.
+                                                             Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - tool_results: typing.Optional[typing.Sequence[ChatStreamRequestToolResultsItem]]. A list of results from invoking tools recommended by the model in the previous chat turn. Results are used to produce a text response and will be referenced in citations. When using `tool_results`, `tools` must be passed as well.
                                                                                                 Each tool_result contains information about how it was invoked, as well as a list of outputs in the form of dictionaries.
 
                                                                                                 **Note**: `outputs` must be a list of objects. If your tool returns a single object (eg `{"status": 200}`), make sure to wrap it in a list.
                                                                                                 ```
                                                                                                 tool_results = [
@@ -1807,38 +2002,93 @@
                                                                                                       <key>: <value>
                                                                                                     }]
                                                                                                   },
                                                                                                   ...
                                                                                                 ]
                                                                                                 ```
                                                                                                 **Note**: Chat calls with `tool_results` should not be included in the Chat history to avoid duplication of the message text.
+                                                                                                Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from cohere import ChatMessage
+        from cohere import (
+            ChatConnector,
+            ChatMessage,
+            ChatStreamRequestConnectorsSearchOptions,
+            ChatStreamRequestToolResultsItem,
+            Tool,
+            ToolCall,
+            ToolParameterDefinitionsValue,
+        )
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         await client.chat_stream(
-            message="Can you give me a global market overview of solar panels?",
+            message="string",
+            model="string",
+            preamble="string",
             chat_history=[
                 ChatMessage(
                     role="CHATBOT",
-                    message="Hi!",
-                ),
-                ChatMessage(
-                    role="CHATBOT",
-                    message="How can I help you today?",
-                ),
+                    message="string",
+                )
             ],
+            conversation_id="string",
             prompt_truncation="OFF",
-            temperature=0.3,
+            connectors=[
+                ChatConnector(
+                    id="string",
+                    user_access_token="string",
+                    continue_on_failure=True,
+                    options={"string": {"key": "value"}},
+                )
+            ],
+            search_queries_only=True,
+            documents=[{{"key": "value"}: {"key": "value"}}],
+            citation_quality="fast",
+            temperature=1.1,
+            max_tokens=1,
+            max_input_tokens=1,
+            k=1,
+            p=1.1,
+            seed=1.1,
+            stop_sequences=["string"],
+            connectors_search_options=ChatStreamRequestConnectorsSearchOptions(
+                model={"key": "value"},
+                temperature={"key": "value"},
+                max_tokens={"key": "value"},
+                preamble={"key": "value"},
+                seed=1.1,
+            ),
+            frequency_penalty=1.1,
+            presence_penalty=1.1,
+            raw_prompting=True,
+            return_prompt=True,
+            tools=[
+                Tool(
+                    name="string",
+                    description="string",
+                    parameter_definitions={
+                        "string": ToolParameterDefinitionsValue(
+                            description="string",
+                            type="string",
+                            required=True,
+                        )
+                    },
+                )
+            ],
+            tool_results=[
+                ChatStreamRequestToolResultsItem(
+                    call=ToolCall(),
+                    outputs=[{"string": {"key": "value"}}],
+                )
+            ],
         )
         """
         _request: typing.Dict[str, typing.Any] = {"message": message, "stream": True}
         if model is not OMIT:
             _request["model"] = model
         if preamble is not OMIT:
             _request["preamble"] = preamble
@@ -1919,15 +2169,15 @@
                         if len(_text) == 0:
                             continue
                         yield typing.cast(StreamedChatResponse, construct_type(type_=StreamedChatResponse, object_=json.loads(_text)))  # type: ignore
                 return
             await _response.aread()
             if _response.status_code == 429:
                 raise TooManyRequestsError(
-                    typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                    typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
                 )
             try:
                 _response_json = _response.json()
             except JSONDecodeError:
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
 
@@ -1961,50 +2211,58 @@
     ) -> NonStreamedChatResponse:
         """
         Generates a text response to a user message.
         To learn how to use Chat with Streaming and RAG follow [this guide](https://docs.cohere.com/docs/cochat-beta#various-ways-of-using-the-chat-endpoint).
 
         Parameters:
             - message: str. Text input for the model to respond to.
+                            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - model: typing.Optional[str]. Defaults to `command-r-plus`.
 
                                            The name of a compatible [Cohere model](https://docs.cohere.com/docs/models) or the ID of a [fine-tuned](https://docs.cohere.com/docs/chat-fine-tuning) model.
+                                           Compatible Deployments: Cohere Platform, Private Deployments
 
             - preamble: typing.Optional[str]. When specified, the default Cohere preamble will be replaced with the provided one. Preambles are a part of the prompt used to adjust the model's overall behavior and conversation style, and use the `SYSTEM` role.
 
                                               The `SYSTEM` role is also used for the contents of the optional `chat_history=` parameter. When used with the `chat_history=` parameter it adds content throughout a conversation. Conversely, when used with the `preamble=` parameter it adds content at the start of the conversation only.
+                                              Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - chat_history: typing.Optional[typing.Sequence[ChatMessage]]. A list of previous messages between the user and the model, giving the model conversational context for responding to the user's `message`.
 
                                                                            Each item represents a single message in the chat history, excluding the current user turn. It has two properties: `role` and `message`. The `role` identifies the sender (`CHATBOT`, `SYSTEM`, or `USER`), while the `message` contains the text content.
 
                                                                            The chat_history parameter should not be used for `SYSTEM` messages in most cases. Instead, to add a `SYSTEM` role message at the beginning of a conversation, the `preamble` parameter should be used.
+                                                                           Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - conversation_id: typing.Optional[str]. An alternative to `chat_history`.
 
                                                      Providing a `conversation_id` creates or resumes a persisted conversation with the specified ID. The ID can be any non empty string.
+                                                     Compatible Deployments: Cohere Platform
 
             - prompt_truncation: typing.Optional[ChatRequestPromptTruncation]. Defaults to `AUTO` when `connectors` are specified and `OFF` in all other cases.
 
                                                                                Dictates how the prompt will be constructed.
 
                                                                                With `prompt_truncation` set to "AUTO", some elements from `chat_history` and `documents` will be dropped in an attempt to construct a prompt that fits within the model's context length limit. During this process the order of the documents and chat history will be changed and ranked by relevance.
 
                                                                                With `prompt_truncation` set to "AUTO_PRESERVE_ORDER", some elements from `chat_history` and `documents` will be dropped in an attempt to construct a prompt that fits within the model's context length limit. During this process the order of the documents and chat history will be preserved as they are inputted into the API.
 
                                                                                With `prompt_truncation` set to "OFF", no elements will be dropped. If the sum of the inputs exceeds the model's context length limit, a `TooManyTokens` error will be returned.
+                                                                               Compatible Deployments: Cohere Platform Only AUTO_PRESERVE_ORDER: Azure, AWS Sagemaker, Private Deployments
 
             - connectors: typing.Optional[typing.Sequence[ChatConnector]]. Accepts `{"id": "web-search"}`, and/or the `"id"` for a custom [connector](https://docs.cohere.com/docs/connectors), if you've [created](https://docs.cohere.com/docs/creating-and-deploying-a-connector) one.
 
                                                                            When specified, the model's reply will be enriched with information found by quering each of the connectors (RAG).
+                                                                           Compatible Deployments: Cohere Platform
 
             - search_queries_only: typing.Optional[bool]. Defaults to `false`.
 
                                                           When `true`, the response will only contain a list of generated search queries, but no search will take place, and no reply from the model to the user's `message` will be generated.
+                                                          Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - documents: typing.Optional[typing.Sequence[ChatDocument]]. A list of relevant documents that the model can cite to generate a more accurate reply. Each document is a string-string dictionary.
 
                                                                          Example:
                                                                          `[
                                                                            { "title": "Tall penguins", "text": "Emperor penguins are the tallest." },
                                                                            { "title": "Penguin habitats", "text": "Emperor penguins only live in Antarctica." },
@@ -2015,56 +2273,73 @@
                                                                          Some suggested keys are "text", "author", and "date". For better generation quality, it is recommended to keep the total word count of the strings in the dictionary to under 300 words.
 
                                                                          An `id` field (string) can be optionally supplied to identify the document in the citations. This field will not be passed to the model.
 
                                                                          An `_excludes` field (array of strings) can be optionally supplied to omit some key-value pairs from being shown to the model. The omitted fields will still show up in the citation object. The "_excludes" field will not be passed to the model.
 
                                                                          See ['Document Mode'](https://docs.cohere.com/docs/retrieval-augmented-generation-rag#document-mode) in the guide for more information.
+                                                                         Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - citation_quality: typing.Optional[ChatRequestCitationQuality]. Defaults to `"accurate"`.
 
                                                                              Dictates the approach taken to generating citations as part of the RAG flow by allowing the user to specify whether they want `"accurate"` results or `"fast"` results.
+                                                                             Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - temperature: typing.Optional[float]. Defaults to `0.3`.
 
                                                    A non-negative float that tunes the degree of randomness in generation. Lower temperatures mean less random generations, and higher temperatures mean more random generations.
 
                                                    Randomness can be further maximized by increasing the  value of the `p` parameter.
+                                                   Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - max_tokens: typing.Optional[int]. The maximum number of tokens the model will generate as part of the response. Note: Setting a low value may result in incomplete generations.
+                                                Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - max_input_tokens: typing.Optional[int]. The maximum number of input tokens to send to the model. If not specified, `max_input_tokens` is the model's context length limit minus a small buffer.
 
                                                       Input will be truncated according to the `prompt_truncation` parameter.
+                                                      Compatible Deployments: Cohere Platform
 
             - k: typing.Optional[int]. Ensures only the top `k` most likely tokens are considered for generation at each step.
                                        Defaults to `0`, min value of `0`, max value of `500`.
+                                       Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - p: typing.Optional[float]. Ensures that only the most likely tokens, with total probability mass of `p`, are considered for generation at each step. If both `k` and `p` are enabled, `p` acts after `k`.
                                          Defaults to `0.75`. min value of `0.01`, max value of `0.99`.
+                                         Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - seed: typing.Optional[float]. If specified, the backend will make a best effort to sample tokens deterministically, such that repeated requests with the same seed and parameters should return the same result. However, determinism cannot be totally guaranteed.
+            - seed: typing.Optional[float]. If specified, the backend will make a best effort to sample tokens
+                                            deterministically, such that repeated requests with the same
+                                            seed and parameters should return the same result. However,
+                                            determinism cannot be totally guaranteed.
+                                            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - stop_sequences: typing.Optional[typing.Sequence[str]]. A list of up to 5 strings that the model will use to stop generation. If the model generates a string that matches any of the strings in the list, it will stop generating tokens and return the generated text up to that point not including the stop sequence.
+                                                                     Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - frequency_penalty: typing.Optional[float]. Defaults to `0.0`, min value of `0.0`, max value of `1.0`.
 
                                                          Used to reduce repetitiveness of generated tokens. The higher the value, the stronger a penalty is applied to previously present tokens, proportional to how many times they have already appeared in the prompt or prior generation.
+                                                         Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - presence_penalty: typing.Optional[float]. Defaults to `0.0`, min value of `0.0`, max value of `1.0`.
 
                                                         Used to reduce repetitiveness of generated tokens. Similar to `frequency_penalty`, except that this penalty is applied equally to all tokens that have already appeared, regardless of their exact frequencies.
+                                                        Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - raw_prompting: typing.Optional[bool]. When enabled, the user's prompt will be sent to the model without any pre-processing.
+            - raw_prompting: typing.Optional[bool]. When enabled, the user's prompt will be sent to the model without
+                                                    any pre-processing.
+                                                    Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - return_prompt: typing.Optional[bool]. The prompt is returned in the `prompt` response field when this is enabled.
 
             - tools: typing.Optional[typing.Sequence[Tool]]. A list of available tools (functions) that the model may suggest invoking before producing a text response.
 
                                                              When `tools` is passed (without `tool_results`), the `text` field in the response will be `""` and the `tool_calls` field in the response will be populated with a list of tool calls that need to be made. If no calls need to be made, the `tool_calls` array will be empty.
+                                                             Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - tool_results: typing.Optional[typing.Sequence[ChatRequestToolResultsItem]]. A list of results from invoking tools recommended by the model in the previous chat turn. Results are used to produce a text response and will be referenced in citations. When using `tool_results`, `tools` must be passed as well.
                                                                                           Each tool_result contains information about how it was invoked, as well as a list of outputs in the form of dictionaries.
 
                                                                                           **Note**: `outputs` must be a list of objects. If your tool returns a single object (eg `{"status": 200}`), make sure to wrap it in a list.
                                                                                           ```
                                                                                           tool_results = [
@@ -2079,14 +2354,15 @@
                                                                                                 <key>: <value>
                                                                                               }]
                                                                                             },
                                                                                             ...
                                                                                           ]
                                                                                           ```
                                                                                           **Note**: Chat calls with `tool_results` should not be included in the Chat history to avoid duplication of the message text.
+                                                                                          Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from cohere import ChatMessage
         from cohere.client import AsyncClient
 
         client = AsyncClient(
@@ -2180,15 +2456,15 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return typing.cast(NonStreamedChatResponse, construct_type(type_=NonStreamedChatResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
@@ -2279,16 +2555,30 @@
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         await client.generate_stream(
-            prompt="Please explain to me how LLMs work",
-            preset="my-preset-a58sbd",
+            prompt="string",
+            model="string",
+            num_generations=1,
+            max_tokens=1,
+            truncate="NONE",
+            temperature=1.1,
+            seed=1.1,
+            preset="string",
+            end_sequences=["string"],
+            stop_sequences=["string"],
+            k=1,
+            p=1.1,
+            frequency_penalty=1.1,
+            presence_penalty=1.1,
+            return_likelihoods="GENERATION",
+            raw_prompting=True,
         )
         """
         _request: typing.Dict[str, typing.Any] = {"prompt": prompt, "stream": True}
         if model is not OMIT:
             _request["model"] = model
         if num_generations is not OMIT:
             _request["num_generations"] = num_generations
@@ -2359,15 +2649,15 @@
             await _response.aread()
             if _response.status_code == 400:
                 raise BadRequestError(
                     typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
                 )
             if _response.status_code == 429:
                 raise TooManyRequestsError(
-                    typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                    typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
                 )
             if _response.status_code == 500:
                 raise InternalServerError(
                     typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
                 )
             try:
                 _response_json = _response.json()
@@ -2463,15 +2753,14 @@
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         await client.generate(
             prompt="Please explain to me how LLMs work",
-            preset="my-preset-a58sbd",
         )
         """
         _request: typing.Dict[str, typing.Any] = {"prompt": prompt, "stream": False}
         if model is not OMIT:
             _request["model"] = model
         if num_generations is not OMIT:
             _request["num_generations"] = num_generations
@@ -2531,15 +2820,15 @@
             return typing.cast(Generation, construct_type(type_=Generation, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 500:
             raise InternalServerError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
@@ -2650,15 +2939,15 @@
             return typing.cast(EmbedResponse, construct_type(type_=EmbedResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 500:
             raise InternalServerError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
@@ -2705,15 +2994,15 @@
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         await client.rerank(
-            model="rerank-english-v2.0",
+            model="rerank-english-v3.0",
             query="What is the capital of the United States?",
             documents=[
                 "Carson City is the capital city of the American state of Nevada.",
                 "The Commonwealth of the Northern Mariana Islands is a group of islands in the Pacific Ocean. Its capital is Saipan.",
                 "Washington, D.C. (also known as simply Washington or D.C., and officially as the District of Columbia) is the capital of the United States. It is a federal district.",
                 "Capital punishment (the death penalty) has existed in the United States since beforethe United States was a country. As of 2017, capital punishment is legal in 30 of the 50 states.",
             ],
@@ -2756,15 +3045,15 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return typing.cast(RerankResponse, construct_type(type_=RerankResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
@@ -2844,15 +3133,14 @@
                     label="Not spam",
                 ),
                 ClassifyExample(
                     text="Pre-read for tomorrow",
                     label="Not spam",
                 ),
             ],
-            preset="my-preset-a58sbd",
         )
         """
         _request: typing.Dict[str, typing.Any] = {"inputs": inputs}
         if examples is not OMIT:
             _request["examples"] = examples
         if model is not OMIT:
             _request["model"] = model
@@ -2890,15 +3178,15 @@
             return typing.cast(ClassifyResponse, construct_type(type_=ClassifyResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 500:
             raise InternalServerError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
@@ -2991,15 +3279,15 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return typing.cast(SummarizeResponse, construct_type(type_=SummarizeResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
@@ -3057,15 +3345,15 @@
             return typing.cast(TokenizeResponse, construct_type(type_=TokenizeResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 500:
             raise InternalServerError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
@@ -3123,15 +3411,65 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return typing.cast(DetokenizeResponse, construct_type(type_=DetokenizeResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
+            )
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def check_api_key(self, *, request_options: typing.Optional[RequestOptions] = None) -> CheckApiKeyResponse:
+        """
+        Checks that the api key in the Authorization header is valid and active
+
+        Parameters:
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from cohere.client import AsyncClient
+
+        client = AsyncClient(
+            client_name="YOUR_CLIENT_NAME",
+            token="YOUR_TOKEN",
+        )
+        await client.check_api_key()
+        """
+        _response = await self._client_wrapper.httpx_client.request(
+            "POST",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "check-api-key"),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
+            if request_options is not None
+            else None,
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
+        )
+        if 200 <= _response.status_code < 300:
+            return typing.cast(CheckApiKeyResponse, construct_type(type_=CheckApiKeyResponse, object_=_response.json()))  # type: ignore
+        if _response.status_code == 429:
+            raise TooManyRequestsError(
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `cohere-5.3.4/src/cohere/client.py` & `cohere-5.3.5/src/cohere/client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/connectors/client.py` & `cohere-5.3.5/src/cohere/connectors/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from ..types.create_connector_o_auth import CreateConnectorOAuth
 from ..types.create_connector_response import CreateConnectorResponse
 from ..types.create_connector_service_auth import CreateConnectorServiceAuth
 from ..types.delete_connector_response import DeleteConnectorResponse
 from ..types.get_connector_response import GetConnectorResponse
 from ..types.list_connectors_response import ListConnectorsResponse
 from ..types.o_auth_authorize_response import OAuthAuthorizeResponse
+from ..types.too_many_requests_error_body import TooManyRequestsErrorBody
 from ..types.update_connector_response import UpdateConnectorResponse
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class ConnectorsClient:
@@ -91,15 +92,15 @@
             return typing.cast(ListConnectorsResponse, construct_type(type_=ListConnectorsResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 500:
             raise InternalServerError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
@@ -200,15 +201,15 @@
             )
         if _response.status_code == 403:
             raise ForbiddenError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 500:
             raise InternalServerError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
@@ -263,15 +264,15 @@
             )
         if _response.status_code == 404:
             raise NotFoundError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 500:
             raise InternalServerError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
@@ -330,15 +331,15 @@
             )
         if _response.status_code == 404:
             raise NotFoundError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 500:
             raise InternalServerError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
@@ -444,15 +445,15 @@
             )
         if _response.status_code == 404:
             raise NotFoundError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 500:
             raise InternalServerError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
@@ -529,15 +530,15 @@
             )
         if _response.status_code == 404:
             raise NotFoundError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 500:
             raise InternalServerError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
@@ -609,15 +610,15 @@
             return typing.cast(ListConnectorsResponse, construct_type(type_=ListConnectorsResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 500:
             raise InternalServerError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
@@ -718,15 +719,15 @@
             )
         if _response.status_code == 403:
             raise ForbiddenError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 500:
             raise InternalServerError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
@@ -781,15 +782,15 @@
             )
         if _response.status_code == 404:
             raise NotFoundError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 500:
             raise InternalServerError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
@@ -850,15 +851,15 @@
             )
         if _response.status_code == 404:
             raise NotFoundError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 500:
             raise InternalServerError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
@@ -964,15 +965,15 @@
             )
         if _response.status_code == 404:
             raise NotFoundError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 500:
             raise InternalServerError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
@@ -1049,15 +1050,15 @@
             )
         if _response.status_code == 404:
             raise NotFoundError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 500:
             raise InternalServerError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
```

### Comparing `cohere-5.3.4/src/cohere/core/__init__.py` & `cohere-5.3.5/src/cohere/core/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/core/client_wrapper.py` & `cohere-5.3.5/src/cohere/core/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/core/datetime_utils.py` & `cohere-5.3.5/src/cohere/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/core/file.py` & `cohere-5.3.5/src/cohere/core/file.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/core/http_client.py` & `cohere-5.3.5/src/cohere/core/http_client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/core/jsonable_encoder.py` & `cohere-5.3.5/src/cohere/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/core/request_options.py` & `cohere-5.3.5/src/cohere/core/request_options.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/core/unchecked_base_model.py` & `cohere-5.3.5/src/cohere/core/unchecked_base_model.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/datasets/client.py` & `cohere-5.3.5/src/cohere/datasets/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from ..core.jsonable_encoder import jsonable_encoder
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
 from ..core.unchecked_base_model import construct_type
 from ..errors.too_many_requests_error import TooManyRequestsError
 from ..types.dataset_type import DatasetType
 from ..types.dataset_validation_status import DatasetValidationStatus
+from ..types.too_many_requests_error_body import TooManyRequestsErrorBody
 from .types.datasets_create_response import DatasetsCreateResponse
 from .types.datasets_get_response import DatasetsGetResponse
 from .types.datasets_get_usage_response import DatasetsGetUsageResponse
 from .types.datasets_list_response import DatasetsListResponse
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
@@ -100,15 +101,15 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return typing.cast(DatasetsListResponse, construct_type(type_=DatasetsListResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
@@ -130,15 +131,15 @@
     ) -> DatasetsCreateResponse:
         """
         Create a dataset by uploading a file. See ['Dataset Creation'](https://docs.cohere.com/docs/datasets#dataset-creation) for more information.
 
         Parameters:
             - name: str. The name of the uploaded dataset.
 
-            - type: DatasetType. The dataset type, which is used to validate the data. Valid types are `embed-input`, `reranker-finetune-input`, `prompt-completion-finetune-input`, `single-label-classification-finetune-input`, `chat-finetune-input`, and `multi-label-classification-finetune-input`.
+            - type: DatasetType. The dataset type, which is used to validate the data. Valid types are `embed-input`, `reranker-finetune-input`, `single-label-classification-finetune-input`, `chat-finetune-input`, and `multi-label-classification-finetune-input`.
 
             - keep_original_file: typing.Optional[bool]. Indicates if the original file should be stored.
 
             - skip_malformed_input: typing.Optional[bool]. Indicates whether rows with malformed input should be dropped (instead of failing the validation check). Dropped rows will be returned in the warnings field.
 
             - keep_fields: typing.Optional[typing.Union[str, typing.Sequence[str]]]. List of names of fields that will be persisted in the Dataset. By default the Dataset will retain only the required fields indicated in the [schema for the corresponding Dataset type](https://docs.cohere.com/docs/datasets#dataset-types). For example, datasets of type `embed-input` will drop all fields other than the required `text` field. If any of the fields in `keep_fields` are missing from the uploaded file, Dataset validation will fail.
 
@@ -211,15 +212,15 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return typing.cast(DatasetsCreateResponse, construct_type(type_=DatasetsCreateResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
@@ -258,15 +259,15 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return typing.cast(DatasetsGetUsageResponse, construct_type(type_=DatasetsGetUsageResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
@@ -309,15 +310,15 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return typing.cast(DatasetsGetResponse, construct_type(type_=DatasetsGetResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
@@ -362,15 +363,15 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return typing.cast(typing.Dict[str, typing.Any], construct_type(type_=typing.Dict[str, typing.Any], object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
@@ -450,15 +451,15 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return typing.cast(DatasetsListResponse, construct_type(type_=DatasetsListResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
@@ -480,15 +481,15 @@
     ) -> DatasetsCreateResponse:
         """
         Create a dataset by uploading a file. See ['Dataset Creation'](https://docs.cohere.com/docs/datasets#dataset-creation) for more information.
 
         Parameters:
             - name: str. The name of the uploaded dataset.
 
-            - type: DatasetType. The dataset type, which is used to validate the data. Valid types are `embed-input`, `reranker-finetune-input`, `prompt-completion-finetune-input`, `single-label-classification-finetune-input`, `chat-finetune-input`, and `multi-label-classification-finetune-input`.
+            - type: DatasetType. The dataset type, which is used to validate the data. Valid types are `embed-input`, `reranker-finetune-input`, `single-label-classification-finetune-input`, `chat-finetune-input`, and `multi-label-classification-finetune-input`.
 
             - keep_original_file: typing.Optional[bool]. Indicates if the original file should be stored.
 
             - skip_malformed_input: typing.Optional[bool]. Indicates whether rows with malformed input should be dropped (instead of failing the validation check). Dropped rows will be returned in the warnings field.
 
             - keep_fields: typing.Optional[typing.Union[str, typing.Sequence[str]]]. List of names of fields that will be persisted in the Dataset. By default the Dataset will retain only the required fields indicated in the [schema for the corresponding Dataset type](https://docs.cohere.com/docs/datasets#dataset-types). For example, datasets of type `embed-input` will drop all fields other than the required `text` field. If any of the fields in `keep_fields` are missing from the uploaded file, Dataset validation will fail.
 
@@ -561,15 +562,15 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return typing.cast(DatasetsCreateResponse, construct_type(type_=DatasetsCreateResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
@@ -608,15 +609,15 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return typing.cast(DatasetsGetUsageResponse, construct_type(type_=DatasetsGetUsageResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
@@ -659,15 +660,15 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return typing.cast(DatasetsGetResponse, construct_type(type_=DatasetsGetResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
@@ -712,14 +713,14 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return typing.cast(typing.Dict[str, typing.Any], construct_type(type_=typing.Dict[str, typing.Any], object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `cohere-5.3.4/src/cohere/datasets/types/__init__.py` & `cohere-5.3.5/src/cohere/datasets/types/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .datasets_create_response import DatasetsCreateResponse
-from .datasets_create_response_dataset_parts import DatasetsCreateResponseDatasetParts
+from .datasets_create_response_dataset_parts_item import DatasetsCreateResponseDatasetPartsItem
 from .datasets_get_response import DatasetsGetResponse
 from .datasets_get_usage_response import DatasetsGetUsageResponse
 from .datasets_list_response import DatasetsListResponse
 
 __all__ = [
     "DatasetsCreateResponse",
-    "DatasetsCreateResponseDatasetParts",
+    "DatasetsCreateResponseDatasetPartsItem",
     "DatasetsGetResponse",
     "DatasetsGetUsageResponse",
     "DatasetsListResponse",
 ]
```

### Comparing `cohere-5.3.4/src/cohere/datasets/types/datasets_create_response.py` & `cohere-5.3.5/src/cohere/datasets/types/datasets_create_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/datasets/types/datasets_create_response_dataset_parts.py` & `cohere-5.3.5/src/cohere/types/metrics_embed_data_fields_item.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from ...core.unchecked_base_model import UncheckedBaseModel
+from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class DatasetsCreateResponseDatasetParts(UncheckedBaseModel):
-    """
-    the underlying files that make up the dataset
-    """
-
+class MetricsEmbedDataFieldsItem(UncheckedBaseModel):
     name: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    the name of the dataset part
-    """
-
-    num_rows: typing.Optional[float] = pydantic_v1.Field(default=None)
-    """
-    the number of rows in the dataset part
+    the name of the field
     """
 
-    samples: typing.Optional[typing.List[str]] = None
-    part_kind: typing.Optional[str] = pydantic_v1.Field(default=None)
+    count: typing.Optional[float] = pydantic_v1.Field(default=None)
     """
-    the kind of dataset part
+    the number of times the field appears in the dataset
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `cohere-5.3.4/src/cohere/datasets/types/datasets_get_response.py` & `cohere-5.3.5/src/cohere/datasets/types/datasets_get_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/datasets/types/datasets_get_usage_response.py` & `cohere-5.3.5/src/cohere/datasets/types/datasets_get_usage_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/datasets/types/datasets_list_response.py` & `cohere-5.3.5/src/cohere/datasets/types/datasets_list_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/embed_jobs/client.py` & `cohere-5.3.5/src/cohere/embed_jobs/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from ..errors.not_found_error import NotFoundError
 from ..errors.too_many_requests_error import TooManyRequestsError
 from ..types.create_embed_job_response import CreateEmbedJobResponse
 from ..types.embed_input_type import EmbedInputType
 from ..types.embed_job import EmbedJob
 from ..types.embedding_type import EmbeddingType
 from ..types.list_embed_job_response import ListEmbedJobResponse
+from ..types.too_many_requests_error_body import TooManyRequestsErrorBody
 from .types.create_embed_job_request_truncate import CreateEmbedJobRequestTruncate
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class EmbedJobsClient:
@@ -68,15 +69,15 @@
             return typing.cast(ListEmbedJobResponse, construct_type(type_=ListEmbedJobResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 500:
             raise InternalServerError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
@@ -176,15 +177,15 @@
             return typing.cast(CreateEmbedJobResponse, construct_type(type_=CreateEmbedJobResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 500:
             raise InternalServerError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
@@ -239,15 +240,15 @@
             )
         if _response.status_code == 404:
             raise NotFoundError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 500:
             raise InternalServerError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
@@ -307,15 +308,15 @@
             )
         if _response.status_code == 404:
             raise NotFoundError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 500:
             raise InternalServerError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
@@ -367,15 +368,15 @@
             return typing.cast(ListEmbedJobResponse, construct_type(type_=ListEmbedJobResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 500:
             raise InternalServerError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
@@ -475,15 +476,15 @@
             return typing.cast(CreateEmbedJobResponse, construct_type(type_=CreateEmbedJobResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 500:
             raise InternalServerError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
@@ -538,15 +539,15 @@
             )
         if _response.status_code == 404:
             raise NotFoundError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 500:
             raise InternalServerError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
@@ -606,15 +607,15 @@
             )
         if _response.status_code == 404:
             raise NotFoundError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 500:
             raise InternalServerError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
```

### Comparing `cohere-5.3.4/src/cohere/errors/__init__.py` & `cohere-5.3.5/src/cohere/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/finetuning/__init__.py` & `cohere-5.3.5/src/cohere/finetuning/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/finetuning/client.py` & `cohere-5.3.5/src/cohere/finetuning/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
             token="YOUR_TOKEN",
         )
         client.finetuning.create_finetuned_model(
             request=FinetunedModel(
                 name="api-test",
                 settings=Settings(
                     base_model=BaseModel(
-                        base_type="BASE_TYPE_GENERATIVE",
+                        base_type="BASE_TYPE_CHAT",
                     ),
                     dataset_id="my-dataset-id",
                 ),
             ),
         )
         """
         _response = self._client_wrapper.httpx_client.request(
@@ -806,15 +806,15 @@
             token="YOUR_TOKEN",
         )
         await client.finetuning.create_finetuned_model(
             request=FinetunedModel(
                 name="api-test",
                 settings=Settings(
                     base_model=BaseModel(
-                        base_type="BASE_TYPE_GENERATIVE",
+                        base_type="BASE_TYPE_CHAT",
                     ),
                     dataset_id="my-dataset-id",
                 ),
             ),
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
```

### Comparing `cohere-5.3.4/src/cohere/finetuning/finetuning/__init__.py` & `cohere-5.3.5/src/cohere/finetuning/finetuning/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/finetuning/finetuning/types/__init__.py` & `cohere-5.3.5/src/cohere/finetuning/finetuning/types/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/finetuning/finetuning/types/base_model.py` & `cohere-5.3.5/src/cohere/finetuning/finetuning/types/base_model.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/finetuning/finetuning/types/create_finetuned_model_response.py` & `cohere-5.3.5/src/cohere/finetuning/finetuning/types/create_finetuned_model_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/finetuning/finetuning/types/error.py` & `cohere-5.3.5/src/cohere/finetuning/finetuning/types/error.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/finetuning/finetuning/types/event.py` & `cohere-5.3.5/src/cohere/finetuning/finetuning/types/event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/finetuning/finetuning/types/finetuned_model.py` & `cohere-5.3.5/src/cohere/finetuning/finetuning/types/finetuned_model.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/finetuning/finetuning/types/get_finetuned_model_response.py` & `cohere-5.3.5/src/cohere/finetuning/finetuning/types/get_finetuned_model_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/finetuning/finetuning/types/hyperparameters.py` & `cohere-5.3.5/src/cohere/finetuning/finetuning/types/hyperparameters.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/finetuning/finetuning/types/list_events_response.py` & `cohere-5.3.5/src/cohere/finetuning/finetuning/types/list_events_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/finetuning/finetuning/types/list_finetuned_models_response.py` & `cohere-5.3.5/src/cohere/finetuning/finetuning/types/list_finetuned_models_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/finetuning/finetuning/types/list_training_step_metrics_response.py` & `cohere-5.3.5/src/cohere/finetuning/finetuning/types/list_training_step_metrics_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/finetuning/finetuning/types/settings.py` & `cohere-5.3.5/src/cohere/finetuning/finetuning/types/settings.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/finetuning/finetuning/types/training_step_metrics.py` & `cohere-5.3.5/src/cohere/finetuning/finetuning/types/training_step_metrics.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/finetuning/finetuning/types/update_finetuned_model_response.py` & `cohere-5.3.5/src/cohere/finetuning/finetuning/types/update_finetuned_model_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/manually_maintained/cache.py` & `cohere-5.3.5/src/cohere/manually_maintained/cache.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/manually_maintained/tokenizers.py` & `cohere-5.3.5/src/cohere/manually_maintained/tokenizers.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/models/client.py` & `cohere-5.3.5/src/cohere/models/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from ..core.unchecked_base_model import construct_type
 from ..errors.bad_request_error import BadRequestError
 from ..errors.internal_server_error import InternalServerError
 from ..errors.too_many_requests_error import TooManyRequestsError
 from ..types.compatible_endpoint import CompatibleEndpoint
 from ..types.get_model_response import GetModelResponse
 from ..types.list_models_response import ListModelsResponse
+from ..types.too_many_requests_error_body import TooManyRequestsErrorBody
 
 
 class ModelsClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def get(self, model: str, *, request_options: typing.Optional[RequestOptions] = None) -> GetModelResponse:
@@ -65,15 +66,15 @@
             return typing.cast(GetModelResponse, construct_type(type_=GetModelResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 500:
             raise InternalServerError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
@@ -144,15 +145,15 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return typing.cast(ListModelsResponse, construct_type(type_=ListModelsResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
@@ -204,15 +205,15 @@
             return typing.cast(GetModelResponse, construct_type(type_=GetModelResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 500:
             raise InternalServerError(
                 typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
@@ -283,14 +284,14 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return typing.cast(ListModelsResponse, construct_type(type_=ListModelsResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
             raise TooManyRequestsError(
-                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                typing.cast(TooManyRequestsErrorBody, construct_type(type_=TooManyRequestsErrorBody, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `cohere-5.3.4/src/cohere/overrides.py` & `cohere-5.3.5/src/cohere/overrides.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/__init__.py` & `cohere-5.3.5/src/cohere/types/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from .chat_stream_request_citation_quality import ChatStreamRequestCitationQuality
 from .chat_stream_request_connectors_search_options import ChatStreamRequestConnectorsSearchOptions
 from .chat_stream_request_prompt_truncation import ChatStreamRequestPromptTruncation
 from .chat_stream_request_tool_results_item import ChatStreamRequestToolResultsItem
 from .chat_stream_start_event import ChatStreamStartEvent
 from .chat_text_generation_event import ChatTextGenerationEvent
 from .chat_tool_calls_generation_event import ChatToolCallsGenerationEvent
+from .check_api_key_response import CheckApiKeyResponse
 from .classify_data_metrics import ClassifyDataMetrics
 from .classify_example import ClassifyExample
 from .classify_request_truncate import ClassifyRequestTruncate
 from .classify_response import ClassifyResponse
 from .classify_response_classifications_item import ClassifyResponseClassificationsItem
 from .classify_response_classifications_item_classification_type import (
     ClassifyResponseClassificationsItemClassificationType,
@@ -85,14 +86,16 @@
 from .get_connector_response import GetConnectorResponse
 from .get_model_response import GetModelResponse
 from .label_metric import LabelMetric
 from .list_connectors_response import ListConnectorsResponse
 from .list_embed_job_response import ListEmbedJobResponse
 from .list_models_response import ListModelsResponse
 from .metrics import Metrics
+from .metrics_embed_data import MetricsEmbedData
+from .metrics_embed_data_fields_item import MetricsEmbedDataFieldsItem
 from .non_streamed_chat_response import NonStreamedChatResponse
 from .o_auth_authorize_response import OAuthAuthorizeResponse
 from .parse_info import ParseInfo
 from .rerank_request_documents_item import RerankRequestDocumentsItem
 from .rerank_request_documents_item_text import RerankRequestDocumentsItemText
 from .rerank_response import RerankResponse
 from .rerank_response_results_item import RerankResponseResultsItem
@@ -112,14 +115,15 @@
     StreamedChatResponse_ToolCallsGeneration,
 )
 from .summarize_request_extractiveness import SummarizeRequestExtractiveness
 from .summarize_request_format import SummarizeRequestFormat
 from .summarize_request_length import SummarizeRequestLength
 from .summarize_response import SummarizeResponse
 from .tokenize_response import TokenizeResponse
+from .too_many_requests_error_body import TooManyRequestsErrorBody
 from .tool import Tool
 from .tool_call import ToolCall
 from .tool_parameter_definitions_value import ToolParameterDefinitionsValue
 from .update_connector_response import UpdateConnectorResponse
 
 __all__ = [
     "ApiMeta",
@@ -149,14 +153,15 @@
     "ChatStreamRequestCitationQuality",
     "ChatStreamRequestConnectorsSearchOptions",
     "ChatStreamRequestPromptTruncation",
     "ChatStreamRequestToolResultsItem",
     "ChatStreamStartEvent",
     "ChatTextGenerationEvent",
     "ChatToolCallsGenerationEvent",
+    "CheckApiKeyResponse",
     "ClassifyDataMetrics",
     "ClassifyExample",
     "ClassifyRequestTruncate",
     "ClassifyResponse",
     "ClassifyResponseClassificationsItem",
     "ClassifyResponseClassificationsItemClassificationType",
     "ClassifyResponseClassificationsItemLabelsValue",
@@ -205,14 +210,16 @@
     "GetConnectorResponse",
     "GetModelResponse",
     "LabelMetric",
     "ListConnectorsResponse",
     "ListEmbedJobResponse",
     "ListModelsResponse",
     "Metrics",
+    "MetricsEmbedData",
+    "MetricsEmbedDataFieldsItem",
     "NonStreamedChatResponse",
     "OAuthAuthorizeResponse",
     "ParseInfo",
     "RerankRequestDocumentsItem",
     "RerankRequestDocumentsItemText",
     "RerankResponse",
     "RerankResponseResultsItem",
@@ -230,12 +237,13 @@
     "StreamedChatResponse_TextGeneration",
     "StreamedChatResponse_ToolCallsGeneration",
     "SummarizeRequestExtractiveness",
     "SummarizeRequestFormat",
     "SummarizeRequestLength",
     "SummarizeResponse",
     "TokenizeResponse",
+    "TooManyRequestsErrorBody",
     "Tool",
     "ToolCall",
     "ToolParameterDefinitionsValue",
     "UpdateConnectorResponse",
 ]
```

### Comparing `cohere-5.3.4/src/cohere/types/api_meta.py` & `cohere-5.3.5/src/cohere/types/api_meta.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/api_meta_api_version.py` & `cohere-5.3.5/src/cohere/types/api_meta_api_version.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/api_meta_billed_units.py` & `cohere-5.3.5/src/cohere/types/api_meta_billed_units.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/api_meta_tokens.py` & `cohere-5.3.5/src/cohere/types/api_meta_tokens.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/chat_citation.py` & `cohere-5.3.5/src/cohere/types/chat_citation.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/chat_citation_generation_event.py` & `cohere-5.3.5/src/cohere/types/chat_citation_generation_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/chat_connector.py` & `cohere-5.3.5/src/cohere/types/chat_connector.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/chat_data_metrics.py` & `cohere-5.3.5/src/cohere/types/chat_data_metrics.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/chat_message.py` & `cohere-5.3.5/src/cohere/types/chat_message.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/chat_request_connectors_search_options.py` & `cohere-5.3.5/src/cohere/types/chat_request_connectors_search_options.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/chat_request_tool_results_item.py` & `cohere-5.3.5/src/cohere/types/chat_request_tool_results_item.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/chat_search_queries_generation_event.py` & `cohere-5.3.5/src/cohere/types/chat_search_queries_generation_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/chat_search_query.py` & `cohere-5.3.5/src/cohere/types/chat_search_query.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/chat_search_result.py` & `cohere-5.3.5/src/cohere/types/chat_search_result.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/chat_search_result_connector.py` & `cohere-5.3.5/src/cohere/types/chat_search_result_connector.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/chat_search_results_event.py` & `cohere-5.3.5/src/cohere/types/chat_search_results_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/chat_stream_end_event.py` & `cohere-5.3.5/src/cohere/types/chat_stream_end_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/chat_stream_event.py` & `cohere-5.3.5/src/cohere/types/chat_stream_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/chat_stream_request_connectors_search_options.py` & `cohere-5.3.5/src/cohere/types/chat_stream_request_connectors_search_options.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/chat_stream_request_tool_results_item.py` & `cohere-5.3.5/src/cohere/types/chat_stream_request_tool_results_item.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/chat_stream_start_event.py` & `cohere-5.3.5/src/cohere/types/chat_stream_start_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/chat_text_generation_event.py` & `cohere-5.3.5/src/cohere/types/chat_text_generation_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/chat_tool_calls_generation_event.py` & `cohere-5.3.5/src/cohere/types/chat_tool_calls_generation_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/classify_data_metrics.py` & `cohere-5.3.5/src/cohere/types/classify_data_metrics.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/classify_example.py` & `cohere-5.3.5/src/cohere/types/classify_example.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/classify_response.py` & `cohere-5.3.5/src/cohere/types/classify_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/classify_response_classifications_item.py` & `cohere-5.3.5/src/cohere/types/classify_response_classifications_item.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/classify_response_classifications_item_labels_value.py` & `cohere-5.3.5/src/cohere/types/classify_response_classifications_item_labels_value.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/connector.py` & `cohere-5.3.5/src/cohere/types/connector.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/connector_o_auth.py` & `cohere-5.3.5/src/cohere/types/connector_o_auth.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/create_connector_o_auth.py` & `cohere-5.3.5/src/cohere/types/create_connector_o_auth.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/create_connector_response.py` & `cohere-5.3.5/src/cohere/types/create_connector_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/create_connector_service_auth.py` & `cohere-5.3.5/src/cohere/types/create_connector_service_auth.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/create_embed_job_response.py` & `cohere-5.3.5/src/cohere/types/create_embed_job_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/dataset.py` & `cohere-5.3.5/src/cohere/types/dataset.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/dataset_part.py` & `cohere-5.3.5/src/cohere/types/dataset_part.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,14 +40,19 @@
     """
 
     original_url: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     The download url of the original file
     """
 
+    samples: typing.Optional[typing.List[str]] = pydantic_v1.Field(default=None)
+    """
+    The first few rows of the parsed file
+    """
+
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `cohere-5.3.4/src/cohere/types/detokenize_response.py` & `cohere-5.3.5/src/cohere/types/detokenize_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/embed_by_type_response.py` & `cohere-5.3.5/src/cohere/types/embed_by_type_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/embed_by_type_response_embeddings.py` & `cohere-5.3.5/src/cohere/types/embed_by_type_response_embeddings.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/embed_floats_response.py` & `cohere-5.3.5/src/cohere/types/embed_floats_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/embed_job.py` & `cohere-5.3.5/src/cohere/types/embed_job.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/embed_response.py` & `cohere-5.3.5/src/cohere/types/embed_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/finetune_dataset_metrics.py` & `cohere-5.3.5/src/cohere/types/finetune_dataset_metrics.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/generate_stream_end.py` & `cohere-5.3.5/src/cohere/types/generate_stream_end.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/generate_stream_end_response.py` & `cohere-5.3.5/src/cohere/types/generate_stream_end_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/generate_stream_error.py` & `cohere-5.3.5/src/cohere/types/generate_stream_error.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/generate_stream_event.py` & `cohere-5.3.5/src/cohere/types/generate_stream_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/generate_stream_text.py` & `cohere-5.3.5/src/cohere/types/generate_stream_text.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/generate_streamed_response.py` & `cohere-5.3.5/src/cohere/types/generate_streamed_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/generation.py` & `cohere-5.3.5/src/cohere/types/generation.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/get_connector_response.py` & `cohere-5.3.5/src/cohere/types/get_connector_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/get_model_response.py` & `cohere-5.3.5/src/cohere/types/get_model_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/label_metric.py` & `cohere-5.3.5/src/cohere/types/label_metric.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/list_connectors_response.py` & `cohere-5.3.5/src/cohere/types/list_connectors_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/list_embed_job_response.py` & `cohere-5.3.5/src/cohere/types/list_embed_job_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/list_models_response.py` & `cohere-5.3.5/src/cohere/types/list_models_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/metrics.py` & `cohere-5.3.5/src/cohere/types/single_generation_token_likelihoods_item.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
-from .finetune_dataset_metrics import FinetuneDatasetMetrics
 
 
-class Metrics(UncheckedBaseModel):
-    finetune_dataset_metrics: typing.Optional[FinetuneDatasetMetrics] = None
+class SingleGenerationTokenLikelihoodsItem(UncheckedBaseModel):
+    token: str
+    likelihood: float
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `cohere-5.3.4/src/cohere/types/non_streamed_chat_response.py` & `cohere-5.3.5/src/cohere/types/non_streamed_chat_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/o_auth_authorize_response.py` & `cohere-5.3.5/src/cohere/types/o_auth_authorize_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/parse_info.py` & `cohere-5.3.5/src/cohere/types/parse_info.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/rerank_request_documents_item_text.py` & `cohere-5.3.5/src/cohere/types/rerank_request_documents_item_text.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/rerank_response.py` & `cohere-5.3.5/src/cohere/types/rerank_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/rerank_response_results_item.py` & `cohere-5.3.5/src/cohere/types/rerank_response_results_item.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/rerank_response_results_item_document.py` & `cohere-5.3.5/src/cohere/types/rerank_response_results_item_document.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/reranker_data_metrics.py` & `cohere-5.3.5/src/cohere/types/reranker_data_metrics.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/single_generation.py` & `cohere-5.3.5/src/cohere/types/single_generation.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/single_generation_in_stream.py` & `cohere-5.3.5/src/cohere/types/single_generation_in_stream.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/single_generation_token_likelihoods_item.py` & `cohere-5.3.5/src/cohere/types/too_many_requests_error_body.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class SingleGenerationTokenLikelihoodsItem(UncheckedBaseModel):
-    token: str
-    likelihood: float
+class TooManyRequestsErrorBody(UncheckedBaseModel):
+    data: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `cohere-5.3.4/src/cohere/types/streamed_chat_response.py` & `cohere-5.3.5/src/cohere/types/streamed_chat_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/summarize_response.py` & `cohere-5.3.5/src/cohere/types/summarize_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/tokenize_response.py` & `cohere-5.3.5/src/cohere/types/tokenize_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/tool.py` & `cohere-5.3.5/src/cohere/types/tool.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/tool_call.py` & `cohere-5.3.5/src/cohere/types/tool_call.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/tool_parameter_definitions_value.py` & `cohere-5.3.5/src/cohere/types/tool_parameter_definitions_value.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/types/update_connector_response.py` & `cohere-5.3.5/src/cohere/types/update_connector_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/src/cohere/utils.py` & `cohere-5.3.5/src/cohere/utils.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.4/PKG-INFO` & `cohere-5.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cohere
-Version: 5.3.4
+Version: 5.3.5
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

