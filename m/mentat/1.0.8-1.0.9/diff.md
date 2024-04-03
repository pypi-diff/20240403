# Comparing `tmp/mentat-1.0.8.tar.gz` & `tmp/mentat-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentat-1.0.8.tar", last modified: Mon Jan  8 20:20:15 2024, max compression
+gzip compressed data, was "mentat-1.0.9.tar", last modified: Fri Jan 19 01:04:02 2024, max compression
```

## Comparing `mentat-1.0.8.tar` & `mentat-1.0.9.tar`

### file list

```diff
@@ -1,160 +1,156 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:20:15.165673 mentat-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-01-08 20:20:04.000000 mentat-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-01-08 20:20:04.000000 mentat-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8328 2024-01-08 20:20:15.165673 mentat-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-01-08 20:20:04.000000 mentat-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-01-08 20:20:04.000000 mentat-1.0.8/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:20:15.149674 mentat-1.0.8/mentat/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/agent_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/app_conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/auto_completer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/broadcast.py
--rw-r--r--   0 runner    (1001) docker     (127)    16292 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/code_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/code_edit_feedback.py
--rw-r--r--   0 runner    (1001) docker     (127)     9827 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/code_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/code_file_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:20:15.153674 mentat-1.0.8/mentat/command/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/command/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:20:15.153674 mentat-1.0.8/mentat/command/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/command/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/command/commands/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/command/commands/clear.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/command/commands/commit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/command/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/command/commands/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/command/commands/exclude.py
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/command/commands/help.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/command/commands/include.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/command/commands/redo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/command/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/command/commands/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/command/commands/screenshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/command/commands/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/command/commands/talk.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/command/commands/undo.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/command/commands/undoall.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/command/commands/viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9376 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    13076 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/cost_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/ctags.py
--rw-r--r--   0 runner    (1001) docker     (127)     7715 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/diff_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/edit_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     6238 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:20:15.153674 mentat-1.0.8/mentat/feature_filters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/feature_filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/feature_filters/default_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/feature_filters/embedding_similarity_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/feature_filters/feature_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6603 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/feature_filters/llm_feature_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/feature_filters/truncate_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8327 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/git_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11478 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/include_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/interval.py
--rw-r--r--   0 runner    (1001) docker     (127)    14053 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/llm_api_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/logging_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:20:15.157673 mentat-1.0.8/mentat/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11253 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/parsers/block_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/parsers/change_display_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/parsers/diff_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13268 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/parsers/file_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/parsers/git_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6689 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/parsers/json_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    17858 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/parsers/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/parsers/parser_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     6094 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/parsers/replacement_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8934 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/parsers/unified_diff_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:20:15.157673 mentat-1.0.8/mentat/prompts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/prompts/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:20:15.157673 mentat-1.0.8/mentat/python_client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/python_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/python_client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:20:15.145674 mentat-1.0.8/mentat/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:20:15.157673 mentat-1.0.8/mentat/resources/conf/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/resources/conf/conf.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:20:15.157673 mentat-1.0.8/mentat/resources/prompts/
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/resources/prompts/agent_command_selection_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/resources/prompts/agent_file_selection_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/resources/prompts/block_parser_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/resources/prompts/feature_selection_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/resources/prompts/json_parser_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/resources/prompts/replacement_parser_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/resources/prompts/unified_diff_parser_prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:20:15.157673 mentat-1.0.8/mentat/resources/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/resources/templates/benchmark.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/resources/templates/conversation_viewer.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:20:15.157673 mentat-1.0.8/mentat/resources/templates/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/resources/templates/css/benchmark.css
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/resources/templates/css/conversation_viewer.css
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/resources/templates/css/transcript.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:20:15.157673 mentat-1.0.8/mentat/resources/templates/js/
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/resources/templates/js/conversation_viewer.js
--rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/resources/templates/js/transcript.js
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/resources/templates/transcript.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:20:15.157673 mentat-1.0.8/mentat/sampler/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/sampler/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     8445 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/sampler/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/sampler/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/sentry.py
--rw-r--r--   0 runner    (1001) docker     (127)    10792 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/session_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/session_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/session_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/streaming_printer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:20:15.161673 mentat-1.0.8/mentat/terminal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/terminal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8679 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/terminal/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/terminal/loading.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/terminal/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/terminal/prompt_completer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/terminal/prompt_session.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/terminal/themes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/transcripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:20:15.161673 mentat-1.0.8/mentat/vision/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/vision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-01-08 20:20:04.000000 mentat-1.0.8/mentat/vision/vision_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:20:15.149674 mentat-1.0.8/mentat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8328 2024-01-08 20:20:15.000000 mentat-1.0.8/mentat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-01-08 20:20:15.000000 mentat-1.0.8/mentat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-08 20:20:15.000000 mentat-1.0.8/mentat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-01-08 20:20:15.000000 mentat-1.0.8/mentat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-01-08 20:20:15.000000 mentat-1.0.8/mentat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-08 20:20:15.000000 mentat-1.0.8/mentat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-01-08 20:20:04.000000 mentat-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-01-08 20:20:04.000000 mentat-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-08 20:20:15.165673 mentat-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-01-08 20:20:04.000000 mentat-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:20:15.165673 mentat-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:20:04.000000 mentat-1.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-01-08 20:20:04.000000 mentat-1.0.8/tests/benchmark_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-01-08 20:20:04.000000 mentat-1.0.8/tests/broadcast_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17282 2024-01-08 20:20:04.000000 mentat-1.0.8/tests/code_context_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-01-08 20:20:04.000000 mentat-1.0.8/tests/code_feature_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-01-08 20:20:04.000000 mentat-1.0.8/tests/code_file_manager_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9804 2024-01-08 20:20:04.000000 mentat-1.0.8/tests/commands_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-01-08 20:20:04.000000 mentat-1.0.8/tests/config_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11447 2024-01-08 20:20:04.000000 mentat-1.0.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-01-08 20:20:04.000000 mentat-1.0.8/tests/conversation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7326 2024-01-08 20:20:04.000000 mentat-1.0.8/tests/diff_context_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-01-08 20:20:04.000000 mentat-1.0.8/tests/embeddings_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-01-08 20:20:04.000000 mentat-1.0.8/tests/git_handler_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-01-08 20:20:04.000000 mentat-1.0.8/tests/include_files_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-01-08 20:20:04.000000 mentat-1.0.8/tests/license_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-01-08 20:20:04.000000 mentat-1.0.8/tests/llm_api_handler_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-01-08 20:20:04.000000 mentat-1.0.8/tests/measure_api_speed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-01-08 20:20:04.000000 mentat-1.0.8/tests/record_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)    15541 2024-01-08 20:20:04.000000 mentat-1.0.8/tests/sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-01-08 20:20:04.000000 mentat-1.0.8/tests/session_input_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-01-08 20:20:04.000000 mentat-1.0.8/tests/system_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-01-08 20:20:04.000000 mentat-1.0.8/tests/test_loading_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-01-08 20:20:04.000000 mentat-1.0.8/tests/ui_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-01-08 20:20:04.000000 mentat-1.0.8/tests/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-01-08 20:20:04.000000 mentat-1.0.8/tests/vision_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 01:04:02.402613 mentat-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-01-19 01:03:42.000000 mentat-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-01-19 01:03:42.000000 mentat-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4987 2024-01-19 01:04:02.402613 mentat-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-01-19 01:03:42.000000 mentat-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 01:04:02.386613 mentat-1.0.9/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-19 01:03:42.000000 mentat-1.0.9/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-01-19 01:03:42.000000 mentat-1.0.9/benchmarks/arg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-01-19 01:03:42.000000 mentat-1.0.9/benchmarks/benchmark_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-01-19 01:03:42.000000 mentat-1.0.9/benchmarks/benchmark_result_summary.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10961 2024-01-19 01:03:42.000000 mentat-1.0.9/benchmarks/benchmark_runner.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7168 2024-01-19 01:03:42.000000 mentat-1.0.9/benchmarks/context_benchmark.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4661 2024-01-19 01:03:42.000000 mentat-1.0.9/benchmarks/edit_rubric_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 01:04:02.386613 mentat-1.0.9/benchmarks/exercise_runners/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-19 01:03:42.000000 mentat-1.0.9/benchmarks/exercise_runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-01-19 01:03:42.000000 mentat-1.0.9/benchmarks/exercise_runners/abstract_exercise_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-01-19 01:03:42.000000 mentat-1.0.9/benchmarks/exercise_runners/clojure_exercise_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-01-19 01:03:42.000000 mentat-1.0.9/benchmarks/exercise_runners/exercise_runner_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-01-19 01:03:42.000000 mentat-1.0.9/benchmarks/exercise_runners/javascript_exercise_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-01-19 01:03:42.000000 mentat-1.0.9/benchmarks/exercise_runners/python_exercise_runner.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8451 2024-01-19 01:03:42.000000 mentat-1.0.9/benchmarks/exercism_practice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-01-19 01:03:42.000000 mentat-1.0.9/benchmarks/run_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-01-19 01:03:42.000000 mentat-1.0.9/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 01:04:02.390613 mentat-1.0.9/mentat/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/agent_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/app_conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10324 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/auto_completer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16357 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/code_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/code_edit_feedback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9827 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/code_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/code_file_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 01:04:02.394613 mentat-1.0.9/mentat/command/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/command/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 01:04:02.394613 mentat-1.0.9/mentat/command/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/command/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/command/commands/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/command/commands/amend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/command/commands/clear.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/command/commands/commit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/command/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/command/commands/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/command/commands/exclude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/command/commands/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/command/commands/include.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/command/commands/redo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/command/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/command/commands/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/command/commands/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/command/commands/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/command/commands/talk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/command/commands/undo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/command/commands/undoall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/command/commands/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10136 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14986 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/cost_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/ctags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7715 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/diff_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/edit_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 01:04:02.398613 mentat-1.0.9/mentat/feature_filters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/feature_filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/feature_filters/default_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/feature_filters/embedding_similarity_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/feature_filters/feature_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6598 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/feature_filters/llm_feature_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/feature_filters/truncate_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8327 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/git_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11478 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/include_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16412 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/llm_api_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/logging_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 01:04:02.398613 mentat-1.0.9/mentat/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11253 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/parsers/block_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7558 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/parsers/change_display_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/parsers/diff_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13212 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/parsers/file_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10246 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/parsers/git_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/parsers/json_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17858 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/parsers/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/parsers/parser_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6094 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/parsers/replacement_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8940 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/parsers/unified_diff_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 01:04:02.398613 mentat-1.0.9/mentat/prompts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/prompts/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 01:04:02.398613 mentat-1.0.9/mentat/python_client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/python_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/python_client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 01:04:02.382613 mentat-1.0.9/mentat/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 01:04:02.398613 mentat-1.0.9/mentat/resources/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/resources/conf/conf.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 01:04:02.398613 mentat-1.0.9/mentat/resources/prompts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/resources/prompts/agent_command_selection_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/resources/prompts/agent_file_selection_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/resources/prompts/block_parser_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/resources/prompts/feature_selection_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/resources/prompts/json_parser_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/resources/prompts/replacement_parser_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/resources/prompts/revisor_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/resources/prompts/unified_diff_parser_prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 01:04:02.402613 mentat-1.0.9/mentat/resources/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/resources/templates/benchmark.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/resources/templates/conversation_viewer.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 01:04:02.402613 mentat-1.0.9/mentat/resources/templates/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/resources/templates/css/benchmark.css
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/resources/templates/css/conversation_viewer.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/resources/templates/css/transcript.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 01:04:02.402613 mentat-1.0.9/mentat/resources/templates/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/resources/templates/js/conversation_viewer.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/resources/templates/js/transcript.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/resources/templates/transcript.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 01:04:02.402613 mentat-1.0.9/mentat/revisor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/revisor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/revisor/revisor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 01:04:02.402613 mentat-1.0.9/mentat/sampler/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/sampler/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8946 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/sampler/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/sampler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/sentry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10688 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/session_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/session_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/session_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/streaming_printer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 01:04:02.402613 mentat-1.0.9/mentat/terminal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/terminal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/terminal/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/terminal/loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/terminal/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/terminal/prompt_completer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/terminal/prompt_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/terminal/themes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/transcripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 01:04:02.402613 mentat-1.0.9/mentat/vision/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/vision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-01-19 01:03:42.000000 mentat-1.0.9/mentat/vision/vision_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 01:04:02.394613 mentat-1.0.9/mentat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4987 2024-01-19 01:04:02.000000 mentat-1.0.9/mentat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-01-19 01:04:02.000000 mentat-1.0.9/mentat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-19 01:04:02.000000 mentat-1.0.9/mentat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-01-19 01:04:02.000000 mentat-1.0.9/mentat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-01-19 01:04:02.000000 mentat-1.0.9/mentat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-19 01:04:02.000000 mentat-1.0.9/mentat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-01-19 01:03:42.000000 mentat-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-01-19 01:03:42.000000 mentat-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-19 01:04:02.402613 mentat-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-01-19 01:03:42.000000 mentat-1.0.9/setup.py
```

### Comparing `mentat-1.0.8/LICENSE` & `mentat-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/agent_handler.py` & `mentat-1.0.9/mentat/agent_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,16 @@
             return []
 
         content = response.choices[0].message.content or ""
 
         messages.append(
             ChatCompletionAssistantMessageParam(role="assistant", content=content)
         )
