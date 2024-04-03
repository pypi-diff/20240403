# Comparing `tmp/sweepai-2.0.0.dev0.tar.gz` & `tmp/sweepai-2.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweepai-2.0.0.dev0.tar", last modified: Tue Apr  2 23:56:11 2024, max compression
+gzip compressed data, was "sweepai-2.0.0.dev1.tar", last modified: Wed Apr  3 16:53:31 2024, max compression
```

## Comparing `sweepai-2.0.0.dev0.tar` & `sweepai-2.0.0.dev1.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 23:56:11.733292 sweepai-2.0.0.dev0/
--rw-r--r--   0 root         (0) root         (0)    34523 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    48104 2024-04-02 23:56:11.733292 sweepai-2.0.0.dev0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6420 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 23:56:11.713292 sweepai-2.0.0.dev0/eval/
--rw-r--r--   0 root         (0) root         (0)    10167 2024-04-02 00:22:38.000000 sweepai-2.0.0.dev0/eval/swe_bench.py
--rw-r--r--   0 root         (0) root         (0)    10513 2024-04-02 00:22:38.000000 sweepai-2.0.0.dev0/eval/swe_bench_utils.py
--rw-r--r--   0 root         (0) root         (0)     1991 2024-04-02 23:53:26.000000 sweepai-2.0.0.dev0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-02 23:56:11.733292 sweepai-2.0.0.dev0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 23:56:11.713292 sweepai-2.0.0.dev0/sweepai/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 23:56:11.717292 sweepai-2.0.0.dev0/sweepai/agents/
--rw-r--r--   0 root         (0) root         (0)     1185 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/agents/agent_utils.py
--rw-r--r--   0 root         (0) root         (0)    52485 2024-04-02 01:55:11.000000 sweepai-2.0.0.dev0/sweepai/agents/assistant_function_modify.py
--rw-r--r--   0 root         (0) root         (0)     4691 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/agents/assistant_functions.py
--rw-r--r--   0 root         (0) root         (0)    12576 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/agents/assistant_planning.py
--rw-r--r--   0 root         (0) root         (0)    18975 2024-04-01 21:54:50.000000 sweepai-2.0.0.dev0/sweepai/agents/assistant_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     4052 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/agents/assistant_wrapper_test.py
--rw-r--r--   0 root         (0) root         (0)     2958 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/agents/complete_code.py
--rw-r--r--   0 root         (0) root         (0)     1772 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/agents/complete_code_test.py
--rw-r--r--   0 root         (0) root         (0)     2448 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/agents/distill_issue.py
--rw-r--r--   0 root         (0) root         (0)    27333 2024-03-28 21:42:33.000000 sweepai-2.0.0.dev0/sweepai/agents/modify_bot.py
--rw-r--r--   0 root         (0) root         (0)     5367 2024-03-28 21:42:33.000000 sweepai-2.0.0.dev0/sweepai/agents/modify_file.py
--rw-r--r--   0 root         (0) root         (0)     1357 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/agents/pr_description_bot.py
--rw-r--r--   0 root         (0) root         (0)     3814 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/agents/prune_modify_snippets.py
--rw-r--r--   0 root         (0) root         (0)    52353 2024-04-01 21:54:50.000000 sweepai-2.0.0.dev0/sweepai/api.py
--rw-r--r--   0 root         (0) root         (0)      753 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/api_test.py
--rw-r--r--   0 root         (0) root         (0)    13534 2024-04-02 23:14:46.000000 sweepai-2.0.0.dev0/sweepai/cli.py
--rw-r--r--   0 root         (0) root         (0)     1143 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/cli_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 23:56:11.717292 sweepai-2.0.0.dev0/sweepai/config/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12383 2024-03-28 21:42:33.000000 sweepai-2.0.0.dev0/sweepai/config/client.py
--rw-r--r--   0 root         (0) root         (0)     9564 2024-04-02 22:54:02.000000 sweepai-2.0.0.dev0/sweepai/config/server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 23:56:11.721292 sweepai-2.0.0.dev0/sweepai/core/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15920 2024-04-02 23:51:20.000000 sweepai-2.0.0.dev0/sweepai/core/chat.py
--rw-r--r--   0 root         (0) root         (0)    42200 2024-04-01 23:04:40.000000 sweepai-2.0.0.dev0/sweepai/core/context_pruning.py
--rw-r--r--   0 root         (0) root         (0)    17833 2024-03-26 17:32:09.000000 sweepai-2.0.0.dev0/sweepai/core/entities.py
--rw-r--r--   0 root         (0) root         (0)     1658 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/core/external_searcher.py
--rw-r--r--   0 root         (0) root         (0)    10630 2024-04-02 18:54:07.000000 sweepai-2.0.0.dev0/sweepai/core/lexical_search.py
--rw-r--r--   0 root         (0) root         (0)     5826 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/core/post_merge.py
--rw-r--r--   0 root         (0) root         (0)     2624 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/core/pr_reader.py
--rw-r--r--   0 root         (0) root         (0)    36545 2024-03-29 19:15:49.000000 sweepai-2.0.0.dev0/sweepai/core/prompts.py
--rw-r--r--   0 root         (0) root         (0)    13688 2024-03-31 22:18:38.000000 sweepai-2.0.0.dev0/sweepai/core/reflection_utils.py
--rw-r--r--   0 root         (0) root         (0)     5377 2024-04-02 00:22:38.000000 sweepai-2.0.0.dev0/sweepai/core/repo_parsing_utils.py
--rw-r--r--   0 root         (0) root         (0)    52470 2024-04-02 18:54:07.000000 sweepai-2.0.0.dev0/sweepai/core/sweep_bot.py
--rw-r--r--   0 root         (0) root         (0)     5758 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/core/update_prompts.py
--rw-r--r--   0 root         (0) root         (0)     9561 2024-04-02 23:24:36.000000 sweepai-2.0.0.dev0/sweepai/core/vector_db.py
--rw-r--r--   0 root         (0) root         (0)       19 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/global_threads.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 23:56:11.721292 sweepai-2.0.0.dev0/sweepai/handlers/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/handlers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15582 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/handlers/create_pr.py
--rw-r--r--   0 root         (0) root         (0)     5670 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/handlers/on_button_click.py
--rw-r--r--   0 root         (0) root         (0)     1569 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/handlers/on_button_click_test.py
--rw-r--r--   0 root         (0) root         (0)     5247 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/handlers/on_check_suite.py
--rw-r--r--   0 root         (0) root         (0)    18961 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/handlers/on_comment.py
--rw-r--r--   0 root         (0) root         (0)     4123 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/handlers/on_merge.py
--rw-r--r--   0 root         (0) root         (0)    13160 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/handlers/on_merge_conflict.py
--rw-r--r--   0 root         (0) root         (0)      722 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/handlers/on_review.py
--rw-r--r--   0 root         (0) root         (0)    86721 2024-03-28 21:42:33.000000 sweepai-2.0.0.dev0/sweepai/handlers/on_ticket.py
--rw-r--r--   0 root         (0) root         (0)     5262 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/handlers/pr_utils.py
--rw-r--r--   0 root         (0) root         (0)    10042 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/handlers/stack_pr.py
--rw-r--r--   0 root         (0) root         (0)     1143 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/handlers/stack_pr_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 23:56:11.721292 sweepai-2.0.0.dev0/sweepai/logn/
--rw-r--r--   0 root         (0) root         (0)       44 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/logn/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5942 2024-03-26 17:31:09.000000 sweepai-2.0.0.dev0/sweepai/logn/cache.py
--rw-r--r--   0 root         (0) root         (0)    11758 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/logn/logn.py
--rw-r--r--   0 root         (0) root         (0)      376 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/logn/trace_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 23:56:11.729292 sweepai-2.0.0.dev0/sweepai/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3152 2024-04-02 23:52:56.000000 sweepai-2.0.0.dev0/sweepai/utils/anthropic_client.py
--rw-r--r--   0 root         (0) root         (0)     1980 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/utils/autoimport.py
--rw-r--r--   0 root         (0) root         (0)     3047 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/utils/buttons.py
--rw-r--r--   0 root         (0) root         (0)     1830 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/utils/buttons_test.py
--rw-r--r--   0 root         (0) root         (0)     7850 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/utils/chat_logger.py
--rw-r--r--   0 root         (0) root         (0)     7882 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/utils/code_tree.py
--rw-r--r--   0 root         (0) root         (0)      716 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/utils/code_tree_test.py
--rw-r--r--   0 root         (0) root         (0)      616 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/utils/comment_utils.py
--rw-r--r--   0 root         (0) root         (0)     1177 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/utils/comment_utils_test.py
--rw-r--r--   0 root         (0) root         (0)     5817 2024-03-30 01:11:28.000000 sweepai-2.0.0.dev0/sweepai/utils/convert_openai_anthropic.py
--rw-r--r--   0 root         (0) root         (0)    12918 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/utils/diff.py
--rw-r--r--   0 root         (0) root         (0)     2902 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/utils/diff_test.py
--rw-r--r--   0 root         (0) root         (0)     1674 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/utils/docker_utils.py
--rw-r--r--   0 root         (0) root         (0)      392 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/utils/docker_utils_test.py
--rw-r--r--   0 root         (0) root         (0)     2637 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/utils/event_logger.py
--rw-r--r--   0 root         (0) root         (0)      432 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/utils/file_utils.py
--rw-r--r--   0 root         (0) root         (0)     6767 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/utils/fuzzy_diff.py
--rw-r--r--   0 root         (0) root         (0)     2709 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/utils/fuzzy_diff_test.py
--rw-r--r--   0 root         (0) root         (0)    24380 2024-04-01 22:09:48.000000 sweepai-2.0.0.dev0/sweepai/utils/github_utils.py
--rw-r--r--   0 root         (0) root         (0)     2291 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/utils/github_utils_test.py
--rw-r--r--   0 root         (0) root         (0)      100 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/utils/hash.py
--rw-r--r--   0 root         (0) root         (0)     1616 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/utils/html_extractor.py
--rw-r--r--   0 root         (0) root         (0)     3008 2024-03-28 21:42:33.000000 sweepai-2.0.0.dev0/sweepai/utils/modify_utils.py
--rw-r--r--   0 root         (0) root         (0)     5697 2024-04-02 18:54:07.000000 sweepai-2.0.0.dev0/sweepai/utils/multi_query.py
--rw-r--r--   0 root         (0) root         (0)    21464 2024-03-31 22:18:38.000000 sweepai-2.0.0.dev0/sweepai/utils/openai_listwise_reranker.py
--rw-r--r--   0 root         (0) root         (0)    11068 2024-03-26 22:42:55.000000 sweepai-2.0.0.dev0/sweepai/utils/openai_proxy.py
--rw-r--r--   0 root         (0) root         (0)     4220 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/utils/openai_proxy_test.py
--rw-r--r--   0 root         (0) root         (0)     1422 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/utils/patch_utils.py
--rw-r--r--   0 root         (0) root         (0)     9641 2024-03-28 21:42:33.000000 sweepai-2.0.0.dev0/sweepai/utils/progress.py
--rw-r--r--   0 root         (0) root         (0)      384 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/utils/progress_test.py
--rw-r--r--   0 root         (0) root         (0)     8711 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/utils/prompt_constructor.py
--rw-r--r--   0 root         (0) root         (0)      924 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/utils/regex_utils.py
--rw-r--r--   0 root         (0) root         (0)      841 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/utils/safe_pqueue.py
--rw-r--r--   0 root         (0) root         (0)     2022 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/utils/scorer.py
--rw-r--r--   0 root         (0) root         (0)      791 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/utils/scorer_test.py
--rw-r--r--   0 root         (0) root         (0)    13788 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/utils/search_and_replace.py
--rw-r--r--   0 root         (0) root         (0)     2101 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/utils/search_and_replace_test.py
--rw-r--r--   0 root         (0) root         (0)     4596 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/utils/str_utils.py
--rw-r--r--   0 root         (0) root         (0)    11345 2024-04-02 18:54:07.000000 sweepai-2.0.0.dev0/sweepai/utils/ticket_utils.py
--rw-r--r--   0 root         (0) root         (0)      606 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/utils/timer.py
--rw-r--r--   0 root         (0) root         (0)     7346 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/utils/tree_utils.py
--rw-r--r--   0 root         (0) root         (0)     2963 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/utils/user_settings.py
--rw-r--r--   0 root         (0) root         (0)    21346 2024-04-02 01:55:11.000000 sweepai-2.0.0.dev0/sweepai/utils/utils.py
--rw-r--r--   0 root         (0) root         (0)      586 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/utils/utils_test.py
--rw-r--r--   0 root         (0) root         (0)     3989 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/watch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 23:56:11.729292 sweepai-2.0.0.dev0/sweepai/web/
--rw-r--r--   0 root         (0) root         (0)     4588 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/web/events.py
--rw-r--r--   0 root         (0) root         (0)     1945 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/web/health.py
--rw-r--r--   0 root         (0) root         (0)     1655 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/sweepai/web/health_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 23:56:11.729292 sweepai-2.0.0.dev0/sweepai.egg-info/
--rw-r--r--   0 root         (0) root         (0)    48104 2024-04-02 23:56:11.000000 sweepai-2.0.0.dev0/sweepai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3296 2024-04-02 23:56:11.000000 sweepai-2.0.0.dev0/sweepai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 23:56:11.000000 sweepai-2.0.0.dev0/sweepai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2024-04-02 23:56:11.000000 sweepai-2.0.0.dev0/sweepai.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      688 2024-04-02 23:56:11.000000 sweepai-2.0.0.dev0/sweepai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       76 2024-04-02 23:56:11.000000 sweepai-2.0.0.dev0/sweepai.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 23:56:11.729292 sweepai-2.0.0.dev0/tests/
--rw-r--r--   0 root         (0) root         (0)      314 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev0/tests/test_watch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 16:53:31.020885 sweepai-2.0.0.dev1/
+-rw-r--r--   0 root         (0) root         (0)    34523 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    48133 2024-04-03 16:53:31.020885 sweepai-2.0.0.dev1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6420 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 16:53:31.004885 sweepai-2.0.0.dev1/eval/
+-rw-r--r--   0 root         (0) root         (0)    10167 2024-04-02 00:22:38.000000 sweepai-2.0.0.dev1/eval/swe_bench.py
+-rw-r--r--   0 root         (0) root         (0)    10513 2024-04-02 00:22:38.000000 sweepai-2.0.0.dev1/eval/swe_bench_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2009 2024-04-03 16:53:23.000000 sweepai-2.0.0.dev1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 16:53:31.020885 sweepai-2.0.0.dev1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 16:53:31.004885 sweepai-2.0.0.dev1/sweepai/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 16:53:31.008885 sweepai-2.0.0.dev1/sweepai/agents/
+-rw-r--r--   0 root         (0) root         (0)     1185 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/agents/agent_utils.py
+-rw-r--r--   0 root         (0) root         (0)    53205 2024-04-03 05:54:24.000000 sweepai-2.0.0.dev1/sweepai/agents/assistant_function_modify.py
+-rw-r--r--   0 root         (0) root         (0)     4691 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/agents/assistant_functions.py
+-rw-r--r--   0 root         (0) root         (0)    12576 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/agents/assistant_planning.py
+-rw-r--r--   0 root         (0) root         (0)    18975 2024-04-01 21:54:50.000000 sweepai-2.0.0.dev1/sweepai/agents/assistant_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     4052 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/agents/assistant_wrapper_test.py
+-rw-r--r--   0 root         (0) root         (0)     2958 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/agents/complete_code.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/agents/complete_code_test.py
+-rw-r--r--   0 root         (0) root         (0)     2448 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/agents/distill_issue.py
+-rw-r--r--   0 root         (0) root         (0)    27333 2024-03-28 21:42:33.000000 sweepai-2.0.0.dev1/sweepai/agents/modify_bot.py
+-rw-r--r--   0 root         (0) root         (0)     5367 2024-03-28 21:42:33.000000 sweepai-2.0.0.dev1/sweepai/agents/modify_file.py
+-rw-r--r--   0 root         (0) root         (0)     1357 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/agents/pr_description_bot.py
+-rw-r--r--   0 root         (0) root         (0)     3814 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/agents/prune_modify_snippets.py
+-rw-r--r--   0 root         (0) root         (0)    52353 2024-04-01 21:54:50.000000 sweepai-2.0.0.dev1/sweepai/api.py
+-rw-r--r--   0 root         (0) root         (0)      753 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/api_test.py
+-rw-r--r--   0 root         (0) root         (0)    13534 2024-04-02 23:14:46.000000 sweepai-2.0.0.dev1/sweepai/cli.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/cli_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 16:53:31.008885 sweepai-2.0.0.dev1/sweepai/config/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12598 2024-04-03 05:54:24.000000 sweepai-2.0.0.dev1/sweepai/config/client.py
+-rw-r--r--   0 root         (0) root         (0)     9564 2024-04-02 22:54:02.000000 sweepai-2.0.0.dev1/sweepai/config/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 16:53:31.008885 sweepai-2.0.0.dev1/sweepai/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15920 2024-04-02 23:51:20.000000 sweepai-2.0.0.dev1/sweepai/core/chat.py
+-rw-r--r--   0 root         (0) root         (0)    42278 2024-04-03 05:54:24.000000 sweepai-2.0.0.dev1/sweepai/core/context_pruning.py
+-rw-r--r--   0 root         (0) root         (0)    17833 2024-03-26 17:32:09.000000 sweepai-2.0.0.dev1/sweepai/core/entities.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/core/external_searcher.py
+-rw-r--r--   0 root         (0) root         (0)    10630 2024-04-02 18:54:07.000000 sweepai-2.0.0.dev1/sweepai/core/lexical_search.py
+-rw-r--r--   0 root         (0) root         (0)     5826 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/core/post_merge.py
+-rw-r--r--   0 root         (0) root         (0)     4345 2024-04-03 05:54:24.000000 sweepai-2.0.0.dev1/sweepai/core/pr_reader.py
+-rw-r--r--   0 root         (0) root         (0)    36545 2024-03-29 19:15:49.000000 sweepai-2.0.0.dev1/sweepai/core/prompts.py
+-rw-r--r--   0 root         (0) root         (0)    13688 2024-03-31 22:18:38.000000 sweepai-2.0.0.dev1/sweepai/core/reflection_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5377 2024-04-02 00:22:38.000000 sweepai-2.0.0.dev1/sweepai/core/repo_parsing_utils.py
+-rw-r--r--   0 root         (0) root         (0)    52641 2024-04-03 05:54:24.000000 sweepai-2.0.0.dev1/sweepai/core/sweep_bot.py
+-rw-r--r--   0 root         (0) root         (0)     5758 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/core/update_prompts.py
+-rw-r--r--   0 root         (0) root         (0)     9561 2024-04-02 23:24:36.000000 sweepai-2.0.0.dev1/sweepai/core/vector_db.py
+-rw-r--r--   0 root         (0) root         (0)       19 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/global_threads.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 16:53:31.012885 sweepai-2.0.0.dev1/sweepai/handlers/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/handlers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15582 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/handlers/create_pr.py
+-rw-r--r--   0 root         (0) root         (0)     5670 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/handlers/on_button_click.py
+-rw-r--r--   0 root         (0) root         (0)     1569 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/handlers/on_button_click_test.py
+-rw-r--r--   0 root         (0) root         (0)     5247 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/handlers/on_check_suite.py
+-rw-r--r--   0 root         (0) root         (0)    18961 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/handlers/on_comment.py
+-rw-r--r--   0 root         (0) root         (0)     4123 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/handlers/on_merge.py
+-rw-r--r--   0 root         (0) root         (0)    13160 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/handlers/on_merge_conflict.py
+-rw-r--r--   0 root         (0) root         (0)      722 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/handlers/on_review.py
+-rw-r--r--   0 root         (0) root         (0)    86721 2024-03-28 21:42:33.000000 sweepai-2.0.0.dev1/sweepai/handlers/on_ticket.py
+-rw-r--r--   0 root         (0) root         (0)     5262 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/handlers/pr_utils.py
+-rw-r--r--   0 root         (0) root         (0)    10042 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/handlers/stack_pr.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/handlers/stack_pr_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 16:53:31.012885 sweepai-2.0.0.dev1/sweepai/logn/
+-rw-r--r--   0 root         (0) root         (0)       44 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/logn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5942 2024-03-26 17:31:09.000000 sweepai-2.0.0.dev1/sweepai/logn/cache.py
+-rw-r--r--   0 root         (0) root         (0)    11758 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/logn/logn.py
+-rw-r--r--   0 root         (0) root         (0)      376 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/logn/trace_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 16:53:31.020885 sweepai-2.0.0.dev1/sweepai/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3152 2024-04-02 23:52:56.000000 sweepai-2.0.0.dev1/sweepai/utils/anthropic_client.py
+-rw-r--r--   0 root         (0) root         (0)     1980 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/autoimport.py
+-rw-r--r--   0 root         (0) root         (0)     3047 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/buttons.py
+-rw-r--r--   0 root         (0) root         (0)     1830 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/buttons_test.py
+-rw-r--r--   0 root         (0) root         (0)     7850 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/chat_logger.py
+-rw-r--r--   0 root         (0) root         (0)     7882 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/code_tree.py
+-rw-r--r--   0 root         (0) root         (0)      716 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/code_tree_test.py
+-rw-r--r--   0 root         (0) root         (0)      616 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/comment_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/comment_utils_test.py
+-rw-r--r--   0 root         (0) root         (0)     5817 2024-03-30 01:11:28.000000 sweepai-2.0.0.dev1/sweepai/utils/convert_openai_anthropic.py
+-rw-r--r--   0 root         (0) root         (0)    12918 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/diff.py
+-rw-r--r--   0 root         (0) root         (0)     2902 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/diff_test.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/docker_utils.py
+-rw-r--r--   0 root         (0) root         (0)      392 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/docker_utils_test.py
+-rw-r--r--   0 root         (0) root         (0)     2637 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/event_logger.py
+-rw-r--r--   0 root         (0) root         (0)      432 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/file_utils.py
+-rw-r--r--   0 root         (0) root         (0)     6767 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/fuzzy_diff.py
+-rw-r--r--   0 root         (0) root         (0)     2709 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/fuzzy_diff_test.py
+-rw-r--r--   0 root         (0) root         (0)    24266 2024-04-03 05:54:24.000000 sweepai-2.0.0.dev1/sweepai/utils/github_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2291 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/github_utils_test.py
+-rw-r--r--   0 root         (0) root         (0)      100 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/hash.py
+-rw-r--r--   0 root         (0) root         (0)     1616 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/html_extractor.py
+-rw-r--r--   0 root         (0) root         (0)     3115 2024-04-03 05:54:24.000000 sweepai-2.0.0.dev1/sweepai/utils/modify_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5802 2024-04-03 05:54:24.000000 sweepai-2.0.0.dev1/sweepai/utils/multi_query.py
+-rw-r--r--   0 root         (0) root         (0)    21464 2024-03-31 22:18:38.000000 sweepai-2.0.0.dev1/sweepai/utils/openai_listwise_reranker.py
+-rw-r--r--   0 root         (0) root         (0)    11068 2024-03-26 22:42:55.000000 sweepai-2.0.0.dev1/sweepai/utils/openai_proxy.py
+-rw-r--r--   0 root         (0) root         (0)     4220 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/openai_proxy_test.py
+-rw-r--r--   0 root         (0) root         (0)     1422 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/patch_utils.py
+-rw-r--r--   0 root         (0) root         (0)     9641 2024-03-28 21:42:33.000000 sweepai-2.0.0.dev1/sweepai/utils/progress.py
+-rw-r--r--   0 root         (0) root         (0)      384 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/progress_test.py
+-rw-r--r--   0 root         (0) root         (0)     8711 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/prompt_constructor.py
+-rw-r--r--   0 root         (0) root         (0)      924 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/regex_utils.py
+-rw-r--r--   0 root         (0) root         (0)      841 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/safe_pqueue.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/scorer.py
+-rw-r--r--   0 root         (0) root         (0)      791 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/scorer_test.py
+-rw-r--r--   0 root         (0) root         (0)    13788 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/search_and_replace.py
+-rw-r--r--   0 root         (0) root         (0)     2101 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/search_and_replace_test.py
+-rw-r--r--   0 root         (0) root         (0)     4596 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/str_utils.py
+-rw-r--r--   0 root         (0) root         (0)    12066 2024-04-03 05:54:24.000000 sweepai-2.0.0.dev1/sweepai/utils/ticket_utils.py
+-rw-r--r--   0 root         (0) root         (0)      606 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/timer.py
+-rw-r--r--   0 root         (0) root         (0)     7346 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/tree_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2963 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/user_settings.py
+-rw-r--r--   0 root         (0) root         (0)    21346 2024-04-02 01:55:11.000000 sweepai-2.0.0.dev1/sweepai/utils/utils.py
+-rw-r--r--   0 root         (0) root         (0)      586 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/utils_test.py
+-rw-r--r--   0 root         (0) root         (0)     3989 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/watch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 16:53:31.020885 sweepai-2.0.0.dev1/sweepai/web/
+-rw-r--r--   0 root         (0) root         (0)     4588 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/web/events.py
+-rw-r--r--   0 root         (0) root         (0)     1945 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/web/health.py
+-rw-r--r--   0 root         (0) root         (0)     1655 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/web/health_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 16:53:31.020885 sweepai-2.0.0.dev1/sweepai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    48133 2024-04-03 16:53:30.000000 sweepai-2.0.0.dev1/sweepai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3296 2024-04-03 16:53:31.000000 sweepai-2.0.0.dev1/sweepai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 16:53:30.000000 sweepai-2.0.0.dev1/sweepai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2024-04-03 16:53:30.000000 sweepai-2.0.0.dev1/sweepai.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      702 2024-04-03 16:53:30.000000 sweepai-2.0.0.dev1/sweepai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       81 2024-04-03 16:53:30.000000 sweepai-2.0.0.dev1/sweepai.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 16:53:31.020885 sweepai-2.0.0.dev1/tests/
+-rw-r--r--   0 root         (0) root         (0)      314 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/tests/test_watch.py
```

### Comparing `sweepai-2.0.0.dev0/LICENSE` & `sweepai-2.0.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/PKG-INFO` & `sweepai-2.0.0.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweepai
-Version: 2.0.0.dev0
+Version: 2.0.0.dev1
 Summary: Sweep fixes GitHub issues
 Author-email: Kevin Lu <kevin@sweep.dev>, William Zeng <william@sweep.dev>, Martin Ye <martin@sweep.dev>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -709,14 +709,15 @@
 Requires-Dist: jinja2==3.1.3
 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: uvicorn==0.29.0
 Requires-Dist: pylint==3.1.0
 Requires-Dist: parea-ai==0.2.114
 Requires-Dist: voyageai==0.2.1
 Requires-Dist: boto3==1.34.70
