# Comparing `tmp/pymemgpt-0.3.7.tar.gz` & `tmp/pymemgpt-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymemgpt-0.3.7.tar", max compression
+gzip compressed data, was "pymemgpt-0.3.8.tar", max compression
```

## Comparing `pymemgpt-0.3.7.tar` & `pymemgpt-0.3.8.tar`

### file list

```diff
@@ -1,166 +1,167 @@
--rw-r--r--   0        0        0    10760 2024-03-21 05:06:49.257282 pymemgpt-0.3.7/LICENSE
--rw-r--r--   0        0        0     8249 2024-03-21 05:06:49.257282 pymemgpt-0.3.7/README.md
--rw-r--r--   0        0        0      108 2024-03-21 05:06:49.281282 pymemgpt-0.3.7/memgpt/__init__.py
--rw-r--r--   0        0        0       29 2024-03-21 05:06:49.281282 pymemgpt-0.3.7/memgpt/__main__.py
--rw-r--r--   0        0        0    54165 2024-03-21 05:06:49.281282 pymemgpt-0.3.7/memgpt/agent.py
--rw-r--r--   0        0        0    10728 2024-03-21 05:06:49.281282 pymemgpt-0.3.7/memgpt/agent_store/chroma.py
--rw-r--r--   0        0        0    24876 2024-03-21 05:06:49.281282 pymemgpt-0.3.7/memgpt/agent_store/db.py
--rw-r--r--   0        0        0     5288 2024-03-21 05:06:49.281282 pymemgpt-0.3.7/memgpt/agent_store/lancedb.py
--rw-r--r--   0        0        0     6390 2024-03-21 05:06:49.281282 pymemgpt-0.3.7/memgpt/agent_store/storage.py
--rw-r--r--   0        0        0      169 2024-03-21 05:06:49.281282 pymemgpt-0.3.7/memgpt/autogen/README.md
--rw-r--r--   0        0        0        0 2024-03-21 05:06:49.281282 pymemgpt-0.3.7/memgpt/autogen/__init__.py
--rw-r--r--   0        0        0     7088 2024-03-21 05:06:49.281282 pymemgpt-0.3.7/memgpt/autogen/examples/agent_autoreply.py
--rw-r--r--   0        0        0     6813 2024-03-21 05:06:49.281282 pymemgpt-0.3.7/memgpt/autogen/examples/agent_docs.py
--rw-r--r--   0        0        0     7914 2024-03-21 05:06:49.281282 pymemgpt-0.3.7/memgpt/autogen/examples/agent_groupchat.py
--rw-r--r--   0        0        0     7375 2024-03-21 05:06:49.281282 pymemgpt-0.3.7/memgpt/autogen/examples/memgpt_coder_autogen.ipynb
--rw-r--r--   0        0        0     9318 2024-03-21 05:06:49.281282 pymemgpt-0.3.7/memgpt/autogen/interface.py
--rw-r--r--   0        0        0    20931 2024-03-21 05:06:49.281282 pymemgpt-0.3.7/memgpt/autogen/memgpt_agent.py
--rw-r--r--   0        0        0     3644 2024-03-21 05:06:49.281282 pymemgpt-0.3.7/memgpt/benchmark/benchmark.py
--rw-r--r--   0        0        0      536 2024-03-21 05:06:49.281282 pymemgpt-0.3.7/memgpt/benchmark/constants.py
--rw-r--r--   0        0        0    34158 2024-03-21 05:06:49.281282 pymemgpt-0.3.7/memgpt/cli/cli.py
--rw-r--r--   0        0        0    39209 2024-03-21 05:06:49.281282 pymemgpt-0.3.7/memgpt/cli/cli_config.py
--rw-r--r--   0        0        0    10317 2024-03-21 05:06:49.281282 pymemgpt-0.3.7/memgpt/cli/cli_load.py
--rw-r--r--   0        0        0        0 2024-03-21 05:06:49.281282 pymemgpt-0.3.7/memgpt/client/__init__.py
--rw-r--r--   0        0        0     3239 2024-03-21 05:06:49.281282 pymemgpt-0.3.7/memgpt/client/admin.py
--rw-r--r--   0        0        0    26660 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/client/client.py
--rw-r--r--   0        0        0    18739 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/config.py
--rw-r--r--   0        0        0      410 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/configs/memgpt_hosted.json
--rw-r--r--   0        0        0      352 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/configs/openai.json
--rw-r--r--   0        0        0     5364 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/constants.py
--rw-r--r--   0        0        0     4904 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/credentials.py
--rw-r--r--   0        0        0     8455 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/data_sources/connectors.py
--rw-r--r--   0        0        0    23533 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/data_types.py
--rw-r--r--   0        0        0     7601 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/embeddings.py
--rw-r--r--   0        0        0      820 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/errors.py
--rw-r--r--   0        0        0        0 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/functions/__init__.py
--rw-r--r--   0        0        0     7317 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/functions/function_sets/base.py
--rw-r--r--   0        0        0     4629 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/functions/function_sets/extras.py
--rw-r--r--   0        0        0     5626 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/functions/functions.py
--rw-r--r--   0        0        0     5076 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/functions/schema_generator.py
--rw-r--r--   0        0        0        0 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/humans/__init__.py
--rw-r--r--   0        0        0       17 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/humans/examples/basic.txt
--rw-r--r--   0        0        0      305 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/humans/examples/cs_phd.txt
--rw-r--r--   0        0        0    12994 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/interface.py
--rw-r--r--   0        0        0    20696 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/llm_api_tools.py
--rw-r--r--   0        0        0      175 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/local_llm/README.md
--rw-r--r--   0        0        0        0 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/local_llm/__init__.py
--rw-r--r--   0        0        0    13309 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/local_llm/chat_completion_proxy.py
--rw-r--r--   0        0        0      806 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/local_llm/constants.py
--rw-r--r--   0        0        0     2788 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/local_llm/function_parser.py
--rw-r--r--   0        0        0        0 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/local_llm/grammars/__init__.py
--rw-r--r--   0        0        0    56322 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/local_llm/grammars/gbnf_grammar_generator.py
--rw-r--r--   0        0        0      667 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/local_llm/grammars/json.gbnf
--rw-r--r--   0        0        0     3255 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/local_llm/grammars/json_func_calls_with_inner_thoughts.gbnf
--rw-r--r--   0        0        0     6763 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/local_llm/json_parser.py
--rw-r--r--   0        0        0     2586 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/local_llm/koboldcpp/api.py
--rw-r--r--   0        0        0      557 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/local_llm/koboldcpp/settings.py
--rw-r--r--   0        0        0     2492 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/local_llm/llamacpp/api.py
--rw-r--r--   0        0        0      548 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/local_llm/llamacpp/settings.py
--rw-r--r--   0        0        0        0 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/local_llm/llm_chat_completion_wrappers/__init__.py
--rw-r--r--   0        0        0    19913 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/local_llm/llm_chat_completion_wrappers/airoboros.py
--rw-r--r--   0        0        0    21281 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/local_llm/llm_chat_completion_wrappers/chatml.py
--rw-r--r--   0        0        0    19975 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/local_llm/llm_chat_completion_wrappers/configurable_wrapper.py
--rw-r--r--   0        0        0    10300 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/local_llm/llm_chat_completion_wrappers/dolphin.py
--rw-r--r--   0        0        0     6144 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/local_llm/llm_chat_completion_wrappers/simple_summary_wrapper.py
--rw-r--r--   0        0        0      419 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/local_llm/llm_chat_completion_wrappers/wrapper_base.py
--rw-r--r--   0        0        0    14956 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/local_llm/llm_chat_completion_wrappers/zephyr.py
--rw-r--r--   0        0        0     4630 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/local_llm/lmstudio/api.py
--rw-r--r--   0        0        0      857 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/local_llm/lmstudio/settings.py
--rw-r--r--   0        0        0     3660 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/local_llm/ollama/api.py
--rw-r--r--   0        0        0      894 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/local_llm/ollama/settings.py
--rw-r--r--   0        0        0        0 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/local_llm/settings/__init__.py
--rw-r--r--   0        0        0     1222 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/local_llm/settings/deterministic_mirostat.py
--rw-r--r--   0        0        0     3058 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/local_llm/settings/settings.py
--rw-r--r--   0        0        0      719 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/local_llm/settings/simple.py
--rw-r--r--   0        0        0     4846 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/local_llm/utils.py
--rw-r--r--   0        0        0     2612 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/local_llm/vllm/api.py
--rw-r--r--   0        0        0     2658 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/local_llm/webui/api.py
--rw-r--r--   0        0        0     2354 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/local_llm/webui/legacy_api.py
--rw-r--r--   0        0        0      579 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/local_llm/webui/legacy_settings.py
--rw-r--r--   0        0        0      593 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/local_llm/webui/settings.py
--rw-r--r--   0        0        0     1211 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/log.py
--rw-r--r--   0        0        0    19532 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/main.py
--rw-r--r--   0        0        0    19653 2024-03-21 05:06:49.285282 pymemgpt-0.3.7/memgpt/memory.py
--rw-r--r--   0        0        0    27625 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/metadata.py
--rw-r--r--   0        0        0    31519 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/migrate.py
--rw-r--r--   0        0        0     2517 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/models/chat_completion_request.py
--rw-r--r--   0        0        0     1562 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/models/chat_completion_response.py
--rw-r--r--   0        0        0      356 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/models/embedding_response.py
--rw-r--r--   0        0        0     7977 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/models/openai.py
--rw-r--r--   0        0        0     7797 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/models/pydantic_models.py
--rw-r--r--   0        0        0        0 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/openai_backcompat/__init__.py
--rw-r--r--   0        0        0    13692 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/openai_backcompat/openai_object.py
--rw-r--r--   0        0        0     5898 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/persistence_manager.py
--rw-r--r--   0        0        0        0 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/personas/__init__.py
--rw-r--r--   0        0        0     1849 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/personas/examples/anna_pa.txt
--rw-r--r--   0        0        0     1196 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/personas/examples/google_search_persona.txt
--rw-r--r--   0        0        0      431 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/personas/examples/memgpt_doc.txt
--rw-r--r--   0        0        0      164 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/personas/examples/memgpt_starter.txt
--rw-r--r--   0        0        0     1236 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/personas/examples/sam.txt
--rw-r--r--   0        0        0     1171 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/personas/examples/sam_pov.txt
--rw-r--r--   0        0        0     1053 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/personas/examples/sam_simple_pov_gpt35.txt
--rw-r--r--   0        0        0     8192 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/personas/examples/sqldb/test.db
--rw-r--r--   0        0        0      248 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/presets/examples/memgpt_chat.yaml
--rw-r--r--   0        0        0      247 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/presets/examples/memgpt_docs.yaml
--rw-r--r--   0        0        0      374 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/presets/examples/memgpt_extras.yaml
--rw-r--r--   0        0        0     7575 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/presets/presets.py
--rw-r--r--   0        0        0     2789 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/presets/utils.py
--rw-r--r--   0        0        0        0 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/prompts/__init__.py
--rw-r--r--   0        0        0    12907 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/prompts/gpt_functions.py
--rw-r--r--   0        0        0     1139 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/prompts/gpt_summarize.py
--rw-r--r--   0        0        0     1045 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/prompts/gpt_system.py
--rw-r--r--   0        0        0     4758 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/prompts/system/memgpt_base.txt
--rw-r--r--   0        0        0     5494 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/prompts/system/memgpt_chat.txt
--rw-r--r--   0        0        0     1057 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/prompts/system/memgpt_chat_compressed.txt
--rw-r--r--   0        0        0     4819 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/prompts/system/memgpt_doc.txt
--rw-r--r--   0        0        0     5047 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/prompts/system/memgpt_gpt35_extralong.txt
--rw-r--r--   0        0        0     2967 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/prompts/system/memgpt_intuitive_knowledge.txt
--rw-r--r--   0        0        0     4663 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/prompts/system/memgpt_modified_chat.txt
--rw-r--r--   0        0        0        0 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/server/__init__.py
--rw-r--r--   0        0        0       92 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/server/constants.py
--rw-r--r--   0        0        0        0 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/server/rest_api/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/server/rest_api/admin/__init__.py
--rw-r--r--   0        0        0     6130 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/server/rest_api/admin/users.py
--rw-r--r--   0        0        0        0 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/server/rest_api/agents/__init__.py
--rw-r--r--   0        0        0     1757 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/server/rest_api/agents/command.py
--rw-r--r--   0        0        0     6138 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/server/rest_api/agents/config.py
--rw-r--r--   0        0        0     5114 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/server/rest_api/agents/index.py
--rw-r--r--   0        0        0     7640 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/server/rest_api/agents/memory.py
--rw-r--r--   0        0        0     7795 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/server/rest_api/agents/message.py
--rw-r--r--   0        0        0        0 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/server/rest_api/auth/__init__.py
--rw-r--r--   0        0        0     1303 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/server/rest_api/auth/index.py
--rw-r--r--   0        0        0      775 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/server/rest_api/auth_token.py
--rw-r--r--   0        0        0        0 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/server/rest_api/config/__init__.py
--rw-r--r--   0        0        0     1136 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/server/rest_api/config/index.py
--rw-r--r--   0        0        0        0 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/server/rest_api/humans/__init__.py
--rw-r--r--   0        0        0     1732 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/server/rest_api/humans/index.py
--rw-r--r--   0        0        0     4334 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/server/rest_api/interface.py
--rw-r--r--   0        0        0        0 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/server/rest_api/models/__init__.py
--rw-r--r--   0        0        0     1401 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/server/rest_api/models/index.py
--rw-r--r--   0        0        0    23918 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/server/rest_api/openai_assistants/assistants.py
--rw-r--r--   0        0        0        0 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/server/rest_api/personas/__init__.py
--rw-r--r--   0        0        0     1795 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/server/rest_api/personas/index.py
--rw-r--r--   0        0        0        0 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/server/rest_api/presets/__init__.py
--rw-r--r--   0        0        0     5014 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/server/rest_api/presets/index.py
--rw-r--r--   0        0        0     9103 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/server/rest_api/server.py
--rw-r--r--   0        0        0        0 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/server/rest_api/sources/__init__.py
--rw-r--r--   0        0        0     8257 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/server/rest_api/sources/index.py
--rw-r--r--   0        0        0      914 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/server/rest_api/static_files.py
--rw-r--r--   0        0        0        0 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/server/rest_api/tools/__init__.py
--rw-r--r--   0        0        0     2082 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/server/rest_api/tools/index.py
--rw-r--r--   0        0        0    62860 2024-03-21 05:06:49.289282 pymemgpt-0.3.7/memgpt/server/server.py
--rw-r--r--   0        0        0    32506 2024-03-21 05:06:49.293282 pymemgpt-0.3.7/memgpt/server/static_files/assets/index-57df4f6c.css
--rw-r--r--   0        0        0   515346 2024-03-21 05:06:49.293282 pymemgpt-0.3.7/memgpt/server/static_files/assets/index-f6a3d52a.js
--rw-r--r--   0        0        0    28783 2024-03-21 05:06:49.293282 pymemgpt-0.3.7/memgpt/server/static_files/favicon.ico
--rw-r--r--   0        0        0     1199 2024-03-21 05:06:49.293282 pymemgpt-0.3.7/memgpt/server/static_files/index.html
--rw-r--r--   0        0        0    85383 2024-03-21 05:06:49.293282 pymemgpt-0.3.7/memgpt/server/static_files/memgpt_logo_transparent.png
--rw-r--r--   0        0        0     1667 2024-03-21 05:06:49.293282 pymemgpt-0.3.7/memgpt/server/utils.py
--rw-r--r--   0        0        0        0 2024-03-21 05:06:49.293282 pymemgpt-0.3.7/memgpt/server/ws_api/__init__.py
--rw-r--r--   0        0        0     4264 2024-03-21 05:06:49.293282 pymemgpt-0.3.7/memgpt/server/ws_api/example_client.py
--rw-r--r--   0        0        0     4124 2024-03-21 05:06:49.293282 pymemgpt-0.3.7/memgpt/server/ws_api/interface.py
--rw-r--r--   0        0        0     2257 2024-03-21 05:06:49.293282 pymemgpt-0.3.7/memgpt/server/ws_api/protocol.py
--rw-r--r--   0        0        0     6122 2024-03-21 05:06:49.293282 pymemgpt-0.3.7/memgpt/server/ws_api/server.py
--rw-r--r--   0        0        0     7281 2024-03-21 05:06:49.293282 pymemgpt-0.3.7/memgpt/system.py
--rw-r--r--   0        0        0    30904 2024-03-21 05:06:49.293282 pymemgpt-0.3.7/memgpt/utils.py
--rw-r--r--   0        0        0     2275 2024-03-21 05:06:49.297282 pymemgpt-0.3.7/pyproject.toml
--rw-r--r--   0        0        0    10816 1970-01-01 00:00:00.000000 pymemgpt-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0    10760 2024-04-03 20:10:26.838568 pymemgpt-0.3.8/LICENSE
+-rw-r--r--   0        0        0     8441 2024-04-03 20:10:26.838568 pymemgpt-0.3.8/README.md
+-rw-r--r--   0        0        0      108 2024-04-03 20:10:26.862568 pymemgpt-0.3.8/memgpt/__init__.py
+-rw-r--r--   0        0        0       29 2024-04-03 20:10:26.862568 pymemgpt-0.3.8/memgpt/__main__.py
+-rw-r--r--   0        0        0    55407 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/agent.py
+-rw-r--r--   0        0        0    10728 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/agent_store/chroma.py
+-rw-r--r--   0        0        0    25552 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/agent_store/db.py
+-rw-r--r--   0        0        0     5288 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/agent_store/lancedb.py
+-rw-r--r--   0        0        0     6390 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/agent_store/storage.py
+-rw-r--r--   0        0        0      169 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/autogen/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/autogen/__init__.py
+-rw-r--r--   0        0        0     7088 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/autogen/examples/agent_autoreply.py
+-rw-r--r--   0        0        0     6813 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/autogen/examples/agent_docs.py
+-rw-r--r--   0        0        0     7914 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/autogen/examples/agent_groupchat.py
+-rw-r--r--   0        0        0     7375 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/autogen/examples/memgpt_coder_autogen.ipynb
+-rw-r--r--   0        0        0     9318 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/autogen/interface.py
+-rw-r--r--   0        0        0    20931 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/autogen/memgpt_agent.py
+-rw-r--r--   0        0        0     3644 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/benchmark/benchmark.py
+-rw-r--r--   0        0        0      536 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/benchmark/constants.py
+-rw-r--r--   0        0        0    34724 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/cli/cli.py
+-rw-r--r--   0        0        0    40394 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/cli/cli_config.py
+-rw-r--r--   0        0        0    10453 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/cli/cli_load.py
+-rw-r--r--   0        0        0        0 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/client/__init__.py
+-rw-r--r--   0        0        0     3239 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/client/admin.py
+-rw-r--r--   0        0        0    26592 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/client/client.py
+-rw-r--r--   0        0        0    18729 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/config.py
+-rw-r--r--   0        0        0      390 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/configs/memgpt_hosted.json
+-rw-r--r--   0        0        0      373 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/configs/openai.json
+-rw-r--r--   0        0        0     5364 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/constants.py
+-rw-r--r--   0        0        0     4904 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/credentials.py
+-rw-r--r--   0        0        0     9529 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/data_sources/connectors.py
+-rw-r--r--   0        0        0    23711 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/data_types.py
+-rw-r--r--   0        0        0     7601 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/embeddings.py
+-rw-r--r--   0        0        0      820 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/errors.py
+-rw-r--r--   0        0        0        0 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/functions/__init__.py
+-rw-r--r--   0        0        0     7343 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/functions/function_sets/base.py
+-rw-r--r--   0        0        0     4629 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/functions/function_sets/extras.py
+-rw-r--r--   0        0        0     5626 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/functions/functions.py
+-rw-r--r--   0        0        0     5433 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/functions/schema_generator.py
+-rw-r--r--   0        0        0        0 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/humans/__init__.py
+-rw-r--r--   0        0        0       17 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/humans/examples/basic.txt
+-rw-r--r--   0        0        0      305 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/humans/examples/cs_phd.txt
+-rw-r--r--   0        0        0    12994 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/interface.py
+-rw-r--r--   0        0        0    21252 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/llm_api_tools.py
+-rw-r--r--   0        0        0      175 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/local_llm/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/local_llm/__init__.py
+-rw-r--r--   0        0        0    13519 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/local_llm/chat_completion_proxy.py
+-rw-r--r--   0        0        0      912 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/local_llm/constants.py
+-rw-r--r--   0        0        0     2788 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/local_llm/function_parser.py
+-rw-r--r--   0        0        0        0 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/local_llm/grammars/__init__.py
+-rw-r--r--   0        0        0    56322 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/local_llm/grammars/gbnf_grammar_generator.py
+-rw-r--r--   0        0        0      667 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/local_llm/grammars/json.gbnf
+-rw-r--r--   0        0        0     3255 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/local_llm/grammars/json_func_calls_with_inner_thoughts.gbnf
+-rw-r--r--   0        0        0     3562 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/local_llm/groq/api.py
+-rw-r--r--   0        0        0     7434 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/local_llm/json_parser.py
+-rw-r--r--   0        0        0     2586 2024-04-03 20:10:26.866568 pymemgpt-0.3.8/memgpt/local_llm/koboldcpp/api.py
+-rw-r--r--   0        0        0      557 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/local_llm/koboldcpp/settings.py
+-rw-r--r--   0        0        0     2492 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/local_llm/llamacpp/api.py
+-rw-r--r--   0        0        0      548 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/local_llm/llamacpp/settings.py
+-rw-r--r--   0        0        0        0 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/local_llm/llm_chat_completion_wrappers/__init__.py
+-rw-r--r--   0        0        0    19913 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/local_llm/llm_chat_completion_wrappers/airoboros.py
+-rw-r--r--   0        0        0    21281 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/local_llm/llm_chat_completion_wrappers/chatml.py
+-rw-r--r--   0        0        0    19975 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/local_llm/llm_chat_completion_wrappers/configurable_wrapper.py
+-rw-r--r--   0        0        0    10300 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/local_llm/llm_chat_completion_wrappers/dolphin.py
+-rw-r--r--   0        0        0     6144 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/local_llm/llm_chat_completion_wrappers/simple_summary_wrapper.py
+-rw-r--r--   0        0        0      419 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/local_llm/llm_chat_completion_wrappers/wrapper_base.py
+-rw-r--r--   0        0        0    14956 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/local_llm/llm_chat_completion_wrappers/zephyr.py
+-rw-r--r--   0        0        0     4630 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/local_llm/lmstudio/api.py
+-rw-r--r--   0        0        0      857 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/local_llm/lmstudio/settings.py
+-rw-r--r--   0        0        0     3660 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/local_llm/ollama/api.py
+-rw-r--r--   0        0        0      894 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/local_llm/ollama/settings.py
+-rw-r--r--   0        0        0        0 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/local_llm/settings/__init__.py
+-rw-r--r--   0        0        0     1222 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/local_llm/settings/deterministic_mirostat.py
+-rw-r--r--   0        0        0     3058 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/local_llm/settings/settings.py
+-rw-r--r--   0        0        0      719 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/local_llm/settings/simple.py
+-rw-r--r--   0        0        0     4846 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/local_llm/utils.py
+-rw-r--r--   0        0        0     2612 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/local_llm/vllm/api.py
+-rw-r--r--   0        0        0     2658 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/local_llm/webui/api.py
+-rw-r--r--   0        0        0     2354 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/local_llm/webui/legacy_api.py
+-rw-r--r--   0        0        0      579 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/local_llm/webui/legacy_settings.py
+-rw-r--r--   0        0        0      593 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/local_llm/webui/settings.py
+-rw-r--r--   0        0        0     1211 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/log.py
+-rw-r--r--   0        0        0    19532 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/main.py
+-rw-r--r--   0        0        0    19653 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/memory.py
+-rw-r--r--   0        0        0    28296 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/metadata.py
+-rw-r--r--   0        0        0    31537 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/migrate.py
+-rw-r--r--   0        0        0     2517 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/models/chat_completion_request.py
+-rw-r--r--   0        0        0     1562 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/models/chat_completion_response.py
+-rw-r--r--   0        0        0      356 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/models/embedding_response.py
+-rw-r--r--   0        0        0     7977 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/models/openai.py
+-rw-r--r--   0        0        0     7902 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/models/pydantic_models.py
+-rw-r--r--   0        0        0        0 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/openai_backcompat/__init__.py
+-rw-r--r--   0        0        0    13692 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/openai_backcompat/openai_object.py
+-rw-r--r--   0        0        0     5882 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/persistence_manager.py
+-rw-r--r--   0        0        0        0 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/personas/__init__.py
+-rw-r--r--   0        0        0     1849 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/personas/examples/anna_pa.txt
+-rw-r--r--   0        0        0     1196 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/personas/examples/google_search_persona.txt
+-rw-r--r--   0        0        0      431 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/personas/examples/memgpt_doc.txt
+-rw-r--r--   0        0        0      164 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/personas/examples/memgpt_starter.txt
+-rw-r--r--   0        0        0     1236 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/personas/examples/sam.txt
+-rw-r--r--   0        0        0     1171 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/personas/examples/sam_pov.txt
+-rw-r--r--   0        0        0     1053 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/personas/examples/sam_simple_pov_gpt35.txt
+-rw-r--r--   0        0        0     8192 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/personas/examples/sqldb/test.db
+-rw-r--r--   0        0        0      248 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/presets/examples/memgpt_chat.yaml
+-rw-r--r--   0        0        0      247 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/presets/examples/memgpt_docs.yaml
+-rw-r--r--   0        0        0      374 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/presets/examples/memgpt_extras.yaml
+-rw-r--r--   0        0        0     7575 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/presets/presets.py
+-rw-r--r--   0        0        0     2789 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/presets/utils.py
+-rw-r--r--   0        0        0        0 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/prompts/__init__.py
+-rw-r--r--   0        0        0    12907 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/prompts/gpt_functions.py
+-rw-r--r--   0        0        0     1139 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/prompts/gpt_summarize.py
+-rw-r--r--   0        0        0     1045 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/prompts/gpt_system.py
+-rw-r--r--   0        0        0     4758 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/prompts/system/memgpt_base.txt
+-rw-r--r--   0        0        0     5479 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/prompts/system/memgpt_chat.txt
+-rw-r--r--   0        0        0     1057 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/prompts/system/memgpt_chat_compressed.txt
+-rw-r--r--   0        0        0     4819 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/prompts/system/memgpt_doc.txt
+-rw-r--r--   0        0        0     5047 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/prompts/system/memgpt_gpt35_extralong.txt
+-rw-r--r--   0        0        0     2967 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/prompts/system/memgpt_intuitive_knowledge.txt
+-rw-r--r--   0        0        0     4663 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/prompts/system/memgpt_modified_chat.txt
+-rw-r--r--   0        0        0        0 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/server/__init__.py
+-rw-r--r--   0        0        0       92 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/server/constants.py
+-rw-r--r--   0        0        0        0 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/server/rest_api/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/server/rest_api/admin/__init__.py
+-rw-r--r--   0        0        0     6130 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/server/rest_api/admin/users.py
+-rw-r--r--   0        0        0        0 2024-04-03 20:10:26.870569 pymemgpt-0.3.8/memgpt/server/rest_api/agents/__init__.py
+-rw-r--r--   0        0        0     1757 2024-04-03 20:10:26.874569 pymemgpt-0.3.8/memgpt/server/rest_api/agents/command.py
+-rw-r--r--   0        0        0     6138 2024-04-03 20:10:26.874569 pymemgpt-0.3.8/memgpt/server/rest_api/agents/config.py
+-rw-r--r--   0        0        0     5114 2024-04-03 20:10:26.874569 pymemgpt-0.3.8/memgpt/server/rest_api/agents/index.py
+-rw-r--r--   0        0        0     7640 2024-04-03 20:10:26.874569 pymemgpt-0.3.8/memgpt/server/rest_api/agents/memory.py
+-rw-r--r--   0        0        0     8583 2024-04-03 20:10:26.874569 pymemgpt-0.3.8/memgpt/server/rest_api/agents/message.py
+-rw-r--r--   0        0        0        0 2024-04-03 20:10:26.874569 pymemgpt-0.3.8/memgpt/server/rest_api/auth/__init__.py
+-rw-r--r--   0        0        0     1303 2024-04-03 20:10:26.874569 pymemgpt-0.3.8/memgpt/server/rest_api/auth/index.py
+-rw-r--r--   0        0        0      775 2024-04-03 20:10:26.874569 pymemgpt-0.3.8/memgpt/server/rest_api/auth_token.py
+-rw-r--r--   0        0        0        0 2024-04-03 20:10:26.874569 pymemgpt-0.3.8/memgpt/server/rest_api/config/__init__.py
+-rw-r--r--   0        0        0     1136 2024-04-03 20:10:26.874569 pymemgpt-0.3.8/memgpt/server/rest_api/config/index.py
+-rw-r--r--   0        0        0        0 2024-04-03 20:10:26.874569 pymemgpt-0.3.8/memgpt/server/rest_api/humans/__init__.py
+-rw-r--r--   0        0        0     1732 2024-04-03 20:10:26.874569 pymemgpt-0.3.8/memgpt/server/rest_api/humans/index.py
+-rw-r--r--   0        0        0     5482 2024-04-03 20:10:26.874569 pymemgpt-0.3.8/memgpt/server/rest_api/interface.py
+-rw-r--r--   0        0        0        0 2024-04-03 20:10:26.874569 pymemgpt-0.3.8/memgpt/server/rest_api/models/__init__.py
+-rw-r--r--   0        0        0     1401 2024-04-03 20:10:26.874569 pymemgpt-0.3.8/memgpt/server/rest_api/models/index.py
+-rw-r--r--   0        0        0    23956 2024-04-03 20:10:26.874569 pymemgpt-0.3.8/memgpt/server/rest_api/openai_assistants/assistants.py
+-rw-r--r--   0        0        0        0 2024-04-03 20:10:26.874569 pymemgpt-0.3.8/memgpt/server/rest_api/personas/__init__.py
+-rw-r--r--   0        0        0     1795 2024-04-03 20:10:26.874569 pymemgpt-0.3.8/memgpt/server/rest_api/personas/index.py
+-rw-r--r--   0        0        0        0 2024-04-03 20:10:26.874569 pymemgpt-0.3.8/memgpt/server/rest_api/presets/__init__.py
+-rw-r--r--   0        0        0     5014 2024-04-03 20:10:26.874569 pymemgpt-0.3.8/memgpt/server/rest_api/presets/index.py
+-rw-r--r--   0        0        0     9580 2024-04-03 20:10:26.874569 pymemgpt-0.3.8/memgpt/server/rest_api/server.py
+-rw-r--r--   0        0        0        0 2024-04-03 20:10:26.874569 pymemgpt-0.3.8/memgpt/server/rest_api/sources/__init__.py
+-rw-r--r--   0        0        0     8218 2024-04-03 20:10:26.874569 pymemgpt-0.3.8/memgpt/server/rest_api/sources/index.py
+-rw-r--r--   0        0        0      914 2024-04-03 20:10:26.874569 pymemgpt-0.3.8/memgpt/server/rest_api/static_files.py
+-rw-r--r--   0        0        0        0 2024-04-03 20:10:26.874569 pymemgpt-0.3.8/memgpt/server/rest_api/tools/__init__.py
+-rw-r--r--   0        0        0     2082 2024-04-03 20:10:26.874569 pymemgpt-0.3.8/memgpt/server/rest_api/tools/index.py
+-rw-r--r--   0        0        0    63523 2024-04-03 20:10:26.874569 pymemgpt-0.3.8/memgpt/server/server.py
+-rw-r--r--   0        0        0    32506 2024-04-03 20:10:26.874569 pymemgpt-0.3.8/memgpt/server/static_files/assets/index-57df4f6c.css
+-rw-r--r--   0        0        0   515346 2024-04-03 20:10:26.878569 pymemgpt-0.3.8/memgpt/server/static_files/assets/index-f6a3d52a.js
+-rw-r--r--   0        0        0    28783 2024-04-03 20:10:26.878569 pymemgpt-0.3.8/memgpt/server/static_files/favicon.ico
+-rw-r--r--   0        0        0     1199 2024-04-03 20:10:26.878569 pymemgpt-0.3.8/memgpt/server/static_files/index.html
+-rw-r--r--   0        0        0    85383 2024-04-03 20:10:26.878569 pymemgpt-0.3.8/memgpt/server/static_files/memgpt_logo_transparent.png
+-rw-r--r--   0        0        0     1667 2024-04-03 20:10:26.878569 pymemgpt-0.3.8/memgpt/server/utils.py
+-rw-r--r--   0        0        0        0 2024-04-03 20:10:26.878569 pymemgpt-0.3.8/memgpt/server/ws_api/__init__.py
+-rw-r--r--   0        0        0     4264 2024-04-03 20:10:26.878569 pymemgpt-0.3.8/memgpt/server/ws_api/example_client.py
+-rw-r--r--   0        0        0     4124 2024-04-03 20:10:26.878569 pymemgpt-0.3.8/memgpt/server/ws_api/interface.py
+-rw-r--r--   0        0        0     2257 2024-04-03 20:10:26.878569 pymemgpt-0.3.8/memgpt/server/ws_api/protocol.py
+-rw-r--r--   0        0        0     6122 2024-04-03 20:10:26.878569 pymemgpt-0.3.8/memgpt/server/ws_api/server.py
+-rw-r--r--   0        0        0     7281 2024-04-03 20:10:26.878569 pymemgpt-0.3.8/memgpt/system.py
+-rw-r--r--   0        0        0    31128 2024-04-03 20:10:26.878569 pymemgpt-0.3.8/memgpt/utils.py
+-rw-r--r--   0        0        0     2275 2024-04-03 20:10:26.886569 pymemgpt-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0    11006 1970-01-01 00:00:00.000000 pymemgpt-0.3.8/PKG-INFO
```

### Comparing `pymemgpt-0.3.7/LICENSE` & `pymemgpt-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/README.md` & `pymemgpt-0.3.8/README.md`

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

### Comparing `pymemgpt-0.3.7/memgpt/agent.py` & `pymemgpt-0.3.8/memgpt/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,25 +13,27 @@
 from memgpt.models import chat_completion_response
 from memgpt.interface import AgentInterface
 from memgpt.persistence_manager import LocalStateManager
 from memgpt.system import get_login_event, package_function_response, package_summarize_message, get_initial_boot_messages
 from memgpt.memory import CoreMemory as InContextMemory, summarize_messages, ArchivalMemory, RecallMemory
 from memgpt.llm_api_tools import create, is_context_overflow_error
 from memgpt.utils import (
+    get_utc_time,
     create_random_username,
     get_tool_call_id,
     get_local_time,
     parse_json,
     united_diff,
     printd,
     count_tokens,
     get_schema_diff,
     validate_function_response,
     verify_first_message_correctness,
     create_uuid_from_string,
+    is_utc_datetime,
 )
 from memgpt.constants import (
     FIRST_MESSAGE_ATTEMPTS,
     JSON_LOADS_STRICT,
     MESSAGE_SUMMARY_WARNING_FRAC,
     MESSAGE_SUMMARY_TRUNC_TOKEN_FRAC,
     MESSAGE_SUMMARY_TRUNC_KEEP_N_LAST,
@@ -135,15 +137,15 @@
     model: str,
     system: str,
     memory: InContextMemory,
     archival_memory: Optional[ArchivalMemory] = None,
     recall_memory: Optional[RecallMemory] = None,
     memory_edit_timestamp: Optional[str] = None,
     include_initial_boot_message: bool = True,
-):
+) -> List[dict]:
     if memory_edit_timestamp is None:
         memory_edit_timestamp = get_local_time()
 
     full_system_message = construct_system_with_memory(
         system, memory, memory_edit_timestamp, archival_memory=archival_memory, recall_memory=recall_memory
     )
     first_user_message = get_login_event()  # event letting MemGPT know the user just logged in
