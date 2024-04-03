# Comparing `tmp/gigachain_community-0.0.6.tar.gz` & `tmp/gigachain_community-0.0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gigachain_community-0.0.6.tar", max compression
+gzip compressed data, was "gigachain_community-0.0.6.1.tar", max compression
```

## Comparing `gigachain_community-0.0.6.tar` & `gigachain_community-0.0.6.1.tar`

### file list

```diff
@@ -1,884 +1,884 @@
--rw-r--r--   0        0        0     1201 2023-12-21 15:51:51.774421 gigachain_community-0.0.6/README.md
--rw-r--r--   0        0        0      307 2023-12-18 12:05:45.464203 gigachain_community-0.0.6/langchain_community/__init__.py
--rw-r--r--   0        0        0        0 2023-12-18 12:05:45.464419 gigachain_community-0.0.6/langchain_community/adapters/__init__.py
--rw-r--r--   0        0        0    12143 2023-12-21 15:51:51.775428 gigachain_community-0.0.6/langchain_community/adapters/openai.py
--rw-r--r--   0        0        0     3327 2023-12-18 12:05:45.466331 gigachain_community-0.0.6/langchain_community/agent_toolkits/__init__.py
--rw-r--r--   0        0        0       25 2023-12-18 12:05:45.466917 gigachain_community-0.0.6/langchain_community/agent_toolkits/ainetwork/__init__.py
--rw-r--r--   0        0        0     1781 2023-12-18 12:05:45.467514 gigachain_community-0.0.6/langchain_community/agent_toolkits/ainetwork/toolkit.py
--rw-r--r--   0        0        0        0 2023-12-18 12:05:45.467736 gigachain_community-0.0.6/langchain_community/agent_toolkits/amadeus/__init__.py
--rw-r--r--   0        0        0      961 2023-12-18 12:05:45.468139 gigachain_community-0.0.6/langchain_community/agent_toolkits/amadeus/toolkit.py
--rw-r--r--   0        0        0     1035 2023-12-18 12:05:45.468506 gigachain_community-0.0.6/langchain_community/agent_toolkits/azure_cognitive_services.py
--rw-r--r--   0        0        0      397 2023-12-18 12:05:45.468850 gigachain_community-0.0.6/langchain_community/agent_toolkits/base.py
--rw-r--r--   0        0        0        0 2023-12-18 12:05:45.469039 gigachain_community-0.0.6/langchain_community/agent_toolkits/clickup/__init__.py
--rw-r--r--   0        0        0     3594 2023-12-18 12:05:45.469520 gigachain_community-0.0.6/langchain_community/agent_toolkits/clickup/toolkit.py
--rw-r--r--   0        0        0     1091 2023-12-18 12:05:45.470285 gigachain_community-0.0.6/langchain_community/agent_toolkits/csv/__init__.py
--rw-r--r--   0        0        0      177 2023-12-18 12:05:45.470616 gigachain_community-0.0.6/langchain_community/agent_toolkits/file_management/__init__.py
--rw-r--r--   0        0        0     3250 2023-12-18 12:05:45.471261 gigachain_community-0.0.6/langchain_community/agent_toolkits/file_management/toolkit.py
--rw-r--r--   0        0        0       22 2023-12-18 12:05:45.471646 gigachain_community-0.0.6/langchain_community/agent_toolkits/github/__init__.py
--rw-r--r--   0        0        0    10135 2023-12-21 15:51:51.776418 gigachain_community-0.0.6/langchain_community/agent_toolkits/github/toolkit.py
--rw-r--r--   0        0        0       22 2023-12-18 12:05:45.472496 gigachain_community-0.0.6/langchain_community/agent_toolkits/gitlab/__init__.py
--rw-r--r--   0        0        0     2904 2023-12-18 12:05:45.472989 gigachain_community-0.0.6/langchain_community/agent_toolkits/gitlab/toolkit.py
--rw-r--r--   0        0        0       21 2023-12-18 12:05:45.473348 gigachain_community-0.0.6/langchain_community/agent_toolkits/gmail/__init__.py
--rw-r--r--   0        0        0     2045 2023-12-18 12:05:45.473719 gigachain_community-0.0.6/langchain_community/agent_toolkits/gmail/toolkit.py
--rw-r--r--   0        0        0       20 2023-12-18 12:05:45.474062 gigachain_community-0.0.6/langchain_community/agent_toolkits/jira/__init__.py
--rw-r--r--   0        0        0     2227 2023-12-18 12:05:45.474505 gigachain_community-0.0.6/langchain_community/agent_toolkits/jira/toolkit.py
--rw-r--r--   0        0        0       18 2023-12-18 12:05:45.474878 gigachain_community-0.0.6/langchain_community/agent_toolkits/json/__init__.py
--rw-r--r--   0        0        0     1894 2023-12-18 12:05:45.475275 gigachain_community-0.0.6/langchain_community/agent_toolkits/json/base.py
--rw-r--r--   0        0        0     3288 2023-12-18 12:05:45.475625 gigachain_community-0.0.6/langchain_community/agent_toolkits/json/prompt.py
--rw-r--r--   0        0        0      595 2023-12-18 12:05:45.475954 gigachain_community-0.0.6/langchain_community/agent_toolkits/json/toolkit.py
--rw-r--r--   0        0        0       23 2023-12-18 12:05:45.476309 gigachain_community-0.0.6/langchain_community/agent_toolkits/multion/__init__.py
--rw-r--r--   0        0        0     1190 2023-12-18 12:05:45.476676 gigachain_community-0.0.6/langchain_community/agent_toolkits/multion/toolkit.py
--rw-r--r--   0        0        0       19 2023-12-18 12:05:45.477080 gigachain_community-0.0.6/langchain_community/agent_toolkits/nasa/__init__.py
--rw-r--r--   0        0        0     1931 2023-12-18 12:05:45.477469 gigachain_community-0.0.6/langchain_community/agent_toolkits/nasa/toolkit.py
--rw-r--r--   0        0        0        0 2023-12-18 12:05:45.477737 gigachain_community-0.0.6/langchain_community/agent_toolkits/nla/__init__.py
--rw-r--r--   0        0        0     2038 2023-12-18 12:05:45.478181 gigachain_community-0.0.6/langchain_community/agent_toolkits/nla/tool.py
--rw-r--r--   0        0        0     4228 2023-12-18 12:05:45.478766 gigachain_community-0.0.6/langchain_community/agent_toolkits/nla/toolkit.py
--rw-r--r--   0        0        0       25 2023-12-18 12:05:45.479165 gigachain_community-0.0.6/langchain_community/agent_toolkits/office365/__init__.py
--rw-r--r--   0        0        0     1812 2023-12-18 12:05:45.479543 gigachain_community-0.0.6/langchain_community/agent_toolkits/office365/toolkit.py
--rw-r--r--   0        0        0       26 2023-12-18 12:05:45.479989 gigachain_community-0.0.6/langchain_community/agent_toolkits/openapi/__init__.py
--rw-r--r--   0        0        0     2870 2023-12-18 12:05:45.480437 gigachain_community-0.0.6/langchain_community/agent_toolkits/openapi/base.py
--rw-r--r--   0        0        0    12987 2023-12-18 12:05:45.481612 gigachain_community-0.0.6/langchain_community/agent_toolkits/openapi/planner.py
--rw-r--r--   0        0        0    19382 2023-12-18 12:05:45.482208 gigachain_community-0.0.6/langchain_community/agent_toolkits/openapi/planner_prompt.py
--rw-r--r--   0        0        0     3174 2023-12-18 12:05:45.482651 gigachain_community-0.0.6/langchain_community/agent_toolkits/openapi/prompt.py
--rw-r--r--   0        0        0     2557 2023-12-18 12:05:45.483038 gigachain_community-0.0.6/langchain_community/agent_toolkits/openapi/spec.py
--rw-r--r--   0        0        0     3317 2023-12-18 12:05:45.483317 gigachain_community-0.0.6/langchain_community/agent_toolkits/openapi/toolkit.py
--rw-r--r--   0        0        0      174 2023-12-18 12:05:45.483588 gigachain_community-0.0.6/langchain_community/agent_toolkits/playwright/__init__.py
--rw-r--r--   0        0        0     4274 2023-12-18 12:05:45.483947 gigachain_community-0.0.6/langchain_community/agent_toolkits/playwright/toolkit.py
--rw-r--r--   0        0        0       22 2023-12-18 12:05:45.484213 gigachain_community-0.0.6/langchain_community/agent_toolkits/powerbi/__init__.py
--rw-r--r--   0        0        0     2507 2023-12-18 12:05:45.484545 gigachain_community-0.0.6/langchain_community/agent_toolkits/powerbi/base.py
--rw-r--r--   0        0        0     2649 2023-12-18 12:05:45.484863 gigachain_community-0.0.6/langchain_community/agent_toolkits/powerbi/chat_base.py
--rw-r--r--   0        0        0     5098 2023-12-18 12:05:45.485270 gigachain_community-0.0.6/langchain_community/agent_toolkits/powerbi/prompt.py
--rw-r--r--   0        0        0     3771 2023-12-18 12:05:45.485517 gigachain_community-0.0.6/langchain_community/agent_toolkits/powerbi/toolkit.py
--rw-r--r--   0        0        0       21 2023-12-18 12:05:45.485842 gigachain_community-0.0.6/langchain_community/agent_toolkits/slack/__init__.py
--rw-r--r--   0        0        0     1114 2023-12-18 12:05:45.486216 gigachain_community-0.0.6/langchain_community/agent_toolkits/slack/toolkit.py
--rw-r--r--   0        0        0       23 2023-12-18 12:05:45.486932 gigachain_community-0.0.6/langchain_community/agent_toolkits/spark_sql/__init__.py
--rw-r--r--   0        0        0     2355 2023-12-18 12:05:45.487251 gigachain_community-0.0.6/langchain_community/agent_toolkits/spark_sql/base.py
--rw-r--r--   0        0        0     2297 2023-12-18 12:05:45.487719 gigachain_community-0.0.6/langchain_community/agent_toolkits/spark_sql/prompt.py
--rw-r--r--   0        0        0     1084 2023-12-18 12:05:45.488627 gigachain_community-0.0.6/langchain_community/agent_toolkits/spark_sql/toolkit.py
--rw-r--r--   0        0        0       17 2023-12-18 12:05:45.489163 gigachain_community-0.0.6/langchain_community/agent_toolkits/sql/__init__.py
--rw-r--r--   0        0        0     3866 2023-12-18 12:05:45.489752 gigachain_community-0.0.6/langchain_community/agent_toolkits/sql/base.py
--rw-r--r--   0        0        0     2727 2023-12-18 12:05:45.490038 gigachain_community-0.0.6/langchain_community/agent_toolkits/sql/prompt.py
--rw-r--r--   0        0        0     2862 2023-12-18 12:05:45.490548 gigachain_community-0.0.6/langchain_community/agent_toolkits/sql/toolkit.py
--rw-r--r--   0        0        0       21 2023-12-18 12:05:45.490899 gigachain_community-0.0.6/langchain_community/agent_toolkits/steam/__init__.py
--rw-r--r--   0        0        0     1465 2023-12-18 12:05:45.491412 gigachain_community-0.0.6/langchain_community/agent_toolkits/steam/toolkit.py
--rw-r--r--   0        0        0     1095 2023-12-18 12:05:45.491874 gigachain_community-0.0.6/langchain_community/agent_toolkits/xorbits/__init__.py
--rw-r--r--   0        0        0       22 2023-12-18 12:05:45.492214 gigachain_community-0.0.6/langchain_community/agent_toolkits/zapier/__init__.py
--rw-r--r--   0        0        0     1933 2023-12-18 12:05:45.492667 gigachain_community-0.0.6/langchain_community/agent_toolkits/zapier/toolkit.py
--rw-r--r--   0        0        0    58113 2023-12-21 15:51:51.777487 gigachain_community-0.0.6/langchain_community/cache.py
--rw-r--r--   0        0        0     2671 2023-12-18 12:05:45.494039 gigachain_community-0.0.6/langchain_community/callbacks/__init__.py
--rw-r--r--   0        0        0    14408 2023-12-18 12:05:45.494709 gigachain_community-0.0.6/langchain_community/callbacks/aim_callback.py
--rw-r--r--   0        0        0    14820 2023-12-18 12:05:45.495433 gigachain_community-0.0.6/langchain_community/callbacks/argilla_callback.py
--rw-r--r--   0        0        0     7438 2023-12-18 12:05:45.496089 gigachain_community-0.0.6/langchain_community/callbacks/arize_callback.py
--rw-r--r--   0        0        0    11266 2023-12-18 12:05:45.496863 gigachain_community-0.0.6/langchain_community/callbacks/arthur_callback.py
--rw-r--r--   0        0        0    18897 2023-12-18 12:05:45.497277 gigachain_community-0.0.6/langchain_community/callbacks/clearml_callback.py
--rw-r--r--   0        0        0    23193 2023-12-18 12:05:45.497760 gigachain_community-0.0.6/langchain_community/callbacks/comet_ml_callback.py
--rw-r--r--   0        0        0     6340 2023-12-18 12:05:45.498346 gigachain_community-0.0.6/langchain_community/callbacks/confident_callback.py
--rw-r--r--   0        0        0     6498 2023-12-18 12:05:45.498833 gigachain_community-0.0.6/langchain_community/callbacks/context_callback.py
--rw-r--r--   0        0        0    13138 2023-12-18 12:05:45.499879 gigachain_community-0.0.6/langchain_community/callbacks/flyte_callback.py
--rw-r--r--   0        0        0     2587 2023-12-18 12:05:45.500223 gigachain_community-0.0.6/langchain_community/callbacks/human.py
--rw-r--r--   0        0        0     9224 2023-12-18 12:05:45.500727 gigachain_community-0.0.6/langchain_community/callbacks/infino_callback.py
--rw-r--r--   0        0        0    13880 2023-12-18 12:05:45.501822 gigachain_community-0.0.6/langchain_community/callbacks/labelstudio_callback.py
--rw-r--r--   0        0        0    20527 2023-12-18 12:05:45.502476 gigachain_community-0.0.6/langchain_community/callbacks/llmonitor_callback.py
--rw-r--r--   0        0        0     1891 2023-12-18 12:05:45.503349 gigachain_community-0.0.6/langchain_community/callbacks/manager.py
--rw-r--r--   0        0        0    24156 2023-12-18 12:05:45.503686 gigachain_community-0.0.6/langchain_community/callbacks/mlflow_callback.py
--rw-r--r--   0        0        0     7309 2023-12-18 12:05:45.504428 gigachain_community-0.0.6/langchain_community/callbacks/openai_info.py
--rw-r--r--   0        0        0     5535 2023-12-18 12:05:45.505111 gigachain_community-0.0.6/langchain_community/callbacks/promptlayer_callback.py
--rw-r--r--   0        0        0     8758 2023-12-18 12:05:45.506012 gigachain_community-0.0.6/langchain_community/callbacks/sagemaker_callback.py
--rw-r--r--   0        0        0     3211 2023-12-18 12:05:45.506509 gigachain_community-0.0.6/langchain_community/callbacks/streamlit/__init__.py
--rw-r--r--   0        0        0     5435 2023-12-18 12:05:45.507080 gigachain_community-0.0.6/langchain_community/callbacks/streamlit/mutable_expander.py
--rw-r--r--   0        0        0    15534 2023-12-18 12:05:45.507739 gigachain_community-0.0.6/langchain_community/callbacks/streamlit/streamlit_callback_handler.py
--rw-r--r--   0        0        0      498 2023-12-18 12:05:45.508143 gigachain_community-0.0.6/langchain_community/callbacks/tracers/__init__.py
--rw-r--r--   0        0        0     4713 2023-12-21 15:51:51.778605 gigachain_community-0.0.6/langchain_community/callbacks/tracers/comet.py
--rw-r--r--   0        0        0    19114 2023-12-18 12:05:45.509395 gigachain_community-0.0.6/langchain_community/callbacks/tracers/wandb.py
--rw-r--r--   0        0        0     4526 2023-12-18 12:05:45.510089 gigachain_community-0.0.6/langchain_community/callbacks/trubrics_callback.py
--rw-r--r--   0        0        0     8505 2023-12-18 12:05:45.510787 gigachain_community-0.0.6/langchain_community/callbacks/utils.py
--rw-r--r--   0        0        0    20601 2023-12-18 12:05:45.511652 gigachain_community-0.0.6/langchain_community/callbacks/wandb_callback.py
--rw-r--r--   0        0        0     8067 2023-12-18 12:05:45.512609 gigachain_community-0.0.6/langchain_community/callbacks/whylabs_callback.py
--rw-r--r--   0        0        0      452 2023-12-18 12:05:45.513350 gigachain_community-0.0.6/langchain_community/chat_loaders/__init__.py
--rw-r--r--   0        0        0      444 2023-12-18 12:05:45.513788 gigachain_community-0.0.6/langchain_community/chat_loaders/base.py
--rw-r--r--   0        0        0     2462 2023-12-18 12:05:45.514215 gigachain_community-0.0.6/langchain_community/chat_loaders/facebook_messenger.py
--rw-r--r--   0        0        0     4048 2023-12-18 12:05:45.514652 gigachain_community-0.0.6/langchain_community/chat_loaders/gmail.py
--rw-r--r--   0        0        0     6768 2023-12-21 15:51:51.779551 gigachain_community-0.0.6/langchain_community/chat_loaders/imessage.py
--rw-r--r--   0        0        0     5742 2023-12-18 12:05:45.515939 gigachain_community-0.0.6/langchain_community/chat_loaders/langsmith.py
--rw-r--r--   0        0        0     3112 2023-12-18 12:05:45.516606 gigachain_community-0.0.6/langchain_community/chat_loaders/slack.py
--rw-r--r--   0        0        0     5390 2023-12-18 12:05:45.517563 gigachain_community-0.0.6/langchain_community/chat_loaders/telegram.py
--rw-r--r--   0        0        0     3270 2023-12-18 12:05:45.517951 gigachain_community-0.0.6/langchain_community/chat_loaders/utils.py
--rw-r--r--   0        0        0     4280 2023-12-18 12:05:45.518507 gigachain_community-0.0.6/langchain_community/chat_loaders/whatsapp.py
--rw-r--r--   0        0        0     2570 2023-12-18 12:05:45.519149 gigachain_community-0.0.6/langchain_community/chat_message_histories/__init__.py
--rw-r--r--   0        0        0     4127 2023-12-18 12:05:45.519995 gigachain_community-0.0.6/langchain_community/chat_message_histories/astradb.py
--rw-r--r--   0        0        0     2392 2023-12-18 12:05:45.520478 gigachain_community-0.0.6/langchain_community/chat_message_histories/cassandra.py
--rw-r--r--   0        0        0     6510 2023-12-18 12:05:45.521121 gigachain_community-0.0.6/langchain_community/chat_message_histories/cosmos_db.py
--rw-r--r--   0        0        0     5810 2023-12-18 12:05:45.521680 gigachain_community-0.0.6/langchain_community/chat_message_histories/dynamodb.py
--rw-r--r--   0        0        0     6836 2023-12-28 13:38:34.455277 gigachain_community-0.0.6/langchain_community/chat_message_histories/elasticsearch.py
--rw-r--r--   0        0        0     1379 2023-12-18 12:05:45.522767 gigachain_community-0.0.6/langchain_community/chat_message_histories/file.py
--rw-r--r--   0        0        0     3349 2023-12-18 12:05:45.523479 gigachain_community-0.0.6/langchain_community/chat_message_histories/firestore.py
--rw-r--r--   0        0        0      633 2023-12-18 12:05:45.524050 gigachain_community-0.0.6/langchain_community/chat_message_histories/in_memory.py
--rw-r--r--   0        0        0     7112 2023-12-18 12:05:45.524641 gigachain_community-0.0.6/langchain_community/chat_message_histories/momento.py
--rw-r--r--   0        0        0     2734 2023-12-18 12:05:45.524978 gigachain_community-0.0.6/langchain_community/chat_message_histories/mongodb.py
--rw-r--r--   0        0        0     4288 2023-12-18 12:05:45.525750 gigachain_community-0.0.6/langchain_community/chat_message_histories/neo4j.py
--rw-r--r--   0        0        0     2659 2023-12-18 12:05:45.526184 gigachain_community-0.0.6/langchain_community/chat_message_histories/postgres.py
--rw-r--r--   0        0        0     1971 2023-12-18 12:05:45.526547 gigachain_community-0.0.6/langchain_community/chat_message_histories/redis.py
--rw-r--r--   0        0        0     9515 2023-12-18 12:05:45.526952 gigachain_community-0.0.6/langchain_community/chat_message_histories/rocksetdb.py
--rw-r--r--   0        0        0    10331 2023-12-18 12:05:45.527836 gigachain_community-0.0.6/langchain_community/chat_message_histories/singlestoredb.py
--rw-r--r--   0        0        0     4717 2023-12-18 12:05:45.528385 gigachain_community-0.0.6/langchain_community/chat_message_histories/sql.py
--rw-r--r--   0        0        0     1176 2023-12-18 12:05:45.528853 gigachain_community-0.0.6/langchain_community/chat_message_histories/streamlit.py
--rw-r--r--   0        0        0     2148 2023-12-18 12:05:45.529276 gigachain_community-0.0.6/langchain_community/chat_message_histories/upstash_redis.py
--rw-r--r--   0        0        0     4652 2023-12-18 12:05:45.529848 gigachain_community-0.0.6/langchain_community/chat_message_histories/xata.py
--rw-r--r--   0        0        0     6452 2023-12-18 12:05:45.530494 gigachain_community-0.0.6/langchain_community/chat_message_histories/zep.py
--rw-r--r--   0        0        0     3403 2023-12-28 13:38:34.456648 gigachain_community-0.0.6/langchain_community/chat_models/__init__.py
--rw-r--r--   0        0        0     7963 2023-12-18 12:05:45.531534 gigachain_community-0.0.6/langchain_community/chat_models/anthropic.py
--rw-r--r--   0        0        0     7945 2023-12-18 12:05:45.532200 gigachain_community-0.0.6/langchain_community/chat_models/anyscale.py
--rw-r--r--   0        0        0    11171 2023-12-28 13:38:34.458109 gigachain_community-0.0.6/langchain_community/chat_models/azure_openai.py
--rw-r--r--   0        0        0     6007 2023-12-18 12:05:45.533360 gigachain_community-0.0.6/langchain_community/chat_models/azureml_endpoint.py
--rw-r--r--   0        0        0    10083 2023-12-18 12:05:45.534129 gigachain_community-0.0.6/langchain_community/chat_models/baichuan.py
--rw-r--r--   0        0        0    12467 2023-12-21 15:51:51.781739 gigachain_community-0.0.6/langchain_community/chat_models/baidu_qianfan_endpoint.py
--rw-r--r--   0        0        0     4284 2023-12-18 12:05:45.535676 gigachain_community-0.0.6/langchain_community/chat_models/bedrock.py
--rw-r--r--   0        0        0     7571 2023-12-18 12:05:45.536327 gigachain_community-0.0.6/langchain_community/chat_models/cohere.py
--rw-r--r--   0        0        0     1250 2023-12-18 12:05:45.537272 gigachain_community-0.0.6/langchain_community/chat_models/databricks.py
--rw-r--r--   0        0        0     7874 2023-12-18 12:05:45.537817 gigachain_community-0.0.6/langchain_community/chat_models/ernie.py
--rw-r--r--   0        0        0     5586 2023-12-18 12:05:45.538348 gigachain_community-0.0.6/langchain_community/chat_models/everlyai.py
--rw-r--r--   0        0        0     3217 2023-12-18 12:05:45.538739 gigachain_community-0.0.6/langchain_community/chat_models/fake.py
--rw-r--r--   0        0        0    11742 2023-12-21 15:51:51.782873 gigachain_community-0.0.6/langchain_community/chat_models/fireworks.py
--rw-r--r--   0        0        0     6225 2023-12-21 15:51:51.785824 gigachain_community-0.0.6/langchain_community/chat_models/gigachat.py
--rw-r--r--   0        0        0    11526 2023-12-18 12:05:45.540634 gigachain_community-0.0.6/langchain_community/chat_models/google_palm.py
--rw-r--r--   0        0        0    12749 2023-12-28 13:38:34.459453 gigachain_community-0.0.6/langchain_community/chat_models/gpt_router.py
--rw-r--r--   0        0        0     5549 2023-12-28 13:38:34.459951 gigachain_community-0.0.6/langchain_community/chat_models/huggingface.py
--rw-r--r--   0        0        0     4202 2023-12-18 12:05:45.541184 gigachain_community-0.0.6/langchain_community/chat_models/human.py
--rw-r--r--   0        0        0    10549 2023-12-18 12:05:45.541892 gigachain_community-0.0.6/langchain_community/chat_models/hunyuan.py
--rw-r--r--   0        0        0     7654 2023-12-18 12:05:45.542512 gigachain_community-0.0.6/langchain_community/chat_models/javelin_ai_gateway.py
--rw-r--r--   0        0        0    15167 2023-12-18 12:05:45.542994 gigachain_community-0.0.6/langchain_community/chat_models/jinachat.py
--rw-r--r--   0        0        0    10588 2023-12-18 12:05:45.543497 gigachain_community-0.0.6/langchain_community/chat_models/konko.py
--rw-r--r--   0        0        0    15671 2023-12-18 12:05:45.544541 gigachain_community-0.0.6/langchain_community/chat_models/litellm.py
--rw-r--r--   0        0        0      967 2023-12-21 15:51:51.787479 gigachain_community-0.0.6/langchain_community/chat_models/meta.py
--rw-r--r--   0        0        0     3180 2023-12-18 12:05:45.545432 gigachain_community-0.0.6/langchain_community/chat_models/minimax.py
--rw-r--r--   0        0        0     7412 2023-12-18 12:05:45.546073 gigachain_community-0.0.6/langchain_community/chat_models/mlflow.py
--rw-r--r--   0        0        0     7241 2023-12-18 12:05:45.546694 gigachain_community-0.0.6/langchain_community/chat_models/mlflow_ai_gateway.py
--rw-r--r--   0        0        0    13165 2023-12-28 13:38:34.460887 gigachain_community-0.0.6/langchain_community/chat_models/ollama.py
--rw-r--r--   0        0        0    26580 2023-12-21 15:51:51.789695 gigachain_community-0.0.6/langchain_community/chat_models/openai.py
--rw-r--r--   0        0        0    11281 2023-12-18 12:05:45.550648 gigachain_community-0.0.6/langchain_community/chat_models/pai_eas_endpoint.py
--rw-r--r--   0        0        0     5261 2023-12-18 12:05:45.551381 gigachain_community-0.0.6/langchain_community/chat_models/promptlayer_openai.py
--rw-r--r--   0        0        0    14047 2023-12-21 15:51:51.793738 gigachain_community-0.0.6/langchain_community/chat_models/tongyi.py
--rw-r--r--   0        0        0    14385 2023-12-28 13:38:34.462031 gigachain_community-0.0.6/langchain_community/chat_models/vertexai.py
--rw-r--r--   0        0        0     5119 2023-12-21 15:51:51.797089 gigachain_community-0.0.6/langchain_community/chat_models/volcengine_maas.py
--rw-r--r--   0        0        0     9392 2023-12-21 15:51:51.798113 gigachain_community-0.0.6/langchain_community/chat_models/yandex.py
--rw-r--r--   0        0        0      549 2023-12-18 12:05:45.555730 gigachain_community-0.0.6/langchain_community/docstore/__init__.py
--rw-r--r--   0        0        0     1090 2023-12-18 12:05:45.556119 gigachain_community-0.0.6/langchain_community/docstore/arbitrary_fn.py
--rw-r--r--   0        0        0      833 2023-12-18 12:05:45.556954 gigachain_community-0.0.6/langchain_community/docstore/base.py
--rw-r--r--   0        0        0       70 2023-12-18 12:05:45.557366 gigachain_community-0.0.6/langchain_community/docstore/document.py
--rw-r--r--   0        0        0     1610 2023-12-18 12:05:45.557773 gigachain_community-0.0.6/langchain_community/docstore/in_memory.py
--rw-r--r--   0        0        0     1487 2023-12-18 12:05:45.558219 gigachain_community-0.0.6/langchain_community/docstore/wikipedia.py
--rw-r--r--   0        0        0    16095 2023-12-28 13:38:34.463521 gigachain_community-0.0.6/langchain_community/document_loaders/__init__.py
--rw-r--r--   0        0        0     2841 2023-12-18 12:05:45.559522 gigachain_community-0.0.6/langchain_community/document_loaders/acreom.py
--rw-r--r--   0        0        0    10240 2023-12-18 12:05:45.560037 gigachain_community-0.0.6/langchain_community/document_loaders/airbyte.py
--rw-r--r--   0        0        0      815 2023-12-18 12:05:45.560483 gigachain_community-0.0.6/langchain_community/document_loaders/airbyte_json.py
--rw-r--r--   0        0        0     1281 2023-12-18 12:05:45.560843 gigachain_community-0.0.6/langchain_community/document_loaders/airtable.py
--rw-r--r--   0        0        0     2759 2023-12-18 12:05:45.561222 gigachain_community-0.0.6/langchain_community/document_loaders/apify_dataset.py
--rw-r--r--   0        0        0     5272 2023-12-18 12:05:45.561756 gigachain_community-0.0.6/langchain_community/document_loaders/arcgis_loader.py
--rw-r--r--   0        0        0      879 2023-12-28 13:38:34.464672 gigachain_community-0.0.6/langchain_community/document_loaders/arxiv.py
--rw-r--r--   0        0        0     4218 2023-12-18 12:05:45.562628 gigachain_community-0.0.6/langchain_community/document_loaders/assemblyai.py
--rw-r--r--   0        0        0     8129 2023-12-18 12:05:45.563265 gigachain_community-0.0.6/langchain_community/document_loaders/async_html.py
--rw-r--r--   0        0        0      563 2023-12-18 12:05:45.563932 gigachain_community-0.0.6/langchain_community/document_loaders/azlyrics.py
--rw-r--r--   0        0        0     1545 2023-12-18 12:05:45.564679 gigachain_community-0.0.6/langchain_community/document_loaders/azure_ai_data.py
--rw-r--r--   0        0        0     1582 2023-12-18 12:05:45.565135 gigachain_community-0.0.6/langchain_community/document_loaders/azure_blob_storage_container.py
--rw-r--r--   0        0        0     1644 2023-12-18 12:05:45.565693 gigachain_community-0.0.6/langchain_community/document_loaders/azure_blob_storage_file.py
--rw-r--r--   0        0        0     1857 2023-12-18 12:05:45.566128 gigachain_community-0.0.6/langchain_community/document_loaders/baiducloud_bos_directory.py
--rw-r--r--   0        0        0     1931 2023-12-18 12:05:45.566645 gigachain_community-0.0.6/langchain_community/document_loaders/baiducloud_bos_file.py
--rw-r--r--   0        0        0     3175 2023-12-18 12:05:45.567038 gigachain_community-0.0.6/langchain_community/document_loaders/base.py
--rw-r--r--   0        0        0     6992 2023-12-18 12:05:45.567647 gigachain_community-0.0.6/langchain_community/document_loaders/base_o365.py
--rw-r--r--   0        0        0     3922 2023-12-18 12:05:45.568154 gigachain_community-0.0.6/langchain_community/document_loaders/bibtex.py
--rw-r--r--   0        0        0     3673 2023-12-18 12:05:45.568593 gigachain_community-0.0.6/langchain_community/document_loaders/bigquery.py
--rw-r--r--   0        0        0     2736 2023-12-18 12:05:45.569329 gigachain_community-0.0.6/langchain_community/document_loaders/bilibili.py
--rw-r--r--   0        0        0    10302 2023-12-18 12:05:45.569842 gigachain_community-0.0.6/langchain_community/document_loaders/blackboard.py
--rw-r--r--   0        0        0      374 2023-12-18 12:05:45.570390 gigachain_community-0.0.6/langchain_community/document_loaders/blob_loaders/__init__.py
--rw-r--r--   0        0        0     5340 2023-12-18 12:05:45.571009 gigachain_community-0.0.6/langchain_community/document_loaders/blob_loaders/file_system.py
--rw-r--r--   0        0        0     6636 2023-12-18 12:05:45.571991 gigachain_community-0.0.6/langchain_community/document_loaders/blob_loaders/schema.py
--rw-r--r--   0        0        0     1526 2023-12-18 12:05:45.572418 gigachain_community-0.0.6/langchain_community/document_loaders/blob_loaders/youtube_audio.py
--rw-r--r--   0        0        0     5709 2023-12-18 12:05:45.573013 gigachain_community-0.0.6/langchain_community/document_loaders/blockchain.py
--rw-r--r--   0        0        0     1047 2023-12-18 12:05:45.573408 gigachain_community-0.0.6/langchain_community/document_loaders/brave_search.py
--rw-r--r--   0        0        0     2124 2023-12-18 12:05:45.573742 gigachain_community-0.0.6/langchain_community/document_loaders/browserless.py
--rw-r--r--   0        0        0     1986 2023-12-18 12:05:45.574097 gigachain_community-0.0.6/langchain_community/document_loaders/chatgpt.py
--rw-r--r--   0        0        0     2746 2023-12-18 12:05:45.574483 gigachain_community-0.0.6/langchain_community/document_loaders/chromium.py
--rw-r--r--   0        0        0      527 2023-12-18 12:05:45.575010 gigachain_community-0.0.6/langchain_community/document_loaders/college_confidential.py
--rw-r--r--   0        0        0     3269 2023-12-18 12:05:45.575773 gigachain_community-0.0.6/langchain_community/document_loaders/concurrent.py
--rw-r--r--   0        0        0    27612 2023-12-18 12:05:45.576326 gigachain_community-0.0.6/langchain_community/document_loaders/confluence.py
--rw-r--r--   0        0        0     1052 2023-12-18 12:05:45.576792 gigachain_community-0.0.6/langchain_community/document_loaders/conllu.py
--rw-r--r--   0        0        0     3649 2023-12-18 12:05:45.577211 gigachain_community-0.0.6/langchain_community/document_loaders/couchbase.py
--rw-r--r--   0        0        0     5926 2023-12-18 12:05:45.577752 gigachain_community-0.0.6/langchain_community/document_loaders/csv_loader.py
--rw-r--r--   0        0        0     6617 2023-12-18 12:05:45.578545 gigachain_community-0.0.6/langchain_community/document_loaders/cube_semantic.py
--rw-r--r--   0        0        0     4937 2023-12-18 12:05:45.579652 gigachain_community-0.0.6/langchain_community/document_loaders/datadog_logs.py
--rw-r--r--   0        0        0     1923 2023-12-18 12:05:45.580180 gigachain_community-0.0.6/langchain_community/document_loaders/dataframe.py
--rw-r--r--   0        0        0     2054 2023-12-18 12:05:45.580587 gigachain_community-0.0.6/langchain_community/document_loaders/diffbot.py
--rw-r--r--   0        0        0     5942 2023-12-28 13:38:34.465530 gigachain_community-0.0.6/langchain_community/document_loaders/directory.py
--rw-r--r--   0        0        0     1237 2023-12-18 12:05:45.581567 gigachain_community-0.0.6/langchain_community/document_loaders/discord.py
--rw-r--r--   0        0        0     3146 2023-12-28 13:38:34.466027 gigachain_community-0.0.6/langchain_community/document_loaders/doc_intelligence.py
--rw-r--r--   0        0        0    13450 2023-12-18 12:05:45.582298 gigachain_community-0.0.6/langchain_community/document_loaders/docugami.py
--rw-r--r--   0        0        0     1852 2023-12-21 15:51:51.799258 gigachain_community-0.0.6/langchain_community/document_loaders/docusaurus.py
--rw-r--r--   0        0        0     6229 2023-12-18 12:05:45.583083 gigachain_community-0.0.6/langchain_community/document_loaders/dropbox.py
--rw-r--r--   0        0        0     3150 2023-12-18 12:05:45.583436 gigachain_community-0.0.6/langchain_community/document_loaders/duckdb_loader.py
--rw-r--r--   0        0        0     3834 2023-12-18 12:05:45.583873 gigachain_community-0.0.6/langchain_community/document_loaders/email.py
--rw-r--r--   0        0        0     1496 2023-12-18 12:05:45.584255 gigachain_community-0.0.6/langchain_community/document_loaders/epub.py
--rw-r--r--   0        0        0     7798 2023-12-18 12:05:45.584871 gigachain_community-0.0.6/langchain_community/document_loaders/etherscan.py
--rw-r--r--   0        0        0     5757 2023-12-18 12:05:45.585493 gigachain_community-0.0.6/langchain_community/document_loaders/evernote.py
--rw-r--r--   0        0        0     1687 2023-12-18 12:05:45.585995 gigachain_community-0.0.6/langchain_community/document_loaders/excel.py
--rw-r--r--   0        0        0     1270 2023-12-18 12:05:45.586905 gigachain_community-0.0.6/langchain_community/document_loaders/facebook_chat.py
--rw-r--r--   0        0        0     2254 2023-12-18 12:05:45.587314 gigachain_community-0.0.6/langchain_community/document_loaders/fauna.py
--rw-r--r--   0        0        0     1543 2023-12-18 12:05:45.587742 gigachain_community-0.0.6/langchain_community/document_loaders/figma.py
--rw-r--r--   0        0        0     2118 2023-12-18 12:05:45.588204 gigachain_community-0.0.6/langchain_community/document_loaders/gcs_directory.py
--rw-r--r--   0        0        0     3138 2023-12-28 13:38:34.466902 gigachain_community-0.0.6/langchain_community/document_loaders/gcs_file.py
--rw-r--r--   0        0        0     6390 2023-12-18 12:05:45.589033 gigachain_community-0.0.6/langchain_community/document_loaders/generic.py
--rw-r--r--   0        0        0     2518 2023-12-18 12:05:45.589513 gigachain_community-0.0.6/langchain_community/document_loaders/geodataframe.py
--rw-r--r--   0        0        0     4116 2023-12-18 12:05:45.590181 gigachain_community-0.0.6/langchain_community/document_loaders/git.py
--rw-r--r--   0        0        0     3453 2023-12-18 12:05:45.590495 gigachain_community-0.0.6/langchain_community/document_loaders/gitbook.py
--rw-r--r--   0        0        0     6973 2023-12-18 12:05:45.590928 gigachain_community-0.0.6/langchain_community/document_loaders/github.py
--rw-r--r--   0        0        0     5096 2023-12-18 12:05:45.591407 gigachain_community-0.0.6/langchain_community/document_loaders/google_speech_to_text.py
--rw-r--r--   0        0        0    14225 2023-12-18 12:05:45.592229 gigachain_community-0.0.6/langchain_community/document_loaders/googledrive.py
--rw-r--r--   0        0        0      928 2023-12-18 12:05:45.592507 gigachain_community-0.0.6/langchain_community/document_loaders/gutenberg.py
--rw-r--r--   0        0        0     1557 2023-12-18 12:05:45.592815 gigachain_community-0.0.6/langchain_community/document_loaders/helpers.py
--rw-r--r--   0        0        0     2075 2023-12-18 12:05:45.593049 gigachain_community-0.0.6/langchain_community/document_loaders/hn.py
--rw-r--r--   0        0        0     1158 2023-12-18 12:05:45.593334 gigachain_community-0.0.6/langchain_community/document_loaders/html.py
--rw-r--r--   0        0        0     2045 2023-12-28 13:38:34.467659 gigachain_community-0.0.6/langchain_community/document_loaders/html_bs.py
--rw-r--r--   0        0        0     3208 2023-12-18 12:05:45.594186 gigachain_community-0.0.6/langchain_community/document_loaders/hugging_face_dataset.py
--rw-r--r--   0        0        0     7642 2023-12-18 12:05:45.594633 gigachain_community-0.0.6/langchain_community/document_loaders/ifixit.py
--rw-r--r--   0        0        0     1173 2023-12-18 12:05:45.595279 gigachain_community-0.0.6/langchain_community/document_loaders/image.py
--rw-r--r--   0        0        0     3594 2023-12-18 12:05:45.596852 gigachain_community-0.0.6/langchain_community/document_loaders/image_captions.py
--rw-r--r--   0        0        0      477 2023-12-18 12:05:45.597367 gigachain_community-0.0.6/langchain_community/document_loaders/imsdb.py
--rw-r--r--   0        0        0     1688 2023-12-18 12:05:45.597983 gigachain_community-0.0.6/langchain_community/document_loaders/iugu.py
--rw-r--r--   0        0        0     3705 2023-12-18 12:05:45.598689 gigachain_community-0.0.6/langchain_community/document_loaders/joplin.py
--rw-r--r--   0        0        0     5907 2023-12-18 12:05:45.599520 gigachain_community-0.0.6/langchain_community/document_loaders/json_loader.py
--rw-r--r--   0        0        0     6058 2023-12-21 15:51:51.800637 gigachain_community-0.0.6/langchain_community/document_loaders/lakefs.py
--rw-r--r--   0        0        0     2008 2023-12-18 12:05:45.600876 gigachain_community-0.0.6/langchain_community/document_loaders/larksuite.py
--rw-r--r--   0        0        0     1818 2023-12-28 13:38:34.468309 gigachain_community-0.0.6/langchain_community/document_loaders/markdown.py
--rw-r--r--   0        0        0     3112 2023-12-18 12:05:45.601726 gigachain_community-0.0.6/langchain_community/document_loaders/mastodon.py
--rw-r--r--   0        0        0     3282 2023-12-18 12:05:45.602072 gigachain_community-0.0.6/langchain_community/document_loaders/max_compute.py
--rw-r--r--   0        0        0     3455 2023-12-18 12:05:45.602561 gigachain_community-0.0.6/langchain_community/document_loaders/mediawikidump.py
--rw-r--r--   0        0        0      846 2023-12-18 12:05:45.602927 gigachain_community-0.0.6/langchain_community/document_loaders/merge.py
--rw-r--r--   0        0        0     2540 2023-12-28 13:38:34.469196 gigachain_community-0.0.6/langchain_community/document_loaders/mhtml.py
--rw-r--r--   0        0        0     3074 2023-12-18 12:05:45.603564 gigachain_community-0.0.6/langchain_community/document_loaders/modern_treasury.py
--rw-r--r--   0        0        0     2522 2023-12-18 12:05:45.604001 gigachain_community-0.0.6/langchain_community/document_loaders/mongodb.py
--rw-r--r--   0        0        0     4296 2023-12-18 12:05:45.604511 gigachain_community-0.0.6/langchain_community/document_loaders/news.py
--rw-r--r--   0        0        0     4301 2023-12-18 12:05:45.605118 gigachain_community-0.0.6/langchain_community/document_loaders/notebook.py
--rw-r--r--   0        0        0      814 2023-12-18 12:05:45.605522 gigachain_community-0.0.6/langchain_community/document_loaders/notion.py
--rw-r--r--   0        0        0     6718 2023-12-18 12:05:45.606331 gigachain_community-0.0.6/langchain_community/document_loaders/notiondb.py
--rw-r--r--   0        0        0     1088 2023-12-18 12:05:45.606811 gigachain_community-0.0.6/langchain_community/document_loaders/nuclia.py
--rw-r--r--   0        0        0     3593 2023-12-18 12:05:45.607288 gigachain_community-0.0.6/langchain_community/document_loaders/obs_directory.py
--rw-r--r--   0        0        0     4768 2023-12-18 12:05:45.607862 gigachain_community-0.0.6/langchain_community/document_loaders/obs_file.py
--rw-r--r--   0        0        0     6150 2023-12-18 12:05:45.608389 gigachain_community-0.0.6/langchain_community/document_loaders/obsidian.py
--rw-r--r--   0        0        0     1770 2023-12-18 12:05:45.608973 gigachain_community-0.0.6/langchain_community/document_loaders/odt.py
--rw-r--r--   0        0        0     3381 2023-12-18 12:05:45.609740 gigachain_community-0.0.6/langchain_community/document_loaders/onedrive.py
--rw-r--r--   0        0        0     1154 2023-12-18 12:05:45.610167 gigachain_community-0.0.6/langchain_community/document_loaders/onedrive_file.py
--rw-r--r--   0        0        0     8074 2023-12-18 12:05:45.610777 gigachain_community-0.0.6/langchain_community/document_loaders/onenote.py
--rw-r--r--   0        0        0     1331 2023-12-18 12:05:45.611177 gigachain_community-0.0.6/langchain_community/document_loaders/open_city_data.py
--rw-r--r--   0        0        0     1748 2023-12-18 12:05:45.611624 gigachain_community-0.0.6/langchain_community/document_loaders/org_mode.py
--rw-r--r--   0        0        0      947 2023-12-28 13:38:34.470016 gigachain_community-0.0.6/langchain_community/document_loaders/parsers/__init__.py
--rw-r--r--   0        0        0    10716 2023-12-18 12:05:45.612771 gigachain_community-0.0.6/langchain_community/document_loaders/parsers/audio.py
--rw-r--r--   0        0        0     4534 2023-12-28 13:38:34.470440 gigachain_community-0.0.6/langchain_community/document_loaders/parsers/doc_intelligence.py
--rw-r--r--   0        0        0    15283 2023-12-18 12:05:45.613557 gigachain_community-0.0.6/langchain_community/document_loaders/parsers/docai.py
--rw-r--r--   0        0        0     2502 2023-12-18 12:05:45.614020 gigachain_community-0.0.6/langchain_community/document_loaders/parsers/generic.py
--rw-r--r--   0        0        0     5767 2023-12-18 12:05:45.614963 gigachain_community-0.0.6/langchain_community/document_loaders/parsers/grobid.py
--rw-r--r--   0        0        0      109 2023-12-18 12:05:45.615405 gigachain_community-0.0.6/langchain_community/document_loaders/parsers/html/__init__.py
--rw-r--r--   0        0        0     1609 2023-12-18 12:05:45.615795 gigachain_community-0.0.6/langchain_community/document_loaders/parsers/html/bs4.py
--rw-r--r--   0        0        0      136 2023-12-18 12:05:45.616382 gigachain_community-0.0.6/langchain_community/document_loaders/parsers/language/__init__.py
--rw-r--r--   0        0        0     3745 2023-12-18 12:05:45.616807 gigachain_community-0.0.6/langchain_community/document_loaders/parsers/language/cobol.py
--rw-r--r--   0        0        0      495 2023-12-18 12:05:45.617260 gigachain_community-0.0.6/langchain_community/document_loaders/parsers/language/code_segmenter.py
--rw-r--r--   0        0        0     2103 2023-12-18 12:05:45.617642 gigachain_community-0.0.6/langchain_community/document_loaders/parsers/language/javascript.py
--rw-r--r--   0        0        0     5114 2023-12-18 12:05:45.618562 gigachain_community-0.0.6/langchain_community/document_loaders/parsers/language/language_parser.py
--rw-r--r--   0        0        0     1679 2023-12-18 12:05:45.618918 gigachain_community-0.0.6/langchain_community/document_loaders/parsers/language/python.py
--rw-r--r--   0        0        0     1664 2023-12-18 12:05:45.619356 gigachain_community-0.0.6/langchain_community/document_loaders/parsers/msword.py
--rw-r--r--   0        0        0    21006 2023-12-28 13:38:34.472391 gigachain_community-0.0.6/langchain_community/document_loaders/parsers/pdf.py
--rw-r--r--   0        0        0     1214 2023-12-18 12:05:45.621291 gigachain_community-0.0.6/langchain_community/document_loaders/parsers/registry.py
--rw-r--r--   0        0        0      505 2023-12-18 12:05:45.621708 gigachain_community-0.0.6/langchain_community/document_loaders/parsers/txt.py
--rw-r--r--   0        0        0    26024 2023-12-18 12:05:45.622152 gigachain_community-0.0.6/langchain_community/document_loaders/pdf.py
--rw-r--r--   0        0        0     1161 2023-12-18 12:05:45.622618 gigachain_community-0.0.6/langchain_community/document_loaders/polars_dataframe.py
--rw-r--r--   0        0        0     2508 2023-12-18 12:05:45.623093 gigachain_community-0.0.6/langchain_community/document_loaders/powerpoint.py
--rw-r--r--   0        0        0     1371 2023-12-18 12:05:45.623484 gigachain_community-0.0.6/langchain_community/document_loaders/psychic.py
--rw-r--r--   0        0        0     1172 2023-12-18 12:05:45.623852 gigachain_community-0.0.6/langchain_community/document_loaders/pubmed.py
--rw-r--r--   0        0        0     3388 2023-12-18 12:05:45.624242 gigachain_community-0.0.6/langchain_community/document_loaders/pyspark_dataframe.py
--rw-r--r--   0        0        0      527 2023-12-18 12:05:45.624513 gigachain_community-0.0.6/langchain_community/document_loaders/python.py
--rw-r--r--   0        0        0     8426 2023-12-18 12:05:45.624979 gigachain_community-0.0.6/langchain_community/document_loaders/quip.py
--rw-r--r--   0        0        0     6928 2023-12-18 12:05:45.625504 gigachain_community-0.0.6/langchain_community/document_loaders/readthedocs.py
--rw-r--r--   0        0        0    11591 2023-12-18 12:05:45.626220 gigachain_community-0.0.6/langchain_community/document_loaders/recursive_url_loader.py
--rw-r--r--   0        0        0     4584 2023-12-18 12:05:45.626883 gigachain_community-0.0.6/langchain_community/document_loaders/reddit.py
--rw-r--r--   0        0        0      705 2023-12-18 12:05:45.627281 gigachain_community-0.0.6/langchain_community/document_loaders/roam.py
--rw-r--r--   0        0        0     4604 2023-12-18 12:05:45.627882 gigachain_community-0.0.6/langchain_community/document_loaders/rocksetdb.py
--rw-r--r--   0        0        0     4936 2023-12-28 13:38:34.473933 gigachain_community-0.0.6/langchain_community/document_loaders/rspace.py
--rw-r--r--   0        0        0     4895 2023-12-18 12:05:45.629065 gigachain_community-0.0.6/langchain_community/document_loaders/rss.py
--rw-r--r--   0        0        0     1832 2023-12-18 12:05:45.629524 gigachain_community-0.0.6/langchain_community/document_loaders/rst.py
--rw-r--r--   0        0        0     2061 2023-12-18 12:05:45.629875 gigachain_community-0.0.6/langchain_community/document_loaders/rtf.py
--rw-r--r--   0        0        0     5759 2023-12-18 12:05:45.630757 gigachain_community-0.0.6/langchain_community/document_loaders/s3_directory.py
--rw-r--r--   0        0        0     5412 2023-12-18 12:05:45.631317 gigachain_community-0.0.6/langchain_community/document_loaders/s3_file.py
--rw-r--r--   0        0        0     2318 2023-12-18 12:05:45.631739 gigachain_community-0.0.6/langchain_community/document_loaders/sharepoint.py
--rw-r--r--   0        0        0     8530 2023-12-18 12:05:45.632550 gigachain_community-0.0.6/langchain_community/document_loaders/sitemap.py
--rw-r--r--   0        0        0     4131 2023-12-18 12:05:45.633088 gigachain_community-0.0.6/langchain_community/document_loaders/slack_directory.py
--rw-r--r--   0        0        0     4799 2023-12-18 12:05:45.633700 gigachain_community-0.0.6/langchain_community/document_loaders/snowflake_loader.py
--rw-r--r--   0        0        0     2004 2023-12-18 12:05:45.634087 gigachain_community-0.0.6/langchain_community/document_loaders/spreedly.py
--rw-r--r--   0        0        0      851 2023-12-18 12:05:45.634481 gigachain_community-0.0.6/langchain_community/document_loaders/srt.py
--rw-r--r--   0        0        0     1811 2023-12-18 12:05:45.634845 gigachain_community-0.0.6/langchain_community/document_loaders/stripe.py
--rw-r--r--   0        0        0     9008 2023-12-18 12:05:45.635464 gigachain_community-0.0.6/langchain_community/document_loaders/telegram.py
--rw-r--r--   0        0        0     1783 2023-12-18 12:05:45.635902 gigachain_community-0.0.6/langchain_community/document_loaders/tencent_cos_directory.py
--rw-r--r--   0        0        0     1700 2023-12-28 13:38:34.474832 gigachain_community-0.0.6/langchain_community/document_loaders/tencent_cos_file.py
--rw-r--r--   0        0        0     3024 2023-12-18 12:05:45.636604 gigachain_community-0.0.6/langchain_community/document_loaders/tensorflow_datasets.py
--rw-r--r--   0        0        0     2010 2023-12-18 12:05:45.636912 gigachain_community-0.0.6/langchain_community/document_loaders/text.py
--rw-r--r--   0        0        0      950 2023-12-18 12:05:45.637263 gigachain_community-0.0.6/langchain_community/document_loaders/tomarkdown.py
--rw-r--r--   0        0        0     1572 2023-12-18 12:05:45.637651 gigachain_community-0.0.6/langchain_community/document_loaders/toml.py
--rw-r--r--   0        0        0     6561 2023-12-18 12:05:45.638520 gigachain_community-0.0.6/langchain_community/document_loaders/trello.py
--rw-r--r--   0        0        0     1293 2023-12-18 12:05:45.639113 gigachain_community-0.0.6/langchain_community/document_loaders/tsv.py
--rw-r--r--   0        0        0     3438 2023-12-18 12:05:45.639710 gigachain_community-0.0.6/langchain_community/document_loaders/twitter.py
--rw-r--r--   0        0        0    13793 2023-12-18 12:05:45.640484 gigachain_community-0.0.6/langchain_community/document_loaders/unstructured.py
--rw-r--r--   0        0        0     6019 2023-12-18 12:05:45.641072 gigachain_community-0.0.6/langchain_community/document_loaders/url.py
--rw-r--r--   0        0        0     7590 2023-12-18 12:05:45.641572 gigachain_community-0.0.6/langchain_community/document_loaders/url_playwright.py
--rw-r--r--   0        0        0     6640 2023-12-18 12:05:45.642173 gigachain_community-0.0.6/langchain_community/document_loaders/url_selenium.py
--rw-r--r--   0        0        0     1682 2023-12-18 12:05:45.642509 gigachain_community-0.0.6/langchain_community/document_loaders/weather.py
--rw-r--r--   0        0        0    10164 2023-12-18 12:05:45.643373 gigachain_community-0.0.6/langchain_community/document_loaders/web_base.py
--rw-r--r--   0        0        0     1770 2023-12-18 12:05:45.643807 gigachain_community-0.0.6/langchain_community/document_loaders/whatsapp_chat.py
--rw-r--r--   0        0        0     2142 2023-12-18 12:05:45.644447 gigachain_community-0.0.6/langchain_community/document_loaders/wikipedia.py
--rw-r--r--   0        0        0     4583 2023-12-18 12:05:45.645033 gigachain_community-0.0.6/langchain_community/document_loaders/word_document.py
--rw-r--r--   0        0        0     1489 2023-12-18 12:05:45.645378 gigachain_community-0.0.6/langchain_community/document_loaders/xml.py
--rw-r--r--   0        0        0     1119 2023-12-18 12:05:45.645826 gigachain_community-0.0.6/langchain_community/document_loaders/xorbits.py
--rw-r--r--   0        0        0    14798 2023-12-18 12:05:45.647523 gigachain_community-0.0.6/langchain_community/document_loaders/youtube.py
--rw-r--r--   0        0        0     1849 2023-12-18 12:05:45.647949 gigachain_community-0.0.6/langchain_community/document_transformers/__init__.py
--rw-r--r--   0        0        0     5214 2023-12-21 15:51:51.802594 gigachain_community-0.0.6/langchain_community/document_transformers/beautiful_soup_transformer.py
--rw-r--r--   0        0        0     3469 2023-12-18 12:05:45.648810 gigachain_community-0.0.6/langchain_community/document_transformers/doctran_text_extract.py
--rw-r--r--   0        0        0     2193 2023-12-18 12:05:45.649227 gigachain_community-0.0.6/langchain_community/document_transformers/doctran_text_qa.py
--rw-r--r--   0        0        0     2337 2023-12-18 12:05:45.649692 gigachain_community-0.0.6/langchain_community/document_transformers/doctran_text_translate.py
--rw-r--r--   0        0        0     7882 2023-12-18 12:05:45.650106 gigachain_community-0.0.6/langchain_community/document_transformers/embeddings_redundant_filter.py
--rw-r--r--   0        0        0     4133 2023-12-18 12:05:45.650606 gigachain_community-0.0.6/langchain_community/document_transformers/google_translate.py
--rw-r--r--   0        0        0     1834 2023-12-18 12:05:45.650961 gigachain_community-0.0.6/langchain_community/document_transformers/html2text.py
--rw-r--r--   0        0        0     1410 2023-12-18 12:05:45.653916 gigachain_community-0.0.6/langchain_community/document_transformers/long_context_reorder.py
--rw-r--r--   0        0        0     1475 2023-12-18 12:05:45.654343 gigachain_community-0.0.6/langchain_community/document_transformers/nuclia_text_transform.py
--rw-r--r--   0        0        0     6243 2023-12-18 12:05:45.655195 gigachain_community-0.0.6/langchain_community/document_transformers/openai_functions.py
--rw-r--r--   0        0        0     6033 2023-12-18 12:05:45.656355 gigachain_community-0.0.6/langchain_community/document_transformers/xsl/html_chunks_with_headers.xslt
--rw-r--r--   0        0        0     6534 2023-12-28 13:38:34.477982 gigachain_community-0.0.6/langchain_community/embeddings/__init__.py
--rw-r--r--   0        0        0     9614 2023-12-18 12:05:45.657933 gigachain_community-0.0.6/langchain_community/embeddings/aleph_alpha.py
--rw-r--r--   0        0        0     1865 2023-12-18 12:05:45.658580 gigachain_community-0.0.6/langchain_community/embeddings/awa.py
--rw-r--r--   0        0        0     7063 2023-12-21 15:51:51.803470 gigachain_community-0.0.6/langchain_community/embeddings/azure_openai.py
--rw-r--r--   0        0        0     4827 2023-12-21 15:51:51.804348 gigachain_community-0.0.6/langchain_community/embeddings/baidu_qianfan_endpoint.py
--rw-r--r--   0        0        0     6723 2023-12-18 12:05:45.660498 gigachain_community-0.0.6/langchain_community/embeddings/bedrock.py
--rw-r--r--   0        0        0     2725 2023-12-18 12:05:45.660858 gigachain_community-0.0.6/langchain_community/embeddings/bookend.py
--rw-r--r--   0        0        0     5454 2023-12-18 12:05:45.661406 gigachain_community-0.0.6/langchain_community/embeddings/clarifai.py
--rw-r--r--   0        0        0     2869 2023-12-18 12:05:45.661963 gigachain_community-0.0.6/langchain_community/embeddings/cloudflare_workersai.py
--rw-r--r--   0        0        0     4660 2023-12-18 12:05:45.662561 gigachain_community-0.0.6/langchain_community/embeddings/cohere.py
--rw-r--r--   0        0        0     4956 2023-12-18 12:05:45.663235 gigachain_community-0.0.6/langchain_community/embeddings/dashscope.py
--rw-r--r--   0        0        0     1310 2023-12-18 12:05:45.663728 gigachain_community-0.0.6/langchain_community/embeddings/databricks.py
--rw-r--r--   0        0        0     4426 2023-12-18 12:05:45.664376 gigachain_community-0.0.6/langchain_community/embeddings/deepinfra.py
--rw-r--r--   0        0        0     3564 2023-12-21 15:51:51.805303 gigachain_community-0.0.6/langchain_community/embeddings/edenai.py
--rw-r--r--   0        0        0     8401 2023-12-18 12:05:45.665414 gigachain_community-0.0.6/langchain_community/embeddings/elasticsearch.py
--rw-r--r--   0        0        0     5418 2023-12-28 13:38:34.479313 gigachain_community-0.0.6/langchain_community/embeddings/embaas.py
--rw-r--r--   0        0        0     4859 2023-12-18 12:05:45.667020 gigachain_community-0.0.6/langchain_community/embeddings/ernie.py
--rw-r--r--   0        0        0     1512 2023-12-18 12:05:45.667503 gigachain_community-0.0.6/langchain_community/embeddings/fake.py
--rw-r--r--   0        0        0     3452 2023-12-18 12:05:45.667862 gigachain_community-0.0.6/langchain_community/embeddings/fastembed.py
--rw-r--r--   0        0        0     4096 2023-12-28 13:38:34.481934 gigachain_community-0.0.6/langchain_community/embeddings/gigachat.py
--rw-r--r--   0        0        0     3272 2023-12-18 12:05:45.668242 gigachain_community-0.0.6/langchain_community/embeddings/google_palm.py
--rw-r--r--   0        0        0     1664 2023-12-18 12:05:45.669050 gigachain_community-0.0.6/langchain_community/embeddings/gpt4all.py
--rw-r--r--   0        0        0     5274 2023-12-21 15:51:51.806243 gigachain_community-0.0.6/langchain_community/embeddings/gradient_ai.py
--rw-r--r--   0        0        0    11898 2023-12-18 12:05:45.670340 gigachain_community-0.0.6/langchain_community/embeddings/huggingface.py
--rw-r--r--   0        0        0     3789 2023-12-18 12:05:45.670872 gigachain_community-0.0.6/langchain_community/embeddings/huggingface_hub.py
--rw-r--r--   0        0        0    10260 2023-12-18 12:05:45.671375 gigachain_community-0.0.6/langchain_community/embeddings/infinity.py
--rw-r--r--   0        0        0     3673 2023-12-18 12:05:45.671824 gigachain_community-0.0.6/langchain_community/embeddings/javelin_ai_gateway.py
--rw-r--r--   0        0        0     2607 2023-12-28 13:38:34.482924 gigachain_community-0.0.6/langchain_community/embeddings/jina.py
--rw-r--r--   0        0        0     2873 2023-12-18 12:05:45.672526 gigachain_community-0.0.6/langchain_community/embeddings/johnsnowlabs.py
--rw-r--r--   0        0        0     4163 2023-12-18 12:05:45.673477 gigachain_community-0.0.6/langchain_community/embeddings/llamacpp.py
--rw-r--r--   0        0        0     2096 2023-12-18 12:05:45.673924 gigachain_community-0.0.6/langchain_community/embeddings/llm_rails.py
--rw-r--r--   0        0        0    12261 2023-12-27 10:44:25.850461 gigachain_community-0.0.6/langchain_community/embeddings/localai.py
--rw-r--r--   0        0        0     4798 2023-12-28 13:38:34.484154 gigachain_community-0.0.6/langchain_community/embeddings/minimax.py
--rw-r--r--   0        0        0     2417 2023-12-18 12:05:45.675851 gigachain_community-0.0.6/langchain_community/embeddings/mlflow.py
--rw-r--r--   0        0        0     2479 2023-12-18 12:05:45.676322 gigachain_community-0.0.6/langchain_community/embeddings/mlflow_gateway.py
--rw-r--r--   0        0        0     2384 2023-12-18 12:05:45.678107 gigachain_community-0.0.6/langchain_community/embeddings/modelscope_hub.py
--rw-r--r--   0        0        0     5115 2023-12-18 12:05:45.678704 gigachain_community-0.0.6/langchain_community/embeddings/mosaicml.py
--rw-r--r--   0        0        0     2203 2023-12-18 12:05:45.679072 gigachain_community-0.0.6/langchain_community/embeddings/nlpcloud.py
--rw-r--r--   0        0        0     3420 2023-12-18 12:05:45.679432 gigachain_community-0.0.6/langchain_community/embeddings/octoai_embeddings.py
--rw-r--r--   0        0        0     7691 2023-12-18 12:05:45.680736 gigachain_community-0.0.6/langchain_community/embeddings/ollama.py
--rw-r--r--   0        0        0    29207 2023-12-18 12:05:45.681405 gigachain_community-0.0.6/langchain_community/embeddings/openai.py
--rw-r--r--   0        0        0     7591 2023-12-18 12:05:45.682567 gigachain_community-0.0.6/langchain_community/embeddings/sagemaker_endpoint.py
--rw-r--r--   0        0        0     3807 2023-12-18 12:05:45.683325 gigachain_community-0.0.6/langchain_community/embeddings/self_hosted.py
--rw-r--r--   0        0        0     6589 2023-12-18 12:05:45.684011 gigachain_community-0.0.6/langchain_community/embeddings/self_hosted_hugging_face.py
--rw-r--r--   0        0        0      189 2023-12-18 12:05:45.684427 gigachain_community-0.0.6/langchain_community/embeddings/sentence_transformer.py
--rw-r--r--   0        0        0     3743 2023-12-18 12:05:45.684825 gigachain_community-0.0.6/langchain_community/embeddings/spacy_embeddings.py
--rw-r--r--   0        0        0     2413 2023-12-18 12:05:45.685136 gigachain_community-0.0.6/langchain_community/embeddings/tensorflow_hub.py
--rw-r--r--   0        0        0    13929 2023-12-28 13:38:34.485210 gigachain_community-0.0.6/langchain_community/embeddings/vertexai.py
--rw-r--r--   0        0        0     6255 2023-12-18 12:05:45.687621 gigachain_community-0.0.6/langchain_community/embeddings/voyageai.py
--rw-r--r--   0        0        0     3303 2023-12-18 12:05:45.688334 gigachain_community-0.0.6/langchain_community/embeddings/xinference.py
--rw-r--r--   0        0        0     5934 2023-12-21 15:51:51.807967 gigachain_community-0.0.6/langchain_community/embeddings/yandex.py
--rw-r--r--   0        0        0      930 2023-12-18 12:05:45.688723 gigachain_community-0.0.6/langchain_community/graphs/__init__.py
--rw-r--r--   0        0        0     6961 2023-12-18 12:05:45.689581 gigachain_community-0.0.6/langchain_community/graphs/arangodb_graph.py
--rw-r--r--   0        0        0     5294 2023-12-18 12:05:45.690457 gigachain_community-0.0.6/langchain_community/graphs/falkordb_graph.py
--rw-r--r--   0        0        0     1584 2023-12-18 12:05:45.690984 gigachain_community-0.0.6/langchain_community/graphs/graph_document.py
--rw-r--r--   0        0        0     1008 2023-12-18 12:05:45.691396 gigachain_community-0.0.6/langchain_community/graphs/graph_store.py
--rw-r--r--   0        0        0     2510 2023-12-18 12:05:45.691835 gigachain_community-0.0.6/langchain_community/graphs/hugegraph.py
--rw-r--r--   0        0        0     4227 2023-12-18 12:05:45.692460 gigachain_community-0.0.6/langchain_community/graphs/kuzu_graph.py
--rw-r--r--   0        0        0     1644 2023-12-18 12:05:45.692879 gigachain_community-0.0.6/langchain_community/graphs/memgraph_graph.py
--rw-r--r--   0        0        0     8112 2023-12-18 12:05:45.693526 gigachain_community-0.0.6/langchain_community/graphs/nebula_graph.py
--rw-r--r--   0        0        0     8388 2023-12-18 12:05:45.693954 gigachain_community-0.0.6/langchain_community/graphs/neo4j_graph.py
--rw-r--r--   0        0        0     9398 2023-12-18 12:05:45.694545 gigachain_community-0.0.6/langchain_community/graphs/neptune_graph.py
--rw-r--r--   0        0        0     6545 2023-12-18 12:05:45.695142 gigachain_community-0.0.6/langchain_community/graphs/networkx_graph.py
--rw-r--r--   0        0        0    10118 2023-12-18 12:05:45.695554 gigachain_community-0.0.6/langchain_community/graphs/rdf_graph.py
--rw-r--r--   0        0        0        0 2023-12-18 12:05:45.695817 gigachain_community-0.0.6/langchain_community/indexes/__init__.py
--rw-r--r--   0        0        0    20960 2023-12-18 12:05:45.696278 gigachain_community-0.0.6/langchain_community/indexes/_sql_record_manager.py
--rw-r--r--   0        0        0     5221 2023-12-18 12:05:45.696935 gigachain_community-0.0.6/langchain_community/indexes/base.py
--rw-r--r--   0        0        0    23006 2023-12-28 13:38:34.486291 gigachain_community-0.0.6/langchain_community/llms/__init__.py
--rw-r--r--   0        0        0     5292 2023-12-18 12:05:45.698661 gigachain_community-0.0.6/langchain_community/llms/ai21.py
--rw-r--r--   0        0        0    11493 2023-12-18 12:05:45.699215 gigachain_community-0.0.6/langchain_community/llms/aleph_alpha.py
--rw-r--r--   0        0        0     3061 2023-12-18 12:05:45.699586 gigachain_community-0.0.6/langchain_community/llms/amazon_api_gateway.py
--rw-r--r--   0        0        0    12356 2023-12-18 12:05:45.700279 gigachain_community-0.0.6/langchain_community/llms/anthropic.py
--rw-r--r--   0        0        0    10630 2023-12-18 12:05:45.700779 gigachain_community-0.0.6/langchain_community/llms/anyscale.py
--rw-r--r--   0        0        0     9619 2023-12-21 15:51:51.809621 gigachain_community-0.0.6/langchain_community/llms/aphrodite.py
--rw-r--r--   0        0        0     4356 2023-12-18 12:05:45.701385 gigachain_community-0.0.6/langchain_community/llms/arcee.py
--rw-r--r--   0        0        0     6007 2023-12-18 12:05:45.701968 gigachain_community-0.0.6/langchain_community/llms/aviary.py
--rw-r--r--   0        0        0    10251 2023-12-18 12:05:45.702392 gigachain_community-0.0.6/langchain_community/llms/azureml_endpoint.py
--rw-r--r--   0        0        0     7293 2023-12-21 15:51:51.810589 gigachain_community-0.0.6/langchain_community/llms/baidu_qianfan_endpoint.py
--rw-r--r--   0        0        0     4725 2023-12-18 12:05:45.703913 gigachain_community-0.0.6/langchain_community/llms/bananadev.py
--rw-r--r--   0        0        0     3187 2023-12-28 13:38:34.487169 gigachain_community-0.0.6/langchain_community/llms/baseten.py
--rw-r--r--   0        0        0     9099 2023-12-18 12:05:45.705119 gigachain_community-0.0.6/langchain_community/llms/beam.py
--rw-r--r--   0        0        0    15469 2023-12-28 13:38:34.488257 gigachain_community-0.0.6/langchain_community/llms/bedrock.py
--rw-r--r--   0        0        0     6232 2023-12-18 12:05:45.707024 gigachain_community-0.0.6/langchain_community/llms/bittensor.py
--rw-r--r--   0        0        0     4044 2023-12-18 12:05:45.707481 gigachain_community-0.0.6/langchain_community/llms/cerebriumai.py
--rw-r--r--   0        0        0     3969 2023-12-18 12:05:45.707879 gigachain_community-0.0.6/langchain_community/llms/chatglm.py
--rw-r--r--   0        0        0     7262 2023-12-18 12:05:45.708779 gigachain_community-0.0.6/langchain_community/llms/clarifai.py
--rw-r--r--   0        0        0     4277 2023-12-18 12:05:45.709389 gigachain_community-0.0.6/langchain_community/llms/cloudflare_workersai.py
--rw-r--r--   0        0        0     7970 2023-12-18 12:05:45.710013 gigachain_community-0.0.6/langchain_community/llms/cohere.py
--rw-r--r--   0        0        0     4227 2023-12-18 12:05:45.711016 gigachain_community-0.0.6/langchain_community/llms/ctransformers.py
--rw-r--r--   0        0        0     4135 2023-12-18 12:05:45.712038 gigachain_community-0.0.6/langchain_community/llms/ctranslate2.py
--rw-r--r--   0        0        0    17597 2023-12-28 13:38:34.489750 gigachain_community-0.0.6/langchain_community/llms/databricks.py
--rw-r--r--   0        0        0     7006 2023-12-18 12:05:45.713379 gigachain_community-0.0.6/langchain_community/llms/deepinfra.py
--rw-r--r--   0        0        0     8615 2023-12-28 13:38:34.491881 gigachain_community-0.0.6/langchain_community/llms/deepsparse.py
--rw-r--r--   0        0        0     9463 2023-12-21 15:51:51.811774 gigachain_community-0.0.6/langchain_community/llms/edenai.py
--rw-r--r--   0        0        0     2444 2023-12-18 12:05:45.714846 gigachain_community-0.0.6/langchain_community/llms/fake.py
--rw-r--r--   0        0        0    11773 2023-12-21 15:51:51.813007 gigachain_community-0.0.6/langchain_community/llms/fireworks.py
--rw-r--r--   0        0        0     3762 2023-12-18 12:05:45.715821 gigachain_community-0.0.6/langchain_community/llms/forefrontai.py
--rw-r--r--   0        0        0    10505 2023-12-28 13:38:34.495098 gigachain_community-0.0.6/langchain_community/llms/gigachat.py
--rw-r--r--   0        0        0     8854 2023-12-21 15:51:51.816031 gigachain_community-0.0.6/langchain_community/llms/google_palm.py
--rw-r--r--   0        0        0     5301 2023-12-18 12:05:45.718164 gigachain_community-0.0.6/langchain_community/llms/gooseai.py
--rw-r--r--   0        0        0     6525 2023-12-18 12:05:45.718855 gigachain_community-0.0.6/langchain_community/llms/gpt4all.py
--rw-r--r--   0        0        0    14199 2023-12-18 12:05:45.719653 gigachain_community-0.0.6/langchain_community/llms/gradient_ai.py
--rw-r--r--   0        0        0      664 2023-12-18 12:05:45.720222 gigachain_community-0.0.6/langchain_community/llms/grammars/json.gbnf
--rw-r--r--   0        0        0      167 2023-12-18 12:05:45.720572 gigachain_community-0.0.6/langchain_community/llms/grammars/list.gbnf
--rw-r--r--   0        0        0     5508 2023-12-18 12:05:45.721443 gigachain_community-0.0.6/langchain_community/llms/huggingface_endpoint.py
--rw-r--r--   0        0        0     4658 2023-12-18 12:05:45.721873 gigachain_community-0.0.6/langchain_community/llms/huggingface_hub.py
--rw-r--r--   0        0        0     9215 2023-12-18 12:05:45.722687 gigachain_community-0.0.6/langchain_community/llms/huggingface_pipeline.py
--rw-r--r--   0        0        0    11403 2023-12-18 12:05:45.723462 gigachain_community-0.0.6/langchain_community/llms/huggingface_text_gen_inference.py
--rw-r--r--   0        0        0     2582 2023-12-18 12:05:45.723857 gigachain_community-0.0.6/langchain_community/llms/human.py
--rw-r--r--   0        0        0     4723 2023-12-18 12:05:45.724545 gigachain_community-0.0.6/langchain_community/llms/javelin_ai_gateway.py
--rw-r--r--   0        0        0     5087 2023-12-18 12:05:45.724912 gigachain_community-0.0.6/langchain_community/llms/koboldai.py
--rw-r--r--   0        0        0    12537 2023-12-18 12:05:45.725808 gigachain_community-0.0.6/langchain_community/llms/llamacpp.py
--rw-r--r--   0        0        0     1328 2023-12-18 12:05:45.726192 gigachain_community-0.0.6/langchain_community/llms/loading.py
--rw-r--r--   0        0        0     1965 2023-12-18 12:05:45.726579 gigachain_community-0.0.6/langchain_community/llms/manifest.py
--rw-r--r--   0        0        0     5470 2023-12-18 12:05:45.727040 gigachain_community-0.0.6/langchain_community/llms/minimax.py
--rw-r--r--   0        0        0     3845 2023-12-18 12:05:45.727455 gigachain_community-0.0.6/langchain_community/llms/mlflow.py
--rw-r--r--   0        0        0     3279 2023-12-18 12:05:45.728237 gigachain_community-0.0.6/langchain_community/llms/mlflow_ai_gateway.py
--rw-r--r--   0        0        0     3288 2023-12-18 12:05:45.730018 gigachain_community-0.0.6/langchain_community/llms/modal.py
--rw-r--r--   0        0        0     6150 2023-12-18 12:05:45.730902 gigachain_community-0.0.6/langchain_community/llms/mosaicml.py
--rw-r--r--   0        0        0     5049 2023-12-18 12:05:45.731352 gigachain_community-0.0.6/langchain_community/llms/nlpcloud.py
--rw-r--r--   0        0        0    12162 2023-12-28 13:38:34.495799 gigachain_community-0.0.6/langchain_community/llms/oci_data_science_model_deployment_endpoint.py
--rw-r--r--   0        0        0     5207 2023-12-18 12:05:45.731708 gigachain_community-0.0.6/langchain_community/llms/octoai_endpoint.py
--rw-r--r--   0        0        0    16092 2023-12-28 13:38:34.496966 gigachain_community-0.0.6/langchain_community/llms/ollama.py
--rw-r--r--   0        0        0     3980 2023-12-18 12:05:45.732462 gigachain_community-0.0.6/langchain_community/llms/opaqueprompts.py
--rw-r--r--   0        0        0    47378 2023-12-21 15:51:51.818449 gigachain_community-0.0.6/langchain_community/llms/openai.py
--rw-r--r--   0        0        0    10743 2023-12-18 12:05:45.733474 gigachain_community-0.0.6/langchain_community/llms/openllm.py
--rw-r--r--   0        0        0      902 2023-12-18 12:05:45.733910 gigachain_community-0.0.6/langchain_community/llms/openlm.py
--rw-r--r--   0        0        0     8059 2023-12-18 12:05:45.734279 gigachain_community-0.0.6/langchain_community/llms/pai_eas_endpoint.py
--rw-r--r--   0        0        0     5402 2023-12-28 13:38:34.498208 gigachain_community-0.0.6/langchain_community/llms/petals.py
--rw-r--r--   0        0        0     4182 2023-12-28 13:38:34.499044 gigachain_community-0.0.6/langchain_community/llms/pipelineai.py
--rw-r--r--   0        0        0     1594 2023-12-28 13:38:34.499702 gigachain_community-0.0.6/langchain_community/llms/predibase.py
--rw-r--r--   0        0        0     4410 2023-12-18 12:05:45.735769 gigachain_community-0.0.6/langchain_community/llms/predictionguard.py
--rw-r--r--   0        0        0     8809 2023-12-21 15:51:51.819566 gigachain_community-0.0.6/langchain_community/llms/promptlayer_openai.py
--rw-r--r--   0        0        0     8024 2023-12-18 12:05:45.736765 gigachain_community-0.0.6/langchain_community/llms/replicate.py
--rw-r--r--   0        0        0     7387 2023-12-18 12:05:45.737203 gigachain_community-0.0.6/langchain_community/llms/rwkv.py
--rw-r--r--   0        0        0    13193 2023-12-18 12:05:45.737817 gigachain_community-0.0.6/langchain_community/llms/sagemaker_endpoint.py
--rw-r--r--   0        0        0     7743 2023-12-18 12:05:45.738142 gigachain_community-0.0.6/langchain_community/llms/self_hosted.py
--rw-r--r--   0        0        0     7743 2023-12-18 12:05:45.738949 gigachain_community-0.0.6/langchain_community/llms/self_hosted_hugging_face.py
--rw-r--r--   0        0        0     4720 2023-12-28 13:38:34.500543 gigachain_community-0.0.6/langchain_community/llms/stochasticai.py
--rw-r--r--   0        0        0     7552 2023-12-18 12:05:45.739825 gigachain_community-0.0.6/langchain_community/llms/symblai_nebula.py
--rw-r--r--   0        0        0    14081 2023-12-21 15:51:51.820638 gigachain_community-0.0.6/langchain_community/llms/textgen.py
--rw-r--r--   0        0        0     5243 2023-12-18 12:05:45.740891 gigachain_community-0.0.6/langchain_community/llms/titan_takeoff.py
--rw-r--r--   0        0        0     7349 2023-12-21 15:51:51.821440 gigachain_community-0.0.6/langchain_community/llms/titan_takeoff_pro.py
--rw-r--r--   0        0        0     7526 2023-12-21 15:51:51.822232 gigachain_community-0.0.6/langchain_community/llms/together.py
--rw-r--r--   0        0        0     9593 2023-12-21 15:51:51.823228 gigachain_community-0.0.6/langchain_community/llms/tongyi.py
--rw-r--r--   0        0        0      258 2023-12-18 12:05:45.742413 gigachain_community-0.0.6/langchain_community/llms/utils.py
--rw-r--r--   0        0        0    18948 2023-12-21 15:51:51.824271 gigachain_community-0.0.6/langchain_community/llms/vertexai.py
--rw-r--r--   0        0        0     5592 2023-12-18 12:05:45.743737 gigachain_community-0.0.6/langchain_community/llms/vllm.py
--rw-r--r--   0        0        0     6591 2023-12-28 13:38:34.501403 gigachain_community-0.0.6/langchain_community/llms/volcengine_maas.py
--rw-r--r--   0        0        0    13164 2023-12-18 12:05:45.744770 gigachain_community-0.0.6/langchain_community/llms/watsonxllm.py
--rw-r--r--   0        0        0     4970 2023-12-18 12:05:45.745301 gigachain_community-0.0.6/langchain_community/llms/writer.py
--rw-r--r--   0        0        0     6325 2023-12-21 15:51:51.825366 gigachain_community-0.0.6/langchain_community/llms/xinference.py
--rw-r--r--   0        0        0    10797 2023-12-21 15:51:51.826293 gigachain_community-0.0.6/langchain_community/llms/yandex.py
--rw-r--r--   0        0        0        0 2023-12-18 12:05:45.746445 gigachain_community-0.0.6/langchain_community/py.typed
--rw-r--r--   0        0        0     4245 2023-12-21 15:51:51.827178 gigachain_community-0.0.6/langchain_community/retrievers/__init__.py
--rw-r--r--   0        0        0     4328 2023-12-18 12:05:45.747540 gigachain_community-0.0.6/langchain_community/retrievers/arcee.py
--rw-r--r--   0        0        0      773 2023-12-18 12:05:45.747949 gigachain_community-0.0.6/langchain_community/retrievers/arxiv.py
--rw-r--r--   0        0        0     4279 2023-12-18 12:05:45.748397 gigachain_community-0.0.6/langchain_community/retrievers/azure_cognitive_search.py
--rw-r--r--   0        0        0     4691 2023-12-21 15:51:51.828732 gigachain_community-0.0.6/langchain_community/retrievers/bedrock.py
--rw-r--r--   0        0        0     3648 2023-12-18 12:05:45.749291 gigachain_community-0.0.6/langchain_community/retrievers/bm25.py
--rw-r--r--   0        0        0     2684 2023-12-18 12:05:45.749632 gigachain_community-0.0.6/langchain_community/retrievers/chaindesk.py
--rw-r--r--   0        0        0     3024 2023-12-18 12:05:45.749873 gigachain_community-0.0.6/langchain_community/retrievers/chatgpt_plugin_retriever.py
--rw-r--r--   0        0        0     2816 2023-12-18 12:05:45.750128 gigachain_community-0.0.6/langchain_community/retrievers/cohere_rag_retriever.py
--rw-r--r--   0        0        0     2338 2023-12-18 12:05:45.750555 gigachain_community-0.0.6/langchain_community/retrievers/databerry.py
--rw-r--r--   0        0        0     6778 2023-12-18 12:05:45.751130 gigachain_community-0.0.6/langchain_community/retrievers/docarray.py
--rw-r--r--   0        0        0     4639 2023-12-18 12:05:45.751921 gigachain_community-0.0.6/langchain_community/retrievers/elastic_search_bm25.py
--rw-r--r--   0        0        0     2000 2023-12-18 12:05:45.752650 gigachain_community-0.0.6/langchain_community/retrievers/embedchain.py
--rw-r--r--   0        0        0     4583 2023-12-18 12:05:45.753268 gigachain_community-0.0.6/langchain_community/retrievers/google_cloud_documentai_warehouse.py
--rw-r--r--   0        0        0    17552 2023-12-28 13:38:34.502238 gigachain_community-0.0.6/langchain_community/retrievers/google_vertex_ai_search.py
--rw-r--r--   0        0        0     1985 2023-12-18 12:05:45.754528 gigachain_community-0.0.6/langchain_community/retrievers/kay.py
--rw-r--r--   0        0        0    13811 2023-12-21 15:51:51.830140 gigachain_community-0.0.6/langchain_community/retrievers/kendra.py
--rw-r--r--   0        0        0     2570 2023-12-18 12:05:45.756151 gigachain_community-0.0.6/langchain_community/retrievers/knn.py
--rw-r--r--   0        0        0     3162 2023-12-18 12:05:45.756542 gigachain_community-0.0.6/langchain_community/retrievers/llama_index.py
--rw-r--r--   0        0        0     1486 2023-12-18 12:05:45.756990 gigachain_community-0.0.6/langchain_community/retrievers/metal.py
--rw-r--r--   0        0        0     2435 2023-12-18 12:05:45.757360 gigachain_community-0.0.6/langchain_community/retrievers/milvus.py
--rw-r--r--   0        0        0      644 2023-12-18 12:05:45.757713 gigachain_community-0.0.6/langchain_community/retrievers/outline.py
--rw-r--r--   0        0        0     5733 2023-12-18 12:05:45.758713 gigachain_community-0.0.6/langchain_community/retrievers/pinecone_hybrid_search.py
--rw-r--r--   0        0        0      643 2023-12-18 12:05:45.759084 gigachain_community-0.0.6/langchain_community/retrievers/pubmed.py
--rw-r--r--   0        0        0      104 2023-12-18 12:05:45.759462 gigachain_community-0.0.6/langchain_community/retrievers/pupmed.py
--rw-r--r--   0        0        0     7468 2023-12-21 15:51:51.831006 gigachain_community-0.0.6/langchain_community/retrievers/qdrant_sparse_vector_retriever.py
--rw-r--r--   0        0        0     1935 2023-12-18 12:05:45.759849 gigachain_community-0.0.6/langchain_community/retrievers/remote_retriever.py
--rw-r--r--   0        0        0     4131 2023-12-18 12:05:45.760244 gigachain_community-0.0.6/langchain_community/retrievers/svm.py
--rw-r--r--   0        0        0     2855 2023-12-18 12:05:45.760593 gigachain_community-0.0.6/langchain_community/retrievers/tavily_search_api.py
--rw-r--r--   0        0        0     4079 2023-12-18 12:05:45.760932 gigachain_community-0.0.6/langchain_community/retrievers/tfidf.py
--rw-r--r--   0        0        0     4555 2023-12-18 12:05:45.761391 gigachain_community-0.0.6/langchain_community/retrievers/vespa_retriever.py
--rw-r--r--   0        0        0     6195 2023-12-18 12:05:45.762141 gigachain_community-0.0.6/langchain_community/retrievers/weaviate_hybrid_search.py
--rw-r--r--   0        0        0      656 2023-12-18 12:05:45.762889 gigachain_community-0.0.6/langchain_community/retrievers/wikipedia.py
--rw-r--r--   0        0        0     2356 2023-12-18 12:05:45.763365 gigachain_community-0.0.6/langchain_community/retrievers/you.py
--rw-r--r--   0        0        0     5904 2023-12-18 12:05:45.763882 gigachain_community-0.0.6/langchain_community/retrievers/zep.py
--rw-r--r--   0        0        0     2735 2023-12-18 12:05:45.764315 gigachain_community-0.0.6/langchain_community/retrievers/zilliz.py
--rw-r--r--   0        0        0      501 2023-12-18 12:05:45.764791 gigachain_community-0.0.6/langchain_community/storage/__init__.py
--rw-r--r--   0        0        0      179 2023-12-18 12:05:45.765177 gigachain_community-0.0.6/langchain_community/storage/exceptions.py
--rw-r--r--   0        0        0     4788 2023-12-18 12:05:45.765839 gigachain_community-0.0.6/langchain_community/storage/redis.py
--rw-r--r--   0        0        0     5764 2023-12-18 12:05:45.766664 gigachain_community-0.0.6/langchain_community/storage/upstash_redis.py
--rw-r--r--   0        0        0    33514 2023-12-18 12:05:45.767310 gigachain_community-0.0.6/langchain_community/tools/__init__.py
--rw-r--r--   0        0        0     3185 2023-12-18 12:05:45.767799 gigachain_community-0.0.6/langchain_community/tools/ainetwork/app.py
--rw-r--r--   0        0        0     2109 2023-12-18 12:05:45.768158 gigachain_community-0.0.6/langchain_community/tools/ainetwork/base.py
--rw-r--r--   0        0        0     4140 2023-12-18 12:05:45.768950 gigachain_community-0.0.6/langchain_community/tools/ainetwork/owner.py
--rw-r--r--   0        0        0     2746 2023-12-18 12:05:45.769433 gigachain_community-0.0.6/langchain_community/tools/ainetwork/rule.py
--rw-r--r--   0        0        0     1074 2023-12-18 12:05:45.769853 gigachain_community-0.0.6/langchain_community/tools/ainetwork/transfer.py
--rw-r--r--   0        0        0     2314 2023-12-18 12:05:45.770226 gigachain_community-0.0.6/langchain_community/tools/ainetwork/utils.py
--rw-r--r--   0        0        0     2624 2023-12-18 12:05:45.770601 gigachain_community-0.0.6/langchain_community/tools/ainetwork/value.py
--rw-r--r--   0        0        0      257 2023-12-18 12:05:45.770978 gigachain_community-0.0.6/langchain_community/tools/amadeus/__init__.py
--rw-r--r--   0        0        0      435 2023-12-18 12:05:45.771420 gigachain_community-0.0.6/langchain_community/tools/amadeus/base.py
--rw-r--r--   0        0        0     1845 2023-12-18 12:05:45.771860 gigachain_community-0.0.6/langchain_community/tools/amadeus/closest_airport.py
--rw-r--r--   0        0        0     5611 2023-12-18 12:05:45.772295 gigachain_community-0.0.6/langchain_community/tools/amadeus/flight_search.py
--rw-r--r--   0        0        0     1276 2023-12-18 12:05:45.773346 gigachain_community-0.0.6/langchain_community/tools/amadeus/utils.py
--rw-r--r--   0        0        0       25 2023-12-18 12:05:45.773797 gigachain_community-0.0.6/langchain_community/tools/arxiv/__init__.py
--rw-r--r--   0        0        0     1228 2023-12-21 15:51:51.832262 gigachain_community-0.0.6/langchain_community/tools/arxiv/tool.py
--rw-r--r--   0        0        0      802 2023-12-18 12:05:45.774697 gigachain_community-0.0.6/langchain_community/tools/azure_cognitive_services/__init__.py
--rw-r--r--   0        0        0     5375 2023-12-18 12:05:45.775110 gigachain_community-0.0.6/langchain_community/tools/azure_cognitive_services/form_recognizer.py
--rw-r--r--   0        0        0     5304 2023-12-18 12:05:45.775653 gigachain_community-0.0.6/langchain_community/tools/azure_cognitive_services/image_analysis.py
--rw-r--r--   0        0        0     4336 2023-12-18 12:05:45.776161 gigachain_community-0.0.6/langchain_community/tools/azure_cognitive_services/speech2text.py
--rw-r--r--   0        0        0     3675 2023-12-18 12:05:45.776545 gigachain_community-0.0.6/langchain_community/tools/azure_cognitive_services/text2speech.py
--rw-r--r--   0        0        0     3542 2023-12-21 15:51:51.833253 gigachain_community-0.0.6/langchain_community/tools/azure_cognitive_services/text_analytics_health.py
--rw-r--r--   0        0        0      776 2023-12-18 12:05:45.777398 gigachain_community-0.0.6/langchain_community/tools/azure_cognitive_services/utils.py
--rw-r--r--   0        0        0        0 2023-12-18 12:05:45.777639 gigachain_community-0.0.6/langchain_community/tools/bearly/__init__.py
--rw-r--r--   0        0        0     5468 2023-12-18 12:05:45.777984 gigachain_community-0.0.6/langchain_community/tools/bearly/tool.py
--rw-r--r--   0        0        0      170 2023-12-18 12:05:45.778478 gigachain_community-0.0.6/langchain_community/tools/bing_search/__init__.py
--rw-r--r--   0        0        0     1463 2023-12-18 12:05:45.779631 gigachain_community-0.0.6/langchain_community/tools/bing_search/tool.py
--rw-r--r--   0        0        0        0 2023-12-18 12:05:45.780012 gigachain_community-0.0.6/langchain_community/tools/brave_search/__init__.py
--rw-r--r--   0        0        0     1354 2023-12-18 12:05:45.780571 gigachain_community-0.0.6/langchain_community/tools/brave_search/tool.py
--rw-r--r--   0        0        0        0 2023-12-18 12:05:45.780739 gigachain_community-0.0.6/langchain_community/tools/clickup/__init__.py
--rw-r--r--   0        0        0     8298 2023-12-18 12:05:45.781291 gigachain_community-0.0.6/langchain_community/tools/clickup/prompt.py
--rw-r--r--   0        0        0     1230 2023-12-18 12:05:45.781701 gigachain_community-0.0.6/langchain_community/tools/clickup/tool.py
--rw-r--r--   0        0        0     1336 2023-12-18 12:05:45.782109 gigachain_community-0.0.6/langchain_community/tools/convert_to_openai.py
--rw-r--r--   0        0        0      268 2023-12-18 12:05:45.782537 gigachain_community-0.0.6/langchain_community/tools/dataforseo_api_search/__init__.py
--rw-r--r--   0        0        0     2214 2023-12-18 12:05:45.783121 gigachain_community-0.0.6/langchain_community/tools/dataforseo_api_search/tool.py
--rw-r--r--   0        0        0      147 2023-12-18 12:05:45.783495 gigachain_community-0.0.6/langchain_community/tools/ddg_search/__init__.py
--rw-r--r--   0        0        0     2641 2023-12-21 15:51:51.835050 gigachain_community-0.0.6/langchain_community/tools/ddg_search/tool.py
--rw-r--r--   0        0        0        0 2023-12-18 12:05:45.783987 gigachain_community-0.0.6/langchain_community/tools/e2b_data_analysis/__init__.py
--rw-r--r--   0        0        0     8015 2023-12-28 13:38:34.503446 gigachain_community-0.0.6/langchain_community/tools/e2b_data_analysis/tool.py
--rw-r--r--   0        0        0    20701 2023-12-21 15:51:51.836025 gigachain_community-0.0.6/langchain_community/tools/e2b_data_analysis/unparse.py
--rw-r--r--   0        0        0     1024 2023-12-18 12:05:45.785160 gigachain_community-0.0.6/langchain_community/tools/edenai/__init__.py
--rw-r--r--   0        0        0     3465 2023-12-18 12:05:45.785432 gigachain_community-0.0.6/langchain_community/tools/edenai/audio_speech_to_text.py
--rw-r--r--   0        0        0     3885 2023-12-18 12:05:45.785916 gigachain_community-0.0.6/langchain_community/tools/edenai/audio_text_to_speech.py
--rw-r--r--   0        0        0     5386 2023-12-18 12:05:45.786625 gigachain_community-0.0.6/langchain_community/tools/edenai/edenai_base_tool.py
--rw-r--r--   0        0        0     2249 2023-12-18 12:05:45.787257 gigachain_community-0.0.6/langchain_community/tools/edenai/image_explicitcontent.py
--rw-r--r--   0        0        0     2476 2023-12-18 12:05:45.787647 gigachain_community-0.0.6/langchain_community/tools/edenai/image_objectdetection.py
--rw-r--r--   0        0        0     1966 2023-12-18 12:05:45.788039 gigachain_community-0.0.6/langchain_community/tools/edenai/ocr_identityparser.py
--rw-r--r--   0        0        0     2187 2023-12-18 12:05:45.788452 gigachain_community-0.0.6/langchain_community/tools/edenai/ocr_invoiceparser.py
--rw-r--r--   0        0        0     2407 2023-12-18 12:05:45.789172 gigachain_community-0.0.6/langchain_community/tools/edenai/text_moderation.py
--rw-r--r--   0        0        0      164 2023-12-18 12:05:45.789668 gigachain_community-0.0.6/langchain_community/tools/eleven_labs/__init__.py
--rw-r--r--   0        0        0      203 2023-12-18 12:05:45.790052 gigachain_community-0.0.6/langchain_community/tools/eleven_labs/models.py
--rw-r--r--   0        0        0     2709 2023-12-18 12:05:45.790521 gigachain_community-0.0.6/langchain_community/tools/eleven_labs/text2speech.py
--rw-r--r--   0        0        0      723 2023-12-18 12:05:45.791133 gigachain_community-0.0.6/langchain_community/tools/file_management/__init__.py
--rw-r--r--   0        0        0     1749 2023-12-18 12:05:45.791626 gigachain_community-0.0.6/langchain_community/tools/file_management/copy.py
--rw-r--r--   0        0        0     1345 2023-12-18 12:05:45.791998 gigachain_community-0.0.6/langchain_community/tools/file_management/delete.py
--rw-r--r--   0        0        0     1965 2023-12-18 12:05:45.792403 gigachain_community-0.0.6/langchain_community/tools/file_management/file_search.py
--rw-r--r--   0        0        0     1432 2023-12-18 12:05:45.792791 gigachain_community-0.0.6/langchain_community/tools/file_management/list_dir.py
--rw-r--r--   0        0        0     1889 2023-12-18 12:05:45.793186 gigachain_community-0.0.6/langchain_community/tools/file_management/move.py
--rw-r--r--   0        0        0     1340 2023-12-18 12:05:45.793625 gigachain_community-0.0.6/langchain_community/tools/file_management/read.py
--rw-r--r--   0        0        0     1726 2023-12-18 12:05:45.794428 gigachain_community-0.0.6/langchain_community/tools/file_management/utils.py
--rw-r--r--   0        0        0     1614 2023-12-18 12:05:45.794830 gigachain_community-0.0.6/langchain_community/tools/file_management/write.py
--rw-r--r--   0        0        0       20 2023-12-18 12:05:45.795246 gigachain_community-0.0.6/langchain_community/tools/github/__init__.py
--rw-r--r--   0        0        0     6220 2023-12-18 12:05:45.795757 gigachain_community-0.0.6/langchain_community/tools/github/prompt.py
--rw-r--r--   0        0        0     1194 2023-12-18 12:05:45.796153 gigachain_community-0.0.6/langchain_community/tools/github/tool.py
--rw-r--r--   0        0        0       20 2023-12-18 12:05:45.796530 gigachain_community-0.0.6/langchain_community/tools/gitlab/__init__.py
--rw-r--r--   0        0        0     3438 2023-12-18 12:05:45.797359 gigachain_community-0.0.6/langchain_community/tools/gitlab/prompt.py
--rw-r--r--   0        0        0      972 2023-12-18 12:05:45.797816 gigachain_community-0.0.6/langchain_community/tools/gitlab/tool.py
--rw-r--r--   0        0        0      601 2023-12-18 12:05:45.798228 gigachain_community-0.0.6/langchain_community/tools/gmail/__init__.py
--rw-r--r--   0        0        0     1004 2023-12-18 12:05:45.798672 gigachain_community-0.0.6/langchain_community/tools/gmail/base.py
--rw-r--r--   0        0        0     2564 2023-12-18 12:05:45.799060 gigachain_community-0.0.6/langchain_community/tools/gmail/create_draft.py
--rw-r--r--   0        0        0     2202 2023-12-18 12:05:45.799653 gigachain_community-0.0.6/langchain_community/tools/gmail/get_message.py
--rw-r--r--   0        0        0     1560 2023-12-18 12:05:45.800071 gigachain_community-0.0.6/langchain_community/tools/gmail/get_thread.py
--rw-r--r--   0        0        0     4874 2023-12-18 12:05:45.801270 gigachain_community-0.0.6/langchain_community/tools/gmail/search.py
--rw-r--r--   0        0        0     2939 2023-12-28 13:38:34.504472 gigachain_community-0.0.6/langchain_community/tools/gmail/send_message.py
--rw-r--r--   0        0        0     4528 2023-12-18 12:05:45.802173 gigachain_community-0.0.6/langchain_community/tools/gmail/utils.py
--rw-r--r--   0        0        0      136 2023-12-18 12:05:45.802569 gigachain_community-0.0.6/langchain_community/tools/golden_query/__init__.py
--rw-r--r--   0        0        0     1108 2023-12-18 12:05:45.802914 gigachain_community-0.0.6/langchain_community/tools/golden_query/tool.py
--rw-r--r--   0        0        0      171 2023-12-18 12:05:45.803350 gigachain_community-0.0.6/langchain_community/tools/google_cloud/__init__.py
--rw-r--r--   0        0        0     3173 2023-12-18 12:05:45.803756 gigachain_community-0.0.6/langchain_community/tools/google_cloud/texttospeech.py
--rw-r--r--   0        0        0      152 2023-12-18 12:05:45.805823 gigachain_community-0.0.6/langchain_community/tools/google_finance/__init__.py
--rw-r--r--   0        0        0      854 2023-12-18 12:05:45.806289 gigachain_community-0.0.6/langchain_community/tools/google_finance/tool.py
--rw-r--r--   0        0        0      140 2023-12-18 12:05:45.806731 gigachain_community-0.0.6/langchain_community/tools/google_jobs/__init__.py
--rw-r--r--   0        0        0      826 2023-12-18 12:05:45.807119 gigachain_community-0.0.6/langchain_community/tools/google_jobs/tool.py
--rw-r--r--   0        0        0      140 2023-12-18 12:05:45.807515 gigachain_community-0.0.6/langchain_community/tools/google_lens/__init__.py
--rw-r--r--   0        0        0      822 2023-12-18 12:05:45.807846 gigachain_community-0.0.6/langchain_community/tools/google_lens/tool.py
--rw-r--r--   0        0        0      140 2023-12-18 12:05:45.808212 gigachain_community-0.0.6/langchain_community/tools/google_places/__init__.py
--rw-r--r--   0        0        0     1141 2023-12-18 12:05:45.808602 gigachain_community-0.0.6/langchain_community/tools/google_places/tool.py
--rw-r--r--   0        0        0      152 2023-12-18 12:05:45.809035 gigachain_community-0.0.6/langchain_community/tools/google_scholar/__init__.py
--rw-r--r--   0        0        0      847 2023-12-18 12:05:45.809424 gigachain_community-0.0.6/langchain_community/tools/google_scholar/tool.py
--rw-r--r--   0        0        0      195 2023-12-18 12:05:45.810892 gigachain_community-0.0.6/langchain_community/tools/google_search/__init__.py
--rw-r--r--   0        0        0     1489 2023-12-18 12:05:45.811333 gigachain_community-0.0.6/langchain_community/tools/google_search/tool.py
--rw-r--r--   0        0        0      243 2023-12-18 12:05:45.811765 gigachain_community-0.0.6/langchain_community/tools/google_serper/__init__.py
--rw-r--r--   0        0        0     2113 2023-12-18 12:05:45.812243 gigachain_community-0.0.6/langchain_community/tools/google_serper/tool.py
--rw-r--r--   0        0        0      148 2023-12-18 12:05:45.812859 gigachain_community-0.0.6/langchain_community/tools/google_trends/__init__.py
--rw-r--r--   0        0        0      844 2023-12-18 12:05:45.813598 gigachain_community-0.0.6/langchain_community/tools/google_trends/tool.py
--rw-r--r--   0        0        0       47 2023-12-18 12:05:45.813986 gigachain_community-0.0.6/langchain_community/tools/graphql/__init__.py
--rw-r--r--   0        0        0     1204 2023-12-18 12:05:45.814359 gigachain_community-0.0.6/langchain_community/tools/graphql/tool.py
--rw-r--r--   0        0        0      132 2023-12-18 12:05:45.814785 gigachain_community-0.0.6/langchain_community/tools/human/__init__.py
--rw-r--r--   0        0        0      983 2023-12-18 12:05:45.815173 gigachain_community-0.0.6/langchain_community/tools/human/tool.py
--rw-r--r--   0        0        0     2286 2023-12-18 12:05:45.815512 gigachain_community-0.0.6/langchain_community/tools/ifttt.py
--rw-r--r--   0        0        0       43 2023-12-18 12:05:45.815966 gigachain_community-0.0.6/langchain_community/tools/interaction/__init__.py
--rw-r--r--   0        0        0      464 2023-12-18 12:05:45.816375 gigachain_community-0.0.6/langchain_community/tools/interaction/tool.py
--rw-r--r--   0        0        0       17 2023-12-18 12:05:45.817112 gigachain_community-0.0.6/langchain_community/tools/jira/__init__.py
--rw-r--r--   0        0        0     3170 2023-12-18 12:05:45.818054 gigachain_community-0.0.6/langchain_community/tools/jira/prompt.py
--rw-r--r--   0        0        0     1342 2023-12-18 12:05:45.818546 gigachain_community-0.0.6/langchain_community/tools/jira/tool.py
--rw-r--r--   0        0        0       46 2023-12-18 12:05:45.819119 gigachain_community-0.0.6/langchain_community/tools/json/__init__.py
--rw-r--r--   0        0        0     4139 2023-12-18 12:05:45.819580 gigachain_community-0.0.6/langchain_community/tools/json/tool.py
--rw-r--r--   0        0        0      134 2023-12-18 12:05:45.820014 gigachain_community-0.0.6/langchain_community/tools/memorize/__init__.py
--rw-r--r--   0        0        0     1828 2023-12-21 15:51:51.837175 gigachain_community-0.0.6/langchain_community/tools/memorize/tool.py
--rw-r--r--   0        0        0       35 2023-12-18 12:05:45.821474 gigachain_community-0.0.6/langchain_community/tools/merriam_webster/__init__.py
--rw-r--r--   0        0        0      853 2023-12-18 12:05:45.822073 gigachain_community-0.0.6/langchain_community/tools/merriam_webster/tool.py
--rw-r--r--   0        0        0      154 2023-12-18 12:05:45.822754 gigachain_community-0.0.6/langchain_community/tools/metaphor_search/__init__.py
--rw-r--r--   0        0        0     2690 2023-12-18 12:05:45.823297 gigachain_community-0.0.6/langchain_community/tools/metaphor_search/tool.py
--rw-r--r--   0        0        0      359 2023-12-18 12:05:45.823831 gigachain_community-0.0.6/langchain_community/tools/multion/__init__.py
--rw-r--r--   0        0        0     2052 2023-12-18 12:05:45.824250 gigachain_community-0.0.6/langchain_community/tools/multion/close_session.py
--rw-r--r--   0        0        0     2585 2023-12-18 12:05:45.824782 gigachain_community-0.0.6/langchain_community/tools/multion/create_session.py
--rw-r--r--   0        0        0     2822 2023-12-18 12:05:45.825198 gigachain_community-0.0.6/langchain_community/tools/multion/update_session.py
--rw-r--r--   0        0        0        0 2023-12-18 12:05:45.825384 gigachain_community-0.0.6/langchain_community/tools/nasa/__init__.py
--rw-r--r--   0        0        0     5197 2023-12-18 12:05:45.825968 gigachain_community-0.0.6/langchain_community/tools/nasa/prompt.py
--rw-r--r--   0        0        0      831 2023-12-18 12:05:45.826349 gigachain_community-0.0.6/langchain_community/tools/nasa/tool.py
--rw-r--r--   0        0        0      111 2023-12-18 12:05:45.826705 gigachain_community-0.0.6/langchain_community/tools/nuclia/__init__.py
--rw-r--r--   0        0        0     7915 2023-12-18 12:05:45.827114 gigachain_community-0.0.6/langchain_community/tools/nuclia/tool.py
--rw-r--r--   0        0        0      654 2023-12-18 12:05:45.827517 gigachain_community-0.0.6/langchain_community/tools/office365/__init__.py
--rw-r--r--   0        0        0      508 2023-12-18 12:05:45.827887 gigachain_community-0.0.6/langchain_community/tools/office365/base.py
--rw-r--r--   0        0        0     1858 2023-12-18 12:05:45.828512 gigachain_community-0.0.6/langchain_community/tools/office365/create_draft_message.py
--rw-r--r--   0        0        0     4833 2023-12-18 12:05:45.828888 gigachain_community-0.0.6/langchain_community/tools/office365/events_search.py
--rw-r--r--   0        0        0     4246 2023-12-18 12:05:45.829447 gigachain_community-0.0.6/langchain_community/tools/office365/messages_search.py
--rw-r--r--   0        0        0     2898 2023-12-18 12:05:45.829858 gigachain_community-0.0.6/langchain_community/tools/office365/send_event.py
--rw-r--r--   0        0        0     1789 2023-12-18 12:05:45.830410 gigachain_community-0.0.6/langchain_community/tools/office365/send_message.py
--rw-r--r--   0        0        0     2212 2023-12-18 12:05:45.831194 gigachain_community-0.0.6/langchain_community/tools/office365/utils.py
--rw-r--r--   0        0        0        0 2023-12-18 12:05:45.831412 gigachain_community-0.0.6/langchain_community/tools/openapi/__init__.py
--rw-r--r--   0        0        0        0 2023-12-18 12:05:45.831880 gigachain_community-0.0.6/langchain_community/tools/openapi/utils/__init__.py
--rw-r--r--   0        0        0    21288 2023-12-18 12:05:45.832707 gigachain_community-0.0.6/langchain_community/tools/openapi/utils/api_models.py
--rw-r--r--   0        0        0      191 2023-12-18 12:05:45.833201 gigachain_community-0.0.6/langchain_community/tools/openapi/utils/openapi_utils.py
--rw-r--r--   0        0        0      162 2023-12-18 12:05:45.833667 gigachain_community-0.0.6/langchain_community/tools/openweathermap/__init__.py
--rw-r--r--   0        0        0      966 2023-12-18 12:05:45.834076 gigachain_community-0.0.6/langchain_community/tools/openweathermap/tool.py
--rw-r--r--   0        0        0      763 2023-12-18 12:05:45.834481 gigachain_community-0.0.6/langchain_community/tools/playwright/__init__.py
--rw-r--r--   0        0        0     2135 2023-12-18 12:05:45.834869 gigachain_community-0.0.6/langchain_community/tools/playwright/base.py
--rw-r--r--   0        0        0     3083 2023-12-18 12:05:45.835282 gigachain_community-0.0.6/langchain_community/tools/playwright/click.py
--rw-r--r--   0        0        0     1340 2023-12-18 12:05:45.835906 gigachain_community-0.0.6/langchain_community/tools/playwright/current_page.py
--rw-r--r--   0        0        0     3051 2023-12-18 12:05:45.836449 gigachain_community-0.0.6/langchain_community/tools/playwright/extract_hyperlinks.py
--rw-r--r--   0        0        0     2383 2023-12-18 12:05:45.836893 gigachain_community-0.0.6/langchain_community/tools/playwright/extract_text.py
--rw-r--r--   0        0        0     3743 2023-12-18 12:05:45.837329 gigachain_community-0.0.6/langchain_community/tools/playwright/get_elements.py
--rw-r--r--   0        0        0     2878 2023-12-18 12:05:45.837738 gigachain_community-0.0.6/langchain_community/tools/playwright/navigate.py
--rw-r--r--   0        0        0     1926 2023-12-18 12:05:45.838120 gigachain_community-0.0.6/langchain_community/tools/playwright/navigate_back.py
--rw-r--r--   0        0        0     3049 2023-12-18 12:05:45.838549 gigachain_community-0.0.6/langchain_community/tools/playwright/utils.py
--rw-r--r--   0        0        0     2902 2023-12-18 12:05:45.838925 gigachain_community-0.0.6/langchain_community/tools/plugin.py
--rw-r--r--   0        0        0       52 2023-12-18 12:05:45.839326 gigachain_community-0.0.6/langchain_community/tools/powerbi/__init__.py
--rw-r--r--   0        0        0     7339 2023-12-18 12:05:45.839823 gigachain_community-0.0.6/langchain_community/tools/powerbi/prompt.py
--rw-r--r--   0        0        0    11075 2023-12-18 12:05:45.840707 gigachain_community-0.0.6/langchain_community/tools/powerbi/tool.py
--rw-r--r--   0        0        0       26 2023-12-18 12:05:45.841143 gigachain_community-0.0.6/langchain_community/tools/pubmed/__init__.py
--rw-r--r--   0        0        0      944 2023-12-18 12:05:45.841564 gigachain_community-0.0.6/langchain_community/tools/pubmed/tool.py
--rw-r--r--   0        0        0     1965 2023-12-18 12:05:45.842001 gigachain_community-0.0.6/langchain_community/tools/reddit_search/tool.py
--rw-r--r--   0        0        0     1586 2023-12-18 12:05:45.842412 gigachain_community-0.0.6/langchain_community/tools/render.py
--rw-r--r--   0        0        0       52 2023-12-18 12:05:45.842780 gigachain_community-0.0.6/langchain_community/tools/requests/__init__.py
--rw-r--r--   0        0        0     6323 2023-12-18 12:05:45.843362 gigachain_community-0.0.6/langchain_community/tools/requests/tool.py
--rw-r--r--   0        0        0       31 2023-12-18 12:05:45.843730 gigachain_community-0.0.6/langchain_community/tools/scenexplain/__init__.py
--rw-r--r--   0        0        0     1100 2023-12-18 12:05:45.844164 gigachain_community-0.0.6/langchain_community/tools/scenexplain/tool.py
--rw-r--r--   0        0        0      214 2023-12-18 12:05:45.844592 gigachain_community-0.0.6/langchain_community/tools/searchapi/__init__.py
--rw-r--r--   0        0        0     2114 2023-12-18 12:05:45.844972 gigachain_community-0.0.6/langchain_community/tools/searchapi/tool.py
--rw-r--r--   0        0        0        0 2023-12-18 12:05:45.845178 gigachain_community-0.0.6/langchain_community/tools/searx_search/__init__.py
--rw-r--r--   0        0        0     2261 2023-12-18 12:05:45.845824 gigachain_community-0.0.6/langchain_community/tools/searx_search/tool.py
--rw-r--r--   0        0        0      103 2023-12-18 12:05:45.846255 gigachain_community-0.0.6/langchain_community/tools/shell/__init__.py
--rw-r--r--   0        0        0     2663 2023-12-18 12:05:45.846662 gigachain_community-0.0.6/langchain_community/tools/shell/tool.py
--rw-r--r--   0        0        0      502 2023-12-18 12:05:45.847147 gigachain_community-0.0.6/langchain_community/tools/slack/__init__.py
--rw-r--r--   0        0        0      460 2023-12-18 12:05:45.847474 gigachain_community-0.0.6/langchain_community/tools/slack/base.py
--rw-r--r--   0        0        0     1118 2023-12-21 15:51:51.838169 gigachain_community-0.0.6/langchain_community/tools/slack/get_channel.py
--rw-r--r--   0        0        0     1402 2023-12-21 15:51:51.839105 gigachain_community-0.0.6/langchain_community/tools/slack/get_message.py
--rw-r--r--   0        0        0     2071 2023-12-18 12:05:45.848876 gigachain_community-0.0.6/langchain_community/tools/slack/schedule_message.py
--rw-r--r--   0        0        0     1222 2023-12-18 12:05:45.849246 gigachain_community-0.0.6/langchain_community/tools/slack/send_message.py
--rw-r--r--   0        0        0     1135 2023-12-18 12:05:45.849856 gigachain_community-0.0.6/langchain_community/tools/slack/utils.py
--rw-r--r--   0        0        0       18 2023-12-18 12:05:45.850305 gigachain_community-0.0.6/langchain_community/tools/sleep/__init__.py
--rw-r--r--   0        0        0     1229 2023-12-18 12:05:45.850716 gigachain_community-0.0.6/langchain_community/tools/sleep/tool.py
--rw-r--r--   0        0        0       44 2023-12-18 12:05:45.851086 gigachain_community-0.0.6/langchain_community/tools/spark_sql/__init__.py
--rw-r--r--   0        0        0      550 2023-12-18 12:05:45.851476 gigachain_community-0.0.6/langchain_community/tools/spark_sql/prompt.py
--rw-r--r--   0        0        0     4376 2023-12-18 12:05:45.851871 gigachain_community-0.0.6/langchain_community/tools/spark_sql/tool.py
--rw-r--r--   0        0        0       49 2023-12-18 12:05:45.852158 gigachain_community-0.0.6/langchain_community/tools/sql_database/__init__.py
--rw-r--r--   0        0        0      597 2023-12-18 12:05:45.852450 gigachain_community-0.0.6/langchain_community/tools/sql_database/prompt.py
--rw-r--r--   0        0        0     4487 2023-12-18 12:05:45.852922 gigachain_community-0.0.6/langchain_community/tools/sql_database/tool.py
--rw-r--r--   0        0        0       33 2023-12-18 12:05:45.853383 gigachain_community-0.0.6/langchain_community/tools/stackexchange/__init__.py
--rw-r--r--   0        0        0      868 2023-12-18 12:05:45.853792 gigachain_community-0.0.6/langchain_community/tools/stackexchange/tool.py
--rw-r--r--   0        0        0       24 2023-12-18 12:05:45.854296 gigachain_community-0.0.6/langchain_community/tools/steam/__init__.py
--rw-r--r--   0        0        0     1657 2023-12-18 12:05:45.854700 gigachain_community-0.0.6/langchain_community/tools/steam/prompt.py
--rw-r--r--   0        0        0      842 2023-12-18 12:05:45.855152 gigachain_community-0.0.6/langchain_community/tools/steam/tool.py
--rw-r--r--   0        0        0      186 2023-12-18 12:05:45.855742 gigachain_community-0.0.6/langchain_community/tools/steamship_image_generation/__init__.py
--rw-r--r--   0        0        0     3377 2023-12-18 12:05:45.856114 gigachain_community-0.0.6/langchain_community/tools/steamship_image_generation/tool.py
--rw-r--r--   0        0        0     1395 2023-12-18 12:05:45.856475 gigachain_community-0.0.6/langchain_community/tools/steamship_image_generation/utils.py
--rw-r--r--   0        0        0      189 2023-12-18 12:05:45.856940 gigachain_community-0.0.6/langchain_community/tools/tavily_search/__init__.py
--rw-r--r--   0        0        0     3375 2023-12-28 13:38:34.505773 gigachain_community-0.0.6/langchain_community/tools/tavily_search/tool.py
--rw-r--r--   0        0        0       51 2023-12-18 12:05:45.858009 gigachain_community-0.0.6/langchain_community/tools/vectorstore/__init__.py
--rw-r--r--   0        0        0     3302 2023-12-18 12:05:45.858410 gigachain_community-0.0.6/langchain_community/tools/vectorstore/tool.py
--rw-r--r--   0        0        0       29 2023-12-18 12:05:45.858782 gigachain_community-0.0.6/langchain_community/tools/wikipedia/__init__.py
--rw-r--r--   0        0        0      867 2023-12-18 12:05:45.859163 gigachain_community-0.0.6/langchain_community/tools/wikipedia/tool.py
--rw-r--r--   0        0        0      156 2023-12-18 12:05:45.859606 gigachain_community-0.0.6/langchain_community/tools/wolfram_alpha/__init__.py
--rw-r--r--   0        0        0      887 2023-12-18 12:05:45.859959 gigachain_community-0.0.6/langchain_community/tools/wolfram_alpha/tool.py
--rw-r--r--   0        0        0     2473 2023-12-18 12:05:45.860331 gigachain_community-0.0.6/langchain_community/tools/yahoo_finance_news.py
--rw-r--r--   0        0        0        0 2023-12-18 12:05:45.860527 gigachain_community-0.0.6/langchain_community/tools/youtube/__init__.py
--rw-r--r--   0        0        0     1729 2023-12-18 12:05:45.861292 gigachain_community-0.0.6/langchain_community/tools/youtube/search.py
--rw-r--r--   0        0        0      193 2023-12-18 12:05:45.861830 gigachain_community-0.0.6/langchain_community/tools/zapier/__init__.py
--rw-r--r--   0        0        0     1182 2023-12-18 12:05:45.862240 gigachain_community-0.0.6/langchain_community/tools/zapier/prompt.py
--rw-r--r--   0        0        0     7730 2023-12-18 12:05:45.863337 gigachain_community-0.0.6/langchain_community/tools/zapier/tool.py
--rw-r--r--   0        0        0    10998 2023-12-18 12:05:45.864315 gigachain_community-0.0.6/langchain_community/utilities/__init__.py
--rw-r--r--   0        0        0     2192 2023-12-18 12:05:45.864880 gigachain_community-0.0.6/langchain_community/utilities/alpha_vantage.py
--rw-r--r--   0        0        0      844 2023-12-18 12:05:45.865288 gigachain_community-0.0.6/langchain_community/utilities/anthropic.py
--rw-r--r--   0        0        0     8458 2023-12-18 12:05:45.865753 gigachain_community-0.0.6/langchain_community/utilities/apify.py
--rw-r--r--   0        0        0     8710 2023-12-18 12:05:45.866259 gigachain_community-0.0.6/langchain_community/utilities/arcee.py
--rw-r--r--   0        0        0     9262 2023-12-21 15:51:51.841117 gigachain_community-0.0.6/langchain_community/utilities/arxiv.py
--rw-r--r--   0        0        0     2437 2023-12-18 12:05:45.867481 gigachain_community-0.0.6/langchain_community/utilities/awslambda.py
--rw-r--r--   0        0        0     2499 2023-12-18 12:05:45.867932 gigachain_community-0.0.6/langchain_community/utilities/bibtex.py
--rw-r--r--   0        0        0     3545 2023-12-18 12:05:45.868301 gigachain_community-0.0.6/langchain_community/utilities/bing_search.py
--rw-r--r--   0        0        0     2356 2023-12-18 12:05:45.868774 gigachain_community-0.0.6/langchain_community/utilities/brave_search.py
--rw-r--r--   0        0        0    19771 2023-12-18 12:05:45.869364 gigachain_community-0.0.6/langchain_community/utilities/clickup.py
--rw-r--r--   0        0        0     6377 2023-12-18 12:05:45.870021 gigachain_community-0.0.6/langchain_community/utilities/dalle_image_generator.py
--rw-r--r--   0        0        0     7854 2023-12-18 12:05:45.870814 gigachain_community-0.0.6/langchain_community/utilities/dataforseo_api_search.py
--rw-r--r--   0        0        0     4310 2023-12-18 12:05:45.871460 gigachain_community-0.0.6/langchain_community/utilities/duckduckgo_search.py
--rw-r--r--   0        0        0    31986 2023-12-21 15:51:51.842273 gigachain_community-0.0.6/langchain_community/utilities/github.py
--rw-r--r--   0        0        0    11959 2023-12-18 12:05:45.872934 gigachain_community-0.0.6/langchain_community/utilities/gitlab.py
--rw-r--r--   0        0        0     1858 2023-12-18 12:05:45.873304 gigachain_community-0.0.6/langchain_community/utilities/golden_query.py
--rw-r--r--   0        0        0     3400 2023-12-21 15:51:51.843661 gigachain_community-0.0.6/langchain_community/utilities/google_finance.py
--rw-r--r--   0        0        0     2804 2023-12-21 15:51:51.844769 gigachain_community-0.0.6/langchain_community/utilities/google_jobs.py
--rw-r--r--   0        0        0     2859 2023-12-18 12:05:45.874583 gigachain_community-0.0.6/langchain_community/utilities/google_lens.py
--rw-r--r--   0        0        0     4107 2023-12-18 12:05:45.874988 gigachain_community-0.0.6/langchain_community/utilities/google_places_api.py
--rw-r--r--   0        0        0     5171 2023-12-18 12:05:45.875442 gigachain_community-0.0.6/langchain_community/utilities/google_scholar.py
--rw-r--r--   0        0        0     5048 2023-12-18 12:05:45.876258 gigachain_community-0.0.6/langchain_community/utilities/google_search.py
--rw-r--r--   0        0        0     6503 2023-12-18 12:05:45.876775 gigachain_community-0.0.6/langchain_community/utilities/google_serper.py
--rw-r--r--   0        0        0     4033 2023-12-18 12:05:45.877158 gigachain_community-0.0.6/langchain_community/utilities/google_trends.py
--rw-r--r--   0        0        0     1903 2023-12-18 12:05:45.877780 gigachain_community-0.0.6/langchain_community/utilities/graphql.py
--rw-r--r--   0        0        0     6195 2023-12-18 12:05:45.878463 gigachain_community-0.0.6/langchain_community/utilities/jira.py
--rw-r--r--   0        0        0     2647 2023-12-18 12:05:45.879155 gigachain_community-0.0.6/langchain_community/utilities/max_compute.py
--rw-r--r--   0        0        0     3748 2023-12-18 12:05:45.879594 gigachain_community-0.0.6/langchain_community/utilities/merriam_webster.py
--rw-r--r--   0        0        0     6809 2023-12-18 12:05:45.880096 gigachain_community-0.0.6/langchain_community/utilities/metaphor_search.py
--rw-r--r--   0        0        0     1820 2023-12-21 15:51:51.846047 gigachain_community-0.0.6/langchain_community/utilities/nasa.py
--rw-r--r--   0        0        0     3287 2023-12-18 12:05:45.881008 gigachain_community-0.0.6/langchain_community/utilities/opaqueprompts.py
--rw-r--r--   0        0        0    11017 2023-12-18 12:05:45.881524 gigachain_community-0.0.6/langchain_community/utilities/openapi.py
--rw-r--r--   0        0        0     2462 2023-12-18 12:05:45.882200 gigachain_community-0.0.6/langchain_community/utilities/openweathermap.py
--rw-r--r--   0        0        0     3351 2023-12-18 12:05:45.882568 gigachain_community-0.0.6/langchain_community/utilities/outline.py
--rw-r--r--   0        0        0     2355 2023-12-18 12:05:45.883116 gigachain_community-0.0.6/langchain_community/utilities/portkey.py
--rw-r--r--   0        0        0    11246 2023-12-18 12:05:45.883973 gigachain_community-0.0.6/langchain_community/utilities/powerbi.py
--rw-r--r--   0        0        0     6936 2023-12-18 12:05:45.884535 gigachain_community-0.0.6/langchain_community/utilities/pubmed.py
--rw-r--r--   0        0        0     2159 2023-12-18 12:05:45.885022 gigachain_community-0.0.6/langchain_community/utilities/python.py
--rw-r--r--   0        0        0     4474 2023-12-18 12:05:45.885341 gigachain_community-0.0.6/langchain_community/utilities/reddit_search.py
--rw-r--r--   0        0        0     8221 2023-12-18 12:05:45.885856 gigachain_community-0.0.6/langchain_community/utilities/redis.py
--rw-r--r--   0        0        0     6992 2023-12-18 12:05:45.886179 gigachain_community-0.0.6/langchain_community/utilities/requests.py
--rw-r--r--   0        0        0     2220 2023-12-18 12:05:45.886517 gigachain_community-0.0.6/langchain_community/utilities/scenexplain.py
--rw-r--r--   0        0        0     5226 2023-12-18 12:05:45.887002 gigachain_community-0.0.6/langchain_community/utilities/searchapi.py
--rw-r--r--   0        0        0    16625 2023-12-18 12:05:45.887512 gigachain_community-0.0.6/langchain_community/utilities/searx_search.py
--rw-r--r--   0        0        0     8490 2023-12-18 12:05:45.889068 gigachain_community-0.0.6/langchain_community/utilities/serpapi.py
--rw-r--r--   0        0        0     7519 2023-12-18 12:05:45.889509 gigachain_community-0.0.6/langchain_community/utilities/spark_sql.py
--rw-r--r--   0        0        0    19639 2023-12-21 15:51:51.847139 gigachain_community-0.0.6/langchain_community/utilities/sql_database.py
--rw-r--r--   0        0        0     2639 2023-12-18 12:05:45.890765 gigachain_community-0.0.6/langchain_community/utilities/stackexchange.py
--rw-r--r--   0        0        0     5857 2023-12-18 12:05:45.891172 gigachain_community-0.0.6/langchain_community/utilities/steam.py
--rw-r--r--   0        0        0     6834 2023-12-18 12:05:45.891644 gigachain_community-0.0.6/langchain_community/utilities/tavily_search.py
--rw-r--r--   0        0        0     4006 2023-12-18 12:05:45.892063 gigachain_community-0.0.6/langchain_community/utilities/tensorflow_datasets.py
--rw-r--r--   0        0        0     3441 2023-12-18 12:05:45.892530 gigachain_community-0.0.6/langchain_community/utilities/twilio.py
--rw-r--r--   0        0        0     4072 2023-12-21 15:51:51.848192 gigachain_community-0.0.6/langchain_community/utilities/vertexai.py
--rw-r--r--   0        0        0     4045 2023-12-18 12:05:45.893264 gigachain_community-0.0.6/langchain_community/utilities/wikipedia.py
--rw-r--r--   0        0        0     2011 2023-12-18 12:05:45.893697 gigachain_community-0.0.6/langchain_community/utilities/wolfram_alpha.py
--rw-r--r--   0        0        0    11666 2023-12-18 12:05:45.894686 gigachain_community-0.0.6/langchain_community/utilities/zapier.py
--rw-r--r--   0        0        0        0 2023-12-18 12:05:45.894897 gigachain_community-0.0.6/langchain_community/utils/__init__.py
--rw-r--r--   0        0        0     2713 2023-12-18 12:05:45.895328 gigachain_community-0.0.6/langchain_community/utils/math.py
--rw-r--r--   0        0        0      264 2023-12-21 15:51:51.849060 gigachain_community-0.0.6/langchain_community/utils/openai.py
--rw-r--r--   0        0        0     1518 2023-12-18 12:05:45.896319 gigachain_community-0.0.6/langchain_community/utils/openai_functions.py
--rw-r--r--   0        0        0    15965 2023-12-21 15:51:51.850380 gigachain_community-0.0.6/langchain_community/vectorstores/__init__.py
--rw-r--r--   0        0        0    19780 2023-12-18 12:05:45.897986 gigachain_community-0.0.6/langchain_community/vectorstores/alibabacloud_opensearch.py
--rw-r--r--   0        0        0    15738 2023-12-18 12:05:45.898774 gigachain_community-0.0.6/langchain_community/vectorstores/analyticdb.py
--rw-r--r--   0        0        0    16632 2023-12-18 12:05:45.899285 gigachain_community-0.0.6/langchain_community/vectorstores/annoy.py
--rw-r--r--   0        0        0    28449 2023-12-18 12:05:45.900342 gigachain_community-0.0.6/langchain_community/vectorstores/astradb.py
--rw-r--r--   0        0        0    12136 2023-12-18 12:05:45.900865 gigachain_community-0.0.6/langchain_community/vectorstores/atlas.py
--rw-r--r--   0        0        0    21155 2023-12-18 12:05:45.918722 gigachain_community-0.0.6/langchain_community/vectorstores/awadb.py
--rw-r--r--   0        0        0    14522 2023-12-18 12:05:45.920951 gigachain_community-0.0.6/langchain_community/vectorstores/azure_cosmos_db.py
--rw-r--r--   0        0        0    27218 2023-12-18 12:05:45.921571 gigachain_community-0.0.6/langchain_community/vectorstores/azuresearch.py
--rw-r--r--   0        0        0    15034 2023-12-18 12:05:45.922399 gigachain_community-0.0.6/langchain_community/vectorstores/bageldb.py
--rw-r--r--   0        0        0    16548 2023-12-18 12:05:45.923166 gigachain_community-0.0.6/langchain_community/vectorstores/baiducloud_vector_search.py
--rw-r--r--   0        0        0    14809 2023-12-18 12:05:45.924380 gigachain_community-0.0.6/langchain_community/vectorstores/cassandra.py
--rw-r--r--   0        0        0    30367 2023-12-18 12:05:45.924915 gigachain_community-0.0.6/langchain_community/vectorstores/chroma.py
--rw-r--r--   0        0        0    10953 2023-12-21 15:51:51.851489 gigachain_community-0.0.6/langchain_community/vectorstores/clarifai.py
--rw-r--r--   0        0        0    17735 2023-12-18 12:05:45.926412 gigachain_community-0.0.6/langchain_community/vectorstores/clickhouse.py
--rw-r--r--   0        0        0    12713 2023-12-21 15:51:51.853117 gigachain_community-0.0.6/langchain_community/vectorstores/dashvector.py
--rw-r--r--   0        0        0    18360 2023-12-18 12:05:45.928909 gigachain_community-0.0.6/langchain_community/vectorstores/databricks_vector_search.py
--rw-r--r--   0        0        0    40265 2023-12-18 12:05:45.929819 gigachain_community-0.0.6/langchain_community/vectorstores/deeplake.py
--rw-r--r--   0        0        0    12973 2023-12-18 12:05:45.930835 gigachain_community-0.0.6/langchain_community/vectorstores/dingo.py
--rw-r--r--   0        0        0      236 2023-12-18 12:05:45.931359 gigachain_community-0.0.6/langchain_community/vectorstores/docarray/__init__.py
--rw-r--r--   0        0        0     6945 2023-12-18 12:05:45.931915 gigachain_community-0.0.6/langchain_community/vectorstores/docarray/base.py
--rw-r--r--   0        0        0     4044 2023-12-18 12:05:45.932338 gigachain_community-0.0.6/langchain_community/vectorstores/docarray/hnsw.py
--rw-r--r--   0        0        0     2418 2023-12-18 12:05:45.932697 gigachain_community-0.0.6/langchain_community/vectorstores/docarray/in_memory.py
--rw-r--r--   0        0        0    28714 2023-12-18 12:05:45.933055 gigachain_community-0.0.6/langchain_community/vectorstores/elastic_vector_search.py
--rw-r--r--   0        0        0    46536 2023-12-18 12:05:45.933608 gigachain_community-0.0.6/langchain_community/vectorstores/elasticsearch.py
--rw-r--r--   0        0        0    14183 2023-12-18 12:05:45.934415 gigachain_community-0.0.6/langchain_community/vectorstores/epsilla.py
--rw-r--r--   0        0        0    42989 2023-12-18 12:05:45.934999 gigachain_community-0.0.6/langchain_community/vectorstores/faiss.py
--rw-r--r--   0        0        0    26837 2023-12-18 12:05:45.935987 gigachain_community-0.0.6/langchain_community/vectorstores/hippo.py
--rw-r--r--   0        0        0    13642 2023-12-18 12:05:45.936884 gigachain_community-0.0.6/langchain_community/vectorstores/hologres.py
--rw-r--r--   0        0        0    14253 2023-12-28 13:38:34.506816 gigachain_community-0.0.6/langchain_community/vectorstores/jaguar.py
--rw-r--r--   0        0        0     4173 2023-12-18 12:05:45.938754 gigachain_community-0.0.6/langchain_community/vectorstores/lancedb.py
--rw-r--r--   0        0        0     7745 2023-12-18 12:05:45.939222 gigachain_community-0.0.6/langchain_community/vectorstores/llm_rails.py
--rw-r--r--   0        0        0    17047 2023-12-18 12:05:45.940104 gigachain_community-0.0.6/langchain_community/vectorstores/marqo.py
--rw-r--r--   0        0        0    21430 2023-12-21 15:51:51.855202 gigachain_community-0.0.6/langchain_community/vectorstores/matching_engine.py
--rw-r--r--   0        0        0    10400 2023-12-18 12:05:45.941286 gigachain_community-0.0.6/langchain_community/vectorstores/meilisearch.py
--rw-r--r--   0        0        0    31749 2023-12-18 12:05:45.941785 gigachain_community-0.0.6/langchain_community/vectorstores/milvus.py
--rw-r--r--   0        0        0    19047 2023-12-28 13:38:34.508044 gigachain_community-0.0.6/langchain_community/vectorstores/momento_vector_index.py
--rw-r--r--   0        0        0    13869 2023-12-21 15:51:51.856691 gigachain_community-0.0.6/langchain_community/vectorstores/mongodb_atlas.py
--rw-r--r--   0        0        0    22546 2023-12-18 12:05:45.943853 gigachain_community-0.0.6/langchain_community/vectorstores/myscale.py
--rw-r--r--   0        0        0    35000 2023-12-21 15:51:51.857828 gigachain_community-0.0.6/langchain_community/vectorstores/neo4j_vector.py
--rw-r--r--   0        0        0     5403 2023-12-18 12:05:45.944847 gigachain_community-0.0.6/langchain_community/vectorstores/nucliadb.py
--rw-r--r--   0        0        0    31850 2023-12-18 12:05:45.946289 gigachain_community-0.0.6/langchain_community/vectorstores/opensearch_vector_search.py
--rw-r--r--   0        0        0    17895 2023-12-18 12:05:45.948220 gigachain_community-0.0.6/langchain_community/vectorstores/pgembedding.py
--rw-r--r--   0        0        0     8891 2023-12-21 15:51:51.859006 gigachain_community-0.0.6/langchain_community/vectorstores/pgvecto_rs.py
--rw-r--r--   0        0        0    34006 2023-12-21 15:51:51.860255 gigachain_community-0.0.6/langchain_community/vectorstores/pgvector.py
--rw-r--r--   0        0        0    17517 2023-12-18 12:05:45.950012 gigachain_community-0.0.6/langchain_community/vectorstores/pinecone.py
--rw-r--r--   0        0        0    89408 2023-12-18 12:05:45.951827 gigachain_community-0.0.6/langchain_community/vectorstores/qdrant.py
--rw-r--r--   0        0        0      265 2023-12-18 12:05:45.952450 gigachain_community-0.0.6/langchain_community/vectorstores/redis/__init__.py
--rw-r--r--   0        0        0    54448 2023-12-18 12:05:45.954415 gigachain_community-0.0.6/langchain_community/vectorstores/redis/base.py
--rw-r--r--   0        0        0      420 2023-12-18 12:05:45.954942 gigachain_community-0.0.6/langchain_community/vectorstores/redis/constants.py
--rw-r--r--   0        0        0    16227 2023-12-18 12:05:45.956102 gigachain_community-0.0.6/langchain_community/vectorstores/redis/filters.py
--rw-r--r--   0        0        0    10419 2023-12-18 12:05:45.957786 gigachain_community-0.0.6/langchain_community/vectorstores/redis/schema.py
--rw-r--r--   0        0        0    12192 2023-12-18 12:05:45.958270 gigachain_community-0.0.6/langchain_community/vectorstores/rocksetdb.py
--rw-r--r--   0        0        0    19610 2023-12-18 12:05:45.958595 gigachain_community-0.0.6/langchain_community/vectorstores/scann.py
--rw-r--r--   0        0        0     9707 2023-12-28 13:38:34.509507 gigachain_community-0.0.6/langchain_community/vectorstores/semadb.py
--rw-r--r--   0        0        0    17628 2023-12-18 12:05:45.959791 gigachain_community-0.0.6/langchain_community/vectorstores/singlestoredb.py
--rw-r--r--   0        0        0    12375 2023-12-21 15:51:51.861914 gigachain_community-0.0.6/langchain_community/vectorstores/sklearn.py
--rw-r--r--   0        0        0     7316 2023-12-18 12:05:45.963006 gigachain_community-0.0.6/langchain_community/vectorstores/sqlitevss.py
--rw-r--r--   0        0        0    17150 2023-12-18 12:05:45.968600 gigachain_community-0.0.6/langchain_community/vectorstores/starrocks.py
--rw-r--r--   0        0        0    15175 2023-12-18 12:05:45.970976 gigachain_community-0.0.6/langchain_community/vectorstores/supabase.py
--rw-r--r--   0        0        0    14706 2023-12-28 13:38:34.510538 gigachain_community-0.0.6/langchain_community/vectorstores/surrealdb.py
--rw-r--r--   0        0        0     9557 2023-12-18 12:05:45.975992 gigachain_community-0.0.6/langchain_community/vectorstores/tair.py
--rw-r--r--   0        0        0    13927 2023-12-21 15:51:51.864636 gigachain_community-0.0.6/langchain_community/vectorstores/tencentvectordb.py
--rw-r--r--   0        0        0     4927 2023-12-18 12:05:45.980251 gigachain_community-0.0.6/langchain_community/vectorstores/tigris.py
--rw-r--r--   0        0        0    28826 2023-12-21 15:51:51.865840 gigachain_community-0.0.6/langchain_community/vectorstores/tiledb.py
--rw-r--r--   0        0        0    29831 2023-12-21 15:51:51.867775 gigachain_community-0.0.6/langchain_community/vectorstores/timescalevector.py
--rw-r--r--   0        0        0     9712 2023-12-18 12:05:45.986913 gigachain_community-0.0.6/langchain_community/vectorstores/typesense.py
--rw-r--r--   0        0        0     5888 2023-12-18 12:05:45.988954 gigachain_community-0.0.6/langchain_community/vectorstores/usearch.py
--rw-r--r--   0        0        0     2474 2023-12-18 12:05:45.989508 gigachain_community-0.0.6/langchain_community/vectorstores/utils.py
--rw-r--r--   0        0        0    12908 2023-12-18 12:05:45.990381 gigachain_community-0.0.6/langchain_community/vectorstores/vald.py
--rw-r--r--   0        0        0    19844 2023-12-18 12:05:45.990761 gigachain_community-0.0.6/langchain_community/vectorstores/vearch.py
--rw-r--r--   0        0        0    21275 2023-12-28 13:38:34.511972 gigachain_community-0.0.6/langchain_community/vectorstores/vectara.py
--rw-r--r--   0        0        0     9785 2023-12-18 12:05:45.998180 gigachain_community-0.0.6/langchain_community/vectorstores/vespa.py
--rw-r--r--   0        0        0    19226 2023-12-18 12:05:46.002110 gigachain_community-0.0.6/langchain_community/vectorstores/weaviate.py
--rw-r--r--   0        0        0     9032 2023-12-18 12:05:46.007223 gigachain_community-0.0.6/langchain_community/vectorstores/xata.py
--rw-r--r--   0        0        0    10761 2023-12-18 12:05:46.013574 gigachain_community-0.0.6/langchain_community/vectorstores/yellowbrick.py
--rw-r--r--   0        0        0    23192 2023-12-18 12:05:46.014090 gigachain_community-0.0.6/langchain_community/vectorstores/zep.py
--rw-r--r--   0        0        0     7575 2023-12-18 12:05:46.016389 gigachain_community-0.0.6/langchain_community/vectorstores/zilliz.py
--rw-r--r--   0        0        0     9698 2023-12-28 13:38:34.523967 gigachain_community-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     7261 1970-01-01 00:00:00.000000 gigachain_community-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1201 2023-12-21 15:51:51.774421 gigachain_community-0.0.6.1/README.md
+-rw-r--r--   0        0        0      307 2023-12-18 12:05:45.464203 gigachain_community-0.0.6.1/langchain_community/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-18 12:05:45.464419 gigachain_community-0.0.6.1/langchain_community/adapters/__init__.py
+-rw-r--r--   0        0        0    12143 2023-12-21 15:51:51.775428 gigachain_community-0.0.6.1/langchain_community/adapters/openai.py
+-rw-r--r--   0        0        0     3327 2023-12-18 12:05:45.466331 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/__init__.py
+-rw-r--r--   0        0        0       25 2023-12-18 12:05:45.466917 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/ainetwork/__init__.py
+-rw-r--r--   0        0        0     1781 2023-12-18 12:05:45.467514 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/ainetwork/toolkit.py
+-rw-r--r--   0        0        0        0 2023-12-18 12:05:45.467736 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/amadeus/__init__.py
+-rw-r--r--   0        0        0      961 2023-12-18 12:05:45.468139 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/amadeus/toolkit.py
+-rw-r--r--   0        0        0     1035 2023-12-18 12:05:45.468506 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/azure_cognitive_services.py
+-rw-r--r--   0        0        0      397 2023-12-18 12:05:45.468850 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/base.py
+-rw-r--r--   0        0        0        0 2023-12-18 12:05:45.469039 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/clickup/__init__.py
+-rw-r--r--   0        0        0     3594 2023-12-18 12:05:45.469520 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/clickup/toolkit.py
+-rw-r--r--   0        0        0     1091 2023-12-18 12:05:45.470285 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/csv/__init__.py
+-rw-r--r--   0        0        0      177 2023-12-18 12:05:45.470616 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/file_management/__init__.py
+-rw-r--r--   0        0        0     3250 2023-12-18 12:05:45.471261 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/file_management/toolkit.py
+-rw-r--r--   0        0        0       22 2023-12-18 12:05:45.471646 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/github/__init__.py
+-rw-r--r--   0        0        0    10135 2023-12-21 15:51:51.776418 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/github/toolkit.py
+-rw-r--r--   0        0        0       22 2023-12-18 12:05:45.472496 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/gitlab/__init__.py
+-rw-r--r--   0        0        0     2904 2023-12-18 12:05:45.472989 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/gitlab/toolkit.py
+-rw-r--r--   0        0        0       21 2023-12-18 12:05:45.473348 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/gmail/__init__.py
+-rw-r--r--   0        0        0     2045 2023-12-18 12:05:45.473719 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/gmail/toolkit.py
+-rw-r--r--   0        0        0       20 2023-12-18 12:05:45.474062 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/jira/__init__.py
+-rw-r--r--   0        0        0     2227 2023-12-18 12:05:45.474505 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/jira/toolkit.py
+-rw-r--r--   0        0        0       18 2023-12-18 12:05:45.474878 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/json/__init__.py
+-rw-r--r--   0        0        0     1894 2023-12-18 12:05:45.475275 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/json/base.py
+-rw-r--r--   0        0        0     3288 2023-12-18 12:05:45.475625 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/json/prompt.py
+-rw-r--r--   0        0        0      595 2023-12-18 12:05:45.475954 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/json/toolkit.py
+-rw-r--r--   0        0        0       23 2023-12-18 12:05:45.476309 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/multion/__init__.py
+-rw-r--r--   0        0        0     1190 2023-12-18 12:05:45.476676 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/multion/toolkit.py
+-rw-r--r--   0        0        0       19 2023-12-18 12:05:45.477080 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/nasa/__init__.py
+-rw-r--r--   0        0        0     1931 2023-12-18 12:05:45.477469 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/nasa/toolkit.py
+-rw-r--r--   0        0        0        0 2023-12-18 12:05:45.477737 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/nla/__init__.py
+-rw-r--r--   0        0        0     2038 2023-12-18 12:05:45.478181 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/nla/tool.py
+-rw-r--r--   0        0        0     4228 2023-12-18 12:05:45.478766 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/nla/toolkit.py
+-rw-r--r--   0        0        0       25 2023-12-18 12:05:45.479165 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/office365/__init__.py
+-rw-r--r--   0        0        0     1812 2023-12-18 12:05:45.479543 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/office365/toolkit.py
+-rw-r--r--   0        0        0       26 2023-12-18 12:05:45.479989 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/openapi/__init__.py
+-rw-r--r--   0        0        0     2870 2023-12-18 12:05:45.480437 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/openapi/base.py
+-rw-r--r--   0        0        0    12987 2023-12-18 12:05:45.481612 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/openapi/planner.py
+-rw-r--r--   0        0        0    19382 2023-12-18 12:05:45.482208 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/openapi/planner_prompt.py
+-rw-r--r--   0        0        0     3174 2023-12-18 12:05:45.482651 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/openapi/prompt.py
+-rw-r--r--   0        0        0     2557 2023-12-18 12:05:45.483038 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/openapi/spec.py
+-rw-r--r--   0        0        0     3317 2023-12-18 12:05:45.483317 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/openapi/toolkit.py
+-rw-r--r--   0        0        0      174 2023-12-18 12:05:45.483588 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/playwright/__init__.py
+-rw-r--r--   0        0        0     4274 2023-12-18 12:05:45.483947 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/playwright/toolkit.py
+-rw-r--r--   0        0        0       22 2023-12-18 12:05:45.484213 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/powerbi/__init__.py
+-rw-r--r--   0        0        0     2507 2023-12-18 12:05:45.484545 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/powerbi/base.py
+-rw-r--r--   0        0        0     2649 2023-12-18 12:05:45.484863 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/powerbi/chat_base.py
+-rw-r--r--   0        0        0     5098 2023-12-18 12:05:45.485270 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/powerbi/prompt.py
+-rw-r--r--   0        0        0     3771 2023-12-18 12:05:45.485517 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/powerbi/toolkit.py
+-rw-r--r--   0        0        0       21 2023-12-18 12:05:45.485842 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/slack/__init__.py
+-rw-r--r--   0        0        0     1114 2023-12-18 12:05:45.486216 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/slack/toolkit.py
+-rw-r--r--   0        0        0       23 2023-12-18 12:05:45.486932 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/spark_sql/__init__.py
+-rw-r--r--   0        0        0     2355 2023-12-18 12:05:45.487251 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/spark_sql/base.py
+-rw-r--r--   0        0        0     2297 2023-12-18 12:05:45.487719 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/spark_sql/prompt.py
+-rw-r--r--   0        0        0     1084 2023-12-18 12:05:45.488627 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/spark_sql/toolkit.py
+-rw-r--r--   0        0        0       17 2023-12-18 12:05:45.489163 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/sql/__init__.py
+-rw-r--r--   0        0        0     3866 2023-12-18 12:05:45.489752 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/sql/base.py
+-rw-r--r--   0        0        0     2727 2023-12-18 12:05:45.490038 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/sql/prompt.py
+-rw-r--r--   0        0        0     2862 2023-12-18 12:05:45.490548 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/sql/toolkit.py
+-rw-r--r--   0        0        0       21 2023-12-18 12:05:45.490899 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/steam/__init__.py
+-rw-r--r--   0        0        0     1465 2023-12-18 12:05:45.491412 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/steam/toolkit.py
+-rw-r--r--   0        0        0     1095 2023-12-18 12:05:45.491874 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/xorbits/__init__.py
+-rw-r--r--   0        0        0       22 2023-12-18 12:05:45.492214 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/zapier/__init__.py
+-rw-r--r--   0        0        0     1933 2023-12-18 12:05:45.492667 gigachain_community-0.0.6.1/langchain_community/agent_toolkits/zapier/toolkit.py
+-rw-r--r--   0        0        0    58113 2023-12-21 15:51:51.777487 gigachain_community-0.0.6.1/langchain_community/cache.py
+-rw-r--r--   0        0        0     2671 2023-12-18 12:05:45.494039 gigachain_community-0.0.6.1/langchain_community/callbacks/__init__.py
+-rw-r--r--   0        0        0    14408 2023-12-18 12:05:45.494709 gigachain_community-0.0.6.1/langchain_community/callbacks/aim_callback.py
+-rw-r--r--   0        0        0    14820 2023-12-18 12:05:45.495433 gigachain_community-0.0.6.1/langchain_community/callbacks/argilla_callback.py
+-rw-r--r--   0        0        0     7438 2023-12-18 12:05:45.496089 gigachain_community-0.0.6.1/langchain_community/callbacks/arize_callback.py
+-rw-r--r--   0        0        0    11266 2023-12-18 12:05:45.496863 gigachain_community-0.0.6.1/langchain_community/callbacks/arthur_callback.py
+-rw-r--r--   0        0        0    18897 2023-12-18 12:05:45.497277 gigachain_community-0.0.6.1/langchain_community/callbacks/clearml_callback.py
+-rw-r--r--   0        0        0    23193 2023-12-18 12:05:45.497760 gigachain_community-0.0.6.1/langchain_community/callbacks/comet_ml_callback.py
+-rw-r--r--   0        0        0     6340 2023-12-18 12:05:45.498346 gigachain_community-0.0.6.1/langchain_community/callbacks/confident_callback.py
+-rw-r--r--   0        0        0     6498 2023-12-18 12:05:45.498833 gigachain_community-0.0.6.1/langchain_community/callbacks/context_callback.py
+-rw-r--r--   0        0        0    13138 2023-12-18 12:05:45.499879 gigachain_community-0.0.6.1/langchain_community/callbacks/flyte_callback.py
+-rw-r--r--   0        0        0     2587 2023-12-18 12:05:45.500223 gigachain_community-0.0.6.1/langchain_community/callbacks/human.py
+-rw-r--r--   0        0        0     9224 2023-12-18 12:05:45.500727 gigachain_community-0.0.6.1/langchain_community/callbacks/infino_callback.py
+-rw-r--r--   0        0        0    13880 2023-12-18 12:05:45.501822 gigachain_community-0.0.6.1/langchain_community/callbacks/labelstudio_callback.py
+-rw-r--r--   0        0        0    20527 2023-12-18 12:05:45.502476 gigachain_community-0.0.6.1/langchain_community/callbacks/llmonitor_callback.py
+-rw-r--r--   0        0        0     1891 2023-12-18 12:05:45.503349 gigachain_community-0.0.6.1/langchain_community/callbacks/manager.py
+-rw-r--r--   0        0        0    24156 2023-12-18 12:05:45.503686 gigachain_community-0.0.6.1/langchain_community/callbacks/mlflow_callback.py
+-rw-r--r--   0        0        0     7309 2023-12-18 12:05:45.504428 gigachain_community-0.0.6.1/langchain_community/callbacks/openai_info.py
+-rw-r--r--   0        0        0     5535 2023-12-18 12:05:45.505111 gigachain_community-0.0.6.1/langchain_community/callbacks/promptlayer_callback.py
+-rw-r--r--   0        0        0     8758 2023-12-18 12:05:45.506012 gigachain_community-0.0.6.1/langchain_community/callbacks/sagemaker_callback.py
+-rw-r--r--   0        0        0     3211 2023-12-18 12:05:45.506509 gigachain_community-0.0.6.1/langchain_community/callbacks/streamlit/__init__.py
+-rw-r--r--   0        0        0     5435 2023-12-18 12:05:45.507080 gigachain_community-0.0.6.1/langchain_community/callbacks/streamlit/mutable_expander.py
+-rw-r--r--   0        0        0    15534 2023-12-18 12:05:45.507739 gigachain_community-0.0.6.1/langchain_community/callbacks/streamlit/streamlit_callback_handler.py
+-rw-r--r--   0        0        0      498 2023-12-18 12:05:45.508143 gigachain_community-0.0.6.1/langchain_community/callbacks/tracers/__init__.py
+-rw-r--r--   0        0        0     4713 2023-12-21 15:51:51.778605 gigachain_community-0.0.6.1/langchain_community/callbacks/tracers/comet.py
+-rw-r--r--   0        0        0    19114 2023-12-18 12:05:45.509395 gigachain_community-0.0.6.1/langchain_community/callbacks/tracers/wandb.py
+-rw-r--r--   0        0        0     4526 2023-12-18 12:05:45.510089 gigachain_community-0.0.6.1/langchain_community/callbacks/trubrics_callback.py
+-rw-r--r--   0        0        0     8505 2023-12-18 12:05:45.510787 gigachain_community-0.0.6.1/langchain_community/callbacks/utils.py
+-rw-r--r--   0        0        0    20601 2023-12-18 12:05:45.511652 gigachain_community-0.0.6.1/langchain_community/callbacks/wandb_callback.py
+-rw-r--r--   0        0        0     8067 2023-12-18 12:05:45.512609 gigachain_community-0.0.6.1/langchain_community/callbacks/whylabs_callback.py
+-rw-r--r--   0        0        0      452 2023-12-18 12:05:45.513350 gigachain_community-0.0.6.1/langchain_community/chat_loaders/__init__.py
+-rw-r--r--   0        0        0      444 2023-12-18 12:05:45.513788 gigachain_community-0.0.6.1/langchain_community/chat_loaders/base.py
+-rw-r--r--   0        0        0     2462 2023-12-18 12:05:45.514215 gigachain_community-0.0.6.1/langchain_community/chat_loaders/facebook_messenger.py
+-rw-r--r--   0        0        0     4048 2023-12-18 12:05:45.514652 gigachain_community-0.0.6.1/langchain_community/chat_loaders/gmail.py
+-rw-r--r--   0        0        0     6768 2023-12-21 15:51:51.779551 gigachain_community-0.0.6.1/langchain_community/chat_loaders/imessage.py
+-rw-r--r--   0        0        0     5742 2023-12-18 12:05:45.515939 gigachain_community-0.0.6.1/langchain_community/chat_loaders/langsmith.py
+-rw-r--r--   0        0        0     3112 2023-12-18 12:05:45.516606 gigachain_community-0.0.6.1/langchain_community/chat_loaders/slack.py
+-rw-r--r--   0        0        0     5390 2023-12-18 12:05:45.517563 gigachain_community-0.0.6.1/langchain_community/chat_loaders/telegram.py
+-rw-r--r--   0        0        0     3270 2023-12-18 12:05:45.517951 gigachain_community-0.0.6.1/langchain_community/chat_loaders/utils.py
+-rw-r--r--   0        0        0     4280 2023-12-18 12:05:45.518507 gigachain_community-0.0.6.1/langchain_community/chat_loaders/whatsapp.py
+-rw-r--r--   0        0        0     2570 2023-12-18 12:05:45.519149 gigachain_community-0.0.6.1/langchain_community/chat_message_histories/__init__.py
+-rw-r--r--   0        0        0     4127 2023-12-18 12:05:45.519995 gigachain_community-0.0.6.1/langchain_community/chat_message_histories/astradb.py
+-rw-r--r--   0        0        0     2392 2023-12-18 12:05:45.520478 gigachain_community-0.0.6.1/langchain_community/chat_message_histories/cassandra.py
+-rw-r--r--   0        0        0     6510 2023-12-18 12:05:45.521121 gigachain_community-0.0.6.1/langchain_community/chat_message_histories/cosmos_db.py
+-rw-r--r--   0        0        0     5810 2023-12-18 12:05:45.521680 gigachain_community-0.0.6.1/langchain_community/chat_message_histories/dynamodb.py
+-rw-r--r--   0        0        0     6836 2023-12-28 13:38:34.455277 gigachain_community-0.0.6.1/langchain_community/chat_message_histories/elasticsearch.py
+-rw-r--r--   0        0        0     1379 2023-12-18 12:05:45.522767 gigachain_community-0.0.6.1/langchain_community/chat_message_histories/file.py
+-rw-r--r--   0        0        0     3349 2023-12-18 12:05:45.523479 gigachain_community-0.0.6.1/langchain_community/chat_message_histories/firestore.py
+-rw-r--r--   0        0        0      633 2023-12-18 12:05:45.524050 gigachain_community-0.0.6.1/langchain_community/chat_message_histories/in_memory.py
+-rw-r--r--   0        0        0     7112 2023-12-18 12:05:45.524641 gigachain_community-0.0.6.1/langchain_community/chat_message_histories/momento.py
+-rw-r--r--   0        0        0     2734 2023-12-18 12:05:45.524978 gigachain_community-0.0.6.1/langchain_community/chat_message_histories/mongodb.py
+-rw-r--r--   0        0        0     4288 2023-12-18 12:05:45.525750 gigachain_community-0.0.6.1/langchain_community/chat_message_histories/neo4j.py
+-rw-r--r--   0        0        0     2659 2023-12-18 12:05:45.526184 gigachain_community-0.0.6.1/langchain_community/chat_message_histories/postgres.py
+-rw-r--r--   0        0        0     1971 2023-12-18 12:05:45.526547 gigachain_community-0.0.6.1/langchain_community/chat_message_histories/redis.py
+-rw-r--r--   0        0        0     9515 2023-12-18 12:05:45.526952 gigachain_community-0.0.6.1/langchain_community/chat_message_histories/rocksetdb.py
+-rw-r--r--   0        0        0    10331 2023-12-18 12:05:45.527836 gigachain_community-0.0.6.1/langchain_community/chat_message_histories/singlestoredb.py
+-rw-r--r--   0        0        0     4717 2023-12-18 12:05:45.528385 gigachain_community-0.0.6.1/langchain_community/chat_message_histories/sql.py
+-rw-r--r--   0        0        0     1176 2023-12-18 12:05:45.528853 gigachain_community-0.0.6.1/langchain_community/chat_message_histories/streamlit.py
+-rw-r--r--   0        0        0     2148 2023-12-18 12:05:45.529276 gigachain_community-0.0.6.1/langchain_community/chat_message_histories/upstash_redis.py
+-rw-r--r--   0        0        0     4652 2023-12-18 12:05:45.529848 gigachain_community-0.0.6.1/langchain_community/chat_message_histories/xata.py
+-rw-r--r--   0        0        0     6452 2023-12-18 12:05:45.530494 gigachain_community-0.0.6.1/langchain_community/chat_message_histories/zep.py
+-rw-r--r--   0        0        0     3403 2023-12-28 13:38:34.456648 gigachain_community-0.0.6.1/langchain_community/chat_models/__init__.py
+-rw-r--r--   0        0        0     7963 2023-12-18 12:05:45.531534 gigachain_community-0.0.6.1/langchain_community/chat_models/anthropic.py
+-rw-r--r--   0        0        0     7945 2023-12-18 12:05:45.532200 gigachain_community-0.0.6.1/langchain_community/chat_models/anyscale.py
+-rw-r--r--   0        0        0    11171 2023-12-28 13:38:34.458109 gigachain_community-0.0.6.1/langchain_community/chat_models/azure_openai.py
+-rw-r--r--   0        0        0     6007 2023-12-18 12:05:45.533360 gigachain_community-0.0.6.1/langchain_community/chat_models/azureml_endpoint.py
+-rw-r--r--   0        0        0    10083 2023-12-18 12:05:45.534129 gigachain_community-0.0.6.1/langchain_community/chat_models/baichuan.py
+-rw-r--r--   0        0        0    12467 2023-12-21 15:51:51.781739 gigachain_community-0.0.6.1/langchain_community/chat_models/baidu_qianfan_endpoint.py
+-rw-r--r--   0        0        0     4284 2023-12-18 12:05:45.535676 gigachain_community-0.0.6.1/langchain_community/chat_models/bedrock.py
+-rw-r--r--   0        0        0     7571 2023-12-18 12:05:45.536327 gigachain_community-0.0.6.1/langchain_community/chat_models/cohere.py
+-rw-r--r--   0        0        0     1250 2023-12-18 12:05:45.537272 gigachain_community-0.0.6.1/langchain_community/chat_models/databricks.py
+-rw-r--r--   0        0        0     7874 2023-12-18 12:05:45.537817 gigachain_community-0.0.6.1/langchain_community/chat_models/ernie.py
+-rw-r--r--   0        0        0     5586 2023-12-18 12:05:45.538348 gigachain_community-0.0.6.1/langchain_community/chat_models/everlyai.py
+-rw-r--r--   0        0        0     3217 2023-12-18 12:05:45.538739 gigachain_community-0.0.6.1/langchain_community/chat_models/fake.py
+-rw-r--r--   0        0        0    11742 2023-12-21 15:51:51.782873 gigachain_community-0.0.6.1/langchain_community/chat_models/fireworks.py
+-rw-r--r--   0        0        0     6225 2023-12-21 15:51:51.785824 gigachain_community-0.0.6.1/langchain_community/chat_models/gigachat.py
+-rw-r--r--   0        0        0    11526 2023-12-18 12:05:45.540634 gigachain_community-0.0.6.1/langchain_community/chat_models/google_palm.py
+-rw-r--r--   0        0        0    12749 2023-12-28 13:38:34.459453 gigachain_community-0.0.6.1/langchain_community/chat_models/gpt_router.py
+-rw-r--r--   0        0        0     5549 2023-12-28 13:38:34.459951 gigachain_community-0.0.6.1/langchain_community/chat_models/huggingface.py
+-rw-r--r--   0        0        0     4202 2023-12-18 12:05:45.541184 gigachain_community-0.0.6.1/langchain_community/chat_models/human.py
+-rw-r--r--   0        0        0    10549 2023-12-18 12:05:45.541892 gigachain_community-0.0.6.1/langchain_community/chat_models/hunyuan.py
+-rw-r--r--   0        0        0     7654 2023-12-18 12:05:45.542512 gigachain_community-0.0.6.1/langchain_community/chat_models/javelin_ai_gateway.py
+-rw-r--r--   0        0        0    15167 2023-12-18 12:05:45.542994 gigachain_community-0.0.6.1/langchain_community/chat_models/jinachat.py
+-rw-r--r--   0        0        0    10588 2023-12-18 12:05:45.543497 gigachain_community-0.0.6.1/langchain_community/chat_models/konko.py
+-rw-r--r--   0        0        0    15671 2023-12-18 12:05:45.544541 gigachain_community-0.0.6.1/langchain_community/chat_models/litellm.py
+-rw-r--r--   0        0        0      967 2023-12-21 15:51:51.787479 gigachain_community-0.0.6.1/langchain_community/chat_models/meta.py
+-rw-r--r--   0        0        0     3180 2023-12-18 12:05:45.545432 gigachain_community-0.0.6.1/langchain_community/chat_models/minimax.py
+-rw-r--r--   0        0        0     7412 2023-12-18 12:05:45.546073 gigachain_community-0.0.6.1/langchain_community/chat_models/mlflow.py
+-rw-r--r--   0        0        0     7241 2023-12-18 12:05:45.546694 gigachain_community-0.0.6.1/langchain_community/chat_models/mlflow_ai_gateway.py
+-rw-r--r--   0        0        0    13165 2023-12-28 13:38:34.460887 gigachain_community-0.0.6.1/langchain_community/chat_models/ollama.py
+-rw-r--r--   0        0        0    26580 2023-12-21 15:51:51.789695 gigachain_community-0.0.6.1/langchain_community/chat_models/openai.py
+-rw-r--r--   0        0        0    11281 2023-12-18 12:05:45.550648 gigachain_community-0.0.6.1/langchain_community/chat_models/pai_eas_endpoint.py
+-rw-r--r--   0        0        0     5261 2023-12-18 12:05:45.551381 gigachain_community-0.0.6.1/langchain_community/chat_models/promptlayer_openai.py
+-rw-r--r--   0        0        0    14047 2023-12-21 15:51:51.793738 gigachain_community-0.0.6.1/langchain_community/chat_models/tongyi.py
+-rw-r--r--   0        0        0    14385 2023-12-28 13:38:34.462031 gigachain_community-0.0.6.1/langchain_community/chat_models/vertexai.py
+-rw-r--r--   0        0        0     5119 2023-12-21 15:51:51.797089 gigachain_community-0.0.6.1/langchain_community/chat_models/volcengine_maas.py
+-rw-r--r--   0        0        0     9392 2023-12-21 15:51:51.798113 gigachain_community-0.0.6.1/langchain_community/chat_models/yandex.py
+-rw-r--r--   0        0        0      549 2023-12-18 12:05:45.555730 gigachain_community-0.0.6.1/langchain_community/docstore/__init__.py
+-rw-r--r--   0        0        0     1090 2023-12-18 12:05:45.556119 gigachain_community-0.0.6.1/langchain_community/docstore/arbitrary_fn.py
+-rw-r--r--   0        0        0      833 2023-12-18 12:05:45.556954 gigachain_community-0.0.6.1/langchain_community/docstore/base.py
+-rw-r--r--   0        0        0       70 2023-12-18 12:05:45.557366 gigachain_community-0.0.6.1/langchain_community/docstore/document.py
+-rw-r--r--   0        0        0     1610 2023-12-18 12:05:45.557773 gigachain_community-0.0.6.1/langchain_community/docstore/in_memory.py
+-rw-r--r--   0        0        0     1487 2023-12-18 12:05:45.558219 gigachain_community-0.0.6.1/langchain_community/docstore/wikipedia.py
+-rw-r--r--   0        0        0    16095 2023-12-28 13:38:34.463521 gigachain_community-0.0.6.1/langchain_community/document_loaders/__init__.py
+-rw-r--r--   0        0        0     2841 2023-12-18 12:05:45.559522 gigachain_community-0.0.6.1/langchain_community/document_loaders/acreom.py
+-rw-r--r--   0        0        0    10240 2023-12-18 12:05:45.560037 gigachain_community-0.0.6.1/langchain_community/document_loaders/airbyte.py
+-rw-r--r--   0        0        0      815 2023-12-18 12:05:45.560483 gigachain_community-0.0.6.1/langchain_community/document_loaders/airbyte_json.py
+-rw-r--r--   0        0        0     1281 2023-12-18 12:05:45.560843 gigachain_community-0.0.6.1/langchain_community/document_loaders/airtable.py
+-rw-r--r--   0        0        0     2759 2023-12-18 12:05:45.561222 gigachain_community-0.0.6.1/langchain_community/document_loaders/apify_dataset.py
+-rw-r--r--   0        0        0     5272 2023-12-18 12:05:45.561756 gigachain_community-0.0.6.1/langchain_community/document_loaders/arcgis_loader.py
+-rw-r--r--   0        0        0      879 2023-12-28 13:38:34.464672 gigachain_community-0.0.6.1/langchain_community/document_loaders/arxiv.py
+-rw-r--r--   0        0        0     4218 2023-12-18 12:05:45.562628 gigachain_community-0.0.6.1/langchain_community/document_loaders/assemblyai.py
+-rw-r--r--   0        0        0     8129 2023-12-18 12:05:45.563265 gigachain_community-0.0.6.1/langchain_community/document_loaders/async_html.py
+-rw-r--r--   0        0        0      563 2023-12-18 12:05:45.563932 gigachain_community-0.0.6.1/langchain_community/document_loaders/azlyrics.py
+-rw-r--r--   0        0        0     1545 2023-12-18 12:05:45.564679 gigachain_community-0.0.6.1/langchain_community/document_loaders/azure_ai_data.py
+-rw-r--r--   0        0        0     1582 2023-12-18 12:05:45.565135 gigachain_community-0.0.6.1/langchain_community/document_loaders/azure_blob_storage_container.py
+-rw-r--r--   0        0        0     1644 2023-12-18 12:05:45.565693 gigachain_community-0.0.6.1/langchain_community/document_loaders/azure_blob_storage_file.py
+-rw-r--r--   0        0        0     1857 2023-12-18 12:05:45.566128 gigachain_community-0.0.6.1/langchain_community/document_loaders/baiducloud_bos_directory.py
+-rw-r--r--   0        0        0     1931 2023-12-18 12:05:45.566645 gigachain_community-0.0.6.1/langchain_community/document_loaders/baiducloud_bos_file.py
+-rw-r--r--   0        0        0     3175 2023-12-18 12:05:45.567038 gigachain_community-0.0.6.1/langchain_community/document_loaders/base.py
+-rw-r--r--   0        0        0     6992 2023-12-18 12:05:45.567647 gigachain_community-0.0.6.1/langchain_community/document_loaders/base_o365.py
+-rw-r--r--   0        0        0     3922 2023-12-18 12:05:45.568154 gigachain_community-0.0.6.1/langchain_community/document_loaders/bibtex.py
+-rw-r--r--   0        0        0     3673 2023-12-18 12:05:45.568593 gigachain_community-0.0.6.1/langchain_community/document_loaders/bigquery.py
+-rw-r--r--   0        0        0     2736 2023-12-18 12:05:45.569329 gigachain_community-0.0.6.1/langchain_community/document_loaders/bilibili.py
+-rw-r--r--   0        0        0    10302 2023-12-18 12:05:45.569842 gigachain_community-0.0.6.1/langchain_community/document_loaders/blackboard.py
+-rw-r--r--   0        0        0      374 2023-12-18 12:05:45.570390 gigachain_community-0.0.6.1/langchain_community/document_loaders/blob_loaders/__init__.py
+-rw-r--r--   0        0        0     5340 2023-12-18 12:05:45.571009 gigachain_community-0.0.6.1/langchain_community/document_loaders/blob_loaders/file_system.py
+-rw-r--r--   0        0        0     6636 2023-12-18 12:05:45.571991 gigachain_community-0.0.6.1/langchain_community/document_loaders/blob_loaders/schema.py
+-rw-r--r--   0        0        0     1526 2023-12-18 12:05:45.572418 gigachain_community-0.0.6.1/langchain_community/document_loaders/blob_loaders/youtube_audio.py
+-rw-r--r--   0        0        0     5709 2023-12-18 12:05:45.573013 gigachain_community-0.0.6.1/langchain_community/document_loaders/blockchain.py
+-rw-r--r--   0        0        0     1047 2023-12-18 12:05:45.573408 gigachain_community-0.0.6.1/langchain_community/document_loaders/brave_search.py
+-rw-r--r--   0        0        0     2124 2023-12-18 12:05:45.573742 gigachain_community-0.0.6.1/langchain_community/document_loaders/browserless.py
+-rw-r--r--   0        0        0     1986 2023-12-18 12:05:45.574097 gigachain_community-0.0.6.1/langchain_community/document_loaders/chatgpt.py
+-rw-r--r--   0        0        0     2746 2023-12-18 12:05:45.574483 gigachain_community-0.0.6.1/langchain_community/document_loaders/chromium.py
+-rw-r--r--   0        0        0      527 2023-12-18 12:05:45.575010 gigachain_community-0.0.6.1/langchain_community/document_loaders/college_confidential.py
+-rw-r--r--   0        0        0     3269 2023-12-18 12:05:45.575773 gigachain_community-0.0.6.1/langchain_community/document_loaders/concurrent.py
+-rw-r--r--   0        0        0    27612 2023-12-18 12:05:45.576326 gigachain_community-0.0.6.1/langchain_community/document_loaders/confluence.py
+-rw-r--r--   0        0        0     1052 2023-12-18 12:05:45.576792 gigachain_community-0.0.6.1/langchain_community/document_loaders/conllu.py
+-rw-r--r--   0        0        0     3649 2023-12-18 12:05:45.577211 gigachain_community-0.0.6.1/langchain_community/document_loaders/couchbase.py
+-rw-r--r--   0        0        0     5926 2023-12-18 12:05:45.577752 gigachain_community-0.0.6.1/langchain_community/document_loaders/csv_loader.py
+-rw-r--r--   0        0        0     6617 2023-12-18 12:05:45.578545 gigachain_community-0.0.6.1/langchain_community/document_loaders/cube_semantic.py
+-rw-r--r--   0        0        0     4937 2023-12-18 12:05:45.579652 gigachain_community-0.0.6.1/langchain_community/document_loaders/datadog_logs.py
+-rw-r--r--   0        0        0     1923 2023-12-18 12:05:45.580180 gigachain_community-0.0.6.1/langchain_community/document_loaders/dataframe.py
+-rw-r--r--   0        0        0     2054 2023-12-18 12:05:45.580587 gigachain_community-0.0.6.1/langchain_community/document_loaders/diffbot.py
+-rw-r--r--   0        0        0     5942 2023-12-28 13:38:34.465530 gigachain_community-0.0.6.1/langchain_community/document_loaders/directory.py
+-rw-r--r--   0        0        0     1237 2023-12-18 12:05:45.581567 gigachain_community-0.0.6.1/langchain_community/document_loaders/discord.py
+-rw-r--r--   0        0        0     3146 2023-12-28 13:38:34.466027 gigachain_community-0.0.6.1/langchain_community/document_loaders/doc_intelligence.py
+-rw-r--r--   0        0        0    13450 2023-12-18 12:05:45.582298 gigachain_community-0.0.6.1/langchain_community/document_loaders/docugami.py
+-rw-r--r--   0        0        0     1852 2023-12-21 15:51:51.799258 gigachain_community-0.0.6.1/langchain_community/document_loaders/docusaurus.py
+-rw-r--r--   0        0        0     6229 2023-12-18 12:05:45.583083 gigachain_community-0.0.6.1/langchain_community/document_loaders/dropbox.py
+-rw-r--r--   0        0        0     3150 2023-12-18 12:05:45.583436 gigachain_community-0.0.6.1/langchain_community/document_loaders/duckdb_loader.py
+-rw-r--r--   0        0        0     3834 2023-12-18 12:05:45.583873 gigachain_community-0.0.6.1/langchain_community/document_loaders/email.py
+-rw-r--r--   0        0        0     1496 2023-12-18 12:05:45.584255 gigachain_community-0.0.6.1/langchain_community/document_loaders/epub.py
+-rw-r--r--   0        0        0     7798 2023-12-18 12:05:45.584871 gigachain_community-0.0.6.1/langchain_community/document_loaders/etherscan.py
+-rw-r--r--   0        0        0     5757 2023-12-18 12:05:45.585493 gigachain_community-0.0.6.1/langchain_community/document_loaders/evernote.py
+-rw-r--r--   0        0        0     1687 2023-12-18 12:05:45.585995 gigachain_community-0.0.6.1/langchain_community/document_loaders/excel.py
+-rw-r--r--   0        0        0     1270 2023-12-18 12:05:45.586905 gigachain_community-0.0.6.1/langchain_community/document_loaders/facebook_chat.py
+-rw-r--r--   0        0        0     2254 2023-12-18 12:05:45.587314 gigachain_community-0.0.6.1/langchain_community/document_loaders/fauna.py
+-rw-r--r--   0        0        0     1543 2023-12-18 12:05:45.587742 gigachain_community-0.0.6.1/langchain_community/document_loaders/figma.py
+-rw-r--r--   0        0        0     2118 2023-12-18 12:05:45.588204 gigachain_community-0.0.6.1/langchain_community/document_loaders/gcs_directory.py
+-rw-r--r--   0        0        0     3138 2023-12-28 13:38:34.466902 gigachain_community-0.0.6.1/langchain_community/document_loaders/gcs_file.py
+-rw-r--r--   0        0        0     6390 2023-12-18 12:05:45.589033 gigachain_community-0.0.6.1/langchain_community/document_loaders/generic.py
+-rw-r--r--   0        0        0     2518 2023-12-18 12:05:45.589513 gigachain_community-0.0.6.1/langchain_community/document_loaders/geodataframe.py
+-rw-r--r--   0        0        0     4116 2023-12-18 12:05:45.590181 gigachain_community-0.0.6.1/langchain_community/document_loaders/git.py
+-rw-r--r--   0        0        0     3453 2023-12-18 12:05:45.590495 gigachain_community-0.0.6.1/langchain_community/document_loaders/gitbook.py
+-rw-r--r--   0        0        0     6973 2023-12-18 12:05:45.590928 gigachain_community-0.0.6.1/langchain_community/document_loaders/github.py
+-rw-r--r--   0        0        0     5096 2023-12-18 12:05:45.591407 gigachain_community-0.0.6.1/langchain_community/document_loaders/google_speech_to_text.py
+-rw-r--r--   0        0        0    14225 2023-12-18 12:05:45.592229 gigachain_community-0.0.6.1/langchain_community/document_loaders/googledrive.py
+-rw-r--r--   0        0        0      928 2023-12-18 12:05:45.592507 gigachain_community-0.0.6.1/langchain_community/document_loaders/gutenberg.py
+-rw-r--r--   0        0        0     1557 2023-12-18 12:05:45.592815 gigachain_community-0.0.6.1/langchain_community/document_loaders/helpers.py
+-rw-r--r--   0        0        0     2075 2023-12-18 12:05:45.593049 gigachain_community-0.0.6.1/langchain_community/document_loaders/hn.py
+-rw-r--r--   0        0        0     1158 2023-12-18 12:05:45.593334 gigachain_community-0.0.6.1/langchain_community/document_loaders/html.py
+-rw-r--r--   0        0        0     2045 2023-12-28 13:38:34.467659 gigachain_community-0.0.6.1/langchain_community/document_loaders/html_bs.py
+-rw-r--r--   0        0        0     3208 2023-12-18 12:05:45.594186 gigachain_community-0.0.6.1/langchain_community/document_loaders/hugging_face_dataset.py
+-rw-r--r--   0        0        0     7642 2023-12-18 12:05:45.594633 gigachain_community-0.0.6.1/langchain_community/document_loaders/ifixit.py
+-rw-r--r--   0        0        0     1173 2023-12-18 12:05:45.595279 gigachain_community-0.0.6.1/langchain_community/document_loaders/image.py
+-rw-r--r--   0        0        0     3594 2023-12-18 12:05:45.596852 gigachain_community-0.0.6.1/langchain_community/document_loaders/image_captions.py
+-rw-r--r--   0        0        0      477 2023-12-18 12:05:45.597367 gigachain_community-0.0.6.1/langchain_community/document_loaders/imsdb.py
+-rw-r--r--   0        0        0     1688 2023-12-18 12:05:45.597983 gigachain_community-0.0.6.1/langchain_community/document_loaders/iugu.py
+-rw-r--r--   0        0        0     3705 2023-12-18 12:05:45.598689 gigachain_community-0.0.6.1/langchain_community/document_loaders/joplin.py
+-rw-r--r--   0        0        0     5907 2023-12-18 12:05:45.599520 gigachain_community-0.0.6.1/langchain_community/document_loaders/json_loader.py
+-rw-r--r--   0        0        0     6058 2023-12-21 15:51:51.800637 gigachain_community-0.0.6.1/langchain_community/document_loaders/lakefs.py
+-rw-r--r--   0        0        0     2008 2023-12-18 12:05:45.600876 gigachain_community-0.0.6.1/langchain_community/document_loaders/larksuite.py
+-rw-r--r--   0        0        0     1818 2023-12-28 13:38:34.468309 gigachain_community-0.0.6.1/langchain_community/document_loaders/markdown.py
+-rw-r--r--   0        0        0     3112 2023-12-18 12:05:45.601726 gigachain_community-0.0.6.1/langchain_community/document_loaders/mastodon.py
+-rw-r--r--   0        0        0     3282 2023-12-18 12:05:45.602072 gigachain_community-0.0.6.1/langchain_community/document_loaders/max_compute.py
+-rw-r--r--   0        0        0     3455 2023-12-18 12:05:45.602561 gigachain_community-0.0.6.1/langchain_community/document_loaders/mediawikidump.py
+-rw-r--r--   0        0        0      846 2023-12-18 12:05:45.602927 gigachain_community-0.0.6.1/langchain_community/document_loaders/merge.py
+-rw-r--r--   0        0        0     2540 2023-12-28 13:38:34.469196 gigachain_community-0.0.6.1/langchain_community/document_loaders/mhtml.py
+-rw-r--r--   0        0        0     3074 2023-12-18 12:05:45.603564 gigachain_community-0.0.6.1/langchain_community/document_loaders/modern_treasury.py
+-rw-r--r--   0        0        0     2522 2023-12-18 12:05:45.604001 gigachain_community-0.0.6.1/langchain_community/document_loaders/mongodb.py
+-rw-r--r--   0        0        0     4296 2023-12-18 12:05:45.604511 gigachain_community-0.0.6.1/langchain_community/document_loaders/news.py
+-rw-r--r--   0        0        0     4301 2023-12-18 12:05:45.605118 gigachain_community-0.0.6.1/langchain_community/document_loaders/notebook.py
+-rw-r--r--   0        0        0      814 2023-12-18 12:05:45.605522 gigachain_community-0.0.6.1/langchain_community/document_loaders/notion.py
+-rw-r--r--   0        0        0     6718 2023-12-18 12:05:45.606331 gigachain_community-0.0.6.1/langchain_community/document_loaders/notiondb.py
+-rw-r--r--   0        0        0     1088 2023-12-18 12:05:45.606811 gigachain_community-0.0.6.1/langchain_community/document_loaders/nuclia.py
+-rw-r--r--   0        0        0     3593 2023-12-18 12:05:45.607288 gigachain_community-0.0.6.1/langchain_community/document_loaders/obs_directory.py
+-rw-r--r--   0        0        0     4768 2023-12-18 12:05:45.607862 gigachain_community-0.0.6.1/langchain_community/document_loaders/obs_file.py
+-rw-r--r--   0        0        0     6150 2023-12-18 12:05:45.608389 gigachain_community-0.0.6.1/langchain_community/document_loaders/obsidian.py
+-rw-r--r--   0        0        0     1770 2023-12-18 12:05:45.608973 gigachain_community-0.0.6.1/langchain_community/document_loaders/odt.py
+-rw-r--r--   0        0        0     3381 2023-12-18 12:05:45.609740 gigachain_community-0.0.6.1/langchain_community/document_loaders/onedrive.py
+-rw-r--r--   0        0        0     1154 2023-12-18 12:05:45.610167 gigachain_community-0.0.6.1/langchain_community/document_loaders/onedrive_file.py
+-rw-r--r--   0        0        0     8074 2023-12-18 12:05:45.610777 gigachain_community-0.0.6.1/langchain_community/document_loaders/onenote.py
+-rw-r--r--   0        0        0     1331 2023-12-18 12:05:45.611177 gigachain_community-0.0.6.1/langchain_community/document_loaders/open_city_data.py
+-rw-r--r--   0        0        0     1748 2023-12-18 12:05:45.611624 gigachain_community-0.0.6.1/langchain_community/document_loaders/org_mode.py
+-rw-r--r--   0        0        0      947 2023-12-28 13:38:34.470016 gigachain_community-0.0.6.1/langchain_community/document_loaders/parsers/__init__.py
+-rw-r--r--   0        0        0    10716 2023-12-18 12:05:45.612771 gigachain_community-0.0.6.1/langchain_community/document_loaders/parsers/audio.py
+-rw-r--r--   0        0        0     4534 2023-12-28 13:38:34.470440 gigachain_community-0.0.6.1/langchain_community/document_loaders/parsers/doc_intelligence.py
+-rw-r--r--   0        0        0    15283 2023-12-18 12:05:45.613557 gigachain_community-0.0.6.1/langchain_community/document_loaders/parsers/docai.py
+-rw-r--r--   0        0        0     2502 2023-12-18 12:05:45.614020 gigachain_community-0.0.6.1/langchain_community/document_loaders/parsers/generic.py
+-rw-r--r--   0        0        0     5767 2023-12-18 12:05:45.614963 gigachain_community-0.0.6.1/langchain_community/document_loaders/parsers/grobid.py
+-rw-r--r--   0        0        0      109 2023-12-18 12:05:45.615405 gigachain_community-0.0.6.1/langchain_community/document_loaders/parsers/html/__init__.py
+-rw-r--r--   0        0        0     1609 2023-12-18 12:05:45.615795 gigachain_community-0.0.6.1/langchain_community/document_loaders/parsers/html/bs4.py
+-rw-r--r--   0        0        0      136 2023-12-18 12:05:45.616382 gigachain_community-0.0.6.1/langchain_community/document_loaders/parsers/language/__init__.py
+-rw-r--r--   0        0        0     3745 2023-12-18 12:05:45.616807 gigachain_community-0.0.6.1/langchain_community/document_loaders/parsers/language/cobol.py
+-rw-r--r--   0        0        0      495 2023-12-18 12:05:45.617260 gigachain_community-0.0.6.1/langchain_community/document_loaders/parsers/language/code_segmenter.py
+-rw-r--r--   0        0        0     2103 2023-12-18 12:05:45.617642 gigachain_community-0.0.6.1/langchain_community/document_loaders/parsers/language/javascript.py
+-rw-r--r--   0        0        0     5114 2023-12-18 12:05:45.618562 gigachain_community-0.0.6.1/langchain_community/document_loaders/parsers/language/language_parser.py
+-rw-r--r--   0        0        0     1679 2023-12-18 12:05:45.618918 gigachain_community-0.0.6.1/langchain_community/document_loaders/parsers/language/python.py
+-rw-r--r--   0        0        0     1664 2023-12-18 12:05:45.619356 gigachain_community-0.0.6.1/langchain_community/document_loaders/parsers/msword.py
+-rw-r--r--   0        0        0    21006 2023-12-28 13:38:34.472391 gigachain_community-0.0.6.1/langchain_community/document_loaders/parsers/pdf.py
+-rw-r--r--   0        0        0     1214 2023-12-18 12:05:45.621291 gigachain_community-0.0.6.1/langchain_community/document_loaders/parsers/registry.py
+-rw-r--r--   0        0        0      505 2023-12-18 12:05:45.621708 gigachain_community-0.0.6.1/langchain_community/document_loaders/parsers/txt.py
+-rw-r--r--   0        0        0    26024 2023-12-18 12:05:45.622152 gigachain_community-0.0.6.1/langchain_community/document_loaders/pdf.py
+-rw-r--r--   0        0        0     1161 2023-12-18 12:05:45.622618 gigachain_community-0.0.6.1/langchain_community/document_loaders/polars_dataframe.py
+-rw-r--r--   0        0        0     2508 2023-12-18 12:05:45.623093 gigachain_community-0.0.6.1/langchain_community/document_loaders/powerpoint.py
+-rw-r--r--   0        0        0     1371 2023-12-18 12:05:45.623484 gigachain_community-0.0.6.1/langchain_community/document_loaders/psychic.py
+-rw-r--r--   0        0        0     1172 2023-12-18 12:05:45.623852 gigachain_community-0.0.6.1/langchain_community/document_loaders/pubmed.py
+-rw-r--r--   0        0        0     3388 2023-12-18 12:05:45.624242 gigachain_community-0.0.6.1/langchain_community/document_loaders/pyspark_dataframe.py
+-rw-r--r--   0        0        0      527 2023-12-18 12:05:45.624513 gigachain_community-0.0.6.1/langchain_community/document_loaders/python.py
+-rw-r--r--   0        0        0     8426 2023-12-18 12:05:45.624979 gigachain_community-0.0.6.1/langchain_community/document_loaders/quip.py
+-rw-r--r--   0        0        0     6928 2023-12-18 12:05:45.625504 gigachain_community-0.0.6.1/langchain_community/document_loaders/readthedocs.py
+-rw-r--r--   0        0        0    11591 2023-12-18 12:05:45.626220 gigachain_community-0.0.6.1/langchain_community/document_loaders/recursive_url_loader.py
+-rw-r--r--   0        0        0     4584 2023-12-18 12:05:45.626883 gigachain_community-0.0.6.1/langchain_community/document_loaders/reddit.py
+-rw-r--r--   0        0        0      705 2023-12-18 12:05:45.627281 gigachain_community-0.0.6.1/langchain_community/document_loaders/roam.py
+-rw-r--r--   0        0        0     4604 2023-12-18 12:05:45.627882 gigachain_community-0.0.6.1/langchain_community/document_loaders/rocksetdb.py
+-rw-r--r--   0        0        0     4936 2023-12-28 13:38:34.473933 gigachain_community-0.0.6.1/langchain_community/document_loaders/rspace.py
+-rw-r--r--   0        0        0     4895 2023-12-18 12:05:45.629065 gigachain_community-0.0.6.1/langchain_community/document_loaders/rss.py
+-rw-r--r--   0        0        0     1832 2023-12-18 12:05:45.629524 gigachain_community-0.0.6.1/langchain_community/document_loaders/rst.py
+-rw-r--r--   0        0        0     2061 2023-12-18 12:05:45.629875 gigachain_community-0.0.6.1/langchain_community/document_loaders/rtf.py
+-rw-r--r--   0        0        0     5759 2023-12-18 12:05:45.630757 gigachain_community-0.0.6.1/langchain_community/document_loaders/s3_directory.py
+-rw-r--r--   0        0        0     5412 2023-12-18 12:05:45.631317 gigachain_community-0.0.6.1/langchain_community/document_loaders/s3_file.py
+-rw-r--r--   0        0        0     2318 2023-12-18 12:05:45.631739 gigachain_community-0.0.6.1/langchain_community/document_loaders/sharepoint.py
+-rw-r--r--   0        0        0     8530 2023-12-18 12:05:45.632550 gigachain_community-0.0.6.1/langchain_community/document_loaders/sitemap.py
+-rw-r--r--   0        0        0     4131 2023-12-18 12:05:45.633088 gigachain_community-0.0.6.1/langchain_community/document_loaders/slack_directory.py
+-rw-r--r--   0        0        0     4799 2023-12-18 12:05:45.633700 gigachain_community-0.0.6.1/langchain_community/document_loaders/snowflake_loader.py
+-rw-r--r--   0        0        0     2004 2023-12-18 12:05:45.634087 gigachain_community-0.0.6.1/langchain_community/document_loaders/spreedly.py
+-rw-r--r--   0        0        0      851 2023-12-18 12:05:45.634481 gigachain_community-0.0.6.1/langchain_community/document_loaders/srt.py
+-rw-r--r--   0        0        0     1811 2023-12-18 12:05:45.634845 gigachain_community-0.0.6.1/langchain_community/document_loaders/stripe.py
+-rw-r--r--   0        0        0     9008 2023-12-18 12:05:45.635464 gigachain_community-0.0.6.1/langchain_community/document_loaders/telegram.py
+-rw-r--r--   0        0        0     1783 2023-12-18 12:05:45.635902 gigachain_community-0.0.6.1/langchain_community/document_loaders/tencent_cos_directory.py
+-rw-r--r--   0        0        0     1700 2023-12-28 13:38:34.474832 gigachain_community-0.0.6.1/langchain_community/document_loaders/tencent_cos_file.py
+-rw-r--r--   0        0        0     3024 2023-12-18 12:05:45.636604 gigachain_community-0.0.6.1/langchain_community/document_loaders/tensorflow_datasets.py
+-rw-r--r--   0        0        0     2010 2023-12-18 12:05:45.636912 gigachain_community-0.0.6.1/langchain_community/document_loaders/text.py
+-rw-r--r--   0        0        0      950 2023-12-18 12:05:45.637263 gigachain_community-0.0.6.1/langchain_community/document_loaders/tomarkdown.py
+-rw-r--r--   0        0        0     1572 2023-12-18 12:05:45.637651 gigachain_community-0.0.6.1/langchain_community/document_loaders/toml.py
+-rw-r--r--   0        0        0     6561 2023-12-18 12:05:45.638520 gigachain_community-0.0.6.1/langchain_community/document_loaders/trello.py
+-rw-r--r--   0        0        0     1293 2023-12-18 12:05:45.639113 gigachain_community-0.0.6.1/langchain_community/document_loaders/tsv.py
+-rw-r--r--   0        0        0     3438 2023-12-18 12:05:45.639710 gigachain_community-0.0.6.1/langchain_community/document_loaders/twitter.py
+-rw-r--r--   0        0        0    13793 2023-12-18 12:05:45.640484 gigachain_community-0.0.6.1/langchain_community/document_loaders/unstructured.py
+-rw-r--r--   0        0        0     6019 2023-12-18 12:05:45.641072 gigachain_community-0.0.6.1/langchain_community/document_loaders/url.py
+-rw-r--r--   0        0        0     7590 2023-12-18 12:05:45.641572 gigachain_community-0.0.6.1/langchain_community/document_loaders/url_playwright.py
+-rw-r--r--   0        0        0     6640 2023-12-18 12:05:45.642173 gigachain_community-0.0.6.1/langchain_community/document_loaders/url_selenium.py
+-rw-r--r--   0        0        0     1682 2023-12-18 12:05:45.642509 gigachain_community-0.0.6.1/langchain_community/document_loaders/weather.py
+-rw-r--r--   0        0        0    10164 2023-12-18 12:05:45.643373 gigachain_community-0.0.6.1/langchain_community/document_loaders/web_base.py
+-rw-r--r--   0        0        0     1770 2023-12-18 12:05:45.643807 gigachain_community-0.0.6.1/langchain_community/document_loaders/whatsapp_chat.py
+-rw-r--r--   0        0        0     2142 2023-12-18 12:05:45.644447 gigachain_community-0.0.6.1/langchain_community/document_loaders/wikipedia.py
+-rw-r--r--   0        0        0     4583 2023-12-18 12:05:45.645033 gigachain_community-0.0.6.1/langchain_community/document_loaders/word_document.py
+-rw-r--r--   0        0        0     1489 2023-12-18 12:05:45.645378 gigachain_community-0.0.6.1/langchain_community/document_loaders/xml.py
+-rw-r--r--   0        0        0     1119 2023-12-18 12:05:45.645826 gigachain_community-0.0.6.1/langchain_community/document_loaders/xorbits.py
+-rw-r--r--   0        0        0    14798 2023-12-18 12:05:45.647523 gigachain_community-0.0.6.1/langchain_community/document_loaders/youtube.py
+-rw-r--r--   0        0        0     1849 2023-12-18 12:05:45.647949 gigachain_community-0.0.6.1/langchain_community/document_transformers/__init__.py
+-rw-r--r--   0        0        0     5214 2023-12-21 15:51:51.802594 gigachain_community-0.0.6.1/langchain_community/document_transformers/beautiful_soup_transformer.py
+-rw-r--r--   0        0        0     3469 2023-12-18 12:05:45.648810 gigachain_community-0.0.6.1/langchain_community/document_transformers/doctran_text_extract.py
+-rw-r--r--   0        0        0     2193 2023-12-18 12:05:45.649227 gigachain_community-0.0.6.1/langchain_community/document_transformers/doctran_text_qa.py
+-rw-r--r--   0        0        0     2337 2023-12-18 12:05:45.649692 gigachain_community-0.0.6.1/langchain_community/document_transformers/doctran_text_translate.py
+-rw-r--r--   0        0        0     7882 2023-12-18 12:05:45.650106 gigachain_community-0.0.6.1/langchain_community/document_transformers/embeddings_redundant_filter.py
+-rw-r--r--   0        0        0     4133 2023-12-18 12:05:45.650606 gigachain_community-0.0.6.1/langchain_community/document_transformers/google_translate.py
+-rw-r--r--   0        0        0     1834 2023-12-18 12:05:45.650961 gigachain_community-0.0.6.1/langchain_community/document_transformers/html2text.py
+-rw-r--r--   0        0        0     1410 2023-12-18 12:05:45.653916 gigachain_community-0.0.6.1/langchain_community/document_transformers/long_context_reorder.py
+-rw-r--r--   0        0        0     1475 2023-12-18 12:05:45.654343 gigachain_community-0.0.6.1/langchain_community/document_transformers/nuclia_text_transform.py
+-rw-r--r--   0        0        0     6243 2023-12-18 12:05:45.655195 gigachain_community-0.0.6.1/langchain_community/document_transformers/openai_functions.py
+-rw-r--r--   0        0        0     6033 2023-12-18 12:05:45.656355 gigachain_community-0.0.6.1/langchain_community/document_transformers/xsl/html_chunks_with_headers.xslt
+-rw-r--r--   0        0        0     6534 2023-12-28 13:38:34.477982 gigachain_community-0.0.6.1/langchain_community/embeddings/__init__.py
+-rw-r--r--   0        0        0     9614 2023-12-18 12:05:45.657933 gigachain_community-0.0.6.1/langchain_community/embeddings/aleph_alpha.py
+-rw-r--r--   0        0        0     1865 2023-12-18 12:05:45.658580 gigachain_community-0.0.6.1/langchain_community/embeddings/awa.py
+-rw-r--r--   0        0        0     7063 2023-12-21 15:51:51.803470 gigachain_community-0.0.6.1/langchain_community/embeddings/azure_openai.py
+-rw-r--r--   0        0        0     4827 2023-12-21 15:51:51.804348 gigachain_community-0.0.6.1/langchain_community/embeddings/baidu_qianfan_endpoint.py
+-rw-r--r--   0        0        0     6723 2023-12-18 12:05:45.660498 gigachain_community-0.0.6.1/langchain_community/embeddings/bedrock.py
+-rw-r--r--   0        0        0     2725 2023-12-18 12:05:45.660858 gigachain_community-0.0.6.1/langchain_community/embeddings/bookend.py
+-rw-r--r--   0        0        0     5454 2023-12-18 12:05:45.661406 gigachain_community-0.0.6.1/langchain_community/embeddings/clarifai.py
+-rw-r--r--   0        0        0     2869 2023-12-18 12:05:45.661963 gigachain_community-0.0.6.1/langchain_community/embeddings/cloudflare_workersai.py
+-rw-r--r--   0        0        0     4660 2023-12-18 12:05:45.662561 gigachain_community-0.0.6.1/langchain_community/embeddings/cohere.py
+-rw-r--r--   0        0        0     4956 2023-12-18 12:05:45.663235 gigachain_community-0.0.6.1/langchain_community/embeddings/dashscope.py
+-rw-r--r--   0        0        0     1310 2023-12-18 12:05:45.663728 gigachain_community-0.0.6.1/langchain_community/embeddings/databricks.py
+-rw-r--r--   0        0        0     4426 2023-12-18 12:05:45.664376 gigachain_community-0.0.6.1/langchain_community/embeddings/deepinfra.py
+-rw-r--r--   0        0        0     3564 2023-12-21 15:51:51.805303 gigachain_community-0.0.6.1/langchain_community/embeddings/edenai.py
+-rw-r--r--   0        0        0     8401 2023-12-18 12:05:45.665414 gigachain_community-0.0.6.1/langchain_community/embeddings/elasticsearch.py
+-rw-r--r--   0        0        0     5418 2023-12-28 13:38:34.479313 gigachain_community-0.0.6.1/langchain_community/embeddings/embaas.py
+-rw-r--r--   0        0        0     4859 2023-12-18 12:05:45.667020 gigachain_community-0.0.6.1/langchain_community/embeddings/ernie.py
+-rw-r--r--   0        0        0     1512 2023-12-18 12:05:45.667503 gigachain_community-0.0.6.1/langchain_community/embeddings/fake.py
+-rw-r--r--   0        0        0     3452 2023-12-18 12:05:45.667862 gigachain_community-0.0.6.1/langchain_community/embeddings/fastembed.py
+-rw-r--r--   0        0        0     4932 2024-01-09 11:56:52.846703 gigachain_community-0.0.6.1/langchain_community/embeddings/gigachat.py
+-rw-r--r--   0        0        0     3272 2023-12-18 12:05:45.668242 gigachain_community-0.0.6.1/langchain_community/embeddings/google_palm.py
+-rw-r--r--   0        0        0     1664 2023-12-18 12:05:45.669050 gigachain_community-0.0.6.1/langchain_community/embeddings/gpt4all.py
+-rw-r--r--   0        0        0     5274 2023-12-21 15:51:51.806243 gigachain_community-0.0.6.1/langchain_community/embeddings/gradient_ai.py
+-rw-r--r--   0        0        0    11898 2023-12-18 12:05:45.670340 gigachain_community-0.0.6.1/langchain_community/embeddings/huggingface.py
+-rw-r--r--   0        0        0     3789 2023-12-18 12:05:45.670872 gigachain_community-0.0.6.1/langchain_community/embeddings/huggingface_hub.py
+-rw-r--r--   0        0        0    10260 2023-12-18 12:05:45.671375 gigachain_community-0.0.6.1/langchain_community/embeddings/infinity.py
+-rw-r--r--   0        0        0     3673 2023-12-18 12:05:45.671824 gigachain_community-0.0.6.1/langchain_community/embeddings/javelin_ai_gateway.py
+-rw-r--r--   0        0        0     2607 2023-12-28 13:38:34.482924 gigachain_community-0.0.6.1/langchain_community/embeddings/jina.py
+-rw-r--r--   0        0        0     2873 2023-12-18 12:05:45.672526 gigachain_community-0.0.6.1/langchain_community/embeddings/johnsnowlabs.py
+-rw-r--r--   0        0        0     4163 2023-12-18 12:05:45.673477 gigachain_community-0.0.6.1/langchain_community/embeddings/llamacpp.py
+-rw-r--r--   0        0        0     2096 2023-12-18 12:05:45.673924 gigachain_community-0.0.6.1/langchain_community/embeddings/llm_rails.py
+-rw-r--r--   0        0        0    12261 2023-12-27 10:44:25.850461 gigachain_community-0.0.6.1/langchain_community/embeddings/localai.py
+-rw-r--r--   0        0        0     4798 2023-12-28 13:38:34.484154 gigachain_community-0.0.6.1/langchain_community/embeddings/minimax.py
+-rw-r--r--   0        0        0     2417 2023-12-18 12:05:45.675851 gigachain_community-0.0.6.1/langchain_community/embeddings/mlflow.py
+-rw-r--r--   0        0        0     2479 2023-12-18 12:05:45.676322 gigachain_community-0.0.6.1/langchain_community/embeddings/mlflow_gateway.py
+-rw-r--r--   0        0        0     2384 2023-12-18 12:05:45.678107 gigachain_community-0.0.6.1/langchain_community/embeddings/modelscope_hub.py
+-rw-r--r--   0        0        0     5115 2023-12-18 12:05:45.678704 gigachain_community-0.0.6.1/langchain_community/embeddings/mosaicml.py
+-rw-r--r--   0        0        0     2203 2023-12-18 12:05:45.679072 gigachain_community-0.0.6.1/langchain_community/embeddings/nlpcloud.py
+-rw-r--r--   0        0        0     3420 2023-12-18 12:05:45.679432 gigachain_community-0.0.6.1/langchain_community/embeddings/octoai_embeddings.py
+-rw-r--r--   0        0        0     7691 2023-12-18 12:05:45.680736 gigachain_community-0.0.6.1/langchain_community/embeddings/ollama.py
+-rw-r--r--   0        0        0    29207 2023-12-18 12:05:45.681405 gigachain_community-0.0.6.1/langchain_community/embeddings/openai.py
+-rw-r--r--   0        0        0     7591 2023-12-18 12:05:45.682567 gigachain_community-0.0.6.1/langchain_community/embeddings/sagemaker_endpoint.py
+-rw-r--r--   0        0        0     3807 2023-12-18 12:05:45.683325 gigachain_community-0.0.6.1/langchain_community/embeddings/self_hosted.py
+-rw-r--r--   0        0        0     6589 2023-12-18 12:05:45.684011 gigachain_community-0.0.6.1/langchain_community/embeddings/self_hosted_hugging_face.py
+-rw-r--r--   0        0        0      189 2023-12-18 12:05:45.684427 gigachain_community-0.0.6.1/langchain_community/embeddings/sentence_transformer.py
+-rw-r--r--   0        0        0     3743 2023-12-18 12:05:45.684825 gigachain_community-0.0.6.1/langchain_community/embeddings/spacy_embeddings.py
+-rw-r--r--   0        0        0     2413 2023-12-18 12:05:45.685136 gigachain_community-0.0.6.1/langchain_community/embeddings/tensorflow_hub.py
+-rw-r--r--   0        0        0    13929 2023-12-28 13:38:34.485210 gigachain_community-0.0.6.1/langchain_community/embeddings/vertexai.py
+-rw-r--r--   0        0        0     6255 2023-12-18 12:05:45.687621 gigachain_community-0.0.6.1/langchain_community/embeddings/voyageai.py
+-rw-r--r--   0        0        0     3303 2023-12-18 12:05:45.688334 gigachain_community-0.0.6.1/langchain_community/embeddings/xinference.py
+-rw-r--r--   0        0        0     5934 2023-12-21 15:51:51.807967 gigachain_community-0.0.6.1/langchain_community/embeddings/yandex.py
+-rw-r--r--   0        0        0      930 2023-12-18 12:05:45.688723 gigachain_community-0.0.6.1/langchain_community/graphs/__init__.py
+-rw-r--r--   0        0        0     6961 2023-12-18 12:05:45.689581 gigachain_community-0.0.6.1/langchain_community/graphs/arangodb_graph.py
+-rw-r--r--   0        0        0     5294 2023-12-18 12:05:45.690457 gigachain_community-0.0.6.1/langchain_community/graphs/falkordb_graph.py
+-rw-r--r--   0        0        0     1584 2023-12-18 12:05:45.690984 gigachain_community-0.0.6.1/langchain_community/graphs/graph_document.py
+-rw-r--r--   0        0        0     1008 2023-12-18 12:05:45.691396 gigachain_community-0.0.6.1/langchain_community/graphs/graph_store.py
+-rw-r--r--   0        0        0     2510 2023-12-18 12:05:45.691835 gigachain_community-0.0.6.1/langchain_community/graphs/hugegraph.py
+-rw-r--r--   0        0        0     4227 2023-12-18 12:05:45.692460 gigachain_community-0.0.6.1/langchain_community/graphs/kuzu_graph.py
+-rw-r--r--   0        0        0     1644 2023-12-18 12:05:45.692879 gigachain_community-0.0.6.1/langchain_community/graphs/memgraph_graph.py
+-rw-r--r--   0        0        0     8112 2023-12-18 12:05:45.693526 gigachain_community-0.0.6.1/langchain_community/graphs/nebula_graph.py
+-rw-r--r--   0        0        0     8388 2023-12-18 12:05:45.693954 gigachain_community-0.0.6.1/langchain_community/graphs/neo4j_graph.py
+-rw-r--r--   0        0        0     9398 2023-12-18 12:05:45.694545 gigachain_community-0.0.6.1/langchain_community/graphs/neptune_graph.py
+-rw-r--r--   0        0        0     6545 2023-12-18 12:05:45.695142 gigachain_community-0.0.6.1/langchain_community/graphs/networkx_graph.py
+-rw-r--r--   0        0        0    10118 2023-12-18 12:05:45.695554 gigachain_community-0.0.6.1/langchain_community/graphs/rdf_graph.py
+-rw-r--r--   0        0        0        0 2023-12-18 12:05:45.695817 gigachain_community-0.0.6.1/langchain_community/indexes/__init__.py
+-rw-r--r--   0        0        0    20960 2023-12-18 12:05:45.696278 gigachain_community-0.0.6.1/langchain_community/indexes/_sql_record_manager.py
+-rw-r--r--   0        0        0     5221 2023-12-18 12:05:45.696935 gigachain_community-0.0.6.1/langchain_community/indexes/base.py
+-rw-r--r--   0        0        0    23006 2023-12-28 13:38:34.486291 gigachain_community-0.0.6.1/langchain_community/llms/__init__.py
+-rw-r--r--   0        0        0     5292 2023-12-18 12:05:45.698661 gigachain_community-0.0.6.1/langchain_community/llms/ai21.py
+-rw-r--r--   0        0        0    11493 2023-12-18 12:05:45.699215 gigachain_community-0.0.6.1/langchain_community/llms/aleph_alpha.py
+-rw-r--r--   0        0        0     3061 2023-12-18 12:05:45.699586 gigachain_community-0.0.6.1/langchain_community/llms/amazon_api_gateway.py
+-rw-r--r--   0        0        0    12356 2023-12-18 12:05:45.700279 gigachain_community-0.0.6.1/langchain_community/llms/anthropic.py
+-rw-r--r--   0        0        0    10630 2023-12-18 12:05:45.700779 gigachain_community-0.0.6.1/langchain_community/llms/anyscale.py
+-rw-r--r--   0        0        0     9619 2023-12-21 15:51:51.809621 gigachain_community-0.0.6.1/langchain_community/llms/aphrodite.py
+-rw-r--r--   0        0        0     4356 2023-12-18 12:05:45.701385 gigachain_community-0.0.6.1/langchain_community/llms/arcee.py
+-rw-r--r--   0        0        0     6007 2023-12-18 12:05:45.701968 gigachain_community-0.0.6.1/langchain_community/llms/aviary.py
+-rw-r--r--   0        0        0    10251 2023-12-18 12:05:45.702392 gigachain_community-0.0.6.1/langchain_community/llms/azureml_endpoint.py
+-rw-r--r--   0        0        0     7293 2023-12-21 15:51:51.810589 gigachain_community-0.0.6.1/langchain_community/llms/baidu_qianfan_endpoint.py
+-rw-r--r--   0        0        0     4725 2023-12-18 12:05:45.703913 gigachain_community-0.0.6.1/langchain_community/llms/bananadev.py
+-rw-r--r--   0        0        0     3187 2023-12-28 13:38:34.487169 gigachain_community-0.0.6.1/langchain_community/llms/baseten.py
+-rw-r--r--   0        0        0     9099 2023-12-18 12:05:45.705119 gigachain_community-0.0.6.1/langchain_community/llms/beam.py
+-rw-r--r--   0        0        0    15469 2023-12-28 13:38:34.488257 gigachain_community-0.0.6.1/langchain_community/llms/bedrock.py
+-rw-r--r--   0        0        0     6232 2023-12-18 12:05:45.707024 gigachain_community-0.0.6.1/langchain_community/llms/bittensor.py
+-rw-r--r--   0        0        0     4044 2023-12-18 12:05:45.707481 gigachain_community-0.0.6.1/langchain_community/llms/cerebriumai.py
+-rw-r--r--   0        0        0     3969 2023-12-18 12:05:45.707879 gigachain_community-0.0.6.1/langchain_community/llms/chatglm.py
+-rw-r--r--   0        0        0     7262 2023-12-18 12:05:45.708779 gigachain_community-0.0.6.1/langchain_community/llms/clarifai.py
+-rw-r--r--   0        0        0     4277 2023-12-18 12:05:45.709389 gigachain_community-0.0.6.1/langchain_community/llms/cloudflare_workersai.py
+-rw-r--r--   0        0        0     7970 2023-12-18 12:05:45.710013 gigachain_community-0.0.6.1/langchain_community/llms/cohere.py
+-rw-r--r--   0        0        0     4227 2023-12-18 12:05:45.711016 gigachain_community-0.0.6.1/langchain_community/llms/ctransformers.py
+-rw-r--r--   0        0        0     4135 2023-12-18 12:05:45.712038 gigachain_community-0.0.6.1/langchain_community/llms/ctranslate2.py
+-rw-r--r--   0        0        0    17597 2023-12-28 13:38:34.489750 gigachain_community-0.0.6.1/langchain_community/llms/databricks.py
+-rw-r--r--   0        0        0     7006 2023-12-18 12:05:45.713379 gigachain_community-0.0.6.1/langchain_community/llms/deepinfra.py
+-rw-r--r--   0        0        0     8615 2023-12-28 13:38:34.491881 gigachain_community-0.0.6.1/langchain_community/llms/deepsparse.py
+-rw-r--r--   0        0        0     9463 2023-12-21 15:51:51.811774 gigachain_community-0.0.6.1/langchain_community/llms/edenai.py
+-rw-r--r--   0        0        0     2444 2023-12-18 12:05:45.714846 gigachain_community-0.0.6.1/langchain_community/llms/fake.py
+-rw-r--r--   0        0        0    11773 2023-12-21 15:51:51.813007 gigachain_community-0.0.6.1/langchain_community/llms/fireworks.py
+-rw-r--r--   0        0        0     3762 2023-12-18 12:05:45.715821 gigachain_community-0.0.6.1/langchain_community/llms/forefrontai.py
+-rw-r--r--   0        0        0    10505 2023-12-28 13:38:34.495098 gigachain_community-0.0.6.1/langchain_community/llms/gigachat.py
+-rw-r--r--   0        0        0     8854 2023-12-21 15:51:51.816031 gigachain_community-0.0.6.1/langchain_community/llms/google_palm.py
+-rw-r--r--   0        0        0     5301 2023-12-18 12:05:45.718164 gigachain_community-0.0.6.1/langchain_community/llms/gooseai.py
+-rw-r--r--   0        0        0     6525 2023-12-18 12:05:45.718855 gigachain_community-0.0.6.1/langchain_community/llms/gpt4all.py
+-rw-r--r--   0        0        0    14199 2023-12-18 12:05:45.719653 gigachain_community-0.0.6.1/langchain_community/llms/gradient_ai.py
+-rw-r--r--   0        0        0      664 2023-12-18 12:05:45.720222 gigachain_community-0.0.6.1/langchain_community/llms/grammars/json.gbnf
+-rw-r--r--   0        0        0      167 2023-12-18 12:05:45.720572 gigachain_community-0.0.6.1/langchain_community/llms/grammars/list.gbnf
+-rw-r--r--   0        0        0     5508 2023-12-18 12:05:45.721443 gigachain_community-0.0.6.1/langchain_community/llms/huggingface_endpoint.py
+-rw-r--r--   0        0        0     4658 2023-12-18 12:05:45.721873 gigachain_community-0.0.6.1/langchain_community/llms/huggingface_hub.py
+-rw-r--r--   0        0        0     9215 2023-12-18 12:05:45.722687 gigachain_community-0.0.6.1/langchain_community/llms/huggingface_pipeline.py
+-rw-r--r--   0        0        0    11403 2023-12-18 12:05:45.723462 gigachain_community-0.0.6.1/langchain_community/llms/huggingface_text_gen_inference.py
+-rw-r--r--   0        0        0     2582 2023-12-18 12:05:45.723857 gigachain_community-0.0.6.1/langchain_community/llms/human.py
+-rw-r--r--   0        0        0     4723 2023-12-18 12:05:45.724545 gigachain_community-0.0.6.1/langchain_community/llms/javelin_ai_gateway.py
+-rw-r--r--   0        0        0     5087 2023-12-18 12:05:45.724912 gigachain_community-0.0.6.1/langchain_community/llms/koboldai.py
+-rw-r--r--   0        0        0    12537 2023-12-18 12:05:45.725808 gigachain_community-0.0.6.1/langchain_community/llms/llamacpp.py
+-rw-r--r--   0        0        0     1328 2023-12-18 12:05:45.726192 gigachain_community-0.0.6.1/langchain_community/llms/loading.py
+-rw-r--r--   0        0        0     1965 2023-12-18 12:05:45.726579 gigachain_community-0.0.6.1/langchain_community/llms/manifest.py
+-rw-r--r--   0        0        0     5470 2023-12-18 12:05:45.727040 gigachain_community-0.0.6.1/langchain_community/llms/minimax.py
+-rw-r--r--   0        0        0     3845 2023-12-18 12:05:45.727455 gigachain_community-0.0.6.1/langchain_community/llms/mlflow.py
+-rw-r--r--   0        0        0     3279 2023-12-18 12:05:45.728237 gigachain_community-0.0.6.1/langchain_community/llms/mlflow_ai_gateway.py
+-rw-r--r--   0        0        0     3288 2023-12-18 12:05:45.730018 gigachain_community-0.0.6.1/langchain_community/llms/modal.py
+-rw-r--r--   0        0        0     6150 2023-12-18 12:05:45.730902 gigachain_community-0.0.6.1/langchain_community/llms/mosaicml.py
+-rw-r--r--   0        0        0     5049 2023-12-18 12:05:45.731352 gigachain_community-0.0.6.1/langchain_community/llms/nlpcloud.py
+-rw-r--r--   0        0        0    12162 2023-12-28 13:38:34.495799 gigachain_community-0.0.6.1/langchain_community/llms/oci_data_science_model_deployment_endpoint.py
+-rw-r--r--   0        0        0     5207 2023-12-18 12:05:45.731708 gigachain_community-0.0.6.1/langchain_community/llms/octoai_endpoint.py
+-rw-r--r--   0        0        0    16092 2023-12-28 13:38:34.496966 gigachain_community-0.0.6.1/langchain_community/llms/ollama.py
+-rw-r--r--   0        0        0     3980 2023-12-18 12:05:45.732462 gigachain_community-0.0.6.1/langchain_community/llms/opaqueprompts.py
+-rw-r--r--   0        0        0    47378 2023-12-21 15:51:51.818449 gigachain_community-0.0.6.1/langchain_community/llms/openai.py
+-rw-r--r--   0        0        0    10743 2023-12-18 12:05:45.733474 gigachain_community-0.0.6.1/langchain_community/llms/openllm.py
+-rw-r--r--   0        0        0      902 2023-12-18 12:05:45.733910 gigachain_community-0.0.6.1/langchain_community/llms/openlm.py
+-rw-r--r--   0        0        0     8059 2023-12-18 12:05:45.734279 gigachain_community-0.0.6.1/langchain_community/llms/pai_eas_endpoint.py
+-rw-r--r--   0        0        0     5402 2023-12-28 13:38:34.498208 gigachain_community-0.0.6.1/langchain_community/llms/petals.py
+-rw-r--r--   0        0        0     4182 2023-12-28 13:38:34.499044 gigachain_community-0.0.6.1/langchain_community/llms/pipelineai.py
+-rw-r--r--   0        0        0     1594 2023-12-28 13:38:34.499702 gigachain_community-0.0.6.1/langchain_community/llms/predibase.py
+-rw-r--r--   0        0        0     4410 2023-12-18 12:05:45.735769 gigachain_community-0.0.6.1/langchain_community/llms/predictionguard.py
+-rw-r--r--   0        0        0     8809 2023-12-21 15:51:51.819566 gigachain_community-0.0.6.1/langchain_community/llms/promptlayer_openai.py
+-rw-r--r--   0        0        0     8024 2023-12-18 12:05:45.736765 gigachain_community-0.0.6.1/langchain_community/llms/replicate.py
+-rw-r--r--   0        0        0     7387 2023-12-18 12:05:45.737203 gigachain_community-0.0.6.1/langchain_community/llms/rwkv.py
+-rw-r--r--   0        0        0    13193 2023-12-18 12:05:45.737817 gigachain_community-0.0.6.1/langchain_community/llms/sagemaker_endpoint.py
+-rw-r--r--   0        0        0     7743 2023-12-18 12:05:45.738142 gigachain_community-0.0.6.1/langchain_community/llms/self_hosted.py
+-rw-r--r--   0        0        0     7743 2023-12-18 12:05:45.738949 gigachain_community-0.0.6.1/langchain_community/llms/self_hosted_hugging_face.py
+-rw-r--r--   0        0        0     4720 2023-12-28 13:38:34.500543 gigachain_community-0.0.6.1/langchain_community/llms/stochasticai.py
+-rw-r--r--   0        0        0     7552 2023-12-18 12:05:45.739825 gigachain_community-0.0.6.1/langchain_community/llms/symblai_nebula.py
+-rw-r--r--   0        0        0    14081 2023-12-21 15:51:51.820638 gigachain_community-0.0.6.1/langchain_community/llms/textgen.py
+-rw-r--r--   0        0        0     5243 2023-12-18 12:05:45.740891 gigachain_community-0.0.6.1/langchain_community/llms/titan_takeoff.py
+-rw-r--r--   0        0        0     7349 2023-12-21 15:51:51.821440 gigachain_community-0.0.6.1/langchain_community/llms/titan_takeoff_pro.py
+-rw-r--r--   0        0        0     7526 2023-12-21 15:51:51.822232 gigachain_community-0.0.6.1/langchain_community/llms/together.py
+-rw-r--r--   0        0        0     9593 2023-12-21 15:51:51.823228 gigachain_community-0.0.6.1/langchain_community/llms/tongyi.py
+-rw-r--r--   0        0        0      258 2023-12-18 12:05:45.742413 gigachain_community-0.0.6.1/langchain_community/llms/utils.py
+-rw-r--r--   0        0        0    18948 2023-12-21 15:51:51.824271 gigachain_community-0.0.6.1/langchain_community/llms/vertexai.py
+-rw-r--r--   0        0        0     5592 2023-12-18 12:05:45.743737 gigachain_community-0.0.6.1/langchain_community/llms/vllm.py
+-rw-r--r--   0        0        0     6591 2023-12-28 13:38:34.501403 gigachain_community-0.0.6.1/langchain_community/llms/volcengine_maas.py
+-rw-r--r--   0        0        0    13164 2023-12-18 12:05:45.744770 gigachain_community-0.0.6.1/langchain_community/llms/watsonxllm.py
+-rw-r--r--   0        0        0     4970 2023-12-18 12:05:45.745301 gigachain_community-0.0.6.1/langchain_community/llms/writer.py
+-rw-r--r--   0        0        0     6325 2023-12-21 15:51:51.825366 gigachain_community-0.0.6.1/langchain_community/llms/xinference.py
+-rw-r--r--   0        0        0    10797 2023-12-21 15:51:51.826293 gigachain_community-0.0.6.1/langchain_community/llms/yandex.py
+-rw-r--r--   0        0        0        0 2023-12-18 12:05:45.746445 gigachain_community-0.0.6.1/langchain_community/py.typed
+-rw-r--r--   0        0        0     4245 2023-12-21 15:51:51.827178 gigachain_community-0.0.6.1/langchain_community/retrievers/__init__.py
+-rw-r--r--   0        0        0     4328 2023-12-18 12:05:45.747540 gigachain_community-0.0.6.1/langchain_community/retrievers/arcee.py
+-rw-r--r--   0        0        0      773 2023-12-18 12:05:45.747949 gigachain_community-0.0.6.1/langchain_community/retrievers/arxiv.py
+-rw-r--r--   0        0        0     4279 2023-12-18 12:05:45.748397 gigachain_community-0.0.6.1/langchain_community/retrievers/azure_cognitive_search.py
+-rw-r--r--   0        0        0     4691 2023-12-21 15:51:51.828732 gigachain_community-0.0.6.1/langchain_community/retrievers/bedrock.py
+-rw-r--r--   0        0        0     3648 2023-12-18 12:05:45.749291 gigachain_community-0.0.6.1/langchain_community/retrievers/bm25.py
+-rw-r--r--   0        0        0     2684 2023-12-18 12:05:45.749632 gigachain_community-0.0.6.1/langchain_community/retrievers/chaindesk.py
+-rw-r--r--   0        0        0     3024 2023-12-18 12:05:45.749873 gigachain_community-0.0.6.1/langchain_community/retrievers/chatgpt_plugin_retriever.py
+-rw-r--r--   0        0        0     2816 2023-12-18 12:05:45.750128 gigachain_community-0.0.6.1/langchain_community/retrievers/cohere_rag_retriever.py
+-rw-r--r--   0        0        0     2338 2023-12-18 12:05:45.750555 gigachain_community-0.0.6.1/langchain_community/retrievers/databerry.py
+-rw-r--r--   0        0        0     6778 2023-12-18 12:05:45.751130 gigachain_community-0.0.6.1/langchain_community/retrievers/docarray.py
+-rw-r--r--   0        0        0     4639 2023-12-18 12:05:45.751921 gigachain_community-0.0.6.1/langchain_community/retrievers/elastic_search_bm25.py
+-rw-r--r--   0        0        0     2000 2023-12-18 12:05:45.752650 gigachain_community-0.0.6.1/langchain_community/retrievers/embedchain.py
+-rw-r--r--   0        0        0     4583 2023-12-18 12:05:45.753268 gigachain_community-0.0.6.1/langchain_community/retrievers/google_cloud_documentai_warehouse.py
+-rw-r--r--   0        0        0    17552 2023-12-28 13:38:34.502238 gigachain_community-0.0.6.1/langchain_community/retrievers/google_vertex_ai_search.py
+-rw-r--r--   0        0        0     1985 2023-12-18 12:05:45.754528 gigachain_community-0.0.6.1/langchain_community/retrievers/kay.py
+-rw-r--r--   0        0        0    13811 2023-12-21 15:51:51.830140 gigachain_community-0.0.6.1/langchain_community/retrievers/kendra.py
+-rw-r--r--   0        0        0     2570 2023-12-18 12:05:45.756151 gigachain_community-0.0.6.1/langchain_community/retrievers/knn.py
+-rw-r--r--   0        0        0     3162 2023-12-18 12:05:45.756542 gigachain_community-0.0.6.1/langchain_community/retrievers/llama_index.py
+-rw-r--r--   0        0        0     1486 2023-12-18 12:05:45.756990 gigachain_community-0.0.6.1/langchain_community/retrievers/metal.py
+-rw-r--r--   0        0        0     2435 2023-12-18 12:05:45.757360 gigachain_community-0.0.6.1/langchain_community/retrievers/milvus.py
+-rw-r--r--   0        0        0      644 2023-12-18 12:05:45.757713 gigachain_community-0.0.6.1/langchain_community/retrievers/outline.py
+-rw-r--r--   0        0        0     5733 2023-12-18 12:05:45.758713 gigachain_community-0.0.6.1/langchain_community/retrievers/pinecone_hybrid_search.py
+-rw-r--r--   0        0        0      643 2023-12-18 12:05:45.759084 gigachain_community-0.0.6.1/langchain_community/retrievers/pubmed.py
+-rw-r--r--   0        0        0      104 2023-12-18 12:05:45.759462 gigachain_community-0.0.6.1/langchain_community/retrievers/pupmed.py
+-rw-r--r--   0        0        0     7468 2023-12-21 15:51:51.831006 gigachain_community-0.0.6.1/langchain_community/retrievers/qdrant_sparse_vector_retriever.py
+-rw-r--r--   0        0        0     1935 2023-12-18 12:05:45.759849 gigachain_community-0.0.6.1/langchain_community/retrievers/remote_retriever.py
+-rw-r--r--   0        0        0     4131 2023-12-18 12:05:45.760244 gigachain_community-0.0.6.1/langchain_community/retrievers/svm.py
+-rw-r--r--   0        0        0     2855 2023-12-18 12:05:45.760593 gigachain_community-0.0.6.1/langchain_community/retrievers/tavily_search_api.py
+-rw-r--r--   0        0        0     4079 2023-12-18 12:05:45.760932 gigachain_community-0.0.6.1/langchain_community/retrievers/tfidf.py
+-rw-r--r--   0        0        0     4555 2023-12-18 12:05:45.761391 gigachain_community-0.0.6.1/langchain_community/retrievers/vespa_retriever.py
+-rw-r--r--   0        0        0     6195 2023-12-18 12:05:45.762141 gigachain_community-0.0.6.1/langchain_community/retrievers/weaviate_hybrid_search.py
+-rw-r--r--   0        0        0      656 2023-12-18 12:05:45.762889 gigachain_community-0.0.6.1/langchain_community/retrievers/wikipedia.py
+-rw-r--r--   0        0        0     2356 2023-12-18 12:05:45.763365 gigachain_community-0.0.6.1/langchain_community/retrievers/you.py
+-rw-r--r--   0        0        0     5904 2023-12-18 12:05:45.763882 gigachain_community-0.0.6.1/langchain_community/retrievers/zep.py
+-rw-r--r--   0        0        0     2735 2023-12-18 12:05:45.764315 gigachain_community-0.0.6.1/langchain_community/retrievers/zilliz.py
+-rw-r--r--   0        0        0      501 2023-12-18 12:05:45.764791 gigachain_community-0.0.6.1/langchain_community/storage/__init__.py
+-rw-r--r--   0        0        0      179 2023-12-18 12:05:45.765177 gigachain_community-0.0.6.1/langchain_community/storage/exceptions.py
+-rw-r--r--   0        0        0     4788 2023-12-18 12:05:45.765839 gigachain_community-0.0.6.1/langchain_community/storage/redis.py
+-rw-r--r--   0        0        0     5764 2023-12-18 12:05:45.766664 gigachain_community-0.0.6.1/langchain_community/storage/upstash_redis.py
+-rw-r--r--   0        0        0    33514 2023-12-18 12:05:45.767310 gigachain_community-0.0.6.1/langchain_community/tools/__init__.py
+-rw-r--r--   0        0        0     3185 2023-12-18 12:05:45.767799 gigachain_community-0.0.6.1/langchain_community/tools/ainetwork/app.py
+-rw-r--r--   0        0        0     2109 2023-12-18 12:05:45.768158 gigachain_community-0.0.6.1/langchain_community/tools/ainetwork/base.py
+-rw-r--r--   0        0        0     4140 2023-12-18 12:05:45.768950 gigachain_community-0.0.6.1/langchain_community/tools/ainetwork/owner.py
+-rw-r--r--   0        0        0     2746 2023-12-18 12:05:45.769433 gigachain_community-0.0.6.1/langchain_community/tools/ainetwork/rule.py
+-rw-r--r--   0        0        0     1074 2023-12-18 12:05:45.769853 gigachain_community-0.0.6.1/langchain_community/tools/ainetwork/transfer.py
+-rw-r--r--   0        0        0     2314 2023-12-18 12:05:45.770226 gigachain_community-0.0.6.1/langchain_community/tools/ainetwork/utils.py
+-rw-r--r--   0        0        0     2624 2023-12-18 12:05:45.770601 gigachain_community-0.0.6.1/langchain_community/tools/ainetwork/value.py
+-rw-r--r--   0        0        0      257 2023-12-18 12:05:45.770978 gigachain_community-0.0.6.1/langchain_community/tools/amadeus/__init__.py
+-rw-r--r--   0        0        0      435 2023-12-18 12:05:45.771420 gigachain_community-0.0.6.1/langchain_community/tools/amadeus/base.py
+-rw-r--r--   0        0        0     1845 2023-12-18 12:05:45.771860 gigachain_community-0.0.6.1/langchain_community/tools/amadeus/closest_airport.py
+-rw-r--r--   0        0        0     5611 2023-12-18 12:05:45.772295 gigachain_community-0.0.6.1/langchain_community/tools/amadeus/flight_search.py
+-rw-r--r--   0        0        0     1276 2023-12-18 12:05:45.773346 gigachain_community-0.0.6.1/langchain_community/tools/amadeus/utils.py
+-rw-r--r--   0        0        0       25 2023-12-18 12:05:45.773797 gigachain_community-0.0.6.1/langchain_community/tools/arxiv/__init__.py
+-rw-r--r--   0        0        0     1228 2023-12-21 15:51:51.832262 gigachain_community-0.0.6.1/langchain_community/tools/arxiv/tool.py
+-rw-r--r--   0        0        0      802 2023-12-18 12:05:45.774697 gigachain_community-0.0.6.1/langchain_community/tools/azure_cognitive_services/__init__.py
+-rw-r--r--   0        0        0     5375 2023-12-18 12:05:45.775110 gigachain_community-0.0.6.1/langchain_community/tools/azure_cognitive_services/form_recognizer.py
+-rw-r--r--   0        0        0     5304 2023-12-18 12:05:45.775653 gigachain_community-0.0.6.1/langchain_community/tools/azure_cognitive_services/image_analysis.py
+-rw-r--r--   0        0        0     4336 2023-12-18 12:05:45.776161 gigachain_community-0.0.6.1/langchain_community/tools/azure_cognitive_services/speech2text.py
+-rw-r--r--   0        0        0     3675 2023-12-18 12:05:45.776545 gigachain_community-0.0.6.1/langchain_community/tools/azure_cognitive_services/text2speech.py
+-rw-r--r--   0        0        0     3542 2023-12-21 15:51:51.833253 gigachain_community-0.0.6.1/langchain_community/tools/azure_cognitive_services/text_analytics_health.py
+-rw-r--r--   0        0        0      776 2023-12-18 12:05:45.777398 gigachain_community-0.0.6.1/langchain_community/tools/azure_cognitive_services/utils.py
+-rw-r--r--   0        0        0        0 2023-12-18 12:05:45.777639 gigachain_community-0.0.6.1/langchain_community/tools/bearly/__init__.py
+-rw-r--r--   0        0        0     5468 2023-12-18 12:05:45.777984 gigachain_community-0.0.6.1/langchain_community/tools/bearly/tool.py
+-rw-r--r--   0        0        0      170 2023-12-18 12:05:45.778478 gigachain_community-0.0.6.1/langchain_community/tools/bing_search/__init__.py
+-rw-r--r--   0        0        0     1463 2023-12-18 12:05:45.779631 gigachain_community-0.0.6.1/langchain_community/tools/bing_search/tool.py
+-rw-r--r--   0        0        0        0 2023-12-18 12:05:45.780012 gigachain_community-0.0.6.1/langchain_community/tools/brave_search/__init__.py
+-rw-r--r--   0        0        0     1354 2023-12-18 12:05:45.780571 gigachain_community-0.0.6.1/langchain_community/tools/brave_search/tool.py
+-rw-r--r--   0        0        0        0 2023-12-18 12:05:45.780739 gigachain_community-0.0.6.1/langchain_community/tools/clickup/__init__.py
+-rw-r--r--   0        0        0     8298 2023-12-18 12:05:45.781291 gigachain_community-0.0.6.1/langchain_community/tools/clickup/prompt.py
+-rw-r--r--   0        0        0     1230 2023-12-18 12:05:45.781701 gigachain_community-0.0.6.1/langchain_community/tools/clickup/tool.py
+-rw-r--r--   0        0        0     1336 2023-12-18 12:05:45.782109 gigachain_community-0.0.6.1/langchain_community/tools/convert_to_openai.py
+-rw-r--r--   0        0        0      268 2023-12-18 12:05:45.782537 gigachain_community-0.0.6.1/langchain_community/tools/dataforseo_api_search/__init__.py
+-rw-r--r--   0        0        0     2214 2023-12-18 12:05:45.783121 gigachain_community-0.0.6.1/langchain_community/tools/dataforseo_api_search/tool.py
+-rw-r--r--   0        0        0      147 2023-12-18 12:05:45.783495 gigachain_community-0.0.6.1/langchain_community/tools/ddg_search/__init__.py
+-rw-r--r--   0        0        0     2641 2023-12-21 15:51:51.835050 gigachain_community-0.0.6.1/langchain_community/tools/ddg_search/tool.py
+-rw-r--r--   0        0        0        0 2023-12-18 12:05:45.783987 gigachain_community-0.0.6.1/langchain_community/tools/e2b_data_analysis/__init__.py
+-rw-r--r--   0        0        0     8015 2023-12-28 13:38:34.503446 gigachain_community-0.0.6.1/langchain_community/tools/e2b_data_analysis/tool.py
+-rw-r--r--   0        0        0    20701 2023-12-21 15:51:51.836025 gigachain_community-0.0.6.1/langchain_community/tools/e2b_data_analysis/unparse.py
+-rw-r--r--   0        0        0     1024 2023-12-18 12:05:45.785160 gigachain_community-0.0.6.1/langchain_community/tools/edenai/__init__.py
+-rw-r--r--   0        0        0     3465 2023-12-18 12:05:45.785432 gigachain_community-0.0.6.1/langchain_community/tools/edenai/audio_speech_to_text.py
+-rw-r--r--   0        0        0     3885 2023-12-18 12:05:45.785916 gigachain_community-0.0.6.1/langchain_community/tools/edenai/audio_text_to_speech.py
+-rw-r--r--   0        0        0     5386 2023-12-18 12:05:45.786625 gigachain_community-0.0.6.1/langchain_community/tools/edenai/edenai_base_tool.py
+-rw-r--r--   0        0        0     2249 2023-12-18 12:05:45.787257 gigachain_community-0.0.6.1/langchain_community/tools/edenai/image_explicitcontent.py
+-rw-r--r--   0        0        0     2476 2023-12-18 12:05:45.787647 gigachain_community-0.0.6.1/langchain_community/tools/edenai/image_objectdetection.py
+-rw-r--r--   0        0        0     1966 2023-12-18 12:05:45.788039 gigachain_community-0.0.6.1/langchain_community/tools/edenai/ocr_identityparser.py
+-rw-r--r--   0        0        0     2187 2023-12-18 12:05:45.788452 gigachain_community-0.0.6.1/langchain_community/tools/edenai/ocr_invoiceparser.py
+-rw-r--r--   0        0        0     2407 2023-12-18 12:05:45.789172 gigachain_community-0.0.6.1/langchain_community/tools/edenai/text_moderation.py
+-rw-r--r--   0        0        0      164 2023-12-18 12:05:45.789668 gigachain_community-0.0.6.1/langchain_community/tools/eleven_labs/__init__.py
+-rw-r--r--   0        0        0      203 2023-12-18 12:05:45.790052 gigachain_community-0.0.6.1/langchain_community/tools/eleven_labs/models.py
+-rw-r--r--   0        0        0     2709 2023-12-18 12:05:45.790521 gigachain_community-0.0.6.1/langchain_community/tools/eleven_labs/text2speech.py
+-rw-r--r--   0        0        0      723 2023-12-18 12:05:45.791133 gigachain_community-0.0.6.1/langchain_community/tools/file_management/__init__.py
+-rw-r--r--   0        0        0     1749 2023-12-18 12:05:45.791626 gigachain_community-0.0.6.1/langchain_community/tools/file_management/copy.py
+-rw-r--r--   0        0        0     1345 2023-12-18 12:05:45.791998 gigachain_community-0.0.6.1/langchain_community/tools/file_management/delete.py
+-rw-r--r--   0        0        0     1965 2023-12-18 12:05:45.792403 gigachain_community-0.0.6.1/langchain_community/tools/file_management/file_search.py
+-rw-r--r--   0        0        0     1432 2023-12-18 12:05:45.792791 gigachain_community-0.0.6.1/langchain_community/tools/file_management/list_dir.py
+-rw-r--r--   0        0        0     1889 2023-12-18 12:05:45.793186 gigachain_community-0.0.6.1/langchain_community/tools/file_management/move.py
+-rw-r--r--   0        0        0     1340 2023-12-18 12:05:45.793625 gigachain_community-0.0.6.1/langchain_community/tools/file_management/read.py
+-rw-r--r--   0        0        0     1726 2023-12-18 12:05:45.794428 gigachain_community-0.0.6.1/langchain_community/tools/file_management/utils.py
+-rw-r--r--   0        0        0     1614 2023-12-18 12:05:45.794830 gigachain_community-0.0.6.1/langchain_community/tools/file_management/write.py
+-rw-r--r--   0        0        0       20 2023-12-18 12:05:45.795246 gigachain_community-0.0.6.1/langchain_community/tools/github/__init__.py
+-rw-r--r--   0        0        0     6220 2023-12-18 12:05:45.795757 gigachain_community-0.0.6.1/langchain_community/tools/github/prompt.py
+-rw-r--r--   0        0        0     1194 2023-12-18 12:05:45.796153 gigachain_community-0.0.6.1/langchain_community/tools/github/tool.py
+-rw-r--r--   0        0        0       20 2023-12-18 12:05:45.796530 gigachain_community-0.0.6.1/langchain_community/tools/gitlab/__init__.py
+-rw-r--r--   0        0        0     3438 2023-12-18 12:05:45.797359 gigachain_community-0.0.6.1/langchain_community/tools/gitlab/prompt.py
+-rw-r--r--   0        0        0      972 2023-12-18 12:05:45.797816 gigachain_community-0.0.6.1/langchain_community/tools/gitlab/tool.py
+-rw-r--r--   0        0        0      601 2023-12-18 12:05:45.798228 gigachain_community-0.0.6.1/langchain_community/tools/gmail/__init__.py
+-rw-r--r--   0        0        0     1004 2023-12-18 12:05:45.798672 gigachain_community-0.0.6.1/langchain_community/tools/gmail/base.py
+-rw-r--r--   0        0        0     2564 2023-12-18 12:05:45.799060 gigachain_community-0.0.6.1/langchain_community/tools/gmail/create_draft.py
+-rw-r--r--   0        0        0     2202 2023-12-18 12:05:45.799653 gigachain_community-0.0.6.1/langchain_community/tools/gmail/get_message.py
+-rw-r--r--   0        0        0     1560 2023-12-18 12:05:45.800071 gigachain_community-0.0.6.1/langchain_community/tools/gmail/get_thread.py
+-rw-r--r--   0        0        0     4874 2023-12-18 12:05:45.801270 gigachain_community-0.0.6.1/langchain_community/tools/gmail/search.py
+-rw-r--r--   0        0        0     2939 2023-12-28 13:38:34.504472 gigachain_community-0.0.6.1/langchain_community/tools/gmail/send_message.py
+-rw-r--r--   0        0        0     4528 2023-12-18 12:05:45.802173 gigachain_community-0.0.6.1/langchain_community/tools/gmail/utils.py
+-rw-r--r--   0        0        0      136 2023-12-18 12:05:45.802569 gigachain_community-0.0.6.1/langchain_community/tools/golden_query/__init__.py
+-rw-r--r--   0        0        0     1108 2023-12-18 12:05:45.802914 gigachain_community-0.0.6.1/langchain_community/tools/golden_query/tool.py
+-rw-r--r--   0        0        0      171 2023-12-18 12:05:45.803350 gigachain_community-0.0.6.1/langchain_community/tools/google_cloud/__init__.py
+-rw-r--r--   0        0        0     3173 2023-12-18 12:05:45.803756 gigachain_community-0.0.6.1/langchain_community/tools/google_cloud/texttospeech.py
+-rw-r--r--   0        0        0      152 2023-12-18 12:05:45.805823 gigachain_community-0.0.6.1/langchain_community/tools/google_finance/__init__.py
+-rw-r--r--   0        0        0      854 2023-12-18 12:05:45.806289 gigachain_community-0.0.6.1/langchain_community/tools/google_finance/tool.py
+-rw-r--r--   0        0        0      140 2023-12-18 12:05:45.806731 gigachain_community-0.0.6.1/langchain_community/tools/google_jobs/__init__.py
+-rw-r--r--   0        0        0      826 2023-12-18 12:05:45.807119 gigachain_community-0.0.6.1/langchain_community/tools/google_jobs/tool.py
+-rw-r--r--   0        0        0      140 2023-12-18 12:05:45.807515 gigachain_community-0.0.6.1/langchain_community/tools/google_lens/__init__.py
+-rw-r--r--   0        0        0      822 2023-12-18 12:05:45.807846 gigachain_community-0.0.6.1/langchain_community/tools/google_lens/tool.py
+-rw-r--r--   0        0        0      140 2023-12-18 12:05:45.808212 gigachain_community-0.0.6.1/langchain_community/tools/google_places/__init__.py
+-rw-r--r--   0        0        0     1141 2023-12-18 12:05:45.808602 gigachain_community-0.0.6.1/langchain_community/tools/google_places/tool.py
+-rw-r--r--   0        0        0      152 2023-12-18 12:05:45.809035 gigachain_community-0.0.6.1/langchain_community/tools/google_scholar/__init__.py
+-rw-r--r--   0        0        0      847 2023-12-18 12:05:45.809424 gigachain_community-0.0.6.1/langchain_community/tools/google_scholar/tool.py
+-rw-r--r--   0        0        0      195 2023-12-18 12:05:45.810892 gigachain_community-0.0.6.1/langchain_community/tools/google_search/__init__.py
+-rw-r--r--   0        0        0     1489 2023-12-18 12:05:45.811333 gigachain_community-0.0.6.1/langchain_community/tools/google_search/tool.py
+-rw-r--r--   0        0        0      243 2023-12-18 12:05:45.811765 gigachain_community-0.0.6.1/langchain_community/tools/google_serper/__init__.py
+-rw-r--r--   0        0        0     2113 2023-12-18 12:05:45.812243 gigachain_community-0.0.6.1/langchain_community/tools/google_serper/tool.py
+-rw-r--r--   0        0        0      148 2023-12-18 12:05:45.812859 gigachain_community-0.0.6.1/langchain_community/tools/google_trends/__init__.py
+-rw-r--r--   0        0        0      844 2023-12-18 12:05:45.813598 gigachain_community-0.0.6.1/langchain_community/tools/google_trends/tool.py
+-rw-r--r--   0        0        0       47 2023-12-18 12:05:45.813986 gigachain_community-0.0.6.1/langchain_community/tools/graphql/__init__.py
+-rw-r--r--   0        0        0     1204 2023-12-18 12:05:45.814359 gigachain_community-0.0.6.1/langchain_community/tools/graphql/tool.py
+-rw-r--r--   0        0        0      132 2023-12-18 12:05:45.814785 gigachain_community-0.0.6.1/langchain_community/tools/human/__init__.py
+-rw-r--r--   0        0        0      983 2023-12-18 12:05:45.815173 gigachain_community-0.0.6.1/langchain_community/tools/human/tool.py
+-rw-r--r--   0        0        0     2286 2023-12-18 12:05:45.815512 gigachain_community-0.0.6.1/langchain_community/tools/ifttt.py
+-rw-r--r--   0        0        0       43 2023-12-18 12:05:45.815966 gigachain_community-0.0.6.1/langchain_community/tools/interaction/__init__.py
+-rw-r--r--   0        0        0      464 2023-12-18 12:05:45.816375 gigachain_community-0.0.6.1/langchain_community/tools/interaction/tool.py
+-rw-r--r--   0        0        0       17 2023-12-18 12:05:45.817112 gigachain_community-0.0.6.1/langchain_community/tools/jira/__init__.py
+-rw-r--r--   0        0        0     3170 2023-12-18 12:05:45.818054 gigachain_community-0.0.6.1/langchain_community/tools/jira/prompt.py
+-rw-r--r--   0        0        0     1342 2023-12-18 12:05:45.818546 gigachain_community-0.0.6.1/langchain_community/tools/jira/tool.py
+-rw-r--r--   0        0        0       46 2023-12-18 12:05:45.819119 gigachain_community-0.0.6.1/langchain_community/tools/json/__init__.py
+-rw-r--r--   0        0        0     4139 2023-12-18 12:05:45.819580 gigachain_community-0.0.6.1/langchain_community/tools/json/tool.py
+-rw-r--r--   0        0        0      134 2023-12-18 12:05:45.820014 gigachain_community-0.0.6.1/langchain_community/tools/memorize/__init__.py
+-rw-r--r--   0        0        0     1828 2023-12-21 15:51:51.837175 gigachain_community-0.0.6.1/langchain_community/tools/memorize/tool.py
+-rw-r--r--   0        0        0       35 2023-12-18 12:05:45.821474 gigachain_community-0.0.6.1/langchain_community/tools/merriam_webster/__init__.py
+-rw-r--r--   0        0        0      853 2023-12-18 12:05:45.822073 gigachain_community-0.0.6.1/langchain_community/tools/merriam_webster/tool.py
+-rw-r--r--   0        0        0      154 2023-12-18 12:05:45.822754 gigachain_community-0.0.6.1/langchain_community/tools/metaphor_search/__init__.py
+-rw-r--r--   0        0        0     2690 2023-12-18 12:05:45.823297 gigachain_community-0.0.6.1/langchain_community/tools/metaphor_search/tool.py
+-rw-r--r--   0        0        0      359 2023-12-18 12:05:45.823831 gigachain_community-0.0.6.1/langchain_community/tools/multion/__init__.py
+-rw-r--r--   0        0        0     2052 2023-12-18 12:05:45.824250 gigachain_community-0.0.6.1/langchain_community/tools/multion/close_session.py
+-rw-r--r--   0        0        0     2585 2023-12-18 12:05:45.824782 gigachain_community-0.0.6.1/langchain_community/tools/multion/create_session.py
+-rw-r--r--   0        0        0     2822 2023-12-18 12:05:45.825198 gigachain_community-0.0.6.1/langchain_community/tools/multion/update_session.py
+-rw-r--r--   0        0        0        0 2023-12-18 12:05:45.825384 gigachain_community-0.0.6.1/langchain_community/tools/nasa/__init__.py
+-rw-r--r--   0        0        0     5197 2023-12-18 12:05:45.825968 gigachain_community-0.0.6.1/langchain_community/tools/nasa/prompt.py
+-rw-r--r--   0        0        0      831 2023-12-18 12:05:45.826349 gigachain_community-0.0.6.1/langchain_community/tools/nasa/tool.py
+-rw-r--r--   0        0        0      111 2023-12-18 12:05:45.826705 gigachain_community-0.0.6.1/langchain_community/tools/nuclia/__init__.py
+-rw-r--r--   0        0        0     7915 2023-12-18 12:05:45.827114 gigachain_community-0.0.6.1/langchain_community/tools/nuclia/tool.py
+-rw-r--r--   0        0        0      654 2023-12-18 12:05:45.827517 gigachain_community-0.0.6.1/langchain_community/tools/office365/__init__.py
+-rw-r--r--   0        0        0      508 2023-12-18 12:05:45.827887 gigachain_community-0.0.6.1/langchain_community/tools/office365/base.py
+-rw-r--r--   0        0        0     1858 2023-12-18 12:05:45.828512 gigachain_community-0.0.6.1/langchain_community/tools/office365/create_draft_message.py
+-rw-r--r--   0        0        0     4833 2023-12-18 12:05:45.828888 gigachain_community-0.0.6.1/langchain_community/tools/office365/events_search.py
+-rw-r--r--   0        0        0     4246 2023-12-18 12:05:45.829447 gigachain_community-0.0.6.1/langchain_community/tools/office365/messages_search.py
+-rw-r--r--   0        0        0     2898 2023-12-18 12:05:45.829858 gigachain_community-0.0.6.1/langchain_community/tools/office365/send_event.py
+-rw-r--r--   0        0        0     1789 2023-12-18 12:05:45.830410 gigachain_community-0.0.6.1/langchain_community/tools/office365/send_message.py
+-rw-r--r--   0        0        0     2212 2023-12-18 12:05:45.831194 gigachain_community-0.0.6.1/langchain_community/tools/office365/utils.py
+-rw-r--r--   0        0        0        0 2023-12-18 12:05:45.831412 gigachain_community-0.0.6.1/langchain_community/tools/openapi/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-18 12:05:45.831880 gigachain_community-0.0.6.1/langchain_community/tools/openapi/utils/__init__.py
+-rw-r--r--   0        0        0    21288 2023-12-18 12:05:45.832707 gigachain_community-0.0.6.1/langchain_community/tools/openapi/utils/api_models.py
+-rw-r--r--   0        0        0      191 2023-12-18 12:05:45.833201 gigachain_community-0.0.6.1/langchain_community/tools/openapi/utils/openapi_utils.py
+-rw-r--r--   0        0        0      162 2023-12-18 12:05:45.833667 gigachain_community-0.0.6.1/langchain_community/tools/openweathermap/__init__.py
+-rw-r--r--   0        0        0      966 2023-12-18 12:05:45.834076 gigachain_community-0.0.6.1/langchain_community/tools/openweathermap/tool.py
+-rw-r--r--   0        0        0      763 2023-12-18 12:05:45.834481 gigachain_community-0.0.6.1/langchain_community/tools/playwright/__init__.py
+-rw-r--r--   0        0        0     2135 2023-12-18 12:05:45.834869 gigachain_community-0.0.6.1/langchain_community/tools/playwright/base.py
+-rw-r--r--   0        0        0     3083 2023-12-18 12:05:45.835282 gigachain_community-0.0.6.1/langchain_community/tools/playwright/click.py
+-rw-r--r--   0        0        0     1340 2023-12-18 12:05:45.835906 gigachain_community-0.0.6.1/langchain_community/tools/playwright/current_page.py
+-rw-r--r--   0        0        0     3051 2023-12-18 12:05:45.836449 gigachain_community-0.0.6.1/langchain_community/tools/playwright/extract_hyperlinks.py
+-rw-r--r--   0        0        0     2383 2023-12-18 12:05:45.836893 gigachain_community-0.0.6.1/langchain_community/tools/playwright/extract_text.py
+-rw-r--r--   0        0        0     3743 2023-12-18 12:05:45.837329 gigachain_community-0.0.6.1/langchain_community/tools/playwright/get_elements.py
+-rw-r--r--   0        0        0     2878 2023-12-18 12:05:45.837738 gigachain_community-0.0.6.1/langchain_community/tools/playwright/navigate.py
+-rw-r--r--   0        0        0     1926 2023-12-18 12:05:45.838120 gigachain_community-0.0.6.1/langchain_community/tools/playwright/navigate_back.py
+-rw-r--r--   0        0        0     3049 2023-12-18 12:05:45.838549 gigachain_community-0.0.6.1/langchain_community/tools/playwright/utils.py
+-rw-r--r--   0        0        0     2902 2023-12-18 12:05:45.838925 gigachain_community-0.0.6.1/langchain_community/tools/plugin.py
+-rw-r--r--   0        0        0       52 2023-12-18 12:05:45.839326 gigachain_community-0.0.6.1/langchain_community/tools/powerbi/__init__.py
+-rw-r--r--   0        0        0     7339 2023-12-18 12:05:45.839823 gigachain_community-0.0.6.1/langchain_community/tools/powerbi/prompt.py
+-rw-r--r--   0        0        0    11075 2023-12-18 12:05:45.840707 gigachain_community-0.0.6.1/langchain_community/tools/powerbi/tool.py
+-rw-r--r--   0        0        0       26 2023-12-18 12:05:45.841143 gigachain_community-0.0.6.1/langchain_community/tools/pubmed/__init__.py
+-rw-r--r--   0        0        0      944 2023-12-18 12:05:45.841564 gigachain_community-0.0.6.1/langchain_community/tools/pubmed/tool.py
+-rw-r--r--   0        0        0     1965 2023-12-18 12:05:45.842001 gigachain_community-0.0.6.1/langchain_community/tools/reddit_search/tool.py
+-rw-r--r--   0        0        0     1586 2023-12-18 12:05:45.842412 gigachain_community-0.0.6.1/langchain_community/tools/render.py
+-rw-r--r--   0        0        0       52 2023-12-18 12:05:45.842780 gigachain_community-0.0.6.1/langchain_community/tools/requests/__init__.py
+-rw-r--r--   0        0        0     6323 2023-12-18 12:05:45.843362 gigachain_community-0.0.6.1/langchain_community/tools/requests/tool.py
+-rw-r--r--   0        0        0       31 2023-12-18 12:05:45.843730 gigachain_community-0.0.6.1/langchain_community/tools/scenexplain/__init__.py
+-rw-r--r--   0        0        0     1100 2023-12-18 12:05:45.844164 gigachain_community-0.0.6.1/langchain_community/tools/scenexplain/tool.py
+-rw-r--r--   0        0        0      214 2023-12-18 12:05:45.844592 gigachain_community-0.0.6.1/langchain_community/tools/searchapi/__init__.py
+-rw-r--r--   0        0        0     2114 2023-12-18 12:05:45.844972 gigachain_community-0.0.6.1/langchain_community/tools/searchapi/tool.py
+-rw-r--r--   0        0        0        0 2023-12-18 12:05:45.845178 gigachain_community-0.0.6.1/langchain_community/tools/searx_search/__init__.py
+-rw-r--r--   0        0        0     2261 2023-12-18 12:05:45.845824 gigachain_community-0.0.6.1/langchain_community/tools/searx_search/tool.py
+-rw-r--r--   0        0        0      103 2023-12-18 12:05:45.846255 gigachain_community-0.0.6.1/langchain_community/tools/shell/__init__.py
+-rw-r--r--   0        0        0     2663 2023-12-18 12:05:45.846662 gigachain_community-0.0.6.1/langchain_community/tools/shell/tool.py
+-rw-r--r--   0        0        0      502 2023-12-18 12:05:45.847147 gigachain_community-0.0.6.1/langchain_community/tools/slack/__init__.py
+-rw-r--r--   0        0        0      460 2023-12-18 12:05:45.847474 gigachain_community-0.0.6.1/langchain_community/tools/slack/base.py
+-rw-r--r--   0        0        0     1118 2023-12-21 15:51:51.838169 gigachain_community-0.0.6.1/langchain_community/tools/slack/get_channel.py
+-rw-r--r--   0        0        0     1402 2023-12-21 15:51:51.839105 gigachain_community-0.0.6.1/langchain_community/tools/slack/get_message.py
+-rw-r--r--   0        0        0     2071 2023-12-18 12:05:45.848876 gigachain_community-0.0.6.1/langchain_community/tools/slack/schedule_message.py
+-rw-r--r--   0        0        0     1222 2023-12-18 12:05:45.849246 gigachain_community-0.0.6.1/langchain_community/tools/slack/send_message.py
+-rw-r--r--   0        0        0     1135 2023-12-18 12:05:45.849856 gigachain_community-0.0.6.1/langchain_community/tools/slack/utils.py
+-rw-r--r--   0        0        0       18 2023-12-18 12:05:45.850305 gigachain_community-0.0.6.1/langchain_community/tools/sleep/__init__.py
+-rw-r--r--   0        0        0     1229 2023-12-18 12:05:45.850716 gigachain_community-0.0.6.1/langchain_community/tools/sleep/tool.py
+-rw-r--r--   0        0        0       44 2023-12-18 12:05:45.851086 gigachain_community-0.0.6.1/langchain_community/tools/spark_sql/__init__.py
+-rw-r--r--   0        0        0      550 2023-12-18 12:05:45.851476 gigachain_community-0.0.6.1/langchain_community/tools/spark_sql/prompt.py
+-rw-r--r--   0        0        0     4376 2023-12-18 12:05:45.851871 gigachain_community-0.0.6.1/langchain_community/tools/spark_sql/tool.py
+-rw-r--r--   0        0        0       49 2023-12-18 12:05:45.852158 gigachain_community-0.0.6.1/langchain_community/tools/sql_database/__init__.py
+-rw-r--r--   0        0        0      597 2023-12-18 12:05:45.852450 gigachain_community-0.0.6.1/langchain_community/tools/sql_database/prompt.py
+-rw-r--r--   0        0        0     4487 2023-12-18 12:05:45.852922 gigachain_community-0.0.6.1/langchain_community/tools/sql_database/tool.py
+-rw-r--r--   0        0        0       33 2023-12-18 12:05:45.853383 gigachain_community-0.0.6.1/langchain_community/tools/stackexchange/__init__.py
+-rw-r--r--   0        0        0      868 2023-12-18 12:05:45.853792 gigachain_community-0.0.6.1/langchain_community/tools/stackexchange/tool.py
+-rw-r--r--   0        0        0       24 2023-12-18 12:05:45.854296 gigachain_community-0.0.6.1/langchain_community/tools/steam/__init__.py
+-rw-r--r--   0        0        0     1657 2023-12-18 12:05:45.854700 gigachain_community-0.0.6.1/langchain_community/tools/steam/prompt.py
+-rw-r--r--   0        0        0      842 2023-12-18 12:05:45.855152 gigachain_community-0.0.6.1/langchain_community/tools/steam/tool.py
+-rw-r--r--   0        0        0      186 2023-12-18 12:05:45.855742 gigachain_community-0.0.6.1/langchain_community/tools/steamship_image_generation/__init__.py
+-rw-r--r--   0        0        0     3377 2023-12-18 12:05:45.856114 gigachain_community-0.0.6.1/langchain_community/tools/steamship_image_generation/tool.py
+-rw-r--r--   0        0        0     1395 2023-12-18 12:05:45.856475 gigachain_community-0.0.6.1/langchain_community/tools/steamship_image_generation/utils.py
+-rw-r--r--   0        0        0      189 2023-12-18 12:05:45.856940 gigachain_community-0.0.6.1/langchain_community/tools/tavily_search/__init__.py
+-rw-r--r--   0        0        0     3375 2023-12-28 13:38:34.505773 gigachain_community-0.0.6.1/langchain_community/tools/tavily_search/tool.py
+-rw-r--r--   0        0        0       51 2023-12-18 12:05:45.858009 gigachain_community-0.0.6.1/langchain_community/tools/vectorstore/__init__.py
+-rw-r--r--   0        0        0     3302 2023-12-18 12:05:45.858410 gigachain_community-0.0.6.1/langchain_community/tools/vectorstore/tool.py
+-rw-r--r--   0        0        0       29 2023-12-18 12:05:45.858782 gigachain_community-0.0.6.1/langchain_community/tools/wikipedia/__init__.py
+-rw-r--r--   0        0        0      867 2023-12-18 12:05:45.859163 gigachain_community-0.0.6.1/langchain_community/tools/wikipedia/tool.py
+-rw-r--r--   0        0        0      156 2023-12-18 12:05:45.859606 gigachain_community-0.0.6.1/langchain_community/tools/wolfram_alpha/__init__.py
+-rw-r--r--   0        0        0      887 2023-12-18 12:05:45.859959 gigachain_community-0.0.6.1/langchain_community/tools/wolfram_alpha/tool.py
+-rw-r--r--   0        0        0     2473 2023-12-18 12:05:45.860331 gigachain_community-0.0.6.1/langchain_community/tools/yahoo_finance_news.py
+-rw-r--r--   0        0        0        0 2023-12-18 12:05:45.860527 gigachain_community-0.0.6.1/langchain_community/tools/youtube/__init__.py
+-rw-r--r--   0        0        0     1729 2023-12-18 12:05:45.861292 gigachain_community-0.0.6.1/langchain_community/tools/youtube/search.py
+-rw-r--r--   0        0        0      193 2023-12-18 12:05:45.861830 gigachain_community-0.0.6.1/langchain_community/tools/zapier/__init__.py
+-rw-r--r--   0        0        0     1182 2023-12-18 12:05:45.862240 gigachain_community-0.0.6.1/langchain_community/tools/zapier/prompt.py
+-rw-r--r--   0        0        0     7730 2023-12-18 12:05:45.863337 gigachain_community-0.0.6.1/langchain_community/tools/zapier/tool.py
+-rw-r--r--   0        0        0    10998 2023-12-18 12:05:45.864315 gigachain_community-0.0.6.1/langchain_community/utilities/__init__.py
+-rw-r--r--   0        0        0     2192 2023-12-18 12:05:45.864880 gigachain_community-0.0.6.1/langchain_community/utilities/alpha_vantage.py
+-rw-r--r--   0        0        0      844 2023-12-18 12:05:45.865288 gigachain_community-0.0.6.1/langchain_community/utilities/anthropic.py
+-rw-r--r--   0        0        0     8458 2023-12-18 12:05:45.865753 gigachain_community-0.0.6.1/langchain_community/utilities/apify.py
+-rw-r--r--   0        0        0     8710 2023-12-18 12:05:45.866259 gigachain_community-0.0.6.1/langchain_community/utilities/arcee.py
+-rw-r--r--   0        0        0     9262 2023-12-21 15:51:51.841117 gigachain_community-0.0.6.1/langchain_community/utilities/arxiv.py
+-rw-r--r--   0        0        0     2437 2023-12-18 12:05:45.867481 gigachain_community-0.0.6.1/langchain_community/utilities/awslambda.py
+-rw-r--r--   0        0        0     2499 2023-12-18 12:05:45.867932 gigachain_community-0.0.6.1/langchain_community/utilities/bibtex.py
+-rw-r--r--   0        0        0     3545 2023-12-18 12:05:45.868301 gigachain_community-0.0.6.1/langchain_community/utilities/bing_search.py
+-rw-r--r--   0        0        0     2356 2023-12-18 12:05:45.868774 gigachain_community-0.0.6.1/langchain_community/utilities/brave_search.py
+-rw-r--r--   0        0        0    19771 2023-12-18 12:05:45.869364 gigachain_community-0.0.6.1/langchain_community/utilities/clickup.py
+-rw-r--r--   0        0        0     6377 2023-12-18 12:05:45.870021 gigachain_community-0.0.6.1/langchain_community/utilities/dalle_image_generator.py
+-rw-r--r--   0        0        0     7854 2023-12-18 12:05:45.870814 gigachain_community-0.0.6.1/langchain_community/utilities/dataforseo_api_search.py
+-rw-r--r--   0        0        0     4310 2023-12-18 12:05:45.871460 gigachain_community-0.0.6.1/langchain_community/utilities/duckduckgo_search.py
+-rw-r--r--   0        0        0    31986 2023-12-21 15:51:51.842273 gigachain_community-0.0.6.1/langchain_community/utilities/github.py
+-rw-r--r--   0        0        0    11959 2023-12-18 12:05:45.872934 gigachain_community-0.0.6.1/langchain_community/utilities/gitlab.py
+-rw-r--r--   0        0        0     1858 2023-12-18 12:05:45.873304 gigachain_community-0.0.6.1/langchain_community/utilities/golden_query.py
+-rw-r--r--   0        0        0     3400 2023-12-21 15:51:51.843661 gigachain_community-0.0.6.1/langchain_community/utilities/google_finance.py
+-rw-r--r--   0        0        0     2804 2023-12-21 15:51:51.844769 gigachain_community-0.0.6.1/langchain_community/utilities/google_jobs.py
+-rw-r--r--   0        0        0     2859 2023-12-18 12:05:45.874583 gigachain_community-0.0.6.1/langchain_community/utilities/google_lens.py
+-rw-r--r--   0        0        0     4107 2023-12-18 12:05:45.874988 gigachain_community-0.0.6.1/langchain_community/utilities/google_places_api.py
+-rw-r--r--   0        0        0     5171 2023-12-18 12:05:45.875442 gigachain_community-0.0.6.1/langchain_community/utilities/google_scholar.py
+-rw-r--r--   0        0        0     5048 2023-12-18 12:05:45.876258 gigachain_community-0.0.6.1/langchain_community/utilities/google_search.py
+-rw-r--r--   0        0        0     6503 2023-12-18 12:05:45.876775 gigachain_community-0.0.6.1/langchain_community/utilities/google_serper.py
+-rw-r--r--   0        0        0     4033 2023-12-18 12:05:45.877158 gigachain_community-0.0.6.1/langchain_community/utilities/google_trends.py
+-rw-r--r--   0        0        0     1903 2023-12-18 12:05:45.877780 gigachain_community-0.0.6.1/langchain_community/utilities/graphql.py
+-rw-r--r--   0        0        0     6195 2023-12-18 12:05:45.878463 gigachain_community-0.0.6.1/langchain_community/utilities/jira.py
+-rw-r--r--   0        0        0     2647 2023-12-18 12:05:45.879155 gigachain_community-0.0.6.1/langchain_community/utilities/max_compute.py
+-rw-r--r--   0        0        0     3748 2023-12-18 12:05:45.879594 gigachain_community-0.0.6.1/langchain_community/utilities/merriam_webster.py
+-rw-r--r--   0        0        0     6809 2023-12-18 12:05:45.880096 gigachain_community-0.0.6.1/langchain_community/utilities/metaphor_search.py
+-rw-r--r--   0        0        0     1820 2023-12-21 15:51:51.846047 gigachain_community-0.0.6.1/langchain_community/utilities/nasa.py
+-rw-r--r--   0        0        0     3287 2023-12-18 12:05:45.881008 gigachain_community-0.0.6.1/langchain_community/utilities/opaqueprompts.py
+-rw-r--r--   0        0        0    11017 2023-12-18 12:05:45.881524 gigachain_community-0.0.6.1/langchain_community/utilities/openapi.py
+-rw-r--r--   0        0        0     2462 2023-12-18 12:05:45.882200 gigachain_community-0.0.6.1/langchain_community/utilities/openweathermap.py
+-rw-r--r--   0        0        0     3351 2023-12-18 12:05:45.882568 gigachain_community-0.0.6.1/langchain_community/utilities/outline.py
+-rw-r--r--   0        0        0     2355 2023-12-18 12:05:45.883116 gigachain_community-0.0.6.1/langchain_community/utilities/portkey.py
+-rw-r--r--   0        0        0    11246 2023-12-18 12:05:45.883973 gigachain_community-0.0.6.1/langchain_community/utilities/powerbi.py
+-rw-r--r--   0        0        0     6936 2023-12-18 12:05:45.884535 gigachain_community-0.0.6.1/langchain_community/utilities/pubmed.py
+-rw-r--r--   0        0        0     2159 2023-12-18 12:05:45.885022 gigachain_community-0.0.6.1/langchain_community/utilities/python.py
+-rw-r--r--   0        0        0     4474 2023-12-18 12:05:45.885341 gigachain_community-0.0.6.1/langchain_community/utilities/reddit_search.py
+-rw-r--r--   0        0        0     8221 2023-12-18 12:05:45.885856 gigachain_community-0.0.6.1/langchain_community/utilities/redis.py
+-rw-r--r--   0        0        0     6992 2023-12-18 12:05:45.886179 gigachain_community-0.0.6.1/langchain_community/utilities/requests.py
+-rw-r--r--   0        0        0     2220 2023-12-18 12:05:45.886517 gigachain_community-0.0.6.1/langchain_community/utilities/scenexplain.py
+-rw-r--r--   0        0        0     5226 2023-12-18 12:05:45.887002 gigachain_community-0.0.6.1/langchain_community/utilities/searchapi.py
+-rw-r--r--   0        0        0    16625 2023-12-18 12:05:45.887512 gigachain_community-0.0.6.1/langchain_community/utilities/searx_search.py
+-rw-r--r--   0        0        0     8490 2023-12-18 12:05:45.889068 gigachain_community-0.0.6.1/langchain_community/utilities/serpapi.py
+-rw-r--r--   0        0        0     7519 2023-12-18 12:05:45.889509 gigachain_community-0.0.6.1/langchain_community/utilities/spark_sql.py
+-rw-r--r--   0        0        0    19639 2023-12-21 15:51:51.847139 gigachain_community-0.0.6.1/langchain_community/utilities/sql_database.py
+-rw-r--r--   0        0        0     2639 2023-12-18 12:05:45.890765 gigachain_community-0.0.6.1/langchain_community/utilities/stackexchange.py
+-rw-r--r--   0        0        0     5857 2023-12-18 12:05:45.891172 gigachain_community-0.0.6.1/langchain_community/utilities/steam.py
+-rw-r--r--   0        0        0     6834 2023-12-18 12:05:45.891644 gigachain_community-0.0.6.1/langchain_community/utilities/tavily_search.py
+-rw-r--r--   0        0        0     4006 2023-12-18 12:05:45.892063 gigachain_community-0.0.6.1/langchain_community/utilities/tensorflow_datasets.py
+-rw-r--r--   0        0        0     3441 2023-12-18 12:05:45.892530 gigachain_community-0.0.6.1/langchain_community/utilities/twilio.py
+-rw-r--r--   0        0        0     4072 2023-12-21 15:51:51.848192 gigachain_community-0.0.6.1/langchain_community/utilities/vertexai.py
+-rw-r--r--   0        0        0     4045 2023-12-18 12:05:45.893264 gigachain_community-0.0.6.1/langchain_community/utilities/wikipedia.py
+-rw-r--r--   0        0        0     2011 2023-12-18 12:05:45.893697 gigachain_community-0.0.6.1/langchain_community/utilities/wolfram_alpha.py
+-rw-r--r--   0        0        0    11666 2023-12-18 12:05:45.894686 gigachain_community-0.0.6.1/langchain_community/utilities/zapier.py
+-rw-r--r--   0        0        0        0 2023-12-18 12:05:45.894897 gigachain_community-0.0.6.1/langchain_community/utils/__init__.py
+-rw-r--r--   0        0        0     2713 2023-12-18 12:05:45.895328 gigachain_community-0.0.6.1/langchain_community/utils/math.py
+-rw-r--r--   0        0        0      264 2023-12-21 15:51:51.849060 gigachain_community-0.0.6.1/langchain_community/utils/openai.py
+-rw-r--r--   0        0        0     1518 2023-12-18 12:05:45.896319 gigachain_community-0.0.6.1/langchain_community/utils/openai_functions.py
+-rw-r--r--   0        0        0    15965 2023-12-21 15:51:51.850380 gigachain_community-0.0.6.1/langchain_community/vectorstores/__init__.py
+-rw-r--r--   0        0        0    19780 2023-12-18 12:05:45.897986 gigachain_community-0.0.6.1/langchain_community/vectorstores/alibabacloud_opensearch.py
+-rw-r--r--   0        0        0    15738 2023-12-18 12:05:45.898774 gigachain_community-0.0.6.1/langchain_community/vectorstores/analyticdb.py
+-rw-r--r--   0        0        0    16632 2023-12-18 12:05:45.899285 gigachain_community-0.0.6.1/langchain_community/vectorstores/annoy.py
+-rw-r--r--   0        0        0    28449 2023-12-18 12:05:45.900342 gigachain_community-0.0.6.1/langchain_community/vectorstores/astradb.py
+-rw-r--r--   0        0        0    12136 2023-12-18 12:05:45.900865 gigachain_community-0.0.6.1/langchain_community/vectorstores/atlas.py
+-rw-r--r--   0        0        0    21155 2023-12-18 12:05:45.918722 gigachain_community-0.0.6.1/langchain_community/vectorstores/awadb.py
+-rw-r--r--   0        0        0    14522 2023-12-18 12:05:45.920951 gigachain_community-0.0.6.1/langchain_community/vectorstores/azure_cosmos_db.py
+-rw-r--r--   0        0        0    27218 2023-12-18 12:05:45.921571 gigachain_community-0.0.6.1/langchain_community/vectorstores/azuresearch.py
+-rw-r--r--   0        0        0    15034 2023-12-18 12:05:45.922399 gigachain_community-0.0.6.1/langchain_community/vectorstores/bageldb.py
+-rw-r--r--   0        0        0    16548 2023-12-18 12:05:45.923166 gigachain_community-0.0.6.1/langchain_community/vectorstores/baiducloud_vector_search.py
+-rw-r--r--   0        0        0    14809 2023-12-18 12:05:45.924380 gigachain_community-0.0.6.1/langchain_community/vectorstores/cassandra.py
+-rw-r--r--   0        0        0    30367 2023-12-18 12:05:45.924915 gigachain_community-0.0.6.1/langchain_community/vectorstores/chroma.py
+-rw-r--r--   0        0        0    10953 2023-12-21 15:51:51.851489 gigachain_community-0.0.6.1/langchain_community/vectorstores/clarifai.py
+-rw-r--r--   0        0        0    17735 2023-12-18 12:05:45.926412 gigachain_community-0.0.6.1/langchain_community/vectorstores/clickhouse.py
+-rw-r--r--   0        0        0    12713 2023-12-21 15:51:51.853117 gigachain_community-0.0.6.1/langchain_community/vectorstores/dashvector.py
+-rw-r--r--   0        0        0    18360 2023-12-18 12:05:45.928909 gigachain_community-0.0.6.1/langchain_community/vectorstores/databricks_vector_search.py
+-rw-r--r--   0        0        0    40265 2023-12-18 12:05:45.929819 gigachain_community-0.0.6.1/langchain_community/vectorstores/deeplake.py
+-rw-r--r--   0        0        0    12973 2023-12-18 12:05:45.930835 gigachain_community-0.0.6.1/langchain_community/vectorstores/dingo.py
+-rw-r--r--   0        0        0      236 2023-12-18 12:05:45.931359 gigachain_community-0.0.6.1/langchain_community/vectorstores/docarray/__init__.py
+-rw-r--r--   0        0        0     6945 2023-12-18 12:05:45.931915 gigachain_community-0.0.6.1/langchain_community/vectorstores/docarray/base.py
+-rw-r--r--   0        0        0     4044 2023-12-18 12:05:45.932338 gigachain_community-0.0.6.1/langchain_community/vectorstores/docarray/hnsw.py
+-rw-r--r--   0        0        0     2418 2023-12-18 12:05:45.932697 gigachain_community-0.0.6.1/langchain_community/vectorstores/docarray/in_memory.py
+-rw-r--r--   0        0        0    28714 2023-12-18 12:05:45.933055 gigachain_community-0.0.6.1/langchain_community/vectorstores/elastic_vector_search.py
+-rw-r--r--   0        0        0    46536 2023-12-18 12:05:45.933608 gigachain_community-0.0.6.1/langchain_community/vectorstores/elasticsearch.py
+-rw-r--r--   0        0        0    14183 2023-12-18 12:05:45.934415 gigachain_community-0.0.6.1/langchain_community/vectorstores/epsilla.py
+-rw-r--r--   0        0        0    42989 2023-12-18 12:05:45.934999 gigachain_community-0.0.6.1/langchain_community/vectorstores/faiss.py
+-rw-r--r--   0        0        0    26837 2023-12-18 12:05:45.935987 gigachain_community-0.0.6.1/langchain_community/vectorstores/hippo.py
+-rw-r--r--   0        0        0    13642 2023-12-18 12:05:45.936884 gigachain_community-0.0.6.1/langchain_community/vectorstores/hologres.py
+-rw-r--r--   0        0        0    14253 2023-12-28 13:38:34.506816 gigachain_community-0.0.6.1/langchain_community/vectorstores/jaguar.py
+-rw-r--r--   0        0        0     4173 2023-12-18 12:05:45.938754 gigachain_community-0.0.6.1/langchain_community/vectorstores/lancedb.py
+-rw-r--r--   0        0        0     7745 2023-12-18 12:05:45.939222 gigachain_community-0.0.6.1/langchain_community/vectorstores/llm_rails.py
+-rw-r--r--   0        0        0    17047 2023-12-18 12:05:45.940104 gigachain_community-0.0.6.1/langchain_community/vectorstores/marqo.py
+-rw-r--r--   0        0        0    21430 2023-12-21 15:51:51.855202 gigachain_community-0.0.6.1/langchain_community/vectorstores/matching_engine.py
+-rw-r--r--   0        0        0    10400 2023-12-18 12:05:45.941286 gigachain_community-0.0.6.1/langchain_community/vectorstores/meilisearch.py
+-rw-r--r--   0        0        0    31749 2023-12-18 12:05:45.941785 gigachain_community-0.0.6.1/langchain_community/vectorstores/milvus.py
+-rw-r--r--   0        0        0    19047 2023-12-28 13:38:34.508044 gigachain_community-0.0.6.1/langchain_community/vectorstores/momento_vector_index.py
+-rw-r--r--   0        0        0    13869 2023-12-21 15:51:51.856691 gigachain_community-0.0.6.1/langchain_community/vectorstores/mongodb_atlas.py
+-rw-r--r--   0        0        0    22546 2023-12-18 12:05:45.943853 gigachain_community-0.0.6.1/langchain_community/vectorstores/myscale.py
+-rw-r--r--   0        0        0    35000 2023-12-21 15:51:51.857828 gigachain_community-0.0.6.1/langchain_community/vectorstores/neo4j_vector.py
+-rw-r--r--   0        0        0     5403 2023-12-18 12:05:45.944847 gigachain_community-0.0.6.1/langchain_community/vectorstores/nucliadb.py
+-rw-r--r--   0        0        0    31850 2023-12-18 12:05:45.946289 gigachain_community-0.0.6.1/langchain_community/vectorstores/opensearch_vector_search.py
+-rw-r--r--   0        0        0    17895 2023-12-18 12:05:45.948220 gigachain_community-0.0.6.1/langchain_community/vectorstores/pgembedding.py
+-rw-r--r--   0        0        0     8891 2023-12-21 15:51:51.859006 gigachain_community-0.0.6.1/langchain_community/vectorstores/pgvecto_rs.py
+-rw-r--r--   0        0        0    34006 2023-12-21 15:51:51.860255 gigachain_community-0.0.6.1/langchain_community/vectorstores/pgvector.py
+-rw-r--r--   0        0        0    17517 2023-12-18 12:05:45.950012 gigachain_community-0.0.6.1/langchain_community/vectorstores/pinecone.py
+-rw-r--r--   0        0        0    89408 2023-12-18 12:05:45.951827 gigachain_community-0.0.6.1/langchain_community/vectorstores/qdrant.py
+-rw-r--r--   0        0        0      265 2023-12-18 12:05:45.952450 gigachain_community-0.0.6.1/langchain_community/vectorstores/redis/__init__.py
+-rw-r--r--   0        0        0    54448 2023-12-18 12:05:45.954415 gigachain_community-0.0.6.1/langchain_community/vectorstores/redis/base.py
+-rw-r--r--   0        0        0      420 2023-12-18 12:05:45.954942 gigachain_community-0.0.6.1/langchain_community/vectorstores/redis/constants.py
+-rw-r--r--   0        0        0    16227 2023-12-18 12:05:45.956102 gigachain_community-0.0.6.1/langchain_community/vectorstores/redis/filters.py
+-rw-r--r--   0        0        0    10419 2023-12-18 12:05:45.957786 gigachain_community-0.0.6.1/langchain_community/vectorstores/redis/schema.py
+-rw-r--r--   0        0        0    12192 2023-12-18 12:05:45.958270 gigachain_community-0.0.6.1/langchain_community/vectorstores/rocksetdb.py
+-rw-r--r--   0        0        0    19610 2023-12-18 12:05:45.958595 gigachain_community-0.0.6.1/langchain_community/vectorstores/scann.py
+-rw-r--r--   0        0        0     9707 2023-12-28 13:38:34.509507 gigachain_community-0.0.6.1/langchain_community/vectorstores/semadb.py
+-rw-r--r--   0        0        0    17628 2023-12-18 12:05:45.959791 gigachain_community-0.0.6.1/langchain_community/vectorstores/singlestoredb.py
+-rw-r--r--   0        0        0    12375 2023-12-21 15:51:51.861914 gigachain_community-0.0.6.1/langchain_community/vectorstores/sklearn.py
+-rw-r--r--   0        0        0     7316 2023-12-18 12:05:45.963006 gigachain_community-0.0.6.1/langchain_community/vectorstores/sqlitevss.py
+-rw-r--r--   0        0        0    17150 2023-12-18 12:05:45.968600 gigachain_community-0.0.6.1/langchain_community/vectorstores/starrocks.py
+-rw-r--r--   0        0        0    15175 2023-12-18 12:05:45.970976 gigachain_community-0.0.6.1/langchain_community/vectorstores/supabase.py
+-rw-r--r--   0        0        0    14706 2023-12-28 13:38:34.510538 gigachain_community-0.0.6.1/langchain_community/vectorstores/surrealdb.py
+-rw-r--r--   0        0        0     9557 2023-12-18 12:05:45.975992 gigachain_community-0.0.6.1/langchain_community/vectorstores/tair.py
+-rw-r--r--   0        0        0    13927 2023-12-21 15:51:51.864636 gigachain_community-0.0.6.1/langchain_community/vectorstores/tencentvectordb.py
+-rw-r--r--   0        0        0     4927 2023-12-18 12:05:45.980251 gigachain_community-0.0.6.1/langchain_community/vectorstores/tigris.py
+-rw-r--r--   0        0        0    28826 2023-12-21 15:51:51.865840 gigachain_community-0.0.6.1/langchain_community/vectorstores/tiledb.py
+-rw-r--r--   0        0        0    29831 2023-12-21 15:51:51.867775 gigachain_community-0.0.6.1/langchain_community/vectorstores/timescalevector.py
+-rw-r--r--   0        0        0     9712 2023-12-18 12:05:45.986913 gigachain_community-0.0.6.1/langchain_community/vectorstores/typesense.py
+-rw-r--r--   0        0        0     5888 2023-12-18 12:05:45.988954 gigachain_community-0.0.6.1/langchain_community/vectorstores/usearch.py
+-rw-r--r--   0        0        0     2474 2023-12-18 12:05:45.989508 gigachain_community-0.0.6.1/langchain_community/vectorstores/utils.py
+-rw-r--r--   0        0        0    12908 2023-12-18 12:05:45.990381 gigachain_community-0.0.6.1/langchain_community/vectorstores/vald.py
+-rw-r--r--   0        0        0    19844 2023-12-18 12:05:45.990761 gigachain_community-0.0.6.1/langchain_community/vectorstores/vearch.py
+-rw-r--r--   0        0        0    21275 2023-12-28 13:38:34.511972 gigachain_community-0.0.6.1/langchain_community/vectorstores/vectara.py
+-rw-r--r--   0        0        0     9785 2023-12-18 12:05:45.998180 gigachain_community-0.0.6.1/langchain_community/vectorstores/vespa.py
+-rw-r--r--   0        0        0    19226 2023-12-18 12:05:46.002110 gigachain_community-0.0.6.1/langchain_community/vectorstores/weaviate.py
+-rw-r--r--   0        0        0     9032 2023-12-18 12:05:46.007223 gigachain_community-0.0.6.1/langchain_community/vectorstores/xata.py
+-rw-r--r--   0        0        0    10761 2023-12-18 12:05:46.013574 gigachain_community-0.0.6.1/langchain_community/vectorstores/yellowbrick.py
+-rw-r--r--   0        0        0    23192 2023-12-18 12:05:46.014090 gigachain_community-0.0.6.1/langchain_community/vectorstores/zep.py
+-rw-r--r--   0        0        0     7575 2023-12-18 12:05:46.016389 gigachain_community-0.0.6.1/langchain_community/vectorstores/zilliz.py
+-rw-r--r--   0        0        0     9700 2024-01-09 14:50:12.847829 gigachain_community-0.0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     7263 1970-01-01 00:00:00.000000 gigachain_community-0.0.6.1/PKG-INFO
```

### Comparing `gigachain_community-0.0.6/README.md` & `gigachain_community-0.0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/adapters/openai.py` & `gigachain_community-0.0.6.1/langchain_community/adapters/openai.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/__init__.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/ainetwork/toolkit.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/ainetwork/toolkit.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/amadeus/toolkit.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/amadeus/toolkit.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/azure_cognitive_services.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/azure_cognitive_services.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/clickup/toolkit.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/clickup/toolkit.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/csv/__init__.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/csv/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/file_management/toolkit.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/file_management/toolkit.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/github/toolkit.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/github/toolkit.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/gitlab/toolkit.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/gitlab/toolkit.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/gmail/toolkit.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/gmail/toolkit.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/jira/toolkit.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/jira/toolkit.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/json/base.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/json/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/json/prompt.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/json/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/json/toolkit.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/json/toolkit.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/multion/toolkit.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/multion/toolkit.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/nasa/toolkit.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/nasa/toolkit.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/nla/tool.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/nla/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/nla/toolkit.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/nla/toolkit.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/office365/toolkit.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/office365/toolkit.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/openapi/base.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/openapi/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/openapi/planner.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/openapi/planner.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/openapi/planner_prompt.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/openapi/planner_prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/openapi/prompt.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/openapi/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/openapi/spec.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/openapi/spec.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/openapi/toolkit.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/openapi/toolkit.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/playwright/toolkit.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/playwright/toolkit.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/powerbi/base.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/powerbi/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/powerbi/chat_base.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/powerbi/chat_base.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/powerbi/prompt.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/powerbi/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/powerbi/toolkit.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/powerbi/toolkit.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/slack/toolkit.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/slack/toolkit.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/spark_sql/base.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/spark_sql/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/spark_sql/prompt.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/spark_sql/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/spark_sql/toolkit.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/spark_sql/toolkit.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/sql/base.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/sql/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/sql/prompt.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/sql/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/sql/toolkit.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/sql/toolkit.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/steam/toolkit.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/steam/toolkit.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/xorbits/__init__.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/xorbits/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/agent_toolkits/zapier/toolkit.py` & `gigachain_community-0.0.6.1/langchain_community/agent_toolkits/zapier/toolkit.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/cache.py` & `gigachain_community-0.0.6.1/langchain_community/cache.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/callbacks/__init__.py` & `gigachain_community-0.0.6.1/langchain_community/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/callbacks/aim_callback.py` & `gigachain_community-0.0.6.1/langchain_community/callbacks/aim_callback.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/callbacks/argilla_callback.py` & `gigachain_community-0.0.6.1/langchain_community/callbacks/argilla_callback.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/callbacks/arize_callback.py` & `gigachain_community-0.0.6.1/langchain_community/callbacks/arize_callback.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/callbacks/arthur_callback.py` & `gigachain_community-0.0.6.1/langchain_community/callbacks/arthur_callback.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/callbacks/clearml_callback.py` & `gigachain_community-0.0.6.1/langchain_community/callbacks/clearml_callback.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/callbacks/comet_ml_callback.py` & `gigachain_community-0.0.6.1/langchain_community/callbacks/comet_ml_callback.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/callbacks/confident_callback.py` & `gigachain_community-0.0.6.1/langchain_community/callbacks/confident_callback.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/callbacks/context_callback.py` & `gigachain_community-0.0.6.1/langchain_community/callbacks/context_callback.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/callbacks/flyte_callback.py` & `gigachain_community-0.0.6.1/langchain_community/callbacks/flyte_callback.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/callbacks/human.py` & `gigachain_community-0.0.6.1/langchain_community/callbacks/human.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/callbacks/infino_callback.py` & `gigachain_community-0.0.6.1/langchain_community/callbacks/infino_callback.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/callbacks/labelstudio_callback.py` & `gigachain_community-0.0.6.1/langchain_community/callbacks/labelstudio_callback.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/callbacks/llmonitor_callback.py` & `gigachain_community-0.0.6.1/langchain_community/callbacks/llmonitor_callback.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/callbacks/manager.py` & `gigachain_community-0.0.6.1/langchain_community/callbacks/manager.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/callbacks/mlflow_callback.py` & `gigachain_community-0.0.6.1/langchain_community/callbacks/mlflow_callback.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/callbacks/openai_info.py` & `gigachain_community-0.0.6.1/langchain_community/callbacks/openai_info.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/callbacks/promptlayer_callback.py` & `gigachain_community-0.0.6.1/langchain_community/callbacks/promptlayer_callback.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/callbacks/sagemaker_callback.py` & `gigachain_community-0.0.6.1/langchain_community/callbacks/sagemaker_callback.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/callbacks/streamlit/__init__.py` & `gigachain_community-0.0.6.1/langchain_community/callbacks/streamlit/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/callbacks/streamlit/mutable_expander.py` & `gigachain_community-0.0.6.1/langchain_community/callbacks/streamlit/mutable_expander.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/callbacks/streamlit/streamlit_callback_handler.py` & `gigachain_community-0.0.6.1/langchain_community/callbacks/streamlit/streamlit_callback_handler.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/callbacks/tracers/comet.py` & `gigachain_community-0.0.6.1/langchain_community/callbacks/tracers/comet.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/callbacks/tracers/wandb.py` & `gigachain_community-0.0.6.1/langchain_community/callbacks/tracers/wandb.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/callbacks/trubrics_callback.py` & `gigachain_community-0.0.6.1/langchain_community/callbacks/trubrics_callback.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/callbacks/utils.py` & `gigachain_community-0.0.6.1/langchain_community/callbacks/utils.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/callbacks/wandb_callback.py` & `gigachain_community-0.0.6.1/langchain_community/callbacks/wandb_callback.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/callbacks/whylabs_callback.py` & `gigachain_community-0.0.6.1/langchain_community/callbacks/whylabs_callback.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_loaders/facebook_messenger.py` & `gigachain_community-0.0.6.1/langchain_community/chat_loaders/facebook_messenger.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_loaders/gmail.py` & `gigachain_community-0.0.6.1/langchain_community/chat_loaders/gmail.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_loaders/imessage.py` & `gigachain_community-0.0.6.1/langchain_community/chat_loaders/imessage.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_loaders/langsmith.py` & `gigachain_community-0.0.6.1/langchain_community/chat_loaders/langsmith.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_loaders/slack.py` & `gigachain_community-0.0.6.1/langchain_community/chat_loaders/slack.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_loaders/telegram.py` & `gigachain_community-0.0.6.1/langchain_community/chat_loaders/telegram.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_loaders/utils.py` & `gigachain_community-0.0.6.1/langchain_community/chat_loaders/utils.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_loaders/whatsapp.py` & `gigachain_community-0.0.6.1/langchain_community/chat_loaders/whatsapp.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_message_histories/__init__.py` & `gigachain_community-0.0.6.1/langchain_community/chat_message_histories/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_message_histories/astradb.py` & `gigachain_community-0.0.6.1/langchain_community/chat_message_histories/astradb.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_message_histories/cassandra.py` & `gigachain_community-0.0.6.1/langchain_community/chat_message_histories/cassandra.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_message_histories/cosmos_db.py` & `gigachain_community-0.0.6.1/langchain_community/chat_message_histories/cosmos_db.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_message_histories/dynamodb.py` & `gigachain_community-0.0.6.1/langchain_community/chat_message_histories/dynamodb.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_message_histories/elasticsearch.py` & `gigachain_community-0.0.6.1/langchain_community/chat_message_histories/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_message_histories/file.py` & `gigachain_community-0.0.6.1/langchain_community/chat_message_histories/file.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_message_histories/firestore.py` & `gigachain_community-0.0.6.1/langchain_community/chat_message_histories/firestore.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_message_histories/in_memory.py` & `gigachain_community-0.0.6.1/langchain_community/chat_message_histories/in_memory.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_message_histories/momento.py` & `gigachain_community-0.0.6.1/langchain_community/chat_message_histories/momento.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_message_histories/mongodb.py` & `gigachain_community-0.0.6.1/langchain_community/chat_message_histories/mongodb.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_message_histories/neo4j.py` & `gigachain_community-0.0.6.1/langchain_community/chat_message_histories/neo4j.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_message_histories/postgres.py` & `gigachain_community-0.0.6.1/langchain_community/chat_message_histories/postgres.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_message_histories/redis.py` & `gigachain_community-0.0.6.1/langchain_community/chat_message_histories/redis.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_message_histories/rocksetdb.py` & `gigachain_community-0.0.6.1/langchain_community/chat_message_histories/rocksetdb.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_message_histories/singlestoredb.py` & `gigachain_community-0.0.6.1/langchain_community/chat_message_histories/singlestoredb.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_message_histories/sql.py` & `gigachain_community-0.0.6.1/langchain_community/chat_message_histories/sql.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_message_histories/streamlit.py` & `gigachain_community-0.0.6.1/langchain_community/chat_message_histories/streamlit.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_message_histories/upstash_redis.py` & `gigachain_community-0.0.6.1/langchain_community/chat_message_histories/upstash_redis.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_message_histories/xata.py` & `gigachain_community-0.0.6.1/langchain_community/chat_message_histories/xata.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_message_histories/zep.py` & `gigachain_community-0.0.6.1/langchain_community/chat_message_histories/zep.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_models/__init__.py` & `gigachain_community-0.0.6.1/langchain_community/chat_models/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_models/anthropic.py` & `gigachain_community-0.0.6.1/langchain_community/chat_models/anthropic.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_models/anyscale.py` & `gigachain_community-0.0.6.1/langchain_community/chat_models/anyscale.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_models/azure_openai.py` & `gigachain_community-0.0.6.1/langchain_community/chat_models/azure_openai.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_models/azureml_endpoint.py` & `gigachain_community-0.0.6.1/langchain_community/chat_models/azureml_endpoint.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_models/baichuan.py` & `gigachain_community-0.0.6.1/langchain_community/chat_models/baichuan.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_models/baidu_qianfan_endpoint.py` & `gigachain_community-0.0.6.1/langchain_community/chat_models/baidu_qianfan_endpoint.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_models/bedrock.py` & `gigachain_community-0.0.6.1/langchain_community/chat_models/bedrock.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_models/cohere.py` & `gigachain_community-0.0.6.1/langchain_community/chat_models/cohere.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_models/databricks.py` & `gigachain_community-0.0.6.1/langchain_community/chat_models/databricks.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_models/ernie.py` & `gigachain_community-0.0.6.1/langchain_community/chat_models/ernie.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_models/everlyai.py` & `gigachain_community-0.0.6.1/langchain_community/chat_models/everlyai.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_models/fake.py` & `gigachain_community-0.0.6.1/langchain_community/chat_models/fake.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_models/fireworks.py` & `gigachain_community-0.0.6.1/langchain_community/chat_models/fireworks.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_models/gigachat.py` & `gigachain_community-0.0.6.1/langchain_community/chat_models/gigachat.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_models/google_palm.py` & `gigachain_community-0.0.6.1/langchain_community/chat_models/google_palm.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_models/gpt_router.py` & `gigachain_community-0.0.6.1/langchain_community/chat_models/gpt_router.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_models/huggingface.py` & `gigachain_community-0.0.6.1/langchain_community/chat_models/huggingface.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_models/human.py` & `gigachain_community-0.0.6.1/langchain_community/chat_models/human.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_models/hunyuan.py` & `gigachain_community-0.0.6.1/langchain_community/chat_models/hunyuan.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_models/javelin_ai_gateway.py` & `gigachain_community-0.0.6.1/langchain_community/chat_models/javelin_ai_gateway.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_models/jinachat.py` & `gigachain_community-0.0.6.1/langchain_community/chat_models/jinachat.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_models/konko.py` & `gigachain_community-0.0.6.1/langchain_community/chat_models/konko.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_models/litellm.py` & `gigachain_community-0.0.6.1/langchain_community/chat_models/litellm.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_models/meta.py` & `gigachain_community-0.0.6.1/langchain_community/chat_models/meta.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_models/minimax.py` & `gigachain_community-0.0.6.1/langchain_community/chat_models/minimax.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_models/mlflow.py` & `gigachain_community-0.0.6.1/langchain_community/chat_models/mlflow.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_models/mlflow_ai_gateway.py` & `gigachain_community-0.0.6.1/langchain_community/chat_models/mlflow_ai_gateway.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_models/ollama.py` & `gigachain_community-0.0.6.1/langchain_community/chat_models/ollama.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_models/openai.py` & `gigachain_community-0.0.6.1/langchain_community/chat_models/openai.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_models/pai_eas_endpoint.py` & `gigachain_community-0.0.6.1/langchain_community/chat_models/pai_eas_endpoint.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_models/promptlayer_openai.py` & `gigachain_community-0.0.6.1/langchain_community/chat_models/promptlayer_openai.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_models/tongyi.py` & `gigachain_community-0.0.6.1/langchain_community/chat_models/tongyi.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_models/vertexai.py` & `gigachain_community-0.0.6.1/langchain_community/chat_models/vertexai.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_models/volcengine_maas.py` & `gigachain_community-0.0.6.1/langchain_community/chat_models/volcengine_maas.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/chat_models/yandex.py` & `gigachain_community-0.0.6.1/langchain_community/chat_models/yandex.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/docstore/__init__.py` & `gigachain_community-0.0.6.1/langchain_community/docstore/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/docstore/arbitrary_fn.py` & `gigachain_community-0.0.6.1/langchain_community/docstore/arbitrary_fn.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/docstore/base.py` & `gigachain_community-0.0.6.1/langchain_community/docstore/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/docstore/in_memory.py` & `gigachain_community-0.0.6.1/langchain_community/docstore/in_memory.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/docstore/wikipedia.py` & `gigachain_community-0.0.6.1/langchain_community/docstore/wikipedia.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/__init__.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/acreom.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/acreom.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/airbyte.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/airbyte.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/airbyte_json.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/airbyte_json.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/airtable.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/airtable.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/apify_dataset.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/apify_dataset.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/arcgis_loader.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/arcgis_loader.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/arxiv.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/arxiv.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/assemblyai.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/assemblyai.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/async_html.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/async_html.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/azlyrics.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/azlyrics.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/azure_ai_data.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/azure_ai_data.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/azure_blob_storage_container.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/azure_blob_storage_container.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/azure_blob_storage_file.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/azure_blob_storage_file.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/baiducloud_bos_directory.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/baiducloud_bos_directory.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/baiducloud_bos_file.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/baiducloud_bos_file.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/base.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/base_o365.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/base_o365.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/bibtex.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/bibtex.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/bigquery.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/bigquery.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/bilibili.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/bilibili.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/blackboard.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/blackboard.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/blob_loaders/file_system.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/blob_loaders/file_system.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/blob_loaders/schema.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/blob_loaders/schema.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/blob_loaders/youtube_audio.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/blob_loaders/youtube_audio.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/blockchain.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/blockchain.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/brave_search.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/brave_search.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/browserless.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/browserless.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/chatgpt.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/chatgpt.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/chromium.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/chromium.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/college_confidential.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/college_confidential.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/concurrent.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/concurrent.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/confluence.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/confluence.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/conllu.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/conllu.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/couchbase.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/couchbase.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/csv_loader.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/csv_loader.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/cube_semantic.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/cube_semantic.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/datadog_logs.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/datadog_logs.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/dataframe.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/dataframe.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/diffbot.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/diffbot.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/directory.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/directory.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/discord.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/discord.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/doc_intelligence.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/doc_intelligence.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/docugami.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/docugami.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/docusaurus.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/docusaurus.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/dropbox.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/dropbox.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/duckdb_loader.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/duckdb_loader.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/email.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/email.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/epub.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/epub.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/etherscan.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/etherscan.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/evernote.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/evernote.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/excel.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/excel.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/facebook_chat.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/facebook_chat.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/fauna.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/fauna.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/figma.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/figma.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/gcs_directory.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/gcs_directory.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/gcs_file.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/gcs_file.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/generic.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/generic.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/geodataframe.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/geodataframe.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/git.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/git.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/gitbook.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/gitbook.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/github.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/github.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/google_speech_to_text.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/google_speech_to_text.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/googledrive.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/googledrive.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/gutenberg.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/gutenberg.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/helpers.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/helpers.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/hn.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/hn.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/html.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/html.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/html_bs.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/html_bs.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/hugging_face_dataset.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/hugging_face_dataset.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/ifixit.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/ifixit.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/image.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/image.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/image_captions.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/image_captions.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/iugu.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/iugu.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/joplin.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/joplin.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/json_loader.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/json_loader.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/lakefs.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/lakefs.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/larksuite.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/larksuite.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/markdown.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/markdown.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/mastodon.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/mastodon.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/max_compute.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/max_compute.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/mediawikidump.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/mediawikidump.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/merge.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/merge.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/mhtml.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/mhtml.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/modern_treasury.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/modern_treasury.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/mongodb.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/mongodb.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/news.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/news.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/notebook.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/notebook.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/notion.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/notion.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/notiondb.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/notiondb.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/nuclia.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/nuclia.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/obs_directory.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/obs_directory.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/obs_file.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/obs_file.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/obsidian.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/obsidian.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/odt.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/odt.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/onedrive.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/onedrive.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/onedrive_file.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/onedrive_file.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/onenote.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/onenote.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/open_city_data.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/open_city_data.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/org_mode.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/org_mode.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/parsers/__init__.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/parsers/audio.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/parsers/audio.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/parsers/doc_intelligence.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/parsers/doc_intelligence.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/parsers/docai.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/parsers/docai.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/parsers/generic.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/parsers/generic.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/parsers/grobid.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/parsers/grobid.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/parsers/html/bs4.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/parsers/html/bs4.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/parsers/language/cobol.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/parsers/language/cobol.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/parsers/language/javascript.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/parsers/language/javascript.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/parsers/language/language_parser.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/parsers/language/language_parser.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/parsers/language/python.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/parsers/language/python.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/parsers/msword.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/parsers/msword.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/parsers/pdf.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/parsers/pdf.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/parsers/registry.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/parsers/registry.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/pdf.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/pdf.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/polars_dataframe.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/polars_dataframe.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/powerpoint.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/powerpoint.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/psychic.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/psychic.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/pubmed.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/pubmed.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/pyspark_dataframe.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/pyspark_dataframe.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/python.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/python.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/quip.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/quip.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/readthedocs.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/readthedocs.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/recursive_url_loader.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/recursive_url_loader.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/reddit.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/reddit.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/roam.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/roam.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/rocksetdb.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/rocksetdb.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/rspace.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/rspace.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/rss.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/rss.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/rst.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/rst.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/rtf.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/rtf.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/s3_directory.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/s3_directory.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/s3_file.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/s3_file.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/sharepoint.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/sharepoint.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/sitemap.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/sitemap.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/slack_directory.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/slack_directory.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/snowflake_loader.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/snowflake_loader.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/spreedly.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/spreedly.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/srt.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/srt.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/stripe.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/stripe.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/telegram.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/telegram.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/tencent_cos_directory.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/tencent_cos_directory.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/tencent_cos_file.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/tencent_cos_file.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/tensorflow_datasets.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/tensorflow_datasets.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/text.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/text.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/tomarkdown.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/tomarkdown.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/toml.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/toml.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/trello.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/trello.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/tsv.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/tsv.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/twitter.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/twitter.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/unstructured.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/unstructured.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/url.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/url.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/url_playwright.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/url_playwright.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/url_selenium.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/url_selenium.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/weather.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/weather.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/web_base.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/web_base.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/whatsapp_chat.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/whatsapp_chat.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/wikipedia.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/wikipedia.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/word_document.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/word_document.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/xml.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/xml.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/xorbits.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/xorbits.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_loaders/youtube.py` & `gigachain_community-0.0.6.1/langchain_community/document_loaders/youtube.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_transformers/__init__.py` & `gigachain_community-0.0.6.1/langchain_community/document_transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_transformers/beautiful_soup_transformer.py` & `gigachain_community-0.0.6.1/langchain_community/document_transformers/beautiful_soup_transformer.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_transformers/doctran_text_extract.py` & `gigachain_community-0.0.6.1/langchain_community/document_transformers/doctran_text_extract.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_transformers/doctran_text_qa.py` & `gigachain_community-0.0.6.1/langchain_community/document_transformers/doctran_text_qa.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_transformers/doctran_text_translate.py` & `gigachain_community-0.0.6.1/langchain_community/document_transformers/doctran_text_translate.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_transformers/embeddings_redundant_filter.py` & `gigachain_community-0.0.6.1/langchain_community/document_transformers/embeddings_redundant_filter.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_transformers/google_translate.py` & `gigachain_community-0.0.6.1/langchain_community/document_transformers/google_translate.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_transformers/html2text.py` & `gigachain_community-0.0.6.1/langchain_community/document_transformers/html2text.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_transformers/long_context_reorder.py` & `gigachain_community-0.0.6.1/langchain_community/document_transformers/long_context_reorder.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_transformers/nuclia_text_transform.py` & `gigachain_community-0.0.6.1/langchain_community/document_transformers/nuclia_text_transform.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_transformers/openai_functions.py` & `gigachain_community-0.0.6.1/langchain_community/document_transformers/openai_functions.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/document_transformers/xsl/html_chunks_with_headers.xslt` & `gigachain_community-0.0.6.1/langchain_community/document_transformers/xsl/html_chunks_with_headers.xslt`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/__init__.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/aleph_alpha.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/aleph_alpha.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/awa.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/awa.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/azure_openai.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/azure_openai.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/baidu_qianfan_endpoint.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/baidu_qianfan_endpoint.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/bedrock.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/bedrock.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/bookend.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/bookend.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/clarifai.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/clarifai.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/cloudflare_workersai.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/cloudflare_workersai.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/cohere.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/cohere.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/dashscope.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/dashscope.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/databricks.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/databricks.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/deepinfra.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/deepinfra.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/edenai.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/edenai.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/elasticsearch.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/embaas.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/embaas.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/ernie.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/ernie.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/fake.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/fake.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/fastembed.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/fastembed.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/google_palm.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/google_palm.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/gpt4all.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/gpt4all.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/gradient_ai.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/gradient_ai.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/huggingface.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/huggingface.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/huggingface_hub.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/huggingface_hub.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/infinity.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/infinity.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/javelin_ai_gateway.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/javelin_ai_gateway.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/jina.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/jina.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/johnsnowlabs.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/johnsnowlabs.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/llamacpp.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/llamacpp.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/llm_rails.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/llm_rails.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/localai.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/localai.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/minimax.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/minimax.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/mlflow.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/mlflow.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/mlflow_gateway.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/mlflow_gateway.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/modelscope_hub.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/modelscope_hub.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/mosaicml.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/mosaicml.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/nlpcloud.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/nlpcloud.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/octoai_embeddings.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/octoai_embeddings.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/ollama.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/ollama.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/openai.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/openai.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/sagemaker_endpoint.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/sagemaker_endpoint.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/self_hosted.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/self_hosted.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/self_hosted_hugging_face.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/self_hosted_hugging_face.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/spacy_embeddings.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/spacy_embeddings.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/tensorflow_hub.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/tensorflow_hub.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/vertexai.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/vertexai.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/voyageai.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/voyageai.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/xinference.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/xinference.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/embeddings/yandex.py` & `gigachain_community-0.0.6.1/langchain_community/embeddings/yandex.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/graphs/__init__.py` & `gigachain_community-0.0.6.1/langchain_community/graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/graphs/arangodb_graph.py` & `gigachain_community-0.0.6.1/langchain_community/graphs/arangodb_graph.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/graphs/falkordb_graph.py` & `gigachain_community-0.0.6.1/langchain_community/graphs/falkordb_graph.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/graphs/graph_document.py` & `gigachain_community-0.0.6.1/langchain_community/graphs/graph_document.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/graphs/graph_store.py` & `gigachain_community-0.0.6.1/langchain_community/graphs/graph_store.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/graphs/hugegraph.py` & `gigachain_community-0.0.6.1/langchain_community/graphs/hugegraph.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/graphs/kuzu_graph.py` & `gigachain_community-0.0.6.1/langchain_community/graphs/kuzu_graph.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/graphs/memgraph_graph.py` & `gigachain_community-0.0.6.1/langchain_community/graphs/memgraph_graph.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/graphs/nebula_graph.py` & `gigachain_community-0.0.6.1/langchain_community/graphs/nebula_graph.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/graphs/neo4j_graph.py` & `gigachain_community-0.0.6.1/langchain_community/graphs/neo4j_graph.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/graphs/neptune_graph.py` & `gigachain_community-0.0.6.1/langchain_community/graphs/neptune_graph.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/graphs/networkx_graph.py` & `gigachain_community-0.0.6.1/langchain_community/graphs/networkx_graph.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/graphs/rdf_graph.py` & `gigachain_community-0.0.6.1/langchain_community/graphs/rdf_graph.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/indexes/_sql_record_manager.py` & `gigachain_community-0.0.6.1/langchain_community/indexes/_sql_record_manager.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/indexes/base.py` & `gigachain_community-0.0.6.1/langchain_community/indexes/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/__init__.py` & `gigachain_community-0.0.6.1/langchain_community/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/ai21.py` & `gigachain_community-0.0.6.1/langchain_community/llms/ai21.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/aleph_alpha.py` & `gigachain_community-0.0.6.1/langchain_community/llms/aleph_alpha.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/amazon_api_gateway.py` & `gigachain_community-0.0.6.1/langchain_community/llms/amazon_api_gateway.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/anthropic.py` & `gigachain_community-0.0.6.1/langchain_community/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/anyscale.py` & `gigachain_community-0.0.6.1/langchain_community/llms/anyscale.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/aphrodite.py` & `gigachain_community-0.0.6.1/langchain_community/llms/aphrodite.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/arcee.py` & `gigachain_community-0.0.6.1/langchain_community/llms/arcee.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/aviary.py` & `gigachain_community-0.0.6.1/langchain_community/llms/aviary.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/azureml_endpoint.py` & `gigachain_community-0.0.6.1/langchain_community/llms/azureml_endpoint.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/baidu_qianfan_endpoint.py` & `gigachain_community-0.0.6.1/langchain_community/llms/baidu_qianfan_endpoint.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/bananadev.py` & `gigachain_community-0.0.6.1/langchain_community/llms/bananadev.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/baseten.py` & `gigachain_community-0.0.6.1/langchain_community/llms/baseten.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/beam.py` & `gigachain_community-0.0.6.1/langchain_community/llms/beam.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/bedrock.py` & `gigachain_community-0.0.6.1/langchain_community/llms/bedrock.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/bittensor.py` & `gigachain_community-0.0.6.1/langchain_community/llms/bittensor.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/cerebriumai.py` & `gigachain_community-0.0.6.1/langchain_community/llms/cerebriumai.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/chatglm.py` & `gigachain_community-0.0.6.1/langchain_community/llms/chatglm.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/clarifai.py` & `gigachain_community-0.0.6.1/langchain_community/llms/clarifai.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/cloudflare_workersai.py` & `gigachain_community-0.0.6.1/langchain_community/llms/cloudflare_workersai.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/cohere.py` & `gigachain_community-0.0.6.1/langchain_community/llms/cohere.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/ctransformers.py` & `gigachain_community-0.0.6.1/langchain_community/llms/ctransformers.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/ctranslate2.py` & `gigachain_community-0.0.6.1/langchain_community/llms/ctranslate2.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/databricks.py` & `gigachain_community-0.0.6.1/langchain_community/llms/databricks.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/deepinfra.py` & `gigachain_community-0.0.6.1/langchain_community/llms/deepinfra.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/deepsparse.py` & `gigachain_community-0.0.6.1/langchain_community/llms/deepsparse.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/edenai.py` & `gigachain_community-0.0.6.1/langchain_community/llms/edenai.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/fake.py` & `gigachain_community-0.0.6.1/langchain_community/llms/fake.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/fireworks.py` & `gigachain_community-0.0.6.1/langchain_community/llms/fireworks.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/forefrontai.py` & `gigachain_community-0.0.6.1/langchain_community/llms/forefrontai.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/gigachat.py` & `gigachain_community-0.0.6.1/langchain_community/llms/gigachat.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/google_palm.py` & `gigachain_community-0.0.6.1/langchain_community/llms/google_palm.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/gooseai.py` & `gigachain_community-0.0.6.1/langchain_community/llms/gooseai.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/gpt4all.py` & `gigachain_community-0.0.6.1/langchain_community/llms/gpt4all.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/gradient_ai.py` & `gigachain_community-0.0.6.1/langchain_community/llms/gradient_ai.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/grammars/json.gbnf` & `gigachain_community-0.0.6.1/langchain_community/llms/grammars/json.gbnf`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/huggingface_endpoint.py` & `gigachain_community-0.0.6.1/langchain_community/llms/huggingface_endpoint.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/huggingface_hub.py` & `gigachain_community-0.0.6.1/langchain_community/llms/huggingface_hub.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/huggingface_pipeline.py` & `gigachain_community-0.0.6.1/langchain_community/llms/huggingface_pipeline.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/huggingface_text_gen_inference.py` & `gigachain_community-0.0.6.1/langchain_community/llms/huggingface_text_gen_inference.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/human.py` & `gigachain_community-0.0.6.1/langchain_community/llms/human.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/javelin_ai_gateway.py` & `gigachain_community-0.0.6.1/langchain_community/llms/javelin_ai_gateway.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/koboldai.py` & `gigachain_community-0.0.6.1/langchain_community/llms/koboldai.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/llamacpp.py` & `gigachain_community-0.0.6.1/langchain_community/llms/llamacpp.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/loading.py` & `gigachain_community-0.0.6.1/langchain_community/llms/loading.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/manifest.py` & `gigachain_community-0.0.6.1/langchain_community/llms/manifest.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/minimax.py` & `gigachain_community-0.0.6.1/langchain_community/llms/minimax.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/mlflow.py` & `gigachain_community-0.0.6.1/langchain_community/llms/mlflow.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/mlflow_ai_gateway.py` & `gigachain_community-0.0.6.1/langchain_community/llms/mlflow_ai_gateway.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/modal.py` & `gigachain_community-0.0.6.1/langchain_community/llms/modal.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/mosaicml.py` & `gigachain_community-0.0.6.1/langchain_community/llms/mosaicml.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/nlpcloud.py` & `gigachain_community-0.0.6.1/langchain_community/llms/nlpcloud.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/oci_data_science_model_deployment_endpoint.py` & `gigachain_community-0.0.6.1/langchain_community/llms/oci_data_science_model_deployment_endpoint.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/octoai_endpoint.py` & `gigachain_community-0.0.6.1/langchain_community/llms/octoai_endpoint.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/ollama.py` & `gigachain_community-0.0.6.1/langchain_community/llms/ollama.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/opaqueprompts.py` & `gigachain_community-0.0.6.1/langchain_community/llms/opaqueprompts.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/openai.py` & `gigachain_community-0.0.6.1/langchain_community/llms/openai.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/openllm.py` & `gigachain_community-0.0.6.1/langchain_community/llms/openllm.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/openlm.py` & `gigachain_community-0.0.6.1/langchain_community/llms/openlm.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/pai_eas_endpoint.py` & `gigachain_community-0.0.6.1/langchain_community/llms/pai_eas_endpoint.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/petals.py` & `gigachain_community-0.0.6.1/langchain_community/llms/petals.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/pipelineai.py` & `gigachain_community-0.0.6.1/langchain_community/llms/pipelineai.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/predibase.py` & `gigachain_community-0.0.6.1/langchain_community/llms/predibase.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/predictionguard.py` & `gigachain_community-0.0.6.1/langchain_community/llms/predictionguard.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/promptlayer_openai.py` & `gigachain_community-0.0.6.1/langchain_community/llms/promptlayer_openai.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/replicate.py` & `gigachain_community-0.0.6.1/langchain_community/llms/replicate.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/rwkv.py` & `gigachain_community-0.0.6.1/langchain_community/llms/rwkv.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/sagemaker_endpoint.py` & `gigachain_community-0.0.6.1/langchain_community/llms/sagemaker_endpoint.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/self_hosted.py` & `gigachain_community-0.0.6.1/langchain_community/llms/self_hosted.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/self_hosted_hugging_face.py` & `gigachain_community-0.0.6.1/langchain_community/llms/self_hosted_hugging_face.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/stochasticai.py` & `gigachain_community-0.0.6.1/langchain_community/llms/stochasticai.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/symblai_nebula.py` & `gigachain_community-0.0.6.1/langchain_community/llms/symblai_nebula.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/textgen.py` & `gigachain_community-0.0.6.1/langchain_community/llms/textgen.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/titan_takeoff.py` & `gigachain_community-0.0.6.1/langchain_community/llms/titan_takeoff.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/titan_takeoff_pro.py` & `gigachain_community-0.0.6.1/langchain_community/llms/titan_takeoff_pro.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/together.py` & `gigachain_community-0.0.6.1/langchain_community/llms/together.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/tongyi.py` & `gigachain_community-0.0.6.1/langchain_community/llms/tongyi.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/vertexai.py` & `gigachain_community-0.0.6.1/langchain_community/llms/vertexai.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/vllm.py` & `gigachain_community-0.0.6.1/langchain_community/llms/vllm.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/volcengine_maas.py` & `gigachain_community-0.0.6.1/langchain_community/llms/volcengine_maas.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/watsonxllm.py` & `gigachain_community-0.0.6.1/langchain_community/llms/watsonxllm.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/writer.py` & `gigachain_community-0.0.6.1/langchain_community/llms/writer.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/xinference.py` & `gigachain_community-0.0.6.1/langchain_community/llms/xinference.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/llms/yandex.py` & `gigachain_community-0.0.6.1/langchain_community/llms/yandex.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/retrievers/__init__.py` & `gigachain_community-0.0.6.1/langchain_community/retrievers/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/retrievers/arcee.py` & `gigachain_community-0.0.6.1/langchain_community/retrievers/arcee.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/retrievers/arxiv.py` & `gigachain_community-0.0.6.1/langchain_community/retrievers/arxiv.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/retrievers/azure_cognitive_search.py` & `gigachain_community-0.0.6.1/langchain_community/retrievers/azure_cognitive_search.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/retrievers/bedrock.py` & `gigachain_community-0.0.6.1/langchain_community/retrievers/bedrock.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/retrievers/bm25.py` & `gigachain_community-0.0.6.1/langchain_community/retrievers/bm25.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/retrievers/chaindesk.py` & `gigachain_community-0.0.6.1/langchain_community/retrievers/chaindesk.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/retrievers/chatgpt_plugin_retriever.py` & `gigachain_community-0.0.6.1/langchain_community/retrievers/chatgpt_plugin_retriever.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/retrievers/cohere_rag_retriever.py` & `gigachain_community-0.0.6.1/langchain_community/retrievers/cohere_rag_retriever.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/retrievers/databerry.py` & `gigachain_community-0.0.6.1/langchain_community/retrievers/databerry.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/retrievers/docarray.py` & `gigachain_community-0.0.6.1/langchain_community/retrievers/docarray.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/retrievers/elastic_search_bm25.py` & `gigachain_community-0.0.6.1/langchain_community/retrievers/elastic_search_bm25.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/retrievers/embedchain.py` & `gigachain_community-0.0.6.1/langchain_community/retrievers/embedchain.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/retrievers/google_cloud_documentai_warehouse.py` & `gigachain_community-0.0.6.1/langchain_community/retrievers/google_cloud_documentai_warehouse.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/retrievers/google_vertex_ai_search.py` & `gigachain_community-0.0.6.1/langchain_community/retrievers/google_vertex_ai_search.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/retrievers/kay.py` & `gigachain_community-0.0.6.1/langchain_community/retrievers/kay.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/retrievers/kendra.py` & `gigachain_community-0.0.6.1/langchain_community/retrievers/kendra.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/retrievers/knn.py` & `gigachain_community-0.0.6.1/langchain_community/retrievers/knn.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/retrievers/llama_index.py` & `gigachain_community-0.0.6.1/langchain_community/retrievers/llama_index.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/retrievers/metal.py` & `gigachain_community-0.0.6.1/langchain_community/retrievers/metal.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/retrievers/milvus.py` & `gigachain_community-0.0.6.1/langchain_community/retrievers/milvus.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/retrievers/outline.py` & `gigachain_community-0.0.6.1/langchain_community/retrievers/outline.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/retrievers/pinecone_hybrid_search.py` & `gigachain_community-0.0.6.1/langchain_community/retrievers/pinecone_hybrid_search.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/retrievers/pubmed.py` & `gigachain_community-0.0.6.1/langchain_community/retrievers/pubmed.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/retrievers/qdrant_sparse_vector_retriever.py` & `gigachain_community-0.0.6.1/langchain_community/retrievers/qdrant_sparse_vector_retriever.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/retrievers/remote_retriever.py` & `gigachain_community-0.0.6.1/langchain_community/retrievers/remote_retriever.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/retrievers/svm.py` & `gigachain_community-0.0.6.1/langchain_community/retrievers/svm.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/retrievers/tavily_search_api.py` & `gigachain_community-0.0.6.1/langchain_community/retrievers/tavily_search_api.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/retrievers/tfidf.py` & `gigachain_community-0.0.6.1/langchain_community/retrievers/tfidf.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/retrievers/vespa_retriever.py` & `gigachain_community-0.0.6.1/langchain_community/retrievers/vespa_retriever.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/retrievers/weaviate_hybrid_search.py` & `gigachain_community-0.0.6.1/langchain_community/retrievers/weaviate_hybrid_search.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/retrievers/wikipedia.py` & `gigachain_community-0.0.6.1/langchain_community/retrievers/wikipedia.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/retrievers/you.py` & `gigachain_community-0.0.6.1/langchain_community/retrievers/you.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/retrievers/zep.py` & `gigachain_community-0.0.6.1/langchain_community/retrievers/zep.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/retrievers/zilliz.py` & `gigachain_community-0.0.6.1/langchain_community/retrievers/zilliz.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/storage/redis.py` & `gigachain_community-0.0.6.1/langchain_community/storage/redis.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/storage/upstash_redis.py` & `gigachain_community-0.0.6.1/langchain_community/storage/upstash_redis.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/__init__.py` & `gigachain_community-0.0.6.1/langchain_community/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/ainetwork/app.py` & `gigachain_community-0.0.6.1/langchain_community/tools/ainetwork/app.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/ainetwork/base.py` & `gigachain_community-0.0.6.1/langchain_community/tools/ainetwork/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/ainetwork/owner.py` & `gigachain_community-0.0.6.1/langchain_community/tools/ainetwork/owner.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/ainetwork/rule.py` & `gigachain_community-0.0.6.1/langchain_community/tools/ainetwork/rule.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/ainetwork/transfer.py` & `gigachain_community-0.0.6.1/langchain_community/tools/ainetwork/transfer.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/ainetwork/utils.py` & `gigachain_community-0.0.6.1/langchain_community/tools/ainetwork/utils.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/ainetwork/value.py` & `gigachain_community-0.0.6.1/langchain_community/tools/ainetwork/value.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/amadeus/closest_airport.py` & `gigachain_community-0.0.6.1/langchain_community/tools/amadeus/closest_airport.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/amadeus/flight_search.py` & `gigachain_community-0.0.6.1/langchain_community/tools/amadeus/flight_search.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/amadeus/utils.py` & `gigachain_community-0.0.6.1/langchain_community/tools/amadeus/utils.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/arxiv/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/arxiv/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/azure_cognitive_services/__init__.py` & `gigachain_community-0.0.6.1/langchain_community/tools/azure_cognitive_services/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/azure_cognitive_services/form_recognizer.py` & `gigachain_community-0.0.6.1/langchain_community/tools/azure_cognitive_services/form_recognizer.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/azure_cognitive_services/image_analysis.py` & `gigachain_community-0.0.6.1/langchain_community/tools/azure_cognitive_services/image_analysis.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/azure_cognitive_services/speech2text.py` & `gigachain_community-0.0.6.1/langchain_community/tools/azure_cognitive_services/speech2text.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/azure_cognitive_services/text2speech.py` & `gigachain_community-0.0.6.1/langchain_community/tools/azure_cognitive_services/text2speech.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/azure_cognitive_services/text_analytics_health.py` & `gigachain_community-0.0.6.1/langchain_community/tools/azure_cognitive_services/text_analytics_health.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/azure_cognitive_services/utils.py` & `gigachain_community-0.0.6.1/langchain_community/tools/azure_cognitive_services/utils.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/bearly/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/bearly/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/bing_search/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/bing_search/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/brave_search/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/brave_search/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/clickup/prompt.py` & `gigachain_community-0.0.6.1/langchain_community/tools/clickup/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/clickup/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/clickup/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/convert_to_openai.py` & `gigachain_community-0.0.6.1/langchain_community/tools/convert_to_openai.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/dataforseo_api_search/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/dataforseo_api_search/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/ddg_search/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/ddg_search/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/e2b_data_analysis/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/e2b_data_analysis/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/e2b_data_analysis/unparse.py` & `gigachain_community-0.0.6.1/langchain_community/tools/e2b_data_analysis/unparse.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/edenai/__init__.py` & `gigachain_community-0.0.6.1/langchain_community/tools/edenai/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/edenai/audio_speech_to_text.py` & `gigachain_community-0.0.6.1/langchain_community/tools/edenai/audio_speech_to_text.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/edenai/audio_text_to_speech.py` & `gigachain_community-0.0.6.1/langchain_community/tools/edenai/audio_text_to_speech.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/edenai/edenai_base_tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/edenai/edenai_base_tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/edenai/image_explicitcontent.py` & `gigachain_community-0.0.6.1/langchain_community/tools/edenai/image_explicitcontent.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/edenai/image_objectdetection.py` & `gigachain_community-0.0.6.1/langchain_community/tools/edenai/image_objectdetection.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/edenai/ocr_identityparser.py` & `gigachain_community-0.0.6.1/langchain_community/tools/edenai/ocr_identityparser.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/edenai/ocr_invoiceparser.py` & `gigachain_community-0.0.6.1/langchain_community/tools/edenai/ocr_invoiceparser.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/edenai/text_moderation.py` & `gigachain_community-0.0.6.1/langchain_community/tools/edenai/text_moderation.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/eleven_labs/text2speech.py` & `gigachain_community-0.0.6.1/langchain_community/tools/eleven_labs/text2speech.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/file_management/__init__.py` & `gigachain_community-0.0.6.1/langchain_community/tools/file_management/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/file_management/copy.py` & `gigachain_community-0.0.6.1/langchain_community/tools/file_management/copy.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/file_management/delete.py` & `gigachain_community-0.0.6.1/langchain_community/tools/file_management/delete.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/file_management/file_search.py` & `gigachain_community-0.0.6.1/langchain_community/tools/file_management/file_search.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/file_management/list_dir.py` & `gigachain_community-0.0.6.1/langchain_community/tools/file_management/list_dir.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/file_management/move.py` & `gigachain_community-0.0.6.1/langchain_community/tools/file_management/move.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/file_management/read.py` & `gigachain_community-0.0.6.1/langchain_community/tools/file_management/read.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/file_management/utils.py` & `gigachain_community-0.0.6.1/langchain_community/tools/file_management/utils.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/file_management/write.py` & `gigachain_community-0.0.6.1/langchain_community/tools/file_management/write.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/github/prompt.py` & `gigachain_community-0.0.6.1/langchain_community/tools/github/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/github/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/github/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/gitlab/prompt.py` & `gigachain_community-0.0.6.1/langchain_community/tools/gitlab/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/gitlab/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/gitlab/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/gmail/__init__.py` & `gigachain_community-0.0.6.1/langchain_community/tools/gmail/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/gmail/base.py` & `gigachain_community-0.0.6.1/langchain_community/tools/gmail/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/gmail/create_draft.py` & `gigachain_community-0.0.6.1/langchain_community/tools/gmail/create_draft.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/gmail/get_message.py` & `gigachain_community-0.0.6.1/langchain_community/tools/gmail/get_message.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/gmail/get_thread.py` & `gigachain_community-0.0.6.1/langchain_community/tools/gmail/get_thread.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/gmail/search.py` & `gigachain_community-0.0.6.1/langchain_community/tools/gmail/search.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/gmail/send_message.py` & `gigachain_community-0.0.6.1/langchain_community/tools/gmail/send_message.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/gmail/utils.py` & `gigachain_community-0.0.6.1/langchain_community/tools/gmail/utils.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/golden_query/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/golden_query/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/google_cloud/texttospeech.py` & `gigachain_community-0.0.6.1/langchain_community/tools/google_cloud/texttospeech.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/google_finance/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/google_finance/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/google_jobs/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/google_jobs/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/google_lens/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/google_lens/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/google_places/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/google_places/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/google_scholar/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/google_scholar/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/google_search/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/google_search/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/google_serper/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/google_serper/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/google_trends/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/google_trends/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/graphql/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/graphql/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/human/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/human/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/ifttt.py` & `gigachain_community-0.0.6.1/langchain_community/tools/ifttt.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/jira/prompt.py` & `gigachain_community-0.0.6.1/langchain_community/tools/jira/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/jira/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/jira/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/json/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/json/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/memorize/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/memorize/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/merriam_webster/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/merriam_webster/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/metaphor_search/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/metaphor_search/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/multion/close_session.py` & `gigachain_community-0.0.6.1/langchain_community/tools/multion/close_session.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/multion/create_session.py` & `gigachain_community-0.0.6.1/langchain_community/tools/multion/create_session.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/multion/update_session.py` & `gigachain_community-0.0.6.1/langchain_community/tools/multion/update_session.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/nasa/prompt.py` & `gigachain_community-0.0.6.1/langchain_community/tools/nasa/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/nasa/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/nasa/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/nuclia/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/nuclia/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/office365/__init__.py` & `gigachain_community-0.0.6.1/langchain_community/tools/office365/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/office365/create_draft_message.py` & `gigachain_community-0.0.6.1/langchain_community/tools/office365/create_draft_message.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/office365/events_search.py` & `gigachain_community-0.0.6.1/langchain_community/tools/office365/events_search.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/office365/messages_search.py` & `gigachain_community-0.0.6.1/langchain_community/tools/office365/messages_search.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/office365/send_event.py` & `gigachain_community-0.0.6.1/langchain_community/tools/office365/send_event.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/office365/send_message.py` & `gigachain_community-0.0.6.1/langchain_community/tools/office365/send_message.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/office365/utils.py` & `gigachain_community-0.0.6.1/langchain_community/tools/office365/utils.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/openapi/utils/api_models.py` & `gigachain_community-0.0.6.1/langchain_community/tools/openapi/utils/api_models.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/openweathermap/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/openweathermap/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/playwright/__init__.py` & `gigachain_community-0.0.6.1/langchain_community/tools/playwright/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/playwright/base.py` & `gigachain_community-0.0.6.1/langchain_community/tools/playwright/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/playwright/click.py` & `gigachain_community-0.0.6.1/langchain_community/tools/playwright/click.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/playwright/current_page.py` & `gigachain_community-0.0.6.1/langchain_community/tools/playwright/current_page.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/playwright/extract_hyperlinks.py` & `gigachain_community-0.0.6.1/langchain_community/tools/playwright/extract_hyperlinks.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/playwright/extract_text.py` & `gigachain_community-0.0.6.1/langchain_community/tools/playwright/extract_text.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/playwright/get_elements.py` & `gigachain_community-0.0.6.1/langchain_community/tools/playwright/get_elements.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/playwright/navigate.py` & `gigachain_community-0.0.6.1/langchain_community/tools/playwright/navigate.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/playwright/navigate_back.py` & `gigachain_community-0.0.6.1/langchain_community/tools/playwright/navigate_back.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/playwright/utils.py` & `gigachain_community-0.0.6.1/langchain_community/tools/playwright/utils.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/plugin.py` & `gigachain_community-0.0.6.1/langchain_community/tools/plugin.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/powerbi/prompt.py` & `gigachain_community-0.0.6.1/langchain_community/tools/powerbi/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/powerbi/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/powerbi/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/pubmed/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/pubmed/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/reddit_search/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/reddit_search/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/render.py` & `gigachain_community-0.0.6.1/langchain_community/tools/render.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/requests/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/requests/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/scenexplain/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/scenexplain/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/searchapi/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/searchapi/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/searx_search/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/searx_search/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/shell/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/shell/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/slack/get_channel.py` & `gigachain_community-0.0.6.1/langchain_community/tools/slack/get_channel.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/slack/get_message.py` & `gigachain_community-0.0.6.1/langchain_community/tools/slack/get_message.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/slack/schedule_message.py` & `gigachain_community-0.0.6.1/langchain_community/tools/slack/schedule_message.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/slack/send_message.py` & `gigachain_community-0.0.6.1/langchain_community/tools/slack/send_message.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/slack/utils.py` & `gigachain_community-0.0.6.1/langchain_community/tools/slack/utils.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/sleep/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/sleep/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/spark_sql/prompt.py` & `gigachain_community-0.0.6.1/langchain_community/tools/spark_sql/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/spark_sql/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/spark_sql/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/sql_database/prompt.py` & `gigachain_community-0.0.6.1/langchain_community/tools/sql_database/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/sql_database/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/sql_database/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/stackexchange/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/stackexchange/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/steam/prompt.py` & `gigachain_community-0.0.6.1/langchain_community/tools/steam/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/steam/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/steam/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/steamship_image_generation/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/steamship_image_generation/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/steamship_image_generation/utils.py` & `gigachain_community-0.0.6.1/langchain_community/tools/steamship_image_generation/utils.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/tavily_search/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/tavily_search/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/vectorstore/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/vectorstore/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/wikipedia/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/wikipedia/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/wolfram_alpha/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/wolfram_alpha/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/yahoo_finance_news.py` & `gigachain_community-0.0.6.1/langchain_community/tools/yahoo_finance_news.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/youtube/search.py` & `gigachain_community-0.0.6.1/langchain_community/tools/youtube/search.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/zapier/prompt.py` & `gigachain_community-0.0.6.1/langchain_community/tools/zapier/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/tools/zapier/tool.py` & `gigachain_community-0.0.6.1/langchain_community/tools/zapier/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/__init__.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/alpha_vantage.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/alpha_vantage.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/anthropic.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/anthropic.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/apify.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/apify.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/arcee.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/arcee.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/arxiv.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/arxiv.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/awslambda.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/awslambda.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/bibtex.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/bibtex.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/bing_search.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/bing_search.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/brave_search.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/brave_search.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/clickup.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/clickup.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/dalle_image_generator.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/dalle_image_generator.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/dataforseo_api_search.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/dataforseo_api_search.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/duckduckgo_search.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/duckduckgo_search.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/github.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/github.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/gitlab.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/gitlab.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/golden_query.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/golden_query.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/google_finance.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/google_finance.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/google_jobs.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/google_jobs.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/google_lens.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/google_lens.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/google_places_api.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/google_places_api.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/google_scholar.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/google_scholar.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/google_search.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/google_search.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/google_serper.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/google_serper.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/google_trends.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/google_trends.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/graphql.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/graphql.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/jira.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/jira.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/max_compute.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/max_compute.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/merriam_webster.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/merriam_webster.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/metaphor_search.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/metaphor_search.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/nasa.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/nasa.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/opaqueprompts.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/opaqueprompts.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/openapi.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/openapi.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/openweathermap.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/openweathermap.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/outline.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/outline.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/portkey.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/portkey.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/powerbi.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/powerbi.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/pubmed.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/pubmed.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/python.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/python.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/reddit_search.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/reddit_search.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/redis.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/redis.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/requests.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/requests.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/scenexplain.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/scenexplain.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/searchapi.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/searchapi.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/searx_search.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/searx_search.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/serpapi.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/serpapi.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/spark_sql.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/spark_sql.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/sql_database.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/sql_database.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/stackexchange.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/stackexchange.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/steam.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/steam.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/tavily_search.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/tavily_search.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/tensorflow_datasets.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/tensorflow_datasets.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/twilio.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/twilio.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/vertexai.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/vertexai.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/wikipedia.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/wikipedia.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/wolfram_alpha.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/wolfram_alpha.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utilities/zapier.py` & `gigachain_community-0.0.6.1/langchain_community/utilities/zapier.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utils/math.py` & `gigachain_community-0.0.6.1/langchain_community/utils/math.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/utils/openai_functions.py` & `gigachain_community-0.0.6.1/langchain_community/utils/openai_functions.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/__init__.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/alibabacloud_opensearch.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/alibabacloud_opensearch.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/analyticdb.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/analyticdb.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/annoy.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/annoy.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/astradb.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/astradb.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/atlas.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/atlas.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/awadb.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/awadb.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/azure_cosmos_db.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/azure_cosmos_db.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/azuresearch.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/azuresearch.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/bageldb.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/bageldb.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/baiducloud_vector_search.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/baiducloud_vector_search.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/cassandra.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/cassandra.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/chroma.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/chroma.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/clarifai.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/clarifai.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/clickhouse.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/clickhouse.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/dashvector.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/dashvector.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/databricks_vector_search.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/databricks_vector_search.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/deeplake.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/deeplake.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/dingo.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/dingo.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/docarray/base.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/docarray/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/docarray/hnsw.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/docarray/hnsw.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/docarray/in_memory.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/docarray/in_memory.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/elastic_vector_search.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/elastic_vector_search.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/elasticsearch.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/epsilla.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/epsilla.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/faiss.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/faiss.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/hippo.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/hippo.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/hologres.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/hologres.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/jaguar.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/jaguar.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/lancedb.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/lancedb.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/llm_rails.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/llm_rails.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/marqo.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/marqo.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/matching_engine.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/matching_engine.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/meilisearch.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/meilisearch.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/milvus.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/milvus.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/momento_vector_index.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/momento_vector_index.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/mongodb_atlas.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/mongodb_atlas.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/myscale.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/myscale.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/neo4j_vector.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/neo4j_vector.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/nucliadb.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/nucliadb.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/opensearch_vector_search.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/opensearch_vector_search.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/pgembedding.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/pgembedding.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/pgvecto_rs.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/pgvecto_rs.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/pgvector.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/pgvector.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/pinecone.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/pinecone.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/qdrant.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/qdrant.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/redis/base.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/redis/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/redis/filters.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/redis/filters.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/redis/schema.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/redis/schema.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/rocksetdb.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/rocksetdb.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/scann.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/scann.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/semadb.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/semadb.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/singlestoredb.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/singlestoredb.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/sklearn.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/sklearn.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/sqlitevss.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/sqlitevss.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/starrocks.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/starrocks.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/supabase.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/supabase.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/surrealdb.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/surrealdb.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/tair.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/tair.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/tencentvectordb.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/tencentvectordb.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/tigris.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/tigris.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/tiledb.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/tiledb.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/timescalevector.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/timescalevector.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/typesense.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/typesense.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/usearch.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/usearch.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/utils.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/utils.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/vald.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/vald.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/vearch.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/vearch.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/vectara.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/vectara.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/vespa.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/vespa.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/weaviate.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/weaviate.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/xata.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/xata.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/yellowbrick.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/yellowbrick.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/zep.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/zep.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/langchain_community/vectorstores/zilliz.py` & `gigachain_community-0.0.6.1/langchain_community/vectorstores/zilliz.py`

 * *Files identical despite different names*

### Comparing `gigachain_community-0.0.6/pyproject.toml` & `gigachain_community-0.0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gigachain-community"
-version = "0.0.6"
+version = "0.0.6.1"
 description = "Community contributed LangChain integrations."
 authors = []
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 packages = [
     {include = "langchain_community"}
```

### Comparing `gigachain_community-0.0.6/PKG-INFO` & `gigachain_community-0.0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gigachain-community
-Version: 0.0.6
+Version: 0.0.6.1
 Summary: Community contributed LangChain integrations.
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

