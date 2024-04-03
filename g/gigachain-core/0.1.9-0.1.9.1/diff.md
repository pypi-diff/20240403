# Comparing `tmp/gigachain_core-0.1.9.tar.gz` & `tmp/gigachain_core-0.1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gigachain_core-0.1.9.tar", max compression
+gzip compressed data, was "gigachain_core-0.1.9.1.tar", max compression
```

## Comparing `gigachain_core-0.1.9.tar` & `gigachain_core-0.1.9.1.tar`

### file list

```diff
@@ -1,120 +1,120 @@
--rw-r--r--   0        0        0     3047 2024-01-10 09:04:40.240772 gigachain_core-0.1.9/README.md
--rw-r--r--   0        0        0      390 2024-01-15 11:51:25.597152 gigachain_core-0.1.9/langchain_core/__init__.py
--rw-r--r--   0        0        0     1025 2024-01-15 11:51:25.598286 gigachain_core-0.1.9/langchain_core/_api/__init__.py
--rw-r--r--   0        0        0     8977 2024-01-15 11:51:25.599167 gigachain_core-0.1.9/langchain_core/_api/beta_decorator.py
--rw-r--r--   0        0        0    13829 2024-01-15 11:51:25.601616 gigachain_core-0.1.9/langchain_core/_api/deprecation.py
--rw-r--r--   0        0        0      662 2024-01-15 11:51:25.602108 gigachain_core-0.1.9/langchain_core/_api/internal.py
--rw-r--r--   0        0        0      984 2023-12-18 12:05:46.602514 gigachain_core-0.1.9/langchain_core/_api/path.py
--rw-r--r--   0        0        0     6197 2023-12-18 12:05:46.603051 gigachain_core-0.1.9/langchain_core/agents.py
--rw-r--r--   0        0        0        0 2023-12-18 12:05:46.603226 gigachain_core-0.1.9/langchain_core/beta/__init__.py
--rw-r--r--   0        0        0        0 2023-12-18 12:05:46.603462 gigachain_core-0.1.9/langchain_core/beta/runnables/__init__.py
--rw-r--r--   0        0        0    10617 2024-01-15 11:51:25.603332 gigachain_core-0.1.9/langchain_core/beta/runnables/context.py
--rw-r--r--   0        0        0      722 2023-12-18 12:05:46.604982 gigachain_core-0.1.9/langchain_core/caches.py
--rw-r--r--   0        0        0     1852 2023-12-18 12:05:46.605433 gigachain_core-0.1.9/langchain_core/callbacks/__init__.py
--rw-r--r--   0        0        0    16850 2023-12-18 12:05:46.606868 gigachain_core-0.1.9/langchain_core/callbacks/base.py
--rw-r--r--   0        0        0    62827 2024-01-15 11:51:25.606221 gigachain_core-0.1.9/langchain_core/callbacks/manager.py
--rw-r--r--   0        0        0     2256 2023-12-18 12:05:46.607875 gigachain_core-0.1.9/langchain_core/callbacks/stdout.py
--rw-r--r--   0        0        0     2433 2023-12-18 12:05:46.608271 gigachain_core-0.1.9/langchain_core/callbacks/streaming_stdout.py
--rw-r--r--   0        0        0     2493 2024-01-10 09:04:40.242637 gigachain_core-0.1.9/langchain_core/chat_history.py
--rw-r--r--   0        0        0      415 2023-12-18 12:05:46.609079 gigachain_core-0.1.9/langchain_core/chat_sessions.py
--rw-r--r--   0        0        0      176 2023-12-18 12:05:46.612530 gigachain_core-0.1.9/langchain_core/documents/__init__.py
--rw-r--r--   0        0        0      839 2023-12-18 12:05:46.612970 gigachain_core-0.1.9/langchain_core/documents/base.py
--rw-r--r--   0        0        0     2494 2024-01-15 11:51:25.608655 gigachain_core-0.1.9/langchain_core/documents/transformers.py
--rw-r--r--   0        0        0      787 2024-01-15 11:51:25.609545 gigachain_core-0.1.9/langchain_core/embeddings.py
--rw-r--r--   0        0        0      486 2024-01-10 09:04:40.243382 gigachain_core-0.1.9/langchain_core/env.py
--rw-r--r--   0        0        0      571 2023-12-18 12:05:46.615278 gigachain_core-0.1.9/langchain_core/example_selectors/__init__.py
--rw-r--r--   0        0        0      516 2024-01-15 11:51:25.610626 gigachain_core-0.1.9/langchain_core/example_selectors/base.py
--rw-r--r--   0        0        0     2453 2023-12-18 12:05:46.615913 gigachain_core-0.1.9/langchain_core/example_selectors/length_based.py
--rw-r--r--   0        0        0     7143 2024-01-15 11:51:25.612090 gigachain_core-0.1.9/langchain_core/example_selectors/semantic_similarity.py
--rw-r--r--   0        0        0     1869 2023-12-18 12:05:46.617107 gigachain_core-0.1.9/langchain_core/exceptions.py
--rw-r--r--   0        0        0     8376 2023-12-18 12:05:46.619340 gigachain_core-0.1.9/langchain_core/globals/__init__.py
--rw-r--r--   0        0        0      522 2024-01-10 09:04:40.244099 gigachain_core-0.1.9/langchain_core/language_models/__init__.py
--rw-r--r--   0        0        0    10688 2024-01-15 11:51:25.614043 gigachain_core-0.1.9/langchain_core/language_models/base.py
--rw-r--r--   0        0        0    29147 2024-01-15 11:51:25.615176 gigachain_core-0.1.9/langchain_core/language_models/chat_models.py
--rw-r--r--   0        0        0    41173 2024-01-15 11:51:25.616692 gigachain_core-0.1.9/langchain_core/language_models/llms.py
--rw-r--r--   0        0        0      261 2023-12-18 12:05:46.624002 gigachain_core-0.1.9/langchain_core/load/__init__.py
--rw-r--r--   0        0        0     1174 2024-01-15 11:51:25.618027 gigachain_core-0.1.9/langchain_core/load/dump.py
--rw-r--r--   0        0        0     5333 2024-01-15 11:51:25.620967 gigachain_core-0.1.9/langchain_core/load/load.py
--rw-r--r--   0        0        0    16194 2024-01-15 11:51:25.622324 gigachain_core-0.1.9/langchain_core/load/mapping.py
--rw-r--r--   0        0        0     6237 2024-01-10 09:04:40.251663 gigachain_core-0.1.9/langchain_core/load/serializable.py
--rw-r--r--   0        0        0     2019 2023-12-18 12:05:46.629384 gigachain_core-0.1.9/langchain_core/memory.py
--rw-r--r--   0        0        0     4642 2024-01-15 11:51:25.623839 gigachain_core-0.1.9/langchain_core/messages/__init__.py
--rw-r--r--   0        0        0     1754 2023-12-18 12:05:46.632061 gigachain_core-0.1.9/langchain_core/messages/ai.py
--rw-r--r--   0        0        0     6254 2024-01-10 09:04:40.253105 gigachain_core-0.1.9/langchain_core/messages/base.py
--rw-r--r--   0        0        0     2047 2023-12-18 12:05:46.633256 gigachain_core-0.1.9/langchain_core/messages/chat.py
--rw-r--r--   0        0        0     1759 2023-12-18 12:05:46.633621 gigachain_core-0.1.9/langchain_core/messages/function.py
--rw-r--r--   0        0        0     1093 2023-12-18 12:05:46.633934 gigachain_core-0.1.9/langchain_core/messages/human.py
--rw-r--r--   0        0        0     1046 2023-12-18 12:05:46.634652 gigachain_core-0.1.9/langchain_core/messages/system.py
--rw-r--r--   0        0        0     1753 2023-12-18 12:05:46.635449 gigachain_core-0.1.9/langchain_core/messages/tool.py
--rw-r--r--   0        0        0     1044 2024-01-15 11:51:25.624790 gigachain_core-0.1.9/langchain_core/output_parsers/__init__.py
--rw-r--r--   0        0        0     9740 2024-01-15 11:51:25.626109 gigachain_core-0.1.9/langchain_core/output_parsers/base.py
--rw-r--r--   0        0        0      527 2024-01-15 11:51:25.626544 gigachain_core-0.1.9/langchain_core/output_parsers/format_instructions.py
--rw-r--r--   0        0        0     7839 2024-01-15 11:51:25.627941 gigachain_core-0.1.9/langchain_core/output_parsers/json.py
--rw-r--r--   0        0        0     5507 2024-01-15 11:51:25.629059 gigachain_core-0.1.9/langchain_core/output_parsers/list.py
--rw-r--r--   0        0        0      789 2023-12-18 12:05:46.638058 gigachain_core-0.1.9/langchain_core/output_parsers/string.py
--rw-r--r--   0        0        0     4466 2023-12-18 12:05:46.638784 gigachain_core-0.1.9/langchain_core/output_parsers/transform.py
--rw-r--r--   0        0        0     6056 2024-01-15 11:51:25.630025 gigachain_core-0.1.9/langchain_core/output_parsers/xml.py
--rw-r--r--   0        0        0      482 2023-12-18 12:05:46.639458 gigachain_core-0.1.9/langchain_core/outputs/__init__.py
--rw-r--r--   0        0        0     2633 2023-12-18 12:05:46.639895 gigachain_core-0.1.9/langchain_core/outputs/chat_generation.py
--rw-r--r--   0        0        0      511 2023-12-18 12:05:46.640270 gigachain_core-0.1.9/langchain_core/outputs/chat_result.py
--rw-r--r--   0        0        0     1848 2023-12-18 12:05:46.640638 gigachain_core-0.1.9/langchain_core/outputs/generation.py
--rw-r--r--   0        0        0     2448 2023-12-18 12:05:46.640994 gigachain_core-0.1.9/langchain_core/outputs/llm_result.py
--rw-r--r--   0        0        0      295 2023-12-18 12:05:46.641373 gigachain_core-0.1.9/langchain_core/outputs/run_info.py
--rw-r--r--   0        0        0     2662 2023-12-18 12:05:46.641779 gigachain_core-0.1.9/langchain_core/prompt_values.py
--rw-r--r--   0        0        0     2581 2023-12-18 12:05:46.642206 gigachain_core-0.1.9/langchain_core/prompts/__init__.py
--rw-r--r--   0        0        0     8833 2024-01-10 09:04:40.259515 gigachain_core-0.1.9/langchain_core/prompts/base.py
--rw-r--r--   0        0        0    25391 2024-01-10 09:04:40.260398 gigachain_core-0.1.9/langchain_core/prompts/chat.py
--rw-r--r--   0        0        0    11888 2024-01-15 11:51:25.631091 gigachain_core-0.1.9/langchain_core/prompts/few_shot.py
--rw-r--r--   0        0        0     5817 2023-12-18 12:05:46.650203 gigachain_core-0.1.9/langchain_core/prompts/few_shot_with_templates.py
--rw-r--r--   0        0        0     6357 2023-12-18 12:05:46.651785 gigachain_core-0.1.9/langchain_core/prompts/loading.py
--rw-r--r--   0        0        0     2498 2023-12-18 12:05:46.656035 gigachain_core-0.1.9/langchain_core/prompts/pipeline.py
--rw-r--r--   0        0        0     9833 2024-01-15 11:51:25.632149 gigachain_core-0.1.9/langchain_core/prompts/prompt.py
--rw-r--r--   0        0        0     5684 2023-12-18 12:05:46.657304 gigachain_core-0.1.9/langchain_core/prompts/string.py
--rw-r--r--   0        0        0        0 2023-12-18 12:05:46.657488 gigachain_core-0.1.9/langchain_core/py.typed
--rw-r--r--   0        0        0      927 2023-12-18 12:05:46.657935 gigachain_core-0.1.9/langchain_core/pydantic_v1/__init__.py
--rw-r--r--   0        0        0      134 2023-12-18 12:05:46.658853 gigachain_core-0.1.9/langchain_core/pydantic_v1/dataclasses.py
--rw-r--r--   0        0        0      120 2023-12-18 12:05:46.659286 gigachain_core-0.1.9/langchain_core/pydantic_v1/main.py
--rw-r--r--   0        0        0    10835 2024-01-15 11:51:25.633405 gigachain_core-0.1.9/langchain_core/retrievers.py
--rw-r--r--   0        0        0     2184 2024-01-15 11:51:25.634897 gigachain_core-0.1.9/langchain_core/runnables/__init__.py
--rw-r--r--   0        0        0   143823 2024-01-15 11:51:25.638702 gigachain_core-0.1.9/langchain_core/runnables/base.py
--rw-r--r--   0        0        0    14400 2024-01-10 09:04:40.265078 gigachain_core-0.1.9/langchain_core/runnables/branch.py
--rw-r--r--   0        0        0    16801 2024-01-15 11:51:25.640474 gigachain_core-0.1.9/langchain_core/runnables/config.py
--rw-r--r--   0        0        0    16031 2024-01-15 11:51:25.642263 gigachain_core-0.1.9/langchain_core/runnables/configurable.py
--rw-r--r--   0        0        0    11862 2023-12-18 12:05:46.667535 gigachain_core-0.1.9/langchain_core/runnables/fallbacks.py
--rw-r--r--   0        0        0     5044 2024-01-10 09:04:40.266898 gigachain_core-0.1.9/langchain_core/runnables/graph.py
--rw-r--r--   0        0        0     8703 2024-01-10 09:04:40.267252 gigachain_core-0.1.9/langchain_core/runnables/graph_draw.py
--rw-r--r--   0        0        0    15977 2024-01-15 11:51:25.643796 gigachain_core-0.1.9/langchain_core/runnables/history.py
--rw-r--r--   0        0        0    21912 2024-01-15 11:51:25.645070 gigachain_core-0.1.9/langchain_core/runnables/passthrough.py
--rw-r--r--   0        0        0    11952 2023-12-18 12:05:46.671577 gigachain_core-0.1.9/langchain_core/runnables/retry.py
--rw-r--r--   0        0        0     6274 2023-12-18 12:05:46.672074 gigachain_core-0.1.9/langchain_core/runnables/router.py
--rw-r--r--   0        0        0    12554 2024-01-15 11:51:25.646185 gigachain_core-0.1.9/langchain_core/runnables/utils.py
--rw-r--r--   0        0        0     1647 2023-12-18 12:05:46.673359 gigachain_core-0.1.9/langchain_core/stores.py
--rw-r--r--   0        0        0     1604 2024-01-15 11:51:25.646707 gigachain_core-0.1.9/langchain_core/sys_info.py
--rw-r--r--   0        0        0    30198 2024-01-15 11:51:25.647602 gigachain_core-0.1.9/langchain_core/tools.py
--rw-r--r--   0        0        0      598 2023-12-18 12:05:46.674639 gigachain_core-0.1.9/langchain_core/tracers/__init__.py
--rw-r--r--   0        0        0    18584 2024-01-15 11:51:25.649094 gigachain_core-0.1.9/langchain_core/tracers/base.py
--rw-r--r--   0        0        0     7626 2024-01-15 11:51:25.650476 gigachain_core-0.1.9/langchain_core/tracers/context.py
--rw-r--r--   0        0        0     8220 2023-12-18 12:05:46.676253 gigachain_core-0.1.9/langchain_core/tracers/evaluation.py
--rw-r--r--   0        0        0     9208 2024-01-15 11:51:25.651383 gigachain_core-0.1.9/langchain_core/tracers/langchain.py
--rw-r--r--   0        0        0     7467 2024-01-15 11:51:25.652669 gigachain_core-0.1.9/langchain_core/tracers/langchain_v1.py
--rw-r--r--   0        0        0    11231 2024-01-15 11:51:25.653683 gigachain_core-0.1.9/langchain_core/tracers/log_stream.py
--rw-r--r--   0        0        0     1706 2024-01-10 09:04:40.273121 gigachain_core-0.1.9/langchain_core/tracers/root_listeners.py
--rw-r--r--   0        0        0     1532 2023-12-18 12:05:46.679787 gigachain_core-0.1.9/langchain_core/tracers/run_collector.py
--rw-r--r--   0        0        0     4265 2024-01-15 11:51:25.654740 gigachain_core-0.1.9/langchain_core/tracers/schemas.py
--rw-r--r--   0        0        0     6186 2023-12-18 12:05:46.681272 gigachain_core-0.1.9/langchain_core/tracers/stdout.py
--rw-r--r--   0        0        0     1232 2023-12-18 12:05:46.681692 gigachain_core-0.1.9/langchain_core/utils/__init__.py
--rw-r--r--   0        0        0     7198 2023-12-18 12:05:46.682359 gigachain_core-0.1.9/langchain_core/utils/aiter.py
--rw-r--r--   0        0        0     1297 2024-01-10 09:04:40.273915 gigachain_core-0.1.9/langchain_core/utils/env.py
--rw-r--r--   0        0        0      907 2024-01-10 09:04:40.274964 gigachain_core-0.1.9/langchain_core/utils/formatting.py
--rw-r--r--   0        0        0     6666 2024-01-15 11:51:25.655416 gigachain_core-0.1.9/langchain_core/utils/function_calling.py
--rw-r--r--   0        0        0     3090 2024-01-15 11:51:25.656309 gigachain_core-0.1.9/langchain_core/utils/html.py
--rw-r--r--   0        0        0     1289 2023-12-18 12:05:46.685205 gigachain_core-0.1.9/langchain_core/utils/input.py
--rw-r--r--   0        0        0     5822 2023-12-18 12:05:46.685803 gigachain_core-0.1.9/langchain_core/utils/iter.py
--rw-r--r--   0        0        0     2318 2024-01-15 11:51:25.657132 gigachain_core-0.1.9/langchain_core/utils/json_schema.py
--rw-r--r--   0        0        0     2012 2023-12-18 12:05:46.689559 gigachain_core-0.1.9/langchain_core/utils/loading.py
--rw-r--r--   0        0        0      301 2023-12-18 12:05:46.690144 gigachain_core-0.1.9/langchain_core/utils/pydantic.py
--rw-r--r--   0        0        0      908 2023-12-18 12:05:46.690493 gigachain_core-0.1.9/langchain_core/utils/strings.py
--rw-r--r--   0        0        0     6160 2023-12-18 12:05:46.691034 gigachain_core-0.1.9/langchain_core/utils/utils.py
--rw-r--r--   0        0        0    25692 2024-01-15 11:51:25.658112 gigachain_core-0.1.9/langchain_core/vectorstores.py
--rw-r--r--   0        0        0     2804 2024-01-15 11:51:25.663015 gigachain_core-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     4007 1970-01-01 00:00:00.000000 gigachain_core-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     3047 2024-01-10 09:04:40.240772 gigachain_core-0.1.9.1/README.md
+-rw-r--r--   0        0        0      390 2024-01-15 11:51:25.597152 gigachain_core-0.1.9.1/langchain_core/__init__.py
+-rw-r--r--   0        0        0     1025 2024-01-15 11:51:25.598286 gigachain_core-0.1.9.1/langchain_core/_api/__init__.py
+-rw-r--r--   0        0        0     8977 2024-01-15 11:51:25.599167 gigachain_core-0.1.9.1/langchain_core/_api/beta_decorator.py
+-rw-r--r--   0        0        0    13829 2024-01-15 11:51:25.601616 gigachain_core-0.1.9.1/langchain_core/_api/deprecation.py
+-rw-r--r--   0        0        0      662 2024-01-15 11:51:25.602108 gigachain_core-0.1.9.1/langchain_core/_api/internal.py
+-rw-r--r--   0        0        0      984 2023-12-18 12:05:46.602514 gigachain_core-0.1.9.1/langchain_core/_api/path.py
+-rw-r--r--   0        0        0     6197 2023-12-18 12:05:46.603051 gigachain_core-0.1.9.1/langchain_core/agents.py
+-rw-r--r--   0        0        0        0 2023-12-18 12:05:46.603226 gigachain_core-0.1.9.1/langchain_core/beta/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-18 12:05:46.603462 gigachain_core-0.1.9.1/langchain_core/beta/runnables/__init__.py
+-rw-r--r--   0        0        0    10617 2024-01-15 11:51:25.603332 gigachain_core-0.1.9.1/langchain_core/beta/runnables/context.py
+-rw-r--r--   0        0        0      722 2023-12-18 12:05:46.604982 gigachain_core-0.1.9.1/langchain_core/caches.py
+-rw-r--r--   0        0        0     1852 2023-12-18 12:05:46.605433 gigachain_core-0.1.9.1/langchain_core/callbacks/__init__.py
+-rw-r--r--   0        0        0    16850 2023-12-18 12:05:46.606868 gigachain_core-0.1.9.1/langchain_core/callbacks/base.py
+-rw-r--r--   0        0        0    62827 2024-01-15 11:51:25.606221 gigachain_core-0.1.9.1/langchain_core/callbacks/manager.py
+-rw-r--r--   0        0        0     2256 2023-12-18 12:05:46.607875 gigachain_core-0.1.9.1/langchain_core/callbacks/stdout.py
+-rw-r--r--   0        0        0     2433 2023-12-18 12:05:46.608271 gigachain_core-0.1.9.1/langchain_core/callbacks/streaming_stdout.py
+-rw-r--r--   0        0        0     2493 2024-01-10 09:04:40.242637 gigachain_core-0.1.9.1/langchain_core/chat_history.py
+-rw-r--r--   0        0        0      415 2023-12-18 12:05:46.609079 gigachain_core-0.1.9.1/langchain_core/chat_sessions.py
+-rw-r--r--   0        0        0      176 2023-12-18 12:05:46.612530 gigachain_core-0.1.9.1/langchain_core/documents/__init__.py
+-rw-r--r--   0        0        0      839 2023-12-18 12:05:46.612970 gigachain_core-0.1.9.1/langchain_core/documents/base.py
+-rw-r--r--   0        0        0     2494 2024-01-15 11:51:25.608655 gigachain_core-0.1.9.1/langchain_core/documents/transformers.py
+-rw-r--r--   0        0        0      787 2024-01-15 11:51:25.609545 gigachain_core-0.1.9.1/langchain_core/embeddings.py
+-rw-r--r--   0        0        0      486 2024-01-10 09:04:40.243382 gigachain_core-0.1.9.1/langchain_core/env.py
+-rw-r--r--   0        0        0      571 2023-12-18 12:05:46.615278 gigachain_core-0.1.9.1/langchain_core/example_selectors/__init__.py
+-rw-r--r--   0        0        0      516 2024-01-15 11:51:25.610626 gigachain_core-0.1.9.1/langchain_core/example_selectors/base.py
+-rw-r--r--   0        0        0     2453 2023-12-18 12:05:46.615913 gigachain_core-0.1.9.1/langchain_core/example_selectors/length_based.py
+-rw-r--r--   0        0        0     7143 2024-01-15 11:51:25.612090 gigachain_core-0.1.9.1/langchain_core/example_selectors/semantic_similarity.py
+-rw-r--r--   0        0        0     1869 2023-12-18 12:05:46.617107 gigachain_core-0.1.9.1/langchain_core/exceptions.py
+-rw-r--r--   0        0        0     8376 2023-12-18 12:05:46.619340 gigachain_core-0.1.9.1/langchain_core/globals/__init__.py
+-rw-r--r--   0        0        0      522 2024-01-10 09:04:40.244099 gigachain_core-0.1.9.1/langchain_core/language_models/__init__.py
+-rw-r--r--   0        0        0    10688 2024-01-15 11:51:25.614043 gigachain_core-0.1.9.1/langchain_core/language_models/base.py
+-rw-r--r--   0        0        0    29147 2024-01-15 11:51:25.615176 gigachain_core-0.1.9.1/langchain_core/language_models/chat_models.py
+-rw-r--r--   0        0        0    41173 2024-01-15 11:51:25.616692 gigachain_core-0.1.9.1/langchain_core/language_models/llms.py
+-rw-r--r--   0        0        0      261 2023-12-18 12:05:46.624002 gigachain_core-0.1.9.1/langchain_core/load/__init__.py
+-rw-r--r--   0        0        0     1174 2024-01-15 11:51:25.618027 gigachain_core-0.1.9.1/langchain_core/load/dump.py
+-rw-r--r--   0        0        0     5333 2024-01-15 11:51:25.620967 gigachain_core-0.1.9.1/langchain_core/load/load.py
+-rw-r--r--   0        0        0    16194 2024-01-15 11:51:25.622324 gigachain_core-0.1.9.1/langchain_core/load/mapping.py
+-rw-r--r--   0        0        0     6237 2024-01-10 09:04:40.251663 gigachain_core-0.1.9.1/langchain_core/load/serializable.py
+-rw-r--r--   0        0        0     2019 2023-12-18 12:05:46.629384 gigachain_core-0.1.9.1/langchain_core/memory.py
+-rw-r--r--   0        0        0     4642 2024-01-15 11:51:25.623839 gigachain_core-0.1.9.1/langchain_core/messages/__init__.py
+-rw-r--r--   0        0        0     1754 2023-12-18 12:05:46.632061 gigachain_core-0.1.9.1/langchain_core/messages/ai.py
+-rw-r--r--   0        0        0     6254 2024-01-10 09:04:40.253105 gigachain_core-0.1.9.1/langchain_core/messages/base.py
+-rw-r--r--   0        0        0     2047 2023-12-18 12:05:46.633256 gigachain_core-0.1.9.1/langchain_core/messages/chat.py
+-rw-r--r--   0        0        0     1759 2023-12-18 12:05:46.633621 gigachain_core-0.1.9.1/langchain_core/messages/function.py
+-rw-r--r--   0        0        0     1093 2023-12-18 12:05:46.633934 gigachain_core-0.1.9.1/langchain_core/messages/human.py
+-rw-r--r--   0        0        0     1046 2023-12-18 12:05:46.634652 gigachain_core-0.1.9.1/langchain_core/messages/system.py
+-rw-r--r--   0        0        0     1753 2023-12-18 12:05:46.635449 gigachain_core-0.1.9.1/langchain_core/messages/tool.py
+-rw-r--r--   0        0        0     1044 2024-01-15 11:51:25.624790 gigachain_core-0.1.9.1/langchain_core/output_parsers/__init__.py
+-rw-r--r--   0        0        0     9740 2024-01-15 11:51:25.626109 gigachain_core-0.1.9.1/langchain_core/output_parsers/base.py
+-rw-r--r--   0        0        0      527 2024-01-15 11:51:25.626544 gigachain_core-0.1.9.1/langchain_core/output_parsers/format_instructions.py
+-rw-r--r--   0        0        0     7839 2024-01-15 11:51:25.627941 gigachain_core-0.1.9.1/langchain_core/output_parsers/json.py
+-rw-r--r--   0        0        0     5507 2024-01-15 11:51:25.629059 gigachain_core-0.1.9.1/langchain_core/output_parsers/list.py
+-rw-r--r--   0        0        0      789 2023-12-18 12:05:46.638058 gigachain_core-0.1.9.1/langchain_core/output_parsers/string.py
+-rw-r--r--   0        0        0     4466 2023-12-18 12:05:46.638784 gigachain_core-0.1.9.1/langchain_core/output_parsers/transform.py
+-rw-r--r--   0        0        0     6056 2024-01-15 11:51:25.630025 gigachain_core-0.1.9.1/langchain_core/output_parsers/xml.py
+-rw-r--r--   0        0        0      482 2023-12-18 12:05:46.639458 gigachain_core-0.1.9.1/langchain_core/outputs/__init__.py
+-rw-r--r--   0        0        0     2633 2023-12-18 12:05:46.639895 gigachain_core-0.1.9.1/langchain_core/outputs/chat_generation.py
+-rw-r--r--   0        0        0      511 2023-12-18 12:05:46.640270 gigachain_core-0.1.9.1/langchain_core/outputs/chat_result.py
+-rw-r--r--   0        0        0     1848 2023-12-18 12:05:46.640638 gigachain_core-0.1.9.1/langchain_core/outputs/generation.py
+-rw-r--r--   0        0        0     2448 2023-12-18 12:05:46.640994 gigachain_core-0.1.9.1/langchain_core/outputs/llm_result.py
+-rw-r--r--   0        0        0      295 2023-12-18 12:05:46.641373 gigachain_core-0.1.9.1/langchain_core/outputs/run_info.py
+-rw-r--r--   0        0        0     2662 2023-12-18 12:05:46.641779 gigachain_core-0.1.9.1/langchain_core/prompt_values.py
+-rw-r--r--   0        0        0     2581 2023-12-18 12:05:46.642206 gigachain_core-0.1.9.1/langchain_core/prompts/__init__.py
+-rw-r--r--   0        0        0     8833 2024-01-10 09:04:40.259515 gigachain_core-0.1.9.1/langchain_core/prompts/base.py
+-rw-r--r--   0        0        0    25556 2024-01-17 10:19:33.365957 gigachain_core-0.1.9.1/langchain_core/prompts/chat.py
+-rw-r--r--   0        0        0    11888 2024-01-15 11:51:25.631091 gigachain_core-0.1.9.1/langchain_core/prompts/few_shot.py
+-rw-r--r--   0        0        0     5817 2023-12-18 12:05:46.650203 gigachain_core-0.1.9.1/langchain_core/prompts/few_shot_with_templates.py
+-rw-r--r--   0        0        0     6355 2024-01-17 10:19:33.363654 gigachain_core-0.1.9.1/langchain_core/prompts/loading.py
+-rw-r--r--   0        0        0     2498 2023-12-18 12:05:46.656035 gigachain_core-0.1.9.1/langchain_core/prompts/pipeline.py
+-rw-r--r--   0        0        0     9833 2024-01-15 11:51:25.632149 gigachain_core-0.1.9.1/langchain_core/prompts/prompt.py
+-rw-r--r--   0        0        0     5684 2023-12-18 12:05:46.657304 gigachain_core-0.1.9.1/langchain_core/prompts/string.py
+-rw-r--r--   0        0        0        0 2023-12-18 12:05:46.657488 gigachain_core-0.1.9.1/langchain_core/py.typed
+-rw-r--r--   0        0        0      927 2023-12-18 12:05:46.657935 gigachain_core-0.1.9.1/langchain_core/pydantic_v1/__init__.py
+-rw-r--r--   0        0        0      134 2023-12-18 12:05:46.658853 gigachain_core-0.1.9.1/langchain_core/pydantic_v1/dataclasses.py
+-rw-r--r--   0        0        0      120 2023-12-18 12:05:46.659286 gigachain_core-0.1.9.1/langchain_core/pydantic_v1/main.py
+-rw-r--r--   0        0        0    10835 2024-01-15 11:51:25.633405 gigachain_core-0.1.9.1/langchain_core/retrievers.py
+-rw-r--r--   0        0        0     2184 2024-01-15 11:51:25.634897 gigachain_core-0.1.9.1/langchain_core/runnables/__init__.py
+-rw-r--r--   0        0        0   143823 2024-01-15 11:51:25.638702 gigachain_core-0.1.9.1/langchain_core/runnables/base.py
+-rw-r--r--   0        0        0    14400 2024-01-10 09:04:40.265078 gigachain_core-0.1.9.1/langchain_core/runnables/branch.py
+-rw-r--r--   0        0        0    16801 2024-01-15 11:51:25.640474 gigachain_core-0.1.9.1/langchain_core/runnables/config.py
+-rw-r--r--   0        0        0    16031 2024-01-15 11:51:25.642263 gigachain_core-0.1.9.1/langchain_core/runnables/configurable.py
+-rw-r--r--   0        0        0    11862 2023-12-18 12:05:46.667535 gigachain_core-0.1.9.1/langchain_core/runnables/fallbacks.py
+-rw-r--r--   0        0        0     5044 2024-01-10 09:04:40.266898 gigachain_core-0.1.9.1/langchain_core/runnables/graph.py
+-rw-r--r--   0        0        0     8703 2024-01-10 09:04:40.267252 gigachain_core-0.1.9.1/langchain_core/runnables/graph_draw.py
+-rw-r--r--   0        0        0    15977 2024-01-15 11:51:25.643796 gigachain_core-0.1.9.1/langchain_core/runnables/history.py
+-rw-r--r--   0        0        0    21912 2024-01-15 11:51:25.645070 gigachain_core-0.1.9.1/langchain_core/runnables/passthrough.py
+-rw-r--r--   0        0        0    11952 2023-12-18 12:05:46.671577 gigachain_core-0.1.9.1/langchain_core/runnables/retry.py
+-rw-r--r--   0        0        0     6274 2023-12-18 12:05:46.672074 gigachain_core-0.1.9.1/langchain_core/runnables/router.py
+-rw-r--r--   0        0        0    12554 2024-01-15 11:51:25.646185 gigachain_core-0.1.9.1/langchain_core/runnables/utils.py
+-rw-r--r--   0        0        0     1647 2023-12-18 12:05:46.673359 gigachain_core-0.1.9.1/langchain_core/stores.py
+-rw-r--r--   0        0        0     1604 2024-01-15 11:51:25.646707 gigachain_core-0.1.9.1/langchain_core/sys_info.py
+-rw-r--r--   0        0        0    30198 2024-01-15 11:51:25.647602 gigachain_core-0.1.9.1/langchain_core/tools.py
+-rw-r--r--   0        0        0      598 2023-12-18 12:05:46.674639 gigachain_core-0.1.9.1/langchain_core/tracers/__init__.py
+-rw-r--r--   0        0        0    18584 2024-01-15 11:51:25.649094 gigachain_core-0.1.9.1/langchain_core/tracers/base.py
+-rw-r--r--   0        0        0     7626 2024-01-15 11:51:25.650476 gigachain_core-0.1.9.1/langchain_core/tracers/context.py
+-rw-r--r--   0        0        0     8220 2023-12-18 12:05:46.676253 gigachain_core-0.1.9.1/langchain_core/tracers/evaluation.py
+-rw-r--r--   0        0        0     9208 2024-01-15 11:51:25.651383 gigachain_core-0.1.9.1/langchain_core/tracers/langchain.py
+-rw-r--r--   0        0        0     7467 2024-01-15 11:51:25.652669 gigachain_core-0.1.9.1/langchain_core/tracers/langchain_v1.py
+-rw-r--r--   0        0        0    11231 2024-01-15 11:51:25.653683 gigachain_core-0.1.9.1/langchain_core/tracers/log_stream.py
+-rw-r--r--   0        0        0     1706 2024-01-10 09:04:40.273121 gigachain_core-0.1.9.1/langchain_core/tracers/root_listeners.py
+-rw-r--r--   0        0        0     1532 2023-12-18 12:05:46.679787 gigachain_core-0.1.9.1/langchain_core/tracers/run_collector.py
+-rw-r--r--   0        0        0     4265 2024-01-15 11:51:25.654740 gigachain_core-0.1.9.1/langchain_core/tracers/schemas.py
+-rw-r--r--   0        0        0     6186 2023-12-18 12:05:46.681272 gigachain_core-0.1.9.1/langchain_core/tracers/stdout.py
+-rw-r--r--   0        0        0     1232 2023-12-18 12:05:46.681692 gigachain_core-0.1.9.1/langchain_core/utils/__init__.py
+-rw-r--r--   0        0        0     7198 2023-12-18 12:05:46.682359 gigachain_core-0.1.9.1/langchain_core/utils/aiter.py
+-rw-r--r--   0        0        0     1297 2024-01-10 09:04:40.273915 gigachain_core-0.1.9.1/langchain_core/utils/env.py
+-rw-r--r--   0        0        0      907 2024-01-10 09:04:40.274964 gigachain_core-0.1.9.1/langchain_core/utils/formatting.py
+-rw-r--r--   0        0        0     6666 2024-01-15 11:51:25.655416 gigachain_core-0.1.9.1/langchain_core/utils/function_calling.py
+-rw-r--r--   0        0        0     3090 2024-01-15 11:51:25.656309 gigachain_core-0.1.9.1/langchain_core/utils/html.py
+-rw-r--r--   0        0        0     1289 2023-12-18 12:05:46.685205 gigachain_core-0.1.9.1/langchain_core/utils/input.py
+-rw-r--r--   0        0        0     5822 2023-12-18 12:05:46.685803 gigachain_core-0.1.9.1/langchain_core/utils/iter.py
+-rw-r--r--   0        0        0     2318 2024-01-15 11:51:25.657132 gigachain_core-0.1.9.1/langchain_core/utils/json_schema.py
+-rw-r--r--   0        0        0     2012 2023-12-18 12:05:46.689559 gigachain_core-0.1.9.1/langchain_core/utils/loading.py
+-rw-r--r--   0        0        0      301 2023-12-18 12:05:46.690144 gigachain_core-0.1.9.1/langchain_core/utils/pydantic.py
+-rw-r--r--   0        0        0      908 2023-12-18 12:05:46.690493 gigachain_core-0.1.9.1/langchain_core/utils/strings.py
+-rw-r--r--   0        0        0     6160 2023-12-18 12:05:46.691034 gigachain_core-0.1.9.1/langchain_core/utils/utils.py
+-rw-r--r--   0        0        0    25692 2024-01-15 13:18:28.709684 gigachain_core-0.1.9.1/langchain_core/vectorstores.py
+-rw-r--r--   0        0        0     2806 2024-01-17 10:40:26.854514 gigachain_core-0.1.9.1/pyproject.toml
+-rw-r--r--   0        0        0     4009 1970-01-01 00:00:00.000000 gigachain_core-0.1.9.1/PKG-INFO
```

### Comparing `gigachain_core-0.1.9/README.md` & `gigachain_core-0.1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/_api/__init__.py` & `gigachain_core-0.1.9.1/langchain_core/_api/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/_api/beta_decorator.py` & `gigachain_core-0.1.9.1/langchain_core/_api/beta_decorator.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/_api/deprecation.py` & `gigachain_core-0.1.9.1/langchain_core/_api/deprecation.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/_api/internal.py` & `gigachain_core-0.1.9.1/langchain_core/_api/internal.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/_api/path.py` & `gigachain_core-0.1.9.1/langchain_core/_api/path.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/agents.py` & `gigachain_core-0.1.9.1/langchain_core/agents.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/beta/runnables/context.py` & `gigachain_core-0.1.9.1/langchain_core/beta/runnables/context.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/caches.py` & `gigachain_core-0.1.9.1/langchain_core/caches.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/callbacks/__init__.py` & `gigachain_core-0.1.9.1/langchain_core/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/callbacks/base.py` & `gigachain_core-0.1.9.1/langchain_core/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/callbacks/manager.py` & `gigachain_core-0.1.9.1/langchain_core/callbacks/manager.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/callbacks/stdout.py` & `gigachain_core-0.1.9.1/langchain_core/callbacks/stdout.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/callbacks/streaming_stdout.py` & `gigachain_core-0.1.9.1/langchain_core/callbacks/streaming_stdout.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/chat_history.py` & `gigachain_core-0.1.9.1/langchain_core/chat_history.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/documents/base.py` & `gigachain_core-0.1.9.1/langchain_core/documents/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/documents/transformers.py` & `gigachain_core-0.1.9.1/langchain_core/documents/transformers.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/embeddings.py` & `gigachain_core-0.1.9.1/langchain_core/embeddings.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/example_selectors/__init__.py` & `gigachain_core-0.1.9.1/langchain_core/example_selectors/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/example_selectors/base.py` & `gigachain_core-0.1.9.1/langchain_core/example_selectors/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/example_selectors/length_based.py` & `gigachain_core-0.1.9.1/langchain_core/example_selectors/length_based.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/example_selectors/semantic_similarity.py` & `gigachain_core-0.1.9.1/langchain_core/example_selectors/semantic_similarity.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/exceptions.py` & `gigachain_core-0.1.9.1/langchain_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/globals/__init__.py` & `gigachain_core-0.1.9.1/langchain_core/globals/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/language_models/__init__.py` & `gigachain_core-0.1.9.1/langchain_core/language_models/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/language_models/base.py` & `gigachain_core-0.1.9.1/langchain_core/language_models/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/language_models/chat_models.py` & `gigachain_core-0.1.9.1/langchain_core/language_models/chat_models.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/language_models/llms.py` & `gigachain_core-0.1.9.1/langchain_core/language_models/llms.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/load/dump.py` & `gigachain_core-0.1.9.1/langchain_core/load/dump.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/load/load.py` & `gigachain_core-0.1.9.1/langchain_core/load/load.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/load/mapping.py` & `gigachain_core-0.1.9.1/langchain_core/load/mapping.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/load/serializable.py` & `gigachain_core-0.1.9.1/langchain_core/load/serializable.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/memory.py` & `gigachain_core-0.1.9.1/langchain_core/memory.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/messages/__init__.py` & `gigachain_core-0.1.9.1/langchain_core/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/messages/ai.py` & `gigachain_core-0.1.9.1/langchain_core/messages/ai.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/messages/base.py` & `gigachain_core-0.1.9.1/langchain_core/messages/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/messages/chat.py` & `gigachain_core-0.1.9.1/langchain_core/messages/chat.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/messages/function.py` & `gigachain_core-0.1.9.1/langchain_core/messages/function.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/messages/human.py` & `gigachain_core-0.1.9.1/langchain_core/messages/human.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/messages/system.py` & `gigachain_core-0.1.9.1/langchain_core/messages/system.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/messages/tool.py` & `gigachain_core-0.1.9.1/langchain_core/messages/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/output_parsers/__init__.py` & `gigachain_core-0.1.9.1/langchain_core/output_parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/output_parsers/base.py` & `gigachain_core-0.1.9.1/langchain_core/output_parsers/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/output_parsers/format_instructions.py` & `gigachain_core-0.1.9.1/langchain_core/output_parsers/format_instructions.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/output_parsers/json.py` & `gigachain_core-0.1.9.1/langchain_core/output_parsers/json.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/output_parsers/list.py` & `gigachain_core-0.1.9.1/langchain_core/output_parsers/list.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/output_parsers/string.py` & `gigachain_core-0.1.9.1/langchain_core/output_parsers/string.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/output_parsers/transform.py` & `gigachain_core-0.1.9.1/langchain_core/output_parsers/transform.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/output_parsers/xml.py` & `gigachain_core-0.1.9.1/langchain_core/output_parsers/xml.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/outputs/chat_generation.py` & `gigachain_core-0.1.9.1/langchain_core/outputs/chat_generation.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/outputs/generation.py` & `gigachain_core-0.1.9.1/langchain_core/outputs/generation.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/outputs/llm_result.py` & `gigachain_core-0.1.9.1/langchain_core/outputs/llm_result.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/prompt_values.py` & `gigachain_core-0.1.9.1/langchain_core/prompt_values.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/prompts/__init__.py` & `gigachain_core-0.1.9.1/langchain_core/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/prompts/base.py` & `gigachain_core-0.1.9.1/langchain_core/prompts/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/prompts/chat.py` & `gigachain_core-0.1.9.1/langchain_core/prompts/chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -528,16 +528,15 @@
         Returns:
             a chat prompt template
         """
         return cls.from_messages(string_messages)
 
     @classmethod
     def from_messages(
-        cls,
-        messages: Sequence[MessageLikeRepresentation],
+        cls, messages: Sequence[MessageLikeRepresentation], **config: Any
     ) -> ChatPromptTemplate:
         """Create a chat prompt template from a variety of message formats.
 
         Examples:
 
             Instantiation from a list of message templates:
 
