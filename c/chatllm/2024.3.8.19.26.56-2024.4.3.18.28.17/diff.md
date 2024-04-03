# Comparing `tmp/chatllm-2024.3.8.19.26.56.tar.gz` & `tmp/chatllm-2024.4.3.18.28.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatllm-2024.3.8.19.26.56.tar", last modified: Fri Mar  8 11:26:58 2024, max compression
+gzip compressed data, was "chatllm-2024.4.3.18.28.17.tar", last modified: Wed Apr  3 10:28:18 2024, max compression
```

## Comparing `chatllm-2024.3.8.19.26.56.tar` & `chatllm-2024.4.3.18.28.17.tar`

### file list

```diff
@@ -1,300 +1,317 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-08 11:26:58.198338 chatllm-2024.3.8.19.26.56/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 chatllm-2024.3.8.19.26.56/.editorconfig
--rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 chatllm-2024.3.8.19.26.56/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-10-16 03:44:58.000000 chatllm-2024.3.8.19.26.56/ITEMS.md
--rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 chatllm-2024.3.8.19.26.56/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)     2466 2023-10-13 02:46:31.000000 chatllm-2024.3.8.19.26.56/LLMS.md
--rw-r--r--   0 betterme   (501) staff       (20)      367 2023-08-28 09:11:46.000000 chatllm-2024.3.8.19.26.56/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 chatllm-2024.3.8.19.26.56/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     8983 2024-03-08 11:26:58.197944 chatllm-2024.3.8.19.26.56/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     6904 2023-11-09 00:43:20.000000 chatllm-2024.3.8.19.26.56/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     5851 2023-05-29 06:46:23.000000 chatllm-2024.3.8.19.26.56/README.md.bak
--rw-r--r--   0 betterme   (501) staff       (20)     1653 2023-07-31 01:36:20.000000 chatllm-2024.3.8.19.26.56/TODO.md
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-08 11:26:58.121097 chatllm-2024.3.8.19.26.56/apps/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2024-01-18 04:12:46.000000 chatllm-2024.3.8.19.26.56/apps/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      563 2024-01-18 04:18:13.000000 chatllm-2024.3.8.19.26.56/apps/allchat.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-08 11:26:58.121953 chatllm-2024.3.8.19.26.56/chatllm/
--rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 chatllm-2024.3.8.19.26.56/chatllm/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-08 11:26:58.123402 chatllm-2024.3.8.19.26.56/chatllm/agent/
--rw-r--r--   0 betterme   (501) staff       (20)      769 2023-10-25 07:22:10.000000 chatllm-2024.3.8.19.26.56/chatllm/agent/MultiPrompt.py
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-10-25 06:26:02.000000 chatllm-2024.3.8.19.26.56/chatllm/agent/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-08 11:26:58.123892 chatllm-2024.3.8.19.26.56/chatllm/aigc/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-05-29 05:16:39.000000 chatllm-2024.3.8.19.26.56/chatllm/aigc/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      834 2023-05-29 05:17:00.000000 chatllm-2024.3.8.19.26.56/chatllm/aigc/common.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-08 11:26:58.126362 chatllm-2024.3.8.19.26.56/chatllm/api/
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-05-29 01:42:28.000000 chatllm-2024.3.8.19.26.56/chatllm/api/TODO.md
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-28 01:04:39.000000 chatllm-2024.3.8.19.26.56/chatllm/api/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      569 2023-07-21 09:14:37.000000 chatllm-2024.3.8.19.26.56/chatllm/api/app.py
--rw-r--r--   0 betterme   (501) staff       (20)     2192 2023-06-26 05:53:59.000000 chatllm-2024.3.8.19.26.56/chatllm/api/config.py
--rw-r--r--   0 betterme   (501) staff       (20)     1010 2023-07-03 09:56:01.000000 chatllm-2024.3.8.19.26.56/chatllm/api/datamodels.py
--rw-r--r--   0 betterme   (501) staff       (20)     1748 2023-07-04 06:45:09.000000 chatllm-2024.3.8.19.26.56/chatllm/api/openai_client.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-08 11:26:58.131564 chatllm-2024.3.8.19.26.56/chatllm/api/routers/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-12-22 04:28:15.000000 chatllm-2024.3.8.19.26.56/chatllm/api/routers/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2125 2024-03-08 11:26:53.000000 chatllm-2024.3.8.19.26.56/chatllm/api/routers/all_chat_completions.py
--rw-r--r--   0 betterme   (501) staff       (20)     4318 2024-02-08 05:44:20.000000 chatllm-2024.3.8.19.26.56/chatllm/api/routers/all_chat_completions_.py
--rw-r--r--   0 betterme   (501) staff       (20)     1020 2023-12-12 04:20:15.000000 chatllm-2024.3.8.19.26.56/chatllm/api/routers/api.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-08 11:26:58.131837 chatllm-2024.3.8.19.26.56/chatllm/api/routers/chat_completions/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2024-02-23 05:17:33.000000 chatllm-2024.3.8.19.26.56/chatllm/api/routers/chat_completions/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     3218 2024-02-22 08:49:06.000000 chatllm-2024.3.8.19.26.56/chatllm/api/routers/chat_completions_extra.py
--rw-r--r--   0 betterme   (501) staff       (20)     2905 2024-03-07 09:38:32.000000 chatllm-2024.3.8.19.26.56/chatllm/api/routers/chat_completions_kimi.py
--rw-r--r--   0 betterme   (501) staff       (20)     3151 2024-02-08 10:20:34.000000 chatllm-2024.3.8.19.26.56/chatllm/api/routers/chat_completions_rag.py
--rw-r--r--   0 betterme   (501) staff       (20)     2286 2024-02-27 02:48:06.000000 chatllm-2024.3.8.19.26.56/chatllm/api/routers/chat_completions_redirect.py
--rw-r--r--   0 betterme   (501) staff       (20)     2322 2024-03-01 07:46:20.000000 chatllm-2024.3.8.19.26.56/chatllm/api/routers/cocopilot.py
--rw-r--r--   0 betterme   (501) staff       (20)      407 2024-01-09 04:17:19.000000 chatllm-2024.3.8.19.26.56/chatllm/api/routers/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     1965 2024-01-11 01:39:06.000000 chatllm-2024.3.8.19.26.56/chatllm/api/routers/embeddings.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-08 11:26:58.132537 chatllm-2024.3.8.19.26.56/chatllm/api/routers/files/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2024-02-23 05:17:02.000000 chatllm-2024.3.8.19.26.56/chatllm/api/routers/files/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     5205 2024-02-06 13:45:01.000000 chatllm-2024.3.8.19.26.56/chatllm/api/routers/files/files_minio.py
--rw-r--r--   0 betterme   (501) staff       (20)     4608 2024-02-08 09:02:43.000000 chatllm-2024.3.8.19.26.56/chatllm/api/routers/files/files_moonshot.py
--rw-r--r--   0 betterme   (501) staff       (20)     5205 2024-02-06 13:45:01.000000 chatllm-2024.3.8.19.26.56/chatllm/api/routers/files_minio.py
--rw-r--r--   0 betterme   (501) staff       (20)     4939 2024-03-04 06:31:29.000000 chatllm-2024.3.8.19.26.56/chatllm/api/routers/files_moonshot.py
--rw-r--r--   0 betterme   (501) staff       (20)     1605 2023-12-20 02:41:07.000000 chatllm-2024.3.8.19.26.56/chatllm/api/routers/local_embeddings.py
--rw-r--r--   0 betterme   (501) staff       (20)      779 2023-08-24 00:45:22.000000 chatllm-2024.3.8.19.26.56/chatllm/api/routers/models.py
--rw-r--r--   0 betterme   (501) staff       (20)     2163 2023-12-22 04:08:42.000000 chatllm-2024.3.8.19.26.56/chatllm/api/routers/smooth_completions.py
--rw-r--r--   0 betterme   (501) staff       (20)     1280 2023-12-26 09:39:01.000000 chatllm-2024.3.8.19.26.56/chatllm/api/routers/speech.py
--rw-r--r--   0 betterme   (501) staff       (20)     4653 2023-11-22 03:55:32.000000 chatllm-2024.3.8.19.26.56/chatllm/api/routers/utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-08 11:26:58.133789 chatllm-2024.3.8.19.26.56/chatllm/api/routes/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-05-25 10:51:34.000000 chatllm-2024.3.8.19.26.56/chatllm/api/routes/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      558 2023-07-24 09:51:52.000000 chatllm-2024.3.8.19.26.56/chatllm/api/routes/api.py
--rw-r--r--   0 betterme   (501) staff       (20)     2200 2023-06-02 01:06:14.000000 chatllm-2024.3.8.19.26.56/chatllm/api/routes/base.py
--rw-r--r--   0 betterme   (501) staff       (20)     5023 2023-07-24 10:21:57.000000 chatllm-2024.3.8.19.26.56/chatllm/api/routes/completions.py
--rw-r--r--   0 betterme   (501) staff       (20)     1904 2023-06-04 06:52:41.000000 chatllm-2024.3.8.19.26.56/chatllm/api/routes/embeddings.py
--rw-r--r--   0 betterme   (501) staff       (20)     3336 2023-08-02 01:55:55.000000 chatllm-2024.3.8.19.26.56/chatllm/api/routes/responses.py
--rw-r--r--   0 betterme   (501) staff       (20)    11497 2023-05-25 09:59:48.000000 chatllm-2024.3.8.19.26.56/chatllm/api/sse_api.py
--rw-r--r--   0 betterme   (501) staff       (20)      845 2023-05-26 07:01:26.000000 chatllm-2024.3.8.19.26.56/chatllm/api/test.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-08 11:26:58.137149 chatllm-2024.3.8.19.26.56/chatllm/applications/
--rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 chatllm-2024.3.8.19.26.56/chatllm/applications/Question2Answer.py
--rw-r--r--   0 betterme   (501) staff       (20)     3937 2023-05-29 07:27:53.000000 chatllm-2024.3.8.19.26.56/chatllm/applications/__chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 chatllm-2024.3.8.19.26.56/chatllm/applications/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2405 2023-06-27 08:56:59.000000 chatllm-2024.3.8.19.26.56/chatllm/applications/chatann.py
--rw-r--r--   0 betterme   (501) staff       (20)      267 2023-05-04 01:43:23.000000 chatllm-2024.3.8.19.26.56/chatllm/applications/chataudio.py
--rw-r--r--   0 betterme   (501) staff       (20)     2420 2023-06-29 01:53:20.000000 chatllm-2024.3.8.19.26.56/chatllm/applications/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)      944 2023-05-29 04:11:25.000000 chatllm-2024.3.8.19.26.56/chatllm/applications/chatcrawler.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 chatllm-2024.3.8.19.26.56/chatllm/applications/chatdoc.py
--rw-r--r--   0 betterme   (501) staff       (20)     1693 2023-06-29 07:30:13.000000 chatllm-2024.3.8.19.26.56/chatllm/applications/chatmind.py
--rw-r--r--   0 betterme   (501) staff       (20)     1350 2023-05-29 07:27:53.000000 chatllm-2024.3.8.19.26.56/chatllm/applications/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)     1875 2023-05-25 06:54:08.000000 chatllm-2024.3.8.19.26.56/chatllm/applications/chatwhoosh.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 chatllm-2024.3.8.19.26.56/chatllm/applications/pipeline.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-08 11:26:58.138324 chatllm-2024.3.8.19.26.56/chatllm/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 chatllm-2024.3.8.19.26.56/chatllm/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      149 2023-09-19 08:35:37.000000 chatllm-2024.3.8.19.26.56/chatllm/clis/TODO.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 chatllm-2024.3.8.19.26.56/chatllm/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1077 2023-08-04 07:09:27.000000 chatllm-2024.3.8.19.26.56/chatllm/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)     1029 2023-11-10 08:40:49.000000 chatllm-2024.3.8.19.26.56/chatllm/closeai.py
--rw-r--r--   0 betterme   (501) staff       (20)      995 2023-12-08 08:11:25.000000 chatllm-2024.3.8.19.26.56/chatllm/llm_test.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-08 11:26:58.138948 chatllm-2024.3.8.19.26.56/chatllm/llmchain/
--rw-r--r--   0 betterme   (501) staff       (20)      376 2023-12-14 00:46:13.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/TODO.md
--rw-r--r--   0 betterme   (501) staff       (20)     2244 2024-02-08 09:53:36.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-08 11:26:58.143876 chatllm-2024.3.8.19.26.56/chatllm/llmchain/applications/
--rw-r--r--   0 betterme   (501) staff       (20)      548 2024-01-04 02:22:28.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/applications/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2636 2024-02-08 02:05:28.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/applications/_chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)     1603 2024-02-07 08:56:45.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/applications/_chatocr.py
--rw-r--r--   0 betterme   (501) staff       (20)     4126 2024-02-07 08:58:52.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/applications/chat4all.py
--rw-r--r--   0 betterme   (501) staff       (20)      267 2023-05-04 01:43:23.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/applications/chataudio.py
--rw-r--r--   0 betterme   (501) staff       (20)     2365 2024-02-07 08:56:45.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/applications/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)      394 2023-11-01 04:09:02.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/applications/chatbook.py
--rw-r--r--   0 betterme   (501) staff       (20)     5509 2024-02-07 08:58:52.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/applications/chatfile.py
--rw-r--r--   0 betterme   (501) staff       (20)     5925 2024-02-07 08:56:45.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/applications/chatfiles.py
--rw-r--r--   0 betterme   (501) staff       (20)     1923 2023-09-25 06:22:11.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/applications/chatocr.py
--rw-r--r--   0 betterme   (501) staff       (20)     1026 2024-02-07 08:56:45.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/applications/chatpicture.py
--rw-r--r--   0 betterme   (501) staff       (20)     5362 2024-02-07 08:58:52.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/applications/chatqa.py
--rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/applications/chatsearch.py
--rw-r--r--   0 betterme   (501) staff       (20)     3974 2024-01-19 03:11:49.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/applications/chaturl.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/applications/chatweb.py
--rw-r--r--   0 betterme   (501) staff       (20)      273 2023-10-16 04:07:00.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/applications/chatwx.py
--rw-r--r--   0 betterme   (501) staff       (20)     2728 2024-02-07 08:56:45.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/applications/summarizer.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-08 11:26:58.144389 chatllm-2024.3.8.19.26.56/chatllm/llmchain/audio/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-12-26 05:06:11.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/audio/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1660 2023-12-26 06:25:37.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/audio/speech.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-08 11:26:58.144867 chatllm-2024.3.8.19.26.56/chatllm/llmchain/callbacks/
--rw-r--r--   0 betterme   (501) staff       (20)      353 2023-07-31 03:48:34.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/callbacks/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1554 2023-08-11 07:26:25.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/callbacks/streaming.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-08 11:26:58.145338 chatllm-2024.3.8.19.26.56/chatllm/llmchain/chat_models/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-07-12 09:45:45.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/chat_models/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1933 2024-02-08 02:04:31.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/chat_models/openai.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-08 11:26:58.150742 chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/
--rw-r--r--   0 betterme   (501) staff       (20)      509 2023-10-09 06:21:53.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     3893 2023-09-11 02:31:54.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/_erniebot.py
--rw-r--r--   0 betterme   (501) staff       (20)     4777 2023-10-09 05:56:00.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/_hunyuan.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2024-01-19 03:12:52.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/base.py
--rw-r--r--   0 betterme   (501) staff       (20)     3660 2024-01-24 07:46:48.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/chat_image.py
--rw-r--r--   0 betterme   (501) staff       (20)     3585 2024-01-24 07:32:54.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/chat_tts.py
--rw-r--r--   0 betterme   (501) staff       (20)     2860 2023-09-26 10:14:03.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/chatglm.py
--rw-r--r--   0 betterme   (501) staff       (20)     6741 2024-01-05 08:26:54.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/deepseek.py
--rw-r--r--   0 betterme   (501) staff       (20)     2521 2023-09-11 03:38:46.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/dify.py
--rw-r--r--   0 betterme   (501) staff       (20)     4875 2023-09-07 02:40:43.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/ernie.py
--rw-r--r--   0 betterme   (501) staff       (20)     9740 2024-03-01 07:54:53.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/github_copilot.py
--rw-r--r--   0 betterme   (501) staff       (20)    11369 2024-02-19 05:45:13.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/github_copilot_.py
--rw-r--r--   0 betterme   (501) staff       (20)     5515 2023-12-20 01:55:07.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/google_enerativeai.py
--rw-r--r--   0 betterme   (501) staff       (20)     2440 2023-12-14 05:38:47.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/google_enerativeai_.py
--rw-r--r--   0 betterme   (501) staff       (20)     2024 2024-02-20 08:41:59.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/groq.py
--rw-r--r--   0 betterme   (501) staff       (20)     5146 2023-11-29 11:08:32.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/hunyuan.py
--rw-r--r--   0 betterme   (501) staff       (20)    13562 2024-03-08 02:26:19.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/kimi.py
--rw-r--r--   0 betterme   (501) staff       (20)    11454 2024-02-29 11:53:22.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/moonshot_kimi.py
--rw-r--r--   0 betterme   (501) staff       (20)    12088 2024-03-05 09:57:31.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/openai_completions.py
--rw-r--r--   0 betterme   (501) staff       (20)    12583 2024-02-28 08:56:13.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/openai_completions_bk.py
--rw-r--r--   0 betterme   (501) staff       (20)     4275 2024-01-09 08:28:12.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/smooth.py
--rw-r--r--   0 betterme   (501) staff       (20)     7397 2023-09-14 07:59:51.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/spark.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-08 11:26:58.151366 chatllm-2024.3.8.19.26.56/chatllm/llmchain/decorators/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-07-31 03:48:34.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/decorators/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1982 2024-02-08 02:05:28.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/decorators/common.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-08 11:26:58.152970 chatllm-2024.3.8.19.26.56/chatllm/llmchain/document_loaders/
--rw-r--r--   0 betterme   (501) staff       (20)     2448 2024-02-07 06:21:54.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/document_loaders/FilesLoader.py
--rw-r--r--   0 betterme   (501) staff       (20)      660 2023-09-21 01:17:36.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/document_loaders/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1713 2024-02-07 06:21:40.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/document_loaders/docx.py
--rw-r--r--   0 betterme   (501) staff       (20)     4824 2024-02-07 05:46:29.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/document_loaders/file.py
--rw-r--r--   0 betterme   (501) staff       (20)     2220 2024-02-07 06:21:54.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/document_loaders/image.py
--rw-r--r--   0 betterme   (501) staff       (20)     1842 2024-02-07 06:21:54.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/document_loaders/pdf.py
--rw-r--r--   0 betterme   (501) staff       (20)     1787 2024-02-07 05:46:15.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/document_loaders/text.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-08 11:26:58.154752 chatllm-2024.3.8.19.26.56/chatllm/llmchain/embeddings/
--rw-r--r--   0 betterme   (501) staff       (20)      935 2024-02-07 08:58:55.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/embeddings/ApiEmbeddings.py
--rw-r--r--   0 betterme   (501) staff       (20)     3534 2024-02-07 08:57:18.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/embeddings/DashScopeEmbeddings.py
--rw-r--r--   0 betterme   (501) staff       (20)     1332 2024-02-07 08:57:18.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/embeddings/HuggingFaceEmbeddings.py
--rw-r--r--   0 betterme   (501) staff       (20)     2327 2024-02-07 08:57:18.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/embeddings/OpenAIEmbeddings.py
--rw-r--r--   0 betterme   (501) staff       (20)     2722 2023-12-20 01:40:26.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/embeddings/XunfeiEmbedding.py
--rw-r--r--   0 betterme   (501) staff       (20)      507 2023-08-10 08:01:04.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/embeddings/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     6980 2024-02-07 01:33:16.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/embeddings/openai_embeddings.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-08 11:26:58.157198 chatllm-2024.3.8.19.26.56/chatllm/llmchain/llms/
--rw-r--r--   0 betterme   (501) staff       (20)      546 2023-12-05 07:56:51.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/llms/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1667 2024-02-07 08:56:45.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/llms/basellm.py
--rw-r--r--   0 betterme   (501) staff       (20)     3362 2024-02-07 08:56:45.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/llms/chatglm.py
--rw-r--r--   0 betterme   (501) staff       (20)     3901 2024-02-07 08:56:45.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/llms/ernie.py
--rw-r--r--   0 betterme   (501) staff       (20)     3395 2024-02-07 08:56:45.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/llms/hunyuan.py
--rw-r--r--   0 betterme   (501) staff       (20)     2437 2023-12-05 07:50:17.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/llms/kimi.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-07-24 05:47:03.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/llms/minimax.py
--rw-r--r--   0 betterme   (501) staff       (20)     2286 2024-02-08 01:57:34.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/llms/spark.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-08 11:26:58.159527 chatllm-2024.3.8.19.26.56/chatllm/llmchain/prompts/
--rw-r--r--   0 betterme   (501) staff       (20)      243 2023-11-09 05:49:28.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/prompts/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      639 2023-09-25 09:52:28.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/prompts/kb.py
--rw-r--r--   0 betterme   (501) staff       (20)     2963 2023-09-20 01:09:40.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/prompts/ocr.py
--rw-r--r--   0 betterme   (501) staff       (20)     4625 2024-02-07 08:56:45.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/prompts/prompt_templates.py
--rw-r--r--   0 betterme   (501) staff       (20)      722 2023-07-13 02:06:43.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/prompts/prompt_watch.py
--rw-r--r--   0 betterme   (501) staff       (20)     2488 2024-02-07 08:56:45.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/prompts/rag.py
--rw-r--r--   0 betterme   (501) staff       (20)     1973 2024-02-07 08:56:45.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/prompts/格式化.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-08 11:26:58.160888 chatllm-2024.3.8.19.26.56/chatllm/llmchain/textsplitter/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-08-16 06:10:25.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/textsplitter/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1389 2023-05-15 07:48:48.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/textsplitter/ali_text_splitter.py
--rw-r--r--   0 betterme   (501) staff       (20)     3356 2023-07-15 06:05:38.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/textsplitter/chinese_text_splitter.py
--rw-r--r--   0 betterme   (501) staff       (20)     3179 2023-06-30 13:02:46.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/textsplitter/zh_title_enhance.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-08 11:26:58.161312 chatllm-2024.3.8.19.26.56/chatllm/llmchain/utils/
--rw-r--r--   0 betterme   (501) staff       (20)      280 2023-07-31 03:48:34.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2653 2024-02-08 02:05:02.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/utils/common.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-08 11:26:58.163387 chatllm-2024.3.8.19.26.56/chatllm/llmchain/vectorstores/
--rw-r--r--   0 betterme   (501) staff       (20)      910 2024-02-07 08:59:38.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/vectorstores/DocArrayInMemorySearch.py
--rw-r--r--   0 betterme   (501) staff       (20)     3891 2024-02-23 03:20:33.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/vectorstores/ElasticsearchStore.py
--rw-r--r--   0 betterme   (501) staff       (20)     4126 2024-02-07 08:59:38.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/vectorstores/FAISS.py
--rw-r--r--   0 betterme   (501) staff       (20)     1334 2024-02-07 08:59:38.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/vectorstores/Milvus.py
--rw-r--r--   0 betterme   (501) staff       (20)     4515 2024-02-07 08:59:38.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/vectorstores/Usearch.py
--rw-r--r--   0 betterme   (501) staff       (20)     4593 2024-02-07 08:59:38.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/vectorstores/VectorRecordManager.py
--rw-r--r--   0 betterme   (501) staff       (20)      661 2023-09-19 01:20:05.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/vectorstores/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1567 2023-07-14 01:13:07.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/vectorstores/base.py
--rw-r--r--   0 betterme   (501) staff       (20)     1332 2024-02-07 08:59:38.000000 chatllm-2024.3.8.19.26.56/chatllm/llmchain/vectorstores/index_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-08 11:26:58.164729 chatllm-2024.3.8.19.26.56/chatllm/llms/
--rw-r--r--   0 betterme   (501) staff       (20)     1526 2023-06-02 12:11:10.000000 chatllm-2024.3.8.19.26.56/chatllm/llms/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2307 2023-06-30 12:28:42.000000 chatllm-2024.3.8.19.26.56/chatllm/llms/chatglm.py
--rw-r--r--   0 betterme   (501) staff       (20)     1143 2023-07-03 09:18:07.000000 chatllm-2024.3.8.19.26.56/chatllm/llms/chatgpt.py
--rw-r--r--   0 betterme   (501) staff       (20)     1559 2023-05-22 08:19:27.000000 chatllm-2024.3.8.19.26.56/chatllm/llms/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     2083 2023-05-22 08:39:00.000000 chatllm-2024.3.8.19.26.56/chatllm/llms/llama.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-08 11:26:58.165195 chatllm-2024.3.8.19.26.56/chatllm/prompts/
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-06-12 03:51:17.000000 chatllm-2024.3.8.19.26.56/chatllm/prompts/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1556 2023-11-20 08:02:57.000000 chatllm-2024.3.8.19.26.56/chatllm/prompts/common.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-08 11:26:58.167171 chatllm-2024.3.8.19.26.56/chatllm/schemas/
--rw-r--r--   0 betterme   (501) staff       (20)     1790 2023-12-11 10:49:08.000000 chatllm-2024.3.8.19.26.56/chatllm/schemas/4v.py
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-07-31 02:38:12.000000 chatllm-2024.3.8.19.26.56/chatllm/schemas/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      867 2024-01-11 01:35:59.000000 chatllm-2024.3.8.19.26.56/chatllm/schemas/embedding.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-08 11:26:58.167739 chatllm-2024.3.8.19.26.56/chatllm/schemas/json_schema_extra/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2024-01-19 07:34:54.000000 chatllm-2024.3.8.19.26.56/chatllm/schemas/json_schema_extra/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-08 11:26:58.168704 chatllm-2024.3.8.19.26.56/chatllm/schemas/kimi/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-11-29 08:43:08.000000 chatllm-2024.3.8.19.26.56/chatllm/schemas/kimi/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2689 2023-12-28 01:16:22.000000 chatllm-2024.3.8.19.26.56/chatllm/schemas/kimi/protocol.py
--rw-r--r--   0 betterme   (501) staff       (20)     3193 2024-02-29 08:15:07.000000 chatllm-2024.3.8.19.26.56/chatllm/schemas/kimi/state.json
--rw-r--r--   0 betterme   (501) staff       (20)     2284 2024-02-29 09:51:31.000000 chatllm-2024.3.8.19.26.56/chatllm/schemas/kimi_types.py
--rw-r--r--   0 betterme   (501) staff       (20)      340 2023-11-03 10:59:44.000000 chatllm-2024.3.8.19.26.56/chatllm/schemas/metadata.py
--rw-r--r--   0 betterme   (501) staff       (20)    10382 2024-03-01 03:08:51.000000 chatllm-2024.3.8.19.26.56/chatllm/schemas/openai_api_protocol.py
--rw-r--r--   0 betterme   (501) staff       (20)     3667 2024-03-07 08:58:04.000000 chatllm-2024.3.8.19.26.56/chatllm/schemas/openai_types.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-08 11:26:58.170560 chatllm-2024.3.8.19.26.56/chatllm/serve/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-07-31 02:40:14.000000 chatllm-2024.3.8.19.26.56/chatllm/serve/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    29234 2023-07-31 02:44:27.000000 chatllm-2024.3.8.19.26.56/chatllm/serve/_openai_api_server.py
--rw-r--r--   0 betterme   (501) staff       (20)     1178 2024-02-07 08:56:45.000000 chatllm-2024.3.8.19.26.56/chatllm/serve/app.py
--rw-r--r--   0 betterme   (501) staff       (20)     1870 2023-07-19 10:34:49.000000 chatllm-2024.3.8.19.26.56/chatllm/serve/constants.py
--rw-r--r--   0 betterme   (501) staff       (20)    25416 2023-08-24 00:45:22.000000 chatllm-2024.3.8.19.26.56/chatllm/serve/openai_api_server.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-08 11:26:58.172864 chatllm-2024.3.8.19.26.56/chatllm/utils/
--rw-r--r--   0 betterme   (501) staff       (20)      278 2023-04-28 04:20:30.000000 chatllm-2024.3.8.19.26.56/chatllm/utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 04:37:16.000000 chatllm-2024.3.8.19.26.56/chatllm/utils/_textsplitter.py
--rw-r--r--   0 betterme   (501) staff       (20)     2270 2024-02-06 13:51:45.000000 chatllm-2024.3.8.19.26.56/chatllm/utils/common.py
--rw-r--r--   0 betterme   (501) staff       (20)     2430 2023-05-19 09:28:43.000000 chatllm-2024.3.8.19.26.56/chatllm/utils/gpu_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     6342 2023-05-30 08:31:55.000000 chatllm-2024.3.8.19.26.56/chatllm/utils/nbce.py
--rw-r--r--   0 betterme   (501) staff       (20)     5208 2023-05-30 08:22:36.000000 chatllm-2024.3.8.19.26.56/chatllm/utils/nbce_test.py
--rw-r--r--   0 betterme   (501) staff       (20)     3144 2024-03-07 09:17:15.000000 chatllm-2024.3.8.19.26.56/chatllm/utils/openai_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-08 11:26:58.189004 chatllm-2024.3.8.19.26.56/chatllm/webui/
--rw-r--r--   0 betterme   (501) staff       (20)     7568 2023-11-09 06:40:18.000000 chatllm-2024.3.8.19.26.56/chatllm/webui/!.png
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 chatllm-2024.3.8.19.26.56/chatllm/webui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)   225373 2023-09-28 00:58:21.000000 chatllm-2024.3.8.19.26.56/chatllm/webui/bot.png
--rw-r--r--   0 betterme   (501) staff       (20)     2747 2023-08-11 06:45:35.000000 chatllm-2024.3.8.19.26.56/chatllm/webui/chat.py
--rw-r--r--   0 betterme   (501) staff       (20)     1826 2023-12-14 02:59:58.000000 chatllm-2024.3.8.19.26.56/chatllm/webui/chat_copilot.py
--rw-r--r--   0 betterme   (501) staff       (20)     1457 2023-05-29 07:27:53.000000 chatllm-2024.3.8.19.26.56/chatllm/webui/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)   123851 2023-10-26 08:17:41.000000 chatllm-2024.3.8.19.26.56/chatllm/webui/chatbook.png
--rw-r--r--   0 betterme   (501) staff       (20)     5660 2024-02-07 08:56:45.000000 chatllm-2024.3.8.19.26.56/chatllm/webui/chatbook.py
--rw-r--r--   0 betterme   (501) staff       (20)    14406 2023-09-05 09:04:59.000000 chatllm-2024.3.8.19.26.56/chatllm/webui/chatbot.png
--rw-r--r--   0 betterme   (501) staff       (20)     3389 2023-09-25 01:29:31.000000 chatllm-2024.3.8.19.26.56/chatllm/webui/chatbot.py
--rw-r--r--   0 betterme   (501) staff       (20)     4044 2023-08-28 06:36:36.000000 chatllm-2024.3.8.19.26.56/chatllm/webui/chatfile.py
--rw-r--r--   0 betterme   (501) staff       (20)     5642 2024-02-07 08:56:45.000000 chatllm-2024.3.8.19.26.56/chatllm/webui/chatfile_nesc.py
--rw-r--r--   0 betterme   (501) staff       (20)     2412 2024-01-12 05:56:43.000000 chatllm-2024.3.8.19.26.56/chatllm/webui/chatfile_nesc_last.py
--rw-r--r--   0 betterme   (501) staff       (20)     5741 2024-02-07 08:56:45.000000 chatllm-2024.3.8.19.26.56/chatllm/webui/chatfile_nesc_v1.py
--rw-r--r--   0 betterme   (501) staff       (20)     3103 2024-01-12 05:56:43.000000 chatllm-2024.3.8.19.26.56/chatllm/webui/chatfile_nesc_v2.py
--rw-r--r--   0 betterme   (501) staff       (20)     2781 2024-02-01 14:00:42.000000 chatllm-2024.3.8.19.26.56/chatllm/webui/chatfile_v0.1.py
--rw-r--r--   0 betterme   (501) staff       (20)     1076 2023-06-29 07:59:43.000000 chatllm-2024.3.8.19.26.56/chatllm/webui/chatmind.py
--rw-r--r--   0 betterme   (501) staff       (20)     3103 2023-08-23 04:01:26.000000 chatllm-2024.3.8.19.26.56/chatllm/webui/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)      134 2023-06-26 02:13:58.000000 chatllm-2024.3.8.19.26.56/chatllm/webui/conf.yaml
--rw-r--r--   0 betterme   (501) staff       (20)     1093 2023-11-06 09:12:04.000000 chatllm-2024.3.8.19.26.56/chatllm/webui/dalle.py
--rw-r--r--   0 betterme   (501) staff       (20)      554 2023-11-15 06:57:01.000000 chatllm-2024.3.8.19.26.56/chatllm/webui/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     4235 2024-01-25 05:24:50.000000 chatllm-2024.3.8.19.26.56/chatllm/webui/fire.png
--rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 chatllm-2024.3.8.19.26.56/chatllm/webui/gradio_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)   856440 2023-09-25 01:29:08.000000 chatllm-2024.3.8.19.26.56/chatllm/webui/logo.png
--rw-r--r--   0 betterme   (501) staff       (20)   102641 2023-08-11 06:34:47.000000 chatllm-2024.3.8.19.26.56/chatllm/webui/nesc.jpeg
--rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 chatllm-2024.3.8.19.26.56/chatllm/webui/nice_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)      557 2024-02-07 08:56:45.000000 chatllm-2024.3.8.19.26.56/chatllm/webui/prompt_maker.py
--rw-r--r--   0 betterme   (501) staff       (20)     4445 2024-02-07 08:59:38.000000 chatllm-2024.3.8.19.26.56/chatllm/webui/qa.py
--rw-r--r--   0 betterme   (501) staff       (20)      426 2024-02-01 13:14:06.000000 chatllm-2024.3.8.19.26.56/chatllm/webui/run.sh
--rw-r--r--   0 betterme   (501) staff       (20)     4312 2023-08-08 10:37:46.000000 chatllm-2024.3.8.19.26.56/chatllm/webui/user.jpg
--rw-r--r--   0 betterme   (501) staff       (20)     3506 2023-05-26 07:39:23.000000 chatllm-2024.3.8.19.26.56/chatllm/webui/visualglm_st.py
--rw-r--r--   0 betterme   (501) staff       (20)   437368 2024-01-12 05:38:09.000000 chatllm-2024.3.8.19.26.56/chatllm/webui/副本人工智能咨询服务协议 汉洁 南京当月糯 20240105(1)(1).docx
--rw-r--r--   0 betterme   (501) staff       (20)    10521 2024-02-01 13:14:34.000000 chatllm-2024.3.8.19.26.56/chatllm/webui/同程报价.xlsx
--rw-r--r--   0 betterme   (501) staff       (20)   303359 2023-09-20 06:32:26.000000 chatllm-2024.3.8.19.26.56/chatllm/webui/规丞相.png
--rw-r--r--   0 betterme   (501) staff       (20)   414314 2024-02-01 13:16:20.000000 chatllm-2024.3.8.19.26.56/chatllm/webui/酒店百问百答.pdf
--rw-r--r--   0 betterme   (501) staff       (20)   741995 2024-01-12 05:38:20.000000 chatllm-2024.3.8.19.26.56/chatllm/webui/附件1：东北证券股份有限公司员工合规手册（2023年12月）.doc
--rw-r--r--   0 betterme   (501) staff       (20)   416458 2023-12-27 07:56:52.000000 chatllm-2024.3.8.19.26.56/chatllm/webui/附件1：东北证券股份有限公司员工合规手册（2023年12月）.docx
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-08 11:26:58.196088 chatllm-2024.3.8.19.26.56/chatllm.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     8983 2024-03-08 11:26:57.000000 chatllm-2024.3.8.19.26.56/chatllm.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     8519 2024-03-08 11:26:58.000000 chatllm-2024.3.8.19.26.56/chatllm.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2024-03-08 11:26:57.000000 chatllm-2024.3.8.19.26.56/chatllm.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       53 2024-03-08 11:26:57.000000 chatllm-2024.3.8.19.26.56/chatllm.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2024-03-08 11:26:57.000000 chatllm-2024.3.8.19.26.56/chatllm.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)      425 2024-03-08 11:26:57.000000 chatllm-2024.3.8.19.26.56/chatllm.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2024-03-08 11:26:57.000000 chatllm-2024.3.8.19.26.56/chatllm.egg-info/top_level.txt
--rw-r--r--   0 betterme   (501) staff       (20)      684 2023-03-20 02:44:39.000000 chatllm-2024.3.8.19.26.56/clear_git_history.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-08 11:26:58.194524 chatllm-2024.3.8.19.26.56/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 chatllm-2024.3.8.19.26.56/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 chatllm-2024.3.8.19.26.56/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 chatllm-2024.3.8.19.26.56/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 chatllm-2024.3.8.19.26.56/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 chatllm-2024.3.8.19.26.56/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 chatllm-2024.3.8.19.26.56/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 chatllm-2024.3.8.19.26.56/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 chatllm-2024.3.8.19.26.56/docs/readme.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)      350 2023-10-16 06:38:24.000000 chatllm-2024.3.8.19.26.56/git_init.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 chatllm-2024.3.8.19.26.56/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)      137 2023-09-14 06:48:16.000000 chatllm-2024.3.8.19.26.56/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)       14 2023-05-19 09:53:16.000000 chatllm-2024.3.8.19.26.56/requirements_ann.txt
--rw-r--r--   0 betterme   (501) staff       (20)       30 2023-05-31 02:41:18.000000 chatllm-2024.3.8.19.26.56/requirements_api.txt
--rw-r--r--   0 betterme   (501) staff       (20)       29 2023-05-26 08:03:09.000000 chatllm-2024.3.8.19.26.56/requirements_openai.txt
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-05-29 04:24:55.000000 chatllm-2024.3.8.19.26.56/requirements_pdf.txt
--rw-r--r--   0 betterme   (501) staff       (20)       22 2024-01-09 05:49:39.000000 chatllm-2024.3.8.19.26.56/requirements_rag.txt
--rw-r--r--   0 betterme   (501) staff       (20)       25 2023-05-29 04:24:55.000000 chatllm-2024.3.8.19.26.56/requirements_streamlit.txt
--rw-r--r--   0 betterme   (501) staff       (20)       38 2024-03-08 11:26:58.198400 chatllm-2024.3.8.19.26.56/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1706 2023-07-19 10:53:05.000000 chatllm-2024.3.8.19.26.56/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-08 11:26:58.195397 chatllm-2024.3.8.19.26.56/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 chatllm-2024.3.8.19.26.56/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1224 2023-12-11 01:53:35.000000 chatllm-2024.3.8.19.26.56/tests/oneapi_test.py
--rw-r--r--   0 betterme   (501) staff       (20)      224 2023-10-25 08:02:40.000000 chatllm-2024.3.8.19.26.56/tests/test_llm4gpt.py
--rw-r--r--   0 betterme   (501) staff       (20)    51173 2023-04-21 11:31:44.000000 chatllm-2024.3.8.19.26.56/tests/内存型.ipynb
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.843667 chatllm-2024.4.3.18.28.17/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 chatllm-2024.4.3.18.28.17/.editorconfig
+-rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 chatllm-2024.4.3.18.28.17/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-10-16 03:44:58.000000 chatllm-2024.4.3.18.28.17/ITEMS.md
+-rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 chatllm-2024.4.3.18.28.17/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)     2466 2023-10-13 02:46:31.000000 chatllm-2024.4.3.18.28.17/LLMS.md
+-rw-r--r--   0 betterme   (501) staff       (20)      367 2023-08-28 09:11:46.000000 chatllm-2024.4.3.18.28.17/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 chatllm-2024.4.3.18.28.17/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     8983 2024-04-03 10:28:18.843305 chatllm-2024.4.3.18.28.17/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     6904 2023-11-09 00:43:20.000000 chatllm-2024.4.3.18.28.17/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     5851 2023-05-29 06:46:23.000000 chatllm-2024.4.3.18.28.17/README.md.bak
+-rw-r--r--   0 betterme   (501) staff       (20)     1653 2023-07-31 01:36:20.000000 chatllm-2024.4.3.18.28.17/TODO.md
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.758033 chatllm-2024.4.3.18.28.17/apps/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2024-01-18 04:12:46.000000 chatllm-2024.4.3.18.28.17/apps/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      563 2024-01-18 04:18:13.000000 chatllm-2024.4.3.18.28.17/apps/allchat.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.758819 chatllm-2024.4.3.18.28.17/chatllm/
+-rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 chatllm-2024.4.3.18.28.17/chatllm/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.760486 chatllm-2024.4.3.18.28.17/chatllm/agent/
+-rw-r--r--   0 betterme   (501) staff       (20)      769 2023-10-25 07:22:10.000000 chatllm-2024.4.3.18.28.17/chatllm/agent/MultiPrompt.py
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-10-25 06:26:02.000000 chatllm-2024.4.3.18.28.17/chatllm/agent/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.761171 chatllm-2024.4.3.18.28.17/chatllm/aigc/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-05-29 05:16:39.000000 chatllm-2024.4.3.18.28.17/chatllm/aigc/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      834 2023-05-29 05:17:00.000000 chatllm-2024.4.3.18.28.17/chatllm/aigc/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.763621 chatllm-2024.4.3.18.28.17/chatllm/api/
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-05-29 01:42:28.000000 chatllm-2024.4.3.18.28.17/chatllm/api/TODO.md
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-28 01:04:39.000000 chatllm-2024.4.3.18.28.17/chatllm/api/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      569 2023-07-21 09:14:37.000000 chatllm-2024.4.3.18.28.17/chatllm/api/app.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2192 2023-06-26 05:53:59.000000 chatllm-2024.4.3.18.28.17/chatllm/api/config.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1010 2023-07-03 09:56:01.000000 chatllm-2024.4.3.18.28.17/chatllm/api/datamodels.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1748 2023-07-04 06:45:09.000000 chatllm-2024.4.3.18.28.17/chatllm/api/openai_client.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.771394 chatllm-2024.4.3.18.28.17/chatllm/api/routers/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-12-22 04:28:15.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2125 2024-03-08 11:26:53.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/all_chat_completions.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4363 2024-03-15 10:26:22.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/all_chat_completions_.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1020 2023-12-12 04:20:15.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/api.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1591 2024-03-27 05:39:55.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/audio_speech.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.771668 chatllm-2024.4.3.18.28.17/chatllm/api/routers/chat_completions/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2024-03-13 06:12:38.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/chat_completions/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2134 2024-03-22 05:53:28.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/chat_completions_copilot.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3062 2024-03-18 12:03:44.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/chat_completions_extra.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2149 2024-03-12 11:53:24.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/chat_completions_glm.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1961 2024-03-13 07:08:37.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/chat_completions_gptall.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2905 2024-03-07 09:38:32.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/chat_completions_kimi.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3151 2024-02-08 10:20:34.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/chat_completions_rag.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2286 2024-02-27 02:48:06.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/chat_completions_redirect.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2133 2024-03-25 04:10:14.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/chat_completions_smooth.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2011 2024-04-03 10:28:14.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/chat_completions_suno.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2273 2024-03-11 09:18:17.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/cocopilot.py
+-rw-r--r--   0 betterme   (501) staff       (20)      407 2024-01-09 04:17:19.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1997 2024-03-15 02:15:46.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/embeddings.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6180 2024-03-26 03:21:15.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/files.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4939 2024-03-04 06:31:29.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/files_moonshot.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4596 2024-03-13 06:15:25.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/files_moonshot_api.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1605 2023-12-20 02:41:07.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/local_embeddings.py
+-rw-r--r--   0 betterme   (501) staff       (20)      779 2023-08-24 00:45:22.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/models.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2163 2023-12-22 04:08:42.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/smooth_completions.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4653 2023-11-22 03:55:32.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.773363 chatllm-2024.4.3.18.28.17/chatllm/api/routes/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-05-25 10:51:34.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routes/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      558 2023-07-24 09:51:52.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routes/api.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2200 2023-06-02 01:06:14.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routes/base.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5023 2023-07-24 10:21:57.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routes/completions.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1904 2023-06-04 06:52:41.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routes/embeddings.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3336 2023-08-02 01:55:55.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routes/responses.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11497 2023-05-25 09:59:48.000000 chatllm-2024.4.3.18.28.17/chatllm/api/sse_api.py
+-rw-r--r--   0 betterme   (501) staff       (20)      845 2023-05-26 07:01:26.000000 chatllm-2024.4.3.18.28.17/chatllm/api/test.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.776984 chatllm-2024.4.3.18.28.17/chatllm/applications/
+-rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 chatllm-2024.4.3.18.28.17/chatllm/applications/Question2Answer.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3937 2023-05-29 07:27:53.000000 chatllm-2024.4.3.18.28.17/chatllm/applications/__chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 chatllm-2024.4.3.18.28.17/chatllm/applications/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2405 2023-06-27 08:56:59.000000 chatllm-2024.4.3.18.28.17/chatllm/applications/chatann.py
+-rw-r--r--   0 betterme   (501) staff       (20)      267 2023-05-04 01:43:23.000000 chatllm-2024.4.3.18.28.17/chatllm/applications/chataudio.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2420 2023-06-29 01:53:20.000000 chatllm-2024.4.3.18.28.17/chatllm/applications/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)      944 2023-05-29 04:11:25.000000 chatllm-2024.4.3.18.28.17/chatllm/applications/chatcrawler.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 chatllm-2024.4.3.18.28.17/chatllm/applications/chatdoc.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1693 2023-06-29 07:30:13.000000 chatllm-2024.4.3.18.28.17/chatllm/applications/chatmind.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1350 2023-05-29 07:27:53.000000 chatllm-2024.4.3.18.28.17/chatllm/applications/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1875 2023-05-25 06:54:08.000000 chatllm-2024.4.3.18.28.17/chatllm/applications/chatwhoosh.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 chatllm-2024.4.3.18.28.17/chatllm/applications/pipeline.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.778111 chatllm-2024.4.3.18.28.17/chatllm/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 chatllm-2024.4.3.18.28.17/chatllm/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      149 2023-09-19 08:35:37.000000 chatllm-2024.4.3.18.28.17/chatllm/clis/TODO.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 chatllm-2024.4.3.18.28.17/chatllm/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1077 2023-08-04 07:09:27.000000 chatllm-2024.4.3.18.28.17/chatllm/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1029 2023-11-10 08:40:49.000000 chatllm-2024.4.3.18.28.17/chatllm/closeai.py
+-rw-r--r--   0 betterme   (501) staff       (20)      995 2023-12-08 08:11:25.000000 chatllm-2024.4.3.18.28.17/chatllm/llm_test.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.778915 chatllm-2024.4.3.18.28.17/chatllm/llmchain/
+-rw-r--r--   0 betterme   (501) staff       (20)      376 2023-12-14 00:46:13.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/TODO.md
+-rw-r--r--   0 betterme   (501) staff       (20)     2244 2024-02-08 09:53:36.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.783756 chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/
+-rw-r--r--   0 betterme   (501) staff       (20)      548 2024-01-04 02:22:28.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2636 2024-02-08 02:05:28.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/_chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1603 2024-02-07 08:56:45.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/_chatocr.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4126 2024-02-07 08:58:52.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chat4all.py
+-rw-r--r--   0 betterme   (501) staff       (20)      267 2023-05-04 01:43:23.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chataudio.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2365 2024-02-07 08:56:45.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)      394 2023-11-01 04:09:02.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chatbook.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5509 2024-02-07 08:58:52.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chatfile.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5930 2024-03-18 12:05:06.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chatfiles.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1923 2023-09-25 06:22:11.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chatocr.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1026 2024-02-07 08:56:45.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chatpicture.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5362 2024-02-07 08:58:52.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chatqa.py
+-rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chatsearch.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3974 2024-01-19 03:11:49.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chaturl.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chatweb.py
+-rw-r--r--   0 betterme   (501) staff       (20)      273 2023-10-16 04:07:00.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chatwx.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2728 2024-02-07 08:56:45.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/summarizer.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.784308 chatllm-2024.4.3.18.28.17/chatllm/llmchain/audio/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-12-26 05:06:11.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/audio/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1660 2023-12-26 06:25:37.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/audio/speech.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.784764 chatllm-2024.4.3.18.28.17/chatllm/llmchain/callbacks/
+-rw-r--r--   0 betterme   (501) staff       (20)      353 2023-07-31 03:48:34.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/callbacks/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1554 2023-08-11 07:26:25.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/callbacks/streaming.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.785229 chatllm-2024.4.3.18.28.17/chatllm/llmchain/chat_models/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-07-12 09:45:45.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/chat_models/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1933 2024-02-08 02:04:31.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/chat_models/openai.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.795262 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/
+-rw-r--r--   0 betterme   (501) staff       (20)      509 2023-10-09 06:21:53.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3893 2023-09-11 02:31:54.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/_erniebot.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4777 2023-10-09 05:56:00.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/_hunyuan.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2024-01-19 03:12:52.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/base.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3660 2024-01-24 07:46:48.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/chat_image.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3585 2024-01-24 07:32:54.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/chat_tts.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2860 2023-09-26 10:14:03.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/chatglm.py
+-rw-r--r--   0 betterme   (501) staff       (20)    13871 2024-04-03 10:03:04.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/chatglm_web.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9862 2024-03-27 05:39:55.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/copilot.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6741 2024-01-05 08:26:54.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/deepseek.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3502 2024-04-03 08:20:19.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2521 2023-09-11 03:38:46.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/dify.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4875 2023-09-07 02:40:43.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/ernie.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9701 2024-03-15 05:39:17.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/github_copilot.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11369 2024-02-19 05:45:13.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/github_copilot_.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5515 2023-12-20 01:55:07.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/google_enerativeai.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2440 2023-12-14 05:38:47.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/google_enerativeai_.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6009 2024-03-18 07:59:15.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/gptall.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2024 2024-02-20 08:41:59.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/groq.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5146 2023-11-29 11:08:32.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/hunyuan.py
+-rw-r--r--   0 betterme   (501) staff       (20)    16320 2024-03-21 10:49:51.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/kimi.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11454 2024-02-29 11:53:22.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/moonshot_kimi.py
+-rw-r--r--   0 betterme   (501) staff       (20)    12421 2024-03-22 06:06:21.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/openai_completions.py
+-rw-r--r--   0 betterme   (501) staff       (20)    12583 2024-02-28 08:56:13.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/openai_completions_bk.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2365 2024-03-25 04:28:28.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/smooth.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4275 2024-01-09 08:28:12.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/smooth_.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7397 2023-09-14 07:59:51.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/spark.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4496 2024-03-26 05:48:00.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/stepchat.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8300 2024-04-03 05:48:58.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/suno.py
+-rw-r--r--   0 betterme   (501) staff       (20)    10613 2024-03-27 13:05:43.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/suno_.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6454 2024-03-28 05:02:51.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/suno__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5720 2024-04-03 10:28:14.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/suno_api.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.795684 chatllm-2024.4.3.18.28.17/chatllm/llmchain/decorators/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2023-07-31 03:48:34.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/decorators/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1982 2024-02-08 02:05:28.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/decorators/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.797894 chatllm-2024.4.3.18.28.17/chatllm/llmchain/document_loaders/
+-rw-r--r--   0 betterme   (501) staff       (20)     2448 2024-02-07 06:21:54.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/document_loaders/FilesLoader.py
+-rw-r--r--   0 betterme   (501) staff       (20)      673 2024-03-18 03:22:30.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/document_loaders/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1713 2024-02-07 06:21:40.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/document_loaders/docx.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4836 2024-03-18 12:05:06.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/document_loaders/file.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3219 2024-03-18 07:47:50.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/document_loaders/file_loader.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2220 2024-02-07 06:21:54.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/document_loaders/image.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1842 2024-02-07 06:21:54.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/document_loaders/pdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1787 2024-02-07 05:46:15.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/document_loaders/text.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.799740 chatllm-2024.4.3.18.28.17/chatllm/llmchain/embeddings/
+-rw-r--r--   0 betterme   (501) staff       (20)      935 2024-02-07 08:58:55.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/embeddings/ApiEmbeddings.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3534 2024-02-07 08:57:18.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/embeddings/DashScopeEmbeddings.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1332 2024-02-07 08:57:18.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/embeddings/HuggingFaceEmbeddings.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2327 2024-02-07 08:57:18.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/embeddings/OpenAIEmbeddings.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2722 2023-12-20 01:40:26.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/embeddings/XunfeiEmbedding.py
+-rw-r--r--   0 betterme   (501) staff       (20)      507 2023-08-10 08:01:04.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/embeddings/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7482 2024-03-15 05:39:32.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/embeddings/openai_embeddings.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.801921 chatllm-2024.4.3.18.28.17/chatllm/llmchain/llms/
+-rw-r--r--   0 betterme   (501) staff       (20)      546 2023-12-05 07:56:51.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/llms/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1667 2024-02-07 08:56:45.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/llms/basellm.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3362 2024-02-07 08:56:45.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/llms/chatglm.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3901 2024-02-07 08:56:45.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/llms/ernie.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3395 2024-02-07 08:56:45.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/llms/hunyuan.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2437 2023-12-05 07:50:17.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/llms/kimi.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-07-24 05:47:03.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/llms/minimax.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2286 2024-02-08 01:57:34.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/llms/spark.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.803723 chatllm-2024.4.3.18.28.17/chatllm/llmchain/prompts/
+-rw-r--r--   0 betterme   (501) staff       (20)      243 2023-11-09 05:49:28.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/prompts/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      639 2023-09-25 09:52:28.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/prompts/kb.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2963 2023-09-20 01:09:40.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/prompts/ocr.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4625 2024-02-07 08:56:45.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/prompts/prompt_templates.py
+-rw-r--r--   0 betterme   (501) staff       (20)      722 2023-07-13 02:06:43.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/prompts/prompt_watch.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2488 2024-02-07 08:56:45.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/prompts/rag.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1973 2024-02-07 08:56:45.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/prompts/格式化.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1650 2024-03-27 16:11:48.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/suno.md
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.804844 chatllm-2024.4.3.18.28.17/chatllm/llmchain/textsplitter/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-08-16 06:10:25.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/textsplitter/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1389 2023-05-15 07:48:48.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/textsplitter/ali_text_splitter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3356 2023-07-15 06:05:38.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/textsplitter/chinese_text_splitter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3179 2023-06-30 13:02:46.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/textsplitter/zh_title_enhance.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.805300 chatllm-2024.4.3.18.28.17/chatllm/llmchain/utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      280 2023-07-31 03:48:34.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2653 2024-02-08 02:05:02.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/utils/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.807444 chatllm-2024.4.3.18.28.17/chatllm/llmchain/vectorstores/
+-rw-r--r--   0 betterme   (501) staff       (20)      910 2024-02-07 08:59:38.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/vectorstores/DocArrayInMemorySearch.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3891 2024-02-23 03:20:33.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/vectorstores/ElasticsearchStore.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4126 2024-02-07 08:59:38.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/vectorstores/FAISS.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1334 2024-02-07 08:59:38.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/vectorstores/Milvus.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4515 2024-02-07 08:59:38.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/vectorstores/Usearch.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4593 2024-02-07 08:59:38.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/vectorstores/VectorRecordManager.py
+-rw-r--r--   0 betterme   (501) staff       (20)      661 2023-09-19 01:20:05.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/vectorstores/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1567 2023-07-14 01:13:07.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/vectorstores/base.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1332 2024-02-07 08:59:38.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/vectorstores/index_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.808760 chatllm-2024.4.3.18.28.17/chatllm/llms/
+-rw-r--r--   0 betterme   (501) staff       (20)     1526 2023-06-02 12:11:10.000000 chatllm-2024.4.3.18.28.17/chatllm/llms/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2307 2023-06-30 12:28:42.000000 chatllm-2024.4.3.18.28.17/chatllm/llms/chatglm.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1143 2023-07-03 09:18:07.000000 chatllm-2024.4.3.18.28.17/chatllm/llms/chatgpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1559 2023-05-22 08:19:27.000000 chatllm-2024.4.3.18.28.17/chatllm/llms/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2083 2023-05-22 08:39:00.000000 chatllm-2024.4.3.18.28.17/chatllm/llms/llama.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.809218 chatllm-2024.4.3.18.28.17/chatllm/prompts/
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-06-12 03:51:17.000000 chatllm-2024.4.3.18.28.17/chatllm/prompts/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1556 2023-11-20 08:02:57.000000 chatllm-2024.4.3.18.28.17/chatllm/prompts/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.812096 chatllm-2024.4.3.18.28.17/chatllm/schemas/
+-rw-r--r--   0 betterme   (501) staff       (20)     1790 2023-12-11 10:49:08.000000 chatllm-2024.4.3.18.28.17/chatllm/schemas/4v.py
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-07-31 02:38:12.000000 chatllm-2024.4.3.18.28.17/chatllm/schemas/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5022 2024-03-21 06:09:38.000000 chatllm-2024.4.3.18.28.17/chatllm/schemas/chatglm_types.py
+-rw-r--r--   0 betterme   (501) staff       (20)      867 2024-01-11 01:35:59.000000 chatllm-2024.4.3.18.28.17/chatllm/schemas/embedding.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.812654 chatllm-2024.4.3.18.28.17/chatllm/schemas/json_schema_extra/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2024-01-19 07:34:54.000000 chatllm-2024.4.3.18.28.17/chatllm/schemas/json_schema_extra/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.813598 chatllm-2024.4.3.18.28.17/chatllm/schemas/kimi/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-11-29 08:43:08.000000 chatllm-2024.4.3.18.28.17/chatllm/schemas/kimi/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2689 2023-12-28 01:16:22.000000 chatllm-2024.4.3.18.28.17/chatllm/schemas/kimi/protocol.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3193 2024-02-29 08:15:07.000000 chatllm-2024.4.3.18.28.17/chatllm/schemas/kimi/state.json
+-rw-r--r--   0 betterme   (501) staff       (20)     3607 2024-03-21 11:03:35.000000 chatllm-2024.4.3.18.28.17/chatllm/schemas/kimi_types.py
+-rw-r--r--   0 betterme   (501) staff       (20)      340 2023-11-03 10:59:44.000000 chatllm-2024.4.3.18.28.17/chatllm/schemas/metadata.py
+-rw-r--r--   0 betterme   (501) staff       (20)    12079 2024-03-27 13:44:00.000000 chatllm-2024.4.3.18.28.17/chatllm/schemas/openai_api_protocol.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4451 2024-03-27 04:49:24.000000 chatllm-2024.4.3.18.28.17/chatllm/schemas/openai_types.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4065 2024-03-28 12:59:41.000000 chatllm-2024.4.3.18.28.17/chatllm/schemas/suno_types.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.815169 chatllm-2024.4.3.18.28.17/chatllm/serve/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-07-31 02:40:14.000000 chatllm-2024.4.3.18.28.17/chatllm/serve/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    29234 2023-07-31 02:44:27.000000 chatllm-2024.4.3.18.28.17/chatllm/serve/_openai_api_server.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1178 2024-02-07 08:56:45.000000 chatllm-2024.4.3.18.28.17/chatllm/serve/app.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1870 2023-07-19 10:34:49.000000 chatllm-2024.4.3.18.28.17/chatllm/serve/constants.py
+-rw-r--r--   0 betterme   (501) staff       (20)    25416 2023-08-24 00:45:22.000000 chatllm-2024.4.3.18.28.17/chatllm/serve/openai_api_server.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.817363 chatllm-2024.4.3.18.28.17/chatllm/utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      278 2023-04-28 04:20:30.000000 chatllm-2024.4.3.18.28.17/chatllm/utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 04:37:16.000000 chatllm-2024.4.3.18.28.17/chatllm/utils/_textsplitter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2270 2024-02-06 13:51:45.000000 chatllm-2024.4.3.18.28.17/chatllm/utils/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2430 2023-05-19 09:28:43.000000 chatllm-2024.4.3.18.28.17/chatllm/utils/gpu_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6342 2023-05-30 08:31:55.000000 chatllm-2024.4.3.18.28.17/chatllm/utils/nbce.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5208 2023-05-30 08:22:36.000000 chatllm-2024.4.3.18.28.17/chatllm/utils/nbce_test.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3360 2024-03-22 08:36:40.000000 chatllm-2024.4.3.18.28.17/chatllm/utils/openai_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.833471 chatllm-2024.4.3.18.28.17/chatllm/webui/
+-rw-r--r--   0 betterme   (501) staff       (20)     7568 2023-11-09 06:40:18.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/!.png
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)   225373 2023-09-28 00:58:21.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/bot.png
+-rw-r--r--   0 betterme   (501) staff       (20)     2747 2023-08-11 06:45:35.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/chat.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1826 2023-12-14 02:59:58.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/chat_copilot.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1457 2023-05-29 07:27:53.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)   123851 2023-10-26 08:17:41.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/chatbook.png
+-rw-r--r--   0 betterme   (501) staff       (20)     5660 2024-02-07 08:56:45.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/chatbook.py
+-rw-r--r--   0 betterme   (501) staff       (20)    14406 2023-09-05 09:04:59.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/chatbot.png
+-rw-r--r--   0 betterme   (501) staff       (20)     3389 2023-09-25 01:29:31.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/chatbot.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4044 2023-08-28 06:36:36.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/chatfile.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5642 2024-02-07 08:56:45.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/chatfile_nesc.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1968 2024-03-25 06:05:55.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/chatfile_nesc_glm_v0.1.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2417 2024-03-20 09:52:09.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/chatfile_nesc_last.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5741 2024-02-07 08:56:45.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/chatfile_nesc_v1.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3103 2024-01-12 05:56:43.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/chatfile_nesc_v2.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2781 2024-02-01 14:00:42.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/chatfile_v0.1.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1076 2023-06-29 07:59:43.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/chatmind.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3103 2023-08-23 04:01:26.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)      134 2023-06-26 02:13:58.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/conf.yaml
+-rw-r--r--   0 betterme   (501) staff       (20)     1093 2023-11-06 09:12:04.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/dalle.py
+-rw-r--r--   0 betterme   (501) staff       (20)      554 2023-11-15 06:57:01.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4235 2024-01-25 05:24:50.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/fire.png
+-rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/gradio_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)   856440 2023-09-25 01:29:08.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/logo.png
+-rw-r--r--   0 betterme   (501) staff       (20)   102641 2023-08-11 06:34:47.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/nesc.jpeg
+-rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/nice_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)      557 2024-02-07 08:56:45.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/prompt_maker.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4445 2024-02-07 08:59:38.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/qa.py
+-rw-r--r--   0 betterme   (501) staff       (20)      468 2024-03-26 09:28:22.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/run.sh
+-rw-r--r--   0 betterme   (501) staff       (20)     4312 2023-08-08 10:37:46.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/user.jpg
+-rw-r--r--   0 betterme   (501) staff       (20)     3506 2023-05-26 07:39:23.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/visualglm_st.py
+-rw-r--r--   0 betterme   (501) staff       (20)   437368 2024-01-12 05:38:09.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/副本人工智能咨询服务协议 汉洁 南京当月糯 20240105(1)(1).docx
+-rw-r--r--   0 betterme   (501) staff       (20)    10521 2024-02-01 13:14:34.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/同程报价.xlsx
+-rw-r--r--   0 betterme   (501) staff       (20)   303359 2023-09-20 06:32:26.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/规丞相.png
+-rw-r--r--   0 betterme   (501) staff       (20)   414314 2024-02-01 13:16:20.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/酒店百问百答.pdf
+-rw-r--r--   0 betterme   (501) staff       (20)   741995 2024-01-12 05:38:20.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/附件1：东北证券股份有限公司员工合规手册（2023年12月）.doc
+-rw-r--r--   0 betterme   (501) staff       (20)   416458 2023-12-27 07:56:52.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/附件1：东北证券股份有限公司员工合规手册（2023年12月）.docx
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.841617 chatllm-2024.4.3.18.28.17/chatllm.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     8983 2024-04-03 10:28:18.000000 chatllm-2024.4.3.18.28.17/chatllm.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     9242 2024-04-03 10:28:18.000000 chatllm-2024.4.3.18.28.17/chatllm.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2024-04-03 10:28:18.000000 chatllm-2024.4.3.18.28.17/chatllm.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       53 2024-04-03 10:28:18.000000 chatllm-2024.4.3.18.28.17/chatllm.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2024-04-03 10:28:18.000000 chatllm-2024.4.3.18.28.17/chatllm.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)      425 2024-04-03 10:28:18.000000 chatllm-2024.4.3.18.28.17/chatllm.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2024-04-03 10:28:18.000000 chatllm-2024.4.3.18.28.17/chatllm.egg-info/top_level.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      684 2023-03-20 02:44:39.000000 chatllm-2024.4.3.18.28.17/clear_git_history.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.840081 chatllm-2024.4.3.18.28.17/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 chatllm-2024.4.3.18.28.17/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 chatllm-2024.4.3.18.28.17/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 chatllm-2024.4.3.18.28.17/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 chatllm-2024.4.3.18.28.17/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 chatllm-2024.4.3.18.28.17/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 chatllm-2024.4.3.18.28.17/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 chatllm-2024.4.3.18.28.17/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 chatllm-2024.4.3.18.28.17/docs/readme.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)      350 2023-10-16 06:38:24.000000 chatllm-2024.4.3.18.28.17/git_init.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 chatllm-2024.4.3.18.28.17/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)      137 2023-09-14 06:48:16.000000 chatllm-2024.4.3.18.28.17/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       14 2023-05-19 09:53:16.000000 chatllm-2024.4.3.18.28.17/requirements_ann.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       30 2023-05-31 02:41:18.000000 chatllm-2024.4.3.18.28.17/requirements_api.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       29 2023-05-26 08:03:09.000000 chatllm-2024.4.3.18.28.17/requirements_openai.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-05-29 04:24:55.000000 chatllm-2024.4.3.18.28.17/requirements_pdf.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       22 2024-01-09 05:49:39.000000 chatllm-2024.4.3.18.28.17/requirements_rag.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       25 2023-05-29 04:24:55.000000 chatllm-2024.4.3.18.28.17/requirements_streamlit.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       38 2024-04-03 10:28:18.843721 chatllm-2024.4.3.18.28.17/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1706 2023-07-19 10:53:05.000000 chatllm-2024.4.3.18.28.17/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.841030 chatllm-2024.4.3.18.28.17/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 chatllm-2024.4.3.18.28.17/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1224 2023-12-11 01:53:35.000000 chatllm-2024.4.3.18.28.17/tests/oneapi_test.py
+-rw-r--r--   0 betterme   (501) staff       (20)      224 2023-10-25 08:02:40.000000 chatllm-2024.4.3.18.28.17/tests/test_llm4gpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)    51173 2023-04-21 11:31:44.000000 chatllm-2024.4.3.18.28.17/tests/内存型.ipynb
```

### Comparing `chatllm-2024.3.8.19.26.56/.gitignore` & `chatllm-2024.4.3.18.28.17/.gitignore`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/LICENSE` & `chatllm-2024.4.3.18.28.17/LICENSE`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/LLMS.md` & `chatllm-2024.4.3.18.28.17/LLMS.md`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/Makefile` & `chatllm-2024.4.3.18.28.17/Makefile`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/PKG-INFO` & `chatllm-2024.4.3.18.28.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatllm
-Version: 2024.3.8.19.26.56
+Version: 2024.4.3.18.28.17
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: chatllm
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -43,25 +43,25 @@
 Requires-Dist: streamlit; extra == "streamlit"
 Requires-Dist: streamlit_chat; extra == "streamlit"
 Provides-Extra: rag
 Requires-Dist: redis; extra == "rag"
 Requires-Dist: minio; extra == "rag"
 Requires-Dist: faiss-cpu; extra == "rag"
 Provides-Extra: all
