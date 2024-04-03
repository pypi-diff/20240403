# Comparing `tmp/llamaindex_py_client-0.1.8.tar.gz` & `tmp/llamaindex_py_client-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llamaindex_py_client-0.1.8.tar", max compression
+gzip compressed data, was "llamaindex_py_client-0.1.9.tar", max compression
```

## Comparing `llamaindex_py_client-0.1.8.tar` & `llamaindex_py_client-0.1.9.tar`

### file list

```diff
@@ -1,155 +1,151 @@
--rw-r--r--   0        0        0     1067 2023-12-08 18:00:31.725552 llamaindex_py_client-0.1.8/LICENSE
--rw-r--r--   0        0        0      195 2023-12-08 18:00:31.725809 llamaindex_py_client-0.1.8/README.md
--rw-r--r--   0        0        0     7057 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/__init__.py
--rw-r--r--   0        0        0     3310 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/client.py
--rw-r--r--   0        0        0      519 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/core/__init__.py
--rw-r--r--   0        0        0      426 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/core/api_error.py
--rw-r--r--   0        0        0     1507 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/core/datetime_utils.py
--rw-r--r--   0        0        0     3799 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      170 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/errors/__init__.py
--rw-r--r--   0        0        0      313 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0      635 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/resources/__init__.py
--rw-r--r--   0        0        0       65 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/resources/api_key/__init__.py
--rw-r--r--   0        0        0    10596 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/resources/api_key/client.py
--rw-r--r--   0        0        0       65 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/resources/component_definition/__init__.py
--rw-r--r--   0        0        0     7861 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/resources/component_definition/client.py
--rw-r--r--   0        0        0      205 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/resources/data_sink/__init__.py
--rw-r--r--   0        0        0    13391 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/resources/data_sink/client.py
--rw-r--r--   0        0        0      269 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/resources/data_sink/types/__init__.py
--rw-r--r--   0        0        0      249 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/resources/data_sink/types/data_sink_update_component.py
--rw-r--r--   0        0        0      524 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/resources/data_sink/types/data_sink_update_component_one.py
--rw-r--r--   0        0        0      213 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/resources/data_source/__init__.py
--rw-r--r--   0        0        0    29074 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/resources/data_source/client.py
--rw-r--r--   0        0        0      281 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/resources/data_source/types/__init__.py
--rw-r--r--   0        0        0      366 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/resources/data_source/types/data_source_update_component.py
--rw-r--r--   0        0        0     1444 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/resources/data_source/types/data_source_update_component_one.py
--rw-r--r--   0        0        0       65 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/resources/eval/__init__.py
--rw-r--r--   0        0        0    24661 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/resources/eval/client.py
--rw-r--r--   0        0        0       65 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/resources/health/__init__.py
--rw-r--r--   0        0        0     2632 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/resources/health/client.py
--rw-r--r--   0        0        0       65 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/resources/pipeline/__init__.py
--rw-r--r--   0        0        0    77987 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/resources/pipeline/client.py
--rw-r--r--   0        0        0       65 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/resources/project/__init__.py
--rw-r--r--   0        0        0    22380 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/resources/project/client.py
--rw-r--r--   0        0        0       65 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/resources/retrieval/__init__.py
--rw-r--r--   0        0        0     7446 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/resources/retrieval/client.py
--rw-r--r--   0        0        0    10066 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/__init__.py
--rw-r--r--   0        0        0     1217 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/api_key.py
--rw-r--r--   0        0        0     3028 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/azure_open_ai_embedding.py
--rw-r--r--   0        0        0     1484 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/base_prompt_template.py
--rw-r--r--   0        0        0     1103 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/base_pydantic_reader.py
--rw-r--r--   0        0        0     1298 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/beautiful_soup_web_reader.py
--rw-r--r--   0        0        0     1627 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/chroma_vector_store.py
--rw-r--r--   0        0        0     1879 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/code_splitter.py
--rw-r--r--   0        0        0     1047 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/configurable_data_sink_names.py
--rw-r--r--   0        0        0     3303 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/configurable_data_source_names.py
--rw-r--r--   0        0        0     1794 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/configurable_transformation_definition.py
--rw-r--r--   0        0        0     3402 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/configurable_transformation_names.py
--rw-r--r--   0        0        0     2159 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/configured_transformation_execution.py
--rw-r--r--   0        0        0      602 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/configured_transformation_execution_run_config_per_op_value.py
--rw-r--r--   0        0        0     1734 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/configured_transformation_item.py
--rw-r--r--   0        0        0      311 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/configured_transformation_item_component.py
--rw-r--r--   0        0        0     1211 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/configured_transformation_item_component_one.py
--rw-r--r--   0        0        0     1412 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/data_sink.py
--rw-r--r--   0        0        0      224 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/data_sink_component.py
--rw-r--r--   0        0        0      473 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/data_sink_component_one.py
--rw-r--r--   0        0        0     1196 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/data_sink_create.py
--rw-r--r--   0        0        0      249 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/data_sink_create_component.py
--rw-r--r--   0        0        0      479 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/data_sink_create_component_one.py
--rw-r--r--   0        0        0     1469 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/data_sink_definition.py
--rw-r--r--   0        0        0     1432 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/data_source.py
--rw-r--r--   0        0        0      326 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/data_source_component.py
--rw-r--r--   0        0        0     1285 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/data_source_component_one.py
--rw-r--r--   0        0        0     1216 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/data_source_create.py
--rw-r--r--   0        0        0      357 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/data_source_create_component.py
--rw-r--r--   0        0        0     1291 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/data_source_create_component_one.py
--rw-r--r--   0        0        0     1483 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/data_source_definition.py
--rw-r--r--   0        0        0     1906 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/data_source_load_execution.py
--rw-r--r--   0        0        0      592 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/data_source_load_execution_run_config_per_op_value.py
--rw-r--r--   0        0        0     2117 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/data_source_managed_ingestion_execution.py
--rw-r--r--   0        0        0      604 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/data_source_managed_ingestion_execution_run_config_per_op_value.py
--rw-r--r--   0        0        0     1171 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/discord_reader.py
--rw-r--r--   0        0        0     2795 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/document.py
--rw-r--r--   0        0        0     1405 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/document_group.py
--rw-r--r--   0        0        0      217 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/document_relationships_value.py
--rw-r--r--   0        0        0     1386 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/elasticsearch_reader.py
--rw-r--r--   0        0        0     1648 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/etl_job_names.py
--rw-r--r--   0        0        0     1316 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/eval_dataset.py
--rw-r--r--   0        0        0     2217 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/eval_dataset_execution.py
--rw-r--r--   0        0        0     1197 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/eval_dataset_execution_config.py
--rw-r--r--   0        0        0      589 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/eval_dataset_execution_run_config_per_op_value.py
--rw-r--r--   0        0        0     1236 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/eval_execution_params.py
--rw-r--r--   0        0        0     1070 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/eval_llm_model_data.py
--rw-r--r--   0        0        0     1512 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/eval_question.py
--rw-r--r--   0        0        0      939 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/eval_question_create.py
--rw-r--r--   0        0        0     2082 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/eval_question_result.py
--rw-r--r--   0        0        0     1286 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/externally_stored_component.py
--rw-r--r--   0        0        0     1009 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/google_docs_reader.py
--rw-r--r--   0        0        0     1023 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/google_sheets_reader.py
--rw-r--r--   0        0        0     1593 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/html_node_parser.py
--rw-r--r--   0        0        0      966 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/http_validation_error.py
--rw-r--r--   0        0        0     4536 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/hugging_face_inference_api_embedding.py
--rw-r--r--   0        0        0     1485 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/json_node_parser.py
--rw-r--r--   0        0        0     2185 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/keyword_extractor.py
--rw-r--r--   0        0        0      196 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/keyword_extractor_llm.py
--rw-r--r--   0        0        0     1586 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/llm.py
--rw-r--r--   0        0        0     1553 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/llm_predictor.py
--rw-r--r--   0        0        0     1487 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/loaded_file.py
--rw-r--r--   0        0        0     2095 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/loaded_file_managed_ingestion_execution.py
--rw-r--r--   0        0        0      604 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/loaded_file_managed_ingestion_execution_run_config_per_op_value.py
--rw-r--r--   0        0        0     1097 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/loaded_file_payload.py
--rw-r--r--   0        0        0     1163 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/managed_data_source_ingestion_job_config.py
--rw-r--r--   0        0        0     1058 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/managed_pipeline_ingestion_job_config.py
--rw-r--r--   0        0        0     1497 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/markdown_node_parser.py
--rw-r--r--   0        0        0      757 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/metadata_mode.py
--rw-r--r--   0        0        0     1145 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/metric_result.py
--rw-r--r--   0        0        0     1136 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/notion_page_reader.py
--rw-r--r--   0        0        0      736 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/object_type.py
--rw-r--r--   0        0        0     2807 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/open_ai_embedding.py
--rw-r--r--   0        0        0     1323 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/pg_vector_store.py
--rw-r--r--   0        0        0     2171 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/pinecone_vector_store.py
--rw-r--r--   0        0        0     2041 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/pipeline.py
--rw-r--r--   0        0        0     2645 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/pipeline_create.py
--rw-r--r--   0        0        0     1994 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/pipeline_managed_ingestion_execution.py
--rw-r--r--   0        0        0      602 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/pipeline_managed_ingestion_execution_run_config_per_op_value.py
--rw-r--r--   0        0        0      551 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/pipeline_type.py
--rw-r--r--   0        0        0      498 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/pooling.py
--rw-r--r--   0        0        0     1913 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/preset_retrieval_params.py
--rw-r--r--   0        0        0     1274 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/project.py
--rw-r--r--   0        0        0      922 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/project_create.py
--rw-r--r--   0        0        0     1048 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/pydantic_program_mode.py
--rw-r--r--   0        0        0     1625 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/qdrant_vector_store.py
--rw-r--r--   0        0        0     2634 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/questions_answered_extractor.py
--rw-r--r--   0        0        0      206 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/questions_answered_extractor_llm.py
--rw-r--r--   0        0        0     1305 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/reader_config.py
--rw-r--r--   0        0        0     1149 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/related_node_info.py
--rw-r--r--   0        0        0     1385 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/retrieve_results.py
--rw-r--r--   0        0        0     1019 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/rss_reader.py
--rw-r--r--   0        0        0     1437 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/run_transform_asset_config.py
--rw-r--r--   0        0        0     2121 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/sentence_splitter.py
--rw-r--r--   0        0        0     1584 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/simple_file_node_parser.py
--rw-r--r--   0        0        0     1283 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/simple_web_page_reader.py
--rw-r--r--   0        0        0     1846 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/slack_reader.py
--rw-r--r--   0        0        0      833 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/status_enum.py
--rw-r--r--   0        0        0     2480 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/summary_extractor.py
--rw-r--r--   0        0        0      196 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/summary_extractor_llm.py
--rw-r--r--   0        0        0     1272 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/supported_eval_llm_model.py
--rw-r--r--   0        0        0      776 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/supported_eval_llm_model_names.py
--rw-r--r--   0        0        0     2839 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/text_node.py
--rw-r--r--   0        0        0      217 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/text_node_relationships_value.py
--rw-r--r--   0        0        0     1137 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/text_node_with_score.py
--rw-r--r--   0        0        0     2611 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/title_extractor.py
--rw-r--r--   0        0        0      194 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/title_extractor_llm.py
--rw-r--r--   0        0        0     1791 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/token_text_splitter.py
--rw-r--r--   0        0        0     1085 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/trafilatura_web_reader.py
--rw-r--r--   0        0        0      825 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/transformation_category_names.py
--rw-r--r--   0        0        0     1411 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/twitter_tweet_reader.py
--rw-r--r--   0        0        0      992 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     1578 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/weaviate_vector_store.py
--rw-r--r--   0        0        0      990 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/wikipedia_reader.py
--rw-r--r--   0        0        0     1044 2024-01-19 01:08:04.000000 llamaindex_py_client-0.1.8/llama_index_client/types/youtube_transcript_reader.py
--rw-r--r--   0        0        0      375 2024-01-18 19:08:39.424090 llamaindex_py_client-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 llamaindex_py_client-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-12-08 18:00:31.725552 llamaindex_py_client-0.1.9/LICENSE
+-rw-r--r--   0        0        0      195 2023-12-08 18:00:31.725809 llamaindex_py_client-0.1.9/README.md
+-rw-r--r--   0        0        0     6259 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/__init__.py
+-rw-r--r--   0        0        0     3535 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/client.py
+-rw-r--r--   0        0        0      519 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/core/api_error.py
+-rw-r--r--   0        0        0     1507 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/core/datetime_utils.py
+-rw-r--r--   0        0        0     3799 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      170 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/errors/__init__.py
+-rw-r--r--   0        0        0      313 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0      659 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/resources/__init__.py
+-rw-r--r--   0        0        0       65 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/resources/api_key/__init__.py
+-rw-r--r--   0        0        0    10596 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/resources/api_key/client.py
+-rw-r--r--   0        0        0       65 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/resources/component_definition/__init__.py
+-rw-r--r--   0        0        0     7861 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/resources/component_definition/client.py
+-rw-r--r--   0        0        0      205 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/resources/data_sink/__init__.py
+-rw-r--r--   0        0        0    13391 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/resources/data_sink/client.py
+-rw-r--r--   0        0        0      269 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/resources/data_sink/types/__init__.py
+-rw-r--r--   0        0        0      249 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/resources/data_sink/types/data_sink_update_component.py
+-rw-r--r--   0        0        0      524 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/resources/data_sink/types/data_sink_update_component_one.py
+-rw-r--r--   0        0        0      213 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/resources/data_source/__init__.py
+-rw-r--r--   0        0        0    30459 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/resources/data_source/client.py
+-rw-r--r--   0        0        0      281 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/resources/data_source/types/__init__.py
+-rw-r--r--   0        0        0      366 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/resources/data_source/types/data_source_update_component.py
+-rw-r--r--   0        0        0     1444 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/resources/data_source/types/data_source_update_component_one.py
+-rw-r--r--   0        0        0       65 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/resources/eval/__init__.py
+-rw-r--r--   0        0        0    24661 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/resources/eval/client.py
+-rw-r--r--   0        0        0       65 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/resources/health/__init__.py
+-rw-r--r--   0        0        0     2632 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/resources/health/client.py
+-rw-r--r--   0        0        0       65 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/resources/parsing/__init__.py
+-rw-r--r--   0        0        0     8046 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/resources/parsing/client.py
+-rw-r--r--   0        0        0       65 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/resources/pipeline/__init__.py
+-rw-r--r--   0        0        0    71981 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/resources/pipeline/client.py
+-rw-r--r--   0        0        0       65 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/resources/project/__init__.py
+-rw-r--r--   0        0        0    22380 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/resources/project/client.py
+-rw-r--r--   0        0        0       65 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/resources/retrieval/__init__.py
+-rw-r--r--   0        0        0     7446 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/resources/retrieval/client.py
+-rw-r--r--   0        0        0     8725 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/__init__.py
+-rw-r--r--   0        0        0     1217 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/api_key.py
+-rw-r--r--   0        0        0     3028 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/azure_open_ai_embedding.py
+-rw-r--r--   0        0        0     1484 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/base_prompt_template.py
+-rw-r--r--   0        0        0     1103 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/base_pydantic_reader.py
+-rw-r--r--   0        0        0     1298 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/beautiful_soup_web_reader.py
+-rw-r--r--   0        0        0     1627 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/chroma_vector_store.py
+-rw-r--r--   0        0        0     1879 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/code_splitter.py
+-rw-r--r--   0        0        0     1047 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/configurable_data_sink_names.py
+-rw-r--r--   0        0        0     3303 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/configurable_data_source_names.py
+-rw-r--r--   0        0        0     1794 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/configurable_transformation_definition.py
+-rw-r--r--   0        0        0     3402 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/configurable_transformation_names.py
+-rw-r--r--   0        0        0     1734 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/configured_transformation_item.py
+-rw-r--r--   0        0        0      311 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/configured_transformation_item_component.py
+-rw-r--r--   0        0        0     1211 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/configured_transformation_item_component_one.py
+-rw-r--r--   0        0        0     1412 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/data_sink.py
+-rw-r--r--   0        0        0      224 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/data_sink_component.py
+-rw-r--r--   0        0        0      473 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/data_sink_component_one.py
+-rw-r--r--   0        0        0     1196 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/data_sink_create.py
+-rw-r--r--   0        0        0      249 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/data_sink_create_component.py
+-rw-r--r--   0        0        0      479 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/data_sink_create_component_one.py
+-rw-r--r--   0        0        0     1469 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/data_sink_definition.py
+-rw-r--r--   0        0        0     1432 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/data_source.py
+-rw-r--r--   0        0        0      326 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/data_source_component.py
+-rw-r--r--   0        0        0     1285 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/data_source_component_one.py
+-rw-r--r--   0        0        0     1216 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/data_source_create.py
+-rw-r--r--   0        0        0      357 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/data_source_create_component.py
+-rw-r--r--   0        0        0     1291 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/data_source_create_component_one.py
+-rw-r--r--   0        0        0     1483 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/data_source_definition.py
+-rw-r--r--   0        0        0     1524 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/data_source_load_job_record.py
+-rw-r--r--   0        0        0     1577 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/data_source_managed_ingestion_job_record.py
+-rw-r--r--   0        0        0     1171 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/discord_reader.py
+-rw-r--r--   0        0        0     2795 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/document.py
+-rw-r--r--   0        0        0     1405 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/document_group.py
+-rw-r--r--   0        0        0      217 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/document_relationships_value.py
+-rw-r--r--   0        0        0     1386 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/elasticsearch_reader.py
+-rw-r--r--   0        0        0     1316 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/eval_dataset.py
+-rw-r--r--   0        0        0     1840 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/eval_dataset_job_record.py
+-rw-r--r--   0        0        0     1263 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/eval_execution_params.py
+-rw-r--r--   0        0        0     1070 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/eval_llm_model_data.py
+-rw-r--r--   0        0        0     1512 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/eval_question.py
+-rw-r--r--   0        0        0      939 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/eval_question_create.py
+-rw-r--r--   0        0        0     2076 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/eval_question_result.py
+-rw-r--r--   0        0        0     1286 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/externally_stored_component.py
+-rw-r--r--   0        0        0     1009 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/google_docs_reader.py
+-rw-r--r--   0        0        0     1023 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/google_sheets_reader.py
+-rw-r--r--   0        0        0     1593 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/html_node_parser.py
+-rw-r--r--   0        0        0      966 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/http_validation_error.py
+-rw-r--r--   0        0        0     4536 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/hugging_face_inference_api_embedding.py
+-rw-r--r--   0        0        0     1612 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/job_names.py
+-rw-r--r--   0        0        0     1485 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/json_node_parser.py
+-rw-r--r--   0        0        0     2185 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/keyword_extractor.py
+-rw-r--r--   0        0        0      196 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/keyword_extractor_llm.py
+-rw-r--r--   0        0        0     1586 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/llm.py
+-rw-r--r--   0        0        0     1553 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/llm_predictor.py
+-rw-r--r--   0        0        0     1487 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/loaded_file.py
+-rw-r--r--   0        0        0     1097 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/loaded_file_payload.py
+-rw-r--r--   0        0        0     1072 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/managed_ingestion_status.py
+-rw-r--r--   0        0        0     1497 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/markdown_node_parser.py
+-rw-r--r--   0        0        0      757 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/metadata_mode.py
+-rw-r--r--   0        0        0     1145 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/metric_result.py
+-rw-r--r--   0        0        0     1136 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/notion_page_reader.py
+-rw-r--r--   0        0        0      736 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/object_type.py
+-rw-r--r--   0        0        0     2807 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/open_ai_embedding.py
+-rw-r--r--   0        0        0    10840 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/parser_languages.py
+-rw-r--r--   0        0        0      924 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/parsing_job.py
+-rw-r--r--   0        0        0      956 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/parsing_job_markdown_result.py
+-rw-r--r--   0        0        0      944 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/parsing_job_text_result.py
+-rw-r--r--   0        0        0     1323 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/pg_vector_store.py
+-rw-r--r--   0        0        0     2171 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/pinecone_vector_store.py
+-rw-r--r--   0        0        0     2247 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/pipeline.py
+-rw-r--r--   0        0        0     2645 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/pipeline_create.py
+-rw-r--r--   0        0        0     1571 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/pipeline_managed_ingestion_job_record.py
+-rw-r--r--   0        0        0      551 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/pipeline_type.py
+-rw-r--r--   0        0        0     1668 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/playground_job_record.py
+-rw-r--r--   0        0        0      498 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/pooling.py
+-rw-r--r--   0        0        0     1913 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/preset_retrieval_params.py
+-rw-r--r--   0        0        0     1274 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/project.py
+-rw-r--r--   0        0        0      922 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/project_create.py
+-rw-r--r--   0        0        0     1048 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/pydantic_program_mode.py
+-rw-r--r--   0        0        0     1625 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/qdrant_vector_store.py
+-rw-r--r--   0        0        0     2634 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/questions_answered_extractor.py
+-rw-r--r--   0        0        0      206 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/questions_answered_extractor_llm.py
+-rw-r--r--   0        0        0     1305 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/reader_config.py
+-rw-r--r--   0        0        0     1149 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/related_node_info.py
+-rw-r--r--   0        0        0     1385 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/retrieve_results.py
+-rw-r--r--   0        0        0     1019 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/rss_reader.py
+-rw-r--r--   0        0        0     2121 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/sentence_splitter.py
+-rw-r--r--   0        0        0     1584 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/simple_file_node_parser.py
+-rw-r--r--   0        0        0     1283 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/simple_web_page_reader.py
+-rw-r--r--   0        0        0     1846 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/slack_reader.py
+-rw-r--r--   0        0        0      833 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/status_enum.py
+-rw-r--r--   0        0        0     2480 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/summary_extractor.py
+-rw-r--r--   0        0        0      196 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/summary_extractor_llm.py
+-rw-r--r--   0        0        0     1272 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/supported_eval_llm_model.py
+-rw-r--r--   0        0        0      776 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/supported_eval_llm_model_names.py
+-rw-r--r--   0        0        0     2839 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/text_node.py
+-rw-r--r--   0        0        0      217 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/text_node_relationships_value.py
+-rw-r--r--   0        0        0     1137 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/text_node_with_score.py
+-rw-r--r--   0        0        0     2611 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/title_extractor.py
+-rw-r--r--   0        0        0      194 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/title_extractor_llm.py
+-rw-r--r--   0        0        0     1791 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/token_text_splitter.py
+-rw-r--r--   0        0        0     1085 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/trafilatura_web_reader.py
+-rw-r--r--   0        0        0      825 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/transformation_category_names.py
+-rw-r--r--   0        0        0     1411 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/twitter_tweet_reader.py
+-rw-r--r--   0        0        0      992 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     1578 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/weaviate_vector_store.py
+-rw-r--r--   0        0        0      990 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/wikipedia_reader.py
+-rw-r--r--   0        0        0     1044 2024-02-03 06:25:26.000000 llamaindex_py_client-0.1.9/llama_index_client/types/youtube_transcript_reader.py
+-rw-r--r--   0        0        0      375 2024-02-02 22:30:20.662600 llamaindex_py_client-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 llamaindex_py_client-0.1.9/PKG-INFO
```

### Comparing `llamaindex_py_client-0.1.8/LICENSE` & `llamaindex_py_client-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/__init__.py` & `llamaindex_py_client-0.1.9/llama_index_client/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,16 +8,14 @@
     BeautifulSoupWebReader,
     ChromaVectorStore,
     CodeSplitter,
     ConfigurableDataSinkNames,
     ConfigurableDataSourceNames,
     ConfigurableTransformationDefinition,
     ConfigurableTransformationNames,