+Requires-Dist: scipy==1.12.0
 
 <p align="center">
     <img src="https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-3e61f57ad233">
 </p>
 <p align="center">
     <i>Github Issues ⟶&nbsp; Pull Requests! </i>
 </p>
```

### Comparing `sweepai-2.0.0.dev0/README.md` & `sweepai-2.0.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/eval/swe_bench.py` & `sweepai-2.0.0.dev1/eval/swe_bench.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/eval/swe_bench_utils.py` & `sweepai-2.0.0.dev1/eval/swe_bench_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/pyproject.toml` & `sweepai-2.0.0.dev1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 Community = "https://discord.gg/sweep"
 Documentation = "https://docs.sweep.dev"
 Homepage = "https://sweep.dev"
 "Bug Tracker" = "https://github.com/sweepai/sweep/issues"
 
 [project]
 name = "sweepai"
-version = "2.0.0.dev0"
+version = "2.0.0.dev1"
 description = "Sweep fixes GitHub issues"
 authors = [
     {name = "Kevin Lu", email = "kevin@sweep.dev"},
     {name = "William Zeng", email = "william@sweep.dev"},
     {name = "Martin Ye", email = "martin@sweep.dev"},
 ]
 readme = "README.md"
@@ -68,14 +68,15 @@
   "jinja2==3.1.3",
   "tiktoken==0.6.0",
   "uvicorn==0.29.0",
   "pylint==3.1.0",
   "parea-ai==0.2.114",
   "voyageai==0.2.1",
   "boto3==1.34.70",
