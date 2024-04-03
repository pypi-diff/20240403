# Comparing `tmp/dbally-0.0.1.tar.gz` & `tmp/dbally-0.0.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbally-0.0.1.tar", last modified: Wed Apr  3 12:51:27 2024, max compression
+gzip compressed data, was "dbally-0.0.1.dev0.tar", last modified: Wed Mar 20 12:00:11 2024, max compression
```

## Comparing `dbally-0.0.1.tar` & `dbally-0.0.1.dev0.tar`

### file list

```diff
@@ -1,108 +1,103 @@
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 12:51:27.567351 dbally-0.0.1/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1078 2024-04-03 11:01:33.000000 dbally-0.0.1/LICENSE
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       97 2024-04-03 11:01:33.000000 dbally-0.0.1/MANIFEST.in
--rw-r--r--   0 mateusz   (1001) mateusz   (1001)     2140 2024-04-03 12:51:27.567351 dbally-0.0.1/PKG-INFO
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     5960 2024-04-03 11:01:33.000000 dbally-0.0.1/README.md
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2969 2024-04-03 11:01:33.000000 dbally-0.0.1/pyproject.toml
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1655 2024-04-03 12:51:27.571351 dbally-0.0.1/setup.cfg
--rwxrwxr-x   0 mateusz   (1001) mateusz   (1001)      150 2024-04-03 11:01:33.000000 dbally-0.0.1/setup.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 12:51:27.487350 dbally-0.0.1/src/
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 12:51:27.495350 dbally-0.0.1/src/dbally/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        5 2024-04-03 12:40:06.000000 dbally-0.0.1/src/dbally/VERSION
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      600 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      180 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/__version__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     6149 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/_collection.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2302 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/_main.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 12:51:27.503350 dbally-0.0.1/src/dbally/assistants/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/assistants/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     4192 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/assistants/base.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     6239 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/assistants/openai.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 12:51:27.503350 dbally-0.0.1/src/dbally/audit/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      347 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/audit/__init__.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 12:51:27.511350 dbally-0.0.1/src/dbally/audit/event_handlers/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       59 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/audit/event_handlers/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1613 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/audit/event_handlers/base.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3243 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/audit/event_handlers/cli_event_handler.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2734 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/audit/event_handlers/langsmith_event_handler.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      409 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/audit/event_span.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2670 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/audit/event_tracker.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 12:51:27.511350 dbally-0.0.1/src/dbally/data_models/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/data_models/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      820 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/data_models/audit.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      330 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/data_models/execution_result.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      573 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/data_models/llm_options.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 12:51:27.519350 dbally-0.0.1/src/dbally/data_models/prompts/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      522 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/data_models/prompts/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1379 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/data_models/prompts/common_validation_utils.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1948 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/data_models/prompts/iql_explainer_prompt_template.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2192 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/data_models/prompts/iql_prompt_template.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1686 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/data_models/prompts/nl_responder_prompt_template.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2638 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/data_models/prompts/prompt_template.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1777 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/data_models/prompts/view_selector_prompt_template.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 12:51:27.523351 dbally-0.0.1/src/dbally/embedding_client/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/embedding_client/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      545 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/embedding_client/base.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1661 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/embedding_client/openai.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 12:51:27.527351 dbally-0.0.1/src/dbally/examples/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/examples/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     5442 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/examples/db.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     4468 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/examples/recruiting.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2155 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/examples/views.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 12:51:27.531350 dbally-0.0.1/src/dbally/iql/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      238 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/iql/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1510 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/iql/_exceptions.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     5064 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/iql/_processor.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      834 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/iql/_query.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2573 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/iql/_type_validators.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2396 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/iql/syntax.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 12:51:27.535351 dbally-0.0.1/src/dbally/iql_generator/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/iql_generator/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3716 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/iql_generator/iql_generator.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 12:51:27.535351 dbally-0.0.1/src/dbally/llm_client/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/llm_client/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2512 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/llm_client/base.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1935 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/llm_client/openai_client.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 12:51:27.539351 dbally-0.0.1/src/dbally/nl_responder/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/nl_responder/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3921 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/nl_responder/nl_responder.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2060 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/nl_responder/token_counters.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 12:51:27.539351 dbally-0.0.1/src/dbally/prompts/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       71 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/prompts/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2387 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/prompts/prompt_builder.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/py.typed
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 12:51:27.547351 dbally-0.0.1/src/dbally/similarity/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      391 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/similarity/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3381 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/similarity/faiss_store.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      382 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/similarity/fetcher.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1986 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/similarity/index.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3594 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/similarity/sqlalchemy_base.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      780 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/similarity/store.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 12:51:27.551351 dbally-0.0.1/src/dbally/utils/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/utils/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      249 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/utils/errors.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 12:51:27.551351 dbally-0.0.1/src/dbally/view_selection/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/view_selection/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      673 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/view_selection/base.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2398 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/view_selection/llm_view_selector.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      865 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/view_selection/random_view_selector.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 12:51:27.555351 dbally-0.0.1/src/dbally/views/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/views/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2253 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/views/base.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      406 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/views/decorators.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3218 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/views/methods_base.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3254 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/views/pandas_base.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3459 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally/views/sqlalchemy_base.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 12:51:27.563351 dbally-0.0.1/src/dbally.egg-info/
--rw-r--r--   0 mateusz   (1001) mateusz   (1001)     2140 2024-04-03 12:51:27.000000 dbally-0.0.1/src/dbally.egg-info/PKG-INFO
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2875 2024-04-03 12:51:27.000000 dbally-0.0.1/src/dbally.egg-info/SOURCES.txt
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        1 2024-04-03 12:51:27.000000 dbally-0.0.1/src/dbally.egg-info/dependency_links.txt
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       47 2024-04-03 12:51:27.000000 dbally-0.0.1/src/dbally.egg-info/entry_points.txt
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        1 2024-01-26 12:33:13.000000 dbally-0.0.1/src/dbally.egg-info/not-zip-safe
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      496 2024-04-03 12:51:27.000000 dbally-0.0.1/src/dbally.egg-info/requires.txt
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       18 2024-04-03 12:51:27.000000 dbally-0.0.1/src/dbally.egg-info/top_level.txt
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 12:51:27.559351 dbally-0.0.1/src/dbally_cli/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally_cli/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      112 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally_cli/example1.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      294 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally_cli/example2.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      235 2024-04-03 11:01:33.000000 dbally-0.0.1/src/dbally_cli/main.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.0.1/src/py.typed
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.682801 dbally-0.0.1.dev0/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1078 2024-03-20 11:52:45.000000 dbally-0.0.1.dev0/LICENSE
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       97 2024-02-02 13:52:13.000000 dbally-0.0.1.dev0/MANIFEST.in
+-rw-r--r--   0 mateusz   (1001) mateusz   (1001)     1413 2024-03-20 12:00:11.678801 dbally-0.0.1.dev0/PKG-INFO
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     4022 2024-03-20 11:48:39.000000 dbally-0.0.1.dev0/README.md
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2969 2024-03-06 13:57:39.000000 dbally-0.0.1.dev0/pyproject.toml
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1358 2024-03-20 12:00:11.682801 dbally-0.0.1.dev0/setup.cfg
+-rwxrwxr-x   0 mateusz   (1001) mateusz   (1001)      150 2024-02-02 13:52:13.000000 dbally-0.0.1.dev0/setup.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.614801 dbally-0.0.1.dev0/src/
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.618801 dbally-0.0.1.dev0/src/dbally/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        9 2024-03-19 08:38:07.000000 dbally-0.0.1.dev0/src/dbally/VERSION
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      372 2024-02-28 12:45:09.000000 dbally-0.0.1.dev0/src/dbally/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      180 2024-02-02 13:52:13.000000 dbally-0.0.1.dev0/src/dbally/__version__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     6149 2024-03-14 08:59:44.000000 dbally-0.0.1.dev0/src/dbally/_collection.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2302 2024-02-29 12:56:28.000000 dbally-0.0.1.dev0/src/dbally/_main.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.626801 dbally-0.0.1.dev0/src/dbally/audit/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      347 2024-03-14 12:16:46.000000 dbally-0.0.1.dev0/src/dbally/audit/__init__.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.630801 dbally-0.0.1.dev0/src/dbally/audit/event_handlers/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       59 2024-03-19 15:18:26.000000 dbally-0.0.1.dev0/src/dbally/audit/event_handlers/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1613 2024-02-27 12:41:08.000000 dbally-0.0.1.dev0/src/dbally/audit/event_handlers/base.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3243 2024-02-28 12:45:09.000000 dbally-0.0.1.dev0/src/dbally/audit/event_handlers/cli_event_handler.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2734 2024-02-27 13:41:27.000000 dbally-0.0.1.dev0/src/dbally/audit/event_handlers/langsmith_event_handler.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      409 2024-02-27 12:41:08.000000 dbally-0.0.1.dev0/src/dbally/audit/event_span.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2670 2024-02-27 12:41:08.000000 dbally-0.0.1.dev0/src/dbally/audit/event_tracker.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.634801 dbally-0.0.1.dev0/src/dbally/data_models/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-02-02 13:52:13.000000 dbally-0.0.1.dev0/src/dbally/data_models/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      820 2024-02-27 13:41:27.000000 dbally-0.0.1.dev0/src/dbally/data_models/audit.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      330 2024-02-29 12:56:28.000000 dbally-0.0.1.dev0/src/dbally/data_models/execution_result.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      573 2024-02-05 10:47:54.000000 dbally-0.0.1.dev0/src/dbally/data_models/llm_options.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.642801 dbally-0.0.1.dev0/src/dbally/data_models/prompts/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      522 2024-02-27 12:41:08.000000 dbally-0.0.1.dev0/src/dbally/data_models/prompts/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1379 2024-02-27 12:41:08.000000 dbally-0.0.1.dev0/src/dbally/data_models/prompts/common_validation_utils.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1948 2024-03-14 08:59:44.000000 dbally-0.0.1.dev0/src/dbally/data_models/prompts/iql_explainer_prompt_template.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2192 2024-03-14 08:59:44.000000 dbally-0.0.1.dev0/src/dbally/data_models/prompts/iql_prompt_template.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1686 2024-02-29 12:56:28.000000 dbally-0.0.1.dev0/src/dbally/data_models/prompts/nl_responder_prompt_template.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2638 2024-03-01 15:02:22.000000 dbally-0.0.1.dev0/src/dbally/data_models/prompts/prompt_template.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1777 2024-02-27 12:41:08.000000 dbally-0.0.1.dev0/src/dbally/data_models/prompts/view_selector_prompt_template.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.642801 dbally-0.0.1.dev0/src/dbally/embedding_client/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-03-13 10:43:31.000000 dbally-0.0.1.dev0/src/dbally/embedding_client/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      545 2024-03-13 10:43:31.000000 dbally-0.0.1.dev0/src/dbally/embedding_client/base.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1661 2024-03-13 10:43:31.000000 dbally-0.0.1.dev0/src/dbally/embedding_client/openai.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.646801 dbally-0.0.1.dev0/src/dbally/examples/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-03-14 08:59:44.000000 dbally-0.0.1.dev0/src/dbally/examples/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3147 2024-03-14 08:59:44.000000 dbally-0.0.1.dev0/src/dbally/examples/db.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3994 2024-03-19 15:18:26.000000 dbally-0.0.1.dev0/src/dbally/examples/recruiting.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2155 2024-03-14 08:59:44.000000 dbally-0.0.1.dev0/src/dbally/examples/views.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.650801 dbally-0.0.1.dev0/src/dbally/iql/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      238 2024-03-14 08:59:44.000000 dbally-0.0.1.dev0/src/dbally/iql/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1510 2024-02-29 12:56:28.000000 dbally-0.0.1.dev0/src/dbally/iql/_exceptions.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     5064 2024-03-14 08:59:44.000000 dbally-0.0.1.dev0/src/dbally/iql/_processor.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      834 2024-03-14 08:59:44.000000 dbally-0.0.1.dev0/src/dbally/iql/_query.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2573 2024-03-12 07:48:26.000000 dbally-0.0.1.dev0/src/dbally/iql/_type_validators.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2396 2024-03-14 08:59:44.000000 dbally-0.0.1.dev0/src/dbally/iql/syntax.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.654801 dbally-0.0.1.dev0/src/dbally/iql_generator/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-02-27 12:41:08.000000 dbally-0.0.1.dev0/src/dbally/iql_generator/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3716 2024-03-14 08:59:44.000000 dbally-0.0.1.dev0/src/dbally/iql_generator/iql_generator.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.654801 dbally-0.0.1.dev0/src/dbally/llm_client/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-02-05 10:36:27.000000 dbally-0.0.1.dev0/src/dbally/llm_client/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2512 2024-03-12 08:02:42.000000 dbally-0.0.1.dev0/src/dbally/llm_client/base.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1935 2024-03-12 08:02:42.000000 dbally-0.0.1.dev0/src/dbally/llm_client/openai_client.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.658801 dbally-0.0.1.dev0/src/dbally/nl_responder/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-03-19 15:18:26.000000 dbally-0.0.1.dev0/src/dbally/nl_responder/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3921 2024-03-14 08:59:44.000000 dbally-0.0.1.dev0/src/dbally/nl_responder/nl_responder.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2057 2024-03-12 08:02:42.000000 dbally-0.0.1.dev0/src/dbally/nl_responder/token_counters.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.658801 dbally-0.0.1.dev0/src/dbally/prompts/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       71 2024-02-02 13:52:13.000000 dbally-0.0.1.dev0/src/dbally/prompts/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2193 2024-02-05 10:36:27.000000 dbally-0.0.1.dev0/src/dbally/prompts/prompt_builder.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-02-02 13:52:13.000000 dbally-0.0.1.dev0/src/dbally/py.typed
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.666801 dbally-0.0.1.dev0/src/dbally/similarity/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      391 2024-03-14 12:16:46.000000 dbally-0.0.1.dev0/src/dbally/similarity/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3381 2024-03-14 12:16:46.000000 dbally-0.0.1.dev0/src/dbally/similarity/faiss_store.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      382 2024-03-06 13:57:39.000000 dbally-0.0.1.dev0/src/dbally/similarity/fetcher.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1986 2024-03-12 07:48:26.000000 dbally-0.0.1.dev0/src/dbally/similarity/index.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3594 2024-03-06 13:57:39.000000 dbally-0.0.1.dev0/src/dbally/similarity/sqlalchemy_base.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      780 2024-03-06 13:57:39.000000 dbally-0.0.1.dev0/src/dbally/similarity/store.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.666801 dbally-0.0.1.dev0/src/dbally/utils/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-03-19 15:18:26.000000 dbally-0.0.1.dev0/src/dbally/utils/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      249 2024-03-14 08:59:44.000000 dbally-0.0.1.dev0/src/dbally/utils/errors.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.670801 dbally-0.0.1.dev0/src/dbally/view_selection/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-02-02 13:52:13.000000 dbally-0.0.1.dev0/src/dbally/view_selection/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      673 2024-02-27 12:41:08.000000 dbally-0.0.1.dev0/src/dbally/view_selection/base.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2398 2024-03-14 08:59:44.000000 dbally-0.0.1.dev0/src/dbally/view_selection/llm_view_selector.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      865 2024-02-27 12:41:08.000000 dbally-0.0.1.dev0/src/dbally/view_selection/random_view_selector.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.674801 dbally-0.0.1.dev0/src/dbally/views/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-03-19 15:18:26.000000 dbally-0.0.1.dev0/src/dbally/views/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2253 2024-03-14 08:59:44.000000 dbally-0.0.1.dev0/src/dbally/views/base.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      406 2024-03-14 08:59:44.000000 dbally-0.0.1.dev0/src/dbally/views/decorators.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1695 2024-03-14 08:59:44.000000 dbally-0.0.1.dev0/src/dbally/views/methods_base.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     4767 2024-03-14 08:59:44.000000 dbally-0.0.1.dev0/src/dbally/views/sqlalchemy_base.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.678801 dbally-0.0.1.dev0/src/dbally.egg-info/
+-rw-r--r--   0 mateusz   (1001) mateusz   (1001)     1413 2024-03-20 12:00:11.000000 dbally-0.0.1.dev0/src/dbally.egg-info/PKG-INFO
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2747 2024-03-20 12:00:11.000000 dbally-0.0.1.dev0/src/dbally.egg-info/SOURCES.txt
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        1 2024-03-20 12:00:11.000000 dbally-0.0.1.dev0/src/dbally.egg-info/dependency_links.txt
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       47 2024-03-20 12:00:11.000000 dbally-0.0.1.dev0/src/dbally.egg-info/entry_points.txt
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        1 2024-01-26 12:33:13.000000 dbally-0.0.1.dev0/src/dbally.egg-info/not-zip-safe
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      261 2024-03-20 12:00:11.000000 dbally-0.0.1.dev0/src/dbally.egg-info/requires.txt
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       18 2024-03-20 12:00:11.000000 dbally-0.0.1.dev0/src/dbally.egg-info/top_level.txt
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.678801 dbally-0.0.1.dev0/src/dbally_cli/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-03-06 13:57:39.000000 dbally-0.0.1.dev0/src/dbally_cli/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      112 2024-03-06 13:57:39.000000 dbally-0.0.1.dev0/src/dbally_cli/example1.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      294 2024-03-06 13:57:39.000000 dbally-0.0.1.dev0/src/dbally_cli/example2.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      235 2024-03-06 13:57:39.000000 dbally-0.0.1.dev0/src/dbally_cli/main.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-02-02 13:52:13.000000 dbally-0.0.1.dev0/src/py.typed
```

### Comparing `dbally-0.0.1/LICENSE` & `dbally-0.0.1.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1/PKG-INFO` & `dbally-0.0.1.dev0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,36 @@
 Metadata-Version: 2.1
 Name: dbally