-    ConfiguredTransformationExecution,
-    ConfiguredTransformationExecutionRunConfigPerOpValue,
     ConfiguredTransformationItem,
     ConfiguredTransformationItemComponent,
     ConfiguredTransformationItemComponentOne,
     DataSink,
     DataSinkComponent,
     DataSinkComponentOne,
     DataSinkCreate,
@@ -27,76 +25,72 @@
     DataSource,
     DataSourceComponent,
     DataSourceComponentOne,
     DataSourceCreate,
     DataSourceCreateComponent,
     DataSourceCreateComponentOne,
     DataSourceDefinition,
-    DataSourceLoadExecution,
-    DataSourceLoadExecutionRunConfigPerOpValue,
-    DataSourceManagedIngestionExecution,
-    DataSourceManagedIngestionExecutionRunConfigPerOpValue,
+    DataSourceLoadJobRecord,
+    DataSourceManagedIngestionJobRecord,
     DiscordReader,
     Document,
     DocumentGroup,
     DocumentRelationshipsValue,
     ElasticsearchReader,
-    EtlJobNames,
     EvalDataset,
-    EvalDatasetExecution,
-    EvalDatasetExecutionConfig,
-    EvalDatasetExecutionRunConfigPerOpValue,
+    EvalDatasetJobRecord,
     EvalExecutionParams,
     EvalLlmModelData,
     EvalQuestion,
     EvalQuestionCreate,
     EvalQuestionResult,
     ExternallyStoredComponent,
     GoogleDocsReader,
     GoogleSheetsReader,
     HtmlNodeParser,
     HttpValidationError,
     HuggingFaceInferenceApiEmbedding,
+    JobNames,
     JsonNodeParser,
     KeywordExtractor,
     KeywordExtractorLlm,
     Llm,
     LlmPredictor,
     LoadedFile,
-    LoadedFileManagedIngestionExecution,
-    LoadedFileManagedIngestionExecutionRunConfigPerOpValue,
     LoadedFilePayload,
-    ManagedDataSourceIngestionJobConfig,
-    ManagedPipelineIngestionJobConfig,
+    ManagedIngestionStatus,
     MarkdownNodeParser,
     MetadataMode,
     MetricResult,
     NotionPageReader,
     ObjectType,
     OpenAiEmbedding,
+    ParserLanguages,
+    ParsingJob,
+    ParsingJobMarkdownResult,
+    ParsingJobTextResult,
     PgVectorStore,
     PineconeVectorStore,
     Pipeline,
     PipelineCreate,
-    PipelineManagedIngestionExecution,
-    PipelineManagedIngestionExecutionRunConfigPerOpValue,
+    PipelineManagedIngestionJobRecord,
     PipelineType,
+    PlaygroundJobRecord,
     Pooling,
     PresetRetrievalParams,
     Project,
     ProjectCreate,
     PydanticProgramMode,
     QdrantVectorStore,
     QuestionsAnsweredExtractor,
     QuestionsAnsweredExtractorLlm,
     ReaderConfig,
     RelatedNodeInfo,
     RetrieveResults,
     RssReader,
-    RunTransformAssetConfig,
     SentenceSplitter,
     SimpleFileNodeParser,
     SimpleWebPageReader,
     SlackReader,
     StatusEnum,
     SummaryExtractor,
     SummaryExtractorLlm,
@@ -125,14 +119,15 @@
     DataSourceUpdateComponentOne,
     api_key,
     component_definition,
     data_sink,
     data_source,
     eval,
     health,
+    parsing,
     pipeline,
     project,
     retrieval,
 )
 
 __all__ = [
     "ApiKey",
@@ -142,16 +137,14 @@
     "BeautifulSoupWebReader",
     "ChromaVectorStore",
     "CodeSplitter",
     "ConfigurableDataSinkNames",
     "ConfigurableDataSourceNames",
     "ConfigurableTransformationDefinition",
     "ConfigurableTransformationNames",
-    "ConfiguredTransformationExecution",
-    "ConfiguredTransformationExecutionRunConfigPerOpValue",
     "ConfiguredTransformationItem",
     "ConfiguredTransformationItemComponent",
     "ConfiguredTransformationItemComponentOne",
     "DataSink",
     "DataSinkComponent",
     "DataSinkComponentOne",
     "DataSinkCreate",
@@ -163,78 +156,74 @@
     "DataSource",
     "DataSourceComponent",
     "DataSourceComponentOne",
     "DataSourceCreate",
     "DataSourceCreateComponent",
     "DataSourceCreateComponentOne",
     "DataSourceDefinition",
-    "DataSourceLoadExecution",
-    "DataSourceLoadExecutionRunConfigPerOpValue",
-    "DataSourceManagedIngestionExecution",
-    "DataSourceManagedIngestionExecutionRunConfigPerOpValue",
+    "DataSourceLoadJobRecord",
+    "DataSourceManagedIngestionJobRecord",
     "DataSourceUpdateComponent",
     "DataSourceUpdateComponentOne",
     "DiscordReader",
     "Document",
     "DocumentGroup",
     "DocumentRelationshipsValue",
     "ElasticsearchReader",
-    "EtlJobNames",
     "EvalDataset",
-    "EvalDatasetExecution",
-    "EvalDatasetExecutionConfig",
-    "EvalDatasetExecutionRunConfigPerOpValue",
+    "EvalDatasetJobRecord",
     "EvalExecutionParams",
     "EvalLlmModelData",
     "EvalQuestion",
     "EvalQuestionCreate",
     "EvalQuestionResult",
     "ExternallyStoredComponent",
     "GoogleDocsReader",
     "GoogleSheetsReader",
     "HtmlNodeParser",
     "HttpValidationError",
     "HuggingFaceInferenceApiEmbedding",
+    "JobNames",
     "JsonNodeParser",
     "KeywordExtractor",
     "KeywordExtractorLlm",
     "Llm",
     "LlmPredictor",
     "LoadedFile",
-    "LoadedFileManagedIngestionExecution",
-    "LoadedFileManagedIngestionExecutionRunConfigPerOpValue",
     "LoadedFilePayload",
-    "ManagedDataSourceIngestionJobConfig",
-    "ManagedPipelineIngestionJobConfig",
+    "ManagedIngestionStatus",
     "MarkdownNodeParser",
     "MetadataMode",
     "MetricResult",
     "NotionPageReader",
     "ObjectType",
     "OpenAiEmbedding",
+    "ParserLanguages",
+    "ParsingJob",
+    "ParsingJobMarkdownResult",
+    "ParsingJobTextResult",
     "PgVectorStore",
     "PineconeVectorStore",
     "Pipeline",
     "PipelineCreate",
-    "PipelineManagedIngestionExecution",
-    "PipelineManagedIngestionExecutionRunConfigPerOpValue",
+    "PipelineManagedIngestionJobRecord",
     "PipelineType",
+    "PlaygroundJobRecord",
     "Pooling",
     "PresetRetrievalParams",
     "Project",
     "ProjectCreate",
     "PydanticProgramMode",
     "QdrantVectorStore",
     "QuestionsAnsweredExtractor",
     "QuestionsAnsweredExtractorLlm",
     "ReaderConfig",
     "RelatedNodeInfo",
     "RetrieveResults",
     "RssReader",
-    "RunTransformAssetConfig",
     "SentenceSplitter",
     "SimpleFileNodeParser",
     "SimpleWebPageReader",
     "SlackReader",
     "StatusEnum",
     "SummaryExtractor",
     "SummaryExtractorLlm",
@@ -257,11 +246,12 @@
     "YoutubeTranscriptReader",
     "api_key",
     "component_definition",
     "data_sink",
     "data_source",
     "eval",
     "health",
+    "parsing",
     "pipeline",
     "project",
     "retrieval",
 ]