+  "scipy==1.12.0"
 ]
 
 [tool.isort]
 profile = "black"
 
 [tool.black]
 string-normalization = false
```

### Comparing `sweepai-2.0.0.dev0/sweepai/agents/agent_utils.py` & `sweepai-2.0.0.dev1/sweepai/agents/agent_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/agents/assistant_function_modify.py` & `sweepai-2.0.0.dev1/sweepai/agents/assistant_function_modify.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from sweepai.agents.agent_utils import ensure_additional_messages_length
 from sweepai.config.client import SweepConfig
 from sweepai.core.entities import AssistantRaisedException, FileChangeRequest, Message
 from sweepai.logn.cache import file_cache
 from sweepai.utils.chat_logger import ChatLogger, discord_log_error
 from sweepai.utils.diff import generate_diff
 from sweepai.utils.file_utils import read_file_with_fallback_encodings
-from sweepai.utils.github_utils import ClonedRepo
+from sweepai.utils.github_utils import ClonedRepo, update_file
 from sweepai.utils.progress import AssistantConversation, TicketProgress
 from sweepai.utils.utils import chunk_code, get_check_results
 from sweepai.utils.modify_utils import post_process_rg_output, manual_code_check
 
 # Pre-amble using ideas from https://github.com/paul-gauthier/aider/blob/main/aider/coders/udiff_prompts.py
 # Doesn't regress on the benchmark but improves average code generated and avoids empty comments.
 
