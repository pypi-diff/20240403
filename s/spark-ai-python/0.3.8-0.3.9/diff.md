# Comparing `tmp/spark_ai_python-0.3.8.tar.gz` & `tmp/spark_ai_python-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_ai_python-0.3.8.tar", max compression
+gzip compressed data, was "spark_ai_python-0.3.9.tar", max compression
```

## Comparing `spark_ai_python-0.3.8.tar` & `spark_ai_python-0.3.9.tar`

### file list

```diff
@@ -1,182 +1,183 @@
--rw-r--r--   0        0        0     1064 2023-04-29 02:30:03.382229 spark_ai_python-0.3.8/LICENSE
--rw-r--r--   0        0        0    15249 2024-03-27 11:34:00.880941 spark_ai_python-0.3.8/README.md
--rw-r--r--   0        0        0     1131 2024-03-27 13:51:04.093990 spark_ai_python-0.3.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-23 01:36:47.370166 spark_ai_python-0.3.8/sparkai/__init__.py
--rw-r--r--   0        0        0     4384 2024-02-23 02:52:25.805091 spark_ai_python-0.3.8/sparkai/_client.py
--rw-r--r--   0        0        0     1762 2023-09-12 02:27:21.029637 spark_ai_python-0.3.8/sparkai/api_resources/__init__.py
--rw-r--r--   0        0        0     1148 2024-02-23 02:40:56.369216 spark_ai_python-0.3.8/sparkai/api_resources/chat/__init__.py
--rw-r--r--   0        0        0      450 2024-02-23 02:41:21.281487 spark_ai_python-0.3.8/sparkai/api_resources/chat/chat.py
--rw-r--r--   0        0        0     3942 2024-02-23 02:42:05.172035 spark_ai_python-0.3.8/sparkai/api_resources/chat/completions.py
--rw-r--r--   0        0        0     4861 2024-02-02 05:46:52.629871 spark_ai_python-0.3.8/sparkai/api_resources/chat_completion.py
--rw-r--r--   0        0        0     3083 2024-03-26 01:49:02.917191 spark_ai_python-0.3.8/sparkai/constants.py
--rw-r--r--   0        0        0    58962 2024-03-26 01:49:02.917678 spark_ai_python-0.3.8/sparkai/conversation/__init__.py
--rw-r--r--   0        0        0     1151 2024-02-23 02:42:42.777600 spark_ai_python-0.3.8/sparkai/core/__init__.py
--rw-r--r--   0        0        0     1001 2024-03-14 02:00:19.515460 spark_ai_python-0.3.8/sparkai/core/_api/__init__.py
--rw-r--r--   0        0        0     9440 2024-03-14 02:01:12.178429 spark_ai_python-0.3.8/sparkai/core/_api/beta_decorator.py
--rw-r--r--   0        0        0    14283 2024-03-14 03:21:46.854366 spark_ai_python-0.3.8/sparkai/core/_api/deprecation.py
--rw-r--r--   0        0        0      664 2024-03-14 06:46:24.360366 spark_ai_python-0.3.8/sparkai/core/_api/internal.py
--rw-r--r--   0        0        0      988 2024-03-14 06:46:24.388394 spark_ai_python-0.3.8/sparkai/core/_api/path.py
--rw-r--r--   0        0        0     1554 2024-02-23 02:43:23.871624 spark_ai_python-0.3.8/sparkai/core/_base_api.py
--rw-r--r--   0        0        0      720 2024-03-14 03:44:52.843347 spark_ai_python-0.3.8/sparkai/core/caches.py
--rw-r--r--   0        0        0     1394 2024-03-14 23:42:45.322294 spark_ai_python-0.3.8/sparkai/core/callbacks/__init__.py
--rw-r--r--   0        0        0    17195 2024-03-14 06:46:24.426429 spark_ai_python-0.3.8/sparkai/core/callbacks/base.py
--rw-r--r--   0        0        0    38599 2024-03-20 14:50:58.232777 spark_ai_python-0.3.8/sparkai/core/callbacks/manager.py
--rw-r--r--   0        0        0     1742 2024-03-14 04:49:02.723919 spark_ai_python-0.3.8/sparkai/core/callbacks/stdout.py
--rw-r--r--   0        0        0     2134 2024-03-14 04:49:43.727566 spark_ai_python-0.3.8/sparkai/core/callbacks/streaming_stdout.py
--rw-r--r--   0        0        0     7376 2024-03-14 06:46:24.402412 spark_ai_python-0.3.8/sparkai/core/globals/__init__.py
--rw-r--r--   0        0        0      516 2024-03-14 03:31:29.182052 spark_ai_python-0.3.8/sparkai/core/language_models/__init__.py
--rw-r--r--   0        0        0    10736 2024-03-14 04:49:53.923298 spark_ai_python-0.3.8/sparkai/core/language_models/base.py
--rw-r--r--   0        0        0    29296 2024-03-14 16:48:12.298618 spark_ai_python-0.3.8/sparkai/core/language_models/chat_models.py
--rw-r--r--   0        0        0    41216 2024-03-14 06:46:24.368076 spark_ai_python-0.3.8/sparkai/core/language_models/llms.py
--rw-r--r--   0        0        0      255 2024-03-14 03:20:36.390329 spark_ai_python-0.3.8/sparkai/core/load/__init__.py
--rw-r--r--   0        0        0     1172 2024-03-14 01:50:26.779862 spark_ai_python-0.3.8/sparkai/core/load/dump.py
--rw-r--r--   0        0        0     5413 2024-03-14 06:46:24.404251 spark_ai_python-0.3.8/sparkai/core/load/load.py
--rw-r--r--   0        0        0    25671 2024-03-14 06:46:24.377304 spark_ai_python-0.3.8/sparkai/core/load/mapping.py
--rw-r--r--   0        0        0     6241 2024-03-14 06:46:24.420899 spark_ai_python-0.3.8/sparkai/core/load/serializable.py
--rw-r--r--   0        0        0     8654 2024-03-14 16:05:33.697435 spark_ai_python-0.3.8/sparkai/core/messages/__init__.py
--rw-r--r--   0        0        0     1724 2024-03-14 03:19:59.153486 spark_ai_python-0.3.8/sparkai/core/messages/ai.py
--rw-r--r--   0        0        0     6952 2024-03-14 03:19:59.155127 spark_ai_python-0.3.8/sparkai/core/messages/base.py
--rw-r--r--   0        0        0     2017 2024-03-14 03:19:59.150666 spark_ai_python-0.3.8/sparkai/core/messages/chat.py
--rw-r--r--   0        0        0     3402 2024-03-14 16:41:51.672975 spark_ai_python-0.3.8/sparkai/core/messages/function.py
--rw-r--r--   0        0        0     1063 2024-03-14 03:19:59.158213 spark_ai_python-0.3.8/sparkai/core/messages/human.py
--rw-r--r--   0        0        0     1016 2024-03-14 03:19:59.156822 spark_ai_python-0.3.8/sparkai/core/messages/system.py
--rw-r--r--   0        0        0     1723 2024-03-14 03:19:59.148824 spark_ai_python-0.3.8/sparkai/core/messages/tool.py
--rw-r--r--   0        0        0      472 2024-03-14 01:48:00.771129 spark_ai_python-0.3.8/sparkai/core/outputs/__init__.py
--rw-r--r--   0        0        0     2596 2024-03-14 06:46:24.353899 spark_ai_python-0.3.8/sparkai/core/outputs/chat_generation.py
--rw-r--r--   0        0        0      507 2024-03-14 01:45:58.509890 spark_ai_python-0.3.8/sparkai/core/outputs/chat_result.py
--rw-r--r--   0        0        0     1815 2024-03-14 06:46:24.370326 spark_ai_python-0.3.8/sparkai/core/outputs/generation.py
--rw-r--r--   0        0        0     2442 2024-03-14 01:47:24.446293 spark_ai_python-0.3.8/sparkai/core/outputs/llm_result.py
--rw-r--r--   0        0        0      293 2024-03-14 01:47:32.585459 spark_ai_python-0.3.8/sparkai/core/outputs/run_info.py
--rw-r--r--   0        0        0     3367 2024-03-14 06:46:24.407495 spark_ai_python-0.3.8/sparkai/core/prompt_values.py
--rw-r--r--   0        0        0     2581 2024-02-02 05:35:24.232000 spark_ai_python-0.3.8/sparkai/core/prompts/__init__.py
--rw-r--r--   0        0        0     8953 2024-03-14 06:46:24.398978 spark_ai_python-0.3.8/sparkai/core/prompts/base.py
--rw-r--r--   0        0        0    33263 2024-03-14 06:46:24.424427 spark_ai_python-0.3.8/sparkai/core/prompts/chat.py
--rw-r--r--   0        0        0    11979 2024-02-02 05:35:24.233000 spark_ai_python-0.3.8/sparkai/core/prompts/few_shot.py
--rw-r--r--   0        0        0     5821 2024-03-14 06:46:24.383831 spark_ai_python-0.3.8/sparkai/core/prompts/few_shot_with_templates.py
--rw-r--r--   0        0        0     2656 2024-02-02 05:35:24.233000 spark_ai_python-0.3.8/sparkai/core/prompts/image.py
--rw-r--r--   0        0        0     6357 2024-02-02 05:35:24.233000 spark_ai_python-0.3.8/sparkai/core/prompts/loading.py
--rw-r--r--   0        0        0     2502 2024-03-14 06:46:24.357524 spark_ai_python-0.3.8/sparkai/core/prompts/pipeline.py
--rw-r--r--   0        0        0     9837 2024-03-14 06:46:24.344416 spark_ai_python-0.3.8/sparkai/core/prompts/prompt.py
--rw-r--r--   0        0        0     6289 2024-03-14 06:46:24.372890 spark_ai_python-0.3.8/sparkai/core/prompts/string.py
--rw-r--r--   0        0        0      927 2024-02-02 05:35:24.234000 spark_ai_python-0.3.8/sparkai/core/pydantic_v1/__init__.py
--rw-r--r--   0        0        0      134 2024-02-02 05:35:24.234000 spark_ai_python-0.3.8/sparkai/core/pydantic_v1/dataclasses.py
--rw-r--r--   0        0        0      120 2024-02-02 05:35:24.234000 spark_ai_python-0.3.8/sparkai/core/pydantic_v1/main.py
--rw-r--r--   0        0        0     2170 2024-03-14 04:50:57.946244 spark_ai_python-0.3.8/sparkai/core/runnables/__init__.py
--rw-r--r--   0        0        0   163501 2024-03-14 06:46:24.395202 spark_ai_python-0.3.8/sparkai/core/runnables/base.py
--rw-r--r--   0        0        0    14390 2024-03-14 06:46:24.418771 spark_ai_python-0.3.8/sparkai/core/runnables/branch.py
--rw-r--r--   0        0        0    16983 2024-03-14 04:50:21.132453 spark_ai_python-0.3.8/sparkai/core/runnables/config.py
--rw-r--r--   0        0        0    16043 2024-03-14 06:46:24.363487 spark_ai_python-0.3.8/sparkai/core/runnables/configurable.py
--rw-r--r--   0        0        0    19821 2024-03-14 06:46:24.400959 spark_ai_python-0.3.8/sparkai/core/runnables/fallbacks.py
--rw-r--r--   0        0        0     5036 2024-03-14 04:50:45.282970 spark_ai_python-0.3.8/sparkai/core/runnables/graph.py
--rw-r--r--   0        0        0     8741 2024-02-02 05:35:24.235000 spark_ai_python-0.3.8/sparkai/core/runnables/graph_draw.py
--rw-r--r--   0        0        0    19025 2024-03-14 06:46:24.397392 spark_ai_python-0.3.8/sparkai/core/runnables/history.py
--rw-r--r--   0        0        0    21904 2024-03-14 06:46:24.381266 spark_ai_python-0.3.8/sparkai/core/runnables/passthrough.py
--rw-r--r--   0        0        0    11959 2024-03-14 06:46:24.411696 spark_ai_python-0.3.8/sparkai/core/runnables/retry.py
--rw-r--r--   0        0        0     6272 2024-03-14 06:46:24.409736 spark_ai_python-0.3.8/sparkai/core/runnables/router.py
--rw-r--r--   0        0        0     4399 2024-02-02 05:35:24.236000 spark_ai_python-0.3.8/sparkai/core/runnables/schema.py
--rw-r--r--   0        0        0    14836 2024-03-14 04:50:36.551170 spark_ai_python-0.3.8/sparkai/core/runnables/utils.py
--rw-r--r--   0        0        0    32988 2024-03-14 16:21:59.432072 spark_ai_python-0.3.8/sparkai/core/tools.py
--rw-r--r--   0        0        0      828 2024-03-20 14:47:11.220780 spark_ai_python-0.3.8/sparkai/core/tracers/__init__.py
--rw-r--r--   0        0        0    23849 2024-03-14 05:22:42.111248 spark_ai_python-0.3.8/sparkai/core/tracers/base.py
--rw-r--r--   0        0        0     7606 2024-03-14 05:20:13.688094 spark_ai_python-0.3.8/sparkai/core/tracers/context.py
--rw-r--r--   0        0        0     8208 2024-03-14 05:20:13.693996 spark_ai_python-0.3.8/sparkai/core/tracers/evaluation.py
--rw-r--r--   0        0        0     8931 2024-03-14 05:24:28.823215 spark_ai_python-0.3.8/sparkai/core/tracers/langchain.py
--rw-r--r--   0        0        0     7716 2024-03-14 06:46:24.349501 spark_ai_python-0.3.8/sparkai/core/tracers/langchain_v1.py
--rw-r--r--   0        0        0    21451 2024-03-14 05:20:13.691027 spark_ai_python-0.3.8/sparkai/core/tracers/log_stream.py
--rw-r--r--   0        0        0     3933 2024-03-14 05:18:56.159000 spark_ai_python-0.3.8/sparkai/core/tracers/memory_stream.py
--rw-r--r--   0        0        0     1698 2024-03-14 05:20:13.686773 spark_ai_python-0.3.8/sparkai/core/tracers/root_listeners.py
--rw-r--r--   0        0        0     1526 2024-03-14 05:20:13.696287 spark_ai_python-0.3.8/sparkai/core/tracers/run_collector.py
--rw-r--r--   0        0        0     2838 2024-03-20 14:46:11.736409 spark_ai_python-0.3.8/sparkai/core/tracers/schemas.py
--rw-r--r--   0        0        0     6180 2024-03-14 05:20:13.685167 spark_ai_python-0.3.8/sparkai/core/tracers/stdout.py
--rw-r--r--   0        0        0     1270 2024-03-14 03:12:55.110592 spark_ai_python-0.3.8/sparkai/core/utils/__init__.py
--rw-r--r--   0        0        0     1616 2024-02-02 05:35:24.238000 spark_ai_python-0.3.8/sparkai/core/utils/_merge.py
--rw-r--r--   0        0        0     7198 2024-02-02 05:35:24.238000 spark_ai_python-0.3.8/sparkai/core/utils/aiter.py
--rw-r--r--   0        0        0     1297 2024-02-02 05:35:24.238000 spark_ai_python-0.3.8/sparkai/core/utils/env.py
--rw-r--r--   0        0        0      907 2024-02-02 05:35:24.238000 spark_ai_python-0.3.8/sparkai/core/utils/formatting.py
--rw-r--r--   0        0        0    10334 2024-03-15 01:32:08.108678 spark_ai_python-0.3.8/sparkai/core/utils/function_calling.py
--rw-r--r--   0        0        0     3090 2024-02-02 05:35:24.238000 spark_ai_python-0.3.8/sparkai/core/utils/html.py
--rw-r--r--   0        0        0      423 2024-02-02 05:35:24.238000 spark_ai_python-0.3.8/sparkai/core/utils/image.py
--rw-r--r--   0        0        0     1289 2024-02-02 05:35:24.238000 spark_ai_python-0.3.8/sparkai/core/utils/input.py
--rw-r--r--   0        0        0      139 2024-02-02 05:35:24.239000 spark_ai_python-0.3.8/sparkai/core/utils/interactive_env.py
--rw-r--r--   0        0        0     5822 2024-02-02 05:35:24.239000 spark_ai_python-0.3.8/sparkai/core/utils/iter.py
--rw-r--r--   0        0        0     2318 2024-02-02 05:35:24.239000 spark_ai_python-0.3.8/sparkai/core/utils/json_schema.py
--rw-r--r--   0        0        0     2011 2024-02-02 05:35:24.239000 spark_ai_python-0.3.8/sparkai/core/utils/loading.py
--rw-r--r--   0        0        0      301 2024-02-02 05:35:24.239000 spark_ai_python-0.3.8/sparkai/core/utils/pydantic.py
--rw-r--r--   0        0        0      908 2024-02-02 05:35:24.239000 spark_ai_python-0.3.8/sparkai/core/utils/strings.py
--rw-r--r--   0        0        0     6158 2024-03-14 01:47:13.885399 spark_ai_python-0.3.8/sparkai/core/utils/utils.py
--rw-r--r--   0        0        0      374 2023-05-03 13:09:38.934327 spark_ai_python-0.3.8/sparkai/deprecation.py
--rw-r--r--   0        0        0     1151 2024-02-02 05:10:31.290500 spark_ai_python-0.3.8/sparkai/depreciated/__init__.py
--rw-r--r--   0        0        0     1151 2024-02-02 05:10:31.287607 spark_ai_python-0.3.8/sparkai/depreciated/client/__init__.py
--rw-r--r--   0        0        0     3670 2024-03-14 15:36:22.936130 spark_ai_python-0.3.8/sparkai/depreciated/client/llm.py
--rw-r--r--   0        0        0     2438 2024-03-14 06:46:24.414331 spark_ai_python-0.3.8/sparkai/depreciated/client/sample_langchain_spark.py
--rw-r--r--   0        0        0     1151 2024-02-02 05:14:30.402301 spark_ai_python-0.3.8/sparkai/depreciated/service/__init__.py
--rw-r--r--   0        0        0     2495 2024-03-14 06:46:24.386756 spark_ai_python-0.3.8/sparkai/depreciated/service/api_server.py
--rw-r--r--   0        0        0     5104 2024-02-02 05:15:10.571713 spark_ai_python-0.3.8/sparkai/depreciated/service/spark_ws.py
--rw-r--r--   0        0        0     1952 2023-05-02 05:58:50.610144 spark_ai_python-0.3.8/sparkai/errors/__init__.py
--rw-r--r--   0        0        0     1907 2024-03-14 05:22:19.678605 spark_ai_python-0.3.8/sparkai/exceptions.py
--rw-r--r--   0        0        0     1151 2024-03-27 09:25:47.330409 spark_ai_python-0.3.8/sparkai/frameworks/__init__.py
--rw-r--r--   0        0        0     9018 2024-03-27 13:54:49.802292 spark_ai_python-0.3.8/sparkai/frameworks/llama_index/__init__.py
--rw-r--r--   0        0        0     1256 2023-04-29 01:49:30.738000 spark_ai_python-0.3.8/sparkai/http_retry/__init__.py
--rw-r--r--   0        0        0     2647 2023-04-29 02:52:26.276574 spark_ai_python-0.3.8/sparkai/http_retry/async_handler.py
--rw-r--r--   0        0        0     2970 2023-04-29 02:52:26.274822 spark_ai_python-0.3.8/sparkai/http_retry/builtin_async_handlers.py
--rw-r--r--   0        0        0     2884 2023-04-29 02:52:26.279895 spark_ai_python-0.3.8/sparkai/http_retry/builtin_handlers.py
--rw-r--r--   0        0        0     1622 2023-04-29 01:49:30.738000 spark_ai_python-0.3.8/sparkai/http_retry/builtin_interval_calculators.py
--rw-r--r--   0        0        0     2455 2023-04-29 02:52:26.278033 spark_ai_python-0.3.8/sparkai/http_retry/handler.py
--rw-r--r--   0        0        0      450 2023-04-29 01:49:30.738000 spark_ai_python-0.3.8/sparkai/http_retry/interval_calculator.py
--rw-r--r--   0        0        0      597 2023-04-29 01:49:30.738000 spark_ai_python-0.3.8/sparkai/http_retry/jitter.py
--rw-r--r--   0        0        0     1035 2023-04-29 01:49:30.738000 spark_ai_python-0.3.8/sparkai/http_retry/request.py
--rw-r--r--   0        0        0      639 2023-04-29 01:49:30.738000 spark_ai_python-0.3.8/sparkai/http_retry/response.py
--rw-r--r--   0        0        0      570 2023-04-29 01:49:30.738000 spark_ai_python-0.3.8/sparkai/http_retry/state.py
--rw-r--r--   0        0        0     1151 2024-02-02 09:55:21.275283 spark_ai_python-0.3.8/sparkai/llm/__init__.py
--rw-r--r--   0        0        0    18815 2024-03-26 01:45:58.539209 spark_ai_python-0.3.8/sparkai/llm/llm.py
--rw-r--r--   0        0        0     1151 2023-07-23 12:42:01.813357 spark_ai_python-0.3.8/sparkai/log/__init__.py
--rw-r--r--   0        0        0     3060 2024-02-02 05:46:52.625440 spark_ai_python-0.3.8/sparkai/log/logger.py
--rw-r--r--   0        0        0     1088 2023-04-29 07:37:03.991801 spark_ai_python-0.3.8/sparkai/memory/__init__.py
--rw-r--r--   0        0        0     3065 2023-04-29 07:35:27.052139 spark_ai_python-0.3.8/sparkai/memory/buffer.py
--rw-r--r--   0        0        0     1143 2023-04-29 07:32:35.289915 spark_ai_python-0.3.8/sparkai/memory/buffer_window.py
--rw-r--r--   0        0        0     1558 2023-04-29 07:30:52.099436 spark_ai_python-0.3.8/sparkai/memory/chat_memory.py
--rw-r--r--   0        0        0      474 2023-04-29 07:21:51.986161 spark_ai_python-0.3.8/sparkai/memory/chat_message_histories/__init__.py
--rw-r--r--   0        0        0     2590 2023-04-29 07:21:51.994679 spark_ai_python-0.3.8/sparkai/memory/chat_message_histories/dynamodb.py
--rw-r--r--   0        0        0     1570 2023-04-29 07:21:51.990773 spark_ai_python-0.3.8/sparkai/memory/chat_message_histories/file.py
--rw-r--r--   0        0        0      548 2023-04-29 07:21:51.989452 spark_ai_python-0.3.8/sparkai/memory/chat_message_histories/in_memory.py
--rw-r--r--   0        0        0     2753 2023-04-29 07:21:51.988132 spark_ai_python-0.3.8/sparkai/memory/chat_message_histories/postgres.py
--rw-r--r--   0        0        0     2047 2023-04-29 07:21:51.991910 spark_ai_python-0.3.8/sparkai/memory/chat_message_histories/redis.py
--rw-r--r--   0        0        0     1489 2023-04-29 07:30:52.110734 spark_ai_python-0.3.8/sparkai/memory/combined.py
--rw-r--r--   0        0        0      787 2023-04-29 07:30:52.102790 spark_ai_python-0.3.8/sparkai/memory/readonly.py
--rw-r--r--   0        0        0      762 2023-04-29 07:30:52.103685 spark_ai_python-0.3.8/sparkai/memory/simple.py
--rw-r--r--   0        0        0     1862 2023-04-29 07:31:29.143884 spark_ai_python-0.3.8/sparkai/memory/token_buffer.py
--rw-r--r--   0        0        0      510 2023-04-29 07:30:52.104836 spark_ai_python-0.3.8/sparkai/memory/utils.py
--rw-r--r--   0        0        0     1046 2024-03-14 03:17:21.191832 spark_ai_python-0.3.8/sparkai/messages.py
--rw-r--r--   0        0        0     2039 2023-05-03 13:10:19.932620 spark_ai_python-0.3.8/sparkai/models/__init__.py
--rw-r--r--   0        0        0     3911 2023-05-03 12:39:55.387507 spark_ai_python-0.3.8/sparkai/models/basic_objects.py
--rw-r--r--   0        0        0     4945 2023-08-13 08:28:00.532036 spark_ai_python-0.3.8/sparkai/models/chat/__init__.py
--rw-r--r--   0        0        0     1384 2023-05-09 07:13:52.048866 spark_ai_python-0.3.8/sparkai/prompts/classification/__init__.py
--rw-r--r--   0        0        0      821 2023-04-29 01:49:30.743000 spark_ai_python-0.3.8/sparkai/proxy_env_variable_loader.py
--rw-r--r--   0        0        0    11977 2023-05-02 02:56:04.982300 spark_ai_python-0.3.8/sparkai/schema.py
--rw-r--r--   0        0        0     1151 2024-03-26 01:49:02.917906 spark_ai_python-0.3.8/sparkai/serve/__init__.py
--rw-r--r--   0        0        0    13061 2024-03-26 01:49:02.918125 spark_ai_python-0.3.8/sparkai/serve/api_provider.py
--rw-r--r--   0        0        0     7020 2024-03-26 08:23:39.323316 spark_ai_python-0.3.8/sparkai/serve/base_model.py
--rw-r--r--   0        0        0    13225 2024-03-26 01:49:02.918454 spark_ai_python-0.3.8/sparkai/serve/controller.py
--rw-r--r--   0        0        0    29007 2024-03-26 01:49:02.918709 spark_ai_python-0.3.8/sparkai/serve/gradio_web_server.py
--rw-r--r--   0        0        0     1151 2024-03-26 01:49:02.918858 spark_ai_python-0.3.8/sparkai/serve/model/__init__.py
--rw-r--r--   0        0        0     5561 2024-03-26 01:49:02.919011 spark_ai_python-0.3.8/sparkai/serve/model/model_adapter.py
--rw-r--r--   0        0        0    18798 2024-03-26 01:49:02.919217 spark_ai_python-0.3.8/sparkai/serve/model/model_registry.py
--rw-r--r--   0        0        0    12951 2024-03-26 01:49:02.919401 spark_ai_python-0.3.8/sparkai/serve/model_worker.py
--rw-r--r--   0        0        0    11895 2024-03-26 01:49:02.919593 spark_ai_python-0.3.8/sparkai/serve/utils/__init__.py
--rw-r--r--   0        0        0     1154 2023-07-23 01:18:08.275512 spark_ai_python-0.3.8/sparkai/socket_mode/__init__.py
--rw-r--r--   0        0        0     5472 2023-08-14 01:40:39.883803 spark_ai_python-0.3.8/sparkai/socket_mode/client.py
--rw-r--r--   0        0        0      907 2023-04-29 01:49:30.745000 spark_ai_python-0.3.8/sparkai/socket_mode/interval_runner.py
--rw-r--r--   0        0        0      525 2023-04-29 02:36:07.360120 spark_ai_python-0.3.8/sparkai/socket_mode/listeners.py
--rw-r--r--   0        0        0     1989 2023-04-29 02:36:07.370555 spark_ai_python-0.3.8/sparkai/socket_mode/request.py
--rw-r--r--   0        0        0      878 2023-04-29 02:36:07.363593 spark_ai_python-0.3.8/sparkai/socket_mode/response.py
--rw-r--r--   0        0        0    21111 2023-07-23 01:49:38.590155 spark_ai_python-0.3.8/sparkai/socket_mode/websocket_client/__init__.py
--rw-r--r--   0        0        0     1802 2024-03-13 07:45:20.129308 spark_ai_python-0.3.8/sparkai/spark_proxy/generate_message.py
--rw-r--r--   0        0        0     1957 2024-03-13 07:45:20.129475 spark_ai_python-0.3.8/sparkai/spark_proxy/generate_stream.py
--rw-r--r--   0        0        0      134 2024-03-13 06:53:32.303669 spark_ai_python-0.3.8/sparkai/spark_proxy/main.py
--rw-r--r--   0        0        0     2866 2024-03-13 07:45:20.129645 spark_ai_python-0.3.8/sparkai/spark_proxy/openai_types.py
--rw-r--r--   0        0        0     3453 2024-03-13 08:47:52.452083 spark_ai_python-0.3.8/sparkai/spark_proxy/server.py
--rw-r--r--   0        0        0     3815 2024-03-24 10:16:30.908132 spark_ai_python-0.3.8/sparkai/spark_proxy/spark_api.py
--rw-r--r--   0        0        0     2052 2024-03-13 06:43:49.970481 spark_ai_python-0.3.8/sparkai/spark_proxy/spark_auth.py
--rw-r--r--   0        0        0       95 2024-03-25 12:03:42.504504 spark_ai_python-0.3.8/sparkai/version.py
--rw-r--r--   0        0        0     1208 2023-04-29 03:12:25.029956 spark_ai_python-0.3.8/sparkai/xf_util.py
--rw-r--r--   0        0        0    16267 1970-01-01 00:00:00.000000 spark_ai_python-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-29 02:30:03.382229 spark_ai_python-0.3.9/LICENSE
+-rw-r--r--   0        0        0    15249 2024-03-27 11:34:00.880941 spark_ai_python-0.3.9/README.md
+-rw-r--r--   0        0        0     1215 2024-03-28 10:20:00.382881 spark_ai_python-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-23 01:36:47.370166 spark_ai_python-0.3.9/sparkai/__init__.py
+-rw-r--r--   0        0        0     4384 2024-02-23 02:52:25.805091 spark_ai_python-0.3.9/sparkai/_client.py
+-rw-r--r--   0        0        0     1762 2023-09-12 02:27:21.029637 spark_ai_python-0.3.9/sparkai/api_resources/__init__.py
+-rw-r--r--   0        0        0     1148 2024-02-23 02:40:56.369216 spark_ai_python-0.3.9/sparkai/api_resources/chat/__init__.py
+-rw-r--r--   0        0        0      450 2024-02-23 02:41:21.281487 spark_ai_python-0.3.9/sparkai/api_resources/chat/chat.py
+-rw-r--r--   0        0        0     3942 2024-02-23 02:42:05.172035 spark_ai_python-0.3.9/sparkai/api_resources/chat/completions.py
+-rw-r--r--   0        0        0     4861 2024-02-02 05:46:52.629871 spark_ai_python-0.3.9/sparkai/api_resources/chat_completion.py
+-rw-r--r--   0        0        0     3083 2024-03-26 01:49:02.917191 spark_ai_python-0.3.9/sparkai/constants.py
+-rw-r--r--   0        0        0    58962 2024-03-26 01:49:02.917678 spark_ai_python-0.3.9/sparkai/conversation/__init__.py
+-rw-r--r--   0        0        0     1151 2024-02-23 02:42:42.777600 spark_ai_python-0.3.9/sparkai/core/__init__.py
+-rw-r--r--   0        0        0     1001 2024-03-14 02:00:19.515460 spark_ai_python-0.3.9/sparkai/core/_api/__init__.py
+-rw-r--r--   0        0        0     9440 2024-03-14 02:01:12.178429 spark_ai_python-0.3.9/sparkai/core/_api/beta_decorator.py
+-rw-r--r--   0        0        0    14283 2024-03-14 03:21:46.854366 spark_ai_python-0.3.9/sparkai/core/_api/deprecation.py
+-rw-r--r--   0        0        0      664 2024-03-14 06:46:24.360366 spark_ai_python-0.3.9/sparkai/core/_api/internal.py
+-rw-r--r--   0        0        0      988 2024-03-14 06:46:24.388394 spark_ai_python-0.3.9/sparkai/core/_api/path.py
+-rw-r--r--   0        0        0     1554 2024-02-23 02:43:23.871624 spark_ai_python-0.3.9/sparkai/core/_base_api.py
+-rw-r--r--   0        0        0      720 2024-03-14 03:44:52.843347 spark_ai_python-0.3.9/sparkai/core/caches.py
+-rw-r--r--   0        0        0     1394 2024-03-14 23:42:45.322294 spark_ai_python-0.3.9/sparkai/core/callbacks/__init__.py
+-rw-r--r--   0        0        0    17195 2024-03-14 06:46:24.426429 spark_ai_python-0.3.9/sparkai/core/callbacks/base.py
+-rw-r--r--   0        0        0    38599 2024-03-20 14:50:58.232777 spark_ai_python-0.3.9/sparkai/core/callbacks/manager.py
+-rw-r--r--   0        0        0     1742 2024-03-14 04:49:02.723919 spark_ai_python-0.3.9/sparkai/core/callbacks/stdout.py
+-rw-r--r--   0        0        0     2134 2024-03-14 04:49:43.727566 spark_ai_python-0.3.9/sparkai/core/callbacks/streaming_stdout.py
+-rw-r--r--   0        0        0     7376 2024-03-14 06:46:24.402412 spark_ai_python-0.3.9/sparkai/core/globals/__init__.py
+-rw-r--r--   0        0        0      516 2024-03-14 03:31:29.182052 spark_ai_python-0.3.9/sparkai/core/language_models/__init__.py
+-rw-r--r--   0        0        0    10736 2024-03-14 04:49:53.923298 spark_ai_python-0.3.9/sparkai/core/language_models/base.py
+-rw-r--r--   0        0        0    29296 2024-03-14 16:48:12.298618 spark_ai_python-0.3.9/sparkai/core/language_models/chat_models.py
+-rw-r--r--   0        0        0    41216 2024-03-14 06:46:24.368076 spark_ai_python-0.3.9/sparkai/core/language_models/llms.py
+-rw-r--r--   0        0        0      255 2024-03-14 03:20:36.390329 spark_ai_python-0.3.9/sparkai/core/load/__init__.py
+-rw-r--r--   0        0        0     1172 2024-03-14 01:50:26.779862 spark_ai_python-0.3.9/sparkai/core/load/dump.py
+-rw-r--r--   0        0        0     5413 2024-03-14 06:46:24.404251 spark_ai_python-0.3.9/sparkai/core/load/load.py
+-rw-r--r--   0        0        0    25671 2024-03-14 06:46:24.377304 spark_ai_python-0.3.9/sparkai/core/load/mapping.py
+-rw-r--r--   0        0        0     6241 2024-03-14 06:46:24.420899 spark_ai_python-0.3.9/sparkai/core/load/serializable.py
+-rw-r--r--   0        0        0     8654 2024-03-14 16:05:33.697435 spark_ai_python-0.3.9/sparkai/core/messages/__init__.py
+-rw-r--r--   0        0        0     1724 2024-03-14 03:19:59.153486 spark_ai_python-0.3.9/sparkai/core/messages/ai.py
+-rw-r--r--   0        0        0     6952 2024-03-14 03:19:59.155127 spark_ai_python-0.3.9/sparkai/core/messages/base.py
+-rw-r--r--   0        0        0     2017 2024-03-14 03:19:59.150666 spark_ai_python-0.3.9/sparkai/core/messages/chat.py
+-rw-r--r--   0        0        0     3402 2024-03-14 16:41:51.672975 spark_ai_python-0.3.9/sparkai/core/messages/function.py
+-rw-r--r--   0        0        0     1063 2024-03-14 03:19:59.158213 spark_ai_python-0.3.9/sparkai/core/messages/human.py
+-rw-r--r--   0        0        0     1016 2024-03-14 03:19:59.156822 spark_ai_python-0.3.9/sparkai/core/messages/system.py
+-rw-r--r--   0        0        0     1723 2024-03-14 03:19:59.148824 spark_ai_python-0.3.9/sparkai/core/messages/tool.py
+-rw-r--r--   0        0        0      472 2024-03-14 01:48:00.771129 spark_ai_python-0.3.9/sparkai/core/outputs/__init__.py
+-rw-r--r--   0        0        0     2596 2024-03-14 06:46:24.353899 spark_ai_python-0.3.9/sparkai/core/outputs/chat_generation.py
+-rw-r--r--   0        0        0      507 2024-03-14 01:45:58.509890 spark_ai_python-0.3.9/sparkai/core/outputs/chat_result.py
+-rw-r--r--   0        0        0     1815 2024-03-14 06:46:24.370326 spark_ai_python-0.3.9/sparkai/core/outputs/generation.py
+-rw-r--r--   0        0        0     2442 2024-03-14 01:47:24.446293 spark_ai_python-0.3.9/sparkai/core/outputs/llm_result.py
+-rw-r--r--   0        0        0      293 2024-03-14 01:47:32.585459 spark_ai_python-0.3.9/sparkai/core/outputs/run_info.py
+-rw-r--r--   0        0        0     3367 2024-03-14 06:46:24.407495 spark_ai_python-0.3.9/sparkai/core/prompt_values.py
+-rw-r--r--   0        0        0     2581 2024-02-02 05:35:24.232000 spark_ai_python-0.3.9/sparkai/core/prompts/__init__.py
+-rw-r--r--   0        0        0     8953 2024-03-14 06:46:24.398978 spark_ai_python-0.3.9/sparkai/core/prompts/base.py
+-rw-r--r--   0        0        0    33263 2024-03-14 06:46:24.424427 spark_ai_python-0.3.9/sparkai/core/prompts/chat.py
+-rw-r--r--   0        0        0    11979 2024-02-02 05:35:24.233000 spark_ai_python-0.3.9/sparkai/core/prompts/few_shot.py
+-rw-r--r--   0        0        0     5821 2024-03-14 06:46:24.383831 spark_ai_python-0.3.9/sparkai/core/prompts/few_shot_with_templates.py
+-rw-r--r--   0        0        0     2656 2024-02-02 05:35:24.233000 spark_ai_python-0.3.9/sparkai/core/prompts/image.py
+-rw-r--r--   0        0        0     6357 2024-02-02 05:35:24.233000 spark_ai_python-0.3.9/sparkai/core/prompts/loading.py
+-rw-r--r--   0        0        0     2502 2024-03-14 06:46:24.357524 spark_ai_python-0.3.9/sparkai/core/prompts/pipeline.py
+-rw-r--r--   0        0        0     9837 2024-03-14 06:46:24.344416 spark_ai_python-0.3.9/sparkai/core/prompts/prompt.py
+-rw-r--r--   0        0        0     6289 2024-03-14 06:46:24.372890 spark_ai_python-0.3.9/sparkai/core/prompts/string.py
+-rw-r--r--   0        0        0      927 2024-02-02 05:35:24.234000 spark_ai_python-0.3.9/sparkai/core/pydantic_v1/__init__.py
+-rw-r--r--   0        0        0      134 2024-02-02 05:35:24.234000 spark_ai_python-0.3.9/sparkai/core/pydantic_v1/dataclasses.py
+-rw-r--r--   0        0        0      120 2024-02-02 05:35:24.234000 spark_ai_python-0.3.9/sparkai/core/pydantic_v1/main.py
+-rw-r--r--   0        0        0     2170 2024-03-14 04:50:57.946244 spark_ai_python-0.3.9/sparkai/core/runnables/__init__.py
+-rw-r--r--   0        0        0   163501 2024-03-14 06:46:24.395202 spark_ai_python-0.3.9/sparkai/core/runnables/base.py
+-rw-r--r--   0        0        0    14390 2024-03-14 06:46:24.418771 spark_ai_python-0.3.9/sparkai/core/runnables/branch.py
+-rw-r--r--   0        0        0    16983 2024-03-14 04:50:21.132453 spark_ai_python-0.3.9/sparkai/core/runnables/config.py
+-rw-r--r--   0        0        0    16043 2024-03-14 06:46:24.363487 spark_ai_python-0.3.9/sparkai/core/runnables/configurable.py
+-rw-r--r--   0        0        0    19821 2024-03-14 06:46:24.400959 spark_ai_python-0.3.9/sparkai/core/runnables/fallbacks.py
+-rw-r--r--   0        0        0     5036 2024-03-14 04:50:45.282970 spark_ai_python-0.3.9/sparkai/core/runnables/graph.py
+-rw-r--r--   0        0        0     8741 2024-02-02 05:35:24.235000 spark_ai_python-0.3.9/sparkai/core/runnables/graph_draw.py
+-rw-r--r--   0        0        0    19025 2024-03-14 06:46:24.397392 spark_ai_python-0.3.9/sparkai/core/runnables/history.py
+-rw-r--r--   0        0        0    21904 2024-03-14 06:46:24.381266 spark_ai_python-0.3.9/sparkai/core/runnables/passthrough.py
+-rw-r--r--   0        0        0    11959 2024-03-14 06:46:24.411696 spark_ai_python-0.3.9/sparkai/core/runnables/retry.py
+-rw-r--r--   0        0        0     6272 2024-03-14 06:46:24.409736 spark_ai_python-0.3.9/sparkai/core/runnables/router.py
+-rw-r--r--   0        0        0     4399 2024-02-02 05:35:24.236000 spark_ai_python-0.3.9/sparkai/core/runnables/schema.py
+-rw-r--r--   0        0        0    14836 2024-03-14 04:50:36.551170 spark_ai_python-0.3.9/sparkai/core/runnables/utils.py
+-rw-r--r--   0        0        0    32988 2024-03-14 16:21:59.432072 spark_ai_python-0.3.9/sparkai/core/tools.py
+-rw-r--r--   0        0        0      828 2024-03-20 14:47:11.220780 spark_ai_python-0.3.9/sparkai/core/tracers/__init__.py
+-rw-r--r--   0        0        0    23849 2024-03-14 05:22:42.111248 spark_ai_python-0.3.9/sparkai/core/tracers/base.py
+-rw-r--r--   0        0        0     7606 2024-03-14 05:20:13.688094 spark_ai_python-0.3.9/sparkai/core/tracers/context.py
+-rw-r--r--   0        0        0     8208 2024-03-14 05:20:13.693996 spark_ai_python-0.3.9/sparkai/core/tracers/evaluation.py
+-rw-r--r--   0        0        0     8931 2024-03-14 05:24:28.823215 spark_ai_python-0.3.9/sparkai/core/tracers/langchain.py
+-rw-r--r--   0        0        0     7716 2024-03-14 06:46:24.349501 spark_ai_python-0.3.9/sparkai/core/tracers/langchain_v1.py
+-rw-r--r--   0        0        0    21451 2024-03-14 05:20:13.691027 spark_ai_python-0.3.9/sparkai/core/tracers/log_stream.py
+-rw-r--r--   0        0        0     3933 2024-03-14 05:18:56.159000 spark_ai_python-0.3.9/sparkai/core/tracers/memory_stream.py
+-rw-r--r--   0        0        0     1698 2024-03-14 05:20:13.686773 spark_ai_python-0.3.9/sparkai/core/tracers/root_listeners.py
+-rw-r--r--   0        0        0     1526 2024-03-14 05:20:13.696287 spark_ai_python-0.3.9/sparkai/core/tracers/run_collector.py
+-rw-r--r--   0        0        0     2838 2024-03-20 14:46:11.736409 spark_ai_python-0.3.9/sparkai/core/tracers/schemas.py
+-rw-r--r--   0        0        0     6180 2024-03-14 05:20:13.685167 spark_ai_python-0.3.9/sparkai/core/tracers/stdout.py
+-rw-r--r--   0        0        0     1270 2024-03-14 03:12:55.110592 spark_ai_python-0.3.9/sparkai/core/utils/__init__.py
+-rw-r--r--   0        0        0     1616 2024-02-02 05:35:24.238000 spark_ai_python-0.3.9/sparkai/core/utils/_merge.py
+-rw-r--r--   0        0        0     7198 2024-02-02 05:35:24.238000 spark_ai_python-0.3.9/sparkai/core/utils/aiter.py
+-rw-r--r--   0        0        0     1297 2024-02-02 05:35:24.238000 spark_ai_python-0.3.9/sparkai/core/utils/env.py
+-rw-r--r--   0        0        0      907 2024-02-02 05:35:24.238000 spark_ai_python-0.3.9/sparkai/core/utils/formatting.py
+-rw-r--r--   0        0        0    10334 2024-03-15 01:32:08.108678 spark_ai_python-0.3.9/sparkai/core/utils/function_calling.py
+-rw-r--r--   0        0        0     3090 2024-02-02 05:35:24.238000 spark_ai_python-0.3.9/sparkai/core/utils/html.py
+-rw-r--r--   0        0        0      423 2024-02-02 05:35:24.238000 spark_ai_python-0.3.9/sparkai/core/utils/image.py
+-rw-r--r--   0        0        0     1289 2024-02-02 05:35:24.238000 spark_ai_python-0.3.9/sparkai/core/utils/input.py
+-rw-r--r--   0        0        0      139 2024-02-02 05:35:24.239000 spark_ai_python-0.3.9/sparkai/core/utils/interactive_env.py
+-rw-r--r--   0        0        0     5822 2024-02-02 05:35:24.239000 spark_ai_python-0.3.9/sparkai/core/utils/iter.py
+-rw-r--r--   0        0        0     2318 2024-02-02 05:35:24.239000 spark_ai_python-0.3.9/sparkai/core/utils/json_schema.py
+-rw-r--r--   0        0        0     2011 2024-02-02 05:35:24.239000 spark_ai_python-0.3.9/sparkai/core/utils/loading.py
+-rw-r--r--   0        0        0      301 2024-02-02 05:35:24.239000 spark_ai_python-0.3.9/sparkai/core/utils/pydantic.py
+-rw-r--r--   0        0        0      908 2024-02-02 05:35:24.239000 spark_ai_python-0.3.9/sparkai/core/utils/strings.py
+-rw-r--r--   0        0        0     6158 2024-03-14 01:47:13.885399 spark_ai_python-0.3.9/sparkai/core/utils/utils.py
+-rw-r--r--   0        0        0      374 2023-05-03 13:09:38.934327 spark_ai_python-0.3.9/sparkai/deprecation.py
+-rw-r--r--   0        0        0     1151 2024-02-02 05:10:31.290500 spark_ai_python-0.3.9/sparkai/depreciated/__init__.py
+-rw-r--r--   0        0        0     1151 2024-02-02 05:10:31.287607 spark_ai_python-0.3.9/sparkai/depreciated/client/__init__.py
+-rw-r--r--   0        0        0     3670 2024-03-14 15:36:22.936130 spark_ai_python-0.3.9/sparkai/depreciated/client/llm.py
+-rw-r--r--   0        0        0     2438 2024-03-14 06:46:24.414331 spark_ai_python-0.3.9/sparkai/depreciated/client/sample_langchain_spark.py
+-rw-r--r--   0        0        0     1151 2024-02-02 05:14:30.402301 spark_ai_python-0.3.9/sparkai/depreciated/service/__init__.py
+-rw-r--r--   0        0        0     2495 2024-03-14 06:46:24.386756 spark_ai_python-0.3.9/sparkai/depreciated/service/api_server.py
+-rw-r--r--   0        0        0     5104 2024-02-02 05:15:10.571713 spark_ai_python-0.3.9/sparkai/depreciated/service/spark_ws.py
+-rw-r--r--   0        0        0     1952 2023-05-02 05:58:50.610144 spark_ai_python-0.3.9/sparkai/errors/__init__.py
+-rw-r--r--   0        0        0     1907 2024-03-14 05:22:19.678605 spark_ai_python-0.3.9/sparkai/exceptions.py
+-rw-r--r--   0        0        0     1151 2024-03-27 09:25:47.330409 spark_ai_python-0.3.9/sparkai/frameworks/__init__.py
+-rw-r--r--   0        0        0     7274 2024-03-29 03:26:20.606528 spark_ai_python-0.3.9/sparkai/frameworks/autogen/__init__.py
+-rw-r--r--   0        0        0     9018 2024-03-27 13:54:49.802292 spark_ai_python-0.3.9/sparkai/frameworks/llama_index/__init__.py
+-rw-r--r--   0        0        0     1256 2023-04-29 01:49:30.738000 spark_ai_python-0.3.9/sparkai/http_retry/__init__.py
+-rw-r--r--   0        0        0     2647 2023-04-29 02:52:26.276574 spark_ai_python-0.3.9/sparkai/http_retry/async_handler.py
+-rw-r--r--   0        0        0     2970 2023-04-29 02:52:26.274822 spark_ai_python-0.3.9/sparkai/http_retry/builtin_async_handlers.py
+-rw-r--r--   0        0        0     2884 2023-04-29 02:52:26.279895 spark_ai_python-0.3.9/sparkai/http_retry/builtin_handlers.py
+-rw-r--r--   0        0        0     1622 2023-04-29 01:49:30.738000 spark_ai_python-0.3.9/sparkai/http_retry/builtin_interval_calculators.py
+-rw-r--r--   0        0        0     2455 2023-04-29 02:52:26.278033 spark_ai_python-0.3.9/sparkai/http_retry/handler.py
+-rw-r--r--   0        0        0      450 2023-04-29 01:49:30.738000 spark_ai_python-0.3.9/sparkai/http_retry/interval_calculator.py
+-rw-r--r--   0        0        0      597 2023-04-29 01:49:30.738000 spark_ai_python-0.3.9/sparkai/http_retry/jitter.py
+-rw-r--r--   0        0        0     1035 2023-04-29 01:49:30.738000 spark_ai_python-0.3.9/sparkai/http_retry/request.py
+-rw-r--r--   0        0        0      639 2023-04-29 01:49:30.738000 spark_ai_python-0.3.9/sparkai/http_retry/response.py
+-rw-r--r--   0        0        0      570 2023-04-29 01:49:30.738000 spark_ai_python-0.3.9/sparkai/http_retry/state.py
+-rw-r--r--   0        0        0     1151 2024-02-02 09:55:21.275283 spark_ai_python-0.3.9/sparkai/llm/__init__.py
+-rw-r--r--   0        0        0    18815 2024-03-26 01:45:58.539209 spark_ai_python-0.3.9/sparkai/llm/llm.py
+-rw-r--r--   0        0        0     1151 2023-07-23 12:42:01.813357 spark_ai_python-0.3.9/sparkai/log/__init__.py
+-rw-r--r--   0        0        0     3060 2024-02-02 05:46:52.625440 spark_ai_python-0.3.9/sparkai/log/logger.py
+-rw-r--r--   0        0        0     1088 2023-04-29 07:37:03.991801 spark_ai_python-0.3.9/sparkai/memory/__init__.py
+-rw-r--r--   0        0        0     3065 2023-04-29 07:35:27.052139 spark_ai_python-0.3.9/sparkai/memory/buffer.py
+-rw-r--r--   0        0        0     1143 2023-04-29 07:32:35.289915 spark_ai_python-0.3.9/sparkai/memory/buffer_window.py
+-rw-r--r--   0        0        0     1558 2023-04-29 07:30:52.099436 spark_ai_python-0.3.9/sparkai/memory/chat_memory.py
+-rw-r--r--   0        0        0      474 2023-04-29 07:21:51.986161 spark_ai_python-0.3.9/sparkai/memory/chat_message_histories/__init__.py
+-rw-r--r--   0        0        0     2590 2023-04-29 07:21:51.994679 spark_ai_python-0.3.9/sparkai/memory/chat_message_histories/dynamodb.py
+-rw-r--r--   0        0        0     1570 2023-04-29 07:21:51.990773 spark_ai_python-0.3.9/sparkai/memory/chat_message_histories/file.py
+-rw-r--r--   0        0        0      548 2023-04-29 07:21:51.989452 spark_ai_python-0.3.9/sparkai/memory/chat_message_histories/in_memory.py
+-rw-r--r--   0        0        0     2753 2023-04-29 07:21:51.988132 spark_ai_python-0.3.9/sparkai/memory/chat_message_histories/postgres.py
+-rw-r--r--   0        0        0     2047 2023-04-29 07:21:51.991910 spark_ai_python-0.3.9/sparkai/memory/chat_message_histories/redis.py
+-rw-r--r--   0        0        0     1489 2023-04-29 07:30:52.110734 spark_ai_python-0.3.9/sparkai/memory/combined.py
+-rw-r--r--   0        0        0      787 2023-04-29 07:30:52.102790 spark_ai_python-0.3.9/sparkai/memory/readonly.py
+-rw-r--r--   0        0        0      762 2023-04-29 07:30:52.103685 spark_ai_python-0.3.9/sparkai/memory/simple.py
+-rw-r--r--   0        0        0     1862 2023-04-29 07:31:29.143884 spark_ai_python-0.3.9/sparkai/memory/token_buffer.py
+-rw-r--r--   0        0        0      510 2023-04-29 07:30:52.104836 spark_ai_python-0.3.9/sparkai/memory/utils.py
+-rw-r--r--   0        0        0     1046 2024-03-14 03:17:21.191832 spark_ai_python-0.3.9/sparkai/messages.py
+-rw-r--r--   0        0        0     2039 2023-05-03 13:10:19.932620 spark_ai_python-0.3.9/sparkai/models/__init__.py
+-rw-r--r--   0        0        0     3911 2023-05-03 12:39:55.387507 spark_ai_python-0.3.9/sparkai/models/basic_objects.py
+-rw-r--r--   0        0        0     4945 2023-08-13 08:28:00.532036 spark_ai_python-0.3.9/sparkai/models/chat/__init__.py
+-rw-r--r--   0        0        0     1384 2023-05-09 07:13:52.048866 spark_ai_python-0.3.9/sparkai/prompts/classification/__init__.py
+-rw-r--r--   0        0        0      821 2023-04-29 01:49:30.743000 spark_ai_python-0.3.9/sparkai/proxy_env_variable_loader.py
+-rw-r--r--   0        0        0    11977 2023-05-02 02:56:04.982300 spark_ai_python-0.3.9/sparkai/schema.py
+-rw-r--r--   0        0        0     1151 2024-03-26 01:49:02.917906 spark_ai_python-0.3.9/sparkai/serve/__init__.py
+-rw-r--r--   0        0        0    13061 2024-03-26 01:49:02.918125 spark_ai_python-0.3.9/sparkai/serve/api_provider.py
+-rw-r--r--   0        0        0     7020 2024-03-26 08:23:39.323316 spark_ai_python-0.3.9/sparkai/serve/base_model.py
+-rw-r--r--   0        0        0    13225 2024-03-26 01:49:02.918454 spark_ai_python-0.3.9/sparkai/serve/controller.py
+-rw-r--r--   0        0        0    29007 2024-03-26 01:49:02.918709 spark_ai_python-0.3.9/sparkai/serve/gradio_web_server.py
+-rw-r--r--   0        0        0     1151 2024-03-26 01:49:02.918858 spark_ai_python-0.3.9/sparkai/serve/model/__init__.py
+-rw-r--r--   0        0        0     5561 2024-03-26 01:49:02.919011 spark_ai_python-0.3.9/sparkai/serve/model/model_adapter.py
+-rw-r--r--   0        0        0    18798 2024-03-26 01:49:02.919217 spark_ai_python-0.3.9/sparkai/serve/model/model_registry.py
+-rw-r--r--   0        0        0    12951 2024-03-26 01:49:02.919401 spark_ai_python-0.3.9/sparkai/serve/model_worker.py
+-rw-r--r--   0        0        0    11895 2024-03-26 01:49:02.919593 spark_ai_python-0.3.9/sparkai/serve/utils/__init__.py
+-rw-r--r--   0        0        0     1154 2023-07-23 01:18:08.275512 spark_ai_python-0.3.9/sparkai/socket_mode/__init__.py
+-rw-r--r--   0        0        0     5472 2023-08-14 01:40:39.883803 spark_ai_python-0.3.9/sparkai/socket_mode/client.py
+-rw-r--r--   0        0        0      907 2023-04-29 01:49:30.745000 spark_ai_python-0.3.9/sparkai/socket_mode/interval_runner.py
+-rw-r--r--   0        0        0      525 2023-04-29 02:36:07.360120 spark_ai_python-0.3.9/sparkai/socket_mode/listeners.py
+-rw-r--r--   0        0        0     1989 2023-04-29 02:36:07.370555 spark_ai_python-0.3.9/sparkai/socket_mode/request.py
+-rw-r--r--   0        0        0      878 2023-04-29 02:36:07.363593 spark_ai_python-0.3.9/sparkai/socket_mode/response.py
+-rw-r--r--   0        0        0    21111 2023-07-23 01:49:38.590155 spark_ai_python-0.3.9/sparkai/socket_mode/websocket_client/__init__.py
+-rw-r--r--   0        0        0     1802 2024-03-13 07:45:20.129308 spark_ai_python-0.3.9/sparkai/spark_proxy/generate_message.py
+-rw-r--r--   0        0        0     1957 2024-03-13 07:45:20.129475 spark_ai_python-0.3.9/sparkai/spark_proxy/generate_stream.py
+-rw-r--r--   0        0        0      134 2024-03-13 06:53:32.303669 spark_ai_python-0.3.9/sparkai/spark_proxy/main.py
+-rw-r--r--   0        0        0     2866 2024-03-13 07:45:20.129645 spark_ai_python-0.3.9/sparkai/spark_proxy/openai_types.py
+-rw-r--r--   0        0        0     3453 2024-03-13 08:47:52.452083 spark_ai_python-0.3.9/sparkai/spark_proxy/server.py
+-rw-r--r--   0        0        0     3815 2024-03-24 10:16:30.908132 spark_ai_python-0.3.9/sparkai/spark_proxy/spark_api.py
+-rw-r--r--   0        0        0     2052 2024-03-13 06:43:49.970481 spark_ai_python-0.3.9/sparkai/spark_proxy/spark_auth.py
+-rw-r--r--   0        0        0       95 2024-03-25 12:03:42.504504 spark_ai_python-0.3.9/sparkai/version.py
+-rw-r--r--   0        0        0     1208 2023-04-29 03:12:25.029956 spark_ai_python-0.3.9/sparkai/xf_util.py
+-rw-r--r--   0        0        0    16399 1970-01-01 00:00:00.000000 spark_ai_python-0.3.9/PKG-INFO
```

### Comparing `spark_ai_python-0.3.8/LICENSE` & `spark_ai_python-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/README.md` & `spark_ai_python-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/pyproject.toml` & `spark_ai_python-0.3.9/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spark-ai-python"
-version = "0.3.8"
+version = "0.3.9"
 description = "a sdk for iflytek's spark LLM."
 authors = ["whybeyoung <ybyang7@iflytek.com>", "mingduan <mingduan@iflytek.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "sparkai" }
 ]