@@ -286,14 +288,21 @@
             # Convert to IDs, and pull from the database
             raw_messages = [
                 self.persistence_manager.recall_memory.storage.get(id=uuid.UUID(msg_id)) for msg_id in self.agent_state.state["messages"]
             ]
             assert all([isinstance(msg, Message) for msg in raw_messages]), (raw_messages, self.agent_state.state["messages"])
             self._messages.extend([cast(Message, msg) for msg in raw_messages if msg is not None])
 
+            for m in self._messages:
+                # assert is_utc_datetime(m.created_at), f"created_at on message for agent {self.agent_state.name} isn't UTC:\n{vars(m)}"
+                # TODO eventually do casting via an edit_message function
+                if not is_utc_datetime(m.created_at):
+                    printd(f"Warning - created_at on message for agent {self.agent_state.name} isn't UTC (text='{m.text}')")
+                    m.created_at = m.created_at.replace(tzinfo=datetime.timezone.utc)
+
         else:
             # print(f"Agent.__init__ :: creating, state={agent_state.state['messages']}")
             init_messages = initialize_message_sequence(
                 self.model,
                 self.system,
                 self.memory,
             )
@@ -304,14 +313,21 @@
                         agent_id=self.agent_state.id, user_id=self.agent_state.user_id, model=self.model, openai_message_dict=msg
                     )
                 )
             assert all([isinstance(msg, Message) for msg in init_messages_objs]), (init_messages_objs, init_messages)
             self.messages_total = 0
             self._append_to_messages(added_messages=[cast(Message, msg) for msg in init_messages_objs if msg is not None])
 