-Version: 0.0.1
+Version: 0.0.1.dev0
 Summary: "Efficient, consistent and secure library for querying structured data with natural language"
 Author: deepsense.ai
 Author-email: contact@deepsense.ai
 License: MIT
 Project-URL: Documentation, https://db-ally.deepsense.ai/
-Project-URL: Source, https://github.com/deepsense-ai/db-ally
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: pandas~=2.0.3
 Requires-Dist: python-dotenv>=0.5.1
 Requires-Dist: SQLAlchemy==2.0.25
 Requires-Dist: tabulate>=0.9.0
+Requires-Dist: transformers>=4.37.1
 Requires-Dist: click~=8.1.7
 Requires-Dist: numpy>=1.24.0
 Provides-Extra: openai
 Requires-Dist: openai>=1.10.0; extra == "openai"
 Requires-Dist: tiktoken>=0.6.0; extra == "openai"
 Provides-Extra: faiss
 Requires-Dist: faiss-cpu>=1.8.0; extra == "faiss"
 Provides-Extra: examples
 Requires-Dist: pydantic~=2.6.0; extra == "examples"
 Requires-Dist: pydantic_settings~=2.1.0; extra == "examples"
 Requires-Dist: psycopg2-binary~=2.9.9; extra == "examples"
-Provides-Extra: langsmith
-Requires-Dist: langsmith>=0.0.87; extra == "langsmith"
-Provides-Extra: transformers
-Requires-Dist: transformers>=4.37.1; extra == "transformers"
-Provides-Extra: benchmark
-Requires-Dist: asyncpg~=0.28.0; extra == "benchmark"
-Requires-Dist: eval-type-backport~=0.1.3; extra == "benchmark"
-Requires-Dist: hydra-core~=1.3.2; extra == "benchmark"
-Requires-Dist: loguru~=0.7.0; extra == "benchmark"
-Requires-Dist: neptune~=1.6.3; extra == "benchmark"
-Requires-Dist: pydantic~=2.6.1; extra == "benchmark"
-Requires-Dist: pydantic-core~=2.16.2; extra == "benchmark"
-Requires-Dist: pydantic-settings~=2.0.3; extra == "benchmark"
-Requires-Dist: psycopg2-binary~=2.9.9; extra == "benchmark"
```

### Comparing `dbally-0.0.1/pyproject.toml` & `dbally-0.0.1.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1/setup.cfg` & `dbally-0.0.1.dev0/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -6,65 +6,51 @@
 author_email = contact@deepsense.ai
 license = MIT
 license_files = LICENSE
 classifiers = 
 	Development Status :: 2 - Pre-Alpha
 	Environment :: Console
 	Intended Audience :: Developers
