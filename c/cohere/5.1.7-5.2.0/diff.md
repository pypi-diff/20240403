# Comparing `tmp/cohere-5.1.7.tar.gz` & `tmp/cohere-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cohere-5.1.7.tar", max compression
+gzip compressed data, was "cohere-5.2.0.tar", max compression
```

## Comparing `cohere-5.1.7.tar` & `cohere-5.2.0.tar`

### file list

```diff
@@ -1,172 +1,172 @@
--rw-r--r--   0        0        0     1062 2024-03-28 18:58:14.201986 cohere-5.1.7/LICENSE
--rw-r--r--   0        0        0     2359 2024-03-28 18:58:14.201986 cohere-5.1.7/README.md
--rw-r--r--   0        0        0      667 2024-03-28 18:58:14.205986 cohere-5.1.7/pyproject.toml
--rw-r--r--   0        0        0     8009 2024-03-28 18:58:14.205986 cohere-5.1.7/src/cohere/__init__.py
--rw-r--r--   0        0        0   198852 2024-03-28 18:58:14.205986 cohere-5.1.7/src/cohere/base_client.py
--rw-r--r--   0        0        0    13980 2024-03-28 18:58:14.205986 cohere-5.1.7/src/cohere/client.py
--rw-r--r--   0        0        0       22 2024-03-28 18:58:14.205986 cohere-5.1.7/src/cohere/config.py
--rw-r--r--   0        0        0       65 2024-03-28 18:58:14.205986 cohere-5.1.7/src/cohere/connectors/__init__.py
--rw-r--r--   0        0        0    46627 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/connectors/client.py
--rw-r--r--   0        0        0      790 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/core/__init__.py
--rw-r--r--   0        0        0      426 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/core/api_error.py
--rw-r--r--   0        0        0     2226 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/core/file.py
--rw-r--r--   0        0        0     5059 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/core/http_client.py
--rw-r--r--   0        0        0     3799 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/core/request_options.py
--rw-r--r--   0        0        0      289 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/datasets/__init__.py
--rw-r--r--   0        0        0    33556 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/datasets/client.py
--rw-r--r--   0        0        0      417 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/datasets/types/__init__.py
--rw-r--r--   0        0        0      998 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/datasets/types/datasets_create_response.py
--rw-r--r--   0        0        0      958 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/datasets/types/datasets_get_response.py
--rw-r--r--   0        0        0     1053 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/datasets/types/datasets_get_usage_response.py
--rw-r--r--   0        0        0      997 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/datasets/types/datasets_list_response.py
--rw-r--r--   0        0        0      159 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/embed_jobs/__init__.py
--rw-r--r--   0        0        0    29689 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/embed_jobs/client.py
--rw-r--r--   0        0        0      187 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/embed_jobs/types/__init__.py
--rw-r--r--   0        0        0      172 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/embed_jobs/types/create_embed_job_request_truncate.py
--rw-r--r--   0        0        0      159 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/environment.py
--rw-r--r--   0        0        0      617 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/errors/__init__.py
--rw-r--r--   0        0        0      248 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/errors/bad_request_error.py
--rw-r--r--   0        0        0      247 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/errors/forbidden_error.py
--rw-r--r--   0        0        0      252 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/errors/internal_server_error.py
--rw-r--r--   0        0        0      246 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/errors/not_found_error.py
--rw-r--r--   0        0        0      290 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/errors/service_unavailable_error.py
--rw-r--r--   0        0        0      253 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/errors/too_many_requests_error.py
--rw-r--r--   0        0        0      284 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/errors/unauthorized_error.py
--rw-r--r--   0        0        0      953 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/finetuning/__init__.py
--rw-r--r--   0        0        0    56439 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/finetuning/client.py
--rw-r--r--   0        0        0      905 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/finetuning/finetuning/__init__.py
--rw-r--r--   0        0        0     1343 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/finetuning/finetuning/types/__init__.py
--rw-r--r--   0        0        0     1460 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/finetuning/finetuning/types/base_model.py
--rw-r--r--   0        0        0      308 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/finetuning/finetuning/types/base_type.py
--rw-r--r--   0        0        0     1169 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/finetuning/finetuning/types/create_finetuned_model_response.py
--rw-r--r--   0        0        0      140 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/finetuning/finetuning/types/delete_finetuned_model_response.py
--rw-r--r--   0        0        0     1077 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/finetuning/finetuning/types/error.py
--rw-r--r--   0        0        0     1388 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/finetuning/finetuning/types/event.py
--rw-r--r--   0        0        0     2324 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/finetuning/finetuning/types/finetuned_model.py
--rw-r--r--   0        0        0     1165 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/finetuning/finetuning/types/get_finetuned_model_response.py
--rw-r--r--   0        0        0     1805 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/finetuning/finetuning/types/hyperparameters.py
--rw-r--r--   0        0        0     1477 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/finetuning/finetuning/types/list_events_response.py
--rw-r--r--   0        0        0     1520 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/finetuning/finetuning/types/list_finetuned_models_response.py
--rw-r--r--   0        0        0     1454 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/finetuning/finetuning/types/list_training_step_metrics_response.py
--rw-r--r--   0        0        0     1562 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/finetuning/finetuning/types/settings.py
--rw-r--r--   0        0        0      405 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/finetuning/finetuning/types/status.py
--rw-r--r--   0        0        0      196 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/finetuning/finetuning/types/strategy.py
--rw-r--r--   0        0        0     1378 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/finetuning/finetuning/types/training_step_metrics.py
--rw-r--r--   0        0        0     1171 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/finetuning/finetuning/types/update_finetuned_model_response.py
--rw-r--r--   0        0        0       65 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/models/__init__.py
--rw-r--r--   0        0        0    12477 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/models/client.py
--rw-r--r--   0        0        0      730 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/overrides.py
--rw-r--r--   0        0        0        0 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/py.typed
--rw-r--r--   0        0        0    10359 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/__init__.py
--rw-r--r--   0        0        0     1168 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/api_meta.py
--rw-r--r--   0        0        0     1012 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/api_meta_api_version.py
--rw-r--r--   0        0        0     1423 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/api_meta_billed_units.py
--rw-r--r--   0        0        0      171 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/auth_token_type.py
--rw-r--r--   0        0        0     1918 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/chat_citation.py
--rw-r--r--   0        0        0     1184 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/chat_citation_generation_event.py
--rw-r--r--   0        0        0     1850 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/chat_connector.py
--rw-r--r--   0        0        0     1412 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/chat_data_metrics.py
--rw-r--r--   0        0        0      117 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/chat_document.py
--rw-r--r--   0        0        0     1639 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/chat_message.py
--rw-r--r--   0        0        0      171 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/chat_message_role.py
--rw-r--r--   0        0        0      173 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/chat_request_citation_quality.py
--rw-r--r--   0        0        0     1706 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/chat_request_connectors_search_options.py
--rw-r--r--   0        0        0     1267 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/chat_request_prompt_override.py
--rw-r--r--   0        0        0      192 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/chat_request_prompt_truncation.py
--rw-r--r--   0        0        0     1012 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/chat_request_tool_results_item.py
--rw-r--r--   0        0        0     1237 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/chat_search_queries_generation_event.py
--rw-r--r--   0        0        0     1242 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/chat_search_query.py
--rw-r--r--   0        0        0     1642 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/chat_search_result.py
--rw-r--r--   0        0        0     1053 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/chat_search_result_connector.py
--rw-r--r--   0        0        0     1471 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/chat_search_results_event.py
--rw-r--r--   0        0        0     1915 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/chat_stream_end_event.py
--rw-r--r--   0        0        0      228 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/chat_stream_end_event_finish_reason.py
--rw-r--r--   0        0        0      894 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/chat_stream_event.py
--rw-r--r--   0        0        0      179 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/chat_stream_request_citation_quality.py
--rw-r--r--   0        0        0     1712 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/chat_stream_request_connectors_search_options.py
--rw-r--r--   0        0        0     1273 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/chat_stream_request_prompt_override.py
--rw-r--r--   0        0        0      198 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/chat_stream_request_prompt_truncation.py
--rw-r--r--   0        0        0     1018 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/chat_stream_request_tool_results_item.py
--rw-r--r--   0        0        0     1159 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/chat_stream_start_event.py
--rw-r--r--   0        0        0     1125 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/chat_text_generation_event.py
--rw-r--r--   0        0        0     1100 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/chat_tool_calls_generation_event.py
--rw-r--r--   0        0        0     1129 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/classify_data_metrics.py
--rw-r--r--   0        0        0      972 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/classify_example.py
--rw-r--r--   0        0        0      174 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/classify_request_truncate.py
--rw-r--r--   0        0        0     1138 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/classify_response.py
--rw-r--r--   0        0        0     2540 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/classify_response_classifications_item.py
--rw-r--r--   0        0        0      217 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/classify_response_classifications_item_classification_type.py
--rw-r--r--   0        0        0      972 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/classify_response_classifications_item_labels_value.py
--rw-r--r--   0        0        0      223 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/compatible_endpoint.py
--rw-r--r--   0        0        0     3345 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/connector.py
--rw-r--r--   0        0        0      166 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/connector_auth_status.py
--rw-r--r--   0        0        0     1646 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/connector_o_auth.py
--rw-r--r--   0        0        0     1711 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/create_connector_o_auth.py
--rw-r--r--   0        0        0      961 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/create_connector_response.py
--rw-r--r--   0        0        0     1193 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/create_connector_service_auth.py
--rw-r--r--   0        0        0     1048 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/create_embed_job_response.py
--rw-r--r--   0        0        0     2186 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/dataset.py
--rw-r--r--   0        0        0     1628 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/dataset_part.py
--rw-r--r--   0        0        0      474 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/dataset_type.py
--rw-r--r--   0        0        0      225 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/dataset_validation_status.py
--rw-r--r--   0        0        0      135 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/delete_connector_response.py
--rw-r--r--   0        0        0     1066 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/detokenize_response.py
--rw-r--r--   0        0        0     1411 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/embed_by_type_response.py
--rw-r--r--   0        0        0     2265 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/embed_by_type_response_embeddings.py
--rw-r--r--   0        0        0     1359 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/embed_floats_response.py
--rw-r--r--   0        0        0      214 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/embed_input_type.py
--rw-r--r--   0        0        0     1841 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/embed_job.py
--rw-r--r--   0        0        0      210 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/embed_job_status.py
--rw-r--r--   0        0        0      159 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/embed_job_truncate.py
--rw-r--r--   0        0        0      171 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/embed_request_truncate.py
--rw-r--r--   0        0        0      847 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/embed_response.py
--rw-r--r--   0        0        0      187 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/embedding_type.py
--rw-r--r--   0        0        0     1940 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/finetune_dataset_metrics.py
--rw-r--r--   0        0        0      225 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/finish_reason.py
--rw-r--r--   0        0        0      188 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/generate_request_return_likelihoods.py
--rw-r--r--   0        0        0      174 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/generate_request_truncate.py
--rw-r--r--   0        0        0     1257 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/generate_stream_end.py
--rw-r--r--   0        0        0     1102 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/generate_stream_end_response.py
--rw-r--r--   0        0        0     1365 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/generate_stream_error.py
--rw-r--r--   0        0        0      898 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/generate_stream_event.py
--rw-r--r--   0        0        0      194 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/generate_stream_request_return_likelihoods.py
--rw-r--r--   0        0        0      180 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/generate_stream_request_truncate.py
--rw-r--r--   0        0        0     1366 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/generate_stream_text.py
--rw-r--r--   0        0        0     1217 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/generate_streamed_response.py
--rw-r--r--   0        0        0     1249 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/generation.py
--rw-r--r--   0        0        0      958 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/get_connector_response.py
--rw-r--r--   0        0        0     2095 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/get_model_response.py
--rw-r--r--   0        0        0     1349 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/label_metric.py
--rw-r--r--   0        0        0     1093 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/list_connectors_response.py
--rw-r--r--   0        0        0      994 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/list_embed_job_response.py
--rw-r--r--   0        0        0     1185 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/list_models_response.py
--rw-r--r--   0        0        0     1025 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/metrics.py
--rw-r--r--   0        0        0     2678 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/non_streamed_chat_response.py
--rw-r--r--   0        0        0     1078 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/o_auth_authorize_response.py
--rw-r--r--   0        0        0      975 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/parse_info.py
--rw-r--r--   0        0        0      239 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/rerank_request_documents_item.py
--rw-r--r--   0        0        0      999 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/rerank_request_documents_item_text.py
--rw-r--r--   0        0        0     1198 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/rerank_response.py
--rw-r--r--   0        0        0     1334 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/rerank_response_results_item.py
--rw-r--r--   0        0        0     1054 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/rerank_response_results_item_document.py
--rw-r--r--   0        0        0     2056 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/reranker_data_metrics.py
--rw-r--r--   0        0        0     1800 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/single_generation.py
--rw-r--r--   0        0        0     1243 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/single_generation_in_stream.py
--rw-r--r--   0        0        0      953 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/single_generation_token_likelihoods_item.py
--rw-r--r--   0        0        0     2812 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/streamed_chat_response.py
--rw-r--r--   0        0        0      182 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/summarize_request_extractiveness.py
--rw-r--r--   0        0        0      173 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/summarize_request_format.py
--rw-r--r--   0        0        0      176 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/summarize_request_length.py
--rw-r--r--   0        0        0     1196 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/summarize_response.py
--rw-r--r--   0        0        0     1125 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/tokenize_response.py
--rw-r--r--   0        0        0     1920 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/tool.py
--rw-r--r--   0        0        0     1216 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/tool_call.py
--rw-r--r--   0        0        0     1323 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/tool_parameter_definitions_value.py
--rw-r--r--   0        0        0      961 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/types/update_connector_response.py
--rw-r--r--   0        0        0    10025 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/utils.py
--rw-r--r--   0        0        0       74 2024-03-28 18:58:14.209986 cohere-5.1.7/src/cohere/version.py
--rw-r--r--   0        0        0     2990 1970-01-01 00:00:00.000000 cohere-5.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-04-03 16:39:06.464279 cohere-5.2.0/LICENSE
+-rw-r--r--   0        0        0     2359 2024-04-03 16:39:06.464279 cohere-5.2.0/README.md
+-rw-r--r--   0        0        0      691 2024-04-03 16:39:06.472278 cohere-5.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7869 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/__init__.py
+-rw-r--r--   0        0        0   197822 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/base_client.py
+-rw-r--r--   0        0        0    18326 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/client.py
+-rw-r--r--   0        0        0       22 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/config.py
+-rw-r--r--   0        0        0       65 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/connectors/__init__.py
+-rw-r--r--   0        0        0    46627 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/connectors/client.py
+-rw-r--r--   0        0        0      790 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/core/api_error.py
+-rw-r--r--   0        0        0     2226 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/core/file.py
+-rw-r--r--   0        0        0     5059 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/core/http_client.py
+-rw-r--r--   0        0        0     3799 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/core/request_options.py
+-rw-r--r--   0        0        0      289 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/datasets/__init__.py
+-rw-r--r--   0        0        0    33980 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/datasets/client.py
+-rw-r--r--   0        0        0      417 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/datasets/types/__init__.py
+-rw-r--r--   0        0        0      998 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/datasets/types/datasets_create_response.py
+-rw-r--r--   0        0        0      958 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/datasets/types/datasets_get_response.py
+-rw-r--r--   0        0        0     1053 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/datasets/types/datasets_get_usage_response.py
+-rw-r--r--   0        0        0      997 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/datasets/types/datasets_list_response.py
+-rw-r--r--   0        0        0      159 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/embed_jobs/__init__.py
+-rw-r--r--   0        0        0    29689 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/embed_jobs/client.py
+-rw-r--r--   0        0        0      187 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/embed_jobs/types/__init__.py
+-rw-r--r--   0        0        0      172 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/embed_jobs/types/create_embed_job_request_truncate.py
+-rw-r--r--   0        0        0      159 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/environment.py
+-rw-r--r--   0        0        0      617 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/errors/__init__.py
+-rw-r--r--   0        0        0      248 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/errors/bad_request_error.py
+-rw-r--r--   0        0        0      247 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/errors/forbidden_error.py
+-rw-r--r--   0        0        0      252 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/errors/internal_server_error.py
+-rw-r--r--   0        0        0      246 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/errors/not_found_error.py
+-rw-r--r--   0        0        0      290 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/errors/service_unavailable_error.py
+-rw-r--r--   0        0        0      253 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/errors/too_many_requests_error.py
+-rw-r--r--   0        0        0      284 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      953 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/__init__.py
+-rw-r--r--   0        0        0    56439 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/client.py
+-rw-r--r--   0        0        0      905 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/finetuning/__init__.py
+-rw-r--r--   0        0        0     1343 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/finetuning/types/__init__.py
+-rw-r--r--   0        0        0     1460 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/finetuning/types/base_model.py
+-rw-r--r--   0        0        0      308 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/finetuning/types/base_type.py
+-rw-r--r--   0        0        0     1169 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/finetuning/types/create_finetuned_model_response.py
+-rw-r--r--   0        0        0      140 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/finetuning/types/delete_finetuned_model_response.py
+-rw-r--r--   0        0        0     1077 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/finetuning/types/error.py
+-rw-r--r--   0        0        0     1388 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/finetuning/types/event.py
+-rw-r--r--   0        0        0     2324 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/finetuning/types/finetuned_model.py
+-rw-r--r--   0        0        0     1165 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/finetuning/types/get_finetuned_model_response.py
+-rw-r--r--   0        0        0     1805 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/finetuning/types/hyperparameters.py
+-rw-r--r--   0        0        0     1477 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/finetuning/types/list_events_response.py
+-rw-r--r--   0        0        0     1520 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/finetuning/types/list_finetuned_models_response.py
+-rw-r--r--   0        0        0     1454 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/finetuning/types/list_training_step_metrics_response.py
+-rw-r--r--   0        0        0     1562 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/finetuning/types/settings.py
+-rw-r--r--   0        0        0      405 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/finetuning/types/status.py
+-rw-r--r--   0        0        0      196 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/finetuning/types/strategy.py
+-rw-r--r--   0        0        0     1378 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/finetuning/types/training_step_metrics.py
+-rw-r--r--   0        0        0     1171 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/finetuning/finetuning/types/update_finetuned_model_response.py
+-rw-r--r--   0        0        0      811 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/manually_maintained/cache.py
+-rw-r--r--   0        0        0     1948 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/manually_maintained/tokenizers.py
+-rw-r--r--   0        0        0       65 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/models/__init__.py
+-rw-r--r--   0        0        0    12477 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/models/client.py
+-rw-r--r--   0        0        0      730 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/overrides.py
+-rw-r--r--   0        0        0        0 2024-04-03 16:39:06.472278 cohere-5.2.0/src/cohere/py.typed
+-rw-r--r--   0        0        0    10138 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/__init__.py
+-rw-r--r--   0        0        0     1168 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/api_meta.py
+-rw-r--r--   0        0        0     1012 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/api_meta_api_version.py
+-rw-r--r--   0        0        0     1423 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/api_meta_billed_units.py
+-rw-r--r--   0        0        0      171 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/auth_token_type.py
+-rw-r--r--   0        0        0     1918 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_citation.py
+-rw-r--r--   0        0        0     1184 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_citation_generation_event.py
+-rw-r--r--   0        0        0     1850 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_connector.py
+-rw-r--r--   0        0        0     1412 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_data_metrics.py
+-rw-r--r--   0        0        0      117 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_document.py
+-rw-r--r--   0        0        0     1639 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_message.py
+-rw-r--r--   0        0        0      171 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_message_role.py
+-rw-r--r--   0        0        0      173 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_request_citation_quality.py
+-rw-r--r--   0        0        0     1706 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_request_connectors_search_options.py
+-rw-r--r--   0        0        0      192 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_request_prompt_truncation.py
+-rw-r--r--   0        0        0     1012 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_request_tool_results_item.py
+-rw-r--r--   0        0        0     1237 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_search_queries_generation_event.py
+-rw-r--r--   0        0        0     1242 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_search_query.py
+-rw-r--r--   0        0        0     1642 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_search_result.py
+-rw-r--r--   0        0        0     1053 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_search_result_connector.py
+-rw-r--r--   0        0        0     1471 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_search_results_event.py
+-rw-r--r--   0        0        0     1915 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_stream_end_event.py
+-rw-r--r--   0        0        0      228 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_stream_end_event_finish_reason.py
+-rw-r--r--   0        0        0      894 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_stream_event.py
+-rw-r--r--   0        0        0      179 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_stream_request_citation_quality.py
+-rw-r--r--   0        0        0     1712 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_stream_request_connectors_search_options.py
+-rw-r--r--   0        0        0      198 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_stream_request_prompt_truncation.py
+-rw-r--r--   0        0        0     1018 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_stream_request_tool_results_item.py
+-rw-r--r--   0        0        0     1159 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_stream_start_event.py
+-rw-r--r--   0        0        0     1125 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_text_generation_event.py
+-rw-r--r--   0        0        0     1100 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/chat_tool_calls_generation_event.py
+-rw-r--r--   0        0        0     1129 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/classify_data_metrics.py
+-rw-r--r--   0        0        0      972 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/classify_example.py
+-rw-r--r--   0        0        0      174 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/classify_request_truncate.py
+-rw-r--r--   0        0        0     1138 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/classify_response.py
+-rw-r--r--   0        0        0     2540 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/classify_response_classifications_item.py
+-rw-r--r--   0        0        0      217 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/classify_response_classifications_item_classification_type.py
+-rw-r--r--   0        0        0      972 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/classify_response_classifications_item_labels_value.py
+-rw-r--r--   0        0        0      223 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/compatible_endpoint.py
+-rw-r--r--   0        0        0     3345 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/connector.py
+-rw-r--r--   0        0        0      166 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/connector_auth_status.py
+-rw-r--r--   0        0        0     1646 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/connector_o_auth.py
+-rw-r--r--   0        0        0     1711 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/create_connector_o_auth.py
+-rw-r--r--   0        0        0      961 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/create_connector_response.py
+-rw-r--r--   0        0        0     1193 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/create_connector_service_auth.py
+-rw-r--r--   0        0        0     1048 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/create_embed_job_response.py
+-rw-r--r--   0        0        0     2186 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/dataset.py
+-rw-r--r--   0        0        0     1628 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/dataset_part.py
+-rw-r--r--   0        0        0      474 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/dataset_type.py
+-rw-r--r--   0        0        0      225 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/dataset_validation_status.py
+-rw-r--r--   0        0        0      135 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/delete_connector_response.py
+-rw-r--r--   0        0        0     1066 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/detokenize_response.py
+-rw-r--r--   0        0        0     1411 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/embed_by_type_response.py
+-rw-r--r--   0        0        0     2265 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/embed_by_type_response_embeddings.py
+-rw-r--r--   0        0        0     1359 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/embed_floats_response.py
+-rw-r--r--   0        0        0      214 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/embed_input_type.py
+-rw-r--r--   0        0        0     1841 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/embed_job.py
+-rw-r--r--   0        0        0      210 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/embed_job_status.py
+-rw-r--r--   0        0        0      159 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/embed_job_truncate.py
+-rw-r--r--   0        0        0      171 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/embed_request_truncate.py
+-rw-r--r--   0        0        0      847 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/embed_response.py
+-rw-r--r--   0        0        0      187 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/embedding_type.py
+-rw-r--r--   0        0        0     1940 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/finetune_dataset_metrics.py
+-rw-r--r--   0        0        0      225 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/finish_reason.py
+-rw-r--r--   0        0        0      188 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/generate_request_return_likelihoods.py
+-rw-r--r--   0        0        0      174 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/generate_request_truncate.py
+-rw-r--r--   0        0        0     1257 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/generate_stream_end.py
+-rw-r--r--   0        0        0     1102 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/generate_stream_end_response.py
+-rw-r--r--   0        0        0     1365 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/generate_stream_error.py
+-rw-r--r--   0        0        0      898 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/generate_stream_event.py
+-rw-r--r--   0        0        0      194 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/generate_stream_request_return_likelihoods.py
+-rw-r--r--   0        0        0      180 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/generate_stream_request_truncate.py
+-rw-r--r--   0        0        0     1366 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/generate_stream_text.py
+-rw-r--r--   0        0        0     1217 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/generate_streamed_response.py
+-rw-r--r--   0        0        0     1249 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/generation.py
+-rw-r--r--   0        0        0      958 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/get_connector_response.py
+-rw-r--r--   0        0        0     2095 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/get_model_response.py
+-rw-r--r--   0        0        0     1349 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/label_metric.py
+-rw-r--r--   0        0        0     1093 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/list_connectors_response.py
+-rw-r--r--   0        0        0      994 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/list_embed_job_response.py
+-rw-r--r--   0        0        0     1185 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/list_models_response.py
+-rw-r--r--   0        0        0     1025 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/metrics.py
+-rw-r--r--   0        0        0     2678 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/non_streamed_chat_response.py
+-rw-r--r--   0        0        0     1078 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/o_auth_authorize_response.py
+-rw-r--r--   0        0        0      975 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/parse_info.py
+-rw-r--r--   0        0        0      239 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/rerank_request_documents_item.py
+-rw-r--r--   0        0        0      999 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/rerank_request_documents_item_text.py
+-rw-r--r--   0        0        0     1198 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/rerank_response.py
+-rw-r--r--   0        0        0     1334 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/rerank_response_results_item.py
+-rw-r--r--   0        0        0     1054 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/rerank_response_results_item_document.py
+-rw-r--r--   0        0        0     2056 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/reranker_data_metrics.py
+-rw-r--r--   0        0        0     1800 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/single_generation.py
+-rw-r--r--   0        0        0     1243 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/single_generation_in_stream.py
+-rw-r--r--   0        0        0      953 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/single_generation_token_likelihoods_item.py
+-rw-r--r--   0        0        0     2812 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/streamed_chat_response.py
+-rw-r--r--   0        0        0      182 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/summarize_request_extractiveness.py
+-rw-r--r--   0        0        0      173 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/summarize_request_format.py
+-rw-r--r--   0        0        0      176 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/summarize_request_length.py
+-rw-r--r--   0        0        0     1196 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/summarize_response.py
+-rw-r--r--   0        0        0     1125 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/tokenize_response.py
+-rw-r--r--   0        0        0     1920 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/tool.py
+-rw-r--r--   0        0        0     1216 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/tool_call.py
+-rw-r--r--   0        0        0     1323 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/tool_parameter_definitions_value.py
+-rw-r--r--   0        0        0      961 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/types/update_connector_response.py
+-rw-r--r--   0        0        0    10025 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/utils.py
+-rw-r--r--   0        0        0       74 2024-04-03 16:39:06.476278 cohere-5.2.0/src/cohere/version.py
+-rw-r--r--   0        0        0     3035 1970-01-01 00:00:00.000000 cohere-5.2.0/PKG-INFO
```

### Comparing `cohere-5.1.7/LICENSE` & `cohere-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/README.md` & `cohere-5.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/pyproject.toml` & `cohere-5.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 [tool.poetry]
 name = "cohere"