-        ctx.conversation.add_model_message(content, messages)
+        parsed_llm_response = await ctx.config.parser.parse_llm_response(content)
+        ctx.conversation.add_model_message(content, messages, parsed_llm_response)
 
         commands = content.strip().split("\n")
         return commands
 
     async def add_agent_context(self) -> bool:
         """
         Returns whether or not control should be handed back to user
```

### Comparing `mentat-1.0.8/mentat/auto_completer.py` & `mentat-1.0.9/mentat/auto_completer.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,18 +266,20 @@
             last_word = last_word[1:]
 
         completions = [
             (f"`{completion}`", completion) for completion in self._all_file_completions
         ]
         return self._replace_last_word(last_word, completions, position)
 
-    def get_completions(self, buffer: str) -> List[Completion]:
+    def get_completions(
+        self, buffer: str, command_autocomplete: bool = False
+    ) -> List[Completion]:
         """
         Get the auto-completion suggestions for the current user buffer.
         """
         if not buffer.strip():
             return []
 
-        if buffer.startswith("/"):
+        if buffer.startswith("/") and command_autocomplete:
             return self._command_argument_completion(buffer[1:])
         else:
             return self.get_file_completions(buffer)
```

### Comparing `mentat-1.0.8/mentat/broadcast.py` & `mentat-1.0.9/mentat/broadcast.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/code_context.py` & `mentat-1.0.9/mentat/code_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from mentat.code_feature import (
     CodeFeature,
     get_code_message_from_features,
     get_consolidated_feature_refs,
     split_file_into_intervals,
 )
 from mentat.diff_context import DiffContext
-from mentat.errors import PathValidationError, ReturnToUser
+from mentat.errors import PathValidationError
 from mentat.feature_filters.default_filter import DefaultFilter
 from mentat.feature_filters.embedding_similarity_filter import EmbeddingSimilarityFilter
 from mentat.git_handler import get_paths_with_git_diffs
 from mentat.include_files import (
     PathType,
     build_path_tree,
     get_code_features_for_path,
@@ -23,15 +23,19 @@
     get_paths_for_directory,
     is_file_text_encoded,
     match_path_with_patterns,
     print_path_tree,
     validate_and_format_path,
 )
 from mentat.interval import parse_intervals, split_intervals_from_path
-from mentat.llm_api_handler import count_tokens, get_max_tokens, is_context_sufficient
+from mentat.llm_api_handler import (
+    count_tokens,
+    get_max_tokens,
+    raise_if_context_exceeds_max,
+)
 from mentat.session_context import SESSION_CONTEXT
 from mentat.session_stream import SessionStream
 
 
 class CodeContext:
     def __init__(
         self,
@@ -106,14 +110,15 @@
 
     async def get_code_message(
         self,
         prompt_tokens: int,
         prompt: Optional[str] = None,
         expected_edits: Optional[list[str]] = None,  # for training/benchmarking
         loading_multiplier: float = 0.0,
+        suppress_context_check: bool = False,
     ) -> str:
         """
         Retrieves the current code message.
         'prompt' argument is embedded and used to search for similar files when auto-context is enabled.
         If prompt is empty, auto context won't be used.
         'prompt_tokens' argument is the total number of tokens used by the prompt before the code message,
         used to ensure that the code message won't overflow the model's context size
@@ -145,16 +150,16 @@
         ]
         include_files_message = get_code_message_from_features(include_features)
         include_files_tokens = count_tokens(
             "\n".join(include_files_message), model, full_message=False
         )
 
         tokens_used = prompt_tokens + meta_tokens + include_files_tokens
-        if not is_context_sufficient(tokens_used):
-            raise ReturnToUser()
+        if not suppress_context_check:
+            raise_if_context_exceeds_max(tokens_used)
         auto_tokens = min(
             get_max_tokens() - tokens_used - config.token_buffer,
             config.auto_context_tokens,
         )
 
         # Get auto included features
         if config.auto_context_tokens > 0 and prompt:
```

### Comparing `mentat-1.0.8/mentat/code_edit_feedback.py` & `mentat-1.0.9/mentat/code_edit_feedback.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/code_feature.py` & `mentat-1.0.9/mentat/code_feature.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/code_file_manager.py` & `mentat-1.0.9/mentat/code_file_manager.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/command/command.py` & `mentat-1.0.9/mentat/command/command.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/command/commands/__init__.py` & `mentat-1.0.9/mentat/command/commands/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # ruff: noqa: F401
 # type: ignore
 
 # Import all of the commands so that they are initialized
 from .agent import AgentCommand
+from .amend import AmendCommand
 from .clear import ClearCommand
 from .commit import CommitCommand
 from .config import ConfigCommand
 from .context import ContextCommand
 from .exclude import ExcludeCommand
 from .help import HelpCommand
 from .include import IncludeCommand
```

### Comparing `mentat-1.0.8/mentat/command/commands/agent.py` & `mentat-1.0.9/mentat/command/commands/agent.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/command/commands/clear.py` & `mentat-1.0.9/mentat/command/commands/clear.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/command/commands/commit.py` & `mentat-1.0.9/mentat/command/commands/commit.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/command/commands/config.py` & `mentat-1.0.9/mentat/command/commands/config.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/command/commands/context.py` & `mentat-1.0.9/mentat/command/commands/context.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/command/commands/exclude.py` & `mentat-1.0.9/mentat/command/commands/exclude.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/command/commands/help.py` & `mentat-1.0.9/mentat/command/commands/help.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/command/commands/include.py` & `mentat-1.0.9/mentat/command/commands/include.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/command/commands/redo.py` & `mentat-1.0.9/mentat/command/commands/undo.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 from typing_extensions import override
 
 from mentat.command.command import Command, CommandArgument
 from mentat.session_context import SESSION_CONTEXT
 
 
-class RedoCommand(Command, command_name="redo"):
+class UndoCommand(Command, command_name="undo"):
     @override
     async def apply(self, *args: str) -> None:
         session_context = SESSION_CONTEXT.get()
         stream = session_context.stream
         code_file_manager = session_context.code_file_manager
 
-        errors = await code_file_manager.history.redo()
+        errors = code_file_manager.history.undo()
         if errors:
             stream.send(errors)
-        stream.send("Redo complete", style="success")
+        stream.send("Undo complete", style="success")
 
     @override
     @classmethod
     def arguments(cls) -> List[CommandArgument]:
         return []
 
     @override
@@ -29,8 +29,8 @@
         cls, arguments: list[str], argument_position: int
     ) -> list[str]:
         return []
 
     @override
     @classmethod
     def help_message(cls) -> str:
-        return "Redo the last change made by Mentat."
+        return "Undo the last change made by Mentat."
```

### Comparing `mentat-1.0.8/mentat/command/commands/run.py` & `mentat-1.0.9/mentat/command/commands/run.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/command/commands/sample.py` & `mentat-1.0.9/mentat/command/commands/sample.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/command/commands/screenshot.py` & `mentat-1.0.9/mentat/command/commands/screenshot.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,8 +58,8 @@
         cls, arguments: list[str], argument_position: int
     ) -> list[str]:
         return get_command_filename_completions(arguments[-1])
 
     @override
     @classmethod
     def help_message(cls) -> str:
-        return "Open a url or local file in Chrome and take a screenshot."
+        return "Open a url or local file in a web browser and take a screenshot."
```

### Comparing `mentat-1.0.8/mentat/command/commands/search.py` & `mentat-1.0.9/mentat/command/commands/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
                         included_paths = code_context.include_features(features)
                         for included_path in included_paths:
                             rel_path = get_relative_path(
                                 included_path, session_context.cwd
                             )
                             stream.send(f"{rel_path} added to context", style="success")
                     else:
-                        stream.send("(Y/n)")
+                        stream.send("(Y/n)", style="input")
                     user_input: str = (
                         await collect_user_input(plain=True)
                     ).data.strip()
                 if user_input.lower() == "n":
                     stream.send("Exiting search mode...", style="input")
                     break
```

### Comparing `mentat-1.0.8/mentat/command/commands/talk.py` & `mentat-1.0.9/mentat/command/commands/talk.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/command/commands/undo.py` & `mentat-1.0.9/mentat/command/commands/undoall.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 from typing_extensions import override
 
 from mentat.command.command import Command, CommandArgument
 from mentat.session_context import SESSION_CONTEXT
 
 
-class UndoCommand(Command, command_name="undo"):
+class UndoAllCommand(Command, command_name="undo-all"):
     @override
     async def apply(self, *args: str) -> None:
         session_context = SESSION_CONTEXT.get()
         stream = session_context.stream
         code_file_manager = session_context.code_file_manager
 
-        errors = code_file_manager.history.undo()
+        errors = code_file_manager.history.undo_all()
         if errors:
             stream.send(errors)
-        stream.send("Undo complete", style="success")
+        stream.send("Undos complete", style="success")
 
     @override
     @classmethod
     def arguments(cls) -> List[CommandArgument]:
         return []
 
     @override
@@ -29,8 +29,8 @@
         cls, arguments: list[str], argument_position: int
     ) -> list[str]:
         return []
 
     @override
     @classmethod
     def help_message(cls) -> str:
-        return "Undo the last change made by Mentat."
+        return "Undo all changes made by Mentat."
```

### Comparing `mentat-1.0.8/mentat/command/commands/undoall.py` & `mentat-1.0.9/mentat/command/commands/redo.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 from typing_extensions import override
 
 from mentat.command.command import Command, CommandArgument
 from mentat.session_context import SESSION_CONTEXT
 
 
-class UndoAllCommand(Command, command_name="undo-all"):
+class RedoCommand(Command, command_name="redo"):
     @override
     async def apply(self, *args: str) -> None:
         session_context = SESSION_CONTEXT.get()
         stream = session_context.stream
         code_file_manager = session_context.code_file_manager
 
-        errors = code_file_manager.history.undo_all()
+        errors = await code_file_manager.history.redo()
         if errors:
             stream.send(errors)
-        stream.send("Undos complete", style="success")
+        stream.send("Redo complete", style="success")
 
     @override
     @classmethod
     def arguments(cls) -> List[CommandArgument]:
         return []
 
     @override
@@ -29,8 +29,8 @@
         cls, arguments: list[str], argument_position: int
     ) -> list[str]:
         return []
 
     @override
     @classmethod
     def help_message(cls) -> str:
