# Comparing `tmp/agentscope-0.0.2.tar.gz` & `tmp/agentscope-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentscope-0.0.2.tar", last modified: Fri Mar 29 10:50:13 2024, max compression
+gzip compressed data, was "agentscope-0.0.3.tar", last modified: Wed Apr  3 10:22:54 2024, max compression
```

## Comparing `agentscope-0.0.2.tar` & `agentscope-0.0.3.tar`

### file list

```diff
@@ -1,122 +1,123 @@
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-03-29 10:50:13.168820 agentscope-0.0.2/
--rw-r--r--   0 pxc        (502) staff       (20)    20637 2024-03-27 12:19:57.000000 agentscope-0.0.2/LICENSE
--rw-r--r--   0 pxc        (502) staff       (20)    22798 2024-03-29 10:50:13.168117 agentscope-0.0.2/PKG-INFO
--rw-r--r--   0 pxc        (502) staff       (20)    18108 2024-03-29 10:49:20.000000 agentscope-0.0.2/README.md
--rw-r--r--   0 pxc        (502) staff       (20)     3589 2024-03-27 12:19:57.000000 agentscope-0.0.2/pyproject.toml
--rw-r--r--   0 pxc        (502) staff       (20)       38 2024-03-29 10:50:13.169432 agentscope-0.0.2/setup.cfg
--rw-r--r--   0 pxc        (502) staff       (20)     2869 2024-03-29 10:49:20.000000 agentscope-0.0.2/setup.py
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-03-29 10:50:13.125655 agentscope-0.0.2/src/
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-03-29 10:50:13.132107 agentscope-0.0.2/src/agentscope/
--rw-r--r--   0 pxc        (502) staff       (20)      356 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/__init__.py
--rw-r--r--   0 pxc        (502) staff       (20)     6434 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/_init.py
--rw-r--r--   0 pxc        (502) staff       (20)     2261 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/_runtime.py
--rw-r--r--   0 pxc        (502) staff       (20)       77 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/_version.py
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-03-29 10:50:13.135992 agentscope-0.0.2/src/agentscope/agents/
--rw-r--r--   0 pxc        (502) staff       (20)      572 2024-03-29 10:20:14.000000 agentscope-0.0.2/src/agentscope/agents/__init__.py
--rw-r--r--   0 pxc        (502) staff       (20)     7700 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/agents/agent.py
--rw-r--r--   0 pxc        (502) staff       (20)     3192 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/agents/dialog_agent.py
--rw-r--r--   0 pxc        (502) staff       (20)     7074 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/agents/dict_dialog_agent.py
--rw-r--r--   0 pxc        (502) staff       (20)      546 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/agents/operator.py
--rw-r--r--   0 pxc        (502) staff       (20)    10029 2024-03-29 10:20:14.000000 agentscope-0.0.2/src/agentscope/agents/react_agent.py
--rw-r--r--   0 pxc        (502) staff       (20)    19212 2024-03-29 10:20:14.000000 agentscope-0.0.2/src/agentscope/agents/rpc_agent.py
--rw-r--r--   0 pxc        (502) staff       (20)     1926 2024-03-29 10:49:20.000000 agentscope-0.0.2/src/agentscope/agents/text_to_image_agent.py
--rw-r--r--   0 pxc        (502) staff       (20)     3495 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/agents/user_agent.py
--rw-r--r--   0 pxc        (502) staff       (20)     1395 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/constants.py
--rw-r--r--   0 pxc        (502) staff       (20)     5379 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/file_manager.py
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-03-29 10:50:13.136717 agentscope-0.0.2/src/agentscope/memory/
--rw-r--r--   0 pxc        (502) staff       (20)      200 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/memory/__init__.py
--rw-r--r--   0 pxc        (502) staff       (20)     2313 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/memory/memory.py
--rw-r--r--   0 pxc        (502) staff       (20)     9381 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/memory/temporary_memory.py
--rw-r--r--   0 pxc        (502) staff       (20)    11539 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/message.py
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-03-29 10:50:13.140239 agentscope-0.0.2/src/agentscope/models/
--rw-r--r--   0 pxc        (502) staff       (20)     4834 2024-03-29 10:20:14.000000 agentscope-0.0.2/src/agentscope/models/__init__.py
--rw-r--r--   0 pxc        (502) staff       (20)     1747 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/models/config.py
--rw-r--r--   0 pxc        (502) staff       (20)    20812 2024-03-29 10:49:20.000000 agentscope-0.0.2/src/agentscope/models/dashscope_model.py
--rw-r--r--   0 pxc        (502) staff       (20)    11112 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/models/gemini_model.py
--rw-r--r--   0 pxc        (502) staff       (20)    10600 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/models/model.py
--rw-r--r--   0 pxc        (502) staff       (20)    13574 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/models/ollama_model.py
--rw-r--r--   0 pxc        (502) staff       (20)    15480 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/models/openai_model.py
--rw-r--r--   0 pxc        (502) staff       (20)     8043 2024-03-29 10:49:20.000000 agentscope-0.0.2/src/agentscope/models/post_model.py
--rw-r--r--   0 pxc        (502) staff       (20)     5007 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/msghub.py
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-03-29 10:50:13.141245 agentscope-0.0.2/src/agentscope/pipelines/
--rw-r--r--   0 pxc        (502) staff       (20)      520 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/pipelines/__init__.py
--rw-r--r--   0 pxc        (502) staff       (20)     5435 2024-03-29 10:20:14.000000 agentscope-0.0.2/src/agentscope/pipelines/functional.py
--rw-r--r--   0 pxc        (502) staff       (20)     8182 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/pipelines/pipeline.py
--rw-r--r--   0 pxc        (502) staff       (20)     6533 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/prompt.py
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-03-29 10:50:13.142404 agentscope-0.0.2/src/agentscope/rpc/
--rw-r--r--   0 pxc        (502) staff       (20)      681 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/rpc/__init__.py
--rw-r--r--   0 pxc        (502) staff       (20)     1407 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/rpc/rpc_agent_client.py
--rw-r--r--   0 pxc        (502) staff       (20)     1230 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/rpc/rpc_agent_pb2.py
--rw-r--r--   0 pxc        (502) staff       (20)     2398 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/rpc/rpc_agent_pb2_grpc.py
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-03-29 10:50:13.143362 agentscope-0.0.2/src/agentscope/service/
--rw-r--r--   0 pxc        (502) staff       (20)     1683 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/service/__init__.py
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-03-29 10:50:13.144386 agentscope-0.0.2/src/agentscope/service/execute_code/
--rw-r--r--   0 pxc        (502) staff       (20)        0 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/service/execute_code/__init__.py
--rw-r--r--   0 pxc        (502) staff       (20)    14781 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/service/execute_code/exec_python.py
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-03-29 10:50:13.147917 agentscope-0.0.2/src/agentscope/service/file/
--rw-r--r--   0 pxc        (502) staff       (20)        0 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/service/file/__init__.py
--rw-r--r--   0 pxc        (502) staff       (20)     6125 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/service/file/common.py
--rw-r--r--   0 pxc        (502) staff       (20)     2320 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/service/file/json.py
--rw-r--r--   0 pxc        (502) staff       (20)     1921 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/service/file/text.py
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-03-29 10:50:13.149053 agentscope-0.0.2/src/agentscope/service/retrieval/
--rw-r--r--   0 pxc        (502) staff       (20)        0 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/service/retrieval/__init__.py
--rw-r--r--   0 pxc        (502) staff       (20)     2908 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/service/retrieval/retrieval_from_list.py
--rw-r--r--   0 pxc        (502) staff       (20)      926 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/service/retrieval/similarity.py
--rw-r--r--   0 pxc        (502) staff       (20)     6009 2024-03-29 10:20:14.000000 agentscope-0.0.2/src/agentscope/service/service_factory.py
--rw-r--r--   0 pxc        (502) staff       (20)      911 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/service/service_response.py
--rw-r--r--   0 pxc        (502) staff       (20)      204 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/service/service_status.py
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-03-29 10:50:13.150025 agentscope-0.0.2/src/agentscope/service/sql_query/
--rw-r--r--   0 pxc        (502) staff       (20)        0 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/service/sql_query/__init__.py
--rw-r--r--   0 pxc        (502) staff       (20)     2350 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/service/sql_query/mongodb.py
--rw-r--r--   0 pxc        (502) staff       (20)     2922 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/service/sql_query/mysql.py
--rw-r--r--   0 pxc        (502) staff       (20)     2263 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/service/sql_query/sqlite.py
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-03-29 10:50:13.150480 agentscope-0.0.2/src/agentscope/service/text_processing/
--rw-r--r--   0 pxc        (502) staff       (20)        0 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/service/text_processing/__init__.py
--rw-r--r--   0 pxc        (502) staff       (20)     3177 2024-03-29 10:20:14.000000 agentscope-0.0.2/src/agentscope/service/text_processing/summarization.py
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-03-29 10:50:13.151239 agentscope-0.0.2/src/agentscope/service/web_search/
--rw-r--r--   0 pxc        (502) staff       (20)        0 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/service/web_search/__init__.py
--rw-r--r--   0 pxc        (502) staff       (20)     6711 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/service/web_search/search.py
--rw-r--r--   0 pxc        (502) staff       (20)     8694 2024-03-29 10:49:20.000000 agentscope-0.0.2/src/agentscope/service/web_search/web_digest.py
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-03-29 10:50:13.153204 agentscope-0.0.2/src/agentscope/utils/
--rw-r--r--   0 pxc        (502) staff       (20)      315 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/utils/__init__.py
--rw-r--r--   0 pxc        (502) staff       (20)     5827 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/utils/common.py
--rw-r--r--   0 pxc        (502) staff       (20)     7723 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/utils/logging_utils.py
--rw-r--r--   0 pxc        (502) staff       (20)    19513 2024-03-29 10:20:14.000000 agentscope-0.0.2/src/agentscope/utils/monitor.py
--rw-r--r--   0 pxc        (502) staff       (20)     5149 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/utils/token_utils.py
--rw-r--r--   0 pxc        (502) staff       (20)     5463 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/utils/tools.py
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-03-29 10:50:13.153721 agentscope-0.0.2/src/agentscope/web/
--rw-r--r--   0 pxc        (502) staff       (20)      116 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/web/__init__.py
--rw-r--r--   0 pxc        (502) staff       (20)     3102 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/web/_app.py
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-03-29 10:50:13.128401 agentscope-0.0.2/src/agentscope/web/static/
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-03-29 10:50:13.157817 agentscope-0.0.2/src/agentscope/web/static/css/
--rw-r--r--   0 pxc        (502) staff       (20)   155751 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/web/static/css/bootstrap.min.css
--rw-r--r--   0 pxc        (502) staff       (20)      614 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/web/static/css/colors.css
--rw-r--r--   0 pxc        (502) staff       (20)     2948 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/web/static/css/components.css
--rw-r--r--   0 pxc        (502) staff       (20)      208 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/web/static/css/fonts.css
--rw-r--r--   0 pxc        (502) staff       (20)     4807 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/web/static/css/home.css
--rw-r--r--   0 pxc        (502) staff       (20)     6675 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/web/static/css/run.css
--rw-r--r--   0 pxc        (502) staff       (20)     1129 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/web/static/css/size.css
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-03-29 10:50:13.158537 agentscope-0.0.2/src/agentscope/web/static/fonts/
--rw-r--r--   0 pxc        (502) staff       (20)    11860 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/web/static/fonts/KRYPTON.ttf
--rw-r--r--   0 pxc        (502) staff       (20)   169108 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/web/static/fonts/OSWALD.ttf
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-03-29 10:50:13.159590 agentscope-0.0.2/src/agentscope/web/static/htmls/
--rw-r--r--   0 pxc        (502) staff       (20)      368 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/web/static/htmls/agent-chat-item.html
--rw-r--r--   0 pxc        (502) staff       (20)      330 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/web/static/htmls/user-chat-item.html
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-03-29 10:50:13.162516 agentscope-0.0.2/src/agentscope/web/static/js/
--rw-r--r--   0 pxc        (502) staff       (20)   193910 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/web/static/js/bootstrap-table.min.js
--rw-r--r--   0 pxc        (502) staff       (20)   122129 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/web/static/js/bootstrap.bundle.min.js
--rw-r--r--   0 pxc        (502) staff       (20)     7162 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/web/static/js/home.js
--rw-r--r--   0 pxc        (502) staff       (20)   137490 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/web/static/js/jquery-3.3.1.min.js
--rw-r--r--   0 pxc        (502) staff       (20)     7339 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/web/static/js/run.js
--rw-r--r--   0 pxc        (502) staff       (20)   177905 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/web/static/js/socket.io.js
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-03-29 10:50:13.163718 agentscope-0.0.2/src/agentscope/web/studio/
--rw-r--r--   0 pxc        (502) staff       (20)        0 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/web/studio/__init__.py
--rw-r--r--   0 pxc        (502) staff       (20)     9329 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/web/studio/studio.py
--rw-r--r--   0 pxc        (502) staff       (20)     6073 2024-03-27 12:19:57.000000 agentscope-0.0.2/src/agentscope/web/studio/utils.py
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-03-29 10:50:13.133466 agentscope-0.0.2/src/agentscope.egg-info/
--rw-r--r--   0 pxc        (502) staff       (20)    22798 2024-03-29 10:50:13.000000 agentscope-0.0.2/src/agentscope.egg-info/PKG-INFO
--rw-r--r--   0 pxc        (502) staff       (20)     3595 2024-03-29 10:50:13.000000 agentscope-0.0.2/src/agentscope.egg-info/SOURCES.txt
--rw-r--r--   0 pxc        (502) staff       (20)        1 2024-03-29 10:50:13.000000 agentscope-0.0.2/src/agentscope.egg-info/dependency_links.txt
--rw-r--r--   0 pxc        (502) staff       (20)       67 2024-03-29 10:50:13.000000 agentscope-0.0.2/src/agentscope.egg-info/entry_points.txt
--rw-r--r--   0 pxc        (502) staff       (20)     1190 2024-03-29 10:50:13.000000 agentscope-0.0.2/src/agentscope.egg-info/requires.txt
--rw-r--r--   0 pxc        (502) staff       (20)       11 2024-03-29 10:50:13.000000 agentscope-0.0.2/src/agentscope.egg-info/top_level.txt
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.059185 agentscope-0.0.3/
+-rw-r--r--   0 pxc        (502) staff       (20)    20637 2024-03-27 12:19:57.000000 agentscope-0.0.3/LICENSE
+-rw-r--r--   0 pxc        (502) staff       (20)    22430 2024-04-03 10:22:54.058112 agentscope-0.0.3/PKG-INFO
+-rw-r--r--   0 pxc        (502) staff       (20)    17712 2024-04-03 10:07:59.000000 agentscope-0.0.3/README.md
+-rw-r--r--   0 pxc        (502) staff       (20)     3589 2024-03-27 12:19:57.000000 agentscope-0.0.3/pyproject.toml
+-rw-r--r--   0 pxc        (502) staff       (20)       38 2024-04-03 10:22:54.059276 agentscope-0.0.3/setup.cfg
+-rw-r--r--   0 pxc        (502) staff       (20)     2876 2024-04-03 10:17:20.000000 agentscope-0.0.3/setup.py
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:53.994984 agentscope-0.0.3/src/
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.003397 agentscope-0.0.3/src/agentscope/
+-rw-r--r--   0 pxc        (502) staff       (20)      356 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/__init__.py
+-rw-r--r--   0 pxc        (502) staff       (20)     6434 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/_init.py
+-rw-r--r--   0 pxc        (502) staff       (20)     2261 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/_runtime.py
+-rw-r--r--   0 pxc        (502) staff       (20)       77 2024-04-03 10:08:40.000000 agentscope-0.0.3/src/agentscope/_version.py
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.008517 agentscope-0.0.3/src/agentscope/agents/
+-rw-r--r--   0 pxc        (502) staff       (20)      572 2024-03-29 10:20:14.000000 agentscope-0.0.3/src/agentscope/agents/__init__.py
+-rw-r--r--   0 pxc        (502) staff       (20)     8263 2024-04-03 10:07:59.000000 agentscope-0.0.3/src/agentscope/agents/agent.py
+-rw-r--r--   0 pxc        (502) staff       (20)     3192 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/agents/dialog_agent.py
+-rw-r--r--   0 pxc        (502) staff       (20)     7238 2024-04-03 10:07:59.000000 agentscope-0.0.3/src/agentscope/agents/dict_dialog_agent.py
+-rw-r--r--   0 pxc        (502) staff       (20)      546 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/agents/operator.py
+-rw-r--r--   0 pxc        (502) staff       (20)    11512 2024-04-03 10:07:59.000000 agentscope-0.0.3/src/agentscope/agents/react_agent.py
+-rw-r--r--   0 pxc        (502) staff       (20)    24390 2024-04-03 10:07:59.000000 agentscope-0.0.3/src/agentscope/agents/rpc_agent.py
+-rw-r--r--   0 pxc        (502) staff       (20)     1926 2024-03-29 10:49:20.000000 agentscope-0.0.3/src/agentscope/agents/text_to_image_agent.py
+-rw-r--r--   0 pxc        (502) staff       (20)     3495 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/agents/user_agent.py
+-rw-r--r--   0 pxc        (502) staff       (20)     1395 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/constants.py
+-rw-r--r--   0 pxc        (502) staff       (20)     5379 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/file_manager.py
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.009508 agentscope-0.0.3/src/agentscope/memory/
+-rw-r--r--   0 pxc        (502) staff       (20)      200 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/memory/__init__.py
+-rw-r--r--   0 pxc        (502) staff       (20)     2313 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/memory/memory.py
+-rw-r--r--   0 pxc        (502) staff       (20)     9381 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/memory/temporary_memory.py
+-rw-r--r--   0 pxc        (502) staff       (20)    12899 2024-04-03 10:07:59.000000 agentscope-0.0.3/src/agentscope/message.py
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.013268 agentscope-0.0.3/src/agentscope/models/
+-rw-r--r--   0 pxc        (502) staff       (20)     4960 2024-04-03 10:07:59.000000 agentscope-0.0.3/src/agentscope/models/__init__.py
+-rw-r--r--   0 pxc        (502) staff       (20)     1747 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/models/config.py
+-rw-r--r--   0 pxc        (502) staff       (20)    18952 2024-04-03 10:07:59.000000 agentscope-0.0.3/src/agentscope/models/dashscope_model.py
+-rw-r--r--   0 pxc        (502) staff       (20)    11877 2024-04-03 10:07:59.000000 agentscope-0.0.3/src/agentscope/models/gemini_model.py
+-rw-r--r--   0 pxc        (502) staff       (20)     9505 2024-04-03 10:07:59.000000 agentscope-0.0.3/src/agentscope/models/model.py
+-rw-r--r--   0 pxc        (502) staff       (20)    14770 2024-04-03 10:07:59.000000 agentscope-0.0.3/src/agentscope/models/ollama_model.py
+-rw-r--r--   0 pxc        (502) staff       (20)    15637 2024-04-03 10:07:59.000000 agentscope-0.0.3/src/agentscope/models/openai_model.py
+-rw-r--r--   0 pxc        (502) staff       (20)     8299 2024-04-03 10:07:59.000000 agentscope-0.0.3/src/agentscope/models/post_model.py
+-rw-r--r--   0 pxc        (502) staff       (20)     4879 2024-04-03 10:07:59.000000 agentscope-0.0.3/src/agentscope/models/response.py
+-rw-r--r--   0 pxc        (502) staff       (20)     5007 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/msghub.py
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.014603 agentscope-0.0.3/src/agentscope/pipelines/
+-rw-r--r--   0 pxc        (502) staff       (20)      520 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/pipelines/__init__.py
+-rw-r--r--   0 pxc        (502) staff       (20)     5435 2024-03-29 10:20:14.000000 agentscope-0.0.3/src/agentscope/pipelines/functional.py
+-rw-r--r--   0 pxc        (502) staff       (20)     8182 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/pipelines/pipeline.py
+-rw-r--r--   0 pxc        (502) staff       (20)     6533 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/prompt.py
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.015995 agentscope-0.0.3/src/agentscope/rpc/
+-rw-r--r--   0 pxc        (502) staff       (20)      775 2024-04-03 10:07:59.000000 agentscope-0.0.3/src/agentscope/rpc/__init__.py
+-rw-r--r--   0 pxc        (502) staff       (20)     4150 2024-04-03 10:07:59.000000 agentscope-0.0.3/src/agentscope/rpc/rpc_agent_client.py
+-rw-r--r--   0 pxc        (502) staff       (20)     1271 2024-04-03 10:07:59.000000 agentscope-0.0.3/src/agentscope/rpc/rpc_agent_pb2.py
+-rw-r--r--   0 pxc        (502) staff       (20)     2406 2024-04-03 10:07:59.000000 agentscope-0.0.3/src/agentscope/rpc/rpc_agent_pb2_grpc.py
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.017915 agentscope-0.0.3/src/agentscope/service/
+-rw-r--r--   0 pxc        (502) staff       (20)     1683 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/service/__init__.py
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.018581 agentscope-0.0.3/src/agentscope/service/execute_code/
+-rw-r--r--   0 pxc        (502) staff       (20)        0 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/service/execute_code/__init__.py
+-rw-r--r--   0 pxc        (502) staff       (20)    14781 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/service/execute_code/exec_python.py
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.020835 agentscope-0.0.3/src/agentscope/service/file/
+-rw-r--r--   0 pxc        (502) staff       (20)        0 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/service/file/__init__.py
+-rw-r--r--   0 pxc        (502) staff       (20)     6125 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/service/file/common.py
+-rw-r--r--   0 pxc        (502) staff       (20)     2320 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/service/file/json.py
+-rw-r--r--   0 pxc        (502) staff       (20)     1921 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/service/file/text.py
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.021582 agentscope-0.0.3/src/agentscope/service/retrieval/
+-rw-r--r--   0 pxc        (502) staff       (20)        0 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/service/retrieval/__init__.py
+-rw-r--r--   0 pxc        (502) staff       (20)     2908 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/service/retrieval/retrieval_from_list.py
+-rw-r--r--   0 pxc        (502) staff       (20)      926 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/service/retrieval/similarity.py
+-rw-r--r--   0 pxc        (502) staff       (20)     6009 2024-03-29 10:20:14.000000 agentscope-0.0.3/src/agentscope/service/service_factory.py
+-rw-r--r--   0 pxc        (502) staff       (20)      911 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/service/service_response.py
+-rw-r--r--   0 pxc        (502) staff       (20)      204 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/service/service_status.py
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.022609 agentscope-0.0.3/src/agentscope/service/sql_query/
+-rw-r--r--   0 pxc        (502) staff       (20)        0 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/service/sql_query/__init__.py
+-rw-r--r--   0 pxc        (502) staff       (20)     2350 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/service/sql_query/mongodb.py
+-rw-r--r--   0 pxc        (502) staff       (20)     2922 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/service/sql_query/mysql.py
+-rw-r--r--   0 pxc        (502) staff       (20)     2263 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/service/sql_query/sqlite.py
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.023306 agentscope-0.0.3/src/agentscope/service/text_processing/
+-rw-r--r--   0 pxc        (502) staff       (20)        0 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/service/text_processing/__init__.py
+-rw-r--r--   0 pxc        (502) staff       (20)     3177 2024-03-29 10:20:14.000000 agentscope-0.0.3/src/agentscope/service/text_processing/summarization.py
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.024812 agentscope-0.0.3/src/agentscope/service/web_search/
+-rw-r--r--   0 pxc        (502) staff       (20)        0 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/service/web_search/__init__.py
+-rw-r--r--   0 pxc        (502) staff       (20)     6711 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/service/web_search/search.py
+-rw-r--r--   0 pxc        (502) staff       (20)     8694 2024-03-29 10:49:20.000000 agentscope-0.0.3/src/agentscope/service/web_search/web_digest.py
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.028085 agentscope-0.0.3/src/agentscope/utils/
+-rw-r--r--   0 pxc        (502) staff       (20)      315 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/utils/__init__.py
+-rw-r--r--   0 pxc        (502) staff       (20)     5827 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/utils/common.py
+-rw-r--r--   0 pxc        (502) staff       (20)     7795 2024-04-03 10:07:59.000000 agentscope-0.0.3/src/agentscope/utils/logging_utils.py
+-rw-r--r--   0 pxc        (502) staff       (20)    19513 2024-03-29 10:20:14.000000 agentscope-0.0.3/src/agentscope/utils/monitor.py
+-rw-r--r--   0 pxc        (502) staff       (20)     5149 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/utils/token_utils.py
+-rw-r--r--   0 pxc        (502) staff       (20)     5463 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/utils/tools.py
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.029397 agentscope-0.0.3/src/agentscope/web/
+-rw-r--r--   0 pxc        (502) staff       (20)      116 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/__init__.py
+-rw-r--r--   0 pxc        (502) staff       (20)     3102 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/_app.py
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:53.998188 agentscope-0.0.3/src/agentscope/web/static/
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.032927 agentscope-0.0.3/src/agentscope/web/static/css/
+-rw-r--r--   0 pxc        (502) staff       (20)   155751 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/static/css/bootstrap.min.css
+-rw-r--r--   0 pxc        (502) staff       (20)      614 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/static/css/colors.css
+-rw-r--r--   0 pxc        (502) staff       (20)     2948 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/static/css/components.css
+-rw-r--r--   0 pxc        (502) staff       (20)      208 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/static/css/fonts.css
+-rw-r--r--   0 pxc        (502) staff       (20)     4807 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/static/css/home.css
+-rw-r--r--   0 pxc        (502) staff       (20)     6675 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/static/css/run.css
+-rw-r--r--   0 pxc        (502) staff       (20)     1129 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/static/css/size.css
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.036516 agentscope-0.0.3/src/agentscope/web/static/fonts/
+-rw-r--r--   0 pxc        (502) staff       (20)    11860 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/static/fonts/KRYPTON.ttf
+-rw-r--r--   0 pxc        (502) staff       (20)   169108 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/static/fonts/OSWALD.ttf
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.045429 agentscope-0.0.3/src/agentscope/web/static/htmls/
+-rw-r--r--   0 pxc        (502) staff       (20)      368 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/static/htmls/agent-chat-item.html
+-rw-r--r--   0 pxc        (502) staff       (20)      330 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/static/htmls/user-chat-item.html
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.050545 agentscope-0.0.3/src/agentscope/web/static/js/
+-rw-r--r--   0 pxc        (502) staff       (20)   193910 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/static/js/bootstrap-table.min.js
+-rw-r--r--   0 pxc        (502) staff       (20)   122129 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/static/js/bootstrap.bundle.min.js
+-rw-r--r--   0 pxc        (502) staff       (20)     7162 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/static/js/home.js
+-rw-r--r--   0 pxc        (502) staff       (20)   137490 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/static/js/jquery-3.3.1.min.js
+-rw-r--r--   0 pxc        (502) staff       (20)     7339 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/static/js/run.js
+-rw-r--r--   0 pxc        (502) staff       (20)   177905 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/static/js/socket.io.js
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.053417 agentscope-0.0.3/src/agentscope/web/studio/
+-rw-r--r--   0 pxc        (502) staff       (20)        0 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/studio/__init__.py
+-rw-r--r--   0 pxc        (502) staff       (20)     9329 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/studio/studio.py
+-rw-r--r--   0 pxc        (502) staff       (20)     6073 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/studio/utils.py
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.005261 agentscope-0.0.3/src/agentscope.egg-info/
+-rw-r--r--   0 pxc        (502) staff       (20)    22430 2024-04-03 10:22:53.000000 agentscope-0.0.3/src/agentscope.egg-info/PKG-INFO
+-rw-r--r--   0 pxc        (502) staff       (20)     3629 2024-04-03 10:22:53.000000 agentscope-0.0.3/src/agentscope.egg-info/SOURCES.txt
+-rw-r--r--   0 pxc        (502) staff       (20)        1 2024-04-03 10:22:53.000000 agentscope-0.0.3/src/agentscope.egg-info/dependency_links.txt
+-rw-r--r--   0 pxc        (502) staff       (20)       67 2024-04-03 10:22:53.000000 agentscope-0.0.3/src/agentscope.egg-info/entry_points.txt
+-rw-r--r--   0 pxc        (502) staff       (20)     1218 2024-04-03 10:22:53.000000 agentscope-0.0.3/src/agentscope.egg-info/requires.txt
+-rw-r--r--   0 pxc        (502) staff       (20)       11 2024-04-03 10:22:53.000000 agentscope-0.0.3/src/agentscope.egg-info/top_level.txt
```

### Comparing `agentscope-0.0.2/LICENSE` & `agentscope-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/PKG-INFO` & `agentscope-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: agentscope
-Version: 0.0.2
+Version: 0.0.3
 Summary: AgentScope: A Flexible yet Robust Multi-Agent Platform.
 Home-page: https://github.com/modelscope/agentscope