-version = "5.1.7"
+version = "5.2.0"
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
+tokenizers = "^0.15.2"
 requests = "^2.31.0"
 types-requests = "^2.31.0.20240311"
 typing_extensions = ">= 4.0.0"
 
+
 [tool.poetry.dev-dependencies]
 mypy = "^1.8.0"
 pytest = "^7.4.0"
 pytest-asyncio = "^0.23.5"
 python-dateutil = "^2.9.0"
 
 [tool.pytest.ini_options]
```

### Comparing `cohere-5.1.7/src/cohere/__init__.py` & `cohere-5.2.0/src/cohere/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,28 +10,26 @@
     ChatConnector,
     ChatDataMetrics,
     ChatDocument,
     ChatMessage,
     ChatMessageRole,
     ChatRequestCitationQuality,
     ChatRequestConnectorsSearchOptions,
-    ChatRequestPromptOverride,
     ChatRequestPromptTruncation,
     ChatRequestToolResultsItem,
     ChatSearchQueriesGenerationEvent,
     ChatSearchQuery,
     ChatSearchResult,
     ChatSearchResultConnector,
     ChatSearchResultsEvent,
     ChatStreamEndEvent,
     ChatStreamEndEventFinishReason,
     ChatStreamEvent,
     ChatStreamRequestCitationQuality,
     ChatStreamRequestConnectorsSearchOptions,
