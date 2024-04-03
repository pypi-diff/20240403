# Comparing `tmp/cohere-5.2.0.tar.gz` & `tmp/cohere-5.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cohere-5.2.0.tar", max compression
+gzip compressed data, was "cohere-5.2.1.tar", max compression
```

## Comparing `cohere-5.2.0.tar` & `cohere-5.2.1.tar`

### file list

```diff
@@ -1,172 +1,172 @@
--rw-r--r--   0        0        0     1062 2024-04-03 16:39:06.464279 cohere-5.2.0/LICENSE
--rw-r--r--   0        0        0     2359 2024-04-03 16:39:06.464279 cohere-5.2.0/README.md
--rw-r--r--   0        0        0      691 2024-04-03 16:39:06.472278 cohere-5.2.0/pyproject.toml
--rw-r--r--   0        0        0     7869 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/__init__.py
--rw-r--r--   0        0        0   197822 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/base_client.py
--rw-r--r--   0        0        0    18326 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/client.py
--rw-r--r--   0        0        0       22 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/config.py
--rw-r--r--   0        0        0       65 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/connectors/__init__.py
--rw-r--r--   0        0        0    46627 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/connectors/client.py
--rw-r--r--   0        0        0      790 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/core/api_error.py
--rw-r--r--   0        0        0     2226 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/core/file.py
--rw-r--r--   0        0        0     5059 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/core/http_client.py
--rw-r--r--   0        0        0     3799 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/core/request_options.py
--rw-r--r--   0        0        0      289 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/datasets/__init__.py
--rw-r--r--   0        0        0    33980 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/datasets/client.py
--rw-r--r--   0        0        0      417 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/datasets/types/__init__.py
--rw-r--r--   0        0        0      998 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/datasets/types/datasets_create_response.py
--rw-r--r--   0        0        0      958 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/datasets/types/datasets_get_response.py
--rw-r--r--   0        0        0     1053 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/datasets/types/datasets_get_usage_response.py
--rw-r--r--   0        0        0      997 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/datasets/types/datasets_list_response.py
--rw-r--r--   0        0        0      159 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/embed_jobs/__init__.py
--rw-r--r--   0        0        0    29689 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/embed_jobs/client.py
--rw-r--r--   0        0        0      187 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/embed_jobs/types/__init__.py
--rw-r--r--   0        0        0      172 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/embed_jobs/types/create_embed_job_request_truncate.py
--rw-r--r--   0        0        0      159 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/environment.py
--rw-r--r--   0        0        0      617 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/errors/__init__.py
--rw-r--r--   0        0        0      248 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/errors/bad_request_error.py
--rw-r--r--   0        0        0      247 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/errors/forbidden_error.py
--rw-r--r--   0        0        0      252 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/errors/internal_server_error.py
--rw-r--r--   0        0        0      246 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/errors/not_found_error.py
--rw-r--r--   0        0        0      290 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/errors/service_unavailable_error.py
--rw-r--r--   0        0        0      253 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/errors/too_many_requests_error.py
--rw-r--r--   0        0        0      284 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/errors/unauthorized_error.py
--rw-r--r--   0        0        0      953 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/__init__.py
--rw-r--r--   0        0        0    56439 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/client.py
--rw-r--r--   0        0        0      905 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/finetuning/__init__.py
--rw-r--r--   0        0        0     1343 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/finetuning/types/__init__.py
--rw-r--r--   0        0        0     1460 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/finetuning/types/base_model.py
--rw-r--r--   0        0        0      308 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/finetuning/types/base_type.py
--rw-r--r--   0        0        0     1169 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/finetuning/types/create_finetuned_model_response.py
--rw-r--r--   0        0        0      140 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/finetuning/types/delete_finetuned_model_response.py
--rw-r--r--   0        0        0     1077 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/finetuning/types/error.py
--rw-r--r--   0        0        0     1388 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/finetuning/types/event.py
--rw-r--r--   0        0        0     2324 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/finetuning/types/finetuned_model.py
--rw-r--r--   0        0        0     1165 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/finetuning/types/get_finetuned_model_response.py
--rw-r--r--   0        0        0     1805 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/finetuning/types/hyperparameters.py
--rw-r--r--   0        0        0     1477 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/finetuning/types/list_events_response.py
--rw-r--r--   0        0        0     1520 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/finetuning/types/list_finetuned_models_response.py
--rw-r--r--   0        0        0     1454 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/finetuning/types/list_training_step_metrics_response.py
--rw-r--r--   0        0        0     1562 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/finetuning/types/settings.py
--rw-r--r--   0        0        0      405 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/finetuning/types/status.py
--rw-r--r--   0        0        0      196 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/finetuning/types/strategy.py
--rw-r--r--   0        0        0     1378 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/finetuning/types/training_step_metrics.py
--rw-r--r--   0        0        0     1171 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/finetuning/types/update_finetuned_model_response.py
--rw-r--r--   0        0        0      811 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/manually_maintained/cache.py
--rw-r--r--   0        0        0     1948 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/manually_maintained/tokenizers.py
--rw-r--r--   0        0        0       65 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/models/__init__.py
--rw-r--r--   0        0        0    12477 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/models/client.py
--rw-r--r--   0        0        0      730 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/overrides.py
--rw-r--r--   0        0        0        0 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/py.typed
--rw-r--r--   0        0        0    10138 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/__init__.py
--rw-r--r--   0        0        0     1168 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/api_meta.py
--rw-r--r--   0        0        0     1012 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/api_meta_api_version.py
--rw-r--r--   0        0        0     1423 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/api_meta_billed_units.py
--rw-r--r--   0        0        0      171 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/auth_token_type.py
--rw-r--r--   0        0        0     1918 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_citation.py
--rw-r--r--   0        0        0     1184 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_citation_generation_event.py
--rw-r--r--   0        0        0     1850 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_connector.py
--rw-r--r--   0        0        0     1412 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_data_metrics.py
--rw-r--r--   0        0        0      117 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_document.py
--rw-r--r--   0        0        0     1639 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_message.py
--rw-r--r--   0        0        0      171 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_message_role.py
--rw-r--r--   0        0        0      173 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_request_citation_quality.py
--rw-r--r--   0        0        0     1706 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_request_connectors_search_options.py
--rw-r--r--   0        0        0      192 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_request_prompt_truncation.py
--rw-r--r--   0        0        0     1012 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_request_tool_results_item.py
--rw-r--r--   0        0        0     1237 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_search_queries_generation_event.py
--rw-r--r--   0        0        0     1242 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_search_query.py
--rw-r--r--   0        0        0     1642 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_search_result.py
--rw-r--r--   0        0        0     1053 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_search_result_connector.py
--rw-r--r--   0        0        0     1471 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_search_results_event.py
--rw-r--r--   0        0        0     1915 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_stream_end_event.py
--rw-r--r--   0        0        0      228 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_stream_end_event_finish_reason.py
--rw-r--r--   0        0        0      894 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_stream_event.py
--rw-r--r--   0        0        0      179 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_stream_request_citation_quality.py
--rw-r--r--   0        0        0     1712 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_stream_request_connectors_search_options.py
--rw-r--r--   0        0        0      198 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_stream_request_prompt_truncation.py
--rw-r--r--   0        0        0     1018 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_stream_request_tool_results_item.py
--rw-r--r--   0        0        0     1159 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_stream_start_event.py
--rw-r--r--   0        0        0     1125 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_text_generation_event.py
--rw-r--r--   0        0        0     1100 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_tool_calls_generation_event.py
--rw-r--r--   0        0        0     1129 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/classify_data_metrics.py
--rw-r--r--   0        0        0      972 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/classify_example.py
--rw-r--r--   0        0        0      174 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/classify_request_truncate.py
--rw-r--r--   0        0        0     1138 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/classify_response.py
--rw-r--r--   0        0        0     2540 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/classify_response_classifications_item.py
--rw-r--r--   0        0        0      217 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/classify_response_classifications_item_classification_type.py
--rw-r--r--   0        0        0      972 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/classify_response_classifications_item_labels_value.py
--rw-r--r--   0        0        0      223 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/compatible_endpoint.py
--rw-r--r--   0        0        0     3345 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/connector.py
--rw-r--r--   0        0        0      166 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/connector_auth_status.py
--rw-r--r--   0        0        0     1646 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/connector_o_auth.py
--rw-r--r--   0        0        0     1711 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/create_connector_o_auth.py
--rw-r--r--   0        0        0      961 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/create_connector_response.py
--rw-r--r--   0        0        0     1193 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/create_connector_service_auth.py
--rw-r--r--   0        0        0     1048 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/create_embed_job_response.py
--rw-r--r--   0        0        0     2186 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/dataset.py
--rw-r--r--   0        0        0     1628 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/dataset_part.py
--rw-r--r--   0        0        0      474 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/dataset_type.py
--rw-r--r--   0        0        0      225 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/dataset_validation_status.py
--rw-r--r--   0        0        0      135 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/delete_connector_response.py
--rw-r--r--   0        0        0     1066 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/detokenize_response.py
--rw-r--r--   0        0        0     1411 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/embed_by_type_response.py
--rw-r--r--   0        0        0     2265 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/embed_by_type_response_embeddings.py
--rw-r--r--   0        0        0     1359 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/embed_floats_response.py
--rw-r--r--   0        0        0      214 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/embed_input_type.py
--rw-r--r--   0        0        0     1841 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/embed_job.py
--rw-r--r--   0        0        0      210 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/embed_job_status.py
--rw-r--r--   0        0        0      159 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/embed_job_truncate.py
--rw-r--r--   0        0        0      171 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/embed_request_truncate.py
--rw-r--r--   0        0        0      847 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/embed_response.py
--rw-r--r--   0        0        0      187 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/embedding_type.py
--rw-r--r--   0        0        0     1940 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/finetune_dataset_metrics.py
--rw-r--r--   0        0        0      225 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/finish_reason.py
--rw-r--r--   0        0        0      188 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/generate_request_return_likelihoods.py
--rw-r--r--   0        0        0      174 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/generate_request_truncate.py
--rw-r--r--   0        0        0     1257 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/generate_stream_end.py
--rw-r--r--   0        0        0     1102 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/generate_stream_end_response.py
--rw-r--r--   0        0        0     1365 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/generate_stream_error.py
--rw-r--r--   0        0        0      898 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/generate_stream_event.py
--rw-r--r--   0        0        0      194 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/generate_stream_request_return_likelihoods.py
--rw-r--r--   0        0        0      180 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/generate_stream_request_truncate.py
--rw-r--r--   0        0        0     1366 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/generate_stream_text.py
--rw-r--r--   0        0        0     1217 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/generate_streamed_response.py
--rw-r--r--   0        0        0     1249 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/generation.py
--rw-r--r--   0        0        0      958 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/get_connector_response.py
--rw-r--r--   0        0        0     2095 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/get_model_response.py
--rw-r--r--   0        0        0     1349 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/label_metric.py
--rw-r--r--   0        0        0     1093 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/list_connectors_response.py
--rw-r--r--   0        0        0      994 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/list_embed_job_response.py
--rw-r--r--   0        0        0     1185 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/list_models_response.py
--rw-r--r--   0        0        0     1025 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/metrics.py
--rw-r--r--   0        0        0     2678 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/non_streamed_chat_response.py
--rw-r--r--   0        0        0     1078 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/o_auth_authorize_response.py
--rw-r--r--   0        0        0      975 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/parse_info.py
--rw-r--r--   0        0        0      239 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/rerank_request_documents_item.py
--rw-r--r--   0        0        0      999 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/rerank_request_documents_item_text.py
--rw-r--r--   0        0        0     1198 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/rerank_response.py
--rw-r--r--   0        0        0     1334 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/rerank_response_results_item.py
--rw-r--r--   0        0        0     1054 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/rerank_response_results_item_document.py
--rw-r--r--   0        0        0     2056 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/reranker_data_metrics.py
--rw-r--r--   0        0        0     1800 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/single_generation.py
--rw-r--r--   0        0        0     1243 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/single_generation_in_stream.py
--rw-r--r--   0        0        0      953 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/single_generation_token_likelihoods_item.py
--rw-r--r--   0        0        0     2812 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/streamed_chat_response.py
--rw-r--r--   0        0        0      182 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/summarize_request_extractiveness.py
--rw-r--r--   0        0        0      173 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/summarize_request_format.py
--rw-r--r--   0        0        0      176 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/summarize_request_length.py
--rw-r--r--   0        0        0     1196 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/summarize_response.py
--rw-r--r--   0        0        0     1125 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/tokenize_response.py
--rw-r--r--   0        0        0     1920 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/tool.py
--rw-r--r--   0        0        0     1216 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/tool_call.py
--rw-r--r--   0        0        0     1323 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/tool_parameter_definitions_value.py
--rw-r--r--   0        0        0      961 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/update_connector_response.py
--rw-r--r--   0        0        0    10025 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/utils.py
--rw-r--r--   0        0        0       74 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/version.py
--rw-r--r--   0        0        0     3035 1970-01-01 00:00:00.000000 cohere-5.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-04-03 19:30:40.460818 cohere-5.2.1/LICENSE
+-rw-r--r--   0        0        0     2359 2024-04-03 19:30:40.460818 cohere-5.2.1/README.md
+-rw-r--r--   0        0        0      690 2024-04-03 19:30:40.468819 cohere-5.2.1/pyproject.toml
+-rw-r--r--   0        0        0     7869 2024-04-03 19:30:40.468819 cohere-5.2.1/src/cohere/__init__.py
+-rw-r--r--   0        0        0   197822 2024-04-03 19:30:40.468819 cohere-5.2.1/src/cohere/base_client.py
+-rw-r--r--   0        0        0    18330 2024-04-03 19:30:40.468819 cohere-5.2.1/src/cohere/client.py
+-rw-r--r--   0        0        0       22 2024-04-03 19:30:40.468819 cohere-5.2.1/src/cohere/config.py
+-rw-r--r--   0        0        0       65 2024-04-03 19:30:40.468819 cohere-5.2.1/src/cohere/connectors/__init__.py
+-rw-r--r--   0        0        0    46627 2024-04-03 19:30:40.468819 cohere-5.2.1/src/cohere/connectors/client.py
+-rw-r--r--   0        0        0      790 2024-04-03 19:30:40.468819 cohere-5.2.1/src/cohere/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-03 19:30:40.468819 cohere-5.2.1/src/cohere/core/api_error.py
+-rw-r--r--   0        0        0     2226 2024-04-03 19:30:40.468819 cohere-5.2.1/src/cohere/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-03 19:30:40.468819 cohere-5.2.1/src/cohere/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-03 19:30:40.468819 cohere-5.2.1/src/cohere/core/file.py
+-rw-r--r--   0        0        0     5059 2024-04-03 19:30:40.468819 cohere-5.2.1/src/cohere/core/http_client.py
+-rw-r--r--   0        0        0     3898 2024-04-03 19:30:40.468819 cohere-5.2.1/src/cohere/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-04-03 19:30:40.468819 cohere-5.2.1/src/cohere/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/core/request_options.py
+-rw-r--r--   0        0        0      289 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/datasets/__init__.py
+-rw-r--r--   0        0        0    33980 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/datasets/client.py
+-rw-r--r--   0        0        0      417 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/datasets/types/__init__.py
+-rw-r--r--   0        0        0      998 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/datasets/types/datasets_create_response.py
+-rw-r--r--   0        0        0      958 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/datasets/types/datasets_get_response.py
+-rw-r--r--   0        0        0     1053 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/datasets/types/datasets_get_usage_response.py
+-rw-r--r--   0        0        0      997 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/datasets/types/datasets_list_response.py
+-rw-r--r--   0        0        0      159 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/embed_jobs/__init__.py
+-rw-r--r--   0        0        0    29689 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/embed_jobs/client.py
+-rw-r--r--   0        0        0      187 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/embed_jobs/types/__init__.py
+-rw-r--r--   0        0        0      172 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/embed_jobs/types/create_embed_job_request_truncate.py
+-rw-r--r--   0        0        0      159 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/environment.py
+-rw-r--r--   0        0        0      617 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/errors/__init__.py
+-rw-r--r--   0        0        0      248 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/errors/bad_request_error.py
+-rw-r--r--   0        0        0      247 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/errors/forbidden_error.py
+-rw-r--r--   0        0        0      252 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/errors/internal_server_error.py
+-rw-r--r--   0        0        0      246 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/errors/not_found_error.py
+-rw-r--r--   0        0        0      290 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/errors/service_unavailable_error.py
+-rw-r--r--   0        0        0      253 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/errors/too_many_requests_error.py
+-rw-r--r--   0        0        0      284 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      953 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/finetuning/__init__.py
+-rw-r--r--   0        0        0    56439 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/finetuning/client.py
+-rw-r--r--   0        0        0      905 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/finetuning/finetuning/__init__.py
+-rw-r--r--   0        0        0     1343 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/finetuning/finetuning/types/__init__.py
+-rw-r--r--   0        0        0     1460 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/finetuning/finetuning/types/base_model.py
+-rw-r--r--   0        0        0      308 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/finetuning/finetuning/types/base_type.py
+-rw-r--r--   0        0        0     1169 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/finetuning/finetuning/types/create_finetuned_model_response.py
+-rw-r--r--   0        0        0      140 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/finetuning/finetuning/types/delete_finetuned_model_response.py
+-rw-r--r--   0        0        0     1077 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/finetuning/finetuning/types/error.py
+-rw-r--r--   0        0        0     1388 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/finetuning/finetuning/types/event.py
+-rw-r--r--   0        0        0     2324 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/finetuning/finetuning/types/finetuned_model.py
+-rw-r--r--   0        0        0     1165 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/finetuning/finetuning/types/get_finetuned_model_response.py
+-rw-r--r--   0        0        0     1805 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/finetuning/finetuning/types/hyperparameters.py
+-rw-r--r--   0        0        0     1477 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/finetuning/finetuning/types/list_events_response.py
+-rw-r--r--   0        0        0     1520 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/finetuning/finetuning/types/list_finetuned_models_response.py
+-rw-r--r--   0        0        0     1454 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/finetuning/finetuning/types/list_training_step_metrics_response.py
+-rw-r--r--   0        0        0     1562 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/finetuning/finetuning/types/settings.py
+-rw-r--r--   0        0        0      405 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/finetuning/finetuning/types/status.py
+-rw-r--r--   0        0        0      196 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/finetuning/finetuning/types/strategy.py
+-rw-r--r--   0        0        0     1378 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/finetuning/finetuning/types/training_step_metrics.py
+-rw-r--r--   0        0        0     1171 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/finetuning/finetuning/types/update_finetuned_model_response.py
+-rw-r--r--   0        0        0      811 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/manually_maintained/cache.py
+-rw-r--r--   0        0        0     1948 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/manually_maintained/tokenizers.py
+-rw-r--r--   0        0        0       65 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/models/__init__.py
+-rw-r--r--   0        0        0    12477 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/models/client.py
+-rw-r--r--   0        0        0      730 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/overrides.py
+-rw-r--r--   0        0        0        0 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/py.typed
+-rw-r--r--   0        0        0    10138 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/__init__.py
+-rw-r--r--   0        0        0     1168 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/api_meta.py
+-rw-r--r--   0        0        0     1012 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/api_meta_api_version.py
+-rw-r--r--   0        0        0     1423 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/api_meta_billed_units.py
+-rw-r--r--   0        0        0      171 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/auth_token_type.py
+-rw-r--r--   0        0        0     1918 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/chat_citation.py
+-rw-r--r--   0        0        0     1184 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/chat_citation_generation_event.py
+-rw-r--r--   0        0        0     1850 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/chat_connector.py
+-rw-r--r--   0        0        0     1412 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/chat_data_metrics.py
+-rw-r--r--   0        0        0      117 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/chat_document.py
+-rw-r--r--   0        0        0     1639 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/chat_message.py
+-rw-r--r--   0        0        0      171 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/chat_message_role.py
+-rw-r--r--   0        0        0      173 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/chat_request_citation_quality.py
+-rw-r--r--   0        0        0     1706 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/chat_request_connectors_search_options.py
+-rw-r--r--   0        0        0      192 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/chat_request_prompt_truncation.py
+-rw-r--r--   0        0        0     1012 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/chat_request_tool_results_item.py
+-rw-r--r--   0        0        0     1237 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/chat_search_queries_generation_event.py
+-rw-r--r--   0        0        0     1242 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/chat_search_query.py
+-rw-r--r--   0        0        0     1642 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/chat_search_result.py
+-rw-r--r--   0        0        0     1053 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/chat_search_result_connector.py
+-rw-r--r--   0        0        0     1471 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/chat_search_results_event.py
+-rw-r--r--   0        0        0     1915 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/chat_stream_end_event.py
+-rw-r--r--   0        0        0      228 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/chat_stream_end_event_finish_reason.py
+-rw-r--r--   0        0        0      894 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/chat_stream_event.py
+-rw-r--r--   0        0        0      179 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/chat_stream_request_citation_quality.py
+-rw-r--r--   0        0        0     1712 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/chat_stream_request_connectors_search_options.py
+-rw-r--r--   0        0        0      198 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/chat_stream_request_prompt_truncation.py
+-rw-r--r--   0        0        0     1018 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/chat_stream_request_tool_results_item.py
+-rw-r--r--   0        0        0     1159 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/chat_stream_start_event.py
+-rw-r--r--   0        0        0     1125 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/chat_text_generation_event.py
+-rw-r--r--   0        0        0     1100 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/chat_tool_calls_generation_event.py
+-rw-r--r--   0        0        0     1129 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/classify_data_metrics.py
+-rw-r--r--   0        0        0      972 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/classify_example.py
+-rw-r--r--   0        0        0      174 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/classify_request_truncate.py
+-rw-r--r--   0        0        0     1138 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/classify_response.py
+-rw-r--r--   0        0        0     2540 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/classify_response_classifications_item.py
+-rw-r--r--   0        0        0      217 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/classify_response_classifications_item_classification_type.py
+-rw-r--r--   0        0        0      972 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/classify_response_classifications_item_labels_value.py
+-rw-r--r--   0        0        0      223 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/compatible_endpoint.py
+-rw-r--r--   0        0        0     3345 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/connector.py
+-rw-r--r--   0        0        0      166 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/connector_auth_status.py
+-rw-r--r--   0        0        0     1646 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/connector_o_auth.py
+-rw-r--r--   0        0        0     1711 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/create_connector_o_auth.py
+-rw-r--r--   0        0        0      961 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/create_connector_response.py
+-rw-r--r--   0        0        0     1193 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/create_connector_service_auth.py
+-rw-r--r--   0        0        0     1048 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/create_embed_job_response.py
+-rw-r--r--   0        0        0     2186 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/dataset.py
+-rw-r--r--   0        0        0     1628 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/dataset_part.py
+-rw-r--r--   0        0        0      474 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/dataset_type.py
+-rw-r--r--   0        0        0      225 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/dataset_validation_status.py
+-rw-r--r--   0        0        0      135 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/delete_connector_response.py
+-rw-r--r--   0        0        0     1066 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/detokenize_response.py
+-rw-r--r--   0        0        0     1411 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/embed_by_type_response.py
+-rw-r--r--   0        0        0     2265 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/embed_by_type_response_embeddings.py
+-rw-r--r--   0        0        0     1359 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/embed_floats_response.py
+-rw-r--r--   0        0        0      214 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/embed_input_type.py
+-rw-r--r--   0        0        0     1841 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/embed_job.py
+-rw-r--r--   0        0        0      210 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/embed_job_status.py
+-rw-r--r--   0        0        0      159 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/embed_job_truncate.py
+-rw-r--r--   0        0        0      171 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/embed_request_truncate.py
+-rw-r--r--   0        0        0      847 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/embed_response.py
+-rw-r--r--   0        0        0      187 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/embedding_type.py
+-rw-r--r--   0        0        0     1940 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/finetune_dataset_metrics.py
+-rw-r--r--   0        0        0      225 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/finish_reason.py
+-rw-r--r--   0        0        0      188 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/generate_request_return_likelihoods.py
+-rw-r--r--   0        0        0      174 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/generate_request_truncate.py
+-rw-r--r--   0        0        0     1257 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/generate_stream_end.py
+-rw-r--r--   0        0        0     1102 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/generate_stream_end_response.py
+-rw-r--r--   0        0        0     1365 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/generate_stream_error.py
+-rw-r--r--   0        0        0      898 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/generate_stream_event.py
+-rw-r--r--   0        0        0      194 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/generate_stream_request_return_likelihoods.py
+-rw-r--r--   0        0        0      180 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/generate_stream_request_truncate.py
+-rw-r--r--   0        0        0     1366 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/generate_stream_text.py
+-rw-r--r--   0        0        0     1217 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/generate_streamed_response.py
+-rw-r--r--   0        0        0     1249 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/generation.py
+-rw-r--r--   0        0        0      958 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/get_connector_response.py
+-rw-r--r--   0        0        0     2095 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/get_model_response.py
+-rw-r--r--   0        0        0     1349 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/label_metric.py
+-rw-r--r--   0        0        0     1093 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/list_connectors_response.py
+-rw-r--r--   0        0        0      994 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/list_embed_job_response.py
+-rw-r--r--   0        0        0     1185 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/list_models_response.py
+-rw-r--r--   0        0        0     1025 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/metrics.py
+-rw-r--r--   0        0        0     2678 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/non_streamed_chat_response.py
+-rw-r--r--   0        0        0     1078 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/o_auth_authorize_response.py
+-rw-r--r--   0        0        0      975 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/parse_info.py
+-rw-r--r--   0        0        0      239 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/rerank_request_documents_item.py
+-rw-r--r--   0        0        0      999 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/rerank_request_documents_item_text.py
+-rw-r--r--   0        0        0     1198 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/rerank_response.py
+-rw-r--r--   0        0        0     1334 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/rerank_response_results_item.py
+-rw-r--r--   0        0        0     1054 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/rerank_response_results_item_document.py
+-rw-r--r--   0        0        0     2056 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/reranker_data_metrics.py
+-rw-r--r--   0        0        0     1800 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/single_generation.py
+-rw-r--r--   0        0        0     1243 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/single_generation_in_stream.py
+-rw-r--r--   0        0        0      953 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/single_generation_token_likelihoods_item.py
+-rw-r--r--   0        0        0     2812 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/streamed_chat_response.py
+-rw-r--r--   0        0        0      182 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/summarize_request_extractiveness.py
+-rw-r--r--   0        0        0      173 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/summarize_request_format.py
+-rw-r--r--   0        0        0      176 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/summarize_request_length.py
+-rw-r--r--   0        0        0     1196 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/summarize_response.py
+-rw-r--r--   0        0        0     1125 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/tokenize_response.py
+-rw-r--r--   0        0        0     1920 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/tool.py
+-rw-r--r--   0        0        0     1216 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/tool_call.py
+-rw-r--r--   0        0        0     1323 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/tool_parameter_definitions_value.py
+-rw-r--r--   0        0        0      961 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/types/update_connector_response.py
+-rw-r--r--   0        0        0    10025 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/utils.py
+-rw-r--r--   0        0        0       74 2024-04-03 19:30:40.472818 cohere-5.2.1/src/cohere/version.py
+-rw-r--r--   0        0        0     3035 1970-01-01 00:00:00.000000 cohere-5.2.1/PKG-INFO
```

### Comparing `cohere-5.2.0/LICENSE` & `cohere-5.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/README.md` & `cohere-5.2.1/README.md`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/pyproject.toml` & `cohere-5.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 [tool.poetry]
 name = "cohere"
-version = "5.2.0"
+version = "5.2.1"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
     { include = "cohere", from = "src"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 fastavro = "^1.9.4"
 httpx = ">=0.21.2"
 pydantic = ">= 1.9.2"
-tokenizers = "^0.15.2"
 requests = "^2.31.0"
+tokenizers = "^0.15.2"
 types-requests = "^2.31.0.20240311"
 typing_extensions = ">= 4.0.0"
 
-
 [tool.poetry.dev-dependencies]
 mypy = "^1.8.0"
 pytest = "^7.4.0"
 pytest-asyncio = "^0.23.5"
 python-dateutil = "^2.9.0"
 
 [tool.pytest.ini_options]
```