-        return "Undo all changes made by Mentat."
+        return "Redo a change that was previously undone with /undo."
```

### Comparing `mentat-1.0.8/mentat/command/commands/viewer.py` & `mentat-1.0.9/mentat/command/commands/viewer.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/config.py` & `mentat-1.0.9/mentat/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
     maximum_context: int | None = attr.field(
         default=None,
         metadata={
             "description": (
                 "The maximum number of lines of context to include in the prompt. It is"
                 " inferred automatically for openai models but you can still set it to"
-                " save costs. It must be set for other models."
+                " save costs. If not set for non-openai models, it defaults to 4096."
             ),
         },
         converter=int_or_none,
         validator=validators.optional(validators.ge(0)),
     )
     token_buffer: int = attr.field(
         default=1000,
@@ -94,14 +94,35 @@
                 "Whether to include the parser prompt in the system message. This"
                 " should only be set to true for fine tuned models."
             ),
             "auto_completions": bool_autocomplete,
         },
         converter=converters.optional(converters.to_bool),
     )
+    revisor: bool = attr.field(
+        default=False,
+        metadata={
+            "description": (
+                "Enables or disables a revisor tweaking model edits after they're made."
+                " The revisor will use the same model regular edits do."
+            ),
+            "auto_completions": bool_autocomplete,
+        },
+        converter=converters.optional(converters.to_bool),
+    )
+    sampler: bool = attr.field(
+        default=False,
+        metadata={
+            "description": (
+                "Automatically saves a git diff snapshot for the sampler on startup."
+            ),
+            "auto_completions": bool_autocomplete,
+        },
+        converter=converters.optional(converters.to_bool),
+    )
 
     # Context specific settings
     file_exclude_glob_list: list[str] = attr.field(
         factory=list,
         metadata={"description": "List of glob patterns to exclude from context"},
     )
     auto_context_tokens: int = attr.field(  # pyright: ignore
```

### Comparing `mentat-1.0.8/mentat/conversation.py` & `mentat-1.0.9/mentat/conversation.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,14 +24,18 @@
 from mentat.parsers.file_edit import FileEdit
 from mentat.parsers.parser import ParsedLLMResponse
 from mentat.session_context import SESSION_CONTEXT
 from mentat.transcripts import ModelMessage, TranscriptMessage, UserMessage
 from mentat.utils import add_newline
 
 
+class MentatAssistantMessageParam(ChatCompletionAssistantMessageParam):
+    parsed_llm_response: ParsedLLMResponse
+
+
 class Conversation:
     def __init__(self):
         self._messages = list[ChatCompletionMessageParam]()
 
         # This contains a list of messages used for transcripts
         self.literal_messages = list[TranscriptMessage]()
 
@@ -56,15 +60,16 @@
                 )
 
         messages = self.get_messages()
         code_message = await code_context.get_code_message(
             prompt_tokens(
                 messages,
                 config.model,
-            )
+            ),
+            suppress_context_check=True,
         )
         messages.append(
             ChatCompletionSystemMessageParam(
                 role="system",
                 content=code_message,
             )
         )
@@ -78,15 +83,15 @@
                 (False, False): " is close to",
                 (False, True): " exceeds",
                 (True, False): "s are close to",
                 (True, True): "s exceed",
             }
             stream.send(
                 f"Included file{message[(_plural, _exceed)]} token limit"
-                f" ({tokens} / {context_size}). Truncating based on task similarity.",
+                f" ({tokens} / {context_size}).",
                 style="warning",
             )
         else:
             stream.send(
                 f"Prompt and included files token count: {tokens} / {context_size}",
                 style="info",
             )
@@ -114,60 +119,83 @@
                     },
                 },
             ]
         self.add_transcript_message(UserMessage(message=content, prior_messages=None))
         self.add_message(ChatCompletionUserMessageParam(role="user", content=content))
 
     def add_model_message(
-        self, message: str, messages_snapshot: list[ChatCompletionMessageParam]
+        self,
+        message: str,
+        messages_snapshot: list[ChatCompletionMessageParam],
+        parsed_llm_response: ParsedLLMResponse,
     ):
         """Used for actual model output messages"""
         self.add_transcript_message(
             ModelMessage(message=message, prior_messages=messages_snapshot)
         )
         self.add_message(
-            ChatCompletionAssistantMessageParam(role="assistant", content=message)
+            MentatAssistantMessageParam(
+                parsed_llm_response=parsed_llm_response,
+                role="assistant",
+                content=message,
+            )
         )
 
     def add_message(self, message: ChatCompletionMessageParam):
         """Used for adding messages to the models conversation. Does not add a left-side message to the transcript!"""
         self._messages.append(message)
 
     def get_messages(
-        self, include_system_prompt: bool = True
+        self,
+        include_system_prompt: bool = True,
+        include_parsed_llm_responses: bool = False,
     ) -> list[ChatCompletionMessageParam]:
         """Returns the messages in the conversation. The system message may change throughout
-        the conversation so it is important to access the messages through this method.
+        the conversation and messages may contain additional metadata not supported by the API,
+        so it is important to access the messages through this method.
         """
         session_context = SESSION_CONTEXT.get()
         config = session_context.config
+
+        _messages = [
+            (  # Remove metadata from messages by default
+                ChatCompletionAssistantMessageParam(
+                    role=msg["role"], content=msg.get("content")
+                )
+                if msg["role"] == "assistant" and include_parsed_llm_responses is False
+                else msg
+            )
+            for msg in self._messages.copy()
+        ]
+
         if config.no_parser_prompt or not include_system_prompt:
-            return self._messages.copy()
+            return _messages
         else:
             parser = config.parser
             prompt = parser.get_system_prompt()
             prompt_message: ChatCompletionMessageParam = (
                 ChatCompletionSystemMessageParam(
                     role="system",
                     content=prompt,
                 )
             )
-            return [prompt_message] + self._messages.copy()
+            return [prompt_message] + _messages
 
     def clear_messages(self) -> None:
         """Clears the messages in the conversation"""
         self._messages = list[ChatCompletionMessageParam]()
 
     async def _stream_model_response(
         self,
         messages: list[ChatCompletionMessageParam],
         loading_multiplier: float = 0.0,
     ) -> ParsedLLMResponse:
         session_context = SESSION_CONTEXT.get()
         stream = session_context.stream
+        code_file_manager = session_context.code_file_manager
         config = session_context.config
         parser = config.parser
         llm_api_handler = session_context.llm_api_handler
         cost_tracker = session_context.cost_tracker
 
         if loading_multiplier:
             stream.send(
@@ -200,14 +228,19 @@
             )
 
         stream.send("Streaming... use control-c to interrupt the model at any point\n")
         async with parser.interrupt_catcher():
             parsed_llm_response = await parser.stream_and_parse_llm_response(
                 add_newline(response)
             )
+        # Sampler and History require previous_file_lines
+        for file_edit in parsed_llm_response.file_edits:
+            file_edit.previous_file_lines = code_file_manager.file_lines.get(
+                file_edit.file_path, []
+            )
         if not parsed_llm_response.interrupted:
             cost_tracker.display_last_api_call()
         else:
             # Generator doesn't log the api call if we interrupt it
             cost_tracker.log_api_call_stats(
                 num_prompt_tokens,
                 count_tokens(
@@ -218,29 +251,31 @@
             )
 
         messages.append(
             ChatCompletionAssistantMessageParam(
                 role="assistant", content=parsed_llm_response.full_response
             )
         )
-        self.add_model_message(parsed_llm_response.full_response, messages)
+        self.add_model_message(
+            parsed_llm_response.full_response, messages, parsed_llm_response
+        )
 
         return parsed_llm_response
 
     async def get_model_response(self) -> ParsedLLMResponse:
         session_context = SESSION_CONTEXT.get()
         stream = session_context.stream
         config = session_context.config
         code_context = session_context.code_context
 
         messages_snapshot = self.get_messages()
 
         # Get current code message
         loading_multiplier = 1.0 if config.auto_context_tokens > 0 else 0.0
-        prompt = messages_snapshot[-1]["content"]
+        prompt = messages_snapshot[-1].get("content")
         if isinstance(prompt, list):
             text_prompts = [
                 p.get("text", "") for p in prompt if p.get("type") == "text"
             ]
             prompt = " ".join(text_prompts)
         code_message = await code_context.get_code_message(
             prompt_tokens(messages_snapshot, config.model),
@@ -248,15 +283,16 @@
                 prompt  # Prompt can be image as well as text
                 if isinstance(prompt, str)
                 else ""
             ),
             loading_multiplier=0.5 * loading_multiplier,
         )
         messages_snapshot.insert(
-            1, ChatCompletionSystemMessageParam(role="system", content=code_message)
+            0 if config.no_parser_prompt else 1,
+            ChatCompletionSystemMessageParam(role="system", content=code_message),
         )
 
         try:
             response = await self._stream_model_response(
                 messages_snapshot,
                 loading_multiplier=0.5 * loading_multiplier,
             )
@@ -341,7 +377,25 @@
         else:
             ctx.stream.send(
                 "Not enough tokens remaining in model's context to add command output"
                 " to model context.",
                 style="error",
             )
             return False
+
+    def _get_user_message(self, message: ChatCompletionUserMessageParam) -> str:
+        if not message["content"]:
+            return ""
+        elif isinstance(message["content"], str):
+            return message["content"]
+        else:
+            full = ""
+            for part in message["content"]:
+                if part["type"] == "text":
+                    full += part["text"]
+            return full
+
+    def amend(self) -> Optional[str]:
+        for i, message in reversed(list(enumerate(self._messages))):
+            if message["role"] == "user" and self._get_user_message(message):
+                self._messages = self._messages[:i]
+                return self._get_user_message(message)
```

### Comparing `mentat-1.0.8/mentat/cost_tracker.py` & `mentat-1.0.9/mentat/cost_tracker.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/ctags.py` & `mentat-1.0.9/mentat/ctags.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/diff_context.py` & `mentat-1.0.9/mentat/diff_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import subprocess
 from pathlib import Path
 from typing import List, Literal, Optional
 
 import attr
 
-from mentat.errors import UserError
+from mentat.errors import MentatError
 from mentat.git_handler import (
     check_head_exists,
     get_diff_for_file,
     get_files_in_diff,
     get_treeish_metadata,
 )
 from mentat.interval import Interval
@@ -30,29 +30,29 @@
 
 
 def parse_diff(diff: str) -> list[DiffAnnotation]:
     """Parse diff into a list of annotations."""
     annotations: list[DiffAnnotation] = []
     active_annotation: Optional[DiffAnnotation] = None
     lines = diff.splitlines()
-    for line in lines[4:]:  # Ignore header
-        if line.startswith(("---", "+++", "//")):
+    for line in lines:
+        if line.startswith(("---", "+++", "//", "diff", "index")):
             continue
         elif line.startswith("@@"):
             if active_annotation:
                 annotations.append(active_annotation)
             _new_index = line.split(" ")[2]
             if "," in _new_index:
                 new_start = _new_index[1:].split(",")[0]
             else:
                 new_start = _new_index[1:]
             active_annotation = DiffAnnotation(start=int(new_start), message=[])
         elif line.startswith(("+", "-")):
             if not active_annotation:
-                raise UserError("Invalid diff")
+                raise MentatError("Invalid diff")
             active_annotation.message.append(line)
     if active_annotation:
         annotations.append(active_annotation)
     annotations.sort(key=lambda a: a.start)
     return annotations
```

### Comparing `mentat-1.0.8/mentat/edit_history.py` & `mentat-1.0.9/mentat/edit_history.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/embeddings.py` & `mentat-1.0.9/mentat/embeddings.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,121 +1,121 @@
-import json
-import os
-import sqlite3
-from pathlib import Path
 from timeit import default_timer
 
-import numpy as np
+import chromadb
+from chromadb.api.types import Embeddable, EmbeddingFunction, Embeddings
 
 from mentat.code_feature import CodeFeature, count_feature_tokens
 from mentat.errors import MentatError
-from mentat.llm_api_handler import (
-    count_tokens,
-    model_context_size,
-    model_price_per_1000_tokens,
-)
+from mentat.llm_api_handler import model_context_size, model_price_per_1000_tokens
 from mentat.session_context import SESSION_CONTEXT
 from mentat.session_input import ask_yes_no