-Download-URL: https://github.com/modelscope/agentscope/archive/v0.0.2.tar.gz
+Download-URL: https://github.com/modelscope/agentscope/archive/v0.0.3.tar.gz
 Author: SysML team of Alibaba Tongyi Lab 
 Author-email: gaodawei.gdw@alibaba-inc.com
 License: Apache License 2.0
 Keywords: deep-learning,multi agents,agents
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: docstring_parser
-Requires-Dist: loguru
+Requires-Dist: loguru==0.6.0
 Requires-Dist: tiktoken
 Requires-Dist: Pillow
 Requires-Dist: requests
 Requires-Dist: chardet
 Requires-Dist: inputimeout
 Requires-Dist: openai>=1.3.0
 Requires-Dist: numpy
@@ -30,15 +30,15 @@
 Requires-Dist: Flask-SocketIO==5.3.6
 Requires-Dist: dashscope==1.14.1
 Requires-Dist: openai>=1.3.0
 Requires-Dist: ollama>=0.1.7
 Requires-Dist: google-generativeai>=0.4.0
 Provides-Extra: distribute
 Requires-Dist: docstring_parser; extra == "distribute"
-Requires-Dist: loguru; extra == "distribute"
+Requires-Dist: loguru==0.6.0; extra == "distribute"
 Requires-Dist: tiktoken; extra == "distribute"
 Requires-Dist: Pillow; extra == "distribute"
 Requires-Dist: requests; extra == "distribute"
 Requires-Dist: chardet; extra == "distribute"
 Requires-Dist: inputimeout; extra == "distribute"
 Requires-Dist: openai>=1.3.0; extra == "distribute"
 Requires-Dist: numpy; extra == "distribute"