```

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/client.py` & `llamaindex_py_client-0.1.9/llama_index_client/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from .core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from .resources.api_key.client import ApiKeyClient, AsyncApiKeyClient
 from .resources.component_definition.client import AsyncComponentDefinitionClient, ComponentDefinitionClient
 from .resources.data_sink.client import AsyncDataSinkClient, DataSinkClient
 from .resources.data_source.client import AsyncDataSourceClient, DataSourceClient
 from .resources.eval.client import AsyncEvalClient, EvalClient
 from .resources.health.client import AsyncHealthClient, HealthClient
+from .resources.parsing.client import AsyncParsingClient, ParsingClient
 from .resources.pipeline.client import AsyncPipelineClient, PipelineClient
 from .resources.project.client import AsyncProjectClient, ProjectClient
 from .resources.retrieval.client import AsyncRetrievalClient, RetrievalClient
 
 
 class PlatformApi:
     def __init__(
@@ -33,14 +34,15 @@
         self.health = HealthClient(client_wrapper=self._client_wrapper)
         self.api_key = ApiKeyClient(client_wrapper=self._client_wrapper)
         self.data_sink = DataSinkClient(client_wrapper=self._client_wrapper)
         self.data_source = DataSourceClient(client_wrapper=self._client_wrapper)
         self.project = ProjectClient(client_wrapper=self._client_wrapper)
         self.pipeline = PipelineClient(client_wrapper=self._client_wrapper)
         self.eval = EvalClient(client_wrapper=self._client_wrapper)
+        self.parsing = ParsingClient(client_wrapper=self._client_wrapper)
         self.retrieval = RetrievalClient(client_wrapper=self._client_wrapper)
         self.component_definition = ComponentDefinitionClient(client_wrapper=self._client_wrapper)
 
 
 class AsyncPlatformApi:
     def __init__(
         self,
@@ -58,9 +60,10 @@
         self.health = AsyncHealthClient(client_wrapper=self._client_wrapper)
         self.api_key = AsyncApiKeyClient(client_wrapper=self._client_wrapper)
         self.data_sink = AsyncDataSinkClient(client_wrapper=self._client_wrapper)
         self.data_source = AsyncDataSourceClient(client_wrapper=self._client_wrapper)
         self.project = AsyncProjectClient(client_wrapper=self._client_wrapper)
         self.pipeline = AsyncPipelineClient(client_wrapper=self._client_wrapper)
         self.eval = AsyncEvalClient(client_wrapper=self._client_wrapper)
+        self.parsing = AsyncParsingClient(client_wrapper=self._client_wrapper)
         self.retrieval = AsyncRetrievalClient(client_wrapper=self._client_wrapper)
         self.component_definition = AsyncComponentDefinitionClient(client_wrapper=self._client_wrapper)
```

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/core/__init__.py` & `llamaindex_py_client-0.1.9/llama_index_client/core/__init__.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/core/client_wrapper.py` & `llamaindex_py_client-0.1.9/llama_index_client/core/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/core/datetime_utils.py` & `llamaindex_py_client-0.1.9/llama_index_client/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/core/jsonable_encoder.py` & `llamaindex_py_client-0.1.9/llama_index_client/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/resources/__init__.py` & `llamaindex_py_client-0.1.9/llama_index_client/resources/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from . import api_key, component_definition, data_sink, data_source, eval, health, pipeline, project, retrieval
+from . import api_key, component_definition, data_sink, data_source, eval, health, parsing, pipeline, project, retrieval
 from .data_sink import DataSinkUpdateComponent, DataSinkUpdateComponentOne
 from .data_source import DataSourceUpdateComponent, DataSourceUpdateComponentOne
 
 __all__ = [
     "DataSinkUpdateComponent",
     "DataSinkUpdateComponentOne",
     "DataSourceUpdateComponent",
     "DataSourceUpdateComponentOne",
     "api_key",
     "component_definition",
     "data_sink",
     "data_source",
     "eval",
     "health",
+    "parsing",
     "pipeline",
     "project",
     "retrieval",
 ]