@@ -565,15 +564,15 @@
                   (message type, template); e.g., ("human", "{user_input}"),
                   (4) 2-tuple of (message class, template), (4) a string which is
                   shorthand for ("human", template); e.g., "{user_input}"
 
         Returns:
             a chat prompt template
         """
-        _messages = [_convert_to_message(message) for message in messages]
+        _messages = [_convert_to_message(message, **config) for message in messages]
 
         # Automatically infer input variables from messages
         input_vars: Set[str] = set()
         for _message in _messages:
             if isinstance(
                 _message, (BaseChatPromptTemplate, BaseMessagePromptTemplate)
             ):
@@ -699,43 +698,43 @@
         Args:
             file_path: path to file.
         """
         raise NotImplementedError()
 
 
 def _create_template_from_message_type(
-    message_type: str, template: str
+    message_type: str, template: str, **config: Any
 ) -> BaseMessagePromptTemplate:
     """Create a message prompt template from a message type and template string.
 
     Args:
         message_type: str the type of the message template (e.g., "human", "ai", etc.)
         template: str the template string.
 
     Returns:
         a message prompt template of the appropriate type.
     """
     if message_type in ("human", "user"):
         message: BaseMessagePromptTemplate = HumanMessagePromptTemplate.from_template(
-            template
+            template, **config
         )
     elif message_type in ("ai", "assistant"):