@@ -51,15 +51,15 @@
 Requires-Dist: google-generativeai>=0.4.0; extra == "distribute"
 Requires-Dist: grpcio==1.60.0; extra == "distribute"
 Requires-Dist: grpcio-tools==1.60.0; extra == "distribute"
 Requires-Dist: protobuf==4.25.0; extra == "distribute"
 Requires-Dist: expiringdict; extra == "distribute"
 Provides-Extra: dev
 Requires-Dist: docstring_parser; extra == "dev"
-Requires-Dist: loguru; extra == "dev"
+Requires-Dist: loguru==0.6.0; extra == "dev"
 Requires-Dist: tiktoken; extra == "dev"
 Requires-Dist: Pillow; extra == "dev"
 Requires-Dist: requests; extra == "dev"
 Requires-Dist: chardet; extra == "dev"
 Requires-Dist: inputimeout; extra == "dev"
 Requires-Dist: openai>=1.3.0; extra == "dev"
 Requires-Dist: numpy; extra == "dev"
@@ -71,15 +71,15 @@
 Requires-Dist: ollama>=0.1.7; extra == "dev"
 Requires-Dist: google-generativeai>=0.4.0; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Provides-Extra: full
 Requires-Dist: docstring_parser; extra == "full"
-Requires-Dist: loguru; extra == "full"
+Requires-Dist: loguru==0.6.0; extra == "full"
 Requires-Dist: tiktoken; extra == "full"
 Requires-Dist: Pillow; extra == "full"
 Requires-Dist: requests; extra == "full"
 Requires-Dist: chardet; extra == "full"
 Requires-Dist: inputimeout; extra == "full"
 Requires-Dist: openai>=1.3.0; extra == "full"
 Requires-Dist: numpy; extra == "full"