-from mentat.utils import mentat_dir_path, sha256
+from mentat.utils import mentat_dir_path
 
 EMBEDDINGS_API_BATCH_SIZE = 2048
 
+client = chromadb.PersistentClient(path=str(mentat_dir_path / "chroma"))
 
-class EmbeddingsDatabase:
-    def __init__(self, output_dir: Path | None = None):
-        self.output_dir = output_dir or mentat_dir_path
-        os.makedirs(self.output_dir, exist_ok=True)
-        self.path = Path(self.output_dir) / "embeddings.sqlite3"
-        self._connect()
-
-    def _connect(self):
-        self.conn = sqlite3.connect(self.path)
-        with self.conn as db:
-            db.execute(
-                "CREATE TABLE IF NOT EXISTS embeddings "
-                "(checksum TEXT PRIMARY KEY, vector BLOB)"
-            )
 
-    def set(self, items: dict[str, list[float]]):
-        with self.conn as db:
-            db.executemany(
-                "INSERT OR REPLACE INTO embeddings (checksum, vector) VALUES (?, ?)",
-                [
-                    (key, sqlite3.Binary(json.dumps(value).encode("utf-8")))
-                    for key, value in items.items()
-                ],
-            )
+class MentatEmbeddingFunction(EmbeddingFunction[Embeddable]):
+    def __call__(self, input: Embeddable) -> Embeddings:
+        if not all(isinstance(item, str) for item in input):
+            raise MentatError("MentatEmbeddings only enabled for text files")
+        session_context = SESSION_CONTEXT.get()
+        config = session_context.config
+        llm_api_handler = session_context.llm_api_handler
 
-    def get(self, keys: list[str]) -> dict[str, list[float]]:
-        with self.conn as db:
-            cursor = db.execute(
-                "SELECT checksum, vector FROM embeddings WHERE checksum IN"
-                f" ({','.join(['?']*len(keys))})",
-                keys,
+        n_batches = (
+            0 if len(input) == 0 else len(input) // EMBEDDINGS_API_BATCH_SIZE + 1
+        )
+        output: Embeddings = []
+        for batch in range(n_batches):
+            i_start, i_end = (
+                batch * EMBEDDINGS_API_BATCH_SIZE,
+                (batch + 1) * EMBEDDINGS_API_BATCH_SIZE,
             )
-            return {row[0]: json.loads(row[1]) for row in cursor.fetchall()}
-
-    def exists(self, key: str) -> bool:
-        with self.conn as db:
-            cursor = db.execute("SELECT 1 FROM embeddings WHERE checksum=?", (key,))
-            return cursor.fetchone() is not None
+            response = llm_api_handler.call_embedding_api(
+                input[i_start:i_end], config.embedding_model
+            )
+            output += response
+        return output
 
-    def __del__(self):
-        self.conn.close()
 
+class Collection:
+    def __init__(self, embedding_model: str):
+        self._collection = client.get_or_create_collection(
+            name=f"mentat-{embedding_model}",
+            embedding_function=MentatEmbeddingFunction(),
+        )
 
-database = EmbeddingsDatabase()
+    def exists(self, id: str) -> bool:
+        assert self._collection is not None, "Collection not initialized"
+        return len(self._collection.get(id)["ids"]) > 0
+
+    def add(self, checksums: list[str], texts: list[str]) -> None:
+        assert self._collection is not None, "Collection not initialized"
+        return self._collection.add(  # type: ignore
+            ids=checksums,
+            documents=texts,
+            metadatas=[{"active": False} for _ in checksums],
+        )
 
+    def query(self, prompt: str, checksums: list[str]) -> dict[str, float]:
+        assert self._collection is not None, "Collection not initialized"
 
-def _cosine_similarity(v1: list[float], v2: list[float]) -> float:
-    """Calculate the cosine similarity between two vectors."""
-    dot_product = np.dot(v1, v2)
-    norm_v1 = np.linalg.norm(v1)
-    norm_v2 = np.linalg.norm(v2)
-    return dot_product / (norm_v1 * norm_v2)  # pyright: ignore
+        self._collection.update(  # type: ignore
+            ids=checksums,
+            metadatas=[{"active": True} for _ in checksums],
+        )
+        results = self._collection.query(  # type: ignore
+            query_texts=[prompt],
+            where={"active": True},
+            n_results=len(checksums) + 1,
+        )
+        self._collection.update(  # type: ignore
+            ids=checksums,
+            metadatas=[{"active": False} for _ in checksums],
+        )
+        assert results["distances"], "Error calculating distances"
+        return {c: e for c, e in zip(results["ids"][0], results["distances"][0])}
 
 
 async def get_feature_similarity_scores(
     prompt: str,
     features: list[CodeFeature],
     loading_multiplier: float = 0.0,
 ) -> list[float]:
     """Return the similarity scores for a given prompt and list of features."""
-    global database
     session_context = SESSION_CONTEXT.get()
     stream = session_context.stream
+    config = session_context.config
     cost_tracker = session_context.cost_tracker
     embedding_model = session_context.config.embedding_model
-    llm_api_handler = session_context.llm_api_handler
 
-    max_model_tokens = model_context_size(embedding_model)
+    max_model_tokens = model_context_size(config.embedding_model)
     if max_model_tokens is None:
         raise MentatError(f"Missing model context size for {embedding_model}.")
-    prompt_tokens = count_tokens(prompt, embedding_model, False)
-    if prompt_tokens > max_model_tokens:
-        stream.send(
-            f"Warning: Prompt contains {prompt_tokens} tokens, but the model"
-            f" can only handle {max_model_tokens} tokens. Ignoring embeddings."
-        )
-        return [0.0 for _ in features]
 
-    prompt_checksum = sha256(prompt)
+    # Initialize DB
+    collection = Collection(embedding_model)
+
+    # Identify which items need embeddings.
     checksums: list[str] = [f.get_checksum() for f in features]
     tokens: list[int] = await count_feature_tokens(features, embedding_model)
     embed_texts = list[str]()
     embed_checksums = list[str]()
     embed_tokens = list[int]()
-    if not database.exists(prompt_checksum):
-        embed_texts.append(prompt)
-        embed_checksums.append(prompt_checksum)
-        embed_tokens.append(prompt_tokens)
     for feature, checksum, token in zip(features, checksums, tokens):
         if token > max_model_tokens:
+            stream.send(
+                f"Warning: Feature {str(feature)} has {token} tokens, which exceeds the"
+                f" maximum of {max_model_tokens} for model {config.embedding_model}."
+                " Skipping."
+            )
             continue
-        if not database.exists(checksum):
+        if not collection.exists(checksum) and checksum not in embed_checksums:
             embed_texts.append("\n".join(feature.get_code_message()))
             embed_checksums.append(checksum)
             embed_tokens.append(token)
 
     # If it costs more than $1, get confirmation from user.
     cost = model_price_per_1000_tokens(embedding_model)
     if cost is None:
@@ -130,46 +130,34 @@
                 f"Embedding {sum(embed_tokens)} tokens will cost ${cost[0]:.2f}."
                 " Continue anyway?"
             )
             if not await ask_yes_no(default_yes=True):
                 stream.send("Ignoring embeddings for now.")
                 return [0.0 for _ in checksums]
 
-    # Fetch embeddings in batches
-    if len(embed_texts) == 0:
-        n_batches = 0
-    else:
-        n_batches = len(embed_texts) // EMBEDDINGS_API_BATCH_SIZE + 1
-    for batch in range(n_batches):
+    # Load embeddings
+    if embed_texts:
+        start_time = default_timer()
         if loading_multiplier:
             stream.send(
-                f"Fetching embeddings, batch {batch+1}/{n_batches}",
+                f"Fetching embeddings for {len(embed_texts)} documents",
                 channel="loading",
-                progress=(100 / n_batches) * loading_multiplier,
+                progress=50 * loading_multiplier,
             )
-        start_time = default_timer()
-        i_start, i_end = (
-            batch * EMBEDDINGS_API_BATCH_SIZE,
-            (batch + 1) * EMBEDDINGS_API_BATCH_SIZE,
-        )
-        _texts = embed_texts[i_start:i_end]
-        _checksums = embed_checksums[i_start:i_end]
-        _tokens = embed_tokens[i_start:i_end]
-
-        response = await llm_api_handler.call_embedding_api(_texts, embedding_model)
+        collection.add(embed_checksums, embed_texts)
         cost_tracker.log_api_call_stats(
-            sum(_tokens),
+            sum(embed_tokens),
             0,
             embedding_model,
             start_time - default_timer(),
         )
-        database.set({k: v for k, v in zip(_checksums, response)})
-
-    # Calculate similarity score for each feature
-    prompt_embedding = database.get([prompt_checksum])[prompt_checksum]
-    embeddings = database.get(checksums)
-    scores = [
-        _cosine_similarity(prompt_embedding, embeddings[k]) if k in embeddings else 0.0
-        for k in checksums
-    ]
 
-    return scores
+    # Get similarity scores
+    if loading_multiplier:
+        stream.send(
+            "Matching relevant documents based on embedding similarity",
+            channel="loading",
+            progress=(50 if embed_texts else 100) * loading_multiplier,
+        )
+    _checksums = list(set(checksums))
+    scores = collection.query(prompt, _checksums)
+    return [scores.get(f.get_checksum(), 0) for f in features]
```

### Comparing `mentat-1.0.8/mentat/errors.py` & `mentat-1.0.9/mentat/errors.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/feature_filters/default_filter.py` & `mentat-1.0.9/mentat/feature_filters/default_filter.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/feature_filters/embedding_similarity_filter.py` & `mentat-1.0.9/mentat/feature_filters/embedding_similarity_filter.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         if self.query == "":
             return [(f, 0.0) for f in features]
 
         sim_scores = await get_feature_similarity_scores(
             self.query, features, self.loading_multiplier
         )
         features_scored = zip(features, sim_scores)
-        return sorted(features_scored, key=lambda x: x[1], reverse=True)
+        return sorted(features_scored, key=lambda x: x[1])
 
     async def filter(
         self,
         features: list[CodeFeature],
     ) -> list[CodeFeature]:
         if self.query == "":
             return features
```

### Comparing `mentat-1.0.8/mentat/feature_filters/feature_filter.py` & `mentat-1.0.9/mentat/feature_filters/feature_filter.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/feature_filters/llm_feature_filter.py` & `mentat-1.0.9/mentat/feature_filters/llm_feature_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,13 +154,13 @@
                         in_feat.path == feature.path and in_feat.interval.intersects
                         for in_feat in preselected_features
                     )
                     postselected_features.add(feature)
             except (PathValidationError, AssertionError):
                 stream.send(
                     f"LLM selected invalid path: {selected_ref}, skipping.",
-                    color="light_yellow",
+                    style="warning",
                 )
 
         # Truncate again to enforce max_tokens
         truncate_filter = TruncateFilter(self.max_tokens, config.model)
         return await truncate_filter.filter(postselected_features)
```

### Comparing `mentat-1.0.8/mentat/feature_filters/truncate_filter.py` & `mentat-1.0.9/mentat/feature_filters/truncate_filter.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/git_handler.py` & `mentat-1.0.9/mentat/git_handler.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/include_files.py` & `mentat-1.0.9/mentat/include_files.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/interval.py` & `mentat-1.0.9/mentat/interval.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/llm_api_handler.py` & `mentat-1.0.9/mentat/llm_api_handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import base64
 import io
 import os
 import sys
+from inspect import iscoroutinefunction
 from pathlib import Path
 from timeit import default_timer
 from typing import (
     Any,
     AsyncIterator,
     Callable,
     Dict,
@@ -17,21 +18,24 @@
     cast,
     overload,
 )
 
 import attr
 import sentry_sdk
 import tiktoken