```

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/resources/api_key/client.py` & `llamaindex_py_client-0.1.9/llama_index_client/resources/api_key/client.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/resources/component_definition/client.py` & `llamaindex_py_client-0.1.9/llama_index_client/resources/component_definition/client.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/resources/data_sink/client.py` & `llamaindex_py_client-0.1.9/llama_index_client/resources/data_sink/client.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/resources/data_sink/types/data_sink_update_component_one.py` & `llamaindex_py_client-0.1.9/llama_index_client/resources/data_sink/types/data_sink_update_component_one.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/resources/data_source/client.py` & `llamaindex_py_client-0.1.9/llama_index_client/resources/data_source/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from ...core.api_error import ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.configurable_data_source_names import ConfigurableDataSourceNames
 from ...types.data_source import DataSource
 from ...types.data_source_create import DataSourceCreate
-from ...types.data_source_load_execution import DataSourceLoadExecution
+from ...types.data_source_load_job_record import DataSourceLoadJobRecord
 from ...types.http_validation_error import HttpValidationError
 from ...types.loaded_file import LoadedFile
 from ...types.loaded_file_payload import LoadedFilePayload
 from .types.data_source_update_component import DataSourceUpdateComponent
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
@@ -259,15 +259,15 @@
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_data_source_executions(self, data_source_id: str) -> typing.List[DataSourceLoadExecution]:
+    def get_data_source_executions(self, data_source_id: str) -> typing.List[DataSourceLoadJobRecord]:
         """
         Get all data source executions for a given data source.
 
         Parameters:
             - data_source_id: str.
         ---
         from platform.client import PlatformApi
@@ -285,70 +285,91 @@
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/data_source/{data_source_id}/execution"
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[DataSourceLoadExecution], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[DataSourceLoadJobRecord], _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def create_data_source_execution(self, data_source_id: str) -> DataSourceLoadExecution:
+    def create_data_source_execution(self, data_source_id: str) -> DataSourceLoadJobRecord:
         """
         Create a new data source execution.
 
         Parameters:
             - data_source_id: str.
+        ---
+        from platform.client import PlatformApi
+
+        client = PlatformApi(
+            token="YOUR_TOKEN",
+            base_url="https://yourhost.com/path/to/api",
+        )
+        client.data_source.create_data_source_execution(
+            data_source_id="data-source-id",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/data_source/{data_source_id}/execution"
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DataSourceLoadExecution, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(DataSourceLoadJobRecord, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_data_source_execution(
         self, data_source_id: str, data_source_load_execution_id: str
-    ) -> DataSourceLoadExecution:
+    ) -> DataSourceLoadJobRecord:
         """
         Get a data source execution by ID.
 
         Parameters:
             - data_source_id: str.
 
             - data_source_load_execution_id: str.
+        ---
+        from platform.client import PlatformApi
+
+        client = PlatformApi(
+            token="YOUR_TOKEN",
+            base_url="https://yourhost.com/path/to/api",
+        )
+        client.data_source.get_data_source_execution(
+            data_source_id="data-source-id",
+            data_source_load_execution_id="data-source-load-execution-id",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"api/data_source/{data_source_id}/execution/{data_source_load_execution_id}",
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DataSourceLoadExecution, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(DataSourceLoadJobRecord, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
@@ -587,15 +608,15 @@
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_data_source_executions(self, data_source_id: str) -> typing.List[DataSourceLoadExecution]:
+    async def get_data_source_executions(self, data_source_id: str) -> typing.List[DataSourceLoadJobRecord]:
         """
         Get all data source executions for a given data source.
 
         Parameters:
             - data_source_id: str.
         ---
         from platform.client import AsyncPlatformApi
@@ -613,70 +634,91 @@
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/data_source/{data_source_id}/execution"
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[DataSourceLoadExecution], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[DataSourceLoadJobRecord], _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def create_data_source_execution(self, data_source_id: str) -> DataSourceLoadExecution:
+    async def create_data_source_execution(self, data_source_id: str) -> DataSourceLoadJobRecord:
         """
         Create a new data source execution.
 
         Parameters:
             - data_source_id: str.
+        ---
+        from platform.client import AsyncPlatformApi
+
+        client = AsyncPlatformApi(
+            token="YOUR_TOKEN",
+            base_url="https://yourhost.com/path/to/api",
+        )
+        await client.data_source.create_data_source_execution(
+            data_source_id="data-source-id",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/data_source/{data_source_id}/execution"
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DataSourceLoadExecution, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(DataSourceLoadJobRecord, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_data_source_execution(
         self, data_source_id: str, data_source_load_execution_id: str
-    ) -> DataSourceLoadExecution:
+    ) -> DataSourceLoadJobRecord:
         """
         Get a data source execution by ID.
 
         Parameters:
             - data_source_id: str.
 
             - data_source_load_execution_id: str.
+        ---
+        from platform.client import AsyncPlatformApi
+
+        client = AsyncPlatformApi(
+            token="YOUR_TOKEN",
+            base_url="https://yourhost.com/path/to/api",
+        )
+        await client.data_source.get_data_source_execution(
+            data_source_id="data-source-id",
+            data_source_load_execution_id="data-source-load-execution-id",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"api/data_source/{data_source_id}/execution/{data_source_load_execution_id}",
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DataSourceLoadExecution, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(DataSourceLoadJobRecord, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/resources/data_source/types/data_source_update_component_one.py` & `llamaindex_py_client-0.1.9/llama_index_client/resources/data_source/types/data_source_update_component_one.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/resources/eval/client.py` & `llamaindex_py_client-0.1.9/llama_index_client/resources/eval/client.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/resources/health/client.py` & `llamaindex_py_client-0.1.9/llama_index_client/resources/health/client.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/resources/pipeline/client.py` & `llamaindex_py_client-0.1.9/llama_index_client/resources/pipeline/client.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 from json.decoder import JSONDecodeError
 
 from ...core.api_error import ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_dict import remove_none_from_dict
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
-from ...types.configured_transformation_execution import ConfiguredTransformationExecution
 from ...types.configured_transformation_item import ConfiguredTransformationItem
 from ...types.data_sink_create import DataSinkCreate
 from ...types.data_source_create import DataSourceCreate
-from ...types.data_source_managed_ingestion_execution import DataSourceManagedIngestionExecution
-from ...types.eval_dataset_execution import EvalDatasetExecution
+from ...types.data_source_managed_ingestion_job_record import DataSourceManagedIngestionJobRecord
+from ...types.eval_dataset_job_record import EvalDatasetJobRecord
 from ...types.eval_execution_params import EvalExecutionParams
 from ...types.eval_question_result import EvalQuestionResult
 from ...types.http_validation_error import HttpValidationError
 from ...types.loaded_file import LoadedFile
-from ...types.loaded_file_managed_ingestion_execution import LoadedFileManagedIngestionExecution
 from ...types.pipeline import Pipeline
-from ...types.pipeline_managed_ingestion_execution import PipelineManagedIngestionExecution
+from ...types.pipeline_managed_ingestion_job_record import PipelineManagedIngestionJobRecord
+from ...types.pipeline_type import PipelineType
+from ...types.playground_job_record import PlaygroundJobRecord
 from ...types.preset_retrieval_params import PresetRetrievalParams
 from ...types.text_node import TextNode
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
@@ -34,61 +34,77 @@
 OMIT = typing.cast(typing.Any, ...)
 
 
 class PipelineClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def get_pipeline_by_name(self, *, pipeline_name: str, project_name: str) -> typing.List[Pipeline]:
+    def search_pipelines(
+        self,
+        *,
+        project_name: str,
+        pipeline_name: typing.Optional[str] = None,
+        pipeline_type: typing.Optional[PipelineType] = None,
+    ) -> typing.List[Pipeline]:
         """
-        Get a pipeline by name.
+        Search for pipelines by various parameters.
 
         Parameters:
-            - pipeline_name: str.
-
             - project_name: str.
+
+            - pipeline_name: typing.Optional[str].
+
+            - pipeline_type: typing.Optional[PipelineType].
         ---
+        from platform import PipelineType
         from platform.client import PlatformApi
 
         client = PlatformApi(
             token="YOUR_TOKEN",
             base_url="https://yourhost.com/path/to/api",
         )
-        client.pipeline.get_pipeline_by_name(
-            pipeline_name="pipeline-name",
+        client.pipeline.search_pipelines(
             project_name="project-name",
+            pipeline_type=PipelineType.PLAYGROUND,
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/pipeline"),
-            params=remove_none_from_dict({"pipeline_name": pipeline_name, "project_name": project_name}),
+            params=remove_none_from_dict(
+                {"project_name": project_name, "pipeline_name": pipeline_name, "pipeline_type": pipeline_type}
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[Pipeline], _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_pipeline_for_project(self, pipeline_id: str) -> Pipeline:
+    def get_pipeline_for_project(
+        self, pipeline_id: str, *, with_managed_ingestion_status: typing.Optional[bool] = None
+    ) -> Pipeline:
         """
         Get a pipeline by ID for a given project.
 
         Parameters:
             - pipeline_id: str.
+
+            - with_managed_ingestion_status: typing.Optional[bool].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/pipeline/{pipeline_id}"),
+            params=remove_none_from_dict({"with_managed_ingestion_status": with_managed_ingestion_status}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Pipeline, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
@@ -308,173 +324,169 @@
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_all_configured_transformation_executions(
-        self, pipeline_id: str
-    ) -> typing.List[ConfiguredTransformationExecution]:
+    def get_all_playground_jobs(self, pipeline_id: str) -> typing.List[PlaygroundJobRecord]:
         """
-        Get all ConfiguredTransformationExecutions for a given pipeline.
+        Get all PlaygroundJobRecords for a given pipeline.
 
         Parameters:
             - pipeline_id: str.
         ---
         from platform.client import PlatformApi
 
         client = PlatformApi(
             token="YOUR_TOKEN",
             base_url="https://yourhost.com/path/to/api",
         )
-        client.pipeline.get_all_configured_transformation_executions(
+        client.pipeline.get_all_playground_jobs(
             pipeline_id="pipeline-id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"api/pipeline/{pipeline_id}/configured_transformation_execution",
+                f"{self._client_wrapper.get_base_url()}/", f"api/pipeline/{pipeline_id}/playground_job"
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[ConfiguredTransformationExecution], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[PlaygroundJobRecord], _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def create_configured_transformation_execution(
-        self,
-        pipeline_id: str,
-        *,
-        configured_transformation_execution_id: typing.Optional[str] = None,
-        loaded_file_ids: typing.Optional[typing.Union[str, typing.List[str]]] = None,
-    ) -> ConfiguredTransformationExecution:
+    def create_playground_job(
+        self, pipeline_id: str, *, loaded_file_ids: typing.Optional[typing.Union[str, typing.List[str]]] = None
+    ) -> PlaygroundJobRecord:
         """
-        Kick off a new ConfiguredTransformation execution.
-        Can optionally supply a configured_transformation_execution_id to run a specific execution.
-        In absense of a configured_transformation_execution_id, the last
-        configured_transformation_execution will be run (which may end up triggering runs
-        for it's prior steps as well)
+        Kick off a new Playground execution.
 
         Parameters:
             - pipeline_id: str.
 
-            - configured_transformation_execution_id: typing.Optional[str].
-
             - loaded_file_ids: typing.Optional[typing.Union[str, typing.List[str]]].
+        ---
+        from platform.client import PlatformApi
+
+        client = PlatformApi(
+            token="YOUR_TOKEN",
+            base_url="https://yourhost.com/path/to/api",
+        )
+        client.pipeline.create_playground_job(
+            pipeline_id="pipeline-id",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"api/pipeline/{pipeline_id}/configured_transformation_execution",
-            ),
-            params=remove_none_from_dict(
-                {
-                    "configured_transformation_execution_id": configured_transformation_execution_id,
-                    "loaded_file_ids": loaded_file_ids,
-                }
+                f"{self._client_wrapper.get_base_url()}/", f"api/pipeline/{pipeline_id}/playground_job"
             ),
+            params=remove_none_from_dict({"loaded_file_ids": loaded_file_ids}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ConfiguredTransformationExecution, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(PlaygroundJobRecord, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_configured_transformation_execution(
-        self, pipeline_id: str, configured_transformation_execution_id: str
-    ) -> ConfiguredTransformationExecution:
+    def get_playground_job_result(
+        self, pipeline_id: str, *, configured_transformation_id: typing.Optional[str] = None
+    ) -> typing.List[TextNode]:
         """
-        Get status of a single pipeline ConfiguredTransformationExecution for a given pipeline.
+        Get the result of the latest Playground job.
 
         Parameters:
             - pipeline_id: str.
 
-            - configured_transformation_execution_id: str.
+            - configured_transformation_id: typing.Optional[str].
+        ---
+        from platform.client import PlatformApi
+
+        client = PlatformApi(
+            token="YOUR_TOKEN",
+            base_url="https://yourhost.com/path/to/api",
+        )
+        client.pipeline.get_playground_job_result(
+            pipeline_id="pipeline-id",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"api/pipeline/{pipeline_id}/configured_transformation_execution/{configured_transformation_execution_id}",
+                f"{self._client_wrapper.get_base_url()}/", f"api/pipeline/{pipeline_id}/playground_job/result"
             ),
+            params=remove_none_from_dict({"configured_transformation_id": configured_transformation_id}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ConfiguredTransformationExecution, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[TextNode], _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_configured_transformation_result(
-        self, pipeline_id: str, configured_transformation_id: str
-    ) -> typing.List[TextNode]:
+    def get_playground_job(self, pipeline_id: str, playground_job_id: str) -> PlaygroundJobRecord:
         """
-        Get the result of an ConfiguredTransformationExecution step.
-        Unlike get_configured_transformation_execution_result, this endpoint does
-        not check the status of the execution that produced the result for the
-        configured_transformation.
+        Get status of a single pipeline PlaygroundJob for a given pipeline.
 
         Parameters:
             - pipeline_id: str.
 
-            - configured_transformation_id: str.
+            - playground_job_id: str.
         ---
         from platform.client import PlatformApi
 
         client = PlatformApi(
             token="YOUR_TOKEN",
             base_url="https://yourhost.com/path/to/api",
         )
-        client.pipeline.get_configured_transformation_result(
+        client.pipeline.get_playground_job(
             pipeline_id="pipeline-id",
-            configured_transformation_id="configured-transformation-id",
+            playground_job_id="playground-job-id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
-                f"api/pipeline/{pipeline_id}/configured_transformation/{configured_transformation_id}/result",
+                f"api/pipeline/{pipeline_id}/playground_job/{playground_job_id}",
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[TextNode], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(PlaygroundJobRecord, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_eval_dataset_executions(self, pipeline_id: str, eval_dataset_id: str) -> typing.List[EvalDatasetExecution]:
+    def get_eval_dataset_executions(self, pipeline_id: str, eval_dataset_id: str) -> typing.List[EvalDatasetJobRecord]:
         """
         Get the status of an EvalDatasetExecution.
 
         Parameters:
             - pipeline_id: str.
 
             - eval_dataset_id: str.
@@ -496,15 +508,15 @@
                 f"{self._client_wrapper.get_base_url()}/",
                 f"api/pipeline/{pipeline_id}/eval_dataset/{eval_dataset_id}/execute",
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[EvalDatasetExecution], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[EvalDatasetJobRecord], _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
@@ -512,15 +524,15 @@
     def execute_eval_dataset(
         self,
         pipeline_id: str,
         eval_dataset_id: str,
         *,
         eval_question_ids: typing.List[str],
         params: EvalExecutionParams,
-    ) -> EvalDatasetExecution:
+    ) -> EvalDatasetJobRecord:
         """
         Execute a dataset.
 
         Parameters:
             - pipeline_id: str.
 
             - eval_dataset_id: str.
@@ -536,15 +548,15 @@
                 f"api/pipeline/{pipeline_id}/eval_dataset/{eval_dataset_id}/execute",
             ),
             json=jsonable_encoder({"eval_question_ids": eval_question_ids, "params": params}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(EvalDatasetExecution, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(EvalDatasetJobRecord, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
@@ -588,15 +600,15 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_eval_dataset_execution(
         self, pipeline_id: str, eval_dataset_id: str, eval_dataset_execution_id: str
-    ) -> EvalDatasetExecution:
+    ) -> EvalDatasetJobRecord:
         """
         Get the status of an EvalDatasetExecution.
 
         Parameters:
             - pipeline_id: str.
 
             - eval_dataset_id: str.
@@ -609,232 +621,152 @@
                 f"{self._client_wrapper.get_base_url()}/",
                 f"api/pipeline/{pipeline_id}/eval_dataset/{eval_dataset_id}/execute/{eval_dataset_execution_id}",
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(EvalDatasetExecution, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(EvalDatasetJobRecord, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_managed_loaded_file_ingestion_executions(
-        self, pipeline_id: str, loaded_file_id: str
-    ) -> typing.List[LoadedFileManagedIngestionExecution]:
+    def get_managed_data_source_ingestion_executions(
+        self, pipeline_id: str, data_source_id: str
+    ) -> typing.List[DataSourceManagedIngestionJobRecord]:
         """
-        Get all ManagedLoadedFileIngestionExecution for a given pipeline and loaded file.
+        Get all ManagedDataSourceIngestionExecution for a given pipeline and data source.
 
         Parameters:
             - pipeline_id: str.
 
-            - loaded_file_id: str.
+            - data_source_id: str.
         ---
         from platform.client import PlatformApi
 
         client = PlatformApi(
             token="YOUR_TOKEN",
             base_url="https://yourhost.com/path/to/api",
         )
-        client.pipeline.get_managed_loaded_file_ingestion_executions(
+        client.pipeline.get_managed_data_source_ingestion_executions(
             pipeline_id="pipeline-id",
-            loaded_file_id="loaded-file-id",
-        )
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"api/pipeline/{pipeline_id}/loaded_file/{loaded_file_id}/managed_ingest",
-            ),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[LoadedFileManagedIngestionExecution], _response.json())  # type: ignore
-        if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def run_managed_loaded_file_ingestion(
-        self, pipeline_id: str, loaded_file_id: str
-    ) -> LoadedFileManagedIngestionExecution:
-        """
-        Execute a ManagedLoadedFileIngestion.
-
-        Parameters:
-            - pipeline_id: str.
-
-            - loaded_file_id: str.
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"api/pipeline/{pipeline_id}/loaded_file/{loaded_file_id}/managed_ingest",
-            ),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            data_source_id="data-source-id",
         )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(LoadedFileManagedIngestionExecution, _response.json())  # type: ignore
-        if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def get_managed_loaded_file_ingestion_execution(
-        self, pipeline_id: str, loaded_file_id: str, managed_loaded_file_ingestion_id: str
-    ) -> LoadedFileManagedIngestionExecution:
-        """
-        Get a single ManagedLoadedFileIngestionExecution for a given pipeline and loaded file.
-
-        Parameters:
-            - pipeline_id: str.
-
-            - loaded_file_id: str.
-
-            - managed_loaded_file_ingestion_id: str.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
-                f"api/pipeline/{pipeline_id}/loaded_file/{loaded_file_id}/managed_ingest/{managed_loaded_file_ingestion_id}",
+                f"api/pipeline/{pipeline_id}/data_source/{data_source_id}/managed_ingest",
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(LoadedFileManagedIngestionExecution, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[DataSourceManagedIngestionJobRecord], _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_managed_data_source_ingestion_executions(
+    def run_managed_data_source_ingestion(
         self, pipeline_id: str, data_source_id: str
-    ) -> typing.List[DataSourceManagedIngestionExecution]:
+    ) -> DataSourceManagedIngestionJobRecord:
         """
-        Get all ManagedDataSourceIngestionExecution for a given pipeline and data source.
+        Execute a ManagedDataSourceIngestion.
 
         Parameters:
             - pipeline_id: str.
 
             - data_source_id: str.
         ---
         from platform.client import PlatformApi
 
         client = PlatformApi(
             token="YOUR_TOKEN",
             base_url="https://yourhost.com/path/to/api",
         )
-        client.pipeline.get_managed_data_source_ingestion_executions(
+        client.pipeline.run_managed_data_source_ingestion(
             pipeline_id="pipeline-id",
             data_source_id="data-source-id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"api/pipeline/{pipeline_id}/data_source/{data_source_id}/managed_ingest",
-            ),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[DataSourceManagedIngestionExecution], _response.json())  # type: ignore
-        if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def run_managed_data_source_ingestion(
-        self, pipeline_id: str, data_source_id: str
-    ) -> DataSourceManagedIngestionExecution:
-        """
-        Execute a ManagedDataSourceIngestion.
-
-        Parameters:
-            - pipeline_id: str.
-
-            - data_source_id: str.
-        """
-        _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"api/pipeline/{pipeline_id}/data_source/{data_source_id}/managed_ingest",
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DataSourceManagedIngestionExecution, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(DataSourceManagedIngestionJobRecord, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_managed_data_source_ingestion_execution(
         self, pipeline_id: str, data_source_id: str, managed_data_source_ingestion_id: str
-    ) -> DataSourceManagedIngestionExecution:
+    ) -> DataSourceManagedIngestionJobRecord:
         """
         Get a single ManagedDataSourceIngestionExecution for a given pipeline and data source.
 
         Parameters:
             - pipeline_id: str.
 
             - data_source_id: str.
 
             - managed_data_source_ingestion_id: str.
+        ---
+        from platform.client import PlatformApi
+
+        client = PlatformApi(
+            token="YOUR_TOKEN",
+            base_url="https://yourhost.com/path/to/api",
+        )
+        client.pipeline.get_managed_data_source_ingestion_execution(
+            pipeline_id="pipeline-id",
+            data_source_id="data-source-id",
+            managed_data_source_ingestion_id="managed-data-source-ingestion-id",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"api/pipeline/{pipeline_id}/data_source/{data_source_id}/managed_ingest/{managed_data_source_ingestion_id}",
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DataSourceManagedIngestionExecution, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(DataSourceManagedIngestionJobRecord, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_managed_pipeline_ingestion_executions(
         self, pipeline_id: str
-    ) -> typing.List[PipelineManagedIngestionExecution]:
+    ) -> typing.List[PipelineManagedIngestionJobRecord]:
         """
         Get all ManagedPipelineIngestionExecution for a given pipeline.
 
         Parameters:
             - pipeline_id: str.
         ---
         from platform.client import PlatformApi
@@ -852,128 +784,165 @@
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/pipeline/{pipeline_id}/managed_ingest"
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[PipelineManagedIngestionExecution], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[PipelineManagedIngestionJobRecord], _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def run_managed_pipeline_ingestion(self, pipeline_id: str) -> PipelineManagedIngestionExecution:
+    def run_managed_pipeline_ingestion(self, pipeline_id: str) -> PipelineManagedIngestionJobRecord:
         """
         Execute a ManagedPipelineIngestion.
 
         Parameters:
             - pipeline_id: str.
+        ---
+        from platform.client import PlatformApi
+
+        client = PlatformApi(
+            token="YOUR_TOKEN",
+            base_url="https://yourhost.com/path/to/api",
+        )
+        client.pipeline.run_managed_pipeline_ingestion(
+            pipeline_id="pipeline-id",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/pipeline/{pipeline_id}/managed_ingest"
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PipelineManagedIngestionExecution, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(PipelineManagedIngestionJobRecord, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_managed_ingestion_execution(
         self, pipeline_id: str, managed_pipeline_ingestion_id: str
-    ) -> PipelineManagedIngestionExecution:
+    ) -> PipelineManagedIngestionJobRecord:
         """
         Parameters:
             - pipeline_id: str.
 
             - managed_pipeline_ingestion_id: str.
+        ---
+        from platform.client import PlatformApi
+
+        client = PlatformApi(
+            token="YOUR_TOKEN",
+            base_url="https://yourhost.com/path/to/api",
+        )
+        client.pipeline.get_managed_ingestion_execution(
+            pipeline_id="pipeline-id",
+            managed_pipeline_ingestion_id="managed-pipeline-ingestion-id",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"api/pipeline/{pipeline_id}/managed_ingest/{managed_pipeline_ingestion_id}",
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PipelineManagedIngestionExecution, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(PipelineManagedIngestionJobRecord, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncPipelineClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def get_pipeline_by_name(self, *, pipeline_name: str, project_name: str) -> typing.List[Pipeline]:
+    async def search_pipelines(
+        self,
+        *,
+        project_name: str,
+        pipeline_name: typing.Optional[str] = None,
+        pipeline_type: typing.Optional[PipelineType] = None,
+    ) -> typing.List[Pipeline]:
         """
-        Get a pipeline by name.
+        Search for pipelines by various parameters.
 
         Parameters:
-            - pipeline_name: str.
-
             - project_name: str.
+
+            - pipeline_name: typing.Optional[str].
+
+            - pipeline_type: typing.Optional[PipelineType].
         ---
+        from platform import PipelineType
         from platform.client import AsyncPlatformApi
 
         client = AsyncPlatformApi(
             token="YOUR_TOKEN",
             base_url="https://yourhost.com/path/to/api",
         )
-        await client.pipeline.get_pipeline_by_name(
-            pipeline_name="pipeline-name",
+        await client.pipeline.search_pipelines(
             project_name="project-name",
+            pipeline_type=PipelineType.PLAYGROUND,
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/pipeline"),
-            params=remove_none_from_dict({"pipeline_name": pipeline_name, "project_name": project_name}),
+            params=remove_none_from_dict(
+                {"project_name": project_name, "pipeline_name": pipeline_name, "pipeline_type": pipeline_type}
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[Pipeline], _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_pipeline_for_project(self, pipeline_id: str) -> Pipeline:
+    async def get_pipeline_for_project(
+        self, pipeline_id: str, *, with_managed_ingestion_status: typing.Optional[bool] = None
+    ) -> Pipeline:
         """
         Get a pipeline by ID for a given project.
 
         Parameters:
             - pipeline_id: str.
+
+            - with_managed_ingestion_status: typing.Optional[bool].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/pipeline/{pipeline_id}"),
+            params=remove_none_from_dict({"with_managed_ingestion_status": with_managed_ingestion_status}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Pipeline, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
@@ -1193,175 +1162,171 @@
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_all_configured_transformation_executions(
-        self, pipeline_id: str
-    ) -> typing.List[ConfiguredTransformationExecution]:
+    async def get_all_playground_jobs(self, pipeline_id: str) -> typing.List[PlaygroundJobRecord]:
         """
-        Get all ConfiguredTransformationExecutions for a given pipeline.
+        Get all PlaygroundJobRecords for a given pipeline.
 
         Parameters:
             - pipeline_id: str.
         ---
         from platform.client import AsyncPlatformApi
 
         client = AsyncPlatformApi(
             token="YOUR_TOKEN",
             base_url="https://yourhost.com/path/to/api",
         )
-        await client.pipeline.get_all_configured_transformation_executions(
+        await client.pipeline.get_all_playground_jobs(
             pipeline_id="pipeline-id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"api/pipeline/{pipeline_id}/configured_transformation_execution",
+                f"{self._client_wrapper.get_base_url()}/", f"api/pipeline/{pipeline_id}/playground_job"
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[ConfiguredTransformationExecution], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[PlaygroundJobRecord], _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def create_configured_transformation_execution(
-        self,
-        pipeline_id: str,
-        *,
-        configured_transformation_execution_id: typing.Optional[str] = None,
-        loaded_file_ids: typing.Optional[typing.Union[str, typing.List[str]]] = None,
-    ) -> ConfiguredTransformationExecution:
+    async def create_playground_job(
+        self, pipeline_id: str, *, loaded_file_ids: typing.Optional[typing.Union[str, typing.List[str]]] = None
+    ) -> PlaygroundJobRecord:
         """
-        Kick off a new ConfiguredTransformation execution.
-        Can optionally supply a configured_transformation_execution_id to run a specific execution.
-        In absense of a configured_transformation_execution_id, the last
-        configured_transformation_execution will be run (which may end up triggering runs
-        for it's prior steps as well)
+        Kick off a new Playground execution.
 
         Parameters:
             - pipeline_id: str.
 
-            - configured_transformation_execution_id: typing.Optional[str].
-
             - loaded_file_ids: typing.Optional[typing.Union[str, typing.List[str]]].
+        ---
+        from platform.client import AsyncPlatformApi
+
+        client = AsyncPlatformApi(
+            token="YOUR_TOKEN",
+            base_url="https://yourhost.com/path/to/api",
+        )
+        await client.pipeline.create_playground_job(
+            pipeline_id="pipeline-id",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"api/pipeline/{pipeline_id}/configured_transformation_execution",
-            ),
-            params=remove_none_from_dict(
-                {
-                    "configured_transformation_execution_id": configured_transformation_execution_id,
-                    "loaded_file_ids": loaded_file_ids,
-                }
+                f"{self._client_wrapper.get_base_url()}/", f"api/pipeline/{pipeline_id}/playground_job"
             ),
+            params=remove_none_from_dict({"loaded_file_ids": loaded_file_ids}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ConfiguredTransformationExecution, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(PlaygroundJobRecord, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_configured_transformation_execution(
-        self, pipeline_id: str, configured_transformation_execution_id: str
-    ) -> ConfiguredTransformationExecution:
+    async def get_playground_job_result(
+        self, pipeline_id: str, *, configured_transformation_id: typing.Optional[str] = None
+    ) -> typing.List[TextNode]:
         """
-        Get status of a single pipeline ConfiguredTransformationExecution for a given pipeline.
+        Get the result of the latest Playground job.
 
         Parameters:
             - pipeline_id: str.
 
-            - configured_transformation_execution_id: str.
+            - configured_transformation_id: typing.Optional[str].
+        ---
+        from platform.client import AsyncPlatformApi
+
+        client = AsyncPlatformApi(
+            token="YOUR_TOKEN",
+            base_url="https://yourhost.com/path/to/api",
+        )
+        await client.pipeline.get_playground_job_result(
+            pipeline_id="pipeline-id",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"api/pipeline/{pipeline_id}/configured_transformation_execution/{configured_transformation_execution_id}",
+                f"{self._client_wrapper.get_base_url()}/", f"api/pipeline/{pipeline_id}/playground_job/result"
             ),
+            params=remove_none_from_dict({"configured_transformation_id": configured_transformation_id}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ConfiguredTransformationExecution, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[TextNode], _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_configured_transformation_result(
-        self, pipeline_id: str, configured_transformation_id: str
-    ) -> typing.List[TextNode]:
+    async def get_playground_job(self, pipeline_id: str, playground_job_id: str) -> PlaygroundJobRecord:
         """
-        Get the result of an ConfiguredTransformationExecution step.
-        Unlike get_configured_transformation_execution_result, this endpoint does
-        not check the status of the execution that produced the result for the
-        configured_transformation.
+        Get status of a single pipeline PlaygroundJob for a given pipeline.
 
         Parameters:
             - pipeline_id: str.
 
-            - configured_transformation_id: str.
+            - playground_job_id: str.
         ---
         from platform.client import AsyncPlatformApi
 
         client = AsyncPlatformApi(
             token="YOUR_TOKEN",
             base_url="https://yourhost.com/path/to/api",
         )
-        await client.pipeline.get_configured_transformation_result(
+        await client.pipeline.get_playground_job(
             pipeline_id="pipeline-id",
-            configured_transformation_id="configured-transformation-id",
+            playground_job_id="playground-job-id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
-                f"api/pipeline/{pipeline_id}/configured_transformation/{configured_transformation_id}/result",
+                f"api/pipeline/{pipeline_id}/playground_job/{playground_job_id}",
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[TextNode], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(PlaygroundJobRecord, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_eval_dataset_executions(
         self, pipeline_id: str, eval_dataset_id: str
-    ) -> typing.List[EvalDatasetExecution]:
+    ) -> typing.List[EvalDatasetJobRecord]:
         """
         Get the status of an EvalDatasetExecution.
 
         Parameters:
             - pipeline_id: str.
 
             - eval_dataset_id: str.
@@ -1383,15 +1348,15 @@
                 f"{self._client_wrapper.get_base_url()}/",
                 f"api/pipeline/{pipeline_id}/eval_dataset/{eval_dataset_id}/execute",
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[EvalDatasetExecution], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[EvalDatasetJobRecord], _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
@@ -1399,15 +1364,15 @@
     async def execute_eval_dataset(
         self,
         pipeline_id: str,
         eval_dataset_id: str,
         *,
         eval_question_ids: typing.List[str],
         params: EvalExecutionParams,
-    ) -> EvalDatasetExecution:
+    ) -> EvalDatasetJobRecord:
         """
         Execute a dataset.
 
         Parameters:
             - pipeline_id: str.
 
             - eval_dataset_id: str.
@@ -1423,15 +1388,15 @@
                 f"api/pipeline/{pipeline_id}/eval_dataset/{eval_dataset_id}/execute",
             ),
             json=jsonable_encoder({"eval_question_ids": eval_question_ids, "params": params}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(EvalDatasetExecution, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(EvalDatasetJobRecord, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
@@ -1475,15 +1440,15 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_eval_dataset_execution(
         self, pipeline_id: str, eval_dataset_id: str, eval_dataset_execution_id: str
-    ) -> EvalDatasetExecution:
+    ) -> EvalDatasetJobRecord:
         """
         Get the status of an EvalDatasetExecution.
 
         Parameters:
             - pipeline_id: str.
 
             - eval_dataset_id: str.
@@ -1496,232 +1461,152 @@
                 f"{self._client_wrapper.get_base_url()}/",
                 f"api/pipeline/{pipeline_id}/eval_dataset/{eval_dataset_id}/execute/{eval_dataset_execution_id}",
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(EvalDatasetExecution, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(EvalDatasetJobRecord, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_managed_loaded_file_ingestion_executions(
-        self, pipeline_id: str, loaded_file_id: str
-    ) -> typing.List[LoadedFileManagedIngestionExecution]:
+    async def get_managed_data_source_ingestion_executions(
+        self, pipeline_id: str, data_source_id: str
+    ) -> typing.List[DataSourceManagedIngestionJobRecord]:
         """
-        Get all ManagedLoadedFileIngestionExecution for a given pipeline and loaded file.
+        Get all ManagedDataSourceIngestionExecution for a given pipeline and data source.
 
         Parameters:
             - pipeline_id: str.
 
-            - loaded_file_id: str.
+            - data_source_id: str.
         ---
         from platform.client import AsyncPlatformApi
 
         client = AsyncPlatformApi(
             token="YOUR_TOKEN",
             base_url="https://yourhost.com/path/to/api",
         )
-        await client.pipeline.get_managed_loaded_file_ingestion_executions(
+        await client.pipeline.get_managed_data_source_ingestion_executions(
             pipeline_id="pipeline-id",
-            loaded_file_id="loaded-file-id",
-        )
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"api/pipeline/{pipeline_id}/loaded_file/{loaded_file_id}/managed_ingest",
-            ),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[LoadedFileManagedIngestionExecution], _response.json())  # type: ignore
-        if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def run_managed_loaded_file_ingestion(
-        self, pipeline_id: str, loaded_file_id: str
-    ) -> LoadedFileManagedIngestionExecution:
-        """
-        Execute a ManagedLoadedFileIngestion.
-
-        Parameters:
-            - pipeline_id: str.
-
-            - loaded_file_id: str.
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"api/pipeline/{pipeline_id}/loaded_file/{loaded_file_id}/managed_ingest",
-            ),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            data_source_id="data-source-id",
         )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(LoadedFileManagedIngestionExecution, _response.json())  # type: ignore
-        if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def get_managed_loaded_file_ingestion_execution(
-        self, pipeline_id: str, loaded_file_id: str, managed_loaded_file_ingestion_id: str
-    ) -> LoadedFileManagedIngestionExecution:
-        """
-        Get a single ManagedLoadedFileIngestionExecution for a given pipeline and loaded file.
-
-        Parameters:
-            - pipeline_id: str.
-
-            - loaded_file_id: str.
-
-            - managed_loaded_file_ingestion_id: str.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
-                f"api/pipeline/{pipeline_id}/loaded_file/{loaded_file_id}/managed_ingest/{managed_loaded_file_ingestion_id}",
+                f"api/pipeline/{pipeline_id}/data_source/{data_source_id}/managed_ingest",
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(LoadedFileManagedIngestionExecution, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[DataSourceManagedIngestionJobRecord], _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_managed_data_source_ingestion_executions(
+    async def run_managed_data_source_ingestion(
         self, pipeline_id: str, data_source_id: str
-    ) -> typing.List[DataSourceManagedIngestionExecution]:
+    ) -> DataSourceManagedIngestionJobRecord:
         """
-        Get all ManagedDataSourceIngestionExecution for a given pipeline and data source.
+        Execute a ManagedDataSourceIngestion.
 
         Parameters:
             - pipeline_id: str.
 
             - data_source_id: str.
         ---
         from platform.client import AsyncPlatformApi
 
         client = AsyncPlatformApi(
             token="YOUR_TOKEN",
             base_url="https://yourhost.com/path/to/api",
         )
-        await client.pipeline.get_managed_data_source_ingestion_executions(
+        await client.pipeline.run_managed_data_source_ingestion(
             pipeline_id="pipeline-id",
             data_source_id="data-source-id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"api/pipeline/{pipeline_id}/data_source/{data_source_id}/managed_ingest",
-            ),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[DataSourceManagedIngestionExecution], _response.json())  # type: ignore
-        if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def run_managed_data_source_ingestion(
-        self, pipeline_id: str, data_source_id: str
-    ) -> DataSourceManagedIngestionExecution:
-        """
-        Execute a ManagedDataSourceIngestion.
-
-        Parameters:
-            - pipeline_id: str.
-
-            - data_source_id: str.
-        """
-        _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"api/pipeline/{pipeline_id}/data_source/{data_source_id}/managed_ingest",
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DataSourceManagedIngestionExecution, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(DataSourceManagedIngestionJobRecord, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_managed_data_source_ingestion_execution(
         self, pipeline_id: str, data_source_id: str, managed_data_source_ingestion_id: str
-    ) -> DataSourceManagedIngestionExecution:
+    ) -> DataSourceManagedIngestionJobRecord:
         """
         Get a single ManagedDataSourceIngestionExecution for a given pipeline and data source.
 
         Parameters:
             - pipeline_id: str.
 
             - data_source_id: str.
 
             - managed_data_source_ingestion_id: str.
+        ---
+        from platform.client import AsyncPlatformApi
+
+        client = AsyncPlatformApi(
+            token="YOUR_TOKEN",
+            base_url="https://yourhost.com/path/to/api",
+        )
+        await client.pipeline.get_managed_data_source_ingestion_execution(
+            pipeline_id="pipeline-id",
+            data_source_id="data-source-id",
+            managed_data_source_ingestion_id="managed-data-source-ingestion-id",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"api/pipeline/{pipeline_id}/data_source/{data_source_id}/managed_ingest/{managed_data_source_ingestion_id}",
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DataSourceManagedIngestionExecution, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(DataSourceManagedIngestionJobRecord, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_managed_pipeline_ingestion_executions(
         self, pipeline_id: str
-    ) -> typing.List[PipelineManagedIngestionExecution]:
+    ) -> typing.List[PipelineManagedIngestionJobRecord]:
         """
         Get all ManagedPipelineIngestionExecution for a given pipeline.
 
         Parameters:
             - pipeline_id: str.
         ---
         from platform.client import AsyncPlatformApi
@@ -1739,68 +1624,89 @@
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/pipeline/{pipeline_id}/managed_ingest"
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[PipelineManagedIngestionExecution], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[PipelineManagedIngestionJobRecord], _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def run_managed_pipeline_ingestion(self, pipeline_id: str) -> PipelineManagedIngestionExecution:
+    async def run_managed_pipeline_ingestion(self, pipeline_id: str) -> PipelineManagedIngestionJobRecord:
         """
         Execute a ManagedPipelineIngestion.
 
         Parameters:
             - pipeline_id: str.
+        ---
+        from platform.client import AsyncPlatformApi
+
+        client = AsyncPlatformApi(
+            token="YOUR_TOKEN",
+            base_url="https://yourhost.com/path/to/api",
+        )
+        await client.pipeline.run_managed_pipeline_ingestion(
+            pipeline_id="pipeline-id",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/pipeline/{pipeline_id}/managed_ingest"
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PipelineManagedIngestionExecution, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(PipelineManagedIngestionJobRecord, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_managed_ingestion_execution(
         self, pipeline_id: str, managed_pipeline_ingestion_id: str
-    ) -> PipelineManagedIngestionExecution:
+    ) -> PipelineManagedIngestionJobRecord:
         """
         Parameters:
             - pipeline_id: str.
 
             - managed_pipeline_ingestion_id: str.
+        ---
+        from platform.client import AsyncPlatformApi
+
+        client = AsyncPlatformApi(
+            token="YOUR_TOKEN",
+            base_url="https://yourhost.com/path/to/api",
+        )
+        await client.pipeline.get_managed_ingestion_execution(
+            pipeline_id="pipeline-id",
+            managed_pipeline_ingestion_id="managed-pipeline-ingestion-id",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"api/pipeline/{pipeline_id}/managed_ingest/{managed_pipeline_ingestion_id}",
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PipelineManagedIngestionExecution, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(PipelineManagedIngestionJobRecord, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/resources/project/client.py` & `llamaindex_py_client-0.1.9/llama_index_client/resources/project/client.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/resources/retrieval/client.py` & `llamaindex_py_client-0.1.9/llama_index_client/resources/retrieval/client.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/__init__.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,18 +7,14 @@
 from .beautiful_soup_web_reader import BeautifulSoupWebReader
 from .chroma_vector_store import ChromaVectorStore
 from .code_splitter import CodeSplitter
 from .configurable_data_sink_names import ConfigurableDataSinkNames
 from .configurable_data_source_names import ConfigurableDataSourceNames
 from .configurable_transformation_definition import ConfigurableTransformationDefinition
 from .configurable_transformation_names import ConfigurableTransformationNames
-from .configured_transformation_execution import ConfiguredTransformationExecution
-from .configured_transformation_execution_run_config_per_op_value import (
-    ConfiguredTransformationExecutionRunConfigPerOpValue,
-)
 from .configured_transformation_item import ConfiguredTransformationItem
 from .configured_transformation_item_component import ConfiguredTransformationItemComponent
 from .configured_transformation_item_component_one import ConfiguredTransformationItemComponentOne
 from .data_sink import DataSink
 from .data_sink_component import DataSinkComponent
 from .data_sink_component_one import DataSinkComponentOne
 from .data_sink_create import DataSinkCreate
@@ -28,82 +24,72 @@
 from .data_source import DataSource
 from .data_source_component import DataSourceComponent
 from .data_source_component_one import DataSourceComponentOne
 from .data_source_create import DataSourceCreate
 from .data_source_create_component import DataSourceCreateComponent
 from .data_source_create_component_one import DataSourceCreateComponentOne
 from .data_source_definition import DataSourceDefinition
-from .data_source_load_execution import DataSourceLoadExecution
-from .data_source_load_execution_run_config_per_op_value import DataSourceLoadExecutionRunConfigPerOpValue
-from .data_source_managed_ingestion_execution import DataSourceManagedIngestionExecution
-from .data_source_managed_ingestion_execution_run_config_per_op_value import (
-    DataSourceManagedIngestionExecutionRunConfigPerOpValue,
-)
+from .data_source_load_job_record import DataSourceLoadJobRecord
+from .data_source_managed_ingestion_job_record import DataSourceManagedIngestionJobRecord
 from .discord_reader import DiscordReader
 from .document import Document
 from .document_group import DocumentGroup
 from .document_relationships_value import DocumentRelationshipsValue
 from .elasticsearch_reader import ElasticsearchReader
-from .etl_job_names import EtlJobNames
 from .eval_dataset import EvalDataset
-from .eval_dataset_execution import EvalDatasetExecution
-from .eval_dataset_execution_config import EvalDatasetExecutionConfig
-from .eval_dataset_execution_run_config_per_op_value import EvalDatasetExecutionRunConfigPerOpValue
+from .eval_dataset_job_record import EvalDatasetJobRecord
 from .eval_execution_params import EvalExecutionParams
 from .eval_llm_model_data import EvalLlmModelData
 from .eval_question import EvalQuestion
 from .eval_question_create import EvalQuestionCreate
 from .eval_question_result import EvalQuestionResult
 from .externally_stored_component import ExternallyStoredComponent
 from .google_docs_reader import GoogleDocsReader
 from .google_sheets_reader import GoogleSheetsReader
 from .html_node_parser import HtmlNodeParser
 from .http_validation_error import HttpValidationError
 from .hugging_face_inference_api_embedding import HuggingFaceInferenceApiEmbedding
+from .job_names import JobNames
 from .json_node_parser import JsonNodeParser
 from .keyword_extractor import KeywordExtractor
 from .keyword_extractor_llm import KeywordExtractorLlm
 from .llm import Llm
 from .llm_predictor import LlmPredictor
 from .loaded_file import LoadedFile
-from .loaded_file_managed_ingestion_execution import LoadedFileManagedIngestionExecution
-from .loaded_file_managed_ingestion_execution_run_config_per_op_value import (
-    LoadedFileManagedIngestionExecutionRunConfigPerOpValue,
-)
 from .loaded_file_payload import LoadedFilePayload
-from .managed_data_source_ingestion_job_config import ManagedDataSourceIngestionJobConfig
-from .managed_pipeline_ingestion_job_config import ManagedPipelineIngestionJobConfig
+from .managed_ingestion_status import ManagedIngestionStatus
 from .markdown_node_parser import MarkdownNodeParser
 from .metadata_mode import MetadataMode
 from .metric_result import MetricResult
 from .notion_page_reader import NotionPageReader
 from .object_type import ObjectType
 from .open_ai_embedding import OpenAiEmbedding
+from .parser_languages import ParserLanguages
+from .parsing_job import ParsingJob
+from .parsing_job_markdown_result import ParsingJobMarkdownResult
+from .parsing_job_text_result import ParsingJobTextResult
 from .pg_vector_store import PgVectorStore
 from .pinecone_vector_store import PineconeVectorStore
 from .pipeline import Pipeline
 from .pipeline_create import PipelineCreate
-from .pipeline_managed_ingestion_execution import PipelineManagedIngestionExecution
-from .pipeline_managed_ingestion_execution_run_config_per_op_value import (
-    PipelineManagedIngestionExecutionRunConfigPerOpValue,
-)
+from .pipeline_managed_ingestion_job_record import PipelineManagedIngestionJobRecord
 from .pipeline_type import PipelineType
+from .playground_job_record import PlaygroundJobRecord
 from .pooling import Pooling
 from .preset_retrieval_params import PresetRetrievalParams
 from .project import Project
 from .project_create import ProjectCreate
 from .pydantic_program_mode import PydanticProgramMode
 from .qdrant_vector_store import QdrantVectorStore
 from .questions_answered_extractor import QuestionsAnsweredExtractor
 from .questions_answered_extractor_llm import QuestionsAnsweredExtractorLlm
 from .reader_config import ReaderConfig
 from .related_node_info import RelatedNodeInfo
 from .retrieve_results import RetrieveResults
 from .rss_reader import RssReader
-from .run_transform_asset_config import RunTransformAssetConfig
 from .sentence_splitter import SentenceSplitter
 from .simple_file_node_parser import SimpleFileNodeParser
 from .simple_web_page_reader import SimpleWebPageReader
 from .slack_reader import SlackReader
 from .status_enum import StatusEnum
 from .summary_extractor import SummaryExtractor
 from .summary_extractor_llm import SummaryExtractorLlm
@@ -132,16 +118,14 @@
     "BeautifulSoupWebReader",
     "ChromaVectorStore",
     "CodeSplitter",
     "ConfigurableDataSinkNames",
     "ConfigurableDataSourceNames",
     "ConfigurableTransformationDefinition",
     "ConfigurableTransformationNames",
-    "ConfiguredTransformationExecution",
-    "ConfiguredTransformationExecutionRunConfigPerOpValue",
     "ConfiguredTransformationItem",
     "ConfiguredTransformationItemComponent",
     "ConfiguredTransformationItemComponentOne",
     "DataSink",
     "DataSinkComponent",
     "DataSinkComponentOne",
     "DataSinkCreate",
@@ -151,76 +135,72 @@
     "DataSource",
     "DataSourceComponent",
     "DataSourceComponentOne",
     "DataSourceCreate",
     "DataSourceCreateComponent",
     "DataSourceCreateComponentOne",
     "DataSourceDefinition",
-    "DataSourceLoadExecution",
-    "DataSourceLoadExecutionRunConfigPerOpValue",
-    "DataSourceManagedIngestionExecution",
-    "DataSourceManagedIngestionExecutionRunConfigPerOpValue",
+    "DataSourceLoadJobRecord",
+    "DataSourceManagedIngestionJobRecord",
     "DiscordReader",
     "Document",
     "DocumentGroup",
     "DocumentRelationshipsValue",
     "ElasticsearchReader",
-    "EtlJobNames",
     "EvalDataset",
-    "EvalDatasetExecution",
-    "EvalDatasetExecutionConfig",
-    "EvalDatasetExecutionRunConfigPerOpValue",
+    "EvalDatasetJobRecord",
     "EvalExecutionParams",
     "EvalLlmModelData",
     "EvalQuestion",
     "EvalQuestionCreate",
     "EvalQuestionResult",
     "ExternallyStoredComponent",
     "GoogleDocsReader",
     "GoogleSheetsReader",
     "HtmlNodeParser",
     "HttpValidationError",
     "HuggingFaceInferenceApiEmbedding",
+    "JobNames",
     "JsonNodeParser",
     "KeywordExtractor",
     "KeywordExtractorLlm",
     "Llm",
     "LlmPredictor",
     "LoadedFile",
-    "LoadedFileManagedIngestionExecution",
-    "LoadedFileManagedIngestionExecutionRunConfigPerOpValue",
     "LoadedFilePayload",
-    "ManagedDataSourceIngestionJobConfig",
-    "ManagedPipelineIngestionJobConfig",
+    "ManagedIngestionStatus",
     "MarkdownNodeParser",
     "MetadataMode",
     "MetricResult",
     "NotionPageReader",
     "ObjectType",
     "OpenAiEmbedding",
+    "ParserLanguages",
+    "ParsingJob",
+    "ParsingJobMarkdownResult",
+    "ParsingJobTextResult",
     "PgVectorStore",
     "PineconeVectorStore",
     "Pipeline",
     "PipelineCreate",
-    "PipelineManagedIngestionExecution",
-    "PipelineManagedIngestionExecutionRunConfigPerOpValue",
+    "PipelineManagedIngestionJobRecord",
     "PipelineType",
+    "PlaygroundJobRecord",
     "Pooling",
     "PresetRetrievalParams",
     "Project",
     "ProjectCreate",
     "PydanticProgramMode",
     "QdrantVectorStore",
     "QuestionsAnsweredExtractor",
     "QuestionsAnsweredExtractorLlm",
     "ReaderConfig",
     "RelatedNodeInfo",
     "RetrieveResults",
     "RssReader",
-    "RunTransformAssetConfig",
     "SentenceSplitter",
     "SimpleFileNodeParser",
     "SimpleWebPageReader",
     "SlackReader",
     "StatusEnum",
     "SummaryExtractor",
     "SummaryExtractorLlm",
```

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/api_key.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/api_key.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/azure_open_ai_embedding.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/azure_open_ai_embedding.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/base_prompt_template.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/base_prompt_template.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/base_pydantic_reader.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/base_pydantic_reader.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/beautiful_soup_web_reader.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/beautiful_soup_web_reader.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/chroma_vector_store.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/chroma_vector_store.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/code_splitter.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/code_splitter.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/configurable_data_sink_names.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/configurable_data_sink_names.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/configurable_data_source_names.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/configurable_data_source_names.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/configurable_transformation_definition.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/configurable_transformation_definition.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/configurable_transformation_names.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/configurable_transformation_names.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/configured_transformation_execution.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/eval_question.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .configured_transformation_execution_run_config_per_op_value import (
-    ConfiguredTransformationExecutionRunConfigPerOpValue,
-)
-from .etl_job_names import EtlJobNames
-from .status_enum import StatusEnum
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class ConfiguredTransformationExecution(pydantic.BaseModel):
+class EvalQuestion(pydantic.BaseModel):
     """
-    Schema for a job that executes a transform step in a pipeline.
+    Base schema model containing common database fields.
     """
 
     id: str = pydantic.Field(description="Unique identifier")
     created_at: typing.Optional[dt.datetime] = pydantic.Field(description="Creation datetime")
     updated_at: typing.Optional[dt.datetime] = pydantic.Field(description="Update datetime")