-	License :: OSI Approved :: MIT License
+	License :: Other/Proprietary License
 	Natural Language :: English
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3.12
 project_urls = 
 	Documentation = https://db-ally.deepsense.ai/
-	Source = https://github.com/deepsense-ai/db-ally
 
 [options]
 package_dir = 
 	=src
 packages = find:
 zip_safe = False
 platforms = any
 include_package_data = True
 python_requires = >=3.8
 install_requires = 
 	pandas~=2.0.3
 	python-dotenv>=0.5.1
 	SQLAlchemy==2.0.25
 	tabulate>=0.9.0
+	transformers>=4.37.1
 	click~=8.1.7
 	numpy>=1.24.0
 
 [options.extras_require]
 openai = 
 	openai>=1.10.0
 	tiktoken>=0.6.0
 faiss = 
 	faiss-cpu>=1.8.0
 examples = 
 	pydantic~=2.6.0
 	pydantic_settings~=2.1.0
 	psycopg2-binary~=2.9.9
-langsmith = 
-	langsmith>=0.0.87
-transformers = 
-	transformers>=4.37.1
-benchmark = 
-	asyncpg~=0.28.0
-	eval-type-backport~=0.1.3
-	hydra-core~=1.3.2
-	loguru~=0.7.0
-	neptune~=1.6.3
-	pydantic~=2.6.1
-	pydantic-core~=2.16.2
-	pydantic-settings~=2.0.3
-	psycopg2-binary~=2.9.9
 
 [options.packages.find]
 where = src
 
 [bdist_wheel]
 universal = 1