-    ChatStreamRequestPromptOverride,
     ChatStreamRequestPromptTruncation,
     ChatStreamRequestToolResultsItem,
     ChatStreamStartEvent,
     ChatTextGenerationEvent,
     ChatToolCallsGenerationEvent,
     ClassifyDataMetrics,
     ClassifyExample,
@@ -147,28 +145,26 @@
     "ChatConnector",
     "ChatDataMetrics",
     "ChatDocument",
     "ChatMessage",
     "ChatMessageRole",
     "ChatRequestCitationQuality",
     "ChatRequestConnectorsSearchOptions",
-    "ChatRequestPromptOverride",
     "ChatRequestPromptTruncation",
     "ChatRequestToolResultsItem",
     "ChatSearchQueriesGenerationEvent",
     "ChatSearchQuery",
     "ChatSearchResult",
     "ChatSearchResultConnector",
     "ChatSearchResultsEvent",
     "ChatStreamEndEvent",
     "ChatStreamEndEventFinishReason",
     "ChatStreamEvent",
     "ChatStreamRequestCitationQuality",
     "ChatStreamRequestConnectorsSearchOptions",
-    "ChatStreamRequestPromptOverride",
     "ChatStreamRequestPromptTruncation",
     "ChatStreamRequestToolResultsItem",
     "ChatStreamStartEvent",
     "ChatTextGenerationEvent",
     "ChatToolCallsGenerationEvent",
     "ClassifyDataMetrics",
     "ClassifyExample",