@@ -577,14 +577,17 @@
                         if error_message:
                             break
                         success_message = ""
                         section_letter = tool_call["section_id"].strip()
                         section_id = excel_col_to_int(section_letter)
                         original_code = tool_call["original_code"].strip("\n")
                         new_code = tool_call["new_code"].strip("\n")
+                        if new_code == original_code:
+                            error_message += "The new_code and original_code are the same. Are you CERTAIN this change needs to be made? If you are certain this change needs to be made, MAKE SURE that the new_code and original_code are NOT the same."
+                            break
                         # get the chunks and contents for the file
                         file_chunks = deepcopy(modify_files_dict[file_name]['chunks'])  
                         file_contents = modify_files_dict[file_name]['contents']
                         warning_message = ""
                         if section_id >= len(file_chunks):
                             error_message = f"Could not find section {section_letter} in file {file_name}, which has {len(file_chunks)} sections."
                             break
@@ -687,15 +690,15 @@
                             error_message
                         )
 
                     if not error_message:
                         success_message = (
                             f"SUCCESS\n\nThe following changes have been applied to {file_name}:\n\n"
                             + generate_diff(file_contents, new_contents)
-                        ) + f"{warning_message}\n\nYou can continue to make changes to the code sections and call the SearchAndReplace tool again, or go back to searching for keywords using the KeywordSearch tool, which is great for finding all definitions or usages of a function or class."
+                        ) + f"{warning_message}\n\nYou can continue to make changes to the code sections and call the make_change tool again, or go back to searching for keywords using the search_codebase tool, which is great for finding all definitions or usages of a function or class."
                         # set contents
                         modify_files_dict[file_name]['contents'] = new_contents
                         modify_files_dict[file_name]['chunks'] = file_chunks
                         logger.info(success_message)
 
                         success_message = create_tool_call_response(tool_name, f"SUCCESS\n\n{success_message}")
                         