```

### Comparing `dbally-0.0.1/src/dbally/_collection.py` & `dbally-0.0.1.dev0/src/dbally/_collection.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1/src/dbally/_main.py` & `dbally-0.0.1.dev0/src/dbally/_main.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1/src/dbally/audit/event_handlers/base.py` & `dbally-0.0.1.dev0/src/dbally/audit/event_handlers/base.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1/src/dbally/audit/event_handlers/cli_event_handler.py` & `dbally-0.0.1.dev0/src/dbally/audit/event_handlers/cli_event_handler.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1/src/dbally/audit/event_handlers/langsmith_event_handler.py` & `dbally-0.0.1.dev0/src/dbally/audit/event_handlers/langsmith_event_handler.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1/src/dbally/audit/event_tracker.py` & `dbally-0.0.1.dev0/src/dbally/audit/event_tracker.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1/src/dbally/data_models/audit.py` & `dbally-0.0.1.dev0/src/dbally/data_models/audit.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1/src/dbally/data_models/llm_options.py` & `dbally-0.0.1.dev0/src/dbally/data_models/llm_options.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1/src/dbally/data_models/prompts/__init__.py` & `dbally-0.0.1.dev0/src/dbally/data_models/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1/src/dbally/data_models/prompts/common_validation_utils.py` & `dbally-0.0.1.dev0/src/dbally/data_models/prompts/common_validation_utils.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1/src/dbally/data_models/prompts/iql_explainer_prompt_template.py` & `dbally-0.0.1.dev0/src/dbally/data_models/prompts/iql_explainer_prompt_template.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1/src/dbally/data_models/prompts/iql_prompt_template.py` & `dbally-0.0.1.dev0/src/dbally/data_models/prompts/iql_prompt_template.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1/src/dbally/data_models/prompts/nl_responder_prompt_template.py` & `dbally-0.0.1.dev0/src/dbally/data_models/prompts/nl_responder_prompt_template.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1/src/dbally/data_models/prompts/prompt_template.py` & `dbally-0.0.1.dev0/src/dbally/data_models/prompts/prompt_template.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1/src/dbally/data_models/prompts/view_selector_prompt_template.py` & `dbally-0.0.1.dev0/src/dbally/data_models/prompts/view_selector_prompt_template.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1/src/dbally/embedding_client/base.py` & `dbally-0.0.1.dev0/src/dbally/embedding_client/base.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1/src/dbally/embedding_client/openai.py` & `dbally-0.0.1.dev0/src/dbally/embedding_client/openai.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1/src/dbally/examples/recruiting.py` & `dbally-0.0.1.dev0/src/dbally/examples/recruiting.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,19 @@
 import asyncio
 from dataclasses import dataclass
 from typing import List
 