+from chromadb.api.types import Embeddings
 from dotenv import load_dotenv
 from openai import (
     APIConnectionError,
     AsyncAzureOpenAI,
     AsyncOpenAI,
     AsyncStream,
     AuthenticationError,
+    AzureOpenAI,
+    OpenAI,
 )
 from openai.types.chat import (
     ChatCompletion,
     ChatCompletionChunk,
     ChatCompletionContentPartParam,
     ChatCompletionMessageParam,
 )
@@ -59,62 +63,83 @@
     """Decorator that should be used on any function that calls the OpenAI API
 
     It does two things:
     1. Raises if the function is called in tests (that aren't benchmarks)
     2. Converts APIConnectionErrors to MentatErrors
     """
 
-    async def wrapper(*args: Any, **kwargs: Any) -> Any:
-        assert (
-            not is_test_environment()
-        ), "OpenAI call attempted in non-benchmark test environment!"
-        try:
-            return await func(*args, **kwargs)
-        except APIConnectionError:
-            raise MentatError(
-                "API connection error: please check your internet connection and try"
-                " again."
-            )
+    if iscoroutinefunction(func):
+
+        async def async_wrapper(*args: Any, **kwargs: Any) -> Any:
+            assert (
+                not is_test_environment()
+            ), "OpenAI call attempted in non-benchmark test environment!"
+            try:
+                return await func(*args, **kwargs)
+            except APIConnectionError:
+                raise MentatError(
+                    "API connection error: please check your internet connection and"
+                    " try again."
+                )
+
+        return async_wrapper
+    else:
+
+        def sync_wrapper(*args: Any, **kwargs: Any) -> Any:
+            assert (
+                not is_test_environment()
+            ), "OpenAI call attempted in non-benchmark test environment!"
+            try:
+                return func(*args, **kwargs)
+            except APIConnectionError:
+                raise MentatError(
+                    "API connection error: please check your internet connection and"
+                    " try again."
+                )
 
-    return wrapper
+        return sync_wrapper
 
 
 # Ensures that each chunk will have at most one newline character
 def chunk_to_lines(chunk: ChatCompletionChunk) -> list[str]:
     content = None
     if len(chunk.choices) > 0:
         content = chunk.choices[0].delta.content
     return ("" if content is None else content).splitlines(keepends=True)
 
 
+def get_encoding_for_model(model: str) -> tiktoken.Encoding:
+    try:
+        # OpenAI fine-tuned models are named `ft:<base model>:<name>:<id>`. If tiktoken
+        # can't match the full string, it tries to match on startswith, e.g. 'gpt-4'
+        _model = model.split(":")[1] if model.startswith("ft:") else model
+        return tiktoken.encoding_for_model(_model)
+    except KeyError:
+        return tiktoken.get_encoding("cl100k_base")
+
+
 def count_tokens(message: str, model: str, full_message: bool) -> int:
     """
     Calculates the tokens in this message. Will NOT be accurate for a full prompt!
     Use prompt_tokens to get the exact amount of tokens for a prompt.
     If full_message is true, will include the extra 4 tokens used in a chat completion by this message
     if this message is part of a prompt. You do NOT want full_message to be true for a response.
     """
-    try:
-        encoding = tiktoken.encoding_for_model(model)
-    except KeyError:
-        encoding = tiktoken.get_encoding("cl100k_base")
+    encoding = get_encoding_for_model(model)
     return len(encoding.encode(message, disallowed_special=())) + (
         4 if full_message else 0
     )
 
 
 def prompt_tokens(messages: list[ChatCompletionMessageParam], model: str):
     """
     Returns the number of tokens used by a prompt if it was sent to OpenAI for a chat completion.
     Adapted from https://platform.openai.com/docs/guides/text-generation/managing-tokens
     """
-    try:
-        encoding = tiktoken.encoding_for_model(model)
-    except KeyError:
-        encoding = tiktoken.get_encoding("cl100k_base")
+    encoding = get_encoding_for_model(model)
 
     num_tokens = 0
     for message in messages:
         # every message follows <|start|>{role/name}\n{content}<|end|>\n
         # this has 5 tokens (start token, role, \n, end token, \n), but we count the role token later
         num_tokens += 4
         for key, value in message.items():
@@ -149,32 +174,63 @@
     name: str = attr.field()
     context_size: int = attr.field()
     input_cost: float = attr.field()
     output_cost: float = attr.field()
     embedding_model: bool = attr.field(default=False)
 
 
-known_models: Dict[str, Model] = {
-    "gpt-4-1106-preview": Model("gpt-4-1106-preview", 128000, 0.01, 0.03),
-    "gpt-4-vision-preview": Model("gpt-4-vision-preview", 128000, 0.01, 0.03),
-    "gpt-4": Model("gpt-4", 8192, 0.03, 0.06),
-    "gpt-4-32k": Model("gpt-4-32k", 32768, 0.06, 0.12),
-    "gpt-4-0613": Model("gpt-4-0613", 8192, 0.03, 0.06),
-    "gpt-4-32k-0613": Model("gpt-4-32k-0613", 32768, 0.06, 0.12),
-    "gpt-4-0314": Model("gpt-4-0314", 8192, 0.03, 0.06),
-    "gpt-4-32k-0314": Model("gpt-4-32k-0314", 32768, 0.06, 0.12),
-    "gpt-3.5-turbo-1106": Model("gpt-3.5-turbo-1106", 16385, 0.001, 0.002),
-    "gpt-3.5-turbo": Model("gpt-3.5-turbo", 16385, 0.001, 0.002),
-    "gpt-3.5-turbo-0613": Model("gpt-3.5-turbo-0613", 4096, 0.0015, 0.002),
-    "gpt-3.5-turbo-16k-0613": Model("gpt-3.5-turbo-16k-0613", 16385, 0.003, 0.004),
-    "gpt-3.5-turbo-0301": Model("gpt-3.5-turbo-0301", 4096, 0.0015, 0.002),
-    "text-embedding-ada-002": Model(
-        "text-embedding-ada-002", 8191, 0.0001, 0, embedding_model=True
-    ),
-}
+class ModelsIndex(Dict[str, Model]):
+    def __init__(self, models: Dict[str, Model]):
+        super().update(models)
+
+    def _validate_key(self, key: str) -> str:
+        """Try to match fine-tuned models to their base models."""
+        if not super().__contains__(key) and key.startswith("ft:"):
+            base_model = key.split(":")[
+                1
+            ]  # e.g. "ft:gpt-3.5-turbo-1106:abante::8dsQMc4F"
+            if super().__contains__(base_model):
+                ctx = SESSION_CONTEXT.get()
+                ctx.stream.send(
+                    f"Using base model {base_model} for size and cost estimates.",
+                    style="info",
+                )
+                super().__setitem__(
+                    key, attr.evolve(super().__getitem__(base_model), name=key)
+                )
+                return key
+        return key
+
+    def __getitem__(self, key: str) -> Model:
+        return super().__getitem__(self._validate_key(key))
+
+    def __contains__(self, key: object) -> bool:
+        return super().__contains__(self._validate_key(str(key)))
+
+
+known_models = ModelsIndex(
+    {
+        "gpt-4-1106-preview": Model("gpt-4-1106-preview", 128000, 0.01, 0.03),
+        "gpt-4-vision-preview": Model("gpt-4-vision-preview", 128000, 0.01, 0.03),
+        "gpt-4": Model("gpt-4", 8192, 0.03, 0.06),
+        "gpt-4-32k": Model("gpt-4-32k", 32768, 0.06, 0.12),
+        "gpt-4-0613": Model("gpt-4-0613", 8192, 0.03, 0.06),
+        "gpt-4-32k-0613": Model("gpt-4-32k-0613", 32768, 0.06, 0.12),
+        "gpt-4-0314": Model("gpt-4-0314", 8192, 0.03, 0.06),
+        "gpt-4-32k-0314": Model("gpt-4-32k-0314", 32768, 0.06, 0.12),
+        "gpt-3.5-turbo-1106": Model("gpt-3.5-turbo-1106", 16385, 0.001, 0.002),
+        "gpt-3.5-turbo": Model("gpt-3.5-turbo", 16385, 0.001, 0.002),
+        "gpt-3.5-turbo-0613": Model("gpt-3.5-turbo-0613", 4096, 0.0015, 0.002),
+        "gpt-3.5-turbo-16k-0613": Model("gpt-3.5-turbo-16k-0613", 16385, 0.003, 0.004),
+        "gpt-3.5-turbo-0301": Model("gpt-3.5-turbo-0301", 4096, 0.0015, 0.002),
+        "text-embedding-ada-002": Model(
+            "text-embedding-ada-002", 8191, 0.0001, 0, embedding_model=True
+        ),
+    }
+)
 
 
 def model_context_size(model: str) -> Optional[int]:
     if model not in known_models:
         return None
     else:
         return known_models[model].context_size
@@ -211,28 +267,26 @@
             " with `/config maximum_context <value>`. Using a default value of"
             f" {maximum_context}.",
             style="error",
         )
         return maximum_context
 
 
-def is_context_sufficient(tokens: int) -> bool:
+def raise_if_context_exceeds_max(tokens: int):
     ctx = SESSION_CONTEXT.get()
 
     max_tokens = get_max_tokens()
     if max_tokens - tokens < ctx.config.token_buffer:
         ctx.stream.send(
             f"The context size is limited to {max_tokens} tokens and your current"
             f" request uses {tokens} tokens. Please use `/exclude` to remove"
             " some files from context or `/clear` to reset the conversation",
             style="error",
         )
-        return False
-
-    return True
+        raise ReturnToUser()
 
 
 class LlmApiHandler:
     """Used for any functions that require calling the external LLM API"""
 
     def initialize_client(self):
         ctx = SESSION_CONTEXT.get()
@@ -240,32 +294,38 @@
         if not load_dotenv(mentat_dir_path / ".env"):
             load_dotenv()
         key = os.getenv("OPENAI_API_KEY")
         base_url = os.getenv("OPENAI_API_BASE")
         azure_key = os.getenv("AZURE_OPENAI_KEY")
         azure_endpoint = os.getenv("AZURE_OPENAI_ENDPOINT")
 
-        # We don't have any use for a synchronous client, but if we ever do we can easily make it here
+        # ChromaDB requires a sync function for embeddings
         if azure_endpoint and azure_key:
-            ctx.stream.send("Using Azure OpenAI client.", color="cyan")
+            ctx.stream.send("Using Azure OpenAI client.", style="warning")
             self.async_client = AsyncAzureOpenAI(
                 api_key=azure_key,
                 api_version="2023-12-01-preview",
                 azure_endpoint=azure_endpoint,
             )
+            self.sync_client = AzureOpenAI(
+                api_key=azure_key,
+                api_version="2023-12-01-preview",
+                azure_endpoint=azure_endpoint,
+            )
         else:
             if not key:
                 if not base_url:
                     raise UserError(
                         "No OpenAI api key detected.\nEither place your key into a .env"
                         " file or export it as an environment variable."
                     )
                 # If they set the base_url but not the key, they probably don't need a key, but the client requires one
                 key = "fake_key"
             self.async_client = AsyncOpenAI(api_key=key, base_url=base_url)
+            self.sync_client = OpenAI(api_key=key, base_url=base_url)
 
         try:
             self.async_client.models.list()  # Test the key
         except AuthenticationError as e:
             raise UserError(f"API gave an Authentication Error:\n{e}")
 
     @overload
@@ -296,16 +356,15 @@
     ) -> ChatCompletion | AsyncIterator[ChatCompletionChunk]:
         session_context = SESSION_CONTEXT.get()
         config = session_context.config
         cost_tracker = session_context.cost_tracker
 
         # Confirm that model has enough tokens remaining.
         tokens = prompt_tokens(messages, model)
-        if not is_context_sufficient(tokens):
-            raise ReturnToUser()
+        raise_if_context_exceeds_max(tokens)
 
         start_time = default_timer()
         with sentry_sdk.start_span(description="LLM Call") as span:
             span.set_tag("model", model)
             # OpenAI's API is bugged; when gpt-4-vision-preview is used, including the response format
             # at all returns a 400 error. Additionally, gpt-4-vision-preview has a max response of 30 tokens by default.
             # Until this is fixed, we have to use this workaround.