@@ -818,21 +821,23 @@
                                 )
                         else: # search whole codebase
                             logger.info(f"Searching for keyword {keyword} in the entire codebase.")
                             rg_command = ["rg", "-n", "-i" , f'"{keyword}"', cwd]
                             try:
                                 # update the cloned repo before running ripgrep as it is possible some of the files have been editted
                                 for file_name, file_data in modify_files_dict.items():
-                                    cloned_repo.update_file(file_name, file_data["contents"])
+                                    updated = update_file(cloned_repo.repo_dir, file_name, file_data["contents"])
+                                    if not updated:
+                                        raise Exception(f"Failed to update file {file_name} in the cloned repo.")
                             except Exception as e:
                                 logger.error(f"FAILURE: An Error occured while trying to update the cloned repo on file {file_name}: {e}")
                                 error_message = f"FAILURE: An Error occured while trying to update the cloned repo on file {file_name}: {e}\n"
                                 # attempt to undo the updates
                                 for file_name, file_data in modify_files_dict.items():
-                                    cloned_repo.update_file(file_name, file_data["original_contents"])
+                                    update_file(cloned_repo.repo_dir, file_name, file_data["original_contents"])
                                 
                             try:
                                 result = subprocess.run(" ".join(rg_command), text=True, shell=True, capture_output=True)
                                 output = result.stdout
                                 if output:
                                     # post process rip grep output to be more condensed
                                     rg_output_pretty = post_process_rg_output(cwd, sweep_config, output)
@@ -841,21 +846,23 @@
                             except Exception as e:
                                 logger.error(f"FAILURE: An Error occured while trying to reset the cloned repo on file {file_name}: {e}\n")
                                 error_message += f"FAILURE: An Error occured while trying to rest the cloned repo on file {file_name}: {e}\n"
 
                             try:
                                 # reset cloned_repo to original state
                                 for file_name, file_data in modify_files_dict.items():
-                                    cloned_repo.update_file(file_name, file_data["original_contents"])
+                                    updated = update_file(cloned_repo.repo_dir, file_name, file_data["original_contents"])
+                                    if not updated:
+                                        raise Exception(f"Failed to update file {file_name} in the cloned repo.")
                             except Exception as e:
                                 logger.error(f"FAILURE: An Error occured while trying to update the cloned repo on file {file_name}: {e}")
                                 error_message = f"FAILURE: An Error occured while trying to update the cloned repo on file {file_name}: {e}"
 
                             if not error_message:
-                                success_message = f"SUCCESS\n\nHere are the search_codebase results:\n{rg_output_pretty}\n\n You can use these results to revise your plan by calling the analyze_problem_and_propose_plan tool again. You can also call the analyze_and_identify_changes tool again."
+                                success_message = f"Here are the search_codebase results:\n{rg_output_pretty}\n\n You can use these results to revise your plan by calling the analyze_problem_and_propose_plan tool again. You can also call the analyze_and_identify_changes tool again."
                                 logger.debug(f"SUCCESS\n\nHere are the search_codebase results:\n{rg_output_pretty}\n\n")
 
                     if error_message:
                         logger.debug(f"ERROR in search_codebase\n\n{error_message}")
                         error_message = create_tool_call_response(tool_name, f"ERROR\n\n{error_message}")
                         tool_name, tool_call = assistant_generator.send(
                             error_message
```

### Comparing `sweepai-2.0.0.dev0/sweepai/agents/assistant_functions.py` & `sweepai-2.0.0.dev1/sweepai/agents/assistant_functions.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/agents/assistant_planning.py` & `sweepai-2.0.0.dev1/sweepai/agents/assistant_planning.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/agents/assistant_wrapper.py` & `sweepai-2.0.0.dev1/sweepai/agents/assistant_wrapper.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/agents/assistant_wrapper_test.py` & `sweepai-2.0.0.dev1/sweepai/agents/assistant_wrapper_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/agents/complete_code.py` & `sweepai-2.0.0.dev1/sweepai/agents/complete_code.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/agents/complete_code_test.py` & `sweepai-2.0.0.dev1/sweepai/agents/complete_code_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/agents/distill_issue.py` & `sweepai-2.0.0.dev1/sweepai/agents/distill_issue.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/agents/modify_bot.py` & `sweepai-2.0.0.dev1/sweepai/agents/modify_bot.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/agents/modify_file.py` & `sweepai-2.0.0.dev1/sweepai/agents/modify_file.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/agents/pr_description_bot.py` & `sweepai-2.0.0.dev1/sweepai/agents/pr_description_bot.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/agents/prune_modify_snippets.py` & `sweepai-2.0.0.dev1/sweepai/agents/prune_modify_snippets.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/api.py` & `sweepai-2.0.0.dev1/sweepai/api.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/api_test.py` & `sweepai-2.0.0.dev1/sweepai/api_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/cli.py` & `sweepai-2.0.0.dev1/sweepai/cli.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/cli_test.py` & `sweepai-2.0.0.dev1/sweepai/cli_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/config/client.py` & `sweepai-2.0.0.dev1/sweepai/config/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,16 +105,20 @@
         ".dfm",
         ".feature",
         "sweep.yaml",
         "pnpm-lock.yaml",
         "LICENSE",
         "poetry.lock",
     ]
+    # cutoff for when we output truncated versions of strings, this is an arbitrary number and can be changed
+    truncation_cutoff: int = 20000
     # Image formats
     max_file_limit: int = 60_000
+    # github comments
+    max_github_comment_body_length: int = 65535
 
     def to_yaml(self) -> str:
         return yaml.safe_dump(self.dict())
 
     @classmethod
     def from_yaml(cls, yaml_str: str) -> "SweepConfig":
         data = yaml.safe_load(yaml_str)
```

### Comparing `sweepai-2.0.0.dev0/sweepai/config/server.py` & `sweepai-2.0.0.dev1/sweepai/config/server.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/core/chat.py` & `sweepai-2.0.0.dev1/sweepai/core/chat.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/core/context_pruning.py` & `sweepai-2.0.0.dev1/sweepai/core/context_pruning.py`

 * *Files 0% similar despite different names*

```diff
@@ -588,15 +588,16 @@
                 user_prompt,
                 repo_context_manager,
                 problem_statement=query,
             )
         except openai.BadRequestError as e:  # sometimes means that run has expired
             logger.exception(e)
         if len(repo_context_manager.current_top_snippets) == 0:
-            repo_context_manager.current_top_snippets = old_top_snippets
+            raise Exception("No snippets found")
+            repo_context_manager.current_top_snippets = old_top_snippets[:20]
         return repo_context_manager
     except Exception as e:
         logger.exception(e)
         return repo_context_manager
 
 
 def update_assistant_conversation(
@@ -717,21 +718,21 @@
                 and file_path in current_top_snippets_string
                 and valid_path
             ):
                 output = f"FAILURE: {file_path} is already in the selected snippets."
             elif valid_path:
                 suffix = f'\nIf you are CERTAIN this file is RELEVANT, call store_file with the same parameters ({{"file_path": "{file_path}"}}).'
                 output = f'Here are the contents of `{file_path}:`\n```\n{file_contents}\n```'
-                if file_path not in [snippet.file_path for snippet in rcm.current_top_snippets]:
+                if file_path not in [snippet.file_path for snippet in repo_context_manager.current_top_snippets]:
                     output += suffix
             else:
                 output = (
                     "FAILURE: This file path does not exist. Please try a new path."
                 )
-        except Exception:
+        except FileNotFoundError:
             file_contents = ""
             similar_file_paths = "\n".join(
                 [
                     f"- {path}"
                     for path in repo_context_manager.cloned_repo.get_similar_file_paths(
                         file_path
                     )
@@ -886,15 +887,15 @@
             )
             for function_call in function_calls:
                 function_output = handle_function_call(repo_context_manager, function_call)
                 if PLAN_SUBMITTED_MESSAGE in function_output:
                     return chat_gpt.messages
             if len(function_calls) == 0:
                 function_output = "No function calls were made or your last function call was incorrectly formatted. The correct syntax for function calling is this:\n" \
-                    + "<function_call>\n<invoke>\n<tool_name>tool_name</tool_name>\n<parameters>\n<param_name>param_value</param_name>\n</parameters>\n</invoke>\n</function_calls>" + "\n\nIf you would like to submit the plan, call the submit function."
+                    + "<function_call>\n<invoke>\n<tool_name>tool_name</tool_name>\n<parameters>\n<param_name>param_value</param_name>\n</parameters>\n</invoke>\n</function_call>" + "\n\nIf you would like to submit the plan, call the submit function."
                 bad_call_count += 1
                 if bad_call_count >= 3:
                     return chat_gpt.messages # set to three, which seems alright
             try:
                 function_calls_string = chat_gpt.chat_anthropic(
                     content=function_output,
                     model=CLAUDE_MODEL,
```

### Comparing `sweepai-2.0.0.dev0/sweepai/core/entities.py` & `sweepai-2.0.0.dev1/sweepai/core/entities.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/core/external_searcher.py` & `sweepai-2.0.0.dev1/sweepai/core/external_searcher.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/core/lexical_search.py` & `sweepai-2.0.0.dev1/sweepai/core/lexical_search.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/core/post_merge.py` & `sweepai-2.0.0.dev1/sweepai/core/post_merge.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/core/prompts.py` & `sweepai-2.0.0.dev1/sweepai/core/prompts.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/core/reflection_utils.py` & `sweepai-2.0.0.dev1/sweepai/core/reflection_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/core/repo_parsing_utils.py` & `sweepai-2.0.0.dev1/sweepai/core/repo_parsing_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/core/sweep_bot.py` & `sweepai-2.0.0.dev1/sweepai/core/sweep_bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -728,17 +728,19 @@
                 )
 
                 first_chars_in_instructions = file_change_request.instructions.lower()
                 first_chars_in_instructions = first_chars_in_instructions[
                     : min(60, len(first_chars_in_instructions))
                 ]
                 # add context on which fcr it is currently on and how many are left
-                all_fcrs_strings = ", ".join(file_change_request.relevant_files)
-                current_fcr_strings = f"To solve the user's request you will modify/create the following {len(file_change_request.relevant_files)} files: {all_fcrs_strings}. You are currently modifying {file_change_request.filename}!"
-                additional_messages += [
+                all_fcrs_strings = ", ".join([file.filename for file in file_change_requests])
+                current_fcr_strings = f"To solve the user's request you will modify/create the following {len(file_change_requests)} files: {all_fcrs_strings}. You are currently modifying {file_change_request.filename}!"
+                # additional_messages should be reset for each file change request
+                additional_messages_copy = copy.deepcopy(additional_messages)
+                additional_messages_copy += [
                     Message(
                         role="user",
                         content=current_fcr_strings,
                         key="instructions",
                     )
                 ]
                 match file_change_request.change_type:
@@ -806,15 +808,15 @@
                             assistant_conversation=(
                                 self.ticket_progress.coding_progress.assistant_conversations[
                                     i
                                 ]
                                 if self.ticket_progress
                                 else None
                             ),
-                            additional_messages=additional_messages,
+                            additional_messages=additional_messages_copy,
                             previous_modify_files_dict=previous_modify_files_dict,
                         )
                         # update previous_modify_files_dict
                         if not previous_modify_files_dict:
                             previous_modify_files_dict = {}
                         if new_file_contents:
                             for key, value in new_file_contents.items():
```

### Comparing `sweepai-2.0.0.dev0/sweepai/core/update_prompts.py` & `sweepai-2.0.0.dev1/sweepai/core/update_prompts.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/core/vector_db.py` & `sweepai-2.0.0.dev1/sweepai/core/vector_db.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/handlers/create_pr.py` & `sweepai-2.0.0.dev1/sweepai/handlers/create_pr.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/handlers/on_button_click.py` & `sweepai-2.0.0.dev1/sweepai/handlers/on_button_click.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/handlers/on_button_click_test.py` & `sweepai-2.0.0.dev1/sweepai/handlers/on_button_click_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/handlers/on_check_suite.py` & `sweepai-2.0.0.dev1/sweepai/handlers/on_check_suite.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/handlers/on_comment.py` & `sweepai-2.0.0.dev1/sweepai/handlers/on_comment.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/handlers/on_merge.py` & `sweepai-2.0.0.dev1/sweepai/handlers/on_merge.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/handlers/on_merge_conflict.py` & `sweepai-2.0.0.dev1/sweepai/handlers/on_merge_conflict.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/handlers/on_review.py` & `sweepai-2.0.0.dev1/sweepai/handlers/on_review.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/handlers/on_ticket.py` & `sweepai-2.0.0.dev1/sweepai/handlers/on_ticket.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/handlers/pr_utils.py` & `sweepai-2.0.0.dev1/sweepai/handlers/pr_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/handlers/stack_pr.py` & `sweepai-2.0.0.dev1/sweepai/handlers/stack_pr.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/handlers/stack_pr_test.py` & `sweepai-2.0.0.dev1/sweepai/handlers/stack_pr_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/logn/cache.py` & `sweepai-2.0.0.dev1/sweepai/logn/cache.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/logn/logn.py` & `sweepai-2.0.0.dev1/sweepai/logn/logn.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/anthropic_client.py` & `sweepai-2.0.0.dev1/sweepai/utils/anthropic_client.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/autoimport.py` & `sweepai-2.0.0.dev1/sweepai/utils/autoimport.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/buttons.py` & `sweepai-2.0.0.dev1/sweepai/utils/buttons.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/buttons_test.py` & `sweepai-2.0.0.dev1/sweepai/utils/buttons_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/chat_logger.py` & `sweepai-2.0.0.dev1/sweepai/utils/chat_logger.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/code_tree.py` & `sweepai-2.0.0.dev1/sweepai/utils/code_tree.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/code_tree_test.py` & `sweepai-2.0.0.dev1/sweepai/utils/code_tree_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/comment_utils.py` & `sweepai-2.0.0.dev1/sweepai/utils/comment_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/comment_utils_test.py` & `sweepai-2.0.0.dev1/sweepai/utils/comment_utils_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/convert_openai_anthropic.py` & `sweepai-2.0.0.dev1/sweepai/utils/convert_openai_anthropic.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/diff.py` & `sweepai-2.0.0.dev1/sweepai/utils/diff.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/diff_test.py` & `sweepai-2.0.0.dev1/sweepai/utils/diff_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/docker_utils.py` & `sweepai-2.0.0.dev1/sweepai/utils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/event_logger.py` & `sweepai-2.0.0.dev1/sweepai/utils/event_logger.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/fuzzy_diff.py` & `sweepai-2.0.0.dev1/sweepai/utils/fuzzy_diff.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/fuzzy_diff_test.py` & `sweepai-2.0.0.dev1/sweepai/utils/fuzzy_diff_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/github_utils.py` & `sweepai-2.0.0.dev1/sweepai/utils/github_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -463,29 +463,25 @@
             key=lambda file_path: file_path_to_ratio[file_path],
             reverse=True,
         )
         # this allows 'config.py' to return 'sweepai/config/server.py', 'sweepai/config/client.py', 'sweepai/config/__init__.py' and no more
         filtered_files_without_matching_name = list(filter(lambda file_path: file_path_to_ratio[file_path] > 50, files_without_matching_name))
         all_files = files_with_matching_name + filtered_files_without_matching_name
         return all_files[:limit]