@@ -126,17 +126,17 @@
 [![](https://img.shields.io/badge/Contribute-Welcome-green)](https://modelscope.github.io/agentscope/tutorial/contribute.html)
 
 If you find our work helpful, please kindly
 cite [our paper](https://arxiv.org/abs/2402.14034).
 
 Welcome to join our community on
 
-| [Discord](https://discord.gg/eYMpfnkG8h)                                                                                         | DingTalk                                                                                                                          | WeChat                                                                                                                            |
-|----------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
-| <img src="https://gw.alicdn.com/imgextra/i1/O1CN01hhD1mu1Dd3BWVUvxN_!!6000000000238-2-tps-400-400.png" width="100" height="100"> | <img src="https://img.alicdn.com/imgextra/i2/O1CN01tuJ5971OmAqNg9cOw_!!6000000001747-0-tps-444-460.jpg" width="100" height="100"> | <img src="https://img.alicdn.com/imgextra/i3/O1CN01UyfWfx1CYBM3WqlBy_!!6000000000092-2-tps-400-400.png" width="100" height="100"> |
+| [Discord](https://discord.gg/eYMpfnkG8h)                                                                                         | DingTalk                                                                                                                          |
+|----------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
+| <img src="https://gw.alicdn.com/imgextra/i1/O1CN01hhD1mu1Dd3BWVUvxN_!!6000000000238-2-tps-400-400.png" width="100" height="100"> | <img src="https://img.alicdn.com/imgextra/i2/O1CN01tuJ5971OmAqNg9cOw_!!6000000001747-0-tps-444-460.jpg" width="100" height="100"> |
 
 ----
 
 ## News
 
 - ![new](https://img.alicdn.com/imgextra/i4/O1CN01kUiDtl1HVxN6G56vN_!!6000000000764-2-tps-43-19.png)
 [2024-03-19] We release **AgentScope** v0.0.2 now! In this new version,
```

### Comparing `agentscope-0.0.2/README.md` & `agentscope-0.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 [![](https://img.shields.io/badge/Contribute-Welcome-green)](https://modelscope.github.io/agentscope/tutorial/contribute.html)
 
 If you find our work helpful, please kindly
 cite [our paper](https://arxiv.org/abs/2402.14034).
 
 Welcome to join our community on
 
-| [Discord](https://discord.gg/eYMpfnkG8h)                                                                                         | DingTalk                                                                                                                          | WeChat                                                                                                                            |
-|----------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
-| <img src="https://gw.alicdn.com/imgextra/i1/O1CN01hhD1mu1Dd3BWVUvxN_!!6000000000238-2-tps-400-400.png" width="100" height="100"> | <img src="https://img.alicdn.com/imgextra/i2/O1CN01tuJ5971OmAqNg9cOw_!!6000000001747-0-tps-444-460.jpg" width="100" height="100"> | <img src="https://img.alicdn.com/imgextra/i3/O1CN01UyfWfx1CYBM3WqlBy_!!6000000000092-2-tps-400-400.png" width="100" height="100"> |
+| [Discord](https://discord.gg/eYMpfnkG8h)                                                                                         | DingTalk                                                                                                                          |
+|----------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
+| <img src="https://gw.alicdn.com/imgextra/i1/O1CN01hhD1mu1Dd3BWVUvxN_!!6000000000238-2-tps-400-400.png" width="100" height="100"> | <img src="https://img.alicdn.com/imgextra/i2/O1CN01tuJ5971OmAqNg9cOw_!!6000000001747-0-tps-444-460.jpg" width="100" height="100"> |
 
 ----
 
 ## News
 
 - ![new](https://img.alicdn.com/imgextra/i4/O1CN01kUiDtl1HVxN6G56vN_!!6000000000764-2-tps-43-19.png)
 [2024-03-19] We release **AgentScope** v0.0.2 now! In this new version,
```

### Comparing `agentscope-0.0.2/pyproject.toml` & `agentscope-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/setup.py` & `agentscope-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 test_requires = ["pytest", "pytest-cov", "pre-commit"]
 
 gradio_requires = ["gradio==4.19.1", "modelscope_studio==0.0.5"]
 
 # released requires
 minimal_requires = [
     "docstring_parser",
-    "loguru",
+    "loguru==0.6.0",
     "tiktoken",
     "Pillow",
     "requests",
     "chardet",
     "inputimeout",
     "openai>=1.3.0",
     "numpy",
```

### Comparing `agentscope-0.0.2/src/agentscope/_init.py` & `agentscope-0.0.3/src/agentscope/_init.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/_runtime.py` & `agentscope-0.0.3/src/agentscope/_runtime.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/agents/__init__.py` & `agentscope-0.0.3/src/agentscope/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/agents/agent.py` & `agentscope-0.0.3/src/agentscope/agents/agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from __future__ import annotations
 from abc import ABCMeta
 from typing import Optional
 from typing import Sequence
 from typing import Union
 from typing import Any
+import uuid
 from loguru import logger
 
 from agentscope.agents.operator import Operator
 from agentscope.models import load_model_by_config_name
 from agentscope.memory import TemporaryMemory
 
 
@@ -52,15 +53,14 @@
                 The name of the model config, which is used to load model from
                 configuration.
             use_memory (`bool`, defaults to `True`):
                 Whether the agent has memory.
             memory_config (`Optional[dict]`):
                 The config of memory.
         """
-
         self.name = name
         self.memory_config = memory_config
 
         if sys_prompt is not None:
             self.sys_prompt = sys_prompt
 
         # TODO: support to receive a ModelWrapper instance
@@ -68,18 +68,27 @@
             self.model = load_model_by_config_name(model_config_name)
 
         if use_memory:
             self.memory = TemporaryMemory(memory_config)
         else:
             self.memory = None
 
+        # The global unique id of this agent
+        self._agent_id = self.__class__.generate_agent_id()
+
         # The audience of this agent, which means if this agent generates a
         # response, it will be passed to all agents in the audience.
         self._audience = None
 
+    @classmethod
+    def generate_agent_id(cls) -> str:
+        """Generate the agent_id of this agent instance"""
+        # TODO: change cls.__name__ into a global unique agent_type
+        return f"{cls.__name__}_{uuid.uuid4().hex}"
+
     def reply(self, x: dict = None) -> dict:
         """Define the actions taken by this agent.
 
         Args:
             x (`dict`, defaults to `None`):
                 Dialog history and some environment information
 
@@ -178,32 +187,41 @@
                 )
 
     def _broadcast_to_audience(self, x: dict) -> None:
         """Broadcast the input to all audiences."""
         for agent in self._audience:
             agent.observe(x)
 
+    @property
+    def agent_id(self) -> str:
+        """The unique id of this agent.
+
+        Returns:
+            str: agent_id
+        """
+        return self._agent_id
+
     def to_dist(
         self,
         host: str = "localhost",
         port: int = None,
-        max_pool_size: int = 100,
+        max_pool_size: int = 8192,
         max_timeout_seconds: int = 1800,
         launch_server: bool = True,
         local_mode: bool = True,
         lazy_launch: bool = True,
     ) -> AgentBase:
         """Convert current agent instance into a distributed version.
 
         Args:
             host (`str`, defaults to `"localhost"`):
                 Hostname of the rpc agent server.
             port (`int`, defaults to `None`):
                 Port of the rpc agent server.
-            max_pool_size (`int`, defaults to `100`):
+            max_pool_size (`int`, defaults to `8192`):
                 Max number of task results that the server can accommodate.
             max_timeout_seconds (`int`, defaults to `1800`):
                 Timeout for task results.
             local_mode (`bool`, defaults to `True`):
                 Whether the started rpc server only listens to local
                 requests.
             lazy_launch (`bool`, defaults to `True`):
@@ -224,8 +242,9 @@
             host=host,
             port=port,
             max_pool_size=max_pool_size,
             max_timeout_seconds=max_timeout_seconds,
             launch_server=launch_server,
             local_mode=local_mode,
             lazy_launch=lazy_launch,
+            agent_id=self.agent_id,
         )
```

### Comparing `agentscope-0.0.2/src/agentscope/agents/dialog_agent.py` & `agentscope-0.0.3/src/agentscope/agents/dialog_agent.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/agents/dict_dialog_agent.py` & `agentscope-0.0.3/src/agentscope/agents/dict_dialog_agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,23 +3,28 @@
 parse the model response."""
 import json
 from typing import Any, Optional, Callable
 from loguru import logger
 
 from ..message import Msg
 from .agent import AgentBase
-from ..models.model import ModelResponse
+from ..models import ModelResponse
 from ..prompt import PromptType
 from ..utils.tools import _convert_to_str
 
 
 def parse_dict(response: ModelResponse) -> ModelResponse:
     """Parse function for DictDialogAgent"""
     try:
-        response_dict = json.loads(response.text)
+        if response.text is not None:
+            response_dict = json.loads(response.text)
+        else:
+            raise ValueError(
+                f"The text field of the response s None: {response}",
+            )
     except json.decoder.JSONDecodeError:
         # Sometimes LLM may return a response with single quotes, which is not
         # a valid JSON format. We replace single quotes with double quotes and
         # try to load it again.
         # TODO: maybe using a more robust json library to handle this case
         response_dict = json.loads(response.text.replace("'", '"'))
```

### Comparing `agentscope-0.0.2/src/agentscope/agents/operator.py` & `agentscope-0.0.3/src/agentscope/agents/operator.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/agents/react_agent.py` & `agentscope-0.0.3/src/agentscope/agents/react_agent.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,69 +4,70 @@
 https://arxiv.org/abs/2210.03629.
 """
 import json
 from typing import Tuple, List
 
 from agentscope.agents import AgentBase
 from agentscope.message import Msg
-from agentscope.models import ModelResponse
+from agentscope.models import ResponseParser, ResponseParsingError
 from agentscope.service import ServiceResponse, ServiceExecStatus
 
 
-DEFAULT_TOOL_PROMPT = """
-The following tool functions are available in the format of
+DEFAULT_TOOL_PROMPT = """The following tool functions are available in the format of
 ```
 {{index}}. {{function name}}: {{function description}}
-    {{argument name}} ({{argument type}}): {{argument description}}
+    {{argument1 name}} ({{argument type}}): {{argument description}}
+    {{argument2 name}} ({{argument type}}): {{argument description}}
     ...
 ```
 
-Tool Functions:
+## Tool Functions:
 {function_prompt}
 
-Notice:
-1. Fully understand the tool function and its arguments before using it.
-2. Only use the tool function when it's necessary.
-3. Check if the arguments you provided to the tool function is correct in type and value.
-4. You can't take some problems for granted. For example, where you are, what's the time now, etc. But you can try to use the tool function to solve the problem.
+## What You Should Do:
+1. First, analyze the current situation, and determine your goal.
+2. Then, check if your goal is already achieved. If so, try to generate a response. Otherwise, think about how to achieve it with the help of provided tool functions.
+3. Respond in the required format.
+
+## Note:
+1. Fully understand the tool functions and their arguments before using them.
+2. You should decide if you need to use the tool functions, if not then return an empty list in "function" field.
+3. Make sure the types and values of the arguments you provided to the tool functions are correct.
+4. Don't take things for granted. For example, where you are, what's the time now, etc. You can try to use the tool functions to get information.
 5. If the function execution fails, you should analyze the error and try to solve it.
 
 """  # noqa
 
 TOOL_HINT_PROMPT = """
-Generate a response in the following format:
-
-Response Format:
-You should respond in the following format, which can be loaded by `json.loads` in Python:
-{{
+## Response Format:
+You should respond with a JSON object in the following format, which can be loaded by `json.loads` in Python directly. If no tool function is used, the "function" field should be an empty list.
+{
     "thought": "what you thought",
     "speak": "what you said",
-    "function": [{{"name": "{{function name}}", "arguments": {{"{{argument name}}": {{argument_value}}, ...}}}}, ...]
-}}
-
-Taking using web_search function as an example, the response should be like this:
-{{
-    "thought": "xxx",
-    "speak": "xxx",
-    "function": [{{"name": "web_search", "arguments": {{"query": "what's the weather today?"}}}}]
-}}
-"""  # noqa
+    "function": [{"name": "{function name}", "arguments": {"{argument1 name}": xxx, "{argument2 name}": xxx}}]
+}"""  # noqa
 
 FUNCTION_RESULT_TITLE_PROMPT = """Execution Results:
 """
 
 FUNCTION_RESULT_PROMPT = """{index}. {function_name}:
     [EXECUTE STATUS]: {status}
     [EXECUTE RESULT]: {result}
 """
 
+ERROR_INFO_PROMPT = """Your response is not a JSON object, and cannot be parsed by `json.loads` in parse function:
+## Your Response:
+[YOUR RESPONSE BEGIN]
+{response}
+[YOUR RESPONSE END]
+
+## Error Information:
+{error_info}
 
-def parse_func(response: ModelResponse) -> ModelResponse:
-    """Parsing the response into a dict object."""
-    return ModelResponse(raw=json.loads(response.text))
+Analyze the reason, and re-correct your response in the correct format."""  # pylint: disable=all  # noqa
 
 
 class ReActAgent(AgentBase):
     """An agent class that implements the ReAct algorithm. More details refer
     to https://arxiv.org/abs/2210.03629.
 
     Note this is an example implementation of ReAct algorithm in AgentScope.
@@ -76,15 +77,15 @@
     """
 
     def __init__(
         self,
         name: str,
         model_config_name: str,
         tools: List[Tuple],
-        sys_prompt: str = "You're a helpful assistant.",
+        sys_prompt: str = "You're a helpful assistant. Your name is {name}.",
         max_iters: int = 10,
         verbose: bool = True,
     ) -> None:
         """Initialize the ReAct agent with the given name, model config name
         and tools.
 
         Args:
@@ -115,17 +116,19 @@
 
         func_prompt, self.func_name_mapping = self.prepare_funcs_prompt(tools)
 
         # Prepare system prompt
         tools_prompt = DEFAULT_TOOL_PROMPT.format(function_prompt=func_prompt)
 
         if sys_prompt.endswith("\n"):
-            self.sys_prompt = sys_prompt + tools_prompt
+            self.sys_prompt = sys_prompt.format(name=self.name) + tools_prompt
         else:
-            self.sys_prompt = sys_prompt + "\n" + tools_prompt
+            self.sys_prompt = (
+                sys_prompt.format(name=self.name) + "\n" + tools_prompt
+            )
 
         # Put sys prompt into memory
         self.memory.add(Msg("system", self.sys_prompt, role="system"))
 
     def reply(self, x: dict = None) -> dict:
         """The reply function that achieves the ReAct algorithm.
         The more details please refer to https://arxiv.org/abs/2210.03629"""
@@ -134,25 +137,47 @@
             self.memory.add(x)
 
         for _ in range(self.max_iters):
             # Step 1: Thought
 
             self.speak(f" ITER {_+1}, STEP 1: REASONING ".center(70, "#"))
 
-            # Generate LLM response
-            prompt = self.model.format(
-                self.memory.get_memory(),
-                Msg("system", TOOL_HINT_PROMPT, role="system"),
-            )
+            try:
+                hint_msg = Msg("system", TOOL_HINT_PROMPT, role="system")
+                self.memory.add(hint_msg)
+
+                # Generate LLM response
+                prompt = self.model.format(self.memory.get_memory())
+                res = self.model(
+                    prompt,
+                    parse_func=ResponseParser.to_dict,
+                    max_retries=1,
+                ).json
+
+            except ResponseParsingError as e:
+                # Record the wrong response from the model
+                response_msg = Msg(self.name, e.response.text, "assistant")
+                self.speak(response_msg)
+
+                # Re-correct by model itself
+                error_msg = Msg(
+                    "system",
+                    ERROR_INFO_PROMPT.format(
+                        parse_func=ResponseParser.to_dict,
+                        error_info=e.error_info,
+                        response=e.response.text,
+                    ),
+                    "system",
+                )
+                self.speak(error_msg)
+
+                self.memory.add([response_msg, error_msg])
 
-            res = self.model(
-                prompt,
-                parse_func=parse_func,
-                max_retries=3,
-            ).raw
+                # Skip acting step to re-correct the response
+                continue
 
             # Record the response in memory
             msg_thought = Msg(self.name, res, role="assistant")
 
             # To better display the response, we reformat it by json.dumps here
             self.speak(
                 Msg(self.name, json.dumps(res, indent=4), role="assistant"),
@@ -166,14 +191,15 @@
                 return msg_thought
 
             # Step 2: Action
 
             self.speak(f" ITER {_+1}, STEP 2: ACTION ".center(70, "#"))
 
             # Execute functions
+            # TODO: check the provided arguments and re-correct them if needed
             execute_results = []
             for i, func in enumerate(res["function"]):
                 # Execute the function
                 func_res = self.execute_func(i, func)
                 execute_results.append(func_res)
 
             # Prepare prompt for execution results
```

### Comparing `agentscope-0.0.2/src/agentscope/agents/rpc_agent.py` & `agentscope-0.0.3/src/agentscope/agents/rpc_agent.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,16 @@
 # -*- coding: utf-8 -*-
 """ Base class for Rpc Agent """
 
-from multiprocessing import (
-    Process,
-    Event,
-    Pipe,
-)
+from multiprocessing import Process, Event, Pipe, cpu_count
 from multiprocessing.synchronize import Event as EventClass
 import socket
 import threading
-import time
 import json
-from typing import Any
-from typing import Optional
-from typing import Union
-from typing import Type
-from typing import Sequence
-from queue import Queue
+from typing import Any, Optional, Union, Type, Sequence
 from concurrent import futures
 from loguru import logger
 
 try:
     import grpc
     from grpc import ServicerContext
 except ImportError:
@@ -69,115 +59,187 @@
 class RpcAgent(AgentBase):
     """A wrapper to extend an AgentBase into a gRPC Client."""
 
     def __init__(
         self,
         name: str,
         agent_class: Type[AgentBase],
-        agent_configs: dict,
+        agent_configs: Optional[dict] = None,
         host: str = "localhost",
         port: int = None,
-        max_pool_size: int = 100,
-        max_timeout_seconds: int = 1800,
         launch_server: bool = True,
+        max_pool_size: int = 8192,
+        max_timeout_seconds: int = 1800,
         local_mode: bool = True,
         lazy_launch: bool = True,
+        agent_id: str = None,
+        create_with_agent_configs: bool = True,
     ) -> None:
         """Initialize a RpcAgent instance.
 
         Args:
-            agent_class (`Type[AgentBase]`, defaults to `None`):
-                The AgentBase subclass encapsulated by this wrapper.
-            agent_configs (`dict`): The args used to initialize the
-                agent_class.
             name (`str`): Name of the agent.
+            agent_class (`Type[AgentBase]`):
+                The AgentBase subclass encapsulated by this wrapper.
+            agent_configs (`dict`, defaults to `None`): The args used to
+                initialize the agent_class.
             host (`str`, defaults to `"localhost"`):
                 Hostname of the rpc agent server.
             port (`int`, defaults to `None`):
                 Port of the rpc agent server.
-            max_pool_size (`int`, defaults to `100`):
+            launch_server (`bool`, defaults to `True`):
+                Whether to launch the gRPC agent server.
+            max_pool_size (`int`, defaults to `8192`):
                 Max number of task results that the server can accommodate.
             max_timeout_seconds (`int`, defaults to `1800`):
                 Timeout for task results.
             local_mode (`bool`, defaults to `True`):
-                Whether the started rpc server only listens to local
+                Whether the started gRPC server only listens to local
                 requests.
             lazy_launch (`bool`, defaults to `True`):
                 Only launch the server when the agent is called.
+            agent_id (`str`, defaults to `None`):
+                The agent id of this instance. If `None`, it will
+                be generated randomly.
+            create_with_agent_configs (`bool`, defaults to `True`):
+                Only takes effect when `agent_configs` is provided.
+                If true, create the agent instance for the agent with
+                provided `agent_configs`, otherwise uses the agent server's
+                default parameters.
         """
         super().__init__(name=name)
         self.host = host
         self.port = port
         self.server_launcher = None
         self.client = None
+        if agent_id is not None:
+            self._agent_id = agent_id
+        else:
+            self._agent_id = agent_class.generate_agent_id()
+        self.agent_class = agent_class
         if launch_server:
             self.server_launcher = RpcAgentServerLauncher(
                 agent_class=agent_class,
-                agent_args=agent_configs["args"],
-                agent_kwargs=agent_configs["kwargs"],
+                agent_args=agent_configs["args"] if agent_configs else None,
+                agent_kwargs=(
+                    agent_configs["kwargs"] if agent_configs else None
+                ),
                 host=host,
                 port=port,
                 max_pool_size=max_pool_size,
                 max_timeout_seconds=max_timeout_seconds,
                 local_mode=local_mode,
             )
             if not lazy_launch:
                 self._launch_server()
         else:
-            self.client = RpcAgentClient(host=self.host, port=self.port)
+            self.client = RpcAgentClient(
+                host=self.host,
+                port=self.port,
+                agent_id=self.agent_id,
+            )
+            self.client.create_agent(
+                agent_configs if create_with_agent_configs else None,
+            )
 
     def _launch_server(self) -> None:
         """Launch a rpc server and update the port and the client"""
         self.server_launcher.launch()
         self.port = self.server_launcher.port
-        self.client = RpcAgentClient(host=self.host, port=self.port)
+        self.client = RpcAgentClient(
+            host=self.host,
+            port=self.port,
+            agent_id=self.agent_id,
+        )
 
     def reply(self, x: dict = None) -> dict:
         if self.client is None:
             self._launch_server()
-        res_msg = self.client.call_func(
-            func_name="_call",
-            value=x.serialize() if x is not None else "",
-        )
         return PlaceholderMessage(
-            **deserialize(res_msg),  # type: ignore[arg-type]
+            name=self.name,
+            content=None,
+            client=self.client,
+            x=x,
         )
 
     def observe(self, x: Union[dict, Sequence[dict]]) -> None:
         if self.client is None:
             self._launch_server()
         self.client.call_func(
             func_name="_observe",
             value=serialize(x),  # type: ignore[arg-type]
         )
 
+    def clone_instances(
+        self,
+        num_instances: int,
+        including_self: bool = True,
+    ) -> Sequence[AgentBase]:
+        """
+        Clone a series of this instance with different agent_id and
+        return them as a list.
+
+        Args:
+            num_instances (`int`): The number of instances in the returned
+            list.
+            including_self (`bool`): Whether to include the instance calling
+            this method in the returned list.
+
+        Returns:
+            `Sequence[AgentBase]`: A list of agent instances.
+        """
+        generated_instance_number = (
+            num_instances - 1 if including_self else num_instances
+        )
+        generated_instances = []
+
+        # launch the server before clone instances
+        if self.client is None:
+            self._launch_server()
+
+        # put itself as the first element of the returned list
+        if including_self:
+            generated_instances.append(self)
+
+        # clone instances without agent server
+        for _ in range(generated_instance_number):
+            generated_instances.append(
+                RpcAgent(
+                    name=self.name,
+                    agent_class=self.agent_class,
+                    host=self.host,
+                    port=self.port,
+                    launch_server=False,
+                    create_with_agent_configs=False,
+                ),
+            )
+        return generated_instances
+
     def stop(self) -> None:
-        """Stop the RpcAgent and the launched rpc server."""
+        """Stop the RpcAgent and the rpc server."""
         if self.server_launcher is not None:
             self.server_launcher.shutdown()
 
     def __del__(self) -> None:
-        if self.server_launcher is not None:
-            self.server_launcher.shutdown()
+        self.stop()
 
 
-def setup_rcp_agent_server(
+def setup_rpc_agent_server(
     agent_class: Type[AgentBase],
     agent_args: tuple,
     agent_kwargs: dict,
     host: str,
     port: int,
     init_settings: dict = None,
     start_event: EventClass = None,
     stop_event: EventClass = None,
     pipe: int = None,
     local_mode: bool = True,
-    max_pool_size: int = 100,
+    max_pool_size: int = 8192,
     max_timeout_seconds: int = 1800,
-    max_workers: int = 4,
 ) -> None:
     """Setup gRPC server rpc agent.
 
     Args:
         agent_class (`Type[AgentBase]`):
             A subclass of AgentBase.
         agent_args (`tuple`): The args tuple used to initialize the
@@ -196,41 +258,41 @@
         stop_event (`EventClass`, defaults to `None`):
             The stop Event instance used to determine whether the child
             process has been stopped.
         pipe (`int`, defaults to `None`):
             A pipe instance used to pass the actual port of the server.
         local_mode (`bool`, defaults to `None`):
             Only listen to local requests.
-        max_pool_size (`int`, defaults to `100`):
+        max_pool_size (`int`, defaults to `8192`):
             Max number of task results that the server can accommodate.
         max_timeout_seconds (`int`, defaults to `1800`):
             Timeout for task results.
-        max_workers (`int`, defaults to `4`):
-            max worker number of grpc server.
     """
 
     if init_settings is not None:
         init_process(**init_settings)
     servicer = RpcServerSideWrapper(
-        agent_class(*agent_args, **agent_kwargs),
+        agent_class,
+        agent_args,
+        agent_kwargs,
         host=host,
         port=port,
         max_pool_size=max_pool_size,
         max_timeout_seconds=max_timeout_seconds,
     )
     while True:
         try:
             port = check_port(port)
             servicer.port = port
             logger.info(
                 f"Starting rpc server [{agent_class.__name__}] at port"
                 f" [{port}]...",
             )
             server = grpc.server(
-                futures.ThreadPoolExecutor(max_workers=max_workers),
+                futures.ThreadPoolExecutor(max_workers=cpu_count()),
             )
             add_RpcAgentServicer_to_server(servicer, server)
             if local_mode:
                 server.add_insecure_port(f"localhost:{port}")
             else:
                 server.add_insecure_port(f"0.0.0.0:{port}")
             server.start()
@@ -244,21 +306,21 @@
         f"rpc server [{agent_class.__name__}] at port [{port}] started "
         "successfully",
     )
     if start_event is not None:
         pipe.send(port)
         start_event.set()
         stop_event.wait()
+        logger.info(
+            f"Stopping rpc server [{agent_class.__name__}] at port [{port}]",
+        )
+        server.stop(1.0).wait()
     else:
         server.wait_for_termination()
     logger.info(
-        f"Stopping rpc server [{agent_class.__name__}] at port [{port}]",
-    )
-    server.stop(0)
-    logger.info(
         f"rpc server [{agent_class.__name__}] at port [{port}] stopped "
         "successfully",
     )
 
 
 def find_available_port() -> int:
     """Get an unoccupied socket port number."""
@@ -302,15 +364,15 @@
     def __init__(
         self,
         agent_class: Type[AgentBase] = None,
         agent_args: tuple = (),
         agent_kwargs: dict = None,
         host: str = "localhost",
         port: int = None,
-        max_pool_size: int = 100,
+        max_pool_size: int = 8192,
         max_timeout_seconds: int = 1800,
         local_mode: bool = False,
     ) -> None:
         """Init a rpc agent server launcher.
 
         Args:
             agent_class (`Type[AgentBase]`, defaults to `None`):
@@ -319,15 +381,15 @@
                 agent_class.
             agent_kwargs (`dict`): The args dict used to initialize the
                 agent_class.
             host (`str`, defaults to `"localhost"`):
                 Hostname of the rpc agent server.
             port (`int`, defaults to `None`):
                 Port of the rpc agent server.
-            max_pool_size (`int`, defaults to `100`):
+            max_pool_size (`int`, defaults to `8192`):
                 Max number of task results that the server can accommodate.
             max_timeout_seconds (`int`, defaults to `1800`):
                 Timeout for task results.
             local_mode (`bool`, defaults to `False`):
                 Whether the started rpc server only listens to local
                 requests.
         """
@@ -342,15 +404,15 @@
         self.server = None
         self.stop_event = None
         self.parent_con = None
 
     def _launch_in_main(self) -> None:
         """Launch gRPC server in main-process"""
         server_thread = threading.Thread(
-            target=setup_rcp_agent_server,
+            target=setup_rpc_agent_server,
             kwargs={
                 "agent_class": self.agent_class,
                 "agent_args": self.agent_args,
                 "agent_kwargs": self.agent_kwargs,
                 "host": self.host,
                 "port": self.port,
                 "max_pool_size": self.max_pool_size,
@@ -367,15 +429,15 @@
 
     def _launch_in_sub(self) -> None:
         """Launch gRPC server in sub-process."""
         self.stop_event = Event()
         self.parent_con, child_con = Pipe()
         start_event = Event()
         server_process = Process(
-            target=setup_rcp_agent_server,
+            target=setup_rpc_agent_server,
             kwargs={
                 "agent_class": self.agent_class,
                 "agent_args": self.agent_args,
                 "agent_kwargs": self.agent_kwargs,
                 "host": self.host,
                 "port": self.port,
                 "init_settings": _INIT_SETTINGS,
@@ -416,86 +478,138 @@
 
     def shutdown(self) -> None:
         """Shutdown the rpc agent server."""
         if self.server is not None:
             if self.stop_event is not None:
                 self.stop_event.set()
                 self.stop_event = None
-            self.server.join(timeout=5)
-            self.server.terminate()
+            self.server.join()
             if self.server.is_alive():
                 self.server.kill()
                 logger.info(
                     f"Rpc server [{self.agent_class.__name__}] at port"
                     f" [{self.port}] is killed.",
                 )
             self.server = None
 
 
 class RpcServerSideWrapper(RpcAgentServicer):
     """A wrapper to extend an AgentBase into a gRPC Servicer."""
 
     def __init__(
         self,
-        agent_instance: AgentBase,
+        agent_class: Type[AgentBase],
+        agent_args: tuple,
+        agent_kwargs: dict,
         host: str = "localhost",
         port: int = None,
-        max_pool_size: int = 100,
+        max_pool_size: int = 8192,
         max_timeout_seconds: int = 1800,
     ):
         """Init the service side wrapper.
 
         Args:
-            agent_instance (`AgentBase`): an instance of `AgentBase`.
+            agent_class (`Type[AgentBase]`): The AgentBase subclass
+                encapsulated by this wrapper.
+            agent_args (`tuple`): The args tuple used to initialize the
+                agent_class.
+            agent_kwargs (`dict`): The args dict used to initialize the
+                agent_class.
             host (`str`, defaults to "localhost"):
                 Hostname of the rpc agent server.
             port (`int`, defaults to `None`):
                 Port of the rpc agent server.
-            max_pool_size (`int`, defaults to `100`):
+            max_pool_size (`int`, defaults to `8192`):
                 The max number of task results that the server can
                 accommodate. Note that the oldest result will be deleted
                 after exceeding the pool size.
             max_timeout_seconds (`int`, defaults to `1800`):
                 Timeout for task results. Note that expired results will be
                 deleted.
         """
+        self.agent_class = agent_class
+        self.agent_args = agent_args
+        self.agent_kwargs = agent_kwargs
         self.host = host
         self.port = port
         self.result_pool = ExpiringDict(
             max_len=max_pool_size,
             max_age_seconds=max_timeout_seconds,
         )
-        self.task_queue = Queue()
-        self.worker_thread = threading.Thread(target=self.process_tasks)
-        self.worker_thread.start()
+        self.executor = futures.ThreadPoolExecutor(max_workers=cpu_count())
         self.task_id_lock = threading.Lock()
+        self.agent_id_lock = threading.Lock()
         self.task_id_counter = 0
-        self.agent = agent_instance
+        self.agent_pool: dict[str, AgentBase] = {}
 
     def get_task_id(self) -> int:
         """Get the auto-increment task id."""
         with self.task_id_lock:
             self.task_id_counter += 1
             return self.task_id_counter
 
+    def check_and_generate_agent(
+        self,
+        agent_id: str,
+        agent_configs: dict = None,
+    ) -> None:
+        """
+        Check whether the agent exists, and create new agent instance
+        for new agent.
+
+        Args:
+            agent_id (`str`): the agent id.
+        """
+        with self.agent_id_lock:
+            if agent_id not in self.agent_pool:
+                if agent_configs is not None:
+                    agent_instance = self.agent_class(
+                        *agent_configs["args"],
+                        **agent_configs["kwargs"],
+                    )
+                else:
+                    agent_instance = self.agent_class(
+                        *self.agent_args,
+                        **self.agent_kwargs,
+                    )
+                agent_instance._agent_id = agent_id  # pylint: disable=W0212
+                self.agent_pool[agent_id] = agent_instance
+                logger.info(f"create agent instance [{agent_id}]")
+
+    def check_and_delete_agent(self, agent_id: str) -> None:
+        """
+        Check whether the agent exists, and delete the agent instance
+        for the agent_id.
+
+        Args:
+            agent_id (`str`): the agent id.
+        """
+        with self.agent_id_lock:
+            if agent_id in self.agent_pool:
+                self.agent_pool.pop(agent_id)
+                logger.info(f"delete agent instance [{agent_id}]")
+
     def call_func(self, request: RpcMsg, _: ServicerContext) -> RpcMsg:
         """Call the specific servicer function."""
         if hasattr(self, request.target_func):
+            if request.target_func not in ["_create_agent", "_get"]:
+                self.check_and_generate_agent(request.agent_id)
             return getattr(self, request.target_func)(request)
         else:
+            # TODO: support other user defined method
             logger.error(f"Unsupported method {request.target_func}")
             return RpcMsg(
                 value=Msg(
-                    name=self.agent.name,
+                    name=self.agent_pool[request.agent_id].name,
                     content=f"Unsupported method {request.target_func}",
                     role="assistant",
                 ).serialize(),
             )
 
-    def _call(self, request: RpcMsg) -> RpcMsg:
+    def _reply(self, request: RpcMsg) -> RpcMsg:
         """Call function of RpcAgentService
 
         Args:
             request (`RpcMsg`):
                 Message containing input parameters or input parameter
                 placeholders.
 
@@ -504,22 +618,25 @@
             port and task_id
         """
         if request.value:
             msg = deserialize(request.value)
         else:
             msg = None
         task_id = self.get_task_id()
-        self.task_queue.put((task_id, msg))
+        self.result_pool[task_id] = threading.Condition()
+        self.executor.submit(
+            self.process_messages,
+            task_id,
+            request.agent_id,
+            msg,  # type: ignore[arg-type]
+        )
         return RpcMsg(
             value=Msg(
-                name=self.agent.name,
+                name=self.agent_pool[request.agent_id].name,
                 content=None,
-                role="assistant",
-                host=self.host,
-                port=self.port,
                 task_id=task_id,
             ).serialize(),
         )
 
     def _get(self, request: RpcMsg) -> RpcMsg:
         """Get function of RpcAgentService
 
@@ -530,22 +647,23 @@
                 {
                     'task_id': int
                 }
 
         Returns:
             `RpcMsg`: Concrete values of the specific message (or part of it).
         """
-        # todo: add format specification of request
         msg = json.loads(request.value)
-        # todo: implement the waiting in a more elegant way, add timeout
         while True:
-            result = self.result_pool.get(msg["task_id"], None)
-            if result is not None:
-                return RpcMsg(value=result.serialize())
-            time.sleep(0.1)
+            result = self.result_pool.get(msg["task_id"])
+            if isinstance(result, threading.Condition):
+                with result:
+                    result.wait(timeout=1)
+            else:
+                break
+        return RpcMsg(value=result.serialize())
 
     def _observe(self, request: RpcMsg) -> RpcMsg:
         """Observe function of RpcAgentService
 
         Args:
             request (`RpcMsg`):
                 The serialized input to be observed.
@@ -553,19 +671,45 @@
         Returns:
             `RpcMsg`: Empty RpcMsg.
         """
         msgs = deserialize(request.value)
         for msg in msgs:
             if isinstance(msg, PlaceholderMessage):
                 msg.update_value()
-        self.agent.observe(msgs)
+        self.agent_pool[request.agent_id].observe(msgs)
         return RpcMsg()
 
-    def process_tasks(self) -> None:
-        """Task processing thread."""
-        while True:
-            task_id, task_msg = self.task_queue.get()
-            # TODO: optimize this and avoid blocking
-            if isinstance(task_msg, PlaceholderMessage):
-                task_msg.update_value()
-            result = self.agent.reply(task_msg)
-            self.result_pool[task_id] = result
+    def _create_agent(self, request: RpcMsg) -> RpcMsg:
+        """Create a new agent instance for the agent_id.
+
+        Args:
+            request (RpcMsg): request message with a `agent_id` field.
+        """
+        self.check_and_generate_agent(
+            request.agent_id,
+            agent_configs=json.loads(request.value) if request.value else None,
+        )
+        return RpcMsg()
+
+    def _delete_agent(self, request: RpcMsg) -> RpcMsg:
+        """Delete the agent instance of the specific sesssion_id.
+
+        Args:
+            request (RpcMsg): request message with a `agent_id` field.
+        """
+        self.check_and_delete_agent(request.agent_id)
+        return RpcMsg()
+
+    def process_messages(
+        self,
+        task_id: int,
+        agent_id: str,
+        task_msg: dict = None,
+    ) -> None:
+        """Task processing."""
+        if isinstance(task_msg, PlaceholderMessage):
+            task_msg.update_value()
+        cond = self.result_pool[task_id]
+        result = self.agent_pool[agent_id].reply(task_msg)
+        self.result_pool[task_id] = result
+        with cond:
+            cond.notify_all()
```

### Comparing `agentscope-0.0.2/src/agentscope/agents/text_to_image_agent.py` & `agentscope-0.0.3/src/agentscope/agents/text_to_image_agent.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/agents/user_agent.py` & `agentscope-0.0.3/src/agentscope/agents/user_agent.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/constants.py` & `agentscope-0.0.3/src/agentscope/constants.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/file_manager.py` & `agentscope-0.0.3/src/agentscope/file_manager.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/memory/memory.py` & `agentscope-0.0.3/src/agentscope/memory/memory.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/memory/temporary_memory.py` & `agentscope-0.0.3/src/agentscope/memory/temporary_memory.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/message.py` & `agentscope-0.0.3/src/agentscope/message.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,39 +3,45 @@
 
 from typing import Any, Optional, Union, Sequence, Literal
 from uuid import uuid4
 import json
 
 from loguru import logger
 
-from .rpc import RpcAgentClient
+from .rpc import RpcAgentClient, ResponseStub, call_in_thread
 from .utils.tools import _get_timestamp
 
 
 class MessageBase(dict):
     """Base Message class, which is used to maintain information for dialog,
     memory and used to construct prompt.
     """
 
     def __init__(
         self,
         name: str,
         content: Any,
+        role: Literal["user", "system", "assistant"] = "assistant",
         url: Optional[Union[Sequence[str], str]] = None,
         timestamp: Optional[str] = None,
         **kwargs: Any,
     ) -> None:
         """Initialize the message object
 
         Args:
             name (`str`):
                 The name of who send the message. It's often used in
                 role-playing scenario to tell the name of the sender.
             content (`Any`):
                 The content of the message.
+            role (`Literal["system", "user", "assistant"]`,
+            defaults to "assistant"):
+                The role of who send the message. It can be one of the
+                `"system"`, `"user"`, or `"assistant"`. Default to
+                `"assistant"`.
             url (`Optional[Union[list[str], str]]`, defaults to None):
                 A url to file, image, video, audio or website.
             timestamp (`Optional[str]`, defaults to None):
                 The timestamp of the message, if None, it will be set to
                 current time.
             **kwargs (`Any`):
                 Other attributes of the message.
@@ -47,14 +53,15 @@
         if timestamp is None:
             self.timestamp = _get_timestamp()
         else:
             self.timestamp = timestamp
 
         self.name = name
         self.content = content
+        self.role = role
 
         if url:
             self.url = url
         else:
             self.url = None
 
         self.update(kwargs)
@@ -208,14 +215,15 @@
     """A placeholder for the return message of RpcAgent."""
 
     PLACEHOLDER_ATTRS = {
         "_host",
         "_port",
         "_client",
         "_task_id",
+        "_stub",
         "_is_placeholder",
     }
 
     LOCAL_ATTRS = {
         "name",
         "timestamp",
         *PLACEHOLDER_ATTRS,
@@ -226,14 +234,16 @@
         name: str,
         content: Any,
         url: Optional[Union[Sequence[str], str]] = None,
         timestamp: Optional[str] = None,
         host: str = None,
         port: int = None,
         task_id: int = None,
+        client: Optional[RpcAgentClient] = None,
+        x: dict = None,
         **kwargs: Any,
     ) -> None:
         """A placeholder message, records the address of the real message.
 
         Args:
             name (`str`):
                 The name of who send the message. It's often used in
@@ -255,27 +265,39 @@
             host (`str`, defaults to `None`):
                 The hostname of the rpc server where the real message is
                 located.
             port (`int`, defaults to `None`):
                 The port of the rpc server where the real message is located.
             task_id (`int`, defaults to `None`):
                 The task id of the real message in the rpc server.
+            client (`RpcAgentClient`, defaults to `None`):
+                An RpcAgentClient instance used to connect to the generator of
+                this placeholder.
+            x (`dict`, defaults to `None`):
+                Input parameters used to call rpc methods on the client.
         """
         super().__init__(
             name=name,
             content=content,
             url=url,
             timestamp=timestamp,
             **kwargs,
         )
         # placeholder indicates whether the real message is still in rpc server
         self._is_placeholder = True
-        self._host = host
-        self._port = port
-        self._task_id = task_id
+        if client is None:
+            self._stub: ResponseStub = None
+            self._host: str = host
+            self._port: int = port
+            self._task_id: int = task_id
+        else:
+            self._stub = call_in_thread(client, x, "_reply")
+            self._host = client.host
+            self._port = client.port
+            self._task_id = None
 
     def __is_local(self, key: Any) -> bool:
         return (
             key in PlaceholderMessage.LOCAL_ATTRS or not self._is_placeholder
         )
 
     def __getattr__(self, __name: str) -> Any:
@@ -305,26 +327,34 @@
     def to_str(self) -> str:
         return f"{self.name}: {self.content}"
 
     def update_value(self) -> MessageBase:
         """Get attribute values from rpc agent server immediately"""
         if self._is_placeholder:
             # retrieve real message from rpc agent server
+            self.__update_task_id()
             client = RpcAgentClient(self._host, self._port)
             result = client.call_func(
                 func_name="_get",
                 value=json.dumps({"task_id": self._task_id}),
             )
             self.update(deserialize(result))
             # the actual value has been updated, not a placeholder any more
             self._is_placeholder = False
         return self
 
+    def __update_task_id(self) -> None:
+        if self._stub is not None:
+            resp = deserialize(self._stub.get_response())
+            self._task_id = resp["task_id"]  # type: ignore[call-overload]
+            self._stub = None
+
     def serialize(self) -> str:
         if self._is_placeholder:
+            self.__update_task_id()
             return json.dumps(
                 {
                     "__type": "PlaceholderMessage",
                     "name": self.name,
                     "content": None,
                     "timestamp": self.timestamp,
                     "host": self._host,
```

### Comparing `agentscope-0.0.2/src/agentscope/models/__init__.py` & `agentscope-0.0.3/src/agentscope/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,20 @@
 """ Import modules in models package."""
 import json
 from typing import Union, Type
 
 from loguru import logger
 
 from .config import _ModelConfig
-from .model import ModelWrapperBase, ModelResponse
+from .model import ModelWrapperBase
+from .response import (
+    ModelResponse,
+    ResponseParsingError,
+    ResponseParser,
+)
 from .post_model import (
     PostAPIModelWrapperBase,
     PostAPIChatWrapper,
 )
 from .openai_model import (
     OpenAIWrapperBase,
     OpenAIChatWrapper,
@@ -32,14 +37,16 @@
     GeminiEmbeddingWrapper,
 )
 
 
 __all__ = [
     "ModelWrapperBase",
     "ModelResponse",
+    "ResponseParser",
+    "ResponseParsingError",
     "PostAPIModelWrapperBase",
     "PostAPIChatWrapper",
     "OpenAIWrapperBase",
     "OpenAIChatWrapper",
     "OpenAIDALLEWrapper",
     "OpenAIEmbeddingWrapper",
     "load_model_by_config_name",
```

### Comparing `agentscope-0.0.2/src/agentscope/models/config.py` & `agentscope-0.0.3/src/agentscope/models/config.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/models/dashscope_model.py` & `agentscope-0.0.3/src/agentscope/models/dashscope_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 """Model wrapper for DashScope models"""
 from abc import ABC
 from http import HTTPStatus
 from typing import Any, Union, List, Sequence
 from loguru import logger
 
-from ..message import Msg
-from ..utils.tools import to_openai_dict, _convert_to_str
+from ..message import MessageBase
+from ..utils.tools import _convert_to_str
 
 try:
     import dashscope
 except ModuleNotFoundError:
     dashscope = None
 
 from .model import ModelWrapperBase, ModelResponse
@@ -61,15 +61,15 @@
         self.max_length = None
 
         # Set monitor accordingly
         self._register_default_metrics()
 
     def format(
         self,
-        *args: Union[Msg, Sequence[Msg]],
+        *args: Union[MessageBase, Sequence[MessageBase]],
     ) -> Union[List[dict], str]:
         raise RuntimeError(
             f"Model Wrapper [{type(self).__name__}] doesn't "
             f"need to format the input. Please try to use the "
             f"model wrapper directly.",
         )
 
@@ -207,87 +207,15 @@
         return ModelResponse(
             text=response.output["choices"][0]["message"]["content"],
             raw=response,
         )
 
     def format(
         self,
-        *args: Union[Msg, Sequence[Msg]],
-    ) -> List:
-        """Format the messages for DashScope Chat API.
-
-        In this format function, the input messages are converted into
-        dictionaries with `role` and `content` fields. This conversation may
-        not meet the requirement that `user` and `assistant` speak
-        alternatively. This requirement can be enforced by calling
-        `preprocess_role` function..
-
-        # TODO: We will merge these two functions into one `format` function
-        soon.
-
-        The following is an example:
-
-        .. code-block:: python
-
-            prompt = model.format(
-                Msg("system", "You're a helpful assistant", role="system"),
-                Msg("Bob", "Hi, how can I help you?", role="assistant"),
-                Msg("user", "What's the date today?", role="user")
-            )
-
-        The prompt will be as follows:
-
-        .. code-block:: python
-
-            [
-                {"role": "system", "content": "You are a helpful assistant"},
-                {"role": "assistant", "content": "Hi, how can I help you"},
-                {"role": "assistant", "content": "What's the date today?"}
-            ]
-
-
-        Args:
-            *args (`Union[Msg, Sequence[Msg]]`):
-                The input arguments to be formatted, where each argument
-                should be a `Msg` object, or a list of `Msg` objects
-
-        Returns:
-            `List[dict]`:
-                The formatted messages.
-        """
-        # TODO: This function only convert agentscope msgs into qwen
-        #  messages, the re-range is executed in _preprocess_role function.
-
-        # TODO: This strategy will be replaced by a new strategy in the future.
-        prompt = []
-        for unit in args:
-            if unit is None:
-                continue
-            if isinstance(unit, Msg):
-                prompt.append(to_openai_dict(unit))
-            elif isinstance(unit, list):
-                for child_unit in unit:
-                    if isinstance(child_unit, Msg):
-                        prompt.append(to_openai_dict(child_unit))
-                    else:
-                        raise TypeError(
-                            f"The input should be a Msg object or a list "
-                            f"of Msg objects, got {type(child_unit)}.",
-                        )
-            else:
-                raise TypeError(
-                    f"The input should be a Msg object or a list "
-                    f"of Msg objects, got {type(unit)}.",
-                )
-
-        return prompt
-
-    def advanced_format(
-        self,
-        *args: Union[Msg, Sequence[Msg]],
+        *args: Union[MessageBase, Sequence[MessageBase]],
     ) -> List:
         """Format the messages for DashScope Chat API.
 
         In this format function, the input messages are formatted into a
         single system messages with format "{name}: {content}" for each
         message. Note this strategy maybe not suitable for all scenarios,
         and developers are encouraged to implement their own prompt
@@ -306,59 +234,88 @@
         The prompt will be as follows:
 
         .. code-block:: python
 
             [
                 {
                     "role": "system",
+                    "content": "You're a helpful assistant",
+                }
+                {
+                    "role": "user",
                     "content": (
-                       "system: You're a helpful assistant\\n",
-                       "Bob: Hi, how can I help you?\\n",
-                       "user: What's the date today?"
+                        "## Dialogue History\n"
+                        "Bob: Hi, how can I help you?\n"
+                        "user: What's the date today?"
                     )
                 }
             ]
 
 
         Args:
-            *args (`Union[Msg, Sequence[Msg]]`):
+            args (`Union[MessageBase, Sequence[MessageBase]]`):
                 The input arguments to be formatted, where each argument
-                should be a `Msg` object, or a list of `Msg` objects
+                should be a `Msg` object, or a list of `Msg` objects.
+                In distribution, placeholder is also allowed.
 
         Returns:
             `List[dict]`:
                 The formatted messages.
         """
         # TODO: This function only convert agentscope msgs into qwen
         #  messages, the re-range is executed in _preprocess_role function.
-        prompt = []
-        for unit in args:
-            if isinstance(unit, Msg):
-                prompt.append(f"{unit.name}: {_convert_to_str(unit.content)}")
-            elif isinstance(unit, list):
-                for child_unit in unit:
-                    if isinstance(child_unit, Msg):
-                        prompt.append(
-                            f"{child_unit.name}: "
-                            f"{_convert_to_str(child_unit.content)}",
-                        )
-                    else:
-                        raise TypeError(
-                            f"The input should be a Msg object or a list "
-                            f"of Msg objects, got {type(child_unit)}.",
-                        )
+
+        # Parse all information into a list of messages
+        input_msgs = []
+        for _ in args:
+            if isinstance(_, MessageBase):
+                input_msgs.append(_)
+            elif isinstance(_, list) and all(
+                isinstance(__, MessageBase) for __ in _
+            ):
+                input_msgs.extend(_)
             else:
                 raise TypeError(
                     f"The input should be a Msg object or a list "
-                    f"of Msg objects, got {type(unit)}.",
+                    f"of Msg objects, got {type(_)}.",
                 )
 
-        prompt_str = "\n".join(prompt)
+        messages = []
+
+        # record dialog history as a list of strings
+        dialogue = []
+        for i, unit in enumerate(input_msgs):
+            if i == 0 and unit.role == "system":
+                # system prompt
+                messages.append(
+                    {
+                        "role": unit.role,
+                        "content": _convert_to_str(unit.content),
+                    },
+                )
+            else:
+                # Merge all messages into a dialogue history prompt
+                dialogue.append(
+                    f"{unit.name}: {_convert_to_str(unit.content)}",
+                )
+
+        dialogue_history = "\n".join(dialogue)
+
+        user_content_template = "## Dialogue History\n{dialogue_history}"
+
+        messages.append(
+            {
+                "role": "user",
+                "content": user_content_template.format(
+                    dialogue_history=dialogue_history,
+                ),
+            },
+        )
 
-        return [{"role": "system", "content": prompt_str}]
+        return messages
 
     def _preprocess_role(self, messages: list) -> list:
         """preprocess role rules for DashScope"""
         # The models in this list require that the roles of messages must
         # alternate between "user" and "assistant".
         message_length = len(messages)
         if message_length % 2 == 1:
```

### Comparing `agentscope-0.0.2/src/agentscope/models/gemini_model.py` & `agentscope-0.0.3/src/agentscope/models/gemini_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 from abc import ABC
 from collections.abc import Iterable
 from typing import Sequence, Union, Any, List
 
 from loguru import logger
 
-from agentscope.message import Msg
+from agentscope.message import Msg, MessageBase
 from agentscope.models import ModelWrapperBase, ModelResponse
 from agentscope.utils.tools import _convert_to_str
 
 try:
     import google.generativeai as genai
 except ImportError:
     genai = None
@@ -193,15 +193,18 @@
             metric_unit="token",
         )
         self.monitor.register(
             self._metric("total_tokens"),
             metric_unit="token",
         )
 
-    def format(self, *args: Union[Msg, Sequence[Msg]]) -> List[dict]:
+    def format(
+        self,
+        *args: Union[MessageBase, Sequence[MessageBase]],
+    ) -> List[dict]:
         """This function provide a basic prompting strategy for Gemini Chat
         API in multi-party conversation, which combines all input into a
         single string, and wrap it into a user message.
 
         We make the above decision based on the following constraints of the
         Gemini generate API:
 
@@ -221,49 +224,75 @@
         Based on the above considerations, we decide to combine all messages
         into a single user message. This is a simple and straightforward
         strategy, if you have any better ideas, pull request and
         discussion are welcome in our GitHub repository
         https://github.com/agentscope/agentscope!
 
         Args:
-            args (`Union[Msg, Sequence[Msg]]`):
-                The items in `args` should be `Msg` objects or a list of
-                `Msg` objects.
+            args (`Union[MessageBase, Sequence[MessageBase]]`):
+                The input arguments to be formatted, where each argument
+                should be a `Msg` object, or a list of `Msg` objects.
+                In distribution, placeholder is also allowed.
 
         Returns:
             `List[dict]`:
                 A list with one user message.
         """
-        prompt = []
-        for unit in args:
-            if unit is None:
-                continue
-            if isinstance(unit, Msg):
-                prompt.append(f"{unit.name}: {_convert_to_str(unit.content)}")
-            elif isinstance(unit, list):
-                for child_unit in unit:
-                    if isinstance(child_unit, Msg):
-                        prompt.append(
-                            f"{child_unit.name}: "
-                            f"{_convert_to_str(child_unit.content)}",
-                        )
-                    else:
-                        raise TypeError(
-                            f"The input should be a Msg object or a list "
-                            f"of Msg objects, got {type(child_unit)}.",
-                        )
+        input_msgs = []
+        for _ in args:
+            if isinstance(_, MessageBase):
+                input_msgs.append(_)
+            elif isinstance(_, list) and all(
+                isinstance(__, MessageBase) for __ in _
+            ):
+                input_msgs.extend(_)
             else:
                 raise TypeError(
                     f"The input should be a Msg object or a list "
-                    f"of Msg objects, got {type(unit)}.",
+                    f"of Msg objects, got {type(_)}.",
                 )
 
-        prompt_str = "\n".join(prompt)
+        # record dialog history as a list of strings
+        sys_prompt = None
+        dialogue = []
+        for i, unit in enumerate(input_msgs):
+            if i == 0 and unit.role == "system":
+                # system prompt
+                sys_prompt = _convert_to_str(unit.content)
+            else:
+                # Merge all messages into a dialogue history prompt
+                dialogue.append(
+                    f"{unit.name}: {_convert_to_str(unit.content)}",
+                )
+
+        dialogue_history = "\n".join(dialogue)
+
+        if sys_prompt is None:
+            user_content_template = "## Dialogue History\n{dialogue_history}"
+        else:
+            user_content_template = (
+                "{sys_prompt}\n"
+                "\n"
+                "## Dialogue History\n"
+                "{dialogue_history}"
+            )
+
+        messages = [
+            {
+                "role": "user",
+                "parts": [
+                    user_content_template.format(
+                        sys_prompt=sys_prompt,
+                        dialogue_history=dialogue_history,
+                    ),
+                ],
+            },
+        ]
 
-        return [{"role": "user", "parts": [prompt_str]}]
+        return messages
 
 
 class GeminiEmbeddingWrapper(GeminiWrapperBase):
     """The wrapper for Google Gemini embedding model,
     e.g. models/embedding-001"""
 
     model_type: str = "gemini_embedding"
```

### Comparing `agentscope-0.0.2/src/agentscope/models/model.py` & `agentscope-0.0.3/src/agentscope/models/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,84 +54,29 @@
 
 """
 import inspect
 import time
 from abc import ABCMeta
 from functools import wraps
 from typing import Sequence, Any, Callable, Union, List
-import json
 
 from loguru import logger
 
 from agentscope.utils import QuotaExceededError
-
+from .response import ResponseParsingError, ModelResponse
 
 from ..file_manager import file_manager
-from ..message import Msg
+from ..message import MessageBase
 from ..utils import MonitorFactory
 from ..utils.monitor import get_full_name
-from ..utils.tools import _get_timestamp, _is_json_serializable
+from ..utils.tools import _get_timestamp
 from ..constants import _DEFAULT_MAX_RETRIES
 from ..constants import _DEFAULT_RETRY_INTERVAL
 
 
-class ModelResponse:
-    """Encapsulation of data returned by the model.
-
-    The main purpose of this class is to align the return formats of different
-    models and act as a bridge between models and agents.
-    """
-
-    def __init__(
-        self,
-        text: str = None,
-        embedding: Sequence = None,
-        image_urls: Sequence[str] = None,
-        raw: Any = None,
-    ) -> None:
-        self._text = text
-        self._embedding = embedding
-        self._image_urls = image_urls
-        self._raw = raw
-
-    @property
-    def text(self) -> str:
-        """Text field."""
-        return self._text
-
-    @property
-    def embedding(self) -> Sequence:
-        """Embedding field."""
-        return self._embedding
-
-    @property
-    def image_urls(self) -> Sequence[str]:
-        """Image URLs field."""
-        return self._image_urls
-
-    @property
-    def raw(self) -> Any:
-        """Raw response field."""
-        return self._raw
-
-    def __str__(self) -> str:
-        if _is_json_serializable(self._raw):
-            raw = self._raw
-        else:
-            raw = str(self._raw)
-
-        serialized_fields = {
-            "text": self.text,
-            "embedding": self.embedding,
-            "image_urls": self.image_urls,
-            "raw": raw,
-        }
-        return json.dumps(serialized_fields, indent=4, ensure_ascii=False)
-
-
 def _response_parse_decorator(
     model_call: Callable,
 ) -> Callable:
     """A decorator for parsing the response of model call. It will take
     `parse_func`, `fault_handler` and `max_retries` as arguments. The
     detailed process is as follows:
 
@@ -166,38 +111,40 @@
 
         # Step2: Call the model and parse the response
         # Return the response directly if parse_func is not provided
         if parse_func is None:
             return model_call(self, *args, **kwargs)
 
         # Otherwise, try to parse the response
-        response = None
         for itr in range(1, max_retries + 1):
             # Call the model
             response = model_call(self, *args, **kwargs)
 
             # Parse the response if needed
             try:
                 return parse_func(response)
             except Exception as e:
-                logger.warning(
-                    f"Fail to parsing response: "
-                    f"{response}.\n Exception: {e}, "
-                    f"\t Attempt {itr} / {max_retries}",
-                )
-                time.sleep(_DEFAULT_RETRY_INTERVAL * itr)
-
-        if fault_handler is not None and callable(fault_handler):
-            return fault_handler(response)
-        else:
-            raise ValueError(
-                f"fail to parsing response with: "
-                f"{parse_func.__name__}. \n  "
-                f"\t Attempts fails {max_retries} times",
-            )
+                if itr < max_retries:
+                    logger.warning(
+                        f"Fail to parse response ({itr}/{max_retries}):\n"
+                        f"{response}.\n"
+                        f"{e.__class__.__name__}: {e}",
+                    )
+                    time.sleep(_DEFAULT_RETRY_INTERVAL * itr)
+                else:
+                    if fault_handler is not None and callable(fault_handler):
+                        return fault_handler(response)
+                    else:
+                        error_info = f"{e.__class__.__name__}: {e}"
+                        raise ResponseParsingError(
+                            parse_func=parse_func,
+                            error_info=error_info,
+                            response=response,
+                        ) from None
+        return {}
 
     return checking_wrapper
 
 
 class _ModelWrapperMeta(ABCMeta):
     """A meta call to replace the model wrapper's __call__ function with
     wrapper about error handling."""
@@ -262,15 +209,15 @@
             f"Model Wrapper [{type(self).__name__}]"
             f" is missing the required `__call__`"
             f" method.",
         )
 
     def format(
         self,
-        *args: Union[Msg, Sequence[Msg]],
+        *args: Union[MessageBase, Sequence[MessageBase]],
     ) -> Union[List[dict], str]:
         """Format the input string or dict into the format that the model
         API required."""
         raise NotImplementedError(
             f"Model Wrapper [{type(self).__name__}]"
             f" is missing the required `format` method",
         )
```

### Comparing `agentscope-0.0.2/src/agentscope/models/ollama_model.py` & `agentscope-0.0.3/src/agentscope/models/ollama_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # -*- coding: utf-8 -*-
 """Model wrapper for Ollama models."""
 from abc import ABC
 from typing import Sequence, Any, Optional, List, Union
 
-from agentscope.message import Msg
+from loguru import logger
+
+from agentscope.message import MessageBase
 from agentscope.models import ModelWrapperBase, ModelResponse
 from agentscope.utils.tools import _convert_to_str
 
 try:
     import ollama
 except ImportError:
     ollama = None
@@ -161,33 +163,46 @@
         self.monitor.register(
             self._metric("total_tokens"),
             metric_unit="token",
         )
 
     def format(
         self,
-        *msgs: Union[Msg, Sequence[Msg]],
+        *args: Union[MessageBase, Sequence[MessageBase]],
     ) -> List[dict]:
         """A basic strategy to format the input into the required format of
         Ollama Chat API.
 
+        Note for ollama chat api, the content field shouldn't be empty string.
+
         Args:
-            *args (`Union[Msg, Sequence[Msg]]`):
+            args (`Union[MessageBase, Sequence[MessageBase]]`):
                 The input arguments to be formatted, where each argument
-                should be a `Msg` object or a list of `Msg` objects
+                should be a `Msg` object, or a list of `Msg` objects.
+                In distribution, placeholder is also allowed.
 
         Returns:
             `List[dict]`:
                 The formatted messages.
         """
         ollama_msgs = []
-        for msg in msgs:
+        for msg in args:
             if msg is None:
                 continue
-            if isinstance(msg, Msg):
+            if isinstance(msg, MessageBase):
+                # content shouldn't be empty string
+                if msg.content == "":
+                    logger.warning(
+                        "In ollama chat API, the content field cannot be "
+                        "empty string. To avoid error, the empty string is "
+                        "replaced by a blank space automatically, but the "
+                        "model may not work as expected.",
+                    )
+                    msg.content = " "
+
                 ollama_msg = {
                     "role": msg.role,
                     "content": _convert_to_str(msg.content),
                 }
 
                 # image url
                 if msg.url is not None:
@@ -279,15 +294,15 @@
         self.monitor.register(
             self._metric("call_counter"),
             metric_unit="times",
         )
 
     def format(
         self,
-        *args: Union[Msg, Sequence[Msg]],
+        *args: Union[MessageBase, Sequence[MessageBase]],
     ) -> Union[List[dict], str]:
         raise RuntimeError(
             f"Model Wrapper [{type(self).__name__}] doesn't "
             f"need to format the input. Please try to use the "
             f"model wrapper directly.",
         )
 
@@ -383,46 +398,62 @@
             metric_unit="token",
         )
         self.monitor.register(
             self._metric("total_tokens"),
             metric_unit="token",
         )
 
-    def format(self, *args: Union[Msg, Sequence[Msg]]) -> str:
+    def format(self, *args: Union[MessageBase, Sequence[MessageBase]]) -> str:
         """Forward the input to the model.
 
         Args:
-            *args (`Union[Msg, Sequence[Msg]]`):
+            args (`Union[MessageBase, Sequence[MessageBase]]`):
                 The input arguments to be formatted, where each argument
-                should be a string or a dict or a list of strings or dicts.
+                should be a `Msg` object, or a list of `Msg` objects.
+                In distribution, placeholder is also allowed.
 
         Returns:
             `str`:
                 The formatted string prompt.
         """
-
-        prompt = []
-
-        for arg in args:
-            if arg is None:
-                continue
-            if isinstance(arg, Msg):
-                prompt.append(f"{arg.name}: {_convert_to_str(arg.content)}")
-            elif isinstance(arg, list):
-                for child_arg in arg:
-                    if isinstance(child_arg, Msg):
-                        prompt.append(
-                            f"{child_arg.name}: "
-                            f"{_convert_to_str(child_arg.content)}",
-                        )
-                    else:
-                        raise TypeError(
-                            f"The input should be a Msg object or a list "
-                            f"of Msg objects, got {type(child_arg)}.",
-                        )
+        input_msgs = []
+        for _ in args:
+            if isinstance(_, MessageBase):
+                input_msgs.append(_)
+            elif isinstance(_, list) and all(
+                isinstance(__, MessageBase) for __ in _
+            ):
+                input_msgs.extend(_)
             else:
                 raise TypeError(
                     f"The input should be a Msg object or a list "
-                    f"of Msg objects, got {type(arg)}.",
+                    f"of Msg objects, got {type(_)}.",
                 )
 
-        return "\n".join(prompt)
+        sys_prompt = None
+        dialogue = []
+        for i, unit in enumerate(input_msgs):
+            if i == 0 and unit.role == "system":
+                # system prompt
+                sys_prompt = _convert_to_str(unit.content)
+            else:
+                # Merge all messages into a dialogue history prompt
+                dialogue.append(
+                    f"{unit.name}: {_convert_to_str(unit.content)}",
+                )
+
+        dialogue_history = "\n".join(dialogue)
+
+        if sys_prompt is None:
+            prompt_template = "## Dialogue History\n{dialogue_history}"
+        else:
+            prompt_template = (
+                "{system_prompt}\n"
+                "\n"
+                "## Dialogue History\n"
+                "{dialogue_history}"
+            )
+
+        return prompt_template.format(
+            system_prompt=sys_prompt,
+            dialogue_history=dialogue_history,
+        )
```

### Comparing `agentscope-0.0.2/src/agentscope/models/openai_model.py` & `agentscope-0.0.3/src/agentscope/models/openai_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from abc import ABC
 from typing import Union, Any, List, Sequence
 
 from loguru import logger
 
 from .model import ModelWrapperBase, ModelResponse
 from ..file_manager import file_manager
-from ..message import Msg
+from ..message import MessageBase
 from ..utils.tools import _convert_to_str
 
 try:
     import openai
 except ImportError:
     openai = None
 
@@ -87,15 +87,15 @@
 
         # Set monitor accordingly
         self._register_budget(model_name, budget)
         self._register_default_metrics()
 
     def format(
         self,
-        *args: Union[Msg, Sequence[Msg]],
+        *args: Union[MessageBase, Sequence[MessageBase]],
     ) -> Union[List[dict], str]:
         raise RuntimeError(
             f"Model Wrapper [{type(self).__name__}] doesn't "
             f"need to format the input. Please try to use the "
             f"model wrapper directly.",
         )
 
@@ -210,35 +210,36 @@
         return ModelResponse(
             text=response.choices[0].message.content,
             raw=response.model_dump(),
         )
 
     def format(
         self,
-        *args: Union[Msg, Sequence[Msg]],
+        *args: Union[MessageBase, Sequence[MessageBase]],
     ) -> List[dict]:
         """Format the input string and dictionary into the format that
         OpenAI Chat API required.
 
         Args:
-            *args (`Union[Msg, Sequence[Msg]]`):
-                The input strings, dictionaries, or list of string and
-                dictionaries to format.
+            args (`Union[MessageBase, Sequence[MessageBase]]`):
+                The input arguments to be formatted, where each argument
+                should be a `Msg` object, or a list of `Msg` objects.
+                In distribution, placeholder is also allowed.
 
         Returns:
             `List[dict]`:
                 The formatted messages in the format that OpenAI Chat API
                 required.
         """
 
         messages = []
         for arg in args:
             if arg is None:
                 continue
-            if isinstance(arg, Msg):
+            if isinstance(arg, MessageBase):
                 messages.append(
                     {
                         "role": arg.role,
                         "name": arg.name,
                         "content": _convert_to_str(arg.content),
                     },
                 )
```

### Comparing `agentscope-0.0.2/src/agentscope/models/post_model.py` & `agentscope-0.0.3/src/agentscope/models/post_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import requests
 from loguru import logger
 
 from .model import ModelWrapperBase, ModelResponse
 from ..constants import _DEFAULT_MAX_RETRIES
 from ..constants import _DEFAULT_MESSAGES_KEY
 from ..constants import _DEFAULT_RETRY_INTERVAL
-from ..message import Msg
+from ..message import MessageBase
 from ..utils.tools import _convert_to_str
 
 
 class PostAPIModelWrapperBase(ModelWrapperBase, ABC):
     """The base model wrapper for the model deployed on the POST API."""
 
     model_type: str = "post_api"
@@ -169,31 +169,36 @@
     def _parse_response(self, response: dict) -> ModelResponse:
         return ModelResponse(
             text=response["data"]["response"]["choices"][0]["message"][
                 "content"
             ],
         )
 
-    def format(self, *args: Union[Msg, Sequence[Msg]]) -> Union[List[dict]]:
+    def format(
+        self,
+        *args: Union[MessageBase, Sequence[MessageBase]],
+    ) -> Union[List[dict]]:
         """Format the input messages into a list of dict, which is
         compatible to OpenAI Chat API.
 
         Args:
-            args (`Union[Msg, Sequence[Msg]]`):
-                The input messages.
+            args (`Union[MessageBase, Sequence[MessageBase]]`):
+                The input arguments to be formatted, where each argument
+                should be a `Msg` object, or a list of `Msg` objects.
+                In distribution, placeholder is also allowed.
 
         Returns:
             `Union[List[dict]]`:
                 The formatted messages.
         """
         messages = []
         for arg in args:
             if arg is None:
                 continue
-            if isinstance(arg, Msg):
+            if isinstance(arg, MessageBase):
                 messages.append(
                     {
                         "role": arg.role,
                         "name": arg.name,
                         "content": _convert_to_str(arg.content),
                     },
                 )
@@ -217,14 +222,14 @@
 
     def _parse_response(self, response: dict) -> ModelResponse:
         urls = [img["url"] for img in response["data"]["response"]["data"]]
         return ModelResponse(image_urls=urls)
 
     def format(
         self,
-        *args: Union[Msg, Sequence[Msg]],
+        *args: Union[MessageBase, Sequence[MessageBase]],
     ) -> Union[List[dict], str]:
         raise RuntimeError(
             f"Model Wrapper [{type(self).__name__}] doesn't "
             f"need to format the input. Please try to use the "
             f"model wrapper directly.",
         )
```

### Comparing `agentscope-0.0.2/src/agentscope/msghub.py` & `agentscope-0.0.3/src/agentscope/msghub.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/pipelines/__init__.py` & `agentscope-0.0.3/src/agentscope/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/pipelines/functional.py` & `agentscope-0.0.3/src/agentscope/pipelines/functional.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/pipelines/pipeline.py` & `agentscope-0.0.3/src/agentscope/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/prompt.py` & `agentscope-0.0.3/src/agentscope/prompt.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/rpc/__init__.py` & `agentscope-0.0.3/src/agentscope/rpc/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 # -*- coding: utf-8 -*-
 """Import all rpc related modules in the package."""
 from typing import Any
-from .rpc_agent_client import RpcAgentClient
+from .rpc_agent_client import RpcAgentClient, ResponseStub, call_in_thread
 
 try:
     from .rpc_agent_pb2 import RpcMsg  # pylint: disable=E0611
 except ModuleNotFoundError:
-    RpcMsg = Any
+    RpcMsg = Any  # type: ignore[misc]
 try:
     from .rpc_agent_pb2_grpc import RpcAgentServicer
     from .rpc_agent_pb2_grpc import RpcAgentStub
     from .rpc_agent_pb2_grpc import add_RpcAgentServicer_to_server
 except ImportError:
     RpcAgentServicer = object
     RpcAgentStub = Any
     add_RpcAgentServicer_to_server = Any
 
 
 __all__ = [
     "RpcAgentClient",
+    "ResponseStub",
+    "call_in_thread",
     "RpcMsg",
     "RpcAgentServicer",
     "RpcAgentStub",
     "add_RpcAgentServicer_to_server",
 ]
```

### Comparing `agentscope-0.0.2/src/agentscope/rpc/rpc_agent_pb2.py` & `agentscope-0.0.3/src/agentscope/rpc/rpc_agent_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x0frpc_agent.proto",\n\x06RpcMsg\x12\r\n\x05value\x18\x01 \x01(\t\x12\x13\n\x0btarget_func\x18\x02 \x01(\t2+\n\x08RpcAgent\x12\x1f\n\tcall_func\x12\x07.RpcMsg\x1a\x07.RpcMsg"\x00\x62\x06proto3',
+    b'\n\x0frpc_agent.proto">\n\x06RpcMsg\x12\r\n\x05value\x18\x01 \x01(\t\x12\x13\n\x0btarget_func\x18\x02 \x01(\t\x12\x10\n\x08\x61gent_id\x18\x03 \x01(\t2+\n\x08RpcAgent\x12\x1f\n\tcall_func\x12\x07.RpcMsg\x1a\x07.RpcMsg"\x00\x62\x06proto3',
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "rpc_agent_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     _globals["_RPCMSG"]._serialized_start = 19
-    _globals["_RPCMSG"]._serialized_end = 63
-    _globals["_RPCAGENT"]._serialized_start = 65
-    _globals["_RPCAGENT"]._serialized_end = 108
+    _globals["_RPCMSG"]._serialized_end = 81
+    _globals["_RPCAGENT"]._serialized_start = 83
+    _globals["_RPCAGENT"]._serialized_end = 126
 # @@protoc_insertion_point(module_scope)
```

### Comparing `agentscope-0.0.2/src/agentscope/rpc/rpc_agent_pb2_grpc.py` & `agentscope-0.0.3/src/agentscope/rpc/rpc_agent_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 except ImportError:
     grpc = None
 
 import agentscope.rpc.rpc_agent_pb2 as rpc__agent__pb2
 
 
 class RpcAgentStub(object):
-    """Rpc agent Server Stub"""
+    """Servicer for rpc agent server"""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
```

### Comparing `agentscope-0.0.2/src/agentscope/service/__init__.py` & `agentscope-0.0.3/src/agentscope/service/__init__.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/service/execute_code/exec_python.py` & `agentscope-0.0.3/src/agentscope/service/execute_code/exec_python.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/service/file/common.py` & `agentscope-0.0.3/src/agentscope/service/file/common.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/service/file/json.py` & `agentscope-0.0.3/src/agentscope/service/file/json.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/service/file/text.py` & `agentscope-0.0.3/src/agentscope/service/file/text.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/service/retrieval/retrieval_from_list.py` & `agentscope-0.0.3/src/agentscope/service/retrieval/retrieval_from_list.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/service/retrieval/similarity.py` & `agentscope-0.0.3/src/agentscope/service/retrieval/similarity.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/service/service_factory.py` & `agentscope-0.0.3/src/agentscope/service/service_factory.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/service/service_response.py` & `agentscope-0.0.3/src/agentscope/service/service_response.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/service/sql_query/mongodb.py` & `agentscope-0.0.3/src/agentscope/service/sql_query/mongodb.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/service/sql_query/mysql.py` & `agentscope-0.0.3/src/agentscope/service/sql_query/mysql.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/service/sql_query/sqlite.py` & `agentscope-0.0.3/src/agentscope/service/sql_query/sqlite.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/service/text_processing/summarization.py` & `agentscope-0.0.3/src/agentscope/service/text_processing/summarization.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/service/web_search/search.py` & `agentscope-0.0.3/src/agentscope/service/web_search/search.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/service/web_search/web_digest.py` & `agentscope-0.0.3/src/agentscope/service/web_search/web_digest.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/utils/common.py` & `agentscope-0.0.3/src/agentscope/utils/common.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/utils/logging_utils.py` & `agentscope-0.0.3/src/agentscope/utils/logging_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,18 +78,18 @@
     Args:
         message (`Union[str, dict]`):
             The message to be logged. If it is a string, it will be logged
             directly. If it's a dict, it should have "name"(or "role") and
             "content" keys, and the message will be logged as "<name/role>:
             <content>".
     """
-    # Save message into file
+    # Save message into file, add default to ignore not serializable objects
     logger.log(
         LEVEL_CHAT_SAVE,
-        json.dumps(message, ensure_ascii=False),
+        json.dumps(message, ensure_ascii=False, default=lambda _: None),
         *args,
         **kwargs,
     )
 
     # Print message in terminal with specific format
     if isinstance(message, dict):
         contain_name_or_role = "name" in message or "role" in message
```

### Comparing `agentscope-0.0.2/src/agentscope/utils/monitor.py` & `agentscope-0.0.3/src/agentscope/utils/monitor.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/utils/token_utils.py` & `agentscope-0.0.3/src/agentscope/utils/token_utils.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/utils/tools.py` & `agentscope-0.0.3/src/agentscope/utils/tools.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/web/_app.py` & `agentscope-0.0.3/src/agentscope/web/_app.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/web/static/css/bootstrap.min.css` & `agentscope-0.0.3/src/agentscope/web/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/web/static/css/colors.css` & `agentscope-0.0.3/src/agentscope/web/static/css/colors.css`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/web/static/css/components.css` & `agentscope-0.0.3/src/agentscope/web/static/css/components.css`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/web/static/css/home.css` & `agentscope-0.0.3/src/agentscope/web/static/css/home.css`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/web/static/css/run.css` & `agentscope-0.0.3/src/agentscope/web/static/css/run.css`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/web/static/css/size.css` & `agentscope-0.0.3/src/agentscope/web/static/css/size.css`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/web/static/fonts/KRYPTON.ttf` & `agentscope-0.0.3/src/agentscope/web/static/fonts/KRYPTON.ttf`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/web/static/fonts/OSWALD.ttf` & `agentscope-0.0.3/src/agentscope/web/static/fonts/OSWALD.ttf`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/web/static/js/bootstrap-table.min.js` & `agentscope-0.0.3/src/agentscope/web/static/js/bootstrap-table.min.js`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/web/static/js/bootstrap.bundle.min.js` & `agentscope-0.0.3/src/agentscope/web/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/web/static/js/home.js` & `agentscope-0.0.3/src/agentscope/web/static/js/home.js`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/web/static/js/jquery-3.3.1.min.js` & `agentscope-0.0.3/src/agentscope/web/static/js/jquery-3.3.1.min.js`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/web/static/js/run.js` & `agentscope-0.0.3/src/agentscope/web/static/js/run.js`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/web/static/js/socket.io.js` & `agentscope-0.0.3/src/agentscope/web/static/js/socket.io.js`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/web/studio/studio.py` & `agentscope-0.0.3/src/agentscope/web/studio/studio.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope/web/studio/utils.py` & `agentscope-0.0.3/src/agentscope/web/studio/utils.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.2/src/agentscope.egg-info/PKG-INFO` & `agentscope-0.0.3/src/agentscope.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: agentscope
-Version: 0.0.2
+Version: 0.0.3
 Summary: AgentScope: A Flexible yet Robust Multi-Agent Platform.
 Home-page: https://github.com/modelscope/agentscope
-Download-URL: https://github.com/modelscope/agentscope/archive/v0.0.2.tar.gz
+Download-URL: https://github.com/modelscope/agentscope/archive/v0.0.3.tar.gz
 Author: SysML team of Alibaba Tongyi Lab 
 Author-email: gaodawei.gdw@alibaba-inc.com
 License: Apache License 2.0
 Keywords: deep-learning,multi agents,agents
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: docstring_parser
-Requires-Dist: loguru
+Requires-Dist: loguru==0.6.0
 Requires-Dist: tiktoken
 Requires-Dist: Pillow
 Requires-Dist: requests
 Requires-Dist: chardet
 Requires-Dist: inputimeout
 Requires-Dist: openai>=1.3.0
 Requires-Dist: numpy
@@ -30,15 +30,15 @@
 Requires-Dist: Flask-SocketIO==5.3.6
 Requires-Dist: dashscope==1.14.1
 Requires-Dist: openai>=1.3.0
 Requires-Dist: ollama>=0.1.7
 Requires-Dist: google-generativeai>=0.4.0
 Provides-Extra: distribute
 Requires-Dist: docstring_parser; extra == "distribute"
-Requires-Dist: loguru; extra == "distribute"
+Requires-Dist: loguru==0.6.0; extra == "distribute"
 Requires-Dist: tiktoken; extra == "distribute"
 Requires-Dist: Pillow; extra == "distribute"
 Requires-Dist: requests; extra == "distribute"
 Requires-Dist: chardet; extra == "distribute"
 Requires-Dist: inputimeout; extra == "distribute"
 Requires-Dist: openai>=1.3.0; extra == "distribute"
 Requires-Dist: numpy; extra == "distribute"
@@ -51,15 +51,15 @@
 Requires-Dist: google-generativeai>=0.4.0; extra == "distribute"
 Requires-Dist: grpcio==1.60.0; extra == "distribute"
 Requires-Dist: grpcio-tools==1.60.0; extra == "distribute"
 Requires-Dist: protobuf==4.25.0; extra == "distribute"
 Requires-Dist: expiringdict; extra == "distribute"
 Provides-Extra: dev
 Requires-Dist: docstring_parser; extra == "dev"
-Requires-Dist: loguru; extra == "dev"
+Requires-Dist: loguru==0.6.0; extra == "dev"
 Requires-Dist: tiktoken; extra == "dev"
 Requires-Dist: Pillow; extra == "dev"
 Requires-Dist: requests; extra == "dev"
 Requires-Dist: chardet; extra == "dev"
 Requires-Dist: inputimeout; extra == "dev"
 Requires-Dist: openai>=1.3.0; extra == "dev"
 Requires-Dist: numpy; extra == "dev"
@@ -71,15 +71,15 @@
 Requires-Dist: ollama>=0.1.7; extra == "dev"
 Requires-Dist: google-generativeai>=0.4.0; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Provides-Extra: full
 Requires-Dist: docstring_parser; extra == "full"
-Requires-Dist: loguru; extra == "full"
+Requires-Dist: loguru==0.6.0; extra == "full"
 Requires-Dist: tiktoken; extra == "full"
 Requires-Dist: Pillow; extra == "full"
 Requires-Dist: requests; extra == "full"
 Requires-Dist: chardet; extra == "full"
 Requires-Dist: inputimeout; extra == "full"
 Requires-Dist: openai>=1.3.0; extra == "full"
 Requires-Dist: numpy; extra == "full"
@@ -126,17 +126,17 @@
 [![](https://img.shields.io/badge/Contribute-Welcome-green)](https://modelscope.github.io/agentscope/tutorial/contribute.html)
 
 If you find our work helpful, please kindly
 cite [our paper](https://arxiv.org/abs/2402.14034).
 
 Welcome to join our community on
 
-| [Discord](https://discord.gg/eYMpfnkG8h)                                                                                         | DingTalk                                                                                                                          | WeChat                                                                                                                            |
-|----------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
-| <img src="https://gw.alicdn.com/imgextra/i1/O1CN01hhD1mu1Dd3BWVUvxN_!!6000000000238-2-tps-400-400.png" width="100" height="100"> | <img src="https://img.alicdn.com/imgextra/i2/O1CN01tuJ5971OmAqNg9cOw_!!6000000001747-0-tps-444-460.jpg" width="100" height="100"> | <img src="https://img.alicdn.com/imgextra/i3/O1CN01UyfWfx1CYBM3WqlBy_!!6000000000092-2-tps-400-400.png" width="100" height="100"> |
+| [Discord](https://discord.gg/eYMpfnkG8h)                                                                                         | DingTalk                                                                                                                          |
+|----------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
+| <img src="https://gw.alicdn.com/imgextra/i1/O1CN01hhD1mu1Dd3BWVUvxN_!!6000000000238-2-tps-400-400.png" width="100" height="100"> | <img src="https://img.alicdn.com/imgextra/i2/O1CN01tuJ5971OmAqNg9cOw_!!6000000001747-0-tps-444-460.jpg" width="100" height="100"> |
 
 ----
 
 ## News
 
 - ![new](https://img.alicdn.com/imgextra/i4/O1CN01kUiDtl1HVxN6G56vN_!!6000000000764-2-tps-43-19.png)
 [2024-03-19] We release **AgentScope** v0.0.2 now! In this new version,
```

### Comparing `agentscope-0.0.2/src/agentscope.egg-info/SOURCES.txt` & `agentscope-0.0.3/src/agentscope.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 src/agentscope/models/config.py
 src/agentscope/models/dashscope_model.py
 src/agentscope/models/gemini_model.py
 src/agentscope/models/model.py
 src/agentscope/models/ollama_model.py
 src/agentscope/models/openai_model.py
 src/agentscope/models/post_model.py
+src/agentscope/models/response.py
 src/agentscope/pipelines/__init__.py
 src/agentscope/pipelines/functional.py
 src/agentscope/pipelines/pipeline.py
 src/agentscope/rpc/__init__.py
 src/agentscope/rpc/rpc_agent_client.py
 src/agentscope/rpc/rpc_agent_pb2.py
 src/agentscope/rpc/rpc_agent_pb2_grpc.py
```

### Comparing `agentscope-0.0.2/src/agentscope.egg-info/requires.txt` & `agentscope-0.0.3/src/agentscope.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 docstring_parser
-loguru
+loguru==0.6.0
 tiktoken
 Pillow
 requests
 chardet
 inputimeout
 openai>=1.3.0
 numpy
@@ -13,15 +13,15 @@
 dashscope==1.14.1
 openai>=1.3.0
 ollama>=0.1.7
 google-generativeai>=0.4.0
 
 [dev]
 docstring_parser
-loguru
+loguru==0.6.0
 tiktoken
 Pillow
 requests
 chardet
 inputimeout
 openai>=1.3.0
 numpy
@@ -33,15 +33,15 @@
 google-generativeai>=0.4.0
 pytest
 pytest-cov
 pre-commit
 
 [distribute]
 docstring_parser
-loguru
+loguru==0.6.0
 tiktoken
 Pillow
 requests
 chardet
 inputimeout
 openai>=1.3.0
 numpy
@@ -54,15 +54,15 @@
 grpcio==1.60.0
 grpcio-tools==1.60.0
 protobuf==4.25.0
 expiringdict
 
 [full]
 docstring_parser
-loguru
+loguru==0.6.0
 tiktoken
 Pillow
 requests
 chardet
 inputimeout
 openai>=1.3.0
 numpy
```