@@ -18,21 +18,25 @@
 websockets = "*"
 nest_asyncio = "*"
 
 packaging = "*"
 tenacity = "*"
 jsonpatch = "*"
 llama-index-core = { version = "^0.10.24.post1", optional = true }
+pyautogen = { version = ">=0.2.20", optional = true }
 uvicorn = { version = ">=0.26.0", optional = true }
 fastapi = { extras = ["all"], version = "^0.110.0", optional = true}
 
 [tool.poetry.extras]
 llama_index = [
     "llama-index-core"
 ]
+autogen = [
+    "pyautogen"
+]
 proxy = [
     "fastapi",
     "uvicorn"
 ]
 
 [tool.pytest.ini_options]
```

### Comparing `spark_ai_python-0.3.8/sparkai/_client.py` & `spark_ai_python-0.3.9/sparkai/_client.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/api_resources/__init__.py` & `spark_ai_python-0.3.9/sparkai/api_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/api_resources/chat/__init__.py` & `spark_ai_python-0.3.9/sparkai/api_resources/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/api_resources/chat/completions.py` & `spark_ai_python-0.3.9/sparkai/api_resources/chat/completions.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/api_resources/chat_completion.py` & `spark_ai_python-0.3.9/sparkai/api_resources/chat_completion.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/constants.py` & `spark_ai_python-0.3.9/sparkai/constants.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/conversation/__init__.py` & `spark_ai_python-0.3.9/sparkai/conversation/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/__init__.py` & `spark_ai_python-0.3.9/sparkai/core/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/_api/__init__.py` & `spark_ai_python-0.3.9/sparkai/core/_api/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/_api/beta_decorator.py` & `spark_ai_python-0.3.9/sparkai/core/_api/beta_decorator.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/_api/deprecation.py` & `spark_ai_python-0.3.9/sparkai/core/_api/deprecation.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/_api/internal.py` & `spark_ai_python-0.3.9/sparkai/core/_api/internal.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/_api/path.py` & `spark_ai_python-0.3.9/sparkai/core/_api/path.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/_base_api.py` & `spark_ai_python-0.3.9/sparkai/core/_base_api.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/caches.py` & `spark_ai_python-0.3.9/sparkai/core/caches.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/callbacks/__init__.py` & `spark_ai_python-0.3.9/sparkai/core/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/callbacks/base.py` & `spark_ai_python-0.3.9/sparkai/core/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/callbacks/manager.py` & `spark_ai_python-0.3.9/sparkai/core/callbacks/manager.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/callbacks/stdout.py` & `spark_ai_python-0.3.9/sparkai/core/callbacks/stdout.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/callbacks/streaming_stdout.py` & `spark_ai_python-0.3.9/sparkai/core/callbacks/streaming_stdout.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/globals/__init__.py` & `spark_ai_python-0.3.9/sparkai/core/globals/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/language_models/__init__.py` & `spark_ai_python-0.3.9/sparkai/core/language_models/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/language_models/base.py` & `spark_ai_python-0.3.9/sparkai/core/language_models/base.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/language_models/chat_models.py` & `spark_ai_python-0.3.9/sparkai/core/language_models/chat_models.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/language_models/llms.py` & `spark_ai_python-0.3.9/sparkai/core/language_models/llms.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/load/dump.py` & `spark_ai_python-0.3.9/sparkai/core/load/dump.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/load/load.py` & `spark_ai_python-0.3.9/sparkai/core/load/load.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/load/mapping.py` & `spark_ai_python-0.3.9/sparkai/core/load/mapping.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/load/serializable.py` & `spark_ai_python-0.3.9/sparkai/core/load/serializable.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/messages/__init__.py` & `spark_ai_python-0.3.9/sparkai/core/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/messages/ai.py` & `spark_ai_python-0.3.9/sparkai/core/messages/ai.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/messages/base.py` & `spark_ai_python-0.3.9/sparkai/core/messages/base.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/messages/chat.py` & `spark_ai_python-0.3.9/sparkai/core/messages/chat.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/messages/function.py` & `spark_ai_python-0.3.9/sparkai/core/messages/function.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/messages/human.py` & `spark_ai_python-0.3.9/sparkai/core/messages/human.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/messages/system.py` & `spark_ai_python-0.3.9/sparkai/core/messages/system.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/messages/tool.py` & `spark_ai_python-0.3.9/sparkai/core/messages/tool.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/outputs/chat_generation.py` & `spark_ai_python-0.3.9/sparkai/core/outputs/chat_generation.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/outputs/generation.py` & `spark_ai_python-0.3.9/sparkai/core/outputs/generation.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/outputs/llm_result.py` & `spark_ai_python-0.3.9/sparkai/core/outputs/llm_result.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/prompt_values.py` & `spark_ai_python-0.3.9/sparkai/core/prompt_values.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/prompts/__init__.py` & `spark_ai_python-0.3.9/sparkai/core/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/prompts/base.py` & `spark_ai_python-0.3.9/sparkai/core/prompts/base.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/prompts/chat.py` & `spark_ai_python-0.3.9/sparkai/core/prompts/chat.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/prompts/few_shot.py` & `spark_ai_python-0.3.9/sparkai/core/prompts/few_shot.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/prompts/few_shot_with_templates.py` & `spark_ai_python-0.3.9/sparkai/core/prompts/few_shot_with_templates.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/prompts/image.py` & `spark_ai_python-0.3.9/sparkai/core/prompts/image.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/prompts/loading.py` & `spark_ai_python-0.3.9/sparkai/core/prompts/loading.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/prompts/pipeline.py` & `spark_ai_python-0.3.9/sparkai/core/prompts/pipeline.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/prompts/prompt.py` & `spark_ai_python-0.3.9/sparkai/core/prompts/prompt.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/prompts/string.py` & `spark_ai_python-0.3.9/sparkai/core/prompts/string.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/pydantic_v1/__init__.py` & `spark_ai_python-0.3.9/sparkai/core/pydantic_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/runnables/__init__.py` & `spark_ai_python-0.3.9/sparkai/core/runnables/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/runnables/base.py` & `spark_ai_python-0.3.9/sparkai/core/runnables/base.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/runnables/branch.py` & `spark_ai_python-0.3.9/sparkai/core/runnables/branch.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/runnables/config.py` & `spark_ai_python-0.3.9/sparkai/core/runnables/config.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/runnables/configurable.py` & `spark_ai_python-0.3.9/sparkai/core/runnables/configurable.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/runnables/fallbacks.py` & `spark_ai_python-0.3.9/sparkai/core/runnables/fallbacks.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/runnables/graph.py` & `spark_ai_python-0.3.9/sparkai/core/runnables/graph.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/runnables/graph_draw.py` & `spark_ai_python-0.3.9/sparkai/core/runnables/graph_draw.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/runnables/history.py` & `spark_ai_python-0.3.9/sparkai/core/runnables/history.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/runnables/passthrough.py` & `spark_ai_python-0.3.9/sparkai/core/runnables/passthrough.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/runnables/retry.py` & `spark_ai_python-0.3.9/sparkai/core/runnables/retry.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/runnables/router.py` & `spark_ai_python-0.3.9/sparkai/core/runnables/router.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/runnables/schema.py` & `spark_ai_python-0.3.9/sparkai/core/runnables/schema.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/runnables/utils.py` & `spark_ai_python-0.3.9/sparkai/core/runnables/utils.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/tools.py` & `spark_ai_python-0.3.9/sparkai/core/tools.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/tracers/__init__.py` & `spark_ai_python-0.3.9/sparkai/core/tracers/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/tracers/base.py` & `spark_ai_python-0.3.9/sparkai/core/tracers/base.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/tracers/context.py` & `spark_ai_python-0.3.9/sparkai/core/tracers/context.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/tracers/evaluation.py` & `spark_ai_python-0.3.9/sparkai/core/tracers/evaluation.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/tracers/langchain.py` & `spark_ai_python-0.3.9/sparkai/core/tracers/langchain.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/tracers/langchain_v1.py` & `spark_ai_python-0.3.9/sparkai/core/tracers/langchain_v1.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/tracers/log_stream.py` & `spark_ai_python-0.3.9/sparkai/core/tracers/log_stream.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/tracers/memory_stream.py` & `spark_ai_python-0.3.9/sparkai/core/tracers/memory_stream.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/tracers/root_listeners.py` & `spark_ai_python-0.3.9/sparkai/core/tracers/root_listeners.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/tracers/run_collector.py` & `spark_ai_python-0.3.9/sparkai/core/tracers/run_collector.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/tracers/schemas.py` & `spark_ai_python-0.3.9/sparkai/core/tracers/schemas.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/tracers/stdout.py` & `spark_ai_python-0.3.9/sparkai/core/tracers/stdout.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/utils/__init__.py` & `spark_ai_python-0.3.9/sparkai/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/utils/_merge.py` & `spark_ai_python-0.3.9/sparkai/core/utils/_merge.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/utils/aiter.py` & `spark_ai_python-0.3.9/sparkai/core/utils/aiter.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/utils/env.py` & `spark_ai_python-0.3.9/sparkai/core/utils/env.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/utils/formatting.py` & `spark_ai_python-0.3.9/sparkai/core/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/utils/function_calling.py` & `spark_ai_python-0.3.9/sparkai/core/utils/function_calling.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/utils/html.py` & `spark_ai_python-0.3.9/sparkai/core/utils/html.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/utils/input.py` & `spark_ai_python-0.3.9/sparkai/core/utils/input.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/utils/iter.py` & `spark_ai_python-0.3.9/sparkai/core/utils/iter.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/utils/json_schema.py` & `spark_ai_python-0.3.9/sparkai/core/utils/json_schema.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/utils/loading.py` & `spark_ai_python-0.3.9/sparkai/core/utils/loading.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/utils/strings.py` & `spark_ai_python-0.3.9/sparkai/core/utils/strings.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/core/utils/utils.py` & `spark_ai_python-0.3.9/sparkai/core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/depreciated/__init__.py` & `spark_ai_python-0.3.9/sparkai/depreciated/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/depreciated/client/__init__.py` & `spark_ai_python-0.3.9/sparkai/depreciated/client/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/depreciated/client/llm.py` & `spark_ai_python-0.3.9/sparkai/depreciated/client/llm.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/depreciated/client/sample_langchain_spark.py` & `spark_ai_python-0.3.9/sparkai/depreciated/client/sample_langchain_spark.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/depreciated/service/__init__.py` & `spark_ai_python-0.3.9/sparkai/depreciated/service/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/depreciated/service/api_server.py` & `spark_ai_python-0.3.9/sparkai/depreciated/service/api_server.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/depreciated/service/spark_ws.py` & `spark_ai_python-0.3.9/sparkai/depreciated/service/spark_ws.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/errors/__init__.py` & `spark_ai_python-0.3.9/sparkai/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/exceptions.py` & `spark_ai_python-0.3.9/sparkai/exceptions.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/frameworks/__init__.py` & `spark_ai_python-0.3.9/sparkai/frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/frameworks/llama_index/__init__.py` & `spark_ai_python-0.3.9/sparkai/frameworks/llama_index/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/http_retry/__init__.py` & `spark_ai_python-0.3.9/sparkai/http_retry/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/http_retry/async_handler.py` & `spark_ai_python-0.3.9/sparkai/http_retry/async_handler.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/http_retry/builtin_async_handlers.py` & `spark_ai_python-0.3.9/sparkai/http_retry/builtin_async_handlers.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/http_retry/builtin_handlers.py` & `spark_ai_python-0.3.9/sparkai/http_retry/builtin_handlers.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/http_retry/builtin_interval_calculators.py` & `spark_ai_python-0.3.9/sparkai/http_retry/builtin_interval_calculators.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/http_retry/handler.py` & `spark_ai_python-0.3.9/sparkai/http_retry/handler.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/http_retry/jitter.py` & `spark_ai_python-0.3.9/sparkai/http_retry/jitter.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/http_retry/request.py` & `spark_ai_python-0.3.9/sparkai/http_retry/request.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/http_retry/response.py` & `spark_ai_python-0.3.9/sparkai/http_retry/response.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/http_retry/state.py` & `spark_ai_python-0.3.9/sparkai/http_retry/state.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/llm/__init__.py` & `spark_ai_python-0.3.9/sparkai/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/llm/llm.py` & `spark_ai_python-0.3.9/sparkai/llm/llm.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/log/__init__.py` & `spark_ai_python-0.3.9/sparkai/log/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/log/logger.py` & `spark_ai_python-0.3.9/sparkai/log/logger.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/memory/__init__.py` & `spark_ai_python-0.3.9/sparkai/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/memory/buffer.py` & `spark_ai_python-0.3.9/sparkai/memory/buffer.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/memory/buffer_window.py` & `spark_ai_python-0.3.9/sparkai/memory/buffer_window.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/memory/chat_memory.py` & `spark_ai_python-0.3.9/sparkai/memory/chat_memory.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/memory/chat_message_histories/dynamodb.py` & `spark_ai_python-0.3.9/sparkai/memory/chat_message_histories/dynamodb.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/memory/chat_message_histories/file.py` & `spark_ai_python-0.3.9/sparkai/memory/chat_message_histories/file.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/memory/chat_message_histories/in_memory.py` & `spark_ai_python-0.3.9/sparkai/memory/chat_message_histories/in_memory.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/memory/chat_message_histories/postgres.py` & `spark_ai_python-0.3.9/sparkai/memory/chat_message_histories/postgres.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/memory/chat_message_histories/redis.py` & `spark_ai_python-0.3.9/sparkai/memory/chat_message_histories/redis.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/memory/combined.py` & `spark_ai_python-0.3.9/sparkai/memory/combined.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/memory/readonly.py` & `spark_ai_python-0.3.9/sparkai/memory/readonly.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/memory/simple.py` & `spark_ai_python-0.3.9/sparkai/memory/simple.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/memory/token_buffer.py` & `spark_ai_python-0.3.9/sparkai/memory/token_buffer.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/messages.py` & `spark_ai_python-0.3.9/sparkai/messages.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/models/__init__.py` & `spark_ai_python-0.3.9/sparkai/models/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/models/basic_objects.py` & `spark_ai_python-0.3.9/sparkai/models/basic_objects.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/models/chat/__init__.py` & `spark_ai_python-0.3.9/sparkai/models/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/prompts/classification/__init__.py` & `spark_ai_python-0.3.9/sparkai/prompts/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/proxy_env_variable_loader.py` & `spark_ai_python-0.3.9/sparkai/proxy_env_variable_loader.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/schema.py` & `spark_ai_python-0.3.9/sparkai/schema.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/serve/__init__.py` & `spark_ai_python-0.3.9/sparkai/serve/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/serve/api_provider.py` & `spark_ai_python-0.3.9/sparkai/serve/api_provider.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/serve/base_model.py` & `spark_ai_python-0.3.9/sparkai/serve/base_model.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/serve/controller.py` & `spark_ai_python-0.3.9/sparkai/serve/controller.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/serve/gradio_web_server.py` & `spark_ai_python-0.3.9/sparkai/serve/gradio_web_server.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/serve/model/__init__.py` & `spark_ai_python-0.3.9/sparkai/serve/model/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/serve/model/model_adapter.py` & `spark_ai_python-0.3.9/sparkai/serve/model/model_adapter.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/serve/model/model_registry.py` & `spark_ai_python-0.3.9/sparkai/serve/model/model_registry.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/serve/model_worker.py` & `spark_ai_python-0.3.9/sparkai/serve/model_worker.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/serve/utils/__init__.py` & `spark_ai_python-0.3.9/sparkai/serve/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/socket_mode/__init__.py` & `spark_ai_python-0.3.9/sparkai/socket_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/socket_mode/client.py` & `spark_ai_python-0.3.9/sparkai/socket_mode/client.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/socket_mode/interval_runner.py` & `spark_ai_python-0.3.9/sparkai/socket_mode/interval_runner.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/socket_mode/listeners.py` & `spark_ai_python-0.3.9/sparkai/socket_mode/listeners.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/socket_mode/request.py` & `spark_ai_python-0.3.9/sparkai/socket_mode/request.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/socket_mode/response.py` & `spark_ai_python-0.3.9/sparkai/socket_mode/response.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/socket_mode/websocket_client/__init__.py` & `spark_ai_python-0.3.9/sparkai/socket_mode/websocket_client/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/spark_proxy/generate_message.py` & `spark_ai_python-0.3.9/sparkai/spark_proxy/generate_message.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/spark_proxy/generate_stream.py` & `spark_ai_python-0.3.9/sparkai/spark_proxy/generate_stream.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/spark_proxy/openai_types.py` & `spark_ai_python-0.3.9/sparkai/spark_proxy/openai_types.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/spark_proxy/server.py` & `spark_ai_python-0.3.9/sparkai/spark_proxy/server.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/spark_proxy/spark_api.py` & `spark_ai_python-0.3.9/sparkai/spark_proxy/spark_api.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/spark_proxy/spark_auth.py` & `spark_ai_python-0.3.9/sparkai/spark_proxy/spark_auth.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/sparkai/xf_util.py` & `spark_ai_python-0.3.9/sparkai/xf_util.py`

 * *Files identical despite different names*

### Comparing `spark_ai_python-0.3.8/PKG-INFO` & `spark_ai_python-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: spark-ai-python
-Version: 0.3.8
+Version: 0.3.9
 Summary: a sdk for iflytek's spark LLM.
 License: MIT
 Author: whybeyoung
 Author-email: ybyang7@iflytek.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Provides-Extra: autogen
 Provides-Extra: llama-index
 Provides-Extra: proxy
 Requires-Dist: aiohttp (>3.3)
 Requires-Dist: fastapi[all] (>=0.110.0,<0.111.0) ; extra == "proxy"
 Requires-Dist: jsonpatch
 Requires-Dist: llama-index-core (>=0.10.24.post1,<0.11.0) ; extra == "llama-index"
 Requires-Dist: nest-asyncio (>=1.6.0,<2.0.0)
 Requires-Dist: nest_asyncio
 Requires-Dist: packaging
+Requires-Dist: pyautogen (>=0.2.20) ; extra == "autogen"
 Requires-Dist: requests
 Requires-Dist: tenacity
 Requires-Dist: uvicorn (>=0.26.0) ; extra == "proxy"
 Requires-Dist: websocket-client (>=1.7.0,<2.0.0)
 Requires-Dist: websockets
 Description-Content-Type: text/markdown
```