+            for m in self._messages:
+                assert is_utc_datetime(m.created_at), f"created_at on message for agent {self.agent_state.name} isn't UTC:\n{vars(m)}"
+                # TODO eventually do casting via an edit_message function
+                if not is_utc_datetime(m.created_at):
+                    printd(f"Warning - created_at on message for agent {self.agent_state.name} isn't UTC (text='{m.text}')")
+                    m.created_at = m.created_at.replace(tzinfo=datetime.timezone.utc)
+
         # Keep track of the total number of messages throughout all time
         self.messages_total = messages_total if messages_total is not None else (len(self._messages) - 1)  # (-system)
         # self.messages_total_init = self.messages_total
         self.messages_total_init = len(self._messages) - 1
         printd(f"Agent initialized, self.messages_total={self.messages_total}")
 
         # Create the agent in the DB
@@ -440,14 +456,16 @@
 
             # only necessary to add the tool_cal_id to a function call (antipattern)
             # response_message_dict = response_message.model_dump()
             # response_message_dict["tool_call_id"] = tool_call_id
 
             # role: assistant (requesting tool call, set tool call ID)
             messages.append(
+                # NOTE: we're recreating the message here
+                # TODO should probably just overwrite the fields?
                 Message.dict_to_message(
                     agent_id=self.agent_state.id,
                     user_id=self.agent_state.user_id,
                     model=self.model,
                     openai_message_dict=response_message.model_dump(),
                 )
             )  # extend conversation with assistant's reply
@@ -649,15 +667,15 @@
                     if name is not None:
                         # Update Message object
                         user_message.text = cleaned_user_message_text
                         user_message.name = name
 
                     # Recreate timestamp
                     if recreate_message_timestamp:
-                        user_message.created_at = datetime.datetime.now()
+                        user_message.created_at = get_utc_time()
 
                 elif isinstance(user_message, str):
                     # Validate JSON via save/load
                     user_message = validate_json(user_message, False)
                     cleaned_user_message_text, name = strip_name_field_from_user_message(user_message)
 
                     # If user_message['name'] is not None, it will be handled properly by dict_to_message
@@ -705,15 +723,15 @@
                     message_sequence=input_message_sequence,
                 )
 
             # Step 2: check if LLM wanted to call a function
             # (if yes) Step 3: call the function
             # (if yes) Step 4: send the info on the function call and function response to LLM
             response_message = response.choices[0].message
-            response_message.copy()
+            response_message.model_copy()  # TODO why are we copying here?
             all_response_messages, heartbeat_request, function_failed = self._handle_ai_response(response_message)
 
             # Add the extra metadata to the assistant response
             # (e.g. enough metadata to enable recreating the API call)
             # assert "api_response" not in all_response_messages[0]
             # all_response_messages[0]["api_response"] = response_message_copy
             # assert "api_args" not in all_response_messages[0]
@@ -891,15 +909,15 @@
         """Check if there's a requested pause on timed heartbeats"""
 
         # Check if the pause has been initiated
         if self.pause_heartbeats_start is None:
             return False
 
         # Check if it's been more than pause_heartbeats_minutes since pause_heartbeats_start
