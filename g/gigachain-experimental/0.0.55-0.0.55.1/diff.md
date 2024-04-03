# Comparing `tmp/gigachain_experimental-0.0.55.tar.gz` & `tmp/gigachain_experimental-0.0.55.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gigachain_experimental-0.0.55.tar", max compression
+gzip compressed data, was "gigachain_experimental-0.0.55.1.tar", max compression
```

## Comparing `gigachain_experimental-0.0.55.tar` & `gigachain_experimental-0.0.55.1.tar`

### file list

```diff
@@ -1,150 +1,150 @@
--rw-r--r--   0        0        0     1067 2024-03-14 13:23:46.793403 gigachain_experimental-0.0.55/LICENSE
--rw-r--r--   0        0        0      731 2023-10-06 15:21:09.714881 gigachain_experimental-0.0.55/README.md
--rw-r--r--   0        0        0      271 2024-03-14 13:23:46.793978 gigachain_experimental-0.0.55/langchain_experimental/__init__.py
--rw-r--r--   0        0        0      643 2024-03-27 08:44:31.265425 gigachain_experimental-0.0.55/langchain_experimental/agents/__init__.py
--rw-r--r--   0        0        0      653 2024-03-14 13:23:46.794474 gigachain_experimental-0.0.55/langchain_experimental/agents/agent_toolkits/__init__.py
--rw-r--r--   0        0        0       19 2024-03-14 13:23:46.794818 gigachain_experimental-0.0.55/langchain_experimental/agents/agent_toolkits/csv/__init__.py
--rw-r--r--   0        0        0     2407 2024-03-14 13:23:46.795018 gigachain_experimental-0.0.55/langchain_experimental/agents/agent_toolkits/csv/base.py
--rw-r--r--   0        0        0       22 2024-03-14 13:23:46.795255 gigachain_experimental-0.0.55/langchain_experimental/agents/agent_toolkits/pandas/__init__.py
--rw-r--r--   0        0        0    11290 2024-03-19 08:17:14.889373 gigachain_experimental-0.0.55/langchain_experimental/agents/agent_toolkits/pandas/base.py
--rw-r--r--   0        0        0     1113 2024-03-14 13:23:46.795892 gigachain_experimental-0.0.55/langchain_experimental/agents/agent_toolkits/pandas/prompt.py
--rw-r--r--   0        0        0        0 2024-03-14 13:23:46.796139 gigachain_experimental-0.0.55/langchain_experimental/agents/agent_toolkits/python/__init__.py
--rw-r--r--   0        0        0     2224 2024-03-14 13:23:46.796434 gigachain_experimental-0.0.55/langchain_experimental/agents/agent_toolkits/python/base.py
--rw-r--r--   0        0        0      513 2024-03-14 13:23:46.796678 gigachain_experimental-0.0.55/langchain_experimental/agents/agent_toolkits/python/prompt.py
--rw-r--r--   0        0        0       20 2024-03-14 13:23:46.797026 gigachain_experimental-0.0.55/langchain_experimental/agents/agent_toolkits/spark/__init__.py
--rw-r--r--   0        0        0     2761 2024-03-14 13:23:46.797378 gigachain_experimental-0.0.55/langchain_experimental/agents/agent_toolkits/spark/base.py
--rw-r--r--   0        0        0      295 2024-03-14 13:23:46.797631 gigachain_experimental-0.0.55/langchain_experimental/agents/agent_toolkits/spark/prompt.py
--rw-r--r--   0        0        0       23 2024-03-14 13:23:46.797989 gigachain_experimental-0.0.55/langchain_experimental/agents/agent_toolkits/xorbits/__init__.py
--rw-r--r--   0        0        0     3143 2024-03-14 13:23:46.798282 gigachain_experimental-0.0.55/langchain_experimental/agents/agent_toolkits/xorbits/base.py
--rw-r--r--   0        0        0     1070 2024-03-14 13:23:46.798536 gigachain_experimental-0.0.55/langchain_experimental/agents/agent_toolkits/xorbits/prompt.py
--rw-r--r--   0        0        0      866 2024-03-27 08:44:31.266754 gigachain_experimental-0.0.55/langchain_experimental/autonomous_agents/__init__.py
--rw-r--r--   0        0        0        0 2023-09-14 13:23:58.140059 gigachain_experimental-0.0.55/langchain_experimental/autonomous_agents/autogpt/__init__.py
--rw-r--r--   0        0        0     5443 2024-03-14 13:23:46.799095 gigachain_experimental-0.0.55/langchain_experimental/autonomous_agents/autogpt/agent.py
--rw-r--r--   0        0        0     1164 2024-03-14 13:23:46.799560 gigachain_experimental-0.0.55/langchain_experimental/autonomous_agents/autogpt/memory.py
--rw-r--r--   0        0        0     1909 2024-03-14 13:23:46.799976 gigachain_experimental-0.0.55/langchain_experimental/autonomous_agents/autogpt/output_parser.py
--rw-r--r--   0        0        0     5000 2024-03-14 13:23:46.800435 gigachain_experimental-0.0.55/langchain_experimental/autonomous_agents/autogpt/prompt.py
--rw-r--r--   0        0        0     7963 2024-03-14 13:23:46.800907 gigachain_experimental-0.0.55/langchain_experimental/autonomous_agents/autogpt/prompt_generator.py
--rw-r--r--   0        0        0      514 2023-09-14 13:23:58.140895 gigachain_experimental-0.0.55/langchain_experimental/autonomous_agents/baby_agi/__init__.py
--rw-r--r--   0        0        0     8687 2024-03-14 13:23:46.801553 gigachain_experimental-0.0.55/langchain_experimental/autonomous_agents/baby_agi/baby_agi.py
--rw-r--r--   0        0        0     1668 2024-03-27 08:44:31.690254 gigachain_experimental-0.0.55/langchain_experimental/autonomous_agents/baby_agi/task_creation.py
--rw-r--r--   0        0        0      967 2024-03-27 08:44:31.689200 gigachain_experimental-0.0.55/langchain_experimental/autonomous_agents/baby_agi/task_execution.py
--rw-r--r--   0        0        0     1283 2024-03-27 08:44:31.688019 gigachain_experimental-0.0.55/langchain_experimental/autonomous_agents/baby_agi/task_prioritization.py
--rw-r--r--   0        0        0        0 2023-09-14 13:23:58.141519 gigachain_experimental-0.0.55/langchain_experimental/autonomous_agents/hugginggpt/__init__.py
--rw-r--r--   0        0        0     1133 2024-03-14 13:23:46.803494 gigachain_experimental-0.0.55/langchain_experimental/autonomous_agents/hugginggpt/hugginggpt.py
--rw-r--r--   0        0        0     1742 2024-03-27 08:44:31.687010 gigachain_experimental-0.0.55/langchain_experimental/autonomous_agents/hugginggpt/repsonse_generator.py
--rw-r--r--   0        0        0     4598 2024-03-14 13:23:46.804390 gigachain_experimental-0.0.55/langchain_experimental/autonomous_agents/hugginggpt/task_executor.py
--rw-r--r--   0        0        0     7859 2024-03-14 13:23:46.804893 gigachain_experimental-0.0.55/langchain_experimental/autonomous_agents/hugginggpt/task_planner.py
--rw-r--r--   0        0        0      674 2024-03-19 08:17:14.889676 gigachain_experimental-0.0.55/langchain_experimental/chat_models/__init__.py
--rw-r--r--   0        0        0     6063 2024-03-19 08:17:14.889885 gigachain_experimental-0.0.55/langchain_experimental/chat_models/llm_wrapper.py
--rw-r--r--   0        0        0     2190 2024-03-27 08:44:31.267084 gigachain_experimental-0.0.55/langchain_experimental/comprehend_moderation/__init__.py
--rw-r--r--   0        0        0     6659 2024-03-14 13:23:46.807228 gigachain_experimental-0.0.55/langchain_experimental/comprehend_moderation/amazon_comprehend_moderation.py
--rw-r--r--   0        0        0     7411 2024-03-14 13:23:46.807736 gigachain_experimental-0.0.55/langchain_experimental/comprehend_moderation/base_moderation.py
--rw-r--r--   0        0        0     2390 2024-03-14 13:23:46.808072 gigachain_experimental-0.0.55/langchain_experimental/comprehend_moderation/base_moderation_callbacks.py
--rw-r--r--   0        0        0     1614 2024-03-14 13:23:46.808388 gigachain_experimental-0.0.55/langchain_experimental/comprehend_moderation/base_moderation_config.py
--rw-r--r--   0        0        0      192 2023-09-14 13:23:58.142645 gigachain_experimental-0.0.55/langchain_experimental/comprehend_moderation/base_moderation_enums.py
--rw-r--r--   0        0        0     1054 2024-03-14 13:23:46.808784 gigachain_experimental-0.0.55/langchain_experimental/comprehend_moderation/base_moderation_exceptions.py
--rw-r--r--   0        0        0     6834 2024-03-14 13:23:46.809097 gigachain_experimental-0.0.55/langchain_experimental/comprehend_moderation/pii.py
--rw-r--r--   0        0        0     3142 2024-03-14 13:23:46.809305 gigachain_experimental-0.0.55/langchain_experimental/comprehend_moderation/prompt_safety.py
--rw-r--r--   0        0        0     8134 2024-03-14 13:23:46.809624 gigachain_experimental-0.0.55/langchain_experimental/comprehend_moderation/toxicity.py
--rw-r--r--   0        0        0      103 2023-10-03 14:29:06.367456 gigachain_experimental-0.0.55/langchain_experimental/cpal/README.md
--rw-r--r--   0        0        0      750 2024-03-27 08:44:31.267314 gigachain_experimental-0.0.55/langchain_experimental/cpal/__init__.py
--rw-r--r--   0        0        0    11087 2024-03-14 13:23:46.809990 gigachain_experimental-0.0.55/langchain_experimental/cpal/base.py
--rw-r--r--   0        0        0      246 2023-09-14 13:23:58.143626 gigachain_experimental-0.0.55/langchain_experimental/cpal/constants.py
--rw-r--r--   0        0        0     9183 2024-03-14 13:23:46.810525 gigachain_experimental-0.0.55/langchain_experimental/cpal/models.py
--rw-r--r--   0        0        0        0 2023-09-14 13:23:58.143845 gigachain_experimental-0.0.55/langchain_experimental/cpal/templates/__init__.py
--rw-r--r--   0        0        0        0 2023-09-14 13:23:58.144036 gigachain_experimental-0.0.55/langchain_experimental/cpal/templates/univariate/__init__.py
--rw-r--r--   0        0        0     2548 2024-03-14 13:23:46.811061 gigachain_experimental-0.0.55/langchain_experimental/cpal/templates/univariate/causal.py
--rw-r--r--   0        0        0      853 2024-03-14 13:23:46.811497 gigachain_experimental-0.0.55/langchain_experimental/cpal/templates/univariate/intervention.py
--rw-r--r--   0        0        0     2905 2024-03-14 13:23:46.811993 gigachain_experimental-0.0.55/langchain_experimental/cpal/templates/univariate/narrative.py
--rw-r--r--   0        0        0     5468 2024-03-14 13:23:46.812441 gigachain_experimental-0.0.55/langchain_experimental/cpal/templates/univariate/query.py
--rw-r--r--   0        0        0      631 2024-03-27 08:44:31.267678 gigachain_experimental-0.0.55/langchain_experimental/data_anonymizer/__init__.py
--rw-r--r--   0        0        0     1811 2024-03-14 13:23:46.813062 gigachain_experimental-0.0.55/langchain_experimental/data_anonymizer/base.py
--rw-r--r--   0        0        0     4793 2024-03-14 13:23:46.813631 gigachain_experimental-0.0.55/langchain_experimental/data_anonymizer/deanonymizer_mapping.py
--rw-r--r--   0        0        0     6801 2024-03-14 13:23:46.814004 gigachain_experimental-0.0.55/langchain_experimental/data_anonymizer/deanonymizer_matching_strategies.py
--rw-r--r--   0        0        0     2861 2024-03-14 13:23:46.814331 gigachain_experimental-0.0.55/langchain_experimental/data_anonymizer/faker_presidio_mapping.py
--rw-r--r--   0        0        0    17162 2024-03-14 13:23:46.814652 gigachain_experimental-0.0.55/langchain_experimental/data_anonymizer/presidio.py
--rw-r--r--   0        0        0      368 2024-03-27 08:44:31.685930 gigachain_experimental-0.0.55/langchain_experimental/fallacy_removal/__init__.py
--rw-r--r--   0        0        0      263 2024-03-27 08:44:31.268238 gigachain_experimental-0.0.55/langchain_experimental/generative_agents/__init__.py
--rw-r--r--   0        0        0    10252 2024-03-27 08:44:31.268950 gigachain_experimental-0.0.55/langchain_experimental/generative_agents/generative_agent.py
--rw-r--r--   0        0        0    13413 2024-03-27 08:44:31.685356 gigachain_experimental-0.0.55/langchain_experimental/generative_agents/memory.py
--rw-r--r--   0        0        0      308 2024-03-27 08:44:31.269247 gigachain_experimental-0.0.55/langchain_experimental/graph_transformers/__init__.py
--rw-r--r--   0        0        0    10723 2024-03-19 08:17:14.890843 gigachain_experimental-0.0.55/langchain_experimental/graph_transformers/diffbot.py
--rw-r--r--   0        0        0    12290 2024-03-27 08:44:31.269530 gigachain_experimental-0.0.55/langchain_experimental/graph_transformers/llm.py
--rw-r--r--   0        0        0       94 2024-03-27 08:44:31.270890 gigachain_experimental-0.0.55/langchain_experimental/llm_bash/__init__.py
--rw-r--r--   0        0        0     4454 2024-03-14 13:23:46.816866 gigachain_experimental-0.0.55/langchain_experimental/llm_bash/base.py
--rw-r--r--   0        0        0     5708 2024-03-14 13:23:46.817282 gigachain_experimental-0.0.55/langchain_experimental/llm_bash/bash.py
--rw-r--r--   0        0        0     2038 2024-03-14 13:23:46.817632 gigachain_experimental-0.0.55/langchain_experimental/llm_bash/prompt.py
--rw-r--r--   0        0        0      164 2024-03-27 08:44:31.271978 gigachain_experimental-0.0.55/langchain_experimental/llm_symbolic_math/__init__.py
--rw-r--r--   0        0        0     5791 2024-03-14 13:23:46.818120 gigachain_experimental-0.0.55/langchain_experimental/llm_symbolic_math/base.py
--rw-r--r--   0        0        0     1087 2023-10-06 15:21:09.721677 gigachain_experimental-0.0.55/langchain_experimental/llm_symbolic_math/prompt.py
--rw-r--r--   0        0        0      453 2024-03-27 08:44:31.272308 gigachain_experimental-0.0.55/langchain_experimental/llms/__init__.py
--rw-r--r--   0        0        0     8768 2024-03-19 08:17:14.891239 gigachain_experimental-0.0.55/langchain_experimental/llms/anthropic_functions.py
--rw-r--r--   0        0        0     2228 2024-03-14 13:23:46.820107 gigachain_experimental-0.0.55/langchain_experimental/llms/jsonformer_decoder.py
--rw-r--r--   0        0        0     4344 2024-03-14 13:23:46.820880 gigachain_experimental-0.0.55/langchain_experimental/llms/llamaapi.py
--rw-r--r--   0        0        0     2843 2024-03-14 13:23:46.821460 gigachain_experimental-0.0.55/langchain_experimental/llms/lmformatenforcer_decoder.py
--rw-r--r--   0        0        0     4932 2024-03-14 13:23:46.821957 gigachain_experimental-0.0.55/langchain_experimental/llms/ollama_functions.py
--rw-r--r--   0        0        0     2342 2024-03-14 13:23:46.822538 gigachain_experimental-0.0.55/langchain_experimental/llms/rellm_decoder.py
--rw-r--r--   0        0        0      346 2024-03-27 08:44:31.272547 gigachain_experimental-0.0.55/langchain_experimental/open_clip/__init__.py
--rw-r--r--   0        0        0     3383 2024-03-14 13:23:46.823943 gigachain_experimental-0.0.55/langchain_experimental/open_clip/open_clip.py
--rw-r--r--   0        0        0      120 2024-03-14 13:23:46.824923 gigachain_experimental-0.0.55/langchain_experimental/openai_assistant/__init__.py
--rw-r--r--   0        0        0      185 2024-03-14 13:23:46.825679 gigachain_experimental-0.0.55/langchain_experimental/openai_assistant/base.py
--rw-r--r--   0        0        0      330 2024-03-27 08:44:31.272811 gigachain_experimental-0.0.55/langchain_experimental/pal_chain/__init__.py
--rw-r--r--   0        0        0    13320 2024-03-14 13:23:46.826384 gigachain_experimental-0.0.55/langchain_experimental/pal_chain/base.py
--rw-r--r--   0        0        0     3537 2023-09-14 13:23:58.147176 gigachain_experimental-0.0.55/langchain_experimental/pal_chain/colored_object_prompt.py
--rw-r--r--   0        0        0     5767 2023-09-14 13:23:58.147272 gigachain_experimental-0.0.55/langchain_experimental/pal_chain/math_prompt.py
--rw-r--r--   0        0        0      488 2024-03-27 08:44:31.273070 gigachain_experimental-0.0.55/langchain_experimental/plan_and_execute/__init__.py
--rw-r--r--   0        0        0     3570 2023-09-14 13:23:58.147536 gigachain_experimental-0.0.55/langchain_experimental/plan_and_execute/agent_executor.py
--rw-r--r--   0        0        0        0 2023-09-14 13:23:58.147634 gigachain_experimental-0.0.55/langchain_experimental/plan_and_execute/executors/__init__.py
--rw-r--r--   0        0        0     1463 2024-03-14 13:23:46.826994 gigachain_experimental-0.0.55/langchain_experimental/plan_and_execute/executors/agent_executor.py
--rw-r--r--   0        0        0     1269 2023-09-14 13:23:58.147861 gigachain_experimental-0.0.55/langchain_experimental/plan_and_execute/executors/base.py
--rw-r--r--   0        0        0        0 2023-09-14 13:23:58.147962 gigachain_experimental-0.0.55/langchain_experimental/plan_and_execute/planners/__init__.py
--rw-r--r--   0        0        0     1567 2023-09-14 13:23:58.148116 gigachain_experimental-0.0.55/langchain_experimental/plan_and_execute/planners/base.py
--rw-r--r--   0        0        0     2314 2024-03-14 13:23:46.827423 gigachain_experimental-0.0.55/langchain_experimental/plan_and_execute/planners/chat_planner.py
--rw-r--r--   0        0        0     1439 2024-03-14 13:23:46.827784 gigachain_experimental-0.0.55/langchain_experimental/plan_and_execute/schema.py
--rw-r--r--   0        0        0      369 2024-03-27 08:44:31.273303 gigachain_experimental-0.0.55/langchain_experimental/prompt_injection_identifier/__init__.py
--rw-r--r--   0        0        0     3369 2024-03-27 08:44:31.273541 gigachain_experimental-0.0.55/langchain_experimental/prompt_injection_identifier/hugging_face_identifier.py
--rw-r--r--   0        0        0      174 2024-03-27 08:44:31.273777 gigachain_experimental-0.0.55/langchain_experimental/prompts/__init__.py
--rw-r--r--   0        0        0     1942 2024-03-14 13:23:46.828890 gigachain_experimental-0.0.55/langchain_experimental/prompts/load.py
--rw-r--r--   0        0        0        0 2023-09-14 13:23:58.148908 gigachain_experimental-0.0.55/langchain_experimental/py.typed
--rw-r--r--   0        0        0     1285 2023-09-14 13:23:58.149124 gigachain_experimental-0.0.55/langchain_experimental/pydantic_v1/__init__.py
--rw-r--r--   0        0        0      548 2023-09-14 13:23:58.149226 gigachain_experimental-0.0.55/langchain_experimental/pydantic_v1/dataclasses.py
--rw-r--r--   0        0        0      520 2023-09-14 13:23:58.149317 gigachain_experimental-0.0.55/langchain_experimental/pydantic_v1/main.py
--rw-r--r--   0        0        0      518 2024-03-27 08:44:31.274033 gigachain_experimental-0.0.55/langchain_experimental/recommenders/__init__.py
--rw-r--r--   0        0        0     7967 2024-03-27 08:44:31.274351 gigachain_experimental-0.0.55/langchain_experimental/recommenders/amazon_personalize.py
--rw-r--r--   0        0        0     6964 2024-03-14 13:23:46.829648 gigachain_experimental-0.0.55/langchain_experimental/recommenders/amazon_personalize_chain.py
--rw-r--r--   0        0        0      200 2024-03-27 08:44:31.274579 gigachain_experimental-0.0.55/langchain_experimental/retrievers/__init__.py
--rw-r--r--   0        0        0     1248 2024-03-14 13:23:46.830070 gigachain_experimental-0.0.55/langchain_experimental/retrievers/vector_sql_database.py
--rw-r--r--   0        0        0     1447 2024-03-27 08:44:31.274825 gigachain_experimental-0.0.55/langchain_experimental/rl_chain/__init__.py
--rw-r--r--   0        0        0    23241 2024-03-14 13:23:46.830706 gigachain_experimental-0.0.55/langchain_experimental/rl_chain/base.py
--rw-r--r--   0        0        0     1989 2024-03-14 13:23:46.831066 gigachain_experimental-0.0.55/langchain_experimental/rl_chain/metrics.py
--rw-r--r--   0        0        0     2126 2024-03-14 13:23:46.831366 gigachain_experimental-0.0.55/langchain_experimental/rl_chain/model_repository.py
--rw-r--r--   0        0        0    16279 2024-03-14 13:23:46.831741 gigachain_experimental-0.0.55/langchain_experimental/rl_chain/pick_best_chain.py
--rw-r--r--   0        0        0      556 2024-03-14 13:23:46.832050 gigachain_experimental-0.0.55/langchain_experimental/rl_chain/vw_logger.py
--rw-r--r--   0        0        0      946 2024-03-27 08:44:31.275078 gigachain_experimental-0.0.55/langchain_experimental/smart_llm/__init__.py
--rw-r--r--   0        0        0    14423 2024-03-14 13:23:46.832807 gigachain_experimental-0.0.55/langchain_experimental/smart_llm/base.py
--rw-r--r--   0        0        0      202 2024-03-27 08:47:25.600968 gigachain_experimental-0.0.55/langchain_experimental/sql/__init__.py
--rw-r--r--   0        0        0    13112 2024-03-14 13:23:46.833225 gigachain_experimental-0.0.55/langchain_experimental/sql/base.py
--rw-r--r--   0        0        0     4658 2023-09-25 11:47:07.505993 gigachain_experimental-0.0.55/langchain_experimental/sql/prompt.py
--rw-r--r--   0        0        0     9846 2024-03-14 13:23:46.833581 gigachain_experimental-0.0.55/langchain_experimental/sql/vector_sql.py
--rw-r--r--   0        0        0     1576 2024-03-27 08:44:31.275349 gigachain_experimental-0.0.55/langchain_experimental/synthetic_data/__init__.py
--rw-r--r--   0        0        0      459 2023-09-25 11:47:07.506582 gigachain_experimental-0.0.55/langchain_experimental/synthetic_data/prompts.py
--rw-r--r--   0        0        0       75 2024-03-27 08:44:31.275555 gigachain_experimental-0.0.55/langchain_experimental/tabular_synthetic_data/__init__.py
--rw-r--r--   0        0        0     5341 2024-03-14 13:23:46.834246 gigachain_experimental-0.0.55/langchain_experimental/tabular_synthetic_data/base.py
--rw-r--r--   0        0        0     2523 2024-03-27 08:44:31.275787 gigachain_experimental-0.0.55/langchain_experimental/tabular_synthetic_data/openai.py
--rw-r--r--   0        0        0      412 2023-10-02 10:00:42.632968 gigachain_experimental-0.0.55/langchain_experimental/tabular_synthetic_data/prompts.py
--rw-r--r--   0        0        0     9717 2024-03-27 08:44:31.276063 gigachain_experimental-0.0.55/langchain_experimental/text_splitter.py
--rw-r--r--   0        0        0      180 2024-03-27 08:44:31.276360 gigachain_experimental-0.0.55/langchain_experimental/tools/__init__.py
--rw-r--r--   0        0        0        0 2024-03-14 13:23:46.835906 gigachain_experimental-0.0.55/langchain_experimental/tools/python/__init__.py
--rw-r--r--   0        0        0     4763 2024-03-14 13:23:46.836127 gigachain_experimental-0.0.55/langchain_experimental/tools/python/tool.py
--rw-r--r--   0        0        0      425 2024-03-27 08:44:31.276709 gigachain_experimental-0.0.55/langchain_experimental/tot/__init__.py
--rw-r--r--   0        0        0     4853 2024-03-14 13:23:46.836804 gigachain_experimental-0.0.55/langchain_experimental/tot/base.py
--rw-r--r--   0        0        0     1405 2023-09-14 13:23:58.150719 gigachain_experimental-0.0.55/langchain_experimental/tot/checker.py
--rw-r--r--   0        0        0     1666 2023-09-14 13:23:58.150815 gigachain_experimental-0.0.55/langchain_experimental/tot/controller.py
--rw-r--r--   0        0        0     1467 2024-03-14 13:23:46.837178 gigachain_experimental-0.0.55/langchain_experimental/tot/memory.py
--rw-r--r--   0        0        0     4797 2024-03-27 08:44:31.682851 gigachain_experimental-0.0.55/langchain_experimental/tot/prompts.py
--rw-r--r--   0        0        0      504 2024-03-14 13:23:46.837821 gigachain_experimental-0.0.55/langchain_experimental/tot/thought.py
--rw-r--r--   0        0        0     3118 2024-03-14 13:23:46.838108 gigachain_experimental-0.0.55/langchain_experimental/tot/thought_generation.py
--rw-r--r--   0        0        0      148 2024-03-27 08:44:31.276951 gigachain_experimental-0.0.55/langchain_experimental/utilities/__init__.py
--rw-r--r--   0        0        0     2154 2024-03-14 13:23:46.838528 gigachain_experimental-0.0.55/langchain_experimental/utilities/python.py
--rw-r--r--   0        0        0     3924 2024-03-27 09:22:36.791968 gigachain_experimental-0.0.55/pyproject.toml
--rw-r--r--   0        0        0     2076 1970-01-01 00:00:00.000000 gigachain_experimental-0.0.55/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-03-14 13:23:46.793403 gigachain_experimental-0.0.55.1/LICENSE
+-rw-r--r--   0        0        0      731 2023-10-06 15:21:09.714881 gigachain_experimental-0.0.55.1/README.md
+-rw-r--r--   0        0        0      271 2024-03-14 13:23:46.793978 gigachain_experimental-0.0.55.1/langchain_experimental/__init__.py
+-rw-r--r--   0        0        0      643 2024-03-28 09:36:51.652536 gigachain_experimental-0.0.55.1/langchain_experimental/agents/__init__.py
+-rw-r--r--   0        0        0      653 2024-03-14 13:23:46.794474 gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/__init__.py
+-rw-r--r--   0        0        0       19 2024-03-14 13:23:46.794818 gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/csv/__init__.py
+-rw-r--r--   0        0        0     2407 2024-03-14 13:23:46.795018 gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/csv/base.py
+-rw-r--r--   0        0        0       22 2024-03-14 13:23:46.795255 gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/pandas/__init__.py
+-rw-r--r--   0        0        0    11290 2024-03-28 09:36:51.653497 gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/pandas/base.py
+-rw-r--r--   0        0        0     1113 2024-03-14 13:23:46.795892 gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/pandas/prompt.py
+-rw-r--r--   0        0        0        0 2024-03-14 13:23:46.796139 gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/python/__init__.py
+-rw-r--r--   0        0        0     2224 2024-03-14 13:23:46.796434 gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/python/base.py
+-rw-r--r--   0        0        0      513 2024-03-14 13:23:46.796678 gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/python/prompt.py
+-rw-r--r--   0        0        0       20 2024-03-14 13:23:46.797026 gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/spark/__init__.py
+-rw-r--r--   0        0        0     2761 2024-03-14 13:23:46.797378 gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/spark/base.py
+-rw-r--r--   0        0        0      295 2024-03-14 13:23:46.797631 gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/spark/prompt.py
+-rw-r--r--   0        0        0       23 2024-03-14 13:23:46.797989 gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/xorbits/__init__.py
+-rw-r--r--   0        0        0     3143 2024-03-14 13:23:46.798282 gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/xorbits/base.py
+-rw-r--r--   0        0        0     1070 2024-03-14 13:23:46.798536 gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/xorbits/prompt.py
+-rw-r--r--   0        0        0      866 2024-03-28 09:36:51.653973 gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-14 13:23:58.140059 gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/autogpt/__init__.py
+-rw-r--r--   0        0        0     5443 2024-03-14 13:23:46.799095 gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/autogpt/agent.py
+-rw-r--r--   0        0        0     1164 2024-03-14 13:23:46.799560 gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/autogpt/memory.py
+-rw-r--r--   0        0        0     1909 2024-03-14 13:23:46.799976 gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/autogpt/output_parser.py
+-rw-r--r--   0        0        0     5000 2024-03-14 13:23:46.800435 gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/autogpt/prompt.py
+-rw-r--r--   0        0        0     7963 2024-03-14 13:23:46.800907 gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/autogpt/prompt_generator.py
+-rw-r--r--   0        0        0      514 2023-09-14 13:23:58.140895 gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/baby_agi/__init__.py
+-rw-r--r--   0        0        0     8687 2024-03-14 13:23:46.801553 gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/baby_agi/baby_agi.py
+-rw-r--r--   0        0        0     1668 2024-03-28 09:36:51.654888 gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/baby_agi/task_creation.py
+-rw-r--r--   0        0        0      967 2024-03-28 09:36:51.655786 gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/baby_agi/task_execution.py
+-rw-r--r--   0        0        0     1283 2024-03-28 09:36:51.656463 gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/baby_agi/task_prioritization.py
+-rw-r--r--   0        0        0        0 2023-09-14 13:23:58.141519 gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/hugginggpt/__init__.py
+-rw-r--r--   0        0        0     1133 2024-03-14 13:23:46.803494 gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/hugginggpt/hugginggpt.py
+-rw-r--r--   0        0        0     1742 2024-03-28 09:36:51.657200 gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/hugginggpt/repsonse_generator.py
+-rw-r--r--   0        0        0     4598 2024-03-14 13:23:46.804390 gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/hugginggpt/task_executor.py
+-rw-r--r--   0        0        0     7859 2024-03-14 13:23:46.804893 gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/hugginggpt/task_planner.py
+-rw-r--r--   0        0        0      674 2024-03-28 09:36:51.657715 gigachain_experimental-0.0.55.1/langchain_experimental/chat_models/__init__.py
+-rw-r--r--   0        0        0     6063 2024-03-28 09:36:51.658161 gigachain_experimental-0.0.55.1/langchain_experimental/chat_models/llm_wrapper.py
+-rw-r--r--   0        0        0     2190 2024-03-28 09:36:51.658590 gigachain_experimental-0.0.55.1/langchain_experimental/comprehend_moderation/__init__.py
+-rw-r--r--   0        0        0     6659 2024-03-14 13:23:46.807228 gigachain_experimental-0.0.55.1/langchain_experimental/comprehend_moderation/amazon_comprehend_moderation.py
+-rw-r--r--   0        0        0     7411 2024-03-14 13:23:46.807736 gigachain_experimental-0.0.55.1/langchain_experimental/comprehend_moderation/base_moderation.py
+-rw-r--r--   0        0        0     2390 2024-03-14 13:23:46.808072 gigachain_experimental-0.0.55.1/langchain_experimental/comprehend_moderation/base_moderation_callbacks.py
+-rw-r--r--   0        0        0     1614 2024-03-14 13:23:46.808388 gigachain_experimental-0.0.55.1/langchain_experimental/comprehend_moderation/base_moderation_config.py
+-rw-r--r--   0        0        0      192 2023-09-14 13:23:58.142645 gigachain_experimental-0.0.55.1/langchain_experimental/comprehend_moderation/base_moderation_enums.py
+-rw-r--r--   0        0        0     1054 2024-03-14 13:23:46.808784 gigachain_experimental-0.0.55.1/langchain_experimental/comprehend_moderation/base_moderation_exceptions.py
+-rw-r--r--   0        0        0     6834 2024-03-14 13:23:46.809097 gigachain_experimental-0.0.55.1/langchain_experimental/comprehend_moderation/pii.py
+-rw-r--r--   0        0        0     3142 2024-03-14 13:23:46.809305 gigachain_experimental-0.0.55.1/langchain_experimental/comprehend_moderation/prompt_safety.py
+-rw-r--r--   0        0        0     8134 2024-03-14 13:23:46.809624 gigachain_experimental-0.0.55.1/langchain_experimental/comprehend_moderation/toxicity.py
+-rw-r--r--   0        0        0      103 2023-10-03 14:29:06.367456 gigachain_experimental-0.0.55.1/langchain_experimental/cpal/README.md
+-rw-r--r--   0        0        0      750 2024-03-28 09:36:51.658918 gigachain_experimental-0.0.55.1/langchain_experimental/cpal/__init__.py
+-rw-r--r--   0        0        0    11087 2024-03-14 13:23:46.809990 gigachain_experimental-0.0.55.1/langchain_experimental/cpal/base.py
+-rw-r--r--   0        0        0      246 2023-09-14 13:23:58.143626 gigachain_experimental-0.0.55.1/langchain_experimental/cpal/constants.py
+-rw-r--r--   0        0        0     9183 2024-03-14 13:23:46.810525 gigachain_experimental-0.0.55.1/langchain_experimental/cpal/models.py
+-rw-r--r--   0        0        0        0 2023-09-14 13:23:58.143845 gigachain_experimental-0.0.55.1/langchain_experimental/cpal/templates/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-14 13:23:58.144036 gigachain_experimental-0.0.55.1/langchain_experimental/cpal/templates/univariate/__init__.py
+-rw-r--r--   0        0        0     2548 2024-03-14 13:23:46.811061 gigachain_experimental-0.0.55.1/langchain_experimental/cpal/templates/univariate/causal.py
+-rw-r--r--   0        0        0      853 2024-03-14 13:23:46.811497 gigachain_experimental-0.0.55.1/langchain_experimental/cpal/templates/univariate/intervention.py
+-rw-r--r--   0        0        0     2905 2024-03-14 13:23:46.811993 gigachain_experimental-0.0.55.1/langchain_experimental/cpal/templates/univariate/narrative.py
+-rw-r--r--   0        0        0     5468 2024-03-14 13:23:46.812441 gigachain_experimental-0.0.55.1/langchain_experimental/cpal/templates/univariate/query.py
+-rw-r--r--   0        0        0      631 2024-03-28 09:36:51.659356 gigachain_experimental-0.0.55.1/langchain_experimental/data_anonymizer/__init__.py
+-rw-r--r--   0        0        0     1811 2024-03-14 13:23:46.813062 gigachain_experimental-0.0.55.1/langchain_experimental/data_anonymizer/base.py
+-rw-r--r--   0        0        0     4793 2024-03-14 13:23:46.813631 gigachain_experimental-0.0.55.1/langchain_experimental/data_anonymizer/deanonymizer_mapping.py
+-rw-r--r--   0        0        0     6801 2024-03-14 13:23:46.814004 gigachain_experimental-0.0.55.1/langchain_experimental/data_anonymizer/deanonymizer_matching_strategies.py
+-rw-r--r--   0        0        0     2861 2024-03-14 13:23:46.814331 gigachain_experimental-0.0.55.1/langchain_experimental/data_anonymizer/faker_presidio_mapping.py
+-rw-r--r--   0        0        0    17162 2024-03-14 13:23:46.814652 gigachain_experimental-0.0.55.1/langchain_experimental/data_anonymizer/presidio.py
+-rw-r--r--   0        0        0      368 2024-03-28 09:36:51.659603 gigachain_experimental-0.0.55.1/langchain_experimental/fallacy_removal/__init__.py
+-rw-r--r--   0        0        0      263 2024-03-28 09:36:51.660007 gigachain_experimental-0.0.55.1/langchain_experimental/generative_agents/__init__.py
+-rw-r--r--   0        0        0    10252 2024-03-28 09:36:51.660456 gigachain_experimental-0.0.55.1/langchain_experimental/generative_agents/generative_agent.py
+-rw-r--r--   0        0        0    13413 2024-03-28 09:36:51.661467 gigachain_experimental-0.0.55.1/langchain_experimental/generative_agents/memory.py
+-rw-r--r--   0        0        0      308 2024-03-28 09:36:51.661909 gigachain_experimental-0.0.55.1/langchain_experimental/graph_transformers/__init__.py
+-rw-r--r--   0        0        0    10723 2024-03-28 09:36:51.662387 gigachain_experimental-0.0.55.1/langchain_experimental/graph_transformers/diffbot.py
+-rw-r--r--   0        0        0    12290 2024-03-28 09:36:51.662690 gigachain_experimental-0.0.55.1/langchain_experimental/graph_transformers/llm.py
+-rw-r--r--   0        0        0       94 2024-03-28 09:36:51.663096 gigachain_experimental-0.0.55.1/langchain_experimental/llm_bash/__init__.py
+-rw-r--r--   0        0        0     4454 2024-03-14 13:23:46.816866 gigachain_experimental-0.0.55.1/langchain_experimental/llm_bash/base.py
+-rw-r--r--   0        0        0     5708 2024-03-14 13:23:46.817282 gigachain_experimental-0.0.55.1/langchain_experimental/llm_bash/bash.py
+-rw-r--r--   0        0        0     2038 2024-03-14 13:23:46.817632 gigachain_experimental-0.0.55.1/langchain_experimental/llm_bash/prompt.py
+-rw-r--r--   0        0        0      164 2024-03-28 09:36:51.663490 gigachain_experimental-0.0.55.1/langchain_experimental/llm_symbolic_math/__init__.py
+-rw-r--r--   0        0        0     5791 2024-03-14 13:23:46.818120 gigachain_experimental-0.0.55.1/langchain_experimental/llm_symbolic_math/base.py
+-rw-r--r--   0        0        0     1087 2023-10-06 15:21:09.721677 gigachain_experimental-0.0.55.1/langchain_experimental/llm_symbolic_math/prompt.py
+-rw-r--r--   0        0        0      453 2024-03-28 09:36:51.663878 gigachain_experimental-0.0.55.1/langchain_experimental/llms/__init__.py
+-rw-r--r--   0        0        0     8768 2024-03-28 09:36:51.664630 gigachain_experimental-0.0.55.1/langchain_experimental/llms/anthropic_functions.py
+-rw-r--r--   0        0        0     2228 2024-03-14 13:23:46.820107 gigachain_experimental-0.0.55.1/langchain_experimental/llms/jsonformer_decoder.py
+-rw-r--r--   0        0        0     4344 2024-03-14 13:23:46.820880 gigachain_experimental-0.0.55.1/langchain_experimental/llms/llamaapi.py
+-rw-r--r--   0        0        0     2843 2024-03-14 13:23:46.821460 gigachain_experimental-0.0.55.1/langchain_experimental/llms/lmformatenforcer_decoder.py
+-rw-r--r--   0        0        0     4932 2024-03-14 13:23:46.821957 gigachain_experimental-0.0.55.1/langchain_experimental/llms/ollama_functions.py
+-rw-r--r--   0        0        0     2342 2024-03-14 13:23:46.822538 gigachain_experimental-0.0.55.1/langchain_experimental/llms/rellm_decoder.py
+-rw-r--r--   0        0        0      346 2024-03-28 09:36:51.665067 gigachain_experimental-0.0.55.1/langchain_experimental/open_clip/__init__.py
+-rw-r--r--   0        0        0     3383 2024-03-14 13:23:46.823943 gigachain_experimental-0.0.55.1/langchain_experimental/open_clip/open_clip.py
+-rw-r--r--   0        0        0      120 2024-03-14 13:23:46.824923 gigachain_experimental-0.0.55.1/langchain_experimental/openai_assistant/__init__.py
+-rw-r--r--   0        0        0      185 2024-03-14 13:23:46.825679 gigachain_experimental-0.0.55.1/langchain_experimental/openai_assistant/base.py
+-rw-r--r--   0        0        0      330 2024-03-28 09:36:51.665470 gigachain_experimental-0.0.55.1/langchain_experimental/pal_chain/__init__.py
+-rw-r--r--   0        0        0    13320 2024-03-14 13:23:46.826384 gigachain_experimental-0.0.55.1/langchain_experimental/pal_chain/base.py
+-rw-r--r--   0        0        0     3537 2023-09-14 13:23:58.147176 gigachain_experimental-0.0.55.1/langchain_experimental/pal_chain/colored_object_prompt.py
+-rw-r--r--   0        0        0     5767 2023-09-14 13:23:58.147272 gigachain_experimental-0.0.55.1/langchain_experimental/pal_chain/math_prompt.py
+-rw-r--r--   0        0        0      488 2024-03-28 09:36:51.665891 gigachain_experimental-0.0.55.1/langchain_experimental/plan_and_execute/__init__.py
+-rw-r--r--   0        0        0     3570 2023-09-14 13:23:58.147536 gigachain_experimental-0.0.55.1/langchain_experimental/plan_and_execute/agent_executor.py
+-rw-r--r--   0        0        0        0 2023-09-14 13:23:58.147634 gigachain_experimental-0.0.55.1/langchain_experimental/plan_and_execute/executors/__init__.py
+-rw-r--r--   0        0        0     1463 2024-03-14 13:23:46.826994 gigachain_experimental-0.0.55.1/langchain_experimental/plan_and_execute/executors/agent_executor.py
+-rw-r--r--   0        0        0     1269 2023-09-14 13:23:58.147861 gigachain_experimental-0.0.55.1/langchain_experimental/plan_and_execute/executors/base.py
+-rw-r--r--   0        0        0        0 2023-09-14 13:23:58.147962 gigachain_experimental-0.0.55.1/langchain_experimental/plan_and_execute/planners/__init__.py
+-rw-r--r--   0        0        0     1567 2023-09-14 13:23:58.148116 gigachain_experimental-0.0.55.1/langchain_experimental/plan_and_execute/planners/base.py
+-rw-r--r--   0        0        0     2314 2024-03-14 13:23:46.827423 gigachain_experimental-0.0.55.1/langchain_experimental/plan_and_execute/planners/chat_planner.py
+-rw-r--r--   0        0        0     1439 2024-03-14 13:23:46.827784 gigachain_experimental-0.0.55.1/langchain_experimental/plan_and_execute/schema.py
+-rw-r--r--   0        0        0      369 2024-03-28 09:36:51.666293 gigachain_experimental-0.0.55.1/langchain_experimental/prompt_injection_identifier/__init__.py
+-rw-r--r--   0        0        0     3369 2024-03-28 09:36:51.666703 gigachain_experimental-0.0.55.1/langchain_experimental/prompt_injection_identifier/hugging_face_identifier.py
+-rw-r--r--   0        0        0      174 2024-03-28 09:36:51.667078 gigachain_experimental-0.0.55.1/langchain_experimental/prompts/__init__.py
+-rw-r--r--   0        0        0     1942 2024-03-14 13:23:46.828890 gigachain_experimental-0.0.55.1/langchain_experimental/prompts/load.py
+-rw-r--r--   0        0        0        0 2023-09-14 13:23:58.148908 gigachain_experimental-0.0.55.1/langchain_experimental/py.typed
+-rw-r--r--   0        0        0     1285 2023-09-14 13:23:58.149124 gigachain_experimental-0.0.55.1/langchain_experimental/pydantic_v1/__init__.py
+-rw-r--r--   0        0        0      548 2023-09-14 13:23:58.149226 gigachain_experimental-0.0.55.1/langchain_experimental/pydantic_v1/dataclasses.py
+-rw-r--r--   0        0        0      520 2023-09-14 13:23:58.149317 gigachain_experimental-0.0.55.1/langchain_experimental/pydantic_v1/main.py
+-rw-r--r--   0        0        0      518 2024-03-28 09:36:51.667459 gigachain_experimental-0.0.55.1/langchain_experimental/recommenders/__init__.py
+-rw-r--r--   0        0        0     7967 2024-03-28 09:36:51.667839 gigachain_experimental-0.0.55.1/langchain_experimental/recommenders/amazon_personalize.py
+-rw-r--r--   0        0        0     6964 2024-03-14 13:23:46.829648 gigachain_experimental-0.0.55.1/langchain_experimental/recommenders/amazon_personalize_chain.py
+-rw-r--r--   0        0        0      200 2024-03-28 09:36:51.668184 gigachain_experimental-0.0.55.1/langchain_experimental/retrievers/__init__.py
+-rw-r--r--   0        0        0     1248 2024-03-14 13:23:46.830070 gigachain_experimental-0.0.55.1/langchain_experimental/retrievers/vector_sql_database.py
+-rw-r--r--   0        0        0     1447 2024-03-28 09:36:51.668550 gigachain_experimental-0.0.55.1/langchain_experimental/rl_chain/__init__.py
+-rw-r--r--   0        0        0    23241 2024-03-14 13:23:46.830706 gigachain_experimental-0.0.55.1/langchain_experimental/rl_chain/base.py
+-rw-r--r--   0        0        0     1989 2024-03-14 13:23:46.831066 gigachain_experimental-0.0.55.1/langchain_experimental/rl_chain/metrics.py
+-rw-r--r--   0        0        0     2126 2024-03-14 13:23:46.831366 gigachain_experimental-0.0.55.1/langchain_experimental/rl_chain/model_repository.py
+-rw-r--r--   0        0        0    16279 2024-03-14 13:23:46.831741 gigachain_experimental-0.0.55.1/langchain_experimental/rl_chain/pick_best_chain.py
+-rw-r--r--   0        0        0      556 2024-03-14 13:23:46.832050 gigachain_experimental-0.0.55.1/langchain_experimental/rl_chain/vw_logger.py
+-rw-r--r--   0        0        0      946 2024-03-28 09:36:51.668927 gigachain_experimental-0.0.55.1/langchain_experimental/smart_llm/__init__.py
+-rw-r--r--   0        0        0    14423 2024-03-14 13:23:46.832807 gigachain_experimental-0.0.55.1/langchain_experimental/smart_llm/base.py
+-rw-r--r--   0        0        0      202 2024-03-28 09:36:51.669275 gigachain_experimental-0.0.55.1/langchain_experimental/sql/__init__.py
+-rw-r--r--   0        0        0    13112 2024-03-14 13:23:46.833225 gigachain_experimental-0.0.55.1/langchain_experimental/sql/base.py
+-rw-r--r--   0        0        0     4658 2023-09-25 11:47:07.505993 gigachain_experimental-0.0.55.1/langchain_experimental/sql/prompt.py
+-rw-r--r--   0        0        0     9846 2024-03-14 13:23:46.833581 gigachain_experimental-0.0.55.1/langchain_experimental/sql/vector_sql.py
+-rw-r--r--   0        0        0     1576 2024-03-28 09:36:51.669999 gigachain_experimental-0.0.55.1/langchain_experimental/synthetic_data/__init__.py
+-rw-r--r--   0        0        0      459 2023-09-25 11:47:07.506582 gigachain_experimental-0.0.55.1/langchain_experimental/synthetic_data/prompts.py
+-rw-r--r--   0        0        0       75 2024-03-28 09:36:51.670326 gigachain_experimental-0.0.55.1/langchain_experimental/tabular_synthetic_data/__init__.py
+-rw-r--r--   0        0        0     5341 2024-03-14 13:23:46.834246 gigachain_experimental-0.0.55.1/langchain_experimental/tabular_synthetic_data/base.py
+-rw-r--r--   0        0        0     2523 2024-03-28 09:36:51.670695 gigachain_experimental-0.0.55.1/langchain_experimental/tabular_synthetic_data/openai.py
+-rw-r--r--   0        0        0      412 2023-10-02 10:00:42.632968 gigachain_experimental-0.0.55.1/langchain_experimental/tabular_synthetic_data/prompts.py
+-rw-r--r--   0        0        0     9717 2024-03-28 09:36:51.671475 gigachain_experimental-0.0.55.1/langchain_experimental/text_splitter.py
+-rw-r--r--   0        0        0      180 2024-03-28 09:36:51.671871 gigachain_experimental-0.0.55.1/langchain_experimental/tools/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-14 13:23:46.835906 gigachain_experimental-0.0.55.1/langchain_experimental/tools/python/__init__.py
+-rw-r--r--   0        0        0     4763 2024-03-14 13:23:46.836127 gigachain_experimental-0.0.55.1/langchain_experimental/tools/python/tool.py
+-rw-r--r--   0        0        0      425 2024-03-28 09:36:51.672261 gigachain_experimental-0.0.55.1/langchain_experimental/tot/__init__.py
+-rw-r--r--   0        0        0     4853 2024-03-14 13:23:46.836804 gigachain_experimental-0.0.55.1/langchain_experimental/tot/base.py
+-rw-r--r--   0        0        0     1405 2023-09-14 13:23:58.150719 gigachain_experimental-0.0.55.1/langchain_experimental/tot/checker.py
+-rw-r--r--   0        0        0     1666 2023-09-14 13:23:58.150815 gigachain_experimental-0.0.55.1/langchain_experimental/tot/controller.py
+-rw-r--r--   0        0        0     1467 2024-03-14 13:23:46.837178 gigachain_experimental-0.0.55.1/langchain_experimental/tot/memory.py
+-rw-r--r--   0        0        0     4797 2024-03-28 09:36:51.672937 gigachain_experimental-0.0.55.1/langchain_experimental/tot/prompts.py
+-rw-r--r--   0        0        0      504 2024-03-14 13:23:46.837821 gigachain_experimental-0.0.55.1/langchain_experimental/tot/thought.py
+-rw-r--r--   0        0        0     3118 2024-03-14 13:23:46.838108 gigachain_experimental-0.0.55.1/langchain_experimental/tot/thought_generation.py
+-rw-r--r--   0        0        0      148 2024-03-28 09:36:51.673359 gigachain_experimental-0.0.55.1/langchain_experimental/utilities/__init__.py
+-rw-r--r--   0        0        0     2154 2024-03-14 13:23:46.838528 gigachain_experimental-0.0.55.1/langchain_experimental/utilities/python.py
+-rw-r--r--   0        0        0     3926 2024-04-03 12:54:10.693476 gigachain_experimental-0.0.55.1/pyproject.toml
+-rw-r--r--   0        0        0     2078 1970-01-01 00:00:00.000000 gigachain_experimental-0.0.55.1/PKG-INFO
```

### Comparing `gigachain_experimental-0.0.55/LICENSE` & `gigachain_experimental-0.0.55.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/README.md` & `gigachain_experimental-0.0.55.1/README.md`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/agents/__init__.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/agents/agent_toolkits/__init__.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/agents/agent_toolkits/csv/base.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/csv/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/agents/agent_toolkits/pandas/base.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/pandas/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/agents/agent_toolkits/pandas/prompt.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/pandas/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/agents/agent_toolkits/python/base.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/python/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/agents/agent_toolkits/python/prompt.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/python/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/agents/agent_toolkits/spark/base.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/spark/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/agents/agent_toolkits/xorbits/base.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/xorbits/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/agents/agent_toolkits/xorbits/prompt.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/xorbits/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/autonomous_agents/__init__.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/autonomous_agents/autogpt/agent.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/autogpt/agent.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/autonomous_agents/autogpt/memory.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/autogpt/memory.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/autonomous_agents/autogpt/output_parser.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/autogpt/output_parser.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/autonomous_agents/autogpt/prompt.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/autogpt/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/autonomous_agents/autogpt/prompt_generator.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/autogpt/prompt_generator.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/autonomous_agents/baby_agi/__init__.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/baby_agi/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/autonomous_agents/baby_agi/baby_agi.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/baby_agi/baby_agi.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/autonomous_agents/baby_agi/task_creation.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/baby_agi/task_creation.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/autonomous_agents/baby_agi/task_execution.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/baby_agi/task_execution.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/autonomous_agents/baby_agi/task_prioritization.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/baby_agi/task_prioritization.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/autonomous_agents/hugginggpt/hugginggpt.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/hugginggpt/hugginggpt.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/autonomous_agents/hugginggpt/repsonse_generator.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/hugginggpt/repsonse_generator.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/autonomous_agents/hugginggpt/task_executor.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/hugginggpt/task_executor.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/autonomous_agents/hugginggpt/task_planner.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/hugginggpt/task_planner.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/chat_models/__init__.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/chat_models/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/chat_models/llm_wrapper.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/chat_models/llm_wrapper.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/comprehend_moderation/__init__.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/comprehend_moderation/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/comprehend_moderation/amazon_comprehend_moderation.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/comprehend_moderation/amazon_comprehend_moderation.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/comprehend_moderation/base_moderation.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/comprehend_moderation/base_moderation.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/comprehend_moderation/base_moderation_callbacks.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/comprehend_moderation/base_moderation_callbacks.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/comprehend_moderation/base_moderation_config.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/comprehend_moderation/base_moderation_config.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/comprehend_moderation/base_moderation_exceptions.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/comprehend_moderation/base_moderation_exceptions.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/comprehend_moderation/pii.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/comprehend_moderation/pii.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/comprehend_moderation/prompt_safety.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/comprehend_moderation/prompt_safety.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/comprehend_moderation/toxicity.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/comprehend_moderation/toxicity.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/cpal/__init__.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/cpal/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/cpal/base.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/cpal/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/cpal/models.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/cpal/models.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/cpal/templates/univariate/causal.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/cpal/templates/univariate/causal.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/cpal/templates/univariate/intervention.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/cpal/templates/univariate/intervention.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/cpal/templates/univariate/narrative.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/cpal/templates/univariate/narrative.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/cpal/templates/univariate/query.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/cpal/templates/univariate/query.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/data_anonymizer/__init__.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/data_anonymizer/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/data_anonymizer/base.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/data_anonymizer/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/data_anonymizer/deanonymizer_mapping.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/data_anonymizer/deanonymizer_mapping.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/data_anonymizer/deanonymizer_matching_strategies.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/data_anonymizer/deanonymizer_matching_strategies.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/data_anonymizer/faker_presidio_mapping.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/data_anonymizer/faker_presidio_mapping.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/data_anonymizer/presidio.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/data_anonymizer/presidio.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/generative_agents/generative_agent.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/generative_agents/generative_agent.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/generative_agents/memory.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/generative_agents/memory.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/graph_transformers/diffbot.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/graph_transformers/diffbot.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/graph_transformers/llm.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/graph_transformers/llm.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/llm_bash/base.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/llm_bash/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/llm_bash/bash.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/llm_bash/bash.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/llm_bash/prompt.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/llm_bash/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/llm_symbolic_math/base.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/llm_symbolic_math/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/llm_symbolic_math/prompt.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/llm_symbolic_math/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/llms/anthropic_functions.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/llms/anthropic_functions.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/llms/jsonformer_decoder.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/llms/jsonformer_decoder.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/llms/llamaapi.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/llms/llamaapi.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/llms/lmformatenforcer_decoder.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/llms/lmformatenforcer_decoder.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/llms/ollama_functions.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/llms/ollama_functions.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/llms/rellm_decoder.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/llms/rellm_decoder.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/open_clip/open_clip.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/open_clip/open_clip.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/pal_chain/base.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/pal_chain/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/pal_chain/colored_object_prompt.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/pal_chain/colored_object_prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/pal_chain/math_prompt.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/pal_chain/math_prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/plan_and_execute/agent_executor.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/plan_and_execute/agent_executor.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/plan_and_execute/executors/agent_executor.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/plan_and_execute/executors/agent_executor.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/plan_and_execute/executors/base.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/plan_and_execute/executors/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/plan_and_execute/planners/base.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/plan_and_execute/planners/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/plan_and_execute/planners/chat_planner.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/plan_and_execute/planners/chat_planner.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/plan_and_execute/schema.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/plan_and_execute/schema.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/prompt_injection_identifier/hugging_face_identifier.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/prompt_injection_identifier/hugging_face_identifier.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/prompts/load.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/prompts/load.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/pydantic_v1/__init__.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/pydantic_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/pydantic_v1/dataclasses.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/pydantic_v1/dataclasses.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/pydantic_v1/main.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/pydantic_v1/main.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/recommenders/__init__.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/recommenders/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/recommenders/amazon_personalize.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/recommenders/amazon_personalize.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/recommenders/amazon_personalize_chain.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/recommenders/amazon_personalize_chain.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/retrievers/vector_sql_database.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/retrievers/vector_sql_database.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/rl_chain/__init__.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/rl_chain/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/rl_chain/base.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/rl_chain/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/rl_chain/metrics.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/rl_chain/metrics.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/rl_chain/model_repository.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/rl_chain/model_repository.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/rl_chain/pick_best_chain.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/rl_chain/pick_best_chain.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/rl_chain/vw_logger.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/rl_chain/vw_logger.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/smart_llm/__init__.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/smart_llm/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/smart_llm/base.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/smart_llm/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/sql/base.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/sql/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/sql/prompt.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/sql/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/sql/vector_sql.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/sql/vector_sql.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/synthetic_data/__init__.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/synthetic_data/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/tabular_synthetic_data/base.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/tabular_synthetic_data/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/tabular_synthetic_data/openai.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/tabular_synthetic_data/openai.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/text_splitter.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/text_splitter.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/tools/python/tool.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/tools/python/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/tot/base.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/tot/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/tot/checker.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/tot/checker.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/tot/controller.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/tot/controller.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/tot/memory.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/tot/memory.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/tot/prompts.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/tot/prompts.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/tot/thought_generation.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/tot/thought_generation.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/langchain_experimental/utilities/python.py` & `gigachain_experimental-0.0.55.1/langchain_experimental/utilities/python.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55/pyproject.toml` & `gigachain_experimental-0.0.55.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gigachain-experimental"
-version = "0.0.55"
+version = "0.0.55.1"
 description = "Building applications with LLMs through composability"
 authors = []
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ai-forever/gigachain"
 packages = [
     {include = "langchain_experimental"}
@@ -58,15 +58,15 @@
 # dependencies used for running tests (e.g., pytest, freezegun, response).
 # Any dependencies that do not meet that criteria will be removed.
 pytest = "^7.3.0"
 pytest-asyncio = "^0.20.3"
 gigachain = {path = "../langchain", develop = true}
 gigachain-core = {path = "../core", develop = true}
 gigachain-community = {path = "../community", develop = true}
-gigachat = "^0.1.20"
+gigachat = "^0.1.22"
 
 
 [tool.poetry.group.test_integration]
 optional = true
 
 [tool.poetry.group.test_integration.dependencies]
 gigachain = {path = "../langchain", develop = true}
```

### Comparing `gigachain_experimental-0.0.55/PKG-INFO` & `gigachain_experimental-0.0.55.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gigachain-experimental
-Version: 0.0.55
+Version: 0.0.55.1
 Summary: Building applications with LLMs through composability
 Home-page: https://github.com/ai-forever/gigachain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