```

### Comparing `cohere-5.1.7/src/cohere/base_client.py` & `cohere-5.2.0/src/cohere/base_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         """
         Generates a text response to a user message.
         To learn how to use Chat with Streaming and RAG follow [this guide](https://docs.cohere.com/docs/cochat-beta#various-ways-of-using-the-chat-endpoint).
 
         Parameters:
             - message: str. Text input for the model to respond to.
 
-            - model: typing.Optional[str]. Defaults to `command`.
+            - model: typing.Optional[str]. Defaults to `command-r`.
 
                                            The name of a compatible [Cohere model](https://docs.cohere.com/docs/models) or the ID of a [fine-tuned](https://docs.cohere.com/docs/chat-fine-tuning) model.
 
             - preamble: typing.Optional[str]. When specified, the default Cohere preamble will be replaced with the provided one. Preambles are a part of the prompt used to adjust the model's overall behavior and conversation style, and use the `SYSTEM` role.
 
                                               The `SYSTEM` role is also used for the contents of the optional `chat_history=` parameter. When used with the `chat_history=` parameter it adds content throughout a conversation. Conversely, when used with the `preamble=` parameter it adds content at the start of the conversation only.
 
@@ -258,15 +258,14 @@
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from cohere import (
             ChatConnector,
             ChatMessage,
             ChatStreamRequestConnectorsSearchOptions,
-            ChatStreamRequestPromptOverride,
             ChatStreamRequestToolResultsItem,
             Tool,
             ToolCall,
             ToolParameterDefinitionsValue,
         )
         from cohere.client import Client
 
@@ -306,19 +305,14 @@
             connectors_search_options=ChatStreamRequestConnectorsSearchOptions(
                 model={"key": "value"},
                 temperature={"key": "value"},
                 max_tokens={"key": "value"},
                 preamble={"key": "value"},
                 seed=1.1,
             ),
-            prompt_override=ChatStreamRequestPromptOverride(
-                preamble={"key": "value"},
-                task_description={"key": "value"},
-                style_guide={"key": "value"},
-            ),
             frequency_penalty=1.1,
             presence_penalty=1.1,
             raw_prompting=True,
             tools=[
                 Tool(
                     name="string",
                     description="string",
@@ -447,15 +441,15 @@
         """
         Generates a text response to a user message.
         To learn how to use Chat with Streaming and RAG follow [this guide](https://docs.cohere.com/docs/cochat-beta#various-ways-of-using-the-chat-endpoint).
 
         Parameters:
             - message: str. Text input for the model to respond to.
 
-            - model: typing.Optional[str]. Defaults to `command`.
+            - model: typing.Optional[str]. Defaults to `command-r`.
 
                                            The name of a compatible [Cohere model](https://docs.cohere.com/docs/models) or the ID of a [fine-tuned](https://docs.cohere.com/docs/chat-fine-tuning) model.
 
             - preamble: typing.Optional[str]. When specified, the default Cohere preamble will be replaced with the provided one. Preambles are a part of the prompt used to adjust the model's overall behavior and conversation style, and use the `SYSTEM` role.
 
                                               The `SYSTEM` role is also used for the contents of the optional `chat_history=` parameter. When used with the `chat_history=` parameter it adds content throughout a conversation. Conversely, when used with the `preamble=` parameter it adds content at the start of the conversation only.
 
@@ -1440,50 +1434,47 @@
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def tokenize(
-        self, *, text: str, model: typing.Optional[str] = OMIT, request_options: typing.Optional[RequestOptions] = None
+        self, *, text: str, model: str, request_options: typing.Optional[RequestOptions] = None
     ) -> TokenizeResponse:
         """
         This endpoint splits input text into smaller units called tokens using byte-pair encoding (BPE). To learn more about tokenization and byte pair encoding, see the tokens page.
 
         Parameters:
             - text: str. The string to be tokenized, the minimum text length is 1 character, and the maximum text length is 65536 characters.
 
-            - model: typing.Optional[str]. An optional parameter to provide the model name. This will ensure that the tokenization uses the tokenizer used by that model.
+            - model: str. An optional parameter to provide the model name. This will ensure that the tokenization uses the tokenizer used by that model.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         client.tokenize(
             text="tokenize me! :D",
             model="command",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"text": text}
-        if model is not OMIT:
-            _request["model"] = model
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "tokenize"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder(_request)
+            json=jsonable_encoder({"text": text, "model": model})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(_request),
+                **jsonable_encoder({"text": text, "model": model}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -1507,53 +1498,47 @@
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def detokenize(
-        self,
-        *,
-        tokens: typing.Sequence[int],
-        model: typing.Optional[str] = OMIT,
-        request_options: typing.Optional[RequestOptions] = None,
+        self, *, tokens: typing.Sequence[int], model: str, request_options: typing.Optional[RequestOptions] = None
     ) -> DetokenizeResponse:
         """
         This endpoint takes tokens using byte-pair encoding and returns their text representation. To learn more about tokenization and byte pair encoding, see the tokens page.
 
         Parameters:
             - tokens: typing.Sequence[int]. The list of tokens to be detokenized.
 
-            - model: typing.Optional[str]. An optional parameter to provide the model name. This will ensure that the detokenization is done by the tokenizer used by that model.
+            - model: str. An optional parameter to provide the model name. This will ensure that the detokenization is done by the tokenizer used by that model.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         client.detokenize(
             tokens=[10104, 12221, 1315, 34, 1420, 69],
+            model="command",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"tokens": tokens}
-        if model is not OMIT:
-            _request["model"] = model
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "detokenize"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder(_request)
+            json=jsonable_encoder({"tokens": tokens, "model": model})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(_request),
+                **jsonable_encoder({"tokens": tokens, "model": model}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -1658,15 +1643,15 @@
         """
         Generates a text response to a user message.
         To learn how to use Chat with Streaming and RAG follow [this guide](https://docs.cohere.com/docs/cochat-beta#various-ways-of-using-the-chat-endpoint).
 
         Parameters:
             - message: str. Text input for the model to respond to.
 
-            - model: typing.Optional[str]. Defaults to `command`.
+            - model: typing.Optional[str]. Defaults to `command-r`.
 
                                            The name of a compatible [Cohere model](https://docs.cohere.com/docs/models) or the ID of a [fine-tuned](https://docs.cohere.com/docs/chat-fine-tuning) model.
 
             - preamble: typing.Optional[str]. When specified, the default Cohere preamble will be replaced with the provided one. Preambles are a part of the prompt used to adjust the model's overall behavior and conversation style, and use the `SYSTEM` role.
 
                                               The `SYSTEM` role is also used for the contents of the optional `chat_history=` parameter. When used with the `chat_history=` parameter it adds content throughout a conversation. Conversely, when used with the `preamble=` parameter it adds content at the start of the conversation only.
 
@@ -1772,15 +1757,14 @@
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from cohere import (
             ChatConnector,
             ChatMessage,
             ChatStreamRequestConnectorsSearchOptions,
-            ChatStreamRequestPromptOverride,
             ChatStreamRequestToolResultsItem,
             Tool,
             ToolCall,
             ToolParameterDefinitionsValue,
         )
         from cohere.client import AsyncClient
 
@@ -1820,19 +1804,14 @@
             connectors_search_options=ChatStreamRequestConnectorsSearchOptions(
                 model={"key": "value"},
                 temperature={"key": "value"},
                 max_tokens={"key": "value"},
                 preamble={"key": "value"},
                 seed=1.1,
             ),
-            prompt_override=ChatStreamRequestPromptOverride(
-                preamble={"key": "value"},
-                task_description={"key": "value"},
-                style_guide={"key": "value"},
-            ),
             frequency_penalty=1.1,
             presence_penalty=1.1,
             raw_prompting=True,
             tools=[
                 Tool(
                     name="string",
                     description="string",
@@ -1961,15 +1940,15 @@
         """
         Generates a text response to a user message.
         To learn how to use Chat with Streaming and RAG follow [this guide](https://docs.cohere.com/docs/cochat-beta#various-ways-of-using-the-chat-endpoint).
 
         Parameters:
             - message: str. Text input for the model to respond to.
 
-            - model: typing.Optional[str]. Defaults to `command`.
+            - model: typing.Optional[str]. Defaults to `command-r`.
 
                                            The name of a compatible [Cohere model](https://docs.cohere.com/docs/models) or the ID of a [fine-tuned](https://docs.cohere.com/docs/chat-fine-tuning) model.
 
             - preamble: typing.Optional[str]. When specified, the default Cohere preamble will be replaced with the provided one. Preambles are a part of the prompt used to adjust the model's overall behavior and conversation style, and use the `SYSTEM` role.
 
                                               The `SYSTEM` role is also used for the contents of the optional `chat_history=` parameter. When used with the `chat_history=` parameter it adds content throughout a conversation. Conversely, when used with the `preamble=` parameter it adds content at the start of the conversation only.
 
@@ -2954,50 +2933,47 @@
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def tokenize(
-        self, *, text: str, model: typing.Optional[str] = OMIT, request_options: typing.Optional[RequestOptions] = None
+        self, *, text: str, model: str, request_options: typing.Optional[RequestOptions] = None
     ) -> TokenizeResponse:
         """
         This endpoint splits input text into smaller units called tokens using byte-pair encoding (BPE). To learn more about tokenization and byte pair encoding, see the tokens page.
 
         Parameters:
             - text: str. The string to be tokenized, the minimum text length is 1 character, and the maximum text length is 65536 characters.
 
-            - model: typing.Optional[str]. An optional parameter to provide the model name. This will ensure that the tokenization uses the tokenizer used by that model.
+            - model: str. An optional parameter to provide the model name. This will ensure that the tokenization uses the tokenizer used by that model.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         await client.tokenize(
             text="tokenize me! :D",
             model="command",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"text": text}
-        if model is not OMIT:
-            _request["model"] = model
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "tokenize"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder(_request)
+            json=jsonable_encoder({"text": text, "model": model})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(_request),
+                **jsonable_encoder({"text": text, "model": model}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -3021,53 +2997,47 @@
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def detokenize(
-        self,
-        *,
-        tokens: typing.Sequence[int],
-        model: typing.Optional[str] = OMIT,
-        request_options: typing.Optional[RequestOptions] = None,
+        self, *, tokens: typing.Sequence[int], model: str, request_options: typing.Optional[RequestOptions] = None
     ) -> DetokenizeResponse:
         """
         This endpoint takes tokens using byte-pair encoding and returns their text representation. To learn more about tokenization and byte pair encoding, see the tokens page.
 
         Parameters:
             - tokens: typing.Sequence[int]. The list of tokens to be detokenized.
 
-            - model: typing.Optional[str]. An optional parameter to provide the model name. This will ensure that the detokenization is done by the tokenizer used by that model.
+            - model: str. An optional parameter to provide the model name. This will ensure that the detokenization is done by the tokenizer used by that model.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         await client.detokenize(
             tokens=[10104, 12221, 1315, 34, 1420, 69],
+            model="command",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"tokens": tokens}
-        if model is not OMIT:
-            _request["model"] = model
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "detokenize"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder(_request)
+            json=jsonable_encoder({"tokens": tokens, "model": model})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(_request),
+                **jsonable_encoder({"tokens": tokens, "model": model}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
```

### Comparing `cohere-5.1.7/src/cohere/client.py` & `cohere-5.2.0/src/cohere/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 import asyncio
 import os
 import typing
 from concurrent.futures import ThreadPoolExecutor
+from tokenizers import Tokenizer  # type: ignore
 
 import httpx
 
+from cohere.types.detokenize_response import DetokenizeResponse
+from cohere.types.tokenize_response import TokenizeResponse
+
 from . import EmbedResponse, EmbedInputType, EmbeddingType, EmbedRequestTruncate
 from .base_client import BaseCohere, AsyncBaseCohere, OMIT
 from .config import embed_batch_size
 from .core import RequestOptions
 from .environment import ClientEnvironment
+from .manually_maintained.cache import CacheMixin
+from .manually_maintained import tokenizers as local_tokenizers
 from .overrides import run_overrides
 from .utils import wait, async_wait, merge_embed_responses, SyncSdkUtils, AsyncSdkUtils
 
 run_overrides()
 
 # Use NoReturn as Never type for compatibility
 Never = typing.NoReturn
@@ -60,24 +66,24 @@
             f"Since python sdk cohere==5.0.0, the function {fn_name}(...) has been deprecated. "
             f"Please update your code. Issues may be filed in https://github.com/cohere-ai/cohere-python/issues."
         )
 
     return fn
 
 
-class Client(BaseCohere):
+class Client(BaseCohere, CacheMixin):
     def __init__(
-            self,
-            api_key: typing.Optional[typing.Union[str, typing.Callable[[], str]]] = None,
-            *,
-            base_url: typing.Optional[str] = os.getenv("CO_API_URL"),
-            environment: ClientEnvironment = ClientEnvironment.PRODUCTION,
-            client_name: typing.Optional[str] = None,
-            timeout: typing.Optional[float] = 60,
-            httpx_client: typing.Optional[httpx.Client] = None,
+        self,
+        api_key: typing.Optional[typing.Union[str, typing.Callable[[], str]]] = None,
+        *,
+        base_url: typing.Optional[str] = os.getenv("CO_API_URL"),
+        environment: ClientEnvironment = ClientEnvironment.PRODUCTION,
+        client_name: typing.Optional[str] = None,
+        timeout: typing.Optional[float] = 60,
+        httpx_client: typing.Optional[httpx.Client] = None,
     ):
         if api_key is None:
             api_key = os.getenv("CO_API_KEY")
 
         BaseCohere.__init__(
             self,
             base_url=base_url,
@@ -101,46 +107,52 @@
         self._client_wrapper.httpx_client.httpx_client.close()
 
     wait = wait
 
     _executor = ThreadPoolExecutor(64)
 
     def embed(
-            self,
-            *,
-            texts: typing.Sequence[str],
-            model: typing.Optional[str] = OMIT,
-            input_type: typing.Optional[EmbedInputType] = OMIT,
-            embedding_types: typing.Optional[typing.Sequence[EmbeddingType]] = OMIT,
-            truncate: typing.Optional[EmbedRequestTruncate] = OMIT,
-            request_options: typing.Optional[RequestOptions] = None,
-            batching: typing.Optional[bool] = True,
+        self,
+        *,
+        texts: typing.Sequence[str],
+        model: typing.Optional[str] = OMIT,
+        input_type: typing.Optional[EmbedInputType] = OMIT,
+        embedding_types: typing.Optional[typing.Sequence[EmbeddingType]] = OMIT,
+        truncate: typing.Optional[EmbedRequestTruncate] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
+        batching: typing.Optional[bool] = True,
     ) -> EmbedResponse:
         if batching is False:
             return BaseCohere.embed(
                 self,
                 texts=texts,
                 model=model,
                 input_type=input_type,
                 embedding_types=embedding_types,
                 truncate=truncate,
                 request_options=request_options,
             )
 
-        texts_batches = [texts[i: i + embed_batch_size] for i in range(0, len(texts), embed_batch_size)]
+        texts_batches = [texts[i : i + embed_batch_size] for i in range(0, len(texts), embed_batch_size)]
 
-        responses = [response for response in self._executor.map(lambda text_batch: BaseCohere.embed(
-                self,
-                texts=text_batch,
-                model=model,
-                input_type=input_type,
-                embedding_types=embedding_types,
-                truncate=truncate,
-                request_options=request_options,
-        ), texts_batches)]
+        responses = [
+            response
+            for response in self._executor.map(
+                lambda text_batch: BaseCohere.embed(
+                    self,
+                    texts=text_batch,
+                    model=model,
+                    input_type=input_type,
+                    embedding_types=embedding_types,
+                    truncate=truncate,
+                    request_options=request_options,
+                ),
+                texts_batches,
+            )
+        ]
 
         return merge_embed_responses(responses)
 
     """
     The following methods have been moved or deprecated in cohere==5.0.0. Please update your usage.
     Issues may be filed in https://github.com/cohere-ai/cohere-python/issues.
     """
@@ -181,25 +193,64 @@
     create_connector: Never = moved_function("create_connector", ".connectors.create")
     update_connector: Never = moved_function("update_connector", ".connectors.update")
     get_connector: Never = moved_function("get_connector", ".connectors.get")
     list_connectors: Never = moved_function("list_connectors", ".connectors.list")
     delete_connector: Never = moved_function("delete_connector", ".connectors.delete")
     oauth_authorize_connector: Never = moved_function("oauth_authorize_connector", ".connectors.o_auth_authorize")
 
+    def tokenize(
+        self,
+        *,
+        text: str,
+        model: str,
+        request_options: typing.Optional[RequestOptions] = None,
+        offline: bool = True,
+    ) -> TokenizeResponse:
+        # `offline` parameter controls whether to use an offline tokenizer. If set to True, the tokenizer config will be downloaded (and cached),
+        # and the request will be processed using the offline tokenizer. If set to False, the request will be processed using the API. The default value is True.
+        if offline:
+            tokens = asyncio.run(local_tokenizers.local_tokenize(self, text=text, model=model))
+            return TokenizeResponse(tokens=tokens, token_strings=[])
+        else:
+            return super().tokenize(text=text, model=model, request_options=request_options)
+
+    def detokenize(
+        self,
+        *,
+        tokens: typing.Sequence[int],
+        model: str,
+        request_options: typing.Optional[RequestOptions] = None,
+        offline: typing.Optional[bool] = True,
+    ) -> DetokenizeResponse:
+        # `offline` parameter controls whether to use an offline tokenizer. If set to True, the tokenizer config will be downloaded (and cached),
+        # and the request will be processed using the offline tokenizer. If set to False, the request will be processed using the API. The default value is True.
+        if offline:
+            model = model or "command"
+            text = asyncio.run(local_tokenizers.local_detokenize(self, model=model, tokens=tokens))
+            return DetokenizeResponse(text=text)
+        else:
+            return super().detokenize(tokens=tokens, model=model, request_options=request_options)
+
+    def fetch_tokenizer(self, *, model: str) -> Tokenizer:
+        """
+        Returns a Hugging Face tokenizer from a given model name.
+        """
+        return local_tokenizers.get_hf_tokenizer(self, model)
+
 
-class AsyncClient(AsyncBaseCohere):
+class AsyncClient(AsyncBaseCohere, CacheMixin):
     def __init__(
-            self,
-            api_key: typing.Optional[typing.Union[str, typing.Callable[[], str]]] = None,
-            *,
-            base_url: typing.Optional[str] = os.getenv("CO_API_URL"),
-            environment: ClientEnvironment = ClientEnvironment.PRODUCTION,
-            client_name: typing.Optional[str] = None,
-            timeout: typing.Optional[float] = 60,
-            httpx_client: typing.Optional[httpx.AsyncClient] = None,
+        self,
+        api_key: typing.Optional[typing.Union[str, typing.Callable[[], str]]] = None,
+        *,
+        base_url: typing.Optional[str] = os.getenv("CO_API_URL"),
+        environment: ClientEnvironment = ClientEnvironment.PRODUCTION,
+        client_name: typing.Optional[str] = None,
+        timeout: typing.Optional[float] = 60,
+        httpx_client: typing.Optional[httpx.AsyncClient] = None,
     ):
         if api_key is None:
             api_key = os.getenv("CO_API_KEY")
 
         AsyncBaseCohere.__init__(
             self,
             base_url=base_url,
@@ -223,46 +274,54 @@
         await self._client_wrapper.httpx_client.httpx_client.aclose()
 
     wait = async_wait
 
     _executor = ThreadPoolExecutor(64)
 
     async def embed(
-            self,
-            *,
-            texts: typing.Sequence[str],
-            model: typing.Optional[str] = OMIT,
-            input_type: typing.Optional[EmbedInputType] = OMIT,
-            embedding_types: typing.Optional[typing.Sequence[EmbeddingType]] = OMIT,
-            truncate: typing.Optional[EmbedRequestTruncate] = OMIT,
-            request_options: typing.Optional[RequestOptions] = None,
-            batching: typing.Optional[bool] = True,
+        self,
+        *,
+        texts: typing.Sequence[str],
+        model: typing.Optional[str] = OMIT,
+        input_type: typing.Optional[EmbedInputType] = OMIT,
+        embedding_types: typing.Optional[typing.Sequence[EmbeddingType]] = OMIT,
+        truncate: typing.Optional[EmbedRequestTruncate] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
+        batching: typing.Optional[bool] = True,
     ) -> EmbedResponse:
         if batching is False:
             return await AsyncBaseCohere.embed(
                 self,
                 texts=texts,
                 model=model,
                 input_type=input_type,
                 embedding_types=embedding_types,
                 truncate=truncate,
                 request_options=request_options,
             )
 
-        texts_batches = [texts[i: i + embed_batch_size] for i in range(0, len(texts), embed_batch_size)]
+        texts_batches = [texts[i : i + embed_batch_size] for i in range(0, len(texts), embed_batch_size)]
 
-        responses = typing.cast(typing.List[EmbedResponse], await asyncio.gather(*[AsyncBaseCohere.embed(
-                self,
-                texts=text_batch,
-                model=model,
-                input_type=input_type,
-                embedding_types=embedding_types,
-                truncate=truncate,
-                request_options=request_options,
-        ) for text_batch in texts_batches]))
+        responses = typing.cast(
+            typing.List[EmbedResponse],
+            await asyncio.gather(
+                *[
+                    AsyncBaseCohere.embed(
+                        self,
+                        texts=text_batch,
+                        model=model,
+                        input_type=input_type,
+                        embedding_types=embedding_types,
+                        truncate=truncate,
+                        request_options=request_options,
+                    )
+                    for text_batch in texts_batches
+                ]
+            ),
+        )
 
         return merge_embed_responses(responses)
 
     """
     The following methods have been moved or deprecated in cohere==5.0.0. Please update your usage.
     Issues may be filed in https://github.com/cohere-ai/cohere-python/issues.
     """
@@ -302,7 +361,47 @@
     list_custom_models: Never = deprecated_function("list_custom_models")
     create_connector: Never = moved_function("create_connector", ".connectors.create")
     update_connector: Never = moved_function("update_connector", ".connectors.update")
     get_connector: Never = moved_function("get_connector", ".connectors.get")
     list_connectors: Never = moved_function("list_connectors", ".connectors.list")
     delete_connector: Never = moved_function("delete_connector", ".connectors.delete")
     oauth_authorize_connector: Never = moved_function("oauth_authorize_connector", ".connectors.o_auth_authorize")
+
+    async def tokenize(
+        self,
+        *,
+        text: str,
+        model: str,
+        request_options: typing.Optional[RequestOptions] = None,
+        offline: typing.Optional[bool] = True,
+    ) -> TokenizeResponse:
+        # `offline` parameter controls whether to use an offline tokenizer. If set to True, the tokenizer config will be downloaded (and cached),
+        # and the request will be processed using the offline tokenizer. If set to False, the request will be processed using the API. The default value is True.
+        if offline:
+            model = model or "command"
+            tokens = await local_tokenizers.local_tokenize(self, model=model, text=text)
+            return TokenizeResponse(tokens=tokens, token_strings=[])
+        else:
+            return await super().tokenize(text=text, model=model, request_options=request_options)
+
+    async def detokenize(
+        self,
+        *,
+        tokens: typing.Sequence[int],
+        model: str,
+        request_options: typing.Optional[RequestOptions] = None,
+        offline: typing.Optional[bool] = True,
+    ) -> DetokenizeResponse:
+        # `offline` parameter controls whether to use an offline tokenizer. If set to True, the tokenizer config will be downloaded (and cached),
+        # and the request will be processed using the offline tokenizer. If set to False, the request will be processed using the API. The default value is True.
+        if offline:
+            model = model or "command"
+            text = await local_tokenizers.local_detokenize(self, model=model, tokens=tokens)
+            return DetokenizeResponse(text=text)
+        else:
+            return await super().detokenize(tokens=tokens, model=model, request_options=request_options)
+
+    async def fetch_tokenizer(self, *, model: str) -> Tokenizer:
+        """
+        Returns a Hugging Face tokenizer from a given model name.
+        """
+        return await local_tokenizers.get_hf_tokenizer(self, model)
```

### Comparing `cohere-5.1.7/src/cohere/connectors/client.py` & `cohere-5.2.0/src/cohere/connectors/client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/core/__init__.py` & `cohere-5.2.0/src/cohere/core/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/core/client_wrapper.py` & `cohere-5.2.0/src/cohere/core/client_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self._base_url = base_url
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "cohere",
-            "X-Fern-SDK-Version": "5.1.7",
+            "X-Fern-SDK-Version": "5.2.0",
         }
         if self._client_name is not None:
             headers["X-Client-Name"] = self._client_name
         headers["Authorization"] = f"Bearer {self._get_token()}"
         return headers
 
     def _get_token(self) -> str:
```

### Comparing `cohere-5.1.7/src/cohere/core/datetime_utils.py` & `cohere-5.2.0/src/cohere/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/core/file.py` & `cohere-5.2.0/src/cohere/core/file.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/core/http_client.py` & `cohere-5.2.0/src/cohere/core/http_client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/core/jsonable_encoder.py` & `cohere-5.2.0/src/cohere/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/core/request_options.py` & `cohere-5.2.0/src/cohere/core/request_options.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/datasets/client.py` & `cohere-5.2.0/src/cohere/datasets/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
     ) -> DatasetsCreateResponse:
         """
         Create a dataset by uploading a file. See ['Dataset Creation'](https://docs.cohere.com/docs/datasets#dataset-creation) for more information.
 
         Parameters:
             - name: str. The name of the uploaded dataset.
 
-            - type: DatasetType. The dataset type, which is used to validate the data.
+            - type: DatasetType. The dataset type, which is used to validate the data. Valid types are `embed-input`, `reranker-finetune-input`, `prompt-completion-finetune-input`, `single-label-classification-finetune-input`, `chat-finetune-input`, and `multi-label-classification-finetune-input`.
 
             - keep_original_file: typing.Optional[bool]. Indicates if the original file should be stored.
 
             - skip_malformed_input: typing.Optional[bool]. Indicates whether rows with malformed input should be dropped (instead of failing the validation check). Dropped rows will be returned in the warnings field.
 
             - keep_fields: typing.Optional[typing.Union[str, typing.Sequence[str]]]. List of names of fields that will be persisted in the Dataset. By default the Dataset will retain only the required fields indicated in the [schema for the corresponding Dataset type](https://docs.cohere.com/docs/datasets#dataset-types). For example, datasets of type `embed-input` will drop all fields other than the required `text` field. If any of the fields in `keep_fields` are missing from the uploaded file, Dataset validation will fail.
 
@@ -464,15 +464,15 @@
     ) -> DatasetsCreateResponse:
         """
         Create a dataset by uploading a file. See ['Dataset Creation'](https://docs.cohere.com/docs/datasets#dataset-creation) for more information.
 
         Parameters:
             - name: str. The name of the uploaded dataset.
 
-            - type: DatasetType. The dataset type, which is used to validate the data.
+            - type: DatasetType. The dataset type, which is used to validate the data. Valid types are `embed-input`, `reranker-finetune-input`, `prompt-completion-finetune-input`, `single-label-classification-finetune-input`, `chat-finetune-input`, and `multi-label-classification-finetune-input`.
 
             - keep_original_file: typing.Optional[bool]. Indicates if the original file should be stored.
 
             - skip_malformed_input: typing.Optional[bool]. Indicates whether rows with malformed input should be dropped (instead of failing the validation check). Dropped rows will be returned in the warnings field.
 
             - keep_fields: typing.Optional[typing.Union[str, typing.Sequence[str]]]. List of names of fields that will be persisted in the Dataset. By default the Dataset will retain only the required fields indicated in the [schema for the corresponding Dataset type](https://docs.cohere.com/docs/datasets#dataset-types). For example, datasets of type `embed-input` will drop all fields other than the required `text` field. If any of the fields in `keep_fields` are missing from the uploaded file, Dataset validation will fail.
```

### Comparing `cohere-5.1.7/src/cohere/datasets/types/datasets_create_response.py` & `cohere-5.2.0/src/cohere/datasets/types/datasets_create_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/datasets/types/datasets_get_response.py` & `cohere-5.2.0/src/cohere/datasets/types/datasets_get_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/datasets/types/datasets_get_usage_response.py` & `cohere-5.2.0/src/cohere/datasets/types/datasets_get_usage_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/datasets/types/datasets_list_response.py` & `cohere-5.2.0/src/cohere/datasets/types/datasets_list_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/embed_jobs/client.py` & `cohere-5.2.0/src/cohere/embed_jobs/client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/errors/__init__.py` & `cohere-5.2.0/src/cohere/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/finetuning/__init__.py` & `cohere-5.2.0/src/cohere/finetuning/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/finetuning/client.py` & `cohere-5.2.0/src/cohere/finetuning/client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/finetuning/finetuning/__init__.py` & `cohere-5.2.0/src/cohere/finetuning/finetuning/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/finetuning/finetuning/types/__init__.py` & `cohere-5.2.0/src/cohere/finetuning/finetuning/types/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/finetuning/finetuning/types/base_model.py` & `cohere-5.2.0/src/cohere/finetuning/finetuning/types/base_model.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/finetuning/finetuning/types/create_finetuned_model_response.py` & `cohere-5.2.0/src/cohere/finetuning/finetuning/types/create_finetuned_model_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/finetuning/finetuning/types/error.py` & `cohere-5.2.0/src/cohere/finetuning/finetuning/types/error.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/finetuning/finetuning/types/event.py` & `cohere-5.2.0/src/cohere/finetuning/finetuning/types/event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/finetuning/finetuning/types/finetuned_model.py` & `cohere-5.2.0/src/cohere/finetuning/finetuning/types/finetuned_model.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/finetuning/finetuning/types/get_finetuned_model_response.py` & `cohere-5.2.0/src/cohere/finetuning/finetuning/types/get_finetuned_model_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/finetuning/finetuning/types/hyperparameters.py` & `cohere-5.2.0/src/cohere/finetuning/finetuning/types/hyperparameters.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/finetuning/finetuning/types/list_events_response.py` & `cohere-5.2.0/src/cohere/finetuning/finetuning/types/list_events_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/finetuning/finetuning/types/list_finetuned_models_response.py` & `cohere-5.2.0/src/cohere/finetuning/finetuning/types/list_finetuned_models_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/finetuning/finetuning/types/list_training_step_metrics_response.py` & `cohere-5.2.0/src/cohere/finetuning/finetuning/types/list_training_step_metrics_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/finetuning/finetuning/types/settings.py` & `cohere-5.2.0/src/cohere/finetuning/finetuning/types/settings.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/finetuning/finetuning/types/training_step_metrics.py` & `cohere-5.2.0/src/cohere/finetuning/finetuning/types/training_step_metrics.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/finetuning/finetuning/types/update_finetuned_model_response.py` & `cohere-5.2.0/src/cohere/finetuning/finetuning/types/update_finetuned_model_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/models/client.py` & `cohere-5.2.0/src/cohere/models/client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/overrides.py` & `cohere-5.2.0/src/cohere/overrides.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/__init__.py` & `cohere-5.2.0/src/cohere/types/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,26 @@
 from .chat_connector import ChatConnector
 from .chat_data_metrics import ChatDataMetrics
 from .chat_document import ChatDocument
 from .chat_message import ChatMessage
 from .chat_message_role import ChatMessageRole
 from .chat_request_citation_quality import ChatRequestCitationQuality
 from .chat_request_connectors_search_options import ChatRequestConnectorsSearchOptions
-from .chat_request_prompt_override import ChatRequestPromptOverride
 from .chat_request_prompt_truncation import ChatRequestPromptTruncation
 from .chat_request_tool_results_item import ChatRequestToolResultsItem
 from .chat_search_queries_generation_event import ChatSearchQueriesGenerationEvent
 from .chat_search_query import ChatSearchQuery
 from .chat_search_result import ChatSearchResult
 from .chat_search_result_connector import ChatSearchResultConnector
 from .chat_search_results_event import ChatSearchResultsEvent
 from .chat_stream_end_event import ChatStreamEndEvent
 from .chat_stream_end_event_finish_reason import ChatStreamEndEventFinishReason
 from .chat_stream_event import ChatStreamEvent
 from .chat_stream_request_citation_quality import ChatStreamRequestCitationQuality
 from .chat_stream_request_connectors_search_options import ChatStreamRequestConnectorsSearchOptions
-from .chat_stream_request_prompt_override import ChatStreamRequestPromptOverride
 from .chat_stream_request_prompt_truncation import ChatStreamRequestPromptTruncation
 from .chat_stream_request_tool_results_item import ChatStreamRequestToolResultsItem
 from .chat_stream_start_event import ChatStreamStartEvent
 from .chat_text_generation_event import ChatTextGenerationEvent
 from .chat_tool_calls_generation_event import ChatToolCallsGenerationEvent
 from .classify_data_metrics import ClassifyDataMetrics
 from .classify_example import ClassifyExample
@@ -132,28 +130,26 @@
     "ChatConnector",
     "ChatDataMetrics",
     "ChatDocument",
     "ChatMessage",
     "ChatMessageRole",
     "ChatRequestCitationQuality",
     "ChatRequestConnectorsSearchOptions",
-    "ChatRequestPromptOverride",
     "ChatRequestPromptTruncation",
     "ChatRequestToolResultsItem",
     "ChatSearchQueriesGenerationEvent",
     "ChatSearchQuery",
     "ChatSearchResult",
     "ChatSearchResultConnector",
     "ChatSearchResultsEvent",
     "ChatStreamEndEvent",
     "ChatStreamEndEventFinishReason",
     "ChatStreamEvent",
     "ChatStreamRequestCitationQuality",
     "ChatStreamRequestConnectorsSearchOptions",
-    "ChatStreamRequestPromptOverride",
     "ChatStreamRequestPromptTruncation",
     "ChatStreamRequestToolResultsItem",
     "ChatStreamStartEvent",
     "ChatTextGenerationEvent",
     "ChatToolCallsGenerationEvent",
     "ClassifyDataMetrics",
     "ClassifyExample",
```

### Comparing `cohere-5.1.7/src/cohere/types/api_meta.py` & `cohere-5.2.0/src/cohere/types/api_meta.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/api_meta_api_version.py` & `cohere-5.2.0/src/cohere/types/api_meta_api_version.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/api_meta_billed_units.py` & `cohere-5.2.0/src/cohere/types/api_meta_billed_units.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/chat_citation.py` & `cohere-5.2.0/src/cohere/types/chat_citation.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/chat_citation_generation_event.py` & `cohere-5.2.0/src/cohere/types/chat_citation_generation_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/chat_connector.py` & `cohere-5.2.0/src/cohere/types/chat_connector.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/chat_data_metrics.py` & `cohere-5.2.0/src/cohere/types/chat_data_metrics.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/chat_message.py` & `cohere-5.2.0/src/cohere/types/chat_message.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/chat_request_connectors_search_options.py` & `cohere-5.2.0/src/cohere/types/chat_request_connectors_search_options.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/chat_request_prompt_override.py` & `cohere-5.2.0/src/cohere/types/parse_info.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,22 +7,17 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class ChatRequestPromptOverride(pydantic.BaseModel):
-    """
-    (internal) Overrides specified parts of the default Chat or RAG preamble. It is recommended that these options only be used in specific scenarios where the defaults are not adequate.
-    """
-
-    preamble: typing.Optional[typing.Any] = None
-    task_description: typing.Optional[typing.Any] = None
-    style_guide: typing.Optional[typing.Any] = None
+class ParseInfo(pydantic.BaseModel):
+    separator: typing.Optional[str] = None
+    delimiter: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `cohere-5.1.7/src/cohere/types/chat_request_tool_results_item.py` & `cohere-5.2.0/src/cohere/types/chat_request_tool_results_item.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/chat_search_queries_generation_event.py` & `cohere-5.2.0/src/cohere/types/chat_search_queries_generation_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/chat_search_query.py` & `cohere-5.2.0/src/cohere/types/chat_search_query.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/chat_search_result.py` & `cohere-5.2.0/src/cohere/types/chat_search_result.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/chat_search_result_connector.py` & `cohere-5.2.0/src/cohere/types/chat_search_result_connector.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/chat_search_results_event.py` & `cohere-5.2.0/src/cohere/types/chat_search_results_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/chat_stream_end_event.py` & `cohere-5.2.0/src/cohere/types/chat_stream_end_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/chat_stream_event.py` & `cohere-5.2.0/src/cohere/types/chat_stream_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/chat_stream_request_connectors_search_options.py` & `cohere-5.2.0/src/cohere/types/chat_stream_request_connectors_search_options.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/chat_stream_request_prompt_override.py` & `cohere-5.2.0/src/cohere/types/tokenize_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from .api_meta import ApiMeta
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class ChatStreamRequestPromptOverride(pydantic.BaseModel):
+class TokenizeResponse(pydantic.BaseModel):
+    tokens: typing.List[int] = pydantic.Field()
     """
-    (internal) Overrides specified parts of the default Chat or RAG preamble. It is recommended that these options only be used in specific scenarios where the defaults are not adequate.
+    An array of tokens, where each token is an integer.
     """
 
-    preamble: typing.Optional[typing.Any] = None
-    task_description: typing.Optional[typing.Any] = None
-    style_guide: typing.Optional[typing.Any] = None
+    token_strings: typing.List[str]
+    meta: typing.Optional[ApiMeta] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `cohere-5.1.7/src/cohere/types/chat_stream_request_tool_results_item.py` & `cohere-5.2.0/src/cohere/types/chat_stream_request_tool_results_item.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/chat_stream_start_event.py` & `cohere-5.2.0/src/cohere/types/chat_stream_start_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/chat_text_generation_event.py` & `cohere-5.2.0/src/cohere/types/chat_text_generation_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/chat_tool_calls_generation_event.py` & `cohere-5.2.0/src/cohere/types/chat_tool_calls_generation_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/classify_data_metrics.py` & `cohere-5.2.0/src/cohere/types/classify_data_metrics.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/classify_example.py` & `cohere-5.2.0/src/cohere/types/classify_example.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/classify_response.py` & `cohere-5.2.0/src/cohere/types/classify_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/classify_response_classifications_item.py` & `cohere-5.2.0/src/cohere/types/classify_response_classifications_item.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/classify_response_classifications_item_labels_value.py` & `cohere-5.2.0/src/cohere/types/classify_response_classifications_item_labels_value.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/connector.py` & `cohere-5.2.0/src/cohere/types/connector.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/connector_o_auth.py` & `cohere-5.2.0/src/cohere/types/connector_o_auth.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/create_connector_o_auth.py` & `cohere-5.2.0/src/cohere/types/create_connector_o_auth.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/create_connector_response.py` & `cohere-5.2.0/src/cohere/types/create_connector_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/create_connector_service_auth.py` & `cohere-5.2.0/src/cohere/types/create_connector_service_auth.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/create_embed_job_response.py` & `cohere-5.2.0/src/cohere/types/create_embed_job_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/dataset.py` & `cohere-5.2.0/src/cohere/types/dataset.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/dataset_part.py` & `cohere-5.2.0/src/cohere/types/dataset_part.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/detokenize_response.py` & `cohere-5.2.0/src/cohere/types/detokenize_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/embed_by_type_response.py` & `cohere-5.2.0/src/cohere/types/embed_by_type_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/embed_by_type_response_embeddings.py` & `cohere-5.2.0/src/cohere/types/embed_by_type_response_embeddings.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/embed_floats_response.py` & `cohere-5.2.0/src/cohere/types/embed_floats_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/embed_job.py` & `cohere-5.2.0/src/cohere/types/embed_job.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/embed_response.py` & `cohere-5.2.0/src/cohere/types/embed_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/finetune_dataset_metrics.py` & `cohere-5.2.0/src/cohere/types/finetune_dataset_metrics.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/generate_stream_end.py` & `cohere-5.2.0/src/cohere/types/generate_stream_end.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/generate_stream_end_response.py` & `cohere-5.2.0/src/cohere/types/generate_stream_end_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/generate_stream_error.py` & `cohere-5.2.0/src/cohere/types/generate_stream_error.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/generate_stream_event.py` & `cohere-5.2.0/src/cohere/types/generate_stream_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/generate_stream_text.py` & `cohere-5.2.0/src/cohere/types/generate_stream_text.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/generate_streamed_response.py` & `cohere-5.2.0/src/cohere/types/generate_streamed_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/generation.py` & `cohere-5.2.0/src/cohere/types/generation.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/get_connector_response.py` & `cohere-5.2.0/src/cohere/types/get_connector_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/get_model_response.py` & `cohere-5.2.0/src/cohere/types/get_model_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/label_metric.py` & `cohere-5.2.0/src/cohere/types/label_metric.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/list_connectors_response.py` & `cohere-5.2.0/src/cohere/types/list_connectors_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/list_embed_job_response.py` & `cohere-5.2.0/src/cohere/types/list_embed_job_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/list_models_response.py` & `cohere-5.2.0/src/cohere/types/list_models_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/metrics.py` & `cohere-5.2.0/src/cohere/types/metrics.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/non_streamed_chat_response.py` & `cohere-5.2.0/src/cohere/types/non_streamed_chat_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/o_auth_authorize_response.py` & `cohere-5.2.0/src/cohere/types/o_auth_authorize_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/parse_info.py` & `cohere-5.2.0/src/cohere/types/single_generation_token_likelihoods_item.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class ParseInfo(pydantic.BaseModel):
-    separator: typing.Optional[str] = None
-    delimiter: typing.Optional[str] = None
+class SingleGenerationTokenLikelihoodsItem(pydantic.BaseModel):
+    token: str
+    likelihood: float
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `cohere-5.1.7/src/cohere/types/rerank_request_documents_item_text.py` & `cohere-5.2.0/src/cohere/types/rerank_request_documents_item_text.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/rerank_response.py` & `cohere-5.2.0/src/cohere/types/rerank_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/rerank_response_results_item.py` & `cohere-5.2.0/src/cohere/types/rerank_response_results_item.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/rerank_response_results_item_document.py` & `cohere-5.2.0/src/cohere/types/rerank_response_results_item_document.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/reranker_data_metrics.py` & `cohere-5.2.0/src/cohere/types/reranker_data_metrics.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/single_generation.py` & `cohere-5.2.0/src/cohere/types/single_generation.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/single_generation_in_stream.py` & `cohere-5.2.0/src/cohere/types/single_generation_in_stream.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/single_generation_token_likelihoods_item.py` & `cohere-5.2.0/src/cohere/types/summarize_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from .api_meta import ApiMeta
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class SingleGenerationTokenLikelihoodsItem(pydantic.BaseModel):
-    token: str
-    likelihood: float
+class SummarizeResponse(pydantic.BaseModel):
+    id: typing.Optional[str] = pydantic.Field(default=None)
+    """
+    Generated ID for the summary
+    """
+
+    summary: typing.Optional[str] = pydantic.Field(default=None)
+    """
+    Generated summary for the text
+    """
+
+    meta: typing.Optional[ApiMeta] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `cohere-5.1.7/src/cohere/types/streamed_chat_response.py` & `cohere-5.2.0/src/cohere/types/streamed_chat_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/summarize_response.py` & `cohere-5.2.0/src/cohere/types/tool_call.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .api_meta import ApiMeta
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class SummarizeResponse(pydantic.BaseModel):
-    id: typing.Optional[str] = pydantic.Field(default=None)
+class ToolCall(pydantic.BaseModel):
     """
-    Generated ID for the summary
+    Contains the tool calls generated by the model. Use it to invoke your tools.
     """
 
-    summary: typing.Optional[str] = pydantic.Field(default=None)
+    name: str = pydantic.Field()
     """
-    Generated summary for the text
+    Name of the tool to call.
     """
 
-    meta: typing.Optional[ApiMeta] = None
+    parameters: typing.Dict[str, typing.Any] = pydantic.Field()
+    """
+    The name and value of the parameters to use when invoking a tool.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `cohere-5.1.7/src/cohere/types/tokenize_response.py` & `cohere-5.2.0/src/cohere/types/tool_parameter_definitions_value.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .api_meta import ApiMeta
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class TokenizeResponse(pydantic.BaseModel):
-    tokens: typing.List[int] = pydantic.Field()
+class ToolParameterDefinitionsValue(pydantic.BaseModel):
+    description: typing.Optional[str] = pydantic.Field(default=None)
     """
-    An array of tokens, where each token is an integer.
+    The description of the parameter.
     """
 
-    token_strings: typing.List[str]
-    meta: typing.Optional[ApiMeta] = None
+    type: str = pydantic.Field()
+    """
+    The type of the parameter. Must be a valid Python type.
+    """
+
+    required: typing.Optional[bool] = pydantic.Field(default=None)
+    """
+    Denotes whether the parameter is always present (required) or not. Defaults to not required.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `cohere-5.1.7/src/cohere/types/tool.py` & `cohere-5.2.0/src/cohere/types/tool.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/src/cohere/types/tool_call.py` & `cohere-5.2.0/src/cohere/types/update_connector_response.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from .connector import Connector
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class ToolCall(pydantic.BaseModel):
-    """
-    Contains the tool calls generated by the model. Use it to invoke your tools.
-    """
-
-    name: str = pydantic.Field()
-    """
-    Name of the tool to call.
-    """
-
-    parameters: typing.Dict[str, typing.Any] = pydantic.Field()
-    """
-    The name and value of the parameters to use when invoking a tool.
-    """
+class UpdateConnectorResponse(pydantic.BaseModel):
+    connector: Connector
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `cohere-5.1.7/src/cohere/utils.py` & `cohere-5.2.0/src/cohere/utils.py`

 * *Files identical despite different names*

### Comparing `cohere-5.1.7/PKG-INFO` & `cohere-5.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: cohere
-Version: 5.1.7
+Version: 5.2.0
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fastavro (>=1.9.4,<2.0.0)
 Requires-Dist: httpx (>=0.21.2)
 Requires-Dist: pydantic (>=1.9.2)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: tokenizers (>=0.15.2,<0.16.0)
 Requires-Dist: types-requests (>=2.31.0.20240311,<3.0.0.0)
 Requires-Dist: typing_extensions (>=4.0.0)
 Description-Content-Type: text/markdown
 
 # Cohere Python SDK
 
 ![](banner.png)
```