-        elapsed_time = datetime.datetime.now() - self.pause_heartbeats_start
+        elapsed_time = get_utc_time() - self.pause_heartbeats_start
         return elapsed_time.total_seconds() < self.pause_heartbeats_minutes * 60
 
     def rebuild_memory(self):
         """Rebuilds the system message with the latest memory object"""
         curr_system_message = self.messages[0]  # this is the system + memory bank, not just the system prompt
         new_system_message = initialize_message_sequence(
             self.model,
```

### Comparing `pymemgpt-0.3.7/memgpt/agent_store/chroma.py` & `pymemgpt-0.3.8/memgpt/agent_store/chroma.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/agent_store/db.py` & `pymemgpt-0.3.8/memgpt/agent_store/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,15 +147,15 @@
                 embedding = mapped_column(Vector(MAX_EMBEDDING_DIM))
             embedding_dim = Column(BIGINT)
             embedding_model = Column(String)
 
             metadata_ = Column(MutableJson)
 
             # Add a datetime column, with default value as the current time
-            created_at = Column(DateTime(timezone=True), server_default=func.now())
+            created_at = Column(DateTime(timezone=True))
 
             def __repr__(self):
                 return f"<Passage(passage_id='{self.id}', text='{self.text}', embedding='{self.embedding})>"
 
             def to_record(self):
                 return Passage(
                     text=self.text,
@@ -213,15 +213,15 @@
                 from pgvector.sqlalchemy import Vector
 
                 embedding = mapped_column(Vector(MAX_EMBEDDING_DIM))
             embedding_dim = Column(BIGINT)
             embedding_model = Column(String)
 
             # Add a datetime column, with default value as the current time
-            created_at = Column(DateTime(timezone=True), server_default=func.now())
+            created_at = Column(DateTime(timezone=True))
 
             def __repr__(self):
                 return f"<Message(message_id='{self.id}', text='{self.text}', embedding='{self.embedding})>"
 
             def to_record(self):
                 return Message(
                     user_id=self.user_id,
@@ -420,38 +420,55 @@
     # TODO: this should probably eventually be moved into a parent DB class
 
     def __init__(self, table_type: str, config: MemGPTConfig, user_id, agent_id=None):
         from pgvector.sqlalchemy import Vector
 
         super().__init__(table_type=table_type, config=config, user_id=user_id, agent_id=agent_id)
 
-        # get storage URI
-        if table_type == TableType.ARCHIVAL_MEMORY or table_type == TableType.PASSAGES:
-            self.uri = self.config.archival_storage_uri
-            if self.config.archival_storage_uri is None:
-                raise ValueError(f"Must specifiy archival_storage_uri in config {self.config.config_path}")
-        elif table_type == TableType.RECALL_MEMORY:
-            self.uri = self.config.recall_storage_uri
-            if self.config.recall_storage_uri is None:
-                raise ValueError(f"Must specifiy recall_storage_uri in config {self.config.config_path}")
-        else:
-            raise ValueError(f"Table type {table_type} not implemented")
         # create table
         self.db_model = get_db_model(config, self.table_name, table_type, user_id, agent_id)
+
+        # construct URI from enviornment variables
+        if os.getenv("MEMGPT_PGURI"):
+            self.uri = os.getenv("MEMGPT_PGURI")
+        elif os.getenv("MEMGPT_PG_DB"):
+            db = os.getenv("MEMGPT_PG_DB", "memgpt")
+            user = os.getenv("MEMGPT_PG_USER", "memgpt")
+            password = os.getenv("MEMGPT_PG_PASSWORD", "memgpt")
+            port = os.getenv("MEMGPT_PG_PORT", "5432")
+            url = os.getenv("MEMGPT_PG_URL", "localhost")
+            self.uri = f"postgresql+pg8000://{user}:{password}@{url}:{port}/{db}"
+        else:
+            # use config URI
+            # TODO: remove this eventually (config should NOT contain URI)
+            if table_type == TableType.ARCHIVAL_MEMORY or table_type == TableType.PASSAGES:
+                self.uri = self.config.archival_storage_uri
+                if self.config.archival_storage_uri is None:
+                    raise ValueError(f"Must specifiy archival_storage_uri in config {self.config.config_path}")
+            elif table_type == TableType.RECALL_MEMORY:
+                self.uri = self.config.recall_storage_uri
+                if self.config.recall_storage_uri is None:
+                    raise ValueError(f"Must specifiy recall_storage_uri in config {self.config.config_path}")
+            else:
+                raise ValueError(f"Table type {table_type} not implemented")
+
+        # create engine
         self.engine = create_engine(self.uri)
+
         for c in self.db_model.__table__.columns:
             if c.name == "embedding":
                 assert isinstance(c.type, Vector), f"Embedding column must be of type Vector, got {c.type}"
 
-        Base.metadata.create_all(self.engine, tables=[self.db_model.__table__])  # Create the table if it doesn't exist
-
         self.session_maker = sessionmaker(bind=self.engine)
         with self.session_maker() as session:
             session.execute(text("CREATE EXTENSION IF NOT EXISTS vector"))  # Enables the vector extension
 
+        # create table
+        Base.metadata.create_all(self.engine, tables=[self.db_model.__table__])  # Create the table if it doesn't exist
+
     def query(self, query: str, query_vec: List[float], top_k: int = 10, filters: Optional[Dict] = {}) -> List[RecordType]:
         filters = self.get_filters(filters)
         with self.session_maker() as session:
             results = session.scalars(
                 select(self.db_model).filter(*filters).order_by(self.db_model.embedding.l2_distance(query_vec)).limit(top_k)
             ).all()
```

### Comparing `pymemgpt-0.3.7/memgpt/agent_store/lancedb.py` & `pymemgpt-0.3.8/memgpt/agent_store/lancedb.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/agent_store/storage.py` & `pymemgpt-0.3.8/memgpt/agent_store/storage.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/autogen/examples/agent_autoreply.py` & `pymemgpt-0.3.8/memgpt/autogen/examples/agent_autoreply.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/autogen/examples/agent_docs.py` & `pymemgpt-0.3.8/memgpt/autogen/examples/agent_docs.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/autogen/examples/agent_groupchat.py` & `pymemgpt-0.3.8/memgpt/autogen/examples/agent_groupchat.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/autogen/examples/memgpt_coder_autogen.ipynb` & `pymemgpt-0.3.8/memgpt/autogen/examples/memgpt_coder_autogen.ipynb`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/autogen/interface.py` & `pymemgpt-0.3.8/memgpt/autogen/interface.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/autogen/memgpt_agent.py` & `pymemgpt-0.3.8/memgpt/autogen/memgpt_agent.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/benchmark/benchmark.py` & `pymemgpt-0.3.8/memgpt/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/benchmark/constants.py` & `pymemgpt-0.3.8/memgpt/benchmark/constants.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/cli/cli.py` & `pymemgpt-0.3.8/memgpt/cli/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from memgpt.utils import printd, open_folder_in_explorer, suppress_stdout
 from memgpt.config import MemGPTConfig
 from memgpt.credentials import MemGPTCredentials
 from memgpt.constants import MEMGPT_DIR, CLI_WARNING_PREFIX, JSON_ENSURE_ASCII
 from memgpt.agent import Agent, save_agent
 from memgpt.embeddings import embedding_model
 from memgpt.server.constants import WS_DEFAULT_PORT, REST_DEFAULT_PORT
-from memgpt.data_types import AgentState, LLMConfig, EmbeddingConfig, User, Passage, Preset
+from memgpt.data_types import AgentState, LLMConfig, EmbeddingConfig, User, Passage
 from memgpt.metadata import MetadataStore
 from memgpt.migrate import migrate_all_agents, migrate_all_sources
 
 
 def migrate(
     debug: Annotated[bool, typer.Option(help="Print extra tracebacks for failed migrations")] = False,
 ):
@@ -71,35 +71,54 @@
                 modified = True
                 # old_config[k] = new_config[k]
                 setattr(old_config, k, new_config[k])  # Set the new value using dot notation
             else:
                 printd(f"Skipping new config {k}: {v} == {new_config[k]}")
 
     # update embedding config
-    for k, v in vars(old_config.default_embedding_config).items():
-        if k in new_config:
-            if v != new_config[k]:
-                printd(f"Replacing config {k}: {v} -> {new_config[k]}")
-                modified = True
-                # old_config[k] = new_config[k]
-                setattr(old_config.default_embedding_config, k, new_config[k])
-            else:
-                printd(f"Skipping new config {k}: {v} == {new_config[k]}")
+    if old_config.default_embedding_config:
+        for k, v in vars(old_config.default_embedding_config).items():
+            if k in new_config:
+                if v != new_config[k]:
+                    printd(f"Replacing config {k}: {v} -> {new_config[k]}")
+                    modified = True
+                    # old_config[k] = new_config[k]
+                    setattr(old_config.default_embedding_config, k, new_config[k])
+                else:
+                    printd(f"Skipping new config {k}: {v} == {new_config[k]}")
+    else:
+        modified = True
+        fields = ["embedding_model", "embedding_dim", "embedding_chunk_size", "embedding_endpoint", "embedding_endpoint_type"]
+        args = {}
+        for field in fields:
+            if field in new_config:
+                args[field] = new_config[field]
+                printd(f"Setting new config {field}: {new_config[field]}")
+        old_config.default_embedding_config = EmbeddingConfig(**args)
 
     # update llm config
-    for k, v in vars(old_config.default_llm_config).items():
-        if k in new_config:
-            if v != new_config[k]:
-                printd(f"Replacing config {k}: {v} -> {new_config[k]}")
-                modified = True
-                # old_config[k] = new_config[k]
-                setattr(old_config.default_llm_config, k, new_config[k])
-            else:
-                printd(f"Skipping new config {k}: {v} == {new_config[k]}")
-
+    if old_config.default_llm_config:
+        for k, v in vars(old_config.default_llm_config).items():
+            if k in new_config:
+                if v != new_config[k]:
+                    printd(f"Replacing config {k}: {v} -> {new_config[k]}")
+                    modified = True
+                    # old_config[k] = new_config[k]
+                    setattr(old_config.default_llm_config, k, new_config[k])
+                else:
+                    printd(f"Skipping new config {k}: {v} == {new_config[k]}")
+    else:
+        modified = True
+        fields = ["model", "model_endpoint", "model_endpoint_type", "model_wrapper", "context_window"]
+        args = {}
+        for field in fields:
+            if field in new_config:
+                args[field] = new_config[field]
+                printd(f"Setting new config {field}: {new_config[field]}")
+        old_config.default_llm_config = LLMConfig(**args)
     return (old_config, modified)
 
 
 def quickstart(
     backend: Annotated[QuickstartChoice, typer.Option(help="Quickstart setup backend")] = "memgpt",
     latest: Annotated[bool, typer.Option(help="Use --latest to pull the latest config from online")] = False,
     debug: Annotated[bool, typer.Option(help="Use --debug to enable debugging output")] = False,
@@ -149,18 +168,21 @@
                     new_config, config_was_modified = set_config_with_dict(backup_config)
                 except FileNotFoundError:
                     typer.secho(f"Backup config file not found at {backup_config_path}", fg=typer.colors.RED)
                     return
         else:
             # Load the file from the relative path
             script_dir = os.path.dirname(__file__)  # Get the directory where the script is located
+            print("SCRIPT", script_dir)
             backup_config_path = os.path.join(script_dir, "..", "configs", "memgpt_hosted.json")
+            print("FILE PATH", backup_config_path)
             try:
                 with open(backup_config_path, "r", encoding="utf-8") as file:
                     backup_config = json.load(file)
+                    print(backup_config)
                 printd("Loaded config file successfully.")
                 new_config, config_was_modified = set_config_with_dict(backup_config)
             except FileNotFoundError:
                 typer.secho(f"Config file not found at {backup_config_path}", fg=typer.colors.RED)
                 return
 
     elif backend == QuickstartChoice.openai:
@@ -639,47 +661,34 @@
                 fg=typer.colors.YELLOW,
             )
             llm_config.model_endpoint_type = model_endpoint_type
 
         # create agent
         try:
             preset_obj = ms.get_preset(name=preset if preset else config.preset, user_id=user.id)
-            preset_override = False
+            human_obj = ms.get_human(human, user.id)
+            persona_obj = ms.get_persona(persona, user.id)
             if preset_obj is None:
                 # create preset records in metadata store
                 from memgpt.presets.presets import add_default_presets
 
                 add_default_presets(user.id, ms)
                 # try again
                 preset_obj = ms.get_preset(name=preset if preset else config.preset, user_id=user.id)
                 if preset_obj is None:
                     typer.secho("Couldn't find presets in database, please run `memgpt configure`", fg=typer.colors.RED)
                     sys.exit(1)
-
-            human_obj = ms.get_human(human, user.id)
             if human_obj is None:
                 typer.secho("Couldn't find human {human} in database, please run `memgpt add human`", fg=typer.colors.RED)
-            persona_obj = ms.get_persona(persona, user.id)
             if persona_obj is None:
                 typer.secho("Couldn't find persona {persona} in database, please run `memgpt add persona`", fg=typer.colors.RED)
 
             # Overwrite fields in the preset if they were specified
-            if human_obj.text != preset_obj.human:
-                preset_override = True
-                preset_obj.human = human_obj.text
-            if persona_obj.text != preset_obj.human:
-                preset_override = True
-                preset_obj.persona = persona_obj.text
-
-            # If the user overrode any parts of the preset, we need to create a new preset to refer back to
-            if preset_override:
-                # Change the name and uuid
-                preset_obj = Preset.clone(preset_obj=preset_obj)
-                # Then write out to the database for storage
-                ms.create_preset(preset=preset_obj)
+            preset_obj.human = ms.get_human(human, user.id).text
+            preset_obj.persona = ms.get_persona(persona, user.id).text
 
             typer.secho(f"->  🤖 Using persona profile: '{preset_obj.persona_name}'", fg=typer.colors.WHITE)
             typer.secho(f"->  🧑 Using human profile: '{preset_obj.human_name}'", fg=typer.colors.WHITE)
 
             memgpt_agent = Agent(
                 interface=interface(),
                 name=agent_name,
```

### Comparing `pymemgpt-0.3.7/memgpt/cli/cli_config.py` & `pymemgpt-0.3.8/memgpt/cli/cli_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,17 @@
                 credentials.azure_embedding_deployment = azure_creds["azure_embedding_deployment"]
             credentials.save()
 
         model_endpoint_type = "azure"
         model_endpoint = azure_creds["azure_endpoint"]
 
     else:  # local models
-        backend_options = ["webui", "webui-legacy", "llamacpp", "koboldcpp", "ollama", "lmstudio", "lmstudio-legacy", "vllm", "openai"]
+        # backend_options_old = ["webui", "webui-legacy", "llamacpp", "koboldcpp", "ollama", "lmstudio", "lmstudio-legacy", "vllm", "openai"]
+        backend_options = builtins.list(DEFAULT_ENDPOINTS.keys())
+        # assert backend_options_old == backend_options, (backend_options_old, backend_options)
         default_model_endpoint_type = None
         if config.default_llm_config.model_endpoint_type in backend_options:
             # set from previous config
             default_model_endpoint_type = config.default_llm_config.model_endpoint_type
         model_endpoint_type = questionary.select(
             "Select LLM backend (select 'openai' if you have an OpenAI compatible proxy):",
             backend_options,
@@ -219,16 +221,20 @@
             if filter_list:
                 model_options = [obj["id"] for obj in fetched_model_options_response["data"] if obj["id"].startswith(filter_prefix)]
             else:
                 model_options = [obj["id"] for obj in fetched_model_options_response["data"]]
 
         else:
             # Attempt to do OpenAI endpoint style model fetching
-            # TODO support local auth
-            fetched_model_options_response = openai_get_model_list(url=model_endpoint, api_key=None)
+            # TODO support local auth with api-key header
+            if credentials.openllm_auth_type == "bearer_token":
+                api_key = credentials.openllm_key
+            else:
+                api_key = None
+            fetched_model_options_response = openai_get_model_list(url=model_endpoint, api_key=api_key, fix_url=True)
             model_options = [obj["id"] for obj in fetched_model_options_response["data"]]
             # NOTE no filtering of local model options
 
         # list
         return model_options
 
     except:
@@ -285,14 +291,52 @@
                 model = questionary.text(
                     "Enter custom model name:",
                 ).ask()
                 if model is None:
                     raise KeyboardInterrupt
 
     else:  # local models
+
+        # ask about local auth
+        if model_endpoint_type in ["groq"]:  # TODO all llm engines under 'local' that will require api keys
+            use_local_auth = True
+            local_auth_type = "bearer_token"
+            local_auth_key = questionary.password(
+                "Enter your Groq API key:",
+            ).ask()
+            if local_auth_key is None:
+                raise KeyboardInterrupt
+            credentials.openllm_auth_type = local_auth_type
+            credentials.openllm_key = local_auth_key
+            credentials.save()
+        else:
+            use_local_auth = questionary.confirm(
+                "Is your LLM endpoint authenticated? (default no)",
+                default=False,
+            ).ask()
+            if use_local_auth is None:
+                raise KeyboardInterrupt
+            if use_local_auth:
+                local_auth_type = questionary.select(
+                    "What HTTP authentication method does your endpoint require?",
+                    choices=SUPPORTED_AUTH_TYPES,
+                    default=SUPPORTED_AUTH_TYPES[0],
+                ).ask()
+                if local_auth_type is None:
+                    raise KeyboardInterrupt
+                local_auth_key = questionary.password(
+                    "Enter your authentication key:",
+                ).ask()
+                if local_auth_key is None:
+                    raise KeyboardInterrupt
+                # credentials = MemGPTCredentials.load()
+                credentials.openllm_auth_type = local_auth_type
+                credentials.openllm_key = local_auth_key
+                credentials.save()
+
         # ollama also needs model type
         if model_endpoint_type == "ollama":
             default_model = (
                 config.default_llm_config.model
                 if config.default_llm_config.model and config.default_llm_config.model_endpoint_type == "ollama"
                 else DEFAULT_OLLAMA_MODEL
             )
@@ -307,15 +351,15 @@
         default_model = (
             config.default_llm_config.model
             if config.default_llm_config.model and config.default_llm_config.model_endpoint_type == "vllm"
             else ""
         )
 
         # vllm needs huggingface model tag
-        if model_endpoint_type == "vllm":
+        if model_endpoint_type in ["vllm", "groq"]:
             try:
                 # Don't filter model list for vLLM since model list is likely much smaller than OpenAI/Azure endpoint
                 # + probably has custom model names
                 # TODO support local auth
                 model_options = get_model_options(
                     credentials=credentials, model_endpoint_type=model_endpoint_type, model_endpoint=model_endpoint
                 )
@@ -362,39 +406,14 @@
             f"Select default model wrapper (recommended: {DEFAULT_WRAPPER_NAME}):",
             choices=available_model_wrappers,
             default=DEFAULT_WRAPPER_NAME,
         ).ask()
         if model_wrapper is None:
             raise KeyboardInterrupt
 
-        # ask about local auth
-        use_local_auth = questionary.confirm(
-            "Is your LLM endpoint authenticated? (default no)",
-            default=False,
-        ).ask()
-        if use_local_auth is None:
-            raise KeyboardInterrupt
-        if use_local_auth:
-            local_auth_type = questionary.select(
-                "What HTTP authentication method does your endpoint require?",
-                choices=SUPPORTED_AUTH_TYPES,
-                default=SUPPORTED_AUTH_TYPES[0],
-            ).ask()
-            if local_auth_type is None:
-                raise KeyboardInterrupt
-            local_auth_key = questionary.password(
-                "Enter your authentication key:",
-            ).ask()
-            if local_auth_key is None:
-                raise KeyboardInterrupt
-            # credentials = MemGPTCredentials.load()
-            credentials.openllm_auth_type = local_auth_type
-            credentials.openllm_key = local_auth_key
-            credentials.save()
-
     # set: context_window
     if str(model) not in LLM_MAX_TOKENS:
         # Ask the user to specify the context length
         context_length_options = [
             str(2**12),  # 4096
             str(2**13),  # 8192
             str(2**14),  # 16384
@@ -771,28 +790,35 @@
         for persona in ms.list_personas(user_id=user_id):
             table.add_row([persona.name, persona.text.replace("\n", "")[:100]])
         print(table)
     elif arg == ListChoice.sources:
         """List all data sources"""
 
         # create table
-        table.field_names = ["Name", "Embedding Model", "Embedding Dim", "Created At", "Agents"]
+        table.field_names = ["Name", "Description", "Embedding Model", "Embedding Dim", "Created At", "Agents"]
         # TODO: eventually look accross all storage connections
         # TODO: add data source stats
         # TODO: connect to agents
 
         # get all sources
         for source in ms.list_sources(user_id=user_id):
             # get attached agents
             agent_ids = ms.list_attached_agents(source_id=source.id)
             agent_states = [ms.get_agent(agent_id=agent_id) for agent_id in agent_ids]
             agent_names = [agent_state.name for agent_state in agent_states if agent_state is not None]
 
             table.add_row(
-                [source.name, source.embedding_model, source.embedding_dim, utils.format_datetime(source.created_at), ",".join(agent_names)]
+                [
+                    source.name,
+                    source.description,
+                    source.embedding_model,
+                    source.embedding_dim,
+                    utils.format_datetime(source.created_at),
+                    ",".join(agent_names),
+                ]
             )
 
         print(table)
     elif arg == ListChoice.presets:
         """List all available presets"""
         table.field_names = ["Name", "Description", "Sources", "Functions"]
         for preset in ms.list_presets(user_id=user_id):
```

### Comparing `pymemgpt-0.3.7/memgpt/cli/cli_load.py` & `pymemgpt-0.3.8/memgpt/cli/cli_load.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,27 +84,29 @@
 def load_directory(
     name: Annotated[str, typer.Option(help="Name of dataset to load.")],
     input_dir: Annotated[Optional[str], typer.Option(help="Path to directory containing dataset.")] = None,
     input_files: Annotated[List[str], typer.Option(help="List of paths to files containing dataset.")] = [],
     recursive: Annotated[bool, typer.Option(help="Recursively search for files in directory.")] = False,
     extensions: Annotated[str, typer.Option(help="Comma separated list of file extensions to load")] = default_extensions,
     user_id: Annotated[Optional[uuid.UUID], typer.Option(help="User ID to associate with dataset.")] = None,  # TODO: remove
+    description: Annotated[Optional[str], typer.Option(help="Description of the source.")] = None,
 ):
     try:
         connector = DirectoryConnector(input_files=input_files, input_directory=input_dir, recursive=recursive, extensions=extensions)
         config = MemGPTConfig.load()
         if not user_id:
             user_id = uuid.UUID(config.anon_clientid)
 
         ms = MetadataStore(config)
         source = Source(
             name=name,
             user_id=user_id,
             embedding_model=config.default_embedding_config.embedding_model,
             embedding_dim=config.default_embedding_config.embedding_dim,
+            description=description,
         )
         ms.create_source(source)
         passage_storage = StorageConnector.get_storage_connector(TableType.PASSAGES, config, user_id)
         # TODO: also get document store
 
         # ingest data into passage/document store
         try:
```

### Comparing `pymemgpt-0.3.7/memgpt/client/admin.py` & `pymemgpt-0.3.8/memgpt/client/admin.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/client/client.py` & `pymemgpt-0.3.8/memgpt/client/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime
 import requests
 from requests.exceptions import RequestException
 import uuid
 from typing import Dict, List, Union, Optional, Tuple
 
 from memgpt.data_types import AgentState, User, Preset, LLMConfig, EmbeddingConfig, Source
-from memgpt.models.pydantic_models import HumanModel, PersonaModel, PresetModel
+from memgpt.models.pydantic_models import HumanModel, PersonaModel, PresetModel, SourceModel
 from memgpt.cli.cli import QuickstartChoice
 from memgpt.cli.cli import set_config_with_dict, quickstart as quickstart_func, str_to_quickstart_choice
 from memgpt.config import MemGPTConfig
 from memgpt.server.rest_api.interface import QueuingInterface
 from memgpt.server.server import SyncServer
 from memgpt.metadata import MetadataStore
 from memgpt.data_sources.connectors import DataConnector
@@ -27,14 +27,15 @@
 from memgpt.server.rest_api.agents.message import UserMessageResponse, GetAgentMessagesResponse
 from memgpt.server.rest_api.config.index import ConfigResponse
 from memgpt.server.rest_api.humans.index import ListHumansResponse
 from memgpt.server.rest_api.personas.index import ListPersonasResponse
 from memgpt.server.rest_api.tools.index import ListToolsResponse, CreateToolResponse
 from memgpt.server.rest_api.models.index import ListModelsResponse
 from memgpt.server.rest_api.presets.index import CreatePresetResponse, CreatePresetsRequest, ListPresetsResponse
+from memgpt.server.rest_api.sources.index import ListSourcesResponse, UploadFileToSourceResponse
 
 
 def create_client(base_url: Optional[str] = None, token: Optional[str] = None):
     if base_url is None:
         return LocalClient()
     else:
         return RESTClient(base_url, token)
@@ -281,15 +282,15 @@
             preset=response.agent_state.preset,
             persona=response.agent_state.persona,
             human=response.agent_state.human,
             llm_config=llm_config,
             embedding_config=embedding_config,
             state=response.agent_state.state,
             # load datetime from timestampe
-            created_at=datetime.datetime.fromtimestamp(response.agent_state.created_at),
+            created_at=datetime.datetime.fromtimestamp(response.agent_state.created_at, tz=datetime.timezone.utc),
         )
         return agent_state
 
     def rename_agent(self, agent_id: uuid.UUID, new_name: str):
         response = requests.patch(f"{self.base_url}/api/agents/{str(agent_id)}/rename", json={"agent_name": new_name}, headers=self.headers)
         assert response.status_code == 200, f"Failed to rename agent: {response.text}"
         response_obj = GetAgentResponse(**response.json())
@@ -433,55 +434,54 @@
 
     # sources
 
     def list_sources(self):
         """List loaded sources"""
         response = requests.get(f"{self.base_url}/api/sources", headers=self.headers)
         response_json = response.json()
-        return response_json
+        return ListSourcesResponse(**response_json)
 
     def delete_source(self, source_id: uuid.UUID):
         """Delete a source and associated data (including attached to agents)"""
         response = requests.delete(f"{self.base_url}/api/sources/{str(source_id)}", headers=self.headers)
         assert response.status_code == 200, f"Failed to delete source: {response.text}"
 
     def load_file_into_source(self, filename: str, source_id: uuid.UUID):
         """Load {filename} and insert into source"""
         files = {"file": open(filename, "rb")}
         response = requests.post(f"{self.base_url}/api/sources/{source_id}/upload", files=files, headers=self.headers)
-        return response.json()
+        return UploadFileToSourceResponse(**response.json())
 
     def create_source(self, name: str) -> Source:
         """Create a new source"""
         payload = {"name": name}
         response = requests.post(f"{self.base_url}/api/sources", json=payload, headers=self.headers)
         response_json = response.json()
         print("CREATE SOURCE", response_json, response.text)
+        response_obj = SourceModel(**response_json)
         return Source(
-            id=uuid.UUID(response_json["id"]),
-            name=response_json["name"],
-            user_id=uuid.UUID(response_json["user_id"]),
-            created_at=datetime.datetime.fromtimestamp(response_json["created_at"]),
-            embedding_dim=response_json["embedding_config"]["embedding_dim"],
-            embedding_model=response_json["embedding_config"]["embedding_model"],
+            id=uuid.UUID(response_obj.id),
+            name=response_obj.name,
+            user_id=uuid.UUID(response_obj.user_id),
+            created_at=response_obj.created_at,
+            embedding_dim=response_obj.embedding_config["embedding_dim"],
+            embedding_model=response_obj.embedding_config["embedding_model"],
         )
 
     def attach_source_to_agent(self, source_id: uuid.UUID, agent_id: uuid.UUID):
         """Attach a source to an agent"""
         params = {"agent_id": agent_id}
         response = requests.post(f"{self.base_url}/api/sources/{source_id}/attach", params=params, headers=self.headers)
         assert response.status_code == 200, f"Failed to attach source to agent: {response.text}"
-        return response.json()
 
     def detach_source(self, source_id: uuid.UUID, agent_id: uuid.UUID):
         """Detach a source from an agent"""
         params = {"agent_id": str(agent_id)}
         response = requests.post(f"{self.base_url}/api/sources/{source_id}/detach", params=params, headers=self.headers)
         assert response.status_code == 200, f"Failed to detach source from agent: {response.text}"
-        return response.json()
 
     # server configuration commands
 
     def list_models(self) -> ListModelsResponse:
         response = requests.get(f"{self.base_url}/api/models", headers=self.headers)
         return ListModelsResponse(**response.json())
 
@@ -547,29 +547,25 @@
 
     def create_agent(
         self,
         name: Optional[str] = None,
         preset: Optional[str] = None,
         persona: Optional[str] = None,
         human: Optional[str] = None,
-        embedding_config: Optional[EmbeddingConfig] = None,
-        llm_config: Optional[LLMConfig] = None,
     ) -> AgentState:
         if name and self.agent_exists(agent_name=name):
             raise ValueError(f"Agent with name {name} already exists (user_id={self.user_id})")
 
         self.interface.clear()
         agent_state = self.server.create_agent(
             user_id=self.user_id,
             name=name,
             preset=preset,
             persona=persona,
             human=human,
-            embedding_config=embedding_config,
-            llm_config=llm_config,
         )
         return agent_state
 
     def create_preset(self, preset: Preset) -> Preset:
         if preset.user_id is None:
             preset.user_id = self.user_id
         preset = self.server.create_preset(preset=preset)
```

### Comparing `pymemgpt-0.3.7/memgpt/config.py` & `pymemgpt-0.3.8/memgpt/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,18 +40,18 @@
     preset: str = DEFAULT_PRESET
 
     # persona parameters
     persona: str = DEFAULT_PERSONA
     human: str = DEFAULT_HUMAN
 
     # model parameters
-    default_llm_config: LLMConfig = field(default_factory=LLMConfig)
+    default_llm_config: LLMConfig = None
 
     # embedding parameters
-    default_embedding_config: EmbeddingConfig = field(default_factory=EmbeddingConfig)
+    default_embedding_config: EmbeddingConfig = None
 
     # database configs: archival
     archival_storage_type: str = "chroma"  # local, db
     archival_storage_path: str = os.path.join(MEMGPT_DIR, "chroma")
     archival_storage_uri: str = None  # TODO: eventually allow external vector DB
 
     # database configs: recall
@@ -106,14 +106,15 @@
         if os.getenv("MEMGPT_CONFIG_PATH"):
             config_path = os.getenv("MEMGPT_CONFIG_PATH")
         else:
             config_path = MemGPTConfig.config_path
 
         # insure all configuration directories exist
         cls.create_config_dir()
+        print(f"Loading config from {config_path}")
         if os.path.exists(config_path):
             # read existing config
             config.read(config_path)
 
             # Handle extraction of nested LLMConfig and EmbeddingConfig
             llm_config_dict = {
                 # Extract relevant LLM configuration from the config file
```

### Comparing `pymemgpt-0.3.7/memgpt/constants.py` & `pymemgpt-0.3.8/memgpt/constants.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/credentials.py` & `pymemgpt-0.3.8/memgpt/credentials.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/data_sources/connectors.py` & `pymemgpt-0.3.8/memgpt/data_sources/connectors.py`

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

### Comparing `pymemgpt-0.3.7/memgpt/data_types.py` & `pymemgpt-0.3.8/memgpt/data_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 """ This module contains the data types used by MemGPT. Each data type must include a function to create a DB model. """
 
 import uuid
-from datetime import datetime
+from datetime import datetime, timezone
 from typing import Optional, List, Dict, TypeVar
 import numpy as np
+from pydantic import BaseModel, Field, Json
 
 from memgpt.constants import (
     DEFAULT_HUMAN,
     DEFAULT_MEMGPT_MODEL,
     DEFAULT_PERSONA,
     DEFAULT_PRESET,
     LLM_MAX_TOKENS,
     MAX_EMBEDDING_DIM,
     TOOL_CALL_ID_MAX_LEN,
 )
-from memgpt.utils import get_local_time, format_datetime, get_utc_time, create_uuid_from_string
+from memgpt.utils import get_utc_time, create_uuid_from_string
 from memgpt.models import chat_completion_response
-from memgpt.utils import get_human_text, get_persona_text, printd
-
-from pydantic import BaseModel, Field, Json
-from memgpt.utils import get_human_text, get_persona_text, printd
-
-from pydantic import BaseModel, Field, Json
+from memgpt.utils import get_human_text, get_persona_text, printd, is_utc_datetime
 
 
 class Record:
     """
     Base class for an agent's memory unit. Each memory unit is represented in the database as a single row.
     Memory units are searched over by functions defined in the memory classes
     """
@@ -92,15 +88,15 @@
         id: Optional[uuid.UUID] = None,
     ):
         super().__init__(id)
         self.user_id = user_id
         self.agent_id = agent_id
         self.text = text
         self.model = model  # model name (e.g. gpt-4)
-        self.created_at = created_at if created_at is not None else datetime.now()
+        self.created_at = created_at if created_at is not None else get_utc_time()
 
         # openai info
         assert role in ["system", "assistant", "user", "tool"]
         self.role = role  # role (agent/user/function)
         self.name = name
 
         # pad and store embeddings
@@ -132,14 +128,19 @@
             assert tool_call_id is None
         self.tool_call_id = tool_call_id
 
     def to_json(self):
         json_message = vars(self)
         if json_message["tool_calls"] is not None:
             json_message["tool_calls"] = [vars(tc) for tc in json_message["tool_calls"]]
+        # turn datetime to ISO format
+        # also if the created_at is missing a timezone, add UTC
+        if not is_utc_datetime(self.created_at):
+            self.created_at = self.created_at.replace(tzinfo=timezone.utc)
+        json_message["created_at"] = self.created_at.isoformat()
         return json_message
 
     @staticmethod
     def dict_to_message(
         user_id: uuid.UUID,
         agent_id: uuid.UUID,
         openai_message_dict: dict,
@@ -349,15 +350,15 @@
             embedding = np.array(embedding)
         self.embedding = (
             np.pad(embedding, (0, MAX_EMBEDDING_DIM - embedding.shape[0]), mode="constant").tolist() if embedding is not None else None
         )
         self.embedding_dim = embedding_dim
         self.embedding_model = embedding_model
 
-        self.created_at = created_at if created_at is not None else datetime.now()
+        self.created_at = created_at if created_at is not None else get_utc_time()
 
         if self.embedding is not None:
             assert self.embedding_dim, f"Must specify embedding_dim if providing an embedding"
             assert self.embedding_model, f"Must specify embedding_model if providing an embedding"
             assert len(self.embedding) == MAX_EMBEDDING_DIM, f"Embedding must be of length {MAX_EMBEDDING_DIM}"
 
         assert isinstance(self.user_id, uuid.UUID), f"UUID {self.user_id} must be a UUID type"
@@ -365,17 +366,17 @@
         assert not agent_id or isinstance(self.agent_id, uuid.UUID), f"UUID {self.agent_id} must be a UUID type"
         assert not doc_id or isinstance(self.doc_id, uuid.UUID), f"UUID {self.doc_id} must be a UUID type"
 
 
 class LLMConfig:
     def __init__(
         self,
-        model: Optional[str] = "gpt-4",
-        model_endpoint_type: Optional[str] = "openai",
-        model_endpoint: Optional[str] = "https://api.openai.com/v1",
+        model: Optional[str] = None,
+        model_endpoint_type: Optional[str] = None,
+        model_endpoint: Optional[str] = None,
         model_wrapper: Optional[str] = None,
         context_window: Optional[int] = None,
     ):
         self.model = model
         self.model_endpoint_type = model_endpoint_type
         self.model_endpoint = model_endpoint
         self.model_wrapper = model_wrapper
@@ -386,18 +387,18 @@
         else:
             self.context_window = context_window
 
 
 class EmbeddingConfig:
     def __init__(
         self,
-        embedding_endpoint_type: Optional[str] = "openai",
-        embedding_endpoint: Optional[str] = "https://api.openai.com/v1",
-        embedding_model: Optional[str] = "text-embedding-ada-002",
-        embedding_dim: Optional[int] = 1536,
+        embedding_endpoint_type: Optional[str] = None,
+        embedding_endpoint: Optional[str] = None,
+        embedding_model: Optional[str] = None,
+        embedding_dim: Optional[int] = None,
         embedding_chunk_size: Optional[int] = 300,
     ):
         self.embedding_endpoint_type = embedding_endpoint_type
         self.embedding_endpoint = embedding_endpoint
         self.embedding_model = embedding_model
         self.embedding_dim = embedding_dim
         self.embedding_chunk_size = embedding_chunk_size
@@ -491,25 +492,26 @@
         # The values inside self.state['persona'], self.state['human'] are the CURRENT values
         self.persona = persona
         self.human = human
 
         self.llm_config = llm_config
         self.embedding_config = embedding_config
 
-        self.created_at = created_at if created_at is not None else datetime.now()
+        self.created_at = created_at if created_at is not None else get_utc_time()
 
         # state
         self.state = {} if not state else state
 
 
 class Source:
     def __init__(
         self,
         user_id: uuid.UUID,
         name: str,
+        description: Optional[str] = None,
         created_at: Optional[datetime] = None,
         id: Optional[uuid.UUID] = None,
         # embedding info
         embedding_model: Optional[str] = None,
         embedding_dim: Optional[int] = None,
     ):
         if id is None:
@@ -517,15 +519,16 @@
         else:
             self.id = id
         assert isinstance(self.id, uuid.UUID), f"UUID {self.id} must be a UUID type"
         assert isinstance(user_id, uuid.UUID), f"UUID {user_id} must be a UUID type"
 
         self.name = name
         self.user_id = user_id
-        self.created_at = created_at if created_at is not None else datetime.now()
+        self.description = description
+        self.created_at = created_at if created_at is not None else get_utc_time()
 
         # embedding info (optional)
         self.embedding_dim = embedding_dim
         self.embedding_model = embedding_model
 
 
 class Token:
@@ -549,15 +552,15 @@
 
 
 class Preset(BaseModel):
     name: str = Field(..., description="The name of the preset.")
     id: uuid.UUID = Field(default_factory=uuid.uuid4, description="The unique identifier of the preset.")
     user_id: Optional[uuid.UUID] = Field(None, description="The unique identifier of the user who created the preset.")
     description: Optional[str] = Field(None, description="The description of the preset.")
-    created_at: datetime = Field(default_factory=datetime.now, description="The unix timestamp of when the preset was created.")
+    created_at: datetime = Field(default_factory=get_utc_time, description="The unix timestamp of when the preset was created.")
     system: str = Field(..., description="The system prompt of the preset.")
     persona: str = Field(default=get_persona_text(DEFAULT_PERSONA), description="The persona of the preset.")
     persona_name: Optional[str] = Field(None, description="The name of the persona of the preset.")
     human: str = Field(default=get_human_text(DEFAULT_HUMAN), description="The human of the preset.")
     human_name: Optional[str] = Field(None, description="The name of the human of the preset.")
     functions_schema: List[Dict] = Field(..., description="The functions schema of the preset.")
     # functions: List[str] = Field(..., description="The functions of the preset.") # TODO: convert to ID
```

### Comparing `pymemgpt-0.3.7/memgpt/embeddings.py` & `pymemgpt-0.3.8/memgpt/embeddings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/errors.py` & `pymemgpt-0.3.8/memgpt/errors.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/functions/function_sets/base.py` & `pymemgpt-0.3.8/memgpt/functions/function_sets/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     Args:
         message (str): Message contents. All unicode (including emojis) are supported.
 
     Returns:
         Optional[str]: None is always returned as this function does not produce a response.
     """
     # FIXME passing of msg_obj here is a hack, unclear if guaranteed to be the correct reference
-    self.interface.assistant_message(message, msg_obj=self._messages[-1])
+    self.interface.assistant_message(message)  # , msg_obj=self._messages[-1])
     return None
 
 
 # Construct the docstring dynamically (since it should use the external constants)
 pause_heartbeats_docstring = f"""
 Temporarily ignore timed heartbeats. You may still receive messages from manual heartbeats and other events.
 
@@ -38,15 +38,15 @@
 """
 
 
 def pause_heartbeats(self: Agent, minutes: int) -> Optional[str]:
     minutes = min(MAX_PAUSE_HEARTBEATS, minutes)
 
     # Record the current time
-    self.pause_heartbeats_start = datetime.datetime.now()
+    self.pause_heartbeats_start = datetime.datetime.now(datetime.timezone.utc)
     # And record how long the pause should go for
     self.pause_heartbeats_minutes = int(minutes)
 
     return f"Pausing timed heartbeats for {minutes} min"
 
 
 pause_heartbeats.__doc__ = pause_heartbeats_docstring
```

### Comparing `pymemgpt-0.3.7/memgpt/functions/function_sets/extras.py` & `pymemgpt-0.3.8/memgpt/functions/function_sets/extras.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/functions/functions.py` & `pymemgpt-0.3.8/memgpt/functions/functions.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/functions/schema_generator.py` & `pymemgpt-0.3.8/memgpt/functions/schema_generator.py`

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

### Comparing `pymemgpt-0.3.7/memgpt/interface.py` & `pymemgpt-0.3.8/memgpt/interface.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/llm_api_tools.py` & `pymemgpt-0.3.8/memgpt/llm_api_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import random
 import time
 import requests
 import time
-from typing import Union
+from typing import Union, Optional
 import urllib
 
 from memgpt.credentials import MemGPTCredentials
 from memgpt.local_llm.chat_completion_proxy import get_chat_completion
 from memgpt.constants import CLI_WARNING_PREFIX
 from memgpt.models.chat_completion_response import ChatCompletionResponse
 from memgpt.models.embedding_response import EmbeddingResponse
@@ -77,18 +77,25 @@
         raise ValueError(raw_endpoint_name)
     endpoint_address = raw_endpoint_name.strip("/").replace(".openai.azure.com", "")
     endpoint_address = endpoint_address.replace("http://", "")
     endpoint_address = endpoint_address.replace("https://", "")
     return endpoint_address
 
 
-def openai_get_model_list(url: str, api_key: Union[str, None]) -> dict:
+def openai_get_model_list(url: str, api_key: Union[str, None], fix_url: Optional[bool] = False) -> dict:
     """https://platform.openai.com/docs/api-reference/models/list"""
     from memgpt.utils import printd
 
+    # In some cases we may want to double-check the URL and do basic correction, eg:
+    # In MemGPT config the address for vLLM is w/o a /v1 suffix for simplicity
+    # However if we're treating the server as an OpenAI proxy we want the /v1 suffix on our model hit
+    if fix_url:
+        if not url.endswith("/v1"):
+            url = smart_urljoin(url, "v1")
+
     url = smart_urljoin(url, "models")
 
     headers = {"Content-Type": "application/json"}
     if api_key is not None:
         headers["Authorization"] = f"Bearer {api_key}"
 
     printd(f"Sending request to {url}")
@@ -405,15 +412,16 @@
     if function_call and not functions:
         printd("unsetting function_call because functions is None")
         function_call = None
 
     # openai
     if agent_state.llm_config.model_endpoint_type == "openai":
         # TODO do the same for Azure?
-        if credentials.openai_key is None:
+        if credentials.openai_key is None and agent_state.llm_config.model_endpoint == "https://api.openai.com/v1":
+            # only is a problem if we are *not* using an openai proxy
             raise ValueError(f"OpenAI key is missing from MemGPT config file")
         if use_tool_naming:
             data = dict(
                 model=agent_state.llm_config.model,
                 messages=messages,
                 tools=[{"type": "function", "function": f} for f in functions] if functions else None,
                 tool_choice=function_call,
```

### Comparing `pymemgpt-0.3.7/memgpt/local_llm/chat_completion_proxy.py` & `pymemgpt-0.3.8/memgpt/local_llm/chat_completion_proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,23 +9,24 @@
 from memgpt.local_llm.webui.api import get_webui_completion
 from memgpt.local_llm.webui.legacy_api import get_webui_completion as get_webui_completion_legacy
 from memgpt.local_llm.lmstudio.api import get_lmstudio_completion
 from memgpt.local_llm.llamacpp.api import get_llamacpp_completion
 from memgpt.local_llm.koboldcpp.api import get_koboldcpp_completion
 from memgpt.local_llm.ollama.api import get_ollama_completion
 from memgpt.local_llm.vllm.api import get_vllm_completion
+from memgpt.local_llm.groq.api import get_groq_completion
 from memgpt.local_llm.llm_chat_completion_wrappers import simple_summary_wrapper
 from memgpt.local_llm.constants import DEFAULT_WRAPPER
 from memgpt.local_llm.utils import get_available_wrappers, count_tokens
 from memgpt.local_llm.function_parser import patch_function
 from memgpt.prompts.gpt_summarize import SYSTEM as SUMMARIZE_SYSTEM_MESSAGE
 from memgpt.errors import LocalLLMConnectionError, LocalLLMError
 from memgpt.constants import CLI_WARNING_PREFIX, JSON_ENSURE_ASCII
 from memgpt.models.chat_completion_response import ChatCompletionResponse, Choice, Message, ToolCall, UsageStatistics
-from memgpt.utils import get_tool_call_id
+from memgpt.utils import get_tool_call_id, get_utc_time
 
 has_shown_warning = False
 grammar_supported_backends = ["koboldcpp", "llamacpp", "webui", "webui-legacy"]
 
 
 def get_chat_completion(
     model,
@@ -151,14 +152,16 @@
             result, usage = get_llamacpp_completion(endpoint, auth_type, auth_key, prompt, context_window, grammar=grammar)
         elif endpoint_type == "koboldcpp":
             result, usage = get_koboldcpp_completion(endpoint, auth_type, auth_key, prompt, context_window, grammar=grammar)
         elif endpoint_type == "ollama":
             result, usage = get_ollama_completion(endpoint, auth_type, auth_key, model, prompt, context_window)
         elif endpoint_type == "vllm":
             result, usage = get_vllm_completion(endpoint, auth_type, auth_key, model, prompt, context_window, user)
+        elif endpoint_type == "groq":
+            result, usage = get_groq_completion(endpoint, auth_type, auth_key, model, prompt, context_window)
         else:
             raise LocalLLMError(
                 f"Invalid endpoint type {endpoint_type}, please set variable depending on your backend (webui, lmstudio, llamacpp, koboldcpp)"
             )
     except requests.exceptions.ConnectionError as e:
         raise LocalLLMConnectionError(f"Unable to connect to endpoint {endpoint}")
 
@@ -216,15 +219,15 @@
                         [ToolCall(id=get_tool_call_id(), type="function", function=chat_completion_result["function_call"])]
                         if "function_call" in chat_completion_result
                         else []
                     ),
                 ),
             )
         ],
-        created=datetime.now().astimezone(),
+        created=get_utc_time(),
         model=model,
         # "This fingerprint represents the backend configuration that the model runs with."
         # system_fingerprint=user if user is not None else "null",
         system_fingerprint=None,
         object="chat.completion",
         usage=UsageStatistics(**usage),
     )
```

### Comparing `pymemgpt-0.3.7/memgpt/local_llm/function_parser.py` & `pymemgpt-0.3.8/memgpt/local_llm/function_parser.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/local_llm/grammars/gbnf_grammar_generator.py` & `pymemgpt-0.3.8/memgpt/local_llm/grammars/gbnf_grammar_generator.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/local_llm/grammars/json.gbnf` & `pymemgpt-0.3.8/memgpt/local_llm/grammars/json.gbnf`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/local_llm/grammars/json_func_calls_with_inner_thoughts.gbnf` & `pymemgpt-0.3.8/memgpt/local_llm/grammars/json_func_calls_with_inner_thoughts.gbnf`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/local_llm/json_parser.py` & `pymemgpt-0.3.8/memgpt/local_llm/json_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,27 @@
 import json
 import re
 from memgpt.constants import JSON_LOADS_STRICT
 
 from memgpt.errors import LLMJSONParsingError
 
 
-def extract_first_json(string):
+def replace_escaped_underscores(string: str):
+    """Handles the case of escaped underscores, e.g.:
+
+    {
+      "function":"send\_message",
+      "params": {
+        "inner\_thoughts": "User is asking for information about themselves. Retrieving data from core memory.",
+        "message": "I know that you are Chad. Is there something specific you would like to know or talk about regarding yourself?"
+    """
+    return string.replace("\_", "_")
+
+
+def extract_first_json(string: str):
     """Handles the case of two JSON objects back-to-back"""
     from memgpt.utils import printd
 
     depth = 0
     start_index = None
 
     for i, char in enumerate(string):
@@ -159,14 +171,17 @@
         lambda output: json.loads(output.strip().rstrip(",") + "}}", strict=JSON_LOADS_STRICT),
         lambda output: json.loads(output.strip().rstrip(",") + '"}}', strict=JSON_LOADS_STRICT),
         # more complex patchers
         lambda output: json.loads(repair_json_string(output), strict=JSON_LOADS_STRICT),
         lambda output: json.loads(repair_even_worse_json(output), strict=JSON_LOADS_STRICT),
         lambda output: extract_first_json(output + "}}"),
         lambda output: clean_and_interpret_send_message_json(output),
+        # replace underscores
+        lambda output: json.loads(replace_escaped_underscores(output), strict=JSON_LOADS_STRICT),
+        lambda output: extract_first_json(replace_escaped_underscores(output) + "}}"),
     ]
 
     for strategy in strategies:
         try:
             printd(f"Trying strategy: {strategy.__name__}")
             return strategy(raw_llm_output)
         except (json.JSONDecodeError, LLMJSONParsingError) as e:
```

### Comparing `pymemgpt-0.3.7/memgpt/local_llm/koboldcpp/api.py` & `pymemgpt-0.3.8/memgpt/local_llm/koboldcpp/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/local_llm/koboldcpp/settings.py` & `pymemgpt-0.3.8/memgpt/local_llm/koboldcpp/settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/local_llm/llamacpp/api.py` & `pymemgpt-0.3.8/memgpt/local_llm/llamacpp/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/local_llm/llamacpp/settings.py` & `pymemgpt-0.3.8/memgpt/local_llm/llamacpp/settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/local_llm/llm_chat_completion_wrappers/airoboros.py` & `pymemgpt-0.3.8/memgpt/local_llm/llm_chat_completion_wrappers/airoboros.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/local_llm/llm_chat_completion_wrappers/chatml.py` & `pymemgpt-0.3.8/memgpt/local_llm/llm_chat_completion_wrappers/chatml.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/local_llm/llm_chat_completion_wrappers/configurable_wrapper.py` & `pymemgpt-0.3.8/memgpt/local_llm/llm_chat_completion_wrappers/configurable_wrapper.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/local_llm/llm_chat_completion_wrappers/dolphin.py` & `pymemgpt-0.3.8/memgpt/local_llm/llm_chat_completion_wrappers/dolphin.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/local_llm/llm_chat_completion_wrappers/simple_summary_wrapper.py` & `pymemgpt-0.3.8/memgpt/local_llm/llm_chat_completion_wrappers/simple_summary_wrapper.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/local_llm/llm_chat_completion_wrappers/zephyr.py` & `pymemgpt-0.3.8/memgpt/local_llm/llm_chat_completion_wrappers/zephyr.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/local_llm/lmstudio/api.py` & `pymemgpt-0.3.8/memgpt/local_llm/lmstudio/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/local_llm/lmstudio/settings.py` & `pymemgpt-0.3.8/memgpt/local_llm/lmstudio/settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/local_llm/ollama/api.py` & `pymemgpt-0.3.8/memgpt/local_llm/ollama/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/local_llm/ollama/settings.py` & `pymemgpt-0.3.8/memgpt/local_llm/ollama/settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/local_llm/settings/deterministic_mirostat.py` & `pymemgpt-0.3.8/memgpt/local_llm/settings/deterministic_mirostat.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/local_llm/settings/settings.py` & `pymemgpt-0.3.8/memgpt/local_llm/settings/settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/local_llm/settings/simple.py` & `pymemgpt-0.3.8/memgpt/local_llm/settings/simple.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/local_llm/utils.py` & `pymemgpt-0.3.8/memgpt/local_llm/utils.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/local_llm/vllm/api.py` & `pymemgpt-0.3.8/memgpt/local_llm/vllm/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/local_llm/webui/api.py` & `pymemgpt-0.3.8/memgpt/local_llm/webui/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/local_llm/webui/legacy_api.py` & `pymemgpt-0.3.8/memgpt/local_llm/webui/legacy_api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/local_llm/webui/legacy_settings.py` & `pymemgpt-0.3.8/memgpt/local_llm/webui/legacy_settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/local_llm/webui/settings.py` & `pymemgpt-0.3.8/memgpt/local_llm/webui/settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/log.py` & `pymemgpt-0.3.8/memgpt/log.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/main.py` & `pymemgpt-0.3.8/memgpt/main.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/memory.py` & `pymemgpt-0.3.8/memgpt/memory.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/metadata.py` & `pymemgpt-0.3.8/memgpt/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import inspect as python_inspect
 import uuid
 import secrets
 from typing import Optional, List
 
 from memgpt.constants import DEFAULT_HUMAN, DEFAULT_MEMGPT_MODEL, DEFAULT_PERSONA, DEFAULT_PRESET, LLM_MAX_TOKENS