+from dbally_benchmark.text2sql.prompt_template import TEXT2SQL_PROMPT_TEMPLATE
+
 import dbally
 from dbally.audit.event_handlers.cli_event_handler import CLIEventHandler
 from dbally.audit.event_tracker import EventTracker
 from dbally.examples.db import ENGINE, fill_candidate_table, get_recruitment_db_description
 from dbally.examples.views import RecruitmentView
 from dbally.llm_client.openai_client import OpenAIClient
-from dbally.prompts.prompt_builder import PromptTemplate
-
-TEXT2SQL_PROMPT_TEMPLATE = PromptTemplate(
-    (
-        {
-            "role": "system",
-            "content": (
-                "You are given the following SQL tables:"
-                "\n\n{schema}\n\n"
-                "Your job is to write queries given a user’s request."
-                "Please return only the query, do not provide any extra text or explanation."
-            ),
-        },
-        {
-            "role": "user",
-            "content": ("{question}"),
-        },
-    )
-)
 
 
 @dataclass
 class Question:
     """
     A question to be asked to the recruitment database.
     """
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `dbally-0.0.1/src/dbally/examples/views.py` & `dbally-0.0.1.dev0/src/dbally/examples/views.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1/src/dbally/iql/_exceptions.py` & `dbally-0.0.1.dev0/src/dbally/iql/_exceptions.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1/src/dbally/iql/_processor.py` & `dbally-0.0.1.dev0/src/dbally/iql/_processor.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1/src/dbally/iql/_query.py` & `dbally-0.0.1.dev0/src/dbally/iql/_query.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1/src/dbally/iql/_type_validators.py` & `dbally-0.0.1.dev0/src/dbally/iql/_type_validators.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1/src/dbally/iql/syntax.py` & `dbally-0.0.1.dev0/src/dbally/iql/syntax.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1/src/dbally/iql_generator/iql_generator.py` & `dbally-0.0.1.dev0/src/dbally/iql_generator/iql_generator.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1/src/dbally/llm_client/base.py` & `dbally-0.0.1.dev0/src/dbally/llm_client/base.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1/src/dbally/llm_client/openai_client.py` & `dbally-0.0.1.dev0/src/dbally/llm_client/openai_client.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1/src/dbally/nl_responder/nl_responder.py` & `dbally-0.0.1.dev0/src/dbally/nl_responder/nl_responder.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1/src/dbally/nl_responder/token_counters.py` & `dbally-0.0.1.dev0/src/dbally/nl_responder/token_counters.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     Raises:
         ImportError: If transformers package is not installed.
     """
 
     try:
         from transformers import AutoTokenizer  # pylint: disable=import-outside-toplevel
     except ImportError as exc:
-        raise ImportError("You need to install transformers package to use huggingface models' tokenizers.") from exc
+        raise ImportError("You need to install transformers package to use Anyscale models' tokenizers.") from exc
 
     tokenizer = AutoTokenizer.from_pretrained(model)
 
     for message in messages:
         message["content"] = message["content"].format(**fmt)
 
     return len(tokenizer.apply_chat_template(messages, tokenize=True, add_generation_prompt=True))
```