@@ -352,21 +411,22 @@
             response = cost_tracker.response_logger_wrapper(
                 tokens, cast(AsyncStream[ChatCompletionChunk], response), model
             )
 
         return response
 
     @api_guard
-    async def call_embedding_api(
+    def call_embedding_api(
         self, input_texts: list[str], model: str = "text-embedding-ada-002"
-    ) -> list[list[float]]:
-        response = await self.async_client.embeddings.create(
+    ) -> Embeddings:
+        embeddings = self.sync_client.embeddings.create(
             input=input_texts, model=model
-        )
-        return [embedding.embedding for embedding in response.data]
+        ).data
+        sorted_embeddings = sorted(embeddings, key=lambda e: e.index)
+        return [result.embedding for result in sorted_embeddings]
 
     @api_guard
     async def call_whisper_api(self, audio_path: Path) -> str:
         audio_file = open(audio_path, "rb")
         transcript = await self.async_client.audio.transcriptions.create(
             model="whisper-1",
             file=audio_file,
```

### Comparing `mentat-1.0.8/mentat/logging_config.py` & `mentat-1.0.9/mentat/logging_config.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/parsers/block_parser.py` & `mentat-1.0.9/mentat/parsers/block_parser.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/parsers/change_display_helper.py` & `mentat-1.0.9/mentat/parsers/change_display_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from mentat.session_context import SESSION_CONTEXT
 from mentat.utils import get_relative_path
 
 change_delimiter = 60 * "="
 
 
-def _get_lexer(file_path: Path):
+def get_lexer(file_path: Path):
     try:
         lexer: Lexer = get_lexer_for_filename(file_path)
     except ClassNotFound:
         lexer = TextLexer()
     lexer.stripnl = False
     lexer.stripall = False
     lexer.ensurenl = False
@@ -60,15 +60,15 @@
     last_changed_line: int = attr.field(default=0)
     new_name: Path | None = attr.field(default=None)
 
     def __attrs_post_init__(self):
         ctx = SESSION_CONTEXT.get()
 
         self.line_number_buffer = get_line_number_buffer(self.file_lines)
-        self.lexer = _get_lexer(self.file_name)
+        self.lexer = get_lexer(self.file_name)
 
         if self.file_name.is_absolute():
             self.file_name = get_relative_path(self.file_name, ctx.cwd)
         if self.new_name is not None and self.new_name.is_absolute():
             self.new_name = get_relative_path(self.new_name, ctx.cwd)
 
 
@@ -187,17 +187,17 @@
         display_information.removed_block,
         display_information.line_number_buffer,
         prefix,
         color,
     )
 
 
-def highlight_text(display_information: DisplayInformation, text: str) -> str:
+def highlight_text(text: str, lexer: Lexer) -> str:
     # pygments doesn't have type hints on TerminalFormatter
-    return highlight(text, display_information.lexer, TerminalFormatter(bg="dark"))  # type: ignore
+    return highlight(text, lexer, TerminalFormatter(bg="dark"))  # type: ignore
 
 
 def get_previous_lines(
     display_information: DisplayInformation,
     num: int = 2,
 ) -> str:
     if display_information.first_changed_line < 0:
@@ -219,15 +219,15 @@
             display_information.line_number_buffer
         )
         + line
         for i, line in enumerate(lines)
     ]
 
     prev = "\n".join(numbered)
-    return highlight_text(display_information, prev)
+    return highlight_text(prev, display_information.lexer)
 
 
 def get_later_lines(
     display_information: DisplayInformation,
     num: int = 2,
 ) -> str:
     if display_information.last_changed_line < 0:
@@ -249,8 +249,8 @@
             display_information.line_number_buffer
         )
         + line
         for i, line in enumerate(lines)
     ]
 
     later = "\n".join(numbered)
-    return highlight_text(display_information, later)
+    return highlight_text(later, display_information.lexer)
```

### Comparing `mentat-1.0.8/mentat/parsers/diff_utils.py` & `mentat-1.0.9/mentat/parsers/diff_utils.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/parsers/file_edit.py` & `mentat-1.0.9/mentat/parsers/file_edit.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 async def _ask_user_change(
     text: str,
 ) -> bool:
     session_context = SESSION_CONTEXT.get()
     stream = session_context.stream
 