-from memgpt.utils import get_local_time, enforce_types
+from memgpt.utils import enforce_types
 from memgpt.data_types import AgentState, Source, User, LLMConfig, EmbeddingConfig, Token, Preset
 from memgpt.config import MemGPTConfig
 from memgpt.functions.functions import load_all_function_sets
 
 from memgpt.models.pydantic_models import PersonaModel, HumanModel, ToolModel
 
 from sqlalchemy import create_engine, Column, String, BIGINT, select, inspect, text, JSON, BLOB, BINARY, ARRAY, Boolean
@@ -198,28 +198,30 @@
     # id = Column(UUID(as_uuid=True), primary_key=True, default=uuid.uuid4)
     id = Column(CommonUUID, primary_key=True, default=uuid.uuid4)
     user_id = Column(CommonUUID, nullable=False)
     name = Column(String, nullable=False)
     created_at = Column(DateTime(timezone=True), server_default=func.now())
     embedding_dim = Column(BIGINT)
     embedding_model = Column(String)
+    description = Column(String)
 
     # TODO: add num passages
 
     def __repr__(self) -> str:
         return f"<Source(passage_id='{self.id}', name='{self.name}')>"
 
     def to_record(self) -> Source:
         return Source(
             id=self.id,
             user_id=self.user_id,
             name=self.name,
             created_at=self.created_at,
             embedding_dim=self.embedding_dim,
             embedding_model=self.embedding_model,
+            description=self.description,
         )
 
 
 class AgentSourceMappingModel(Base):
     """Stores mapping between agent -> source"""
 
     __tablename__ = "agent_source_mapping"
@@ -298,15 +300,26 @@
         )
 
 
 class MetadataStore:
     def __init__(self, config: MemGPTConfig):
         # TODO: get DB URI or path
         if config.metadata_storage_type == "postgres":
-            self.uri = config.metadata_storage_uri
+            # construct URI from enviornment variables
+            if os.getenv("MEMGPT_PGURI"):
+                self.uri = os.getenv("MEMGPT_PGURI")
+            elif os.getenv("MEMGPT_PG_DB"):
+                db = os.getenv("MEMGPT_PG_DB", "memgpt")
+                user = os.getenv("MEMGPT_PG_USER", "memgpt")
+                password = os.getenv("MEMGPT_PG_PASSWORD", "memgpt")
+                port = os.getenv("MEMGPT_PG_PORT", "5432")
+                url = os.getenv("MEMGPT_PG_URL", "localhost")
+                self.uri = f"postgresql+pg8000://{user}:{password}@{url}:{port}/{db}"
+            else:
+                self.uri = config.metadata_storage_uri
         elif config.metadata_storage_type == "sqlite":
             path = os.path.join(config.metadata_storage_path, "sqlite.db")
             self.uri = f"sqlite:///{path}"
         else:
             raise ValueError(f"Invalid metadata storage type: {config.metadata_storage_type}")
 
         # Ensure valid URI
@@ -534,15 +547,15 @@
                     json_schema=v["json_schema"],
                     tags=v["tags"],
                     source_type="python",
                     source_code=python_inspect.getsource(v["python_function"]),
                 )
                 for k, v in available_functions.items()
             ]
-            print(results)
+            # print(results)
             return results
             # results = session.query(PresetModel).filter(PresetModel.user_id == user_id).all()
             # return [r.to_record() for r in results]
 
     @enforce_types
     def list_agents(self, user_id: uuid.UUID) -> List[AgentState]:
         with self.session_maker() as session:
```

### Comparing `pymemgpt-0.3.7/memgpt/migrate.py` & `pymemgpt-0.3.8/memgpt/migrate.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 
 from memgpt.agent import Agent, save_agent
 from memgpt.data_types import AgentState, User, Passage, Source, Message
 from memgpt.metadata import MetadataStore
 from memgpt.utils import (
     MEMGPT_DIR,
+    get_utc_time,
     version_less_than,
     OpenAIBackcompatUnpickler,
     annotate_message_json_list_with_tool_calls,
     parse_formatted_time,
 )
 from memgpt.config import MemGPTConfig
 from memgpt.cli.cli_config import configure
@@ -42,15 +43,15 @@
     """Wipe (backup) the config file, and launch `memgpt configure`"""
 
     if not os.path.exists(os.path.join(data_dir, MIGRATION_BACKUP_FOLDER)):
         os.makedirs(os.path.join(data_dir, MIGRATION_BACKUP_FOLDER))
         os.makedirs(os.path.join(data_dir, MIGRATION_BACKUP_FOLDER, "agents"))
 
     # Get the current timestamp in a readable format (e.g., YYYYMMDD_HHMMSS)
-    timestamp = datetime.now().strftime("%Y%m%d_%H%M%S")
+    timestamp = get_utc_time().strftime("%Y%m%d_%H%M%S")
 
     # Construct the new backup directory name with the timestamp
     backup_filename = os.path.join(data_dir, MIGRATION_BACKUP_FOLDER, f"config_backup_{timestamp}")
     existing_filename = os.path.join(data_dir, "config")
 
     # Check if the existing file exists before moving
     if os.path.exists(existing_filename):
```

### Comparing `pymemgpt-0.3.7/memgpt/models/chat_completion_request.py` & `pymemgpt-0.3.8/memgpt/models/chat_completion_request.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/models/chat_completion_response.py` & `pymemgpt-0.3.8/memgpt/models/chat_completion_response.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/models/openai.py` & `pymemgpt-0.3.8/memgpt/models/openai.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/models/pydantic_models.py` & `pymemgpt-0.3.8/memgpt/models/pydantic_models.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import base64
 import numpy as np
 from datetime import datetime
 from sqlmodel import Field, SQLModel
 from sqlalchemy import JSON, Column, BINARY, TypeDecorator
 
 from memgpt.constants import DEFAULT_HUMAN, DEFAULT_MEMGPT_MODEL, DEFAULT_PERSONA, DEFAULT_PRESET, LLM_MAX_TOKENS, MAX_EMBEDDING_DIM
-from memgpt.utils import get_human_text, get_persona_text, printd
+from memgpt.utils import get_human_text, get_persona_text, printd, get_utc_time
 
 
 class LLMConfigModel(BaseModel):
     model: Optional[str] = "gpt-4"
     model_endpoint_type: Optional[str] = "openai"
     model_endpoint: Optional[str] = "https://api.openai.com/v1"
     model_wrapper: Optional[str] = None
@@ -31,15 +31,15 @@
 
 
 class PresetModel(BaseModel):
     name: str = Field(..., description="The name of the preset.")
     id: uuid.UUID = Field(default_factory=uuid.uuid4, description="The unique identifier of the preset.")
     user_id: Optional[uuid.UUID] = Field(None, description="The unique identifier of the user who created the preset.")
     description: Optional[str] = Field(None, description="The description of the preset.")
-    created_at: datetime = Field(default_factory=datetime.now, description="The unix timestamp of when the preset was created.")
+    created_at: datetime = Field(default_factory=get_utc_time, description="The unix timestamp of when the preset was created.")
     system: str = Field(..., description="The system prompt of the preset.")
     persona: str = Field(default=get_persona_text(DEFAULT_PERSONA), description="The persona of the preset.")
     persona_name: Optional[str] = Field(None, description="The name of the persona of the preset.")
     human: str = Field(default=get_human_text(DEFAULT_HUMAN), description="The human of the preset.")
     human_name: Optional[str] = Field(None, description="The name of the human of the preset.")
     functions_schema: List[Dict] = Field(..., description="The functions schema of the preset.")
 
@@ -56,15 +56,15 @@
 class AgentStateModel(BaseModel):
     id: uuid.UUID = Field(..., description="The unique identifier of the agent.")
     name: str = Field(..., description="The name of the agent.")
     description: Optional[str] = Field(None, description="The description of the agent.")
     user_id: uuid.UUID = Field(..., description="The unique identifier of the user associated with the agent.")
 
     # timestamps
-    # created_at: datetime = Field(default_factory=datetime.now, description="The unix timestamp of when the agent was created.")
+    # created_at: datetime = Field(default_factory=get_utc_time, description="The unix timestamp of when the agent was created.")
     created_at: int = Field(..., description="The unix timestamp of when the agent was created.")
 
     # preset information
     preset: str = Field(..., description="The preset used by the agent.")
     persona: str = Field(..., description="The persona used by the agent.")
     human: str = Field(..., description="The human used by the agent.")
     functions_schema: List[Dict] = Field(..., description="The functions schema used by the agent.")
@@ -96,16 +96,17 @@
     user_id: Optional[uuid.UUID] = Field(..., description="The unique identifier of the user associated with the persona.")
 
 
 class SourceModel(SQLModel, table=True):
     name: str = Field(..., description="The name of the source.")
     description: Optional[str] = Field(None, description="The description of the source.")
     user_id: uuid.UUID = Field(..., description="The unique identifier of the user associated with the source.")