### Comparing `cohere-5.2.0/src/cohere/__init__.py` & `cohere-5.2.1/src/cohere/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/base_client.py` & `cohere-5.2.1/src/cohere/base_client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/client.py` & `cohere-5.2.1/src/cohere/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     def __init__(
         self,
         api_key: typing.Optional[typing.Union[str, typing.Callable[[], str]]] = None,
         *,
         base_url: typing.Optional[str] = os.getenv("CO_API_URL"),
         environment: ClientEnvironment = ClientEnvironment.PRODUCTION,
         client_name: typing.Optional[str] = None,
-        timeout: typing.Optional[float] = 60,
+        timeout: typing.Optional[float] = None,
         httpx_client: typing.Optional[httpx.Client] = None,
     ):
         if api_key is None:
             api_key = os.getenv("CO_API_KEY")
 
         BaseCohere.__init__(
             self,
@@ -241,15 +241,15 @@
     def __init__(
         self,
         api_key: typing.Optional[typing.Union[str, typing.Callable[[], str]]] = None,
         *,
         base_url: typing.Optional[str] = os.getenv("CO_API_URL"),
         environment: ClientEnvironment = ClientEnvironment.PRODUCTION,
         client_name: typing.Optional[str] = None,
-        timeout: typing.Optional[float] = 60,
+        timeout: typing.Optional[float] = None,
         httpx_client: typing.Optional[httpx.AsyncClient] = None,
     ):
         if api_key is None:
             api_key = os.getenv("CO_API_KEY")
 
         AsyncBaseCohere.__init__(
             self,
```

### Comparing `cohere-5.2.0/src/cohere/connectors/client.py` & `cohere-5.2.1/src/cohere/connectors/client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/core/__init__.py` & `cohere-5.2.1/src/cohere/core/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/core/client_wrapper.py` & `cohere-5.2.1/src/cohere/core/client_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self._base_url = base_url
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "cohere",
-            "X-Fern-SDK-Version": "5.2.0",
+            "X-Fern-SDK-Version": "5.2.1",
         }
         if self._client_name is not None:
             headers["X-Client-Name"] = self._client_name
         headers["Authorization"] = f"Bearer {self._get_token()}"
         return headers
 
     def _get_token(self) -> str:
```

### Comparing `cohere-5.2.0/src/cohere/core/datetime_utils.py` & `cohere-5.2.1/src/cohere/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/core/file.py` & `cohere-5.2.1/src/cohere/core/file.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/core/http_client.py` & `cohere-5.2.1/src/cohere/core/http_client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/core/jsonable_encoder.py` & `cohere-5.2.1/src/cohere/core/jsonable_encoder.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,47 +12,51 @@
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
+import pydantic
 
 from .datetime_utils import serialize_datetime
 
+IS_PYDANTIC_V2 = pydantic.VERSION.startswith("2.")
+
+if IS_PYDANTIC_V2:
+    import pydantic.v1 as pydantic_v1  # type: ignore
+else:
+    import pydantic as pydantic_v1  # type: ignore
+
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
@@ -80,16 +84,16 @@
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

### Comparing `cohere-5.2.0/src/cohere/core/request_options.py` & `cohere-5.2.1/src/cohere/core/request_options.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/datasets/client.py` & `cohere-5.2.1/src/cohere/datasets/client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/datasets/types/datasets_create_response.py` & `cohere-5.2.1/src/cohere/datasets/types/datasets_create_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/datasets/types/datasets_get_response.py` & `cohere-5.2.1/src/cohere/datasets/types/datasets_get_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/datasets/types/datasets_get_usage_response.py` & `cohere-5.2.1/src/cohere/datasets/types/datasets_get_usage_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/datasets/types/datasets_list_response.py` & `cohere-5.2.1/src/cohere/datasets/types/datasets_list_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/embed_jobs/client.py` & `cohere-5.2.1/src/cohere/embed_jobs/client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/errors/__init__.py` & `cohere-5.2.1/src/cohere/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/finetuning/__init__.py` & `cohere-5.2.1/src/cohere/finetuning/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/finetuning/client.py` & `cohere-5.2.1/src/cohere/finetuning/client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/finetuning/finetuning/__init__.py` & `cohere-5.2.1/src/cohere/finetuning/finetuning/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/finetuning/finetuning/types/__init__.py` & `cohere-5.2.1/src/cohere/finetuning/finetuning/types/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/finetuning/finetuning/types/base_model.py` & `cohere-5.2.1/src/cohere/finetuning/finetuning/types/base_model.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/finetuning/finetuning/types/create_finetuned_model_response.py` & `cohere-5.2.1/src/cohere/finetuning/finetuning/types/create_finetuned_model_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/finetuning/finetuning/types/error.py` & `cohere-5.2.1/src/cohere/finetuning/finetuning/types/error.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/finetuning/finetuning/types/event.py` & `cohere-5.2.1/src/cohere/finetuning/finetuning/types/event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/finetuning/finetuning/types/finetuned_model.py` & `cohere-5.2.1/src/cohere/finetuning/finetuning/types/finetuned_model.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/finetuning/finetuning/types/get_finetuned_model_response.py` & `cohere-5.2.1/src/cohere/finetuning/finetuning/types/get_finetuned_model_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/finetuning/finetuning/types/hyperparameters.py` & `cohere-5.2.1/src/cohere/finetuning/finetuning/types/hyperparameters.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/finetuning/finetuning/types/list_events_response.py` & `cohere-5.2.1/src/cohere/finetuning/finetuning/types/list_events_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/finetuning/finetuning/types/list_finetuned_models_response.py` & `cohere-5.2.1/src/cohere/finetuning/finetuning/types/list_finetuned_models_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/finetuning/finetuning/types/list_training_step_metrics_response.py` & `cohere-5.2.1/src/cohere/finetuning/finetuning/types/list_training_step_metrics_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/finetuning/finetuning/types/settings.py` & `cohere-5.2.1/src/cohere/finetuning/finetuning/types/settings.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/finetuning/finetuning/types/training_step_metrics.py` & `cohere-5.2.1/src/cohere/finetuning/finetuning/types/training_step_metrics.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/finetuning/finetuning/types/update_finetuned_model_response.py` & `cohere-5.2.1/src/cohere/finetuning/finetuning/types/update_finetuned_model_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/manually_maintained/cache.py` & `cohere-5.2.1/src/cohere/manually_maintained/cache.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/manually_maintained/tokenizers.py` & `cohere-5.2.1/src/cohere/manually_maintained/tokenizers.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/models/client.py` & `cohere-5.2.1/src/cohere/models/client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/overrides.py` & `cohere-5.2.1/src/cohere/overrides.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/__init__.py` & `cohere-5.2.1/src/cohere/types/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/api_meta.py` & `cohere-5.2.1/src/cohere/types/api_meta.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/api_meta_api_version.py` & `cohere-5.2.1/src/cohere/types/api_meta_api_version.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/api_meta_billed_units.py` & `cohere-5.2.1/src/cohere/types/api_meta_billed_units.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/chat_citation.py` & `cohere-5.2.1/src/cohere/types/chat_citation.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/chat_citation_generation_event.py` & `cohere-5.2.1/src/cohere/types/chat_citation_generation_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/chat_connector.py` & `cohere-5.2.1/src/cohere/types/chat_connector.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/chat_data_metrics.py` & `cohere-5.2.1/src/cohere/types/chat_data_metrics.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/chat_message.py` & `cohere-5.2.1/src/cohere/types/chat_message.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/chat_request_connectors_search_options.py` & `cohere-5.2.1/src/cohere/types/chat_request_connectors_search_options.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/chat_request_tool_results_item.py` & `cohere-5.2.1/src/cohere/types/chat_request_tool_results_item.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/chat_search_queries_generation_event.py` & `cohere-5.2.1/src/cohere/types/chat_search_queries_generation_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/chat_search_query.py` & `cohere-5.2.1/src/cohere/types/chat_search_query.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/chat_search_result.py` & `cohere-5.2.1/src/cohere/types/chat_search_result.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/chat_search_result_connector.py` & `cohere-5.2.1/src/cohere/types/chat_search_result_connector.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/chat_search_results_event.py` & `cohere-5.2.1/src/cohere/types/chat_search_results_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/chat_stream_end_event.py` & `cohere-5.2.1/src/cohere/types/chat_stream_end_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/chat_stream_event.py` & `cohere-5.2.1/src/cohere/types/chat_stream_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/chat_stream_request_connectors_search_options.py` & `cohere-5.2.1/src/cohere/types/chat_stream_request_connectors_search_options.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/chat_stream_request_tool_results_item.py` & `cohere-5.2.1/src/cohere/types/chat_stream_request_tool_results_item.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/chat_stream_start_event.py` & `cohere-5.2.1/src/cohere/types/chat_stream_start_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/chat_text_generation_event.py` & `cohere-5.2.1/src/cohere/types/chat_text_generation_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/chat_tool_calls_generation_event.py` & `cohere-5.2.1/src/cohere/types/chat_tool_calls_generation_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/classify_data_metrics.py` & `cohere-5.2.1/src/cohere/types/classify_data_metrics.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/classify_example.py` & `cohere-5.2.1/src/cohere/types/classify_example.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/classify_response.py` & `cohere-5.2.1/src/cohere/types/classify_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/classify_response_classifications_item.py` & `cohere-5.2.1/src/cohere/types/classify_response_classifications_item.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/classify_response_classifications_item_labels_value.py` & `cohere-5.2.1/src/cohere/types/classify_response_classifications_item_labels_value.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/connector.py` & `cohere-5.2.1/src/cohere/types/connector.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/connector_o_auth.py` & `cohere-5.2.1/src/cohere/types/connector_o_auth.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/create_connector_o_auth.py` & `cohere-5.2.1/src/cohere/types/create_connector_o_auth.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/create_connector_response.py` & `cohere-5.2.1/src/cohere/types/create_connector_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/create_connector_service_auth.py` & `cohere-5.2.1/src/cohere/types/create_connector_service_auth.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/create_embed_job_response.py` & `cohere-5.2.1/src/cohere/types/create_embed_job_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/dataset.py` & `cohere-5.2.1/src/cohere/types/dataset.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/dataset_part.py` & `cohere-5.2.1/src/cohere/types/dataset_part.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/detokenize_response.py` & `cohere-5.2.1/src/cohere/types/detokenize_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/embed_by_type_response.py` & `cohere-5.2.1/src/cohere/types/embed_by_type_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/embed_by_type_response_embeddings.py` & `cohere-5.2.1/src/cohere/types/embed_by_type_response_embeddings.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/embed_floats_response.py` & `cohere-5.2.1/src/cohere/types/embed_floats_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/embed_job.py` & `cohere-5.2.1/src/cohere/types/embed_job.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/embed_response.py` & `cohere-5.2.1/src/cohere/types/embed_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/finetune_dataset_metrics.py` & `cohere-5.2.1/src/cohere/types/finetune_dataset_metrics.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/generate_stream_end.py` & `cohere-5.2.1/src/cohere/types/generate_stream_end.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/generate_stream_end_response.py` & `cohere-5.2.1/src/cohere/types/generate_stream_end_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/generate_stream_error.py` & `cohere-5.2.1/src/cohere/types/generate_stream_error.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/generate_stream_event.py` & `cohere-5.2.1/src/cohere/types/generate_stream_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/generate_stream_text.py` & `cohere-5.2.1/src/cohere/types/generate_stream_text.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/generate_streamed_response.py` & `cohere-5.2.1/src/cohere/types/generate_streamed_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/generation.py` & `cohere-5.2.1/src/cohere/types/generation.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/get_connector_response.py` & `cohere-5.2.1/src/cohere/types/get_connector_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/get_model_response.py` & `cohere-5.2.1/src/cohere/types/get_model_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/label_metric.py` & `cohere-5.2.1/src/cohere/types/label_metric.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/list_connectors_response.py` & `cohere-5.2.1/src/cohere/types/list_connectors_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/list_embed_job_response.py` & `cohere-5.2.1/src/cohere/types/list_embed_job_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/list_models_response.py` & `cohere-5.2.1/src/cohere/types/list_models_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/metrics.py` & `cohere-5.2.1/src/cohere/types/metrics.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/non_streamed_chat_response.py` & `cohere-5.2.1/src/cohere/types/non_streamed_chat_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/o_auth_authorize_response.py` & `cohere-5.2.1/src/cohere/types/o_auth_authorize_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/parse_info.py` & `cohere-5.2.1/src/cohere/types/parse_info.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/rerank_request_documents_item_text.py` & `cohere-5.2.1/src/cohere/types/rerank_request_documents_item_text.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/rerank_response.py` & `cohere-5.2.1/src/cohere/types/rerank_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/rerank_response_results_item.py` & `cohere-5.2.1/src/cohere/types/rerank_response_results_item.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/rerank_response_results_item_document.py` & `cohere-5.2.1/src/cohere/types/rerank_response_results_item_document.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/reranker_data_metrics.py` & `cohere-5.2.1/src/cohere/types/reranker_data_metrics.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/single_generation.py` & `cohere-5.2.1/src/cohere/types/single_generation.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/single_generation_in_stream.py` & `cohere-5.2.1/src/cohere/types/single_generation_in_stream.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/single_generation_token_likelihoods_item.py` & `cohere-5.2.1/src/cohere/types/single_generation_token_likelihoods_item.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/streamed_chat_response.py` & `cohere-5.2.1/src/cohere/types/streamed_chat_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/summarize_response.py` & `cohere-5.2.1/src/cohere/types/summarize_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/tokenize_response.py` & `cohere-5.2.1/src/cohere/types/tokenize_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/tool.py` & `cohere-5.2.1/src/cohere/types/tool.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/tool_call.py` & `cohere-5.2.1/src/cohere/types/tool_call.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/tool_parameter_definitions_value.py` & `cohere-5.2.1/src/cohere/types/tool_parameter_definitions_value.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/types/update_connector_response.py` & `cohere-5.2.1/src/cohere/types/update_connector_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/src/cohere/utils.py` & `cohere-5.2.1/src/cohere/utils.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.0/PKG-INFO` & `cohere-5.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cohere
-Version: 5.2.0
+Version: 5.2.1
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