-    stream.send(text, color="light_blue")
+    stream.send(text, style="input")
     return await ask_yes_no(default_yes=True)
 
 
 @attr.define
 class FileEdit:
     """
     Represents that this file_path content should have specified Replacements applied to it.
@@ -149,46 +149,46 @@
 
         display_path = get_relative_path(self.file_path, session_context.cwd)
 
         if self.is_creation:
             if self.file_path.exists():
                 stream.send(
                     f"File {display_path} already exists, canceling creation.",
-                    color="light_yellow",
+                    style="warning",
                 )
                 return False
         else:
             if not self.file_path.exists():
                 stream.send(
                     f"File {display_path} does not exist, canceling all edits to file.",
-                    color="light_yellow",
+                    style="warning",
                 )
                 return False
             file_features_in_context = [
                 f for f in code_context.auto_features if f.path == self.file_path
             ] + code_context.include_files.get(self.file_path, [])
             if not all(
                 any(f.interval.contains(i) for f in file_features_in_context)
                 for r in self.replacements
                 for i in range(r.starting_line + 1, r.ending_line + 1)
             ):
                 stream.send(
                     f"File {display_path} not in context, canceling all edits to file.",
-                    color="light_yellow",
+                    style="warning",
                 )
                 return False
 
         if self.rename_file_path is not None and self.rename_file_path.exists():
             rel_rename_path = None
             if self.rename_file_path.is_relative_to(session_context.cwd):
                 rel_rename_path = self.rename_file_path.relative_to(session_context.cwd)
             stream.send(
                 f"File {display_path} being renamed to existing file"
                 f" {rel_rename_path or self.rename_file_path}, canceling rename.",
-                color="light_yellow",
+                style="warning",
             )
             self.rename_file_path = None
         return True
 
     async def filter_replacements(
         self,
     ) -> bool:
@@ -211,15 +211,15 @@
         if self.rename_file_path is not None:
             self._display_rename()
             if not await _ask_user_change("Rename this file?"):
                 self.rename_file_path = None
 
         if not self.is_creation:
             new_replacements = list[Replacement]()
-            for replacement in self.replacements:
+            for replacement in sorted(self.replacements):
                 self._display_replacement(replacement, file_lines)
                 if await _ask_user_change("Keep this change?"):
                     new_replacements.append(replacement)
             self.replacements = new_replacements
 
         return (
             self.is_creation
@@ -232,15 +232,15 @@
         session_context = SESSION_CONTEXT.get()
         stream = session_context.stream
 
         stream.send("Change overlap detected, auto-merged back to back changes:\n")
         stream.send(self.file_path)
         stream.send(change_delimiter)
         for line in first.new_lines + second.new_lines:
-            stream.send("+ " + line, color="green")
+            stream.send("+ " + line, style="success")
         stream.send(change_delimiter)
 
     def resolve_conflicts(self):
         self.replacements.sort(reverse=True)
         for index, replacement in enumerate(self.replacements):
             for other in self.replacements[index + 1 :]:
                 if (
@@ -287,15 +287,15 @@
                 raise HistoryError(
                     f"File {self.file_path} does not exist; unable to delete"
                 )
             ctx.code_file_manager.delete_file(self.file_path)
 
             self._display_creation(prefix=prefix)
             ctx.stream.send(
-                f"Creation of file {self.file_path} undone", color="light_blue"
+                f"Creation of file {self.file_path} undone", style="success"
             )
             return
 
         if self.rename_file_path is not None:
             if self.file_path.exists():
                 raise HistoryError(
                     f"File {self.file_path} already exists; unable to undo rename to"
@@ -307,15 +307,15 @@
                     f" rename from {self.file_path}"
                 )
             ctx.code_file_manager.rename_file(self.rename_file_path, self.file_path)
 
             self._display_rename(prefix=prefix)
             ctx.stream.send(
                 f"Rename of file {self.file_path} to {self.rename_file_path} undone",
-                color="light_blue",
+                style="success",
             )
 
         if self.is_deletion:
             if self.file_path.exists():
                 raise HistoryError(
                     f"File {self.file_path} already exists; unable to re-create"
                 )
@@ -326,25 +326,23 @@
                 )
             ctx.code_file_manager.create_file(
                 self.file_path, content="\n".join(self.previous_file_lines)
             )
 
             self._display_deletion(self.previous_file_lines, prefix=prefix)
             ctx.stream.send(
-                f"Deletion of file {self.file_path} undone", color="light_red"
+                f"Deletion of file {self.file_path} undone", style="success"
             )
         elif self.replacements:
             if not self.file_path.exists():
                 raise HistoryError(
                     f"File {self.file_path} does not exist; unable to undo edit"
                 )
             if not self.previous_file_lines:
                 # Should never happen
                 raise ValueError("Previous file lines not set when undoing file edit")
 
             with open(self.file_path, "w") as f:
                 f.write("\n".join(self.previous_file_lines))
 
             self._display_replacements(self.previous_file_lines, prefix=prefix)
-            ctx.stream.send(
-                f"Edits to file {self.file_path} undone", color="light_blue"
-            )
+            ctx.stream.send(f"Edits to file {self.file_path} undone", style="success")
```

### Comparing `mentat-1.0.8/mentat/parsers/json_parser.py` & `mentat-1.0.9/mentat/parsers/json_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,19 +129,19 @@
         logging.debug(message)
 
         try:
             response_json = json.loads(message)
             validate(instance=response_json, schema=output_schema)
         except JSONDecodeError:
             # Should never happen with OpenAI's response_format set to json
-            stream.send("Error processing model response: Invalid JSON", color="red")
+            stream.send("Error processing model response: Invalid JSON", style="error")
             return ParsedLLMResponse(message, "", [])
         except ValidationError:
             stream.send(
-                "Error processing model response: Invalid format given", color="red"
+                "Error processing model response: Invalid format given", style="error"
             )
             return ParsedLLMResponse(message, "", [])
 
         file_edits: Dict[Path, FileEdit] = {}
         for obj in response_json["content"]:
             filename = (session_context.cwd / obj.get("filename", "")).resolve()
             if filename in rename_map:
```

### Comparing `mentat-1.0.8/mentat/parsers/parser.py` & `mentat-1.0.9/mentat/parsers/parser.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/parsers/parser_map.py` & `mentat-1.0.9/mentat/parsers/parser_map.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/parsers/replacement_parser.py` & `mentat-1.0.9/mentat/parsers/replacement_parser.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/parsers/unified_diff_parser.py` & `mentat-1.0.9/mentat/parsers/unified_diff_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         if cur_line == UnifiedDiffDelimiter.MidChange.value:
             return change_delimiter + "\n"
         elif cur_line.startswith("+"):
             return colored(content, "green")
         elif cur_line.startswith("-"):
             return colored(content, "red")
         else:
-            return highlight_text(display_information, content)
+            return highlight_text(content, display_information.lexer)
 
     @override
     def _could_be_special(self, cur_line: str) -> bool:
         return (
             # Since the model is printing the context lines, we can only
             # highlight them once we get a full line, so we choose to
             # add the lines to the printer all at once.
```

### Comparing `mentat-1.0.8/mentat/python_client/client.py` & `mentat-1.0.9/mentat/python_client/client.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/resources/prompts/agent_command_selection_prompt.txt` & `mentat-1.0.9/mentat/resources/prompts/agent_command_selection_prompt.txt`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/resources/prompts/agent_file_selection_prompt.txt` & `mentat-1.0.9/mentat/resources/prompts/agent_file_selection_prompt.txt`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/resources/prompts/block_parser_prompt.txt` & `mentat-1.0.9/mentat/resources/prompts/block_parser_prompt.txt`

 * *Files 14% similar despite different names*

```diff
@@ -123,54 +123,7 @@
 @@end
 @@start
 {
     "file": "core/goodbye_world.py",
     "action": "delete-file"
 }
 @@end
-
-
-Example 2:
-
-Here's an example response to a user request where the user is requesting changes to
-a function that is in "Code Files", but they want to use a function that needs to be 
-imported from a file in "Code Map":
-
-Code Files:
-
-core/hello_world.py
-1:
-2:def hello_world():
-3:    print("Hello, World!")
-4:
-
-User Request:
-Call say_goodbye after printing hello world
-
-Example Response:
-
-I will make the modifications to hello_world.py
-
-Steps:
-1. Import the say_goodbye function in hello_world.py
-2. Modify hello_world.py, adding a function call for say_goodbye
-
-@@start
-{
-    "file": "core/hello_world.py",
-    "action": "insert",
-    "insert-after-line": 0,
-    "insert-before-line": 1
-}
-@@code
-from core.script import say_goodbye
-@@end
-@@start
-{
-    "file": "core/hello_world.py",
-    "action": "insert",
-    "insert-after-line": 4,
-    "insert-before-line": 5
-}
-@@code
-    say_goodbye()
-@@end
```

### Comparing `mentat-1.0.8/mentat/resources/prompts/feature_selection_prompt.txt` & `mentat-1.0.9/mentat/resources/prompts/feature_selection_prompt.txt`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/resources/prompts/json_parser_prompt.txt` & `mentat-1.0.9/mentat/resources/prompts/json_parser_prompt.txt`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/resources/prompts/replacement_parser_prompt.txt` & `mentat-1.0.9/mentat/resources/prompts/replacement_parser_prompt.txt`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/resources/prompts/unified_diff_parser_prompt.txt` & `mentat-1.0.9/mentat/resources/prompts/unified_diff_parser_prompt.txt`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/resources/templates/benchmark.jinja` & `mentat-1.0.9/mentat/resources/templates/benchmark.jinja`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/resources/templates/conversation_viewer.jinja` & `mentat-1.0.9/mentat/resources/templates/conversation_viewer.jinja`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/resources/templates/css/benchmark.css` & `mentat-1.0.9/mentat/resources/templates/css/benchmark.css`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/resources/templates/css/transcript.css` & `mentat-1.0.9/mentat/resources/templates/css/transcript.css`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,18 @@
     background-color: rgb(255, 255, 255);
 }
 
 .agent {
     background-color: rgb(255, 197, 197);
 }
 
+.revisor {
+    background-color: rgb(243, 246, 196);
+}
+
 .button-group {
     position: absolute;
     top: 20px;
     right: 20px;
 }
 .modal {
     display: none;
```

### Comparing `mentat-1.0.8/mentat/resources/templates/js/conversation_viewer.js` & `mentat-1.0.9/mentat/resources/templates/js/conversation_viewer.js`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/resources/templates/js/transcript.js` & `mentat-1.0.9/mentat/resources/templates/js/transcript.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -26,15 +26,15 @@
         method: "POST",
         mode: "no-cors",
         headers: {
             'Content-Type': 'application/json'
         },
         body: JSON.stringify(data)
     }).then(response => {
-        return `https://abante-shared-usage-examples.s3.us-east-2.amazonaws.com/${key}`;
+        return `http://transcripts.mentat.ai/${key}`;
     })
 }
 
 function makeToast(message) {
     const toast = document.createElement("div");
     toast.classList.add("toast");
     toast.textContent = message;
```

### Comparing `mentat-1.0.8/mentat/resources/templates/transcript.jinja` & `mentat-1.0.9/mentat/resources/templates/transcript.jinja`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/sampler/sample.py` & `mentat-1.0.9/mentat/sampler/sample.py`

 * *Files 20% similar despite different names*

```diff
@@ -33,13 +33,17 @@
             json.dump(attr.asdict(self), f, indent=4)
 
     @classmethod
     def load(cls, fname: str | Path) -> Sample:
         with open(fname, "r") as f:
             kwargs = json.load(f)
             _version = kwargs.get("version")
+            if _version and _version < "0.2.0":
+                kwargs["message_history"] = kwargs.get("message_history", [])[::-1]
+                kwargs["version"] = "0.2.0"
+                _version = kwargs["version"]
             if _version != __version__:
                 raise SampleError(
                     f"Warning: sample version ({_version}) does not match current"
                     f" version ({__version__})."
                 )
             return cls(**kwargs)
```

### Comparing `mentat-1.0.8/mentat/sampler/sampler.py` & `mentat-1.0.9/mentat/sampler/sampler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,74 +1,52 @@
 import subprocess
 from pathlib import Path
 from uuid import uuid4
 
 from git import GitCommandError, Repo  # type: ignore
-from openai.types.chat import ChatCompletionMessageParam
 
 from mentat.code_feature import get_consolidated_feature_refs
 from mentat.errors import SampleError
 from mentat.git_handler import get_git_diff, get_git_root_for_path, get_hexsha_active
 from mentat.parsers.git_parser import GitParser
+from mentat.parsers.parser import ParsedLLMResponse
 from mentat.sampler.sample import Sample
 from mentat.sampler.utils import get_active_snapshot_commit
 from mentat.session_context import SESSION_CONTEXT
 from mentat.session_input import collect_user_input
 from mentat.utils import get_relative_path
 
 
-def parse_message(message: ChatCompletionMessageParam) -> dict[str, str]:
-    ctx = SESSION_CONTEXT.get()
-    content = message.get("content")
-    text, code = "", ""
-    if isinstance(content, str):
-        if message.get("role") != "assistant":
-            text = content
-        output = list[str]()
-        in_special = False
-        for line in content.splitlines():
-            if ctx.config.parser._starts_special(line):  # type: ignore
-                in_special = True
-            if not in_special:
-                output.append(line)
-            else:
-                pass  # TODO: Convert to git diff format, replace 'code' above
-            if ctx.config.parser._ends_code(line):  # type: ignore
-                in_special = False
-        while output[-1] == "":
-            output.pop()
-        text = "\n".join(output)
-    elif isinstance(content, list) and len(content) > 0:
-        content = content[0]
-        if "text" in content and isinstance(content.get("text"), str):  # type: ignore
-            text = content.get("text")  # type: ignore
-    return {"text": text, "code": code}
-
-
 class Sampler:
-    active: bool = True
     diff_active: str | None = None
     commit_active: str | None = None
     last_sample_id: str | None = None
     last_sample_hexsha: str | None = None
 
     def set_active_diff(self):
         # Create a temporary commit with the active changes
         ctx = SESSION_CONTEXT.get()
         git_root = get_git_root_for_path(ctx.cwd, raise_error=False)
         if not git_root:
             return
         repo = Repo(git_root)
-        self.commit_active = get_active_snapshot_commit(repo)
-        # If changes were made since the last sample, don't list it as parent.
-        if not self.last_sample_hexsha:
-            return
-        if self.last_sample_hexsha != get_hexsha_active():
-            self.last_sample_id = None
-            self.last_sample_hexsha = None
+        try:
+            self.commit_active = get_active_snapshot_commit(repo)
+            # If changes were made since the last sample, don't list it as parent.
+            if not self.last_sample_hexsha:
+                return
+            if self.last_sample_hexsha != get_hexsha_active():
+                self.last_sample_id = None
+                self.last_sample_hexsha = None
+        except SampleError as e:
+            ctx.stream.send(
+                f"Sampler error setting active diff: {e}. Disabling sampler.",
+                style="error",
+            )
+            ctx.config.sampler = False
 
     async def create_sample(self) -> Sample:
         # Check for repo and merge_base in config
         session_context = SESSION_CONTEXT.get()
         stream = session_context.stream
         code_context = session_context.code_context
         config = session_context.config
@@ -96,15 +74,15 @@
                     )
         if not merge_base:
             merge_base = git_repo.head.commit.hexsha
             stream.send(
                 f"Use latest commit ({merge_base[:10]} as merge base? Press 'ENTER' to"
                 " accept, or enter a new merge base commit."
             )
-            response = (await collect_user_input()).data.strip()
+            response = str((await collect_user_input()).data).strip()
             if response:
                 merge_base = response
         try:
             assert merge_base is not None, "No merge base found"
             diff_merge_base = get_git_diff(merge_base, "HEAD")
         except (AssertionError, GitCommandError) as e:
             raise SampleError(f"Error getting diff for merge base: {e}")
@@ -123,59 +101,92 @@
                 f"Found repo URL: {remote_url}. Press 'ENTER' to accept, or enter a new"
                 " URL."
             )
             response = (await collect_user_input()).data.strip()
             if response == "y":
                 repo = remote_url
             else:
-                repo = response
+                repo = str(response)
             config.sample_repo = repo
 
         stream.send("Sample Title:")
         title = (await collect_user_input()).data.strip() or ""
         stream.send("Description: (optional)")
         description = (await collect_user_input()).data.strip() or ""
         stream.send("Test Command: (optional, e.g. 'pytest -k foo')")
         test_command = (await collect_user_input()).data.strip() or ""
 
-        message_history, message_prompt, message_edit = list[dict[str, str]](), "", ""
-        for m in conversation.get_messages()[::-1]:
-            if m["role"] not in {"user", "assistant"}:
-                continue
-            parsed = parse_message(m)
-            text = parsed["text"]
-            code = parsed["code"]
-            if not message_prompt:
-                if m["role"] == "user":
+        message_history: list[dict[str, str]] = []
+        message_prompt = ""
+        response_edit: None | ParsedLLMResponse = None
+        for m in conversation.get_messages(include_parsed_llm_responses=True)[::-1]:
+            response: str | ParsedLLMResponse | None = None
+            role, content = m["role"], m.get("content")
+            if role == "user":
+                if isinstance(content, str):
+                    text = content
+                elif isinstance(content, list) and len(content) > 0:
+                    text = content[0].get("text", "")
+                else:
+                    continue
+
+                if not message_prompt:
                     message_prompt = text
-                elif m["role"] == "assistant":
-                    message_edit += text
-            else:
-                message_history.append({"role": m["role"], "content": text + code})
+                else:
+                    message_history.insert(0, {"role": role, "content": text})
+
+            elif role == "assistant":
+                parsed_llm_response = m.get("parsed_llm_response")
+                if parsed_llm_response is None:
+                    raise SampleError(
+                        "Assistant messages must include a the parsed_llm_response."
+                        " Hint: Use"
+                        " mentat.conversation.MentatAssistantMessageParam"
+                        " instead  of"
+                        " openai.types.chat.ChatCompletionAssistantMessageParam."
+                    )
+
+                if not message_prompt:
+                    response_edit = parsed_llm_response
+                else:
+                    message_history.append(
+                        {
+                            "role": role,
+                            "content": GitParser().file_edits_to_llm_message(
+                                parsed_llm_response
+                            ),
+                        }
+                    )
 
-        diff_active = ""
-        diff_edit = get_git_diff("HEAD")
+        if not response_edit:
+            raise SampleError("No LLM response found.")
+        message_edit = response_edit.conversation.strip()
         if self.commit_active:
             diff_active = get_git_diff("HEAD", self.commit_active)
-            diff_edit = get_git_diff(self.commit_active)
+        else:
+            diff_active = ""
+        if response_edit.file_edits:
+            diff_edit = get_git_diff(self.commit_active or "HEAD")
+        else:
+            diff_edit = ""
 
         context = set[str]()
 
         def _rp(f: str | Path) -> str:
             return get_relative_path(Path(f), git_root).as_posix()
 
         # Add include_files from context
         if code_context.include_files:
             feature_refs = get_consolidated_feature_refs(
                 [f for fs in code_context.include_files.values() for f in fs]
             )
             context.update(_rp(f) for f in feature_refs)
         # Undo adds/removes/renames to match pre-diff_edit state
         if diff_edit:
-            file_edits = GitParser().parse_string(diff_edit).file_edits
+            file_edits = GitParser().parse_llm_response(diff_edit).file_edits
             for file_edit in file_edits:
                 file_path = _rp(file_edit.file_path)
                 rename_path = (
                     ""
                     if not file_edit.rename_file_path
                     else _rp(file_edit.rename_file_path)
                 )
```

### Comparing `mentat-1.0.8/mentat/sampler/utils.py` & `mentat-1.0.9/mentat/sampler/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from git import GitCommandError, Repo  # type: ignore
 
 from mentat.errors import SampleError
 from mentat.git_handler import get_non_gitignored_files
 from mentat.utils import is_file_text_encoded
 
-CLONE_TO_DIR = Path(__file__).parent.parent.parent / "benchmark_repos"
+CLONE_TO_DIR = Path("benchmarks/benchmark_repos")
 
 
 def clone_repo(
     url: str, local_dir_name: str, refresh: bool = False, depth: int = 0
 ) -> Path | None:
     local_dir = CLONE_TO_DIR / local_dir_name
     if os.path.exists(local_dir):
@@ -92,15 +92,15 @@
             raise SampleError(f"Error applying diff_active: {errors}")
 
     return repo
 
 
 def get_active_snapshot_commit(repo: Repo) -> str | None:
     """Returns the commit hash of the current active snapshot, or None if there are no active changes."""
-    if not repo.is_dirty():
+    if not repo.is_dirty() and not repo.untracked_files:
         return None
     if not repo.config_reader().has_option("user", "name"):
         raise SampleError(
             "ERROR: Git user.name not set. Please run 'git config --global user.name"
             ' "Your Name"\'.'
         )
     try:
```

### Comparing `mentat-1.0.8/mentat/sentry.py` & `mentat-1.0.9/mentat/sentry.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/session.py` & `mentat-1.0.9/mentat/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,19 @@
 from mentat.code_context import CodeContext
 from mentat.code_edit_feedback import get_user_feedback_on_edits
 from mentat.code_file_manager import CodeFileManager
 from mentat.config import Config
 from mentat.conversation import Conversation
 from mentat.cost_tracker import CostTracker
 from mentat.ctags import ensure_ctags_installed
-from mentat.errors import MentatError, ReturnToUser, SampleError, SessionExit, UserError
+from mentat.errors import MentatError, ReturnToUser, SessionExit, UserError
 from mentat.git_handler import get_git_root_for_path
 from mentat.llm_api_handler import LlmApiHandler, is_test_environment
 from mentat.logging_config import setup_logging
+from mentat.revisor.revisor import revise_edits
 from mentat.sampler.sampler import Sampler
 from mentat.sentry import sentry_init
 from mentat.session_context import SESSION_CONTEXT, SessionContext
 from mentat.session_input import collect_input_with_commands
 from mentat.session_stream import SessionStream
 from mentat.utils import check_version, mentat_dir_path
 from mentat.vision.vision_manager import VisionManager
@@ -112,14 +113,16 @@
         if (
             code_context.diff_context is not None
             and len(code_context.include_files) == 0
             and (diff or pr_diff)
         ):
             for file in code_context.diff_context.diff_files():
                 code_context.include(file)
+        if config.sampler:
+            sampler.set_active_diff()
 
     def _create_task(self, coro: Coroutine[None, None, Any]):
         """Utility method for running a Task in the background"""
 
         def task_cleanup(task: asyncio.Task[None]):
             self._tasks.remove(task)
 
@@ -167,32 +170,27 @@
 
                 parsed_llm_response = await conversation.get_model_response()
                 file_edits = [
                     file_edit
                     for file_edit in parsed_llm_response.file_edits
                     if file_edit.is_valid()
                 ]
+                for file_edit in file_edits:
+                    file_edit.resolve_conflicts()
                 if file_edits:
+                    if session_context.config.revisor:
+                        await revise_edits(file_edits)
+
                     if not agent_handler.agent_enabled:
                         file_edits, need_user_request = (
                             await get_user_feedback_on_edits(file_edits)
                         )
-                    for file_edit in file_edits:
-                        file_edit.resolve_conflicts()
 
-                    if session_context.sampler and session_context.sampler.active:
-                        try:
-                            session_context.sampler.set_active_diff()
-                        except SampleError as e:
-                            stream.send(
-                                f"Sampler error setting active diff: {e}. Disabling"
-                                " sampler.",
-                                style="error",
-                            )
-                            session_context.sampler.active = False
+                    if session_context.config.sampler:
+                        session_context.sampler.set_active_diff()
 
                     applied_edits = await code_file_manager.write_changes_to_files(
                         file_edits
                     )
                     stream.send(
                         "Changes applied." if applied_edits else "No changes applied.",
                         style="input",
@@ -219,15 +217,18 @@
         await self.stream.recv(channel="session_exit")
         self._main_task.cancel()
 
     async def listen_for_completion_requests(self):
         ctx = SESSION_CONTEXT.get()
 
         async for message in self.stream.listen(channel="completion_request"):
-            completions = ctx.auto_completer.get_completions(message.data)
+            completions = ctx.auto_completer.get_completions(
+                message.data,
+                command_autocomplete=message.extra.get("command_autocomplete", False),
+            )
             # Will intermediary client for vscode serialize/deserialize all messages automatically?
             self.stream.send(completions, channel=f"completion_request:{message.id}")
 
     ### lifecycle
 
     def start(self):
         """Asynchronously start the Session.