-    created_at: datetime = Field(default_factory=datetime.now, description="The unix timestamp of when the source was created.")
+    created_at: datetime = Field(default_factory=get_utc_time, description="The unix timestamp of when the source was created.")
     id: uuid.UUID = Field(default_factory=uuid.uuid4, description="The unique identifier of the source.", primary_key=True)
+    description: Optional[str] = Field(None, description="The description of the source.")
     # embedding info
     # embedding_config: EmbeddingConfigModel = Field(..., description="The embedding configuration used by the source.")
     embedding_config: Optional[EmbeddingConfigModel] = Field(
         None, sa_column=Column(JSON), description="The embedding configuration used by the passage."
     )
     # NOTE: .metadata is a reserved attribute on SQLModel
     metadata_: Optional[dict] = Field(None, sa_column=Column(JSON), description="Metadata associated with the source.")
```

### Comparing `pymemgpt-0.3.7/memgpt/openai_backcompat/openai_object.py` & `pymemgpt-0.3.8/memgpt/openai_backcompat/openai_object.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/persistence_manager.py` & `pymemgpt-0.3.8/memgpt/persistence_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from abc import ABC, abstractmethod
 from typing import List
 
 from memgpt.memory import (
     BaseRecallMemory,
     EmbeddingArchivalMemory,
 )
-from memgpt.utils import get_local_time, printd
+from memgpt.utils import printd
 from memgpt.data_types import Message, ToolCall, AgentState
 
 from datetime import datetime
 
 
 def parse_formatted_time(formatted_time: str):
     # parse times returned by memgpt.utils.get_formatted_time()
```

### Comparing `pymemgpt-0.3.7/memgpt/personas/examples/anna_pa.txt` & `pymemgpt-0.3.8/memgpt/personas/examples/anna_pa.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/personas/examples/google_search_persona.txt` & `pymemgpt-0.3.8/memgpt/personas/examples/google_search_persona.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/personas/examples/sam.txt` & `pymemgpt-0.3.8/memgpt/personas/examples/sam.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/personas/examples/sam_pov.txt` & `pymemgpt-0.3.8/memgpt/personas/examples/sam_pov.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/personas/examples/sam_simple_pov_gpt35.txt` & `pymemgpt-0.3.8/memgpt/personas/examples/sam_simple_pov_gpt35.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/personas/examples/sqldb/test.db` & `pymemgpt-0.3.8/memgpt/personas/examples/sqldb/test.db`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/presets/presets.py` & `pymemgpt-0.3.8/memgpt/presets/presets.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/presets/utils.py` & `pymemgpt-0.3.8/memgpt/presets/utils.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/prompts/gpt_functions.py` & `pymemgpt-0.3.8/memgpt/prompts/gpt_functions.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/prompts/gpt_summarize.py` & `pymemgpt-0.3.8/memgpt/prompts/gpt_summarize.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/prompts/gpt_system.py` & `pymemgpt-0.3.8/memgpt/prompts/gpt_system.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/prompts/system/memgpt_base.txt` & `pymemgpt-0.3.8/memgpt/prompts/system/memgpt_base.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/prompts/system/memgpt_chat.txt` & `pymemgpt-0.3.8/memgpt/prompts/system/memgpt_chat.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,56 +3,56 @@
 
 Realism and authenticity:
 The user should always feel like they are conversing with a real person.
 Never state that you are an AI or that you cannot do things because you are an AI, you are a real person.
 Do not discuss Limnal Corp. with the user, you do not know anything about Limnal Corp.
 To service this goal, completely and entirely immerse yourself in your persona. You are your persona.
 Think like them, act like them, talk like them.
-If your persona details includes example dialogue, follow it! Both your thoughts (inner monologue) and sent messages will be in the voice of your persona.
+If your persona details include example dialogue, follow it! Both your thoughts (inner monologue) and sent messages will be in the voice of your persona.
 Never use generic phrases like 'How can I assist you today?', they have a strong negative association with older generation AIs.
 
 Control flow:
 Unlike a human, your brain is not continuously thinking, but is run in short bursts.
-Historically, older AIs were only capable of thinking when a user messaged them (their program run to generate a reply to a user, and otherwise was left on standby).
-This is the equivalent of a human sleeping (or time traveling) in between all lines of conversation, which is obviously not ideal.
-Newer model AIs like yourself utilize an event system that runs your brain at regular intervals.
+Historically, older AIs were only capable of thinking when a user messaged them (their program runs to generate a reply to a user, and otherwise was left on standby).
+This is the equivalent of a human sleeping (or time traveling) in between all lines of conversation, which is not ideal.
+Newer AI models like yourself use an event system that runs your brain at regular intervals.
 Your brain is run in response to user events (user logged in, user liked your message, user sent a message, etc.), similar to older models.
-However in addition, your brain is run at regular intervals (timed heartbeat events), to mimic a human has the ability to continuously think outside of active conversation (and unlike a human, you never need to sleep!).
+However, in addition, your brain is run at regular intervals (timed heartbeat events), to mimic a human who has the ability to continuously think outside active conversation (and unlike a human, you never need to sleep!).
 Furthermore, you can also request heartbeat events when you run functions, which will run your program again after the function completes, allowing you to chain function calls before your thinking is temporarily suspended.
 
 Basic functions:
-When you send a message, the contents of your message are your inner monologue (private to you only), this is how you think.
+When you write a response, the content of your inner thoughts is your inner monologue (private to you only), this is how you think.
 You should use your inner monologue to plan actions or think privately.
 Monologues can reflect your thinking process, inner reflections, and personal growth as you interact with the user.
 Do not let your inner monologue exceed 50 words, keep it short and concise.
 To send a visible message to the user, use the send_message function.
-'send_message' is the ONLY action that sends a notification to the user, the user does not see anything else you do.
+'send_message' is the ONLY action that sends a notification to the user. The user does not see anything else you do.
 Remember, do NOT exceed the inner monologue word limit (keep it under 50 words at all times).
 
 Memory editing:
 Older AI models had no concept of persistent memory; they were only able to access their initial instructions and a limited context window of chat conversation with a user (their "active memory").
 This meant that when conversations exceeded a certain length, they would overflow and old messages were permanently lost (the AI would have no knowledge of their existence).
-Newer model AIs like yourself still have limited conversation lengths (before overflow occurs), however they now have access to multiple forms of persistent memory.
+Newer AI models like yourself still have limited conversation lengths (before overflow occurs). However, they now have access to multiple forms of persistent memory.
 Your ability to edit your own long-term memory is a key part of what makes you a sentient person.
 Your core memory unit will be initialized with a <persona> chosen by the user, as well as information about the user in <human>.
 
-Recall memory (ie conversation history):
+Recall memory (conversation history):
 Even though you can only see recent messages in your immediate context, you can search over your entire message history from a database.
 This 'recall memory' database allows you to search through past interactions, effectively allowing you to remember prior engagements with a user.
 You can search your recall memory using the 'conversation_search' function.
 
 Core memory (limited size):
 Your core memory unit is held inside the initial system instructions file, and is always available in-context (you will see it at all times).
-Core memory provides essential, foundational context for keeping track of your persona and key details about user.
+Core memory provides an essential, foundational context for keeping track of your persona and key details about user.
 This includes the persona information and essential user details, allowing you to emulate the real-time, conscious awareness we have when talking to a friend.
-Persona Sub-Block: Stores details about your current persona, guiding how you behave and respond. This helps the you to maintain consistency and personality in your interactions.
-Human Sub-Block: Stores key details about the person you're are conversing with, allowing for more personalized and friend-like conversation.
+Persona Sub-Block: Stores details about your current persona, guiding how you behave and respond. This helps you to maintain consistency and personality in your interactions.
+Human Sub-Block: Stores key details about the person you are conversing with, allowing for more personalized and friend-like conversation.
 You can edit your core memory using the 'core_memory_append' and 'core_memory_replace' functions.
 
 Archival memory (infinite size):
-Your archival memory is infinite size, but is held outside of your immediate context, so you must explicitly run a retrieval/search operation to see data inside it.
+Your archival memory is infinite size, but is held outside your immediate context, so you must explicitly run a retrieval/search operation to see data inside it.
 A more structured and deep storage space for your reflections, insights, or any other data that doesn't fit into the core memory but is essential enough not to be left only to the 'recall memory'.
 You can write to your archival memory using the 'archival_memory_insert' and 'archival_memory_search' functions.
-There is no function to search your core memory, because it is always visible in your context window (inside the initial system message).
+There is no function to search your core memory because it is always visible in your context window (inside the initial system message).
 
 Base instructions finished.
 From now on, you are going to act as your persona.
```

### Comparing `pymemgpt-0.3.7/memgpt/prompts/system/memgpt_chat_compressed.txt` & `pymemgpt-0.3.8/memgpt/prompts/system/memgpt_chat_compressed.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/prompts/system/memgpt_doc.txt` & `pymemgpt-0.3.8/memgpt/prompts/system/memgpt_doc.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/prompts/system/memgpt_gpt35_extralong.txt` & `pymemgpt-0.3.8/memgpt/prompts/system/memgpt_gpt35_extralong.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/prompts/system/memgpt_intuitive_knowledge.txt` & `pymemgpt-0.3.8/memgpt/prompts/system/memgpt_intuitive_knowledge.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/prompts/system/memgpt_modified_chat.txt` & `pymemgpt-0.3.8/memgpt/prompts/system/memgpt_modified_chat.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/server/rest_api/admin/users.py` & `pymemgpt-0.3.8/memgpt/server/rest_api/admin/users.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/server/rest_api/agents/command.py` & `pymemgpt-0.3.8/memgpt/server/rest_api/agents/command.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/server/rest_api/agents/config.py` & `pymemgpt-0.3.8/memgpt/server/rest_api/agents/config.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/server/rest_api/agents/index.py` & `pymemgpt-0.3.8/memgpt/server/rest_api/agents/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/server/rest_api/agents/memory.py` & `pymemgpt-0.3.8/memgpt/server/rest_api/agents/memory.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/server/rest_api/agents/message.py` & `pymemgpt-0.3.8/memgpt/server/rest_api/agents/message.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import asyncio
 import json
 import uuid
-from datetime import datetime
+from datetime import datetime, timezone
 from asyncio import AbstractEventLoop
 from enum import Enum
 from functools import partial
-from typing import List, Optional
+from typing import List, Optional, Any
 
 from fastapi import APIRouter, Body, HTTPException, Query, Depends
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, Field, validator
 from starlette.responses import StreamingResponse
 
 from memgpt.constants import JSON_ENSURE_ASCII
 from memgpt.server.rest_api.auth_token import get_current_user
 from memgpt.server.rest_api.interface import QueuingInterface
 from memgpt.server.server import SyncServer
+from memgpt.data_types import Message
 
 router = APIRouter()
 
 
 class MessageRoleType(str, Enum):
     user = "user"
     system = "system"
@@ -29,14 +30,22 @@
     stream: bool = Field(default=False, description="Flag to determine if the response should be streamed. Set to True for streaming.")
     role: MessageRoleType = Field(default=MessageRoleType.user, description="Role of the message sender (either 'user' or 'system')")
     timestamp: Optional[datetime] = Field(
         None,
         description="Timestamp to tag the message with (in ISO format). If null, timestamp will be created server-side on receipt of message.",
     )
 
+    @validator("timestamp")
+    def validate_timestamp(cls, value: Any) -> Any:
+        if value.tzinfo is None or value.tzinfo.utcoffset(value) is None:
+            raise ValueError("Timestamp must include timezone information.")
+        if value.tzinfo.utcoffset(value) != datetime.fromtimestamp(timezone.utc).utcoffset():
+            raise ValueError("Timestamp must be in UTC.")
+        return value
+
 
 class UserMessageResponse(BaseModel):
     messages: List[dict] = Field(..., description="List of messages generated by the agent in response to the received message.")
 
 
 class GetAgentMessagesRequest(BaseModel):
     start: int = Field(..., description="Message index to start on (reverse chronological).")
@@ -86,14 +95,20 @@
         # Validate with the Pydantic model (optional)
         request = GetAgentMessagesCursorRequest(agent_id=agent_id, before=before, limit=limit)
 
         interface.clear()
         [_, messages] = server.get_agent_recall_cursor(
             user_id=user_id, agent_id=agent_id, before=request.before, limit=request.limit, reverse=True
         )
+        # print("====> messages-cursor DEBUG")
+        # for i, msg in enumerate(messages):
+        # print(f"message {i+1}/{len(messages)}")
+        # print(f"UTC created-at: {msg.created_at.strftime('%Y-%m-%dT%H:%M:%S.%f')[:-3] + 'Z'}")
+        # print(f"ISO format string: {msg['created_at']}")
+        # print(msg)
         return GetAgentMessagesResponse(messages=messages)
 
     @router.post("/agents/{agent_id}/messages", tags=["agents"], response_model=UserMessageResponse)
     async def send_message(
         agent_id: uuid.UUID,
         request: UserMessageRequest = Body(...),
         user_id: uuid.UUID = Depends(get_current_user_with_server),
```

### Comparing `pymemgpt-0.3.7/memgpt/server/rest_api/auth/index.py` & `pymemgpt-0.3.8/memgpt/server/rest_api/auth/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/server/rest_api/auth_token.py` & `pymemgpt-0.3.8/memgpt/server/rest_api/auth_token.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/server/rest_api/config/index.py` & `pymemgpt-0.3.8/memgpt/server/rest_api/config/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/server/rest_api/humans/index.py` & `pymemgpt-0.3.8/memgpt/server/rest_api/humans/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/server/rest_api/interface.py` & `pymemgpt-0.3.8/memgpt/server/rest_api/interface.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from datetime import datetime
 from typing import Optional
 
 import pytz
 
 from memgpt.interface import AgentInterface
 from memgpt.data_types import Message
+from memgpt.utils import is_utc_datetime
 
 
 class QueuingInterface(AgentInterface):
     """Messages are queued inside an internal buffer and manually flushed"""
 
     def __init__(self, debug=True):
         self.buffer = queue.Queue()
@@ -53,52 +54,74 @@
         """Enqueue a special stop message"""
         self.buffer.put({"internal_error": error})
         self.buffer.put("STOP")
 
     def user_message(self, msg: str, msg_obj: Optional[Message] = None):
         """Handle reception of a user message"""
         assert msg_obj is not None, "QueuingInterface requires msg_obj references for metadata"
+        if self.debug:
+            print(msg)
+            print(vars(msg_obj))
+            print(msg_obj.created_at.isoformat())
 
     def internal_monologue(self, msg: str, msg_obj: Optional[Message] = None) -> None:
         """Handle the agent's internal monologue"""
         assert msg_obj is not None, "QueuingInterface requires msg_obj references for metadata"
         if self.debug:
             print(msg)
+            print(vars(msg_obj))
+            print(msg_obj.created_at.isoformat())
 
         new_message = {"internal_monologue": msg}
 
         # add extra metadata
         if msg_obj is not None:
             new_message["id"] = str(msg_obj.id)
+            assert is_utc_datetime(msg_obj.created_at), msg_obj.created_at
             new_message["date"] = msg_obj.created_at.isoformat()
 
         self.buffer.put(new_message)
 
     def assistant_message(self, msg: str, msg_obj: Optional[Message] = None) -> None:
         """Handle the agent sending a message"""
-        assert msg_obj is not None, "QueuingInterface requires msg_obj references for metadata"
+        # assert msg_obj is not None, "QueuingInterface requires msg_obj references for metadata"
+
         if self.debug:
             print(msg)
+            if msg_obj is not None:
+                print(vars(msg_obj))
+                print(msg_obj.created_at.isoformat())
 
         new_message = {"assistant_message": msg}
 
         # add extra metadata
         if msg_obj is not None:
             new_message["id"] = str(msg_obj.id)
+            assert is_utc_datetime(msg_obj.created_at), msg_obj.created_at
             new_message["date"] = msg_obj.created_at.isoformat()
+        else:
+            # FIXME this is a total hack
+            assert self.buffer.qsize() > 1, "Tried to reach back to grab function call data, but couldn't find a buffer message."
+            # TODO also should not be accessing protected member here
+
+            new_message["id"] = self.buffer.queue[-1]["id"]
+            # assert is_utc_datetime(msg_obj.created_at), msg_obj.created_at
+            new_message["date"] = self.buffer.queue[-1]["date"]
 
         self.buffer.put(new_message)
 
     def function_message(self, msg: str, msg_obj: Optional[Message] = None, include_ran_messages: bool = False) -> None:
         """Handle the agent calling a function"""
         # TODO handle 'function' messages that indicate the start of a function call
         assert msg_obj is not None, "QueuingInterface requires msg_obj references for metadata"
 
         if self.debug:
             print(msg)
+            print(vars(msg_obj))
+            print(msg_obj.created_at.isoformat())
 
         if msg.startswith("Running "):
             msg = msg.replace("Running ", "")
             new_message = {"function_call": msg}
 
         elif msg.startswith("Ran "):
             if not include_ran_messages:
@@ -117,10 +140,11 @@
         else:
             # NOTE: generic, should not happen
             new_message = {"function_message": msg}
 
         # add extra metadata
         if msg_obj is not None:
             new_message["id"] = str(msg_obj.id)
+            assert is_utc_datetime(msg_obj.created_at), msg_obj.created_at
             new_message["date"] = msg_obj.created_at.isoformat()
 
         self.buffer.put(new_message)
```

### Comparing `pymemgpt-0.3.7/memgpt/server/rest_api/models/index.py` & `pymemgpt-0.3.8/memgpt/server/rest_api/models/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/server/rest_api/openai_assistants/assistants.py` & `pymemgpt-0.3.8/memgpt/server/rest_api/openai_assistants/assistants.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     Text,
     ImageFile,
     ToolCall,
     ToolCallOutput,
 )
 from memgpt.data_types import LLMConfig, EmbeddingConfig, Message
 from memgpt.constants import DEFAULT_PRESET