### Comparing `dbally-0.0.1/src/dbally/prompts/prompt_builder.py` & `dbally-0.0.1.dev0/src/dbally/prompts/prompt_builder.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import TYPE_CHECKING, Dict, Optional, Union
+from typing import Dict, Optional, Union
 
-from dbally.data_models.prompts.prompt_template import ChatFormat, PromptTemplate
+from transformers import AutoTokenizer
+from transformers.tokenization_utils import PreTrainedTokenizer
 
-if TYPE_CHECKING:
-    from transformers.tokenization_utils import PreTrainedTokenizer
+from dbally.data_models.prompts.prompt_template import ChatFormat, PromptTemplate
 
 
 class PromptBuilder:
     """Class used to build prompts"""
 
     def __init__(self, model_name: Optional[str] = None) -> None:
         """
@@ -15,23 +15,19 @@
 
         Args:
             model_name: Name of the model to load a tokenizer for.
                         Tokenizer is used to append special tokens to the prompt. If empty, no tokens will be added.
         Raises:
             OSError: If model_name is not found in huggingface.co/models
         """
-        self._tokenizer: Optional["PreTrainedTokenizer"] = None
-
-        if model_name is not None and not model_name.startswith("gpt"):
-            try:
-                from transformers import AutoTokenizer  # pylint: disable=import-outside-toplevel
-            except ImportError as exc:
-                raise ImportError("You need to install transformers package to use huggingface models.") from exc
-
-            self._tokenizer = AutoTokenizer.from_pretrained(model_name)
+        self._tokenizer: Optional[PreTrainedTokenizer] = None
+        if model_name is not None:
+            # openAI client handles special tokens for gpt.
+            if not model_name.startswith("gpt"):
+                self._tokenizer = AutoTokenizer.from_pretrained(model_name)
 
     def _format_prompt(self, prompt_template: PromptTemplate, fmt: Dict[str, str]) -> ChatFormat:
         """
         Format prompt using provided arguments
 
         Args:
             prompt_template: this template will be modified in place
```

### Comparing `dbally-0.0.1/src/dbally/similarity/faiss_store.py` & `dbally-0.0.1.dev0/src/dbally/similarity/faiss_store.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1/src/dbally/similarity/index.py` & `dbally-0.0.1.dev0/src/dbally/similarity/index.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1/src/dbally/similarity/sqlalchemy_base.py` & `dbally-0.0.1.dev0/src/dbally/similarity/sqlalchemy_base.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1/src/dbally/similarity/store.py` & `dbally-0.0.1.dev0/src/dbally/similarity/store.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1/src/dbally/view_selection/base.py` & `dbally-0.0.1.dev0/src/dbally/view_selection/base.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1/src/dbally/view_selection/llm_view_selector.py` & `dbally-0.0.1.dev0/src/dbally/view_selection/llm_view_selector.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1/src/dbally/view_selection/random_view_selector.py` & `dbally-0.0.1.dev0/src/dbally/view_selection/random_view_selector.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1/src/dbally/views/base.py` & `dbally-0.0.1.dev0/src/dbally/views/base.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1/src/dbally.egg-info/PKG-INFO` & `dbally-0.0.1.dev0/src/dbally.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,36 @@
 Metadata-Version: 2.1
 Name: dbally
-Version: 0.0.1
+Version: 0.0.1.dev0
 Summary: "Efficient, consistent and secure library for querying structured data with natural language"
 Author: deepsense.ai
 Author-email: contact@deepsense.ai
 License: MIT
 Project-URL: Documentation, https://db-ally.deepsense.ai/
-Project-URL: Source, https://github.com/deepsense-ai/db-ally
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: pandas~=2.0.3
 Requires-Dist: python-dotenv>=0.5.1
 Requires-Dist: SQLAlchemy==2.0.25
 Requires-Dist: tabulate>=0.9.0
+Requires-Dist: transformers>=4.37.1
 Requires-Dist: click~=8.1.7
 Requires-Dist: numpy>=1.24.0
 Provides-Extra: openai
 Requires-Dist: openai>=1.10.0; extra == "openai"
 Requires-Dist: tiktoken>=0.6.0; extra == "openai"
 Provides-Extra: faiss
 Requires-Dist: faiss-cpu>=1.8.0; extra == "faiss"
 Provides-Extra: examples
 Requires-Dist: pydantic~=2.6.0; extra == "examples"
 Requires-Dist: pydantic_settings~=2.1.0; extra == "examples"
 Requires-Dist: psycopg2-binary~=2.9.9; extra == "examples"
-Provides-Extra: langsmith
-Requires-Dist: langsmith>=0.0.87; extra == "langsmith"
-Provides-Extra: transformers
-Requires-Dist: transformers>=4.37.1; extra == "transformers"
-Provides-Extra: benchmark
-Requires-Dist: asyncpg~=0.28.0; extra == "benchmark"
-Requires-Dist: eval-type-backport~=0.1.3; extra == "benchmark"
-Requires-Dist: hydra-core~=1.3.2; extra == "benchmark"
-Requires-Dist: loguru~=0.7.0; extra == "benchmark"
-Requires-Dist: neptune~=1.6.3; extra == "benchmark"
-Requires-Dist: pydantic~=2.6.1; extra == "benchmark"
-Requires-Dist: pydantic-core~=2.16.2; extra == "benchmark"
-Requires-Dist: pydantic-settings~=2.0.3; extra == "benchmark"
-Requires-Dist: psycopg2-binary~=2.9.9; extra == "benchmark"
```

### Comparing `dbally-0.0.1/src/dbally.egg-info/SOURCES.txt` & `dbally-0.0.1.dev0/src/dbally.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,14 @@
 src/dbally.egg-info/PKG-INFO
 src/dbally.egg-info/SOURCES.txt
 src/dbally.egg-info/dependency_links.txt
 src/dbally.egg-info/entry_points.txt
 src/dbally.egg-info/not-zip-safe
 src/dbally.egg-info/requires.txt
 src/dbally.egg-info/top_level.txt
-src/dbally/assistants/__init__.py
-src/dbally/assistants/base.py
-src/dbally/assistants/openai.py
 src/dbally/audit/__init__.py
 src/dbally/audit/event_span.py
 src/dbally/audit/event_tracker.py
 src/dbally/audit/event_handlers/__init__.py
 src/dbally/audit/event_handlers/base.py
 src/dbally/audit/event_handlers/cli_event_handler.py
 src/dbally/audit/event_handlers/langsmith_event_handler.py
@@ -74,13 +71,12 @@
 src/dbally/view_selection/base.py
 src/dbally/view_selection/llm_view_selector.py
 src/dbally/view_selection/random_view_selector.py
 src/dbally/views/__init__.py
 src/dbally/views/base.py
 src/dbally/views/decorators.py
 src/dbally/views/methods_base.py
-src/dbally/views/pandas_base.py
 src/dbally/views/sqlalchemy_base.py
 src/dbally_cli/__init__.py
 src/dbally_cli/example1.py
 src/dbally_cli/example2.py
 src/dbally_cli/main.py
```