```

### Comparing `mentat-1.0.8/mentat/session_context.py` & `mentat-1.0.9/mentat/session_context.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/session_input.py` & `mentat-1.0.9/mentat/session_input.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,24 +15,28 @@
 
     message = stream.send("", channel="input_request", **kwargs)
     response = await stream.recv(f"input_request:{message.id}")
     logging.debug(f"User Input: {response.data}")
     return response
 
 
-async def collect_user_input(plain: bool = False) -> StreamMessage:
+async def collect_user_input(
+    plain: bool = False, command_autocomplete: bool = False
+) -> StreamMessage:
     """
     Listens for user input on a new channel
 
     send a message requesting user to send a response
     create a new broadcast channel that listens for the input
     close the channel after receiving the input
     """
 
-    response = await _get_input_request(plain=plain)
+    response = await _get_input_request(
+        plain=plain, command_autocomplete=command_autocomplete
+    )
     # Quit on q
     if isinstance(response.data, str) and response.data.strip() == "q":
         raise SessionExit
 
     return response
 
 
@@ -50,24 +54,24 @@
     return content == "y" or (content != "n" and default_yes)
 
 
 async def collect_input_with_commands() -> StreamMessage:
     session_context = SESSION_CONTEXT.get()
     stream = session_context.stream
 
-    response = await collect_user_input()
+    response = await collect_user_input(command_autocomplete=True)
     while isinstance(response.data, str) and response.data.startswith("/"):
         try:
             # We only use shlex to split the arguments, not the command itself
             arguments = shlex.split(" ".join(response.data.split(" ")[1:]))
             command = Command.create_command(response.data[1:].split(" ")[0])
             await command.apply(*arguments)
         except ValueError as e:
             stream.send(f"Error processing command arguments: {e}", style="error")
-        response = await collect_user_input()
+        response = await collect_user_input(command_autocomplete=True)
     return response
 
 
 async def listen_for_interrupt(
     coro: Coroutine[None, None, Any], raise_exception_on_interrupt: bool = True
 ):
     """Listens for an 'interrupt' message from a client
```

### Comparing `mentat-1.0.8/mentat/streaming_printer.py` & `mentat-1.0.9/mentat/streaming_printer.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/terminal/client.py` & `mentat-1.0.9/mentat/terminal/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,17 @@
         while True:
             input_request_message = await self.session.stream.recv("input_request")
             # TODO: Make extra kwargs like plain constants
             if input_request_message.extra.get("plain"):
                 prompt_session = self._plain_session
             else:
                 prompt_session = self._prompt_session
+            self.mentat_completer.command_autocomplete = (
+                input_request_message.extra.get("command_autocomplete", False)
+            )
 
             default_prompt = self._default_prompt.strip()
             self._default_prompt = ""
 
             user_input = await prompt_session.prompt_async(
                 handle_sigint=False, default=default_prompt
             )
@@ -144,17 +147,17 @@
             self.ignore_paths,
             self.diff,
             self.pr_diff,
             self.config,
         )
         self.session.start()
 
-        mentat_completer = MentatCompleter(self.session.stream)
+        self.mentat_completer = MentatCompleter(self.session.stream)
         self._prompt_session = MentatPromptSession(
-            completer=mentat_completer,
+            completer=self.mentat_completer,
             style=Style(self.config.input_style),
             enable_suspend=True,
         )
 
         plain_bindings = KeyBindings()
 
         @plain_bindings.add("c-c")
```

### Comparing `mentat-1.0.8/mentat/terminal/loading.py` & `mentat-1.0.9/mentat/terminal/loading.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/terminal/output.py` & `mentat-1.0.9/mentat/terminal/output.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/terminal/prompt_completer.py` & `mentat-1.0.9/mentat/terminal/prompt_completer.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,26 +7,30 @@
 from mentat.auto_completer import Completion
 from mentat.session_stream import SessionStream, StreamMessageSource
 
 
 class MentatCompleter(Completer):
     def __init__(self, stream: SessionStream):
         self.stream = stream
+        self.command_autocomplete = False
 
     def get_completions(
         self, document: Document, complete_event: CompleteEvent
     ) -> Iterable[PromptToolkitCompletion]:
         raise NotImplementedError
 
     async def get_completions_async(
         self, document: Document, complete_event: CompleteEvent
     ):
         text = document.text_before_cursor
         message = self.stream.send(
-            text, source=StreamMessageSource.CLIENT, channel="completion_request"
+            text,
+            source=StreamMessageSource.CLIENT,
+            channel="completion_request",
+            command_autocomplete=self.command_autocomplete,
         )
 
         response = await self.stream.recv(channel=f"completion_request:{message.id}")
         completions: List[Completion] = response.data
         for completion in completions:
             yield PromptToolkitCompletion(
                 text=completion["content"],
```

### Comparing `mentat-1.0.8/mentat/terminal/prompt_session.py` & `mentat-1.0.9/mentat/terminal/prompt_session.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/transcripts.py` & `mentat-1.0.9/mentat/transcripts.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/utils.py` & `mentat-1.0.9/mentat/utils.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat/vision/vision_manager.py` & `mentat-1.0.9/mentat/vision/vision_manager.py`

 * *Files identical despite different names*

### Comparing `mentat-1.0.8/mentat.egg-info/requires.txt` & `mentat-1.0.9/mentat.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 attrs==23.1.0
 backoff==2.2.1
+chromadb==0.4.22
 fire==0.5.0
-gitpython==3.1.37
+gitpython==3.1.41
 jinja2==3.1.2
 jsonschema>=4.17.0
 numpy==1.26.0
 openai==1.3.0
 pillow==10.1.0
 prompt-toolkit==3.0.39
 Pygments==2.15.1
@@ -23,13 +24,13 @@
 typing_extensions==4.8.0
 tqdm==4.66.1
 webdriver_manager==4.0.1
 
 [dev]
 aiomultiprocess==0.9.0
 black==23.9.1
-gitpython==3.1.37
+gitpython==3.1.41
 isort==5.12.0
 pip-licenses==4.3.3
 pyright==1.1.339
 pytest-xdist==3.3.1
 ruff==0.0.292
```

### Comparing `mentat-1.0.8/setup.py` & `mentat-1.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,17 @@
     long_description = f.read()
 
 
 setup(
     name="mentat",
     version=__version__,
     python_requires=">=3.10",
-    packages=find_packages(include=["mentat", "mentat.*", "tests"]),
+    packages=find_packages(
+        include=["mentat", "mentat.*", "benchmarks", "benchmarks.*"]
+    ),
     install_requires=[
         str(r)
         for r in pkg_resources.parse_requirements(
             open(os.path.join(os.path.dirname(__file__), "requirements.txt"))
         )
     ],
     entry_points={
```