-        message = AIMessagePromptTemplate.from_template(template)
+        message = AIMessagePromptTemplate.from_template(template, **config)
     elif message_type == "system":
-        message = SystemMessagePromptTemplate.from_template(template)
+        message = SystemMessagePromptTemplate.from_template(template, **config)
     else:
         raise ValueError(
             f"Unexpected message type: {message_type}. Use one of 'human',"
             f" 'user', 'ai', 'assistant', or 'system'."
         )
     return message
 
 
 def _convert_to_message(
-    message: MessageLikeRepresentation,
+    message: MessageLikeRepresentation, **config: Any
 ) -> Union[BaseMessage, BaseMessagePromptTemplate, BaseChatPromptTemplate]:
     """Instantiate a message from a variety of message formats.
 
     The message format can be one of the following:
 
     - BaseMessagePromptTemplate
     - BaseMessage
@@ -752,20 +751,24 @@
     if isinstance(message, (BaseMessagePromptTemplate, BaseChatPromptTemplate)):
         _message: Union[
             BaseMessage, BaseMessagePromptTemplate, BaseChatPromptTemplate
         ] = message
     elif isinstance(message, BaseMessage):
         _message = message
     elif isinstance(message, str):
-        _message = _create_template_from_message_type("human", message)
+        _message = _create_template_from_message_type("human", message, **config)
     elif isinstance(message, tuple):
         if len(message) != 2:
             raise ValueError(f"Expected 2-tuple of (role, template), got {message}")
         message_type_str, template = message
         if isinstance(message_type_str, str):
-            _message = _create_template_from_message_type(message_type_str, template)
+            _message = _create_template_from_message_type(
+                message_type_str, template, **config
+            )
         else:
-            _message = message_type_str(prompt=PromptTemplate.from_template(template))
+            _message = message_type_str(
+                prompt=PromptTemplate.from_template(template, **config)
+            )
     else:
         raise NotImplementedError(f"Unsupported message type: {type(message)}")
 
     return _message
```

### Comparing `gigachain_core-0.1.9/langchain_core/prompts/few_shot.py` & `gigachain_core-0.1.9.1/langchain_core/prompts/few_shot.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/prompts/few_shot_with_templates.py` & `gigachain_core-0.1.9.1/langchain_core/prompts/few_shot_with_templates.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/prompts/loading.py` & `gigachain_core-0.1.9.1/langchain_core/prompts/loading.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,23 +153,22 @@
         raise ValueError(f"Got unsupported file type {file_path.suffix}")
     # Load the prompt from the config now.
     return load_prompt_from_config(config)
 
 
 def _load_chat_prompt(config: Dict) -> ChatPromptTemplate:
     """Load chat prompt from config"""
-
     messages = config.pop("messages")
-    template = messages[0]["prompt"].pop("template") if messages else None
     config.pop("input_variables")
-
-    if not template:
-        raise ValueError("Can't load chat prompt without template")
-
-    return ChatPromptTemplate.from_template(template=template, **config)
+    text_messages = []
+    for message in messages:
+        text_messages.append(
+            (message.get("role", "user"), message["prompt"].pop("template"))
+        )
+    return ChatPromptTemplate.from_messages(text_messages, **config)
 
 
 type_to_loader_dict: Dict[str, Callable[[dict], BasePromptTemplate]] = {
     "prompt": _load_prompt,
     "few_shot": _load_few_shot_prompt,
     "chat": _load_chat_prompt,
 }
```

### Comparing `gigachain_core-0.1.9/langchain_core/prompts/pipeline.py` & `gigachain_core-0.1.9.1/langchain_core/prompts/pipeline.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/prompts/prompt.py` & `gigachain_core-0.1.9.1/langchain_core/prompts/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/prompts/string.py` & `gigachain_core-0.1.9.1/langchain_core/prompts/string.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/pydantic_v1/__init__.py` & `gigachain_core-0.1.9.1/langchain_core/pydantic_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/retrievers.py` & `gigachain_core-0.1.9.1/langchain_core/retrievers.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/runnables/__init__.py` & `gigachain_core-0.1.9.1/langchain_core/runnables/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/runnables/base.py` & `gigachain_core-0.1.9.1/langchain_core/runnables/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/runnables/branch.py` & `gigachain_core-0.1.9.1/langchain_core/runnables/branch.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/runnables/config.py` & `gigachain_core-0.1.9.1/langchain_core/runnables/config.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/runnables/configurable.py` & `gigachain_core-0.1.9.1/langchain_core/runnables/configurable.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/runnables/fallbacks.py` & `gigachain_core-0.1.9.1/langchain_core/runnables/fallbacks.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/runnables/graph.py` & `gigachain_core-0.1.9.1/langchain_core/runnables/graph.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/runnables/graph_draw.py` & `gigachain_core-0.1.9.1/langchain_core/runnables/graph_draw.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/runnables/history.py` & `gigachain_core-0.1.9.1/langchain_core/runnables/history.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/runnables/passthrough.py` & `gigachain_core-0.1.9.1/langchain_core/runnables/passthrough.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/runnables/retry.py` & `gigachain_core-0.1.9.1/langchain_core/runnables/retry.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/runnables/router.py` & `gigachain_core-0.1.9.1/langchain_core/runnables/router.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/runnables/utils.py` & `gigachain_core-0.1.9.1/langchain_core/runnables/utils.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/stores.py` & `gigachain_core-0.1.9.1/langchain_core/stores.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/sys_info.py` & `gigachain_core-0.1.9.1/langchain_core/sys_info.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/tools.py` & `gigachain_core-0.1.9.1/langchain_core/tools.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/tracers/__init__.py` & `gigachain_core-0.1.9.1/langchain_core/tracers/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/tracers/base.py` & `gigachain_core-0.1.9.1/langchain_core/tracers/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/tracers/context.py` & `gigachain_core-0.1.9.1/langchain_core/tracers/context.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/tracers/evaluation.py` & `gigachain_core-0.1.9.1/langchain_core/tracers/evaluation.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/tracers/langchain.py` & `gigachain_core-0.1.9.1/langchain_core/tracers/langchain.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/tracers/langchain_v1.py` & `gigachain_core-0.1.9.1/langchain_core/tracers/langchain_v1.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/tracers/log_stream.py` & `gigachain_core-0.1.9.1/langchain_core/tracers/log_stream.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/tracers/root_listeners.py` & `gigachain_core-0.1.9.1/langchain_core/tracers/root_listeners.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/tracers/run_collector.py` & `gigachain_core-0.1.9.1/langchain_core/tracers/run_collector.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/tracers/schemas.py` & `gigachain_core-0.1.9.1/langchain_core/tracers/schemas.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/tracers/stdout.py` & `gigachain_core-0.1.9.1/langchain_core/tracers/stdout.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/utils/__init__.py` & `gigachain_core-0.1.9.1/langchain_core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/utils/aiter.py` & `gigachain_core-0.1.9.1/langchain_core/utils/aiter.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/utils/env.py` & `gigachain_core-0.1.9.1/langchain_core/utils/env.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/utils/formatting.py` & `gigachain_core-0.1.9.1/langchain_core/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/utils/function_calling.py` & `gigachain_core-0.1.9.1/langchain_core/utils/function_calling.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/utils/html.py` & `gigachain_core-0.1.9.1/langchain_core/utils/html.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/utils/input.py` & `gigachain_core-0.1.9.1/langchain_core/utils/input.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/utils/iter.py` & `gigachain_core-0.1.9.1/langchain_core/utils/iter.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/utils/json_schema.py` & `gigachain_core-0.1.9.1/langchain_core/utils/json_schema.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/utils/loading.py` & `gigachain_core-0.1.9.1/langchain_core/utils/loading.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/utils/strings.py` & `gigachain_core-0.1.9.1/langchain_core/utils/strings.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/utils/utils.py` & `gigachain_core-0.1.9.1/langchain_core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/langchain_core/vectorstores.py` & `gigachain_core-0.1.9.1/langchain_core/vectorstores.py`

 * *Files identical despite different names*

### Comparing `gigachain_core-0.1.9/pyproject.toml` & `gigachain_core-0.1.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gigachain-core"
-version = "0.1.9"
+version = "0.1.9.1"
 description = "Building applications with LLMs through composability"
 authors = []
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 packages = [
     {include = "langchain_core"}
```

### Comparing `gigachain_core-0.1.9/PKG-INFO` & `gigachain_core-0.1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gigachain-core
-Version: 0.1.9
+Version: 0.1.9.1
 Summary: Building applications with LLMs through composability
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