-Requires-Dist: streamlit_chat; extra == "all"
-Requires-Dist: fastapi; extra == "all"
-Requires-Dist: qdrant-client; extra == "all"
-Requires-Dist: openai; extra == "all"
-Requires-Dist: streamlit; extra == "all"
 Requires-Dist: pymupdf; extra == "all"
-Requires-Dist: sse_starlette; extra == "all"
-Requires-Dist: minio; extra == "all"
 Requires-Dist: sse-starlette; extra == "all"
-Requires-Dist: faiss-cpu; extra == "all"
+Requires-Dist: streamlit; extra == "all"
+Requires-Dist: sse_starlette; extra == "all"
 Requires-Dist: redis; extra == "all"
+Requires-Dist: streamlit_chat; extra == "all"
+Requires-Dist: openai; extra == "all"
+Requires-Dist: faiss-cpu; extra == "all"
+Requires-Dist: minio; extra == "all"
+Requires-Dist: qdrant-client; extra == "all"
+Requires-Dist: fastapi; extra == "all"
 
 ![image](https://img.shields.io/pypi/v/chatllm.svg) ![image](https://img.shields.io/travis/yuanjie-ai/chatllm.svg) ![image](https://readthedocs.org/projects/chatllm/badge/?version=latest)
 
 <h1 align = "center">🔥ChatLLM 基于知识库🔥</h1>
 
 <div align=center>
 <img src="data/imgs/LLM.drawio.png"/>
```

### Comparing `chatllm-2024.3.8.19.26.56/README.md` & `chatllm-2024.4.3.18.28.17/README.md`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/README.md.bak` & `chatllm-2024.4.3.18.28.17/README.md.bak`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/TODO.md` & `chatllm-2024.4.3.18.28.17/TODO.md`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/apps/allchat.py` & `chatllm-2024.4.3.18.28.17/apps/allchat.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/agent/MultiPrompt.py` & `chatllm-2024.4.3.18.28.17/chatllm/agent/MultiPrompt.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/aigc/common.py` & `chatllm-2024.4.3.18.28.17/chatllm/aigc/common.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/api/app.py` & `chatllm-2024.4.3.18.28.17/chatllm/api/app.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/api/config.py` & `chatllm-2024.4.3.18.28.17/chatllm/api/config.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/api/datamodels.py` & `chatllm-2024.4.3.18.28.17/chatllm/api/datamodels.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/api/openai_client.py` & `chatllm-2024.4.3.18.28.17/chatllm/api/openai_client.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/api/routers/all_chat_completions.py` & `chatllm-2024.4.3.18.28.17/chatllm/api/routers/all_chat_completions.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/api/routers/all_chat_completions_.py` & `chatllm-2024.4.3.18.28.17/chatllm/api/routers/all_chat_completions_.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,16 @@
         from chatllm.llmchain.applications import ChatFiles
 
         minio_client = Minio(
             endpoint=os.getenv('MINIO_ENDPOINT'),
             access_key=os.getenv('MINIO_ACCESS_KEY'),
             secret_key=os.getenv('MINIO_SECRET_KEY'),
             secure=False)
+        minio_client.presigned_get_object()
+
 
         file_map = {} or Redis(**os.getenv("REDIS_CLIENT_PARAMS", {}), decode_responses=True)
 
         file_id = request.file_id or f"file-{model.split('-file-')[-1]}"
         file_name = file_map.get(file_id)
 
         logger.debug(file_id)
```

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/api/routers/api.py` & `chatllm-2024.4.3.18.28.17/chatllm/api/routers/api.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/api/routers/chat_completions_extra.py` & `chatllm-2024.4.3.18.28.17/chatllm/api/routers/chat_completions_extra.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,18 +16,14 @@
 from fastapi import APIRouter, File, UploadFile, Query, Form, Depends, Request, HTTPException, status
 from fastapi.responses import RedirectResponse
 
 from openai import OpenAI, AsyncOpenAI
 from openai.types.chat import ChatCompletion, ChatCompletionChunk
 
 from chatllm.utils.openai_utils import to_openai_completion_params, openai_response2sse
-from chatllm.llmchain.completions import moonshot_kimi
-from chatllm.llmchain.completions import deepseek
-from chatllm.llmchain.applications import chaturl
-
 from chatllm.schemas.openai_types import chat_completion_per, chat_completion_slogan, chat_completion_chunk_slogan
 from chatllm.schemas.openai_api_protocol import ChatCompletionRequest, UsageInfo
 
 router = APIRouter()
 
 ChatCompletionResponse = Union[ChatCompletion, List[ChatCompletionChunk]]
```

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/api/routers/chat_completions_kimi.py` & `chatllm-2024.4.3.18.28.17/chatllm/api/routers/chat_completions_kimi.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/api/routers/chat_completions_rag.py` & `chatllm-2024.4.3.18.28.17/chatllm/api/routers/chat_completions_rag.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/api/routers/chat_completions_redirect.py` & `chatllm-2024.4.3.18.28.17/chatllm/api/routers/chat_completions_redirect.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/api/routers/cocopilot.py` & `chatllm-2024.4.3.18.28.17/chatllm/api/routers/cocopilot.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,21 +22,21 @@
         # "Accept": "*/*",
         # "Accept-Encoding": "gzip, deflate, br",
         # "Connection": "close"
     }
     # response = requests.get('https://api.github.com/copilot_internal/v2/token', headers=headers)
     # response = requests.get('https://enterprise.mstp.online/copilot_internal/v2/token', headers=headers)
     url = 'http://152.136.138.142:28443'
-    # url = 'http://D45B233069CB4852915E7EEE1B97922E@152.136.138.142:28443'
-    url = "https://highcopilot.micosoft.icu" # MTI3LmI4Y2JkOWNkMGEwZTgxZGRmOGEyY2I4YzkwOGYzOTkw
+    url = 'http://152.136.138.142:28443'
+    # url = "https://highcopilot.micosoft.icu" # MTI3LmI4Y2JkOWNkMGEwZTgxZGRmOGEyY2I4YzkwOGYzOTkw
     response = requests.get(f'{url}/copilot_internal/v2/token', headers=headers)
 
     # print("Auth:", response.text)
     return response.json()
 
 "https://copilot-proxy.githubusercontent.com/v1/engines/copilot-codex/completions"
 
-print(forward_request('MTI3LmI4Y2JkOWNkMGEwZTgxZGRmOGEyY2I4YzkwOGYzOTkw'))
+print(forward_request('D45B233069CB4852915E7EEE1B97922E'))
 
 # Auth: {"message":"请先退出账号 重新登陆授权","error_details":{"url":"https://copilotglobal.me","message":"请先退出账号 重新登陆授权","title":"Copilot Global","notification_id":"feature_flag_blocked"}}
 
 # {'annotations_enabled': False, 'chat_enabled': True, 'chat_jetbrains_enabled': True, 'code_quote_enabled': False, 'copilot_ide_agent_chat_gpt4_small_prompt': False, 'copilotignore_enabled': False, 'expires_at': 3417858815, 'intellij_editor_fetcher': False, 'prompt_8k': True, 'public_suggestions': 'disabled', 'refresh_in': 60, 'sku': 'trial_30_monthly_subscriber', 'snippy_load_test_enabled': False, 'telemetry': 'disabled', 'token': 'tid=60915f939e94c7ea27b53e46416ae003;exp=1708930130;sku=trial_30_monthly_subscriber;st=dotcom;chat=1;sn=1;8kp=1:a4ef112c506ff1ec951570adeb009b3d939140028b672d4506d119ab7e18691b', 'tracking_id': '60915f939e94c7ea27b53e46416ae003', 'vsc_panel_v2': False}
```

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/api/routers/embeddings.py` & `chatllm-2024.4.3.18.28.17/chatllm/api/routers/embeddings.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 @router.post("/embeddings", summary="Embedding")  # request.model_dump(exclude={"user"})
 async def create_embeddings(
     request: EmbeddingRequest,
     auth: Optional[HTTPAuthorizationCredentials] = Depends(get_bearer_token),
 ) -> CreateEmbeddingResponse:
     logger.debug(request)
 
-    api_key = auth and auth.credentials or None
+    api_key = auth and auth.credentials or None  # api_key错误发生了阻塞
     if api_key is None:
         detail = {
             "error": {
                 "message": "",
                 "type": "invalid_request_error",
                 "param": None,
                 "code": "invalid_api_key",
```

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/api/routers/files/files_minio.py` & `chatllm-2024.4.3.18.28.17/chatllm/api/routers/files_moonshot.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,149 +4,140 @@
 # @File         : files
 # @Time         : 2023/12/29 14:21
 # @Author       : betterme
 # @WeChat       : meutils
 # @Software     : PyCharm
 # @Description  : todo: 返回链接，参考kimi，接入文档解析，16c32g机器部署，不能通服务调用, minio_client通用化 id 映射
 
-import shortuuid
+# 注意，单个用户最多只能上传 1000 个文件，单文件不超过100MB，同时所有已上传的文件总和不超过 10G 容量。如果您要抽取更多文件，需要先删除一部分不再需要的文件。
 
 from meutils.pipe import *
 from meutils.serving.fastapi.dependencies.auth import get_bearer_token, HTTPAuthorizationCredentials
 from chatllm.utils.openai_utils import per_create
+from chatllm.llmchain.completions import kimi
 
 from enum import Enum
-from minio import Minio
-from redis import Redis
 from openai import OpenAI
 from openai._types import FileTypes
 from openai.types.file_object import FileObject
 from fastapi import APIRouter, File, UploadFile, Query, Form, BackgroundTasks, Depends, HTTPException, Request, status
 from fastapi.responses import Response, FileResponse
 
 router = APIRouter()
 
-file_map = {} or Redis(**os.getenv("REDIS_CLIENT_PARAMS", {}), decode_responses=True)  # redis_client_params
+client = OpenAI(
+    api_key=os.getenv('MOONSHOT_API_KEY'),
+    base_url=os.getenv('MOONSHOT_BASE_URL'),
+)
 
 
 class Purpose(str, Enum):
     file_extract = "file-extract"
     assistants = "assistants"
     fine_tune = "fine-tune"
 
 
-minio_client = Minio(
-    endpoint=os.getenv('MINIO_ENDPOINT'),
-    access_key=os.getenv('MINIO_ACCESS_KEY'),
-    secret_key=os.getenv('MINIO_SECRET_KEY'),
-    secure=False if ":" in os.getenv('MINIO_ENDPOINT') else True
-)
+@router.get("/files")
+async def get_files(
+    auth: Optional[HTTPAuthorizationCredentials] = Depends(get_bearer_token),
+):
+    api_key = auth and auth.credentials or None
+    if api_key is None:
+        raise HTTPException(status_code=status.HTTP_401_UNAUTHORIZED, detail="认证失败")
 
-OPENAI_BUCKET = os.getenv('OPENAI_BUCKET', 'openai')
+    try:
+        _ = per_create(api_key=api_key)  # 按次计费
+    except Exception as e:
+        raise HTTPException(status_code=status.HTTP_401_UNAUTHORIZED, detail=str(e))
+
+    return client.files.list()
 
 
 @router.get("/files/{file_id}")
-async def get_files(
+async def get_file(
     file_id: str,
     auth: Optional[HTTPAuthorizationCredentials] = Depends(get_bearer_token),
 
 ):
     api_key = auth and auth.credentials or None
     if api_key is None:
         raise HTTPException(status_code=status.HTTP_401_UNAUTHORIZED, detail="认证失败")
-
     try:
-        file_name = file_map.get(file_id)
-        response = minio_client.get_object(OPENAI_BUCKET, f"{api_key}/{file_name}")
-        data = response.read()
-
-        return FileObject(
-            id=file_id,
-            bytes=len(data),
-            created_at=int(time.time()),
-            filename=file_name,
-            object='file',
-            purpose='assistants',
-            status='uploaded',
-        )
+        _ = per_create(api_key=api_key)  # 按次计费
     except Exception as e:
-        raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail=f"File error: {e}")
+        raise HTTPException(status_code=status.HTTP_401_UNAUTHORIZED, detail=str(e))
+
+    return client.files.retrieve(file_id=file_id)
 
 
 @router.get("/files/{file_id}/content")
-async def get_files_content(
+async def get_file_content(
     file_id: str,
     auth: Optional[HTTPAuthorizationCredentials] = Depends(get_bearer_token),
 
 ):
     api_key = auth and auth.credentials or None
     if api_key is None:
         raise HTTPException(status_code=status.HTTP_401_UNAUTHORIZED, detail="认证失败")
     try:
-        file_name = file_map.get(file_id)
-        response = minio_client.get_object(OPENAI_BUCKET, f"{api_key}/{file_name}")  # 获取链接
-        data = response.data
+        _ = per_create(api_key=api_key)  # 按次计费
+    except Exception as e:
+        raise HTTPException(status_code=status.HTTP_401_UNAUTHORIZED, detail=str(e))
+
+    file_content = client.files.content(file_id=file_id).text
+    return Response(content=file_content, media_type="application/octet-stream")
 
-        return Response(content=data, media_type="application/octet-stream")
+
+@router.delete("/files/{file_id}")
+async def delete_file(
+    file_id: str,
+    auth: Optional[HTTPAuthorizationCredentials] = Depends(get_bearer_token),
+):
+    api_key = auth and auth.credentials or None
+    if api_key is None:
+        raise HTTPException(status_code=status.HTTP_401_UNAUTHORIZED, detail="认证失败")
+
+    try:
+        _ = per_create(api_key=api_key)  # 按次计费
     except Exception as e:
-        raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail=f"File content error: {e}")
+        raise HTTPException(status_code=status.HTTP_401_UNAUTHORIZED, detail=str(e))
+
+    return client.files.delete(file_id=file_id)
 
 
 @router.post("/files")  # 同名文件会被覆盖
 async def upload_files(
     file: UploadFile = File(...),
     purpose: Purpose = Form(...),
     # return_url=Form(...)
     auth: Optional[HTTPAuthorizationCredentials] = Depends(get_bearer_token),
 
 ):
     api_key = auth and auth.credentials or None
     if api_key is None:
         raise HTTPException(status_code=status.HTTP_401_UNAUTHORIZED, detail="认证失败")
 
-    if purpose == Purpose.fine_tune:
-        # 对于微调，验证上传文件的格式
-        content = await file.read()
-        try:
-            lines = content.decode().split("\n")
-            for line in lines:
-                record = json.loads(line)
-                if "prompt" not in record or "completion" not in record:
-                    raise ValueError("Invalid format")
-        except:
-            raise HTTPException(status_code=400, detail="Invalid file format for fine-tuning")
-    elif purpose == Purpose.assistants:
-        # 对于助手和消息，你可能需要进行不同的处理
-        # todo: 直接解析到 es【后面支持队列】
-
-        minio_client.put_object(OPENAI_BUCKET, f"{api_key}/{file.filename}", data=file.file, length=file.size)
-
-        # fileid2filename
-        file_id = f"file-{hash(file.filename)}"
-        file_map[file_id] = file.filename  # shortuuid.uuid('a') "file-HASH"
-        # logger.debug(file_map)
-
-        # 按次计费
-        try:
-            _ = per_create(api_key=api_key)  # 无效key
-        except Exception as e:
-            logger.error(e)
-            raise HTTPException(status_code=status.HTTP_401_UNAUTHORIZED, detail="认证失败")
-
-        return FileObject(
-            # id=f"file-{shortuuid.random()}",  # 新的模型名称
-            id=file_id,
-
-            bytes=file.size,
-            created_at=int(time.time()),
-            filename=file.filename,
-            object='file',
-            purpose='assistants',
-            status='uploaded',  # Deprecated
-        )
+    try:
+        _ = per_create(api_key=api_key, model='per-file')  # 按次计费
+    except Exception as e:
+        raise HTTPException(status_code=status.HTTP_401_UNAUTHORIZED, detail=str(e))
+
+    # kimi官方api
+    # if 'kimi-api':
+    #     file_object = client.files.create(file=(file.filename, file.file), purpose="file-extract")
+
+    # kimi逆向：验证是否无限文件【跨用户无法问答】
+    # if purpose =='kimi-all':
+    # access_token = httpx.get("http://154.3.0.117:39009/kimi/v1/access_token").text.strip('"')
+    file_object = kimi.Completions().file_extract(file)
+
+    # if hasattr(file, 'filename'):
+    #     file_object.filename = file.filename
+
+    return file_object
 
 
 if __name__ == '__main__':
     from meutils.serving.fastapi import App
 
     VERSION_PREFIX = '/v1'
```

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/api/routers/files/files_moonshot.py` & `chatllm-2024.4.3.18.28.17/chatllm/api/routers/files_moonshot_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # @Description  : todo: 返回链接，参考kimi，接入文档解析，16c32g机器部署，不能通服务调用, minio_client通用化 id 映射
 
 # 注意，单个用户最多只能上传 1000 个文件，单文件不超过100MB，同时所有已上传的文件总和不超过 10G 容量。如果您要抽取更多文件，需要先删除一部分不再需要的文件。
 
 from meutils.pipe import *
 from meutils.serving.fastapi.dependencies.auth import get_bearer_token, HTTPAuthorizationCredentials
 from chatllm.utils.openai_utils import per_create
+from chatllm.llmchain.completions import kimi
 
 from enum import Enum
 from openai import OpenAI
 from openai._types import FileTypes
 from openai.types.file_object import FileObject
 from fastapi import APIRouter, File, UploadFile, Query, Form, BackgroundTasks, Depends, HTTPException, Request, status
 from fastapi.responses import Response, FileResponse
@@ -116,18 +117,17 @@
         raise HTTPException(status_code=status.HTTP_401_UNAUTHORIZED, detail="认证失败")
 
     try:
         _ = per_create(api_key=api_key, model='per-file')  # 按次计费
     except Exception as e:
         raise HTTPException(status_code=status.HTTP_401_UNAUTHORIZED, detail=str(e))
 
-    # file_object
-    file_object = client.files.create(file=(file.filename, file.file), purpose="file-extract")
-    # if hasattr(file, 'filename'):
-    #     file_object.filename = file.filename
+    # kimi官方api
+    if 'kimi-api':
+        file_object = client.files.create(file=(file.filename, file.file), purpose="file-extract")
 
     return file_object
 
 
 if __name__ == '__main__':
     from meutils.serving.fastapi import App
```

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/api/routers/local_embeddings.py` & `chatllm-2024.4.3.18.28.17/chatllm/api/routers/local_embeddings.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/api/routers/models.py` & `chatllm-2024.4.3.18.28.17/chatllm/api/routers/models.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/api/routers/smooth_completions.py` & `chatllm-2024.4.3.18.28.17/chatllm/api/routers/smooth_completions.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/api/routers/speech.py` & `chatllm-2024.4.3.18.28.17/chatllm/api/routers/audio_speech.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,33 +5,44 @@
 # @Time         : 2023/12/26 14:12
 # @Author       : betterme
 # @WeChat       : meutils
 # @Software     : PyCharm
 # @Description  :
 
 from meutils.pipe import *
+from meutils.ai_audio.tts import EdgeTTS
 from meutils.serving.fastapi.dependencies.auth import get_bearer_token, HTTPAuthorizationCredentials
 
 from fastapi import APIRouter, File, UploadFile, Query, Form, Depends, Request, status
 from fastapi.responses import JSONResponse, StreamingResponse
 
-from chatllm.llmchain.audio.speech import Speech
-from chatllm.schemas.openai_types import SpeechCreateRequest
+from chatllm.schemas.openai_types import SpeechCreateRequest  #
 
 router = APIRouter()
 
 
 @router.post("/audio/speech")
 async def create_speech(request: SpeechCreateRequest):
     logger.debug(request)
 
+    # media_types = {
+    #     "mp3": "audio/mpeg",
+    #     "opus": "audio/opus",
+    #     "aac": "audio/aac",
+    #     "flac": "audio/flac",
+    #     "wav": "audio/wav",
+    #     "pcm": "text/event-stream",
+    # }
+    # media_types.get(request.response_format)
+
     try:
         data = request.model_dump()
-        stream = await Speech().acreate(**data)
-        return StreamingResponse(stream)
+        stream = await EdgeTTS().acreate_for_openai(**data)
+
+        return StreamingResponse(stream, media_type="text/event-stream")
 
     except Exception as e:
         logger.error(traceback.format_exc())
 
         return JSONResponse(
             status_code=status.HTTP_400_BAD_REQUEST,
             content={"error": {"message": f"{e}", "type": "api_error"}}
```

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/api/routers/utils.py` & `chatllm-2024.4.3.18.28.17/chatllm/api/routers/utils.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/api/routes/api.py` & `chatllm-2024.4.3.18.28.17/chatllm/api/routes/api.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/api/routes/base.py` & `chatllm-2024.4.3.18.28.17/chatllm/api/routes/base.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/api/routes/completions.py` & `chatllm-2024.4.3.18.28.17/chatllm/api/routes/completions.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/api/routes/embeddings.py` & `chatllm-2024.4.3.18.28.17/chatllm/api/routes/embeddings.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/api/routes/responses.py` & `chatllm-2024.4.3.18.28.17/chatllm/api/routes/responses.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/api/sse_api.py` & `chatllm-2024.4.3.18.28.17/chatllm/api/sse_api.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/api/test.py` & `chatllm-2024.4.3.18.28.17/chatllm/api/test.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/applications/Question2Answer.py` & `chatllm-2024.4.3.18.28.17/chatllm/applications/Question2Answer.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/applications/__chatbase.py` & `chatllm-2024.4.3.18.28.17/chatllm/applications/__chatbase.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/applications/chatann.py` & `chatllm-2024.4.3.18.28.17/chatllm/applications/chatann.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/applications/chatbase.py` & `chatllm-2024.4.3.18.28.17/chatllm/applications/chatbase.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/applications/chatcrawler.py` & `chatllm-2024.4.3.18.28.17/chatllm/applications/chatcrawler.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/applications/chatmind.py` & `chatllm-2024.4.3.18.28.17/chatllm/applications/chatmind.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/applications/chatpdf.py` & `chatllm-2024.4.3.18.28.17/chatllm/applications/chatpdf.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/applications/chatwhoosh.py` & `chatllm-2024.4.3.18.28.17/chatllm/applications/chatwhoosh.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/clis/cli.py` & `chatllm-2024.4.3.18.28.17/chatllm/clis/cli.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/closeai.py` & `chatllm-2024.4.3.18.28.17/chatllm/closeai.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llm_test.py` & `chatllm-2024.4.3.18.28.17/chatllm/llm_test.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/__init__.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/__init__.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/applications/__init__.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/applications/_chatbase.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/_chatbase.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/applications/_chatocr.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/_chatocr.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/applications/chat4all.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chat4all.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/applications/chatbase.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chatbase.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/applications/chatfile.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chatfile.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/applications/chatfiles.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chatfiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from chatllm.schemas.openai_types import chat_completion, chat_completion_chunk
 
 from langchain.text_splitter import *
 from langchain_community.chat_models import ChatOpenAI
 from langchain.chains.question_answering import load_qa_chain
 from langchain.prompts import ChatPromptTemplate
 from langchain_community.document_loaders import UnstructuredFileLoader
-from chatllm.llmchain.document_loaders import FileLoader
+from chatllm.llmchain.document_loaders.file import FileLoader
 
 from meutils.pipe import *
 from meutils.notice.feishu import send_message
 from typing import IO
 
 
 class ChatFiles(object):
```

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/applications/chatocr.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chatocr.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/applications/chatpicture.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chatpicture.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/applications/chatqa.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chatqa.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/applications/chaturl.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chaturl.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/applications/summarizer.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/summarizer.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/audio/speech.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/audio/speech.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/callbacks/streaming.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/callbacks/streaming.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/chat_models/openai.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/chat_models/openai.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/_erniebot.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/_erniebot.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/_hunyuan.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/_hunyuan.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/chat_image.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/chat_image.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/chat_tts.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/chat_tts.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/chatglm.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/chatglm.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/deepseek.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/deepseek.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/dify.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/dify.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/ernie.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/ernie.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/github_copilot.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/github_copilot.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # @Author       : betterme
 # @WeChat       : meutils
 # @Software     : PyCharm
 # @Description  : 不准白嫖 必须 star, todo: 兜底设计、gpt/图片
 # https://github.com/CaoYunzhou/cocopilot-gpt/blob/main/main.py
 # todo: chatfire sdk
 # todo: "https://copilot-proxy.githubusercontent.com/v1/engines/copilot-codex/completions"
+# tddo: 异步
 
 import openai
 
 from meutils.pipe import *
 from meutils.cache_utils import ttl_cache
 from meutils.decorators.retry import retrying
 from meutils.queues.uniform_queue import UniformQueue
@@ -26,91 +27,93 @@
 from chatllm.schemas.openai_api_protocol import ChatCompletionRequest, UsageInfo
 from chatllm.utils.openai_utils import to_openai_completion_params, openai_response2sse
 
 
 class Completions(object):
     def __init__(self, **client_params):
         self.api_key = client_params.get('api_key')
-        self.access_token = self.get_access_token(api_key=self.api_key)
+        if self.api_key.startswith('http'):  # 白嫖 https://chat.aifree.best/api/openai/v1
+            self.access_token = self.api_key
+        else:
+            self.access_token = self.get_access_token(api_key=self.api_key)
         self.completions = openai_completions.Completions(api_key=self.access_token)
 
     def create(self, request: ChatCompletionRequest, **kwargs):
         # logger.debug(request)
 
         request.model = request.model.startswith('gpt-4') and 'gpt-4' or 'gpt-3.5-turbo'
 
         if request.stream:
             stream = self.completions.create(request)
 
             if "gpt-4" in request.model:
-                interval = 0.05
+                interval = 0.06
                 return UniformQueue(stream).consumer(interval=interval, break_fn=self.break_fn)
 
             return stream
 
         else:
             return self.completions.create(request)
 
     def create_sse(self, request: ChatCompletionRequest):
+        redirect_model = request.model
         response = self.create(request)
-        return openai_response2sse(response, redirect_model=request.model)
+        return openai_response2sse(response, redirect_model=redirect_model)
 
     @staticmethod
     def get_access_token(api_key):  # embedding 依赖于此
         token = Completions._get_access_token(api_key=api_key)
+
         # expires_at = int(token.split('exp=')[1][:10])  # tid=7fdaed051cf26939e7cc11e4aed37893;exp=1705749197
         if token and int(token.split('exp=')[1][:10]) < time.time():  # 过期刷新
             token = Completions._get_access_token(api_key, dynamic_param=time.time() // 180)  # 缓存3分钟
         return token
 
     @staticmethod
     @retrying(max_retries=1)
     @ttl_cache(ttl=1200)  # todo: 清除缓存
     def _get_access_token(api_key: Optional[str] = None, dynamic_param=None):
 
         api_key = api_key or os.getenv("GITHUB_COPILOT_TOKEN")
         assert api_key
 
         if api_key.startswith('ghu_'):  # api_key.startswith('ghu_')
-            host = 'api.github.com'
-        elif api_key.startswith('ccu_'):  # api_key.startswith('ghu_')
-            host = 'api.cocopilot.org'
-        elif api_key.startswith('net|ccu_'):  # 新车
-            host = 'api.cocopilot.net'
-            api_key = api_key.strip('net|')
+            host = 'https://api.github.com'
+        elif api_key.startswith('ccu_'):
+            # host = 'api.cocopilot.org'
+            host = 'https://api.cocopilot.net'
         elif len(api_key) == 36:  # 7d0d0949-f7d0-48eb-9117-c557c74f3786
-            host = "enterprise.mstp.online"
+            host = "https://enterprise.mstp.online"
         elif len(api_key) == 48:  # MTI3LmI4Y2JkOWNkMGEwZTgxZGRmOGEyY2I4YzkwOGYzOTkw
-            logger.debug('xxxxx')
-            host = "highcopilot.micosoft.icu"
+            host = "https://highcopilot.micosoft.icu"
         else:
-            api_key = None
-            host = '152.136.138.142:28443'
-            # host = 'D45B233069CB4852915E7EEE1B97922E@152.136.138.142:28443'
+            host = 'http://152.136.138.142:28443'
+            api_key = 'D45B233069CB4852915E7EEE1B97922E'
 
         headers = {
-            'Host': host,
-            # 'authorization': f'Bearer {api_key}',
-            'authorization': f'token {api_key}',
+            'Authorization': f'token {api_key}',
 
             'Editor-Version': 'vscode/1.86.2',
             'Editor-Plugin-Version': 'copilot-chat/0.11.1',
             'User-Agent': 'GitHubCopilotChat/0.11.1',
             'Accept': '*/*'
         }
-        if api_key:
-            url = f"https://{headers.get('Host')}/copilot_internal/v2/token"
-        else:
-            url = f"http://{headers.get('Host')}/copilot_internal/v2/token"
 
-        response = httpx.get(url, headers=headers, timeout=10)  # todo: httpx
+        url = f"{host}/copilot_internal/v2/token"
+
+        response = httpx.get(url, headers=headers)
+
+        logger.debug(response.text)
+
         resp = response.json()
         resp['api_key'] = api_key
         _ = resp.get('token')
 
+        # logger.debug(resp)
+
         if not _:
             send_message(str(resp), "github_copilot异常")
 
         return _
 
     @staticmethod
     def break_fn(line: ChatCompletionChunk):
@@ -203,37 +206,39 @@
     #
     # for i in tqdm(range(1000)):
     #     _ = Completions().create(**data)
     #     print(_.choices[0].message.content)
     #     break
 
     # with timer():
-    api_key = Completions.get_access_token('net|ccu_3LuyRKolN7XCsumLWkG8LVYv3rB53eLohMh4')
+    # api_key = Completions.get_access_token('net|ccu_3LuyRKolN7XCsumLWkG8LVYv3rB53eLohMh4')
 
-    api_key = Completions.get_access_token('MTI3LmI4Y2JkOWNkMGEwZTgxZGRmOGEyY2I4YzkwOGYzOTkw')
+    api_key = Completions.get_access_token('ccu_3LuyRKolN7XCsumLWkG8LVYv3rB53eLohMh411')
+    print(api_key)
 
     # Completions().create(**data)
-    params = dict(
-        api_key=api_key or 'sk-...',
-        base_url='https://api.githubcopilot.com',
-        default_headers={'Editor-Version': 'vscode/1.85.1'},
-
-        max_retries=0,
-        # timeout=5,
-    )
-    from openai import OpenAI
-
-    # 如果这一步就报错呢
-    client = OpenAI(**params)  # todo: 异步
-    data['stream'] = False
-    with timer():
-        try:
-            r = client.chat.completions.create(**data)
-            print(r)
-            for i in r:
-                print(i)
-                if i.choices and i.choices[0].finish_reason == 'content_filter':
-                    print(i.model_dump())
-            #         raise Exception('content_filter error') # Unprocessable Entity
-            # break
-        except Exception as e:  # 'Unprocessable Entity'
-            print(e)
+    # api_key = None
+    # params = dict(
+    #     api_key=api_key or 'sk-...',
+    #     base_url='https://api.githubcopilot.com',
+    #     default_headers={'Editor-Version': 'vscode/1.85.1'},
+    #
+    #     max_retries=0,
+    #     # timeout=5,
+    # )
+    # from openai import OpenAI
+    #
+    # # 如果这一步就报错呢
+    # client = OpenAI(**params)  # todo: 异步
+    # data['stream'] = False
+    # with timer():
+    #     try:
+    #         r = client.chat.completions.create(**data)
+    #         print(r)
+    #         for i in r:
+    #             print(i)
+    #             if i.choices and i.choices[0].finish_reason == 'content_filter':
+    #                 print(i.model_dump())
+    #         #         raise Exception('content_filter error') # Unprocessable Entity
+    #         # break
+    #     except Exception as e:  # 'Unprocessable Entity'
+    #         print(e)
```

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/github_copilot_.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/github_copilot_.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/google_enerativeai.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/google_enerativeai.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/google_enerativeai_.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/google_enerativeai_.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/groq.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/groq.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/hunyuan.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/hunyuan.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/kimi.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/kimi.py`

 * *Files 15% similar despite different names*

```diff
@@ -40,24 +40,29 @@
         with self.httpx_client.stream("POST", url=url, json=payload) as response:
             for line in response.iter_lines():
                 yield from self.do_chunk(line)
 
     async def acreate(self, request: ChatCompletionRequest):
         request = self.do_request(request)
 
+        # chat_id =request.conversation_id or self.chat_id # 会话失败还得重新建
+
         url = f"https://kimi.moonshot.cn/api/chat/{self.chat_id}/completion/stream"
 
         payload = request.model_dump()
         # response = self.httpx_client.post(url=url, json=payload)
         response: httpx.Response
         async with self.httpx_aclient.stream("POST", url=url, json=payload) as response:
             async for line in response.aiter_lines():
                 for chunk in self.do_chunk(line):
                     yield chunk
 
+                    # 多输出几行就可以替换掉kimi【水印】
+                    # 我是Kimi，由月之暗面科技有限公司开发的人工智能助手。我在这里为您提供帮助，回答问题，并协助您处理各种信息和任务。如果您有任何问题或需要帮助，请随时告诉我！
+
     def create_sse(self, request: ChatCompletionRequest):
         if request.stream:
             return openai_response2sse(self.acreate(request), redirect_model=request.model)
         else:
             _chat_completion = chat_completion.model_copy(deep=True)
             _chat_completion.usage.prompt_tokens = len(request.messages[-1]["content"])
             for i in self.create(request):
@@ -65,35 +70,43 @@
 
             return openai_response2sse(_chat_completion, redirect_model=request.model)
 
     def do_request(self, request: ChatCompletionRequest):
 
         history = request.messages[:-1]
         history = history and f"""可参考系统历史对话回答问题：\n```json\n{json.dumps(history, ensure_ascii=False, indent=4)}\n```"""  # todo: 优化
+        # history = history and f"""History:\n```json\n{json.dumps(history, ensure_ascii=False, indent=4)}\n```"""
 
         question = request.messages[-1]["content"]
+        if isinstance(question, list):
+            # 文件  {"type": "image_url", "image_url": {"url": image_url1}}
+            # {
+            #     "type": "http://ai.chatfire.cn/files/document/绩效面谈表-模版-nine-1710139239100-nine-66b3829d5.pdf text"
+            # }
+
+            send_message(request.messages)
 
         # 链接转换
         if not request.model.startswith(("moonshot",)):  # moonshot不支持链接
             question = self._url2content(question) or question
 
         request.messages = [
             {
                 'role': 'user',
-                'content': f"""{history}\n\n问题：{question}""" if history else question
+                'content': f"""{history}\n\nQuery: {question}""" if history else question
             }
         ]
 
         return request
 
     def do_chunk(self, line):
 
         if line := line.strip().strip('data: '):
 
-            # logger.debug(line)
+            logger.debug(line)
 
             kimi_data = KimiData.model_validate_json(line)
 
             for chunk in self.search_plus(kimi_data):
                 yield chunk
 
             if kimi_data.event == 'cmpl':
@@ -171,15 +184,15 @@
         if response.status_code != 200:
             send_message(f"Kimi refresh_token:\n\n{response.text}\n\n{refresh_token}", title="Kimi")
             response.raise_for_status()
 
         # refresh_token = response.get("refresh_token") # 是否去更新
         return response.json().get("access_token")
 
-    def file_extract(self, file: Union[str, UploadFile]):
+    def file_extract(self, file: Union[str, Path, UploadFile]):
 
         if isinstance(file, str) and Path(file).exists():
             filename = Path(file).name
             file = Path(file).read_bytes()
         else:
             filename = file.filename or file.file.name
             file = file.file
@@ -198,40 +211,57 @@
         self.httpx_client.put(url, files=files)
 
         # 获取文件id
         url = "https://kimi.moonshot.cn/api/file"
         payload = {"type": "file", "name": filename, "object_name": object_name}
         file_response = self.httpx_client.post(url, json=payload, headers=self.headers).json()
 
-        logger.debug(file_response)
+        # logger.debug(file_response)
+        # {
+        #     "id": "cnrtn82lnl9f8h6k6eqg",
+        #     "name": "东北证券股份有限公司合规手册（东证合规发〔2023〕22号 20231228）.pdf",
+        #     "parent_path": "",
+        #     "type": "file",
+        #     "status": "initialized",
+        #     "presigned_url": "https://prod-chat-kimi.tos-s3-cn-beijing.volces.com/prod-chat-kimi/cki094b3aeslglj6fo2g/2024-03-18/cnrtn7998onq6ckol4jg/%E4%B8%9C%E5%8C%97%E8%AF%81%E5%88%B8%E8%82%A1%E4%BB%BD%E6%9C%89%E9%99%90%E5%85%AC%E5%8F%B8%E5%90%88%E8%A7%84%E6%89%8B%E5%86%8C%EF%BC%88%E4%B8%9C%E8%AF%81%E5%90%88%E8%A7%84%E5%8F%91%E3%80%942023%E3%80%9522%E5%8F%B7%2020231228%EF%BC%89.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256\u0026X-Amz-Credential=AKLTYTJlNjgwMjY2ZDBkNDFiYmI5YWNiZDBlZmFmYjIzZTA%2F20240318%2Fcn-beijing%2Fs3%2Faws4_request\u0026X-Amz-Date=20240318T061352Z\u0026X-Amz-Expires=3600\u0026X-Amz-SignedHeaders=host\u0026X-Amz-Signature=95041dfc608a81e07fe0b91d6bb44668112d057b6b6313dde6d23ea1e76c9b77",
+        #     "text_presigned_url": "https://prod-chat-kimi.tos-s3-cn-beijing.volces.com/prod-chat-kimi/cki094b3aeslglj6fo2g/2024-03-18/cnrtn82lnl9f8h6k6eq0/?X-Amz-Algorithm=AWS4-HMAC-SHA256\u0026X-Amz-Credential=AKLTYTJlNjgwMjY2ZDBkNDFiYmI5YWNiZDBlZmFmYjIzZTA%2F20240318%2Fcn-beijing%2Fs3%2Faws4_request\u0026X-Amz-Date=20240318T061352Z\u0026X-Amz-Expires=3600\u0026X-Amz-SignedHeaders=host\u0026X-Amz-Signature=c1157fd8a0b65864a89480bb9e743d48004705126a7c04c24c0e2abc15131773",
+        #     "uploaded_at": "2024-03-18T06:13:49Z",
+        #     "created_at": "2024-03-18T14:13:52.036471136+08:00",
+        #     "updated_at": "2024-03-18T14:13:52.036471136+08:00"
+        # }
 
         file_id = file_response.get("id")
 
         # 解析文件
         url = "https://kimi.moonshot.cn/api/file/parse_process"
         payload = {"ids": [file_id]}
-        resp = self.httpx_client.post(url, json=payload, headers=self.headers).text.strip('data: ')
+        resp = self.httpx_client.post(url, json=payload, headers=self.headers, timeout=180).text.strip('data: ')
         resp = json.loads(resp)
         resp['file_info'].update(file_response)
 
-        status = resp.get("status") == "parsed" and "processed"
+        logger.debug(resp)
+
+        status = resp.get("status") == "parsed" and "processed" or "error"
 
         file_object = FileObject(
             id=file_id,
             bytes=resp['file_info']['size'],
             created_at=int(time.time()),
             filename=filename,
             object='file',
             purpose="assistants",
             status=status,
             status_details=str(resp)
         )
 
         return file_object
 
+    def file_upload(self, file: Union[str, UploadFile]):
+        return self.file_extract(file)
+
 
 # 2024-03-04 09:29:24.815 | DEBUG    | __main__:f:186 - {'ids': ['cnii7t4udu62fbesjteg']}
 # data: {"event":"resp","file_info":{"id":"cnii7t4udu62fbesjteg","name":"å­å­åµæ³.pdf","type":"file","content_type":"pdf","status":"parsed","size":607093,"token_size":91753,"failed_reason":""},"id":"cnii7t4udu62fbesjteg","status":"parsed"}
 
 
 # def do_refresh_token(refresh_token):
 #     headers = {
@@ -274,49 +304,48 @@
     # print(Completions().access_token)
 
     # print(Completions().chat_id)
     t = "eyJhbGciOiJIUzUxMiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJ1c2VyLWNlbnRlciIsImV4cCI6MTcwOTgwMDIxMCwiaWF0IjoxNzA5Nzk5MzEwLCJqdGkiOiJjbmtuZjNocmRpamFpbGlkNGNqZyIsInR5cCI6ImFjY2VzcyIsInN1YiI6ImNraTA5NGIzYWVzbGdsajZmbzMwIiwic3BhY2VfaWQiOiJja2kwOTRiM2Flc2xnbGo2Zm8yZyIsImFic3RyYWN0X3VzZXJfaWQiOiJja2kwOTRiM2Flc2xnbGo2Zm8zMCJ9.fm5Hd16J3DNtmRT4zctcKrIvojEcByORFfHm2OziddOMF1dL5nqX3U9skERvF-q-QlpSpMSm8SDRVLXde1Balw"
     c = Completions(access_token=t)
     c = Completions()
 
-
-    async def f(x):
-        _ = c.create(
-            ChatCompletionRequest(
-                messages=[
-                    # {'role': 'user', 'name': '_resource', 'content': "你现在扮演的角色是GPT请牢记"},
-                    {'role': 'user', 'content': '1+1'},  # 不能有系统信息
-                    # {'role': 'user', 'content': '总结这篇文章 https://f.chatllm.vip/rag-dev/trento2013.pdf'},
-                    # {'role': 'user', 'content': '总结这篇文章'},
-
-                ],
-                # file_ids=['cnijpe6cp7f0sq79ahtg']
-                # file_ids=['cnimvq03r076lsmj7ohg']
-            )
-        )
-
-        _ = c.acreate(
-            ChatCompletionRequest(
-                messages=[
-                    {'role': 'user', 'content': '1+1'},  # 不能有系统信息
-
-                ],
-
-            )
-        )
-        s = ""
-        async for i in _:
-            s += i.choices[0].delta.content
-            print(i.choices[0].delta.content, end='')
-
-        chat_completion.choices[0].message.content = s
-        return chat_completion
-
-
-    print(arun(f('')))
+    # async def f(x):
+    #     _ = c.create(
+    #         ChatCompletionRequest(
+    #             messages=[
+    #                 # {'role': 'user', 'name': '_resource', 'content': "你现在扮演的角色是GPT请牢记"},
+    #                 {'role': 'user', 'content': '1+1'},  # 不能有系统信息
+    #                 # {'role': 'user', 'content': '总结这篇文章 https://f.chatllm.vip/rag-dev/trento2013.pdf'},
+    #                 # {'role': 'user', 'content': '总结这篇文章'},
+    #
+    #             ],
+    #             # file_ids=['cnijpe6cp7f0sq79ahtg']
+    #             # file_ids=['cnimvq03r076lsmj7ohg']
+    #         )
+    #     )
+    #
+    #     _ = c.acreate(
+    #         ChatCompletionRequest(
+    #             messages=[
+    #                 {'role': 'user', 'content': '1+1'},  # 不能有系统信息
+    #
+    #             ],
+    #
+    #         )
+    #     )
+    #     s = ""
+    #     async for i in _:
+    #         s += i.choices[0].delta.content
+    #         print(i.choices[0].delta.content, end='')
+    #
+    #     chat_completion.choices[0].message.content = s
+    #     return chat_completion
+    #
+    #
+    # print(arun(f('')))
 
     # with timer("过期时间"):
     #     while 1:
     #
     #         try:
     #
     #             f('')
@@ -335,8 +364,8 @@
     # # async def main():
     # #     async for i in _:
     # #         yield i
     # print(type(_))
     # for i in async2sync_generator(_):
     #     print(i)
 
-    # print(Completions().file_extract('/Users/betterme/PycharmProjects/AI/ChatLLM/data/孙子兵法.pdf'))
+    print(Completions().file_extract('/Users/betterme/PycharmProjects/AI/ChatLLM/data/孙子兵法.pdf'))
```

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/moonshot_kimi.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/moonshot_kimi.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/openai_completions.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/openai_completions.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # @WeChat       : meutils
 # @Software     : PyCharm
 # @Description  : https://github.com/openai/openai-python
 # todo: 设计更加通用的兜底方案【首先得有靠谱的渠道（多个兜底渠道，作双兜底）】
 # 3.5 deepseek
 # 遇到内容审核【只要抛错就走备用】
 # 完全兼容openai 去掉无关字段
-import itertools
+# 重写支持异步
 
 from meutils.pipe import *
 from meutils.notice.feishu import send_message
 
 from openai import OpenAI, AsyncOpenAI
 from chatllm.schemas.openai_types import chat_completion_error, chat_completion_chunk_error, completion_keys
 from chatllm.schemas.openai_api_protocol import ChatCompletionRequest, UsageInfo
@@ -24,14 +24,23 @@
 send_message = partial(
     send_message,
     title="ChatCompletion主备",
     url="https://open.feishu.cn/open-apis/bot/v2/hook/e2f5c8eb-4421-4a0b-88ea-e2d9441990f2"
 )
 
 
+class MeOpenAI(OpenAI):
+    # @default_headers.default_headers.setter
+    # def default_headers(self, value):
+    #     self._default_headers = value
+    @property
+    def default_headers(self):
+        return {}
+
+
 @lru_cache()
 class Completions(object):
     cache_store = {}
 
     def __init__(self, api_key: Optional[str] = None, base_url: Optional[str] = None, **kwargs):
         self.clients = []
 
@@ -40,14 +49,16 @@
             api_key=api_key or 'sk-...',
             base_url=base_url or 'https://api.githubcopilot.com',
             default_headers={'Editor-Version': 'vscode/1.85.1'},
             max_retries=0,
         )
         # 如果这一步就报错呢
         self.client = OpenAI(**params)  # todo: 异步
+        if api_key and api_key.startswith("http"):  # 白嫖
+            self.client = MeOpenAI(base_url=api_key)
 
         self.backup_client = OpenAI(
             api_key=os.getenv("BACKUP_API_KEY"),
             base_url=os.getenv("OPENAI_BASE_URL", "https://api.chatllm.vip/v1"),
             max_retries=1,  # 如果还有采用直连
         )
```

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/openai_completions_bk.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/openai_completions_bk.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/smooth.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/smooth_.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/completions/spark.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/spark.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/decorators/common.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/decorators/common.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/document_loaders/FilesLoader.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/document_loaders/FilesLoader.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/document_loaders/__init__.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/document_loaders/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 # @Time         : 2023/6/30 18:47
 # @Author       : betterme
 # @WeChat       : meutils
 # @Software     : PyCharm
 # @Description  :
 
 
-from chatllm.llmchain.document_loaders.text import TextLoader
-from chatllm.llmchain.document_loaders.pdf import PyMuPDFLoader
-from chatllm.llmchain.document_loaders.docx import Docx2txtLoader
-from chatllm.llmchain.document_loaders.image import UnstructuredImageLoader  # 依赖 nltk
-
-from chatllm.llmchain.document_loaders.file import FileLoader
-from chatllm.llmchain.document_loaders.FilesLoader import FilesLoader
+# from chatllm.llmchain.document_loaders.text import TextLoader
+# from chatllm.llmchain.document_loaders.pdf import PyMuPDFLoader
+# from chatllm.llmchain.document_loaders.docx import Docx2txtLoader
+# from chatllm.llmchain.document_loaders.image import UnstructuredImageLoader  # 依赖 nltk
+#
+# from chatllm.llmchain.document_loaders.file import FileLoader
+# from chatllm.llmchain.document_loaders.FilesLoader import FilesLoader
```

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/document_loaders/docx.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/document_loaders/docx.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/document_loaders/file.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/document_loaders/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # @Description  :
 
 from meutils.pipe import *
 from langchain.text_splitter import *
 from langchain_community.document_loaders import CSVLoader, UnstructuredFileLoader
 from langchain_community.document_loaders.base import BaseLoader
 from langchain.schema import Document
-from chatllm.llmchain.document_loaders import TextLoader, Docx2txtLoader, PyMuPDFLoader
+from chatllm.llmchain.document_loaders.FilesLoader import TextLoader, Docx2txtLoader, PyMuPDFLoader
 
 
 class FileLoader(BaseLoader):
     """
         loader = FilesLoader('data/古今医统大全.txt')
         docs = loader.load_and_split()
     """
```

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/document_loaders/image.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/document_loaders/image.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/document_loaders/pdf.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/document_loaders/pdf.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/document_loaders/text.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/document_loaders/text.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/embeddings/ApiEmbeddings.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/embeddings/ApiEmbeddings.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/embeddings/DashScopeEmbeddings.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/embeddings/DashScopeEmbeddings.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/embeddings/HuggingFaceEmbeddings.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/embeddings/HuggingFaceEmbeddings.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/embeddings/OpenAIEmbeddings.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/embeddings/OpenAIEmbeddings.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/embeddings/XunfeiEmbedding.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/embeddings/XunfeiEmbedding.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/embeddings/openai_embeddings.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/embeddings/openai_embeddings.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 class Embeddings(object):
     def __init__(self, api_key: Optional[str] = None, base_url: Optional[str] = None, **kwargs):
         # 需要兜底的模型
         params = dict(
             api_key=api_key or 'sk-...',
             base_url=base_url or 'https://api.githubcopilot.com',
             default_headers={'Editor-Version': 'vscode/1.85.1'},
+            max_retries=0,
         )
         self.client = OpenAI(**params)  # todo: 异步
 
         self.backup_client = OpenAI(
             api_key=os.getenv("BACKUP_API_KEY"),
             base_url=os.getenv("OPENAI_BASE_URL", "https://api.chatllm.vip/v1")
         )
@@ -101,11 +102,28 @@
              'Show HN: Geppetto, an open source AI companion for your Slack teams',
              "Deeptechia/geppetto: Geppetto: Advanced Slack bot integrating OpenAI's ChatGPT-4 and DALL-E-3 for interactive AI conversations and image generation. Enhances Slack communication with automated greetin",
              'Geppetto is an open source Slack App that allows users to use ChatGPT inside their workspace, written in Python and easy to tinker and fork.',
              'The project is available on GitHub at https://github.com/Deeptechia/geppetto and the first public release can be found at https://deeptechia.io/blog/geppetto-ai-companion-for-slack',
              'Sámi National Day', 'Sámi National Day',
              'The Sámi National Day is on February 6, commemorating the first Sámi congress held in 1917 in Trondheim, Norway, where Norwegian and Swedish Sámi came together to address common problems.']
 
-    # api_key = Completions.get_access_token(None)
-    # _ = Embeddings(api_key=api_key).create(input=input[:3], model='text-embedding-ada-002')
+    from asgiref.sync import sync_to_async
 
-    print(len(input))
+
+    @sync_to_async(thread_sensitive=False)
+    def get_access_token(k):
+        return Completions.get_access_token(k)
+    #
+    with timer(1):
+        api_key = Completions.get_access_token('ccu_')
+        # api_key = Completions.get_access_token('ccu_')
+    #
+    # with timer(11):
+    #     api_key = Completions.get_access_token('ccu_1')
+    #     api_key = Completions.get_access_token('ccu_2')
+
+    # with timer(2):
+    #     api_key = arun(get_access_token('ccu_11'))
+    #
+    # with timer(22):
+    #     api_key = get_access_token('ccu_11')
+    #     api_key = get_access_token('ccu_111')
```

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/llms/__init__.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/llms/basellm.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/llms/basellm.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/llms/chatglm.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/llms/chatglm.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/llms/ernie.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/llms/ernie.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/llms/hunyuan.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/llms/hunyuan.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/llms/kimi.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/llms/kimi.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/llms/spark.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/llms/spark.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/prompts/kb.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/prompts/kb.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/prompts/ocr.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/prompts/ocr.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/prompts/prompt_templates.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/prompts/prompt_templates.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/prompts/prompt_watch.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/prompts/prompt_watch.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/prompts/rag.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/prompts/rag.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/prompts/格式化.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/prompts/格式化.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/textsplitter/ali_text_splitter.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/textsplitter/ali_text_splitter.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/textsplitter/chinese_text_splitter.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/textsplitter/chinese_text_splitter.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/textsplitter/zh_title_enhance.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/textsplitter/zh_title_enhance.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/utils/common.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/utils/common.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/vectorstores/DocArrayInMemorySearch.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/vectorstores/DocArrayInMemorySearch.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/vectorstores/ElasticsearchStore.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/vectorstores/ElasticsearchStore.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/vectorstores/FAISS.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/vectorstores/FAISS.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/vectorstores/Milvus.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/vectorstores/Milvus.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/vectorstores/Usearch.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/vectorstores/Usearch.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/vectorstores/VectorRecordManager.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/vectorstores/VectorRecordManager.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/vectorstores/__init__.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/vectorstores/__init__.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/vectorstores/base.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/vectorstores/base.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llmchain/vectorstores/index_utils.py` & `chatllm-2024.4.3.18.28.17/chatllm/llmchain/vectorstores/index_utils.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llms/__init__.py` & `chatllm-2024.4.3.18.28.17/chatllm/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llms/chatglm.py` & `chatllm-2024.4.3.18.28.17/chatllm/llms/chatglm.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llms/chatgpt.py` & `chatllm-2024.4.3.18.28.17/chatllm/llms/chatgpt.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llms/demo.py` & `chatllm-2024.4.3.18.28.17/chatllm/llms/demo.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/llms/llama.py` & `chatllm-2024.4.3.18.28.17/chatllm/llms/llama.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/prompts/common.py` & `chatllm-2024.4.3.18.28.17/chatllm/prompts/common.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/schemas/4v.py` & `chatllm-2024.4.3.18.28.17/chatllm/schemas/4v.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/schemas/embedding.py` & `chatllm-2024.4.3.18.28.17/chatllm/schemas/embedding.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/schemas/kimi/protocol.py` & `chatllm-2024.4.3.18.28.17/chatllm/schemas/kimi/protocol.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/schemas/kimi/state.json` & `chatllm-2024.4.3.18.28.17/chatllm/schemas/kimi/state.json`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/schemas/openai_api_protocol.py` & `chatllm-2024.4.3.18.28.17/chatllm/schemas/openai_api_protocol.py`

 * *Files 12% similar despite different names*

```diff
@@ -72,15 +72,18 @@
     """
     prompt_filter_result.content_filter_results
     choice.content_filter_results
 
     todo: ['messages', 'model', 'frequency_penalty', 'function_call', 'functions', 'logit_bias', 'logprobs', 'max_tokens', 'n', 'presence_penalty', 'response_format', 'seed', 'stop', 'stream', 'temperature', 'tool_choice', 'tools', 'top_logprobs', 'top_p', 'user']
     """
     model: str = ''  # "gpt-3.5-turbo-file-id"
-    messages: Union[str, List[Dict[str, str]]] = [{'role': 'user', 'content': 'hi'}]
+
+    # content: [{"type": "text", "text": "hi"}]
+    messages: Union[str, List[Dict[str, Any]]] = [{'role': 'user', 'content': 'hi'}]
+
     temperature: Optional[float] = 1
     top_p: Optional[float] = 1.0
     n: Optional[int] = 1
     max_tokens: Optional[int] = None
     stop: Optional[Union[str, List[str]]] = None
     stream: Optional[bool] = False
     presence_penalty: Optional[float] = 0.0
@@ -90,20 +93,50 @@
     # 1106
     response_format: Optional[Any] = None
     function_call: Optional[Any] = None
 
     # 拓展字段
     additional_kwargs: Optional[Dict[str, Any]] = Field(default_factory=dict)
 
+    refs: List[str] = []
     file_ids: List[str] = []
 
-    # kimi
-    refs: List[str] = []
+    search: Optional[bool] = None
     use_search: Optional[bool] = None  # 自动推断联网
 
+    # glm
+    assistant_id: str = ""
+    conversation_id: str = ""  # kimi、glm4
+
+    # 模型水印
+    watermark: Optional[str] = ""
+
+    # 我是Kimi，由月之暗面科技有限公司开发的人工智能助手
+
+    # todo：设计apikey入参
+    # rag
+
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+
+        if file_ids := self.file_ids or self.refs:
+            self.file_ids = file_ids
+            self.refs = file_ids
+
+        if search := self.use_search or self.search:
+            self.search = search
+            self.use_search = search
+
+        # glm
+        self.assistant_id = self.assistant_id or "65940acff94777010aa6b796"
+
+        # if isinstance(self.messages[-1].get('content'), list): # [{'type': 'text', 'text': 'hi'}]
+        #     part_content = self.messages[-1]['content'][0]
+        #
+
     model_config = {
         "json_schema_extra": {
             "examples": [
                 {
                     "model": "gpt-3.5-turbo",
                     "messages": [
                         {
@@ -150,20 +183,17 @@
                     "file_ids": ["cn2a0s83r07am0knkeag", "cn2a3ralnl9crebipv4g"]
                 }
 
             ]
         }
     }
 
-    def __init__(__pydantic_self__, **data):
-        super().__init__(**data)
-        if __pydantic_self__.file_ids or __pydantic_self__.refs:
-            common_value = __pydantic_self__.file_ids or __pydantic_self__.refs
-            __pydantic_self__.file_ids = common_value
-            __pydantic_self__.refs = common_value
+
+class ChatCompletionRequestForSuno(BaseModel):
+    pass
 
 
 class ChatMessage(BaseModel):
     role: str
     content: str
     #
     function_call: Optional[Any] = None
@@ -326,13 +356,45 @@
        'usage': {'completion_tokens': 188,
                  'prompt_tokens': 1115,
                  'total_tokens': 1303}}
 
 if __name__ == '__main__':
     import openai
     import langchain
+
     # openai.types
     req1 = ChatCompletionRequest(file_ids=["1"])
     print(req1.file_ids, req1.refs)  # ['1'] ['1']
 
     req2 = ChatCompletionRequest(refs=["2"])
     print(req2.file_ids, req2.refs)  # ['2'] ['2']
+
+    req1 = ChatCompletionRequest(search=True)
+    print(req1.use_search, req1.search)  # ['1'] ['1']
+
+    req1 = ChatCompletionRequest(search=False)
+    print(req1.use_search, req1.search)  # ['1'] ['1']
+
+    req2 = ChatCompletionRequest(use_search=False)
+    print(req2.use_search, req2.search)  # ['1'] ['1']
+
+    data = {
+        "stream": True,
+        "temperature": 0.8,
+        "model": "kimi-all",
+        "messages": [
+            {
+                "role": "system",
+                "content": "Hi，我是 火哥AI助手～\\n很高兴遇见你！你可以随时把网址🔗或者文件📃发给我，我来帮你看看\\n Current date: 2024-03-11"
+            },
+            {
+                "role": "user",
+                "content": [
+                    {
+                        "type": "http://ai.chatfire.cn/files/document/绩效面谈表-模版-nine-1710139239100-nine-66b3829d5.pdf text"
+                    }
+                ]
+            }
+        ]
+    }
+
+    print(type(ChatCompletionRequest(**data).messages[-1]['content']))
```

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/schemas/openai_types.py` & `chatllm-2024.4.3.18.28.17/chatllm/schemas/openai_types.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 completion_keys = get_function_params()
 
 
 class SpeechCreateRequest(BaseModel):
     input: str
     model: str = 'tts'
     voice: str = "alloy"
-    response_format: Literal["mp3", "opus", "aac", "flac"] = "mp3"
+    response_format: Literal["mp3", "opus", "aac", "flac", "wav", "pcm"] = "mp3"
     speed: float = 1
 
 
 # todo: 结构体
 chat_completion = {
     "id": "chatcmpl-id",
     "object": "chat.completion",
@@ -94,28 +94,50 @@
 chat_completion_per = chat_completion.model_copy(deep=True)
 chat_completion_per.choices[0].message.content = "按次收费"
 chat_completion_per.choices[0].finish_reason = "stop"
 chat_completion_chunk_ppu = chat_completion_chunk.model_copy(deep=True)
 chat_completion_chunk_ppu.choices[0].delta.content = "按次收费"
 
 
-
-
-
 class ImageRequest(BaseModel):
     prompt: str
     model: str = 'dall-e-3'
     n: int = 1
     quality: str = 'standard'
     response_format: Literal["url", "b64_json"] = "url"
     size: Literal["256x256", "512x512", "1024x1024", "1792x1024", "1024x1792"] = '1792x1024'  # 测试默认值
     style: Literal["vivid", "natural"] = "vivid"
     extra_body: dict = {}
 
 
+# ChatCompletionUserMessageParam
+class ChatCompletionContentTextPart(BaseModel):
+    """A part of the content of a message."""
+    text: str
+    """The text of the content part."""
+    type: Literal["text", "image", "video", "audio", "file"]
+    """The type of the content part."""
+
+
+class ChatCompletionContentImagePart(BaseModel):
+    """A part of the content of a message."""
+    text: str
+    """The text of the content part."""
+    type: Literal["text", "image", "video", "audio", "file"]
+    """The type of the content part."""
+
+
+class ChatCompletionUserMessage(BaseModel):
+    role: str = "user"
+    """The role of the messages author, in this case `user`."""
+
+    # content: Union[str, List[ChatCompletionContentPart]]
+    """The contents of the user message."""
+
+
 if __name__ == '__main__':
     # data = {"stream": True, "model": "gpt-3.5-turbo", "messages": [{"role": "user", "content": "你好"}]}
     # print(ChatCompletionRequest(request=data).request)
     # print(chat_completion_error)
     # print(chat_completion_slogan)
 
     # print(chat_completion_chunk_stop)
```

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/serve/_openai_api_server.py` & `chatllm-2024.4.3.18.28.17/chatllm/serve/_openai_api_server.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/serve/app.py` & `chatllm-2024.4.3.18.28.17/chatllm/serve/app.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/serve/constants.py` & `chatllm-2024.4.3.18.28.17/chatllm/serve/constants.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/serve/openai_api_server.py` & `chatllm-2024.4.3.18.28.17/chatllm/serve/openai_api_server.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/utils/common.py` & `chatllm-2024.4.3.18.28.17/chatllm/utils/common.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/utils/gpu_utils.py` & `chatllm-2024.4.3.18.28.17/chatllm/utils/gpu_utils.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/utils/nbce.py` & `chatllm-2024.4.3.18.28.17/chatllm/utils/nbce.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/utils/nbce_test.py` & `chatllm-2024.4.3.18.28.17/chatllm/utils/nbce_test.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/utils/openai_utils.py` & `chatllm-2024.4.3.18.28.17/chatllm/utils/openai_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # @Project      : AI.  @by PyCharm
 # @File         : ppu_utils
 # @Time         : 2024/1/8 16:46
 # @Author       : betterme
 # @WeChat       : meutils
 # @Software     : PyCharm
 # @Description  : 按次计费
+import time
 
 import openai
 from openai import OpenAI
 
 from meutils.pipe import *
 from chatllm.schemas.openai_types import completion_keys
 from chatllm.schemas.openai_api_protocol import ChatCompletionRequest
@@ -53,48 +54,54 @@
     :param response:
     :param redirect_model: request.model
     :param n:
     :return:
     """
     from sse_starlette import EventSourceResponse
 
-    # logger.debug(response)
+    # logger.debug(type(response))
 
     if isinstance(response, ChatCompletion):
         response.model = redirect_model or response.model
 
         response.usage.prompt_tokens = int(response.usage.prompt_tokens * n)
         completion_tokens = response.usage.completion_tokens or len(response.choices[0].message.content)
         response.usage.completion_tokens = int(completion_tokens * n)
         response.usage.total_tokens = response.usage.prompt_tokens + response.usage.completion_tokens
 
         return response
 
     def do_chunk(chunk):
         chunk: ChatCompletionChunk
         chunk.model = redirect_model or chunk.model
-        if chunk.choices:
+
+        # logger.debug(chunk.choices)
+
+        if chunk.choices and chunk.choices[0].delta.content:  # 跳过首行空值
             if chunk.choices[0].finish_reason == "stop":
                 chunk.choices[0].delta.content = ""  # "delta":{} "delta":{"content":""}
                 yield chunk.model_dump_json()
-                yield "[DONE]"  # 兼容标准格式
+                # yield "[DONE]"  # 兼容标准格式
                 return
             else:
                 yield chunk.model_dump_json()
 
+
     if inspect.isasyncgen(response) or isinstance(response, openai.AsyncStream):
         async def gen():
             async for chunk in response:
                 for chunk in do_chunk(chunk):
                     yield chunk
+            yield "[DONE]"  # 兼容标准格式
 
     else:
         def gen():
             for chunk in response:
                 for chunk in do_chunk(chunk):
                     yield chunk
+            yield "[DONE]"  # 兼容标准格式
 
     return EventSourceResponse(gen(), ping=10000)  # sse_response
 
 
 if __name__ == '__main__':
     print(per_create())
```

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/webui/!.png` & `chatllm-2024.4.3.18.28.17/chatllm/webui/!.png`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/webui/bot.png` & `chatllm-2024.4.3.18.28.17/chatllm/webui/bot.png`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/webui/chat.py` & `chatllm-2024.4.3.18.28.17/chatllm/webui/chat.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/webui/chat_copilot.py` & `chatllm-2024.4.3.18.28.17/chatllm/webui/chat_copilot.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/webui/chatbase.py` & `chatllm-2024.4.3.18.28.17/chatllm/webui/chatbase.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/webui/chatbook.png` & `chatllm-2024.4.3.18.28.17/chatllm/webui/chatbook.png`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/webui/chatbook.py` & `chatllm-2024.4.3.18.28.17/chatllm/webui/chatbook.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/webui/chatbot.png` & `chatllm-2024.4.3.18.28.17/chatllm/webui/chatbot.png`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/webui/chatbot.py` & `chatllm-2024.4.3.18.28.17/chatllm/webui/chatbot.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/webui/chatfile.py` & `chatllm-2024.4.3.18.28.17/chatllm/webui/chatfile.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/webui/chatfile_nesc.py` & `chatllm-2024.4.3.18.28.17/chatllm/webui/chatfile_nesc.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/webui/chatfile_nesc_last.py` & `chatllm-2024.4.3.18.28.17/chatllm/webui/chatfile_nesc_last.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import streamlit as st
 # st.set_page_config('🔥ChatLLM', layout='wide', initial_sidebar_state='collapsed')
 
 
 
 from chatllm.llmchain import init_cache
 from chatllm.llmchain.applications import ChatFile
-from chatllm.llmchain.document_loaders import FileLoader
+from chatllm.llmchain.document_loaders.file import FileLoader
 from chatllm.llmchain.embeddings import OpenAIEmbeddings
 from meutils.serving.streamlit import hide_st_style, st_chat_message, ChatMessage
 
 from chatllm.llmchain.prompts.rag import template
 
 hide_st_style()
```

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/webui/chatfile_nesc_v1.py` & `chatllm-2024.4.3.18.28.17/chatllm/webui/chatfile_nesc_v1.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/webui/chatfile_nesc_v2.py` & `chatllm-2024.4.3.18.28.17/chatllm/webui/chatfile_nesc_v2.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/webui/chatfile_v0.1.py` & `chatllm-2024.4.3.18.28.17/chatllm/webui/chatfile_v0.1.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/webui/chatmind.py` & `chatllm-2024.4.3.18.28.17/chatllm/webui/chatmind.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/webui/chatpdf.py` & `chatllm-2024.4.3.18.28.17/chatllm/webui/chatpdf.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/webui/dalle.py` & `chatllm-2024.4.3.18.28.17/chatllm/webui/dalle.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/webui/demo.py` & `chatllm-2024.4.3.18.28.17/chatllm/webui/demo.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/webui/fire.png` & `chatllm-2024.4.3.18.28.17/chatllm/webui/fire.png`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/webui/gradio_ui.py` & `chatllm-2024.4.3.18.28.17/chatllm/webui/gradio_ui.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/webui/logo.png` & `chatllm-2024.4.3.18.28.17/chatllm/webui/logo.png`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/webui/nesc.jpeg` & `chatllm-2024.4.3.18.28.17/chatllm/webui/nesc.jpeg`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/webui/nice_ui.py` & `chatllm-2024.4.3.18.28.17/chatllm/webui/nice_ui.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/webui/prompt_maker.py` & `chatllm-2024.4.3.18.28.17/chatllm/webui/prompt_maker.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/webui/qa.py` & `chatllm-2024.4.3.18.28.17/chatllm/webui/qa.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/webui/user.jpg` & `chatllm-2024.4.3.18.28.17/chatllm/webui/user.jpg`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/webui/visualglm_st.py` & `chatllm-2024.4.3.18.28.17/chatllm/webui/visualglm_st.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/webui/副本人工智能咨询服务协议 汉洁 南京当月糯 20240105(1)(1).docx` & `chatllm-2024.4.3.18.28.17/chatllm/webui/副本人工智能咨询服务协议 汉洁 南京当月糯 20240105(1)(1).docx`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/webui/同程报价.xlsx` & `chatllm-2024.4.3.18.28.17/chatllm/webui/同程报价.xlsx`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/webui/规丞相.png` & `chatllm-2024.4.3.18.28.17/chatllm/webui/规丞相.png`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/webui/酒店百问百答.pdf` & `chatllm-2024.4.3.18.28.17/chatllm/webui/酒店百问百答.pdf`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/webui/附件1：东北证券股份有限公司员工合规手册（2023年12月）.doc` & `chatllm-2024.4.3.18.28.17/chatllm/webui/附件1：东北证券股份有限公司员工合规手册（2023年12月）.doc`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm/webui/附件1：东北证券股份有限公司员工合规手册（2023年12月）.docx` & `chatllm-2024.4.3.18.28.17/chatllm/webui/附件1：东北证券股份有限公司员工合规手册（2023年12月）.docx`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/chatllm.egg-info/PKG-INFO` & `chatllm-2024.4.3.18.28.17/chatllm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatllm
-Version: 2024.3.8.19.26.56
+Version: 2024.4.3.18.28.17
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: chatllm
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -43,25 +43,25 @@
 Requires-Dist: streamlit; extra == "streamlit"
 Requires-Dist: streamlit_chat; extra == "streamlit"
 Provides-Extra: rag
 Requires-Dist: redis; extra == "rag"
 Requires-Dist: minio; extra == "rag"
 Requires-Dist: faiss-cpu; extra == "rag"
 Provides-Extra: all
-Requires-Dist: streamlit_chat; extra == "all"
-Requires-Dist: fastapi; extra == "all"
-Requires-Dist: qdrant-client; extra == "all"
-Requires-Dist: openai; extra == "all"
-Requires-Dist: streamlit; extra == "all"
 Requires-Dist: pymupdf; extra == "all"
-Requires-Dist: sse_starlette; extra == "all"
-Requires-Dist: minio; extra == "all"
 Requires-Dist: sse-starlette; extra == "all"
-Requires-Dist: faiss-cpu; extra == "all"
+Requires-Dist: streamlit; extra == "all"
+Requires-Dist: sse_starlette; extra == "all"
 Requires-Dist: redis; extra == "all"
+Requires-Dist: streamlit_chat; extra == "all"
+Requires-Dist: openai; extra == "all"
+Requires-Dist: faiss-cpu; extra == "all"
+Requires-Dist: minio; extra == "all"
+Requires-Dist: qdrant-client; extra == "all"
+Requires-Dist: fastapi; extra == "all"
 
 ![image](https://img.shields.io/pypi/v/chatllm.svg) ![image](https://img.shields.io/travis/yuanjie-ai/chatllm.svg) ![image](https://readthedocs.org/projects/chatllm/badge/?version=latest)
 
 <h1 align = "center">🔥ChatLLM 基于知识库🔥</h1>
 
 <div align=center>
 <img src="data/imgs/LLM.drawio.png"/>
```

### Comparing `chatllm-2024.3.8.19.26.56/chatllm.egg-info/SOURCES.txt` & `chatllm-2024.4.3.18.28.17/chatllm.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -43,32 +43,35 @@
 chatllm/api/openai_client.py
 chatllm/api/sse_api.py
 chatllm/api/test.py
 chatllm/api/routers/__init__.py
 chatllm/api/routers/all_chat_completions.py
 chatllm/api/routers/all_chat_completions_.py
 chatllm/api/routers/api.py
+chatllm/api/routers/audio_speech.py
+chatllm/api/routers/chat_completions_copilot.py
 chatllm/api/routers/chat_completions_extra.py
+chatllm/api/routers/chat_completions_glm.py
+chatllm/api/routers/chat_completions_gptall.py
 chatllm/api/routers/chat_completions_kimi.py
 chatllm/api/routers/chat_completions_rag.py
 chatllm/api/routers/chat_completions_redirect.py
+chatllm/api/routers/chat_completions_smooth.py
+chatllm/api/routers/chat_completions_suno.py
 chatllm/api/routers/cocopilot.py
 chatllm/api/routers/demo.py
 chatllm/api/routers/embeddings.py
-chatllm/api/routers/files_minio.py
+chatllm/api/routers/files.py
 chatllm/api/routers/files_moonshot.py
+chatllm/api/routers/files_moonshot_api.py
 chatllm/api/routers/local_embeddings.py
 chatllm/api/routers/models.py
 chatllm/api/routers/smooth_completions.py
-chatllm/api/routers/speech.py
 chatllm/api/routers/utils.py
 chatllm/api/routers/chat_completions/__init__.py
-chatllm/api/routers/files/__init__.py
-chatllm/api/routers/files/files_minio.py
-chatllm/api/routers/files/files_moonshot.py
 chatllm/api/routes/__init__.py
 chatllm/api/routes/api.py
 chatllm/api/routes/base.py
 chatllm/api/routes/completions.py
 chatllm/api/routes/embeddings.py
 chatllm/api/routes/responses.py
 chatllm/applications/Question2Answer.py
@@ -85,14 +88,15 @@
 chatllm/applications/pipeline.py
 chatllm/clis/README.md
 chatllm/clis/TODO.md
 chatllm/clis/__init__.py
 chatllm/clis/cli.py
 chatllm/llmchain/TODO.md
 chatllm/llmchain/__init__.py
+chatllm/llmchain/suno.md
 chatllm/llmchain/applications/__init__.py
 chatllm/llmchain/applications/_chatbase.py
 chatllm/llmchain/applications/_chatocr.py
 chatllm/llmchain/applications/chat4all.py
 chatllm/llmchain/applications/chataudio.py
 chatllm/llmchain/applications/chatbase.py
 chatllm/llmchain/applications/chatbook.py
@@ -115,35 +119,46 @@
 chatllm/llmchain/completions/__init__.py
 chatllm/llmchain/completions/_erniebot.py
 chatllm/llmchain/completions/_hunyuan.py
 chatllm/llmchain/completions/base.py
 chatllm/llmchain/completions/chat_image.py
 chatllm/llmchain/completions/chat_tts.py
 chatllm/llmchain/completions/chatglm.py
+chatllm/llmchain/completions/chatglm_web.py
+chatllm/llmchain/completions/copilot.py
 chatllm/llmchain/completions/deepseek.py
+chatllm/llmchain/completions/demo.py
 chatllm/llmchain/completions/dify.py
 chatllm/llmchain/completions/ernie.py
 chatllm/llmchain/completions/github_copilot.py
 chatllm/llmchain/completions/github_copilot_.py
 chatllm/llmchain/completions/google_enerativeai.py
 chatllm/llmchain/completions/google_enerativeai_.py
+chatllm/llmchain/completions/gptall.py
 chatllm/llmchain/completions/groq.py
 chatllm/llmchain/completions/hunyuan.py
 chatllm/llmchain/completions/kimi.py
 chatllm/llmchain/completions/moonshot_kimi.py
 chatllm/llmchain/completions/openai_completions.py
 chatllm/llmchain/completions/openai_completions_bk.py
 chatllm/llmchain/completions/smooth.py
+chatllm/llmchain/completions/smooth_.py
 chatllm/llmchain/completions/spark.py
+chatllm/llmchain/completions/stepchat.py
+chatllm/llmchain/completions/suno.py
+chatllm/llmchain/completions/suno_.py
+chatllm/llmchain/completions/suno__.py
+chatllm/llmchain/completions/suno_api.py
 chatllm/llmchain/decorators/__init__.py
 chatllm/llmchain/decorators/common.py
 chatllm/llmchain/document_loaders/FilesLoader.py
 chatllm/llmchain/document_loaders/__init__.py
 chatllm/llmchain/document_loaders/docx.py
 chatllm/llmchain/document_loaders/file.py
+chatllm/llmchain/document_loaders/file_loader.py
 chatllm/llmchain/document_loaders/image.py
 chatllm/llmchain/document_loaders/pdf.py
 chatllm/llmchain/document_loaders/text.py
 chatllm/llmchain/embeddings/ApiEmbeddings.py
 chatllm/llmchain/embeddings/DashScopeEmbeddings.py
 chatllm/llmchain/embeddings/HuggingFaceEmbeddings.py
 chatllm/llmchain/embeddings/OpenAIEmbeddings.py
@@ -185,19 +200,21 @@
 chatllm/llms/chatgpt.py
 chatllm/llms/demo.py
 chatllm/llms/llama.py
 chatllm/prompts/__init__.py
 chatllm/prompts/common.py
 chatllm/schemas/4v.py
 chatllm/schemas/__init__.py
+chatllm/schemas/chatglm_types.py
 chatllm/schemas/embedding.py
 chatllm/schemas/kimi_types.py
 chatllm/schemas/metadata.py
 chatllm/schemas/openai_api_protocol.py
 chatllm/schemas/openai_types.py
+chatllm/schemas/suno_types.py
 chatllm/schemas/json_schema_extra/__init__.py
 chatllm/schemas/kimi/__init__.py
 chatllm/schemas/kimi/protocol.py
 chatllm/schemas/kimi/state.json
 chatllm/serve/__init__.py
 chatllm/serve/_openai_api_server.py
 chatllm/serve/app.py
@@ -218,14 +235,15 @@
 chatllm/webui/chatbase.py
 chatllm/webui/chatbook.png
 chatllm/webui/chatbook.py
 chatllm/webui/chatbot.png
 chatllm/webui/chatbot.py
 chatllm/webui/chatfile.py
 chatllm/webui/chatfile_nesc.py
+chatllm/webui/chatfile_nesc_glm_v0.1.py
 chatllm/webui/chatfile_nesc_last.py
 chatllm/webui/chatfile_nesc_v1.py
 chatllm/webui/chatfile_nesc_v2.py
 chatllm/webui/chatfile_v0.1.py
 chatllm/webui/chatmind.py
 chatllm/webui/chatpdf.py
 chatllm/webui/conf.yaml
```

### Comparing `chatllm-2024.3.8.19.26.56/clear_git_history.sh` & `chatllm-2024.4.3.18.28.17/clear_git_history.sh`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/docs/Makefile` & `chatllm-2024.4.3.18.28.17/docs/Makefile`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/docs/conf.py` & `chatllm-2024.4.3.18.28.17/docs/conf.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/docs/make.bat` & `chatllm-2024.4.3.18.28.17/docs/make.bat`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/setup.py` & `chatllm-2024.4.3.18.28.17/setup.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/tests/oneapi_test.py` & `chatllm-2024.4.3.18.28.17/tests/oneapi_test.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.3.8.19.26.56/tests/内存型.ipynb` & `chatllm-2024.4.3.18.28.17/tests/内存型.ipynb`

 * *Files identical despite different names*