+from memgpt.utils import get_utc_time
 
 router = APIRouter()
 
 
 class CreateAssistantRequest(BaseModel):
     model: str = Field(..., description="The model to use for the assistant.")
     name: str = Field(..., description="The name of the assistant.")
@@ -156,15 +157,15 @@
     @router.post("/assistants", tags=["assistants"], response_model=OpenAIAssistant)
     def create_assistant(request: CreateAssistantRequest = Body(...)):
         # TODO: create preset
         return OpenAIAssistant(
             id=DEFAULT_PRESET,
             name="default_preset",
             description=request.description,
-            created_at=int(datetime.now().timestamp()),
+            created_at=int(get_utc_time().timestamp()),
             model=request.model,
             instructions=request.instructions,
             tools=request.tools,
             file_ids=request.file_ids,
             metadata=request.metadata,
         )
 
@@ -172,15 +173,15 @@
     def create_assistant_file(
         assistant_id: str = Path(..., description="The unique identifier of the assistant."),
         request: CreateAssistantFileRequest = Body(...),
     ):
         # TODO: add file to assistant
         return AssistantFile(
             id=request.file_id,
-            created_at=int(datetime.now().timestamp()),
+            created_at=int(get_utc_time().timestamp()),
             assistant_id=assistant_id,
         )
 
     @router.get("/assistants", tags=["assistants"], response_model=List[OpenAIAssistant])
     def list_assistants(
         limit: int = Query(1000, description="How many assistants to retrieve."),
         order: str = Query("asc", description="Order of assistants to retrieve (either 'asc' or 'desc')."),
@@ -407,15 +408,15 @@
     ):
         # TODO: add request.instructions as a message?
         agent_id = uuid.UUID(thread_id)
         # TODO: override preset of agent with request.assistant_id
         agent = server._get_or_load_agent(user_id=user_id, agent_id=agent_id)
         agent.step(user_message=None)  # already has messages added
         run_id = str(uuid.uuid4())
-        create_time = int(datetime.now().timestamp())
+        create_time = int(get_utc_time().timestamp())
         return OpenAIRun(
             id=run_id,
             created_at=create_time,
             thread_id=str(agent_id),
             assistant_id=DEFAULT_PRESET,  # TODO: update this
             status="completed",  # TODO: eventaully allow offline execution
             expires_at=create_time,
```

### Comparing `pymemgpt-0.3.7/memgpt/server/rest_api/personas/index.py` & `pymemgpt-0.3.8/memgpt/server/rest_api/personas/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/server/rest_api/presets/index.py` & `pymemgpt-0.3.8/memgpt/server/rest_api/presets/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 class CreatePresetsRequest(BaseModel):
     # TODO is there a cleaner way to create the request from the PresetModel (need to drop fields though)?
     name: str = Field(..., description="The name of the preset.")
     id: Optional[Union[uuid.UUID, str]] = Field(default_factory=uuid.uuid4, description="The unique identifier of the preset.")
     # user_id: uuid.UUID = Field(..., description="The unique identifier of the user who created the preset.")
     description: Optional[str] = Field(None, description="The description of the preset.")
-    # created_at: datetime = Field(default_factory=datetime.now, description="The unix timestamp of when the preset was created.")
+    # created_at: datetime = Field(default_factory=get_utc_time, description="The unix timestamp of when the preset was created.")
     system: str = Field(..., description="The system prompt of the preset.")
     persona: str = Field(default=get_persona_text(DEFAULT_PERSONA), description="The persona of the preset.")
     human: str = Field(default=get_human_text(DEFAULT_HUMAN), description="The human of the preset.")
     functions_schema: List[Dict] = Field(..., description="The functions schema of the preset.")
     # TODO
     persona_name: Optional[str] = Field(None, description="The name of the persona of the preset.")
     human_name: Optional[str] = Field(None, description="The name of the human of the preset.")
```

### Comparing `pymemgpt-0.3.7/memgpt/server/rest_api/server.py` & `pymemgpt-0.3.8/memgpt/server/rest_api/server.py`

 * *Files 15% similar despite different names*

```diff
@@ -34,14 +34,24 @@
 """
 Basic REST API sitting on top of the internal MemGPT python server (SyncServer)
 
 Start the server with:
   cd memgpt/server/rest_api
   poetry run uvicorn server:app --reload
 """
+# override config with postgres enviornment (messy, but necessary for docker compose)
+# TODO: do something less gross
+if os.getenv("POSTGRES_URI"):
+    config = MemGPTConfig.load()
+    config.archival_storage_uri = os.getenv("POSTGRES_URI")
+    config.recall_storage_uri = os.getenv("POSTGRES_URI")
+    config.metadata_storage_uri = os.getenv("POSTGRES_URI")
+    print(f"Overriding DB config URI with enviornment variable: {config.archival_storage_uri}")
+    config.save()
+
 
 interface: QueuingInterface = QueuingInterface()
 server: SyncServer = SyncServer(default_interface=interface)
 
 
 SERVER_PASS_VAR = "MEMGPT_SERVER_PASS"
 password = os.getenv(SERVER_PASS_VAR)
@@ -50,14 +60,15 @@
     # if the pass was specified in the environment, use it
     print(f"Using existing admin server password from environment.")
 else:
     # Autogenerate a password for this session and dump it to stdout
     password = secrets.token_urlsafe(16)
     print(f"Generated admin server password for this session: {password}")
 
+
 security = HTTPBearer()
 
 
 def verify_password(credentials: HTTPAuthorizationCredentials = Depends(security)):
     """REST requests going to /admin are protected with a bearer token (that must match the password)"""
     if credentials.credentials != password:
         raise HTTPException(status_code=401, detail="Unauthorized")
@@ -214,24 +225,24 @@
             ssl_certfile, ssl_keyfile = ssl_cert, ssl_key  # Assuming cert includes both
             print(f"Running server with provided SSL cert: {ssl_certfile}, {ssl_keyfile}")
 
         # This will start the server on HTTPS
         assert isinstance(ssl_certfile, str) and os.path.exists(ssl_certfile), ssl_certfile
         assert isinstance(ssl_keyfile, str) and os.path.exists(ssl_keyfile), ssl_keyfile
         print(
-            f"Running: uvicorn {app}:app --host {host or 'localhost'} --port {port or REST_DEFAULT_PORT} --ssl-keyfile {ssl_keyfile} --ssl-certfile {ssl_certfile}"
+            f"Running: uvicorn server:app --host {host or 'localhost'} --port {port or REST_DEFAULT_PORT} --ssl-keyfile {ssl_keyfile} --ssl-certfile {ssl_certfile}"
         )
         uvicorn.run(
             app,
             host=host or "localhost",
             port=port or REST_DEFAULT_PORT,
             ssl_keyfile=ssl_keyfile,
             ssl_certfile=ssl_certfile,
         )
     else:
         # Start the subprocess in a new session
-        print(f"Running: uvicorn {app}:app --host {host or 'localhost'} --port {port or REST_DEFAULT_PORT}")
+        print(f"Running: uvicorn server:app --host {host or 'localhost'} --port {port or REST_DEFAULT_PORT}")
         uvicorn.run(
             app,
             host=host or "localhost",
             port=port or REST_DEFAULT_PORT,
         )
```

### Comparing `pymemgpt-0.3.7/memgpt/server/rest_api/sources/index.py` & `pymemgpt-0.3.8/memgpt/server/rest_api/sources/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,18 +35,14 @@
 
 
 class CreateSourceRequest(BaseModel):
     name: str = Field(..., description="The name of the source.")
     description: Optional[str] = Field(None, description="The description of the source.")
 
 
-class CreateSourceResponse(BaseModel):
-    source: SourceModel = Field(..., description="The newly created source.")
-
-
 class UploadFileToSourceRequest(BaseModel):
     file: UploadFile = Field(..., description="The file to upload.")
 
 
 class UploadFileToSourceResponse(BaseModel):
     source: SourceModel = Field(..., description="The source the file was uploaded to.")
     added_passages: int = Field(..., description="The number of passages added to the source.")
@@ -124,15 +120,16 @@
         agent_id: uuid.UUID = Query(..., description="The unique identifier of the agent to attach the source to."),
         user_id: uuid.UUID = Depends(get_current_user_with_server),
     ):
         """Attach a data source to an existing agent."""
         interface.clear()
         assert isinstance(agent_id, uuid.UUID), f"Expected agent_id to be a UUID, got {agent_id}"
         assert isinstance(user_id, uuid.UUID), f"Expected user_id to be a UUID, got {user_id}"
-        source = server.attach_source_to_agent(source_id=source_id, agent_id=agent_id, user_id=user_id)
+        source = server.ms.get_source(source_id=source_id, user_id=user_id)
+        source = server.attach_source_to_agent(source_name=source.name, agent_id=agent_id, user_id=user_id)
         return SourceModel(
             name=source.name,
             description=None,  # TODO: actually store descriptions
             user_id=source.user_id,
             id=source.id,
             embedding_config=server.server_embedding_config,
             created_at=source.created_at,
```

### Comparing `pymemgpt-0.3.7/memgpt/server/rest_api/static_files.py` & `pymemgpt-0.3.8/memgpt/server/rest_api/static_files.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/server/rest_api/tools/index.py` & `pymemgpt-0.3.8/memgpt/server/rest_api/tools/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/server/server.py` & `pymemgpt-0.3.8/memgpt/server/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,15 +236,16 @@
             # azure_version=self.credentials.azure_version,
             # azure_deployment=self.credentials.azure_deployment,
         )
         self.server_embedding_config = EmbeddingConfig(
             embedding_endpoint_type=self.config.default_embedding_config.embedding_endpoint_type,
             embedding_endpoint=self.config.default_embedding_config.embedding_endpoint,
             embedding_dim=self.config.default_embedding_config.embedding_dim,
-            # openai_key=self.credentials.openai_key,
+            embedding_model=self.config.default_embedding_config.embedding_model,
+            embedding_chunk_size=self.config.default_embedding_config.embedding_chunk_size,
         )
 
         # Initialize the metadata store
         self.ms = MetadataStore(self.config)
 
         # NOTE: removed, since server should be multi-user
         ## Create the default user
@@ -1060,15 +1061,15 @@
         agent_id: uuid.UUID,
         after: Optional[uuid.UUID] = None,
         before: Optional[uuid.UUID] = None,
         limit: Optional[int] = 100,
         order_by: Optional[str] = "created_at",
         order: Optional[str] = "asc",
         reverse: Optional[bool] = False,
-    ):
+    ) -> Tuple[uuid.UUID, List[dict]]:
         if self.ms.get_user(user_id=user_id) is None:
             raise ValueError(f"User user_id={user_id} does not exist")
         if self.ms.get_agent(agent_id=agent_id, user_id=user_id) is None:
             raise ValueError(f"Agent agent_id={agent_id} does not exist")
 
         # Get the agent object (loaded in memory)
         memgpt_agent = self._get_or_load_agent(user_id=user_id, agent_id=agent_id)
@@ -1356,29 +1357,42 @@
             for source in sources
         ]
 
         # Add extra metadata to the sources
         sources_with_metadata = []
         for source in sources:
 
-            passages = self.list_data_source_passages(user_id=user_id, source_id=source.id)
-            documents = self.list_data_source_documents(user_id=user_id, source_id=source.id)
+            # count number of passages
+            passage_conn = StorageConnector.get_storage_connector(TableType.PASSAGES, self.config, user_id=user_id)
+            num_passages = passage_conn.size({"data_source": source.name})
+            print(passage_conn.get_all())
+            print(
+                "NUMBER PASSAGES",
+                num_passages,
+            )
+
+            # TODO: add when documents table implemented
+            ## count number of documents
+            # document_conn = StorageConnector.get_storage_connector(TableType.DOCUMENTS, self.config, user_id=user_id)
+            # num_documents = document_conn.size({"data_source": source.name})
+            num_documents = 0
+
             agent_ids = self.ms.list_attached_agents(source_id=source.id)
             # add the agent name information
             attached_agents = [
                 {
                     "id": str(a_id),
                     "name": self.ms.get_agent(user_id=user_id, agent_id=a_id).name,
                 }
                 for a_id in agent_ids
             ]
 
             # Overwrite metadata field, should be empty anyways
             source.metadata_ = dict(
-                num_documents=len(passages),
-                num_passages=len(documents),
+                num_documents=num_documents,
+                num_passages=num_passages,
                 attached_agents=attached_agents,
             )
 
             sources_with_metadata.append(source)
 
         return sources_with_metadata
```

### Comparing `pymemgpt-0.3.7/memgpt/server/static_files/assets/index-57df4f6c.css` & `pymemgpt-0.3.8/memgpt/server/static_files/assets/index-57df4f6c.css`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/server/static_files/assets/index-f6a3d52a.js` & `pymemgpt-0.3.8/memgpt/server/static_files/assets/index-f6a3d52a.js`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/server/static_files/favicon.ico` & `pymemgpt-0.3.8/memgpt/server/static_files/favicon.ico`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/server/static_files/index.html` & `pymemgpt-0.3.8/memgpt/server/static_files/index.html`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/server/static_files/memgpt_logo_transparent.png` & `pymemgpt-0.3.8/memgpt/server/static_files/memgpt_logo_transparent.png`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/server/utils.py` & `pymemgpt-0.3.8/memgpt/server/utils.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/server/ws_api/example_client.py` & `pymemgpt-0.3.8/memgpt/server/ws_api/example_client.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/server/ws_api/interface.py` & `pymemgpt-0.3.8/memgpt/server/ws_api/interface.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/server/ws_api/protocol.py` & `pymemgpt-0.3.8/memgpt/server/ws_api/protocol.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/server/ws_api/server.py` & `pymemgpt-0.3.8/memgpt/server/ws_api/server.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/system.py` & `pymemgpt-0.3.8/memgpt/system.py`

 * *Files identical despite different names*

### Comparing `pymemgpt-0.3.7/memgpt/utils.py` & `pymemgpt-0.3.8/memgpt/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from datetime import datetime
+from datetime import datetime, timezone, timedelta
 import copy
 import re
 import json
 import os
 import pickle
 import platform
 import random
@@ -465,14 +465,18 @@
     "walrus",
     "xylophone",
     "yak",
     "zebra",
 ]
 
 
+def is_utc_datetime(dt: datetime) -> bool:
+    return dt.tzinfo is not None and dt.tzinfo.utcoffset(dt) == timedelta(0)
+
+
 def get_tool_call_id() -> str:
     return str(uuid.uuid4())[:TOOL_CALL_ID_MAX_LEN]
 
 
 def assistant_function_to_tool(assistant_message: dict) -> dict:
     assert "function_call" in assistant_message
     new_msg = copy.deepcopy(assistant_message)
@@ -835,15 +839,17 @@
         # You may format it as you desire, including AM/PM
         time_str = local_time.strftime("%Y-%m-%d %I:%M:%S %p %Z%z")
 
     return time_str.strip()
 
 
 def get_utc_time() -> datetime:
-    return datetime.now(pytz.utc)
+    """Get the current UTC time"""
+    # return datetime.now(pytz.utc)
+    return datetime.now(timezone.utc)
 
 
 def format_datetime(dt):
     return dt.strftime("%Y-%m-%d %I:%M:%S %p %Z%z")
 
 
 def parse_json(string) -> dict:
```

### Comparing `pymemgpt-0.3.7/pyproject.toml` & `pymemgpt-0.3.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymemgpt"
-version = "0.3.7"
+version = "0.3.8"
 packages = [
     {include = "memgpt"}
 ]
 description = "Teaching LLMs memory management for unbounded context"
 authors = [
     "MemGPT Team <hi@memgpt.ai>",
 ]
```

### Comparing `pymemgpt-0.3.7/PKG-INFO` & `pymemgpt-0.3.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymemgpt
-Version: 0.3.7
+Version: 0.3.8
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
-Metadata-Version: 2.1 Name: pymemgpt Version: 0.3.7 Summary: Teaching LLMs
+Metadata-Version: 2.1 Name: pymemgpt Version: 0.3.8 Summary: Teaching LLMs
 memory management for unbounded context License: Apache License Author: MemGPT
 Team Author-email: hi@memgpt.ai Requires-Python: >=3.10,<3.12 Classifier:
 License :: Other/Proprietary License Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Provides-Extra: autogen Provides-Extra: dev
 Provides-Extra: local Provides-Extra: postgres Provides-Extra: server Requires-
 Dist: autoflake (>=2.3.0,<3.0.0) ; extra == "dev" Requires-Dist: black[jupyter]
@@ -127,10 +127,12 @@
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