-    
-    def update_file(self, file_path: str, new_contents: str):
-        local_path = (
-            f"{self.repo_dir}{file_path}"
-            if file_path.startswith("/")
-            else f"{self.repo_dir}/{file_path}"
-        )
-        try:
-            with open(local_path, "w", encoding="utf-8", errors="replace") as f:
-                f.write(new_contents)
-            return True
-        except Exception as e:
-            logger.error(f"Failed to update file: {e}")
-            return False
 
+# updates a file with new_contents, returns True if successful
+def update_file(root_dir: str, file_path: str, new_contents: str):
+    local_path = os.path.join(root_dir, file_path)
+    try:
+        with open(local_path, "w") as f:
+            f.write(new_contents)
+        return True
+    except Exception as e:
+        logger.error(f"Failed to update file: {e}")
+        return False
 
 @dataclass
 class MockClonedRepo(ClonedRepo):
     _repo_dir: str = ""
     git_repo: git.Repo | None = None
 
     def __init__(
```

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/github_utils_test.py` & `sweepai-2.0.0.dev1/sweepai/utils/github_utils_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/html_extractor.py` & `sweepai-2.0.0.dev1/sweepai/utils/html_extractor.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/modify_utils.py` & `sweepai-2.0.0.dev1/sweepai/utils/modify_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,21 +12,23 @@
         filename, content = line.split(":", 1)
         filename = filename[len(root_directory) + 1:]
         if not sweep_config.is_file_excluded_aggressive(root_directory, filename):
             file_output_dict[filename].append(content)
     
     # determine if we need to truncate the output
     total_output_length = sum([len(line) for content in file_output_dict.values() for line in content])
-    if total_output_length > 20000:
+    if total_output_length > sweep_config.truncation_cutoff:
         for filename, content in file_output_dict.items():
-            processed_output += f"File: {filename} had the following matching lines of code (some lines have been truncated):\n"
-            if len(content) < 3:
+            processed_output += f"File: {filename} had the following matching lines of code"
+            if len(content) < 4:
+                processed_output += " :\n"
                 for line in content:
                     processed_output += f"{line}\n"
             else:
+                processed_output += " (some lines have been truncated):\n"
                 line1 = content[0]
                 line2 = content[-1]
                 if len(line1) > 200:
                     line1 = line1[:20] + " ..."
                 if len(line2) > 200:
                     line2 = line2[:20] + " ..."
                 processed_output += f"{line1}\n"
```

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/multi_query.py` & `sweepai-2.0.0.dev1/sweepai/utils/multi_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,45 +14,48 @@
 
 2. Solution
 
 Describe thoroughly in extreme detail what the ideal code fix would look like:
 - Dive deep into the low-level implementation details of how you would change each file. Explain the logic, algorithms, data structures, etc. 
 - Explicitly call out any helper functions, utility modules, libraries or APIs you would leverage.
 - Carefully consider ALL parts of the codebase that could be relevant, including:
-  - Database schemas, models, and query logic 
   - Type definitions, interfaces, enums, constants
   - Shared utility code for common operations
+  - Database schemas, models, mutators and query logic 
+  - User-facing messages, error messages, localization, i18n
+  - Exception handling, error recovery, retries, fallbacks
   - API routes, request/response handling, serialization
   - UI components, client-side logic, event handlers
   - Backend services, data processing, business logic
-  - User-facing copy, error messages, localization, i18n
   - Logging, monitoring, metrics, error tracking, observability, o11y
   - Auth flows, session management, encryption
   - Infrastructure, CI/CD, deployments, config
 - List out any unfamiliar domain terms to search for to better understand schemas, types, relationships between entities, etc. Finding data models is key.
 - Rate limiting, caching and other cross-cutting concerns could be very relevant for issues with scale or performance.
 
 3. Queries
 
-Generate a list of 15 highly specific, focused "where" queries to use as vector database search queries to find the most relevant code sections to directly resolve the GitHub issue.
+Generate a list of 10 diverse, highly specific, focused "where" queries to use as vector database search queries to find the most relevant code sections to directly resolve the GitHub issue.
 - Reference very specific functions, variables, classes, endpoints, etc. using exact names.
 - Describe the purpose and behavior of the code in detail to differentiate it. 
 - Ask about granular logic within individual functions/methods.
 - Mention adjacent code like schemas, configs, and helpers to establish context.
 - Use verbose natural language that mirrors the terminology in the codebase.
 - Aim for high specificity to pinpoint the most relevant code in a large codebase.
 
 Format your response like this:
 
 <summary>
 [Brief 1-2 sentence summary of the key points of the issue]
 </summary>
 
 <solution>
-[1-2 sentences describing what an ideal fix would change in the code and how] Relevant parts of the codebase that could be used in the solution include:
+[detailed sentences describing what an ideal fix would change in the code and how
+
+Exhaustive list of relevant parts of the codebase that could be used in the solution include:
 - [Module, service, function or endpoint 1] 
 - [Module, service, function or endpoint 2]
 - [etc.]
 </solution>
 
 <queries>
 <query>Where is the [extremely specific description of code section 1]?</query>
```

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/openai_listwise_reranker.py` & `sweepai-2.0.0.dev1/sweepai/utils/openai_listwise_reranker.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/openai_proxy.py` & `sweepai-2.0.0.dev1/sweepai/utils/openai_proxy.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/openai_proxy_test.py` & `sweepai-2.0.0.dev1/sweepai/utils/openai_proxy_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/patch_utils.py` & `sweepai-2.0.0.dev1/sweepai/utils/patch_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/progress.py` & `sweepai-2.0.0.dev1/sweepai/utils/progress.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/prompt_constructor.py` & `sweepai-2.0.0.dev1/sweepai/utils/prompt_constructor.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/regex_utils.py` & `sweepai-2.0.0.dev1/sweepai/utils/regex_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/safe_pqueue.py` & `sweepai-2.0.0.dev1/sweepai/utils/safe_pqueue.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/scorer.py` & `sweepai-2.0.0.dev1/sweepai/utils/scorer.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/scorer_test.py` & `sweepai-2.0.0.dev1/sweepai/utils/scorer_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/search_and_replace.py` & `sweepai-2.0.0.dev1/sweepai/utils/search_and_replace.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/search_and_replace_test.py` & `sweepai-2.0.0.dev1/sweepai/utils/search_and_replace_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/str_utils.py` & `sweepai-2.0.0.dev1/sweepai/utils/str_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/ticket_utils.py` & `sweepai-2.0.0.dev1/sweepai/utils/ticket_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,48 +134,50 @@
 ):
     ranked_snippets_list, snippets, content_to_lexical_score_list = multi_get_top_k_snippets(
         cloned_repo, [query], ticket_progress, k
     )
     return ranked_snippets_list[0], snippets, content_to_lexical_score_list[0]
 
 
-def prep_snippets(
+def multi_prep_snippets(
     cloned_repo: ClonedRepo,
-    query: str,
+    queries: list[str],
     ticket_progress: TicketProgress | None = None,
     k: int = 15,
     skip_reranking: bool = False,
-    use_multi_query: bool = True,
 ):
-    if use_multi_query:
+    """
+    Assume 0th index is the main query.
+    """
+    rank_fusion_offset = 0
+    if len(queries) > 1:
         logger.info("Using multi query...")
-        queries = [query, *generate_multi_queries(query)]
         ranked_snippets_list, snippets, content_to_lexical_score_list = multi_get_top_k_snippets(
             cloned_repo, queries, ticket_progress, k * 3 # k * 3 to have enough snippets to rerank
         )
         # Use RRF to rerank snippets
         content_to_lexical_score = defaultdict(float)
         for i, ordered_snippets in enumerate(ranked_snippets_list):
             for j, snippet in enumerate(ordered_snippets):
-                content_to_lexical_score[snippet.denotation] += content_to_lexical_score_list[i][snippet.denotation] * (1 / (j + 1))
+                content_to_lexical_score[snippet.denotation] += content_to_lexical_score_list[i][snippet.denotation] * (1 / (rank_fusion_offset + j + 1))
         ranked_snippets = sorted(
             snippets,
             key=lambda snippet: content_to_lexical_score[snippet.denotation],
             reverse=True,
         )[:k]
     else:
         ranked_snippets, snippets, content_to_lexical_score = get_top_k_snippets(
-            cloned_repo, query, ticket_progress, k
+            cloned_repo, queries[0], ticket_progress, k
         )
     if ticket_progress:
         ticket_progress.search_progress.retrieved_snippets = ranked_snippets
         ticket_progress.save()
     # you can use snippet.denotation and snippet.get_snippet()
     if not skip_reranking:
-        ranked_snippets[:NUM_SNIPPETS_TO_RERANK] = listwise_rerank_snippets(query, ranked_snippets[:NUM_SNIPPETS_TO_RERANK])
+        ranked_snippets[:NUM_SNIPPETS_TO_RERANK] = listwise_rerank_snippets(queries[0], ranked_snippets[:NUM_SNIPPETS_TO_RERANK])
     snippet_paths = [snippet.file_path for snippet in ranked_snippets]
     prefixes = []
     for snippet_path in snippet_paths:
         snippet_depth = len(snippet_path.split("/"))
         for idx in range(snippet_depth):  # heuristic
             if idx > snippet_depth // 2:
                 prefixes.append("/".join(snippet_path.split("/")[:idx]) + "/")
@@ -190,14 +192,29 @@
         current_top_snippets=ranked_snippets,
         snippets=snippets,
         snippet_scores=content_to_lexical_score,
         cloned_repo=cloned_repo,
     )
     return repo_context_manager
 
+def prep_snippets(
+    cloned_repo: ClonedRepo,
+    query: str,
+    ticket_progress: TicketProgress | None = None,
+    k: int = 15,
+    skip_reranking: bool = False,
+    use_multi_query: bool = True,
+):
+    if use_multi_query:
+        queries = [query, *generate_multi_queries(query)]
+    else:
+        queries = [query]
+    return multi_prep_snippets(
+        cloned_repo, queries, ticket_progress, k, skip_reranking
+    )
 
 def fetch_relevant_files(
     cloned_repo,
     title,
     summary,
     replies_text,
     username,
@@ -321,13 +338,19 @@
 if __name__ == "__main__":
     from sweepai.utils.github_utils import MockClonedRepo
 
     cloned_repo = MockClonedRepo(
         _repo_dir="/tmp/sweep",
         repo_full_name="sweepai/sweep",
     )
+    cloned_repo = MockClonedRepo(
+        _repo_dir="/tmp/pulse-alp",
+        repo_full_name="trilogy-group/pulse-alp",
+    )
     rcm = prep_snippets(
         cloned_repo,
-        "I am trying to set up payment processing in my app using Stripe, but I keep getting a 400 error when I try to create a payment intent. I have checked the API key and the request body, but I can't figure out what's wrong. Here is the error message I'm getting: 'Invalid request: request parameters are invalid'. I have attached the relevant code snippets below. Can you help me find the part of the code that is causing this error?",
+        # "I am trying to set up payment processing in my app using Stripe, but I keep getting a 400 error when I try to create a payment intent. I have checked the API key and the request body, but I can't figure out what's wrong. Here is the error message I'm getting: 'Invalid request: request parameters are invalid'. I have attached the relevant code snippets below. Can you help me find the part of the code that is causing this error?",
+        "Where can I find the section that checks if assembly line workers are active or disabled?",
+        use_multi_query=False,
         skip_reranking=True
     )
     breakpoint()
```

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/timer.py` & `sweepai-2.0.0.dev1/sweepai/utils/timer.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/tree_utils.py` & `sweepai-2.0.0.dev1/sweepai/utils/tree_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/user_settings.py` & `sweepai-2.0.0.dev1/sweepai/utils/user_settings.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/utils.py` & `sweepai-2.0.0.dev1/sweepai/utils/utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/utils/utils_test.py` & `sweepai-2.0.0.dev1/sweepai/utils/utils_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/watch.py` & `sweepai-2.0.0.dev1/sweepai/watch.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/web/events.py` & `sweepai-2.0.0.dev1/sweepai/web/events.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/web/health.py` & `sweepai-2.0.0.dev1/sweepai/web/health.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai/web/health_test.py` & `sweepai-2.0.0.dev1/sweepai/web/health_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai.egg-info/PKG-INFO` & `sweepai-2.0.0.dev1/sweepai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweepai
-Version: 2.0.0.dev0
+Version: 2.0.0.dev1
 Summary: Sweep fixes GitHub issues
 Author-email: Kevin Lu <kevin@sweep.dev>, William Zeng <william@sweep.dev>, Martin Ye <martin@sweep.dev>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -709,14 +709,15 @@
 Requires-Dist: jinja2==3.1.3
 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: uvicorn==0.29.0
 Requires-Dist: pylint==3.1.0
 Requires-Dist: parea-ai==0.2.114
 Requires-Dist: voyageai==0.2.1
 Requires-Dist: boto3==1.34.70
+Requires-Dist: scipy==1.12.0
 
 <p align="center">
     <img src="https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-3e61f57ad233">
 </p>
 <p align="center">
     <i>Github Issues ⟶&nbsp; Pull Requests! </i>
 </p>
```

### Comparing `sweepai-2.0.0.dev0/sweepai.egg-info/SOURCES.txt` & `sweepai-2.0.0.dev1/sweepai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev0/sweepai.egg-info/requires.txt` & `sweepai-2.0.0.dev1/sweepai.egg-info/requires.txt`

 * *Files 21% similar despite different names*

```diff
@@ -34,7 +34,8 @@
 jinja2==3.1.3
 tiktoken==0.6.0
 uvicorn==0.29.0
 pylint==3.1.0
 parea-ai==0.2.114
 voyageai==0.2.1
 boto3==1.34.70
+scipy==1.12.0
```

