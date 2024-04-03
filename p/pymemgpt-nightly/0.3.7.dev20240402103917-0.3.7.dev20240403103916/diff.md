# Comparing `tmp/pymemgpt_nightly-0.3.7.dev20240402103917.tar.gz` & `tmp/pymemgpt_nightly-0.3.7.dev20240403103916.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymemgpt_nightly-0.3.7.dev20240402103917.tar", max compression
+gzip compressed data, was "pymemgpt_nightly-0.3.7.dev20240403103916.tar", max compression
```

## Comparing `pymemgpt_nightly-0.3.7.dev20240402103917.tar` & `pymemgpt_nightly-0.3.7.dev20240403103916.tar`

### file list

```diff
@@ -1,167 +1,167 @@
--rw-r--r--   0        0        0    10760 2024-04-02 10:39:07.362594 pymemgpt_nightly-0.3.7.dev20240402103917/LICENSE
--rw-r--r--   0        0        0     8249 2024-04-02 10:39:07.362594 pymemgpt_nightly-0.3.7.dev20240402103917/README.md
--rw-r--r--   0        0        0      108 2024-04-02 10:39:17.406518 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/__init__.py
--rw-r--r--   0        0        0       29 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/__main__.py
--rw-r--r--   0        0        0    55407 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/agent.py
--rw-r--r--   0        0        0    10728 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/agent_store/chroma.py
--rw-r--r--   0        0        0    25394 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/agent_store/db.py
--rw-r--r--   0        0        0     5288 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/agent_store/lancedb.py
--rw-r--r--   0        0        0     6390 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/agent_store/storage.py
--rw-r--r--   0        0        0      169 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/autogen/README.md
--rw-r--r--   0        0        0        0 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/autogen/__init__.py
--rw-r--r--   0        0        0     7088 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/autogen/examples/agent_autoreply.py
--rw-r--r--   0        0        0     6813 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/autogen/examples/agent_docs.py
--rw-r--r--   0        0        0     7914 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/autogen/examples/agent_groupchat.py
--rw-r--r--   0        0        0     7375 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/autogen/examples/memgpt_coder_autogen.ipynb
--rw-r--r--   0        0        0     9318 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/autogen/interface.py
--rw-r--r--   0        0        0    20931 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/autogen/memgpt_agent.py
--rw-r--r--   0        0        0     3644 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/benchmark/benchmark.py
--rw-r--r--   0        0        0      536 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/benchmark/constants.py
--rw-r--r--   0        0        0    34724 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/cli/cli.py
--rw-r--r--   0        0        0    40394 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/cli/cli_config.py
--rw-r--r--   0        0        0    10453 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/cli/cli_load.py
--rw-r--r--   0        0        0        0 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/client/__init__.py
--rw-r--r--   0        0        0     3239 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/client/admin.py
--rw-r--r--   0        0        0    26592 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/client/client.py
--rw-r--r--   0        0        0    18729 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/config.py
--rw-r--r--   0        0        0      390 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/configs/memgpt_hosted.json
--rw-r--r--   0        0        0      373 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/configs/openai.json
--rw-r--r--   0        0        0     5364 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/constants.py
--rw-r--r--   0        0        0     4904 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/credentials.py
--rw-r--r--   0        0        0     8455 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/data_sources/connectors.py
--rw-r--r--   0        0        0    23711 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/data_types.py
--rw-r--r--   0        0        0     7601 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/embeddings.py
--rw-r--r--   0        0        0      820 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/errors.py
--rw-r--r--   0        0        0        0 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/functions/__init__.py
--rw-r--r--   0        0        0     7343 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/functions/function_sets/base.py
--rw-r--r--   0        0        0     4629 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/functions/function_sets/extras.py
--rw-r--r--   0        0        0     5626 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/functions/functions.py
--rw-r--r--   0        0        0     5076 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/functions/schema_generator.py
--rw-r--r--   0        0        0        0 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/humans/__init__.py
--rw-r--r--   0        0        0       17 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/humans/examples/basic.txt
--rw-r--r--   0        0        0      305 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/humans/examples/cs_phd.txt
--rw-r--r--   0        0        0    12994 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/interface.py
--rw-r--r--   0        0        0    21252 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/llm_api_tools.py
--rw-r--r--   0        0        0      175 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/README.md
--rw-r--r--   0        0        0        0 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/__init__.py
--rw-r--r--   0        0        0    13519 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/chat_completion_proxy.py
--rw-r--r--   0        0        0      912 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/constants.py
--rw-r--r--   0        0        0     2788 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/function_parser.py
--rw-r--r--   0        0        0        0 2024-04-02 10:39:07.390593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/grammars/__init__.py
--rw-r--r--   0        0        0    56322 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/grammars/gbnf_grammar_generator.py
--rw-r--r--   0        0        0      667 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/grammars/json.gbnf
--rw-r--r--   0        0        0     3255 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/grammars/json_func_calls_with_inner_thoughts.gbnf
--rw-r--r--   0        0        0     3562 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/groq/api.py
--rw-r--r--   0        0        0     7434 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/json_parser.py
--rw-r--r--   0        0        0     2586 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/koboldcpp/api.py
--rw-r--r--   0        0        0      557 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/koboldcpp/settings.py
--rw-r--r--   0        0        0     2492 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/llamacpp/api.py
--rw-r--r--   0        0        0      548 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/llamacpp/settings.py
--rw-r--r--   0        0        0        0 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/llm_chat_completion_wrappers/__init__.py
--rw-r--r--   0        0        0    19913 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/llm_chat_completion_wrappers/airoboros.py
--rw-r--r--   0        0        0    21281 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/llm_chat_completion_wrappers/chatml.py
--rw-r--r--   0        0        0    19975 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/llm_chat_completion_wrappers/configurable_wrapper.py
--rw-r--r--   0        0        0    10300 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/llm_chat_completion_wrappers/dolphin.py
--rw-r--r--   0        0        0     6144 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/llm_chat_completion_wrappers/simple_summary_wrapper.py
--rw-r--r--   0        0        0      419 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/llm_chat_completion_wrappers/wrapper_base.py
--rw-r--r--   0        0        0    14956 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/llm_chat_completion_wrappers/zephyr.py
--rw-r--r--   0        0        0     4630 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/lmstudio/api.py
--rw-r--r--   0        0        0      857 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/lmstudio/settings.py
--rw-r--r--   0        0        0     3660 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/ollama/api.py
--rw-r--r--   0        0        0      894 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/ollama/settings.py
--rw-r--r--   0        0        0        0 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/settings/__init__.py
--rw-r--r--   0        0        0     1222 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/settings/deterministic_mirostat.py
--rw-r--r--   0        0        0     3058 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/settings/settings.py
--rw-r--r--   0        0        0      719 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/settings/simple.py
--rw-r--r--   0        0        0     4846 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/utils.py
--rw-r--r--   0        0        0     2612 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/vllm/api.py
--rw-r--r--   0        0        0     2658 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/webui/api.py
--rw-r--r--   0        0        0     2354 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/webui/legacy_api.py
--rw-r--r--   0        0        0      579 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/webui/legacy_settings.py
--rw-r--r--   0        0        0      593 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/webui/settings.py
--rw-r--r--   0        0        0     1211 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/log.py
--rw-r--r--   0        0        0    19532 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/main.py
--rw-r--r--   0        0        0    19653 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/memory.py
--rw-r--r--   0        0        0    28197 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/metadata.py
--rw-r--r--   0        0        0    31537 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/migrate.py
--rw-r--r--   0        0        0     2517 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/models/chat_completion_request.py
--rw-r--r--   0        0        0     1562 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/models/chat_completion_response.py
--rw-r--r--   0        0        0      356 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/models/embedding_response.py
--rw-r--r--   0        0        0     7977 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/models/openai.py
--rw-r--r--   0        0        0     7902 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/models/pydantic_models.py
--rw-r--r--   0        0        0        0 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/openai_backcompat/__init__.py
--rw-r--r--   0        0        0    13692 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/openai_backcompat/openai_object.py
--rw-r--r--   0        0        0     5882 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/persistence_manager.py
--rw-r--r--   0        0        0        0 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/personas/__init__.py
--rw-r--r--   0        0        0     1849 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/personas/examples/anna_pa.txt
--rw-r--r--   0        0        0     1196 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/personas/examples/google_search_persona.txt
--rw-r--r--   0        0        0      431 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/personas/examples/memgpt_doc.txt
--rw-r--r--   0        0        0      164 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/personas/examples/memgpt_starter.txt
--rw-r--r--   0        0        0     1236 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/personas/examples/sam.txt
--rw-r--r--   0        0        0     1171 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/personas/examples/sam_pov.txt
--rw-r--r--   0        0        0     1053 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/personas/examples/sam_simple_pov_gpt35.txt
--rw-r--r--   0        0        0     8192 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/personas/examples/sqldb/test.db
--rw-r--r--   0        0        0      248 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/presets/examples/memgpt_chat.yaml
--rw-r--r--   0        0        0      247 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/presets/examples/memgpt_docs.yaml
--rw-r--r--   0        0        0      374 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/presets/examples/memgpt_extras.yaml
--rw-r--r--   0        0        0     7575 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/presets/presets.py
--rw-r--r--   0        0        0     2789 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/presets/utils.py
--rw-r--r--   0        0        0        0 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/prompts/__init__.py
--rw-r--r--   0        0        0    12907 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/prompts/gpt_functions.py
--rw-r--r--   0        0        0     1139 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/prompts/gpt_summarize.py
--rw-r--r--   0        0        0     1045 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/prompts/gpt_system.py
--rw-r--r--   0        0        0     4758 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/prompts/system/memgpt_base.txt
--rw-r--r--   0        0        0     5494 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/prompts/system/memgpt_chat.txt
--rw-r--r--   0        0        0     1057 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/prompts/system/memgpt_chat_compressed.txt
--rw-r--r--   0        0        0     4819 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/prompts/system/memgpt_doc.txt
--rw-r--r--   0        0        0     5047 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/prompts/system/memgpt_gpt35_extralong.txt
--rw-r--r--   0        0        0     2967 2024-04-02 10:39:07.394593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/prompts/system/memgpt_intuitive_knowledge.txt
--rw-r--r--   0        0        0     4663 2024-04-02 10:39:07.398594 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/prompts/system/memgpt_modified_chat.txt
--rw-r--r--   0        0        0        0 2024-04-02 10:39:07.398594 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/__init__.py
--rw-r--r--   0        0        0       92 2024-04-02 10:39:07.398594 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/constants.py
--rw-r--r--   0        0        0        0 2024-04-02 10:39:07.398594 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 10:39:07.398594 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/admin/__init__.py
--rw-r--r--   0        0        0     6130 2024-04-02 10:39:07.398594 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/admin/users.py
--rw-r--r--   0        0        0        0 2024-04-02 10:39:07.398594 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/agents/__init__.py
--rw-r--r--   0        0        0     1757 2024-04-02 10:39:07.398594 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/agents/command.py
--rw-r--r--   0        0        0     6138 2024-04-02 10:39:07.398594 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/agents/config.py
--rw-r--r--   0        0        0     5114 2024-04-02 10:39:07.398594 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/agents/index.py
--rw-r--r--   0        0        0     7640 2024-04-02 10:39:07.398594 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/agents/memory.py
--rw-r--r--   0        0        0     8583 2024-04-02 10:39:07.398594 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/agents/message.py
--rw-r--r--   0        0        0        0 2024-04-02 10:39:07.398594 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/auth/__init__.py
--rw-r--r--   0        0        0     1303 2024-04-02 10:39:07.398594 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/auth/index.py
--rw-r--r--   0        0        0      775 2024-04-02 10:39:07.398594 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/auth_token.py
--rw-r--r--   0        0        0        0 2024-04-02 10:39:07.398594 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/config/__init__.py
--rw-r--r--   0        0        0     1136 2024-04-02 10:39:07.398594 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/config/index.py
--rw-r--r--   0        0        0        0 2024-04-02 10:39:07.398594 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/humans/__init__.py
--rw-r--r--   0        0        0     1732 2024-04-02 10:39:07.398594 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/humans/index.py
--rw-r--r--   0        0        0     5482 2024-04-02 10:39:07.398594 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/interface.py
--rw-r--r--   0        0        0        0 2024-04-02 10:39:07.398594 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/models/__init__.py
--rw-r--r--   0        0        0     1401 2024-04-02 10:39:07.398594 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/models/index.py
--rw-r--r--   0        0        0    23956 2024-04-02 10:39:07.398594 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/openai_assistants/assistants.py
--rw-r--r--   0        0        0        0 2024-04-02 10:39:07.398594 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/personas/__init__.py
--rw-r--r--   0        0        0     1795 2024-04-02 10:39:07.398594 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/personas/index.py
--rw-r--r--   0        0        0        0 2024-04-02 10:39:07.398594 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/presets/__init__.py
--rw-r--r--   0        0        0     5014 2024-04-02 10:39:07.398594 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/presets/index.py
--rw-r--r--   0        0        0     9580 2024-04-02 10:39:07.398594 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/server.py
--rw-r--r--   0        0        0        0 2024-04-02 10:39:07.398594 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/sources/__init__.py
--rw-r--r--   0        0        0     8218 2024-04-02 10:39:07.398594 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/sources/index.py
--rw-r--r--   0        0        0      914 2024-04-02 10:39:07.398594 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/static_files.py
--rw-r--r--   0        0        0        0 2024-04-02 10:39:07.398594 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/tools/__init__.py
--rw-r--r--   0        0        0     2082 2024-04-02 10:39:07.398594 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/tools/index.py
--rw-r--r--   0        0        0    63523 2024-04-02 10:39:07.398594 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/server.py
--rw-r--r--   0        0        0    32506 2024-04-02 10:39:07.398594 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/static_files/assets/index-57df4f6c.css
--rw-r--r--   0        0        0   515346 2024-04-02 10:39:07.402593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/static_files/assets/index-f6a3d52a.js
--rw-r--r--   0        0        0    28783 2024-04-02 10:39:07.402593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/static_files/favicon.ico
--rw-r--r--   0        0        0     1199 2024-04-02 10:39:07.402593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/static_files/index.html
--rw-r--r--   0        0        0    85383 2024-04-02 10:39:07.402593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/static_files/memgpt_logo_transparent.png
--rw-r--r--   0        0        0     1667 2024-04-02 10:39:07.402593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/utils.py
--rw-r--r--   0        0        0        0 2024-04-02 10:39:07.402593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/ws_api/__init__.py
--rw-r--r--   0        0        0     4264 2024-04-02 10:39:07.402593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/ws_api/example_client.py
--rw-r--r--   0        0        0     4124 2024-04-02 10:39:07.402593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/ws_api/interface.py
--rw-r--r--   0        0        0     2257 2024-04-02 10:39:07.402593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/ws_api/protocol.py
--rw-r--r--   0        0        0     6122 2024-04-02 10:39:07.402593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/ws_api/server.py
--rw-r--r--   0        0        0     7281 2024-04-02 10:39:07.402593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/system.py
--rw-r--r--   0        0        0    31128 2024-04-02 10:39:07.402593 pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/utils.py
--rw-r--r--   0        0        0     2301 2024-04-02 10:39:17.402518 pymemgpt_nightly-0.3.7.dev20240402103917/pyproject.toml
--rw-r--r--   0        0        0    10842 1970-01-01 00:00:00.000000 pymemgpt_nightly-0.3.7.dev20240402103917/PKG-INFO
+-rw-r--r--   0        0        0    10760 2024-04-03 10:39:06.148132 pymemgpt_nightly-0.3.7.dev20240403103916/LICENSE
+-rw-r--r--   0        0        0     8441 2024-04-03 10:39:06.148132 pymemgpt_nightly-0.3.7.dev20240403103916/README.md
+-rw-r--r--   0        0        0      108 2024-04-03 10:39:16.328214 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/__init__.py
+-rw-r--r--   0        0        0       29 2024-04-03 10:39:06.172132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/__main__.py
+-rw-r--r--   0        0        0    55407 2024-04-03 10:39:06.172132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/agent.py
+-rw-r--r--   0        0        0    10728 2024-04-03 10:39:06.172132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/agent_store/chroma.py
+-rw-r--r--   0        0        0    25394 2024-04-03 10:39:06.172132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/agent_store/db.py
+-rw-r--r--   0        0        0     5288 2024-04-03 10:39:06.172132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/agent_store/lancedb.py
+-rw-r--r--   0        0        0     6390 2024-04-03 10:39:06.172132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/agent_store/storage.py
+-rw-r--r--   0        0        0      169 2024-04-03 10:39:06.172132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/autogen/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 10:39:06.172132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/autogen/__init__.py
+-rw-r--r--   0        0        0     7088 2024-04-03 10:39:06.172132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/autogen/examples/agent_autoreply.py
+-rw-r--r--   0        0        0     6813 2024-04-03 10:39:06.172132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/autogen/examples/agent_docs.py
+-rw-r--r--   0        0        0     7914 2024-04-03 10:39:06.172132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/autogen/examples/agent_groupchat.py
+-rw-r--r--   0        0        0     7375 2024-04-03 10:39:06.172132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/autogen/examples/memgpt_coder_autogen.ipynb
+-rw-r--r--   0        0        0     9318 2024-04-03 10:39:06.172132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/autogen/interface.py
+-rw-r--r--   0        0        0    20931 2024-04-03 10:39:06.172132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/autogen/memgpt_agent.py
+-rw-r--r--   0        0        0     3644 2024-04-03 10:39:06.172132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/benchmark/benchmark.py
+-rw-r--r--   0        0        0      536 2024-04-03 10:39:06.172132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/benchmark/constants.py
+-rw-r--r--   0        0        0    34724 2024-04-03 10:39:06.172132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/cli/cli.py
+-rw-r--r--   0        0        0    40394 2024-04-03 10:39:06.172132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/cli/cli_config.py
+-rw-r--r--   0        0        0    10453 2024-04-03 10:39:06.172132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/cli/cli_load.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/client/__init__.py
+-rw-r--r--   0        0        0     3239 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/client/admin.py
+-rw-r--r--   0        0        0    26592 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/client/client.py
+-rw-r--r--   0        0        0    18729 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/config.py
+-rw-r--r--   0        0        0      390 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/configs/memgpt_hosted.json
+-rw-r--r--   0        0        0      373 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/configs/openai.json
+-rw-r--r--   0        0        0     5364 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/constants.py
+-rw-r--r--   0        0        0     4904 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/credentials.py
+-rw-r--r--   0        0        0     9529 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/data_sources/connectors.py
+-rw-r--r--   0        0        0    23711 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/data_types.py
+-rw-r--r--   0        0        0     7601 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/embeddings.py
+-rw-r--r--   0        0        0      820 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/errors.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/functions/__init__.py
+-rw-r--r--   0        0        0     7343 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/functions/function_sets/base.py
+-rw-r--r--   0        0        0     4629 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/functions/function_sets/extras.py
+-rw-r--r--   0        0        0     5626 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/functions/functions.py
+-rw-r--r--   0        0        0     5433 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/functions/schema_generator.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/humans/__init__.py
+-rw-r--r--   0        0        0       17 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/humans/examples/basic.txt
+-rw-r--r--   0        0        0      305 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/humans/examples/cs_phd.txt
+-rw-r--r--   0        0        0    12994 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/interface.py
+-rw-r--r--   0        0        0    21252 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/llm_api_tools.py
+-rw-r--r--   0        0        0      175 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/__init__.py
+-rw-r--r--   0        0        0    13519 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/chat_completion_proxy.py
+-rw-r--r--   0        0        0      912 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/constants.py
+-rw-r--r--   0        0        0     2788 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/function_parser.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/grammars/__init__.py
+-rw-r--r--   0        0        0    56322 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/grammars/gbnf_grammar_generator.py
+-rw-r--r--   0        0        0      667 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/grammars/json.gbnf
+-rw-r--r--   0        0        0     3255 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/grammars/json_func_calls_with_inner_thoughts.gbnf
+-rw-r--r--   0        0        0     3562 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/groq/api.py
+-rw-r--r--   0        0        0     7434 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/json_parser.py
+-rw-r--r--   0        0        0     2586 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/koboldcpp/api.py
+-rw-r--r--   0        0        0      557 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/koboldcpp/settings.py
+-rw-r--r--   0        0        0     2492 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/llamacpp/api.py
+-rw-r--r--   0        0        0      548 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/llamacpp/settings.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/llm_chat_completion_wrappers/__init__.py
+-rw-r--r--   0        0        0    19913 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/llm_chat_completion_wrappers/airoboros.py
+-rw-r--r--   0        0        0    21281 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/llm_chat_completion_wrappers/chatml.py
+-rw-r--r--   0        0        0    19975 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/llm_chat_completion_wrappers/configurable_wrapper.py
+-rw-r--r--   0        0        0    10300 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/llm_chat_completion_wrappers/dolphin.py
+-rw-r--r--   0        0        0     6144 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/llm_chat_completion_wrappers/simple_summary_wrapper.py
+-rw-r--r--   0        0        0      419 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/llm_chat_completion_wrappers/wrapper_base.py
+-rw-r--r--   0        0        0    14956 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/llm_chat_completion_wrappers/zephyr.py
+-rw-r--r--   0        0        0     4630 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/lmstudio/api.py
+-rw-r--r--   0        0        0      857 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/lmstudio/settings.py
+-rw-r--r--   0        0        0     3660 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/ollama/api.py
+-rw-r--r--   0        0        0      894 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/ollama/settings.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/settings/__init__.py
+-rw-r--r--   0        0        0     1222 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/settings/deterministic_mirostat.py
+-rw-r--r--   0        0        0     3058 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/settings/settings.py
+-rw-r--r--   0        0        0      719 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/settings/simple.py
+-rw-r--r--   0        0        0     4846 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/utils.py
+-rw-r--r--   0        0        0     2612 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/vllm/api.py
+-rw-r--r--   0        0        0     2658 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/webui/api.py
+-rw-r--r--   0        0        0     2354 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/webui/legacy_api.py
+-rw-r--r--   0        0        0      579 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/webui/legacy_settings.py
+-rw-r--r--   0        0        0      593 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/webui/settings.py
+-rw-r--r--   0        0        0     1211 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/log.py
+-rw-r--r--   0        0        0    19532 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/main.py
+-rw-r--r--   0        0        0    19653 2024-04-03 10:39:06.176132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/memory.py
+-rw-r--r--   0        0        0    28197 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/metadata.py
+-rw-r--r--   0        0        0    31537 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/migrate.py
+-rw-r--r--   0        0        0     2517 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/models/chat_completion_request.py
+-rw-r--r--   0        0        0     1562 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/models/chat_completion_response.py
+-rw-r--r--   0        0        0      356 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/models/embedding_response.py
+-rw-r--r--   0        0        0     7977 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/models/openai.py
+-rw-r--r--   0        0        0     7902 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/models/pydantic_models.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/openai_backcompat/__init__.py
+-rw-r--r--   0        0        0    13692 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/openai_backcompat/openai_object.py
+-rw-r--r--   0        0        0     5882 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/persistence_manager.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/personas/__init__.py
+-rw-r--r--   0        0        0     1849 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/personas/examples/anna_pa.txt
+-rw-r--r--   0        0        0     1196 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/personas/examples/google_search_persona.txt
+-rw-r--r--   0        0        0      431 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/personas/examples/memgpt_doc.txt
+-rw-r--r--   0        0        0      164 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/personas/examples/memgpt_starter.txt
+-rw-r--r--   0        0        0     1236 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/personas/examples/sam.txt
+-rw-r--r--   0        0        0     1171 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/personas/examples/sam_pov.txt
+-rw-r--r--   0        0        0     1053 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/personas/examples/sam_simple_pov_gpt35.txt
+-rw-r--r--   0        0        0     8192 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/personas/examples/sqldb/test.db
+-rw-r--r--   0        0        0      248 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/presets/examples/memgpt_chat.yaml
+-rw-r--r--   0        0        0      247 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/presets/examples/memgpt_docs.yaml
+-rw-r--r--   0        0        0      374 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/presets/examples/memgpt_extras.yaml
+-rw-r--r--   0        0        0     7575 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/presets/presets.py
+-rw-r--r--   0        0        0     2789 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/presets/utils.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/prompts/__init__.py
+-rw-r--r--   0        0        0    12907 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/prompts/gpt_functions.py
+-rw-r--r--   0        0        0     1139 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/prompts/gpt_summarize.py
+-rw-r--r--   0        0        0     1045 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/prompts/gpt_system.py
+-rw-r--r--   0        0        0     4758 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/prompts/system/memgpt_base.txt
+-rw-r--r--   0        0        0     5494 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/prompts/system/memgpt_chat.txt
+-rw-r--r--   0        0        0     1057 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/prompts/system/memgpt_chat_compressed.txt
+-rw-r--r--   0        0        0     4819 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/prompts/system/memgpt_doc.txt
+-rw-r--r--   0        0        0     5047 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/prompts/system/memgpt_gpt35_extralong.txt
+-rw-r--r--   0        0        0     2967 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/prompts/system/memgpt_intuitive_knowledge.txt
+-rw-r--r--   0        0        0     4663 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/prompts/system/memgpt_modified_chat.txt
+-rw-r--r--   0        0        0        0 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/__init__.py
+-rw-r--r--   0        0        0       92 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/constants.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/admin/__init__.py
+-rw-r--r--   0        0        0     6130 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/admin/users.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/agents/__init__.py
+-rw-r--r--   0        0        0     1757 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/agents/command.py
+-rw-r--r--   0        0        0     6138 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/agents/config.py
+-rw-r--r--   0        0        0     5114 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/agents/index.py
+-rw-r--r--   0        0        0     7640 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/agents/memory.py
+-rw-r--r--   0        0        0     8583 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/agents/message.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/auth/__init__.py
+-rw-r--r--   0        0        0     1303 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/auth/index.py
+-rw-r--r--   0        0        0      775 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/auth_token.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/config/__init__.py
+-rw-r--r--   0        0        0     1136 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/config/index.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/humans/__init__.py
+-rw-r--r--   0        0        0     1732 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/humans/index.py
+-rw-r--r--   0        0        0     5482 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/interface.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/models/__init__.py
+-rw-r--r--   0        0        0     1401 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/models/index.py
+-rw-r--r--   0        0        0    23956 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/openai_assistants/assistants.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/personas/__init__.py
+-rw-r--r--   0        0        0     1795 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/personas/index.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/presets/__init__.py
+-rw-r--r--   0        0        0     5014 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/presets/index.py
+-rw-r--r--   0        0        0     9580 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/server.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/sources/__init__.py
+-rw-r--r--   0        0        0     8218 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/sources/index.py
+-rw-r--r--   0        0        0      914 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/static_files.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/tools/__init__.py
+-rw-r--r--   0        0        0     2082 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/tools/index.py
+-rw-r--r--   0        0        0    63523 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/server.py
+-rw-r--r--   0        0        0    32506 2024-04-03 10:39:06.180132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/static_files/assets/index-57df4f6c.css
+-rw-r--r--   0        0        0   515346 2024-04-03 10:39:06.184132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/static_files/assets/index-f6a3d52a.js
+-rw-r--r--   0        0        0    28783 2024-04-03 10:39:06.184132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/static_files/favicon.ico
+-rw-r--r--   0        0        0     1199 2024-04-03 10:39:06.184132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/static_files/index.html
+-rw-r--r--   0        0        0    85383 2024-04-03 10:39:06.184132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/static_files/memgpt_logo_transparent.png
+-rw-r--r--   0        0        0     1667 2024-04-03 10:39:06.184132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/utils.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:39:06.184132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/ws_api/__init__.py
+-rw-r--r--   0        0        0     4264 2024-04-03 10:39:06.184132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/ws_api/example_client.py
+-rw-r--r--   0        0        0     4124 2024-04-03 10:39:06.184132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/ws_api/interface.py
+-rw-r--r--   0        0        0     2257 2024-04-03 10:39:06.184132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/ws_api/protocol.py
+-rw-r--r--   0        0        0     6122 2024-04-03 10:39:06.184132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/ws_api/server.py
+-rw-r--r--   0        0        0     7281 2024-04-03 10:39:06.184132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/system.py
+-rw-r--r--   0        0        0    31128 2024-04-03 10:39:06.184132 pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/utils.py
+-rw-r--r--   0        0        0     2301 2024-04-03 10:39:16.328214 pymemgpt_nightly-0.3.7.dev20240403103916/pyproject.toml
+-rw-r--r--   0        0        0    11032 1970-01-01 00:00:00.000000 pymemgpt_nightly-0.3.7.dev20240403103916/PKG-INFO
```

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/LICENSE` & `pymemgpt_nightly-0.3.7.dev20240403103916/LICENSE`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/README.md` & `pymemgpt_nightly-0.3.7.dev20240403103916/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -159,9 +159,12 @@
 
 ## Support
 For issues and feature requests, please [open a GitHub issue](https://github.com/cpacker/MemGPT/issues) or message us on our `#support` channel on [Discord](https://discord.gg/9GEQrxmVyE).
 
 ## Datasets
 Datasets used in our [paper](https://arxiv.org/abs/2310.08560) can be downloaded at [Hugging Face](https://huggingface.co/MemGPT).
 
+## Legal notices
+By using MemGPT and related MemGPT services (such as the MemGPT endpoint or hosted service), you agree to our [privacy policy](PRIVACY.md) and [terms of service](TERMS.md).
+
 ## Roadmap
-You can view (and comment on!) the MemGPT developer roadmap on GitHub: https://github.com/cpacker/MemGPT/issues/1044.
+You can view (and comment on!) the MemGPT developer roadmap on GitHub: https://github.com/cpacker/MemGPT/issues/1200.
```

#### html2text {}

```diff
@@ -91,10 +91,12 @@
 calling capabilities of a model. You can help track what LLMs work well with
 MemGPT by contributing your benchmark results via [this form](https://
 forms.gle/XiBGKEEPFFLNSR348), which will be used to update the spreadsheet. ##
 Support For issues and feature requests, please [open a GitHub issue](https://
 github.com/cpacker/MemGPT/issues) or message us on our `#support` channel on
 [Discord](https://discord.gg/9GEQrxmVyE). ## Datasets Datasets used in our
 [paper](https://arxiv.org/abs/2310.08560) can be downloaded at [Hugging Face]
-(https://huggingface.co/MemGPT). ## Roadmap You can view (and comment on!) the
-MemGPT developer roadmap on GitHub: https://github.com/cpacker/MemGPT/issues/
-1044.
+(https://huggingface.co/MemGPT). ## Legal notices By using MemGPT and related
+MemGPT services (such as the MemGPT endpoint or hosted service), you agree to
+our [privacy policy](PRIVACY.md) and [terms of service](TERMS.md). ## Roadmap
+You can view (and comment on!) the MemGPT developer roadmap on GitHub: https://
+github.com/cpacker/MemGPT/issues/1200.
```

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/agent.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/agent.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/agent_store/chroma.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/agent_store/chroma.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/agent_store/db.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/agent_store/db.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/agent_store/lancedb.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/agent_store/lancedb.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/agent_store/storage.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/agent_store/storage.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/autogen/examples/agent_autoreply.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/autogen/examples/agent_autoreply.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/autogen/examples/agent_docs.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/autogen/examples/agent_docs.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/autogen/examples/agent_groupchat.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/autogen/examples/agent_groupchat.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/autogen/examples/memgpt_coder_autogen.ipynb` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/autogen/examples/memgpt_coder_autogen.ipynb`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/autogen/interface.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/autogen/interface.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/autogen/memgpt_agent.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/autogen/memgpt_agent.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/benchmark/benchmark.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/benchmark/constants.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/benchmark/constants.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/cli/cli.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/cli/cli.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/cli/cli_config.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/cli/cli_config.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/cli/cli_load.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/cli/cli_load.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/client/admin.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/client/admin.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/client/client.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/client/client.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/config.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/config.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/constants.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/constants.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/credentials.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/credentials.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/data_sources/connectors.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/data_sources/connectors.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     ), f"Source and embedding config dimensions must match, got: {source.embedding_dim} and {embedding_config.embedding_dim}."
 
     # embedding model
     embed_model = embedding_model(embedding_config)
 
     # insert passages/documents
     passages = []
+    embedding_to_document_name = {}
     passage_count = 0
     document_count = 0
     for document_text, document_metadata in connector.generate_documents():
         # insert document into storage
         document = Document(
             id=create_uuid_from_string(f"{str(source.id)}_{document_text}"),
             text=document_text,
@@ -50,14 +51,24 @@
         )
         document_count += 1
         if document_store:
             document_store.insert(document)
 
         # generate passages
         for passage_text, passage_metadata in connector.generate_passages([document], chunk_size=embedding_config.embedding_chunk_size):
+
+            # for some reason, llama index parsers sometimes return empty strings
+            if len(passage_text) == 0:
+                typer.secho(
+                    f"Warning: Llama index parser returned empty string, skipping insert of passage with metadata '{passage_metadata}' into VectorDB. You can usually ignore this warning.",
+                    fg=typer.colors.YELLOW,
+                )
+                continue
+
+            # get embedding
             try:
                 embedding = embed_model.get_text_embedding(passage_text)
             except Exception as e:
                 typer.secho(
                     f"Warning: Failed to get embedding for {passage_text} (error: {str(e)}), skipping insert into VectorDB.",
                     fg=typer.colors.YELLOW,
                 )
@@ -71,15 +82,25 @@
                 user_id=source.user_id,
                 data_source=source.name,
                 embedding_dim=source.embedding_dim,
                 embedding_model=source.embedding_model,
                 embedding=embedding,
             )
 
+            hashable_embedding = tuple(passage.embedding)
+            document_name = document.metadata.get("file_path", document.id)
+            if hashable_embedding in embedding_to_document_name:
+                typer.secho(
+                    f"Warning: Duplicate embedding found for passage in {document_name} (already exists in {embedding_to_document_name[hashable_embedding]}), skipping insert into VectorDB.",
+                    fg=typer.colors.YELLOW,
+                )
+                continue
+
             passages.append(passage)
+            embedding_to_document_name[hashable_embedding] = document_name
             if len(passages) >= embedding_config.embedding_chunk_size:
                 # insert passages into passage store
                 passage_store.insert_many(passages)
 
                 passage_count += len(passages)
                 passages = []
```

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/data_types.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/data_types.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/embeddings.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/embeddings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/errors.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/errors.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/functions/function_sets/base.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/functions/function_sets/base.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/functions/function_sets/extras.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/functions/function_sets/extras.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/functions/functions.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/functions/functions.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/functions/schema_generator.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/functions/schema_generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import inspect
 import typing
-from typing import get_args
+from typing import get_args, get_origin
 
 from docstring_parser import parse
 from pydantic import BaseModel
 
 from memgpt.constants import FUNCTION_PARAM_NAME_REQ_HEARTBEAT, FUNCTION_PARAM_TYPE_REQ_HEARTBEAT, FUNCTION_PARAM_DESCRIPTION_REQ_HEARTBEAT
 
 NO_HEARTBEAT_FUNCTIONS = ["send_message", "pause_heartbeats"]
@@ -42,14 +42,15 @@
 
     # Mapping of Python types to JSON schema types
     type_map = {
         int: "integer",
         str: "string",
         bool: "boolean",
         float: "number",
+        list[str]: "array",
         # Add more mappings as needed
     }
     if py_type not in type_map:
         raise ValueError(f"Python type {py_type} has no corresponding JSON schema type")
 
     return type_map.get(py_type, "string")  # Default to "string" if type not in map
 
@@ -117,14 +118,21 @@
                 # "type": "string" if param.annotation == str else str(param.annotation),
                 "type": type_to_json_schema_type(param.annotation) if param.annotation != inspect.Parameter.empty else "string",
                 "description": param_doc.description,
             }
         if param.default == inspect.Parameter.empty:
             schema["parameters"]["required"].append(param.name)
 
+        if get_origin(param.annotation) is list:
+            if get_args(param.annotation)[0] is str:
+                schema["parameters"]["properties"][param.name]["items"] = {"type": "string"}
+
+        if param.annotation == inspect.Parameter.empty:
+            schema["parameters"]["required"].append(param.name)
+
     # append the heartbeat
     if function.__name__ not in NO_HEARTBEAT_FUNCTIONS:
         schema["parameters"]["properties"][FUNCTION_PARAM_NAME_REQ_HEARTBEAT] = {
             "type": FUNCTION_PARAM_TYPE_REQ_HEARTBEAT,
             "description": FUNCTION_PARAM_DESCRIPTION_REQ_HEARTBEAT,
         }
         schema["parameters"]["required"].append(FUNCTION_PARAM_NAME_REQ_HEARTBEAT)
```

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/interface.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/interface.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/llm_api_tools.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/llm_api_tools.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/chat_completion_proxy.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/chat_completion_proxy.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/constants.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/constants.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/function_parser.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/function_parser.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/grammars/gbnf_grammar_generator.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/grammars/gbnf_grammar_generator.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/grammars/json.gbnf` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/grammars/json.gbnf`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/grammars/json_func_calls_with_inner_thoughts.gbnf` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/grammars/json_func_calls_with_inner_thoughts.gbnf`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/groq/api.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/groq/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/json_parser.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/json_parser.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/koboldcpp/api.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/koboldcpp/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/koboldcpp/settings.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/koboldcpp/settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/llamacpp/api.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/llamacpp/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/llamacpp/settings.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/llamacpp/settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/llm_chat_completion_wrappers/airoboros.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/llm_chat_completion_wrappers/airoboros.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/llm_chat_completion_wrappers/chatml.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/llm_chat_completion_wrappers/chatml.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/llm_chat_completion_wrappers/configurable_wrapper.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/llm_chat_completion_wrappers/configurable_wrapper.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/llm_chat_completion_wrappers/dolphin.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/llm_chat_completion_wrappers/dolphin.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/llm_chat_completion_wrappers/simple_summary_wrapper.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/llm_chat_completion_wrappers/simple_summary_wrapper.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/llm_chat_completion_wrappers/zephyr.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/llm_chat_completion_wrappers/zephyr.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/lmstudio/api.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/lmstudio/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/lmstudio/settings.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/lmstudio/settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/ollama/api.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/ollama/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/ollama/settings.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/ollama/settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/settings/deterministic_mirostat.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/settings/deterministic_mirostat.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/settings/settings.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/settings/settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/settings/simple.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/settings/simple.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/utils.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/utils.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/vllm/api.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/vllm/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/webui/api.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/webui/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/webui/legacy_api.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/webui/legacy_api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/webui/legacy_settings.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/webui/legacy_settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/local_llm/webui/settings.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/local_llm/webui/settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/log.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/log.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/main.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/main.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/memory.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/memory.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/metadata.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/metadata.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/migrate.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/migrate.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/models/chat_completion_request.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/models/chat_completion_request.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/models/chat_completion_response.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/models/chat_completion_response.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/models/openai.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/models/openai.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/models/pydantic_models.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/models/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/openai_backcompat/openai_object.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/openai_backcompat/openai_object.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/persistence_manager.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/persistence_manager.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/personas/examples/anna_pa.txt` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/personas/examples/anna_pa.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/personas/examples/google_search_persona.txt` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/personas/examples/google_search_persona.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/personas/examples/sam.txt` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/personas/examples/sam.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/personas/examples/sam_pov.txt` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/personas/examples/sam_pov.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/personas/examples/sam_simple_pov_gpt35.txt` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/personas/examples/sam_simple_pov_gpt35.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/personas/examples/sqldb/test.db` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/personas/examples/sqldb/test.db`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/presets/presets.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/presets/presets.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/presets/utils.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/presets/utils.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/prompts/gpt_functions.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/prompts/gpt_functions.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/prompts/gpt_summarize.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/prompts/gpt_summarize.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/prompts/gpt_system.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/prompts/gpt_system.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/prompts/system/memgpt_base.txt` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/prompts/system/memgpt_base.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/prompts/system/memgpt_chat.txt` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/prompts/system/memgpt_chat.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/prompts/system/memgpt_chat_compressed.txt` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/prompts/system/memgpt_chat_compressed.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/prompts/system/memgpt_doc.txt` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/prompts/system/memgpt_doc.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/prompts/system/memgpt_gpt35_extralong.txt` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/prompts/system/memgpt_gpt35_extralong.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/prompts/system/memgpt_intuitive_knowledge.txt` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/prompts/system/memgpt_intuitive_knowledge.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/prompts/system/memgpt_modified_chat.txt` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/prompts/system/memgpt_modified_chat.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/admin/users.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/admin/users.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/agents/command.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/agents/command.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/agents/config.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/agents/config.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/agents/index.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/agents/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/agents/memory.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/agents/memory.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/agents/message.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/agents/message.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/auth/index.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/auth/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/auth_token.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/auth_token.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/config/index.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/config/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/humans/index.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/humans/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/interface.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/interface.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/models/index.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/models/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/openai_assistants/assistants.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/openai_assistants/assistants.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/personas/index.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/personas/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/presets/index.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/presets/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/server.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/server.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/sources/index.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/sources/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/static_files.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/static_files.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/rest_api/tools/index.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/rest_api/tools/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/server.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/server.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/static_files/assets/index-57df4f6c.css` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/static_files/assets/index-57df4f6c.css`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/static_files/assets/index-f6a3d52a.js` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/static_files/assets/index-f6a3d52a.js`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/static_files/favicon.ico` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/static_files/favicon.ico`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/static_files/index.html` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/static_files/index.html`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/static_files/memgpt_logo_transparent.png` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/static_files/memgpt_logo_transparent.png`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/utils.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/utils.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/ws_api/example_client.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/ws_api/example_client.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/ws_api/interface.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/ws_api/interface.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/ws_api/protocol.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/ws_api/protocol.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/server/ws_api/server.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/server/ws_api/server.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/system.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/system.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/memgpt/utils.py` & `pymemgpt_nightly-0.3.7.dev20240403103916/memgpt/utils.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/pyproject.toml` & `pymemgpt_nightly-0.3.7.dev20240403103916/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymemgpt-nightly"
-version = "0.3.7.dev20240402103917"
+version = "0.3.7.dev20240403103916"
 packages = [
     {include = "memgpt"}
 ]
 description = "Teaching LLMs memory management for unbounded context"
 authors = [
     "MemGPT Team <hi@memgpt.ai>",
 ]
```

### Comparing `pymemgpt_nightly-0.3.7.dev20240402103917/PKG-INFO` & `pymemgpt_nightly-0.3.7.dev20240403103916/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymemgpt-nightly
-Version: 0.3.7.dev20240402103917
+Version: 0.3.7.dev20240403103916
 Summary: Teaching LLMs memory management for unbounded context
 License: Apache License
 Author: MemGPT Team
 Author-email: hi@memgpt.ai
 Requires-Python: >=3.10,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -220,10 +220,12 @@
 
 ## Support
 For issues and feature requests, please [open a GitHub issue](https://github.com/cpacker/MemGPT/issues) or message us on our `#support` channel on [Discord](https://discord.gg/9GEQrxmVyE).
 
 ## Datasets
 Datasets used in our [paper](https://arxiv.org/abs/2310.08560) can be downloaded at [Hugging Face](https://huggingface.co/MemGPT).
 
-## Roadmap
-You can view (and comment on!) the MemGPT developer roadmap on GitHub: https://github.com/cpacker/MemGPT/issues/1044.
+## Legal notices
+By using MemGPT and related MemGPT services (such as the MemGPT endpoint or hosted service), you agree to our [privacy policy](PRIVACY.md) and [terms of service](TERMS.md).
 
+## Roadmap
+You can view (and comment on!) the MemGPT developer roadmap on GitHub: https://github.com/cpacker/MemGPT/issues/1200.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymemgpt-nightly Version: 0.3.7.dev20240402103917
+Metadata-Version: 2.1 Name: pymemgpt-nightly Version: 0.3.7.dev20240403103916
 Summary: Teaching LLMs memory management for unbounded context License: Apache
 License Author: MemGPT Team Author-email: hi@memgpt.ai Requires-Python:
 >=3.10,<3.12 Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Provides-Extra:
 autogen Provides-Extra: dev Provides-Extra: local Provides-Extra: postgres
 Provides-Extra: server Requires-Dist: autoflake (>=2.3.0,<3.0.0) ; extra ==
@@ -128,10 +128,12 @@
 calling capabilities of a model. You can help track what LLMs work well with
 MemGPT by contributing your benchmark results via [this form](https://
 forms.gle/XiBGKEEPFFLNSR348), which will be used to update the spreadsheet. ##
 Support For issues and feature requests, please [open a GitHub issue](https://
 github.com/cpacker/MemGPT/issues) or message us on our `#support` channel on
 [Discord](https://discord.gg/9GEQrxmVyE). ## Datasets Datasets used in our
 [paper](https://arxiv.org/abs/2310.08560) can be downloaded at [Hugging Face]
-(https://huggingface.co/MemGPT). ## Roadmap You can view (and comment on!) the
-MemGPT developer roadmap on GitHub: https://github.com/cpacker/MemGPT/issues/
-1044.
+(https://huggingface.co/MemGPT). ## Legal notices By using MemGPT and related
+MemGPT services (such as the MemGPT endpoint or hosted service), you agree to
+our [privacy policy](PRIVACY.md) and [terms of service](TERMS.md). ## Roadmap
+You can view (and comment on!) the MemGPT developer roadmap on GitHub: https://
+github.com/cpacker/MemGPT/issues/1200.
```