-    job_name: EtlJobNames
-    status: StatusEnum
-    started_at: typing.Optional[dt.datetime]
-    ended_at: typing.Optional[dt.datetime]
-    run_config_per_op: typing.Dict[str, ConfiguredTransformationExecutionRunConfigPerOpValue] = pydantic.Field(
-        description="Run config that was given to the Dagster job"
-    )
-    partitions: typing.Optional[typing.Dict[str, str]] = pydantic.Field(description="Partition information")
-    pipeline_id: str = pydantic.Field(
-        description="The ID for the Pipeline for which this execution ran a particular transformation."
-    )
-    configured_transformation_id: str = pydantic.Field(
-        description="The ID for the specific configured transformation step this execution ran."
+    content: str = pydantic.Field(description="The content of the question.")
+    eval_dataset_id: str
+    eval_dataset_index: int = pydantic.Field(
+        description="The index at which this question is positioned relative to the other questions in the linked EvalDataset. Client is responsible for setting this correctly."
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/configured_transformation_item.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/configured_transformation_item.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/configured_transformation_item_component_one.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/configured_transformation_item_component_one.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/data_sink.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/data_sink.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/data_sink_create.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/data_sink_create.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/data_sink_definition.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/data_sink_definition.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/data_source.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/data_source.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/data_source_component_one.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/data_source_component_one.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/data_source_create.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/data_source_create.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/data_source_create_component_one.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/data_source_create_component_one.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/data_source_definition.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/data_source_definition.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/data_source_load_execution.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/data_source_managed_ingestion_job_record.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,35 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .data_source_load_execution_run_config_per_op_value import DataSourceLoadExecutionRunConfigPerOpValue
-from .etl_job_names import EtlJobNames
+from .job_names import JobNames
 from .status_enum import StatusEnum
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class DataSourceLoadExecution(pydantic.BaseModel):
+class DataSourceManagedIngestionJobRecord(pydantic.BaseModel):
     """
-    Schema for job that loads from a data source.
+    Schema for job that executes managed pipeline ingestion over a single data-source linked to a pipeline.
     """
 
-    id: str = pydantic.Field(description="Unique identifier")
-    created_at: typing.Optional[dt.datetime] = pydantic.Field(description="Creation datetime")
-    updated_at: typing.Optional[dt.datetime] = pydantic.Field(description="Update datetime")
-    job_name: EtlJobNames
+    id: typing.Optional[str] = pydantic.Field(description="Unique identifier")
+    job_name: JobNames
     status: StatusEnum
     started_at: typing.Optional[dt.datetime]
     ended_at: typing.Optional[dt.datetime]
-    run_config_per_op: typing.Dict[str, DataSourceLoadExecutionRunConfigPerOpValue] = pydantic.Field(
-        description="Run config that was given to the Dagster job"
-    )
-    partitions: typing.Optional[typing.Dict[str, str]] = pydantic.Field(description="Partition information")
-    data_source_id: str = pydantic.Field(description="The ID for the DataSource this execution loaded documents from.")
+    created_at: typing.Optional[dt.datetime] = pydantic.Field(description="Creation datetime")
+    updated_at: typing.Optional[dt.datetime] = pydantic.Field(description="Update datetime")
+    partitions: typing.Dict[str, str] = pydantic.Field(description="The partitions for this execution.")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/data_source_managed_ingestion_execution.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/pipeline_managed_ingestion_job_record.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,35 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .data_source_managed_ingestion_execution_run_config_per_op_value import (
-    DataSourceManagedIngestionExecutionRunConfigPerOpValue,
-)
-from .etl_job_names import EtlJobNames
+from .job_names import JobNames
 from .status_enum import StatusEnum
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class DataSourceManagedIngestionExecution(pydantic.BaseModel):
+class PipelineManagedIngestionJobRecord(pydantic.BaseModel):
     """
-    Schema for job that executes managed pipeline ingestion over a single data-source linked to a pipeline.
+    Schema for job that executes managed pipeline ingestion over all data-sources linked to a pipeline.
     """
 
-    id: str = pydantic.Field(description="Unique identifier")
-    created_at: typing.Optional[dt.datetime] = pydantic.Field(description="Creation datetime")
-    updated_at: typing.Optional[dt.datetime] = pydantic.Field(description="Update datetime")
-    job_name: EtlJobNames
+    id: typing.Optional[str] = pydantic.Field(description="Unique identifier")
+    job_name: JobNames
     status: StatusEnum
     started_at: typing.Optional[dt.datetime]
     ended_at: typing.Optional[dt.datetime]
-    run_config_per_op: typing.Dict[str, DataSourceManagedIngestionExecutionRunConfigPerOpValue] = pydantic.Field(
-        description="Run config that was given to the Dagster job"
-    )
-    partitions: typing.Optional[typing.Dict[str, str]] = pydantic.Field(description="Partition information")
-    pipeline_id: str = pydantic.Field(description="The ID for the Pipeline this execution ran against.")
-    data_source_id: str = pydantic.Field(description="The ID for the DataSource this execution ran against.")
+    created_at: typing.Optional[dt.datetime] = pydantic.Field(description="Creation datetime")
+    updated_at: typing.Optional[dt.datetime] = pydantic.Field(description="Update datetime")
+    partitions: typing.Dict[str, str] = pydantic.Field(description="The partitions for this execution.")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/discord_reader.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/discord_reader.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/document.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/document.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/document_group.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/document_group.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/elasticsearch_reader.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/elasticsearch_reader.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/eval_dataset.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/eval_dataset.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/eval_dataset_execution.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/eval_question_result.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .etl_job_names import EtlJobNames
-from .eval_dataset_execution_run_config_per_op_value import EvalDatasetExecutionRunConfigPerOpValue
 from .eval_execution_params import EvalExecutionParams
-from .status_enum import StatusEnum
+from .metric_result import MetricResult
+from .text_node import TextNode
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class EvalDatasetExecution(pydantic.BaseModel):
+class EvalQuestionResult(pydantic.BaseModel):
     """
-    Schema for job that evaluates an EvalDataset against a pipeline.
+    Schema for the result of an eval question job.
     """
 
-    id: str = pydantic.Field(description="Unique identifier")
-    created_at: typing.Optional[dt.datetime] = pydantic.Field(description="Creation datetime")
-    updated_at: typing.Optional[dt.datetime] = pydantic.Field(description="Update datetime")
-    job_name: EtlJobNames
-    status: StatusEnum
-    started_at: typing.Optional[dt.datetime]
-    ended_at: typing.Optional[dt.datetime]
-    run_config_per_op: typing.Dict[str, EvalDatasetExecutionRunConfigPerOpValue] = pydantic.Field(
-        description="Run config that was given to the Dagster job"
+    eval_question_id: str = pydantic.Field(description="The ID of the question that was executed.")
+    pipeline_id: str = pydantic.Field(description="The ID of the pipeline that the question was executed against.")
+    source_nodes: typing.List[TextNode] = pydantic.Field(
+        description="The nodes retrieved by the pipeline for the given question."
     )
-    pipeline_id: str = pydantic.Field(description="The ID for the Pipeline this execution ran against.")
-    eval_dataset_id: str = pydantic.Field(description="The ID for the EvalDataset this execution ran against.")
-    eval_question_ids: typing.List[str] = pydantic.Field(
-        description="The IDs for the EvalQuestions this execution ran against."
+    answer: str = pydantic.Field(description="The answer to the question.")
+    eval_metrics: typing.Dict[str, MetricResult] = pydantic.Field(description="The eval metrics for the question.")
+    eval_dataset_execution_id: str = pydantic.Field(
+        description="The ID of the EvalDatasetJobRecord that this result was generated from."
     )
-    eval_execution_params: EvalExecutionParams = pydantic.Field(description="The parameters for the eval execution.")
+    eval_dataset_execution_params: EvalExecutionParams = pydantic.Field(
+        description="The EvalExecutionParams that were used when this result was generated."
+    )
+    eval_finished_at: dt.datetime = pydantic.Field(description="The timestamp when the eval finished.")
+    class_name: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/eval_dataset_execution_config.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/externally_stored_component.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class EvalDatasetExecutionConfig(pydantic.BaseModel):
+class ExternallyStoredComponent(pydantic.BaseModel):
     """
-    Dagster op configuration for eval_dataset_execution job.
+    Base schema model for BaseComponent classes used in the platform.
+    Comes with special serialization logic for types used commonly in platform codebase.
     """
 
-    pipeline_id: str
-    eval_dataset_id: str
-    eval_question_ids: typing.List[str] = pydantic.Field(description="List of eval question ids")
-    eval_exec_params_json: str = pydantic.Field(description="JSON serialized EvalExecutionParams object")
+    id: str = pydantic.Field(description="The ID of the externally stored component.")
+    extra_path_prefix: str = pydantic.Field(description="The extra path prefix for the externally stored component.")
+    class_name: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/eval_execution_params.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/eval_execution_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 
 class EvalExecutionParams(pydantic.BaseModel):
     """
     Schema for the params for an eval execution.
     """
 
     llm_model: SupportedEvalLlmModelNames = pydantic.Field(description="The LLM model to use within eval execution.")
-    number_of_node_to_retrieve: int = pydantic.Field(description="Number of nodes to retrieve within eval execution.")
+    number_of_node_to_retrieve: int = pydantic.Field(
+        description="DEPRECATED - Number of nodes to retrieve within eval execution."
+    )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/eval_llm_model_data.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/eval_llm_model_data.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/eval_question.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/slack_reader.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,27 +7,39 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class EvalQuestion(pydantic.BaseModel):
+class SlackReader(pydantic.BaseModel):
     """
-    Base schema model containing common database fields.
+    Slack reader.
+
+    Reads conversations from channels. If an earliest_date is provided, an
+    optional latest_date can also be provided. If no latest_date is provided,
+    we assume the latest date is the current timestamp.
+
+    Args:
+    slack_token (Optional[str]): Slack token. If not provided, we
+    assume the environment variable `SLACK_BOT_TOKEN` is set.
+    ssl (Optional[str]): Custom SSL context. If not provided, it is assumed
+    there is already an SSL context available.
+    earliest_date (Optional[datetime]): Earliest date from which
+    to read conversations. If not provided, we read all messages.
+    latest_date (Optional[datetime]): Latest date from which to
+    read conversations. If not provided, defaults to current timestamp
+    in combination with earliest_date.
     """
 
-    id: str = pydantic.Field(description="Unique identifier")
-    created_at: typing.Optional[dt.datetime] = pydantic.Field(description="Creation datetime")
-    updated_at: typing.Optional[dt.datetime] = pydantic.Field(description="Update datetime")
-    content: str = pydantic.Field(description="The content of the question.")
-    eval_dataset_id: str
-    eval_dataset_index: int = pydantic.Field(
-        description="The index at which this question is positioned relative to the other questions in the linked EvalDataset. Client is responsible for setting this correctly."
-    )
+    is_remote: typing.Optional[bool]
+    slack_token: str
+    earliest_date_timestamp: typing.Optional[float]
+    latest_date_timestamp: float
+    class_name: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/eval_question_create.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/eval_question_create.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/eval_question_result.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/retrieve_results.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .eval_execution_params import EvalExecutionParams
-from .metric_result import MetricResult
-from .text_node import TextNode
+from .text_node_with_score import TextNodeWithScore
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class EvalQuestionResult(pydantic.BaseModel):
+class RetrieveResults(pydantic.BaseModel):
     """
-    Schema for the result of an eval question execution.
+    Schema for the result of an retrieval execution.
     """
 
-    eval_question_id: str = pydantic.Field(description="The ID of the question that was executed.")
-    pipeline_id: str = pydantic.Field(description="The ID of the pipeline that the question was executed against.")
-    source_nodes: typing.List[TextNode] = pydantic.Field(
-        description="The nodes retrieved by the pipeline for the given question."
+    pipeline_id: str = pydantic.Field(description="The ID of the pipeline that the query was retrieved against.")
+    retrieval_nodes: typing.List[TextNodeWithScore] = pydantic.Field(
+        description="The nodes retrieved by the pipeline for the given query."
     )
-    answer: str = pydantic.Field(description="The answer to the question.")
-    eval_metrics: typing.Dict[str, MetricResult] = pydantic.Field(description="The eval metrics for the question.")
-    eval_dataset_execution_id: str = pydantic.Field(
-        description="The ID of the EvalDatasetExecution that this result was generated from."
-    )
-    eval_dataset_execution_params: EvalExecutionParams = pydantic.Field(
-        description="The EvalExecutionParams that were used when this result was generated."
-    )
-    eval_finished_at: dt.datetime = pydantic.Field(description="The timestamp when the eval finished.")
+    retrieval_latency: float = pydantic.Field(description="The end-to-end latency for retrieval.")
     class_name: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/externally_stored_component.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/text_node_with_score.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from .text_node import TextNode
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class ExternallyStoredComponent(pydantic.BaseModel):
+class TextNodeWithScore(pydantic.BaseModel):
     """
-    Base schema model for BaseComponent classes used in the platform.
-    Comes with special serialization logic for types used commonly in platform codebase.
+    Same as NodeWithScore but type for node is a TextNode instead of BaseNode.
+    FastAPI doesn't accept abstract classes like BaseNode.
     """
 
-    id: str = pydantic.Field(description="The ID of the externally stored component.")
-    extra_path_prefix: str = pydantic.Field(description="The extra path prefix for the externally stored component.")
+    node: TextNode
+    score: typing.Optional[float]
     class_name: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/google_docs_reader.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/google_docs_reader.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/google_sheets_reader.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/google_sheets_reader.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/html_node_parser.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/html_node_parser.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/http_validation_error.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/hugging_face_inference_api_embedding.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/hugging_face_inference_api_embedding.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/json_node_parser.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/json_node_parser.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/keyword_extractor.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/keyword_extractor.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/llm.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/llm.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/llm_predictor.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/llm_predictor.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/loaded_file.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/loaded_file.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/loaded_file_managed_ingestion_execution.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/playground_job_record.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,38 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .etl_job_names import EtlJobNames
-from .loaded_file_managed_ingestion_execution_run_config_per_op_value import (
-    LoadedFileManagedIngestionExecutionRunConfigPerOpValue,
-)
+from .job_names import JobNames
 from .status_enum import StatusEnum
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class LoadedFileManagedIngestionExecution(pydantic.BaseModel):
+class PlaygroundJobRecord(pydantic.BaseModel):
     """
-    Schema for job that executes managed pipeline ingestion for a single loaded file.
+    Schema for a job that executes a playground pipeline.
     """
 
-    id: str = pydantic.Field(description="Unique identifier")
-    created_at: typing.Optional[dt.datetime] = pydantic.Field(description="Creation datetime")
-    updated_at: typing.Optional[dt.datetime] = pydantic.Field(description="Update datetime")
-    job_name: EtlJobNames
+    id: typing.Optional[str] = pydantic.Field(description="Unique identifier")
+    job_name: JobNames
     status: StatusEnum
     started_at: typing.Optional[dt.datetime]
     ended_at: typing.Optional[dt.datetime]
-    run_config_per_op: typing.Dict[str, LoadedFileManagedIngestionExecutionRunConfigPerOpValue] = pydantic.Field(
-        description="Run config that was given to the Dagster job"
+    created_at: typing.Optional[dt.datetime] = pydantic.Field(description="Creation datetime")
+    updated_at: typing.Optional[dt.datetime] = pydantic.Field(description="Update datetime")
+    partitions: typing.Dict[str, str] = pydantic.Field(description="The partitions for this execution.")
+    loaded_file_ids: typing.Optional[typing.List[str]] = pydantic.Field(
+        description="The IDs for the LoadedFiles this execution ran against."
     )
-    partitions: typing.Optional[typing.Dict[str, str]] = pydantic.Field(description="Partition information")
-    pipeline_id: str = pydantic.Field(description="The ID for the Pipeline this execution ran against.")
-    loaded_file_id: str = pydantic.Field(description="The ID for the LoadedFile this execution ran against.")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/loaded_file_payload.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/loaded_file_payload.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/managed_data_source_ingestion_job_config.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/parsing_job.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from .status_enum import StatusEnum
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class ManagedDataSourceIngestionJobConfig(pydantic.BaseModel):
-    """
-    Dagster op configuration for data-source-level managed ingestion job.
-    """
-
-    pipeline_id: str = pydantic.Field(description="Pipeline ID to run managed ingestion for")
-    data_source_id: str = pydantic.Field(description="Data source ID to run managed ingestion for")
+class ParsingJob(pydantic.BaseModel):
+    id: str
+    status: StatusEnum
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/managed_pipeline_ingestion_job_config.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/wikipedia_reader.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,20 +7,23 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class ManagedPipelineIngestionJobConfig(pydantic.BaseModel):
+class WikipediaReader(pydantic.BaseModel):
     """
-    Dagster op configuration for pipeline-level managed ingestion job.
+    Wikipedia reader.
+
+    Reads a page.
     """
 
-    pipeline_id: str = pydantic.Field(description="Pipeline ID to run managed ingestion for")
+    is_remote: typing.Optional[bool]
+    class_name: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/markdown_node_parser.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/markdown_node_parser.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/metadata_mode.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/metadata_mode.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/metric_result.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/metric_result.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/notion_page_reader.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/notion_page_reader.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/object_type.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/object_type.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/open_ai_embedding.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/open_ai_embedding.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/pg_vector_store.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/pg_vector_store.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/pinecone_vector_store.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/pinecone_vector_store.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/pipeline.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/pipeline.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from .configured_transformation_item import ConfiguredTransformationItem
 from .data_sink import DataSink
 from .data_source import DataSource
+from .managed_ingestion_status import ManagedIngestionStatus
 from .pipeline_type import PipelineType
 from .preset_retrieval_params import PresetRetrievalParams
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
@@ -32,14 +33,17 @@
     )
     managed_pipeline_id: typing.Optional[str] = pydantic.Field(
         description="The ID of the ManagedPipeline this playground pipeline is linked to."
     )
     preset_retrieval_parameters: typing.Optional[PresetRetrievalParams] = pydantic.Field(
         description="Preset retrieval parameters for the pipeline."
     )
+    managed_ingestion_status: typing.Optional[ManagedIngestionStatus] = pydantic.Field(
+        description="Status of Managed Ingestion."
+    )
     data_sources: typing.List[DataSource]
     data_sinks: typing.List[DataSink]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/pipeline_create.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/pipeline_create.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/pipeline_managed_ingestion_execution.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/sentence_splitter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .etl_job_names import EtlJobNames
-from .pipeline_managed_ingestion_execution_run_config_per_op_value import (
-    PipelineManagedIngestionExecutionRunConfigPerOpValue,
-)
-from .status_enum import StatusEnum
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class PipelineManagedIngestionExecution(pydantic.BaseModel):
+class SentenceSplitter(pydantic.BaseModel):
     """
-    Schema for job that executes managed pipeline ingestion over all data-sources linked to a pipeline.
+    Parse text with a preference for complete sentences.
+
+    In general, this class tries to keep sentences and paragraphs together. Therefore
+    compared to the original TokenTextSplitter, there are less likely to be
+    hanging sentences or parts of sentences at the end of the node chunk.
     """
 
-    id: str = pydantic.Field(description="Unique identifier")
-    created_at: typing.Optional[dt.datetime] = pydantic.Field(description="Creation datetime")
-    updated_at: typing.Optional[dt.datetime] = pydantic.Field(description="Update datetime")
-    job_name: EtlJobNames
-    status: StatusEnum
-    started_at: typing.Optional[dt.datetime]
-    ended_at: typing.Optional[dt.datetime]
-    run_config_per_op: typing.Dict[str, PipelineManagedIngestionExecutionRunConfigPerOpValue] = pydantic.Field(
-        description="Run config that was given to the Dagster job"
+    include_metadata: typing.Optional[bool] = pydantic.Field(
+        description="Whether or not to consider metadata when splitting."
+    )
+    include_prev_next_rel: typing.Optional[bool] = pydantic.Field(description="Include prev/next node relationships.")
+    callback_manager: typing.Optional[typing.Dict[str, typing.Any]]
+    chunk_size: typing.Optional[int] = pydantic.Field(description="The token chunk size for each chunk.")
+    chunk_overlap: typing.Optional[int] = pydantic.Field(description="The token overlap of each chunk when splitting.")
+    separator: typing.Optional[str] = pydantic.Field(description="Default separator for splitting into words")
+    paragraph_separator: typing.Optional[str] = pydantic.Field(description="Separator between paragraphs.")
+    secondary_chunking_regex: typing.Optional[str] = pydantic.Field(
+        description="Backup regex for splitting into sentences."
     )
-    partitions: typing.Optional[typing.Dict[str, str]] = pydantic.Field(description="Partition information")
-    pipeline_id: str = pydantic.Field(description="The ID for the Pipeline this execution ran against.")
+    class_name: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/pipeline_type.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/pipeline_type.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/preset_retrieval_params.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/preset_retrieval_params.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/project.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/project.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/project_create.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/project_create.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/pydantic_program_mode.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/pydantic_program_mode.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/qdrant_vector_store.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/qdrant_vector_store.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/questions_answered_extractor.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/questions_answered_extractor.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/reader_config.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/reader_config.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/related_node_info.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/related_node_info.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/retrieve_results.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/simple_web_page_reader.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .text_node_with_score import TextNodeWithScore
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class RetrieveResults(pydantic.BaseModel):
+class SimpleWebPageReader(pydantic.BaseModel):
     """
-    Schema for the result of an retrieval execution.
+    Simple web page reader.
+
+    Reads pages from the web.
+
+    Args:
+    html_to_text (bool): Whether to convert HTML to text.
+    Requires `html2text` package.
+    metadata_fn (Optional[Callable[[str], Dict]]): A function that takes in
+    a URL and returns a dictionary of metadata.
+    Default is None.
     """
 
-    pipeline_id: str = pydantic.Field(description="The ID of the pipeline that the query was retrieved against.")
-    retrieval_nodes: typing.List[TextNodeWithScore] = pydantic.Field(
-        description="The nodes retrieved by the pipeline for the given query."
-    )
-    retrieval_latency: float = pydantic.Field(description="The end-to-end latency for retrieval.")
+    is_remote: typing.Optional[bool]
+    html_to_text: bool
     class_name: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/rss_reader.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/rss_reader.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/run_transform_asset_config.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/simple_file_node_parser.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,27 +7,32 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class RunTransformAssetConfig(pydantic.BaseModel):
+class SimpleFileNodeParser(pydantic.BaseModel):
     """
-    Dagster asset configuration for run_transform asset.
+    Simple file node parser.
+
+    Splits a document loaded from a file into Nodes using logic based on the file type
+    automatically detects the NodeParser to use based on file type
+
+    Args:
+    include_metadata (bool): whether to include metadata in nodes
+    include_prev_next_rel (bool): whether to include prev/next relationships
     """
 
-    pipeline_id: str
-    configured_transformation_id: str
-    should_initiate_next_transform: typing.Optional[bool] = pydantic.Field(
-        description="Whether to kick of the job to run the next configured transformation in the pipeline after this one succeeds"
-    )
-    loaded_file_ids: typing.Optional[typing.List[str]] = pydantic.Field(
-        description="List of LoadedFile IDs to run the transform on. If None or empty, all LoadedFiles from connected data-sources will be used."
+    include_metadata: typing.Optional[bool] = pydantic.Field(
+        description="Whether or not to consider metadata when splitting."
     )
+    include_prev_next_rel: typing.Optional[bool] = pydantic.Field(description="Include prev/next node relationships.")
+    callback_manager: typing.Optional[typing.Dict[str, typing.Any]]
+    class_name: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/sentence_splitter.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/summary_extractor.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,50 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from .metadata_mode import MetadataMode
+from .summary_extractor_llm import SummaryExtractorLlm
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class SentenceSplitter(pydantic.BaseModel):
+class SummaryExtractor(pydantic.BaseModel):
     """
-    Parse text with a preference for complete sentences.
-
-    In general, this class tries to keep sentences and paragraphs together. Therefore
-    compared to the original TokenTextSplitter, there are less likely to be
-    hanging sentences or parts of sentences at the end of the node chunk.
+    Summary extractor. Node-level extractor with adjacent sharing.
+    Extracts `section_summary`, `prev_section_summary`, `next_section_summary`
+    metadata fields.
+
+    Args:
+    llm (Optional[LLM]): LLM
+    summaries (List[str]): list of summaries to extract: 'self', 'prev', 'next'
+    prompt_template (str): template for summary extraction
     """
 
-    include_metadata: typing.Optional[bool] = pydantic.Field(
-        description="Whether or not to consider metadata when splitting."
+    is_text_node_only: typing.Optional[bool]
+    show_progress: typing.Optional[bool] = pydantic.Field(description="Whether to show progress.")
+    metadata_mode: typing.Optional[MetadataMode] = pydantic.Field(
+        description="Metadata mode to use when reading nodes."
+    )
+    node_text_template: typing.Optional[str] = pydantic.Field(
+        description="Template to represent how node text is mixed with metadata text."
     )
-    include_prev_next_rel: typing.Optional[bool] = pydantic.Field(description="Include prev/next node relationships.")
-    callback_manager: typing.Optional[typing.Dict[str, typing.Any]]
-    chunk_size: typing.Optional[int] = pydantic.Field(description="The token chunk size for each chunk.")
-    chunk_overlap: typing.Optional[int] = pydantic.Field(description="The token overlap of each chunk when splitting.")
-    separator: typing.Optional[str] = pydantic.Field(description="Default separator for splitting into words")
-    paragraph_separator: typing.Optional[str] = pydantic.Field(description="Separator between paragraphs.")
-    secondary_chunking_regex: typing.Optional[str] = pydantic.Field(
-        description="Backup regex for splitting into sentences."
+    disable_template_rewrite: typing.Optional[bool] = pydantic.Field(description="Disable the node template rewrite.")
+    in_place: typing.Optional[bool] = pydantic.Field(description="Whether to process nodes in place.")
+    num_workers: typing.Optional[int] = pydantic.Field(
+        description="Number of workers to use for concurrent async processing."
     )
+    llm: SummaryExtractorLlm = pydantic.Field(description="The LLM to use for generation.")
+    summaries: typing.List[str] = pydantic.Field(description="List of summaries to extract: 'self', 'prev', 'next'")
+    prompt_template: typing.Optional[str] = pydantic.Field(description="Template to use when generating summaries.")
     class_name: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/simple_web_page_reader.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/trafilatura_web_reader.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,30 +7,24 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class SimpleWebPageReader(pydantic.BaseModel):
+class TrafilaturaWebReader(pydantic.BaseModel):
     """
-    Simple web page reader.
+    Trafilatura web page reader.
 
     Reads pages from the web.
-
-    Args:
-    html_to_text (bool): Whether to convert HTML to text.
-    Requires `html2text` package.
-    metadata_fn (Optional[Callable[[str], Dict]]): A function that takes in
-    a URL and returns a dictionary of metadata.
-    Default is None.
+    Requires the `trafilatura` package.
     """
 
     is_remote: typing.Optional[bool]
-    html_to_text: bool
+    error_on_missing: bool
     class_name: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/status_enum.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/status_enum.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/summary_extractor.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/title_extractor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from .metadata_mode import MetadataMode
-from .summary_extractor_llm import SummaryExtractorLlm
+from .title_extractor_llm import TitleExtractorLlm
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class SummaryExtractor(pydantic.BaseModel):
+class TitleExtractor(pydantic.BaseModel):
     """
-    Summary extractor. Node-level extractor with adjacent sharing.
-    Extracts `section_summary`, `prev_section_summary`, `next_section_summary`
-    metadata fields.
+    Title extractor. Useful for long documents. Extracts `document_title`
+    metadata field.
 
     Args:
     llm (Optional[LLM]): LLM
-    summaries (List[str]): list of summaries to extract: 'self', 'prev', 'next'
-    prompt_template (str): template for summary extraction
+    nodes (int): number of nodes from front to use for title extraction
+    node_template (str): template for node-level title clues extraction
+    combine_template (str): template for combining node-level clues into
+    a document-level title
     """
 
     is_text_node_only: typing.Optional[bool]
     show_progress: typing.Optional[bool] = pydantic.Field(description="Whether to show progress.")
     metadata_mode: typing.Optional[MetadataMode] = pydantic.Field(
         description="Metadata mode to use when reading nodes."
     )
@@ -34,17 +35,18 @@
         description="Template to represent how node text is mixed with metadata text."
     )
     disable_template_rewrite: typing.Optional[bool] = pydantic.Field(description="Disable the node template rewrite.")
     in_place: typing.Optional[bool] = pydantic.Field(description="Whether to process nodes in place.")
     num_workers: typing.Optional[int] = pydantic.Field(
         description="Number of workers to use for concurrent async processing."
     )
-    llm: SummaryExtractorLlm = pydantic.Field(description="The LLM to use for generation.")
-    summaries: typing.List[str] = pydantic.Field(description="List of summaries to extract: 'self', 'prev', 'next'")
-    prompt_template: typing.Optional[str] = pydantic.Field(description="Template to use when generating summaries.")
+    llm: TitleExtractorLlm = pydantic.Field(description="The LLM to use for generation.")
+    nodes: typing.Optional[int] = pydantic.Field(description="The number of nodes to extract titles from.")
+    node_template: typing.Optional[str] = pydantic.Field(description="The prompt template to extract titles with.")
+    combine_template: typing.Optional[str] = pydantic.Field(description="The prompt template to merge titles with.")
     class_name: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/supported_eval_llm_model.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/supported_eval_llm_model.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/supported_eval_llm_model_names.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/supported_eval_llm_model_names.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/text_node.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/text_node.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/text_node_with_score.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/youtube_transcript_reader.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .text_node import TextNode
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class TextNodeWithScore(pydantic.BaseModel):
+class YoutubeTranscriptReader(pydantic.BaseModel):
     """
-    Same as NodeWithScore but type for node is a TextNode instead of BaseNode.
-    FastAPI doesn't accept abstract classes like BaseNode.
+    Youtube Transcript reader.
     """
 
-    node: TextNode
-    score: typing.Optional[float]
+    is_remote: typing.Optional[bool]
+    languages: typing.Optional[typing.List[typing.Any]]
     class_name: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/token_text_splitter.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/token_text_splitter.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/trafilatura_web_reader.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/parsing_job_text_result.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,25 +7,16 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class TrafilaturaWebReader(pydantic.BaseModel):
-    """
-    Trafilatura web page reader.
-
-    Reads pages from the web.
-    Requires the `trafilatura` package.
-    """
-
-    is_remote: typing.Optional[bool]
-    error_on_missing: bool
-    class_name: typing.Optional[str]
+class ParsingJobTextResult(pydantic.BaseModel):
+    text: str = pydantic.Field(description="The text result of the parsing job")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/transformation_category_names.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/transformation_category_names.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/twitter_tweet_reader.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/twitter_tweet_reader.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/validation_error.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/weaviate_vector_store.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/weaviate_vector_store.py`

 * *Files identical despite different names*

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/wikipedia_reader.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/parsing_job_markdown_result.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,23 +7,16 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class WikipediaReader(pydantic.BaseModel):
-    """
-    Wikipedia reader.
-
-    Reads a page.
-    """
-
-    is_remote: typing.Optional[bool]
-    class_name: typing.Optional[str]
+class ParsingJobMarkdownResult(pydantic.BaseModel):
+    markdown: str = pydantic.Field(description="The markdown result of the parsing job")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `llamaindex_py_client-0.1.8/llama_index_client/types/youtube_transcript_reader.py` & `llamaindex_py_client-0.1.9/llama_index_client/types/data_source_load_job_record.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from .job_names import JobNames
+from .status_enum import StatusEnum
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class YoutubeTranscriptReader(pydantic.BaseModel):
+class DataSourceLoadJobRecord(pydantic.BaseModel):
     """
-    Youtube Transcript reader.
+    Schema for job that loads from a data source.
     """
 
-    is_remote: typing.Optional[bool]
-    languages: typing.Optional[typing.List[typing.Any]]
-    class_name: typing.Optional[str]
+    id: typing.Optional[str] = pydantic.Field(description="Unique identifier")
+    job_name: typing.Optional[JobNames]
+    status: StatusEnum
+    started_at: typing.Optional[dt.datetime]
+    ended_at: typing.Optional[dt.datetime]
+    created_at: typing.Optional[dt.datetime] = pydantic.Field(description="Creation datetime")
+    updated_at: typing.Optional[dt.datetime] = pydantic.Field(description="Update datetime")
+    partitions: typing.Dict[str, str] = pydantic.Field(description="The partitions for this execution.")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `llamaindex_py_client-0.1.8/PKG-INFO` & `llamaindex_py_client-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llamaindex-py-client
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Logan Markewich
 Author-email: logan@runllama.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

